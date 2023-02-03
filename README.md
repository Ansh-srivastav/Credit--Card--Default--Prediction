** Credit--Card--Default--Prediction**
**Credit Card -** 
A credit card is a financial instrument issued by bank with a pre-set credit limit, helping you make cashless transactions. the credit card issuer determines the credit limit based on your credit score, credit history and your income.

**What is Credit Card default?**
Missing credit card payments once or twice does not count as a default. A payment default occurs when you fail to pay the Minimum Amount Due on the credit card for a few consecutive months. Usually, the default notice is sent by the card issuer after 6 consecutive missed payments. However, the final call rests with the bank.

**Problem Statement**
This project is aimed at predicting the case of customers default payments in Taiwan. From the perspective of risk management, the result of predictive accuracy of the estimated probability of default will be more valuable than the binary result of classification - credible or not credible clients. We can use the K-S chart to evaluate which customers will default on their credit card payments.

X1: Amount of the given credit (NT dollar): it includes both the individual consumer credit and his/her family (supplementary) credit.
X2: Gender (1 = male; 2 = female).
X3: Education (1 = graduate school; 2 = university; 3 = high school; 4 = others).
X4: Marital status (1 = married; 2 = single; 3 = others).
X5: Age (year).
X6 - X11: History of past payment. We tracked the past monthly payment records (from April to September, 2005) as follows: X6 = the repayment status in September, 2005; X7 = the repayment status in August, 2005; . . .;X11 = the repayment status in April, 2005. The measurement scale for the repayment status is: -1 = pay duly; 1 = payment delay for one month; 2 = payment delay for two months; . . .; 8 = payment delay for eight months; 9 = payment delay for nine months and above.
X12-X17: Amount of bill statement (NT dollar). X12 = amount of bill statement in September, 2005; X13 = amount of bill statement in August, 2005; . . .; X17 = amount of bill statement in April, 2005.
X18-X23: Amount of previous payment (NT dollar). X18 = amount paid in September, 2005; X19 = amount paid in August, 2005; . . .;X23 = amount paid in April, 2005.

**Steps involed**
Exploratory data analysis
Handling class imbalanced
Feature engineering
One hot encoding
logistic regression 
decision tree
random forest classifier
SVM
XGBoost
hyperparameter tuning

**Conclusion**
From the project we can conclude that the default rate is higher for males, increases as the education increases, and also increases as the age of a person increases. i.e clients whose age over 60 was higher than mid-age and young people. In all of these models, our recall revolves in the range of 78 to 86%.with the best fit model as random forest.
From all baseline model, Random forest classifier shows highest train accuracy, test accuracy and F1 score .
After cross validation and hyperparameter tunning, XG Boost shows highest test accuracy score of 83.03%.
Cross validation and hyperparameter tunning certainly reduces chances of overfitting and also increases performance of model.

