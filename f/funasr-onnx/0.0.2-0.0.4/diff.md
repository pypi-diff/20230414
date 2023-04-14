# Comparing `tmp/funasr_onnx-0.0.2.tar.gz` & `tmp/funasr_onnx-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/funasr_onnx-0.0.2.tar", last modified: Fri Mar 24 05:26:37 2023, max compression
+gzip compressed data, was "dist/funasr_onnx-0.0.4.tar", last modified: Fri Apr 14 15:10:30 2023, max compression
```

## Comparing `funasr_onnx-0.0.2.tar` & `funasr_onnx-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:26:37.000000 funasr_onnx-0.0.2/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2918 2023-03-24 05:26:37.000000 funasr_onnx-0.0.2/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2309 2023-03-24 05:23:58.000000 funasr_onnx-0.0.2/README.md
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:26:37.000000 funasr_onnx-0.0.2/funasr_onnx/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       65 2023-03-24 03:38:09.000000 funasr_onnx-0.0.2/funasr_onnx/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7685 2023-03-24 03:38:09.000000 funasr_onnx-0.0.2/funasr_onnx/paraformer_bin.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:26:37.000000 funasr_onnx-0.0.2/funasr_onnx/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-24 03:38:09.000000 funasr_onnx-0.0.2/funasr_onnx/utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7040 2023-03-24 03:38:09.000000 funasr_onnx-0.0.2/funasr_onnx/utils/frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-24 03:38:09.000000 funasr_onnx-0.0.2/funasr_onnx/utils/postprocess_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-24 03:38:09.000000 funasr_onnx-0.0.2/funasr_onnx/utils/timestamp_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     8795 2023-03-24 03:38:09.000000 funasr_onnx-0.0.2/funasr_onnx/utils/utils.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-03-24 05:26:37.000000 funasr_onnx-0.0.2/funasr_onnx.egg-info/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2918 2023-03-24 05:26:37.000000 funasr_onnx-0.0.2/funasr_onnx.egg-info/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      409 2023-03-24 05:26:37.000000 funasr_onnx-0.0.2/funasr_onnx.egg-info/SOURCES.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-03-24 05:26:37.000000 funasr_onnx-0.0.2/funasr_onnx.egg-info/dependency_links.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       90 2023-03-24 05:26:37.000000 funasr_onnx-0.0.2/funasr_onnx.egg-info/requires.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       12 2023-03-24 05:26:37.000000 funasr_onnx-0.0.2/funasr_onnx.egg-info/top_level.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       38 2023-03-24 05:26:37.000000 funasr_onnx-0.0.2/setup.cfg
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1384 2023-03-24 05:11:50.000000 funasr_onnx-0.0.2/setup.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2957 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/PKG-INFO
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2348 2023-04-07 06:55:12.000000 funasr_onnx-0.0.4/README.md
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      218 2023-04-14 03:21:54.000000 funasr_onnx-0.0.4/funasr_onnx/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7786 2023-04-14 02:00:09.000000 funasr_onnx-0.0.4/funasr_onnx/paraformer_bin.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12135 2023-04-14 03:21:54.000000 funasr_onnx-0.0.4/funasr_onnx/punc_bin.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx/utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-29 02:53:52.000000 funasr_onnx-0.0.4/funasr_onnx/utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    28927 2023-04-14 02:00:09.000000 funasr_onnx-0.0.4/funasr_onnx/utils/e2e_vad.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    15845 2023-04-14 02:00:09.000000 funasr_onnx-0.0.4/funasr_onnx/utils/frontend.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-29 02:53:52.000000 funasr_onnx-0.0.4/funasr_onnx/utils/postprocess_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-29 02:53:52.000000 funasr_onnx-0.0.4/funasr_onnx/utils/timestamp_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9176 2023-04-14 02:00:09.000000 funasr_onnx-0.0.4/funasr_onnx/utils/utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9707 2023-04-14 03:21:54.000000 funasr_onnx-0.0.4/funasr_onnx/vad_bin.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx.egg-info/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2957 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx.egg-info/PKG-INFO
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      485 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx.egg-info/SOURCES.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx.egg-info/dependency_links.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       90 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx.egg-info/requires.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       12 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/funasr_onnx.egg-info/top_level.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       38 2023-04-14 15:10:30.000000 funasr_onnx-0.0.4/setup.cfg
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1384 2023-04-14 03:21:54.000000 funasr_onnx-0.0.4/setup.py
```

### Comparing `funasr_onnx-0.0.2/PKG-INFO` & `funasr_onnx-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr_onnx
-Version: 0.0.2
+Version: 0.0.4
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab, Alibaba Group, China
 Author-email: funasr@list.alibaba-inc.com
 License: MIT
 Keywords: funasr,asr
 Platform: Any
