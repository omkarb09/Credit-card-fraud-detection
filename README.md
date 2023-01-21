# Credit-card-fraud-detection
Code for the project in jupyter notebook. Dataset for credit card transactions masked using PCA was used to fit a logistic regression model to classify fraudulent transactions.

-	Logistic regression is the machine learning methods used for classification
-	The approach selected here is binary logistic regression as the feature ‘Class’ has two values (0 = not fraudulent, 1= fraudulent)
-	Two logistic regression models are created. One is the full model which has all the features and the other is a partial model which omits non-correlated features.
-	The two models are compared based on various metrics such as precision, recall, f1-score & ROC 

Logistic regression
-	The data was divided into training (75%) and test data (25%)
-	Counts of target feature ‘Class’ to check the distribution of values. 284315 values were 0 and 492 values were 1.
-	Plotting correlation heatmap to identify which features are correlated with ‘Class’. Features V4, V8, V13, V15, V22, V23, V24, V25 and V26 have no meaningful correlation with ‘Class’.
[image](https://user-images.githubusercontent.com/44408619/213869395-8a346e2e-8606-42fc-8671-9ca4d51b5dbc.png)

 -	Two logistic regression models are created. One is the full model which has all the features and the other is a partial model which omits non-correlated features (features mentioned above).
-	Full model score Vs Partial model score
![image](https://user-images.githubusercontent.com/44408619/213869410-bc856393-9768-41de-82ae-1ba0c23c62ec.png)
![image](https://user-images.githubusercontent.com/44408619/213869419-13771e98-8de0-4898-bd60-91f60de9ed68.png)

-	Full model classification report Vs Partial model classification report
![image](https://user-images.githubusercontent.com/44408619/213869450-dabc90d1-d638-430e-87dc-bf85e439d59c.png)
![image](https://user-images.githubusercontent.com/44408619/213869453-acb3530a-6a7d-4106-ac03-79fdb2ee3701.png)

-	Full model ROC vs Partial model ROC
![image](https://user-images.githubusercontent.com/44408619/213869484-652a8a3e-2b19-4f0e-bc71-44e19ab0d6de.png)
![image](https://user-images.githubusercontent.com/44408619/213869488-e9a72587-6e26-442a-b624-8d8fff9903c2.png)

Things achieved through the project
-	Exploratory Data Analysis of the Dataset. Getting the counts of target feature ‘Class’ to check the distribution of values, getting correlation between all features and plotting correlation heatmap to identify which features are correlated with ‘Class’
-	Splitting the dataset into Training and Testing set
-	Implementation of the Logistic Regression model for all features (full model).
-	Calculation model score for full model. Creating confusion matrix
-	Creating classification report which includes precision, recall, f1-score for full model. Plotting ROC curve for full model
-	Creating second Logistic Regression model which omits non-correlated features (partial model)
-	Performing the same steps for the partial model as performed above for the full model. Comparing the two models.
	 
