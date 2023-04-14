# Comparing `tmp/ultralight-2.0.0.tar.gz` & `tmp/ultralight-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralight-2.0.0.tar", last modified: Mon Apr 10 17:17:27 2023, max compression
+gzip compressed data, was "ultralight-2.1.0.tar", last modified: Fri Apr 14 14:52:20 2023, max compression
```

## Comparing `ultralight-2.0.0.tar` & `ultralight-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-04-10 17:17:27.157510 ultralight-2.0.0/
--rw-r--r--   0 abionics   (501) staff       (20)     1068 2023-01-20 20:49:15.000000 ultralight-2.0.0/LICENSE.txt
--rw-r--r--   0 abionics   (501) staff       (20)     2235 2023-04-10 17:17:27.157574 ultralight-2.0.0/PKG-INFO
--rw-r--r--   0 abionics   (501) staff       (20)     1118 2023-04-06 17:02:58.000000 ultralight-2.0.0/README.md
--rw-r--r--   0 abionics   (501) staff       (20)       79 2023-04-10 17:17:27.157793 ultralight-2.0.0/setup.cfg
--rw-r--r--   0 abionics   (501) staff       (20)     1829 2023-04-05 13:57:36.000000 ultralight-2.0.0/setup.py
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-04-10 17:17:27.156768 ultralight-2.0.0/ultralight/
--rw-r--r--   0 abionics   (501) staff       (20)      166 2023-04-07 13:03:47.000000 ultralight-2.0.0/ultralight/__init__.py
--rw-r--r--   0 abionics   (501) staff       (20)      174 2023-04-06 16:44:43.000000 ultralight-2.0.0/ultralight/exceptions.py
--rw-r--r--   0 abionics   (501) staff       (20)     1514 2023-04-07 13:14:59.000000 ultralight-2.0.0/ultralight/loader.py
--rw-r--r--   0 abionics   (501) staff       (20)      188 2023-04-06 17:02:58.000000 ultralight-2.0.0/ultralight/types.py
--rw-r--r--   0 abionics   (501) staff       (20)     8345 2023-04-07 13:07:42.000000 ultralight-2.0.0/ultralight/ultralight.py
--rw-r--r--   0 abionics   (501) staff       (20)     3225 2023-04-06 16:52:40.000000 ultralight-2.0.0/ultralight/utils.py
-drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-04-10 17:17:27.157419 ultralight-2.0.0/ultralight.egg-info/
--rw-r--r--   0 abionics   (501) staff       (20)     2235 2023-04-10 17:17:27.000000 ultralight-2.0.0/ultralight.egg-info/PKG-INFO
--rw-r--r--   0 abionics   (501) staff       (20)      376 2023-04-10 17:17:27.000000 ultralight-2.0.0/ultralight.egg-info/SOURCES.txt
--rw-r--r--   0 abionics   (501) staff       (20)        1 2023-04-10 17:17:27.000000 ultralight-2.0.0/ultralight.egg-info/dependency_links.txt
--rw-r--r--   0 abionics   (501) staff       (20)        1 2023-04-10 17:17:27.000000 ultralight-2.0.0/ultralight.egg-info/not-zip-safe
--rw-r--r--   0 abionics   (501) staff       (20)       54 2023-04-10 17:17:27.000000 ultralight-2.0.0/ultralight.egg-info/requires.txt
--rw-r--r--   0 abionics   (501) staff       (20)       11 2023-04-10 17:17:27.000000 ultralight-2.0.0/ultralight.egg-info/top_level.txt
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-04-14 14:52:20.410391 ultralight-2.1.0/
+-rw-r--r--   0 abionics   (501) staff       (20)     1068 2023-01-20 20:49:15.000000 ultralight-2.1.0/LICENSE.txt
+-rw-r--r--   0 abionics   (501) staff       (20)     2235 2023-04-14 14:52:20.410516 ultralight-2.1.0/PKG-INFO
+-rw-r--r--   0 abionics   (501) staff       (20)     1118 2023-04-06 17:02:58.000000 ultralight-2.1.0/README.md
+-rw-r--r--   0 abionics   (501) staff       (20)       79 2023-04-14 14:52:20.410810 ultralight-2.1.0/setup.cfg
+-rw-r--r--   0 abionics   (501) staff       (20)     1829 2023-04-05 13:57:36.000000 ultralight-2.1.0/setup.py
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-04-14 14:52:20.408563 ultralight-2.1.0/ultralight/
+-rw-r--r--   0 abionics   (501) staff       (20)      166 2023-04-14 14:52:03.000000 ultralight-2.1.0/ultralight/__init__.py
+-rw-r--r--   0 abionics   (501) staff       (20)      174 2023-04-06 16:44:43.000000 ultralight-2.1.0/ultralight/exceptions.py
+-rw-r--r--   0 abionics   (501) staff       (20)     1514 2023-04-07 13:14:59.000000 ultralight-2.1.0/ultralight/loader.py
+-rw-r--r--   0 abionics   (501) staff       (20)      188 2023-04-06 17:02:58.000000 ultralight-2.1.0/ultralight/types.py
+-rw-r--r--   0 abionics   (501) staff       (20)     8301 2023-04-14 14:50:15.000000 ultralight-2.1.0/ultralight/ultralight.py
+-rw-r--r--   0 abionics   (501) staff       (20)     3225 2023-04-06 16:52:40.000000 ultralight-2.1.0/ultralight/utils.py
+drwxr-xr-x   0 abionics   (501) staff       (20)        0 2023-04-14 14:52:20.410257 ultralight-2.1.0/ultralight.egg-info/
+-rw-r--r--   0 abionics   (501) staff       (20)     2235 2023-04-14 14:52:20.000000 ultralight-2.1.0/ultralight.egg-info/PKG-INFO
+-rw-r--r--   0 abionics   (501) staff       (20)      376 2023-04-14 14:52:20.000000 ultralight-2.1.0/ultralight.egg-info/SOURCES.txt
+-rw-r--r--   0 abionics   (501) staff       (20)        1 2023-04-14 14:52:20.000000 ultralight-2.1.0/ultralight.egg-info/dependency_links.txt
+-rw-r--r--   0 abionics   (501) staff       (20)        1 2023-04-14 14:52:20.000000 ultralight-2.1.0/ultralight.egg-info/not-zip-safe
+-rw-r--r--   0 abionics   (501) staff       (20)       54 2023-04-14 14:52:20.000000 ultralight-2.1.0/ultralight.egg-info/requires.txt
+-rw-r--r--   0 abionics   (501) staff       (20)       11 2023-04-14 14:52:20.000000 ultralight-2.1.0/ultralight.egg-info/top_level.txt
```

### Comparing `ultralight-2.0.0/LICENSE.txt` & `ultralight-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ultralight-2.0.0/PKG-INFO` & `ultralight-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralight
-Version: 2.0.0
+Version: 2.1.0
 Summary: Ultra Light Fast Generic Face Detector 👨‍👩‍👧‍👦🖼
 Home-page: https://github.com/abionics/UltraLight
 Author: Alex Ermolaev
 Author-email: abionics.dev@gmail.com
 License: MIT
 Keywords: face detection ai ultra light
 Platform: UNKNOWN
