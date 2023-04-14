# Comparing `tmp/django-checkbox-normalize-0.1.2.tar.gz` & `tmp/django-checkbox-normalize-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-checkbox-normalize-0.1.2.tar", last modified: Wed Sep  9 03:17:14 2020, max compression
+gzip compressed data, was "django-checkbox-normalize-0.2.0.tar", last modified: Fri Apr 14 02:33:53 2023, max compression
```

## Comparing `django-checkbox-normalize-0.1.2.tar` & `django-checkbox-normalize-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxrwxrwx   0        0        0        0 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/
--rw-rw-rw-   0        0        0     1067 2020-06-28 01:22:41.000000 django-checkbox-normalize-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      243 2020-09-09 03:15:59.000000 django-checkbox-normalize-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1842 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      695 2020-09-09 03:10:02.000000 django-checkbox-normalize-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize/
--rw-rw-rw-   0        0        0        0 2020-09-09 02:05:00.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize/__init__.py
--rw-rw-rw-   0        0        0        0 2020-09-09 03:10:17.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize/admin.py
--rw-rw-rw-   0        0        0        0 2020-09-09 03:10:24.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize/apps.py
-drwxrwxrwx   0        0        0        0 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize/migrations/
--rw-rw-rw-   0        0        0        0 2020-09-09 02:05:00.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize/migrations/__init__.py
--rw-rw-rw-   0        0        0        0 2020-09-09 03:10:12.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize/models.py
-drwxrwxrwx   0        0        0        0 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize/templates/
-drwxrwxrwx   0        0        0        0 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize/templates/admin/
-drwxrwxrwx   0        0        0        0 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize/templates/admin/includes/
--rw-rw-rw-   0        0        0     1951 2020-09-09 03:12:59.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize/templates/admin/includes/fieldset.html
--rw-rw-rw-   0        0        0        0 2020-09-09 03:10:09.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize/tests.py
--rw-rw-rw-   0        0        0        0 2020-09-09 03:10:06.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize/views.py
-drwxrwxrwx   0        0        0        0 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize.egg-info/
--rw-rw-rw-   0        0        0     1842 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      674 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/django_checkbox_normalize.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        8 2020-09-09 02:05:00.000000 django-checkbox-normalize-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2020-09-09 03:17:14.000000 django-checkbox-normalize-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1547 2020-09-09 03:15:41.000000 django-checkbox-normalize-0.1.2/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-14 02:33:53.209005 django-checkbox-normalize-0.2.0/
+-rw-r--r--   0 test       (501) staff       (20)     1067 2023-04-14 02:06:48.000000 django-checkbox-normalize-0.2.0/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      243 2023-04-14 01:30:54.000000 django-checkbox-normalize-0.2.0/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     2016 2023-04-14 02:33:53.208886 django-checkbox-normalize-0.2.0/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1267 2023-04-14 02:24:01.000000 django-checkbox-normalize-0.2.0/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-14 02:33:53.207532 django-checkbox-normalize-0.2.0/django_checkbox_normalize/
+-rw-r--r--   0 test       (501) staff       (20)       85 2023-04-14 02:07:29.000000 django-checkbox-normalize-0.2.0/django_checkbox_normalize/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)      392 2023-04-14 02:11:07.000000 django-checkbox-normalize-0.2.0/django_checkbox_normalize/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      872 2023-04-14 02:00:51.000000 django-checkbox-normalize-0.2.0/django_checkbox_normalize/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-14 02:33:53.208514 django-checkbox-normalize-0.2.0/django_checkbox_normalize/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2023-04-14 01:30:54.000000 django-checkbox-normalize-0.2.0/django_checkbox_normalize/migrations/__init__.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-14 02:33:53.206181 django-checkbox-normalize-0.2.0/django_checkbox_normalize/static/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-14 02:33:53.206221 django-checkbox-normalize-0.2.0/django_checkbox_normalize/static/django_checkbox_normalize/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-14 02:33:53.208608 django-checkbox-normalize-0.2.0/django_checkbox_normalize/static/django_checkbox_normalize/js/
+-rw-r--r--   0 test       (501) staff       (20)      378 2023-04-14 02:19:45.000000 django-checkbox-normalize-0.2.0/django_checkbox_normalize/static/django_checkbox_normalize/js/django_checkbox_normalize.js
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-14 02:33:53.208410 django-checkbox-normalize-0.2.0/django_checkbox_normalize.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     2016 2023-04-14 02:33:53.000000 django-checkbox-normalize-0.2.0/django_checkbox_normalize.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      594 2023-04-14 02:33:53.000000 django-checkbox-normalize-0.2.0/django_checkbox_normalize.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-14 02:33:53.000000 django-checkbox-normalize-0.2.0/django_checkbox_normalize.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-14 02:33:53.000000 django-checkbox-normalize-0.2.0/django_checkbox_normalize.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)        7 2023-04-14 02:33:53.000000 django-checkbox-normalize-0.2.0/django_checkbox_normalize.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       26 2023-04-14 02:33:53.000000 django-checkbox-normalize-0.2.0/django_checkbox_normalize.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)        8 2023-04-14 01:30:54.000000 django-checkbox-normalize-0.2.0/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2023-04-14 02:33:53.209038 django-checkbox-normalize-0.2.0/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1554 2023-04-14 02:12:23.000000 django-checkbox-normalize-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-checkbox-normalize-0.1.2/LICENSE` & `django-checkbox-normalize-0.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 zencore.cn
+Copyright (c) 2020 zencore.cn
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-checkbox-normalize-0.1.2/django_checkbox_normalize.egg-info/SOURCES.txt` & `django-checkbox-normalize-0.2.0/django_checkbox_normalize.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 django_checkbox_normalize/__init__.py
 django_checkbox_normalize/admin.py
 django_checkbox_normalize/apps.py
-django_checkbox_normalize/models.py
-django_checkbox_normalize/tests.py
-django_checkbox_normalize/views.py
 django_checkbox_normalize.egg-info/PKG-INFO
 django_checkbox_normalize.egg-info/SOURCES.txt
 django_checkbox_normalize.egg-info/dependency_links.txt
 django_checkbox_normalize.egg-info/not-zip-safe
 django_checkbox_normalize.egg-info/requires.txt
 django_checkbox_normalize.egg-info/top_level.txt
 django_checkbox_normalize/migrations/__init__.py
-django_checkbox_normalize/templates/admin/includes/fieldset.html
+django_checkbox_normalize/static/django_checkbox_normalize/js/django_checkbox_normalize.js
```

### Comparing `django-checkbox-normalize-0.1.2/setup.py` & `django-checkbox-normalize-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="django-checkbox-normalize",
-    version="0.1.2",
-    description="It's bad design to put label after checkbox for BooleanField widget, so let's make it normal.",
+    version="0.2.0",
+    description="It's NOT a good design to put label after checkbox for BooleanField widget, so let's make it normal.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="zencore",
     author_email="dobetter@zencore.cn",
     url="https://github.com/zencore-cn/zencore-issues",
     license="MIT",
     classifiers=[
```

