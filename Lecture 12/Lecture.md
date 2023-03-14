March 14th, 2023

Happy pie day!

Unsupervised Learning AKA Clustering: We are given only the samples- we do NOT know any labels. Clustering looks for similar samples.

![Clustering Diagram](images/clustering.png)

For clustering, we first must partition our data by some metric:
![partitions](images/partitions.png)

### K-Means Clustering

Given some dataset $\{x_1, x_2, \dots, x_n\}$, K-Means partitions the data into K clusters- each cluster has a cluster center, called a centroid.

![k-means clustering](images/k-means.png)

**Procedure**:
1. Randomly initialize the cluster centroids $\mu_1, \mu_2, \dots, \mu_k$
2. Repeat the following until no change in $\mu_k$:
	1. Classify N samples in terms of the nearest cluster centroid
	2. Re-compute the cluster centroid

