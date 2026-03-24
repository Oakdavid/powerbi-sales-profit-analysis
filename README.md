# Sales and Profit Analysis Dashboard (Power BI)

## Overview

Power BI report built using the MPR dataset to analyze sales performance and identify key drivers of profit.

## Features

### Page 1: Sales Analysis

* Total Sales by Category with drill-down:

  * Category → Sub-Category → Product
* Total Sales by Region

  * Tooltip shows Sales by Segment

### Page 2: Profit Analysis

* Decomposition Tree for Total Profit:

  * Year → Quarter → Month → Region → Segment → Category
  * Default level set to Year
* Key Influencers visual for Profit Margin

## Tools

* Power BI
* Power Query
* DAX

## Key Measures

```DAX id="d8d9ja"
Total Sales = SUM(Orders[Sales])

Profit Margin = DIVIDE(SUM(Orders[Profit]), SUM(Orders[Sales]), 0)
```

## Insights

* Sales vary across regions and product categories
* High sales do not always mean high profit
* Profit margin is influenced by category and segment
* Time trends impact overall performance

## Usage

Open the `.pbix` file in Power BI Desktop and interact with the visuals.
