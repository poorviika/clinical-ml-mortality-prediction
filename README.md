Clinical ML Mortality Prediction Project

Overview
This project analyzes a clinical dataset to predict patient mortality using multiple machine learning models. The goal is to compare models, evaluate robustness, and select the most practical model for real-world use.

Dataset:Synthetic Clinical Dataset
- Contains patient health features such as age, BMI, blood pressure, glucose, etc.
- Target variable: mortality (0/1 classification)
- Dataset source: Kaggle (https://www.kaggle.com/datasets/uom190346a/synthetic-clinical-tabular-dataset)

To Run
Open the notebooks in order:
	rq-01.ipynb
	rq-02.ipynb
	rq-03.ipynb
	rq-04.ipynb
	rq-05.ipynb
	rq-06.ipynb
	rq-07.ipynb

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
	clinical-ml-project/
	│
	├── notebooks/
	│   ├── rq-01.ipynb
	│   ├── rq-02.ipynb
	│   ├── rq-03.ipynb
	│   ├── rq-04.ipynb
	│   ├── rq-05.ipynb
	│   ├── rq-06.ipynb
	│   ├── rq-07.ipynb
	│
	├── results/
	│   ├── rq1_table.csv
	│   ├── rq2_table.csv
	│   ├── rq3_table.csv
	│   ├── rq4_top_features.csv
	│   ├── rq5_ranking.csv
	│   ├── rq6_table.csv	
	│
	│   ├── rq1_bar_chart.pdf
	│   ├── rq2_roc_curve.pdf
	│   ├── rq3_bar_chart.pdf
	│   ├── rq4_feature_importance.pdf
	│   ├── rq5_ranking_plot.pdf
	│   ├── rq7_final_comparison.pdf
	│   
	├── README.md
	├── requirements.txt

Conclusion

Logistic Regression is selected as the final model due to:
- Better balance between precision and recall
- Higher F1-score
- Good interpretability
- Stability under noise and missing data

Author
Poorvika Sreenivasa
