# Executive Tableau Dashboard for Retail Business Performance

## Business Problem Summary

This project develops an executive Tableau dashboard to help retail leadership monitor business performance and support strategic decision-making. The dashboard provides insights into sales trends, regional performance, category profitability, customer segments, shipping performance, discount impact, and return patterns.

---

# Dataset Description

The dataset contains retail transaction information including:

- Order Date
- Order ID
- Customer ID
- Region
- State
- City
- Category
- Sub Category
- Customer Segment
- Ship Mode
- Campaign Channel
- Sales
- Profit
- Quantity
- Discount
- Delivery Days
- Customer Rating
- Return Flag

The data was connected directly to Tableau and appropriate data types were verified before analysis.

---

# Tableau Workbook Description

Workbook Name:

**executive_dashboard.twbx**

The workbook contains multiple worksheets and one executive dashboard designed for business leadership.

Included Views:

- Sales Trend View
- Regional Performance View
- Category Profitability View
- Customer Segment View
- Shipping Performance View
- Discount vs Profit View
- Return Analysis View
- Executive Dashboard

---

# Calculated Fields Created

The following calculated fields were created in Tableau:

| Calculated Field | Formula |
|------------------|---------|
| Profit Margin | Profit / Sales |
| Cost | Sales - Profit |
| Average Order Value | Sales / COUNTD(Order ID) |
| Return Rate | AVG(Return Flag) |
| Shipping Delay Bucket | Delivery Days grouped into delay categories |

---

# Dashboard Components

The executive dashboard includes:

- Total Sales KPI
- Total Profit KPI
- Profit Margin KPI
- Sales Trend Analysis
- Regional Performance
- Category Profitability
- Shipping Performance
- State Sales Map

---

# Filters and Interactions Used

Interactive dashboard filters include:

- Region
- Category
- Customer Segment
- Ship Mode

Dashboard Action:

- Selecting a region filters the remaining dashboard views for detailed regional analysis.

---

# Key Business Insights

- Sales remain relatively stable throughout the reporting period.
- South region generates the highest sales and profit.
- Technology is the most profitable product category.
- Customer segments contribute differently to overall revenue.
- Higher discounts do not always improve profitability.
- Shipping performance differs across shipping modes.
- Return analysis helps identify areas requiring operational improvement.
- Geographic analysis highlights opportunities for regional expansion.

---

# Dashboard Story Summary

The dashboard presents business performance from a leadership perspective by combining KPIs with operational and financial insights. It highlights high-performing regions and categories while identifying areas requiring improvement such as shipping efficiency and discount strategy. The dashboard supports data-driven business decisions by connecting sales, profitability, customer behaviour, and operational performance into one interactive view.

---

# Assumptions and Limitations

## Assumptions

- Dataset values are complete and accurate.
- Return Flag correctly identifies returned orders.
- Delivery Days accurately represent shipping performance.
- Sales and Profit values are correctly recorded.

## Limitations

- Dashboard is based on historical data only.
- External factors such as market competition, inflation, and seasonality are not included.
- Dashboard identifies business associations but does not establish causation.

---

# Screenshots Included

The repository contains the following screenshots:

- full_dashboard.png
- sales_trend_view.png
- regional_performance_view.png
- category_profitability_view.png
- filter_interaction_view.png

---

# Repository Structure

```
part4_tableau_dashboard/
├── data/
│   └── dashboard_sales_data.xlsx
├── tableau/
│   └── executive_dashboard.twbx
├── outputs/
│   ├── dashboard_story.md
│   ├── business_insights.md
│   └── chart_selection_justification.md
├── screenshots/
│   ├── full_dashboard.png
│   ├── sales_trend_view.png
│   ├── regional_performance_view.png
│   ├── category_profitability_view.png
│   └── filter_interaction_view.png
└── README.md
```

## Conclusion

This Tableau dashboard provides an interactive and business-focused overview of retail performance. It enables leadership to monitor key metrics, compare business performance across regions and categories, evaluate operational efficiency, and identify opportunities for improving profitability and future growth.
