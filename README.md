# Heart Failure Prediction Models

This project focuses on predicting heart failure in patients using various classification models. We process patient data, convert features into numerical representations, and build machine learning models to classify the risk of heart disease.

## Dataset Features
* Age: Patient's age (years)
* Sex: Patient's sex (M/F)
* Chest Pain Type: TA (Typical Angina), ATA (Atypical Angina), NAP (Non-Anginal Pain), ASY (Asymptomatic)
* Resting BP: Resting blood pressure
* Cholesterol: Serum cholesterol
* Fasting BS: Fasting blood sugar
* Resting ECG: Resting electrocardiogram results
* Max HR: Maximum heart rate achieved
* Exercise Angina: Exercise-induced angina
* Old peak: ST depression induced by exercise
* ST_Slope: Slope of the peak exercise ST segment
* Heart Disease: Target variable (1: heart disease, 0: normal)

## Models Implemented
* Custom Random Forest
* K-Nearest Neighbors (KNN)
* AdaBoost

The dataset is divided into training, validation, and test subsets. Proper preprocessing, including missing value imputation and one-hot encoding of categorical variables, is performed before model training. Hyperparameters are tuned, and the final models are evaluated using accuracy, F1 score, and ROC-AUC metrics.

## Results
Based on our hyperparameter tuning and evaluation on the validation split:

| Model | Accuracy | F1 Score | AUC |
| :--- | :--- | :--- | :--- |
| **Custom Random Forest** | 0.878 | 0.835 | 0.889 |
| **KNN (K-Nearest Neighbors)** | 0.864 | 0.881 | 0.911 |
| **AdaBoost** | 0.857 | 0.880 | 0.896 |

**Best Model:**
The **Custom Random Forest** model achieved the highest validation accuracy (87.75%). When evaluating this finalized model on the unseen distinct test set, it secured an **accuracy of 87.07%** and an **F1 Score of 0.885**. It proved to be highly robust to outliers and well-equipped to generalize predicting heart disease risk without overfitting.
