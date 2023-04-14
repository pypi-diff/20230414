# Comparing `tmp/salure_helpers_planday-0.0.1.tar.gz` & `tmp/salure_helpers_planday-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_planday-0.0.1.tar", last modified: Mon Dec 19 16:11:58 2022, max compression
+gzip compressed data, was "dist/salure_helpers_planday-0.0.2.tar", last modified: Fri Apr 14 11:45:18 2023, max compression
```

## Comparing `salure_helpers_planday-0.0.1.tar` & `salure_helpers_planday-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:11:58.000000 salure_helpers_planday-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      265 2022-12-19 16:11:58.000000 salure_helpers_planday-0.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:11:58.000000 salure_helpers_planday-0.0.1/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:11:58.000000 salure_helpers_planday-0.0.1/salure_helpers/planday/
--rw-rw-rw-   0 root         (0) root         (0)       50 2022-12-19 16:11:37.000000 salure_helpers_planday-0.0.1/salure_helpers/planday/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12832 2022-12-19 16:11:37.000000 salure_helpers_planday-0.0.1/salure_helpers/planday/planday.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 16:11:58.000000 salure_helpers_planday-0.0.1/salure_helpers_planday.egg-info/
--rw-r--r--   0 root         (0) root         (0)      265 2022-12-19 16:11:58.000000 salure_helpers_planday-0.0.1/salure_helpers_planday.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2022-12-19 16:11:58.000000 salure_helpers_planday-0.0.1/salure_helpers_planday.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-19 16:11:58.000000 salure_helpers_planday-0.0.1/salure_helpers_planday.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-19 16:11:58.000000 salure_helpers_planday-0.0.1/salure_helpers_planday.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2022-12-19 16:11:58.000000 salure_helpers_planday-0.0.1/salure_helpers_planday.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-12-19 16:11:58.000000 salure_helpers_planday-0.0.1/salure_helpers_planday.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-19 16:11:58.000000 salure_helpers_planday-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      484 2022-12-19 16:11:37.000000 salure_helpers_planday-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers/planday/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-14 11:45:03.000000 salure_helpers_planday-0.0.2/salure_helpers/planday/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12872 2023-04-14 11:45:03.000000 salure_helpers_planday-0.0.2/salure_helpers/planday/planday.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/salure_helpers_planday.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 11:45:18.000000 salure_helpers_planday-0.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-14 11:45:03.000000 salure_helpers_planday-0.0.2/setup.py
```

### Comparing `salure_helpers_planday-0.0.1/salure_helpers/planday/planday.py` & `salure_helpers_planday-0.0.2/salure_helpers/planday/planday.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
         Returns headers for a planday request
         :param access_token: child token for a portal request
         :return: headers
         """
         headers = {
             'X-ClientId': self.client_id,
             'Authorization': f'Bearer {access_token}',
-            'Content-Type': "application/json"
+            'Content-Type': "application/json",
+            'Connection': 'keep-alive'
         }
 
         return headers
 
     def get_portals(self) -> pd.DataFrame:
         """
         This function returns all possible portals (environments) for the access token
```

