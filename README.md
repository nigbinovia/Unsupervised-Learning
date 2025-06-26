# Unsupervised-Learning

This project explores unsupervised learning by implementing the K-Means clustering algorithm. Unlike supervised methods that rely on labeled data, unsupervised learning discovers patterns and groupings in unlabeled datasets. K-Means clustering is used to partition data into clusters based on feature similarity, using centroid-based grouping.

## Code Development

To solve the clustering task, the `kmeans.py` program was developed. This program accepts a training dataset and a validation dataset, both in text file format. The training data is used to form clusters, while the validation data checks cluster accuracy.

The program includes several helper methods:
```
read_data(filename): this method reads and parses data from the specified file.

euclidean_distance(a, b): this method computes the Euclidean distance between two points.

update_centroids(clusters): this mehtod calculates updated centroid positions based on the current cluster assignments.

classify_validation_data(validation_data, centroids, cluster_labels): this method assigns validation data to the nearest centroid and compares predicted labels with true labels (if available).

kmeans(training_file, validation_file, k): this method executes the K-Means clustering process and returns classification accuracy.
```
The K-Means algorithm iteratively assigns points to the nearest centroid, updates centroids based on these assignments, and repeats the process until convergence. The validation step assesses how well the clusters align with any known labels.
