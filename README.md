# Cluster-flowers-into-Categories-using-KMeans
Using an unsupervised machine learning algorithm K-Means, we find clusters in the Iris dataset. Each entry of the Iris dataset specifies a flower's Sepal length, 
Sepal width, Petal length, and Petal width.

Here we use the **Elbow Method**, to find the optimum number of clusters.

![Elbow Method](https://user-images.githubusercontent.com/66300295/120334537-55b7cf00-c30e-11eb-98e5-af3ac2aa4a8c.png)

**Note**: The drop in the parameter WCSS(Within Cluster Sum Of Squares of distance from centroid) is negligibe after K = 3. Therefore K = 3 is the optimum number of clusters.

## Without Principal Component Analysis

Then we use the K-Means++ algorithm to find the clusters and avoid the random initialization trap.
Here's what it looks like when plotted against Sepal length and Sepal Width...

![Clustering_without_PCA](https://user-images.githubusercontent.com/66300295/120438701-53518580-c39f-11eb-9473-4cd80110d3bf.png)

## With Principal Component Analysis

In Clustering_with_PCA.ipynb we use Prinicipal Component analysis to reduce the dimensionality of the dataset and reduce the matrix of features to two principal components.
Here's what it looks like when plotted against Principal Component 1 and 2...

![Clustering_with_PCA](https://user-images.githubusercontent.com/66300295/120334632-6a946280-c30e-11eb-8fb4-299c6e68c915.png)

