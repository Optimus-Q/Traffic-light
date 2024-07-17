# Traffic-light detection for DMS system using YOLO V8

![Traffic Light Detection DMS](output/traffic.png)

![Traffic Light Detection DMS](output/traficlight.avi)

## Overview

This repository contains the implementation of a Traffic Light Detection Driver Monitoring System (DMS) using the YOLOv8 model. The system is designed to detect traffic lights in video feeds or images, leveraging custom-trained datasets to enhance detection accuracy and performance.

## Dataset

The custom training dataset used for this project includes a diverse set of images capturing traffic lights in different conditions and from various angles. The dataset is annotated with bounding boxes for the traffic lights, providing the necessary ground truth for training the YOLOv8 model. I used dataset from Roboflow.

## Installation

To run the Traffic Light Detection DMS system, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Optimus-Q/Traffic-light.git
   cd traffic-light-detection-dms
   ```
   
2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Download the Pretrained Model:**
   Download the pretrained YOLOv8 model weights and place them in the `models` directory.

## Usage

1. **Running the Detector:**
   To run the traffic light detection on a video feed:
   ```bash
   yolo task=detect mode=predict model=models/best.pt source=trafficlight.mp4
   ```

## Training

To train the YOLOv8 model on the custom dataset:

1. **Prepare the Dataset:**
   Ensure your dataset is structured correctly with images and corresponding annotations. Follow my blog article on this
   https://community.telemus.ai/post/36

   


