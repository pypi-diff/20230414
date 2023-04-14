# Comparing `tmp/lupin-danquin-0.0.1.dev9.tar.gz` & `tmp/lupin-danquin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-danquin-0.0.1.dev9.tar", last modified: Wed Apr 12 14:56:49 2023, max compression
+gzip compressed data, was "lupin-danquin-1.0.0.tar", last modified: Fri Apr 14 13:07:40 2023, max compression
```

## Comparing `lupin-danquin-0.0.1.dev9.tar` & `lupin-danquin-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.990008 lupin-danquin-0.0.1.dev9/
--rw-rw-rw-   0        0        0     1093 2023-04-11 13:56:08.000000 lupin-danquin-0.0.1.dev9/LICENCE
--rw-rw-rw-   0        0        0       67 2023-04-12 12:24:19.000000 lupin-danquin-0.0.1.dev9/MANIFEST.in
--rw-rw-rw-   0        0        0      573 2023-04-12 14:56:49.990008 lupin-danquin-0.0.1.dev9/PKG-INFO
--rw-rw-rw-   0        0        0     1809 2023-04-12 12:25:35.000000 lupin-danquin-0.0.1.dev9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.949904 lupin-danquin-0.0.1.dev9/lupin_danquin/
--rw-rw-rw-   0        0        0       28 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/__init__.py
--rw-rw-rw-   0        0        0       78 2023-04-12 12:24:19.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.969651 lupin-danquin-0.0.1.dev9/lupin_danquin/assets/
--rw-rw-rw-   0        0        0     6730 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/assets/BeginingOfFile.md
--rw-rw-rw-   0        0        0      379 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/assets/EndOfFile.md
-drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.981118 lupin-danquin-0.0.1.dev9/lupin_danquin/core/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/__init__.py
--rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/application.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.984008 lupin-danquin-0.0.1.dev9/lupin_danquin/core/coding_rules_validator/
--rw-rw-rw-   0        0        0        0 2023-04-12 13:03:44.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/coding_rules_validator/__init__.py
--rw-rw-rw-   0        0        0     1339 2023-04-12 14:40:35.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/coding_rules_validator/coging_rules_validator.py
--rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/global_variable.py
--rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/line_ended.py
--rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/local_variable.py
--rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/parameter.py
--rw-rw-rw-   0        0        0     4619 2023-04-11 13:55:43.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/program.py
--rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.986007 lupin-danquin-0.0.1.dev9/lupin_danquin/core/tools/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/tools/__init__.py
--rw-rw-rw-   0        0        0     2008 2023-04-12 14:39:37.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.988007 lupin-danquin-0.0.1.dev9/lupin_danquin/core/val3_doc_generator/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/val3_doc_generator/__init__.py
--rw-rw-rw-   0        0        0     2657 2023-04-12 14:54:07.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
--rw-rw-rw-   0        0        0     3078 2023-04-12 14:56:15.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/run.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.989009 lupin-danquin-0.0.1.dev9/lupin_danquin/templates/
--rw-rw-rw-   0        0        0     2801 2023-04-12 12:24:19.000000 lupin-danquin-0.0.1.dev9/lupin_danquin/templates/val3_documentation_md.j2
-drwxrwxrwx   0        0        0        0 2023-04-12 14:56:49.966976 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/
--rw-rw-rw-   0        0        0      573 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1069 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 14:28:43.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 14:56:49.000000 lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      906 2023-04-12 14:56:49.992526 lupin-danquin-0.0.1.dev9/setup.cfg
--rw-rw-rw-   0        0        0      178 2023-04-11 14:20:31.000000 lupin-danquin-0.0.1.dev9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:40.591047 lupin-danquin-1.0.0/
+-rw-rw-rw-   0        0        0     1093 2023-04-11 13:56:08.000000 lupin-danquin-1.0.0/LICENCE
+-rw-rw-rw-   0        0        0       67 2023-04-12 12:24:19.000000 lupin-danquin-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      568 2023-04-14 13:07:40.592053 lupin-danquin-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1809 2023-04-12 12:25:35.000000 lupin-danquin-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:40.472238 lupin-danquin-1.0.0/lupin_danquin/
+-rw-rw-rw-   0        0        0       23 2023-04-14 13:07:40.000000 lupin-danquin-1.0.0/lupin_danquin/__init__.py
+-rw-rw-rw-   0        0        0       78 2023-04-12 12:24:19.000000 lupin-danquin-1.0.0/lupin_danquin/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:40.542800 lupin-danquin-1.0.0/lupin_danquin/assets/
+-rw-rw-rw-   0        0        0     6730 2023-04-03 12:43:51.000000 lupin-danquin-1.0.0/lupin_danquin/assets/BeginingOfFile.md
+-rw-rw-rw-   0        0        0      379 2023-04-03 12:43:51.000000 lupin-danquin-1.0.0/lupin_danquin/assets/EndOfFile.md
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:40.550304 lupin-danquin-1.0.0/lupin_danquin/core/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-1.0.0/lupin_danquin/core/__init__.py
+-rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-1.0.0/lupin_danquin/core/application.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:40.551834 lupin-danquin-1.0.0/lupin_danquin/core/coding_rules_validator/
+-rw-rw-rw-   0        0        0        0 2023-04-12 15:23:46.000000 lupin-danquin-1.0.0/lupin_danquin/core/coding_rules_validator/__init__.py
+-rw-rw-rw-   0        0        0     1390 2023-04-14 13:06:50.000000 lupin-danquin-1.0.0/lupin_danquin/core/coding_rules_validator/coging_rules_validator.py
+-rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-1.0.0/lupin_danquin/core/global_variable.py
+-rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-1.0.0/lupin_danquin/core/line_ended.py
+-rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-1.0.0/lupin_danquin/core/local_variable.py
+-rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-1.0.0/lupin_danquin/core/parameter.py
+-rw-rw-rw-   0        0        0     4619 2023-04-11 13:55:43.000000 lupin-danquin-1.0.0/lupin_danquin/core/program.py
+-rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-1.0.0/lupin_danquin/core/rules.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:40.553837 lupin-danquin-1.0.0/lupin_danquin/core/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-1.0.0/lupin_danquin/core/tools/__init__.py
+-rw-rw-rw-   0        0        0     2008 2023-04-12 15:23:46.000000 lupin-danquin-1.0.0/lupin_danquin/core/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:40.556835 lupin-danquin-1.0.0/lupin_danquin/core/val3_doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-1.0.0/lupin_danquin/core/val3_doc_generator/__init__.py
+-rw-rw-rw-   0        0        0     2657 2023-04-12 15:23:46.000000 lupin-danquin-1.0.0/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
+-rw-rw-rw-   0        0        0     3078 2023-04-12 15:23:46.000000 lupin-danquin-1.0.0/lupin_danquin/run.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:40.589541 lupin-danquin-1.0.0/lupin_danquin/templates/
+-rw-rw-rw-   0        0        0     2801 2023-04-12 12:24:19.000000 lupin-danquin-1.0.0/lupin_danquin/templates/val3_documentation_md.j2
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:40.492986 lupin-danquin-1.0.0/lupin_danquin.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-04-14 13:07:40.000000 lupin-danquin-1.0.0/lupin_danquin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1069 2023-04-14 13:07:40.000000 lupin-danquin-1.0.0/lupin_danquin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:07:40.000000 lupin-danquin-1.0.0/lupin_danquin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-14 13:07:40.000000 lupin-danquin-1.0.0/lupin_danquin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 14:28:43.000000 lupin-danquin-1.0.0/lupin_danquin.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-04-14 13:07:40.000000 lupin-danquin-1.0.0/lupin_danquin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-14 13:07:40.000000 lupin-danquin-1.0.0/lupin_danquin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      901 2023-04-14 13:07:40.597062 lupin-danquin-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      178 2023-04-11 14:20:31.000000 lupin-danquin-1.0.0/setup.py
```

### Comparing `lupin-danquin-0.0.1.dev9/LICENCE` & `lupin-danquin-1.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev9/PKG-INFO` & `lupin-danquin-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev9
+Version: 1.0.0
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-0.0.1.dev9/README.md` & `lupin-danquin-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev9/lupin_danquin/assets/BeginingOfFile.md` & `lupin-danquin-1.0.0/lupin_danquin/assets/BeginingOfFile.md`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev9/lupin_danquin/core/application.py` & `lupin-danquin-1.0.0/lupin_danquin/core/application.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev9/lupin_danquin/core/coding_rules_validator/coging_rules_validator.py` & `lupin-danquin-1.0.0/lupin_danquin/core/coding_rules_validator/coging_rules_validator.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,9 +26,10 @@
     def validate(self):
         """Validate coding rules"""
         result = self._check_coding_rules()
         if len(result) > 0:
             info(msg=f"{len(result)} errors found while checking coding rules")
             for error in result:
                 warn(msg=error)
+            die(msg="Coding rules not respected")
         else:
             info(msg="No error found while checking coding rules")
```

