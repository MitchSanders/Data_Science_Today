# Understanding Dimensions

#### 2-Dimensions

The image below shows a 2-dimensional feature vector \(each point has two dimensions, an x and a y\). 

We understand two dimensions as graphed on an x and y axis plane. X as a reminder is the horizontal axis, and Y is the vertical axis. The RED cluster below on an \(x,y\) coordinated plane would be at about \(1,6\) location. The BLUE cluster at \(9,10\). These x and y axis are consider two separate attributes or dimensions. 

![](/assets/2d.jpg)

#### 3-Dimensions

In your applications, you will probably be working with data that has a lot of features. In fact each data-point may be hundreds of dimensions. We can visualize clusters in up to 3 dimensions but beyond that you have to rely on a more mathematical understanding. 

![](/assets/3d.jpg)



#### 4-Dimensions

To help start comprehending 4-dimensions I recommend watching this great[ demonstration](https://youtu.be/N0WjV6MmCyM) by Carl Sagan and for a better understanding of dimensions in general and specifically how a 2-dimensional reality would work it is worth reading the short book "[Flatland](https://en.wikipedia.org/wiki/Flatland)" by Edwin A. Abbott written in 1884 .

![](/assets/4d.PNG)

#### N-Dimensions !

Mentally, we can't comprehend anything other than 3 dimensions except through mathematics. It is important though in Data Science and in Clustering to realize though at each and every added Attribute \(also called Dimensions or Features\), we are adding that much more complexity to the model. 

The sub-study of Dimensionality Reduction is a set of techniques to minimize dimensions for better problem solving. Much dimensionality reduction can be done though with simple data manipulation applying good understanding of the data itself. Eliminating noise and combining dimensions and even creating whole new dimensions not even in the data is a field of data science and skill set often call "[Feature Extraction](https://en.wikipedia.org/wiki/Feature_extraction)" and "[Feature Selection](https://en.wikipedia.org/wiki/Feature_selection)". In this context you will also hear references to the famous "Curse of Dimensionality" which many try to explain in simple terms, [but few do very well](http://stats.stackexchange.com/questions/169156/explain-curse-of-dimensionality-to-a-child). My intuitive explanation is simply that the more dimensions you have, the further the distance of data \(think gaseous molecules vs solid state molecules\) and thus the combinational relationships, and thus ironically the more data - horizontally, that is x values when flattened - the less value the data is able to exhibit. It is a paradox. The lesson is, reduce your data to the essentials if possible.



![](/assets/Houghton_EC85_Ab264_884f_-_Flatland,_cover.jpg)





