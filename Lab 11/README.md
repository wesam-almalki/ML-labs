# Credit Card Customer Segmentation using K-Means

## Project Overview
This project applies K-Means Clustering to segment credit card customers based on their spending and payment behavior.  
The goal is to group similar customers together using unsupervised machine learning.

## Dataset
The dataset used is `CC_GENERAL.csv`, which contains credit card customer behavior data such as:

- Balance
- Purchases
- Cash Advance
- Credit Limit
- Payments
- Minimum Payments
- Tenure

Dataset source: Kaggle Credit Card Dataset

## Machine Learning Type
This is an **Unsupervised Learning** project because the dataset does not contain predefined target labels.  
The model discovers customer groups automatically based on feature similarities.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Steps
1. Import required libraries
2. Load the dataset
3. Explore the data
4. Clean the dataset
5. Handle missing values using mean imputation
6. Drop the `CUST_ID` column
7. Perform exploratory data analysis
8. Scale features using StandardScaler
9. Apply the Elbow Method
10. Calculate Silhouette Scores
11. Train the final K-Means model
12. Analyze customer clusters
13. Visualize clusters using PCA

## Data Preprocessing
The `CUST_ID` column was removed because it is only an identifier and does not represent customer behavior.

Missing values were handled using mean imputation.

Feature scaling was applied because K-Means is a distance-based algorithm, and features with larger values can dominate the clustering process.

## Model
The final model uses:

```python
KMeans(n_clusters=4, random_state=42, n_init=10)
