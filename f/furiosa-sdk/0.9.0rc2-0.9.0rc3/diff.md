# Comparing `tmp/furiosa-sdk-0.9.0rc2.tar.gz` & `tmp/furiosa-sdk-0.9.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-sdk-0.9.0rc2.tar", last modified: Fri Apr 14 20:49:40 2023, max compression
+gzip compressed data, was "furiosa-sdk-0.9.0rc3.tar", last modified: Fri Apr 14 21:26:11 2023, max compression
```

## Comparing `furiosa-sdk-0.9.0rc2.tar` & `furiosa-sdk-0.9.0rc3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      386 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/Makefile
--rw-r--r--   0        0        0     2542 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/README.md
--rw-r--r--   0        0        0     1107 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/docs/Makefile
--rw-r--r--   0        0        0     5330 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/docs/conf.py
--rw-r--r--   0        0        0      670 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/docs/furiosa.rst
--rw-r--r--   0        0        0      470 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/docs/index.rst
--rw-r--r--   0        0        0      795 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/docs/make.bat
--rw-r--r--   0        0        0       18 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/furiosa/sdk/__init__.py
--rw-r--r--   0        0        0     1833 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/pyproject.toml
--rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 furiosa-sdk-0.9.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      386 2023-04-14 21:20:22.940569 furiosa-sdk-0.9.0rc3/Makefile
+-rw-r--r--   0        0        0     2542 2023-04-14 21:20:22.940569 furiosa-sdk-0.9.0rc3/README.md
+-rw-r--r--   0        0        0     1107 2023-04-14 21:20:22.940569 furiosa-sdk-0.9.0rc3/docs/Makefile
+-rw-r--r--   0        0        0     5330 2023-04-14 21:20:22.940569 furiosa-sdk-0.9.0rc3/docs/conf.py
+-rw-r--r--   0        0        0      670 2023-04-14 21:20:22.940569 furiosa-sdk-0.9.0rc3/docs/furiosa.rst
+-rw-r--r--   0        0        0      470 2023-04-14 21:20:22.944569 furiosa-sdk-0.9.0rc3/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-04-14 21:20:22.944569 furiosa-sdk-0.9.0rc3/docs/make.bat
+-rw-r--r--   0        0        0       18 2023-04-14 21:20:22.944569 furiosa-sdk-0.9.0rc3/furiosa/sdk/__init__.py
+-rw-r--r--   0        0        0     1833 2023-04-14 21:20:22.944569 furiosa-sdk-0.9.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 furiosa-sdk-0.9.0rc3/PKG-INFO
```

### Comparing `furiosa-sdk-0.9.0rc2/README.md` & `furiosa-sdk-0.9.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `furiosa-sdk-0.9.0rc2/docs/Makefile` & `furiosa-sdk-0.9.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `furiosa-sdk-0.9.0rc2/docs/conf.py` & `furiosa-sdk-0.9.0rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `furiosa-sdk-0.9.0rc2/docs/furiosa.rst` & `furiosa-sdk-0.9.0rc3/docs/furiosa.rst`

 * *Files identical despite different names*

### Comparing `furiosa-sdk-0.9.0rc2/docs/make.bat` & `furiosa-sdk-0.9.0rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `furiosa-sdk-0.9.0rc2/pyproject.toml` & `furiosa-sdk-0.9.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "furiosa-sdk"
-version = "0.9.0.rc2"
+version = "0.9.0.rc3"
 authors = [{ name = "FurioaAI, Inc.", email = "pkg@furiosa.ai" }]
 readme = "README.md"
 license = { text = "Apache License 2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
```

### Comparing `furiosa-sdk-0.9.0rc2/PKG-INFO` & `furiosa-sdk-0.9.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furiosa-sdk
-Version: 0.9.0rc2
+Version: 0.9.0rc3
 Summary: Furiosa SDK
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

