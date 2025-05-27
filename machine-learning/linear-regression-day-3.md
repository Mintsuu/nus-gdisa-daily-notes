# Introduction to Machine Learning
## Software Dev vs Machine Learning
- Software development cannot create a varying formula (the programmers decide the formula)
- Machine learning can adapt the formula based on the trained data
## Supervised vs Unsupervised Learning
- Supervised
  - Algorithms - logistic regression, KNN, decision tree, etc.
  - Lee Chiang will teach supervised learning
  - Linear regression for predicting a value
- Unsupervised
  - Clustering(aka Pattern Discovery)
    - Algorithms - K-means, Hierarchical Clustering, DBScan, etc. 
- Label/Outcome: The attribute that determines the outcome of the dataset
- Variables/Features: The attributes that contribute to the outcome of the dataset

## Exam Notes
- Regression important for exams

# Linear Regression 
## Validating the machine learning model
- 2 common types of validation to measure the accuracy of the linear regression model
  - Mean squared
  - R-squared
## Residuals (distance between the datapoint and the plotted regression line)
- The difference is a measurement of the accuracy of the model, which is why mean-squared and r-squared came about
- Rsquared can increase by just adding more independent variables to the model, which is why it might not be as accurate in the future

## Overfitting
- Model fits the training data well but performs poorly on new data

# Classification Learning
- Logistic regression
  - Uses a sigmoid function (aka the gaussian graph) to calculate the range of values??

## Validating accuracy
- Use confusion matrix
- F1 score
  - Precision: Num of correct positive results / Num of all positive results
  - Recall: Num of correct positive results / num of actual positive results


## Questions
- Why do all the residual validation methods use square? Why can't you just modulus the difference between yi and y(t) to get actual difference? What is the significance of squaring the difference?
- Is there a reason why 20-25% test to training data is the middle ground for machine learning? Is there a statistical significance of using 20-25%?
- Does it make sense to run a classification learning model on a dataset to determine features that have statistical significance to a outcome, before performing a linear regression on the shortlisted features?
