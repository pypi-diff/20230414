# Comparing `tmp/xlsmloader-1.0.1.tar.gz` & `tmp/xlsmloader-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlsmloader-1.0.1.tar", last modified: Mon Mar 27 00:53:10 2023, max compression
+gzip compressed data, was "xlsmloader-1.0.2.tar", last modified: Thu Apr 13 23:30:23 2023, max compression
```

## Comparing `xlsmloader-1.0.1.tar` & `xlsmloader-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-03-27 00:53:10.580512 xlsmloader-1.0.1/
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1084 2023-03-13 12:23:28.000000 xlsmloader-1.0.1/LICENSE
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1097 2023-03-26 14:58:23.000000 xlsmloader-1.0.1/MIT
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1480 2023-03-27 00:53:10.580512 xlsmloader-1.0.1/PKG-INFO
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)       13 2023-03-13 13:48:03.000000 xlsmloader-1.0.1/README.md
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)      604 2023-03-27 00:53:02.000000 xlsmloader-1.0.1/pyproject.toml
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)       38 2023-03-27 00:53:10.580512 xlsmloader-1.0.1/setup.cfg
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1121 2023-03-27 00:42:14.000000 xlsmloader-1.0.1/setup.py
-drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-03-27 00:53:10.580512 xlsmloader-1.0.1/src/
-drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-03-27 00:53:10.580512 xlsmloader-1.0.1/src/xlsmloader/
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)       50 2023-03-27 00:51:53.000000 xlsmloader-1.0.1/src/xlsmloader/__init__.py
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)       70 2023-03-26 14:27:02.000000 xlsmloader-1.0.1/src/xlsmloader/__main__.py
-drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-03-27 00:53:10.580512 xlsmloader-1.0.1/src/xlsmloader/commons/
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)        0 2023-03-26 13:50:15.000000 xlsmloader-1.0.1/src/xlsmloader/commons/__init__.py
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)      477 2023-03-25 19:07:56.000000 xlsmloader-1.0.1/src/xlsmloader/commons/converters.py
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     5066 2023-03-12 14:30:06.000000 xlsmloader-1.0.1/src/xlsmloader/commons/openpyxl_wo_formatting.py
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1664 2023-03-26 14:06:08.000000 xlsmloader-1.0.1/src/xlsmloader/commons/utils.py
-drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-03-27 00:53:10.580512 xlsmloader-1.0.1/src/xlsmloader/loader/
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)        0 2023-03-27 00:13:05.000000 xlsmloader-1.0.1/src/xlsmloader/loader/__init__.py
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1917 2023-03-26 14:24:23.000000 xlsmloader-1.0.1/src/xlsmloader/loader/loader.py
-drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-03-27 00:53:10.580512 xlsmloader-1.0.1/src/xlsmloader/models/
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)        0 2023-03-26 13:50:04.000000 xlsmloader-1.0.1/src/xlsmloader/models/__init__.py
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     3898 2023-03-25 20:11:02.000000 xlsmloader-1.0.1/src/xlsmloader/models/assets.py
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1789 2023-03-25 18:09:16.000000 xlsmloader-1.0.1/src/xlsmloader/models/photos.py
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     7220 2023-03-26 13:25:29.000000 xlsmloader-1.0.1/src/xlsmloader/models/systems.py
-drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-03-27 00:53:10.580512 xlsmloader-1.0.1/src/xlsmloader.egg-info/
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1480 2023-03-27 00:53:10.000000 xlsmloader-1.0.1/src/xlsmloader.egg-info/PKG-INFO
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)      679 2023-03-27 00:53:10.000000 xlsmloader-1.0.1/src/xlsmloader.egg-info/SOURCES.txt
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)        1 2023-03-27 00:53:10.000000 xlsmloader-1.0.1/src/xlsmloader.egg-info/dependency_links.txt
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)       61 2023-03-27 00:53:10.000000 xlsmloader-1.0.1/src/xlsmloader.egg-info/entry_points.txt
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)      146 2023-03-27 00:53:10.000000 xlsmloader-1.0.1/src/xlsmloader.egg-info/requires.txt
--rw-rw-r--   0 paulosales  (1000) paulosales  (1000)       11 2023-03-27 00:53:10.000000 xlsmloader-1.0.1/src/xlsmloader.egg-info/top_level.txt
+drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-04-13 23:30:23.886394 xlsmloader-1.0.2/
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1084 2023-03-13 12:23:28.000000 xlsmloader-1.0.2/LICENSE
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1097 2023-03-26 14:58:23.000000 xlsmloader-1.0.2/MIT
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1540 2023-04-13 23:30:23.886394 xlsmloader-1.0.2/PKG-INFO
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)       73 2023-04-13 14:26:06.000000 xlsmloader-1.0.2/README.md
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)      604 2023-04-13 23:28:59.000000 xlsmloader-1.0.2/pyproject.toml
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)       38 2023-04-13 23:30:23.886394 xlsmloader-1.0.2/setup.cfg
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)      769 2023-04-13 23:30:16.000000 xlsmloader-1.0.2/setup.py
+drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-04-13 23:30:23.882394 xlsmloader-1.0.2/src/
+drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-04-13 23:30:23.886394 xlsmloader-1.0.2/src/commons/
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)        0 2023-03-26 13:50:15.000000 xlsmloader-1.0.2/src/commons/__init__.py
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)      559 2023-04-01 13:27:15.000000 xlsmloader-1.0.2/src/commons/converters.py
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     5066 2023-03-28 11:13:33.000000 xlsmloader-1.0.2/src/commons/openpyxl_wo_formatting.py
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     3836 2023-04-04 23:30:12.000000 xlsmloader-1.0.2/src/commons/utils.py
+drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-04-13 23:30:23.886394 xlsmloader-1.0.2/src/loader/
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)        0 2023-03-27 00:13:05.000000 xlsmloader-1.0.2/src/loader/__init__.py
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     3118 2023-03-31 12:49:04.000000 xlsmloader-1.0.2/src/loader/loader.py
+drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-04-13 23:30:23.886394 xlsmloader-1.0.2/src/models/
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)        0 2023-03-26 13:50:04.000000 xlsmloader-1.0.2/src/models/__init__.py
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     4359 2023-04-04 23:34:04.000000 xlsmloader-1.0.2/src/models/assets.py
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1789 2023-03-25 18:09:16.000000 xlsmloader-1.0.2/src/models/photos.py
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     7516 2023-04-01 14:26:03.000000 xlsmloader-1.0.2/src/models/systems.py
+drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-04-13 23:30:23.886394 xlsmloader-1.0.2/src/xlsmloader.egg-info/
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1540 2023-04-13 23:30:23.000000 xlsmloader-1.0.2/src/xlsmloader.egg-info/PKG-INFO
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)      651 2023-04-13 23:30:23.000000 xlsmloader-1.0.2/src/xlsmloader.egg-info/SOURCES.txt
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)        1 2023-04-13 23:30:23.000000 xlsmloader-1.0.2/src/xlsmloader.egg-info/dependency_links.txt
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)       50 2023-04-13 23:30:23.000000 xlsmloader-1.0.2/src/xlsmloader.egg-info/entry_points.txt
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)      146 2023-04-13 23:30:23.000000 xlsmloader-1.0.2/src/xlsmloader.egg-info/requires.txt
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)       22 2023-04-13 23:30:23.000000 xlsmloader-1.0.2/src/xlsmloader.egg-info/top_level.txt
+drwxrwxr-x   0 paulosales  (1000) paulosales  (1000)        0 2023-04-13 23:30:23.886394 xlsmloader-1.0.2/tests/
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     1028 2023-04-13 23:19:51.000000 xlsmloader-1.0.2/tests/test_extract_asset_name.py
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)      476 2023-04-13 23:19:45.000000 xlsmloader-1.0.2/tests/test_is_site.py
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)      979 2023-04-13 23:19:58.000000 xlsmloader-1.0.2/tests/test_parse_asset_floors.py
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)     2845 2023-04-13 23:20:08.000000 xlsmloader-1.0.2/tests/test_sanitize.py
+-rw-rw-r--   0 paulosales  (1000) paulosales  (1000)      722 2023-04-13 23:20:15.000000 xlsmloader-1.0.2/tests/test_sql_escape.py
```

### Comparing `xlsmloader-1.0.1/LICENSE` & `xlsmloader-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xlsmloader-1.0.1/MIT` & `xlsmloader-1.0.2/MIT`

 * *Files identical despite different names*

### Comparing `xlsmloader-1.0.1/PKG-INFO` & `xlsmloader-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlsmloader
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://xlsmloader.pypa.io/
 Author: Paulo Rogerio Sales Santos
 Author-email: Paulo Rogério Sales Santos <paulosales@gmail.com>
 License: Copyright 2023 Paulo Rogério Sales Santos - paulosales@gmail.com
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -13,7 +13,14 @@
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Keywords: xlsm,reader,assets,sql
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # xlsmloader
+
+## Pre-requisites
+
+Python 3 installed.
+
+## How to install
+
```

### Comparing `xlsmloader-1.0.1/pyproject.toml` & `xlsmloader-1.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "xlsmloader"
-version = "1.0.1"
+version = "1.0.2"
 description = ""
 readme = "README.md"
 authors = [{ name = "Paulo Rogério Sales Santos", email = "paulosales@gmail.com" }]
 license = { file = "MIT" }
 keywords = ["xlsm", "reader", "assets", "sql"]
 
 dependencies = [
```

### Comparing `xlsmloader-1.0.1/setup.py` & `xlsmloader-1.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,32 +5,24 @@
 def read(rel_path: str) -> str:
     here = os.path.abspath(os.path.dirname(__file__))
     # intentionally *not* adding an encoding option to open, See:
     #   https://github.com/pypa/virtualenv/issues/201#issuecomment-3145690
     with open(os.path.join(here, rel_path)) as fp:
         return fp.read()
 
-def get_version(rel_path: str) -> str:
-    for line in read(rel_path).splitlines():
-        if line.startswith("__version__"):
-            # __version__ = "0.9"
-            delim = '"' if '"' in line else "'"
-            return line.split(delim)[1]
-    raise RuntimeError("Unable to find version string.")
-
 setup(
     name='xlsmloader',
-    version=get_version("src/xlsmloader/__init__.py"),
+    version="1.0.2",
     author="Paulo Rogerio Sales Santos",
     author_email="paulosales@gmail.com",
     package_dir={"": "src"},
     packages=find_packages(
         where="src",
     ),
     url="https://xlsmloader.pypa.io/",
     entry_points={
         "console_scripts": [
-            "xlsmloader=xlsmloader.loader.loader:load",
+            "xlsmloader=loader.loader:load",
         ],
     },
     python_requires=">=3.7",
 )
```

### Comparing `xlsmloader-1.0.1/src/xlsmloader/commons/openpyxl_wo_formatting.py` & `xlsmloader-1.0.2/src/commons/openpyxl_wo_formatting.py`

 * *Files identical despite different names*

### Comparing `xlsmloader-1.0.1/src/xlsmloader/loader/loader.py` & `xlsmloader-1.0.2/src/loader/loader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,73 @@
 import glob
 import sys
 import warnings
+import os
+import traceback
 from datetime import datetime, timedelta
 from commons.utils import generate_log_filename, current_milli_time
 import commons.openpyxl_wo_formatting as openpyxl_wo_formatting
 from models.assets import Asset
 from models.systems import System
 from models.photos import Photo
 
+RED = "\033[1;31m"
+RESET = "\033[0;0m"
+MAX_SPREADSHEETS_PER_SQL_FILE = 20;
+
 warnings.simplefilter("ignore", category=UserWarning)
 
 def load():
     if len(sys.argv) <= 1:
         directory_path = input("Inform the XLSM file directory: ")
     else:
         directory_path = sys.argv[1]
 
     start_time_ms = current_milli_time()
     print(f"Processing start time {datetime.now()}")
     print(f"processing XLSM files from {directory_path}")
     xlsm_files = glob.glob(directory_path + '/*.xlsm')
     print(f"{len(xlsm_files)} files found.")
 
-    with open(generate_log_filename(), "w") as sql_file:
-        sql_file.write("DECLARE\n")
-        sql_file.write("  description_clob CLOB;\n")
-        sql_file.write("  asset_id number;\n")
-        sql_file.write("  system_id number;\n")
-        sql_file.write("BEGIN\n")
-        for workbook_filename in xlsm_files:
-            print(f"reading file {workbook_filename}...")
-            asset = Asset(workbook_filename)
-            system = System(workbook_filename, asset)
-            photo = Photo(workbook_filename, asset)
-            sql_file.write(asset.create_update_sql())
-            sql_file.write("\r\n\n")
-            sql_file.write(system.create_update_sql())
-            sql_file.write("\r\n\n")
-            sql_file.write(photo.create_insert_sql())
-            sql_file.write("\r\n")
-        sql_file.write("  COMMIT;\n")
-        sql_file.write("END;\n")
-        sql_file.close()
+    for subset_index in range(0, len(xlsm_files), MAX_SPREADSHEETS_PER_SQL_FILE):
+        with open(generate_log_filename(subset_index // MAX_SPREADSHEETS_PER_SQL_FILE), "w") as sql_file:
+            sql_file.write("DECLARE\n")
+            sql_file.write("  description_clob CLOB;\n")
+            sql_file.write("  asset_id number;\n")
+            sql_file.write("  system_id number;\n")
+            sql_file.write("  count_systems number;\n")
+            sql_file.write("BEGIN\n")
+            for workbook_filename in xlsm_files[subset_index:subset_index+MAX_SPREADSHEETS_PER_SQL_FILE]:
+                try:
+                    print(f"reading file {os.path.basename(workbook_filename)}...")
+                    asset = Asset(workbook_filename)
+                    system = System(workbook_filename, asset)
+                    photo = Photo(workbook_filename, asset)
+                    asset.setSystem(system)
+
+                    asset_sql = asset.create_update_sql()
+                    system_sql = system.create_update_sql()
+                    photo_sql = photo.create_insert_sql()
+
+                    sql_file.write(f"  -- {os.path.basename(workbook_filename)} data\r\n\n")
+                    sql_file.write(asset_sql)
+                    sql_file.write("\r\n\n")
+                    sql_file.write(system_sql)
+                    sql_file.write("\r\n\n")
+                    sql_file.write(photo_sql)
+                    sql_file.write("\r\n")
+                    print(f"file {os.path.basename(workbook_filename)} processed successfully.")
+                except (BaseException) as e:
+                    error_message = f"File {os.path.basename(workbook_filename)} processed with error: {e}."
+                    tb_info = traceback.format_exc()
+                    print(f"{RED}{error_message}{RESET}", file=sys.stderr)
+                    print(tb_info, file=sys.stderr)
+
+            sql_file.write("  COMMIT;\n")
+            sql_file.write("END;\n")
+            sql_file.close()
 
     print(f"Processing finished time {datetime.now()}")
     end_time_ms = current_milli_time()
     elapsed_time_ms = end_time_ms - start_time_ms
     elapsed_time = timedelta(milliseconds=elapsed_time_ms)
     print(f"Elapsed time: {elapsed_time}")
```

### Comparing `xlsmloader-1.0.1/src/xlsmloader/models/assets.py` & `xlsmloader-1.0.2/src/models/assets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,66 @@
-from commons.utils import to_excel_date, split_oracle_string
+from commons.utils import to_excel_date, split_oracle_string, remove_chars
 import pandas as pd
-from commons.utils import sanitize
+from commons.utils import sanitize, to_canonical_date_format, parse_asset_floors, is_valid_asset_id, is_site, extract_asset_name
 from commons.converters import province_converter
 
 
 class Asset:
     
     def __init__(self, workbook_filename) -> None:
+        self.system = None
+        self.is_a_site = is_site(workbook_filename)
         self.__background_worksheet = pd.read_excel(
             workbook_filename,
             engine='openpyxl_wo_formatting',
             skiprows=0,
             sheet_name='Background'
         );
 
+    def load(self):
         row_offset = 0;
         self.region = self.__background_worksheet.iloc[row_offset+5, 3]
         self.campus = self.__background_worksheet.iloc[row_offset+6, 3]
         number_and_name = self.__background_worksheet.iloc[row_offset+7,3]
-        self.name = number_and_name.split("-")[1].strip()
+        self.name = extract_asset_name(number_and_name)
         self.number = self.__background_worksheet.iloc[row_offset+10,3]
         self.eid = self.__background_worksheet.iloc[row_offset+9,3]
         self.description = self.__background_worksheet.iloc[row_offset+5,10]
         self.size = self.__background_worksheet.iloc[row_offset+22,3]
         self.size_units = self.__background_worksheet.iloc[row_offset+22,4]
-        self.year_constructed = self.__background_worksheet.iloc[row_offset+23,3]
+        self.year_constructed = remove_chars(self.__background_worksheet.iloc[row_offset+23,3])
         self.type = self.__background_worksheet.iloc[row_offset+24,3]
         self.use = self.__background_worksheet.iloc[row_offset+25,3]
         self.ocupancy = self.__background_worksheet.iloc[row_offset+26,3]
-        self.stories = self.__background_worksheet.iloc[row_offset+27,3]
+        self.stories = parse_asset_floors(self.__background_worksheet.iloc[row_offset+27,3])
         self.address_line_1 = self.__background_worksheet.iloc[row_offset+28,3]
         self.address_line_2 = self.__background_worksheet.iloc[row_offset+29,3]
         self.city = self.__background_worksheet.iloc[row_offset+30,3]
         self.province = province_converter(self.__background_worksheet.iloc[row_offset+31,3])
         self.postal_code = self.__background_worksheet.iloc[row_offset+32,3]
-        self.date_of_assessment = to_excel_date(self.__background_worksheet.iloc[row_offset+34,3])
+        self.date_of_assessment = to_canonical_date_format(to_excel_date(self.__background_worksheet.iloc[row_offset+34,3]))
         self.country = "CA"
         self.currency = "CAD"
 
+        if not is_valid_asset_id(self.eid) and self.system != None:
+            self.eid = self.system.get_asset_id()
+    
+    def setSystem(self, system):
+        self.system = system
+
     def create_update_sql(self):
+        self.load()
         description_chuncks = split_oracle_string(self.description, 1000)
         if len(description_chuncks) == 0:
             description_chuncks = ['']
 
         sql = (
             f"  UPDATE ASSETS SET\n" +
             f"    ASSET_NUMBER = {sanitize(self.number)},\n" +
-            f"    NAME = {sanitize(self.name)},\n    DESCRIPTION = {sanitize(description_chuncks[0])},\n" + 
+            f"    NAME = {sanitize(self.name)},\n    DESCRIPTION = {description_chuncks[0]},\n" + 
             f"    ASSET_SIZE = {sanitize(self.size)},\n    SIZE_UNITS = {sanitize(self.size_units)},\n" + 
             f"    YEAR_CONSTRUCTED = {self.year_constructed},\n    ASSET_TYPE = {sanitize(self.type)},\n" +
             f"    ASSET_USE = {sanitize(self.use)},\n    ASSET_OCCUPANCY = {sanitize(self.ocupancy)},\n" +
             f"    STORIES = {sanitize(self.stories)},\n    ADDRESS_LINE_1 = {sanitize(self.address_line_1)},\n" +
             f"    ADDRESS_LINE_2 = {sanitize(self.address_line_2)},\n    CITY = {sanitize(self.city)},\n" +
             f"    PROVINCE = {sanitize(self.province)},\n    POSTAL_CODE = {sanitize(self.postal_code)},\n" +
             f"    COUNTRY = {sanitize(self.country)},\n    CURRENCY = {sanitize(self.currency)},\n" +
```

### Comparing `xlsmloader-1.0.1/src/xlsmloader/models/photos.py` & `xlsmloader-1.0.2/src/models/photos.py`

 * *Files identical despite different names*

### Comparing `xlsmloader-1.0.1/src/xlsmloader/models/systems.py` & `xlsmloader-1.0.2/src/models/systems.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from commons.utils import to_excel_datetime, split_oracle_string
 import pandas as pd
 import math
-from commons.utils import sanitize
+from commons.utils import sanitize, to_canonical_date_format, to_excel_datetime, split_oracle_string
 from commons.converters import requeriment_type_converter
 
 class System:
     def __init__(self, workbook_filename, asset) -> None:
+        self.asset = asset
         self.__bca_worksheet = pd.read_excel(
             workbook_filename,
             engine='openpyxl_wo_formatting',
             header=None,
             skiprows=0,
             sheet_name='BCA Worksheet'
         );
 
+    def load(self):
         row_offset = 0;
         self.systems = []
         eid = self.__bca_worksheet.iloc[row_offset+4,0]
         self.load_system_data(row_offset, eid)
         while self.has_system_data(eid):
             self.systems.append({
-                "asset": asset,
+                "asset": self.asset,
                 "eid": eid,
                 "name": self.__name,
                 "uniformat": self.__uniformat,
                 "uniformat_code": self.__uniformat_code,
                 "description": self.__description,
                 "year_installed": self.__year_installed,
                 "lifetime": self.__lifetime,
@@ -53,27 +54,27 @@
         return eid != None and eid != "" and not (type(eid) == float and math.isnan(eid))
 
     def load_system_data(self, row_offset, eid):
         if(self.has_system_data(eid)):
             self.__uniformat = self.__bca_worksheet.iloc[row_offset+4,5]
             self.__uniformat_code = self.__uniformat.split("-")[0].strip()
             self.__name = self.__bca_worksheet.iloc[row_offset+4,8]
-            self.__description = self.__bca_worksheet.iloc[row_offset+4,9]
+            self.__description = self.__bca_worksheet.iloc[row_offset+4,10]
             if type(self.__description) == float:
                 self.__description = ""
             self.__current_year = int(self.__bca_worksheet.iloc[0,7])
             self.__year_installed = self.__bca_worksheet.iloc[row_offset+4,13]
             self.__lifetime = self.__bca_worksheet.iloc[row_offset+4,14]
             self.__requirement_type = requeriment_type_converter(self.__bca_worksheet.iloc[row_offset+4,15])
             self.__requirement_action_item = self.__bca_worksheet.iloc[row_offset+4,18]
             self.__quantity = float(self.__bca_worksheet.iloc[row_offset+4, 19])
             self.__unit = self.__bca_worksheet.iloc[row_offset+4, 20]
             self.__unit_cost = float(self.__bca_worksheet.iloc[row_offset+4, 21])
             self.__percent_renew = self.__bca_worksheet.iloc[row_offset+4,22]
-            self.__date_inspected = to_excel_datetime(self.__bca_worksheet.iloc[row_offset+4,32])
+            self.__date_inspected = to_canonical_date_format(to_excel_datetime(self.__bca_worksheet.iloc[row_offset+4,32]))
             self.__inspector = self.__bca_worksheet.iloc[row_offset+4,36]
             self.__adjustment_factor = float(self.__bca_worksheet.iloc[row_offset+4, 25])
             self.__years_remaining = self.__bca_worksheet.iloc[row_offset+4,16]
             if self.__requirement_type != None:
                 if self.__requirement_type.upper() == "LIFECYCLE":
                     self.__replacement_cost = float(self.__bca_worksheet.iloc[row_offset+4, 26])
                     self.__renewal_cost = None
@@ -84,57 +85,62 @@
                     self.__replacement_cost = None
                     self.__renewal_cost = None
             else:
                 self.__replacement_cost = None
                 self.__renewal_cost = None
 
     def create_update_sql(self):
+        self.load()
         sqls = []
         for sys in self.systems:
             description_chuncks = split_oracle_string(sys['description'], 1000)
             if len(description_chuncks) == 0:
                 description_chuncks = ['']
 
+            inspected_date = sanitize(sys['date_inspected']);
+            
             sql = (
-                f"  UPDATE SYSTEMS SET\n" +
-                f"    ASSET_ID = asset_id,\n" +
-                f"    UNIFORMAT_CODE = {sanitize(sys['uniformat_code'])},\n" +
-                f"    UNIFORMAT = {sanitize(sys['uniformat'])},\n    NAME = {sanitize(sys['name'])},\n" +
-                f"    DESCRIPTION = {sanitize(description_chuncks[0])},\n    YEAR_INSTALLED = {sanitize(sys['year_installed'])},\n" +
-                f"    LIFETIME = {sanitize(sys['lifetime'])},\n    YEARS_REMAINING = {sys['years_remaining']},\n" +
-                f"    QUANTITY = {sanitize(sys['quantity'])},\n    UNIT = {sanitize(sys['unit'])},\n" +
-                f"    UNIT_COST = {sanitize(sys['unit_cost'])},\n    PERCENT_RENEW = {sanitize(sys['percent_renew'])},\n" +
-                f"    ADJUSTMENT_FACTOR = {sanitize(sys['adjustment_factor'])},\n" +
-                f"    DATE_INSPECTED = TO_DATE({sanitize(sys['date_inspected'])}, 'MM/DD/YYYY'),\n" +
-                f"    INSPECTOR = {sanitize(sys['inspector'])},\n    RENEWAL_COST = {sanitize(sys['renewal_cost'])},\n" +
-                f"    REPLACEMENT_COST = {sanitize(sys['replacement_cost'])}\n"
-                f"  WHERE EID = {sanitize(sys['eid'])}\n" +
-                f"  RETURNING DESCRIPTION\n" +
-                f"  INTO description_clob;\n\n"
+                f"  SELECT count(id) INTO count_systems FROM SYSTEMS WHERE EID = {sanitize(sys['eid'])};\n\n" +
+                "   IF count_systems > 0 THEN\n"+
+                f"    UPDATE SYSTEMS SET\n" +
+                f"      ASSET_ID = asset_id,\n" +
+                f"      UNIFORMAT_CODE = {sanitize(sys['uniformat_code'])},\n" +
+                f"      UNIFORMAT = {sanitize(sys['uniformat'])},\n      NAME = {sanitize(sys['name'])},\n" +
+                f"      DESCRIPTION = {description_chuncks[0]},\n      YEAR_INSTALLED = {sanitize(sys['year_installed'])},\n" +
+                f"      LIFETIME = {sanitize(sys['lifetime'])},\n      YEARS_REMAINING = {sys['years_remaining']},\n" +
+                f"      QUANTITY = {sanitize(sys['quantity'])},\n      UNIT = {sanitize(sys['unit'])},\n" +
+                f"      UNIT_COST = {sanitize(sys['unit_cost'])},\n      PERCENT_RENEW = {sanitize(sys['percent_renew'])},\n" +
+                f"      ADJUSTMENT_FACTOR = {sanitize(sys['adjustment_factor'])},\n" +
+                (f"      DATE_INSPECTED = TO_DATE({inspected_date}, 'MM/DD/YYYY'),\n" if inspected_date != "'null'" else "") +
+                f"      INSPECTOR = {sanitize(sys['inspector'])},\n      RENEWAL_COST = {sanitize(sys['renewal_cost'])},\n" +
+                f"      REPLACEMENT_COST = {sanitize(sys['replacement_cost'])}\n"
+                f"    WHERE EID = {sanitize(sys['eid'])}\n" +
+                f"    RETURNING DESCRIPTION\n" +
+                f"    INTO description_clob;\n\n"
             )
 
             del description_chuncks[0]
 
             for chunck in description_chuncks:
                 sql = sql + (
-                    f"  DBMS_LOB.writeappend(\n" +
-                    f"    description_clob,\n" +
-                    f"    LENGTH ({chunck}),\n" +
-                    f"    {chunck}\n" +
-                    f"  );\n\n"
+                    f"    DBMS_LOB.writeappend(\n" +
+                    f"      description_clob,\n" +
+                    f"      LENGTH ({chunck}),\n" +
+                    f"      {chunck}\n" +
+                    f"    );\n\n"
                 )
 
-            sql = sql + f"  SELECT id INTO system_id FROM SYSTEMS WHERE EID = {sanitize(sys['eid'])};\n\n";
-
-            sql = sql + f"  UPDATE REQUIREMENTS r SET r.NAME = '[LEGACY] ' || r.NAME\n"
-            sql = sql + f"  WHERE SYSTEM_ID = system_id\n"
-            sql = sql + f"  AND SUBSTR(r.NAME, 1, 8) <> '[LEGACY]';\n\n"
-
-            sql = sql + f"  UPDATE PHOTOS p SET p.CAPTION = '[LEGACY] ' || p.CAPTION\n"
-            sql = sql + f"  WHERE ASSET_ID = asset_id\n"
-            sql = sql + f"  AND SUBSTR(p.CAPTION, 1, 8) <> '[LEGACY]';\n\n"
-
-            sql = sql + f"  INSERT INTO REQUIREMENTS(SYSTEM_ID, REQUIREMENT_TYPE, ACTION_YEAR)\n"
-            sql = sql + f"  VALUES(system_id, {sanitize(sys['requirement_type'])}, {sanitize(sys['requirement_action_item'])});\n\n"
+            sql = sql + f"    SELECT id INTO system_id FROM SYSTEMS WHERE EID = {sanitize(sys['eid'])};\n\n";
 
+            sql = sql + f"    UPDATE REQUIREMENTS r SET r.NAME = '[LEGACY] ' || r.NAME\n"
+            sql = sql + f"    WHERE SYSTEM_ID = system_id\n"
+            sql = sql + f"    AND SUBSTR(r.NAME, 1, 8) <> '[LEGACY]';\n\n"
+
+            sql = sql + f"    UPDATE PHOTOS p SET p.CAPTION = '[LEGACY] ' || p.CAPTION\n"
+            sql = sql + f"    WHERE ASSET_ID = asset_id\n"
+            sql = sql + f"    AND SUBSTR(p.CAPTION, 1, 8) <> '[LEGACY]';\n"
+            sql = sql + f"  END IF;\n\n"
             sqls.append(sql)
         return "\n\n".join(sqls);
+
+    def get_asset_id(self):
+        return self.__bca_worksheet.iloc[4,1]
```

### Comparing `xlsmloader-1.0.1/src/xlsmloader.egg-info/PKG-INFO` & `xlsmloader-1.0.2/src/xlsmloader.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlsmloader
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://xlsmloader.pypa.io/
 Author: Paulo Rogerio Sales Santos
 Author-email: Paulo Rogério Sales Santos <paulosales@gmail.com>
 License: Copyright 2023 Paulo Rogério Sales Santos - paulosales@gmail.com
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -13,7 +13,14 @@
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Keywords: xlsm,reader,assets,sql
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # xlsmloader
+
+## Pre-requisites
+
+Python 3 installed.
+
+## How to install
+
```

