# Loan Default Risk Prediction with Business Cost Optimization

## Project Overview
This project predicts the likelihood of a loan default using machine learning and optimizes the decision threshold based on **business cost-benefit analysis**.  
The dataset used is the **Default of Credit Card Clients Dataset** from the UCI Machine Learning Repository.

By modeling loan defaults and incorporating financial costs of misclassification, the project helps financial institutions minimize losses and make better lending decisions.


## Dataset
- **Source:** [UCI Repository – Default of Credit Card Clients Dataset](https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients)  
- **File:** `default_of_credit_card_clients.xls`  
- **Description:** Contains payment records of 30,000 Taiwanese credit card clients, including demographics, bill statements, payment history, and default status.

**Target Variable:**  
- `default.payment.next.month` → `1` if client defaulted, `0` otherwise.


## Project Workflow
1. **Data Cleaning & Preprocessing**
   - Handle missing values
   - Encode categorical variables
   - Feature scaling

2. **Exploratory Data Analysis (EDA)**
   - Distribution of features
   - Correlation analysis
   - Class imbalance check

3. **Model Training**
   - Logistic Regression
   - CatBoost Classifier
   - Other classification models for comparison

4. **Business Cost Optimization**
   - Define business costs:
     - **False Positive (FP):** Approving a risky client (loss to bank)  
     - **False Negative (FN):** Rejecting a good client (opportunity cost)  
   - Adjust classification threshold to minimize total cost

5. **Evaluation Metrics**
   - Accuracy, Precision, Recall, F1-score
   - ROC-AUC curve
   - Business cost function

## Results
- Models compared on traditional metrics and **optimized cost**.  
- Business-aware thresholding showed significant improvement in minimizing financial loss compared to the default 0.5 threshold.


