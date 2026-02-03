# HR Analytics Dashboard — Attrition & Workforce Insights

## 📌 Project Overview
This project delivers an end-to-end HR analytics solution focused on understanding workforce composition, attrition risk, and retention drivers. The solution is designed using enterprise data modeling principles and executive-oriented Power BI dashboards.

The analysis emphasizes **decision support**, not just visualization.

---

## 📂 Dataset Summary
- Link: https://figshare.com/articles/dataset/Human_Resources_csv/28780886?file=53616341
- Total rows: ~37,400
- Valid employee records: ~22,200
- Invalid / empty rows removed: ~15,000

Key data challenges addressed:
- Inconsistent date formats
- Partial null termination dates
- Incorrect data types
- Mixed categorical values

---

## 🛠 Data Cleaning & Feature Engineering
- Removed invalid employee IDs
- Standardized `hire_date`, `birthdate`, and `termdate`
- Engineered:
  - Employee age
  - Tenure (in years)
  - Employment status (Active / Terminated)
- Converted key fields to categorical types

---

## 🧱 Data Model (Star Schema)
**Fact Table**
- `FactEmployees`: one row per employee with measurable attributes

**Dimension Tables**
- `DimDepartment`
- `DimLocation`
- `DimDate`

### Why Star Schema?
- Improves performance and scalability
- Clean separation of facts and attributes
- Aligns with enterprise BI best practices

---

## 📊 Power BI Dashboards

### Page 1 — Executive Overview
**Objective:** Provide leadership with a high-level workforce health summary.

**Key KPIs**
- Headcount
- Attrition & Attrition Rate
- Average Tenure
- Workforce Risk Level
- Departments at Risk

**Insights**
- Organization-level attrition is at “Watch” level
- Risk is concentrated in specific departments
- Attrition persists even in high-tenure teams

---

### Page 2 — Workforce Diversity & Representation
**Objective:** Understand workforce distribution across age, department, and geography.

**Key KPIs**
- Total Active Employees
- Department Coverage
- State Coverage
- Average Age
- Early-Career Workforce %

> Note: Gender and race attributes were not available; analysis focuses on ethical and reliable dimensions.

---

### Page 3 — Attrition Deep Dive
**Objective:** Identify who leaves, when they leave, and where attrition risk is concentrated.

**Key Findings**
- Early tenure attrition is low (9.1%)
- Majority of exits occur among mid-to-late tenure employees
- 11 departments exceed attrition thresholds

---

## 📐 Key DAX Measures
- Attrition Rate
- Early Tenure Attrition %
- Workforce Risk Level
- Department Risk Flag
- Dynamic Recommendations
- Tenure & Age Bucketing

---

## 🧠 Key Business Takeaways
- Attrition is structural, not onboarding-driven
- Mid-career engagement and leadership effectiveness are critical
- Targeted, department-level interventions yield higher ROI than blanket policies

---

## 🚀 Tools & Technologies
- Python (Pandas, NumPy)
- Power BI
- DAX
- Data Modeling (Star Schema)

---

## 📬 Contact
If you’d like to discuss this project, BI design, or analytics roles:
- LinkedIn: https://www.linkedin.com/posts/jyotigupta-da_dataanalytics-powerbi-hranalytics-activity-7424493165199515649-TuzZ?utm_source=share&utm_medium=member_desktop&rcm=ACoAAExVrF0Bonclg9qL8pLUeG0Z3wvbFD0SGLo
- GitHub: https://github.com/jyoti7575
