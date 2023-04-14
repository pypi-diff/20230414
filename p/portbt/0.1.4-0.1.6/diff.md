# Comparing `tmp/portbt-0.1.4.tar.gz` & `tmp/portbt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portbt-0.1.4.tar", max compression
+gzip compressed data, was "portbt-0.1.6.tar", max compression
```

## Comparing `portbt-0.1.4.tar` & `portbt-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 portbt-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0      127 2023-04-12 00:16:50.304309 portbt-0.1.4/portbt/__init__.py
--rw-r--r--   0        0        0     3139 2023-04-12 03:01:01.868034 portbt-0.1.4/portbt/backtest_functions.py
--rw-r--r--   0        0        0     1663 2023-04-12 03:03:15.656462 portbt-0.1.4/portbt/portfolio.py
--rw-r--r--   0        0        0      658 2023-04-11 22:15:59.356410 portbt-0.1.4/portbt/utils.py
--rw-r--r--   0        0        0      575 2023-04-12 03:09:55.339039 portbt-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3755 2023-04-12 03:09:19.187519 portbt-0.1.4/README.md
--rw-r--r--   0        0        0     4368 1970-01-01 00:00:00.000000 portbt-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 portbt-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0      127 2023-04-12 00:16:50.304309 portbt-0.1.6/portbt/__init__.py
+-rw-r--r--   0        0        0     3631 2023-04-14 19:52:14.229468 portbt-0.1.6/portbt/backtest_functions.py
+-rw-r--r--   0        0        0     2517 2023-04-14 20:04:37.261364 portbt-0.1.6/portbt/portfolio.py
+-rw-r--r--   0        0        0      656 2023-04-14 19:38:38.483240 portbt-0.1.6/portbt/utils.py
+-rw-r--r--   0        0        0      575 2023-04-14 19:55:57.799795 portbt-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4417 2023-04-14 20:04:30.388418 portbt-0.1.6/README.md
+-rw-r--r--   0        0        0     5014 1970-01-01 00:00:00.000000 portbt-0.1.6/PKG-INFO
```

### Comparing `portbt-0.1.4/LICENSE.txt` & `portbt-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `portbt-0.1.4/portbt/backtest_functions.py` & `portbt-0.1.6/portbt/backtest_functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,35 @@
 import pandas as pd
 
 from pandas import DataFrame
 
 from .utils import get_rebalance_dates
 
+def validate_weights(weights):
+    if isinstance(weights, dict):
+        if len(weights) == 0:
+            raise ValueError('Dict for the weights has zero length.')
+    
+        if sum(weights.values()) > 1:
+            raise ValueError('Dict for the weights has sum more than 1.')
+        
+        if sum(weights.values()) < 1:
+            raise ValueError('Dict for the weights has sum less than 1.')
+    
+    if isinstance(weights, str) and weights not in ["ew"]:
+        raise ValueError(f"""Not a valid string value for weights parameter: {weights}.
+                         If it isn't a dict, it has to be 'ew' (equal weight)""")
+
+def backtest_without_rebalance(
+    prices,
+    start_weights: dict | str = "ew"
+    ) -> dict:
+
+    validate_weights(start_weights)
 
-def backtest_without_rebalance(prices, start_weights: dict | str = "ew"):
     if start_weights == "ew":
         values = prices.pct_change().fillna(0).add(1).cumprod()
         backtest_result = values.sum(axis=1).pct_change().fillna(0).add(1).cumprod()
 
     if isinstance(start_weights, dict):
         tickers = prices.columns.to_list()
 
@@ -24,44 +44,43 @@
     backtest_result.index.name = "date"
     backtest_result.columns = ["backtest"]
 
     total_value = values.sum(axis=1)
     exposure = values.apply(lambda row: row / total_value.loc[row.name], axis=1)
 
     backtest = {
+        "prices": prices,
         "values": values,
         "exposure": exposure,
         "result": backtest_result,
         "all_dates": backtest_result.index.to_list(),
         "rebal_dates": [],
     }
 
     return backtest
 
 
 def backtest_with_rebalance(
     prices: DataFrame,
     rebal_weights: dict | str,
     rebal_freq: str = "1M",
-) -> dict:
+    ) -> dict:
+
+    validate_weights(rebal_weights)
+
     tickers = prices.columns.to_list()
     n_tickers = len(prices.columns)
     returns = prices.pct_change().fillna(0)
     all_dates = prices.index.to_list()
     rebal_dates = get_rebalance_dates(all_dates, rebal_freq)
 
     if rebal_weights == "ew":
         weights = pd.Series(index=tickers).fillna(1 / n_tickers).to_dict()
 
-    if isinstance(rebal_weights, str) and rebal_weights not in ["ew"]:
-        raise ValueError(f"Not a valid string value for 'rebal_weights': {rebal_weights}")
-
     if isinstance(rebal_weights, dict):
-        if len(rebal_weights) == 0:
-            raise ValueError(f'Dict "rebal_weights" has zero length. Please enter a valid dictionary (length > 0).')   
         weights = rebal_weights.copy()          
 
     values = pd.DataFrame()
     for i, date in enumerate(all_dates):
         for ticker in tickers:
             if i == 0:
                 values.loc[date, ticker] = 1
@@ -75,14 +94,15 @@
     exposure = values.apply(lambda row: row / total_value.loc[row.name], axis=1)
 
     backtest_result = pd.DataFrame(total_value).pct_change().fillna(0).add(1).cumprod()
     backtest_result.index.name = "date"
     backtest_result.columns = ["backtest"]
 
     backtest = {
+        "prices": prices,
         "values": values,
         "exposure": exposure,
         "result": backtest_result,
         "all_dates": all_dates,
         "rebal_dates": rebal_dates,
     }
```

