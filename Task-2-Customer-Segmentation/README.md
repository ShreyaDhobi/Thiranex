# Customer Segmentation

## Overview

This project focuses on segmenting customers based on their purchasing behavior using historical retail transaction data.

Customer-level features were created from transaction records and used to group customers into distinct segments using K-Means clustering. The resulting segments were analyzed and visualized to understand differences in customer purchasing patterns.

## Objectives

- Segment customers based on purchasing behavior.
- Analyze customer purchase patterns and preferences.
- Identify the key characteristics of different customer segments.
- Visualize customer segments for better interpretation.

## Dataset

The project uses the **Online Retail Dataset**, which contains historical retail transaction records.

### Dataset Attributes

- **Invoice** – Transaction identifier
- **StockCode** – Product identifier
- **Description** – Product description
- **Quantity** – Number of products purchased
- **InvoiceDate** – Date and time of the transaction
- **Price** – Unit price of the product
- **Customer ID** – Customer identifier
- **Country** – Customer's country

## Data Preparation

The transaction data was prepared before segmentation by:

- Removing duplicate records.
- Handling missing customer identifiers.
- Removing transactions with non-positive quantities.
- Removing transactions with non-positive prices.
- Calculating total sales for each transaction.

## Customer-Level Features

Customer purchasing behavior was summarized using three features:

| Feature | Description |
|---|---|
| **Total Quantity** | Total number of products purchased by a customer |
| **Total Spending** | Total amount spent by a customer |
| **Purchase Frequency** | Number of unique transactions made by a customer |

These features were standardized before applying the clustering algorithm.

## Methodology

The project follows these main steps:

1. Load the historical retail transaction data.
2. Clean and preprocess the transaction records.
3. Calculate transaction-level sales.
4. Aggregate transactions at the customer level.
5. Create customer purchasing behavior features.
6. Standardize the features for clustering.
7. Apply K-Means clustering to create customer segments.
8. Analyze the characteristics of each segment.
9. Visualize the resulting customer segments.

## Clustering

K-Means clustering was used to divide customers into **four segments** based on their purchasing behavior.

The clustering was performed using the following features:

- Total Quantity
- Total Spending
- Purchase Frequency

## Results

The analysis identified four customer segments with different purchasing patterns.

The segments were compared based on their:

- Average quantity purchased
- Average spending
- Average purchase frequency

This provides a clear view of how customer purchasing behavior varies across the identified segments.

## Visualizations

The project includes visualizations for:

- Customer segments based on spending and purchase frequency.
- Key characteristics of the identified customer segments.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

