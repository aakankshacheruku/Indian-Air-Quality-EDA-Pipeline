# CPCB Air Quality Time-Series Analysis ($PM_{2.5}$)
An end-to-end Python time-series EDA investigating **31,000+ hourly $PM_{2.5}$ particulate readings** across India to analyze diurnal rush-hour congestion patterns and seasonal atmospheric trends.
---
## Context & Motivation
Visiting family in Hyderabad during monsoon season highlighted unusual atmospheric patterns—minimal rainfall, high heat/humidity, and intense short-distance traffic delays (5–7 km). This project explores Central Pollution Control Board (CPCB) data using Python and Pandas to evaluate how hourly traffic and seasonal changes impact local $PM_{2.5}$ concentrations.
---
## Key Analytical Findings
* **Evening Rush-Hour Spike:** $PM_{2.5}$ peaks between **5:00 PM – 7:00 PM** (~54.3 µg/m³), driven by heavy evening commuter traffic and cooling ground temperatures trapping vehicular exhaust.
* **Monsoon Clean-up vs. Winter Inversion:** July and August drop to yearly lows (~21.7 µg/m³) due to rain washing out particulates, while January surges to **79.1 µg/m³** due to winter thermal inversion.
* **Weekday Consistency:** $PM_{2.5}$ averages stay nearly flat across weekdays (~46 to 48 µg/m³), highlighting steady baseline urban emissions.
---
## Tech Stack & Methods
* **Language & Libraries:** Python, Pandas, Seaborn, Matplotlib
* **Data Wrangling:** String-to-datetime parsing (`pd.to_datetime`), missing value auditing, temporal feature extraction (`Hour`, `Month`, `Day_of_Week`)
* **Aggregation:** `.groupby()` time-series aggregations
* **Visualization:** Dual-panel Seaborn line and bar charts with updated palette handling
