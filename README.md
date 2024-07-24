# [PowerBI] Customer Behavior Analysis

## I. Introduction
### 1. Business context
Sales representatives from regional sales offices have assigned sales territories in the United States, Canada, England, Australia, Germany, and France. Each regional office consists of several sales representatives and a team manager. In their daily sales activities, sales representatives use both laptops and Handheld PCs that run Microsoft® Windows CE. A typical work day for a sales representative starts with the representative dialing in to the regional office and downloading current data such as inventory, product, and promotional information. During customer visits, the sales representative takes orders on the laptop or Handheld PC. At the end of each day, the sales representative sets up appointments for the following day or week, checks the appointments of other representatives in the area for possible collaboration, and updates the contact list. The sales representative dials back into the regional office, sends updated information, and receives any new internal communications from the base office or regional office. The company currently uses Microsoft Outlook® for email.

### 2. Business questions
The sales teams have identified the following requirements that will enable them to perform their jobs better:

Customer segmentation and profiling:
- Analyze customers based on their purchase behaviours: RFM (recency, frequency, and monetary value of a transaction)
- Who are the best customer across all product lines? With whom should the sales team focus its efforts for building long-term relationships?
- What products are popular and at what rate among customer group?
### 3. Dataset
Dataset: **adventureworks2019** (public Google BigQuery dataset)

Dataset dictionary: Please reach file "Data Dictionary" attached above

Dataset Schema: https://i0.wp.com/improveandrepeat.com/wp-content/uploads/2018/12/AdvWorksOLTPSchemaVisio.png?ssl=1

Dataset access: 
- Log in to your Google Cloud Platform account and create a new project.
- Navigate to the BigQuery console and select your newly created project.
- In the navigation panel, select "Add Data" and then "Star a project by name".
- Enter the project name "adventurework2019"

## II. Apply design thinking mindset
**1. Empathize**

![image](https://github.com/user-attachments/assets/5082ae49-5a4e-441d-b14b-dc4cdf5fac02)

**2. Define point of view**

![image](https://github.com/user-attachments/assets/99c0c294-2ed5-40c0-8582-fe6cccd6aa0a)


**3. Ideate**

![image](https://github.com/user-attachments/assets/1a70413c-e5f2-4650-999f-7f9948db13da)

**4&5. Prototype and review**

![image](https://github.com/user-attachments/assets/3e6ce36e-55e4-4e89-8fc4-2a3b74bc7a41)


## III. Main Process
### 1. Connect data to PBI and modelling

- Connect queries above and available tables of dataset to PBI
- Modelling

![image](https://github.com/user-attachments/assets/06605c8a-d9e3-43e3-b44e-f6c7e442bba0)

### 3. Build dashboard

- Using DAX to create measures and calculated columns
- Build 2 report pages

**Customer Purchase Behavior**

![image](https://github.com/user-attachments/assets/57ed7ff5-29d7-48e9-a4b0-121387842c18)

**Product**

![image](https://github.com/user-attachments/assets/22c01183-3c7d-4941-9f35-65e45f77a193)

## IV. Insights and Recommendations
- From 2011-2014, the New Customer customer group had the largest number of customers, accounting for 24% of the total customers: These are customers who have recently purchased, have low cart value and do not buy frequently.
- Champion customer group is a group of customers who have recently transacted (1 day), purchased frequently (total 973 times), and spent the most (total $75M) from 2011 - 2014
- On the contrary, the Lost Customer group is the group with the longest time without a transaction (290 days), purchasing frequency (total 80 times) and shopping cart value is also very low (total $60K).

→ For the New Customer group, businesses should offer more promotional offers to this group of customers to stimulate them to buy more often. When they get used to regularly buying from the business -> Customers have more trust in the brand -> in the future they may consider spending more money on higher value products.

→ For the Champion group, the company should especially build close relationships with customers in this group because this is the group that helps "feed" the company's growth.

→ For the lost customer group, businesses can consider eliminating resources, paying attention to this group of customers and only saving their information so that in case they can return in the future -> the business still has the information. to suggest suitable products for this group

- Among the 275K products sold, the Bikes product group brings in the most revenue (accounting for 86% of total revenue) (Easy to understand because the nature of bicycle products has a higher value/product compared to the other 3 industries). remaining onion).
- On the contrary, the Accessories product group brings the least revenue to the business (accounting for 1.16% of total revenue).
- However, the Accessories category (34%) and the Bikes category (33%) have similar rates in terms of customer purchases.

→ This shows that businesses should still promote sales in both of these industries instead of just focusing on the Bikes industry.

- Among all customer groups, Champion Group is the group that brings in the most revenue (57%) not only for the category with the highest revenue, which is Bikes, but also for the other 3 industry groups. This corresponds to the total number of purchases as the Champion group also buys many Assessories and Bikes

→ Businesses should focus on sales in both high-value product groups such as Bikes and low-value product groups such as Assesories for the Champion customer group


