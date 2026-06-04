# Project Overview
This project involves a comprehensive data analysis of GhanaStream, a subscription-based streaming service. The goal was to transform raw, inconsistent data into a high-level executive dashboard to help stakeholders understand revenue health, regional performance, and user retention.

The final workbook includes a cleaned data model, a dedicated Q&A section for business-critical metrics, and a visual dashboard.

## Data Cleaning and Transformation
Before the analysis, I performed significant data cleaning to ensure accuracy:
  1. Data Modeling: Converted raw ranges into structured Excel Tables to allow for dynamic data expansion and more readable formulas.
  2. Geographic Integrity: I identified inconsistencies where states (e.g., Greater Accra) were incorrectly mapped to multiple regions. I      built a nested logical function to standardize the 16 regions of Ghana into four primary zones: Southern, Northern, Eastern, and          Western Ghana.
  3. Financial Logic: Created a custom Revenue column to account for promotional discounts:
        Revenue = Subscription Fee - (Discount * Subscription Fee)

## Key Business Metrics (Q&A)
I developed a "Stakeholder Q&A" sheet to provide direct answers to essential business questions using advanced Excel formulas:
  1. Total Revenue "Formula = SUM(GhanaStream[Revenue])".
  2. Market Size "Formula = COUNTA(GhanaStream[Order ID])"
  3. Monthly Recurring Revenue (MRR) "Formula = SUMIFS(GhanaStream[Revenue],GhanaStream[Plan Type],"Monthly") +   (SUMIFS(GhanaStream[Revenue],GhanaStream[Plan Type],"Annual")/12)"
  4. Annual Recurring Revenue (ARR) Formula = MRR * 12"
  5. Churn Rate "Formula = COUNTIF(GhanaStream[ChurnFlag],"Yes")/COUNTA(GhanaStream[Order ID])"

## The Dashboard
The GhanaStream General Overview dashboard was designed for executive decision-making. 

### KPIs
- Total Orders
-  Total SalesP
-  Perecntage Churned

###Visualizations
1. Revenue Segmentation: A breakdown of revenue by subscription tier (Basic, Standard, Premium) and geographic region.
2. 2. User Behavior: A donut chart showing the percentage split per device, revealing that Mobile (40%) is the primary way users interact       with the platform.
3. 3. Trend Analysis: A monthly view of recurring revenue across 2023 and 2024 to identify seasonal growth patterns.

###Slicers
Slicers to make the dashboard interactive and filter through data include:
- Year
- Plan Type
- Device Type
- Region

## Technical Skills Demonstrated
- Data Cleaning: Nested IF and OR logic for data standardization.
- Financial Modeling: Calculating MRR/ARR from mixed-duration subscription plans.
- Data Visualization: Pivot Charts, KPIs, Slicers custom color formatting, and UI/UX layout design in Excel.
- Analytical Thinking: Converting "Data" into a business-ready case study.

## How to Use
  1. Download the GhanaStream_Dataset.xlsx file.
  2. Navigate to the Dashboard tab for the visual overview.
  3. Review the Q&A tab for the raw metric calculations. 
