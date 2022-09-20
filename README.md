# e-commerce
Analytic project for online store including **analysis of statistical values within a time series**, **сohort analysis of users**, and **RFM user segmentation**. 

## Annotation
Analysis of completed purchases and answer the following questions from prodact-manager:
   1. How many users do we have who made a purchase only once?;
   2. How many orders per month, on average, are not delivered for various reasons (display details by reasons)?;
   3. For each product, determine on which day of the week the product is most often bought?;
   4. How many purchases does each user make on average per week (by months)?;
   5. Cohort analysis of users. Between January and December, identify the cohort with the highest retention for the 3rd month;
   6. Build RFM user segmentation to qualitatively evaluate your audience.For each RFM segment, plot the boundaries of the recency, frequency, and monetary metrics to interpret these clusters.;

## Files with data
**[olist_customers_datase.csv](https://disk.yandex.ru/d/FUi5uSd6BfG_ig)** - table with unique user ids.

 - **customer_unique_id** - unique userID
 - **customer_zip_code_prefix** - user's zip code
 - **customer_city** — user delivery city
 - **customer_state** - user's delivery state

**[olist_orders_dataset.csv](https://disk.yandex.ru/d/t9Li4JOfgxuUrg)** - table of orders.

 - **order_id** - unique order identifier
 - **customer_id** - custom userID
 - **order_status** — order status
 - **order_purchase_timestamp** - order creation time
 - **order_approved_at** - order payment confirmation time
 - **order_delivered_carrier_date** - time of transferring the order to   the logistics service
 - **order_delivered_customer_date** — order delivery times
 - **order_estimated_delivery_date** - estimated delivery date

**[olist_order_items_dataset.csv](https://disk.yandex.ru/d/Gbt-yAcQrOe3Pw)** - table of commodity items included in orders

 - **order_id** - unique order identifier
 - **order_item_id** - item identifier within one order
 - **product_id** — productID
 - **seller_id** - ID of the product manufacturer
 - **shipping_limit_date** - maximum date of delivery by the seller to transfer the order to the logistics partner
 - **price** - price per item
 - **freight_value** — goods weight
