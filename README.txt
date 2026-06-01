Telecom Customer Churn Prediction and Retention Intelligence System



1) Project Overview  

This project presents an end-to-end Data Science workflow for telecom customer churn prediction using machine learning, explainable AI, and business-driven analytics.

The objective is to identify customers with a high probability of leaving the telecom provider and generate actionable business recommendations to improve customer retention.

The project covers the complete data science lifecycle including data understanding, cleaning, exploratory analysis, feature engineering, model development, evaluation, optimization, and explainability.

The work was designed to simulate a real-world telecom analytics use case aligned with industry data science practices.

------------------------------------------------------------------------

2) Business Problem

Customer churn is one of the most important business challenges in the telecommunications industry.

Acquiring new customers is significantly more expensive than retaining existing ones. Therefore, telecom companies need predictive systems capable of detecting customers likely to leave before churn occurs.

The goal of this project is to:

* Predict customer churn risk.
* Understand the main drivers behind churn behavior.
* Generate business recommendations to support retention strategies.
* Compare multiple machine learning algorithms for telecom analytics.

------------------------------------------------------------------------


3) Dataset

Dataset: IBM Telco Customer Churn Dataset

The dataset contains customer information related to:

* Customer demographics
* Service subscriptions
* Contract information
* Billing and payment behavior
* Internet and telecom services
* Customer retention outcome

Target Variable:

`Churn`

Binary Classification Problem:

* Yes = Customer churned
* No = Customer retained

------------------------------------------------------------------------

4)  Project Workflow

1. Data Understanding and Cleaning

Performed:

* Dataset inspection
* Data type validation
* Missing value analysis
* Duplicate detection
* Numeric conversion of TotalCharges
* Removal of non-predictive identifier columns



2. Exploratory Data Analysis

Exploratory analysis was conducted to understand customer behavior and churn patterns.

Key analytical findings included:

* Month-to-month contracts showed higher churn probability.
* Short-tenure customers were more likely to churn.
* Monthly charges influenced customer retention behavior.
* Service usage patterns affected churn likelihood.

Visualization techniques included:

* Count plots
* Box plots
* Histograms
* Correlation heatmaps



3. Feature Engineering

Additional features were created to improve predictive performance.

Examples:

`ServiceCount`

Represents the number of subscribed telecom services.

`ChargesPerMonth`

Captures customer spending behavior relative to account duration.



4. Machine Learning Models

Multiple machine learning algorithms were benchmarked.

Implemented models:

* Logistic Regression
* Random Forest
* XGBoost
* Tuned Random Forest

Cross-validation and hyperparameter tuning were applied to improve model robustness.



5. Model Evaluation

Evaluation metrics included:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC

Final experimental results:

| Model                      | Accuracy | Precision | Recall | F1     | ROC_AUC |
| -------------------------- | -------- | --------- | ------ | ------ | ------- |
| Scaled Logistic Regression | 0.8084   | 0.6745    | 0.5374 | 0.5982 | 0.8462  |
| Random Forest              | 0.8055   | 0.6701    | 0.5267 | 0.5898 | 0.8406  |
| XGBoost                    | 0.7999   | 0.6503    | 0.5321 | 0.5853 | 0.8390  |
| Tuned Random Forest        | 0.8013   | 0.6556    | 0.5294 | 0.5858 | 0.8419  |


(Scaled Logistic Regression achieved the strongest overall performance in this experiment).


------------------------------------------------------------------------


5) Explainable AI

SHAP explainability was used to understand model behavior and identify feature contributions at both global and local prediction levels.

This analysis helped explain how factors such as contract type, tenure, and pricing behavior influenced churn predictions.


------------------------------------------------------------------------


6) Business Recommendations

Based on the analytical findings and model outputs, several business recommendations were generated.

Contract Strategy:

Encourage migration from month-to-month subscriptions toward longer-term contracts using retention incentives.

Customer Onboarding:

Implement targeted retention campaigns during the first months of customer lifecycle.

Pricing Optimization:

Review pricing strategies for customer segments exposed to elevated churn risk.

Service Bundling:

Promote multi-service packages to improve customer engagement and retention.

------------------------------------------------------------------------

7) Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

XGBoost

SHAP

Jupyter Notebook

------------------------------------------------------------------------


8) Project Structure


   Orange-Telecom-Churn-Prediction/

     data/
     images/
     Orange_Telecom_Churn_Prediction.ipynb
     README.md
     requirements.txt
   
   
------------------------------------------------------------------------



9) How to Run the Project

Clone the repository:

bash
git clone <your_repository_link>


Install dependencies:

bash
pip install -r requirements.txt


Launch Jupyter Notebook:

bash
jupyter notebook


Open:

`Orange_Telecom_Churn_Prediction.ipynb`

Run all notebook cells sequentially.

------------------------------------------------------------------------


10) Future Improvements

Potential future enhancements include:

* Streamlit deployment
* Power BI dashboard integration
* Threshold optimization
* Class imbalance handling with SMOTE
* Production-ready API deployment
* Advanced telecom customer segmentation
