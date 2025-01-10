# E-commerce Sales Detective: Uncovering Trends & Customer Insights

## Project Overview

This project analyzes an e-commerce sales dataset to uncover trends, customer behaviors, and actionable insights. By leveraging data analysis techniques, the project aims to optimize business strategies and improve decision-making.

## Dataset Description

- Dataset Name: TDI Online Sales Dataset
- File: TDI_online_sales_dataset2.csv
- Size: 49,782 rows and 18 columns
- Attributes:
  - InvoiceNo: Unique identifier for transactions
  - Stock Code: Product SKU
  - Description: Product name
  - Quantity: Number of units sold
  - Invoice Date: Date of purchase
  - Invoice Time: Time of purchase
  - Unit Price: Price per unit
  - Customer ID: Unique customer identifier
  - Country: Customer's country
  - Discount: Discount applied to the transaction
  - Payment Method: Payment type (e.g., PayPal, Bank Transfer)
  - Shipping Cost: Cost of shipping
  - Category: Product category
  - Sales Channel: Mode of sale (e.g., Online, In-store)
  - Return Status: Whether the item was returned
  - Shipment Provider: Courier used for delivery
  - Warehouse Location: Origin warehouse
  - Order Priority: Priority level of the order (High, Medium, Low)

## Objectives
- Analyze customer behaviors across countries, shipment provider and categories.
- Highlight the impact of discounts and shipping costs on sales.
- Detect anomalies or patterns in return rates.
- Highlight the total quantity sold by category,description

##  Data Cleaning and Preparation
### Issues Identified:

- Missing values in Customer ID, Shipping Cost, and Warehouse Location.
- Negative values in Quantity and Unit Price indicating returns or errors.
- Some product descriptions were found under wrong category.

### Actions Taken:

- Missing values in Customer ID, Shipping Cost were replaced with 0 while missing values in Warehouse Location were replaced with unknown.
- Corrected anomalies in Quantity and Unit Price by segregating returns.
- Product description were mapped to their corresponding categories and column were created for corredcted category

## Exploratory Data Analysis (EDA)
### Key Findings:


- Customer Behavior:
  - Top countries by total sales: United Kingdom, Belgium, Germany
 
