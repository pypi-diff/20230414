# Comparing `tmp/fca-algorithms-0.2.2.tar.gz` & `tmp/fca-algorithms-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fca-algorithms-0.2.2.tar", last modified: Wed Mar 29 16:55:10 2023, max compression
+gzip compressed data, was "fca-algorithms-0.2.3.tar", last modified: Fri Apr 14 13:02:32 2023, max compression
```

## Comparing `fca-algorithms-0.2.2.tar` & `fca-algorithms-0.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:55:10.876899 fca-algorithms-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)    18655 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2307 2023-03-29 16:55:10.875898 fca-algorithms-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1964 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-29 16:55:10.876899 fca-algorithms-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:55:10.861897 fca-algorithms-0.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:55:10.865898 fca-algorithms-0.2.2/src/fca/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4898 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/api_models.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/association_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     2366 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/base_models.py
--rw-rw-rw-   0 root         (0) root         (0)     2769 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/border_hasse.py
--rw-rw-rw-   0 root         (0) root         (0)     1795 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/get_lattice.py
--rw-rw-rw-   0 root         (0) root         (0)     2524 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/in_close.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:55:10.867898 fca-algorithms-0.2.2/src/fca/plot/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7164 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/plot/plot.py
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/plot/tikz_tpl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:55:10.869898 fca-algorithms-0.2.2/src/fca/rca/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/rca/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2523 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/rca/cpop.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/rca/models.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/rca/p18n.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/rca/rca.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/rca/rca_mickael.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:55:10.870898 fca-algorithms-0.2.2/src/fca/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/scripts/export_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/scripts/fca_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2979 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/scripts/import_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:55:10.871898 fca-algorithms-0.2.2/src/fca/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1847 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/fca/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:55:10.874899 fca-algorithms-0.2.2/src/fca_algorithms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2307 2023-03-29 16:55:10.000000 fca-algorithms-0.2.2/src/fca_algorithms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      920 2023-03-29 16:55:10.000000 fca-algorithms-0.2.2/src/fca_algorithms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 16:55:10.000000 fca-algorithms-0.2.2/src/fca_algorithms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-03-29 16:55:10.000000 fca-algorithms-0.2.2/src/fca_algorithms.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-03-29 16:55:10.000000 fca-algorithms-0.2.2/src/fca_algorithms.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-29 16:55:10.000000 fca-algorithms-0.2.2/src/fca_algorithms.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:55:10.875898 fca-algorithms-0.2.2/src/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2915 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/tests/test_in_close.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-03-29 16:54:36.000000 fca-algorithms-0.2.2/src/tests/test_rca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:02:32.162160 fca-algorithms-0.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)    18655 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-04-14 13:02:32.162160 fca-algorithms-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 13:02:32.163077 fca-algorithms-0.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:02:32.148977 fca-algorithms-0.2.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:02:32.153910 fca-algorithms-0.2.3/src/fca/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4898 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/api_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/association_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     2366 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/base_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2769 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/border_hasse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1800 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/get_lattice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2524 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/in_close.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:02:32.154826 fca-algorithms-0.2.3/src/fca/plot/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7164 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/plot/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/plot/tikz_tpl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:02:32.156660 fca-algorithms-0.2.3/src/fca/rca/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/rca/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2523 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/rca/cpop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/rca/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/rca/p18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/rca/rca.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/rca/rca_mickael.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:02:32.158493 fca-algorithms-0.2.3/src/fca/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/scripts/export_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/scripts/fca_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2979 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/scripts/import_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:02:32.158493 fca-algorithms-0.2.3/src/fca/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1847 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/fca/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:02:32.160327 fca-algorithms-0.2.3/src/fca_algorithms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-04-14 13:02:32.000000 fca-algorithms-0.2.3/src/fca_algorithms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      920 2023-04-14 13:02:32.000000 fca-algorithms-0.2.3/src/fca_algorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 13:02:32.000000 fca-algorithms-0.2.3/src/fca_algorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-14 13:02:32.000000 fca-algorithms-0.2.3/src/fca_algorithms.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-14 13:02:32.000000 fca-algorithms-0.2.3/src/fca_algorithms.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-14 13:02:32.000000 fca-algorithms-0.2.3/src/fca_algorithms.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:02:32.162160 fca-algorithms-0.2.3/src/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2915 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/tests/test_in_close.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-04-14 13:01:59.000000 fca-algorithms-0.2.3/src/tests/test_rca.py
```

### Comparing `fca-algorithms-0.2.2/LICENSE` & `fca-algorithms-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/PKG-INFO` & `fca-algorithms-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fca-algorithms
-Version: 0.2.2
+Version: 0.2.3
 Summary: FCA basic algorithms
 Author: Ramshell
 Author-email: ramshellcinox@gmail.com
 License: CC By 4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `fca-algorithms-0.2.2/README.md` & `fca-algorithms-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/setup.py` & `fca-algorithms-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fca-algorithms",
-    version="0.2.2",
+    version="0.2.3",
     author="Ramshell",
     author_email="ramshellcinox@gmail.com",
     license="CC By 4.0",
     description="FCA basic algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `fca-algorithms-0.2.2/src/fca/api_models.py` & `fca-algorithms-0.2.3/src/fca/api_models.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca/association_rules.py` & `fca-algorithms-0.2.3/src/fca/association_rules.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca/base_models.py` & `fca-algorithms-0.2.3/src/fca/base_models.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca/border_hasse.py` & `fca-algorithms-0.2.3/src/fca/border_hasse.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca/get_lattice.py` & `fca-algorithms-0.2.3/src/fca/get_lattice.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,10 +45,10 @@
             if is_related_to_all:
                 objects_with_all_attributes.append(i)
         return Concept(ctx, objects_with_all_attributes,
                        [j for j in range(len(ctx.A))])
 
     def _has_bottom(self, ctx, concepts) -> bool:
         for concept in concepts:
