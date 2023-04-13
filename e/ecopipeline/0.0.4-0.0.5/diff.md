# Comparing `tmp/ecopipeline-0.0.4.tar.gz` & `tmp/ecopipeline-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecopipeline-0.0.4.tar", last modified: Mon Apr 10 20:32:05 2023, max compression
+gzip compressed data, was "ecopipeline-0.0.5.tar", last modified: Thu Apr 13 22:45:55 2023, max compression
```

## Comparing `ecopipeline-0.0.4.tar` & `ecopipeline-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 20:32:02.655057 ecopipeline-0.0.4/
--rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1024 2023-04-10 20:32:05.652147 ecopipeline-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      579 2023-02-17 15:53:40.000000 ecopipeline-0.0.4/README.md
--rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      721 2023-04-10 20:32:05.771201 ecopipeline-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:32:02.755057 ecopipeline-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 20:32:02.755057 ecopipeline-0.0.4/src/ecopipeline/
--rw-rw-rw-   0        0        0     2030 2023-04-10 18:45:52.000000 ecopipeline-0.0.4/src/ecopipeline/__init__.py
--rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.4/src/ecopipeline/bayview.py
--rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.4/src/ecopipeline/config.py
--rw-rw-rw-   0        0        0    13858 2023-04-10 20:26:32.000000 ecopipeline-0.0.4/src/ecopipeline/extract.py
--rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.4/src/ecopipeline/lbnl.py
--rw-rw-rw-   0        0        0     9434 2023-04-10 18:47:39.000000 ecopipeline-0.0.4/src/ecopipeline/load.py
--rw-rw-rw-   0        0        0    28442 2023-04-10 17:21:58.000000 ecopipeline-0.0.4/src/ecopipeline/transform.py
--rw-rw-rw-   0        0        0     2696 2023-02-17 15:53:41.000000 ecopipeline-0.0.4/src/ecopipeline/unit_convert.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:32:02.807057 ecopipeline-0.0.4/src/ecopipeline.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-04-10 20:32:02.000000 ecopipeline-0.0.4/src/ecopipeline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-04-10 20:32:02.000000 ecopipeline-0.0.4/src/ecopipeline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 20:32:02.000000 ecopipeline-0.0.4/src/ecopipeline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-04-10 20:32:02.000000 ecopipeline-0.0.4/src/ecopipeline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-10 20:32:02.000000 ecopipeline-0.0.4/src/ecopipeline.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 22:45:55.543100 ecopipeline-0.0.5/
+-rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1086 2023-04-13 22:45:55.566088 ecopipeline-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-04-10 20:35:13.000000 ecopipeline-0.0.5/README.md
+-rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      735 2023-04-13 22:45:55.609610 ecopipeline-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:45:53.807097 ecopipeline-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 22:45:54.975099 ecopipeline-0.0.5/src/ecopipeline/
+-rw-rw-rw-   0        0        0     2060 2023-04-13 22:42:27.000000 ecopipeline-0.0.5/src/ecopipeline/__init__.py
+-rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.5/src/ecopipeline/bayview.py
+-rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.5/src/ecopipeline/config.py
+-rw-rw-rw-   0        0        0    13858 2023-04-10 20:26:32.000000 ecopipeline-0.0.5/src/ecopipeline/extract.py
+-rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.5/src/ecopipeline/lbnl.py
+-rw-rw-rw-   0        0        0     9434 2023-04-10 18:47:39.000000 ecopipeline-0.0.5/src/ecopipeline/load.py
+-rw-rw-rw-   0        0        0    29945 2023-04-13 22:42:27.000000 ecopipeline-0.0.5/src/ecopipeline/transform.py
+-rw-rw-rw-   0        0        0     2696 2023-02-17 15:53:41.000000 ecopipeline-0.0.5/src/ecopipeline/unit_convert.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:45:55.331099 ecopipeline-0.0.5/src/ecopipeline.egg-info/
+-rw-rw-rw-   0        0        0     1086 2023-04-13 22:45:53.000000 ecopipeline-0.0.5/src/ecopipeline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-04-13 22:45:53.000000 ecopipeline-0.0.5/src/ecopipeline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 22:45:53.000000 ecopipeline-0.0.5/src/ecopipeline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-04-13 22:45:53.000000 ecopipeline-0.0.5/src/ecopipeline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-13 22:45:53.000000 ecopipeline-0.0.5/src/ecopipeline.egg-info/top_level.txt
```

### Comparing `ecopipeline-0.0.4/PKG-INFO` & `ecopipeline-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.4
+Version: 0.0.5
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DataPipelinePackage
 
