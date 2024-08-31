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

### Best Model:

The **XGBoost Regressor** appears to be the best model among the ones compared. It has the highest R² score (0.9987), indicating that it explains the variance in the data better than the other models. Additionally, it has the lowest MAE (1.55), MSE (5.27), and RMSE (2.30), which suggests that its predictions are the most accurate and closest to the actual values.

The Random Forest Regressor also performed very well, but XGBoost slightly edges it out in terms of accuracy.
