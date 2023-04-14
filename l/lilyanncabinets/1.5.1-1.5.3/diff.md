# Comparing `tmp/lilyanncabinets-1.5.1.tar.gz` & `tmp/lilyanncabinets-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lilyanncabinets-1.5.1.tar", last modified: Tue Apr 11 08:05:03 2023, max compression
+gzip compressed data, was "lilyanncabinets-1.5.3.tar", last modified: Fri Apr 14 16:12:38 2023, max compression
```

## Comparing `lilyanncabinets-1.5.1.tar` & `lilyanncabinets-1.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 08:05:03.659424 lilyanncabinets-1.5.1/
--rw-rw-rw-   0        0        0        0 2023-03-27 21:28:54.000000 lilyanncabinets-1.5.1/LICENSE
--rw-rw-rw-   0        0        0     1487 2023-04-11 08:05:03.659424 lilyanncabinets-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1011 2023-04-11 08:04:47.000000 lilyanncabinets-1.5.1/README.md
--rw-rw-rw-   0        0        0      108 2023-03-27 21:24:36.000000 lilyanncabinets-1.5.1/pyproject.toml
--rw-rw-rw-   0        0        0      607 2023-04-11 08:05:03.664423 lilyanncabinets-1.5.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 08:05:03.636422 lilyanncabinets-1.5.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 08:05:03.643422 lilyanncabinets-1.5.1/src/lilyanncabinets/
--rw-rw-rw-   0        0        0        0 2023-03-27 21:30:52.000000 lilyanncabinets-1.5.1/src/lilyanncabinets/__init__.py
--rw-rw-rw-   0        0        0      212 2023-03-30 15:10:59.000000 lilyanncabinets-1.5.1/src/lilyanncabinets/main.py
--rw-rw-rw-   0        0        0      777 2023-04-11 07:55:31.000000 lilyanncabinets-1.5.1/src/lilyanncabinets/sheets.py
-drwxrwxrwx   0        0        0        0 2023-04-11 08:05:03.658424 lilyanncabinets-1.5.1/src/lilyanncabinets.egg-info/
--rw-rw-rw-   0        0        0     1487 2023-04-11 08:05:03.000000 lilyanncabinets-1.5.1/src/lilyanncabinets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-11 08:05:03.000000 lilyanncabinets-1.5.1/src/lilyanncabinets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 08:05:03.000000 lilyanncabinets-1.5.1/src/lilyanncabinets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-11 08:05:03.000000 lilyanncabinets-1.5.1/src/lilyanncabinets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 16:12:38.638998 lilyanncabinets-1.5.3/
+-rw-rw-rw-   0        0        0        0 2023-03-27 21:28:54.000000 lilyanncabinets-1.5.3/LICENSE
+-rw-rw-rw-   0        0        0     1939 2023-04-14 16:12:38.638998 lilyanncabinets-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1463 2023-04-14 16:12:29.000000 lilyanncabinets-1.5.3/README.md
+-rw-rw-rw-   0        0        0      108 2023-03-27 21:24:36.000000 lilyanncabinets-1.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0      607 2023-04-14 16:12:38.639999 lilyanncabinets-1.5.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 16:12:38.616676 lilyanncabinets-1.5.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 16:12:38.630998 lilyanncabinets-1.5.3/src/lilyanncabinets/
+-rw-rw-rw-   0        0        0        0 2023-03-27 21:30:52.000000 lilyanncabinets-1.5.3/src/lilyanncabinets/__init__.py
+-rw-rw-rw-   0        0        0      212 2023-03-30 15:10:59.000000 lilyanncabinets-1.5.3/src/lilyanncabinets/main.py
+-rw-rw-rw-   0        0        0      895 2023-04-14 16:00:37.000000 lilyanncabinets-1.5.3/src/lilyanncabinets/sheets.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:12:38.638998 lilyanncabinets-1.5.3/src/lilyanncabinets.egg-info/
+-rw-rw-rw-   0        0        0     1939 2023-04-14 16:12:38.000000 lilyanncabinets-1.5.3/src/lilyanncabinets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-14 16:12:38.000000 lilyanncabinets-1.5.3/src/lilyanncabinets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 16:12:38.000000 lilyanncabinets-1.5.3/src/lilyanncabinets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-14 16:12:38.000000 lilyanncabinets-1.5.3/src/lilyanncabinets.egg-info/top_level.txt
```

### Comparing `lilyanncabinets-1.5.1/PKG-INFO` & `lilyanncabinets-1.5.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 Metadata-Version: 2.1
 Name: lilyanncabinets