+## To Install the Package
+
+    $ pip install ecopipeline
+
 ## Functions in Data Pipeline package:
 ### extract.py
 - load raw JSON-formatted data into a dataframe
 - merge NOAA weather data with sensor data
 
 ### clean.py
 - remove outliers specified in the configuration file
```

### Comparing `ecopipeline-0.0.4/setup.cfg` & `ecopipeline-0.0.5/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 636f 7069 7065 6c69 6e65 0d0a   = ecopipeline..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 340d  version = 0.0.4.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 350d  version = 0.0.5.
 00000030: 0a61 7574 686f 7220 3d20 4e6f 6c61 6e20  .author = Nolan 
 00000040: 616e 6420 5355 2053 7475 6465 6e74 730d  and SU Students.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 6e6f 6c61 6e40 6563 6f74 6f70 652e 636f  nolan@ecotope.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2043 6f6e 7461 696e 7320 6675 6e63 7469   Contains functi
 00000090: 6f6e 7320 666f 7220 7573 6520 696e 2045  ons for use in E
@@ -33,14 +33,14 @@
 00000200: 7569 7265 7320 3d20 3e3d 332e 3131 0d0a  uires = >=3.11..
 00000210: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
 00000220: 203d 200d 0a09 7061 6e64 6173 3e3d 2031   = ...pandas>= 1
 00000230: 2e35 2e33 0d0a 096e 756d 7079 3e3d 312e  .5.3...numpy>=1.
 00000240: 3234 2e31 0d0a 096d 7973 716c 2d63 6f6e  24.1...mysql-con
 00000250: 6e65 6374 6f72 2d70 7974 686f 6e3e 3d38  nector-python>=8
 00000260: 2e30 2e33 320d 0a09 7363 696b 6974 2d6c  .0.32...scikit-l
