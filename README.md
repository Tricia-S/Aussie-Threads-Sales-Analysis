# Aussie-Threads-Sales-Analysis
Data Analysis presented to a Sales Manager at Aussie Threads


## Table Of Contents

1. Project Overview
   - Problem Statement
   - Scope of the Project
   - Objectives

2. Data Overview
   - Dataset Summary
   - Data Description

3. Analytical Framework
   - Exploratory Questions
   - Data Analysis and Visualizations

4. Stakeholder & Outcomes
   - Stakeholder Background
   - Actionable Insights
   - Dashboard

5. Future Enhancements

6. Conclusion & Resources
   - Conclusion
   - References

  
## Project Overview

### 1. Problem Statement

Company Background

![image](https://github.com/user-attachments/assets/440fa781-0245-4d32-844a-e565f63445ce)

Aussie Threads is a newly established online apparel e-commerce shop that has quickly become a rising star in Australia's fashion scene. Founded 10 months ago in 2023, the company has already made significant strides in establishing itself as a go-to destination for stylish, affordable, and comfortable clothing. With a strong emphasis on quality, sustainability, and customer satisfaction, Aussie Threads is capturing the attention of fashion-forward Australians across the country.

The sales manager at Aussie Threads requires a comprehensive and interactive dashboard to help with data-driven decision-making. The current lack of easily accessible and actionable insights from the sales and inventory data is hindering effective planning and performance tracking. As a data analyst, my task is to apply the Design Thinking process to better understand the sales manager’s needs, analyze the available data, and create a solution that provides clear, visual insights that can drive business decisions.

### 2. Scope of the Project

In this project, I will apply the Design Thinking process to explore the provided datasets and develop actionable insights for the sales manager at Aussie Threads. The project will utilize the 5 phases of the Design Thinking framework—Empathize, Define, Ideate, Prototype, and Test—focusing on delivering an interactive dashboard that addresses the sales manager's key needs.


### 3. Objectives

The main objective of the project is to perform an exploratory data analysis (EDA) on the provided datasets, extract meaningful insights, and present them in the form of a dashboard. This will enable the sales manager to make informed, data-driven decisions that can improve sales performance and operational efficiency. I will be assessed on the relevance, clarity, and effectiveness of the insights, as well as the design and functionality of the final dashboard.


## Data Overview

### 4. Dataset Summary

Definition of Attribute/Field

1.	Customer File
•	Customer_Code is a unique number which identifies a particular customer 
•	Customer_Age refers to customer’s age as of 2021

2.	Item File
•	Item_Code is a unique number to identify each item
•	Item_Selling_Price is the standard selling price of the item which the company sells it to customers.  The standard selling price may be different from Order Details File  Selling_Price_Per_Unit if the company offered seasonal promotions, special discounts or further marked up the standard selling price to customers.
•	On_Hand_Quantity refers to the balance of stocks as of 20 Nov 2021

3.	Order File
•	Order_No is a unique number to identify each sales order from one customer 
•	Customer_Code refers to a particular customer who placed an order (i.e. Order_No) to the company

4.	Order Details File (Keep track of the order details for each sales order placed by a customer)
•	Sales_No is a system generated number that uniquely identify each row 
•	Order_No is an order placed by a customer
Example:
Customer_Code = 64 has placed a sales order with Order_No = 1
The Order_No = 1 consists of 6 products in the Order Details file (Sales_No = 0 to 5)
In this scenario, the Customer “64” has made an order with order_id “1” for 6 products 

![image](https://github.com/user-attachments/assets/72257761-9106-42dc-b1cc-ced3905db84e)

•	Selling_Price_Per_Unit refers to the actual selling price that the company transacted including any discount given to customer
•	Cost_Per_Unit refers to the purchase price per unit that the company paid to supplier to bring in the product
•	Order_Quantity refers to the order quantity that placed by the customer


### 5. Data Description
The project centers on a new e-commerce apparel shop called Aussie Threads that has been operating in Australia for 10 months. Data from four flat files will be analyzed to build comprehensive Power BI reports and dashboards:

Customer.xlsx
Item.xlsx (quantity_on_hand as of 20 Nov 2021)
Order.xlsx
Order Details.xlsx

The structure of each dataset will be examined to meet stakeholder goals and to address actionable insights.


## Analytical Framework

### 6. Exploratory Questions
1.	Does the customer state impact products type demand? 
2.	What are top 10 most profitable items and how sellable are these items? And what item type are they categorised by?
3.	How does the total order quantity differ between customers of different generation groups?
4.	What is the trend of profit and sales over the past 10 months?
5.	What is the sales trend by season?


### 7. Data Analysis and Visualizations
1. Order demand by the customer state and item type

![image](https://github.com/user-attachments/assets/35b00340-9944-4eb2-8b93-5a6b25f12e9f)

From this visual, we can see that South Australia has the highest order volume of 1425 while the Northern Territory is the lowest in terms of order volume 1085. 

I think one of the few reasons why South Australia has had the highest sales is that this online apparel store, Aussie Threads might have targeted South Australia specifically with effective marketing and promotion strategies, resulting in increased visibility and awareness among the local population that would have caused a higher order volume as compared to the rest of the states. One reason as to why Queensland got the most order quantity for jackets by almost 1.5 times more than in the Northern Territory could be due to the differences in fashion trends and the customer preferences same with the rest of the states.  

2. Top 10 item Name by profit and their respective order quantities

![image](https://github.com/user-attachments/assets/e785e660-a276-458d-a00a-db91d4c3aebe)

![image](https://github.com/user-attachments/assets/f94546db-5cc6-43bf-8f50-b5fe4882c44c)

From this visual, we can see the best performing items in terms of profitability and how sellable they are. The top 10 items consist of 5 types of Jackets, 2 types of trousers, 4 types of shirts which shows that the items under the category of Jackets generally are the ones that bring in the most profit. With ‘Denim’ items being the most profitable item has a high order volume of about 2 times more than the order volume of ‘Chinos’ items which were ranked as the 10th most profitable item in this visual. From this list of top 10, we can also identify what was the fashion trend in the year of 2021 up to the month of October. 
 
We could also identify which items are needed to be restocked and we can work with the inventory manager on forecast demand that helps in maintaining optimal inventory levels and preventing stockouts.
 
We can also work with the purchasing manager to determine what products and quantities need to be purchased to meet projected sales demand and to maintain an optimal stock level.

3. Order Volume by Generation 

![image](https://github.com/user-attachments/assets/9a7e6403-fd53-47e6-8580-01b289b7524e)

This chart shows the percentage of the order volume from different generation groups. From this chart, it appears that the generation group, Baby Boomers have the highest order quantity compared to the other generation groups with almost 1/3 of the total order quantity coming from them. On the other hand, The Silent Generation has ordered 6 times less the amount compared to Baby Boomers. The order volume in percentage of Gen X and Millennials are very similar with only a 0.45% in difference. And the order volume of Gen X and Millennials and Baby Boomers are also in a similar range of around 25% and above which is almost 1/3 of the total order volume. This shows that the marketing schemes and targeted promotions should be based on Baby Boomers and Gen X as well as Millennials. I believe the one of the reasons why Baby Boomers have contributed to the order volume the most is due to the convenience of online shopping. Online shopping provides convenience and flexibility, allowing baby boomers to browse and buy products from the comfort of their homes, avoiding the need to visit physical stores. As baby boomers age, some may face health or mobility issues that make traditional shopping more challenging. Online shopping provides a practical solution for obtaining essential items without leaving home. On the other hand, it has been shown that the generation group, The Silent Generation has contributed the least in terms of order volume. This is likely because they haven’t adapted to online shopping and rely solely on physical retail shops.


4. Sales and profit trend

![image](https://github.com/user-attachments/assets/8566b5d7-a462-4092-a659-fe65800c67a7)

From this chart, the highest sales and profit was in the month of March period and the lowest sales and profit is in October period. October period is about 1.5 times lesser than the profit generated in March. 
 
The general trend in sales over the 10 months is decreasing with a number of fluctuations. There are a few inflection points in the sales trend, such as in the month of April and August. Sales reached a peak in March which is the start of autumn, and it has been shown in the sales trend by season visual that the sales during the season of august was the 2nd highest. Sales show a notable increase during the start of each season, while sales tend to dip slightly during the end of each season. Sales experienced multiple fluctuations in the first 4 months. Which was followed by a gentle increase in the next 3 months. In the last 3 months, there was only a gentle decrease in the trend ending at slightly under 100K in dollars.
 
There are a few inflection points in the profit trend, such as in the month of February and March and April. The trend in profits generally mirror the trend in sales with a higher range and more drastic fluctuations. Profits experienced multiple fluctuations in the first 4 months. Which was followed by a gentle increase in the next 3 months. In the last 3 months, there was only a gentle decrease in the trend ending at 14.2K in dollars. There were a few reasons as to why the sales were fluctuating dramatically in the first 4 months after the company’s opening. A few would be the growth phase of a company and Market Penetration.
 
This could also be because the company was in its growth phase, this can be referenced from a business perspective. In the growth phase, companies experience rapid sales growth. As sales increase rapidly, businesses start seeing profit once they pass the break-even point. However, since the profit cycle still lags the sales cycle, the profit level is not as high as sales. Thus, one example of that could be in the month of March the sales was at 131K in dollars while the profit had only reached 24.7K in dollars.
 
And surprisingly, the sales were quite high in the first month after the company’s opening. This could be due to market penetration. The sales may be so high because in the early stages, the company may be trying to establish its presence in the market. Intensive marketing and promotional efforts from the marketing team could lead to a sudden increase in sales initially. As these efforts subside or as competitors respond which leads to the fluctuations in the first few months after its opening.


## Stakeholder & Outcomes

### 8. Stakeholder Background
A sales manager’s responsibilities may vary from one organisation to another, but in general, sales managers are the business leaders who set sales objectives and quotas and encourage their team to meet them. They also manage the entire sales cycle, including forecasting and budgeting sales revenue, profit margin, recruitment, selection of sales personnel, and ensuring that proper training and performance evaluations are conducted. 
 
Apart from developing sales plans and performing data analysis, they actively seek new clients, convert leads from various marketing channels, and create short and long-term sales plans to meet objectives. While sticking to the revenue goals of the organisation, they explore opportunities to upsell and cross-sell to their existing customers and expand the sales pipeline through referrals from their current clients. The sales manager also focuses on managing customer relationships, identifying customer needs, and providing insights for product portfolio improvements based on customer feedback. Furthermore, they manage key accounts, develop new accounts, and oversee pre- to post-sales support activities, while striving to achieve the highest level of customer satisfaction.


### 9. Actionable Insights
1.	Conduct an in-depth analysis of historical data to discern customers' geographic locations and their corresponding order quantities for each item type. This is to explore potential correlations between customer locations and their apparel preferences. Consequently, this knowledge will facilitate improved strategic planning and enable the implementation of targeted marketing campaigns aimed at boosting overall sales. 

2.	Analyse the historical data to identify the top 10 in profitability and their order volume respectively. This can be calculated from the profit and the order quantity of each item name. By doing so, we can uncover popular clothing choices in each state in Australia and identify regions that drive significant sales. This helps us identify the high-performing items and allows us to focus on the production, supply chain, and marketing schemes on these items which helps to further boost sales and profitability.

3.	Firstly, categorize the ages of all the customers into generation groups. Then analyse the historical data to identify if the generation group the customers belong to affect their respective order quantities. Use this information to tailor marketing campaigns and promotions that specifically target each generation's preferences and buying behaviour, which could potentially lead to increased sales and customer loyalty. 

4.	Analyse the historical data to identify any patterns or trends in the sales data for over the past 10 months. Use these insights to make data-driven decisions, such as adjusting pricing strategies, optimizing inventory levels, or launching targeted promotions as marketing schemes, to improve overall business performance.

5.	Analyse the historical data to identify any seasonal trends and demand fluctuations. Based on the findings, develop season-specific marketing and sales strategies to capitalize on peak seasons and mitigate challenges during slower periods in Australia, ultimately maximizing revenue throughout the year.


### 10. Dashboard

![image](https://github.com/user-attachments/assets/83043dc2-1086-4db4-9453-5ef759a6b7d6)

## Future Enhancements

## Conclusion & Resources

### 11. Conclusion

### 12. References
