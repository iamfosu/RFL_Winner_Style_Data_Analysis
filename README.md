# 📊 Sales & Operations Planning (S&OP) Executive Dashboard

A comprehensive, production-ready **Sales and Operations Planning (S&OP)** analytical dashboard built entirely in Microsoft Excel. This project bridges supply chain management with data analytics, focusing on robust data quality auditing, mathematical formula validation, and interactive executive reporting.

---

## 🚀 Executive Summary
Effective S&OP balancing is vital for mitigating stockouts, managing working capital, and aligning market demand with inventory constraints. This project features a rigorous data quality audit of a multi-variable operational dataset, resolving forecast error inconsistencies, refining dynamic inventory gap tracking, and delivering a clean, executive-level Power BI-style Excel dashboard.

---

## 🛠️ Key Technical & Supply Chain Highlights

* **Advanced Formulas & Logic Validation**: 
  * Implemented absolute error normalization (`=ABS()`) to resolve sign discrepancies in forecast error calculations.
  * Maintained directional `+/-` indicators in **Inventory Gap** (`Inventory Level - Demand Forecast`) to accurately segregate surplus inventory from critical stockouts.
  * Designed dynamic conditional rules for **Stock Status** and automated **Suggested Reorder Quantities**.
* **Data Quality Audit & Correction**: Cleaned raw dataset structures, standardized unit-based metrics, and corrected misaligned KPI card formats.
* **Executive Visualization & Layout**: 
  * Real-time KPI summary cards (*Net Sales Value*, *Total Unit Sold*, *Avg Discount*, *Inventory Units*, and *Avg Forecast Accuracy*).
  * Multi-dimensional performance tracking across regions, product categories, seasonal trends, and competitor pricing tiers (`Higher`/`Lower`/`Same`).

---

## 📈 Dashboard Preview
![S&OP Executive Dashboard](Dashboard/sop_dashboard_view.png)

---

## 📂 Repository Architecture

```text
├── Data/
│   ├── raw_dataset.csv            # Original uncleaned dataset with logical flaws
│   └── cleaned_sop_dataset.xlsx   # Audited & formula-validated dataset
├── Dashboard/
│   ├── sop_dashboard_view.png     # High-resolution screenshot of the final dashboard
│   └── sop_model.xlsx             # Complete Excel workbook with Pivot Tables & Slicers
└── README.md                      # Project documentation
