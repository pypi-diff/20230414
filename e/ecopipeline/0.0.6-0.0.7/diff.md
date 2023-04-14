# Comparing `tmp/ecopipeline-0.0.6.tar.gz` & `tmp/ecopipeline-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecopipeline-0.0.6.tar", last modified: Fri Apr 14 00:01:09 2023, max compression
+gzip compressed data, was "ecopipeline-0.0.7.tar", last modified: Fri Apr 14 19:22:19 2023, max compression
```

## Comparing `ecopipeline-0.0.6.tar` & `ecopipeline-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 00:01:09.543626 ecopipeline-0.0.6/
--rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1086 2023-04-14 00:01:09.625867 ecopipeline-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-04-10 20:35:13.000000 ecopipeline-0.0.6/README.md
--rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      735 2023-04-14 00:01:09.839381 ecopipeline-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:01:01.287613 ecopipeline-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 00:01:06.191621 ecopipeline-0.0.6/src/ecopipeline/
--rw-rw-rw-   0        0        0     2060 2023-04-13 22:42:27.000000 ecopipeline-0.0.6/src/ecopipeline/__init__.py
--rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.6/src/ecopipeline/bayview.py
--rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.6/src/ecopipeline/config.py
--rw-rw-rw-   0        0        0    13858 2023-04-10 20:26:32.000000 ecopipeline-0.0.6/src/ecopipeline/extract.py
--rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.6/src/ecopipeline/lbnl.py
--rw-rw-rw-   0        0        0     9434 2023-04-10 18:47:39.000000 ecopipeline-0.0.6/src/ecopipeline/load.py
--rw-rw-rw-   0        0        0    30210 2023-04-14 00:00:20.000000 ecopipeline-0.0.6/src/ecopipeline/transform.py
--rw-rw-rw-   0        0        0     2696 2023-02-17 15:53:41.000000 ecopipeline-0.0.6/src/ecopipeline/unit_convert.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:01:09.087626 ecopipeline-0.0.6/src/ecopipeline.egg-info/
--rw-rw-rw-   0        0        0     1086 2023-04-14 00:00:59.000000 ecopipeline-0.0.6/src/ecopipeline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-04-14 00:01:00.000000 ecopipeline-0.0.6/src/ecopipeline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 00:00:59.000000 ecopipeline-0.0.6/src/ecopipeline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-04-14 00:00:59.000000 ecopipeline-0.0.6/src/ecopipeline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-14 00:00:59.000000 ecopipeline-0.0.6/src/ecopipeline.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 19:22:16.602633 ecopipeline-0.0.7/
+-rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1086 2023-04-14 19:22:19.640019 ecopipeline-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-04-10 20:35:13.000000 ecopipeline-0.0.7/README.md
+-rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      735 2023-04-14 19:22:19.747578 ecopipeline-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:22:16.718633 ecopipeline-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 19:22:16.706633 ecopipeline-0.0.7/src/ecopipeline/
+-rw-rw-rw-   0        0        0     2060 2023-04-13 22:42:27.000000 ecopipeline-0.0.7/src/ecopipeline/__init__.py
+-rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.7/src/ecopipeline/bayview.py
+-rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.7/src/ecopipeline/config.py
+-rw-rw-rw-   0        0        0    13858 2023-04-10 20:26:32.000000 ecopipeline-0.0.7/src/ecopipeline/extract.py
+-rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.7/src/ecopipeline/lbnl.py
+-rw-rw-rw-   0        0        0     9434 2023-04-10 18:47:39.000000 ecopipeline-0.0.7/src/ecopipeline/load.py
+-rw-rw-rw-   0        0        0    30494 2023-04-14 19:16:37.000000 ecopipeline-0.0.7/src/ecopipeline/transform.py
+-rw-rw-rw-   0        0        0     2780 2023-04-14 17:28:33.000000 ecopipeline-0.0.7/src/ecopipeline/unit_convert.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:22:16.762633 ecopipeline-0.0.7/src/ecopipeline.egg-info/
+-rw-rw-rw-   0        0        0     1086 2023-04-14 19:22:16.000000 ecopipeline-0.0.7/src/ecopipeline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-04-14 19:22:16.000000 ecopipeline-0.0.7/src/ecopipeline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 19:22:16.000000 ecopipeline-0.0.7/src/ecopipeline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-04-14 19:22:16.000000 ecopipeline-0.0.7/src/ecopipeline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 19:22:16.000000 ecopipeline-0.0.7/src/ecopipeline.egg-info/top_level.txt
```

### Comparing `ecopipeline-0.0.6/PKG-INFO` & `ecopipeline-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.6
+Version: 0.0.7
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ecopipeline-0.0.6/README.md` & `ecopipeline-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.6/setup.cfg` & `ecopipeline-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 636f 7069 7065 6c69 6e65 0d0a   = ecopipeline..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 360d  version = 0.0.6.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 370d  version = 0.0.7.
 00000030: 0a61 7574 686f 7220 3d20 4e6f 6c61 6e20  .author = Nolan 
 00000040: 616e 6420 5355 2053 7475 6465 6e74 730d  and SU Students.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 6e6f 6c61 6e40 6563 6f74 6f70 652e 636f  nolan@ecotope.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2043 6f6e 7461 696e 7320 6675 6e63 7469   Contains functi
 00000090: 6f6e 7320 666f 7220 7573 6520 696e 2045  ons for use in E
