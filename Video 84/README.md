# `HistGradientBoostingClassifier` using Scikit-Learn

`HistGradientBoostingClassifier` classifier implements gradient boosting using histogram-based techniques. It aggregates feature values into discrete bins (histograms) and processes these bins instead of individual samples. This algorithm is faster and more memory-efficient for large datasets. It can handle datasets with millions of samples due to its binning strategy.

I used `letter_recognition.csv` dataset for this example. The dataset is available in the repository. It's target column contains 26 capital letters in the English alphabet.

I obtained the following confusion matrix:

<img src="https://github.com/randomaccess2023/MG2023/blob/main/Video%2084/Confusion_Matrix.png" width="450" height="450">

### The full code is available at `Hist_GBC.ipynb` file.
