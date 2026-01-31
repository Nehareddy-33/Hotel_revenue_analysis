# Hotel Revenue Analysis – Power BI Project

# Project Overview

This project focuses on analyzing **hotel performance and revenue trends** using **Power BI Desktop**. The dataset represents **daily aggregated hotel data**, including check-ins, check-outs, ADR, RevPAR, bookings, and cancellations.

The goal of this project is to build a **clean star schema model**, create **meaningful KPIs**, and design an **interactive dashboard** that provides insights into hotel revenue, room categories, seasons, and hotel types (Resort vs City).

---

## Objectives

* Analyze **total and monthly revenue trends**
* Compare performance between **Resort Hotel and City Hotel**
* Understand revenue contribution by **room category**
* Identify **seasonal impact** on revenue
* Apply **proper data modeling (Star Schema)** in Power BI

---

## Dataset Description

The dataset contains **aggregated daily metrics** and does not include guest-level or room-level identifiers.

### Fact Table (fact)

* Revenue
* ADR (Average Daily Rate)
* RevPAR
* Checkins
* Checkouts
* Bookings
* Cancellations
* Available_Rooms
* Average_Review_Score
* booking_duration (derived)

---

## Data Model (Star Schema)

The model follows a **Star Schema design**, where the fact table is connected to multiple dimension tables using **many-to-one relationships**.

### Dimension Tables

#### 📅 Date Dimension

* Date
* Month
* Quarter
* Season

#### 🛏 Room Dimension

* room_id (derived surrogate key)
* room_category (Standard / Deluxe / Premium)

#### 👤 Customer Dimension

* customer_id (single surrogate key for aggregated data)
* Booking_Channel
* Guest_Type
* Guest_Country

#### 🏢 Hotel Branch Dimension

* hotel_id
* hotel_name (Resort Hotel / City Hotel)

All relationships are:

* **Many-to-One (*** → 1)**
* **Single direction filtering**
* **Active relationships**

---

## Data Transformation (Power Query)

Key transformations performed in Power Query Editor include:

* Creating **room_category** using ADR-based conditions
* Creating **room_id** by mapping room categories
* Creating **customer_id** as a constant surrogate key
* Deriving **booking_duration (estimated)**
* Renaming columns for consistency
* Replacing values and filtering rows

---

## Dashboard & Visualizations

### KPIs

* **Total Revenue (Card)**
* **Average ADR**
* **Average RevPAR**

### Visuals Used

* Line chart: Revenue trend by Month & Quarter
* Column chart: Revenue by Hotel Type
* Donut chart: Room Category Revenue Contribution
* Waterfall chart: Revenue by Season
* Bar chart: Revenue comparison between Resort and City Hotel

### Filters & Slicers

* Date
* Hotel Name
* Room Category

---

## Key Insights

* City Hotel generates higher total revenue compared to Resort Hotel
* Deluxe rooms contribute the highest share of revenue
* Revenue shows clear seasonal variation
* ADR-based room categorization provides meaningful segmentation

---

## Tools & Technologies

* **Power BI Desktop**
* **Power Query (M Language)**
* **DAX (Measures)**
* **Star Schema Data Modeling**

---

## Learnings

* Importance of **proper data modeling** in Power BI
* Handling **aggregated datasets** without granular identifiers
* Creating **derived dimensions** safely and transparently
* Building **interview-ready dashboards**

---

## Conclusion

This project demonstrates how to convert aggregated hotel data into a well-structured analytical model and build insightful dashboards using Power BI. It follows industry best practices in data modeling and visualization.

---

## Author

**Nehasri Anumula**
Aspiring Data Analyst | Power BI | SQL | Python



