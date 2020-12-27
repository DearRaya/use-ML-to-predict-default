Submission for [Kaggle challenge](https://www.kaggle.com/uciml/default-of-credit-card-clients-dataset) to predict the probability of various demographics defaulting on their credit card payment

## Questions I was trying to address:
* What are the dependent vairables for someone to default next month?
* What are the weights for these variables?
* What are some possible approaches?
* What might be the appropriate model?

## Step-by-step analysis
1. Tried to understand the data first, categorical/discrete vs continuous
2. Ruled out possible solutions such as senario analysis(i.e., if Sex == 1 && if Marriage == 1 && Education == 1 && Age >= 20 && Age <= 30) or isolating dependent variables(i.e., only look at Sex == 1 and all data points under Sex == 1)
3. Exploratory Anlysis by visualization
4. Normalization
5. Decided on models based on the mix of categorical/discrete vs continuous data points
6. Applied decision tree(random forest), multivariate linear regression

## Conclusion
* Random Forest Accuracy: 81%
* Decision Tree: 72%
* Biggest weight using multivariate linear regression is PAY_0 with beta of 0.968, smallest weight is BILL_AMT1 with beta of -0.66
