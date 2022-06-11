# INTRODUCTION: A MUST READ
Cardiovascular diseases (CVDs) are a group of disorders of the heart and blood vessels.According to a report by WHO updated in June, 2021:

Cardiovascular diseases (CVDs) are the leading cause of death globally.

An estimated 17.9 million people died from CVDs in 2019, representing 32% of all global deaths. Of these deaths, 85% were due to heart attack and stroke.

Over three quarters of CVD deaths take place in low- and middle-income countries.

Although there are various kinds of cardiovascular disease like coronary heart disease(CHD), cerebrovascular disease, peripheral arterial disease, rheumatic heart disease, congenital heart disease, deep vein thrombosis and pulmonary embolism. But our main focus for this analysis will be CHD only.

Coronary heart disease is the term that describes what happens when your heart's blood supply is blocked or interrupted by a build-up of fatty substances in the 
coronary arteries.

Over time, the walls of your arteries can become furred up with fatty deposits. This process is known as atherosclerosis and the fatty deposits are called atheroma.

Atherosclerosis can be caused by lifestyle factors, such as smoking and regularly drinking excessive amounts of alcohol, unhealthy diet and physical inactivity.

You're also more at risk of getting atherosclerosis if you have conditions like high cholesterol, high blood pressure (hypertension) or diabetes.

Coronary heart disease cannot be cured but treatment can help manage the symptoms and reduce the chances of problems such as heart attacks.

### Treatment can include :

lifestyle changes, such as regular exercise and stopping smoking, medicines, angioplasty – where balloons and stents are used to treat narrow heart arteries surgery.

# Problem Description

The dataset is from an ongoing cardiovascular study on residents of the town of Framingham,Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides the patients’ information. It includes over 4,000 records and 15 attributes.

## So, where does machine learning fit it ?

Due to the multi-contributory risk factors such as high blood pressure, high cholesterol, diabetes and various others it gets very constrained to identify the risk factors for some of the patients. That's why we are turning to data mining and machine learning for predicting the disease to avert the risks.

Machine learning (ML), due to its distinction in pattern detection and classification, proves to be effective in assisting decision making and risk assessment from the large quantity of data produced by the healthcare industry on heart disease.


#


Initially started with the exploratory data analysis of dependent and independent  variables. Then searched for correlation between the variables to scrutinize. In dataset class imbalance was quite evident so used SMOTE technique to balance that  and also standardized the variables before feeding to models. 

On target variable, being a binary class, applied various supervised classification  algorithms like logistic regression, k nearest neighbour, decision tree, random forest,  xgboost, naïve bayes and support vector machine. 

Used metrics like confusion matrix, accuracy, F1 score and AUC ROC curve to evaluate  and compare result of models. 

Some very important findings from the EDA were - age, systolic blood pressure, total  cholesterol and heart rate were important features in the case of random forest. 

Males were more at risk of CHD even though the females outnumbered the males in our  dataset. 

There were some cases where people smoked 70 cigarettes a day and still were not at  risk of CHD.  

In general, there was no proper demarcation in between the readings whether the person  had the risk of CHD or not given the variables present in our dataset. Though there were quite a lot of readings that seemed  anomalous in comparison to other readings for the same variable. 

For running models we did hyperparameter tuning with the aid of grid search CV to get  the optimal parameters. 

Naïve bayes classifier was not able to perform well on our dataset. 

Support vector machine and random forest gave similar results and were better than the  rest. Accuracy for both models was around 90% and F1 score revolved around 90% too. 

If there were have been more data points better models could have been built but there’s  always scope for improvement.



