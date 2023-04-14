# Comparing `tmp/pybw-23.4.4.1.tar.gz` & `tmp/pybw-23.4.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pybw-23.4.4.1.tar", last modified: Tue Apr  4 04:14:15 2023, max compression
+gzip compressed data, was "dist\pybw-23.4.4.2.tar", last modified: Tue Apr  4 04:44:23 2023, max compression
```

## Comparing `pybw-23.4.4.1.tar` & `pybw-23.4.4.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 04:14:15.497351 pybw-23.4.4.1/
--rw-rw-rw-   0        0        0      577 2023-04-03 07:29:43.000000 pybw-23.4.4.1/- command.txt
--rw-rw-rw-   0        0        0     1187 2023-03-14 02:03:31.000000 pybw-23.4.4.1/LICENSE
--rw-rw-rw-   0        0        0       17 2023-03-14 02:03:31.000000 pybw-23.4.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0      732 2023-04-04 04:14:15.496372 pybw-23.4.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       40 2023-03-14 02:03:31.000000 pybw-23.4.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 04:14:15.427350 pybw-23.4.4.1/pybw/
--rw-rw-rw-   0        0        0        0 2023-03-14 02:03:31.000000 pybw-23.4.4.1/pybw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:14:15.442366 pybw-23.4.4.1/pybw/ccnb_mod/
--rw-rw-rw-   0        0        0        0 2023-03-14 02:03:31.000000 pybw-23.4.4.1/pybw/ccnb_mod/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:14:15.466351 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/
--rw-rw-rw-   0        0        0    21496 2022-05-07 14:14:53.000000 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/BVAnalysis.py
--rw-rw-rw-   0        0        0    23935 2022-08-21 14:07:41.000000 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/BVAnalysisLi.py
--rw-rw-rw-   0        0        0     5071 2022-05-07 14:14:53.000000 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/BVSEParam.dat
--rw-rw-rw-   0        0        0    24461 2022-08-18 06:43:45.000000 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/Structure.py
--rw-rw-rw-   0        0        0     8889 2022-08-21 07:59:31.000000 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:14:15.476351 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/__pycache__/
--rw-rw-rw-   0        0        0    14330 2022-08-11 03:54:41.000000 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysis.cpython-39.pyc
--rw-rw-rw-   0        0        0    15658 2022-08-21 14:07:58.000000 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysisLi.cpython-39.pyc
--rw-rw-rw-   0        0        0    22032 2022-08-21 07:46:04.000000 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/__pycache__/Structure.cpython-39.pyc
--rw-rw-rw-   0        0        0     8727 2022-08-21 07:59:41.000000 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    43144 2022-05-07 14:14:53.000000 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/bvmparam.dat
--rw-rw-rw-   0        0        0    31000 2022-05-07 14:14:53.000000 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/bvse.dat
--rw-rw-rw-   0        0        0     6500 2022-05-07 14:14:53.000000 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/elements.dat
--rw-rw-rw-   0        0        0     7538 2022-08-18 08:53:58.000000 pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/temp.py
--rw-rw-rw-   0        0        0    17720 2023-03-16 06:53:29.000000 pybw-23.4.4.1/pybw/ccnb_mod/ccnb_mod.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:14:15.478352 pybw-23.4.4.1/pybw/core/
--rw-rw-rw-   0        0        0     2291 2023-04-04 01:55:09.000000 pybw-23.4.4.1/pybw/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:14:15.488352 pybw-23.4.4.1/pybw/tricks/
--rw-rw-rw-   0        0        0      119 2023-03-14 02:03:31.000000 pybw-23.4.4.1/pybw/tricks/__init__.py
--rw-rw-rw-   0        0        0     1042 2023-04-04 02:31:30.000000 pybw-23.4.4.1/pybw/tricks/lazy_import.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:14:15.411350 pybw-23.4.4.1/pybw/utils/
-drwxrwxrwx   0        0        0        0 2023-04-04 04:14:15.491352 pybw-23.4.4.1/pybw/utils/pymatgen/
--rw-rw-rw-   0        0        0     7582 2023-03-14 08:29:49.000000 pybw-23.4.4.1/pybw/utils/pymatgen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:14:15.438356 pybw-23.4.4.1/pybw.egg-info/
--rw-rw-rw-   0        0        0      732 2023-04-04 04:14:15.000000 pybw-23.4.4.1/pybw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2023-04-04 04:14:15.000000 pybw-23.4.4.1/pybw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 04:14:15.000000 pybw-23.4.4.1/pybw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-04 04:14:15.000000 pybw-23.4.4.1/pybw.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2023-04-04 04:14:15.000000 pybw-23.4.4.1/pybw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       17 2023-03-14 02:03:31.000000 pybw-23.4.4.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 04:14:15.497351 pybw-23.4.4.1/setup.cfg
--rw-rw-rw-   0        0        0     3051 2023-04-04 04:14:05.000000 pybw-23.4.4.1/setup.py
--rwxrwxrwx   0        0        0      221 2023-04-03 07:29:43.000000 pybw-23.4.4.1/upload_pypi.bat
+drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.636054 pybw-23.4.4.2/
+-rw-rw-rw-   0        0        0      577 2023-04-03 07:29:43.000000 pybw-23.4.4.2/- command.txt
+-rw-rw-rw-   0        0        0     1187 2023-03-14 02:03:31.000000 pybw-23.4.4.2/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-03-14 02:03:31.000000 pybw-23.4.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      732 2023-04-04 04:44:23.634068 pybw-23.4.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2023-03-14 02:03:31.000000 pybw-23.4.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.566055 pybw-23.4.4.2/pybw/
+-rw-rw-rw-   0        0        0        0 2023-03-14 02:03:31.000000 pybw-23.4.4.2/pybw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.579070 pybw-23.4.4.2/pybw/ccnb_mod/
+-rw-rw-rw-   0        0        0        0 2023-03-14 02:03:31.000000 pybw-23.4.4.2/pybw/ccnb_mod/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.602054 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/
+-rw-rw-rw-   0        0        0    21496 2022-05-07 14:14:53.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/BVAnalysis.py
+-rw-rw-rw-   0        0        0    23935 2022-08-21 14:07:41.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/BVAnalysisLi.py
+-rw-rw-rw-   0        0        0     5071 2022-05-07 14:14:53.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/BVSEParam.dat
+-rw-rw-rw-   0        0        0    24461 2022-08-18 06:43:45.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/Structure.py
+-rw-rw-rw-   0        0        0     8889 2022-08-21 07:59:31.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.623057 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/
+-rw-rw-rw-   0        0        0    14330 2022-08-11 03:54:41.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysis.cpython-39.pyc
+-rw-rw-rw-   0        0        0    15658 2022-08-21 14:07:58.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysisLi.cpython-39.pyc
+-rw-rw-rw-   0        0        0    22032 2022-08-21 07:46:04.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/Structure.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8727 2022-08-21 07:59:41.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    43144 2022-05-07 14:14:53.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/bvmparam.dat
+-rw-rw-rw-   0        0        0    31000 2022-05-07 14:14:53.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/bvse.dat
+-rw-rw-rw-   0        0        0     6500 2022-05-07 14:14:53.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/elements.dat
+-rw-rw-rw-   0        0        0     7538 2022-08-18 08:53:58.000000 pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/temp.py
+-rw-rw-rw-   0        0        0    17720 2023-03-16 06:53:29.000000 pybw-23.4.4.2/pybw/ccnb_mod/ccnb_mod.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.625052 pybw-23.4.4.2/pybw/core/
+-rw-rw-rw-   0        0        0     2361 2023-04-04 04:43:57.000000 pybw-23.4.4.2/pybw/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.629071 pybw-23.4.4.2/pybw/tricks/
+-rw-rw-rw-   0        0        0      119 2023-03-14 02:03:31.000000 pybw-23.4.4.2/pybw/tricks/__init__.py
+-rw-rw-rw-   0        0        0     1042 2023-04-04 02:31:30.000000 pybw-23.4.4.2/pybw/tricks/lazy_import.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.544056 pybw-23.4.4.2/pybw/utils/
+drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.631068 pybw-23.4.4.2/pybw/utils/pymatgen/
+-rw-rw-rw-   0        0        0     7582 2023-03-14 08:29:49.000000 pybw-23.4.4.2/pybw/utils/pymatgen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-04 04:44:23.575053 pybw-23.4.4.2/pybw.egg-info/
+-rw-rw-rw-   0        0        0      732 2023-04-04 04:44:23.000000 pybw-23.4.4.2/pybw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      938 2023-04-04 04:44:23.000000 pybw-23.4.4.2/pybw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-04 04:44:23.000000 pybw-23.4.4.2/pybw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-04 04:44:23.000000 pybw-23.4.4.2/pybw.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2023-04-04 04:44:23.000000 pybw-23.4.4.2/pybw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       17 2023-03-14 02:03:31.000000 pybw-23.4.4.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-04 04:44:23.636054 pybw-23.4.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     3051 2023-04-04 04:44:14.000000 pybw-23.4.4.2/setup.py
+-rwxrwxrwx   0        0        0      221 2023-04-03 07:29:43.000000 pybw-23.4.4.2/upload_pypi.bat
```

### Comparing `pybw-23.4.4.1/- command.txt` & `pybw-23.4.4.2/- command.txt`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/LICENSE` & `pybw-23.4.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/PKG-INFO` & `pybw-23.4.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybw
-Version: 23.4.4.1
+Version: 23.4.4.2
 Summary: pybw
 Home-page: https://gitee.com/pubowei/pybw
 Author: Bowei Pu
 Author-email: pubowei@foxmail.com
 License: MIT
 Project-URL: Docs, https://gitee.com/pubowei/pybw
 Project-URL: Package, https://pypi.org/project/pybw
```

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/BVAnalysis.py` & `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/BVAnalysis.py`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/BVAnalysisLi.py` & `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/BVAnalysisLi.py`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/BVSEParam.dat` & `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/BVSEParam.dat`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/Structure.py` & `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/Structure.py`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/__init__.py` & `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__init__.py`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysis.cpython-39.pyc` & `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysisLi.cpython-39.pyc` & `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/BVAnalysisLi.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/__pycache__/Structure.cpython-39.pyc` & `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/Structure.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/__pycache__/__init__.cpython-39.pyc` & `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/bvmparam.dat` & `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/bvmparam.dat`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/bvse.dat` & `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/bvse.dat`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/elements.dat` & `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/elements.dat`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/bvseLi/temp.py` & `pybw-23.4.4.2/pybw/ccnb_mod/bvseLi/temp.py`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/ccnb_mod/ccnb_mod.py` & `pybw-23.4.4.2/pybw/ccnb_mod/ccnb_mod.py`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/core/__init__.py` & `pybw-23.4.4.2/pybw/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     s = int(sec)
     m, sec = s // 60, s % 60
     h, mins = m // 60, m % 60
     day, hour = h // 24, h % 24
     return {'day': day, 'hour': hour, 'min': mins, 'sec': sec, 's': s}
 
 
