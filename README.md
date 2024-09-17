# Retail Sales SQL Analysis Project

## Project Overview
This project contains SQL queries and analysis related to retail sales data. The dataset contains various columns including sales revenue, units sold, product categories, store locations, marketing spend, and more. The queries are designed to perform data analysis tasks such as calculating total sales by region, identifying top-performing products, and analyzing marketing impact on sales.

## Project Structure
- `queries.sql`: This file contains SQL queries used to analyze the retail sales data.
- `README.md`: This file provides an overview of the project, setup instructions, and usage guidelines.

## Contents of `queries.sql
The `queries.sql` file includes the following types of queries:
- Exploration Queries:
  - View sample data from the retail sales table.
  - Count total records in the dataset.
  - Identify missing or null values.
  
- Aggregation Queries:
  - Calculate total sales by region.
  - Summarize units sold by product category.
  - Determine the top-performing products by revenue and units sold.
  
- Time-Based Analysis:
  - Analyze sales trends by month.
  - Compare units sold by day of the week to spot patterns.

- Marketing Analysis:
  - Evaluate the correlation between marketing spend and total sales.
  - Summarize marketing spend by region.

## Setup Instructions

### 1. Prerequisites
Ensure you have the following installed:
- PostgreSQL
- Git (for managing repository)

### 2. Cloning the Repository
To clone this repository, run the following command in your terminal:

```bash
git clone https://github.com/web8080/sql-project.git
```

### 3. Importing the Dataset
Before running the queries, make sure you’ve imported your dataset into the PostgreSQL database. You can follow these steps:
1. Create a table in your PostgreSQL database that matches the dataset structure (e.g., `retail_sales`).
2. Use the `\copy` command to import the dataset:

   ```sql
   \copy retail_sales(store_id, product_id, sale_date, units_sold, sales_revenue, discount_percentage, marketing_spend, store_location, product_category, day_of_week, holiday_effect)
   FROM '/path/to/your/file.csv'
   DELIMITER ',' CSV HEADER;
   ```

3. Verify the data is correctly imported by running a simple query:

   ```sql
   SELECT * FROM retail_sales LIMIT 10;
   ```

### 4. Running the SQL Queries
Once the data is loaded into PostgreSQL, you can run the queries found in `queries.sql` using the `psql` command-line interface or any SQL client tool like pgAdmin.

To execute the queries:
1. Open the `psql` tool:
   ```bash
   psql -U postgres -d your_database
   ```

2. Run the queries from `queries.sql`. You can either copy/paste them or use the `\i` command to run the SQL file directly:

   ```sql
   \i /path/to/queries.sql
   ```

### 5. Results**
The results of the queries will show various analyses based on the dataset, including:
- Total sales per region.
- Top-performing products.
- Marketing impact on sales.

## Usage
You can modify the SQL queries in the `queries.sql` file to adjust for different datasets or to extend the analysis as needed.

## Contributing
Feel free to fork this repository and submit pull requests for any improvements or additional features you think would enhance the project.

---

### **Author**
- Victor Ibhafidon
- [Your GitHub Profile](https://github.com/web8080
