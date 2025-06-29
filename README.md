TECHNICAL REPORT FOR FASHION SALES ANALYSIS USING POWER BI

INTRODUCTION

The fashion industry changes quickly, and it’s important for businesses to understand what sells and why. With more people shopping online, using sales data can help make better decisions.

This report looks at fashion sales to find out which items sell the most, how price affects sales, and what customers like. The goal is to help fashion brands and retailers improve their sales, manage stock better, and give customers what they want.

Aim:
To analyze fashion sales data to identify trends, understand customer preferences, and support better sales and inventory decisions.

Objectives:

· To identify top-selling fashion items and categories.

· To analyze how pricing affects sales performance.

· To study seasonal or time-based trends in customer purchases.

· To understand which products, have high or low customer interest.

· To provide recommendations for improving sales and stock management

PROBLEM BEING ADDRESSED

Fashion retailers often struggle to understand which products sell well, what customers prefer, and how pricing or seasons affect sales. Without clear insights from sales data, it’s hard to make smart decisions about inventory, pricing, and marketing. This report aims to solve that problem by analyzing fashion sales data to find useful patterns and improve business performance.

KEY DATASET AND METHODOLOGIES

Dataset
The dataset used for this analysis includes information on fashion products such as Item Purchased, Payment Method, Date Purchased, Review Rating, Total customers, Purchase Amount, Total Purchased Amount, Customer Referenced ID. This data helps in understanding what items are popular, how pricing affects sales, and how trends change over time.

Methodologies:

· I used Power Query Editor for the Data Cleaning

· Checked for missing or inconsistent values

· Ensured consistent letters (e.g., uppercase or lower case)

· Ensured correct data types (e.g., numerical, text, date)

· Summarized key statistics like best-selling products, average price

· Studied how sales changed over time (e.g., by month or season).

· Compared sales performance across different product categories

· Created charts and graphs (using Power BI) to clearly present insights.

· Explored relationships between price, rating, and quantity sold.

STORY OF DATA

Fashion Sales dataset downloaded from Kaggle

Data structure: The Fashion dataset used in this analysis is structured in a flat table format, where each row represents a single transaction and each column represents a specific attribute such as Date Purchased, Payment Method, Review Rating, Item purchased, customer reference ID etc.

IMPORTANT FEATURES AND THEIR SIGNIFICANCE

Item Purchased

Significance: This Indicates which product was bought, it enables product-level performance analysis and helps identify popular items and trends

Purchase Amount

Significance: This Represents the transaction value. Critical for analyzing revenue, average transaction size and customer spending patterns.

Customer Reference ID

Significance: This uniquely identifies each customer, it is useful for tracking purchase behavior, repeat purchases, and building customer profiles

Date Purchased

Significance: This captures the exact purchase date. This allows for time series analysis, seasonal checks and peak sale period identification

Review Rating

Significance: This Reflects customer satisfaction, helps evaluate quality, customer experience, and its correlation with future sales

Payment Method

Significance: This Shows how the customer paid (e.g., credit card, cash etc.), helps in analyzing preferred payment modes and optimizing checkout experience

Weekdays (New calculated Column)

Significance: Extracted from purchase date to analyze sales performance by day of week. Useful for planning promotions, staffing, and scheduling restocks.

Data Cleaning

I used Power Query Editor for the Data Cleaning

Checked for missing or inconsistent values

Ensured consistent letters (e.g., uppercase or lower case)

Ensured correct data types (e.g., numerical, text, dates)

Data splitting

The data were split into two categories

Independent and dependent variables or value

PRE- ANALYSIS BOARD

Project Split

Category 1 independent Variables/values

Payment method

Item Purchased

Category 2 Dependent Variables/Values

Date Purchased

Review Rating

Total customers

Purchase Amount,

Total Purchased Amount

customer Referenced Id

Industry Type: the dataset is fashion sales dataset

Stakeholder: Company Management Team

DAX (DATA ANALYSIS EXPRESSION)

New Measures

DAX (Data analysis expression)

New Measures

Total Purchased Amount= sum (fashion-retail-sales purchase amount)

Total customers=DISTINCTCOUNT (Fashion-Retail-Sales [customer Reference ID])

Average Purchase Amount= Average (Fashion-Retail-Sales [purchase Amount] (USD))

Count of item purchased =COUNT (Fashion-Retail-Sales [item purchased])

Calculated Columns appending new column for weekdays

