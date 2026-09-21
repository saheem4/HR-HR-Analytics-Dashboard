# HR Analytics Dashboard

An interactive Power BI dashboard analyzing employee attrition, demographics, and job satisfaction to support HR decision-making.

## Overview

Built on employee-level HR data (282 employees), this dashboard surfaces attrition trends across departments, age groups, and job roles — helping HR teams identify where and why employees are leaving, and prioritize retention efforts.

## Key Metrics Tracked

- **Overall headcount:** 282 employees (238 active, 44 attrited)
- **Attrition rate:** 15.6%
- **Average age:** 37
- Department-wise attrition breakdown (R&D, Sales, HR)
- Attrition by age band and gender
- Job satisfaction scores by job role (1–4 scale)
- Attrition trends by education field

## Key Insights

- **R&D carries the highest attrition volume** (64.5% of all departures), despite likely being the largest department — worth checking whether this is proportional or a red flag.
- The **25–44 age bracket accounts for the bulk of attrition**, suggesting retention efforts should focus on early-to-mid career employees rather than near-retirement staff.
- Job satisfaction scores vary meaningfully by role — Laboratory Technicians and Manufacturing Directors show the widest satisfaction spread, flagging them as roles to investigate further.

## Tools & Techniques

- **Power BI** — dashboard design, interactive slicers (education level filter), drill-through visuals
- **DAX** — calculated measures for attrition rate, age banding (`CF_age band`), and attrition labeling (`CF_attrition label`)
- **Data modeling** — structured HR dataset with calculated columns for segmentation

## Dashboard Components

| Visual | Purpose |
|---|---|
| KPI cards | Headcount, attrition count/rate, active employees, average age at a glance |
| Department-wise attrition (pie) | Which departments lose the most people |
| Employees by age group (bar, gender-split) | Workforce age distribution |
| Job satisfaction (matrix) | Satisfaction score distribution per role |
| Education field (bar) | Attrition count by education background |
| Age-band donuts | Attrition rate within each age bracket |

## Data

Employee-level HR dataset with fields including Attrition, Department, Job Role, Age Band, Education Field, Gender, Marital Status, Business Travel, and OverTime status.

## Files

- `HR_Analytics_Dashboard.pbix` — Power BI report file
- `screenshots/` — dashboard views for quick preview without opening Power BI
