# Housing Data Clustering Analysis

This repository contains Python scripts for performing cluster analysis on housing data using different clustering algorithms.

## Overview

The scripts analyze housing data using two popular clustering techniques:
- K-means clustering (assignment_6.py)
- DBSCAN clustering (sankalpa_a7.py)

Both implementations include data preprocessing, algorithm application, and evaluation metrics to assess clustering performance.

## Files

### 1. assignment_6.py

K-means clustering implementation with the following features:
- Data standardization using `StandardScaler`
- K-means clustering with predefined cluster count (k=3)
- Performance evaluation metrics:
  - Inertia (Sum of squared distances)
  - Silhouette score
  - Davies-Bouldin index
- Cluster centers visualization

### 2. sankalpa_a7.py

DBSCAN (Density-Based Spatial Clustering of Applications with Noise) implementation with:
- Data standardization
- Dimensionality reduction using PCA
- DBSCAN clustering with customizable parameters (eps, min_samples)
- Identification of noise points
- Performance evaluation metrics:
  - Silhouette score
  - Davies-Bouldin index
- 2D visualization of clusters using matplotlib

## Requirements

These scripts require the following Python libraries:
- pandas
- numpy
- scikit-learn
- matplotlib

You can install the required packages using:

```bash
pip install pandas numpy scikit-learn matplotlib
```

## Usage

### K-means Clustering
```python
python assignment_6.py
```

### DBSCAN Clustering
```python
python sankalpa_a7.py
```

## Dataset

Both scripts are designed to work with a housing dataset (`housing.csv`). The dataset path can be modified in the scripts.

## Parameter Tuning

### K-means
You can experiment with different values of `k` (number of clusters) in assignment_6.py.

### DBSCAN
The DBSCAN implementation allows for customization of:
- `eps`: The maximum distance between two samples for one to be considered as in the neighborhood of the other
- `min_samples`: The number of samples in a neighborhood for a point to be considered as a core point
- `n_components`: Number of components for PCA dimension