weekdays=Format (Fashion-Retail-Sales [Date Purchase],”dddd”

Potential Analysis

Top selling product by purchase amount

Best Payment method by Total Purchase Amount

Best 5 items purchased by review rating

Monthly sales trends

Total Purchase amount by weekdays

Average Purchased Amount by Item purchased

Total number of customers

Total Revenue (purchase amount)

Potential Insights

The Top selling products are Tunic, this helps the company to know the best performing product and this can help in stock inventory

Best Payment method by Total Purchase Amount, the best payment method will help the company finetune the preferable payment method their customers used most and how to improve

Best 4 items purchased by review rating, this help to know the average review rating overall, it helps finetune items that sell well but have low ratings, this could be as a result of quality.

The months with the highest purchased amount, will help us know the month with peak sales and how to boost sales in the low month sales

The bestselling days with total purchase will help us know the days of the week that has highest revenue and this will help to replicate what work well in those day to the low sales days

  
IN-ANALYSIS BOARD

  In-Analysis Observation

The Top selling products are Tunic, Jeans, Pajamas, Shorts and Handbag with purchase amount of 17.3k,13.1k, 12.8k, 12.7k, and 12.7k respectively.

Best Payment method by Total Purchase Amount, the best payment method with the highest percentage purchase amount is credit card 53.5%

Best 4 items purchased by review rating, the best item with the highest review rating are skirt (258.9), Belt (252.1), Shorts (235.6), Tank Top (235,6)

The months with the highest purchased amount are May, November, and December with a total sale of 48K, 47K, 46K respectively

The bestselling days with total purchase amount is Monday 88k, followed by Friday 66k and Tuesday 66k 

                                         


IN-ANALYSIS INSIGHTS

•	The Top selling product is Tunic, and most frequently purchased product, Tunic also appear with high average purchase amount. 
•	Best Payment method by total purchase amount is credit card (53.5%), this means majority of the company customers prefer credit card but cash is still significant (46.5%)
•	The best items with high review ratings, is skirts and Belts though they are not in the top 5 selling products, this means the customers like these products but they are not selling as Tunic and jeans, this may be as a result of high price or customers are not aware of the high-quality product due to limited marketing or ads, or the product might be widely available both online or store.

•	The best days with the highest sales are Monday, this might be possible because of the new stock or marketing/ads campaign in the week.

•	The months with the highest purchased amount are May, November and December, this might be as a result of mid-year sales and holiday/end of the year shopping, those methods put in place to achieve that can be replicated in the other low sales month

FINAL OBSERVATION AND RECOMMENDATION

Final Observations

•	The Top selling products are Tunic, Jeans, Pajamas, Shorts and Handbag with purchase amount,
for Top product Tunic, the total revenue is 17.3k, total number of customers is 51, bestselling days is Monday 5.8k, followed by Friday 5.0k, average purchase amount by item purchased for Tunic is 320, the review rating is 139.6, the best payment method is credit card-81.4%. card-18.6%, the month with the highest sales is Dec 9.4k and Nov 2.6k.
for product Jeans, the second top product, the total revenue is 13.1k, total number of customers is 46, best payment method is cash 58.6%, followed by credit card 41.4%. average purchase amount by item purchase for Jean is 272, the review rating is 169.7, bestselling days is Friday 5.4k, Thursday 3.9k. The month with the highest sales is May 5.7k, Nov 3.1k

for the Third Top product, Pajamas, the total revenue is 12.8k, total number of customers 67, best payment method is credit card 82.2%, Cash 17.8%, pajamas have review rating of 205.9, the average purchase amount by item purchase for pajamas is 210, bestselling days is Monday 4.7k Friday 2.9k, the month with the highest sales September 4.3k and May 2.9k.

For the product, Short, the total revenue is 12.7k, total number of customers is 63, best payment method is Cash 70.8%, followed by credit card 29.2%, bestselling days is Friday 6.3k, the review rating for shorts is 372, best monthly sales are Aug 5.8k

For product Handbag, the total revenue is 12.7k, best payment method, credit card 76.5%, Cash 23.5%, the review rating for handbag is 199.7, monthly sales are May 4.9k, Average purchase amount for handbag is 215, bestselling days is Tuesday 5.6k

•	Best Payment method by Total Purchase Amount, the best payment method with the highest percentage purchase amount is credit card 53.5%
for Best Payment method, Credit card-total revenue 231k, top product is Tunic, total number of customers is 166, bestselling days is Monday,48k, followed by Tuesday 39k, the Top average purchase amount by item purchased is Tunic 562, slippers 355, Boots 350, best month with highest sales December 31k, followed closely by Nov 30k, then May 21k.Top selling products Tunic 14.1k, Pajamas 10.5k, handbag 9.7k, product with high review rating skirt 164.1, Belt 150,5, T-shirt 125.4, Cardigan 122.4. for cash payment, total revenue is 200k, total number of customers 166, bestselling days is Monday 39k followed by Friday 35k, The Top average purchase amount by item purchased is Bowtie 325, Jean 294, Trousers 286, Best Monthly sales with highest revenue May 27k, Top selling products is shorts 9.0k, sweeter 8.2k, Jean 7.7k, Product with high review rating is Tank top 139.1, Shorts 130.5, pants 123.4

•	Best 4 items purchased by review rating, the best item with the highest review rating are skirt (258.9), Belt (252.1), Shorts (235.6), Tank Top (235,6)

•	The months with the highest purchased amount are May, November, and December with a total sale of 48K, 47K, 46K respectively

•	The bestselling days with total purchase amount is Monday 88k, followed by Friday 66k and Tuesday 66k 


RECOMMENDATIONS

•	Promote product with High Review-Rating, yet they are Underperforming, I Recommend the company should focus marketing on skirts and Belts (high rating and not in top sales, this will help to improve their visibility and sales

•	I Recommend that the company should boost sales on low traffic days, this can be achieved by running promotional offers on low purchase days (Wednesday and Saturday) to balance weekly revenue.

•	I Recommend that the company should prepare for seasonal peaks, Month of May, November and December are the peak sales months, ensure to stock more of the products. also check what they did well in the month of May, Nov and Dec such as slash sales, discount offer. more ads and they should replicate that in the other low month sales.

•	For the Best payment method, I recommend in-store- only discounts, rewards for using cash payment should be considered for card users, since cash payment still account for large portion (46.5%)

•	I recommend that the company should consider loyalty programs or personalized offers for the customer which could increase customer lifetime value thereby increasing the company revenue. 

•	For the Top performing product, the company should inform the inventory department to ensure that the product is not out of stock to prevent losing customers or discourage them.

Conclusions
This report provided an analytical overview of key factors influencing fashion sales, based on customer transactions, product performance, and purchasing behavior. By examining variables such as purchase amount, item category, review ratings, and day-of-week trends, we gained meaningful insights into consumer preferences and sales dynamics. The analysis highlights opportunities to optimize marketing strategies, enhance customer satisfaction, and improve inventory planning. These findings can support data-driven decision-making and contribute to overall business growth in a competitive retail environment.








