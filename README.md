# Hardware-Sales-Insights
Created a Power BI-based report to check the sales patterns throughout the years and months.


ATLIQ HARDWARE is a company that supplies computer hardware and peripherals to many clients across India. The Sales Director of the company faces a lot of challenges. He is facing issues in terms of tracking sales, revenue, and many more.

To tackle this issue, we have created a Power BI-based report along with the dashboard to check the sales patterns throughout the years and months.

Report shows:
1. Revenue
2. Sales Quantity
3. Revenue by zones
4. Sales Quantity by zones
5. Revenue by Markets
6. Sales Quantity by Markets
7. Top 5 Customer Name in terms of Revenue
8. Top 5 Customer Name in terms of Sales Quantity
9. Revenue Trend

Skills needed to complete the job:
1. Data Cleansing
2. DAX language
3. Analytical Skills
4. Business Intelligence Knowledge
5. SQL Query Language

Below are some of the queries which we can run to validate our results from the Power BI visuals:-

1. Below query will tell us the Revenue generated in the month of February and in the year 2020 -
select sum(t.sales_amount) from transactions t inner join date d on t.order_date= d.date
where d.year= 2020 and d.month_name = "February" and (t.currency = 'INR\r' or t.currency = 'USD\r');

2. Also we can find the Revenue generated for particular region, as I have find for "Mumbai" -
select sum(t.sales_amount) from transactions t inner join date d on t.order_date= d.date
where d.year= 2020 and t.market_code = "Mark002" and (t.currency = 'INR\r' or t.currency = 'USD\r'); 
