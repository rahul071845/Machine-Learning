# Multiple Variable Linear Regression

This is my second project, where I'm expanding my understanding of linear regression to include **multiple variables**.

## **Project Goal**

The main goal of this project is to:
* Learn how to use multiple features (independent variables) to predict a single target variable.
* Practice data cleaning and preprocessing techniques, such as handling text data and missing values.
* Use `scikit-learn`'s `LinearRegression` model with multiple inputs.

## **Dataset**

The dataset used is `hiring.csv`. It contains information about job applicants and their salaries. The columns are:
* `experience`: The number of years of work experience (note: some values are text).
* `test_score(out of 10)`: The score the candidate received on a test (note: some values are missing).
* `interview_score(out of 10)`: The score the candidate received in their interview.
* `salary($)`: The target variable—the salary offered to the candidate.

## **Data Preprocessing**

Before building the model, I performed some essential data cleaning steps:
* **Handling Text Data**: The `experience` column, which contained text like 'two' and 'five', was converted to numerical values (2 and 5) to be used in the model.
* **Handling Missing Values**: The missing values in the `test_score` column were filled in, likely with the mean or median of the existing scores, to ensure the model could be trained without errors.

## **Code and Analysis**

The code for this project is in the `2_MultipleVariable.ipynb` Jupyter Notebook.
* The model uses `experience`, `test_score`, and `interview_score` as features to predict the `salary`.
* After training the model on the cleaned data, I can use it to make predictions for new candidates.
* For example, a candidate with **2 years** of experience, a **test score of 9**, and an **interview score of 6** is predicted to have a salary of approximately **$53,713.87**.
* A candidate with **12 years** of experience, a **test score of 10**, and an **interview score of 10** is predicted to have a salary of approximately **$93,747.80**.

## **What I've Learned**

* How to handle datasets with multiple features.
* The importance of data preprocessing, including handling categorical data (text) and missing numerical data.
* How to fit a more complex linear regression model and interpret its output.