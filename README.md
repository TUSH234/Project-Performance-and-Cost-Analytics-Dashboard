# Project Performance and Cost Analytics Dashboard

## 📌 Project Overview
This project is an interactive Power BI dashboard that analyzes 1,000+ project records. It helps companies track where they are losing money (budget overruns) and why projects are getting late (supply chain delays).

---

## 🛑 The Problem (Business Challenges)
Management was facing major operational and financial problems but didn't have a clear way to track them:
1. **Budget Out of Control:** Projects were spending way more than the estimated budget.
2. **Project Delays:** Materials were arriving late, which delayed the entire project and increased overhead costs.
3. **Missing & Messy Data:** The raw data was scattered and had blank cells in critical columns like 'Region' and 'Target Days', which was messing up the total calculations.

---

## 🎯 The Solution (How the Dashboard Solved the Problem)
This dashboard didn't just show charts; it solved the core business problems for management in three main ways:
1. **Stopped the Budget Blindness (Cost Solution):** The *Budget Overrun Analysis* chart clearly proved that the **North Region** was the main culprit where actual spending crossed the budget. Management can now immediately stop over-spending in the North.
2. **Fixed the Timeline Bottlenecks (Operational Solution):** By correlating data with the *Material Delay Flag*, the dashboard proved that material delays are the direct reason why projects get late. Now, management knows they need to fix logistics or supplier issues.
3. **Enabled Instant Decisions:** Instead of looking at 1,000 messy rows in Excel, management can now use the *Dynamic Slicers* to filter and get any project's health status in just 1-click.

---

## 🛠️ Tools Used & Data Cleaning Steps
* **Microsoft Excel (Data Processing & Feature Engineering):** 
  * **Feature Generation (IF Conditions):** Wrote custom **IF formulas** to logically calculate and generate the values for **Actual Spend** and **Actual Days** based on project status and risk flags.
  * **Project Names:** Used the **VLOOKUP** formula to map and pull the correct project names into the main data sheet from a secondary reference table.
  * **Region Column:** Filled all blank cells with **'N/A'** to keep the geographical data structured.
  * **Target Days Column:** Calculated the **Mode** (most frequent value) of the column and used it to fill all the blank rows so that the average timeline metric doesn't get distorted.
  * Verified all data consistency and aggregates using Pivot Tables.
* **Power BI (Data Visualization):** Imported the cleaned Excel sheet, designed the dashboard layout, and built the interactive charts.

---

## 📊 Key Insights from the Dashboard

1. **Global Numbers (KPI Cards):**
   * **Total Projects:** 1,000 projects tracked.
   * **Total Budget:** 490 Million total estimated cost.
   * **Average Days:** It takes around 171 days on average to finish a project.

2. **Main Charts:**
   * **Budget Overrun Analysis:** Shows Estimated Budget vs. Actual Spend. It highlights that the **North Region** has the highest budget burst.
   * **Supply Chain Delay Impact:** Proves that projects facing material delays take much longer to complete compared to normal projects.
   * **Region-wise Project % Share:** Shows how many projects are running in each region.
   * **Regional Timeline Distribution:** Shows the breakdown of project durations by region.

3. **Interactive Slicers (Filters):**
   * Added click buttons for **Region** and **Project Name** so users can filter the entire dashboard instantly.

---

## 🚀 How to Run
1. Download **Power BI Desktop** (Free).
2. Download the `.pbix` file from this repository.
3. Open the file to view and click through the interactive dashboard!
