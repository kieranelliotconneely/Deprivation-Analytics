Deprivation and Demographic Disparities in the West of England
Using Publicly Available Expenditure and Social Data
📊 Executive Summary
This Power BI project explores two interconnected themes:

Socio-demographic disparities in deprivation, focusing on ethnicity, disability status, and age; and

Public expenditure transparency using spending data over £500 from the West of England Combined Authority (WECA).

Using open data, the dashboard investigates how deprivation varies across demographic groups and provides tools to visualise patterns of government spending. The project aligns with regional goals on inclusion, equality, and accountability, and seeks to support open governance through accessible, reproducible analysis.

🗺️ Key Findings
Ethnic minorities and disabled individuals are overrepresented in the most deprived areas.

Younger (0–17) and older (65+) populations also experience higher deprivation levels.

A linear regression model of public expenditure showed no conclusive relationship with deprivation scores; however, forecasting visuals were added to support stakeholder insights on spending patterns.

📁 Datasets Used
All data was obtained from the West of England Combined Authority Open Data Portal:

Index of Multiple Deprivation (IMD), 2019

Demographic data (ethnicity, age band, disability status)

Quarterly financial transactions >£500

⚙️ Data Preparation
Data was cleaned, standardised, and merged at the Lower Super Output Area (LSOA) level. Cleaning steps included:

Removing duplicates and nulls

Standardising formats and date types

Encoding categorical data

Outlier analysis

All transformation was done within Power BI using:

Power Query M Code (Advanced Editor)

DAX measures for modelling and regression

A sample of the M Code for linear regression and forecasting can be found in /scripts/expenditure_forecast.m.

📈 Analytical Techniques
Correlation analysis between IMD and demographics

Logistic regression in DAX to assess demographic likelihood of deprivation

Bar/column charts for area-level comparisons

Expenditure trend analysis using linear regression and Power BI’s built-in forecasting

⚠️ The linear regression on expenditure data was inconclusive. A forecasting visual was added instead to aid intuitive comparisons.

📊 Dashboard Overview
The Power BI report consists of three main panels:

IMD and Demographic Analysis

Expenditure Dashboard

Narrative Visuals and Storytelling Panels

Visual design emphasised clarity and accessibility, using stacked bar charts, line graphs, and annotated callouts to guide interpretation.

🔍 Literature and Context
This work is informed by public health and policy research, including:

ONS IMD Data (2019)

Joseph Rowntree Foundation (2022) UK Poverty Report

Public Health England reports on ethnicity and inequality

A full bibliography is provided at the end of this document.

🧭 Recommendations
Prioritise high-deprivation, high-vulnerability LSOAs in funding models

Integrate more granular indicators (employment, household, education)

Enhance disability and intersectional data collection

Apply spatial or machine learning clustering for future segmentation

Track deprivation longitudinally using time-series methods

🧑‍💻 How to Use
You can:

Clone this repository

Open the .pbix file in Power BI Desktop

Review scripts/expenditure_forecast.m for regression/forecast logic

Explore each dashboard tab to view findings by topic

Note: All processing was completed within Power BI. No external Python/R scripts were used.

⚖️ Ethics & FAIR Data Principles
This project follows the FAIR principles:

Findable

Accessible

Interoperable

Reusable

The analysis supports ethical, transparent governance through open-data use and documentation.

📚 References
Office for National Statistics (2019). English Indices of Deprivation

West of England Combined Authority (2024). Spending Over £500

Joseph Rowntree Foundation (2022). UK Poverty 2022

Public Health England (2021). Health Inequalities and Ethnicity

Tufte, E.R. (2001). The Visual Display of Quantitative Information

Kennedy, S. (2023). Geospatial Methods in Public Policy Analysis

WECA (2025). Open Data Portal