```

### Comparing `ecopipeline-0.0.6/src/ecopipeline/__init__.py` & `ecopipeline-0.0.7/src/ecopipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.6/src/ecopipeline/bayview.py` & `ecopipeline-0.0.7/src/ecopipeline/bayview.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.6/src/ecopipeline/config.py` & `ecopipeline-0.0.7/src/ecopipeline/config.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.6/src/ecopipeline/extract.py` & `ecopipeline-0.0.7/src/ecopipeline/extract.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.6/src/ecopipeline/lbnl.py` & `ecopipeline-0.0.7/src/ecopipeline/lbnl.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.6/src/ecopipeline/load.py` & `ecopipeline-0.0.7/src/ecopipeline/load.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.6/src/ecopipeline/transform.py` & `ecopipeline-0.0.7/src/ecopipeline/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import numpy as np
 import datetime as dt
 import csv
 import os
-from ecopipeline.unit_convert import energy_to_power, energy_btu_to_kwh, energy_kwh_to_kbtu
+from ecopipeline.unit_convert import energy_to_power, energy_btu_to_kwh, energy_kwh_to_kbtu, power_flow_to_kW
 from ecopipeline.config import _input_directory, _output_directory
 
 pd.set_option('display.max_columns', None)
 
 
 def concat_last_row(df: pd.DataFrame, last_row: pd.DataFrame) -> pd.DataFrame:
     """
@@ -398,48 +398,53 @@
 
     except ZeroDivisionError:
         print("DIVIDED BY ZERO ERROR")
         return df
 
     return cop_values
 
-def cop_method_2(df: pd.DataFrame, cop_tm):
+def cop_method_2(df: pd.DataFrame, cop_tm, cop_primary_column_name):
+    # TODO this is specific for Maria and Antonia
     """
     Performs COP calculation method 2 as deffined by Scott's whiteboard image
     COP = COP_primary(ELEC_primary/ELEC_total) + COP_tm(ELEC_tm/ELEC_total)
 
     Args: 
         df (pd.DataFrame): Pandas DataFrame to add COP columns to
         cop_tm (float): fixed COP value for temputure Maintenece system
+        cop_primary_column_name (str): Name of the column used for COP_Primary values
 
     Returns: 
         pd.DataFrame: Pandas DataFrame with the added COP columns. 
     """
-    columns_to_check = ['Temp_HPWH1Outlet', 'Flow_HPWH1', 'PowerIn_HPWH1', 'PowerIn_SwingTank', 'PowerIn_Total', 'Temp_CityWater'] # TODO what if there is only 1 HPWH?
+    columns_to_check = [cop_primary_column_name, 'PowerIn_Total']
 
     missing_columns = [col for col in columns_to_check if col not in df.columns]
 
     if missing_columns:
         print('Cannot calculate COP as the following columns are missing from the DataFrame:', missing_columns)
         return df
     
-    #calculate primary COP that is actually equipment COP
-    df['COP_Primary'] = energy_kwh_to_kbtu(df['Flow_HPWH1'], df['Temp_HPWH1Outlet']-df['Temp_CityWater']) / df['PowerIn_HPWH1']
-    
     # Create list of column names to sum
-    sum_cols = [col for col in df.columns if col.startswith('PowerIn_HPWH') or col == 'PowerIn_SecLoopPump']
+    sum_primary_cols = [col for col in df.columns if col.startswith('PowerIn_HPWH') or col == 'PowerIn_SecLoopPump']
+    sum_tm_cols = [col for col in df.columns if col.startswith('PowerIn_SwingTank')]
 
-    if len(sum_cols) == 0:
+    if len(sum_primary_cols) == 0:
         print('Cannot calculate COP as the primary power columns (such as PowerIn_HPWH and PowerIn_SecLoopPump) are missing from the DataFrame')
         return df
 
+    if len(sum_tm_cols) == 0:
+        print('Cannot calculate COP as the temperature maintenance power columns (such as PowerIn_SwingTank) are missing from the DataFrame')
+        return df
+    
     # Create new DataFrame with one column called 'PowerIn_Primary' that contains the sum of the specified columns
-    new_df = pd.DataFrame({'PowerIn_Primary': df[sum_cols].sum(axis=1)})
+    sum_power_in_df = pd.DataFrame({'PowerIn_Primary': df[sum_primary_cols].sum(axis=1),
+                                    'PowerIn_TM': df[sum_tm_cols].sum(axis=1)})
 
-    df['COP'] = (df['COP_Primary'] * (new_df['PowerIn_Primary']/df['PowerIn_Total'])) + (cop_tm * (df['PowerIn_SwingTank']/df['PowerIn_Total'])) # TODO confirm these values
+    df['COP_DHWSys_2'] = (df[cop_primary_column_name] * (sum_power_in_df['PowerIn_Primary']/df['PowerIn_Total'])) + (cop_tm * (sum_power_in_df['PowerIn_TM']/df['PowerIn_Total']))
     return df
 
 
 # loops through a list of dateTime objects, compares if the date of that object matches the
 # date of the row name, which is also a dateTime object. If it matches, load_shift is True (happened that day)
 def _ls_helper(row, dt_list):
     """
```

### Comparing `ecopipeline-0.0.6/src/ecopipeline/unit_convert.py` & `ecopipeline-0.0.7/src/ecopipeline/unit_convert.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,8 +81,11 @@
     return energy * 60
 
 # Used in aggregate_values
 def energy_btu_to_kwh(sensor_readings):
     return sensor_readings / (60 * 3.412)
 
 def energy_kwh_to_kbtu(gpm, delta_t):
-    return 60 * 8.33 * gpm * delta_t / 1000
+    return 60 * 8.33 * gpm * delta_t / 1000
+
+def power_flow_to_kW(gpm, delta_t):
+    return 60 * 8.33 * gpm * delta_t / 3412
```

### Comparing `ecopipeline-0.0.6/src/ecopipeline.egg-info/PKG-INFO` & `ecopipeline-0.0.7/src/ecopipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.6
+Version: 0.0.7
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

