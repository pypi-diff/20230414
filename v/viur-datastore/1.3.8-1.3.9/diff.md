# Comparing `tmp/viur-datastore-1.3.8.tar.gz` & `tmp/viur-datastore-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur-datastore-1.3.8.tar", last modified: Mon Apr  3 16:23:11 2023, max compression
+gzip compressed data, was "viur-datastore-1.3.9.tar", last modified: Fri Apr 14 08:28:37 2023, max compression
```

## Comparing `viur-datastore-1.3.8.tar` & `viur-datastore-1.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 hotte     (1001) hotte     (1001)        0 2023-04-03 16:23:11.283265 viur-datastore-1.3.8/
--rw-r--r--   0 hotte     (1001) hotte     (1001)      206 2022-03-17 15:38:51.000000 viur-datastore-1.3.8/LICENSE
--rw-r--r--   0 hotte     (1001) hotte     (1001)    11356 2022-03-17 15:38:51.000000 viur-datastore-1.3.8/LICENSE-APACHE
--rw-r--r--   0 hotte     (1001) hotte     (1001)     7651 2022-03-17 15:38:51.000000 viur-datastore-1.3.8/LICENSE-GPL
--rw-r--r--   0 hotte     (1001) hotte     (1001)       92 2022-03-17 15:38:51.000000 viur-datastore-1.3.8/MANIFEST.in
--rw-r--r--   0 hotte     (1001) hotte     (1001)     3371 2023-04-03 16:23:11.283265 viur-datastore-1.3.8/PKG-INFO
--rw-r--r--   0 hotte     (1001) hotte     (1001)     2735 2022-09-22 17:51:49.000000 viur-datastore-1.3.8/README.md
--rw-r--r--   0 hotte     (1001) hotte     (1001)      102 2022-03-17 15:38:51.000000 viur-datastore-1.3.8/pyproject.toml
--rw-r--r--   0 hotte     (1001) hotte     (1001)       38 2023-04-03 16:23:11.283265 viur-datastore-1.3.8/setup.cfg
--rw-r--r--   0 hotte     (1001) hotte     (1001)      979 2023-04-03 15:09:16.000000 viur-datastore-1.3.8/setup.py
-drwxr-xr-x   0 hotte     (1001) hotte     (1001)        0 2023-04-03 16:23:11.280265 viur-datastore-1.3.8/src/
-drwxr-xr-x   0 hotte     (1001) hotte     (1001)        0 2023-04-03 16:23:11.280265 viur-datastore-1.3.8/src/viur/
-drwxr-xr-x   0 hotte     (1001) hotte     (1001)        0 2023-04-03 16:23:11.282265 viur-datastore-1.3.8/src/viur/datastore/
--rw-r--r--   0 hotte     (1001) hotte     (1001)     1517 2022-12-22 09:20:39.000000 viur-datastore-1.3.8/src/viur/datastore/__init__.py
--rw-r--r--   0 hotte     (1001) hotte     (1001)      750 2022-12-07 11:49:00.000000 viur-datastore-1.3.8/src/viur/datastore/config.py
--rw-r--r--   0 hotte     (1001) hotte     (1001)     4619 2022-09-22 17:51:49.000000 viur-datastore-1.3.8/src/viur/datastore/errors.py
--rw-r--r--   0 hotte     (1001) hotte     (1001)    27984 2023-04-03 15:02:31.000000 viur-datastore-1.3.8/src/viur/datastore/query.py
--rw-r--r--   0 hotte     (1001) hotte     (1001)   504844 2022-12-22 09:20:37.000000 viur-datastore-1.3.8/src/viur/datastore/simdjson.cpp
--rw-r--r--   0 hotte     (1001) hotte     (1001)   939337 2022-12-22 09:20:37.000000 viur-datastore-1.3.8/src/viur/datastore/simdjson.h
--rw-r--r--   0 hotte     (1001) hotte     (1001)   875865 2023-04-03 16:23:11.000000 viur-datastore-1.3.8/src/viur/datastore/transport.cpp
--rw-r--r--   0 hotte     (1001) hotte     (1001)    33659 2022-12-22 09:42:07.000000 viur-datastore-1.3.8/src/viur/datastore/transport.pyx
--rw-r--r--   0 hotte     (1001) hotte     (1001)     6787 2023-01-13 00:14:34.000000 viur-datastore-1.3.8/src/viur/datastore/types.py
--rw-r--r--   0 hotte     (1001) hotte     (1001)     5862 2023-04-03 16:02:25.000000 viur-datastore-1.3.8/src/viur/datastore/utils.py
-drwxr-xr-x   0 hotte     (1001) hotte     (1001)        0 2023-04-03 16:23:11.283265 viur-datastore-1.3.8/src/viur_datastore.egg-info/
--rw-r--r--   0 hotte     (1001) hotte     (1001)     3371 2023-04-03 16:23:11.000000 viur-datastore-1.3.8/src/viur_datastore.egg-info/PKG-INFO
--rw-r--r--   0 hotte     (1001) hotte     (1001)      549 2023-04-03 16:23:11.000000 viur-datastore-1.3.8/src/viur_datastore.egg-info/SOURCES.txt
--rw-r--r--   0 hotte     (1001) hotte     (1001)        1 2023-04-03 16:23:11.000000 viur-datastore-1.3.8/src/viur_datastore.egg-info/dependency_links.txt
--rw-r--r--   0 hotte     (1001) hotte     (1001)        5 2023-04-03 16:23:11.000000 viur-datastore-1.3.8/src/viur_datastore.egg-info/top_level.txt
+drwxr-xr-x   0 hotte     (1001) hotte     (1001)        0 2023-04-14 08:28:37.167093 viur-datastore-1.3.9/
+-rw-r--r--   0 hotte     (1001) hotte     (1001)      206 2022-03-17 15:38:51.000000 viur-datastore-1.3.9/LICENSE
+-rw-r--r--   0 hotte     (1001) hotte     (1001)    11356 2022-03-17 15:38:51.000000 viur-datastore-1.3.9/LICENSE-APACHE
+-rw-r--r--   0 hotte     (1001) hotte     (1001)     7651 2022-03-17 15:38:51.000000 viur-datastore-1.3.9/LICENSE-GPL
+-rw-r--r--   0 hotte     (1001) hotte     (1001)       92 2022-03-17 15:38:51.000000 viur-datastore-1.3.9/MANIFEST.in
+-rw-r--r--   0 hotte     (1001) hotte     (1001)     3371 2023-04-14 08:28:37.167093 viur-datastore-1.3.9/PKG-INFO
+-rw-r--r--   0 hotte     (1001) hotte     (1001)     2735 2022-09-22 17:51:49.000000 viur-datastore-1.3.9/README.md
+-rw-r--r--   0 hotte     (1001) hotte     (1001)      102 2022-03-17 15:38:51.000000 viur-datastore-1.3.9/pyproject.toml
+-rw-r--r--   0 hotte     (1001) hotte     (1001)       38 2023-04-14 08:28:37.167093 viur-datastore-1.3.9/setup.cfg
+-rw-r--r--   0 hotte     (1001) hotte     (1001)      979 2023-04-14 08:27:20.000000 viur-datastore-1.3.9/setup.py
+drwxr-xr-x   0 hotte     (1001) hotte     (1001)        0 2023-04-14 08:28:37.165093 viur-datastore-1.3.9/src/
+drwxr-xr-x   0 hotte     (1001) hotte     (1001)        0 2023-04-14 08:28:37.165093 viur-datastore-1.3.9/src/viur/
+drwxr-xr-x   0 hotte     (1001) hotte     (1001)        0 2023-04-14 08:28:37.167093 viur-datastore-1.3.9/src/viur/datastore/
+-rw-r--r--   0 hotte     (1001) hotte     (1001)     1517 2022-12-22 09:20:39.000000 viur-datastore-1.3.9/src/viur/datastore/__init__.py
+-rw-r--r--   0 hotte     (1001) hotte     (1001)      750 2022-12-07 11:49:00.000000 viur-datastore-1.3.9/src/viur/datastore/config.py
+-rw-r--r--   0 hotte     (1001) hotte     (1001)     4619 2022-09-22 17:51:49.000000 viur-datastore-1.3.9/src/viur/datastore/errors.py
+-rw-r--r--   0 hotte     (1001) hotte     (1001)    27984 2023-04-03 15:02:31.000000 viur-datastore-1.3.9/src/viur/datastore/query.py
+-rw-r--r--   0 hotte     (1001) hotte     (1001)   504844 2022-12-22 09:20:37.000000 viur-datastore-1.3.9/src/viur/datastore/simdjson.cpp
+-rw-r--r--   0 hotte     (1001) hotte     (1001)   939337 2022-12-22 09:20:37.000000 viur-datastore-1.3.9/src/viur/datastore/simdjson.h
+-rw-r--r--   0 hotte     (1001) hotte     (1001)   885747 2023-04-14 08:28:36.000000 viur-datastore-1.3.9/src/viur/datastore/transport.cpp
+-rw-r--r--   0 hotte     (1001) hotte     (1001)    33998 2023-04-14 08:20:25.000000 viur-datastore-1.3.9/src/viur/datastore/transport.pyx
+-rw-r--r--   0 hotte     (1001) hotte     (1001)     6787 2023-01-13 00:14:34.000000 viur-datastore-1.3.9/src/viur/datastore/types.py
+-rw-r--r--   0 hotte     (1001) hotte     (1001)     5862 2023-04-03 16:02:25.000000 viur-datastore-1.3.9/src/viur/datastore/utils.py
+drwxr-xr-x   0 hotte     (1001) hotte     (1001)        0 2023-04-14 08:28:37.167093 viur-datastore-1.3.9/src/viur_datastore.egg-info/
+-rw-r--r--   0 hotte     (1001) hotte     (1001)     3371 2023-04-14 08:28:37.000000 viur-datastore-1.3.9/src/viur_datastore.egg-info/PKG-INFO
+-rw-r--r--   0 hotte     (1001) hotte     (1001)      549 2023-04-14 08:28:37.000000 viur-datastore-1.3.9/src/viur_datastore.egg-info/SOURCES.txt
+-rw-r--r--   0 hotte     (1001) hotte     (1001)        1 2023-04-14 08:28:37.000000 viur-datastore-1.3.9/src/viur_datastore.egg-info/dependency_links.txt
+-rw-r--r--   0 hotte     (1001) hotte     (1001)        5 2023-04-14 08:28:37.000000 viur-datastore-1.3.9/src/viur_datastore.egg-info/top_level.txt
```

### Comparing `viur-datastore-1.3.8/LICENSE-APACHE` & `viur-datastore-1.3.9/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `viur-datastore-1.3.8/LICENSE-GPL` & `viur-datastore-1.3.9/LICENSE-GPL`

 * *Files identical despite different names*

### Comparing `viur-datastore-1.3.8/PKG-INFO` & `viur-datastore-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-datastore
-Version: 1.3.8
+Version: 1.3.9
 Summary: A faster replacement for google-cloud-datastore
 Home-page: https://github.com/viur-framework/viur-datastore
 Author: Tobias Steinrücken, Stefan Kögl
 Author-email: devs@viur.dev
 Maintainer: Stefan Kögl
 Maintainer-email: devs@viur.dev
 Classifier: Programming Language :: Python :: 3
```

### Comparing `viur-datastore-1.3.8/README.md` & `viur-datastore-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `viur-datastore-1.3.8/setup.py` & `viur-datastore-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, Extension
 from Cython.Build import cythonize
 from Cython.Distutils import build_ext
 
 setup(
 	name='viur-datastore',
-	version="1.3.8",
+	version="1.3.9",
 	author="Tobias Steinrücken, Stefan Kögl",
 	author_email="devs@viur.dev",
 	maintainer="Stefan Kögl",
 	maintainer_email="devs@viur.dev",
 	description="A faster replacement for google-cloud-datastore",
 	long_description=open("README.md", "r").read(),
 	long_description_content_type="text/markdown",
```

### Comparing `viur-datastore-1.3.8/src/viur/datastore/__init__.py` & `viur-datastore-1.3.9/src/viur/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `viur-datastore-1.3.8/src/viur/datastore/config.py` & `viur-datastore-1.3.9/src/viur/datastore/config.py`

 * *Files identical despite different names*

### Comparing `viur-datastore-1.3.8/src/viur/datastore/errors.py` & `viur-datastore-1.3.9/src/viur/datastore/errors.py`

 * *Files identical despite different names*

### Comparing `viur-datastore-1.3.8/src/viur/datastore/query.py` & `viur-datastore-1.3.9/src/viur/datastore/query.py`

 * *Files identical despite different names*

### Comparing `viur-datastore-1.3.8/src/viur/datastore/simdjson.cpp` & `viur-datastore-1.3.9/src/viur/datastore/simdjson.cpp`

 * *Files identical despite different names*

### Comparing `viur-datastore-1.3.8/src/viur/datastore/simdjson.h` & `viur-datastore-1.3.9/src/viur/datastore/simdjson.h`

 * *Files identical despite different names*

### Comparing `viur-datastore-1.3.8/src/viur/datastore/transport.cpp` & `viur-datastore-1.3.9/src/viur/datastore/transport.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1951,19 +1951,21 @@
 static const char __pyx_k_RequestsConnectionError[] = "RequestsConnectionError";
 static const char __pyx_k_viur_datastore_transport[] = "viur.datastore.transport";
 static const char __pyx_k_INVALID_RESPONSE_RECEIVED[] = "INVALID RESPONSE RECEIVED";
 static const char __pyx_k_Invalid_key_in_entity_json_s[] = "Invalid key in entity json: %s";
 static const char __pyx_k_No_mutation_results_received[] = "No mutation results received";
 static const char __pyx_k_is_viur_datastore_request_ok[] = "is_viur_datastore_request_ok";
 static const char __pyx_k_No_mutation_results_received_2[] = "No mutation-results received";
+static const char __pyx_k_Please_create_a_matching_index[] = ". - Please create a matching index";
 static const char __pyx_k_All_retries_are_exhausted_for_th[] = "All retries are exhausted for this transaction";
 static const char __pyx_k_Cannot_call_runInTransaction_whi[] = "Cannot call runInTransaction while inside a transaction!";
 static const char __pyx_k_Empty_response_received_from_Dat[] = "Empty response received from Datastore API";
 static const char __pyx_k_Invalid_data_received_from_Datas[] = "Invalid data received from Datastore API";
 static const char __pyx_k_Invalid_number_of_mutation_resul[] = "Invalid number of mutation-results received";
+static const char __pyx_k_Query_not_finished_Maybe_some_en[] = "Query not finished. Maybe some entries are missing.";
 static const char __pyx_k_Received_an_unexpected_key_updat[] = "Received an unexpected key-update";
 static const char __pyx_k_Retrying_http_post_request_to_da[] = "Retrying http post request to datastore";
 static const char __pyx_k_The_Count_aggregation_query_is_a[] = "The 'Count() aggregation' query is a technical preview and cannot be guaranteed to work at this time!!!";
 static const char __pyx_k_We_read_an_incomplete_null_key_f[] = "We read an incomplete/null key from the datastore. This is likely a bug!";
 static const char __pyx_k_https_datastore_googleapis_com_v[] = "https://datastore.googleapis.com/v1/projects/%s:runQuery";
 static const char __pyx_k_https_www_googleapis_com_auth_da[] = "https://www.googleapis.com/auth/datastore";
 static const char __pyx_k_src_viur_datastore_transport_pyx[] = "src/viur/datastore/transport.pyx";
@@ -2005,17 +2007,19 @@
 static PyObject *__pyx_n_u_NON_TRANSACTIONAL;
 static PyObject *__pyx_n_u_NOT_FINISHED;
 static PyObject *__pyx_n_u_NO_MORE_RESULTS;
 static PyObject *__pyx_n_s_NoMutationResultsError;
 static PyObject *__pyx_kp_u_No_mutation_results_received;
 static PyObject *__pyx_kp_u_No_mutation_results_received_2;
 static PyObject *__pyx_kp_u_None;
+static PyObject *__pyx_kp_u_Please_create_a_matching_index;
 static PyObject *__pyx_n_s_Put;
 static PyObject *__pyx_kp_u_Queried;
 static PyObject *__pyx_n_s_QueryDefinition;
+static PyObject *__pyx_kp_u_Query_not_finished_Maybe_some_en;
 static PyObject *__pyx_kp_u_Received_an_unexpected_key_updat;
 static PyObject *__pyx_n_s_RecursionError;
 static PyObject *__pyx_n_s_RequestsConnectionError;
 static PyObject *__pyx_kp_u_Retrying_http_post_request_to_da;
 static PyObject *__pyx_kp_u_Returned;
 static PyObject *__pyx_n_s_RunInTransaction;
 static PyObject *__pyx_n_u_STRONG;
@@ -8274,15 +8278,15 @@
     if (__pyx_t_12) {
 
       /* "viur/datastore/transport.pyx":547
  * 		element = element.at_key("batch")
  * 		if element.at_pointer("/entityResults").error() == SUCCESS:
  * 			res.extend(toEntityStructure(element.at_key("entityResults"), isInitial=False))             # <<<<<<<<<<<<<<
  * 		else:  # No results received
- * 			break
+ * 			if toPyStr(element.at_key("moreResults").get_string()) == "NOT_FINISHED":
  */
       try {
         __pyx_t_18 = __pyx_v_element.at_key(((char const *)"entityResults"));
       } catch(...) {
         __Pyx_CppExn2PyErr();
         __PYX_ERR(0, 547, __pyx_L1_error)
       }
@@ -8302,386 +8306,552 @@
  */
       goto __pyx_L39;
     }
 
     /* "viur/datastore/transport.pyx":549
  * 			res.extend(toEntityStructure(element.at_key("entityResults"), isInitial=False))
  * 		else:  # No results received
- * 			break             # <<<<<<<<<<<<<<
+ * 			if toPyStr(element.at_key("moreResults").get_string()) == "NOT_FINISHED":             # <<<<<<<<<<<<<<
+ * 				logging.warning("Query not finished. Maybe some entries are missing.")
+ * 				logging.warning("Queried %s with filter %s and orders %s. - Please create a matching index" % (
+ */
+    /*else*/ {
+      try {
+        __pyx_t_18 = __pyx_v_element.at_key(((char const *)"moreResults"));
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(0, 549, __pyx_L1_error)
+      }
+      try {
+        __pyx_t_20 = __pyx_t_18.get_string();
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(0, 549, __pyx_L1_error)
+      }
+      __pyx_t_2 = __pyx_f_4viur_9datastore_9transport_toPyStr(__pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 549, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_12 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_NOT_FINISHED, Py_EQ)); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 549, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      if (__pyx_t_12) {
+
+        /* "viur/datastore/transport.pyx":550
+ * 		else:  # No results received
+ * 			if toPyStr(element.at_key("moreResults").get_string()) == "NOT_FINISHED":
+ * 				logging.warning("Query not finished. Maybe some entries are missing.")             # <<<<<<<<<<<<<<
+ * 				logging.warning("Queried %s with filter %s and orders %s. - Please create a matching index" % (
+ * 					queryDefinition.kind, queryDefinition.filters, queryDefinition.orders))
+ */
+        __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logging); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 550, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warning); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 550, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __pyx_t_1 = NULL;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+          __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
+          if (likely(__pyx_t_1)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+            __Pyx_INCREF(__pyx_t_1);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_5, function);
+          }
+        }
+        __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_1, __pyx_kp_u_Query_not_finished_Maybe_some_en) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u_Query_not_finished_Maybe_some_en);
+        __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 550, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+        /* "viur/datastore/transport.pyx":551
+ * 			if toPyStr(element.at_key("moreResults").get_string()) == "NOT_FINISHED":
+ * 				logging.warning("Query not finished. Maybe some entries are missing.")
+ * 				logging.warning("Queried %s with filter %s and orders %s. - Please create a matching index" % (             # <<<<<<<<<<<<<<
+ * 					queryDefinition.kind, queryDefinition.filters, queryDefinition.orders))
+ * 			else:
+ */
+        __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logging); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 551, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_warning); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 551, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __pyx_t_5 = PyTuple_New(7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 551, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_7 = 0;
+        __pyx_t_21 = 127;
+        __Pyx_INCREF(__pyx_kp_u_Queried);
+        __pyx_t_7 += 8;
+        __Pyx_GIVEREF(__pyx_kp_u_Queried);
+        PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_kp_u_Queried);
+
+        /* "viur/datastore/transport.pyx":552
+ * 				logging.warning("Query not finished. Maybe some entries are missing.")
+ * 				logging.warning("Queried %s with filter %s and orders %s. - Please create a matching index" % (
+ * 					queryDefinition.kind, queryDefinition.filters, queryDefinition.orders))             # <<<<<<<<<<<<<<
+ * 			else:
+ * 				break
+ */
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_kind); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 552, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_10 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_t_3), __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 552, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __pyx_t_21 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) > __pyx_t_21) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) : __pyx_t_21;
+        __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_10);
+        __Pyx_GIVEREF(__pyx_t_10);
+        PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_10);
+        __pyx_t_10 = 0;
+        __Pyx_INCREF(__pyx_kp_u_with_filter);
+        __pyx_t_7 += 13;
+        __Pyx_GIVEREF(__pyx_kp_u_with_filter);
+        PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_kp_u_with_filter);
+        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_filters); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 552, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __pyx_t_3 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_t_10), __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 552, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __pyx_t_21 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_21) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_21;
+        __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
+        __Pyx_GIVEREF(__pyx_t_3);
+        PyTuple_SET_ITEM(__pyx_t_5, 3, __pyx_t_3);
+        __pyx_t_3 = 0;
+        __Pyx_INCREF(__pyx_kp_u_and_orders);
+        __pyx_t_7 += 12;
+        __Pyx_GIVEREF(__pyx_kp_u_and_orders);
+        PyTuple_SET_ITEM(__pyx_t_5, 4, __pyx_kp_u_and_orders);
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_orders); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 552, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_10 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_t_3), __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 552, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __pyx_t_21 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) > __pyx_t_21) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) : __pyx_t_21;
+        __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_10);
+        __Pyx_GIVEREF(__pyx_t_10);
+        PyTuple_SET_ITEM(__pyx_t_5, 5, __pyx_t_10);
+        __pyx_t_10 = 0;
+        __Pyx_INCREF(__pyx_kp_u_Please_create_a_matching_index);
+        __pyx_t_7 += 34;
+        __Pyx_GIVEREF(__pyx_kp_u_Please_create_a_matching_index);
+        PyTuple_SET_ITEM(__pyx_t_5, 6, __pyx_kp_u_Please_create_a_matching_index);
+
+        /* "viur/datastore/transport.pyx":551
+ * 			if toPyStr(element.at_key("moreResults").get_string()) == "NOT_FINISHED":
+ * 				logging.warning("Query not finished. Maybe some entries are missing.")
+ * 				logging.warning("Queried %s with filter %s and orders %s. - Please create a matching index" % (             # <<<<<<<<<<<<<<
+ * 					queryDefinition.kind, queryDefinition.filters, queryDefinition.orders))
+ * 			else:
+ */
+        __pyx_t_10 = __Pyx_PyUnicode_Join(__pyx_t_5, 7, __pyx_t_7, __pyx_t_21); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 551, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __pyx_t_5 = NULL;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+          __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+          if (likely(__pyx_t_5)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+            __Pyx_INCREF(__pyx_t_5);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_1, function);
+          }
+        }
+        __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_10);
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 551, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+        /* "viur/datastore/transport.pyx":549
+ * 			res.extend(toEntityStructure(element.at_key("entityResults"), isInitial=False))
+ * 		else:  # No results received
+ * 			if toPyStr(element.at_key("moreResults").get_string()) == "NOT_FINISHED":             # <<<<<<<<<<<<<<
+ * 				logging.warning("Query not finished. Maybe some entries are missing.")
+ * 				logging.warning("Queried %s with filter %s and orders %s. - Please create a matching index" % (
+ */
+        goto __pyx_L40;
+      }
+
+      /* "viur/datastore/transport.pyx":554
+ * 					queryDefinition.kind, queryDefinition.filters, queryDefinition.orders))
+ * 			else:
+ * 				break             # <<<<<<<<<<<<<<
  * 		if toPyStr(element.at_key("moreResults").get_string()) == "NO_MORE_RESULTS":
  * 			internalStartCursor = None
  */
-    /*else*/ {
-      goto __pyx_L5_break;
+      /*else*/ {
+        goto __pyx_L5_break;
+      }
+      __pyx_L40:;
     }
     __pyx_L39:;
 
-    /* "viur/datastore/transport.pyx":550
- * 		else:  # No results received
- * 			break
+    /* "viur/datastore/transport.pyx":555
+ * 			else:
+ * 				break
  * 		if toPyStr(element.at_key("moreResults").get_string()) == "NO_MORE_RESULTS":             # <<<<<<<<<<<<<<
  * 			internalStartCursor = None
  * 		else:
  */
     try {
       __pyx_t_18 = __pyx_v_element.at_key(((char const *)"moreResults"));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 550, __pyx_L1_error)
+      __PYX_ERR(0, 555, __pyx_L1_error)
     }
     try {
       __pyx_t_20 = __pyx_t_18.get_string();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 550, __pyx_L1_error)
+      __PYX_ERR(0, 555, __pyx_L1_error)
     }
-    __pyx_t_2 = __pyx_f_4viur_9datastore_9transport_toPyStr(__pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 550, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_4viur_9datastore_9transport_toPyStr(__pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 555, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_12 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_NO_MORE_RESULTS, Py_EQ)); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 550, __pyx_L1_error)
+    __pyx_t_12 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_NO_MORE_RESULTS, Py_EQ)); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 555, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (__pyx_t_12) {
 
-      /* "viur/datastore/transport.pyx":551
- * 			break
+      /* "viur/datastore/transport.pyx":556
+ * 				break
  * 		if toPyStr(element.at_key("moreResults").get_string()) == "NO_MORE_RESULTS":
  * 			internalStartCursor = None             # <<<<<<<<<<<<<<
  * 		else:
  * 			internalStartCursor = toPyStr(element.at_key("endCursor").get_string())
  */
       __Pyx_INCREF(Py_None);
       __Pyx_DECREF_SET(__pyx_v_internalStartCursor, Py_None);
 
-      /* "viur/datastore/transport.pyx":550
- * 		else:  # No results received
- * 			break
+      /* "viur/datastore/transport.pyx":555
+ * 			else:
+ * 				break
  * 		if toPyStr(element.at_key("moreResults").get_string()) == "NO_MORE_RESULTS":             # <<<<<<<<<<<<<<
  * 			internalStartCursor = None
  * 		else:
  */
-      goto __pyx_L40;
+      goto __pyx_L41;
     }
 
-    /* "viur/datastore/transport.pyx":553
+    /* "viur/datastore/transport.pyx":558
  * 			internalStartCursor = None
  * 		else:
  * 			internalStartCursor = toPyStr(element.at_key("endCursor").get_string())             # <<<<<<<<<<<<<<
  * 		if toPyStr(element.at_key("moreResults").get_string()) != "NOT_FINISHED" or len(res) == limit:
  * 			break
  */
     /*else*/ {
       try {
         __pyx_t_18 = __pyx_v_element.at_key(((char const *)"endCursor"));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 553, __pyx_L1_error)
+        __PYX_ERR(0, 558, __pyx_L1_error)
       }
       try {
         __pyx_t_20 = __pyx_t_18.get_string();
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 553, __pyx_L1_error)
+        __PYX_ERR(0, 558, __pyx_L1_error)
       }
-      __pyx_t_2 = __pyx_f_4viur_9datastore_9transport_toPyStr(__pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 553, __pyx_L1_error)
+      __pyx_t_2 = __pyx_f_4viur_9datastore_9transport_toPyStr(__pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 558, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF_SET(__pyx_v_internalStartCursor, __pyx_t_2);
       __pyx_t_2 = 0;
     }
-    __pyx_L40:;
+    __pyx_L41:;
 
-    /* "viur/datastore/transport.pyx":554
+    /* "viur/datastore/transport.pyx":559
  * 		else:
  * 			internalStartCursor = toPyStr(element.at_key("endCursor").get_string())
  * 		if toPyStr(element.at_key("moreResults").get_string()) != "NOT_FINISHED" or len(res) == limit:             # <<<<<<<<<<<<<<
  * 			break
  * 	queryDefinition.currentCursor = internalStartCursor
  */
     try {
       __pyx_t_18 = __pyx_v_element.at_key(((char const *)"moreResults"));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 554, __pyx_L1_error)
+      __PYX_ERR(0, 559, __pyx_L1_error)
     }
     try {
       __pyx_t_20 = __pyx_t_18.get_string();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 554, __pyx_L1_error)
+      __PYX_ERR(0, 559, __pyx_L1_error)
     }
-    __pyx_t_2 = __pyx_f_4viur_9datastore_9transport_toPyStr(__pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 554, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_4viur_9datastore_9transport_toPyStr(__pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 559, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_NOT_FINISHED, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 554, __pyx_L1_error)
+    __pyx_t_4 = (__Pyx_PyUnicode_Equals(__pyx_t_2, __pyx_n_u_NOT_FINISHED, Py_NE)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 559, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (!__pyx_t_4) {
     } else {
       __pyx_t_12 = __pyx_t_4;
-      goto __pyx_L42_bool_binop_done;
+      goto __pyx_L43_bool_binop_done;
     }
-    __pyx_t_7 = PyList_GET_SIZE(__pyx_v_res); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 554, __pyx_L1_error)
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 554, __pyx_L1_error)
+    __pyx_t_7 = PyList_GET_SIZE(__pyx_v_res); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 559, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 559, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_v_limit, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 554, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_v_limit, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 559, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 554, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 559, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_12 = __pyx_t_4;
-    __pyx_L42_bool_binop_done:;
+    __pyx_L43_bool_binop_done:;
     if (__pyx_t_12) {
 
-      /* "viur/datastore/transport.pyx":555
+      /* "viur/datastore/transport.pyx":560
  * 			internalStartCursor = toPyStr(element.at_key("endCursor").get_string())
  * 		if toPyStr(element.at_key("moreResults").get_string()) != "NOT_FINISHED" or len(res) == limit:
  * 			break             # <<<<<<<<<<<<<<
  * 	queryDefinition.currentCursor = internalStartCursor
  * 	if conf["traceQueries"]:
  */
       goto __pyx_L5_break;
 
-      /* "viur/datastore/transport.pyx":554
+      /* "viur/datastore/transport.pyx":559
  * 		else:
  * 			internalStartCursor = toPyStr(element.at_key("endCursor").get_string())
  * 		if toPyStr(element.at_key("moreResults").get_string()) != "NOT_FINISHED" or len(res) == limit:             # <<<<<<<<<<<<<<
  * 			break
  * 	queryDefinition.currentCursor = internalStartCursor
  */
     }
   }
   __pyx_L5_break:;
 
-  /* "viur/datastore/transport.pyx":556
+  /* "viur/datastore/transport.pyx":561
  * 		if toPyStr(element.at_key("moreResults").get_string()) != "NOT_FINISHED" or len(res) == limit:
  * 			break
  * 	queryDefinition.currentCursor = internalStartCursor             # <<<<<<<<<<<<<<
  * 	if conf["traceQueries"]:
  * 		orders = queryDefinition.orders
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_currentCursor, __pyx_v_internalStartCursor) < 0) __PYX_ERR(0, 556, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_currentCursor, __pyx_v_internalStartCursor) < 0) __PYX_ERR(0, 561, __pyx_L1_error)
 
-  /* "viur/datastore/transport.pyx":557
+  /* "viur/datastore/transport.pyx":562
  * 			break
  * 	queryDefinition.currentCursor = internalStartCursor
  * 	if conf["traceQueries"]:             # <<<<<<<<<<<<<<
  * 		orders = queryDefinition.orders
  * 		filters = queryDefinition.filters
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_conf); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 557, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_conf); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_traceQueries); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 557, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_traceQueries); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 557, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 562, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_12) {
 
-    /* "viur/datastore/transport.pyx":558
+    /* "viur/datastore/transport.pyx":563
  * 	queryDefinition.currentCursor = internalStartCursor
  * 	if conf["traceQueries"]:
  * 		orders = queryDefinition.orders             # <<<<<<<<<<<<<<
  * 		filters = queryDefinition.filters
  * 		distinctOn = " distinct on %s" % str(queryDefinition.distinct) if queryDefinition.distinct else ""
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_orders); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 558, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_orders); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 563, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_orders = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "viur/datastore/transport.pyx":559
+    /* "viur/datastore/transport.pyx":564
  * 	if conf["traceQueries"]:
  * 		orders = queryDefinition.orders
  * 		filters = queryDefinition.filters             # <<<<<<<<<<<<<<
  * 		distinctOn = " distinct on %s" % str(queryDefinition.distinct) if queryDefinition.distinct else ""
  * 		logging.debug("Queried %s with filter %s and orders %s%s. Returned %s results" % (
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_filters); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 559, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_filters); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 564, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_filters = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "viur/datastore/transport.pyx":560
+    /* "viur/datastore/transport.pyx":565
  * 		orders = queryDefinition.orders
  * 		filters = queryDefinition.filters
  * 		distinctOn = " distinct on %s" % str(queryDefinition.distinct) if queryDefinition.distinct else ""             # <<<<<<<<<<<<<<
  * 		logging.debug("Queried %s with filter %s and orders %s%s. Returned %s results" % (
  * 				queryDefinition.kind, filters, orders, distinctOn, len(res)))
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_distinct); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 560, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_distinct); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 565, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 560, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 565, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_12) {
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_distinct); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 560, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_distinct); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 565, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 560, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_10 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 565, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = PyUnicode_Format(__pyx_kp_u_distinct_on_s, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 560, __pyx_L1_error)
+      __pyx_t_1 = PyUnicode_Format(__pyx_kp_u_distinct_on_s, __pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 565, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_2 = __pyx_t_1;
       __pyx_t_1 = 0;
     } else {
       __Pyx_INCREF(__pyx_kp_u__12);
       __pyx_t_2 = __pyx_kp_u__12;
     }
     __pyx_v_distinctOn = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "viur/datastore/transport.pyx":561
+    /* "viur/datastore/transport.pyx":566
  * 		filters = queryDefinition.filters
  * 		distinctOn = " distinct on %s" % str(queryDefinition.distinct) if queryDefinition.distinct else ""
  * 		logging.debug("Queried %s with filter %s and orders %s%s. Returned %s results" % (             # <<<<<<<<<<<<<<
  * 				queryDefinition.kind, filters, orders, distinctOn, len(res)))
  * 	if flipResults:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logging); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 561, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logging); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 566, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_debug); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 561, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_debug); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 566, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyTuple_New(10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 561, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 566, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_7 = 0;
     __pyx_t_21 = 127;
     __Pyx_INCREF(__pyx_kp_u_Queried);
     __pyx_t_7 += 8;
     __Pyx_GIVEREF(__pyx_kp_u_Queried);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Queried);
 
-    /* "viur/datastore/transport.pyx":562
+    /* "viur/datastore/transport.pyx":567
  * 		distinctOn = " distinct on %s" % str(queryDefinition.distinct) if queryDefinition.distinct else ""
  * 		logging.debug("Queried %s with filter %s and orders %s%s. Returned %s results" % (
  * 				queryDefinition.kind, filters, orders, distinctOn, len(res)))             # <<<<<<<<<<<<<<
  * 	if flipResults:
  * 		return res[::-1]
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_kind); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 562, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_kind); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 567, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_3 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_t_5), __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 567, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_10 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_t_3), __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 562, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_21 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) > __pyx_t_21) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) : __pyx_t_21;
-    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_10);
-    __Pyx_GIVEREF(__pyx_t_10);
-    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_10);
-    __pyx_t_10 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_21 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_21) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_21;
+    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
+    __pyx_t_3 = 0;
     __Pyx_INCREF(__pyx_kp_u_with_filter);
     __pyx_t_7 += 13;
     __Pyx_GIVEREF(__pyx_kp_u_with_filter);
     PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_with_filter);
-    __pyx_t_10 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_filters), __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 562, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_21 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) > __pyx_t_21) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) : __pyx_t_21;
-    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_10);
-    __Pyx_GIVEREF(__pyx_t_10);
-    PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_10);
-    __pyx_t_10 = 0;
+    __pyx_t_3 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_filters), __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 567, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_21 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_21) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_21;
+    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_3);
+    __pyx_t_3 = 0;
     __Pyx_INCREF(__pyx_kp_u_and_orders);
     __pyx_t_7 += 12;
     __Pyx_GIVEREF(__pyx_kp_u_and_orders);
     PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u_and_orders);
-    __pyx_t_10 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_orders), __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 562, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_21 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) > __pyx_t_21) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) : __pyx_t_21;
-    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_10);
-    __Pyx_GIVEREF(__pyx_t_10);
-    PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_t_10);
-    __pyx_t_10 = 0;
-    __pyx_t_10 = __Pyx_PyUnicode_Unicode(__pyx_v_distinctOn); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 562, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_21 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) > __pyx_t_21) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) : __pyx_t_21;
-    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_10);
-    __Pyx_GIVEREF(__pyx_t_10);
-    PyTuple_SET_ITEM(__pyx_t_1, 6, __pyx_t_10);
-    __pyx_t_10 = 0;
+    __pyx_t_3 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Unicode(__pyx_v_orders), __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 567, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_21 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_21) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_21;
+    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_t_3);
+    __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyUnicode_Unicode(__pyx_v_distinctOn); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 567, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_21 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) > __pyx_t_21) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_3) : __pyx_t_21;
+    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_1, 6, __pyx_t_3);
+    __pyx_t_3 = 0;
     __Pyx_INCREF(__pyx_kp_u_Returned);
     __pyx_t_7 += 11;
     __Pyx_GIVEREF(__pyx_kp_u_Returned);
     PyTuple_SET_ITEM(__pyx_t_1, 7, __pyx_kp_u_Returned);
-    __pyx_t_6 = PyList_GET_SIZE(__pyx_v_res); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 562, __pyx_L1_error)
-    __pyx_t_10 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_6, 0, ' ', 'd'); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 562, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
-    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_10);
-    __Pyx_GIVEREF(__pyx_t_10);
-    PyTuple_SET_ITEM(__pyx_t_1, 8, __pyx_t_10);
-    __pyx_t_10 = 0;
+    __pyx_t_6 = PyList_GET_SIZE(__pyx_v_res); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 567, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_6, 0, ' ', 'd'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 567, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_1, 8, __pyx_t_3);
+    __pyx_t_3 = 0;
     __Pyx_INCREF(__pyx_kp_u_results);
     __pyx_t_7 += 8;
     __Pyx_GIVEREF(__pyx_kp_u_results);
     PyTuple_SET_ITEM(__pyx_t_1, 9, __pyx_kp_u_results);
 
-    /* "viur/datastore/transport.pyx":561
+    /* "viur/datastore/transport.pyx":566
  * 		filters = queryDefinition.filters
  * 		distinctOn = " distinct on %s" % str(queryDefinition.distinct) if queryDefinition.distinct else ""
  * 		logging.debug("Queried %s with filter %s and orders %s%s. Returned %s results" % (             # <<<<<<<<<<<<<<
  * 				queryDefinition.kind, filters, orders, distinctOn, len(res)))
  * 	if flipResults:
  */
