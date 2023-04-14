# Comparing `tmp/test_query_tool-0.3.5.tar.gz` & `tmp/test_query_tool-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_query_tool-0.3.5.tar", last modified: Thu Apr 13 18:16:38 2023, max compression
+gzip compressed data, was "test_query_tool-0.3.7.tar", last modified: Fri Apr 14 10:06:26 2023, max compression
```

## Comparing `test_query_tool-0.3.5.tar` & `test_query_tool-0.3.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.990313 test_query_tool-0.3.5/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 test_query_tool-0.3.5/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 test_query_tool-0.3.5/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 18:16:38.989904 test_query_tool-0.3.5/PKG-INFO
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.981346 test_query_tool-0.3.5/query_tool/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3587 2023-04-13 18:16:00.000000 test_query_tool-0.3.5/query_tool/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.979752 test_query_tool-0.3.5/query_tool/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.982145 test_query_tool-0.3.5/query_tool/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.985141 test_query_tool-0.3.5/query_tool/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044761 2023-04-13 18:12:35.000000 test_query_tool-0.3.5/query_tool/frontend/dist/assets/index-49ab9bc7.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-13 18:12:35.000000 test_query_tool-0.3.5/query_tool/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-13 18:12:47.000000 test_query_tool-0.3.5/query_tool/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-13 18:12:34.000000 test_query_tool-0.3.5/query_tool/frontend/dist/vite.svg
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.987593 test_query_tool-0.3.5/query_tool/services/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/dimension_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/entities_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/filters_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/query_tool_factory.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/query_tool_service.py
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 test_query_tool-0.3.5/query_tool/services/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-13 18:16:38.990422 test_query_tool-0.3.5/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-13 18:16:12.000000 test_query_tool-0.3.5/setup.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:16:38.989400 test_query_tool-0.3.5/test_query_tool.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 18:16:38.000000 test_query_tool-0.3.5/test_query_tool.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      684 2023-04-13 18:16:38.000000 test_query_tool-0.3.5/test_query_tool.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-13 18:16:38.000000 test_query_tool-0.3.5/test_query_tool.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-13 18:16:38.000000 test_query_tool-0.3.5/test_query_tool.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-13 18:16:38.000000 test_query_tool-0.3.5/test_query_tool.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-14 10:06:26.558933 test_query_tool-0.3.7/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 test_query_tool-0.3.7/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 test_query_tool-0.3.7/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-14 10:06:26.558658 test_query_tool-0.3.7/PKG-INFO
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-14 10:06:26.549570 test_query_tool-0.3.7/query_tool/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3587 2023-04-13 18:16:00.000000 test_query_tool-0.3.7/query_tool/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-14 10:06:26.547746 test_query_tool-0.3.7/query_tool/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-14 10:06:26.550349 test_query_tool-0.3.7/query_tool/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-14 10:06:26.552430 test_query_tool-0.3.7/query_tool/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044744 2023-04-14 10:05:07.000000 test_query_tool-0.3.7/query_tool/frontend/dist/assets/index-99e5fe3f.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-14 10:05:07.000000 test_query_tool-0.3.7/query_tool/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-14 10:05:13.000000 test_query_tool-0.3.7/query_tool/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-14 10:05:06.000000 test_query_tool-0.3.7/query_tool/frontend/dist/vite.svg
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-14 10:06:26.555801 test_query_tool-0.3.7/query_tool/services/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 test_query_tool-0.3.7/query_tool/services/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 test_query_tool-0.3.7/query_tool/services/dimension_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 test_query_tool-0.3.7/query_tool/services/entities_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 test_query_tool-0.3.7/query_tool/services/filters_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 test_query_tool-0.3.7/query_tool/services/query_tool_factory.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 test_query_tool-0.3.7/query_tool/services/query_tool_service.py
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 test_query_tool-0.3.7/query_tool/services/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-14 10:06:26.559032 test_query_tool-0.3.7/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-14 10:05:33.000000 test_query_tool-0.3.7/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-14 10:06:26.558117 test_query_tool-0.3.7/test_query_tool.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-14 10:06:26.000000 test_query_tool-0.3.7/test_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      684 2023-04-14 10:06:26.000000 test_query_tool-0.3.7/test_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-14 10:06:26.000000 test_query_tool-0.3.7/test_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-14 10:06:26.000000 test_query_tool-0.3.7/test_query_tool.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-14 10:06:26.000000 test_query_tool-0.3.7/test_query_tool.egg-info/top_level.txt
```

### Comparing `test_query_tool-0.3.5/LICENSE` & `test_query_tool-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.5/query_tool/__init__.py` & `test_query_tool-0.3.7/query_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.5/query_tool/frontend/dist/assets/index-49ab9bc7.js` & `test_query_tool-0.3.7/query_tool/frontend/dist/assets/index-99e5fe3f.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -45647,15 +45647,15 @@
             column: "",
             measures: [],
             id: lo()
         }]), N = C.useCallback(P => {
             o(P)
         }, [o]);
         C.useEffect(() => {
-            console.log("onResize"), l()
+            l()
         }, [I, S, O, l, n]);
         const g = () => {
                 const [P = [], b] = VEe(pI(I));
                 if (!b || (P == null ? void 0 : P.length) === 0) return null;
                 const [H, x] = YEe(pI(S));
                 if (!x) return null;
                 const [V, J] = kEe(pI(O));
@@ -45739,15 +45739,15 @@
                 mt: 3,
                 p: 3,
                 gap: 2,
                 children: [Ue(wn, {
                     direction: "row",
                     justifyContent: "space-between",
                     children: [U(la, {
-                        variant: "h6",
+                        variant: "subtitle1",
                         p: 0,
                         children: U(Bi, {
                             children: "QUERY"
                         })
                     }), U(gr, {
                         title: "Copy to clipboard",
                         placement: "top",
```

### Comparing `test_query_tool-0.3.5/query_tool/frontend/dist/vite.svg` & `test_query_tool-0.3.7/query_tool/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.5/query_tool/services/dimension_service.py` & `test_query_tool-0.3.7/query_tool/services/dimension_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.5/query_tool/services/entities_service.py` & `test_query_tool-0.3.7/query_tool/services/entities_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.5/query_tool/services/filters_service.py` & `test_query_tool-0.3.7/query_tool/services/filters_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.5/query_tool/services/query_tool_service.py` & `test_query_tool-0.3.7/query_tool/services/query_tool_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.5/query_tool/services/register.py` & `test_query_tool-0.3.7/query_tool/services/register.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.5/setup.py` & `test_query_tool-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="test_query_tool",
-    version="0.3.5",
+    version="0.3.7",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="Query tool to generate query from selection",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `test_query_tool-0.3.5/test_query_tool.egg-info/SOURCES.txt` & `test_query_tool-0.3.7/test_query_tool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE
 MANIFEST.in
 setup.py
 query_tool/__init__.py
 query_tool/frontend/dist/index.html
 query_tool/frontend/dist/vite.svg
-query_tool/frontend/dist/assets/index-49ab9bc7.js
+query_tool/frontend/dist/assets/index-99e5fe3f.js
 query_tool/frontend/dist/assets/index-d081bea5.css
 query_tool/services/__init__.py
 query_tool/services/dimension_service.py
 query_tool/services/entities_service.py
 query_tool/services/filters_service.py
 query_tool/services/query_tool_factory.py
 query_tool/services/query_tool_service.py
```

