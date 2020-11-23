# ML_heart_disease

# Predicting heart disease using machine learning

### 1. Problem definition

Given clinical parameters about a patient and predict whether or not they have heart disease.

### 2. Data

Data from Kaggle.
Get more information of each features [here](https://www.kaggle.com/ronitf/heart-disease-uci).

### 3. EDA

###### 1. Target
![target](https://github.com/bay1020/ML_heart_disease/blob/main/images/target.png)

###### 2. Heart disease frequency for sex
![heart_Disease_Frequency_for_Sex](https://github.com/bay1020/ML_heart_disease/blob/main/images/heart_Disease_Frequency_for_Sex.png)

###### 3. Heart disease in function of age and max heart rate 
![heart_Disease_in_function_of_Age_and_Max_Heart_Rate](https://github.com/bay1020/ML_heart_disease/blob/main/images/heart_Disease_in_function_of_Age_and_Max_Heart_Rate.png)

###### 4. Heart disease frequency per chest pain type
![heart_Disease_Frequency_Per_Chest_Pain_Type](https://github.com/bay1020/ML_heart_disease/blob/main/images/heart_Disease_Frequency_Per_Chest_Pain_Type.png)

###### 5. Correlation matrix
![corr_matrix](https://github.com/bay1020/ML_heart_disease/blob/main/images/corr_matrix.png)

### 4. Modeling
 
###### 1. Fit and score models
|        Model          |      Score       |
|-----------------------|:----------------:|
| Logistic Regression   |0.8852459016393442|
| KNN                   |0.6885245901639344|
| RandomForestClassifier|0.8360655737704918|

###### 2. Hyperparameter tuning 

|        Model          |      Method      |      Score       |
|-----------------------|------------------|:----------------:|
| KNN                   |by hand           |0.7540983606557377|
| Logistic Regression   |RandomizedSearchCV|0.8852459016393442|
| RandomForestClassifier|RandomizedSearchCV|0.8688524590163934|
| Logistic Regression   |GridSearchCV      |0.8852459016393442|

### 5. Evaluate
###### 1. Plot ROC curve & calculate AUC
![roc_curve](https://github.com/bay1020/ML_heart_disease/blob/main/images/roc_curve.png)

###### 2. Confusion matrix
![confusion_matrix](https://github.com/bay1020/ML_heart_disease/blob/main/images/confusion_matrix.png)

###### 3. Classification report
![classification_report](https://github.com/bay1020/ML_heart_disease/blob/main/images/classification_report.png)

###### 4. Calculate evaluation metrics using cross-validation
|Evaluation metrics|      Score       |
|------------------|:----------------:|
|F1-score          |0.8705403543192143|
|Recall            |0.9272727272727274|
|Precision         |0.8215873015873015|
|Accuracy          |0.8479781420765027|

![cv_metrics](https://github.com/bay1020/ML_heart_disease/blob/main/images/cv_metrics.png)

### 6. Feature Importance
![feature_importance](https://github.com/bay1020/ML_heart_disease/blob/main/images/feature_importance.png)
