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



