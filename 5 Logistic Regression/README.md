# HR Analytics: Employee Turnover Prediction

This project is an exploratory data analysis and predictive modeling exercise using a dataset of employee information. The primary goal is to build a model that can predict which employees are likely to leave the company.

---

### **Project Objective**

* To explore and visualize key features of the employee dataset.
* To perform data preprocessing, including handling categorical variables.
* To build a machine learning model for **classification** to predict employee turnover.

---

### **Files in This Repository**

* `hr_analytics.csv`: This dataset contains 14,999 employee records with 10 features, including performance metrics, project counts, salary, and whether they have left the company.
* `1_Analysis.ipynb`: A Jupyter Notebook that begins the data analysis process. It includes data loading, initial data exploration, and likely some visualization to understand the relationships between different features and the `left` variable.

---

### **Key Concepts & Analysis**

The analysis focuses on predicting the `left` column, which acts as the target variable for a classification task. The value `1` indicates an employee has left, while `0` indicates they are still with the company.

The dataset includes several important features:
* **Numerical Features**: `satisfaction_level`, `last_evaluation`, `number_project`, `average_montly_hours`, `time_spend_company`.
* **Categorical Features**: `Department` and `salary` are text-based columns that will require preprocessing (e.g., one-hot encoding) before being used in the model.

The notebook begins by using `pandas` for data manipulation and `matplotlib` for visualization, which are standard practices for understanding a dataset before modeling begins. This project is a great example of using data to solve a real-world business problem like predicting employee turnover.