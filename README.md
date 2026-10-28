# Online Fashion Store Sales Analysis (Microsoft Excel Dashboard)

## 1. Project Overview
This project analyzes one year (2022) of online order data from an Indian fashion store. I used Microsoft Excel PivotTables, charts, and slicers to build an interactive annual report dashboard that shows sales trends, customer segments, order status, top states, and sales channels.

**Note:** This project uses a practice dataset. The findings are for learning purposes and are not real business conclusions.

## 2. Business Questions
1. How do orders and sales change month by month?
2. How do sales differ between men and women?
3. What share of orders are delivered, returned, cancelled, or refunded?
4. Which five states generate the most sales?
5. How do orders differ across age groups and gender?
6. Which sales channels bring the most orders?

## 3. Tools Used
- Microsoft Excel: PivotTables, PivotCharts, Slicers, Dashboard design

## 4. Dataset Description
| Item | Detail |
|---|---|
| Rows | 31,047 order records |
| Columns | 21 |
| Period | January to December 2022 |
| Currency | INR (Rs) |
| Total sales | Rs 21,176,377 (about Rs 21.18M) |

Key columns: Order ID, Cust ID, Gender, Age, Age Group, Date, Month, Status, Channel, SKU, Category, Size, Qty, Amount, ship-city, ship-state, B2B.

**Data check:** The dataset has no missing values and no exact duplicate rows, so no cleaning was needed. The `Order ID` column contains 28,471 unique IDs across 31,047 rows (some orders have more than one line), so "orders" in this project means order records.

## 5. Methodology (Steps Performed)
1. Loaded the dataset into Excel and reviewed its structure and columns.
2. Created one PivotTable per business question, each on its own sheet:
   - `Orders Vs Sales`: monthly sales (Sum of Amount) and order count (Count of Order ID)
   - `Men vs Women`: sales by gender
   - `Order Status`: share of orders by status
   - `Top States`: top 5 states by sales
   - `Age n Gender`: orders by age group and gender
   - `Channels`: share of orders by sales channel
3. Built a chart from each PivotTable (combo, pie, bar, and column charts).
4. Added slicers for Month, Channel, and Category so that the dashboard can be filtered.
5. Combined all charts and slicers on one dashboard sheet, `Store's Report 2022`.

## 6. Dashboard Components
| Chart | Type | Question Answered |
|---|---|---|
| Orders vs Sales | Column + line | Monthly trend |
| Sales: Men vs Women | Pie | Gender split |
| Order Status | Pie | Delivery performance |
| Sales: Top 5 States | Bar | Geographic performance |
| Orders: Age vs Gender | Column | Customer segments |
| Orders: Channels | Pie | Channel share |

## 7. Key Insights
1. **Monthly trend:** Sales and orders peak in March (Rs 1.93M, 2,819 orders) and then decline gradually, with the lowest sales in November (Rs 1.62M).
2. **Gender:** Women account for 64% of sales and men for 36%.
3. **Order status:** 92% of orders are delivered. Returned (3.4%), cancelled (2.7%), and refunded (1.7%) orders together make up about 8%.
4. **Top states:** Maharashtra (Rs 2.99M), Karnataka (Rs 2.65M), Uttar Pradesh (Rs 2.10M), Telangana (Rs 1.71M), and Tamil Nadu (Rs 1.68M).
5. **Customer segments:** Adult women are the largest group at 34.6% of orders, followed by teenage women (21.1%) and adult men (15.5%).
6. **Channels:** Amazon brings the most orders (35%), followed by Myntra (23%) and Flipkart (22%). Together they account for about 80% of orders.
7. **Category:** "Set" is the largest category at about 50% of sales, followed by kurta (23%).

## 8. Recommendations
- Focus marketing and stock planning on women customers and on the Amazon, Myntra, and Flipkart channels.
- Investigate why sales decline after March and prepare promotions for the weaker months at the end of the year.
- Review the causes of returns and cancellations to bring the 8% non-delivered share down.
- Strengthen delivery and promotions in the top five states.

## 9. Skills Demonstrated
Data Analysis, Exploratory Data Analysis (EDA), PivotTables, Data Visualization, Dashboard Design, Interactive Slicers, Business Insights

## 10. Repository Contents
| File | Description |
|---|---|
| `Online_Fashion_Store_Sales_Analysis.xlsx` | Workbook with the dataset, PivotTables, charts, and dashboard |
| `dashboard.png` | Dashboard screenshot |
| `README.md` | Project documentation |

## 11. Limitations
- The analysis covers one year and does not include costs or profit, so conclusions are about sales, not profitability.
- The dataset is a practice dataset, so the findings are not real business results.
- The analysis is descriptive. It does not include forecasting or statistical testing.
