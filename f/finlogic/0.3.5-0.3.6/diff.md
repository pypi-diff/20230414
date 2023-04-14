# Comparing `tmp/FinLogic-0.3.5.tar.gz` & `tmp/FinLogic-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinLogic-0.3.5.tar", last modified: Sun Apr  9 20:52:53 2023, max compression
+gzip compressed data, was "FinLogic-0.3.6.tar", last modified: Fri Apr 14 09:14:29 2023, max compression
```

## Comparing `FinLogic-0.3.5.tar` & `FinLogic-0.3.6.tar`

### file list

```diff
@@ -1,11 +1,16 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 FinLogic-0.3.5/LICENSE
--rw-r--r--   0        0        0    10136 2023-04-03 10:41:08.794859 FinLogic-0.3.5/README.md
--rw-r--r--   0        0        0      423 2023-04-09 20:49:47.249787 FinLogic-0.3.5/finlogic/__init__.py
--rw-r--r--   0        0        0    22313 2023-04-09 20:35:22.450104 FinLogic-0.3.5/finlogic/company.py
--rw-r--r--   0        0        0      745 2023-03-19 09:29:48.278335 FinLogic-0.3.5/finlogic/config.py
--rw-r--r--   0        0        0    16372 2023-04-09 20:35:22.450104 FinLogic-0.3.5/finlogic/database.py
--rw-r--r--   0        0        0      996 2023-04-02 12:44:27.971854 FinLogic-0.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 FinLogic-0.3.5/tests/__init__.py
--rw-r--r--   0        0        0     2232 2023-04-02 12:44:27.971854 FinLogic-0.3.5/tests/test_company.py
--rw-r--r--   0        0        0      683 2023-04-03 10:41:04.879825 FinLogic-0.3.5/tests/test_database.py
--rw-r--r--   0        0        0    10776 1970-01-01 00:00:00.000000 FinLogic-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 FinLogic-0.3.6/LICENSE
+-rw-r--r--   0        0        0    10136 2023-04-03 10:41:08.794859 FinLogic-0.3.6/README.md
+-rw-r--r--   0        0        0       37 2023-04-10 11:28:54.467326 FinLogic-0.3.6/finlogic/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-04-10 11:28:54.467326 FinLogic-0.3.6/finlogic/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2023-04-10 11:28:54.467326 FinLogic-0.3.6/finlogic/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2023-04-10 11:28:54.467326 FinLogic-0.3.6/finlogic/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-04-10 11:28:54.467326 FinLogic-0.3.6/finlogic/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      423 2023-04-14 01:44:35.137202 FinLogic-0.3.6/finlogic/__init__.py
+-rw-r--r--   0        0        0    21829 2023-04-14 09:12:15.664615 FinLogic-0.3.6/finlogic/company.py
+-rw-r--r--   0        0        0      745 2023-03-19 09:29:48.278335 FinLogic-0.3.6/finlogic/config.py
+-rw-r--r--   0        0        0    16130 2023-04-14 01:44:35.137202 FinLogic-0.3.6/finlogic/database.py
+-rw-r--r--   0        0        0      996 2023-04-02 12:44:27.971854 FinLogic-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 FinLogic-0.3.6/tests/__init__.py
+-rw-r--r--   0        0        0     2125 2023-04-14 09:12:15.664615 FinLogic-0.3.6/tests/test_company.py
+-rw-r--r--   0        0        0      597 2023-04-14 09:12:15.664615 FinLogic-0.3.6/tests/test_database.py
+-rw-r--r--   0        0        0    10776 1970-01-01 00:00:00.000000 FinLogic-0.3.6/PKG-INFO
```

### Comparing `FinLogic-0.3.5/LICENSE` & `FinLogic-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.5/README.md` & `FinLogic-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.5/finlogic/company.py` & `FinLogic-0.3.6/finlogic/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,75 +15,67 @@
 import pandas as pd
 from . import config as c
 
 
 class Company:
     """A class to represent a company financial data.
 
-    This class provides methods to create financial reports and to
-    calculate financial indicators based on a company's accounting data.
-    The class also has an AI generated dictionary to translate from
-    Portuguese to English.
-
-    Attributes:
-        identifier:
-            A unique identifier to filter a company in FinLogic
-            Database. Both CVM ID or Fiscal ID can be used. CVM ID
-            (regulator number) must be an integer. Fiscal ID must be a
-            string in 'XX.XXX.XXX/XXXX-XX' format.
+    This class provides methods to create financial reports and to calculate
+    financial indicators based on a company's accounting data. The class also
+    has an AI generated dictionary to translate from Portuguese to English.
 
     Methods:
-        report:
-            Generates a financial report based on a specified report
-            type and accounting level.
-        custom_report:
-            Creates a financial report from a custom list of accounting
-            codes.
-        indicators:
-            Returns a DataFrame with common financial indicators for the
-            company.
+        report: Creates a financial report for the company.
+        custom_report: Creates a custom financial report for the company.
+        indicators: Calculates the financial indicators of the company.
 
     Raises:
         ValueError: If the input arguments are invalid.
     """
 
     def __init__(
         self,
         identifier: int | str,
         acc_method: Literal["consolidated", "separate"] = "consolidated",
         acc_unit: float | str = 1.0,
         tax_rate: float = 0.34,
         language: str = "english",
     ):
         """Initializes a new instance of the Company class."""
