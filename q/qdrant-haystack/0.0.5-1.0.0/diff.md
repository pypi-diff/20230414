# Comparing `tmp/qdrant_haystack-0.0.5.tar.gz` & `tmp/qdrant_haystack-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_haystack-0.0.5.tar", max compression
+gzip compressed data, was "qdrant_haystack-1.0.0.tar", max compression
```

## Comparing `qdrant_haystack-0.0.5.tar` & `qdrant_haystack-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-04-07 15:46:44.909403 qdrant_haystack-0.0.5/LICENSE
--rw-r--r--   0        0        0     3160 2023-04-07 15:46:44.909403 qdrant_haystack-0.0.5/README.md
--rw-r--r--   0        0        0      746 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      100 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/src/qdrant_haystack/__init__.py
--rw-r--r--   0        0        0      107 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/__init__.py
--rw-r--r--   0        0        0     2285 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/converters.py
--rw-r--r--   0        0        0     8295 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/filters.py
--rw-r--r--   0        0        0    19054 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/qdrant.py
--rw-r--r--   0        0        0        0 2023-04-07 15:46:44.913403 qdrant_haystack-0.0.5/src/qdrant_haystack/utils.py
--rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 qdrant_haystack-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-14 09:42:32.838009 qdrant_haystack-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3160 2023-04-14 09:42:32.838009 qdrant_haystack-1.0.0/README.md
+-rw-r--r--   0        0        0      746 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/src/qdrant_haystack/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0     2285 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/converters.py
+-rw-r--r--   0        0        0     8295 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/filters.py
+-rw-r--r--   0        0        0    20253 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/qdrant.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/src/qdrant_haystack/utils.py
+-rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 qdrant_haystack-1.0.0/PKG-INFO
```

### Comparing `qdrant_haystack-0.0.5/LICENSE` & `qdrant_haystack-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-0.0.5/README.md` & `qdrant_haystack-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-0.0.5/pyproject.toml` & `qdrant_haystack-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "qdrant-haystack"
-version = "0.0.5"
+version = "1.0.0"
 description = "An integration of Qdrant ANN vector database backend with Haystack"
 authors = ["Kacper Łukawski <kacper.lukawski@qdrant.com>"]
 packages = [
     {include = "qdrant_haystack", from = "src"}
 ]
 readme = "README.md"
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<=3.11"
-qdrant-client = "^1.1.2"
+qdrant-client = "^1.1.4"
 farm-haystack = "^1.13.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 pre-commit = "^3.1.0"
 black = "^23.1.0"
 isort = "^5.12.0"
```

### Comparing `qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/converters.py` & `qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/filters.py` & `qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-0.0.5/src/qdrant_haystack/document_stores/qdrant.py` & `qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/qdrant.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 from typing import Any, Dict, Generator, List, Optional, Union, cast
 
 import numpy as np
 import qdrant_client
-from grpc._channel import _InactiveRpcError
+from grpc import RpcError
 from haystack import Document, Label
 from haystack.document_stores import BaseDocumentStore
 from haystack.document_stores.base import get_batches_from_generator
 from haystack.errors import DocumentStoreError
 from haystack.nodes import DenseRetriever
 from haystack.schema import FilterType
 from qdrant_client import grpc
+from qdrant_client.conversions import common_types as types
 from qdrant_client.http import models as rest
 from qdrant_client.http.exceptions import UnexpectedResponse
 from tqdm import tqdm
 
 from qdrant_haystack.document_stores.converters import (
     HaystackToQdrant,
     QdrantToHaystack,
@@ -46,23 +47,31 @@
         api_key: Optional[str] = None,
         prefix: Optional[str] = None,
         timeout: Optional[float] = None,
         host: Optional[str] = None,
         path: Optional[str] = None,
         index: str = "Document",
         embedding_dim: int = 768,
-        hnsw_config: Optional[Dict] = None,
         content_field: str = "content",
         name_field: str = "name",
         embedding_field: str = "vector",
         similarity: str = "cosine",
         return_embedding: bool = False,
         progress_bar: bool = True,
         duplicate_documents: str = "overwrite",
         recreate_index: bool = False,
+        shard_number: Optional[int] = None,
+        replication_factor: Optional[int] = None,
+        write_consistency_factor: Optional[int] = None,
+        on_disk_payload: Optional[bool] = None,
+        hnsw_config: Optional[Union[types.HnswConfigDiff, dict]] = None,
+        optimizers_config: Optional[types.OptimizersConfigDiff] = None,
+        wal_config: Optional[types.WalConfigDiff] = None,
+        quantization_config: Optional[types.QuantizationConfig] = None,
+        init_from: Optional[types.InitFrom] = None,
         **kwargs,
     ):
         super().__init__()
 
         self.client = qdrant_client.QdrantClient(
             location=location,
             url=url,
@@ -74,23 +83,32 @@
             prefix=prefix,
             timeout=timeout,
             host=host,
             path=path,
             **kwargs,
         )
 
