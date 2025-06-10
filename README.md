Home_Sales

Determine key metrics about home sales data using SparkSQL and then use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.
Table of Contents

    Getting Started
    Prerequisites
    Coding Instruction

Getting Started

Using Jupyter Notebook and PySpark SQL, analyze home sales data and determine key metrics by observing the data and answering the questions provided.
Prerequisites

Requirements for the software and other tools to build, test and push

    Jupyter Notebook
    PySpark SQL
    Pyspark

Coding Instruction
District Summary

Perform the necessary calculations and then create a high-level snapshot of the district's key metrics in a DataFrame.

    Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.
    Import the necessary PySpark SQL functions for this assignment.
    Read the home_sales_revised.csv from the provided AWS S3 bucket location into a PySpark DataFrame.
    Create a temporary table called home_sales.
    Answer the following questions using SparkSQL:
        What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
        What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? Round off your answer to two decimal places.
        What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.
        What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.
    Cache your temporary table home_sales.
    Check if your temporary table is cached.
    Using the cached data, run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
    Partition by the "date_built" field on the formatted parquet home sales data.
    Create a temporary table for the parquet data.
    Run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
    Uncache the home_sales temporary table.
    Verify that the home_sales temporary table is uncached using PySpark.
    Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository.
