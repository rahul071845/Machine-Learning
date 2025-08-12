# Titanic Survival Prediction: A Classification Project

This project focuses on a classic machine learning problem: predicting survival on the Titanic. Using a dataset of passenger information, a classification model is built and trained to predict whether an individual survived the disaster.

---

### **Project Objective**

* To practice data preprocessing on a real-world dataset.
* To handle missing values and encode categorical features.
* To build and train a **Decision Tree Classifier** to predict a binary outcome (survived or not survived).
* To evaluate the model's performance on a test set.

---

### **Files in This Repository**

* `titanic.csv`: The dataset containing various features for each passenger on the Titanic, including age, gender, and ticket class.
* `1_Analysis.ipynb`: This Jupyter Notebook contains all the code for the project, from data loading to model evaluation.

---

### **Data Preprocessing and Analysis**

The `1_Analysis.ipynb` notebook outlines the following steps to prepare the data for the model:

* **Feature Selection**: Several irrelevant features were dropped from the dataset, including `PassengerId`, `Name`, `SibSp`, `Parch`, `Ticket`, `Cabin`, and `Embarked`.
* **Missing Values**: The `Age` column had missing values, which were filled with the median age of the dataset to prevent errors during training.
* **Categorical Encoding**: The `Sex` column, which contained text (`male` and `female`), was converted into numerical values using `LabelEncoder` from `scikit-learn`.

### **Modeling and Results**

* **Model**: A `DecisionTreeClassifier` model was chosen for this classification task and trained on the preprocessed data.
* **Evaluation**: The model was trained on 80% of the data and tested on the remaining 20%. The model achieved a prediction accuracy score of approximately **73.74%** on the test set.

---

### **What I've Learned**

* How to handle and prepare real-world, messy data for a machine learning model.
* The importance of dropping irrelevant features and handling missing values.
* A practical application of a classification model, specifically the **Decision Tree Classifier**, to predict a binary outcome.
* The process of splitting data and evaluating a model's performance on unseen data.