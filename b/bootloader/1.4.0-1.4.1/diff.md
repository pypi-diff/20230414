# Comparing `tmp/bootloader-1.4.0.tar.gz` & `tmp/bootloader-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootloader-1.4.0.tar", max compression
+gzip compressed data, was "bootloader-1.4.1.tar", max compression
```

## Comparing `bootloader-1.4.0.tar` & `bootloader-1.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1068 2022-12-19 18:58:28.870281 bootloader-1.4.0/LICENSE
--rw-r--r--   0        0        0     3239 2023-03-07 15:58:25.560681 bootloader-1.4.0/README.md
--rw-r--r--   0        0        0       22 2023-03-08 17:00:11.198309 bootloader-1.4.0/bootloader/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 19:46:32.973881 bootloader-1.4.0/bootloader/commands/__init__.py
--rw-r--r--   0        0        0     6999 2023-03-08 17:00:11.198309 bootloader-1.4.0/bootloader/commands/flash_bt121.py
--rw-r--r--   0        0        0     8588 2023-03-07 23:20:10.512596 bootloader-1.4.0/bootloader/commands/flash_microcontroller.py
--rw-r--r--   0        0        0     8144 2023-03-07 15:56:43.786751 bootloader-1.4.0/bootloader/commands/init.py
--rw-r--r--   0        0        0     3767 2023-03-07 15:58:25.568681 bootloader-1.4.0/bootloader/commands/list.py
--rw-r--r--   0        0        0        0 2023-02-15 16:28:02.234575 bootloader-1.4.0/bootloader/console/__init__.py
--rw-r--r--   0        0        0     1305 2023-03-07 23:19:19.797479 bootloader-1.4.0/bootloader/console/application.py
--rw-r--r--   0        0        0      342 2023-02-15 16:28:02.234575 bootloader-1.4.0/bootloader/console/main.py
--rw-r--r--   0        0        0        0 2023-03-06 19:46:32.989881 bootloader-1.4.0/bootloader/exceptions/__init__.py
--rw-r--r--   0        0        0     3993 2023-03-07 15:56:43.786751 bootloader-1.4.0/bootloader/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-03 16:44:58.455351 bootloader-1.4.0/bootloader/utilities/__init__.py
--rw-r--r--   0        0        0     4222 2023-03-03 21:10:06.988405 bootloader-1.4.0/bootloader/utilities/aws.py
--rw-r--r--   0        0        0     1747 2023-03-07 15:58:25.568681 bootloader-1.4.0/bootloader/utilities/config.py
--rw-r--r--   0        0        0      606 2023-03-03 16:45:23.602951 bootloader-1.4.0/bootloader/utilities/logo.py
--rw-r--r--   0        0        0     2323 2023-03-06 19:46:32.993882 bootloader-1.4.0/bootloader/utilities/system_utils.py
--rw-r--r--   0        0        0      978 2023-03-08 17:00:11.198309 bootloader-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     3830 1970-01-01 00:00:00.000000 bootloader-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-12-19 18:58:28.870281 bootloader-1.4.1/LICENSE
+-rw-r--r--   0        0        0     3239 2023-03-13 20:24:21.945906 bootloader-1.4.1/README.md
+-rw-r--r--   0        0        0       22 2023-04-14 21:16:53.726064 bootloader-1.4.1/bootloader/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-24 17:44:46.556517 bootloader-1.4.1/bootloader/commands/__init__.py
+-rw-r--r--   0        0        0     6999 2023-04-14 21:09:57.642446 bootloader-1.4.1/bootloader/commands/flash_bt121.py
+-rw-r--r--   0        0        0     8588 2023-04-14 21:09:57.642446 bootloader-1.4.1/bootloader/commands/flash_microcontroller.py
+-rw-r--r--   0        0        0     8126 2023-04-14 21:16:18.417382 bootloader-1.4.1/bootloader/commands/init.py
+-rw-r--r--   0        0        0     3767 2023-04-14 21:09:57.646446 bootloader-1.4.1/bootloader/commands/list.py
+-rw-r--r--   0        0        0        0 2023-03-24 17:39:39.085470 bootloader-1.4.1/bootloader/console/__init__.py
+-rw-r--r--   0        0        0     1305 2023-04-14 21:09:57.650446 bootloader-1.4.1/bootloader/console/application.py
+-rw-r--r--   0        0        0      342 2023-03-24 17:39:50.209378 bootloader-1.4.1/bootloader/console/main.py
+-rw-r--r--   0        0        0        0 2023-04-14 21:09:57.650446 bootloader-1.4.1/bootloader/exceptions/__init__.py
+-rw-r--r--   0        0        0     3993 2023-04-14 21:09:57.650446 bootloader-1.4.1/bootloader/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-27 18:32:24.861693 bootloader-1.4.1/bootloader/utilities/__init__.py
+-rw-r--r--   0        0        0     4222 2023-04-14 21:09:57.654446 bootloader-1.4.1/bootloader/utilities/aws.py
+-rw-r--r--   0        0        0     1747 2023-04-14 21:09:57.654446 bootloader-1.4.1/bootloader/utilities/config.py
+-rw-r--r--   0        0        0      606 2023-04-14 21:09:57.654446 bootloader-1.4.1/bootloader/utilities/logo.py
+-rw-r--r--   0        0        0     2323 2023-04-14 21:09:57.658446 bootloader-1.4.1/bootloader/utilities/system_utils.py
+-rw-r--r--   0        0        0      978 2023-04-14 21:16:42.421845 bootloader-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3830 1970-01-01 00:00:00.000000 bootloader-1.4.1/PKG-INFO
```

### Comparing `bootloader-1.4.0/LICENSE` & `bootloader-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bootloader-1.4.0/README.md` & `bootloader-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bootloader-1.4.0/bootloader/commands/flash_bt121.py` & `bootloader-1.4.1/bootloader/commands/flash_bt121.py`

 * *Files identical despite different names*

### Comparing `bootloader-1.4.0/bootloader/commands/flash_microcontroller.py` & `bootloader-1.4.1/bootloader/commands/flash_microcontroller.py`

 * *Files identical despite different names*

### Comparing `bootloader-1.4.0/bootloader/commands/init.py` & `bootloader-1.4.1/bootloader/commands/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
                 self.line(f"\n\t<info>{tool}</info> <warning>not found.</warning>")
 
                 self.write("\tDownloading...")
 
                 try:
                     # boto3 requires dest be either IOBase or str
                     toolObj = str(Path(_os).joinpath(tool).as_posix())
