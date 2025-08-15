# Classification with Random Forest

This project is an introduction to **classification**, a fundamental machine learning task, using the classic **Iris dataset** and the **Random Forest Classifier** algorithm.

---

### **Project Objective**

* To learn the fundamentals of **classification**, a type of supervised learning.
* To use the `sklearn` library to train and evaluate a **Random Forest Classifier** model.
* To understand the importance of splitting data into training and testing sets.
* To explore the effect of a key hyperparameter (`n_estimators`) on model performance.

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
* The data is first loaded and then split into training and testing sets, with 30% of the data reserved for testing.
* A `RandomForestClassifier` model is created and trained on the training data.
* The model's performance on the test data is evaluated, achieving a perfect score of **1.0**.
* Additionally, a second model with `n_estimators=1` was tested, resulting in a score of approximately **0.978**. This demonstrates how the number of trees in the forest can affect accuracy.

---

### **What I've Learned**

* **Random Forest**: It is a powerful ensemble learning algorithm for classification.
* **Data Splitting**: Splitting data into training and testing sets is crucial to ensure the model's performance is evaluated on unseen data, preventing overfitting.
* **Hyperparameter Tuning**: Key parameters, such as `n_estimators`, can be adjusted to optimize the model's performance.