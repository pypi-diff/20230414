# Comparing `tmp/django-vite-react-0.0.1.tar.gz` & `tmp/django-vite-react-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vite-react-0.0.1.tar", last modified: Fri Apr 14 06:25:26 2023, max compression
+gzip compressed data, was "django-vite-react-0.0.2.tar", last modified: Fri Apr 14 06:37:20 2023, max compression
```

## Comparing `django-vite-react-0.0.1.tar` & `django-vite-react-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:25:26.961453 django-vite-react-0.0.1/
--rw-r--r--   0 chen      (1000) chen      (1000)     1063 2022-05-11 08:46:06.000000 django-vite-react-0.0.1/LICENSE
--rw-r--r--   0 chen      (1000) chen      (1000)      141 2023-04-14 06:09:06.000000 django-vite-react-0.0.1/MANIFEST.in
--rw-r--r--   0 chen      (1000) chen      (1000)     3176 2023-04-14 06:25:26.961453 django-vite-react-0.0.1/PKG-INFO
--rw-r--r--   0 chen      (1000) chen      (1000)     2291 2023-04-14 06:25:21.000000 django-vite-react-0.0.1/README.rst
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:25:26.961453 django-vite-react-0.0.1/django_vite_react.egg-info/
--rw-r--r--   0 chen      (1000) chen      (1000)     3176 2023-04-14 06:25:26.000000 django-vite-react-0.0.1/django_vite_react.egg-info/PKG-INFO
--rw-r--r--   0 chen      (1000) chen      (1000)      520 2023-04-14 06:25:26.000000 django-vite-react-0.0.1/django_vite_react.egg-info/SOURCES.txt
--rw-r--r--   0 chen      (1000) chen      (1000)        1 2023-04-14 06:25:26.000000 django-vite-react-0.0.1/django_vite_react.egg-info/dependency_links.txt
--rw-r--r--   0 chen      (1000) chen      (1000)       12 2023-04-14 06:25:26.000000 django-vite-react-0.0.1/django_vite_react.egg-info/requires.txt
--rw-r--r--   0 chen      (1000) chen      (1000)        6 2023-04-14 06:25:26.000000 django-vite-react-0.0.1/django_vite_react.egg-info/top_level.txt
--rw-r--r--   0 chen      (1000) chen      (1000)      108 2023-04-14 06:04:51.000000 django-vite-react-0.0.1/pyproject.toml
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:25:26.961453 django-vite-react-0.0.1/react/
--rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-11 08:44:48.000000 django-vite-react-0.0.1/react/__init__.py
--rw-r--r--   0 chen      (1000) chen      (1000)       63 2022-05-11 08:44:48.000000 django-vite-react-0.0.1/react/admin.py
--rw-r--r--   0 chen      (1000) chen      (1000)      142 2022-05-11 08:44:48.000000 django-vite-react-0.0.1/react/apps.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:25:26.961453 django-vite-react-0.0.1/react/components/
--rw-r--r--   0 chen      (1000) chen      (1000)      280 2022-05-11 08:44:48.000000 django-vite-react-0.0.1/react/components/app.jsx
--rw-r--r--   0 chen      (1000) chen      (1000)      370 2022-05-11 08:44:48.000000 django-vite-react-0.0.1/react/generic.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:25:26.961453 django-vite-react-0.0.1/react/migrations/
--rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-11 08:44:48.000000 django-vite-react-0.0.1/react/migrations/__init__.py
--rw-r--r--   0 chen      (1000) chen      (1000)      442 2022-05-12 03:05:04.000000 django-vite-react-0.0.1/react/mixins.py
--rw-r--r--   0 chen      (1000) chen      (1000)       57 2022-05-11 08:44:48.000000 django-vite-react-0.0.1/react/models.py
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:25:26.958120 django-vite-react-0.0.1/react/templates/
-drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:25:26.961453 django-vite-react-0.0.1/react/templates/react/
--rw-r--r--   0 chen      (1000) chen      (1000)      288 2022-05-12 03:04:03.000000 django-vite-react-0.0.1/react/templates/react/react.html
--rw-r--r--   0 chen      (1000) chen      (1000)      182 2022-05-12 03:04:09.000000 django-vite-react-0.0.1/react/templates/react/react_props.html
--rw-r--r--   0 chen      (1000) chen      (1000)       60 2022-05-11 08:44:48.000000 django-vite-react-0.0.1/react/tests.py
--rw-r--r--   0 chen      (1000) chen      (1000)       63 2022-05-11 08:44:48.000000 django-vite-react-0.0.1/react/views.py
--rw-r--r--   0 chen      (1000) chen      (1000)      895 2023-04-14 06:25:26.961453 django-vite-react-0.0.1/setup.cfg
--rw-r--r--   0 chen      (1000) chen      (1000)       38 2023-04-14 06:07:50.000000 django-vite-react-0.0.1/setup.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/
+-rw-r--r--   0 chen      (1000) chen      (1000)     1063 2022-05-11 08:46:06.000000 django-vite-react-0.0.2/LICENSE
+-rw-r--r--   0 chen      (1000) chen      (1000)      141 2023-04-14 06:09:06.000000 django-vite-react-0.0.2/MANIFEST.in
+-rw-r--r--   0 chen      (1000) chen      (1000)     3176 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/PKG-INFO
+-rw-r--r--   0 chen      (1000) chen      (1000)     2291 2023-04-14 06:25:21.000000 django-vite-react-0.0.2/README.rst
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/django_vite_react.egg-info/
+-rw-r--r--   0 chen      (1000) chen      (1000)     3176 2023-04-14 06:37:20.000000 django-vite-react-0.0.2/django_vite_react.egg-info/PKG-INFO
+-rw-r--r--   0 chen      (1000) chen      (1000)      520 2023-04-14 06:37:20.000000 django-vite-react-0.0.2/django_vite_react.egg-info/SOURCES.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)        1 2023-04-14 06:37:20.000000 django-vite-react-0.0.2/django_vite_react.egg-info/dependency_links.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)       12 2023-04-14 06:37:20.000000 django-vite-react-0.0.2/django_vite_react.egg-info/requires.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)        6 2023-04-14 06:37:20.000000 django-vite-react-0.0.2/django_vite_react.egg-info/top_level.txt
+-rw-r--r--   0 chen      (1000) chen      (1000)      108 2023-04-14 06:04:51.000000 django-vite-react-0.0.2/pyproject.toml
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/react/
+-rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/__init__.py
+-rw-r--r--   0 chen      (1000) chen      (1000)       63 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/admin.py
+-rw-r--r--   0 chen      (1000) chen      (1000)      142 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/apps.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/react/components/
+-rw-r--r--   0 chen      (1000) chen      (1000)      280 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/components/app.jsx
+-rw-r--r--   0 chen      (1000) chen      (1000)      370 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/generic.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/react/migrations/
+-rw-r--r--   0 chen      (1000) chen      (1000)        0 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/migrations/__init__.py
+-rw-r--r--   0 chen      (1000) chen      (1000)      442 2022-05-12 03:05:04.000000 django-vite-react-0.0.2/react/mixins.py
+-rw-r--r--   0 chen      (1000) chen      (1000)       57 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/models.py
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.759502 django-vite-react-0.0.2/react/templates/
+drwxr-xr-x   0 chen      (1000) chen      (1000)        0 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/react/templates/react/
+-rw-r--r--   0 chen      (1000) chen      (1000)      288 2022-05-12 03:04:03.000000 django-vite-react-0.0.2/react/templates/react/react.html
+-rw-r--r--   0 chen      (1000) chen      (1000)      182 2022-05-12 03:04:09.000000 django-vite-react-0.0.2/react/templates/react/react_props.html
+-rw-r--r--   0 chen      (1000) chen      (1000)       60 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/tests.py
+-rw-r--r--   0 chen      (1000) chen      (1000)       63 2022-05-11 08:44:48.000000 django-vite-react-0.0.2/react/views.py
+-rw-r--r--   0 chen      (1000) chen      (1000)      895 2023-04-14 06:37:20.762835 django-vite-react-0.0.2/setup.cfg
+-rw-r--r--   0 chen      (1000) chen      (1000)       38 2023-04-14 06:07:50.000000 django-vite-react-0.0.2/setup.py
```

### Comparing `django-vite-react-0.0.1/LICENSE` & `django-vite-react-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vite-react-0.0.1/PKG-INFO` & `django-vite-react-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vite-react
-Version: 0.0.1
+Version: 0.0.2
 Summary: An easy way to Write React Component with Django.
 Home-page: https://github.com/ChanMo/django-react/
 Author: ChanMo
 Author-email: chan.mo@outlook.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-vite-react-0.0.1/README.rst` & `django-vite-react-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-vite-react-0.0.1/django_vite_react.egg-info/PKG-INFO` & `django-vite-react-0.0.2/django_vite_react.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vite-react
-Version: 0.0.1
+Version: 0.0.2
 Summary: An easy way to Write React Component with Django.
 Home-page: https://github.com/ChanMo/django-react/
 Author: ChanMo
 Author-email: chan.mo@outlook.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-vite-react-0.0.1/django_vite_react.egg-info/SOURCES.txt` & `django-vite-react-0.0.2/django_vite_react.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-vite-react-0.0.1/setup.cfg` & `django-vite-react-0.0.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-vite-react
-version = 0.0.1
+version = 0.0.2
 description = An easy way to Write React Component with Django.
 long_description = file: README.rst
 url = https://github.com/ChanMo/django-react/
 author = ChanMo
 author_email = chan.mo@outlook.com
 license = MIT
 classifiers =
```

