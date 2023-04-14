# Comparing `tmp/lifeomic_patient_ml_types-7.3.0.tar.gz` & `tmp/lifeomic_patient_ml_types-7.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeomic_patient_ml_types-7.3.0.tar", max compression
+gzip compressed data, was "lifeomic_patient_ml_types-7.4.1.tar", max compression
```

## Comparing `lifeomic_patient_ml_types-7.3.0.tar` & `lifeomic_patient_ml_types-7.4.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    13999 2023-04-10 13:04:24.063575 lifeomic_patient_ml_types-7.3.0/lifeomic_patient_ml_types/schemas.py
--rw-r--r--   0        0        0      664 2023-04-10 13:05:47.262969 lifeomic_patient_ml_types-7.3.0/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.3.0/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.3.0/PKG-INFO
+-rw-r--r--   0        0        0    13999 2023-04-14 13:46:44.313518 lifeomic_patient_ml_types-7.4.1/lifeomic_patient_ml_types/schemas.py
+-rw-r--r--   0        0        0      664 2023-04-14 13:48:13.416859 lifeomic_patient_ml_types-7.4.1/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.4.1/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.4.1/PKG-INFO
```

### Comparing `lifeomic_patient_ml_types-7.3.0/lifeomic_patient_ml_types/schemas.py` & `lifeomic_patient_ml_types-7.4.1/lifeomic_patient_ml_types/schemas.py`

 * *Files identical despite different names*

### Comparing `lifeomic_patient_ml_types-7.3.0/pyproject.toml` & `lifeomic_patient_ml_types-7.4.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lifeomic-patient-ml-types"
-version = "7.3.0"
+version = "7.4.1"
 description = "Shared types for the patient-ml-service repos."
 authors = ["LifeOmic <development@lifeomic.com>"]
 license = "UNLICENSED"
 
 [tool.poe.tasks]
 format = "black lifeomic_patient_ml_types"
 lint = "pyright lifeomic_patient_ml_types"
@@ -12,15 +12,15 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 datamodel-code-generator = "^0.14.0"
 black = "^22.12.0"
 poethepoet = "^0.17.1"
-pyright = "^1.1.285"
+pyright = "^1.1.302"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 include = ["src"]
```

### Comparing `lifeomic_patient_ml_types-7.3.0/setup.py` & `lifeomic_patient_ml_types-7.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['lifeomic_patient_ml_types']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'lifeomic-patient-ml-types',
-    'version': '7.3.0',
+    'version': '7.4.1',
     'description': 'Shared types for the patient-ml-service repos.',
     'long_description': 'None',
     'author': 'LifeOmic',
     'author_email': 'development@lifeomic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

