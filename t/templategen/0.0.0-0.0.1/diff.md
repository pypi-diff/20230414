# Comparing `tmp/templategen-0.0.0.tar.gz` & `tmp/templategen-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/templategen-0.0.0.tar", last modified: Fri Apr 14 13:38:43 2023, max compression
+gzip compressed data, was "dist/templategen-0.0.1.tar", last modified: Fri Apr 14 14:50:45 2023, max compression
```

## Comparing `templategen-0.0.0.tar` & `templategen-0.0.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 13:38:43.000000 templategen-0.0.0/
--rw-rw-r--   0 tedi      (1000) tedi      (1000)       42 2023-04-14 11:36:12.000000 templategen-0.0.0/.gitignore
--rw-rw-r--   0 tedi      (1000) tedi      (1000)     1870 2023-04-14 13:38:43.000000 templategen-0.0.0/PKG-INFO
-drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 13:38:43.000000 templategen-0.0.0/images/
--rw-rw-r--   0 tedi      (1000) tedi      (1000)     5018 2023-04-14 08:56:30.000000 templategen-0.0.0/images/logo.jpeg
-drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 13:38:43.000000 templategen-0.0.0/templategen.egg-info/
--rw-rw-r--   0 tedi      (1000) tedi      (1000)     1870 2023-04-14 13:38:43.000000 templategen-0.0.0/templategen.egg-info/PKG-INFO
--rw-rw-r--   0 tedi      (1000) tedi      (1000)       57 2023-04-14 13:38:43.000000 templategen-0.0.0/templategen.egg-info/entry_points.txt
--rw-rw-r--   0 tedi      (1000) tedi      (1000)        1 2023-04-14 13:38:43.000000 templategen-0.0.0/templategen.egg-info/dependency_links.txt
--rw-rw-r--   0 tedi      (1000) tedi      (1000)      670 2023-04-14 13:38:43.000000 templategen-0.0.0/templategen.egg-info/SOURCES.txt
--rw-rw-r--   0 tedi      (1000) tedi      (1000)       12 2023-04-14 13:38:43.000000 templategen-0.0.0/templategen.egg-info/top_level.txt
--rw-rw-r--   0 tedi      (1000) tedi      (1000)       12 2023-04-14 13:38:43.000000 templategen-0.0.0/templategen.egg-info/requires.txt
--rw-rw-r--   0 tedi      (1000) tedi      (1000)       12 2023-04-14 08:42:25.000000 templategen-0.0.0/requirements.txt
-drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 13:38:43.000000 templategen-0.0.0/templategen/
--rw-rw-r--   0 tedi      (1000) tedi      (1000)     2674 2023-04-14 13:23:23.000000 templategen-0.0.0/templategen/utils.py
--rwxrwxr-x   0 tedi      (1000) tedi      (1000)     4406 2023-04-14 13:24:29.000000 templategen-0.0.0/templategen/app.py
--rw-rw-r--   0 tedi      (1000) tedi      (1000)      108 2023-04-14 11:16:04.000000 templategen-0.0.0/templategen/__main__.py
--rw-rw-r--   0 tedi      (1000) tedi      (1000)      409 2023-04-14 11:16:04.000000 templategen-0.0.0/templategen/__init__.py
--rwxrwxr-x   0 tedi      (1000) tedi      (1000)     2574 2023-04-14 11:49:34.000000 templategen-0.0.0/setup.py
--rw-rw-r--   0 tedi      (1000) tedi      (1000)      379 2023-04-14 11:24:06.000000 templategen-0.0.0/Makefile
--rw-rw-r--   0 tedi      (1000) tedi      (1000)       38 2023-04-14 13:38:43.000000 templategen-0.0.0/setup.cfg
-drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 13:38:43.000000 templategen-0.0.0/static/
--rw-rw-r--   0 tedi      (1000) tedi      (1000)       62 2023-04-14 11:55:24.000000 templategen-0.0.0/static/config.json
-drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 13:38:43.000000 templategen-0.0.0/static/templates/
-drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 13:38:43.000000 templategen-0.0.0/static/templates/python/
--rwxrwxr-x   0 tedi      (1000) tedi      (1000)      208 2023-04-14 12:33:39.000000 templategen-0.0.0/static/templates/python/template.py
-drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 13:38:43.000000 templategen-0.0.0/static/templates/c/
--rwxrwxr-x   0 tedi      (1000) tedi      (1000)     2483 2023-04-14 08:00:33.000000 templategen-0.0.0/static/templates/c/template.c
--rwxrwxr-x   0 tedi      (1000) tedi      (1000)     2649 2023-04-14 07:56:28.000000 templategen-0.0.0/static/templates/c/template.h
--rw-rw-r--   0 tedi      (1000) tedi      (1000)     1129 2023-04-14 13:34:50.000000 templategen-0.0.0/README.md
--rw-rw-r--   0 tedi      (1000) tedi      (1000)    35141 2023-04-12 19:35:00.000000 templategen-0.0.0/LICENSE
+drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 14:50:45.000000 templategen-0.0.1/
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)       42 2023-04-14 11:36:12.000000 templategen-0.0.1/.gitignore
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)     1870 2023-04-14 14:50:45.000000 templategen-0.0.1/PKG-INFO
+drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 14:50:45.000000 templategen-0.0.1/images/
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)     5018 2023-04-14 08:56:30.000000 templategen-0.0.1/images/logo.jpeg
+drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 14:50:45.000000 templategen-0.0.1/templategen.egg-info/
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)     1870 2023-04-14 14:50:44.000000 templategen-0.0.1/templategen.egg-info/PKG-INFO
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)       57 2023-04-14 14:50:44.000000 templategen-0.0.1/templategen.egg-info/entry_points.txt
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)        1 2023-04-14 14:50:44.000000 templategen-0.0.1/templategen.egg-info/dependency_links.txt
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)      681 2023-04-14 14:50:44.000000 templategen-0.0.1/templategen.egg-info/SOURCES.txt
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)       12 2023-04-14 14:50:44.000000 templategen-0.0.1/templategen.egg-info/top_level.txt
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)       12 2023-04-14 14:50:44.000000 templategen-0.0.1/templategen.egg-info/requires.txt
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)       12 2023-04-14 08:42:25.000000 templategen-0.0.1/requirements.txt
+drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 14:50:45.000000 templategen-0.0.1/templategen/
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)     2674 2023-04-14 13:23:23.000000 templategen-0.0.1/templategen/utils.py
+-rwxrwxr-x   0 tedi      (1000) tedi      (1000)     4501 2023-04-14 14:25:18.000000 templategen-0.0.1/templategen/app.py
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)      108 2023-04-14 11:16:04.000000 templategen-0.0.1/templategen/__main__.py
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)      409 2023-04-14 11:16:04.000000 templategen-0.0.1/templategen/__init__.py
+-rwxrwxr-x   0 tedi      (1000) tedi      (1000)     2574 2023-04-14 14:50:42.000000 templategen-0.0.1/setup.py
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)      379 2023-04-14 11:24:06.000000 templategen-0.0.1/Makefile
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)       38 2023-04-14 14:50:45.000000 templategen-0.0.1/setup.cfg
+drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 14:50:45.000000 templategen-0.0.1/static/
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)       62 2023-04-14 11:55:24.000000 templategen-0.0.1/static/config.json
+drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 14:50:45.000000 templategen-0.0.1/static/templates/
+drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 14:50:45.000000 templategen-0.0.1/static/templates/python/
+-rwxrwxr-x   0 tedi      (1000) tedi      (1000)      208 2023-04-14 12:33:39.000000 templategen-0.0.1/static/templates/python/template.py
+drwxrwxr-x   0 tedi      (1000) tedi      (1000)        0 2023-04-14 14:50:45.000000 templategen-0.0.1/static/templates/c/
+-rwxrwxr-x   0 tedi      (1000) tedi      (1000)     2483 2023-04-14 08:00:33.000000 templategen-0.0.1/static/templates/c/template.c
+-rwxrwxr-x   0 tedi      (1000) tedi      (1000)     2649 2023-04-14 07:56:28.000000 templategen-0.0.1/static/templates/c/template.h
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)      376 2023-04-14 14:15:19.000000 templategen-0.0.1/.drone.yml
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)     1129 2023-04-14 13:34:50.000000 templategen-0.0.1/README.md
+-rw-rw-r--   0 tedi      (1000) tedi      (1000)    35141 2023-04-12 19:35:00.000000 templategen-0.0.1/LICENSE
```

### Comparing `templategen-0.0.0/PKG-INFO` & `templategen-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templategen
-Version: 0.0.0
+Version: 0.0.1
 Summary: Souce code generator from a given template
 Home-page: https://github.com/TediCreations/templategen
 Author: Kanelis Elias
 Author-email: hkanelhs@yahoo.gr
 License: MIT
 Download-URL: https://github.com/TediCreations/templategen/archive/Unknown.tar.gz
 Keywords: build,make,util
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: templategen Version: 0.0.0 Summary: Souce code
+Metadata-Version: 2.1 Name: templategen Version: 0.0.1 Summary: Souce code
 generator from a given template Home-page: https://github.com/TediCreations/
 templategen Author: Kanelis Elias Author-email: hkanelhs@yahoo.gr License: MIT
 Download-URL: https://github.com/TediCreations/templategen/archive/
 Unknown.tar.gz Keywords: build,make,util Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
