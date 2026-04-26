# Lab 9: Decision Trees and Random Forest Classification

## Objective
To compare the performance of a single **Decision Tree** against a **Random Forest** ensemble model in predicting loan repayments based on lending data.

---

## Workflow Stages

### 1. Exploratory Data Analysis (EDA)
* Used **Matplotlib** and **Seaborn** to visualize FICO scores and interest rates.
* Created **Countplots** and **Jointplots** to analyze the relationship between loan purpose and the likelihood of being "not fully paid."

### 2. Categorical Data Handling
* Identified the `purpose` column as a categorical feature.
* Applied **One-Hot Encoding** using `pd.get_dummies` to transform text categories into numerical binary columns for model compatibility.

### 3. Decision Tree Model
* Built an initial **Decision Tree Classifier**.
* **Observation:** The model showed decent recall for the minority class (not fully paid), but was less stable overall.

### 4. Random Forest Model
* Implemented a **Random Forest Classifier** with `n_estimators=600`.
* **Observation:** The ensemble model significantly improved overall **Accuracy** to **85%** but struggled with recall for the minority class compared to the single tree.

### 5. Final Evaluation & Comparison
* Evaluated both models using **Confusion Matrices** and **Classification Reports**.
* **Conclusion:** While Random Forest provided higher stability and precision, the Decision Tree was more effective at identifying risky borrowers (Recall), demonstrating the trade-off between accuracy and class sensitivity in imbalanced datasets.
