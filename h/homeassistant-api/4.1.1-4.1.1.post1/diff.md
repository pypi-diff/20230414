# Comparing `tmp/homeassistant_api-4.1.1.tar.gz` & `tmp/homeassistant_api-4.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant_api-4.1.1.tar", max compression
+gzip compressed data, was "homeassistant_api-4.1.1.post1.tar", max compression
```

## Comparing `homeassistant_api-4.1.1.tar` & `homeassistant_api-4.1.1.post1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    32473 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/LICENSE
--rw-r--r--   0        0        0     2069 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/README.md
--rw-r--r--   0        0        0     1139 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/homeassistant_api/__init__.py
--rw-r--r--   0        0        0     1313 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/homeassistant_api/client.py
--rw-r--r--   0        0        0     2841 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/homeassistant_api/errors.py
--rw-r--r--   0        0        0      474 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/homeassistant_api/models/__init__.py
--rw-r--r--   0        0        0      594 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/homeassistant_api/models/base.py
--rw-r--r--   0        0        0     4256 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/homeassistant_api/models/domains.py
--rw-r--r--   0        0        0     4293 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/homeassistant_api/models/entity.py
--rw-r--r--   0        0        0     1387 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/homeassistant_api/models/events.py
--rw-r--r--   0        0        0      720 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/homeassistant_api/models/history.py
--rw-r--r--   0        0        0      983 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/homeassistant_api/models/logbook.py
--rw-r--r--   0        0        0     1322 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/homeassistant_api/models/states.py
--rw-r--r--   0        0        0     5391 2023-03-12 00:00:38.243436 homeassistant_api-4.1.1/homeassistant_api/processing.py
--rw-r--r--   0        0        0        0 2023-03-12 00:00:38.247436 homeassistant_api-4.1.1/homeassistant_api/py.typed
--rw-r--r--   0        0        0    12645 2023-03-12 00:00:38.247436 homeassistant_api-4.1.1/homeassistant_api/rawasyncclient.py
--rw-r--r--   0        0        0     5570 2023-03-12 00:00:38.247436 homeassistant_api-4.1.1/homeassistant_api/rawbaseclient.py
--rw-r--r--   0        0        0    12191 2023-03-12 00:00:38.247436 homeassistant_api-4.1.1/homeassistant_api/rawclient.py
--rw-r--r--   0        0        0     2261 2023-03-12 00:00:38.247436 homeassistant_api-4.1.1/pyproject.toml
--rw-r--r--   0        0        0     3194 1970-01-01 00:00:00.000000 homeassistant_api-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-04-14 18:04:37.583228 homeassistant_api-4.1.1.post1/LICENSE
+-rw-r--r--   0        0        0     2069 2023-04-14 18:04:37.583228 homeassistant_api-4.1.1.post1/README.md
+-rw-r--r--   0        0        0     1139 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/__init__.py
+-rw-r--r--   0        0        0     1313 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/client.py
+-rw-r--r--   0        0        0     2841 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/errors.py
+-rw-r--r--   0        0        0      474 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/__init__.py
+-rw-r--r--   0        0        0      594 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/base.py
+-rw-r--r--   0        0        0     4241 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/domains.py
+-rw-r--r--   0        0        0     4293 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/entity.py
+-rw-r--r--   0        0        0     1387 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/events.py
+-rw-r--r--   0        0        0      720 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/history.py
+-rw-r--r--   0        0        0      983 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/logbook.py
+-rw-r--r--   0        0        0     1322 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/models/states.py
+-rw-r--r--   0        0        0     5391 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/processing.py
+-rw-r--r--   0        0        0        0 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/py.typed
+-rw-r--r--   0        0        0    12645 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/rawasyncclient.py
+-rw-r--r--   0        0        0     5570 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/rawbaseclient.py
+-rw-r--r--   0        0        0    12191 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/homeassistant_api/rawclient.py
+-rw-r--r--   0        0        0     2267 2023-04-14 18:04:37.587225 homeassistant_api-4.1.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     3200 1970-01-01 00:00:00.000000 homeassistant_api-4.1.1.post1/PKG-INFO
```

### Comparing `homeassistant_api-4.1.1/LICENSE` & `homeassistant_api-4.1.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/README.md` & `homeassistant_api-4.1.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/homeassistant_api/__init__.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/__init__.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/homeassistant_api/client.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/client.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/homeassistant_api/errors.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/errors.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/homeassistant_api/models/base.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/models/base.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/homeassistant_api/models/domains.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/models/domains.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         assert isinstance(services, dict)
         for service_id, data in services.items():
             domain._add_service(service_id, **data)
         return domain
 
     def _add_service(self, service_id: str, **data) -> None:
         """Registers services into a domain to be used or accessed. Used internally."""
