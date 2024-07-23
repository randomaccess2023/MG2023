# `Multinomial Naive Bayes` using Scikit-Learnn

`Multinomial Naive Bayes` is a supervised machine learning algorithm which has been used for a classification task in this example. It is suitable for classification with discrete features (e.g., word counts for text classification). It normally requires integer feature counts but, fractional counts may also work in practice.

I used `financial_sentiment_dataset.csv` for this example. The dataset is available in the repository. It contains the sentiments for financial news headlines from the perspective of a retail investor. The sentiments are categorized into three types: __negative, neutral, or positive__.

_Count vectorizer has been used to convert the news headlines into numerical vector representation of token counts_.

This shows the amount of unique sentiments in the dataset:

![unique_sentiments.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2063/unique_sentiments.png "unique_sentiments.png")

I obtained the following confusion matrix:

![confusion_matrix.png](https://github.com/randomaccess2023/MG2023/blob/main/Video%2063/confusion_matrix.png "confusion_matrix.png")

### The full code is available at `Multinomial_NB.ipynb` file.
