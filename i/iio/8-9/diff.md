# Comparing `tmp/iio-8.tar.gz` & `tmp/iio-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iio-8.tar", last modified: Fri Feb 10 14:28:44 2023, max compression
+gzip compressed data, was "iio-9.tar", last modified: Thu Feb 16 09:52:39 2023, max compression
```

## Comparing `iio-8.tar` & `iio-9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-02-10 14:28:44.518411 iio-8/
--rw-rw-r--   0 coco      (1000) coco      (1000)      316 2023-02-10 14:28:44.518411 iio-8/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)      362 2022-10-17 15:31:36.000000 iio-8/README
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-02-10 14:28:44.518411 iio-8/iio/
--rw-rw-r--   0 coco      (1000) coco      (1000)   182534 2022-10-17 15:04:27.000000 iio-8/iio/iio.c
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-02-10 14:28:44.518411 iio-8/iio.egg-info/
--rw-rw-r--   0 coco      (1000) coco      (1000)      316 2023-02-10 14:28:44.000000 iio-8/iio.egg-info/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)      153 2023-02-10 14:28:44.000000 iio-8/iio.egg-info/SOURCES.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-02-10 14:28:44.000000 iio-8/iio.egg-info/dependency_links.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)       11 2023-02-10 14:28:44.000000 iio-8/iio.egg-info/top_level.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)     4637 2023-02-10 14:15:57.000000 iio-8/iio.py
--rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-02-10 14:28:44.518411 iio-8/setup.cfg
--rw-rw-r--   0 coco      (1000) coco      (1000)     2580 2023-02-10 14:05:30.000000 iio-8/setup.py
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-02-10 14:28:44.518411 iio-8/test/
--rw-------   0 coco      (1000) coco      (1000)      124 2019-06-27 14:05:35.000000 iio-8/test/test.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-02-16 09:52:39.422267 iio-9/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      316 2023-02-16 09:52:39.422267 iio-9/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)      362 2022-10-17 15:31:36.000000 iio-9/README
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-02-16 09:52:39.418267 iio-9/iio/
+-rw-rw-r--   0 coco      (1000) coco      (1000)   182534 2022-10-17 15:04:27.000000 iio-9/iio/iio.c
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-02-16 09:52:39.422267 iio-9/iio.egg-info/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      316 2023-02-16 09:52:39.000000 iio-9/iio.egg-info/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)      153 2023-02-16 09:52:39.000000 iio-9/iio.egg-info/SOURCES.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-02-16 09:52:39.000000 iio-9/iio.egg-info/dependency_links.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)       11 2023-02-16 09:52:39.000000 iio-9/iio.egg-info/top_level.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)     5036 2023-02-16 09:51:25.000000 iio-9/iio.py
+-rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-02-16 09:52:39.422267 iio-9/setup.cfg
+-rw-rw-r--   0 coco      (1000) coco      (1000)     2580 2023-02-16 09:51:25.000000 iio-9/setup.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-02-16 09:52:39.422267 iio-9/test/
+-rw-------   0 coco      (1000) coco      (1000)      124 2019-06-27 14:05:35.000000 iio-9/test/test.py
```

### Comparing `iio-8/iio/iio.c` & `iio-9/iio/iio.c`

 * *Files identical despite different names*

### Comparing `iio-8/iio.py` & `iio-9/iio.py`

 * *Files 15% similar despite different names*

```diff
@@ -82,19 +82,34 @@
 def __notebookP():
 	try:
 		x = get_ipython().config
 		return True
 	except NameError:
 		return False
 
+# internal function to do some notebook magic (only for gray images, by now)
+def __heuristic_reshape(s):
+	try:
+		w = get_ipython().all_ns_refs[0]['w']
+		h = get_ipython().all_ns_refs[0]['h']
+		if s[0] == w*h:
+			return (h,w)
+		else:
+			return s
+	except (NameError, KeyError):
+		return s
 
 # internal function to urlencode a numpy array into html
 def __img_tag_with_b64jpg(x):
 	if (x.shape[0] > 4000):
-		return f'<b>cannot display image of size {x.shape}</b>'
+		s = __heuristic_reshape(x.shape)
+		if s == x.shape:
+			return f'<b>cannot display image of size {x.shape}</b>'
+		else:
+			x = x.reshape(s)
 
 	from tempfile import NamedTemporaryFile
 	from base64 import b64encode
 	from os import unlink
 
 	f = NamedTemporaryFile(prefix="iioshow_", suffix=".jpg", delete=False)
 	write(f.name, x)
@@ -125,15 +140,16 @@
 
 	from  IPython.display import display, HTML
 
 	L = ""  # html list of gallery items
 	h = 0   # height of the gallery (height of the tallest image)
 	i = 0   # loop counter
 	for x in images:
-		h = max(h, x.shape[0])
+		s = __heuristic_reshape(x.shape)
+		h = max(h, s[0])
 		j = __img_tag_with_b64jpg(x)
 		L = f'{L}<li><a href="#">{i}<span>{j}</span></a>'
 		i = i + 1
 
 	html = f"""
 	<div class="gallery2">
 		<ul class="index">
@@ -186,10 +202,10 @@
 	"""
 
 	display(HTML( html ))
 	display(HTML( css ))
 
 
 # API
-version = 8
+version = 9
 
 __all__ = [ "read", "write", "display", "gallery", "version" ]
```

### Comparing `iio-8/setup.py` & `iio-9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         # for each file, match string between
         # second last and last dot and trim it
         matcher = re.compile('\.([^.]+)\.so$')
         return [batch_rename(file, re.sub(matcher, '.so', file))
                 for file in outfiles]
 
 setup(name="iio",
-      version='8',
+      version='9',
       author="Jérémy Anger, Gabriele Facciolo, Enric Meinhardt-Llopis",
       author_email="enric.meinhardt@fastmail.com",
       description="Python wrapper to iio",
       url='https://github.com/mnhrdt/iio',
       classifiers=[
           "Operating System :: OS Independent",
       ],
```

