📊 Swiggy Dashboard Analysis – Power BI
This project presents an end-to-end Power BI dashboard built to analyze Swiggy food order data and extract meaningful business insights. The dashboard helps understand customer ordering behavior, food type performance, city-wise revenue contribution, and time-based trends.

🎯 Business Objective

The objective of this project is to:

Compare Veg vs Non-Veg order performance

Identify top revenue-generating cities

Analyze peak ordering days and trends

Provide executive-level KPIs for quick decision-making

🗂️ Dataset

Source: Swiggy raw order data (Excel)

Type: Transactional data

Key Columns:

Order ID

Order Date

City

Item Name

Food Type (Veg / Non-Veg)

Order Amount

🔧 Data Cleaning & Transformation

Performed using Power Query:

Removed duplicate and null records

Standardized city and item names

Converted data types for accurate analysis

Created derived columns:

Weekday

Month

Food Type classification

🧠 Data Modeling

Implemented a single fact table optimized for performance

Ensured clean schema and correct data types

Prepared data for efficient DAX calculations

📐 DAX Measures

Key measures created in Power BI:

Total Orders = COUNT('Swiggy'[Order ID])

Total Revenue = SUM('Swiggy'[Order Amount])

Average Order Value =
DIVIDE([Total Revenue], [Total Orders])

Veg Orders =
CALCULATE([Total Orders], 'Swiggy'[Food Type] = "Veg")

Non Veg Orders =
CALCULATE([Total Orders], 'Swiggy'[Food Type] = "Non-Veg")

📊 Dashboard Pages
1️⃣ Executive Overview

KPI Cards: Total Orders, Revenue, AOV

Order trend analysis

Veg vs Non-Veg comparison

Top cities by revenue

2️⃣ Food Type Analysis

Revenue comparison between Veg and Non-Veg

Item-level performance table

3️⃣ Time Analysis

Orders by weekday

Revenue trends over time

4️⃣ City Performance

City-wise revenue distribution

Top-performing cities

🔍 Key Insights

Non-Veg orders generate higher revenue per order

Weekends show peak demand

A few cities contribute most of the total revenue

Veg orders are more frequent but lower in average value

💼 Business Impact

This dashboard enables:

Data-driven promotional strategies

City-wise marketing optimization

Better staffing and operational planning

Faster executive decision-making

🛠️ Tools & Technologies

Power BI Desktop

Power Query

DAX

Excel

📁 Repository Structure
📦 Swiggy-PowerBI-Dashboard
 ┣ 📂 Dataset
 ┃ ┗ Swiggy_Raw_Data.xlsx
 ┣ 📂 Dashboard
 ┃ ┗ Swiggy_Orders_Performance.pbix
 ┣ 📂 Screenshots
 ┃ ┗ Dashboard_Overview.png
 ┗ README.md

🚀 How to Use

Download the repository

Open the Swiggy data analysis.pbix file in Power BI Desktop :https://github.com/Avrodita/power-Bi-project/blob/main/swiggy%20data%20analysis.pbix

Dashboard look like: https://github.com/Avrodita/power-Bi-project/blob/main/Swiggy%20Dashboard%20Ananlysis.png

Refresh data (if required)

Explore dashboards using slicers

✨ Conclusion

This project demonstrates my ability to transform raw data into actionable business insights using Power BI, combining data modeling, DAX, and professional dashboard design.

⭐ If you like this project, feel free to star the repository!
