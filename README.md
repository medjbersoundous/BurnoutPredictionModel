# Employee Burn Rate Prediction

This project was developed using **Google Colab** and contains a machine learning workflow aimed at predicting **employee Burn Rate**. The goal is to evaluate different regression algorithms and identify the best-performing model for accurate and reliable predictions.

## Dataset
The dataset used for this project can be found in this repository with the name: **`raw_data.csv`**.  
It includes information about employees, such as:
- Employee details (ID, Date of Joining)
- Gender and Company Type
- Work From Home setup
- Designation, Resource Allocation, Mental Fatigue Score
- Burn Rate (target variable)

## Project Steps
1. **Data Exploration & Cleaning**
   - Checked for missing values and duplicates
   - Created new features such as `TenureDays`
   - Handled missing data by dropping incomplete rows

2. **Data Preprocessing**
   - Encoded categorical variables using one-hot encoding
   - Scaled numerical features with `StandardScaler`

3. **Feature Analysis**
   - Correlation analysis to understand feature importance
   - Visualizations for distributions and relationships

4. **Model Training & Evaluation**
   - Models used: Linear Regression, Ridge, Lasso, Random Forest, Gradient Boosting
   - Evaluation metrics: R², RMSE, MAE, Cross-Validation
   - **Gradient Boosting achieved the best performance:**
     - **Test R² = 0.9266**
     - **RMSE = 0.0533**
     - **MAE = 0.0437**

5. **Model Interpretation**
   - Feature importance analysis with Random Forest
   - Residual analysis to ensure accuracy and unbiased predictions

## Results
- Gradient Boosting provided the most accurate predictions.
- The model can reliably estimate Burn Rate, useful for employee management and planning.

## Visualizations
- Feature distributions
- Correlation heatmaps
- Model comparison charts (R², RMSE, MAE)
- Predicted vs Actual plots and residual analysis

## How to Use
1. Open the notebook in **Google Colab**.
2. Ensure that **`raw_data.csv`** is present in the repository or Colab workspace.
3. Run all cells sequentially to reproduce the analysis.
4. Alternatively, you can clone the repository and run locally:
   ```bash
   git clone https://github.com/medjbersoundous/BurnoutPredictionModel.git
