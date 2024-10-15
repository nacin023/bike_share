# Bike Share Data Analysis

## 1. Background and Overview
**Project Context**:  
This project analyzes key performance indicators (KPIs) for a bike share company during 2021 and 2022. The primary goal is to guide decision-making for the upcoming calendar year, with a focus on determining whether prices should be raised.

**Main Goal**:  
To assess trends in revenue, profit, and rider demographics, and to recommend whether the company should raise prices in the upcoming year based on data-driven insights.

**Key Metrics (North Star KPIs)**:
- Total Revenue
- Total Profit
- Rider Demographics (Casual vs. Registered)
- Seasonal Revenue Trends
- Weekday Revenue Trends

**Data Sources**:
- Bike Share Datasets from 2021 and 2022.
- Cost data from a secondary dataset.

**Tools Used**:
- Microsoft SQL Server Management Studio for data preparation and queries.
- Power BI for data visualization and dashboard creation.

## 2. Data Structure Overview
**Dataset Summary**:  
The data consists of three datasets combined through SQL queries, containing information on daily bike rides, including variables such as season, year, rider type, number of riders, price, cost of goods sold (COGS), and calculated fields for revenue and profit.

**Key Metrics**:
- Revenue (calculated as `riders * price`)
- Profit (calculated as `revenue - COGS * riders`)
- Rider Demographics (Casual vs. Registered riders)

**Dimensions**:
- **Time**: Year, Season, Weekday, Hour
- **Location**: Data spans across all operational regions of the company.
- **Product**: Bike rides sold at varying prices between 2021 and 2022.

**Grain (Table Granularity)**:  
Each row represents the daily aggregated performance at the ride level.

**ERD**:  
[Insert ERD or link to image]

## 3. Executive Summary
**Key Insights Summary**:
1. **Revenue Growth**: Revenue increased by 106.20% from 2021 to 2022, despite a 25% price increase.
2. **Rider Demand**: The number of riders increased by 64.88%, signaling robust demand despite the price increase.
3. **Profit Stability**: The profit margin remained consistent, with only a slight decrease from 68.92% (2021) to 68.74% (2022).
   
**Dashboard Overview**:  
[Include image or link to the Power BI dashboard]

**Key Performance Metrics**:
- **Revenue Increase**: 106.20%
- **Profit Increase**: 105.65%
- **Rider Growth**: 64.88%
- **Price Increase**: 25.06%

## 4. Insights Deep Dive
**Insight 1: Revenue by Season**  
- **Quantified Value**: Season 3 (July-September) generated the highest revenue at $4.9M, followed by Season 2 ($4.2M), Season 4 ($3.9M), and Season 1 ($2.2M).
- **Business Impact**: Targeting promotions during peak seasons can maximize revenue.
- **Historical Trend/Story**: Peak revenue months were May through October, with a slight dip in colder months.
- **Sliced by Dimension**: Revenue varies seasonally, with the most significant increases seen in late spring through early fall.

**Insight 2: Rider Demographics**  
- **Quantified Value**: 81% of riders were registered users, while 18% were casual users.
- **Business Impact**: Encouraging casual riders to register could increase rider loyalty and ride frequency.
- **Sliced by Dimension**: Demographic breakdowns show minimal variance across days of the week.

**Insight 3: Weekday Revenue Trends**  
- **Quantified Value**: Friday, Saturday, and Sunday are the highest revenue-generating days, though there is no significant difference between weekdays.
- **Business Impact**: Potential to boost weekday sales through promotions or special offers targeting casual riders.

## 5. Recommendations
1. **Price Strategy**: Given the strong performance, a cautious price increase of 5-15% could be tested in certain regions to evaluate consumer response. However, further market research is advised to avoid alienating price-sensitive customers.
   
2. **Market Research**: Conduct surveys to assess customer satisfaction and pricing sensitivity, and analyze competitor pricing strategies. This will ensure any price adjustments remain competitive while maintaining demand.

3. **Loyalty Incentives**: Implement loyalty programs that offer registered users discounted rates, further encouraging casual riders to sign up and potentially increasing ride frequency.

4. **Performance Measurement Suggestions**: Track KPIs such as rider growth, profit margin, and customer retention rates post-price adjustment to evaluate the impact.

## Caveats and Assumptions
- Data is limited to 2021 and 2022, and may not fully capture longer-term trends.
- Assumptions were made regarding consistent COGS across regions, which could vary in reality.
