# Comparing `tmp/datedays-2.2.3.tar.gz` & `tmp/datedays-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datedays-2.2.3.tar", last modified: Thu Apr 13 06:24:19 2023, max compression
+gzip compressed data, was "datedays-2.2.4.tar", last modified: Fri Apr 14 03:36:14 2023, max compression
```

## Comparing `datedays-2.2.3.tar` & `datedays-2.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:24:19.727114 datedays-2.2.3/
--rw-rw-rw-   0        0        0     1086 2022-08-05 07:39:04.000000 datedays-2.2.3/LICENSE
--rw-rw-rw-   0        0        0     6413 2023-04-13 06:24:19.725119 datedays-2.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     5883 2023-04-13 05:52:35.000000 datedays-2.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 06:24:19.685855 datedays-2.2.3/datedays/
--rw-rw-rw-   0        0        0      847 2023-04-13 05:57:23.000000 datedays-2.2.3/datedays/__init__.py
--rw-rw-rw-   0        0        0    14571 2023-04-13 06:24:01.000000 datedays-2.2.3/datedays/datedays.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:24:19.723124 datedays-2.2.3/datedays.egg-info/
--rw-rw-rw-   0        0        0     6413 2023-04-13 06:24:19.000000 datedays-2.2.3/datedays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-13 06:24:19.000000 datedays-2.2.3/datedays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:24:19.000000 datedays-2.2.3/datedays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-04-13 06:24:19.000000 datedays-2.2.3/datedays.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 06:24:19.000000 datedays-2.2.3/datedays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 06:24:19.728111 datedays-2.2.3/setup.cfg
--rw-rw-rw-   0        0        0      753 2023-04-13 05:55:43.000000 datedays-2.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:36:14.198565 datedays-2.2.4/
+-rw-rw-rw-   0        0        0     1086 2022-08-05 07:39:04.000000 datedays-2.2.4/LICENSE
+-rw-rw-rw-   0        0        0     6411 2023-04-14 03:36:14.195576 datedays-2.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5882 2023-04-14 03:36:04.000000 datedays-2.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 03:36:14.185600 datedays-2.2.4/datedays/
+-rw-rw-rw-   0        0        0      847 2023-04-13 05:57:23.000000 datedays-2.2.4/datedays/__init__.py
+-rw-rw-rw-   0        0        0    14686 2023-04-14 03:36:05.000000 datedays-2.2.4/datedays/datedays.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:36:14.194595 datedays-2.2.4/datedays.egg-info/
+-rw-rw-rw-   0        0        0     6411 2023-04-14 03:36:13.000000 datedays-2.2.4/datedays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-14 03:36:14.000000 datedays-2.2.4/datedays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 03:36:13.000000 datedays-2.2.4/datedays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-04-14 03:36:13.000000 datedays-2.2.4/datedays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 03:36:13.000000 datedays-2.2.4/datedays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 03:36:14.198565 datedays-2.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      753 2023-04-14 03:36:12.000000 datedays-2.2.4/setup.py
```

### Comparing `datedays-2.2.3/LICENSE` & `datedays-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datedays-2.2.3/PKG-INFO` & `datedays-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: datedays
-Version: 2.2.3
+Version: 2.2.4
 Summary: Python Date Tools
 Home-page: https://github.com/liang1024/datedays
 Author: liang1024
 Author-email: chinalzge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # datedays
 
