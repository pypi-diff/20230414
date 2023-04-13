# Comparing `tmp/otoe-0.0.2.tar.gz` & `tmp/otoe-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otoe-0.0.2.tar", last modified: Thu Apr 13 18:52:55 2023, max compression
+gzip compressed data, was "otoe-0.0.3.tar", last modified: Thu Apr 13 23:19:10 2023, max compression
```

## Comparing `otoe-0.0.2.tar` & `otoe-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-13 18:52:55.903335 otoe-0.0.2/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      961 2023-04-13 18:52:55.903208 otoe-0.0.2/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.2/README.md
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-13 18:52:55.902173 otoe-0.0.2/otoe/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-13 18:52:55.902228 otoe-0.0.2/otoe/src/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-13 18:52:55.903018 otoe-0.0.2/otoe/src/otoe.egg-info/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      961 2023-04-13 18:52:55.000000 otoe-0.0.2/otoe/src/otoe.egg-info/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      166 2023-04-13 18:52:55.000000 otoe-0.0.2/otoe/src/otoe.egg-info/SOURCES.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-13 18:52:55.000000 otoe-0.0.2/otoe/src/otoe.egg-info/dependency_links.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-13 18:52:55.000000 otoe-0.0.2/otoe/src/otoe.egg-info/top_level.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-13 18:52:55.903373 otoe-0.0.2/setup.cfg
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1387 2023-04-13 18:50:53.000000 otoe-0.0.2/setup.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-13 23:19:10.905728 otoe-0.0.3/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      961 2023-04-13 23:19:10.905605 otoe-0.0.3/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.3/README.md
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-13 23:19:10.904487 otoe-0.0.3/otoe/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-13 23:19:10.904541 otoe-0.0.3/otoe/src/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-13 23:19:10.905433 otoe-0.0.3/otoe/src/otoe.egg-info/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      961 2023-04-13 23:19:10.000000 otoe-0.0.3/otoe/src/otoe.egg-info/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      206 2023-04-13 23:19:10.000000 otoe-0.0.3/otoe/src/otoe.egg-info/SOURCES.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-13 23:19:10.000000 otoe-0.0.3/otoe/src/otoe.egg-info/dependency_links.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       39 2023-04-13 23:19:10.000000 otoe-0.0.3/otoe/src/otoe.egg-info/entry_points.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-13 23:19:10.000000 otoe-0.0.3/otoe/src/otoe.egg-info/top_level.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-13 23:19:10.905771 otoe-0.0.3/setup.cfg
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1377 2023-04-13 23:18:32.000000 otoe-0.0.3/setup.py
```

### Comparing `otoe-0.0.2/PKG-INFO` & `otoe-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.2
+Version: 0.0.3
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.2/README.md` & `otoe-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `otoe-0.0.2/otoe/src/otoe.egg-info/PKG-INFO` & `otoe-0.0.3/otoe/src/otoe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.2
+Version: 0.0.3
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.2/setup.py` & `otoe-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 srcpath = str(Path(__file__).parent / 'src' / 'otoe_epicker')
 
 setuptools.setup(
     name="otoe",                     # This is the name of the package
-    version="0.0.2",                        # The initial release version
+    version="0.0.3",                        # The initial release version
     author="Yakov Varnaev",                     # Full name of the author
     description="Sort of a UI for espanso configs.",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.11',                # Minimum version requirement of the package
     py_modules=["otoe"],             # Name of the python package
     package_dir={'': 'otoe/src'},     # Directory of the source code of the package
     install_requires=[],                     # Install other dependencies if any
-    # entry_points={
-    #     'console_scripts': [
-    #         'otoe=src:otoe:main',
-    #    ],
-    # }
+    entry_points={
+        'console_scripts': [
+            'otoe=obsidian:main',
+       ],
+    }
 )
```

