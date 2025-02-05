# **Supervised Learning Analysis**
This repository contains a Jupyter Notebook that explores **Supervised Learning models** using a dataset of 5001 records. The analysis includes **data preprocessing, feature engineering, model training, evaluation, and recommendations**.

## **Project Overview**
The project applies various supervised machine learning models to classify data and assess their performance using different metrics. The models analyzed include:
- **Logistic Regression**
- **Support Vector Machine (SVM)**
- **Decision Tree**
- **Random Forest**
- **k-Nearest Neighbors (KNN)**
- **Naive Bayes**
- **XGBoost**

## **Dataset and Preprocessing**
- **Missing Values:** The dataset had no missing values.
- **Categorical Data:** Ordinal and One-Hot Encoding were applied where necessary.
- **Numerical Features:** Min-Max Scaling was used to standardize numerical data.
- **Outliers:** Box plots were analyzed, but outliers were retained for model learning.

## **Model Evaluation**
### **Performance Metrics:**
| Model                 | Accuracy | Macro F1-score | Weighted F1-score |
|-----------------------|----------|---------------|------------------|
| Logistic Regression  | 33.24%   | 0.32          | 0.32             |
| SVM                  | 32.05%   | 0.16          | 0.16             |
| Decision Tree        | 33.58%   | 0.34          | 0.34             |
| KNN                  | 34.18%   | 0.34          | 0.34             |
| Random Forest        | 33.78%   | 0.34          | 0.34             |

- **Best Accuracy:** KNN (34.18%) performed the best.
- **Fastest Model:** Naive Bayes (0.0041s) and KNN (0.0046s).
- **Computationally Expensive:** Random Forest and SVM took significantly longer to execute.

## **Key Insights**
- **KNN provided the best trade-off between accuracy and runtime.**
- **Decision Tree and Logistic Regression performed similarly, but Decision Tree had a slight edge.**
- **Random Forest offered marginal accuracy improvements but was computationally heavy.**
- **SVM struggled with class imbalances, leading to poor F1-scores.**
- **Feature selection and cross-validation were applied to improve model robustness.**

## **Recommendations**
- **For quick, interpretable results:** Use **Logistic Regression**.
- **For better accuracy and efficiency:** Use **KNN**.
- **For deep feature interactions:** Use **Random Forest**, but be aware of computational costs.
- **For large-scale applications:** Consider tuning **Decision Trees** with pruning.

## **Repository Contents**
- 📂 `055046_Supervised_Learning.ipynb` → Jupyter Notebook with full analysis and results.
- 📄 `README.md` → Project documentation.
