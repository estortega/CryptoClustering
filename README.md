# Crypto Clustering with K-Means and PCA

## 📈 Overview

This project applies unsupervised machine learning techniques—**K-Means Clustering** and **Principal Component Analysis (PCA)**—to cluster cryptocurrencies based on their market performance data. The goal is to group similar cryptocurrencies and visualize the clusters both before and after dimensionality reduction.

## 🧠 Skills Demonstrated

- Data Cleaning and Scaling with `StandardScaler`
- Clustering using `KMeans` from `scikit-learn`
- Dimensionality Reduction with `PCA`
- Data Visualization using `hvPlot`
- Elbow Method to determine optimal number of clusters

## 📁 Dataset

- File: `Resources/crypto_market_data.csv`
- Columns:  
  - `price_change_percentage_24h`  
  - `price_change_percentage_7d`  
  - `price_change_percentage_14d`  
  - `price_change_percentage_30d`  
  - `price_change_percentage_60d`  
  - `price_change_percentage_200d`  
  - `price_change_percentage_1y`  

## ⚙️ Technologies

- Python 3.x
- pandas
- scikit-learn
- hvPlot
- Jupyter Notebook

## 🧪 Project Workflow

1. **Load and Inspect Data**  
   Load CSV and check basic stats.

2. **Preprocessing**  
   Normalize market data using `StandardScaler`.

3. **Clustering (Raw Features)**  
   - Use K-Means clustering with Elbow Method to find optimal `k`.
   - Visualize clusters using a scatter plot of selected features.

4. **Clustering with PCA**  
   - Reduce dimensionality to 3 principal components.
   - Re-run K-Means clustering and compare clusters.

5. **Comparison and Evaluation**  
   - Visualize elbow curves for both raw and PCA data.
   - Contrast cluster visualization before and after PCA.

## 📊 Key Results

- PCA helped simplify the dataset while retaining most of the variance.
- Cluster shapes and separations became more apparent with fewer dimensions.
- Elbow method provided different optimal `k` values for raw and PCA-reduced data.

## 📝 Future Improvements

- Add more features like market cap, volume, or volatility.
- Use DBSCAN or Hierarchical clustering to compare methods.
- Deploy the results in a dashboard or web app for live crypto data.



