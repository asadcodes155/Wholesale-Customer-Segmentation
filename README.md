# Wholesale Customer Segmentation using K-Means

## Overview

This project uses the **K-Means clustering algorithm** from scikit-learn to segment wholesale customers based on their purchasing behavior.

Unlike supervised learning, there are **no target labels**. The objective is to discover natural customer groups that exhibit similar buying patterns.

The resulting clusters can help businesses:

- Understand customer purchasing behavior
- Identify different customer segments
- Improve marketing strategies
- Personalize promotions
- Support business decision-making

---

## Dataset

**Dataset:** Wholesale Customers Dataset

Features used:

- Fresh
- Milk
- Grocery
- Frozen
- Detergents_Paper
- Delicassen

These features represent the annual spending of each customer in different product categories.

---

## Problem Statement

Given customers' annual spending across several product categories, identify groups of customers with similar purchasing habits using **K-Means Clustering**.

Since no customer labels are provided, this is an **unsupervised machine learning** problem.

---

## Technologies Used

- Python
- Pandas
- Matplotlib
- Scikit-learn

---

## Machine Learning Workflow

### 1. Load the Dataset

Read the customer dataset into a Pandas DataFrame.

### 2. Explore the Data

- Inspect the dataset
- Check data types
- Generate summary statistics

### 3. Feature Selection

Only purchasing-related columns are selected for clustering.

```python
Fresh
Milk
Grocery
Frozen
Detergents_Paper
Delicassen
```

### 4. Feature Scaling

The dataset is standardized using **StandardScaler**.

Since K-Means uses Euclidean distance, scaling ensures every feature contributes equally.

### 5. Determine the Optimal Number of Clusters

The **Elbow Method** is used by plotting inertia against different values of K.

### 6. Train the Model

A K-Means model is trained using the selected number of clusters.

### 7. Assign Cluster Labels

Each customer is assigned to one cluster.

### 8. Analyze the Clusters

Cluster averages are calculated to understand customer spending behavior.

### 9. Predict New Customers

The trained model can classify new customers into existing clusters.

---



## Concepts Learned

This project demonstrates the following machine learning concepts:

- Unsupervised Learning
- Clustering
- K-Means Algorithm
- Feature Scaling
- StandardScaler
- Elbow Method
- Inertia
- Cluster Centers
- Customer Segmentation
- Model Prediction

---

## Key Scikit-Learn Components

| Component | Purpose |
|-----------|---------|
| StandardScaler | Standardizes numerical features |
| KMeans | Groups similar customers into clusters |
| fit() | Learns cluster centers |
| labels_ | Returns the assigned cluster for each customer |
| cluster_centers_ | Returns the center of each cluster |
| predict() | Assigns new customers to a cluster |

---

## Results

The K-Means algorithm successfully groups customers into distinct purchasing segments.

Each cluster represents customers with similar spending habits across product categories, allowing businesses to better understand customer behavior.

---

## What I Learned

During this project I learned how to:

- Apply K-Means clustering using scikit-learn
- Preprocess data with StandardScaler
- Determine the optimal number of clusters using the Elbow Method
- Interpret cluster centers
- Analyze customer segments
- Predict the cluster of new customers
- Build a complete unsupervised machine learning workflow

---

## References

- Scikit-learn Documentation
- Wholesale Customers Dataset
