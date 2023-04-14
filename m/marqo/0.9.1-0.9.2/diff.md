# Comparing `tmp/marqo-0.9.1.tar.gz` & `tmp/marqo-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marqo-0.9.1.tar", last modified: Wed Apr  5 06:19:34 2023, max compression
+gzip compressed data, was "marqo-0.9.2.tar", last modified: Fri Apr 14 06:08:25 2023, max compression
```

## Comparing `marqo-0.9.1.tar` & `marqo-0.9.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:19:34.034199 marqo-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-04-05 06:19:21.000000 marqo-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-05 06:19:34.034199 marqo-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-04-05 06:19:21.000000 marqo-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-05 06:19:21.000000 marqo-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 06:19:34.034199 marqo-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-05 06:19:21.000000 marqo-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:19:34.030199 marqo-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:19:34.034199 marqo-0.9.1/src/marqo/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-05 06:19:21.000000 marqo-0.9.1/src/marqo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-05 06:19:21.000000 marqo-0.9.1/src/marqo/_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-05 06:19:21.000000 marqo-0.9.1/src/marqo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-05 06:19:21.000000 marqo-0.9.1/src/marqo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-05 06:19:21.000000 marqo-0.9.1/src/marqo/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-05 06:19:21.000000 marqo-0.9.1/src/marqo/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-05 06:19:21.000000 marqo-0.9.1/src/marqo/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26740 2023-04-05 06:19:21.000000 marqo-0.9.1/src/marqo/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-05 06:19:21.000000 marqo-0.9.1/src/marqo/marqo_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-05 06:19:21.000000 marqo-0.9.1/src/marqo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-05 06:19:21.000000 marqo-0.9.1/src/marqo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-05 06:19:21.000000 marqo-0.9.1/src/marqo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:19:34.034199 marqo-0.9.1/src/marqo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-05 06:19:34.000000 marqo-0.9.1/src/marqo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-05 06:19:34.000000 marqo-0.9.1/src/marqo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 06:19:34.000000 marqo-0.9.1/src/marqo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-05 06:19:34.000000 marqo-0.9.1/src/marqo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 06:19:34.000000 marqo-0.9.1/src/marqo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:08:25.529800 marqo-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-04-14 06:08:15.000000 marqo-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-14 06:08:25.529800 marqo-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-04-14 06:08:15.000000 marqo-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 06:08:15.000000 marqo-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:08:25.529800 marqo-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-14 06:08:15.000000 marqo-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:08:25.521799 marqo-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:08:25.525800 marqo-0.9.2/src/marqo/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/marqo_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-14 06:08:15.000000 marqo-0.9.2/src/marqo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:08:25.529800 marqo-0.9.2/src/marqo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-14 06:08:25.000000 marqo-0.9.2/src/marqo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 06:08:25.000000 marqo-0.9.2/src/marqo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:08:25.000000 marqo-0.9.2/src/marqo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 06:08:25.000000 marqo-0.9.2/src/marqo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 06:08:25.000000 marqo-0.9.2/src/marqo.egg-info/top_level.txt
```

### Comparing `marqo-0.9.1/LICENSE` & `marqo-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `marqo-0.9.1/PKG-INFO` & `marqo-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 0.9.1 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 0.9.2 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
                                     [Marqo]
```

### Comparing `marqo-0.9.1/README.md` & `marqo-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `marqo-0.9.1/setup.py` & `marqo-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "pydantic"
     ],
     tests_require=[
         "pytest",
         "tox"
     ],
     name="marqo",
-    version="0.9.1",
+    version="0.9.2",
     author="marqo org",
     author_email="org@marqo.io",
     description="Tensor search for humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", exclude=("tests*",)),
     keywords="search python marqo opensearch tensor neural semantic vector embedding",
```

### Comparing `marqo-0.9.1/src/marqo/_httprequests.py` & `marqo-0.9.2/src/marqo/_httprequests.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.1/src/marqo/client.py` & `marqo-0.9.2/src/marqo/client.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.1/src/marqo/config.py` & `marqo-0.9.2/src/marqo/config.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.1/src/marqo/defaults.py` & `marqo-0.9.2/src/marqo/defaults.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.1/src/marqo/errors.py` & `marqo-0.9.2/src/marqo/errors.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.1/src/marqo/index.py` & `marqo-0.9.2/src/marqo/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -338,17 +338,19 @@
         server_batch_size: int = None,
         client_batch_size: int = None,
         processes: int = None,
         device: str = None,
         non_tensor_fields: List = None,
         use_existing_tensors: bool = False,
         image_download_headers: dict = None,