+
 ## What can it do?
 
 * [1. Get common date data](#datadays)
 * [2. Operating excel report](#excel)
 * [3. Perform common encryption signature](#hash)
 * [4. Obtain the encrypted signature of the file](#file)
 * [5. Other](#other)
@@ -58,16 +59,14 @@
 ------------------------------
 yesterday: 2022-08-18
 the day before yesterday: 2022-08-17
 180 days ago: 2022-02-20
 1000 days ago: 2019-11-23
 ```
 
-
-
 ### Still updating
 
 ## 1. Get common date data
 
 Method | description | return result | parameter<a id = "datadays"></a>
 :---: | :---:| :---:| :---:
 getnow() | get today's date | for example: 2022-08-16 17:56:17|
```

### Comparing `datedays-2.2.3/README.md` & `datedays-2.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # datedays
 
+
 ## What can it do?
 
 * [1. Get common date data](#datadays)
 * [2. Operating excel report](#excel)
 * [3. Perform common encryption signature](#hash)
 * [4. Obtain the encrypted signature of the file](#file)
 * [5. Other](#other)
@@ -45,16 +46,14 @@
 ------------------------------
 yesterday: 2022-08-18
 the day before yesterday: 2022-08-17
 180 days ago: 2022-02-20
 1000 days ago: 2019-11-23
 ```
 
-
-
 ### Still updating
 
 ## 1. Get common date data
 
 Method | description | return result | parameter<a id = "datadays"></a>
 :---: | :---:| :---:| :---:
 getnow() | get today's date | for example: 2022-08-16 17:56:17|
```

### Comparing `datedays-2.2.3/datedays/__init__.py` & `datedays-2.2.4/datedays/__init__.py`

 * *Files identical despite different names*

### Comparing `datedays-2.2.3/datedays/datedays.py` & `datedays-2.2.4/datedays/datedays.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,47 +587,47 @@
 
 
 def logger(txt=None, base_name=None, file_name='log.txt', log_base=None,
            fmt=f'%(asctime)s - %(name)s - %(levelname)s - %(message)s',
            mode='a',
            encoding='utf-8'):
     '''logger'''
+    logger = logging.getLogger(base_name)
 
-    if not base_name:
-        base_name = os.path.basename(sys.argv[0]).split('.')[0]
+    if not logger.handlers:
+        if not base_name:
+            base_name = os.path.basename(sys.argv[0]).split('.')[0]
 
-    if not log_base:
-        arg = sys.argv[0]
-        log_base = arg[:arg.rfind('/')]
-        # log_base = arg[:arg[:arg.rfind('/')].rfind('/')]
-
-    date_dir = f"{log_base}/log/{base_name}/{datetime.date.today().strftime('%Y-%m-%d')}"
-
-    if not os.path.exists(date_dir):
-        print(f'logger create dir:{date_dir}')
-        os.makedirs(date_dir)
+        if not log_base:
+            arg = sys.argv[0]
+            log_base = arg[:arg.rfind('/')]
+            # log_base = arg[:arg[:arg.rfind('/')].rfind('/')]
 
-    logger = logging.getLogger(base_name)
+        date_dir = f"{log_base}/log/{base_name}/{datetime.date.today().strftime('%Y-%m-%d')}"
+
+        if not os.path.exists(date_dir):
+            print(f'logger create dir:{date_dir}')
+            os.makedirs(date_dir)
+
+        formatter = logging.Formatter(fmt)
+
+        # filehandler
+        fh = logging.FileHandler(f'{date_dir}/{file_name}', mode=mode, encoding=encoding)
+        fh.setFormatter(formatter)
 
-    formatter = logging.Formatter(fmt)
+        # consolehandler
+        ch = logging.StreamHandler()
+        ch.setFormatter(formatter)
 
-    # filehandler
-    fh = logging.FileHandler(f'{date_dir}/{file_name}', mode=mode, encoding=encoding)
-    fh.setFormatter(formatter)
-
-    # consolehandler
-    ch = logging.StreamHandler()
-    ch.setFormatter(formatter)
-
-    # add handler
-    logger.addHandler(fh)
-    logger.addHandler(ch)
+        # add handler
+        logger.addHandler(fh)
+        logger.addHandler(ch)
 
-    # set level=debug
-    logger.setLevel(logging.DEBUG)
+        # set level=debug
+        logger.setLevel(logging.DEBUG)
 
     if txt:
         logger.debug(txt)
 
     return logger
```

### Comparing `datedays-2.2.3/datedays.egg-info/PKG-INFO` & `datedays-2.2.4/datedays.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: datedays
-Version: 2.2.3
+Version: 2.2.4
 Summary: Python Date Tools
 Home-page: https://github.com/liang1024/datedays
 Author: liang1024
 Author-email: chinalzge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # datedays
 
+
 ## What can it do?
 
 * [1. Get common date data](#datadays)
 * [2. Operating excel report](#excel)
 * [3. Perform common encryption signature](#hash)
 * [4. Obtain the encrypted signature of the file](#file)
 * [5. Other](#other)
@@ -58,16 +59,14 @@
 ------------------------------
 yesterday: 2022-08-18
 the day before yesterday: 2022-08-17
 180 days ago: 2022-02-20
 1000 days ago: 2019-11-23
 ```
 
-
-
 ### Still updating
 
 ## 1. Get common date data
 
 Method | description | return result | parameter<a id = "datadays"></a>
 :---: | :---:| :---:| :---:
 getnow() | get today's date | for example: 2022-08-16 17:56:17|
```

### Comparing `datedays-2.2.3/setup.py` & `datedays-2.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "python-dateutil>=2.8.2",
 ]
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="datedays",
-    version="2.2.3",
+    version="2.2.4",
     author="liang1024",
     author_email="chinalzge@gmail.com",
     description="Python Date Tools",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/liang1024/datedays",
     packages=setuptools.find_packages(),
```

