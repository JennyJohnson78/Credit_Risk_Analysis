# Credit Risk Analysis

## Overview

Having worked at a financial insitution and writing consolidation loans for individuals who could not pay their loans, financial risk, including credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore different techniques are needed to train and evaluate models with unbalanced classes. In this analysis, credit card data will be oversampled using the RandomOverSampler and SMOTE algorithms, and undersampled using the ClusterCentroids algorithm. Then, a combinatorial approach of over- and undersampling using the SMOTEENN algorithm will be conducted. Next, the machine learning models BalancedRandomForestClassifier and EasyEnsembleClassifier will be used to predict credit risk. Finally, there will be an evaluation the performance of these models and a written recommendation on whether they should be used to predict credit risk.

## Results

- Naive Random Oversampling Results: The balanced accuracy test is 65.72%, the precision score for high risk is very low at 1%. The recall is 62%.

![image](https://user-images.githubusercontent.com/67409852/149710467-013938a8-259b-41b1-954f-2f0631f7a4ae.png)

![image](https://user-images.githubusercontent.com/67409852/149710622-c8e50f96-5978-413f-86e1-69b8d79d9760.png)

- SMOTE Oversampling Results: The balanced accuracy test is 64.78%, the precision score for high risk is very low at 1%. The recall is 68%.

![image](https://user-images.githubusercontent.com/67409852/149710809-fddad8d7-c1c0-47be-9395-bb35f143172f.png)

![image](https://user-images.githubusercontent.com/67409852/149710909-4bd8a29b-6ca3-4c40-8d2d-bfa18678e441.png)

- Undersampling Results: The balanced accuracy test is 54.43%, the precision score is 99%. The recall is 40%.

![image](https://user-images.githubusercontent.com/67409852/149711890-9c6619d8-7f0e-4212-952d-39a7b9f327f8.png)

![image](https://user-images.githubusercontent.com/67409852/149712016-1dc7b332-eb9a-47a5-9aca-84e0194fa1af.png)

- Combination (Undersampling and Oversampling) Results: The balanced accuracy test is 64.47%, the precision score is 99%. The recall is 57%.

![image](https://user-images.githubusercontent.com/67409852/149720027-5dd690be-ffa1-4199-aebb-8462470211b0.png)

![image](https://user-images.githubusercontent.com/67409852/149720144-77b2ee64-2e15-4189-976e-d9c5d37948a6.png)

- Balanced Random Forest Classifier Results: The balanced accuracy test is 77.38%, the precision score is 99%. The recall is 87%.

![image](https://user-images.githubusercontent.com/67409852/149712597-0afb3a70-d571-4d74-bf68-7faed67dc543.png)

![image](https://user-images.githubusercontent.com/67409852/149712689-23526481-fb74-4a99-a614-0d8c926e7704.png)

- Easy Ensemble AdaBoost Classifier Results: The balanced accuracy test is 93.17%, the precision score is 99%. The recall is 94%.

![image](https://user-images.githubusercontent.com/67409852/149712801-5326f9d1-5672-4adf-8d24-9fc37b48da11.png)

![image](https://user-images.githubusercontent.com/67409852/149712920-e1d662aa-f4d6-4dee-b0b8-ae58e892e280.png)

## Summary

The first four models dealt with undersampling, oversampling, and a combination of both under and oversampling. These models were used to analyze credit card data and determine which model is the most effective at predicting the highest risk loans. The ensemble classifier is used to analyze and predict which loans are high risk or low risk. The first four models have accuracy scores that are not as high as the ensemble classifiers. Their recall percentages are low as well. Essemble classifiers have the best balance of precision and recall, which is preferable in a model. Therefore, I recomment the Easy Ensemble Classifier model.
