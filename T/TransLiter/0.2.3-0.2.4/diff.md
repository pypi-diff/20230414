# Comparing `tmp/TransLiter-0.2.3.tar.gz` & `tmp/TransLiter-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TransLiter-0.2.3.tar", last modified: Wed Apr 12 22:12:27 2023, max compression
+gzip compressed data, was "TransLiter-0.2.4.tar", last modified: Fri Apr 14 18:42:38 2023, max compression
```

## Comparing `TransLiter-0.2.3.tar` & `TransLiter-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-12 22:12:27.915787 TransLiter-0.2.3/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1067 2023-04-07 00:09:21.000000 TransLiter-0.2.3/LICENSE
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     4437 2023-04-12 22:12:27.915670 TransLiter-0.2.3/PKG-INFO
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     4087 2023-04-12 22:10:54.000000 TransLiter-0.2.3/README.md
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-12 22:12:27.914813 TransLiter-0.2.3/TransLiter/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      110 2023-04-12 17:26:39.000000 TransLiter-0.2.3/TransLiter/__init__.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     3374 2023-04-12 19:11:15.000000 TransLiter-0.2.3/TransLiter/jp_list.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1116 2023-04-12 00:32:24.000000 TransLiter-0.2.3/TransLiter/ko_jamo.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      370 2023-04-12 17:31:03.000000 TransLiter-0.2.3/TransLiter/spacing.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     2060 2023-04-12 19:28:12.000000 TransLiter-0.2.3/TransLiter/transliter_jp.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     2360 2023-04-12 19:11:14.000000 TransLiter-0.2.3/TransLiter/transliter_ko.py
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-12 22:12:27.915500 TransLiter-0.2.3/TransLiter.egg-info/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     4437 2023-04-12 22:12:27.000000 TransLiter-0.2.3/TransLiter.egg-info/PKG-INFO
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      373 2023-04-12 22:12:27.000000 TransLiter-0.2.3/TransLiter.egg-info/SOURCES.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-04-12 22:12:27.000000 TransLiter-0.2.3/TransLiter.egg-info/dependency_links.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-04-12 22:12:27.000000 TransLiter-0.2.3/TransLiter.egg-info/not-zip-safe
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       16 2023-04-12 22:12:27.000000 TransLiter-0.2.3/TransLiter.egg-info/requires.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       11 2023-04-12 22:12:27.000000 TransLiter-0.2.3/TransLiter.egg-info/top_level.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       38 2023-04-12 22:12:27.915832 TransLiter-0.2.3/setup.cfg
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      647 2023-04-12 22:11:18.000000 TransLiter-0.2.3/setup.py
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-14 18:42:38.866818 TransLiter-0.2.4/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     1067 2023-04-07 00:09:21.000000 TransLiter-0.2.4/LICENSE
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     4438 2023-04-14 18:42:38.866702 TransLiter-0.2.4/PKG-INFO
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     4088 2023-04-13 18:14:28.000000 TransLiter-0.2.4/README.md
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-14 18:42:38.865837 TransLiter-0.2.4/TransLiter/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      110 2023-04-12 17:26:39.000000 TransLiter-0.2.4/TransLiter/__init__.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     3374 2023-04-12 19:11:15.000000 TransLiter-0.2.4/TransLiter/jp_list.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     1116 2023-04-12 00:32:24.000000 TransLiter-0.2.4/TransLiter/ko_jamo.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      370 2023-04-12 17:31:03.000000 TransLiter-0.2.4/TransLiter/spacing.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     2082 2023-04-14 18:40:59.000000 TransLiter-0.2.4/TransLiter/transliter_jp.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     2382 2023-04-14 18:31:29.000000 TransLiter-0.2.4/TransLiter/transliter_ko.py
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-14 18:42:38.866510 TransLiter-0.2.4/TransLiter.egg-info/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     4438 2023-04-14 18:42:38.000000 TransLiter-0.2.4/TransLiter.egg-info/PKG-INFO
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      373 2023-04-14 18:42:38.000000 TransLiter-0.2.4/TransLiter.egg-info/SOURCES.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-04-14 18:42:38.000000 TransLiter-0.2.4/TransLiter.egg-info/dependency_links.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-04-14 18:42:38.000000 TransLiter-0.2.4/TransLiter.egg-info/not-zip-safe
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       16 2023-04-14 18:42:38.000000 TransLiter-0.2.4/TransLiter.egg-info/requires.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       11 2023-04-14 18:42:38.000000 TransLiter-0.2.4/TransLiter.egg-info/top_level.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       38 2023-04-14 18:42:38.866855 TransLiter-0.2.4/setup.cfg
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      647 2023-04-14 04:08:10.000000 TransLiter-0.2.4/setup.py
```

### Comparing `TransLiter-0.2.3/LICENSE` & `TransLiter-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TransLiter-0.2.3/PKG-INFO` & `TransLiter-0.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TransLiter
-Version: 0.2.3
+Version: 0.2.4
 Summary: TransLiter transliterates multilingual text into English.
 Home-page: https://github.com/elibooklover/TransLiter
 Author: Hoyeol Kim
 Author-email: elibooklover@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -37,15 +37,15 @@
 $ Python
 
 > import TransLiter as tl
 ```
 
 ## 1. Korean
 
-### 1-1. Simpe functions.
+### 1-1. Simple functions.
 
 ```
 > tl.ko("안녕하세요. 날씨가 좋네요!")
 annyeohaseyo. narssiga johneyo!
 ```
 
 If you want to use the transliteration function several times in a row:
```

