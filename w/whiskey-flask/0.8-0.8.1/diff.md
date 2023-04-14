# Comparing `tmp/whiskey-flask-0.8.tar.gz` & `tmp/whiskey-flask-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whiskey-flask-0.8.tar", last modified: Wed Mar 29 00:45:04 2023, max compression
+gzip compressed data, was "whiskey-flask-0.8.1.tar", last modified: Fri Apr 14 18:16:51 2023, max compression
```

## Comparing `whiskey-flask-0.8.tar` & `whiskey-flask-0.8.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-03-29 00:45:04.888084 whiskey-flask-0.8/
--rw-r--r--   0 nick       (501) staff       (20)     1065 2023-03-29 00:45:04.888434 whiskey-flask-0.8/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      793 2021-12-21 22:34:04.000000 whiskey-flask-0.8/README.md
--rw-r--r--   0 nick       (501) staff       (20)       78 2023-03-29 00:45:04.889454 whiskey-flask-0.8/setup.cfg
--rw-r--r--   0 nick       (501) staff       (20)     1066 2023-03-29 00:44:18.000000 whiskey-flask-0.8/setup.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-03-29 00:45:04.881284 whiskey-flask-0.8/whiskey/
--rw-r--r--   0 nick       (501) staff       (20)      724 2023-01-05 22:22:19.000000 whiskey-flask-0.8/whiskey/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     2046 2022-10-03 14:56:43.000000 whiskey-flask-0.8/whiskey/commands.py
--rw-r--r--   0 nick       (501) staff       (20)     6737 2022-12-01 13:36:37.000000 whiskey-flask-0.8/whiskey/feeds.py
--rw-r--r--   0 nick       (501) staff       (20)     2695 2021-12-21 22:34:04.000000 whiskey-flask-0.8/whiskey/flatpandoc.py
--rw-r--r--   0 nick       (501) staff       (20)      587 2021-12-21 22:34:04.000000 whiskey-flask-0.8/whiskey/formatter.py
--rw-r--r--   0 nick       (501) staff       (20)      642 2021-12-22 15:54:07.000000 whiskey-flask-0.8/whiskey/freeze.py
--rw-r--r--   0 nick       (501) staff       (20)     5747 2023-01-05 20:45:06.000000 whiskey-flask-0.8/whiskey/helpers.py
--rw-r--r--   0 nick       (501) staff       (20)      890 2021-12-21 22:34:04.000000 whiskey-flask-0.8/whiskey/settings.py
--rw-r--r--   0 nick       (501) staff       (20)     2031 2022-04-28 01:52:46.000000 whiskey-flask-0.8/whiskey/tasks.py
--rw-r--r--   0 nick       (501) staff       (20)      420 2022-12-07 12:48:07.000000 whiskey-flask-0.8/whiskey/templates.py
--rw-r--r--   0 nick       (501) staff       (20)     8330 2023-03-28 23:06:28.000000 whiskey-flask-0.8/whiskey/views.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-03-29 00:45:04.886892 whiskey-flask-0.8/whiskey_flask.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)     1065 2023-03-29 00:45:04.000000 whiskey-flask-0.8/whiskey_flask.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)      460 2023-03-29 00:45:04.000000 whiskey-flask-0.8/whiskey_flask.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2023-03-29 00:45:04.000000 whiskey-flask-0.8/whiskey_flask.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2021-12-21 22:51:35.000000 whiskey-flask-0.8/whiskey_flask.egg-info/not-zip-safe
--rw-r--r--   0 nick       (501) staff       (20)      158 2023-03-29 00:45:04.000000 whiskey-flask-0.8/whiskey_flask.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)        8 2023-03-29 00:45:04.000000 whiskey-flask-0.8/whiskey_flask.egg-info/top_level.txt
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-14 18:16:51.587756 whiskey-flask-0.8.1/
+-rw-r--r--   0 nick       (501) staff       (20)     1067 2023-04-14 18:16:51.587977 whiskey-flask-0.8.1/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)      793 2021-12-21 22:34:04.000000 whiskey-flask-0.8.1/README.md
+-rw-r--r--   0 nick       (501) staff       (20)       78 2023-04-14 18:16:51.588716 whiskey-flask-0.8.1/setup.cfg
+-rw-r--r--   0 nick       (501) staff       (20)     1068 2023-04-14 18:16:36.000000 whiskey-flask-0.8.1/setup.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-14 18:16:51.583808 whiskey-flask-0.8.1/whiskey/
+-rw-r--r--   0 nick       (501) staff       (20)      724 2023-01-05 22:22:19.000000 whiskey-flask-0.8.1/whiskey/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     2046 2022-10-03 14:56:43.000000 whiskey-flask-0.8.1/whiskey/commands.py
+-rw-r--r--   0 nick       (501) staff       (20)     6737 2022-12-01 13:36:37.000000 whiskey-flask-0.8.1/whiskey/feeds.py
+-rw-r--r--   0 nick       (501) staff       (20)     2695 2021-12-21 22:34:04.000000 whiskey-flask-0.8.1/whiskey/flatpandoc.py
+-rw-r--r--   0 nick       (501) staff       (20)      587 2021-12-21 22:34:04.000000 whiskey-flask-0.8.1/whiskey/formatter.py
+-rw-r--r--   0 nick       (501) staff       (20)      642 2021-12-22 15:54:07.000000 whiskey-flask-0.8.1/whiskey/freeze.py
+-rw-r--r--   0 nick       (501) staff       (20)     5747 2023-01-05 20:45:06.000000 whiskey-flask-0.8.1/whiskey/helpers.py
+-rw-r--r--   0 nick       (501) staff       (20)      890 2021-12-21 22:34:04.000000 whiskey-flask-0.8.1/whiskey/settings.py
+-rw-r--r--   0 nick       (501) staff       (20)     2031 2022-04-28 01:52:46.000000 whiskey-flask-0.8.1/whiskey/tasks.py
+-rw-r--r--   0 nick       (501) staff       (20)      420 2022-12-07 12:48:07.000000 whiskey-flask-0.8.1/whiskey/templates.py
+-rw-r--r--   0 nick       (501) staff       (20)     8286 2023-04-14 18:16:22.000000 whiskey-flask-0.8.1/whiskey/views.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2023-04-14 18:16:51.587406 whiskey-flask-0.8.1/whiskey_flask.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)     1067 2023-04-14 18:16:50.000000 whiskey-flask-0.8.1/whiskey_flask.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)      460 2023-04-14 18:16:51.000000 whiskey-flask-0.8.1/whiskey_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2023-04-14 18:16:50.000000 whiskey-flask-0.8.1/whiskey_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2021-12-21 22:51:35.000000 whiskey-flask-0.8.1/whiskey_flask.egg-info/not-zip-safe
+-rw-r--r--   0 nick       (501) staff       (20)      158 2023-04-14 18:16:51.000000 whiskey-flask-0.8.1/whiskey_flask.egg-info/requires.txt
+-rw-r--r--   0 nick       (501) staff       (20)        8 2023-04-14 18:16:51.000000 whiskey-flask-0.8.1/whiskey_flask.egg-info/top_level.txt
```

### Comparing `whiskey-flask-0.8/PKG-INFO` & `whiskey-flask-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiskey-flask
-Version: 0.8
+Version: 0.8.1
 Summary: Whiskey makes writing happen.
 Home-page: https://github.com/nickwynja/whiskey
 Author: Nick Wynja
 Author-email: nick@nickwynja.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `whiskey-flask-0.8/README.md` & `whiskey-flask-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `whiskey-flask-0.8/setup.py` & `whiskey-flask-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='whiskey-flask',