-    __pyx_t_10 = __Pyx_PyUnicode_Join(__pyx_t_1, 10, __pyx_t_7, __pyx_t_21); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 561, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_3 = __Pyx_PyUnicode_Join(__pyx_t_1, 10, __pyx_t_7, __pyx_t_21); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 566, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_10);
       if (likely(__pyx_t_1)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __Pyx_DECREF_SET(__pyx_t_10, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_1, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_10);
+    __pyx_t_2 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_1, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 566, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "viur/datastore/transport.pyx":557
+    /* "viur/datastore/transport.pyx":562
  * 			break
  * 	queryDefinition.currentCursor = internalStartCursor
  * 	if conf["traceQueries"]:             # <<<<<<<<<<<<<<
  * 		orders = queryDefinition.orders
  * 		filters = queryDefinition.filters
  */
   }
 
-  /* "viur/datastore/transport.pyx":563
+  /* "viur/datastore/transport.pyx":568
  * 		logging.debug("Queried %s with filter %s and orders %s%s. Returned %s results" % (
  * 				queryDefinition.kind, filters, orders, distinctOn, len(res)))
  * 	if flipResults:             # <<<<<<<<<<<<<<
  * 		return res[::-1]
  * 	return res
  */
-  __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_v_flipResults); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_IsTrue(__pyx_v_flipResults); if (unlikely(__pyx_t_12 < 0)) __PYX_ERR(0, 568, __pyx_L1_error)
   if (__pyx_t_12) {
 
-    /* "viur/datastore/transport.pyx":564
+    /* "viur/datastore/transport.pyx":569
  * 				queryDefinition.kind, filters, orders, distinctOn, len(res)))
  * 	if flipResults:
  * 		return res[::-1]             # <<<<<<<<<<<<<<
  * 	return res
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_res, __pyx_slice__13); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 564, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_res, __pyx_slice__13); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 569, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "viur/datastore/transport.pyx":563
+    /* "viur/datastore/transport.pyx":568
  * 		logging.debug("Queried %s with filter %s and orders %s%s. Returned %s results" % (
  * 				queryDefinition.kind, filters, orders, distinctOn, len(res)))
  * 	if flipResults:             # <<<<<<<<<<<<<<
  * 		return res[::-1]
  * 	return res
  */
   }
 
-  /* "viur/datastore/transport.pyx":565
+  /* "viur/datastore/transport.pyx":570
  * 	if flipResults:
  * 		return res[::-1]
  * 	return res             # <<<<<<<<<<<<<<
  * 
  * def Get(keys: Union[Key, List[Key]]) -> Union[None, Entity, List[Entity]]:
  */
   __Pyx_XDECREF(__pyx_r);
@@ -8728,15 +8898,15 @@
   __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_sortOrder);
   __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_distinctKey);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viur/datastore/transport.pyx":567
+/* "viur/datastore/transport.pyx":572
  * 	return res
  * 
  * def Get(keys: Union[Key, List[Key]]) -> Union[None, Entity, List[Entity]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Fetches the entities determined by keys from the datastore. Returns or inserts None if a key is not found.
  */
 
@@ -8788,274 +8958,274 @@
   struct __pyx_opt_args_4viur_9datastore_9transport_toEntityStructure __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Get", 0);
   __Pyx_INCREF(__pyx_v_keys);
 
-  /* "viur/datastore/transport.pyx":573
+  /* "viur/datastore/transport.pyx":578
  * 		:return: The entity or None for the given key, a list of Entities/None if a list has been supplied
  * 	"""
  * 	cdef simdjsonParser parser = simdjsonParser()             # <<<<<<<<<<<<<<
  * 	cdef Py_ssize_t pysize
  * 	cdef char * data_ptr
  */
   __pyx_v_parser = simdjson::dom::parser();
 
-  /* "viur/datastore/transport.pyx":577
+  /* "viur/datastore/transport.pyx":582
  * 	cdef char * data_ptr
  * 	cdef simdjsonElement element
  * 	isMulti = True             # <<<<<<<<<<<<<<
  * 	if isinstance(keys, Key):
  * 		keys = [keys]
  */
   __pyx_v_isMulti = 1;
 
-  /* "viur/datastore/transport.pyx":578
+  /* "viur/datastore/transport.pyx":583
  * 	cdef simdjsonElement element
  * 	isMulti = True
  * 	if isinstance(keys, Key):             # <<<<<<<<<<<<<<
  * 		keys = [keys]
  * 		isMulti = False
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 578, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_keys, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 578, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_keys, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "viur/datastore/transport.pyx":579
+    /* "viur/datastore/transport.pyx":584
  * 	isMulti = True
  * 	if isinstance(keys, Key):
  * 		keys = [keys]             # <<<<<<<<<<<<<<
  * 		isMulti = False
  * 	accessLog = currentDbAccessLog.get()
  */
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 579, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 584, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_keys);
     __Pyx_GIVEREF(__pyx_v_keys);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_v_keys);
     __Pyx_DECREF_SET(__pyx_v_keys, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "viur/datastore/transport.pyx":580
+    /* "viur/datastore/transport.pyx":585
  * 	if isinstance(keys, Key):
  * 		keys = [keys]
  * 		isMulti = False             # <<<<<<<<<<<<<<
  * 	accessLog = currentDbAccessLog.get()
  * 	if isinstance(accessLog, set):
  */
     __pyx_v_isMulti = 0;
 
-    /* "viur/datastore/transport.pyx":578
+    /* "viur/datastore/transport.pyx":583
  * 	cdef simdjsonElement element
  * 	isMulti = True
  * 	if isinstance(keys, Key):             # <<<<<<<<<<<<<<
  * 		keys = [keys]
  * 		isMulti = False
  */
   }
 
-  /* "viur/datastore/transport.pyx":581
+  /* "viur/datastore/transport.pyx":586
  * 		keys = [keys]
  * 		isMulti = False
  * 	accessLog = currentDbAccessLog.get()             # <<<<<<<<<<<<<<
  * 	if isinstance(accessLog, set):
  * 		accessLog.update(set(keys))
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_currentDbAccessLog); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 581, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_currentDbAccessLog); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 581, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 581, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_accessLog = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "viur/datastore/transport.pyx":582
+  /* "viur/datastore/transport.pyx":587
  * 		isMulti = False
  * 	accessLog = currentDbAccessLog.get()
  * 	if isinstance(accessLog, set):             # <<<<<<<<<<<<<<
  * 		accessLog.update(set(keys))
  * 	keyList = [
  */
   __pyx_t_3 = PySet_Check(__pyx_v_accessLog); 
   __pyx_t_2 = (__pyx_t_3 != 0);
   if (__pyx_t_2) {
 
-    /* "viur/datastore/transport.pyx":583
+    /* "viur/datastore/transport.pyx":588
  * 	accessLog = currentDbAccessLog.get()
  * 	if isinstance(accessLog, set):
  * 		accessLog.update(set(keys))             # <<<<<<<<<<<<<<
  * 	keyList = [
  * 		{
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_accessLog, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 583, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_accessLog, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 588, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = PySet_New(__pyx_v_keys); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 583, __pyx_L1_error)
+    __pyx_t_4 = PySet_New(__pyx_v_keys); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 588, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 583, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "viur/datastore/transport.pyx":582
+    /* "viur/datastore/transport.pyx":587
  * 		isMulti = False
  * 	accessLog = currentDbAccessLog.get()
  * 	if isinstance(accessLog, set):             # <<<<<<<<<<<<<<
  * 		accessLog.update(set(keys))
  * 	keyList = [
  */
   }
 
-  /* "viur/datastore/transport.pyx":584
+  /* "viur/datastore/transport.pyx":589
  * 	if isinstance(accessLog, set):
  * 		accessLog.update(set(keys))
  * 	keyList = [             # <<<<<<<<<<<<<<
  * 		{
  * 			"partitionId": {
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 584, __pyx_L7_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 589, __pyx_L7_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "viur/datastore/transport.pyx":591
+    /* "viur/datastore/transport.pyx":596
  * 			"path": keyToPath(x)
  * 		}
  * 		for x in keys]             # <<<<<<<<<<<<<<
  * 
  * 	currentTxn = currentTransaction.get()
  */
     if (likely(PyList_CheckExact(__pyx_v_keys)) || PyTuple_CheckExact(__pyx_v_keys)) {
       __pyx_t_5 = __pyx_v_keys; __Pyx_INCREF(__pyx_t_5); __pyx_t_7 = 0;
       __pyx_t_8 = NULL;
     } else {
-      __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_keys); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 591, __pyx_L7_error)
+      __pyx_t_7 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_keys); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 596, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_8 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 591, __pyx_L7_error)
+      __pyx_t_8 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 596, __pyx_L7_error)
     }
     for (;;) {
       if (likely(!__pyx_t_8)) {
         if (likely(PyList_CheckExact(__pyx_t_5))) {
           if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_5)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 591, __pyx_L7_error)
+          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 596, __pyx_L7_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 591, __pyx_L7_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 596, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         } else {
           if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 591, __pyx_L7_error)
+          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 596, __pyx_L7_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 591, __pyx_L7_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 596, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         }
       } else {
         __pyx_t_4 = __pyx_t_8(__pyx_t_5);
         if (unlikely(!__pyx_t_4)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 591, __pyx_L7_error)
+            else __PYX_ERR(0, 596, __pyx_L7_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_4);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr4__pyx_v_x, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "viur/datastore/transport.pyx":586
+      /* "viur/datastore/transport.pyx":591
  * 	keyList = [
  * 		{
  * 			"partitionId": {             # <<<<<<<<<<<<<<
  * 				"project_id": projectID,
  * 			},
  */
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 586, __pyx_L7_error)
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 591, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_4);
 
-      /* "viur/datastore/transport.pyx":587
+      /* "viur/datastore/transport.pyx":592
  * 		{
  * 			"partitionId": {
  * 				"project_id": projectID,             # <<<<<<<<<<<<<<
  * 			},
  * 			"path": keyToPath(x)
  */
-      __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 587, __pyx_L7_error)
+      __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 592, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_projectID); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 587, __pyx_L7_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_projectID); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 592, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_9);
-      if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_project_id, __pyx_t_9) < 0) __PYX_ERR(0, 587, __pyx_L7_error)
+      if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_project_id, __pyx_t_9) < 0) __PYX_ERR(0, 592, __pyx_L7_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_partitionId, __pyx_t_6) < 0) __PYX_ERR(0, 586, __pyx_L7_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_partitionId, __pyx_t_6) < 0) __PYX_ERR(0, 591, __pyx_L7_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "viur/datastore/transport.pyx":589
+      /* "viur/datastore/transport.pyx":594
  * 				"project_id": projectID,
  * 			},
  * 			"path": keyToPath(x)             # <<<<<<<<<<<<<<
  * 		}
  * 		for x in keys]
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_keyToPath); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 589, __pyx_L7_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_keyToPath); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 594, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
         }
       }
       __pyx_t_6 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_10, __pyx_8genexpr4__pyx_v_x) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_8genexpr4__pyx_v_x);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 589, __pyx_L7_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 594, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_path, __pyx_t_6) < 0) __PYX_ERR(0, 586, __pyx_L7_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_path, __pyx_t_6) < 0) __PYX_ERR(0, 591, __pyx_L7_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 584, __pyx_L7_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 589, __pyx_L7_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "viur/datastore/transport.pyx":591
+      /* "viur/datastore/transport.pyx":596
  * 			"path": keyToPath(x)
  * 		}
  * 		for x in keys]             # <<<<<<<<<<<<<<
  * 
  * 	currentTxn = currentTransaction.get()
  */
     }
@@ -9066,493 +9236,493 @@
     __Pyx_XDECREF(__pyx_8genexpr4__pyx_v_x); __pyx_8genexpr4__pyx_v_x = 0;
     goto __pyx_L1_error;
     __pyx_L10_exit_scope:;
   } /* exit inner scope */
   __pyx_v_keyList = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "viur/datastore/transport.pyx":593
+  /* "viur/datastore/transport.pyx":598
  * 		for x in keys]
  * 
  * 	currentTxn = currentTransaction.get()             # <<<<<<<<<<<<<<
  * 	if currentTxn:
  * 		readOptions = {"transaction": currentTxn["key"]}
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 593, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_get); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 593, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_get); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 593, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_currentTxn = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "viur/datastore/transport.pyx":594
+  /* "viur/datastore/transport.pyx":599
  * 
  * 	currentTxn = currentTransaction.get()
  * 	if currentTxn:             # <<<<<<<<<<<<<<
  * 		readOptions = {"transaction": currentTxn["key"]}
  * 	else:
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_currentTxn); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 594, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_currentTxn); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 599, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "viur/datastore/transport.pyx":595
+    /* "viur/datastore/transport.pyx":600
  * 	currentTxn = currentTransaction.get()
  * 	if currentTxn:
  * 		readOptions = {"transaction": currentTxn["key"]}             # <<<<<<<<<<<<<<
  * 	else:
  * 		readOptions = {"readConsistency": "STRONG"}
  */
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 595, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_currentTxn, __pyx_n_u_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 595, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Dict_GetItem(__pyx_v_currentTxn, __pyx_n_u_key); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 600, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_transaction, __pyx_t_4) < 0) __PYX_ERR(0, 595, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_transaction, __pyx_t_4) < 0) __PYX_ERR(0, 600, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_readOptions = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "viur/datastore/transport.pyx":594
+    /* "viur/datastore/transport.pyx":599
  * 
  * 	currentTxn = currentTransaction.get()
  * 	if currentTxn:             # <<<<<<<<<<<<<<
  * 		readOptions = {"transaction": currentTxn["key"]}
  * 	else:
  */
     goto __pyx_L11;
   }
 
-  /* "viur/datastore/transport.pyx":597
+  /* "viur/datastore/transport.pyx":602
  * 		readOptions = {"transaction": currentTxn["key"]}
  * 	else:
  * 		readOptions = {"readConsistency": "STRONG"}             # <<<<<<<<<<<<<<
  * 	res = {}
  * 	while keyList:
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 597, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 602, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_readConsistency, __pyx_n_u_STRONG) < 0) __PYX_ERR(0, 597, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_readConsistency, __pyx_n_u_STRONG) < 0) __PYX_ERR(0, 602, __pyx_L1_error)
     __pyx_v_readOptions = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
   }
   __pyx_L11:;
 
-  /* "viur/datastore/transport.pyx":598
+  /* "viur/datastore/transport.pyx":603
  * 	else:
  * 		readOptions = {"readConsistency": "STRONG"}
  * 	res = {}             # <<<<<<<<<<<<<<
  * 	while keyList:
  * 		requestedKeys = keyList[:300]
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_res = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "viur/datastore/transport.pyx":599
+  /* "viur/datastore/transport.pyx":604
  * 		readOptions = {"readConsistency": "STRONG"}
  * 	res = {}
  * 	while keyList:             # <<<<<<<<<<<<<<
  * 		requestedKeys = keyList[:300]
  * 		postData = {
  */
   while (1) {
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_keyList); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 599, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_keyList); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 604, __pyx_L1_error)
     if (!__pyx_t_2) break;
 
-    /* "viur/datastore/transport.pyx":600
+    /* "viur/datastore/transport.pyx":605
  * 	res = {}
  * 	while keyList:
  * 		requestedKeys = keyList[:300]             # <<<<<<<<<<<<<<
  * 		postData = {
  * 			"readOptions": readOptions,
  */
-    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_keyList, 0, 0x12C, NULL, NULL, &__pyx_slice__14, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_keyList, 0, 0x12C, NULL, NULL, &__pyx_slice__14, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_requestedKeys, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "viur/datastore/transport.pyx":602
+    /* "viur/datastore/transport.pyx":607
  * 		requestedKeys = keyList[:300]
  * 		postData = {
  * 			"readOptions": readOptions,             # <<<<<<<<<<<<<<
  * 			"keys": requestedKeys,
  * 		}
  */
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 602, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_readOptions, __pyx_v_readOptions) < 0) __PYX_ERR(0, 602, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_readOptions, __pyx_v_readOptions) < 0) __PYX_ERR(0, 607, __pyx_L1_error)
 
-    /* "viur/datastore/transport.pyx":603
+    /* "viur/datastore/transport.pyx":608
  * 		postData = {
  * 			"readOptions": readOptions,
  * 			"keys": requestedKeys,             # <<<<<<<<<<<<<<
  * 		}
  * 		req = authenticatedRequest(
  */
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_keys, __pyx_v_requestedKeys) < 0) __PYX_ERR(0, 602, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_keys, __pyx_v_requestedKeys) < 0) __PYX_ERR(0, 607, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_postData, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "viur/datastore/transport.pyx":605
+    /* "viur/datastore/transport.pyx":610
  * 			"keys": requestedKeys,
  * 		}
  * 		req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 			url="https://datastore.googleapis.com/v1/projects/%s:lookup" % projectID,
  * 			data=json.dumps(postData).encode("UTF-8"),
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "viur/datastore/transport.pyx":606
+    /* "viur/datastore/transport.pyx":611
  * 		}
  * 		req = authenticatedRequest(
  * 			url="https://datastore.googleapis.com/v1/projects/%s:lookup" % projectID,             # <<<<<<<<<<<<<<
  * 			data=json.dumps(postData).encode("UTF-8"),
  * 		)
  */
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 606, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 611, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_projectID); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 606, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_projectID); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 611, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_2, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 606, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_2, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 611, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_url, __pyx_t_6) < 0) __PYX_ERR(0, 606, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_url, __pyx_t_6) < 0) __PYX_ERR(0, 611, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "viur/datastore/transport.pyx":607
+    /* "viur/datastore/transport.pyx":612
  * 		req = authenticatedRequest(
  * 			url="https://datastore.googleapis.com/v1/projects/%s:lookup" % projectID,
  * 			data=json.dumps(postData).encode("UTF-8"),             # <<<<<<<<<<<<<<
  * 		)
  * 		assert req.status_code == 200
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_json); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 607, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_json); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 612, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_dumps); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 607, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_dumps); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 612, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_10, function);
       }
     }
     __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_9, __pyx_v_postData) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_v_postData);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 607, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 612, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_encode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 607, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_encode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 612, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_10);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_10, function);
       }
     }
     __pyx_t_6 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_5, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_kp_u_UTF_8);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 607, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 612, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_data, __pyx_t_6) < 0) __PYX_ERR(0, 606, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_data, __pyx_t_6) < 0) __PYX_ERR(0, 611, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "viur/datastore/transport.pyx":605
+    /* "viur/datastore/transport.pyx":610
  * 			"keys": requestedKeys,
  * 		}
  * 		req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 			url="https://datastore.googleapis.com/v1/projects/%s:lookup" % projectID,
  * 			data=json.dumps(postData).encode("UTF-8"),
  */
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 605, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 610, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF_SET(__pyx_v_req, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "viur/datastore/transport.pyx":609
+    /* "viur/datastore/transport.pyx":614
  * 			data=json.dumps(postData).encode("UTF-8"),
  * 		)
  * 		assert req.status_code == 200             # <<<<<<<<<<<<<<
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
     if (unlikely(!Py_OptimizeFlag)) {
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_status_code); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 609, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_status_code); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 614, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_t_6, __pyx_int_200, 0xC8, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 609, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_t_6, __pyx_int_200, 0xC8, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 614, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 609, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 614, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (unlikely(!__pyx_t_2)) {
         PyErr_SetNone(PyExc_AssertionError);
-        __PYX_ERR(0, 609, __pyx_L1_error)
+        __PYX_ERR(0, 614, __pyx_L1_error)
       }
     }
     #endif
 
-    /* "viur/datastore/transport.pyx":610
+    /* "viur/datastore/transport.pyx":615
  * 		)
  * 		assert req.status_code == 200
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1             # <<<<<<<<<<<<<<
  * 		element = parser.parse(data_ptr, pysize, 1)
  * 		if (element.at_pointer("/found").error() == SUCCESS):
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
     if (unlikely(!Py_OptimizeFlag)) {
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 610, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 615, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_11 = PyBytes_AsStringAndSize(__pyx_t_4, (&__pyx_v_data_ptr), (&__pyx_v_pysize)); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 610, __pyx_L1_error)
+      __pyx_t_11 = PyBytes_AsStringAndSize(__pyx_t_4, (&__pyx_v_data_ptr), (&__pyx_v_pysize)); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 615, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (unlikely(!((__pyx_t_11 != -1L) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
-        __PYX_ERR(0, 610, __pyx_L1_error)
+        __PYX_ERR(0, 615, __pyx_L1_error)
       }
     }
     #endif
 
-    /* "viur/datastore/transport.pyx":611
+    /* "viur/datastore/transport.pyx":616
  * 		assert req.status_code == 200
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)             # <<<<<<<<<<<<<<
  * 		if (element.at_pointer("/found").error() == SUCCESS):
  * 			res.update(toEntityStructure(element.at_key("found"), isInitial=True))
  */
     try {
       __pyx_t_12 = __pyx_v_parser.parse(__pyx_v_data_ptr, __pyx_v_pysize, 1);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 611, __pyx_L1_error)
+      __PYX_ERR(0, 616, __pyx_L1_error)
     }
     __pyx_v_element = __pyx_t_12;
 
-    /* "viur/datastore/transport.pyx":612
+    /* "viur/datastore/transport.pyx":617
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)
  * 		if (element.at_pointer("/found").error() == SUCCESS):             # <<<<<<<<<<<<<<
  * 			res.update(toEntityStructure(element.at_key("found"), isInitial=True))
  * 		if (element.at_pointer("/deferred").error() == SUCCESS):
  */
     __pyx_t_2 = ((__pyx_v_element.at_pointer(((char const *)"/found")).error() == simdjson::error_code::SUCCESS) != 0);
     if (__pyx_t_2) {
 
-      /* "viur/datastore/transport.pyx":613
+      /* "viur/datastore/transport.pyx":618
  * 		element = parser.parse(data_ptr, pysize, 1)
  * 		if (element.at_pointer("/found").error() == SUCCESS):
  * 			res.update(toEntityStructure(element.at_key("found"), isInitial=True))             # <<<<<<<<<<<<<<
  * 		if (element.at_pointer("/deferred").error() == SUCCESS):
  * 			keyList = toPythonStructure(element.at_key("deferred")) + keyList[300:]
  */
       try {
         __pyx_t_12 = __pyx_v_element.at_key(((char const *)"found"));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 613, __pyx_L1_error)
+        __PYX_ERR(0, 618, __pyx_L1_error)
       }
       __pyx_t_13.__pyx_n = 1;
       __pyx_t_13.isInitial = 1;
-      __pyx_t_4 = __pyx_f_4viur_9datastore_9transport_toEntityStructure(__pyx_t_12, &__pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 613, __pyx_L1_error)
+      __pyx_t_4 = __pyx_f_4viur_9datastore_9transport_toEntityStructure(__pyx_t_12, &__pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 618, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyDict_Type_update, __pyx_v_res, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 613, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyDict_Type_update, __pyx_v_res, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 618, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "viur/datastore/transport.pyx":612
+      /* "viur/datastore/transport.pyx":617
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)
  * 		if (element.at_pointer("/found").error() == SUCCESS):             # <<<<<<<<<<<<<<
  * 			res.update(toEntityStructure(element.at_key("found"), isInitial=True))
  * 		if (element.at_pointer("/deferred").error() == SUCCESS):
  */
     }
 
-    /* "viur/datastore/transport.pyx":614
+    /* "viur/datastore/transport.pyx":619
  * 		if (element.at_pointer("/found").error() == SUCCESS):
  * 			res.update(toEntityStructure(element.at_key("found"), isInitial=True))
  * 		if (element.at_pointer("/deferred").error() == SUCCESS):             # <<<<<<<<<<<<<<
  * 			keyList = toPythonStructure(element.at_key("deferred")) + keyList[300:]
  * 		else:
  */
     __pyx_t_2 = ((__pyx_v_element.at_pointer(((char const *)"/deferred")).error() == simdjson::error_code::SUCCESS) != 0);
     if (__pyx_t_2) {
 
-      /* "viur/datastore/transport.pyx":615
+      /* "viur/datastore/transport.pyx":620
  * 			res.update(toEntityStructure(element.at_key("found"), isInitial=True))
  * 		if (element.at_pointer("/deferred").error() == SUCCESS):
  * 			keyList = toPythonStructure(element.at_key("deferred")) + keyList[300:]             # <<<<<<<<<<<<<<
  * 		else:
  * 			keyList = keyList[300:]
  */
       try {
         __pyx_t_12 = __pyx_v_element.at_key(((char const *)"deferred"));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 615, __pyx_L1_error)
+        __PYX_ERR(0, 620, __pyx_L1_error)
       }
-      __pyx_t_6 = __pyx_f_4viur_9datastore_9transport_toPythonStructure(__pyx_t_12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 615, __pyx_L1_error)
+      __pyx_t_6 = __pyx_f_4viur_9datastore_9transport_toPythonStructure(__pyx_t_12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 620, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_v_keyList, 0x12C, 0, NULL, NULL, &__pyx_slice__15, 1, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 615, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_v_keyList, 0x12C, 0, NULL, NULL, &__pyx_slice__15, 1, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 620, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 615, __pyx_L1_error)
+      __pyx_t_1 = PyNumber_Add(__pyx_t_6, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 620, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF_SET(__pyx_v_keyList, __pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "viur/datastore/transport.pyx":614
+      /* "viur/datastore/transport.pyx":619
  * 		if (element.at_pointer("/found").error() == SUCCESS):
  * 			res.update(toEntityStructure(element.at_key("found"), isInitial=True))
  * 		if (element.at_pointer("/deferred").error() == SUCCESS):             # <<<<<<<<<<<<<<
  * 			keyList = toPythonStructure(element.at_key("deferred")) + keyList[300:]
  * 		else:
  */
       goto __pyx_L15;
     }
 
-    /* "viur/datastore/transport.pyx":617
+    /* "viur/datastore/transport.pyx":622
  * 			keyList = toPythonStructure(element.at_key("deferred")) + keyList[300:]
  * 		else:
  * 			keyList = keyList[300:]             # <<<<<<<<<<<<<<
  * 	if not isMulti:
  * 		return res.get(keys[0])
  */
     /*else*/ {
-      __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_keyList, 0x12C, 0, NULL, NULL, &__pyx_slice__15, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 617, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_keyList, 0x12C, 0, NULL, NULL, &__pyx_slice__15, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 622, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF_SET(__pyx_v_keyList, __pyx_t_1);
       __pyx_t_1 = 0;
     }
     __pyx_L15:;
   }
 
-  /* "viur/datastore/transport.pyx":618
+  /* "viur/datastore/transport.pyx":623
  * 		else:
  * 			keyList = keyList[300:]
  * 	if not isMulti:             # <<<<<<<<<<<<<<
  * 		return res.get(keys[0])
  * 	else:
  */
   __pyx_t_2 = ((!(__pyx_v_isMulti != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "viur/datastore/transport.pyx":619
+    /* "viur/datastore/transport.pyx":624
  * 			keyList = keyList[300:]
  * 	if not isMulti:
  * 		return res.get(keys[0])             # <<<<<<<<<<<<<<
  * 	else:
  * 		return [res.get(x) for x in keys]  # Sort by order of incoming keys
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_keys, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_keys, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 624, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyDict_GetItemDefault(__pyx_v_res, __pyx_t_1, Py_None); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 619, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_GetItemDefault(__pyx_v_res, __pyx_t_1, Py_None); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 624, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "viur/datastore/transport.pyx":618
+    /* "viur/datastore/transport.pyx":623
  * 		else:
  * 			keyList = keyList[300:]
  * 	if not isMulti:             # <<<<<<<<<<<<<<
  * 		return res.get(keys[0])
  * 	else:
  */
   }
 
-  /* "viur/datastore/transport.pyx":621
+  /* "viur/datastore/transport.pyx":626
  * 		return res.get(keys[0])
  * 	else:
  * 		return [res.get(x) for x in keys]  # Sort by order of incoming keys             # <<<<<<<<<<<<<<
  * 
  * def Delete(keys: Union[Key, List[Key], Entity, List[Entity]]) -> None:
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     { /* enter inner scope */
-      __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 621, __pyx_L19_error)
+      __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 626, __pyx_L19_error)
       __Pyx_GOTREF(__pyx_t_4);
       if (likely(PyList_CheckExact(__pyx_v_keys)) || PyTuple_CheckExact(__pyx_v_keys)) {
         __pyx_t_1 = __pyx_v_keys; __Pyx_INCREF(__pyx_t_1); __pyx_t_7 = 0;
         __pyx_t_8 = NULL;
       } else {
-        __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_keys); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 621, __pyx_L19_error)
+        __pyx_t_7 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_keys); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 626, __pyx_L19_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_8 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 621, __pyx_L19_error)
+        __pyx_t_8 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 626, __pyx_L19_error)
       }
       for (;;) {
         if (likely(!__pyx_t_8)) {
           if (likely(PyList_CheckExact(__pyx_t_1))) {
             if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_1)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_6); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 621, __pyx_L19_error)
+            __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_6); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 626, __pyx_L19_error)
             #else
-            __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 621, __pyx_L19_error)
+            __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 626, __pyx_L19_error)
             __Pyx_GOTREF(__pyx_t_6);
             #endif
           } else {
             if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_6); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 621, __pyx_L19_error)
+            __pyx_t_6 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_7); __Pyx_INCREF(__pyx_t_6); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 626, __pyx_L19_error)
             #else
-            __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 621, __pyx_L19_error)
+            __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 626, __pyx_L19_error)
             __Pyx_GOTREF(__pyx_t_6);
             #endif
           }
         } else {
           __pyx_t_6 = __pyx_t_8(__pyx_t_1);
           if (unlikely(!__pyx_t_6)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 621, __pyx_L19_error)
+              else __PYX_ERR(0, 626, __pyx_L19_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_6);
         }
         __Pyx_XDECREF_SET(__pyx_8genexpr5__pyx_v_x, __pyx_t_6);
         __pyx_t_6 = 0;
-        __pyx_t_6 = __Pyx_PyDict_GetItemDefault(__pyx_v_res, __pyx_8genexpr5__pyx_v_x, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 621, __pyx_L19_error)
+        __pyx_t_6 = __Pyx_PyDict_GetItemDefault(__pyx_v_res, __pyx_8genexpr5__pyx_v_x, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 626, __pyx_L19_error)
         __Pyx_GOTREF(__pyx_t_6);
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_4, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 621, __pyx_L19_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_4, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 626, __pyx_L19_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_x); __pyx_8genexpr5__pyx_v_x = 0;
       goto __pyx_L22_exit_scope;
       __pyx_L19_error:;
       __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_x); __pyx_8genexpr5__pyx_v_x = 0;
@@ -9560,15 +9730,15 @@
       __pyx_L22_exit_scope:;
     } /* exit inner scope */
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
   }
 
-  /* "viur/datastore/transport.pyx":567
+  /* "viur/datastore/transport.pyx":572
  * 	return res
  * 
  * def Get(keys: Union[Key, List[Key]]) -> Union[None, Entity, List[Entity]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Fetches the entities determined by keys from the datastore. Returns or inserts None if a key is not found.
  */
 
@@ -9595,15 +9765,15 @@
   __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_x);
   __Pyx_XDECREF(__pyx_v_keys);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viur/datastore/transport.pyx":623
+/* "viur/datastore/transport.pyx":628
  * 		return [res.get(x) for x in keys]  # Sort by order of incoming keys
  * 
  * def Delete(keys: Union[Key, List[Key], Entity, List[Entity]]) -> None:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Deletes the entities stored under the given key(s).
  */
 
@@ -9652,397 +9822,397 @@
   simdjson::dom::array __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Delete", 0);
   __Pyx_INCREF(__pyx_v_keys);
 
-  /* "viur/datastore/transport.pyx":631
+  /* "viur/datastore/transport.pyx":636
  * 		:param keys: A Key or a List of Keys
  * 	"""
  * 	cdef simdjsonParser parser = simdjsonParser()             # <<<<<<<<<<<<<<
  * 	cdef Py_ssize_t pysize
  * 	cdef char * data_ptr
  */
   __pyx_v_parser = simdjson::dom::parser();
 
-  /* "viur/datastore/transport.pyx":636
+  /* "viur/datastore/transport.pyx":641
  * 	cdef simdjsonElement element
  * 	cdef simdjsonArray arrayElem
  * 	if isinstance(keys, Key):             # <<<<<<<<<<<<<<
  * 		keys = [keys]
  * 	elif isinstance(keys, Entity):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 636, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 641, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_keys, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 636, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_keys, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 641, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "viur/datastore/transport.pyx":637
+    /* "viur/datastore/transport.pyx":642
  * 	cdef simdjsonArray arrayElem
  * 	if isinstance(keys, Key):
  * 		keys = [keys]             # <<<<<<<<<<<<<<
  * 	elif isinstance(keys, Entity):
  * 		keys = [keys.key]
  */
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 637, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 642, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_keys);
     __Pyx_GIVEREF(__pyx_v_keys);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_v_keys);
     __Pyx_DECREF_SET(__pyx_v_keys, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "viur/datastore/transport.pyx":636
+    /* "viur/datastore/transport.pyx":641
  * 	cdef simdjsonElement element
  * 	cdef simdjsonArray arrayElem
  * 	if isinstance(keys, Key):             # <<<<<<<<<<<<<<
  * 		keys = [keys]
  * 	elif isinstance(keys, Entity):
  */
     goto __pyx_L3;
   }
 
-  /* "viur/datastore/transport.pyx":638
+  /* "viur/datastore/transport.pyx":643
  * 	if isinstance(keys, Key):
  * 		keys = [keys]
  * 	elif isinstance(keys, Entity):             # <<<<<<<<<<<<<<
  * 		keys = [keys.key]
  * 	keys = [(x.key if isinstance(x, Entity) else x) for x in keys]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Entity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 638, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Entity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 643, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyObject_IsInstance(__pyx_v_keys, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 638, __pyx_L1_error)
+  __pyx_t_3 = PyObject_IsInstance(__pyx_v_keys, __pyx_t_1); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 643, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_2 = (__pyx_t_3 != 0);
   if (__pyx_t_2) {
 
-    /* "viur/datastore/transport.pyx":639
+    /* "viur/datastore/transport.pyx":644
  * 		keys = [keys]
  * 	elif isinstance(keys, Entity):
  * 		keys = [keys.key]             # <<<<<<<<<<<<<<
  * 	keys = [(x.key if isinstance(x, Entity) else x) for x in keys]
  * 	accessLog = currentDbAccessLog.get()
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_keys, __pyx_n_s_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 639, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_keys, __pyx_n_s_key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 644, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 639, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 644, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_1);
     PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
     __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_keys, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "viur/datastore/transport.pyx":638
+    /* "viur/datastore/transport.pyx":643
  * 	if isinstance(keys, Key):
  * 		keys = [keys]
  * 	elif isinstance(keys, Entity):             # <<<<<<<<<<<<<<
  * 		keys = [keys.key]
  * 	keys = [(x.key if isinstance(x, Entity) else x) for x in keys]
  */
   }
   __pyx_L3:;
 
