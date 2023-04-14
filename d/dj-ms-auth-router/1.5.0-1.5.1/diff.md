# Comparing `tmp/dj-ms-auth-router-1.5.0.tar.gz` & `tmp/dj-ms-auth-router-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-ms-auth-router-1.5.0.tar", last modified: Thu Apr  6 13:02:14 2023, max compression
+gzip compressed data, was "dj-ms-auth-router-1.5.1.tar", last modified: Fri Apr 14 07:38:10 2023, max compression
```

## Comparing `dj-ms-auth-router-1.5.0.tar` & `dj-ms-auth-router-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-06 13:02:14.359276 dj-ms-auth-router-1.5.0/
--rw-r--r--   0 rustam     (501) staff       (20)     1545 2022-11-28 11:45:05.000000 dj-ms-auth-router-1.5.0/LICENSE
--rw-r--r--   0 rustam     (501) staff       (20)       58 2022-11-28 11:45:05.000000 dj-ms-auth-router-1.5.0/MANIFEST.in
--rw-r--r--   0 rustam     (501) staff       (20)     3324 2023-04-06 13:02:14.359366 dj-ms-auth-router-1.5.0/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)     2136 2023-03-01 06:26:54.000000 dj-ms-auth-router-1.5.0/README.md
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-06 13:02:14.356034 dj-ms-auth-router-1.5.0/dj_ms_auth_router.egg-info/
--rw-r--r--   0 rustam     (501) staff       (20)     3324 2023-04-06 13:02:14.000000 dj-ms-auth-router-1.5.0/dj_ms_auth_router.egg-info/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)      350 2023-04-06 13:02:14.000000 dj-ms-auth-router-1.5.0/dj_ms_auth_router.egg-info/SOURCES.txt
--rw-r--r--   0 rustam     (501) staff       (20)        1 2023-04-06 13:02:14.000000 dj-ms-auth-router-1.5.0/dj_ms_auth_router.egg-info/dependency_links.txt
--rw-r--r--   0 rustam     (501) staff       (20)       12 2023-04-06 13:02:14.000000 dj-ms-auth-router-1.5.0/dj_ms_auth_router.egg-info/requires.txt
--rw-r--r--   0 rustam     (501) staff       (20)       15 2023-04-06 13:02:14.000000 dj-ms-auth-router-1.5.0/dj_ms_auth_router.egg-info/top_level.txt
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-06 13:02:14.353082 dj-ms-auth-router-1.5.0/docs/
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-06 13:02:14.356298 dj-ms-auth-router-1.5.0/docs/media/
--rw-r--r--   0 rustam     (501) staff       (20)   232442 2023-02-04 13:33:44.000000 dj-ms-auth-router-1.5.0/docs/media/scheme.png
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-06 13:02:14.358888 dj-ms-auth-router-1.5.0/ms_auth_router/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2023-02-01 11:09:19.000000 dj-ms-auth-router-1.5.0/ms_auth_router/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)     1765 2023-03-01 04:55:08.000000 dj-ms-auth-router-1.5.0/ms_auth_router/apps.py
--rw-r--r--   0 rustam     (501) staff       (20)     2214 2023-03-01 05:36:54.000000 dj-ms-auth-router-1.5.0/ms_auth_router/routers.py
--rw-r--r--   0 rustam     (501) staff       (20)     1114 2023-04-06 13:02:14.359772 dj-ms-auth-router-1.5.0/setup.cfg
--rw-r--r--   0 rustam     (501) staff       (20)      242 2023-02-01 11:08:10.000000 dj-ms-auth-router-1.5.0/setup.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-14 07:38:10.659401 dj-ms-auth-router-1.5.1/
+-rw-r--r--   0 rustam     (501) staff       (20)     1545 2022-11-28 11:45:05.000000 dj-ms-auth-router-1.5.1/LICENSE
+-rw-r--r--   0 rustam     (501) staff       (20)       58 2022-11-28 11:45:05.000000 dj-ms-auth-router-1.5.1/MANIFEST.in
+-rw-r--r--   0 rustam     (501) staff       (20)     3324 2023-04-14 07:38:10.659515 dj-ms-auth-router-1.5.1/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)     2136 2023-03-01 06:26:54.000000 dj-ms-auth-router-1.5.1/README.md
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-14 07:38:10.655809 dj-ms-auth-router-1.5.1/dj_ms_auth_router.egg-info/
+-rw-r--r--   0 rustam     (501) staff       (20)     3324 2023-04-14 07:38:10.000000 dj-ms-auth-router-1.5.1/dj_ms_auth_router.egg-info/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)      350 2023-04-14 07:38:10.000000 dj-ms-auth-router-1.5.1/dj_ms_auth_router.egg-info/SOURCES.txt
+-rw-r--r--   0 rustam     (501) staff       (20)        1 2023-04-14 07:38:10.000000 dj-ms-auth-router-1.5.1/dj_ms_auth_router.egg-info/dependency_links.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       12 2023-04-14 07:38:10.000000 dj-ms-auth-router-1.5.1/dj_ms_auth_router.egg-info/requires.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       15 2023-04-14 07:38:10.000000 dj-ms-auth-router-1.5.1/dj_ms_auth_router.egg-info/top_level.txt
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-14 07:38:10.652358 dj-ms-auth-router-1.5.1/docs/
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-14 07:38:10.656093 dj-ms-auth-router-1.5.1/docs/media/
+-rw-r--r--   0 rustam     (501) staff       (20)   232442 2023-02-04 13:33:44.000000 dj-ms-auth-router-1.5.1/docs/media/scheme.png
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-14 07:38:10.658915 dj-ms-auth-router-1.5.1/ms_auth_router/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2023-02-01 11:09:19.000000 dj-ms-auth-router-1.5.1/ms_auth_router/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1903 2023-04-14 07:37:56.000000 dj-ms-auth-router-1.5.1/ms_auth_router/apps.py
+-rw-r--r--   0 rustam     (501) staff       (20)     2214 2023-03-01 05:36:54.000000 dj-ms-auth-router-1.5.1/ms_auth_router/routers.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1114 2023-04-14 07:38:10.660033 dj-ms-auth-router-1.5.1/setup.cfg
+-rw-r--r--   0 rustam     (501) staff       (20)      242 2023-02-01 11:08:10.000000 dj-ms-auth-router-1.5.1/setup.py
```

### Comparing `dj-ms-auth-router-1.5.0/LICENSE` & `dj-ms-auth-router-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-ms-auth-router-1.5.0/PKG-INFO` & `dj-ms-auth-router-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-ms-auth-router
-Version: 1.5.0
+Version: 1.5.1
 Summary: Simple database router that helps to implement microservices architecture with Django.
 Home-page: https://github.com/dj-ms/dj-ms-auth-router
 Author: Astafeev Rustam
 Author-email: astafeev0308@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj-ms-auth-router-1.5.0/README.md` & `dj-ms-auth-router-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dj-ms-auth-router-1.5.0/dj_ms_auth_router.egg-info/PKG-INFO` & `dj-ms-auth-router-1.5.1/dj_ms_auth_router.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-ms-auth-router
