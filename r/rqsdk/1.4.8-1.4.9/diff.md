# Comparing `tmp/rqsdk-1.4.8.tar.gz` & `tmp/rqsdk-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rqsdk-1.4.8.tar", last modified: Thu Oct 13 07:06:25 2022, max compression
+gzip compressed data, was "dist/rqsdk-1.4.9.tar", last modified: Fri Nov 11 08:11:12 2022, max compression
```

## Comparing `rqsdk-1.4.8.tar` & `rqsdk-1.4.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-10-13 07:06:25.661508 rqsdk-1.4.8/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      256 2022-10-13 07:06:15.000000 rqsdk-1.4.8/HISTORY.md
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      173 2022-10-13 07:06:15.000000 rqsdk-1.4.8/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      736 2022-10-13 07:06:25.661508 rqsdk-1.4.8/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1111 2022-10-13 07:06:15.000000 rqsdk-1.4.8/README.md
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-10-13 07:06:25.664508 rqsdk-1.4.8/rqsdk/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      752 2022-10-13 07:06:15.000000 rqsdk-1.4.8/rqsdk/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      680 2022-10-13 07:06:15.000000 rqsdk-1.4.8/rqsdk/__main__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      497 2022-10-13 07:06:25.664508 rqsdk-1.4.8/rqsdk/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    12452 2022-10-13 07:06:15.000000 rqsdk-1.4.8/rqsdk/cmds.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1719 2022-10-13 07:06:15.000000 rqsdk-1.4.8/rqsdk/const.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     6715 2022-10-13 07:06:15.000000 rqsdk-1.4.8/rqsdk/license_helper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      319 2022-10-13 07:06:15.000000 rqsdk-1.4.8/rqsdk/proxy_helper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2453 2022-10-13 07:06:15.000000 rqsdk-1.4.8/rqsdk/script_update.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      741 2022-10-13 07:06:15.000000 rqsdk-1.4.8/rqsdk/testing.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-10-13 07:06:25.661508 rqsdk-1.4.8/rqsdk.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      736 2022-10-13 07:06:25.000000 rqsdk-1.4.8/rqsdk.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      438 2022-10-13 07:06:25.000000 rqsdk-1.4.8/rqsdk.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2022-10-13 07:06:25.000000 rqsdk-1.4.8/rqsdk.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)       44 2022-10-13 07:06:25.000000 rqsdk-1.4.8/rqsdk.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2022-10-13 07:06:25.000000 rqsdk-1.4.8/rqsdk.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2994 2022-10-13 07:06:25.000000 rqsdk-1.4.8/rqsdk.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)        6 2022-10-13 07:06:25.000000 rqsdk-1.4.8/rqsdk.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)      244 2022-10-13 07:06:25.662508 rqsdk-1.4.8/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3258 2022-10-13 07:06:15.000000 rqsdk-1.4.8/setup.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1001)    79815 2022-10-13 07:06:15.000000 rqsdk-1.4.8/versioneer.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-11-11 08:11:12.621627 rqsdk-1.4.9/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      256 2022-11-11 08:11:07.000000 rqsdk-1.4.9/HISTORY.md
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      173 2022-11-11 08:11:07.000000 rqsdk-1.4.9/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      736 2022-11-11 08:11:12.621627 rqsdk-1.4.9/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1111 2022-11-11 08:11:07.000000 rqsdk-1.4.9/README.md
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-11-11 08:11:12.622627 rqsdk-1.4.9/rqsdk/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      752 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      680 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/__main__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      497 2022-11-11 08:11:12.622627 rqsdk-1.4.9/rqsdk/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    12452 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/cmds.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     1719 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/const.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     6715 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/license_helper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      319 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/proxy_helper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2453 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/script_update.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      741 2022-11-11 08:11:07.000000 rqsdk-1.4.9/rqsdk/testing.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1001)        0 2022-11-11 08:11:12.621627 rqsdk-1.4.9/rqsdk.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      736 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      438 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)       44 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        1 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     2994 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)        6 2022-11-11 08:11:12.000000 rqsdk-1.4.9/rqsdk.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)      244 2022-11-11 08:11:12.622627 rqsdk-1.4.9/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)     3258 2022-11-11 08:11:07.000000 rqsdk-1.4.9/setup.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1001)    79815 2022-11-11 08:11:07.000000 rqsdk-1.4.9/versioneer.py
```

### Comparing `rqsdk-1.4.8/PKG-INFO` & `rqsdk-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqsdk
-Version: 1.4.8
+Version: 1.4.9
 Summary: Ricequant Native SDK
 Home-page: https://www.ricequant.com/
 Author: Ricequant
 Author-email: public@ricequant.com
 License: UNKNOWN
 Keywords: rqsdk
 Platform: UNKNOWN
