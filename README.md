# Coffee Sales Dashboard

## Project Overview

This project showcases the creation of a **Coffee Sales Dashboard** in Microsoft Excel to visualize and analyze sales data over multiple years. Using advanced Excel functions, the dashboard provides insights into sales trends, top countries, and high-value customers, offering a dynamic and interactive experience.

## Table of Contents

- [Data Sources](#data-sources)
- [Data Processing](#data-processing)
- [Dashboard Visualizations](#dashboard-visualizations)
- [Interactive Features](#interactive-features)
- [Usage Instructions](#usage-instructions)
- [Conclusion](#conclusion)
- [Author](#author)

## Data Sources

The project leverages three datasets:

1. **Customers**:
   - Customer ID, Customer Name, Email, Phone Number, Address, City, Country, Postcode, Loyalty Card.
   
2. **Products**:
   - Product ID, Coffee Type, Roast Type, Size, Unit Price, Price per 100g, Profit.
   
3. **Orders**:
   - Order ID, Order Date, Customer ID, Product ID, Quantity, Customer Name, Email, Country, Coffee Type, Roast Type, Size, Unit Price (INR), Sales (INR), Loyalty Card.

> **Note**: Customer and product details were integrated into the *Orders* table using **XLOOKUP** and **INDEX-MATCH** functions.

## Data Processing

Key transformations and calculations:

- **Customer and Product Data Integration**: Used **XLOOKUP** to pull customer details and **INDEX-MATCH** for product information from the corresponding tables.
- **Unit Price (INR)**: Calculated by converting the product's original price into Indian Rupees.
- **Sales (INR)**: Computed as `Quantity * Unit Price (INR)`.
- **Coffee Type Name & Roast Type Name**: Generated using **IF conditions** to categorize data for easier visualization.

## Dashboard Visualizations

The dashboard includes three main charts:

1. **Coffee Sales Over Time** (Line Chart): 
   - Visualizes monthly sales trends across different coffee types (Arabica, Excelsa, Liberica, Robusta) over multiple years.
   
2. **Top 3 Countries by Total Sales** (Column Chart): 
   - Highlights the top-performing countries in terms of total sales (United States, Ireland, United Kingdom).

3. **Top 5 Customers by Sales** (Column Chart): 
   - Displays the highest-spending customers, showcasing key contributors to revenue.

## Interactive Features

The dashboard includes **Slicers** to filter data dynamically:

1. **Roast Type Name**: Filter by Dark, Light, or Medium roast types.
2. **Loyalty Card**: Filter based on whether a customer holds a loyalty card.
3. **Size**: Filter by product size (0.2 Kg, 0.5 Kg, 1.0 Kg, 2.5 Kg).

These slicers allow for real-time filtering and more granular insights into the data.

## Usage Instructions

1. **Open the Excel Workbook**: Navigate to the "Dashboard" worksheet.
2. **Filter Data**: Use the slicers on the right to filter by Roast Type, Loyalty Card, and Size. The charts will update dynamically based on your selection.
3. **Analyze Data**:
   - Review coffee sales trends in the line chart.
   - Observe top countries in the column chart.
   - Analyze the top customers and their contribution to total sales.

## Conclusion

This Coffee Sales Dashboard is designed to provide a clear and interactive view of the sales data, making it easier to identify trends, evaluate product performance, and understand customer behavior. With dynamic filtering and calculated metrics, the dashboard offers valuable insights for decision-making.

## Author

**Velampudi Rohit** 
