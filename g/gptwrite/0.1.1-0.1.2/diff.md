# Comparing `tmp/gptwrite-0.1.1.tar.gz` & `tmp/gptwrite-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptwrite-0.1.1.tar", max compression
+gzip compressed data, was "gptwrite-0.1.2.tar", max compression
```

## Comparing `gptwrite-0.1.1.tar` & `gptwrite-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-04-14 07:11:21.401780 gptwrite-0.1.1/LICENSE
--rw-r--r--   0        0        0      704 2023-04-14 12:43:12.028075 gptwrite-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-14 06:16:34.208243 gptwrite-0.1.1/gptwrite/__init__.py
--rw-r--r--   0        0        0     2743 2023-04-14 05:00:14.431977 gptwrite-0.1.1/gptwrite/accepted_language.py
--rw-r--r--   0        0        0     3445 2023-04-14 12:58:39.539409 gptwrite-0.1.1/gptwrite/core.py
--rw-r--r--   0        0        0      928 2023-04-14 04:44:50.773866 gptwrite-0.1.1/gptwrite/locales/messages.en.yaml
--rw-r--r--   0        0        0     1161 2023-04-14 04:44:54.886027 gptwrite-0.1.1/gptwrite/locales/messages.ja.yaml
--rwxr-xr-x   0        0        0     2786 2023-04-14 09:02:24.246429 gptwrite-0.1.1/gptwrite/main.py
--rw-r--r--   0        0        0     2468 2023-04-14 09:22:44.209502 gptwrite-0.1.1/gptwrite/prompts.py
--rw-r--r--   0        0        0      479 2023-04-14 07:01:47.032687 gptwrite-0.1.1/gptwrite/util.py
--rw-r--r--   0        0        0      770 2023-04-14 13:00:22.251884 gptwrite-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1536 1970-01-01 00:00:00.000000 gptwrite-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-14 07:11:21.401780 gptwrite-0.1.2/LICENSE
+-rw-r--r--   0        0        0      888 2023-04-14 16:45:09.409762 gptwrite-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 06:16:34.208243 gptwrite-0.1.2/gptwrite/__init__.py
+-rw-r--r--   0        0        0     2743 2023-04-14 05:00:14.431977 gptwrite-0.1.2/gptwrite/accepted_language.py
+-rw-r--r--   0        0        0     4558 2023-04-14 16:57:41.208171 gptwrite-0.1.2/gptwrite/core.py
+-rw-r--r--   0        0        0      992 2023-04-14 16:42:13.161836 gptwrite-0.1.2/gptwrite/locales/messages.en.yaml
+-rw-r--r--   0        0        0     1242 2023-04-14 16:41:42.455582 gptwrite-0.1.2/gptwrite/locales/messages.ja.yaml
+-rwxr-xr-x   0        0        0     2786 2023-04-14 16:21:46.515115 gptwrite-0.1.2/gptwrite/main.py
+-rw-r--r--   0        0        0     2642 2023-04-14 16:52:13.826245 gptwrite-0.1.2/gptwrite/prompts.py
+-rw-r--r--   0        0        0      516 2023-04-14 16:14:00.271931 gptwrite-0.1.2/gptwrite/util.py
+-rw-r--r--   0        0        0      770 2023-04-14 17:03:39.408110 gptwrite-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 gptwrite-0.1.2/PKG-INFO
```

### Comparing `gptwrite-0.1.1/LICENSE` & `gptwrite-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.1/gptwrite/accepted_language.py` & `gptwrite-0.1.2/gptwrite/accepted_language.py`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.1/gptwrite/core.py` & `gptwrite-0.1.2/gptwrite/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,59 @@
 import re
 import logging
+from typing import List, Callable, Optional, Dict
 import i18n
 import openai
 import questionary
 from gptwrite.prompts import build_prompt_generate_topics, build_prompt_generate_texts, build_prompt_rewrite_texts
 
 
+GenerateFunc = Callable[[str, List[str], Optional[str], str, str], str]
+OpenAIMessages = List[Dict[str, str]]
+
 ACTIONS = ["Thought", "Consult", "Write"]
 
 logger = logging.getLogger(__name__)
 
 
-def select_topics(topics, lang_for_description):
+def generate_text_by_llm(
+        messages: OpenAIMessages,
+        model_name: str = "gpt-3.5-turbo",
+        stop: Optional[str] = None
+    ) -> str:
+    response = openai.ChatCompletion.create(
+        model=model_name,
+        messages=messages,
+        stop=stop)
+    content = response.choices[0].message.content
+    return content
+
+def select_topics(
+        topics: List[str],
+        lang_for_description: str,
+    ) -> List[str]:
     selected_topics = questionary.checkbox(
         i18n.t("messages.want_topic", locale=lang_for_description),
         choices=topics).unsafe_ask()
     return selected_topics
 
-def generate_topics(theme, lang_for_generating, nuance=None):
+def generate_topics(
+        theme: str,
+        lang_for_generating: str,
+        nuance: Optional[str] = None,
+        generate_text_func: GenerateFunc = generate_text_by_llm,
+    ) -> List[str]:
     messages = [{
         "role": "user",
         "content": build_prompt_generate_topics(theme, lang_for_generating, nuance)
     }]
-    response = openai.ChatCompletion.create(
-            model="gpt-3.5-turbo",
-            messages=messages)
-    content = response.choices[0].message.content
+    content = generate_text_func(messages=messages)
     return put_generated_text_into_list(content)
 
-def put_generated_text_into_list(text):
+def put_generated_text_into_list(text: str) -> List[str]:
     topics = []
     for line in text.split("\n"):
         if line.startswith("- "):
             topics.append(line[2:].strip())
             continue
         if line.startswith("・ "):
             topics.append(line[2:].strip())
@@ -42,28 +63,31 @@
             continue
         num_list_match = re.search(r"^(\d+)\. ", line)
         if num_list_match:
             topics.append(line[len(num_list_match.groups()[0]):].strip())
             continue
     return topics
 
-def generate_texts(theme, topics, nuance, lang_for_generating, lang_for_description):
+def generate_texts(
+        theme: str,
+        topics: List[str],
+        nuance: Optional[str],
+        lang_for_generating: str,
+        lang_for_description: str,
+        generate_text_func: GenerateFunc  = generate_text_by_llm,
+    ) -> str:
     messages = [{
         "role": "user",
         "content": build_prompt_generate_texts(theme, topics, nuance, lang_for_generating)
     }]
 
     writes = []
 
     while True:
-        response = openai.ChatCompletion.create(
-                model="gpt-3.5-turbo",
-                messages=messages,
-                stop="\n\n")
-        content = response.choices[0].message.content
+        content = generate_text_func(messages=messages, stop="\n\n")
         print(content)
 
         if content.startswith("[Consult]"):
             comprementary = questionary.text(i18n.t("messages.want_complementary", locale=lang_for_description)).unsafe_ask()
             messages.append({
                 "role": "user",
                 "content": f"[Complement]{comprementary}"
@@ -85,19 +109,30 @@
                 "role": "assistant",
                 "content": f"[Request]{i18n.t('messages.want_more', locale=lang_for_description)}"
             }) 
             continue
 
         messages.append({"role": "system", "content": i18n.t("messages.", locale=lang_for_description)})
 
-    return rewrite_texts(writes, lang_for_generating)
+    return rewrite_texts(writes, lang_for_generating, lang_for_description, generate_text_func)
 
-def rewrite_texts(sentences, lang_for_generating):
+def rewrite_texts(
+        sentences: List[str],
+        lang_for_generating: str,
+        lang_for_description: str,
+        generate_text_func: GenerateFunc = generate_text_by_llm,
+    ) -> str:
+    print(i18n.t("messages.rewrite", locale=lang_for_description))
     messages = [{
         "role": "user",
         "content": build_prompt_rewrite_texts(sentences, lang_for_generating)
     }]
-    response = openai.ChatCompletion.create(
-            model="gpt-3.5-turbo",
-            messages=messages)
-    content = response.choices[0].message.content
-    return content
+
+    result_texts = ""
+    while True:
+        content = generate_text_func(messages)
+        print(content)
+        result_texts += content
+        if not questionary.confirm(i18n.t("messages.want_more", locale=lang_for_description)).unsafe_ask():
+            break
+        messages.append({"role": "user", "content": f"[Request]{i18n.t('messages.want_more', locale=lang_for_description)}"})
+    return result_texts
```

