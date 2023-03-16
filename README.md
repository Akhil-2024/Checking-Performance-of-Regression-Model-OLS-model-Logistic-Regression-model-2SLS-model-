# Checking-Performance-of-Regression-Model-OLS-model-Logistic-Regression-model-2SLS-model-
We want to predict the species of an iris flower based on the measurements of its sepal length, sepal width, petal length, and petal width.

**DataSet:-** I have used the iris dataset, which contains measurements for 150 iris flowers (50 flowers from each of the 3 species). Each row of the dataset represents one iris flower and its corresponding measurements.

**How to use OLS(Ordinary Least Squares):-**
Ordinary Least Squares is a statistical method used to estimate the parameters of a linear regression model. Here are the general steps to use the OLS model:

Step-1-

Collect data: collect data that contains the dependent variable (Y) and one or more independent variables (X).

Step-2-

Define the model: Based on the data collected, define a linear regression model that represents the relationship between the independent variables and the dependent variable.

Step-3-

Estimate the coefficients: Use the OLS method to estimate the coefficients (also called parameters or beta coefficients) of the linear regression model. The OLS method estimates the coefficients that minimize the sum of the squared differences between the observed values of the dependent variable and the predicted values from the model.

Step-4-

Assess the model: Assess the goodness of fit of the model using various measures such as R-squared, adjusted R-squared, F-statistic, and residual plots.

Step-5-

Make predictions: Once the model is validated, you can use it to make predictions by plugging in the values of the independent variables.

**How to Use Logistic Regression:-**
Regression is a statistical method that is commonly used to analyze the relationship between a binary dependent variable (i.e , a variable that can take only two values, such as 0 or 1) and one or more independent variables.

Logistic regression is often used for predictive modeling and classification.

Step:1

Define the problem: Determine what you want to predict using the logistic regression model. For example, you may want to predict whether a customer will buy a product or not based on their demographic information.

Step:2

Collect data: Gather the data needed for the model. This may include both dependent and independent variables.

Step:3

Prepare the data: Preprocessing of data, including cleaning the data, handling missing values, and encoding categorical variables.

Step:4

Split the data: Divide the data into two sets: a training set and a testing set. The training set will be used to train the model, while the testing set will be used to evaluate its performance.

Step:5

Train the model: Fit the logistic regression model to the training data.

Step:6

Evaluate the model: Evaluate the performance of the model on the testing data. This may involve calculating various metrics such as accuracy, precision, recall, and F1-score.

**How to Use 2SLS(Two-Stage Least Squares):-**
2SLS model is a statistical method used to estimate causal relationships between variables in the presence of endogeneity, which occurs when a predictor variable is correlated with the error term in a regression model.

steps to follow when using the 2SLS model:

Step-1

Identify the endogenous variable(s): An endogenous variable is a predictor variable that is correlated with the error term in a regression model. You need to identify the variable(s) that might be endogenous in your model.

Step-2

Find an instrumental variable(s): An instrumental variable is a variable that is correlated with the endogenous variable but not with the error term in the regression model. You need to find an instrumental variable that is correlated with the endogenous variable(s) and has no other direct effect on the dependent variable.

Step-3

Estimate the first stage regression: In the first stage, you regress the endogenous variable(s) on the instrumental variable(s) and any other relevant variables. This will give you the predicted values of the endogenous variable(s)

Step-4

Estimate the second stage regression: In the second stage, you regress the dependent variable on the predicted values of the endogenous variable(s) from the first stage, the instrumental variable(s), and any other relevant variables.

Step-5

Check for validity of the instrumental variable(s): It is important to check the validity of the instrumental variable(s) to ensure that they meet the required criteria for use in the 2SLS model. This includes testing for the relevance and exogeneity of the instrumental variable(s).

Step-6

Interpret the results: Interpret the coefficients from the second stage regression to make causal inferences about the relationship between the dependent variable and the endogenous variable(s).

**When To Use The Ordinary Least Squares (OLS) model:-**
The Ordinary Least Squares (OLS) model is a statistical method used to estimate the relationship between a dependent variable and one or more independent variables. OLS is a popular method for linear regression analysis, and it assumes that the relationship between the dependent variable and independent variables is linear.

OLS can be used in many situations where we want to model the relationship between a dependent variable and one or more independent variables, such as in economics, finance, social sciences, and engineering. OLS is particularly useful when we have a large dataset with many observations, as it is a relatively simple and efficient method.

OLS is generally appropriate when the following assumptions are met:

Linearity: The relationship between the dependent variable and independent variables is linear. Independence: The errors are independent of each other. Homoscedasticity: The variance of the errors is constant across all values of the independent variables. Normality: The errors are normally distributed with a mean of zero. If these assumptions are not met, the OLS model may not provide accurate or reliable estimates of the parameters. In such cases, alternative regression models such as weighted least squares or robust regression may be more appropriate


**When To Use The Logistic Regression**
Logistic regression can be used in various applications such as:

Predicting the likelihood of a person buying a product or not, based on demographic data like age, income, etc. Identifying the likelihood of a patient having a particular disease based on their symptoms. Predicting the probability of default on a loan based on credit score, income, etc. Logistic regression can also be used in multi-class classification problems, where the dependent variable can take more than two values. In such cases, we can use multinomial logistic regression or softmax regression to model the probability of each class.

Overall, logistic regression is a useful tool for predicting binary or multi-class outcomes in various fields, such as marketing, healthcare, finance, and many others.

**When To Use Two-stage least squares (2SLS):-**

Two-stage least squares (2SLS) model is a statistical technique used to estimate the parameters of a linear regression model when the independent variables are potentially endogenous, meaning that they are correlated with the error term of the model.

2SLS is particularly useful when dealing with endogeneity in a regression model. Endogeneity can arise when there is a two-way causal relationship between the dependent variable and one or more independent variables, or when there are omitted variables that are correlated with the independent variables. In such cases, ordinary least squares (OLS) regression, which assumes that the independent variables are exogenous, can produce biased and inconsistent estimates of the parameters.

The 2SLS model is a two-stage procedure that involves first estimating a set of instrumental variables (IVs) that are uncorrelated with the error term, and then using these IVs to obtain consistent estimates of the parameters in the main regression model. IVs are variables that are correlated with the endogenous independent variables, but not with the error term of the model.

2SLS is typically used in econometric analysis and is particularly useful when dealing with issues such as measurement error, simultaneity, and omitted variables. It is commonly used in the analysis of panel data, time series data, and cross-sectional data.
