# `ExtraTreesClassifier` using Scikit-Learn

`ExtraTreesClassifier` is a supervised machine learning algorithm. It is a type of ensemble learning technique which fits a number of randomized decision trees (i.e., extra trees) on various sub-samples of the dataset. It contributes to reducing the variance of the model and results in less overfitting.

I used `Ionosphere.csv` dataset for this example. The dataset is available in the repository. It contains 2 types of radars: __b & g__ for _bad_ and _good_, respectively.

I obtained the following confusion matrix:

<img src="https://github.com/randomaccess2023/MG2023/blob/main/Video%2078/confusion_matrix.jpg" width="450" height="450">

I plotted one of the trees:

<img src="https://github.com/randomaccess2023/MG2023/blob/main/Video%2078/plot_a_tree.jpg" width="850" height="550">

This is the plot of feature importance:

<img src="https://github.com/randomaccess2023/MG2023/blob/main/Video%2078/feature_importance.jpg" width="500" height="400">

### The full code is available in `ExtraTreesClassifier.ipynb` file.
