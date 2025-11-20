# US Arrests Pattern Analysis (Capstone Project) 🇺🇸

This project applies **Unsupervised Machine Learning** techniques to the `UsArrests` dataset to identify clusters of US states with similar crime profiles.

## 📊 Project Overview
**Context:** Final Capstone Project for the Stellenbosch University / HyperionDev Data Science Bootcamp.
**Goal:** To explore relationships between crime rates (Murder, Assault, Rape) and Urban Population, and to categorize states into distinct clusters for policy or safety analysis.

## 🛠️ Technologies & Algorithms
* **Python 3** (Jupyter Notebook)
* **Pandas & Numpy:** Data manipulation.
* **Seaborn & Matplotlib:** Data visualization (Correlation heatmaps, Dendrograms).
* **Scikit-Learn:**
    * **PCA (Principal Component Analysis):** For dimensionality reduction.
    * **K-Means Clustering:** For partitioning states into groups.
    * **Agglomerative Clustering:** For hierarchical grouping.

## 🔎 Key Analysis Steps
1.  **Exploratory Data Analysis (EDA):**
    * Analyzed statistical properties of the dataset.
    * Visualized feature distributions and correlations (e.g., correlation between Murder and Assault).
2.  **Data Preprocessing:**
    * Standardized data using `StandardScaler` to ensure equal weighting for PCA (since variance differs significantly between features).
3.  **Principal Component Analysis (PCA):**
    * Reduced dimensions to identify the primary drivers of variance in the data.
    * Visualized the "Biplot" to see how different crimes contribute to the principal components.
4.  **Cluster Analysis:**
    * Utilized **Dendrograms** to determine the optimal number of clusters.
    * Applied **K-Means** and **Agglomerative Clustering** to group states into safety categories (e.g., "High Danger", "Safe Urban", "Rural Safe").

## 📈 Findings
* The analysis successfully grouped states based on crime severity.
* PCA revealed that violent crimes (Murder, Assault, Rape) are highly correlated, while Urban Population forms a distinct, separate component of variance.

## 🚀 How to Run
1. Ensure `UsArrests.csv` is in the same directory as the notebook.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
