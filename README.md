# GMM
This project demonstrates how to generate synthetic data using Gaussian blobs, visualize it in 2D space, and apply Gaussian Mixture Model (GMM) clustering. The goal is to understand how probabilistic clustering works and how GMM can identify underlying data distributions with different variances.  
# Gaussian Mixture Model Clustering on Synthetic Data

## Overview
This project generates synthetic 2D data using Gaussian blobs and visualizes it.
A Gaussian Mixture Model (GMM) is then applied to cluster the data based on
probabilistic distributions.

The project is useful for understanding:
- Data generation with different cluster spreads
- Data visualization in 2D
- GMM-based clustering
- Comparison between true labels and predicted clusters

---

## Dataset
The dataset is generated using `make_blobs` from `scikit-learn`.

**Parameters used:**
- Number of samples: 500
- Number of centers: 3
- Cluster standard deviations: [1.0, 1.5, 0.8]
- Random state: 42

Each data point has two features, making it easy to visualize.

---

## Visualization
The blob data is visualized using a scatter plot:
- Each point represents a sample
- Colors represent the true cluster labels
- The plot helps verify cluster separation and spread

---

## Gaussian Mixture Model (GMM)
A Gaussian Mixture Model is trained with:
- 3 Gaussian components
- Full covariance matrices

The GMM:
- Learns the mean and covariance of each cluster
- Assigns each data point to the most probable Gaussian component

Cluster centers are visualized on top of the data.

---

## Requirements
- Python 3.x
- NumPy
- Matplotlib
- Scikit-learn

Install dependencies using:
```bash
pip install numpy matplotlib scikit-learn
