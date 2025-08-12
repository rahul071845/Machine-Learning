# Classification with Logistic Regression

This project is an introduction to **classification**, a fundamental machine learning task, using the classic **Iris dataset** and the **Logistic Regression** algorithm.

---

### **Project Objective**

* To learn the fundamentals of **classification**, a type of supervised learning.
* To use the `sklearn` library to train and evaluate a **Logistic Regression** model.
* To understand the importance of splitting data into training and testing sets.
* To evaluate a classification model's performance using a **confusion matrix**.

---

### **Dataset**

The project uses the built-in **Iris dataset** from `scikit-learn`. This is a famous dataset that contains measurements of iris flowers from three different species: `setosa`, `versicolor`, and `virginica`. The features used in the model are:
* `sepal length (cm)`
* `sepal width (cm)`
* `petal length (cm)`
* `petal width (cm)`

---

### **Code and Analysis**

The code is in the `1_Analysis.ipynb` Jupyter Notebook.
* The data is first loaded and then split into training and testing sets, with 20% of the data reserved for testing.
* A `LogisticRegression` model is created and trained on the training data.
* The model's performance on the test data is evaluated, and a **confusion matrix** is generated. The confusion matrix provides a detailed breakdown of correct and incorrect predictions for each class.

---

### **What I've Learned**

* **Logistic Regression**: It is a powerful algorithm for solving classification problems.
* **Data Splitting**: Splitting data into training and testing sets is crucial to ensure the model's performance is evaluated on unseen data, preventing overfitting.
* **Confusion Matrix**: This visualization is a key tool for understanding the strengths and weaknesses of a classification model, showing where the model succeeded and where it failed.