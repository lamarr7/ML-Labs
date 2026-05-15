# Lab 10: Support Vector Machines Classification

## Objective

To implement and evaluate a **Support Vector Machine (SVM)** model to classify flower species based on the Iris dataset, and to use **Grid Search** to optimize model hyperparameters.

---

## Workflow Stages

### 1. Exploratory Data Analysis (EDA)
* Used **Matplotlib** and **Seaborn** to visualize feature distributions.
* Created **Pairplots** to identify the separability of species and observed that **Setosa** was the most linearly separable.
* Generated a **KDE plot** to analyze the density relationship between sepal length and width for specific species.

### 2. Data Preparation
* Defined features ($X$) and the target species label ($y$).
* Split the dataset into a training set and a testing set using a **70/30 split** via `train_test_split`.

### 3. SVM Model Training
* Built an initial **Support Vector Classifier (SVC)** with default parameters.
* **Observation:** The model performed exceptionally well on the test set, especially in identifying the Setosa species.

### 4. Hyperparameter Tuning (Grid Search)
* Implemented `GridSearchCV` to find the optimal values for `C` and `gamma`.
* Created a **parameter grid** to test various exponential values for both hyperparameters to improve the decision boundary.

### 5. Model Evaluation
* Evaluated the final model using **Confusion Matrices** and **Classification Reports**.
* Achieved high precision and recall, demonstrating the effectiveness of SVMs for multivariate classification tasks.
