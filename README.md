# DataMining

### Assignment 1
Take your data set from the previous assignment and perform partitioning unsupervised learning. You need to use diagnostics to

decide which algorithm to choose, and
decide on the number of clusters.
Select a final model and explain why you selected it.

Consider using these functions:

kmeans()
cluster::clara()
cluster::fanny()
cluster::pam()
other partitioning functions from other packages in R
 
Take your data set from the previous assignment and perform hierarchical unsupervised learning. You need to use diagnostics to decide which algorithm to choose, the parameters to use, and the number of clusters.

Build a hierarchical clustering that is a good model for outlier detection.
Build a hierarchical clustering that is a good model for partitioning your data into (approximately) equal sized groups.
Select two final models, and explain why you selected them.

Consider using these functions:
hclust()
cluster::agnes()
cluster::diana()
cluster::mona()
other hierarchical functions from other packages in R

### Assignment 2
Perform dimension reduction on your predictor variables.
1) Convert all categorical and ordinal predictor variables data to dummy variables
Note: normally we want to avoid including categorical or ordinal data in PCA, we are including them to maintain the number of dimensions of the data.
2) Perform rank two principal component analysis on your predictor variables
scatterplot the two components; use your target variable to determine the point character/point color/point size etc. 
3) Perform rank two t-SNE analysis on your predictor variables
scatterplot the two components; use your your target variable to determine the point character/point color/point size etc.
4) Perform nonnegative matrix factorization with two topics on your predictor variables
You will need to change the range of predictor variables with negative values
scatterplot the two basis vectors; use your target variable to determine the point character/point color/point size etc. 
Write a paragraph describing which technique gave the best results.

### Assignment 3
Take your data and build multiple Bayesian network models, calculate network scores, then select your best model. Use the bnlearn package in R to fit the models.

Build your models :

Build a Bayesian network using a constraint-based algorithm.
Build a Bayesian network using a score-based algorithm.
Build a Bayesian network using a hybrid algorithm.
Build a Bayesian network using a local discovery algorithm.
Score your models :

Read the bnlearn documentation regarding network-scores.
Select a network-score. Write a short paragraph why you chose that measurement for model selection.
Run bnlearn::score() on each model.
Present the values in a sorted table (largest to smallest).
State which model is the best according to the table.

Visualize your final model:

Use graphviz.plot() to visualize the selected model.
Predict your target variable:

For the target variable that you used in previous assignments, for each observation in your training set, predict the target variable.
Choose a method to evaluate model fit, MSE, Chi-squared, MAE, R^2, adjusted R^2, confusion matrix, sensitivity, specificity, AUC, etc.
Write a short paragraph stating if you feel that you could use the model at work. What type of projects could you use the model for?
Note: For this assignment, you are evaluating the models on your training data. We are doing this to make it easier for you to complete the assignment. On real projects at work, you would use the train-validate-test paradigm when building models.