-00000270: 6561 726e 3e3d 312e 322e 310d 0a0d 0a5b  earn>=1.2.1....[
-00000280: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000290: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-000002a0: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
-000002b0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-000002c0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-000002d0: 0a                                       .
+00000270: 6561 726e 3e3d 312e 322e 310d 0a09 7374  earn>=1.2.1...st
+00000280: 6174 736d 6f64 656c 730d 0a0d 0a5b 6f70  atsmodels....[op
+00000290: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+000002a0: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+000002b0: 630d 0a0d 0a5b 6567 675f 696e 666f 5d0d  c....[egg_info].
+000002c0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+000002d0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `ecopipeline-0.0.4/src/ecopipeline/__init__.py` & `ecopipeline-0.0.5/src/ecopipeline/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .extract import get_noaa_data, json_to_df, extract_files, get_last_full_day_from_db, extract_new, csv_to_df, get_sub_dirs
-from .transform import rename_sensors, avg_duplicate_times, remove_outliers, ffill_missing, sensor_adjustment, get_energy_by_min, verify_power_energy, round_time, aggregate_df, join_to_hourly, concat_last_row, join_to_daily, get_temp_zones120, get_storage_gals120
+from .transform import rename_sensors, avg_duplicate_times, remove_outliers, ffill_missing, sensor_adjustment, get_energy_by_min, verify_power_energy, round_time, aggregate_df, join_to_hourly, concat_last_row, join_to_daily, get_temp_zones120, get_storage_gals120, cop_method_2
 from .load import get_login_info, connect_db, check_table_exists, create_new_table, load_database, load_overwrite_database
 from .lbnl import nclarity_filter_new, site_specific, condensate_calculations, gas_valve_diff, gather_outdoor_conditions, nclarity_csv_to_df, add_date, aqsuite_filter_new, get_refrig_charge, elev_correction, change_ID_to_HVAC, get_cop_values, get_cfm_values, replace_humidity, create_fan_curves, lbnl_temperature_conversions, lbnl_pressure_conversions, lbnl_sat_calculations
 from .bayview import calculate_cop_values, aggregate_values
 __all__ = ["get_last_full_day_from_db", "set_input", "set_output","get_noaa_data", "json_to_df", "extract_files", "avg_duplicate_times", "remove_outliers", "ffill_missing", "sensor_adjustment", "get_energy_by_min", "verify_power_energy",
            "set_data", "aggregate_values", "calculate_cop_values", "get_login_info", "connect_db", "check_table_exists", "create_new_table", "createUnknownColumns", "load_database", "load_overwrite_database", "rename_sensors", "round_time", "aggregate_df", 
-           "extract_new", "csv_to_df", "set_config", "get_sub_dirs", "join_to_hourly", "concat_last_row", "join_to_daily", "get_temp_zones120", "get_storage_gals120",  "site_specific", "condensate_calculations", "gas_valve_diff",
+           "extract_new", "csv_to_df", "set_config", "get_sub_dirs", "join_to_hourly", "concat_last_row", "join_to_daily", "get_temp_zones120", "get_storage_gals120", "cop_method_2",  "site_specific", "condensate_calculations", "gas_valve_diff",
            "nclarity_filter_new", "gather_outdoor_conditions", "nclarity_csv_to_df", "add_date", "aqsuite_filter_new", "elev_correction", "get_refrig_charge", "change_ID_to_HVAC", "get_cop_values", "get_cfm_values", "replace_humidity", "create_fan_curves", 
            "lbnl_temperature_conversions", "lbnl_pressure_conversions", "lbnl_sat_calculations"]
```

### Comparing `ecopipeline-0.0.4/src/ecopipeline/bayview.py` & `ecopipeline-0.0.5/src/ecopipeline/bayview.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.4/src/ecopipeline/config.py` & `ecopipeline-0.0.5/src/ecopipeline/config.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.4/src/ecopipeline/extract.py` & `ecopipeline-0.0.5/src/ecopipeline/extract.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.4/src/ecopipeline/lbnl.py` & `ecopipeline-0.0.5/src/ecopipeline/lbnl.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.4/src/ecopipeline/load.py` & `ecopipeline-0.0.5/src/ecopipeline/load.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.4/src/ecopipeline/transform.py` & `ecopipeline-0.0.5/src/ecopipeline/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -398,14 +398,48 @@
 
     except ZeroDivisionError:
         print("DIVIDED BY ZERO ERROR")
         return df
 
     return cop_values
 
+def cop_method_2(df: pd.DataFrame, cop_tm):
+    """
+    Performs COP calculation method 2 as deffined by Scott's whiteboard image
+    COP = COP_primary(ELEC_primary/ELEC_total) + COP_tm(ELEC_tm/ELEC_total)
+
+    Args: 
+        df (pd.DataFrame): Pandas DataFrame to add COP columns to
+        cop_tm (float): fixed COP value for temputure Maintenece system
+
+    Returns: 
+        pd.DataFrame: Pandas DataFrame with the added COP columns. 
+    """
+    columns_to_check = ['COP_Primary', 'PowerIn_HPWH1', 'PowerIn_SwingTank', 'PowerIn_Total']
+
+    missing_columns = [col for col in columns_to_check if col not in df.columns]
+
+    if missing_columns:
+        print('Cannot calculate COP as the following columns are missing from the DataFrame:', missing_columns)
+        return df
+    
+    # Create list of column names to sum
+    sum_cols = [col for col in df.columns if col.startswith('PowerIn_HPWH') or col == 'PowerIn_SecLoopPump']
+
+    if len(sum_cols) == 0:
+        print('Cannot calculate COP as the primary power columns (such as PowerIn_HPWH and PowerIn_SecLoopPump) are missing from the DataFrame')
+        return df
+
+    # Create new DataFrame with one column called 'PowerIn_Primary' that contains the sum of the specified columns
+    new_df = pd.DataFrame({'PowerIn_Primary': df[sum_cols].sum(axis=1)})
+
+    df['COP'] = (df['COP_Primary'] * (new_df['PowerIn_Primary']/df['PowerIn_Total'])) + (cop_tm * (df['PowerIn_SwingTank']/df['PowerIn_Total'])) # TODO confirm these values
+    return df
+
+
 # loops through a list of dateTime objects, compares if the date of that object matches the
 # date of the row name, which is also a dateTime object. If it matches, load_shift is True (happened that day)
 def _ls_helper(row, dt_list):
     """
     Function takes in a pandas series and a list of dates, then checks
     each entry in the series and if it matches a date in the list of dates,
     sets the series load_shift_day to True.
```

### Comparing `ecopipeline-0.0.4/src/ecopipeline/unit_convert.py` & `ecopipeline-0.0.5/src/ecopipeline/unit_convert.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.4/src/ecopipeline.egg-info/PKG-INFO` & `ecopipeline-0.0.5/src/ecopipeline.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.4
+Version: 0.0.5
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DataPipelinePackage
 
+## To Install the Package
+
+    $ pip install ecopipeline
+
 ## Functions in Data Pipeline package:
 ### extract.py
 - load raw JSON-formatted data into a dataframe
 - merge NOAA weather data with sensor data
 
 ### clean.py
 - remove outliers specified in the configuration file
```

