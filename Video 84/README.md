# `HistGradientBoostingClassifier` using Scikit-Learn

`HistGradientBoostingClassifier` implements gradient boosting using histogram-based techniques. It aggregates feature values into discrete bins (histograms) and processes these bins instead of individual samples. This algorithm is faster and more memory-efficient for large datasets. It can handle datasets with millions of samples due to its binning strategy.

I used `letter_recognition.csv` dataset for this example. The dataset is available in the repository. Its target column contains 26 capital letters in the English alphabet.

I obtained the following confusion matrix:

<img src="https://github.com/randomaccess2023/MG2023/blob/main/Video%2084/Confusion_Matrix.png" width="500" height="500">

### The full code is available in `Hist_GBC.ipynb` file.

[![Hist_GBC](https://markdown-videos-api.jorgenkh.no/youtube/VuEJ_6iVVyE)](https://youtu.be/VuEJ_6iVVyE)
