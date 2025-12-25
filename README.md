# Heart-disease-prediction
Used the UCI Machine Learning Heart Disease dataset.

- Test set metrics
- Accuracy : 0.8689
- Precision : 0.8846
- Recall : 0.8214 (Sensitivity)
- Specificity : 0.9091
- F1 Score : 0.8519
- ROC AUC : 0.9307

# Features
The Cleaveland Database was used from the dataset consisting of 303 records and these features were used for training:

1. **age**  
   - Age of the patient in years

2. **sex**  
   - 1 = Male  
   - 0 = Female  

3. **cp** (Chest Pain Type)  
   ○ 1 = Typical angina  
   ○ 2 = Atypical angina  
   ○ 3 = Non-anginal pain  
   ○ 4 = Asymptomatic  

4. **trestbps**  
   - Resting blood pressure (in mm Hg on admission to the hospital)

5. **chol**  
   - Serum cholesterol in mg/dl

6. **fbs**  
   - Fasting blood sugar > 120 mg/dl  
   - 1 = True  
   - 0 = False  

7. **restecg** (Resting Electrocardiographic Results)  
   ○ 0 = Normal  
   ○ 1 = ST-T wave abnormality  
     (T wave inversions and/or ST elevation or depression > 0.05 mV)  
   ○ 2 = Probable or definite left ventricular hypertrophy  
     (by Estes' criteria)

8. **thalach**  
   - Maximum heart rate achieved

9. **exang**  
   - Exercise-induced angina  
   - 1 = Yes  
   - 0 = No  

10. **oldpeak**  
    - ST depression induced by exercise relative to rest

11. **slope** (Slope of the peak exercise ST segment)  
    ○ 1 = Upsloping  
    ○ 2 = Flat  
    ○ 3 = Downsloping  

12. **ca**  
    - Number of major vessels (0–3) colored by fluoroscopy

13. **thal**  
    ○ 3 = Normal  
    ○ 6 = Fixed defect  
    ○ 7 = Reversible defect  

14. **num** (Diagnosis of Heart Disease)  
    ○ 0 = < 50% diameter narrowing  
    ○ 1 = > 50% diameter narrowing  

# Things done

1. Imputation of missing values using KNN
2. Creation of new domain-aware features
3. Creation of new categorical bins
4. EDA with Correlation heatmap, pairplot and crosstab
5. One-hot / Label encoding of features as per requirement
6. PCA projection of feature space
7. Hyperparameter tuning of the models with hyperopt and Stratified K Fold CV.
8. Comparison of tuned models with approximately good parameters
9. Create a pipeline for Ensemble learning with LogisticRegression as meta learner
10. Calibration of the model with CalibratedClassifierCV
