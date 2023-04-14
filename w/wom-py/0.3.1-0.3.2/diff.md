# Comparing `tmp/wom_py-0.3.1.tar.gz` & `tmp/wom_py-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wom_py-0.3.1.tar", max compression
+gzip compressed data, was "wom_py-0.3.2.tar", max compression
```

## Comparing `wom_py-0.3.1.tar` & `wom_py-0.3.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1074 2023-04-13 00:11:49.609447 wom_py-0.3.1/LICENSE
--rw-r--r--   0        0        0     1942 2023-04-13 00:11:49.609447 wom_py-0.3.1/README.md
--rw-r--r--   0        0        0     2138 2023-04-13 00:11:49.609447 wom_py-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4295 2023-04-13 00:11:49.693447 wom_py-0.3.1/wom/__init__.py
--rw-r--r--   0        0        0     1324 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/__main__.py
--rw-r--r--   0        0        0     1808 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/_cli.py
--rw-r--r--   0        0        0     7795 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/client.py
--rw-r--r--   0        0        0     1447 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/constants.py
--rw-r--r--   0        0        0     7212 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/enums.py
--rw-r--r--   0        0        0     1729 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/errors.py
--rw-r--r--   0        0        0     3138 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/__init__.py
--rw-r--r--   0        0        0     1555 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/base.py
--rw-r--r--   0        0        0     1673 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/competitions/__init__.py
--rw-r--r--   0        0        0     1591 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/competitions/enums.py
--rw-r--r--   0        0        0     7364 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/competitions/models.py
--rw-r--r--   0        0        0     1289 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/deltas/__init__.py
--rw-r--r--   0        0        0     1824 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/deltas/models.py
--rw-r--r--   0        0        0     1716 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/groups/__init__.py
--rw-r--r--   0        0        0     7780 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/groups/enums.py
--rw-r--r--   0        0        0     9075 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/groups/models.py
--rw-r--r--   0        0        0     1738 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/http.py
--rw-r--r--   0        0        0     1381 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/names/__init__.py
--rw-r--r--   0        0        0     1413 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/names/enums.py
--rw-r--r--   0        0        0     3778 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/names/models.py
--rw-r--r--   0        0        0     1754 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/players/__init__.py
--rw-r--r--   0        0        0     5664 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/players/enums.py
--rw-r--r--   0        0        0    11832 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/players/models.py
--rw-r--r--   0        0        0     1300 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/records/__init__.py
--rw-r--r--   0        0        0     2217 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/models/records/models.py
--rw-r--r--   0        0        0        0 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/py.typed
--rw-r--r--   0        0        0     5509 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/result.py
--rw-r--r--   0        0        0     6420 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/routes.py
--rw-r--r--   0        0        0    33973 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/serializer.py
--rw-r--r--   0        0        0     1709 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/__init__.py
--rw-r--r--   0        0        0     2042 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/base.py
--rw-r--r--   0        0        0    20760 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/competitions.py
--rw-r--r--   0        0        0     3477 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/deltas.py
--rw-r--r--   0        0        0     3637 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/efficiency.py
--rw-r--r--   0        0        0    23384 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/groups.py
--rw-r--r--   0        0        0     5355 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/http.py
--rw-r--r--   0        0        0     4722 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/names.py
--rw-r--r--   0        0        0    17519 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/players.py
--rw-r--r--   0        0        0     3455 2023-04-13 00:11:49.613447 wom_py-0.3.1/wom/services/records.py
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 wom_py-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-14 20:14:27.072223 wom_py-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1942 2023-04-14 20:14:27.072223 wom_py-0.3.2/README.md
+-rw-r--r--   0        0        0     2138 2023-04-14 20:14:27.076223 wom_py-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4295 2023-04-14 20:14:27.184223 wom_py-0.3.2/wom/__init__.py
+-rw-r--r--   0        0        0     1324 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/__main__.py
+-rw-r--r--   0        0        0     1808 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/_cli.py
+-rw-r--r--   0        0        0     8494 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/client.py
+-rw-r--r--   0        0        0     1447 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/constants.py
+-rw-r--r--   0        0        0     7212 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/enums.py
+-rw-r--r--   0        0        0     1729 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/errors.py
+-rw-r--r--   0        0        0     3138 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/__init__.py
+-rw-r--r--   0        0        0     1555 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/base.py
+-rw-r--r--   0        0        0     1673 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/competitions/__init__.py
+-rw-r--r--   0        0        0     1591 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/competitions/enums.py
+-rw-r--r--   0        0        0     7364 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/competitions/models.py
+-rw-r--r--   0        0        0     1289 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/deltas/__init__.py
+-rw-r--r--   0        0        0     1824 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/deltas/models.py
+-rw-r--r--   0        0        0     1716 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/groups/__init__.py
+-rw-r--r--   0        0        0     7780 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/groups/enums.py
+-rw-r--r--   0        0        0     9075 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/groups/models.py
+-rw-r--r--   0        0        0     1738 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/http.py
+-rw-r--r--   0        0        0     1381 2023-04-14 20:14:27.076223 wom_py-0.3.2/wom/models/names/__init__.py
+-rw-r--r--   0        0        0     1413 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/names/enums.py
+-rw-r--r--   0        0        0     3778 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/names/models.py
+-rw-r--r--   0        0        0     1754 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/players/__init__.py
+-rw-r--r--   0        0        0     5664 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/players/enums.py
+-rw-r--r--   0        0        0    11832 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/players/models.py
+-rw-r--r--   0        0        0     1300 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/records/__init__.py
+-rw-r--r--   0        0        0     2217 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/models/records/models.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/py.typed
+-rw-r--r--   0        0        0     5561 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/result.py
+-rw-r--r--   0        0        0     6420 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/routes.py
+-rw-r--r--   0        0        0    33973 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/serializer.py
+-rw-r--r--   0        0        0     1709 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/__init__.py
+-rw-r--r--   0        0        0     2042 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/base.py
+-rw-r--r--   0        0        0    21066 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/competitions.py
+-rw-r--r--   0        0        0     3511 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/deltas.py
+-rw-r--r--   0        0        0     3671 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/efficiency.py
+-rw-r--r--   0        0        0    23928 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/groups.py
+-rw-r--r--   0        0        0     5750 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/http.py
+-rw-r--r--   0        0        0     4824 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/names.py
+-rw-r--r--   0        0        0    17995 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/players.py
+-rw-r--r--   0        0        0     3489 2023-04-14 20:14:27.080223 wom_py-0.3.2/wom/services/records.py
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 wom_py-0.3.2/PKG-INFO
```

### Comparing `wom_py-0.3.1/LICENSE` & `wom_py-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/README.md` & `wom_py-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/pyproject.toml` & `wom_py-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wom.py"
-version = "0.3.1"
+version = "0.3.2"
 description = "An asynchronous wrapper for the Wise Old Man API."
 authors = ["Jonxslays"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/wom.py"
 repository = "https://github.com/Jonxslays/wom.py"
 documentation = "https://jonxslays.github.io/wom.py"
```

### Comparing `wom_py-0.3.1/wom/__init__.py` & `wom_py-0.3.2/wom/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,23 +130,23 @@
     "Team",
     "Top5ProgressResult",
     "UnwrapError",
     "WomError",
 )
 
 __packagename__: Final[str] = "wom.py"
