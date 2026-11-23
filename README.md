# Sales Performance Dashboard (Power BI)

A Power BI dashboard built as a course assignment, using a star-schema sales dataset of 600,000 orders from 2021 to 2024.

## What it shows
- Headline KPIs: Total Sales (1.53bn), Total Profit (299.89M), Total Orders (600K) and Profit % (19.6%)
- Monthly sales trend, with running total and year-on-year growth in the tooltip
- Sales by category, region and customer segment
- Top 10 products and top 10 stores by sales
- Slicers for date, region and category

## Data model
One fact table (`fact_sales`) connected to four dimension tables (customers, products, stores, promotions), plus a separate Date table marked as the date table. All relationships are one-to-many.

## Measures (DAX)
Total Sales, Total Profit, Total Orders, Profit %, Sales LY, YoY Growth %, Running Total

## Assumptions I made
- Region comes from the Stores table, because the Region column in the sales table did not match the store's region.
- Ship Date was left out, because many ship dates were earlier than the order date.

## What I found
 - Monthly sales stay between about 29M and 33M with no clear growth or decline. February is the lowest month in all four years, at roughly 29–30M. 
 - Technology leads categories, and East leads regions with North lowest a gap of about 100M. 
 - Consumer is the largest segment at 532.3M, then Corporate at 502.8M and Home Office at 496.1M, so the three are close.
 - Every top product and store is within a few percent of the others.
   
## Screenshots
<img width="1323" height="842" alt="Page 1" src="https://github.com/user-attachments/assets/ef6e763c-69e4-4ab0-b9bd-71f006034256" />
<img width="1217" height="721" alt="Page 2" src="https://github.com/user-attachments/assets/4813454d-1e6d-468c-b6ad-a955f88be65a" />
<img width="1207" height="687" alt="Page 3" src="https://github.com/user-attachments/assets/c71fcfb6-f96a-40b1-b443-16461d43ab13" />


## Files
 - Sales_Dashboard.pbix (https://drive.google.com/file/d/1RUt01l5g9CHHX2exDyBuWgef77C_6Jks/view?usp=sharing) : the Power BI file (open in Power BI Desktop)

## Tools
Power BI Desktop, Power Query, DAX
