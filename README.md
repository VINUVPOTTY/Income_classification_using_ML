# Income_classification_using_ML
💼 Income Classification using Machine Learning
📌 Project Overview
This project aims to predict whether an individual's income exceeds a certain threshold (commonly $50K) based on features such as education, work class, occupation, and others. We approach this as a binary classification problem using algorithms like K-Nearest Neighbors (KNN), Naive Bayes, and Support Vector Machine (SVM).

🧾 Dataset Summary
The dataset contains personal and professional details of individuals, including:

Work class

Education level

Occupation

Relationship status

Race and sex

Native country

Salary category (target)

Key Preprocessing Steps:
Label Encoding was applied to the target (salary) to convert it into numerical format.

Chi-Square Tests were used to identify categorical features with significant impact on income.

Irrelevant or less significant features like fnlwgt, race, sex, and native-country were dropped based on analysis.

📊 Exploratory Data Analysis
Boxplots were used to identify outliers in numeric features.

IQR filtering helped remove outliers and improve model robustness.

Correlation matrix and heatmaps were used to understand relationships between features.

Chi-squared tests helped evaluate categorical feature relevance.

🔄 Handling Imbalanced Data
The dataset initially had an imbalanced distribution of income classes. To resolve this:

SMOTE (Synthetic Minority Over-sampling Technique) was used to balance the dataset by generating synthetic examples of the minority class.

Post-SMOTE distribution was visualized to confirm class balance.

⚙️ Feature Engineering
One-Hot Encoding was applied to categorical variables like work class, education, and occupation.

These encoded features were then concatenated to the main dataset.

🧠 Model Building
Three classification algorithms were trained and compared:

K-Nearest Neighbors (KNN)

Bernoulli Naive Bayes

Support Vector Classifier (SVC)

Each model was trained on a 70/30 train-test split.

📏 Evaluation Metrics
Each model's performance was evaluated using:

Confusion Matrix

Accuracy Score

Classification Report (Precision, Recall, F1-Score)

Visual confusion matrices were also plotted for comparison.

✅ Results Summary
Model comparison showed differences in performance, with each classifier having strengths in different areas (e.g., precision vs. recall).

The use of SMOTE and Standard Scaling improved model fairness and performance across classes.

🔮 Future Improvements
Try ensemble models like Random Forest or XGBoost.

Apply hyperparameter tuning using Grid Search or Random Search.

Explore PCA or feature selection techniques to reduce dimensionality.
