# Loan_Approval-Classification
## Overview
this project examines the Loan Approval Prediction dataset from Kaggle. Data cleansing, Data wrangling, Data Visualization, exploratory data analysis (EDA), model training and evaluation are all included in the analysis.

## About the Dataset
Information about loan applicants and their loan approval status may be found in the Loan Approval Classification Dataset, which was obtained via Kaggle. The dataset contains 45,000 records and 14 variables, each described below:

Demographic information: age, gender, education level  <br /> 
Financial information: Annual income, work experience "years", loan amount requested, loan intention  <br />
Credit information: Credit score, credit histoy length, previous loans  <br />
Asset information: home ownership  <br />
Target variable: Loan status (Approved/Rejected)

## Project Key Steps and Summary

### 1- Loading Data
- Read data from a local file upladed from kaggle <br />
### 2- Data Cleaning 
- Checked for null values and didn't find any  <br />
- Checked for duplicates and didn't find any <br />
- Checked for missing values and didn't find any <br />

### 3- Data Wrangling
- Created dummies for client gender   <br />
- Converted age, income, loan amount and length of credit history from float into integer format <br />
- Listed categorical and numerical variables separately <br />

### 4- Data Visualization
- Plot categorical variables in pie charts  <br />
- Plot histograms for numerical variables <br />

### 5- Exploratory Data Analysis (EDA)
- Explored the relationship beteen income an loan amount using scatter plot and found them  inversely correlated  <br />
- Used a bar plot to expore the loan intention and loan status relationship and found that people with Debt Consilidation loan intention had a better chance to get approved  <br />
- We used a confusion matrix to find age, experience and credit history length are highly correlated  <br />

### 6- Data Splitting and Model Training

- Manually split data into 80% training and 20% testing sets <br />
- Performed feature scaling <br />
- Trained Logistic Regression,  KNN and Random Forest models and implemented cross-validation on them <br />

### 7- Model Evaluation
- Evaluated model using accuracy, precision, F1-score
- Compared results from manual split with cross-validation

## Results
### Logistic Regression Model Performance
- Logistic Regression evaluation on the test data: <br />
  - Accuracy: 89.44% <br />
  - Precision: 77.52% <br />
  - F1-score: 75.86% <br />

- Cross Validation Logistic regression scores:
   - Accuracy: 89.71% <br />
   - Precision: 77.91% <br />
   - F1-score: 76.35% <br />

### K-Neighrest Neighbor Model Performance
- K-Neighrest Neighbor evaluation on the test data: <br />
  - Accuracy: 88.93% <br />
  - Precision: 79.37% <br />
  - F1-score: 73.34% <br />

- Cross Validation K-Neighrest Neighbor scores:
   - Accuracy: 88.96% <br />
   - Precision: 78.78% <br />
   - F1-score: 73.43% <br />

### Random Forest Model Performance
- Random Forest evaluation on the test data: <br />
  - Accuracy: 93.00% <br />
  - Precision: 89.98% <br />
  - F1-score: 83.14% <br />

- Cross Validation Random Forest scores:
   - Accuracy: 92.73% <br />
   - Precision: 89.42% <br />
   - F1-score: 82.34% <br />


As we can see, Random Forest algorithm is best suited for this data since it had a better accuracy of 93.00% on test data and 92.73% using cross validation method.

## Author

Salman Al Gahuri



