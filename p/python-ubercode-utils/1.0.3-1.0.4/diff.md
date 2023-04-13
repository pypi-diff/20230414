# Comparing `tmp/python-ubercode-utils-1.0.3.tar.gz` & `tmp/python-ubercode-utils-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-ubercode-utils-1.0.3.tar", last modified: Wed Apr 12 21:16:31 2023, max compression
+gzip compressed data, was "dist/python-ubercode-utils-1.0.4.tar", last modified: Thu Apr 13 22:47:32 2023, max compression
```

## Comparing `python-ubercode-utils-1.0.3.tar` & `python-ubercode-utils-1.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-12 21:16:31.684824 python-ubercode-utils-1.0.3/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1069 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/LICENSE
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       43 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/MANIFEST.in
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1330 2023-04-12 21:16:31.684824 python-ubercode-utils-1.0.3/PKG-INFO
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      683 2023-03-06 19:32:30.000000 python-ubercode-utils-1.0.3/README.md
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-12 21:16:31.680824 python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1330 2023-04-12 21:16:31.000000 python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/PKG-INFO
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      676 2023-04-12 21:16:31.000000 python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2023-04-12 21:16:31.000000 python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2023-04-12 21:16:18.000000 python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/not-zip-safe
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        9 2023-04-12 21:16:31.000000 python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/top_level.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       38 2023-04-12 21:16:31.684824 python-ubercode-utils-1.0.3/setup.cfg
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      886 2023-04-12 21:14:02.000000 python-ubercode-utils-1.0.3/setup.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-12 21:16:31.684824 python-ubercode-utils-1.0.3/test/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    10392 2023-03-09 18:12:52.000000 python-ubercode-utils-1.0.3/test/test_convert.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2712 2023-03-09 19:13:29.000000 python-ubercode-utils-1.0.3/test/test_cursor.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1088 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/test/test_dataframe.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     5379 2023-03-20 19:57:36.000000 python-ubercode-utils-1.0.3/test/test_environment.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     3000 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/test/test_json.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2855 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/test/test_logging.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     5139 2023-04-12 21:13:14.000000 python-ubercode-utils-1.0.3/test/test_urls.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2144 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/test/test_xml.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-12 21:16:31.684824 python-ubercode-utils-1.0.3/ubercode/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/ubercode/__init__.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-12 21:16:31.684824 python-ubercode-utils-1.0.3/ubercode/utils/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/ubercode/utils/__init__.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9473 2023-04-02 15:21:19.000000 python-ubercode-utils-1.0.3/ubercode/utils/convert.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1118 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/ubercode/utils/cursor.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      870 2023-04-03 13:13:43.000000 python-ubercode-utils-1.0.3/ubercode/utils/dataframe.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9704 2023-03-20 20:57:41.000000 python-ubercode-utils-1.0.3/ubercode/utils/environment.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1630 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/ubercode/utils/json.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9199 2023-03-06 22:18:08.000000 python-ubercode-utils-1.0.3/ubercode/utils/logging.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     7557 2023-04-12 21:11:31.000000 python-ubercode-utils-1.0.3/ubercode/utils/urls.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2876 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.3/ubercode/utils/xml.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-13 22:47:32.714927 python-ubercode-utils-1.0.4/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1069 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.4/LICENSE
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       43 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.4/MANIFEST.in
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1330 2023-04-13 22:47:32.714927 python-ubercode-utils-1.0.4/PKG-INFO
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      683 2023-03-06 19:32:30.000000 python-ubercode-utils-1.0.4/README.md
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-13 22:47:32.710927 python-ubercode-utils-1.0.4/python_ubercode_utils.egg-info/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1330 2023-04-13 22:47:32.000000 python-ubercode-utils-1.0.4/python_ubercode_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      676 2023-04-13 22:47:32.000000 python-ubercode-utils-1.0.4/python_ubercode_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2023-04-13 22:47:32.000000 python-ubercode-utils-1.0.4/python_ubercode_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2023-04-13 22:47:18.000000 python-ubercode-utils-1.0.4/python_ubercode_utils.egg-info/not-zip-safe
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        9 2023-04-13 22:47:32.000000 python-ubercode-utils-1.0.4/python_ubercode_utils.egg-info/top_level.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       38 2023-04-13 22:47:32.714927 python-ubercode-utils-1.0.4/setup.cfg
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      886 2023-04-13 22:46:22.000000 python-ubercode-utils-1.0.4/setup.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-13 22:47:32.710927 python-ubercode-utils-1.0.4/test/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    10441 2023-04-13 22:45:39.000000 python-ubercode-utils-1.0.4/test/test_convert.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2712 2023-03-09 19:13:29.000000 python-ubercode-utils-1.0.4/test/test_cursor.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1234 2023-04-13 22:45:39.000000 python-ubercode-utils-1.0.4/test/test_dataframe.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     5657 2023-04-13 22:45:39.000000 python-ubercode-utils-1.0.4/test/test_environment.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     3000 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.4/test/test_json.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2855 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.4/test/test_logging.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     5139 2023-04-12 21:13:14.000000 python-ubercode-utils-1.0.4/test/test_urls.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2144 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.4/test/test_xml.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-13 22:47:32.710927 python-ubercode-utils-1.0.4/ubercode/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.4/ubercode/__init__.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2023-04-13 22:47:32.714927 python-ubercode-utils-1.0.4/ubercode/utils/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.4/ubercode/utils/__init__.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9937 2023-04-13 22:45:39.000000 python-ubercode-utils-1.0.4/ubercode/utils/convert.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1118 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.4/ubercode/utils/cursor.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      870 2023-04-03 13:13:43.000000 python-ubercode-utils-1.0.4/ubercode/utils/dataframe.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    10854 2023-04-13 22:45:39.000000 python-ubercode-utils-1.0.4/ubercode/utils/environment.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1630 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.4/ubercode/utils/json.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     9199 2023-03-06 22:18:08.000000 python-ubercode-utils-1.0.4/ubercode/utils/logging.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     7557 2023-04-12 21:11:31.000000 python-ubercode-utils-1.0.4/ubercode/utils/urls.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     2876 2023-03-06 19:22:56.000000 python-ubercode-utils-1.0.4/ubercode/utils/xml.py
```

### Comparing `python-ubercode-utils-1.0.3/LICENSE` & `python-ubercode-utils-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.3/PKG-INFO` & `python-ubercode-utils-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ubercode-utils
-Version: 1.0.3
+Version: 1.0.4
 Summary: Core python utilities for all apps
 Home-page: https://github.com/sstacha/python-ubercode-utils
 Author: Steve Stacha
 Author-email: sstacha@gmail.com
 License: MIT
 Description: # python-ubercode-utils
         Extracting common python utilities re-used between all projects.  The intent is to have minimal dependencies
