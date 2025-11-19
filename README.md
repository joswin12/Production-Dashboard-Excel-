# Production Dashboard (Excel)

- Sheets used:
  - `Production Dataset` – raw production records with Production Date, Region, Manager, Product Type, Units Produced, Total Cost, Gender, Age, Age Groups, and Production Cost Per Unit.
  - `Pivot 1` – Total Production Cost by Product Type.
  - `Pivot 2` – Number of Tasks handled by each Manager.
  - `Pivot 3` – Units Produced by Year and Month.
  - `Pivot 4` – Average Production Cost Per Unit by Product Type.
  - `Dashboard` – final interactive production dashboard.

## Problem Statement

This dashboard helps track production performance across regions, managers, and product types. It gives a consolidated view of total cost, units produced, task distribution among managers, and cost efficiency per unit, enabling management to identify high-cost areas and optimize resource allocation.

## Data Overview

- Total records: 120 production entries.  
- Time period: Production data for 2023 and 2024.  
- Key fields:
  - Operational: ProductionID, ProductionDate, Region, Manager, ProductType, UnitsProduced, TotalCost.
  - Demographics: Gender, Age, Age Groups (A1, A2, A3).
  - Calculated: Production Cost Per Unit.

## Key Metrics & Insights

### Total Cost by Product Type (Pivot 1)

- Automobiles: 1,152,805 total cost.  
- Electronics: 604,575 total cost.  
- Furniture: 703,282 total cost.  
- Machinery: 910,416 total cost.  
- Grand Total: 3,371,078 total production cost.  

### Manager Workload – Number of Tasks (Pivot 2)

- Nancy Grey: 37 tasks (highest workload).  
- Jane Smith: 18 tasks.  
- John Doe: 13 tasks.  
- Mike Brown: 11 tasks.  
- Others (sample): Andrew Blue 10, Laura Black 8, Sarah Lee 5.  
- Grand Total: 120 tasks.  

### Units Produced Over Time (Pivot 3)

- 2023: 11,171 units produced.  
- 2024: 23,556 units produced.  
- Grand Total: 34,727 units.  
- Monthly breakdown example:
  - 2023: Sep 771, Oct 3,103, Nov 4,803, Dec 2,494 units.  
  - 2024: Jan 3,026, Feb 4,127, Mar 3,875, Apr 1,528, May 1,684, Jun 3,537, Jul 1,536, Aug 2,864, Sep 1,379 units.  

### Average Production Cost Per Unit (Pivot 4)

- Automobiles: 140.87 per unit.  
- Electronics: 108.37 per unit.  
- Furniture: 180.44 per unit (highest cost per unit).  
- Machinery: 108.98 per unit.  
- Overall average: 132.39 per unit.  

## Steps Followed

- Step 1: Loaded production data into the `Production Dataset` sheet and ensured correct data types for dates, numbers, and text fields.  
- Step 2: Created a calculated column `Production Cost Per Unit` as `TotalCost / UnitsProduced` for each record.  
- Step 3: Built PivotTables:
  - Pivot 1: Sum of TotalCost by ProductType.
  - Pivot 2: Count of ProductionID (Number of Tasks) by Manager.
  - Pivot 3: Sum of UnitsProduced by Year and Month.
  - Pivot 4: Average of Production Cost Per Unit by ProductType.
- Step 4: Inserted charts (column and line charts) based on each pivot and arranged them on the `Dashboard` sheet.  
- Step 5: Added slicers for Region, Manager, ProductType, and Year to interactively filter all visuals.  
- Step 6: Applied a consistent layout, titles, and formatting to highlight key KPIs like Total Cost, Units Produced, and Average Cost Per Unit.  

## How to Use the Dashboard

- Open `Excel-Dashboard-2.xlsx` and navigate to the `Dashboard` sheet.  
- Use slicers (Region, Manager, ProductType, Year) to analyze cost and production trends for specific segments.  
- Review:
  - Total Cost by Product Type chart to see where most spending occurs.
  - Units Produced over time chart to track production volume by month and year.
  - Manager Tasks chart to understand workload distribution.
  - Average Cost Per Unit chart to compare efficiency across product types.  
