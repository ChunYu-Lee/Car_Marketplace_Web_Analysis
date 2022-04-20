# Car_Marketplace_Web_Analysis
This is a project to predict the views on a car marketplace website and try to classify the tier of each car. <br />

First question, based on the data could I predict the tier of each car?  There are three tiers: Basic, Plus, Premium.<br />
![This is an image]()
The reason why I pick BalancedRandomForest model is because this dataset has imbalance issue and high dimensions. Random Forest has the class weight parameter, bootstrap to avoid the imbalance issue and increase randomized and it is not hard to train with high dimensions dataset. Unlike SVM or KNN. Also, it performs well in Random Forest than Naive Bayes in this dataset. <br />

The result from the BalancedRandomForest model is Macro F1 score: 0.527. <br />


Second question, based on the data could I predict the views for each post? <br />
Because the views are a continuous number I use regression models. However, we face the outlier issue in detail views. Therefore, I use linear and non-linear models to predict the detail views because of the difference in robustness on outliers. <br />
The result from the Random Forest Regressor model is R-Squared: 0.7, MAE: 40.53.
