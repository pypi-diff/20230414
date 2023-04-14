# Comparing `tmp/Architectural Lens-0.0.3.tar.gz` & `tmp/Architectural Lens-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Architectural Lens-0.0.3.tar", last modified: Thu Apr  6 10:11:52 2023, max compression
+gzip compressed data, was "Architectural Lens-0.0.4.tar", last modified: Fri Apr 14 10:24:16 2023, max compression
```

## Comparing `Architectural Lens-0.0.3.tar` & `Architectural Lens-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:11:52.719928 Architectural Lens-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:11:52.715928 Architectural Lens-0.0.3/Architectural_Lens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-06 10:11:52.000000 Architectural Lens-0.0.3/Architectural_Lens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-06 10:11:52.000000 Architectural Lens-0.0.3/Architectural_Lens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 10:11:52.000000 Architectural Lens-0.0.3/Architectural_Lens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-06 10:11:52.000000 Architectural Lens-0.0.3/Architectural_Lens.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 10:11:52.000000 Architectural Lens-0.0.3/Architectural_Lens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-06 10:11:52.000000 Architectural Lens-0.0.3/Architectural_Lens.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-06 10:11:52.719928 Architectural Lens-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-06 10:11:52.723928 Architectural Lens-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:11:52.715928 Architectural Lens-0.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/cli_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:11:52.719928 Architectural Lens-0.0.3/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/core/bt_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/core/bt_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/core/bt_module.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:11:52.719928 Architectural Lens-0.0.3/src/plantuml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/plantuml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/plantuml/fetch_git.py
--rw-r--r--   0 runner    (1001) docker     (123)    19854 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/plantuml/plantuml_file_creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:11:52.719928 Architectural Lens-0.0.3/src/plantumlv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/plantumlv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/plantumlv2/pu_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/plantumlv2/pu_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/plantumlv2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:11:52.719928 Architectural Lens-0.0.3/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/utils/config_manager_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-06 10:11:40.000000 Architectural Lens-0.0.3/src/utils/path_manager_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/Architectural_Lens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 10:24:16.000000 Architectural Lens-0.0.4/Architectural_Lens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-14 10:24:16.000000 Architectural Lens-0.0.4/Architectural_Lens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:24:16.000000 Architectural Lens-0.0.4/Architectural_Lens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 10:24:16.000000 Architectural Lens-0.0.4/Architectural_Lens.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 10:24:16.000000 Architectural Lens-0.0.4/Architectural_Lens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 10:24:16.000000 Architectural Lens-0.0.4/Architectural_Lens.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 10:24:16.945555 Architectural Lens-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/cli_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/core/bt_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/core/bt_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/core/bt_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/src/plantuml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantuml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantuml/fetch_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19854 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantuml/plantuml_file_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/src/plantumlv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantumlv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantumlv2/pu_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantumlv2/pu_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/plantumlv2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:16.941555 Architectural Lens-0.0.4/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/utils/config_manager_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-14 10:24:05.000000 Architectural Lens-0.0.4/src/utils/path_manager_singleton.py
```

### Comparing `Architectural Lens-0.0.3/Architectural_Lens.egg-info/SOURCES.txt` & `Architectural Lens-0.0.4/Architectural_Lens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.3/README.md` & `Architectural Lens-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.3/setup.py` & `Architectural Lens-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Architectural Lens",
-    version="0.0.3",
+    version="0.0.4",
     description="Thesis project",
     author="Nikolai Perlt",
     author_email="npe@itu.dk",
     url="https://github.com/Perlten/MT-diagrams",
     packages=find_packages(),
     long_description="This is the long description",
     install_requires=[
```

### Comparing `Architectural Lens-0.0.3/src/cli_interface.py` & `Architectural Lens-0.0.4/src/cli_interface.py`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.3/src/core/bt_file.py` & `Architectural Lens-0.0.4/src/core/bt_file.py`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.3/src/core/bt_graph.py` & `Architectural Lens-0.0.4/src/core/bt_graph.py`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.3/src/core/bt_module.py` & `Architectural Lens-0.0.4/src/core/bt_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,17 +74,15 @@
     def get_module_dependencies(self) -> set["BTModule"]:
         dependencies = set()
         for child in self.file_list:
             dependencies.update(map(lambda e: e.module, child.edge_to))
         return dependencies
 
     def get_dependency_count(self, other: "BTModule"):
-        file_dependencies = other.get_files_recursive()
+        file_dependencies = other.file_list
         files = [
-            edge
-            for element in self.get_files_recursive()
-            for edge in element.edge_to
+            edge for element in self.file_list for edge in element.edge_to
         ]
         count = len(
             [element for element in files if element in file_dependencies]
         )
         return count
```

### Comparing `Architectural Lens-0.0.3/src/plantuml/plantuml_file_creator.py` & `Architectural Lens-0.0.4/src/plantuml/plantuml_file_creator.py`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.3/src/plantumlv2/pu_entities.py` & `Architectural Lens-0.0.4/src/plantumlv2/pu_entities.py`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.3/src/plantumlv2/pu_manager.py` & `Architectural Lens-0.0.4/src/plantumlv2/pu_manager.py`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.3/src/utils/functions.py` & `Architectural Lens-0.0.4/src/utils/functions.py`

 * *Files identical despite different names*

### Comparing `Architectural Lens-0.0.3/src/utils/path_manager_singleton.py` & `Architectural Lens-0.0.4/src/utils/path_manager_singleton.py`

 * *Files identical despite different names*

