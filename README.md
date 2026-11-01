# object-detection-using-yolov3
Implementation of YOLOv3 using TensorFlow and OpenCV for real-time object detection, bounding box prediction, and multi-class object recognition.
# Object Detection Using YOLOv3 and TensorFlow

## Project Overview

This project implements an object detection system using YOLOv3 (You Only Look Once), a deep learning-based object detection algorithm.

The model identifies multiple objects in an image, predicts their class labels, and locates them using bounding boxes. The implementation uses the Darknet-53 backbone and pretrained YOLOv3 weights trained on the COCO dataset.

## Technologies Used

- Python
- TensorFlow
- Keras
- OpenCV
- NumPy
- Matplotlib
- YOLOv3
- Google Colab / Jupyter Notebook

## Key Features

- Detects multiple objects within a single image.
- Uses the Darknet-53 backbone for feature extraction.
- Supports multi-scale object detection.
- Predicts object classes and bounding box coordinates.
- Uses anchor boxes for object localization.
- Applies Non-Maximum Suppression (NMS) to eliminate overlapping detections.
- Visualizes detected objects with bounding boxes and confidence scores.

## Model Architecture

The project uses the YOLOv3 architecture, consisting of:

- **Darknet-53 Backbone:** Extracts important visual features from input images.
- **Detection Heads:** Generate predictions at three different scales.
- **Anchor Boxes:** Help detect objects of different sizes.
- **Non-Maximum Suppression:** Removes redundant bounding box predictions.

## Implementation Workflow

1. Import the required libraries and configure the YOLOv3 parameters.
2. Define anchor boxes, masks, and COCO class labels.
3. Load pretrained Darknet weights.
4. Build the Darknet convolutional and residual blocks.
5. Construct the YOLOv3 backbone and detection heads.
6. Generate bounding box predictions.
7. Apply confidence filtering and Non-Maximum Suppression.
8. Run inference on input images and visualize the detected objects.

## Model Details

| Component | Details |
|---|---|
| Detection algorithm | YOLOv3 |
| Backbone | Darknet-53 |
| Framework | TensorFlow / Keras |
| Pretrained weights | Darknet YOLOv3 |
| Dataset classes | COCO (80 classes) |
| Input image size | 416 × 416 |

## Installation

Install the required dependencies:

```bash
pip install tensorflow opencv-python numpy matplotlib
```

## Execution

1. Open the notebook in Google Colab or Jupyter Notebook.
2. Install the required dependencies.
3. Download the pretrained YOLOv3 weights.
4. Initialize the model and load the weights.
5. Provide an input image.
6. Run the prediction function to detect and visualize objects.

## Learning Outcomes

This project provided practical exposure to deep learning-based computer vision, YOLOv3 architecture, convolutional neural networks, image preprocessing, object localization, and bounding box prediction.

It also helped explore TensorFlow model construction, pretrained weight loading, and object detection inference.
