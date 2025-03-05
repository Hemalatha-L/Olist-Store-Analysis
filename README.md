
# E-Commerce: Olist Store Analysis

### Dashboard Link : https://public.tableau.com/app/profile/lagudu.hemalatha/viz/OlistStoreAnalysis_17411684876880/Dashboard?publish=yes

## Project Objective

The Olist Store Analysis project aims to analyze customer purchasing patterns and payment statistics on an E-commerce platform, Olist. This project covers several key performance indicators (KPIs) such as weekday vs weekend sales, payment statistics, delivery time, and customer behavior. 

###Tools Used: The Analysis was done using Excel, Power BI, Tableau and SQL

#### Datasets Details

Project covers several key performance indicators (KPIs) such as weekday vs weekend sales, payment statistics, delivery time, and customer behavior. The analysis is based on nine CSV files, which are cleaned and manipulated to extract valuable insights.

Description of Our source Data:

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

##### Data Cleaning 

- Standardized City Names: Different spellings of “Sao Paulo”(example ” São Paulo”) were standardized to “Sao Paulo" using find and replace in Power Query.

- Corrected Sellers Location Data: In sellers table city names were mistakenly entered as zip codes(example replaced “04482258” with “Rio De Janeiro”).

- Handled Missing Values in Products Table: Replaced null to “0” & Blank values to Unidentified(for product category name).

- Filled Missing Values in Reviews Data: In Reviews Table, missing values in review messages and titles were replace with “No Message” and “No Title” respectively.

- Fixed Headers in Product Category Name Translation Table: Applied the “Use First Row as Headers” option to correctly structure the columns names.

- Removed Duplicates & Cleaned Data: Identified and removed duplicate records to ensure data consistency.


   
 
