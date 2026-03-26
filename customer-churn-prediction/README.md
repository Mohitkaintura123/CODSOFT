# Customer Churn Prediction using Machine Learning

##  Overview
This project predicts whether a customer will churn (leave a service) using machine learning techniques on a banking dataset.

## Objective
To identify customers likely to churn so that businesses can take preventive actions.



## Dataset
The dataset contains customer information such as:
- Age
- Balance
- Credit Score
- Geography
- Number of Products
- Activity status



##  Workflow

1. Data Loading & Inspection  
2. Exploratory Data Analysis (EDA)  
3. Data Preprocessing (Encoding + Scaling)  
4. Handling Class Imbalance using SMOTE  
5. Model Training (Multiple Models)  
6. Model Evaluation (ROC-AUC, Precision, Recall)  
7. XGBoost Optimization  
8. Cross Validation  
9. SHAP Explainability  


## Models Used

- Logistic Regression  
- Random Forest  
- Gradient Boosting  
- **XGBoost (Best Model)**  



## Final Results

- Accuracy: **85%**  
- Precision: **63%**  
- Recall: **64%**  
- F1 Score: **64%**  
- ROC-AUC: **0.87**  



## Key Insights

- Older customers are more likely to churn  
- Inactive users show higher churn rates  
- Customers with fewer products tend to leave  



##  Techniques Used

- SMOTE (Handling Imbalanced Data)  
- Cross Validation  
- Hyperparameter Tuning  
- SHAP (Explainability)  



##  Business Impact

- Helps identify high-risk customers  
- Improves retention strategies  
- Reduces revenue loss  



##  Tech Stack

- Python  
- Pandas, NumPy  
- Scikit-learn  
- XGBoost  
- Matplotlib, Seaborn  
- SHAP  



##  Files

- notebook.ipynb → Full ML pipeline  
- best_model.pkl → Trained model  
- scaler.pkl → Data scaler  
- requirements.txt → Dependencies  



## Future Improvements

- Deploy using Streamlit  
- Add API integration  
- Use deep learning models  



##  Acknowledgement

This project was completed as part of the **CODSOFT Machine Learning Internship**.


