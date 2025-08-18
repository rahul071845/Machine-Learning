# Heart Disease Prediction and Model Evaluation

This project is a comprehensive machine learning exercise focused on building and evaluating models to predict the presence of heart disease. It demonstrates key steps in the data science workflow, from data preprocessing to comparing multiple models.

---

### **Project Objective**

* To explore and prepare a real-world medical dataset for machine learning.
* To perform essential data preprocessing steps, including one-hot encoding and data scaling.
* To build and compare the performance of several classification models, including **Logistic Regression**, **Support Vector Classifier (SVC)**, and **Random Forest Classifier**.
* To explore the effect of **Principal Component Analysis (PCA)** on model performance.

---

### **Files in This Repository**

* `heart.csv`: The dataset containing various health metrics and a target variable indicating the presence of heart disease.
* `1_Analysis.ipynb`: The Jupyter Notebook containing all the code and analysis for this project.

---

### **Key Concepts & Analysis**

The `1_Analysis.ipynb` notebook outlines the following key steps:

* **Data Preprocessing**: Categorical features like `Sex` and `ExerciseAngina` were converted to numerical values using `LabelEncoder`. Other categorical columns like `ChestPainType` were handled using one-hot encoding with `pandas.get_dummies`. The data was then scaled using `MinMaxScaler` to ensure all features had a similar range.
* **Model Comparison**: The project compares the performance of three different models: Logistic Regression, SVC, and Random Forest Classifier.
* **Dimensionality Reduction**: Principal Component Analysis (PCA) was applied to the dataset to reduce the number of features while retaining 95% of the variance. The number of components was reduced to 10. The models were then re-evaluated on this reduced dataset.

### **Model Performance**

The average cross-validation scores for the models, both with and without PCA, are as follows:

* **Logistic Regression**: `0.830` (without PCA), `0.831` (with PCA)
* **SVC**: `0.832` (without PCA), `0.832` (with PCA)
* **Random Forest Classifier**: `0.827` (without PCA), `0.812` (with PCA)

Based on these results, the **SVC** and **Logistic Regression** models performed the best, and PCA had a minimal impact on their performance.

---

### **What I've Learned**

* **Data Preparation**: The importance of cleaning, preprocessing, and scaling data before feeding it into a machine learning model.
* **Model Selection**: It's crucial to compare different models to find the one best suited for a specific problem.
* **Dimensionality Reduction**: I've gained an understanding of how PCA can be used to reduce the complexity of a dataset without significantly compromising model accuracy.