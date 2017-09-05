# Machine Learning with Python

**Problem Statement:** Use Machine Learning to process and transform Pima Indian data to create a prediction model. This model must predict with people are likely to develop diabetes with 70% or greater accuracy.


#### *ML Algorithm for predicting patients Diabetes* using Supervised Learning
![alt text](RoleOfAlgorithm.png)

Candidate Algorithms
1. Naiave Bayes
2. Logic Regression
3. Decision Tree

**Naive Bayes** - Bases on likelihood and probability on previous data, combined with the probability with nearby feature values. *Ex. How often the person having high blood pressure correlate with having diabetes.*  It makes the navie assumption that all fo the features we pass in are independent of each other and equally impact the result. This algorithm requires a small amount of data to train.  
![alt_text](naivebayes.png)

**Logistic Regression** - Returns a Binary result. The algorithm measures values of each feature and weights them based on their impact on the result. The result and values are mapped against a curve between 1 and 0, which is equivalent to diabetes or no diabetes in our case.
![alt_text](logicregression.png)

**Decision Tree** - Uses a binary tree structure, which each node making a decision based upon values of the feature. At each node, the feature value causes us to go down one path or another. May require alot of data to determent the outcome. 
![alt_text](decisiontree.png)


### Training
Split data between training and test

**scikit-lean** will be used for training functions


#### Confusion Matrix
The Confusion Matrix provides a matrix that compares the predicted natural results for diabetes. 
The columns are the predicted values. The left column is predicted true. 
The right column is predicted false. 
Rows are the actual values, top row is actual true, bottom row is actual false. 


    52 28 
    33 118
 
    TP FP       True-Positive   Flase-Positive
    FN TN       Flase-Negitive  True-Negitive
    
    
|     |      |
|-------------------------------------------------------|-----------------------------------------------------------|
| TP - Actual diabetes and predicted to be diabetes     | FP - Actual not diabetes but predicted to be diabetes     |
| FN - Actual diabetes but predicted to be not diabetes | TN - Actual not diabetes and predicted not to be diabetes |


    
"Perfect" Classifier

    80  0
    0   151
    
### Random Forest
Its an ensemble algroritm which uses binary decision trees

Fits multiple trees with subsets fo data

Averages tree results to improve performance and control overfitting


*If accuracy is very high with Training data but not with Test data, then the algorithm has learned the training data too well.*

### Fixing Overfitting
Regulariation hyperparameter




 