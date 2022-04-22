# Credit_Risk_Analysis
Module 1 Challenge

Abstract 

The purpose of this project is to create a machine learning model that is capable of predicting credit card risk (i.e. the level of risk a customer presents to the credit card company). The model will help credit companies more accurately avoid issuing credit cards to customers that likely cannot pay their debt, therefore saving the credit company money.

Data

The data used in this analysis was sourced from LendingClub, a lending services company. There exists 68,817 records and 86 columns. There is a significant imbalance in the "loan status" classes: 
•	1 / low risk: 68470 records
•	0 / high risk: 347 records


Methods
Python 3 was used for all data wrangling and analysis via Jupyter Notebooks. First, several Imbalanced Learn sampling methods were tested to find the best approach to balancing the “loan status” classes. These sampling methods were then tested using a logistic classifier and compared. 
Resampling Methods
•	Naive Random Oversampling - RandomOverSampler algorithm
•	SMOTE Oversampling - SMOTE algorithm
•	Undersampling – RandomUnderSampler algorithm
•	Combination (Over and Under) Sampling - SMOTEENN algorithm

Next, two different ensemble modeling algorithms were tested to find the best performer. 
Ensemble Methods
•	Balanced Random Forest Classifier 
•	Easy Ensemble AdaBoost Classifier
The results of each model were measured using three methods:
1.	Confusion matrix: see table below
	Predicted True	Predicted False
Actually True	TRUE POSITIVE	FALSE NEGATIVE
Actually False	FALSE POSITIVE	TRUE NEGATIVE
2.	Balanced accuracy score: defined as the average of recall obtained on each class
3.	Imbalanced classification report: report compiles the state-of-the-art metrics of precision/recall/specificity, geometric mean, and index balanced accuracy of the geometric mean

Results

Resampling Results
•	Naive Random Oversampling 
 
•	SMOTE Oversampling 
 
•	Undersampling 
 
•	Combination (Over and Under) Sampling 
 

Ensemble Results
•	Balanced Random Forest Classifier  
•	Easy Ensemble AdaBoost Classifier 

Discussion
The resampling methods all performed similarly but the combination sampling did score better overall by a small margin. However, the ensemble algorithms greatly out performed all of the resampling methods with the AdaBoost doing the best overall. Therefore, I would recommend the AdaBoost algorithm to predict credit card risk. 
