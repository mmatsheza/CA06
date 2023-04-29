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
