🌿 Plant Disease Prediction Using CNN and Flask
📌 Project Description
This project focuses on detecting plant leaf diseases using image classification with deep learning. It helps in early diagnosis of plant diseases, which is crucial for agricultural productivity and crop health. The system classifies uploaded leaf images into one of three categories: Healthy, Powdery Mildew, or Rust.

🎯 Objective
To build a web-based system that:

Automatically detects plant diseases from leaf images.

Uses a Convolutional Neural Network (CNN) for classification.

Allows users to upload leaf images via a simple web interface.

Returns the disease type (or confirms the leaf is healthy) as a prediction.

🧾 Dataset Information
Categories: Healthy, Powdery, Rust.

Structure: The dataset was divided into three main sets:

Training set

Validation set

Test set

Format: Each set contained subfolders for each disease category.

Total Samples: The images were manually organized and labeled into respective folders. The dataset was likely sourced from public plant disease datasets (e.g., PlantVillage), though the exact origin is not specified.

⚙️ Model Development
Model Type: Convolutional Neural Network (CNN).

Input Image Size: 225x225 pixels.

Training Details:

Epochs: 5

Batch Size: 32

Loss Function: Categorical Crossentropy

Optimizer: Adam

Performance Metrics: Accuracy

Augmentation Techniques:

Rescaling

Shearing

Zooming

Horizontal Flipping

The model was trained on the training dataset and validated using the validation set.

📈 Model Evaluation
Plotted training and validation accuracy across epochs to monitor performance.

Evaluated final model performance on unseen test images to ensure generalization.

💾 Model Storage
The trained model was saved in HDF5 format as model.h5.

This file was later loaded for real-time predictions within the web app.

🌐 Web Application (Flask-based)
Built using Flask, a lightweight Python web framework.

Features:

Upload functionality for leaf images.

Backend processes the image and performs prediction using the trained model.

Result (Healthy / Powdery / Rust) is displayed to the user.

Deployment Platform: Localhost (http://127.0.0.1:5000)

🛠️ Technologies Used
Python

TensorFlow / Keras – for model building and training

Flask – for web deployment

NumPy – for numerical operations

Matplotlib / Seaborn – for training visualization

PIL (Pillow) – for image handling

HTML / CSS (via templates) – for front-end of the web interface

📌 Conclusion
This project demonstrates the practical use of deep learning in agriculture, providing a simple yet effective tool for identifying plant leaf diseases. By combining CNN-based classification with a Flask web interface, the system offers a user-friendly solution for disease detection, useful for farmers, researchers, or agricultural app developers.

