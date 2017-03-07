# Clustering Analysis

### What is Clustering? What’s it good for? How is it used?

##### 

##### What Clustering Is

Clustering is Unsupervised Learning. A machine learning approach that seeks to DISCOVER groupings within data. Seeking out similar and dissimilar data objects in a space where pre-determined groupings are not known.

##### 

##### What Clustering is Not

It is NOT predictive nor is it what’s normally termed as Classification where a certain subgroup of data objects have a known classification and can therefore be used to train data into a model to be used to predict classifications for data not classified yet. Instead clustering is finding natural groupings of data that hopefully lend to insights of clusters where meaning can be applied afterwards from human intelligence determining why one cluster is cohesive and dissimilar from another separate cluster.

##### 

##### How is Clustering used?

Clustering is useful for data that we cannot classify or identify. Perhaps no existing labels exist for attributes. Data useful for Clustering is usually not totally unstructured. Generally attributes are consistent of type with each attribute whether numerical, ordinal or nominal. Objects themselves should represent an event or dated grouping of data as usually depicted two-dimensional in rows, whereas the attributes would be the columns. An example might be a list of customers where each row is a unique customer and columns are attributes of each customer. Perhaps address, phone number, geography, purchases, demographics of income, status, sex, etc. What would not be known is how each of these customers group together. Clustering could be applied to find similar groups of customers for segmentation purposes to possibly target with specific products.

Clustering can also be used to group documents by grouping similar words or phrases to where scientific papers and fiction and non-fiction and poetry might all cluster into four separate groups. Further clustering can be applied to sub-divide clusters themselves.

Clustering also can be beneficial as a pre-processing technique to prepare data for further data mining techniques. Grouping data into self-determining natural clusters might allow predictive or deeper analytical work to be applied to individual clusters lending data to business intelligence not allowed when not pre-divided by a natural clustering technique.

##### 

##### Problems that can inhibit successful clustering

Certain techniques require an apriori knowledge of number clusters naturally with the data. Levels of clusters and deciding what best captures the intelligence needed can sometimes be a problem. Neither one cluster nor a cluster for every single data object is very valuable. Some middle ground is needed. For example, of a hundred customer it may be beneficial to select 2, 3, 4, … or even 10 clusters. Obviously 100 clusters reveals no useful abstraction, nor does grouping 100 customers into a single or maybe even only 2 clusters may be helpful. This discernment is left to the data scientist to interpret and decide upon.

Noisy data can be a problem, whereas, meaningless data that does not add value to a meaningful cluster only creates distraction for an algorithm to try to incorporate into a cluster and instead only makes the clusters less meaningful. Pre-processing from a domain expert and a data scientist can help eliminate non-useful noise.

Similar to noisy data, high dimensional data can be a problem. Hundreds or thousands of data attributes, even if relevant, can create processing problems. This problem comes into play especially with nominal data that has many possibilities. For example, sales orders shipped to hundreds or thousands of different localities, if each localities \(city or town\) is considered a unique point attribute for a single set of sales events, then these hundreds of possible locals incorporated in tens of thousands of orders can create very wide data sets that require high processing. A pre-processing of data to maybe state or country levels might allow clustering to be made in more practical processing requirements.

Incremental and order of data can also skew or make variations on what a clustering algorithm may find. This should be considered and tried experimentally to test for inconsistencies of clustering.

Interpret-ability can be another issue for clustering. Even with good strong clustering that meets quality testing, a person that understand the data usually still has to infer why each cluster congeals different than anther. An example might be a clustering of text surveys responses for customers based on works. Four or five clusters may be a good natural set of groupings but a human usually would have to interpret the each cluster by reading the survey text to see what the common theme might be, whether a complaint about product quality, or praise for service, or issues with delivery, etc. These are human interpreted and subjective but needed for business intelligence applicability.

### Clustering Methods

Clustering can be divided up several different ways. _Data Mining Concepts and Techniques_ authors do it as such:

> 1. ##### Basic Cluster Methods
>
>    1. ###### Partitioning methods, also known as Prototype methods
>
>       1. k-Means: Centroid Based
>       2. k-Medoids: Representative Object Based
>    2. ###### Hierarchical Methods
>
>       1. Agglomerative \(vs. Divisive\)
>       2. BIRCH
>       3. Chameleon
>       4. Probabilistic
>    3. ###### Density-based Methods
>
>       1. STING
>       2. CLIQUE
>    4. ###### Grid-based Methods
> 2. ##### Advanced Cluster Methods
>
>    1. ###### Probabilistic Model-Based Clustering
>    2. ###### Mixture Models – Univariate Gaussian
>    3. ###### Expectation-Maximization Algorithm – Fuzzy Clustering
>    4. ###### High-Dimensional Data Clustering
>
>       1. Subspace Search Methods
>          1. CLIQUE
>          2. PROCLUS
>       2. Correlation-based Methods - PCA
>          1. Bi-Clustering Methods
>          2. Optimization-based Methods
>          3. Enumeration Methods
>       3. Dimensionality Reduction and Spectral Clustering
>          1. Eigenvector Methods
>          2. Ng-Jordan-Weiss Algorithm
>    5. ###### Graph and Network Node Clustering
>
>       1. Bipartite Graph
>       2. Web Search Engines
>       3. Social Networks
> 3. ##### Other Clustering Aspects
>
>    1. ###### Evaluation of Clustering
>
>       1. Assessing Tendency
>       2. Determining Number of Clusters
>       3. Measuring Quality
>    2. ###### Clustering with Constraints – categories of constraints
>
>       1. On Instances, Clusters, and Similarity Measurements
>       2. Hard and Soft Constraints
>       3. Conflicting Constraints

### Clustering methods we will be studying in this book are:

1. Prototype based methods such as K-Means and the multiple variations of centroid based spherical-shaped clustering, such as K-Mode, K-Means++, and Bisecting K-Means.
2. Hierarchial clustering such as agglomerative where you do not need to pick a number of centroids and visualization can be in dendrograms.
3. DBSCAN which is useful for non-globularized data and outliers using density of data.
4. Graph-based clustering such as spectral clustering which uses eigenvectors and similiarity matrixes.

### K-Means

#### Intuition

Figure 1 shows k-means with a 2-dimensional feature vector \(each point has two dimensions, an x and a y\). In your applications, will probably be working with data that has a lot of features. In fact each data-point may be hundreds of dimensions. We can visualize clusters in up to 3 dimensions \(see figure 3\) but beyond that you have to rely on a more mathematical understanding.

![](/assets/two_centroid_clustering.png)

![](http://stanford.edu/~cpiech/cs221/img/kmeans3d.png)

Figure 3: KMeans in other dimensions. \(left\) K-means in 2d. \(right\) K-means in 3d. You have to imagine k-means in 4d.

