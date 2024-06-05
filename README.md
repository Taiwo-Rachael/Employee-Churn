# Employee Churn Data Analysis and Modeling
#  📊 📈 📉 Introduction
This project involved analyzing an organization's employee churn data to identify factors contributing to the churn rate and training a machine learning model to identify employees who are likely to leave the company

# Data Cleaning
The data used for this project was clean, not containing any null or duplicated data, so no further cleaning was reqired.

#  🔍💡  Exploratory Data Analysis
The EDA process revealed some intresting insights. It was discovered that majority of the staff did not get promoted or get bonuses, and about 40% of them left the organization. interestingly, almost the same percentage of those who got bonuses and got promoted also left, showing that the lack of bonuses or promotion were not factors contributing to the churn rate. It was also discovered that those who left the organization had had higher review scores than those who stayed, which was quite curious.

It was also discoverd that those who left had spend more years in the organization (an average of 8 years) than those who stayed, majority having spent about 6 years. The analysis also showed that for those who left, as their tenure time (number of years spent) increased, the average hours of work in a month also increased which could have contributed to their leaving the organization.

The satisfaction score of the employees was also found to be low, between 0.4 - 0.6, both for those who left and those who stayed. Suggesting that even those employees who still stayed might eventually leave the organization after a few more years, since they had not even stayed as long as those who left.

# Feature Scaling
To prepare the data for modeling, the StandardScaler was used to standardize the data to a more uniform scale.

# Categorical Encoding
The OneHot Encoder was used to transformm the department column from categorical to numeric  while the OrdinalEncoder was used for the Salary column

# Modeling
I built a model to predict employees who are likely to leave the organization using classification algorithms. In this process, imbalanced data problem became quite obvious as the model overfit the class of those who stayed in the organization because of their higher number and the data had to be resampled using the RandomUnderSampler. This corrected the overfitting problem. The best performing model was the RandomForest Classifier with an accuracy of 84% and recall percentages of 84% for both classes.

# Conclusion 
The insights drawn from this project will help the organization to reduce their churn rate and the model will help the organization to identify members of staff who are likely to leave, and take possible measures to prevent this from happening.

