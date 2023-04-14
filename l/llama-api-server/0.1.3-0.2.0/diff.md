# Comparing `tmp/llama_api_server-0.1.3.tar.gz` & `tmp/llama_api_server-0.2.0.tar.gz`

## Comparing `llama_api_server-0.1.3.tar` & `llama_api_server-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.gitattributes
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/Makefile
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/SECURITY.md
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/version.txt
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.github/FUNDING.yml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.github/dependabot.yml
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.github/workflows/release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/llama_api_server/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/llama_api_server/__main__.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/llama_api_server/app.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/llama_api_server/model_pool.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/llama_api_server/utils.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/llama_api_server/models/llama_cpp.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/LICENSE
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/README.md
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 llama_api_server-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.gitattributes
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/Makefile
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/SECURITY.md
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/version.txt
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/__main__.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/app.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/config.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/model_pool.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/utils.py
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/models/llama_cpp.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/models/pyllama.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/models/pyllama_quant.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/README.md
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/PKG-INFO
```

### Comparing `llama_api_server-0.1.3/SECURITY.md` & `llama_api_server-0.2.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.1.3/.github/FUNDING.yml` & `llama_api_server-0.2.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md` & `llama_api_server-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `llama_api_server-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.1.3/.github/workflows/release.yml` & `llama_api_server-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.1.3/llama_api_server/models/llama_cpp.py` & `llama_api_server-0.2.0/llama_api_server/models/llama_cpp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,116 @@
 import llamacpp
 import array
 from llama_api_server.utils import get_uuid, get_timestamp, unpack_cfloat_array
 
 
-class LlamaCpp:
+def _create_llama_model(model_path, embedding=False):
+    params = llamacpp.LlamaContextParams()
+    params.seed = -1
+    params.embedding = embedding
+    model = llamacpp.LlamaContext(model_path, params)
+    return model
+
+
+def _eval_token(model, tokens, n_past, n_batch, n_thread):
+    l = len(tokens)
+    for s in range(0, l, n_batch):
+        e = min(l, s + n_batch)
+        p = e - s
+        model.eval(array.array("i", tokens[s:e]), p, n_past, n_thread)
+        n_past += p
+    return n_past
+
+
+class LlamaCppCompletion:
     def __init__(self, params):
-        self.model_path = params["path"]
-        self.n_batch = params.get("n_batch", None) or 16
+        model_path = params["path"]
+        self.model = _create_llama_model(model_path, False)
+        self.n_batch = params.get("n_batch", None) or 2
         self.n_thread = params.get("n_thread", None) or 4
 
     def completions(self, args):
-        params = llamacpp.LlamaContextParams()
-        params.seed = -1
-
-        model = llamacpp.LlamaContext(self.model_path, params)
-
         # args can be None, so need the "or" part to handle
-        top_k = args.get("top_k", None) or 1
-        top_p = args.get("top_p", None) or 1
-        temp = args.get("temperature", None) or 1.0
-        echo = args.get("echo", None) or False
-        max_tokens = args.get("max_tokens", None) or 16
+        top_k = args["top_k"]
+        top_p = args["top_p"]
+        temp = args["temperature"]
+        echo = args["echo"]
+        max_tokens = args["max_tokens"]
+        suffix = args["suffix"]
         repeat_penalty = 1.3
 
         prompt = args["prompt"]
-        prompt_tokens = model.str_to_token(prompt, True).tolist()
-        n_past = self.eval_token(model, prompt_tokens[:-1], 0)
+        prompt_tokens = self.model.str_to_token(prompt, True).tolist()
+        n_past = _eval_token(
+            self.model, prompt_tokens[:-1], 0, self.n_batch, self.n_thread
+        )
 
         result = prompt if echo else ""
         token = prompt_tokens[-1]
         finish_reason = "length"
         for i in range(max_tokens):
-            model.eval(array.array("i", [token]), 1, n_past, self.n_thread)
+            self.model.eval(array.array("i", [token]), 1, n_past, self.n_thread)
 
-            token = model.sample_top_p_top_k(
+            token = self.model.sample_top_p_top_k(
                 array.array("i", []), top_k, top_p, temp, repeat_penalty
             )
             if token == 2:
                 # EOS
                 finish_reason = "stop"
                 break
 
-            text = model.token_to_str(token)
+            text = self.model.token_to_str(token)
             result += text
             n_past += 1
 
         c_prompt_tokens = len(prompt_tokens)
         return {
             "id": get_uuid(),
             "object": "text_completion",
             "created": get_timestamp(),
             "model": args["model"],
             "choices": [
                 {
-                    "text": result,
+                    "text": result + suffix,
                     "index": 0,
                     "logprobs": None,
                     "finish_reason": finish_reason,
                 }
             ],
             "usage": {
                 "prompt_tokens": c_prompt_tokens,
                 "completion_tokens": n_past - c_prompt_tokens,
                 "total_tokens": n_past,
             },
         }
 
-    def embeddings(self, args):
-        params = llamacpp.LlamaContextParams()
-        params.seed = -1
-        params.embedding = True
 
-        model = llamacpp.LlamaContext(self.model_path, params)
+class LlamaCppEmbedding:
+    def __init__(self, params):
+        model_path = params["path"]
+        self.model = _create_llama_model(model_path, True)
+        self.n_batch = params.get("n_batch", None) or 2
+        self.n_thread = params.get("n_thread", None) or 4
 
+    def embeddings(self, args):
         inputs = args["input"]
         if inputs is str:
             inputs = [inputs]
             is_array = False
         else:
             is_array = True
         embeds = []
 
         for i in inputs:
-            prompt_tokens = model.str_to_token(i, True)
-            n_past = self.eval_token(model, prompt_tokens, 0)
+            prompt_tokens = self.model.str_to_token(i, True)
+            n_past = _eval_token(
+                self.model, prompt_tokens, 0, self.n_batch, self.n_thread
+            )
 
-            embed = unpack_cfloat_array(model.get_embeddings())
+            embed = unpack_cfloat_array(self.model.get_embeddings())
             embeds.append(embed)
 
         if not is_array:
             embeds = embeds[0]
 
         c_prompt_tokens = len(prompt_tokens)
         return {
@@ -97,16 +118,7 @@
             "data": [{"object": "embedding", "embedding": embed, "index": 0}],
             "model": args["model"],
             "usage": {
                 "prompt_tokens": c_prompt_tokens,
                 "total_tokens": c_prompt_tokens,
             },
         }
-
-    def eval_token(self, model, tokens, n_past):
-        l = len(tokens)
-        for s in range(0, l, self.n_batch):
-            e = min(l, s + self.n_batch)
-            p = e - s
-            model.eval(array.array("i", tokens[s:e]), p, n_past, self.n_thread)
-            n_past += p
-        return n_past
```

