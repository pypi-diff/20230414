# Comparing `tmp/funasr_torch-0.0.3.tar.gz` & `tmp/funasr_torch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/funasr_torch-0.0.3.tar", last modified: Fri Mar 24 05:25:09 2023, max compression
+gzip compressed data, was "dist/funasr_torch-0.0.4.tar", last modified: Fri Apr 14 15:21:07 2023, max compression
```

## Comparing `funasr_torch-0.0.3.tar` & `funasr_torch-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:25:09.000000 funasr_torch-0.0.3/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3308 2023-03-24 05:25:09.000000 funasr_torch-0.0.3/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2665 2023-03-24 05:23:58.000000 funasr_torch-0.0.3/README.md
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:25:09.000000 funasr_torch-0.0.3/funasr_torch.egg-info/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     3308 2023-03-24 05:25:09.000000 funasr_torch-0.0.3/funasr_torch.egg-info/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      197 2023-03-24 05:25:09.000000 funasr_torch-0.0.3/funasr_torch.egg-info/SOURCES.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-03-24 05:25:09.000000 funasr_torch-0.0.3/funasr_torch.egg-info/dependency_links.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      109 2023-03-24 05:25:09.000000 funasr_torch-0.0.3/funasr_torch.egg-info/requires.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-03-24 05:25:09.000000 funasr_torch-0.0.3/funasr_torch.egg-info/top_level.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       38 2023-03-24 05:25:09.000000 funasr_torch-0.0.3/setup.cfg
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1433 2023-03-24 05:23:58.000000 funasr_torch-0.0.3/setup.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:21:07.000000 funasr_torch-0.0.4/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3506 2023-04-14 15:21:07.000000 funasr_torch-0.0.4/PKG-INFO
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2863 2023-04-14 15:19:44.000000 funasr_torch-0.0.4/README.md
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:21:07.000000 funasr_torch-0.0.4/funasr_torch.egg-info/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     3506 2023-04-14 15:21:07.000000 funasr_torch-0.0.4/funasr_torch.egg-info/PKG-INFO
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      197 2023-04-14 15:21:07.000000 funasr_torch-0.0.4/funasr_torch.egg-info/SOURCES.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-04-14 15:21:07.000000 funasr_torch-0.0.4/funasr_torch.egg-info/dependency_links.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      109 2023-04-14 15:21:07.000000 funasr_torch-0.0.4/funasr_torch.egg-info/requires.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-04-14 15:21:07.000000 funasr_torch-0.0.4/funasr_torch.egg-info/top_level.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       38 2023-04-14 15:21:07.000000 funasr_torch-0.0.4/setup.cfg
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1433 2023-04-14 15:16:16.000000 funasr_torch-0.0.4/setup.py
```

### Comparing `funasr_torch-0.0.3/PKG-INFO` & `funasr_torch-0.0.4/funasr_torch.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: funasr_torch
-Version: 0.0.3
+Name: funasr-torch
+Version: 0.0.4
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab, Alibaba Group, China
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Keywords: funasr,paraformer, funasr_torch
 Platform: Any
