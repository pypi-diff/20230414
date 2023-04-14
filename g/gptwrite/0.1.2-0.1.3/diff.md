# Comparing `tmp/gptwrite-0.1.2.tar.gz` & `tmp/gptwrite-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptwrite-0.1.2.tar", max compression
+gzip compressed data, was "gptwrite-0.1.3.tar", max compression
```

## Comparing `gptwrite-0.1.2.tar` & `gptwrite-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-04-14 07:11:21.401780 gptwrite-0.1.2/LICENSE
--rw-r--r--   0        0        0      888 2023-04-14 16:45:09.409762 gptwrite-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-14 06:16:34.208243 gptwrite-0.1.2/gptwrite/__init__.py
--rw-r--r--   0        0        0     2743 2023-04-14 05:00:14.431977 gptwrite-0.1.2/gptwrite/accepted_language.py
--rw-r--r--   0        0        0     4558 2023-04-14 16:57:41.208171 gptwrite-0.1.2/gptwrite/core.py
--rw-r--r--   0        0        0      992 2023-04-14 16:42:13.161836 gptwrite-0.1.2/gptwrite/locales/messages.en.yaml
--rw-r--r--   0        0        0     1242 2023-04-14 16:41:42.455582 gptwrite-0.1.2/gptwrite/locales/messages.ja.yaml
--rwxr-xr-x   0        0        0     2786 2023-04-14 16:21:46.515115 gptwrite-0.1.2/gptwrite/main.py
--rw-r--r--   0        0        0     2642 2023-04-14 16:52:13.826245 gptwrite-0.1.2/gptwrite/prompts.py
--rw-r--r--   0        0        0      516 2023-04-14 16:14:00.271931 gptwrite-0.1.2/gptwrite/util.py
--rw-r--r--   0        0        0      770 2023-04-14 17:03:39.408110 gptwrite-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 gptwrite-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-14 07:11:21.401780 gptwrite-0.1.3/LICENSE
+-rw-r--r--   0        0        0      888 2023-04-14 16:45:09.409762 gptwrite-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 06:16:34.208243 gptwrite-0.1.3/gptwrite/__init__.py
+-rw-r--r--   0        0        0     2743 2023-04-14 05:00:14.431977 gptwrite-0.1.3/gptwrite/accepted_language.py
+-rw-r--r--   0        0        0     4679 2023-04-14 17:33:30.849479 gptwrite-0.1.3/gptwrite/core.py
+-rw-r--r--   0        0        0      992 2023-04-14 16:42:13.161836 gptwrite-0.1.3/gptwrite/locales/messages.en.yaml
+-rw-r--r--   0        0        0     1242 2023-04-14 16:41:42.455582 gptwrite-0.1.3/gptwrite/locales/messages.ja.yaml
+-rwxr-xr-x   0        0        0     2786 2023-04-14 16:21:46.515115 gptwrite-0.1.3/gptwrite/main.py
+-rw-r--r--   0        0        0     2642 2023-04-14 16:52:13.826245 gptwrite-0.1.3/gptwrite/prompts.py
+-rw-r--r--   0        0        0      516 2023-04-14 16:14:00.271931 gptwrite-0.1.3/gptwrite/util.py
+-rw-r--r--   0        0        0      809 2023-04-14 17:40:11.866157 gptwrite-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 gptwrite-0.1.3/PKG-INFO
```

### Comparing `gptwrite-0.1.2/LICENSE` & `gptwrite-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.2/README.md` & `gptwrite-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.2/gptwrite/accepted_language.py` & `gptwrite-0.1.3/gptwrite/accepted_language.py`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.2/gptwrite/core.py` & `gptwrite-0.1.3/gptwrite/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import List, Callable, Optional, Dict
 import i18n
 import openai
 import questionary
 from gptwrite.prompts import build_prompt_generate_topics, build_prompt_generate_texts, build_prompt_rewrite_texts
 
 
-GenerateFunc = Callable[[str, List[str], Optional[str], str, str], str]
 OpenAIMessages = List[Dict[str, str]]
+GenerateFunc = Callable[[OpenAIMessages, str, Optional[str]], str]
 
 ACTIONS = ["Thought", "Consult", "Write"]
 
 logger = logging.getLogger(__name__)
 
 
 def generate_text_by_llm(
@@ -38,17 +38,18 @@
 
 def generate_topics(
         theme: str,
         lang_for_generating: str,
         nuance: Optional[str] = None,
         generate_text_func: GenerateFunc = generate_text_by_llm,
     ) -> List[str]:
+    prompt = build_prompt_generate_topics(theme=theme, language=lang_for_generating, nuance=nuance)
     messages = [{
         "role": "user",
-        "content": build_prompt_generate_topics(theme, lang_for_generating, nuance)
+        "content": prompt,
     }]
     content = generate_text_func(messages=messages)
     return put_generated_text_into_list(content)
 
 def put_generated_text_into_list(text: str) -> List[str]:
     topics = []
     for line in text.split("\n"):
@@ -66,69 +67,71 @@
             topics.append(line[len(num_list_match.groups()[0]):].strip())
             continue
     return topics
 
 def generate_texts(
         theme: str,
         topics: List[str],
-        nuance: Optional[str],
+        nuance: str,
         lang_for_generating: str,
         lang_for_description: str,
         generate_text_func: GenerateFunc  = generate_text_by_llm,
     ) -> str:
+    prompt = build_prompt_generate_texts(theme=theme, topics=topics, nuance=nuance, language=lang_for_generating)
     messages = [{
         "role": "user",
-        "content": build_prompt_generate_texts(theme, topics, nuance, lang_for_generating)
+        "content": prompt,
     }]
 
     writes = []
 
     while True:
         content = generate_text_func(messages=messages, stop="\n\n")
         print(content)
 
         if content.startswith("[Consult]"):
             comprementary = questionary.text(i18n.t("messages.want_complementary", locale=lang_for_description)).unsafe_ask()
             messages.append({
                 "role": "user",
-                "content": f"[Complement]{comprementary}"
+                "content": f"[Complement]{comprementary}",
             })
             continue
 
         if content.startswith("[Thought]"):
             messages.append({
                 "role": "assistant",
-                "content": content
+                "content": content,
             })
             continue
         
         if content.startswith("[Write]"):
             writes.append(content[7:].strip())
             if not questionary.confirm(i18n.t("messages.confirm_want_more", locale=lang_for_description)).unsafe_ask():
                 break
             messages.append({
                 "role": "assistant",
-                "content": f"[Request]{i18n.t('messages.want_more', locale=lang_for_description)}"
+                "content": f"[Request]{i18n.t('messages.want_more', locale=lang_for_description)}",
             }) 
             continue
 
         messages.append({"role": "system", "content": i18n.t("messages.", locale=lang_for_description)})
 
     return rewrite_texts(writes, lang_for_generating, lang_for_description, generate_text_func)
 
 def rewrite_texts(
         sentences: List[str],
         lang_for_generating: str,
         lang_for_description: str,
         generate_text_func: GenerateFunc = generate_text_by_llm,
     ) -> str:
     print(i18n.t("messages.rewrite", locale=lang_for_description))
+    prompt = build_prompt_rewrite_texts(sentences=sentences, language=lang_for_generating)
     messages = [{
         "role": "user",
-        "content": build_prompt_rewrite_texts(sentences, lang_for_generating)
+        "content": prompt,
     }]
 
     result_texts = ""
     while True:
         content = generate_text_func(messages)
         print(content)
         result_texts += content
```

