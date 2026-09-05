# 🎬 Movie Database SQL Analysis

> **End-to-end movie box office analysis using SQL and Microsoft Excel**

![SQL](https://img.shields.io/badge/SQL-MySQL--Compatible-4479A1?logo=mysql&logoColor=white)
![Excel](https://img.shields.io/badge/Microsoft%20Excel-Analysis%20%26%20Dashboard-217346?logo=microsoftexcel&logoColor=white)
![Dataset](https://img.shields.io/badge/Dataset-4%2C535%20Films-6C63FF)
![Period](https://img.shields.io/badge/Period-2000--2017-555555)

---

## 📌 Project Overview

This project analyses **4,535 films released between 2000 and 2017** using the Cisco Networking Academy Movies dataset.

The project combines **SQL analysis** with **Microsoft Excel** to investigate movie box-office performance across:

- Revenue
- Profit
- Return on Investment (ROI)
- Production Budget
- Original Language
- Popularity
- Runtime
- Audience Ratings
- Yearly Performance

The objective is to transform raw movie data into meaningful insights about **commercial performance, profitability, and production efficiency**.

---

# 🎯 Business Questions

The analysis answers the following questions:

1. How large is the dataset and what period does it cover?
2. Which films generated the highest box-office revenue?
3. Which films achieved the highest return on investment?
4. How did annual box-office revenue change from 2000–2017?
5. Which original languages generated the strongest revenue?
6. Do larger production budgets guarantee better returns?
7. Which films achieved both strong audience ratings and commercial success?
8. Does popularity correspond to higher audience ratings and revenue?
9. Does movie runtime relate to box-office revenue?
10. Which years generated the highest aggregate profit?
11. How do English-language films compare with non-English films?

---

# 📊 Key Results

The Excel analysis provides the following project-level metrics:

| Metric | Result |
|---|---:|
| Source dataset | **4,535 films** |
| Films retained after cleaning | **3,420 films** |
| Analysis period | **2000–2017** |
| Total box-office revenue | **$364.79B** |
| Total production budget | **$129.97B** |
| Average ROI* | **234,252.8%** |
| Profitable films | **68.3%** |
| Highest-grossing film | **Avatar** |
| Highest-ROI film | **Welcome to Dongmakgol** |
| Primary language | **English (en)** |
| Most productive year | **2011** |

### ⚠️ ROI Interpretation

The reported average ROI of **234,252.8%** is extremely high because percentage ROI is highly sensitive to very small production budgets.

Therefore, this figure should be interpreted as a **dataset-level comparative efficiency metric**, rather than a typical industry-wide average.

The SQL ROI analysis also applies a **$1 million minimum budget filter** to reduce the influence of micro-budget outliers.

---

# 🔎 Key Findings

## 💰 1. Revenue and ROI tell different stories

High-budget productions generate the highest average revenue, but the largest box-office numbers do not necessarily produce the strongest percentage returns.

The budget-tier analysis shows that **mid-budget films can achieve significantly stronger average ROI than blockbuster productions**.

This demonstrates why revenue and ROI should be evaluated separately.

---

## 🎬 2. Low-budget films can generate exceptional returns

The ROI analysis identifies films that generated several times their original production budgets.

For example, **Get Out** achieved an exceptionally high ROI despite its relatively small production budget.

This highlights how smaller productions can deliver strong financial efficiency.

---

## 🌍 3. English-language films dominate revenue

English-language films account for the largest share of revenue within the analysed dataset.

However, non-English films can still achieve competitive performance when profitability and ROI are considered.

---

## 📈 4. Box-office performance changed over time

Annual revenue changed significantly throughout the 2000–2017 period.

The Excel analysis provides a year-by-year revenue trend to show how overall box-office performance evolved over time.

---

## ⭐ 5. Critical and commercial success can overlap

The SQL analysis combines audience ratings, revenue and vote counts to identify films that performed strongly both commercially and with audiences.

This provides a broader view of movie success beyond box-office revenue alone.

---

# 🧮 SQL Analysis

The SQL component contains **10 core queries plus 1 bonus query**.

| # | Analysis | Main SQL Concepts |
|---|---|---|
| **01** | Dataset overview & date range | `COUNT`, `MIN`, `MAX`, `AVG` |
| **02** | Top 10 highest-grossing films | `WHERE`, `ORDER BY`, `LIMIT` |
| **03** | Top 10 films by ROI | Calculated fields, filtering, sorting |
| **04** | Annual box-office trends | `GROUP BY`, aggregate functions |
| **05** | Revenue by original language | `GROUP BY`, `HAVING` |
| **06** | Budget tier analysis | `CASE WHEN` |
| **07** | Critical + commercial success | Subqueries |
| **08** | Popularity band analysis | `CASE WHEN`, aggregation |
| **09** | Runtime vs revenue | `CASE WHEN`, grouping |
| **10** | Most productive years | Aggregation, calculated metrics |
| **Bonus** | English vs non-English comparison | Derived table + `CASE` |

---

# 🛠️ SQL Skills Demonstrated

```text
SELECT
WHERE
GROUP BY
HAVING
ORDER BY
LIMIT
CASE WHEN
Aggregate Functions
Calculated Fields
Subqueries
Derived Tables
Data Segmentation
Business Question Analysis
