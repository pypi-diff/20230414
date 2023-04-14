# Comparing `tmp/hackyargparser-0.10.tar.gz` & `tmp/hackyargparser-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hackyargparser-0.10.tar", last modified: Fri Apr 14 05:02:53 2023, max compression
+gzip compressed data, was "hackyargparser-0.11.tar", last modified: Fri Apr 14 05:51:15 2023, max compression
```

## Comparing `hackyargparser-0.10.tar` & `hackyargparser-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 05:02:53.428509 hackyargparser-0.10/
--rw-rw-rw-   0        0        0     1148 2023-04-14 05:02:51.000000 hackyargparser-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      145 2023-04-14 05:02:51.000000 hackyargparser-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     4685 2023-04-14 05:02:53.428509 hackyargparser-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     3833 2023-04-14 04:52:15.000000 hackyargparser-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 05:02:53.425518 hackyargparser-0.10/hackyargparser/
--rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 hackyargparser-0.10/hackyargparser/LICENSE
--rw-rw-rw-   0        0        0     3833 2023-04-14 04:52:15.000000 hackyargparser-0.10/hackyargparser/README.md
--rw-rw-rw-   0        0        0     4273 2023-04-14 04:28:31.000000 hackyargparser-0.10/hackyargparser/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-14 05:02:52.000000 hackyargparser-0.10/hackyargparser/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-04-14 05:02:52.000000 hackyargparser-0.10/hackyargparser/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-14 05:02:53.428509 hackyargparser-0.10/hackyargparser.egg-info/
--rw-rw-rw-   0        0        0     4685 2023-04-14 05:02:53.000000 hackyargparser-0.10/hackyargparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-14 05:02:53.000000 hackyargparser-0.10/hackyargparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 05:02:53.000000 hackyargparser-0.10/hackyargparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-14 05:02:53.000000 hackyargparser-0.10/hackyargparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-04-14 05:02:53.429539 hackyargparser-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-04-14 05:02:52.000000 hackyargparser-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:51:15.379812 hackyargparser-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-04-14 05:51:13.000000 hackyargparser-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      145 2023-04-14 05:51:12.000000 hackyargparser-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     4685 2023-04-14 05:51:15.379812 hackyargparser-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     3833 2023-04-14 04:52:15.000000 hackyargparser-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 05:51:15.372318 hackyargparser-0.11/hackyargparser/
+-rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 hackyargparser-0.11/hackyargparser/LICENSE
+-rw-rw-rw-   0        0        0     3833 2023-04-14 04:52:15.000000 hackyargparser-0.11/hackyargparser/README.md
+-rw-rw-rw-   0        0        0     4450 2023-04-14 05:48:51.000000 hackyargparser-0.11/hackyargparser/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 05:51:14.000000 hackyargparser-0.11/hackyargparser/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 05:51:14.000000 hackyargparser-0.11/hackyargparser/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-14 05:51:15.378302 hackyargparser-0.11/hackyargparser.egg-info/
+-rw-rw-rw-   0        0        0     4685 2023-04-14 05:51:15.000000 hackyargparser-0.11/hackyargparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-14 05:51:15.000000 hackyargparser-0.11/hackyargparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 05:51:15.000000 hackyargparser-0.11/hackyargparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 05:51:15.000000 hackyargparser-0.11/hackyargparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-04-14 05:51:15.381315 hackyargparser-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-04-14 05:51:14.000000 hackyargparser-0.11/setup.py
```

### Comparing `hackyargparser-0.10/LICENSE.rst` & `hackyargparser-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hackyargparser-0.10/PKG-INFO` & `hackyargparser-0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hackyargparser
-Version: 0.10
+Version: 0.11
 Summary: Hacky argparser - parses arguments and changes the defaults of functions
 Home-page: https://github.com/hansalemaos/hackyargparser
 Author: Johannes Fischer
 Author-email: <aulasparticularesdealemaosp@gmail.com>
 License: MIT
 Keywords: argparser
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hackyargparser-0.10/README.md` & `hackyargparser-0.11/README.md`

 * *Files identical despite different names*

### Comparing `hackyargparser-0.10/hackyargparser/LICENSE` & `hackyargparser-0.11/hackyargparser/LICENSE`

 * *Files identical despite different names*

### Comparing `hackyargparser-0.10/hackyargparser/README.md` & `hackyargparser-0.11/hackyargparser/README.md`

 * *Files identical despite different names*

### Comparing `hackyargparser-0.10/hackyargparser/__init__.py` & `hackyargparser-0.11/hackyargparser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,20 +96,23 @@
                         conva = literal_eval(config.parsedargs[a])
                         if type(conva) in allanotdict[a].__args__:
                             dtypegood = True
                     except Exception:
                         pass
 
                     if not dtypegood:
-                        for dty in allanotdict[a].__args__:
-                            try:
-                                conva = dty(config.parsedargs[a])
-                                break
-                            except Exception as fe:
-                                continue
+                        try:
+                            for dty in allanotdict[a].__args__:
+                                try:
+                                    conva = dty(config.parsedargs[a])
+                                    break
+                                except Exception as fe:
+                                    continue
+                        except Exception as fa:
+                            conva = allanotdict[a](config.parsedargs[a])
                     newargs.append(conva)
                 except Exception as adf:
                     newargs.append(b)
                     continue
 
             setattr(
                 dct[func.__name__].__dict__["__wrapped__"],
```

### Comparing `hackyargparser-0.10/hackyargparser.egg-info/PKG-INFO` & `hackyargparser-0.11/hackyargparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hackyargparser
-Version: 0.10
+Version: 0.11
 Summary: Hacky argparser - parses arguments and changes the defaults of functions
 Home-page: https://github.com/hansalemaos/hackyargparser
 Author: Johannes Fischer
 Author-email: <aulasparticularesdealemaosp@gmail.com>
 License: MIT
 Keywords: argparser
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hackyargparser-0.10/setup.py` & `hackyargparser-0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #change to dict
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.10'
+VERSION = '0.11'
 DESCRIPTION = "Hacky argparser - parses arguments and changes the defaults of functions"
 
 # Setting up
 setup(
     name="hackyargparser",
     version=VERSION,
     license='MIT',
```

