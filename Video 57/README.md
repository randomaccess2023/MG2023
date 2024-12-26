# `K-Nearest Neighbors (KNN)` using Scikit-Learn

__KNN__ is a supervised machine learning algorithm which has been used for a classification task in this example. This algorithm determines the _class_ of a new data point based on a majority vote. The majority here is basically its nearest neighbors `K` (`K` is an integer) in the feature space. The label of the majority decides the class of the new data.

I used `wheat_seed.csv` dataset for this example. The dataset is available in the repository. This dataset contains three varieties of wheat seed. I initially chose `K=4` but later found out that `K=2` gives the same result as `K=4` and `K=10` for this dataset. In that case, a lower value of __K__ is the desirable one.

I selected two features (`Length of the nucleus` and `Width of the core`) to display the three classes of the dataset in a 2D scatter plot without scaling the features:

![selected_feature_visualization.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2057/selected_feature_visualization.png "selected_feature_visualization.png")

I obtained this confusion matrix using `K=4`:

![confusion_matrix.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2057/confusion_matrix.png "confusion_matrix.png")

I also plotted the scores for different values of __K__:

![scores_for_different_k.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2057/scores_for_different_k.png "scores_for_different_k.png")

### The full code is available in `knn.ipynb` file.
