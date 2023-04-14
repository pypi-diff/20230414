# Comparing `tmp/gpt-api-0.1.1.tar.gz` & `tmp/gpt-api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-api-0.1.1.tar", last modified: Thu Apr 13 02:23:57 2023, max compression
+gzip compressed data, was "gpt-api-0.2.1.tar", last modified: Fri Apr 14 09:17:15 2023, max compression
```

## Comparing `gpt-api-0.1.1.tar` & `gpt-api-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:57.857870 gpt-api-0.1.1/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-13 02:23:57.857556 gpt-api-0.1.1/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:57.854143 gpt-api-0.1.1/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt-api-0.1.1/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)     3762 2023-04-13 02:09:07.000000 gpt-api-0.1.1/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:57.857118 gpt-api-0.1.1/gpt_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-13 02:23:57.000000 gpt-api-0.1.1/gpt_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      189 2023-04-13 02:23:57.000000 gpt-api-0.1.1/gpt_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-04-13 02:23:57.000000 gpt-api-0.1.1/gpt_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-04-13 02:23:57.000000 gpt-api-0.1.1/gpt_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-04-13 02:23:57.000000 gpt-api-0.1.1/gpt_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-04-13 02:23:57.857995 gpt-api-0.1.1/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      765 2023-04-13 02:23:39.000000 gpt-api-0.1.1/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 09:17:15.782808 gpt-api-0.2.1/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-14 09:17:15.782120 gpt-api-0.2.1/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 09:17:15.779531 gpt-api-0.2.1/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt-api-0.2.1/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)     3924 2023-04-14 09:16:21.000000 gpt-api-0.2.1/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 09:17:15.781610 gpt-api-0.2.1/gpt_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-14 09:17:15.000000 gpt-api-0.2.1/gpt_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      189 2023-04-14 09:17:15.000000 gpt-api-0.2.1/gpt_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-04-14 09:17:15.000000 gpt-api-0.2.1/gpt_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-04-14 09:17:15.000000 gpt-api-0.2.1/gpt_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-04-14 09:17:15.000000 gpt-api-0.2.1/gpt_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-04-14 09:17:15.782977 gpt-api-0.2.1/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      765 2023-04-13 02:23:39.000000 gpt-api-0.2.1/setup.py
```

### Comparing `gpt-api-0.1.1/api/gpt.py` & `gpt-api-0.2.1/api/gpt.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,80 +5,84 @@
 import asyncio
 from pathlib import Path
 log = getLogger(__name__)
 log.setLevel(INFO)
 
 
 class GPT4(object):
-    def __init__(self, key=None, model='gpt-4-0314', temperature=0.8, top_p=1, presence_penalty=0, frequency_penalty=0, n=1, system_content=None):
+    def __init__(self, key=None, model='gpt-4', temperature=0.8, top_p=1, presence_penalty=0, frequency_penalty=0, n=1, stream=False, system_content=None):
         if os.environ.get("OPENAI_API_KEY") is None:
             if key:
                 openai.api_key = key
         self.model = model
         self.temperature = temperature
         # 用于控制生成文本的随机性和创造性的参数。值越高，生成文本越随机和创造性；值越低，生成文本越可预测和保守
         self.top_p = top_p
         # 用于对生成文本进行选择的参数，它表示只选择所有可能的令牌中累计概率高于给定阈值的那些令牌。默认值为1，表示选择所有可能的令牌
         self.presence_penalty = presence_penalty
         # 用于惩罚生成文本中未出现过的片段的参数。默认值为0，表示不进行惩罚
         self.frequency_penalty = frequency_penalty
         # 用于惩罚生成文本中频繁出现的重复片段的参数。默认值为0，表示不进行惩罚
         self.n = n
         # 要生成的文本的数量。默认为1，表示生成一段文本
-        self.stream = True
+        self.stream = stream
         # 是否将生成的文本作为流返回，而不是一次性返回所有文本。默认为False，表示一次性返回所有文本
         self.system_content = system_content or "一个拥有20年经验的c++程序员，帮助分析代码问题"
         self.messages = [
             {"role": "system", "content": self.system_content}
         ]
 
     @staticmethod
     def read_prompt(path):
         return Path(path).read_text()
 
     def asyncio_run_gpt_ask(self, prompt, realTime_output=False):
-        if self.stream:
-            if realTime_output:
-                print("## You")
-                print(prompt)
-                print("\n")
-                print("## chatGPT")
-            return asyncio.run(self.__ask(prompt, realTime_output))[0]
-        else:
-            return False
-
-    async def __ask(self, prompt, realTime_output=False):
         if len(self.messages) == 0:
             self.messages.append({"role": "system", "content": self.system_content})
         self.messages.append({"role": "user", "content": prompt})
+        if realTime_output:
+            print("## You")
+            print(prompt)
+            print("## chatGPT")
+        if self.stream:
+            return asyncio.run(self.__ask(realTime_output))[0]
+        else:
+            start_time = time.time()
+            response = openai.ChatCompletion.create(
+                model=self.model,
+                messages=self.messages,
+                temperature=self.temperature
+            )
+            elapsed_time = time.time() - start_time
+            return response['choices'][0]['message']['content'], int(round(elapsed_time, 0))
+
+    async def __ask(self, realTime_output=False):
         return await asyncio.gather(*[self.__generate_text_async(realTime_output)])
 
     async def __generate_text_async(self, realTime_output) -> tuple:
         response_text_array = []
         response_text = ""
         start_time = time.time()
         async for chunk in await openai.ChatCompletion.acreate(
             model=self.model,
             messages=self.messages,
+            # max_tokens=7000,
             temperature=self.temperature,
             top_p=self.top_p,
+            # timeout=600,
             presence_penalty=self.presence_penalty,
             frequency_penalty=self.frequency_penalty,
             n=self.n,
             stream=self.stream
         ):
-            if self.stream:
-                chunk = chunk['choices'][0]
-                if "content" in chunk["delta"]:
-                    text = chunk["delta"]['content']
-                    response_text += text
-                    if text in ["\n"]:
-                        response_text_array.append(response_text)
-                        if realTime_output:
-                            print(response_text)
-                        response_text = ""
-            else:
-                response_text = chunk.choices[0]["delta"]['content']
+            chunk = chunk['choices'][0]
+            if "content" in chunk["delta"]:
+                text = chunk["delta"]['content']
+                response_text += text
+                if text in ["\n"]:
+                    response_text_array.append(response_text)
+                    if realTime_output:
+                        print(response_text)
+                    response_text = ""
         elapsed_time = time.time() - start_time
         log.info(f"{elapsed_time:.2f} seconds to execute")
-        response_text = "\n".join(response_text_array)
-        return response_text, int(round(elapsed_time, 0))
+        return "\n".join(response_text_array), int(round(elapsed_time, 0))
```

### Comparing `gpt-api-0.1.1/setup.py` & `gpt-api-0.2.1/setup.py`

 * *Files identical despite different names*

