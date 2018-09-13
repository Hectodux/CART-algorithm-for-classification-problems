# CART-algorithm-for-classification-problems
The three files in this project are used to run a CART(Classification and Regression Trees) algorithm on a certain dataset, currently the algorithm is working for classification problem.
The algorithm works by splitting the dataset using each value for each attribute and then it uses the gini_index function to evaluate which split has the lowest cost(Is more "pure").
After that it uses the best split to build a binary tree and tries to make prediction with it.
The final result is the evaluation made by cross validation split

The file to use is the main.py file it takes 4 arguments:

* the filename of the dataset
* the number of folds for the cross validation split
* the maximum depth for our tree
* the minimum number of rows per node

The algorithm may take a while since the splitting technique is very greedy and the gini_index function needs to be calculated on every split.
