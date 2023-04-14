# Comparing `tmp/ml-cli-azureml-pipeline-0.0.8.tar.gz` & `tmp/ml-cli-azureml-pipeline-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-cli-azureml-pipeline-0.0.8.tar", last modified: Thu Oct 20 12:13:09 2022, max compression
+gzip compressed data, was "ml-cli-azureml-pipeline-0.0.9.tar", last modified: Thu Oct 20 13:12:36 2022, max compression
```

## Comparing `ml-cli-azureml-pipeline-0.0.8.tar` & `ml-cli-azureml-pipeline-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:09.388893 ml-cli-azureml-pipeline-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-10-20 12:13:09.388893 ml-cli-azureml-pipeline-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-20 12:13:09.388893 ml-cli-azureml-pipeline-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:09.384892 ml-cli-azureml-pipeline-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:09.384892 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3737 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:09.384892 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:09.388893 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/extraction/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/extraction/extraction.py
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/extraction/extraction_step.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/extraction/ml_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:09.388893 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/chunk_files.py
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/data_ingestion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/data_ingestion_step.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:09.388893 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/tests/test_chunk_files.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:09.388893 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/save/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/save/aggregate_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/save/save.py
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/save/save_step.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:09.388893 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/save/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/save/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/save/tests/test_aggregate_output.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:09.388893 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/pipelines/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2857 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/pipelines/train_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     3648 2022-10-20 12:13:00.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 12:13:09.384892 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-10-20 12:13:09.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-10-20 12:13:09.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 12:13:09.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-20 12:13:09.000000 ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:36.021863 ml-cli-azureml-pipeline-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2022-10-20 13:12:36.021863 ml-cli-azureml-pipeline-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-20 13:12:36.021863 ml-cli-azureml-pipeline-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      937 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:36.017863 ml-cli-azureml-pipeline-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:36.017863 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3737 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:36.017863 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:36.017863 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/extraction/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/extraction/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/extraction/extraction_step.py
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/extraction/ml_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:36.021863 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/chunk_files.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/data_ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/data_ingestion_step.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:36.021863 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/tests/test_chunk_files.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:36.021863 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/save/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/save/aggregate_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/save/save_step.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:36.021863 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/save/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/save/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/save/tests/test_aggregate_output.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:36.021863 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2857 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/pipelines/train_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3648 2022-10-20 13:12:29.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 13:12:36.017863 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2022-10-20 13:12:36.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-10-20 13:12:36.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 13:12:36.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-20 13:12:36.000000 ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline.egg-info/top_level.txt
```

### Comparing `ml-cli-azureml-pipeline-0.0.8/LICENSE` & `ml-cli-azureml-pipeline-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/PKG-INFO` & `ml-cli-azureml-pipeline-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-cli-azureml-pipeline
-Version: 0.0.8
+Version: 0.0.9
 Summary: ML-Cli run in an azureML Pipeline
 Home-page: https://github.com/AxaGuilDEv/ml-cli-azureml-pipeline
 Author: Axa_france
 Author-email: guillaume.chervet@axa.fr
 Platform: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ml-cli-azureml-pipeline-0.0.8/setup.py` & `ml-cli-azureml-pipeline-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/environment.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/environment.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/extraction/extraction.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/extraction/extraction.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/extraction/extraction_step.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/extraction/extraction_step.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/extraction/ml_cli.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/extraction/ml_cli.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/chunk_files.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/chunk_files.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/data_ingestion.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/data_ingestion_step.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/data_ingestion_step.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/tests/test_chunk_files.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/ingestion_chunk/tests/test_chunk_files.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/save/aggregate_output.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/save/aggregate_output.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/save/save.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/save/save.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,14 @@
 json_chunk_name = "json" + chunk_name
 output_jsons = str(data_output_dir_path / json_chunk_name)
 create_summary(output_jsons, str(data_output_dir_path / summary_filename))
 
 
 dstore = Datastore.get(workspace, save_datastore_name)
 dataset = Dataset.File.upload_directory(
-    src_dir=str(data_output_dir_path), target=DataPath(dstore, save_datastore_path), pattern="*.json", show_progress=True,
+    src_dir=str(data_output_dir_path), target=DataPath(dstore, save_datastore_path), pattern="*", show_progress=True,
     overwrite=True
 )
 
 
 # End the run
 run.complete()
```

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/save/save_step.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/save/save_step.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/modules/save/tests/test_aggregate_output.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/modules/save/tests/test_aggregate_output.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/pipelines/train_pipeline.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/pipelines/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline/run.py` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline/run.py`

 * *Files identical despite different names*

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline.egg-info/PKG-INFO` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-cli-azureml-pipeline
-Version: 0.0.8
+Version: 0.0.9
 Summary: ML-Cli run in an azureML Pipeline
 Home-page: https://github.com/AxaGuilDEv/ml-cli-azureml-pipeline
 Author: Axa_france
 Author-email: guillaume.chervet@axa.fr
 Platform: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ml-cli-azureml-pipeline-0.0.8/src/ml_cli_azureml_pipeline.egg-info/SOURCES.txt` & `ml-cli-azureml-pipeline-0.0.9/src/ml_cli_azureml_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

