# Walmart Sales Data Analysis

## Overview

This project analyzes Walmart sales data to understand top-performing branches and products, sales trends, and customer behavior. The dataset, sourced from the Kaggle Walmart Sales Forecasting Competition, includes sales transactions from Walmart stores in Mandalay, Yangon, and Naypyitaw.

## Objectives

### Product Analysis
- Assess product lines' performance to identify top performers and areas for improvement.

### Sales Analysis
- Examine sales trends to evaluate and optimize sales strategies.

### Customer Analysis
- Explore customer segments and purchasing behavior to enhance profitability.

## Schema

### Table: `sales`

- **invoice_id**: Unique invoice ID
- **branch**: Branch location
- **city**: City
- **customer_type**: Type of customer
- **gender**: Customer's gender
- **product_line**: Product category
- **unit_price**: Price per unit
- **quantity**: Quantity sold
- **tax_pct**: Tax percentage
- **total**: Total amount
- **date**: Transaction date
- **time**: Transaction time
- **payment**: Payment method
- **cogs**: Cost of goods sold
- **gross_margin_pct**: Gross margin percentage
- **gross_income**: Gross income
- **rating**: Customer rating
- **time_of_day**: Time of day (Morning, Afternoon, Evening)
- **day_name**: Day of the week
- **month_name**: Month

## Key Questions

### General
- **How many unique cities are in the dataset?**
- **Which city hosts each branch?**

### Product
- **How many product lines are there?**
- **What is the most common payment method?**
- **What is the highest-selling product line?**
- **What are the total revenues and COGS by month?**
- **Which city generates the most revenue?**
- **How does each product line perform in terms of sales and VAT?**

### Sales
- **How do sales vary by time of day and weekday?**
- **Which customer type generates the most revenue and VAT?**

### Customer
- **How many customer types and payment methods are there?**
- **What is the gender distribution across branches?**
- **When do customers give the highest ratings?**

## Revenue and Profit Calculations

- **COGS**: unit_price * quantity
- **VAT**: 5% of COGS
- **Total Sales**: VAT + COGS
- **Gross Profit**: Total Sales - COGS
- **Gross Margin**: (Gross Profit / Total Sales) * 100%

### Example Calculation
For a unit price of $45.79 and quantity of 7:

- **COGS**: $320.53
- **VAT**: $16.03
- **Total Sales**: $336.56
- **Gross Margin**: 4.76%

