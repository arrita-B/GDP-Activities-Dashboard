# Guided Project – GDP by Production (Activities) | Power BI


![Dashboard Page 1](/Dashboard%20view.png)

## Introduction
This dashboard was created as a **self-directed Power BI practice project**, using official macroeconomic data from the **Kosovo Statistics Agency**. The goal of the project is to present a clear and intuitive overview of **GDP from the production (activities) side**, focusing on value added, sectoral shares, and contributions to nominal growth.

The dashboard is intended for **analysts in public institutions, students of economics, and the general public** who want to quickly understand the structure of Kosovo’s economy and identify the main contributors to GDP growth without working directly with raw statistical tables.

## Analytical Objective
The dashboard aims to provide a **clear and fast way to identify**:
- The largest activities in terms of value added.
- The main contributors to nominal GDP growth in a given year.

By selecting a single year, users can immediately see which sectors dominate economic activity and which drive changes in overall GDP.

## Data Source & Methodology

- **Source:** Kosovo Statistics Agency  
- **Geographic Scope:** Kosovo  
- **Frequency:** Annual  
- **Period:** 2009–2024 (latest available)  
- **Type:** Nominal GDP data  

GDP from the production side is constructed as:

**Total Value Added + Taxes − Subsidies**

### Data Preparation
The original dataset was provided in a **wide (horizontal) format**, with economic activities as columns and years as rows. To prepare the data for analysis:

- Taxes and subsidies were separated in Excel into a dedicated structure.
- Activity data was transformed into a **long format** using pivot and unpivot operations.
- Columns were cleaned and converted to appropriate data types.
- A separate **date table** was created and merged with the activity and tax–subsidy tables.

This data model enables consistent calculation of levels, shares, and growth contributions within Power BI.

## Skills Showcased

- **Data Cleaning & Transformation (Excel + Power Query)**  
  Restructured raw GDP data from a wide format into an analysis-ready long format. Separated taxes and subsidies, unpivoted activity data, standardized data types, and prepared consistent yearly structures for modeling.

- **Data Modeling**  
  Built a relational model by creating a dedicated date table and merging it with activity-level and tax–subsidy tables to enable consistent filtering and aggregation.

- **DAX Measures & Economic Indicators**  
  Created measures for GDP, total value added, taxes, subsidies, sectoral shares, and year-on-year nominal growth. Implemented contribution-to-growth logic using activity shares of total value added.

- **Analytical Dashboard Design**  
  Designed a single-page dashboard focused on clarity and analytical purpose, prioritizing interpretability over visual complexity.

- **Interactive Reporting**  
  Enabled year-based analysis through slicers and dynamic measures, allowing users to immediately assess sectoral structure and growth drivers for any selected year.


## Key Indicators

The dashboard focuses on a concise set of macroeconomically meaningful indicators:

- **GDP (level)**
- **Total Value Added (level)**
- **Taxes and Subsidies (levels)**
- **Activity Shares** of total value added
- **Contribution to Nominal Growth** by activity

Growth is defined as **year-on-year nominal growth**, and contributions are calculated by weighting total growth by each activity’s share of total value added in the selected year.

## Dashboard Overview

### Single-Page Analytical View

The dashboard consists of **one page**, intentionally designed to keep the analysis focused and accessible.

Workflow:
1. The user selects a **year**.
2. KPI cards display GDP, total value added, taxes, and subsidies.
3. Visuals show:
   - Sectoral shares of total value added.
   - Contributions to total value added growth by activity.

This structure allows users to quickly understand both the **composition** of the economy and its **growth drivers**.

## Scope & Limitations

This dashboard is intentionally descriptive and does not attempt to answer questions outside its analytical scope:

- No real (inflation-adjusted) GDP analysis.
- No employment, productivity, or income distribution indicators.
- No causal interpretation or forecasting.
- No regional or international comparisons.

The dashboard is designed strictly for **structural analysis of nominal GDP** from the production side.

## Conclusion
This project demonstrates how Power BI can be used to transform official macroeconomic data into a **clear and accessible analytical tool**. By combining levels, shares, and growth contributions in a single view, the dashboard enables users to quickly understand the structure and drivers of Kosovo’s economy while serving as a practical exercise in data transformation, modeling, and macroeconomic analysis.
