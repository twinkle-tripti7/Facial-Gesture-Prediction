# Facial-Gesture-Prediction

🚀 Project Overview
This project uses Convolutional Neural Networks (CNNs) to classify facial gestures based on image data. The model is trained on a dataset of facial expressions and gestures, performing classification into different categories such as smiling, neutral, surprised, mouth open, etc.

The model is built using TensorFlow and Keras, with data augmentation applied to improve generalization. The trained model can be used to predict expressions from images or real-time webcam input using OpenCV.

🛠 Features
Image Classification: Recognizes different facial gestures from images.
Deep Learning Model: Uses a CNN with multiple Conv2D, BatchNormalization, MaxPooling, and Dense layers.
Data Augmentation: Improves model performance with rotation, zoom, width/height shift, and horizontal flip.
Performance Monitoring: Includes validation accuracy, loss metrics, and confusion matrix visualization.
Real-Time Prediction: Supports live webcam-based gesture detection using OpenCV.
📂 Dataset & Preprocessing
Dataset is stored in the gestures/ directory, structured as:
bash
Copy
Edit
/gestures
  /smile
  /neutral
  /surprised
  /mouth_open
Images are resized to 64x64 pixels and normalized (rescale=1.0/255.0).
Data is split (80-20) for training and validation.


🏗 Model Architecture
3 Convolutional Layers with ReLU activation and MaxPooling
Batch Normalization to stabilize training
Fully Connected Layers with Dropout (50% dropout rate)
Softmax Output Layer for multi-class classification
Optimizer: Adam (learning_rate=0.0001)
Loss Function: Categorical Crossentropy
