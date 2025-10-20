📰 Fake News Detection using Machine Learning
This project demonstrates how to detect fake news articles using modern machine learning models and text processing techniques in Python.
It integrates multiple classification algorithms and natural language preprocessing to differentiate between real and fake news headlines and content accurately.

📘 Project Overview
The goal of this project is to build a binary classifier that predicts whether a news article is Fake or Real.
It uses data preprocessing, text vectorization, and machine learning models to perform classification.

Workflow Summary
Load and combine “Fake” and “True” news datasets

Clean and preprocess text data (removing punctuation, URLs, stopwords)

Convert text into TF–IDF features

Train multiple classifiers:

Logistic Regression

Decision Tree Classifier

Gradient Boosting Classifier

Random Forest Classifier

Evaluate performance and compare model accuracies

Test prediction with manual user input

🧠 Models and Accuracy
Model	Accuracy	Key Features
Logistic Regression	98.8%	High performance, simple linear classifier
Decision Tree Classifier	99.4%	Handles non-linear relationships well
Gradient Boosting Classifier	99.5%	Best performing model with excellent precision and recall
Random Forest Classifier	99.1%	Robust to overfitting and good generalization performance
All models achieved over 98% accuracy, with Gradient Boosting slightly outperforming others.

🧩 Dataset
Fake.csv — contains examples of fake news articles

True.csv — contains examples of real news articles
Each entry includes a title, text body, subject, and publication date.

Dataset Preparation
Combined into a single dataset labeled:

0 → Fake news

1 → Real news

Randomly shuffled to ensure unbiased model learning.

🧹 Data Preprocessing
Key preprocessing steps included:

Removal of punctuation, URLs, and special symbols

Conversion to lowercase

Substitution of unnecessary characters using regex

Text vectorization using TfidfVectorizer (Term Frequency–Inverse Document Frequency)

Splitting data into training and testing sets (75/25)

🧪 Model Evaluation
Each model’s performance was assessed via:

Accuracy Score

Precision / Recall / F1 Score

Classification Report

Example metrics for Gradient Boosting:

text
Accuracy: 1.00
Precision: 0.99
Recall: 1.00
F1-Score: 1.00
🧍 Manual Testing
You can test individual news text snippets manually:

python
def manual_testing(news):
    testing_news = {"text": [news]}
    new_def_test = pd.DataFrame(testing_news)
    new_x_test = vectorization.transform(new_def_test["text"])
    pred = GBC.predict(new_x_test)
    return "Fake News" if pred == 0 else "Real News"
⚙️ Technologies Used
Python 3.8+

Pandas / NumPy / Seaborn / Matplotlib

Scikit-learn (LogisticRegression, DecisionTreeClassifier, GradientBoosting, RandomForest)

TF–IDF for feature extraction

Jupyter Notebook

🚀 How to Run
Clone Repository
bash
git clone https://github.com/<your-username>/Fake_news_detection.git
cd Fake_news_detection
Install Dependencies
bash
pip install -r requirements.txt
Run the Notebook
bash
jupyter notebook Fake_news_detection.ipynb
🧾 Results
✅ High prediction accuracy (99%)
✅ Reliable model comparison
✅ Easy-to-use manual testing section

📈 Future Improvements
Implement deep learning models (LSTM / BERT)

Deploy via Flask streamlit app

Build an interactive web interface

🤝 Contributing
Contributions, issues, and feature requests are welcome!
Fork the repo and submit a pull request.

🧑‍💻 Author
[Your Name]
Full Stack Developer | Machine Learning Enthusiast
📧 Email: your-email@example.com
🌐 GitHub: github.com/your-username