```

### Comparing `rqsdk-1.4.8/README.md` & `rqsdk-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.8/rqsdk/__init__.py` & `rqsdk-1.4.9/rqsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.8/rqsdk/__main__.py` & `rqsdk-1.4.9/rqsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.8/rqsdk/cmds.py` & `rqsdk-1.4.9/rqsdk/cmds.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.8/rqsdk/const.py` & `rqsdk-1.4.9/rqsdk/const.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.8/rqsdk/license_helper.py` & `rqsdk-1.4.9/rqsdk/license_helper.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.8/rqsdk/script_update.py` & `rqsdk-1.4.9/rqsdk/script_update.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.8/rqsdk/testing.py` & `rqsdk-1.4.9/rqsdk/testing.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.4.8/rqsdk.egg-info/PKG-INFO` & `rqsdk-1.4.9/rqsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqsdk
-Version: 1.4.8
+Version: 1.4.9
 Summary: Ricequant Native SDK
 Home-page: https://www.ricequant.com/
 Author: Ricequant
 Author-email: public@ricequant.com
 License: UNKNOWN
 Keywords: rqsdk
 Platform: UNKNOWN
```

### Comparing `rqsdk-1.4.8/rqsdk.egg-info/requires.txt` & `rqsdk-1.4.9/rqsdk.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-wcwidth
-statsmodels>=0.12.1
-click>=7.0
-rqdatac>=2.9.44
-pyjwt==1.7.1
+tabulate
 patsy>=0.5.1
+rqdatac>=2.9.44
+click>=7.0
+statsmodels>=0.12.1
 pandas>=0.24.2
-tabulate
-rqdatac_fund==1.0.*,>=1.0.18
 requests
+pyjwt==1.7.1
+rqdatac_fund==1.0.*,>=1.0.18
+wcwidth
 
 [:python_version <= "3.6"]
-numpy>=1.19.5
-python-rapidjson<=1.5
 cryptography==2.9.2
+python-rapidjson<=1.5
+numpy>=1.19.5
 
 [:python_version <= "3.7"]
 scipy<=1.7.3
 
 [:python_version == "3.7"]
 numpy>=1.20.0
 
 [:python_version > "3.7"]
 cryptography<=36.0.2,>=2.9.2
 
 [:python_version >= "3.8"]
-scipy>=1.8.0
 numpy>=1.23.0
+scipy>=1.8.0
 
 [rqalpha_plus]
-rqdatac>=2.9.44
-hdf5plugin
-click>=7.0
-rqalpha-mod-incremental==0.0.6
-h5py>=3.0.0
-rqalpha-plus==4.2.2
-pyjwt==1.7.1
-patsy>=0.5.1
-rqalpha-mod-ricequant-data==2.3.*,>=2.3.7
-rqalpha-mod-spot==1.0.*,>=1.0.8
 matplotlib<=3.5.0
-rqdatac_fund==1.0.*,>=1.0.18
-requests
-rqalpha==4.12.0
+tabulate
 rqalpha-mod-optimizer2==1.0.*,>=1.0.8
+rqalpha-mod-rqfactor==1.0.10
 rqrisk==1.0.3
-wcwidth
-statsmodels>=0.12.1
+rqalpha-plus==4.2.2
+click>=7.0
 rqalpha-mod-option==1.1.*,>=1.1.19
-rqfactor==1.3.*,>=1.3.1
-ta-lib==0.4.20
-pandas>=0.24.2
+requests
+hdf5plugin
+rqdatac_fund==1.0.*,>=1.0.18
+patsy>=0.5.1
+wcwidth
+rqalpha-mod-incremental==0.0.7
+rqalpha==4.13.0
 rqalpha-mod-convertible==1.2.*,>=1.2.14
-rqalpha-mod-rqfactor==1.0.10
-tabulate
+rqalpha-mod-spot==1.0.*,>=1.0.8
 rqalpha-mod-fund==0.0.11
+rqalpha-mod-ricequant-data==2.3.*,>=2.3.8
+rqdatac>=2.9.44
+ta-lib==0.4.20
+statsmodels>=0.12.1
+pandas>=0.24.2
+h5py>=3.0.0
+pyjwt==1.7.1
+rqfactor==1.3.*,>=1.3.1
 
 [rqalpha_plus:python_version <= "3.6"]
 python-rapidjson<=1.5
-cryptography==2.9.2
 numpy>=1.19.5
+cryptography==2.9.2
 
 [rqalpha_plus:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqalpha_plus:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqalpha_plus:python_version > "3.7"]
 cryptography<=36.0.2,>=2.9.2
 
 [rqalpha_plus:python_version >= "3.8"]
-scipy>=1.8.0
 numpy>=1.23.0
+scipy>=1.8.0
 
 [rqdatac]
-wcwidth
-statsmodels>=0.12.1
-click>=7.0
-rqdatac>=2.9.44
-pyjwt==1.7.1
+tabulate
 patsy>=0.5.1
+rqdatac>=2.9.44
+click>=7.0
+statsmodels>=0.12.1
 pandas>=0.24.2
-tabulate
-rqdatac_fund==1.0.*,>=1.0.18
 requests
+pyjwt==1.7.1
+rqdatac_fund==1.0.*,>=1.0.18
+wcwidth
 
 [rqdatac:python_version <= "3.6"]
