# Home Sales Data Analysis with PySpark

## Overview

This project aims to analyze home sales data using PySpark, a powerful analytics engine for large-scale data processing. The dataset used in this analysis contains information about home sales, including sale dates, prices, number of bedrooms and bathrooms, square footage, and other relevant details.

## Requirements

To run the code in this project, you'll need:

- Python 3.x
- PySpark
- Jupyter Notebook or any Python IDE
- An internet connection to access the dataset stored on AWS S3

## Description

1. **Data Loading**: The code starts by importing the necessary libraries and loading the home sales dataset from an AWS S3 bucket into a PySpark DataFrame.

2. **Data Exploration**: Various SQL queries are executed to explore the dataset, including calculating average prices for different criteria such as number of bedrooms, bathrooms, and year built.

3. **Data Caching**: The script demonstrates how to cache the DataFrame for improved performance when running multiple queries.

4. **Data Partitioning**: The DataFrame is partitioned by the `date_built` field and written to disk in the Parquet format for efficient storage and retrieval.

5. **Parquet Data Analysis**: The Parquet data is read back into a DataFrame, and similar SQL queries are executed to analyze the data, comparing performance with the cached DataFrame.

6. **Uncaching**: Finally, the cached DataFrame is uncached to release memory resources.

## Usage

To use this project:

1. Ensure you have met the requirements mentioned above.
2. Clone or download the repository to your local machine.
3. Open the `home_sales_analysis.ipynb` notebook in a Jupyter Notebook or your preferred Python IDE.
4. Run the code cells sequentially to execute the data analysis tasks.