# Comparing `tmp/gptwrite-0.1.0.tar.gz` & `tmp/gptwrite-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptwrite-0.1.0.tar", max compression
+gzip compressed data, was "gptwrite-0.1.1.tar", max compression
```

## Comparing `gptwrite-0.1.0.tar` & `gptwrite-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-04-14 07:11:21.401780 gptwrite-0.1.0/LICENSE
--rw-r--r--   0        0        0      613 2023-04-14 11:39:25.153660 gptwrite-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-14 06:16:34.208243 gptwrite-0.1.0/gptwrite/__init__.py
--rw-r--r--   0        0        0     2743 2023-04-14 05:00:14.431977 gptwrite-0.1.0/gptwrite/accepted_language.py
--rw-r--r--   0        0        0     3445 2023-04-14 09:21:01.755399 gptwrite-0.1.0/gptwrite/core.py
--rw-r--r--   0        0        0      928 2023-04-14 04:44:50.773866 gptwrite-0.1.0/gptwrite/locales/messages.en.yaml
--rw-r--r--   0        0        0     1161 2023-04-14 04:44:54.886027 gptwrite-0.1.0/gptwrite/locales/messages.ja.yaml
--rwxr-xr-x   0        0        0     2786 2023-04-14 09:02:24.246429 gptwrite-0.1.0/gptwrite/main.py
--rw-r--r--   0        0        0     2468 2023-04-14 09:22:44.209502 gptwrite-0.1.0/gptwrite/prompts.py
--rw-r--r--   0        0        0      479 2023-04-14 07:01:47.032687 gptwrite-0.1.0/gptwrite/util.py
--rw-r--r--   0        0        0      770 2023-04-14 07:40:00.527530 gptwrite-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 gptwrite-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-14 07:11:21.401780 gptwrite-0.1.1/LICENSE
+-rw-r--r--   0        0        0      704 2023-04-14 12:43:12.028075 gptwrite-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 06:16:34.208243 gptwrite-0.1.1/gptwrite/__init__.py
+-rw-r--r--   0        0        0     2743 2023-04-14 05:00:14.431977 gptwrite-0.1.1/gptwrite/accepted_language.py
+-rw-r--r--   0        0        0     3445 2023-04-14 12:58:39.539409 gptwrite-0.1.1/gptwrite/core.py
+-rw-r--r--   0        0        0      928 2023-04-14 04:44:50.773866 gptwrite-0.1.1/gptwrite/locales/messages.en.yaml
+-rw-r--r--   0        0        0     1161 2023-04-14 04:44:54.886027 gptwrite-0.1.1/gptwrite/locales/messages.ja.yaml
+-rwxr-xr-x   0        0        0     2786 2023-04-14 09:02:24.246429 gptwrite-0.1.1/gptwrite/main.py
+-rw-r--r--   0        0        0     2468 2023-04-14 09:22:44.209502 gptwrite-0.1.1/gptwrite/prompts.py
+-rw-r--r--   0        0        0      479 2023-04-14 07:01:47.032687 gptwrite-0.1.1/gptwrite/util.py
+-rw-r--r--   0        0        0      770 2023-04-14 13:00:22.251884 gptwrite-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1536 1970-01-01 00:00:00.000000 gptwrite-0.1.1/PKG-INFO
```

### Comparing `gptwrite-0.1.0/LICENSE` & `gptwrite-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.0/README.md` & `gptwrite-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # GPT-Write✍️
 
 GPT make writing an article brazing fast🔥.  
----
+![GPT-Write Demo](https://github.com/otakumesi/gpt-write/blob/main/demo.gif?raw=true "デモ")
 
 ## What's this tool?
 
 GPT-Write is the CLI tool for Intractive Automated Article Writing.  
 You can create articles, just answer the questions.   
 Since the language is specified in the prompt and GPT is allowed to generate the text, it could theoretically be used in a variety of languages.
```

### Comparing `gptwrite-0.1.0/gptwrite/accepted_language.py` & `gptwrite-0.1.1/gptwrite/accepted_language.py`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.0/gptwrite/core.py` & `gptwrite-0.1.1/gptwrite/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,22 +62,22 @@
         content = response.choices[0].message.content
         print(content)
 
         if content.startswith("[Consult]"):
             comprementary = questionary.text(i18n.t("messages.want_complementary", locale=lang_for_description)).unsafe_ask()
             messages.append({
                 "role": "user",
-                "content": comprementary
+                "content": f"[Complement]{comprementary}"
             })
             continue
 
         if content.startswith("[Thought]"):
             messages.append({
                 "role": "assistant",
-                "content": f"[Complement]{content}"
+                "content": content
             })
             continue
         
         if content.startswith("[Write]"):
             writes.append(content[7:].strip())
             if not questionary.confirm(i18n.t("messages.confirm_want_more", locale=lang_for_description)).unsafe_ask():
                 break
```

### Comparing `gptwrite-0.1.0/gptwrite/locales/messages.en.yaml` & `gptwrite-0.1.1/gptwrite/locales/messages.en.yaml`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.0/gptwrite/locales/messages.ja.yaml` & `gptwrite-0.1.1/gptwrite/locales/messages.ja.yaml`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.0/gptwrite/main.py` & `gptwrite-0.1.1/gptwrite/main.py`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.0/gptwrite/prompts.py` & `gptwrite-0.1.1/gptwrite/prompts.py`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.0/pyproject.toml` & `gptwrite-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gptwrite"
-version = "0.1.0"
+version = "0.1.1"
 description = "CLI for Automated article writing"
 authors = ["otakumesi <bakednt@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/otakumesi/gpt-write"
 repository = "https://github.com/otakumesi/gpt-write"
 readme = "README.md"
 keywords = ["gpt", "openai", "cli", "article", "writing"]
```

### Comparing `gptwrite-0.1.0/PKG-INFO` & `gptwrite-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptwrite
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI for Automated article writing
 Home-page: https://github.com/otakumesi/gpt-write
 License: MIT
 Keywords: gpt,openai,cli,article,writing
 Author: otakumesi
 Author-email: bakednt@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -21,15 +21,15 @@
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://github.com/otakumesi/gpt-write
 Description-Content-Type: text/markdown
 
 # GPT-Write✍️
 
 GPT make writing an article brazing fast🔥.  
----
+![GPT-Write Demo](https://github.com/otakumesi/gpt-write/blob/main/demo.gif?raw=true "デモ")
 
 ## What's this tool?
 
 GPT-Write is the CLI tool for Intractive Automated Article Writing.  
 You can create articles, just answer the questions.   
 Since the language is specified in the prompt and GPT is allowed to generate the text, it could theoretically be used in a variety of languages.
```