-__version__: Final[str] = "0.3.1"
+__version__: Final[str] = "0.3.2"
 __author__: Final[str] = "Jonxslays"
 __copyright__: Final[str] = "2023-present Jonxslays"
 __description__: Final[str] = "An asynchronous wrapper for the Wise Old Man API."
 __url__: Final[str] = "https://github.com/Jonxslays/wom.py"
 __docs__: Final[str] = "https://jonxslays.github.io/wom.py"
 __repository__: Final[str] = __url__
 __license__: Final[str] = "MIT"
-__git_sha__: Final[str] = "[8864456]"
+__git_sha__: Final[str] = "[d9d3e5e]"
 
 from . import client
 from . import constants
 from . import enums
 from . import errors
 from . import models
 from . import result
```

### Comparing `wom_py-0.3.1/wom/__main__.py` & `wom_py-0.3.2/wom/__main__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/_cli.py` & `wom_py-0.3.2/wom/_cli.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/client.py` & `wom_py-0.3.2/wom/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 !!! example
 
     ```py
     from wom import Client
 
     client = Client(user_agent="@your_discord_handle#1234")
 
+    await client.start()
+
     result = await client.players.search_players("Jonxslays", limit=1)
 
     if result.is_ok:
         print(result.unwrap())
     else:
         print(f"ERROR: {result.unwrap_err()}")
 
@@ -83,14 +85,16 @@
 
         client = wom.Client(
             environ["WOM_API_KEY"],
             user_agent="@me#1234",
             api_base_url=environ["LOCAL_WOM_DOMAIN"],
         )
 
+        await client.start()  # Start the client
+
         # ... Use the client
 
         await client.close()  # Close the client
         ```
     """
 
     __slots__ = (
@@ -245,31 +249,59 @@
             client = wom.Client(...)
 
             client.set_api_base_url("https://api.wiseoldman.net/v2")
             ```
         """
         self._http.set_base_url(base_url)
 