-  /* "viur/datastore/transport.pyx":640
+  /* "viur/datastore/transport.pyx":645
  * 	elif isinstance(keys, Entity):
  * 		keys = [keys.key]
  * 	keys = [(x.key if isinstance(x, Entity) else x) for x in keys]             # <<<<<<<<<<<<<<
  * 	accessLog = currentDbAccessLog.get()
  * 	if isinstance(accessLog, set):
  */
   { /* enter inner scope */
-    __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 640, __pyx_L6_error)
+    __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 645, __pyx_L6_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (likely(PyList_CheckExact(__pyx_v_keys)) || PyTuple_CheckExact(__pyx_v_keys)) {
       __pyx_t_1 = __pyx_v_keys; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_keys); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 640, __pyx_L6_error)
+      __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_keys); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 645, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 640, __pyx_L6_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 645, __pyx_L6_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 640, __pyx_L6_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 645, __pyx_L6_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 640, __pyx_L6_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 645, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 640, __pyx_L6_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 645, __pyx_L6_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 640, __pyx_L6_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 645, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_1);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 640, __pyx_L6_error)
+            else __PYX_ERR(0, 645, __pyx_L6_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr6__pyx_v_x, __pyx_t_7);
       __pyx_t_7 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Entity); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 640, __pyx_L6_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Entity); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 645, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_2 = PyObject_IsInstance(__pyx_8genexpr6__pyx_v_x, __pyx_t_8); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 640, __pyx_L6_error)
+      __pyx_t_2 = PyObject_IsInstance(__pyx_8genexpr6__pyx_v_x, __pyx_t_8); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 645, __pyx_L6_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       if ((__pyx_t_2 != 0)) {
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr6__pyx_v_x, __pyx_n_s_key); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 640, __pyx_L6_error)
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr6__pyx_v_x, __pyx_n_s_key); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 645, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_8);
         __pyx_t_7 = __pyx_t_8;
         __pyx_t_8 = 0;
       } else {
         __Pyx_INCREF(__pyx_8genexpr6__pyx_v_x);
         __pyx_t_7 = __pyx_8genexpr6__pyx_v_x;
       }
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_4, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 640, __pyx_L6_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_4, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 645, __pyx_L6_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_x); __pyx_8genexpr6__pyx_v_x = 0;
     goto __pyx_L9_exit_scope;
     __pyx_L6_error:;
     __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_x); __pyx_8genexpr6__pyx_v_x = 0;
     goto __pyx_L1_error;
     __pyx_L9_exit_scope:;
   } /* exit inner scope */
   __Pyx_DECREF_SET(__pyx_v_keys, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":641
+  /* "viur/datastore/transport.pyx":646
  * 		keys = [keys.key]
  * 	keys = [(x.key if isinstance(x, Entity) else x) for x in keys]
  * 	accessLog = currentDbAccessLog.get()             # <<<<<<<<<<<<<<
  * 	if isinstance(accessLog, set):
  * 		accessLog.update(set(keys))
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_currentDbAccessLog); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 641, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_currentDbAccessLog); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_get); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 641, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_get); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 641, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_accessLog = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":642
+  /* "viur/datastore/transport.pyx":647
  * 	keys = [(x.key if isinstance(x, Entity) else x) for x in keys]
  * 	accessLog = currentDbAccessLog.get()
  * 	if isinstance(accessLog, set):             # <<<<<<<<<<<<<<
  * 		accessLog.update(set(keys))
  * 	if not keys:  # We got an empty list (probably a query that returned no results), noting to do here
  */
   __pyx_t_2 = PySet_Check(__pyx_v_accessLog); 
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "viur/datastore/transport.pyx":643
+    /* "viur/datastore/transport.pyx":648
  * 	accessLog = currentDbAccessLog.get()
  * 	if isinstance(accessLog, set):
  * 		accessLog.update(set(keys))             # <<<<<<<<<<<<<<
  * 	if not keys:  # We got an empty list (probably a query that returned no results), noting to do here
  * 		return
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_accessLog, __pyx_n_s_update); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 643, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_accessLog, __pyx_n_s_update); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 648, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_1 = PySet_New(__pyx_v_keys); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 643, __pyx_L1_error)
+    __pyx_t_1 = PySet_New(__pyx_v_keys); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 648, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_1);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 643, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 648, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "viur/datastore/transport.pyx":642
+    /* "viur/datastore/transport.pyx":647
  * 	keys = [(x.key if isinstance(x, Entity) else x) for x in keys]
  * 	accessLog = currentDbAccessLog.get()
  * 	if isinstance(accessLog, set):             # <<<<<<<<<<<<<<
  * 		accessLog.update(set(keys))
  * 	if not keys:  # We got an empty list (probably a query that returned no results), noting to do here
  */
   }
 
-  /* "viur/datastore/transport.pyx":644
+  /* "viur/datastore/transport.pyx":649
  * 	if isinstance(accessLog, set):
  * 		accessLog.update(set(keys))
  * 	if not keys:  # We got an empty list (probably a query that returned no results), noting to do here             # <<<<<<<<<<<<<<
  * 		return
  * 	postData = {
  */
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_keys); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 644, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_keys); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 649, __pyx_L1_error)
   __pyx_t_2 = ((!__pyx_t_3) != 0);
   if (__pyx_t_2) {
 
-    /* "viur/datastore/transport.pyx":645
+    /* "viur/datastore/transport.pyx":650
  * 		accessLog.update(set(keys))
  * 	if not keys:  # We got an empty list (probably a query that returned no results), noting to do here
  * 		return             # <<<<<<<<<<<<<<
  * 	postData = {
  * 		"mode": "NON_TRANSACTIONAL",  #"TRANSACTIONAL", #
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "viur/datastore/transport.pyx":644
+    /* "viur/datastore/transport.pyx":649
  * 	if isinstance(accessLog, set):
  * 		accessLog.update(set(keys))
  * 	if not keys:  # We got an empty list (probably a query that returned no results), noting to do here             # <<<<<<<<<<<<<<
  * 		return
  * 	postData = {
  */
   }
 
-  /* "viur/datastore/transport.pyx":647
+  /* "viur/datastore/transport.pyx":652
  * 		return
  * 	postData = {
  * 		"mode": "NON_TRANSACTIONAL",  #"TRANSACTIONAL", #             # <<<<<<<<<<<<<<
  * 		"mutations": [
  * 			{
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 647, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 652, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_mode, __pyx_n_u_NON_TRANSACTIONAL) < 0) __PYX_ERR(0, 647, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_mode, __pyx_n_u_NON_TRANSACTIONAL) < 0) __PYX_ERR(0, 652, __pyx_L1_error)
   { /* enter inner scope */
 
-    /* "viur/datastore/transport.pyx":648
+    /* "viur/datastore/transport.pyx":653
  * 	postData = {
  * 		"mode": "NON_TRANSACTIONAL",  #"TRANSACTIONAL", #
  * 		"mutations": [             # <<<<<<<<<<<<<<
  * 			{
  * 				"delete": pythonPropToJson(x)["keyValue"]
  */
-    __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 648, __pyx_L14_error)
+    __pyx_t_7 = PyList_New(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 653, __pyx_L14_error)
     __Pyx_GOTREF(__pyx_t_7);
 
-    /* "viur/datastore/transport.pyx":652
+    /* "viur/datastore/transport.pyx":657
  * 				"delete": pythonPropToJson(x)["keyValue"]
  * 			}
  * 			for x in keys             # <<<<<<<<<<<<<<
  * 		]
  * 	}
  */
     if (likely(PyList_CheckExact(__pyx_v_keys)) || PyTuple_CheckExact(__pyx_v_keys)) {
       __pyx_t_1 = __pyx_v_keys; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_keys); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 652, __pyx_L14_error)
+      __pyx_t_5 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_keys); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 657, __pyx_L14_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 652, __pyx_L14_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 657, __pyx_L14_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_8 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_8); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 652, __pyx_L14_error)
+          __pyx_t_8 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_8); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 657, __pyx_L14_error)
           #else
-          __pyx_t_8 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 652, __pyx_L14_error)
+          __pyx_t_8 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 657, __pyx_L14_error)
           __Pyx_GOTREF(__pyx_t_8);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_8); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 652, __pyx_L14_error)
+          __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_8); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 657, __pyx_L14_error)
           #else
-          __pyx_t_8 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 652, __pyx_L14_error)
+          __pyx_t_8 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 657, __pyx_L14_error)
           __Pyx_GOTREF(__pyx_t_8);
           #endif
         }
       } else {
         __pyx_t_8 = __pyx_t_6(__pyx_t_1);
         if (unlikely(!__pyx_t_8)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 652, __pyx_L14_error)
+            else __PYX_ERR(0, 657, __pyx_L14_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_8);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr7__pyx_v_x, __pyx_t_8);
       __pyx_t_8 = 0;
 
-      /* "viur/datastore/transport.pyx":650
+      /* "viur/datastore/transport.pyx":655
  * 		"mutations": [
  * 			{
  * 				"delete": pythonPropToJson(x)["keyValue"]             # <<<<<<<<<<<<<<
  * 			}
  * 			for x in keys
  */
-      __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 650, __pyx_L14_error)
+      __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 655, __pyx_L14_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_pythonPropToJson); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 650, __pyx_L14_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_pythonPropToJson); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 655, __pyx_L14_error)
       __Pyx_GOTREF(__pyx_t_10);
       __pyx_t_11 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_10);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
           __Pyx_INCREF(__pyx_t_11);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_10, function);
         }
       }
       __pyx_t_9 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_11, __pyx_8genexpr7__pyx_v_x) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_8genexpr7__pyx_v_x);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 650, __pyx_L14_error)
+      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 655, __pyx_L14_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_t_9, __pyx_n_u_keyValue); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 650, __pyx_L14_error)
+      __pyx_t_10 = __Pyx_PyObject_Dict_GetItem(__pyx_t_9, __pyx_n_u_keyValue); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 655, __pyx_L14_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_delete, __pyx_t_10) < 0) __PYX_ERR(0, 650, __pyx_L14_error)
+      if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_delete, __pyx_t_10) < 0) __PYX_ERR(0, 655, __pyx_L14_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_7, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 648, __pyx_L14_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_7, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 653, __pyx_L14_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "viur/datastore/transport.pyx":652
+      /* "viur/datastore/transport.pyx":657
  * 				"delete": pythonPropToJson(x)["keyValue"]
  * 			}
  * 			for x in keys             # <<<<<<<<<<<<<<
  * 		]
  * 	}
  */
     }
@@ -10050,105 +10220,105 @@
     __Pyx_XDECREF(__pyx_8genexpr7__pyx_v_x); __pyx_8genexpr7__pyx_v_x = 0;
     goto __pyx_L17_exit_scope;
     __pyx_L14_error:;
     __Pyx_XDECREF(__pyx_8genexpr7__pyx_v_x); __pyx_8genexpr7__pyx_v_x = 0;
     goto __pyx_L1_error;
     __pyx_L17_exit_scope:;
   } /* exit inner scope */
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_mutations, __pyx_t_7) < 0) __PYX_ERR(0, 647, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_mutations, __pyx_t_7) < 0) __PYX_ERR(0, 652, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_postData = ((PyObject*)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":655
+  /* "viur/datastore/transport.pyx":660
  * 		]
  * 	}
  * 	currentTxn = currentTransaction.get()             # <<<<<<<<<<<<<<
  * 	if currentTxn:
  * 		currentTxn["mutations"].extend(postData["mutations"])
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 655, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 655, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_get); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_7) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 655, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_currentTxn = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":656
+  /* "viur/datastore/transport.pyx":661
  * 	}
  * 	currentTxn = currentTransaction.get()
  * 	if currentTxn:             # <<<<<<<<<<<<<<
  * 		currentTxn["mutations"].extend(postData["mutations"])
  * 		# Insert placeholders into affectedEntities as we receive a mutation-result for each key deleted
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_currentTxn); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 656, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_currentTxn); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 661, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "viur/datastore/transport.pyx":657
+    /* "viur/datastore/transport.pyx":662
  * 	currentTxn = currentTransaction.get()
  * 	if currentTxn:
  * 		currentTxn["mutations"].extend(postData["mutations"])             # <<<<<<<<<<<<<<
  * 		# Insert placeholders into affectedEntities as we receive a mutation-result for each key deleted
  * 		currentTxn["affectedEntities"].extend([None] * len(keys))
  */
-    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_currentTxn, __pyx_n_u_mutations); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 657, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_v_currentTxn, __pyx_n_u_mutations); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_extend); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 657, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_extend); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 662, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_postData, __pyx_n_u_mutations); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 657, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_postData, __pyx_n_u_mutations); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
     __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_1);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 657, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 662, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "viur/datastore/transport.pyx":659
+    /* "viur/datastore/transport.pyx":664
  * 		currentTxn["mutations"].extend(postData["mutations"])
  * 		# Insert placeholders into affectedEntities as we receive a mutation-result for each key deleted
  * 		currentTxn["affectedEntities"].extend([None] * len(keys))             # <<<<<<<<<<<<<<
  * 		return
  * 	req = authenticatedRequest(
  */
-    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_currentTxn, __pyx_n_u_affectedEntities); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 659, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_v_currentTxn, __pyx_n_u_affectedEntities); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 664, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_extend); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 659, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_extend); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 664, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_5 = PyObject_Length(__pyx_v_keys); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 659, __pyx_L1_error)
-    __pyx_t_7 = PyList_New(1 * ((__pyx_t_5<0) ? 0:__pyx_t_5)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 659, __pyx_L1_error)
+    __pyx_t_5 = PyObject_Length(__pyx_v_keys); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 664, __pyx_L1_error)
+    __pyx_t_7 = PyList_New(1 * ((__pyx_t_5<0) ? 0:__pyx_t_5)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 664, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_t_5; __pyx_temp++) {
         __Pyx_INCREF(Py_None);
         __Pyx_GIVEREF(Py_None);
         PyList_SET_ITEM(__pyx_t_7, __pyx_temp, Py_None);
       }
@@ -10162,356 +10332,356 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_8, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_7);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 659, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 664, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "viur/datastore/transport.pyx":660
+    /* "viur/datastore/transport.pyx":665
  * 		# Insert placeholders into affectedEntities as we receive a mutation-result for each key deleted
  * 		currentTxn["affectedEntities"].extend([None] * len(keys))
  * 		return             # <<<<<<<<<<<<<<
  * 	req = authenticatedRequest(
  * 		url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "viur/datastore/transport.pyx":656
+    /* "viur/datastore/transport.pyx":661
  * 	}
  * 	currentTxn = currentTransaction.get()
  * 	if currentTxn:             # <<<<<<<<<<<<<<
  * 		currentTxn["mutations"].extend(postData["mutations"])
  * 		# Insert placeholders into affectedEntities as we receive a mutation-result for each key deleted
  */
   }
 
-  /* "viur/datastore/transport.pyx":661
+  /* "viur/datastore/transport.pyx":666
  * 		currentTxn["affectedEntities"].extend([None] * len(keys))
  * 		return
  * 	req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 		url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,
  * 		data=json.dumps(postData).encode("UTF-8"),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 661, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 666, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
-  /* "viur/datastore/transport.pyx":662
+  /* "viur/datastore/transport.pyx":667
  * 		return
  * 	req = authenticatedRequest(
  * 		url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,             # <<<<<<<<<<<<<<
  * 		data=json.dumps(postData).encode("UTF-8"),
  * 	)
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 667, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_projectID); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 662, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_projectID); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 667, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_3, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 662, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_3, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 667, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_url, __pyx_t_8) < 0) __PYX_ERR(0, 662, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_url, __pyx_t_8) < 0) __PYX_ERR(0, 667, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "viur/datastore/transport.pyx":663
+  /* "viur/datastore/transport.pyx":668
  * 	req = authenticatedRequest(
  * 		url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,
  * 		data=json.dumps(postData).encode("UTF-8"),             # <<<<<<<<<<<<<<
  * 	)
  * 	if is_viur_datastore_request_ok(req):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_json); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 663, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_json); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 668, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_dumps); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 663, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_dumps); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 668, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_t_10 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_10);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_9, function);
     }
   }
   __pyx_t_7 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_10, __pyx_v_postData) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_postData);
   __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 663, __pyx_L1_error)
+  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 668, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 663, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_encode); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 668, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_9);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_9, function);
     }
   }
   __pyx_t_8 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_7, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_kp_u_UTF_8);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 663, __pyx_L1_error)
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 668, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_data, __pyx_t_8) < 0) __PYX_ERR(0, 662, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_data, __pyx_t_8) < 0) __PYX_ERR(0, 667, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "viur/datastore/transport.pyx":661
+  /* "viur/datastore/transport.pyx":666
  * 		currentTxn["affectedEntities"].extend([None] * len(keys))
  * 		return
  * 	req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 		url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,
  * 		data=json.dumps(postData).encode("UTF-8"),
  */
-  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 661, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 666, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_req = __pyx_t_8;
   __pyx_t_8 = 0;
 
-  /* "viur/datastore/transport.pyx":665
+  /* "viur/datastore/transport.pyx":670
  * 		data=json.dumps(postData).encode("UTF-8"),
  * 	)
  * 	if is_viur_datastore_request_ok(req):             # <<<<<<<<<<<<<<
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_is_viur_datastore_request_ok); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 665, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_is_viur_datastore_request_ok); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 670, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
   __pyx_t_8 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_v_req) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_req);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 665, __pyx_L1_error)
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 670, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 665, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 670, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   if (__pyx_t_2) {
 
-    /* "viur/datastore/transport.pyx":666
+    /* "viur/datastore/transport.pyx":671
  * 	)
  * 	if is_viur_datastore_request_ok(req):
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1             # <<<<<<<<<<<<<<
  * 		element = parser.parse(data_ptr, pysize, 1)
  * 		if (element.at_pointer("/mutationResults").error() != SUCCESS):
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
     if (unlikely(!Py_OptimizeFlag)) {
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 666, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 671, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_12 = PyBytes_AsStringAndSize(__pyx_t_8, (&__pyx_v_data_ptr), (&__pyx_v_pysize)); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 666, __pyx_L1_error)
+      __pyx_t_12 = PyBytes_AsStringAndSize(__pyx_t_8, (&__pyx_v_data_ptr), (&__pyx_v_pysize)); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 671, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       if (unlikely(!((__pyx_t_12 != -1L) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
-        __PYX_ERR(0, 666, __pyx_L1_error)
+        __PYX_ERR(0, 671, __pyx_L1_error)
       }
     }
     #endif
 
-    /* "viur/datastore/transport.pyx":667
+    /* "viur/datastore/transport.pyx":672
  * 	if is_viur_datastore_request_ok(req):
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)             # <<<<<<<<<<<<<<
  * 		if (element.at_pointer("/mutationResults").error() != SUCCESS):
  * 			pprint(req.content)
  */
     try {
       __pyx_t_13 = __pyx_v_parser.parse(__pyx_v_data_ptr, __pyx_v_pysize, 1);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 667, __pyx_L1_error)
+      __PYX_ERR(0, 672, __pyx_L1_error)
     }
     __pyx_v_element = __pyx_t_13;
 
-    /* "viur/datastore/transport.pyx":668
+    /* "viur/datastore/transport.pyx":673
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)
  * 		if (element.at_pointer("/mutationResults").error() != SUCCESS):             # <<<<<<<<<<<<<<
  * 			pprint(req.content)
  * 			raise NoMutationResultsError("No mutation results received")
  */
     __pyx_t_2 = ((__pyx_v_element.at_pointer(((char const *)"/mutationResults")).error() != simdjson::error_code::SUCCESS) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "viur/datastore/transport.pyx":669
+      /* "viur/datastore/transport.pyx":674
  * 		element = parser.parse(data_ptr, pysize, 1)
  * 		if (element.at_pointer("/mutationResults").error() != SUCCESS):
  * 			pprint(req.content)             # <<<<<<<<<<<<<<
  * 			raise NoMutationResultsError("No mutation results received")
  * 		arrayElem = element.at_key("mutationResults").get_array()
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pprint); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 669, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pprint); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 674, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 669, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 674, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_9 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_9)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
           __Pyx_INCREF(__pyx_t_9);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
       __pyx_t_8 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_9, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_4);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 669, __pyx_L1_error)
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 674, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "viur/datastore/transport.pyx":670
+      /* "viur/datastore/transport.pyx":675
  * 		if (element.at_pointer("/mutationResults").error() != SUCCESS):
  * 			pprint(req.content)
  * 			raise NoMutationResultsError("No mutation results received")             # <<<<<<<<<<<<<<
  * 		arrayElem = element.at_key("mutationResults").get_array()
  * 		if arrayElem.size() != abs(len(keys)):
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_NoMutationResultsError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 670, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_NoMutationResultsError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 675, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
       __pyx_t_8 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_kp_u_No_mutation_results_received) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_u_No_mutation_results_received);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 670, __pyx_L1_error)
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 675, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(0, 670, __pyx_L1_error)
+      __PYX_ERR(0, 675, __pyx_L1_error)
 
-      /* "viur/datastore/transport.pyx":668
+      /* "viur/datastore/transport.pyx":673
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)
  * 		if (element.at_pointer("/mutationResults").error() != SUCCESS):             # <<<<<<<<<<<<<<
  * 			pprint(req.content)
  * 			raise NoMutationResultsError("No mutation results received")
  */
     }
 
-    /* "viur/datastore/transport.pyx":671
+    /* "viur/datastore/transport.pyx":676
  * 			pprint(req.content)
  * 			raise NoMutationResultsError("No mutation results received")
  * 		arrayElem = element.at_key("mutationResults").get_array()             # <<<<<<<<<<<<<<
  * 		if arrayElem.size() != abs(len(keys)):
  * 			print(req.content)
  */
     try {
       __pyx_t_13 = __pyx_v_element.at_key(((char const *)"mutationResults"));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 671, __pyx_L1_error)
+      __PYX_ERR(0, 676, __pyx_L1_error)
     }
     try {
       __pyx_t_14 = __pyx_t_13.get_array();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 671, __pyx_L1_error)
+      __PYX_ERR(0, 676, __pyx_L1_error)
     }
     __pyx_v_arrayElem = __pyx_t_14;
 
-    /* "viur/datastore/transport.pyx":672
+    /* "viur/datastore/transport.pyx":677
  * 			raise NoMutationResultsError("No mutation results received")
  * 		arrayElem = element.at_key("mutationResults").get_array()
  * 		if arrayElem.size() != abs(len(keys)):             # <<<<<<<<<<<<<<
  * 			print(req.content)
  * 			raise ValueError("Invalid number of mutation-results received")
  */
-    __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_arrayElem.size()); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 672, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_arrayElem.size()); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 677, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_5 = PyObject_Length(__pyx_v_keys); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 672, __pyx_L1_error)
-    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 672, __pyx_L1_error)
+    __pyx_t_5 = PyObject_Length(__pyx_v_keys); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 677, __pyx_L1_error)
+    __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 677, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyNumber_Absolute(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 672, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Absolute(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 677, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = PyObject_RichCompare(__pyx_t_8, __pyx_t_4, Py_NE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 672, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_t_8, __pyx_t_4, Py_NE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 677, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 672, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 677, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(__pyx_t_2)) {
 
-      /* "viur/datastore/transport.pyx":673
+      /* "viur/datastore/transport.pyx":678
  * 		arrayElem = element.at_key("mutationResults").get_array()
  * 		if arrayElem.size() != abs(len(keys)):
  * 			print(req.content)             # <<<<<<<<<<<<<<
  * 			raise ValueError("Invalid number of mutation-results received")
  * 
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 673, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 678, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 673, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 678, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "viur/datastore/transport.pyx":674
+      /* "viur/datastore/transport.pyx":679
  * 		if arrayElem.size() != abs(len(keys)):
  * 			print(req.content)
  * 			raise ValueError("Invalid number of mutation-results received")             # <<<<<<<<<<<<<<
  * 
  * def Put(entities: Union[Entity, List[Entity]]) -> Union[Entity, List[Entity]]:
  */
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 674, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 679, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 674, __pyx_L1_error)
+      __PYX_ERR(0, 679, __pyx_L1_error)
 
-      /* "viur/datastore/transport.pyx":672
+      /* "viur/datastore/transport.pyx":677
  * 			raise NoMutationResultsError("No mutation results received")
  * 		arrayElem = element.at_key("mutationResults").get_array()
  * 		if arrayElem.size() != abs(len(keys)):             # <<<<<<<<<<<<<<
  * 			print(req.content)
  * 			raise ValueError("Invalid number of mutation-results received")
  */
     }
 
-    /* "viur/datastore/transport.pyx":665
+    /* "viur/datastore/transport.pyx":670
  * 		data=json.dumps(postData).encode("UTF-8"),
  * 	)
  * 	if is_viur_datastore_request_ok(req):             # <<<<<<<<<<<<<<
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)
  */
   }
 
-  /* "viur/datastore/transport.pyx":623
+  /* "viur/datastore/transport.pyx":628
  * 		return [res.get(x) for x in keys]  # Sort by order of incoming keys
  * 
  * def Delete(keys: Union[Key, List[Key], Entity, List[Entity]]) -> None:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Deletes the entities stored under the given key(s).
  */
 
@@ -10537,15 +10707,15 @@
   __Pyx_XDECREF(__pyx_8genexpr7__pyx_v_x);
   __Pyx_XDECREF(__pyx_v_keys);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viur/datastore/transport.pyx":676
+/* "viur/datastore/transport.pyx":681
  * 			raise ValueError("Invalid number of mutation-results received")
  * 
  * def Put(entities: Union[Entity, List[Entity]]) -> Union[Entity, List[Entity]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Writes the given entities into the datastore. The entities can be from different kinds. If an entity has an
  */
 
@@ -10598,179 +10768,179 @@
   std::string_view __pyx_t_15;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Put", 0);
   __Pyx_INCREF(__pyx_v_entities);
 
-  /* "viur/datastore/transport.pyx":685
+  /* "viur/datastore/transport.pyx":690
  * 			inside a transaction, in which case we return None as no Keys have been determined yet)
  * 	"""
  * 	cdef simdjsonParser parser = simdjsonParser()             # <<<<<<<<<<<<<<
  * 	cdef Py_ssize_t pysize
  * 	cdef char * data_ptr
  */
   __pyx_v_parser = simdjson::dom::parser();
 
-  /* "viur/datastore/transport.pyx":691
+  /* "viur/datastore/transport.pyx":696
  * 	cdef simdjsonArray arrayElem
  * 	cdef simdjsonArray.iterator arrayIt
  * 	if isinstance(entities, Entity):             # <<<<<<<<<<<<<<
  * 		entities = [entities]
  * 	accessLog = currentDbAccessLog.get()
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Entity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 691, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Entity); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 696, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_entities, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 691, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_entities, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 696, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "viur/datastore/transport.pyx":692
+    /* "viur/datastore/transport.pyx":697
  * 	cdef simdjsonArray.iterator arrayIt
  * 	if isinstance(entities, Entity):
  * 		entities = [entities]             # <<<<<<<<<<<<<<
  * 	accessLog = currentDbAccessLog.get()
  * 	if isinstance(accessLog, set):
  */
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 692, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 697, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_entities);
     __Pyx_GIVEREF(__pyx_v_entities);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_v_entities);
     __Pyx_DECREF_SET(__pyx_v_entities, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "viur/datastore/transport.pyx":691
+    /* "viur/datastore/transport.pyx":696
  * 	cdef simdjsonArray arrayElem
  * 	cdef simdjsonArray.iterator arrayIt
  * 	if isinstance(entities, Entity):             # <<<<<<<<<<<<<<
  * 		entities = [entities]
  * 	accessLog = currentDbAccessLog.get()
  */
   }
 
-  /* "viur/datastore/transport.pyx":693
+  /* "viur/datastore/transport.pyx":698
  * 	if isinstance(entities, Entity):
  * 		entities = [entities]
  * 	accessLog = currentDbAccessLog.get()             # <<<<<<<<<<<<<<
  * 	if isinstance(accessLog, set):
  * 		accessLog.update(set([x.key for x in entities if not x.key.is_partial]))
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_currentDbAccessLog); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 693, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_currentDbAccessLog); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 693, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 693, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_accessLog = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "viur/datastore/transport.pyx":694
+  /* "viur/datastore/transport.pyx":699
  * 		entities = [entities]
  * 	accessLog = currentDbAccessLog.get()
  * 	if isinstance(accessLog, set):             # <<<<<<<<<<<<<<
  * 		accessLog.update(set([x.key for x in entities if not x.key.is_partial]))
  * 	postData = {
  */
   __pyx_t_3 = PySet_Check(__pyx_v_accessLog); 
   __pyx_t_2 = (__pyx_t_3 != 0);
   if (__pyx_t_2) {
 
-    /* "viur/datastore/transport.pyx":695
+    /* "viur/datastore/transport.pyx":700
  * 	accessLog = currentDbAccessLog.get()
  * 	if isinstance(accessLog, set):
  * 		accessLog.update(set([x.key for x in entities if not x.key.is_partial]))             # <<<<<<<<<<<<<<
  * 	postData = {
  * 		"mode": "NON_TRANSACTIONAL",  # Always NON_TRANSACTIONAL; if we're inside a transaction we'll abort below
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_accessLog, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 695, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_accessLog, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 700, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     { /* enter inner scope */
-      __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 695, __pyx_L7_error)
+      __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 700, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_4);
       if (likely(PyList_CheckExact(__pyx_v_entities)) || PyTuple_CheckExact(__pyx_v_entities)) {
         __pyx_t_6 = __pyx_v_entities; __Pyx_INCREF(__pyx_t_6); __pyx_t_7 = 0;
         __pyx_t_8 = NULL;
       } else {
-        __pyx_t_7 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_entities); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 695, __pyx_L7_error)
+        __pyx_t_7 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_entities); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 700, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_8 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 695, __pyx_L7_error)
+        __pyx_t_8 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 700, __pyx_L7_error)
       }
       for (;;) {
         if (likely(!__pyx_t_8)) {
           if (likely(PyList_CheckExact(__pyx_t_6))) {
             if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_6)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_9 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 695, __pyx_L7_error)
+            __pyx_t_9 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 700, __pyx_L7_error)
             #else
-            __pyx_t_9 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 695, __pyx_L7_error)
+            __pyx_t_9 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 700, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_9);
             #endif
           } else {
             if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 695, __pyx_L7_error)
+            __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 700, __pyx_L7_error)
             #else
-            __pyx_t_9 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 695, __pyx_L7_error)
+            __pyx_t_9 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 700, __pyx_L7_error)
             __Pyx_GOTREF(__pyx_t_9);
             #endif
           }
         } else {
           __pyx_t_9 = __pyx_t_8(__pyx_t_6);
           if (unlikely(!__pyx_t_9)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 695, __pyx_L7_error)
+              else __PYX_ERR(0, 700, __pyx_L7_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_9);
         }
         __Pyx_XDECREF_SET(__pyx_8genexpr8__pyx_v_x, __pyx_t_9);
         __pyx_t_9 = 0;
-        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr8__pyx_v_x, __pyx_n_s_key); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 695, __pyx_L7_error)
+        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr8__pyx_v_x, __pyx_n_s_key); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 700, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_9);
-        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_is_partial); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 695, __pyx_L7_error)
+        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_is_partial); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 700, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 695, __pyx_L7_error)
+        __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 700, __pyx_L7_error)
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         __pyx_t_3 = ((!__pyx_t_2) != 0);
         if (__pyx_t_3) {
-          __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr8__pyx_v_x, __pyx_n_s_key); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 695, __pyx_L7_error)
+          __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr8__pyx_v_x, __pyx_n_s_key); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 700, __pyx_L7_error)
           __Pyx_GOTREF(__pyx_t_10);
-          if (unlikely(__Pyx_ListComp_Append(__pyx_t_4, (PyObject*)__pyx_t_10))) __PYX_ERR(0, 695, __pyx_L7_error)
+          if (unlikely(__Pyx_ListComp_Append(__pyx_t_4, (PyObject*)__pyx_t_10))) __PYX_ERR(0, 700, __pyx_L7_error)
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         }
       }
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_8genexpr8__pyx_v_x); __pyx_8genexpr8__pyx_v_x = 0;
       goto __pyx_L11_exit_scope;
       __pyx_L7_error:;
       __Pyx_XDECREF(__pyx_8genexpr8__pyx_v_x); __pyx_8genexpr8__pyx_v_x = 0;
       goto __pyx_L1_error;
       __pyx_L11_exit_scope:;
     } /* exit inner scope */
-    __pyx_t_6 = PySet_New(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 695, __pyx_L1_error)
+    __pyx_t_6 = PySet_New(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 700, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -10778,134 +10948,134 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 695, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 700, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "viur/datastore/transport.pyx":694
+    /* "viur/datastore/transport.pyx":699
  * 		entities = [entities]
  * 	accessLog = currentDbAccessLog.get()
  * 	if isinstance(accessLog, set):             # <<<<<<<<<<<<<<
  * 		accessLog.update(set([x.key for x in entities if not x.key.is_partial]))
  * 	postData = {
  */
   }
 
-  /* "viur/datastore/transport.pyx":697
+  /* "viur/datastore/transport.pyx":702
  * 		accessLog.update(set([x.key for x in entities if not x.key.is_partial]))
  * 	postData = {
  * 		"mode": "NON_TRANSACTIONAL",  # Always NON_TRANSACTIONAL; if we're inside a transaction we'll abort below             # <<<<<<<<<<<<<<
  * 		"mutations": [
  * 			{
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 697, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 702, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_mode, __pyx_n_u_NON_TRANSACTIONAL) < 0) __PYX_ERR(0, 697, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_mode, __pyx_n_u_NON_TRANSACTIONAL) < 0) __PYX_ERR(0, 702, __pyx_L1_error)
   { /* enter inner scope */
 
-    /* "viur/datastore/transport.pyx":698
+    /* "viur/datastore/transport.pyx":703
  * 	postData = {
  * 		"mode": "NON_TRANSACTIONAL",  # Always NON_TRANSACTIONAL; if we're inside a transaction we'll abort below
  * 		"mutations": [             # <<<<<<<<<<<<<<
  * 			{
  * 				"upsert": pythonPropToJson(x)["entityValue"]
  */
-    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 698, __pyx_L14_error)
+    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 703, __pyx_L14_error)
     __Pyx_GOTREF(__pyx_t_5);
 
-    /* "viur/datastore/transport.pyx":702
+    /* "viur/datastore/transport.pyx":707
  * 				"upsert": pythonPropToJson(x)["entityValue"]
  * 			}
  * 			for x in entities             # <<<<<<<<<<<<<<
  * 		]
  * 	}
  */
     if (likely(PyList_CheckExact(__pyx_v_entities)) || PyTuple_CheckExact(__pyx_v_entities)) {
       __pyx_t_6 = __pyx_v_entities; __Pyx_INCREF(__pyx_t_6); __pyx_t_7 = 0;
       __pyx_t_8 = NULL;
     } else {
-      __pyx_t_7 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_entities); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 702, __pyx_L14_error)
+      __pyx_t_7 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_entities); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 707, __pyx_L14_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_8 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 702, __pyx_L14_error)
+      __pyx_t_8 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 707, __pyx_L14_error)
     }
     for (;;) {
       if (likely(!__pyx_t_8)) {
         if (likely(PyList_CheckExact(__pyx_t_6))) {
           if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_6)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 702, __pyx_L14_error)
+          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 707, __pyx_L14_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 702, __pyx_L14_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 707, __pyx_L14_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         } else {
           if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 702, __pyx_L14_error)
+          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_4); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 707, __pyx_L14_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 702, __pyx_L14_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 707, __pyx_L14_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         }
       } else {
         __pyx_t_4 = __pyx_t_8(__pyx_t_6);
         if (unlikely(!__pyx_t_4)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 702, __pyx_L14_error)
+            else __PYX_ERR(0, 707, __pyx_L14_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_4);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr9__pyx_v_x, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "viur/datastore/transport.pyx":700
+      /* "viur/datastore/transport.pyx":705
  * 		"mutations": [
  * 			{
  * 				"upsert": pythonPropToJson(x)["entityValue"]             # <<<<<<<<<<<<<<
  * 			}
  * 			for x in entities
  */
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 700, __pyx_L14_error)
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 705, __pyx_L14_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_pythonPropToJson); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 700, __pyx_L14_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_pythonPropToJson); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 705, __pyx_L14_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_11 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_11)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_11);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
         }
       }
       __pyx_t_10 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_11, __pyx_8genexpr9__pyx_v_x) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_8genexpr9__pyx_v_x);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 700, __pyx_L14_error)
