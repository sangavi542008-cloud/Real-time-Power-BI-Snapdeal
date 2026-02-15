1. Introduction

E-commerce platforms generate massive volumes of transactional data every second. Analyzing this data in real-time helps businesses make faster and smarter decisions.

This project focuses on building a real-time Power BI dashboard using Snapdeal-like e-commerce data generated and processed using coding techniques.

The goal is to simulate and analyze Snapdeal’s sales, customers, and product performance using Business Intelligence tools.

2.Snapdeal is one of India's leading online marketplaces.

It offers:

Electronics

Fashion

Home & Kitchen

Beauty Products

Accessories

Snapdeal connects sellers and customers across India, generating real-time transactional data such as:

Orders

Payments

Customer details

Product categories

Delivery tracking

3. Problem Statement

E-commerce companies like Snapdeal require:

Real-time monitoring of sales performance

Tracking of top-selling products

Regional sales analysis

Customer behavior analysis

Revenue forecasting

Manual reporting is slow and inefficient. Therefore, a real-time dashboard using Power BI is required.

4. Objectives of the Project

To generate Snapdeal-like e-commerce dataset using coding.

To clean and transform the data.

To connect the dataset with Power BI.

To build interactive real-time dashboards.

To analyze sales, revenue, and customer insights.

5. Technologies Used
Technology	Purpose
Python	Data generation & preprocessing
Pandas	Data cleaning
CSV / SQL	Data storage
Power BI	Dashboard creation
DAX	Calculations & KPIs
6. Methodology
Step 1: Data Generation (Coding)

Using Python, I created simulated Snapdeal transaction data including:

Order ID

Product Name

Category

Quantity

Price

Customer Location

Order Date

Payment Mode

Example Code Snippet:

import pandas as pd
import random

products = ["Mobile", "Laptop", "Shoes", "Watch"]
data = []

for i in range(1000):
    data.append([
        i,
        random.choice(products),
        random.randint(1,5),
        random.randint(500,50000)
    ])

df = pd.DataFrame(data, columns=["OrderID","Product","Quantity","Price"])
df.to_csv("snapdeal_data.csv", index=False)

Step 2: Data Cleaning

Removed null values

Standardized category names

Created calculated columns (Total Revenue = Quantity × Price)

Step 3: Power BI Dashboard Creation
4

The dashboard includes:

📈 Total Revenue KPI

🛒 Total Orders

🏆 Top Selling Products

🌍 Sales by Region

📅 Monthly Sales Trend

💳 Payment Mode Analysis

6. Key Dashboard Metrics

Total Revenue

Average Order Value

Sales Growth Rate

Top 5 Products

Customer Distribution by State

Category-wise Profit

7. Sample DAX Measures
Total Revenue = SUMX(Sales, Sales[Quantity] * Sales[Price])

Total Orders = COUNT(Sales[OrderID])

Average Order Value = DIVIDE([Total Revenue], [Total Orders])

8. Results & Insights

From the dashboard analysis:

Electronics category generated highest revenue.

Tier-1 cities contributed more sales.

Cash on Delivery was the most preferred payment method.

Sales increased during festive months.

9. Benefits of This Project

✔ Demonstrates understanding of Business Intelligence
✔ Combines coding + data analytics
✔ Shows real-time data handling skills
✔ Improves decision-making ability
✔ Enhances resume for IT & Business roles

10. Future Enhancements

Connect with live SQL database

Integrate API-based real-time streaming data

Add predictive analysis using Machine Learning

Deploy dashboard on Power BI Service

11. Conclusion

This project successfully demonstrates how real-time Power BI  insights can be generated using coding and Power BI.

By simulating Snapdeal’s e-commerce environment, the dashboard helps analyze sales performance, customer trends, and revenue growth efficiently.

The project bridges the gap between commerce knowledge and technical implementation.
