# Bike Buyer Demographics & Purchase Behavior Dashboard

An interactive Excel dashboard built with PivotTables, PivotCharts and slicers
to find which customers are most likely to buy a bike.

![Dashboard](images/Bike%20Buyer%20Demographics%20and%20Purchase%20Behavior%20Dashboard.png)

## Key findings
- 48.1% of the 1,000 customers bought a bike (481).
- Shorter commutes buy more: 58.6% at 2-5 miles and 54.6% at 0-1 miles, versus 29.7% beyond 10 miles.
- Customers with 0-1 cars buy at 57-61%, versus 36-39% for 2 or more cars.
- Ages 31-54 buy at 54.6%, versus 35.5% for ages 25-30 and 31.2% for 55+.
- Income is a weak predictor: the 30-50k band buys most (56.7%), while those over 90k buy at 48.6%.
- Best segment: ages 31-54 with 0-1 cars and a commute of 5 miles or less buy at 66.8% (361 customers).

## Data and cleaning
- Source: the public Bike Buyers sample dataset (1,026 raw rows).
- Removed 26 duplicate IDs (1,000 rows remain) and expanded coded values into readable labels.
- Added age brackets (Young Adult 25-30, Middle Age 31-54, Senior 55+), an income band column and a purchase flag using nested IF formulas.

## How it works
- PivotTables calculate purchase rate by segment (average of a 1/0 purchase flag).
- KPI cards (customers, bikes purchased, purchase rate, average income) are linked to a pivot with GETPIVOTDATA.
- Five slicers (Marital Status, Gender, Education, Occupation, Region) filter every chart and card.

## Limitations
These are patterns in one sample, not proof of cause. Some groups are small
(for example Partial High School, n = 76), and the data has no revenue or price information.

## Tools
Microsoft Excel: PivotTables, PivotCharts, slicers, GETPIVOTDATA, nested IF formulas, dashboard design.

## Files
- `Bike Store Sales Project.xlsx` - the workbook
- `images/` - dashboard screenshot

## Author
Mohammed Faisal Fardin Chowdhury - B.Sc. in CSE, IIUC
