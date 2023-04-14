# Comparing `tmp/binance_historical_data-0.1.8.tar.gz` & `tmp/binance_historical_data-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance_historical_data-0.1.8.tar", max compression
+gzip compressed data, was "binance_historical_data-0.1.9.tar", max compression
```

## Comparing `binance_historical_data-0.1.8.tar` & `binance_historical_data-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1095 2022-02-16 18:24:10.000000 binance_historical_data-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0      520 2022-05-25 05:44:42.828639 binance_historical_data-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     7173 2022-05-25 05:26:03.122672 binance_historical_data-0.1.8/README.rst
--rw-r--r--   0        0        0      370 2022-02-23 19:13:56.000000 binance_historical_data-0.1.8/src/binance_historical_data/__init__.py
--rw-r--r--   0        0        0    21872 2022-05-25 05:44:36.452020 binance_historical_data-0.1.8/src/binance_historical_data/data_dumper.py
--rw-r--r--   0        0        0     4695 2022-02-11 17:48:50.000000 binance_historical_data-0.1.8/src/binance_historical_data/logger.py
--rw-r--r--   0        0        0     7983 2022-05-25 05:45:17.277601 binance_historical_data-0.1.8/setup.py
--rw-r--r--   0        0        0     7754 2022-05-25 05:45:17.278602 binance_historical_data-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1095 2022-02-16 18:24:10.000000 binance_historical_data-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0      520 2022-06-03 14:09:06.594617 binance_historical_data-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     7173 2022-05-25 05:26:03.122672 binance_historical_data-0.1.9/README.rst
+-rw-r--r--   0        0        0      370 2022-02-23 19:13:56.000000 binance_historical_data-0.1.9/src/binance_historical_data/__init__.py
+-rw-r--r--   0        0        0    21959 2022-06-03 14:54:14.399594 binance_historical_data-0.1.9/src/binance_historical_data/data_dumper.py
+-rw-r--r--   0        0        0     4695 2022-02-11 17:48:50.000000 binance_historical_data-0.1.9/src/binance_historical_data/logger.py
+-rw-r--r--   0        0        0     7983 2022-06-03 14:58:54.222396 binance_historical_data-0.1.9/setup.py
+-rw-r--r--   0        0        0     7754 2022-06-03 14:58:54.222396 binance_historical_data-0.1.9/PKG-INFO
```

### Comparing `binance_historical_data-0.1.8/LICENSE.txt` & `binance_historical_data-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `binance_historical_data-0.1.8/pyproject.toml` & `binance_historical_data-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "binance_historical_data"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["stanislav <stas.prokopiev@gmail.com>"]
 readme = "README.rst"
 license="MIT"
 repository = "https://github.com/stas-prokopiev/binance_historical_data"
 
 [tool.poetry.dependencies]
```

### Comparing `binance_historical_data-0.1.8/README.rst` & `binance_historical_data-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `binance_historical_data-0.1.8/src/binance_historical_data/data_dumper.py` & `binance_historical_data-0.1.9/src/binance_historical_data/data_dumper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Module with class to download candle historical data from binance"""
 # Standard library imports
 import os
-from typing import Optional, Any, Union
+# from typing import Optional, Any, Union
 import urllib.request
 import json
 import logging
 from collections import defaultdict
 from collections import Counter
 import zipfile
 import datetime
@@ -224,22 +224,24 @@
     def dump_data(
             self,
             tickers=None,
             date_start=None,
             date_end=None,
             is_to_update_existing=False,
             int_max_tickers_to_get=None,
-            tickers_to_exclude : Optional[list[str]] = None,
+            tickers_to_exclude=None,
     ):
         """Main method to dump new of update existing historical data
 
         Args:
             tickers (list[str]):\
                 list trading pairs for which to dump data\
                 by default all ****USDT pairs will be taken
+            tickers_to_exclude (list[str]):\
+                list trading pairs which to exclude from dump
             date_start (datetime.date): Date from which to start dump
             date_end (datetime.date): The last date for which to dump data
             is_to_update_existing (bool): \
                 Flag if you want to update data if it's already exists
             int_max_tickers_to_get (int): Max number of trading pairs to get
         """
         self.dict_new_points_saved_by_ticker.clear()
