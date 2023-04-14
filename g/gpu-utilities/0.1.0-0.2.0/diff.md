# Comparing `tmp/gpu_utilities-0.1.0.tar.gz` & `tmp/gpu_utilities-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/dusaliyev/code/work/gpu_utils/dist/.tmp-e1xw6yam/gpu_utilities-0.1.0.tar", last modified: Tue Mar  7 04:37:08 2023, max compression
+gzip compressed data, was "/Users/dusaliyev/code/work/gpu_utils/dist/.tmp-sndfdhjt/gpu_utilities-0.2.0.tar", last modified: Fri Apr 14 11:56:40 2023, max compression
```

## Comparing `gpu_utilities-0.1.0.tar` & `gpu_utilities-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 dusaliyev   (502) staff       (20)        0 2023-03-07 04:37:08.000000 gpu_utilities-0.1.0/
--rw-r--r--   0 dusaliyev   (502) staff       (20)     1075 2023-03-06 10:39:10.000000 gpu_utilities-0.1.0/LICENSE
--rw-r--r--   0 dusaliyev   (502) staff       (20)      386 2023-03-07 04:37:08.000000 gpu_utilities-0.1.0/PKG-INFO
-drwxr-xr-x   0 dusaliyev   (502) staff       (20)        0 2023-03-07 04:37:08.000000 gpu_utilities-0.1.0/gpu_utilities/
--rw-r--r--   0 dusaliyev   (502) staff       (20)        0 2023-03-06 10:33:55.000000 gpu_utilities-0.1.0/gpu_utilities/__init__.py
--rw-r--r--   0 dusaliyev   (502) staff       (20)      145 2023-03-06 10:33:55.000000 gpu_utilities-0.1.0/gpu_utilities/errors.py
--rw-r--r--   0 dusaliyev   (502) staff       (20)      696 2023-03-06 10:33:55.000000 gpu_utilities-0.1.0/gpu_utilities/gpu.py
--rw-r--r--   0 dusaliyev   (502) staff       (20)     1138 2023-03-06 11:43:04.000000 gpu_utilities-0.1.0/gpu_utilities/gpu_info_obtainer.py
--rw-r--r--   0 dusaliyev   (502) staff       (20)     2981 2023-03-06 11:43:16.000000 gpu_utilities-0.1.0/gpu_utilities/gpu_selector.py
-drwxr-xr-x   0 dusaliyev   (502) staff       (20)        0 2023-03-07 04:37:08.000000 gpu_utilities-0.1.0/gpu_utilities.egg-info/
--rw-r--r--   0 dusaliyev   (502) staff       (20)      386 2023-03-07 04:37:08.000000 gpu_utilities-0.1.0/gpu_utilities.egg-info/PKG-INFO
--rw-r--r--   0 dusaliyev   (502) staff       (20)      401 2023-03-07 04:37:08.000000 gpu_utilities-0.1.0/gpu_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 dusaliyev   (502) staff       (20)        1 2023-03-07 04:37:08.000000 gpu_utilities-0.1.0/gpu_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 dusaliyev   (502) staff       (20)       14 2023-03-07 04:37:08.000000 gpu_utilities-0.1.0/gpu_utilities.egg-info/requires.txt
--rw-r--r--   0 dusaliyev   (502) staff       (20)       14 2023-03-07 04:37:08.000000 gpu_utilities-0.1.0/gpu_utilities.egg-info/top_level.txt
--rw-r--r--   0 dusaliyev   (502) staff       (20)      447 2023-03-06 11:48:08.000000 gpu_utilities-0.1.0/pyproject.toml
--rw-r--r--   0 dusaliyev   (502) staff       (20)       38 2023-03-07 04:37:08.000000 gpu_utilities-0.1.0/setup.cfg
-drwxr-xr-x   0 dusaliyev   (502) staff       (20)        0 2023-03-07 04:37:08.000000 gpu_utilities-0.1.0/tests/
--rw-r--r--   0 dusaliyev   (502) staff       (20)      421 2023-03-06 11:44:39.000000 gpu_utilities-0.1.0/tests/test_gpu_info_obtainer.py
--rw-r--r--   0 dusaliyev   (502) staff       (20)     6577 2023-03-06 11:44:42.000000 gpu_utilities-0.1.0/tests/test_gpu_selector.py
+drwxr-xr-x   0 dusaliyev   (502) staff       (20)        0 2023-04-14 11:56:40.000000 gpu_utilities-0.2.0/
+-rw-r--r--   0 dusaliyev   (502) staff       (20)     1075 2023-03-06 10:39:10.000000 gpu_utilities-0.2.0/LICENSE
+-rw-r--r--   0 dusaliyev   (502) staff       (20)      429 2023-04-14 11:56:40.000000 gpu_utilities-0.2.0/PKG-INFO
+drwxr-xr-x   0 dusaliyev   (502) staff       (20)        0 2023-04-14 11:56:40.000000 gpu_utilities-0.2.0/gpu_utilities/
+-rw-r--r--   0 dusaliyev   (502) staff       (20)        0 2023-03-06 10:33:55.000000 gpu_utilities-0.2.0/gpu_utilities/__init__.py
+-rw-r--r--   0 dusaliyev   (502) staff       (20)      145 2023-03-06 10:33:55.000000 gpu_utilities-0.2.0/gpu_utilities/errors.py
+-rw-r--r--   0 dusaliyev   (502) staff       (20)      745 2023-04-14 11:56:24.000000 gpu_utilities-0.2.0/gpu_utilities/gpu.py
+-rw-r--r--   0 dusaliyev   (502) staff       (20)      263 2023-04-14 11:56:24.000000 gpu_utilities-0.2.0/gpu_utilities/gpu_info_obtainer.py
+-rw-r--r--   0 dusaliyev   (502) staff       (20)     2981 2023-03-06 11:43:16.000000 gpu_utilities-0.2.0/gpu_utilities/gpu_selector.py
+drwxr-xr-x   0 dusaliyev   (502) staff       (20)        0 2023-04-14 11:56:40.000000 gpu_utilities-0.2.0/gpu_utilities/obtainers/
+-rw-r--r--   0 dusaliyev   (502) staff       (20)        0 2023-04-14 11:56:24.000000 gpu_utilities-0.2.0/gpu_utilities/obtainers/__init__.py
+-rw-r--r--   0 dusaliyev   (502) staff       (20)     2269 2023-04-14 11:56:24.000000 gpu_utilities-0.2.0/gpu_utilities/obtainers/nvml.py
+-rw-r--r--   0 dusaliyev   (502) staff       (20)     1323 2023-04-14 11:56:24.000000 gpu_utilities-0.2.0/gpu_utilities/obtainers/torch.py
+drwxr-xr-x   0 dusaliyev   (502) staff       (20)        0 2023-04-14 11:56:40.000000 gpu_utilities-0.2.0/gpu_utilities/utils/
+-rw-r--r--   0 dusaliyev   (502) staff       (20)        0 2023-04-14 11:56:24.000000 gpu_utilities-0.2.0/gpu_utilities/utils/__init__.py
+-rw-r--r--   0 dusaliyev   (502) staff       (20)     1072 2023-04-14 11:56:24.000000 gpu_utilities-0.2.0/gpu_utilities/utils/bytes.py
+drwxr-xr-x   0 dusaliyev   (502) staff       (20)        0 2023-04-14 11:56:40.000000 gpu_utilities-0.2.0/gpu_utilities.egg-info/
+-rw-r--r--   0 dusaliyev   (502) staff       (20)      429 2023-04-14 11:56:40.000000 gpu_utilities-0.2.0/gpu_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 dusaliyev   (502) staff       (20)      531 2023-04-14 11:56:40.000000 gpu_utilities-0.2.0/gpu_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 dusaliyev   (502) staff       (20)        1 2023-04-14 11:56:40.000000 gpu_utilities-0.2.0/gpu_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 dusaliyev   (502) staff       (20)       65 2023-04-14 11:56:40.000000 gpu_utilities-0.2.0/gpu_utilities.egg-info/requires.txt
+-rw-r--r--   0 dusaliyev   (502) staff       (20)       14 2023-04-14 11:56:40.000000 gpu_utilities-0.2.0/gpu_utilities.egg-info/top_level.txt
+-rw-r--r--   0 dusaliyev   (502) staff       (20)      537 2023-04-14 11:56:24.000000 gpu_utilities-0.2.0/pyproject.toml
+-rw-r--r--   0 dusaliyev   (502) staff       (20)       38 2023-04-14 11:56:40.000000 gpu_utilities-0.2.0/setup.cfg
+drwxr-xr-x   0 dusaliyev   (502) staff       (20)        0 2023-04-14 11:56:40.000000 gpu_utilities-0.2.0/tests/
+-rw-r--r--   0 dusaliyev   (502) staff       (20)     6577 2023-03-06 11:44:42.000000 gpu_utilities-0.2.0/tests/test_gpu_selector.py
```

### Comparing `gpu_utilities-0.1.0/LICENSE` & `gpu_utilities-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpu_utilities-0.1.0/gpu_utilities/gpu.py` & `gpu_utilities-0.2.0/gpu_utilities/gpu.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 class GPU:
     def __init__(
         self,
         cuda_id: int,
         name: str,
         max_available_memory_bytes: int,
         current_memory_utlization_bytes: int,
+        uuid: str = "",
     ) -> None:
         self.cuda_id = cuda_id
         self.name = name
         self.max_available_memory_bytes = max_available_memory_bytes
         self.current_memory_utlization_bytes = current_memory_utlization_bytes
+        self.uuid = uuid
 
     def __repr__(self) -> str:
         return str(self.__dict__)
 
     def to_torch_device(self) -> str:
         return f"cuda:{self.cuda_id}"
```

### Comparing `gpu_utilities-0.1.0/gpu_utilities/gpu_selector.py` & `gpu_utilities-0.2.0/gpu_utilities/gpu_selector.py`

 * *Files identical despite different names*

### Comparing `gpu_utilities-0.1.0/tests/test_gpu_selector.py` & `gpu_utilities-0.2.0/tests/test_gpu_selector.py`

 * *Files identical despite different names*

