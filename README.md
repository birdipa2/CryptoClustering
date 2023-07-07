# Crypto Market Data Clustering and Dimensionality Reduction

This repository contains Python code for clustering and dimensionality reduction of cryptocurrency market data. The code uses K-means clustering and Principal Component Analysis (PCA) to group cryptocurrencies based on their price change percentages and reduce the dimensionality of the data for visualization.

## Requirements

To run the code, you'll need the following libraries and dependencies installed:

- pandas
- hvplot
- scikit-learn

## Usage

1. Clone the repository to your local machine.
2. Place the `crypto_market_data.csv` file in the `Resources` folder.
3. Run the `crypto_clustering.ipynb` script.

## Code Overview

The code performs the following steps:

1. Load the cryptocurrency market data from the CSV file.
2. Prepare and normalize the data using the `StandardScaler` from scikit-learn.
3. Find the best value for `k` using the original data by implementing the Elbow method.
4. Cluster the cryptocurrencies using K-means with the best value of `k` and visualize the results.
5. Apply Principal Component Analysis (PCA) to the scaled data to reduce the dimensionality.
6. Find the best value for `k` using the PCA data and visualize the Elbow curve.
7. Cluster the cryptocurrencies using K-means with the best value of `k` for the PCA data and visualize the results.
8. Compare the clustering results and visualizations obtained from the original data and PCA data.

## Results and Analysis

The code provides insights into the clustering of cryptocurrencies and the impact of dimensionality reduction. The visualizations and analysis help understand the different clusters formed and how they change with the use of fewer features.

The results show that using the original data with all available features leads to diverse clusters, but some data points may overlap, making it challenging to distinguish well-defined groups. However, by applying PCA and using three principal components, the clustering results become more distinct, with less overlap and more visually separable clusters.

These findings suggest that dimensionality reduction techniques like PCA can improve clustering results by focusing on the most informative features and reducing noise in the data.

## Conclusion

The code demonstrates how to cluster cryptocurrency market data using K-means and how dimensionality reduction techniques like PCA can optimize the clustering results. By reducing the number of features, PCA helps identify the most relevant information and creates more distinguishable clusters. This information can be valuable for understanding patterns and structures in the cryptocurrency market.

Feel free to explore and modify the code to further analyze and visualize the clustering and dimensionality reduction results.

