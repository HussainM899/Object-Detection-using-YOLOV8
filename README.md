# YOLOv8 Object Detection

## Introduction
This notebook demonstrates object detection on images and videos using YOLO (You Only Look Once) with the Ultralytics implementation. The focus is on applying YOLOv8 for detecting various objects such as cars, trucks, and traffic lights in both static images and video streams.

## Dependencies
- Python 3.10.12
- PyTorch 2.1.0+cu121
- Ultralytics YOLOv8
- OpenCV for video processing
- Matplotlib for visualization

## Installation
Ensure Python 3.10 and PyTorch 2.1.0 with CUDA 12.1 support are installed. Install Ultralytics YOLOv8 via pip:
```bash
pip install ultralytics
```

## Usage
- **Image Detection:** Place your images in the specified directory and use the detect mode with the appropriate model.
- **Video Detection:** Provide the path to the video file. The output includes both the detected objects and their classifications.

## Features
- Object detection in images and videos
- Support for multiple object classes
- Option to save cropped detections
- Visualization of detection results

## Results
- **Image Detection:** Identified objects like persons, cars, buses, traffic lights, backpacks, and handbags with detection time averaging around 115.6ms per image.
- **Video Detection:** Detected cars, trucks, and other objects across video frames with processing speed ranging from 7.2ms to 11.6ms per frame, demonstrating the model's efficiency in real-time applications.

## Performance Metrics
- **Detection Speed:** Ranges from 7.2ms to 115.6ms depending on the complexity of the scene and the number of objects.
- **Accuracy:** Highly accurate in identifying and classifying various objects in both day and night scenes.
- **GPU Utilization:** Tested on Tesla T4 GPU with 15102MiB memory, showcasing efficient CUDA utilization for fast processing.

## Notes
- Ensure appropriate hardware (GPU) support for optimal performance.
- Model weights (e.g., yolov8s.pt) are automatically downloaded upon first use.

## Future Work
- Explore the integration of more advanced models for improved accuracy.
- Test on a broader range of video datasets including challenging weather conditions.

## Credits
Developed using the Ultralytics YOLOv8 framework. For more information, visit [Ultralytics GitHub](https://github.com/ultralytics/yolov5).

