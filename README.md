This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The objective of the dataset is to diagnostically predict whether or not a patient has diabetes, based on certain diagnostic measurements included in the dataset. Several constraints were placed on the selection of these instances from a larger database. In particular, all patients here are females at least 21 years old of Pima Indian heritage.
I have done EDA which includes descriptive statistics. 
Then I have used median values of the respective outcomes to fill the missing values in all the columns. The primary reason behind using the median value is the presence of outliers.
In first notebook, I have build the logistic regression model by scalling the model using Power Transformer method and tuned the hyper-parameters and finally used bagging classifier to get the best model.
In second notebook, I have build the KNN model and tuned the hyper-parameter and finally used bagging classifier to get the best model. 
In third notebook, I have build the DecisionTree Classifier model and tuned the hyper-parameter and finally used bagging classifier to get the best model.
In fourth notebook, I have build the Support Vector Classifier model and tuned the hyper-parameter and finally used bagging classifier to get the best model.
In fifth notebook, I have build the RandomForest Classifier model and tuned the hyper-parameter and finally used feature importance to get the most important feature.
Out of all the models, RandomForest Classifier gave the best output across the performance metrics and bagging model of KNN was the close second with .90 roc-auc-score. However if the priority is to identify most diabetic patient correctly, Decision Tree model can also be a good option.
In feature extraction through RandomForest, Insulin was the most important feature in predicting whether the patient is diabetic or not. Intutively also insulin was supposed to be the most important factor as it decide the level of sugar in the body. As per my expectation, glucose should have been the close 2nd, but it wasn't, skin thickness was the 2nd best feature followed by glucose.
