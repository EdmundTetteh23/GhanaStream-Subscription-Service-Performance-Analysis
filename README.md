# GhanaStream-Subscription-Service-Performance-Analysis

# Project Overview
This project involves a comprehensive data analysis of GhanaStream, a subscription-based streaming service. The goal was to transform raw, inconsistent data into a high-level executive dashboard to help stakeholders understand revenue health, regional performance, and user retention.

The final workbook includes a cleaned data model, a dedicated Q&A section for business-critical metrics, and a visual dashboard.

## Data Cleaning and Transformation
Before the analysis, I performed significant data cleaning to ensure accuracy:
  1. Data Modeling: Converted raw ranges into structured Excel Tables to allow for dynamic data expansion and more readable formulas.
  2. Geographic Integrity: I identified inconsistencies where states (e.g., Greater Accra) were incorrectly mapped to multiple regions. I      built a nested logical function to standardize the 16 regions of Ghana into four primary zones: Southern, Northern, Eastern, and          Western Ghana.
  3. Financial Logic: Created a custom Revenue column to account for promotional discounts:
        Revenue = Subscription\ Fee - (Discount \times Subscription\ Fee)

## Key Business Metrics (Q&A)
I developed a "Stakeholder Q&A" sheet to provide direct answers to essential business questions using advanced Excel formulas:
MetricFormula LogicInsightTotal RevenueSUM(GhanaStream[Revenue])Total capital generated across all tiers.Market SizeCOUNTA(GhanaStream[Order ID])Total volume of transactions processed.MRRSUMIFS (Monthly) + (SUMIFS Annual / 12)Standardized monthly recurring revenue.ARRMRR * 12Projected yearly revenue based on current MRR.Churn RateCOUNTIF (Churn="Yes") / COUNTAPercentage of customers leaving the service.
The Dashboard
The GhanaStream General Overview dashboard was designed for executive decision-making, focusing on three core pillars
  1. Revenue Segmentation: A breakdown of revenue by subscription tier (Basic, Standard, Premium) and geographic region.
  2. User Behavior: A donut chart showing the percentage split per device, revealing that Mobile (40%) is the primary way users interact       with the platform.
  3. Trend Analysis: A monthly view of recurring revenue across 2023 and 2024 to identify seasonal growth patterns.
Technical Skills Demonstrated
Data Cleaning: Nested IF and OR logic for data standardization.
Financial Modeling: Calculating MRR/ARR from mixed-duration subscription plans.
Data Visualization: Pivot Charts, custom color formatting, and UI/UX layout design in Excel.
Analytical Thinking: Converting "Classroom Data" into a business-ready case study.

## How to Use
  1. Download the GhanaStream_Dataset.xlsx file.
  2. Navigate to the Dashboard tab for the visual overview.
  3. Check the Q&A tab for the raw metric calculations. 