-        self.set_id(identifier)
+        self.identifier = identifier
         self.acc_method = acc_method
         self.acc_unit = acc_unit
         self.tax_rate = tax_rate
         self.language = language
 
-    def set_id(self, identifier) -> None:
+    @property
+    def identifier(self) -> int | str:
         """Set a unique identifier to select the company in FinLogic Database.
 
         This method sets the company's CVM and fiscal ID based on a given
         identifier. The identifier can be either the CVM ID or the Fiscal ID
         (CNPJ). If the identifier is not found in the database, a KeyError is
         raised.
-        Args:
 
-        identifier: A unique identifier for the company, either as a CVM ID or
-            Fiscal ID (CNPJ). CVM ID (regulator ID) must be an integer.
-            Fiscal ID must be a string in the format 'XX.XXX.XXX/XXXX-XX'.
+        Args:
+            identifier: A unique identifier to select a company in FinLogic
+                Database. Both CVM ID or Fiscal ID can be used. CVM ID
+                (regulator number) must be an integer. Fiscal ID must be a
+                string in 'XX.XXX.XXX/XXXX-XX' format.
 
         Returns:
             None
 
         Raises:
             KeyError: If the given identifier isn't found in Finlogic Database.
         """
+        return self._identifier
+
+    @identifier.setter
+    def identifier(self, identifier: int | str):
         # Create custom data frame for ID selection
         df = (
             c.main_df[["cvm_id", "fiscal_id"]]
             .drop_duplicates()
             .astype({"cvm_id": int, "fiscal_id": str})
         )
         if identifier in df["cvm_id"].values:
@@ -92,14 +84,15 @@
         elif identifier in df["fiscal_id"].values:
             self._fiscal_id = identifier
             self._cvm_id = df.loc[df["fiscal_id"] == identifier, "cvm_id"].item()
         else:
             raise KeyError("Company 'identifier' not found in database")
         # Only set company data after object identifier validation
         self._set_main_data()
