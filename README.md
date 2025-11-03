# 📊 Healthcare Payment Trends in Pittsburgh, PA (2023)

This project analyzes **CMS Open Payments** data to explore financial relationships between healthcare providers and industry manufacturers in **Pittsburgh, Pennsylvania (2023)**. The goal is to improve transparency and uncover trends in **general** and **research-related** industry payments to physicians and teaching hospitals.

> Part of a graduate-level healthcare analytics project. Data explored includes CMS Open Payments General & Research datasets.

---

## 🧠 Project Summary

The **Open Payments Program** publicly reports transfers of value from:

- Pharmaceutical & Medical Device Companies  
- Group Purchasing Organizations  

To:

- Physicians  
- Teaching Hospitals  

This analysis answers:

- Which specialties and products receive the most payments?
- How do **General Payments** differ from **Research Payments**?
- Which companies & devices dominate the payment ecosystem?
- Are there seasonal or geospatial trends in payment activity?

---

## ✅ Key Insights

### General Payments
- Majority of payments related to **medical devices**, followed by pharmaceuticals.
- **Food & Beverage** is the largest non-research category.
- Seasonal peaks observed in **March** and **October**.
- Highest paid products: **Orthopedic implants** (shoulder & biceps).
- Top spenders include **Arthrex**, **DePuy Synthes**, **AbbVie**, **Vitalant**.

### Research Payments
- Highly concentrated among **UPMC** institutions & **NSABP Foundation**.
- Driven by **clinical trial** investments.
- Fewer recipients but significantly **higher payment values** per transaction.

### Geography
- Payments cluster around Pittsburgh's medical hubs.
- **93%** of travel-related general payments occur **within the U.S.**
- Top non-PA states for travel: **Florida, Texas, California**

---

## 🛠 Methodology

### Data Sources
- CMS Open Payments — General Payments (2023)
- CMS Open Payments — Research Payments (2023)
- U.S. ZIP Code Database (for geospatial mapping)

### Processing Steps
- Dropped columns with **>95% null values**
- Removed extreme outliers (> $100,000) and capped 99th percentile
- Combined and standardized provider & product fields
- Used ZIP codes to geocode payment activity

### Tools Used
| Category | Tools |
|---|---|
Data cleaning | Python, Pandas, NumPy  
Visualization | Matplotlib, Seaborn, Plotly  
Geo-mapping | GeoPandas, Folium  
Notebook | Jupyter Notebook  
Presentation | PowerPoint  
