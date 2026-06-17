📊 E-Commerce Business Analytics (SQL + Power BI)
📌 Project Overview
The objective of this project was to process e-commerce transactional data, calculate complex business metrics using SQL, and build an interactive Power BI dashboard to support strategic decision-making.

🛠️ Tech Stack
SQL Server (T-SQL): CTEs, Window Functions, Data Cleaning, VIEW Creation.

Power BI: Data Modeling (Snowflake Schema), DAX, Interactive Visualization.

⚙️ Data Engineering (ETL & Normalization)
Executed a full ETL (Extract, Transform, Load) cycle and optimized the data architecture:

Data Transformation & Cleaning: Cleaned raw data by removing duplicates, fixing text anomalies (trimming spaces & correcting casing issues), and standardizing date formats.

Data Normalization: Normalized the dataset following 3rd Normal Form (3NF) principles. Isolated the fact_Orders table from reference dimension tables (dim_Products, dim_Sub_Category, dim_Category, dim_Customer, dim_Location).

Optimization via VIEWs: Created pre-configured Views in SQL to minimize the volume of data imported into Power BI, eliminating the need for redundant joins within the BI model.

🚀 SQL Analytics & Data Processing
Built optimized SQL Views on top of the fact_Orders and dimension tables to perform advanced analysis:

RFM Segmentation: Grouped customers into behavioral segments (e.g., Champions, At Risk, Lost) using NTILE() and CASE WHEN conditional statements.

MoM Customer Growth: Utilized the LAG() window function to track and measure the monthly growth or decline rate of the active customer base.

Cumulative Sales (Running Total): Calculated the historical growth of sales over time, partitioned by market regions and product categories.

Moving Average: Implemented 3-day and 7-day moving averages to smooth out noise and reveal underlying sales trends.

Granular Product Insights: Identified top-performing products whose individual average sales outperformed their respective sub-category's overall average.

📉 Power BI Modeling & Visualizations
Data Modeling: Designed a robust Snowflake Schema with 1-to-Many relationships to ensure clean, high-performance data filtering.

Visualizations & Interactivity:

Line & Area Charts: Deployed to visualize moving averages and cumulative sales dynamics.

Slicers: Enabled dynamic filtering by RFM segments, geographical regions, and product hierarchies.

Leaderboards: Developed rankings to showcase top products exceeding their sub-category averages.
<img width="872" height="495" alt="1" src="https://github.com/user-attachments/assets/5f2eba5c-e940-4e2b-9597-bd65ec3f7a03" />
<img width="876" height="490" alt="2" src="https://github.com/user-attachments/assets/e31dd4cf-9cdb-495d-abc5-908036cddcab" />
<img width="876" height="490" alt="3" src="https://github.com/user-attachments/assets/c8a07021-2583-419d-a834-afeb8b3ea2a6" />
<img width="878" height="493" alt="4" src="https://github.com/user-attachments/assets/89dc9174-3560-42ba-95e8-94dd293c9cf5" />
<img width="872" height="488" alt="5" src="https://github.com/user-attachments/assets/e8a73f12-21fa-43d8-9c4b-1aa5d0769c85" />
<img width="875" height="490" alt="6" src="https://github.com/user-attachments/assets/4062b9e6-f301-444f-883d-6565c5e7f983" />
<img width="875" height="486" alt="7" src="https://github.com/user-attachments/assets/10f5f5c4-ad5e-41c6-93fa-221a9fa12e65" />
<img width="875" height="487" alt="8" src="https://github.com/user-attachments/assets/d0d4e8c2-2e5e-49d3-8f9a-5dd78d283434" />
<img width="875" height="488" alt="9" src="https://github.com/user-attachments/assets/442a25ed-127d-4240-8101-e2de9b5ded8c" />