+        # raise ValueError(data)
         self.services.update(
             {
                 service_id: Service(
                     service_id=service_id,
                     domain=self,
                     **data,
                 )
@@ -69,29 +70,28 @@
         return super().__getattribute__(attr)
 
 
 class ServiceField(BaseModel):
     """Model for service parameters/fields."""
 
     description: Optional[str] = None
-    example: Any
+    example: Any = None
     selector: Optional[Dict[str, Any]] = None
     name: Optional[str] = None
     required: Optional[bool] = None
 
 
 class Service(BaseModel):
     """Model representing services from homeassistant"""
 
     service_id: str
     domain: Domain = Field(exclude=True, repr=False)
     name: Optional[str] = None
     description: Optional[str] = None
     fields: Optional[Dict[str, ServiceField]] = None
-    target: Optional[Dict[str, Dict[str, Any]]] = None
 
     def trigger(self, **service_data) -> Tuple[State, ...]:
         """Triggers the service associated with this object."""
         return self.domain._client.trigger_service(
             self.domain.domain_id,
             self.service_id,
             **service_data,
```

### Comparing `homeassistant_api-4.1.1/homeassistant_api/models/entity.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/models/entity.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/homeassistant_api/models/events.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/models/events.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/homeassistant_api/models/history.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/models/history.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/homeassistant_api/models/logbook.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/models/logbook.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/homeassistant_api/models/states.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/models/states.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/homeassistant_api/processing.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/processing.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/homeassistant_api/rawasyncclient.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/rawasyncclient.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/homeassistant_api/rawbaseclient.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/rawbaseclient.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/homeassistant_api/rawclient.py` & `homeassistant_api-4.1.1.post1/homeassistant_api/rawclient.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.1.1/pyproject.toml` & `homeassistant_api-4.1.1.post1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 documentation = "https://homeassistantapi.readthedocs.io"
 homepage = "https://github.com/GrandMoff100/HomeAssistantAPI"
 license = "GPL-3.0-or-later"
 name = "HomeAssistant-API"
 readme = "README.md"
 include = ["homeassistant_api/py.typed"]
 repository = "https://github.com/GrandMoff100/HomeAssistantAPI"
-version = "4.1.1"
+version = "4.1.1.post1"
 packages = [{ include = "homeassistant_api" }]
 
 [tool.poetry.dependencies]
 aiohttp = "^3.8.1"
 aiohttp-client-cache = "^0.6.1"
 pydantic = "<=1.9.0"
 python = "^3.7,<4.0.0"
```

### Comparing `homeassistant_api-4.1.1/PKG-INFO` & `homeassistant_api-4.1.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeassistant-api
-Version: 4.1.1
+Version: 4.1.1.post1
 Summary: Python Wrapper for Homeassistant's REST API
 Home-page: https://github.com/GrandMoff100/HomeAssistantAPI
 License: GPL-3.0-or-later
 Author: GrandMoff100
 Author-email: minecraftcrusher100@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: homeassistant-api Version: 4.1.1 Summary: Python
-Wrapper for Homeassistant's REST API Home-page: https://github.com/
+Metadata-Version: 2.1 Name: homeassistant-api Version: 4.1.1.post1 Summary:
+Python Wrapper for Homeassistant's REST API Home-page: https://github.com/
 GrandMoff100/HomeAssistantAPI License: GPL-3.0-or-later Author: GrandMoff100
 Author-email: minecraftcrusher100@gmail.com Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later
 (GPLv3+) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

