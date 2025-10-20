📰 Fake News Detection using Machine Learning
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=
[![Scikit-learn](https://img.shields.io/badge/ScikitLearn-ML-yellow?logo
[![License](https://img.shields.io/badge
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?

A complete end-to-end Fake News Detection project powered by machine learning and natural language processing (NLP), built to classify real and fake news articles with over 98% accuracy.

🧭 Table of Contents
About The Project

Directory Structure

Dataset Source

Model Overview

Installation

Usage

Performance

Future Improvements

Author

📖 About The Project
Fake news spreads quickly on the internet, influencing public opinion and generating misinformation.
This project aims to detect fake news automatically by training multiple machine learning models on real-world data.

Workflow Summary
Combine and clean real and fake news datasets

Remove punctuation, symbols, and stopwords

Convert text into numerical vectors using TF–IDF

Train and compare different models: Logistic Regression, Decision Tree, Gradient Boosting, and Random Forest

Evaluate accuracy and F1 scores

🗂️ Directory Structure
text
Fake_news_detection/
│
├── data/
│   ├── Fake.csv
│   ├── True.csv
│
├── notebooks/
│   ├── Fake_news_detection.ipynb
│
├── README.md
└── requirements.txt
🧩 Dataset Source
The project uses publicly available data:

Fake.csv – Contains fake news articles

True.csv – Contains verified real articles

Each record includes:

title → Headline of the article

text → Full article content

subject → Category or topic

date → Publication date

⚙️ Model Overview
Model	Accuracy	Description
Logistic Regression	98.8%	Linear baseline with high interpretability
Decision Tree Classifier	99.4%	Handles non-linear data well
Gradient Boosting Classifier	99.5%	Best performer with minimal overfitting
Random Forest Classifier	99.1%	Robust ensemble method
📦 Installation
Clone the repository and install dependencies.

bash
git clone https://github.com/<your-username>/Fake_news_detection.git
cd Fake_news_detection
pip install -r requirements.txt
Make sure to install Jupyter Notebook if not already:

bash
pip install notebook
🚀 Usage
Run the Jupyter notebook to train and test the models:

bash
jupyter notebook Fake_news_detection.ipynb
Try manual testing with a custom news example in the notebook:

python
manual_testing("The government announced a new healthcare plan today...")
📊 Performance
Evaluation Metrics (Gradient Boosting)
python
Accuracy: 99.5%
Precision: 0.99
Recall: 1.00
F1-score: 1.00
Visualization highlights include:

Confusion matrix of prediction classes

Feature importance plots using TF–IDF

💡 Future Improvements
Enhance with deep learning models (LSTM, BERT)

Build a real-time web application for prediction

