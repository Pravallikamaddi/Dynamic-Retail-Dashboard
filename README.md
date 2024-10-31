# Dynamic Retail Dashboard

This repository contains a **Dynamic Retail Dashboard** built using three tables: **Orders**, **People**, and **Returns**. The dashboard provides insightful analyses and key performance indicators (KPIs) that facilitate better understanding and decision-making in retail management.

---

## Objective

The main objective of this project is to create a dynamic and interactive dashboard that displays critical metrics related to retail performance. The dashboard aims to enable users to:
- Monitor total sales, profits, and order statistics.
- Analyze sales trends by category, segment, and region.
- Make informed business decisions based on data-driven insights.

---

## Data Overview

The dashboard utilizes three key data tables:

### 1. Orders Table

The **Orders** table includes transaction details such as customer and product information.

**Sample Data**:
| Row ID | Order ID       | Order Date | Ship Date | Ship Mode  | Customer ID | Customer Name   | Segment  | City           | State      | Country       | Postal Code | Market | Region | Product ID        | Category   | Sub-Category | Product Name                                        | Sales   | Quantity | Discount | Profit   | Shipping Cost | Order Priority |
|--------|----------------|------------|-----------|------------|-------------|-----------------|----------|----------------|------------|---------------|-------------|--------|--------|-------------------|------------|--------------|----------------------------------------------------|---------|----------|----------|----------|----------------|----------------|
| 32298  | CA-2012-124891 | 31-07-2020 | 31-07-2020 | Same Day   | RH-19495    | Rick Hansen     | Consumer | New York City  | New York   | United States | 10024       | US     | East   | TEC-AC-10003033   | Technology | Accessories  | Plantronics CS510 - Wireless Headset               | 2309.65 | 7        | 0        | 762.1845 | 933.57        | Critical       |

### 2. People Table

The **People** table provides information about customer regions for segmentation analysis.

**Sample Data**:
| Person           | Region  |
|------------------|---------|
| Anna Andreadi    | Central |
| Chuck Magee      | South   |
| Kelly Williams   | East    |
| Matt Collister   | West    |

### 3. Returns Table

The **Returns** table tracks the return status of orders.

**Sample Data**:
| Returned | Order ID       | Market   |
|----------|----------------|----------|
| Yes      | MX-2013-168137 | LATAM    |
| Yes      | US-2011-165316 | LATAM    |
| Yes      | ES-2013-1525878| EU       |
| Yes      | CA-2013-118311 | United States |

---

## Solved Problem Questions

The following analyses have been conducted to derive insights from the data:

1. **KPIs**: Total sales, total profit, quantity, number of orders, and profit margin.
   ![image](https://github.com/user-attachments/assets/1f74e74a-07ac-42f0-bc03-0d3cd6859118)

2. **Sales and Profit Analysis**: Understanding the relationship between sales and profitability.
3. **Category-wise Profit**: Analyzing profit contributions from different categories.
4. **Segment-wise Sales Share**: Evaluating sales distribution across customer segments.
5. **Sales by Country**: Geographic analysis of sales performance.
6. **Top 5 Subcategories**: Identifying the highest-selling subcategories.
7. **Bottom 5 Subcategories**: Recognizing the lowest-performing subcategories.
8. **Yearly Sales Trend**: Visualizing sales performance over multiple years.

---

## Next Steps for Project Development

Future enhancements for the dashboard include:
- **Return Analysis**: Deep dive into return rates and their impacts on sales.
- **Top Customer Identification**: Discovering the most profitable customers.
- **Bottom Customer Analysis**: Identifying customers with the least profitability.
- **Segment Analysis**: Further understanding customer segments and their behavior.
- **Market Analysis**: Examining sales performance across different markets.
- **Product Analysis**: Detailed insights on product-level performance.

---

## Dynamic KPI Table

To ensure the dashboard is dynamic and user-friendly, a KPI table has been created with the following metrics:

| Name           | Metric                | Symbol |
|----------------|-----------------------|--------|
| Total Sales    | Sum of Sales          | 💰     |
| Total Profit   | Sum of Profit         | 📈     |
| Total Quantity | Sum of Quantity       | 📦     |
| No. of Orders  | Count of Order ID     | 🛒     |
| Profitability  | Sum of Profitability  | 💹     |
| Average Discount | Average of Discount  | 🔍     |

---

## Implementation Steps

### Step 1: Load and Clean Data
- Import the `Orders`, `People`, and `Returns` tables into your analysis tool (Excel, Power BI, etc.).
- Clean the data by handling missing values and converting data types.

### Step 2: Integrate Data
- Join the `Orders` and `Returns` tables using `Order ID` to incorporate return data.
- Link the `People` table to the `Orders` table based on `Region`.

### Step 3: Create the KPI Table
- Define a KPI table that calculates essential metrics for display on the dashboard.

### Step 4: Build the Dashboard
- **Create KPIs**: Display the dynamic values using the KPI table.
- **Add Filters and Slicers**: Implement filtering options for categories, countries, and segments.
- **Visualize Data**:
  - Show total sales and profits.
  - Use charts for sales trends and category analyses.
  - Identify top and bottom subcategories using bar graphs.
  - Add line graphs for yearly sales trends.

### Step 5: Generate and Interpret Insights
- Utilize the dashboard to interpret trends and performance metrics.
- Share insights with stakeholders to inform decision-making.

---

## Conclusion

The **Dynamic Retail Dashboard** serves as an essential tool for analyzing retail performance data. It provides critical insights into sales, profitability, and customer segmentation, enabling data-driven decisions. As the project evolves, additional analyses will further enhance its capabilities, making it an invaluable resource for retail management.
![image](https://github.com/user-attachments/assets/785de72c-4182-4cc2-8c04-89306903b0a3)