```

### Comparing `python-ubercode-utils-1.0.3/README.md` & `python-ubercode-utils-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/PKG-INFO` & `python-ubercode-utils-1.0.4/python_ubercode_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ubercode-utils
-Version: 1.0.3
+Version: 1.0.4
 Summary: Core python utilities for all apps
 Home-page: https://github.com/sstacha/python-ubercode-utils
 Author: Steve Stacha
 Author-email: sstacha@gmail.com
 License: MIT
 Description: # python-ubercode-utils
         Extracting common python utilities re-used between all projects.  The intent is to have minimal dependencies
```

### Comparing `python-ubercode-utils-1.0.3/python_ubercode_utils.egg-info/SOURCES.txt` & `python-ubercode-utils-1.0.4/python_ubercode_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.3/setup.py` & `python-ubercode-utils-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='python-ubercode-utils',
-      version='1.0.3',
+      version='1.0.4',
       description='Core python utilities for all apps',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/sstacha/python-ubercode-utils',
       author='Steve Stacha',
       author_email='sstacha@gmail.com',
       license='MIT',
```

### Comparing `python-ubercode-utils-1.0.3/test/test_convert.py` & `python-ubercode-utils-1.0.4/test/test_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,17 @@
         # test that a non class item without a dict gives the string representation
         with redirect_stdout(StringIO()) as sout:
             convert.dump("Test String")
         log_output = sout.getvalue()
         # note: print adds a newline
         self.assertEqual(log_output, "Test String" + os.linesep)
 