+    async def start(self) -> None:
+        """Starts the client session to be used for http requests.
+
+        !!! warning
+
+            If this is not called before you use any of the services,
+            your program will crash with a `RuntimeError`.
+
+        !!! note
+
+            Don't forget to close the client!
+
+        ??? example
+
+            ```py
+            import wom
+
+            client = wom.Client(...)
+
+            await client.start()
+            ```
+        """
+        await self._http.start()
+
     async def close(self) -> None:
         """Closes the existing client session, if it's still open.
 
         !!! tip
 
             Only call this once, at the end of your program or if you are done
             with the client completely.
 
+            This method will do nothing if the Client was never started.
+
         !!! warning
 
             If this is not called before your program terminates, you will
             receive an error in your console.
 
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.close()
             ```
         """
         await self._http.close()
```

### Comparing `wom_py-0.3.1/wom/constants.py` & `wom_py-0.3.2/wom/constants.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/enums.py` & `wom_py-0.3.2/wom/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/errors.py` & `wom_py-0.3.2/wom/errors.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/__init__.py` & `wom_py-0.3.2/wom/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/base.py` & `wom_py-0.3.2/wom/models/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/competitions/__init__.py` & `wom_py-0.3.2/wom/models/competitions/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/competitions/enums.py` & `wom_py-0.3.2/wom/models/competitions/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/competitions/models.py` & `wom_py-0.3.2/wom/models/competitions/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/deltas/__init__.py` & `wom_py-0.3.2/wom/models/deltas/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/deltas/models.py` & `wom_py-0.3.2/wom/models/deltas/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/groups/__init__.py` & `wom_py-0.3.2/wom/models/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/groups/enums.py` & `wom_py-0.3.2/wom/models/groups/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/groups/models.py` & `wom_py-0.3.2/wom/models/groups/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/http.py` & `wom_py-0.3.2/wom/models/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/names/__init__.py` & `wom_py-0.3.2/wom/models/names/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/names/enums.py` & `wom_py-0.3.2/wom/models/names/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/names/models.py` & `wom_py-0.3.2/wom/models/names/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/players/__init__.py` & `wom_py-0.3.2/wom/models/players/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/players/enums.py` & `wom_py-0.3.2/wom/models/players/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/players/models.py` & `wom_py-0.3.2/wom/models/players/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/records/__init__.py` & `wom_py-0.3.2/wom/models/records/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/models/records/models.py` & `wom_py-0.3.2/wom/models/records/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/result.py` & `wom_py-0.3.2/wom/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,27 +23,31 @@
 all [`Client`][wom.Client] calls.
 
 !!! success "Correct usage"
 
     ```py
     client = wom.Client()
 
+    await client.start()
+
     result = await client.players.update_player("Jonxslays")
 
     if result.is_ok:
         print(result.unwrap())
     else:
         print(result.unwrap_err())
     ```
 
 !!! failure "Incorrect usage"
 
     ```py
     client = wom.Client()
 
+    await client.start()
+
     result = await client.players.update_player("eeeeeeeeeeeee")
 
     print(result.unwrap()) # <-- Exception raised
     # Raises UnwrapError because the username was too long
     ```
 """
```

### Comparing `wom_py-0.3.1/wom/routes.py` & `wom_py-0.3.2/wom/routes.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/serializer.py` & `wom_py-0.3.2/wom/serializer.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/services/__init__.py` & `wom_py-0.3.2/wom/services/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/services/base.py` & `wom_py-0.3.2/wom/services/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.3.1/wom/services/competitions.py` & `wom_py-0.3.2/wom/services/competitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.competitions.search_competitions(
                 title="Sick Competition",
                 type=wom.CompetitionType.Classic,
                 status=wom.CompetitionStatus.Ongoing,
                 limit=3,
                 offset=1
             )
@@ -129,14 +131,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.competitions.get_details(123)
 
             result2 = await client.competitions.get_details(
                 123, wom.Skills.Attack
             )
             ```
         """
