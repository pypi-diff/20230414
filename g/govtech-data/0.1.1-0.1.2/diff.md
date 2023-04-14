# Comparing `tmp/govtech_data-0.1.1.tar.gz` & `tmp/govtech_data-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govtech_data-0.1.1.tar", max compression
+gzip compressed data, was "govtech_data-0.1.2.tar", max compression
```

## Comparing `govtech_data-0.1.1.tar` & `govtech_data-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,14 @@
--rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.1/README.md
--rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.1/govtech_data/__init__.py
--rw-r--r--   0        0        0     3143 2023-04-14 10:06:22.322708 govtech_data-0.1.1/govtech_data/client.py
--rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.1/govtech_data/models/__init__.py
--rw-r--r--   0        0        0      187 2023-04-14 06:22:56.953684 govtech_data-0.1.1/govtech_data/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      907 2023-04-14 09:25:09.266500 govtech_data-0.1.1/govtech_data/models/__pycache__/api.cpython-310.pyc
--rw-r--r--   0        0        0      349 2023-04-14 09:18:13.465611 govtech_data-0.1.1/govtech_data/models/api.py
--rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.1/govtech_data/models/resources/__init__.py
--rw-r--r--   0        0        0      197 2023-04-14 07:45:03.425736 govtech_data-0.1.1/govtech_data/models/resources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      854 2023-04-14 09:27:05.144157 govtech_data-0.1.1/govtech_data/models/resources/__pycache__/package_list.cpython-310.pyc
--rw-r--r--   0        0        0     5700 2023-04-14 09:27:05.145341 govtech_data-0.1.1/govtech_data/models/resources/__pycache__/package_show.cpython-310.pyc
--rw-r--r--   0        0        0     2851 2023-04-14 09:27:05.150383 govtech_data-0.1.1/govtech_data/models/resources/__pycache__/resource_show.cpython-310.pyc
--rw-r--r--   0        0        0     1541 2023-04-14 09:27:05.352977 govtech_data-0.1.1/govtech_data/models/resources/datastore_search.py
--rw-r--r--   0        0        0      407 2023-04-14 09:27:05.287711 govtech_data-0.1.1/govtech_data/models/resources/package_list.py
--rw-r--r--   0        0        0     4441 2023-04-14 09:27:05.332541 govtech_data-0.1.1/govtech_data/models/resources/package_show.py
--rw-r--r--   0        0        0     1994 2023-04-14 09:27:05.372624 govtech_data-0.1.1/govtech_data/models/resources/resource_show.py
--rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.1/govtech_data/utils/__init__.py
--rw-r--r--   0        0        0      186 2023-04-14 05:44:50.989776 govtech_data-0.1.1/govtech_data/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1392 2023-04-14 08:17:29.977018 govtech_data-0.1.1/govtech_data/utils/__pycache__/models.cpython-310.pyc
--rw-r--r--   0        0        0     1109 2023-04-14 09:37:13.383824 govtech_data-0.1.1/govtech_data/utils/models.py
--rw-r--r--   0        0        0      761 2023-04-14 10:14:52.463452 govtech_data-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 govtech_data-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.2/README.md
+-rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.2/govtech_data/__init__.py
+-rw-r--r--   0        0        0     3143 2023-04-14 10:06:22.322708 govtech_data-0.1.2/govtech_data/client.py
+-rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.2/govtech_data/models/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-14 09:18:13.465611 govtech_data-0.1.2/govtech_data/models/api.py
+-rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.2/govtech_data/models/resources/__init__.py
+-rw-r--r--   0        0        0     1541 2023-04-14 09:27:05.352977 govtech_data-0.1.2/govtech_data/models/resources/datastore_search.py
+-rw-r--r--   0        0        0      407 2023-04-14 09:27:05.287711 govtech_data-0.1.2/govtech_data/models/resources/package_list.py
+-rw-r--r--   0        0        0     4441 2023-04-14 09:27:05.332541 govtech_data-0.1.2/govtech_data/models/resources/package_show.py
+-rw-r--r--   0        0        0     1994 2023-04-14 09:27:05.372624 govtech_data-0.1.2/govtech_data/models/resources/resource_show.py
+-rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.2/govtech_data/utils/__init__.py
+-rw-r--r--   0        0        0     1109 2023-04-14 09:37:13.383824 govtech_data-0.1.2/govtech_data/utils/models.py
+-rw-r--r--   0        0        0      817 2023-04-14 10:52:31.036713 govtech_data-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 govtech_data-0.1.2/PKG-INFO
```

### Comparing `govtech_data-0.1.1/govtech_data/client.py` & `govtech_data-0.1.2/govtech_data/client.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.1/govtech_data/models/resources/datastore_search.py` & `govtech_data-0.1.2/govtech_data/models/resources/datastore_search.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.1/govtech_data/models/resources/package_show.py` & `govtech_data-0.1.2/govtech_data/models/resources/package_show.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.1/govtech_data/models/resources/resource_show.py` & `govtech_data-0.1.2/govtech_data/models/resources/resource_show.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.1/govtech_data/utils/models.py` & `govtech_data-0.1.2/govtech_data/utils/models.py`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.1/pyproject.toml` & `govtech_data-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "govtech-data"
-version = "0.1.1"
+version = "0.1.2"
 description = "Library to easily access and read data from data.gov.sg"
 authors = ["Khee-Chin Chua <kheechin@gmail.com>"]
 license = "Singapore Open Data License"
 readme = "README.md"
 packages = [{include = "govtech_data"}]
+repository = "https://github.com/merlin83/govtech-data"
 
 [tool.poetry.dependencies]
 black = "^23.3.0"
 datamodel-code-generator = "^0.17.2"
 fuzzywuzzy = "^0.18.0"
 loguru = "^0.7.0"
 pydantic = "^1.10.7"
```

### Comparing `govtech_data-0.1.1/PKG-INFO` & `govtech_data-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: govtech-data
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library to easily access and read data from data.gov.sg
+Home-page: https://github.com/merlin83/govtech-data
 License: Singapore Open Data License
 Author: Khee-Chin Chua
 Author-email: kheechin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -14,10 +15,11 @@
 Requires-Dist: datamodel-code-generator (>=0.17.2,<0.18.0)
 Requires-Dist: fuzzywuzzy (>=0.18.0,<0.19.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-levenshtein (>=0.20.9,<0.21.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
+Project-URL: Repository, https://github.com/merlin83/govtech-data
 Description-Content-Type: text/markdown
```

