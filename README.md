# Home Credit Default Risk – Machine Learning Project

This project predicts **loan default risk** using historical financial data provided by the [Home Credit](https://www.kaggle.com/competitions/home-credit-default-risk/data) competition.  
By analyzing multiple financial datasets, the goal is to improve risk assessment and minimize losses for lenders.

> All code is split across modular notebooks, with outputs and explanations included.

---

## Live App Deployment

This project is also deployed as a real-time inference tool via an **Angular + Flask web application**:

[Try the Live Loan Default Predictor](https://ai.fullstackista.com/ai-loan-default-predictor)

---

## What This Project Covers

- End-to-end machine learning pipeline on real-world financial data
- Modular notebooks: each dataset is explored, cleaned, engineered, and aggregated individually
- Feature-rich model using **LightGBM** with hyperparameter tuning
- Final model evaluated on AUC-ROC, and deployed for real-time predictions

---

## Project Notebooks  

### Main Dataset and Model Training  
- [1. Application Train (Main Dataset)](./01_application_train.ipynb)  
- [2. Model Training and Final Pipeline](./02_model_training_pipeline.ipynb)  

### Secondary Datasets Processing  
- [3. Bureau Data](./03_bureau_data.ipynb)  
- [4. Bureau Balance Data](./04_bureau_balance.ipynb)  
- [5. Credit Card Balance](./05_credit_card_balance.ipynb)  
- [6. Previous Applications](./06_previous_applications.ipynb)  
- [7. POS Cash Balance](./07_pos_cash_balance.ipynb)  
- [8. Installments Payments](./08_installments_payments.ipynb)  

### Final Prediction  
- [9. Model Predictions on Test Data](./09_model_predictions.ipynb)  
- [10. Application Test Data Processing](./10_application_test_processing.ipynb)

---

## Notebook Structure

Each dataset-specific notebook includes:

1. **Initial Data Inspection** – Understand structure, missing values, and anomalies  
2. **Data Cleaning** – Handle nulls, fix types, remove invalid values  
3. **Exploratory Data Analysis (EDA)** – Identify trends and patterns  
4. **Feature Engineering** – Domain-driven aggregations (means, maxes, flags, ratios)  
5. **Aggregation** – Grouped stats per customer ID  
6. **Merging** – Output dataset merged into the master training data for modeling

---

## Tech Stack

| Component        | Tools Used                         |
|------------------|------------------------------------|
| Language         | Python, Jupyter Notebooks          |
| ML Framework     | LightGBM                           |
| Libraries        | Pandas, NumPy, Matplotlib, Seaborn |
| Model Evaluation | AUC-ROC, Stratified K-Fold CV      |
| Hosting          | [GitHub](https://github.com/ognjenmedic/home-credit-ml-project) + [Deployed App](https://ai.fullstackista.com/ai-loan-default-predictor)

---

## Outcome

- Final model achieved **0.7807 AUC** – comparable to public leaderboard scale (offline evaluation, not submitted).
- Clean, modular design makes it easy to extend or retrain on new datasets
- Real-time predictions delivered through a custom-built full-stack web app

---

## Also Available On

- [View Kaggle Notebooks](https://www.kaggle.com/code/ognjenmedic/home-credit-model-training)
- [About the Author](https://www.fullstackista.com/about-us)

---
