# Ecommerce Analysis - Olist Dataset

Welcome to this analysis of the **Brazilian Ecommerce Olist Dataset**! This dataset contains over **100,000 orders** made between **2016 and 2018** at multiple marketplaces in Brazil, providing valuable insights into various aspects of online shopping behavior.

The dataset features various details about each order, including:

- **Order status**: Processed, delivered, canceled, etc.
- **Price**: The value of each product purchased.
- **Freight**: Shipping and delivery-related data.
- **Product attributes**: Product category, name length, description, and more.
- **Reviews**: Ratings and feedback provided by customers.
- **Customer information**: Customer location, shipping address, etc.

## Project Goals

The primary objective of this analysis is to uncover key performance indicators (KPIs) and provide actionable insights on various aspects of the ecommerce platform. Specifically, I focused on the following:

1. **Top Sold Products**: Identifying the most popular products in terms of order volume.
2. **Worst Performing Products**: Analyzing products with the lowest review scores and categorizing them based on their performance.
3. **Delivery Time vs Review Score**: Examining the correlation between delivery time and customer satisfaction (review scores). Analyzing if faster deliveries correlate with higher satisfaction.

## Analysis and Key Insights

### 1. **Top Sold Products**:
   By aggregating the order data, we identified the most sold products across different categories. This information is important for understanding product demand, stock management, and sales strategies.

### 2. **Worst Products by Review Score**:
   We also categorized products based on their review scores to identify those that received the lowest ratings. These products could benefit from attention to improve customer satisfaction, whether by improving product quality, better descriptions, or addressing specific customer complaints.

### 3. **Delivery Time vs Review Score**:
   One of the primary KPIs we explored was the relationship between **delivery time** and **customer satisfaction** (review score). We computed the delivery time for each order and divided the data into **fast deliveries** (those delivered before the median delivery time) and **slow deliveries** (those delivered after the median). A statistical test (T-test) was used to determine if there was a significant difference in satisfaction between these two groups.

   The analysis revealed that faster delivery times generally correlated with **better review scores**, highlighting the importance of delivery efficiency in improving customer satisfaction.

## Dataset Details

The dataset includes the following files:
- `olist_orders_dataset.csv`: Contains order-level data, including order ID, purchase timestamps, delivery dates, etc.
- `olist_customers_dataset.csv`: Customer-related data such as customer ID and location.
- `olist_order_items_dataset.csv`: Detailed information on products included in each order.
- `olist_order_reviews_dataset.csv`: Customer reviews for the products purchased.
- `olist_products_dataset.csv`: Product attributes, including category, description, and dimensions.
- `olist_sellers_dataset.csv`: Seller information related to each product.
- `olist_order_payments_dataset.csv`: Payment-related information for each order.
- `olist_geolocation_dataset.csv`: Geolocation data linking Brazilian zip codes to latitudes and longitudes.

## Requirements

To run this analysis on your own machine, you'll need the following Python libraries:

- `pandas` - for data manipulation
- `matplotlib` - for data visualization
- `seaborn` - for additional visualizations
- `scipy` - for statistical tests (e.g., T-test)

 Open the `notebook` or run the Python scripts to explore the data and the analyses.

## Conclusion

This analysis provides information about the Brazilian ecommerce landscape, offering insights into top-selling products, product performance by customer reviews, and the impact of delivery times on customer satisfaction. The findings can be leveraged by sellers, logistics teams, and marketers to optimize operations and improve customer experiences.
