# Credit_Risk_Analysis

## Overview of the analysis

Our work and practices led us to applying machine learning to credit card risk assessments. Using the dataset from LendingClub, we are to test and evaluate 6 different algorithms to predict credit card risks.

## Results
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

- RandomOver

<img width="413" alt="RamdomOver_bas" src="https://user-images.githubusercontent.com/68725398/105642608-ba42b900-5e58-11eb-8366-5711f5e7665f.png">
<img width="612" alt="RandomOver_cri" src="https://user-images.githubusercontent.com/68725398/105642606-ba42b900-5e58-11eb-993b-8a31b13de12d.png">

The Random Over Sampling Model above has an accuracy score of 65%. This model performed badly in terms of predicting high risk as indicated by the low precision score of 1%, however the recall percentage is at 69% for high_risks.

- SMOTE

<img width="369" alt="SMOTE_bas" src="https://user-images.githubusercontent.com/68725398/105642639-e78f6700-5e58-11eb-828b-34036fff23c6.png">
<img width="604" alt="SMOTE_cri" src="https://user-images.githubusercontent.com/68725398/105642640-e827fd80-5e58-11eb-9fe4-5d55cc57a45a.png">

The accuracy score for this model is slightly higher at 66%. However, this model still has a bad precision rate of 1% only. The recall rate also didn't change by much at 63% compared to the previous model. 

- ClusterCentroids

<img width="370" alt="UnderSamp_bas" src="https://user-images.githubusercontent.com/68725398/105642654-fd049100-5e58-11eb-8660-88ac58da1279.png">
<img width="607" alt="UnderSamp_cri" src="https://user-images.githubusercontent.com/68725398/105642655-fd9d2780-5e58-11eb-9c86-d9be57466a29.png">

The accuracy score for this model is much lower than the previous ones at 55% only. With the precision rate still at around 1%, the recall rate was increased to 68% for high risk but was lowered to 41% for low risk.


- Combined SMOTEENN

<img width="377" alt="Combined_bas" src="https://user-images.githubusercontent.com/68725398/105642671-19a0c900-5e59-11eb-8c4f-5e5eae0489fd.png">
<img width="616" alt="Combined_cri" src="https://user-images.githubusercontent.com/68725398/105642672-19a0c900-5e59-11eb-9964-bb3a70e754b5.png">

This model did better than the above with 67% accuracy. Precision wise, there has been no changes to the high risk labels. Recall rate is higher at 78% for high risk and 57% for low risk. 

- Balanced Random Forest Classifier

<img width="341" alt="BRFC_bas" src="https://user-images.githubusercontent.com/68725398/105642685-29201200-5e59-11eb-943b-217e76aec23f.png">
<img width="608" alt="BRFC_cri" src="https://user-images.githubusercontent.com/68725398/105642683-29201200-5e59-11eb-9ea4-f01e20fcf52e.png">


This model has an accuracy score 79% and the first out of the above that had an improved high risk precision of 3%. The recall rate is also high with high risk rate at 70% and the low risk rate at 87%.

- Easy Ensemble Adaboost Classifier

<img width="353" alt="EasyEnsemble_bas" src="https://user-images.githubusercontent.com/68725398/105642695-34733d80-5e59-11eb-83cc-f59c49d501be.png">
<img width="608" alt="EasyEnsemble_cri" src="https://user-images.githubusercontent.com/68725398/105642696-350bd400-5e59-11eb-93a5-169e89c2d40e.png">

Of all the models so far in this challenge, the Easy Ensemble model has had that highest accuracy, precision and recall rate. Accuracy is at 93%, highest much higher than any of the others. Precision is at 9% and recall is at 92% for high and 94% for low.

## Summary

The analysis of the machine learning models above shows that Easy Ensemble Adaboost Classifier is the best overall compared to the other five. In terms of credit card risk predictions though, this model would not be suggested because although precision is high for low risk, the high risk precision is still too low. This would be an issue if high risk applicants isn't rejected correctly as this will probably cost a lot of money leaving the applicants on.
