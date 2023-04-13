# Comparing `tmp/headscale_api-0.1.1.tar.gz` & `tmp/headscale_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headscale_api-0.1.1.tar", max compression
+gzip compressed data, was "headscale_api-0.1.2.tar", max compression
```

## Comparing `headscale_api-0.1.1.tar` & `headscale_api-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-04-13 22:41:45.194685 headscale_api-0.1.1/LICENSE
--rw-r--r--   0        0        0       68 2023-04-13 22:41:45.194685 headscale_api-0.1.1/README.md
--rw-r--r--   0        0        0      447 2023-04-13 22:41:45.194685 headscale_api-0.1.1/headscale_api/__init__.py
--rw-r--r--   0        0        0      428 2023-04-13 22:41:45.194685 headscale_api-0.1.1/headscale_api/config.py
--rw-r--r--   0        0        0     9775 2023-04-13 22:41:45.194685 headscale_api-0.1.1/headscale_api/endpoints.py
--rw-r--r--   0        0        0     6179 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/headscale.py
--rw-r--r--   0        0        0        0 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/py.typed
--rw-r--r--   0        0        0        0 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/schema/__init__.py
--rw-r--r--   0        0        0     3967 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/schema/config.py
--rw-r--r--   0        0        0        0 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/schema/google/__init__.py
--rw-r--r--   0        0        0    15302 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/schema/google/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/schema/headscale/__init__.py
--rw-r--r--   0        0        0    48167 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/schema/headscale/v1/__init__.py
--rw-r--r--   0        0        0     1684 2023-04-13 22:41:45.198685 headscale_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 headscale_api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-13 22:52:40.095588 headscale_api-0.1.2/LICENSE
+-rw-r--r--   0        0        0       68 2023-04-13 22:52:40.095588 headscale_api-0.1.2/README.md
+-rw-r--r--   0        0        0      447 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/__init__.py
+-rw-r--r--   0        0        0      428 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/config.py
+-rw-r--r--   0        0        0     9775 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/endpoints.py
+-rw-r--r--   0        0        0     6664 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/headscale.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/py.typed
+-rw-r--r--   0        0        0        0 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/schema/__init__.py
+-rw-r--r--   0        0        0     3967 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/schema/config.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/schema/google/__init__.py
+-rw-r--r--   0        0        0    15302 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/schema/google/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/schema/headscale/__init__.py
+-rw-r--r--   0        0        0    48167 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/schema/headscale/v1/__init__.py
+-rw-r--r--   0        0        0     1684 2023-04-13 22:52:40.099588 headscale_api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 headscale_api-0.1.2/PKG-INFO
```

### Comparing `headscale_api-0.1.1/LICENSE` & `headscale_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.1/headscale_api/endpoints.py` & `headscale_api-0.1.2/headscale_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.1/headscale_api/headscale.py` & `headscale_api-0.1.2/headscale_api/headscale.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,31 @@
                 "Accept": "application/json",
                 "Authorization": f"Bearer {new_api_key}",
             },
             timeout=self.timeout,
         )
         return response.status_code == 200
 
+    @property
+    def base_url(self):
+        """Get base URL of the Headscale server."""
+        return self._base_url
+
+    @property
+    def health_url(self) -> str:
+        """Get health check URL of the Headscale server."""
+        return f"{self.base_url}/health"
+
+    async def health_check(self) -> bool:
+        """Perform a health check.
+
+        Returns True if check passed.
+        """
+        return requests.get(self.health_url, timeout=self.timeout).status_code == 200
+
     def _safe_snake_case_recursive(
         self, dictionary: Dict[Any, Any]
     ) -> Generator[Tuple[Any, Any], None, None]:
         assert isinstance(dictionary, dict)
         for key, value in dictionary.items():
             if isinstance(value, dict):
                 yield key, dict(self._safe_snake_case_recursive(value))  # type: ignore
```

### Comparing `headscale_api-0.1.1/headscale_api/schema/config.py` & `headscale_api-0.1.2/headscale_api/schema/config.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.1/headscale_api/schema/google/api/__init__.py` & `headscale_api-0.1.2/headscale_api/schema/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.1/headscale_api/schema/headscale/v1/__init__.py` & `headscale_api-0.1.2/headscale_api/schema/headscale/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.1/pyproject.toml` & `headscale_api-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "headscale-api"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python Headscale API and configuration abstraction."
 authors = ["Marek Pikuła <marek@serenitycode.dev>"]
 maintainers = ["Marek Pikuła <marek@serenitycode.dev>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `headscale_api-0.1.1/PKG-INFO` & `headscale_api-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headscale-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Headscale API and configuration abstraction.
 Home-page: https://github.com/MarekPikula/python-headscale-api
 License: MIT
 Author: Marek Pikuła
 Author-email: marek@serenitycode.dev
 Maintainer: Marek Pikuła
 Maintainer-email: marek@serenitycode.dev
```

