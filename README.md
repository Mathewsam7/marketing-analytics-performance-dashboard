# marketing-analytics-performance-dashboard
# Cross-Channel Digital Marketing Performance Dashboard (Jan - May 2026)

## 📌 Project Overview
This project focuses on the end-to-end data pipeline of a digital marketing analyst. Working with a raw, multi-channel dataset (simulating exports from Google Ads, Facebook, and LinkedIn), I programmatically cleaned the data using Python, engineered core marketing KPIs, and built an interactive dashboard in Tableau to track budget efficiency and campaign ROI.

### 📊 View Interactive Dashboard

https://public.tableau.com/app/profile/sam.mathew2377/viz/DigitalMarketingPerformance_17806705800870/Dashboard2
---

## 🛠️ Tech Stack & Skills
* **Data Cleaning & Engineering:** Python (Pandas, NumPy)
* **Data Visualization:** Tableau Public
* **Marketing Analytics Concepts:** ROI, Cost Per Click (CPC), Click-Through Rate (CTR), Customer Acquisition Cost (CAC)

---

## 🧼 Phase 1: Data Cleaning Checklist (Python)
The raw data contained several tracking inconsistencies and real-world data glitches that required cleaning via Pandas before analysis:
* **Text Standardization:** Resolved trailing spaces and casing mismatches in channel naming (e.g., converted `google ads `, `GOOGLE`, `Google Ads` into a unified `google ads`).
* **Mixed Date Formats:** Handled inconsistent date logging (`YYYY-MM-DD` vs `DD/MM/YYYY`) using mixed-format datetime parsing.
* **Missing Values:** Imputed missing values (`NaN`) in Spend and Leads with `0` to keep row integrity for impressions.
* **Logic Errors & Outliers:** Discarded corrupted tracking data where `Clicks > Impressions` or where ad spend registered as negative numbers.

---

## 📈 Phase 2: Feature Engineering & KPIs
Using NumPy, I built custom calculations to evaluate platform efficiency:
* **Click-Through Rate (CTR):** $\frac{\text{Clicks}}{\text{Impressions}}$
* **Cost Per Click (CPC):** $\frac{\text{Spend}}{\text{Clicks}}$
* **Return on Investment (ROI):** $\frac{\text{Revenue} - \text{Spend}}{\text{Spend}}$

---

## 💡 Key Business Insights
* **Top Revenue Driver:** Google Ads brought in the highest total revenue volume over the 5-month period.
* **Highest Efficiency:** Facebook yielded the highest consistent ROI (**235.42%**) and the lowest overall Cost Per Lead, making it the ideal channel for scaling budget.
* **Underperforming Asset:** LinkedIn demonstrated a significantly higher Cost Per Click, making it less efficient for broad audience lead generation compared to Facebook.

---
