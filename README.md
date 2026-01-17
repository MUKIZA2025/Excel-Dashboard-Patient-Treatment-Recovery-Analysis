# 📊 Excel Dashboard – Patient Treatment & Recovery Analysis

## 🖼️ Dashboard Preview

![Patient Treatment & Recovery Excel Dashboard](screenshots/dashboard_overview.png)


## 📌 Project Overview

Healthcare analytics is one of the most impactful applications of data visualization. In this project, I developed an **interactive Excel Dashboard** to analyze patient treatment and recovery performance using a **real-world-style hospital dataset**.

The main objective was to answer key healthcare questions such as:

- Which medical departments achieve the best recovery outcomes?
- Do higher treatment costs guarantee better patient recovery?
- How do age and gender influence recovery scores?
- Which treatment types and doctors perform better?

The entire analysis was built **exclusively in Microsoft Excel**, using calculated columns, Pivot Tables, slicers, KPIs, and charts. This project demonstrates how powerful Excel can be for analytics — even without programming.

---

## 🧾 Step 1: Understanding the Dataset

The dataset represents hospital patient records and contains both **categorical and numerical variables**, making it ideal for analytical reporting.

| Column | Type | Description |
|------|------|------------|
| Patient ID | Identifier | Unique patient identifier (e.g., P1001) |
| Department | Categorical | Medical department (Cardiology, Pediatrics, etc.) |
| Treatment Type | Categorical | Surgery, Medication, Therapy, Observation |
| Doctor Name | Categorical | Consulting doctor |
| Gender | Categorical | Male, Female, Other |
| Age | Numerical | Patient age (years) |
| Treatment Cost | Numerical | Total treatment cost |
| Hospital Stay (Days) | Numerical | Length of hospital admission |
| Recovery Score | Numerical | Recovery performance score (0–100) |

📌 **Dataset Source:**  
Synthetic Hospital Patient Treatment Dataset (Kaggle / SlideScope)

---

## 💡 Step 2: Creating Calculated Columns

To enrich the analysis, I added derived fields directly in Excel using formulas.

### (A) Cost Category

This column groups patients based on their treatment expenditure.

```excel
=IF(G2<=53410,"Low Cost",
IF(G2<=101376,"Medium Cost","High Cost"))
