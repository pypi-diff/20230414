# Comparing `tmp/openai_pricing_logger-0.0.1.tar.gz` & `tmp/openai_pricing_logger-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_pricing_logger-0.0.1.tar", last modified: Thu Apr 13 21:10:56 2023, max compression
+gzip compressed data, was "openai_pricing_logger-0.0.2.tar", last modified: Fri Apr 14 00:32:35 2023, max compression
```

## Comparing `openai_pricing_logger-0.0.1.tar` & `openai_pricing_logger-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 maxhager   (501) staff       (20)        0 2023-04-13 21:10:56.532738 openai_pricing_logger-0.0.1/
--rw-r--r--   0 maxhager   (501) staff       (20)     1066 2023-04-13 05:31:12.000000 openai_pricing_logger-0.0.1/LICENSE
--rw-r--r--   0 maxhager   (501) staff       (20)      654 2023-04-13 21:10:56.532565 openai_pricing_logger-0.0.1/PKG-INFO
--rw-r--r--   0 maxhager   (501) staff       (20)     1261 2023-04-13 05:38:51.000000 openai_pricing_logger-0.0.1/README.md
-drwxr-xr-x   0 maxhager   (501) staff       (20)        0 2023-04-13 21:10:56.531722 openai_pricing_logger-0.0.1/openai_pricing_logger/
--rw-r--r--   0 maxhager   (501) staff       (20)       40 2023-04-13 04:58:31.000000 openai_pricing_logger-0.0.1/openai_pricing_logger/__init__.py
--rw-r--r--   0 maxhager   (501) staff       (20)     2667 2023-04-13 20:58:51.000000 openai_pricing_logger-0.0.1/openai_pricing_logger/logger.py
-drwxr-xr-x   0 maxhager   (501) staff       (20)        0 2023-04-13 21:10:56.532372 openai_pricing_logger-0.0.1/openai_pricing_logger.egg-info/
--rw-r--r--   0 maxhager   (501) staff       (20)      654 2023-04-13 21:10:56.000000 openai_pricing_logger-0.0.1/openai_pricing_logger.egg-info/PKG-INFO
--rw-r--r--   0 maxhager   (501) staff       (20)      272 2023-04-13 21:10:56.000000 openai_pricing_logger-0.0.1/openai_pricing_logger.egg-info/SOURCES.txt
--rw-r--r--   0 maxhager   (501) staff       (20)        1 2023-04-13 21:10:56.000000 openai_pricing_logger-0.0.1/openai_pricing_logger.egg-info/dependency_links.txt
--rw-r--r--   0 maxhager   (501) staff       (20)       22 2023-04-13 21:10:56.000000 openai_pricing_logger-0.0.1/openai_pricing_logger.egg-info/top_level.txt
--rw-r--r--   0 maxhager   (501) staff       (20)       38 2023-04-13 21:10:56.532783 openai_pricing_logger-0.0.1/setup.cfg
--rw-r--r--   0 maxhager   (501) staff       (20)      838 2023-04-13 21:10:12.000000 openai_pricing_logger-0.0.1/setup.py
+drwxr-xr-x   0 maxhager   (501) staff       (20)        0 2023-04-14 00:32:35.404468 openai_pricing_logger-0.0.2/
+-rw-r--r--   0 maxhager   (501) staff       (20)     1066 2023-04-13 05:31:12.000000 openai_pricing_logger-0.0.2/LICENSE
+-rw-r--r--   0 maxhager   (501) staff       (20)      654 2023-04-14 00:32:35.404235 openai_pricing_logger-0.0.2/PKG-INFO
+-rw-r--r--   0 maxhager   (501) staff       (20)     1261 2023-04-13 05:38:51.000000 openai_pricing_logger-0.0.2/README.md
+drwxr-xr-x   0 maxhager   (501) staff       (20)        0 2023-04-14 00:32:35.403475 openai_pricing_logger-0.0.2/openai_pricing_logger/
+-rw-r--r--   0 maxhager   (501) staff       (20)       40 2023-04-13 04:58:31.000000 openai_pricing_logger-0.0.2/openai_pricing_logger/__init__.py
+-rw-r--r--   0 maxhager   (501) staff       (20)     2667 2023-04-13 20:58:51.000000 openai_pricing_logger-0.0.2/openai_pricing_logger/logger.py
+drwxr-xr-x   0 maxhager   (501) staff       (20)        0 2023-04-14 00:32:35.404047 openai_pricing_logger-0.0.2/openai_pricing_logger.egg-info/
+-rw-r--r--   0 maxhager   (501) staff       (20)      654 2023-04-14 00:32:35.000000 openai_pricing_logger-0.0.2/openai_pricing_logger.egg-info/PKG-INFO
+-rw-r--r--   0 maxhager   (501) staff       (20)      272 2023-04-14 00:32:35.000000 openai_pricing_logger-0.0.2/openai_pricing_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 maxhager   (501) staff       (20)        1 2023-04-14 00:32:35.000000 openai_pricing_logger-0.0.2/openai_pricing_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 maxhager   (501) staff       (20)       22 2023-04-14 00:32:35.000000 openai_pricing_logger-0.0.2/openai_pricing_logger.egg-info/top_level.txt
+-rw-r--r--   0 maxhager   (501) staff       (20)       38 2023-04-14 00:32:35.404505 openai_pricing_logger-0.0.2/setup.cfg
+-rw-r--r--   0 maxhager   (501) staff       (20)      838 2023-04-14 00:31:30.000000 openai_pricing_logger-0.0.2/setup.py
```

### Comparing `openai_pricing_logger-0.0.1/LICENSE` & `openai_pricing_logger-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_pricing_logger-0.0.1/PKG-INFO` & `openai_pricing_logger-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_pricing_logger
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to log OpenAI API costs
 Home-page: https://github.com/yachty66/openai_pricing_logger
 Author: Max Hager
 Author-email: maxhager28@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openai_pricing_logger-0.0.1/README.md` & `openai_pricing_logger-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `openai_pricing_logger-0.0.1/openai_pricing_logger/logger.py` & `openai_pricing_logger-0.0.2/openai_pricing_logger/logger.py`

 * *Files identical despite different names*

### Comparing `openai_pricing_logger-0.0.1/openai_pricing_logger.egg-info/PKG-INFO` & `openai_pricing_logger-0.0.2/openai_pricing_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pricing-logger
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to log OpenAI API costs
 Home-page: https://github.com/yachty66/openai_pricing_logger
 Author: Max Hager
 Author-email: maxhager28@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openai_pricing_logger-0.0.1/setup.py` & `openai_pricing_logger-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="openai_pricing_logger",
-    version="0.0.1",
+    version="0.0.2",
     author="Max Hager",
     author_email="maxhager28@gmail.com",
     description="A package to log OpenAI API costs",
     url="https://github.com/yachty66/openai_pricing_logger",
     packages=find_packages(),
     package_data={"logger_package": ["pricing.json"]},
     include_package_data=True,
```