+    def test_human_readable(self):
+        pass
+
     # -------- helper conversions ----------
     def test_mask(self):
         """ Tests the mask helper conversion function """
         # test normal masking for an expected value & that the shown limits to 6 chars
         original_str = "Some random password with spaces and #@!!$%^&"
         self.assertEqual("Some r*********************************!!$%^&", convert.to_mask(original_str))
         # test None returns original value
```

### Comparing `python-ubercode-utils-1.0.3/test/test_cursor.py` & `python-ubercode-utils-1.0.4/test/test_cursor.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.3/test/test_dataframe.py` & `python-ubercode-utils-1.0.4/test/test_dataframe.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,17 +13,19 @@
         tlog = dataframe.DataframeLogger("test_log")
         # test that we can print a string with a label instead of a dataframe
         with redirect_stdout(StringIO()) as sout:
             tlog.dataframe("Test Dataframe", "Test Label")
         log_lines = sout.getvalue()
         label_string = logging.TermColor.OKBLUE + "Test Label"
         self.assertTrue(str(log_lines).startswith(label_string))
-        # always doesn't have a color so lets change the color and test for it
+        # always doesn't have a color so let's change the color and test for it
         with redirect_stdout(StringIO()) as sout:
-            tlog.dataframe("Test Dataframe", "Test Label", color="WARN")
+            tlog.dataframe("Test Dataframe", "Test Label", color="WARN", df_color="DEBUG")
         log_lines = sout.getvalue()
-        content_string = logging.TermColor.WARNING + "Test Dataframe"
+        content_string = logging.TermColor.WARNING + "Test Label"
+        self.assertTrue(content_string in str(log_lines))
+        content_string = logging.TermColor.F_DarkGray + "Test Dataframe"
         self.assertTrue(content_string in str(log_lines))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `python-ubercode-utils-1.0.3/test/test_environment.py` & `python-ubercode-utils-1.0.4/test/test_environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import unittest
+import time
 from contextlib import redirect_stdout
 from io import StringIO
 from pathlib import Path
 
 from ubercode.utils import logging, convert
-from ubercode.utils.environment import Environment
+from ubercode.utils.environment import Environment, Timer
 
 
 class TestEnvironment(unittest.TestCase):
 
     # -------- environment class ----------
     def test_override_variable(self):
         os_vars = {"OVERRIDE_DEBUG": "False",
@@ -104,10 +105,18 @@
         self.assertEqual(DATABASES['default']['PORT'], 3306)
         # test our password is encoded when logged
         self.assertTrue("Test_insecure_password" not in log_output)
         self.assertTrue("Test_************sword" in log_output)
         # test a None still works for initialization
         self.assertIsNotNone(Environment())
 
+    def test_timer(self):
+        timer = Timer().start()
+        time.sleep(3)
+        timer.stop()
+        print(str(timer))
+        self.assertEqual(timer.startTime.second + 3, timer.endTime.second)
+        self.assertTrue(timer.duration.startswith('3'))
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `python-ubercode-utils-1.0.3/test/test_json.py` & `python-ubercode-utils-1.0.4/test/test_json.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.3/test/test_logging.py` & `python-ubercode-utils-1.0.4/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.3/test/test_urls.py` & `python-ubercode-utils-1.0.4/test/test_urls.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.3/test/test_xml.py` & `python-ubercode-utils-1.0.4/test/test_xml.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.3/ubercode/utils/convert.py` & `python-ubercode-utils-1.0.4/ubercode/utils/convert.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,30 @@
             pprint(vars(value), indent=4)
         else:
             print(vars(value))
     else:
         print(str(value))
 
 
