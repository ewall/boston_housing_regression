# Boston Housing Pricing - Decision Tree Regression Example

## Background

This is just a simple example of using decision trees for regression (not classification), using the Boston housing pricing dataset with the [REPtree](http://weka.sourceforge.net/doc.dev/weka/classifiers/trees/REPTree.html) algorithm in [Weka](https://www.cs.waikato.ac.nz/ml/weka/).

## Dataset

Boston Housing Pricing Dataset is archive on the UCI ML Reposity here:
[https://archive.ics.uci.edu/ml/machine-learning-databases/housing/](https://archive.ics.uci.edu/ml/machine-learning-databases/housing/)

However, there's an ARFF-formatted version ready for Weka here:
[http://tunedit.org/repo/UCI/numeric/housing.arff](http://tunedit.org/repo/UCI/numeric/housing.arff)

## Instructions

1. Load Weka version 3.8 or higher.
2. Open to the KnowledgeFlow GUI.
3. Load the file `boston_housing_dt_regression_results.kf1`
4. Re-map the dataset to `housing.arff` if necessary.
5. Execute and view the results in the TextViewer node.

## Results

Results of a 10-fold cross validation training on 80% of the data, tested on the remaining 20%:

| Metric | Value |
| ------ | ----- |
| Correlation coefficient | 0.9008 |
| Mean absolute error | 2.83 |
| Root mean squared error | 4.1201 |
| Relative absolute error | 41.3798 % |
| Root relative squared error | 43.818  % |
| Total Number of Instances | 405 |

Hyperparameters:

* minimum number of instances per leaf: 1
* minimum numeric class variance proportion: 0.001
* pruning enabled, using 3 folds for validation
* allow maximum tree depth


Command Line:

`REPTree -M 1 -V 0.001 -N 3 -S 1 -L -1 -I 0.0`

