# Comparing `tmp/better-translation-0.3.1.tar.gz` & `tmp/better-translation-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better-translation-0.3.1.tar", last modified: Sun Apr  9 21:32:18 2023, max compression
+gzip compressed data, was "better-translation-0.3.2.tar", last modified: Fri Apr 14 17:50:04 2023, max compression
```

## Comparing `better-translation-0.3.1.tar` & `better-translation-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:18.286028 better-translation-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-09 21:32:18.286028 better-translation-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-09 21:32:15.000000 better-translation-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:18.282028 better-translation-0.3.1/better_translation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:18.282028 better-translation-0.3.1/better_translation/_babel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/_babel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/_babel/lazy_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:18.282028 better-translation-0.3.1/better_translation/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:18.286028 better-translation-0.3.1/better_translation/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/integrations/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/integrations/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/integrations/django/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-09 21:32:15.000000 better-translation-0.3.1/better_translation/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:32:18.282028 better-translation-0.3.1/better_translation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-09 21:32:18.000000 better-translation-0.3.1/better_translation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-09 21:32:18.000000 better-translation-0.3.1/better_translation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 21:32:18.000000 better-translation-0.3.1/better_translation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-09 21:32:18.000000 better-translation-0.3.1/better_translation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-09 21:32:15.000000 better-translation-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 21:32:18.286028 better-translation-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-09 21:32:17.000000 better-translation-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:04.147652 better-translation-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 17:50:04.147652 better-translation-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-14 17:50:01.000000 better-translation-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:04.147652 better-translation-0.3.2/better_translation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:04.147652 better-translation-0.3.2/better_translation/_babel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/_babel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/_babel/lazy_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:04.147652 better-translation-0.3.2/better_translation/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:04.147652 better-translation-0.3.2/better_translation/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/integrations/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/integrations/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/integrations/django/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-14 17:50:01.000000 better-translation-0.3.2/better_translation/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:50:04.147652 better-translation-0.3.2/better_translation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 17:50:04.000000 better-translation-0.3.2/better_translation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-14 17:50:04.000000 better-translation-0.3.2/better_translation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:50:04.000000 better-translation-0.3.2/better_translation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 17:50:04.000000 better-translation-0.3.2/better_translation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-14 17:50:01.000000 better-translation-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:50:04.147652 better-translation-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-14 17:50:03.000000 better-translation-0.3.2/setup.py
```

### Comparing `better-translation-0.3.1/better_translation/_babel/lazy_proxy.py` & `better-translation-0.3.2/better_translation/_babel/lazy_proxy.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.1/better_translation/extractor.py` & `better-translation-0.3.2/better_translation/extractor.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.1/better_translation/integrations/django/admin.py` & `better-translation-0.3.2/better_translation/integrations/django/admin.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.1/better_translation/integrations/django/models.py` & `better-translation-0.3.2/better_translation/integrations/django/models.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.1/better_translation/integrations/django/storage.py` & `better-translation-0.3.2/better_translation/integrations/django/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,15 @@
                 logger.debug(
                     "Message '%s' is already in the storage",
                     message,
                 )
                 continue
 
             logger.info("Adding message '%s' to the storage", message)
+            self.storage[message.id] = message
             messages_to_create.add(self._get_message_model(message))
 
         await self.message_model.objects.abulk_create(messages_to_create)
 
     async def add_messages_from_dirs(self, *dirs: Path) -> None:
         messages: list[StorageMessage] = []
         for directory_path in dirs:
```

### Comparing `better-translation-0.3.1/better_translation/provider.py` & `better-translation-0.3.2/better_translation/provider.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.1/better_translation/storage.py` & `better-translation-0.3.2/better_translation/storage.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.1/better_translation/translator.py` & `better-translation-0.3.2/better_translation/translator.py`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.1/better_translation.egg-info/SOURCES.txt` & `better-translation-0.3.2/better_translation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.1/pyproject.toml` & `better-translation-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `better-translation-0.3.1/setup.py` & `better-translation-0.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 _version = (
-    "0.3.1"  # Version will be replaced by the CD pipeline
+    "0.3.2"  # Version will be replaced by the CD pipeline
 )
 VERSION = "0.0.0" if _version.startswith("{{") else _version
 
 
 def get_readme() -> str:
     readme = Path("README.md")
     return readme.read_text(encoding="utf-8")
```

