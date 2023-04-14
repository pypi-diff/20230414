# Comparing `tmp/defisheye-1.0.2.tar.gz` & `tmp/defisheye-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defisheye-1.0.2.tar", last modified: Fri Apr 14 11:00:10 2023, max compression
+gzip compressed data, was "defisheye-1.0.3.tar", last modified: Fri Apr 14 11:20:35 2023, max compression
```

## Comparing `defisheye-1.0.2.tar` & `defisheye-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 11:00:10.350771 defisheye-1.0.2/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5067 2023-04-14 11:00:10.350771 defisheye-1.0.2/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4774 2023-04-13 12:43:38.000000 defisheye-1.0.2/README.md
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-14 11:00:10.350771 defisheye-1.0.2/setup.cfg
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      707 2023-04-14 10:59:13.000000 defisheye-1.0.2/setup.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 11:00:10.350771 defisheye-1.0.2/src/
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 11:00:10.350771 defisheye-1.0.2/src/defisheye/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      750 2023-04-13 12:40:23.000000 defisheye-1.0.2/src/defisheye/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5198 2023-04-14 10:58:09.000000 defisheye-1.0.2/src/defisheye/defisheye.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 11:00:10.350771 defisheye-1.0.2/src/defisheye.egg-info/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5067 2023-04-14 11:00:10.000000 defisheye-1.0.2/src/defisheye.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      255 2023-04-14 11:00:10.000000 defisheye-1.0.2/src/defisheye.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-14 11:00:10.000000 defisheye-1.0.2/src/defisheye.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       20 2023-04-14 11:00:10.000000 defisheye-1.0.2/src/defisheye.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       10 2023-04-14 11:00:10.000000 defisheye-1.0.2/src/defisheye.egg-info/top_level.txt
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 11:20:35.620569 defisheye-1.0.3/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5067 2023-04-14 11:20:35.620569 defisheye-1.0.3/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     4774 2023-04-13 12:43:38.000000 defisheye-1.0.3/README.md
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-14 11:20:35.620569 defisheye-1.0.3/setup.cfg
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      707 2023-04-14 11:20:14.000000 defisheye-1.0.3/setup.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 11:20:35.620569 defisheye-1.0.3/src/
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 11:20:35.620569 defisheye-1.0.3/src/defisheye/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      750 2023-04-13 12:40:23.000000 defisheye-1.0.3/src/defisheye/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5197 2023-04-14 11:19:59.000000 defisheye-1.0.3/src/defisheye/defisheye.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-14 11:20:35.620569 defisheye-1.0.3/src/defisheye.egg-info/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     5067 2023-04-14 11:20:35.000000 defisheye-1.0.3/src/defisheye.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      255 2023-04-14 11:20:35.000000 defisheye-1.0.3/src/defisheye.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-14 11:20:35.000000 defisheye-1.0.3/src/defisheye.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       20 2023-04-14 11:20:35.000000 defisheye-1.0.3/src/defisheye.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       10 2023-04-14 11:20:35.000000 defisheye-1.0.3/src/defisheye.egg-info/top_level.txt
```

### Comparing `defisheye-1.0.2/PKG-INFO` & `defisheye-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defisheye
-Version: 1.0.2
+Version: 1.0.3
 Summary: Fast defisheye algorithm
 Home-page: https://github.com/duducosmos/defisheye
 Author: Eduardo S. Pereira
 Author-email: pereira.somoza@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `defisheye-1.0.2/README.md` & `defisheye-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `defisheye-1.0.2/setup.py` & `defisheye-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(filename):
     return open(os.path.join(os.path.dirname(__file__), filename)).read()
 
 
 setup(
     name="defisheye",
     license="Apache License 2.0",
-    version='1.0.2',
+    version='1.0.3',
     author='Eduardo S. Pereira',
     author_email='pereira.somoza@gmail.com',
     packages=find_packages("src"),
     package_dir={"": "src"},
     description="Fast defisheye algorithm",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
```

### Comparing `defisheye-1.0.2/src/defisheye/__init__.py` & `defisheye-1.0.3/src/defisheye/__init__.py`

 * *Files identical despite different names*

### Comparing `defisheye-1.0.2/src/defisheye/defisheye.py` & `defisheye-1.0.3/src/defisheye/defisheye.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self._start_att(vkwargs, kwargs)
 
         if type(infile) == str:
             _image = cv2.imread(infile)
         elif type(infile) == ndarray:
             _image = infile
         else:
-            raise ImageError("Image format not recognized")
+            raise Exception("Image format not recognized")
 
         width = _image.shape[1]
         height = _image.shape[0]
         xcenter = width // 2
         ycenter = height // 2
 
         dim = min(width, height)
```

### Comparing `defisheye-1.0.2/src/defisheye.egg-info/PKG-INFO` & `defisheye-1.0.3/src/defisheye.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defisheye
-Version: 1.0.2
+Version: 1.0.3
 Summary: Fast defisheye algorithm
 Home-page: https://github.com/duducosmos/defisheye
 Author: Eduardo S. Pereira
 Author-email: pereira.somoza@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

