Task 4: Binary Classification with Logistic Regression
Objective
To build a machine learning model that classifies tumors as Malignant or Benign using the Breast Cancer Wisconsin dataset.

Key Steps Taken
1. Data Preprocessing: Cleaned the dataset by removing irrelevant columns (id, Unnamed: 32) and encoding the categorical diagnosis into numerical format (M=1, B=0).
2. Feature Scaling: Applied StandardScaler to normalize the feature set, as Logistic Regression is sensitive to the scale of input variables.
3. Modeling: Trained a Logistic Regression model using Scikit-learn.
4. Evaluation Metrics:
Confusion Matrix: Visualized True Positives vs. False Positives.
Recall: Focused on high Recall since missing a Malignant case is high-risk.
ROC-AUC: Achieved an AUC score (typically >0.98 for this dataset), indicating excellent separation between classes.

The Sigmoid Function:
It maps any real-valued number into a value between 0 and 1, which we interpret as the probability of the tumor being Malignant.

Threshold Tuning
While the default threshold is 0.5, we explored how lowering the threshold (e.g., to 0.3) helps in reducing "False Negatives," which is critical in healthcare diagnostics.
