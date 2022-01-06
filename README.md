We are given the data of direct marketing campaigns (phone calls) of a Portuguese banking institution. The classification goal is to predict if the client will subscribe to a term deposit or not(target variable y). 

The dataset was picked from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/bank+marketing). This was also a competition on Kaggle.

This is a binary classification problem.

I've performed some Exploratory Data Analysis (EDA) to determine which features are essential using Pearson's Correlation, if there's any data missing and needs to be imputed, tackled the class imbalancing problem, determine whether the dataset needs any cleaning/wrangling and also performed some routine data pre-processing.

Missing values were imputed using two mechanisms - 

* Used Maximum Likelihood Estimation (MLE) to guage the empirical probability distribution, which was sampled from to guess missing values.
* Used kNN and a Euclidean Distance metric to determine nearest neighbors and then impute missing values.


I've implemented Binary Logistic Regression, RBF Kernel SVM & XGBoost and drawn comparisons between the three using the AUC performance metric since we have imbalanced classes here.

I've also tried to provide some insight into how this analysis could be useful to the bank in determining potential customers, so they could target their ad campaigns accordingly.
