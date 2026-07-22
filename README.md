# COVID-19 Chest X-Ray Image Classification

### Introduction

Early and accurate diagnosis of COVID-19 is critical for effective patient management and public health response. Traditional diagnostic methods can be time-consuming or resource-constrained during peak outbreaks. 

This project aims to support healthcare professionals and radiologists by providing an automated **Computer-Aided Diagnosis (CAD)** tool that accurately detects COVID-19 signatures from RGB chest X-ray images.

### Data Overview

The dataset consists of preprocessed chest X-ray images and their corresponding target labels:

* **`CovidImages.npy`**: A NumPy binary file containing image arrays with shape **`(251, 128, 128, 3)`** — representing 251 samples, $128 \times 128$ spatial resolution, and 3 RGB color channels.
* **`CovidLabels.csv`**: Target label annotations for each image:
  * **COVID-19 (`1`)**: Radiographic evidence of COVID-19 infection.
  * **Normal (`0`)**: Healthy lungs with no symptoms or indications of pulmonary infection.

### **Data Distribution & Preprocessing**
* **Train/Val/Test Split**: Stratified split of $70\%$ training, $15\%$ validation, and $15\%$ testing sets to preserve class balance.
* **Pixel Normalization**: Scaled raw pixel intensity range from $[0, 255]$ to $[0.0, 1.0]$ by dividing by $255.0$ to optimize gradient descent stabilization.

### Features
- COVID-19 vs Normal chest X-ray classification
- Image preprocessing and normalization
- CNN model built using TensorFlow/Keras
- Model training and evaluation
- Performance visualization with accuracy and loss graphs
- Prediction on new chest X-ray images

### Technologies Used
- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- OpenCV
- Jupyter Notebook

### Dataset
The dataset contains chest X-ray images classified into two categories:
- COVID-19
- Normal

### Project Workflow
1. Import required libraries
2. Load and preprocess the dataset
3. Build the CNN model
4. Train the model
5. Evaluate model performance
6. Predict COVID-19 from new X-ray images

### Objective
To develop an AI-based diagnostic system capable of detecting COVID-19 from chest X-ray images with high accuracy, helping support faster medical diagnosis.
