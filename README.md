## Crypto Clustering

**Description:**  
This repository contains the code for clustering cryptocurrencies using K-means and Principal Component Analysis (PCA). The analysis is performed on the `crypto_market_data.csv` dataset, which contains information about various cryptocurrencies.

**Files:**
- `Crypto_Clustering.ipynb`: Jupyter Notebook with Python code for clustering cryptocurrencies.
- `crypto_market_data.csv`: Dataset containing cryptocurrency market data.

**Requirements:**
- **Libraries Used:**
  - **pandas:** For data manipulation and analysis, especially loading and handling tabular data.
  - **matplotlib.pyplot:** For creating visualizations in Python.
  - **sklearn.cluster.KMeans:** For K-Means clustering.
  - **sklearn.decomposition.PCA:** For Principal Component Analysis (PCA).
  - **sklearn.preprocessing.StandardScaler:** For standardizing features.
  - **hvplot.pandas:** For interactive visualizations with Pandas DataFrames.

**Analysis Steps:**
1. **Find the Best Value for k:**
   - Implement the elbow method algorithm to find the best value for k.
   - Visualize inertia values to identify the optimal k.
   
2. **Cluster Cryptocurrencies with K-Means:**
   - Initialize K-means with the best k.
   - Fit the K-means model on original data.
   - Predict clusters for cryptocurrencies.
   - Visualize clusters using hvPlot scatter plot.
   
3. **Optimize Clusters with PCA:**
   - Create PCA model with `n_components=3`.
   - Reduce features to three principal components.
   - Calculate explained variance.
   - Create new DataFrame with PCA data.
   
4. **Find Best Value for k Using PCA:**
   - Implement elbow method with PCA data.
   - Visualize inertia values to find optimal k.
   
5. **Cluster Cryptocurrencies with K-Means Using PCA:**
   - Initialize K-means with optimal k from PCA.
   - Fit K-means model using PCA data.
   - Predict clusters based on PCA.
   - Visualize clusters using hvPlot scatter plot.
   
**Visualize and Compare Results:**
- Compare elbow curves and clusters from original data and PCA using composite plots.
- Analyze impact of using fewer features for K-means clustering.