```

### Comparing `ultralight-2.0.0/README.md` & `ultralight-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ultralight-2.0.0/setup.py` & `ultralight-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ultralight-2.0.0/ultralight/loader.py` & `ultralight-2.1.0/ultralight/loader.py`

 * *Files identical despite different names*

### Comparing `ultralight-2.0.0/ultralight/ultralight.py` & `ultralight-2.1.0/ultralight/ultralight.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,19 +97,18 @@
             height, width, _ = image.shape
             boxes, scores = self._postprocess(boxes, scores, width, height, fit_to_image)
             results.append((boxes, scores))
         return results
 
     def _preprocess_images(self, images: Sequence[np.ndarray]) -> np.ndarray:
         images = np.asarray([
-            cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
-            for image in images
-        ])
-        images = np.asarray([
-            cv2.resize(image, self._model_shape)
+            cv2.resize(
+                cv2.cvtColor(image, cv2.COLOR_BGR2RGB),
+                self._model_shape,
+            )
             for image in images
         ])
         images = images.astype(np.float32)  # noqa used in numexpr
         images = ne.evaluate('(images - 127) / 128')
         return np.transpose(images, [0, 3, 1, 2])
 
     def _postprocess(
```

### Comparing `ultralight-2.0.0/ultralight/utils.py` & `ultralight-2.1.0/ultralight/utils.py`

 * *Files identical despite different names*

### Comparing `ultralight-2.0.0/ultralight.egg-info/PKG-INFO` & `ultralight-2.1.0/ultralight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralight
-Version: 2.0.0
+Version: 2.1.0
 Summary: Ultra Light Fast Generic Face Detector 👨‍👩‍👧‍👦🖼
 Home-page: https://github.com/abionics/UltraLight
 Author: Alex Ermolaev
 Author-email: abionics.dev@gmail.com
 License: MIT
 Keywords: face detection ai ultra light
 Platform: UNKNOWN
```

