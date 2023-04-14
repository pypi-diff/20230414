# Comparing `tmp/pht_train_container_library-2.0.2.tar.gz` & `tmp/pht_train_container_library-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pht_train_container_library-2.0.2.tar", max compression
+gzip compressed data, was "pht_train_container_library-2.0.4.tar", max compression
```

## Comparing `pht_train_container_library-2.0.2.tar` & `pht_train_container_library-2.0.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1068 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/LICENSE.txt
--rw-r--r--   0        0        0     5852 2023-03-07 12:16:53.453164 pht_train_container_library-2.0.2/README.md
--rw-r--r--   0        0        0     1826 2023-03-30 14:42:44.115410 pht_train_container_library-2.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/__init__.py
--rw-r--r--   0        0        0       32 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/clients/__init__.py
--rw-r--r--   0        0        0      107 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/clients/fhir/__init__.py
--rw-r--r--   0        0        0    19926 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/clients/fhir/fhir_client.py
--rw-r--r--   0        0        0     2509 2023-03-07 12:14:19.038419 pht_train_container_library-2.0.2/train_lib/clients/fhir/fhir_k_anonymity.py
--rw-r--r--   0        0        0     3788 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/clients/fhir/fhir_query_builder.py
--rw-r--r--   0        0        0      297 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/clients/fhir/minimal_query.json
--rw-r--r--   0        0        0      758 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/clients/fhir/query.json
--rw-r--r--   0        0        0       16 2023-03-30 14:37:53.022014 pht_train_container_library-2.0.2/train_lib/docker_util/__init__.py
--rw-r--r--   0        0        0     4933 2023-03-30 14:41:16.291214 pht_train_container_library-2.0.2/train_lib/docker_util/docker_ops.py
--rw-r--r--   0        0        0     6219 2023-03-30 14:41:16.691214 pht_train_container_library-2.0.2/train_lib/docker_util/validate_master_image.py
--rw-r--r--   0        0        0        1 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/security/__init__.py
--rw-r--r--   0        0        0     4436 2023-03-07 12:17:00.953436 pht_train_container_library-2.0.2/train_lib/security/encryption.py
--rw-r--r--   0        0        0      248 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/security/errors.py
--rw-r--r--   0        0        0     2543 2023-03-07 12:16:53.463164 pht_train_container_library-2.0.2/train_lib/security/hashing.py
--rw-r--r--   0        0        0     1483 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/security/homomorphic_addition.py
--rw-r--r--   0        0        0     6336 2023-03-07 12:16:53.463164 pht_train_container_library-2.0.2/train_lib/security/key_manager.py
--rw-r--r--   0        0        0     1772 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/security/primes.py
--rw-r--r--   0        0        0    32677 2023-03-30 14:41:17.171215 pht_train_container_library-2.0.2/train_lib/security/protocol.py
--rw-r--r--   0        0        0     2628 2023-03-07 12:41:46.414956 pht_train_container_library-2.0.2/train_lib/security/train_config.py
--rw-r--r--   0        0        0    11507 2023-03-30 14:41:16.301214 pht_train_container_library-2.0.2/train_lib/tests/conftest.py
--rw-r--r--   0        0        0    10607 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/tests/test_fhir_functionality.py
--rw-r--r--   0        0        0     2425 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/tests/test_homomorphic_addition.py
--rw-r--r--   0        0        0      116 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.2/train_lib/tests/test_key_manager.py
--rw-r--r--   0        0        0     5127 2023-03-07 12:17:04.923592 pht_train_container_library-2.0.2/train_lib/tests/test_security_functions.py
--rw-r--r--   0        0        0    23503 2023-03-07 12:17:05.793630 pht_train_container_library-2.0.2/train_lib/tests/test_security_protocol.py
--rw-r--r--   0        0        0     7602 2023-03-27 15:40:16.372314 pht_train_container_library-2.0.2/train_lib/tests/test_validate_master_image.py
--rw-r--r--   0        0        0     6575 1970-01-01 00:00:00.000000 pht_train_container_library-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     5852 2023-03-07 12:16:53.453164 pht_train_container_library-2.0.4/README.md
+-rw-r--r--   0        0        0     1848 2023-04-12 13:19:41.590587 pht_train_container_library-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/__init__.py
+-rw-r--r--   0        0        0       32 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/clients/__init__.py
+-rw-r--r--   0        0        0      107 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/clients/fhir/__init__.py
+-rw-r--r--   0        0        0    19926 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/clients/fhir/fhir_client.py
+-rw-r--r--   0        0        0     2509 2023-03-07 12:14:19.038419 pht_train_container_library-2.0.4/train_lib/clients/fhir/fhir_k_anonymity.py
+-rw-r--r--   0        0        0     3788 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/clients/fhir/fhir_query_builder.py
+-rw-r--r--   0        0        0      297 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/clients/fhir/minimal_query.json
+-rw-r--r--   0        0        0      758 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/clients/fhir/query.json
+-rw-r--r--   0        0        0       14 2023-04-12 10:34:43.891083 pht_train_container_library-2.0.4/train_lib/docker_util/__init__.py
+-rw-r--r--   0        0        0     6596 2023-04-12 12:11:47.347039 pht_train_container_library-2.0.4/train_lib/docker_util/docker_ops.py
+-rw-r--r--   0        0        0     6219 2023-03-30 14:41:16.691214 pht_train_container_library-2.0.4/train_lib/docker_util/validate_master_image.py
+-rw-r--r--   0        0        0        1 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/security/__init__.py
+-rw-r--r--   0        0        0      257 2023-04-12 13:21:36.885381 pht_train_container_library-2.0.4/train_lib/security/constants.py
+-rw-r--r--   0        0        0     4436 2023-03-07 12:17:00.953436 pht_train_container_library-2.0.4/train_lib/security/encryption.py
+-rw-r--r--   0        0        0      248 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/security/errors.py
+-rw-r--r--   0        0        0     2543 2023-03-07 12:16:53.463164 pht_train_container_library-2.0.4/train_lib/security/hashing.py
+-rw-r--r--   0        0        0     1483 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/security/homomorphic_addition.py
+-rw-r--r--   0        0        0     6336 2023-03-07 12:16:53.463164 pht_train_container_library-2.0.4/train_lib/security/key_manager.py
+-rw-r--r--   0        0        0     1772 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/security/primes.py
+-rw-r--r--   0        0        0    32244 2023-04-12 12:11:47.497039 pht_train_container_library-2.0.4/train_lib/security/protocol.py
+-rw-r--r--   0        0        0     2628 2023-03-07 12:41:46.414956 pht_train_container_library-2.0.4/train_lib/security/train_config.py
+-rw-r--r--   0        0        0    11507 2023-03-30 14:41:16.301214 pht_train_container_library-2.0.4/train_lib/tests/conftest.py
+-rw-r--r--   0        0        0    10607 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/tests/test_fhir_functionality.py
+-rw-r--r--   0        0        0     2425 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/tests/test_homomorphic_addition.py
+-rw-r--r--   0        0        0      116 2023-03-04 08:26:17.804579 pht_train_container_library-2.0.4/train_lib/tests/test_key_manager.py
+-rw-r--r--   0        0        0     5127 2023-03-07 12:17:04.923592 pht_train_container_library-2.0.4/train_lib/tests/test_security_functions.py
+-rw-r--r--   0        0        0    23503 2023-03-07 12:17:05.793630 pht_train_container_library-2.0.4/train_lib/tests/test_security_protocol.py
+-rw-r--r--   0        0        0     7602 2023-03-27 15:40:16.372314 pht_train_container_library-2.0.4/train_lib/tests/test_validate_master_image.py
+-rw-r--r--   0        0        0     6575 1970-01-01 00:00:00.000000 pht_train_container_library-2.0.4/PKG-INFO
```

### Comparing `pht_train_container_library-2.0.2/LICENSE.txt` & `pht_train_container_library-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/README.md` & `pht_train_container_library-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/pyproject.toml` & `pht_train_container_library-2.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pht-train-container-library"
-version = "2.0.2"
+version = "2.0.4"
 description = "Python library for handling containerized PHT trains"
 authors = ["Michael Graf <michael.graf@uni-tuebingen.com>"]
 readme = "README.md"
 packages = [{include = "train_lib"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -26,14 +26,15 @@
 python-dotenv = "^0.21.0"
 pytest-dotenv = "^0.5.2"
 pytest-asyncio = "^0.20.3"
 pre-commit = "^2.21.0"
 tox = "*"
 mkdocs = "*"
 mkdocs-material = "*"
+ipykernel = "^6.22.0"
 
 
 
 [tool.ruff]
 line-length = 120
```

### Comparing `pht_train_container_library-2.0.2/train_lib/clients/fhir/fhir_client.py` & `pht_train_container_library-2.0.4/train_lib/clients/fhir/fhir_client.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/clients/fhir/fhir_k_anonymity.py` & `pht_train_container_library-2.0.4/train_lib/clients/fhir/fhir_k_anonymity.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/clients/fhir/fhir_query_builder.py` & `pht_train_container_library-2.0.4/train_lib/clients/fhir/fhir_query_builder.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/clients/fhir/query.json` & `pht_train_container_library-2.0.4/train_lib/clients/fhir/query.json`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/docker_util/validate_master_image.py` & `pht_train_container_library-2.0.4/train_lib/docker_util/validate_master_image.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/security/encryption.py` & `pht_train_container_library-2.0.4/train_lib/security/encryption.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/security/hashing.py` & `pht_train_container_library-2.0.4/train_lib/security/hashing.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/security/homomorphic_addition.py` & `pht_train_container_library-2.0.4/train_lib/security/homomorphic_addition.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/security/key_manager.py` & `pht_train_container_library-2.0.4/train_lib/security/key_manager.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/security/primes.py` & `pht_train_container_library-2.0.4/train_lib/security/primes.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/security/protocol.py` & `pht_train_container_library-2.0.4/train_lib/security/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import tarfile
 import time
-from enum import Enum
 from io import BytesIO
 from tarfile import TarInfo
 from typing import BinaryIO, List, Tuple, Union
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import padding, utils
@@ -17,35 +16,25 @@
 import docker.models
 from train_lib.docker_util import TIMEOUT
 from train_lib.docker_util.docker_ops import (
     display_archive_content,
     extract_archive,
     extract_query_json,
     files_from_archive,
+    rebase_train_image,
     result_files_from_archive,
 )
+from train_lib.security.constants import TrainPaths
 from train_lib.security.encryption import FileEncryptor
 from train_lib.security.errors import ValidationError
 from train_lib.security.hashing import hash_immutable_files, hash_results
 from train_lib.security.key_manager import KeyManager
 from train_lib.security.train_config import RouteEntry, TrainConfig
 
 
-class TrainPaths(Enum):
-    IMMUTABLE_DIR = "/opt/pht_train"
-    RESULT_DIR = "/opt/pht_results"
-    CONFIG_PATH = "/opt/train_config.json"
-
-
-class TrainTags(Enum):
-    LATEST = "latest"
-    BASE = "base"
-    DECRYPTED = "decrypted"
-
-
 class SecurityProtocol:
     """
     Class that performs the security protocol outlined in the security concept
 
     :param station_id: PID used to identify the station and to access the correct security values inside the
         train_config.json
 
@@ -220,17 +209,22 @@
             img,
             results_archive=results_archive,
             results_path="/opt",
             config_path="/opt",
             train_files=encrypted_files,
             file_names=file_names,
             query=query,
-            rebase=rebase,
         )
 
+        if rebase:
+            base_image = self._get_base_image(img)
+
+            # Rebase the image on the latest version of the base image
+            rebase_train_image(base_image=base_image, train_image=img)
+
         logger.info(f"Successfully executed post run protocol on img: {img}")
 
     def extract_immutable_files(
         self,
         img: str,
         directory: str,
         symmetric_key: bytes = None,
@@ -336,15 +330,14 @@
         )
         results_hash = hash_results(
             files, session_id=bytes.fromhex(self.config.session_id), binary_files=True
         )
         if results_hash != bytes.fromhex(self.config.result_hash):
             raise ValidationError("Previous results have changed")
         try:
-
             station_public_key.verify(
                 signature=bytes.fromhex(self.config.result_signature),
                 data=results_hash,
                 padding=padding.PSS(
                     mgf=padding.MGF1(hashes.SHA512()),
                     salt_length=padding.PSS.MAX_LENGTH,
                 ),
@@ -404,15 +397,14 @@
 
         sorted_route = sorted(self.config.route, key=lambda x: x.index)
 
         for stop in sorted_route:
             if stop.index >= self.route_stop.index:
                 break
             else:
-
                 if not stop.signature:
                     error = ValidationError(
                         f"Missing digital signature for previous stop {stop}. \n"
                         f" While currently at {self.route_stop}"
                     )
                     logger.error(error)
                     raise error
@@ -445,15 +437,14 @@
                 bytes.fromhex(content),
                 padding.PKCS1v15(),
                 hashes.SHA512(),
             )
             logger.info("OK")
 
         except Exception as e:
-
             logger.error(f"Error\n {e}")
             raise ValidationError("Error validating build signature.")
 
     def encrypt_immutable_files(
         self, files: List[BytesIO], symmetric_key: bytes, query=None
     ):
         """
@@ -550,38 +541,28 @@
         img: str,
         results_archive: BytesIO = None,
         results_path: str = "/opt",
         config_path: str = None,
         train_files: List[BytesIO] = None,
         file_names: List[str] = None,
         query: bytes = None,
-        rebase: bool = False,
         tag: str = "latest",
     ):
         """
         Update the base image with the encrypted results files and the updated train_config.json and tag it as
         latest.
 
         """
         # If a config path is given update the train config inside the container
         client = (
             self.docker_client
             if self.docker_client
             else docker.from_env(timeout=TIMEOUT)
         )
-
-        # if rebase create container based on base image
-        if rebase:
-            logger.info("Rebasing image")
-            # get base image
-            base_img = self._get_base_image(img)
-            # create container based on base image
-            container = client.containers.create(base_img)
-        else:
-            container = client.containers.create(img)
+        container = client.containers.create(img)
 
         if config_path:
             logger.info("Updating train config")
             config_archive = self._make_train_config_archive()
             config_archive.seek(0)
             # add_archive(img, config_archive, config_path)
             container.put_archive(config_path, config_archive)
@@ -618,14 +599,15 @@
             train_archive.seek(0)
             # add the train archive to the image
             container.put_archive("/opt", train_archive)
             container.wait()
 
         # Tag container as latest
         self._commit_to_image(container, img, tag)
+        container.remove()
 
     @staticmethod
     def _make_results_archive(archive_members, file_members, updated_files):
         """
         Creates a tar archive containing the updated results
 
         :param archive_members: tar directory structure of the pht_results directory
@@ -708,15 +690,14 @@
             docker_tag = img_split[-1]
 
         logger.debug(
             f"Committing Container ({container.id}) to image ({repo}:{docker_tag})"
         )
         container.commit(repository=repo, tag=docker_tag)
         container.wait()
-        container.remove()
 
     @staticmethod
     def _make_train_files_archive(
         train_files: List[BytesIO], file_names: List[str], query: BytesIO = None
     ) -> BytesIO:
         """
         Create a tar archive containing the train files and the query file
@@ -738,15 +719,14 @@
             info.mtime = time.time()
             tar.addfile(info, query)
 
         for i, train_file in enumerate(train_files):
             name = f"pht_train/{file_names[i]}"
             train_file.seek(0)
             logger.debug(f"Adding train file: {name} to archive")
-            logger.debug(train_file.read())
             train_file.seek(0)
             info = TarInfo(name=name)
             info.size = train_file.getbuffer().nbytes
             info.mtime = time.time()
             # add config data and reset the archive
             tar.addfile(info, train_file)
         tar.close()
@@ -773,15 +753,14 @@
         archive_obj.seek(0)
         return archive_obj
 
     def _make_user_key(self):
         archive_obj = BytesIO()
         tar = tarfile.open(fileobj=archive_obj, mode="w")
         # Extract user key from config and convert it to bytesio
-        print(self.config.creator)
         data = BytesIO(bytes.fromhex(self.config.creator.encrypted_key))
         info = TarInfo(name="user_sym_key.key")
         info.size = data.getbuffer().nbytes
         info.mtime = time.time()
         tar.addfile(info, data)
         tar.close()
         archive_obj.seek(0)
@@ -805,15 +784,15 @@
         """
         Parses the exported files from a container and sorts them into relevant categories
         :param target_dir: directory in which to find all files
         :return: Tuple consisting of lists of paths for the different file types
         """
         files = list()
         logger.info("Detecting files...")
-        for (dir_path, dir_names, file_names) in os.walk(target_dir):
+        for dir_path, dir_names, file_names in os.walk(target_dir):
             files += [os.path.join(dir_path, file) for file in file_names]
         logger.info(f"Found {len(files)} Files")
         return files
 
     def _update_symmetric_keys(self, new_sym_key: bytes):
         """
         Updates the symmetric key for the train creator and all stations on the route
```

### Comparing `pht_train_container_library-2.0.2/train_lib/security/train_config.py` & `pht_train_container_library-2.0.4/train_lib/security/train_config.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/tests/conftest.py` & `pht_train_container_library-2.0.4/train_lib/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/tests/test_fhir_functionality.py` & `pht_train_container_library-2.0.4/train_lib/tests/test_fhir_functionality.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/tests/test_homomorphic_addition.py` & `pht_train_container_library-2.0.4/train_lib/tests/test_homomorphic_addition.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/tests/test_security_functions.py` & `pht_train_container_library-2.0.4/train_lib/tests/test_security_functions.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/tests/test_security_protocol.py` & `pht_train_container_library-2.0.4/train_lib/tests/test_security_protocol.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/train_lib/tests/test_validate_master_image.py` & `pht_train_container_library-2.0.4/train_lib/tests/test_validate_master_image.py`

 * *Files identical despite different names*

### Comparing `pht_train_container_library-2.0.2/PKG-INFO` & `pht_train_container_library-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pht-train-container-library
-Version: 2.0.2
+Version: 2.0.4
 Summary: Python library for handling containerized PHT trains
 Author: Michael Graf
 Author-email: michael.graf@uni-tuebingen.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