-            if len(concept.A) == ctx.A:
+            if len(concept.A) == len(ctx.A):
                 return True
         return False
```

### Comparing `fca-algorithms-0.2.2/src/fca/in_close.py` & `fca-algorithms-0.2.3/src/fca/in_close.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca/plot/plot.py` & `fca-algorithms-0.2.3/src/fca/plot/plot.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca/rca/cpop.py` & `fca-algorithms-0.2.3/src/fca/rca/cpop.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca/rca/models.py` & `fca-algorithms-0.2.3/src/fca/rca/models.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca/rca/rca.py` & `fca-algorithms-0.2.3/src/fca/rca/rca.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca/rca/rca_mickael.py` & `fca-algorithms-0.2.3/src/fca/rca/rca_mickael.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca/scripts/export_utils.py` & `fca-algorithms-0.2.3/src/fca/scripts/export_utils.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca/scripts/fca_cli.py` & `fca-algorithms-0.2.3/src/fca/scripts/fca_cli.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca/scripts/import_utils.py` & `fca-algorithms-0.2.3/src/fca/scripts/import_utils.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca/utils/utils.py` & `fca-algorithms-0.2.3/src/fca/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/fca_algorithms.egg-info/PKG-INFO` & `fca-algorithms-0.2.3/src/fca_algorithms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fca-algorithms
-Version: 0.2.2
+Version: 0.2.3
 Summary: FCA basic algorithms
 Author: Ramshell
 Author-email: ramshellcinox@gmail.com
 License: CC By 4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `fca-algorithms-0.2.2/src/fca_algorithms.egg-info/SOURCES.txt` & `fca-algorithms-0.2.3/src/fca_algorithms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/tests/conftest.py` & `fca-algorithms-0.2.3/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/tests/test_in_close.py` & `fca-algorithms-0.2.3/src/tests/test_in_close.py`

 * *Files identical despite different names*

### Comparing `fca-algorithms-0.2.2/src/tests/test_rca.py` & `fca-algorithms-0.2.3/src/tests/test_rca.py`

 * *Files identical despite different names*

