## **Simple Linear Regression: Predicting House Prices**

**Objective:**

Your task is to build a **Linear Regression** model to predict the **price of a house** based on its size. This exercise will help you understand the relationship between variables and how to apply Linear Regression for real-world prediction tasks.

**Dataset:**

You will work with a dataset `data/housing.csv` containing the following columns:
- **price**: The price of the house in dollars.
- **area**: The size of the house in square feet.


Steps to Complete:

1. **Data Loading and Exploration**  
   - Visualize the relationship between **Size** and **Price** using a scatter plot.
   - Check for outliers, missing values, or anomalies in the dataset.

2. **Build a Linear Regression Model**  
   - Split the dataset into **training** and **test sets** (80% training, 20% testing).
   - Implement a **Simple Linear Regression** model using:
     - **Manual Calculation** (Optional): Derive the slope $m$ and intercept $b$ using the formulas for linear regression:
       $$
       m = \frac{\sum{(x_i - \bar{x})(y_i - \bar{y})}}{\sum{(x_i - \bar{x})^2}}, \quad b = \bar{y} - m\bar{x}
       $$
     - **Scikit-learn**: Use `LinearRegression` from `sklearn.linear_model` to fit the model.

3. **Model Evaluation**  
   - Predict the test set house prices using the model.
   - Evaluate the model’s performance using:
     - **Mean Absolute Error (MAE)**
     - **Mean Squared Error (MSE)**
     - **R² Score**
   - Interpret the slope ($m$) and intercept ($b$) of the linear equation.

4. **Visualization**  
   - Plot the **regression line** over the scatter plot of **area** vs. **price**.
   - Visualize the residuals (errors) between the actual and predicted house prices.

5. **Prediction**  
   - Use the trained model to predict the price of a house with a size of 1,000 square feet.
   - Discuss whether the prediction seems reasonable based on the dataset.


**Deliverables:**

- A Python script or Jupyter Notebook containing:
  - Data loading, preprocessing, and visualization.
  - Implementation of Simple Linear Regression.
  - Model evaluation and insights.
  - Predictions and their interpretation.
- A brief report discussing:
  - The relationship between **Size** and **Price**.
  - The limitations of using Linear Regression for this dataset.


**Useful Hints:**

- Use `numpy` for manual calculations and matrix operations.
- Use `pandas` for data manipulation and `matplotlib`/`seaborn` for visualizations.
- Experiment with data transformations (e.g., log or scaling) to improve results.