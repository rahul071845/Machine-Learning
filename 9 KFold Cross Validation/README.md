# Multi-Model Classification with Cross-Validation

This project compares the performance of several popular machine learning classification models on the classic **Iris dataset** using **cross-validation**. The goal is to understand how different algorithms perform on the same data and to evaluate their accuracy in a robust way.

---

### **Project Objective**

* To use the `scikit-learn` library to train and evaluate multiple classification models, including:
    * **Logistic Regression**
    * **Decision Tree Classifier**
    * **Support Vector Classifier (SVC)**
    * **Random Forest Classifier**
* To use **k-fold cross-validation** to get a more reliable estimate of each model's performance.
* To compare the average accuracy scores of the different models.

---

### **Dataset**

The project uses the built-in **Iris dataset** from `scikit-learn`. This is a famous dataset that contains measurements of iris flowers from three different species: `setosa`, `versicolor`, and `virginica`. The four features (`sepal length`, `sepal width`, `petal length`, and `petal width`) are used to predict the species of the flower.

---

### **Code and Analysis**

The code is in the `1_Analysis.ipynb` Jupyter Notebook.
* The data is loaded from `scikit-learn`.
* The `cross_val_score` function is used to evaluate each model's performance. It splits the data into multiple folds, trains the model on some folds, and tests it on the remaining one, repeating this process for all folds to get an average score.
* The average scores for each model are as follows:
    * **Logistic Regression**: `97.33%`
    * **Decision Tree Classifier**: `96.00%`
    * **Support Vector Classifier (SVC)**: `96.67%`
    * **Random Forest Classifier**: `96.00%`

---

### **What I've Learned**

* **Cross-Validation**: This is a powerful technique to evaluate a model's performance and avoid overfitting. It provides a more robust accuracy score than a single train-test split.
* **Model Comparison**: Different algorithms can have varying performance on the same dataset. The Logistic Regression model performed slightly better than the others in this particular case.
* **Classification Models**: I've gained practical experience with several key classification models from the `scikit-learn` library.