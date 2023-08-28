# Crypto_Clustering

## Introduction

The CryptoClustering project aims to predict the impact of 24-hour or 7-day price changes on cryptocurrencies using unsupervised learning techniques. By applying K-means clustering and Principal Component Analysis (PCA), this project investigates the relationships between cryptocurrency behaviors and various features.

## Getting Started

1. Create a new repository named "CryptoClustering".
2. Clone the repository to your local machine.
3. Upload the provided "crypto_market_data.csv" file to the repository.

## Files

The project includes the following files:

- `crypto_market_data.csv`: Contains the raw cryptocurrency market data.
- `crypto_clustering.ipynb`: Jupyter Notebook containing the Python code for the project.

## Dependencies

Ensure you have the following libraries installed:

- `pandas`: For data manipulation and analysis.
- `hvplot`: For interactive data visualization.
- `sklearn`: For machine learning and data preprocessing.

Install these dependencies using the following command:

pip install pandas hvplot scikit-learn

## Data Preparation

- Load the market data into a Pandas DataFrame.
- Normalize the data using `StandardScaler()` from scikit-learn.
- Create a DataFrame with the scaled data, indexed by coin ID.

## Finding the Optimal Number of Clusters

- Implement the elbow method to determine the best value for k (number of clusters).
- Visualize the elbow curve to identify the optimal k value.

## Clustering Cryptocurrencies

- Apply K-means clustering using the optimal k value to the original scaled data.
- Predict and assign cluster labels to each cryptocurrency.
- Visualize the clusters on a scatter plot using `hvPlot`.

## Optimizing Clusters with PCA

- Perform Principal Component Analysis (PCA) to reduce feature dimensions.
- Retrieve explained variance ratios for each principal component.
- Create a DataFrame with PCA data and coin IDs as the index.

## Re-evaluating Optimal Clusters with PCA

- Apply the elbow method to determine the best k value using PCA data.
- Compare the elbow curve with the original scaled data.

## Cluster Visualization and Comparison

- Visualize the elbow curves and cluster results side by side.
- Compare K-means clustering results with and without PCA.

## Conclusion

After a thorough analysis of cryptocurrency data using unsupervised learning techniques, this project provides insights into clustering patterns and relationships within the market. By leveraging K-means clustering and PCA, it becomes possible to uncover hidden trends and behavioral groups among cryptocurrencies.

For detailed implementation and results, refer to the `crypto_clustering.ipynb` notebook.

---

**Note:** This README provides an overview of the project. Refer to the Jupyter Notebook for full implementation details and analysis.
