# K-Means Clustering for Unsupervised Learning

This project is an introduction to **unsupervised learning** and the **K-Means clustering algorithm**. The goal is to group similar data points together without any predefined labels.

---

### **Project Objective**

* To understand the core concepts of unsupervised learning and clustering.
* To use the `scikit-learn` library to implement the **K-Means** algorithm.
* To learn the importance of data scaling and apply it using `MinMaxScaler`.
* To use the **elbow method** to determine the optimal number of clusters for the dataset.
* To visualize the resulting clusters.

---

### **Dataset**

The project uses the classic **Iris dataset**, which is loaded directly from `scikit-learn`. For this project, only the `petal length (cm)` and `petal width (cm)` features are used to cluster the data points.

---

### **Code and Analysis**

The code for this project is in the `1_Analysis.ipynb` Jupyter Notebook.
* **Data Scaling**: The numerical features were scaled using `MinMaxScaler` to ensure all features contribute equally to the distance calculations.
* **Elbow Method**: The sum of squared errors (SSE) was calculated for different numbers of clusters (K). A plot of K vs. SSE shows the "elbow" where the rate of decrease in SSE slows down, suggesting the optimal number of clusters.
* **Clustering**: A `KMeans` model was trained to cluster the data. The model's predictions assigned each data point to one of the clusters.
* **Visualization**: A scatter plot was created to visualize the different clusters and their centroids, providing a clear view of the groups the algorithm identified.

---

### **What I've Learned**

* **Unsupervised Learning**: I've learned the key difference between supervised and unsupervised learning—the latter works with unlabeled data to discover hidden patterns.
* **K-Means Algorithm**: I now understand the iterative process of K-Means: initializing centroids, assigning data points to the nearest centroid, and re-calculating centroids until convergence.
* **Preprocessing for Clustering**: Data scaling is crucial for distance-based algorithms like K-Means, and the elbow method is a practical way to find the right number of clusters for a dataset.