# Brain-Tumor-Detection-Segmentation-YOLOv11-SAM2
Implementing Brain Tumor Detection and Segmentation using YOLOv11 and SAM2 models. This project applies real-time object detection and precise segmentation to MRI images for accurate tumor detection. Built with Python, Ultralytics YOLOv11, and Meta AI SAM2 for medical imaging applications.
This project implements Brain Tumor Detection and Segmentation using state-of-the-art YOLOv11 (You Only Look Once version 11) and SAM2 (Segment Anything Model 2) models. The goal of this project is to apply deep learning techniques for the detection and segmentation of brain tumors in MRI images.

# Project Overview
This project utilizes two key models:

# YOLOv11: A real-time object detection model known for its speed and accuracy, used here to detect and localize brain tumors in MRI images.

# SAM2: An advanced image segmentation model by Meta AI, used to precisely segment the detected tumor regions in the image.

# Features
YOLOv11: Detects and localizes tumors in MRI images in real-time.

SAM2: Segments and isolates the tumor regions, making it suitable for medical imaging applications.

Python Implementation: The code is implemented using Python with the Ultralytics YOLOv11 and Meta AI SAM2 models.

High Accuracy: Achieved high accuracy in tumor detection and segmentation on MRI datasets.

# Technologies Used
Python: Programming language used for model development.

YOLOv11: For real-time object detection.

SAM2: For image segmentation.

Jupyter Notebook: For running experiments and model evaluations.

Google Colab: Used for cloud-based model training and inference.

# Installation
1. Clone the repository:
git clone https://github.com/QADEER-AHMED-cs/Brain-Tumor-Detection-Segmentation-YOLOv11-SAM2.git
cd Brain-Tumor-Detection-Segmentation-YOLOv11-SAM2

2. Install the required dependencies:
   pip install -r requirements.txt
Dataset
The dataset used in this project consists of MRI scans labeled with brain tumors. You can use your dataset or download publicly available MRI datasets.

# Training the Model
1. Prepare your dataset in the required format (YAML file).\
2. Run the training script:
python train.py
3. The model will be trained and saved in the runs/detect/train directory.

# Running Inference
After training, you can run inference on test images using the following command:
python detect.py --imgsz 640 --weights runs/detect/train/weights/best.pt --source test_images/

# Model Evaluation
You can evaluate the model’s performance on your test set using metrics like accuracy, precision, and IoU (Intersection over Union). The evaluation script will generate results and store them in the output directory.

