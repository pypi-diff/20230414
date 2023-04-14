# Comparing `tmp/ddr_analysis_tools-0.0.7.tar.gz` & `tmp/ddr_analysis_tools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddr_analysis_tools-0.0.7.tar", last modified: Sat Mar 25 11:59:43 2023, max compression
+gzip compressed data, was "ddr_analysis_tools-0.0.8.tar", last modified: Fri Apr 14 08:01:50 2023, max compression
```

## Comparing `ddr_analysis_tools-0.0.7.tar` & `ddr_analysis_tools-0.0.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:59:43.094365 ddr_analysis_tools-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-25 11:59:43.094365 ddr_analysis_tools-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 11:59:43.094365 ddr_analysis_tools-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:59:43.086365 ddr_analysis_tools-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:59:43.090365 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/ddr_FFT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/ddr_POD.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/ddr_PSD_welch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/ddr_SPOD.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:59:43.090365 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:59:43.090365 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/emulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/emulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/emulation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/emulation/neural_nets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:59:43.090365 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/pod/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/pod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/pod/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/pod/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/pod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:59:43.094365 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/spod/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/spod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32217 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/spod/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/spod/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/spod/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)    27252 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/spod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:59:43.094365 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    59426 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/utils/postproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/utils/weights.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-25 11:59:34.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:59:43.090365 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-25 11:59:43.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-25 11:59:43.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 11:59:43.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-25 11:59:43.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-25 11:59:43.000000 ddr_analysis_tools-0.0.7/src/ddr_analysis_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:01:50.289246 ddr_analysis_tools-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-14 08:01:50.289246 ddr_analysis_tools-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:01:50.289246 ddr_analysis_tools-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:01:50.281246 ddr_analysis_tools-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:01:50.281246 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/ddr_FFT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/ddr_POD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/ddr_PSD_welch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/ddr_SPOD.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:01:50.285246 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:01:50.285246 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/emulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/emulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/emulation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/emulation/neural_nets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:01:50.285246 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/pod/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/pod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/pod/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/pod/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/pod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:01:50.285246 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/spod/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/spod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32217 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/spod/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/spod/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/spod/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27252 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/spod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:01:50.289246 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59426 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/utils/postproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/utils/weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 08:01:39.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:01:50.285246 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-14 08:01:50.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-14 08:01:50.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:01:50.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 08:01:50.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 08:01:50.000000 ddr_analysis_tools-0.0.8/src/ddr_analysis_tools.egg-info/top_level.txt
```

### Comparing `ddr_analysis_tools-0.0.7/LICENSE.txt` & `ddr_analysis_tools-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/PKG-INFO` & `ddr_analysis_tools-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddr_analysis_tools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package for data analysis tools
 Home-page: https://github.com/ddrathod121294/ddr_analysis_tools
 Author: Darshan Rathod
 Author-email: darshan.rathod1994@gmail.com
 Keywords: ddr,time series data analysis,data analysis,POD,SPOD,FFT,ddr_FFT,ddr_SPOD,ddr_PODddr_analysis_tools
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `ddr_analysis_tools-0.0.7/setup.py` & `ddr_analysis_tools-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/ddr_FFT.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/ddr_FFT.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/ddr_PSD_welch.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/ddr_PSD_welch.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         if scale == "loglog":
             ax.loglog(xdata, ydata, label=label, **kwargs)
         else:
             ax.plot(xdata, ydata, label=label, **kwargs)
 
         ax.set_xlabel(xlabel)
         ax.set_ylabel(ylabel)
-        ax.grid()
 
         return ax
 
     def filtered_PSD(self, N: int = 20, Wn: list | float = 1, btype: str = 'highpass') -> tuple[np.ndarray, np.ndarray]:
         """_summary_
 
         Parameters
```

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/ddr_SPOD.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/ddr_SPOD.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/emulation/base.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/emulation/base.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/emulation/neural_nets.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/emulation/neural_nets.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/pod/base.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/pod/base.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/pod/standard.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/pod/standard.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/pod/utils.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/pod/utils.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/spod/base.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/spod/base.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/spod/standard.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/spod/standard.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/spod/streaming.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/spod/streaming.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/spod/utils.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/spod/utils.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/utils/errors.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/utils/errors.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/utils/io.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/utils/io.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/utils/parallel.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/utils/postproc.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/utils/postproc.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/pyspod_local/utils/weights.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/pyspod_local/utils/weights.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools/utils.py` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools/utils.py`

 * *Files identical despite different names*

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools.egg-info/PKG-INFO` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddr-analysis-tools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package for data analysis tools
 Home-page: https://github.com/ddrathod121294/ddr_analysis_tools
 Author: Darshan Rathod
 Author-email: darshan.rathod1994@gmail.com
 Keywords: ddr,time series data analysis,data analysis,POD,SPOD,FFT,ddr_FFT,ddr_SPOD,ddr_PODddr_analysis_tools
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `ddr_analysis_tools-0.0.7/src/ddr_analysis_tools.egg-info/SOURCES.txt` & `ddr_analysis_tools-0.0.8/src/ddr_analysis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

