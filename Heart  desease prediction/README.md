# Heart Disease Risk Prediction Model - Complete Guide

## 📋 Project Overview
This project builds a machine learning model to predict whether a person is at risk of heart disease based on their health data using the Heart Disease UCI Dataset.

## 📊 What's Included

### Notebook: `heart_disease_prediction.ipynb`

The notebook covers 10 comprehensive sections:

1. **Import Required Libraries**
   - pandas, numpy, scikit-learn, matplotlib, seaborn
   - All necessary tools for data analysis and ML modeling

2. **Load and Explore the Dataset**
   - Loads the dataset.csv file
   - Displays dataset shape, info, and statistical summary
   - Shows target variable distribution

3. **Data Cleaning and Preprocessing**
   - Checks for missing values (handled if any)
   - Removes duplicate rows
   - Identifies numerical and categorical columns
   - Prepares data for feature engineering

4. **Exploratory Data Analysis (EDA)**
   - Target distribution visualization
   - Age distribution analysis
   - Sex-based risk analysis
   - Correlation heatmap for all features
   - Chest pain type analysis
   - Thalassemia distribution
   - Max heart rate and cholesterol patterns

5. **Feature Engineering and Selection**
   - Encodes categorical variables using LabelEncoder
   - Prepares features (X) and target (y)
   - Creates train-test split (80-20)
   - Scales numerical features using StandardScaler

6. **Train Classification Models**
   - **Logistic Regression**: Linear classification model
   - **Decision Tree**: Tree-based classification model
   - Both models trained on scaled/original features as appropriate

7. **Model Evaluation and Metrics**
   - Accuracy, Precision, Recall, F1-Score
   - Confusion matrices for both models
   - Detailed classification reports
   - Evaluation on both training and test sets

8. **Feature Importance Analysis**
   - **Logistic Regression**: Coefficient-based importance
   - **Decision Tree**: Tree-based importance scores
   - Top 10 features visualization
   - Clinical interpretation of important features

9. **ROC Curve and AUC Analysis**
   - ROC curves for both models
   - AUC score calculation and interpretation
   - Model discrimination ability assessment
   - Comparison with random classifier baseline

10. **Summary and Conclusions**
    - Comprehensive summary report
    - Model performance comparison
    - Key features affecting prediction
    - Recommendations for clinical use

## 🚀 How to Run

### Prerequisites
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter ipykernel
```

### Running the Notebook
```bash
# Navigate to the project directory
cd /Users/tayyabraza/Desktop/DEVELOPERS_HUB/DEv_hub_tasks/TASK_3

# Launch Jupyter
jupyter notebook heart_disease_prediction.ipynb
```

## 📈 Key Features in the Analysis

### Features Used (13 total):
- **age**: Patient age in years
- **sex**: Patient gender (Male/Female)
- **chest_pain_type**: Type of chest pain experienced
- **resting_blood_pressure**: Blood pressure at rest
- **cholestoral**: Serum cholesterol level
- **fasting_blood_sugar**: Fasting blood sugar level
- **rest_ecg**: Resting electrocardiographic results
- **Max_heart_rate**: Maximum heart rate achieved
- **exercise_induced_angina**: Presence of exercise-induced angina
- **oldpeak**: ST depression induced by exercise
- **slope**: Slope of the ST segment
- **vessels_colored_by_flourosopy**: Number of vessels colored by fluoroscopy
- **thalassemia**: Thalassemia type

### Target Variable:
- **0**: No heart disease risk
- **1**: Heart disease risk present

## 📊 Expected Model Performance

The notebook will generate:
- **Confusion Matrices**: Visual representation of True Positives, True Negatives, False Positives, False Negatives
- **ROC Curves**: Receiver Operating Characteristic curves for both models
- **Feature Importance Plots**: Bar charts showing top features
- **Performance Metrics**: 
  - Accuracy: Overall correctness
  - Precision: Accuracy of positive predictions
  - Recall: Coverage of actual positives
  - F1-Score: Harmonic mean of precision and recall
  - ROC-AUC: Area under the ROC curve

## 🔍 Output Interpretation

### Accuracy
- Percentage of correct predictions
- Range: 0-100%

### ROC-AUC Score
- 0.9-1.0: Excellent discrimination
- 0.8-0.9: Good discrimination
- 0.7-0.8: Fair discrimination
- 0.6-0.7: Poor discrimination

### Feature Importance
- **Positive coefficient (LR)**: Increases heart disease risk
- **Negative coefficient (LR)**: Decreases heart disease risk
- Higher importance score (DT): More influential in predictions

## 💡 Medical Insights

The analysis will highlight which health factors are most important for predicting heart disease risk:
- Cardiovascular indicators (heart rate, blood pressure)
- ECG results and ST segment changes
- Exercise response and angina presence
- Blood chemistry indicators

## 📝 Notes

- The dataset is already cleaned and provided
- The model uses binary classification (Risk vs. No Risk)
- Both Logistic Regression and Decision Tree models are compared
- Recommendations are provided on which model to use

## 🎯 Use Cases

1. **Screening Tool**: Initial assessment of heart disease risk
2. **Clinical Decision Support**: Assist doctors in diagnosis
3. **Risk Stratification**: Identify high-risk patients
4. **Research**: Understand feature-target relationships

## ⚠️ Disclaimer

This model is for educational purposes and research use only. It should NOT be used for actual medical diagnosis without professional medical consultation. Always consult with a qualified healthcare provider for medical advice.

---

**Created**: 2026-04-28
**Dataset**: Heart Disease UCI Dataset
**Models**: Logistic Regression, Decision Tree
**Language**: Python with Jupyter Notebook