### Comparing `llama_api_server-0.1.3/.gitignore` & `llama_api_server-0.2.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 /models
 *.swp
 /.idea
 .DS_Store
 /config.yml
+/tokens.txt
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `llama_api_server-0.1.3/LICENSE` & `llama_api_server-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.1.3/pyproject.toml` & `llama_api_server-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "llama_api_server"
-version = "0.1.3"
+version = "0.2.0"
 description = ""
 authors = [
     {name = "iaalm", email= "iaalmsimon@gmail.com"}
 ]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.7"
@@ -27,10 +27,16 @@
 dependencies = [
   "llamacpp>=0.1.11",
   "Flask>=2.0.0",
   "numpy",
   "pyyaml",
 ]
 
+[project.optional-dependencies]
+pyllama = [
+    "pyllama>=0.0.9",
+    "transformers>=4.27.4",
+]
+
 [project.urls]
 homepage = "https://github.com/iaalm/llama-api-server"
 repository = "https://github.com/iaalm/llama-api-server"
```

### Comparing `llama_api_server-0.1.3/PKG-INFO` & `llama_api_server-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: llama_api_server
-Version: 0.1.3
-Project-URL: homepage, https://github.com/iaalm/llama-api-server
-Project-URL: repository, https://github.com/iaalm/llama-api-server
-Author-email: iaalm <iaalmsimon@gmail.com>
-License: MIT
-License-File: LICENSE
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Requires-Dist: flask>=2.0.0
-Requires-Dist: llamacpp>=0.1.11
-Requires-Dist: numpy
-Requires-Dist: pyyaml
-Description-Content-Type: text/markdown
-
 llama-api-server
 =======
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Release](https://github.com/iaalm/llama-api-server/actions/workflows/release.yml/badge.svg)](https://github.com/iaalm/llama-api-server/actions/workflows/release.yml)
 
 This project is under active deployment. Breaking changes could be made any time.
@@ -32,41 +9,64 @@
 Llama as a Service! This project try to build a REST-ful API server compatible to OpenAI API using open source backends like llama.
 
 ## Get started
 
 ### Prepare model
 
 #### llama.cpp
-If you you don't have quantize llama, you need to follow [instruction](https://github.com/ggerganov/llama.cpp#usage) to prepare model.
+If you you don't have quantized llama.cpp, you need to follow [instruction](https://github.com/ggerganov/llama.cpp#usage) to prepare model.
+
+#### pyllama
+If you you don't have quantize pyllama, you need to follow [instruction](https://github.com/juncongmoo/pyllama#-quantize-llama-to-run-in-a-4gb-gpu) to prepare model.
+
 
 ### Install
 ```
 pip install llama-api-server
+
+# to run wth pyllama
+pip install llama-api-server[pyllama]
+
 echo > config.yml << EOF
 models:
   completions:
-    text-davinci-003:
+    text-ada-002:
       type: llama_cpp
       params:
         path: /absolute/path/to/your/7B/ggml-model-q4_0.bin
+    text-davinci-002:
+      type: pyllama_quant
+      params:
+        path: /absolute/path/to/your/pyllama-7B4b.pt
+    text-davinci-003:
+      type: pyllama
+      params:
+        ckpt_dir: /absolute/path/to/your/7B/
+        tokenizer_path: /absolute/path/to/your/tokenizer.model
   embeddings:
     text-embedding-ada-002:
       type: llama_cpp
       params:
         path: /absolute/path/to/your/7B/ggml-model-q4_0.bin
 EOF
 
+echo "SOME_TOKEN" > tokens.txt
+
 # start web server
 python -m llama_api_server
 ```
 
 ### Call with openai-python
 ```
+export OPENAI_API_KEY=SOME_TOKEN
 export OPENAI_API_BASE=http://127.0.0.1:5000/v1
-openai api completions.create -e text-davinci-003 -p "hello?"
+
+openai api completions.create -e text-ada-002 -p "hello?"
+
+curl -X POST http://127.0.0.1:5000/v1/embeddings -H 'Content-Type: application/json' -d '{"model":"text-embedding-ada-002", "input":"It is good."}'  -H "Authorization: Bearer SOME_TOKEN"
 ```
 
 ## Roadmap
 
 #### Tested with
 - [X] openai-python
     - [X] OPENAI\_API\_TYPE=default
@@ -80,17 +80,22 @@
     - [ ] set `stream`
     - [ ] set `n`
     - [ ] set `presence_penalty` and `frequency_penalty`
     - [ ] set `logit_bias`
 - [X] Embeddings
     - [X] batch process
 - [ ] Chat
+- [ ] List model
 
 #### Supported backed
 - [X] [llama.cpp](https://github.com/ggerganov/llama.cpp) via [llamacpp-python](https://github.com/thomasantony/llamacpp-python)
+- [X] [llama](https://github.com/facebookresearch/llama) via [pyllama](https://github.com/juncongmoo/pyllama)
+    - [X] Without Quantization
+    - [X] With Quantization
 
 #### Others
 - [X] Performance parameters like `n_batch` and `n_thread`
+- [X] Token auth
 - [ ] Documents
-- [ ] Token auth
 - [ ] Intergration tests
 - [ ] A tool to download/prepare pretrain model
+- [ ] Make config.ini and token file configable
```

