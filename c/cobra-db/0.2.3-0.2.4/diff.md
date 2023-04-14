# Comparing `tmp/cobra_db-0.2.3.tar.gz` & `tmp/cobra_db-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobra_db-0.2.3.tar", max compression
+gzip compressed data, was "cobra_db-0.2.4.tar", max compression
```

## Comparing `cobra_db-0.2.3.tar` & `cobra_db-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0      609 2023-04-05 15:03:04.412490 cobra_db-0.2.3/LICENSE
--rw-r--r--   0        0        0     3540 2023-04-05 15:03:04.412490 cobra_db-0.2.3/README.md
--rw-r--r--   0        0        0     1803 2023-04-05 15:03:55.350191 cobra_db-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      332 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/__init__.py
--rw-r--r--   0        0        0     2160 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/dataset_mod.py
--rw-r--r--   0        0        0     4177 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/deid.py
--rw-r--r--   0        0        0    18585 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/deid_recipe.txt
--rw-r--r--   0        0        0     2382 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/deid_recipe_mr.txt
--rw-r--r--   0        0        0     4423 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/encrypt.py
--rw-r--r--   0        0        0     4603 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/enums.py
--rw-r--r--   0        0        0     2266 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/filesystem.py
--rw-r--r--   0        0        0    17338 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/model.py
--rw-r--r--   0        0        0    19218 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/mongo_dao.py
--rw-r--r--   0        0        0        0 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/scripts/__init__.py
--rw-r--r--   0        0        0     9731 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/scripts/pseudonymize_image_metadata.py
--rw-r--r--   0        0        0    13064 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/scripts/stage_1_ingest_images.py
--rw-r--r--   0        0        0     2508 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/scripts/stage_2.py
--rw-r--r--   0        0        0     2397 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/scripts/stage_2_group_patients.py
--rw-r--r--   0        0        0     4709 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/scripts/stage_2_group_series.py
--rw-r--r--   0        0        0     5058 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/scripts/stage_2_group_studies.py
--rw-r--r--   0        0        0     1042 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/scripts/utils.py
--rw-r--r--   0        0        0      535 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/types.py
--rw-r--r--   0        0        0     4635 2023-04-05 15:03:04.432491 cobra_db-0.2.3/src/cobra_db/utils.py
--rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 cobra_db-0.2.3/PKG-INFO
+-rwxr-xr-x   0        0        0      609 2023-04-14 11:52:48.232131 cobra_db-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3540 2023-04-14 11:52:48.232131 cobra_db-0.2.4/README.md
+-rw-r--r--   0        0        0     1813 2023-04-14 11:53:31.316266 cobra_db-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      332 2023-04-14 11:52:48.248131 cobra_db-0.2.4/src/cobra_db/__init__.py
+-rw-r--r--   0        0        0     2160 2023-04-14 11:52:48.248131 cobra_db-0.2.4/src/cobra_db/dataset_mod.py
+-rw-r--r--   0        0        0     4177 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/deid.py
+-rw-r--r--   0        0        0    18585 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/deid_recipe.txt
+-rw-r--r--   0        0        0     2382 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/deid_recipe_mr.txt
+-rw-r--r--   0        0        0     4423 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/encrypt.py
+-rw-r--r--   0        0        0     4603 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/enums.py
+-rw-r--r--   0        0        0     2266 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/filesystem.py
+-rw-r--r--   0        0        0    17338 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/model.py
+-rw-r--r--   0        0        0    19218 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/mongo_dao.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/__init__.py
+-rw-r--r--   0        0        0     9731 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/pseudonymize_image_metadata.py
+-rw-r--r--   0        0        0    13064 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/stage_1_ingest_images.py
+-rw-r--r--   0        0        0     2508 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/stage_2.py
+-rw-r--r--   0        0        0     2397 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/stage_2_group_patients.py
+-rw-r--r--   0        0        0     4709 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/stage_2_group_series.py
+-rw-r--r--   0        0        0     5058 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/stage_2_group_studies.py
+-rw-r--r--   0        0        0     1042 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/scripts/utils.py
+-rw-r--r--   0        0        0      535 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/types.py
+-rw-r--r--   0        0        0     4635 2023-04-14 11:52:48.252131 cobra_db-0.2.4/src/cobra_db/utils.py
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 cobra_db-0.2.4/PKG-INFO
```

### Comparing `cobra_db-0.2.3/LICENSE` & `cobra_db-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/README.md` & `cobra_db-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/pyproject.toml` & `cobra_db-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "cobra_db"
-version = "0.2.3"
+version = "0.2.4"
 description = "COnsolidated BReast cancer Analysis DataBase"
-authors = ["Fernando Cossio", "Apostolia Tsirikoglou", "Haiko Schurz", "Fredrik Strand"]
+authors = ["Fernando Cossio", "Apostolia Tsirikoglou", "Haiko Schurz", "Hui Li", "Fredrik Strand"]
 license = "Apache License 2.0"
 readme = "README.md"
 include = ["src/cobra_db/deid_recipe.txt"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydicom = "^2.3.0"
```

### Comparing `cobra_db-0.2.3/src/cobra_db/dataset_mod.py` & `cobra_db-0.2.4/src/cobra_db/dataset_mod.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/deid.py` & `cobra_db-0.2.4/src/cobra_db/deid.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/deid_recipe.txt` & `cobra_db-0.2.4/src/cobra_db/deid_recipe.txt`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/deid_recipe_mr.txt` & `cobra_db-0.2.4/src/cobra_db/deid_recipe_mr.txt`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/encrypt.py` & `cobra_db-0.2.4/src/cobra_db/encrypt.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/enums.py` & `cobra_db-0.2.4/src/cobra_db/enums.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/filesystem.py` & `cobra_db-0.2.4/src/cobra_db/filesystem.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/model.py` & `cobra_db-0.2.4/src/cobra_db/model.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/mongo_dao.py` & `cobra_db-0.2.4/src/cobra_db/mongo_dao.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/scripts/pseudonymize_image_metadata.py` & `cobra_db-0.2.4/src/cobra_db/scripts/pseudonymize_image_metadata.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/scripts/stage_1_ingest_images.py` & `cobra_db-0.2.4/src/cobra_db/scripts/stage_1_ingest_images.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/scripts/stage_2.py` & `cobra_db-0.2.4/src/cobra_db/scripts/stage_2.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/scripts/stage_2_group_patients.py` & `cobra_db-0.2.4/src/cobra_db/scripts/stage_2_group_patients.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/scripts/stage_2_group_series.py` & `cobra_db-0.2.4/src/cobra_db/scripts/stage_2_group_series.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/scripts/stage_2_group_studies.py` & `cobra_db-0.2.4/src/cobra_db/scripts/stage_2_group_studies.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/scripts/utils.py` & `cobra_db-0.2.4/src/cobra_db/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/types.py` & `cobra_db-0.2.4/src/cobra_db/types.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/src/cobra_db/utils.py` & `cobra_db-0.2.4/src/cobra_db/utils.py`

 * *Files identical despite different names*

### Comparing `cobra_db-0.2.3/PKG-INFO` & `cobra_db-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobra-db
-Version: 0.2.3
+Version: 0.2.4
 Summary: COnsolidated BReast cancer Analysis DataBase
 License: Apache-2.0
 Author: Fernando Cossio
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

