# Project_ensemble_techniques_breast_cancer_detection
![h0Hi18KpgEuy](https://user-images.githubusercontent.com/108978683/202143545-e72e5146-afc0-4d83-b008-40ea15901068.jpg)

Predicting Breast Cancer in a patient 

## Project Summary:

In this project we used three different Ensemble models to our Breast Cancer Diagnosis dataset. Our results are reported with 75:25 training test data split and for 10 fold cross validation.

### Comparing F1 Score:
* our proposed ensemble learning models achieved F1 score accuracies of 94%, 90% and 92% respectively.
* Voting Classifier performs better than XG Boost with an accuracy of 94%

Since our project is medical diagnosis we need to give maximum importance to Type II error in statistics(False Negative).False Negative is that the truth is positive, but the test predicts a negative. The person is sick, but the test inaccurately reports that they are not.To know the performance over False negative rate we will compare our ensemble models with confusion matrix ,ROC and DET curves.

![download (1)](https://user-images.githubusercontent.com/108978683/202146712-096588ff-32ab-4e7f-a17f-6b5db79e0592.png)

### Comparing confusion matrix:
* Voting classifier has less number False Negatives compared to XG Boost and Bagging Classifier

![download (2)](https://user-images.githubusercontent.com/108978683/202146911-ab738360-9ab2-4afc-8884-9c0d3a874006.png)

### Comparing ROC Curve:
* While comparing ROC Curves we found Voting classifier lies at ideal point that is top left corner and has larger area under the curve (AUC) which is 0.99 compared to XG Boost which has 0.98 and Bagging classifier with 0.94

Comparing DET Curve:
* The DET Curve has distinct advantages over the standard ROC type curve for presenting performance results where tradeoffs of two error types are involved. Here we can observe Voting Classifier has lesser error tradeoff compared to XG Boost.

![download](https://user-images.githubusercontent.com/108978683/202146488-92db522b-54d8-45f1-a994-2cc6f2bc8e3f.png)

Experimental results show that Voting Classifier(soft voting) was the most powerful prediction model than other ensemble machine learning techniques for Breast Cancer dataset.
