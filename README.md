# Analyzing Credit Risk

# Overview

## Purpose

The user will practice widely-known, beginner level supervised machine-learning method to assess individual customer credit risk. Since good loans typically outnumber risky loans, credit risk is an inherently unbalanced classification problem. Because of this, we will use different techniques to train and evaluate models with unbalanced classes. We will use **imbalanced-learn** and **scikit-learn** libraries to build and evaluate models using resampling. We will use a credit card dataset from LendingClub, a peer-to-peer lending services company. 


## Results


Below are the models' respective accuracy scores and classification reports.

- RandomOverSampler

<img width="467" alt="Naive Random Over Samp Accuracy Score" src="https://user-images.githubusercontent.com/106895220/193920434-2ae0d317-aba4-4065-80a9-7cf257fbde23.png">
<img width="705" alt="Naive Random Over Sample Class" src="https://user-images.githubusercontent.com/106895220/193920437-d16080dc-c412-4119-8bbd-5de24ec4a41e.png">




- SMOTE

<img width="380" alt="SMOTE Acc" src="https://user-images.githubusercontent.com/106895220/193920487-c75d5b95-a239-4dc8-a207-343436410ccc.png">
<img width="705" alt="SMOTE Class" src="https://user-images.githubusercontent.com/106895220/193920492-9b8b32f7-ec35-4f54-abe5-426c758cc804.png">



- ClusterCentroids

<img width="380" alt="Cluster Centroids Acc" src="https://user-images.githubusercontent.com/106895220/193920547-44086349-b61f-4557-8595-0d9e13477f8d.png">
<img width="705" alt="Cluster Centroids Class" src="https://user-images.githubusercontent.com/106895220/193920550-8715a84f-6780-48db-a4f6-6ab7d2b91049.png">



- SMOTEENN

<img width="383" alt="SMOTEEN Acc" src="https://user-images.githubusercontent.com/106895220/193920569-9e538c6f-b673-4a58-be90-8d19c1dc9294.png">
<img width="704" alt="SMOTEEN Class" src="https://user-images.githubusercontent.com/106895220/193920571-307056b3-85b9-4f90-84dd-643f1c0fd9b7.png">




- BalancedRandomForestClassifier


<img width="476" alt="Bal Rand Acc" src="https://user-images.githubusercontent.com/106895220/193920592-d5aa3245-745f-47a3-8748-207294761837.png">
<img width="700" alt="Bal Rand Class" src="https://user-images.githubusercontent.com/106895220/193920595-fe3d47b0-d6bf-4214-8955-61459a2f8c79.png">



- EasyEnsembleClassifier


<img width="378" alt="AdaBoost Acc" src="https://user-images.githubusercontent.com/106895220/193920612-652b0d6a-0297-4a7b-944d-9202016c1838.png">
<img width="706" alt="Ada Boost Class" src="https://user-images.githubusercontent.com/106895220/193920614-7576693e-8723-4564-b14f-85f7e3a5db4b.png">


## Summary

While employing the models from granted us an increasingly accurate score, all the models show weak precision in determining credit risk. The ensemble models, overall, give a vast improvement compared to the others. However, despute its recall score of 92% (detecting almost all high-risk credit), it contains low precision. This could falsely detect low risk credits as high risk. Morevoer, the high accuracy could be attributed to dataset;s unbalanced characteristics. While there is potential for these algorithms, creditors would be at too great a risk if they were to use these specific ones in their current state 
