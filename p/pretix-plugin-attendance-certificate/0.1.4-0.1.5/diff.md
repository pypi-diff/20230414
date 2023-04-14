# Comparing `tmp/pretix_plugin_attendance_certificate-0.1.4.tar.gz` & `tmp/pretix_plugin_attendance_certificate-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix_plugin_attendance_certificate-0.1.4.tar", last modified: Thu Apr 13 14:00:06 2023, max compression
+gzip compressed data, was "pretix_plugin_attendance_certificate-0.1.5.tar", last modified: Fri Apr 14 00:50:07 2023, max compression
```

## Comparing `pretix_plugin_attendance_certificate-0.1.4.tar` & `pretix_plugin_attendance_certificate-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-04-13 13:59:48.137488 pretix_plugin_attendance_certificate-0.1.4/LICENSE
--rw-r--r--   0        0        0      161 2023-04-13 13:59:48.137488 pretix_plugin_attendance_certificate-0.1.4/README.md
--rw-r--r--   0        0        0     1100 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/__init__.py
--rw-r--r--   0        0        0      313 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/locale/de_Informal/.gitkeep
--rw-r--r--   0        0        0      313 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1960 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/migrations/__init__.py
--rw-r--r--   0        0        0     1380 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/models.py
--rw-r--r--   0        0        0     1516 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/render.py
--rw-r--r--   0        0        0     2478 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/signals.py
--rw-r--r--   0        0        0        0 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/static/pretix_attendance_certificate/.gitkeep
--rw-r--r--   0        0        0      779 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf
--rw-r--r--   0        0        0     2615 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/tasks.py
--rw-r--r--   0        0        0        0 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/templates/pretix_attendance_certificate/.gitkeep
--rw-r--r--   0        0        0       90 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/templates/pretix_attendance_certificate/history_fragment_attendance_certificate.html
--rw-r--r--   0        0        0      117 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/templates/pretix_attendance_certificate/send_form_fragment_attendance_certificate.html
--rw-r--r--   0        0        0      495 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/urls.py
--rw-r--r--   0        0        0        0 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/views/__init__.py
--rw-r--r--   0        0        0     3611 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/views/editor.py
--rw-r--r--   0        0        0     2319 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/views/emails.py
--rw-r--r--   0        0        0      706 2023-04-13 14:00:06.657369 pretix_plugin_attendance_certificate-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pretix_plugin_attendance_certificate-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/LICENSE
+-rw-r--r--   0        0        0      161 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/README.md
+-rw-r--r--   0        0        0     1100 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/locale/de_Informal/.gitkeep
+-rw-r--r--   0        0        0      313 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1950 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/migrations/__init__.py
+-rw-r--r--   0        0        0     1380 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/models.py
+-rw-r--r--   0        0        0     1516 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/render.py
+-rw-r--r--   0        0        0     2478 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/signals.py
+-rw-r--r--   0        0        0        0 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/static/pretix_attendance_certificate/.gitkeep
+-rw-r--r--   0        0        0      779 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf
+-rw-r--r--   0        0        0     2615 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/templates/pretix_attendance_certificate/.gitkeep
+-rw-r--r--   0        0        0       90 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/templates/pretix_attendance_certificate/history_fragment_attendance_certificate.html
+-rw-r--r--   0        0        0      117 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/templates/pretix_attendance_certificate/send_form_fragment_attendance_certificate.html
+-rw-r--r--   0        0        0      495 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/urls.py
+-rw-r--r--   0        0        0        0 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/views/__init__.py
+-rw-r--r--   0        0        0     3611 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/views/editor.py
+-rw-r--r--   0        0        0     2319 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/views/emails.py
+-rw-r--r--   0        0        0      706 2023-04-14 00:50:07.891702 pretix_plugin_attendance_certificate-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pretix_plugin_attendance_certificate-0.1.5/PKG-INFO
```

### Comparing `pretix_plugin_attendance_certificate-0.1.4/LICENSE` & `pretix_plugin_attendance_certificate-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/__init__.py` & `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/migrations/0001_initial.py` & `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/migrations/0001_initial.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pretix_attendance_certificate.models
 
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = [
-        ("pretixbase", "0237_question_valid_string_length"),
+        ("pretixbase", "0235_auto_20230316_2023"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="AttendanceCertificateLayout",
             fields=[
                 (
```

### Comparing `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/models.py` & `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/models.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/render.py` & `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/render.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/signals.py` & `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/signals.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf` & `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/tasks.py` & `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/tasks.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/views/editor.py` & `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/views/editor.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/views/emails.py` & `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/views/emails.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.4/pyproject.toml` & `pretix_plugin_attendance_certificate-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "pretix-plugin-attendance-certificate"
-version = "0.1.4"
+version = "0.1.5"
 description = "Create attendance certificates"
 authors = [
     { name = "Python Italia" },
 ]
 dependencies = []
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
```

