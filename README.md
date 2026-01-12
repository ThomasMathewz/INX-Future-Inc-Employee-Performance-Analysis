# INX Future Inc – Employee Performance Analysis
---
## Project Overview

This project presents an end-to-end data science and machine learning solution to analyze and predict employee performance for INX Future Inc, a global analytics and automation solutions provider. The primary objective is to identify key factors influencing employee performance, analyze department-wise trends, and build a robust predictive model to support data-driven HR decision-making.

The project follows a modular, reproducible, and industry-standard structure, separating data processing, exploratory analysis, modeling, visualization, and business reporting.

---
## Objectives

- Analyze employee performance trends across departments and job roles
- Identify the most important factors affecting employee performance
- Build and evaluate multiple machine learning models
- Select the best-performing model for prediction
- Provide actionable recommendations to improve organizational performance

---
## Machine Learning Models Used

The following classification models were trained and evaluated:
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Gradient Boosting Classifier

Models were compared using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

Among all evaluated models, Random Forest demonstrated the most balanced and consistent performance and was selected as the final model.

---
## Project Structure (Industry Standard)

The project follows a standard data science directory structure commonly used in production and enterprise environments.

INX_Employee_Performance_Analysis/ <br>
│ <br>
├── Project Summary/ <br>
│   ├── Requirement/ <br>
│   │   └── business_problem.md <br>
│   │ <br>
│   ├── Analysis/ <br>
│   │   └── analysis_summary.md <br>
│   │ <br>
│   └── Summary/ <br>
│       └── final_recommendations.md <br>
│ <br>
├── data/ <br>
│   ├── raw/ <br>
│   │   └── INX_Future_Inc_Employee_Performance_CDS_Project2_Data_V1.8.xls <br>
│   │ <br>
│   ├── processed/ <br>
│   │   ├── X.csv <br>
│   │   ├── y.csv <br>
│   │   ├── X_train.csv <br>
│   │   ├── X_test.csv <br>
│   │   ├── y_train.csv <br>
│   │   ├── y_test.csv <br>
│   │   └── feature_names.txt <br>
│   │ <br>
│   └── external/ <br>
│ <br>
├── src/ <br>
│   ├── Data Processing/ <br>
│   │   ├── data_processing.ipynb <br>
│   │   └── data_exploratory_analysis.ipynb <br>
│   │ <br>
│   ├── models/ <br>
│   │   ├── train_model.ipynb <br>
│   │   └── predict_model.ipynb <br>
│   │ <br>
│   └── visualization/ <br>
│       └── visualize.ipynb <br>
│ <br>
├── models/ <br>
│   ├── scaler.pkl <br>
│   └── random_forest_model.pkl <br>
│ <br>
├── prediction.py <br>
│ <br>
└── README.md <br>

----
## Explanation of Folder Design
`data/`
- raw/: Original dataset (never modified)
- processed/: Cleaned, encoded, and split datasets saved for reproducibility

`src/`
- Data Processing/: Data cleaning, encoding, feature preparation, and EDA
- models/: Model training, evaluation, and prediction logic
- visualization/: Final plots and visual summaries for reporting

`models/`
- Stores the trained machine learning model and scaler using serialization
- Enables consistent and reproducible predictions

`Project Summary/`
- Contains all business-facing documentation
- Includes problem definition, analysis insights, conclusions, and recommendations
- Clearly separates code from narrative, following professional standards

---
## Prediction File (Single-File Deployment)

The file prediction.py (located at the project root) contains the entire prediction pipeline in one consolidated script, including:
- Loading the saved scaler and trained model
- Loading feature names
- Preprocessing new input data
- Generating employee performance predictions

This file is designed for:
- Easy deployment
- Quick testing
- Integration with APIs (Flask/Django)
- Demonstrating a production-ready workflow

> While the project internally follows a modular structure, `prediction.py` provides a single-file implementation of the complete prediction logic for real-world usage.

--
## Tools & Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---
## Key Outcomes
- Identified key drivers of employee performance such as environment satisfaction, salary hikes, and promotion frequency
- Built and evaluated multiple machine learning models
- Selected Random Forest as the final predictive model
- Delivered actionable, data-driven HR recommendations
- Designed a reusable and production-aligned project structure

---
## Conclusion

This project demonstrates a complete machine learning lifecycle—from data ingestion to deployment-ready prediction—using industry-standard practices. It provides both technical rigor and business relevance, making it suitable for academic evaluation, professional portfolios, and real-world HR analytics applications.