+def getsizeof(obj):
+    return sys.getsizeof(pickle.dumps(obj))
+
+
 class EasyPickle():
     '''
     Easy usage for pickle
     '''
     def __init__(self):
         self._function = 'Easy usage for pickle'
```

### Comparing `pybw-23.4.4.1/pybw/tricks/lazy_import.py` & `pybw-23.4.4.2/pybw/tricks/lazy_import.py`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw/utils/pymatgen/__init__.py` & `pybw-23.4.4.2/pybw/utils/pymatgen/__init__.py`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/pybw.egg-info/PKG-INFO` & `pybw-23.4.4.2/pybw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybw
-Version: 23.4.4.1
+Version: 23.4.4.2
 Summary: pybw
 Home-page: https://gitee.com/pubowei/pybw
 Author: Bowei Pu
 Author-email: pubowei@foxmail.com
 License: MIT
 Project-URL: Docs, https://gitee.com/pubowei/pybw
 Project-URL: Package, https://pypi.org/project/pybw
```

### Comparing `pybw-23.4.4.1/pybw.egg-info/SOURCES.txt` & `pybw-23.4.4.2/pybw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybw-23.4.4.1/setup.py` & `pybw-23.4.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name='pybw',
-    version='23.4.4.1',
+    version='23.4.4.2',
     python_requires='>=3.6',
     
     author='Bowei Pu',
     author_email='pubowei@foxmail.com',
     
     description='pybw',
     long_description=readme,
```