@@ -34,19 +34,29 @@
          ```
        - `e.g.`, Export model from local path, the model'name must be `model.pb`.
          ```shell
          python -m funasr.export.export_model --model-name ./damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch --export-dir ./export --type onnx --quantize False
          ```
 
 
-2. Install the `funasr_onnx`.
+2. Install the `funasr_onnx`
+
+install from pip
 ```shell
-pip install funasr_onnx -i https://pypi.Python.org/simple
+pip install --upgrade funasr_onnx -i https://pypi.Python.org/simple
 ```
 
+or install from source code
+
+```shell
+git clone https://github.com/alibaba/FunASR.git && cd FunASR
+cd funasr/runtime/python/onnxruntime
+python setup.py build
+python setup.py install
+```
 
 3. Run the demo.
    - Model_dir: the model path, which contains `model.onnx`, `config.yaml`, `am.mvn`.
    - Input: wav formt file, support formats: `str, np.ndarray, List[str]`
    - Output: `List[str]`: recognition result.
    - Example:
         ```python
@@ -57,22 +67,14 @@
 
         wav_path = ['/nfs/zhifu.gzf/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/example/asr_example.wav']
 
         result = model(wav_path)
         print(result)
         ```
 
-## Speed
-
-Environment：Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz
-
-Test [wav, 5.53s, 100 times avg.](https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav)
-
-| Backend |        RTF        |
-|:-------:|:-----------------:|
-| Pytorch |       0.110       |
-|  Onnx   |       0.038       |
+## Performance benchmark
 
+Please ref to [benchmark](https://github.com/alibaba-damo-academy/FunASR/blob/main/funasr/runtime/python/benchmark_onnx.md)
 
 ## Acknowledge
 1. This project is maintained by [FunASR community](https://github.com/alibaba-damo-academy/FunASR).
 2. We acknowledge [SWHL](https://github.com/RapidAI/RapidASR) for contributing the onnxruntime (for paraformer model).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `funasr_onnx-0.0.2/README.md` & `funasr_onnx-0.0.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -17,19 +17,29 @@
          ```
        - `e.g.`, Export model from local path, the model'name must be `model.pb`.
          ```shell
          python -m funasr.export.export_model --model-name ./damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch --export-dir ./export --type onnx --quantize False
          ```
 
 
-2. Install the `funasr_onnx`.
+2. Install the `funasr_onnx`
+
+install from pip
 ```shell
-pip install funasr_onnx -i https://pypi.Python.org/simple
+pip install --upgrade funasr_onnx -i https://pypi.Python.org/simple
 ```
 
+or install from source code
+
+```shell
+git clone https://github.com/alibaba/FunASR.git && cd FunASR
+cd funasr/runtime/python/onnxruntime
+python setup.py build
+python setup.py install
+```
 
 3. Run the demo.
    - Model_dir: the model path, which contains `model.onnx`, `config.yaml`, `am.mvn`.
    - Input: wav formt file, support formats: `str, np.ndarray, List[str]`
    - Output: `List[str]`: recognition result.
    - Example:
         ```python
@@ -40,22 +50,14 @@
 
         wav_path = ['/nfs/zhifu.gzf/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/example/asr_example.wav']
 
         result = model(wav_path)
         print(result)
         ```
 
-## Speed
-
-Environment：Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz
-
-Test [wav, 5.53s, 100 times avg.](https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav)
-
-| Backend |        RTF        |
-|:-------:|:-----------------:|
-| Pytorch |       0.110       |
-|  Onnx   |       0.038       |
+## Performance benchmark
 
+Please ref to [benchmark](https://github.com/alibaba-damo-academy/FunASR/blob/main/funasr/runtime/python/benchmark_onnx.md)
 
 ## Acknowledge
 1. This project is maintained by [FunASR community](https://github.com/alibaba-damo-academy/FunASR).
 2. We acknowledge [SWHL](https://github.com/RapidAI/RapidASR) for contributing the onnxruntime (for paraformer model).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `funasr_onnx-0.0.2/funasr_onnx/paraformer_bin.py` & `funasr_onnx-0.0.4/funasr_onnx/paraformer_bin.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 
 class Paraformer():
     def __init__(self, model_dir: Union[str, Path] = None,
                  batch_size: int = 1,
                  device_id: Union[str, int] = "-1",
                  plot_timestamp_to: str = "",
-                 pred_bias: int = 1,
                  quantize: bool = False,
                  intra_op_num_threads: int = 4,
                  ):
 
         if not Path(model_dir).exists():
             raise FileNotFoundError(f'{model_dir} does not exist.')
 