### Comparing `gptwrite-0.1.1/gptwrite/locales/messages.en.yaml` & `gptwrite-0.1.2/gptwrite/locales/messages.en.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -8,9 +8,10 @@
   want_paragraph_topic: Which topic will you write the content from this time?
   want_complementary: Please give additional information that GPT wants.
   include_action: Be sure to prefix the word Thought, Consult, or Write with the prefix [<Action>].
   accept_text: This paragraph was generated. How do you like it?
   remove_topics: Do you want to write anymore about your selected topic?
   confirm_want_more: Want me to write more? 
   want_more: Please continue.
+  rewrite: Rewrite the generated text to make it more readable.
   save: Want to save generated paragraphs into file?
   no_api_key: Please set OPENAI_API_KEY environment variable.
```

### Comparing `gptwrite-0.1.1/gptwrite/locales/messages.ja.yaml` & `gptwrite-0.1.2/gptwrite/locales/messages.ja.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -8,9 +8,10 @@
   want_paragraph_topic: 今回はどのトピックから内容を書きますか？
   want_complementary: GPTが欲しがってる追加の情報をあげてください。
   include_action: 必ず言葉の先頭にThought, Consult, Writeのいずれかを [<Action>] というprefixとしてつけてください。
   accept_text: こんなパラグラフが生成されました。いかがでしょうか？
   remove_topics: 選択したトピックについてはもう書きませんか？
   confirm_want_more: もっと書いて欲しいですか？
   want_more: 続きを書いてください。
