# Comparing `tmp/gradio_client-0.1.2.tar.gz` & `tmp/gradio_client-0.1.2b1.tar.gz`

## Comparing `gradio_client-0.1.2.tar` & `gradio_client-0.1.2b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.1.2/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.1.2/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.1.2/gradio_client/__init__.py
--rw-r--r--   0        0        0    45304 2020-02-02 00:00:00.000000 gradio_client-0.1.2/gradio_client/client.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.1.2/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 gradio_client-0.1.2/gradio_client/documentation.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.1.2/gradio_client/media_data.py
--rw-r--r--   0        0        0    19981 2020-02-02 00:00:00.000000 gradio_client-0.1.2/gradio_client/serializing.py
--rw-r--r--   0        0        0    13725 2020-02-02 00:00:00.000000 gradio_client-0.1.2/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.1.2/gradio_client/version.txt
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.1.2/.gitignore
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/__init__.py
+-rw-r--r--   0        0        0    45304 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/client.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/media_data.py
+-rw-r--r--   0        0        0    19981 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/serializing.py
+-rw-r--r--   0        0        0    13725 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/utils.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/gradio_client/version.txt
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/.gitignore
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/pyproject.toml
+-rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 gradio_client-0.1.2b1/PKG-INFO
```

### Comparing `gradio_client-0.1.2/README.md` & `gradio_client-0.1.2b1/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.2/gradio_client/client.py` & `gradio_client-0.1.2b1/gradio_client/client.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.2/gradio_client/documentation.py` & `gradio_client-0.1.2b1/gradio_client/documentation.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.2/gradio_client/media_data.py` & `gradio_client-0.1.2b1/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.2/gradio_client/serializing.py` & `gradio_client-0.1.2b1/gradio_client/serializing.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.2/gradio_client/utils.py` & `gradio_client-0.1.2b1/gradio_client/utils.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.2/.gitignore` & `gradio_client-0.1.2b1/.gitignore`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.2/pyproject.toml` & `gradio_client-0.1.2b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradio_client-0.1.2/PKG-INFO` & `gradio_client-0.1.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.1.2
+Version: 0.1.2b1
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Requires-Python: >=3.7
 Requires-Dist: fsspec
```

