# Comparing `tmp/promsoft_weight_calc_interface-0.1.3.tar.gz` & `tmp/promsoft_weight_calc_interface-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promsoft_weight_calc_interface-0.1.3.tar", max compression
+gzip compressed data, was "promsoft_weight_calc_interface-0.1.4.tar", max compression
```

## Comparing `promsoft_weight_calc_interface-0.1.3.tar` & `promsoft_weight_calc_interface-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      477 2023-04-11 10:22:56.136598 promsoft_weight_calc_interface-0.1.3/README.md
--rw-r--r--   0        0        0       68 2023-04-07 05:47:16.006748 promsoft_weight_calc_interface-0.1.3/promsoft_weight_calc_interface/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-07 05:47:16.010748 promsoft_weight_calc_interface-0.1.3/promsoft_weight_calc_interface/models.py
--rw-r--r--   0        0        0      521 2023-04-11 10:22:56.136598 promsoft_weight_calc_interface-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 promsoft_weight_calc_interface-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      392 2023-04-14 07:41:57.164500 promsoft_weight_calc_interface-0.1.4/README.md
+-rw-r--r--   0        0        0       68 2023-04-07 05:47:16.006748 promsoft_weight_calc_interface-0.1.4/promsoft_weight_calc_interface/__init__.py
+-rw-r--r--   0        0        0     1533 2023-04-07 05:47:16.010748 promsoft_weight_calc_interface-0.1.4/promsoft_weight_calc_interface/models.py
+-rw-r--r--   0        0        0      521 2023-04-14 07:41:57.164500 promsoft_weight_calc_interface-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 promsoft_weight_calc_interface-0.1.4/PKG-INFO
```

### Comparing `promsoft_weight_calc_interface-0.1.3/promsoft_weight_calc_interface/models.py` & `promsoft_weight_calc_interface-0.1.4/promsoft_weight_calc_interface/models.py`

 * *Files identical despite different names*

### Comparing `promsoft_weight_calc_interface-0.1.3/pyproject.toml` & `promsoft_weight_calc_interface-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promsoft_weight_calc_interface"
-version = "0.1.3"
+version = "0.1.4"
 description = "Интерфейс для сервиса weight_calc."
 authors = ["Alena Chegodaikina <alena@promsoft.ru>"]
 readme = "README.md"
 packages = [{include = "promsoft_weight_calc_interface"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `promsoft_weight_calc_interface-0.1.3/PKG-INFO` & `promsoft_weight_calc_interface-0.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promsoft-weight-calc-interface
-Version: 0.1.3
+Version: 0.1.4
 Summary: Интерфейс для сервиса weight_calc.
 Author: Alena Chegodaikina
 Author-email: alena@promsoft.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,11 +21,7 @@
 my_entry = Entry(id=10004, cnt=2)
 print(f"Entry as dict: {my_entry.dict()}")
 
 my_compl_entry = ComplEntry(items=[Entry(id=10004, cnt=2), Entry(id=10005, cnt=2)], return_sizes_goods=True)
 print(f"ComplEntry as dict: {my_compl_entry.dict()}")
 
 ```
-
-Feel free to contribute!
-https://git3.promsoft.ru/interfaces/weight_calc_interface
-
```

