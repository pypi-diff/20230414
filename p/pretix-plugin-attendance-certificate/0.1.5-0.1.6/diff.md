# Comparing `tmp/pretix_plugin_attendance_certificate-0.1.5.tar.gz` & `tmp/pretix_plugin_attendance_certificate-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix_plugin_attendance_certificate-0.1.5.tar", last modified: Fri Apr 14 00:50:07 2023, max compression
+gzip compressed data, was "pretix_plugin_attendance_certificate-0.1.6.tar", last modified: Fri Apr 14 09:18:21 2023, max compression
```

## Comparing `pretix_plugin_attendance_certificate-0.1.5.tar` & `pretix_plugin_attendance_certificate-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/LICENSE
--rw-r--r--   0        0        0      161 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/README.md
--rw-r--r--   0        0        0     1100 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/__init__.py
--rw-r--r--   0        0        0      313 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/locale/de_Informal/.gitkeep
--rw-r--r--   0        0        0      313 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1950 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/migrations/__init__.py
--rw-r--r--   0        0        0     1380 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/models.py
--rw-r--r--   0        0        0     1516 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/render.py
--rw-r--r--   0        0        0     2478 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/signals.py
--rw-r--r--   0        0        0        0 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/static/pretix_attendance_certificate/.gitkeep
--rw-r--r--   0        0        0      779 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf
--rw-r--r--   0        0        0     2615 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/tasks.py
--rw-r--r--   0        0        0        0 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/templates/pretix_attendance_certificate/.gitkeep
--rw-r--r--   0        0        0       90 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/templates/pretix_attendance_certificate/history_fragment_attendance_certificate.html
--rw-r--r--   0        0        0      117 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/templates/pretix_attendance_certificate/send_form_fragment_attendance_certificate.html
--rw-r--r--   0        0        0      495 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/urls.py
--rw-r--r--   0        0        0        0 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/views/__init__.py
--rw-r--r--   0        0        0     3611 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/views/editor.py
--rw-r--r--   0        0        0     2319 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/views/emails.py
--rw-r--r--   0        0        0      706 2023-04-14 00:50:07.891702 pretix_plugin_attendance_certificate-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 00:49:57.319649 pretix_plugin_attendance_certificate-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pretix_plugin_attendance_certificate-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/LICENSE
+-rw-r--r--   0        0        0      161 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/README.md
+-rw-r--r--   0        0        0     1100 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/locale/de_Informal/.gitkeep
+-rw-r--r--   0        0        0      313 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1950 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/migrations/__init__.py
+-rw-r--r--   0        0        0     1380 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/models.py
+-rw-r--r--   0        0        0     1516 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/render.py
+-rw-r--r--   0        0        0     3109 2023-04-14 09:18:10.468483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/signals.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/static/pretix_attendance_certificate/.gitkeep
+-rw-r--r--   0        0        0      779 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf
+-rw-r--r--   0        0        0     2615 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/templates/pretix_attendance_certificate/.gitkeep
+-rw-r--r--   0        0        0       90 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/templates/pretix_attendance_certificate/history_fragment_attendance_certificate.html
+-rw-r--r--   0        0        0      117 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/templates/pretix_attendance_certificate/send_form_fragment_attendance_certificate.html
+-rw-r--r--   0        0        0      495 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/urls.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/views/__init__.py
+-rw-r--r--   0        0        0     3611 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/views/editor.py
+-rw-r--r--   0        0        0     2319 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/views/emails.py
+-rw-r--r--   0        0        0      706 2023-04-14 09:18:21.644515 pretix_plugin_attendance_certificate-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 09:18:10.472483 pretix_plugin_attendance_certificate-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pretix_plugin_attendance_certificate-0.1.6/PKG-INFO
```

### Comparing `pretix_plugin_attendance_certificate-0.1.5/LICENSE` & `pretix_plugin_attendance_certificate-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/__init__.py` & `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/migrations/0001_initial.py` & `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/models.py` & `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/models.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/render.py` & `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/render.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/signals.py` & `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/signals.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from django.urls import resolve, reverse
 from django.dispatch import receiver
 from pretix_attendance_certificate.views.emails import SendCertificateEmailView
 from pretix.control.signals import (
     nav_event,
 )
 from pretix.plugins.sendmail.signals import sendmail_view_classes
+from pretix.base.signals import logentry_display
+from pretix.base.models import OrderPosition
 
 
 @receiver(nav_event, dispatch_uid="certificate_of_attendance_nav")
 def control_nav_import(sender, request=None, **kwargs):
     url = resolve(request.path_info)
     p = request.user.has_event_permission(
         request.organizer, request.event, "can_change_settings", request
@@ -61,7 +63,20 @@
 
 
 @receiver(
     sendmail_view_classes, dispatch_uid="pretix_attendance_certificate_sendmail_view"
 )
 def register_sendmail_view(sender, **kwargs):
     return [SendCertificateEmailView]
+
+
+@receiver(
+    signal=logentry_display,
+    dispatch_uid="pretix_attendance_certificate_sendmail_view_logentry_display",
+)
+def logentry_display(sender, logentry, **kwargs):
+    if logentry.action_type == "pretix_attendance_certificate.sent.attendee":
+        order_position = OrderPosition.objects.get(id=logentry.parsed_data["position"])
+        return _(
+            "An email has been sent with the certificate of attendance "
+            'to attendee "{attendee_name}"'
+        ).format(attendee_name=order_position.attendee_name)
```

### Comparing `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf` & `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/tasks.py` & `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/tasks.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/views/editor.py` & `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/views/editor.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.5/pretix_attendance_certificate/views/emails.py` & `pretix_plugin_attendance_certificate-0.1.6/pretix_attendance_certificate/views/emails.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.5/pyproject.toml` & `pretix_plugin_attendance_certificate-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "pretix-plugin-attendance-certificate"
-version = "0.1.5"
+version = "0.1.6"
 description = "Create attendance certificates"
 authors = [
     { name = "Python Italia" },
 ]
 dependencies = []
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
```

