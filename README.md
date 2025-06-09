
# Data-Cleaning-with-Power-BI

### Project Overview
The project aims to clean and transform Cafe Sales data using Power Bi and Power Query Editor, ensuring accucurate analysis and informed business decisions. Key tasks include data inspection, cleaning, transformation, and modeling to provide reliable insighjts on sales trends and revenue.


### Data Source
Dirty Cafe Sales: The primary dataset used for this analysis is the [Uploading dirty_cafe_sales.csv…]()  

### Tools
- Power Bi - Data cleaning, Data Analysis, Visualization/Report

### Data Cleaning/Preparation
Data Cleaning tasks include:
- Data loading and inspection:
 10,000 rows dataset was availalble in the dirty cafe sales data. After checking for the validity of the data by ensuring the datatypes are corrrect. We observe that some columns contains errors, by removing this errors the rows reduced to 9031.
- Handling missing data
  For the Location Column: Replace Blank- instore, Error - Takeaway and Unknown - Instore
  For Payment Column: Replace Blank - Cash, Error - Digital Wallet, Unknown - Credit Card
- Data Formatting:
Split the original table based on price per unit, we observe that the items have a fixed price per unit.

  Cookie- 1.0, Tea- 1.5,  Coffee - 2.0, Cake and Juice - 3.0, Smoothie and Sandwich-4.0 and Salad-5.0.

  For each new table for Cookie, Tea, Coffee and Salad the Error, Empty and Unknown values of the price per unit was replaced by their respective price per unit. 

  For Cake and Juice having the same price per unit, Error value for Cake while Empty and Unknown for Juice. 

  For Smoothie and Sandwich having the same price per unit, Empty and Unknown for Smoothies while Error for Sandwich. 

  For Null Price per unit: Replace the null price by using conditional formatting to get the price the price from the Replace Error, Empty and Unknown with 1.0 which is equivalent to Cookie.

 For Quantity and Total spent, Null values were replaced with Zero

Merge the tables together to give a clean cafe data. 
Remove 145 rows of data due to Null date values. 
**8886** rows of data was used for the final analysis. 
Approximately 89% of yhe data was used for the final visualization.