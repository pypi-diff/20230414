# Comparing `tmp/ecopipeline-0.0.5.tar.gz` & `tmp/ecopipeline-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecopipeline-0.0.5.tar", last modified: Thu Apr 13 22:45:55 2023, max compression
+gzip compressed data, was "ecopipeline-0.0.6.tar", last modified: Fri Apr 14 00:01:09 2023, max compression
```

## Comparing `ecopipeline-0.0.5.tar` & `ecopipeline-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 22:45:55.543100 ecopipeline-0.0.5/
--rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1086 2023-04-13 22:45:55.566088 ecopipeline-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-04-10 20:35:13.000000 ecopipeline-0.0.5/README.md
--rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      735 2023-04-13 22:45:55.609610 ecopipeline-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 22:45:53.807097 ecopipeline-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 22:45:54.975099 ecopipeline-0.0.5/src/ecopipeline/
--rw-rw-rw-   0        0        0     2060 2023-04-13 22:42:27.000000 ecopipeline-0.0.5/src/ecopipeline/__init__.py
--rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.5/src/ecopipeline/bayview.py
--rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.5/src/ecopipeline/config.py
--rw-rw-rw-   0        0        0    13858 2023-04-10 20:26:32.000000 ecopipeline-0.0.5/src/ecopipeline/extract.py
--rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.5/src/ecopipeline/lbnl.py
--rw-rw-rw-   0        0        0     9434 2023-04-10 18:47:39.000000 ecopipeline-0.0.5/src/ecopipeline/load.py
--rw-rw-rw-   0        0        0    29945 2023-04-13 22:42:27.000000 ecopipeline-0.0.5/src/ecopipeline/transform.py
--rw-rw-rw-   0        0        0     2696 2023-02-17 15:53:41.000000 ecopipeline-0.0.5/src/ecopipeline/unit_convert.py
-drwxrwxrwx   0        0        0        0 2023-04-13 22:45:55.331099 ecopipeline-0.0.5/src/ecopipeline.egg-info/
--rw-rw-rw-   0        0        0     1086 2023-04-13 22:45:53.000000 ecopipeline-0.0.5/src/ecopipeline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-04-13 22:45:53.000000 ecopipeline-0.0.5/src/ecopipeline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 22:45:53.000000 ecopipeline-0.0.5/src/ecopipeline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-04-13 22:45:53.000000 ecopipeline-0.0.5/src/ecopipeline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-13 22:45:53.000000 ecopipeline-0.0.5/src/ecopipeline.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 00:01:09.543626 ecopipeline-0.0.6/
+-rw-rw-rw-   0        0        0        0 2023-02-17 15:53:40.000000 ecopipeline-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1086 2023-04-14 00:01:09.625867 ecopipeline-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-04-10 20:35:13.000000 ecopipeline-0.0.6/README.md
+-rw-rw-rw-   0        0        0      108 2023-04-10 17:10:50.000000 ecopipeline-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      735 2023-04-14 00:01:09.839381 ecopipeline-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-10 17:18:28.000000 ecopipeline-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:01:01.287613 ecopipeline-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 00:01:06.191621 ecopipeline-0.0.6/src/ecopipeline/
+-rw-rw-rw-   0        0        0     2060 2023-04-13 22:42:27.000000 ecopipeline-0.0.6/src/ecopipeline/__init__.py
+-rw-rw-rw-   0        0        0     5746 2023-04-10 17:21:13.000000 ecopipeline-0.0.6/src/ecopipeline/bayview.py
+-rw-rw-rw-   0        0        0      809 2023-03-31 18:26:04.000000 ecopipeline-0.0.6/src/ecopipeline/config.py
+-rw-rw-rw-   0        0        0    13858 2023-04-10 20:26:32.000000 ecopipeline-0.0.6/src/ecopipeline/extract.py
+-rw-rw-rw-   0        0        0    24099 2023-04-10 17:21:39.000000 ecopipeline-0.0.6/src/ecopipeline/lbnl.py
+-rw-rw-rw-   0        0        0     9434 2023-04-10 18:47:39.000000 ecopipeline-0.0.6/src/ecopipeline/load.py
+-rw-rw-rw-   0        0        0    30210 2023-04-14 00:00:20.000000 ecopipeline-0.0.6/src/ecopipeline/transform.py
+-rw-rw-rw-   0        0        0     2696 2023-02-17 15:53:41.000000 ecopipeline-0.0.6/src/ecopipeline/unit_convert.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:01:09.087626 ecopipeline-0.0.6/src/ecopipeline.egg-info/
+-rw-rw-rw-   0        0        0     1086 2023-04-14 00:00:59.000000 ecopipeline-0.0.6/src/ecopipeline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-04-14 00:01:00.000000 ecopipeline-0.0.6/src/ecopipeline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 00:00:59.000000 ecopipeline-0.0.6/src/ecopipeline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-04-14 00:00:59.000000 ecopipeline-0.0.6/src/ecopipeline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 00:00:59.000000 ecopipeline-0.0.6/src/ecopipeline.egg-info/top_level.txt
```

### Comparing `ecopipeline-0.0.5/PKG-INFO` & `ecopipeline-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.5
+Version: 0.0.6
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ecopipeline-0.0.5/README.md` & `ecopipeline-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.5/setup.cfg` & `ecopipeline-0.0.6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 636f 7069 7065 6c69 6e65 0d0a   = ecopipeline..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 350d  version = 0.0.5.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 360d  version = 0.0.6.
 00000030: 0a61 7574 686f 7220 3d20 4e6f 6c61 6e20  .author = Nolan 
 00000040: 616e 6420 5355 2053 7475 6465 6e74 730d  and SU Students.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 6e6f 6c61 6e40 6563 6f74 6f70 652e 636f  nolan@ecotope.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2043 6f6e 7461 696e 7320 6675 6e63 7469   Contains functi
 00000090: 6f6e 7320 666f 7220 7573 6520 696e 2045  ons for use in E
