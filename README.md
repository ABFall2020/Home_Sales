# Home_Sales

Home Sales Analysis with PySpark
In this project, we leverage PySpark and SparkSQL to perform a comprehensive analysis of home sales data. The primary goal is to extract key metrics and insights, such as average home prices across various dimensions. Through this challenge, we also explore advanced data handling techniques including data caching, partitioning, and performance optimization using PySpark.

Project Overview:
Data Loading and Transformation: We begin by importing and reading home sales data from a CSV file into a Spark DataFrame. This data is then registered as a temporary SQL table, allowing for efficient querying and manipulation.

SQL-Based Analysis: Using SparkSQL, we conduct a series of analyses to uncover trends in home prices:

Calculate average prices for four-bedroom houses sold each year.
Determine average prices for homes with specific features (e.g., three bedrooms and three bathrooms) for each year they were built.
Analyze the average price of larger homes (with two floors and at least 2,000 square feet) built each year.
Investigate how home prices vary by "view" rating, particularly focusing on homes priced at $350,000 or higher.
Performance Optimization: We enhance query performance by caching the temporary table and compare query runtimes with and without caching. This demonstrates the impact of caching on computational efficiency in Spark.

Data Partitioning: The home sales data is partitioned by the construction year (date_built), which facilitates efficient storage and querying of large datasets. We analyze how partitioning affects query performance.

Resource Management: To maintain optimal resource usage, we explore how to cache and uncache data in Spark, ensuring that temporary tables are properly managed throughout the process.

This project highlights the power of PySpark for large-scale data analysis and the importance of SQL-based querying, data caching, and partitioning to optimize data processing workflows.
