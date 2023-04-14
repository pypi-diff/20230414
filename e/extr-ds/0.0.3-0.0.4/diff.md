# Comparing `tmp/extr-ds-0.0.3.tar.gz` & `tmp/extr-ds-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-ds-0.0.3.tar", last modified: Fri Apr 14 10:34:40 2023, max compression
+gzip compressed data, was "extr-ds-0.0.4.tar", last modified: Fri Apr 14 12:30:19 2023, max compression
```

## Comparing `extr-ds-0.0.3.tar` & `extr-ds-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 10:34:40.681237 extr-ds-0.0.3/
--rw-rw-rw-   0        0        0     2045 2023-04-14 10:34:40.669943 extr-ds-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1282 2023-04-14 10:32:19.000000 extr-ds-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 10:34:40.684556 extr-ds-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      607 2023-04-14 10:32:59.000000 extr-ds-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:34:40.342558 extr-ds-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 10:34:40.445405 extr-ds-0.0.3/src/extr_ds/
--rw-rw-rw-   0        0        0       28 2023-04-14 09:40:56.000000 extr-ds-0.0.3/src/extr_ds/__init__.py
--rw-rw-rw-   0        0        0     1528 2023-04-13 12:42:40.000000 extr-ds-0.0.3/src/extr_ds/labellers.py
--rw-rw-rw-   0        0        0      719 2023-04-14 10:33:59.000000 extr-ds-0.0.3/src/extr_ds/merges.py
--rw-rw-rw-   0        0        0      698 2023-04-13 12:44:06.000000 extr-ds-0.0.3/src/extr_ds/models.py
--rw-rw-rw-   0        0        0      939 2023-04-13 12:37:43.000000 extr-ds-0.0.3/src/extr_ds/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:34:40.663312 extr-ds-0.0.3/src/extr_ds.egg-info/
--rw-rw-rw-   0        0        0     2045 2023-04-14 10:34:39.000000 extr-ds-0.0.3/src/extr_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-04-14 10:34:39.000000 extr-ds-0.0.3/src/extr_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 10:34:39.000000 extr-ds-0.0.3/src/extr_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-14 10:34:39.000000 extr-ds-0.0.3/src/extr_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 10:34:39.000000 extr-ds-0.0.3/src/extr_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 12:30:19.435400 extr-ds-0.0.4/
+-rw-rw-rw-   0        0        0     2591 2023-04-14 12:30:19.417144 extr-ds-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1732 2023-04-14 12:29:13.000000 extr-ds-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 12:30:19.444048 extr-ds-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      607 2023-04-14 12:30:15.000000 extr-ds-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:30:19.016054 extr-ds-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 12:30:19.099971 extr-ds-0.0.4/src/extr_ds/
+-rw-rw-rw-   0        0        0       28 2023-04-14 09:40:56.000000 extr-ds-0.0.4/src/extr_ds/__init__.py
+-rw-rw-rw-   0        0        0     1528 2023-04-13 12:42:40.000000 extr-ds-0.0.4/src/extr_ds/labellers.py
+-rw-rw-rw-   0        0        0      698 2023-04-13 12:44:06.000000 extr-ds-0.0.4/src/extr_ds/models.py
+-rw-rw-rw-   0        0        0      939 2023-04-13 12:37:43.000000 extr-ds-0.0.4/src/extr_ds/tokenizer.py
+-rw-rw-rw-   0        0        0     1527 2023-04-14 12:22:51.000000 extr-ds-0.0.4/src/extr_ds/validators.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:30:19.389322 extr-ds-0.0.4/src/extr_ds.egg-info/
+-rw-rw-rw-   0        0        0     2591 2023-04-14 12:30:18.000000 extr-ds-0.0.4/src/extr_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-04-14 12:30:18.000000 extr-ds-0.0.4/src/extr_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 12:30:18.000000 extr-ds-0.0.4/src/extr_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 12:30:18.000000 extr-ds-0.0.4/src/extr_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 12:30:18.000000 extr-ds-0.0.4/src/extr_ds.egg-info/top_level.txt
```

### Comparing `extr-ds-0.0.3/PKG-INFO` & `extr-ds-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr-ds
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
 Home-page: https://github.com/dpasse/extr-ds
 License: UNKNOWN
 Description: # extr-ds
         > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
         
         <br />
@@ -21,15 +21,15 @@
         text = 'Ted Johnson is a pitcher. Ted went to my school.'
         ```
         
         ### 1. Label Entities for Named-Entity Recognition Task (NER)
         
         ```python
         from extr import RegEx, RegExLabel, EntityExtactor
