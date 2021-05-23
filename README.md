# Healthcare-Provider-Fraud-detection

**Summary:**

Source for the Data: HEALTHCARE PROVIDER FRAUD DETECTION ANALYSIS | Kaggle

The raw data comprises of the Inpatient, outpatient and the beneficiary details of Health Insurance Providers covering various aspects as below:
  a)	Inpatient Data: Claims filed, admission & discharge dates and admit & diagnosis code
  b)	Outpatient Data: Claims filed for those patients who visit hospitals and not admitted in it
  c)	Beneficiary Details: KYC details like health conditions, region they belong etc


**Objective of the Activity:**

The objective is to predict the potentially fraudulent providers based on the claims filed by each of the providers.

**Procedure:**

Currently the project is a Work In Progress. Although the process covered so far is as below:

  1.	Landscape of the Data Provided: 4 CSV files are provided and the shape of the dataset is as below:
        Shape of Train Beneficiary file Data: (138556, 25)
        Shape of Train In-patient file Data: (40474, 30)
        Shape of Train Out-patient file Data: (517737, 27)
        Shape of Train file Data: (5410, 2) 
  2.	The class distribution of the Dependent variable, which in our case is the Potential Fraud is Unbalanced with 90% of the claims being non-fraudulent whereas a 10% of the           cases being fraudulent 
  3.	Employed various Imputing techniques to impute missing values in various columns of each of the 3 data files: Beneficiary. Inpatient and outpatient data
  4.	Performed Univariate Analysis of different columns to look at the PDF and CDFs respectively