+  rewrite: 生成された文章を読みやすいように書き直します。
   save: 生成された文章をファイルに保存しますか？
   no_api_key: OPENAI_API_KEYを環境変数にセットしてください。
```

### Comparing `gptwrite-0.1.1/gptwrite/main.py` & `gptwrite-0.1.2/gptwrite/main.py`

 * *Files identical despite different names*

### Comparing `gptwrite-0.1.1/gptwrite/prompts.py` & `gptwrite-0.1.2/gptwrite/prompts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+from typing import List, Optional
+
+
 # Topic Prompts
 
-def build_prompt_generate_topics(theme, language, nuance=None):
+def build_prompt_generate_topics(
+        theme: str,
+        language: str,
+        nuance: Optional[str] = None
+    ):
     prompt = GENERATE_TOPICS_PROMPT_PREFIX.format(theme=theme, language=language)
     if nuance:
         prompt += GENERATE_TOPICS_PROMPT_NUANCE.format(nuance=nuance)
     prompt += GENERATE_TOPICS_PROMPT_SUFFIX.format(language=language)
     return prompt
 
 GENERATE_TOPICS_PROMPT_PREFIX = """# Instruction
@@ -33,15 +40,20 @@
 # System Output (Topics)
 <Your outputs>"""
 
 
 
 # Text Generating Prompts
 
-def build_prompt_generate_texts(theme, topics, nuance, language):
+def build_prompt_generate_texts(
+        theme: str,
+        nuance: str,
+        language: str,
+        topics: List[str],
+    ):
     return GENERATE_TEXT_PROMPT.format(
         theme=theme,
         topics="\n".join(["- " + topic for topic in topics]),
         nuance=nuance,
         language=language)
 
 GENERATE_TEXT_PROMPT = """# Instruction
@@ -71,15 +83,15 @@
 - Please include the action in your answer.
 - Please write the action in square brackets.
 - Please must be sure to reply using {language}!"""
 
 
 # Text Rewriting Prompts
 
-def build_prompt_rewrite_texts(sentences, language):
+def build_prompt_rewrite_texts(sentences: List[str], language: str):
     return REWRITING_TEXT_PROMPT.format(
         sentences="\n".join(["- " + sentence for sentence in sentences]),
         language=language)
 
 REWRITING_TEXT_PROMPT = """# Instruction
 Please Write good paragraphs, piecing together the following sentences given.
```

### Comparing `gptwrite-0.1.1/pyproject.toml` & `gptwrite-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gptwrite"
-version = "0.1.1"
+version = "0.1.2"
 description = "CLI for Automated article writing"
 authors = ["otakumesi <bakednt@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/otakumesi/gpt-write"
 repository = "https://github.com/otakumesi/gpt-write"
 readme = "README.md"
 keywords = ["gpt", "openai", "cli", "article", "writing"]
```

### Comparing `gptwrite-0.1.1/PKG-INFO` & `gptwrite-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptwrite
-Version: 0.1.1
+Version: 0.1.2
 Summary: CLI for Automated article writing
 Home-page: https://github.com/otakumesi/gpt-write
 License: MIT
 Keywords: gpt,openai,cli,article,writing
 Author: otakumesi
 Author-email: bakednt@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -18,31 +18,36 @@
 Requires-Dist: iso639-lang
 Requires-Dist: openai
 Requires-Dist: python-i18n[yaml]
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Project-URL: Repository, https://github.com/otakumesi/gpt-write
 Description-Content-Type: text/markdown
 
-# GPT-Write✍️
+# GPT-Write :writing_hand:
+
+__GPT make writing an article brazing fast :fire:.__
+
+PyPi:
+- https://pypi.org/project/gptwrite/
 
-GPT make writing an article brazing fast🔥.  
 ![GPT-Write Demo](https://github.com/otakumesi/gpt-write/blob/main/demo.gif?raw=true "デモ")
 
-## What's this tool?
+## :telescope: Overview
+- GPT-Write is the CLI tool for Intractive Automated Article Writing.  
+- You can create articles, just answer the questions.   
+- Since the language is specified in the GPT prompt and GPT is allowed to generate the text, it could theoretically be used in a variety of languages.  
+    - However, the supported languages in the shell messages are only English and Japanese.
 
-GPT-Write is the CLI tool for Intractive Automated Article Writing.  
-You can create articles, just answer the questions.   
-Since the language is specified in the prompt and GPT is allowed to generate the text, it could theoretically be used in a variety of languages.  
 
-## Installation
+## :runner: Installation
 ```sh
 pip install gptwrite
 ```
 
-## Usage
+## :computer: Usage
 
 ```sh
 # Set Environment "OPENAI_API_KEY"
 export OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxx
 
 # Run
 gptwrite
```

