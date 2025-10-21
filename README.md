This repository contains a **mini-project simulating fraud detection in a parcel delivery platform** similar to Snapp Box. The goal is to create a realistic environment to practice **data analysis, anomaly detection, and reporting** for delivery services.

---

## 🎯 Project Goal
- Simulate a delivery service dataset for analysis purposes.
- Identify potential **fraudulent driver behaviors** such as:
  - High cancellation rate
  - Extremely short or unusual trips
  - Repeated trips with the same origin and destination
- Provide an environment for **SQL and Python practice** in fraud detection.

---

## 📦 Dataset Overview
The dataset is **synthetically generated**, meaning it is **not real user data** but simulates realistic scenarios for practice. It represents **drivers, rides, and payments** over a period of 3 weeks.

---

## 🔹 Dataset Dictionary

| Column Name       | Type        | Description                                                   | Example |
|------------------|------------|---------------------------------------------------------------|---------|
| `driver_id`       | String     | Unique ID for each driver                                     | D001    |
| `ride_id`         | String     | Unique ID for each ride                                       | R0001   |
| `pickup_time`     | DateTime   | Ride start time                                               | 2025-10-01 08:15:00 |
| `dropoff_time`    | DateTime   | Ride end time                                                 | 2025-10-01 08:40:00 |
| `trip_distance`   | Float      | Distance of the trip in kilometers                             | 12.5    |
| `trip_duration`   | Int        | Duration of the trip in minutes                                 | 25      |
| `status`          | String     | Ride status: `completed`, `canceled`, or `suspicious`        | completed |
| `payment_amount`  | Float      | Fare amount paid for the ride                                  | 50.0    |
| `rating`          | Int        | Customer rating for the driver (1–5)                           | 5       |
| `fraud_flag`      | Int        | 0 = Normal ride, 1 = Suspicious/fraudulent ride               | 1       |

---

## ⚙️ Dataset Creation
- **Number of drivers:** 200  
- **Number of rides:** 3000  
- **Time period:** 21 days  
- **Fraud rules simulated:**
  - Canceled rides flagged as suspicious with 30% probability
  - Very short trips (<2 km or <5 minutes) flagged as suspicious
  - Normal rides labeled as completed

This synthetic approach ensures **data privacy** while still reflecting realistic patterns that could occur in a delivery service like Snapp Box.

---

## 📊 Hypothetical Analysis Scenarios
You can practice or demonstrate the following analyses using this dataset:

1. **Driver Fraud Detection:** Identify drivers with unusual patterns (high cancellation rate, very short trips, repeated locations).  
2. **Outlier Detection:** Use statistical methods or visualization to find anomalous rides.  
3. **Aggregated Reporting:** Calculate metrics like average trip distance, duration, payment, and number of suspicious rides per driver.  
4. **Visualization:** Plot distributions of trip distance, duration, canceled trips, or suspicious trips to explore patterns.  
5. **SQL Practice:** Run queries to filter suspicious rides, group by driver, or calculate ratios.

---
