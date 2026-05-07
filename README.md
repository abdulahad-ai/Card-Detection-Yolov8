[README.md](https://github.com/user-attachments/files/24541771/README.md)
# YOLOv8 Playing Card Detection

This project implements a YOLOv8-based object detection system to
identify playing cards in images. The model is trained using a custom
dataset obtained from Roboflow and is optimized with advanced data
augmentation and training strategies. After training, the model is
exported to ONNX format for efficient deployment in web and
cross-platform applications.

## Features

-   Uses YOLOv8 (You Only Look Once) for real-time object detection
-   Custom playing card dataset from Roboflow
-   Data augmentation for better generalization
-   Optimized training with AdamW optimizer
-   Model export to ONNX format for deployment
-   Compatible with Google Colab and local environments

## Technologies Used

-   Python
-   YOLOv8 (Ultralytics)
-   Roboflow
-   OpenCV
-   ONNX

## Dataset

The dataset consists of labeled images of playing cards, split into: -
Training set - Validation set - Test set

Annotations are provided in YOLOv8 format.

## Model Training

The YOLOv8 Small (yolov8s) pretrained model is fine-tuned on the playing
card dataset using: - Image size: 640x640 - Epochs: 200 - Optimizer:
AdamW - Data augmentation techniques such as rotation, scaling,
flipping, mosaic, and mixup

## Evaluation

Model performance is evaluated using: - mAP@50 - mAP@50--95

The trained model achieves strong accuracy in detecting playing cards
under varying conditions.

## Export

The best trained model is exported to ONNX format to allow: -
Cross-platform compatibility - Faster inference - Easy web and
application deployment

## Usage

1.  Install dependencies:

    ``` bash
    pip install ultralytics roboflow onnx
    ```

2.  Train the model using the provided training script.

3.  Export the trained model to ONNX.

4.  Use the ONNX model for inference or deployment.

## Applications

-   Online card games
-   Casino automation systems
-   Card recognition applications
-   Computer vision learning projects
-   Web-based AI solutions

## Author

This project was developed as a learning and implementation exercise in
computer vision and deep learning using YOLOv8.
