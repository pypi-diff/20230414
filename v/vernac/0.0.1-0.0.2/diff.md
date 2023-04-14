# Comparing `tmp/vernac-0.0.1.tar.gz` & `tmp/vernac-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vernac-0.0.1.tar", last modified: Thu Apr 13 17:51:15 2023, max compression
+gzip compressed data, was "vernac-0.0.2.tar", last modified: Thu Apr 13 18:56:40 2023, max compression
```

## Comparing `vernac-0.0.1.tar` & `vernac-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 17:51:15.983838 vernac-0.0.1/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1867 2023-04-13 17:01:30.000000 vernac-0.0.1/.gitignore
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1074 2023-04-13 16:57:19.000000 vernac-0.0.1/LICENSE
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1994 2023-04-13 17:51:15.983838 vernac-0.0.1/PKG-INFO
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1837 2023-04-13 16:57:36.000000 vernac-0.0.1/README.md
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1153 2023-04-13 16:59:44.000000 vernac-0.0.1/dev-requirements.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       34 2023-04-13 16:59:44.000000 vernac-0.0.1/local-dev-requirements.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      452 2023-04-13 17:40:54.000000 vernac-0.0.1/pyproject.toml
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       38 2023-04-13 17:51:15.983838 vernac-0.0.1/setup.cfg
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 17:51:15.983838 vernac-0.0.1/src/
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 17:51:15.983838 vernac-0.0.1/src/vernac/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     5980 2023-04-13 16:59:08.000000 vernac-0.0.1/src/vernac/compile.py
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 17:51:15.983838 vernac-0.0.1/src/vernac.egg-info/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1994 2023-04-13 17:51:15.000000 vernac-0.0.1/src/vernac.egg-info/PKG-INFO
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      319 2023-04-13 17:51:15.000000 vernac-0.0.1/src/vernac.egg-info/SOURCES.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        1 2023-04-13 17:51:15.000000 vernac-0.0.1/src/vernac.egg-info/dependency_links.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       54 2023-04-13 17:51:15.000000 vernac-0.0.1/src/vernac.egg-info/entry_points.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       65 2023-04-13 17:51:15.000000 vernac-0.0.1/src/vernac.egg-info/requires.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        7 2023-04-13 17:51:15.000000 vernac-0.0.1/src/vernac.egg-info/top_level.txt
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 18:56:40.753269 vernac-0.0.2/
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1867 2023-04-13 17:01:30.000000 vernac-0.0.2/.gitignore
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1074 2023-04-13 16:57:19.000000 vernac-0.0.2/LICENSE
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2123 2023-04-13 18:56:40.753269 vernac-0.0.2/PKG-INFO
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1840 2023-04-13 18:44:27.000000 vernac-0.0.2/README.md
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1153 2023-04-13 16:59:44.000000 vernac-0.0.2/dev-requirements.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       34 2023-04-13 16:59:44.000000 vernac-0.0.2/local-dev-requirements.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      574 2023-04-13 18:49:35.000000 vernac-0.0.2/pyproject.toml
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       38 2023-04-13 18:56:40.753269 vernac-0.0.2/setup.cfg
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 18:56:40.753269 vernac-0.0.2/src/
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 18:56:40.753269 vernac-0.0.2/src/vernac/
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     5980 2023-04-13 16:59:08.000000 vernac-0.0.2/src/vernac/compile.py
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 18:56:40.753269 vernac-0.0.2/src/vernac.egg-info/
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2123 2023-04-13 18:56:40.000000 vernac-0.0.2/src/vernac.egg-info/PKG-INFO
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      319 2023-04-13 18:56:40.000000 vernac-0.0.2/src/vernac.egg-info/SOURCES.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        1 2023-04-13 18:56:40.000000 vernac-0.0.2/src/vernac.egg-info/dependency_links.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       54 2023-04-13 18:56:40.000000 vernac-0.0.2/src/vernac.egg-info/entry_points.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       65 2023-04-13 18:56:40.000000 vernac-0.0.2/src/vernac.egg-info/requires.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        7 2023-04-13 18:56:40.000000 vernac-0.0.2/src/vernac.egg-info/top_level.txt
```

### Comparing `vernac-0.0.1/.gitignore` & `vernac-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `vernac-0.0.1/LICENSE` & `vernac-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vernac-0.0.1/PKG-INFO` & `vernac-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,11 @@
-Metadata-Version: 2.1
-Name: vernac
-Version: 0.0.1
-Requires-Python: ~=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
+Vernac: programming (in) language 📖
+====================================
 
-Vernac: programming (in) language
-=================================
-
-Vernac is a tool for writing software in "vernacular"—plain language. 📖
+Vernac is a tool for writing software in "vernacular"—plain language.
 
 Vernac isn't for turning English into code; it's for turning English into _programs_:
 
 ```console
 $ cat fizzbuzz.vn
 print all the numbers between 1 and 100
 print 'fizz' instead of the number if it’s divisible by 3
```

### Comparing `vernac-0.0.1/README.md` & `vernac-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,21 @@
-Vernac: programming (in) language
-=================================
+Metadata-Version: 2.1
+Name: vernac
+Version: 0.0.2
+Project-URL: homepage, https://github.com/bsilverthorn/vernac
+Project-URL: repository, https://github.com/bsilverthorn/vernac
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
 
-Vernac is a tool for writing software in "vernacular"—plain language. 📖
+Vernac: programming (in) language 📖
+====================================
+
+Vernac is a tool for writing software in "vernacular"—plain language.
 
 Vernac isn't for turning English into code; it's for turning English into _programs_:
 
 ```console
 $ cat fizzbuzz.vn
 print all the numbers between 1 and 100
 print 'fizz' instead of the number if it’s divisible by 3
```

### Comparing `vernac-0.0.1/dev-requirements.txt` & `vernac-0.0.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `vernac-0.0.1/src/vernac/compile.py` & `vernac-0.0.2/src/vernac/compile.py`

 * *Files identical despite different names*

### Comparing `vernac-0.0.1/src/vernac.egg-info/PKG-INFO` & `vernac-0.0.2/src/vernac.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: vernac
-Version: 0.0.1
-Requires-Python: ~=3.11
+Version: 0.0.2
+Project-URL: homepage, https://github.com/bsilverthorn/vernac
+Project-URL: repository, https://github.com/bsilverthorn/vernac
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-Vernac: programming (in) language
-=================================
+Vernac: programming (in) language 📖
+====================================
 
-Vernac is a tool for writing software in "vernacular"—plain language. 📖
+Vernac is a tool for writing software in "vernacular"—plain language.
 
 Vernac isn't for turning English into code; it's for turning English into _programs_:
 
 ```console
 $ cat fizzbuzz.vn
 print all the numbers between 1 and 100
 print 'fizz' instead of the number if it’s divisible by 3
```

