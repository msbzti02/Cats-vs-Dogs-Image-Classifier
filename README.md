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
Input: (150, 150, 3)
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
**cats_vs_dogs.ipynb**

The model will train for 10 epochs by default and save as cats_vs_dogs_model.h5.


#### Predict a single image:
After training, run:
**cats_vs_dogs.ipynb**

Then input the path of an image when prompted.



## 📊 Training Results
The script will plot:


Training & Validation Accuracy


Training & Validation Loss


Example:
MetricDescriptionAccuracyModel’s ability to correctly classify imagesLossBinary cross-entropy loss over epochs

🐾 Example Output
When predicting an image:
Enter the path of the image: C:\projects ml\dogs and cats\traindogs\dog.5.jpg
Prediction: Dog

And the image will be displayed with the predicted label:


💾 Model Saving
The trained model is saved automatically as:
cats_vs_dogs_model.h5

You can reload it later with:
model = keras.models.load_model("cats_vs_dogs_model.h5")


📈 Future Improvements


Add data augmentation for better generalization


Integrate with a GUI or web app for real-time predictions


Experiment with transfer learning (e.g., VGG16, ResNet50)



🧑‍💻 Author
Your Name
📧 [your.email@example.com]
💻 [GitHub Profile Link]

# My Project Title
## Overview
### Features
#### Installation
##### Example Code
###### Notes