@@ -43,15 +42,18 @@
         self.frontend = WavFrontend(
             cmvn_file=cmvn_file,
             **config['frontend_conf']
         )
         self.ort_infer = OrtInferSession(model_file, device_id, intra_op_num_threads=intra_op_num_threads)
         self.batch_size = batch_size
         self.plot_timestamp_to = plot_timestamp_to
-        self.pred_bias = pred_bias
+        if "predictor_bias" in config['model_conf'].keys():
+            self.pred_bias = config['model_conf']['predictor_bias']
+        else:
+            self.pred_bias = 0
 
     def __call__(self, wav_content: Union[str, np.ndarray, List[str]], **kwargs) -> List:
         waveform_list = self.load_data(wav_content, self.frontend.opts.frame_opts.samp_freq)
         waveform_nums = len(waveform_list)
         asr_res = []
         for beg_idx in range(0, waveform_nums, self.batch_size):
```

### Comparing `funasr_onnx-0.0.2/funasr_onnx/utils/postprocess_utils.py` & `funasr_onnx-0.0.4/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.2/funasr_onnx/utils/timestamp_utils.py` & `funasr_onnx-0.0.4/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.2/funasr_onnx/utils/utils.py` & `funasr_onnx-0.0.4/funasr_onnx/utils/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,48 +20,33 @@
 
 
 class TokenIDConverter():
     def __init__(self, token_list: Union[List, str],
                  ):
         check_argument_types()
 
-        # self.token_list = self.load_token(token_path)
         self.token_list = token_list
         self.unk_symbol = token_list[-1]
+        self.token2id = {v: i for i, v in enumerate(self.token_list)}
+        self.unk_id = self.token2id[self.unk_symbol]
 
-    # @staticmethod
-    # def load_token(file_path: Union[Path, str]) -> List:
-    #     if not Path(file_path).exists():
-    #         raise TokenIDConverterError(f'The {file_path} does not exist.')
-    #
-    #     with open(str(file_path), 'rb') as f:
-    #         token_list = pickle.load(f)
-    #
-    #     if len(token_list) != len(set(token_list)):
-    #         raise TokenIDConverterError('The Token exists duplicated symbol.')
-    #     return token_list
 
     def get_num_vocabulary_size(self) -> int:
         return len(self.token_list)
 
     def ids2tokens(self,
                    integers: Union[np.ndarray, Iterable[int]]) -> List[str]:
         if isinstance(integers, np.ndarray) and integers.ndim != 1:
             raise TokenIDConverterError(
                 f"Must be 1 dim ndarray, but got {integers.ndim}")
         return [self.token_list[i] for i in integers]
 
     def tokens2ids(self, tokens: Iterable[str]) -> List[int]:
-        token2id = {v: i for i, v in enumerate(self.token_list)}
-        if self.unk_symbol not in token2id:
-            raise TokenIDConverterError(
-                f"Unknown symbol '{self.unk_symbol}' doesn't exist in the token_list"
-            )
-        unk_id = token2id[self.unk_symbol]
-        return [token2id.get(i, unk_id) for i in tokens]
+
+        return [self.token2id.get(i, self.unk_id) for i in tokens]
 
 
 class CharTokenizer():
     def __init__(
         self,
         symbol_value: Union[Path, str, Iterable[str]] = None,
         space_symbol: str = "<space>",
@@ -184,15 +169,15 @@
                           'https://onnxruntime.ai/docs/execution-providers/CUDA-ExecutionProvider.html',
                           RuntimeWarning)
 
     def __call__(self,
                  input_content: List[Union[np.ndarray, np.ndarray]]) -> np.ndarray:
         input_dict = dict(zip(self.get_input_names(), input_content))
         try:
-            return self.session.run(None, input_dict)
+            return self.session.run(self.get_output_names(), input_dict)
         except Exception as e:
             raise ONNXRuntimeError('ONNXRuntime inferece failed.') from e
 
     def get_input_names(self, ):
         return [v.name for v in self.session.get_inputs()]
 
     def get_output_names(self,):
@@ -211,26 +196,58 @@
     def _verify_model(model_path):
         model_path = Path(model_path)
         if not model_path.exists():
             raise FileNotFoundError(f'{model_path} does not exists.')
         if not model_path.is_file():
             raise FileExistsError(f'{model_path} is not a file.')
 
