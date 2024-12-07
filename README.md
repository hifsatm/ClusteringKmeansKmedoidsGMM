# ClusteringKmeansKmedoidsGMM
The code aims to compare multiple clustering methods across diverse datasets and evaluate their effectiveness through comprehensive metrics and visualizations. It is designed for rigorous benchmarking of clustering techniques to identify the best-performing method for each dataset.


This extensive script provides a comprehensive implementation for clustering analysis using various methods, including K-Means, K-Medoids, GMM (Gaussian Mixture Models), and other clustering techniques like Agglomerative Clustering, DBSCAN, Spectral Clustering, OPTICS, BIRCH, and DIANA. The main features include:

Dataset Preprocessing:

Nine datasets are loaded, scaled using StandardScaler, and reduced to lower dimensions using PCA for noise reduction and visualization.
Datasets include common benchmarks like Banknote, Ionosphere, Sonar, Wine, Iris, etc.
Clustering Algorithms:

Each dataset is clustered using K-Means, K-Medoids, and GMM with predefined cluster counts.
Advanced methods like Agglomerative Clustering (Ward/Complete), DBSCAN, OPTICS, Spectral Clustering, BIRCH, and DIANA are also applied to specific datasets.

Evaluation Metrics:
Metrics such as Silhouette Score, Davies-Bouldin Index, Purity, Accuracy, Precision, Recall, F1-Score, and Execution Time are calculated to assess clustering quality.
A custom function aligns clustering labels with true labels using the Hungarian algorithm for more accurate metric evaluation.

Visualization:
Scatter plots display dataset distributions before and after clustering.
GMM-specific density plots visualize the density of each cluster along with overall data density.
Results Output:

Results are stored in a structured dictionary, converted into a DataFrame, and saved as CSV files for detailed analysis.
Additional files store metrics with or without label alignment.
Special Features:

Includes a dedicated function for DIANA clustering using hierarchical methods.
Incorporates density function plotting for each cluster under GMM.
