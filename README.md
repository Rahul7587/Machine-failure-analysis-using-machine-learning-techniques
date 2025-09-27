# Industrial-Machine-failure-analysis-using-machine-learning-techniques
# Machine Failure Prediction 🤖🔧

Predicting electrical and mechanical failures using machine learning classifiers.

## 📂 Project Overview

This project focuses on predicting mechanical and electrical failures of machines using a dataset containing various operational parameters.

### Data Loading & Preparation 📊

- Loaded data from an Excel file.
- Installed necessary libraries (`openpyxl`, `xgboost`).
- Created dictionaries to map machine IDs to names and breakdown codes to types.
- Dropped irrelevant columns based on initial analysis.
- Created a unified 'date' column and dropped redundant date-related columns.
- Filtered the data to include only electrical ('D') and mechanical ('F') breakdowns, along with instances of 'NO BREAKDOWN'.
- Converted relevant columns to numeric types, handling potential errors by coercing to NaN and filling with 0.
- Standardized features using `StandardScaler`.
- Created a `Breakdown_Flag` column (1 for breakdown, 0 for no breakdown).
- Sorted the data by date.

### Exploratory Data Analysis (EDA) 🔍

- Checked the information and descriptive statistics of the dataset.
- Identified unique machines and their corresponding IDs.
- Analyzed missing values.
- Identified columns with unique values for a specific machine.
- Visualized feature correlations using a heatmap.
- Plotted scatter plots of features against `Breakdown_Flag` to explore potential patterns.

### Machine Learning Modeling 🤖

- Split the data into training and testing sets.
- Trained and evaluated several classification models:
    - Logistic Regression
    - Random Forest Classifier
    - XGBoost Classifier
    - Support Vector Machine (SVC)
    - Decision Tree Classifier

- Evaluated models using Accuracy, Precision, Recall, F1 Score, and Confusion Matrix.

## 💻 Tech Stack

- Python 🐍
- pandas, numpy: data manipulation and analysis
- matplotlib, seaborn: data visualization
- scikit-learn: data preprocessing, model selection, and model training (Logistic Regression, RandomForestClassifier, SVC, DecisionTreeClassifier)
- xgboost: Gradient Boosting

## 🖼️ Sample visuals
<img width="1010" height="843" alt="image" src="https://github.com/user-attachments/assets/c9daed54-1ff6-49b4-9a80-9a90e9564379" />
<img width="869" height="683" alt="image" src="https://github.com/user-attachments/assets/daa15628-2804-4c51-8434-c9f2001e4f2c" />
<img width="830" height="683" alt="image" src="https://github.com/user-attachments/assets/24d04323-648b-4b3a-bafa-823f49639f16" />
<img width="869" height="683" alt="image" src="https://github.com/user-attachments/assets/ce5c739e-3e34-44db-91ba-18addd720bfd" />
<img width="1044" height="617" alt="image" src="https://github.com/user-attachments/assets/1a33776b-4f9b-41a2-ab1c-7601cefe6953" />
<img width="1054" height="629" alt="image" src="https://github.com/user-attachments/assets/845245c9-ddbe-46ee-b7a7-c0e79c52d1ba" />


## 🏆 Future Work

- Compare the performance metrics of all trained models to select the best one.
- Fine-tune the hyperparameters of the selected model(s) to potentially improve performance.
- Explore other relevant features or feature engineering techniques.
- Implement other classification algorithms.
- Investigate time-series analysis techniques given the date column to predict future breakdowns.
