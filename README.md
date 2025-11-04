# 🐶🐱 Cats vs Dogs Image Classifier (TensorFlow CNN)

## 📘 Overview
This project is a Convolutional Neural Network (CNN) built with TensorFlow and Keras to classify images of cats and dogs.
It includes:

 - Dataset loading and preprocessing
 - Model training and validation
 - Accuracy and loss visualization
 - Model saving and loading
 - Image prediction on new data

  Model Architecture
The CNN architecture used:
 - → Input: (150, 150, 3)
 - → Conv2D(32, 3x3) + ReLU + MaxPooling
 - → Conv2D(64, 3x3) + ReLU + MaxPooling
 - → Conv2D(128, 3x3) + ReLU + MaxPooling
 - → Flatten
 - → Dense(512) + ReLU
 - → Dense(1) + Sigmoid

This binary classifier outputs 1 for Dog and 0 for Cat.

## 📂 Project Structure
<img width="337" height="451" alt="image" src="https://github.com/user-attachments/assets/307d7b6e-88b2-4e51-93cd-64ce1e9a4d7e" />




## ⚙️ Requirements
Install the following Python packages:
pip install tensorflow matplotlib numpy


## 🚀 How to Run


Prepare dataset:
Create folders as follows:
dataset
 - traincats
 - traindogs

Place cat and dog images in their respective folders.


Train the model:
- **cats_vs_dogs.ipynb**
- The model will train for 10 epochs by default and save as cats_vs_dogs_model.h5.

Then input the path of an image when prompted.


## 📊 Training Results
The script will plot:

Training & Validation Accuracy and loss

<img width="483" height="369" alt="image" src="https://github.com/user-attachments/assets/cba597d1-8a52-4b61-9b0d-b35ac208c9b3" />

<img width="471" height="366" alt="image" src="https://github.com/user-attachments/assets/e77e30f5-06cc-445f-8644-dbf10726acd3" />



## 💾 Model Saving
- The trained model is saved automatically as:
- cats_vs_dogs_model.h5

You can reload it later with:
model = keras.models.load_model("cats_vs_dogs_model.h5")

## prediction 
<img width="470" height="496" alt="image" src="https://github.com/user-attachments/assets/d2757f24-9bcc-4a91-8c00-6593ea0c292d" />




## 🧑‍💻 Author
- Mourad sleem ibshene
- moradbshina@gmail.com


