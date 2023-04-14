# Comparing `tmp/django-custom-modal-admin-0.2.0.tar.gz` & `tmp/django-custom-modal-admin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-custom-modal-admin-0.2.0.tar", last modified: Mon Nov 22 16:53:07 2021, max compression
+gzip compressed data, was "django-custom-modal-admin-0.2.1.tar", last modified: Fri Apr 14 07:58:59 2023, max compression
```

## Comparing `django-custom-modal-admin-0.2.0.tar` & `django-custom-modal-admin-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 16:53:07.339358 django-custom-modal-admin-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-11-22 16:52:57.000000 django-custom-modal-admin-0.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3375 2021-11-22 16:52:57.000000 django-custom-modal-admin-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-11-22 16:52:57.000000 django-custom-modal-admin-0.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2021-11-22 16:52:57.000000 django-custom-modal-admin-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      244 2021-11-22 16:52:57.000000 django-custom-modal-admin-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4881 2021-11-22 16:53:07.339358 django-custom-modal-admin-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3992 2021-11-22 16:52:57.000000 django-custom-modal-admin-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 16:53:07.339358 django-custom-modal-admin-0.2.0/custom_modal_admin/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-22 16:52:57.000000 django-custom-modal-admin-0.2.0/custom_modal_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      449 2021-11-22 16:52:57.000000 django-custom-modal-admin-0.2.0/custom_modal_admin/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-11-22 16:52:57.000000 django-custom-modal-admin-0.2.0/custom_modal_admin/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 16:53:07.339358 django-custom-modal-admin-0.2.0/custom_modal_admin/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 16:53:07.339358 django-custom-modal-admin-0.2.0/custom_modal_admin/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)      591 2021-11-22 16:52:57.000000 django-custom-modal-admin-0.2.0/custom_modal_admin/static/js/custom_modal_admin.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 16:53:07.339358 django-custom-modal-admin-0.2.0/django_custom_modal_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4881 2021-11-22 16:53:07.000000 django-custom-modal-admin-0.2.0/django_custom_modal_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      561 2021-11-22 16:53:07.000000 django-custom-modal-admin-0.2.0/django_custom_modal_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-22 16:53:07.000000 django-custom-modal-admin-0.2.0/django_custom_modal_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-22 16:53:07.000000 django-custom-modal-admin-0.2.0/django_custom_modal_admin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-11-22 16:53:07.000000 django-custom-modal-admin-0.2.0/django_custom_modal_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-11-22 16:53:07.000000 django-custom-modal-admin-0.2.0/django_custom_modal_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-22 16:52:57.000000 django-custom-modal-admin-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3030 2021-11-22 16:52:57.000000 django-custom-modal-admin-0.2.0/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2021-11-22 16:53:07.343359 django-custom-modal-admin-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2324 2021-11-22 16:52:57.000000 django-custom-modal-admin-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:59.725947 django-custom-modal-admin-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-14 07:58:59.725947 django-custom-modal-admin-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:59.721947 django-custom-modal-admin-0.2.1/custom_modal_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/custom_modal_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/custom_modal_admin/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/custom_modal_admin/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:59.717947 django-custom-modal-admin-0.2.1/custom_modal_admin/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:59.721947 django-custom-modal-admin-0.2.1/custom_modal_admin/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/custom_modal_admin/static/css/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:59.721947 django-custom-modal-admin-0.2.1/custom_modal_admin/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/custom_modal_admin/static/js/custom_modal_admin.js
+-rw-r--r--   0 runner    (1001) docker     (123)   253747 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/custom_modal_admin/static/js/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:58:59.725947 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-14 07:58:59.000000 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-14 07:58:59.000000 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:58:59.000000 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:58:59.000000 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 07:58:59.000000 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 07:58:59.000000 django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-14 07:58:59.725947 django-custom-modal-admin-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2275 2023-04-14 07:58:48.000000 django-custom-modal-admin-0.2.1/setup.py
```

### Comparing `django-custom-modal-admin-0.2.0/CONTRIBUTING.rst` & `django-custom-modal-admin-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.0/LICENSE.md` & `django-custom-modal-admin-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.0/PKG-INFO` & `django-custom-modal-admin-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: django-custom-modal-admin
-Version: 0.2.0
+Version: 0.2.1
 Summary: Your project description goes here
 Home-page: https://github.com/frankhood/django-custom-modal-admin
 Author: FrankHood Business Solutions srl
 Author-email: info@frankhood.it
 License: MIT
 Keywords: django-custom-modal-admin
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE.md
 
 =============================
 Django custom modal admin
@@ -166,9 +164,7 @@
 History
 _______
 
 0.2.0 (2021-11-22)
 __________________
 
 * First release on PyPI.