+      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 705, __pyx_L14_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_t_10, __pyx_n_u_entityValue); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 700, __pyx_L14_error)
+      __pyx_t_9 = __Pyx_PyObject_Dict_GetItem(__pyx_t_10, __pyx_n_u_entityValue); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 705, __pyx_L14_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_upsert, __pyx_t_9) < 0) __PYX_ERR(0, 700, __pyx_L14_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_upsert, __pyx_t_9) < 0) __PYX_ERR(0, 705, __pyx_L14_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 698, __pyx_L14_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 703, __pyx_L14_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "viur/datastore/transport.pyx":702
+      /* "viur/datastore/transport.pyx":707
  * 				"upsert": pythonPropToJson(x)["entityValue"]
  * 			}
  * 			for x in entities             # <<<<<<<<<<<<<<
  * 		]
  * 	}
  */
     }
@@ -10913,597 +11083,597 @@
     __Pyx_XDECREF(__pyx_8genexpr9__pyx_v_x); __pyx_8genexpr9__pyx_v_x = 0;
     goto __pyx_L17_exit_scope;
     __pyx_L14_error:;
     __Pyx_XDECREF(__pyx_8genexpr9__pyx_v_x); __pyx_8genexpr9__pyx_v_x = 0;
     goto __pyx_L1_error;
     __pyx_L17_exit_scope:;
   } /* exit inner scope */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_mutations, __pyx_t_5) < 0) __PYX_ERR(0, 697, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_mutations, __pyx_t_5) < 0) __PYX_ERR(0, 702, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_postData = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "viur/datastore/transport.pyx":705
+  /* "viur/datastore/transport.pyx":710
  * 		]
  * 	}
  * 	currentTxn = currentTransaction.get()             # <<<<<<<<<<<<<<
  * 	if currentTxn:  # We're currently inside a transaction, just queue the changes
  * 		currentTxn["mutations"].extend(postData["mutations"])
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 705, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 710, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 705, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_get); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 710, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 705, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 710, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_currentTxn = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "viur/datastore/transport.pyx":706
+  /* "viur/datastore/transport.pyx":711
  * 	}
  * 	currentTxn = currentTransaction.get()
  * 	if currentTxn:  # We're currently inside a transaction, just queue the changes             # <<<<<<<<<<<<<<
  * 		currentTxn["mutations"].extend(postData["mutations"])
  * 		currentTxn["affectedEntities"].extend(entities)
  */
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_currentTxn); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 706, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_currentTxn); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 711, __pyx_L1_error)
   if (__pyx_t_3) {
 
-    /* "viur/datastore/transport.pyx":707
+    /* "viur/datastore/transport.pyx":712
  * 	currentTxn = currentTransaction.get()
  * 	if currentTxn:  # We're currently inside a transaction, just queue the changes
  * 		currentTxn["mutations"].extend(postData["mutations"])             # <<<<<<<<<<<<<<
  * 		currentTxn["affectedEntities"].extend(entities)
  * 		return
  */
-    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_currentTxn, __pyx_n_u_mutations); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 707, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Dict_GetItem(__pyx_v_currentTxn, __pyx_n_u_mutations); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 712, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_extend); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 707, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_extend); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 712, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_postData, __pyx_n_u_mutations); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 707, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_postData, __pyx_n_u_mutations); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 712, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 707, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 712, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "viur/datastore/transport.pyx":708
+    /* "viur/datastore/transport.pyx":713
  * 	if currentTxn:  # We're currently inside a transaction, just queue the changes
  * 		currentTxn["mutations"].extend(postData["mutations"])
  * 		currentTxn["affectedEntities"].extend(entities)             # <<<<<<<<<<<<<<
  * 		return
  * 	req = authenticatedRequest(
  */
-    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_currentTxn, __pyx_n_u_affectedEntities); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 708, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_currentTxn, __pyx_n_u_affectedEntities); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 713, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_extend); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 708, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_extend); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 713, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_entities) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_entities);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 708, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 713, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "viur/datastore/transport.pyx":709
+    /* "viur/datastore/transport.pyx":714
  * 		currentTxn["mutations"].extend(postData["mutations"])
  * 		currentTxn["affectedEntities"].extend(entities)
  * 		return             # <<<<<<<<<<<<<<
  * 	req = authenticatedRequest(
  * 		url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "viur/datastore/transport.pyx":706
+    /* "viur/datastore/transport.pyx":711
  * 	}
  * 	currentTxn = currentTransaction.get()
  * 	if currentTxn:  # We're currently inside a transaction, just queue the changes             # <<<<<<<<<<<<<<
  * 		currentTxn["mutations"].extend(postData["mutations"])
  * 		currentTxn["affectedEntities"].extend(entities)
  */
   }
 
-  /* "viur/datastore/transport.pyx":710
+  /* "viur/datastore/transport.pyx":715
  * 		currentTxn["affectedEntities"].extend(entities)
  * 		return
  * 	req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 		url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,
  * 		data=json.dumps(postData).encode("UTF-8"),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 710, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 715, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "viur/datastore/transport.pyx":711
+  /* "viur/datastore/transport.pyx":716
  * 		return
  * 	req = authenticatedRequest(
  * 		url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,             # <<<<<<<<<<<<<<
  * 		data=json.dumps(postData).encode("UTF-8"),
  * 	)
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 716, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_projectID); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_projectID); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 716, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 716, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_url, __pyx_t_4) < 0) __PYX_ERR(0, 711, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_url, __pyx_t_4) < 0) __PYX_ERR(0, 716, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":712
+  /* "viur/datastore/transport.pyx":717
  * 	req = authenticatedRequest(
  * 		url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,
  * 		data=json.dumps(postData).encode("UTF-8"),             # <<<<<<<<<<<<<<
  * 	)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_json); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 712, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_json); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 717, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_dumps); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 712, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_dumps); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 717, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_10, function);
     }
   }
   __pyx_t_5 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_9, __pyx_v_postData) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_v_postData);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 712, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 717, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_encode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 712, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_encode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 717, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_10, function);
     }
   }
   __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_5, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_kp_u_UTF_8);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 712, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 717, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_data, __pyx_t_4) < 0) __PYX_ERR(0, 711, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_data, __pyx_t_4) < 0) __PYX_ERR(0, 716, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":710
+  /* "viur/datastore/transport.pyx":715
  * 		currentTxn["affectedEntities"].extend(entities)
  * 		return
  * 	req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 		url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,
  * 		data=json.dumps(postData).encode("UTF-8"),
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 710, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 715, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_req = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":715
+  /* "viur/datastore/transport.pyx":720
  * 	)
  * 
  * 	if is_viur_datastore_request_ok(req):             # <<<<<<<<<<<<<<
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_is_viur_datastore_request_ok); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 715, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_is_viur_datastore_request_ok); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_1, __pyx_v_req) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_req);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 715, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 715, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_3) {
 
-    /* "viur/datastore/transport.pyx":716
+    /* "viur/datastore/transport.pyx":721
  * 
  * 	if is_viur_datastore_request_ok(req):
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1             # <<<<<<<<<<<<<<
  * 		element = parser.parse(data_ptr, pysize, 1)
  * 		if (element.at_pointer("/mutationResults").error() != SUCCESS):
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
     if (unlikely(!Py_OptimizeFlag)) {
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 716, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 721, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_12 = PyBytes_AsStringAndSize(__pyx_t_4, (&__pyx_v_data_ptr), (&__pyx_v_pysize)); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 716, __pyx_L1_error)
+      __pyx_t_12 = PyBytes_AsStringAndSize(__pyx_t_4, (&__pyx_v_data_ptr), (&__pyx_v_pysize)); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(0, 721, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (unlikely(!((__pyx_t_12 != -1L) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
-        __PYX_ERR(0, 716, __pyx_L1_error)
+        __PYX_ERR(0, 721, __pyx_L1_error)
       }
     }
     #endif
 
-    /* "viur/datastore/transport.pyx":717
+    /* "viur/datastore/transport.pyx":722
  * 	if is_viur_datastore_request_ok(req):
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)             # <<<<<<<<<<<<<<
  * 		if (element.at_pointer("/mutationResults").error() != SUCCESS):
  * 			print(req.content)
  */
     try {
       __pyx_t_13 = __pyx_v_parser.parse(__pyx_v_data_ptr, __pyx_v_pysize, 1);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 717, __pyx_L1_error)
+      __PYX_ERR(0, 722, __pyx_L1_error)
     }
     __pyx_v_element = __pyx_t_13;
 
-    /* "viur/datastore/transport.pyx":718
+    /* "viur/datastore/transport.pyx":723
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)
  * 		if (element.at_pointer("/mutationResults").error() != SUCCESS):             # <<<<<<<<<<<<<<
  * 			print(req.content)
  * 			raise ValueError("No mutation-results received")
  */
     __pyx_t_3 = ((__pyx_v_element.at_pointer(((char const *)"/mutationResults")).error() != simdjson::error_code::SUCCESS) != 0);
     if (unlikely(__pyx_t_3)) {
 
-      /* "viur/datastore/transport.pyx":719
+      /* "viur/datastore/transport.pyx":724
  * 		element = parser.parse(data_ptr, pysize, 1)
  * 		if (element.at_pointer("/mutationResults").error() != SUCCESS):
  * 			print(req.content)             # <<<<<<<<<<<<<<
  * 			raise ValueError("No mutation-results received")
  * 		arrayElem = element.at_key("mutationResults").get_array()
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 719, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 724, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 719, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 724, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "viur/datastore/transport.pyx":720
+      /* "viur/datastore/transport.pyx":725
  * 		if (element.at_pointer("/mutationResults").error() != SUCCESS):
  * 			print(req.content)
  * 			raise ValueError("No mutation-results received")             # <<<<<<<<<<<<<<
  * 		arrayElem = element.at_key("mutationResults").get_array()
  * 		if arrayElem.size() != abs(len(entities)):
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 720, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 725, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 720, __pyx_L1_error)
+      __PYX_ERR(0, 725, __pyx_L1_error)
 
-      /* "viur/datastore/transport.pyx":718
+      /* "viur/datastore/transport.pyx":723
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)
  * 		if (element.at_pointer("/mutationResults").error() != SUCCESS):             # <<<<<<<<<<<<<<
  * 			print(req.content)
  * 			raise ValueError("No mutation-results received")
  */
     }
 
-    /* "viur/datastore/transport.pyx":721
+    /* "viur/datastore/transport.pyx":726
  * 			print(req.content)
  * 			raise ValueError("No mutation-results received")
  * 		arrayElem = element.at_key("mutationResults").get_array()             # <<<<<<<<<<<<<<
  * 		if arrayElem.size() != abs(len(entities)):
  * 			pprint(req.content)
  */
     try {
       __pyx_t_13 = __pyx_v_element.at_key(((char const *)"mutationResults"));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 721, __pyx_L1_error)
+      __PYX_ERR(0, 726, __pyx_L1_error)
     }
     try {
       __pyx_t_14 = __pyx_t_13.get_array();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 721, __pyx_L1_error)
+      __PYX_ERR(0, 726, __pyx_L1_error)
     }
     __pyx_v_arrayElem = __pyx_t_14;
 
-    /* "viur/datastore/transport.pyx":722
+    /* "viur/datastore/transport.pyx":727
  * 			raise ValueError("No mutation-results received")
  * 		arrayElem = element.at_key("mutationResults").get_array()
  * 		if arrayElem.size() != abs(len(entities)):             # <<<<<<<<<<<<<<
  * 			pprint(req.content)
  * 			raise NoMutationResultsError("Invalid number of mutation-results received")
  */
-    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_arrayElem.size()); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 722, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_arrayElem.size()); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 727, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = PyObject_Length(__pyx_v_entities); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 722, __pyx_L1_error)
-    __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 722, __pyx_L1_error)
+    __pyx_t_7 = PyObject_Length(__pyx_v_entities); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 727, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 727, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = __Pyx_PyNumber_Absolute(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 722, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyNumber_Absolute(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 727, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyObject_RichCompare(__pyx_t_6, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 722, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_t_6, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 727, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 722, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 727, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "viur/datastore/transport.pyx":723
+      /* "viur/datastore/transport.pyx":728
  * 		arrayElem = element.at_key("mutationResults").get_array()
  * 		if arrayElem.size() != abs(len(entities)):
  * 			pprint(req.content)             # <<<<<<<<<<<<<<
  * 			raise NoMutationResultsError("Invalid number of mutation-results received")
  * 		arrayIt = arrayElem.begin()
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pprint); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 723, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pprint); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 728, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 723, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 728, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
       __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_10, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_6);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 723, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 728, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "viur/datastore/transport.pyx":724
+      /* "viur/datastore/transport.pyx":729
  * 		if arrayElem.size() != abs(len(entities)):
  * 			pprint(req.content)
  * 			raise NoMutationResultsError("Invalid number of mutation-results received")             # <<<<<<<<<<<<<<
  * 		arrayIt = arrayElem.begin()
  * 		idx = 0
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_NoMutationResultsError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 724, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_NoMutationResultsError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 729, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_6 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
         if (likely(__pyx_t_6)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_1, function);
         }
       }
       __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_kp_u_Invalid_number_of_mutation_resul) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_u_Invalid_number_of_mutation_resul);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 724, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 729, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 724, __pyx_L1_error)
+      __PYX_ERR(0, 729, __pyx_L1_error)
 
-      /* "viur/datastore/transport.pyx":722
+      /* "viur/datastore/transport.pyx":727
  * 			raise ValueError("No mutation-results received")
  * 		arrayElem = element.at_key("mutationResults").get_array()
  * 		if arrayElem.size() != abs(len(entities)):             # <<<<<<<<<<<<<<
  * 			pprint(req.content)
  * 			raise NoMutationResultsError("Invalid number of mutation-results received")
  */
     }
 
-    /* "viur/datastore/transport.pyx":725
+    /* "viur/datastore/transport.pyx":730
  * 			pprint(req.content)
  * 			raise NoMutationResultsError("Invalid number of mutation-results received")
  * 		arrayIt = arrayElem.begin()             # <<<<<<<<<<<<<<
  * 		idx = 0
  * 		while arrayIt != arrayElem.end():
  */
     __pyx_v_arrayIt = __pyx_v_arrayElem.begin();
 
-    /* "viur/datastore/transport.pyx":726
+    /* "viur/datastore/transport.pyx":731
  * 			raise NoMutationResultsError("Invalid number of mutation-results received")
  * 		arrayIt = arrayElem.begin()
  * 		idx = 0             # <<<<<<<<<<<<<<
  * 		while arrayIt != arrayElem.end():
  * 			innerArrayElem = dereference(arrayIt)
  */
     __Pyx_INCREF(__pyx_int_0);
     __pyx_v_idx = __pyx_int_0;
 
-    /* "viur/datastore/transport.pyx":727
+    /* "viur/datastore/transport.pyx":732
  * 		arrayIt = arrayElem.begin()
  * 		idx = 0
  * 		while arrayIt != arrayElem.end():             # <<<<<<<<<<<<<<
  * 			innerArrayElem = dereference(arrayIt)
  * 			if innerArrayElem.at_pointer("/key").error() == SUCCESS:  # We got a new key assigned
  */
     while (1) {
       __pyx_t_3 = ((__pyx_v_arrayIt != __pyx_v_arrayElem.end()) != 0);
       if (!__pyx_t_3) break;
 
-      /* "viur/datastore/transport.pyx":728
+      /* "viur/datastore/transport.pyx":733
  * 		idx = 0
  * 		while arrayIt != arrayElem.end():
  * 			innerArrayElem = dereference(arrayIt)             # <<<<<<<<<<<<<<
  * 			if innerArrayElem.at_pointer("/key").error() == SUCCESS:  # We got a new key assigned
  * 				entities[idx].key = parseKey(innerArrayElem.at_key("key"))
  */
       __pyx_v_innerArrayElem = (*__pyx_v_arrayIt);
 
-      /* "viur/datastore/transport.pyx":729
+      /* "viur/datastore/transport.pyx":734
  * 		while arrayIt != arrayElem.end():
  * 			innerArrayElem = dereference(arrayIt)
  * 			if innerArrayElem.at_pointer("/key").error() == SUCCESS:  # We got a new key assigned             # <<<<<<<<<<<<<<
  * 				entities[idx].key = parseKey(innerArrayElem.at_key("key"))
  * 			entities[idx].version = toPyStr(innerArrayElem.at_key("version").get_string())
  */
       __pyx_t_3 = ((__pyx_v_innerArrayElem.at_pointer(((char const *)"/key")).error() == simdjson::error_code::SUCCESS) != 0);
       if (__pyx_t_3) {
 
-        /* "viur/datastore/transport.pyx":730
+        /* "viur/datastore/transport.pyx":735
  * 			innerArrayElem = dereference(arrayIt)
  * 			if innerArrayElem.at_pointer("/key").error() == SUCCESS:  # We got a new key assigned
  * 				entities[idx].key = parseKey(innerArrayElem.at_key("key"))             # <<<<<<<<<<<<<<
  * 			entities[idx].version = toPyStr(innerArrayElem.at_key("version").get_string())
  * 			preincrement(arrayIt)
  */
         try {
           __pyx_t_13 = __pyx_v_innerArrayElem.at_key(((char const *)"key"));
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 730, __pyx_L1_error)
+          __PYX_ERR(0, 735, __pyx_L1_error)
         }
-        __pyx_t_4 = __pyx_f_4viur_9datastore_9transport_parseKey(__pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 730, __pyx_L1_error)
+        __pyx_t_4 = __pyx_f_4viur_9datastore_9transport_parseKey(__pyx_t_13); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 735, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_entities, __pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 730, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_entities, __pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 735, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_key, __pyx_t_4) < 0) __PYX_ERR(0, 730, __pyx_L1_error)
+        if (__Pyx_PyObject_SetAttrStr(__pyx_t_1, __pyx_n_s_key, __pyx_t_4) < 0) __PYX_ERR(0, 735, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "viur/datastore/transport.pyx":729
+        /* "viur/datastore/transport.pyx":734
  * 		while arrayIt != arrayElem.end():
  * 			innerArrayElem = dereference(arrayIt)
  * 			if innerArrayElem.at_pointer("/key").error() == SUCCESS:  # We got a new key assigned             # <<<<<<<<<<<<<<
  * 				entities[idx].key = parseKey(innerArrayElem.at_key("key"))
  * 			entities[idx].version = toPyStr(innerArrayElem.at_key("version").get_string())
  */
       }
 
-      /* "viur/datastore/transport.pyx":731
+      /* "viur/datastore/transport.pyx":736
  * 			if innerArrayElem.at_pointer("/key").error() == SUCCESS:  # We got a new key assigned
  * 				entities[idx].key = parseKey(innerArrayElem.at_key("key"))
  * 			entities[idx].version = toPyStr(innerArrayElem.at_key("version").get_string())             # <<<<<<<<<<<<<<
  * 			preincrement(arrayIt)
  * 			idx += 1
  */
       try {
         __pyx_t_13 = __pyx_v_innerArrayElem.at_key(((char const *)"version"));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 731, __pyx_L1_error)
+        __PYX_ERR(0, 736, __pyx_L1_error)
       }
       try {
         __pyx_t_15 = __pyx_t_13.get_string();
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 731, __pyx_L1_error)
+        __PYX_ERR(0, 736, __pyx_L1_error)
       }
-      __pyx_t_1 = __pyx_f_4viur_9datastore_9transport_toPyStr(__pyx_t_15); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 731, __pyx_L1_error)
+      __pyx_t_1 = __pyx_f_4viur_9datastore_9transport_toPyStr(__pyx_t_15); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 736, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_entities, __pyx_v_idx); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 731, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_v_entities, __pyx_v_idx); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 736, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (__Pyx_PyObject_SetAttrStr(__pyx_t_4, __pyx_n_s_version, __pyx_t_1) < 0) __PYX_ERR(0, 731, __pyx_L1_error)
+      if (__Pyx_PyObject_SetAttrStr(__pyx_t_4, __pyx_n_s_version, __pyx_t_1) < 0) __PYX_ERR(0, 736, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "viur/datastore/transport.pyx":732
+      /* "viur/datastore/transport.pyx":737
  * 				entities[idx].key = parseKey(innerArrayElem.at_key("key"))
  * 			entities[idx].version = toPyStr(innerArrayElem.at_key("version").get_string())
  * 			preincrement(arrayIt)             # <<<<<<<<<<<<<<
  * 			idx += 1
  * 	return entities
  */
       (void)((++__pyx_v_arrayIt));
 
-      /* "viur/datastore/transport.pyx":733
+      /* "viur/datastore/transport.pyx":738
  * 			entities[idx].version = toPyStr(innerArrayElem.at_key("version").get_string())
  * 			preincrement(arrayIt)
  * 			idx += 1             # <<<<<<<<<<<<<<
  * 	return entities
  * 
  */
-      __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_v_idx, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 733, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_v_idx, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 738, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF_SET(__pyx_v_idx, __pyx_t_4);
       __pyx_t_4 = 0;
     }
 
-    /* "viur/datastore/transport.pyx":715
+    /* "viur/datastore/transport.pyx":720
  * 	)
  * 
  * 	if is_viur_datastore_request_ok(req):             # <<<<<<<<<<<<<<
  * 		assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 		element = parser.parse(data_ptr, pysize, 1)
  */
   }
 
-  /* "viur/datastore/transport.pyx":734
+  /* "viur/datastore/transport.pyx":739
  * 			preincrement(arrayIt)
  * 			idx += 1
  * 	return entities             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_entities);
   __pyx_r = __pyx_v_entities;
   goto __pyx_L0;
 
-  /* "viur/datastore/transport.pyx":676
+  /* "viur/datastore/transport.pyx":681
  * 			raise ValueError("Invalid number of mutation-results received")
  * 
  * def Put(entities: Union[Entity, List[Entity]]) -> Union[Entity, List[Entity]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Writes the given entities into the datastore. The entities can be from different kinds. If an entity has an
  */
 
@@ -11528,15 +11698,15 @@
   __Pyx_XDECREF(__pyx_8genexpr9__pyx_v_x);
   __Pyx_XDECREF(__pyx_v_entities);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viur/datastore/transport.pyx":737
+/* "viur/datastore/transport.pyx":742
  * 
  * 
  * def RunInTransaction(callback: callable, *args, **kwargs) -> Any:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Runs the given function inside a AID transaction.
  */
 
@@ -11583,26 +11753,26 @@
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_callback)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t used_pos_args = (pos_args < 1) ? pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, used_pos_args, "RunInTransaction") < 0)) __PYX_ERR(0, 737, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, used_pos_args, "RunInTransaction") < 0)) __PYX_ERR(0, 742, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) < 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_callback = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("RunInTransaction", 0, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 737, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("RunInTransaction", 0, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 742, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_args); __pyx_v_args = 0;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("viur.datastore.transport.RunInTransaction", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -11663,37 +11833,37 @@
   PyObject *__pyx_t_25 = NULL;
   PyObject *__pyx_t_26 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("RunInTransaction", 0);
 
-  /* "viur/datastore/transport.pyx":746
+  /* "viur/datastore/transport.pyx":751
  * 		:return: The return-value of the callback function
  * 	"""
  * 	cdef simdjsonParser parser = simdjsonParser()             # <<<<<<<<<<<<<<
  * 	cdef Py_ssize_t pysize
  * 	cdef char * data_ptr
  */
   __pyx_v_parser = simdjson::dom::parser();
 
-  /* "viur/datastore/transport.pyx":752
+  /* "viur/datastore/transport.pyx":757
  * 	cdef simdjsonArray arrayElem
  * 	cdef simdjsonArray.iterator arrayIt
  * 	for exponential_backoff in range(1, 4):             # <<<<<<<<<<<<<<
  * 		try:
  * 			oldTxn = currentTransaction.get()
  */
   for (__pyx_t_1 = 1; __pyx_t_1 < 4; __pyx_t_1+=1) {
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 752, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 757, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_exponential_backoff, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "viur/datastore/transport.pyx":753
+    /* "viur/datastore/transport.pyx":758
  * 	cdef simdjsonArray.iterator arrayIt
  * 	for exponential_backoff in range(1, 4):
  * 		try:             # <<<<<<<<<<<<<<
  * 			oldTxn = currentTransaction.get()
  * 			allowOverriding = kwargs.pop("__allowOverriding__", None)
  */
     {
@@ -11701,381 +11871,381 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
-        /* "viur/datastore/transport.pyx":754
+        /* "viur/datastore/transport.pyx":759
  * 	for exponential_backoff in range(1, 4):
  * 		try:
  * 			oldTxn = currentTransaction.get()             # <<<<<<<<<<<<<<
  * 			allowOverriding = kwargs.pop("__allowOverriding__", None)
  * 			if oldTxn:
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 754, __pyx_L5_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 759, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_get); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 754, __pyx_L5_error)
+        __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_get); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 759, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_t_6 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
           if (likely(__pyx_t_6)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
             __Pyx_INCREF(__pyx_t_6);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_7, function);
           }
         }
         __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 754, __pyx_L5_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 759, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_XDECREF_SET(__pyx_v_oldTxn, __pyx_t_2);
         __pyx_t_2 = 0;
 
-        /* "viur/datastore/transport.pyx":755
+        /* "viur/datastore/transport.pyx":760
  * 		try:
  * 			oldTxn = currentTransaction.get()
  * 			allowOverriding = kwargs.pop("__allowOverriding__", None)             # <<<<<<<<<<<<<<
  * 			if oldTxn:
  * 				if not allowOverriding:
  */
-        __pyx_t_2 = __Pyx_PyDict_Pop(__pyx_v_kwargs, __pyx_n_u_allowOverriding, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 755, __pyx_L5_error)
+        __pyx_t_2 = __Pyx_PyDict_Pop(__pyx_v_kwargs, __pyx_n_u_allowOverriding, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 760, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_XDECREF_SET(__pyx_v_allowOverriding, __pyx_t_2);
         __pyx_t_2 = 0;
 
-        /* "viur/datastore/transport.pyx":756
+        /* "viur/datastore/transport.pyx":761
  * 			oldTxn = currentTransaction.get()
  * 			allowOverriding = kwargs.pop("__allowOverriding__", None)
  * 			if oldTxn:             # <<<<<<<<<<<<<<
  * 				if not allowOverriding:
  * 					raise RecursionError("Cannot call runInTransaction while inside a transaction!")
  */
-        __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_oldTxn); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 756, __pyx_L5_error)
+        __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_oldTxn); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 761, __pyx_L5_error)
         if (__pyx_t_8) {
 
-          /* "viur/datastore/transport.pyx":757
+          /* "viur/datastore/transport.pyx":762
  * 			allowOverriding = kwargs.pop("__allowOverriding__", None)
  * 			if oldTxn:
  * 				if not allowOverriding:             # <<<<<<<<<<<<<<
  * 					raise RecursionError("Cannot call runInTransaction while inside a transaction!")
  * 				txnOptions = {
  */
-          __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_allowOverriding); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 757, __pyx_L5_error)
+          __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_allowOverriding); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 762, __pyx_L5_error)
           __pyx_t_9 = ((!__pyx_t_8) != 0);
           if (unlikely(__pyx_t_9)) {
 
-            /* "viur/datastore/transport.pyx":758
+            /* "viur/datastore/transport.pyx":763
  * 			if oldTxn:
  * 				if not allowOverriding:
  * 					raise RecursionError("Cannot call runInTransaction while inside a transaction!")             # <<<<<<<<<<<<<<
  * 				txnOptions = {
  * 					"previousTransaction": oldTxn["key"]
  */
-            __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_RecursionError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 758, __pyx_L5_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_RecursionError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 763, __pyx_L5_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 758, __pyx_L5_error)
+            __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 763, __pyx_L5_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_Raise(__pyx_t_7, 0, 0, 0);
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-            __PYX_ERR(0, 758, __pyx_L5_error)
+            __PYX_ERR(0, 763, __pyx_L5_error)
 
-            /* "viur/datastore/transport.pyx":757
+            /* "viur/datastore/transport.pyx":762
  * 			allowOverriding = kwargs.pop("__allowOverriding__", None)
  * 			if oldTxn:
  * 				if not allowOverriding:             # <<<<<<<<<<<<<<
  * 					raise RecursionError("Cannot call runInTransaction while inside a transaction!")
  * 				txnOptions = {
  */
           }
 
-          /* "viur/datastore/transport.pyx":760
+          /* "viur/datastore/transport.pyx":765
  * 					raise RecursionError("Cannot call runInTransaction while inside a transaction!")
  * 				txnOptions = {
  * 					"previousTransaction": oldTxn["key"]             # <<<<<<<<<<<<<<
  * 				}
  * 			else:
  */
-          __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 760, __pyx_L5_error)
+          __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 765, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_7);
-          __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_oldTxn, __pyx_n_u_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 760, __pyx_L5_error)
+          __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_v_oldTxn, __pyx_n_u_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 765, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
-          if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_previousTransaction, __pyx_t_2) < 0) __PYX_ERR(0, 760, __pyx_L5_error)
+          if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_previousTransaction, __pyx_t_2) < 0) __PYX_ERR(0, 765, __pyx_L5_error)
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_XDECREF_SET(__pyx_v_txnOptions, ((PyObject*)__pyx_t_7));
           __pyx_t_7 = 0;
 
-          /* "viur/datastore/transport.pyx":756
+          /* "viur/datastore/transport.pyx":761
  * 			oldTxn = currentTransaction.get()
  * 			allowOverriding = kwargs.pop("__allowOverriding__", None)
  * 			if oldTxn:             # <<<<<<<<<<<<<<
  * 				if not allowOverriding:
  * 					raise RecursionError("Cannot call runInTransaction while inside a transaction!")
  */
           goto __pyx_L13;
         }
 
-        /* "viur/datastore/transport.pyx":763
+        /* "viur/datastore/transport.pyx":768
  * 				}
  * 			else:
  * 				txnOptions = {}             # <<<<<<<<<<<<<<
  * 			postData = {
  * 				"transactionOptions": {
  */
         /*else*/ {
-          __pyx_t_7 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 763, __pyx_L5_error)
+          __pyx_t_7 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 768, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_XDECREF_SET(__pyx_v_txnOptions, ((PyObject*)__pyx_t_7));
           __pyx_t_7 = 0;
         }
         __pyx_L13:;
 
-        /* "viur/datastore/transport.pyx":765
+        /* "viur/datastore/transport.pyx":770
  * 				txnOptions = {}
  * 			postData = {
  * 				"transactionOptions": {             # <<<<<<<<<<<<<<
  * 					"readWrite": txnOptions
  * 				}
  */
-        __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 765, __pyx_L5_error)
+        __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 770, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_7);
 
-        /* "viur/datastore/transport.pyx":766
+        /* "viur/datastore/transport.pyx":771
  * 			postData = {
  * 				"transactionOptions": {
  * 					"readWrite": txnOptions             # <<<<<<<<<<<<<<
  * 				}
  * 			}
  */
-        __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 766, __pyx_L5_error)
+        __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 771, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_2);
-        if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_readWrite, __pyx_v_txnOptions) < 0) __PYX_ERR(0, 766, __pyx_L5_error)
-        if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_transactionOptions, __pyx_t_2) < 0) __PYX_ERR(0, 765, __pyx_L5_error)
+        if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_readWrite, __pyx_v_txnOptions) < 0) __PYX_ERR(0, 771, __pyx_L5_error)
+        if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_transactionOptions, __pyx_t_2) < 0) __PYX_ERR(0, 770, __pyx_L5_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF_SET(__pyx_v_postData, ((PyObject*)__pyx_t_7));
         __pyx_t_7 = 0;
 
-        /* "viur/datastore/transport.pyx":769
+        /* "viur/datastore/transport.pyx":774
  * 				}
  * 			}
  * 			req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 				url="https://datastore.googleapis.com/v1/projects/%s:beginTransaction" % projectID,
  * 				data=json.dumps(postData).encode("UTF-8"),
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 769, __pyx_L5_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 774, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_7);
 
-        /* "viur/datastore/transport.pyx":770
+        /* "viur/datastore/transport.pyx":775
  * 			}
  * 			req = authenticatedRequest(
  * 				url="https://datastore.googleapis.com/v1/projects/%s:beginTransaction" % projectID,             # <<<<<<<<<<<<<<
  * 				data=json.dumps(postData).encode("UTF-8"),
  * 			)
  */
-        __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 770, __pyx_L5_error)
+        __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 775, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_projectID); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 770, __pyx_L5_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_projectID); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 775, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_10 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_4, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 770, __pyx_L5_error)
+        __pyx_t_10 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_4, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 775, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_url, __pyx_t_10) < 0) __PYX_ERR(0, 770, __pyx_L5_error)
+        if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_url, __pyx_t_10) < 0) __PYX_ERR(0, 775, __pyx_L5_error)
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-        /* "viur/datastore/transport.pyx":771
+        /* "viur/datastore/transport.pyx":776
  * 			req = authenticatedRequest(
  * 				url="https://datastore.googleapis.com/v1/projects/%s:beginTransaction" % projectID,
  * 				data=json.dumps(postData).encode("UTF-8"),             # <<<<<<<<<<<<<<
  * 			)
  * 			if is_viur_datastore_request_ok(req):
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_json); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 771, __pyx_L5_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_json); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 776, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_dumps); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 771, __pyx_L5_error)
+        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_dumps); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 776, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __pyx_t_11 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
           __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_12);
           if (likely(__pyx_t_11)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
             __Pyx_INCREF(__pyx_t_11);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_12, function);
           }
         }
         __pyx_t_6 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_11, __pyx_v_postData) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_v_postData);
         __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 771, __pyx_L5_error)
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 776, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_encode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 771, __pyx_L5_error)
+        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_encode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 776, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_t_6 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_12);
           if (likely(__pyx_t_6)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
             __Pyx_INCREF(__pyx_t_6);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_12, function);
           }
         }
         __pyx_t_10 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_6, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_kp_u_UTF_8);
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 771, __pyx_L5_error)
+        if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 776, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_t_10) < 0) __PYX_ERR(0, 770, __pyx_L5_error)
+        if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_t_10) < 0) __PYX_ERR(0, 775, __pyx_L5_error)
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-        /* "viur/datastore/transport.pyx":769
+        /* "viur/datastore/transport.pyx":774
  * 				}
  * 			}
  * 			req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 				url="https://datastore.googleapis.com/v1/projects/%s:beginTransaction" % projectID,
  * 				data=json.dumps(postData).encode("UTF-8"),
  */
-        __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 769, __pyx_L5_error)
+        __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 774, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF_SET(__pyx_v_req, __pyx_t_10);
         __pyx_t_10 = 0;
 
-        /* "viur/datastore/transport.pyx":773
+        /* "viur/datastore/transport.pyx":778
  * 				data=json.dumps(postData).encode("UTF-8"),
  * 			)
  * 			if is_viur_datastore_request_ok(req):             # <<<<<<<<<<<<<<
  * 				txnKey = json.loads(req.content)["transaction"]
  * 				try:
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_is_viur_datastore_request_ok); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 773, __pyx_L5_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_is_viur_datastore_request_ok); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 778, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_7 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_7);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
         __pyx_t_10 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_7, __pyx_v_req) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_req);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 773, __pyx_L5_error)
+        if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 778, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 773, __pyx_L5_error)
+        __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 778, __pyx_L5_error)
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         if (__pyx_t_9) {
 
-          /* "viur/datastore/transport.pyx":774
+          /* "viur/datastore/transport.pyx":779
  * 			)
  * 			if is_viur_datastore_request_ok(req):
  * 				txnKey = json.loads(req.content)["transaction"]             # <<<<<<<<<<<<<<
  * 				try:
  * 					currentTxn = {"key": txnKey, "mutations": [], "affectedEntities": []}
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 774, __pyx_L5_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 779, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_loads); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 774, __pyx_L5_error)
+          __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_loads); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 779, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 774, __pyx_L5_error)
+          __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 779, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
           __pyx_t_12 = NULL;
           if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
             __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_7);
             if (likely(__pyx_t_12)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
               __Pyx_INCREF(__pyx_t_12);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_7, function);
             }
           }
           __pyx_t_10 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_12, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_2);
           __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-          if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 774, __pyx_L5_error)
+          if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 779, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_10);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-          __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_10, __pyx_n_u_transaction); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 774, __pyx_L5_error)
+          __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_10, __pyx_n_u_transaction); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 779, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
           __Pyx_XDECREF_SET(__pyx_v_txnKey, __pyx_t_7);
           __pyx_t_7 = 0;
 
-          /* "viur/datastore/transport.pyx":775
+          /* "viur/datastore/transport.pyx":780
  * 			if is_viur_datastore_request_ok(req):
  * 				txnKey = json.loads(req.content)["transaction"]
  * 				try:             # <<<<<<<<<<<<<<
  * 					currentTxn = {"key": txnKey, "mutations": [], "affectedEntities": []}
  * 					currentTransaction.set(currentTxn)
  */
           /*try:*/ {
 
-            /* "viur/datastore/transport.pyx":776
+            /* "viur/datastore/transport.pyx":781
  * 				txnKey = json.loads(req.content)["transaction"]
  * 				try:
  * 					currentTxn = {"key": txnKey, "mutations": [], "affectedEntities": []}             # <<<<<<<<<<<<<<
  * 					currentTransaction.set(currentTxn)
  * 					try:
  */
-            __pyx_t_7 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 776, __pyx_L19_error)
+            __pyx_t_7 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 781, __pyx_L19_error)
             __Pyx_GOTREF(__pyx_t_7);
