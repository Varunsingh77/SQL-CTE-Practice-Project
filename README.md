# SQL-CTE-Practice-Project
This project demonstrates the use of Common Table Expressions (CTEs), CASE statements, and JOINs in SQL using a small, realistic Sales dataset. It simulates a retail environment with products, stores, and sales transactions — allowing data analysts to practice structured query building and modular query design with CTEs

# The dataset includes:

sales_data: individual sales transactions

products: product information (category, cost price)

stores: store and manager details

Using this data, multiple analytical queries are written to explore:

Sales performance per store, region, and product

Revenue patterns by payment method and date

Ranking and categorization using CASE and window functions

Multi-level CTEs for hierarchical analysis

# Database Schema

# products

Column	Type	Description
product_id	INT	Unique product identifier
product_name	VARCHAR(50)	Product name
category	VARCHAR(30)	Product category
cost_price	DECIMAL(10,2)	Cost price of product

# stores

Column	Type	Description
store_id	INT	Unique store identifier
store_name	VARCHAR(50)	Store name
city	VARCHAR(30)	Store location
manager_name	VARCHAR(30)	Store manager’s name

# sales_data

Column	Type	Description
sale_id	INT	Unique sale transaction
sale_date	DATE	Date of sale
store_id	INT	Linked to store
product_id	INT	Linked to product
quantity	INT	Units sold
unit_price	DECIMAL(10,2)	Selling price per unit
payment_method	VARCHAR(20)	UPI, Cash, or Card
region	VARCHAR(20)	Regional location

# SQL Concepts Covered

Concept	Example Used
CTE (Common Table Expression)	Reusable temporary result sets for clean logic
CASE Statement	Categorize store performance
JOINs	Combine sales, products, and store info
Window Functions	Ranking regions by sales
Aggregate Functions	SUM, AVG, COUNT used for analytics
Nested / Multi-level CTEs	Average revenue comparison

 # Queries Implemented

Total Sales Amount per Sale → Filters transactions above ₹1000

Store Revenue Calculation → Filters stores with revenue > ₹3000

Product-wise Quantity Sold → Joins CTE output with product names

Revenue by Payment Method → Finds top-earning method

Region Ranking → Uses RANK() to rank total sales

Store Categorization → Uses CASE to label stores as High/Average/Low performing

Daily Revenue → Identifies the most profitable day

Two-level CTE → Finds stores with above-average revenue

Profit per Category (optional future extension)

Multi-table Joins for combined insights

🧠 Learning Outcomes

By practicing this project, you’ll learn to:

Write clean, modular SQL using CTEs.

Simplify complex aggregations and filtering.

Analyze business metrics using SQL directly.

Use CASE and window functions for analytical insights.

Structure SQL queries suitable for data analytics interviews.

# Tech Stack

Database: MySQL

Concepts: CTE, JOIN, CASE, Window Functions

Dataset: Manually created dummy dataset for analysis practice using copilot

# How to Run

Clone or copy this SQL script into your local environment.

Run:

CREATE DATABASE cte;
USE cte;


Execute the table creation and insert statements.

Run each CTE query individually to observe the output and logic.

# Author

Varun Singh
🎓 BBA Student | 📊 Aspiring Data Analyst
💡 Skills: SQL | Excel | Power BI | Python
🔗 Connect with me on LinkedIn → www.linkedin.com/in/varunsingh-analytics
