# Digit Classification with K-Nearest Neighbors (KNN)

This project is a deep dive into **classification** and **model evaluation** using the **K-Nearest Neighbors (KNN)** algorithm. It focuses on predicting handwritten digits and uses advanced techniques like **Grid Search** to find the optimal model.

---

### **Project Objective**

* To use the `scikit-learn` library to build a classification model for image data.
* To understand the concept of **K-Nearest Neighbors (KNN)** and its application in digit recognition.
* To use **Grid Search** with cross-validation to find the best number of neighbors (`n_neighbors`) for the KNN model.
* To evaluate the model's performance using a **confusion matrix** and a **classification report**.

---

### **Dataset**

The project utilizes the **Digits dataset** from `scikit-learn`. This dataset consists of 8x8 pixel images of handwritten digits, from 0 to 9. The goal is to predict the correct digit (0-9) based on these pixel values.

---

### **Code and Analysis**

The code is in the `1_Analysis.ipynb` Jupyter Notebook.
* The data is loaded and split into training and testing sets, with 20% of the data allocated for testing.
* **Grid Search**: A grid search was performed to find the best value for `n_neighbors` by testing `3`, `5`, `7`, and `9`. The best score of `0.967` was achieved with `n_neighbors=3`.
* **Model Evaluation**: A final KNN model with `n_neighbors=3` was trained and tested. The model achieved an accuracy of approximately **98.33%** on the test set.
* **Visualizing Results**: A **confusion matrix** was generated to visualize the model's performance across different digits. The matrix and a **classification report** showed that the model performed exceptionally well, with high precision, recall, and f1-scores for most digits.

---

### **What I've Learned**

* **KNN Algorithm**: I've gained a deeper understanding of how this simple, yet powerful, algorithm works by classifying data points based on their neighbors.
* **Hyperparameter Tuning**: **Grid Search** is a powerful technique to find the optimal settings for a model's hyperparameters, which can significantly improve performance.
* **Comprehensive Evaluation**: Beyond a simple accuracy score, tools like a **confusion matrix** and **classification report** provide a detailed view of a classification model's strengths and weaknesses.