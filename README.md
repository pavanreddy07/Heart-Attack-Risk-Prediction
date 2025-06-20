❤️ Heart Attack Risk Prediction using Machine Learning
A Machine Learning project to predict the risk of a heart attack based on individual health records using various classification algorithms.

📌 Project Overview
Heart disease is one of the leading causes of death worldwide. Early detection and timely intervention can significantly reduce the risk of fatal outcomes. This project leverages machine learning algorithms to analyze patient health data and predict the risk of a heart attack by classifying individuals into Low Risk and High Risk categories.

The goal is to assist healthcare professionals in identifying high-risk individuals and enable preventive care using data-driven insights.

📊 Dataset Information
Source: Kaggle

Records: 100,000 entries

Features:

Age

Gender

Blood Pressure (Systolic & Diastolic)

Cholesterol Levels (HDL, LDL, Total)

Smoking Habits

Diabetes

Family History

Physical Activity

Diet (Fat/Salt intake)

BMI

Blood Sugar Levels

Stress Levels

Heart Rate

ECG

Exercise-Induced Angina

Target Variable:

Heart Attack Risk: 1 (High Risk), 0 (Low Risk)

🛠️ Technologies & Libraries Used
Language: Python

Libraries:

pandas, numpy – Data handling

scikit-learn – ML algorithms and preprocessing

matplotlib, seaborn – Visualization (optional)

ML Models:

Naive Bayes Classifier

K-Nearest Neighbors (KNN)

Logistic Regression

Linear Regression

🧠 Implementation Steps
1. Data Preprocessing
Handled missing values

Encoded categorical features using LabelEncoder

Applied feature scaling using StandardScaler

2. Model Training
Splitting dataset with various train-test ratios: 50:50, 60:40, 70:30, 80:20

Trained each model on all splits to analyze performance consistency

3. Model Evaluation
Evaluation metrics:

Accuracy

F1 Score

Best performance was achieved using K-Nearest Neighbors with 99.77% accuracy (80:20 split)

📈 Accuracy Comparison Table
Train-Test Split	Naive Bayes	KNN	Linear Regression	Logistic Regression
50:50	64.22%	96.65%	64.23%	64.23%
60:40	64.09%	98.54%	64.09%	64.09%
70:30	64.03%	99.26%	64.03%	64.03%
80:20	64.20%	99.77%	64.20%	64.02%

🎯 Key Insights
KNN performed exceptionally well due to:

Clear separation of risk categories

Well-scaled data

Optimal value of k chosen (k=5)

Logistic and Linear Regression underperformed due to potential linearity limitations

Naive Bayes had consistent but lower accuracy, possibly due to feature dependency

✅ Conclusion
This project demonstrates how machine learning can be used in healthcare to predict critical outcomes like heart attacks. The KNN model proved to be the most accurate and reliable in this context.

Further improvements could include:

Incorporating more lifestyle and genetic data

Feature selection/engineering for better model training

Deploying the model as a web-based risk assessment tool for clinics
