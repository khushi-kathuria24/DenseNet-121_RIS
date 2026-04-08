# DenseNet-121 for Radiology Image Annotation

## What This Project Does
This project is a proof-of-concept for automatic annotation of chest X-ray images.
It uses a DenseNet-121 based deep learning model to find and localize chest diseases in radiology images.

The model predicts disease presence and generates bounding box locations for the detected findings.

## Dataset Used
The model is trained using the NIH ChestX-ray14 dataset:
https://nihcc.app.box.com/v/ChestXray-NIHCC

Transfer learning is used with DenseNet-121 weights pretrained on ImageNet.

## Disease Classes
The project localizes these 8 classes:
- Atelectasis
- Cardiomegaly
- Effusion
- Infiltration
- Mass
- Nodule
- Pneumonia
- Pneumothorax

## Project Flow
1. Preprocess chest X-ray images.
2. Train or load the DenseNet-121 based model.
3. Predict disease probabilities.
4. Generate/localize bounding boxes for detected diseases.
5. Visualize and serve results through a Flask web interface.

## Main Tools and Libraries Used
- Python
- PyTorch and torchvision
- NumPy and SciPy
- OpenCV
- scikit-image
- matplotlib
- Flask

## Key Scripts
- Training and model logic
- Preprocessing and utility scripts
- Localization and IoU calculation scripts
- Flask app scripts for upload and result display

## Notes
- This is a research/demo style implementation.
- Reported performance in the original project context is around 75% mAP.





