**Heart Attack Risk Prediction using Machine Learning**

**📌 Project Overview**

Heart disease is one of the leading causes of death worldwide. Early detection and timely intervention can significantly reduce the risk of fatal outcomes. This project leverages machine learning algorithms to analyze patient health data and predict the risk of a heart attack by classifying individuals into Low Risk and High Risk categories.
The goal is to assist healthcare professionals in identifying high-risk individuals and enable preventive care using data-driven insights.


📊 Dataset Information
•	Source: Kaggle

•	Records: 100,000 entries

•	Features:
    o	Age
    o	Gender
    o	Blood Pressure (Systolic & Diastolic)
    o	Cholesterol Levels (HDL, LDL, Total)
    o	Smoking Habits
    o	Diabetes
    o	Family History
    o	Physical Activity
    o	Diet (Fat/Salt intake)
    o	BMI
    o	Blood Sugar Levels
    o	Stress Levels
    o	Heart Rate
    o	ECG
    o	Exercise-Induced Angina
•	Target Variable:
    o	Heart Attack Risk: 1 (High Risk), 0 (Low Risk)
    
**🛠️ Technologies & Libraries Used**
•	Language: Python
•	Libraries:
    o	pandas, numpy – Data handling
    o	scikit-learn – ML algorithms and preprocessing
    o	matplotlib, seaborn – Visualization (optional)
•	ML Models:
    o	Naive Bayes Classifier
    o	K-Nearest Neighbors (KNN)
    o	Logistic Regression
    o	Linear Regression

**🧠 Implementation Steps**
1. Data Preprocessing
    •	Handled missing values
    •	Encoded categorical features using LabelEncoder
    •	Applied feature scaling using StandardScaler
2. Model Training
    •	Splitting dataset with various train-test ratios: 50:50, 60:40, 70:30, 80:20
    •	Trained each model on all splits to analyze performance consistency
3. Model Evaluation
    •	Evaluation metrics:
      o	Accuracy
      o	F1 Score
    •	Best performance was achieved using K-Nearest Neighbors with 99.77% accuracy (80:20 split)
   
**📈 Accuracy Comparison Table**
Train-Test Split	Naive Bayes	KNN	Linear Regression	Logistic Regression
50:50	64.22%	96.65%	64.23%	64.23%
60:40	64.09%	98.54%	64.09%	64.09%
70:30	64.03%	99.26%	64.03%	64.03%
80:20	64.20%	99.77%	64.20%	64.02%

**🎯 Key Insights**
    •	KNN performed exceptionally well due to:
        o	Clear separation of risk categories
        o	Well-scaled data
        o	Optimal value of k chosen (k=5)
    •	Logistic and Linear Regression underperformed due to potential linearity limitations
    •	Naive Bayes had consistent but lower accuracy, possibly due to feature dependency
    
**✅ Conclusion**
This project demonstrates how machine learning can be used in healthcare to predict critical outcomes like heart attacks. The KNN model proved to be the most accurate and reliable in this context.
Further improvements could include:
    •	Incorporating more lifestyle and genetic data
    •	Feature selection/engineering for better model training
    •	Deploying the model as a web-based risk assessment tool for clinics


