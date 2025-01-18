## Fraud-Transaction-Detection

### **Objective**
Detect fraudulent transactions using machine learning classification models and data analysis techniques.

### **Dataset Overview**
- The dataset contains synthetic financial transaction records, including transaction amounts, balances, and fraud indicators.
- Key features:
  - `amount`: Transaction amount.
  - `oldbalanceOrg` and `newbalanceOrig`: Balance before and after transactions for the origin account.
  - `isFraud`: Binary label indicating whether a transaction is fraudulent.

### **Workflow**
1. **Data Preprocessing**:
   - Outliers were identified and removed using the Z-score method.
   - Irrelevant columns (`nameOrig`, `nameDest`) were dropped to simplify the analysis.

2. **Exploratory Data Analysis (EDA)**:
   - **Fraud Analysis**:
     - Class distribution for `isFraud` (fraud vs non-fraud).
   - **Feature Insights**:
     - Visualized transaction trends over time using scatter plots.
     - Correlation heatmap for numerical features to understand relationships.

3. **Feature Engineering**:
   - Applied Label Encoding to categorical variables (`type`).
   - Created a structured feature set for model training.

4. **Model Development**:
   - Models evaluated:
     - Logistic Regression
     - Naive Bayes
     - Decision Tree
     - K-Nearest Neighbors (KNN)
   - Cross-validation used for performance comparison.

5. **Results**:
   - Logistic Regression achieved high accuracy for fraud detection.
   - Visualization of model predictions vs true values.

### **Key Visualizations**
- Fraud and non-fraud transaction trends over time.
- Correlation heatmap of numerical features.
- Boxplots comparing fraud vs non-fraud transaction amounts.


### **Future Enhancements**
- Implement advanced ensemble models like Random Forest or Gradient Boosting.
- Evaluate feature selection methods for model optimization.
