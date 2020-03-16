# startup-classification

Machine learning Project

I have used the startup dataset (https://www.kaggle.com/arindam235/startup-investments-crunchbase) and applied various machine learning algorithms on it to predict wether the startup wil or run or not given the various funding rounds.

Target variable is Status (changed it to binary value -- considered running and acquired in same category :1)

Step1: Done preprocessing of data i.e imputing NA's , changing categorical values into one hot vectors and binary values and removing unwated row/columns

Used MinMax Scaler to scale the dataset

Methods Used:

1. KNN classification:Applied KNN method with cross validation and Grid search CV to find the best accuracy score and best hyperparameter i.e best value of N = 11 and score = 0.94649

2. Applied logistic regression method with cross validation to get best possible score of 0.94644

3. Applied SVM (support Vector Machine) method using grid search.
    
    3.a Parameters used  [{'C': [1, 10], 'kernel': ['linear']}]
        scoring = 'accuracy',cv = 5         
                           
    3.b Parameters used   [{'C': [1, 10, 100, 1000], 'kernel': ['rbf'], 'gamma': [0.1, 0.2, 0.3, 0.4, 0.5, 0.6]}]
        scoring = 'accuracy',cv = 5
    
    3.c parameters used    [{'C': [1, 10, 100, 1000], 'kernel': ['poly'], 'degree': [2,3,4,5]}]
        scoring = 'accuracy',cv = 5
 

              
              
