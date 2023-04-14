# Comparing `tmp/beamer-slider-0.1.8.tar.gz` & `tmp/beamer-slider-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\tuhe\Documents\slider\dist\tmpq5p6wtv5\beamer-slider-0.1.8.tar", last modified: Wed Sep  8 20:50:42 2021, max compression
+gzip compressed data, was "C:\Users\tuhe\Documents\slider\dist\tmpyayqj7d2\beamer-slider-0.1.9.tar", last modified: Wed Sep  8 21:01:52 2021, max compression
```

## Comparing `beamer-slider-0.1.8.tar` & `beamer-slider-0.1.9.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxrwxrwx   0        0        0        0 2021-09-08 20:50:42.071814 beamer-slider-0.1.8/
--rw-rw-rw-   0        0        0     1091 2021-09-02 10:11:20.000000 beamer-slider-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     4751 2021-09-08 20:50:42.066245 beamer-slider-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4187 2021-09-08 20:20:21.000000 beamer-slider-0.1.8/README.md
--rw-rw-rw-   0        0        0      108 2021-09-02 10:05:30.000000 beamer-slider-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2021-09-08 20:50:42.073387 beamer-slider-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1444 2021-09-08 20:49:37.000000 beamer-slider-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-09-08 20:50:41.621966 beamer-slider-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2021-09-08 20:50:41.833024 beamer-slider-0.1.8/src/beamer_slider.egg-info/
--rw-rw-rw-   0        0        0     4751 2021-09-08 20:50:41.000000 beamer-slider-0.1.8/src/beamer_slider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      845 2021-09-08 20:50:41.000000 beamer-slider-0.1.8/src/beamer_slider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-08 20:50:41.000000 beamer-slider-0.1.8/src/beamer_slider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2021-09-08 20:50:41.000000 beamer-slider-0.1.8/src/beamer_slider.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       90 2021-09-08 20:50:41.000000 beamer-slider-0.1.8/src/beamer_slider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2021-09-08 20:50:41.000000 beamer-slider-0.1.8/src/beamer_slider.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-09-08 20:50:41.873233 beamer-slider-0.1.8/src/jinjafy/
--rw-rw-rw-   0        0        0     1303 2021-09-03 09:31:50.000000 beamer-slider-0.1.8/src/jinjafy/__init__.py
--rw-rw-rw-   0        0        0     1381 2021-09-06 18:56:37.000000 beamer-slider-0.1.8/src/jinjafy/bibliography_maker.py
-drwxrwxrwx   0        0        0        0 2021-09-08 20:50:41.881229 beamer-slider-0.1.8/src/jinjafy/cache/
--rw-rw-rw-   0        0        0      474 2021-09-02 18:13:53.000000 beamer-slider-0.1.8/src/jinjafy/cache/__init__.py
--rw-rw-rw-   0        0        0     2607 2020-11-25 11:09:15.000000 beamer-slider-0.1.8/src/jinjafy/cache/simplecache.py
--rw-rw-rw-   0        0        0     3347 2021-08-09 14:26:09.000000 beamer-slider-0.1.8/src/jinjafy/jinja_env.py
--rw-rw-rw-   0        0        0     4223 2020-11-25 11:09:15.000000 beamer-slider-0.1.8/src/jinjafy/jinja_matlab_load.py
--rw-rw-rw-   0        0        0     7067 2021-09-02 18:29:37.000000 beamer-slider-0.1.8/src/jinjafy/jinjafy.py
-drwxrwxrwx   0        0        0        0 2021-09-08 20:50:41.891237 beamer-slider-0.1.8/src/jinjafy/plot/
--rw-rw-rw-   0        0        0       43 2020-11-25 11:09:15.000000 beamer-slider-0.1.8/src/jinjafy/plot/__init__.py
--rw-rw-rw-   0        0        0     1347 2021-09-03 09:58:47.000000 beamer-slider-0.1.8/src/jinjafy/plot/plot_helpers.py
--rw-rw-rw-   0        0        0     3362 2021-09-02 18:29:37.000000 beamer-slider-0.1.8/src/jinjafy/snipper.py
--rw-rw-rw-   0        0        0     5489 2021-09-02 18:35:08.000000 beamer-slider-0.1.8/src/jinjafy/textools.py
-drwxrwxrwx   0        0        0        0 2021-09-08 20:50:42.054151 beamer-slider-0.1.8/src/slider/
--rw-rw-rw-   0        0        0       78 2021-09-04 15:31:29.000000 beamer-slider-0.1.8/src/slider/__init__.py
--rw-rw-rw-   0        0        0      114 2021-09-04 15:31:29.000000 beamer-slider-0.1.8/src/slider/__main__.py
--rw-rw-rw-   0        0        0     2246 2021-09-06 08:38:18.000000 beamer-slider-0.1.8/src/slider/beamer_nup.py
--rw-rw-rw-   0        0        0     4502 2021-09-04 14:06:42.000000 beamer-slider-0.1.8/src/slider/convert.py
--rw-rw-rw-   0        0        0     1150 2021-09-03 08:37:52.000000 beamer-slider-0.1.8/src/slider/latexutils.py
--rw-rw-rw-   0        0        0    19855 2021-09-03 20:09:02.000000 beamer-slider-0.1.8/src/slider/legacy_importer.py
--rw-rw-rw-   0        0        0    11191 2021-09-04 10:54:02.000000 beamer-slider-0.1.8/src/slider/slide.py
--rw-rw-rw-   0        0        0     4841 2021-09-03 17:55:44.000000 beamer-slider-0.1.8/src/slider/slide_fixer.py
--rw-rw-rw-   0        0        0     3063 2021-09-04 14:33:03.000000 beamer-slider-0.1.8/src/slider/slider_cli.py
--rw-rw-rw-   0        0        0     1884 2021-09-04 11:31:36.000000 beamer-slider-0.1.8/src/slider/slider_init.py
+drwxrwxrwx   0        0        0        0 2021-09-08 21:01:52.236431 beamer-slider-0.1.9/
+-rw-rw-rw-   0        0        0     1091 2021-09-02 10:11:20.000000 beamer-slider-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       56 2021-09-08 21:00:53.000000 beamer-slider-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4751 2021-09-08 21:01:52.234432 beamer-slider-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4187 2021-09-08 20:20:21.000000 beamer-slider-0.1.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-02 10:05:30.000000 beamer-slider-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2021-09-08 21:01:52.237430 beamer-slider-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1444 2021-09-08 21:01:07.000000 beamer-slider-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-09-08 21:01:51.832257 beamer-slider-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2021-09-08 21:01:51.899258 beamer-slider-0.1.9/src/beamer_slider.egg-info/
+-rw-rw-rw-   0        0        0     4751 2021-09-08 21:01:50.000000 beamer-slider-0.1.9/src/beamer_slider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      906 2021-09-08 21:01:51.000000 beamer-slider-0.1.9/src/beamer_slider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-09-08 21:01:50.000000 beamer-slider-0.1.9/src/beamer_slider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2021-09-08 21:01:50.000000 beamer-slider-0.1.9/src/beamer_slider.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       90 2021-09-08 21:01:50.000000 beamer-slider-0.1.9/src/beamer_slider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2021-09-08 21:01:50.000000 beamer-slider-0.1.9/src/beamer_slider.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-09-08 21:01:51.928258 beamer-slider-0.1.9/src/jinjafy/
+-rw-rw-rw-   0        0        0     1303 2021-09-03 09:31:50.000000 beamer-slider-0.1.9/src/jinjafy/__init__.py
+-rw-rw-rw-   0        0        0     1381 2021-09-06 18:56:37.000000 beamer-slider-0.1.9/src/jinjafy/bibliography_maker.py
+drwxrwxrwx   0        0        0        0 2021-09-08 21:01:51.940254 beamer-slider-0.1.9/src/jinjafy/cache/
+-rw-rw-rw-   0        0        0      474 2021-09-02 18:13:53.000000 beamer-slider-0.1.9/src/jinjafy/cache/__init__.py
+-rw-rw-rw-   0        0        0     2607 2020-11-25 11:09:15.000000 beamer-slider-0.1.9/src/jinjafy/cache/simplecache.py
+-rw-rw-rw-   0        0        0     3347 2021-08-09 14:26:09.000000 beamer-slider-0.1.9/src/jinjafy/jinja_env.py
+-rw-rw-rw-   0        0        0     4223 2020-11-25 11:09:15.000000 beamer-slider-0.1.9/src/jinjafy/jinja_matlab_load.py
+-rw-rw-rw-   0        0        0     7067 2021-09-02 18:29:37.000000 beamer-slider-0.1.9/src/jinjafy/jinjafy.py
+drwxrwxrwx   0        0        0        0 2021-09-08 21:01:51.948253 beamer-slider-0.1.9/src/jinjafy/plot/
+-rw-rw-rw-   0        0        0       43 2020-11-25 11:09:15.000000 beamer-slider-0.1.9/src/jinjafy/plot/__init__.py
+-rw-rw-rw-   0        0        0     1347 2021-09-03 09:58:47.000000 beamer-slider-0.1.9/src/jinjafy/plot/plot_helpers.py
+-rw-rw-rw-   0        0        0     3362 2021-09-02 18:29:37.000000 beamer-slider-0.1.9/src/jinjafy/snipper.py
+-rw-rw-rw-   0        0        0     5489 2021-09-02 18:35:08.000000 beamer-slider-0.1.9/src/jinjafy/textools.py
+drwxrwxrwx   0        0        0        0 2021-09-08 21:01:52.165300 beamer-slider-0.1.9/src/slider/
+drwxrwxrwx   0        0        0        0 2021-09-08 21:01:52.228431 beamer-slider-0.1.9/src/slider/DTU_Beamer_files/
+-rw-rw-rw-   0        0        0    63154 2021-09-08 20:46:10.000000 beamer-slider-0.1.9/src/slider/DTU_Beamer_files/DTU_Beamer_files.zip
+-rw-rw-rw-   0        0        0       78 2021-09-04 15:31:29.000000 beamer-slider-0.1.9/src/slider/__init__.py
+-rw-rw-rw-   0        0        0      114 2021-09-04 15:31:29.000000 beamer-slider-0.1.9/src/slider/__main__.py
+-rw-rw-rw-   0        0        0     2246 2021-09-06 08:38:18.000000 beamer-slider-0.1.9/src/slider/beamer_nup.py
+-rw-rw-rw-   0        0        0     4502 2021-09-04 14:06:42.000000 beamer-slider-0.1.9/src/slider/convert.py
+-rw-rw-rw-   0        0        0     1150 2021-09-03 08:37:52.000000 beamer-slider-0.1.9/src/slider/latexutils.py
+-rw-rw-rw-   0        0        0    19855 2021-09-03 20:09:02.000000 beamer-slider-0.1.9/src/slider/legacy_importer.py
+-rw-rw-rw-   0        0        0    11191 2021-09-04 10:54:02.000000 beamer-slider-0.1.9/src/slider/slide.py
+-rw-rw-rw-   0        0        0     4841 2021-09-03 17:55:44.000000 beamer-slider-0.1.9/src/slider/slide_fixer.py
+-rw-rw-rw-   0        0        0     3063 2021-09-04 14:33:03.000000 beamer-slider-0.1.9/src/slider/slider_cli.py
+-rw-rw-rw-   0        0        0     1884 2021-09-04 11:31:36.000000 beamer-slider-0.1.9/src/slider/slider_init.py
```

### Comparing `beamer-slider-0.1.8/LICENSE` & `beamer-slider-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/PKG-INFO` & `beamer-slider-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beamer-slider
-Version: 0.1.8
+Version: 0.1.9
 Summary: Software to create inkscape overlays in Beamer
 Home-page: https://lab.compute.dtu.dk/tuhe/slider
 Author: Tue Herlau
 Author-email: tuhe@dtu.dk
 License: MIT
 Project-URL: Bug Tracker, https://lab.compute.dtu.dk/tuhe/slider/issues
 Platform: UNKNOWN
