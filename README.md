# 🎓 Student Dropout Prediction using Logistic Regression

![Python](https://img.shields.io/badge/Python-Data%20Science-blue)
![Project](https://img.shields.io/badge/Project-Machine%20Learning-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Level](https://img.shields.io/badge/Level-Intermediate-purple)
![Focus](https://img.shields.io/badge/Focus-Classification-yellow)

------------------------------------------------------------------------

## 👨‍💻 Author

**Ashish Jonnada** 

🎓 B.Tech CSE (AI & Data Science) — Marwadi University 

🔗 LinkedIn: [Ashish Jonnada](https://www.linkedin.com/in/jonnada-ashish) 

------------------------------------------------------------------------

## 📌 Project Overview

This project predicts whether a student is likely to drop out using a Logistic Regression model based on academic and behavioral features.

The model acts as an early warning system, helping institutions identify at-risk students and take timely intervention.

------------------------------------------------------------------------

## ⚠️ Problem Statement

Student dropout is a major issue in educational institutions. Factors such as low academic performance, poor attendance, and high stress contribute significantly to dropout risk.

This project focuses on analyzing these factors and building a predictive model to identify students at risk.

------------------------------------------------------------------------

## 🧠 Methodology

- Data understanding and imbalance handling  
- Exploratory Data Analysis  
- Feature Engineering (Effort Ratio, Stress Impact)  
- Multicollinearity removal  
- Logistic Regression model training  
- Regularization tuning (C parameter)  
- Threshold optimization  
- Evaluation and error analysis  

------------------------------------------------------------------------

## 🛠 Feature Engineering

- Effort Ratio → Study_Hours / (GPA + 1)  
- Stress Impact → Stress × (100 - Attendance)  
- Academic Risk → Removed due to multicollinearity  

------------------------------------------------------------------------

## ⚙️ Performance Tuning (Threshold Comparison)

| Threshold | Precision | Recall | F1 Score | Interpretation |
|----------|----------|--------|---------|----------------|
| 0.5 | 0.45 | 0.74 | 0.56 | High recall but too many false positives |
| 0.6 | 0.54 | 0.64 | 0.59 | Best balance |
| 0.7 | 0.62 | 0.48 | 0.54 | Misses many dropout cases |


Threshold = 0.6 was selected as it provides the best trade-off between precision and recall.

------------------------------------------------------------------------

## 📈 Model Performance

| Metric | Value |
|------|------|
| Accuracy | 0.79 |
| Precision | 0.54 |
| Recall | 0.64 |
| F1 Score | 0.59 |
| ROC-AUC | 0.82 |

------------------------------------------------------------------------

## 🔍 Confusion Matrix Analysis

The model correctly identifies most non-dropout students and captures a significant portion of dropout cases.

Some false positives are present as a trade-off, while a few dropout students are missed. Reducing false negatives is an area for improvement.

------------------------------------------------------------------------

## 📊 Key Insights

- GPA is the strongest predictor  
- Low attendance increases dropout risk  
- High stress + low attendance indicates risk  
- Effort mismatch reveals hidden patterns  
 


------------------------------------------------------------------------

## 🛠 Tools & Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook  
- Git & GitHub
------------------------------------------------------------------------
## 📁Project Structure
```
Student-Dropout-Prediction_Logistic-Regression/
├── data/
│   └── student_dropout_dataset.csv
├── notebooks/
│   └── Student-Dropout-Prediction_Logistic-Regression.ipynb
├── images/
│   ├── correlation_heatmap.png
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   └── eda_plots.png
├── README.md
```

------------------------------------------------------------------------

## 🏁 Conclusion

This project shows how Logistic Regression can predict student dropout effectively.

The model can act as an early warning system to identify at-risk students and support timely intervention.