-Version: 1.5.0
+Version: 1.5.1
 Summary: Simple database router that helps to implement microservices architecture with Django.
 Home-page: https://github.com/dj-ms/dj-ms-auth-router
 Author: Astafeev Rustam
 Author-email: astafeev0308@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj-ms-auth-router-1.5.0/docs/media/scheme.png` & `dj-ms-auth-router-1.5.1/docs/media/scheme.png`

 * *Files identical despite different names*

### Comparing `dj-ms-auth-router-1.5.0/ms_auth_router/apps.py` & `dj-ms-auth-router-1.5.1/ms_auth_router/apps.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,54 @@
+import threading
+
 from django.apps import AppConfig
 
 
 class MsAuthRouterConfig(AppConfig):
-
     name = 'ms_auth_router'
 
     def ready(self):
         from django.apps import apps
         from .routers import route_app_labels
         all_apps = apps.get_app_configs()
         apps_for_route = list(app.name.split('.')[-1] for app in all_apps
                               if app.name.split('.')[-1] not in route_app_labels)
 
         def get_all_models():
             for app in apps_for_route:
                 yield from apps.get_app_config(app).get_models()
 
         models = get_all_models()
+        for model in models:
+            PermissionUpdate(model).start()
+
+
+class PermissionUpdate(threading.Thread):
+    def __init__(self, model):
+        super().__init__()
+        self.model = model
+
+    def run(self):
         import logging
         from django.contrib.contenttypes.models import ContentType
         from django.contrib.auth.models import Permission
-        for model in models:
-            try:
-                content_type = ContentType.objects.get_for_model(model)
-            except Exception as e:
-                logging.error(f'Error while loading model {model}: {e}')
-                continue
-            else:
-                meta = model._meta
-                default_permissions = meta.default_permissions
-                for permission in default_permissions:
-                    Permission.objects.get_or_create(
-                        codename=f'{permission}_{content_type.model}',
-                        content_type=content_type,
-                        defaults={'name': f'Can {permission} {content_type.name}'}
-                    )
-                extra_permissions = meta.permissions
-                for permission in extra_permissions:
-                    Permission.objects.get_or_create(
-                        codename=permission[0],
-                        content_type=content_type,
-                        defaults={'name': permission[1]}
-                    )
+        try:
+            content_type = ContentType.objects.get_for_model(self.model)
+        except Exception as e:
+            logging.debug(f'ms_auth_router: cannot load model {self.model.__name__}: {e}.')
+        else:
+            meta = self.model._meta
+            default_permissions = meta.default_permissions
+            for permission in default_permissions:
+                Permission.objects.get_or_create(
+                    codename=f'{permission}_{content_type.model}',
+                    content_type=content_type,
+                    defaults={'name': f'Can {permission} {content_type.name}'}
+                )
+            extra_permissions = meta.permissions
+            for permission in extra_permissions:
+                Permission.objects.get_or_create(
+                    codename=permission[0],
+                    content_type=content_type,
+                    defaults={'name': permission[1]}
+                )
```

### Comparing `dj-ms-auth-router-1.5.0/ms_auth_router/routers.py` & `dj-ms-auth-router-1.5.1/ms_auth_router/routers.py`

 * *Files identical despite different names*

### Comparing `dj-ms-auth-router-1.5.0/setup.cfg` & `dj-ms-auth-router-1.5.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-ms-auth-router
-version = 1.5.0
+version = 1.5.1
 description = Simple database router that helps to implement microservices architecture with Django.
 long_description = file: README.md
 url = https://github.com/dj-ms/dj-ms-auth-router
 author = Astafeev Rustam
 author_email = astafeev0308@gmail.com
 license = BSD-3-Clause
 classifiers =
```

