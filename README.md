# Retail-Sales-Prediction-Regression

Predicting retail sales can be a challenging task, as it involves forecasting consumer behavior and market trends. However, it is an important task for businesses, as accurate sales predictions can help them make informed decisions about inventory management, marketing strategies, and financial planning.

There are several approaches that can be taken to predict retail sales. One common approach is to use statistical models and machine learning techniques to analyze past sales data and identify patterns that may be used to forecast future sales. This may involve using techniques such as regression analysis.

Another approach is to gather data from external sources, such as economic indicators, demographic data, and consumer sentiment data, and use this information to inform the sales prediction model. This can help to incorporate external factors that may impact sales and improve the accuracy of the forecast.

Regardless of the approach taken, it is important to validate the accuracy of the sales prediction model through testing and to continuously update and refine the model as new data becomes available. This can help to ensure that the model remains relevant and accurate over time.

The interest for a product continues to change occasionally. No business can work on its monetary growth without assessing client interest and future demand of items precisely. Sales forecasting refers to the process of estimating demand for or sales of a particular product over a specific period of time. For a good sales forecast, it is extremely important to get a good dataset as well. Forecasts heavily depend on the past records, trends and patterns observed for sales of a particular store. The variations could be due to a number of reasons. Talking from a business’s point of view, these sales forecasts are done consistently to improve their sales forecasting models as they directly impact their decision making process, goals, plans and growth strategies. In this Retail Sales Prediction, machine learning models are created that predict sales of these 1115 drug stores across the European market and compare the results of these models. In addition to this, an effort has been made to analyze and find all the features that are contributing to higher sales and the features which are leading to lower sales, so that improvement plans can be worked upon.

We have been provided with 2 data sets.

1) Rosemann store Data: Information about sales and related factors

Store: Unique Store Id.

DayOfWeek: No. of day of the week.

Date: current Date of the day.

Sales: no. of sales of the day.

Customers: footfall of the day.

Open: store is open or closed.

Promo: Store running promotion or not.

StateHoliday: state holiday or not.

SchoolHoliday: school holiday or not.

2) Store: Information about the store

Store: Unique Store Id.

StoreType: 4 different type of stores a,b,c,d.

Assortment: A collection of goods or services that a business provides to a consumer.

CompetitionDistance: distance in meters to the nearest competitor store.

CompetitionOpenSinceMonth: Month in which the competition store was open.

CompetitionOpenSinceYear: Year in which the competition store was open.

Promo2: Store running consecutive promotion or not.

Promo2SinceWeek: calendar week when the store started participating in Promo2.

Promo2SinceYear: year when the store started participating in Promo2.

PromoInterval:The month in which the promotion starts eg: Jan,Apr,Jul,Oct.

# Conclusion from Model Training
We saw that Sales column contains 172817 rows with 0 sale. So we created a new dataframe in which we removed 0 sales rows and tried to train our model. We used various algorithms and got accuracy score around 74%.

We werealso curious about the total dataset(including Sales = 0 rows). So we trained another model using various algorithms and we got accuracy near about 92% which is far better than previous model.

So we came to conclusion that removing sales=0 rows actually removes lot of information from dataset as it has 172817 rows which is quite large and therefore we decided not to remove those values.We got our best rmpse score from Random Forest model,we tried taking an optimum parameter so that our model doesnt overfit.

# CONCLUSION FROM EDA
1)From plot sales and competition Open Since Month shows sales go increasing from November and highest in month December.

2)From plot Sales and day of week, Sales highest on Monday and start declining from Tuesday to Saturday and on Sunday Sales almost near to Zero.

3)Plot between Promotion and Sales shows that promotion helps in increasing Sales.

4)Type of Store plays an important role in opening pattern of stores.

5)All Type ‘b’ stores never closed except for refurbishment or other reason.

6)All Type ‘b’ stores have comparatively higher sales and it mostly constant with peaks appears on weekends.

7)ssortment Level ‘b’ is only offered at Store Type ‘b’.

8)We can observe that most of the stores remain closed during State Holidays. But it is interesting to note that the number of stores opened during School Holidays were more than that were opened during State Holidays.