-        from extr-ds import IOB
+        from extr_ds import IOB
         
         entity_extractor = EntityExtactor([
             RegExLabel('PERSON', [
                 RegEx([r'(ted\s+johnson|ted)'], re.IGNORECASE)
             ]),
             RegExLabel('POSITION', [
                 RegEx([r'pitcher'], re.IGNORECASE)
@@ -41,23 +41,35 @@
         
         ## labels ==  [
         ##     ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
         ##     ['B-PERSON', 'O', 'O', 'O', 'O', 'O']
         ## ]
         ```
         
-        ### 2. Verify Actual vs Model
+        ### 2. Find and define the type of difference between labels
         
         ```python
-        from extr-ds.merges import check_for_differences
+        from extr_ds.validators import check_for_differences
         
         differences_in_labels = check_for_differences(
             ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
             ['B-PERSON', 'O', 'O', 'O', 'B-POSITION', 'O']
         )
         
         ## differences_in_labels.has_diffs == True
-        ## differences_in_labels.diffs_between_labels = [1]
+        ## differences_in_labels.diffs_between_labels == [
+        ##      <Difference index=1, diff_type=DifferenceTypes.S2_MISSING>
+        ## ]
+        
+        differences_in_labels = check_for_differences(
+            ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
+            ['B-PERSON', 'B-PERSON', 'O', 'O', 'B-POSITION', 'O']
+        )
+        
+        ## differences_in_labels.has_diffs == True
+        ## differences_in_labels.diffs_between_labels == [
+        ##      <Difference index=1, diff_type=DifferenceTypes.MISMATCH>
+        ## ]
         ```
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `extr-ds-0.0.3/README.md` & `extr-ds-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 text = 'Ted Johnson is a pitcher. Ted went to my school.'
 ```
 
 ### 1. Label Entities for Named-Entity Recognition Task (NER)
 
 ```python
 from extr import RegEx, RegExLabel, EntityExtactor
-from extr-ds import IOB
+from extr_ds import IOB
 
 entity_extractor = EntityExtactor([
     RegExLabel('PERSON', [
         RegEx([r'(ted\s+johnson|ted)'], re.IGNORECASE)
     ]),
     RegExLabel('POSITION', [
         RegEx([r'pitcher'], re.IGNORECASE)
@@ -35,20 +35,32 @@
 
 ## labels ==  [
 ##     ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
 ##     ['B-PERSON', 'O', 'O', 'O', 'O', 'O']
 ## ]
 ```
 
-### 2. Verify Actual vs Model
+### 2. Find and define the type of difference between labels
 
 ```python
-from extr-ds.merges import check_for_differences
+from extr_ds.validators import check_for_differences
 
 differences_in_labels = check_for_differences(
     ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
     ['B-PERSON', 'O', 'O', 'O', 'B-POSITION', 'O']
 )
 
 ## differences_in_labels.has_diffs == True
-## differences_in_labels.diffs_between_labels = [1]
+## differences_in_labels.diffs_between_labels == [
+##      <Difference index=1, diff_type=DifferenceTypes.S2_MISSING>
+## ]
+
+differences_in_labels = check_for_differences(
+    ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
+    ['B-PERSON', 'B-PERSON', 'O', 'O', 'B-POSITION', 'O']
+)
+
+## differences_in_labels.has_diffs == True
+## differences_in_labels.diffs_between_labels == [
+##      <Difference index=1, diff_type=DifferenceTypes.MISMATCH>
+## ]
 ```
```

### Comparing `extr-ds-0.0.3/setup.py` & `extr-ds-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='extr-ds',
-    version='0.0.3',
+    version='0.0.4',
     keywords='',
     description='Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.',
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[
         'extr==0.0.5'
     ],
```

### Comparing `extr-ds-0.0.3/src/extr_ds/labellers.py` & `extr-ds-0.0.4/src/extr_ds/labellers.py`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.3/src/extr_ds/models.py` & `extr-ds-0.0.4/src/extr_ds/models.py`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.3/src/extr_ds/tokenizer.py` & `extr-ds-0.0.4/src/extr_ds/tokenizer.py`

 * *Files identical despite different names*

### Comparing `extr-ds-0.0.3/src/extr_ds.egg-info/PKG-INFO` & `extr-ds-0.0.4/src/extr_ds.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extr-ds
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
 Home-page: https://github.com/dpasse/extr-ds
 License: UNKNOWN
 Description: # extr-ds
         > Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
         
         <br />
@@ -21,15 +21,15 @@
         text = 'Ted Johnson is a pitcher. Ted went to my school.'
         ```
         
         ### 1. Label Entities for Named-Entity Recognition Task (NER)
         
         ```python
         from extr import RegEx, RegExLabel, EntityExtactor
-        from extr-ds import IOB
+        from extr_ds import IOB
         
         entity_extractor = EntityExtactor([
             RegExLabel('PERSON', [
                 RegEx([r'(ted\s+johnson|ted)'], re.IGNORECASE)
             ]),
             RegExLabel('POSITION', [
                 RegEx([r'pitcher'], re.IGNORECASE)
@@ -41,23 +41,35 @@
         
         ## labels ==  [
         ##     ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
         ##     ['B-PERSON', 'O', 'O', 'O', 'O', 'O']
         ## ]
         ```
         
-        ### 2. Verify Actual vs Model
+        ### 2. Find and define the type of difference between labels
         
         ```python
-        from extr-ds.merges import check_for_differences
+        from extr_ds.validators import check_for_differences
         
         differences_in_labels = check_for_differences(
             ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
             ['B-PERSON', 'O', 'O', 'O', 'B-POSITION', 'O']
         )
         
         ## differences_in_labels.has_diffs == True
-        ## differences_in_labels.diffs_between_labels = [1]
+        ## differences_in_labels.diffs_between_labels == [
+        ##      <Difference index=1, diff_type=DifferenceTypes.S2_MISSING>
+        ## ]
+        
+        differences_in_labels = check_for_differences(
+            ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
+            ['B-PERSON', 'B-PERSON', 'O', 'O', 'B-POSITION', 'O']
+        )
+        
+        ## differences_in_labels.has_diffs == True
+        ## differences_in_labels.diffs_between_labels == [
+        ##      <Difference index=1, diff_type=DifferenceTypes.MISMATCH>
+        ## ]
         ```
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

