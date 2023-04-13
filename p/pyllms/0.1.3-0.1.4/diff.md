# Comparing `tmp/pyllms-0.1.3.tar.gz` & `tmp/pyllms-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllms-0.1.3.tar", last modified: Thu Apr 13 02:50:24 2023, max compression
+gzip compressed data, was "pyllms-0.1.4.tar", last modified: Thu Apr 13 22:14:21 2023, max compression
```

## Comparing `pyllms-0.1.3.tar` & `pyllms-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 02:50:24.089695 pyllms-0.1.3/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.3/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)    12096 2023-04-13 02:50:24.089385 pyllms-0.1.3/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)    10933 2023-04-13 02:43:49.000000 pyllms-0.1.3/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 02:50:24.086948 pyllms-0.1.3/llms/
--rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.1.3/llms/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)    16270 2023-04-13 02:48:48.000000 pyllms-0.1.3/llms/llms.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 02:50:24.087978 pyllms-0.1.3/llms/providers/
--rw-r--r--   0 prelovac   (502) staff       (20)      107 2023-04-09 20:11:29.000000 pyllms-0.1.3/llms/providers/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2397 2023-04-13 02:27:57.000000 pyllms-0.1.3/llms/providers/ai21.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2756 2023-04-13 02:27:53.000000 pyllms-0.1.3/llms/providers/anthropic.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2421 2023-04-13 02:28:08.000000 pyllms-0.1.3/llms/providers/openai.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 02:50:24.089054 pyllms-0.1.3/pyllms.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)    12096 2023-04-13 02:50:24.000000 pyllms-0.1.3/pyllms.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      308 2023-04-13 02:50:24.000000 pyllms-0.1.3/pyllms.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-13 02:50:24.000000 pyllms-0.1.3/pyllms.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       60 2023-04-13 02:50:24.000000 pyllms-0.1.3/pyllms.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-13 02:50:24.000000 pyllms-0.1.3/pyllms.egg-info/top_level.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-13 02:50:24.089774 pyllms-0.1.3/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1682 2023-04-13 02:49:56.000000 pyllms-0.1.3/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 22:14:21.413453 pyllms-0.1.4/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.4/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)    13651 2023-04-13 22:14:21.413151 pyllms-0.1.4/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    12410 2023-04-13 22:10:16.000000 pyllms-0.1.4/README.md
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 22:14:21.410615 pyllms-0.1.4/llms/
+-rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.1.4/llms/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    16855 2023-04-13 22:03:17.000000 pyllms-0.1.4/llms/llms.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 22:14:21.411758 pyllms-0.1.4/llms/providers/
+-rw-r--r--   0 prelovac   (502) staff       (20)      107 2023-04-09 20:11:29.000000 pyllms-0.1.4/llms/providers/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2333 2023-04-13 21:39:49.000000 pyllms-0.1.4/llms/providers/ai21.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     4084 2023-04-13 22:10:49.000000 pyllms-0.1.4/llms/providers/anthropic.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3569 2023-04-13 21:35:11.000000 pyllms-0.1.4/llms/providers/openai.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 22:14:21.412820 pyllms-0.1.4/pyllms.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)    13651 2023-04-13 22:14:21.000000 pyllms-0.1.4/pyllms.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      308 2023-04-13 22:14:21.000000 pyllms-0.1.4/pyllms.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-13 22:14:21.000000 pyllms-0.1.4/pyllms.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       60 2023-04-13 22:14:21.000000 pyllms-0.1.4/pyllms.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-13 22:14:21.000000 pyllms-0.1.4/pyllms.egg-info/top_level.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-13 22:14:21.413544 pyllms-0.1.4/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     1760 2023-04-13 22:13:55.000000 pyllms-0.1.4/setup.py
```

### Comparing `pyllms-0.1.3/LICENSE` & `pyllms-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.3/PKG-INFO` & `pyllms-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: pyllms
-Version: 0.1.3
-Summary: A brief description of your package
-Author: Vladimir Prelovac
-Author-email: vlad@kagi.com
-Project-URL: Documentation, https://github.com/kagisearch/pyllms
-Project-URL: Source Code, https://github.com/kagisearch/pyllms
-Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
-Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
-Classifier: Topic :: Text Processing
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyLLMs
 
 A lightweight Python that strives to enable dead-simple interaction with popular language models from OpenAI, Anthropic, AI21 and others.
 
 ## Installation
 
 Clone this repository and install the package using pip:
@@ -85,30 +59,57 @@
 The result will also contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and response latency in the 'meta' field:
 ```
 >>> print(result.meta)
 {'model': 'gpt-3.5-turbo', 'tokens': 15, 'tokens_prompt': 14, 'tokens_completion': 1, 'cost': 3e-05, 'latency': 0.48232388496398926}
 ```
 
 
-
-
 ## Multi-model usage
 
 You can also initialize multiple models at once! This is very useful for testing and comparing output of different models in parallel. 
 
 ```
 >>> models=llms.init(model=['gpt-3.5-turbo','claude-instant-v1'])
 >>> result=models.complete('what is the capital of country where mozzart was born')
 >>> print(result.text)
 ['The capital of the country where Mozart was born is Vienna, Austria.', 'Wolfgang Amadeus Mozart was born in Salzburg, Austria.\n\nSo the capital of the country where Mozart was born is Vienna, Austria.']
 
 >>> print(result.meta)
 [{'model': 'gpt-3.5-turbo', 'tokens': 34, 'tokens_prompt': 20, 'tokens_completion': 14, 'cost': 6.8e-05, 'latency': 0.7097790241241455}, {'model': 'claude-instant-v1', 'tokens': 54, 'tokens_prompt': 20, 'tokens_completion': 34, 'cost': 5.79e-05, 'latency': 0.7291600704193115}]
 ```
 
+## Streaming support
+
+PyLLMs supports streaming from compatible models. 'complete_stream' method will return generator object and all you have to do is iterate through it:
+
+```
+>>> model= llms.init('claude-v1')
+>>> result = model.complete_stream("write an essay on civil war")
+>>> for chunks in result:
+...        if content is not None:
+...          print(chunks, end='')   
+... 
+
+Here is a paragraph about civil rights:
+
+
+Civil rights are the basic rights and freedoms that all citizens should have in a society. They include fundamental rights like the right to vote, the right to free speech, the right to practice the religion of one's choice, the right to equal treatment under the law, and the right to live free from discrimination. The civil rights movement in the United States fought to secure these rights for African Americans and other minorities in the face of institutionalized racism and discrimination. Leaders like Martin Luther King Jr. helped pass laws like the Civil Rights Act of 1964 and the Voting Rights Act of 1965 which outlawed discrimination and dismantled barriers to voting. The struggle for civil rights continues today as more work is still needed to promote racial equality and protect the rights of all citizens.
+
+```
+
+Current limitations:
+- When streaming, 'meta' is not available
+- Multi-models are not supported for streaming
+
+
+Tip: if you are testing this in python3 CLI, run it with -u parameter to disable buffering:
+
+```
+python3 -u
+```
 
 ## Benchmarks
 
 Models are appearing like mushrooms after rain and we are interested in:
 
 1) Quality
 2) Speed
```

### Comparing `pyllms-0.1.3/llms/llms.py` & `pyllms-0.1.4/llms/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     def text(self):
         if len(self._results) == 1:
             return self._results[0]["text"]
         return [result["text"] for result in self._results]
 
     @property
     def html(self):
+        if len(self._results) == 1:
+            return markdown2.markdown(self._results[0]["text"])
         return [markdown2.markdown(result["text"]) for result in self._results]
 
     @property
     def meta(self):
         if len(self._results) == 1:
             return self._results[0]["meta"]
         return [result["meta"] for result in self._results]
@@ -98,38 +100,52 @@
         )
         return sorted_list
 
     def complete(self, prompt, history=None, **kwargs):
         def _generate(provider):
            
             response = provider.complete(prompt, history, **kwargs)
-            
+    
             formatted_cost = format(response["meta"]["cost"], '.5f')
             formatted_latency = round(response["meta"]["latency"], 2)
             
             response["meta"]["cost"] = formatted_cost
             response["meta"]["latency"] = formatted_latency
 
             return {
                 "text": response["text"],
                 "meta": response["meta"],
                 "provider": provider,
             }
-
+     
         results = []
         with ThreadPoolExecutor() as executor:
             futures = {
                 executor.submit(_generate, provider): provider
                 for provider in self._providers
             }
             for future in as_completed(futures):
                 results.append(future.result())
 
         return Result(results)
 
