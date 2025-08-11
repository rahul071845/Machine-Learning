# Model Persistence with Pickle and Joblib

This project demonstrates the crucial concept of **model persistence** in machine learning, which involves saving a trained model to a file and later loading it for future use without the need for retraining.

---

### **Project Objective**

* To learn how to use the `pickle` and `joblib` libraries to save a trained machine learning model to a file.
* To load the saved model files and use them to make predictions, confirming that the model's state is preserved.
* To understand the differences and common use cases for both libraries.

---

### **Files in This Repository**

* `1_Using_Pickle_Joblib.ipynb`: A Jupyter Notebook that walks through the process of training a linear regression model, saving it using both `pickle` and `joblib`, and then loading the saved models.
* `canada_per_capita_income.csv`: The dataset used to train the linear regression model.
* `model_pickle`: The binary file containing the model saved with the `pickle` library.
* `model_joblib`: The binary file containing the model saved with the `joblib` library.

---

### **Analysis and Key Learnings**

The project uses the linear regression model from a previous topic to demonstrate model persistence.

#### **Pickle**
The `pickle` library serializes and deserializes Python objects, converting an object into a byte stream. This allows the model object to be saved to a file (`model_pickle`).

#### **Joblib**
The `joblib` library is a more efficient alternative to `pickle` for large models, especially those containing NumPy arrays. It stores data more effectively, making it faster to save and load large models. This is demonstrated by saving the model to `model_joblib`.

By completing this project, I've learned that model persistence is a vital step in the machine learning workflow, enabling models to be deployed and reused efficiently without repeating the training process.