### Comparing `gptwrite-0.1.2/gptwrite/locales/messages.en.yaml` & `gptwrite-0.1.3/gptwrite/locales/messages.en.yaml`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.2/gptwrite/locales/messages.ja.yaml` & `gptwrite-0.1.3/gptwrite/locales/messages.ja.yaml`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.2/gptwrite/main.py` & `gptwrite-0.1.3/gptwrite/main.py`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.2/gptwrite/prompts.py` & `gptwrite-0.1.3/gptwrite/prompts.py`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.2/gptwrite/util.py` & `gptwrite-0.1.3/gptwrite/util.py`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.2/PKG-INFO` & `gptwrite-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptwrite
-Version: 0.1.2
+Version: 0.1.3
 Summary: CLI for Automated article writing
 Home-page: https://github.com/otakumesi/gpt-write
 License: MIT
 Keywords: gpt,openai,cli,article,writing
 Author: otakumesi
 Author-email: bakednt@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click
 Requires-Dist: iso639-lang
 Requires-Dist: openai
 Requires-Dist: python-i18n[yaml]
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
+Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Project-URL: Repository, https://github.com/otakumesi/gpt-write
 Description-Content-Type: text/markdown
 
 # GPT-Write :writing_hand:
 
 __GPT make writing an article brazing fast :fire:.__
```

