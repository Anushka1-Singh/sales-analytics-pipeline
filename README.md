# Sales Analytics Pipeline

This is my data analytics project where I built a complete pipeline 
from raw sales data to an interactive Power BI dashboard.

## Dashboard Preview

![Dashboard](dashboard.png)


## What this project does

- Takes raw sales data from an Excel file
- Cleans the data using Python and pandas
- Stores the cleaned data in a MySQL database
- Visualizes the data using a Power BI dashboard

## Tools and Technologies used

- Python
- pandas
- MySQL
- SQLAlchemy
- pymysql
- Power BI
- Jupyter Notebook

## Project Steps

**Step 1 - Data Cleaning (cleaning.ipynb)**
Loaded raw Excel data of 520 rows, removed 20 duplicate rows, 
fixed invalid dates, and created 3 new columns - Profit, Year and Month.
Final clean data has 482 rows and 10 columns.

**Step 2 - Load to MySQL (cleaning.ipynb)**
Connected Python to MySQL using SQLAlchemy and loaded the 
cleaned data into a database called salesdb.

**Step 3 - Append New Data (append_2026.ipynb)**
Loaded new 2026 sales data and appended it to the existing 
MySQL table. Total records went from 482 to 682.

**Step 4 - Power BI Dashboard**
Connected Power BI directly to MySQL and built an interactive 
dashboard showing total profit, total sales, monthly trends, 
product performance and region-wise profit.

## Files in this project

- cleaning.ipynb - data cleaning and MySQL loading notebook
- append_2026.ipynb - new data append notebook  
- sales_raw_500.xlsx - original raw data
- sales_raw_new_2026.csv - new 2026 data
- sales_cleaned.csv - cleaned output data
