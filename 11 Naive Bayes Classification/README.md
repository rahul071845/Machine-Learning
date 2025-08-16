# Naive Bayes Classification

This project is an introduction to **classification** using the **Naive Bayes** family of algorithms. It demonstrates how to build and compare two types of Naive Bayes classifiers on the classic wine dataset.

---

### **Project Objective**

* To understand the fundamentals of the **Naive Bayes** algorithm.
* To use the `scikit-learn` library to implement both **Gaussian Naive Bayes** and **Multinomial Naive Bayes**.
* To compare the performance of these two models on a classification task.

---

### **Dataset**

The project uses the **Wine dataset**, which is loaded directly from `scikit-learn`. This is a classification dataset with 13 features describing the chemical properties of different wines and the cultivar they came from. The goal is to predict the cultivar based on the wine's chemical analysis.

---

### **Code and Analysis**

The code is in the `1.Analysis.ipynb` Jupyter Notebook.
* The data is loaded from `scikit-learn` and split into training and testing sets.
* Two models, a **Gaussian Naive Bayes** (`GaussianNB`) and a **Multinomial Naive Bayes** (`MultinomialNB`), are created and trained on the data.
* The performance of each model is evaluated on the test data.

#### **Model Performance**

The accuracy scores on the test set were as follows:
* **Gaussian Naive Bayes**: `1.0`
* **Multinomial Naive Bayes**: `0.888...`

---

### **What I've Learned**

* **Naive Bayes**: I've gained a fundamental understanding of how this probabilistic algorithm can be used for classification.
* **Gaussian vs. Multinomial**: The performance difference highlights that the choice of Naive Bayes variant depends on the data. In this case, Gaussian Naive Bayes, which assumes features follow a normal distribution, was a better fit for the dataset than the Multinomial variant.