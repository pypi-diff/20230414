# Comparing `tmp/readme-metrics-2.2.3.tar.gz` & `tmp/readme-metrics-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme-metrics-2.2.3.tar", last modified: Thu Apr  6 16:06:17 2023, max compression
+gzip compressed data, was "readme-metrics-3.0.0.tar", last modified: Fri Apr 14 14:14:35 2023, max compression
```

## Comparing `readme-metrics-2.2.3.tar` & `readme-metrics-3.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 domh       (501) staff       (20)        0 2023-04-06 16:06:17.022446 readme-metrics-2.2.3/
--rw-r--r--   0 domh       (501) staff       (20)      725 2022-08-22 12:38:51.000000 readme-metrics-2.2.3/LICENSE
--rw-r--r--   0 domh       (501) staff       (20)     2414 2023-04-06 16:06:17.022322 readme-metrics-2.2.3/PKG-INFO
--rw-r--r--   0 domh       (501) staff       (20)     2091 2023-02-22 13:36:42.000000 readme-metrics-2.2.3/README.md
-drwxr-xr-x   0 domh       (501) staff       (20)        0 2023-04-06 16:06:17.021519 readme-metrics-2.2.3/readme_metrics/
--rw-r--r--   0 domh       (501) staff       (20)     3856 2022-09-06 16:49:05.000000 readme-metrics-2.2.3/readme_metrics/Metrics.py
--rw-r--r--   0 domh       (501) staff       (20)     5998 2022-09-06 16:49:05.000000 readme-metrics-2.2.3/readme_metrics/MetricsApiConfig.py
--rw-r--r--   0 domh       (501) staff       (20)     4225 2022-08-22 12:38:51.000000 readme-metrics-2.2.3/readme_metrics/MetricsMiddleware.py
--rw-r--r--   0 domh       (501) staff       (20)    14362 2022-09-15 09:53:54.000000 readme-metrics-2.2.3/readme_metrics/PayloadBuilder.py
--rw-r--r--   0 domh       (501) staff       (20)     1246 2022-04-13 15:12:08.000000 readme-metrics-2.2.3/readme_metrics/ResponseInfoWrapper.py
--rw-r--r--   0 domh       (501) staff       (20)     1058 2022-08-22 12:38:51.000000 readme-metrics-2.2.3/readme_metrics/VerifyWebhook.py
--rw-r--r--   0 domh       (501) staff       (20)      147 2023-04-06 16:02:26.000000 readme-metrics-2.2.3/readme_metrics/__init__.py
--rw-r--r--   0 domh       (501) staff       (20)     1868 2022-09-06 16:49:05.000000 readme-metrics-2.2.3/readme_metrics/django.py
--rw-r--r--   0 domh       (501) staff       (20)     2021 2022-08-24 14:21:21.000000 readme-metrics-2.2.3/readme_metrics/flask_readme.py
--rw-r--r--   0 domh       (501) staff       (20)     1565 2023-02-22 13:36:42.000000 readme-metrics-2.2.3/readme_metrics/publisher.py
--rw-r--r--   0 domh       (501) staff       (20)      357 2022-09-06 09:57:52.000000 readme-metrics-2.2.3/readme_metrics/util.py
-drwxr-xr-x   0 domh       (501) staff       (20)        0 2023-04-06 16:06:17.022146 readme-metrics-2.2.3/readme_metrics.egg-info/
--rw-r--r--   0 domh       (501) staff       (20)     2414 2023-04-06 16:06:16.000000 readme-metrics-2.2.3/readme_metrics.egg-info/PKG-INFO
--rw-r--r--   0 domh       (501) staff       (20)      549 2023-04-06 16:06:16.000000 readme-metrics-2.2.3/readme_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 domh       (501) staff       (20)        1 2023-04-06 16:06:16.000000 readme-metrics-2.2.3/readme_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 domh       (501) staff       (20)       50 2023-04-06 16:06:16.000000 readme-metrics-2.2.3/readme_metrics.egg-info/requires.txt
--rw-r--r--   0 domh       (501) staff       (20)       15 2023-04-06 16:06:16.000000 readme-metrics-2.2.3/readme_metrics.egg-info/top_level.txt
--rw-r--r--   0 domh       (501) staff       (20)       38 2023-04-06 16:06:17.022498 readme-metrics-2.2.3/setup.cfg
--rw-r--r--   0 domh       (501) staff       (20)      650 2022-08-22 12:38:51.000000 readme-metrics-2.2.3/setup.py
+drwxr-xr-x   0 domh       (501) staff       (20)        0 2023-04-14 14:14:35.906556 readme-metrics-3.0.0/
+-rw-r--r--   0 domh       (501) staff       (20)      725 2022-08-22 12:38:51.000000 readme-metrics-3.0.0/LICENSE
+-rw-r--r--   0 domh       (501) staff       (20)     2414 2023-04-14 14:14:35.906420 readme-metrics-3.0.0/PKG-INFO
+-rw-r--r--   0 domh       (501) staff       (20)     2091 2023-02-22 13:36:42.000000 readme-metrics-3.0.0/README.md
+drwxr-xr-x   0 domh       (501) staff       (20)        0 2023-04-14 14:14:35.905538 readme-metrics-3.0.0/readme_metrics/
+-rw-r--r--   0 domh       (501) staff       (20)     3856 2022-09-06 16:49:05.000000 readme-metrics-3.0.0/readme_metrics/Metrics.py
+-rw-r--r--   0 domh       (501) staff       (20)     5998 2022-09-06 16:49:05.000000 readme-metrics-3.0.0/readme_metrics/MetricsApiConfig.py
+-rw-r--r--   0 domh       (501) staff       (20)     4225 2022-08-22 12:38:51.000000 readme-metrics-3.0.0/readme_metrics/MetricsMiddleware.py
+-rw-r--r--   0 domh       (501) staff       (20)    14362 2022-09-15 09:53:54.000000 readme-metrics-3.0.0/readme_metrics/PayloadBuilder.py
+-rw-r--r--   0 domh       (501) staff       (20)     1246 2022-04-13 15:12:08.000000 readme-metrics-3.0.0/readme_metrics/ResponseInfoWrapper.py
+-rw-r--r--   0 domh       (501) staff       (20)     1107 2023-04-14 14:08:19.000000 readme-metrics-3.0.0/readme_metrics/VerifyWebhook.py
+-rw-r--r--   0 domh       (501) staff       (20)      147 2023-04-14 14:12:56.000000 readme-metrics-3.0.0/readme_metrics/__init__.py
+-rw-r--r--   0 domh       (501) staff       (20)     1868 2022-09-06 16:49:05.000000 readme-metrics-3.0.0/readme_metrics/django.py
+-rw-r--r--   0 domh       (501) staff       (20)     2021 2022-08-24 14:21:21.000000 readme-metrics-3.0.0/readme_metrics/flask_readme.py
+-rw-r--r--   0 domh       (501) staff       (20)     1565 2023-02-22 13:36:42.000000 readme-metrics-3.0.0/readme_metrics/publisher.py
+-rw-r--r--   0 domh       (501) staff       (20)      357 2022-09-06 09:57:52.000000 readme-metrics-3.0.0/readme_metrics/util.py
+drwxr-xr-x   0 domh       (501) staff       (20)        0 2023-04-14 14:14:35.906244 readme-metrics-3.0.0/readme_metrics.egg-info/
+-rw-r--r--   0 domh       (501) staff       (20)     2414 2023-04-14 14:14:35.000000 readme-metrics-3.0.0/readme_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 domh       (501) staff       (20)      549 2023-04-14 14:14:35.000000 readme-metrics-3.0.0/readme_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 domh       (501) staff       (20)        1 2023-04-14 14:14:35.000000 readme-metrics-3.0.0/readme_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 domh       (501) staff       (20)       50 2023-04-14 14:14:35.000000 readme-metrics-3.0.0/readme_metrics.egg-info/requires.txt
+-rw-r--r--   0 domh       (501) staff       (20)       15 2023-04-14 14:14:35.000000 readme-metrics-3.0.0/readme_metrics.egg-info/top_level.txt
+-rw-r--r--   0 domh       (501) staff       (20)       38 2023-04-14 14:14:35.906601 readme-metrics-3.0.0/setup.cfg
+-rw-r--r--   0 domh       (501) staff       (20)      650 2022-08-22 12:38:51.000000 readme-metrics-3.0.0/setup.py
```

### Comparing `readme-metrics-2.2.3/LICENSE` & `readme-metrics-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readme-metrics-2.2.3/PKG-INFO` & `readme-metrics-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readme-metrics
-Version: 2.2.3
+Version: 3.0.0
 Summary: ReadMe API Metrics SDK
 Home-page: https://github.com/readmeio/metrics-sdks/tree/main/packages/python
 Author: ReadMe
 Author-email: support@readme.io
 Description-Content-Type: text/markdown
 Provides-Extra: Flask
 Provides-Extra: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: readme-metrics Version: 2.2.3 Summary: ReadMe API
