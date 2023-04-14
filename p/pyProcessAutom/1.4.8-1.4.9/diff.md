# Comparing `tmp/pyProcessAutom-1.4.8.tar.gz` & `tmp/pyProcessAutom-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyProcessAutom-1.4.8.tar", last modified: Fri Apr 14 12:41:56 2023, max compression
+gzip compressed data, was "pyProcessAutom-1.4.9.tar", last modified: Fri Apr 14 12:46:49 2023, max compression
```

## Comparing `pyProcessAutom-1.4.8.tar` & `pyProcessAutom-1.4.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 12:41:56.214608 pyProcessAutom-1.4.8/
--rw-rw-rw-   0        0        0     1918 2023-04-14 12:41:56.213636 pyProcessAutom-1.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     1691 2023-04-14 06:00:54.000000 pyProcessAutom-1.4.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 12:41:56.184610 pyProcessAutom-1.4.8/auto_preprocess/
--rw-rw-rw-   0        0        0       45 2023-04-13 06:47:07.000000 pyProcessAutom-1.4.8/auto_preprocess/__init__.py
--rw-rw-rw-   0        0        0     2431 2023-04-14 12:40:47.000000 pyProcessAutom-1.4.8/auto_preprocess/data_preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:41:56.201613 pyProcessAutom-1.4.8/pyProcessAutom.egg-info/
--rw-rw-rw-   0        0        0     1918 2023-04-14 12:41:56.000000 pyProcessAutom-1.4.8/pyProcessAutom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-14 12:41:56.000000 pyProcessAutom-1.4.8/pyProcessAutom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 12:41:56.000000 pyProcessAutom-1.4.8/pyProcessAutom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-14 12:41:56.000000 pyProcessAutom-1.4.8/pyProcessAutom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-14 12:41:56.000000 pyProcessAutom-1.4.8/pyProcessAutom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      370 2023-04-12 17:17:20.000000 pyProcessAutom-1.4.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 12:41:56.214608 pyProcessAutom-1.4.8/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-04-14 12:41:35.000000 pyProcessAutom-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:46:49.651930 pyProcessAutom-1.4.9/
+-rw-rw-rw-   0        0        0     1923 2023-04-14 12:46:49.650944 pyProcessAutom-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1696 2023-04-14 12:46:09.000000 pyProcessAutom-1.4.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 12:46:49.622924 pyProcessAutom-1.4.9/auto_preprocess/
+-rw-rw-rw-   0        0        0       45 2023-04-13 06:47:07.000000 pyProcessAutom-1.4.9/auto_preprocess/__init__.py
+-rw-rw-rw-   0        0        0     2444 2023-04-14 12:46:45.000000 pyProcessAutom-1.4.9/auto_preprocess/data_preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:46:49.638925 pyProcessAutom-1.4.9/pyProcessAutom.egg-info/
+-rw-rw-rw-   0        0        0     1923 2023-04-14 12:46:49.000000 pyProcessAutom-1.4.9/pyProcessAutom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-14 12:46:49.000000 pyProcessAutom-1.4.9/pyProcessAutom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 12:46:49.000000 pyProcessAutom-1.4.9/pyProcessAutom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-14 12:46:49.000000 pyProcessAutom-1.4.9/pyProcessAutom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-14 12:46:49.000000 pyProcessAutom-1.4.9/pyProcessAutom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      370 2023-04-12 17:17:20.000000 pyProcessAutom-1.4.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 12:46:49.651930 pyProcessAutom-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-04-14 12:46:32.000000 pyProcessAutom-1.4.9/setup.py
```

### Comparing `pyProcessAutom-1.4.8/PKG-INFO` & `pyProcessAutom-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyProcessAutom
-Version: 1.4.8
+Version: 1.4.9
 Summary: A data preprocessing library
 Home-page: UNKNOWN
 Author: Aryan Sakhala
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -39,15 +39,15 @@
 preprocessed_df = preprocessor.df
 ```
 # Use the preprocessed data as needed
 Functions
 This library provides the following functions for preprocessing data:
 
 * remove_outliers(): Removes outliers from all numeric columns in the DataFrame.
-* scale(scaler_type): Scales all numeric columns in the DataFrame using either a standard scaler or a min-max scaler.
+* scale(scaler_type): Scales all numeric columns in the DataFrame using either a standard scaler or a min-max scaler. [Arguments = 'standard','minmax']
 * label_encode(): Encodes all columns with binary categories using label encoding.
-* impute(method): Fills all columns with less than 10% NaN values with either the mean, median, or mode, as specified by the user.
+* impute(method): Fills all columns  with either the mean, median, or mode, as specified by the user.
 * drop(): Drops all columns with more than 30% NaN values from the DataFrame.
 License
 
 This project is licensed under the MIT License - see the LICENSE.txt file for details.
```

