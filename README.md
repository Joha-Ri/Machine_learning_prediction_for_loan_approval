# Project Loan Approval Prediction 🏦 💰

## The Team: Joel, Johana, Lucie, Manuel  👓


## Project Overview 📑
W are developing a machine learning model to predict whether a loan will be approved or rejected based on various features of the applicants. 
This prediction helps the bank make informed lending decisions.

## Dataset 
### Data Cleaning: 
- Removed leading and trailing spaces from both column names and data entries to ensure clean data for processing.
- Dropped the `loan_id` column as it is non-relevant for modeling.Removed leading and trailing spaces from both column names and data entries.

### Feature Engineering: 
- Created a new column named **`Total_Asset_Value`**, which is the sum of the following asset columns:
  - `residential_assets_value`
  - `commercial_assets_value`
  - `luxury_assets_value`
  - `bank_asset_value`Created a new column (Total_Asset_Value) as the sum of various asset columns.

### Encoding: 
Categorical variables: (like education and self_employed) were converted into dummy variables using one-hot encoding, allowing effective handling of these features in machine learning models.
Normalization/Standardization: The dataset was normalized and standardized to see which method yielded better accuracy.

## Normalization and Standardization 🔧
 The dataset was normalized using **Min-Max Scaling** and standardized using **Standard Scaler** to observe which method yields better accuracy for the predictive models.

## Machine Learning 🧠
### Techniques used 🧰
1. **Logistic Regression**: Used as a baseline model.
2. **K-Nearest Neighbors (KNN)**: Chosen for its simplicity and effectiveness in instance-based learning.
3. **Random Forest**: An ensemble method that improves prediction accuracy by reducing overfitting.

## Model performances and Key findings 🗝️
- **Logistic Regression**:
  - Normalized Model:
    - Accuracy: 91.22%
    - Precision: 89%
    - Recall: 87%
    - F1 Score: 88%
    - AUC-ROC: 97%
  - Standardized Model:
    - Similar performance metrics, indicating stability across different scaling methods.

- **Random Forest**:
  - Both normalized and standardized versions achieved accuracy rates of approximately 98%, highlighting its effectiveness for this classification problem.

- **KNN**:
  - Normalized Model:
    - Accuracy: 90%
    - Precision: 86%
    - Recall: 88%
    - F1 Score: 87%
  - Standardized Model:
    - Slightly lower performance metrics compared to the normalized version.

## Result 📈
The evaluation of the models highlighted Random Forest as the most effective model for predicting loan approvals. 
Logistic Regression and KNN also provided strong performance but were outperformed by the ensemble method.

## Conclusion : ✔️
The project demonstrated how machine learning can enhance decision-making in the banking sector. 
By analyzing various features and their impact, we were able to build robust predictive models. 