+Metadata-Version: 2.1 Name: readme-metrics Version: 3.0.0 Summary: ReadMe API
 Metrics SDK Home-page: https://github.com/readmeio/metrics-sdks/tree/main/
 packages/python Author: ReadMe Author-email: support@readme.io Description-
 Content-Type: text/markdown Provides-Extra: Flask Provides-Extra: Django
 License-File: LICENSE # ReadMe Metrics
 [https://user-images.githubusercontent.com/33762/182927634-2aebeb46-c215-4ac3-
                             9e98-61f931e33583.png]
             Track usage of your API and troubleshoot issues faster.
```

### Comparing `readme-metrics-2.2.3/README.md` & `readme-metrics-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `readme-metrics-2.2.3/readme_metrics/Metrics.py` & `readme-metrics-3.0.0/readme_metrics/Metrics.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-2.2.3/readme_metrics/MetricsApiConfig.py` & `readme-metrics-3.0.0/readme_metrics/MetricsApiConfig.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-2.2.3/readme_metrics/MetricsMiddleware.py` & `readme-metrics-3.0.0/readme_metrics/MetricsMiddleware.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-2.2.3/readme_metrics/PayloadBuilder.py` & `readme-metrics-3.0.0/readme_metrics/PayloadBuilder.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-2.2.3/readme_metrics/ResponseInfoWrapper.py` & `readme-metrics-3.0.0/readme_metrics/ResponseInfoWrapper.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-2.2.3/readme_metrics/VerifyWebhook.py` & `readme-metrics-3.0.0/readme_metrics/VerifyWebhook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import hmac
 from datetime import datetime, timedelta
 
 
 class VerifyWebhook:
-    def __init__(self, body, signature, secret):
+    def __init__(self, body: dict, signature: str, secret: str):
         if signature is None:
             raise Exception("Missing Signature")
 
         parsed_input = dict(
             (x.strip(), y.strip())
             for x, y in (element.split("=") for element in signature.split(","))
         )
@@ -18,15 +18,15 @@
         if datetime.now() - datetime.fromtimestamp(
             int(parsed_input["t"]) / 1000
         ) > timedelta(minutes=30):
             raise Exception("Expired Signature")
 
         unsigned = time + "." + json.dumps(body, separators=(",", ":"))
         verify_signature = hmac.new(
-            secret,
+            secret.encode("utf-8", errors="ignore"),
             unsigned.encode("utf8"),
             "sha256",
         ).hexdigest()
         readme_signature = parsed_input["v0"]
         if (
             hmac.compare_digest(
                 verify_signature.encode(), readme_signature.encode("utf8")
```

