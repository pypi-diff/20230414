# Comparing `tmp/funasr_onnx-0.0.4.tar.gz` & `tmp/funasr_onnx-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/funasr_onnx-0.0.4.tar", last modified: Fri Apr 14 15:10:30 2023, max compression
+gzip compressed data, was "dist/funasr_onnx-0.0.5.tar", last modified: Fri Apr 14 15:16:44 2023, max compression
```

## Comparing `funasr_onnx-0.0.4.tar` & `funasr_onnx-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2957 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2348 2023-04-07 06:55:12.000000 funasr_onnx-0.0.4/README.md
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      218 2023-04-14 03:21:54.000000 funasr_onnx-0.0.4/funasr_onnx/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7786 2023-04-14 02:00:09.000000 funasr_onnx-0.0.4/funasr_onnx/paraformer_bin.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12135 2023-04-14 03:21:54.000000 funasr_onnx-0.0.4/funasr_onnx/punc_bin.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-29 02:53:52.000000 funasr_onnx-0.0.4/funasr_onnx/utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    28927 2023-04-14 02:00:09.000000 funasr_onnx-0.0.4/funasr_onnx/utils/e2e_vad.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    15845 2023-04-14 02:00:09.000000 funasr_onnx-0.0.4/funasr_onnx/utils/frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-29 02:53:52.000000 funasr_onnx-0.0.4/funasr_onnx/utils/postprocess_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-29 02:53:52.000000 funasr_onnx-0.0.4/funasr_onnx/utils/timestamp_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9176 2023-04-14 02:00:09.000000 funasr_onnx-0.0.4/funasr_onnx/utils/utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9707 2023-04-14 03:21:54.000000 funasr_onnx-0.0.4/funasr_onnx/vad_bin.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx.egg-info/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2957 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx.egg-info/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      485 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx.egg-info/SOURCES.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx.egg-info/dependency_links.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       90 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx.egg-info/requires.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       12 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx.egg-info/top_level.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       38 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/setup.cfg
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1384 2023-04-14 03:21:54.000000 funasr_onnx-0.0.4/setup.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2784 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/PKG-INFO
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2175 2023-04-14 15:16:16.000000 funasr_onnx-0.0.5/README.md
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      218 2023-04-14 03:21:54.000000 funasr_onnx-0.0.5/funasr_onnx/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7786 2023-04-14 02:00:09.000000 funasr_onnx-0.0.5/funasr_onnx/paraformer_bin.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12135 2023-04-14 03:21:54.000000 funasr_onnx-0.0.5/funasr_onnx/punc_bin.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx/utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-29 02:53:52.000000 funasr_onnx-0.0.5/funasr_onnx/utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    28927 2023-04-14 02:00:09.000000 funasr_onnx-0.0.5/funasr_onnx/utils/e2e_vad.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    15845 2023-04-14 02:00:09.000000 funasr_onnx-0.0.5/funasr_onnx/utils/frontend.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-29 02:53:52.000000 funasr_onnx-0.0.5/funasr_onnx/utils/postprocess_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-29 02:53:52.000000 funasr_onnx-0.0.5/funasr_onnx/utils/timestamp_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9176 2023-04-14 02:00:09.000000 funasr_onnx-0.0.5/funasr_onnx/utils/utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9707 2023-04-14 03:21:54.000000 funasr_onnx-0.0.5/funasr_onnx/vad_bin.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx.egg-info/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2784 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx.egg-info/PKG-INFO
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      485 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx.egg-info/SOURCES.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx.egg-info/dependency_links.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       90 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx.egg-info/requires.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       12 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx.egg-info/top_level.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       38 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/setup.cfg
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1384 2023-04-14 15:16:16.000000 funasr_onnx-0.0.5/setup.py
```

### Comparing `funasr_onnx-0.0.4/PKG-INFO` & `funasr_onnx-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr_onnx
-Version: 0.0.4
+Version: 0.0.5
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab, Alibaba Group, China
 Author-email: funasr@list.alibaba-inc.com
 License: MIT
 Keywords: funasr,asr
 Platform: Any
@@ -14,18 +14,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 ## Using funasr with ONNXRuntime
 
 
-### Introduction
-- Model comes from [speech_paraformer](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary).
-
-
 ### Steps:
 1. Export the model.
    - Command: (`Tips`: torch >= 1.11.0 is required.)
 
        More details ref to ([export docs](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/export))
 
        - `e.g.`, Export model from modelscope
```

### Comparing `funasr_onnx-0.0.4/README.md` & `funasr_onnx-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 ## Using funasr with ONNXRuntime
 
 
-### Introduction
-- Model comes from [speech_paraformer](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary).
-
-
 ### Steps:
 1. Export the model.
    - Command: (`Tips`: torch >= 1.11.0 is required.)
 
        More details ref to ([export docs](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/export))
 
        - `e.g.`, Export model from modelscope
```

### Comparing `funasr_onnx-0.0.4/funasr_onnx/paraformer_bin.py` & `funasr_onnx-0.0.5/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.4/funasr_onnx/punc_bin.py` & `funasr_onnx-0.0.5/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.4/funasr_onnx/utils/e2e_vad.py` & `funasr_onnx-0.0.5/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.4/funasr_onnx/utils/frontend.py` & `funasr_onnx-0.0.5/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.4/funasr_onnx/utils/postprocess_utils.py` & `funasr_onnx-0.0.5/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.4/funasr_onnx/utils/timestamp_utils.py` & `funasr_onnx-0.0.5/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.4/funasr_onnx/utils/utils.py` & `funasr_onnx-0.0.5/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.4/funasr_onnx/vad_bin.py` & `funasr_onnx-0.0.5/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.4/funasr_onnx.egg-info/PKG-INFO` & `funasr_onnx-0.0.5/funasr_onnx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr-onnx
-Version: 0.0.4
+Version: 0.0.5
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab, Alibaba Group, China
 Author-email: funasr@list.alibaba-inc.com
 License: MIT
 Keywords: funasr,asr
 Platform: Any
@@ -14,18 +14,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 ## Using funasr with ONNXRuntime
 
 
-### Introduction
-- Model comes from [speech_paraformer](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary).
-
-
 ### Steps:
 1. Export the model.
    - Command: (`Tips`: torch >= 1.11.0 is required.)
 
        More details ref to ([export docs](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/export))
 
        - `e.g.`, Export model from modelscope
```

### Comparing `funasr_onnx-0.0.4/setup.py` & `funasr_onnx-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     print(readme_path)
     with open(readme_path, 'r', encoding='utf-8') as f:
         readme = f.read()
     return readme
 
 
 MODULE_NAME = 'funasr_onnx'
-VERSION_NUM = '0.0.4'
+VERSION_NUM = '0.0.5'
 
 setuptools.setup(
     name=MODULE_NAME,
     version=VERSION_NUM,
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
     author="Speech Lab, Alibaba Group, China",
```