-
-
```

### Comparing `django-custom-modal-admin-0.2.0/README.rst` & `django-custom-modal-admin-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.0/custom_modal_admin/static/js/custom_modal_admin.js` & `django-custom-modal-admin-0.2.1/custom_modal_admin/static/js/custom_modal_admin.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,20 @@
-$(function() {
-    $('.js-django-admin-custom-modal').each(function(index, element) {
-        var $currentEl = $(element);
-        $currentEl.on('click', function(e) {
-            var targetModalSelector = '[data-django-admin-custom-modal=' + $currentEl.data('targetName') + ']';
-            var $targetModal = $(targetModalSelector);
+(function($) {
+    $(function() {
+        $('.js-django-admin-custom-modal').each(function(index, element) {
+            var $currentEl = $(element);
+            $currentEl.on('click', function(e) {
+                var targetModalSelector = '[data-django-admin-custom-modal=' + $currentEl.data('targetName') + ']';
+                var $targetModal = $(targetModalSelector);
 
-            e.preventDefault();
-            e.stopPropagation();
-            $targetModal.dialog({
-                resizable: false,
-                height: 'auto',
-                width: 'auto',
-                modal: true
+                e.preventDefault();
+                e.stopPropagation();
+                $targetModal.dialog({
+                    resizable: false,
+                    height: 'auto',
+                    width: 'auto',
+                    modal: true
+                });
             });
         });
     });
-});
+})(window.django ? window.django.jQuery : window.jQuery);
```

### Comparing `django-custom-modal-admin-0.2.0/django_custom_modal_admin.egg-info/PKG-INFO` & `django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: django-custom-modal-admin
-Version: 0.2.0
+Version: 0.2.1
 Summary: Your project description goes here
 Home-page: https://github.com/frankhood/django-custom-modal-admin
 Author: FrankHood Business Solutions srl
 Author-email: info@frankhood.it
 License: MIT
 Keywords: django-custom-modal-admin
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE.md
 
 =============================
 Django custom modal admin
@@ -166,9 +164,7 @@
 History
 _______
 
 0.2.0 (2021-11-22)
 __________________
 
 * First release on PyPI.
-
-
```

### Comparing `django-custom-modal-admin-0.2.0/django_custom_modal_admin.egg-info/SOURCES.txt` & `django-custom-modal-admin-0.2.1/django_custom_modal_admin.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 requirements.txt
 requirements_test.txt
 setup.cfg
 setup.py
 custom_modal_admin/__init__.py
 custom_modal_admin/admin.py
 custom_modal_admin/apps.py
+custom_modal_admin/static/css/jquery-ui.css
 custom_modal_admin/static/js/custom_modal_admin.js
+custom_modal_admin/static/js/jquery-ui.min.js
 django_custom_modal_admin.egg-info/PKG-INFO
 django_custom_modal_admin.egg-info/SOURCES.txt
 django_custom_modal_admin.egg-info/dependency_links.txt
 django_custom_modal_admin.egg-info/not-zip-safe
 django_custom_modal_admin.egg-info/requires.txt
 django_custom_modal_admin.egg-info/top_level.txt
```

### Comparing `django-custom-modal-admin-0.2.0/requirements_test.txt` & `django-custom-modal-admin-0.2.1/requirements_test.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #
 # This file is autogenerated by pip-compile with python 3.6
 # To update, run:
 #
 #    pip-compile --output-file=requirements_test.txt requirements_test.in
 #
-asgiref==3.4.1
-    # via django
 backports.entry-points-selectable==1.1.1
     # via virtualenv
 bleach==4.1.0
     # via readme-renderer
 bump2version==1.0.1
     # via bumpversion
 bumpversion==0.6.0
@@ -18,25 +16,22 @@
     # via requests
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==2.0.7
     # via requests
 click==8.0.3
     # via pip-tools
-codecov==2.1.12
-    # via -r requirements_test.in
 colorama==0.4.4
     # via
     #   twine
     #   zest.releaser
 coverage==6.1.2
     # via
     #   -r requirements_dev.in
     #   -r requirements_test.in
-    #   codecov
 distlib==0.3.3
     # via virtualenv
 docutils==0.18
     # via readme-renderer
 filelock==3.4.0
     # via
     #   tox
@@ -100,15 +95,14 @@
     # via django
 pyyaml==6.0
     # via pre-commit
 readme-renderer==30.0
     # via twine
 requests==2.26.0
     # via
-    #   codecov
     #   requests-toolbelt
     #   twine
     #   zest.releaser
 requests-toolbelt==0.9.1
     # via twine
 rfc3986==1.5.0
     # via twine
@@ -132,15 +126,14 @@
     # via twine
 twine==3.6.0
     # via
     #   -r requirements_dev.in
     #   zest.releaser
 typing-extensions==4.0.0
     # via
-    #   asgiref
     #   importlib-metadata
 urllib3==1.26.7
     # via requests
 virtualenv==20.10.0
     # via
     #   pre-commit
     #   tox
```

### Comparing `django-custom-modal-admin-0.2.0/setup.cfg` & `django-custom-modal-admin-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-custom-modal-admin-0.2.0/setup.py` & `django-custom-modal-admin-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,13 +64,12 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.2",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
 )
```