### Comparing `lupin-danquin-0.0.1.dev9/lupin_danquin/core/global_variable.py` & `lupin-danquin-1.0.0/lupin_danquin/core/global_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev9/lupin_danquin/core/local_variable.py` & `lupin-danquin-1.0.0/lupin_danquin/core/local_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev9/lupin_danquin/core/parameter.py` & `lupin-danquin-1.0.0/lupin_danquin/core/parameter.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev9/lupin_danquin/core/program.py` & `lupin-danquin-1.0.0/lupin_danquin/core/program.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev9/lupin_danquin/core/tools/utils.py` & `lupin-danquin-1.0.0/lupin_danquin/core/tools/utils.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev9/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py` & `lupin-danquin-1.0.0/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev9/lupin_danquin/run.py` & `lupin-danquin-1.0.0/lupin_danquin/run.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev9/lupin_danquin/templates/val3_documentation_md.j2` & `lupin-danquin-1.0.0/lupin_danquin/templates/val3_documentation_md.j2`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/PKG-INFO` & `lupin-danquin-1.0.0/lupin_danquin.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev9
+Version: 1.0.0
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-0.0.1.dev9/lupin_danquin.egg-info/SOURCES.txt` & `lupin-danquin-1.0.0/lupin_danquin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev9/setup.cfg` & `lupin-danquin-1.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d64 616e 7175 696e   = lupin-danquin
-00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
-00000030: 312e 6465 7639 0d0a 6465 7363 7269 7074  1.dev9..descript
-00000040: 696f 6e20 3d20 5465 7374 696e 6720 2d20  ion = Testing - 
-00000050: 446f 6375 6d65 6e74 6174 696f 6e0d 0a6c  Documentation..l
-00000060: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-00000070: 3d20 5465 7374 2056 414c 3320 636f 6465  = Test VAL3 code
-00000080: 2061 6e64 2067 656e 6572 6174 6520 646f   and generate do
-00000090: 6375 6d65 6e74 6174 696f 6e20 6672 6f6d  cumentation from
-000000a0: 2069 740d 0a6b 6579 776f 7264 7320 3d20   it..keywords = 
-000000b0: 646f 6375 6d65 6e74 6174 696f 6e2c 2074  documentation, t
-000000c0: 6573 7469 6e67 0d0a 6c69 6365 6e73 6520  esting..license 
-000000d0: 3d20 4d49 5420 4c69 6365 6e73 650d 0a63  = MIT License..c
-000000e0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
-000000f0: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
-00000100: 7573 203a 3a20 3320 2d20 416c 7068 610d  us :: 3 - Alpha.
-00000110: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
-00000120: 6e63 6520 3a3a 2049 6e66 6f72 6d61 7469  nce :: Informati
-00000130: 6f6e 2054 6563 686e 6f6c 6f67 790d 0a09  on Technology...
-00000140: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
-00000150: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
-00000160: 2054 6573 7469 6e67 0d0a 0954 6f70 6963   Testing...Topic
-00000170: 203a 3a20 446f 6375 6d65 6e74 6174 696f   :: Documentatio
-00000180: 6e0d 0a09 5072 6f67 7261 6d6d 696e 6720  n...Programming 
-00000190: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000001a0: 6f6e 203a 3a20 332e 3130 0d0a 094c 6963  on :: 3.10...Lic
-000001b0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-000001c0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-000001d0: 6e73 650d 0a0d 0a5b 6f70 7469 6f6e 735d  nse....[options]
-000001e0: 0d0a 7a69 705f 7361 6665 203d 2046 616c  ..zip_safe = Fal
-000001f0: 7365 0d0a 696e 636c 7564 655f 7061 636b  se..include_pack
-00000200: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
-00000210: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-00000220: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
-00000230: 6573 203d 203e 3d33 2e31 300d 0a69 6e73  es = >=3.10..ins
-00000240: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-00000250: 0d0a 0974 7970 6572 5b61 6c6c 5d3d 3d30  ...typer[all]==0
-00000260: 2e36 2e31 0d0a 0970 7974 686f 6e2d 646f  .6.1...python-do
-00000270: 7465 6e76 3d3d 302e 3231 2e30 0d0a 094a  tenv==0.21.0...J
-00000280: 696e 6a61 323d 3d33 2e31 2e32 0d0a 0d0a  inja2==3.1.2....
-00000290: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
-000002a0: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
-000002b0: 7363 7269 7074 7320 3d20 0d0a 0964 616e  scripts = ...dan
-000002c0: 7120 3d20 6c75 7069 6e5f 6461 6e71 7569  q = lupin_danqui
-000002d0: 6e2e 7275 6e3a 636c 690d 0a0d 0a5b 6f70  n.run:cli....[op
-000002e0: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
-000002f0: 7569 7265 5d0d 0a74 6573 7420 3d20 0d0a  uire]..test = ..
-00000300: 0970 7974 6573 743d 3d37 2e32 2e32 0d0a  .pytest==7.2.2..
-00000310: 0966 6c61 6b65 383d 3d36 2e30 2e30 0d0a  .flake8==6.0.0..
-00000320: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-00000330: 6765 732e 6669 6e64 5d0d 0a65 7863 6c75  ges.find]..exclu
-00000340: 6465 203d 200d 0a09 6c75 7069 6e5f 6461  de = ...lupin_da
-00000350: 6e71 7569 6e2e 7465 7374 732a 0d0a 0d0a  nquin.tests*....
-00000360: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000370: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000380: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 302e  ..version = 1.0.
+00000030: 300d 0a64 6573 6372 6970 7469 6f6e 203d  0..description =
+00000040: 2054 6573 7469 6e67 202d 2044 6f63 756d   Testing - Docum
+00000050: 656e 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  entation..long_d
+00000060: 6573 6372 6970 7469 6f6e 203d 2054 6573  escription = Tes
+00000070: 7420 5641 4c33 2063 6f64 6520 616e 6420  t VAL3 code and 
+00000080: 6765 6e65 7261 7465 2064 6f63 756d 656e  generate documen
+00000090: 7461 7469 6f6e 2066 726f 6d20 6974 0d0a  tation from it..
+000000a0: 6b65 7977 6f72 6473 203d 2064 6f63 756d  keywords = docum
+000000b0: 656e 7461 7469 6f6e 2c20 7465 7374 696e  entation, testin
+000000c0: 670d 0a6c 6963 656e 7365 203d 204d 4954  g..license = MIT
+000000d0: 204c 6963 656e 7365 0d0a 636c 6173 7369   License..classi
+000000e0: 6669 6572 7320 3d20 0d0a 0944 6576 656c  fiers = ...Devel
+000000f0: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+00000100: 2033 202d 2041 6c70 6861 0d0a 0949 6e74   3 - Alpha...Int
+00000110: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+00000120: 3a20 496e 666f 726d 6174 696f 6e20 5465  : Information Te
+00000130: 6368 6e6f 6c6f 6779 0d0a 0954 6f70 6963  chnology...Topic
+00000140: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
+00000150: 656c 6f70 6d65 6e74 203a 3a20 5465 7374  elopment :: Test
+00000160: 696e 670d 0a09 546f 7069 6320 3a3a 2044  ing...Topic :: D
+00000170: 6f63 756d 656e 7461 7469 6f6e 0d0a 0950  ocumentation...P
+00000180: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000190: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001a0: 2033 2e31 300d 0a09 4c69 6365 6e73 6520   3.10...License 
+000001b0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+000001c0: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
+000001d0: 0d0a 5b6f 7074 696f 6e73 5d0d 0a7a 6970  ..[options]..zip
+000001e0: 5f73 6166 6520 3d20 4661 6c73 650d 0a69  _safe = False..i
+000001f0: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+00000200: 6174 6120 3d20 5472 7565 0d0a 7061 636b  ata = True..pack
+00000210: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+00000220: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000230: 3e3d 332e 3130 0d0a 696e 7374 616c 6c5f  >=3.10..install_
+00000240: 7265 7175 6972 6573 203d 200d 0a09 7479  requires = ...ty
+00000250: 7065 725b 616c 6c5d 3d3d 302e 362e 310d  per[all]==0.6.1.
+00000260: 0a09 7079 7468 6f6e 2d64 6f74 656e 763d  ..python-dotenv=
+00000270: 3d30 2e32 312e 300d 0a09 4a69 6e6a 6132  =0.21.0...Jinja2
+00000280: 3d3d 332e 312e 320d 0a0d 0a5b 6f70 7469  ==3.1.2....[opti
+00000290: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
+000002a0: 5d0d 0a63 6f6e 736f 6c65 5f73 6372 6970  ]..console_scrip
+000002b0: 7473 203d 200d 0a09 6461 6e71 203d 206c  ts = ...danq = l
+000002c0: 7570 696e 5f64 616e 7175 696e 2e72 756e  upin_danquin.run
+000002d0: 3a63 6c69 0d0a 0d0a 5b6f 7074 696f 6e73  :cli....[options
+000002e0: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
+000002f0: 0d0a 7465 7374 203d 200d 0a09 7079 7465  ..test = ...pyte
+00000300: 7374 3d3d 372e 322e 320d 0a09 666c 616b  st==7.2.2...flak
+00000310: 6538 3d3d 362e 302e 300d 0a0d 0a5b 6f70  e8==6.0.0....[op
+00000320: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+00000330: 696e 645d 0d0a 6578 636c 7564 6520 3d20  ind]..exclude = 
+00000340: 0d0a 096c 7570 696e 5f64 616e 7175 696e  ...lupin_danquin
+00000350: 2e74 6573 7473 2a0d 0a0d 0a5b 6567 675f  .tests*....[egg_
+00000360: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000370: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000380: 300d 0a0d 0a                             0....
```

