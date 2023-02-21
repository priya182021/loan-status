# loan-status
# Data Description
loan_Id
Gender: Male, Female
Married: Yes,No.
Dependents: is the customer having any other applicant who is also responsible for the loan.
Education: Graduate, non graduate.
A self-employed person does not work for a specific employer who pays them a consistent salary or wage. so is the customer self employeed or not.
Applicant income : it is the income of that customer.Primary apllicant
Co applicant income: A co-applicant is a person who is jointly applying for a loan with the primary applicant.
Loan Amount
Loan amount term: in days
Credit history: is the customer having any credit history. 0: means bad credit history and 1: good credit history.
Property area: Rural or Urban.
Loan status: is the customer has been sanctioned the loan or not?

# Analysis

We start with Descriptive statistics for numerical data and categorical data. 
Then we treat missing values by filling up the null values with suitable value of mean, median or mode.
Then to find outliers we use box plot and find outliers in Applicant income, co applican income and Loan amount. As a result we discard the observation which contains outliers.
We show univariate Analysis for above three categoriies and try to normalize them to obtain better result by using log transform method.
Also we show univariate analysis  for each category.
we also observe the impact  of applicant income and co applicant income on loan status.
we also try to find the impact of loan amount and loan amount term on loan status.
we then compare each category with target variable.
then we clean the data by deleting some unwanted features. 
Also we do feature engineering by label encoding some of the features.
After all preprocessing is done we seperate the target feature Loan status for further analysis.
Since we can see the target variable is imbalanced. There are more yes as compared to no. so we try to balance data by using SMOTE method.
After balancing data  we split them into training data and testing data by train test split data.
Then we use ML algorithm like logistic regression and Gradient Boost model for predicting whether to give loan or not.
And check which model is best by building confusion matrix for both models.
