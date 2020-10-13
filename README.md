# World wide Products Inc.
# Data science project_5

The dataset contains historical product demand for a manufacturing company with footprints globally. The company provides thousands of products within dozens of product categories. There are four central warehouses to ship products within the region it is  responsible for.

This dataset contains 1 CSV file.

Product_demand.csv - CSV data file containing product demand for encoded product id's

I have used two models, FbProphet and ARIMA to determine the demand for a product and forecast its demand for next one year using the other columns as features.
## Data source :
https://www.kaggle.com/felixzhao/productdemandforecasting

### Output of this project:
This project processes the data which contains products,its warehouses,catergories,its demand and with the help of all these features it forecasts a product demand for next one year. Selection of product is done by plotting a plt from given dataset.

### Data cleaning and feature engineering:
1.There are null values in "Date" column. I have dropped those goru since they don't add any value.
2.From "Order_demand" column I've remove special characters and changed the data type to float.
3.Replaced the duplicated rows with their mean
4.Changed data type for Date column
5.Extracted "date","month","year" from Date column

### Data exploration:
1.Plotted a plt to see which category has highest order demand.
2.Plotted another graph to see which ware house produces most unique products and found out that "J" produces most unique produts.
3.Plotted a garph to see "order_demand" from years 2011 to 2017.
4.Checked which products are being produced in how many warehouses.

### Product with high demand:
1.Tried figuring out by using plt which product has highest demand and i've observed that "prod_1245" has highest demand.

### Observations:
1. The demand for product_1245 has been increasing from 2012 with a high increase from 2014
2.If we see weekly trend,the demand is great on Thursday and it goes negative on sundays 
3. If we see yearly,the demand is high during mid of March and less during September
4.If we see daily the demand is more during early hours 4:00 am and in the night 8:00 pm
