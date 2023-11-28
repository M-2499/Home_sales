# Home Sales Data Analysis with PySpark SQL

## Overview

In this project, I'll be utilizing PySpark SQL to analyze key metrics related to home sales data. The tasks involve creating temporary views, partitioning data, caching and uncaching temporary tables, and assessing query runtimes.

## Before I Begin

1. I have created a new repository for this project called "Home_Sales." I made sure not to add this homework to an existing repository.
2. I have cloned the new repository to my computer.
3. I pushed my changes to GitHub.

## Files

I have downloaded the necessary files to get started: [Module 22 Challenge files](#) (Link to be provided).

## Instructions

1. **Setup:**
   - I have renamed the `Home_Sales_starter_code.ipynb` file as `Home_Sales.ipynb`.
   - I have imported the necessary PySpark SQL functions for this assignment.

2. **Data Loading:**
   - I read the `home_sales_revised.csv` data in the starter code into a Spark DataFrame.
   - I created a temporary table called `home_sales`.

3. **SparkSQL Analysis:**
   - I answered the following questions using SparkSQL:
     - What is the average price for a four-bedroom house sold for each year? (Rounded off to two decimal places.)
     - What is the average price of a home for each year it was built with three bedrooms and three bathrooms? (Rounded off to two decimal places.)
     - What is the average price of a home for each year with three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? (Rounded off to two decimal places.)
     - What is the "view" rating for homes costing more than or equal to $350,000? I determined the run time for this query. (Rounded off to two decimal places.)

4. **Caching:**
   - I cached my temporary table `home_sales`.
   - I checked if my temporary table is cached.
   - Using the cached data, I ran the query that filters out the view ratings with an average price greater than or equal to $350,000. I determined the runtime and compared it to uncached runtime.

5. **Data Partitioning:**
   - I partitioned by the "date_built" field on the formatted parquet home sales data.
   - I created a temporary table for the parquet data.

6. **Query Performance:**
   - I ran the query that filters out the view ratings with an average price greater than or equal to $350,000 using the parquet data. I determined the runtime and compared it to uncached runtime.

7. **Uncaching:**
   - I uncached the `home_sales` temporary table.
   - I verified that the `home_sales` temporary table is uncached using PySpark.

8. **Final Steps:**
   - I downloaded my `Home_Sales.ipynb` file and uploaded it into my "Home_Sales" GitHub repository.

Feel free to reach out if you have any questions or need further clarification. Happy coding!
