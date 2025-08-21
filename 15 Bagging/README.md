# Heart Disease Prediction with Ensemble Learning (Bagging)

This project focuses on **classification** and **ensemble learning** using a real-world dataset to predict the presence of heart disease. It demonstrates advanced data preprocessing techniques and the use of bagging classifiers to improve model performance.

---

### **Project Objective**

* To perform data preprocessing, including outlier removal and handling categorical variables.
* To build a classification model using **ensemble learning**, specifically `BaggingClassifier`.
* To compare the performance of different base estimators within the bagging framework, such as **Support Vector Classifier (SVC)** and **Decision Tree Classifier**.
* To evaluate the models using cross-validation and out-of-bag (OOB) scoring.

---

### **Files in This Repository**

* `heart.csv`: A dataset containing various health metrics and a binary target variable `HeartDisease`.
* `1_Analysis.ipynb`: The Jupyter Notebook with all the code, analysis, and results for this project.

---

### **Data Preprocessing and Analysis**

The `1_Analysis.ipynb` notebook outlines the following key data preparation steps:
* **Outlier Removal**: The notebook identifies and removes outliers from several features, including `RestingBP`, `Cholesterol`, `MaxHR`, and `Oldpeak`. This is done by filtering out data points that fall outside of three standard deviations from the mean.
* **Categorical to Numerical**: Categorical features `ExerciseAngina` and `Sex` were converted to numerical values (`0` and `1`).
* **One-Hot Encoding**: The remaining categorical columns like `ChestPainType`, `RestingECG`, and `ST_Slope` are one-hot encoded to create new binary features for each unique category.

### **Modeling and Results**

The project uses `BaggingClassifier` with two different base estimators:
* **SVC Bagging**: A bagging model with 100 `SVC` estimators was trained and achieved an out-of-bag score of **86.51%** and a test score of **89.44%**.
* **Decision Tree Bagging**: A bagging model with 100 `DecisionTreeClassifier` estimators was trained and achieved an out-of-bag score of **84.7%** and a test score of **86.11%**.

---

### **What I've Learned**

* **Ensemble Learning**: Bagging is a powerful technique to improve model stability and accuracy by reducing variance, as demonstrated by the improved scores compared to a single SVC or Decision Tree classifier.
* **Robust Data Cleaning**: I've practiced crucial data cleaning steps, such as outlier removal and handling different types of categorical data, which are vital for building effective models.
* **Model Evaluation**: I've learned how to use OOB scoring and test set scores to evaluate a bagging model's performance.