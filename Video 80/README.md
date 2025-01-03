# `K-fold cross validation` using Scikit-Learn

`K-fold cross validation` is a technique used for evaluating the performance of machine learning models. It uses different portions of the dataset as train and test sets in multiple iterations and helps a model to generalize well on unseen data.

Scikit-Learn's __train_test_split__ method uses a fixed set of samples as the train set and the rest of the samples outside the train set as the test set, which can often result in high variance. On the other hand, the __K-fold cross validation__ method provides a more robust estimate of a model's performance.

I used `car_evaluation.csv` dataset for this example. The dataset is available in the repository. It has 4 evaluation criteria: __unacceptable, acceptable, good & very good__.

After performing cross validation over the entire dataset, we calculate the mean score on all the folds. _**If we use multiple models, we decide to choose the model with a better mean score than the others for a particular dataset**_.

### The full code is available in `k_fold_cv.ipynb` file.

[![kfold](https://markdown-videos-api.jorgenkh.no/youtube/IbnqJeecxIc)](https://youtu.be/IbnqJeecxIc)
