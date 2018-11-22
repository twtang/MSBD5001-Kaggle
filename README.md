# MSBD5001-Kaggle


## Note for running
1. Programming Language: Python 3 on Jupyter Notebook
2. Required packages: pandas, numpy, sklearn, statsmodels, datetime

## Feature engineering
1. if n_jobs = -1, change to 16
2. if n_classes = 2, change to 1
3. Create a new feature, x = log(max_iter * n_samples * n_features * n_classes / (1 + n_jobs))
4. Group n_jobs into (1, 2, and 2+)
5. Group penalty into ('elasticnet', 'l1' and 'l2 or none')
6. y = log(time)

## Model
Weighted linear regression (Degree 1 and 2) on x <br>
Fit weighted linear regression by groups (n_jobs and penalty) <br>
Weight is the exponential of normalized x <br>