![image](https://github.com/user-attachments/assets/7a4cc32a-6ff3-4afa-84d1-e56f1810f32b)

![image](https://github.com/user-attachments/assets/b400ca69-9744-46c2-83ae-c755bf1ccdb1)

- Customers prefer online sale channel.

  ![image](https://github.com/user-attachments/assets/cdf15703-8511-40b7-bd73-5219450e55ce)


             
- Product Performance:
 - Accessories has the highest quantity sold

   ![image](https://github.com/user-attachments/assets/7193234b-6477-44c8-b538-03502c2ac4e5)

 - Furniture dominate total sales in category.

   ![image](https://github.com/user-attachments/assets/60dc5cf0-41bf-482f-bb48-bf233c29fb0e)


- Impact of Discounts and Shipping Costs:
 - Moderate discounts (10-20%) correlate with higher sales volumes.
 - Free shipping boosts purchases, particularly for low-cost items.

![image](https://github.com/user-attachments/assets/08efa490-7ec8-4e47-8c37-195a4224388e)

![image](https://github.com/user-attachments/assets/4f463a45-6a56-489c-8944-6a5c9855d34e)

![image](https://github.com/user-attachments/assets/d10d87b3-06f6-416b-bc13-8f77212444ce)





## Methodology
- Libraries Used: pandas, numpy, matplotlib, seaborn.

### Visualization Techniques:

- Heatmaps to understand regional sales.
- Bar plots for product category performance, total sales by shipping method, country sales performance, total sales by shipping method.
- Bar plots also to detect number of quantity sold by product description, category.
- Scatter plots to see impact of shipping cost and discount on total sales 

### Statistical Analysis: Correlation analysis to link discounts, shipping cost and sales.

### Results and Insights

- Top-Performing Products:USB Cables and Backpack.

  ![image](https://github.com/user-attachments/assets/1290037c-8cd9-4a8c-973b-1fdba2d4b11a)

- Customer Insights: Customers prefer online shopping with Bank transfer as the most popular payment method.

  ![image](https://github.com/user-attachments/assets/edd02f7b-5bf6-4e4a-b364-280c6c9f6187)

- Returns: High return rate linked to specific categories, suggesting quality issues or misalignment with customer expectations.

  ![image](https://github.com/user-attachments/assets/36d44d75-0d26-42f1-928a-93ec96635ffe)


## Challenges and Solutions

### Data Quality: 
- Missing values addressed through imputation.
- Anomalies in Data: Negative quantities identified as returns were analyzed separately.

### Recommendations
  1. Target International Markets:

- Focus on maintaining and expanding your reach in the United Kingdom, Belgium, and Germany, as these countries are leading in sales.
Promote Accessories and Furniture:
- Given the high quantity sold for accessories and the dominance of furniture in total sales, consider targeted marketing campaigns for these categories to maximize more revenue.
- Product Focus on USB Cables and Backpacks:
- Increase inventory or offer bundled promotions for USB Cables and Backpacks to capitalize on their popularity.
  
 2. Enhance Customer Experience:
- Since online shopping is favored, improve the user interface and offer better navigation and product filtering for an optimized experience.
- Ensure that payment options (especially bank transfer) are seamless to reduce friction during checkout.

3. Address Return Issues:
- Investigate the quality and customer expectations for categories with high return rates and adjust product descriptions or quality control measures to reduce returns.
- Leverage Discounts and Free Shipping:
- Experiment with discounts within the 10-20% range to drive higher sales volumes and continue offering free shipping, particularly on low-cost items, to encourage more purchases.

4. Underperforming Product Categories:
- Identify Key Issues: Start by analyzing why certain categories are underperforming. It could be due to factors such as poor product quality, misalignment with customer expectations, or ineffective marketing strategies.
  
- Improve Product Offerings:
 - For categories with low sales, consider introducing new products or revamping existing ones to cater to customer preferences.
 - Product diversification can also help. For example, if a category is stagnant, test introducing complementary items or variations that might appeal to a broader audience.
  
- Targeted Promotions: Use targeted promotions or discounts to boost sales in underperforming categories. Offering limited-time deals can generate a sense of urgency and attract customers to those specific products.

- Customer Feedback and Research: Gather customer feedback on the underperforming categories. Use surveys, reviews, or focus groups to better understand their pain points and expectations.
  
- Increase Visibility: Improve the visibility of these categories through optimized search and filtering options on your online platform or through focused advertising that targets potential customers more effectively.

5. Countries with Low Sales:
- Market Research: Conduct thorough market research to understand why sales are low in specific countries. Key factors might include:
 - Cultural preferences: Certain products may not resonate with local tastes.
 - Price sensitivity: Customers in some countries may be more price-sensitive, so adjusting pricing or introducing more affordable options could help.
 - Payment and shipping: Ensure that the payment methods and shipping options are convenient for customers in low-performing countries. Consider adding more localized payment methods or offering discounted international shipping.
- Localized Marketing Strategies: Tailor your marketing campaigns to appeal to local audiences. Highlight products that align with cultural preferences and engage with local influencers to boost brand visibility.

- Discounts and Incentives: Offer country-specific discounts or promotions to increase sales volume. You might also consider offering free shipping to encourage customers from low-sales regions to make purchases.

- Local Partnerships: Collaborate with local e-commerce platforms or retailers to help boost brand presence and credibility in underperforming regions


## Reflection

This project enhanced my ability to analyze complex datasets, identify patterns, and provide actionable business insights. It demonstrated the importance of data cleaning and visualization in storytelling and decision-making.
 


