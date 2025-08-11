# One-Hot Encoding and Multivariable Linear Regression

This project demonstrates the process of handling categorical data in a machine learning model, a crucial step known as **one-hot encoding**. It uses a car price dataset to build and train a multivariable linear regression model.

---

### **Project Objective**

* To understand and apply **one-hot encoding** to convert categorical text data into a numerical format suitable for machine learning algorithms.
* To use the `pandas` library for efficient data manipulation and preprocessing.
* To build a linear regression model with multiple variables using the `scikit-learn` library.

---

### **Files in This Repository**

* `carprices.csv`: The primary dataset for the project. It contains data on various car models, their mileage, and prices.
* `1_Using_Pandas.ipynb`: This notebook focuses on data preprocessing. It demonstrates how to read the CSV file, identify the categorical `Car Model` column, and apply one-hot encoding using `pandas.get_dummies()`.
* `2_Using_Sklearn.ipynb`: This notebook builds upon the preprocessed data. It shows how to split the data into training and testing sets, train a `LinearRegression` model from `scikit-learn`, and then make predictions.

---

### **Key Concepts**

1.  **Categorical Variables**: Machine learning models typically require numerical input. Columns like "Car Model" are categorical and need to be converted before the model can be trained.
2.  **One-Hot Encoding**: A technique that transforms categorical variables into a numerical format. It creates a new binary column for each unique category, where a `1` indicates the presence of that category and a `0` indicates its absence. This prevents the model from assuming a false ordinal relationship between categories.
3.  **Multivariable Linear Regression**: An extension of linear regression that uses multiple independent variables (in this case, mileage and the one-hot encoded car models) to predict a single dependent variable (price).

By completing this project, I've learned how to prepare non-numerical data for a machine learning model and successfully built a more complex regression model.