-            if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_key, __pyx_v_txnKey) < 0) __PYX_ERR(0, 776, __pyx_L19_error)
-            __pyx_t_10 = PyList_New(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 776, __pyx_L19_error)
+            if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_key, __pyx_v_txnKey) < 0) __PYX_ERR(0, 781, __pyx_L19_error)
+            __pyx_t_10 = PyList_New(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 781, __pyx_L19_error)
             __Pyx_GOTREF(__pyx_t_10);
-            if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_mutations, __pyx_t_10) < 0) __PYX_ERR(0, 776, __pyx_L19_error)
+            if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_mutations, __pyx_t_10) < 0) __PYX_ERR(0, 781, __pyx_L19_error)
             __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-            __pyx_t_10 = PyList_New(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 776, __pyx_L19_error)
+            __pyx_t_10 = PyList_New(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 781, __pyx_L19_error)
             __Pyx_GOTREF(__pyx_t_10);
-            if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_affectedEntities, __pyx_t_10) < 0) __PYX_ERR(0, 776, __pyx_L19_error)
+            if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_affectedEntities, __pyx_t_10) < 0) __PYX_ERR(0, 781, __pyx_L19_error)
             __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
             __Pyx_XDECREF_SET(__pyx_v_currentTxn, ((PyObject*)__pyx_t_7));
             __pyx_t_7 = 0;
 
-            /* "viur/datastore/transport.pyx":777
+            /* "viur/datastore/transport.pyx":782
  * 				try:
  * 					currentTxn = {"key": txnKey, "mutations": [], "affectedEntities": []}
  * 					currentTransaction.set(currentTxn)             # <<<<<<<<<<<<<<
  * 					try:
  * 						res = callback(*args, **kwargs)
  */
-            __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 777, __pyx_L19_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 782, __pyx_L19_error)
             __Pyx_GOTREF(__pyx_t_10);
-            __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 777, __pyx_L19_error)
+            __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 782, __pyx_L19_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
             __pyx_t_10 = NULL;
             if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
               __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_2);
               if (likely(__pyx_t_10)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
                 __Pyx_INCREF(__pyx_t_10);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_2, function);
               }
             }
             __pyx_t_7 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_10, __pyx_v_currentTxn) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_currentTxn);
             __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-            if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 777, __pyx_L19_error)
+            if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 782, __pyx_L19_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-            /* "viur/datastore/transport.pyx":778
+            /* "viur/datastore/transport.pyx":783
  * 					currentTxn = {"key": txnKey, "mutations": [], "affectedEntities": []}
  * 					currentTransaction.set(currentTxn)
  * 					try:             # <<<<<<<<<<<<<<
  * 						res = callback(*args, **kwargs)
  * 					except:
  */
             {
@@ -12083,30 +12253,30 @@
               __Pyx_PyThreadState_assign
               __Pyx_ExceptionSave(&__pyx_t_13, &__pyx_t_14, &__pyx_t_15);
               __Pyx_XGOTREF(__pyx_t_13);
               __Pyx_XGOTREF(__pyx_t_14);
               __Pyx_XGOTREF(__pyx_t_15);
               /*try:*/ {
 
-                /* "viur/datastore/transport.pyx":779
+                /* "viur/datastore/transport.pyx":784
  * 					currentTransaction.set(currentTxn)
  * 					try:
  * 						res = callback(*args, **kwargs)             # <<<<<<<<<<<<<<
  * 					except:
  * 						_rollbackTxn(txnKey)
  */
-                __pyx_t_7 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 779, __pyx_L21_error)
+                __pyx_t_7 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 784, __pyx_L21_error)
                 __Pyx_GOTREF(__pyx_t_7);
-                __pyx_t_2 = __Pyx_PyObject_Call(__pyx_v_callback, __pyx_v_args, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 779, __pyx_L21_error)
+                __pyx_t_2 = __Pyx_PyObject_Call(__pyx_v_callback, __pyx_v_args, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 784, __pyx_L21_error)
                 __Pyx_GOTREF(__pyx_t_2);
                 __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
                 __Pyx_XDECREF_SET(__pyx_v_res, __pyx_t_2);
                 __pyx_t_2 = 0;
 
-                /* "viur/datastore/transport.pyx":778
+                /* "viur/datastore/transport.pyx":783
  * 					currentTxn = {"key": txnKey, "mutations": [], "affectedEntities": []}
  * 					currentTransaction.set(currentTxn)
  * 					try:             # <<<<<<<<<<<<<<
  * 						res = callback(*args, **kwargs)
  * 					except:
  */
               }
@@ -12118,717 +12288,717 @@
               __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
               __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
               __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
               __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
               __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
               __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-              /* "viur/datastore/transport.pyx":780
+              /* "viur/datastore/transport.pyx":785
  * 					try:
  * 						res = callback(*args, **kwargs)
  * 					except:             # <<<<<<<<<<<<<<
  * 						_rollbackTxn(txnKey)
  * 						raise
  */
               /*except:*/ {
                 __Pyx_AddTraceback("viur.datastore.transport.RunInTransaction", __pyx_clineno, __pyx_lineno, __pyx_filename);
-                if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_7, &__pyx_t_10) < 0) __PYX_ERR(0, 780, __pyx_L23_except_error)
+                if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_7, &__pyx_t_10) < 0) __PYX_ERR(0, 785, __pyx_L23_except_error)
                 __Pyx_GOTREF(__pyx_t_2);
                 __Pyx_GOTREF(__pyx_t_7);
                 __Pyx_GOTREF(__pyx_t_10);
 
-                /* "viur/datastore/transport.pyx":781
+                /* "viur/datastore/transport.pyx":786
  * 						res = callback(*args, **kwargs)
  * 					except:
  * 						_rollbackTxn(txnKey)             # <<<<<<<<<<<<<<
  * 						raise
  * 					if currentTxn["mutations"]:
  */
-                __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_rollbackTxn); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 781, __pyx_L23_except_error)
+                __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_rollbackTxn); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 786, __pyx_L23_except_error)
                 __Pyx_GOTREF(__pyx_t_6);
                 __pyx_t_11 = NULL;
                 if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
                   __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_6);
                   if (likely(__pyx_t_11)) {
                     PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
                     __Pyx_INCREF(__pyx_t_11);
                     __Pyx_INCREF(function);
                     __Pyx_DECREF_SET(__pyx_t_6, function);
                   }
                 }
                 __pyx_t_12 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_11, __pyx_v_txnKey) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_txnKey);
                 __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-                if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 781, __pyx_L23_except_error)
+                if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 786, __pyx_L23_except_error)
                 __Pyx_GOTREF(__pyx_t_12);
                 __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
                 __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-                /* "viur/datastore/transport.pyx":782
+                /* "viur/datastore/transport.pyx":787
  * 					except:
  * 						_rollbackTxn(txnKey)
  * 						raise             # <<<<<<<<<<<<<<
  * 					if currentTxn["mutations"]:
  * 						# Commit TXN
  */
                 __Pyx_GIVEREF(__pyx_t_2);
                 __Pyx_GIVEREF(__pyx_t_7);
                 __Pyx_XGIVEREF(__pyx_t_10);
                 __Pyx_ErrRestoreWithState(__pyx_t_2, __pyx_t_7, __pyx_t_10);
                 __pyx_t_2 = 0; __pyx_t_7 = 0; __pyx_t_10 = 0; 
-                __PYX_ERR(0, 782, __pyx_L23_except_error)
+                __PYX_ERR(0, 787, __pyx_L23_except_error)
               }
               __pyx_L23_except_error:;
 
-              /* "viur/datastore/transport.pyx":778
+              /* "viur/datastore/transport.pyx":783
  * 					currentTxn = {"key": txnKey, "mutations": [], "affectedEntities": []}
  * 					currentTransaction.set(currentTxn)
  * 					try:             # <<<<<<<<<<<<<<
  * 						res = callback(*args, **kwargs)
  * 					except:
  */
               __Pyx_XGIVEREF(__pyx_t_13);
               __Pyx_XGIVEREF(__pyx_t_14);
               __Pyx_XGIVEREF(__pyx_t_15);
               __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_14, __pyx_t_15);
               goto __pyx_L19_error;
               __pyx_L28_try_end:;
             }
 
-            /* "viur/datastore/transport.pyx":783
+            /* "viur/datastore/transport.pyx":788
  * 						_rollbackTxn(txnKey)
  * 						raise
  * 					if currentTxn["mutations"]:             # <<<<<<<<<<<<<<
  * 						# Commit TXN
  * 						postData = {
  */
-            __pyx_t_10 = __Pyx_PyDict_GetItem(__pyx_v_currentTxn, __pyx_n_u_mutations); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 783, __pyx_L19_error)
+            __pyx_t_10 = __Pyx_PyDict_GetItem(__pyx_v_currentTxn, __pyx_n_u_mutations); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 788, __pyx_L19_error)
             __Pyx_GOTREF(__pyx_t_10);
-            __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 783, __pyx_L19_error)
+            __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 788, __pyx_L19_error)
             __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
             if (__pyx_t_9) {
 
-              /* "viur/datastore/transport.pyx":786
+              /* "viur/datastore/transport.pyx":791
  * 						# Commit TXN
  * 						postData = {
  * 							"mode": "TRANSACTIONAL",  #             # <<<<<<<<<<<<<<
  * 							"transaction": txnKey,
  * 							"mutations": currentTxn["mutations"]
  */
-              __pyx_t_10 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 786, __pyx_L19_error)
+              __pyx_t_10 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 791, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_10);
-              if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_mode, __pyx_n_u_TRANSACTIONAL) < 0) __PYX_ERR(0, 786, __pyx_L19_error)
+              if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_mode, __pyx_n_u_TRANSACTIONAL) < 0) __PYX_ERR(0, 791, __pyx_L19_error)
 
-              /* "viur/datastore/transport.pyx":787
+              /* "viur/datastore/transport.pyx":792
  * 						postData = {
  * 							"mode": "TRANSACTIONAL",  #
  * 							"transaction": txnKey,             # <<<<<<<<<<<<<<
  * 							"mutations": currentTxn["mutations"]
  * 						}
  */
-              if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_transaction, __pyx_v_txnKey) < 0) __PYX_ERR(0, 786, __pyx_L19_error)
+              if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_transaction, __pyx_v_txnKey) < 0) __PYX_ERR(0, 791, __pyx_L19_error)
 
-              /* "viur/datastore/transport.pyx":788
+              /* "viur/datastore/transport.pyx":793
  * 							"mode": "TRANSACTIONAL",  #
  * 							"transaction": txnKey,
  * 							"mutations": currentTxn["mutations"]             # <<<<<<<<<<<<<<
  * 						}
  * 						req = authenticatedRequest(
  */
-              __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_currentTxn, __pyx_n_u_mutations); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 788, __pyx_L19_error)
+              __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_currentTxn, __pyx_n_u_mutations); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 793, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_7);
-              if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_mutations, __pyx_t_7) < 0) __PYX_ERR(0, 786, __pyx_L19_error)
+              if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_mutations, __pyx_t_7) < 0) __PYX_ERR(0, 791, __pyx_L19_error)
               __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
               __Pyx_DECREF_SET(__pyx_v_postData, ((PyObject*)__pyx_t_10));
               __pyx_t_10 = 0;
 
-              /* "viur/datastore/transport.pyx":790
+              /* "viur/datastore/transport.pyx":795
  * 							"mutations": currentTxn["mutations"]
  * 						}
  * 						req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 							url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,
  * 							data=json.dumps(postData).encode("UTF-8"),
  */
-              __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 790, __pyx_L19_error)
+              __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 795, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_10);
 
-              /* "viur/datastore/transport.pyx":791
+              /* "viur/datastore/transport.pyx":796
  * 						}
  * 						req = authenticatedRequest(
  * 							url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,             # <<<<<<<<<<<<<<
  * 							data=json.dumps(postData).encode("UTF-8"),
  * 						)
  */
-              __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 791, __pyx_L19_error)
+              __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 796, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_7);
-              __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_projectID); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 791, __pyx_L19_error)
+              __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_projectID); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 796, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_2);
-              __pyx_t_12 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_3, __pyx_t_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 791, __pyx_L19_error)
+              __pyx_t_12 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_3, __pyx_t_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 796, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_12);
               __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-              if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_url, __pyx_t_12) < 0) __PYX_ERR(0, 791, __pyx_L19_error)
+              if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_url, __pyx_t_12) < 0) __PYX_ERR(0, 796, __pyx_L19_error)
               __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-              /* "viur/datastore/transport.pyx":792
+              /* "viur/datastore/transport.pyx":797
  * 						req = authenticatedRequest(
  * 							url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,
  * 							data=json.dumps(postData).encode("UTF-8"),             # <<<<<<<<<<<<<<
  * 						)
  * 
  */
-              __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_json); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 792, __pyx_L19_error)
+              __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_json); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 797, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_6);
-              __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_dumps); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 792, __pyx_L19_error)
+              __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_dumps); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 797, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_11);
               __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
               __pyx_t_6 = NULL;
               if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
                 __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_11);
                 if (likely(__pyx_t_6)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
                   __Pyx_INCREF(__pyx_t_6);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_11, function);
                 }
               }
               __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_6, __pyx_v_postData) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_v_postData);
               __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-              if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 792, __pyx_L19_error)
+              if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 797, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_2);
               __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-              __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_encode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 792, __pyx_L19_error)
+              __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_encode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 797, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_11);
               __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
               __pyx_t_2 = NULL;
               if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
                 __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_11);
                 if (likely(__pyx_t_2)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
                   __Pyx_INCREF(__pyx_t_2);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_11, function);
                 }
               }
               __pyx_t_12 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_2, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_kp_u_UTF_8);
               __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-              if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 792, __pyx_L19_error)
+              if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 797, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_12);
               __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-              if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_data, __pyx_t_12) < 0) __PYX_ERR(0, 791, __pyx_L19_error)
+              if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_data, __pyx_t_12) < 0) __PYX_ERR(0, 796, __pyx_L19_error)
               __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-              /* "viur/datastore/transport.pyx":790
+              /* "viur/datastore/transport.pyx":795
  * 							"mutations": currentTxn["mutations"]
  * 						}
  * 						req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 							url="https://datastore.googleapis.com/v1/projects/%s:commit" % projectID,
  * 							data=json.dumps(postData).encode("UTF-8"),
  */
-              __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 790, __pyx_L19_error)
+              __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 795, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_12);
               __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
               __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
               __Pyx_DECREF_SET(__pyx_v_req, __pyx_t_12);
               __pyx_t_12 = 0;
 
-              /* "viur/datastore/transport.pyx":795
+              /* "viur/datastore/transport.pyx":800
  * 						)
  * 
  * 						is_viur_datastore_request_ok(req)             # <<<<<<<<<<<<<<
  * 						assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 						element = parser.parse(data_ptr, pysize, 1)
  */
-              __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_is_viur_datastore_request_ok); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 795, __pyx_L19_error)
+              __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_is_viur_datastore_request_ok); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 800, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_7);
               __pyx_t_10 = NULL;
               if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
                 __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_7);
                 if (likely(__pyx_t_10)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
                   __Pyx_INCREF(__pyx_t_10);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_7, function);
                 }
               }
               __pyx_t_12 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_10, __pyx_v_req) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_req);
               __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-              if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 795, __pyx_L19_error)
+              if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 800, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_12);
               __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
               __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-              /* "viur/datastore/transport.pyx":796
+              /* "viur/datastore/transport.pyx":801
  * 
  * 						is_viur_datastore_request_ok(req)
  * 						assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1             # <<<<<<<<<<<<<<
  * 						element = parser.parse(data_ptr, pysize, 1)
  * 						if (element.at_pointer("/mutationResults").error() != SUCCESS):
  */
               #ifndef CYTHON_WITHOUT_ASSERTIONS
               if (unlikely(!Py_OptimizeFlag)) {
-                __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 796, __pyx_L19_error)
+                __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 801, __pyx_L19_error)
                 __Pyx_GOTREF(__pyx_t_12);
-                __pyx_t_16 = PyBytes_AsStringAndSize(__pyx_t_12, (&__pyx_v_data_ptr), (&__pyx_v_pysize)); if (unlikely(__pyx_t_16 == ((int)-1))) __PYX_ERR(0, 796, __pyx_L19_error)
+                __pyx_t_16 = PyBytes_AsStringAndSize(__pyx_t_12, (&__pyx_v_data_ptr), (&__pyx_v_pysize)); if (unlikely(__pyx_t_16 == ((int)-1))) __PYX_ERR(0, 801, __pyx_L19_error)
                 __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
                 if (unlikely(!((__pyx_t_16 != -1L) != 0))) {
                   PyErr_SetNone(PyExc_AssertionError);
-                  __PYX_ERR(0, 796, __pyx_L19_error)
+                  __PYX_ERR(0, 801, __pyx_L19_error)
                 }
               }
               #endif
 
-              /* "viur/datastore/transport.pyx":797
+              /* "viur/datastore/transport.pyx":802
  * 						is_viur_datastore_request_ok(req)
  * 						assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 						element = parser.parse(data_ptr, pysize, 1)             # <<<<<<<<<<<<<<
  * 						if (element.at_pointer("/mutationResults").error() != SUCCESS):
  * 							pprint(req.content)
  */
               try {
                 __pyx_t_17 = __pyx_v_parser.parse(__pyx_v_data_ptr, __pyx_v_pysize, 1);
               } catch(...) {
                 __Pyx_CppExn2PyErr();
-                __PYX_ERR(0, 797, __pyx_L19_error)
+                __PYX_ERR(0, 802, __pyx_L19_error)
               }
               __pyx_v_element = __pyx_t_17;
 
-              /* "viur/datastore/transport.pyx":798
+              /* "viur/datastore/transport.pyx":803
  * 						assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 						element = parser.parse(data_ptr, pysize, 1)
  * 						if (element.at_pointer("/mutationResults").error() != SUCCESS):             # <<<<<<<<<<<<<<
  * 							pprint(req.content)
  * 							raise NoMutationResultsError("No mutation-results received")
  */
               __pyx_t_9 = ((__pyx_v_element.at_pointer(((char const *)"/mutationResults")).error() != simdjson::error_code::SUCCESS) != 0);
               if (unlikely(__pyx_t_9)) {
 
-                /* "viur/datastore/transport.pyx":799
+                /* "viur/datastore/transport.pyx":804
  * 						element = parser.parse(data_ptr, pysize, 1)
  * 						if (element.at_pointer("/mutationResults").error() != SUCCESS):
  * 							pprint(req.content)             # <<<<<<<<<<<<<<
  * 							raise NoMutationResultsError("No mutation-results received")
  * 						arrayElem = element.at_key("mutationResults").get_array()
  */
-                __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_pprint); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 799, __pyx_L19_error)
+                __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_pprint); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 804, __pyx_L19_error)
                 __Pyx_GOTREF(__pyx_t_7);
-                __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 799, __pyx_L19_error)
+                __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 804, __pyx_L19_error)
                 __Pyx_GOTREF(__pyx_t_10);
                 __pyx_t_11 = NULL;
                 if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
                   __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_7);
                   if (likely(__pyx_t_11)) {
                     PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
                     __Pyx_INCREF(__pyx_t_11);
                     __Pyx_INCREF(function);
                     __Pyx_DECREF_SET(__pyx_t_7, function);
                   }
                 }
                 __pyx_t_12 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_11, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_10);
                 __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
                 __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-                if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 799, __pyx_L19_error)
+                if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 804, __pyx_L19_error)
                 __Pyx_GOTREF(__pyx_t_12);
                 __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
                 __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-                /* "viur/datastore/transport.pyx":800
+                /* "viur/datastore/transport.pyx":805
  * 						if (element.at_pointer("/mutationResults").error() != SUCCESS):
  * 							pprint(req.content)
  * 							raise NoMutationResultsError("No mutation-results received")             # <<<<<<<<<<<<<<
  * 						arrayElem = element.at_key("mutationResults").get_array()
  * 						if arrayElem.size() != abs(len(currentTxn["affectedEntities"])):
  */
-                __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_NoMutationResultsError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 800, __pyx_L19_error)
+                __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_NoMutationResultsError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 805, __pyx_L19_error)
                 __Pyx_GOTREF(__pyx_t_7);
                 __pyx_t_10 = NULL;
                 if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
                   __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_7);
                   if (likely(__pyx_t_10)) {
                     PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
                     __Pyx_INCREF(__pyx_t_10);
                     __Pyx_INCREF(function);
                     __Pyx_DECREF_SET(__pyx_t_7, function);
                   }
                 }
                 __pyx_t_12 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_10, __pyx_kp_u_No_mutation_results_received_2) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u_No_mutation_results_received_2);
                 __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-                if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 800, __pyx_L19_error)
+                if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 805, __pyx_L19_error)
                 __Pyx_GOTREF(__pyx_t_12);
                 __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
                 __Pyx_Raise(__pyx_t_12, 0, 0, 0);
                 __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-                __PYX_ERR(0, 800, __pyx_L19_error)
+                __PYX_ERR(0, 805, __pyx_L19_error)
 
-                /* "viur/datastore/transport.pyx":798
+                /* "viur/datastore/transport.pyx":803
  * 						assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 						element = parser.parse(data_ptr, pysize, 1)
  * 						if (element.at_pointer("/mutationResults").error() != SUCCESS):             # <<<<<<<<<<<<<<
  * 							pprint(req.content)
  * 							raise NoMutationResultsError("No mutation-results received")
  */
               }
 
-              /* "viur/datastore/transport.pyx":801
+              /* "viur/datastore/transport.pyx":806
  * 							pprint(req.content)
  * 							raise NoMutationResultsError("No mutation-results received")
  * 						arrayElem = element.at_key("mutationResults").get_array()             # <<<<<<<<<<<<<<
  * 						if arrayElem.size() != abs(len(currentTxn["affectedEntities"])):
  * 							print(req.content)
  */
               try {
                 __pyx_t_17 = __pyx_v_element.at_key(((char const *)"mutationResults"));
               } catch(...) {
                 __Pyx_CppExn2PyErr();
-                __PYX_ERR(0, 801, __pyx_L19_error)
+                __PYX_ERR(0, 806, __pyx_L19_error)
               }
               try {
                 __pyx_t_18 = __pyx_t_17.get_array();
               } catch(...) {
                 __Pyx_CppExn2PyErr();
-                __PYX_ERR(0, 801, __pyx_L19_error)
+                __PYX_ERR(0, 806, __pyx_L19_error)
               }
               __pyx_v_arrayElem = __pyx_t_18;
 
-              /* "viur/datastore/transport.pyx":802
+              /* "viur/datastore/transport.pyx":807
  * 							raise NoMutationResultsError("No mutation-results received")
  * 						arrayElem = element.at_key("mutationResults").get_array()
  * 						if arrayElem.size() != abs(len(currentTxn["affectedEntities"])):             # <<<<<<<<<<<<<<
  * 							print(req.content)
  * 							raise ViurDatastoreError("Invalid number of mutation-results received")
  */
-              __pyx_t_12 = __Pyx_PyInt_From_int(__pyx_v_arrayElem.size()); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 802, __pyx_L19_error)
+              __pyx_t_12 = __Pyx_PyInt_From_int(__pyx_v_arrayElem.size()); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 807, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_12);
-              __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_currentTxn, __pyx_n_u_affectedEntities); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 802, __pyx_L19_error)
+              __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_currentTxn, __pyx_n_u_affectedEntities); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 807, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_7);
-              __pyx_t_19 = PyObject_Length(__pyx_t_7); if (unlikely(__pyx_t_19 == ((Py_ssize_t)-1))) __PYX_ERR(0, 802, __pyx_L19_error)
+              __pyx_t_19 = PyObject_Length(__pyx_t_7); if (unlikely(__pyx_t_19 == ((Py_ssize_t)-1))) __PYX_ERR(0, 807, __pyx_L19_error)
               __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-              __pyx_t_7 = PyInt_FromSsize_t(__pyx_t_19); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 802, __pyx_L19_error)
+              __pyx_t_7 = PyInt_FromSsize_t(__pyx_t_19); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 807, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_7);
-              __pyx_t_10 = __Pyx_PyNumber_Absolute(__pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 802, __pyx_L19_error)
+              __pyx_t_10 = __Pyx_PyNumber_Absolute(__pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 807, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_10);
               __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-              __pyx_t_7 = PyObject_RichCompare(__pyx_t_12, __pyx_t_10, Py_NE); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 802, __pyx_L19_error)
+              __pyx_t_7 = PyObject_RichCompare(__pyx_t_12, __pyx_t_10, Py_NE); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 807, __pyx_L19_error)
               __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
               __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-              __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 802, __pyx_L19_error)
+              __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 807, __pyx_L19_error)
               __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
               if (unlikely(__pyx_t_9)) {
 
-                /* "viur/datastore/transport.pyx":803
+                /* "viur/datastore/transport.pyx":808
  * 						arrayElem = element.at_key("mutationResults").get_array()
  * 						if arrayElem.size() != abs(len(currentTxn["affectedEntities"])):
  * 							print(req.content)             # <<<<<<<<<<<<<<
  * 							raise ViurDatastoreError("Invalid number of mutation-results received")
  * 						arrayIt = arrayElem.begin()
  */
-                __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 803, __pyx_L19_error)
+                __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 808, __pyx_L19_error)
                 __Pyx_GOTREF(__pyx_t_7);
-                __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 803, __pyx_L19_error)
+                __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 808, __pyx_L19_error)
                 __Pyx_GOTREF(__pyx_t_10);
                 __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
                 __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-                /* "viur/datastore/transport.pyx":804
+                /* "viur/datastore/transport.pyx":809
  * 						if arrayElem.size() != abs(len(currentTxn["affectedEntities"])):
  * 							print(req.content)
  * 							raise ViurDatastoreError("Invalid number of mutation-results received")             # <<<<<<<<<<<<<<
  * 						arrayIt = arrayElem.begin()
  * 						idx = 0
  */
-                __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_ViurDatastoreError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 804, __pyx_L19_error)
+                __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_ViurDatastoreError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 809, __pyx_L19_error)
                 __Pyx_GOTREF(__pyx_t_7);
                 __pyx_t_12 = NULL;
                 if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
                   __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_7);
                   if (likely(__pyx_t_12)) {
                     PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
                     __Pyx_INCREF(__pyx_t_12);
                     __Pyx_INCREF(function);
                     __Pyx_DECREF_SET(__pyx_t_7, function);
                   }
                 }
                 __pyx_t_10 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_12, __pyx_kp_u_Invalid_number_of_mutation_resul) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u_Invalid_number_of_mutation_resul);
                 __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-                if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 804, __pyx_L19_error)
+                if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 809, __pyx_L19_error)
                 __Pyx_GOTREF(__pyx_t_10);
                 __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
                 __Pyx_Raise(__pyx_t_10, 0, 0, 0);
                 __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-                __PYX_ERR(0, 804, __pyx_L19_error)
+                __PYX_ERR(0, 809, __pyx_L19_error)
 
-                /* "viur/datastore/transport.pyx":802
+                /* "viur/datastore/transport.pyx":807
  * 							raise NoMutationResultsError("No mutation-results received")
  * 						arrayElem = element.at_key("mutationResults").get_array()
  * 						if arrayElem.size() != abs(len(currentTxn["affectedEntities"])):             # <<<<<<<<<<<<<<
  * 							print(req.content)
  * 							raise ViurDatastoreError("Invalid number of mutation-results received")
  */
               }
 
-              /* "viur/datastore/transport.pyx":805
+              /* "viur/datastore/transport.pyx":810
  * 							print(req.content)
  * 							raise ViurDatastoreError("Invalid number of mutation-results received")
  * 						arrayIt = arrayElem.begin()             # <<<<<<<<<<<<<<
  * 						idx = 0
  * 						while arrayIt != arrayElem.end():
  */
               __pyx_v_arrayIt = __pyx_v_arrayElem.begin();
 
-              /* "viur/datastore/transport.pyx":806
+              /* "viur/datastore/transport.pyx":811
  * 							raise ViurDatastoreError("Invalid number of mutation-results received")
  * 						arrayIt = arrayElem.begin()
  * 						idx = 0             # <<<<<<<<<<<<<<
  * 						while arrayIt != arrayElem.end():
  * 							innerArrayElem = dereference(arrayIt)
  */
               __Pyx_INCREF(__pyx_int_0);
               __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_int_0);
 
-              /* "viur/datastore/transport.pyx":807
+              /* "viur/datastore/transport.pyx":812
  * 						arrayIt = arrayElem.begin()
  * 						idx = 0
  * 						while arrayIt != arrayElem.end():             # <<<<<<<<<<<<<<
  * 							innerArrayElem = dereference(arrayIt)
  * 							if innerArrayElem.at_pointer("/key").error() == SUCCESS:  # We got a new key assigned
  */
               while (1) {
                 __pyx_t_9 = ((__pyx_v_arrayIt != __pyx_v_arrayElem.end()) != 0);
                 if (!__pyx_t_9) break;
 
-                /* "viur/datastore/transport.pyx":808
+                /* "viur/datastore/transport.pyx":813
  * 						idx = 0
  * 						while arrayIt != arrayElem.end():
  * 							innerArrayElem = dereference(arrayIt)             # <<<<<<<<<<<<<<
  * 							if innerArrayElem.at_pointer("/key").error() == SUCCESS:  # We got a new key assigned
  * 								affectedEntity = currentTxn["affectedEntities"][idx]
  */
                 __pyx_v_innerArrayElem = (*__pyx_v_arrayIt);
 
-                /* "viur/datastore/transport.pyx":809
+                /* "viur/datastore/transport.pyx":814
  * 						while arrayIt != arrayElem.end():
  * 							innerArrayElem = dereference(arrayIt)
  * 							if innerArrayElem.at_pointer("/key").error() == SUCCESS:  # We got a new key assigned             # <<<<<<<<<<<<<<
  * 								affectedEntity = currentTxn["affectedEntities"][idx]
  * 								if not affectedEntity:
  */
                 __pyx_t_9 = ((__pyx_v_innerArrayElem.at_pointer(((char const *)"/key")).error() == simdjson::error_code::SUCCESS) != 0);
                 if (__pyx_t_9) {
 
-                  /* "viur/datastore/transport.pyx":810
+                  /* "viur/datastore/transport.pyx":815
  * 							innerArrayElem = dereference(arrayIt)
  * 							if innerArrayElem.at_pointer("/key").error() == SUCCESS:  # We got a new key assigned
  * 								affectedEntity = currentTxn["affectedEntities"][idx]             # <<<<<<<<<<<<<<
  * 								if not affectedEntity:
  * 									print(req.content)
  */
-                  __pyx_t_10 = __Pyx_PyDict_GetItem(__pyx_v_currentTxn, __pyx_n_u_affectedEntities); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 810, __pyx_L19_error)
+                  __pyx_t_10 = __Pyx_PyDict_GetItem(__pyx_v_currentTxn, __pyx_n_u_affectedEntities); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 815, __pyx_L19_error)
                   __Pyx_GOTREF(__pyx_t_10);
-                  __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_10, __pyx_v_idx); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 810, __pyx_L19_error)
+                  __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_10, __pyx_v_idx); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 815, __pyx_L19_error)
                   __Pyx_GOTREF(__pyx_t_7);
                   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
                   __Pyx_XDECREF_SET(__pyx_v_affectedEntity, __pyx_t_7);
                   __pyx_t_7 = 0;
 
-                  /* "viur/datastore/transport.pyx":811
+                  /* "viur/datastore/transport.pyx":816
  * 							if innerArrayElem.at_pointer("/key").error() == SUCCESS:  # We got a new key assigned
  * 								affectedEntity = currentTxn["affectedEntities"][idx]
  * 								if not affectedEntity:             # <<<<<<<<<<<<<<
  * 									print(req.content)
  * 									raise ViurDatastoreError("Received an unexpected key-update")
  */
-                  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_v_affectedEntity); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 811, __pyx_L19_error)
+                  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_v_affectedEntity); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 816, __pyx_L19_error)
                   __pyx_t_8 = ((!__pyx_t_9) != 0);
                   if (unlikely(__pyx_t_8)) {
 
-                    /* "viur/datastore/transport.pyx":812
+                    /* "viur/datastore/transport.pyx":817
  * 								affectedEntity = currentTxn["affectedEntities"][idx]
  * 								if not affectedEntity:
  * 									print(req.content)             # <<<<<<<<<<<<<<
  * 									raise ViurDatastoreError("Received an unexpected key-update")
  * 								affectedEntity.key = parseKey(innerArrayElem.at_key("key"))
  */
-                    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 812, __pyx_L19_error)
+                    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 817, __pyx_L19_error)
                     __Pyx_GOTREF(__pyx_t_7);
-                    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 812, __pyx_L19_error)
+                    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_print, __pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 817, __pyx_L19_error)
                     __Pyx_GOTREF(__pyx_t_10);
                     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
                     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-                    /* "viur/datastore/transport.pyx":813
+                    /* "viur/datastore/transport.pyx":818
  * 								if not affectedEntity:
  * 									print(req.content)
  * 									raise ViurDatastoreError("Received an unexpected key-update")             # <<<<<<<<<<<<<<
  * 								affectedEntity.key = parseKey(innerArrayElem.at_key("key"))
  * 								affectedEntity.version = toPyStr(innerArrayElem.at_key("version").get_string())
  */
-                    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_ViurDatastoreError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 813, __pyx_L19_error)
+                    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_ViurDatastoreError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 818, __pyx_L19_error)
                     __Pyx_GOTREF(__pyx_t_7);
                     __pyx_t_12 = NULL;
                     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
                       __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_7);
                       if (likely(__pyx_t_12)) {
                         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
                         __Pyx_INCREF(__pyx_t_12);
                         __Pyx_INCREF(function);
                         __Pyx_DECREF_SET(__pyx_t_7, function);
                       }
                     }
                     __pyx_t_10 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_12, __pyx_kp_u_Received_an_unexpected_key_updat) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u_Received_an_unexpected_key_updat);
                     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-                    if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 813, __pyx_L19_error)
+                    if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 818, __pyx_L19_error)
                     __Pyx_GOTREF(__pyx_t_10);
                     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
                     __Pyx_Raise(__pyx_t_10, 0, 0, 0);
                     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-                    __PYX_ERR(0, 813, __pyx_L19_error)
+                    __PYX_ERR(0, 818, __pyx_L19_error)
 
-                    /* "viur/datastore/transport.pyx":811
+                    /* "viur/datastore/transport.pyx":816
  * 							if innerArrayElem.at_pointer("/key").error() == SUCCESS:  # We got a new key assigned
  * 								affectedEntity = currentTxn["affectedEntities"][idx]
  * 								if not affectedEntity:             # <<<<<<<<<<<<<<
  * 									print(req.content)
  * 									raise ViurDatastoreError("Received an unexpected key-update")
  */
                   }
 
-                  /* "viur/datastore/transport.pyx":814
+                  /* "viur/datastore/transport.pyx":819
  * 									print(req.content)
  * 									raise ViurDatastoreError("Received an unexpected key-update")
  * 								affectedEntity.key = parseKey(innerArrayElem.at_key("key"))             # <<<<<<<<<<<<<<
  * 								affectedEntity.version = toPyStr(innerArrayElem.at_key("version").get_string())
  * 							preincrement(arrayIt)
  */
                   try {
                     __pyx_t_17 = __pyx_v_innerArrayElem.at_key(((char const *)"key"));
                   } catch(...) {
                     __Pyx_CppExn2PyErr();
-                    __PYX_ERR(0, 814, __pyx_L19_error)
+                    __PYX_ERR(0, 819, __pyx_L19_error)
                   }
-                  __pyx_t_10 = __pyx_f_4viur_9datastore_9transport_parseKey(__pyx_t_17); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 814, __pyx_L19_error)
+                  __pyx_t_10 = __pyx_f_4viur_9datastore_9transport_parseKey(__pyx_t_17); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 819, __pyx_L19_error)
                   __Pyx_GOTREF(__pyx_t_10);
