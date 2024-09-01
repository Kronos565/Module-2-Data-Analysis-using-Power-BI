# Power BI Portfolio: Detailed Sales and Financial Performance Analysis

## Overview

This Power BI portfolio project offers a comprehensive analysis of sales and financial performance across various business segments, countries, and products. The dashboard is designed for interactivity, enabling users to filter data based on segments and other key metrics, uncovering valuable insights into business operations.

## Features

- **Interactive Slicer:** The dashboard includes a segment slicer that allows users to filter the visualizations by different business segments, such as Channel Partners, Enterprise, Government, Midmarket, and Small Business.
  
- **Detailed Sales and Financial Performance Dashboard (Page 1):**
  - **Total Profit by Year and Segment:** A line chart visualizing the sum of total profit across years, segmented by business type, highlighting trends in profitability.
  - **Total Sales by Product and Segment:** A bar chart displaying the total sales for each product, segmented by business type, revealing product performance differences across segments.
  - **Total Units Sold by Segment and Country:** A clustered bar chart showing the total units sold in each segment, broken down by country, to identify strong markets and growth opportunities.
  - **Total Discounts and Total Units Sold by Segment and Year:** A combo chart showing the relationship between discounts offered and units sold over the years, offering insights into the impact of pricing strategies.
  - **Gross Sales Summary:** A card visual summarizing the gross sales value, providing a quick snapshot of overall sales performance.
  - **Segment Breakdown:** A tree map providing a visual breakdown of the segments, offering insights into segment contributions to the overall business.

- **Detailed Sales Insight Dashboard (Page 2):**
  - **Detailed Sales Insight Table:** A table offering a detailed view of total profit and units sold by country, product, and segment, enabling granular analysis.
  - **Discounts by Segment:** A pie chart representing the distribution of total discounts across segments, highlighting which segments are more discount-driven.
  - **Total Discounts and Total Units Sold by Product and Segment:** A stacked area chart visualizing the cumulative discounts and units sold for each product across segments, indicating the correlation between discounting and sales volume.

## Key Insights and Trends

- **Profitability Trends:** The **Total Profit by Year and Segment** chart reveals that the Government and Enterprise segments have shown steady growth in profitability, while the Channel Partners segment is volatile, possibly due to market conditions or competitive pressures.

- **Product Performance:** Analysis from the **Total Sales by Product and Segment** chart indicates that specific products such as 'Fosco' and 'Velo' are top performers in the Enterprise and Channel Partners segments, respectively, suggesting a targeted sales strategy.

- **Market Strength:** The **Total Units Sold by Segment and Country** chart identifies Canada and Germany as strong markets for the Enterprise segment, presenting opportunities for further market penetration.

- **Impact of Discounts:** Insights from the **Total Discounts and Total Units Sold by Segment and Year** chart suggest that while discounts drive volume in the Channel Partners segment, they do not significantly impact the Enterprise segment, indicating different customer sensitivity to pricing.

- **Segment Contribution:** The **Segment Breakdown** tree map shows that the Midmarket and Small Business segments contribute significantly to overall sales, which could inform future marketing and sales strategies.

## Data

The data used in this project is derived from the `financials` table, which includes key columns such as:

- `Segment`
- `Country`
- `Product`
- `Units Sold`
- `Sale Price`
- `COGS (Cost of Goods Sold)`
- `Profit`
- `Discounts`
- `Year`

## DAX Calculations

This project leverages several DAX formulas to create calculated tables and measures, ensuring accurate analysis and insights:

- **SalesByProductTable:** A summary of total sales, units sold, and profit by product.
- **SegmentCountryCOGSmetricsTable:** COGS and profit metrics summarized by segment and country.
- **UnitsAndDiscountsBySegmentYearTable:** Total units sold and discounts summarized by segment and year.
- **DetailedSalesInsightsTable:** A union of two tables to capture total units sold and profit by country and segment, with or without product details.
- **DiscountImpactByProductTable:** Calculation of discount impact for products where the discount exceeds 10%.
- **DiscountsAndAveragePriceByCountryYearTable:** A summary of discounts and average sale price by country and year.
- **ProfitBySegmentYearTable:** Calculation of profit by segment and year.

## How to Use

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/your-repository.git
