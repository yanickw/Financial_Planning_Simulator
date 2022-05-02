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

### 3. Analyze the Data

After getting the summary statistic and visualize the data we then aim our focus on the analysis of specific dates to run an arbitrage profits simulation.

### 4. Calculate the Arbitrage Profits

First order of business is to mesure the arbitrage spread. Followed by the spread returns which leads us to find the positive returns exceeding 1% minimum threshold that we need to cover our costs. The following steps calculates the potential arbitrage profits on each days. Finally, we total the cumulative sum using the  `.cumsum`  and visual graph of the results.

----------

## [](https://github.com/yanickw/crypto_arbitrage#contributors)Contributors

This application originated from a Berkeley Bootcamp.

For any inquieries, feedbacks or comments about this project please email me at  [yanickw@gmail.com](mailto:yanickw@gmail.com)

I can also be reached on  [LinkedIn](https://www.linkedin.com/in/yanickwilisky/)  or  [Twitter](https://twitter.com/yanickwilisky).

----------

## [](https://github.com/yanickw/crypto_arbitrage#license)License

MIT License

Copyright (c) 2022 Yanick Wilisky

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