-                  if (__Pyx_PyObject_SetAttrStr(__pyx_v_affectedEntity, __pyx_n_s_key, __pyx_t_10) < 0) __PYX_ERR(0, 814, __pyx_L19_error)
+                  if (__Pyx_PyObject_SetAttrStr(__pyx_v_affectedEntity, __pyx_n_s_key, __pyx_t_10) < 0) __PYX_ERR(0, 819, __pyx_L19_error)
                   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-                  /* "viur/datastore/transport.pyx":815
+                  /* "viur/datastore/transport.pyx":820
  * 									raise ViurDatastoreError("Received an unexpected key-update")
  * 								affectedEntity.key = parseKey(innerArrayElem.at_key("key"))
  * 								affectedEntity.version = toPyStr(innerArrayElem.at_key("version").get_string())             # <<<<<<<<<<<<<<
  * 							preincrement(arrayIt)
  * 							idx += 1
  */
                   try {
                     __pyx_t_17 = __pyx_v_innerArrayElem.at_key(((char const *)"version"));
                   } catch(...) {
                     __Pyx_CppExn2PyErr();
-                    __PYX_ERR(0, 815, __pyx_L19_error)
+                    __PYX_ERR(0, 820, __pyx_L19_error)
                   }
                   try {
                     __pyx_t_20 = __pyx_t_17.get_string();
                   } catch(...) {
                     __Pyx_CppExn2PyErr();
-                    __PYX_ERR(0, 815, __pyx_L19_error)
+                    __PYX_ERR(0, 820, __pyx_L19_error)
                   }
-                  __pyx_t_10 = __pyx_f_4viur_9datastore_9transport_toPyStr(__pyx_t_20); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 815, __pyx_L19_error)
+                  __pyx_t_10 = __pyx_f_4viur_9datastore_9transport_toPyStr(__pyx_t_20); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 820, __pyx_L19_error)
                   __Pyx_GOTREF(__pyx_t_10);
-                  if (__Pyx_PyObject_SetAttrStr(__pyx_v_affectedEntity, __pyx_n_s_version, __pyx_t_10) < 0) __PYX_ERR(0, 815, __pyx_L19_error)
+                  if (__Pyx_PyObject_SetAttrStr(__pyx_v_affectedEntity, __pyx_n_s_version, __pyx_t_10) < 0) __PYX_ERR(0, 820, __pyx_L19_error)
                   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-                  /* "viur/datastore/transport.pyx":809
+                  /* "viur/datastore/transport.pyx":814
  * 						while arrayIt != arrayElem.end():
  * 							innerArrayElem = dereference(arrayIt)
  * 							if innerArrayElem.at_pointer("/key").error() == SUCCESS:  # We got a new key assigned             # <<<<<<<<<<<<<<
  * 								affectedEntity = currentTxn["affectedEntities"][idx]
  * 								if not affectedEntity:
  */
                 }
 
-                /* "viur/datastore/transport.pyx":816
+                /* "viur/datastore/transport.pyx":821
  * 								affectedEntity.key = parseKey(innerArrayElem.at_key("key"))
  * 								affectedEntity.version = toPyStr(innerArrayElem.at_key("version").get_string())
  * 							preincrement(arrayIt)             # <<<<<<<<<<<<<<
  * 							idx += 1
  * 						return res
  */
                 (void)((++__pyx_v_arrayIt));
 
-                /* "viur/datastore/transport.pyx":817
+                /* "viur/datastore/transport.pyx":822
  * 								affectedEntity.version = toPyStr(innerArrayElem.at_key("version").get_string())
  * 							preincrement(arrayIt)
  * 							idx += 1             # <<<<<<<<<<<<<<
  * 						return res
  * 					else:  # No changes have been made - free txn
  */
-                __pyx_t_10 = __Pyx_PyInt_AddObjC(__pyx_v_idx, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 817, __pyx_L19_error)
+                __pyx_t_10 = __Pyx_PyInt_AddObjC(__pyx_v_idx, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 822, __pyx_L19_error)
                 __Pyx_GOTREF(__pyx_t_10);
                 __Pyx_DECREF_SET(__pyx_v_idx, __pyx_t_10);
                 __pyx_t_10 = 0;
               }
 
-              /* "viur/datastore/transport.pyx":818
+              /* "viur/datastore/transport.pyx":823
  * 							preincrement(arrayIt)
  * 							idx += 1
  * 						return res             # <<<<<<<<<<<<<<
  * 					else:  # No changes have been made - free txn
  * 						_rollbackTxn(txnKey)
  */
               __Pyx_XDECREF(__pyx_r);
               __Pyx_INCREF(__pyx_v_res);
               __pyx_r = __pyx_v_res;
               goto __pyx_L18_return;
 
-              /* "viur/datastore/transport.pyx":783
+              /* "viur/datastore/transport.pyx":788
  * 						_rollbackTxn(txnKey)
  * 						raise
  * 					if currentTxn["mutations"]:             # <<<<<<<<<<<<<<
  * 						# Commit TXN
  * 						postData = {
  */
             }
 
-            /* "viur/datastore/transport.pyx":820
+            /* "viur/datastore/transport.pyx":825
  * 						return res
  * 					else:  # No changes have been made - free txn
  * 						_rollbackTxn(txnKey)             # <<<<<<<<<<<<<<
  * 						return res
  * 				finally:  # Ensure, currentTransaction is always set back to none
  */
             /*else*/ {
-              __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_rollbackTxn); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 820, __pyx_L19_error)
+              __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_rollbackTxn); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 825, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_7);
               __pyx_t_12 = NULL;
               if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
                 __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_7);
                 if (likely(__pyx_t_12)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
                   __Pyx_INCREF(__pyx_t_12);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_7, function);
                 }
               }
               __pyx_t_10 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_12, __pyx_v_txnKey) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_txnKey);
               __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-              if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 820, __pyx_L19_error)
+              if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 825, __pyx_L19_error)
               __Pyx_GOTREF(__pyx_t_10);
               __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
               __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-              /* "viur/datastore/transport.pyx":821
+              /* "viur/datastore/transport.pyx":826
  * 					else:  # No changes have been made - free txn
  * 						_rollbackTxn(txnKey)
  * 						return res             # <<<<<<<<<<<<<<
  * 				finally:  # Ensure, currentTransaction is always set back to none
  * 					currentTransaction.set(None)
  */
               __Pyx_XDECREF(__pyx_r);
               __Pyx_INCREF(__pyx_v_res);
               __pyx_r = __pyx_v_res;
               goto __pyx_L18_return;
             }
           }
 
-          /* "viur/datastore/transport.pyx":823
+          /* "viur/datastore/transport.pyx":828
  * 						return res
  * 				finally:  # Ensure, currentTransaction is always set back to none
  * 					currentTransaction.set(None)             # <<<<<<<<<<<<<<
  * 		except CollisionError:  # Got a collision; retry the entire transaction
  * 			sleep(2 ** exponential_backoff)
  */
           /*finally:*/ {
@@ -12849,32 +13019,32 @@
               __Pyx_XGOTREF(__pyx_t_14);
               __Pyx_XGOTREF(__pyx_t_13);
               __Pyx_XGOTREF(__pyx_t_23);
               __Pyx_XGOTREF(__pyx_t_24);
               __Pyx_XGOTREF(__pyx_t_25);
               __pyx_t_16 = __pyx_lineno; __pyx_t_21 = __pyx_clineno; __pyx_t_22 = __pyx_filename;
               {
-                __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 823, __pyx_L41_error)
+                __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 828, __pyx_L41_error)
                 __Pyx_GOTREF(__pyx_t_7);
-                __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_set); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 823, __pyx_L41_error)
+                __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_set); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 828, __pyx_L41_error)
                 __Pyx_GOTREF(__pyx_t_12);
                 __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
                 __pyx_t_7 = NULL;
                 if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
                   __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_12);
                   if (likely(__pyx_t_7)) {
                     PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
                     __Pyx_INCREF(__pyx_t_7);
                     __Pyx_INCREF(function);
                     __Pyx_DECREF_SET(__pyx_t_12, function);
                   }
                 }
                 __pyx_t_10 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_7, Py_None) : __Pyx_PyObject_CallOneArg(__pyx_t_12, Py_None);
                 __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-                if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 823, __pyx_L41_error)
+                if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 828, __pyx_L41_error)
                 __Pyx_GOTREF(__pyx_t_10);
                 __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
                 __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
               }
               if (PY_MAJOR_VERSION >= 3) {
                 __Pyx_XGIVEREF(__pyx_t_23);
                 __Pyx_XGIVEREF(__pyx_t_24);
@@ -12900,51 +13070,51 @@
               __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
               __pyx_t_23 = 0; __pyx_t_24 = 0; __pyx_t_25 = 0;
               goto __pyx_L5_error;
             }
             __pyx_L18_return: {
               __pyx_t_25 = __pyx_r;
               __pyx_r = 0;
-              __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 823, __pyx_L5_error)
+              __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_currentTransaction); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 828, __pyx_L5_error)
               __Pyx_GOTREF(__pyx_t_12);
-              __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_set); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 823, __pyx_L5_error)
+              __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_set); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 828, __pyx_L5_error)
               __Pyx_GOTREF(__pyx_t_7);
               __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
               __pyx_t_12 = NULL;
               if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
                 __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_7);
                 if (likely(__pyx_t_12)) {
                   PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
                   __Pyx_INCREF(__pyx_t_12);
                   __Pyx_INCREF(function);
                   __Pyx_DECREF_SET(__pyx_t_7, function);
                 }
               }
               __pyx_t_10 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_12, Py_None) : __Pyx_PyObject_CallOneArg(__pyx_t_7, Py_None);
               __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-              if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 823, __pyx_L5_error)
+              if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 828, __pyx_L5_error)
               __Pyx_GOTREF(__pyx_t_10);
               __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
               __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
               __pyx_r = __pyx_t_25;
               __pyx_t_25 = 0;
               goto __pyx_L9_try_return;
             }
           }
 
-          /* "viur/datastore/transport.pyx":773
+          /* "viur/datastore/transport.pyx":778
  * 				data=json.dumps(postData).encode("UTF-8"),
  * 			)
  * 			if is_viur_datastore_request_ok(req):             # <<<<<<<<<<<<<<
  * 				txnKey = json.loads(req.content)["transaction"]
  * 				try:
  */
         }
 
-        /* "viur/datastore/transport.pyx":753
+        /* "viur/datastore/transport.pyx":758
  * 	cdef simdjsonArray.iterator arrayIt
  * 	for exponential_backoff in range(1, 4):
  * 		try:             # <<<<<<<<<<<<<<
  * 			oldTxn = currentTransaction.get()
  * 			allowOverriding = kwargs.pop("__allowOverriding__", None)
  */
       }
@@ -12956,72 +13126,72 @@
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "viur/datastore/transport.pyx":824
+      /* "viur/datastore/transport.pyx":829
  * 				finally:  # Ensure, currentTransaction is always set back to none
  * 					currentTransaction.set(None)
  * 		except CollisionError:  # Got a collision; retry the entire transaction             # <<<<<<<<<<<<<<
  * 			sleep(2 ** exponential_backoff)
  * 	raise CollisionError("All retries are exhausted for this transaction") # If we made it here, all tries are exhausted
  */
       __Pyx_ErrFetch(&__pyx_t_10, &__pyx_t_7, &__pyx_t_12);
-      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_CollisionError); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 824, __pyx_L7_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_CollisionError); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 829, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_11);
       __pyx_t_21 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_10, __pyx_t_11);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_ErrRestore(__pyx_t_10, __pyx_t_7, __pyx_t_12);
       __pyx_t_10 = 0; __pyx_t_7 = 0; __pyx_t_12 = 0;
       if (__pyx_t_21) {
         __Pyx_AddTraceback("viur.datastore.transport.RunInTransaction", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_12, &__pyx_t_7, &__pyx_t_10) < 0) __PYX_ERR(0, 824, __pyx_L7_except_error)
+        if (__Pyx_GetException(&__pyx_t_12, &__pyx_t_7, &__pyx_t_10) < 0) __PYX_ERR(0, 829, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_10);
 
-        /* "viur/datastore/transport.pyx":825
+        /* "viur/datastore/transport.pyx":830
  * 					currentTransaction.set(None)
  * 		except CollisionError:  # Got a collision; retry the entire transaction
  * 			sleep(2 ** exponential_backoff)             # <<<<<<<<<<<<<<
  * 	raise CollisionError("All retries are exhausted for this transaction") # If we made it here, all tries are exhausted
  * 
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_sleep); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 825, __pyx_L7_except_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_sleep); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 830, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_6 = __Pyx_PyNumber_PowerOf2(__pyx_int_2, __pyx_v_exponential_backoff, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 825, __pyx_L7_except_error)
+        __pyx_t_6 = __Pyx_PyNumber_PowerOf2(__pyx_int_2, __pyx_v_exponential_backoff, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 830, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_26 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_26 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_26)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_26);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
         __pyx_t_11 = (__pyx_t_26) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_26, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_6);
         __Pyx_XDECREF(__pyx_t_26); __pyx_t_26 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 825, __pyx_L7_except_error)
+        if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 830, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         goto __pyx_L6_exception_handled;
       }
       goto __pyx_L7_except_error;
       __pyx_L7_except_error:;
 
-      /* "viur/datastore/transport.pyx":753
+      /* "viur/datastore/transport.pyx":758
  * 	cdef simdjsonArray.iterator arrayIt
  * 	for exponential_backoff in range(1, 4):
  * 		try:             # <<<<<<<<<<<<<<
  * 			oldTxn = currentTransaction.get()
  * 			allowOverriding = kwargs.pop("__allowOverriding__", None)
  */
       __Pyx_XGIVEREF(__pyx_t_3);
@@ -13040,43 +13210,43 @@
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       __pyx_L12_try_end:;
     }
   }
 
-  /* "viur/datastore/transport.pyx":826
+  /* "viur/datastore/transport.pyx":831
  * 		except CollisionError:  # Got a collision; retry the entire transaction
  * 			sleep(2 ** exponential_backoff)
  * 	raise CollisionError("All retries are exhausted for this transaction") # If we made it here, all tries are exhausted             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_CollisionError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 826, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_CollisionError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 831, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_12 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_12)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_12);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_10 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_12, __pyx_kp_u_All_retries_are_exhausted_for_th) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_kp_u_All_retries_are_exhausted_for_th);
   __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 826, __pyx_L1_error)
+  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 831, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_Raise(__pyx_t_10, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __PYX_ERR(0, 826, __pyx_L1_error)
+  __PYX_ERR(0, 831, __pyx_L1_error)
 
-  /* "viur/datastore/transport.pyx":737
+  /* "viur/datastore/transport.pyx":742
  * 
  * 
  * def RunInTransaction(callback: callable, *args, **kwargs) -> Any:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Runs the given function inside a AID transaction.
  */
 
@@ -13104,15 +13274,15 @@
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XDECREF(__pyx_v_affectedEntity);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viur/datastore/transport.pyx":829
+/* "viur/datastore/transport.pyx":834
  * 
  * 
  * def _rollbackTxn(txnKey: str):             # <<<<<<<<<<<<<<
  * 	"""
  * 		Internal helper that aborts the given transaction. It's important to abort pending transactions (instead
  */
 
@@ -13123,15 +13293,15 @@
 static PyObject *__pyx_pw_4viur_9datastore_9transport_17_rollbackTxn(PyObject *__pyx_self, PyObject *__pyx_v_txnKey) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_rollbackTxn (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_txnKey), (&PyUnicode_Type), 1, "txnKey", 1))) __PYX_ERR(0, 829, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_txnKey), (&PyUnicode_Type), 1, "txnKey", 1))) __PYX_ERR(0, 834, __pyx_L1_error)
   __pyx_r = __pyx_pf_4viur_9datastore_9transport_16_rollbackTxn(__pyx_self, ((PyObject*)__pyx_v_txnKey));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -13151,117 +13321,117 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_rollbackTxn", 0);
 
-  /* "viur/datastore/transport.pyx":838
+  /* "viur/datastore/transport.pyx":843
  * 	"""
  * 	postData = {
  * 		"transaction": txnKey             # <<<<<<<<<<<<<<
  * 	}
  * 	req = authenticatedRequest(
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 838, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 843, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_transaction, __pyx_v_txnKey) < 0) __PYX_ERR(0, 838, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_transaction, __pyx_v_txnKey) < 0) __PYX_ERR(0, 843, __pyx_L1_error)
   __pyx_v_postData = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "viur/datastore/transport.pyx":840
+  /* "viur/datastore/transport.pyx":845
  * 		"transaction": txnKey
  * 	}
  * 	req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 		url="https://datastore.googleapis.com/v1/projects/%s:rollback" % projectID,
  * 		data=json.dumps(postData).encode("UTF-8"),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 840, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 845, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "viur/datastore/transport.pyx":841
+  /* "viur/datastore/transport.pyx":846
  * 	}
  * 	req = authenticatedRequest(
  * 		url="https://datastore.googleapis.com/v1/projects/%s:rollback" % projectID,             # <<<<<<<<<<<<<<
  * 		data=json.dumps(postData).encode("UTF-8"),
  * 	)
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 841, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 846, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_projectID); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 841, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_projectID); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 846, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_5, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 841, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_5, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 846, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_url, __pyx_t_4) < 0) __PYX_ERR(0, 841, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_url, __pyx_t_4) < 0) __PYX_ERR(0, 846, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":842
+  /* "viur/datastore/transport.pyx":847
  * 	req = authenticatedRequest(
  * 		url="https://datastore.googleapis.com/v1/projects/%s:rollback" % projectID,
  * 		data=json.dumps(postData).encode("UTF-8"),             # <<<<<<<<<<<<<<
  * 	)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 842, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_json); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 847, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_dumps); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 842, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_dumps); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 847, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_v_postData) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_postData);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 842, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 847, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 842, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 847, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
     }
   }
   __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_3, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_kp_u_UTF_8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 842, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 847, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_t_4) < 0) __PYX_ERR(0, 841, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_data, __pyx_t_4) < 0) __PYX_ERR(0, 846, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":840
+  /* "viur/datastore/transport.pyx":845
  * 		"transaction": txnKey
  * 	}
  * 	req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 		url="https://datastore.googleapis.com/v1/projects/%s:rollback" % projectID,
  * 		data=json.dumps(postData).encode("UTF-8"),
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 840, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 845, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_req = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":829
+  /* "viur/datastore/transport.pyx":834
  * 
  * 
  * def _rollbackTxn(txnKey: str):             # <<<<<<<<<<<<<<
  * 	"""
  * 		Internal helper that aborts the given transaction. It's important to abort pending transactions (instead
  */
 
@@ -13281,15 +13451,15 @@
   __Pyx_XDECREF(__pyx_v_postData);
   __Pyx_XDECREF(__pyx_v_req);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viur/datastore/transport.pyx":845
+/* "viur/datastore/transport.pyx":850
  * 	)
  * 
  * def AllocateIDs(keys: Union[Key, List[Key]]) -> Union[Key, List[Key]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Allocates numeric IDs for the keys given.
  */
 
@@ -13341,195 +13511,195 @@
   int __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("AllocateIDs", 0);
   __Pyx_INCREF(__pyx_v_keys);
 
-  /* "viur/datastore/transport.pyx":853
+  /* "viur/datastore/transport.pyx":858
  * 			be allocated immediately, even if the transaction aborts.
  * 	"""
  * 	cdef simdjsonParser parser = simdjsonParser()             # <<<<<<<<<<<<<<
  * 	cdef Py_ssize_t pysize
  * 	cdef char * data_ptr
  */
   __pyx_v_parser = simdjson::dom::parser();
 
-  /* "viur/datastore/transport.pyx":857
+  /* "viur/datastore/transport.pyx":862
  * 	cdef char * data_ptr
  * 	cdef simdjsonElement element
  * 	isMulti = True             # <<<<<<<<<<<<<<
  * 	if isinstance(keys, Key):
  * 		keys = [keys]
  */
   __pyx_v_isMulti = 1;
 
-  /* "viur/datastore/transport.pyx":858
+  /* "viur/datastore/transport.pyx":863
  * 	cdef simdjsonElement element
  * 	isMulti = True
  * 	if isinstance(keys, Key):             # <<<<<<<<<<<<<<
  * 		keys = [keys]
  * 		isMulti = False
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 858, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Key); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 863, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_keys, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 858, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_keys, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 863, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "viur/datastore/transport.pyx":859
+    /* "viur/datastore/transport.pyx":864
  * 	isMulti = True
  * 	if isinstance(keys, Key):
  * 		keys = [keys]             # <<<<<<<<<<<<<<
  * 		isMulti = False
  * 	keyList = [
  */
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 859, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 864, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_keys);
     __Pyx_GIVEREF(__pyx_v_keys);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_v_keys);
     __Pyx_DECREF_SET(__pyx_v_keys, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "viur/datastore/transport.pyx":860
+    /* "viur/datastore/transport.pyx":865
  * 	if isinstance(keys, Key):
  * 		keys = [keys]
  * 		isMulti = False             # <<<<<<<<<<<<<<
  * 	keyList = [
  * 		{
  */
     __pyx_v_isMulti = 0;
 
-    /* "viur/datastore/transport.pyx":858
+    /* "viur/datastore/transport.pyx":863
  * 	cdef simdjsonElement element
  * 	isMulti = True
  * 	if isinstance(keys, Key):             # <<<<<<<<<<<<<<
  * 		keys = [keys]
  * 		isMulti = False
  */
   }
 
-  /* "viur/datastore/transport.pyx":861
+  /* "viur/datastore/transport.pyx":866
  * 		keys = [keys]
  * 		isMulti = False
  * 	keyList = [             # <<<<<<<<<<<<<<
  * 		{
  * 			"partitionId": {
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 861, __pyx_L6_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 866, __pyx_L6_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "viur/datastore/transport.pyx":868
+    /* "viur/datastore/transport.pyx":873
  * 			"path": keyToPath(x)
  * 		}
  * 		for x in keys]             # <<<<<<<<<<<<<<
  * 
  * 	requestedKeys = keyList[:300]
  */
     if (likely(PyList_CheckExact(__pyx_v_keys)) || PyTuple_CheckExact(__pyx_v_keys)) {
       __pyx_t_4 = __pyx_v_keys; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_keys); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 868, __pyx_L6_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_keys); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 873, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 868, __pyx_L6_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 873, __pyx_L6_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 868, __pyx_L6_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 873, __pyx_L6_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 868, __pyx_L6_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 873, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 868, __pyx_L6_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 873, __pyx_L6_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 868, __pyx_L6_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 873, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 868, __pyx_L6_error)
+            else __PYX_ERR(0, 873, __pyx_L6_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_9genexpr10__pyx_v_x, __pyx_t_7);
       __pyx_t_7 = 0;
 
-      /* "viur/datastore/transport.pyx":863
+      /* "viur/datastore/transport.pyx":868
  * 	keyList = [
  * 		{
  * 			"partitionId": {             # <<<<<<<<<<<<<<
  * 				"project_id": projectID,
  * 			},
  */
-      __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 863, __pyx_L6_error)
+      __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 868, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "viur/datastore/transport.pyx":864
+      /* "viur/datastore/transport.pyx":869
  * 		{
  * 			"partitionId": {
  * 				"project_id": projectID,             # <<<<<<<<<<<<<<
  * 			},
  * 			"path": keyToPath(x)
  */
-      __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 864, __pyx_L6_error)
+      __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 869, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_projectID); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 864, __pyx_L6_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_projectID); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 869, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_9);
-      if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_project_id, __pyx_t_9) < 0) __PYX_ERR(0, 864, __pyx_L6_error)
+      if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_project_id, __pyx_t_9) < 0) __PYX_ERR(0, 869, __pyx_L6_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_partitionId, __pyx_t_8) < 0) __PYX_ERR(0, 863, __pyx_L6_error)
+      if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_partitionId, __pyx_t_8) < 0) __PYX_ERR(0, 868, __pyx_L6_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "viur/datastore/transport.pyx":866
+      /* "viur/datastore/transport.pyx":871
  * 				"project_id": projectID,
  * 			},
  * 			"path": keyToPath(x)             # <<<<<<<<<<<<<<
  * 		}
  * 		for x in keys]
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_keyToPath); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 866, __pyx_L6_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_keyToPath); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 871, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_10 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_10)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
           __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_9, function);
         }
       }
       __pyx_t_8 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_10, __pyx_9genexpr10__pyx_v_x) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_9genexpr10__pyx_v_x);
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 866, __pyx_L6_error)
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 871, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_path, __pyx_t_8) < 0) __PYX_ERR(0, 863, __pyx_L6_error)
+      if (PyDict_SetItem(__pyx_t_7, __pyx_n_u_path, __pyx_t_8) < 0) __PYX_ERR(0, 868, __pyx_L6_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 861, __pyx_L6_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_7))) __PYX_ERR(0, 866, __pyx_L6_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "viur/datastore/transport.pyx":868
+      /* "viur/datastore/transport.pyx":873
  * 			"path": keyToPath(x)
  * 		}
  * 		for x in keys]             # <<<<<<<<<<<<<<
  * 
  * 	requestedKeys = keyList[:300]
  */
     }
@@ -13540,446 +13710,446 @@
     __Pyx_XDECREF(__pyx_9genexpr10__pyx_v_x); __pyx_9genexpr10__pyx_v_x = 0;
     goto __pyx_L1_error;
     __pyx_L9_exit_scope:;
   } /* exit inner scope */
   __pyx_v_keyList = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "viur/datastore/transport.pyx":870
+  /* "viur/datastore/transport.pyx":875
  * 		for x in keys]
  * 
  * 	requestedKeys = keyList[:300]             # <<<<<<<<<<<<<<
  * 	postData = {
  * 		"keys": requestedKeys,
  */
-  __pyx_t_1 = __Pyx_PyList_GetSlice(__pyx_v_keyList, 0, 0x12C); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 870, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyList_GetSlice(__pyx_v_keyList, 0, 0x12C); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 875, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_requestedKeys = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "viur/datastore/transport.pyx":872
+  /* "viur/datastore/transport.pyx":877
  * 	requestedKeys = keyList[:300]
  * 	postData = {
  * 		"keys": requestedKeys,             # <<<<<<<<<<<<<<
  * 	}
  * 	req = authenticatedRequest(
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 872, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 877, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_keys, __pyx_v_requestedKeys) < 0) __PYX_ERR(0, 872, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_keys, __pyx_v_requestedKeys) < 0) __PYX_ERR(0, 877, __pyx_L1_error)
   __pyx_v_postData = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "viur/datastore/transport.pyx":874
+  /* "viur/datastore/transport.pyx":879
  * 		"keys": requestedKeys,
  * 	}
  * 	req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 		url="https://datastore.googleapis.com/v1/projects/%s:allocateIds" % projectID,
  * 		data=json.dumps(postData).encode("UTF-8"),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 874, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 879, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "viur/datastore/transport.pyx":875
+  /* "viur/datastore/transport.pyx":880
  * 	}
  * 	req = authenticatedRequest(
  * 		url="https://datastore.googleapis.com/v1/projects/%s:allocateIds" % projectID,             # <<<<<<<<<<<<<<
  * 		data=json.dumps(postData).encode("UTF-8"),
  * 	)
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 875, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 880, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_projectID); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 875, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_projectID); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 880, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_6, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 875, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_6, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 880, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_url, __pyx_t_8) < 0) __PYX_ERR(0, 875, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_url, __pyx_t_8) < 0) __PYX_ERR(0, 880, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "viur/datastore/transport.pyx":876
+  /* "viur/datastore/transport.pyx":881
  * 	req = authenticatedRequest(
  * 		url="https://datastore.googleapis.com/v1/projects/%s:allocateIds" % projectID,
  * 		data=json.dumps(postData).encode("UTF-8"),             # <<<<<<<<<<<<<<
  * 	)
  * 	assert req.status_code == 200
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_json); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 876, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_json); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 881, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_dumps); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 876, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_dumps); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 881, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __pyx_t_9 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_9)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
       __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_10, function);
     }
   }
   __pyx_t_7 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_9, __pyx_v_postData) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_v_postData);
   __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 876, __pyx_L1_error)
+  if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 881, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_encode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 876, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_encode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 881, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_10, function);
     }
   }
   __pyx_t_8 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_7, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_kp_u_UTF_8);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 876, __pyx_L1_error)
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 881, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_data, __pyx_t_8) < 0) __PYX_ERR(0, 875, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_data, __pyx_t_8) < 0) __PYX_ERR(0, 880, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "viur/datastore/transport.pyx":874
+  /* "viur/datastore/transport.pyx":879
  * 		"keys": requestedKeys,
  * 	}
  * 	req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 		url="https://datastore.googleapis.com/v1/projects/%s:allocateIds" % projectID,
  * 		data=json.dumps(postData).encode("UTF-8"),
  */
-  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 874, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 879, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_req = __pyx_t_8;
   __pyx_t_8 = 0;
 
-  /* "viur/datastore/transport.pyx":878
+  /* "viur/datastore/transport.pyx":883
  * 		data=json.dumps(postData).encode("UTF-8"),
  * 	)
  * 	assert req.status_code == 200             # <<<<<<<<<<<<<<
  * 	assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 	element = parser.parse(data_ptr, pysize, 1)
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_status_code); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 878, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_status_code); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 883, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_t_8, __pyx_int_200, 0xC8, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 878, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_t_8, __pyx_int_200, 0xC8, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 883, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 878, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 883, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_3)) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 878, __pyx_L1_error)
+      __PYX_ERR(0, 883, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "viur/datastore/transport.pyx":879
+  /* "viur/datastore/transport.pyx":884
  * 	)
  * 	assert req.status_code == 200
  * 	assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1             # <<<<<<<<<<<<<<
  * 	element = parser.parse(data_ptr, pysize, 1)
  * 	res = []
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 879, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 884, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_11 = PyBytes_AsStringAndSize(__pyx_t_4, (&__pyx_v_data_ptr), (&__pyx_v_pysize)); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 879, __pyx_L1_error)
+    __pyx_t_11 = PyBytes_AsStringAndSize(__pyx_t_4, (&__pyx_v_data_ptr), (&__pyx_v_pysize)); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 884, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!((__pyx_t_11 != -1L) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 879, __pyx_L1_error)
+      __PYX_ERR(0, 884, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "viur/datastore/transport.pyx":880
+  /* "viur/datastore/transport.pyx":885
  * 	assert req.status_code == 200
  * 	assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 	element = parser.parse(data_ptr, pysize, 1)             # <<<<<<<<<<<<<<
  * 	res = []
  * 	if (element.at_pointer("/keys").error() == SUCCESS):
  */
   try {
     __pyx_t_12 = __pyx_v_parser.parse(__pyx_v_data_ptr, __pyx_v_pysize, 1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 880, __pyx_L1_error)
+    __PYX_ERR(0, 885, __pyx_L1_error)
   }
   __pyx_v_element = __pyx_t_12;
 
-  /* "viur/datastore/transport.pyx":881
+  /* "viur/datastore/transport.pyx":886
  * 	assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 	element = parser.parse(data_ptr, pysize, 1)
  * 	res = []             # <<<<<<<<<<<<<<
  * 	if (element.at_pointer("/keys").error() == SUCCESS):
  * 		arrayElem = element.at_key("keys").get_array()
  */
-  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 881, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 886, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_v_res = ((PyObject*)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":882
+  /* "viur/datastore/transport.pyx":887
  * 	element = parser.parse(data_ptr, pysize, 1)
  * 	res = []
  * 	if (element.at_pointer("/keys").error() == SUCCESS):             # <<<<<<<<<<<<<<
  * 		arrayElem = element.at_key("keys").get_array()
  * 		arrayIt = arrayElem.begin()
  */
   __pyx_t_3 = ((__pyx_v_element.at_pointer(((char const *)"/keys")).error() == simdjson::error_code::SUCCESS) != 0);
   if (likely(__pyx_t_3)) {
 
-    /* "viur/datastore/transport.pyx":883
+    /* "viur/datastore/transport.pyx":888
  * 	res = []
  * 	if (element.at_pointer("/keys").error() == SUCCESS):
  * 		arrayElem = element.at_key("keys").get_array()             # <<<<<<<<<<<<<<
  * 		arrayIt = arrayElem.begin()
  * 		while arrayIt != arrayElem.end():
  */
     try {
       __pyx_t_12 = __pyx_v_element.at_key(((char const *)"keys"));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 883, __pyx_L1_error)
+      __PYX_ERR(0, 888, __pyx_L1_error)
     }
     try {
       __pyx_t_13 = __pyx_t_12.get_array();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 883, __pyx_L1_error)
+      __PYX_ERR(0, 888, __pyx_L1_error)
     }
     __pyx_v_arrayElem = __pyx_t_13;
 
-    /* "viur/datastore/transport.pyx":884
+    /* "viur/datastore/transport.pyx":889
  * 	if (element.at_pointer("/keys").error() == SUCCESS):
  * 		arrayElem = element.at_key("keys").get_array()
  * 		arrayIt = arrayElem.begin()             # <<<<<<<<<<<<<<
  * 		while arrayIt != arrayElem.end():
  * 			innerArrayElem = dereference(arrayIt)
  */
     __pyx_v_arrayIt = __pyx_v_arrayElem.begin();
 
-    /* "viur/datastore/transport.pyx":885
+    /* "viur/datastore/transport.pyx":890
  * 		arrayElem = element.at_key("keys").get_array()
  * 		arrayIt = arrayElem.begin()
  * 		while arrayIt != arrayElem.end():             # <<<<<<<<<<<<<<
  * 			innerArrayElem = dereference(arrayIt)
  * 			res.append( parseKey(innerArrayElem))
  */
     while (1) {
       __pyx_t_3 = ((__pyx_v_arrayIt != __pyx_v_arrayElem.end()) != 0);
       if (!__pyx_t_3) break;
 
-      /* "viur/datastore/transport.pyx":886
+      /* "viur/datastore/transport.pyx":891
  * 		arrayIt = arrayElem.begin()
  * 		while arrayIt != arrayElem.end():
  * 			innerArrayElem = dereference(arrayIt)             # <<<<<<<<<<<<<<
  * 			res.append( parseKey(innerArrayElem))
  * 			preincrement(arrayIt)
  */
       __pyx_v_innerArrayElem = (*__pyx_v_arrayIt);
 
-      /* "viur/datastore/transport.pyx":887
+      /* "viur/datastore/transport.pyx":892
  * 		while arrayIt != arrayElem.end():
  * 			innerArrayElem = dereference(arrayIt)
  * 			res.append( parseKey(innerArrayElem))             # <<<<<<<<<<<<<<
  * 			preincrement(arrayIt)
  * 		if not res:
  */
-      __pyx_t_4 = __pyx_f_4viur_9datastore_9transport_parseKey(__pyx_v_innerArrayElem); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 887, __pyx_L1_error)
+      __pyx_t_4 = __pyx_f_4viur_9datastore_9transport_parseKey(__pyx_v_innerArrayElem); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 892, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_res, __pyx_t_4); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 887, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyList_Append(__pyx_v_res, __pyx_t_4); if (unlikely(__pyx_t_14 == ((int)-1))) __PYX_ERR(0, 892, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "viur/datastore/transport.pyx":888
+      /* "viur/datastore/transport.pyx":893
  * 			innerArrayElem = dereference(arrayIt)
  * 			res.append( parseKey(innerArrayElem))
  * 			preincrement(arrayIt)             # <<<<<<<<<<<<<<
  * 		if not res:
  * 			raise ValueError("Empty response received from Datastore API")
  */
       (void)((++__pyx_v_arrayIt));
     }
 
-    /* "viur/datastore/transport.pyx":889
+    /* "viur/datastore/transport.pyx":894
  * 			res.append( parseKey(innerArrayElem))
  * 			preincrement(arrayIt)
  * 		if not res:             # <<<<<<<<<<<<<<
  * 			raise ValueError("Empty response received from Datastore API")
  * 		elif not isMulti:
  */
     __pyx_t_3 = (PyList_GET_SIZE(__pyx_v_res) != 0);
     __pyx_t_2 = ((!__pyx_t_3) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "viur/datastore/transport.pyx":890
+      /* "viur/datastore/transport.pyx":895
  * 			preincrement(arrayIt)
  * 		if not res:
  * 			raise ValueError("Empty response received from Datastore API")             # <<<<<<<<<<<<<<
  * 		elif not isMulti:
  * 			return res[0]
  */
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 890, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 895, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 890, __pyx_L1_error)
+      __PYX_ERR(0, 895, __pyx_L1_error)
 
-      /* "viur/datastore/transport.pyx":889
+      /* "viur/datastore/transport.pyx":894
  * 			res.append( parseKey(innerArrayElem))
  * 			preincrement(arrayIt)
  * 		if not res:             # <<<<<<<<<<<<<<
  * 			raise ValueError("Empty response received from Datastore API")
  * 		elif not isMulti:
  */
     }
 
