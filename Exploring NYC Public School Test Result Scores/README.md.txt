# 🎓 NYC Public School SAT Performance Analysis

## 📌 Project Overview
This project analyzes SAT performance across New York City public schools using real educational data.

The SAT (Scholastic Assessment Test) is a standardized exam used for college admissions in the United States. It consists of three sections:
- Math
- Reading
- Writing  
(each scored out of 800)

The goal of this project is to explore school performance, identify top schools, and analyze differences across NYC boroughs.

---

## 🎯 Objectives
In this project, we aim to answer three key questions:

1. Which schools are the best for math performance?
2. Which schools have the highest overall SAT scores?
3. Which NYC borough shows the greatest variation in SAT performance?

---

## 🛠️ Tools & Libraries
- Python 🐍  
- Pandas  

---

## 📁 Dataset Description

The dataset used is `schools.csv`, which contains SAT performance data for NYC public schools.

| Column | Description |
|--------|-------------|
| school_name | Name of the school |
| average_math | Average SAT Math score |
| average_reading | Average SAT Reading score |
| average_writing | Average SAT Writing score |
| borough | NYC borough where the school is located |

---

## 🔍 Data Preparation

We first loaded and inspected the dataset:

```python
import pandas as pd

schools = pd.read_csv("schools.csv")
schools.head()