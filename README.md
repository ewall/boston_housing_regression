# Boston Housing Pricing - Decision Tree Regression Example

## Background

This is just a simple example of using decision trees for regression (not classification), using the Boston housing pricing dataset and Weka's REPtree implementation.

## Dataset

Boston Housing Pricing Dataset is archive on the UCI ML Reposity here:
https://archive.ics.uci.edu/ml/machine-learning-databases/housing/

However, there's an ARFF-formatted version ready for Weka here:
http://tunedit.org/repo/UCI/numeric/housing.arff

## Instructions

1) Load Weka version 3.8 or higher.
2) Open to the KnowledgeFlow GUI.
3) Load the file "boston_housing_dt_regression.kf".
4) Re-map the dataset to "housing.arff" if necessary.
5) Execute and view the results in the TextViewer node.

## Results

=== Evaluation result ===

Scheme: REPTree
Options: -M 2 -V 0.001 -N 3 -S 1 -L -1 -I 0.0

Correlation coefficient                  0.8818
Mean absolute error                      2.9752
Root mean squared error                  4.4418
Relative absolute error                 43.5023 %
Root relative squared error             47.2397 %
Total Number of Instances              405     
