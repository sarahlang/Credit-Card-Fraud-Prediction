# Fraud Prediction from Credit Card Data

Data Files: https://entuedu-my.sharepoint.com/:f:/g/personal/n2203082b_e_ntu_edu_sg/EvbAYvY8kQRBpxJclbmSEEEBebQZspKpv6iyP5o6ujo0Qw?e=IPjfJU

ABOUT THE DATASET

With the rising credit card fraud cases in recent years, it is important for us to understand more about credit fraud, combat identity fraud and stop fraudulent transactions. This project is a credit card fraudulent detector/predictor using a simulated credit card transactions dataset from GitHub for the duration of Jan 1st 2019 to Dec 31 2020. It covers information of credit cards of more than 1000 customers doing transactions with a pool of 800 merchants. The key objective of this detection system is to identify and predict the factors that cause suspicious events in the future using train and test datasets.


DATA EXPLORATION AND CLEANING 

Yuezhu worked mostly on this part of the project. In the data exploration process, we dived into the correlation between whether the transaction is fraud (our y variable) and each variable. We calculated and analyzed the fraud rate for values inside of each variable and used different types of graphs, such as bar charts, violin charts, histograms, word clouds, etc., to visualize each variable’s value breakdown. We also performed variable-specific data analysis with regards to the unique characteristics of each variable. We dropped customers’ information--sensitive variables such as credit card number, customer's name and date of birth--and generated new variables  from the original variables such as the customers’ age and the transaction day of the week, to further analyze the possible factors that correlated with credit fraud in our dataset.


MODEL TRAINING AND TUNING

Xinyu worked mostly on this part of the project. We cleaned the data and encoded the data using one-hot encoding and label encoding. We used four base machine learning models to discover patterns in the underlying dataset, namely Gaussian Naive Bayes, Decision Tree, Logistic Regression, and Random Forest. Since we have a rather imbalanced dataset with much more non-fraudulent cases than fraudulent cases (only 0.5% of all transactions), all four models achieved more than 99% precision, recall, F-1 score for detecting non-fraudulent cases while the scores are much lower for detecting fraudulent cases. Therefore, we tuned our model using SMOTE resampling by over-sampling the fraudulent data to make our dataset more balanced, and the aforementioned scores improved for all four models. Our conclusion is that Random Forest model outperforms other models with its efficiency with large datasets and high accuracy for classification.


REFERENCES 

Data source: https://www.kaggle.com/datasets/kartik2112/fraud-detection
