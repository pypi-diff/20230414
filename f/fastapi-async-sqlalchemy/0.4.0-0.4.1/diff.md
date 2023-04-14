# Comparing `tmp/fastapi-async-sqlalchemy-0.4.0.tar.gz` & `tmp/fastapi-async-sqlalchemy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-async-sqlalchemy-0.4.0.tar", last modified: Thu Apr 13 14:04:35 2023, max compression
+gzip compressed data, was "fastapi-async-sqlalchemy-0.4.1.tar", last modified: Fri Apr 14 17:39:01 2023, max compression
```

## Comparing `fastapi-async-sqlalchemy-0.4.0.tar` & `fastapi-async-sqlalchemy-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:04:35.054276 fastapi-async-sqlalchemy-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-13 14:04:35.054276 fastapi-async-sqlalchemy-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:04:35.054276 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:04:35.054276 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-13 14:04:35.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 14:04:35.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:04:35.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:04:35.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 14:04:35.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 14:04:35.000000 fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:04:35.054276 fastapi-async-sqlalchemy-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-13 14:04:26.000000 fastapi-async-sqlalchemy-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:39:01.197147 fastapi-async-sqlalchemy-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 17:38:52.000000 fastapi-async-sqlalchemy-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-14 17:39:01.197147 fastapi-async-sqlalchemy-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-14 17:38:52.000000 fastapi-async-sqlalchemy-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:39:01.197147 fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-14 17:38:52.000000 fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-14 17:38:52.000000 fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-14 17:38:52.000000 fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:38:52.000000 fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:39:01.197147 fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-14 17:39:01.000000 fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 17:39:01.000000 fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:39:01.000000 fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:39:01.000000 fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 17:39:01.000000 fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 17:39:01.000000 fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-14 17:38:52.000000 fastapi-async-sqlalchemy-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:39:01.197147 fastapi-async-sqlalchemy-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-14 17:38:52.000000 fastapi-async-sqlalchemy-0.4.1/setup.py
```

### Comparing `fastapi-async-sqlalchemy-0.4.0/LICENSE` & `fastapi-async-sqlalchemy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-async-sqlalchemy-0.4.0/PKG-INFO` & `fastapi-async-sqlalchemy-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-async-sqlalchemy
-Version: 0.4.0
+Version: 0.4.1
 Summary: SQLAlchemy middleware for FastAPI
 Home-page: https://github.com/h0rn3t/fastapi-async-sqlalchemy.git
 Author: Eugene Shershen
 Author-email: h0rn3t.null@gmail.com
 License: MIT
 Project-URL: Code, https://github.com/h0rn3t/fastapi-async-sqlalchemy
 Project-URL: Issue tracker, https://github.com/h0rn3t/fastapi-async-sqlalchemy/issues
@@ -13,14 +13,16 @@
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fastapi-async-sqlalchemy-0.4.0/README.md` & `fastapi-async-sqlalchemy-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/exceptions.py` & `fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy/middleware.py` & `fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi-async-sqlalchemy-0.4.0/fastapi_async_sqlalchemy.egg-info/PKG-INFO` & `fastapi-async-sqlalchemy-0.4.1/fastapi_async_sqlalchemy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-async-sqlalchemy
-Version: 0.4.0
+Version: 0.4.1
 Summary: SQLAlchemy middleware for FastAPI
 Home-page: https://github.com/h0rn3t/fastapi-async-sqlalchemy.git
 Author: Eugene Shershen
 Author-email: h0rn3t.null@gmail.com
 License: MIT
 Project-URL: Code, https://github.com/h0rn3t/fastapi-async-sqlalchemy
 Project-URL: Issue tracker, https://github.com/h0rn3t/fastapi-async-sqlalchemy/issues
@@ -13,14 +13,16 @@
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fastapi-async-sqlalchemy-0.4.0/setup.py` & `fastapi-async-sqlalchemy-0.4.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,25 +23,27 @@
     description="SQLAlchemy middleware for FastAPI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["fastapi_async_sqlalchemy"],
     package_data={"fastapi_async_sqlalchemy": ["py.typed"]},
     zip_safe=False,
     python_requires=">=3.7",
-    install_requires=["starlette>=0.13.6", "SQLAlchemy>=1.4.11"],
+    install_requires=["starlette>=0.13.6", "SQLAlchemy>=2.0.0"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: AsyncIO",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