```

### Comparing `beamer-slider-0.1.8/README.md` & `beamer-slider-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/setup.py` & `beamer-slider-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 import pkg_resources
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="beamer-slider",
-    version="0.1.8",
+    version="0.1.9",
     author="Tue Herlau",
     author_email="tuhe@dtu.dk",
     description="Software to create inkscape overlays in Beamer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url='https://lab.compute.dtu.dk/tuhe/slider',
```

### Comparing `beamer-slider-0.1.8/src/beamer_slider.egg-info/PKG-INFO` & `beamer-slider-0.1.9/src/beamer_slider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beamer-slider
-Version: 0.1.8
+Version: 0.1.9
 Summary: Software to create inkscape overlays in Beamer
 Home-page: https://lab.compute.dtu.dk/tuhe/slider
 Author: Tue Herlau
 Author-email: tuhe@dtu.dk
 License: MIT
 Project-URL: Bug Tracker, https://lab.compute.dtu.dk/tuhe/slider/issues
 Platform: UNKNOWN
```

### Comparing `beamer-slider-0.1.8/src/beamer_slider.egg-info/SOURCES.txt` & `beamer-slider-0.1.9/src/beamer_slider.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/beamer_slider.egg-info/PKG-INFO
 src/beamer_slider.egg-info/SOURCES.txt
 src/beamer_slider.egg-info/dependency_links.txt
 src/beamer_slider.egg-info/entry_points.txt
