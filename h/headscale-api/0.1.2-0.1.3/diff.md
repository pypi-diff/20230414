# Comparing `tmp/headscale_api-0.1.2.tar.gz` & `tmp/headscale_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headscale_api-0.1.2.tar", max compression
+gzip compressed data, was "headscale_api-0.1.3.tar", max compression
```

## Comparing `headscale_api-0.1.2.tar` & `headscale_api-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-04-13 22:52:40.095588 headscale_api-0.1.2/LICENSE
--rw-r--r--   0        0        0       68 2023-04-13 22:52:40.095588 headscale_api-0.1.2/README.md
--rw-r--r--   0        0        0      447 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/__init__.py
--rw-r--r--   0        0        0      428 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/config.py
--rw-r--r--   0        0        0     9775 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/endpoints.py
--rw-r--r--   0        0        0     6664 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/headscale.py
--rw-r--r--   0        0        0        0 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/py.typed
--rw-r--r--   0        0        0        0 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/schema/__init__.py
--rw-r--r--   0        0        0     3967 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/schema/config.py
--rw-r--r--   0        0        0        0 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/schema/google/__init__.py
--rw-r--r--   0        0        0    15302 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/schema/google/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/schema/headscale/__init__.py
--rw-r--r--   0        0        0    48167 2023-04-13 22:52:40.095588 headscale_api-0.1.2/headscale_api/schema/headscale/v1/__init__.py
--rw-r--r--   0        0        0     1684 2023-04-13 22:52:40.099588 headscale_api-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 headscale_api-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-14 01:20:03.795404 headscale_api-0.1.3/LICENSE
+-rw-r--r--   0        0        0       68 2023-04-14 01:20:03.795404 headscale_api-0.1.3/README.md
+-rw-r--r--   0        0        0      537 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/__init__.py
+-rw-r--r--   0        0        0      428 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/config.py
+-rw-r--r--   0        0        0     9775 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/endpoints.py
+-rw-r--r--   0        0        0     7084 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/headscale.py
+-rw-r--r--   0        0        0        0 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/py.typed
+-rw-r--r--   0        0        0        0 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/schema/__init__.py
+-rw-r--r--   0        0        0     3967 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/schema/config.py
+-rw-r--r--   0        0        0        0 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/schema/google/__init__.py
+-rw-r--r--   0        0        0    15302 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/schema/google/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/schema/headscale/__init__.py
+-rw-r--r--   0        0        0    48177 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/schema/headscale/v1/__init__.py
+-rw-r--r--   0        0        0     1684 2023-04-14 01:20:03.795404 headscale_api-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 headscale_api-0.1.3/PKG-INFO
```

### Comparing `headscale_api-0.1.2/LICENSE` & `headscale_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.2/headscale_api/endpoints.py` & `headscale_api-0.1.3/headscale_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.2/headscale_api/headscale.py` & `headscale_api-0.1.3/headscale_api/headscale.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,24 +108,35 @@
         """Perform a health check.
 
         Returns True if check passed.
         """
         return requests.get(self.health_url, timeout=self.timeout).status_code == 200
 
     def _safe_snake_case_recursive(
-        self, dictionary: Dict[Any, Any]
-    ) -> Generator[Tuple[Any, Any], None, None]:
+        self, dictionary: Dict[str, Any]
+    ) -> Generator[Tuple[str, Any], None, None]:
         assert isinstance(dictionary, dict)
         for key, value in dictionary.items():
+            escaped_key = safe_snake_case(key)
             if isinstance(value, dict):
-                yield key, dict(self._safe_snake_case_recursive(value))  # type: ignore
-            elif isinstance(key, str):
-                yield safe_snake_case(key), value
+                yield (
+                    escaped_key,
+                    dict(self._safe_snake_case_recursive(value)),  # type: ignore
+                )
+            elif isinstance(value, list):
+                yield escaped_key, list(
+                    list_value
+                    if not isinstance(list_value, dict)
+                    else dict(
+                        self._safe_snake_case_recursive(list_value)  # type: ignore
+                    )
+                    for list_value in value  # type: ignore
+                )
             else:
-                yield key, value
+                yield escaped_key, value
 
     async def _unary_unary(  # type: ignore
         self,
         route: str,
         request: Message,
         response_type: Type[MessageT],
         *,
```

### Comparing `headscale_api-0.1.2/headscale_api/schema/config.py` & `headscale_api-0.1.3/headscale_api/schema/config.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.2/headscale_api/schema/google/api/__init__.py` & `headscale_api-0.1.3/headscale_api/schema/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.2/headscale_api/schema/headscale/v1/__init__.py` & `headscale_api-0.1.3/headscale_api/schema/headscale/v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 @dataclass(eq=False, repr=False)
 class ApiKey(betterproto.Message):
     id: int = betterproto.uint64_field(1)
     prefix: str = betterproto.string_field(2)
     expiration: datetime = betterproto.message_field(3)
     created_at: datetime = betterproto.message_field(4)
-    last_seen: datetime = betterproto.message_field(5)
+    last_seen: Optional[datetime] = betterproto.message_field(5)
 
 
 @dataclass(eq=False, repr=False)
 class CreateApiKeyRequest(betterproto.Message):
     expiration: datetime = betterproto.message_field(1)
```

### Comparing `headscale_api-0.1.2/pyproject.toml` & `headscale_api-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "headscale-api"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python Headscale API and configuration abstraction."
 authors = ["Marek Pikuła <marek@serenitycode.dev>"]
 maintainers = ["Marek Pikuła <marek@serenitycode.dev>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `headscale_api-0.1.2/PKG-INFO` & `headscale_api-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headscale-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Headscale API and configuration abstraction.
 Home-page: https://github.com/MarekPikula/python-headscale-api
 License: MIT
 Author: Marek Pikuła
 Author-email: marek@serenitycode.dev
 Maintainer: Marek Pikuła
 Maintainer-email: marek@serenitycode.dev
```

