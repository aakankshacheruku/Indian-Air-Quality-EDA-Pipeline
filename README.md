# CPCB Air Quality Time-Series Analysis (PM2.5)

An end-to-end Python time-series exploratory data analysis investigating 31,000+ hourly PM2.5 particulate readings across India to analyze diurnal rush-hour congestion patterns and seasonal atmospheric trends.

---
## Context & Motivation

Visiting family in Hyderabad during monsoon season highlighted unusual atmospheric patterns—minimal rainfall, high heat and humidity, and intense short-distance traffic delays across 5–7 km distances. This project explores Central Pollution Control Board (CPCB) data using Python and Pandas to evaluate how hourly traffic and seasonal changes impact local PM2.5 concentrations.

---
## Key Analytical Findings

* Evening Rush-Hour Spike: PM2.5 peaks between 5:00 PM and 7:00 PM (reaching ~54.3 µg/m³), driven by heavy evening commuter traffic and cooling ground temperatures trapping vehicular exhaust near the surface.
* Monsoon Clean-up vs. Winter Inversion: July and August drop to yearly lows (~21.7 µg/m³) due to rain washing out particulates, while January surges to 79.1 µg/m³ due to winter thermal inversion.
* Weekday Consistency: PM2.5 averages stay nearly flat across weekdays (holding steady around 46 to 48 µg/m³), highlighting constant baseline urban emissions.

---
## Tech Stack & Methods

* Language & Libraries: Python, Pandas, Seaborn, Matplotlib
* Data Wrangling: String-to-datetime parsing (`pd.to_datetime`), missing value auditing, temporal feature extraction (`Hour`, `Month`, `Day_of_Week`)
* Aggregation: Time-series `.groupby()` aggregations
* Visualization: Dual-panel Seaborn line and bar charts with updated palette handling
