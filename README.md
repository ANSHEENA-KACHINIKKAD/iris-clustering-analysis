# Iris Dataset Clustering Analysis

## Overview

This project demonstrates the application of two fundamental clustering algorithms, KMeans and Hierarchical clustering, to the well-known Iris flower dataset. The goal is to identify natural groupings within the data based on its features (sepal length, sepal width, petal length, petal width) using unsupervised learning techniques.

## Key Components

1.  **Loading and Preprocessing:**
    * Loads the Iris dataset directly from the `sklearn` library.
    * Prepares the data for clustering by dropping the 'species' (target) column, as this is an unsupervised learning task.
    * Scales the features using `StandardScaler` to ensure that all features contribute equally to the distance calculations.

2.  **KMeans Clustering:**
    * Provides a brief description of how the KMeans algorithm works, highlighting its iterative process of assigning data points to clusters based on their proximity to centroids and then updating the centroids.
    * Explains the suitability of KMeans for the Iris dataset, considering its potential for well-defined, roughly spherical clusters.
    * Implements KMeans clustering using `sklearn.cluster.KMeans` with a specified number of clusters (typically 3, based on the known number of species, though this is treated as unknown during the clustering process).
    * Visualizes the resulting clusters in a 2D scatter plot after applying Principal Component Analysis (PCA) for dimensionality reduction. The cluster centroids are also visualized.

3.  **Hierarchical Clustering:**
    * Provides a brief description of how Hierarchical clustering works, outlining the agglomerative (bottom-up) approach of iteratively merging the closest clusters.
    * Explains the suitability of Hierarchical clustering for the Iris dataset, emphasizing its ability to reveal the hierarchical structure of the data and the fact that it doesn't require a pre-specified number of clusters.
    * Implements Agglomerative Hierarchical clustering using `scipy.cluster.hierarchy.linkage` and visualizes the clustering process using a dendrogram.
    * Extracts cluster assignments by cutting the dendrogram to obtain a specific number of clusters (again, typically 3 for comparison) and visualizes these clusters in a 2D scatter plot using PCA.

 ## Files

   * README.md
   * Iris-clustering-Analysis.ipynb

