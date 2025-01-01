# YOLOv11 Object Detection Project

This repository contains a Jupyter Notebook for implementing object detection using the YOLOv11 model. The project demonstrates the use of the ultralytics library to perform object detection tasks, leveraging GPU acceleration in a Google Colab environment.

## Features

- Custom YOLOv11 model (yolo11n.pt) for object detection.

- Integration with Google Drive for data and model storage.

- GPU-accelerated processing for fast predictions.

- Utilizes the Fridge More Food Dataset for training and evaluation.

- Detects the following food item classes: meat, milk, onion, tomato, zucchini.

## Dataset

The project uses the Fridge More Food Dataset, a comprehensive dataset containing images of various food items in a fridge. This dataset is ideal for training object detection models due to its diverse classes and annotations.

## Prerequisites

Before running the notebook, ensure you have:

A Google account to access Google Colab and Google Drive.

Python 3.7 or later.

The following Python packages (installed automatically in the notebook):

ultralytics

google.colab

Getting Started

Clone this repository or download the Yolov11.ipynb file.

Open the notebook in Google Colab.

Mount your Google Drive to access required data and save outputs.

from google.colab import drive
drive.mount('/content/drive')

Install the required dependencies:

!pip install ultralytics

Verify GPU availability:

!nvidia-smi

Download the Fridge More Food Dataset from Roboflow and load it into your Google Drive or Colab environment.

Run the YOLOv11 prediction command:

!yolo predict model=yolo11n.pt source='/path/to/your/image.jpg'

Results

The notebook processes the input images and generates predictions using the YOLOv11 model.

Outputs include labeled images with detected objects and confidence scores.

Acknowledgments

This project uses the Ultralytics implementation of YOLO. The dataset is sourced from Roboflow Universe, a platform for computer vision datasets. Special thanks to the Google Colab team for providing a free and powerful environment for machine learning.

License

This project is licensed under the MIT License. See the LICENSE file for details.