+        self._identifier = identifier
 
     @property
     def acc_method(self) -> Literal["consolidated", "separate"]:
         """Gets or sets the accounting method for registering investments in
         subsidiaries.
 
         The "acc_method" must be "consolidated" or "separate". Consolidated
@@ -209,17 +202,16 @@
     @language.setter
     def language(self, language: str):
         # Supported languages
         list_languages = ["english", "portuguese"]
         if language.lower() in list_languages:
             self._language = language.capitalize()
         else:
-            raise KeyError(
-                f"'{language}' not supported. Supported languages: {', '.join(list_languages)}"
-            )
+            sup_lang = f"Supported languages: {', '.join(list_languages)}"
+            raise KeyError(f"'{language}' not supported. {sup_lang}")
 
     def _set_main_data(self) -> pd.DataFrame:
         self._COMP_DF = (
             c.main_df.query("cvm_id == @self._cvm_id")
             .astype(
                 {
                     "co_name": str,
@@ -248,31 +240,29 @@
         self._LAST_ANNUAL = self._COMP_DF.query('report_type == "annual"')[
             "period_end"
         ].max()
         self._LAST_QUARTERLY = self._COMP_DF.query('report_type == "quarterly"')[
             "period_end"
         ].max()
 
-    def info(self) -> pd.DataFrame:
-        """Return dataframe with company info."""
+    def info(self) -> dict:
+        """Return a dictionay with company info."""
         company_info = {
             "Name": self._NAME,
             "CVM ID": self._cvm_id,
             "Fiscal ID (CNPJ)": self._fiscal_id,
             "Total Accounting Rows": len(self._COMP_DF.index),
             "Selected Tax Rate": self._tax_rate,
             "Selected Accounting Method": self._acc_method,
             "Selected Accounting Unit": self._acc_unit,
             "First Annual Report": self._FIRST_ANNUAL.strftime("%Y-%m-%d"),
             "Last Annual Report": self._LAST_ANNUAL.strftime("%Y-%m-%d"),
             "Last Quarterly Report": self._LAST_QUARTERLY.strftime("%Y-%m-%d"),
         }
-        df = pd.DataFrame.from_dict(company_info, orient="index", columns=["Values"])
-        df.index.name = "Company Info"
-        return df
+        return company_info
 
     def report(
         self,
         report_type: str,
         acc_level: int | None = None,
         num_years: int = 0,
     ) -> pd.DataFrame:
@@ -286,19 +276,19 @@
                 include: "assets", "cash", "current_assets",
                 "non_current_assets", "liabilities", "debt",
                 "current_liabilities", "non_current_liabilities",
                 "liabilities_and_equity", "equity", "income",
                 "earnings_per_share", "comprehensive_income",
                 "changes_in_equity", "cash_flow" and "added_value".
             acc_level: Detail level to show for account codes. Options are 2,
-                3, 4 or None. Defaults to None.
-                    None -> X...       (default: show all accounts)
+                3, 4 or None. Defaults to None. How the values works:
                     2    -> X.YY       (show 2 levels)
                     3    -> X.YY.ZZ    (show 3 levels)
                     4    -> X.YY.ZZ.WW (show 4 levels)
+                    None -> X...       (default: show all accounts)
             num_years: Number of years to include in the report. Defaults to 0
                 (all years).
 
         Returns:
             pd.DataFrame: Generated financial report as a pandas DataFrame.
 
         Raises:
@@ -533,16 +523,14 @@
         dfo.loc["after_tax_operating_margin"] = ebit * (1 - self._tax_rate) / revenues
         dfo.loc["net_margin"] = net_income / revenues
 
         dfo.index.name = "Company Financial Indicators"
         # Show only the selected number of years
         if num_years > 0:
             dfo = dfo[dfo.columns[-num_years:]]
-        # Since all columns are strings representing corporate year, convert them to datetime64
-        # dfo.columns = pd.to_datetime(dfo.columns)
         return dfo
 
     def _make_report(self, dfi: pd.DataFrame) -> pd.DataFrame:
         # keep only last quarterly fs
         if self._LAST_ANNUAL > self._LAST_QUARTERLY:
             df = dfi.query('report_type == "annual"').copy()
             df.query(
@@ -564,19 +552,17 @@
 
         # Create output dataframe with only the index
         dfo = df.sort_values(by="period_end", ascending=True)[
             ["acc_name", "acc_code", "acc_fixed"]
         ].drop_duplicates(subset="acc_code", ignore_index=True, keep="last")
 
         periods = list(df["period_end"].sort_values().unique())
-
         for period in periods:
-            df_year = df.query("period_end == @period")[
-                ["acc_value", "acc_code"]
-            ].copy()
-            period_str = str(np.datetime_as_string(period, unit="D"))
+            year_cols = ["acc_value", "acc_code"]
+            df_year = df.query("period_end == @period")[year_cols].copy()
+            period_str = period.strftime("%Y-%m-%d")
             if period == self._LAST_QUARTERLY:
                 period_str += " (ttm)"
             df_year.rename(columns={"acc_value": period_str}, inplace=True)
             dfo = pd.merge(dfo, df_year, how="left", on=["acc_code"])
 
         return dfo.sort_values("acc_code", ignore_index=True)
```

### Comparing `FinLogic-0.3.5/finlogic/config.py` & `FinLogic-0.3.6/finlogic/config.py`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.5/finlogic/database.py` & `FinLogic-0.3.6/finlogic/database.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 """
 
 import os
 from pathlib import Path
 import shutil
 import math
 import zipfile