-        mappings:dict = None
+        mappings: dict = None
     ) -> Union[Dict[str, Any], List[Dict[str, Any]]]:
 
+        error_detected_message = ('Errors detected in add documents call. '
+                                  'Please examine the returned result object for more information.')
         if non_tensor_fields is None:
             non_tensor_fields = []
 
         selected_device = device if device is not None else self.config.indexing_device
         num_docs = len(documents)
 
         # ADD DOCS TIMER-LOGGER (1)
@@ -400,42 +402,50 @@
 
 
             end_time_client_request = timer()
             total_client_request_time = end_time_client_request - start_time_client_request
 
             mq_logger.debug(f"add_documents roundtrip: took {(total_client_request_time):.3f}s to send {num_docs} "
                             f"docs to Marqo (roundtrip, unbatched), for an average of {(total_client_request_time / num_docs):.3f}s per doc.")
-
+            errors_detected = False
             if server_batch_size is not None:
                 # with Server Batching (show processing time for each batch)
                 mq_logger.debug(f"add_documents Marqo index (server-side batch reports): ")
 
                 if processes is not None and processes > 1:
                     # for multiprocess, timing messages should be arranged by process, then batch
                     for process in range(len(res)):
                         mq_logger.debug(f"   process {process}:")
 
                         for batch in range(len(res[process])):
                             server_batch_result_count = len(res[process][batch]["items"])
                             mq_logger.debug(f"       marqo server batch {batch}: "
                                             f"processed {server_batch_result_count} docs in {(res[process][batch]['processingTimeMs'] / 1000):.3f}s, "
                                             f"for an average of {(res[process][batch]['processingTimeMs'] / (1000 * server_batch_result_count)):.3f}s per doc.")
+                            if 'errors' in res[process][batch] and res[process][batch]['errors']:
+                                errors_detected = True
                 else:
                     # for single process, timing messages should be arranged by batch ONLY
                     for batch in range(len(res)):
                         server_batch_result_count = len(res[batch]["items"])
                         mq_logger.debug(f"   marqo server batch {batch}: "
                                         f"processed {server_batch_result_count} docs in {(res[batch]['processingTimeMs'] / 1000):.3f}s, "
                                         f"for an average of {(res[batch]['processingTimeMs'] / (1000 * server_batch_result_count)):.3f}s per doc.")
+                        if 'errors' in res[batch] and res[batch]['errors']:
+                            errors_detected = True
             else:
                 # no Server Batching
                 if 'processingTimeMs' in res:       # Only outputs log if response is non-empty
                     mq_logger.debug(f"add_documents Marqo index: took {(res['processingTimeMs'] / 1000):.3f}s for Marqo to process & index {num_docs} "
                                     f"docs (server unbatched), for an average of {(res['processingTimeMs'] / (1000 * num_docs)):.3f}s per doc.")
+                if 'errors' in res and res['errors']:
+                    mq_logger.info(error_detected_message)
 
+            if errors_detected:
+                mq_logger.info(error_detected_message)
         total_add_docs_time = timer() - t0
         mq_logger.debug(f"add_documents completed. total time taken: {(total_add_docs_time):.3f}s.")
         return res
 
     def delete_documents(self, ids: List[str], auto_refresh: bool = None) -> Dict[str, int]:
         """Delete documents from this index by a list of their ids.
 
@@ -488,71 +498,82 @@
         Returns:
             A list of responses, which have information about the batch
             operation
         """
         path_with_query_str = f"{base_path}?refresh=false{query_str_params}"
 
         mq_logger.debug(f"starting batch ingestion with batch size {batch_size}")
+        error_detected_message = ('Errors detected in add documents call. '
+                                  'Please examine the returned result object for more information.')
 
         deeper = ((doc, i, batch_size) for i, doc in enumerate(docs))
