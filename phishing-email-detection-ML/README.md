# Phishing Email Detection Using Machine Learning

This project explores machine learning techniques for identifying phishing emails from legitimate ones.  
The notebook includes preprocessing, feature engineering, TF-IDF vectorization, model training, and evaluation.

---

## Project Overview

The goal of this project is to classify emails as phishing or legitimate using supervised learning models.  
The CEAS 2008 dataset (≈39K samples) was used.

Models implemented:
- Logistic Regression  
- Random Forest Classifier  

---

## Repository Structure

phishing-email-detection-ML/
│
├── notebook/
│ └── Project_619_2.ipynb
│
├── report/
│ ├── Final_Project_Report_Team08.docx
│ └── Project_619_22_1764986457.pdf
│
└── README.md


---

## Methodology

### 1. Data Preprocessing
- Merged email subject + body  
- Extracted features: subject_length, email_length, sender_domain  
- Lowercased text, removed punctuation and extra whitespace  

### 2. Feature Engineering
- Applied TF-IDF to text  
- Combined numerical + categorical features  

### 3. Model Training
- Stratified 80/20 train-test split  
- Trained Logistic Regression  
- Trained Random Forest  

### 4. Evaluation Metrics
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

---

## Model Performance

### Logistic Regression
- **Accuracy: 99.48%**  
- Strong precision and recall for both classes  

### Random Forest
- **Accuracy: 95.88%**  
- Good performance with slightly reduced recall for phishing samples  

---

## Notebook Preview

GitHub displays the notebook outputs directly:

- Confusion matrices  
- Classification reports  
- Evaluation metrics  
- TF-IDF vectors  

No execution is needed to view results.

---

## Run in Google Colab 

https://colab.research.google.com/github/USERNAME/REPO/blob/main/notebook/Project_619_2.ipynb


---

## Reports

Full project documentation:

- `Final_Project_Report_Team08.docx`  
- `Project_619_22_1764986457.pdf`

---

## Summary

This project demonstrates a complete ML workflow for phishing detection using text-based features.  
Both Logistic Regression and Random Forest achieved high accuracy, with Logistic Regression performing the best.  
The repository includes the full notebook, results, and written reports.




