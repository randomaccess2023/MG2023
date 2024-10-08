# `GridSearchCV` using Scikit-Learn

`GridSearchCV` is a function that comes with Scikit-Learn library and it is a process for tuning hyperparameters in machine learning models. The performance of a machine learning model significantly depends on the selection of hyperparameters. `GridSearchCV` loops through a predefined set of hyperparameters and selects the optimal values from them after exhaustively considering all parameter combinations.

I used `early_stage_diabetes_risk_prediction.csv` dataset for this example. The dataset is available in the repository. It's target column contains 2 unique entities: __Positive & Negative__.

After trying several combinations of two different hyperparameters (__`n_estimators` & `max_depth`__) for three different machine learning models (__`Random Forest Classifier`, `Extra Trees Classifier` & `Gradient Boosting Classifier`__), we obtained the following best results:

| selected_model | best_score_obtained | best_params_obtained |
| ---: | ---: | ---: |
| RandomForestClassifier(random_state=42) | 0.946154 | {'max_depth': 5, 'n_estimators': 10} |
| ExtraTreesClassifier(random_state=42) | 0.951923 | {'max_depth': 5, 'n_estimators': 10} |
| GradientBoostingClassifier(random_state=42) | 0.959615 | {'max_depth': 5, 'n_estimators': 5} |

Among them, We notice that __Gradient Boosting Classifier__ is better than other two models.

### The full code is available at `GridSearchCV.ipynb` file.

[![gridsearchcv](https://markdown-videos-api.jorgenkh.no/youtube/niEJvCcw8mM)](https://youtu.be/niEJvCcw8mM)
