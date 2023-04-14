# Comparing `tmp/drs-compliance-1.0.0.tar.gz` & `tmp/drs-compliance-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drs-compliance-1.0.0.tar", last modified: Tue Apr 11 14:39:51 2023, max compression
+gzip compressed data, was "drs-compliance-1.0.1.tar", last modified: Fri Apr 14 18:10:23 2023, max compression
```

## Comparing `drs-compliance-1.0.0.tar` & `drs-compliance-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-11 14:39:51.000225 drs-compliance-1.0.0/
--rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-1.0.0/LICENSE
--rw-r--r--   0 ypuligun   (502) staff       (20)     5788 2023-04-11 14:39:50.999792 drs-compliance-1.0.0/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)     5383 2023-04-07 18:32:26.000000 drs-compliance-1.0.0/README.md
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-11 14:39:50.983970 drs-compliance-1.0.0/compliance_suite/
--rw-r--r--   0 ypuligun   (502) staff       (20)        0 2022-11-18 15:12:54.000000 drs-compliance-1.0.0/compliance_suite/__init__.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-06 20:14:45.000000 drs-compliance-1.0.0/compliance_suite/constants.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     6314 2023-04-07 18:32:26.000000 drs-compliance-1.0.0/compliance_suite/helper.py
--rw-r--r--   0 ypuligun   (502) staff       (20)    17151 2023-04-10 19:53:24.000000 drs-compliance-1.0.0/compliance_suite/report_runner.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      544 2023-03-28 19:17:32.000000 drs-compliance-1.0.0/compliance_suite/report_server.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-11 14:39:50.986991 drs-compliance-1.0.0/compliance_suite/schemas/
--rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2022-11-23 19:16:25.000000 drs-compliance-1.0.0/compliance_suite/schemas/service_info.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2022-11-23 19:16:25.000000 drs-compliance-1.0.0/compliance_suite/schemas/service_type.json
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-11 14:39:50.995611 drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/
--rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2022-12-02 15:11:02.000000 drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/access_method.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      799 2022-12-02 15:11:02.000000 drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/access_url.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-03-16 14:44:23.000000 drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/checksum.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-06 20:14:00.000000 drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/contents_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-06 20:14:45.000000 drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/drs_bundle.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-03-24 20:39:33.000000 drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/drs_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      635 2022-12-02 15:11:02.000000 drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/error.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-10 19:53:24.000000 drs-compliance-1.0.0/compliance_suite/validate_drs_object_response.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     3563 2023-04-06 20:06:37.000000 drs-compliance-1.0.0/compliance_suite/validate_response.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-11 14:39:50.999310 drs-compliance-1.0.0/drs_compliance.egg-info/
--rw-r--r--   0 ypuligun   (502) staff       (20)     5788 2023-04-11 14:39:50.000000 drs-compliance-1.0.0/drs_compliance.egg-info/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)      920 2023-04-11 14:39:50.000000 drs-compliance-1.0.0/drs_compliance.egg-info/SOURCES.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-11 14:39:50.000000 drs-compliance-1.0.0/drs_compliance.egg-info/dependency_links.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       71 2023-04-11 14:39:50.000000 drs-compliance-1.0.0/drs_compliance.egg-info/entry_points.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-11 14:39:50.000000 drs-compliance-1.0.0/drs_compliance.egg-info/requires.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-11 14:39:50.000000 drs-compliance-1.0.0/drs_compliance.egg-info/top_level.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-11 14:39:51.001030 drs-compliance-1.0.0/setup.cfg
--rw-r--r--   0 ypuligun   (502) staff       (20)     1259 2023-04-11 14:39:35.000000 drs-compliance-1.0.0/setup.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-14 18:10:23.493146 drs-compliance-1.0.1/
+-rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-1.0.1/LICENSE
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-14 18:10:23.492486 drs-compliance-1.0.1/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7269 2023-04-14 18:07:14.000000 drs-compliance-1.0.1/README.md
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-14 18:10:23.471738 drs-compliance-1.0.1/compliance_suite/
+-rw-r--r--   0 ypuligun   (502) staff       (20)        0 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/__init__.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/constants.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     6314 2023-04-12 18:19:20.000000 drs-compliance-1.0.1/compliance_suite/helper.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)    17151 2023-04-12 18:16:28.000000 drs-compliance-1.0.1/compliance_suite/report_runner.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      557 2023-04-14 18:07:14.000000 drs-compliance-1.0.1/compliance_suite/report_server.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-14 18:10:23.474266 drs-compliance-1.0.1/compliance_suite/schemas/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/service_info.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/service_type.json
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-14 18:10:23.483430 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/access_method.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      799 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/access_url.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/checksum.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/contents_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/drs_bundle.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/drs_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      635 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/error.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/validate_drs_object_response.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3563 2023-04-12 18:08:46.000000 drs-compliance-1.0.1/compliance_suite/validate_response.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-14 18:10:23.491534 drs-compliance-1.0.1/drs_compliance.egg-info/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7674 2023-04-14 18:10:23.000000 drs-compliance-1.0.1/drs_compliance.egg-info/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)      920 2023-04-14 18:10:23.000000 drs-compliance-1.0.1/drs_compliance.egg-info/SOURCES.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-14 18:10:23.000000 drs-compliance-1.0.1/drs_compliance.egg-info/dependency_links.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       71 2023-04-14 18:10:23.000000 drs-compliance-1.0.1/drs_compliance.egg-info/entry_points.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-14 18:10:23.000000 drs-compliance-1.0.1/drs_compliance.egg-info/requires.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-14 18:10:23.000000 drs-compliance-1.0.1/drs_compliance.egg-info/top_level.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-14 18:10:23.494885 drs-compliance-1.0.1/setup.cfg
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1259 2023-04-14 18:07:14.000000 drs-compliance-1.0.1/setup.py
```

### Comparing `drs-compliance-1.0.0/LICENSE` & `drs-compliance-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/compliance_suite/helper.py` & `drs-compliance-1.0.1/compliance_suite/helper.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/compliance_suite/report_runner.py` & `drs-compliance-1.0.1/compliance_suite/report_runner.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/compliance_suite/schemas/service_info.json` & `drs-compliance-1.0.1/compliance_suite/schemas/service_info.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/compliance_suite/schemas/service_type.json` & `drs-compliance-1.0.1/compliance_suite/schemas/service_type.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/access_method.json` & `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/access_method.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/access_url.json` & `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/access_url.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/checksum.json` & `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/checksum.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/contents_object.json` & `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/contents_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/drs_bundle.json` & `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/drs_bundle.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/drs_object.json` & `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/drs_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/compliance_suite/schemas/v1.2.0/error.json` & `drs-compliance-1.0.1/compliance_suite/schemas/v1.2.0/error.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/compliance_suite/validate_drs_object_response.py` & `drs-compliance-1.0.1/compliance_suite/validate_drs_object_response.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/compliance_suite/validate_response.py` & `drs-compliance-1.0.1/compliance_suite/validate_response.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/drs_compliance.egg-info/SOURCES.txt` & `drs-compliance-1.0.1/drs_compliance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drs-compliance-1.0.0/setup.py` & `drs-compliance-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from supported_drs_versions import SUPPORTED_DRS_VERSIONS
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="drs-compliance",
-    version="1.0.0",
+    version="1.0.1",
     author="Yash Puligundla",
     author_email="yasasvini.puligundla@ga4gh.org",
     packages=["compliance_suite"],
     package_data={'compliance_suite': ['config/*', 'schemas/*', 'schemas/v1.2.0/*']},
     description="A compliance utility reporting system for GA4GH DRS server implementations. "
                 "Supports GA4GH DRS versions - " + ",".join(SUPPORTED_DRS_VERSIONS),
     long_description=long_description,
```