-    /* "viur/datastore/transport.pyx":891
+    /* "viur/datastore/transport.pyx":896
  * 		if not res:
  * 			raise ValueError("Empty response received from Datastore API")
  * 		elif not isMulti:             # <<<<<<<<<<<<<<
  * 			return res[0]
  * 		else:
  */
     __pyx_t_2 = ((!(__pyx_v_isMulti != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "viur/datastore/transport.pyx":892
+      /* "viur/datastore/transport.pyx":897
  * 			raise ValueError("Empty response received from Datastore API")
  * 		elif not isMulti:
  * 			return res[0]             # <<<<<<<<<<<<<<
  * 		else:
  * 			return res
  */
       __Pyx_XDECREF(__pyx_r);
-      __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_res, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 892, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt_List(__pyx_v_res, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 897, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_r = __pyx_t_4;
       __pyx_t_4 = 0;
       goto __pyx_L0;
 
-      /* "viur/datastore/transport.pyx":891
+      /* "viur/datastore/transport.pyx":896
  * 		if not res:
  * 			raise ValueError("Empty response received from Datastore API")
  * 		elif not isMulti:             # <<<<<<<<<<<<<<
  * 			return res[0]
  * 		else:
  */
     }
 
-    /* "viur/datastore/transport.pyx":894
+    /* "viur/datastore/transport.pyx":899
  * 			return res[0]
  * 		else:
  * 			return res             # <<<<<<<<<<<<<<
  * 	else:
  * 		logging.error("Invalid data received from Datastore API")
  */
     /*else*/ {
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(__pyx_v_res);
       __pyx_r = __pyx_v_res;
       goto __pyx_L0;
     }
 
-    /* "viur/datastore/transport.pyx":882
+    /* "viur/datastore/transport.pyx":887
  * 	element = parser.parse(data_ptr, pysize, 1)
  * 	res = []
  * 	if (element.at_pointer("/keys").error() == SUCCESS):             # <<<<<<<<<<<<<<
  * 		arrayElem = element.at_key("keys").get_array()
  * 		arrayIt = arrayElem.begin()
  */
   }
 
-  /* "viur/datastore/transport.pyx":896
+  /* "viur/datastore/transport.pyx":901
  * 			return res
  * 	else:
  * 		logging.error("Invalid data received from Datastore API")             # <<<<<<<<<<<<<<
  * 		logging.error(req.content)
  * 		raise ValueError("Invalid data received from Datastore API")
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_logging); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 896, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_logging); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 901, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 896, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 901, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_8, __pyx_kp_u_Invalid_data_received_from_Datas) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_u_Invalid_data_received_from_Datas);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 896, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 901, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "viur/datastore/transport.pyx":897
+    /* "viur/datastore/transport.pyx":902
  * 	else:
  * 		logging.error("Invalid data received from Datastore API")
  * 		logging.error(req.content)             # <<<<<<<<<<<<<<
  * 		raise ValueError("Invalid data received from Datastore API")
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logging); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 897, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_logging); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 902, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_error); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 897, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_error); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 902, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 897, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 902, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_10 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_8, function);
       }
     }
     __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_10, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_1);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 897, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 902, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "viur/datastore/transport.pyx":898
+    /* "viur/datastore/transport.pyx":903
  * 		logging.error("Invalid data received from Datastore API")
  * 		logging.error(req.content)
  * 		raise ValueError("Invalid data received from Datastore API")             # <<<<<<<<<<<<<<
  * 
  * def Count(kind: str = None, up_to= 2 ** 63 - 1, queryDefinition: QueryDefinition = None) -> Union[Key, List[Key]]:
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 898, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 903, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 898, __pyx_L1_error)
+    __PYX_ERR(0, 903, __pyx_L1_error)
   }
 
-  /* "viur/datastore/transport.pyx":845
+  /* "viur/datastore/transport.pyx":850
  * 	)
  * 
  * def AllocateIDs(keys: Union[Key, List[Key]]) -> Union[Key, List[Key]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Allocates numeric IDs for the keys given.
  */
 
@@ -14002,15 +14172,15 @@
   __Pyx_XDECREF(__pyx_9genexpr10__pyx_v_x);
   __Pyx_XDECREF(__pyx_v_keys);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "viur/datastore/transport.pyx":900
+/* "viur/datastore/transport.pyx":905
  * 		raise ValueError("Invalid data received from Datastore API")
  * 
  * def Count(kind: str = None, up_to= 2 ** 63 - 1, queryDefinition: QueryDefinition = None) -> Union[Key, List[Key]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Count all entries in a kind if there is only a kind is provided
  */
 
@@ -14064,15 +14234,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_queryDefinition);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "Count") < 0)) __PYX_ERR(0, 900, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "Count") < 0)) __PYX_ERR(0, 905, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -14084,21 +14254,21 @@
     }
     __pyx_v_kind = ((PyObject*)values[0]);
     __pyx_v_up_to = values[1];
     __pyx_v_queryDefinition = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("Count", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 900, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("Count", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 905, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("viur.datastore.transport.Count", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kind), (&PyUnicode_Type), 1, "kind", 1))) __PYX_ERR(0, 900, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kind), (&PyUnicode_Type), 1, "kind", 1))) __PYX_ERR(0, 905, __pyx_L1_error)
   __pyx_r = __pyx_pf_4viur_9datastore_9transport_20Count(__pyx_self, __pyx_v_kind, __pyx_v_up_to, __pyx_v_queryDefinition);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -14141,952 +14311,952 @@
   simdjson::dom::element __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("Count", 0);
   __Pyx_INCREF(__pyx_v_kind);
 
-  /* "viur/datastore/transport.pyx":912
+  /* "viur/datastore/transport.pyx":917
  * 			be allocated immediately, even if the transaction aborts.
  * 	"""
  * 	cdef simdjsonParser parser = simdjsonParser()             # <<<<<<<<<<<<<<
  * 	cdef Py_ssize_t pysize
  * 	cdef char * data_ptr
  */
   __pyx_v_parser = simdjson::dom::parser();
 
-  /* "viur/datastore/transport.pyx":918
+  /* "viur/datastore/transport.pyx":923
  * 	cdef simdjsonElement element_inner
  * 	cdef simdjsonArray array_element, array_element_inner
  * 	logging.warning("The 'Count() aggregation' query is a technical preview and cannot be guaranteed to work at this time!!!")             # <<<<<<<<<<<<<<
  * 	if not kind:
  * 		kind = queryDefinition.kind
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 918, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logging); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 923, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_warning); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 918, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_warning); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 923, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_kp_u_The_Count_aggregation_query_is_a) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_The_Count_aggregation_query_is_a);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 918, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 923, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "viur/datastore/transport.pyx":919
+  /* "viur/datastore/transport.pyx":924
  * 	cdef simdjsonArray array_element, array_element_inner
  * 	logging.warning("The 'Count() aggregation' query is a technical preview and cannot be guaranteed to work at this time!!!")
  * 	if not kind:             # <<<<<<<<<<<<<<
  * 		kind = queryDefinition.kind
  * 
  */
   __pyx_t_4 = (__pyx_v_kind != Py_None)&&(__Pyx_PyUnicode_IS_TRUE(__pyx_v_kind) != 0);
   __pyx_t_5 = ((!__pyx_t_4) != 0);
   if (__pyx_t_5) {
 
-    /* "viur/datastore/transport.pyx":920
+    /* "viur/datastore/transport.pyx":925
  * 	logging.warning("The 'Count() aggregation' query is a technical preview and cannot be guaranteed to work at this time!!!")
  * 	if not kind:
  * 		kind = queryDefinition.kind             # <<<<<<<<<<<<<<
  * 
  * 	post_data = {
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_kind); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 920, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_kind); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 925, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 920, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 925, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_kind, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "viur/datastore/transport.pyx":919
+    /* "viur/datastore/transport.pyx":924
  * 	cdef simdjsonArray array_element, array_element_inner
  * 	logging.warning("The 'Count() aggregation' query is a technical preview and cannot be guaranteed to work at this time!!!")
  * 	if not kind:             # <<<<<<<<<<<<<<
  * 		kind = queryDefinition.kind
  * 
  */
   }
 
-  /* "viur/datastore/transport.pyx":924
+  /* "viur/datastore/transport.pyx":929
  * 	post_data = {
  * 
  * 		"partitionId": {             # <<<<<<<<<<<<<<
  * 			"project_id": projectID,
  * 		}, "aggregation_query": {
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 924, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 929, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "viur/datastore/transport.pyx":925
+  /* "viur/datastore/transport.pyx":930
  * 
  * 		"partitionId": {
  * 			"project_id": projectID,             # <<<<<<<<<<<<<<
  * 		}, "aggregation_query": {
  * 			"aggregations": {"count": {"up_to": up_to}},
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 925, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 930, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_projectID); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 925, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_projectID); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 930, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_project_id, __pyx_t_2) < 0) __PYX_ERR(0, 925, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_project_id, __pyx_t_2) < 0) __PYX_ERR(0, 930, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_partitionId, __pyx_t_3) < 0) __PYX_ERR(0, 924, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_partitionId, __pyx_t_3) < 0) __PYX_ERR(0, 929, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "viur/datastore/transport.pyx":927
+  /* "viur/datastore/transport.pyx":932
  * 			"project_id": projectID,
  * 		}, "aggregation_query": {
  * 			"aggregations": {"count": {"up_to": up_to}},             # <<<<<<<<<<<<<<
  * 			"nested_query": {"kind": [{"name": kind}]}
  * 		},
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 927, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 927, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 927, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_up_to, __pyx_v_up_to) < 0) __PYX_ERR(0, 927, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_count, __pyx_t_6) < 0) __PYX_ERR(0, 927, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_up_to, __pyx_v_up_to) < 0) __PYX_ERR(0, 932, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_count, __pyx_t_6) < 0) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_aggregations, __pyx_t_2) < 0) __PYX_ERR(0, 927, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_aggregations, __pyx_t_2) < 0) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "viur/datastore/transport.pyx":928
+  /* "viur/datastore/transport.pyx":933
  * 		}, "aggregation_query": {
  * 			"aggregations": {"count": {"up_to": up_to}},
  * 			"nested_query": {"kind": [{"name": kind}]}             # <<<<<<<<<<<<<<
  * 		},
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 928, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 933, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 928, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 933, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_name, __pyx_v_kind) < 0) __PYX_ERR(0, 928, __pyx_L1_error)
-  __pyx_t_7 = PyList_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 928, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_name, __pyx_v_kind) < 0) __PYX_ERR(0, 933, __pyx_L1_error)
+  __pyx_t_7 = PyList_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 933, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_6);
   PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_kind, __pyx_t_7) < 0) __PYX_ERR(0, 928, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_kind, __pyx_t_7) < 0) __PYX_ERR(0, 933, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_nested_query, __pyx_t_2) < 0) __PYX_ERR(0, 927, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_nested_query, __pyx_t_2) < 0) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_aggregation_query, __pyx_t_3) < 0) __PYX_ERR(0, 924, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_aggregation_query, __pyx_t_3) < 0) __PYX_ERR(0, 929, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_post_data = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "viur/datastore/transport.pyx":932
+  /* "viur/datastore/transport.pyx":937
  * 
  * 	}
  * 	if queryDefinition:             # <<<<<<<<<<<<<<
  * 		if queryDefinition.filters:
  * 			filterList = []
  */
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_queryDefinition); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 932, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_queryDefinition); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 937, __pyx_L1_error)
   if (__pyx_t_5) {
 
-    /* "viur/datastore/transport.pyx":933
+    /* "viur/datastore/transport.pyx":938
  * 	}
  * 	if queryDefinition:
  * 		if queryDefinition.filters:             # <<<<<<<<<<<<<<
  * 			filterList = []
  * 			for k, v in queryDefinition.filters.items():
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_filters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 933, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_filters); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 938, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 933, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 938, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (__pyx_t_5) {
 
-      /* "viur/datastore/transport.pyx":934
+      /* "viur/datastore/transport.pyx":939
  * 	if queryDefinition:
  * 		if queryDefinition.filters:
  * 			filterList = []             # <<<<<<<<<<<<<<
  * 			for k, v in queryDefinition.filters.items():
  * 				key, op = k.split(" ")
  */
-      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 934, __pyx_L1_error)
+      __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 939, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_v_filterList = ((PyObject*)__pyx_t_1);
       __pyx_t_1 = 0;
 
-      /* "viur/datastore/transport.pyx":935
+      /* "viur/datastore/transport.pyx":940
  * 		if queryDefinition.filters:
  * 			filterList = []
  * 			for k, v in queryDefinition.filters.items():             # <<<<<<<<<<<<<<
  * 				key, op = k.split(" ")
  * 				if op == "=":
  */
       __pyx_t_8 = 0;
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_filters); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 935, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_queryDefinition, __pyx_n_s_filters); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 940, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       if (unlikely(__pyx_t_3 == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-        __PYX_ERR(0, 935, __pyx_L1_error)
+        __PYX_ERR(0, 940, __pyx_L1_error)
       }
-      __pyx_t_2 = __Pyx_dict_iterator(__pyx_t_3, 0, __pyx_n_s_items, (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 935, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_dict_iterator(__pyx_t_3, 0, __pyx_n_s_items, (&__pyx_t_9), (&__pyx_t_10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 940, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_t_1);
       __pyx_t_1 = __pyx_t_2;
       __pyx_t_2 = 0;
       while (1) {
         __pyx_t_11 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_9, &__pyx_t_8, &__pyx_t_2, &__pyx_t_3, NULL, __pyx_t_10);
         if (unlikely(__pyx_t_11 == 0)) break;
-        if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 935, __pyx_L1_error)
+        if (unlikely(__pyx_t_11 == -1)) __PYX_ERR(0, 940, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_3);
         __pyx_t_3 = 0;
 
-        /* "viur/datastore/transport.pyx":936
+        /* "viur/datastore/transport.pyx":941
  * 			filterList = []
  * 			for k, v in queryDefinition.filters.items():
  * 				key, op = k.split(" ")             # <<<<<<<<<<<<<<
  * 				if op == "=":
  * 					op = "EQUAL"
  */
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_k, __pyx_n_s_split); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 936, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_k, __pyx_n_s_split); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 941, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_7 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_7)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_7);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
         __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_7, __pyx_kp_u__5) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u__5);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 936, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 941, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
           PyObject* sequence = __pyx_t_3;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 936, __pyx_L1_error)
+            __PYX_ERR(0, 941, __pyx_L1_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
             __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
             __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
           } else {
             __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
             __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
           }
           __Pyx_INCREF(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_7);
           #else
-          __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 936, __pyx_L1_error)
+          __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 941, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 936, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 941, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 936, __pyx_L1_error)
+          __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 941, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __pyx_t_12 = Py_TYPE(__pyx_t_6)->tp_iternext;
           index = 0; __pyx_t_2 = __pyx_t_12(__pyx_t_6); if (unlikely(!__pyx_t_2)) goto __pyx_L8_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_2);
           index = 1; __pyx_t_7 = __pyx_t_12(__pyx_t_6); if (unlikely(!__pyx_t_7)) goto __pyx_L8_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_7);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_6), 2) < 0) __PYX_ERR(0, 936, __pyx_L1_error)
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_12(__pyx_t_6), 2) < 0) __PYX_ERR(0, 941, __pyx_L1_error)
           __pyx_t_12 = NULL;
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           goto __pyx_L9_unpacking_done;
           __pyx_L8_unpacking_failed:;
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_12 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 936, __pyx_L1_error)
+          __PYX_ERR(0, 941, __pyx_L1_error)
           __pyx_L9_unpacking_done:;
         }
         __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_XDECREF_SET(__pyx_v_op, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "viur/datastore/transport.pyx":937
+        /* "viur/datastore/transport.pyx":942
  * 			for k, v in queryDefinition.filters.items():
  * 				key, op = k.split(" ")
  * 				if op == "=":             # <<<<<<<<<<<<<<
  * 					op = "EQUAL"
  * 				elif op == "<":
  */
-        __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_op, __pyx_kp_u__6, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 937, __pyx_L1_error)
+        __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_op, __pyx_kp_u__6, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 942, __pyx_L1_error)
         if (__pyx_t_5) {
 
-          /* "viur/datastore/transport.pyx":938
+          /* "viur/datastore/transport.pyx":943
  * 				key, op = k.split(" ")
  * 				if op == "=":
  * 					op = "EQUAL"             # <<<<<<<<<<<<<<
  * 				elif op == "<":
  * 					op = "LESS_THAN"
  */
           __Pyx_INCREF(__pyx_n_u_EQUAL);
           __Pyx_DECREF_SET(__pyx_v_op, __pyx_n_u_EQUAL);
 
-          /* "viur/datastore/transport.pyx":937
+          /* "viur/datastore/transport.pyx":942
  * 			for k, v in queryDefinition.filters.items():
  * 				key, op = k.split(" ")
  * 				if op == "=":             # <<<<<<<<<<<<<<
  * 					op = "EQUAL"
  * 				elif op == "<":
  */
           goto __pyx_L10;
         }
 
-        /* "viur/datastore/transport.pyx":939
+        /* "viur/datastore/transport.pyx":944
  * 				if op == "=":
  * 					op = "EQUAL"
  * 				elif op == "<":             # <<<<<<<<<<<<<<
  * 					op = "LESS_THAN"
  * 				elif op == "<=":
  */
-        __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_op, __pyx_kp_u__7, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 939, __pyx_L1_error)
+        __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_op, __pyx_kp_u__7, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 944, __pyx_L1_error)
         if (__pyx_t_5) {
 
-          /* "viur/datastore/transport.pyx":940
+          /* "viur/datastore/transport.pyx":945
  * 					op = "EQUAL"
  * 				elif op == "<":
  * 					op = "LESS_THAN"             # <<<<<<<<<<<<<<
  * 				elif op == "<=":
  * 					op = "LESS_THAN_OR_EQUAL"
  */
           __Pyx_INCREF(__pyx_n_u_LESS_THAN);
           __Pyx_DECREF_SET(__pyx_v_op, __pyx_n_u_LESS_THAN);
 
-          /* "viur/datastore/transport.pyx":939
+          /* "viur/datastore/transport.pyx":944
  * 				if op == "=":
  * 					op = "EQUAL"
  * 				elif op == "<":             # <<<<<<<<<<<<<<
  * 					op = "LESS_THAN"
  * 				elif op == "<=":
  */
           goto __pyx_L10;
         }
 
-        /* "viur/datastore/transport.pyx":941
+        /* "viur/datastore/transport.pyx":946
  * 				elif op == "<":
  * 					op = "LESS_THAN"
  * 				elif op == "<=":             # <<<<<<<<<<<<<<
  * 					op = "LESS_THAN_OR_EQUAL"
  * 				elif op == ">":
  */
-        __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_op, __pyx_kp_u__8, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 941, __pyx_L1_error)
+        __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_op, __pyx_kp_u__8, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 946, __pyx_L1_error)
         if (__pyx_t_5) {
 
-          /* "viur/datastore/transport.pyx":942
+          /* "viur/datastore/transport.pyx":947
  * 					op = "LESS_THAN"
  * 				elif op == "<=":
  * 					op = "LESS_THAN_OR_EQUAL"             # <<<<<<<<<<<<<<
  * 				elif op == ">":
  * 					op = "GREATER_THAN"
  */
           __Pyx_INCREF(__pyx_n_u_LESS_THAN_OR_EQUAL);
           __Pyx_DECREF_SET(__pyx_v_op, __pyx_n_u_LESS_THAN_OR_EQUAL);
 
-          /* "viur/datastore/transport.pyx":941
+          /* "viur/datastore/transport.pyx":946
  * 				elif op == "<":
  * 					op = "LESS_THAN"
  * 				elif op == "<=":             # <<<<<<<<<<<<<<
  * 					op = "LESS_THAN_OR_EQUAL"
  * 				elif op == ">":
  */
           goto __pyx_L10;
         }
 
-        /* "viur/datastore/transport.pyx":943
+        /* "viur/datastore/transport.pyx":948
  * 				elif op == "<=":
  * 					op = "LESS_THAN_OR_EQUAL"
  * 				elif op == ">":             # <<<<<<<<<<<<<<
  * 					op = "GREATER_THAN"
  * 				elif op == ">=":
  */
-        __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_op, __pyx_kp_u__9, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 943, __pyx_L1_error)
+        __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_op, __pyx_kp_u__9, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 948, __pyx_L1_error)
         if (__pyx_t_5) {
 
-          /* "viur/datastore/transport.pyx":944
+          /* "viur/datastore/transport.pyx":949
  * 					op = "LESS_THAN_OR_EQUAL"
  * 				elif op == ">":
  * 					op = "GREATER_THAN"             # <<<<<<<<<<<<<<
  * 				elif op == ">=":
  * 					op = "GREATER_THAN_OR_EQUAL"
  */
           __Pyx_INCREF(__pyx_n_u_GREATER_THAN);
           __Pyx_DECREF_SET(__pyx_v_op, __pyx_n_u_GREATER_THAN);
 
-          /* "viur/datastore/transport.pyx":943
+          /* "viur/datastore/transport.pyx":948
  * 				elif op == "<=":
  * 					op = "LESS_THAN_OR_EQUAL"
  * 				elif op == ">":             # <<<<<<<<<<<<<<
  * 					op = "GREATER_THAN"
  * 				elif op == ">=":
  */
           goto __pyx_L10;
         }
 
-        /* "viur/datastore/transport.pyx":945
+        /* "viur/datastore/transport.pyx":950
  * 				elif op == ">":
  * 					op = "GREATER_THAN"
  * 				elif op == ">=":             # <<<<<<<<<<<<<<
  * 					op = "GREATER_THAN_OR_EQUAL"
  * 				else:
  */
-        __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_op, __pyx_kp_u__10, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 945, __pyx_L1_error)
+        __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_op, __pyx_kp_u__10, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 950, __pyx_L1_error)
         if (likely(__pyx_t_5)) {
 
-          /* "viur/datastore/transport.pyx":946
+          /* "viur/datastore/transport.pyx":951
  * 					op = "GREATER_THAN"
  * 				elif op == ">=":
  * 					op = "GREATER_THAN_OR_EQUAL"             # <<<<<<<<<<<<<<
  * 				else:
  * 					raise ValueError("Invalid op %s" % op)
  */
           __Pyx_INCREF(__pyx_n_u_GREATER_THAN_OR_EQUAL);
           __Pyx_DECREF_SET(__pyx_v_op, __pyx_n_u_GREATER_THAN_OR_EQUAL);
 
-          /* "viur/datastore/transport.pyx":945
+          /* "viur/datastore/transport.pyx":950
  * 				elif op == ">":
  * 					op = "GREATER_THAN"
  * 				elif op == ">=":             # <<<<<<<<<<<<<<
  * 					op = "GREATER_THAN_OR_EQUAL"
  * 				else:
  */
           goto __pyx_L10;
         }
 
-        /* "viur/datastore/transport.pyx":948
+        /* "viur/datastore/transport.pyx":953
  * 					op = "GREATER_THAN_OR_EQUAL"
  * 				else:
  * 					raise ValueError("Invalid op %s" % op)             # <<<<<<<<<<<<<<
  * 				if not isinstance(v, list):
  * 					# An entity can have a list of values for a single property, so it's possible to enforce
  */
         /*else*/ {
-          __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Invalid_op_s, __pyx_v_op); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 948, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Invalid_op_s, __pyx_v_op); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 953, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 948, __pyx_L1_error)
+          __pyx_t_7 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 953, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_Raise(__pyx_t_7, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-          __PYX_ERR(0, 948, __pyx_L1_error)
+          __PYX_ERR(0, 953, __pyx_L1_error)
         }
         __pyx_L10:;
 
-        /* "viur/datastore/transport.pyx":949
+        /* "viur/datastore/transport.pyx":954
  * 				else:
  * 					raise ValueError("Invalid op %s" % op)
  * 				if not isinstance(v, list):             # <<<<<<<<<<<<<<
  * 					# An entity can have a list of values for a single property, so it's possible to enforce
  * 					# more an one constraint for a a single property (e.g. x==5 and x==7 can be true), so
  */
         __pyx_t_5 = PyList_Check(__pyx_v_v); 
         __pyx_t_4 = ((!(__pyx_t_5 != 0)) != 0);
         if (__pyx_t_4) {
 
-          /* "viur/datastore/transport.pyx":953
+          /* "viur/datastore/transport.pyx":958
  * 					# more an one constraint for a a single property (e.g. x==5 and x==7 can be true), so
  * 					# enforce we always have a list here
  * 					v = [v]             # <<<<<<<<<<<<<<
  * 				for singleValue in v:
  * 					filterList.append({
  */
-          __pyx_t_7 = PyList_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 953, __pyx_L1_error)
+          __pyx_t_7 = PyList_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 958, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           __Pyx_INCREF(__pyx_v_v);
           __Pyx_GIVEREF(__pyx_v_v);
           PyList_SET_ITEM(__pyx_t_7, 0, __pyx_v_v);
           __Pyx_DECREF_SET(__pyx_v_v, __pyx_t_7);
           __pyx_t_7 = 0;
 
-          /* "viur/datastore/transport.pyx":949
+          /* "viur/datastore/transport.pyx":954
  * 				else:
  * 					raise ValueError("Invalid op %s" % op)
  * 				if not isinstance(v, list):             # <<<<<<<<<<<<<<
  * 					# An entity can have a list of values for a single property, so it's possible to enforce
  * 					# more an one constraint for a a single property (e.g. x==5 and x==7 can be true), so
  */
         }
 
-        /* "viur/datastore/transport.pyx":954
+        /* "viur/datastore/transport.pyx":959
  * 					# enforce we always have a list here
  * 					v = [v]
  * 				for singleValue in v:             # <<<<<<<<<<<<<<
  * 					filterList.append({
  * 						"propertyFilter": {
  */
         if (likely(PyList_CheckExact(__pyx_v_v)) || PyTuple_CheckExact(__pyx_v_v)) {
           __pyx_t_7 = __pyx_v_v; __Pyx_INCREF(__pyx_t_7); __pyx_t_13 = 0;
           __pyx_t_14 = NULL;
         } else {
-          __pyx_t_13 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_v_v); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 954, __pyx_L1_error)
+          __pyx_t_13 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_v_v); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 959, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
-          __pyx_t_14 = Py_TYPE(__pyx_t_7)->tp_iternext; if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 954, __pyx_L1_error)
+          __pyx_t_14 = Py_TYPE(__pyx_t_7)->tp_iternext; if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 959, __pyx_L1_error)
         }
         for (;;) {
           if (likely(!__pyx_t_14)) {
             if (likely(PyList_CheckExact(__pyx_t_7))) {
               if (__pyx_t_13 >= PyList_GET_SIZE(__pyx_t_7)) break;
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_3 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_13); __Pyx_INCREF(__pyx_t_3); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 954, __pyx_L1_error)
+              __pyx_t_3 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_13); __Pyx_INCREF(__pyx_t_3); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 959, __pyx_L1_error)
               #else
-              __pyx_t_3 = PySequence_ITEM(__pyx_t_7, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 954, __pyx_L1_error)
+              __pyx_t_3 = PySequence_ITEM(__pyx_t_7, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 959, __pyx_L1_error)
               __Pyx_GOTREF(__pyx_t_3);
               #endif
             } else {
               if (__pyx_t_13 >= PyTuple_GET_SIZE(__pyx_t_7)) break;
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-              __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_13); __Pyx_INCREF(__pyx_t_3); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 954, __pyx_L1_error)
+              __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_13); __Pyx_INCREF(__pyx_t_3); __pyx_t_13++; if (unlikely(0 < 0)) __PYX_ERR(0, 959, __pyx_L1_error)
               #else
-              __pyx_t_3 = PySequence_ITEM(__pyx_t_7, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 954, __pyx_L1_error)
+              __pyx_t_3 = PySequence_ITEM(__pyx_t_7, __pyx_t_13); __pyx_t_13++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 959, __pyx_L1_error)
               __Pyx_GOTREF(__pyx_t_3);
               #endif
             }
           } else {
             __pyx_t_3 = __pyx_t_14(__pyx_t_7);
             if (unlikely(!__pyx_t_3)) {
               PyObject* exc_type = PyErr_Occurred();
               if (exc_type) {
                 if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                else __PYX_ERR(0, 954, __pyx_L1_error)
+                else __PYX_ERR(0, 959, __pyx_L1_error)
               }
               break;
             }
             __Pyx_GOTREF(__pyx_t_3);
           }
           __Pyx_XDECREF_SET(__pyx_v_singleValue, __pyx_t_3);
           __pyx_t_3 = 0;
 
-          /* "viur/datastore/transport.pyx":956
+          /* "viur/datastore/transport.pyx":961
  * 				for singleValue in v:
  * 					filterList.append({
  * 						"propertyFilter": {             # <<<<<<<<<<<<<<
  * 							"property": {
  * 								"name": key,
  */
-          __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 956, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 961, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
 
-          /* "viur/datastore/transport.pyx":957
+          /* "viur/datastore/transport.pyx":962
  * 					filterList.append({
  * 						"propertyFilter": {
  * 							"property": {             # <<<<<<<<<<<<<<
  * 								"name": key,
  * 							},
  */
-          __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 957, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 962, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
 
-          /* "viur/datastore/transport.pyx":958
+          /* "viur/datastore/transport.pyx":963
  * 						"propertyFilter": {
  * 							"property": {
  * 								"name": key,             # <<<<<<<<<<<<<<
  * 							},
  * 							"op": op,
  */
-          __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 958, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 963, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_name, __pyx_v_key) < 0) __PYX_ERR(0, 958, __pyx_L1_error)
-          if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_property, __pyx_t_6) < 0) __PYX_ERR(0, 957, __pyx_L1_error)
+          if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_name, __pyx_v_key) < 0) __PYX_ERR(0, 963, __pyx_L1_error)
+          if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_property, __pyx_t_6) < 0) __PYX_ERR(0, 962, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-          /* "viur/datastore/transport.pyx":960
+          /* "viur/datastore/transport.pyx":965
  * 								"name": key,
  * 							},
  * 							"op": op,             # <<<<<<<<<<<<<<
  * 							"value": pythonPropToJson(singleValue)
  * 						}
  */
-          if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_op, __pyx_v_op) < 0) __PYX_ERR(0, 957, __pyx_L1_error)
+          if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_op, __pyx_v_op) < 0) __PYX_ERR(0, 962, __pyx_L1_error)
 
-          /* "viur/datastore/transport.pyx":961
+          /* "viur/datastore/transport.pyx":966
  * 							},
  * 							"op": op,
  * 							"value": pythonPropToJson(singleValue)             # <<<<<<<<<<<<<<
  * 						}
  * 					})
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_pythonPropToJson); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 961, __pyx_L1_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_pythonPropToJson); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 966, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_15);
           __pyx_t_16 = NULL;
           if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
             __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_15);
             if (likely(__pyx_t_16)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
               __Pyx_INCREF(__pyx_t_16);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_15, function);
             }
           }
           __pyx_t_6 = (__pyx_t_16) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_16, __pyx_v_singleValue) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_v_singleValue);
           __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
-          if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 961, __pyx_L1_error)
+          if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 966, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-          if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_value, __pyx_t_6) < 0) __PYX_ERR(0, 957, __pyx_L1_error)
+          if (PyDict_SetItem(__pyx_t_2, __pyx_n_u_value, __pyx_t_6) < 0) __PYX_ERR(0, 962, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-          if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_propertyFilter, __pyx_t_2) < 0) __PYX_ERR(0, 956, __pyx_L1_error)
+          if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_propertyFilter, __pyx_t_2) < 0) __PYX_ERR(0, 961, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-          /* "viur/datastore/transport.pyx":955
+          /* "viur/datastore/transport.pyx":960
  * 					v = [v]
  * 				for singleValue in v:
  * 					filterList.append({             # <<<<<<<<<<<<<<
  * 						"propertyFilter": {
  * 							"property": {
  */
-          __pyx_t_17 = __Pyx_PyList_Append(__pyx_v_filterList, __pyx_t_3); if (unlikely(__pyx_t_17 == ((int)-1))) __PYX_ERR(0, 955, __pyx_L1_error)
+          __pyx_t_17 = __Pyx_PyList_Append(__pyx_v_filterList, __pyx_t_3); if (unlikely(__pyx_t_17 == ((int)-1))) __PYX_ERR(0, 960, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-          /* "viur/datastore/transport.pyx":954
+          /* "viur/datastore/transport.pyx":959
  * 					# enforce we always have a list here
  * 					v = [v]
  * 				for singleValue in v:             # <<<<<<<<<<<<<<
  * 					filterList.append({
  * 						"propertyFilter": {
  */
         }
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "viur/datastore/transport.pyx":964
+      /* "viur/datastore/transport.pyx":969
  * 						}
  * 					})
  * 			if len(filterList) == 1:  # Special, single filter             # <<<<<<<<<<<<<<
  * 				post_data["aggregation_query"]["nested_query"]["filter"] = filterList[0]
  * 			else:
  */
-      __pyx_t_9 = PyList_GET_SIZE(__pyx_v_filterList); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 964, __pyx_L1_error)
+      __pyx_t_9 = PyList_GET_SIZE(__pyx_v_filterList); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 969, __pyx_L1_error)
       __pyx_t_4 = ((__pyx_t_9 == 1) != 0);
       if (__pyx_t_4) {
 
-        /* "viur/datastore/transport.pyx":965
+        /* "viur/datastore/transport.pyx":970
  * 					})
  * 			if len(filterList) == 1:  # Special, single filter
  * 				post_data["aggregation_query"]["nested_query"]["filter"] = filterList[0]             # <<<<<<<<<<<<<<
  * 			else:
  * 				post_data["aggregation_query"]["nested_query"]["filter"] = {
  */
-        __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_filterList, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 965, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_filterList, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 970, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_post_data, __pyx_n_u_aggregation_query); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 965, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_v_post_data, __pyx_n_u_aggregation_query); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 970, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_nested_query); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 965, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_nested_query); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 970, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_n_u_filter, __pyx_t_1) < 0)) __PYX_ERR(0, 965, __pyx_L1_error)
+        if (unlikely(PyObject_SetItem(__pyx_t_3, __pyx_n_u_filter, __pyx_t_1) < 0)) __PYX_ERR(0, 970, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "viur/datastore/transport.pyx":964
+        /* "viur/datastore/transport.pyx":969
  * 						}
  * 					})
  * 			if len(filterList) == 1:  # Special, single filter             # <<<<<<<<<<<<<<
  * 				post_data["aggregation_query"]["nested_query"]["filter"] = filterList[0]
  * 			else:
  */
         goto __pyx_L14;
       }
 
-      /* "viur/datastore/transport.pyx":968
+      /* "viur/datastore/transport.pyx":973
  * 			else:
  * 				post_data["aggregation_query"]["nested_query"]["filter"] = {
  * 					"compositeFilter": {             # <<<<<<<<<<<<<<
  * 						"op": "AND",
  * 						"filters": filterList
  */
       /*else*/ {
-        __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 968, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 973, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
 
-        /* "viur/datastore/transport.pyx":969
+        /* "viur/datastore/transport.pyx":974
  * 				post_data["aggregation_query"]["nested_query"]["filter"] = {
  * 					"compositeFilter": {
  * 						"op": "AND",             # <<<<<<<<<<<<<<
  * 						"filters": filterList
  * 					}
  */
-        __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 969, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 974, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_op, __pyx_n_u_AND) < 0) __PYX_ERR(0, 969, __pyx_L1_error)
+        if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_op, __pyx_n_u_AND) < 0) __PYX_ERR(0, 974, __pyx_L1_error)
 
-        /* "viur/datastore/transport.pyx":970
+        /* "viur/datastore/transport.pyx":975
  * 					"compositeFilter": {
  * 						"op": "AND",
  * 						"filters": filterList             # <<<<<<<<<<<<<<
  * 					}
  * 				}
  */
-        if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_filters, __pyx_v_filterList) < 0) __PYX_ERR(0, 969, __pyx_L1_error)
-        if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_compositeFilter, __pyx_t_3) < 0) __PYX_ERR(0, 968, __pyx_L1_error)
+        if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_filters, __pyx_v_filterList) < 0) __PYX_ERR(0, 974, __pyx_L1_error)
+        if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_compositeFilter, __pyx_t_3) < 0) __PYX_ERR(0, 973, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "viur/datastore/transport.pyx":967
+        /* "viur/datastore/transport.pyx":972
  * 				post_data["aggregation_query"]["nested_query"]["filter"] = filterList[0]
  * 			else:
  * 				post_data["aggregation_query"]["nested_query"]["filter"] = {             # <<<<<<<<<<<<<<
  * 					"compositeFilter": {
  * 						"op": "AND",
  */
-        __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_post_data, __pyx_n_u_aggregation_query); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 967, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_post_data, __pyx_n_u_aggregation_query); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 972, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_nested_query); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 967, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_nested_query); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 972, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(PyObject_SetItem(__pyx_t_7, __pyx_n_u_filter, __pyx_t_1) < 0)) __PYX_ERR(0, 967, __pyx_L1_error)
+        if (unlikely(PyObject_SetItem(__pyx_t_7, __pyx_n_u_filter, __pyx_t_1) < 0)) __PYX_ERR(0, 972, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
       __pyx_L14:;
 
-      /* "viur/datastore/transport.pyx":933
+      /* "viur/datastore/transport.pyx":938
  * 	}
  * 	if queryDefinition:
  * 		if queryDefinition.filters:             # <<<<<<<<<<<<<<
  * 			filterList = []
  * 			for k, v in queryDefinition.filters.items():
  */
     }
 
