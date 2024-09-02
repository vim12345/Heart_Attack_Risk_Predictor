# Project Name: Heart Attack Risk Predictor

# Objective:
Develop an application that predicts the risk of a heart attack in a patient using various machine learning algorithms. The project involves comparing different models to determine which provides the best accuracy and then employing AutoML library EvalML for further prediction enhancements.

# Project Steps:

# Data Analysis: 
Initial exploration and understanding of the dataset, including data types, distributions, and relationships.
# Feature Engineering: 
Enhancing the dataset by creating new features or modifying existing ones to improve model performance.
# Standardization:
Normalizing the dataset to ensure that features contribute equally to the model.
# Model Building: 
Training multiple machine learning models to predict the risk of a heart attack.
# Predictions: 
Evaluating the models to see which performs best on the given dataset.
#Dataset Features:

Age: Age of the patient.
Sex: Sex of the patient.
exang: Exercise-induced angina (1 = yes; 0 = no).
ca: Number of major vessels (0-3).
cp: Chest pain type:
0: Typical angina
1: Atypical angina
2: Non-anginal pain
3: Asymptomatic
trtbps: Resting blood pressure (in mm Hg).
chol: Cholesterol in mg/dl fetched via BMI sensor.
fbs: Fasting blood sugar > 120 mg/dl (1 = true; 0 = false).
rest_ecg: Resting electrocardiographic results:
0: Normal
1: ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)
2: Probable or definite left ventricular hypertrophy by Estes' criteria
thalach: Maximum heart rate achieved.
target: 0 = less chance of heart attack, 1 = more chance of heart attack.
# Modeling Approach:

# Random Forest (RF):
Initial model achieved an accuracy of ~80%.
# K-Nearest Neighbors (KNN):
A function was implemented to select the optimal value of k for maximum accuracy.
# Support Vector Machine (SVM): 
Achieved an accuracy of 80%.
# Adaboost Classifier: 
Implemented as a boosting technique using multiple models for better accuracy. Initial performance was 50% accuracy, leading to hyperparameter tuning using Grid Search CV.
# Grid Search CV:
Applied to the top 3 performing algorithms for hyperparameter tuning, resulting in an accuracy of 81%.
# Final Model: 
Logistic Regression emerged as the best model without hyperparameter tuning, achieving an accuracy of 85.7%.
# Serialization:

The final model was serialized using Python's pickle library for future deployment.
# AutoML with EvalML:

EvalML, an open-source AutoML library, was employed to automate and evaluate different machine learning pipelines for optimal performance on the dataset.
Outcome: Successfully developed a predictive model with 85.7% accuracy in identifying individuals at risk of a heart attack.

