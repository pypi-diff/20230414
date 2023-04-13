# Comparing `tmp/pytmv1-0.2.0.tar.gz` & `tmp/pytmv1-0.3.0.tar.gz`

## Comparing `pytmv1-0.2.0.tar` & `pytmv1-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.2.0/.coveragerc
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.2.0/tox.ini
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/__about__.py
--rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/__init__.py
--rwxr-xr-x   0        0        0    26165 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/caller.py
--rwxr-xr-x   0        0        0    10922 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/core.py
--rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/exceptions.py
--rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/logger.py
--rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/mapper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/py.typed
--rwxr-xr-x   0        0        0     3916 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/results.py
--rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/model/__init__.py
--rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/model/commons.py
--rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/model/enums.py
--rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/model/requests.py
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 pytmv1-0.2.0/src/pytmv1/model/responses.py
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.2.0/.gitignore
--rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.2.0/LICENSE.txt
--rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.2.0/README.md
--rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.3.0/.coveragerc
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.3.0/tox.ini
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/__about__.py
+-rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/__init__.py
+-rwxr-xr-x   0        0        0    26132 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/caller.py
+-rwxr-xr-x   0        0        0    10922 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/core.py
+-rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/exceptions.py
+-rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/logger.py
+-rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/mapper.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/py.typed
+-rwxr-xr-x   0        0        0     3916 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/results.py
+-rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/model/__init__.py
+-rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/model/commons.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/model/enums.py
+-rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/model/requests.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/model/responses.py
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.3.0/.gitignore
+-rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.3.0/LICENSE.txt
+-rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.3.0/README.md
+-rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.3.0/PKG-INFO
```

### Comparing `pytmv1-0.2.0/src/pytmv1/__init__.py` & `pytmv1-0.3.0/src/pytmv1/__init__.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.2.0/src/pytmv1/caller.py` & `pytmv1-0.3.0/src/pytmv1/caller.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,33 +325,33 @@
             poll_time_sec,
         )
 
     def edit_alert_status(
         self,
         alert_id: str,
         status: InvestigationStatus,
-        if_match: Optional[str] = None,
+        if_match: str,
     ) -> Result[NoContentResp]:
         """Edit the status of an alert or investigation triggered in Workbench.
 
         :param alert_id: Workbench alert id.
         :type alert_id: str
         :param status: Status to be updated.
         :type status: InvestigationStatus
         :param if_match: Target resource will be updated only if
          it matches ETag of the target one.
-        :type if_match: Optional[str]
+        :type if_match: str
         :rtype: Result[NoContentResp]:
         """
         return self._core.send(
             NoContentResp,
             Api.EDIT_ALERT_STATUS.value.format(alert_id),
             HttpMethod.PATCH,
             json={"investigationStatus": status},
-            headers=utils.filter_none({"If-Match": if_match}),
+            headers={"If-Match": '"' + if_match + '"'},
         )
 
     def enable_account(self, *accounts: AccountTask) -> MultiResult[MultiResp]:
         """Allows the user to sign in to new application and browser sessions.
 
         :param accounts: Account(s) to enable.
         :type accounts: Tuple[AccountTask, ...]
@@ -750,14 +750,14 @@
         :type processes: Tuple[ProcessTask, ...]
         :rtype: MultiResult[MultiResp]
         """
         return self._core.send_endpoint(
             Api.TERMINATE_ENDPOINT_PROCESS, *processes
         )
 
-    def test_connectivity(self) -> Result[ConnectivityResp]:
+    def check_connectivity(self) -> Result[ConnectivityResp]:
         """Checks the connection to the API service
         and verifies if your authentication token is valid.
 
         :rtype: Result[ConnectivityResp]
         """
         return self._core.send(ConnectivityResp, Api.CONNECTIVITY)
```

### Comparing `pytmv1-0.2.0/src/pytmv1/core.py` & `pytmv1-0.3.0/src/pytmv1/core.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.2.0/src/pytmv1/exceptions.py` & `pytmv1-0.3.0/src/pytmv1/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.2.0/src/pytmv1/logger.py` & `pytmv1-0.3.0/src/pytmv1/logger.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.2.0/src/pytmv1/mapper.py` & `pytmv1-0.3.0/src/pytmv1/mapper.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.2.0/src/pytmv1/results.py` & `pytmv1-0.3.0/src/pytmv1/results.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.2.0/src/pytmv1/utils.py` & `pytmv1-0.3.0/src/pytmv1/utils.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.2.0/src/pytmv1/model/commons.py` & `pytmv1-0.3.0/src/pytmv1/model/commons.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,19 +121,29 @@
     status: int
     code: Optional[str] = None
     message: Optional[str] = None
     number: Optional[int] = None
 
 
 class ExceptionObject(BaseConsumable):
-    url: str
+    value: str
     type: ObjectType
     last_modified_date_time: str
     description: Optional[str]
 
+    def __init__(self, **data: str) -> None:
+        super().__init__(value=self._obj_value(data), **data)
+
+    @staticmethod
+    def _obj_value(args: Dict[str, str]) -> str:
+        obj_value: Optional[str] = args.get(args.get("type", ""))
+        if obj_value is None:
+            raise ValueError("Object value not found")
+        return obj_value
+
 
 class ImpactScope(BaseModel):
     desktop_count: int
     server_count: int
     account_count: int
     email_address_count: int
     entities: List[Entity]
```

### Comparing `pytmv1-0.2.0/src/pytmv1/model/enums.py` & `pytmv1-0.3.0/src/pytmv1/model/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
 
 class QueryOp(str, Enum):
     AND = " and "
     OR = " or "
 
 
 class RiskLevel(str, Enum):
+    NO_RISK = "noRisk"
     LOW = "low"
     MEDIUM = "medium"
     HIGH = "high"
 
 
 class SandboxAction(str, Enum):
     ANALYZE_FILE = "analyzeFile"
```

### Comparing `pytmv1-0.2.0/src/pytmv1/model/requests.py` & `pytmv1-0.3.0/src/pytmv1/model/requests.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.2.0/src/pytmv1/model/responses.py` & `pytmv1-0.3.0/src/pytmv1/model/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,20 +70,20 @@
     location: str = Field(alias="Location")
 
     def note_id(self) -> str:
         return self.location.split("/")[-1]
 
 
 class BlockListTaskResp(BaseTaskResp):
-    object_type: str
-    object_value: str
+    type: ObjectType
+    value: str
 
     def __init__(self, **data: str) -> None:
         obj: Tuple[str, str] = self._map(data)
-        super().__init__(objectType=obj[0], objectValue=obj[1], **data)
+        super().__init__(type=obj[0], value=obj[1], **data)
 
     @staticmethod
     def _map(args: Dict[str, str]) -> Tuple[str, str]:
         return {
             (k, v)
             for k, v in args.items()
             if k in map(lambda ot: ot.value, ObjectType)
```

### Comparing `pytmv1-0.2.0/LICENSE.txt` & `pytmv1-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytmv1-0.2.0/README.md` & `pytmv1-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pytmv1-0.2.0/pyproject.toml` & `pytmv1-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytmv1-0.2.0/PKG-INFO` & `pytmv1-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmv1
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python library for Trend Micro Vision One
 Project-URL: Source, https://github.com/TrendATI/pytmv1
 Project-URL: Issues, https://github.com/TrendATI/pytmv1/issues
 Author-email: Thomas Legros <thomas_legros@trendmicro.com>
 Maintainer-email: TrendATI <ati-integration@trendmicro.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

