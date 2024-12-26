# `Isolation Forest` using Scikit-Learn

The purpose of using the `Isolation Forest` algorithm in Scikit-learn is to perform __anomaly detection__, which involves identifying rare or unusual data points that deviate significantly from the majority of observations. The algorithm is based on the principle that anomalies are few and different, making them easier to isolate through random partitioning.

`Isolation Forest` achieves this by constructing a collection of isolation trees (_binary trees_), where data points are recursively split using random feature selection and thresholds. Anomalies tend to have shorter path lengths in these trees because they are isolated faster than normal points. The algorithm assigns an __anomaly score__ based on the average path length across all trees, enabling the classification of points as _**normal**_ or _**anomalous**_.

This method is efficient, scalable to large datasets, and works well in high-dimensional spaces. Unlike traditional techniques, Isolation Forest does not assume a specific data distribution, making it robust in diverse scenarios. It is widely used in applications such as _fraud detection_, _network intrusion detection_, and _defect detection_ in manufacturing.

In summary, `Isolation Forest` in Scikit-learn is a powerful and versatile tool for detecting anomalies in unlabeled datasets, offering a computationally efficient and distribution-independent approach to identifying outliers.

This obtained the following scatter plots using `data.csv` dataset:

<p align="center">
<img src="https://github.com/randomaccess2023/MG2023/blob/main/Video%2085/scatter_plot.jpg" width="400" height="300">
<img src="https://github.com/randomaccess2023/MG2023/blob/main/Video%2085/scatter_plot_with_outliers.jpg" width="400" height="300">
</p>

### The full code is available in `isolation_forest.ipynb` file.
