# CIFAR-10-Object-Recognition-using-ResNet50
CIFAR-10 Image Classification Using Transfer Learning
This project implements an image classification model using a Convolutional Neural Network (CNN) enhanced with transfer learning via a pre-trained ResNet50 architecture. The goal is to accurately classify images from the CIFAR-10 dataset into 10 object categories.

📊 Dataset
The CIFAR-10 dataset consists of:
60,000 color images (32x32 pixels)
50,000 training images
10,000 test images
10 classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck

🧱 Project Structure
Data Acquisition
Dataset is downloaded via the Kaggle API (kaggle.json required).
Data Preprocessing
Image scaling to [0, 1]
Label encoding
Dataset split into training and testing sets

Model Architecture
Uses ResNet50 (pre-trained on ImageNet) without the top layer
Input images are resized from 32x32 to 224x224
Added custom fully connected layers with Dropout and BatchNormalization for classification

Model Training
Optimizer: Adam
Loss Function: categorical_crossentropy
Real-time plotting of training/validation accuracy and loss

Model Evaluation
Final evaluation on the test dataset
Performance metrics (accuracy, loss) reported

Model saved as cifar10_model.h5

Prediction Interface
User uploads an image
Image is preprocessed and passed to the trained model
Predicted class is displayed alongside the image

🧪 Sample Results
(Optional: Add a sample confusion matrix or accuracy plot here)

📦 Dependencies
Python 3
NumPy, Pandas
OpenCV (cv2)
Pillow (PIL)
Matplotlib
Scikit-learn
TensorFlow / Keras
Py7zr
Kaggle API

🚀 Usage
Setup:
Place your kaggle.json in ~/.kaggle/ or the project root
Install required dependencies (e.g., via pip install -r requirements.txt)

Run:

Open the Jupyter Notebook/Colab and execute all cells step by step

Prediction:
Use the interface to upload an image
Model will display the predicted class

🔧 Future Improvements
Hyperparameter tuning (e.g., learning rate, batch size)
Data augmentation to improve generalization
Try different architectures like MobileNetV2, EfficientNet, or ViT
Add model deployment via Flask, Streamlit, or TensorFlow.js

📁 License
This project is licensed under the MIT License. Feel free to use and modify it for your own learning or development purposes.
