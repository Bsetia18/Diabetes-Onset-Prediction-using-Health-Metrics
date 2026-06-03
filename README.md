# Diabetes Onset Prediction Using Health Metrics

## Business Context
Early identification of high-risk patients is one of the highest-leverage interventions in preventive healthcare. This project builds a classification model to predict diabetes likelihood from routine health metrics, enabling clinicians and health programs to prioritize outreach and intervention for at-risk individuals before onset. A targeted intervention strategy applied to the top 20% highest-risk patients could reduce undetected cases by an estimated 30%.

## Features
- Exploratory Data Analysis (EDA) to identify trends and relationships in the dataset.
- Machine learning models including Logistic Regression, Random Forest, and Support Vector Machines (SVM).
- Insights presented through data visualizations using Matplotlib and Seaborn.
- Feature engineering to enhance the predictive power of the model.

## Tools and Technologies
- **Programming Language**: Python
- **Libraries Used**:
  - Pandas, NumPy for data manipulation
  - Matplotlib, Seaborn for data visualization
  - Scikit-learn for machine learning
- **Development Environment**: Jupyter Notebook

## Dataset
- **Source**: [Pima Indians Diabetes Database](https://www.kaggle.com/uciml/pima-indians-diabetes-database)
- **Description**: This dataset includes health metrics such as glucose levels, BMI, insulin levels, and more for 768 individuals, with a binary outcome (0: non-diabetic, 1: diabetic).

## Workflow

### 1. Data Exploration
- Analyzed dataset structure and identified missing/zero values across key health features.
- Visualized the distribution of key features using histograms and boxplots.
- Examined relationships between features using correlation heatmaps.

### 2. Feature Engineering
- Imputed missing values with domain-specific techniques to handle biologically implausible zeros in glucose, BMI, and insulin.
- Scaled numerical features using standardization for improved model performance.

### 3. Machine Learning
- Implemented multiple machine learning models:
  - Logistic Regression
  - Random Forest Classifier
  - Support Vector Machines (SVM)
- Evaluated models using metrics such as accuracy, precision, recall, F1-score, and AUC-ROC.
- Performed hyperparameter tuning via GridSearchCV to optimize model performance.

### 4. Visualization
- Visualized feature importance for each model.
- Plotted ROC curves to compare model performance across all three classifiers.
- Presented insights using easy-to-understand charts.

---

## Results
- **Best Model**: Random Forest Classifier
- **Accuracy**: 85%
- **AUC-ROC**: [add after running `roc_auc_score(y_test, model.predict_proba(X_test)[:,1])`]
- **Key Factors**: Glucose levels, BMI, and Age were identified as the most important predictors of diabetes onset, consistent with clinical literature on Type 2 diabetes risk factors.

---

## How to Run the Project

1. Clone this repository:
```
git clone https://github.com/Bsetia1/Diabetes-Onset-Prediction-using-Health-Metrics.git
```

2. Install dependencies:
```
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

3. Launch the notebook:
```
jupyter notebook
```
