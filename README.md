📰 Fake News Detection Using a Neural Network

This project implements a Fake News Detection system using a Feedforward Neural Network built with PyTorch.
The model learns to classify news articles as Fake News or Real News by analyzing the text content.

The system uses TF-IDF text vectorization to convert news articles into numerical features that can be processed by a neural network.

📌 Project Overview

Fake news has become a major issue in the digital age. This project demonstrates how Machine Learning and Neural Networks can be used to automatically detect misleading or false news articles.

The model is trained on a dataset containing real news articles and fake news articles and learns patterns that distinguish them.

⚙️ Technologies Used
Python
PyTorch
Pandas
NumPy
Scikit-learn
Matplotlib
Jupyter Notebook / Google Colab

📂 Dataset

The dataset contains two files:
Fake.csv → Fake news articles
True.csv → Real news articles

Each article contains text data used for training the model.

🚀 Project Steps

The project follows 7 major steps:

Step 1 — Load and Explore the Dataset

Using Pandas, the dataset is loaded and explored.
Tasks performed:
Read the dataset
Display the first few rows
Check the number of fake vs real news samples

Step 2 — Text Preprocessing

Since neural networks cannot process raw text, the text is converted into numerical vectors.
Technique used:
TF-IDF Vectorization
This transforms each article into a numerical feature vector.

Step 3 — Split the Dataset
The dataset is split into:
80% Training Data
20% Testing Data

This allows the model to learn from training data and be evaluated on unseen data.

Step 4 — Build the Neural Network
A Feedforward Neural Network is created using PyTorch.
Architecture:
Input Layer
   ↓
128 Neurons (ReLU)
   ↓
64 Neurons (ReLU)
   ↓
Output Layer (Sigmoid)

The output layer predicts whether the news is Fake or Real.

Step 5 — Train the Model
The model is trained using:
Loss Function: Binary Cross Entropy
Optimizer: Adam
Learning Rate: 0.001
Epochs: 15

Training loss is monitored to observe learning progress.

Step 6 — Evaluate the Model
Model performance is evaluated using:
Accuracy
Confusion Matrix
Loss Visualization

This shows how well the model distinguishes fake and real news.

Step 7 — Test the Model
The trained model allows users to manually test news headlines.
Example headlines:
Scientists confirm water on Mars.
Secret government project creates invisible humans.
The model predicts whether the headline is Fake News or Real News.

📊 Example Output
STEP 7: Enter a news headline to test the model

Headline: Scientists confirm water on Mars
Prediction: Real News

💾 Model Saving
The trained model is saved as:
fake_news_model.pth

This allows the model to be reused without retraining.

📁 Project Structure
Fake-News-Detection/
│
├── Fake.csv
├── True.csv
├── fake_news_detection.ipynb
├── fake_news_model.pth
└── README.md
🎯 Learning Outcomes

This project demonstrates:

Natural Language Processing (NLP)

Text Vectorization (TF-IDF)

Neural Network Design

Model Training and Evaluation

Fake News Detection using AI

🔮 Future Improvements

Possible improvements include:

Using Deep Learning models (LSTM / Transformers)

Adding text cleaning and preprocessing

Building a web application for real-time fake news detection

Using larger and more diverse datasets
