## Forecasting CPI and Unemployment in various Walmart stores

#### Data collection
This project involves analyzing data collected from the Walmart Super Market Dataset to predict the Consumer Price Index (CPI) and Unemployment rate across various Walmart stores. The dataset spans from 2010 to 2013 and includes weekly sales data for different Walmart locations.
The primary goal of this analysis is to predict the CPI and Unemployment rate for different Walmart stores a week after 2013 using historical data. By leveraging this information, we aim to provide insights into economic indicators that impact Walmart's performance and potentially influence business decisions.
![WALMART-STOREFRONT-iStock-1205217071](https://github.com/Neelesh1305/Walmartdata-Forecasting-CPI-Unemployment/assets/113800036/d3096186-5afa-4098-828c-12464f5f8a6d)

The dataset comprises several key features:

Store: The unique identifier for each Walmart store.

Type: The type/category of the store.

Size: The physical size of the store.

Date: The specific week of the sales data.

IsHoliday: A boolean indicator showing whether the week included a special holiday.

Temperature: The average temperature in the region during that week.

Fuel_Price: The cost of fuel in the region during that week.

MarkDown1-5: Anonymized data representing various promotional markdowns by Walmart.

CPI: The Consumer Price Index, which reflects the average change in prices paid by consumers over time.

Unemployment: The unemployment rate in the region.

#### Data Cleaning/feature engineering

After checking outliers and null values, and checking the correlation MarkDown1-5 showed no significance, and have a lot of missing data in them, hence they are removed. The feature 'IsHoliday' also showed very less signifcance, hence dropped.
Based on the correlation and visulaizations the data looks very linear and hence regression models are used for forecasting.

#### Modeling/Results
Various regression models are used for forecasting the CPI and Unemployment across various Walmart stores. Models used include Linear Regression, XGB Regressor, KNNRegressor, Random forest regressor, fully connected neural network and Decision Tree Regressors. 
Random forest Regressor showed a training r2 score of 0.99 for both CPI and Unemployment. And testing r2 score of 0.69 for CPI and 0.99 for Unemployment.
<img width="656" alt="Screenshot 2024-05-31 at 3 56 43 PM" src="https://github.com/Neelesh1305/Walmartdata-Forecasting-CPI-Unemployment/assets/113800036/1c1bf1c5-eb26-4cba-8515-8d003c04469d">

#### References
1. Walmart - Super Market Dataset. (n.d.). Www.kaggle.com. https://www.kaggle.com/datasets/saurabhbadole/walmart-super-market-dataset
2. Walmart to Open 150+ Large-Format Stores Across the U.S. | SupplyChainBrain. (n.d.). Www.supplychainbrain.com. Retrieved May 31, 2024, from https://www.supplychainbrain.com/articles/38998-walmart-to-open-150-large-format-stores-across-the-us
