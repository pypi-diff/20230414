# Comparing `tmp/polywrap_http_plugin-0.1.0a3.tar.gz` & `tmp/polywrap_http_plugin-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_http_plugin-0.1.0a3.tar", max compression
+gzip compressed data, was "polywrap_http_plugin-0.1.0a4.tar", max compression
```

## Comparing `polywrap_http_plugin-0.1.0a3.tar` & `polywrap_http_plugin-0.1.0a4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       22 2023-04-11 11:16:49.724598 polywrap_http_plugin-0.1.0a3/README.md
--rw-r--r--   0        0        0     3413 2023-04-12 10:16:18.139428 polywrap_http_plugin-0.1.0a3/polywrap_http_plugin/__init__.py
--rw-r--r--   0        0        0    12372 2023-04-11 11:16:49.723724 polywrap_http_plugin-0.1.0a3/polywrap_http_plugin/manifest.json
--rw-r--r--   0        0        0     1156 2023-04-14 13:15:24.660446 polywrap_http_plugin-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0a3/setup.py
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-04-11 11:16:49.724598 polywrap_http_plugin-0.1.0a4/README.md
+-rw-r--r--   0        0        0     3413 2023-04-12 10:16:18.139428 polywrap_http_plugin-0.1.0a4/polywrap_http_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:16:45.789654 polywrap_http_plugin-0.1.0a4/polywrap_http_plugin/py.typed
+-rw-r--r--   0        0        0     1156 2023-04-14 13:19:24.509723 polywrap_http_plugin-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0a4/setup.py
+-rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0a4/PKG-INFO
```

### Comparing `polywrap_http_plugin-0.1.0a3/polywrap_http_plugin/__init__.py` & `polywrap_http_plugin-0.1.0a4/polywrap_http_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0a3/pyproject.toml` & `polywrap_http_plugin-0.1.0a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-http-plugin"
-version = "0.1.0a3"
+version = "0.1.0a4"
 description = ""
 authors = ["Niraj Kamdar <niraj@polywrap.io>"]
 readme = "README.md"
 packages = [{include = "polywrap_http_plugin"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `polywrap_http_plugin-0.1.0a3/setup.py` & `polywrap_http_plugin-0.1.0a4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'polywrap-core>=0.1.0a28,<0.2.0',
  'polywrap-manifest>=0.1.0a28,<0.2.0',
  'polywrap-msgpack>=0.1.0a28,<0.2.0',
  'polywrap-plugin==0.1.0a28']
 
 setup_kwargs = {
     'name': 'polywrap-http-plugin',
-    'version': '0.1.0a3',
+    'version': '0.1.0a4',
     'description': '',
     'long_description': '# Polywrap HTTP Plugin',
     'author': 'Niraj Kamdar',
     'author_email': 'niraj@polywrap.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `polywrap_http_plugin-0.1.0a3/PKG-INFO` & `polywrap_http_plugin-0.1.0a4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polywrap-http-plugin
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: 
 Author: Niraj Kamdar
 Author-email: niraj@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

