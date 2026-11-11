# 📊 Sales & Operations Planning (S&OP) & Data Quality Audit Dashboard

A comprehensive, executive-ready **Sales and Operations Planning (S&OP)** analytical solution and data quality audit built entirely in Microsoft Excel. This project bridges supply chain management with robust data analytics, focusing on formula optimization, rigorous error normalization, and dynamic business intelligence reporting.

## 📈 Dashboard Preview
![S&OP Executive Dashboard](Dashboard_winner_style.png)

---

## 🎯 Executive Summary & Business Context
Effective Sales and Operations Planning (S&OP) is critical for balancing market demand with inventory constraints, preventing costly stockouts, and optimizing working capital. This project addresses structural and logical flaws in raw operational datasets, implements advanced mathematical validations, and delivers an interactive executive dashboard to drive data-backed supply chain decisions.

---

## 🔍 Data Quality Audit & Analytical Findings
During the initial exploratory data analysis and quality audit of the raw dataset, several critical logic flaws and discrepancies were identified and resolved:

* **Forecast Error Normalization (`ABS` Implementation)**: 
  * *Issue*: The initial formula (`Demand Forecast - Units Sold`) produced negative values (`-5.96`, `-4.74`), which distorted aggregate accuracy metrics due to positive and negative values cancelling each other out.
  * *Resolution*: Implemented absolute error normalization (`=ABS([@[Demand Forecast]]-[@[Units Sold]])`) to ensure consistent, accurate tracking of absolute forecast deviation.
* **Inventory Gap & Stock Status Integrity**: 
  * *Finding*: Maintained directional `+/-` indicators (`Inventory Level - Demand Forecast`) intentionally. This allows the system to clearly distinguish between surplus inventory (Healthy Stock) and critical shortages (Low Stock).
* **UI/UX & Financial Formatting Standards**: 
  * *Issue*: Unit-based KPIs (such as *Total Units Sold*) were incorrectly formatted with currency symbols (`$`), creating misleading business metrics.
  * *Resolution*: Standardized formatting by stripping currency symbols from unit-based KPIs and aligning chart Y-axis baselines to zero to prevent visual distortion.

---

## 📈 Key Insights & Operational Metrics
* **Inventory Optimization**: Identified instances of critical low stock (e.g., Row 7 showing a deficit of `-1.82` units), automatically triggering a **Suggested Reorder Quantity** of `2` units to mitigate stockouts.
* **Sales & Regional Performance**: Tracked total net sales value (`$494.97M`) and regional revenue distribution evenly across East, North, South, and West regions (~25% each).
* **Pricing & Discount Impact**: Evaluated competitor pricing strategies (`Higher`, `Lower`, `Same`) and analyzed discount tier efficiency against total sales value.

---

## 🛠️ Tech Stack & Methodologies
* **Tool**: Microsoft Excel (Advanced Formulas, Pivot Tables, Pivot Charts, Slicers, Conditional Formatting, Custom Number Formatting).
* **Domain Expertise**: Sales & Operations Planning (S&OP), Supply Chain Analytics, Inventory Gap Analysis, and Error Metric Standardization (MAE/Accuracy).

---

## 📂 Repository Structure

```text
├── Winner_Style_Data_Analyst_Assessment_Tarakuzzaman.xlsx   # Audited & formula-validated Excel model
├── Dashboard_winner_style.png                               # High-resolution screenshot of the final dashboard
└── README.md                                                # Project documentation & analytical report
