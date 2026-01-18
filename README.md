# 📊 Excel Dashboard – Patient Treatment & Recovery Analysis

## 🖼️ Dashboard Preview

![Patient Treatment & Recovery Excel Dashboard](Dashboard-ScreenShoot.png)

[Check out for Project Video Demo](https://www.linkedin.com/feed/update/urn:li:activity:7418577162984923136/)


## 📌 Project Overview

Healthcare analytics is one of the most impactful applications of data visualization. In this project, I developed an **interactive Excel Dashboard** to analyze patient treatment and recovery performance using a **real-world-style hospital dataset**.

The main objective was to answer key healthcare questions such as:

- Which medical departments achieve the best recovery outcomes?
- Do higher treatment costs guarantee better patient recovery?
- How do age and gender influence recovery scores?
- Which treatment types and doctors perform better?

The entire analysis was built **exclusively in Microsoft Excel**, using calculated columns, Pivot Tables, slicers, KPIs, and charts. This project demonstrates how powerful Excel can be for analytics — even without programming.

# 🧠 Skills Demonstrated

- Data cleaning and preparation in Excel

- Calculated columns using Excel formulas

- Pivot Tables for analytical summaries

- KPI creation and reporting

- Interactive dashboards using slicers

- Healthcare data interpretation

- Visual storytelling with charts

---

## 🧾 Understanding the Dataset

The dataset represents synthetic hospital patient records and was sourced from Kaggle for educational and analytical purposes.
It contains both **categorical and numerical variables**, making it ideal for analytical reporting.

**⚠️ Note:**
This is **synthetic data**, not real patient data. It is used strictly for learning, demonstration, and analytics practice.

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

📌 **Dataset Source:**  [Hospital Patient Treatment Dataset](https://www.kaggle.com/datasets/slidescope/hospital-patient-treatment-dataset/)

Synthetic Hospital Patient Treatment Dataset (Kaggle)

---

## 💡 Creating Calculated Columns

To enrich the analysis, I added derived fields directly in Excel using formulas.

### (A) Cost Category

This column groups patients based on their treatment expenditure.

```excel
=IF(G2<=53410,"Low Cost",
IF(G2<=101376,"Medium Cost","High Cost"))
```
This categorizes patients into **Low, Medium**, and **High** treatment cost groups, enabling cost-effectiveness analysis.

**Purpose:**

- Helps analyze whether higher spending leads to better recovery outcomes
- Enables cost-effectiveness comparison across departments and treatments

### (B) Age Group

Patients were grouped into meaningful life-stage categories.
```excel
=IF(F2<=5,"Infant / Toddler",
IF(F2<=12,"Child",
IF(F2<=19,"Teenager",
IF(F2<=29,"Young Adult",
IF(F2<=44,"Adult",
IF(F2<=59,"Middle-aged",
IF(F2<=74,"Senior","Elderly")))))))
```
This creates **eight life-stage age groups** for demographic-based recovery analysis.

**Purpose:**

- Allows age-based recovery analysis
- Improves clarity in charts and Pivot Tables

## 📊 Key Performance Indicators (KPIs)

Using Pivot Tables and Excel formulas, I created the following KPIs:

- Total Patients
- Average Treatment Cost
- Average Patient Age
- Average Hospital Stay
- Average Recovery Score

All KPIs are powered by Pivot Tables and displayed on the dashboard.

---

## 📊 Pivot Table Analysis

All dashboard visuals are powered by Pivot Tables created on a dedicated **Report sheet**.

Key analyses include:

- Average Recovery Score by Department
- Average Recovery Score by Doctor
- Average Recovery Score by Treatment Type
- Average & Total Treatment Cost by Gender
- Average Recovery Score by Age Group
- Recovery Score by Cost Category

These summaries form the analytical backbone of the dashboard.

---

## 📈 Dashboard Visualizations

To present insights clearly, The dashboard includes::

- **Clustered Column Chart** – Avg Recovery Score by Department
- **Clustered Bar Chart** – Avg Recovery Score by Doctor Name
- **Doughnut Chart** – Avg Recovery Score by Gender
- **Funnel Chart** – Avg Recovery Score by Treatment Type
- **Bar Chart** – Avg Recovery Score by Cost Category
- **Clustered Bar Chart** – Avg Recovery Score by Age Group

Each chart was carefully selected to match the type of comparison being made.

---

## 🧭 Interactivity (Slicers)

To make the dashboard dynamic and user-friendly, I added slicers for:

- Gender
- Department
- Doctor Name
- Treatment Type

All slicers are connected across Pivot Tables using **Report Connections**, ensuring synchronized filtering across all visuals.

This allows users to:

- Compare departments
- Analyze individual doctor performance
- Study recovery outcomes by treatment type or gender

---

## 🎨 Dashboard Design & Formatting

To improve usability and aesthetics:

- Applied a green and white healthcare color theme
- Added icons to KPIs (patients, cost, hospital stay, recovery)
- Ensured uniform slicer styling
- Used clean alignment, spacing, and section headers
- Applied rounded corners and subtle shadows to visuals

A clean layout ensures insights are easy to interpret.

---

## 🔍 Key Insights

After analyzing the data, several insights emerged:

- Pediatrics, Oncology, and Gastroenterology showed higher recovery scores
- Surgery and Therapy generally outperformed medication-only treatments
- Higher treatment cost did not consistently lead to better recovery outcomes
- Elderly, Senior, and Infant/Toddler groups showed relatively higher recovery scores
- Teenager patients recorded lower average recovery scores

These insights can support **resource allocation, treatment planning, and performance evaluation** in healthcare settings.
# 🛠 Tools Used

- Microsoft Excel
- Pivot Tables
- Excel Charts
- Slicers

---

## 🧠 Why Excel Dashboards Matter

This project demonstrates that Microsoft Excel can:

- Deliver BI-level analytics without coding
- Support interactive reporting with slicers
- Combine KPIs, charts, and summaries in one view
- Serve as a powerful tool for small-to-medium datasets

When used effectively, Excel can rival tools like **Power BI** or **Tableau**.


## 🎓 Training & Professional Context

This project was developed as part of **independent data analytics training and mentorship**, delivered directly to an individual learner outside of a formal organizational program.

I currently serve as a **Volunteer Course Instructor at EduConnect Rwanda**, where I support learners by teaching data analysis tools such as Excel, Power BI, SQL, R, and Python.

However, this specific project and training engagement were conducted **independently**, based on a direct request from a learner, and not as an official EduConnect Rwanda program.

## 📚 Acknowledgment

- Synthetic dataset sourced from **Kaggle** | [Hospital Patient Treatment Dataset](https://www.kaggle.com/datasets/slidescope/hospital-patient-treatment-dataset/)

- Project structure inspired by a similar healthcare analytics exercise by
**Ankit Srivastava – Data Analytics Trainer, SlideScope Institute**,
with additional creativity, instructional enhancements, and customization.

## 📂 More Practice Datasets

For additional practice and similar hospital datasets, you can explore: [Colorstech Practice Datasets](https://colorstech.net/category/practice-datasets/)  
*(This link provides more real-world-style datasets for healthcare analytics practice.)*


## 👤 Author

**Ezra Habumukiza**

Statistician: Deomgraphy | Data Analyst | Data Instructor

Volunteer Course Instructor – EduConnect Rwanda

Rwanda

## 🔗 Connect with Me

[Ezra Habumukiza on LinkedIn](https://www.linkedin.com/in/mukizaezra)

mukizaezraa@gmail.com | (+250) 780510913





