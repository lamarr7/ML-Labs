### Lab 8: K-Nearest Neighbors Classification
**Objective:** To implement a distance based classification model and optimize its predictive performance by finding the ideal number of neighbors through the Elbow Method.

**Workflow Stages Implemented:**
* **Exploratory Data Analysis (EDA):** Generated a **Seaborn Pairplot** with class hue to visualize feature overlap and identify separation boundaries between target classes.
* **Data Standardization:** Implemented **StandardScaler** to normalize feature magnitudes. This ensures the KNN distance calculation is not biased toward features with larger numerical ranges.
* **Model Training & Evaluation:** Built an initial KNN classifier with $K=1$. Evaluated performance using a **Confusion Matrix** and **Classification Report** (Precision, Recall, and F1-Score).
* **Hyperparameter Optimization:** Executed the **Elbow Method** by iterating through $K$ values (1–40). Plotted the **Error Rate** to visually identify the "elbow" where the model achieves the best balance between bias and variance.
* **Final Model Refinement:** Retrained the classifier using the optimal value ($K=30$), successfully increasing model accuracy from **75%** to **84%**.
