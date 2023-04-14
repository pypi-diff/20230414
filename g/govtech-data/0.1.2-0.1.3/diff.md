# Comparing `tmp/govtech_data-0.1.2.tar.gz` & `tmp/govtech_data-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govtech_data-0.1.2.tar", max compression
+gzip compressed data, was "govtech_data-0.1.3.tar", max compression
```

## Comparing `govtech_data-0.1.2.tar` & `govtech_data-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.2/README.md
--rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.2/govtech_data/__init__.py
--rw-r--r--   0        0        0     3143 2023-04-14 10:06:22.322708 govtech_data-0.1.2/govtech_data/client.py
--rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.2/govtech_data/models/__init__.py
--rw-r--r--   0        0        0      349 2023-04-14 09:18:13.465611 govtech_data-0.1.2/govtech_data/models/api.py
--rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.2/govtech_data/models/resources/__init__.py
--rw-r--r--   0        0        0     1541 2023-04-14 09:27:05.352977 govtech_data-0.1.2/govtech_data/models/resources/datastore_search.py
--rw-r--r--   0        0        0      407 2023-04-14 09:27:05.287711 govtech_data-0.1.2/govtech_data/models/resources/package_list.py
--rw-r--r--   0        0        0     4441 2023-04-14 09:27:05.332541 govtech_data-0.1.2/govtech_data/models/resources/package_show.py
--rw-r--r--   0        0        0     1994 2023-04-14 09:27:05.372624 govtech_data-0.1.2/govtech_data/models/resources/resource_show.py
--rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.2/govtech_data/utils/__init__.py
--rw-r--r--   0        0        0     1109 2023-04-14 09:37:13.383824 govtech_data-0.1.2/govtech_data/utils/models.py
--rw-r--r--   0        0        0      817 2023-04-14 10:52:31.036713 govtech_data-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 govtech_data-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.3/README.md
+-rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.3/govtech_data/__init__.py
+-rw-r--r--   0        0        0     3143 2023-04-14 10:06:22.322708 govtech_data-0.1.3/govtech_data/client.py
+-rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.3/govtech_data/models/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-14 09:18:13.465611 govtech_data-0.1.3/govtech_data/models/api.py
+-rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.3/govtech_data/models/resources/__init__.py
+-rw-r--r--   0        0        0     1541 2023-04-14 09:27:05.352977 govtech_data-0.1.3/govtech_data/models/resources/datastore_search.py
+-rw-r--r--   0        0        0      407 2023-04-14 09:27:05.287711 govtech_data-0.1.3/govtech_data/models/resources/package_list.py
+-rw-r--r--   0        0        0     4441 2023-04-14 09:27:05.332541 govtech_data-0.1.3/govtech_data/models/resources/package_show.py
+-rw-r--r--   0        0        0     1994 2023-04-14 09:27:05.372624 govtech_data-0.1.3/govtech_data/models/resources/resource_show.py
+-rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.3/govtech_data/utils/__init__.py
+-rw-r--r--   0        0        0     1109 2023-04-14 09:37:13.383824 govtech_data-0.1.3/govtech_data/utils/models.py
+-rw-r--r--   0        0        0      867 2023-04-14 17:47:39.163246 govtech_data-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 govtech_data-0.1.3/PKG-INFO
```

### Comparing `govtech_data-0.1.2/govtech_data/client.py` & `govtech_data-0.1.3/govtech_data/client.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.2/govtech_data/models/resources/datastore_search.py` & `govtech_data-0.1.3/govtech_data/models/resources/datastore_search.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.2/govtech_data/models/resources/package_show.py` & `govtech_data-0.1.3/govtech_data/models/resources/package_show.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.2/govtech_data/models/resources/resource_show.py` & `govtech_data-0.1.3/govtech_data/models/resources/resource_show.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.2/govtech_data/utils/models.py` & `govtech_data-0.1.3/govtech_data/utils/models.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.2/pyproject.toml` & `govtech_data-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [tool.poetry]
 name = "govtech-data"
-version = "0.1.2"
+version = "0.1.3"
 description = "Library to easily access and read data from data.gov.sg"
 authors = ["Khee-Chin Chua <kheechin@gmail.com>"]
 license = "Singapore Open Data License"
 readme = "README.md"
 packages = [{include = "govtech_data"}]
 repository = "https://github.com/merlin83/govtech-data"
 
 [tool.poetry.dependencies]
-black = "^23.3.0"
-datamodel-code-generator = "^0.17.2"
 fuzzywuzzy = "^0.18.0"
 loguru = "^0.7.0"
+pandas = "^2.0.0"
 pydantic = "^1.10.7"
 python = "^3.10"
 python-levenshtein = "^0.20.9"
 requests = "^2.28.2"
+
+[tool.poetry.dev-dependencies]
+black = "^23.3.0"
+datamodel-code-generator = "^0.17.2"
 isort = "^5.12.0"
 
 [tool.poetry.scripts]
 generate-models = "govtech_data.utils.models:generate_models"
 
 [tool.isort]
 profile = 'black'
```

### Comparing `govtech_data-0.1.2/PKG-INFO` & `govtech_data-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: govtech-data
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library to easily access and read data from data.gov.sg
 Home-page: https://github.com/merlin83/govtech-data
 License: Singapore Open Data License
 Author: Khee-Chin Chua
 Author-email: kheechin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: black (>=23.3.0,<24.0.0)
-Requires-Dist: datamodel-code-generator (>=0.17.2,<0.18.0)
 Requires-Dist: fuzzywuzzy (>=0.18.0,<0.19.0)
-Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-levenshtein (>=0.20.9,<0.21.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/merlin83/govtech-data
 Description-Content-Type: text/markdown
```

