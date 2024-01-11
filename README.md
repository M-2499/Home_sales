**Home-Sales-Big-Data-with-PySpark-SQL**

## This project involved working with Big Data and SparkSQL in order to analyze and query home sales data. The data analysis processes where conducted as follow:

Importing packages: The project started by importing the necessary packages, including findspark to initialize Spark and pyspark.sql for working with SparkSQL.

Creating a SparkSession: A SparkSession was created using SparkSession.builder.appName("SparkSQL").getOrCreate() to establish a connection to Spark.

Reading data: The home sales data was read from an AWS S3 bucket into a DataFrame using the provided URL.

Creating a temporary view: A temporary view named "my_table" was created for the DataFrame using createOrReplaceTempView() method. This allowed for running SQL queries on the DataFrame.

Querying the data: Several SQL queries were executed to analyze the home sales data. This included calculating the average price for a four-bedroom house sold in each year and the average price of homes based on different criteria such as bedrooms, bathrooms, and square footage.

Caching the data: The temporary table "home_sales_df" was cached using spark.catalog.cacheTable() method to improve query performance by storing the data in memory.

Query runtime comparison: The runtime of a specific query was compared between the cached version and the version using Parquet data. The start time was recorded using time.time() before executing each query, and the difference in time was calculated to measure the runtime.

Writing Parquet data: The formatted home sales data was written to Parquet format with partitioning based on the "date_built" field using the partitionBy().parquet() method.

Reading Parquet data: The Parquet data was read into a DataFrame to perform further analysis.



## Through utilizing PySpark and Spark SQL on Google Colab, the project serves to determine key metrics about home sales data. Some of the data key metric questions that were answered:

What is the average price for a four-bedroom house sold for each year?

What is the average price of a home for each year it was built that has three bedrooms and three bathrooms?

What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet?

What is the "view" rating for homes costing more than or equal to $350,000?

The project involved analyzing, cleansing, plotting, featurizing and modeling about a year's worth (20K) home sales in the Seattle metro-area from 2014-2015. I used the tools and libraries from Python, Numpy, Pandas, Seaborn, StatsModel, Sklearn and Scipy. We had a requirement to develop a multiple linear regression model as an initial approach to forecasting home prices. Here you can find my final business presentation and my Jupyter notebook.

Feel free to reach out if you have any questions or need further clarification. Happy coding!
