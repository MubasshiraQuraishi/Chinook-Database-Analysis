This repository contains SQL queries, analyses, and stored procedures built on the **Chinook sample database** – a popular dataset that simulates a digital media store.

### 🔎 Database Overview

* **Invoices**: 2240
* **Customers**: 59
* **Employees**: 8
* **Artists**: 275
* **Total Revenue**: \$2328.60

The database includes tables for customers, invoices, invoice lines, employees, tracks, albums, artists, playlists, and genres, making it ideal for practicing **SQL joins, aggregations, window functions, and analytical queries**.

---

### 📊 Key Insights & Queries

* **Sales Trends**: Revenue by year, month, and region
* **Top Performers**: Highest-spending customers, top-grossing artists, best sales agents
* **Genre & Track Analysis**: Most sold genres, tracks that never sold, percentage contribution of each genre
* **Regional Insights**: Revenue distribution by country and city, average invoice value per country
* **Advanced Analytics**:

  * Month-over-Month revenue growth using window functions
  * Best customer per genre
  * Longest tracks in the database
  * Track recommendations using collaborative filtering logic

---

### 🛠️ Featured Stored Procedure

**Track Recommendation (Customers Like You)**
Suggests tracks for a customer (e.g., `CustomerId = 5`) that they haven’t purchased yet, but are popular among other customers who bought the same tracks.

* Implements a collaborative filtering approach
* Joins across invoices, invoice lines, tracks, albums, and artists
* Ranks recommendations by popularity
