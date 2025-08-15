# Digit Classification with Support Vector Machines (SVM)

This project is a practical exercise in **classification** using a classic dataset and the **Support Vector Machine (SVM)** algorithm. It focuses on training a model to recognize handwritten digits and explores the impact of different kernel functions on the model's performance.

---

### **Project Objective**

* To use the `scikit-learn` library to build a classification model for image data.
* To understand the concept of **Support Vector Machines (SVM)** and its use in digit recognition.
* To compare the performance of different SVM kernels: `rbf`, `linear`, `sigmoid`, and `poly`.
* To practice splitting data into training and testing sets and evaluating the model's accuracy.

---

### **Dataset**

The project utilizes the **Digits dataset** from `scikit-learn`. This dataset consists of 1,797 8x8 pixel images of handwritten digits, from 0 to 9. Each image is represented as a flattened array of 64 pixel values. The goal is to predict the correct digit (0-9) based on these pixel values.

---

### **Code and Analysis**

The code is in the `1_Analysis.ipynb` Jupyter Notebook.
* The data is loaded and structured into a `pandas` DataFrame.
* The dataset is split into training and testing sets, with 20% of the data allocated for testing.
* Several `SVC` (Support Vector Classifier) models are trained, each with a different kernel function.

#### **Model Performance**

The accuracy of each kernel on the test data is as follows:
* **RBF kernel**: `0.986` (98.6%)
* **Linear kernel**: `0.978` (97.8%)
* **Polynomial kernel**: `0.986` (98.6%)
* **Sigmoid kernel**: `0.078` (7.8%)

---

### **What I've Learned**

* **SVMs for Classification**: SVMs are a powerful tool for classification tasks, capable of finding complex decision boundaries.
* **Kernel Functions**: The choice of kernel is critical for model performance. The `rbf` and `poly` kernels performed exceptionally well on this dataset, while the `sigmoid` kernel performed poorly.
* **Data Splitting**: Splitting the data is essential for a fair evaluation of the model's ability to generalize to new, unseen data.