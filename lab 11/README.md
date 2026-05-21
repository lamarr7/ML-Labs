# Lab 11: K-Means Clustering

## Objective

To implement and evaluate a K-Means Clustering model to segment credit card customers based on the CC_GENERAL dataset, and to use the Elbow Method and Silhouette Score to optimize model parameters.

---

## Workflow Stages

### 1. Exploratory Data Analysis (EDA)
* Used **Matplotlib** and **Seaborn** to visualize feature distributions.
* Created **Histograms** and **Scatter Plots** to look for correlations, trends, and clusters within the dataset features.
* Generated a **Correlation Heatmap** to analyze the linear relationships between all numerical features.

### 2. Data Preparation
* Defined the feature matrix ($X$).
* Handled missing values using **mean imputation** via `fillna()` to ensure data integrity.
* Scaled the data features using **StandardScaler** to normalize the ranges before model training.

### 3. K-Means Clustering Model Training
* Built an initial **KMeans** model with default parameters.
* **Observation:** The model effectively grouped patterns in the dataset, clearly differentiating unique behavioral segments across features.

### 4. Hyperparameter Tuning / Evaluation
* Implemented the **Elbow Method** and **Silhouette Score** loops to find the optimal values for `n_clusters`.
* Utilized **Principal Component Analysis (PCA)** to reduce dimensions into two components for clear 2D visualization of the final model boundaries.
