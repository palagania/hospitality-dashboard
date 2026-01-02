📊 Hospitality Analytics Dashboard (Power BI)

    This project analyzes hotel booking trends, revenue performance, occupancy, cancellations, and customer behavior using a structured end-to-end Exploratory Data Analysis (EDA) workflow.
    It was completed as part of Codebasics: Data Analytics Roadmap – Project 1 (Hospitality Domain).

📘 Project Overview

    This project analyzes hotel booking data to uncover insights into revenue, occupancy, cancellations, customer ratings, room category behavior, and booking trends.
    It follows an end-to-end EDA workflow, inspired by Codebasics – Project 1 (Hospitality Domain) by Dhaval Patel.

    The final deliverable is an interactive Power BI dashboard presenting key KPIs, trends, and business insights for stakeholders.

🔍 Objectives

     Perform EDA on raw hospitality booking data

     Build a consistent analytical dataset using ETL steps

     Implement a clean Star Schema (Fact + Dimension Tables)

     Write DAX measures for KPIs and business insights

     Design a professional, intuitive Power BI dashboard

     Enable dynamic exploration using slicers and interactions

🛠 Tech Stack & Tools

    Power BI, Power Query / M, DAX, Excel / CSV, ETL & Data Modeling, Star Schema Design

🧹 Data Cleaning & Transformation Workflow

    Inspected missing values, outliers, data inconsistencies

     Corrected data types, standardized categories

     Generated derived fields (weekday/weekend, month-year, week number, rating groups)

     Created a Date Dimension with the proper hierarchy

     Merged and shaped fact + dimensions

     Built a semantic model optimized for reporting

📈 Core DAX Measures (Examples)

     Total Revenue =
     SUM(bookings_clean_data[revenue_realized])

     Total Bookings =
     COUNTROWS(bookings_clean_data)

     Total Guests =
     SUM(bookings_clean_data[no_guests])

     Average Rating =
     AVERAGE(bookings_clean_data[rating])

     Booking Occupancy Rate =
     DIVIDE(SUM(bookings_clean_data[no_guests]),
       SUM(bookings_clean_data[successful_bookings]))

     Weekend Revenue =
     CALCULATE(
    SUM(bookings_clean_data[revenue_realized]),
    WEEKDAY(bookings_clean_data[check_in_date], 2) >= 6
     )

     Weekday Revenue =
     CALCULATE(
    SUM(bookings_clean_data[revenue_realized]),
    WEEKDAY(bookings_clean_data[check_in_date], 2) <= 5
     )


📊 Dashboard Highlights

       KPI Summary, Total Revenue, Total Bookings, Average Rating, Total Guests, Occupancy Rate
  
2. Trend Analysis

       Monthly Revenue Trend, Booking Trend Over Time, Customer Rating Trends

3. Room & City Insights

       Revenue by Room Category, Revenue by City, Occupancy comparison by category

4. Customer Behavior Metrics

       Weekday vs Weekend performance, Booking Platform Share, Cancellation Patterns

5. Interactive Slicers

       Month / Year, Week, Room Category, City, Booking Platform

🖼 Dashboard Preview

<img width="1373" height="800" alt="Screenshot 2025-12-10 124146" src="https://github.com/user-attachments/assets/787925c3-851a-4ed4-bc54-a10b32299e88" />

📂 Repository Structure

     hospitality-dashboard/
     │
     ├── Hospitality_Analysis.pbix
     ├── README.md
     └── assets/
    ├── dashboard_main.png
    ├── kpi_section.png
    └── city_revenue.png

Codebasics Data Analytics Roadmap
Instructor: Dhaval Patel
Course Link: https://codebasics.io

🙋 Author

Abhinash Palagani
GitHub: https://github.com/palagania

LinkedIn: https://www.linkedin.com/in/abhinash-palagani-47a881193/

