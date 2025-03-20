# Home_Sales using SparkSQL Big Data 

## Overview
This project demonstrates the use of Apache Spark with PySpark to perform large-scale data analysis using SparkSQL. The dataset `home_sales_revised.csv` is read from an AWS S3 bucket into a PySpark DataFrame and analyzed using SparkSQL queries.

## Objectives
1. Install and set up Spark in Google Colab.
2. Read a CSV file from an S3 bucket into a Spark DataFrame.
3. Create and query temporary views using SparkSQL.
4. Cache and uncache data for performance analysis.
5. Partition data using Parquet format for optimized queries.

## Setup Instructions
1. Open Google Colab.
2. Upload the `.ipynb` notebook to Colab.
3. Install Spark and PySpark using the provided code snippet.
4. Run the notebook cells in order.

## Code Breakdown
### 1. Installation and Setup
- Install OpenJDK and Spark.
- Set up environment variables for Spark.

### 2. Read CSV from S3
- Load the CSV into a DataFrame.
- Display schema and sample data.

### 3. Create Temporary View
- Create a temporary view from the DataFrame.
- Use SparkSQL to query data.

### 4. Perform Data Analysis
- Average price of four-bedroom houses sold per year.
- Average price of 3-bedroom, 3-bathroom homes by year built.
- Average price for homes with specific criteria.

### 5. Performance Analysis
- Compare query runtime for cached vs. uncached data.
- Use Parquet files and partitioning to improve performance.

### 6. Cache and Uncache Data
- Cache and uncache data to compare performance.

### 7. Partitioning and Parquet
- Partition by `date_built` and save as Parquet.
- Read and query partitioned Parquet data.

## Expected Output
- Query results should show properly rounded values.
- Cached queries should run faster than uncached ones.
- Partitioning should improve query efficiency.

## Results and Performance
- Cached queries should improve query performance.
- Partitioned data should enhance query execution speed.

## Notes
- Ensure that the correct Spark version is used.
- PySpark must be installed using `pip install pyspark`.
- Ensure that the S3 bucket is publicly accessible.

