# 📊 Gender Inequality in HIV Infections Among Adolescents  
### Tableau Public Health Analytics Project

[![Tableau Public](https://img.shields.io/badge/View-Live%20Dashboard-blue?logo=tableau)](https://public.tableau.com/views/GenderInequalityinHIVInfectionsinAdolescents_17710132765110/GenderInequalityinHIVInfectionsinAdolescents?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
![Tool](https://img.shields.io/badge/Tool-Tableau-blue)
![Focus](https://img.shields.io/badge/Focus-Gender%20Equity-purple)
![Domain](https://img.shields.io/badge/Domain-Public%20Health-green)

---

## 🔎 Project Summary

This Tableau dashboard analyzes **gender disparities in HIV infections and AIDS-related outcomes among adolescents (ages 10–19)** across countries and UNICEF regions.

The objective was to uncover measurable patterns of gender inequality in:

- HIV incidence rates  
- Annual new HIV infections  
- Adolescents living with HIV  
- AIDS-related mortality  

This project demonstrates applied skills in **data transformation, calculated fields, dashboard architecture, and analytical storytelling.**

🔗 **Live Dashboard:**  
https://public.tableau.com/views/GenderInequalityinHIVInfectionsinAdolescents_17710132765110/GenderInequalityinHIVInfectionsinAdolescents

---

## 🎯 Business / Policy Questions Addressed

1. Are adolescent girls disproportionately affected by HIV compared to boys?
2. Which countries show the largest gender gaps in new infections?
3. How have infection trends evolved over time?
4. Do regions with larger gender disparities also experience higher mortality?
5. Where is progress improving — and where is it stagnating?

---

## 🛠 Technical Implementation

### Tableau Features Used
- Calculated Fields (gender difference metric)
- Context Filters (to preserve aggregation accuracy)
- Shared Dashboard Filters
- Custom Sorting by Calculated Measure
- Multi-line Trend Analysis
- Scatter Plot Correlation Analysis
- Heat Maps for Regional Comparison

---

### Key Calculated Field

To quantify gender inequality:

```tableau
SUM(IF [Sex] = "Female" THEN [Estimated number of annual new HIV infections] END)
-
SUM(IF [Sex] = "Male" THEN [Estimated number of annual new HIV infections] END)