### Comparing `readme-metrics-2.2.3/readme_metrics/django.py` & `readme-metrics-3.0.0/readme_metrics/django.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-2.2.3/readme_metrics/flask_readme.py` & `readme-metrics-3.0.0/readme_metrics/flask_readme.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-2.2.3/readme_metrics/publisher.py` & `readme-metrics-3.0.0/readme_metrics/publisher.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-2.2.3/readme_metrics.egg-info/PKG-INFO` & `readme-metrics-3.0.0/readme_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readme-metrics
-Version: 2.2.3
+Version: 3.0.0
 Summary: ReadMe API Metrics SDK
 Home-page: https://github.com/readmeio/metrics-sdks/tree/main/packages/python
 Author: ReadMe
 Author-email: support@readme.io
 Description-Content-Type: text/markdown
 Provides-Extra: Flask
 Provides-Extra: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: readme-metrics Version: 2.2.3 Summary: ReadMe API
+Metadata-Version: 2.1 Name: readme-metrics Version: 3.0.0 Summary: ReadMe API
 Metrics SDK Home-page: https://github.com/readmeio/metrics-sdks/tree/main/
 packages/python Author: ReadMe Author-email: support@readme.io Description-
 Content-Type: text/markdown Provides-Extra: Flask Provides-Extra: Django
 License-File: LICENSE # ReadMe Metrics
 [https://user-images.githubusercontent.com/33762/182927634-2aebeb46-c215-4ac3-
                             9e98-61f931e33583.png]
             Track usage of your API and troubleshoot issues faster.
```

### Comparing `readme-metrics-2.2.3/readme_metrics.egg-info/SOURCES.txt` & `readme-metrics-3.0.0/readme_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `readme-metrics-2.2.3/setup.py` & `readme-metrics-3.0.0/setup.py`

 * *Files identical despite different names*

