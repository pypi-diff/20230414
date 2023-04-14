# Comparing `tmp/arlq-1.0.1.tar.gz` & `tmp/arlq-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arlq-1.0.1.tar", last modified: Fri Apr 14 17:24:26 2023, max compression
+gzip compressed data, was "arlq-1.0.2.tar", last modified: Fri Apr 14 18:06:10 2023, max compression
```

## Comparing `arlq-1.0.1.tar` & `arlq-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 17:24:26.240857 arlq-1.0.1/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-13 14:12:27.000000 arlq-1.0.1/LICENSE
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-14 17:24:26.240857 arlq-1.0.1/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4216 2023-04-14 17:16:04.000000 arlq-1.0.1/README.md
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 17:24:26.240857 arlq-1.0.1/arlq/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 17:09:07.000000 arlq-1.0.1/arlq/__init__.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-14 17:17:51.000000 arlq-1.0.1/arlq/_version.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    17399 2023-04-14 17:09:07.000000 arlq-1.0.1/arlq/arlq.py
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 17:24:26.240857 arlq-1.0.1/arlq.egg-info/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-14 17:24:26.000000 arlq-1.0.1/arlq.egg-info/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-14 17:24:26.000000 arlq-1.0.1/arlq.egg-info/SOURCES.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-14 17:24:26.000000 arlq-1.0.1/arlq.egg-info/dependency_links.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-14 17:24:26.000000 arlq-1.0.1/arlq.egg-info/entry_points.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-14 17:24:26.000000 arlq-1.0.1/arlq.egg-info/requires.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-14 17:24:26.000000 arlq-1.0.1/arlq.egg-info/top_level.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      836 2023-04-14 17:24:26.240857 arlq-1.0.1/setup.cfg
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 17:09:07.000000 arlq-1.0.1/setup.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 18:06:10.966935 arlq-1.0.2/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-14 17:26:18.000000 arlq-1.0.2/LICENSE
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-14 18:06:10.966935 arlq-1.0.2/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4216 2023-04-14 17:16:04.000000 arlq-1.0.2/README.md
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 18:06:10.966935 arlq-1.0.2/arlq/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 17:26:18.000000 arlq-1.0.2/arlq/__init__.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-14 18:05:06.000000 arlq-1.0.2/arlq/_version.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    17399 2023-04-14 18:00:27.000000 arlq-1.0.2/arlq/arlq.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 18:06:10.966935 arlq-1.0.2/arlq.egg-info/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-14 18:06:10.000000 arlq-1.0.2/arlq.egg-info/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-14 18:06:10.000000 arlq-1.0.2/arlq.egg-info/SOURCES.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-14 18:06:10.000000 arlq-1.0.2/arlq.egg-info/dependency_links.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-14 18:06:10.000000 arlq-1.0.2/arlq.egg-info/entry_points.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-14 18:06:10.000000 arlq-1.0.2/arlq.egg-info/requires.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-14 18:06:10.000000 arlq-1.0.2/arlq.egg-info/top_level.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      836 2023-04-14 18:06:10.966935 arlq-1.0.2/setup.cfg
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 17:26:18.000000 arlq-1.0.2/setup.py
```

### Comparing `arlq-1.0.1/LICENSE` & `arlq-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arlq-1.0.1/PKG-INFO` & `arlq-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlq
-Version: 1.0.1
+Version: 1.0.2
 Summary: ARQL, another rogue-like quest game.
 Home-page: https://github.com/tos-kamiya/arlq
 Author: Toshihiro Kamiya
 Author-email: kamiya@mbj.nifty.com
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arlq-1.0.1/README.md` & `arlq-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `arlq-1.0.1/arlq/arlq.py` & `arlq-1.0.2/arlq/arlq.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,19 +167,19 @@
     MonsterKind('A', 1, FOOD_AMOEBA, item=ITEM_SPECIAL_EXP),  # Amoeba rare
     MonsterKind('B', 3, FOOD_SPECIAL_BISON, item=ITEM_SPECIAL_BISON_MEAT),  # Bison rare
     MonsterKind('C', 6, FOOD_CHIMERA, item=ITEM_SWORD_AND_CLAIRVOYANCE),  # Chimera rare
 ]
 
 MONSTER_KIND_POPULATION: Dict[str, int] = {
     'a': 20,
-    'b': 5,
-    'c': 5,
+    'b': 4,
+    'c': 4,
     'd': 4,
     'D': 1,
-    'E': 3,
+    'E': 2,
     'f': 1,
 }
 
 
 def find_random_place(objects: List[Entity], field: List[List[str]], distance: int) -> Point:
     places = [(o.x, o.y) for o in objects]
     while True:
```

### Comparing `arlq-1.0.1/arlq.egg-info/PKG-INFO` & `arlq-1.0.2/arlq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlq
-Version: 1.0.1
+Version: 1.0.2
 Summary: ARQL, another rogue-like quest game.
 Home-page: https://github.com/tos-kamiya/arlq
 Author: Toshihiro Kamiya
 Author-email: kamiya@mbj.nifty.com
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arlq-1.0.1/setup.cfg` & `arlq-1.0.2/setup.cfg`

 * *Files identical despite different names*

