# Comparing `tmp/unitest-1.4.8.tar.gz` & `tmp/unitest-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitest-1.4.8.tar", last modified: Fri Jul  1 08:19:35 2022, max compression
+gzip compressed data, was "unitest-1.4.9.tar", last modified: Fri Jul 22 09:40:10 2022, max compression
```

## Comparing `unitest-1.4.8.tar` & `unitest-1.4.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 saurabhsharma   (502) staff       (20)        0 2022-07-01 08:19:35.650233 unitest-1.4.8/
--rw-r--r--   0 saurabhsharma   (502) staff       (20)     1073 2022-04-26 09:15:42.000000 unitest-1.4.8/LICENSE
--rw-r--r--   0 saurabhsharma   (502) staff       (20)      562 2022-07-01 08:19:35.649799 unitest-1.4.8/PKG-INFO
--rw-r--r--   0 saurabhsharma   (502) staff       (20)      133 2022-04-26 10:23:09.000000 unitest-1.4.8/README.md
--rw-r--r--   0 saurabhsharma   (502) staff       (20)      103 2022-04-26 09:15:42.000000 unitest-1.4.8/pyproject.toml
--rw-r--r--   0 saurabhsharma   (502) staff       (20)       38 2022-07-01 08:19:35.650359 unitest-1.4.8/setup.cfg
--rw-r--r--   0 saurabhsharma   (502) staff       (20)     1269 2022-07-01 08:17:12.000000 unitest-1.4.8/setup.py
-drwxr-xr-x   0 saurabhsharma   (502) staff       (20)        0 2022-07-01 08:19:35.637005 unitest-1.4.8/src/
-drwxr-xr-x   0 saurabhsharma   (502) staff       (20)        0 2022-07-01 08:19:35.645182 unitest-1.4.8/src/unitest/
--rw-r--r--   0 saurabhsharma   (502) staff       (20)        0 2022-04-26 09:15:42.000000 unitest-1.4.8/src/unitest/__init__.py
--rw-r--r--   0 saurabhsharma   (502) staff       (20)     1546 2022-05-05 07:18:11.000000 unitest-1.4.8/src/unitest/chrome_driver_setup.py
--rw-r--r--   0 saurabhsharma   (502) staff       (20)     1481 2022-04-26 10:23:09.000000 unitest-1.4.8/src/unitest/csv_reader.py
--rw-r--r--   0 saurabhsharma   (502) staff       (20)    11815 2022-06-30 19:48:43.000000 unitest-1.4.8/src/unitest/jsoncompare.py
--rw-r--r--   0 saurabhsharma   (502) staff       (20)    14733 2022-04-26 10:23:09.000000 unitest-1.4.8/src/unitest/listeners.py
--rw-r--r--   0 saurabhsharma   (502) staff       (20)     6434 2022-07-01 08:17:00.000000 unitest-1.4.8/src/unitest/python_adapter.py
--rw-r--r--   0 saurabhsharma   (502) staff       (20)      288 2022-04-26 10:23:09.000000 unitest-1.4.8/src/unitest/uniresponse_utils.py
--rw-r--r--   0 saurabhsharma   (502) staff       (20)     8574 2022-05-05 07:18:11.000000 unitest-1.4.8/src/unitest/utilities.py
-drwxr-xr-x   0 saurabhsharma   (502) staff       (20)        0 2022-07-01 08:19:35.648986 unitest-1.4.8/src/unitest.egg-info/
--rw-r--r--   0 saurabhsharma   (502) staff       (20)      562 2022-07-01 08:19:35.000000 unitest-1.4.8/src/unitest.egg-info/PKG-INFO
--rw-r--r--   0 saurabhsharma   (502) staff       (20)      440 2022-07-01 08:19:35.000000 unitest-1.4.8/src/unitest.egg-info/SOURCES.txt
--rw-r--r--   0 saurabhsharma   (502) staff       (20)        1 2022-07-01 08:19:35.000000 unitest-1.4.8/src/unitest.egg-info/dependency_links.txt
--rw-r--r--   0 saurabhsharma   (502) staff       (20)      335 2022-07-01 08:19:35.000000 unitest-1.4.8/src/unitest.egg-info/requires.txt
--rw-r--r--   0 saurabhsharma   (502) staff       (20)        8 2022-07-01 08:19:35.000000 unitest-1.4.8/src/unitest.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-22 09:40:10.553321 unitest-1.4.9/
+-rw-r--r--   0 root         (0) root         (0)     1073 2022-07-22 09:39:36.000000 unitest-1.4.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      576 2022-07-22 09:40:10.553321 unitest-1.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      147 2022-07-22 09:39:36.000000 unitest-1.4.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      103 2022-07-22 09:39:36.000000 unitest-1.4.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-07-22 09:40:10.553321 unitest-1.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1394 2022-07-22 09:39:36.000000 unitest-1.4.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-22 09:40:10.549321 unitest-1.4.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-22 09:40:10.549321 unitest-1.4.9/src/unitest/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 09:39:36.000000 unitest-1.4.9/src/unitest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2022-07-22 09:39:36.000000 unitest-1.4.9/src/unitest/chrome_driver_setup.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2022-07-22 09:39:36.000000 unitest-1.4.9/src/unitest/csv_reader.py
+-rw-r--r--   0 root         (0) root         (0)    11815 2022-07-22 09:39:36.000000 unitest-1.4.9/src/unitest/jsoncompare.py
+-rw-r--r--   0 root         (0) root         (0)    14733 2022-07-22 09:39:36.000000 unitest-1.4.9/src/unitest/listeners.py
+-rw-r--r--   0 root         (0) root         (0)     7406 2022-07-22 09:39:36.000000 unitest-1.4.9/src/unitest/python_adapter.py
+-rw-r--r--   0 root         (0) root         (0)      288 2022-07-22 09:39:36.000000 unitest-1.4.9/src/unitest/uniresponse_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8574 2022-07-22 09:39:36.000000 unitest-1.4.9/src/unitest/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-22 09:40:10.553321 unitest-1.4.9/src/unitest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      576 2022-07-22 09:40:10.000000 unitest-1.4.9/src/unitest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2022-07-22 09:40:10.000000 unitest-1.4.9/src/unitest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-22 09:40:10.000000 unitest-1.4.9/src/unitest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      335 2022-07-22 09:40:10.000000 unitest-1.4.9/src/unitest.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-07-22 09:40:10.000000 unitest-1.4.9/src/unitest.egg-info/top_level.txt
```

### Comparing `unitest-1.4.8/LICENSE` & `unitest-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unitest-1.4.8/PKG-INFO` & `unitest-1.4.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: unitest
-Version: 1.4.8
+Version: 1.4.9
 Summary: Utilities required for performance and functional tests
 Home-page: https://bitbucket.org/zetaengg/unitest_plutus/src/main/
 Author: Zeta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to unitest
 
 Tech: python 3
