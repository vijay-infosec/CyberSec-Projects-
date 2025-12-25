Phishing Email Detection Using Machine Learning

This project explores machine learning techniques for identifying phishing emails based on text content. The work includes data cleaning, feature engineering, TF-IDF vectorization, model training and evaluation, and a comparison of performance between Logistic Regression and Random Forest classifiers.

Project Overview

The objective is to build and evaluate models that distinguish phishing emails from legitimate ones.
The dataset used for this project is the CEAS 2008 email dataset, which contains a little over 39,000 samples.

Two supervised learning models were tested:

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
Data preprocessing

Combined email subject and body into a single text field

Extracted basic features such as subject length, email length, and sender domain

Applied standard text-cleaning steps (lowercasing, removing punctuation, etc.)

Feature Engineering

TF-IDF applied to the text component

Numerical and categorical features were merged into a single feature space

Model Training

Dataset split into training and testing sets (80/20, stratified)

Implemented Logistic Regression and Random Forest models

Evaluation

Models were assessed using:

Accuracy

Precision

Recall

F1-score

Confusion matrix

Model Performance
Logistic Regression

Accuracy: 99.48%

Very strong precision and recall for both classes

Random Forest

Accuracy: 95.88%

Good overall performance with slightly lower recall on phishing samples

These results are consistent with the analysis presented in the project report.

Notebook Preview

The notebook in this repository includes all outputs, so it can be viewed directly on GitHub without running the code.
It displays the confusion matrices, performance metrics, and intermediate steps of the workflow.

Running the Notebook in Google Colab

After uploading the repository, replace the link below with your actual GitHub path if you'd like the notebook to run in Google Colab:

https://colab.research.google.com/github/USERNAME/REPO/blob/main/notebook/Project_619_2.ipynb

Reports

The full explanation of the project, including background, methods, and discussion of results, is included in:

Final_Project_Report_Team08.docx

Project_619_22_1764986457.pdf

Summary

This project demonstrates a complete workflow for detecting phishing emails using machine learning, starting from preprocessing and feature extraction to training and evaluating two classification models. Both models performed well, with Logistic Regression showing the highest accuracy. The repository includes all code, results, and written documentation.
