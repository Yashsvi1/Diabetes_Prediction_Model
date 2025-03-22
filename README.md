# Diabetes Prediction Project

## Project Background

The Diabetes Prediction Project aims to analyze health-related attributes to predict the likelihood of diabetes. This project involves data cleaning, feature engineering, model building, and evaluation to derive meaningful insights for diabetes prediction. The objective is to improve prediction accuracy using various machine learning models while ensuring data reliability and integrity.

## Insights and Recommendations

### Data Exploration and Cleaning

#### **Category 1: Data Analysis and Cleaning**
- **Insight 1**: The dataset shows a high average glucose level, indicating a potential risk of diabetes among the population.
- **Insight 2**: BMI values exhibit a wide distribution with noticeable outliers.
- **Insight 3**: Some blood pressure values are recorded as zero, indicating missing or incorrect data.
- **Insight 4**: Insulin levels display significant variation, requiring further analysis.

  ![image](https://github.com/user-attachments/assets/e2163c2b-9b42-4f1f-ac90-65d2b308bcf2)


#### **Data Cleaning Process**
- **Outlier Handling**: The IQR method was used to detect and remove extreme outliers in insulin and skin thickness.
- **Missing Values Handling**: Median imputation was applied to missing values in insulin and skin thickness to retain as much data as possible.

  ![image](https://github.com/user-attachments/assets/faa40b9b-cb97-4015-a523-da22827681f5)


### Feature Engineering

#### **Category 2: Feature Creation and Selection**
- **Insight 1**: New features such as the **Glucose-BMI Index** and **Age-BMI Index** were created to capture metabolic risk factors.
- **Insight 2**: Correlation analysis helped eliminate redundant features to improve model performance.

### Model Building and Evaluation

#### **Category 3: Model Selection and Performance**
- **Insight 1**: Several models were tested, including Logistic Regression, Random Forest, SVM, Decision Tree, and XGBoost.
- **Insight 2**: Random Forest was selected as the best model due to its superior **AUC-ROC** and **Recall**, which are crucial for medical predictions.
- **Insight 3**: Cross-validation was performed to ensure the robustness of model performance.

## Data Structure & Initial Checks

### **Diabetes Dataset**
The dataset consists of multiple health-related attributes used to predict diabetes outcomes.

#### **Columns:**
- **Pregnancies**: Number of times the individual has been pregnant.
- **Glucose**: Plasma glucose concentration.
- **BloodPressure**: Diastolic blood pressure (mm Hg).
- **SkinThickness**: Triceps skinfold thickness (mm).
- **Insulin**: 2-Hour serum insulin (mu U/ml).
- **BMI**: Body Mass Index.
- **DiabetesPedigreeFunction**: A function that scores the likelihood of an individual having diabetes based on family history.
- **Age**: Age of the individual.
- **Outcome**: Whether the individual has diabetes (1) or not (0).

#### **Total Records:** 768 entries

## Executive Summary

### **Key Findings**
- **Data Reliability**: Handling missing values and outliers improved model accuracy.
- **Feature Engineering**: New composite features enhanced predictive power.
- **Model Performance**: Random Forest outperformed other models in Recall and AUC-ROC.

### **Insights Deep Dive**

#### **Data Insights**
- **Glucose and BMI** are strong predictors of diabetes.
- **Feature interaction** significantly improved model performance.
- **Addressing missing values and outliers** led to a more reliable dataset.

#### **Model Insights**
- **Random Forest** achieved the highest Recall, making it the best model for this medical prediction task.
- **Cross-validation** ensured generalizability and robustness.
  
  ![image](https://github.com/user-attachments/assets/1b20b3fc-45a5-441d-b9e1-cd6ccbe099b3)
  
  ![image](https://github.com/user-attachments/assets/159c2059-a806-446e-bfaf-83aa9f622c69)



## Recommendations

1. **Improve Data Collection**: Collect additional data to enhance model accuracy.
2. **Explore Deep Learning**: Implement neural networks for better performance.
3. **Deployment**: Deploy the model as a web app for real-world usability.

## Assumptions and Caveats

- Missing or erroneous data was excluded or imputed using median values.
- Feature engineering was based on domain knowledge and statistical analysis.
- Model selection was based on Recall, as false negatives in diabetes prediction are more critical than false positives.

This README serves as a documentation template for the Diabetes Prediction Project, ensuring clarity, reproducibility, and actionable insights for stakeholders.

