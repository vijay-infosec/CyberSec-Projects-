Phishing Email Detection Using Machine Learning

This project builds and evaluates machine learning models for classifying emails as phishing or legitimate using text-based features.
The notebook includes preprocessing, feature engineering, TF-IDF vectorization, model training, evaluation, and performance visualization.

🚀 Project Overview

The goal is to detect phishing emails using supervised machine learning.
Two models were implemented:

Logistic Regression

Random Forest Classifier

Both models were trained on the CEAS 2008 spam/phishing dataset, containing 39,153 emails.

📂 Repository Structure
phishing-email-detection-ML/
│
├── notebook/
│   └── Project_619_2.ipynb          # Full ML workflow with outputs
│
├── report/
│   ├── Final_Project_Report_Team08.docx
│   ├── Project_619_22_1764986457.pdf
│
└── README.md

🧠 Methodology
✔ Data Preprocessing

Subject and body merged

Feature extraction: email_length, subject_length, sender_domain

Text cleaning (lowercase, punctuation removal, whitespace normalization)

✔ Feature Engineering

TF-IDF vectorization for text

Numerical + categorical features combined

✔ Model Training

80/20 stratified train-test split

Logistic Regression

Random Forest

✔ Evaluation Metrics

Accuracy

Precision

Recall

F1-score

Confusion Matrix

📊 Model Performance
Logistic Regression

Accuracy: 99.48%

Perfect precision, recall, and F1-score for both classes

Random Forest

Accuracy: 95.88%

Strong overall performance with slightly lower recall for phishing samples

Both results match the findings in the PDF and DOCX reports.

🔍 Notebook Preview

GitHub will automatically render all outputs from:

Confusion matrices

Classification reports

Evaluation metrics

TF-IDF statistics

Visualizations

No execution required.

▶️ Run the Notebook in Google Colab


[https://colab.research.google.com/github/USERNAME/REPO/blob/main/notebook/Project_619_2.ipynb](https://colab.research.google.com/github/vijay-infosec/phishing-email-detection-ML/blob/main/notebook/Project_619_2.ipynb
)

📑 Reports

Detailed explanation, methodology, and discussion are in:

report/Final_Project_Report_Team08.docx

report/Project_619_22_1764986457.pdf

📌 Summary

This project demonstrates the full workflow for building an email phishing detection system:

Real dataset

Text processing

Feature engineering

ML model training and evaluation

High-accuracy results

Clean documentation and reproducible notebook
