# Comparing `tmp/gpt-api-0.1.2.tar.gz` & `tmp/gpt-api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-api-0.1.2.tar", last modified: Thu Apr 13 09:31:33 2023, max compression
+gzip compressed data, was "gpt-api-0.1.3.tar", last modified: Fri Apr 14 02:29:27 2023, max compression
```

## Comparing `gpt-api-0.1.2.tar` & `gpt-api-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 09:31:33.239142 gpt-api-0.1.2/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-13 09:31:33.238877 gpt-api-0.1.2/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 09:31:33.236752 gpt-api-0.1.2/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt-api-0.1.2/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)     3757 2023-04-13 09:31:10.000000 gpt-api-0.1.2/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 09:31:33.238499 gpt-api-0.1.2/gpt_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-13 09:31:33.000000 gpt-api-0.1.2/gpt_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      189 2023-04-13 09:31:33.000000 gpt-api-0.1.2/gpt_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-04-13 09:31:33.000000 gpt-api-0.1.2/gpt_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-04-13 09:31:33.000000 gpt-api-0.1.2/gpt_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-04-13 09:31:33.000000 gpt-api-0.1.2/gpt_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-04-13 09:31:33.239241 gpt-api-0.1.2/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      765 2023-04-13 02:23:39.000000 gpt-api-0.1.2/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 02:29:27.063912 gpt-api-0.1.3/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-14 02:29:27.063501 gpt-api-0.1.3/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 02:29:27.061498 gpt-api-0.1.3/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt-api-0.1.3/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)     3811 2023-04-14 02:27:51.000000 gpt-api-0.1.3/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 02:29:27.062960 gpt-api-0.1.3/gpt_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-14 02:29:27.000000 gpt-api-0.1.3/gpt_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      189 2023-04-14 02:29:27.000000 gpt-api-0.1.3/gpt_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-04-14 02:29:27.000000 gpt-api-0.1.3/gpt_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-04-14 02:29:27.000000 gpt-api-0.1.3/gpt_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-04-14 02:29:27.000000 gpt-api-0.1.3/gpt_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-04-14 02:29:27.064083 gpt-api-0.1.3/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      765 2023-04-13 02:23:39.000000 gpt-api-0.1.3/setup.py
```

### Comparing `gpt-api-0.1.2/api/gpt.py` & `gpt-api-0.1.3/api/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,18 @@
     async def __generate_text_async(self, realTime_output) -> tuple:
         response_text_array = []
         response_text = ""
         start_time = time.time()
         async for chunk in await openai.ChatCompletion.acreate(
             model=self.model,
             messages=self.messages,
+            max_tokens=4096,
             temperature=self.temperature,
             top_p=self.top_p,
+            timeout=600,
             presence_penalty=self.presence_penalty,
             frequency_penalty=self.frequency_penalty,
             n=self.n,
             stream=self.stream
         ):
             if self.stream:
                 chunk = chunk['choices'][0]
```

### Comparing `gpt-api-0.1.2/setup.py` & `gpt-api-0.1.3/setup.py`

 * *Files identical despite different names*