-Version: 1.5.1
+Version: 1.5.3
 Summary: Package for use by Lily Ann Cabinets
 Home-page: https://github.com/JosephCaligiuri/lilyanncabinets
 Author: Joseph Caligiuri
 Author-email: jcaligiuri1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Version 1.5.1
+Current Version: 1.5.3
 
-patch notes: 
-===========================================================================
-- [1.5.1]: "Creating a new "build" added an auto spreadsheet creating and updating function for use with both robot and manual data tracking, 
+Patch Notes: 
+
+===================================================================================================
+
+[1.5.3]: Fixed patchnotes formating 
+
+===================================================================================================
+
+[1.5.2]: Fixed issue where writeToSheet() would just create a new sheet and delete the previous data
+
+===================================================================================================
+
+[1.5.1]: Creating a new "build" added an auto spreadsheet creating and updating function for use with both robot and manual data tracking, 
 
 - added createNewSheet(): to create the sheet (names the sheet the current date)
 
 - added writeToSheet(): Use to write data to the created sheet although running "createNewSheet()" is not required as the function will create one if a sheet under the current date cannot be located. Format for the function is writeToSheet(Row, Column, data)
 
-===========================================================================
+===================================================================================================
 
-- [0.5.2]: "Added equations for "limelight" functions"
+[0.5.2]: "Added equations for "limelight" functions"
 
-===========================================================================
+===================================================================================================
 
-- [0.5.1]: "Started Unstable build 0.5"
+[0.5.1]: "Started Unstable build 0.5"
 
