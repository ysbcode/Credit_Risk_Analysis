# Credit_Risk_Analysis

## Overview

In this project, we use Python and JupyterNotebook to build and evaluate several machine learning models to predict credit risk. We applied the following ML methods: 

 - Oversampling using the RandomOverSampler 
 - Oversampling using the SMOTE algorithm.
 - Undersampling using the ClusterCentroids algorithm.
 - A combination approach of over-undersampling using the SMOTEENN algorithm.
 - The BalancedRandomForestClassifier algorithm. 
 - The EasyEnsembleClassifier algorithm. 

We evaluated the performance of these models and make a recommendation on whether they should be used to predict credit risk.

## Results

### Oversampling with RandomOverSampler

![](https://github.com/ysbcode/Credit_Risk_Analysis/blob/main/Screenshots/1_RandomOverSampling1.PNG?raw=true)
![](https://github.com/ysbcode/Credit_Risk_Analysis/blob/main/Screenshots/1_RandomOverSampling2.PNG?raw=true)

### Oversampling with SMOTE

![](https://github.com/ysbcode/Credit_Risk_Analysis/blob/main/Screenshots/2_SMOTEOverSampling1.PNG?raw=true)
![](https://github.com/ysbcode/Credit_Risk_Analysis/blob/main/Screenshots/2_SMOTEOverSampling2.PNG?raw=true)

### Undersampling with ClusterCentroids

![](https://github.com/ysbcode/Credit_Risk_Analysis/blob/main/Screenshots/3_UnderSampling1.PNG?raw=true)
![](https://github.com/ysbcode/Credit_Risk_Analysis/blob/main/Screenshots/3_UnderSampling2.PNG?raw=true)

### SMOTEENN

![](https://github.com/ysbcode/Credit_Risk_Analysis/blob/main/Screenshots/4_SMOTEENNSampling1.PNG?raw=true)
![](https://github.com/ysbcode/Credit_Risk_Analysis/blob/main/Screenshots/4_SMOTEENNSampling2.PNG?raw=true)

### BalancedRandomForestClassifier

![](https://github.com/ysbcode/Credit_Risk_Analysis/blob/main/Screenshots/5_BalancedRandomForrest1.PNG?raw=true)
![](https://github.com/ysbcode/Credit_Risk_Analysis/blob/main/Screenshots/5_BalancedRandomForrest2.PNG?raw=true)

### EasyEnsembleClassifier

![](https://github.com/ysbcode/Credit_Risk_Analysis/blob/main/Screenshots/6_EasyEnsembleAdaBoost1.PNG?raw=true)

![](https://github.com/ysbcode/Credit_Risk_Analysis/blob/main/Screenshots/6_EasyEnsembleAdaBoost2.PNG?raw=true)

Overall, we can see that the accuracy score for all oversampling and undersampling methods were poor with scores ranging from the low 50 percents to the high 60 percents. Using the ensemble clasifiers improved the accuracy score from approx 90 to the mid 90 percents. However, the precision of the both ensamble models remained poor leading on overall low F1 score for both.

## Summary

The ensamble methods are much better at predicting high risk loans with accuracy in the high 80s to mid 90s. However with a low precision for both models, we can see that there are a significantly high number of false positives. This means a significant number of customers are being turned down because they are being tagged as high risk even when they are not which means ultimately the bank is missing out on good customers and make a profit. Out of the 6 methods the Easy Ensemble had the best balance of all methods because of it's high accuracy score and good balance of precision and recall scores. Overall my recommendation would be to not use any of the 6 models.

