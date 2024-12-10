# CryptoClustering

## Overview
This project demonstrates the application of machine learning techniques—K-means clustering and Principal Component Analysis (PCA)—to segment cryptocurrencies based on their price behavior. By analyzing percentage changes over various timeframes, this project identifies meaningful patterns and groups in the cryptocurrency market.

## Purpose

**The project aims to:** 

#### 1. Cluster Cryptocurrencies: Group cryptocurrencies based on similarities in their price changes.
#### 2. Optimize Clustering: Use the Elbow Method to determine the optimal number of clusters (k).
#### 3. Simplify with PCA: Reduce the dimensions of the data using PCA, retaining most of its variance for easier clustering and interpretation.
#### 4. Visualize Results: Compare clustering results with and without PCA to analyze the impact of dimensionality reduction.

## Process

**1. Data Preprocessing**
- The data consists of percentage changes in cryptocurrency prices over various time periods.
- StandardScaler was used to normalize the data for uniformity and improved clustering performance.
  
**2. Optimal k Selection**
- The Elbow Method was applied to determine the best number of clusters (k) by analyzing inertia (the sum of squared distances to centroids).
- This was done for both the original data and the PCA-transformed data.
  
**3. Clustering**
- K-means clustering grouped cryptocurrencies into clusters based on the normalized data.
- Clustering was performed separately for:
    - The original scaled data.
    - The PCA-transformed data.

**4. PCA Transformation**
- PCA reduced the dataset to three components, retaining ~90% of the variance.
- Clustering on PCA-transformed data provided a simplified view of the groups.

**5. Visualization**
- Elbow Curves: Compared the optimal k-values for original and PCA data.
- Cluster Plots: Visualized cluster assignments for original and PCA data.

## Results

**Key Findings**

**1. Elbow Curve Analysis**
- The optimal k-value for both the original and PCA-transformed data was consistent (e.g., k=3 or k=4).
Clustering:

**2. Clustering:** 
- Clustering on PCA-transformed data produced results similar to the original data but with reduced noise and improved interpretability.

**3. Impact of PCA:**
- PCA simplified the data while preserving meaningful variance, making clusters more distinct and easier to analyze.
  

## Visualization

**1. Elbow Curves**
- Compared inertia values for different k-values in the original and PCA-transformed datasets.

**2. Cluster Plots**
- Original Data: Clusters based on raw features.
- PCA Data: Clusters based on principal components (PC1 and PC2).
  
  
## Conclusion 

**This project highlights the power of PCA in reducing dimensionality while maintaining clustering quality. It demonstrates that:**

- K-means clustering effectively segments cryptocurrencies based on their price behavior.
- PCA provides a simpler, more interpretable clustering framework without compromising on key insights.


## Getting Started and References 

**How to Run**
- Clone the repository.
- Install required libraries: pip install -r requirements.txt.
- Run the Jupyter Notebook to execute the analysis and view visualizations.


**Technologies Used**
- Python: Data processing and analysis.
- Pandas: Data manipulation.
- Scikit-learn: Machine learning algorithms (K-means, PCA).
- hvPlot: Interactive plots for enhanced visualization.


**References**

- ChatGPT and Xpert Learning Assistant were used for README outline and format, and troubleshooting errors for this project assignment.

- OpenAI. (December, 2024). ChatGPT (GPT-4) [Large language model]. https://chat.openai.com/ Xpert Learning Assistant was used for troubleshooting errors for this project assignment.

- Xpert Learning Assistant. (2024). Retrieved from https://bootcampspot.instructure.com/
