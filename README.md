# Clustering
Clustering is a machine learning and data analysis technique used to group similar objects or data points together into clusters, based on their inherent similarities and/or dissimilarities. The goal of clustering is to partition a dataset in such a way that objects within the same cluster are more similar to each other than to those in other clusters, while the clusters themselves are as distinct as possible.

Some common clustering algorithms include k-means, hierarchical clustering, DBSCAN (Density-Based Spatial Clustering of Applications with Noise), and Gaussian Mixture Models. Each algorithm has its own strengths, weaknesses, and assumptions, making it suitable for different types of data and problem domains.

### K-Means Clustering:

K-means is one of the most well-known clustering algorithms. It aims to partition data into K clusters, where K is a user-defined parameter. The algorithm starts by randomly selecting K initial cluster centroids. It then iteratively assigns each data point to the nearest centroid and recalculates the centroids based on the mean of the data points assigned to each cluster. This process continues until the centroids stabilize or a predefined number of iterations is reached. K-means is sensitive to the initial centroid placement and is best suited for spherical clusters.

### Hierarchical Clustering:

Hierarchical clustering builds a hierarchy of clusters by iteratively merging or splitting clusters. There are two main types: Agglomerative and Divisive. Agglomerative starts with each data point as its own cluster and then successively merges the closest clusters until a single cluster remains. Divisive clustering begins with all data points in one cluster and then splits clusters recursively until each data point is its own cluster. Hierarchical clustering results in a dendrogram, which is a tree-like structure showing the merging/splitting history.

### DBSCAN (Density-Based Spatial Clustering of Applications with Noise):

DBSCAN is based on the density of data points. It defines clusters as regions of high data point density separated by regions of lower density. It categorizes points as core points (dense regions), border points (close to core points), and noise points (isolated points). The algorithm starts with a core point and expands the cluster by connecting directly reachable core points. This algorithm is effective in identifying clusters of arbitrary shapes and handling noise.

## Implementation

- Importing the required Libraries and Reading the dataset
- Performing EDA (Exploratory Data Analysis) on the data
  Performing the following Types of Clustering:
- Hierarchical Clustering
  - Normalizing the data
  - Creating Dendrogram structure
  - Creating Hierarchical cluster
  - Draw inferences
- K-Means Clustering
  - Normalization of the data
  - Plotting Elbow Curve for K value
  - Creating K-Means cluster
  - Draw inferences
- DBSCAN Clustering
  - Normalizing the data
  - Plotting Elbow Curve for Epsilon (eps) value
  - Creating DBSCAN cluster
  - Draw inferences
- Comparison and Conclusions.

## Packages Used

- pandas
- numpy
- matplotlib.pyplot
- seaborn
- from sklearn.cluster import AgglomerativeClustering
- from sklearn.cluster import KMeans
- from sklearn.cluster import DBSCAN
- from sklearn.preprocessing import MinMaxScaler
- from scipy.cluster.hierarchy import linkage
- import scipy.cluster.hierarchy as sch
