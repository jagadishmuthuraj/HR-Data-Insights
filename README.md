
# HR Data Insights

## Problem Statement

In today’s dynamic business environment, human resources play a critical role in shaping organizational success. However, HR departments often face challenges in accessing, interpreting, and leveraging workforce data in a timely and effective manner. The lack of consolidated, visualized, and interactive insights makes it difficult to identify trends in workforce composition, track diversity metrics, and understand departmental distribution.

This Power BI HR Dashboard addresses these challenges by providing a centralized view of employee headcount analytics. The dashboard leverages interactive visuals to deliver key insights across several critical dimensions: 

In conclusion, this HR Analytics Dashboard transforms raw data into meaningful insights that support smarter, faster, and more strategic HR decisions — all through the power of interactive data visualization in Power BI


### Steps followed 
1️⃣Data Collection

The first step was gathering employee data in an Excel spreadsheet. This data included essential fields such as Employee ID, Name, Gender, Age, Job Title, Department, Business Unit, Country, Joining Date, and Employment Year. This dataset served as the foundation for all analysis and reporting within the dashboard.


---

2️⃣ Data Cleaning & Transformation

Using Power Query, the data was cleaned and transformed. Null values were removed, incorrect data types were corrected, and irrelevant columns were excluded. New columns such as Age Group and Year were derived to enable category-based visualizations. All text data (like department names) was standardized to avoid duplication and improve grouping in charts.


---

3️⃣ Data Modeling

A logical data model was built using a star schema, connecting the central employee table (fact table) to various dimension tables like Department, Country, Business Unit, and Job Title. Several DAX measures were created to calculate KPIs like:

Total Headcount = COUNT(Employee[Employee ID])
Female % = DIVIDE([Female Count], [Total Headcount]) * 100

This modeling ensured accurate and scalable reporting across multiple filters and visuals.


---

4️⃣ Dashboard Design

🎨 The dashboard layout was carefully crafted for clarity and usability:

Top Panel: KPI cards for Total Employees, Gender Split, and Date.

Sidebar: Slicers for Country, Department, Employee Name, and Date.

Main Area: Visuals grouped logically (Trends, Demographics, Distribution, Titles).


Corporate colors and consistent formatting were used to keep the design professional and clean.


---

5️⃣ Creating Visualizations

The following visuals were used to present HR data effectively:

📈 Line Chart: Employee headcount over years.

🟡 Pie Chart: Gender distribution.

📊 Bar Charts: Age groups and job titles.

🌍 Stacked Bar Chart: Country-wise distribution.

🧩 Treemap: Business unit headcount.


Each visual was interactive and updated in real-time based on slicer selections.


---

6️⃣ Filters & Interactivity

Dynamic slicers were added to filter data by:

🌎 Country

🏢 Department

👤 Full Name

📅 Date Range


Cross-filtering and tooltips were enabled to improve interactivity. Clicking any visual element updated the entire report for contextual analysis.


---

7️⃣ Testing & Optimization

The dashboard was tested to ensure:

✅ Accurate data representation

⚡ Smooth performance (by removing unused columns)

📐 Clean alignment and consistent formatting

✔️ Proper interaction among slicers and visuals


This step ensured the final report was reliable, fast, and user-friendly
  
  
Key Performance Indicators (KPIs) - HR Dashboard Analysis 📊👥

1. Total Headcount 👨‍💼👩‍💼

👥 1000 Employees
Shows the total number of active employees as of 20-03-2025.


---

2. Gender Distribution ⚖️

♂️ Male: 485 (48.5%)

♀️ Female: 515 (51.5%)
Insight: A nearly balanced workforce, with a slight female majority.



---

3. Age Group Distribution 🎂

Age brackets include:
20 | 25 | 29 | 30 | 35 | 40 | 45 | 47 | 49 | 50 | 55 | 60
Each bar represents the number of employees in that group.
Insight: Helpful for workforce planning and generational diversity strategies.


---

4. Employee Growth Over Years 📈

Trend from 2000 to 2025

Sharp increases around 2018, 2020, and 2023
Insight: Indicates business expansion and hiring growth.



---

5. Country-wise Distribution 🌍

🇺🇸 United States: 634

🇨🇳 China: 122

🇧🇷 Brazil: 244
Insight: Majority of the workforce is based in the USA.



---

6. Department Filter 🏢

Departments include:

Accounting

Engineering

Finance
Custom filtering available!
Insight: Enables deeper dives into team composition.



---

7. Business Unit Breakdown 🧩

Specialty Products: 266

Corporate: 254

Research & Development: 253

Manufacturing: 226
Insight: Balanced workforce allocation across core units.



---

8. Job Title Distribution 🧑‍💼

Top roles by count:

Manager

Vice President

Sr. Manager

Director

Analyst
Insight: Reflects leadership and organizational structure.



---

9. Date Range Filter 🗓️

From: 30-04-1993

To: 25-12-2022
Insight: Useful for historical analysis and trend tracking
  
      a) Average delay in arrival(minutes) - 15.09
      b) Average delay in departure(minutes) - 14.71
Average delay will change if different visual filters will be applied.

