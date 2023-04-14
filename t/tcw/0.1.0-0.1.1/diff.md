# Comparing `tmp/tcw-0.1.0.tar.gz` & `tmp/tcw-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcw-0.1.0.tar", last modified: Thu Apr 13 11:26:27 2023, max compression
+gzip compressed data, was "tcw-0.1.1.tar", last modified: Fri Apr 14 11:52:47 2023, max compression
```

## Comparing `tcw-0.1.0.tar` & `tcw-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1060 2022-12-16 20:39:46.000000 tcw-0.1.0/LICENSE
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-04-13 11:26:27.403007 tcw-0.1.0/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1029 2022-12-16 20:39:46.000000 tcw-0.1.0/README.md
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-04-13 11:26:27.403007 tcw-0.1.0/setup.cfg
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      544 2023-04-13 11:12:51.000000 tcw-0.1.0/setup.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1615 2022-12-21 05:31:36.000000 tcw-0.1.0/tcw/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/apps/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/apps/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/apps/contest/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/apps/contest/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1131 2022-12-17 03:59:32.000000 tcw-0.1.0/tcw/apps/contest/forms.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3534 2023-01-01 20:54:30.000000 tcw-0.1.0/tcw/apps/contest/models.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/apps/contest/templates/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/apps/contest/templates/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/apps/contest/templates/contest/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/apps/contest/templates/contest/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     3313 2023-01-21 12:31:08.000000 tcw-0.1.0/tcw/apps/contest/views.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1198 2022-12-18 22:49:28.000000 tcw-0.1.0/tcw/config.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1081 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/database.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      166 2023-04-13 11:23:23.000000 tcw-0.1.0/tcw/run.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      171 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/srv.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/static/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/static/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/static/images/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/static/images/__init__.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw/templates/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.0/tcw/templates/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1568 2022-12-21 05:40:29.000000 tcw-0.1.0/tcw/utils.py
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-13 11:26:27.403007 tcw-0.1.0/tcw.egg-info/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-04-13 11:26:27.000000 tcw-0.1.0/tcw.egg-info/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      535 2023-04-13 11:26:27.000000 tcw-0.1.0/tcw.egg-info/SOURCES.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-04-13 11:26:27.000000 tcw-0.1.0/tcw.egg-info/dependency_links.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)       36 2023-04-13 11:26:27.000000 tcw-0.1.0/tcw.egg-info/requires.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        4 2023-04-13 11:26:27.000000 tcw-0.1.0/tcw.egg-info/top_level.txt
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-14 11:52:47.745005 tcw-0.1.1/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1060 2022-12-16 20:39:46.000000 tcw-0.1.1/LICENSE
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-04-14 11:52:47.745005 tcw-0.1.1/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1029 2022-12-16 20:39:46.000000 tcw-0.1.1/README.md
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       38 2023-04-14 11:52:47.745005 tcw-0.1.1/setup.cfg
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      544 2023-04-14 11:47:13.000000 tcw-0.1.1/setup.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-14 11:52:47.741006 tcw-0.1.1/tcw/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1668 2023-04-14 11:48:11.000000 tcw-0.1.1/tcw/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-14 11:52:47.745005 tcw-0.1.1/tcw/apps/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.1/tcw/apps/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-14 11:52:47.745005 tcw-0.1.1/tcw/apps/contest/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.1/tcw/apps/contest/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1131 2022-12-17 03:59:32.000000 tcw-0.1.1/tcw/apps/contest/forms.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3534 2023-01-01 20:54:30.000000 tcw-0.1.1/tcw/apps/contest/models.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-14 11:52:47.745005 tcw-0.1.1/tcw/apps/contest/templates/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.1/tcw/apps/contest/templates/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-14 11:52:47.745005 tcw-0.1.1/tcw/apps/contest/templates/contest/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.1/tcw/apps/contest/templates/contest/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     3313 2023-01-21 12:31:08.000000 tcw-0.1.1/tcw/apps/contest/views.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1198 2022-12-18 22:49:28.000000 tcw-0.1.1/tcw/config.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1081 2022-12-16 20:39:46.000000 tcw-0.1.1/tcw/database.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      171 2023-04-14 11:51:00.000000 tcw-0.1.1/tcw/run.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-14 11:52:47.745005 tcw-0.1.1/tcw/static/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.1/tcw/static/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-14 11:52:47.745005 tcw-0.1.1/tcw/static/images/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.1/tcw/static/images/__init__.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-14 11:52:47.745005 tcw-0.1.1/tcw/templates/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        0 2022-12-16 20:39:46.000000 tcw-0.1.1/tcw/templates/__init__.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1568 2022-12-21 05:40:29.000000 tcw-0.1.1/tcw/utils.py
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      186 2023-04-14 11:50:36.000000 tcw-0.1.1/tcw/wsgi.py
+drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2023-04-14 11:52:47.745005 tcw-0.1.1/tcw.egg-info/
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)     1240 2023-04-14 11:52:47.000000 tcw-0.1.1/tcw.egg-info/PKG-INFO
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)      536 2023-04-14 11:52:47.000000 tcw-0.1.1/tcw.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2023-04-14 11:52:47.000000 tcw-0.1.1/tcw.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)       36 2023-04-14 11:52:47.000000 tcw-0.1.1/tcw.egg-info/requires.txt
+-rw-rw-r--   0 jeff      (1000) jeff      (1000)        4 2023-04-14 11:52:47.000000 tcw-0.1.1/tcw.egg-info/top_level.txt
```

### Comparing `tcw-0.1.0/LICENSE` & `tcw-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcw-0.1.0/PKG-INFO` & `tcw-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcw
-Version: 0.1.0
+Version: 0.1.1
 Summary: tiny contest winners application
 Author: J Leary
 Author-email: tinycontestwinners@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TCW: Tiny Contest Winners
