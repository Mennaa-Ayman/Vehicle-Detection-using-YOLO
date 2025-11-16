# 🚗 Vehicle-Detection-using-YOLOv8

## 📘 Overview

This project implements a **vehicle detection model** using the YOLOv8 architecture, trained on the Kaggle dataset: **Vehicle Detection — YOLO v8 by alkan erturan**

The goal is to **recognize** and **localize** vehicles such as cars, trucks, buses and motorbikes by drawing **bounding boxes** and **class labels** around them.


## ⚙️ Training the model 
```
from ultralytics import YOLO
model = YOLO("yolov8s.pt")

train_results = model.train(
    data=yaml_dir,  
    epochs=10,  
    imgsz=640,  
    device="cpu", 
)
```
## 📊 Evaluation
| Metric       | Value   |
| ------------ | ------- |
| mAP@0.5      | **76.8%** |
| mAP@0.5:0.95 | **60.9%** |
| Precision    | **76.8%** |

## Results
<p align="center"> <<img width="1118" height="545" alt="image" src="https://github.com/user-attachments/assets/a27ea1b1-ac22-4a54-8c0c-42c241d8ec94" /> </p>

## 📦 Dependencies
```
Python 3.8+
ultralytics
opencv-python
numpy
matplotlib
``` 
**Install YOLOv8:**

`pip install ultralytics`
