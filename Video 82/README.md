# `RandomizedSearchCV` using Scikit-Learn

`RandomizedSearchCV` is a hyperparameter tuning technique that comes with the Scikit-Learn library. It explores a predefined search space of hyperparameters and randomly selects a few combinations to evaluate model performance.

Unlike GridSearchCV which systematically examines all the possible combinations, RandomizedSearchCV selects a fixed number of combinations randomly.

If the hyperparameter search space is very large, RandomizedSearchCV tends to become a more efficient method for the purpose of hyperparameter tuning. On the other hand, GridSearchCV is a more suitable option if the search space is relatively small and computationally feasible.

I used `indian_liver_patient_dataset.csv` dataset for this example. The dataset is available in the repository. Its target column contains 2 unique entities: __1 & 2__ that denote _Liver Patient_ and _Non Liver Patient_, respectively.

I used three different machine learning models (__Random Forest Classifier__, __K Neighbors Classifier__ & __Decision Tree Classifier__) and randomly selected 15, 8 & 5 hyperparameter combinations out of 27, 18 & 9 possible combinations, respectively. The following best results were obtained:

| selected_model | best_score_obtained | best_params_obtained |
| ---: | ---: | ---: |
| RandomForestClassifier(random_state=42) | 0.718486 | {'n_estimators': 10, 'max_depth': 5, 'criterion': 'gini'} |
| KNeighborsClassifier() | 0.701304 | {'weights': 'uniform', 'n_neighbors': 4, 'metric': 'euclidean'} |
| DecisionTreeClassifier(random_state=42) | 0.706402 | {'max_depth': 4, 'criterion': 'log_loss'} |

Among them, We notice that __Random Forest Classifier__ is better than other two models.

### The full code is available in `RandomizedSearchCV.ipynb` file.

[![randomizedsearchcv](https://markdown-videos-api.jorgenkh.no/youtube/naM4AwY3WoY)](https://youtu.be/naM4AwY3WoY)