```

### Comparing `tcw-0.1.0/README.md` & `tcw-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tcw-0.1.0/setup.py` & `tcw-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='tcw',
-    version='0.1.0',
+    version='0.1.1',
     author='J Leary',
     author_email='tinycontestwinners@gmail.com',
     description='tiny contest winners application',
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
     packages=find_packages(),
```

### Comparing `tcw-0.1.0/tcw/__init__.py` & `tcw-0.1.1/tcw/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 from tcw.config import Development, Production
 from tcw.database import init_db
 
 
 BASEDIR = os.path.abspath(os.path.dirname(__file__))
 
 
-def create_app(name='tiny contest winners', config=None):
+def create_app(name='tiny contest winners', config=None, root=None):
     """
     Create the Flask app
 
     args:
         - name
         - config object
     """
 
     if config is None:
         config = Development
 
-    app = Flask(name, root_path=BASEDIR)
+    if root is None:
+        root = BASEDIR
+
+    app = Flask(name, root_path=root)
     configure_app(app, config)
     load_filters(app)
     load_handlers(app)
     load_blueprints(app)
     load_views()
 
     return app
```

### Comparing `tcw-0.1.0/tcw/apps/contest/forms.py` & `tcw-0.1.1/tcw/apps/contest/forms.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.0/tcw/apps/contest/models.py` & `tcw-0.1.1/tcw/apps/contest/models.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.0/tcw/apps/contest/views.py` & `tcw-0.1.1/tcw/apps/contest/views.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.0/tcw/config.py` & `tcw-0.1.1/tcw/config.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.0/tcw/database.py` & `tcw-0.1.1/tcw/database.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.0/tcw/utils.py` & `tcw-0.1.1/tcw/utils.py`

 * *Files identical despite different names*

### Comparing `tcw-0.1.0/tcw.egg-info/PKG-INFO` & `tcw-0.1.1/tcw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcw
-Version: 0.1.0
+Version: 0.1.1
 Summary: tiny contest winners application
 Author: J Leary
 Author-email: tinycontestwinners@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TCW: Tiny Contest Winners
```

### Comparing `tcw-0.1.0/tcw.egg-info/SOURCES.txt` & `tcw-0.1.1/tcw.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 README.md
 setup.py
 tcw/__init__.py
 tcw/config.py
 tcw/database.py
 tcw/run.py
-tcw/srv.py
 tcw/utils.py
+tcw/wsgi.py
 tcw.egg-info/PKG-INFO
 tcw.egg-info/SOURCES.txt
 tcw.egg-info/dependency_links.txt
 tcw.egg-info/requires.txt
 tcw.egg-info/top_level.txt
 tcw/apps/__init__.py
 tcw/apps/contest/__init__.py
```

