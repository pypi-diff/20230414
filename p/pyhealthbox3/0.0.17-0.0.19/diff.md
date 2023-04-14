# Comparing `tmp/pyhealthbox3-0.0.17.tar.gz` & `tmp/pyhealthbox3-0.0.19.tar.gz`

## Comparing `pyhealthbox3-0.0.17.tar` & `pyhealthbox3-0.0.19.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/requirements.txt
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/.github/workflows/publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/pyhealthbox3/__init__.py
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/pyhealthbox3/healthbox3.py
--rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/pyhealthbox3/models.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/LICENSE
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/README.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/pyproject.toml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.19/requirements.txt
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.19/.github/workflows/publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.19/pyhealthbox3/__init__.py
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.19/pyhealthbox3/healthbox3.py
+-rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.19/pyhealthbox3/models.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.19/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.19/LICENSE
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.19/README.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.19/pyproject.toml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pyhealthbox3-0.0.19/PKG-INFO
```

### Comparing `pyhealthbox3-0.0.17/pyhealthbox3/healthbox3.py` & `pyhealthbox3-0.0.19/pyhealthbox3/healthbox3.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,27 +103,30 @@
                 method=METH_GET, endpoint=f"/v2/api/boost/{room_id}"
             )
             return Healthbox3RoomBoost(level=data["level"],enabled=data["enable"],remaining=data["remaining"])
         except:
             return Healthbox3RoomBoost()
         
 
-    async def async_enable_advanced_api_features(self):
+    async def async_enable_advanced_api_features(self, pre_validation: bool = True):
         """Enable advanced API Features."""
         if self._api_key:
-            already_valid = await self._async_validate_advanced_api_features()
+            already_valid = False
+            if pre_validation:
+                _LOGGER.debug("Pre validating advanced API to check if already enabled.")
+                already_valid = await self._async_validate_advanced_api_features()
             if not already_valid:
                 _LOGGER.debug("Enabling Advanced API.")
                 await self.request(
                     method=METH_POST,
                     endpoint="/v2/api/api_key",
                     data=f"{self._api_key}",
                     expect_json_error=True,
                 )
-                await asyncio.sleep(5)
+                await asyncio.sleep(10)
                 if await self._async_validate_advanced_api_features() == False:
                     await self.close()
                     raise Healthbox3ApiClientAuthenticationError
             else:
                 _LOGGER.debug("Advanced API already enabled.")
         else:
             raise Healthbox3ApiClientAuthenticationError
```

### Comparing `pyhealthbox3-0.0.17/pyhealthbox3/models.py` & `pyhealthbox3-0.0.19/pyhealthbox3/models.py`

 * *Files identical despite different names*

### Comparing `pyhealthbox3-0.0.17/.gitignore` & `pyhealthbox3-0.0.19/.gitignore`

 * *Files identical despite different names*

### Comparing `pyhealthbox3-0.0.17/LICENSE` & `pyhealthbox3-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhealthbox3-0.0.17/pyproject.toml` & `pyhealthbox3-0.0.19/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyhealthbox3"
-version = "0.0.17"
+version = "0.0.19"
 authors = [
   { name="rmassch", email="1083135+rmassch@users.noreply.github.com" },
 ]
 description = "Renson Healthbox3 Package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyhealthbox3-0.0.17/PKG-INFO` & `pyhealthbox3-0.0.19/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhealthbox3
-Version: 0.0.17
+Version: 0.0.19
 Summary: Renson Healthbox3 Package
 Project-URL: Homepage, https://github.com/rmassch/pyhealthbox3
 Project-URL: Bug Tracker, https://github.com/rmassch/pyhealthbox3/issues
 Author-email: rmassch <1083135+rmassch@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

