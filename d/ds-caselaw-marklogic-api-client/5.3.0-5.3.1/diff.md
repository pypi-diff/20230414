# Comparing `tmp/ds_caselaw_marklogic_api_client-5.3.0.tar.gz` & `tmp/ds_caselaw_marklogic_api_client-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds_caselaw_marklogic_api_client-5.3.0.tar", max compression
+gzip compressed data, was "ds_caselaw_marklogic_api_client-5.3.1.tar", max compression
```

## Comparing `ds_caselaw_marklogic_api_client-5.3.0.tar` & `ds_caselaw_marklogic_api_client-5.3.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1108 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/LICENSE.md
--rw-r--r--   0        0        0     3139 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/README.md
--rw-r--r--   0        0        0      843 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/pyproject.toml
--rw-r--r--   0        0        0    25434 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/Client.py
--rw-r--r--   0        0        0        0 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/__init__.py
--rw-r--r--   0        0        0     1954 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/content_hash.py
--rw-r--r--   0        0        0     2318 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/errors.py
--rw-r--r--   0        0        0        0 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/models/__init__.py
--rw-r--r--   0        0        0     5272 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/models/judgments.py
--rw-r--r--   0        0        0     1128 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/models/utilities/__init__.py
--rw-r--r--   0        0        0     3453 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/models/utilities/aws.py
--rw-r--r--   0        0        0        0 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/py.typed
--rw-r--r--   0        0        0     3580 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xml_tools.py
--rw-r--r--   0        0        0      220 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/break_judgment_checkout.xqy
--rw-r--r--   0        0        0      197 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/checkin_judgment.xqy
--rw-r--r--   0        0        0      385 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/checkout_judgment.xqy
--rw-r--r--   0        0        0      318 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/copy_judgment.xqy
--rw-r--r--   0        0        0      302 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/delete_judgment.xqy
--rw-r--r--   0        0        0      715 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_judgment.xqy
--rw-r--r--   0        0        0      193 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_judgment_checkout_status.xqy
--rw-r--r--   0        0        0      292 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_judgment_version.xqy
--rw-r--r--   0        0        0      172 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_last_modified.xqy
--rw-r--r--   0        0        0      338 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_metadata_citation.xqy
--rw-r--r--   0        0        0      339 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_metadata_court.xqy
--rw-r--r--   0        0        0      221 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_metadata_name.xqy
--rw-r--r--   0        0        0      358 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_metadata_work_date.xqy
--rw-r--r--   0        0        0      594 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_properties_for_search_results.xqy
--rw-r--r--   0        0        0      209 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_property.xqy
--rw-r--r--   0        0        0      326 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/insert_judgment.xqy
--rw-r--r--   0        0        0      190 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/list_judgment_versions.xqy
--rw-r--r--   0        0        0      355 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_boolean_property.xqy
--rw-r--r--   0        0        0      659 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_citation.xqy
--rw-r--r--   0        0        0     1013 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_court.xqy
--rw-r--r--   0        0        0      756 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_name.xqy
--rw-r--r--   0        0        0     1762 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_this_uri.xqy
--rw-r--r--   0        0        0      939 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy
--rw-r--r--   0        0        0      343 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_property.xqy
--rw-r--r--   0        0        0      420 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/update_judgment.xqy
--rw-r--r--   0        0        0      556 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/update_locked_judgment.xqy
--rw-r--r--   0        0        0      371 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/user_has_privilege.xqy
--rw-r--r--   0        0        0      246 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/user_has_role.xqy
--rw-r--r--   0        0        0      156 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/validate_all_documents.xqy
--rw-r--r--   0        0        0      199 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/xslt.xqy
--rw-r--r--   0        0        0     1381 2023-04-12 15:42:38.666958 ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/xslt_transform.xqy
--rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 ds_caselaw_marklogic_api_client-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-04-13 13:47:15.927457 ds_caselaw_marklogic_api_client-5.3.1/LICENSE.md
+-rw-r--r--   0        0        0     3139 2023-04-13 13:47:15.927457 ds_caselaw_marklogic_api_client-5.3.1/README.md
+-rw-r--r--   0        0        0      853 2023-04-13 13:47:15.927457 ds_caselaw_marklogic_api_client-5.3.1/pyproject.toml
+-rw-r--r--   0        0        0    25434 2023-04-13 13:47:15.927457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/Client.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:47:15.927457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/__init__.py
+-rw-r--r--   0        0        0     1954 2023-04-13 13:47:15.927457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/content_hash.py
+-rw-r--r--   0        0        0     2318 2023-04-13 13:47:15.927457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/errors.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:47:15.927457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/models/__init__.py
+-rw-r--r--   0        0        0     5272 2023-04-13 13:47:15.927457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/models/judgments.py
+-rw-r--r--   0        0        0     1128 2023-04-13 13:47:15.927457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/models/utilities/__init__.py
+-rw-r--r--   0        0        0     3453 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/models/utilities/aws.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/py.typed
+-rw-r--r--   0        0        0     3580 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xml_tools.py
+-rw-r--r--   0        0        0      220 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/break_judgment_checkout.xqy
+-rw-r--r--   0        0        0      197 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/checkin_judgment.xqy
+-rw-r--r--   0        0        0      385 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/checkout_judgment.xqy
+-rw-r--r--   0        0        0      318 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/copy_judgment.xqy
+-rw-r--r--   0        0        0      302 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/delete_judgment.xqy
+-rw-r--r--   0        0        0      715 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/get_judgment.xqy
+-rw-r--r--   0        0        0      193 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/get_judgment_checkout_status.xqy
+-rw-r--r--   0        0        0      292 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/get_judgment_version.xqy
+-rw-r--r--   0        0        0      172 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/get_last_modified.xqy
+-rw-r--r--   0        0        0      338 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/get_metadata_citation.xqy
+-rw-r--r--   0        0        0      339 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/get_metadata_court.xqy
+-rw-r--r--   0        0        0      221 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/get_metadata_name.xqy
+-rw-r--r--   0        0        0      358 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/get_metadata_work_date.xqy
+-rw-r--r--   0        0        0      594 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/get_properties_for_search_results.xqy
+-rw-r--r--   0        0        0      209 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/get_property.xqy
+-rw-r--r--   0        0        0      326 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/insert_judgment.xqy
+-rw-r--r--   0        0        0      190 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/list_judgment_versions.xqy
+-rw-r--r--   0        0        0      355 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/set_boolean_property.xqy
+-rw-r--r--   0        0        0      659 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/set_metadata_citation.xqy
+-rw-r--r--   0        0        0     1013 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/set_metadata_court.xqy
+-rw-r--r--   0        0        0      756 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/set_metadata_name.xqy
+-rw-r--r--   0        0        0     1762 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/set_metadata_this_uri.xqy
+-rw-r--r--   0        0        0      939 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/set_metadata_work_expression_date.xqy
+-rw-r--r--   0        0        0      343 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/set_property.xqy
+-rw-r--r--   0        0        0      420 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/update_judgment.xqy
+-rw-r--r--   0        0        0      556 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/update_locked_judgment.xqy
+-rw-r--r--   0        0        0      371 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/user_has_privilege.xqy
+-rw-r--r--   0        0        0      246 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/user_has_role.xqy
+-rw-r--r--   0        0        0      156 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/validate_all_documents.xqy
+-rw-r--r--   0        0        0      199 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/xslt.xqy
+-rw-r--r--   0        0        0     1381 2023-04-13 13:47:15.931457 ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/xslt_transform.xqy
+-rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 ds_caselaw_marklogic_api_client-5.3.1/PKG-INFO
```

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/LICENSE.md` & `ds_caselaw_marklogic_api_client-5.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/README.md` & `ds_caselaw_marklogic_api_client-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/pyproject.toml` & `ds_caselaw_marklogic_api_client-5.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "ds-caselaw-marklogic-api-client"
-version = "5.3.0"
+version = "5.3.1"
 description = "An API client for interacting with the underlying data in Find Caselaw."
 authors = ["The National Archives"]
 homepage = "https://github.com/nationalarchives/ds-caselaw-custom-api-client"
 keywords = ["national archives", "caselaw"]
 readme = "README.md"
 packages = [
-    { include = "src/caselawclient" },
+    { include = "caselawclient", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 certifi = "2022.12.7"
 charset-normalizer = "2.1.1"
 django-environ = "0.10.0"
 idna = "3.4"
 requests = "2.28.2"
 requests-toolbelt = "0.10.1"
 urllib3 = "1.26.15"
 memoization = "0.4.0"
 lxml = "4.9.2"
-ds-caselaw-utils = "^0.5.0"
-boto3 = "^1.26.107"
+ds-caselaw-utils = "^1.0.0"
+boto3 = "^1.26.112"
 
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.3"
 pytest = "7.3.0"
 
 [build-system]
```

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/Client.py` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/Client.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/content_hash.py` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/content_hash.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/errors.py` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/errors.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/models/judgments.py` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/models/judgments.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/models/utilities/__init__.py` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/models/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/models/utilities/aws.py` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/models/utilities/aws.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xml_tools.py` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xml_tools.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_judgment.xqy` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/get_judgment.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/get_properties_for_search_results.xqy` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/get_properties_for_search_results.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_citation.xqy` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/set_metadata_citation.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_court.xqy` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/set_metadata_court.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_name.xqy` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/set_metadata_name.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_this_uri.xqy` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/set_metadata_this_uri.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/set_metadata_work_expression_date.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/update_locked_judgment.xqy` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/update_locked_judgment.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/src/caselawclient/xquery/xslt_transform.xqy` & `ds_caselaw_marklogic_api_client-5.3.1/src/caselawclient/xquery/xslt_transform.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-5.3.0/PKG-INFO` & `ds_caselaw_marklogic_api_client-5.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ds-caselaw-marklogic-api-client
-Version: 5.3.0
+Version: 5.3.1
 Summary: An API client for interacting with the underlying data in Find Caselaw.
 Home-page: https://github.com/nationalarchives/ds-caselaw-custom-api-client
 Keywords: national archives,caselaw
 Author: The National Archives
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: boto3 (>=1.26.107,<2.0.0)
+Requires-Dist: boto3 (>=1.26.112,<2.0.0)
 Requires-Dist: certifi (==2022.12.7)
 Requires-Dist: charset-normalizer (==2.1.1)
 Requires-Dist: django-environ (==0.10.0)
-Requires-Dist: ds-caselaw-utils (>=0.5.0,<0.6.0)
+Requires-Dist: ds-caselaw-utils (>=1.0.0,<2.0.0)
 Requires-Dist: idna (==3.4)
 Requires-Dist: lxml (==4.9.2)
 Requires-Dist: memoization (==0.4.0)
 Requires-Dist: requests (==2.28.2)
 Requires-Dist: requests-toolbelt (==0.10.1)
 Requires-Dist: urllib3 (==1.26.15)
 Description-Content-Type: text/markdown
```

