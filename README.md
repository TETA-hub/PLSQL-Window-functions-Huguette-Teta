## Project Overview
A comprehensive implementation of SQL window functions for business analytics, featuring customer segmentation, sales trend analysis, and regional performance metrics using Mysql. This academic project demonstrates practical applications of analytical SQL for e-commerce business intelligence.

          A, Problem diffentiton

1.	Company: East African Goods
2.	Department: Sales & Marketing Analytics  

   2.Business Challenge:
 AfroMart needs to analyze customer purchasing patterns across East African regions to optimize inventory management, identify high-value customers, and develop targeted marketing campaigns. The company lacks data-driven insights into regional performance, customer segmentation, and sales trends.

 3.Expected Outcome:
Data-driven decisions for inventory optimization, customer retention strategies, and regional marketing focus based on quantitative analysis of sales patterns and customer behavior.

         B, Database Schema 
The database contain three related tables 
1.customers 
  .Customer_id
  .Name
  .Region
2.products
  .Product_id
  .Name
  .Category
3.transactions
  .Transaction_id
   .Customer_id
  .Product_id
  .Sales_date
  .Amount
  
It also contain an ER-Diagram there is ascreenshot for it

 Window Functions Implemented

1.RANK():
     This shows the top 5 products per region/quarter, 
  interpretation: it helps to know which products are popular in which areas and during which time of the year
2.SUM() OVER():
    This Runs monthly sales totals,
  interpretation: This shows the cumulative sales up to each month, helping to track overall growth.
3.LAG()/LEAD()
    Month-over-month growth
  interpretation:This helps to see if sales are increasing or decreasing from one month to the next.
4.NTILE(4):
    Customer quartiles 
 interpretation:This helps to identify which customers are the top spenders (top quartile) and which are the lowest (bottom quartile).   
5.AVG() OV:
    3-month moving averages
 interpretation: This smooths out short-term fluctuations and helps to see the underlying trend.

  Result Analysis
1.Descriptive (What Happened)

Electronics and Nairobi brought in the most sales.
January and July were the strongest months.

2.Diagnostic (Why It Happened)

Nairobi customers have higher income and electronics are expensive.
Bonuses and holidays increased spending in January and July.

3.Prescriptive (What To Do Next)

Take care of big spenders and keep basic goods in stock.
Advertise the right products in each region and give offers in slow months.

 References
1.	MYSQL8.0V VERSION-Window functions: https://dev.mysql.com/doc/refman/8.0/en/window-functions.html
2.	Mullins, C. S. (2020) - "Advanced SQL for Data Analysis" in Database Trends and Applications
3.	East Africa Business Council (2023) - "E-commerce Trends in East African Markets"
4.	Provost, F., & Fawcett, T. (2013) - Data Science for Business. O'Reilly Media.
5.	MYSQL Tutorial: https://www.mysqltutorial.org/mysql-window-functions/

“All sources were properly cited. Implementations and analysis represent original work. No AI-
generated content was copied without attribution or adaptation.”


 
	
