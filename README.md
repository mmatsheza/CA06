# ML CA06 Customer Segmentation using K-Means Clustering

## Objective
The objective of this project is to perform customer segmentation using k-means clustering on a dataset of mall customers. This will help us identify underlying patterns in the data and understand customer behavior, which is essential for developing targeted marketing strategies.

## Data
The dataset contains information about mall customers, including their CustomerID, Genre, Age, Annual Income (in thousands of dollars), and Spending Score (1-100).

## Libraries Used
pandas
numpy
matplotlib
seaborn
sklearn

## Steps Followed
Data Loading and Exploration: Loaded the dataset into a pandas DataFrame and performed initial exploration using methods like head(), info(), and describe().

Prepare the Data for Clustering: Preprocessed the data by:
a. Scaling the features using StandardScaler
b. Selecting appropriate features for clustering (started with 'Annual Income (k$)' and 'Spending Score (1-100)')

Implement K-Means Clustering:
a. Imported the KMeans class from the sklearn.cluster module
b. Determined the optimal number of clusters using the Silhouette Method
c. Trained the KMeans model with the optimal number of clusters
d. Obtained the cluster assignments for each data point

Visualize and Analyze the Clusters: Created scatter plots of the selected features colored by cluster assignment. Performed the same analysis with different sets of features (e.g., 'Age' and 'Spending Score (1-100)') and compared the results.

## Results
The optimal number of clusters for 'Annual Income' and 'Spending Score' was determined to be 5.
The optimal number of clusters for 'Age' and 'Spending Score' was determined to be 2.
Scatter plots were created to visualize and analyze the clusters for both sets of features.

# Customer Segmentation using K-Means Clustering: Report
1. Introduction
The dataset used in this project contains information about 200 mall customers. The data includes the following attributes:

CustomerID
Genre
Age
Annual Income (in thousands of dollars)
Spending Score (1-100)
The main objective of this project is to perform customer segmentation using k-means clustering to identify underlying patterns in the data and understand customer behavior. This is essential for developing targeted marketing strategies.

2. Data Preprocessing and Feature Selection
During the data preprocessing phase, the following steps were taken:

Loaded the dataset into a Pandas DataFrame.
Explored the dataset using descriptive statistics and visualizations.
Selected appropriate features for clustering. Initially, 'Annual Income' and 'Spending Score' were selected. Later, 'Age' and 'Spending Score' were also considered.
Feature scaling was performed using the StandardScaler from scikit-learn to ensure that the features were on the same scale and that the clustering algorithm was not affected by the differences in units or magnitudes.

3. K-Means Clustering Implementation
The k-means clustering algorithm from scikit-learn was used to group the customers based on their selected features. To determine the optimal number of clusters, the Silhouette Method was employed. The Silhouette Coefficient, which ranges from -1 to 1, was calculated for various numbers of clusters. The number of clusters that resulted in the highest Silhouette Coefficient was considered the optimal number.

Based on the analysis, the optimal number of clusters for 'Annual Income' and 'Spending Score' was found to be 5, while the optimal number of clusters for 'Age' and 'Spending Score' was 2.

4. Cluster Visualization and Analysis
Scatter plots were created to visualize and analyze the clusters for both sets of features. The plots revealed distinct customer segments based on their spending patterns.

For 'Annual Income' and 'Spending Score', the five clusters can be characterized as:

Low income, low spending
Low income, high spending
Average income, average spending
High income, low spending
High income, high spending
For 'Age' and 'Spending Score', the two clusters can be described as:

Younger customers with higher spending scores
Older customers with lower spending scores
5. Insights and Recommendations
Based on the analysis, the following insights and recommendations can be provided:

Customers with high spending scores and low incomes can be targeted with promotions and discounts, as they are likely to be more price-sensitive.
High-income customers with high spending scores can be targeted with premium products and services.
Marketing campaigns can be tailored based on the age of the customers. Younger customers tend to have higher spending scores, so campaigns targeting them should focus on products and services that appeal to this demographic.
Overall, this project demonstrates the potential of k-means clustering to reveal useful insights into customer behavior and inform targeted marketing strategies.
