# Comparing `tmp/taigapy-3.3.4-py2.py3-none-any.whl.zip` & `tmp/taigapy-3.3.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 24200 bytes, number of entries: 14
--rw-r--r--  2.0 unx      388 b- defN 22-Jun-09 15:33 taigapy/__init__.py
--rw-r--r--  2.0 unx    38183 b- defN 22-Jun-08 19:54 taigapy/client.py
--rw-r--r--  2.0 unx      272 b- defN 22-Apr-27 15:36 taigapy/consts.py
--rw-r--r--  2.0 unx     1331 b- defN 22-Apr-27 15:36 taigapy/custom_exceptions.py
--rw-r--r--  2.0 unx     1565 b- defN 22-Apr-27 15:36 taigapy/figshare.py
--rw-r--r--  2.0 unx    13324 b- defN 22-Jun-08 17:35 taigapy/taiga_api.py
--rw-r--r--  2.0 unx    13425 b- defN 22-Jun-08 17:35 taigapy/taiga_cache.py
--rw-r--r--  2.0 unx     8449 b- defN 22-Jun-08 17:35 taigapy/types.py
--rw-r--r--  2.0 unx     8425 b- defN 22-Jun-08 17:35 taigapy/utils.py
--rwxr-xr-x  2.0 unx     4337 b- defN 22-Jun-09 15:52 taigapy-3.3.4.data/scripts/taigaclient
--rw-r--r--  2.0 unx     6125 b- defN 22-Jun-09 15:52 taigapy-3.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Jun-09 15:52 taigapy-3.3.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 22-Jun-09 15:52 taigapy-3.3.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1081 b- defN 22-Jun-09 15:52 taigapy-3.3.4.dist-info/RECORD
-14 files, 97023 bytes uncompressed, 22434 bytes compressed:  76.9%
+Zip file size: 24376 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      388 b- defN 23-Apr-14 14:56 taigapy/__init__.py
+-rw-r--r--  2.0 unx    38827 b- defN 23-Apr-13 19:24 taigapy/client.py
+-rw-r--r--  2.0 unx      272 b- defN 23-Mar-01 23:08 taigapy/consts.py
+-rw-r--r--  2.0 unx     1331 b- defN 23-Mar-01 23:08 taigapy/custom_exceptions.py
+-rw-r--r--  2.0 unx     1565 b- defN 23-Mar-01 23:08 taigapy/figshare.py
+-rw-r--r--  2.0 unx    13324 b- defN 23-Mar-06 18:27 taigapy/taiga_api.py
+-rw-r--r--  2.0 unx    13425 b- defN 23-Mar-01 23:08 taigapy/taiga_cache.py
+-rw-r--r--  2.0 unx     9211 b- defN 23-Apr-13 19:24 taigapy/types.py
+-rw-r--r--  2.0 unx     8425 b- defN 23-Mar-01 23:08 taigapy/utils.py
+-rwxr-xr-x  2.0 unx     4337 b- defN 23-Apr-14 15:17 taigapy-3.3.5.data/scripts/taigaclient
+-rw-r--r--  2.0 unx     6442 b- defN 23-Apr-14 15:17 taigapy-3.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:17 taigapy-3.3.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-14 15:17 taigapy-3.3.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1081 b- defN 23-Apr-14 15:17 taigapy-3.3.5.dist-info/RECORD
+14 files, 98746 bytes uncompressed, 22610 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: taigapy/types.py
 Comment: 
 
 Filename: taigapy/utils.py
 Comment: 
 
-Filename: taigapy-3.3.4.data/scripts/taigaclient
+Filename: taigapy-3.3.5.data/scripts/taigaclient
 Comment: 
 
-Filename: taigapy-3.3.4.dist-info/METADATA
+Filename: taigapy-3.3.5.dist-info/METADATA
 Comment: 
 
