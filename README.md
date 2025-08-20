# Cats-Dogs-Clustering
🐱🐶 Cats vs Dogs Classification using HOG + SVM

This project implements an image classification model to distinguish between cats and dogs using Histogram of Oriented Gradients (HOG) features and a Support Vector Machine (SVM) classifier.

🚀 Features

Extracts HOG features from grayscale images

Uses GridSearchCV to find best hyperparameters for SVM

Provides classification report & accuracy

Supports custom image prediction

🛠️ Tech Stack

Python

OpenCV – Image preprocessing

scikit-image – HOG feature extraction

scikit-learn – Train/Test split, SVM, GridSearchCV

Matplotlib – Image visualization

📂 Dataset

The dataset structure used:

train/
   ├── cat/
   │     ├── cat1.jpg
   │     ├── cat2.jpg
   ├── dog/
         ├── dog1.jpg
         ├── dog2.jpg

test/
   ├── 55.jpg
   ├── 72.jpg

▶️ How It Works

Preprocessing

Convert images to grayscale

Resize to 64x64

Extract HOG features

Training

Split into train/test sets

Train SVM with different kernels (linear, rbf, poly)

Use GridSearchCV to select best parameters

Evaluation

Prints accuracy

Displays classification report

Prediction

Preprocess a custom test image

Predict whether it’s a Cat or Dog

📊 Example Output
Best Parameters: {'C': 10, 'kernel': 'rbf'}
Accuracy: 0.88
              precision    recall  f1-score   support

         cat       0.87      0.89      0.88        20
         dog       0.89      0.87      0.88        20

Predicted Label: ['dog']

▶️ Run Locally
git clone https://github.com/your-username/Cats-Dogs-Clustering.git
cd Cats-Dogs-Clustering
pip install -r requirements.txt
python main.py
