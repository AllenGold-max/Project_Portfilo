# Bike Sales Analysis (Excel)
A project on Bike Sales leveraging Excel to analyze and organize the dataset, creating pivot tables, pivot charts and using formula. I then built a dashboard to visualize the data,  to easily track key metrics and make informed decisions.

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
This project analyzes a dataset containing information on customer demographics(age,income, region, marital status, gender e.t.c), commute distance and purchased product for a bike company. Using Excel, I cleaned and organized the data, then created pivot tables and charts to identify purchase trends and customer behavior patterns. Finally, I developed a dashboard to visualize key metrics such as average income to make data-driven decisions. [Bikes Sales Excel Project.xlsx](https://github.com/user-attachments/files/16805824/Bikes.Sales.Excel.Project.xlsx)

![Excel Dashboard docx](https://github.com/user-attachments/assets/0f0c99b0-4740-4907-89d4-9e75d59d3ce7)

---
### Data Source
The primary dataset used for this analysis is the "[Excel Project Dataset.xlsx](https://github.com/user-attachments/files/16805832/Excel.Project.Dataset.xlsx)" file, containing detailed information about each purchase made by the customer.

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
The analysis result are summarized as follows:
- The average income of purchased bikes is greater in the male gender, with a noticeable peak among customers commuting between 0-1 mile distance. Middle age customers should be targeted for marketing efforts. 

---
### Recommendation
Based on the analysis, I recommend the following actions:
- The company should tailor its marketing campaigns to target customers within the average income brackets with more spending power.
- Since most bike purchasers commute between 0-1 miles, the company should emphasize the convenience and cost-effectiveness of biking for short distances. Marketing efforts could highlight the environmental and health benefits of using bikes for local errands or short commutes.
- With the most significant number of bike purchasers being the middle age, the company should design age-specific promotions. This could include offering bikes with features appealing to this age group, such as family-friendly models or bikes suited for both commuting and recreational use. Advertising campaigns could also focus on lifestyle aspects relevant to this age group, such as fitness and work-life balance.
---

### Limitations
- I had to replace the initials in a word with their full meanings, for example, 'M' for '**Male**' and 'F' for '**Female**' in the `Gender` column, and 'M' for '**Married**' and 'S' for '**Single**' in the `Marital Status` column so as not to confuse readers who might not understand what the initials stand for.








