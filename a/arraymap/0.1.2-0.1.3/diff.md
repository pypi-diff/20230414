# Comparing `tmp/arraymap-0.1.2.tar.gz` & `tmp/arraymap-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraymap-0.1.2.tar", last modified: Thu Apr 13 00:33:21 2023, max compression
+gzip compressed data, was "arraymap-0.1.3.tar", last modified: Fri Apr 14 17:57:47 2023, max compression
```

## Comparing `arraymap-0.1.2.tar` & `arraymap-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:33:21.326186 arraymap-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-13 00:33:16.000000 arraymap-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 00:33:16.000000 arraymap-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-13 00:33:21.326186 arraymap-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-13 00:33:16.000000 arraymap-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    60830 2023-04-13 00:33:16.000000 arraymap-0.1.2/arraymap.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:33:21.326186 arraymap-0.1.2/arraymap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-13 00:33:21.000000 arraymap-0.1.2/arraymap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 00:33:21.000000 arraymap-0.1.2/arraymap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:33:21.000000 arraymap-0.1.2/arraymap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 00:33:21.000000 arraymap-0.1.2/arraymap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 00:33:21.326186 arraymap-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-13 00:33:16.000000 arraymap-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:33:21.326186 arraymap-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-13 00:33:16.000000 arraymap-0.1.2/test/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    15233 2023-04-13 00:33:16.000000 arraymap-0.1.2/test/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:57:47.078973 arraymap-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-14 17:57:45.000000 arraymap-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 17:57:45.000000 arraymap-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-14 17:57:47.078973 arraymap-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-14 17:57:45.000000 arraymap-0.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    60830 2023-04-14 17:57:45.000000 arraymap-0.1.3/arraymap.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:57:47.074973 arraymap-0.1.3/arraymap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-14 17:57:47.000000 arraymap-0.1.3/arraymap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-14 17:57:47.000000 arraymap-0.1.3/arraymap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:57:47.000000 arraymap-0.1.3/arraymap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 17:57:47.000000 arraymap-0.1.3/arraymap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 17:57:47.000000 arraymap-0.1.3/arraymap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 17:57:47.078973 arraymap-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-14 17:57:45.000000 arraymap-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:57:47.078973 arraymap-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-14 17:57:45.000000 arraymap-0.1.3/test/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15233 2023-04-14 17:57:45.000000 arraymap-0.1.3/test/test_unit.py
```

### Comparing `arraymap-0.1.2/LICENSE.md` & `arraymap-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arraymap-0.1.2/arraymap.c` & `arraymap-0.1.3/arraymap.c`

 * *Files identical despite different names*

### Comparing `arraymap-0.1.2/setup.py` & `arraymap-0.1.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 import typing as tp
 import site
 import os
 
 
-AM_VERSION = "0.1.2"
+AM_VERSION = "0.1.3"
 
 
-with open("README.md") as file:
+with open("README.rst") as file:
     LONG_DESCRIPTION = file.read()
 
 
 def get_ext_dir(*components: tp.Iterable[str]) -> tp.Sequence[str]:
     dirs = []
     for sp in site.getsitepackages():
         fp = os.path.join(sp, *components)
@@ -22,23 +22,37 @@
 
 extension = setuptools.Extension(
     "arraymap",
     ["arraymap.c"],
     include_dirs=get_ext_dir("numpy", "core", "include"),
     library_dirs=get_ext_dir("numpy", "core", "lib"),
     define_macros=[("AM_VERSION", AM_VERSION)],
-    libraries=["npymath"],  # not including mlib at this time
+    libraries=["npymath"],
 )
 
 
 setuptools.setup(
-    author="Christopher Ariza, Brandt Bucher",
+    name="arraymap",
     version=AM_VERSION,
     description="Dictionary-like lookup from NumPy array values to their integer positions",
-    ext_modules=[extension],
-    license="MIT",
     long_description=LONG_DESCRIPTION,
-    long_description_content_type="text/markdown",
-    name="arraymap",
     python_requires=">=3.7.0",
+    install_requires=["numpy>=1.18.5"],
     url="https://github.com/static-frame/arraymap",
+    author="Christopher Ariza, Brandt Bucher",
+    license="MIT",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: POSIX",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
+    ext_modules=[extension],
 )
```

### Comparing `arraymap-0.1.2/test/test_property.py` & `arraymap-0.1.3/test/test_property.py`

 * *Files identical despite different names*

### Comparing `arraymap-0.1.2/test/test_unit.py` & `arraymap-0.1.3/test/test_unit.py`

 * *Files identical despite different names*

