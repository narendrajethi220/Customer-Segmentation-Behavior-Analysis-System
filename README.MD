# Customer Segmentation & Behaviour Analysis using Unsupervised Learning

##  Project Overview

Businesses collect large amounts of customer data but often do not know how different customers behave.

This project applies unsupervised learning techniques to discover hidden customer patterns and create meaningful customer segments.

The objective is to group customer with similar characteristics and generate meaningful insights.

## Business Problem

A Mall company wants to understand its customer's better.

The company wants to identify:
- High value customers
- Low engagement customers
- Different customer behaviour patterns

Since customer group s are not predefined, an unsupervised learning approach is used.

## Dataset

Dataset contains customer demographic and spending information.

Features:

| CusteromID | Gender | Age | Annual Income(k-$) | Spending_Score (1-100)

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebool
- Unsupervised Learning

## Machine Learning Workflow

Raw -> Data Understanding -> Feature Selection -> Feature Scaling -> PCA for dimensionality reduction -> KMeans Clustering -> Cluster Analysis -> Business Interpretation

## Data Preprocessing

### Remove ClusterID

CustomerID is only an identifier and does not represent customer behaviour.

### Feature selection

Two experiments were performed

1. Using:
- Age
- Income
- Spending Score

2. Using:
- Gender
- Age
- Income
- Spending Score

The impact of demographc information was compared.

## Dimensionality Reduction

PCA was applied to reduce feature dimension and visualize customer distribution.

The original features were transformed into:

- PC1
- PC2

These components represents the maximum variance directions in the dataset.

## Clustering Models

### KMeans clustering

KMeans was used to divide customers into groups based on similarity.

The optimal number of clusters was selected using:
- Elbow Method
- Silhouette Score

## Model Evaluation 

Silhoutte Score was used to evaluate cluster separations.
It gives us a score evaluating how well a model separated unknown clusters.
Higher score indicates better deined clusters.

## Business Insights

Cluster 0:

Average Age: 48 years
Average Income: 60K
Average Spending Score: 32

Interpretation:

Older customer with moderate income but lower spending behaviour.

Cluster 2:

Average Age: 28 years
Average Income: 60k
Average Spending Score: 69

Interpretation:

Younger customers showing higher engagement and spending.

## Project Structure

Customer-Segmentation/

│

├── data/

│   └── customers.csv


├── notebooks/

│   └── customer_segmentation.ipynb


├── README.md


└── requirements.txt


## Future Improvements

- Add transaction history features
- Deploy segmenation dashboard using Streamlit
- Automate customer classification pipelin 