-
 This is a package for all common and reusable standard functionalities across testing framework
+version: 1.4.9
```

### Comparing `unitest-1.4.8/setup.py` & `unitest-1.4.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+with open('README.md', "r", encoding="utf-8") as version:
+    version_number = version.readlines()[-1].split(":")[-1]
+
 setuptools.setup(
     name="unitest",
-    version="1.4.8",
+    version=version_number,
     author="Zeta",
     description="Utilities required for performance and functional tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bitbucket.org/zetaengg/unitest_plutus/src/main/",
     classifiers=[
         "Programming Language :: Python :: 3",
@@ -36,9 +39,8 @@
         "webdriver-manager>=3.5.2",
         "greenlet>=1.1.2",
         "faker>=11.3.0",
         "exrex>=0.10.5",
         "decorator",
         "prometheus_client"
     ]
-
 )
```

### Comparing `unitest-1.4.8/src/unitest/chrome_driver_setup.py` & `unitest-1.4.9/src/unitest/chrome_driver_setup.py`

 * *Files identical despite different names*

### Comparing `unitest-1.4.8/src/unitest/csv_reader.py` & `unitest-1.4.9/src/unitest/csv_reader.py`

 * *Files identical despite different names*

### Comparing `unitest-1.4.8/src/unitest/jsoncompare.py` & `unitest-1.4.9/src/unitest/jsoncompare.py`

 * *Files identical despite different names*

### Comparing `unitest-1.4.8/src/unitest/listeners.py` & `unitest-1.4.9/src/unitest/listeners.py`

 * *Files identical despite different names*

### Comparing `unitest-1.4.8/src/unitest/python_adapter.py` & `unitest-1.4.9/src/unitest/python_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 import json
 import os
-import requests
 import time
 
+import requests
 from decorator import decorator
-from prometheus_client import CollectorRegistry, Gauge, push_to_gateway
-
-registry = CollectorRegistry()
-guage = Gauge("flow_probe_status", "Endpoint status", ["probeId", "probeName", "flowId", "flow_name"], registry=registry)
 
 original_request_method = requests.request
 PRETTY_OUTPUT = True
 
 os.environ["ENABLE_REQUEST_ADAPTER"] = "False"
 os.environ["SKIP_ADAPTER"] = "False"
 
 header = {"Content-Type": "application/json"}
 
+env = os.environ.get("ENV", "beta")
+
+
+def get_probe_runner_host():
+    if env.lower() == 'stage':
+        return "https://proberunner.internal.mum1-stage.zetaapps.in"
+    if env.lower() == 'pre-prod':
+        return "https://proberunner.internal.mum1-pp.zetaapps.in"
+    if env.lower() == 'beta':
+        return "https://proberunner.internal.hdfc-beta.zetaapps.in"
+    else:
+        raise ValueError("Incorrect argument passed as env : " + env)
+
 
 def trace():
     os.environ["SKIP_ADAPTER"] = "True"
     headers = dict()
