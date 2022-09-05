# Credit_Risk_Analysis

## Overview of the analysis:
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Finally, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results:
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.
- RandomOverSampler
  - An accuracy score was calculated for the model:
    0.653
  
  - A confustion matrix was generated:
     ([[   72,    29],
       [ 6943, 10161]])
  
  - An imbalanced classification report was generated:
                       pre       rec       spe        f1       geo       iba       sup

        high_risk       0.01      0.71      0.59      0.02      0.65      0.43       101
         low_risk       1.00      0.59      0.71      0.74      0.65      0.42     17104

      avg / total       0.99      0.59      0.71      0.74      0.65      0.42     17205
  

- SMOTE
 - An accuracy score was calculated for the model:
    0.636
  
  - A confustion matrix was generated:
     ([[   61,    40],
       [ 5671, 11433]])
       
  - An imbalanced classification report was generated:
                      pre       rec       spe        f1       geo       iba       sup

      high_risk       0.01      0.60      0.67      0.02      0.64      0.40       101
       low_risk       1.00      0.67      0.60      0.80      0.64      0.41     17104

    avg / total       0.99      0.67      0.60      0.80      0.64      0.41     17205


- ClusterCentroids
  - An accuracy score was calculated for the model:
      0.636

    - A confustion matrix was generated:
     ([[   68,    33],
       [10392,  6712]])

    - An imbalanced classification report was generated:
                       pre       rec       spe        f1       geo       iba       sup

        high_risk       0.01      0.67      0.39      0.01      0.51      0.27       101
         low_risk       1.00      0.39      0.67      0.56      0.51      0.26     17104

      avg / total       0.99      0.39      0.67      0.56      0.51      0.26     17205



- Combination (over and undersampling) (SMOTEENN)
  - An accuracy score was calculated for the model:
    0.654
  
  - A confustion matrix was generated:
     ([[   72,    29],
       [ 6928, 10176]])
  
  - An imbalanced classification report was generated:
                       pre       rec       spe        f1       geo       iba       sup

      high_risk       0.01      0.71      0.59      0.02      0.65      0.43       101
       low_risk       1.00      0.59      0.71      0.75      0.65      0.42     17104

    avg / total       0.99      0.60      0.71      0.74      0.65      0.42     17205


- BalancedRandomForestClassifier
  - An accuracy score was calculated for the model:
    0.789
  
  - A confustion matrix was generated:
     ([[   71,    30],
       [ 2153, 14951]])
  
  - An imbalanced classification report was generated:
                       pre       rec       spe        f1       geo       iba       sup

      high_risk       0.03      0.70      0.87      0.06      0.78      0.60       101
       low_risk       1.00      0.87      0.70      0.93      0.78      0.62     17104

    avg / total       0.99      0.87      0.70      0.93      0.78      0.62     17205


- EasyEnsembleClassifier
  - An accuracy score was calculated for the model:
    0.932
  
  - A confustion matrix was generated:
     ([[   93,     8],
       [  983, 16121]])
  
  - An imbalanced classification report was generated:
                       pre       rec       spe        f1       geo       iba       sup

      high_risk       0.09      0.92      0.94      0.16      0.93      0.87       101
       low_risk       1.00      0.94      0.92      0.97      0.93      0.87     17104

    avg / total       0.99      0.94      0.92      0.97      0.93      0.87     17205
    

## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

