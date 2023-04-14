# Comparing `tmp/pyProcessAutom-1.4.6.tar.gz` & `tmp/pyProcessAutom-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyProcessAutom-1.4.6.tar", last modified: Fri Apr 14 06:01:14 2023, max compression
+gzip compressed data, was "pyProcessAutom-1.4.7.tar", last modified: Fri Apr 14 12:20:12 2023, max compression
```

## Comparing `pyProcessAutom-1.4.6.tar` & `pyProcessAutom-1.4.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 06:01:14.212736 pyProcessAutom-1.4.6/
--rw-rw-rw-   0        0        0     1918 2023-04-14 06:01:14.211723 pyProcessAutom-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     1691 2023-04-14 06:00:54.000000 pyProcessAutom-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 06:01:14.188727 pyProcessAutom-1.4.6/auto_preprocess/
--rw-rw-rw-   0        0        0       45 2023-04-13 06:47:07.000000 pyProcessAutom-1.4.6/auto_preprocess/__init__.py
--rw-rw-rw-   0        0        0     2543 2023-04-14 06:00:29.000000 pyProcessAutom-1.4.6/auto_preprocess/data_preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-14 06:01:14.210727 pyProcessAutom-1.4.6/pyProcessAutom.egg-info/
--rw-rw-rw-   0        0        0     1918 2023-04-14 06:01:14.000000 pyProcessAutom-1.4.6/pyProcessAutom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-14 06:01:14.000000 pyProcessAutom-1.4.6/pyProcessAutom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 06:01:14.000000 pyProcessAutom-1.4.6/pyProcessAutom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-14 06:01:14.000000 pyProcessAutom-1.4.6/pyProcessAutom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-14 06:01:14.000000 pyProcessAutom-1.4.6/pyProcessAutom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      370 2023-04-12 17:17:20.000000 pyProcessAutom-1.4.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 06:01:14.213729 pyProcessAutom-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-04-14 06:00:36.000000 pyProcessAutom-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:20:12.521984 pyProcessAutom-1.4.7/
+-rw-rw-rw-   0        0        0     1918 2023-04-14 12:20:12.520982 pyProcessAutom-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1691 2023-04-14 06:00:54.000000 pyProcessAutom-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 12:20:12.502981 pyProcessAutom-1.4.7/auto_preprocess/
+-rw-rw-rw-   0        0        0       45 2023-04-13 06:47:07.000000 pyProcessAutom-1.4.7/auto_preprocess/__init__.py
+-rw-rw-rw-   0        0        0     2619 2023-04-14 12:16:32.000000 pyProcessAutom-1.4.7/auto_preprocess/data_preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:20:12.519979 pyProcessAutom-1.4.7/pyProcessAutom.egg-info/
+-rw-rw-rw-   0        0        0     1918 2023-04-14 12:20:12.000000 pyProcessAutom-1.4.7/pyProcessAutom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-14 12:20:12.000000 pyProcessAutom-1.4.7/pyProcessAutom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 12:20:12.000000 pyProcessAutom-1.4.7/pyProcessAutom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-14 12:20:12.000000 pyProcessAutom-1.4.7/pyProcessAutom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-14 12:20:12.000000 pyProcessAutom-1.4.7/pyProcessAutom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      370 2023-04-12 17:17:20.000000 pyProcessAutom-1.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 12:20:12.522980 pyProcessAutom-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-04-14 12:19:51.000000 pyProcessAutom-1.4.7/setup.py
```

### Comparing `pyProcessAutom-1.4.6/PKG-INFO` & `pyProcessAutom-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyProcessAutom
-Version: 1.4.6
+Version: 1.4.7
 Summary: A data preprocessing library
 Home-page: UNKNOWN
 Author: Aryan Sakhala
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pyProcessAutom-1.4.6/README.md` & `pyProcessAutom-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `pyProcessAutom-1.4.6/auto_preprocess/data_preprocess.py` & `pyProcessAutom-1.4.7/auto_preprocess/data_preprocess.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,22 +36,25 @@
     
     def impute(self, method='mean'):
         # Get numeric columns with missing values
         num_cols = self.df.select_dtypes(include=['float64', 'int64']).columns[self.df.select_dtypes(include=['float64', 'int64']).isna().any()].tolist()
         # Fill missing values with specified method or default to mean
         if method == 'mean':
             self.df[num_cols] = self.df[num_cols].fillna(self.df[num_cols].mean())
+            self.df = self.df
         elif method == 'mode':
             self.df[num_cols] = self.df[num_cols].fillna(self.df[num_cols].mode().iloc[0])
+            self.df = self.df
         elif method == 'median':
             self.df[num_cols] = self.df[num_cols].fillna(self.df[num_cols].median())
+            self.df = self.df
         else:
             raise ValueError('Invalid imputation method. Valid options are "mean", "mode", or "median"')
             
         # Make the changes permanent by assigning the modified DataFrame to self.df
-        self.df = self.df
+        
 
             
     def drop(self):
         nan_percent = self.df.isna().sum() / self.df.shape[0]
         cols_to_drop = nan_percent[nan_percent > 0.3].index.tolist()
         self.df = self.df.drop(columns=cols_to_drop)
```

### Comparing `pyProcessAutom-1.4.6/pyProcessAutom.egg-info/PKG-INFO` & `pyProcessAutom-1.4.7/pyProcessAutom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyProcessAutom
-Version: 1.4.6
+Version: 1.4.7
 Summary: A data preprocessing library
 Home-page: UNKNOWN
 Author: Aryan Sakhala
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

