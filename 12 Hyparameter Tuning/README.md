# Multi-Model Classification with Grid Search

This project focuses on a key step in the machine learning workflow: **hyperparameter tuning** and **model selection**. It compares the performance of several classification algorithms and uses `GridSearchCV` to find the best-performing model and its optimal parameters on the handwritten digits dataset.

---

### **Project Objective**

* To compare the performance of several popular machine learning classification models.
* To use **Grid Search** and **cross-validation** to systematically find the best hyperparameters for each model.
* To identify the best-performing model and its optimal configuration for this specific dataset.

---

### **Dataset**

The project uses the **Digits dataset** from `scikit-learn`. This dataset consists of 1,797 8x8 pixel images of handwritten digits, from 0 to 9. The goal is to predict the correct digit (0-9) based on these pixel values.

---

### **Code and Analysis**

The code is in the `1_Analysis.ipynb` Jupyter Notebook. It sets up a dictionary of models and their respective parameter grids to be tested. The `GridSearchCV` function then performs cross-validation for each model and parameter combination to find the best fit.

The results of the analysis are summarized in a DataFrame:

* **logistic_regression**: Best score: `0.922`, Best parameters: `{'C': 1}`.
* **decision_tree**: Best score: `0.812`, Best parameters: `{'criterion': 'entropy', 'max_depth': 20, 'min_samples_leaf': 4, 'min_samples_split': 2}`.
* **svm**: Best score: `0.947`, Best parameters: `{'C': 1, 'kernel': 'linear'}`.
* **random_forest**: Best score: `0.925`, Best parameters: `{'n_estimators': 20}`.
* **gaussian_nb**: Best score: `0.806`.
* **multi_nb**: Best score: `0.870`, Best parameters: `{'alpha': 0.1}`.

Based on these results, the **Support Vector Machine (SVM)** with a **linear kernel** and a C value of 1 was the top-performing model with an accuracy of approximately **94.7%** on this dataset.

---

### **What I've Learned**

* **Grid Search**: This is an effective and automated way to search for the best hyperparameters for a model.
* **Model Selection**: Different algorithms perform differently on the same dataset. This project highlights the importance of trying multiple models to find the one that fits the data best.
* **Robust Evaluation**: Using cross-validation provides a more reliable estimate of a model's performance than a single train-test split.