-        self._set_up_collection(
-            index, embedding_dim, hnsw_config, recreate_index, similarity
-        )
+        # Store the Qdrant specific attributes
+        self.shard_number = shard_number
+        self.replication_factor = replication_factor
+        self.write_consistency_factor = write_consistency_factor
+        self.on_disk_payload = on_disk_payload
+        self.hnsw_config = hnsw_config
+        self.optimizers_config = optimizers_config
+        self.wal_config = wal_config
+        self.quantization_config = quantization_config
+        self.init_from = init_from
+
+        # Make sure the collection is properly set up
+        self._set_up_collection(index, embedding_dim, recreate_index, similarity)
 
         self.embedding_dim = embedding_dim
         self.content_field = content_field
         self.name_field = name_field
         self.embedding_field = embedding_field
-        self.hnsw_config = hnsw_config
         self.similarity = similarity
         self.index = index
         self.return_embedding = return_embedding
         self.progress_bar = progress_bar
         self.duplicate_documents = duplicate_documents
         self.qdrant_filter_converter = QdrantFilterConverter()
         self.haystack_to_qdrant_converter = HaystackToQdrant()
@@ -255,17 +273,15 @@
         documents: Union[List[dict], List[Document]],
         index: Optional[str] = None,
         batch_size: int = 10_000,
         duplicate_documents: Optional[str] = None,
         headers: Optional[Dict[str, str]] = None,
     ):
         index = index or self.index
-        self._set_up_collection(
-            index, self.embedding_dim, self.hnsw_config, False, self.similarity
-        )
+        self._set_up_collection(index, self.embedding_dim, False, self.similarity)
         field_map = self._create_document_field_map()
 
         duplicate_documents = duplicate_documents or self.duplicate_documents
         assert (
             duplicate_documents in self.duplicate_documents_options
         ), f"duplicate_documents parameter must be {', '.join(self.duplicate_documents_options)}"
 
@@ -476,42 +492,37 @@
                 f"{', '.join(self.SIMILARITY.keys())}"
             )
 
     def _set_up_collection(
         self,
         collection_name: str,
         embedding_dim: int,
-        hnsw_config: dict,
         recreate_collection: bool,
         similarity: str,
     ):
         distance = self._get_distance(similarity)
 
         if recreate_collection:
             # There is no need to verify the current configuration of that
             # collection. It might be just recreated again.
-            self._recreate_collection(
-                collection_name, distance, embedding_dim, hnsw_config
-            )
+            self._recreate_collection(collection_name, distance, embedding_dim)
             return
 
         try:
             # Check if the collection already exists and validate its
             # current configuration with the parameters.
             collection_info = self.client.get_collection(collection_name)
-        except (UnexpectedResponse, _InactiveRpcError, ValueError):
+        except (UnexpectedResponse, RpcError, ValueError):
             # That indicates the collection does not exist, so it can be
             # safely created with any configuration.
             #
             # Qdrant local raises ValueError if the collection is not found, but
-            # with the remote server UnexpectedResponse / _InactiveRpcError is raised.
+            # with the remote server UnexpectedResponse / RpcError is raised.
             # Until that's unified, we need to catch both.
-            self._recreate_collection(
-                collection_name, distance, embedding_dim, hnsw_config
-            )
+            self._recreate_collection(collection_name, distance, embedding_dim)
             return
 
         current_distance = collection_info.config.params.vectors.distance
         current_vector_size = collection_info.config.params.vectors.size
 
         if current_distance != distance:
             raise ValueError(
@@ -525,18 +536,24 @@
             raise ValueError(
                 f"Collection '{collection_name}' already exists in Qdrant, "
                 f"but it is configured with a vector size '{current_vector_size}'. "
                 f"If you want to use that collection, but with a different "
                 f"vector size, please set `recreate_collection=True` argument."
             )
 
-    def _recreate_collection(
-        self, collection_name, distance, embedding_dim, hnsw_config
-    ):
+    def _recreate_collection(self, collection_name: str, distance, embedding_dim: int):
         self.client.recreate_collection(
             collection_name=collection_name,
             vectors_config=rest.VectorParams(
                 size=embedding_dim,
                 distance=distance,
             ),
-            hnsw_config=hnsw_config,
+            shard_number=self.shard_number,
+            replication_factor=self.replication_factor,
+            write_consistency_factor=self.write_consistency_factor,
+            on_disk_payload=self.on_disk_payload,
+            hnsw_config=self.hnsw_config,
+            optimizers_config=self.optimizers_config,
+            wal_config=self.wal_config,
+            quantization_config=self.quantization_config,
+            init_from=self.init_from,
         )
```

### Comparing `qdrant_haystack-0.0.5/PKG-INFO` & `qdrant_haystack-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: qdrant-haystack
-Version: 0.0.5
+Version: 1.0.0
 Summary: An integration of Qdrant ANN vector database backend with Haystack
 License: Apache 2.0
 Author: Kacper Łukawski
 Author-email: kacper.lukawski@qdrant.com
 Requires-Python: >=3.8.1,<=3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: farm-haystack (>=1.13.0,<2.0.0)
-Requires-Dist: qdrant-client (>=1.1.2,<2.0.0)
+Requires-Dist: qdrant-client (>=1.1.4,<2.0.0)
 Description-Content-Type: text/markdown
 
 # qdrant-haystack
 
 An integration of [Qdrant](https://qdrant.tech) vector database with [Haystack](https://haystack.deepset.ai/)
 by [deepset](https://www.deepset.ai).
```

