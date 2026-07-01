# 🌾 PMFBY District-Level Crop Insurance Analysis Dashboard

## 📌 Overview

This project presents an interactive **Power BI dashboard** built using the **Pradhan Mantri Fasal Bima Yojana (PMFBY)** district-level dataset. The dashboard analyzes crop insurance coverage, farmer participation, premium contributions, and demographic distribution across Indian states and districts.

The project demonstrates the complete data analytics workflow, including data preprocessing, data modeling, DAX calculations, and interactive dashboard development.

---

# 🎯 Objectives

- Analyze PMFBY district-level crop insurance data.
- Evaluate farmer participation across states and districts.
- Compare insurance coverage and premium contributions.
- Understand demographic distribution of insured farmers.
- Build an interactive dashboard for data-driven decision-making.

---

# 🛠️ Tools & Technologies

- Microsoft Excel
- Power Query
- Power BI Desktop
- DAX (Data Analysis Expressions)

---

# 📂 Dataset

The dataset includes:

- Year
- Season
- Scheme
- State Name
- District Name
- Farmer Count
- Loanee Farmers
- Non-Loanee Farmers
- Area Insured (Hectares)
- Sum Insured
- Gross Premium
- Farmer Share
- Government of India Share
- State Government Share
- Gender Distribution
- Social Category Distribution
- Farmer Category Distribution

---

# 🧹 Data Preprocessing

Data preprocessing was performed using Microsoft Excel and Power Query.

### Steps Performed

- Removed duplicate records
- Handled missing values
- Corrected data types
- Renamed columns for consistency
- Filtered inactive records
- Verified data quality before loading into Power BI

---

# ⭐ Data Modeling

A **Star Schema** was implemented to improve report performance and simplify filtering.

## Fact Table

- **pmfby-district-level**

## Dimension Tables

- DimYear
- DimState
- DimDistrict
- DimSeason
- DimScheme

### Relationships

| Fact Table | Dimension Table | Cardinality |
|------------|-----------------|-------------|
| Year | DimYear | Many-to-One (*:1) |
| State Name | DimState | Many-to-One (*:1) |
| District Name | DimDistrict | Many-to-One (*:1) |
| Season | DimSeason | Many-to-One (*:1) |
| Scheme | DimScheme | Many-to-One (*:1) |

All relationships are active with single-direction filtering.

---

# 📈 DAX Measures

The following DAX measures were created:

- Total Farmers Insured
- Total Area Covered
- Gross Premium
- Total Sum Insured
- GOI Contribution
- State Contribution
- Premium per Farmer
- Area per Farmer
- District Count
- Gender Gap
- Farmer Category Percentage

---

# 📊 Dashboard Pages

## 📄 Executive Overview

### KPI Cards

- Area Covered
- Gross Premium
- Sum Insured
- GOI Contribution
- State Contribution

### Visualizations

- Top 10 States by Insured Farmers
- Gross Premium Trend (2018–2022)

---

## 📄 State & District Performance Analysis

### Visualizations

- Interactive Hierarchical Filter
- District-wise Gross Premium Treemap
- India Map (Farmer Coverage)
- State-wise Coverage Summary
- Performance KPI Cards
- Key Insights Panel

---

## 📄 Demographic Analysis

### Visualizations

- Gender-wise Farmer Coverage
- Social Category Distribution
- Farmer Category Composition

---

# ✨ Dashboard Features

- Interactive slicers
- Drill-down analysis
- Hierarchical filtering
- Cross-filtering
- KPI cards
- Dynamic charts
- Responsive dashboard layout

---

# 📈 Key Insights

- Identified the top-performing states based on farmer participation.
- Compared gross premium contributions across districts.
- Analyzed year-wise premium trends.
- Evaluated demographic distribution of insured farmers.
- Examined social category and farmer category composition.

---



