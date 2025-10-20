# 📰 Fake News Detection using Machine Learning  

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)]()  
[![Scikit-learn](https://img.shields.io/badge/ScikitLearn-ML-yellow?logo=scikit-learn)]()  
[![License](https://img.shields.io/badge/License-MIT-green.svg)]()  
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)]()  

> A complete end-to-end **Fake News Detection** system built using machine learning and NLP that classifies real and fake news articles with over 98% accuracy.

---

## 🧭 Table of Contents
- [About The Project](#about-the-project)
- [Directory Structure](#directory-structure)
- [Dataset Source](#dataset-source)
- [Model Overview](#model-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Performance](#performance)
- [Future Improvements](#future-improvements)
- [Author](#author)
- [License](#license)

---

## 📖 About The Project

Fake news spreads fast online, influencing public perception and trust.  
This project builds a **binary classifier** to automatically identify fake news articles.

### Workflow Summary
- Load and combine fake and real news datasets  
- Clean text (stopwords, punctuation, etc.)  
- Convert text into **TF–IDF feature vectors**  
- Train ML models: `Logistic Regression`, `Decision Tree`, `Random Forest`, `Gradient Boosting`  
- Evaluate and compare model performance  

---

## 🗂️ Directory Structure
Fake_news_detection/
│
├── data/
│ ├── Fake.csv
│ ├── True.csv
│
├── notebooks/
│ └── Fake_news_detection.ipynb
│
├── README.md
└── requirements.txt

text

---

## 🧩 Dataset Source

Uses two main datasets:  

- **Fake.csv** — fake or misleading articles  
- **True.csv** — verified real news  

Each entry includes the following features:
| Column | Description |
|---------|--------------|
| title   | Headline text |
| text    | Full content of article |
| subject | Topic category |
| date    | Publication date |

---

## ⚙️ Model Overview

| Model | Accuracy | Notes |
|-------|-----------|-------|
| Logistic Regression | 98.8% | Linear model, quick and efficient |
| Decision Tree | 99.4% | Handles complex relationships |
| Gradient Boosting | 99.5% | Best performing model |
| Random Forest | 99.1% | Robust, less overfitting |

---

## 📦 Installation

**Step 1:** Clone the repository  
git clone https://github.com/<your-username>/Fake_news_detection.git
cd Fake_news_detection

text

**Step 2:** Install dependencies  
pip install -r requirements.txt

text

**Step 3:** Launch Jupyter Notebook  
jupyter notebook Fake_news_detection.ipynb

text

---

## 🚀 Usage

Test the model by running the notebook cells, or try custom input:

manual_testing("The government announced a new healthcare plan today...")

text

The model will return **"Real News"** or **"Fake News"** based on its prediction.

---

## 📊 Performance

Gradient Boosting achieved:
Accuracy: 99.5%
Precision: 0.99
Recall: 1.00
F1-Score: 1.00

text

Key visualizations:
- Confusion Matrix  
- Feature Importance (TF–IDF)  
- Model Comparison Chart  

---

## 💡 Future Improvements

- 🧠 Integrate Deep Learning models (e.g., LSTM, BERT)  
- 🌐 Build a web interface using Flask or Streamlit  
- 📊 Add live news sentiment analysis  