-from datetime import datetime
 from typing import List
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 import requests
 import pandas as pd
 import numpy as np
 from . import config as c
 
 URL_DFP = "http://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/DFP/DADOS/"
 URL_ITR = "http://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/ITR/DADOS/"
-URL_LANGUAGE = "https://raw.githubusercontent.com/fe-lipe-c/finlogic_datasets/master/data/pten_df.csv"
+URL_LANGUAGE = "https://raw.githubusercontent.com/fe-lipe-c/finlogic_datasets/master/data/pten_df.csv"  # noqa
 RAW_DIR = c.DATA_PATH / "raw"
 PROCESSED_DIR = c.DATA_PATH / "processed"
 INTERIM_DIR = c.DATA_PATH / "interim"
 CHECKMARK = "\033[32m\u2714\033[0m"
 
 
 def list_urls() -> List[str]:
@@ -61,38 +60,39 @@
 def update_raw_file(url: str) -> Path:
     """Update raw file from CVM portal. Return a Path if file is updated."""
     raw_path = Path(RAW_DIR, url[-23:])  # filename = url final
     with requests.Session() as s:
         r = s.get(url, stream=True)
         if r.status_code != requests.codes.ok:
             return None
-        if Path.exists(raw_path):
-            local_file_size = raw_path.stat().st_size
-        else:
-            local_file_size = 0
-        url_file_size = int(r.headers["Content-Length"])
-        if local_file_size == url_file_size:
-            return None
-        with raw_path.open(mode="wb") as f:
-            f.write(r.content)
 
-        # Timestamps
-        ts_gmt = pd.to_datetime(r.headers["Last-Modified"])
-        ts_sao_paulo = ts_gmt.tz_convert("America/sao_paulo")
-        ts_now = pd.Timestamp.now().tz_localize("America/sao_paulo")
-
-        # Store URL files metadata
-        c.cvm_df.loc[ts_now] = [
-            raw_path.name,
-            r.headers["Content-Length"],
-            r.headers["ETag"],
-            ts_sao_paulo,
-        ]
-        print(f"    {CHECKMARK} {raw_path.name} downloaded.")
-        return raw_path
+    if Path.exists(raw_path):
+        local_file_size = raw_path.stat().st_size
+    else:
+        local_file_size = 0
+    url_file_size = int(r.headers["Content-Length"])
+    if local_file_size == url_file_size:
+        # File is already updated
+        return None
+    with raw_path.open(mode="wb") as f:
+        f.write(r.content)
+
+    # headers["Last-Modified"] -> 'Wed, 23 Jun 2021 12:19:24 GMT'
+    ts_server = pd.to_datetime(
+        r.headers["Last-Modified"], format="%a, %d %b %Y %H:%M:%S %Z"
+    )
+    # Store URL files metadata
+    c.cvm_df.loc[pd.Timestamp.now()] = [
+        raw_path.name,
+        r.headers["Content-Length"],
+        r.headers["ETag"],
+        ts_server,
+    ]
+    print(f"    {CHECKMARK} {raw_path.name} downloaded.")
+    return raw_path
 
 
 def update_raw_files(urls: str) -> List[Path]:
     """Update local CVM raw files asynchronously."""
     with ThreadPoolExecutor() as executor:
         results = executor.map(update_raw_file, urls)
     c.cvm_df.to_pickle(c.CVM_DF_PATH)
