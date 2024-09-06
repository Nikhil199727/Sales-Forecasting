# Sales-Forecasting
## Introduction

In every business, sales performance is one of the most crucial indicators of success. Accurately understanding and forecasting sales patterns is key to making informed decisions about production, marketing, and inventory management. This project was designed to explore historical sales data, identify trends, and forecast future sales performance. By leveraging statistical techniques and machine learning models, we aimed to uncover insights about how sales fluctuate over time and predict sales for upcoming months.

The project involved reshaping the dataset, visualizing sales patterns, and using a linear regression model to predict future sales. The approach focused on understanding past performance, visualizing sales distribution, and predicting sales for the next six months.

---

## Dataset Description

The dataset used for this project contains historical sales records across various product categories, labeled as "keys." The data captures monthly sales for each product across different years. Below is a summary based on the `.info()` command output:

- **Rows**: Approximately 1,000
- **Variables**:
  - `keys`: Represents the different product categories.
  - `date` columns: Sales figures for different months and years.
  - `sales`: Represents the sales amount for each product.

### Dataset Quality

- **Missing Values**: Minimal missing values, as indicated by the `.isna().sum()` results.
- **Data Type**: Numerical data for sales and time-based data for dates, with a nominal scale for the `keys`.
- **Measurement Accuracy**: The data appears accurate, but it was necessary to reshape the dataset for time-series analysis.
- **Scale of Measurement**: The dataset contains **nominal** values (`keys`), and **numerical** values (`sales`).

---

## Objectives of the Project

### Content-Related Objectives
1. **Sales Trends**: Analyze and visualize sales trends over time for different product categories.
2. **Sales Distribution**: Understand the overall distribution of sales across different products and months.
3. **Future Sales Forecasting**: Predict future sales for the next six months using machine learning techniques.

### Statistical Objectives
1. **Regression Modeling**: Use linear regression to model the relationship between sales and time (month/year).
2. **Sales Forecasting**: Forecast sales for future months based on historical patterns.
3. **Evaluate Model Performance**: Assess the model’s performance using metrics like Mean Squared Error (MSE).

---

## Tools

- **Programming Language**: Python
- **Libraries Used**:
  - **Pandas**: For data manipulation and reshaping.
  - **Matplotlib & Seaborn**: For data visualization.
  - **Sklearn**: For model building and evaluation.
  - **Numpy**: For numerical computations.
  
---

## Insights

### 1. **Sales Trends Over Time**
The sales data was reshaped into a long format for better visualization and analysis. Using line plots, we explored the sales trends for each product over time. 
- **Observations**:
  - There were seasonal fluctuations in sales, with some products showing consistent growth while others experienced cyclical patterns.
  - Some keys showed significant peaks during specific months, indicating potential seasonality in demand.
  
**Plot 1: Sales Over Time for Each Key**
- **Purpose**: Visualize how sales change over time for different product categories.
- **Insight**: Products have varied sales trends, with some showing sharp increases during certain months.

![download](https://github.com/user-attachments/assets/372549c2-c8ba-458f-8de1-6b6e2cdcddb1)

### 2. **Sales Distribution**
A histogram was used to visualize the distribution of sales values across all products. The majority of sales were concentrated around specific ranges, with fewer outliers showing extremely high or low sales.
  
**Plot 2: Sales Distribution**
- **Purpose**: Understand the frequency of different sales values.
- **Insight**: Most products had moderate sales values, but there were occasional high-sales outliers that could represent top-performing items.

![download](https://github.com/user-attachments/assets/29c3bc1f-326d-4110-8e46-00f8f7b6a4d7)

### 3. **Linear Regression for Sales Prediction**
Linear regression was employed to forecast future sales based on the historical data. The model was trained using the sales data split into training and testing sets, and the Mean Squared Error (MSE) was calculated to evaluate the model’s performance.
  
- **Mean Squared Error**: The model yielded an MSE that reflected moderate predictive performance, meaning it could reasonably forecast sales based on time-based factors (month, year).
  
**Plot 3: Actual vs Predicted Sales**
- **Purpose**: Compare actual sales values with predicted sales to understand model performance.
- **Insight**: The scatterplot shows a moderate correlation between actual and predicted values, though some variability exists in the predictions.

![download](https://github.com/user-attachments/assets/0319f9b3-4a28-4a0f-a805-abaec5abf8c9)

### 4. **Future Sales Predictions**
Using the trained regression model, sales for the next six months were forecasted. This allows businesses to prepare inventory and marketing strategies in advance, ensuring stock availability and customer satisfaction.

**Plot 4: Future Sales Predictions**
- **Purpose**: Visualize forecasted sales for the next six months.
- **Insight**: Sales predictions for the next six months indicated a steady pattern, with minor fluctuations.

![download](https://github.com/user-attachments/assets/49930889-a0e6-459a-905f-9daf0424f888)

### 5. **Average Monthly Sales**
We aggregated the sales data to calculate the average sales per month. This analysis helped to identify which months consistently perform better in terms of sales, allowing for better resource allocation and marketing focus.
  
**Plot 5: Average Monthly Sales**
- **Purpose**: Identify which months see the highest average sales across all years.
- **Insight**: Sales were generally higher during specific months, likely due to seasonal trends, providing valuable input for strategic planning.

![download](https://github.com/user-attachments/assets/4ee73dfd-fbb9-462c-acd4-06216c7348d8)



## Recommendations and Future Analysis

### Recommendations:
1. **Inventory Management**: Use the sales forecasts to optimize inventory levels for the upcoming months, reducing overstock or stockouts.
2. **Seasonal Marketing**: Focus marketing efforts during peak months when sales typically rise, and use promotions to boost sales in slower months.
3. **Further Model Refinement**: Consider more advanced time-series forecasting models like ARIMA or SARIMAX to improve the accuracy of sales predictions.

### Future Analysis:
1. **Product-Level Forecasting**: Refine the model to provide product-specific sales forecasts, offering more granular insights into inventory needs.
2. **Customer Segmentation**: Use customer data (if available) to segment sales performance by region or customer demographics.
3. **External Factors**: Incorporate external factors such as economic indicators or weather data to enhance sales forecasts, particularly for seasonal products. 

This project provided valuable insights into historical sales patterns and offered a foundation for forecasting future sales, helping businesses make data-driven decisions and plan ahead.
