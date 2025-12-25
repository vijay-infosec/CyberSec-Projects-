Phishing Email Detection Using Machine Learning

This project explores machine learning techniques for identifying phishing emails using text-based features. The notebook covers data cleaning, feature engineering, TF-IDF vectorization, model training, and evaluation.

Project Overview

The objective is to build and evaluate models that classify emails as phishing or legitimate.
The dataset used is the CEAS 2008 email dataset containing a little over 39,000 samples.

Models used:

Logistic Regression

Random Forest Classifier

Repository Structure
phishing-email-detection-ML/
│
├── notebook/
│   └── Project_619_2.ipynb
│
├── report/
│   ├── Final_Project_Report_Team08.docx
│   └── Project_619_22_1764986457.pdf
│
└── README.md

Methodology
Data Preprocessing

Combined email subject and body

Extracted subject length, email length, sender domain

Cleaned text (lowercasing, removing punctuation, trimming whitespace)

Feature Engineering

TF-IDF vectorization applied to email text

Numerical + categorical features merged

Model Training

80/20 stratified train-test split

Logistic Regression model

Random Forest Classifier

Evaluation Metrics

Accuracy

Precision

Recall

F1-score

Confusion matrix

Model Performance
Logistic Regression

Accuracy: 99.48%

High precision and recall across both classes

Random Forest

Accuracy: 95.88%

Slightly lower recall on phishing samples

Notebook Preview

GitHub renders the notebook outputs automatically.
The .ipynb file includes:

Confusion matrices

Classification reports

Evaluation metrics

TF-IDF processing steps

No execution is required to view results.

Run the Notebook in Google Colab

Replace USERNAME and REPO with your GitHub details if you want to offer a runnable version:

https://colab.research.google.com/github/USERNAME/REPO/blob/main/notebook/Project_619_2.ipynb

Reports

The full writeup is available in:

Final_Project_Report_Team08.docx

Project_619_22_1764986457.pdf

Summary

This project demonstrates a complete workflow for detecting phishing emails using machine learning.
Both Logistic Regression and Random Forest performed well, with Logistic Regression achieving the highest accuracy. The repository includes the notebook, outputs, and written reports.
