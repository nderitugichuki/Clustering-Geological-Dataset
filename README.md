# Clustering-Geological-Dataset
## **Overview**

This dataset contains measurements from geological formations, and it can be used for clustering purposes, specifically for unsupervised learning algorithms like K-means, DBSCAN, and hierarchical clustering. The main focus is on clustering based on properties such as bulk density, neutron porosity, gamma ray measurements, and sonic data.

The dataset is particularly useful for exploring clustering techniques in geological and petrophysical data to identify different subsurface rock types and their properties.

---

## **Dataset Information**

The dataset contains the following features:

- **RHOB**: Bulk density of the formation (g/cm³).
- **GR**: Gamma ray measurements (API units).
- **NPHI**: Neutron porosity (decimal form).
- **PEF**: Photoelectric factor (barns/electron).
- **DTC**: Sonic transit time (μs/ft).

---

## **Clustering Techniques Used**

1. **K-means Clustering**: 
   - The K-means algorithm is applied to partition the data into distinct clusters based on the geological measurements.
   - An elbow method was used to determine the optimal number of clusters (K), and clustering results were visualized using scatter plots of various feature combinations.

2. **Hierarchical Clustering**: 
   - Hierarchical clustering was used to create a dendrogram to visualize the hierarchical relationships between different clusters.
   - This method is useful when the user is interested in nested clusters or when the data doesn't have a clear "flat" structure.

---

## **Data Preprocessing**

The features were standardized using **StandardScaler** before applying the clustering algorithms. This ensures that each feature contributes equally to the clustering process, avoiding bias due to differing units or scales.

---

## **Visualization**

Several scatter plots were generated using Seaborn to visualize the clusters formed by different algorithms:

- **RHOB vs NPHI**: This plot helps identify different rock formations based on bulk density and porosity.
- **Other Feature Combinations**: Various combinations of features like **GR**, **PEF**, and **DTC** were also visualized to better understand the clustering results.

---

## **Usage**

This dataset and the accompanying code can be used to:

1. Understand and explore clustering techniques in unsupervised learning.
2. Visualize geological data to identify different subsurface formations.
3. Experiment with different clustering algorithms, such as K-means, DBSCAN, and hierarchical clustering.


---

## **Requirements**

- **Python 3.7+**
- **Libraries**:
  - pandas
  - numpy
  - scikit-learn
  - seaborn
  - matplotlib
  - scipy

To install the necessary dependencies, run:

```bash
pip install pandas numpy scikit-learn seaborn matplotlib scipy
```

---

## **License**

This dataset and the accompanying code are open for educational and research purposes. Please ensure proper attribution if used in academic or commercial projects.

---
