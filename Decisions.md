
# Decisions Made During the Project

# 1. Data Ingestion
I chose to use `dbt seed` to load the `sales.csv` and `customers.csv` files directly into Snowflake. This method is simple and fast for small datasets.

## 2. Data Transformation
- I created the `transformed_sales_data.sql` model to extract year, month, and day from the `order_date`, and to calculate the `total_sales_amount`.
- The data was aggregated and structured to make querying easier for further analysis.

 3. Query Optimizations
- I used SQL functions such as `EXTRACT` to break down the date into components.
- To answer business questions, I grouped and ordered data efficiently to ensure queries were optimized for performance.

# Challenges
- Handling Snowflake schema and connection was the biggest challenge initially, but I was able to configure it correctly by following the dbt documentation.

