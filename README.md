# Calories_Burned_Prediction
Based on the metrics extracted from the notebook, here is a comparison of the models:

1. **XGBoost Regressor**:
   - **R² Score**: 0.9987
   - **MAE**: 1.55
   - **MSE**: 5.27
   - **RMSE**: 2.30

2. **Linear Regression**:
   - **R² Score**: 0.9656
   - **MAE**: 8.48
   - **MSE**: 138.12
   - **RMSE**: 11.75

3. **Decision Tree Regressor**:
   - **R² Score**: 0.9924
   - **MAE**: 3.50
   - **MSE**: 30.38
   - **RMSE**: 5.51

4. **Random Forest Regressor**:
   - **R² Score**: 0.9977
   - **MAE**: 1.80
   - **MSE**: 9.22
   - **RMSE**: 3.04

### - Best Model:

The **`XGBoost Regressor`** appears to be the best model among the ones compared. It has the highest R² score (0.9987), indicating that it explains the variance in the data better than the other models. Additionally, it has the lowest MAE (1.55), MSE (5.27), and RMSE (2.30), which suggests that its predictions are the most accurate and closest to the actual values.

The Random Forest Regressor also performed very well, but XGBoost slightly edges it out in terms of accuracy.


### - Other than XGBoost, the `Random Forest Regressor` is the next best model based on the metrics:

- **R² Score**: 0.9977 (very close to XGBoost)
- **MAE**: 1.80
- **MSE**: 9.22
- **RMSE**: 3.04

### Why Random Forest?

- **High R² Score**: It has a very high R² score, meaning it explains almost all the variance in the data.
- **Low Errors**: The MAE, MSE, and RMSE values are low, indicating that the predictions are accurate and have minimal deviation from the actual values.

This combination of high accuracy and low error metrics makes the Random Forest Regressor a strong choice, second only to XGBoost.


### - Between **`Linear Regression`** and the **`Decision Tree Regressor`**, the **`Decision Tree Regressor`** is the better model based on the following metrics:

### Decision Tree Regressor:
- **R² Score**: 0.9924
- **MAE**: 3.50
- **MSE**: 30.38
- **RMSE**: 5.51

### Linear Regression:
- **R² Score**: 0.9656
- **MAE**: 8.48
- **MSE**: 138.12
- **RMSE**: 11.75

### Why Decision Tree?

- **Higher R² Score**: The Decision Tree Regressor has a significantly higher R² score (0.9924 vs. 0.9656), meaning it explains more variance in the data.
- **Lower Errors**: The MAE, MSE, and RMSE are all much lower for the Decision Tree, indicating that its predictions are closer to the actual values compared to Linear Regression.

In summary, the Decision Tree Regressor outperforms Linear Regression in terms of both accuracy and error metrics, making it the better choice between the two.
