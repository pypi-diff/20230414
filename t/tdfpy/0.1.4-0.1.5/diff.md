# Comparing `tmp/tdfpy-0.1.4.tar.gz` & `tmp/tdfpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdfpy-0.1.4.tar", last modified: Thu Apr 13 22:23:44 2023, max compression
+gzip compressed data, was "tdfpy-0.1.5.tar", last modified: Thu Apr 13 22:27:15 2023, max compression
```

## Comparing `tdfpy-0.1.4.tar` & `tdfpy-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 22:23:44.548803 tdfpy-0.1.4/
--rw-rw-rw-   0        0        0      444 2023-04-13 22:23:44.547801 tdfpy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      728 2022-09-29 06:32:54.000000 tdfpy-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 22:23:44.548803 tdfpy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      792 2023-04-13 22:23:27.000000 tdfpy-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 22:23:44.531300 tdfpy-0.1.4/tdfpy/
--rw-rw-rw-   0        0        0       33 2022-09-29 01:16:01.000000 tdfpy-0.1.4/tdfpy/__init__.py
--rw-rw-rw-   0        0        0      809 2022-09-28 21:38:22.000000 tdfpy-0.1.4/tdfpy/constants.py
--rw-rw-rw-   0        0        0 13529648 2022-09-28 18:45:28.000000 tdfpy-0.1.4/tdfpy/libtimsdata.so
--rw-rw-rw-   0        0        0     3176 2023-04-13 21:47:32.000000 tdfpy-0.1.4/tdfpy/pandas_tdf.py
--rw-rw-rw-   0        0        0  2861288 2022-09-28 18:45:28.000000 tdfpy-0.1.4/tdfpy/timsdata.dll
--rw-rw-rw-   0        0        0    18058 2023-04-13 21:52:04.000000 tdfpy-0.1.4/tdfpy/timsdata.py
-drwxrwxrwx   0        0        0        0 2023-04-13 22:23:44.545439 tdfpy-0.1.4/tdfpy.egg-info/
--rw-rw-rw-   0        0        0      444 2023-04-13 22:23:44.000000 tdfpy-0.1.4/tdfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-04-13 22:23:44.000000 tdfpy-0.1.4/tdfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 22:23:44.000000 tdfpy-0.1.4/tdfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-13 22:23:44.000000 tdfpy-0.1.4/tdfpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 22:23:44.000000 tdfpy-0.1.4/tdfpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 22:23:44.546764 tdfpy-0.1.4/tests/
--rw-rw-rw-   0        0        0     2422 2023-04-13 21:52:04.000000 tdfpy-0.1.4/tests/test_pandas_tdf.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:27:15.678462 tdfpy-0.1.5/
+-rw-rw-rw-   0        0        0      444 2023-04-13 22:27:15.677456 tdfpy-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      728 2022-09-29 06:32:54.000000 tdfpy-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 22:27:15.678462 tdfpy-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-04-13 22:26:52.000000 tdfpy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:27:15.664905 tdfpy-0.1.5/tdfpy/
+-rw-rw-rw-   0        0        0       33 2022-09-29 01:16:01.000000 tdfpy-0.1.5/tdfpy/__init__.py
+-rw-rw-rw-   0        0        0      809 2022-09-28 21:38:22.000000 tdfpy-0.1.5/tdfpy/constants.py
+-rw-rw-rw-   0        0        0 13529648 2022-09-28 18:45:28.000000 tdfpy-0.1.5/tdfpy/libtimsdata.so
+-rw-rw-rw-   0        0        0     3176 2023-04-13 21:47:32.000000 tdfpy-0.1.5/tdfpy/pandas_tdf.py
+-rw-rw-rw-   0        0        0  2861288 2022-09-28 18:45:28.000000 tdfpy-0.1.5/tdfpy/timsdata.dll
+-rw-rw-rw-   0        0        0    18058 2023-04-13 21:52:04.000000 tdfpy-0.1.5/tdfpy/timsdata.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:27:15.676456 tdfpy-0.1.5/tdfpy.egg-info/
+-rw-rw-rw-   0        0        0      444 2023-04-13 22:27:15.000000 tdfpy-0.1.5/tdfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-04-13 22:27:15.000000 tdfpy-0.1.5/tdfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 22:27:15.000000 tdfpy-0.1.5/tdfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-13 22:27:15.000000 tdfpy-0.1.5/tdfpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 22:27:15.000000 tdfpy-0.1.5/tdfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 22:27:15.677456 tdfpy-0.1.5/tests/
+-rw-rw-rw-   0        0        0     2422 2023-04-13 21:52:04.000000 tdfpy-0.1.5/tests/test_pandas_tdf.py
```

### Comparing `tdfpy-0.1.4/README.md` & `tdfpy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.4/setup.py` & `tdfpy-0.1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 
 setup(
     name='tdfpy',
-    version='0.1.4',
+    version='0.1.5',
     description='Pip package to work with bruker tdf and tdf_bin files',
     url='https://github.com/pgarrett-scripps/tdfpy',
     author='Patrick Garrett',
     author_email='pgarrett@scripps.edu',
     license='MIT',
     packages=['tdfpy'],
     package_dir={'tdfpy': 'tdfpy'},
     include_package_data=True,
     package_data={'tdfpy': ['timsdata.dll', 'libtimsdata.so']},
-    install_requires=['pandas~=1.24.2',
-                      'numpy~=2.0.0',
+    install_requires=['pandas~=2.0.0',
+                      'numpy~=1.24.2',
                       ],
 
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3.10',
```

### Comparing `tdfpy-0.1.4/tdfpy/constants.py` & `tdfpy-0.1.5/tdfpy/constants.py`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.4/tdfpy/libtimsdata.so` & `tdfpy-0.1.5/tdfpy/libtimsdata.so`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.4/tdfpy/pandas_tdf.py` & `tdfpy-0.1.5/tdfpy/pandas_tdf.py`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.4/tdfpy/timsdata.dll` & `tdfpy-0.1.5/tdfpy/timsdata.dll`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.4/tdfpy/timsdata.py` & `tdfpy-0.1.5/tdfpy/timsdata.py`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.4/tests/test_pandas_tdf.py` & `tdfpy-0.1.5/tests/test_pandas_tdf.py`

 * *Files identical despite different names*

