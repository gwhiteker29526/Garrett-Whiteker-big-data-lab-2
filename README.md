# Garrett-Whiteker-big-data-lab-2
# Clustering Analysis Lab: K-Means vs K-Medoids (Wine Dataset)

## Purpose of the Lab
The purpose of this lab was to explore clustering techniques using the Wine Dataset from sklearn. The goal was to apply and compare two unsupervised learning algorithms, K-Means and K-Medoids, to better understand how data can be grouped without labeled outputs. Additionally, this lab focused on evaluating clustering performance using metrics such as Silhouette Score and Adjusted Rand Index (ARI), as well as visualizing the structure of the clusters.

---

## Key Insights and Observations

- **K-Means Results:**
  - Produced well-defined and compact clusters.
  - Achieved a higher Silhouette Score, indicating better separation between clusters.
  - Clusters appeared more spherical due to the use of centroids (means).

- **K-Medoids Results:**
  - Was more robust to noise and outliers since it uses actual data points as cluster centers.
  - Produced slightly different cluster shapes and positions compared to K-Means.
  - In some cases, the Adjusted Rand Index (ARI) was comparable, showing similar alignment with true labels.

- **Comparison:**
  - K-Means performed better in terms of overall cluster separation and efficiency.
  - K-Medoids provided more stable clustering when considering potential outliers.
  - Visualization showed that K-Means clusters were more evenly distributed, while K-Medoids clusters were slightly less uniform.

---

## Challenges and Decisions

One of the main challenges faced during this lab was setting up the Python environment in VS Code. Initially, the Jupyter Notebook was connected to a SQL kernel instead of a Python kernel, which prevented running the code. Additionally, there was an issue with activating the virtual environment due to PowerShell script execution restrictions. This required adjusting the execution policy and properly selecting the correct Python interpreter.

Another important decision was standardizing the dataset using z-score normalization. This step was necessary because clustering algorithms rely on distance calculations, and inconsistent feature scales could negatively impact the results.

---

## Conclusion

This lab demonstrated how different clustering algorithms can produce varying results depending on their underlying approach. K-Means proved to be efficient and effective for well-separated data, while K-Medoids offered advantages in handling noise and outliers. Overall, both methods provided valuable insights into the structure of the dataset and highlighted the importance of preprocessing and evaluation in clustering tasks.