-numpy>=1.19.5
-python-rapidjson<=1.5
 cryptography==2.9.2
+python-rapidjson<=1.5
+numpy>=1.19.5
 
 [rqdatac:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqdatac:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqdatac:python_version > "3.7"]
 cryptography<=36.0.2,>=2.9.2
 
 [rqdatac:python_version >= "3.8"]
-scipy>=1.8.0
 numpy>=1.23.0
+scipy>=1.8.0
 
 [rqfactor]
-rqdatac>=2.9.44
+tabulate
 click>=7.0
-pyjwt==1.7.1
-patsy>=0.5.1
-rqdatac_fund==1.0.*,>=1.0.18
 requests
+rqdatac_fund==1.0.*,>=1.0.18
+patsy>=0.5.1
 wcwidth
-statsmodels>=0.12.1
-rqfactor==1.3.*,>=1.3.1
+rqdatac>=2.9.44
 ta-lib==0.4.20
+statsmodels>=0.12.1
 pandas>=0.24.2
-tabulate
+pyjwt==1.7.1
+rqfactor==1.3.*,>=1.3.1
 
 [rqfactor:python_version <= "3.6"]
 python-rapidjson<=1.5
-cryptography==2.9.2
 numpy>=1.19.5
+cryptography==2.9.2
 
 [rqfactor:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqfactor:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqfactor:python_version > "3.7"]
 cryptography<=36.0.2,>=2.9.2
 
 [rqfactor:python_version >= "3.8"]
-scipy>=1.8.0
 numpy>=1.23.0
+scipy>=1.8.0
 
 [rqoptimizer]
-rqdatac>=2.9.44
+tabulate
 click>=7.0
-pyjwt==1.7.1
-patsy>=0.5.1
-scs==2.1.4
-rqdatac_fund==1.0.*,>=1.0.18
+rqoptimizer2==1.2.*,>=1.2.17
 requests
 osqp==0.6.2.post5
+rqdatac_fund==1.0.*,>=1.0.18
+patsy>=0.5.1
 wcwidth
+scs==2.1.4
+rqdatac>=2.9.44
+rqoptimizer==1.2.*,>=1.2.17
 statsmodels>=0.12.1
-ecos==2.0.10
 pandas>=0.24.2
-rqoptimizer==1.2.*,>=1.2.17
-tabulate
-rqoptimizer2==1.2.*,>=1.2.17
+pyjwt==1.7.1
+ecos==2.0.10
 
 [rqoptimizer:python_version <= "3.6"]
 python-rapidjson<=1.5
-cryptography==2.9.2
 numpy>=1.19.5
+cryptography==2.9.2
 
 [rqoptimizer:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqoptimizer:python_version == "3.6"]
 cvxpy==1.1.18
 
@@ -169,9 +169,9 @@
 [rqoptimizer:python_version > "3.7"]
 cryptography<=36.0.2,>=2.9.2
 
 [rqoptimizer:python_version >= "3.7"]
 cvxpy==1.2.0
 
 [rqoptimizer:python_version >= "3.8"]
-scipy>=1.8.0
 numpy>=1.23.0
+scipy>=1.8.0
```

### Comparing `rqsdk-1.4.8/setup.py` & `rqsdk-1.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,23 +34,23 @@
     "cvxpy==1.1.18 ; python_version == '3.6'",
     "cvxpy==1.2.0 ; python_version >= '3.7'",
     "osqp==0.6.2.post5",
     "rqoptimizer==1.2.*,>=1.2.17",
     "rqoptimizer2==1.2.*,>=1.2.17",
 }
 version_map["rqalpha_plus"] = version_map["rqfactor"] | {
-    "rqalpha==4.12.0",
+    "rqalpha==4.13.0",
     "rqalpha-mod-option==1.1.*,>=1.1.19",
     "rqalpha-mod-optimizer2==1.0.*, >=1.0.8",
     "rqalpha-mod-convertible==1.2.*,>=1.2.14",
-    "rqalpha-mod-ricequant-data==2.3.*,>=2.3.7",
+    "rqalpha-mod-ricequant-data==2.3.*,>=2.3.8",
     "rqalpha-mod-rqfactor==1.0.10",
     "rqalpha-mod-spot==1.0.*,>=1.0.8",
     "rqalpha-mod-fund==0.0.11",
-    "rqalpha-mod-incremental==0.0.6",
+    "rqalpha-mod-incremental==0.0.7",
     "rqalpha-plus==4.2.2",
     "rqrisk==1.0.3",
     "h5py>=3.0.0",
     "hdf5plugin",
     # 3.6.0 在 pycharm 中画图存在问题，待 3.6.1 发布后可移除这一限制
     # https://youtrack.jetbrains.com/issue/PY-56370
     # https://github.com/matplotlib/matplotlib/pull/23912
```

### Comparing `rqsdk-1.4.8/versioneer.py` & `rqsdk-1.4.9/versioneer.py`

 * *Files identical despite different names*