+    def complete_stream(self, prompt, history=None, **kwargs):
+                 
+        if len(self._providers)>1:
+            raise ValueError(
+                "Streaming is possible only with a single model"
+            )
+        if isinstance(self._providers[0], AI21Provider):
+            raise ValueError(
+                "Streaming is not yet supported with AI21 models"
+            )
+            
+        yield from self._providers[0].complete_stream(prompt, history, **kwargs)
+
+
     def benchmark(self, prompts=None, evaluator=None, show_outputs=False, html=False):
         if not prompts:
             prompts = [
                 "What is the capital of the country where Christopher Columbus was born?",
                 "A glass door has ‘push’ written on it in mirror writing. Should you push or pull it and why?",
                 "Solve the quadratic equation: x^2 - 5x + 6 = 0",
                 "How much is 7! * 3! -1234.5 ?",
```

### Comparing `pyllms-0.1.3/llms/providers/ai21.py` & `pyllms-0.1.4/llms/providers/ai21.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,18 +34,17 @@
 
         if history is not None:
             role_cycle = itertools.cycle((HUMAN_PROMPT, AI_PROMPT))
             history_messages = itertools.chain.from_iterable(history)
             history_prompt = "".join(itertools.chain.from_iterable(zip(role_cycle, history_messages)))
             prompt = f"{history_prompt}{prompt}"
 
-        maxTokens = max_tokens  # Assign max_tokens to maxTokens
 
         if 'maxTokens' not in kwargs:
-            kwargs['maxTokens'] = maxTokens  # Add maxTokens to kwargs if not present
+            kwargs['maxTokens'] = max_tokens  # Add maxTokens to kwargs if not present
 
         start_time = time.time()
         response = ai21.Completion.execute(model=self.model, prompt=prompt, temperature=temperature, **kwargs)
         latency = time.time() - start_time
 
         completion = response.completions[0].data.text.strip()
         prompt_tokens = len(response.prompt.tokens)
```

### Comparing `pyllms-0.1.3/llms/providers/anthropic.py` & `pyllms-0.1.4/llms/providers/anthropic.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,18 +37,16 @@
         formatted_prompt = f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}"
         if history is not None:
             role_cycle = itertools.cycle((anthropic.HUMAN_PROMPT, anthropic.AI_PROMPT))
             history_messages = itertools.chain.from_iterable(history)
             history_prompt = "".join(itertools.chain.from_iterable(zip(role_cycle, history_messages)))
             formatted_prompt = f"{history_prompt}{formatted_prompt}"
 
-        max_tokens_to_sample = max_tokens  # Assign max_tokens to maxTokens
-
         if 'max_tokens_to_sample' not in kwargs:
-            kwargs['max_tokens_to_sample'] = max_tokens_to_sample  # Add maxTokens to kwargs if not present
+            kwargs['max_tokens_to_sample'] = max_tokens  # Add maxTokens to kwargs if not present
 
         start_time = time.time()
         response = self.client.completion(
             prompt=formatted_prompt,
             stop_sequences=[anthropic.HUMAN_PROMPT],
             temperature=temperature,
             model=self.model,
@@ -74,7 +72,47 @@
                 "tokens": total_tokens,
                 "tokens_prompt": prompt_tokens,
                 "tokens_completion": completion_tokens,
                 "cost": cost,
                 "latency": latency,
             },
         }
+
+
+    def complete_stream(self,
+                 prompt: str,
+                 history: Optional[List[tuple]] = None,
+                 temperature: float = 0,
+                 max_tokens: int = 300,
+                 **kwargs
+                 ):
+
+        formatted_prompt = f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}"
+        if history is not None:
+            role_cycle = itertools.cycle((anthropic.HUMAN_PROMPT, anthropic.AI_PROMPT))
+            history_messages = itertools.chain.from_iterable(history)
+            history_prompt = "".join(itertools.chain.from_iterable(zip(role_cycle, history_messages)))
+            formatted_prompt = f"{history_prompt}{formatted_prompt}"
+
+
+        if 'max_tokens_to_sample' not in kwargs:
+            kwargs['max_tokens_to_sample'] = max_tokens  # Add maxTokens to kwargs if not present
+
+        if 'stream' not in kwargs:
+            kwargs['stream'] = True  # Add stream param if not present
+
+        response = self.client.completion_stream(
+            prompt=formatted_prompt,
+            stop_sequences=[anthropic.HUMAN_PROMPT],
+            temperature=temperature,
+            model=self.model,
+            **kwargs,
+        )
+    
+        last_completion = ""
+        for data in response:
+            new_chunk = data['completion'][len(last_completion):]
+            last_completion = data['completion']  
+            yield(new_chunk)
+
+       
+
```

### Comparing `pyllms-0.1.3/setup.py` & `pyllms-0.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 _project_homepage = "https://github.com/kagisearch/pyllms"
 
 setup(
     name="pyllms",
-    version="0.1.3",
-    description="A brief description of your package",
+    version="0.1.4",
+    description="Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vladimir Prelovac",
     author_email="vlad@kagi.com",
     packages=find_packages(),
     install_requires=[
         "openai",
```

