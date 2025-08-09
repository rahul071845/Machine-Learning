# Gradient Descent for Linear Regression

This project focuses on understanding and implementing the **Gradient Descent** optimization algorithm. Gradient descent is a fundamental concept in machine learning used to find the optimal parameters (weights and biases) for a model by iteratively minimizing a cost function.

## **Project Goals**

* **Implement Gradient Descent from scratch**: Manually write the core logic of the algorithm to gain a deeper understanding of how it works.
* **Apply the algorithm to a real dataset**: Use the implemented function to find the best-fit line for a set of data points.
* **Compare results**: Verify the accuracy of the custom implementation by comparing its output to the results from **scikit-learn's** built-in `LinearRegression` model.

---

## **Repository Structure**

* `1_GD.ipynb`: Contains the manual implementation of the gradient descent algorithm using simple arrays for a straightforward demonstration.
* `2_Practice.ipynb`: Applies the same algorithm to a real-world dataset and includes a more robust implementation with a dynamic stopping condition.
* `test_scores.csv`: The dataset used in the `2_Practice.ipynb` notebook.

## **Analysis and Findings**

The core of this project is the `gradient_descent` function, which calculates the slope (`m`) and y-intercept (`b`) of a line that minimizes the mean squared error (cost) between predicted and actual values.

The final optimized values for the model parameters after running the algorithm on the `test_scores.csv` data are:

* **Slope (m)**: `1.0177`
* **Y-Intercept (b)**: `1.9151`

These values are nearly identical to the results from the `LinearRegression` model from `scikit-learn`, which confirms the correctness of the custom gradient descent implementation. The iterative process of reducing the cost function over many iterations is a powerful way to train machine learning models.