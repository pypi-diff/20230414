# Comparing `tmp/osint-python-starter-service-2.0.6.tar.gz` & `tmp/osint-python-starter-service-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-starter-service-2.0.6.tar", last modified: Thu Apr 13 20:24:22 2023, max compression
+gzip compressed data, was "osint-python-starter-service-2.0.7.tar", last modified: Fri Apr 14 16:06:04 2023, max compression
```

## Comparing `osint-python-starter-service-2.0.6.tar` & `osint-python-starter-service-2.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.6/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1713 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.6/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-13 20:24:22.000000 osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      874 2023-04-13 20:24:22.000000 osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-13 20:24:22.000000 osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-04-13 20:24:22.000000 osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-04-13 20:24:22.000000 osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-04-13 20:23:17.000000 osint-python-starter-service-2.0.6/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/starter_service/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.6/starter_service/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.6/starter_service/api.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6865 2023-04-13 19:34:38.000000 osint-python-starter-service-2.0.6/starter_service/api_server.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4731 2023-04-06 18:13:23.000000 osint-python-starter-service-2.0.6/starter_service/avro_parser.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3061 2023-04-13 19:34:38.000000 osint-python-starter-service-2.0.6/starter_service/base_service.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1264 2023-04-13 20:22:15.000000 osint-python-starter-service-2.0.6/starter_service/env.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/starter_service/examples/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.6/starter_service/examples/__init__.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-13 20:24:22.353258 osint-python-starter-service-2.0.6/starter_service/examples/classes/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-13 20:13:48.000000 osint-python-starter-service-2.0.6/starter_service/examples/classes/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2569 2023-04-13 20:19:59.000000 osint-python-starter-service-2.0.6/starter_service/examples/classes/article_raw_en.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      637 2023-04-13 20:19:59.000000 osint-python-starter-service-2.0.6/starter_service/examples/classes/metadata_item_key_en.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      708 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.6/starter_service/examples/error.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      912 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.6/starter_service/examples/manual_kafka.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1298 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.6/starter_service/examples/multi.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1047 2023-04-13 20:22:57.000000 osint-python-starter-service-2.0.6/starter_service/examples/single.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6887 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.6/starter_service/kafka_adapter.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.6/starter_service/messages.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6239 2023-04-12 13:42:48.000000 osint-python-starter-service-2.0.6/starter_service/schemas.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-starter-service-2.0.7/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1713 2023-04-12 12:26:34.000000 osint-python-starter-service-2.0.7/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2184 2023-04-14 16:06:04.000000 osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      874 2023-04-14 16:06:04.000000 osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-04-14 16:06:04.000000 osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      108 2023-04-14 16:06:04.000000 osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       16 2023-04-14 16:06:04.000000 osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      778 2023-04-14 16:02:11.000000 osint-python-starter-service-2.0.7/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/starter_service/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2022-06-04 21:05:58.000000 osint-python-starter-service-2.0.7/starter_service/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      973 2023-04-06 22:41:55.000000 osint-python-starter-service-2.0.7/starter_service/api.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6865 2023-04-13 19:34:38.000000 osint-python-starter-service-2.0.7/starter_service/api_server.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     4731 2023-04-06 18:13:23.000000 osint-python-starter-service-2.0.7/starter_service/avro_parser.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3061 2023-04-13 19:34:38.000000 osint-python-starter-service-2.0.7/starter_service/base_service.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1264 2023-04-13 20:22:15.000000 osint-python-starter-service-2.0.7/starter_service/env.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/starter_service/examples/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-29 02:03:27.000000 osint-python-starter-service-2.0.7/starter_service/examples/__init__.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-14 16:06:04.820448 osint-python-starter-service-2.0.7/starter_service/examples/classes/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-04-14 15:58:14.000000 osint-python-starter-service-2.0.7/starter_service/examples/classes/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2569 2023-04-14 16:03:53.000000 osint-python-starter-service-2.0.7/starter_service/examples/classes/article_raw_en.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      637 2023-04-14 16:03:53.000000 osint-python-starter-service-2.0.7/starter_service/examples/classes/metadata_item_key_en.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      708 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.7/starter_service/examples/error.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      912 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.7/starter_service/examples/manual_kafka.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1298 2023-04-12 12:51:41.000000 osint-python-starter-service-2.0.7/starter_service/examples/multi.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1186 2023-04-14 16:04:08.000000 osint-python-starter-service-2.0.7/starter_service/examples/single.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6887 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.7/starter_service/kafka_adapter.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2023-04-07 10:37:28.000000 osint-python-starter-service-2.0.7/starter_service/messages.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     6392 2023-04-14 16:04:58.000000 osint-python-starter-service-2.0.7/starter_service/schemas.py
```

### Comparing `osint-python-starter-service-2.0.6/LICENSE` & `osint-python-starter-service-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/PKG-INFO` & `osint-python-starter-service-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.0.6/README.md` & `osint-python-starter-service-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/PKG-INFO` & `osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-starter-service
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python starter service
 Home-page: https://github.com/OSINT-VDU-TNO/python-starter-service
 Author: mindpetk
 Author-email: petkeviciusm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `osint-python-starter-service-2.0.6/osint_python_starter_service.egg-info/SOURCES.txt` & `osint-python-starter-service-2.0.7/osint_python_starter_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/setup.py` & `osint-python-starter-service-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 setuptools.setup(
     name="osint-python-starter-service",
-    version="2.0.6",
+    version="2.0.7",
     author="mindpetk",
     author_email="petkeviciusm@gmail.com",
     description="Python starter service",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-starter-service",
     include_package_data=True,
```

