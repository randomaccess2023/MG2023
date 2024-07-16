# `Random Forest` using Scikit-Learn

`Random Forest` is a supervised machine learning algorithm which has been used for a classification task in this example. It uses multiple decision trees and takes a majority vote on them to reach a single decision. __Random Forest__ is an _ensemble learning_ method.

I used `secondary_mushroom_dataset.csv` for this example. The dataset is available in the repository. This dataset contains two types of mushrooms: __edible & poisonous__. It has 20 features. But, 9 of them contain null values and I dropped them before fitting the dataset to the model. I used 5 trees to train the `Random Forest` model.

I obtained the following confusion matrix:

![confusion_matrix.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2061/confusion_matrix.png "confusion_matrix.png")

This is the plot of feature importance:

![feature_importance.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2061/feature_importance.png "feature_importance.png")

### The full code is available at `random_forest.ipynb` file.
