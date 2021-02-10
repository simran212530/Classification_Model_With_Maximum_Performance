# Classification_Model_With_Maximum_Performance

---
## Outline

1. [Observation](#observation)
2. [Model - 1](#Model - 1 Analsysis)
3. [Model - 2](#Model - 2 Analsysis)
4. [Model - 3](#Model - 3 Analsysis)
5. [Dataset](#dataset) 
6. [Methodology](#methodology)
   * [Classification Techniques](#classification-techniques)
7. [References](#references)

---

## Project Description
### Observation from the model designs: 
The data was highly imbalanced (1.44% instances having ‘T’ value as 0 amongst the rest being 1s). Due to the numerical nature of the data, we have done some basic pre-processing like dropping records having null values and removing duplicates.

### Model - 1 Analsysis: 
Training on the entire dataset but a parameter ‘scale_pos_weight’ provided to inform the classifier about the ratio of the 0s wrt 1s.

Learning
We had a great time analysing the data provided to us. We experimented with
various under-sampling as well as over-sampling techniques like Random
Under/Oversampling, Tomek Links, Wilson’s ENN and SMOTE. We only
managed to carry out our checks with kNN, Decision Tree and RandomForrest
Classifiers. We experimented with tuning our hyper-parameters using
GridSearchCV and RandomSearchCV. It was an amazing learning experience by
getting familiar with the training and prediction times of different models and
tuning their hyper-parameters to the data’s convenience.

### Model - 2 Analysis: 
Undersampled the training data as to get twice the amount of samples having ‘T’ values as 1 than 0. Therefore, provided ‘scale_pos_weight’ appropriately.

### Model - 3 Analysis: 
Undersampled and then used the SMOTE technique to oversample the data to get a similar distribution. Applied ‘scale_pos_weight’ accordingly.

### Dataset
The following Dataset was used for making the model : https://www.kaggle.com/t/cb719aca29ab4452a3c048eec64e0608
Dataset: (uploaded on Kaggle)
Given Dataset size - 20,41,687 rows X 9 columns
Target variable - ‘T’


### Methodology
#### Classification Techniques
We had a great time analysing the data provided to us. We experimented with
various under-sampling as well as over-sampling techniques like Random
Under/Oversampling, Tomek Links, Wilson’s ENN and SMOTE. We only
managed to carry out our checks with kNN, Decision Tree and RandomForrest
Classifiers. We experimented with tuning our hyper-parameters using
GridSearchCV and RandomSearchCV. It was an amazing learning experience by
getting familiar with the training and prediction times of different models and
tuning their hyper-parameters to the data’s convenience.


### References:
https://machinelearningmastery.com/save-load-machine-learning-models-python-scikit-learn/
https://docs.python.org/2/library/pickle.html
https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_csv.html
https://towardsdatascience.com/understanding-auc-roc-curve-68b2303cc9c5
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.roc_auc_score.html#sklearn.m
etrics.roc_auc_score
