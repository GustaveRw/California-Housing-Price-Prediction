## California Housing Price Prediction

**Objective:** The goal of this project is to build a model for predicting median house values in California based on various metrics such as location, housing age, income, and population. The model should be capable of making predictions for any district in California.

**Analysis Steps:**

1. **Data Loading:** We start by loading the dataset from the "housing.csv" file and examining the first few rows to understand the data's structure.

2. **Handling Missing Values:** Missing values in the dataset are filled with the mean of their respective columns to ensure data completeness.

3. **Categorical Data Encoding:** Categorical data, specifically the "ocean_proximity" column, is converted into numerical values using one-hot encoding.

4. **Data Splitting:** The dataset is split into an 80% training dataset and a 20% test dataset to train and evaluate our models.

5. **Data Standardization:** Both training and test datasets are standardized to ensure consistent scales for numerical features.

6. **Linear Regression:** We apply Linear Regression to the training data to build a predictive model. The model is then used to predict house prices on the test dataset. The Root Mean Squared Error (RMSE) is calculated to assess its performance.

7. **Decision Tree Regression:** Similarly, Decision Tree Regression is applied to the training data and evaluated on the test data using RMSE.

8. **Random Forest Regression:** Random Forest Regression is employed on the training data, and predictions are made on the test data. RMSE is calculated to measure the model's accuracy.

9. **Bonus: Linear Regression with median_income:** We perform a linear regression using only the "median_income" feature as an independent variable. This provides insight into the relationship between income and housing prices. RMSE is calculated for evaluation.

10. **Model Visualization:** To assess how well the models fit the data, we visualize the fitted regression lines for both the training and test datasets.

**Conclusion:**

- Linear Regression, Decision Tree Regression, and Random Forest Regression models were built and evaluated for predicting housing prices.
- The Linear Regression model with the "median_income" feature yielded a reasonable RMSE, highlighting the strong correlation between income and housing prices.
- Visualization of the fitted models allowed us to visually inspect how well the models fit the data.

**Recommendations:**

- The Random Forest Regression model outperformed other models in terms of RMSE, making it a suitable choice for predicting housing prices.
- Further feature engineering and exploration could enhance model performance.
- Regular model updates and monitoring are advised to ensure accurate predictions as factors affecting housing prices change over time.

This project serves as a foundation for developing a housing price prediction system for California, which can be valuable for real estate professionals, homebuyers, and policymakers.
