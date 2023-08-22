# Mini-Project-2-Pre-Interview-Assessment

The aim of this project is to predict, if a candidate with given features will be accepted for the interview.

 To run the code, first download the notebook and the data. Then you can run it locally if you have Jupyter installed, or upload it to google colab, for which you will need google account.

 Modules used.
 'Pandas' is used to load the dataset. 'Matplotlib' is used to visualize the data. 'train_test_split' from sklearn.model_selection is used to split the data into training and test datasets. 'StandartScaler, OrdinalEncoder and LabelEncoder' are used to rescale the numerical values and turn categorical ones into integers. 'LogisticRegression, GaussianNB and Kneighborsclassifier' are used to build and fit the classification models. 'mean_squared_error, classification_report, confusion_matrix and model.score (which is r2 score)' are used to evaluate the models.

 The dataset contains 'Age,	BusinessTravel,	Education,	MaritalStatus,	OverTime,	EmployeeNumber,	DailyRate,	Gender.' features, from which only 'EmployeeNumber' is not used, because it has no meaning. The label is 'accepted for the interview' which has values 'True' and 'False' (1 and 0 respectivly after performing label encoder).

 Data visualization.

 We see that only small fraction of candidates are accepted.![accepted or not](https://github.com/SargisArzumanyan/Mini-Project-2-Pre-Interview-Assessment/assets/82839525/377b3a0c-6696-44ab-991f-30844eb4132a)

We see that most of the candidates are between 25-45 years old.![age distribution](https://github.com/SargisArzumanyan/Mini-Project-2-Pre-Interview-Assessment/assets/82839525/cd12fa51-7b34-48ee-95e5-e86b1cefe5bd)

We see that most of the candidates has education level 2, 3, or 4.![education level](https://github.com/SargisArzumanyan/Mini-Project-2-Pre-Interview-Assessment/assets/82839525/271d9227-c37b-4448-b11f-7b6c9636ad62)

We also see that most of them don't work overtime. ![works overtime](https://github.com/SargisArzumanyan/Mini-Project-2-Pre-Interview-Assessment/assets/82839525/d6cbbb98-6b90-4e25-8e5d-da863c5298d5)

Results.

Overall K-nearest neighbors performed the best, but naive bayes had fewer false negatives. You can see classification reports, ROC curves and confusion matricies for the models below.

For logistic regression.
![изображение](https://github.com/SargisArzumanyan/Mini-Project-2-Pre-Interview-Assessment/assets/82839525/00c8cad6-6c3f-4248-a2dc-a91659667e0a)

![log cm](https://github.com/SargisArzumanyan/Mini-Project-2-Pre-Interview-Assessment/assets/82839525/3e4433bb-01a3-475b-91c6-527279381306)

![log_roc](https://github.com/SargisArzumanyan/Mini-Project-2-Pre-Interview-Assessment/assets/82839525/852a65c2-e5cb-49d5-bbff-7fe4890cbf47)

for naive bayes.
![изображение](https://github.com/SargisArzumanyan/Mini-Project-2-Pre-Interview-Assessment/assets/82839525/fbfe2faf-33dc-49a9-b443-9a8e5c97ee91)

![bayes cm](https://github.com/SargisArzumanyan/Mini-Project-2-Pre-Interview-Assessment/assets/82839525/6211775c-39da-4c39-b563-e079739053c6)

![bayes_roc](https://github.com/SargisArzumanyan/Mini-Project-2-Pre-Interview-Assessment/assets/82839525/c22f760a-3a48-48b8-ba72-3559af7b6af8)

for knn
![изображение](https://github.com/SargisArzumanyan/Mini-Project-2-Pre-Interview-Assessment/assets/82839525/603ef020-c65a-4e83-b309-7c10561a8e2d)

![knn cm](https://github.com/SargisArzumanyan/Mini-Project-2-Pre-Interview-Assessment/assets/82839525/5fee2ad2-7d52-4a28-838b-47943f45b80b)

![knn_roc](https://github.com/SargisArzumanyan/Mini-Project-2-Pre-Interview-Assessment/assets/82839525/230fb2ac-3ab0-44d0-9848-b77148619318)
