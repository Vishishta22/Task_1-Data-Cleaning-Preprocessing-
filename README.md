# Task_1-Data-Cleaning-Preprocessing-
Loan Approval Prediction – Data Cleaning & Preprocessing
This repository contains a Jupyter Notebook demonstrating data cleaning and preprocessing techniques on the Loan Approval Prediction dataset.

Task Objective
To prepare raw data for machine learning by applying essential preprocessing steps using Python, Pandas, NumPy, Seaborn, and Matplotlib.

Steps Performed
1. Dataset Loading & Exploration
    Imported the Loan Approval dataset using Pandas
    Explored the shape, data types, and checked for null values
    Identified columns with missing data for further handling
   
3. Missing Value Handling

Categorical: filled using mode because categories like 'Dependents' and 'Credit_History' often have a most frequent (typical) value that makes sense to use as a filler.
Numerical: filled using median to prevent skewing the data when outliers are present (which is common in income or loan amounts).

3. Categorical Encoding

    1. Applied Label Encoding for binary categorical columns (e.g., Gender, Married)
    2. Used One-Hot Encoding for multiclass features like Dependents and Property_Area to convert them into numerical format

4. Feature Scaling

    1. Standardized numerical features for consistent range to ensure they have a mean of 0 and a standard deviation of 1

5. Removed outliers using IQR method
   1. Created boxplots to visualize outliers in numerical columns
   2. Used the Interquartile Range (IQR) method to remove data points outside acceptable ranges

Dataset Columns Used
Loan_ID, Gender, Married, Dependents, Education, Self_Employed, ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term, Credit_History, Property_Area, Loan_Status

How to Run
    1. Clone the repo or download the .ipynb file
    2. Open in Jupyter Notebook or Google Colab
    3. Install required libraries (Pandas, NumPy, Seaborn, Matplotlib, sklearn)
    4. Run the notebook step by step
