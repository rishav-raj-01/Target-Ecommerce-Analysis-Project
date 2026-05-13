# Target-Ecommerce-Analysis-Project
A data analysis project where I explored an e-commerce dataset (similar to Target's Brazil operations) using Python and MySQL. The goal was to practice end-to-end data work — loading raw CSVs into a relational database and then writing SQL queries to answer business questions, with some visualizations along the way.

### **What This Project Does**
The notebook is split into two parts:
1. Data Ingestion
Loads 7 CSV files into a local MySQL database automatically. It reads each file with pandas, infers column data types, creates the corresponding table in MySQL, and inserts all the rows. Handles NaN → NULL conversion so the data doesn't break during insertion.
2. Business Analysis (14 Questions)
Connects to the database and runs SQL queries to answer real analytical questions. Some results are returned as DataFrames, some are plotted using matplotlib/seaborn.

### **Analysis Covered**

* All unique cities where customers are located
* Total orders placed in 2017
* Total sales revenue per product category
* Percentage of orders paid in installments
* Customer count by state (bar chart)
* Monthly order count for 2018 (bar chart)
* Average products per order, grouped by customer city
* Correlation between product price and purchase frequency
* Total revenue per seller with dense rank
* Moving average of order value per customer (3-row window)
* Cumulative sales per month across years
* Year-over-year sales growth rate
* Customer retention rate (repurchase within 6 months)
* Top 3 highest-spending customers per year (bar chart)

The later questions (10–14) involve window functions like LAG, DENSE_RANK, rolling averages, and CTEs

### **Tech Stack**

* Python — pandas, matplotlib, seaborn, numpy
* MySQL — via mysql-connector-python
* Jupyter Notebook


### **What I Learned**

* How to automate CSV-to-MySQL loading with dynamic schema creation
* Writing window functions in SQL (moving averages, cumulative sums, YoY growth, ranking)
* Joining multiple tables to answer layered business questions
* Using pandas + seaborn for quick visualizations from query results



### **Notes**
* This was a personal project I built to get more comfortable with SQL analytics and connecting it to Python. The dataset is publicly available and inspired by Target's e-commerce operations in Brazil (originally from Kaggle/OLIST). Nothing is production-ready — it's meant as a learning exercise and portfolio piece.
