# Talent Acquisition Analytics Dashboard

A Power BI recruitment analytics dashboard built from a 2,400-row dataset spanning 11 departments and FY 2022–2023. The project covers end-to-end data preparation, modelling, and visualisation to surface actionable hiring insights.

---

## 📊 Dashboard Overview

| KPI | Value |
|---|---|
| Total Applications | 2,400 |
| Total Hired | 397 |
| Hire Rate | 19.95% |
| Offer Acceptance Rate | 49.87% |
| Average Time to Fill | 26.78 days |

---

## 🗂️ Project Structure

```
├── Data Preparation     # Power Query — null handling, imputation, data cleaning
├── Data Model           # Star schema — 1 fact table, 3 dimension tables
├── DAX Measures         # KPIs — Time to Fill, Hire Rate, Offer Acceptance Rate
└── Dashboard            # Power BI — 5 visuals + slicers + KPI cards
```

---

## 🔧 Data Model

| Table | Type | Primary Key |
|---|---|---|
| `Fact_Recruitment` | Fact | `Candidate_ID` + `Open Position` |
| `Dim_Candidate` | Dimension | `Candidate_ID` |
| `Dim_Department` | Dimension | `Department_ID` |
| `Dim_Position` | Dimension | `Open Position` |

---

## 🛠️ Tools Used

- **Microsoft Excel** — Power Query for data cleaning and transformation
- **Power BI Desktop** — Data modelling, DAX measures, and dashboard visualisation

---

## 💡 Key Findings

- Offer acceptance rate is critically low at **49.87%** — IT (16%) and HR (40%) are the worst performing departments
- **54.22%** of all candidates failed the recruitment process indicating weak shortlisting
- **Capacity Building** leads with a 40% hire rate and 72% offer acceptance rate
- Application volumes peak in **March–April** and drop sharply in June
- **IT department** requires urgent intervention with only a 6% hire rate

---

## 📁 Files

| File | Description |
|---|---|
| `recruitment_dataset.xlsx` | Raw source data |
| `recruitment_cleaned.xlsx` | Cleaned data with imputed dates and flag columns |
| `TalentAcquisitionAnalytics.pbix` | Power BI dashboard file |

---

## 👤 Author
Built as part of an HR analytics project to improve data-driven recruitment decision-making.