### Comparing `osint-python-starter-service-2.0.6/starter_service/api.py` & `osint-python-starter-service-2.0.7/starter_service/api.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/starter_service/api_server.py` & `osint-python-starter-service-2.0.7/starter_service/api_server.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/starter_service/avro_parser.py` & `osint-python-starter-service-2.0.7/starter_service/avro_parser.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/starter_service/base_service.py` & `osint-python-starter-service-2.0.7/starter_service/base_service.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/starter_service/env.py` & `osint-python-starter-service-2.0.7/starter_service/env.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/starter_service/examples/classes/article_raw_en.py` & `osint-python-starter-service-2.0.7/starter_service/examples/classes/article_raw_en.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/starter_service/examples/classes/metadata_item_key_en.py` & `osint-python-starter-service-2.0.7/starter_service/examples/classes/metadata_item_key_en.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/starter_service/examples/error.py` & `osint-python-starter-service-2.0.7/starter_service/examples/error.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/starter_service/examples/manual_kafka.py` & `osint-python-starter-service-2.0.7/starter_service/examples/manual_kafka.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/starter_service/examples/multi.py` & `osint-python-starter-service-2.0.7/starter_service/examples/multi.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/starter_service/examples/single.py` & `osint-python-starter-service-2.0.7/starter_service/examples/single.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import sys
 
 sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
 os.environ['CONSUME'] = 'article_raw_en'
 os.environ['PRODUCE'] = 'metadata_item_key_en'
 os.environ['REST_API_ENABLED'] = 'True'
+os.environ['REST_API_PORT'] = '8081'
+os.environ['KAFKA_HOST'] = 'kafka:9092'
+os.environ['SCHEMA_REGISTRY'] = 'http://schema-registry:8081'
 
 from starter_service.base_service import StarterService
 from starter_service.api import API
 
 
 class SingleRoute(StarterService):
     name = "single"
```

### Comparing `osint-python-starter-service-2.0.6/starter_service/kafka_adapter.py` & `osint-python-starter-service-2.0.7/starter_service/kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/starter_service/messages.py` & `osint-python-starter-service-2.0.7/starter_service/messages.py`

 * *Files identical despite different names*

### Comparing `osint-python-starter-service-2.0.6/starter_service/schemas.py` & `osint-python-starter-service-2.0.7/starter_service/schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 import logging
-import os
 from pathlib import Path
 from pydoc import locate
 from threading import Lock
 
 from starter_service.avro_parser import avsc_to_pydantic
 
-_path = str(Path().absolute())
+_pathlib_path = Path().absolute()
 _logger = logging.getLogger(__name__)
 
 
 class Schema:
 
     def __init__(self, topic=None, filename=None, class_name=None, class_obj=None, full_path=None):
         self.topic = topic
@@ -54,39 +53,42 @@
         self._load_local_schemas()
         # load classes from folder
         self._load_local_classes()
 
     def _load_local_schemas(self):
         # load avro schemas from local folder
         _schemas = []
-        for file in os.listdir(f"{_path}/schemas"):
-            if file.endswith(".avsc") or file.endswith("-value.avsc") or file.endswith("-key.avsc"):
+        schemas_dir = _pathlib_path / "schemas"
+        for file in schemas_dir.iterdir():
+            if file.suffix == ".avsc" or file.suffix == "-value.avsc" or file.suffix == "-key.avsc":
                 _schemas.append(file)
 
         if len(_schemas) == 0:
-            self._logger.warning(f"No schemas found in {_path}/schemas")
+            self._logger.warning(f"No schemas found in {_pathlib_path.absolute()}")
             return
 
         for file in _schemas:
