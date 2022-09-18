# Credit_Risk_Analysis
## Overview
In this analysis I will be assiting Fast Lending in using machine learning(ML) to predit credit risk. ML will help to make this a quicker process with reliable results.
We will be utilizing oversampling, undersampling, and balanced/imbalanced classifiers.

## How it went
### Naive Random Over Sampling

![NRO](https://user-images.githubusercontent.com/19378130/190882900-575cc99d-9619-4da6-b4a3-64a22a5de0d8.PNG)

![NRO imbal class report](https://user-images.githubusercontent.com/19378130/190882902-e62db363-6adf-420a-8e3e-a3be2ef2430d.PNG)

- Balanced Accuracy Score = 63%
- High Risk:
  - Precision = 1%
  - Recall = 57%
- Low Risk:
  - Precision = 100%
  - Recall = 68%
  
### SMOTE Oversampling

![SMOTE O](https://user-images.githubusercontent.com/19378130/190883081-f9527aec-29b9-4919-ad6b-1210dd8d69ff.PNG)

![SMOTE imbal class report](https://user-images.githubusercontent.com/19378130/190883084-6fd7f799-fd55-49b8-8c8f-a796bdaa6adc.PNG)

- Balanced Accuracy Score = 62.8%
- High Risk:
  - Precision = 1%
  - Recall = 62%
- Low Risk:
  - Precision = 100%
  - Recall = 63%

### Cluster Centroids Undersampling

![CC U](https://user-images.githubusercontent.com/19378130/190883108-ba511de7-4a83-48a7-8c52-0b9db4e4582c.PNG)

![CC Imbal class report](https://user-images.githubusercontent.com/19378130/190883110-eaa58df7-2f24-48b0-872f-a23d95fd20ab.PNG)

- Balanced Accuracy Score = 51.1%
- High Risk: 
  - Precision = 1%
  - Recall = 59%
- Low Risk:
  - Precision = 100%
  - Recall = 44%
  
### SMOTEENN Combination Sampling
  
![SMOTEEN Comb](https://user-images.githubusercontent.com/19378130/190883136-f71e0022-41d5-422c-bd48-1835939d8977.PNG)

![SMOTEEN imbal class report](https://user-images.githubusercontent.com/19378130/190883139-eb56cc44-44be-4f9b-92de-5836434ee582.PNG)

- Balanced Accuracy Score = 65.5%
- High Risk:
  - Precision = 1%
  - Recall = 70%
- Low Risk:
  - Precision = 100%
  - Recall = 61%
  
### Balanced Random Forest Classifier

![Bal Rand Forest Class](https://user-images.githubusercontent.com/19378130/190883164-2aab5c5e-3bac-439d-93a5-42a8d9ef983b.PNG)

![Bal Rand Forest Class imbal class report](https://user-images.githubusercontent.com/19378130/190883169-ec6aa2b9-5e67-4463-ac30-e6b8a809d5b9.PNG)

- Balanced Accuracy Score = 78.8%
- High Risk:
  - Precision = 4%
  - Recall = 67%
- Low Risk:
  - Precision = 100%
  - Recall = 91%
  
### Easy Ensemble Classifier

![Easy Ens Class](https://user-images.githubusercontent.com/19378130/190883188-4e93f6e2-b898-463a-a37e-0abc46a703ec.PNG)

![Easy ens imbal class report](https://user-images.githubusercontent.com/19378130/190883190-fe5a36e7-2e58-4399-b16a-d53a1b861944.PNG)

- Balanced Accuracy Score = 92.5%
- High Risk:
  - Precision = 7%
  - Recall = 91%
- Low Risk:
  - Precision = 100%
  - Recall = 94%
  

## What does it mean?
According to our accuracy scores, the Easy Ensemble Classifier was the best model when it came to reliability.
Althought the F1 scores for the high risk was relatively low at 14%, it was still the best high rish F1 score out of all the models.
The worst model, by far was the Cluster Centroids Undersampling model. Its low risk F1 score was 61%, the lowest of all the low risk models. It also had the worst accuracy score at 51.1%

With all this information in mind, I would reccoment the Easy Ensemble Classifier. While it may not be perfect, it did perform the best out of these six.
