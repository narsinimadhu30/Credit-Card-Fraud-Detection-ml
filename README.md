# **Credit Card Fraud Detection using Machine Learning**



&nbsp; Detecting fraudulent transactions in highly imbalanced financial data using robust ML techniques.





## Project Overview



Credit card fraud is a major financial threat worldwide. Fraudulent transactions cause billions of dollars in losses every year.



The goal of this project is to build a **machine learning model** that can accurately detect fraudulent credit card transactions while minimizing false alarms.



Since fraud cases are **extremely rare (only 0.172%),** this is a classic **imbalanced classification problem** - making it both challenging and realistic.





## Problem Statement



Credit card companies must detect fraudulent transactions quickly so customers are not charged for purchases they never made.



* Total transactions: **284,807**
* 
* Fraud transactions: **492**
* 
* Fraud percentage: **0.172%**
* 
* Highly imbalanced dataset





If we simply predict **"Not Fraud"** for every transaction, we get **99.8% accuracy** - but the model becomes useless.



&nbsp;

Therefore, this project focuses on using **better evaluation metrics** suitable for imbalanced data such as:



* Precision
* Recall
* F1 Score
* AUPRC (Area Under Precision-Recall Curve)
* Average Precision Recall Score (APRS)





## Dataset Information

**Dataset link** :- https://drive.google.com/drive/folders/1O-tkKRSVTOwaFxk699Mz9DhwbJyfz6hV?usp=sharing

* Transactions made in **September 2013**
* European cardholders
* Duration: 2 days of transactions
* Source: Research collaboration between Worldline \& ULB Machine Learning Group





## Features



| Feature  | Description                            |

| -------- | -------------------------------------- |

| V1 – V28 | PCA-transformed anonymized features    |

| Time     | Seconds elapsed between transactions   |

| Amount   | Transaction amount                     |

| Class    | Target variable (0 = Legit, 1 = Fraud) |



⚠️ Due to confidentiality, original feature names are not available.







**## What I Performed in This Project**



## Data Understanding & Exploration



* Checked class imbalance
* Analyzed fraud vs non-fraud distribution
* Studied transaction amount patterns





## Data Preprocessing



* **Feature scaling (StandardScaler)**
* Train-test split
* Handled class imbalance





## Model Building



Implemented multiple models:



* Logistic Regression
* Decision Tree
* Random Forest





## Handling Imbalance



Used techniques such as:



* Synthetic Minority Over-sampling Technique(SMOTE)
* Evaluation using Precision-Recall metrics





## Model Evaluation



Since accuracy is misleading in imbalanced datasets, the following metrics **(Classification Report)** were used:



* Precision
* Recall
* F1 Score
* ROC-AUC
* **Precision-Recall Curve (AUPRC)**





## Model Performance (Example Summary)



| Metric                        | Score                                  |

| ----------------------------- | -------------------------------------- |

| Accuracy                      | ~97%                                   |

| Recall (Fraud Detection Rate) | High (Focused on catching fraud)       |

| Precision                     | Moderate (Reduced false alarms)        |

| F1 Score                      | Balanced performance                   |

| AUPRC                         | Strong performance for imbalanced data |



The model prioritizes high recall, ensuring most fraudulent transactions are detected.





## Tech Stack



* Python
* Pandas
* NumPy
* Matplotlib \& Seaborn
* Scikit-learn





## Research & References



This dataset is part of published research work by **ULB Machine Learning Group**.



If using this dataset for research, please cite:



1. Dal Pozzolo et al., IEEE CIDM 2015
2. Expert Systems with Applications (2014)
3. IEEE Transactions on Neural Networks (2018)
4. Information Sciences (2019)





## Future Improvements



* Implement **SMOTE** for **synthetic oversampling**
* Try XGBoost / LightGBM
* Deploy model with Flask / FastAPI
* Real-time fraud detection simulation
* Cost-sensitive learning implementation





## Conclusion



This project demonstrates how to build a **real-world fraud detection system** in a highly imbalanced environment.



Instead of focusing only on accuracy, this project emphasizes **business-relevant evaluation metrics**, making the solution practical and industry-ready.



Fraud detection is not just about machine learning - it's about balancing customer protection and operational efficiency.

