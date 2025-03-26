# No Code Forecasting

#### Current status: Complete

___

### Personal Progress
* What I learned: How to use Jupyter Notebooks generally and Hex's specific implementation. How to use statsmodel and Prophet for generating time series models.
* What I wish I had done differently: Developed functionaility for users to be able to import their own data rather than jsut relying on demo data.
* What I am most proud of: [Lines 135-170](https://github.com/brayden-s-haws/no_code_forecasting/blob/4f744d5cb7516b32a8f2cbc65660f2f69ab4d5b4/No-Code%20Time%20Series%20Forecasting.yaml#L135) of No-Code Time Series Forecasting.yaml, one of the key inputs to these models is determining the seasonal period of the data. While this is just a dumb set of if statements it avoids the user needing to understand the this concept or needing to inspect their data and make a choice.
* What I want to learn next: I completed Kaggle data science track where I learned all about SciKit Learn. However I did not feel proficient enough to use it here. I would like to better understand what is available there and use it to create more powerful and reliable forecasts.

## Description
This app allows users to generate a set of time series forecasts without any technical knowledge. They can select a sample dataset, the number of periods to forecast, and the types of forecasts to run. This is meant to be a proof of concept for building advanced analytical tools that can be configured and run with a no-code interface.

![CleanShot Safari-2023-12-19](https://github.com/brayden-s-haws/no_code_forecasting/assets/58832489/470a6921-c386-48aa-8394-125ac2ec5efe)


## How It Works
The app comes pre-loaded with a series of datasets. These datasets span domains (sales, search trends, churn, supply chain) and time intervals (daily, weekly, monthly, quarterly). The user is able to select the dataset they wish to work with and the number of intervals they would like to forecast. They then select the type of forecast(s) to run: linear, simple seasonal ([SARIMAX](https://towardsdatascience.com/time-series-forecasting-with-arima-sarima-and-sarimax-ee61099e78f6)), advanced seasonal ([Prophet](https://facebook.github.io/prophet/)). The app then does the work to determine the correct configuration for each forecast based on the selected dataset. It runs the forecast models and generates a chart with the outputs. The outputs can also be exported to csv or xlsx.

The app is hosted on [Hex](https://hex.tech) and your can test it for yourself at this [link](https://app.hex.tech/455658aa-ee04-480f-945a-3fd455933fa2/app/6356acb1-2d8d-4f12-96a9-376dac1bb85e/latest).

The code for this is available in two forms:
* A jupyter notebook file that you can run on the configuration of your choice
* A yaml file that is meant for importing into Hex


