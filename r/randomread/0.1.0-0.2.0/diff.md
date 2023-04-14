# Comparing `tmp/randomread-0.1.0.tar.gz` & `tmp/randomread-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randomread-0.1.0.tar", max compression
+gzip compressed data, was "randomread-0.2.0.tar", max compression
```

## Comparing `randomread-0.1.0.tar` & `randomread-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      304 2023-04-14 12:13:46.367022 randomread-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-14 12:19:36.689952 randomread-0.1.0/randomread/__init__.py
--rw-r--r--   0        0        0     1697 2023-04-14 12:22:42.500204 randomread-0.1.0/randomread/utils.py
--rw-r--r--   0        0        0      502 2023-04-14 12:31:25.539563 randomread-0.1.0/setup.py
--rw-r--r--   0        0        0      298 2023-04-14 12:31:25.539695 randomread-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      304 2023-04-14 12:50:30.294920 randomread-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       25 2023-04-14 12:50:38.373522 randomread-0.2.0/randomread/__init__.py
+-rw-r--r--   0        0        0     1767 2023-04-14 12:48:07.726733 randomread-0.2.0/randomread/utils.py
+-rw-r--r--   0        0        0      502 2023-04-14 12:51:05.978854 randomread-0.2.0/setup.py
+-rw-r--r--   0        0        0      298 2023-04-14 12:51:05.978997 randomread-0.2.0/PKG-INFO
```

### Comparing `randomread-0.1.0/randomread/utils.py` & `randomread-0.2.0/randomread/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 from pathlib import Path
 import random
 from math import ceil
 
-def sample(path, no_words, chunk_size=50000, word_len_estimate=10):
+def sample(path, no_words, chunk_size=5000, word_len_estimate=10):
     """
     Sample text chunks from a .txt file
 
     
     """
     texts = []
     filepath = Path(path).expanduser()
     file_stats = filepath.stat()
     file_len_bytes = file_stats.st_size
     print(file_len_bytes)
     
-    chunks = ceil(no_words * word_len_estimate / chunk_size)
+    chunks = ceil(no_words / chunk_size)
     print(f"Generate {chunks} chunks")
     
-    chunks = [random.randint(0, file_len_bytes-chunk_size) for _ in range(chunks)]
+    chunks = [random.randint(0, file_len_bytes - chunk_size * word_len_estimate) for _ in range(chunks)]
     chunks = sorted(chunks)
 
     f = filepath.open("rb")    
     for chunk in chunks:
         current_pos = f.tell()
         print(f"Current position in file {current_pos}")
         f.seek(chunk)
         print(f"Go to {chunk}. Current position in file {f.tell()}")
-        current_bytes = f.read(chunk_size)
+        current_bytes = f.read(chunk_size * word_len_estimate)
         current_text = current_bytes.decode("utf-8")
         current_text = current_text.split()
         current_text = current_text[1:]
         current_text = current_text[:-1]
+        current_text = current_text[:chunk_size]
         current_text = " ".join(current_text)
         texts.append(current_text)
     f.close()
     random.shuffle(texts)
     current_no_words = 0
     text = ""
     for t in texts:
```

