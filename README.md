# Inventory Management Analysis

## Overview

This project aims to optimize inventory management for a medium-sized manufacturing company by analyzing key aspects of inventory data. The analysis includes cleaning and preprocessing data, calculating lead times, determining safety stock levels, identifying excess inventory, evaluating vendor performance, identifying top-selling items and stores, and calculating Economic Order Quantity (EOQ). The goal is to reduce costs, improve efficiency, and enhance customer satisfaction.

## Objectives

1. **Improving Data Quality**: Ensure the inventory data is clean, consistent, and ready for analysis.

2. **Understanding Lead Times**: Analyze supplier performance by calculating and visualizing lead times.

3. **Preventing Stockouts**: Calculate safety stock levels to avoid stockouts and ensure product availability.

4. **Reducing Excess Inventory**: Identify items with excess inventory and recommend strategies to reduce carrying costs.

5. **Evaluating Vendor Performance**: Analyze vendor performance based on total spend and payment cycles.

6. **Identifying Top Performers**: Determine the top-selling items and stores to focus on high-revenue products and locations.

7. **Optimizing Order Quantities**: Calculate the Economic Order Quantity (EOQ) to minimize ordering and carrying costs.

### Data Sources

The project uses the following CSV files from the Inventory_Analysis_Case_Study.zip file:

- InvoicePurchases12312016.csv
- EndInvFINAL12312016.csv
- BegInvFINAL12312016.csv
- 2017PurchasePricesDec.csv
- SalesFINAL12312016.csv
- PurchasesFINAL12312016.csv

### Project Workflow

The project uses the following steps:

**1. Loading Data**
- Loads CSV files from the zip archive into pandas DataFrames.

**2. Cleaning and Preprocessing Data**
- Handles missing values and duplicates.
- Removes leading/trailing whitespace from string columns.
- Converts date columns to the datetime format.

**3. Analyzing Lead Times**
- Calculates lead times (time between placing an order and receiving it).
- Summarizes max, min, average, and standard deviation of lead times.

**4. Calculating Safety Stock**
- Calculates safety stock levels to avoid stockouts using average daily sales and lead time variability.

**5. Identifying Excess Inventory**
- Compares current inventory levels with safety stock to identify excess inventory.

**6. Analyzing Vendor Performance**
- Evaluates vendor performance based on total spend and payment cycles.

**7. Analyzing Top-Selling Items and Stores**
- Identifies top-performing products and stores based on sales data.

**8. Calculating Economic Order Quantity (EOQ)**
- Determines the optimal order quantity to minimize ordering and carrying costs.

### Expected Output

1. Top 10 Excess Inventory Items: A list of items with excess inventory.
2. Top 10 Vendors by Total Spend: A list of top-performing vendors.
3. Top 10 Selling Items: A list of top-selling products.
4. Top 10 Selling Stores: A list of top-performing stores.
5. EOQ Summary: A list of Economic Order Quantities for each product.

### Results

**1. Excess Inventory**
- Items like Gekkeikan Black & Gold Sake and Three Olives Espresso Vodka have significant excess inventory.

**2. Vendor Performance**
- DIAGEO NORTH AMERICA INC is the top vendor, with total spend of $50,959,796.85.

**3. Top-Selling Items and Stores**
- Smirnoff 80 Proof is the top-selling item, with 28,544 units sold.
- Store 15 is the top-performing store, generating 101,078 units in sales.

**4. Economic Order Quantity (EOQ)**
- The EOQ for Gekkeikan Black & Gold Sake is 266 units.

### Source

https://www.kaggle.com/datasets/bhanupratapbiswas/inventory-analysis-case-study