```

### Comparing `ecopipeline-0.0.5/src/ecopipeline/__init__.py` & `ecopipeline-0.0.6/src/ecopipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.5/src/ecopipeline/bayview.py` & `ecopipeline-0.0.6/src/ecopipeline/bayview.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.5/src/ecopipeline/config.py` & `ecopipeline-0.0.6/src/ecopipeline/config.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.5/src/ecopipeline/extract.py` & `ecopipeline-0.0.6/src/ecopipeline/extract.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.5/src/ecopipeline/lbnl.py` & `ecopipeline-0.0.6/src/ecopipeline/lbnl.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.5/src/ecopipeline/load.py` & `ecopipeline-0.0.6/src/ecopipeline/load.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.5/src/ecopipeline/transform.py` & `ecopipeline-0.0.6/src/ecopipeline/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,22 +410,25 @@
     Args: 
         df (pd.DataFrame): Pandas DataFrame to add COP columns to
         cop_tm (float): fixed COP value for temputure Maintenece system
 
     Returns: 
         pd.DataFrame: Pandas DataFrame with the added COP columns. 
     """
-    columns_to_check = ['COP_Primary', 'PowerIn_HPWH1', 'PowerIn_SwingTank', 'PowerIn_Total']
+    columns_to_check = ['Temp_HPWH1Outlet', 'Flow_HPWH1', 'PowerIn_HPWH1', 'PowerIn_SwingTank', 'PowerIn_Total', 'Temp_CityWater'] # TODO what if there is only 1 HPWH?
 
     missing_columns = [col for col in columns_to_check if col not in df.columns]
 
     if missing_columns:
         print('Cannot calculate COP as the following columns are missing from the DataFrame:', missing_columns)
         return df
     
+    #calculate primary COP that is actually equipment COP
+    df['COP_Primary'] = energy_kwh_to_kbtu(df['Flow_HPWH1'], df['Temp_HPWH1Outlet']-df['Temp_CityWater']) / df['PowerIn_HPWH1']
+    
     # Create list of column names to sum
     sum_cols = [col for col in df.columns if col.startswith('PowerIn_HPWH') or col == 'PowerIn_SecLoopPump']
 
     if len(sum_cols) == 0:
         print('Cannot calculate COP as the primary power columns (such as PowerIn_HPWH and PowerIn_SecLoopPump) are missing from the DataFrame')
         return df
```

### Comparing `ecopipeline-0.0.5/src/ecopipeline/unit_convert.py` & `ecopipeline-0.0.6/src/ecopipeline/unit_convert.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.0.5/src/ecopipeline.egg-info/PKG-INFO` & `ecopipeline-0.0.6/src/ecopipeline.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.0.5
+Version: 0.0.6
 Summary: Contains functions for use in Ecotope Datapipelines
 Author: Nolan and SU Students
 Author-email: nolan@ecotope.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

