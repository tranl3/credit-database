# credit-database

Consider the provided dataset “credit.sav” that contains sample data on 1000 past credit applications
at a bank. Each application is described by 32 different variables. Explanations of each variable can
be found in “variables.xls“.

Each application is rated as either “good” or “bad” credit and is encoded in the RESPONSE variable as 1 or
0, respectively. We are interested in creating a model to help us predict whether new applicants pose
a credit risk for the bank.

Tasks to cover:
(a) Import necessary libraries, load the data, and run some exploratory data analysis / summary
statistics.
(b) Visualize the absolute and relative distribution of the RESPONSE target variable.
(c) Preprocess the data into a feature matrix X and a target vector y.
(d) Split the data 70:30 into training and testing. Fix the seed for the random split to 1234 using
the random_state=1234 argument in scikit-learn’s train_test_split() function.
(e) Check that the splitwas successful by visualizing the relative distribution of the response/target
variable in the original dataset, as well as in the training and testing partition.
(f) Using scikit-learn’s library, build a Decision Tree model that predicts the response/target variable.
How accurate is your model on the unseen testing data?
(g) You will have noticed by now that the response labels are imbalanced. Re-balance the data
using SMOTE.
(h) Build a second Decision Tree model using the rebalanced data. How accurate is your model on
the unseen testing data?
(i) Evaluate both of your models using a confusion matrix and ROC chart (including the AUC
values for both models). Do you find one model clearly outperforming the other?
(j) Using MS Excel, determin the expected value of both models. Assume that the (average) net
profit from the credit decisions is as follows:
• Granting credit for an actual “good” case: 200AC,
• Granting credit for an actual “bad” case: 􀀀500AC.
Does taking the misclassifcation costs into account change the model performance?
(k) Write a brief conclusion on which model you would advise to deploy.
