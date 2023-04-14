# Comparing `tmp/pyProcessAutom-1.4.4.tar.gz` & `tmp/pyProcessAutom-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyProcessAutom-1.4.4.tar", last modified: Thu Apr 13 09:17:54 2023, max compression
+gzip compressed data, was "pyProcessAutom-1.4.5.tar", last modified: Fri Apr 14 05:52:16 2023, max compression
```

## Comparing `pyProcessAutom-1.4.4.tar` & `pyProcessAutom-1.4.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 09:17:54.507016 pyProcessAutom-1.4.4/
--rw-rw-rw-   0        0        0     1897 2023-04-13 09:17:54.506017 pyProcessAutom-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     1670 2023-04-13 09:17:34.000000 pyProcessAutom-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 09:17:54.462017 pyProcessAutom-1.4.4/auto_preprocess/
--rw-rw-rw-   0        0        0       45 2023-04-13 06:47:07.000000 pyProcessAutom-1.4.4/auto_preprocess/__init__.py
--rw-rw-rw-   0        0        0     2344 2023-04-13 04:16:40.000000 pyProcessAutom-1.4.4/auto_preprocess/data_preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:17:54.503044 pyProcessAutom-1.4.4/pyProcessAutom.egg-info/
--rw-rw-rw-   0        0        0     1897 2023-04-13 09:17:54.000000 pyProcessAutom-1.4.4/pyProcessAutom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-13 09:17:54.000000 pyProcessAutom-1.4.4/pyProcessAutom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 09:17:54.000000 pyProcessAutom-1.4.4/pyProcessAutom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-13 09:17:54.000000 pyProcessAutom-1.4.4/pyProcessAutom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 09:17:54.000000 pyProcessAutom-1.4.4/pyProcessAutom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      370 2023-04-12 17:17:20.000000 pyProcessAutom-1.4.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 09:17:54.508017 pyProcessAutom-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-04-13 09:16:36.000000 pyProcessAutom-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:52:16.201195 pyProcessAutom-1.4.5/
+-rw-rw-rw-   0        0        0     1913 2023-04-14 05:52:16.200196 pyProcessAutom-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1686 2023-04-14 05:52:00.000000 pyProcessAutom-1.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 05:52:16.165197 pyProcessAutom-1.4.5/auto_preprocess/
+-rw-rw-rw-   0        0        0       45 2023-04-13 06:47:07.000000 pyProcessAutom-1.4.5/auto_preprocess/__init__.py
+-rw-rw-rw-   0        0        0     2343 2023-04-14 05:51:23.000000 pyProcessAutom-1.4.5/auto_preprocess/data_preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:52:16.198192 pyProcessAutom-1.4.5/pyProcessAutom.egg-info/
+-rw-rw-rw-   0        0        0     1913 2023-04-14 05:52:16.000000 pyProcessAutom-1.4.5/pyProcessAutom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-14 05:52:16.000000 pyProcessAutom-1.4.5/pyProcessAutom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 05:52:16.000000 pyProcessAutom-1.4.5/pyProcessAutom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-14 05:52:16.000000 pyProcessAutom-1.4.5/pyProcessAutom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-14 05:52:16.000000 pyProcessAutom-1.4.5/pyProcessAutom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      370 2023-04-12 17:17:20.000000 pyProcessAutom-1.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 05:52:16.202201 pyProcessAutom-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-04-14 05:52:10.000000 pyProcessAutom-1.4.5/setup.py
```

### Comparing `pyProcessAutom-1.4.4/PKG-INFO` & `pyProcessAutom-1.4.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,8 @@
-Metadata-Version: 2.1
-Name: pyProcessAutom
-Version: 1.4.4
-Summary: A data preprocessing library
-Home-page: UNKNOWN
-Author: Aryan Sakhala
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-Data Preprocessing Library
+Data Preprocessing Library - Aryan Sakhala
 This library provides a set of functions for preprocessing data in pandas DataFrames.
 
 Installation
 You can install this package using pip:
 
 ```
 pip install pyProcessAutom
@@ -44,9 +34,8 @@
 * remove_outliers(): Removes outliers from all numeric columns in the DataFrame.
 * scale(scaler_type): Scales all numeric columns in the DataFrame using either a standard scaler or a min-max scaler.
 * label_encode(): Encodes all columns with binary categories using label encoding.
 * impute(method): Fills all columns with less than 10% NaN values with either the mean, median, or mode, as specified by the user.
 * drop(): Drops all columns with more than 30% NaN values from the DataFrame.
 License
 
-This project is licensed under the MIT License - see the LICENSE.txt file for details.
-
+This project is licensed under the MIT License - see the LICENSE.txt file for details.
```

