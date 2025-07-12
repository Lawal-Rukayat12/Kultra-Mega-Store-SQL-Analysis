
📊 SQL Case Study: Kultra Mega Store Analysis  
Comprehensive SQL case study analysis for Kultra Mega Stores' inventory and sales data. Includes data cleaning, business insight queries, shipping cost evaluation, customer segmentation, and performance breakdowns.

---

📝 **INTRODUCTION**  
Kultra Mega Stores (KMS) is a rapidly expanding retail chain in Nigeria, with operations primarily in Lagos and Abuja. This SQL case study explores historical inventory and sales data (2009–2012) to extract insights into product demand, shipping efficiency, customer segmentation, and profitability using SQL.

---

📖 **BACKGROUND**  
As a Business Intelligence Analyst, I analyzed KMS’s operational data to provide strategic insights. The project focuses on sales trends, customer behavior, logistics optimization, and revenue opportunities.

Key questions addressed include:
- Which product categories drive the most revenue?
- Who are the most profitable customers?
- Where can operational costs be reduced, especially in shipping?

---

🎯 **OBJECTIVES**
- Identify best-selling product categories
- Analyze regional sales performance
- Evaluate appliance sales in Ontario
- Recommend actions for low-spending customers
- Identify costliest shipping methods
- Determine high-value and returning customers
- Check alignment of shipping mode with order priority

---

📂 **DATA OVERVIEW**
**Dataset Origin**: Digital Skills Africa / Incubator Hub  
**Key Table**: KMS SQL Case Study  
**Key Fields**:
- Product Category/Sub-Category
- Sales, Profits, Discounts
- Customer Segment, Region, Province
- Ship Mode, Shipping Cost
- Order Dates and Priority

---

🛠 **TOOLS USED**
- SQL Server Management Studio (SSMS)
- Power BI (for visualization)
- GitHub (for version control)
- SQL functions (GROUP BY, WHERE, JOIN, etc.)

---

📈 **KEY ANALYSIS & INSIGHTS**

1. **Top-Selling Product**  
*Query:* `SELECT Product_Name, SUM(Sales) FROM ... GROUP BY Product_Name ORDER BY SUM(Sales) DESC`  
🔍 *Insight*: Global Troy™ Executive Leather Low-Back Tilter topped sales with ₦275,941.52.

2. **Regional Sales Performance**  
*Query:* Total sales grouped by Region  
🔍 *Insight*: Top 3 regions – West, Ontario, Prairie. Bottom 3 – Atlantic, Quebec, Northwest Territories.

3. **Ontario Appliance Sales**  
*Query:* Sales WHERE Region = 'Ontario' AND Sub_Category = 'Appliances'  
🔍 *Insight*: ₦202,346.84 worth of appliances sold in Ontario.

4. **Bottom 10 Customers**  
*Analysis*: Low order frequency, lower average order value.  
🔍 *Recommendation*: Offer promotions and personalized offers to boost engagement.

5. **Costliest Shipping Method**  
*Query:* `GROUP BY Ship_Mode ORDER BY SUM(Shipping_Cost)`  
🔍 *Insight*: Delivery Truck incurred the highest total cost (₦51,971.94).

6. **Most Valuable Customers**  
*Query:* Top 5 by Profit and Product Sub-Category  
🔍 *Top Customers*: Emily Phan, Grant Carroll, Raymond Book...

7. **Small Business Top Performer**  
*Query:* Top 1 in Small Business Segment by Sales  
🔍 *Insight*: Dennis Kane – ₦75,967.59 in sales.

8. **Top Corporate Client (2009–2012)**  
*Query:* COUNT(Order_ID) for 'Corporate' segment  
🔍 *Insight*: Adam Hart placed 27 orders, highest among corporate clients.

9. **Most Profitable Consumer**  
*Query:* SUM(Profit) for 'Consumer' segment  
🔍 *Insight*: Emily Phan – ₦34,005.44 profit.

10. **Returned Items by Segment**  
*Query:* `WHERE Profit < 0`  
🔍 *Insight*: Returns seen across all segments, suggesting review of return policies.

11. **Shipping Cost vs Order Priority**  
*Insight*: Low-priority orders incur higher shipping costs than critical ones – a clear mismatch.  
📊 **Recommendations**:
- Use Delivery Truck for low-priority
- Automate shipping based on order urgency
- Track KPIs monthly

---

📌 **FINAL CONCLUSION**  
This case study highlights how SQL analysis helps optimize inventory, customer targeting, and shipping cost strategies at KMS. It lays a strong foundation for future automation, Power BI integration, and advanced analytics.

---

👤 **Author**  
Lawal Rukayat Ayomide  
📧 Email: rukayat12@gmail.com
