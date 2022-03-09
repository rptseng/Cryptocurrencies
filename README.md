# Cryptocurrencies
## Overview
Using an unsupervised machine learning model, we will be attempting to cluster various classes of cryptocurrencies currently on the trading market.

## Pre-processing and creating PCA Dimensions
First the data in crypto_data.csv is cleaned using Pandas to remove any currencies that are not actively trading or have null values. The get_dummies() method is then applied to create variables for the two text features, "Algorithm" and "ProofType".

The values were then scaled and the PCA algorithm was run to reduce the dimensions of the dataframe to three principal components.

## K-Means Clustering
An elbow curve was created to determine a cluster limit of k=4. Below is the 3D Scatter plot for cryptocurrencies by class across the three principal components.
![3d_scatter.png](https://github.com/rptseng/Cryptocurrencies/blob/main/Resources/3d_scatter.png)

2D Scatter plot created for TotalCoinSupply vs TotalCoinsMined, coloured by class.
![2d_scatter.png](https://github.com/rptseng/Cryptocurrencies/blob/main/Resources/2d_scatter.png)

