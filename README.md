# Customer Segmentation using K-Means Clustering

## Project Overview

This project demonstrates **customer segmentation** using **unsupervised machine learning** with the **K-Means clustering algorithm**.
The goal is to group customers based on features like **Age**, **Annual Income**, and **Spending Score**, which helps businesses identify distinct customer segments for targeted marketing and personalized strategies.

## Workflow

### 1. Data Preparation

* A sample dataset of 10 customers is created with the following features:

  * `CustomerID`
  * `Age`
  * `Annual Income (k$)`
  * `Spending Score (1-100)`
* Features for clustering are selected: `Age`, `Annual_Income(k$)`, and `Spending_Score(1-100)`.

### 2. Feature Scaling

* **StandardScaler** from `sklearn.preprocessing` is used to normalize the features.
* Scaling ensures all features contribute equally to the distance calculations in clustering.

### 3. K-Means Clustering

* The **K-Means algorithm** is applied with 3 clusters (`n_clusters=3`).
* Each customer is assigned a **cluster label** based on similarity across the features.
* `random_state` ensures reproducibility and `n_init=10` improves stability of clustering.

### 4. Results & Visualization

* The dataset now includes a `Cluster` column indicating each customer’s segment.
* A **scatter plot** visualizes customer clusters using **Annual Income** vs **Spending Score**, colored by cluster.
* This helps to easily identify high-spending, low-spending, and other customer groups.

## Techniques Used

* **Unsupervised Learning (Clustering)**
* **Feature Scaling (Standardization)**
* **K-Means Algorithm**
* **Data Visualization (Scatter Plot)**

## Libraries and Tools

| Library      | Purpose                              |
| ------------ | ------------------------------------ |
| Pandas       | Data manipulation and analysis       |
| Matplotlib   | Plotting and visualization           |
| Scikit-learn | Preprocessing and K-Means clustering |

## Results

* Customers are grouped into 3 distinct clusters based on spending behavior and income.
* The scatter plot clearly shows separation between clusters, enabling businesses to target each segment effectively.
