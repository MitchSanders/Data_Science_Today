# Clustering Analysis

Clustering is dividing into four major methods.

1. Prototype based methods such as K-Means and the multiple variations of centroid based spherical-shaped clustering, such as K-Mode, K-Means++, and Bisecting K-Means.
2. Hierarchial clustering such as agglomerative where you do not need to pick a number of centroids and visualization can be in dendrograms.
3. DBSCAN which is useful for non-globularized data and outliers using density of data.
4. Graph-based clustering such as spectral clustering which uses eigenvectors and similiarity matrixes.

## K-Means

### Intuition

Figure 1 shows k-means with a 2-dimensional feature vector \(each point has two dimensions, an x and a y\). In your applications, will probably be working with data that has a lot of features. In fact each data-point may be hundreds of dimensions. We can visualize clusters in up to 3 dimensions \(see figure 3\) but beyond that you have to rely on a more mathematical understanding.

![](/assets/import.png)

![](http://stanford.edu/~cpiech/cs221/img/kmeans3d.png)

Figure 3: KMeans in other dimensions. \(left\) K-means in 2d. \(right\) K-means in 3d. You have to imagine k-means in 4d.

