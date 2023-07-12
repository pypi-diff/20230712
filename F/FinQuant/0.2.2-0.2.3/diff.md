# Comparing `tmp/FinQuant-0.2.2.tar.gz` & `tmp/FinQuant-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/FinQuant-0.2.2.tar", last modified: Sun May  3 16:19:06 2020, max compression
+gzip compressed data, was "FinQuant-0.2.3.tar", last modified: Wed Jul 12 07:32:42 2023, max compression
```

## Comparing `FinQuant-0.2.2.tar` & `FinQuant-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,30 @@
-drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2020-05-03 16:19:06.000000 FinQuant-0.2.2/
-drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2020-05-03 16:19:06.000000 FinQuant-0.2.2/FinQuant.egg-info/
--rw-rw-r--   0 frank     (1000) frank     (1000)    16986 2020-05-03 16:19:05.000000 FinQuant-0.2.2/FinQuant.egg-info/PKG-INFO
--rw-rw-r--   0 frank     (1000) frank     (1000)      376 2020-05-03 16:19:05.000000 FinQuant-0.2.2/FinQuant.egg-info/SOURCES.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)        1 2020-05-03 16:19:05.000000 FinQuant-0.2.2/FinQuant.egg-info/dependency_links.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)       53 2020-05-03 16:19:05.000000 FinQuant-0.2.2/FinQuant.egg-info/requires.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)        9 2020-05-03 16:19:05.000000 FinQuant-0.2.2/FinQuant.egg-info/top_level.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)    16986 2020-05-03 16:19:06.000000 FinQuant-0.2.2/PKG-INFO
--rw-rw-r--   0 frank     (1000) frank     (1000)    13666 2020-05-03 16:06:42.000000 FinQuant-0.2.2/README.md
-drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2020-05-03 16:19:06.000000 FinQuant-0.2.2/finquant/
--rw-rw-r--   0 frank     (1000) frank     (1000)        0 2019-01-29 18:51:16.000000 FinQuant-0.2.2/finquant/__init__.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    16801 2019-08-11 10:44:27.000000 FinQuant-0.2.2/finquant/efficient_frontier.py
--rw-rw-r--   0 frank     (1000) frank     (1000)     2064 2019-01-29 18:51:16.000000 FinQuant-0.2.2/finquant/minimise_fun.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    11145 2020-05-03 16:03:46.000000 FinQuant-0.2.2/finquant/monte_carlo.py
--rw-rw-r--   0 frank     (1000) frank     (1000)     6685 2020-04-12 13:09:18.000000 FinQuant-0.2.2/finquant/moving_average.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    47487 2020-05-03 16:03:46.000000 FinQuant-0.2.2/finquant/portfolio.py
--rw-rw-r--   0 frank     (1000) frank     (1000)     3936 2020-04-12 13:09:18.000000 FinQuant-0.2.2/finquant/quants.py
--rw-rw-r--   0 frank     (1000) frank     (1000)     2142 2020-04-12 13:09:18.000000 FinQuant-0.2.2/finquant/returns.py
--rw-rw-r--   0 frank     (1000) frank     (1000)      106 2020-05-03 16:19:06.000000 FinQuant-0.2.2/setup.cfg
--rw-rw-r--   0 frank     (1000) frank     (1000)     1800 2020-04-12 13:09:18.000000 FinQuant-0.2.2/setup.py
+drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-12 07:32:43.098627 FinQuant-0.2.3/
+drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-12 07:32:42.939143 FinQuant-0.2.3/FinQuant.egg-info/
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    14845 2023-07-12 07:32:42.000000 FinQuant-0.2.3/FinQuant.egg-info/PKG-INFO
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      582 2023-07-12 07:32:42.000000 FinQuant-0.2.3/FinQuant.egg-info/SOURCES.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)        1 2023-07-12 07:32:42.000000 FinQuant-0.2.3/FinQuant.egg-info/dependency_links.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      193 2023-07-12 07:32:42.000000 FinQuant-0.2.3/FinQuant.egg-info/requires.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)        9 2023-07-12 07:32:42.000000 FinQuant-0.2.3/FinQuant.egg-info/top_level.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1059 2023-07-08 06:47:36.000000 FinQuant-0.2.3/LICENSE.txt
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    14845 2023-07-12 07:32:43.099125 FinQuant-0.2.3/PKG-INFO
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    13659 2023-07-11 12:42:27.000000 FinQuant-0.2.3/README.md
+drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-12 07:32:43.022645 FinQuant-0.2.3/finquant/
+-rwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-08 06:47:36.000000 FinQuant-0.2.3/finquant/__init__.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    16801 2023-07-10 17:36:45.000000 FinQuant-0.2.3/finquant/efficient_frontier.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1990 2023-07-10 13:30:17.000000 FinQuant-0.2.3/finquant/minimise_fun.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    11159 2023-07-08 06:47:36.000000 FinQuant-0.2.3/finquant/monte_carlo.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     6685 2023-07-08 06:47:36.000000 FinQuant-0.2.3/finquant/moving_average.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    43673 2023-07-08 08:26:58.000000 FinQuant-0.2.3/finquant/portfolio.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     3936 2023-07-08 06:47:36.000000 FinQuant-0.2.3/finquant/quants.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     2142 2023-07-08 06:47:36.000000 FinQuant-0.2.3/finquant/returns.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     4291 2023-07-08 08:26:58.000000 FinQuant-0.2.3/finquant/stock.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      106 2023-07-12 07:32:43.102127 FinQuant-0.2.3/setup.cfg
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     2173 2023-07-12 07:27:20.000000 FinQuant-0.2.3/setup.py
+drwxrwxrwx   0 frank     (1000) frank     (1000)        0 2023-07-12 07:32:43.088627 FinQuant-0.2.3/tests/
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      212 2023-07-08 06:47:36.000000 FinQuant-0.2.3/tests/test_efficient_frontier.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     6288 2023-07-08 08:26:58.000000 FinQuant-0.2.3/tests/test_moving_average.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)      212 2023-07-08 06:47:36.000000 FinQuant-0.2.3/tests/test_optimisation.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)    15918 2023-07-08 08:26:58.000000 FinQuant-0.2.3/tests/test_portfolio.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1283 2023-07-08 06:47:36.000000 FinQuant-0.2.3/tests/test_quants.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     2250 2023-07-08 06:47:36.000000 FinQuant-0.2.3/tests/test_returns.py
+-rwxrwxrwx   0 frank     (1000) frank     (1000)     1926 2023-07-08 08:26:58.000000 FinQuant-0.2.3/tests/test_stock.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `FinQuant-0.2.2/FinQuant.egg-info/PKG-INFO` & `FinQuant-0.2.3/FinQuant.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,297 +1,299 @@
 Metadata-Version: 2.1
 Name: FinQuant
-Version: 0.2.2
+Version: 0.2.3
 Summary: A program for financial portfolio management, analysis and optimisation
 Home-page: https://github.com/fmilthaler/FinQuant
+Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.2.3.tar.gz
 Author: Frank Milthaler
 Author-email: f.milthaler@gmail.com
 License: MIT
-Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.2.2.tar.gz
 Project-URL: Documentation, https://finquant.readthedocs.io
-Description: <p align="center">
-          <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-logo.png" width="45%">
-        </p>
-        
-        <p align="center">
-          <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
-            <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star&maxAge=2592000" alt='pypi'>
-          </a>
-          <a href="https://pypi.org/project/FinQuant">
-            <img src="https://img.shields.io/badge/pypi-v0.2.2-brightgreen.svg?style=popout" alt='pypi'>
-          </a>
-          <a href="https://travis-ci.org/fmilthaler/FinQuant">
-            <img src="https://travis-ci.org/fmilthaler/FinQuant.svg?style=popout?branch=master" alt='travis'>
-          </a>
-          <a href="http://finquant.readthedocs.io/">
-            <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
-          </a>
-          <a href="https://GitHub.com/fmilthaler/FinQuant/graphs/contributors/">
-            <img src="https://img.shields.io/github/contributors/fmilthaler/FinQuant.svg?style=popout" alt="contributors">
-          </a>
-          <a href="https://github.com/fmilthaler/FinQuant/issues">
-            <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=popout" alt="contributions">
-          </a>
-          <a href="https://github.com/fmilthaler/FinQuant/blob/master/LICENSE.txt">
-            <img src="https://img.shields.io/github/license/fmilthaler/FinQuant.svg?style=popout" alt="license">
-          </a>
-        </p>
-        
-        # FinQuant
-        *FinQuant* is a program for financial **portfolio management, analysis and optimisation**.
-        
-        This README only gives a brief overview of *FinQuant*. The interested reader should refer to its [documentation](https://finquant.readthedocs.io "FinQuant Documentation").
-        
-        ## Table of contents
-         - [Motivation](#Motivation)
-         - [Installation](#Installation)
-         - [Portfolio Management](#Portfolio-Management)
-         - [Returns](#Returns)
-         - [Moving Averages](#Moving-Averages)
-         - [Portfolio Optimisation](#Portfolio-Optimisation)
-           - [Efficient Frontier](#Efficient-Frontier)
-           - [Monte Carlo](#Monte-Carlo)
-         - [Examples](#Examples)
-           - [Building a portfolio with data from web](#Building-a-portfolio-with-data-from-web)
-           - [Building a portfolio with preset data](#Building-a-portfolio-with-preset-data)
-           - [Analysis of a portfolio](#Analysis-of-a-portfolio)
-           - [Optimisation of a portfolio](#Optimisation-of-a-portfolio)
-        
-        ## Motivation
-        Within a few lines of code, *FinQuant* can generate an object that holds your stock prices of your desired financial portfolio, analyses it, and can create plots of different kinds of *Returns*, *Moving Averages*, *Moving Average Bands with buy/sell signals*, and *Bollinger Bands*. It also allows for the optimisation based on the *Efficient Frontier* or a *Monte Carlo* run of the financial portfolio within a few lines of code. Some of the results are shown here.
-        
-        ### Automatically generating an instance of `Portfolio`
-        `finquant.portfolio.build_portfolio` is a function that eases the creating of your portfolio. See below for one of several ways of using `build_portfolio`.
-        ```
-        from finquant.portfolio import build_portfolio
-        names = ['GOOG', 'AMZN', 'MCD', 'DIS']
-        start_date = '2015-01-01'
-        end_date = '2017-12-31'
-        pf = build_portfolio(names=names,
-                            start_date=start_date,
-                            end_date=end_date)
-        ```
-        `pf` is an instance of `finquant.portfolio.Portfolio`, which contains the prices of the stocks in your portfolio. Then...
-        ```
-        pf.data.head(3)
-        ```
-        yields
-        ```
-                      GOOG    AMZN        MCD        DIS
-        Date
-        2015-01-02  524.81  308.52  85.783317  90.586146
-        2015-01-05  513.87  302.19  84.835892  89.262380
-        2015-01-06  501.96  295.29  84.992263  88.788916
-        ```
-        
-        ### Portfolio properties
-        Nicely printing out the portfolio's properties
-        ```
-        pf.properties()
-        ```
-        Depending on the stocks within your portfolio, the output looks something like the below.
-        ```
-        ----------------------------------------------------------------------
-        Stocks: GOOG, AMZN, MCD, DIS
-        Time window/frequency: 252
-        Risk free rate: 0.005
-        Portfolio expected return: 0.266
-        Portfolio volatility: 0.156
-        Portfolio Sharpe ratio: 1.674
-        
-        Skewness:
-               GOOG      AMZN      MCD       DIS
-        0  0.124184  0.087516  0.58698  0.040569
-        
-        Kurtosis:
-               GOOG      AMZN       MCD       DIS
-        0 -0.751818 -0.856101 -0.602008 -0.892666
-        
-        Information:
-           Allocation  Name
-        0        0.25  GOOG
-        1        0.25  AMZN
-        2        0.25   MCD
-        3        0.25   DIS
-        ----------------------------------------------------------------------
-        ```
-        
-        ### Cumulative Return
-        ```
-        pf.comp_cumulative_returns().plot().axhline(y = 0, color = "black", lw = 3)
-        ```
-        yields
-        <p align="center">
-          <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/cumulative-return.svg?sanitize=true" width="60%">
-        </p>
-        
-        ### Band Moving Average (Buy/Sell Signals)
-        ```
-        from finquant.moving_average import compute_ma, ema
-        # get stock data for disney
-        dis = pf.get_stock("DIS").data.copy(deep=True)
-        spans = [10, 50, 100, 150, 200]
-        ma = compute_ma(dis, ema, spans, plot=True)
-        ```
-        yields
-        <p align="center">
-          <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ma-band-buysell-signals.svg?sanitize=true" width="60%">
-        </p>
-        
-        ### Bollinger Band
-        ```
-        from finquant.moving_average import plot_bollinger_band
-        # get stock data for disney
-        dis = pf.get_stock("DIS").data.copy(deep=True)
-        span=20
-        plot_bollinger_band(dis, sma, span)
-        ```
-        yields
-        <p align="center">
-          <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/bollinger-band.svg?sanitize=true" width="60%">
-        </p>
-        
-        ### Portfolio Optimisation
-        ```
-        # performs and plots results of Monte Carlo run (5000 iterations)
-        opt_w, opt_res = pf.mc_optimisation(num_trials=5000)
-        # plots the results of the Monte Carlo optimisation
-        pf.mc_plot_results()
-        # plots the Efficient Frontier
-        pf.ef_plot_efrontier()
-        # plots optimal portfolios based on Efficient Frontier
-        pf.ef.plot_optimal_portfolios()
-        # plots individual plots of the portfolio
-        pf.plot_stocks()
-        ```
-        <p align="center">
-          <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ef-mc-overlay.svg?sanitize=true" width="60%">
-        </p>
-        
-        ## Installation
-        As it is common for open-source projects, there are several ways to get hold of the code. Choose whichever suits you and your purposes best.
-        
-        ### Dependencies
-        *FinQuant* depends on the following Python packages:
-         - python>=3.5.0
-         - numpy>=1.15
-         - pandas>=0.24
-         - matplotlib>=1.5.1
-         - quandl>=3.4.5
-         - yfinance>=0.1.43
-         - scipy>=1.2.0
-         - pytest>=2.8.7
-        
-        ### From PyPI
-        *FinQuant* can be obtained from PyPI
-        
-        ```pip install FinQuant```
-        
-        ### From GitHub
-        Get the code from GitHub:
-        
-        ```git clone https://github.com/fmilthaler/FinQuant.git```
-        
-        Then inside `FinQuant` run:
-        
-        ```python setup.py install```
-        
-        Alternatively, if you do not wish to install *FinQuant*, you can also download/clone it as stated above, and then make sure to add it to your ``PYTHONPATH``.
-        
-        ## Portfolio Management
-        This is the core of *FinQuant*. `finquant.portfolio.Portfolio` provides an object that holds prices of all stocks in your portfolio, and automatically computes the most common quantities for you. To make *FinQuant* an user-friendly program, that combines data analysis, visualisation and optimisation, the object provides interfaces to the main features that are provided in the modules in `./finquant/`.
-        
-        To learn more about the object, please read through the [documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant Documentation"), docstring of the module/class, and/or have a look at the examples.
-        
-        `finquant.portfolio.Portfolio` also provides a function `build_portfolio` which is designed to automatically generate an instance of `Portfolio` for the user's convenience. For more information on how to use `build_portfolio`, please refer to the [documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant Documentation"), its `docstring` and/or have a look at the examples.
-        
-        ## Returns
-        Daily returns of stocks are often computed in different ways. *FinQuant* provides three different ways of computing the daily returns in `finquant.returns`:
-        1. The cumulative return: <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/tex/738645698dc3073b4bb52a0c078ae829.svg?invert_in_darkmode&sanitize=true" align=middle width=194.52263655pt height=46.976899200000005pt/>
-        2. Percentage change of daily returns: <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/tex/27215e5f36fd0308b51ab510444edf0d.svg?invert_in_darkmode&sanitize=true" align=middle width=126.07712039999997pt height=48.84266309999997pt/>
-        3. Log Return: <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/tex/ef37c00ad58fe657a64041c3093e0640.svg?invert_in_darkmode&sanitize=true" align=middle width=208.3327686pt height=57.53473439999999pt/>
-        
-        In addition to those, the module provides the function `historical_mean_return(data, freq=252)`, which computes the historical mean of the daily returns over a time period `freq`.
-        
-        ## Moving Averages
-        The module `finquant.moving_average` allows the computation and visualisation of Moving Averages of the stocks listed in the portfolio is also provided. It entails functions to compute and visualise the
-         - `sma`: Simple Moving Average, and
-         - `ema`: Exponential Moving Average.
-         - `compute_ma`: a Band of Moving Averages (of different time windows/spans) including Buy/Sell signals
-         - `plot_bollinger_band`: a Bollinger Band for
-           - `sma`,
-           - `ema`.
-        
-        ## Portfolio Optimisation
-        ### Efficient Frontier
-        An implementation of the Efficient Frontier (`finquant.efficient_frontier.EfficientFrontier`) allows for the optimisation of the portfolio for
-         - `minimum_volatility` Minimum Volatility,
-         - `maximum_sharpe_ratio` Maximum Sharpe Ratio
-         - `efficient_return` Minimum Volatility for a given expected return
-         - `efficient_volatility` Maximum Sharpe Ratio for a given target volatility
-        
-        by performing a numerical solve to minimise/maximise an objective function.
-        
-        Often it is useful to visualise the *Efficient Frontier* as well as the optimal solution. This can be achieved with the following methods:
-         - `plot_efrontier`: Plots the *Efficient Frontier*. If no minimum/maximum Return values are provided, the algorithm automatically chooses those limits for the *Efficient Frontier* based on the minimum/maximum Return values of all stocks within the given portfolio.
-         - `plot_optimal_portfolios`: Plots markers of the portfolios with the Minimum Volatility and Maximum Sharpe Ratio.
-        
-        For reasons of user-friendliness, interfaces to these functions are provided in `finquant.portfolio.Portfolio`. Please have a look at the [documentation](https://finquant.readthedocs.io "FinQuant Documentation").
-        
-        ### Monte Carlo
-        Alternatively a *Monte Carlo* run of `n` trials can be performed to find the optimal portfolios for
-         - minimum volatility,
-         - maximum Sharpe ratio
-        
-        The approach branded as *Efficient Frontier* should be the preferred method for reasons of computational effort and accuracy. The latter approach is only included for the sake of completeness, and creation of beautiful plots.
-        
-        ## Examples
-        For more information about the project and details on how to use it, please
-        look at the examples provided in `./example`.
-        
-        **Note**: In the below examples, `pf` refers to an instance of `finquant.portfolio.Portfolio`, the object that holds all stock prices and computes its most common quantities automatically. To make *FinQuant* a user-friendly program, that combines data analysis, visualisation and optimisation, the object also provides interfaces to the main features that are provided in the modules in `./finquant/` and are discussed throughout this README.
-        
-        ### Building a portfolio with data from web
-        `./example/Example-Build-Portfolio-from-web.py`: Shows how to use *FinQuant* to build a financial portfolio by downloading stock price data through the Python package `quandl`/`yfinance`.
-        
-        ### Building a portfolio with preset data
-        `./example/Example-Build-Portfolio-from-file.py`: Shows how to use *FinQuant* to build a financial portfolio by providing stock price data yourself, e.g. by reading data from disk/file.
-        
-        ### Analysis of a portfolio
-        `./example/Example-Analysis.py`: This example shows how to use an instance of `finquant.portfolio.Portfolio`, get the portfolio's quantities, such as
-         - Expected Returns,
-         - Volatility,
-         - Sharpe Ratio.
-        
-        It also shows how to extract individual stocks from the given portfolio. Moreover it shows how to compute and visualise:
-         - the different Returns provided by the module `finquant.returns`,
-         - *Moving Averages*, a band of *Moving Averages*, and a *Bollinger Band*.
-        
-        ### Optimisation of a portfolio
-        `./example/Example-Optimisation.py`: This example focusses on the optimisation of a portfolio. To achieve this, the example shows the usage of `finquant.efficient_frontier.EfficientFrontier` for optimising the portfolio, for the
-         - Minimum Volatility
-         - Maximum Sharpe Ratio
-         - Minimum Volatility for a given target Return
-         - Maximum Sharpe Ratio for a given target Volatility.
-        
-        Furthermore, it is also shown how the entire *Efficient Frontier* and the optimal portfolios can be computed and visualised. If needed, it also gives an example of plotting the individual stocks of the given portfolio within the computed *Efficient Frontier*.
-        
-        Also, the optimisation of a portfolio and its visualisation based on a *Monte Carlo* is shown.
-        
-        Finally, *FinQuant*'s visualisation methods allow for overlays, if this is desired. Thus, with only the following few lines of code, one can create an overlay of the *Monte Carlo* run, the *Efficient Frontier*, its optimised portfolios for *Minimum Volatility* and *Maximum Sharpe Ratio*, as well as the portfolio's individual stocks.
-        
-        
 Keywords: finance,portfolio,investment,numerical,optimisation,monte carlo,efficient frontier,quantitative,quant
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: publish
+License-File: LICENSE.txt
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-logo.png" width="45%">
+</p>
+
+<p align="center">
+  <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
+    <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star" alt='pypi'>
+  </a>
+  <a href="https://pypi.org/project/FinQuant">
+    <img src="https://img.shields.io/badge/pypi-v0.2.2-brightgreen.svg?style=popout" alt='pypi'>
+  </a>
+  <a href="https://github.com/fmilthaler/FinQuant">
+    <img src="https://github.com/fmilthaler/finquant/actions/workflows/pytest.yml/badge.svg?branch=master" alt='GitHub Actions'>
+  </a>
+  <a href="http://finquant.readthedocs.io/">
+    <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
+  </a>
+  <a href="https://GitHub.com/fmilthaler/FinQuant/graphs/contributors/">
+    <img src="https://img.shields.io/github/contributors/fmilthaler/FinQuant.svg?style=popout" alt="contributors">
+  </a>
+  <a href="https://github.com/fmilthaler/FinQuant/issues">
+    <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=popout" alt="contributions">
+  </a>
+  <a href="https://github.com/fmilthaler/FinQuant/blob/master/LICENSE.txt">
+    <img src="https://img.shields.io/github/license/fmilthaler/FinQuant.svg?style=popout" alt="license">
+  </a>
+</p>
+
+# FinQuant
+*FinQuant* is a program for financial **portfolio management, analysis and optimisation**.
+
+This README only gives a brief overview of *FinQuant*. The interested reader should refer to its [documentation](https://finquant.readthedocs.io "FinQuant Documentation").
+
+## Table of contents
+ - [Motivation](#Motivation)
+ - [Installation](#Installation)
+ - [Portfolio Management](#Portfolio-Management)
+ - [Returns](#Returns)
+ - [Moving Averages](#Moving-Averages)
+ - [Portfolio Optimisation](#Portfolio-Optimisation)
+   - [Efficient Frontier](#Efficient-Frontier)
+   - [Monte Carlo](#Monte-Carlo)
+ - [Examples](#Examples)
+   - [Building a portfolio with data from web](#Building-a-portfolio-with-data-from-web)
+   - [Building a portfolio with preset data](#Building-a-portfolio-with-preset-data)
+   - [Analysis of a portfolio](#Analysis-of-a-portfolio)
+   - [Optimisation of a portfolio](#Optimisation-of-a-portfolio)
+
+## Motivation
+Within a few lines of code, *FinQuant* can generate an object that holds your stock prices of your desired financial portfolio, analyses it, and can create plots of different kinds of *Returns*, *Moving Averages*, *Moving Average Bands with buy/sell signals*, and *Bollinger Bands*. It also allows for the optimisation based on the *Efficient Frontier* or a *Monte Carlo* run of the financial portfolio within a few lines of code. Some of the results are shown here.
+
+### Automatically generating an instance of `Portfolio`
+`finquant.portfolio.build_portfolio` is a function that eases the creating of your portfolio. See below for one of several ways of using `build_portfolio`.
+```
+from finquant.portfolio import build_portfolio
+names = ['GOOG', 'AMZN', 'MCD', 'DIS']
+start_date = '2015-01-01'
+end_date = '2017-12-31'
+pf = build_portfolio(names=names,
+                    start_date=start_date,
+                    end_date=end_date)
+```
+`pf` is an instance of `finquant.portfolio.Portfolio`, which contains the prices of the stocks in your portfolio. Then...
+```
+pf.data.head(3)
+```
+yields
+```
+              GOOG    AMZN        MCD        DIS
+Date
+2015-01-02  524.81  308.52  85.783317  90.586146
+2015-01-05  513.87  302.19  84.835892  89.262380
+2015-01-06  501.96  295.29  84.992263  88.788916
+```
+
+### Portfolio properties
+Nicely printing out the portfolio's properties
+```
+pf.properties()
+```
+Depending on the stocks within your portfolio, the output looks something like the below.
+```
+----------------------------------------------------------------------
+Stocks: GOOG, AMZN, MCD, DIS
+Time window/frequency: 252
+Risk free rate: 0.005
+Portfolio expected return: 0.266
+Portfolio volatility: 0.156
+Portfolio Sharpe ratio: 1.674
+
+Skewness:
+       GOOG      AMZN      MCD       DIS
+0  0.124184  0.087516  0.58698  0.040569
+
+Kurtosis:
+       GOOG      AMZN       MCD       DIS
+0 -0.751818 -0.856101 -0.602008 -0.892666
+
+Information:
+   Allocation  Name
+0        0.25  GOOG
+1        0.25  AMZN
+2        0.25   MCD
+3        0.25   DIS
+----------------------------------------------------------------------
+```
+
+### Cumulative Return
+```
+pf.comp_cumulative_returns().plot().axhline(y = 0, color = "black", lw = 3)
+```
+yields
+<p align="center">
+  <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/cumulative-return.svg?sanitize=true" width="60%">
+</p>
+
+### Band Moving Average (Buy/Sell Signals)
+```
+from finquant.moving_average import compute_ma, ema
+# get stock data for disney
+dis = pf.get_stock("DIS").data.copy(deep=True)
+spans = [10, 50, 100, 150, 200]
+ma = compute_ma(dis, ema, spans, plot=True)
+```
+yields
+<p align="center">
+  <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ma-band-buysell-signals.svg?sanitize=true" width="60%">
+</p>
+
+### Bollinger Band
+```
+from finquant.moving_average import plot_bollinger_band, sma
+# get stock data for disney
+dis = pf.get_stock("DIS").data.copy(deep=True)
+span=20
+plot_bollinger_band(dis, sma, span)
+```
+yields
+<p align="center">
+  <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/bollinger-band.svg?sanitize=true" width="60%">
+</p>
+
+### Portfolio Optimisation
+```
+# performs and plots results of Monte Carlo run (5000 iterations)
+opt_w, opt_res = pf.mc_optimisation(num_trials=5000)
+# plots the results of the Monte Carlo optimisation
+pf.mc_plot_results()
+# plots the Efficient Frontier
+pf.ef_plot_efrontier()
+# plots optimal portfolios based on Efficient Frontier
+pf.ef.plot_optimal_portfolios()
+# plots individual plots of the portfolio
+pf.plot_stocks()
+```
+<p align="center">
+  <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ef-mc-overlay.svg?sanitize=true" width="60%">
+</p>
+
+## Installation
+As it is common for open-source projects, there are several ways to get hold of the code. Choose whichever suits you and your purposes best.
+
+### Dependencies
+*FinQuant* depends on the following Python packages:
+ - python>=3.10
+ - numpy>=1.15
+ - pandas>=2.0
+ - matplotlib>=3.0
+ - quandl>=3.4.5
+ - yfinance>=0.1.43
+ - scipy>=1.2.0
+
+### From PyPI
+*FinQuant* can be obtained from PyPI
+
+```pip install FinQuant```
+
+### From GitHub
+Get the code from GitHub:
+
+```git clone https://github.com/fmilthaler/FinQuant.git```
+
+Then inside `FinQuant` run:
+
+```python setup.py install```
+
+Alternatively, if you do not wish to install *FinQuant*, you can also download/clone it as stated above, and then make sure to add it to your ``PYTHONPATH``.
+
+## Portfolio Management
+This is the core of *FinQuant*. `finquant.portfolio.Portfolio` provides an object that holds prices of all stocks in your portfolio, and automatically computes the most common quantities for you. To make *FinQuant* an user-friendly program, that combines data analysis, visualisation and optimisation, the object provides interfaces to the main features that are provided in the modules in `./finquant/`.
+
+To learn more about the object, please read through the [documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant Documentation"), docstring of the module/class, and/or have a look at the examples.
+
+`finquant.portfolio.Portfolio` also provides a function `build_portfolio` which is designed to automatically generate an instance of `Portfolio` for the user's convenience. For more information on how to use `build_portfolio`, please refer to the [documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant Documentation"), its `docstring` and/or have a look at the examples.
+
+## Returns
+Daily returns of stocks are often computed in different ways. *FinQuant* provides three different ways of computing the daily returns in `finquant.returns`:
+1. The cumulative return: <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/tex/738645698dc3073b4bb52a0c078ae829.svg?invert_in_darkmode&sanitize=true" align=middle width=194.52263655pt height=46.976899200000005pt/>
+2. Percentage change of daily returns: <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/tex/27215e5f36fd0308b51ab510444edf0d.svg?invert_in_darkmode&sanitize=true" align=middle width=126.07712039999997pt height=48.84266309999997pt/>
+3. Log Return: <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/tex/ef37c00ad58fe657a64041c3093e0640.svg?invert_in_darkmode&sanitize=true" align=middle width=208.3327686pt height=57.53473439999999pt/>
+
+In addition to those, the module provides the function `historical_mean_return(data, freq=252)`, which computes the historical mean of the daily returns over a time period `freq`.
+
+## Moving Averages
+The module `finquant.moving_average` allows the computation and visualisation of Moving Averages of the stocks listed in the portfolio is also provided. It entails functions to compute and visualise the
+ - `sma`: Simple Moving Average, and
+ - `ema`: Exponential Moving Average.
+ - `compute_ma`: a Band of Moving Averages (of different time windows/spans) including Buy/Sell signals
+ - `plot_bollinger_band`: a Bollinger Band for
+   - `sma`,
+   - `ema`.
+
+## Portfolio Optimisation
+### Efficient Frontier
+An implementation of the Efficient Frontier (`finquant.efficient_frontier.EfficientFrontier`) allows for the optimisation of the portfolio for
+ - `minimum_volatility` Minimum Volatility,
+ - `maximum_sharpe_ratio` Maximum Sharpe Ratio
+ - `efficient_return` Minimum Volatility for a given expected return
+ - `efficient_volatility` Maximum Sharpe Ratio for a given target volatility
+
+by performing a numerical solve to minimise/maximise an objective function.
+
+Often it is useful to visualise the *Efficient Frontier* as well as the optimal solution. This can be achieved with the following methods:
+ - `plot_efrontier`: Plots the *Efficient Frontier*. If no minimum/maximum Return values are provided, the algorithm automatically chooses those limits for the *Efficient Frontier* based on the minimum/maximum Return values of all stocks within the given portfolio.
+ - `plot_optimal_portfolios`: Plots markers of the portfolios with the Minimum Volatility and Maximum Sharpe Ratio.
+
+For reasons of user-friendliness, interfaces to these functions are provided in `finquant.portfolio.Portfolio`. Please have a look at the [documentation](https://finquant.readthedocs.io "FinQuant Documentation").
+
+### Monte Carlo
+Alternatively a *Monte Carlo* run of `n` trials can be performed to find the optimal portfolios for
+ - minimum volatility,
+ - maximum Sharpe ratio
+
+The approach branded as *Efficient Frontier* should be the preferred method for reasons of computational effort and accuracy. The latter approach is only included for the sake of completeness, and creation of beautiful plots.
+
+## Examples
+For more information about the project and details on how to use it, please
+look at the examples provided in `./example`.
+
+**Note**: In the below examples, `pf` refers to an instance of `finquant.portfolio.Portfolio`, the object that holds all stock prices and computes its most common quantities automatically. To make *FinQuant* a user-friendly program, that combines data analysis, visualisation and optimisation, the object also provides interfaces to the main features that are provided in the modules in `./finquant/` and are discussed throughout this README.
+
+### Building a portfolio with data from web
+`./example/Example-Build-Portfolio-from-web.py`: Shows how to use *FinQuant* to build a financial portfolio by downloading stock price data through the Python package `quandl`/`yfinance`.
+
+### Building a portfolio with preset data
+`./example/Example-Build-Portfolio-from-file.py`: Shows how to use *FinQuant* to build a financial portfolio by providing stock price data yourself, e.g. by reading data from disk/file.
+
+### Analysis of a portfolio
+`./example/Example-Analysis.py`: This example shows how to use an instance of `finquant.portfolio.Portfolio`, get the portfolio's quantities, such as
+ - Expected Returns,
+ - Volatility,
+ - Sharpe Ratio.
+
+It also shows how to extract individual stocks from the given portfolio. Moreover it shows how to compute and visualise:
+ - the different Returns provided by the module `finquant.returns`,
+ - *Moving Averages*, a band of *Moving Averages*, and a *Bollinger Band*.
+
+### Optimisation of a portfolio
+`./example/Example-Optimisation.py`: This example focusses on the optimisation of a portfolio. To achieve this, the example shows the usage of `finquant.efficient_frontier.EfficientFrontier` for optimising the portfolio, for the
+ - Minimum Volatility
+ - Maximum Sharpe Ratio
+ - Minimum Volatility for a given target Return
+ - Maximum Sharpe Ratio for a given target Volatility.
+
+Furthermore, it is also shown how the entire *Efficient Frontier* and the optimal portfolios can be computed and visualised. If needed, it also gives an example of plotting the individual stocks of the given portfolio within the computed *Efficient Frontier*.
+
+Also, the optimisation of a portfolio and its visualisation based on a *Monte Carlo* is shown.
+
+Finally, *FinQuant*'s visualisation methods allow for overlays, if this is desired. Thus, with only the following few lines of code, one can create an overlay of the *Monte Carlo* run, the *Efficient Frontier*, its optimised portfolios for *Minimum Volatility* and *Maximum Sharpe Ratio*, as well as the portfolio's individual stocks.
+
```

#### html2text {}

```diff
@@ -1,16 +1,27 @@
-Metadata-Version: 2.1 Name: FinQuant Version: 0.2.2 Summary: A program for
+Metadata-Version: 2.1 Name: FinQuant Version: 0.2.3 Summary: A program for
 financial portfolio management, analysis and optimisation Home-page: https://
-github.com/fmilthaler/FinQuant Author: Frank Milthaler Author-email:
-f.milthaler@gmail.com License: MIT Download-URL: https://github.com/fmilthaler/
-FinQuant/archive/v0.2.2.tar.gz Project-URL: Documentation, https://
-finquant.readthedocs.io Description:
+github.com/fmilthaler/FinQuant Download-URL: https://github.com/fmilthaler/
+FinQuant/archive/v0.2.3.tar.gz Author: Frank Milthaler Author-email:
+f.milthaler@gmail.com License: MIT Project-URL: Documentation, https://
+finquant.readthedocs.io Keywords:
+finance,portfolio,investment,numerical,optimisation,monte carlo,efficient
+frontier,quantitative,quant Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Education Classifier: Intended Audience ::
+Financial and Insurance Industry Classifier: Intended Audience :: Other
+Audience Classifier: Intended Audience :: Science/Research Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
+Provides-Extra: test Provides-Extra: dev Provides-Extra: docs Provides-Extra:
+publish License-File: LICENSE.txt
 [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-
                                    logo.png]
-    [pypi] [pypi] [travis] [docs] [contributors] [contributions] [license]
+[pypi] [pypi] [GitHub_Actions] [docs] [contributors] [contributions] [license]
 # FinQuant *FinQuant* is a program for financial **portfolio management,
 analysis and optimisation**. This README only gives a brief overview of
 *FinQuant*. The interested reader should refer to its [documentation](https://
 finquant.readthedocs.io "FinQuant Documentation"). ## Table of contents -
 [Motivation](#Motivation) - [Installation](#Installation) - [Portfolio
 Management](#Portfolio-Management) - [Returns](#Returns) - [Moving Averages]
 (#Moving-Averages) - [Portfolio Optimisation](#Portfolio-Optimisation) -
@@ -50,44 +61,44 @@
                      cumulative-return.svg?sanitize=true]
 ### Band Moving Average (Buy/Sell Signals) ``` from finquant.moving_average
 import compute_ma, ema # get stock data for disney dis = pf.get_stock
 ("DIS").data.copy(deep=True) spans = [10, 50, 100, 150, 200] ma = compute_ma
 (dis, ema, spans, plot=True) ``` yields
  [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ma-band-
                       buysell-signals.svg?sanitize=true]
-### Bollinger Band ``` from finquant.moving_average import plot_bollinger_band
-# get stock data for disney dis = pf.get_stock("DIS").data.copy(deep=True)
+### Bollinger Band ``` from finquant.moving_average import plot_bollinger_band,
+sma # get stock data for disney dis = pf.get_stock("DIS").data.copy(deep=True)
 span=20 plot_bollinger_band(dis, sma, span) ``` yields
 [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/bollinger-
                             band.svg?sanitize=true]
 ### Portfolio Optimisation ``` # performs and plots results of Monte Carlo run
 (5000 iterations) opt_w, opt_res = pf.mc_optimisation(num_trials=5000) # plots
 the results of the Monte Carlo optimisation pf.mc_plot_results() # plots the
 Efficient Frontier pf.ef_plot_efrontier() # plots optimal portfolios based on
 Efficient Frontier pf.ef.plot_optimal_portfolios() # plots individual plots of
 the portfolio pf.plot_stocks() ```
   [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ef-mc-
                           overlay.svg?sanitize=true]
 ## Installation As it is common for open-source projects, there are several
 ways to get hold of the code. Choose whichever suits you and your purposes
 best. ### Dependencies *FinQuant* depends on the following Python packages: -
-python>=3.5.0 - numpy>=1.15 - pandas>=0.24 - matplotlib>=1.5.1 - quandl>=3.4.5
-- yfinance>=0.1.43 - scipy>=1.2.0 - pytest>=2.8.7 ### From PyPI *FinQuant* can
-be obtained from PyPI ```pip install FinQuant``` ### From GitHub Get the code
-from GitHub: ```git clone https://github.com/fmilthaler/FinQuant.git``` Then
-inside `FinQuant` run: ```python setup.py install``` Alternatively, if you do
-not wish to install *FinQuant*, you can also download/clone it as stated above,
-and then make sure to add it to your ``PYTHONPATH``. ## Portfolio Management
-This is the core of *FinQuant*. `finquant.portfolio.Portfolio` provides an
-object that holds prices of all stocks in your portfolio, and automatically
-computes the most common quantities for you. To make *FinQuant* an user-
-friendly program, that combines data analysis, visualisation and optimisation,
-the object provides interfaces to the main features that are provided in the
-modules in `./finquant/`. To learn more about the object, please read through
-the [documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant
+python>=3.10 - numpy>=1.15 - pandas>=2.0 - matplotlib>=3.0 - quandl>=3.4.5 -
+yfinance>=0.1.43 - scipy>=1.2.0 ### From PyPI *FinQuant* can be obtained from
+PyPI ```pip install FinQuant``` ### From GitHub Get the code from GitHub:
+```git clone https://github.com/fmilthaler/FinQuant.git``` Then inside
+`FinQuant` run: ```python setup.py install``` Alternatively, if you do not wish
+to install *FinQuant*, you can also download/clone it as stated above, and then
+make sure to add it to your ``PYTHONPATH``. ## Portfolio Management This is the
+core of *FinQuant*. `finquant.portfolio.Portfolio` provides an object that
+holds prices of all stocks in your portfolio, and automatically computes the
+most common quantities for you. To make *FinQuant* an user-friendly program,
+that combines data analysis, visualisation and optimisation, the object
+provides interfaces to the main features that are provided in the modules in
+`./finquant/`. To learn more about the object, please read through the
+[documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant
 Documentation"), docstring of the module/class, and/or have a look at the
 examples. `finquant.portfolio.Portfolio` also provides a function
 `build_portfolio` which is designed to automatically generate an instance of
 `Portfolio` for the user's convenience. For more information on how to use
 `build_portfolio`, please refer to the [documentation](https://
 finquant.readthedocs.io/en/latest/ "FinQuant Documentation"), its `docstring`
 and/or have a look at the examples. ## Returns Daily returns of stocks are
@@ -161,17 +172,8 @@
 example of plotting the individual stocks of the given portfolio within the
 computed *Efficient Frontier*. Also, the optimisation of a portfolio and its
 visualisation based on a *Monte Carlo* is shown. Finally, *FinQuant*'s
 visualisation methods allow for overlays, if this is desired. Thus, with only
 the following few lines of code, one can create an overlay of the *Monte Carlo*
 run, the *Efficient Frontier*, its optimised portfolios for *Minimum
 Volatility* and *Maximum Sharpe Ratio*, as well as the portfolio's individual
-stocks. Keywords: finance,portfolio,investment,numerical,optimisation,monte
-carlo,efficient frontier,quantitative,quant Platform: UNKNOWN Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Financial and Insurance Industry Classifier:
-Intended Audience :: Other Audience Classifier: Intended Audience :: Science/
-Research Classifier: Programming Language :: Python :: 3 :: Only Classifier:
-Programming Language :: Python :: 3.5 Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.5 Description-Content-Type: text/markdown
+stocks.
```

### Comparing `FinQuant-0.2.2/PKG-INFO` & `FinQuant-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,297 +1,299 @@
 Metadata-Version: 2.1
 Name: FinQuant
-Version: 0.2.2
+Version: 0.2.3
 Summary: A program for financial portfolio management, analysis and optimisation
 Home-page: https://github.com/fmilthaler/FinQuant
+Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.2.3.tar.gz
 Author: Frank Milthaler
 Author-email: f.milthaler@gmail.com
 License: MIT
-Download-URL: https://github.com/fmilthaler/FinQuant/archive/v0.2.2.tar.gz
 Project-URL: Documentation, https://finquant.readthedocs.io
-Description: <p align="center">
-          <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-logo.png" width="45%">
-        </p>
-        
-        <p align="center">
-          <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
-            <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star&maxAge=2592000" alt='pypi'>
-          </a>
-          <a href="https://pypi.org/project/FinQuant">
-            <img src="https://img.shields.io/badge/pypi-v0.2.2-brightgreen.svg?style=popout" alt='pypi'>
-          </a>
-          <a href="https://travis-ci.org/fmilthaler/FinQuant">
-            <img src="https://travis-ci.org/fmilthaler/FinQuant.svg?style=popout?branch=master" alt='travis'>
-          </a>
-          <a href="http://finquant.readthedocs.io/">
-            <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
-          </a>
-          <a href="https://GitHub.com/fmilthaler/FinQuant/graphs/contributors/">
-            <img src="https://img.shields.io/github/contributors/fmilthaler/FinQuant.svg?style=popout" alt="contributors">
-          </a>
-          <a href="https://github.com/fmilthaler/FinQuant/issues">
-            <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=popout" alt="contributions">
-          </a>
-          <a href="https://github.com/fmilthaler/FinQuant/blob/master/LICENSE.txt">
-            <img src="https://img.shields.io/github/license/fmilthaler/FinQuant.svg?style=popout" alt="license">
-          </a>
-        </p>
-        
-        # FinQuant
-        *FinQuant* is a program for financial **portfolio management, analysis and optimisation**.
-        
-        This README only gives a brief overview of *FinQuant*. The interested reader should refer to its [documentation](https://finquant.readthedocs.io "FinQuant Documentation").
-        
-        ## Table of contents
-         - [Motivation](#Motivation)
-         - [Installation](#Installation)
-         - [Portfolio Management](#Portfolio-Management)
-         - [Returns](#Returns)
-         - [Moving Averages](#Moving-Averages)
-         - [Portfolio Optimisation](#Portfolio-Optimisation)
-           - [Efficient Frontier](#Efficient-Frontier)
-           - [Monte Carlo](#Monte-Carlo)
-         - [Examples](#Examples)
-           - [Building a portfolio with data from web](#Building-a-portfolio-with-data-from-web)
-           - [Building a portfolio with preset data](#Building-a-portfolio-with-preset-data)
-           - [Analysis of a portfolio](#Analysis-of-a-portfolio)
-           - [Optimisation of a portfolio](#Optimisation-of-a-portfolio)
-        
-        ## Motivation
-        Within a few lines of code, *FinQuant* can generate an object that holds your stock prices of your desired financial portfolio, analyses it, and can create plots of different kinds of *Returns*, *Moving Averages*, *Moving Average Bands with buy/sell signals*, and *Bollinger Bands*. It also allows for the optimisation based on the *Efficient Frontier* or a *Monte Carlo* run of the financial portfolio within a few lines of code. Some of the results are shown here.
-        
-        ### Automatically generating an instance of `Portfolio`
-        `finquant.portfolio.build_portfolio` is a function that eases the creating of your portfolio. See below for one of several ways of using `build_portfolio`.
-        ```
-        from finquant.portfolio import build_portfolio
-        names = ['GOOG', 'AMZN', 'MCD', 'DIS']
-        start_date = '2015-01-01'
-        end_date = '2017-12-31'
-        pf = build_portfolio(names=names,
-                            start_date=start_date,
-                            end_date=end_date)
-        ```
-        `pf` is an instance of `finquant.portfolio.Portfolio`, which contains the prices of the stocks in your portfolio. Then...
-        ```
-        pf.data.head(3)
-        ```
-        yields
-        ```
-                      GOOG    AMZN        MCD        DIS
-        Date
-        2015-01-02  524.81  308.52  85.783317  90.586146
-        2015-01-05  513.87  302.19  84.835892  89.262380
-        2015-01-06  501.96  295.29  84.992263  88.788916
-        ```
-        
-        ### Portfolio properties
-        Nicely printing out the portfolio's properties
-        ```
-        pf.properties()
-        ```
-        Depending on the stocks within your portfolio, the output looks something like the below.
-        ```
-        ----------------------------------------------------------------------
-        Stocks: GOOG, AMZN, MCD, DIS
-        Time window/frequency: 252
-        Risk free rate: 0.005
-        Portfolio expected return: 0.266
-        Portfolio volatility: 0.156
-        Portfolio Sharpe ratio: 1.674
-        
-        Skewness:
-               GOOG      AMZN      MCD       DIS
-        0  0.124184  0.087516  0.58698  0.040569
-        
-        Kurtosis:
-               GOOG      AMZN       MCD       DIS
-        0 -0.751818 -0.856101 -0.602008 -0.892666
-        
-        Information:
-           Allocation  Name
-        0        0.25  GOOG
-        1        0.25  AMZN
-        2        0.25   MCD
-        3        0.25   DIS
-        ----------------------------------------------------------------------
-        ```
-        
-        ### Cumulative Return
-        ```
-        pf.comp_cumulative_returns().plot().axhline(y = 0, color = "black", lw = 3)
-        ```
-        yields
-        <p align="center">
-          <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/cumulative-return.svg?sanitize=true" width="60%">
-        </p>
-        
-        ### Band Moving Average (Buy/Sell Signals)
-        ```
-        from finquant.moving_average import compute_ma, ema
-        # get stock data for disney
-        dis = pf.get_stock("DIS").data.copy(deep=True)
-        spans = [10, 50, 100, 150, 200]
-        ma = compute_ma(dis, ema, spans, plot=True)
-        ```
-        yields
-        <p align="center">
-          <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ma-band-buysell-signals.svg?sanitize=true" width="60%">
-        </p>
-        
-        ### Bollinger Band
-        ```
-        from finquant.moving_average import plot_bollinger_band
-        # get stock data for disney
-        dis = pf.get_stock("DIS").data.copy(deep=True)
-        span=20
-        plot_bollinger_band(dis, sma, span)
-        ```
-        yields
-        <p align="center">
-          <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/bollinger-band.svg?sanitize=true" width="60%">
-        </p>
-        
-        ### Portfolio Optimisation
-        ```
-        # performs and plots results of Monte Carlo run (5000 iterations)
-        opt_w, opt_res = pf.mc_optimisation(num_trials=5000)
-        # plots the results of the Monte Carlo optimisation
-        pf.mc_plot_results()
-        # plots the Efficient Frontier
-        pf.ef_plot_efrontier()
-        # plots optimal portfolios based on Efficient Frontier
-        pf.ef.plot_optimal_portfolios()
-        # plots individual plots of the portfolio
-        pf.plot_stocks()
-        ```
-        <p align="center">
-          <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ef-mc-overlay.svg?sanitize=true" width="60%">
-        </p>
-        
-        ## Installation
-        As it is common for open-source projects, there are several ways to get hold of the code. Choose whichever suits you and your purposes best.
-        
-        ### Dependencies
-        *FinQuant* depends on the following Python packages:
-         - python>=3.5.0
-         - numpy>=1.15
-         - pandas>=0.24
-         - matplotlib>=1.5.1
-         - quandl>=3.4.5
-         - yfinance>=0.1.43
-         - scipy>=1.2.0
-         - pytest>=2.8.7
-        
-        ### From PyPI
-        *FinQuant* can be obtained from PyPI
-        
-        ```pip install FinQuant```
-        
-        ### From GitHub
-        Get the code from GitHub:
-        
-        ```git clone https://github.com/fmilthaler/FinQuant.git```
-        
-        Then inside `FinQuant` run:
-        
-        ```python setup.py install```
-        
-        Alternatively, if you do not wish to install *FinQuant*, you can also download/clone it as stated above, and then make sure to add it to your ``PYTHONPATH``.
-        
-        ## Portfolio Management
-        This is the core of *FinQuant*. `finquant.portfolio.Portfolio` provides an object that holds prices of all stocks in your portfolio, and automatically computes the most common quantities for you. To make *FinQuant* an user-friendly program, that combines data analysis, visualisation and optimisation, the object provides interfaces to the main features that are provided in the modules in `./finquant/`.
-        
-        To learn more about the object, please read through the [documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant Documentation"), docstring of the module/class, and/or have a look at the examples.
-        
-        `finquant.portfolio.Portfolio` also provides a function `build_portfolio` which is designed to automatically generate an instance of `Portfolio` for the user's convenience. For more information on how to use `build_portfolio`, please refer to the [documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant Documentation"), its `docstring` and/or have a look at the examples.
-        
-        ## Returns
-        Daily returns of stocks are often computed in different ways. *FinQuant* provides three different ways of computing the daily returns in `finquant.returns`:
-        1. The cumulative return: <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/tex/738645698dc3073b4bb52a0c078ae829.svg?invert_in_darkmode&sanitize=true" align=middle width=194.52263655pt height=46.976899200000005pt/>
-        2. Percentage change of daily returns: <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/tex/27215e5f36fd0308b51ab510444edf0d.svg?invert_in_darkmode&sanitize=true" align=middle width=126.07712039999997pt height=48.84266309999997pt/>
-        3. Log Return: <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/tex/ef37c00ad58fe657a64041c3093e0640.svg?invert_in_darkmode&sanitize=true" align=middle width=208.3327686pt height=57.53473439999999pt/>
-        
-        In addition to those, the module provides the function `historical_mean_return(data, freq=252)`, which computes the historical mean of the daily returns over a time period `freq`.
-        
-        ## Moving Averages
-        The module `finquant.moving_average` allows the computation and visualisation of Moving Averages of the stocks listed in the portfolio is also provided. It entails functions to compute and visualise the
-         - `sma`: Simple Moving Average, and
-         - `ema`: Exponential Moving Average.
-         - `compute_ma`: a Band of Moving Averages (of different time windows/spans) including Buy/Sell signals
-         - `plot_bollinger_band`: a Bollinger Band for
-           - `sma`,
-           - `ema`.
-        
-        ## Portfolio Optimisation
-        ### Efficient Frontier
-        An implementation of the Efficient Frontier (`finquant.efficient_frontier.EfficientFrontier`) allows for the optimisation of the portfolio for
-         - `minimum_volatility` Minimum Volatility,
-         - `maximum_sharpe_ratio` Maximum Sharpe Ratio
-         - `efficient_return` Minimum Volatility for a given expected return
-         - `efficient_volatility` Maximum Sharpe Ratio for a given target volatility
-        
-        by performing a numerical solve to minimise/maximise an objective function.
-        
-        Often it is useful to visualise the *Efficient Frontier* as well as the optimal solution. This can be achieved with the following methods:
-         - `plot_efrontier`: Plots the *Efficient Frontier*. If no minimum/maximum Return values are provided, the algorithm automatically chooses those limits for the *Efficient Frontier* based on the minimum/maximum Return values of all stocks within the given portfolio.
-         - `plot_optimal_portfolios`: Plots markers of the portfolios with the Minimum Volatility and Maximum Sharpe Ratio.
-        
-        For reasons of user-friendliness, interfaces to these functions are provided in `finquant.portfolio.Portfolio`. Please have a look at the [documentation](https://finquant.readthedocs.io "FinQuant Documentation").
-        
-        ### Monte Carlo
-        Alternatively a *Monte Carlo* run of `n` trials can be performed to find the optimal portfolios for
-         - minimum volatility,
-         - maximum Sharpe ratio
-        
-        The approach branded as *Efficient Frontier* should be the preferred method for reasons of computational effort and accuracy. The latter approach is only included for the sake of completeness, and creation of beautiful plots.
-        
-        ## Examples
-        For more information about the project and details on how to use it, please
-        look at the examples provided in `./example`.
-        
-        **Note**: In the below examples, `pf` refers to an instance of `finquant.portfolio.Portfolio`, the object that holds all stock prices and computes its most common quantities automatically. To make *FinQuant* a user-friendly program, that combines data analysis, visualisation and optimisation, the object also provides interfaces to the main features that are provided in the modules in `./finquant/` and are discussed throughout this README.
-        
-        ### Building a portfolio with data from web
-        `./example/Example-Build-Portfolio-from-web.py`: Shows how to use *FinQuant* to build a financial portfolio by downloading stock price data through the Python package `quandl`/`yfinance`.
-        
-        ### Building a portfolio with preset data
-        `./example/Example-Build-Portfolio-from-file.py`: Shows how to use *FinQuant* to build a financial portfolio by providing stock price data yourself, e.g. by reading data from disk/file.
-        
-        ### Analysis of a portfolio
-        `./example/Example-Analysis.py`: This example shows how to use an instance of `finquant.portfolio.Portfolio`, get the portfolio's quantities, such as
-         - Expected Returns,
-         - Volatility,
-         - Sharpe Ratio.
-        
-        It also shows how to extract individual stocks from the given portfolio. Moreover it shows how to compute and visualise:
-         - the different Returns provided by the module `finquant.returns`,
-         - *Moving Averages*, a band of *Moving Averages*, and a *Bollinger Band*.
-        
-        ### Optimisation of a portfolio
-        `./example/Example-Optimisation.py`: This example focusses on the optimisation of a portfolio. To achieve this, the example shows the usage of `finquant.efficient_frontier.EfficientFrontier` for optimising the portfolio, for the
-         - Minimum Volatility
-         - Maximum Sharpe Ratio
-         - Minimum Volatility for a given target Return
-         - Maximum Sharpe Ratio for a given target Volatility.
-        
-        Furthermore, it is also shown how the entire *Efficient Frontier* and the optimal portfolios can be computed and visualised. If needed, it also gives an example of plotting the individual stocks of the given portfolio within the computed *Efficient Frontier*.
-        
-        Also, the optimisation of a portfolio and its visualisation based on a *Monte Carlo* is shown.
-        
-        Finally, *FinQuant*'s visualisation methods allow for overlays, if this is desired. Thus, with only the following few lines of code, one can create an overlay of the *Monte Carlo* run, the *Efficient Frontier*, its optimised portfolios for *Minimum Volatility* and *Maximum Sharpe Ratio*, as well as the portfolio's individual stocks.
-        
-        
 Keywords: finance,portfolio,investment,numerical,optimisation,monte carlo,efficient frontier,quantitative,quant
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: publish
+License-File: LICENSE.txt
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-logo.png" width="45%">
+</p>
+
+<p align="center">
+  <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
+    <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star" alt='pypi'>
+  </a>
+  <a href="https://pypi.org/project/FinQuant">
+    <img src="https://img.shields.io/badge/pypi-v0.2.2-brightgreen.svg?style=popout" alt='pypi'>
+  </a>
+  <a href="https://github.com/fmilthaler/FinQuant">
+    <img src="https://github.com/fmilthaler/finquant/actions/workflows/pytest.yml/badge.svg?branch=master" alt='GitHub Actions'>
+  </a>
+  <a href="http://finquant.readthedocs.io/">
+    <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
+  </a>
+  <a href="https://GitHub.com/fmilthaler/FinQuant/graphs/contributors/">
+    <img src="https://img.shields.io/github/contributors/fmilthaler/FinQuant.svg?style=popout" alt="contributors">
+  </a>
+  <a href="https://github.com/fmilthaler/FinQuant/issues">
+    <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=popout" alt="contributions">
+  </a>
+  <a href="https://github.com/fmilthaler/FinQuant/blob/master/LICENSE.txt">
+    <img src="https://img.shields.io/github/license/fmilthaler/FinQuant.svg?style=popout" alt="license">
+  </a>
+</p>
+
+# FinQuant
+*FinQuant* is a program for financial **portfolio management, analysis and optimisation**.
+
+This README only gives a brief overview of *FinQuant*. The interested reader should refer to its [documentation](https://finquant.readthedocs.io "FinQuant Documentation").
+
+## Table of contents
+ - [Motivation](#Motivation)
+ - [Installation](#Installation)
+ - [Portfolio Management](#Portfolio-Management)
+ - [Returns](#Returns)
+ - [Moving Averages](#Moving-Averages)
+ - [Portfolio Optimisation](#Portfolio-Optimisation)
+   - [Efficient Frontier](#Efficient-Frontier)
+   - [Monte Carlo](#Monte-Carlo)
+ - [Examples](#Examples)
+   - [Building a portfolio with data from web](#Building-a-portfolio-with-data-from-web)
+   - [Building a portfolio with preset data](#Building-a-portfolio-with-preset-data)
+   - [Analysis of a portfolio](#Analysis-of-a-portfolio)
+   - [Optimisation of a portfolio](#Optimisation-of-a-portfolio)
+
+## Motivation
+Within a few lines of code, *FinQuant* can generate an object that holds your stock prices of your desired financial portfolio, analyses it, and can create plots of different kinds of *Returns*, *Moving Averages*, *Moving Average Bands with buy/sell signals*, and *Bollinger Bands*. It also allows for the optimisation based on the *Efficient Frontier* or a *Monte Carlo* run of the financial portfolio within a few lines of code. Some of the results are shown here.
+
+### Automatically generating an instance of `Portfolio`
+`finquant.portfolio.build_portfolio` is a function that eases the creating of your portfolio. See below for one of several ways of using `build_portfolio`.
+```
+from finquant.portfolio import build_portfolio
+names = ['GOOG', 'AMZN', 'MCD', 'DIS']
+start_date = '2015-01-01'
+end_date = '2017-12-31'
+pf = build_portfolio(names=names,
+                    start_date=start_date,
+                    end_date=end_date)
+```
+`pf` is an instance of `finquant.portfolio.Portfolio`, which contains the prices of the stocks in your portfolio. Then...
+```
+pf.data.head(3)
+```
+yields
+```
+              GOOG    AMZN        MCD        DIS
+Date
+2015-01-02  524.81  308.52  85.783317  90.586146
+2015-01-05  513.87  302.19  84.835892  89.262380
+2015-01-06  501.96  295.29  84.992263  88.788916
+```
+
+### Portfolio properties
+Nicely printing out the portfolio's properties
+```
+pf.properties()
+```
+Depending on the stocks within your portfolio, the output looks something like the below.
+```
+----------------------------------------------------------------------
+Stocks: GOOG, AMZN, MCD, DIS
+Time window/frequency: 252
+Risk free rate: 0.005
+Portfolio expected return: 0.266
+Portfolio volatility: 0.156
+Portfolio Sharpe ratio: 1.674
+
+Skewness:
+       GOOG      AMZN      MCD       DIS
+0  0.124184  0.087516  0.58698  0.040569
+
+Kurtosis:
+       GOOG      AMZN       MCD       DIS
+0 -0.751818 -0.856101 -0.602008 -0.892666
+
+Information:
+   Allocation  Name
+0        0.25  GOOG
+1        0.25  AMZN
+2        0.25   MCD
+3        0.25   DIS
+----------------------------------------------------------------------
+```
+
+### Cumulative Return
+```
+pf.comp_cumulative_returns().plot().axhline(y = 0, color = "black", lw = 3)
+```
+yields
+<p align="center">
+  <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/cumulative-return.svg?sanitize=true" width="60%">
+</p>
+
+### Band Moving Average (Buy/Sell Signals)
+```
+from finquant.moving_average import compute_ma, ema
+# get stock data for disney
+dis = pf.get_stock("DIS").data.copy(deep=True)
+spans = [10, 50, 100, 150, 200]
+ma = compute_ma(dis, ema, spans, plot=True)
+```
+yields
+<p align="center">
+  <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ma-band-buysell-signals.svg?sanitize=true" width="60%">
+</p>
+
+### Bollinger Band
+```
+from finquant.moving_average import plot_bollinger_band, sma
+# get stock data for disney
+dis = pf.get_stock("DIS").data.copy(deep=True)
+span=20
+plot_bollinger_band(dis, sma, span)
+```
+yields
+<p align="center">
+  <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/bollinger-band.svg?sanitize=true" width="60%">
+</p>
+
+### Portfolio Optimisation
+```
+# performs and plots results of Monte Carlo run (5000 iterations)
+opt_w, opt_res = pf.mc_optimisation(num_trials=5000)
+# plots the results of the Monte Carlo optimisation
+pf.mc_plot_results()
+# plots the Efficient Frontier
+pf.ef_plot_efrontier()
+# plots optimal portfolios based on Efficient Frontier
+pf.ef.plot_optimal_portfolios()
+# plots individual plots of the portfolio
+pf.plot_stocks()
+```
+<p align="center">
+  <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ef-mc-overlay.svg?sanitize=true" width="60%">
+</p>
+
+## Installation
+As it is common for open-source projects, there are several ways to get hold of the code. Choose whichever suits you and your purposes best.
+
+### Dependencies
+*FinQuant* depends on the following Python packages:
+ - python>=3.10
+ - numpy>=1.15
+ - pandas>=2.0
+ - matplotlib>=3.0
+ - quandl>=3.4.5
+ - yfinance>=0.1.43
+ - scipy>=1.2.0
+
+### From PyPI
+*FinQuant* can be obtained from PyPI
+
+```pip install FinQuant```
+
+### From GitHub
+Get the code from GitHub:
+
+```git clone https://github.com/fmilthaler/FinQuant.git```
+
+Then inside `FinQuant` run:
+
+```python setup.py install```
+
+Alternatively, if you do not wish to install *FinQuant*, you can also download/clone it as stated above, and then make sure to add it to your ``PYTHONPATH``.
+
+## Portfolio Management
+This is the core of *FinQuant*. `finquant.portfolio.Portfolio` provides an object that holds prices of all stocks in your portfolio, and automatically computes the most common quantities for you. To make *FinQuant* an user-friendly program, that combines data analysis, visualisation and optimisation, the object provides interfaces to the main features that are provided in the modules in `./finquant/`.
+
+To learn more about the object, please read through the [documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant Documentation"), docstring of the module/class, and/or have a look at the examples.
+
+`finquant.portfolio.Portfolio` also provides a function `build_portfolio` which is designed to automatically generate an instance of `Portfolio` for the user's convenience. For more information on how to use `build_portfolio`, please refer to the [documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant Documentation"), its `docstring` and/or have a look at the examples.
+
+## Returns
+Daily returns of stocks are often computed in different ways. *FinQuant* provides three different ways of computing the daily returns in `finquant.returns`:
+1. The cumulative return: <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/tex/738645698dc3073b4bb52a0c078ae829.svg?invert_in_darkmode&sanitize=true" align=middle width=194.52263655pt height=46.976899200000005pt/>
+2. Percentage change of daily returns: <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/tex/27215e5f36fd0308b51ab510444edf0d.svg?invert_in_darkmode&sanitize=true" align=middle width=126.07712039999997pt height=48.84266309999997pt/>
+3. Log Return: <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/tex/ef37c00ad58fe657a64041c3093e0640.svg?invert_in_darkmode&sanitize=true" align=middle width=208.3327686pt height=57.53473439999999pt/>
+
+In addition to those, the module provides the function `historical_mean_return(data, freq=252)`, which computes the historical mean of the daily returns over a time period `freq`.
+
+## Moving Averages
+The module `finquant.moving_average` allows the computation and visualisation of Moving Averages of the stocks listed in the portfolio is also provided. It entails functions to compute and visualise the
+ - `sma`: Simple Moving Average, and
+ - `ema`: Exponential Moving Average.
+ - `compute_ma`: a Band of Moving Averages (of different time windows/spans) including Buy/Sell signals
+ - `plot_bollinger_band`: a Bollinger Band for
+   - `sma`,
+   - `ema`.
+
+## Portfolio Optimisation
+### Efficient Frontier
+An implementation of the Efficient Frontier (`finquant.efficient_frontier.EfficientFrontier`) allows for the optimisation of the portfolio for
+ - `minimum_volatility` Minimum Volatility,
+ - `maximum_sharpe_ratio` Maximum Sharpe Ratio
+ - `efficient_return` Minimum Volatility for a given expected return
+ - `efficient_volatility` Maximum Sharpe Ratio for a given target volatility
+
+by performing a numerical solve to minimise/maximise an objective function.
+
+Often it is useful to visualise the *Efficient Frontier* as well as the optimal solution. This can be achieved with the following methods:
+ - `plot_efrontier`: Plots the *Efficient Frontier*. If no minimum/maximum Return values are provided, the algorithm automatically chooses those limits for the *Efficient Frontier* based on the minimum/maximum Return values of all stocks within the given portfolio.
+ - `plot_optimal_portfolios`: Plots markers of the portfolios with the Minimum Volatility and Maximum Sharpe Ratio.
+
+For reasons of user-friendliness, interfaces to these functions are provided in `finquant.portfolio.Portfolio`. Please have a look at the [documentation](https://finquant.readthedocs.io "FinQuant Documentation").
+
+### Monte Carlo
+Alternatively a *Monte Carlo* run of `n` trials can be performed to find the optimal portfolios for
+ - minimum volatility,
+ - maximum Sharpe ratio
+
+The approach branded as *Efficient Frontier* should be the preferred method for reasons of computational effort and accuracy. The latter approach is only included for the sake of completeness, and creation of beautiful plots.
+
+## Examples
+For more information about the project and details on how to use it, please
+look at the examples provided in `./example`.
+
+**Note**: In the below examples, `pf` refers to an instance of `finquant.portfolio.Portfolio`, the object that holds all stock prices and computes its most common quantities automatically. To make *FinQuant* a user-friendly program, that combines data analysis, visualisation and optimisation, the object also provides interfaces to the main features that are provided in the modules in `./finquant/` and are discussed throughout this README.
+
+### Building a portfolio with data from web
+`./example/Example-Build-Portfolio-from-web.py`: Shows how to use *FinQuant* to build a financial portfolio by downloading stock price data through the Python package `quandl`/`yfinance`.
+
+### Building a portfolio with preset data
+`./example/Example-Build-Portfolio-from-file.py`: Shows how to use *FinQuant* to build a financial portfolio by providing stock price data yourself, e.g. by reading data from disk/file.
+
+### Analysis of a portfolio
+`./example/Example-Analysis.py`: This example shows how to use an instance of `finquant.portfolio.Portfolio`, get the portfolio's quantities, such as
+ - Expected Returns,
+ - Volatility,
+ - Sharpe Ratio.
+
+It also shows how to extract individual stocks from the given portfolio. Moreover it shows how to compute and visualise:
+ - the different Returns provided by the module `finquant.returns`,
+ - *Moving Averages*, a band of *Moving Averages*, and a *Bollinger Band*.
+
+### Optimisation of a portfolio
+`./example/Example-Optimisation.py`: This example focusses on the optimisation of a portfolio. To achieve this, the example shows the usage of `finquant.efficient_frontier.EfficientFrontier` for optimising the portfolio, for the
+ - Minimum Volatility
+ - Maximum Sharpe Ratio
+ - Minimum Volatility for a given target Return
+ - Maximum Sharpe Ratio for a given target Volatility.
+
+Furthermore, it is also shown how the entire *Efficient Frontier* and the optimal portfolios can be computed and visualised. If needed, it also gives an example of plotting the individual stocks of the given portfolio within the computed *Efficient Frontier*.
+
+Also, the optimisation of a portfolio and its visualisation based on a *Monte Carlo* is shown.
+
+Finally, *FinQuant*'s visualisation methods allow for overlays, if this is desired. Thus, with only the following few lines of code, one can create an overlay of the *Monte Carlo* run, the *Efficient Frontier*, its optimised portfolios for *Minimum Volatility* and *Maximum Sharpe Ratio*, as well as the portfolio's individual stocks.
+
```

#### html2text {}

```diff
@@ -1,16 +1,27 @@
-Metadata-Version: 2.1 Name: FinQuant Version: 0.2.2 Summary: A program for
+Metadata-Version: 2.1 Name: FinQuant Version: 0.2.3 Summary: A program for
 financial portfolio management, analysis and optimisation Home-page: https://
-github.com/fmilthaler/FinQuant Author: Frank Milthaler Author-email:
-f.milthaler@gmail.com License: MIT Download-URL: https://github.com/fmilthaler/
-FinQuant/archive/v0.2.2.tar.gz Project-URL: Documentation, https://
-finquant.readthedocs.io Description:
+github.com/fmilthaler/FinQuant Download-URL: https://github.com/fmilthaler/
+FinQuant/archive/v0.2.3.tar.gz Author: Frank Milthaler Author-email:
+f.milthaler@gmail.com License: MIT Project-URL: Documentation, https://
+finquant.readthedocs.io Keywords:
+finance,portfolio,investment,numerical,optimisation,monte carlo,efficient
+frontier,quantitative,quant Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Education Classifier: Intended Audience ::
+Financial and Insurance Industry Classifier: Intended Audience :: Other
+Audience Classifier: Intended Audience :: Science/Research Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.10 Description-Content-Type: text/markdown
+Provides-Extra: test Provides-Extra: dev Provides-Extra: docs Provides-Extra:
+publish License-File: LICENSE.txt
 [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-
                                    logo.png]
-    [pypi] [pypi] [travis] [docs] [contributors] [contributions] [license]
+[pypi] [pypi] [GitHub_Actions] [docs] [contributors] [contributions] [license]
 # FinQuant *FinQuant* is a program for financial **portfolio management,
 analysis and optimisation**. This README only gives a brief overview of
 *FinQuant*. The interested reader should refer to its [documentation](https://
 finquant.readthedocs.io "FinQuant Documentation"). ## Table of contents -
 [Motivation](#Motivation) - [Installation](#Installation) - [Portfolio
 Management](#Portfolio-Management) - [Returns](#Returns) - [Moving Averages]
 (#Moving-Averages) - [Portfolio Optimisation](#Portfolio-Optimisation) -
@@ -50,44 +61,44 @@
                      cumulative-return.svg?sanitize=true]
 ### Band Moving Average (Buy/Sell Signals) ``` from finquant.moving_average
 import compute_ma, ema # get stock data for disney dis = pf.get_stock
 ("DIS").data.copy(deep=True) spans = [10, 50, 100, 150, 200] ma = compute_ma
 (dis, ema, spans, plot=True) ``` yields
  [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ma-band-
                       buysell-signals.svg?sanitize=true]
-### Bollinger Band ``` from finquant.moving_average import plot_bollinger_band
-# get stock data for disney dis = pf.get_stock("DIS").data.copy(deep=True)
+### Bollinger Band ``` from finquant.moving_average import plot_bollinger_band,
+sma # get stock data for disney dis = pf.get_stock("DIS").data.copy(deep=True)
 span=20 plot_bollinger_band(dis, sma, span) ``` yields
 [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/bollinger-
                             band.svg?sanitize=true]
 ### Portfolio Optimisation ``` # performs and plots results of Monte Carlo run
 (5000 iterations) opt_w, opt_res = pf.mc_optimisation(num_trials=5000) # plots
 the results of the Monte Carlo optimisation pf.mc_plot_results() # plots the
 Efficient Frontier pf.ef_plot_efrontier() # plots optimal portfolios based on
 Efficient Frontier pf.ef.plot_optimal_portfolios() # plots individual plots of
 the portfolio pf.plot_stocks() ```
   [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ef-mc-
                           overlay.svg?sanitize=true]
 ## Installation As it is common for open-source projects, there are several
 ways to get hold of the code. Choose whichever suits you and your purposes
 best. ### Dependencies *FinQuant* depends on the following Python packages: -
-python>=3.5.0 - numpy>=1.15 - pandas>=0.24 - matplotlib>=1.5.1 - quandl>=3.4.5
-- yfinance>=0.1.43 - scipy>=1.2.0 - pytest>=2.8.7 ### From PyPI *FinQuant* can
-be obtained from PyPI ```pip install FinQuant``` ### From GitHub Get the code
-from GitHub: ```git clone https://github.com/fmilthaler/FinQuant.git``` Then
-inside `FinQuant` run: ```python setup.py install``` Alternatively, if you do
-not wish to install *FinQuant*, you can also download/clone it as stated above,
-and then make sure to add it to your ``PYTHONPATH``. ## Portfolio Management
-This is the core of *FinQuant*. `finquant.portfolio.Portfolio` provides an
-object that holds prices of all stocks in your portfolio, and automatically
-computes the most common quantities for you. To make *FinQuant* an user-
-friendly program, that combines data analysis, visualisation and optimisation,
-the object provides interfaces to the main features that are provided in the
-modules in `./finquant/`. To learn more about the object, please read through
-the [documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant
+python>=3.10 - numpy>=1.15 - pandas>=2.0 - matplotlib>=3.0 - quandl>=3.4.5 -
+yfinance>=0.1.43 - scipy>=1.2.0 ### From PyPI *FinQuant* can be obtained from
+PyPI ```pip install FinQuant``` ### From GitHub Get the code from GitHub:
+```git clone https://github.com/fmilthaler/FinQuant.git``` Then inside
+`FinQuant` run: ```python setup.py install``` Alternatively, if you do not wish
+to install *FinQuant*, you can also download/clone it as stated above, and then
+make sure to add it to your ``PYTHONPATH``. ## Portfolio Management This is the
+core of *FinQuant*. `finquant.portfolio.Portfolio` provides an object that
+holds prices of all stocks in your portfolio, and automatically computes the
+most common quantities for you. To make *FinQuant* an user-friendly program,
+that combines data analysis, visualisation and optimisation, the object
+provides interfaces to the main features that are provided in the modules in
+`./finquant/`. To learn more about the object, please read through the
+[documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant
 Documentation"), docstring of the module/class, and/or have a look at the
 examples. `finquant.portfolio.Portfolio` also provides a function
 `build_portfolio` which is designed to automatically generate an instance of
 `Portfolio` for the user's convenience. For more information on how to use
 `build_portfolio`, please refer to the [documentation](https://
 finquant.readthedocs.io/en/latest/ "FinQuant Documentation"), its `docstring`
 and/or have a look at the examples. ## Returns Daily returns of stocks are
@@ -161,17 +172,8 @@
 example of plotting the individual stocks of the given portfolio within the
 computed *Efficient Frontier*. Also, the optimisation of a portfolio and its
 visualisation based on a *Monte Carlo* is shown. Finally, *FinQuant*'s
 visualisation methods allow for overlays, if this is desired. Thus, with only
 the following few lines of code, one can create an overlay of the *Monte Carlo*
 run, the *Efficient Frontier*, its optimised portfolios for *Minimum
 Volatility* and *Maximum Sharpe Ratio*, as well as the portfolio's individual
-stocks. Keywords: finance,portfolio,investment,numerical,optimisation,monte
-carlo,efficient frontier,quantitative,quant Platform: UNKNOWN Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Financial and Insurance Industry Classifier:
-Intended Audience :: Other Audience Classifier: Intended Audience :: Science/
-Research Classifier: Programming Language :: Python :: 3 :: Only Classifier:
-Programming Language :: Python :: 3.5 Classifier: Programming Language ::
-Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.5 Description-Content-Type: text/markdown
+stocks.
```

### Comparing `FinQuant-0.2.2/README.md` & `FinQuant-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-logo.png" width="45%">
 </p>
 
 <p align="center">
   <a href="https://GitHub.com/fmilthaler/FinQuant/stargazers/">
-    <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star&maxAge=2592000" alt='pypi'>
+    <img src="https://img.shields.io/github/stars/fmilthaler/FinQuant.svg?style=social&label=Star" alt='pypi'>
   </a>
   <a href="https://pypi.org/project/FinQuant">
     <img src="https://img.shields.io/badge/pypi-v0.2.2-brightgreen.svg?style=popout" alt='pypi'>
   </a>
-  <a href="https://travis-ci.org/fmilthaler/FinQuant">
-    <img src="https://travis-ci.org/fmilthaler/FinQuant.svg?style=popout?branch=master" alt='travis'>
+  <a href="https://github.com/fmilthaler/FinQuant">
+    <img src="https://github.com/fmilthaler/finquant/actions/workflows/pytest.yml/badge.svg?branch=master" alt='GitHub Actions'>
   </a>
   <a href="http://finquant.readthedocs.io/">
     <img src="https://img.shields.io/readthedocs/finquant.svg?style=popout" alt="docs">
   </a>
   <a href="https://GitHub.com/fmilthaler/FinQuant/graphs/contributors/">
     <img src="https://img.shields.io/github/contributors/fmilthaler/FinQuant.svg?style=popout" alt="contributors">
   </a>
@@ -125,15 +125,15 @@
 yields
 <p align="center">
   <img src="https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ma-band-buysell-signals.svg?sanitize=true" width="60%">
 </p>
 
 ### Bollinger Band
 ```
-from finquant.moving_average import plot_bollinger_band
+from finquant.moving_average import plot_bollinger_band, sma
 # get stock data for disney
 dis = pf.get_stock("DIS").data.copy(deep=True)
 span=20
 plot_bollinger_band(dis, sma, span)
 ```
 yields
 <p align="center">
@@ -158,22 +158,21 @@
 </p>
 
 ## Installation
 As it is common for open-source projects, there are several ways to get hold of the code. Choose whichever suits you and your purposes best.
 
 ### Dependencies
 *FinQuant* depends on the following Python packages:
- - python>=3.5.0
+ - python>=3.10
  - numpy>=1.15
- - pandas>=0.24
- - matplotlib>=1.5.1
+ - pandas>=2.0
+ - matplotlib>=3.0
  - quandl>=3.4.5
  - yfinance>=0.1.43
  - scipy>=1.2.0
- - pytest>=2.8.7
 
 ### From PyPI
 *FinQuant* can be obtained from PyPI
 
 ```pip install FinQuant```
 
 ### From GitHub
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/finquant-
                                    logo.png]
-    [pypi] [pypi] [travis] [docs] [contributors] [contributions] [license]
+[pypi] [pypi] [GitHub_Actions] [docs] [contributors] [contributions] [license]
 # FinQuant *FinQuant* is a program for financial **portfolio management,
 analysis and optimisation**. This README only gives a brief overview of
 *FinQuant*. The interested reader should refer to its [documentation](https://
 finquant.readthedocs.io "FinQuant Documentation"). ## Table of contents -
 [Motivation](#Motivation) - [Installation](#Installation) - [Portfolio
 Management](#Portfolio-Management) - [Returns](#Returns) - [Moving Averages]
 (#Moving-Averages) - [Portfolio Optimisation](#Portfolio-Optimisation) -
@@ -44,44 +44,44 @@
                      cumulative-return.svg?sanitize=true]
 ### Band Moving Average (Buy/Sell Signals) ``` from finquant.moving_average
 import compute_ma, ema # get stock data for disney dis = pf.get_stock
 ("DIS").data.copy(deep=True) spans = [10, 50, 100, 150, 200] ma = compute_ma
 (dis, ema, spans, plot=True) ``` yields
  [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ma-band-
                       buysell-signals.svg?sanitize=true]
-### Bollinger Band ``` from finquant.moving_average import plot_bollinger_band
-# get stock data for disney dis = pf.get_stock("DIS").data.copy(deep=True)
+### Bollinger Band ``` from finquant.moving_average import plot_bollinger_band,
+sma # get stock data for disney dis = pf.get_stock("DIS").data.copy(deep=True)
 span=20 plot_bollinger_band(dis, sma, span) ``` yields
 [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/bollinger-
                             band.svg?sanitize=true]
 ### Portfolio Optimisation ``` # performs and plots results of Monte Carlo run
 (5000 iterations) opt_w, opt_res = pf.mc_optimisation(num_trials=5000) # plots
 the results of the Monte Carlo optimisation pf.mc_plot_results() # plots the
 Efficient Frontier pf.ef_plot_efrontier() # plots optimal portfolios based on
 Efficient Frontier pf.ef.plot_optimal_portfolios() # plots individual plots of
 the portfolio pf.plot_stocks() ```
   [https://raw.githubusercontent.com/fmilthaler/finquant/master/images/ef-mc-
                           overlay.svg?sanitize=true]
 ## Installation As it is common for open-source projects, there are several
 ways to get hold of the code. Choose whichever suits you and your purposes
 best. ### Dependencies *FinQuant* depends on the following Python packages: -
-python>=3.5.0 - numpy>=1.15 - pandas>=0.24 - matplotlib>=1.5.1 - quandl>=3.4.5
-- yfinance>=0.1.43 - scipy>=1.2.0 - pytest>=2.8.7 ### From PyPI *FinQuant* can
-be obtained from PyPI ```pip install FinQuant``` ### From GitHub Get the code
-from GitHub: ```git clone https://github.com/fmilthaler/FinQuant.git``` Then
-inside `FinQuant` run: ```python setup.py install``` Alternatively, if you do
-not wish to install *FinQuant*, you can also download/clone it as stated above,
-and then make sure to add it to your ``PYTHONPATH``. ## Portfolio Management
-This is the core of *FinQuant*. `finquant.portfolio.Portfolio` provides an
-object that holds prices of all stocks in your portfolio, and automatically
-computes the most common quantities for you. To make *FinQuant* an user-
-friendly program, that combines data analysis, visualisation and optimisation,
-the object provides interfaces to the main features that are provided in the
-modules in `./finquant/`. To learn more about the object, please read through
-the [documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant
+python>=3.10 - numpy>=1.15 - pandas>=2.0 - matplotlib>=3.0 - quandl>=3.4.5 -
+yfinance>=0.1.43 - scipy>=1.2.0 ### From PyPI *FinQuant* can be obtained from
+PyPI ```pip install FinQuant``` ### From GitHub Get the code from GitHub:
+```git clone https://github.com/fmilthaler/FinQuant.git``` Then inside
+`FinQuant` run: ```python setup.py install``` Alternatively, if you do not wish
+to install *FinQuant*, you can also download/clone it as stated above, and then
+make sure to add it to your ``PYTHONPATH``. ## Portfolio Management This is the
+core of *FinQuant*. `finquant.portfolio.Portfolio` provides an object that
+holds prices of all stocks in your portfolio, and automatically computes the
+most common quantities for you. To make *FinQuant* an user-friendly program,
+that combines data analysis, visualisation and optimisation, the object
+provides interfaces to the main features that are provided in the modules in
+`./finquant/`. To learn more about the object, please read through the
+[documentation](https://finquant.readthedocs.io/en/latest/ "FinQuant
 Documentation"), docstring of the module/class, and/or have a look at the
 examples. `finquant.portfolio.Portfolio` also provides a function
 `build_portfolio` which is designed to automatically generate an instance of
 `Portfolio` for the user's convenience. For more information on how to use
 `build_portfolio`, please refer to the [documentation](https://
 finquant.readthedocs.io/en/latest/ "FinQuant Documentation"), its `docstring`
 and/or have a look at the examples. ## Returns Daily returns of stocks are
```

### Comparing `FinQuant-0.2.2/finquant/efficient_frontier.py` & `FinQuant-0.2.3/finquant/efficient_frontier.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.2.2/finquant/minimise_fun.py` & `FinQuant-0.2.3/finquant/minimise_fun.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 """
 
 
 from finquant.quants import annualised_portfolio_quantities
 
 
 def portfolio_volatility(weights, mean_returns, cov_matrix):
-    """Calculates the negative Sharpe ratio of a portfolio
+    """Calculates the volatility a portfolio
 
     :Input:
      :weights: numpy.ndarray, weights of the stocks in the portfolio
      :mean_returns: pandas.Series, individual expected returns for all stocks
          in the portfolio
      :cov_matrix: pandas.DataFrame, covariance matrix of returns
-     :risk_free_rate: Float (default=0.005), risk free rate
 
     Output:
      :volatility: annualised volatility
     """
     return annualised_portfolio_quantities(weights, mean_returns, cov_matrix)[1]
```

### Comparing `FinQuant-0.2.2/finquant/monte_carlo.py` & `FinQuant-0.2.3/finquant/monte_carlo.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         :Output:
          :result: List of quantities returned from `fun` at each iteration.
         """
         result = []
         for i in range(self.num_trials):
             res = fun(**kwargs)
             result.append(res)
-        return np.asarray(result)
+        return np.asarray(result, dtype=object)
 
 
 class MonteCarloOpt(MonteCarlo):
     """An object to perform a Monte Carlo run/simulation for finding
     optimised financial portfolios.
 
     Inherits from `MonteCarlo`.
```

### Comparing `FinQuant-0.2.2/finquant/moving_average.py` & `FinQuant-0.2.3/finquant/moving_average.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.2.2/finquant/portfolio.py` & `FinQuant-0.2.3/finquant/portfolio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """This module is the **core** of `FinQuant`. It provides
 
-- a public class ``Stock`` that holds and calculates quantities of a single stock,
 - a public class ``Portfolio`` that holds and calculates quantities of a financial
-  portfolio, which is a collection of Stock instances.
+  portfolio, which is a collection of ``Stock`` instances (the ``Stock`` class is provided in ``finquant.stock``).
 - a public function ``build_portfolio()`` that automatically constructs and returns
-  an instance of ``Portfolio`` and instances of ``Stock``. The relevant stock
-  data is either retrieved through `quandl`/`yfinance` or provided by the user as a
+  an instance of ``Portfolio`` and instances of ``Stock``. 
+  The relevant stock data is either retrieved through `quandl`/`yfinance` or provided by the user as a
   ``pandas.DataFrame`` (after loading it manually from disk/reading from file).
   For an example on how to use it, please read the corresponding docstring,
   or have a look at the examples in the sub-directory ``example``.
 
-The classes ``Stock`` and ``Portfolio`` are designed to easily manage your
-financial portfolio, and make the most common quantitative calculations, such as:
+The class ``Portfolio`` is designed to easily manage your financial portfolio, 
+and makes the most common quantitative calculations, such as:
 
 - cumulative returns of the portfolio's stocks
 - daily returns of the portfolio's stocks (daily percentage change),
 - daily log returns of the portfolio's stocks,
 - Expected (annualised) Return,
 - Volatility,
 - Sharpe Ratio,
@@ -51,124 +50,21 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pylab as plt
 from finquant.quants import weighted_mean, weighted_std, sharpe_ratio
 from finquant.returns import historical_mean_return
 from finquant.returns import daily_returns, cumulative_returns
 from finquant.returns import daily_log_returns
+from finquant.stock import Stock
 from finquant.efficient_frontier import EfficientFrontier
 from finquant.monte_carlo import MonteCarloOpt
 
 
-class Stock(object):
-    """Object that contains information about a stock/fund.
-    To initialise the object, it requires a name, information about
-    the stock/fund given as one of the following data structures:
-
-    - ``pandas.Series``
-    - ``pandas.DataFrame``
-
-    The investment information can contain as little information as its name,
-    and the amount invested in it, the column labels must be ``Name`` and ``Allocation``
-    respectively, but it can also contain more information, such as
-
-    - Year
-    - Strategy
-    - CCY
-    - etc.
-
-    It also requires either data, e.g. daily closing prices as a
-    ``pandas.DataFrame`` or ``pandas.Series``.
-    ``data`` must be given as a ``pandas.DataFrame``, and at least one data column
-    is required to containing the closing price, hence it is required to
-    contain one column label ``<stock_name> - Adj. Close`` which is used to
-    compute the return of investment. However, ``data`` can contain more
-    data in additional columns.
-    """
-
-    def __init__(self, investmentinfo, data):
-        """
-        :Input:
-         :investmentinfo: ``pandas.DataFrame`` of investment information
-         :data: ``pandas.DataFrame`` of stock price
-        """
-        self.name = investmentinfo.Name
-        self.investmentinfo = investmentinfo
-        self.data = data
-        # compute expected return and volatility of stock
-        self.expected_return = self.comp_expected_return()
-        self.volatility = self.comp_volatility()
-        self.skew = self._comp_skew()
-        self.kurtosis = self._comp_kurtosis()
-
-    # functions to compute quantities
-    def comp_daily_returns(self):
-        """Computes the daily returns (percentage change).
-        See ``finquant.returns.daily_returns``.
-        """
-        return daily_returns(self.data)
-
-    def comp_expected_return(self, freq=252):
-        """Computes the Expected Return of the stock.
-
-        :Input:
-         :freq: ``int`` (default: ``252``), number of trading days, default
-             value corresponds to trading days in a year
-
-        :Output:
-         :expected_return: Expected Return of stock.
-        """
-        return historical_mean_return(self.data, freq=freq)
-
-    def comp_volatility(self, freq=252):
-        """Computes the Volatility of the stock.
-
-        :Input:
-         :freq: ``int`` (default: ``252``), number of trading days, default
-             value corresponds to trading days in a year
-
-        :Output:
-         :volatility: Volatility of stock.
-        """
-        return self.comp_daily_returns().std() * np.sqrt(freq)
-
-    def _comp_skew(self):
-        """Computes and returns the skewness of the stock."""
-        return self.data.skew().values[0]
-
-    def _comp_kurtosis(self):
-        """Computes and returns the Kurtosis of the stock."""
-        return self.data.kurt().values[0]
-
-    def properties(self):
-        """Nicely prints out the properties of the stock: Expected Return,
-        Volatility, Skewness, Kurtosis as well as the ``Allocation`` (and other
-        information provided in investmentinfo.)
-        """
-        # nicely printing out information and quantities of the stock
-        string = "-" * 50
-        string += "\nStock: {}".format(self.name)
-        string += "\nExpected Return:{:0.3f}".format(self.expected_return.values[0])
-        string += "\nVolatility: {:0.3f}".format(self.volatility.values[0])
-        string += "\nSkewness: {:0.5f}".format(self.skew)
-        string += "\nKurtosis: {:0.5f}".format(self.kurtosis)
-        string += "\nInformation:"
-        string += "\n" + str(self.investmentinfo.to_frame().transpose())
-        string += "\n"
-        string += "-" * 50
-        print(string)
-
-    def __str__(self):
-        # print short description
-        string = "Contains information about " + str(self.name) + "."
-        return string
-
-
 class Portfolio(object):
-    """Object that contains information about a investment portfolio.
+    """Object that contains information about an investment portfolio.
     To initialise the object, it does not require any input.
     To fill the portfolio with investment information, the
     function ``add_stock(stock)`` should be used, in which ``stock`` is
     an object of ``Stock``.
     """
 
     def __init__(self):
@@ -194,15 +90,15 @@
     def totalinvestment(self):
         return self.__totalinvestment
 
     @totalinvestment.setter
     def totalinvestment(self, val):
         if val is not None:
             # treat "None" as initialisation
-            if not isinstance(val, (float, int)):
+            if not isinstance(val, (float, int, np.floating, np.integer)):
                 raise ValueError("Total investment must be a float or integer.")
             elif val <= 0:
                 raise ValueError(
                     "The money to be invested in the portfolio must be > 0."
                 )
             else:
                 self.__totalinvestment = val
@@ -253,15 +149,17 @@
 
         :Input:
          :stock: an object of ``Stock``
         """
         # adding stock to dictionary containing all stocks provided
         self.stocks.update({stock.name: stock})
         # adding information of stock to the portfolio
-        self.portfolio = self.portfolio.append(stock.investmentinfo, ignore_index=True)
+        self.portfolio = pd.concat(
+            [self.portfolio, stock.investmentinfo.to_frame().T], ignore_index=True
+        )
         # setting an appropriate name for the portfolio
         self.portfolio.name = "Allocation of stocks"
         # also add stock data of stock to the dataframe
         self._add_stock_data(stock.data)
 
         # update quantities of portfolio
         self._update()
@@ -677,15 +575,14 @@
             plt.annotate(
                 txt,
                 (stock_volatility[i], stock_returns[i]),
                 xytext=(10, 0),
                 textcoords="offset points",
                 label=i,
             )
-            plt.legend()
 
     def properties(self):
         """Nicely prints out the properties of the portfolio:
 
         - Expected Return,
         - Volatility,
         - Sharpe Ratio,
```

### Comparing `FinQuant-0.2.2/finquant/quants.py` & `FinQuant-0.2.3/finquant/quants.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.2.2/finquant/returns.py` & `FinQuant-0.2.3/finquant/returns.py`

 * *Files identical despite different names*

### Comparing `FinQuant-0.2.2/setup.py` & `FinQuant-0.2.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,66 @@
 import setuptools
 
 # get version/release from file
 with open("version", "r") as f:
-    ver = dict(x.rstrip().split("=") for x in f)
+    version = dict(x.rstrip().split("=") for x in f)
 
+# get long description from README
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+# get dependencies
+def read_requirements(file_path):
+    with open(file_path, "r") as f:
+        return [line.strip() for line in f if line.strip()]
+
+install_requires = read_requirements("requirements.txt")
+
+extras_require = {
+    "test": read_requirements("requirements_test.txt"),
+    "dev": read_requirements("requirements_dev.txt"),
+    "docs": read_requirements("requirements_docs.txt"),
+    "publish": read_requirements("requirements_publish.txt"),
+}
+
 setuptools.setup(
     name="FinQuant",
-    version=ver["version"],
+    version=version["version"],
     author="Frank Milthaler",
     author_email="f.milthaler@gmail.com",
     description="A program for financial portfolio management, analysis and optimisation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fmilthaler/FinQuant",
     download_url="https://github.com/fmilthaler/FinQuant/archive/v{}.tar.gz".format(
-        ver["release"]
+        version["release"]
     ),
     license="MIT",
     packages=setuptools.find_packages(),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Education",
         "Intended Audience :: Financial and Insurance Industry",
         "Intended Audience :: Other Audience",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords=[
         "finance",
         "portfolio",
         "investment",
         "numerical",
         "optimisation",
         "monte carlo",
         "efficient frontier",
         "quantitative",
         "quant",
     ],
-    python_requires=">=3.5",
-    install_requires=[
-        "quandl",
-        "yfinance",
-        "numpy",
-        "pandas",
-        "scipy",
-        "matplotlib",
-        "pytest",
-    ],
+    python_requires=">=3.10",
+    install_requires=install_requires,
+    extras_require=extras_require,
     project_urls={"Documentation": "https://finquant.readthedocs.io"},
 )
```

