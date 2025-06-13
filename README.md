Hotel Management Dashboard – Power BI

This is an end-to-end Business Intelligence project built in Power BI for a hotel management case study. The objective is to analyze hotel operations using various data sources and deliver a dashboard that supports decision-making for revenue, occupancy, customer behavior, and booking trends.

 Objectives
- Load and clean multiple hotel-related datasets
- Model the data using a star schema
- Create DAX measures and calculated columns
- Build an interactive and insightful dashboard


 📁 Files

- HotelDashboard.pbix: Main Power BI file
 -screenshots of the project

 Tools & Technologies
- Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
- Power BI Service


## 📊 Dashboard Overview

### 📌 Key Insights

- Total Revenue, Average Stay, and Occupancy KPIs
- Revenue trends over time
- Room performance by type
- Customer bookings by segment and nationality
- Filterable by date, customer country, and room type

### 📸 Dashboard Screenshot

![Final Dashboard](./screenshots/dashboard.png)

---

## 🔧 Data Model – Star Schema

![Data Model](./screenshots/data-model.png)

---

## 🔍 Data Cleaning & Transformation

Handled using Power Query:

- Removed nulls
- Formatted date columns
- Renamed columns for readability
- Joined multiple datasets

![Transformations](./screenshots/transformations.png)

---

## 🧮 DAX Measures

A few of the custom DAX measures include:

```DAX
Total Revenue = SUM(fact_bookings[Revenue])
Occupancy Rate = DIVIDE([Total Booked Rooms], [Total Available Rooms])
YOY Revenue Change = [This Year Revenue] - [Last Year Revenue]
