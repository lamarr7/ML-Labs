### Lab 7: Logistic Regression for Classification
**Objective:** To build and evaluate a binary classification model to predict user behavior (ad clicks) based on demographic and website usage metrics.

**Workflow Stages Implemented:**
* **Exploratory Data Analysis (EDA):** Performed multivariate analysis using **Seaborn Pairplots** and **Jointplots** to identify clusters and feature correlations.
* **Feature Selection:** Selected key numerical predictors: *Daily Time Spent on Site*, *Age*, *Area Income*, and *Daily Internet Usage*.
* **Model Pipeline:** * Split the dataset into training (70%) and testing (30%) sets using `train_test_split`.
    * Implemented and trained a **Logistic Regression** model using `scikit-learn`.
* **Model Optimization:** Addressed `ConvergenceWarnings` by increasing the maximum iterations (`max_iter=1000`) to ensure the optimization algorithm reached the global minimum.
* **Evaluation Metrics:** Achieved high performance with an **Accuracy of ~91%**, verified through a detailed **Classification Report** (Precision, Recall, and F1-Score).
