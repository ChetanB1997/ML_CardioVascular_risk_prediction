# ML_CardioVascular_risk_prediction
## 1. Introduction:
* Cardiovascular diseases (CVDs) are the major cause of mortality worldwide. According to WHO, 17.9 million people died from CVDs in 2019,     accounting for 32% of all global fatalities.
* Though CVDs cannot be treated, predicting the risk of the disease and taking the necessary precautions and medications can help to avoid     severe symptoms and, in some cases, even death.
* As a result, it is critical that we accurately predict the risk of heart disease in order to avert as many fatalities as possible.
* The goal of this project is to develop a classification model that can predict if a patient is at risk of coronary heart disease (CHD)       over the period of 10 years, based on demographic, lifestyle, and medical history.

## 2. EDA Summary:
* The dependent variable is unbalanced, with only ~15% of the patients who tested positive for CHD.
* All the continuous variables are positively skewed except age (which is almost normally distributed)
* Majority of the patients belong to the education level 1, followed by 2, 3, and 4 respectively.
* There are more female patients compared to male patients.
* Almost half the patients are smokers.
* 100 patients under the study are undertaking blood pressure medication.
* 22 patients under the study have experienced a stroke.
* 1069 patients have hypertension.
* 87 patients have diabetes.
* The risk of CHD is higher for older patients than younger patients.
* 18%, 11%, 12%, 14% of the patients belonging to the education level 1, 2, 3, 4 respectively were eventually diagnosed with CHD.
* Male patients have significantly higher risk of CHD (18%) than female patients (12%)
* Patients who smoke have significantly higher risk of CHD (16%) than patients who don't smoke (13%)
* Patients who take BP medicines have significantly higher risk of CHD (33%) than other patients (14%)
* Patients who had experienced a stroke in their life have significantly higher risk of CHD (45%) than other patients (14%)
* Hypertensive patients have significantly higher risk of CHD (23%) than other patients (11%)
* Diabetic patients have significantly higher risk of CHD (37%) than other patients (14%)
* Above is the correlation heatmap for all the continuous variables in the dataset.
* The variables ‘systolic BP’ and ‘diastolic BP’ are highly correlated.
* To handle high correlation between two independent variables, we can introduce a new variable ‘pulse_pressure’

## 3. Models:
1) Linear regression
2) K nearest neighbours
3) Naive Bayas
4) Decision trees
5) Random forest
   
## 4. Conclusion:
* We used 5 machine learning models to perform this prediction also did hyperparameter tuning on some.
* We implemented normalizing techniques, scaling, sampling to remove outliers and reduce bias.
* Recall was chosen as the model evaluation metric because it was very important that we reduce the false negatives.
* It is critical that the model we develop has a high recall score. It is OK if the model incorrectly identifies a healthy patient as a     high risk patient because it will not result in death, but if a high risk patient is incorrectly labelled as healthy, it may result in    fatality.
* We were able to create a model with a recall of just 0.75 because of limitated data available and limited computational power availabe.
* From our analysis, it is also found that the age of a person was the most important feature in determining the risk of a patient          getting infected with CHD
* Future developments must include a strategy to improve the model recall score
