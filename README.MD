# Recognize vehicles and human face by YOLOv8
## Introduction
This project is built to recognize vehicles (buses, cars, trucks, motorcycles) and human faces in real-world environments using [YOLOv8](https://docs.ultralytics.com/models/yolov8/) with the details is YOLOv8m and YOLOv8n-face models. By identifying and numbering the IDs of the appearing objects, the model will track the disappearance time of the object and save it to a json file.

## How to use
1. Download the source code in the repository.
2. Install all requirements libraries
3. run this code: 

```python
    python Object_Detection.py --input Your_video/mp4
```

## Features
**Vehicales Detection**: This model focuses on detecting vehicles such as motorbikes, cars, buses, trucks and numbering the IDs of the appearing objects.

**Human Face Detection**: Detect human face and assign IDs separate from vehicle IDs, and save data to json file.

**Bounding Boxes**: When detecting a vehicle or human face, the model will Bounding Boxes and assign IDs. Parameters displayed on the output include: ID of the vehicle/face in the video and the accompanying accuracy.

**Time appeared and disappeared**: The time of appearance of the vehicle/face is recorded in the json file exported with the output video.

## Requirements
* CV2
* Ultralytics.YOLO
* Json
* Collections
* Os