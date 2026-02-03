# Forecasting and Cancellation Trends Dashboard

## Overview

This report analyzes hotel booking performance by combining booking demand forecasting, occupancy trend analysis, and cancellation behavior. The solution integrates Python-based forecasting with Power BI analytics to provide actionable insights for short-term planning and operational decision-making.

---

## Forecasting Approach

### Booking Forecast (Python)

* A monthly bookings table was created using:

  * Month End Date
  * Total Bookings
* Booking forecasting was performed in Python using Facebook Prophet.
* Prophet was chosen for its ability to:

  * Capture underlying trends
  * Provide confidence intervals to reflect uncertainty

**Forecast Outputs**

* yhat – Predicted bookings
* yhat_lower – Lower confidence bound
* yhat_upper – Upper confidence bound

The forecasted results were exported as a CSV file and imported into Power BI for visualization.

---

### Occupancy % Forecast (Power BI)

* Occupancy percentage forecasting was performed directly in Power BI using the Analytics → Forecast feature.
* Power BI applies exponential smoothing techniques for short-term trend projection.
* Forecasted occupancy was compared with actual historical occupancy to evaluate trend consistency.

This approach supports short-term operational planning without assuming long-term seasonality.

---

## Cancellation and No-Show Analysis Logic

### Cancellation Rate

Cancellation Rate was calculated using a DAX measure:

Cancellation Rate (%) = (Cancelled Bookings / Total Bookings) × 100

* Calculated dynamically using Power BI measures
* Analyzed across time (monthly) and hotel type (City Hotel vs Resort Hotel)

### No-Show Analysis

* No-shows were aggregated by month and analyzed alongside cancellation rate
* This combined analysis helps differentiate between advance cancellations and guests who fail to arrive

---

## Key Insights from Forecasting and Trend Analysis

* Monthly booking forecasts show moderate variation in future demand rather than sharp seasonal spikes
* Forecast confidence intervals widen over time, indicating increasing uncertainty
* Actual daily occupancy shows short-term fluctuations, while forecasted occupancy follows a stable trend
* Cancellation rates vary independently of booking volume
* No-show behavior does not always align with cancellation trends, indicating distinct customer behaviors

---

## Business Implications

### Demand and Capacity Planning

* Monthly booking forecasts support inventory and staffing decisions
* Occupancy forecasts assist with short-term operational planning

### Revenue Risk Management

* Higher cancellation and no-show periods indicate potential revenue leakage
* Insights can support overbooking strategies and cancellation policy adjustments

### Decision Support Under Uncertainty

* Forecast confidence intervals highlight risk levels
* Enables proactive decision-making rather than reactive responses

---

## Assumptions and Limitations

* Forecasting was performed with limited historical data
* Long-term and yearly seasonality conclusions were intentionally avoided
* Power BI occupancy forecasting is suitable for short-term analysis only

---

## Tools and Technologies

* Python (Prophet) – Monthly booking forecasting
* Power BI – Occupancy forecasting, DAX calculations, and dashboards
* CSV Integration – Forecast outputs imported into Power BI

---

## Conclusion

By combining Python-based booking forecasts with Power BI occupancy and cancellation analysis, this project provides a realistic and business-focused view of hotel demand, booking reliability, and operational risk.