### Comparing `pyProcessAutom-1.4.4/README.md` & `pyProcessAutom-1.4.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,18 @@
-Data Preprocessing Library
+Metadata-Version: 2.1
+Name: pyProcessAutom
+Version: 1.4.5
+Summary: A data preprocessing library
+Home-page: UNKNOWN
+Author: Aryan Sakhala
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
+Data Preprocessing Library - Aryan Sakhala
 This library provides a set of functions for preprocessing data in pandas DataFrames.
 
 Installation
 You can install this package using pip:
 
 ```
 pip install pyProcessAutom
@@ -34,8 +44,9 @@
 * remove_outliers(): Removes outliers from all numeric columns in the DataFrame.
 * scale(scaler_type): Scales all numeric columns in the DataFrame using either a standard scaler or a min-max scaler.
 * label_encode(): Encodes all columns with binary categories using label encoding.
 * impute(method): Fills all columns with less than 10% NaN values with either the mean, median, or mode, as specified by the user.
 * drop(): Drops all columns with more than 30% NaN values from the DataFrame.
 License
 
-This project is licensed under the MIT License - see the LICENSE.txt file for details.
+This project is licensed under the MIT License - see the LICENSE.txt file for details.
+
```

### Comparing `pyProcessAutom-1.4.4/auto_preprocess/data_preprocess.py` & `pyProcessAutom-1.4.5/auto_preprocess/data_preprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,24 +29,24 @@
     def label_encode(self):
         bin_cols = self.df.select_dtypes(include=['bool']).columns.tolist()
         le = LabelEncoder()
         for col in bin_cols:
             self.df[col] = le.fit_transform(self.df[col])
     
     def impute(self, method='mean'):
-        num_missing = self.df.select_dtypes(include=['float64', 'int64']).isna().sum()
-        num_cols = num_missing[num_missing > 0].index.tolist()
-        for col in num_cols:
-            if self.df[col].isna().sum() / self.df.shape[0] < 0.1:
-                if method == 'mean':
-                    self.df[col] = self.df[col].fillna(self.df[col].mean())
-                elif method == 'mode':
-                    self.df[col] = self.df[col].fillna(self.df[col].mode().iloc[0])
-                elif method == 'median':
-                    self.df[col] = self.df[col].fillna(self.df[col].median())
-                else:
-                    raise ValueError('Invalid imputation method. Valid options are "mean", "mode", or "median"')
+    # Get numeric columns with missing values
+        num_cols = self.df.select_dtypes(include=['float64', 'int64']).columns[self.df.select_dtypes(include=['float64', 'int64']).isna().any()].tolist()
+        # Fill missing values with specified method or default to mean
+        if method == 'mean':
+            self.df[num_cols] = self.df[num_cols].fillna(self.df[num_cols].mean())
     
+        elif method == 'mode':
+            self.df[num_cols] = self.df[num_cols].fillna(self.df[num_cols].mode())
+        elif method == 'median':
+            self.df[num_cols] = self.df[num_cols].fillna(self.df[num_cols].median())
+        else:
+            raise ValueError('Invalid imputation method. Valid options are "mean", "mode", or "median"')
+
     def drop(self):
         nan_percent = self.df.isna().sum() / self.df.shape[0]
         cols_to_drop = nan_percent[nan_percent > 0.3].index.tolist()
         self.df = self.df.drop(columns=cols_to_drop)
```

### Comparing `pyProcessAutom-1.4.4/pyProcessAutom.egg-info/PKG-INFO` & `pyProcessAutom-1.4.5/pyProcessAutom.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyProcessAutom
-Version: 1.4.4
+Version: 1.4.5
 Summary: A data preprocessing library
 Home-page: UNKNOWN
 Author: Aryan Sakhala
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-Data Preprocessing Library
+Data Preprocessing Library - Aryan Sakhala
 This library provides a set of functions for preprocessing data in pandas DataFrames.
 
 Installation
 You can install this package using pip:
 
 ```
 pip install pyProcessAutom
```