-    probe_url = f'https://proberunner.internal.mum1-stage.zetaapps.in/trace/headers'
+    probe_url = get_probe_runner_host() + "/trace/headers"
     response = requests.get(url=probe_url, headers=header)
     os.environ["SKIP_ADAPTER"] = "False"
     try:
         headers = response.json()['traceHeaders']
     except:
         return headers
     return headers
@@ -124,59 +133,82 @@
                 "statusCode": status_code,
                 "status": flag
             }]
 
             probe_id = get_probe(flow_probe_name, flow_id)
 
             if probe_id != "":
-                push_to_probe(probe_id, probe_data)
+                save_probe_invocation(probe_id, probe_data)
             else:
                 probe_id = create_probe(create_probe_body)
-                push_to_probe(probe_id, probe_data)
+                save_probe_invocation(probe_id, probe_data)
 
             flow_probe_name_with_id = f"{flow_probe_name}_{probe_id}"
 
-            guage.labels(probe_id, flow_probe_name_with_id, flow_id, flow_id).set(flag)
-            push_to_gateway("https://pushgateway.internal.mum1-stage.zetaapps.in/", job="PROBE-METRICS", registry=registry)
+            prometheus_push_body = {
+                "metricName": "flow_probe_status",
+                "metricDescription": "Endpoint status",
+                "metricLabels": {
+                    "probeName": flow_probe_name_with_id,
+                    "probeId": probe_id,
+                    "flowId": flow_id,
+                    "flowName": flow_id
+                },
+                "metricValue": flag
+            }
+
+            push_to_prometheus(prometheus_push_body)
 
 
 def get_probe(flow_probe_name, flow_id):
     os.environ["SKIP_ADAPTER"] = "True"
-    url = f"https://proberunner.internal.mum1-stage.zetaapps.in/probe/{flow_probe_name}/flow/{flow_id}"
-    response = requests.get(url, headers=header)
+    get_probe_url = get_probe_runner_host() + f"/probe/{flow_probe_name}/flow/{flow_id}"
+    response = requests.get(get_probe_url, headers=header)
     os.environ["SKIP_ADAPTER"] = "False"
     if response.text:
         return response.json()["probeId"]
     else:
         return ""
 
 
-def push_to_probe(probe_id, probe_data):
+def save_probe_invocation(probe_id, probe_data):
     os.environ["SKIP_ADAPTER"] = "True"
-    url = f"https://proberunner.internal.mum1-stage.zetaapps.in/probe/{probe_id}/invocations"
+    save_probe_invocation_url = get_probe_runner_host() + f"/probe/{probe_id}/invocations"
     data = json.dumps(probe_data)
-    response = requests.post(url, data=data, headers=header)
+    response = requests.post(save_probe_invocation_url, data=data, headers=header)
     if response.status_code != 200:
         return response.text
     os.environ["SKIP_ADAPTER"] = "False"
     if response.text == "1 invocations saved":
         return True
     else:
         if response.json()["message"] == "failure to get a peer from the ring-balancer":
             return True
 
 
 def create_probe(create_probe_body):
     os.environ["SKIP_ADAPTER"] = "True"
-    url = "https://proberunner.internal.mum1-stage.zetaapps.in/probe"
+    create_probe_url = get_probe_runner_host() + "/probe"
     data = json.dumps(create_probe_body)
-    response = requests.post(url, data=data, headers=header)
+    response = requests.post(create_probe_url, data=data, headers=header)
     os.environ["SKIP_ADAPTER"] = "False"
     if response.status_code == 200:
         return response.json()["probeId"]
     else:
         raise TypeError("Could not create a probe.")
 
 
+def push_to_prometheus(prometheus_push_body):
+    os.environ["SKIP_ADAPTER"] = "True"
+    push_to_prometheus_url = get_probe_runner_host() + "/prometheus/push?jobName=PROBE-METRICS"
+    data = json.dumps(prometheus_push_body)
+    response = requests.post(push_to_prometheus_url, data=data, headers=header)
+    os.environ["SKIP_ADAPTER"] = "False"
+    if response.status_code == 200:
+        return
+    else:
+        raise TypeError("Could not push data to prometheus.")
+
+
 def patcher():
     requests.api.request = logged_request
     requests.request = logged_request
```

### Comparing `unitest-1.4.8/src/unitest/utilities.py` & `unitest-1.4.9/src/unitest/utilities.py`

 * *Files identical despite different names*

### Comparing `unitest-1.4.8/src/unitest.egg-info/PKG-INFO` & `unitest-1.4.9/src/unitest.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: unitest
-Version: 1.4.8
+Version: 1.4.9
 Summary: Utilities required for performance and functional tests
 Home-page: https://bitbucket.org/zetaengg/unitest_plutus/src/main/
 Author: Zeta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to unitest
 
 Tech: python 3
-
 This is a package for all common and reusable standard functionalities across testing framework
+version: 1.4.9
```

