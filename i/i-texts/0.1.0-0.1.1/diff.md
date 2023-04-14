# Comparing `tmp/i-texts-0.1.0.tar.gz` & `tmp/i-texts-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i-texts-0.1.0.tar", last modified: Fri Apr 14 18:34:23 2023, max compression
+gzip compressed data, was "i-texts-0.1.1.tar", last modified: Fri Apr 14 18:55:54 2023, max compression
```

## Comparing `i-texts-0.1.0.tar` & `i-texts-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       48 2023-04-14 17:47:10.481893 i-texts-0.1.0/i_texts/__init__.py
--rw-r--r--   0        0        0      693 2023-04-14 18:15:43.123566 i-texts-0.1.0/i_texts/core.py
--rw-r--r--   0        0        0      169 2023-04-14 18:21:43.478803 i-texts-0.1.0/i_texts/main.py
--rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 i-texts-0.1.0/i_texts/py.typed
--rw-r--r--   0        0        0      491 2023-04-14 18:04:02.840505 i-texts-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      410 2023-04-14 18:33:24.697451 i-texts-0.1.0/README.md
--rw-r--r--   0        0        0      190 2023-04-14 18:18:14.845213 i-texts-0.1.0/tests/__main__.py
--rw-r--r--   0        0        0       24 2023-04-14 18:17:18.897658 i-texts-0.1.0/tests/locales/ru.yml
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 i-texts-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-04-14 17:47:10.481893 i-texts-0.1.1/i_texts/__init__.py
+-rw-r--r--   0        0        0      710 2023-04-14 18:54:17.413781 i-texts-0.1.1/i_texts/core.py
+-rw-r--r--   0        0        0      169 2023-04-14 18:21:43.478803 i-texts-0.1.1/i_texts/main.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 i-texts-0.1.1/i_texts/py.typed
+-rw-r--r--   0        0        0      491 2023-04-14 18:55:13.631243 i-texts-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      434 2023-04-14 18:55:44.354629 i-texts-0.1.1/README.md
+-rw-r--r--   0        0        0      214 2023-04-14 18:54:29.966911 i-texts-0.1.1/tests/__main__.py
+-rw-r--r--   0        0        0       48 2023-04-14 18:53:06.818508 i-texts-0.1.1/tests/locales/ru.yml
+-rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 i-texts-0.1.1/PKG-INFO
```

### Comparing `i-texts-0.1.0/i_texts/core.py` & `i-texts-0.1.1/i_texts/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import yaml
 
 Key = int | str
 
 
 class Texts:
     def __init__(self, path: str) -> None:
-        with open(path) as stream:
+        with open(path, encoding="utf8") as stream:
             raw_dict: dict = yaml.unsafe_load(stream)
         self.dict = {k: str(v) for k, v in raw_dict.items()}
 
     def get_words(self, key: Key) -> list[str]:
         text = self[key]
         return text.split()
```

### Comparing `i-texts-0.1.0/PKG-INFO` & `i-texts-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i-texts
-Version: 0.1.0
+Version: 0.1.1
 License: MIT
 Author-email: levch <levchenko.d.a1998@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # I18n texts loader
 
@@ -14,13 +14,13 @@
 - Loads texts from "{`LOCALES_PATH`}/{`LOCALE`}.yml"
 
 ## Example
 
 ```py
 from i_texts import texts
 
-assert texts.dict == {1: "1", "a": "a", "words": "a b c"}
+assert texts.dict == {1: "1", "a": "a", "words": "a b c", "ru": "русский"}
 assert texts[1] == "1"
 assert texts["a"] == "a"
 assert texts.get_words("words") == ["a", "b", "c"]
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

