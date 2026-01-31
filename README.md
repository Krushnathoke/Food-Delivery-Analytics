# Food Delivery Data Insights & ETL 🍕📉

## 📌 Project Overview
Developed by **Krushna Thoke**, this project focuses on solving complex data integration challenges within a food delivery ecosystem. The objective was to perform an **ETL (Extract, Transform, Load)** process on multi-format datasets—CSV, JSON, and SQL—to build a "Single Source of Truth" and extract actionable business intelligence.

## 📁 Data Sources
To simulate a real-world environment, the data was gathered from three distinct sources:
- **Transactional Data**: `orders.csv` (Order history and transaction amounts)
- **User Master**: `users.json` (Customer demographics and membership tiers)
- **Restaurant Master**: `restaurants.sql` (Cuisine types and service ratings)

## 🛠️ Technical Stack
- **Data Processing**: Python 3.10+
- **Analysis Engine**: Pandas, NumPy
- **Database Connectivity**: SQLite3 (for SQL script parsing)
- **Development Environment**: Jupyter Notebook

## ⚙️ Implementation Steps

### 1. Data Extraction
- Structured flat CSV files into DataFrames.
- Parsed JSON objects to map user profiles.
- Initialized an in-memory SQL database to execute and read the restaurant master records.

### 2. The Merge Strategy
- Applied a **Left Join** on `user_id` to link transactions with specific customer profiles.
- Integrated restaurant details using `restaurant_id` to add cuisine and rating context.
- Resulted in a consolidated dataset of **10,000 records**.

### 3. Business Logic & Analysis
- **Membership Impact**: Evaluated the spending habits of Gold vs. Regular members.
- **Geographic Trends**: Identified Hyderabad and Chennai as high-performance hubs.
- **Seasonality**: Analyzed revenue distribution across four quarters (Q1-Q4).

## 📊 High-Level Insights
- **Gold Loyalty**: Gold members contribute nearly **50%** of total order volume.
- **Premium Cuisines**: **Mexican** cuisine yields the highest Average Order Value (AOV).
- **Service Quality**: Restaurants rated **4.6 - 5.0** generate the maximum revenue share.
- **Peak Performance**: The third quarter (**Q3**) recorded the highest total revenue of the year.



## 🚀 How to Use

Ensure the data files are in the root directory.

Open solution.ipynb in Jupyter Notebook or VS Code.

Execute all cells to reproduce the analysis and exported CSV.

## 🤝 Connect with Me

**Krushna Thoke**
Data Analysis Enthusiast
1. Clone the repository:
   ```bash
   git clone [https://github.com/KrushnaThoke/Food-Delivery-Insights.git](https://github.com/KrushnaThoke/Food-Delivery-Insights.git)
