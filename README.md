# Retail Sales SQL Assessment

## About the Project

This project is a SQL-based Retail Sales Analysis completed as part of a SQL assessment.

The main aim of this project is to analyze retail sales and return data and find useful information about customers, orders, stores, regions, products, and returns.

The data is for the period **October 1, 2026 to October 31, 2026** and all amounts are in **USD**.

## Tools Used

- DB Fiddle
- MySQL 9
- SQL

## Tables Used

The project contains the following tables:

- Customers
- Stores
- Products
- Orders
- OrderItems
- Returns
- Regions

## What I Did

### 1. Region Data Cleaning
- Standardized the region names.
- Created a `Regions` table.
- Connected the stores with the corresponding regions.

### 2. Duplicate Data Cleaning
- Checked duplicate `OrderItemID` values.
- Kept the latest record using the `LoadedAt` column.

### 3. Customer and Order Analysis
- Found orders with matching customers.
- Found orders with unmatched customer IDs.
- Identified customers who did not place any orders.

### 4. Return Analysis
- Found order items having multiple return transactions.
- Calculated returned quantities.
- Analyzed returns by region and product category.

### 5. Sales Analysis
- Calculated gross sales for each region and store.
- Calculated return value.
- Calculated net sales.

**Net Sales = Gross Sales - Return Value**

### 6. Regional and Store Performance
- Compared the performance of North, South, and West regions.
- Found the highest net-sales store in each region.
- Compared gross sales and net sales.

## Some Key Findings

- North had the highest gross sales of **$14,389.25**.
- South had the highest net sales of **$13,037.00**.
- South's net sales were **$210 higher than North**.
- North had **$1,562.25** in return value.
- Electronics was the highest-return category in North with **$669.00**.

### Highest Net Sales Stores

| Region | Store | Net Sales |
|---|---|---:|
| North | Riverfront | $6,592.50 |
| South | Cedar Market | $7,112.50 |
| West | Summit Mall | $6,607.50 |

## Recommendation

Based on the analysis, North region needs more attention towards product returns, especially in the Electronics category.

Some possible actions are:

- Check products with high return rates.
- Understand the reasons for customer returns.
- Improve product descriptions and packaging.
- Track returns by product and store.
- Collect customer feedback.

## Project Structure

```text
Retail-Sales-SQL-Assessment/
│
├── README.md
│
├── Assessment/
│   └── Completed_Worksheet.docx
│
├── SQL/
│   └── Retail_Sales_Assessment.sql
│
├── SQL_Output/
│   ├── Q1_Output.png
│   ├── Q2_Output.png
│   ├── Q4_Output.png
│   ├── Q5_Output.png
│   ├── Q6_Output.png
│   ├── Q7_Output.png
│   ├── Q8_Output.png
│   ├── Q9_Output.png
│   ├── Q10_Output.png
│   └── Q11_Output.png
│
├── ER_Diagram/
│   └── Retail_ER_Diagram.png
│
└── Presentation/
    └── Retail_Sales_Findings.pptx
```

## Conclusion

Through this project, I practiced SQL concepts such as:

- Joins
- Aggregate functions
- GROUP BY
- CASE statements
- CTEs
- Window functions
- Data cleaning
- Duplicate handling
- Sales analysis
- Return analysis

This project helped me understand how SQL can be used to analyze real-world business data and generate useful insights.