-    version='0.8',
+    version='0.8.1',
     author="Nick Wynja",
     author_email="nick@nickwynja.com",
     description="Whiskey makes writing happen.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nickwynja/whiskey",
     packages=find_packages(),
```

### Comparing `whiskey-flask-0.8/whiskey/__init__.py` & `whiskey-flask-0.8.1/whiskey/__init__.py`

 * *Files identical despite different names*

### Comparing `whiskey-flask-0.8/whiskey/commands.py` & `whiskey-flask-0.8.1/whiskey/commands.py`

 * *Files identical despite different names*

### Comparing `whiskey-flask-0.8/whiskey/feeds.py` & `whiskey-flask-0.8.1/whiskey/feeds.py`

 * *Files identical despite different names*

### Comparing `whiskey-flask-0.8/whiskey/flatpandoc.py` & `whiskey-flask-0.8.1/whiskey/flatpandoc.py`

 * *Files identical despite different names*

### Comparing `whiskey-flask-0.8/whiskey/formatter.py` & `whiskey-flask-0.8.1/whiskey/formatter.py`

 * *Files identical despite different names*

### Comparing `whiskey-flask-0.8/whiskey/freeze.py` & `whiskey-flask-0.8.1/whiskey/freeze.py`

 * *Files identical despite different names*

### Comparing `whiskey-flask-0.8/whiskey/helpers.py` & `whiskey-flask-0.8.1/whiskey/helpers.py`

 * *Files identical despite different names*

### Comparing `whiskey-flask-0.8/whiskey/settings.py` & `whiskey-flask-0.8.1/whiskey/settings.py`

 * *Files identical despite different names*

### Comparing `whiskey-flask-0.8/whiskey/tasks.py` & `whiskey-flask-0.8.1/whiskey/tasks.py`

 * *Files identical despite different names*

### Comparing `whiskey-flask-0.8/whiskey/views.py` & `whiskey-flask-0.8.1/whiskey/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,20 +152,18 @@
                 )
         return send_from_directory(
             app.config['CONTENT_PATH'], '%s.%s' % (name, "pdf")
         )
     elif ext in ['txt', 'md']:
         file = '{}/{}.{}'.format(app.config['CONTENT_PATH'], name, ext)
         return helpers.get_flatfile_or_404(file)
-    elif ext == "pdf":
+    else:
         return send_from_directory(
-            app.config['CONTENT_PATH'], '%s.%s' % (name, "pdf")
+            app.config['CONTENT_PATH'], '%s.%s' % (name, ext)
         )
-    else:
-        abort(404)
 
 
 if app.config['SITE_STYLE'] in ("blog", "hybrid"):
 
     @app.route("/updates.html")
     def updates():
         updates = reversed(helpers.get_updates())
```

### Comparing `whiskey-flask-0.8/whiskey_flask.egg-info/PKG-INFO` & `whiskey-flask-0.8.1/whiskey_flask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiskey-flask
-Version: 0.8
+Version: 0.8.1
 Summary: Whiskey makes writing happen.
 Home-page: https://github.com/nickwynja/whiskey
 Author: Nick Wynja
 Author-email: nick@nickwynja.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

