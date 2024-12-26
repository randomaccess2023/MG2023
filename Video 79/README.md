# `GradientBoostingClassifier` using Scikit-Learn

`GradientBoostingClassifier` is a supervised machine learning algorithm. It builds an additive model in a forward stage-wise fashion and allows for the optimization of arbitrary differentiable loss functions.

I used `credit_approval.csv` dataset for this example. The dataset is available in the repository. Its target column contains 2 types of unique values: __`+` & `-`__ most probably to indicate whether credit will be approved or not.

I obtained the following confusion matrix:

<img src="https://github.com/randomaccess2023/MG2023/blob/main/Video%2079/confusion_matrix.jpg" width="400" height="400">

This is the plot of feature importance:

<img src="https://github.com/randomaccess2023/MG2023/blob/main/Video%2079/feature_importance.jpg" width="480" height="380">

### The full code is available in `GBC.ipynb` file.