```

### Comparing `templategen-0.0.0/images/logo.jpeg` & `templategen-0.0.1/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `templategen-0.0.0/templategen.egg-info/PKG-INFO` & `templategen-0.0.1/templategen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templategen
-Version: 0.0.0
+Version: 0.0.1
 Summary: Souce code generator from a given template
 Home-page: https://github.com/TediCreations/templategen
 Author: Kanelis Elias
 Author-email: hkanelhs@yahoo.gr
 License: MIT
 Download-URL: https://github.com/TediCreations/templategen/archive/Unknown.tar.gz
 Keywords: build,make,util
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: templategen Version: 0.0.0 Summary: Souce code
+Metadata-Version: 2.1 Name: templategen Version: 0.0.1 Summary: Souce code
 generator from a given template Home-page: https://github.com/TediCreations/
 templategen Author: Kanelis Elias Author-email: hkanelhs@yahoo.gr License: MIT
 Download-URL: https://github.com/TediCreations/templategen/archive/
 Unknown.tar.gz Keywords: build,make,util Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
```

### Comparing `templategen-0.0.0/templategen.egg-info/SOURCES.txt` & `templategen-0.0.1/templategen.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.drone.yml
 .gitignore
 LICENSE
 Makefile
 README.md
 requirements.txt
 setup.py
 images/logo.jpeg
