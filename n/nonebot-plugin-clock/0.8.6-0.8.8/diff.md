# Comparing `tmp/nonebot-plugin-clock-0.8.6.tar.gz` & `tmp/nonebot-plugin-clock-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nonebot-plugin-clock-0.8.6.tar", last modified: Thu Apr 13 09:32:33 2023, max compression
+gzip compressed data, was "dist/nonebot-plugin-clock-0.8.8.tar", last modified: Fri Apr 14 05:16:16 2023, max compression
```

## Comparing `nonebot-plugin-clock-0.8.6.tar` & `nonebot-plugin-clock-0.8.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 09:32:33.000000 nonebot-plugin-clock-0.8.6/
--rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.6/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8.6/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 09:32:33.000000 nonebot-plugin-clock-0.8.6/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1462 2023-04-13 03:19:28.000000 nonebot-plugin-clock-0.8.6/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 09:32:33.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/
--rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/Clock.py
--rw-r--r--   0 mac        (501) staff       (20)     6182 2023-04-13 09:30:23.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1956 2023-04-13 04:01:40.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/database.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-13 09:32:33.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-13 09:32:32.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-13 09:32:32.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-13 09:32:32.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-13 09:32:32.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-13 09:32:32.000000 nonebot-plugin-clock-0.8.6/nonebot_plugin_clock.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.6/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-13 09:32:33.000000 nonebot-plugin-clock-0.8.6/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-13 09:30:52.000000 nonebot-plugin-clock-0.8.6/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/
+-rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.8/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8.8/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1462 2023-04-13 03:19:28.000000 nonebot-plugin-clock-0.8.8/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/
+-rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/Clock.py
+-rw-r--r--   0 mac        (501) staff       (20)     6182 2023-04-13 09:30:23.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1972 2023-04-14 05:16:05.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/database.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.8/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-14 05:15:40.000000 nonebot-plugin-clock-0.8.8/setup.py
```

### Comparing `nonebot-plugin-clock-0.8.6/LICENSE` & `nonebot-plugin-clock-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.6/README.md` & `nonebot-plugin-clock-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/Clock.py` & `nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/Clock.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/__init__.py` & `nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.6/nonebot_plugin_clock/database.py` & `nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         res = list(res)
         conn.commit()
         conn.close()
         return res
 
 
     def add_clock(self, clock: Clock):
-        sql = f'''INSERT INTO {self.table} (type, user, content, month, day, week, c_time, ones)
-        values ("{clock.type}", {clock.user}, "{clock.content}","{clock.month}","{clock.day}","{clock.week}","{clock.time}",{clock.ones});'''
+        sql = f'''INSERT INTO {self.table} (id, type, user, content, month, day, week, c_time, ones)
+        values ({clock.id}, "{clock.type}", {clock.user}, "{clock.content}","{clock.month}","{clock.day}","{clock.week}","{clock.time}",{clock.ones});'''
         self.execute(sql)
 
     def del_clock(self, id: int, user: int):
         if self.execute(f"SELECT id FROM {self.table} where id = {id} and user = {user}"):
             self.execute(f"DELETE from {self.table} where id = {id}")
             return True
```

### Comparing `nonebot-plugin-clock-0.8.6/setup.py` & `nonebot-plugin-clock-0.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8
 
 from setuptools import setup
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setup(
     name='nonebot-plugin-clock',
-    version='0.8.6',
+    version='0.8.8',
     author='Zeta',
     author_email='',
     long_description="https://github.com/Zeta-qixi/nonebot-plugin-clock",
     license="MIT Licence",
     url='https://github.com/Zeta-qixi/nonebot-plugin-clock/',
     description='nonebot_plugin about clock',
     packages=['nonebot_plugin_clock'],
```