-
         def batch_requests(gathered, doc_tuple):
             doc, i, the_batch_size = doc_tuple
             if i % the_batch_size == 0:
                 gathered.append([doc, ])
             else:
                 gathered[-1].append(doc)
             return gathered
 
         batched = functools.reduce(lambda x, y: batch_requests(x, y), deeper, [])
 
         def verbosely_add_docs(i, docs):
+            errors_detected = False
+
             t0 = timer()
             if update_method == 'replace':
                 res = self.http.post(path=path_with_query_str, body=docs)
             elif update_method == 'update':
                 res = self.http.put(path=path_with_query_str, body=docs)
             else:
                 raise ValueError(f'Received unknown update_method `{update_method}`. '
                                  f'Allowed update_methods: ["replace", "update"] ')
             total_batch_time = timer() - t0
             num_docs = len(docs)
 
             if isinstance(res, list):
                 # with Server Batching (show processing time for each batch)
                 mq_logger.info(
-                    f"   add_documents batch {i} roundtrip: took {(total_batch_time):.3f}s to add {num_docs} docs, "
+                    f"    add_documents batch {i} roundtrip: took {(total_batch_time):.3f}s to add {num_docs} docs, "
                     f"for an average of {(total_batch_time / num_docs):.3f}s per doc.")
 
                 if isinstance(res[0], list):
                     # for multiprocess, timing messages should be arranged by process, then batch
                     for process in range(len(res)):
                         mq_logger.debug(f"       process {process}:")
 
                         for batch in range(len(res[process])):
                             server_batch_result_count = len(res[process][batch]["items"])
                             mq_logger.debug(f"           marqo server batch {batch}: "
                                             f"processed {server_batch_result_count} docs in {(res[process][batch]['processingTimeMs'] / 1000):.3f}s, "
                                             f"for an average of {(res[process][batch]['processingTimeMs'] / (1000 * server_batch_result_count)):.3f}s per doc.")
+                            if 'errors' in res[process][batch] and res[process][batch]['errors']:
+                                errors_detected = True
+
                 else:
                     # for single process, timing messages should be arranged by batch ONLY
                     for batch in range(len(res)):
                         server_batch_result_count = len(res[batch]["items"])
                         mq_logger.debug(f"       marqo server batch {batch}: "
                                         f"processed {server_batch_result_count} docs in {(res[batch]['processingTimeMs'] / 1000):.3f}s, "
                                         f"for an average of {(res[batch]['processingTimeMs'] / (1000 * server_batch_result_count)):.3f}s per doc.")
+                        if 'errors' in res[batch] and res[batch]['errors']:
+                            errors_detected = True
             else:
                 # no Server Batching
                 if 'processingTimeMs' in res:       # Only outputs log if response is non-empty
                     mq_logger.info(
-                        f"   add_documents batch {i}: took {(res['processingTimeMs'] / 1000):.3f}s for Marqo to process & index {num_docs} "
+                        f"    add_documents batch {i}: took {(res['processingTimeMs'] / 1000):.3f}s for Marqo to process & index {num_docs} "
                         f"docs (server unbatched), for an average of {(res['processingTimeMs'] / (1000 * num_docs)):.3f}s per doc."
                         f" Roundtrip time: {(total_batch_time):.3f}s")
+                    if 'errors' in res and res['errors']:
+                        errors_detected = True
 
-
+            if errors_detected:
+                mq_logger.info(f"    add_documents batch {i}: {error_detected_message}")
             if verbose:
                 mq_logger.info(f"results from indexing batch {i}: {res}")
             return res
 
         results = [verbosely_add_docs(i, docs) for i, docs in enumerate(batched)]
         if auto_refresh:
             self.refresh()
```

### Comparing `marqo-0.9.1/src/marqo/models.py` & `marqo-0.9.2/src/marqo/models.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.1/src/marqo/utils.py` & `marqo-0.9.2/src/marqo/utils.py`

 * *Files identical despite different names*

### Comparing `marqo-0.9.1/src/marqo.egg-info/PKG-INFO` & `marqo-0.9.2/src/marqo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marqo Version: 0.9.1 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 0.9.2 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE
                                     [Marqo]
```

