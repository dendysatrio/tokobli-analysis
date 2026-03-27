# 🛒 TokoBli E-Commerce Data Analysis

Campaign performance evaluation and data cleaning for TokoBli, an Indonesian 
e-commerce platform, analyzing twin-date campaigns (10/10, 11/11, 12/12) of 2023.

**Program:** RevoU Full Stack Data Analytics — Spreadsheet Module  
**Period:** Oct 2025

---

## 🎯 Business Context

TokoBli runs large-scale promotional campaigns on twin-date events to boost 
transaction volume and attract new customers. This project evaluates campaign 
effectiveness, identifies top-performing product categories, and supports 
future marketing decisions.

---

## 🧹 Data Cleaning Summary

- **Missing values** — filled 3 missing values (Price, Discount, Quantity) 
  using reverse formula calculations
- **Duplicates** — removed 5 duplicate rows → 4,212 unique records
- **Outliers** — removed 12 extreme revenue values using IQR method 
  (threshold: Rp13,955,000) → final dataset: **4,200 valid rows**
- **Columns removed** — `Status` (incomplete) and `Shipping Cost` (all zeros)
- **Data types** — reformatted IDs to text, currency columns to Rupiah format

---

## 🔍 Key Findings

**Campaign Performance:**
- **10/10** was the most revenue-efficient campaign — highest Revenue per 
  Rp1 of discount spent
- **11/11** had the highest total discount but lower revenue than 10/10, 
  likely due to customer fatigue from back-to-back promotions
- **10/10** recorded the highest number of products sold across all campaigns

**Top Categories:**
- **Beauty & Grooming** dominated both 10/10 and 11/11 in revenue and volume
- **Men's Fashion** consistently achieved the best revenue efficiency 
  across all three campaigns (ratios: 130.5 → 172.1 → 114.2)
- **Health & Sports** led 12/12 in product volume (380 units)

**A/B Test — Product Page:**
- New product page generated significantly higher transaction value 
  (Rp830,460 vs Rp746,012 old page, p-value: 0.000)
- Recommendation: roll out new product page to all users

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Google Sheets | Data cleaning, pivot tables, descriptive stats |
| XLMiner Analysis ToolPak | Statistical analysis (before/after outlier removal) |

---

## 📁 Files

| File | Description |
|---|---|
| `[Dendy Satrio] Small Dataset TokoBli E-commerce Data.xlsx` | Cleaned dataset |
| `[W2W3 OCT25]_dendy_satrio_intermediate.pptx` | Full analysis deck |
