# 🌊 River Thames Water Level Analysis (Time Series Study)

## 📌 Project Overview
This project analyzes historical water level data from the River Thames at London Bridge. The dataset captures tidal measurements over time, allowing us to explore patterns in high and low tides, statistical behavior, and extreme water level events.

The goal is to apply time series data handling, statistical analysis, and feature extraction techniques to better understand tidal behavior.

Dataset source: British Oceanographic Data Centre.

---

## 🛠️ Tools & Libraries
- Python 🐍  
- Pandas  

---

## 📁 Dataset Description

The dataset (`10-11_London_Bridge.txt`) contains three main variables:

| Variable | Description |
|----------|-------------|
| datetime | Timestamp of measurement (GMT) |
| water_level | Measured tide level (metres) |
| flag | Tide indicator (1 = high tide, 0 = low tide) |

---

## 🔧 Data Preparation

The dataset was cleaned and structured for analysis:
- Converted datetime column to proper datetime format
- Converted water level to float
- Extracted year from timestamp
- Split data into high tide and low tide subsets

```python
london_Bridge_sm["datetime"] = pd.to_datetime(london_Bridge_sm["datetime"])
london_Bridge_sm["water_level"] = london_Bridge_sm["water_level"].astype(float)
london_Bridge_sm["year"] = london_Bridge_sm["datetime"].dt.year