### Comparing `pyProcessAutom-1.4.8/README.md` & `pyProcessAutom-1.4.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,14 @@
 preprocessed_df = preprocessor.df
 ```
 # Use the preprocessed data as needed
 Functions
 This library provides the following functions for preprocessing data:
 
 * remove_outliers(): Removes outliers from all numeric columns in the DataFrame.
-* scale(scaler_type): Scales all numeric columns in the DataFrame using either a standard scaler or a min-max scaler.
+* scale(scaler_type): Scales all numeric columns in the DataFrame using either a standard scaler or a min-max scaler. [Arguments = 'standard','minmax']
 * label_encode(): Encodes all columns with binary categories using label encoding.
-* impute(method): Fills all columns with less than 10% NaN values with either the mean, median, or mode, as specified by the user.
+* impute(method): Fills all columns  with either the mean, median, or mode, as specified by the user.
 * drop(): Drops all columns with more than 30% NaN values from the DataFrame.
 License
 
 This project is licensed under the MIT License - see the LICENSE.txt file for details.
```

### Comparing `pyProcessAutom-1.4.8/auto_preprocess/data_preprocess.py` & `pyProcessAutom-1.4.9/auto_preprocess/data_preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             Q1 = self.df[col].quantile(0.25)
             Q3 = self.df[col].quantile(0.75)
             IQR = Q3 - Q1
             lower_bound = Q1 - 1.5 * IQR
             upper_bound = Q3 + 1.5 * IQR
             self.df = self.df[(self.df[col] >= lower_bound) & (self.df[col] <= upper_bound)]
     
-    def scale(self, scaler_type):
+    def scale(self, scaler_type = 'standard'):
         num_cols = self.df.select_dtypes(include=['float64', 'int64']).columns.tolist()
         if scaler_type == 'standard':
             scaler = StandardScaler()
         elif scaler_type == 'minmax':
             scaler = MinMaxScaler()
         else:
             raise ValueError('Invalid scaler type. Valid options are "standard" or "minmax"')
```

### Comparing `pyProcessAutom-1.4.8/pyProcessAutom.egg-info/PKG-INFO` & `pyProcessAutom-1.4.9/pyProcessAutom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyProcessAutom
-Version: 1.4.8
+Version: 1.4.9
 Summary: A data preprocessing library
 Home-page: UNKNOWN
 Author: Aryan Sakhala
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
@@ -39,15 +39,15 @@
 preprocessed_df = preprocessor.df
 ```
 # Use the preprocessed data as needed
 Functions
 This library provides the following functions for preprocessing data:
 
 * remove_outliers(): Removes outliers from all numeric columns in the DataFrame.
-* scale(scaler_type): Scales all numeric columns in the DataFrame using either a standard scaler or a min-max scaler.
+* scale(scaler_type): Scales all numeric columns in the DataFrame using either a standard scaler or a min-max scaler. [Arguments = 'standard','minmax']
 * label_encode(): Encodes all columns with binary categories using label encoding.
-* impute(method): Fills all columns with less than 10% NaN values with either the mean, median, or mode, as specified by the user.
+* impute(method): Fills all columns  with either the mean, median, or mode, as specified by the user.
 * drop(): Drops all columns with more than 30% NaN values from the DataFrame.
 License
 
 This project is licensed under the MIT License - see the LICENSE.txt file for details.
```