```

### Comparing `templategen-0.0.0/templategen/utils.py` & `templategen-0.0.1/templategen/utils.py`

 * *Files identical despite different names*

### Comparing `templategen-0.0.0/templategen/app.py` & `templategen-0.0.1/templategen/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,18 @@
             print(f"Template file '{template_filepath}' does not exist")
             sys.exit(1)
 
 
 def app_run():
     """Entry point for the app."""
     # -------------------------------------------------------------------------
+    # Prepare
+    create_config_if_missing()
+
+    # -------------------------------------------------------------------------
     # Arguments
     templates = list_templates()
 
     parser = argparse.ArgumentParser(
         description='Source code template generator')
     parser.add_argument('-n',
                         '--name',
@@ -115,13 +119,12 @@
     name = args.name
     target_dirpath = os.path.abspath(args.path)
     template_name = args.template
 
     # -------------------------------------------------------------------------
     # Generate
 
-    create_config_if_missing()
     generate(name, template_name, target_dirpath)
 
 
 if __name__ == "__main__":
     app_run()
```

### Comparing `templategen-0.0.0/setup.py` & `templategen-0.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `templategen-0.0.0/static/templates/c/template.c` & `templategen-0.0.1/static/templates/c/template.c`

 * *Files identical despite different names*

### Comparing `templategen-0.0.0/static/templates/c/template.h` & `templategen-0.0.1/static/templates/c/template.h`

 * *Files identical despite different names*

### Comparing `templategen-0.0.0/README.md` & `templategen-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `templategen-0.0.0/LICENSE` & `templategen-0.0.1/LICENSE`

 * *Files identical despite different names*

