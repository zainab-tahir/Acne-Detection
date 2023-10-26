# Acne-Detection
## Overview
This project focuses on detecting two types of acne: Cystic and Pustular acne using the YOLOv5 object detection framework. The system can identify and classify these acne types in images.

## Requirements
%pip install -qr /content/yolov5/requirements.txt

## Dataset
I have personally annotated and customized the acne dataset using Roboflow. "https://universe.roboflow.com/acne-detection-5ny43/acne-detection-wietx"

## Getting Started
!git clone https://github.com/ultralytics/yolov5

!python train.py --img 416 --batch 16 --epochs 100 --data /content/yolov5/data/coco128.yaml --weights yolov5m.pt --cache

!python detect.py --weights /content/yolov5/runs/train/exp/weights/best.pt --img 416 --conf 0.50 --source /content/cystic1.jpeg

## Results
![cystic0](https://github.com/zainab-tahir/Acne-Detection/assets/121153871/e702c7dd-4043-4571-8dc3-24a7b746acb9)
![cystic1](https://github.com/zainab-tahir/Acne-Detection/assets/121153871/e6ae5c5f-9032-41a4-a0fa-afbbe77ebc71)
![download2](https://github.com/zainab-tahir/Acne-Detection/assets/121153871/1d19ed50-3e23-4516-adaa-42cfa2670dab)
![F1_curve (2)](https://github.com/zainab-tahir/Acne-Detection/assets/121153871/d96360b3-8840-4f6c-865a-2f45faf2217e)