@@ -15,16 +15,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 ## Using funasr with libtorch
 
 [FunASR](https://github.com/alibaba-damo-academy/FunASR) hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on ModelScope, researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
-### Introduction
-- Model comes from [speech_paraformer](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary).
 
 ### Steps:
 1. Export the model.
    - Command: (`Tips`: torch >= 1.11.0 is required.)
 
        More details ref to ([export docs](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/export))
 
@@ -35,18 +33,26 @@
        - `e.g.`, Export model from local path, the model'name must be `model.pb`.
          ```shell
          python -m funasr.export.export_model --model-name ./damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch --export-dir ./export --type torch --quantize False
          ```
 
 
 2. Install the `funasr_torch`.
+    
+    install from pip
     ```shell
-    pip install funasr_torch -i https://pypi.Python.org/simple
+    pip install --upgrade funasr_torch -i https://pypi.Python.org/simple
     ```
+    or install from source code
 
+    ```shell
+    git clone https://github.com/alibaba/FunASR.git && cd FunASR
+    cd funasr/runtime/python/libtorch
+    pip install -e ./
+    ```
 
 3. Run the demo.
    - Model_dir: the model path, which contains `model.torchscripts`, `config.yaml`, `am.mvn`.
    - Input: wav formt file, support formats: `str, np.ndarray, List[str]`
    - Output: `List[str]`: recognition result.
    - Example:
         ```python
@@ -57,14 +63,18 @@
 
         wav_path = ['/nfs/zhifu.gzf/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/example/asr_example.wav']
 
         result = model(wav_path)
         print(result)
         ```
 
+## Performance benchmark
+
+Please ref to [benchmark](https://github.com/alibaba-damo-academy/FunASR/blob/main/funasr/runtime/python/benchmark_libtorch.md)
+
 ## Speed
 
 Environment：Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz
 
 Test [wav, 5.53s, 100 times avg.](https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav)
 
 | Backend  | RTF (FP32) |
```

### Comparing `funasr_torch-0.0.3/README.md` & `funasr_torch-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 ## Using funasr with libtorch
 
 [FunASR](https://github.com/alibaba-damo-academy/FunASR) hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on ModelScope, researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
-### Introduction
-- Model comes from [speech_paraformer](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary).
 
 ### Steps:
 1. Export the model.
    - Command: (`Tips`: torch >= 1.11.0 is required.)
 
        More details ref to ([export docs](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/export))
 
@@ -18,18 +16,26 @@
        - `e.g.`, Export model from local path, the model'name must be `model.pb`.
          ```shell
          python -m funasr.export.export_model --model-name ./damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch --export-dir ./export --type torch --quantize False
          ```
 
 
 2. Install the `funasr_torch`.
+    
+    install from pip
     ```shell
-    pip install funasr_torch -i https://pypi.Python.org/simple
+    pip install --upgrade funasr_torch -i https://pypi.Python.org/simple
     ```
+    or install from source code
 
+    ```shell
+    git clone https://github.com/alibaba/FunASR.git && cd FunASR
+    cd funasr/runtime/python/libtorch
+    pip install -e ./
+    ```
 
 3. Run the demo.
    - Model_dir: the model path, which contains `model.torchscripts`, `config.yaml`, `am.mvn`.
    - Input: wav formt file, support formats: `str, np.ndarray, List[str]`
    - Output: `List[str]`: recognition result.
    - Example:
         ```python
@@ -40,14 +46,18 @@
 
         wav_path = ['/nfs/zhifu.gzf/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/example/asr_example.wav']
 
         result = model(wav_path)
         print(result)
         ```
 
+## Performance benchmark
+
+Please ref to [benchmark](https://github.com/alibaba-damo-academy/FunASR/blob/main/funasr/runtime/python/benchmark_libtorch.md)
+
 ## Speed
 
 Environment：Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz
 
 Test [wav, 5.53s, 100 times avg.](https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav)
 
 | Backend  | RTF (FP32) |
```

### Comparing `funasr_torch-0.0.3/funasr_torch.egg-info/PKG-INFO` & `funasr_torch-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: funasr-torch
-Version: 0.0.3
+Name: funasr_torch
+Version: 0.0.4
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab, Alibaba Group, China
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Keywords: funasr,paraformer, funasr_torch
 Platform: Any
@@ -15,16 +15,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 ## Using funasr with libtorch
 
 [FunASR](https://github.com/alibaba-damo-academy/FunASR) hopes to build a bridge between academic research and industrial applications on speech recognition. By supporting the training & finetuning of the industrial-grade speech recognition model released on ModelScope, researchers and developers can conduct research and production of speech recognition models more conveniently, and promote the development of speech recognition ecology. ASR for Fun！
 
-### Introduction
-- Model comes from [speech_paraformer](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary).
 
 ### Steps:
 1. Export the model.
    - Command: (`Tips`: torch >= 1.11.0 is required.)
 
        More details ref to ([export docs](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/export))
 
@@ -35,18 +33,26 @@
        - `e.g.`, Export model from local path, the model'name must be `model.pb`.
          ```shell
          python -m funasr.export.export_model --model-name ./damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch --export-dir ./export --type torch --quantize False
          ```
 
 
 2. Install the `funasr_torch`.
+    
+    install from pip
     ```shell
-    pip install funasr_torch -i https://pypi.Python.org/simple
+    pip install --upgrade funasr_torch -i https://pypi.Python.org/simple
     ```
+    or install from source code
 
+    ```shell
+    git clone https://github.com/alibaba/FunASR.git && cd FunASR
+    cd funasr/runtime/python/libtorch
+    pip install -e ./
+    ```
 
 3. Run the demo.
    - Model_dir: the model path, which contains `model.torchscripts`, `config.yaml`, `am.mvn`.
    - Input: wav formt file, support formats: `str, np.ndarray, List[str]`
    - Output: `List[str]`: recognition result.
    - Example:
         ```python
@@ -57,14 +63,18 @@
 
         wav_path = ['/nfs/zhifu.gzf/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/example/asr_example.wav']
 
         result = model(wav_path)
         print(result)
         ```
 
+## Performance benchmark
+
+Please ref to [benchmark](https://github.com/alibaba-damo-academy/FunASR/blob/main/funasr/runtime/python/benchmark_libtorch.md)
+
 ## Speed
 
 Environment：Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz
 
 Test [wav, 5.53s, 100 times avg.](https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav)
 
 | Backend  | RTF (FP32) |
```

### Comparing `funasr_torch-0.0.3/setup.py` & `funasr_torch-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         readme = f.read()
     return readme
 
 
 
 setuptools.setup(
     name='funasr_torch',
-    version='0.0.3',
+    version='0.0.4',
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
     author="Speech Lab, Alibaba Group, China",
     author_email="funasr@list.alibaba-inc.com",
     description="FunASR: A Fundamental End-to-End Speech Recognition Toolkit",
     license="The MIT License",
     long_description=get_readme(),
```

