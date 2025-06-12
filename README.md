# Fake Job Detection System

This project uses machine learning and NLP to identify potentially fraudulent job postings based on their title and description.

## 🎯 Objective
Fake job scams are becoming increasingly common on job platforms, especially for students and freshers. This project aims to help detect these fake listings using a classification model trained on real-world data.

## 🗂️ Dataset
- Source: [Kaggle - Fake Job Postings](https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction)
- Contains 17,880 job postings with features such as job title, description, and a `fraudulent` label (0 = real, 1 = fake).

## 🛠 Tech Stack
- Python
- Pandas & NumPy
- NLTK for NLP preprocessing
- TF-IDF for feature extraction
- Logistic Regression for classification
- Matplotlib & Seaborn for evaluation visuals

## 📊 Features
- Cleaned and processed raw job titles + descriptions
- Removed stopwords and non-alphabetic tokens using NLTK
- Converted text into numerical vectors using TF-IDF
- Trained a Logistic Regression classifier to detect fraud
- Evaluated using accuracy, precision, recall, F1-score, and confusion matrix
- Tested with custom job descriptions to validate prediction

## 🚀 Example Usage
Paste a job description into the prediction function and see whether it’s real or fake.

```python
predict_fake("Remote data entry job. No experience needed. Quick money guaranteed!")
# Output: 1 (Fake)