@@ -345,14 +349,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.competitions.edit_competition(
                 123, "111-111-111", title="New title"
             )
             ```
         """
         payload = self._generate_map(
             title=title,
@@ -394,14 +400,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.competitions.delete_competition(
                 123, "111-111-111"
             )
             ```
         """
         payload = self._generate_map(verificationCode=verification_code)
         route = routes.DELETE_COMPETITION.compile(id)
@@ -421,14 +429,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.competitions.add_participants(
                 123, "111-111-111", "Jonxslays", "Zezima"
             )
             ```
 
         Args:
             id: The ID of the competition.
@@ -460,14 +470,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.competitions.remove_participants(
                 123, "111-111-111", "Jonxslays"
             )
             ```
 
         Args:
             id: The ID of the competition.
@@ -498,14 +510,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.competitions.add_teams(
                 123,
                 "111-111-111",
                 wom.Team("Team 1", ["Jonxslays", "Zezima"]),
                 wom.Team("Team 2", ["lilyuffie88", "the old nite"]),
             )
             ```
@@ -542,14 +556,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.competitions.remove_teams(
                 123, "111-111-111", "Team 1", "Team 2"
             )
             ```
 
         Args:
             id: The ID of the competition.
@@ -602,14 +618,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.competitions.update_outdated_participants(
                 123, "111-111-111"
             )
             ```
 
         Args:
             id: The ID of the competition.
```

### Comparing `wom_py-0.3.1/wom/services/deltas.py` & `wom_py-0.3.2/wom/services/deltas.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.deltas.get_global_leaderboards(
                 wom.Skills.Attack,
                 wom.Period.Day,
                 country=wom.Country.Gb,
             )
             ```
         """
```

### Comparing `wom_py-0.3.1/wom/services/efficiency.py` & `wom_py-0.3.2/wom/services/efficiency.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.efficiency.get_global_leaderboard(
                 player_type=wom.PlayerType.Ironman,
             )
             ```
         """
         params = self._generate_map(
             metric=metric.value if not both else "+".join(m.value for m in enums.ComputedMetrics),
```

### Comparing `wom_py-0.3.1/wom/services/groups.py` & `wom_py-0.3.2/wom/services/groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.search_groups("Some group", limit=3)
             ```
         """
         params = self._generate_map(name=name, limit=limit, offset=offset)
         route = routes.SEARCH_GROUPS.compile().with_params(params)
         data = await self._http.fetch(route, self._list)
 
@@ -94,14 +96,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.get_details(1234)
             ```
         """
         route = routes.GROUP_DETAILS.compile(id)
         data = await self._http.fetch(route, self._dict)
 
         if isinstance(data, models.HttpErrorResponse):
@@ -140,14 +144,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.create_group(
                 "My new group",
                 "Jonxslays",
                 "Zezima",
                 description="The most epic group."
             )
             ```
@@ -217,14 +223,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.edit_group(
                 123,
                 "111-111-111",
                 name="My new group name",
                 members=["Jonxslays"],
                 description="Some new description."
             )
@@ -268,14 +276,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.delete_group(123, "111-111-111")
             ```
         """
         payload = self._generate_map(verificationCode=verification_code)
         route = routes.DELETE_GROUP.compile(id)
         data = await self._http.fetch(route, models.HttpErrorResponse, payload=payload)
 
