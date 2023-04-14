# Comparing `tmp/tap-zoom-1.1.1.tar.gz` & `tmp/tap-zoom-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-zoom-1.1.1.tar", last modified: Wed Apr 12 16:15:07 2023, max compression
+gzip compressed data, was "tap-zoom-1.1.2.tar", last modified: Fri Apr 14 07:45:06 2023, max compression
```

## Comparing `tap-zoom-1.1.1.tar` & `tap-zoom-1.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 16:15:07.306177 tap-zoom-1.1.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34522 2023-03-17 17:28:32.000000 tap-zoom-1.1.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      191 2023-04-12 16:15:07.306177 tap-zoom-1.1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3915 2023-04-12 16:12:22.000000 tap-zoom-1.1.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-12 16:15:07.306177 tap-zoom-1.1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-04-12 16:12:22.000000 tap-zoom-1.1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 16:15:07.302176 tap-zoom-1.1.1/tap_zoom/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2023-03-17 17:28:32.000000 tap-zoom-1.1.1/tap_zoom/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4584 2023-04-12 16:12:22.000000 tap-zoom-1.1.1/tap_zoom/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2531 2023-04-06 12:56:04.000000 tap-zoom-1.1.1/tap_zoom/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8021 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/endpoints.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 16:15:07.306177 tap-zoom-1.1.1/tap_zoom/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/meeting_files.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      757 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/meeting_poll_results.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/meeting_polls.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1414 2023-03-17 17:28:32.000000 tap-zoom-1.1.1/tap_zoom/schemas/meeting_questions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2272 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/meeting_registrants.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7940 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/meetings.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/report_meeting_participants.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1623 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/report_meetings.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      832 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/report_webinar_participants.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1785 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/report_webinars.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1500 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/users.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2274 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/webinar_absentees.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/webinar_files.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      444 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/webinar_panelists.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      757 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/webinar_poll_results.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/webinar_polls.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      757 2023-03-17 17:28:32.000000 tap-zoom-1.1.1/tap_zoom/schemas/webinar_qna_results.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1414 2023-03-17 17:28:32.000000 tap-zoom-1.1.1/tap_zoom/schemas/webinar_questions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2272 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/webinar_registrants.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      557 2023-03-17 17:28:32.000000 tap-zoom-1.1.1/tap_zoom/schemas/webinar_tracking_sources.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6714 2023-04-12 16:12:18.000000 tap-zoom-1.1.1/tap_zoom/schemas/webinars.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5406 2023-04-06 12:56:04.000000 tap-zoom-1.1.1/tap_zoom/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-12 16:15:07.302176 tap-zoom-1.1.1/tap_zoom.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      191 2023-04-12 16:15:07.000000 tap-zoom-1.1.1/tap_zoom.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-04-12 16:15:07.000000 tap-zoom-1.1.1/tap_zoom.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-12 16:15:07.000000 tap-zoom-1.1.1/tap_zoom.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2023-04-12 16:15:07.000000 tap-zoom-1.1.1/tap_zoom.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-04-12 16:15:07.000000 tap-zoom-1.1.1/tap_zoom.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-04-12 16:15:07.000000 tap-zoom-1.1.1/tap_zoom.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 07:45:06.134903 tap-zoom-1.1.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34522 2023-03-17 17:28:32.000000 tap-zoom-1.1.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      191 2023-04-14 07:45:06.134903 tap-zoom-1.1.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3915 2023-04-12 16:12:22.000000 tap-zoom-1.1.2/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-14 07:45:06.134903 tap-zoom-1.1.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-04-14 07:43:27.000000 tap-zoom-1.1.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 07:45:06.130903 tap-zoom-1.1.2/tap_zoom/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2023-03-17 17:28:32.000000 tap-zoom-1.1.2/tap_zoom/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4584 2023-04-14 07:43:27.000000 tap-zoom-1.1.2/tap_zoom/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2531 2023-04-06 12:56:04.000000 tap-zoom-1.1.2/tap_zoom/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8021 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/endpoints.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 07:45:06.134903 tap-zoom-1.1.2/tap_zoom/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/meeting_files.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      757 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/meeting_poll_results.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/meeting_polls.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1414 2023-03-17 17:28:32.000000 tap-zoom-1.1.2/tap_zoom/schemas/meeting_questions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2272 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/meeting_registrants.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7940 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/meetings.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/report_meeting_participants.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1623 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/report_meetings.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      832 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/report_webinar_participants.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1785 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/report_webinars.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1500 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/users.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2274 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/webinar_absentees.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/webinar_files.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      444 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/webinar_panelists.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      757 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/webinar_poll_results.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/webinar_polls.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      757 2023-03-17 17:28:32.000000 tap-zoom-1.1.2/tap_zoom/schemas/webinar_qna_results.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1414 2023-03-17 17:28:32.000000 tap-zoom-1.1.2/tap_zoom/schemas/webinar_questions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2272 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/webinar_registrants.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      557 2023-03-17 17:28:32.000000 tap-zoom-1.1.2/tap_zoom/schemas/webinar_tracking_sources.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6714 2023-04-12 16:12:18.000000 tap-zoom-1.1.2/tap_zoom/schemas/webinars.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5406 2023-04-06 12:56:04.000000 tap-zoom-1.1.2/tap_zoom/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 07:45:06.130903 tap-zoom-1.1.2/tap_zoom.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      191 2023-04-14 07:45:06.000000 tap-zoom-1.1.2/tap_zoom.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-04-14 07:45:06.000000 tap-zoom-1.1.2/tap_zoom.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-14 07:45:06.000000 tap-zoom-1.1.2/tap_zoom.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2023-04-14 07:45:06.000000 tap-zoom-1.1.2/tap_zoom.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-04-14 07:45:06.000000 tap-zoom-1.1.2/tap_zoom.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-04-14 07:45:06.000000 tap-zoom-1.1.2/tap_zoom.egg-info/top_level.txt
```

### Comparing `tap-zoom-1.1.1/LICENSE` & `tap-zoom-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/README.md` & `tap-zoom-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/setup.py` & `tap-zoom-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-zoom',
-      version='1.1.1',
+      version='1.1.2',
       description='Singer.io tap for extracting data from the Zoom API',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_zoom'],
       install_requires=[
         'backoff==1.8.0',
         'ratelimit==2.2.1',
         'requests==2.23.0',
```

### Comparing `tap-zoom-1.1.1/tap_zoom/__init__.py` & `tap-zoom-1.1.2/tap_zoom/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/client.py` & `tap-zoom-1.1.2/tap_zoom/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                           on_backoff=log_backoff_attempt,
                           factor=3)
     @backoff.on_exception(backoff.constant,
                           RateLimitException,
                           max_tries=8,
                           on_backoff=log_backoff_attempt,
                           jitter=None,
-                          interval=15)
+                          interval=30)
     @limits(calls=300, period=60)
     def request(self,
                 method,
                 path=None,
                 url=None,
                 ignore_zoom_error_codes=[],
                 ignore_http_error_codes=[],
```

### Comparing `tap-zoom-1.1.1/tap_zoom/discover.py` & `tap-zoom-1.1.2/tap_zoom/discover.py`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/endpoints.py` & `tap-zoom-1.1.2/tap_zoom/endpoints.py`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/meeting_poll_results.json` & `tap-zoom-1.1.2/tap_zoom/schemas/meeting_poll_results.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/meeting_polls.json` & `tap-zoom-1.1.2/tap_zoom/schemas/meeting_polls.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/meeting_questions.json` & `tap-zoom-1.1.2/tap_zoom/schemas/meeting_questions.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/meeting_registrants.json` & `tap-zoom-1.1.2/tap_zoom/schemas/meeting_registrants.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/meetings.json` & `tap-zoom-1.1.2/tap_zoom/schemas/meetings.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/report_meeting_participants.json` & `tap-zoom-1.1.2/tap_zoom/schemas/report_meeting_participants.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/report_meetings.json` & `tap-zoom-1.1.2/tap_zoom/schemas/report_meetings.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/report_webinar_participants.json` & `tap-zoom-1.1.2/tap_zoom/schemas/report_webinar_participants.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/report_webinars.json` & `tap-zoom-1.1.2/tap_zoom/schemas/report_webinars.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/users.json` & `tap-zoom-1.1.2/tap_zoom/schemas/users.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/webinar_absentees.json` & `tap-zoom-1.1.2/tap_zoom/schemas/webinar_absentees.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/webinar_poll_results.json` & `tap-zoom-1.1.2/tap_zoom/schemas/webinar_poll_results.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/webinar_polls.json` & `tap-zoom-1.1.2/tap_zoom/schemas/webinar_polls.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/webinar_qna_results.json` & `tap-zoom-1.1.2/tap_zoom/schemas/webinar_qna_results.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/webinar_questions.json` & `tap-zoom-1.1.2/tap_zoom/schemas/webinar_questions.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/webinar_registrants.json` & `tap-zoom-1.1.2/tap_zoom/schemas/webinar_registrants.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/webinar_tracking_sources.json` & `tap-zoom-1.1.2/tap_zoom/schemas/webinar_tracking_sources.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/schemas/webinars.json` & `tap-zoom-1.1.2/tap_zoom/schemas/webinars.json`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom/sync.py` & `tap-zoom-1.1.2/tap_zoom/sync.py`

 * *Files identical despite different names*

### Comparing `tap-zoom-1.1.1/tap_zoom.egg-info/SOURCES.txt` & `tap-zoom-1.1.2/tap_zoom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

