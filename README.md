
# E-Commerce: Olist Store Analysis

## Project Objective

The Olist Store Analysis project aims to analyze customer purchasing patterns and payment statistics on an E-commerce platform, Olist. This project covers several key performance indicators (KPIs) such as weekday vs weekend sales, payment statistics, delivery time, and customer behavior. 

### Tools Used: The Analysis was done using Excel, Power BI, Tableau and SQL

#### Datasets Details

Project covers several key performance indicators (KPIs) such as weekday vs weekend sales, payment statistics, delivery time, and customer behavior. The analysis is based on nine CSV files, which are cleaned and manipulated to extract valuable insights.

### Description of Our source Data:

We chose the Brazilian-eCommerce olist store dataset from ExcelR Solutions for our analysis. This dataset contains approximately 100,000 customer orders, along with corresponding files on product information and English translations of product categories originally in Portuguese. Nine files from the original  dataset were chosen for further analysis: 

A] olist_geolocation_dataset

B] olist_customers_dataset

C] olist_sellers_dataset

D] olist_product_dataset

E] olist_order_items_dataset

F] olist_orders_dataset

G] olist_order_payments_dataset

H] olist_order_reviews_dataset

I] product_category_name_translation.

### Data Modelling
We used joins to create relationship between data tables in Power bi.The Entity Relationship Diagram(ERD) below shows the connectivity between the 9 data tables used in our analysis.

<img width="827" alt="image" src="https://github.com/user-attachments/assets/60c9a51e-2ee2-4235-9334-6cbf77aae85b" />

The description of these tables is as follows:

olist_orders_dataset: This table is connected to 4 other tables. It is used to connect all the details related to an order.

olist_order_items_dataset: It contains the details of an item that had been purchased such as freight value, price and so on.

olist_order_reviews_dataset: It contains details related to any reviews posted by the customer on a particular product that he had purchased.

olist_products_dataset: It contains related to a product such as the Product ID, Product category name and measurements.

olist_order_payments_dataset: The information contained in this table is related to the payment details associated with a particular order type.

olist_customers_dataset: Details the customer base information of this firm.

olist_geolocation_dataset: It contains geographical information related to both the sellers and customers.

olist_sellers_dataset: This table contains the information related to all the sellers who have registered with this firm.

olist_product_category_name_translation: This table is connected to products database.


##### Data Cleaning 

- Standardized City Names: Different spellings of “Sao Paulo”(example ” São Paulo”) were standardized to “Sao Paulo" using find and replace in Power Query.

- Corrected Sellers Location Data: In sellers table city names were mistakenly entered as zip codes(example replaced “04482258” with “Rio De Janeiro”).

- Handled Missing Values in Products Table: Replaced null to “0” & Blank values to Unidentified(for product category name).

- Filled Missing Values in Reviews Data: In Reviews Table, missing values in review messages and titles were replace with “No Message” and “No Title” respectively.

- Fixed Headers in Product Category Name Translation Table: Applied the “Use First Row as Headers” option to correctly structure the columns names.

- Removed Duplicates & Cleaned Data: Identified and removed duplicate records to ensure data consistency.

#### Data Visualizations
**KPI 1: WEEKDAY VS WEEKEND (ORDER_PURCHASE_TIMESTAMP) PAYMENT STATISTICS**

A conditional Column weekend/weekday was created to analyse order trends and payment trends over weekdays and weekends.
Count of orders placed and Average payment value is more on weekdays (~77%, $154.44) as compared to weekends(~23%, $152.95)

The least number of orders placed are observed on Saturday (10,887), whereas highest is observed on Monday (16196). 
![image](https://github.com/user-attachments/assets/07e013b5-f224-4657-881f-26d37347222f)
![image](https://github.com/user-attachments/assets/1242155b-c7db-4561-a25c-28b080be71cd)

**KPI 2: TOTAL NUMBER OF ORDERS WITH REVIEW SCORE 5 AND PAYMENT TYPE AS CREDIT CARD**
Approximately 77% of the customers prefer credit card as a payment method and 58% of the reviews are rated 5 for this payment type.

The highest Orders with review score 5 using credit card is  43981 & The average review score is 4.09
![image](https://github.com/user-attachments/assets/4feda3fb-ffb4-48fc-9b6f-5f4ce826857d)

**KPI 3: Average number of days taken for order_ delivered _customer _ date for pet_ shop**
For product category pet shop it is observed that it takes average of  11 delivery days approximately. 

![image](https://github.com/user-attachments/assets/2a0e713d-fb1b-4a56-915e-f6000a804bd0)

**KPI 4: Average price and payment values from customers of Sao Paulo city**
Approximate values for both Avg payment value  and Avg price as 136 and 108.
![image](https://github.com/user-attachments/assets/f24f13ed-d030-4cdb-8e68-5200e55c211f)

**KPI 5: Relationship between shipping days Vs review scores**
Its observered that as average delivery days decrease, the review scores increase.
![image](https://github.com/user-attachments/assets/12696199-3dd5-4dc6-bbae-4287f7e2b29b)

### Dashboard Link : https://public.tableau.com/app/profile/lagudu.hemalatha/viz/OlistStoreAnalysis_17411684876880/Dashboard?publish=yes


