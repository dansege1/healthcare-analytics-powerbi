# healthcare-analytics-powerbi
Multi-State Healthcare Analytics Dashboard built with Power BI
# 🏥 Multi-State Healthcare Analytics Dashboard (Power BI)

An executive-level, 5-page Power BI analytics platform built for a multi-state hospital network in Nigeria. This end-to-end solution provides deep visibility into patient demographics, facility operations, financial health, and service quality metrics.

---

## 📌 Executive Summary & Key Highlights
* **Star Schema Architecture:** Star schema data modeling connecting visit facts to state, department, service, and date dimensions.
* **DAX & KPI Engine:** Dedicated measures table computing core metrics including Revenue, Cost, Profit Margins (%), Waiting Times, and Satisfaction Scores.
* **Interactive Navigation:** Full-width dark navy header banner with a horizontal Page Navigator across all 5 report pages.

---

## 📊 Dashboard Structure & Pages

1. **Executive Overview:** High-level network KPIs, state revenue distribution, and operational metrics.
2. **Patient Analysis:** Demographic breakdowns (age groups, gender, diagnosis patterns, and volume metrics).
3. **Hospital Operations:** Service demand trends, department cost drivers, and queue wait-time bottlenecks.
4. **Financial Performance:** Revenue trends vs. cost over time, profit margins by unit, and payment method distribution.
5. **Patient Experience:** Satisfaction score tracking across states/departments and service quality correlations.

---

## 🛠️ Data Architecture & DAX Measures
* **Data Model:** Star Schema model with a centralized `_Measures` table.
* **Key DAX Formulas:**
  * `Total Revenue = SUM(Patient_Visits[Revenue_NGN])`
  * `Total Cost = SUM(Patient_Visits[Cost_NGN])`
  * `Total Profit = [Total Revenue] - [Total Cost]`
  * `Profit Margin = DIVIDE([Total Profit], [Total Revenue], 0)`
  * `Average Waiting Time = AVERAGE(Patient_Visits[Waiting_Time_Mins])`
  * `Average Satisfaction = AVERAGE(Patient_Visits[Satisfaction_Score])`

---

## 🖼️ Dashboard Screenshots

| Page | Preview |
| :--- | :--- |
| **1. Executive Overview** | ![Executive Overview](docs/dashboard_overview.png) |
| **2. Patient Analysis** | ![Patient Analysis](docs/patient_analysis.png) |
| **3. Hospital Operations** | ![Hospital Operations](docs/hospital_operations.png) |
| **4. Financial Performance** | ![Financial Performance](docs/financial_performance.png) |
| **5. Patient Experience** | ![Patient Experience](docs/patient_experience.png) |

---

## 🚀 How to View
1. Download `Healthcare_Analytics_Dashboard.pbix` from this repository.
2. Open in **Power BI Desktop** (latest version recommended).
