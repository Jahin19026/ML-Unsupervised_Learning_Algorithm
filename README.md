**<span style="color: purple; font-size: 30px;">Breast Cancer Clustering Using K-Means</span>**

## Project Overview
This project applies **unsupervised machine learning** techniques to the Breast Cancer dataset in order to identify natural groupings of patients based on their cell characteristics.  
Since the dataset does not include diagnostic labels (Malignant/Benign), **K-Means clustering** is used to divide patients into distinct clusters, which can later be interpreted as potential cancerous or non-cancerous groups.

## Objectives
- Perform data preprocessing (handling unimportant features, scaling features).
- Apply **K-Means clustering** to group patients.
- Evaluate clustering quality using **Silhouette Score**, **Davies-Bouldin Index**, and **Calinski-Harabasz Score**.
- Analyze feature patterns within each cluster to interpret which cluster may correspond to malignant vs benign tumors.

## Key Steps
1. **Data Preprocessing**  
   - Removed non-numeric columns (like ID).  
   - Standardized features using `StandardScaler`.

2. **Clustering**  
   - Applied K-Means with `k=2` clusters.  
   - Added cluster labels to the dataset.

3. **Evaluation**  
   - Measured clustering quality using unsupervised metrics.  
   - Compared feature means across clusters for interpretation.

## Insights
- K-Means successfully grouped patients into 2 clusters.  
- Evaluation metrics help determine how well-defined the clusters are.  
- Feature averages per cluster can be used to hypothesize which group might represent malignant vs benign tumors.

## Technologies Used
- **Python**
- **Pandas, NumPy** for data handling
- **Scikit-learn** for clustering and evaluation
- **Matplotlib/Seaborn** for visualization
