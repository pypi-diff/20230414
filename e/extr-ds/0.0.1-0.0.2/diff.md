# Comparing `tmp/extr-ds-0.0.1.tar.gz` & `tmp/extr-ds-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-ds-0.0.1.tar", last modified: Fri Apr 14 09:54:20 2023, max compression
+gzip compressed data, was "extr-ds-0.0.2.tar", last modified: Fri Apr 14 10:05:22 2023, max compression
```

## Comparing `extr-ds-0.0.1.tar` & `extr-ds-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 09:54:20.862703 extr-ds-0.0.1/
--rw-rw-rw-   0        0        0     1621 2023-04-14 09:54:20.860209 extr-ds-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      996 2023-04-14 09:49:18.000000 extr-ds-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 09:54:20.865996 extr-ds-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      580 2023-04-14 09:53:55.000000 extr-ds-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:54:20.663927 extr-ds-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 09:54:20.705629 extr-ds-0.0.1/src/extr_ds/
--rw-rw-rw-   0        0        0       28 2023-04-14 09:40:56.000000 extr-ds-0.0.1/src/extr_ds/__init__.py
--rw-rw-rw-   0        0        0     1528 2023-04-13 12:42:40.000000 extr-ds-0.0.1/src/extr_ds/labellers.py
--rw-rw-rw-   0        0        0      698 2023-04-13 12:44:06.000000 extr-ds-0.0.1/src/extr_ds/models.py
--rw-rw-rw-   0        0        0      939 2023-04-13 12:37:43.000000 extr-ds-0.0.1/src/extr_ds/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:54:20.853739 extr-ds-0.0.1/src/extr_ds.egg-info/
--rw-rw-rw-   0        0        0     1621 2023-04-14 09:54:20.000000 extr-ds-0.0.1/src/extr_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-04-14 09:54:20.000000 extr-ds-0.0.1/src/extr_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:54:20.000000 extr-ds-0.0.1/src/extr_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-14 09:54:20.000000 extr-ds-0.0.1/src/extr_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 09:54:20.000000 extr-ds-0.0.1/src/extr_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 10:05:22.307503 extr-ds-0.0.2/
+-rw-rw-rw-   0        0        0     1568 2023-04-14 10:05:22.286497 extr-ds-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      917 2023-04-14 09:57:19.000000 extr-ds-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 10:05:22.323650 extr-ds-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      607 2023-04-14 10:04:02.000000 extr-ds-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:05:22.124302 extr-ds-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 10:05:22.177562 extr-ds-0.0.2/src/extr_ds/
+-rw-rw-rw-   0        0        0       28 2023-04-14 09:40:56.000000 extr-ds-0.0.2/src/extr_ds/__init__.py
+-rw-rw-rw-   0        0        0     1528 2023-04-13 12:42:40.000000 extr-ds-0.0.2/src/extr_ds/labellers.py
+-rw-rw-rw-   0        0        0      698 2023-04-13 12:44:06.000000 extr-ds-0.0.2/src/extr_ds/models.py
+-rw-rw-rw-   0        0        0      939 2023-04-13 12:37:43.000000 extr-ds-0.0.2/src/extr_ds/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:05:22.270076 extr-ds-0.0.2/src/extr_ds.egg-info/
+-rw-rw-rw-   0        0        0     1568 2023-04-14 10:05:21.000000 extr-ds-0.0.2/src/extr_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-04-14 10:05:22.000000 extr-ds-0.0.2/src/extr_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 10:05:21.000000 extr-ds-0.0.2/src/extr_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 10:05:21.000000 extr-ds-0.0.2/src/extr_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 10:05:21.000000 extr-ds-0.0.2/src/extr_ds.egg-info/top_level.txt
```

### Comparing `extr-ds-0.0.1/PKG-INFO` & `extr-ds-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: extr-ds
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
-Home-page: UNKNOWN
+Home-page: https://github.com/dpasse/extr-ds
 License: UNKNOWN
 Description: # extr-ds
-        > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks. <br /><br />Extension of the [extr]('https://github.com/dpasse/extr') library.
+        > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
         
         <br />
         
         ## Install
         
         ```
         pip install extr-ds
```

### Comparing `extr-ds-0.0.1/README.md` & `extr-ds-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # extr-ds
-> Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks. <br /><br />Extension of the [extr]('https://github.com/dpasse/extr') library.
+> Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
 
 <br />
 
 ## Install
 
 ```
 pip install extr-ds
```

### Comparing `extr-ds-0.0.1/src/extr_ds/labellers.py` & `extr-ds-0.0.2/src/extr_ds/labellers.py`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.1/src/extr_ds/models.py` & `extr-ds-0.0.2/src/extr_ds/models.py`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.1/src/extr_ds/tokenizer.py` & `extr-ds-0.0.2/src/extr_ds/tokenizer.py`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.1/src/extr_ds.egg-info/PKG-INFO` & `extr-ds-0.0.2/src/extr_ds.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: extr-ds
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
-Home-page: UNKNOWN
+Home-page: https://github.com/dpasse/extr-ds
 License: UNKNOWN
 Description: # extr-ds
-        > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks. <br /><br />Extension of the [extr]('https://github.com/dpasse/extr') library.
+        > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
         
         <br />
         
         ## Install
         
         ```
         pip install extr-ds
```

