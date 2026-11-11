# BMW Sales Performance Dashboard

An interactive Power BI dashboard that analyses BMW sales from 2010 to 2024 by model, region, fuel type, and transmission.

![BMW Sales Dashboard](images/dashboard.png)

## Project Overview

This project turns a 50,000-row BMW sales dataset into a one-page Power BI dashboard. It shows headline KPIs and lets users filter by model and fuel type to see how sales change across years, regions, and vehicle types.

## Business Questions

- How have BMW sales changed from 2010 to 2024?
- Which regions and models sell the most?
- How do fuel type and transmission relate to sales volume?
- What are the total revenue, average price, and average mileage?

## Dataset

- **Source:** [add the source and link]
- **Size:** 50,000 rows and 11 columns
- **Period:** 2010 to 2024
- **Fields:** Model, Year, Region, Color, Fuel_Type, Transmission, Engine_Size_L, Mileage_KM, Price_USD, Sales_Volume, Sales_Classification
- **Note:** [add if true: The figures come from a sample dataset and are not official BMW sales records.]

## Tools Used

- Power BI Desktop
- DAX
- Power Query

## Methodology

1. **Data loading:** imported the CSV file into Power BI with Power Query and set the correct data types for all 11 columns.
2. **Data quality checks:** checked every column for missing values and the table for duplicate rows. None were found.
3. **DAX measures:** created the measures below.
4. **Dashboard design:** built KPI cards, slicers, and charts on one page.

| Measure | Logic |
|---|---|
| Total Sales | Sum of Sales_Volume |
| Total Revenue | Sum of (Price_USD x Sales_Volume) for each row |
| Average Price | Average of Price_USD |
| Average Mileage | Average of Mileage_KM |

## Dashboard Features

- **KPI cards:** Total Sales, Total Revenue, Average Price, Average Mileage
- **Slicers:** Model and Fuel Type
- **Line chart:** total sales by year
- **Bar charts:** total sales by region, model, fuel type, and transmission
- **Dynamic tooltip text** that updates with the selected model and fuel type

## Key Findings

- Total sales volume across 2010 to 2024 is about **253.4 million**. The average price is about **$75,035** and the average mileage is about **100,307 km**.
- Sales are spread very evenly. **Asia** leads the regions with about 43.0 million, only about 3.4% above the lowest region, South America (about 41.6 million).
- The **7 Series** is the top model (about 23.8 million) and the **M3** is the lowest (about 22.3 million), a gap of about 6.4%.
- All four fuel types are close. **Hybrid** leads (about 64.5 million) and **Diesel** is lowest (about 62.4 million).
- **Manual** (about 127.4 million) and **Automatic** (about 126.0 million) are nearly equal.
- Yearly sales stayed between about 16.3 million and 17.9 million. The peak year was **2022** and the lowest year was **2023**.

## Recommendations

- No single region, model, or fuel type dominates sales, so growth is unlikely to come from focusing on one segment alone.
- Asia and Hybrid lead by small margins. They are worth monitoring, but the gaps are small.
- Next steps: add year-over-year growth, and compare High and Low sales classifications to look for stronger drivers.

## Limitations

- The findings are descriptive. No statistical tests were run, so small differences between categories should not be treated as significant.

## Repository Structure

- `data/`: [describe the files, e.g. the BMW sales dataset in CSV format]
- `images/`: [dashboard screenshots]
- [`BMW_Dashboard.pbix`: the Power BI file, if you add it to the repo]

## Author

**Geh Desmond Yembi Meh**
[LinkedIn](https://www.linkedin.com/in/desmond-yembi-4a897621b/) | [GitHub](https://github.com/Desmond-Yembi) | desmondyembi72@gmail.com
