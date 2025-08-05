# Telco Customer Churn Prediction

## 📋 Project Overview

This project aims to predict customer churn for a telecommunications company using supervised machine learning. By identifying customers likely to leave, the company can take proactive steps to improve retention and reduce revenue loss.

---

## 🚀 Problem Statement

**Goal:**  
Predict which customers are likely to churn (leave the company) based on their demographics, account information, and service usage patterns.

---

## 🗂️ Project Structure

```
Telco-Customer-Churn-Prediction/
│
├── Data/                # Data.csc,cleaned_dataset.csv,Featured_Data.csv
│
├── Notebooks/           # Jupyter notebooks for each step
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda
│   ├── 03_feature_engineering.ipynb
│   ├── 04_modeling.ipynb
│
├── Outputs/             # Plots ,results
├── requirements.txt     # Python dependencies
├── README.md            # Project documentation
└── .gitignore
```

---

## 🛠️ Workflow

1. **Data Cleaning & Preprocessing**
   - Handled missing values and corrected data types
   - Dropped irrelevant columns (e.g., customerID)
2. **Exploratory Data Analysis (EDA)**
   - Visualized churn rates and feature distributions
   - Identified key patterns and potential predictors
3. **Feature Engineering**
   - Encoded categorical variables
   - Scaled numerical features
   - Created new features (if needed)
4. **Model Training & Hyperparameter Tuning**
   - Tried multiple models: Logistic Regression, Decision Tree, Random Forest, AdaBoost, SVC, Gradient Boosting
   - Used RandomizedSearchCV for hyperparameter tuning
5. **Model Evaluation & Selection**
   - Compared models using F1 score, accuracy, and ROC AUC
   - Selected the best model based on test set performance
6. **Interpretation & Business Insights**
   - Analyzed feature importance
   - Provided actionable recommendations

---

## 🏆 Results

- **Best Model:** logistic Regression 
- **Test Accuracy:**  0.7978
- **Test ROC AUC:** 0.8460  
![alt text](image-1.png)

The model can accurately identify customers at risk of churning, enabling targeted retention strategies.

---

## 📊 Key Insights

- **Contract type**, **tenure**, and **monthly charges** are strong predictors of churn.
- Customers with month-to-month contracts and higher monthly charges are more likely to churn.
- The model can be integrated into business processes for real-time churn prediction.

---

## 💡 Business Recommendations

- Focus retention efforts on customers with high predicted churn risk.
- Offer incentives or improved service to customers with month-to-month contracts.
- Monitor and retrain the model regularly to adapt to changing customer behavior.

---

## 🖥️ How to Run

1. **Clone this repository:**
   ```bash
   git clone https://github.com/qosain-bukhari/Telco-Customer-Churn-Prediction.git
   cd Telco-Customer-Churn-Prediction
   ```
2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Place the raw dataset in `Data/` if not already present.**
4. **Run the notebooks in order (from data cleaning to modeling).**
5. **Review the outputs and results in the `Outputs/` folder.**

---

## 📚 Data Source

- [Kaggle: Telco Customer Churn Dataset](https://www.kaggle.com/blastchar/telco-customer-churn)

---

## 👤 Author

- Qosain Bukhari  
-
https://github.com/qosain-bukhari/Telco-Customer-Churn-Prediction
---

## 📄 License


This project is for educational purposes. Please refer to the [Kaggle dataset license](https://www.kaggle.com/blastchar/telco-customer-churn) for data usage terms.