-                    fxu.download(toolObj, cfg.toolsBucket, str(dest), cfg.dephyProfile)
+                    fxu.download(toolObj, cfg.toolsBucket, str(dest))
                 except bce.EndpointConnectionError as err:
                     raise err
                 except AssertionError as err:
                     raise exceptions.S3DownloadError(
                         cfg.toolsBucket, toolObj, str(dest)
                     ) from err
```

### Comparing `bootloader-1.4.0/bootloader/commands/list.py` & `bootloader-1.4.1/bootloader/commands/list.py`

 * *Files identical despite different names*

### Comparing `bootloader-1.4.0/bootloader/console/application.py` & `bootloader-1.4.1/bootloader/console/application.py`

 * *Files identical despite different names*

### Comparing `bootloader-1.4.0/bootloader/exceptions/exceptions.py` & `bootloader-1.4.1/bootloader/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `bootloader-1.4.0/bootloader/utilities/aws.py` & `bootloader-1.4.1/bootloader/utilities/aws.py`

 * *Files identical despite different names*

### Comparing `bootloader-1.4.0/bootloader/utilities/config.py` & `bootloader-1.4.1/bootloader/utilities/config.py`

 * *Files identical despite different names*

### Comparing `bootloader-1.4.0/bootloader/utilities/logo.py` & `bootloader-1.4.1/bootloader/utilities/logo.py`

 * *Files identical despite different names*

### Comparing `bootloader-1.4.0/bootloader/utilities/system_utils.py` & `bootloader-1.4.1/bootloader/utilities/system_utils.py`

 * *Files identical despite different names*

### Comparing `bootloader-1.4.0/pyproject.toml` & `bootloader-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bootloader"
-version = "1.4.0"
+version = "1.4.1"
 description = "A tool for loading firmware onto Dephy devices."
 authors = ["Jared <jcoughlin@dephy.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `bootloader-1.4.0/PKG-INFO` & `bootloader-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootloader
-Version: 1.4.0
+Version: 1.4.1
 Summary: A tool for loading firmware onto Dephy devices.
 License: MIT
 Author: Jared
 Author-email: jcoughlin@dephy.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

