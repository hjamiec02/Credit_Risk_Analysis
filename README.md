# Credit_Risk_Analysis

## Overview of the analysis:
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Finally, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results:

- RandomOverSampler 
  - An accuracy score was calculated for the model:
    0.653
  
  - A confustion matrix was generated and imbalanced classification report was generated: 
              
     <img width="736" alt="Screen Shot 2022-09-05 at 7 33 12 AM" src="https://user-images.githubusercontent.com/105119531/188440308-da36c58e-75c8-4711-96b7-acd08e4a3211.png">

  

- SMOTE
  - An accuracy score was calculated for the model:
    0.636
  
   - A confustion matrix was generated and imbalanced classification report was generated:

    <img width="726" alt="Screen Shot 2022-09-05 at 7 33 51 AM" src="https://user-images.githubusercontent.com/105119531/188440614-623af902-4297-4c92-bbab-3b7efe7f3c40.png">



- ClusterCentroids
    - An accuracy score was calculated for the model:
      0.636

    - A confustion matrix was generated and imbalanced classification report was generated:
    
      <img width="718" alt="Screen Shot 2022-09-05 at 7 34 33 AM" src="https://user-images.githubusercontent.com/105119531/188440907-457529af-d61d-46b4-a3bb-97992bbf7e56.png">



- Combination (over and undersampling) (SMOTEENN)
  - An accuracy score was calculated for the model:
    0.654
  
  - A confustion matrix was generated and imbalanced classification report was generated:
  
    <img width="733" alt="Screen Shot 2022-09-05 at 7 35 08 AM" src="https://user-images.githubusercontent.com/105119531/188441189-eb5c9553-cc4f-4d65-8257-752b044fecea.png">


- BalancedRandomForestClassifier
  - An accuracy score was calculated for the model:
    0.789
  
  - A confustion matrix was generated and imbalanced classification report was generated:
  
    <img width="714" alt="Screen Shot 2022-09-05 at 7 35 47 AM" src="https://user-images.githubusercontent.com/105119531/188441346-9395bee7-d420-4bbd-9d90-089a4f9468b7.png">



- EasyEnsembleClassifier
  - An accuracy score was calculated for the model:
    0.932
  
  - A confustion matrix was generated and imbalanced classification report was generated:
  
    <img width="720" alt="Screen Shot 2022-09-05 at 7 36 20 AM" src="https://user-images.githubusercontent.com/105119531/188441564-fc31f233-8d3a-484d-9394-5363f085ceae.png">

    

## Summary: 
In conclusion, the resampling models did not produce an adequate f1 score to be a useful model for assessing risk.  The model that performed the best was the EasyEnsambleClassifier model, producing and f1 score of 0.16. If I were going to use one of the model to predict high risk loans, the EasyEnsambleClassifier would be by far the best but improvements could still be made and it is not ideal for assessing risk. 