-===========================================================================
+===================================================================================================
 
 reminder to py -m build
 and py -m twine upload --repository pypi dist/*
```

### Comparing `lilyanncabinets-1.5.1/README.md` & `lilyanncabinets-1.5.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,32 @@
-Version 1.5.1
+Current Version: 1.5.3
 
-patch notes: 
-===========================================================================
-- [1.5.1]: "Creating a new "build" added an auto spreadsheet creating and updating function for use with both robot and manual data tracking, 
+Patch Notes: 
+
+===================================================================================================
+
+[1.5.3]: Fixed patchnotes formating 
+
+===================================================================================================
+
+[1.5.2]: Fixed issue where writeToSheet() would just create a new sheet and delete the previous data
+
+===================================================================================================
+
+[1.5.1]: Creating a new "build" added an auto spreadsheet creating and updating function for use with both robot and manual data tracking, 
 
 - added createNewSheet(): to create the sheet (names the sheet the current date)
 
 - added writeToSheet(): Use to write data to the created sheet although running "createNewSheet()" is not required as the function will create one if a sheet under the current date cannot be located. Format for the function is writeToSheet(Row, Column, data)
 
-===========================================================================
+===================================================================================================
 
-- [0.5.2]: "Added equations for "limelight" functions"
+[0.5.2]: "Added equations for "limelight" functions"
 
-===========================================================================
+===================================================================================================
 
-- [0.5.1]: "Started Unstable build 0.5"
+[0.5.1]: "Started Unstable build 0.5"
 
-===========================================================================
+===================================================================================================
 
 reminder to py -m build
 and py -m twine upload --repository pypi dist/*
```

### Comparing `lilyanncabinets-1.5.1/setup.cfg` & `lilyanncabinets-1.5.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 696c 7961 6e6e 6361 6269 6e65   = lilyanncabine
 00000020: 7473 0d0a 7665 7273 696f 6e20 3d20 312e  ts..version = 1.
-00000030: 352e 310d 0a61 7574 686f 7220 3d20 4a6f  5.1..author = Jo
+00000030: 352e 330d 0a61 7574 686f 7220 3d20 4a6f  5.3..author = Jo
 00000040: 7365 7068 2043 616c 6967 6975 7269 0d0a  seph Caligiuri..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 206a  author_email = j
 00000060: 6361 6c69 6769 7572 6931 4067 6d61 696c  caligiuri1@gmail
 00000070: 2e63 6f6d 0d0a 6465 7363 7269 7074 696f  .com..descriptio
 00000080: 6e20 3d20 5061 636b 6167 6520 666f 7220  n = Package for 
 00000090: 7573 6520 6279 204c 696c 7920 416e 6e20  use by Lily Ann 
 000000a0: 4361 6269 6e65 7473 0d0a 6c6f 6e67 5f64  Cabinets..long_d
```

### Comparing `lilyanncabinets-1.5.1/src/lilyanncabinets/sheets.py` & `lilyanncabinets-1.5.3/src/lilyanncabinets/sheets.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,26 +10,29 @@
     
     directory = 'sheet/'
     if not os.path.exists(directory):
         os.mkdir(directory)
 
 
     workbook.save(directory + date +'.xlsx')
-    
-
 
 def writeToSheet(r, c, count):
     today = datetime.date.today()
     date = today.strftime('%d-%m-%Y')
-
     directory = 'sheet/'
 
-    if not os.path.exists(directory + date + '.xlsx'):
-        createNewSheet()
+    if not os.path.exists(directory):
+        os.mkdir(directory)
+
+    file_path = os.path.join(directory, date + '.xlsx')
+
+    if not os.path.exists(file_path):
+        workbook = openpyxl.Workbook()
+        workbook.save(file_path)
 
-    workbook = openpyxl.load_workbook(directory + date +'.xlsx')
+    workbook = openpyxl.load_workbook(file_path)
     worksheet = workbook.active
 
     cell = worksheet.cell(row=r, column=c)
     cell.value = count
 
-    workbook.save(directory + date +'.xlsx')
+    workbook.save(file_path)
```

### Comparing `lilyanncabinets-1.5.1/src/lilyanncabinets.egg-info/PKG-INFO` & `lilyanncabinets-1.5.3/src/lilyanncabinets.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 Metadata-Version: 2.1
 Name: lilyanncabinets
-Version: 1.5.1
+Version: 1.5.3
 Summary: Package for use by Lily Ann Cabinets
 Home-page: https://github.com/JosephCaligiuri/lilyanncabinets
 Author: Joseph Caligiuri
 Author-email: jcaligiuri1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Version 1.5.1
+Current Version: 1.5.3
 
-patch notes: 
-===========================================================================
-- [1.5.1]: "Creating a new "build" added an auto spreadsheet creating and updating function for use with both robot and manual data tracking, 
+Patch Notes: 
+
+===================================================================================================
+
+[1.5.3]: Fixed patchnotes formating 
+
+===================================================================================================
+
+[1.5.2]: Fixed issue where writeToSheet() would just create a new sheet and delete the previous data
+
+===================================================================================================
+
+[1.5.1]: Creating a new "build" added an auto spreadsheet creating and updating function for use with both robot and manual data tracking, 
 
 - added createNewSheet(): to create the sheet (names the sheet the current date)
 
 - added writeToSheet(): Use to write data to the created sheet although running "createNewSheet()" is not required as the function will create one if a sheet under the current date cannot be located. Format for the function is writeToSheet(Row, Column, data)
 
-===========================================================================
+===================================================================================================
 
-- [0.5.2]: "Added equations for "limelight" functions"
+[0.5.2]: "Added equations for "limelight" functions"
 
-===========================================================================
+===================================================================================================
 
-- [0.5.1]: "Started Unstable build 0.5"
+[0.5.1]: "Started Unstable build 0.5"
 
-===========================================================================
+===================================================================================================
 
 reminder to py -m build
 and py -m twine upload --repository pypi dist/*
```

