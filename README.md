# 📊 AI Jobs Market Dashboard | Tableau & Power BI

An interactive data visualization project that analyzes the **Global AI Jobs Market** using **Tableau** and **Microsoft Power BI**. The dashboards provide insights into salary trends, job distributions, experience levels, remote work adoption, and geographic hiring patterns, enabling data-driven decision-making for HR professionals, recruiters, and job seekers.

---

## 🚀 Project Overview

This project explores AI job market data through interactive dashboards built in both **Tableau** and **Power BI**. It demonstrates how modern Business Intelligence (BI) tools can transform raw data into meaningful insights using visual analytics, calculated fields, and interactive filtering.

The dashboards are designed to answer key questions such as:

- Which AI roles offer the highest salaries?
- How does experience affect compensation?
- Which industries and company sizes pay the most?
- What is the distribution of remote, hybrid, and onsite jobs?
- Which regions have the highest concentration of AI opportunities?

---

## 🛠️ Tools & Technologies

- 📈 Tableau
- 📊 Microsoft Power BI
- 🧮 DAX (Power BI)
- 📐 Tableau Calculated Fields
- 🌍 Interactive Maps
- 📋 Data Visualization Techniques

---

## 📌 Dashboard Features

### Tableau Dashboard

- Horizontal Bar Chart – Average Salary by Job Title
- Grouped Bar Chart – Salary by Company Size & Industry
- Stacked Bar Chart – Salary by Experience Level
- Heatmap – Job Postings by Month & Role
- Geographic Map – Global AI Hiring Distribution
- Pie Charts – Experience Distribution & Remote Work Prevalence
- Work Type vs Salary Distribution Analysis

### Power BI Dashboard

- Grouped Bar Chart – Salary by Company Size & Industry
- Stacked Bar Chart – Job Count by Remote Work & Salary Category
- Horizontal Bar Chart – Average Salary by Job Title
- 100% Stacked Bar Chart – Salary by Experience & Employment Type
- Interactive Map Visualization
- Experience & Remote Work Distribution Charts

---

## 📊 Calculated Fields

### Salary Category

Classifies salaries into four categories:

- Low
- Medium
- High
- Very High

### Tableau Formula

```text
IF [Average Salary] < 90000 THEN "Low"
ELSEIF [Average Salary] < 120000 THEN "Medium"
ELSEIF [Average Salary] < 150000 THEN "High"
ELSE "Very High"
END
```

### Power BI (DAX)

```DAX
Salary_Category =
SWITCH(
    TRUE(),
    [Average Salary] < 90000, "Low",
    [Average Salary] < 120000, "Medium",
    [Average Salary] < 150000, "High",
    "Very High"
)
```

---

## 👨‍💼 Experience Level Categorization

Experience is grouped into:

- Entry
- Mid
- Senior
- Expert

### Tableau

```text
IF [Years Experience] < 2 THEN "Entry"
ELSEIF [Years Experience] < 5 THEN "Mid"
ELSEIF [Years Experience] < 10 THEN "Senior"
ELSE "Expert"
END
```

### Power BI (DAX)

```DAX
Experience_Level =
SWITCH(
    TRUE(),
    [Years_Experience] < 2, "Entry",
    [Years_Experience] < 5, "Mid",
    [Years_Experience] < 10, "Senior",
    "Expert"
)
```

---

## 🎛️ Interactive Features

- Global Filters/Slicers
  - Company Size
  - Industry
  - Experience Level
  - Geography
  - Work Type

- Salary Metric Toggle
  - Average Salary
  - Median Salary

- Dynamic Dashboard Updates

---

## 📈 Key Insights

- 💰 Senior and Principal AI professionals earn the highest salaries.
- 🏢 Larger companies generally offer higher compensation packages.
- 🌍 North America and Western Europe dominate high-paying AI opportunities.
- 🏠 Remote and hybrid work arrangements are common without significant salary reductions.
- 📅 Seasonal hiring patterns can be identified through monthly job posting trends.
- 📊 Experience level strongly influences salary growth.

---

## 🔄 Tableau vs Power BI Comparison

| Feature | Tableau | Power BI |
|----------|----------|----------|
| Ease of Use | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| Drag & Drop | Excellent | Good |
| Calculated Fields | Simple | DAX-based |
| Mapping | Automatic Geocoding | Requires Cleaner Data |
| Interactivity | Excellent Parameters | Powerful Slicers |
| Enterprise Integration | Tableau Cloud/Public | Microsoft Ecosystem |
| Learning Curve | Lower | Moderate to High |

### Tableau Strengths

- Easy drag-and-drop interface
- Fast dashboard prototyping
- Powerful parameter controls
- Intuitive calculated fields
- Excellent visual customization

### Power BI Strengths

- Strong data modeling capabilities
- Deep Microsoft ecosystem integration
- Powerful DAX functions
- Enterprise-ready reporting
- Advanced business intelligence features
---

## 🎯 Business Value

This project helps:

- HR Teams identify salary benchmarks
- Recruiters understand hiring trends
- Organizations compare compensation across industries
- Job seekers explore career opportunities
- Analysts uncover workforce patterns in the AI sector

---
## 🔮 Future Enhancements

- Predictive salary modeling
- Real-time job market integration
- Skill demand analysis
- AI-powered recommendation engine
- Interactive drill-through reports
- Automated dashboard refresh

---

## 📜 License

This project was developed as part of the **B9DA106 – Data Visualization** module for academic purposes.
