# Clustering

Checks whether patients form natural groups without using the labels, and whether those groups match the labels.

## Notebooks

| Notebook | Data | Labels compared |
|---|---|---|
| `DS1_Clustering.ipynb` | DS1 processed training set (320 rows, 24 features) | CKD vs not CKD |
| `DS2_Clustering.ipynb` | DS2 processed training set (16,430 rows, 46 features including 2 engineered; 3,000-row sample where needed) | 5 risk levels |

Run the matching preprocessing notebook in `../Data_Preprocessing/` first.

## Methods

| Method | Idea | Setting |
|---|---|---|
| k-means | Groups around a centre | k from 2 to 8 |
| Hierarchical (Ward) | Tree of merges | Dendrogram, k from 2 to 8 |
| Gaussian mixture | Soft, oval groups | Diagonal covariance, k from 2 to 8 |
| DBSCAN | Dense regions, outliers as noise | min_samples 5, eps from 5-NN distance percentiles |

Clusters are compared with the labels using the Adjusted Rand index (ARI): 1 is a perfect match, 0 is random.

## Results

| | DS1 | DS2 |
|---|---|---|
| PCA components for 90% variance | 12 of 24 | 31 of 46 |
| Best silhouette | 0.24 | 0.04 |
| ARI, k-means | 0.42 | 0.00 |
| ARI, hierarchical | 0.95 | 0.00 |
| ARI, Gaussian mixture | 0.21 | 0.00 |
| ARI, DBSCAN (best eps) | 0.66 | 0.01 |
| ARI, hierarchical, without 0/1 features | 0.90 | 0.00 |
| ARI, hierarchical, continuous only | 0.21 | 0.00 |
| ARI, hierarchical, 0/1 features only | 0.74 | 0.00 |

## Summary

- DS1: hierarchical clustering recovers CKD vs not CKD almost exactly without seeing the labels
- DS2: no method finds groups, and no clusters match the risk levels
- Same methods on both datasets, so the lack of groups in DS2 comes from the data, not the method

## Limitations

- Euclidean distance on mixed 0/1 and numeric features
- 0/1 features are not scaled, so they count less in the distance
- Gaussian mixture assumes bell-shaped features
- Number of clusters chosen to match the labels (2 for DS1, 5 for DS2)
