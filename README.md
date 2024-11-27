# FinalProject2024
Final Project for CSCI-1070
This project uses a heart failure dataset from Kaggle: [https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction](url)
The dataset contains 918 observations with 12 recorded attributes (variables).
The purpose of this project is to use Machine Learning Techniques to predict instances of heart failure with the variables given. 
Null Hypothesis: The variables are not correlated to heart failure instances in any meaningful way (overall accuracy below 70%)
Alternate Hypothesis: The variables do have a significant relation to heart failure instances and can predict them fairly well (accuracy above 70%)

The variables are Age, Sex, Chest Pain Type, Resting Blood Pressure, Cholesterol, Fasting Blood Pressure, Resting Electrocardiogram results, Maximum Heart Rate, Exercise Induced Agina, and Oldpeak, and the ST Slope.


I cleaned the data by replacing null values w/ median, one hot encoding for categorical columns, and standardizing the data. I didn't have to use data cleaning or deal with multicolinearity (any multicolinearity was artificiallly induced by one hot encoding) True/ False instances were fairly close (about 40/60) so I didnt have to use oversampling techniques.

After I cleaned the data, I used KNN and Logistical Regression ML models first to predict the data. The KNN wasn't successful (69% accuracy) but Logistical Regression performed very well with an overall accuracy of 86%, 90% precision and 84% recall for positive instances and 80% precision and 87% recall for negative instances.

Since this is a medical dataset, recall is the most significant measurement of effectiveness. It was very high (higher than most of my other datasets) so probably this dataset was relatively straightforward in correlations because simple Logistical regression worked really well.

In conclusion, this project succesfully proved the alternate hypothesis with an overall accuracy of 86% (a roaring success if you ask me).
Link to Presentation: [https://docs.google.com/presentation/d/1R50fYovxgLy74BUrGt3fpifndTeImPjInfd-jziOuC0/edit?usp=sharing](url)
