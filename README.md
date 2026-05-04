Clinical ML Mortality Prediction

This project analyzes a clinical dataset to predict patient mortality using multiple machine learning models. The goal is to compare models, evaluate robustness, and select the most practical model for real-world use.

Dataset:Synthetic Clinical Dataset
- Contains patient health features such as age, BMI, blood pressure, glucose, etc.
- Target variable: mortality (0/1 classification)
- Dataset source: Kaggle (https://www.kaggle.com/datasets/uom190346a/synthetic-clinical-tabular-dataset)

To Run
open the notebooks in order
Run each notebook step by step
Outputs (tables + figures) will be generated automatically

Models Used:
- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)
- XGBoost

Key Findings
- Logistic Regression performed best based on F1-score
- Random Forest and XGBoost showed high accuracy but failed to predict minority class
- Dataset is highly imbalanced, so accuracy is misleading
- Recall and F1-score are more reliable for this task

Requirements
Install required libraries:
- pip install pandas numpy matplotlib scikit-learn xgboost

Project Structure

- notebooks/ → RQ1 to RQ7 notebooks  
- results/ → CSV tables and PDF plots  
- README.md  
- requirements.txt

Conclusion

Logistic Regression is selected as the final model due to:
- Better balance between precision and recall
- Higher F1-score
- Good interpretability
- Stability under noise and missing data

