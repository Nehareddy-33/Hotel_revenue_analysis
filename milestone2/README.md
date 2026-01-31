# Milestone 2

## Overview

This Power BI dashboard provides a comprehensive analysis of hotel booking performance, focusing on **Revenue, Occupancy, Booking Trends, and Guest Behavior**. The dashboard is designed to help stakeholders understand business performance across time, channels, seasons, and guest segments, enabling data-driven decisions.

The report is divided into **two main sections**:

1. **Revenue and Occupancy Analysis**
2. **Guest Analysis**

##  Data Scope

The dashboard is built using hotel booking data containing information such as:

* Booking date (day, month, year)
* Number of bookings
* Revenue
* Occupancy and ADR metrics
* Booking channel (Direct, OTA)
* Hotel type (City Hotel, Resort Hotel)
* Room category
* Guest type, frequency, and country
* Stay duration

---

## Report 1: Revenue and Occupancy Analysis

### Revenue & Occupancy Metrics Explained

* **Occupancy %**: Calculated as the ratio of occupied rooms to total available rooms. It indicates how effectively hotel capacity is utilized.
* **Average Daily Rate (ADR)**: Represents the average revenue earned per occupied room. It is calculated as total room revenue divided by the number of occupied rooms.
* **RevPAR (Revenue per Available Room)**: Measures overall revenue performance by combining occupancy and pricing. It is calculated as total room revenue divided by total available rooms.

These three metrics together provide a holistic view of hotel performance—balancing volume (occupancy) and value (pricing).

### Key KPIs

* **Occupancy %** – Percentage of occupied rooms over available rooms
* **Average Daily Rate (ADR)** – Average revenue earned per occupied room
* **RevPAR** – Revenue per available room

These KPIs provide a high-level snapshot of hotel performance.

### Visual Insights

* **Total Bookings by Day**: Daily booking trend to identify demand fluctuations
* **Total Bookings by Year and Month**: Monthly trend analysis to observe growth and seasonality
* **Total Bookings by Season**: Comparison of bookings across Winter, Summer, and Spring
* **Total Bookings by Booking Channel**: Distribution of bookings between Direct and OTA channels
* **Revenue by Booking Channel**: Comparison of revenue contribution from each channel

### Filters & Slicers

* Hotel Name (City Hotel / Resort Hotel)
* Room Category
* Booking Channel

These slicers allow users to drill down into specific segments.

---

## Report 2: Guest Analysis

### Guest Classification & Segmentation Logic

Guests are segmented using booking characteristics to better understand behavior and value:

* **Guest Type**:

  * *Business Guests*: Typically shorter stays, often mid-week bookings
  * *Leisure Guests*: Longer stays, commonly during weekends or holidays

* **Guest Frequency**:

  * *One-time Guest*: Single booking
  * *Repeat Guest*: 2–3 bookings
  * *Loyal Guest*: More than 3 bookings

* **Stay Type (based on booking duration)**:

  * *Short Stay*: 1–2 nights
  * *Medium Stay*: 3–5 nights
  * *Long Stay*: More than 5 nights

This segmentation helps identify high-value and loyal customers, as well as different travel behaviors across regions.

###  Guest Segmentation

Guests are classified based on booking characteristics such as:

* **Guest Type**: Business vs Leisure
* **Guest Frequency**:

  * One-time Guest
  * Repeat Guest
  * Loyal Guest
* **Stay Type**:

  * Short Stay
  * Medium Stay
  * Long Stay

### Visual Insights

* **Total Bookings by Guest Type**: Share of business vs leisure guests
* **Total Bookings by Guest Frequency**: Distribution of one-time, repeat, and loyal guests
* **Geographical Map**: Revenue and ADR by Guest Country, segmented by guest frequency
* **Bookings by Country and Stay Type**: Comparison of stay duration patterns across countries

### Filters & Slicers

* Booking Channel

These help analyze guest behavior by booking source.

##  Business Value

### Key Insights & Observations

* **Occupancy remains strong** while ADR fluctuations indicate seasonal pricing strategies.
* **Direct bookings generate higher revenue** compared to OTA, highlighting the importance of direct channels.
* **Repeat guests form the majority of bookings**, indicating good customer retention.
* **Leisure guests dominate overall bookings**, especially during peak seasons.
* **Certain countries contribute higher revenue with longer stays**, making them key target markets.
* **Loyal guests show higher ADR and revenue contribution**, emphasizing the value of loyalty programs.

These insights support decisions related to pricing, marketing focus, guest retention strategies, and regional targeting.

This dashboard helps stakeholders to:

* Identify peak seasons and demand patterns
* Compare performance across booking channels
* Understand guest behavior and loyalty
* Analyze geographical distribution of high-value guests
* Support pricing, marketing, and capacity planning decisions

---

##  Tools & Technologies

* **Power BI Desktop** – Data modeling and visualization
* **DAX** – Measures and calculated columns for KPIs and segmentation
* **Power Query** – Data cleaning and transformation

---

## Usage Instructions

1. Open the `.pbix` file in Power BI Desktop
2. Use slicers to filter data by hotel, room category, and channel
3. Hover over visuals to view detailed tooltips
4. Analyze trends across both report pages for insights

---

## Future Enhancements

* Add forecasting for bookings and revenue
* Introduce guest lifetime value (LTV)
* Include cancellation and no-show analysis
* Add dynamic targets and KPI comparisons

---

## Author

**Nehasri Anumula**
Aspiring Data Analyst | Power BI Enthusiast

---

✅ *This dashboard is created as part of a data analytics learning project and demonstrates end-to-end analysis using Power BI.*
