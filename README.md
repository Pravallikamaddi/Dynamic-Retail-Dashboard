# Dynamic Retail Dashboard

This repository contains a **Dynamic Retail Dashboard** that provides key insights into retail data. Built with sample data tables for orders, people, and returns, this dashboard dynamically displays metrics and analyses essential for monitoring sales, profitability, and customer segmentation. It allows users to gain a comprehensive view of retail performance across various dimensions, such as regions, customer segments, and product categories.

---

## Objective

The objective of this project is to create a dynamic retail dashboard that offers real-time insights into key metrics like total sales, profit, quantity sold, and order count, as well as advanced analyses based on customer segments, product categories, and regions. This dashboard serves as a tool for data-driven decision-making, enabling businesses to identify trends, analyze profitability, and optimize sales strategies.

## Significance

This dashboard helps users:
- **Monitor essential business metrics** such as sales, profit, order count, and profitability.
- **Gain insights into customer segmentation and product performance** by analyzing data by regions, segments, and product categories.
- **Identify top and bottom performers** within product categories and customer segments to help improve inventory and marketing strategies.
- **Make informed business decisions** by using a data-driven approach to understand and optimize sales and profitability across different regions.

---

## Data Overview

The dashboard uses three main data tables: `Orders`, `People`, and `Returns`.

### 1. Orders Table
Contains transaction details including customer and product data for each order.

**Sample Columns**:
- `Order ID`, `Order Date`, `Ship Date`, `Ship Mode`, `Customer ID`, `Customer Name`, `Segment`, `City`, `State`, `Country`, `Product ID`, `Category`, `Sub-Category`, `Sales`, `Quantity`, `Discount`, `Profit`, `Shipping Cost`, `Order Priority`

**Sample Data**:
| Row ID | Order ID       | Order Date | Ship Date | Ship Mode  | Customer ID | Customer Name   | Segment  | City           | State      | Country    | Market | Region   | Product ID        | Category   | Sub-Category | Product Name                                        | Sales   | Quantity | Discount | Profit   | Shipping Cost | Order Priority |
|--------|----------------|------------|-----------|------------|-------------|-----------------|----------|----------------|------------|------------|--------|----------|-------------------|------------|--------------|----------------------------------------------------|---------|----------|----------|----------|---------------|----------------|
| 32298  | CA-2012-124891 | 31-07-2020 | 31-07-2020 | Same Day   | RH-19495    | Rick Hansen     | Consumer | New York City  | New York   | United States | US  | East     | TEC-AC-10003033   | Technology | Accessories  | Plantronics CS510 - Wireless Headset               | 2309.65 | 7        | 0        | 762.1845 | 933.57       | Critical       |

### 2. People Table
Connects people with their respective regions for customer segmentation analysis.

**Sample Columns**:
- `Person`, `Region`

**Sample Data**:
| Person           | Region  |
|------------------|---------|
| Anna Andreadi    | Central |
| Chuck Magee      | South   |
| Kelly Williams   | East    |
| Matt Collister   | West    |

### 3. Returns Table
Tracks returns by order ID for return trend analysis.

**Sample Columns**:
- `Returned`, `Order ID`, `Market`

**Sample Data**:
| Returned | Order ID       | Market   |
|----------|----------------|----------|
| Yes      | MX-2013-168137 | LATAM    |
| Yes      | US-2011-165316 | LATAM    |

---

## Implemented KPIs and Analyses

### Key Performance Indicators (KPIs)
1. **Total Sales (💰)**: Total revenue from all sales.
2. **Total Profit (📈)**: Sum of all profit across transactions.
3. **Total Quantity (📦)**: Total quantity of products sold.
4. **Number of Orders (🛒)**: Total count of unique orders.
5. **Profitability (💹)**: Profit as a percentage of total sales.
6. **Average Discount (🔍)**: Average discount applied across transactions.

### Analysis Features
1. **Sales and Profit Analysis**: Graphical representation of sales and profit to assess overall performance.
2. **Category-wise Profit**: Breakdown of profit by product category.
3. **Segment-wise Sales Share**: Share of sales for each customer segment.
4. **Sales by Country**: Distribution of total sales across different countries.
5. **Top 5 and Bottom 5 Subcategories**: Identification of best and worst-performing subcategories.
6. **Yearly Sales Trend**: Analysis of year-over-year sales trends.

---

## Next Steps for Expansion

Planned analyses include:
1. **Return Analysis**: Examine return rates and trends across markets and customer segments.
2. **Top and Bottom Customers**: Identify the most and least profitable customers.
3. **Segment Analysis**: In-depth profitability and sales analysis by customer segment.
4. **Market Analysis**: Insights into market performance in different regions.
5. **Product Analysis**: Detailed analysis of product-specific metrics to improve inventory and sales strategies.

---

## Implementation Steps

### Step 1: Load and Clean Data
1. Import the `Orders`, `People`, and `Returns` tables into your data analysis tool (Excel, Power BI, or other).
2. Perform data cleaning:
   - Handle missing values.
   - Convert data types (e.g., dates and numbers).
   - Remove any duplicate records.

### Step 2: Integrate Data
1. Join the `Orders` and `Returns` tables using `Order ID` to incorporate return data with each order.
2. Link the `People` table with the `Orders` table based on `Region` to enrich data with region information.

### Step 3: Create KPI Table
1. Define a KPI table to store essential dynamic metrics, which will be calculated using formulas or calculated fields.

**Sample KPI Table**:

| Name           | Metric                | Symbol |
|----------------|-----------------------|--------|
| Total Sales    | Sum of Sales          | 💰     |
| Total Profit   | Sum of Profit         | 📈     |
| Total Quantity | Sum of Quantity       | 📦     |
| Number of Orders | Count of Order ID   | 🛒     |
| Profitability  | Sum of Profitability  | 💹     |
| Average Discount | Average of Discount | 🔍     |

### Step 4: Build the Dashboard
1. **Create KPIs**: Display dynamic values using the KPI table.
2. **Add Filters and Slicers**: Implement filters for `Category`, `Country`, `Segment`, and `Order Date` for flexible analysis.
3. **Visualize Data**:
   - Display total sales, profit, and other KPIs.
   - Use charts to represent sales, profit trends, and distribution.
   - Add top and bottom subcategories using bar charts.
4. **Yearly Trend Analysis**: Add line graphs to display year-over-year sales performance.

### Step 5: Generate and Interpret Insights
1. Use the visualizations and KPIs to interpret trends, segment performance, and return trends.
2. Share findings to inform strategies for improving sales, profit, and customer engagement.

---

## Conclusion

The **Dynamic Retail Dashboard** is a powerful tool for analyzing retail data, providing key insights into KPIs and other metrics across various segments, products, and regions. This dashboard not only allows for effective tracking of retail performance but also provides a strong foundation for further analysis, such as return analysis and customer insights. With these insights, businesses can make informed, data-driven decisions to optimize their operations and strategies.


