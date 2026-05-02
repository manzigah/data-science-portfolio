# 🏈 Super Bowl Data Analysis (52 Years of Football, TV & Halftime Shows)

## 📌 Project Overview
This project explores data from 52 Super Bowls (up to 2018), focusing on game results, TV viewership, and halftime performances. The goal is to identify trends in audience engagement, game competitiveness, and entertainment impact over time.

The datasets are sourced from cleaned Wikipedia data and include three main files:
- Game statistics (`super_bowls.csv`)
- TV viewership data (`tv.csv`)
- Halftime show performances (`halftime_musicians.csv`)

---

## 🛠️ Tools & Libraries
- Python 🐍  
- Pandas  
- Matplotlib  

---

## 📁 Dataset Description

### 1. super_bowls.csv
Contains details about each Super Bowl game:
- Teams
- Scores
- Point differences
- Date and location

### 2. tv.csv
Contains TV-related metrics:
- Average US viewers
- Household ratings
- Advertisement costs

### 3. halftime_musicians.csv
Contains halftime show data:
- Musician or group name
- Number of songs performed
- Super Bowl number

---

## 📊 Key Analysis & Findings

### 📈 Super Bowl Viewership Trend
A line plot was used to visualize how average US viewership has changed over time.

```python
plt.plot(tv["super_bowl"], tv["avg_us_viewers"], marker='o')
plt.xlabel("Super Bowl")
plt.ylabel("Average US Viewers")
plt.title("Super Bowl Viewership Over Time")
plt.show()