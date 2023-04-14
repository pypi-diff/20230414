# Comparing `tmp/gpt-api-0.1.3.tar.gz` & `tmp/gpt-api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-api-0.1.3.tar", last modified: Fri Apr 14 02:29:27 2023, max compression
+gzip compressed data, was "gpt-api-0.2.0.tar", last modified: Fri Apr 14 04:40:51 2023, max compression
```

## Comparing `gpt-api-0.1.3.tar` & `gpt-api-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 02:29:27.063912 gpt-api-0.1.3/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-14 02:29:27.063501 gpt-api-0.1.3/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 02:29:27.061498 gpt-api-0.1.3/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt-api-0.1.3/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)     3811 2023-04-14 02:27:51.000000 gpt-api-0.1.3/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 02:29:27.062960 gpt-api-0.1.3/gpt_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-14 02:29:27.000000 gpt-api-0.1.3/gpt_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      189 2023-04-14 02:29:27.000000 gpt-api-0.1.3/gpt_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-04-14 02:29:27.000000 gpt-api-0.1.3/gpt_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-04-14 02:29:27.000000 gpt-api-0.1.3/gpt_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-04-14 02:29:27.000000 gpt-api-0.1.3/gpt_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-04-14 02:29:27.064083 gpt-api-0.1.3/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      765 2023-04-13 02:23:39.000000 gpt-api-0.1.3/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 04:40:51.959655 gpt-api-0.2.0/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-14 04:40:51.959313 gpt-api-0.2.0/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 04:40:51.956045 gpt-api-0.2.0/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt-api-0.2.0/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)     3666 2023-04-14 04:40:08.000000 gpt-api-0.2.0/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 04:40:51.958820 gpt-api-0.2.0/gpt_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-14 04:40:51.000000 gpt-api-0.2.0/gpt_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      189 2023-04-14 04:40:51.000000 gpt-api-0.2.0/gpt_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-04-14 04:40:51.000000 gpt-api-0.2.0/gpt_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-04-14 04:40:51.000000 gpt-api-0.2.0/gpt_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-04-14 04:40:51.000000 gpt-api-0.2.0/gpt_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-04-14 04:40:51.959784 gpt-api-0.2.0/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      765 2023-04-13 02:23:39.000000 gpt-api-0.2.0/setup.py
```

### Comparing `gpt-api-0.1.3/api/gpt.py` & `gpt-api-0.2.0/api/gpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import asyncio
 from pathlib import Path
 log = getLogger(__name__)
 log.setLevel(INFO)
 
 
 class GPT4(object):
-    def __init__(self, key=None, model='gpt-4', temperature=0.8, top_p=1, presence_penalty=0, frequency_penalty=0, n=1, system_content=None):
+    def __init__(self, key=None, model='gpt-4', top_p=1, presence_penalty=0, frequency_penalty=0, n=1, system_content=None):
         if os.environ.get("OPENAI_API_KEY") is None:
             if key:
                 openai.api_key = key
         self.model = model
-        self.temperature = temperature
+        self.temperature = 0.8
         # 用于控制生成文本的随机性和创造性的参数。值越高，生成文本越随机和创造性；值越低，生成文本越可预测和保守
         self.top_p = top_p
         # 用于对生成文本进行选择的参数，它表示只选择所有可能的令牌中累计概率高于给定阈值的那些令牌。默认值为1，表示选择所有可能的令牌
         self.presence_penalty = presence_penalty
         # 用于惩罚生成文本中未出现过的片段的参数。默认值为0，表示不进行惩罚
         self.frequency_penalty = frequency_penalty
         # 用于惩罚生成文本中频繁出现的重复片段的参数。默认值为0，表示不进行惩罚
@@ -36,15 +36,14 @@
         return Path(path).read_text()
 
     def asyncio_run_gpt_ask(self, prompt, realTime_output=False):
         if self.stream:
             if realTime_output:
                 print("## You")
                 print(prompt)
-                print("\n")
                 print("## chatGPT")
             return asyncio.run(self.__ask(prompt, realTime_output))[0]
         else:
             return False
 
     async def __ask(self, prompt, realTime_output=False):
         if len(self.messages) == 0:
@@ -55,18 +54,16 @@
     async def __generate_text_async(self, realTime_output) -> tuple:
         response_text_array = []
         response_text = ""
         start_time = time.time()
         async for chunk in await openai.ChatCompletion.acreate(
             model=self.model,
             messages=self.messages,
-            max_tokens=4096,
             temperature=self.temperature,
             top_p=self.top_p,
-            timeout=600,
             presence_penalty=self.presence_penalty,
             frequency_penalty=self.frequency_penalty,
             n=self.n,
             stream=self.stream
         ):
             if self.stream:
                 chunk = chunk['choices'][0]
@@ -78,9 +75,8 @@
                         if realTime_output:
                             print(response_text)
                         response_text = ""
             else:
                 response_text = chunk.choices[0]["delta"]['content']
         elapsed_time = time.time() - start_time
         log.info(f"{elapsed_time:.2f} seconds to execute")
-        response_text = "\n".join(response_text_array)
-        return response_text, int(round(elapsed_time, 0))
+        return "\n".join(response_text_array), int(round(elapsed_time, 0))
```

### Comparing `gpt-api-0.1.3/setup.py` & `gpt-api-0.2.0/setup.py`

 * *Files identical despite different names*