-            self._load_schema_from_file(file)
+            self._load_schema_from_file(file.name)
 
     def _load_local_classes(self):
-        for file in os.listdir(f"{_path}/classes"):
-            if file.endswith(".py") and not file.startswith("__"):
-                topic = file.replace(".py", "")
+        classes_dir = _pathlib_path / "classes"
+        for file in classes_dir.iterdir():
+            if file.suffix == ".py" and file.name != "__init__.py":
+                topic = file.name.replace(".py", "")
                 if topic in self._schemas:
                     continue
                 self._logger.info(f"Loading class {topic} from file {file}")
                 main_class = self._read_main_class_from_file(file)
                 schema = Schema(topic, file, main_class, self._load_class_from_file(f'{topic}.py', main_class), file)
                 self._schemas[topic] = schema
 
     def _read_main_class_from_file(self, file):
         main_class = None
-        with open(f"{_path}/classes/{file}", "r") as f:
+        file_path = _pathlib_path / "classes" / file
+        with open(file_path, "r") as f:
             for line in f.readlines():
                 if line.startswith("main_class"):
                     main_class = line.split(" ")[2].strip()
         return main_class
 
     def register_schema(self, schema: [str, dict], topic: str):
         """
@@ -94,15 +96,16 @@
         :param schema: AVRO string schema
         :param topic: topic to register the schema for
         :param _type: SchemaType Enum (consume or produce)
         :return:
         """
         self._logger.info(f"Registering schema for topic {topic}")
         filename, main_class, python_classes = self._avro_to_file(schema)
-        full_path = os.path.join(_path, "classes", f'{topic}.py')
+
+        full_path = _pathlib_path / "classes" / f'{topic}.py'
         with open(full_path, "w") as f:
             f.write(python_classes)
         schema = Schema(topic, filename, main_class, self._load_class_from_file(f'{topic}.py', main_class), full_path)
         self._schemas[topic] = schema
 
     def _load_class_from_file(self, filename, class_name):
         self._logger.info(f"Loading class from file {filename} with class {class_name}")
@@ -121,46 +124,47 @@
         python_classes, main_class = avsc_to_pydantic(schema)
         filename = f"{class_name.lower()}.py"
         return filename, main_class, python_classes
 
     def _load_schema_from_file(self, filename):
         try:
             self._logger.info(f"Loading schema {filename}")
-            with open(f"{_path}/schemas/{filename}", "r") as f:
+            filepath = _pathlib_path / "schemas" / filename
+            with open(filepath, "r") as f:
                 self.register_schema(f.read(), self._filename_to_topic(filename))
         except Exception as e:
             self._logger.error(f"Error loading schema {filename}: {e}")
 
     def _filename_to_topic(self, filename):
         if filename.endswith("-value.avsc"):
             return filename[:-11].lower()
         if filename.endswith("-key.avsc"):
             return filename[:-9].lower()
         if filename.endswith(".avsc"):
             return filename[:-5].lower()
 
     def _init_dir(self):
-        if not os.path.exists(f"{_path}/classes"):
+        classes_dir = _pathlib_path / "classes"
+        if not classes_dir.exists():
             try:
-                os.makedirs(f"{_path}/classes")
-                with open(f"{_path}/classes/__init__.py", "w") as f:
-                    f.write("")
-                with open(f"{_path}/classes/readme.txt", "w") as f:
-                    f.write("This folder contains all the generated classes from the schemas")
+                classes_dir.mkdir()
+                init_file = classes_dir / "__init__.py"
+                init_file.touch()
+                readme_file = classes_dir / "readme.txt"
+                readme_file.write_text("This folder contains all the generated classes from the schemas")
             except Exception as e:
                 self._logger.error(f"Error creating classes folder {e}")
                 raise e
 
-        if not os.path.exists(f"{_path}/schemas"):
+        schemas_dir = _pathlib_path / "schemas"
+        if not schemas_dir.exists():
             try:
-                os.makedirs(f"{_path}/schemas")
-                with open(f"{_path}/schemas/readme.txt", "w") as f:
-                    f.write(
-                        "Use this folder to provide AVRO schemas"
-                    )
+                schemas_dir.mkdir()
+                readme_file = schemas_dir / "readme.txt"
+                readme_file.write_text("Use this folder to provide AVRO schemas")
             except Exception as e:
                 self._logger.error(f"Error creating schema folder {e}")
                 raise e
 
     def get_schema(self, topic) -> object or dict:
         with self._lock:
             if not topic or topic not in self._schemas:
```

