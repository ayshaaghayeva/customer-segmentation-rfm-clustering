# Customer Segmentation Project Notes

## Data Exploration and Cleaning

The dataset was explored to understand its structure, data types, summary statistics, and potential quality issues.

Data cleaning steps included:
- Handling missing values by removing records with missing CustomerID values
- Removing duplicate records
- Removing cancelled transactions
- Removing zero-priced transactions

## RFM Feature Engineering

Customer-level features were created using the **RFM (Recency, Frequency, Monetary)** model.

- **Recency:** Number of days since the customer's last purchase.
- **Frequency:** Number of purchases made by each customer.
- **Monetary:** Total spending amount by each customer.

These features summarize customer purchasing behavior and were used as inputs for clustering algorithms.

## Feature Preparation

The RFM features were examined for skewness before clustering.

A **logarithmic transformation** was applied to reduce skewness, and **StandardScaler** was used to standardize the features so that all variables contributed equally during clustering.

## Clustering Methods

Three clustering algorithms were evaluated:

- **K-Means Clustering**
- **Hierarchical Clustering**
- **DBSCAN**

K-Means and Hierarchical Clustering produced meaningful customer segments. DBSCAN identified outlier customers but generated less detailed customer segmentation.

## Selecting the Number of Clusters

The optimal number of clusters was determined using the **Elbow Method** and **Silhouette Analysis**.

Both methods indicated that **three clusters** provided a suitable balance between cluster compactness and separation. Therefore, three clusters were selected for the final K-Means model.

## Customer Segments

### Cluster 0: Inactive Customers
Customers with high recency, low purchase frequency, and low spending. These customers may require re-engagement strategies.

### Cluster 1: Loyal Customers
Customers with recent purchases, high purchase frequency, and high spending. These customers represent the most valuable customer segment.

### Cluster 2: Regular Customers
Customers with moderate purchasing behavior and represent potential loyal customers through targeted marketing efforts.

## Business Recommendations

- **Loyal Customers:** Use special programs and offers to retain high-value customers.
- **Regular Customers:** Encourage repeat purchases through personalized promotions and recommendations.
- **Inactive Customers:** Implement reactivation campaigns, discounts, and targeted communications to encourage future purchases.