@@ -174,118 +174,113 @@
     [cols.remove(col) for col in cols_remove]
     # Ascending order --> last is the newest report_version
     c.main_df.drop_duplicates(cols, keep="last", inplace=True)
     c.main_df.to_pickle(c.MAIN_DF_PATH)
 
 
 def search_company(expression: str) -> pd.DataFrame:
-    """Search for company names in the FinLogic Database containing a given expression.
+    """Search for company names in the FinLogic Database.
 
-    This function searches the 'co_name' column in the FinLogic Database for company names
-    that contain the provided expression. It returns a DataFrame containing the search
-    results, with each row representing a unique company that matches the search criteria.
+    This function searches the 'co_name' column in the FinLogic Database for
+    company names that contain the provided expression. It returns a DataFrame
+    containing the search results, with each row representing a unique company
+    that matches the search criteria.
 
     Args:
-        expression (str): A string to search for in the FinLogic Database 'co_name' column.
+        expression (str): A string to search for in the FinLogic Database
+            'co_name' column.
 
     Returns:
-        pd.DataFrame: A DataFrame containing the search results, with columns 'co_name',
-            'cvm_id', and 'fiscal_id' for each unique company that matches the search
-            criteria.
+        pd.DataFrame: A DataFrame containing the search results, with columns
+            'co_name', 'cvm_id', and 'fiscal_id' for each unique company that
+            matches the search criteria.
     """
     expression = expression.upper()
     df = (
         c.main_df.query("co_name.str.contains(@expression)")
         .sort_values(by="co_name")
         .drop_duplicates(subset="cvm_id", ignore_index=True)[
             ["co_name", "cvm_id", "fiscal_id"]
         ]
     )
     return df
 
 
-def database_info() -> pd.DataFrame:
+def database_info() -> dict:
     """Returns general information about FinLogic Database.
 
     This function generates a pandas DataFrame containing various information
     about the FinLogic database, such as the database path, file size, last
     update call, last modified dates, size in memory, number of accounting rows,
     unique accounting codes, companies, unique financial statements, first
     financial statement date, and last financial statement date.
 
     Returns:
