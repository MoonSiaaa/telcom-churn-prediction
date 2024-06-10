# Telecom - churn prediction
## Customer Churn Prediction in Telecommunications: A Machine Learning Approach
### Introduction

This report details the development of a churn prediction model for a telecommunications company. The objective is to identify customers at risk of leaving, enabling proactive retention strategies.

### Data and Preprocessing

The publicly available Telco-Customer-Churn dataset from Kaggle was used. Preprocessing steps included handling missing values, encoding categorical variables using one-hot encoding, and data cleaning.

### Exploratory Data Analysis (EDA)

EDA revealed key insights into customer behavior and churn factors:

High Churn with High Monthly Charges: Customers with higher monthly charges exhibited a higher propensity to churn.
Surprising Insight: Lower Total Charges and Churn: Interestingly, churn was also observed at lower total charges. This seemingly contradictory finding was explained through feature engineering.
### Feature Engineering

A new feature, "Total Charge," was created by multiplying "Monthly Charges" and "Tenure." This helped clarify the relationship between churn and charges:

Higher Monthly Charge and Lower Tenure Lead to Lower Total Charge and Higher Churn: Customers with high monthly charges but short tenures (resulting in lower total charges) were more likely to churn.
Model Building and Evaluation

Several machine learning algorithms were explored for churn prediction: decision trees, random forests, and principal component analysis (PCA). However, the Random Forest model achieved the best performance based on metrics like accuracy, precision, recall, and F1-score (specific metrics not provided due to missing information).

### Key Findings

Contract Type: Customers with month-to-month contracts exhibited higher churn rates due to a lack of commitment.
Value-Added Services: Customers without online security, tech support, or fiber optic internet were more prone to churn, suggesting a desire for these services.
Customer Tenure: Customers in their first year of service had a higher churn probability, while those engaged for over five years showed lower churn.
Uninfluential Factors: Gender, phone service availability, and the number of lines had minimal impact on churn.
Conclusion

This project successfully developed a churn prediction model using a Random Forest algorithm. The analysis identified factors influencing churn, including contract type, value-added services, customer tenure, and specific demographics. These insights can be used by the telecommunications company to implement targeted retention strategies for high-risk customers.

### Future Work

Further exploration could involve:

Experimenting with different hyperparameter tuning for the Random Forest model.
Analyzing churn reasons provided by customers (if available) to gain deeper insights.
Utilizing feature selection techniques to identify the most impactful features for churn prediction.
Implementing the model in a production environment to monitor churn and refine strategies over time.
Fully Deplying the project using Flask 
