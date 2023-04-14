# Comparing `tmp/dipwmsearch-0.1.7.tar.gz` & `tmp/dipwmsearch-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipwmsearch-0.1.7.tar", last modified: Wed Feb 22 17:27:51 2023, max compression
+gzip compressed data, was "dipwmsearch-0.1.8.tar", last modified: Fri Apr 14 16:50:17 2023, max compression
```

## Comparing `dipwmsearch-0.1.7.tar` & `dipwmsearch-0.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwx------   0 rivals    (1001) rivals    (1001)        0 2023-02-22 17:27:51.204840 dipwmsearch-0.1.7/
--rw-------   0 rivals    (1001) rivals    (1001)    21582 2023-02-17 15:45:14.000000 dipwmsearch-0.1.7/LICENSE.txt
--rw-------   0 rivals    (1001) rivals    (1001)    27650 2023-02-22 17:27:51.204840 dipwmsearch-0.1.7/PKG-INFO
--rw-------   0 rivals    (1001) rivals    (1001)     1058 2022-12-31 18:32:39.000000 dipwmsearch-0.1.7/README.md
-drwx------   0 rivals    (1001) rivals    (1001)        0 2023-02-22 17:27:51.200840 dipwmsearch-0.1.7/dipwmsearch.egg-info/
--rw-------   0 rivals    (1001) rivals    (1001)    27650 2023-02-22 17:27:51.000000 dipwmsearch-0.1.7/dipwmsearch.egg-info/PKG-INFO
--rw-------   0 rivals    (1001) rivals    (1001)      475 2023-02-22 17:27:51.000000 dipwmsearch-0.1.7/dipwmsearch.egg-info/SOURCES.txt
--rw-------   0 rivals    (1001) rivals    (1001)        1 2023-02-22 17:27:51.000000 dipwmsearch-0.1.7/dipwmsearch.egg-info/dependency_links.txt
--rw-------   0 rivals    (1001) rivals    (1001)       38 2023-02-22 17:27:51.000000 dipwmsearch-0.1.7/dipwmsearch.egg-info/requires.txt
--rw-------   0 rivals    (1001) rivals    (1001)       12 2023-02-22 17:27:51.000000 dipwmsearch-0.1.7/dipwmsearch.egg-info/top_level.txt
--rw-------   0 rivals    (1001) rivals    (1001)     1407 2023-02-22 17:00:23.000000 dipwmsearch-0.1.7/pyproject.toml
--rw-------   0 rivals    (1001) rivals    (1001)       38 2023-02-22 17:27:51.204840 dipwmsearch-0.1.7/setup.cfg
--rw-------   0 rivals    (1001) rivals    (1001)      132 2023-01-05 13:30:16.000000 dipwmsearch-0.1.7/setup.py
-drwx------   0 rivals    (1001) rivals    (1001)        0 2023-02-22 17:27:51.200840 dipwmsearch-0.1.7/src/
--rw-------   0 rivals    (1001) rivals    (1001)     3465 2023-02-17 15:45:14.000000 dipwmsearch-0.1.7/src/AhoCorasick.py
--rw-------   0 rivals    (1001) rivals    (1001)    11344 2023-02-22 09:25:42.000000 dipwmsearch-0.1.7/src/Block.py
--rw-------   0 rivals    (1001) rivals    (1001)     3306 2022-12-31 18:32:39.000000 dipwmsearch-0.1.7/src/Enumerate.py
--rw-------   0 rivals    (1001) rivals    (1001)    10836 2022-12-31 18:32:39.000000 dipwmsearch-0.1.7/src/SemiNaive.py
--rw-------   0 rivals    (1001) rivals    (1001)      590 2023-01-05 13:30:16.000000 dipwmsearch-0.1.7/src/__init__.py
--rw-------   0 rivals    (1001) rivals    (1001)     5144 2023-02-22 10:20:38.000000 dipwmsearch-0.1.7/src/__main__.py
--rw-------   0 rivals    (1001) rivals    (1001)    18556 2023-02-17 15:45:14.000000 dipwmsearch-0.1.7/src/diPwm.py
-drwx------   0 rivals    (1001) rivals    (1001)        0 2023-02-22 17:27:51.200840 dipwmsearch-0.1.7/test/
--rw-------   0 rivals    (1001) rivals    (1001)      429 2022-12-31 18:32:39.000000 dipwmsearch-0.1.7/test/test_Aho.py
--rw-------   0 rivals    (1001) rivals    (1001)     2366 2022-12-31 18:32:39.000000 dipwmsearch-0.1.7/test/test_Block.py
--rw-------   0 rivals    (1001) rivals    (1001)     1045 2022-12-31 18:32:39.000000 dipwmsearch-0.1.7/test/test_Enumerate.py
--rw-------   0 rivals    (1001) rivals    (1001)     1349 2023-02-17 15:45:14.000000 dipwmsearch-0.1.7/test/test_Pvalue.py
--rw-------   0 rivals    (1001) rivals    (1001)     7778 2022-12-31 18:32:39.000000 dipwmsearch-0.1.7/test/test_SemiNaive.py
--rw-------   0 rivals    (1001) rivals    (1001)     1583 2022-12-31 18:32:39.000000 dipwmsearch-0.1.7/test/test_diPWM.py
--rw-------   0 rivals    (1001) rivals    (1001)     1860 2022-12-31 18:32:39.000000 dipwmsearch-0.1.7/test/test_diPWM_file.py
+drwx------   0 rivals    (1001) rivals    (1001)        0 2023-04-14 16:50:17.934685 dipwmsearch-0.1.8/
+-rw-------   0 rivals    (1001) rivals    (1001)    21582 2023-02-17 15:45:14.000000 dipwmsearch-0.1.8/LICENSE.txt
+-rw-------   0 rivals    (1001) rivals    (1001)    27650 2023-04-14 16:50:17.934685 dipwmsearch-0.1.8/PKG-INFO
+-rw-------   0 rivals    (1001) rivals    (1001)     1058 2022-12-31 18:32:39.000000 dipwmsearch-0.1.8/README.md
+drwx------   0 rivals    (1001) rivals    (1001)        0 2023-04-14 16:50:17.934685 dipwmsearch-0.1.8/dipwmsearch.egg-info/
+-rw-------   0 rivals    (1001) rivals    (1001)    27650 2023-04-14 16:50:17.000000 dipwmsearch-0.1.8/dipwmsearch.egg-info/PKG-INFO
+-rw-------   0 rivals    (1001) rivals    (1001)      475 2023-04-14 16:50:17.000000 dipwmsearch-0.1.8/dipwmsearch.egg-info/SOURCES.txt
+-rw-------   0 rivals    (1001) rivals    (1001)        1 2023-04-14 16:50:17.000000 dipwmsearch-0.1.8/dipwmsearch.egg-info/dependency_links.txt
+-rw-------   0 rivals    (1001) rivals    (1001)       38 2023-04-14 16:50:17.000000 dipwmsearch-0.1.8/dipwmsearch.egg-info/requires.txt
+-rw-------   0 rivals    (1001) rivals    (1001)       12 2023-04-14 16:50:17.000000 dipwmsearch-0.1.8/dipwmsearch.egg-info/top_level.txt
+-rw-------   0 rivals    (1001) rivals    (1001)     1407 2023-04-14 16:50:10.000000 dipwmsearch-0.1.8/pyproject.toml
+-rw-------   0 rivals    (1001) rivals    (1001)       38 2023-04-14 16:50:17.934685 dipwmsearch-0.1.8/setup.cfg
+-rw-------   0 rivals    (1001) rivals    (1001)      132 2023-01-05 13:30:16.000000 dipwmsearch-0.1.8/setup.py
+drwx------   0 rivals    (1001) rivals    (1001)        0 2023-04-14 16:50:17.934685 dipwmsearch-0.1.8/src/
+-rw-------   0 rivals    (1001) rivals    (1001)     3465 2023-02-17 15:45:14.000000 dipwmsearch-0.1.8/src/AhoCorasick.py
+-rw-------   0 rivals    (1001) rivals    (1001)    11344 2023-02-22 09:25:42.000000 dipwmsearch-0.1.8/src/Block.py
+-rw-------   0 rivals    (1001) rivals    (1001)     3306 2022-12-31 18:32:39.000000 dipwmsearch-0.1.8/src/Enumerate.py
+-rw-------   0 rivals    (1001) rivals    (1001)    10836 2022-12-31 18:32:39.000000 dipwmsearch-0.1.8/src/SemiNaive.py
+-rw-------   0 rivals    (1001) rivals    (1001)      590 2023-01-05 13:30:16.000000 dipwmsearch-0.1.8/src/__init__.py
+-rw-------   0 rivals    (1001) rivals    (1001)     5144 2023-02-22 10:20:38.000000 dipwmsearch-0.1.8/src/__main__.py
+-rw-------   0 rivals    (1001) rivals    (1001)    18556 2023-02-17 15:45:14.000000 dipwmsearch-0.1.8/src/diPwm.py
+drwx------   0 rivals    (1001) rivals    (1001)        0 2023-04-14 16:50:17.934685 dipwmsearch-0.1.8/test/
+-rw-------   0 rivals    (1001) rivals    (1001)      429 2022-12-31 18:32:39.000000 dipwmsearch-0.1.8/test/test_Aho.py
+-rw-------   0 rivals    (1001) rivals    (1001)     2366 2022-12-31 18:32:39.000000 dipwmsearch-0.1.8/test/test_Block.py
+-rw-------   0 rivals    (1001) rivals    (1001)     1045 2022-12-31 18:32:39.000000 dipwmsearch-0.1.8/test/test_Enumerate.py
+-rw-------   0 rivals    (1001) rivals    (1001)     1349 2023-02-17 15:45:14.000000 dipwmsearch-0.1.8/test/test_Pvalue.py
+-rw-------   0 rivals    (1001) rivals    (1001)     7778 2022-12-31 18:32:39.000000 dipwmsearch-0.1.8/test/test_SemiNaive.py
+-rw-------   0 rivals    (1001) rivals    (1001)     1583 2022-12-31 18:32:39.000000 dipwmsearch-0.1.8/test/test_diPWM.py
+-rw-------   0 rivals    (1001) rivals    (1001)     1860 2022-12-31 18:32:39.000000 dipwmsearch-0.1.8/test/test_diPWM_file.py
```

### Comparing `dipwmsearch-0.1.7/LICENSE.txt` & `dipwmsearch-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/PKG-INFO` & `dipwmsearch-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipwmsearch
-Version: 0.1.7
+Version: 0.1.8
 Summary: Provides functions to search for any di-nucleotidic Position Weight Matrix (di-PWM) in a genomic sequence (IUPAC compliant).
 Author-email: Marie Mille <m.mariemille@gmail.com>, Bastien Cazaux <bast.cazaux@gmail.com>, Julie Ripoll <julie.ripoll@lirmm.fr>, Eric Rivals <rivals@lirmm.fr>
 License: A package dedicated to search for diPWM motifs in a sequence or a text. Copyright CNRS 2021-; by Marie Mille, Bastien Cazaux, Julie Ripoll and Eric Rivals.
         Contact email : dipwm@lirmm.fr
