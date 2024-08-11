# Machine Learning: `LightGBM Classifier` using Python API

Light Gradient-Boosting Machine (`LightGBM`) is a gradient-boosting algorithm for machine learning. It uses a histogram-based method in which data is bucketed into bins using a histogram of the distribution.

I used `magic_gamma_telescope.csv` dataset for this example. The dataset is available in the repository. It contains 2 types of entities in the target column: __g=gamma(signal) & h=hadron(background)__.

I obtained the following confusion matrix:

![confusion_matrix.jpg](https://github.com/randomaccess2023/MG2023/blob/main/Video%2070/confusion_matrix.jpg "confusion_matrix.jpg")

This is the plot of feature importance:

![feature_importance.jpg](https://github.com/randomaccess2023/MG2023/blob/main/Video%2070/feature_importance.jpg "feature_importance.jpg")

### The full code is available at `LightGBM_Classifier.ipynb` file.
