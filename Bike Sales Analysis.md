# Bike Sales Analysis (Excel)
This project on bike sales uses Excel to efficiently analyze and structure the dataset, employing pivot tables, pivot charts, and advanced formulas to extract valuable insights. A comprehensive dashboard was designed to visualize the data, enabling easy tracking of essential metrics and empowering data-driven decision-making.

## Table of Content
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Excel Utilization for Data Cleaning and Visualization](#excel-utilization-for-data-cleaning-and-visualization)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results or Findings](#results-or-findings)
- [Recommendation](#recommendation)
- [Limitations](#limitations)

---
### Project Overview
This project centers on analyzing a dataset with customer demographics (including age, income, region, marital status, and gender), commute distance, and purchased products for a bike company. Using Excel, I first cleaned and structured the data, then created pivot tables and charts to reveal purchasing trends and customer behavior patterns. To support data-driven decisions, I developed an interactive dashboard to visualize key metrics, such as average income and purchase frequency. [Bikes Sales Excel Project.xlsx](https://github.com/user-attachments/files/16805824/Bikes.Sales.Excel.Project.xlsx)

![Excel Dashboard docx](https://github.com/user-attachments/assets/0f0c99b0-4740-4907-89d4-9e75d59d3ce7)

---
### Data Source
The main dataset for this analysis is the "[Excel Project Dataset.xlsx](https://github.com/user-attachments/files/16805832/Excel.Project.Dataset.xlsx)" file, which includes comprehensive details on each customer purchase.
---
### Tools
- Microsoft Excel

---
### Excel Utilization for Data Cleaning and Visualization
I utilized Excel for:
1. Table population using IF function.
2. Currency formatting.
3. Removing duplicates or blank cells.
4. Generating pivot tables and pivot charts to visualize findings.
5. Compiling all charts and filters into a cohesive dashboard.

---
### Exploratory Data Analysis
This involved exploring the purchase data to answer key questions, such as:
- What is the average income of those who purchased these bikes?
- What is the distance covered by those who purchased these bikes?
- Which age group purchased the most bikes?

---
### Data Analysis
This includes an interesting function worked with:
```IF function
=IF(L2>=55,"Older Adults (55 & above)",IF(L2>=31,"Middle Age (31-54)",IF(L2<31,"Adults (0-30)","Invalid")))
```

---
### Results or Findings
The analysis results are summarized as follows:

- The average income of bike purchasers is higher among male customers, with a significant peak observed among those commuting 0-1 mile. Marketing efforts should focus on middle-aged customers to maximize impact.
---
### Recommendation
Based on the analysis, the following actions are recommended:

- **Targeted Marketing:** Tailor marketing efforts towards customers in the average income bracket who demonstrate strong purchasing power.
- **Highlight Short Commute Benefits:** Since the majority of bike buyers commute 0-1 miles, emphasize the convenience, cost-effectiveness, and environmental benefits of biking short distances. Campaigns could spotlight the health advantages of biking for local errands or short commutes.
- **Age-Specific Promotions:** With middle-aged customers as the primary buyers, create age-focused promotions. This could include models with family-friendly features or designs suited for commuting and leisure. Marketing can highlight lifestyle themes such as fitness, work-life balance, and versatile use.

### Limitations
- I had to replace the initials in a word with their full meanings, for example, 'M' for '**Male**' and 'F' for '**Female**' in the `Gender` column, and 'M' for '**Married**' and 'S' for '**Single**' in the `Marital Status` column so as not to confuse readers who might not understand what the initials stand for.