+def split_to_mini_sentence(words: list, word_limit: int = 20):
+    assert word_limit > 1
+    if len(words) <= word_limit:
+        return [words]
+    sentences = []
+    length = len(words)
+    sentence_len = length // word_limit
+    for i in range(sentence_len):
+        sentences.append(words[i * word_limit:(i + 1) * word_limit])
+    if length % word_limit > 0:
+        sentences.append(words[sentence_len * word_limit:])
+    return sentences
+
+def code_mix_split_words(text: str):
+    words = []
+    segs = text.split()
+    for seg in segs:
+        # There is no space in seg.
+        current_word = ""
+        for c in seg:
+            if len(c.encode()) == 1:
+                # This is an ASCII char.
+                current_word += c
+            else:
+                # This is a Chinese char.
+                if len(current_word) > 0:
+                    words.append(current_word)
+                    current_word = ""
+                words.append(c)
+        if len(current_word) > 0:
+            words.append(current_word)
+    return words
 
 def read_yaml(yaml_path: Union[str, Path]) -> Dict:
     if not Path(yaml_path).exists():
         raise FileExistsError(f'The {yaml_path} does not exist.')
 
     with open(str(yaml_path), 'rb') as f:
         data = yaml.load(f, Loader=yaml.Loader)
     return data
 
 
 @functools.lru_cache()
-def get_logger(name='rapdi_paraformer'):
+def get_logger(name='funasr_onnx'):
     """Initialize and get a logger by name.
     If the logger has not been initialized, this method will initialize the
     logger by adding one or two handlers, otherwise the initialized logger will
     be directly returned. During initialization, a StreamHandler will always be
     added.
     Args:
         name (str): Logger name.
```

### Comparing `funasr_onnx-0.0.2/funasr_onnx.egg-info/PKG-INFO` & `funasr_onnx-0.0.4/funasr_onnx.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr-onnx
-Version: 0.0.2
+Version: 0.0.4
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab, Alibaba Group, China
 Author-email: funasr@list.alibaba-inc.com
 License: MIT
 Keywords: funasr,asr
 Platform: Any
@@ -34,19 +34,29 @@
          ```
        - `e.g.`, Export model from local path, the model'name must be `model.pb`.
          ```shell
          python -m funasr.export.export_model --model-name ./damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch --export-dir ./export --type onnx --quantize False
          ```
 
 
-2. Install the `funasr_onnx`.
+2. Install the `funasr_onnx`
+
+install from pip
 ```shell
-pip install funasr_onnx -i https://pypi.Python.org/simple
+pip install --upgrade funasr_onnx -i https://pypi.Python.org/simple
 ```
 
+or install from source code
+
+```shell
+git clone https://github.com/alibaba/FunASR.git && cd FunASR
+cd funasr/runtime/python/onnxruntime
+python setup.py build
+python setup.py install
+```
 
 3. Run the demo.
    - Model_dir: the model path, which contains `model.onnx`, `config.yaml`, `am.mvn`.
    - Input: wav formt file, support formats: `str, np.ndarray, List[str]`
    - Output: `List[str]`: recognition result.
    - Example:
         ```python
@@ -57,22 +67,14 @@
 
         wav_path = ['/nfs/zhifu.gzf/export/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/example/asr_example.wav']
 
         result = model(wav_path)
         print(result)
         ```
 
-## Speed
-
-Environment：Intel(R) Xeon(R) Platinum 8163 CPU @ 2.50GHz
-
-Test [wav, 5.53s, 100 times avg.](https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav)
-
-| Backend |        RTF        |
-|:-------:|:-----------------:|
-| Pytorch |       0.110       |
-|  Onnx   |       0.038       |
+## Performance benchmark
 
+Please ref to [benchmark](https://github.com/alibaba-damo-academy/FunASR/blob/main/funasr/runtime/python/benchmark_onnx.md)
 
 ## Acknowledge
 1. This project is maintained by [FunASR community](https://github.com/alibaba-damo-academy/FunASR).
 2. We acknowledge [SWHL](https://github.com/RapidAI/RapidASR) for contributing the onnxruntime (for paraformer model).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `funasr_onnx-0.0.2/setup.py` & `funasr_onnx-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     print(readme_path)
     with open(readme_path, 'r', encoding='utf-8') as f:
         readme = f.read()
     return readme
 
 
 MODULE_NAME = 'funasr_onnx'
-VERSION_NUM = '0.0.2'
+VERSION_NUM = '0.0.4'
 
 setuptools.setup(
     name=MODULE_NAME,
     version=VERSION_NUM,
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
     author="Speech Lab, Alibaba Group, China",
```

