# 🚖 Ola Data Analysis Project

## 📊 Overview
This project presents an in-depth data analysis of **Ola Cabs** using **Power BI** and **SQL**.  
The main objective is to explore ride trends, customer behavior, revenue distribution, and operational efficiency through insightful dashboards and queries.

---

## 🧠 Objectives
- Analyze ride data to identify peak hours, locations, and user preferences.
- Examine revenue generation and ride frequency patterns.
- Visualize driver and customer performance metrics.
- Build an interactive Power BI dashboard for clear and dynamic reporting.

---

## 🛠️ Tools & Technologies Used
| Tool/Technology | Purpose |
|-----------------|----------|
| **Power BI** | Data visualization and dashboard creation |
| **SQL (MySQL / SQL Server)** | Data cleaning, transformation, and querying |
| **Excel / CSV** | Data preprocessing and import |
| **GitHub** | Version control and project hosting |

---

## 🗃️ Dataset
The dataset contains details about Ola rides such as:
- Ride ID, Date, and Time  
- Pickup and Drop Locations  
- Driver and Customer Details  
- Trip Distance, Duration, and Fare Amount  
- Ratings and Payment Mode  

> *Note: The dataset used is a simulated or anonymized version for academic and analysis purposes.*

---

## 🧩 SQL Analysis
Key SQL queries were used to:
- Calculate total rides per city and time period.  
- Identify top-performing drivers.  
- Analyze average trip fare and distance.  
- Determine peak demand times and cancellation rates.

Example query:
```sql
SELECT city, COUNT(ride_id) AS total_rides, 
       AVG(fare_amount) AS avg_fare
FROM ola_rides
GROUP BY city
ORDER BY total_rides DESC;