-        pd.DataFrame: A DataFrame containing the FinLogic Database information.
+        A dictionary containing the FinLogic Database information.
     """
     if c.main_df.empty:
-        print("There is no data in database")
+        print("Finlogic Database is empty")
         return
-    info_df = pd.DataFrame()
-    info_df.index.name = "FinLogic Database Info"
-    info_df["Value"] = ""
-    info_df.loc["Database Path"] = c.DATA_PATH
-    info_df.loc["File Size (MB)"] = round(
-        c.MAIN_DF_PATH.lstat().st_size / (1024 * 1024), 1
-    )
-    info_df.loc["Last Update Call"] = c.cvm_df.index.max().round("1s").tz_localize(None)
-    # Convert python datetime to Pandas Timestamp
-    last_modified_python = datetime.fromtimestamp(c.MAIN_DF_PATH.lstat().st_mtime)
-    last_modified_pandas = pd.to_datetime(last_modified_python).round("1s")
-    info_df.loc["Finlogic Last Modified"] = last_modified_pandas
-    info_df.loc["CVM Last Update"] = c.cvm_df["last_modified"].max().tz_localize(None)
-    info_df.loc["Size in Memory (MB)"] = round(
-        c.main_df.memory_usage(index=True, deep=True).sum() / (1024 * 1024), 1
-    )
-    info_df.loc["Accounting Rows"] = len(c.main_df.index)
-    info_df.loc["Unique Accounting Codes"] = c.main_df["acc_code"].nunique()
-    info_df.loc["Companies"] = c.main_df["cvm_id"].nunique()
+    info_dict = {}
+    info_dict["Database Path"] = c.DATA_PATH
+    file_size = c.MAIN_DF_PATH.stat().st_size
+    info_dict["File Size (MB)"] = round(file_size / (1024 * 1024), 1)
+    info_dict["Last Update Call"] = c.cvm_df.index.max().round("1s").isoformat()
+    ts_unix = round(c.MAIN_DF_PATH.stat().st_mtime, 0)
+    ts_iso = pd.Timestamp.fromtimestamp(ts_unix).isoformat()
+    info_dict["Finlogic Last Modified"] = ts_iso
+    info_dict["CVM Last Update"] = c.cvm_df["last_modified"].max().isoformat()
+    data_size = c.main_df.memory_usage(index=True, deep=True).sum()
+    info_dict["Data Size in Memory (MB)"] = round(data_size / (1024 * 1024), 1)
+    info_dict["Accounting Rows"] = len(c.main_df.index)
+    info_dict["Unique Accounting Codes"] = c.main_df["acc_code"].nunique()
+    info_dict["Companies"] = c.main_df["cvm_id"].nunique()
     columns_duplicates = ["cvm_id", "report_version", "report_type", "period_reference"]
-    info_df.loc["Unique Financial Statements"] = len(
-        c.main_df.drop_duplicates(subset=columns_duplicates).index
-    )
-    info_df.loc["First Financial Statement"] = (
-        c.main_df["period_end"].astype("datetime64[ns]").min().strftime("%Y-%m-%d")
-    )
-    info_df.loc["Last Financial Statement"] = (
-        c.main_df["period_end"].astype("datetime64[ns]").max().strftime("%Y-%m-%d")
-    )
-    return info_df
+    num_unique = len(c.main_df.drop_duplicates(subset=columns_duplicates).index)
+    info_dict["Unique Financial Statements"] = num_unique
+    first_statement = c.main_df["period_end"].astype("datetime64[ns]").min()
+    info_dict["First Financial Statement"] = first_statement.strftime("%Y-%m-%d")
+    last_statement = c.main_df["period_end"].astype("datetime64[ns]").max()
+    info_dict["Last Financial Statement"] = last_statement.strftime("%Y-%m-%d")
+    return info_dict
 
 
 def update_database(
     reset_data: bool = False, asynchronous: bool = False, cpu_usage: float = 0.75
 ):
-    """Create/Update all remote files (raw files) and process them for local data
-    access.
+    """Verify changes in remote files and update them in Finlogic Database.
 
     Args:
-        reset_data: Delete all raw files and force a full database recompilation. Default
-            is False.
-        asynchronous: Generate the database by processing raw files asynchronously.
-            Works only on Linux and Mac. Default is False.
-        cpu_usage: A number between 0 and 1, where 1 represents 100% CPU usage. This
-            argument will define the number of cpu cores used for data processing when
-            function asynchronous mode is set to 'True'. Default is 0.75.
+        reset_data: Delete all raw files and force a full database
+            recompilation. Default is False.
+        asynchronous: Generate the database by processing raw files
+            asynchronously. Works only on Linux and Mac. Default is False.
+        cpu_usage: A number between 0 and 1, where 1 represents 100% CPU usage.
+            This argument will define the number of cpu cores used for data
+            processing when function asynchronous mode is set to 'True'. Default
+            is 0.75.
 
     Returns:
         None
     """
-    # Parameter 'reset_data'-> delete, if they exist, data folders
+    # Parameter 'reset_data'-> delete, if they exist, data folders.
     if reset_data:
         if Path.exists(c.DATA_PATH):
             shutil.rmtree(c.DATA_PATH)
         c.main_df = pd.DataFrame()
