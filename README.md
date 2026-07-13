# Customer Segmentation Using RFM Analysis and Clustering

## Project Overview

This project applies RFM (Recency, Frequency, Monetary) analysis and clustering techniques to segment customers based on their purchasing behavior.

The objective is to identify distinct customer groups that can support targeted marketing strategies, customer retention efforts, and business decision-making.

## Dataset

The dataset contains online retail transactions, including:

- Invoice information
- Product details
- Quantities purchased
- Unit prices
- Customer identifiers
- Country information

## Methods Used

### Data Preparation
- Handling missing values
- Removing duplicate records
- Removing cancelled transactions
- Removing zero-priced transactions

### Feature Engineering
- RFM (Recency, Frequency, Monetary) Analysis
- Total spending calculation

### Feature Preparation
- Logarithmic transformation
- Feature scaling using StandardScaler

### Clustering Techniques
- K-Means Clustering
- Hierarchical Clustering
- DBSCAN

### Cluster Validation
- Elbow Method
- Silhouette Analysis

### Visualization
- PCA (Principal Component Analysis)
- t-SNE (t-Distributed Stochastic Neighbor Embedding)
- Dendrogram

## Results

K-Means clustering identified three customer segments:

- Loyal Customers
- Regular Customers
- Inactive Customers
