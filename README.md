# Home-sales

# Contributors 

By: Alex Calametti 

---

# Home Sales Data Analysis with PySpark

## Overview

The goal of this project is to analyze home sales data using PySpark. The script performs various data manipulations, runs Spark SQL queries, and demonstrates caching strategies to optimize query performance and answer metrics questions pertaining to the data set.

## Requirements

- Programs: PySpark, Java, Google Colab
- Access to an AWS S3 bucket containing the home sales data.
- home_sales_starter_code.ipynb

# Steps

1. **Data Setup**
   - Create the Spark Session
   - Read in home sales data from the AWS S3 bucket into a PySpark DataFrame using the link.
   - Creates a temporary view of the DataFrame to perform Spark SQL queries.

3. **Queries:**
   - Executes Spark SQL queries to answer questions about the home sales data to learn more about average home prices.

4. **Cache Management:**
   - Use caching strategies by caching and uncaching a temporary table (`home_sales`) to improve query time.
   - Compare query runtimes between the cached and uncached scenarios.

5. **Parquet File Operations:**
   - Write the DataFrame to a partitioned Parquet file using the "date_built" field.
   - Read the Parquet formatted data into a new pandas DataFrame.
   - Create a temporary table for the Parquet data and re-run the query.


