# Comparing `tmp/promsoft_cdek_interface-0.1.2.tar.gz` & `tmp/promsoft_cdek_interface-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promsoft_cdek_interface-0.1.2.tar", max compression
+gzip compressed data, was "promsoft_cdek_interface-0.1.3.tar", max compression
```

## Comparing `promsoft_cdek_interface-0.1.2.tar` & `promsoft_cdek_interface-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      313 2023-04-11 04:47:49.587553 promsoft_cdek_interface-0.1.2/README.md
--rw-r--r--   0        0        0      363 2023-04-11 04:47:49.587553 promsoft_cdek_interface-0.1.2/promsoft_cdek_interface/__init__.py
--rw-r--r--   0        0        0    20275 2023-04-11 05:08:21.468321 promsoft_cdek_interface-0.1.2/promsoft_cdek_interface/models.py
--rw-r--r--   0        0        0      473 2023-04-11 05:08:21.468321 promsoft_cdek_interface-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 promsoft_cdek_interface-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      240 2023-04-14 07:23:36.387574 promsoft_cdek_interface-0.1.3/README.md
+-rw-r--r--   0        0        0      363 2023-04-11 04:47:49.587553 promsoft_cdek_interface-0.1.3/promsoft_cdek_interface/__init__.py
+-rw-r--r--   0        0        0    20275 2023-04-11 05:08:21.468321 promsoft_cdek_interface-0.1.3/promsoft_cdek_interface/models.py
+-rw-r--r--   0        0        0      473 2023-04-14 07:23:36.391574 promsoft_cdek_interface-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 promsoft_cdek_interface-0.1.3/PKG-INFO
```

### Comparing `promsoft_cdek_interface-0.1.2/promsoft_cdek_interface/models.py` & `promsoft_cdek_interface-0.1.3/promsoft_cdek_interface/models.py`

 * *Files identical despite different names*

### Comparing `promsoft_cdek_interface-0.1.2/PKG-INFO` & `promsoft_cdek_interface-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promsoft-cdek-interface
-Version: 0.1.2
+Version: 0.1.3
 Summary: An interface for CDEK HTTP API
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,10 +20,9 @@
 ```python
 from promsoft_cdek_interface import CdekContact
 
 my_contact = CdekContact(name="123")
 print(f"As dict: {my_contact.dict()}")
 ```
 
-Feel free to contribute!
-https://git3.promsoft.ru/karasyuk/cdek_interface
+
```

