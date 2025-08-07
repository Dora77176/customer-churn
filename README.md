# Telco Customer Churn Prediction

## Project Overview

This project aims to predict customer churn for a telecommunications company using machine learning techniques. By analyzing customer data, the goal is to identify which customers are likely to leave the service, allowing the company to take proactive retention measures.

## Dataset

The dataset contains customer information such as demographics, account details, and service usage. It includes both numerical and categorical variables and a target column indicating whether a customer has churned.

## Data Preprocessing

- Removed the `customerID` column as it is not useful for prediction.
- Converted the target variable `Churn` into binary format (`Yes` → 1, `No` → 0).
- Handled missing values in `TotalCharges`.
- Encoded categorical variables using one-hot encoding.

## Handling Imbalanced Data

The dataset is imbalanced, with fewer customers who churn than those who don't. To address this, the SMOTE (Synthetic Minority Over-sampling Technique) method was applied to balance the classes in the training set.

## Model Training

A Random Forest classifier was trained on the balanced dataset. The model was evaluated on the test set using metrics such as precision, recall, f1-score, and accuracy.

## Results and Interpretation

The model achieved an accuracy of approximately 78%. After applying SMOTE, recall improved for the churn class, indicating better identification of customers likely to churn, although precision decreased slightly. This trade-off is important for business decisions around customer retention.

## Conclusion

This project demonstrates the application of machine learning techniques to predict customer churn, including preprocessing, handling imbalanced data, model training, and evaluation. It can be further improved by hyperparameter tuning, feature engineering, and business cost analysis.

## How to Run
## How to Run

1. Clone the repository:
```bash
git clone https://github.com/ton-utilisateur/ton-projet.git
```
cd ton-projet
2. Install dependencies listed in `requirements.txt`.
3. Place the dataset file Telco-Customer-Churn.csv in the project folder.
4. Run the Jupyter notebook sequentially to follow the steps from data loading to model evaluation.

---

Feel free to reach out at ptheodora@outlook.fr for any questions or suggestions.