```

### Comparing `dipwmsearch-0.1.7/README.md` & `dipwmsearch-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/dipwmsearch.egg-info/PKG-INFO` & `dipwmsearch-0.1.8/dipwmsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipwmsearch
-Version: 0.1.7
+Version: 0.1.8
 Summary: Provides functions to search for any di-nucleotidic Position Weight Matrix (di-PWM) in a genomic sequence (IUPAC compliant).
 Author-email: Marie Mille <m.mariemille@gmail.com>, Bastien Cazaux <bast.cazaux@gmail.com>, Julie Ripoll <julie.ripoll@lirmm.fr>, Eric Rivals <rivals@lirmm.fr>
 License: A package dedicated to search for diPWM motifs in a sequence or a text. Copyright CNRS 2021-; by Marie Mille, Bastien Cazaux, Julie Ripoll and Eric Rivals.
         Contact email : dipwm@lirmm.fr
```

### Comparing `dipwmsearch-0.1.7/pyproject.toml` & `dipwmsearch-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dipwmsearch"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Marie Mille", email="m.mariemille@gmail.com" },
   { name="Bastien Cazaux", email="bast.cazaux@gmail.com" },
   { name="Julie Ripoll", email="julie.ripoll@lirmm.fr" },
   { name="Eric Rivals", email="rivals@lirmm.fr" },
 ]
 description = "Provides functions to search for any di-nucleotidic Position Weight Matrix (di-PWM) in a genomic sequence (IUPAC compliant)."
