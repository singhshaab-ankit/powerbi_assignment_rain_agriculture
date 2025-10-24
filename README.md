# powerbi_assignment_rain_agriculture
🔹 Project Title

Analyzing Rainfall Impact on Agricultural Productivity in India

🔹 Project Overview

This project investigates how rainfall variability influences agricultural productivity across Indian states.
Using Power BI, the analysis visualizes the correlation between monsoon rainfall trends (June–September) and crop area/yield from 1966–2017.

The goal is to help stakeholders and learners understand rainfall-driven agricultural patterns and make data-backed decisions for sustainable farming.

🔹 Dataset Information

Dataset Name: rain-agriculture.csv
Source: HeroX Private Limited (Learning Dataset)
Time Period: 1966–2017
Key Columns:

State Name – Name of Indian state

Year – Year of observation

RICE AREA, WHEAT AREA, MAIZE AREA – Crop area (in 1000 ha)

JUN, JUL, AUG, SEP – Monthly rainfall (in mm)

🔹 Tools & Technologies Used

Microsoft Power BI Desktop

Power Query (for data cleaning & transformation)

DAX (for calculated measures)

Visualization Components: Line, Bar, Map, Scatter, KPI Cards

🔹 Data Cleaning & Transformation Steps

Imported dataset into Power BI (Get Data → Text/CSV).

Checked Data Types: Converted numeric and text fields appropriately.

Unpivoted crop columns (RICE AREA, WHEAT AREA, etc.) → Created Crop Type & Crop Area.

Created Total Rainfall:

Total_Rainfall = [JUN] + [JUL] + [AUG] + [SEP]


Unpivoted Month Columns (JUN–SEP) → Month & Monthly_Rainfall.

Derived Season Field:

JUN → Early Monsoon

JUL & AUG → Peak Monsoon

SEP → Late Monsoon

Removed nulls, duplicates, and standardized numerical precision.

Applied Close & Load to finalize data for visuals.

🔹 DAX Measures Used
Total Rainfall = SUM('TableName'[Total_Rainfall])
Avg Rainfall = AVERAGE('TableName'[Total_Rainfall])
Avg Crop Area = AVERAGE('TableName'[Crop Area])
Max Crop Area = MAX('TableName'[Crop Area])


🔹 Dashboard Visuals Summary
Visual Type	Purpose	Fields Used
Line Chart	Yearly Rainfall Trends	Year vs Total Rainfall
Bar Chart	Rainfall vs Crop Area by State	State Name, Total Rainfall, Crop Area
Scatter Plot	Rainfall vs Agricultural Productivity	Total Rainfall vs Crop Area
Map	Geographic Crop Area Distribution	State Name, Crop Area, Avg Rainfall
KPI Cards	Key Metrics	Avg Rainfall, Avg Crop Area, Max Crop Area

🔹 Key Analytical Findings
🌧️ Rainfall Trends:

Annual rainfall fluctuated between 1.6M – 2.4M mm.

Long-term average ~ 1.9M mm, showing periodic drought years.

🌾 Seasonal Pattern:

July–August consistently record the highest rainfall.

June marks the monsoon onset with moderate rains.

September shows tapering rainfall contributing to soil moisture.

📈 Regional Analysis:

Punjab & Haryana: High productivity despite moderate rainfall.

Kerala, Odisha, West Bengal: High rainfall but moderate yield efficiency.

Rajasthan: Low rainfall → limited crop area expansion.

🔹 Insights & Recommendations

Insights:

Peak monsoon (Jul–Aug) plays the most crucial role in crop growth.

Balanced rainfall (not extreme) correlates with higher yield efficiency.

Late monsoon (Sep) supports post-harvest soil health.

Recommendations:

Develop rainfall-based crop planning frameworks.

Improve irrigation & water harvesting in low-rainfall regions.

Encourage crop diversification aligned with rainfall patterns.

Use real-time rainfall prediction for adaptive crop management.

Strengthen data-driven decision support for farmers and policymakers.

🔹 Files Submitted
File Name	Description
rain-agriculture.csv	Original dataset
Rainfall_Agriculture_Analysis.pbix	Power BI Dashboard
Rainfall_Agriculture_Analysis.pptx	PowerPoint summary presentation

🔹 Author Information
Name: Ankit Chauhan
Batch: CPDA - B5
Tool Used: Microsoft Power BI
Date: October 2025