```

### Comparing `binance_historical_data-0.1.8/src/binance_historical_data/logger.py` & `binance_historical_data-0.1.9/src/binance_historical_data/logger.py`

 * *Files identical despite different names*

### Comparing `binance_historical_data-0.1.8/setup.py` & `binance_historical_data-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['char>=0.1.2,<0.2.0',
  'ipywidgets>=7.6.5,<8.0.0',
  'mpire>=2.3.3,<3.0.0',
  'tqdm>=4.62.3,<5.0.0']
 
 setup_kwargs = {
     'name': 'binance-historical-data',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '========================\nbinance_historical_data\n========================\n\n.. image:: https://img.shields.io/github/last-commit/stas-prokopiev/binance_historical_data\n   :target: https://img.shields.io/github/last-commit/stas-prokopiev/binance_historical_data\n   :alt: GitHub last commit\n\n.. image:: https://img.shields.io/github/license/stas-prokopiev/binance_historical_data\n    :target: https://github.com/stas-prokopiev/binance_historical_data/blob/master/LICENSE.txt\n    :alt: GitHub license<space><space>\n\n.. image:: https://img.shields.io/pypi/v/binance_historical_data\n   :target: https://img.shields.io/pypi/v/binance_historical_data\n   :alt: PyPI\n\n.. image:: https://img.shields.io/pypi/pyversions/binance_historical_data\n   :target: https://img.shields.io/pypi/pyversions/binance_historical_data\n   :alt: PyPI - Python Version\n\n\n.. contents:: **Table of Contents**\n\nShort Overview.\n=========================\nbinance_historical_data is a python package (**py>=3.8**)\nwhich makes download of historical crypto data (prices and volumes) from binance server as simple as it can only be.\n**You don\'t even need to have an account at binance.com to download all history of crypto data**\n\n| Data is taken from here: https://data.binance.vision/?prefix=data/spot/\n| Dumped locally and then unzipped,\n| so you would have an identical local ready to use data copy\n\n| Using this package you will be able to have full historical data of prices and volumes with only 3 lines of python code\n| And if you need to update already downloaded data then once again 3 lines of python code will do the job\n\n\n| **Limitations**: The previous day data appears on binance server a few minutes after 0 a.m. UTC\n| So there is a delay in which you can get the data.\n\nInstallation via pip:\n======================\n\n.. code-block:: bash\n\n    pip install binance_historical_data\n\nHow to use it\n===========================\n\nInitialize main object: **data_dumper**\n---------------------------------------------\n\n.. code-block:: python\n\n    from binance_historical_data import BinanceDataDumper\n\n    data_dumper = BinanceDataDumper(\n        path_dir_where_to_dump=".",\n        data_type="klines",  # aggTrades, klines, trades\n        data_frequency="1m",  # argument for data_type="klines"\n    )\n\nArguments:\n\n#. **path_dir_where_to_dump**:\n    | (string) Path to folder where to dump the data\n#. **data_type="klines"**:\n    | (string) data type to dump: [aggTrades, klines, trades]\n#. **str_data_frequency**:\n    | (string) One of [1m, 3m, 5m, 15m, 30m, 1h, 2h, 4h, 6h, 8h, 12h]\n    | Frequency of price-volume data candles to get\n\n1) The only method to dump the data\n------------------------------------------\n\n.. code-block:: python\n\n    data_dumper.dump_data(\n        tickers=None,\n        date_start=None,\n        date_end=None,\n        is_to_update_existing=False,\n        tickers_to_exclude=["UST"],\n    )\n\nArguments:\n\n#. **tickers=None**:\n    | (list) Trading pairs for which to dump data\n    | *if equals to None* - all **USDT** pairs will be used\n#. **date_start=None**:\n    | (datetime.date) The date from which to start dump\n    | *if equals to None* - every trading pair will be dumped from the early begining (the earliest is 2017-01-01)\n#. **date_end=True=None**:\n    | (datetime.date) The last date for which to dump data\n    | *if equals to None* - Today\'s date will be used\n#. **is_to_update_existing=False**:\n    | (bool) Flag if you want to update the data if it\'s already exist\n#. **tickers_to_exclude=None**:\n    | (list) Tickers to exclude from dump\n\n\n2) Delete outdated daily results\n----------------------------------------------------\n\nDeleta all daily data for which full month monthly data was already dumped\n\n.. code-block:: python\n\n    data_dumper.delete_outdated_daily_results()\n\n.csv klines (candles) files columns\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\n| "Open time" - Timestamp\n| "Open"\n| "High"\n| "Low"\n| "Close"\n| "Volume"\n| "Close time" - Timestamp\n| "Quote asset volume"\n| "Number of trades"\n| "Taker buy base asset volume"\n| "Taker buy quote asset volume"\n| "Ignore"\n\nExamples\n===========================\n\nHow to dump all data for all USDT trading pairs\n------------------------------------------------\n\nPlease be advised that the first data dump for all trading pairs might take some time (~40 minutes)\n\n.. code-block:: python\n\n    data_dumper.dump_data()\n\nHow to update data (get all new data)\n----------------------------------------------\n\n| It\'s as easy as running the exactly same method **dump_data** once again\n| The **data_dumper** will find all the dates for which data already exists\n| and will try to dump only the new data\n\n.. code-block:: python\n\n    data_dumper.dump_data()\n\nHow to update (reload) data for the asked time period\n----------------------------------------------------------\n\n.. code-block:: python\n\n    data_dumper.dump_data(\n        date_start=datetime.date(year=2021, month=1, day=1),\n        date_end=datetime.date(year=2022, month=1, day=1),\n        is_to_update_existing=True\n    )\n\nOther useful methods\n===========================\n\nGet all trading pairs (tickers) from binance\n----------------------------------------------------\n\n.. code-block:: python\n\n    print(data_dumper.get_list_all_trading_pairs())\n\nGet all tickers with locally saved data\n----------------------------------------------------\n\n.. code-block:: python\n\n    print(\n        data_dumper.get_all_tickers_with_data(timeperiod_per_file="daily")\n    )\n\n\nGet all dates for which there is locally saved data\n----------------------------------------------------\n\n.. code-block:: python\n\n    print(\n        data_dumper.get_all_dates_with_data_for_ticker(\n            ticker,\n            timeperiod_per_file="monthly"\n        )\n    )\n\nGet directory where the local data of exact ticker lies\n--------------------------------------------------------\n\n.. code-block:: python\n\n    print(\n        data_dumper.get_local_dir_to_data(\n            ticker,\n            timeperiod_per_file,\n        )\n    )\n\nCreate file name for the local file\n----------------------------------------------------\n\n.. code-block:: python\n\n    print(\n        data_dumper.create_filename(\n            ticker,\n            date_obj,\n            timeperiod_per_file="monthly",\n        )\n    )\n\nLinks\n=====\n\n    * `PYPI <https://pypi.org/project/binance_historical_data/>`_\n    * `GitHub <https://github.com/stas-prokopiev/binance_historical_data>`_\n\nProject local Links\n===================\n\n    * `CHANGELOG <https://github.com/stas-prokopiev/binance_historical_data/blob/master/CHANGELOG.rst>`_.\n    * `CONTRIBUTING <https://github.com/stas-prokopiev/binance_historical_data/blob/master/CONTRIBUTING.rst>`_.\n\nContacts\n========\n\n    * Email: stas.prokopiev@gmail.com\n    * `vk.com <https://vk.com/stas.prokopyev>`_\n    * `Facebook <https://www.facebook.com/profile.php?id=100009380530321>`_\n\nLicense\n=======\n\nThis project is licensed under the MIT License.',
     'author': 'stanislav',
     'author_email': 'stas.prokopiev@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/stas-prokopiev/binance_historical_data',
```

### Comparing `binance_historical_data-0.1.8/PKG-INFO` & `binance_historical_data-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-historical-data
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Home-page: https://github.com/stas-prokopiev/binance_historical_data
 License: MIT
 Author: stanislav
 Author-email: stas.prokopiev@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