-    # create data folders if they do not exist
+    # Create data folders if they do not exist.
     Path.mkdir(RAW_DIR, parents=True, exist_ok=True)
     Path.mkdir(PROCESSED_DIR, parents=True, exist_ok=True)
-    # Define the number of cpu cores for parallel data processing
+    # Define the number of cpu cores for parallel data processing.
     workers = math.trunc(os.cpu_count() * cpu_usage)
     if workers < 1:
         workers = 1
     print("Updating financial statements...")
     urls = list_urls()
+    # urls = urls[:1]  # Test
     raw_paths = update_raw_files(urls)
     print(f"Number of financial statements updated = {len(raw_paths)}")
     print("\nProcessing financial statements...")
     processed_filenames = process_raw_files(
         workers, raw_paths, asynchronous=asynchronous
     )
     print("\nConsolidating processed files...")
```

### Comparing `FinLogic-0.3.5/pyproject.toml` & `FinLogic-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pandas>=1.4.0",
     "requests>=2.27.0",
     "zstandard>=0.17.0",
 ]
-version = "0.3.5"
+version = "0.3.6"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.0.0",
```

### Comparing `FinLogic-0.3.5/tests/test_company.py` & `FinLogic-0.3.6/tests/test_company.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import finlogic as fl
 
 
 def test_petro_info():
     # Petro info
     petro = fl.Company(9512, acc_method="separate", acc_unit="billion")
-    petro_info = petro.info()
     # Get the info
-    co_name = petro_info.at["Name", "Values"]
-    cvm_id = petro_info.at["CVM ID", "Values"]
-    fiscal_id = petro_info.at["Fiscal ID (CNPJ)", "Values"]
+    petro_info = petro.info()
     # Check the info
-    assert co_name == "PETROLEO BRASILEIRO S.A. PETROBRAS"
-    assert cvm_id == 9512
-    assert fiscal_id == "33.000.167/0001-01"
+    assert petro_info["Name"] == "PETROLEO BRASILEIRO S.A. PETROBRAS"
+    assert petro_info["CVM ID"] == 9512
+    assert petro_info["Fiscal ID (CNPJ)"] == "33.000.167/0001-01"
 
 
 def test_petro_report():
     # Petro reports
     petro = fl.Company(9512, acc_method="consolidated", acc_unit="billion")
     petro_report = petro.report(report_type="assets")
     # Get Total Assets
```

### Comparing `FinLogic-0.3.5/tests/test_database.py` & `FinLogic-0.3.6/tests/test_database.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import finlogic as fl
 
 
 def test_db_info():
     db_info = fl.database_info()
-    first_statement = db_info.at["First Financial Statement", "Value"]
-    acc_rows = db_info.at["Accounting Rows", "Value"]
-    assert first_statement == "2009-01-31"
-    assert acc_rows > 20_000_000
+    assert db_info["First Financial Statement"] == "2009-01-31"
+    assert db_info["Accounting Rows"] > 20_000_000
 
 
 def test_search_company():
     # Search for petrobras
     search_result = fl.search_company("petrobras")
     """
         co_name                            cvm_id  fiscal_id
```

### Comparing `FinLogic-0.3.5/PKG-INFO` & `FinLogic-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinLogic
-Version: 0.3.5
+Version: 0.3.6
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-email: Carlos Carvalho <cr.cj@outlook.com>
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FinLogic Version: 0.3.5 Summary: Finance toolkit
+Metadata-Version: 2.1 Name: FinLogic Version: 0.3.6 Summary: Finance toolkit
 for listed Brazilian companies Keywords: pandas, cvm, finance, investment,
 accounting Author-email: Carlos Carvalho
 cj@outlook.com> Requires-Python: >=3.10 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Office/Business ::
 Financial :: Accounting Classifier: Topic :: Office/Business :: Financial ::
 Investment Provides-Extra: test Project-URL: repository, https://github.com/
```

