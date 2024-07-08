# `Support Vector Machine (SVM)` using Scikit-Learn

`SVM` is a supervised machine learning algorithm which has been used for a classification task in this example. SVM can perform both linear and non-linear classification using the _kernel trick_. The main objective of `SVM` is to find the optimal hyperplane in an N-dimensional space that can separate the data points in different classes in the feature space.

I used `mushrooms.csv` dataset for this example. The dataset is available in the repository. This dataset contains two types of mushrooms: __edible & poisonous__. It has 22 features. I used a `polynomial` kernel with `degree` _2_ to train the `SVM` model and got __99.71%__ accuracy on the test set. The `gamma` and `regularization (C)` parameters were set to _auto_ and _0.2_, respectively.

#### _Feel free to change some of the parameters!_

I obtained the following confusion matrix:

![confusion_matrix.jpg](https://github.com/randomaccess2023/MG2023/blob/main/Video%2059/confusion_matrix.jpg "confusion_matrix.jpg")

## The full code is available at `svm.ipynb` file 
