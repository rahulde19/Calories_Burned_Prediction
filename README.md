# Model Performance Analysis

## Understanding the Metrics

**R² Score (Coefficient of Determination)**: Ranges from 0 to 1, where 1 means perfect prediction. It shows how much variance in your target variable is explained by the model.

**MAE (Mean Absolute Error)**: Average absolute difference between predictions and actual values. Lower is better.

**MSE (Mean Squared Error)**: Average of squared errors. Penalizes larger errors more heavily than MAE.

**RMSE (Root Mean Squared Error)**: Square root of MSE, in the same units as your target variable. More interpretable than MSE.

## Model-by-Model Analysis

### 1. **Linear Regression**
- **R² = 0.9656** (Good)
- **MAE = 8.48**
- **RMSE = 11.75**
- **Conclusion**: Decent but notably worse than other models. The higher errors suggest the relationship in your data may not be strictly linear, or there are non-linear patterns the model cannot capture.

### 2. **Decision Tree Regressor**
- **R² = 0.9925** (Very Good)
- **MAE = 3.50**
- **RMSE = 5.48**
- **Conclusion**: Strong performance. Can capture non-linear relationships well. However, decision trees are prone to overfitting, so validation on test data is crucial.

### 3. **Random Forest Regressor**
- **R² = 0.9978** (Excellent)
- **MAE = 1.79**
- **RMSE = 3.00**
- **Conclusion**: Excellent performance, nearly matching XGBoost. The ensemble approach reduces overfitting compared to a single decision tree while maintaining strong predictive power.

### 4. **XGBoost Regression** 
- **R² = 0.9987** (Excellent)
- **MAE = 1.55**
- **RMSE = 2.30**
- **Conclusion**: Exceptional performance with near-perfect predictions. The model explains 99.87% of the variance. On average, predictions are off by only 1.55 units.

## Key Insights

1. **Non-linear relationships exist**: Linear Regression significantly underperforms compared to tree-based models, indicating the data has non-linear patterns or complex feature interactions.

2. **Tree-based models excel**: XGBoost, Random Forest, and Decision Trees all perform very well, suggesting ensemble and tree-based methods are well-suited for this problem.

3. **Error magnitude**: The best models (XGBoost and Random Forest) have very small errors (MAE ~1.5-1.8 units), indicating highly accurate predictions.

4. **Potential overfitting concern**: The exceptionally high R² scores (>0.99) for XGBoost, Random Forest, and Decision Tree might indicate overfitting, especially for the Decision Tree. Thus, the evaluation is performed on a separate test set, not training data.

## Best Model: **XGBoost Regression**

**Winner**: XGBoost edges out the competition with:
- Highest R² score (0.9987)
- Lowest MAE (1.55)
- Lowest RMSE (2.30)

**Why XGBoost wins**:
- Best overall accuracy metrics
- Gradient boosting typically generalizes better than single decision trees
- Built-in regularization helps prevent overfitting compared to Decision Trees
- Only marginally better than Random Forest, but consistently superior across all metrics



**Final Conclusions**: **XGBoost** gives maximum accuracy, but **Random Forest** is also a strong backup option.
