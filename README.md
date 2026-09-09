# 🚕 Uber Trip Analysis Dashboard | Power BI

An end-to-end business intelligence solution built in **Power BI**, analyzing Uber trip data to uncover booking trends, revenue patterns, trip efficiency, and location-based demand — enabling stakeholders to make faster, data-driven operational decisions.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

## 📌 Project Overview

Uber generates massive volumes of trip data every day — bookings, cancellations, distances, payment types, pickup and drop-off points. Buried in this data are answers to critical business questions: *When does demand peak? Which locations drive the most trips? How efficient are rides in terms of time and distance? Where is revenue being generated, and how?*

This project transforms raw trip-level data into a **3-page interactive Power BI dashboard**, moving from a high-level operational overview down to granular, record-level detail — giving both executives and analysts the view they need.

---

## 🎯 Business Objectives

- Track booking volume and revenue trends over time
- Measure trip efficiency (distance & duration)
- Understand demand patterns by time, day, and location
- Identify high-value locations and vehicle preferences
- Enable self-service, drill-through exploration of raw trip records

---

## 📊 Dashboards

### 1️⃣ Overview Analysis
The command-center view of the business — key metrics and comparative breakdowns.

- **Core KPIs:** Total Bookings, Total Booking Value, Average Booking Value, Total Trip Distance, Average Trip Distance, Average Trip Time
- **Dynamic Measure Selector** — a disconnected-table-driven toggle that lets users switch the entire dashboard's focus between Bookings, Revenue, and Distance, with the chart title updating dynamically to match
- **Payment Type & Trip Type breakdowns** (Card/Cash/Wallet, Day/Night)
- **Vehicle Type Performance Grid** — a matrix visual comparing KPIs across vehicle categories, with conditional formatting to instantly flag high/low performers
- **Total Bookings by Day** — trend and anomaly detection for demand planning
- **Location Intelligence** — most frequent pickup & drop-off points, farthest trip, top 5 locations by booking volume, and most preferred vehicle type per pickup location
- **UX Enhancements** — a "Data Details" bookmark panel explaining every metric, a one-click "Clear Filters" reset button, and a raw data export option

### 2️⃣ Time Analysis
A deep dive into *when* demand happens.

- **Global Dynamic Measure** — the same toggle logic from Dashboard 1, applied here to drive every time-based visual
- **10-Minute Interval Area Chart** — pinpoints peak and off-peak windows within a single day
- **Day-of-Week Line Chart** — compares weekday vs. weekend demand
- **Hour × Day Heatmap** — a matrix visual (hours 0–23 vs. Mon–Sun) that instantly surfaces the busiest booking windows across the week

### 3️⃣ Details Tab
The analyst's playground — full transparency into the underlying data.

- **Grid Table** with essential trip-level fields
- **Drill-Through Functionality** — right-click any data point on the other two dashboards to jump straight to its underlying records
- **"View Full Data" Bookmark** — toggle instantly between filtered drill-through results and the complete dataset

---

## 🛠️ Technical Highlights

This project goes beyond basic charting — it demonstrates practical, production-style Power BI skills:

| Technique | Why It Matters |
|---|---|
| **Disconnected table + dynamic DAX measure** | Lets one set of visuals serve three different analytical purposes without duplicating charts |
| **Dynamic chart titles** | Visuals communicate exactly what they're showing at any given moment, with zero manual updates |
| **Activated inactive relationship** (Pickup ↔ Drop-off) | Solves a common Power BI modeling challenge — using `USERELATIONSHIP` to analyze the same location field in two different roles |
| **Bookmarks + buttons** | Simulates app-like navigation and interactivity (data glossary panel, filter reset, full-data toggle) |
| **Drill-through pages** | Connects summary-level insight to record-level detail in a single click |
| **Conditional formatting** | Turns a plain table into an at-a-glance performance grid |

---

## 🧰 Tools & Technologies

- **Power BI Desktop** — data modeling, visualization, dashboard design
- **DAX** — dynamic measures, calculated KPIs, relationship handling
- **Power Query** — data cleaning and transformation

---

## 📂 Repository Structure

```
uber-trip-analysis-powerbi/
│
├── README.md
│
├── data/
│   └── location table.xlsx
|   └── uber trip details.xlsx
│
├── powerbi/
│   └── dashboard.pbix
│
└── screenshots/
|   ├── overview-analysis.png
|   ├── time-analysis.png
|   └── details.png
│
├── report/
│   └── project_report


---

## 📸 Dashboard Previews

> _Screenshots to be added_

| Overview | Time Analysis | Details Tab |
|---|---|---|
| ![Overview](screenshots/overview-analysis.png) | ![Time Analysis](screenshots/time-analysis.png) | ![Details](screenshots/details.png) |

---

## 🔑 Key Takeaways / Business Impact

- Enables data-driven pricing and driver-allocation decisions by exposing peak-demand hours and high-traffic locations
- Reduces time-to-insight by letting stakeholders self-serve through slicers, bookmarks, and drill-through rather than requesting custom reports
- Demonstrates a scalable dashboard architecture (dynamic measure selector) that can extend to additional KPIs without rebuilding visuals

---

## 📬 Contact

**Sowmya Sanikommu**
Feel free to connect for feedback, collaboration, or questions about this project.
