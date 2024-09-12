## Project Title: Forgery-Detector-Classifying-Genuine-vs.-Forged-Banknotes

### Data Source : 
- Link : https://openml.org/search?type=data&sort=runs&status=active&id=1462&utm_source=datacontinuum.beehiiv.com&utm_medium=referral&utm_campaign=hypothesis-testing-deciding-kpi-and-a-cool-dataset

### Model : Classification
- LogisticRegression

  ### Project Link: 

### Project Report :

# **Project Report: Banknote Authenticity Classification**


**Objective**: The purpose of this project is to develop a machine learning model to classify banknotes as either genuine or forged using features provided in the dataset.

**Dataset Overview:** The dataset includes four features (V1, V2, V3, V4) and a target variable (Class), where the Class 1 represents whether a banknote is genuine  and Class 2 forged.

### **Data Exploration and Preprocessing**

**Data Exploration:**

- I performed initial exploratory data analysis (EDA) to understand the spread and distribution of features and target variables using a histogram
to  identify patterns between genuine and forged banknotes.

**Data Cleaning:**

- I checked the dataset for missing values, and outliers preparing the datset for  the analysis. Features were standardized to ensure they are on the same scale for optimal model performance.

**Feature Engineering**
- No new features were created, but existing features (V1, V2, V3, V4) were used for modeling.
- The feature importance analysis was conducted to identify which features had the most influence on the classification.

### **Model Building**

**Model Selection**

- I used the  Logistic Regression for this analysis which provided good results after evaluation.

**Train-Test Split:**

- The data was split into training and testing sets using an 70/30 ratio. 
 **Target** : Class (1  represent genuine note, 2 represent forged note)
 **Features** : V1, V2, V3, V4

**Accuracy** 

- The Logistic Regression model achieved an accuracy of 99% on the test set.

**Other Metrics:**

|             |precision |recall     |f1-score    |   support |
|-------------|----------|-----------|------------|-----------|
|           1 |      0.99|      0.99 |     0.99   |    229    |
|           2 |      0.98|      0.99 |     0.99   |    183    |
|             |          |           |            |           |
|    accuracy |          |           |     0.99   |    412    |
|   macro avg |      0.99|      0.99 |     0.99   |    412    |
|weighted avg |      0.99|      0.99 |     0.99   |    412    |
|             |          |           |            |           |




- Confusion matrix: confusion matrix was used to visualize true positives, false positives, false negatives, and true negatives.

**Feature Importance Analysis**

- I analyzed feature importance to understand which features (V1, V2, V3, V4) had the greatest impact on classification.

**Key Insights**

- Feature V4 was identified as the strongest predictor of whether a banknote is genuine or forged, followed by V2.

### **Conclusion**

**Summary of Findings**

- The model effectively classified banknotes as genuine or forged, with an accuracy of 98% on the test data.

- Feature V4 had the highest importance in predicting authenticity.

**Next Steps**

- Further improvements could include gathering more data to enhance the model's performance, testing additional algorithms, or deploying the model in a real-time currency authentication system.
- Additional research could focus on integrating more features or applying unsupervised learning techniques for anomaly detection.

**Challenges**
- The features meta data only provided for V1 and V2  as (V1. variance of Wavelet Transformed image (continuous)
V2. skewness of Wavelet Transformed image (continuous)) and nothing is explained about V3, V4


