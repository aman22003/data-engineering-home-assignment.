# data-engineering-home-assignment.

This project analyzes sales data for a fictional company to answer key business questions. The analysis was performed using "dbt"  and Snowflake.

## Setup Instructions

1. Snowflake Setup
A. Created a Snowflake account  and set up a database named `home_assignment`.
B. In the `~/.dbt/profiles.yml` file, configured Snowflake as per the instructions.

 2. dbt Setup
1. Installed dbt 
2. Connected Snowflake account is configured correctly in the `profiles.yml` file.
3. Test the connection with:
  Command-
   dbt debug

3. Ingesting Data
-paste the sales.csv and customers.csv files in the data/ folder in project named dbt_banxware_assignment.
Run the following command to load the raw data:
Command-
dbt seed

4.Data Transformation with dbt
Created a model for transformed_sales_data in the models folder in dbt.

SQL Transformation: Create a file transformed_sales_data.sql and used this SQL to transform the raw sales data:
Execute the transformations:
command-
dbt run

5. Running the SQL Queries
Navigate to the queries folder and run each SQL file in Snowflake to get the answers to the business questions.

