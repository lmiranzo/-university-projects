

# Graph-Based Clustering Techniques: Spectral Clustering in Marketing Campaigns

This repository contains Python scripts developed for my undergraduate thesis, titled Graph-Based Clustering Techniques: Spectral Clustering for Customer Segmentation in Marketing Campaigns. The primary goal of this project is to identify the most promising customer groups for targeted marketing efforts using graph-based clustering techniques, specifically spectral clustering.

### Context and Dataset
To apply the clustering algorithm developed in this project, we use the "Bank Marketing (with social/economic context)" dataset, available through the UCI Machine Learning Repository. This dataset contains real-world data from a Portuguese bank collected between May 2008 and June 2013, with 52,944 telemarketing interactions in total. Telemarketing, a common sales strategy, involves direct calls to potential customers to promote products or services. Here, we aim to identify customer clusters with the highest likelihood of subscribing to a banking product, optimizing the selection process for future marketing calls.

### Problem Statement
The objective of this project is to develop a clustering approach to identify high-probability customer segments based on customer data and behavioral metrics. Using machine learning, we transform this problem into a clustering task to uncover patterns in customer behavior, which can be strategically leveraged in telemarketing campaigns.

### Algorithms Implemented
To achieve robust clustering, we implement and compare the following algorithms:

Unnormalized Laplacian: A spectral clustering approach based on the unnormalized graph Laplacian.
Normalized Laplacian: A spectral clustering approach using the normalized Laplacian, implemented with both the Shi-Malik and Ng-Jordan-Weiss methods.
Classic k-means: Used as a baseline to evaluate the performance of spectral clustering techniques.

The models are evaluated using common clustering performance metrics:

#### Silhouette Score:
- Unnormalized Laplacian: 0.7448
- Normalized Laplacian (Shi-Malik): 0.7524
- Normalized Laplacian (Ng-Jordan-Weiss): 0.7629
- Classic k-means: 0.661
#### Calinski-Harabasz Index:
- Unnormalized Laplacian: 1586.403
- Normalized Laplacian (Shi-Malik): 1153.693
- Normalized Laplacian (Ng-Jordan-Weiss): 1878.095
- Classic k-means: 5592.151
#### Davies-Bouldin Index:
- Unnormalized Laplacian: 0.621
- Normalized Laplacian (Shi-Malik): 0.902
- Normalized Laplacian (Ng-Jordan-Weiss): 0.566
- Classic k-means: 0.487
