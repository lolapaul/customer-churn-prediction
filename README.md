#  Customer Churn Prediction

This project builds a machine learning model to predict customer churn for Interconnect, a telecom provider. The company wants to proactively identify customers likely to leave and offer them retention incentives. The model is trained using personal, contractual, and service usage data.

---

##  Objective

Predict churn probability for each customer based on their:
- Contract type
- Internet & phone services
- Payment method
- Tenure and other behavioral patterns

---

##  Dataset Description

The data is composed of four CSV files:

1. **contract.csv** – Contract type and duration
2. **personal.csv** – Personal customer data
3. **internet.csv** – Internet services used
4. **phone.csv** – Phone services used

All datasets are linked using `customerID`. The target column is:
- `EndDate`: if `No`, the customer stayed (label = 0), otherwise, churned (label = 1)

---

##  Project Workflow

1. **Data Preparation**
   - Merge datasets using `customerID`
   - Handle missing values
   - Encode categorical features

2. **EDA & Feature Engineering**
   - Distribution of churn across services
   - Correlation between tenure, services, and churn

3. **Model Training**
   - Split into training/validation/test sets
   - Test multiple models: Logistic Regression, Random Forest, XGBoost
   - Use AUC-ROC as the main metric

4. **Model Evaluation**
   - Final model achieves **AUC-ROC ≥ 0.88**
   - Evaluate precision, recall, F1-score

---

##  Key Features Used

- Contract length
- Type of Internet & phone service
- Monthly charges
- Number of additional services
- Payment method
- Tenure

---

##  Tools & Libraries Used

- Python
- pandas
- matplotlib & seaborn
- scikit-learn
- xgboost
- Jupyter Notebook

---

##  Status

✔️ Project completed as part of the **TripleTen Bootcamp** – Sprint: *Predictive Modeling & Classification*

---

##  Project Structure
```
customer-churn-prediction/
│
├── customer_churn_prediction.ipynb
├── contract.csv
├── personal.csv
├── internet.csv
├── phone.csv
├── requirements.txt
└── README.md
```


---

##  Author

David Villanueva  
[LinkedIn](https://www.linkedin.com/in/david-villanueva-59659727)  
[GitHub](https://github.com/lolapaul)
