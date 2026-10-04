# Telecom Churn Prediction — ML Client Project

## Project Overview

This project develops a machine learning solution to predict customer churn for a telecom company.

The project was completed as part of the DataMites ML Client Project — No-Churn Telecom.

## Business Problem

Customer churn is an important business problem for telecom companies. Identifying customers who are likely to leave can help the business take proactive retention actions.

The objective is to understand the factors influencing customer churn and generate churn risk predictions.

## Project Objective

- Analyze customer attributes related to telecom churn.
- Build a machine learning classification model to predict churn.
- Evaluate model performance using classification metrics.
- Generate churn risk scores for customers.
- Create a `CHURN-FLAG` to identify customers predicted as likely to churn.

## Dataset

The project uses the telecom churn dataset provided for the client project.

The dataset contains customer and service-related attributes such as:

- State
- Account Length
- Area Code
- Phone
- International Plan
- VMail Plan
- VMail Message
- Day Mins
- Day Calls
- Day Charge
- Eve Mins
- Eve Calls
- Eve Charge
- Night Mins
- Night Calls
- Night Charge
- International Mins
- International Calls
- International Charge
- Cust Serv Calls
- Churn

The original project specification contains the database details and dataset information. Database credentials are not included in this repository.

## Approach

1. Loaded and inspected the telecom churn dataset.
2. Performed data-quality and missing-value checks.
3. Analyzed numerical and categorical variables.
4. Encoded categorical features.
5. Removed the `Phone` identifier field.
6. Performed exploratory data analysis.
7. Analyzed the churn distribution.
8. Handled extreme values using IQR-based treatment.
9. Prepared the features and target variable.
10. Split the data into training and testing sets.
11. Built a baseline classification model.
12. Performed hyperparameter tuning using GridSearchCV.
13. Applied SMOTE to address class imbalance.
14. Trained the final churn prediction model.
15. Evaluated the model using classification metrics and ROC-AUC.
16. Generated customer churn risk scores.
17. Created `CHURN-FLAG` predictions to identify high-risk customers.

## Model Evaluation

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

## Churn Risk Analysis

The final workflow generates a churn risk score for each customer.

A `CHURN-FLAG` is also created to identify customers predicted as likely to churn, supporting customer retention analysis.

## Results

The complete exploratory analysis, preprocessing, model development, hyperparameter tuning, evaluation results, churn risk scoring, and predictions are available in the Jupyter Notebook.

## Limitations

- Churn behaviour can be influenced by factors that are not available in the dataset.
- Class imbalance can affect model performance.
- Customer behaviour and telecom service conditions can change over time.
- Risk predictions should support business decisions rather than replace business judgement.

## Future Improvements

- Test additional classification algorithms.
- Perform more extensive hyperparameter optimization.
- Explore advanced ensemble models.
- Improve feature engineering.
- Monitor model performance on newer customer data.
- Deploy the churn prediction model as an API or dashboard.

## Project Structure

```text
ML-Client-Project-No-Churn-Telecom/
│
├── Telecom_Churn_FINAL_with_outputs.ipynb
├── README.md
├── requirements.txt
└── .gitignore

How to Run
1. Clone the Repository
git clone https://github.com/pegadapallyadithya/ML-Client-Project-No-Churn-Telecom.git
cd ML-Client-Project-No-Churn-Telecom

2. Install Required Libraries
pip install pandas numpy scikit-learn matplotlib seaborn imbalanced-learn sqlalchemy pymysql jupyter

3. Prepare the Dataset
Use the authorized telecom churn dataset for the project.
Database credentials and sensitive connection details are not stored in this repository.

4. Open the Notebook
jupyter notebook

Open the telecom churn Jupyter Notebook.
5. Run the Notebook
Run the notebook cells sequentially to reproduce the data analysis, preprocessing, model training, evaluation, and churn risk prediction workflow.
Technology Stack
Technology	Purpose
Python	Core programming language
Pandas	Data loading and data analysis
NumPy	Numerical operations
Scikit-learn	Machine learning and model evaluation
Imbalanced-learn	SMOTE for class imbalance
SQLAlchemy	Database connectivity
PyMySQL	MySQL database connection
Matplotlib	Data visualization
Seaborn	Statistical visualization
GridSearchCV	Hyperparameter tuning
Jupyter Notebook	Project development and documentation


Machine Learning Workflow
Data Loading → Data Quality Checks → EDA → Preprocessing → Feature Preparation → Train/Test Split → Baseline Model → Hyperparameter Tuning → SMOTE → Final Model → Evaluation → Churn Risk Scoring → CHURN-FLAG
Author
Pegadapally Adithya
Machine Learning / AI Project
