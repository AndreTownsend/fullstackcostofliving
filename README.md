# 🌍 Inflation in the Digital Age — Economic Pressure Analysis

## 📌 Executive Summary
This project analyzes the impact of inflation on real wages and cost of living across major global economies from 2015 to 2023. By combining World Bank data with wage growth and housing cost indicators, the analysis introduces an **Economic Pressure Index** to measure how inflation, rent, and wage stagnation affect consumers.

The results highlight widening economic pressure in developed economies, particularly where inflation outpaces wage growth.

---

## ❗ Business Problem
Rising inflation has become a global concern, but its real impact depends on how wages and living costs respond.

**Key Questions:**
- Are wages keeping up with inflation?  
- Which countries are experiencing the most financial pressure?  
- How do housing costs amplify economic stress?  
- What trends define the modern cost-of-living crisis?  

---

## ⚙️ Methodology

### 📡 Data Sources
- World Bank API (`wbgapi`)
  - Inflation (CPI)
  - GDP per capita
  - Unemployment rate  
- Simulated / supplemental datasets:
  - Wage growth (selected countries)
  - Housing cost index & rent %

---

### 🔧 Data Processing
- Merged datasets using country + year keys  
- Calculated:
  - **Real Wage Growth = Wage Growth − Inflation**
  - **Wage Squeeze Indicator** (negative real wage)
  - **Cumulative Real Wage Growth** over time  

---

### 📊 Economic Pressure Index (2023)
A custom index combining:
- Inflation (40%)  
- Rent burden (30%)  
- Negative real wage pressure (30%)  

Normalized and scaled to 0–100.

---

### 🗄️ Data Engineering
- Stored structured data in **SQLite database**
- Queried using SQL for aggregated insights

---

## 📊 Key Visualizations

### 📈 Cumulative Real Wage Growth
```markdown
![Real Wage Growth](your_line_chart.png)

![Economic Pressure Map](your_map.png)
