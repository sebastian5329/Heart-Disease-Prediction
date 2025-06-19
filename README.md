# Heart-Disease-Prediction
Project Aim

The main aim of this project is to create a model to predict the likelihood of heart disease in patients using clinical and demographic data. This can help healthcare providers identify high-risk patients early and take proactive measures.

How It Helps

1)Early Detection: Flags individuals at risk of heart disease before symptoms become severe.
2)Data-Driven Decisions: Helps doctors make more informed decisions with supporting analytics.
3)Resource Allocation: Enables hospitals to prioritise patients who require urgent care.
4)Cost-effective Screening: Useful in remote areas where full diagnostics may not be readily available.

Workflow Overview

1) Data Collection
Used a structured heart disease dataset with features like age, cholesterol, heart rate, etc.
2) Exploratory Data Analysis (EDA)
• Identified feature distributions, class imbalance, and correlations.
• Detected influential predictors such as chest pain type, oldpeak, and exercise-induced angina.
3) Data Preprocessing
• Categorical column (thal )was encoded using one hot encoder. 
• Applied StandardScaler to numerical  columns such as:
    a)Resting Blood Pressure
		b)Serum Cholesterol
		c)Max Heart Rate
		d)ST Depression (oldpeak)
• Balanced the dataset using SMOTE (Synthetic Minority Oversampling Technique).
4) Model Building
Trained and evaluated several classification algorithms:
	  a)Logistic Regression
    b)KNN
    c)Support Vector Machine (SVC)
	  d)Decision Tree
	  e)Random Forest (Best)
	  f)Gradient Boosting
	  g)XGBoost
5) Hyper-parameter Tuning
Used both RandomizedSearchCV and GridSearchCV to optimize models.
6) Evaluation Metrics
   a)Accuracy
   b)Precision
   c)Recall
   d)F1-Score

Result

Best Performing Model: 
Random Forest Classifier
f1 score: 0.8
accuracy score:0.82
precision score:0.8
recall score:0.8

Key Insights

• Oldpeak (ST depression) was a strong predictor of heart disease.
• Scaling impacted different models differently – some like SVM and Logistic Regression performed better after scaling.
• Random Forest outperformed gradient and XGBoost models due to its robustness and lower variance.
• Decision Tree had a strong recall (0.86), which is crucial in medical diagnosis but slightly lower precision.
• XGBoost had high recall (0.86) but suffered in precision (0.68), making Random Forest more balanced.

Conclusion

This project demonstrates how machine learning can play a vital role in healthcare by offering predictive capabilities that assist in timely diagnosis and better patient outcomes. It also highlights the importance of model tuning and data preprocessing in achieving optimal performance.