@@ -303,14 +313,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.add_members(
                 123,
                 "111-111-111",
                 wom.GroupMemberFragment(
                     "Jonxslays", wom.GroupRole.Administrator
                 ),
                 wom.GroupMemberFragment("Zezima"),
@@ -350,14 +362,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.remove_members(
                 123,
                 "111-111-111",
                 "Jonxslays",
                 "Zezima",
             )
             ```
@@ -393,14 +407,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.change_member_role(
                 123,
                 "111-111-111",
                 "Jonxslays",
                 wom.GroupRole.Admiral
             )
             ```
@@ -443,14 +459,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.groups.update_outdated_members(
                 123, "111-111-111"
             )
             ```
 
         Args:
             id: The ID of the group.
@@ -490,14 +508,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.get_competitions(123, limit=10)
             ```
         """
         params = self._generate_map(limit=limit, offset=offset)
         route = routes.GROUP_COMPETITIONS.compile(id).with_params(params)
         data = await self._http.fetch(route, self._list)
 
@@ -550,14 +570,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.get_gains(
                 123, wom.Bosses.Zulrah, limit=10
             )
             ```
         """
         params = self._generate_map(
             limit=limit,
@@ -600,14 +622,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.get_achievements(123, limit=10)
             ```
         """
         params = self._generate_map(limit=limit, offset=offset)
         route = routes.GROUP_ACHIEVEMENTS.compile(id).with_params(params)
         data = await self._http.fetch(route, self._list)
 
@@ -646,14 +670,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.get_records(
                 123, wom.Bosses.Zulrah, wom.Period.Day, limit=3
             )
             ```
         """
         params = self._generate_map(
             limit=limit,
@@ -697,14 +723,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.get_hiscores(
                 123, wom.Skills.Runecrafting, limit=10
             )
             ```
         """
         params = self._generate_map(limit=limit, offset=offset, metric=metric.value)
         route = routes.GROUP_HISCORES.compile(id).with_params(params)
@@ -734,14 +762,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.get_name_changes(123, limit=10)
             ```
         """
         params = self._generate_map(limit=limit, offset=offset)
         route = routes.GROUP_NAME_CHANGES.compile(id).with_params(params)
         data = await self._http.fetch(route, self._list)
 
@@ -762,14 +792,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             await client.groups.get_statistics(123)
             ```
         """
         route = routes.GROUP_STATISTICS.compile(id)
         data = await self._http.fetch(route, self._dict)
 
         if isinstance(data, models.HttpErrorResponse):
```

### Comparing `wom_py-0.3.1/wom/services/http.py` & `wom_py-0.3.2/wom/services/http.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,22 +63,14 @@
             )
         }
 
         if api_key:
             self._headers["x-api-key"] = api_key
 
         self._base_url = api_base_url or constants.WOM_BASE_URL
-        self._session = aiohttp.ClientSession()
-        self._method_mapping = {
-            "GET": self._session.get,
-            "POST": self._session.post,
-            "PUT": self._session.put,
-            "PATCH": self._session.patch,
-            "DELETE": self._session.delete,
-        }
 
     async def _try_get_json(self, response: aiohttp.ClientResponse) -> t.Any:
         try:
             return await response.json()
         except Exception:
             return models.HttpErrorResponse(
                 response.status, "Unable to deserialize response, the api is likely down."
@@ -98,16 +90,29 @@
                 response.status,
                 data.get("message", "An unexpected error occurred while making the request."),
             )
 
         return data
 
     def _get_request_func(self, method: str) -> t.Callable[..., t.Awaitable[t.Any]]:
+        if not hasattr(self, "_method_mapping"):
+            raise RuntimeError("HttpService.start was never called, aborting...")
+
         return self._method_mapping[method]  # type: ignore
 
+    async def _init_session(self) -> None:
+        self._session = aiohttp.ClientSession()
+        self._method_mapping = {
+            "GET": self._session.get,
+            "POST": self._session.post,
+            "PUT": self._session.put,
+            "PATCH": self._session.patch,
+            "DELETE": self._session.delete,
+        }
+
     def set_api_key(self, api_key: str) -> None:
         """Sets the api key used by the http service.
 
         Args:
             api_key: The new api key to use.
         """
         self._headers["x-api-key"] = api_key
@@ -129,17 +134,22 @@
         """Sets the api base url used by the http service.
 
         Args:
             base_url: The new base url to use.
         """
         self._base_url = base_url
 
+    async def start(self) -> None:
+        """Starts the client session to be used by the http service."""
+        if not hasattr(self, "_session"):
+            await self._init_session()
+
     async def close(self) -> None:
         """Closes the existing client session, if it's still open."""
-        if not self._session.closed:
+        if hasattr(self, "_session") and not self._session.closed:
             await self._session.close()
 
     async def fetch(
         self,
         route: routes.CompiledRoute,
         _: t.Type[T],
         *,
```

### Comparing `wom_py-0.3.1/wom/services/names.py` & `wom_py-0.3.2/wom/services/names.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,14 +69,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.names.search_name_changes(
                 "Jonxslays", limit=1
             )
             ```
         """
         params = self._generate_map(username=username, status=status, limit=limit, offset=offset)
         route = routes.SEARCH_NAME_CHANGES.compile().with_params(params)
@@ -101,14 +103,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.names.submit_name_change(
                 "Jonxslays", "I Mahatma I"
             )
             ```
         """
         payload = self._generate_map(oldName=old_name, newName=new_name)
         route = routes.SUBMIT_NAME_CHANGE.compile()
@@ -131,14 +135,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.names.get_name_change_details(123)
             ```
         """
         route = routes.NAME_CHANGE_DETAILS.compile(id)
         data = await self._http.fetch(route, self._dict)
 
         if isinstance(data, models.HttpErrorResponse):
```

### Comparing `wom_py-0.3.1/wom/services/players.py` & `wom_py-0.3.2/wom/services/players.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.search_players("Jonxslays", limit=3)
             ```
         """
         params = self._generate_map(username=username, limit=limit, offset=offset)
         route = routes.SEARCH_PLAYERS.compile().with_params(params)
         data = await self._http.fetch(route, self._list)
 
@@ -93,14 +95,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.update_player("Jonxslays")
             ```
         """
         route = routes.UPDATE_PLAYER.compile(username)
         data = await self._http.fetch(route, self._dict)
 
         if isinstance(data, models.HttpErrorResponse):
@@ -121,14 +125,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.assert_player_type("Jonxslays")
             ```
         """
         route = routes.ASSERT_PLAYER_TYPE.compile(username)
         data = await self._http.fetch(route, self._dict)
 
         if isinstance(data, models.HttpErrorResponse):
@@ -148,14 +154,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.get_details("Jonxslays")
             ```
         """
         route = routes.PLAYER_DETAILS.compile(username)
         data = await self._http.fetch(route, self._dict)
 
         if isinstance(data, models.HttpErrorResponse):
@@ -175,14 +183,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.get_details_by_id(1234)
             ```
         """
         route = routes.PLAYER_DETAILS_BY_ID.compile(player_id)
         data = await self._http.fetch(route, self._dict)
 
         if isinstance(data, models.HttpErrorResponse):
@@ -203,14 +213,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.get_achievements("Jonxslays")
             ```
         """
         route = routes.PLAYER_ACHIEVEMENTS.compile(username)
         data = await self._http.fetch(route, self._list)
 
         if isinstance(data, models.HttpErrorResponse):
@@ -233,14 +245,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.get_achievement_progress("Jonxslays")
             ```
         """
         route = routes.PLAYER_ACHIEVEMENT_PROGRESS.compile(username)
         data = await self._http.fetch(route, self._list)
 
         if isinstance(data, models.HttpErrorResponse):
@@ -281,14 +295,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.get_achievement_progress("Jonxslays")
             ```
         """
         params = self._generate_map(
             status=status.value if status else None, limit=limit, offset=offset
         )
 
@@ -319,14 +335,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.get_competition_standings(
                 "Jonxslays", wom.CompetitionStatus.Ongoing
             )
             ```
         """
         params = self._generate_map(status=status.value)
         route = routes.PLAYER_COMPETITION_STANDINGS.compile(username).with_params(params)
@@ -361,14 +379,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.get_group_memberships(
                 "Jonxslays", limit=3
             )
             ```
         """
         params = self._generate_map(limit=limit, offset=offset)
         route = routes.PLAYER_GROUP_MEMBERSHIPS.compile(username).with_params(params)
@@ -413,14 +433,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.get_gains(
                 "Jonxslays", period=wom.Period.Day
             )
             ```
         """
         params = self._generate_map(
             period=period.value if period else None,
@@ -462,14 +484,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.get_records(
                 "Jonxslays", period=wom.Period.Day, metric=wom.Skills.Attack
             )
             ```
         """
         params = self._generate_map(
             period=period.value if period else None, metric=metric.value if metric else None
@@ -517,14 +541,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.get_snapshots(
                 "Jonxslays", period=wom.Period.Week
             )
             ```
         """
         params = self._generate_map(
             period=period.value if period else None,
@@ -552,14 +578,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.players.get_name_changes("Jonxslays")
             ```
         """
         route = routes.PLAYER_NAME_CHANGES.compile(username)
         data = await self._http.fetch(route, self._list)
 
         if isinstance(data, models.HttpErrorResponse):
```

### Comparing `wom_py-0.3.1/wom/services/records.py` & `wom_py-0.3.2/wom/services/records.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,16 @@
         ??? example
 
             ```py
             import wom
 
             client = wom.Client(...)
 
+            await client.start()
+
             result = await client.records.get_global_record_leaderboards(
                 wom.Skills.Attack,
                 wom.Period.Day,
                 country=wom.Country.Us,
             )
             ```
         """
```

### Comparing `wom_py-0.3.1/PKG-INFO` & `wom_py-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wom-py
-Version: 0.3.1
+Version: 0.3.2
 Summary: An asynchronous wrapper for the Wise Old Man API.
 Home-page: https://github.com/Jonxslays/wom.py
 License: MIT
 Author: Jonxslays
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

