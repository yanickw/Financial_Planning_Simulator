# Financial Planning Simulator
*FINANCIAL PLANNING SIMULATOR* is a financial planning application utilizing the power of API's to analyse different probability over time using a diversity of available portfolio which are run through a Monte Carlo Simulation model for forcast.

## Requirements

This application was writen in Jupyter Lab 3.3.2 using Python 3.9.7

**Operating System:**

-   Window 10 (or higher) using Gitbash.
-   MacOS 10.14 (or higher) using a terminal.
-   Linux Ubuntu 22.04 (or higher) using a terminal.

**Will need to be installed:**

_jupyter lab_  3.3.2

```
$ pip install jupyterlab
```

_pandas_  1.4.2
```
$ pip install pandas
```

_pathlib_  1.0.1

```
$ pip install pathlib
```

_dotenv_ 

```
$ pip install python-dotenv
```
_alpaca-trade-api_ 

```
$ pip3 install alpaca-trade-api
```
_MCForecastTools_ 

```
$ pip install mc-simulation
```
----------

## Installation

To install the application you will need to clone the GitHub repository.

```
$ git clone https://github.com/yanickw/Financial_Planning_Simulator

```

----------

## Get Started

Using the  _Financial Planning Simulator_:

Open a gitbash, navigate to your github cloned repositery. Start  _Jupyter Lab_

```
$ jupyter lab
```

### 1. Setup the Portfolio.

Once the Jupyter Lab application running, you will need to input relative information of the portfolio like amount of coins for each cryptocurrency in wallet and monthly income.

```
# Import the data by reading in the CSV file and setting the DatetimeIndex.
<crypto ticker>_coins = <amount> #value
monthly_income = <value> #float
```

### 2. Update Prices of Cryptocurrencies and Portfolio Using API's.

Series process to clean both dataframe for analysis.

1.  Set you desire API url to get price on cryptocurrency.
2.  Using  `request.get(<url of crypto API>)`  get the json file containing various information about the selected cryptocurrency.
3.  Parse the json file to get the price of thes elected cryptocurrency .
4.  Calculate the Financial value of the Portfolio.

### 3. Update Prices of Stocks and Bonds of Portfolio Using Alpaca SDK.

1.  Review the total number of shares held.
2.  Set the variables for the Alpaca API and secret keys and API Call.
3.  Get the current closing prices for the stocks and bonds by using the Alpaca  `get_bars`  function and store them as variables..
4.  Calculate the value, in US dollars, of the current amount of shares in each of the stock and bond portions of the portfolio.

### 4. Evaluate the Emergency Fund
In this section, you’ll use the valuations for the cryptocurrency wallet and for the stock and bond portions of the portfolio to determine if the credit union member has enough savings to build an emergency fund into their financial plan.

### 5. Create a Financial Planner for Retirement
1. Create the Monte Carlo Simulation useing the MCForecastTools library for the Portfolio.
2. Analyze the Retirement Portfolio Forecasts using the current value of only the stock and bond portion of the portfolio and the summary statistics generated from the Monte Carlo simulation
----------

## Contributors

This application originated from a Berkeley Bootcamp.

For any inquieries, feedbacks or comments about this project please email me at  [yanickw@gmail.com](mailto:yanickw@gmail.com)

I can also be reached on  [LinkedIn](https://www.linkedin.com/in/yanickwilisky/)  or  [Twitter](https://twitter.com/yanickwilisky).

----------

## License

MIT License

Copyright (c) 2022 Yanick Wilisky

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