### Comparing `TransLiter-0.2.3/README.md` & `TransLiter-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 $ Python
 
 > import TransLiter as tl
 ```
 
 ## 1. Korean
 
-### 1-1. Simpe functions.
+### 1-1. Simple functions.
 
 ```
 > tl.ko("안녕하세요. 날씨가 좋네요!")
 annyeohaseyo. narssiga johneyo!
 ```
 
 If you want to use the transliteration function several times in a row:
```

### Comparing `TransLiter-0.2.3/TransLiter/jp_list.py` & `TransLiter-0.2.4/TransLiter/jp_list.py`

 * *Files identical despite different names*

### Comparing `TransLiter-0.2.3/TransLiter/ko_jamo.py` & `TransLiter-0.2.4/TransLiter/ko_jamo.py`

 * *Files identical despite different names*

### Comparing `TransLiter-0.2.3/TransLiter/transliter_jp.py` & `TransLiter-0.2.4/TransLiter/transliter_jp.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,10 +64,10 @@
     for sentence in lines:
         st = sentence.strip()
         tr = jp(st)
         sentence_list.append(st)
         transliter_list.append(tr)
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
-    data.to_csv("output_jp.csv")
+    data.to_csv("output_jp.csv", encoding="utf-8-sig")
     print(data)
     f.close()
```

### Comparing `TransLiter-0.2.3/TransLiter/transliter_ko.py` & `TransLiter-0.2.4/TransLiter/transliter_ko.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,10 +68,10 @@
     for sentence in lines:
         st = sentence.strip()
         tr = ko(st)
         sentence_list.append(st)
         transliter_list.append(tr)
 
     data = pd.DataFrame({'Original Text': sentence_list, 'Transliterated Text': transliter_list}, index=index_list)
-    data.to_csv("output_ko.csv")
+    data.to_csv("output_ko.csv", encoding="utf-8-sig")
     print(data)
     f.close()
```

### Comparing `TransLiter-0.2.3/TransLiter.egg-info/PKG-INFO` & `TransLiter-0.2.4/TransLiter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TransLiter
-Version: 0.2.3
+Version: 0.2.4
 Summary: TransLiter transliterates multilingual text into English.
 Home-page: https://github.com/elibooklover/TransLiter
 Author: Hoyeol Kim
 Author-email: elibooklover@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -37,15 +37,15 @@
 $ Python
 
 > import TransLiter as tl
 ```
 
 ## 1. Korean
 
-### 1-1. Simpe functions.
+### 1-1. Simple functions.
 
 ```
 > tl.ko("안녕하세요. 날씨가 좋네요!")
 annyeohaseyo. narssiga johneyo!
 ```
 
 If you want to use the transliteration function several times in a row:
```

### Comparing `TransLiter-0.2.3/setup.py` & `TransLiter-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='TransLiter',
     python_requires='>=3.6',
-    version='0.2.3',
+    version='0.2.4',
     url='https://github.com/elibooklover/TransLiter',
     license='MIT',
     author='Hoyeol Kim',
     author_email='elibooklover@gmail.com',
     description='TransLiter transliterates multilingual text into English.',
     packages=['TransLiter', ],
     long_description=long_description,
```

