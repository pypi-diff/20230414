# Comparing `tmp/melkit-0.1.6.tar.gz` & `tmp/melkit-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melkit-0.1.6.tar", last modified: Thu Apr 13 16:24:56 2023, max compression
+gzip compressed data, was "melkit-0.1.7.tar", last modified: Fri Apr 14 07:58:44 2023, max compression
```

## Comparing `melkit-0.1.6.tar` & `melkit-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:24:56.990030 melkit-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 16:24:56.000000 melkit-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 16:24:56.000000 melkit-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 16:24:56.990030 melkit-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-13 16:24:56.000000 melkit-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:24:56.990030 melkit-0.1.6/melkit/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21127 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:24:56.990030 melkit-0.1.6/melkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 16:24:56.000000 melkit-0.1.6/melkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 16:24:56.000000 melkit-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 16:24:56.990030 melkit-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-13 16:24:56.000000 melkit-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:44.160835 melkit-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 07:58:43.000000 melkit-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 07:58:43.000000 melkit-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-14 07:58:44.160835 melkit-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-14 07:58:43.000000 melkit-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:44.160835 melkit-0.1.7/melkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 07:58:43.000000 melkit-0.1.7/melkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 07:58:43.000000 melkit-0.1.7/melkit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 07:58:43.000000 melkit-0.1.7/melkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-14 07:58:43.000000 melkit-0.1.7/melkit/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21118 2023-04-14 07:58:43.000000 melkit-0.1.7/melkit/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 07:58:43.000000 melkit-0.1.7/melkit/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:44.160835 melkit-0.1.7/melkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-14 07:58:44.000000 melkit-0.1.7/melkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 07:58:44.000000 melkit-0.1.7/melkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:58:44.000000 melkit-0.1.7/melkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-14 07:58:44.000000 melkit-0.1.7/melkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 07:58:44.000000 melkit-0.1.7/melkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 07:58:43.000000 melkit-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 07:58:44.160835 melkit-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-14 07:58:43.000000 melkit-0.1.7/setup.py
```

### Comparing `melkit-0.1.6/LICENSE` & `melkit-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `melkit-0.1.6/README.md` & `melkit-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `melkit-0.1.6/melkit/inputs.py` & `melkit-0.1.7/melkit/inputs.py`

 * *Files identical despite different names*

### Comparing `melkit-0.1.6/melkit/toolkit.py` & `melkit-0.1.7/melkit/toolkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         src_file = self._filename
         new_file = new_file or src_file + '_NEW'
 
         with open(src_file, 'r') as f1, open(new_file, 'w') as f2:
             written = False
             for line in f1:
                 if line.startswith('.') and not written:
-                    f2.write('*\n' + str(obj) + '*\n' + line)
+                    f2.write(str(obj) + '\n' + line)
                     written = True
                 else:
                     f2.write(line)
 
         if overwrite:
             remove(src_file)
             rename(new_file, src_file)
```

### Comparing `melkit-0.1.6/setup.py` & `melkit-0.1.7/setup.py`

 * *Files identical despite different names*

