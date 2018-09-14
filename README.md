# CART-algorithm-for-classification-problems
The three files in this project are used to run a CART(Classification and Regression Trees) algorithm on a certain dataset, currently the algorithm is working for classification problem.
The algorithm works by splitting the dataset using each value for each attribute, then the gini_index function is used to evaluate which split has the lowest cost(Is more "pure").
The best split is then used to build a binary tree so that we can make prediction with it.
The final result is the evaluation made by cross validation splits.

To run the algorithm execute the main.py file with 4 arguments:

* the filename of the dataset
* the number of folds for the cross validation split
* the maximum depth for our tree
* the minimum number of rows per node

The other two .py files needs to be in same folder of the main.py file.
The algorithm may take a while since the splitting technique is very computationally expensive and the gini_index function needs to be calculated on every split.