```

### Comparing `dipwmsearch-0.1.7/src/AhoCorasick.py` & `dipwmsearch-0.1.8/src/AhoCorasick.py`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/src/Block.py` & `dipwmsearch-0.1.8/src/Block.py`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/src/Enumerate.py` & `dipwmsearch-0.1.8/src/Enumerate.py`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/src/SemiNaive.py` & `dipwmsearch-0.1.8/src/SemiNaive.py`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/src/__init__.py` & `dipwmsearch-0.1.8/src/__init__.py`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/src/__main__.py` & `dipwmsearch-0.1.8/src/__main__.py`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/src/diPwm.py` & `dipwmsearch-0.1.8/src/diPwm.py`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/test/test_Block.py` & `dipwmsearch-0.1.8/test/test_Block.py`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/test/test_Enumerate.py` & `dipwmsearch-0.1.8/test/test_Enumerate.py`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/test/test_Pvalue.py` & `dipwmsearch-0.1.8/test/test_Pvalue.py`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/test/test_SemiNaive.py` & `dipwmsearch-0.1.8/test/test_SemiNaive.py`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/test/test_diPWM.py` & `dipwmsearch-0.1.8/test/test_diPWM.py`

 * *Files identical despite different names*

### Comparing `dipwmsearch-0.1.7/test/test_diPWM_file.py` & `dipwmsearch-0.1.8/test/test_diPWM_file.py`

 * *Files identical despite different names*

