Overview of the Dynamic Retail Dashboard
The Dynamic Retail Dashboard offers a clear and interactive view of key business metrics such as sales, profit, returns, and customer orders. With slicers for Market, Region, Category, Sales Person, and Order Date, users can easily filter and explore data to gain actionable insights.

The dashboard helps monitor return rates, track shipment performance, and assess sales team effectiveness by linking sales representatives to their assigned regions. This allows for quick identification of improvement areas, supporting better decision-making to boost efficiency, profitability, and customer satisfaction.

sample data of Order Table

| Order ID | Market | Region | Category        | Sub-Category | Sales | Profit | Returns | Customer Name  | Sales Person   | Order Date |
| -------- | ------ | ------ | --------------- | ------------ | ----- | ------ | ------- | -------------- | -------------- | ---------- |
| ORD001   | APAC   | East   | Technology      | Phones       | 1500  | 300    | No      | John Doe       | Emily Smith    | 2024-01-15 |
| ORD002   | EU     | West   | Furniture       | Chairs       | 800   | 120    | Yes     | Alice Brown    | Michael Lee    | 2024-02-10 |
| ORD003   | US     | South  | Office Supplies | Paper        | 200   | 30     | No      | Chris Green    | Olivia Johnson | 2024-02-25 |
| ORD004   | APAC   | North  | Technology      | Laptops      | 2500  | 500    | No      | David White    | Emily Smith    | 2024-03-05 |
| ORD005   | EU     | East   | Furniture       | Tables       | 1200  | 250    | Yes     | Emma Black     | Michael Lee    | 2024-03-18 |
| ORD006   | US     | West   | Office Supplies | Binders      | 300   | 45     | No      | Liam Grey      | Olivia Johnson | 2024-04-01 |
| ORD007   | APAC   | South  | Technology      | Accessories  | 600   | 100    | No      | Noah Young     | Emily Smith    | 2024-04-12 |
| ORD008   | EU     | North  | Furniture       | Bookcases    | 950   | 180    | No      | Olivia King    | Michael Lee    | 2024-04-25 |
| ORD009   | US     | East   | Office Supplies | Envelopes    | 150   | 20     | Yes     | Ava Hill       | Olivia Johnson | 2024-05-03 |
| ORD010   | APAC   | West   | Technology      | Copiers      | 3000  | 600    | No      | Isabella Scott | Emily Smith    | 2024-05-15 |


people Table

| Sales Person   | Region |
| -------------- | ------ |
| Emily Smith    | East   |
| Michael Lee    | West   |
| Olivia Johnson | South  |
| David Miller   | North  |

Return Table

| Order ID | Returned |
| -------- | -------- |
| ORD002   | Yes      |
| ORD005   | Yes      |
| ORD009   | Yes      |
| ORD001   | No       |
| ORD003   | No       |
| ORD004   | No       |
| ORD006   | No       |
| ORD007   | No       |
| ORD008   | No       |
| ORD010   | No       |

KPI's Table

| KPI's                | Name           | Symbol |
| -------------------- | -------------- | ------ |
| Sum of Sales         | Total Sales    | 📈     |
| Sum of Profit        | Total Profit   | 💰     |
| Sum of Quantity      | Total Quantity | 📦     |
| Count of Order ID    | No of orders   | 🛒     |
| Sum of Profit Margin | Profit Margin  | 🔍     |

But your KPI Card Values show this:
| Total Sales  | Total Profit | Total Quantity | No of Orders | Profit Margin |
| ------------ | ------------ | -------------- | ------------ | ------------- |
| ₹ 12,642,502 | ₹ 1,467,457  | 178,312        | 51,290       | 11.61%        |

Problem Description:

1- Profit Margin Calculation Issue:
Your KPI table suggests "Sum of Profit Margin" — which is incorrect, because profit margin should not be summed.
Profit Margin = (Total Profit / Total Sales) * 100
In the final KPI card, the correct calculated 11.61% is shown — but your KPI table says "Sum of Profit Margin", which is misleading.

2- Incorrect KPI Description:
Count of Order ID is correct as it counts orders.
But for Profit Margin, you should write:
"Calculated Profit Margin = (Total Profit / Total Sales) * 100" instead of "Sum of Profit Margin".

Solution Description:

1️⃣ Total Sales (₹12,642,502)
Description:
Total Sales represents the complete revenue generated from all customer purchases over the given period. This value shows the business’s overall ability to generate income by selling products to its customers. A higher total sales figure indicates a strong market demand and effective selling strategies.

2️⃣ Total Profit (₹1,467,457)
Description:
Total Profit indicates how much money the company has earned after covering all costs associated with the products sold. It reflects the business's efficiency in managing costs and pricing products. A positive profit shows that the company is running successfully, whereas negative profit would indicate potential issues in pricing, costs, or sales.

3️⃣ Total Quantity Sold (178,312 Units)
Description:
This metric shows the total number of product units sold to customers. It helps in understanding the scale of operations and product demand. A larger quantity sold reflects strong product acceptance and higher customer demand in the market.

4️⃣ Number of Orders (51,290 Orders)
Description:
This value reflects the total number of individual purchase orders placed by customers. It is a useful indicator to measure order volume, customer activity, and engagement level. More orders typically imply greater customer reach and market penetration.

5️⃣ Profit Margin (11.61%)
Description:
Profit Margin shows the percentage of revenue that remains as profit after all costs are deducted. It is a critical measure of how efficiently the company converts sales into actual profit. A healthy profit margin indicates good pricing strategies, cost control, and overall profitability of the business.

Summary Table:
| KPI            | Description                                                                                   | Value         |
| -------------- | --------------------------------------------------------------------------------------------- | ------------- |
| Total Sales    | Overall revenue earned from selling products to customers.                                    | ₹12,642,502   |
| Total Profit   | Total money earned after covering the costs of goods sold.                                    | ₹1,467,457    |
| Total Quantity | Total number of product units sold to customers.                                              | 178,312 Units |
| No of Orders   | Total count of orders placed by customers.                                                    | 51,290 Orders |
| Profit Margin  | Percentage of total sales that turned into profit, reflecting overall business profitability. | 11.61%        |