+def to_human_readable(duration: int) -> str:
+    days = duration // 86400
+    hours = duration // 3600 % 24
+    minutes = duration // 60 % 60
+    seconds = duration % 60
+    human_duration = ""
+    if days >= 1:
+        human_duration += f"{days} days, "
+    if hours >= 1:
+        human_duration += f"{hours} hours, "
+    if minutes >= 1:
+        human_duration += f"{minutes} minutes, "
+    human_duration += f"{seconds:.2f} seconds"
+    return human_duration
+
+
 # -------- primitive conversions --------
 def to_str(value: Any, none_to_empty: bool = True) -> str:
     """
     While not absolutely necessary; nice to have a common function to convert None values or not
     NOTE: this is exactly the same as [str(x) if x is not None else ''] if none_to_empty is true
     :param value: Any value
     :param none_to_empty: should we convert None to ''
```

### Comparing `python-ubercode-utils-1.0.3/ubercode/utils/cursor.py` & `python-ubercode-utils-1.0.4/ubercode/utils/cursor.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.3/ubercode/utils/dataframe.py` & `python-ubercode-utils-1.0.4/ubercode/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.3/ubercode/utils/environment.py` & `python-ubercode-utils-1.0.4/ubercode/utils/environment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,53 @@
 """
 A collection of environment utilities that can be used without circular dependencies.  For example,
 should be usable inside django settings.py!
 """
 import os
+import time
 from datetime import datetime
 from typing import Any, Tuple
 from ubercode.utils.logging import ColorLogger
 from ubercode.utils import convert
 
 _utils_settings_logger = ColorLogger("utils.environment")
 
 
+class Timer:
+    """
+    simple timer class to encapsulate starting, stopping and getting info from timeing
+    start_time = datetime point in time when started
+    end_time = datetime point in time when ended
+    _perf_start = arbitrary start counter (not a point in time)
+    _perf_end = arbitrary end counter (not a point in time)
+    duration = string representing the duration in human-readable format
+    """
+    def __init__(self):
+        self.startTime = None
+        self.endTime = None
+        self._perf_start = None
+        self._perf_end = None
+        self.duration = None
+
+    def start(self):
+        self.startTime = convert.to_date().astimezone()
+        self._perf_start = time.perf_counter()
+        return self
+
+    def stop(self):
+        self.endTime = convert.to_date().astimezone()
+        if not self._perf_start:
+            self._perf_start = time.perf_counter()
+        self._perf_end = time.perf_counter()
+        self.duration = convert.to_human_readable(self._perf_end - self._perf_start)
+
+    def __str__(self):
+        return f"START: {self.startTime}\nEND: {self.endTime}\nDURATION: {self.duration}"
+
+
 class Environment:
     """
     simple class to encapsulate overriding environment variable values if they exist
     """
     VARIABLE_DATA_TYPES = ["str", "bool", "int", "date"]
     DEFAULT_SECRET_PROPERTIES = ("PW", "PWD", "PASSWORD")
```

### Comparing `python-ubercode-utils-1.0.3/ubercode/utils/json.py` & `python-ubercode-utils-1.0.4/ubercode/utils/json.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.3/ubercode/utils/logging.py` & `python-ubercode-utils-1.0.4/ubercode/utils/logging.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.3/ubercode/utils/urls.py` & `python-ubercode-utils-1.0.4/ubercode/utils/urls.py`

 * *Files identical despite different names*

### Comparing `python-ubercode-utils-1.0.3/ubercode/utils/xml.py` & `python-ubercode-utils-1.0.4/ubercode/utils/xml.py`

 * *Files identical despite different names*