-Filename: taigapy-3.3.4.dist-info/WHEEL
+Filename: taigapy-3.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: taigapy-3.3.4.dist-info/top_level.txt
+Filename: taigapy-3.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: taigapy-3.3.4.dist-info/RECORD
+Filename: taigapy-3.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## taigapy/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.3.4"
+__version__ = "3.3.5"
 
 from .consts import DEFAULT_TAIGA_URL, DEFAULT_CACHE_DIR, CACHE_FILE
 from .client import TaigaClient
 
 try:
     default_tc = TaigaClient()
 except Exception as e:
```

## taigapy/client.py

```diff
@@ -667,21 +667,23 @@
             upload_files {Optional[Sequence[Dict[str, str]]]} -- List of files to upload, where files are provided as dictionary objects d where
                 - d["path"] is the path of the file to upload
                 - d["name"] is what the file should be named in the dataset. Uses the base name of the file if not provided
                 - d["format"] is the Format of the file (as a string).
                 And optionally,
                 - d["encoding"] is the character encoding of the file. Uses "UTF-8" if not provided
                 (default: {None})
+                - "custom_metadata" is an optional json encoded dictionary, with keys representing the metadata name, and values representing the metadata value
             add_taiga_ids {Optional[Sequence[Dict[str, str]]]} -- List of virtual datafiles to add, where files are provided as dictionary objects with keys
                 - "taiga_id" equal to the Taiga ID of the reference datafile in dataset_permaname.dataset_version/datafile_name format
                 - "name" (optional) for what the virtual datafile should be called in the new dataset (will use the reference datafile name if not provided).
                 (default: {None})
             add_gcs_files {Optional[Sequence[Dict[str, str]]} -- List of GCS objects to add where each dictionary has the keys
                 - "gcs_path" the GCS path (must start with "gs://...") of the object to associate with the provided name
                 - "name" for what the datafile should be called in the new dataset
+                - "custom_metadata" is an optional json encoded dictionary, with keys representing the metadata name, and values representing the metadata value
             folder_id {str} -- The ID of the containing folder. If not specified, will use home folder of user. (default: {None})
             upload_async {bool} -- Whether to upload asynchronously (parallel) or in serial
 
         Returns:
             Optional[str] -- The id of the new dataset, or None if the operation was not successful.
         """
         self._set_token_and_initialized_api()
@@ -747,21 +749,23 @@
             upload_files {Optional[Sequence[Dict[str, str]]]} -- Sequence of files to upload, where files are provided as dictionary objects d where
                 - d["path"] is the path of the file to upload
                 - d["name"] is what the file should be named in the dataset. Uses the base name of the file if not provided
                 - d["format"] is the Format of the file (as a string).
                 And optionally,
                 - d["encoding"] is the character encoding of the file. Uses "UTF-8" if not provided
                 (default: {None})
+                - "custom_metadata" is an optional json encoded dictionary, with keys representing the metadata name, and values representing the metadata value
             add_taiga_ids {Optional[Sequence[Dict[str, str]]]} -- Sequence of virtual datafiles to add, where files are provided as dictionary objects with keys
                 - "taiga_id" equal to the Taiga ID of the reference datafile in dataset_permaname.dataset_version/datafile_name format
                 - "name" (optional) for what the virtual datafile should be called in the new dataset (will use the reference datafile name if not provided).
                 (default: {None})
             add_gcs_files {Optional[Sequence[Dict[str, str]]} -- Sequence of GCS objects to add where each dictionary has the keys
                 - "gcs_path" the GCS path (must start with "gs://...") of the object to associate with the provided name
                 - "name" for what the datafile should be called in the new dataset
+                - "custom_metadata" is an optional json encoded dictionary, with keys representing the metadata name, and values representing the metadata value
             add_all_existing_files {bool} -- Whether to add all files from the base dataset version as virtual datafiles in the new dataset version. If a name collides with one in upload_files or add_taiga_ids, that file is ignored. (default: {False})
             upload_async {bool} -- Whether to upload asynchronously (parallel) or in serial
 
         Returns:
             Optional[str] -- The id of the new dataset version, or None if the operation was not successful.
         """
         self._set_token_and_initialized_api()
```

## taigapy/types.py

```diff
@@ -1,13 +1,13 @@
 import codecs
 import os
 
 from abc import ABC
 from enum import Enum
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 from typing_extensions import Literal, TypedDict
 
 
 class DataFileType(Enum):
     S3 = "s3"
     Virtual = "virtual"
     GCS = "gcs"
@@ -58,14 +58,15 @@
         "id": str,
         "name": str,
         "short_summary": str,
         "type": str,  # DataFileFormat
         "underlying_file_id": Optional[str],
         "original_file_md5": Optional[str],
         "original_file_sha256": Optional[str],
+        "custom_metadata": Optional[Dict[str, Any]],
     },
 )
 DatasetVersionLongDict = TypedDict(
     "DatasetVersionLongDict",
     {
         "can_edit": bool,
         "can_view": bool,
@@ -192,21 +193,28 @@
         self.prefix: str = s3_credentials_dict["prefix"]
         self.secret_access_key: str = s3_credentials_dict["secretAccessKey"]
         self.session_token: str = s3_credentials_dict["sessionToken"]
 
 
 UploadS3DataFileDict = TypedDict(
     "UploadS3DataFileDict",
-    {"path": str, "name": Optional[str], "format": str, "encoding": Optional[str]},
+    {
+        "path": str,
+        "name": Optional[str],
+        "format": str,
+        "encoding": Optional[str],
+        "custom_metadata": Optional[Dict[str, Any]],
+    },
     total=False,
 )
 
 
 class UploadDataFile(ABC):
     file_name: str
+    custom_metadata: Optional[Dict[str, Any]]
 
     def to_api_param(self):
         pass
 
 
 class UploadS3DataFile(UploadDataFile):
     def __init__(self, upload_s3_file_dict: UploadS3DataFileDict):
@@ -216,61 +224,75 @@
         if not os.path.exists(self.file_path):
             raise Exception(
                 "File '{}' does not exist.".format(upload_s3_file_dict["path"])
             )
         self.file_name = upload_s3_file_dict.get(
             "name", standardize_file_name(self.file_path)
         )
+        self.custom_metadata = upload_s3_file_dict.get("custom_metadata", None)
         self.datafile_format = DataFileUploadFormat(upload_s3_file_dict["format"])
         self.encoding = codecs.lookup(upload_s3_file_dict.get("encoding", "utf-8")).name
         self.bucket: Optional[str] = None
         self.key: Optional[str] = None
 
     def add_s3_upload_information(self, bucket: str, key: str):
         self.bucket = bucket
         self.key = key
 
     def to_api_param(self):
         return {
             "filename": self.file_name,
             "filetype": "s3",
+            "custom_metadata": self.custom_metadata,
             "s3Upload": {
                 "format": self.datafile_format.value,
                 "bucket": self.bucket,
                 "key": self.key,
                 "encoding": self.encoding,
             },
         }
 
 
 UploadVirtualDataFileDict = TypedDict(
-    "UploadVirtualDataFileDict", {"taiga_id": str, "name": str}, total=False
+    "UploadVirtualDataFileDict",
+    {"taiga_id": str, "name": str, "custom_metadata": Optional[Dict[str, Any]]},
+    total=False,
 )
 
 
 class UploadVirtualDataFile(UploadDataFile):
     def __init__(self, upload_virtual_file_dict: UploadVirtualDataFileDict):
         self.taiga_id = upload_virtual_file_dict["taiga_id"]
         self.file_name = upload_virtual_file_dict.get(
             "name", self.taiga_id.split("/", 1)[1]
         )
+        self.custom_metadata = upload_virtual_file_dict.get("custom_metadata", None)
 
     def to_api_param(self):
         return {
             "filename": self.file_name,
+            "custom_metadata": self.custom_metadata,
             "filetype": "virtual",
             "existingTaigaId": self.taiga_id,
         }
 
 
 UploadGCSDataFileDict = TypedDict(
-    "UploadGCSDataFileDict", {"gcs_path": str, "name": str}, total=False
+    "UploadGCSDataFileDict",
+    {"gcs_path": str, "name": str, "custom_metadata": Optional[Dict[str, Any]]},
+    total=False,
 )
 
 
 class UploadGCSDataFile(UploadDataFile):
     def __init__(self, upload_gsc_file_dict: UploadGCSDataFileDict):
         self.file_name = upload_gsc_file_dict["name"]
         self.gcs_path = upload_gsc_file_dict["gcs_path"]
+        self.custom_metadata = upload_gsc_file_dict.get("custom_metadata", None)
 
     def to_api_param(self):
-        return {"filename": self.file_name, "filetype": "gcs", "gcsPath": self.gcs_path}
+        return {
+            "filename": self.file_name,
+            "filetype": "gcs",
+            "gcsPath": self.gcs_path,
+            "custom_metadata": self.custom_metadata,
+        }
```

## Comparing `taigapy-3.3.4.data/scripts/taigaclient` & `taigapy-3.3.5.data/scripts/taigaclient`

 * *Files identical despite different names*

## Comparing `taigapy-3.3.4.dist-info/METADATA` & `taigapy-3.3.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: taigapy
-Version: 3.3.4
+Version: 3.3.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Remi Marenco
 Author-email: rmarenco@broadinstitute.org
 License: Creative Commons Attribution-Noncommercial-Share Alike license
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pandas (<2.0.0,>=1.0.0)
 Requires-Dist: aiobotocore (==1.2.2)
 Requires-Dist: boto3 (<1.16.53,>=1.16.0)
 Requires-Dist: nest-asyncio (<2.0.0,>=1.5.1)
 Requires-Dist: colorful
-Requires-Dist: progressbar2 (>=3.3.0<4.0.0)
+Requires-Dist: progressbar2 (<4.0.0,>=3.3.0)
 Requires-Dist: pyarrow (>=3.0.0)
 
 # taigapy
 ![Run tests](https://github.com/broadinstitute/taigapy/workflows/Run%20tests/badge.svg)
 
 Python client for fetching datafiles from and creating/updating datasets in [Taiga](https://github.com/broadinstitute/taiga).
 
@@ -97,14 +97,20 @@
     ],
     add_taiga_ids=[
         {
             "taiga_id": "achilles-v2-4-6.4/data",
             "name": "name in new dataset" # optional, will use name in referenced dataset if not provided (required if there is a name collision)
         }
     ],
+    add_gcs_files=[
+        {
+            "gcs_path": "gs://bucket_name/file_name.extension",
+            "name": "name of file in dataset",
+        }
+    ],
     folder_id="folder_id", # optional, will default to your home folder if not provided
 )
 ```
 
 #### Update dataset
 Create a new dataset in folder with id `folder_id`, with local files `upload_files` and virtual files `add_taiga_ids`.
 ```python
@@ -123,14 +129,20 @@
     ],
     add_taiga_ids=[
         {
             "taiga_id": "achilles-v2-4-6.4/data",
             "name": "name in new dataset" # optional, will use name in referenced dataset if not provided (required if there is a name collision)
         }
     ],
+    add_gcs_files=[
+        {
+            "gcs_path": "gs://bucket_name/file_name.extension",
+            "name": "name of file in dataset",
+        }
+    ],
     add_all_existing_files=True, # If True, will add all files from the base dataset version, except files with the same names as those in upload_files or add_taiga_ids
 )
 ```
 
 #### Get dataset metadata
 Get metadata about a dataset or dataset version. See fields returned in [TaigaClient API](docs/TaigaClient%20API.md#returns-4)
 ```python
```

