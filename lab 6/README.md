### Lab 6: Linear Regression Analysis
**Objective:** To implement a linear regression model to predict continuous numerical outcomes (Yearly Amount Spent) and evaluate model performance through residual analysis.

**Workflow Stages Implemented:**
* **Exploratory Data Analysis (EDA):** Utilized **Heatmaps** and **Pairplots** to identify strong linear correlations, specifically discovering that 'Length of Membership' is the most significant predictor of spending.
* **Data Preparation:** Separated the dataset into feature matrix ($X$) and target vector ($y$), followed by a **70/30 Train-Test Split** to ensure model generalizability.
* **Model Training:** Initialized and trained a **LinearRegression** model from Scikit-Learn to establish the mathematical relationship between customer behavior and revenue.
* **Residual Analysis:** Generated a **Residual Histogram** to confirm that the prediction errors were normally distributed, validating the assumptions of the linear model.
* **Performance Metrics:** Evaluated accuracy using **MAE**, **MSE**, and **RMSE**, providing a clear quantitative measure of the model's predictive error in dollar units.
