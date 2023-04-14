# Comparing `tmp/pretix_plugin_attendance_certificate-0.1.6.tar.gz` & `tmp/pretix_plugin_attendance_certificate-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix_plugin_attendance_certificate-0.1.6.tar", last modified: Fri Apr 14 09:18:21 2023, max compression
+gzip compressed data, was "pretix_plugin_attendance_certificate-0.1.7.tar", last modified: Fri Apr 14 11:29:10 2023, max compression
```

## Comparing `pretix_plugin_attendance_certificate-0.1.6.tar` & `pretix_plugin_attendance_certificate-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/LICENSE
--rw-r--r--   0        0        0      161 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/README.md
--rw-r--r--   0        0        0     1100 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/__init__.py
--rw-r--r--   0        0        0      313 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/locale/de_Informal/.gitkeep
--rw-r--r--   0        0        0      313 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1950 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/migrations/__init__.py
--rw-r--r--   0        0        0     1380 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/models.py
--rw-r--r--   0        0        0     1516 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/render.py
--rw-r--r--   0        0        0     3109 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/signals.py
--rw-r--r--   0        0        0        0 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/static/pretix_attendance_certificate/.gitkeep
--rw-r--r--   0        0        0      779 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf
--rw-r--r--   0        0        0     2615 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/tasks.py
--rw-r--r--   0        0        0        0 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/templates/pretix_attendance_certificate/.gitkeep
--rw-r--r--   0        0        0       90 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/templates/pretix_attendance_certificate/history_fragment_attendance_certificate.html
--rw-r--r--   0        0        0      117 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/templates/pretix_attendance_certificate/send_form_fragment_attendance_certificate.html
--rw-r--r--   0        0        0      495 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/urls.py
--rw-r--r--   0        0        0        0 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/views/__init__.py
--rw-r--r--   0        0        0     3611 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/views/editor.py
--rw-r--r--   0        0        0     2319 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/views/emails.py
--rw-r--r--   0        0        0      706 2023-04-14 09:18:21.644515 pretix_plugin_attendance_certificate-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/tests/conftest.py
--rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pretix_plugin_attendance_certificate-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/LICENSE
+-rw-r--r--   0        0        0      161 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/README.md
+-rw-r--r--   0        0        0     1100 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/locale/de_Informal/.gitkeep
+-rw-r--r--   0        0        0      313 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1950 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/migrations/__init__.py
+-rw-r--r--   0        0        0     1380 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/models.py
+-rw-r--r--   0        0        0     1516 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/render.py
+-rw-r--r--   0        0        0     3475 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/signals.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/static/pretix_attendance_certificate/.gitkeep
+-rw-r--r--   0        0        0      779 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf
+-rw-r--r--   0        0        0     2615 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/templates/pretix_attendance_certificate/.gitkeep
+-rw-r--r--   0        0        0       90 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/templates/pretix_attendance_certificate/history_fragment_attendance_certificate.html
+-rw-r--r--   0        0        0      117 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/templates/pretix_attendance_certificate/send_form_fragment_attendance_certificate.html
+-rw-r--r--   0        0        0      495 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/urls.py
+-rw-r--r--   0        0        0        0 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/views/__init__.py
+-rw-r--r--   0        0        0     3611 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/views/editor.py
+-rw-r--r--   0        0        0     2319 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/views/emails.py
+-rw-r--r--   0        0        0      706 2023-04-14 11:29:10.696577 pretix_plugin_attendance_certificate-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 11:29:00.784401 pretix_plugin_attendance_certificate-0.1.7/tests/conftest.py
+-rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pretix_plugin_attendance_certificate-0.1.7/PKG-INFO
```

### Comparing `pretix_plugin_attendance_certificate-0.1.6/LICENSE` & `pretix_plugin_attendance_certificate-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/__init__.py` & `pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/migrations/0001_initial.py` & `pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/models.py` & `pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/models.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/render.py` & `pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/render.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/signals.py` & `pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/signals.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,7 +76,16 @@
 def logentry_display(sender, logentry, **kwargs):
     if logentry.action_type == "pretix_attendance_certificate.sent.attendee":
         order_position = OrderPosition.objects.get(id=logentry.parsed_data["position"])
         return _(
             "An email has been sent with the certificate of attendance "
             'to attendee "{attendee_name}"'
         ).format(attendee_name=order_position.attendee_name)
+
+    if (
+        logentry.action_type
+        == "pretix.plugins.pretix_attendance_certificate.layout.changed"
+    ):
+        return _("The layout of the certificate of attendance has been changed.")
+
+    if logentry.action_type == "pretix_attendance_certificate.sendmail.sent":
+        return _("The certificate of attendance has been sent out to all attendees.")
```

### Comparing `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf` & `pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/tasks.py` & `pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/tasks.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/views/editor.py` & `pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/views/editor.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/views/emails.py` & `pretix_plugin_attendance_certificate-0.1.7/pretix_attendance_certificate/views/emails.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.6/pyproject.toml` & `pretix_plugin_attendance_certificate-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "pretix-plugin-attendance-certificate"
-version = "0.1.6"
+version = "0.1.7"
 description = "Create attendance certificates"
 authors = [
     { name = "Python Italia" },
 ]
 dependencies = []
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
```