@@ -24,8 +25,9 @@
 src/slider/beamer_nup.py
 src/slider/convert.py
 src/slider/latexutils.py
 src/slider/legacy_importer.py
 src/slider/slide.py
 src/slider/slide_fixer.py
 src/slider/slider_cli.py
-src/slider/slider_init.py
+src/slider/slider_init.py
+src/slider/DTU_Beamer_files/DTU_Beamer_files.zip
```

### Comparing `beamer-slider-0.1.8/src/jinjafy/__init__.py` & `beamer-slider-0.1.9/src/jinjafy/__init__.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/jinjafy/bibliography_maker.py` & `beamer-slider-0.1.9/src/jinjafy/bibliography_maker.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/jinjafy/cache/simplecache.py` & `beamer-slider-0.1.9/src/jinjafy/cache/simplecache.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/jinjafy/jinja_env.py` & `beamer-slider-0.1.9/src/jinjafy/jinja_env.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/jinjafy/jinja_matlab_load.py` & `beamer-slider-0.1.9/src/jinjafy/jinja_matlab_load.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/jinjafy/jinjafy.py` & `beamer-slider-0.1.9/src/jinjafy/jinjafy.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/jinjafy/plot/plot_helpers.py` & `beamer-slider-0.1.9/src/jinjafy/plot/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/jinjafy/snipper.py` & `beamer-slider-0.1.9/src/jinjafy/snipper.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/jinjafy/textools.py` & `beamer-slider-0.1.9/src/jinjafy/textools.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/slider/beamer_nup.py` & `beamer-slider-0.1.9/src/slider/beamer_nup.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/slider/convert.py` & `beamer-slider-0.1.9/src/slider/convert.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/slider/latexutils.py` & `beamer-slider-0.1.9/src/slider/latexutils.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/slider/legacy_importer.py` & `beamer-slider-0.1.9/src/slider/legacy_importer.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/slider/slide.py` & `beamer-slider-0.1.9/src/slider/slide.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/slider/slide_fixer.py` & `beamer-slider-0.1.9/src/slider/slide_fixer.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/slider/slider_cli.py` & `beamer-slider-0.1.9/src/slider/slider_cli.py`

 * *Files identical despite different names*

### Comparing `beamer-slider-0.1.8/src/slider/slider_init.py` & `beamer-slider-0.1.9/src/slider/slider_init.py`

 * *Files identical despite different names*

