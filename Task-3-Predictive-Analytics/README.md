# Predictive Analytics Using Historical Data

## Retail Sales Forecasting

### Overview

This project uses historical retail transaction data to build a predictive model for forecasting future sales trends.

The historical transaction data is cleaned, transformed into monthly sales data, and used to train a Linear Regression model. The model is evaluated on unseen test data and then used to forecast sales for the next five months.

## Objectives

- Clean and preprocess historical retail data.
- Analyze historical monthly sales trends.
- Build a predictive model for sales forecasting.
- Evaluate model performance using MAE and R².
- Forecast future sales based on historical trends.
- Visualize historical, predicted, and future sales.

## Dataset

The project uses the **Online Retail II Dataset**, containing historical retail transaction records from two periods:

- Year 2009–2010
- Year 2010–2011

### Dataset Attributes

- **Invoice** – Transaction identifier
- **StockCode** – Product identifier
- **Description** – Product description
- **Quantity** – Number of products purchased
- **InvoiceDate** – Date and time of the transaction
- **Price** – Unit price of the product
- **Customer ID** – Customer identifier
- **Country** – Customer's country

## Data Cleaning and Preprocessing

The historical transaction data was prepared by:

- Removing duplicate records.
- Checking for missing values.
- Removing records with missing values in required forecasting fields.
- Calculating sales using Quantity × Price.
- Converting InvoiceDate into datetime format.
- Removing transactions with non-positive quantities.
- Removing transactions with non-positive prices.

## Monthly Sales Analysis

The cleaned transaction data was aggregated by month to create a historical monthly sales dataset.

A time index was then created to represent the chronological sequence of the monthly observations.

The historical monthly sales trend was visualized before building the predictive model.

## Predictive Model

**Linear Regression** was used to learn the relationship between the time index and historical monthly sales.

The monthly sales data was divided chronologically into:

- **80% Training Data**
- **20% Testing Data**

The training data was used to build the model, while the testing data was used to evaluate its predictions.

## Model Evaluation

The model was evaluated using two metrics:

- **Mean Absolute Error (MAE)** – Measures the average absolute difference between actual and predicted sales.
- **R² Score** – Measures how well the model explains the variation in the sales data.

The model's predictions were compared with the actual sales values from the test period.

## Actual vs Predicted Sales

An actual-versus-predicted sales visualization was created to compare the model's predictions with the actual sales during the testing period.

## Future Sales Forecast

The trained Linear Regression model was used to forecast sales for the **next five months** based on the historical sales trend.

The forecast covers:

- January 2012
- February 2012
- March 2012
- April 2012
- May 2012

The predicted future sales were also visualized to show the projected sales trend.

## Project Workflow

1. Import the historical retail datasets.
2. Combine the two dataset sheets.
3. Clean and preprocess the transaction data.
4. Calculate sales amounts.
5. Convert transaction dates into datetime format.
6. Filter valid sales records.
7. Aggregate sales by month.
8. Visualize the historical sales trend.
9. Create a time index.
10. Split the data chronologically into training and testing sets.
11. Build a Linear Regression model.
12. Evaluate the model using MAE and R².
13. Compare actual and predicted sales.
14. Forecast sales for the next five months.
15. Visualize the future sales forecast.

## Visualizations

The project includes:

- Historical Monthly Sales Trend
- Actual vs Predicted Sales
- Future Sales Forecast

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