-    /* "viur/datastore/transport.pyx":932
+    /* "viur/datastore/transport.pyx":937
  * 
  * 	}
  * 	if queryDefinition:             # <<<<<<<<<<<<<<
  * 		if queryDefinition.filters:
  * 			filterList = []
  */
   }
 
-  /* "viur/datastore/transport.pyx":973
+  /* "viur/datastore/transport.pyx":978
  * 					}
  * 				}
  * 	req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 		url="https://datastore.googleapis.com/v1/projects/%s:runAggregationQuery" % projectID,
  * 		data=json.dumps(post_data).encode("UTF-8"),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 973, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_authenticatedRequest); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 978, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "viur/datastore/transport.pyx":974
+  /* "viur/datastore/transport.pyx":979
  * 				}
  * 	req = authenticatedRequest(
  * 		url="https://datastore.googleapis.com/v1/projects/%s:runAggregationQuery" % projectID,             # <<<<<<<<<<<<<<
  * 		data=json.dumps(post_data).encode("UTF-8"),
  * 	)
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 974, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 979, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_projectID); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 974, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_projectID); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 979, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_7, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 974, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_https_datastore_googleapis_com_v_7, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 979, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_url, __pyx_t_2) < 0) __PYX_ERR(0, 974, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_url, __pyx_t_2) < 0) __PYX_ERR(0, 979, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "viur/datastore/transport.pyx":975
+  /* "viur/datastore/transport.pyx":980
  * 	req = authenticatedRequest(
  * 		url="https://datastore.googleapis.com/v1/projects/%s:runAggregationQuery" % projectID,
  * 		data=json.dumps(post_data).encode("UTF-8"),             # <<<<<<<<<<<<<<
  * 	)
  * 	assert req.status_code == 200
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_json); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 975, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_json); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 980, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_dumps); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 975, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_dumps); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 980, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
   __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_6, __pyx_v_post_data) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_v_post_data);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 975, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 980, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_encode); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 975, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_encode); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 980, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
   __pyx_t_2 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_3, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_kp_u_UTF_8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 975, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 980, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_data, __pyx_t_2) < 0) __PYX_ERR(0, 974, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_data, __pyx_t_2) < 0) __PYX_ERR(0, 979, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "viur/datastore/transport.pyx":973
+  /* "viur/datastore/transport.pyx":978
  * 					}
  * 				}
  * 	req = authenticatedRequest(             # <<<<<<<<<<<<<<
  * 		url="https://datastore.googleapis.com/v1/projects/%s:runAggregationQuery" % projectID,
  * 		data=json.dumps(post_data).encode("UTF-8"),
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 973, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 978, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_v_req = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "viur/datastore/transport.pyx":977
+  /* "viur/datastore/transport.pyx":982
  * 		data=json.dumps(post_data).encode("UTF-8"),
  * 	)
  * 	assert req.status_code == 200             # <<<<<<<<<<<<<<
  * 	assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 	element = parser.parse(data_ptr, pysize, 1)
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 977, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_status_code); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 982, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = __Pyx_PyInt_EqObjC(__pyx_t_2, __pyx_int_200, 0xC8, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 977, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_EqObjC(__pyx_t_2, __pyx_int_200, 0xC8, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 982, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 977, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 982, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (unlikely(!__pyx_t_4)) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 977, __pyx_L1_error)
+      __PYX_ERR(0, 982, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "viur/datastore/transport.pyx":978
+  /* "viur/datastore/transport.pyx":983
  * 	)
  * 	assert req.status_code == 200
  * 	assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1             # <<<<<<<<<<<<<<
  * 	element = parser.parse(data_ptr, pysize, 1)
  * 	if element.at_pointer("/batch").error() != SUCCESS:
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 978, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 983, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_10 = PyBytes_AsStringAndSize(__pyx_t_7, (&__pyx_v_data_ptr), (&__pyx_v_pysize)); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 978, __pyx_L1_error)
+    __pyx_t_10 = PyBytes_AsStringAndSize(__pyx_t_7, (&__pyx_v_data_ptr), (&__pyx_v_pysize)); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 983, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (unlikely(!((__pyx_t_10 != -1L) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 978, __pyx_L1_error)
+      __PYX_ERR(0, 983, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "viur/datastore/transport.pyx":979
+  /* "viur/datastore/transport.pyx":984
  * 	assert req.status_code == 200
  * 	assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 	element = parser.parse(data_ptr, pysize, 1)             # <<<<<<<<<<<<<<
  * 	if element.at_pointer("/batch").error() != SUCCESS:
  * 		print("INVALID RESPONSE RECEIVED")
  */
   try {
     __pyx_t_18 = __pyx_v_parser.parse(__pyx_v_data_ptr, __pyx_v_pysize, 1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 979, __pyx_L1_error)
+    __PYX_ERR(0, 984, __pyx_L1_error)
   }
   __pyx_v_element = __pyx_t_18;
 
-  /* "viur/datastore/transport.pyx":980
+  /* "viur/datastore/transport.pyx":985
  * 	assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 	element = parser.parse(data_ptr, pysize, 1)
  * 	if element.at_pointer("/batch").error() != SUCCESS:             # <<<<<<<<<<<<<<
  * 		print("INVALID RESPONSE RECEIVED")
  * 		pprint.pprint(json.loads(req.content))
  */
   __pyx_t_4 = ((__pyx_v_element.at_pointer(((char const *)"/batch")).error() != simdjson::error_code::SUCCESS) != 0);
   if (__pyx_t_4) {
 
-    /* "viur/datastore/transport.pyx":981
+    /* "viur/datastore/transport.pyx":986
  * 	element = parser.parse(data_ptr, pysize, 1)
  * 	if element.at_pointer("/batch").error() != SUCCESS:
  * 		print("INVALID RESPONSE RECEIVED")             # <<<<<<<<<<<<<<
  * 		pprint.pprint(json.loads(req.content))
  * 	element = element.at_key("batch")
  */
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 981, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_print, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 986, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "viur/datastore/transport.pyx":982
+    /* "viur/datastore/transport.pyx":987
  * 	if element.at_pointer("/batch").error() != SUCCESS:
  * 		print("INVALID RESPONSE RECEIVED")
  * 		pprint.pprint(json.loads(req.content))             # <<<<<<<<<<<<<<
  * 	element = element.at_key("batch")
  * 	# TODO  maybe this can be solved more elegant
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pprint); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 982, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pprint); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 987, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_pprint); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 982, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_pprint); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 987, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_json); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 982, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_json); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 987, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_loads); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 982, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_loads); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 987, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-    __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 982, __pyx_L1_error)
+    __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v_req, __pyx_n_s_content); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 987, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_t_15) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_15);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 982, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 987, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
@@ -15094,74 +15264,74 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_7 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 982, __pyx_L1_error)
+    if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 987, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "viur/datastore/transport.pyx":980
+    /* "viur/datastore/transport.pyx":985
  * 	assert PyBytes_AsStringAndSize(req.content, &data_ptr, &pysize) != -1
  * 	element = parser.parse(data_ptr, pysize, 1)
  * 	if element.at_pointer("/batch").error() != SUCCESS:             # <<<<<<<<<<<<<<
  * 		print("INVALID RESPONSE RECEIVED")
  * 		pprint.pprint(json.loads(req.content))
  */
   }
 
-  /* "viur/datastore/transport.pyx":983
+  /* "viur/datastore/transport.pyx":988
  * 		print("INVALID RESPONSE RECEIVED")
  * 		pprint.pprint(json.loads(req.content))
  * 	element = element.at_key("batch")             # <<<<<<<<<<<<<<
  * 	# TODO  maybe this can be solved more elegant
  * 	return int(toPythonStructure(element)["aggregationResults"][0]["aggregateProperties"]["property_1"]["integerValue"])
  */
   try {
     __pyx_t_18 = __pyx_v_element.at_key(((char const *)"batch"));
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 983, __pyx_L1_error)
+    __PYX_ERR(0, 988, __pyx_L1_error)
   }
   __pyx_v_element = __pyx_t_18;
 
-  /* "viur/datastore/transport.pyx":985
+  /* "viur/datastore/transport.pyx":990
  * 	element = element.at_key("batch")
  * 	# TODO  maybe this can be solved more elegant
  * 	return int(toPythonStructure(element)["aggregationResults"][0]["aggregateProperties"]["property_1"]["integerValue"])             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_7 = __pyx_f_4viur_9datastore_9transport_toPythonStructure(__pyx_v_element); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 985, __pyx_L1_error)
+  __pyx_t_7 = __pyx_f_4viur_9datastore_9transport_toPythonStructure(__pyx_v_element); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_aggregationResults); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 985, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_aggregationResults); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 985, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_aggregateProperties); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 985, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_aggregateProperties); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_property_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 985, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Dict_GetItem(__pyx_t_1, __pyx_n_u_property_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_integerValue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 985, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_7, __pyx_n_u_integerValue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 985, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "viur/datastore/transport.pyx":900
+  /* "viur/datastore/transport.pyx":905
  * 		raise ValueError("Invalid data received from Datastore API")
  * 
  * def Count(kind: str = None, up_to= 2 ** 63 - 1, queryDefinition: QueryDefinition = None) -> Union[Key, List[Key]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Count all entries in a kind if there is only a kind is provided
  */
 
@@ -15413,17 +15583,19 @@
   {&__pyx_n_u_NON_TRANSACTIONAL, __pyx_k_NON_TRANSACTIONAL, sizeof(__pyx_k_NON_TRANSACTIONAL), 0, 1, 0, 1},
   {&__pyx_n_u_NOT_FINISHED, __pyx_k_NOT_FINISHED, sizeof(__pyx_k_NOT_FINISHED), 0, 1, 0, 1},
   {&__pyx_n_u_NO_MORE_RESULTS, __pyx_k_NO_MORE_RESULTS, sizeof(__pyx_k_NO_MORE_RESULTS), 0, 1, 0, 1},
   {&__pyx_n_s_NoMutationResultsError, __pyx_k_NoMutationResultsError, sizeof(__pyx_k_NoMutationResultsError), 0, 0, 1, 1},
   {&__pyx_kp_u_No_mutation_results_received, __pyx_k_No_mutation_results_received, sizeof(__pyx_k_No_mutation_results_received), 0, 1, 0, 0},
   {&__pyx_kp_u_No_mutation_results_received_2, __pyx_k_No_mutation_results_received_2, sizeof(__pyx_k_No_mutation_results_received_2), 0, 1, 0, 0},
   {&__pyx_kp_u_None, __pyx_k_None, sizeof(__pyx_k_None), 0, 1, 0, 0},
+  {&__pyx_kp_u_Please_create_a_matching_index, __pyx_k_Please_create_a_matching_index, sizeof(__pyx_k_Please_create_a_matching_index), 0, 1, 0, 0},
   {&__pyx_n_s_Put, __pyx_k_Put, sizeof(__pyx_k_Put), 0, 0, 1, 1},
   {&__pyx_kp_u_Queried, __pyx_k_Queried, sizeof(__pyx_k_Queried), 0, 1, 0, 0},
   {&__pyx_n_s_QueryDefinition, __pyx_k_QueryDefinition, sizeof(__pyx_k_QueryDefinition), 0, 0, 1, 1},
+  {&__pyx_kp_u_Query_not_finished_Maybe_some_en, __pyx_k_Query_not_finished_Maybe_some_en, sizeof(__pyx_k_Query_not_finished_Maybe_some_en), 0, 1, 0, 0},
   {&__pyx_kp_u_Received_an_unexpected_key_updat, __pyx_k_Received_an_unexpected_key_updat, sizeof(__pyx_k_Received_an_unexpected_key_updat), 0, 1, 0, 0},
   {&__pyx_n_s_RecursionError, __pyx_k_RecursionError, sizeof(__pyx_k_RecursionError), 0, 0, 1, 1},
   {&__pyx_n_s_RequestsConnectionError, __pyx_k_RequestsConnectionError, sizeof(__pyx_k_RequestsConnectionError), 0, 0, 1, 1},
   {&__pyx_kp_u_Retrying_http_post_request_to_da, __pyx_k_Retrying_http_post_request_to_da, sizeof(__pyx_k_Retrying_http_post_request_to_da), 0, 1, 0, 0},
   {&__pyx_kp_u_Returned, __pyx_k_Returned, sizeof(__pyx_k_Returned), 0, 1, 0, 0},
   {&__pyx_n_s_RunInTransaction, __pyx_k_RunInTransaction, sizeof(__pyx_k_RunInTransaction), 0, 0, 1, 1},
   {&__pyx_n_u_STRONG, __pyx_k_STRONG, sizeof(__pyx_k_STRONG), 0, 1, 0, 1},
@@ -15698,99 +15870,99 @@
  * 			pprint.pprint(json.loads(req.content))
  * 		#	res.update(toEntityStructure(element.at_key("batch"), isInitial=True))
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_INVALID_RESPONSE_RECEIVED); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 542, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "viur/datastore/transport.pyx":564
+  /* "viur/datastore/transport.pyx":569
  * 				queryDefinition.kind, filters, orders, distinctOn, len(res)))
  * 	if flipResults:
  * 		return res[::-1]             # <<<<<<<<<<<<<<
  * 	return res
  * 
  */
-  __pyx_slice__13 = PySlice_New(Py_None, Py_None, __pyx_int_neg_1); if (unlikely(!__pyx_slice__13)) __PYX_ERR(0, 564, __pyx_L1_error)
+  __pyx_slice__13 = PySlice_New(Py_None, Py_None, __pyx_int_neg_1); if (unlikely(!__pyx_slice__13)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__13);
   __Pyx_GIVEREF(__pyx_slice__13);
 
-  /* "viur/datastore/transport.pyx":600
+  /* "viur/datastore/transport.pyx":605
  * 	res = {}
  * 	while keyList:
  * 		requestedKeys = keyList[:300]             # <<<<<<<<<<<<<<
  * 		postData = {
  * 			"readOptions": readOptions,
  */
-  __pyx_slice__14 = PySlice_New(Py_None, __pyx_int_300, Py_None); if (unlikely(!__pyx_slice__14)) __PYX_ERR(0, 600, __pyx_L1_error)
+  __pyx_slice__14 = PySlice_New(Py_None, __pyx_int_300, Py_None); if (unlikely(!__pyx_slice__14)) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__14);
   __Pyx_GIVEREF(__pyx_slice__14);
 
-  /* "viur/datastore/transport.pyx":615
+  /* "viur/datastore/transport.pyx":620
  * 			res.update(toEntityStructure(element.at_key("found"), isInitial=True))
  * 		if (element.at_pointer("/deferred").error() == SUCCESS):
  * 			keyList = toPythonStructure(element.at_key("deferred")) + keyList[300:]             # <<<<<<<<<<<<<<
  * 		else:
  * 			keyList = keyList[300:]
  */
-  __pyx_slice__15 = PySlice_New(__pyx_int_300, Py_None, Py_None); if (unlikely(!__pyx_slice__15)) __PYX_ERR(0, 615, __pyx_L1_error)
+  __pyx_slice__15 = PySlice_New(__pyx_int_300, Py_None, Py_None); if (unlikely(!__pyx_slice__15)) __PYX_ERR(0, 620, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__15);
   __Pyx_GIVEREF(__pyx_slice__15);
 
-  /* "viur/datastore/transport.pyx":674
+  /* "viur/datastore/transport.pyx":679
  * 		if arrayElem.size() != abs(len(keys)):
  * 			print(req.content)
  * 			raise ValueError("Invalid number of mutation-results received")             # <<<<<<<<<<<<<<
  * 
  * def Put(entities: Union[Entity, List[Entity]]) -> Union[Entity, List[Entity]]:
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_Invalid_number_of_mutation_resul); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 674, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_Invalid_number_of_mutation_resul); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "viur/datastore/transport.pyx":720
+  /* "viur/datastore/transport.pyx":725
  * 		if (element.at_pointer("/mutationResults").error() != SUCCESS):
  * 			print(req.content)
  * 			raise ValueError("No mutation-results received")             # <<<<<<<<<<<<<<
  * 		arrayElem = element.at_key("mutationResults").get_array()
  * 		if arrayElem.size() != abs(len(entities)):
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_No_mutation_results_received_2); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 720, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_No_mutation_results_received_2); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 725, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "viur/datastore/transport.pyx":758
+  /* "viur/datastore/transport.pyx":763
  * 			if oldTxn:
  * 				if not allowOverriding:
  * 					raise RecursionError("Cannot call runInTransaction while inside a transaction!")             # <<<<<<<<<<<<<<
  * 				txnOptions = {
  * 					"previousTransaction": oldTxn["key"]
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_u_Cannot_call_runInTransaction_whi); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 758, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_u_Cannot_call_runInTransaction_whi); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 763, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
 
-  /* "viur/datastore/transport.pyx":890
+  /* "viur/datastore/transport.pyx":895
  * 			preincrement(arrayIt)
  * 		if not res:
  * 			raise ValueError("Empty response received from Datastore API")             # <<<<<<<<<<<<<<
  * 		elif not isMulti:
  * 			return res[0]
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_u_Empty_response_received_from_Dat); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 890, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_u_Empty_response_received_from_Dat); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 895, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
 
-  /* "viur/datastore/transport.pyx":898
+  /* "viur/datastore/transport.pyx":903
  * 		logging.error("Invalid data received from Datastore API")
  * 		logging.error(req.content)
  * 		raise ValueError("Invalid data received from Datastore API")             # <<<<<<<<<<<<<<
  * 
  * def Count(kind: str = None, up_to= 2 ** 63 - 1, queryDefinition: QueryDefinition = None) -> Union[Key, List[Key]]:
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_u_Invalid_data_received_from_Datas); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 898, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_u_Invalid_data_received_from_Datas); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 903, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "viur/datastore/transport.pyx":107
  * )
  * 
  * def authenticatedRequest(url:str, data: bytes) -> requests.Response:             # <<<<<<<<<<<<<<
@@ -15834,97 +16006,97 @@
  * 		Runs a single Query as defined by queryDefinition. The limit of the queryDefinition is ignored and must
  */
   __pyx_tuple__28 = PyTuple_Pack(24, __pyx_n_s_queryDefinition, __pyx_n_s_limit, __pyx_n_s_parser, __pyx_n_s_pysize, __pyx_n_s_data_ptr, __pyx_n_s_element, __pyx_n_s_res, __pyx_n_s_internalStartCursor, __pyx_n_s_flipResults, __pyx_n_s_currentTxn, __pyx_n_s_readOptions, __pyx_n_s_postData, __pyx_n_s_filterList, __pyx_n_s_k, __pyx_n_s_v, __pyx_n_s_key, __pyx_n_s_op, __pyx_n_s_singleValue, __pyx_n_s_req, __pyx_n_s_orders, __pyx_n_s_filters, __pyx_n_s_distinctOn, __pyx_n_s_sortOrder, __pyx_n_s_distinctKey); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 439, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
   __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(2, 0, 24, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_runSingleFilter, 439, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 439, __pyx_L1_error)
 
-  /* "viur/datastore/transport.pyx":567
+  /* "viur/datastore/transport.pyx":572
  * 	return res
  * 
  * def Get(keys: Union[Key, List[Key]]) -> Union[None, Entity, List[Entity]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Fetches the entities determined by keys from the datastore. Returns or inserts None if a key is not found.
  */
-  __pyx_tuple__30 = PyTuple_Pack(16, __pyx_n_s_keys, __pyx_n_s_parser, __pyx_n_s_pysize, __pyx_n_s_data_ptr, __pyx_n_s_element, __pyx_n_s_isMulti, __pyx_n_s_accessLog, __pyx_n_s_keyList, __pyx_n_s_currentTxn, __pyx_n_s_readOptions, __pyx_n_s_res, __pyx_n_s_requestedKeys, __pyx_n_s_postData, __pyx_n_s_req, __pyx_n_s_x, __pyx_n_s_x); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 567, __pyx_L1_error)
+  __pyx_tuple__30 = PyTuple_Pack(16, __pyx_n_s_keys, __pyx_n_s_parser, __pyx_n_s_pysize, __pyx_n_s_data_ptr, __pyx_n_s_element, __pyx_n_s_isMulti, __pyx_n_s_accessLog, __pyx_n_s_keyList, __pyx_n_s_currentTxn, __pyx_n_s_readOptions, __pyx_n_s_res, __pyx_n_s_requestedKeys, __pyx_n_s_postData, __pyx_n_s_req, __pyx_n_s_x, __pyx_n_s_x); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 572, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__30);
   __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_Get, 567, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 567, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_Get, 572, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 572, __pyx_L1_error)
 
-  /* "viur/datastore/transport.pyx":623
+  /* "viur/datastore/transport.pyx":628
  * 		return [res.get(x) for x in keys]  # Sort by order of incoming keys
  * 
  * def Delete(keys: Union[Key, List[Key], Entity, List[Entity]]) -> None:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Deletes the entities stored under the given key(s).
  */
-  __pyx_tuple__32 = PyTuple_Pack(12, __pyx_n_s_keys, __pyx_n_s_parser, __pyx_n_s_pysize, __pyx_n_s_data_ptr, __pyx_n_s_element, __pyx_n_s_arrayElem, __pyx_n_s_accessLog, __pyx_n_s_postData, __pyx_n_s_currentTxn, __pyx_n_s_req, __pyx_n_s_x, __pyx_n_s_x); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 623, __pyx_L1_error)
+  __pyx_tuple__32 = PyTuple_Pack(12, __pyx_n_s_keys, __pyx_n_s_parser, __pyx_n_s_pysize, __pyx_n_s_data_ptr, __pyx_n_s_element, __pyx_n_s_arrayElem, __pyx_n_s_accessLog, __pyx_n_s_postData, __pyx_n_s_currentTxn, __pyx_n_s_req, __pyx_n_s_x, __pyx_n_s_x); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__32);
   __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(1, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_Delete, 623, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 623, __pyx_L1_error)
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(1, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_Delete, 628, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 628, __pyx_L1_error)
 
-  /* "viur/datastore/transport.pyx":676
+  /* "viur/datastore/transport.pyx":681
  * 			raise ValueError("Invalid number of mutation-results received")
  * 
  * def Put(entities: Union[Entity, List[Entity]]) -> Union[Entity, List[Entity]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Writes the given entities into the datastore. The entities can be from different kinds. If an entity has an
  */
-  __pyx_tuple__34 = PyTuple_Pack(15, __pyx_n_s_entities, __pyx_n_s_parser, __pyx_n_s_pysize, __pyx_n_s_data_ptr, __pyx_n_s_element, __pyx_n_s_innerArrayElem, __pyx_n_s_arrayElem, __pyx_n_s_arrayIt, __pyx_n_s_accessLog, __pyx_n_s_postData, __pyx_n_s_currentTxn, __pyx_n_s_req, __pyx_n_s_idx, __pyx_n_s_x, __pyx_n_s_x); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 676, __pyx_L1_error)
+  __pyx_tuple__34 = PyTuple_Pack(15, __pyx_n_s_entities, __pyx_n_s_parser, __pyx_n_s_pysize, __pyx_n_s_data_ptr, __pyx_n_s_element, __pyx_n_s_innerArrayElem, __pyx_n_s_arrayElem, __pyx_n_s_arrayIt, __pyx_n_s_accessLog, __pyx_n_s_postData, __pyx_n_s_currentTxn, __pyx_n_s_req, __pyx_n_s_idx, __pyx_n_s_x, __pyx_n_s_x); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(1, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_Put, 676, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 676, __pyx_L1_error)
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(1, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_Put, 681, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 681, __pyx_L1_error)
 
-  /* "viur/datastore/transport.pyx":737
+  /* "viur/datastore/transport.pyx":742
  * 
  * 
  * def RunInTransaction(callback: callable, *args, **kwargs) -> Any:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Runs the given function inside a AID transaction.
  */
-  __pyx_tuple__36 = PyTuple_Pack(21, __pyx_n_s_callback, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_parser, __pyx_n_s_pysize, __pyx_n_s_data_ptr, __pyx_n_s_element, __pyx_n_s_innerArrayElem, __pyx_n_s_arrayElem, __pyx_n_s_arrayIt, __pyx_n_s_exponential_backoff, __pyx_n_s_oldTxn, __pyx_n_s_allowOverriding_2, __pyx_n_s_txnOptions, __pyx_n_s_postData, __pyx_n_s_req, __pyx_n_s_txnKey, __pyx_n_s_currentTxn, __pyx_n_s_res, __pyx_n_s_idx, __pyx_n_s_affectedEntity); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 737, __pyx_L1_error)
+  __pyx_tuple__36 = PyTuple_Pack(21, __pyx_n_s_callback, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_parser, __pyx_n_s_pysize, __pyx_n_s_data_ptr, __pyx_n_s_element, __pyx_n_s_innerArrayElem, __pyx_n_s_arrayElem, __pyx_n_s_arrayIt, __pyx_n_s_exponential_backoff, __pyx_n_s_oldTxn, __pyx_n_s_allowOverriding_2, __pyx_n_s_txnOptions, __pyx_n_s_postData, __pyx_n_s_req, __pyx_n_s_txnKey, __pyx_n_s_currentTxn, __pyx_n_s_res, __pyx_n_s_idx, __pyx_n_s_affectedEntity); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__36);
   __Pyx_GIVEREF(__pyx_tuple__36);
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(1, 0, 21, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_RunInTransaction, 737, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 737, __pyx_L1_error)
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(1, 0, 21, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_RunInTransaction, 742, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 742, __pyx_L1_error)
 
-  /* "viur/datastore/transport.pyx":829
+  /* "viur/datastore/transport.pyx":834
  * 
  * 
  * def _rollbackTxn(txnKey: str):             # <<<<<<<<<<<<<<
  * 	"""
  * 		Internal helper that aborts the given transaction. It's important to abort pending transactions (instead
  */
-  __pyx_tuple__38 = PyTuple_Pack(3, __pyx_n_s_txnKey, __pyx_n_s_postData, __pyx_n_s_req); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 829, __pyx_L1_error)
+  __pyx_tuple__38 = PyTuple_Pack(3, __pyx_n_s_txnKey, __pyx_n_s_postData, __pyx_n_s_req); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 834, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__38);
   __Pyx_GIVEREF(__pyx_tuple__38);
-  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_rollbackTxn, 829, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 829, __pyx_L1_error)
+  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_rollbackTxn, 834, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 834, __pyx_L1_error)
 
-  /* "viur/datastore/transport.pyx":845
+  /* "viur/datastore/transport.pyx":850
  * 	)
  * 
  * def AllocateIDs(keys: Union[Key, List[Key]]) -> Union[Key, List[Key]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Allocates numeric IDs for the keys given.
  */
-  __pyx_tuple__40 = PyTuple_Pack(15, __pyx_n_s_keys, __pyx_n_s_parser, __pyx_n_s_pysize, __pyx_n_s_data_ptr, __pyx_n_s_element, __pyx_n_s_isMulti, __pyx_n_s_keyList, __pyx_n_s_requestedKeys, __pyx_n_s_postData, __pyx_n_s_req, __pyx_n_s_res, __pyx_n_s_arrayElem, __pyx_n_s_arrayIt, __pyx_n_s_innerArrayElem, __pyx_n_s_x); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 845, __pyx_L1_error)
+  __pyx_tuple__40 = PyTuple_Pack(15, __pyx_n_s_keys, __pyx_n_s_parser, __pyx_n_s_pysize, __pyx_n_s_data_ptr, __pyx_n_s_element, __pyx_n_s_isMulti, __pyx_n_s_keyList, __pyx_n_s_requestedKeys, __pyx_n_s_postData, __pyx_n_s_req, __pyx_n_s_res, __pyx_n_s_arrayElem, __pyx_n_s_arrayIt, __pyx_n_s_innerArrayElem, __pyx_n_s_x); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 850, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__40);
   __Pyx_GIVEREF(__pyx_tuple__40);
-  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(1, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_AllocateIDs, 845, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 845, __pyx_L1_error)
+  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(1, 0, 15, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_AllocateIDs, 850, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 850, __pyx_L1_error)
 
-  /* "viur/datastore/transport.pyx":900
+  /* "viur/datastore/transport.pyx":905
  * 		raise ValueError("Invalid data received from Datastore API")
  * 
  * def Count(kind: str = None, up_to= 2 ** 63 - 1, queryDefinition: QueryDefinition = None) -> Union[Key, List[Key]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Count all entries in a kind if there is only a kind is provided
  */
-  __pyx_tuple__42 = PyTuple_Pack(18, __pyx_n_s_kind, __pyx_n_s_up_to, __pyx_n_s_queryDefinition, __pyx_n_s_parser, __pyx_n_s_pysize, __pyx_n_s_data_ptr, __pyx_n_s_element, __pyx_n_s_element_inner, __pyx_n_s_array_element, __pyx_n_s_array_element_inner, __pyx_n_s_post_data, __pyx_n_s_filterList, __pyx_n_s_k, __pyx_n_s_v, __pyx_n_s_key, __pyx_n_s_op, __pyx_n_s_singleValue, __pyx_n_s_req); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(0, 900, __pyx_L1_error)
+  __pyx_tuple__42 = PyTuple_Pack(18, __pyx_n_s_kind, __pyx_n_s_up_to, __pyx_n_s_queryDefinition, __pyx_n_s_parser, __pyx_n_s_pysize, __pyx_n_s_data_ptr, __pyx_n_s_element, __pyx_n_s_element_inner, __pyx_n_s_array_element, __pyx_n_s_array_element_inner, __pyx_n_s_post_data, __pyx_n_s_filterList, __pyx_n_s_k, __pyx_n_s_v, __pyx_n_s_key, __pyx_n_s_op, __pyx_n_s_singleValue, __pyx_n_s_req); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(0, 905, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__42);
   __Pyx_GIVEREF(__pyx_tuple__42);
-  __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(3, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_Count, 900, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(0, 900, __pyx_L1_error)
+  __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(3, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_viur_datastore_transport_pyx, __pyx_n_s_Count, 905, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(0, 905, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -16712,96 +16884,96 @@
  * 		Runs a single Query as defined by queryDefinition. The limit of the queryDefinition is ignored and must
  */
   __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_7runSingleFilter, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 439, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_runSingleFilter, __pyx_t_4) < 0) __PYX_ERR(0, 439, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":567
+  /* "viur/datastore/transport.pyx":572
  * 	return res
  * 
  * def Get(keys: Union[Key, List[Key]]) -> Union[None, Entity, List[Entity]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Fetches the entities determined by keys from the datastore. Returns or inserts None if a key is not found.
  */
-  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_9Get, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 567, __pyx_L1_error)
+  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_9Get, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 572, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Get, __pyx_t_4) < 0) __PYX_ERR(0, 567, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Get, __pyx_t_4) < 0) __PYX_ERR(0, 572, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":623
+  /* "viur/datastore/transport.pyx":628
  * 		return [res.get(x) for x in keys]  # Sort by order of incoming keys
  * 
  * def Delete(keys: Union[Key, List[Key], Entity, List[Entity]]) -> None:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Deletes the entities stored under the given key(s).
  */
-  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_11Delete, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 623, __pyx_L1_error)
+  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_11Delete, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Delete, __pyx_t_4) < 0) __PYX_ERR(0, 623, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Delete, __pyx_t_4) < 0) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":676
+  /* "viur/datastore/transport.pyx":681
  * 			raise ValueError("Invalid number of mutation-results received")
  * 
  * def Put(entities: Union[Entity, List[Entity]]) -> Union[Entity, List[Entity]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Writes the given entities into the datastore. The entities can be from different kinds. If an entity has an
  */
-  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_13Put, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 676, __pyx_L1_error)
+  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_13Put, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Put, __pyx_t_4) < 0) __PYX_ERR(0, 676, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Put, __pyx_t_4) < 0) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":737
+  /* "viur/datastore/transport.pyx":742
  * 
  * 
  * def RunInTransaction(callback: callable, *args, **kwargs) -> Any:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Runs the given function inside a AID transaction.
  */
-  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_15RunInTransaction, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 737, __pyx_L1_error)
+  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_15RunInTransaction, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RunInTransaction, __pyx_t_4) < 0) __PYX_ERR(0, 737, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RunInTransaction, __pyx_t_4) < 0) __PYX_ERR(0, 742, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":829
+  /* "viur/datastore/transport.pyx":834
  * 
  * 
  * def _rollbackTxn(txnKey: str):             # <<<<<<<<<<<<<<
  * 	"""
  * 		Internal helper that aborts the given transaction. It's important to abort pending transactions (instead
  */
-  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_17_rollbackTxn, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 829, __pyx_L1_error)
+  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_17_rollbackTxn, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 834, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rollbackTxn, __pyx_t_4) < 0) __PYX_ERR(0, 829, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rollbackTxn, __pyx_t_4) < 0) __PYX_ERR(0, 834, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":845
+  /* "viur/datastore/transport.pyx":850
  * 	)
  * 
  * def AllocateIDs(keys: Union[Key, List[Key]]) -> Union[Key, List[Key]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Allocates numeric IDs for the keys given.
  */
-  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_19AllocateIDs, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 845, __pyx_L1_error)
+  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_19AllocateIDs, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 850, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_AllocateIDs, __pyx_t_4) < 0) __PYX_ERR(0, 845, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_AllocateIDs, __pyx_t_4) < 0) __PYX_ERR(0, 850, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "viur/datastore/transport.pyx":900
+  /* "viur/datastore/transport.pyx":905
  * 		raise ValueError("Invalid data received from Datastore API")
  * 
  * def Count(kind: str = None, up_to= 2 ** 63 - 1, queryDefinition: QueryDefinition = None) -> Union[Key, List[Key]]:             # <<<<<<<<<<<<<<
  * 	"""
  * 		Count all entries in a kind if there is only a kind is provided
  */
-  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_21Count, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 900, __pyx_L1_error)
+  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_4viur_9datastore_9transport_21Count, NULL, __pyx_n_s_viur_datastore_transport); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 905, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Count, __pyx_t_4) < 0) __PYX_ERR(0, 900, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Count, __pyx_t_4) < 0) __PYX_ERR(0, 905, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "viur/datastore/transport.pyx":1
  * # distutils: sources = src/viur/datastore/simdjson.cpp             # <<<<<<<<<<<<<<
  * # distutils: language = c++
  * # cython: language_level=3
  */
```

### Comparing `viur-datastore-1.3.8/src/viur/datastore/transport.pyx` & `viur-datastore-1.3.9/src/viur/datastore/transport.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -542,15 +542,20 @@
 			print("INVALID RESPONSE RECEIVED")
 			pprint.pprint(json.loads(req.content))
 		#	res.update(toEntityStructure(element.at_key("batch"), isInitial=True))
 		element = element.at_key("batch")
 		if element.at_pointer("/entityResults").error() == SUCCESS:
 			res.extend(toEntityStructure(element.at_key("entityResults"), isInitial=False))
 		else:  # No results received
-			break
+			if toPyStr(element.at_key("moreResults").get_string()) == "NOT_FINISHED":
+				logging.warning("Query not finished. Maybe some entries are missing.")
+				logging.warning("Queried %s with filter %s and orders %s. - Please create a matching index" % (
+					queryDefinition.kind, queryDefinition.filters, queryDefinition.orders))
+			else:
+				break
 		if toPyStr(element.at_key("moreResults").get_string()) == "NO_MORE_RESULTS":
 			internalStartCursor = None
 		else:
 			internalStartCursor = toPyStr(element.at_key("endCursor").get_string())
 		if toPyStr(element.at_key("moreResults").get_string()) != "NOT_FINISHED" or len(res) == limit:
 			break
 	queryDefinition.currentCursor = internalStartCursor
```

### Comparing `viur-datastore-1.3.8/src/viur/datastore/types.py` & `viur-datastore-1.3.9/src/viur/datastore/types.py`

 * *Files identical despite different names*

### Comparing `viur-datastore-1.3.8/src/viur/datastore/utils.py` & `viur-datastore-1.3.9/src/viur/datastore/utils.py`

 * *Files identical despite different names*

### Comparing `viur-datastore-1.3.8/src/viur_datastore.egg-info/PKG-INFO` & `viur-datastore-1.3.9/src/viur_datastore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-datastore
-Version: 1.3.8
+Version: 1.3.9
 Summary: A faster replacement for google-cloud-datastore
 Home-page: https://github.com/viur-framework/viur-datastore
 Author: Tobias Steinrücken, Stefan Kögl
 Author-email: devs@viur.dev
 Maintainer: Stefan Kögl
 Maintainer-email: devs@viur.dev
 Classifier: Programming Language :: Python :: 3
```

### Comparing `viur-datastore-1.3.8/src/viur_datastore.egg-info/SOURCES.txt` & `viur-datastore-1.3.9/src/viur_datastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

