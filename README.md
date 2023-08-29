# NetworkAnalysis
This project employs machine learning to cluster nodes in complex networks, using local properties to reveal shared structural traits. It aims to uncover patterns for applications like marketing and community detection, distinguishing from global community detection methods.

1.Data preparation and preprocessing:

Data for the social network Facebook has been loaded from the specified file.
A chart was created from the data using networkx.
All orphaned nodes (nodes without connectivity) have been removed from the diagram.
Local features such as node grade, closeness centrality, and betweenness centrality were extracted from the chart.
We created feature data by joining the extracted features into a dataframe and standardizing.

2.Elbow method:
Determining the optimal number of clusters

We used the elbow method to determine the optimal number of clusters.
This method runs the K-means clustering algorithm for different k values (ranging from 2 to 10).
For each value of k, inertia, Silhouette score, Calinski-Harabasz score, and Davis-Bouldin score were calculated.
Results were graphed to visualize the relationship between evaluation metrics and number of clusters.
An 'elbow' point on the inertia curve was used to determine the optimal number of clusters. In this case, the optimal k value was found to be {optimal_k}.

3.Cluster analysis with optimal number of clusters
The K-means clustering algorithm was applied again, this time using the optimal number of clusters.
A cluster label was assigned to each node based on the clustering results.
Evaluation measures (Silhouette score, Calinski-Harabasz score, and Davies-Bouldin score) were calculated for the clustering results.
Evaluation metrics provide insight into the quality and performance of clustering algorithms. 


4.Results and visualization:
The optimal number of clusters (k) was determined to be {optimal_k}.
Evaluation metrics:

Optimal Number of Clusters (k): 10
Silhouette Score: 0.5115007050294721
Calinski-Harabasz Score: 4641.7998517523765
Davies-Bouldin Score: 0.5747455700201132

A graphical representation of the social network Facebook is graphed and coloured according to the cluster to which each node is assigned.
This graph visually represents the clustering results and allows a deeper understanding of the community structure within the network. 

<img width="499" alt="image" src="https://github.com/avani-potl/NetworkAnalysis/assets/137739877/407d77d1-6f14-453a-b703-92ce08bd3ca5">

<img width="496" alt="image" src="https://github.com/avani-potl/NetworkAnalysis/assets/137739877/2d7c97ac-1606-47a1-8adf-42fe29511fac">

<img width="489" alt="image" src="https://github.com/avani-potl/NetworkAnalysis/assets/137739877/6ee8d5dc-66b2-4cc7-b683-6793f704a2fe">

<img width="511" alt="image" src="https://github.com/avani-potl/NetworkAnalysis/assets/137739877/79c1f54e-266f-4ac4-a268-13f56cbcaa9b">





