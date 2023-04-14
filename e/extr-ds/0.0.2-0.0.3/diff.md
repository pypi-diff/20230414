# Comparing `tmp/extr-ds-0.0.2.tar.gz` & `tmp/extr-ds-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-ds-0.0.2.tar", last modified: Fri Apr 14 10:05:22 2023, max compression
+gzip compressed data, was "extr-ds-0.0.3.tar", last modified: Fri Apr 14 10:34:40 2023, max compression
```

## Comparing `extr-ds-0.0.2.tar` & `extr-ds-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 10:05:22.307503 extr-ds-0.0.2/
--rw-rw-rw-   0        0        0     1568 2023-04-14 10:05:22.286497 extr-ds-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      917 2023-04-14 09:57:19.000000 extr-ds-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 10:05:22.323650 extr-ds-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      607 2023-04-14 10:04:02.000000 extr-ds-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:05:22.124302 extr-ds-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 10:05:22.177562 extr-ds-0.0.2/src/extr_ds/
--rw-rw-rw-   0        0        0       28 2023-04-14 09:40:56.000000 extr-ds-0.0.2/src/extr_ds/__init__.py
--rw-rw-rw-   0        0        0     1528 2023-04-13 12:42:40.000000 extr-ds-0.0.2/src/extr_ds/labellers.py
--rw-rw-rw-   0        0        0      698 2023-04-13 12:44:06.000000 extr-ds-0.0.2/src/extr_ds/models.py
--rw-rw-rw-   0        0        0      939 2023-04-13 12:37:43.000000 extr-ds-0.0.2/src/extr_ds/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:05:22.270076 extr-ds-0.0.2/src/extr_ds.egg-info/
--rw-rw-rw-   0        0        0     1568 2023-04-14 10:05:21.000000 extr-ds-0.0.2/src/extr_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-04-14 10:05:22.000000 extr-ds-0.0.2/src/extr_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 10:05:21.000000 extr-ds-0.0.2/src/extr_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-14 10:05:21.000000 extr-ds-0.0.2/src/extr_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 10:05:21.000000 extr-ds-0.0.2/src/extr_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 10:34:40.681237 extr-ds-0.0.3/
+-rw-rw-rw-   0        0        0     2045 2023-04-14 10:34:40.669943 extr-ds-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1282 2023-04-14 10:32:19.000000 extr-ds-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 10:34:40.684556 extr-ds-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      607 2023-04-14 10:32:59.000000 extr-ds-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:34:40.342558 extr-ds-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 10:34:40.445405 extr-ds-0.0.3/src/extr_ds/
+-rw-rw-rw-   0        0        0       28 2023-04-14 09:40:56.000000 extr-ds-0.0.3/src/extr_ds/__init__.py
+-rw-rw-rw-   0        0        0     1528 2023-04-13 12:42:40.000000 extr-ds-0.0.3/src/extr_ds/labellers.py
+-rw-rw-rw-   0        0        0      719 2023-04-14 10:33:59.000000 extr-ds-0.0.3/src/extr_ds/merges.py
+-rw-rw-rw-   0        0        0      698 2023-04-13 12:44:06.000000 extr-ds-0.0.3/src/extr_ds/models.py
+-rw-rw-rw-   0        0        0      939 2023-04-13 12:37:43.000000 extr-ds-0.0.3/src/extr_ds/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:34:40.663312 extr-ds-0.0.3/src/extr_ds.egg-info/
+-rw-rw-rw-   0        0        0     2045 2023-04-14 10:34:39.000000 extr-ds-0.0.3/src/extr_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-04-14 10:34:39.000000 extr-ds-0.0.3/src/extr_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 10:34:39.000000 extr-ds-0.0.3/src/extr_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 10:34:39.000000 extr-ds-0.0.3/src/extr_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 10:34:39.000000 extr-ds-0.0.3/src/extr_ds.egg-info/top_level.txt
```

### Comparing `extr-ds-0.0.2/PKG-INFO` & `extr-ds-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr-ds
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
 Home-page: https://github.com/dpasse/extr-ds
 License: UNKNOWN
 Description: # extr-ds
         > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
         
         <br />
@@ -41,9 +41,23 @@
         
         ## labels ==  [
         ##     ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
         ##     ['B-PERSON', 'O', 'O', 'O', 'O', 'O']
         ## ]
         ```
         
+        ### 2. Verify Actual vs Model
+        
+        ```python
+        from extr-ds.merges import check_for_differences
+        
+        differences_in_labels = check_for_differences(
+            ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
+            ['B-PERSON', 'O', 'O', 'O', 'B-POSITION', 'O']
+        )
+        
+        ## differences_in_labels.has_diffs == True
+        ## differences_in_labels.diffs_between_labels = [1]
+        ```
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `extr-ds-0.0.2/README.md` & `extr-ds-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -34,7 +34,21 @@
 labels = IOB(sentence_tokenizer, entity_extractor).label(text)
 
 ## labels ==  [
 ##     ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
 ##     ['B-PERSON', 'O', 'O', 'O', 'O', 'O']
 ## ]
 ```
+
+### 2. Verify Actual vs Model
+
+```python
+from extr-ds.merges import check_for_differences
+
+differences_in_labels = check_for_differences(
+    ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
+    ['B-PERSON', 'O', 'O', 'O', 'B-POSITION', 'O']
+)
+
+## differences_in_labels.has_diffs == True
+## differences_in_labels.diffs_between_labels = [1]
+```
```

### Comparing `extr-ds-0.0.2/setup.py` & `extr-ds-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='extr-ds',
-    version='0.0.2',
+    version='0.0.3',
     keywords='',
     description='Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.',
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[
         'extr==0.0.5'
     ],
```

### Comparing `extr-ds-0.0.2/src/extr_ds/labellers.py` & `extr-ds-0.0.3/src/extr_ds/labellers.py`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.2/src/extr_ds/models.py` & `extr-ds-0.0.3/src/extr_ds/models.py`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.2/src/extr_ds/tokenizer.py` & `extr-ds-0.0.3/src/extr_ds/tokenizer.py`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.2/src/extr_ds.egg-info/PKG-INFO` & `extr-ds-0.0.3/src/extr_ds.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr-ds
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
 Home-page: https://github.com/dpasse/extr-ds
 License: UNKNOWN
 Description: # extr-ds
         > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
         
         <br />
@@ -41,9 +41,23 @@
         
         ## labels ==  [
         ##     ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
         ##     ['B-PERSON', 'O', 'O', 'O', 'O', 'O']
         ## ]
         ```
         
+        ### 2. Verify Actual vs Model
+        
+        ```python
+        from extr-ds.merges import check_for_differences
+        
+        differences_in_labels = check_for_differences(
+            ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
+            ['B-PERSON', 'O', 'O', 'O', 'B-POSITION', 'O']
+        )
+        
+        ## differences_in_labels.has_diffs == True
+        ## differences_in_labels.diffs_between_labels = [1]
+        ```
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