### Comparing `portbt-0.1.4/portbt/utils.py` & `portbt-0.1.6/portbt/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 
 def get_rebalance_dates(all_dates, freq):
     _rebal_dates = pd.DataFrame(index=all_dates, columns=["0"]).resample(freq).last().index
     aux = pd.DataFrame(index=_rebal_dates, columns=[0]).fillna(1)
     aux_daily = pd.concat([aux, pd.DataFrame(index=all_dates)], axis=1).shift(1)
     aux_daily.iloc[0] = 1  # start
     rebal_dates = aux_daily.dropna().index.to_list()
-    return rebal_dates
+    return rebal_dates
```

### Comparing `portbt-0.1.4/pyproject.toml` & `portbt-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "portbt"
-version = "0.1.4"
+version = "0.1.6"
 description = "Python library designed to make portfolio backtesting easy and intuitive"
 authors = ["renanmoretto <himynameisrenan@outlook.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/renanmoretto/portbt"
 
 [tool.poetry.dependencies]
```

### Comparing `portbt-0.1.4/README.md` & `portbt-0.1.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -40,16 +40,17 @@
 2023-04-10  39.040001  98.660004  24.670000  24.510000  86.349998  78.230003
 ```
 ---
 ## Creating the portfolio and backtesting
 ```python
 portfolio = pbt.Portfolio(prices)
 
-backtest = portfolio.run_backtest_without_rebalance()
+backtest = portfolio.run_backtest(rebalance=False)
 
+# backtest.prices -> prices for each asset, "raw data"
 # backtest.values -> values for each asset (starting capital = 1)
 # backtest.exposure -> exposure for each asset
 # backtest.result -> backtest result, starting from 1
 # backtest.all_dates -> all dates for the backtesting, if needed
 # backtest.rebal_dates -> rebalace dates only
 
 # example
@@ -68,22 +69,37 @@
 2023-04-03  0.253178  0.102909  0.141708  0.130782  0.139475  0.231949
 2023-04-04  0.257288  0.103096  0.144492  0.129566  0.140236  0.225321
 2023-04-05  0.258185  0.102898  0.145396  0.130913  0.139037  0.223571
 2023-04-06  0.258177  0.103195  0.145399  0.129457  0.139871  0.223901
 2023-04-10  0.255589  0.103228  0.145400  0.130815  0.139155  0.225814
 ```
 
-## Portfolio functions
+## Portfolio backtesting - main function
 ```
-Portfolio.backtest_with_rebalance() -> Backtest
-    Optional parameters:
-        rebal_weights: dict | str,
-        rebal_freq: str,
-
-Portfolio.backtest_without_rebalance() -> Backtest
-    Optional parameters:
-        start_weights: dict | str,
+Portfolio.run_backtest() -> Backtest
+
+    Parameters:
+
+        - rebalance: bool (required)
+            If 'True', the backtest will rebalance itself.
+
+        - weights: str or dict, default 'ew'
+            If 'dict', than it is the weight for each asset (number between 0 and 1),
+            The sum can't be different than one.
+            Example:
+                asset_weights = {
+                    'asset1': 0.3,
+                    'asset2': 0.2,
+                    'asset3': 0.5,
+                }
+            If str (has to be 'ew'), runs the backtest using equal weight for all 
+            assets (1 / number of assets).
+
+        - rebal_freq: str, default '1M'
+            Rebalance frequency. Has the same valid inputs as pandas.DataFrame.resample() 
+            function.
 ```
 
 ## TODO
 - Performance metrics and visualizations
-- Reports
+- Reports
+- Yahoo Finance implementation
```

### Comparing `portbt-0.1.4/PKG-INFO` & `portbt-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portbt
-Version: 0.1.4
+Version: 0.1.6
 Summary: Python library designed to make portfolio backtesting easy and intuitive
 Home-page: https://github.com/renanmoretto/portbt
 License: MIT
 Author: renanmoretto
 Author-email: himynameisrenan@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -59,16 +59,17 @@
 2023-04-10  39.040001  98.660004  24.670000  24.510000  86.349998  78.230003
 ```
 ---
 ## Creating the portfolio and backtesting
 ```python
 portfolio = pbt.Portfolio(prices)
 
-backtest = portfolio.run_backtest_without_rebalance()
+backtest = portfolio.run_backtest(rebalance=False)
 
+# backtest.prices -> prices for each asset, "raw data"
 # backtest.values -> values for each asset (starting capital = 1)
 # backtest.exposure -> exposure for each asset
 # backtest.result -> backtest result, starting from 1
 # backtest.all_dates -> all dates for the backtesting, if needed
 # backtest.rebal_dates -> rebalace dates only
 
 # example
@@ -87,22 +88,37 @@
 2023-04-03  0.253178  0.102909  0.141708  0.130782  0.139475  0.231949
 2023-04-04  0.257288  0.103096  0.144492  0.129566  0.140236  0.225321
 2023-04-05  0.258185  0.102898  0.145396  0.130913  0.139037  0.223571
 2023-04-06  0.258177  0.103195  0.145399  0.129457  0.139871  0.223901
 2023-04-10  0.255589  0.103228  0.145400  0.130815  0.139155  0.225814
 ```
 
-## Portfolio functions
+## Portfolio backtesting - main function
 ```
-Portfolio.backtest_with_rebalance() -> Backtest
-    Optional parameters:
-        rebal_weights: dict | str,
-        rebal_freq: str,
-
-Portfolio.backtest_without_rebalance() -> Backtest
-    Optional parameters:
-        start_weights: dict | str,
+Portfolio.run_backtest() -> Backtest
+
+    Parameters:
+
+        - rebalance: bool (required)
+            If 'True', the backtest will rebalance itself.
+
+        - weights: str or dict, default 'ew'
+            If 'dict', than it is the weight for each asset (number between 0 and 1),
+            The sum can't be different than one.
+            Example:
+                asset_weights = {
+                    'asset1': 0.3,
+                    'asset2': 0.2,
+                    'asset3': 0.5,
+                }
+            If str (has to be 'ew'), runs the backtest using equal weight for all 
+            assets (1 / number of assets).
+
+        - rebal_freq: str, default '1M'
+            Rebalance frequency. Has the same valid inputs as pandas.DataFrame.resample() 
+            function.
 ```
 
 ## TODO
 - Performance metrics and visualizations
 - Reports
+- Yahoo Finance implementation
```

