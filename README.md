# churn_Prediction_Smote
![image](https://user-images.githubusercontent.com/71244843/194754698-35bdadca-8052-4bb8-89ec-a14addca202f.png)
![image](https://user-images.githubusercontent.com/71244843/194754716-86885ca5-6215-410c-ba77-0af35b8e3313.png)
![image](https://user-images.githubusercontent.com/71244843/194754732-1b392715-f17e-4958-ba36-73c8a6f06f28.png)

Implementation:
Module 1 : EXPLORATORY DATA ANALYSIS

Step 1: Data Collection & Preprocessing:
Features {{ X(customerID,gender, SeniorCitizen, Partner, Dependents, tenure, PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies, Contract, PaperlessBilling, PaymentMethod, MonthlyCharges, TotalCharges), Y(Churn)}}
Step1.1 : Ratio of Churners/Non-churners
Step1.2 : Categorical analysis : Univariate analysis by Churn (All X by Y), Bivariate analysis, Multivariate analysis (n(X) with Y) -> Ex. Male Monthly SeniorCitizen by Churn is more
Step1.3 : Numerical analysis: Correlation Matrix -> MonthlyChargers, Tenure = 0.9 -> Pattern in dependency
Step1.4 : Gather insights form EDA![image](https://user-images.githubusercontent.com/71244843/194754778-03189881-ab6d-4517-8e91-7a92c7651b24.png)


Module 2:  BUILDING MODELS

Step 2: Create variables and bifurcate training and testing data
Step 2.1: Build a Decision Tree Classifier – Gini Index
![image](https://user-images.githubusercontent.com/71244843/194754827-d5bcbe75-ad83-4d29-8548-8b327ca18595.png)
Step 2.2: Calculate the prediction score
Step 2.3: Import Smote- EEN for Oversampling to increase accuracy
Step 2.4: Build a Random Forest Classifier – Gini Index
![image](https://user-images.githubusercontent.com/71244843/194754870-1603efa4-7866-46a2-aecf-6f11ea9f7768.png)
Step 2.5: Calculate the prediction score and save the model using pickle


Module 3 : DEPLOYMENT

Step 3: Initialize Flask, read the data and load the UI(HTML) page
Step 3.1: List the input queries
Step 3.2: Load the model
Step 3.3: Predict the churn
Step 3.4: Return the result with score!



