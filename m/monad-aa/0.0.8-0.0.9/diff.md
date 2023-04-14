# Comparing `tmp/monad_aa-0.0.8.tar.gz` & `tmp/monad_aa-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monad_aa-0.0.8.tar", last modified: Fri Mar 24 21:01:16 2023, max compression
+gzip compressed data, was "monad_aa-0.0.9.tar", last modified: Fri Mar 24 21:41:58 2023, max compression
```

## Comparing `monad_aa-0.0.8.tar` & `monad_aa-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:01:16.555709 monad_aa-0.0.8/
--rw-r--r--   0 dmkamath   (501) staff       (20)     1068 2022-06-21 12:54:35.000000 monad_aa-0.0.8/LICENSE
--rw-r--r--   0 dmkamath   (501) staff       (20)      498 2023-03-24 21:01:16.555107 monad_aa-0.0.8/PKG-INFO
--rw-r--r--   0 dmkamath   (501) staff       (20)      760 2023-03-24 21:01:07.000000 monad_aa-0.0.8/pyproject.toml
--rw-r--r--   0 dmkamath   (501) staff       (20)       38 2023-03-24 21:01:16.555944 monad_aa-0.0.8/setup.cfg
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:01:16.525798 monad_aa-0.0.8/src/
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:01:16.530741 monad_aa-0.0.8/src/aa/
--rw-r--r--   0 dmkamath   (501) staff       (20)      322 2023-03-16 04:22:06.000000 monad_aa-0.0.8/src/aa/__init__.py
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:01:16.537259 monad_aa-0.0.8/src/aa/business_logic/
--rw-r--r--   0 dmkamath   (501) staff       (20)      120 2023-03-16 03:45:37.000000 monad_aa-0.0.8/src/aa/business_logic/authenticator.py
--rw-r--r--   0 dmkamath   (501) staff       (20)      141 2023-03-16 03:53:48.000000 monad_aa-0.0.8/src/aa/business_logic/authorizer.py
--rw-r--r--   0 dmkamath   (501) staff       (20)     3241 2023-03-18 04:11:37.000000 monad_aa-0.0.8/src/aa/business_logic/report_generator.py
--rw-r--r--   0 dmkamath   (501) staff       (20)      680 2023-03-18 03:00:59.000000 monad_aa-0.0.8/src/aa/business_logic/report_status.py
--rw-r--r--   0 dmkamath   (501) staff       (20)       78 2023-03-16 03:13:59.000000 monad_aa-0.0.8/src/aa/business_logic/report_validator.py
--rw-r--r--   0 dmkamath   (501) staff       (20)     3531 2023-03-24 19:54:56.000000 monad_aa-0.0.8/src/aa/main_interactors.py
--rw-r--r--   0 dmkamath   (501) staff       (20)     1451 2023-03-18 03:38:00.000000 monad_aa-0.0.8/src/aa/plug_point_config.py
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:01:16.548520 monad_aa-0.0.8/src/aa/plugs/
--rw-r--r--   0 dmkamath   (501) staff       (20)     1316 2023-03-18 04:41:59.000000 monad_aa-0.0.8/src/aa/plugs/aa_report_persistence_plug_in.py
--rw-r--r--   0 dmkamath   (501) staff       (20)      494 2023-03-18 03:38:00.000000 monad_aa-0.0.8/src/aa/plugs/aa_report_persistence_plug_point.py
--rw-r--r--   0 dmkamath   (501) staff       (20)     1253 2023-03-18 04:07:08.000000 monad_aa-0.0.8/src/aa/plugs/initiate_report_generation_plug_in.py
--rw-r--r--   0 dmkamath   (501) staff       (20)      451 2023-03-18 02:54:24.000000 monad_aa-0.0.8/src/aa/plugs/initiate_report_generation_plug_point.py
--rw-r--r--   0 dmkamath   (501) staff       (20)      535 2023-03-18 03:42:41.000000 monad_aa-0.0.8/src/aa/plugs/report_status_plug_in.py
--rw-r--r--   0 dmkamath   (501) staff       (20)      409 2023-03-16 03:36:31.000000 monad_aa-0.0.8/src/aa/plugs/report_status_plug_point.py
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:01:16.552125 monad_aa-0.0.8/src/monad_aa.egg-info/
--rw-r--r--   0 dmkamath   (501) staff       (20)      498 2023-03-24 21:01:16.000000 monad_aa-0.0.8/src/monad_aa.egg-info/PKG-INFO
--rw-r--r--   0 dmkamath   (501) staff       (20)      785 2023-03-24 21:01:16.000000 monad_aa-0.0.8/src/monad_aa.egg-info/SOURCES.txt
--rw-r--r--   0 dmkamath   (501) staff       (20)        1 2023-03-24 21:01:16.000000 monad_aa-0.0.8/src/monad_aa.egg-info/dependency_links.txt
--rw-r--r--   0 dmkamath   (501) staff       (20)       14 2023-03-24 21:01:16.000000 monad_aa-0.0.8/src/monad_aa.egg-info/requires.txt
--rw-r--r--   0 dmkamath   (501) staff       (20)        3 2023-03-24 21:01:16.000000 monad_aa-0.0.8/src/monad_aa.egg-info/top_level.txt
-drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:01:16.553211 monad_aa-0.0.8/tests/
--rw-r--r--   0 dmkamath   (501) staff       (20)     1009 2023-03-24 20:16:37.000000 monad_aa-0.0.8/tests/test_business_scenarios.py
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:41:58.970779 monad_aa-0.0.9/
+-rw-r--r--   0 dmkamath   (501) staff       (20)     1068 2022-06-21 12:54:35.000000 monad_aa-0.0.9/LICENSE
+-rw-r--r--   0 dmkamath   (501) staff       (20)      498 2023-03-24 21:41:58.970328 monad_aa-0.0.9/PKG-INFO
+-rw-r--r--   0 dmkamath   (501) staff       (20)      760 2023-03-24 21:41:51.000000 monad_aa-0.0.9/pyproject.toml
+-rw-r--r--   0 dmkamath   (501) staff       (20)       38 2023-03-24 21:41:58.971126 monad_aa-0.0.9/setup.cfg
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:41:58.951458 monad_aa-0.0.9/src/
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:41:58.955900 monad_aa-0.0.9/src/aa/
+-rw-r--r--   0 dmkamath   (501) staff       (20)      322 2023-03-16 04:22:06.000000 monad_aa-0.0.9/src/aa/__init__.py
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:41:58.960652 monad_aa-0.0.9/src/aa/business_logic/
+-rw-r--r--   0 dmkamath   (501) staff       (20)      120 2023-03-16 03:45:37.000000 monad_aa-0.0.9/src/aa/business_logic/authenticator.py
+-rw-r--r--   0 dmkamath   (501) staff       (20)      141 2023-03-16 03:53:48.000000 monad_aa-0.0.9/src/aa/business_logic/authorizer.py
+-rw-r--r--   0 dmkamath   (501) staff       (20)     3241 2023-03-18 04:11:37.000000 monad_aa-0.0.9/src/aa/business_logic/report_generator.py
+-rw-r--r--   0 dmkamath   (501) staff       (20)      680 2023-03-18 03:00:59.000000 monad_aa-0.0.9/src/aa/business_logic/report_status.py
+-rw-r--r--   0 dmkamath   (501) staff       (20)       78 2023-03-16 03:13:59.000000 monad_aa-0.0.9/src/aa/business_logic/report_validator.py
+-rw-r--r--   0 dmkamath   (501) staff       (20)     3527 2023-03-24 21:41:32.000000 monad_aa-0.0.9/src/aa/entry_points.py
+-rw-r--r--   0 dmkamath   (501) staff       (20)     1451 2023-03-18 03:38:00.000000 monad_aa-0.0.9/src/aa/plug_point_config.py
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:41:58.966575 monad_aa-0.0.9/src/aa/plugs/
+-rw-r--r--   0 dmkamath   (501) staff       (20)     1316 2023-03-18 04:41:59.000000 monad_aa-0.0.9/src/aa/plugs/aa_report_persistence_plug_in.py
+-rw-r--r--   0 dmkamath   (501) staff       (20)      494 2023-03-18 03:38:00.000000 monad_aa-0.0.9/src/aa/plugs/aa_report_persistence_plug_point.py
+-rw-r--r--   0 dmkamath   (501) staff       (20)     1253 2023-03-18 04:07:08.000000 monad_aa-0.0.9/src/aa/plugs/initiate_report_generation_plug_in.py
+-rw-r--r--   0 dmkamath   (501) staff       (20)      451 2023-03-18 02:54:24.000000 monad_aa-0.0.9/src/aa/plugs/initiate_report_generation_plug_point.py
+-rw-r--r--   0 dmkamath   (501) staff       (20)      535 2023-03-18 03:42:41.000000 monad_aa-0.0.9/src/aa/plugs/report_status_plug_in.py
+-rw-r--r--   0 dmkamath   (501) staff       (20)      409 2023-03-16 03:36:31.000000 monad_aa-0.0.9/src/aa/plugs/report_status_plug_point.py
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:41:58.969343 monad_aa-0.0.9/src/monad_aa.egg-info/
+-rw-r--r--   0 dmkamath   (501) staff       (20)      498 2023-03-24 21:41:58.000000 monad_aa-0.0.9/src/monad_aa.egg-info/PKG-INFO
+-rw-r--r--   0 dmkamath   (501) staff       (20)      781 2023-03-24 21:41:58.000000 monad_aa-0.0.9/src/monad_aa.egg-info/SOURCES.txt
+-rw-r--r--   0 dmkamath   (501) staff       (20)        1 2023-03-24 21:41:58.000000 monad_aa-0.0.9/src/monad_aa.egg-info/dependency_links.txt
+-rw-r--r--   0 dmkamath   (501) staff       (20)       14 2023-03-24 21:41:58.000000 monad_aa-0.0.9/src/monad_aa.egg-info/requires.txt
+-rw-r--r--   0 dmkamath   (501) staff       (20)        3 2023-03-24 21:41:58.000000 monad_aa-0.0.9/src/monad_aa.egg-info/top_level.txt
+drwxr-xr-x   0 dmkamath   (501) staff       (20)        0 2023-03-24 21:41:58.969858 monad_aa-0.0.9/tests/
+-rw-r--r--   0 dmkamath   (501) staff       (20)      997 2023-03-24 21:41:32.000000 monad_aa-0.0.9/tests/test_business_scenarios.py
```

### Comparing `monad_aa-0.0.8/LICENSE` & `monad_aa-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `monad_aa-0.0.8/pyproject.toml` & `monad_aa-0.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # build-backend = "hatchling.build"
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "monad_aa"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Dinesh Kamath", email="dmkamath@gmail.com" },
 ]
 description = "monad for concept aa"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `monad_aa-0.0.8/src/aa/business_logic/report_generator.py` & `monad_aa-0.0.9/src/aa/business_logic/report_generator.py`

 * *Files identical despite different names*

### Comparing `monad_aa-0.0.8/src/aa/business_logic/report_status.py` & `monad_aa-0.0.9/src/aa/business_logic/report_status.py`

 * *Files identical despite different names*

### Comparing `monad_aa-0.0.8/src/aa/main_interactors.py` & `monad_aa-0.0.9/src/aa/entry_points.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-main_interactors.py
+entry_points.py
 # TODO rename this to entry_points.py
 this file contains the main interactors of this monad.
 an interactor is a function that responds to business commands and
 business events.
 
 typically UI applications (or CLI) invokes commands.
 the monad responds to the commands by performing business logic.
```

### Comparing `monad_aa-0.0.8/src/aa/plug_point_config.py` & `monad_aa-0.0.9/src/aa/plug_point_config.py`

 * *Files identical despite different names*

### Comparing `monad_aa-0.0.8/src/aa/plugs/aa_report_persistence_plug_in.py` & `monad_aa-0.0.9/src/aa/plugs/aa_report_persistence_plug_in.py`

 * *Files identical despite different names*

### Comparing `monad_aa-0.0.8/src/aa/plugs/initiate_report_generation_plug_in.py` & `monad_aa-0.0.9/src/aa/plugs/initiate_report_generation_plug_in.py`

 * *Files identical despite different names*

### Comparing `monad_aa-0.0.8/src/aa/plugs/report_status_plug_in.py` & `monad_aa-0.0.9/src/aa/plugs/report_status_plug_in.py`

 * *Files identical despite different names*

### Comparing `monad_aa-0.0.8/src/monad_aa.egg-info/SOURCES.txt` & `monad_aa-0.0.9/src/monad_aa.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 pyproject.toml
 src/aa/__init__.py
-src/aa/main_interactors.py
+src/aa/entry_points.py
 src/aa/plug_point_config.py
 src/aa/business_logic/authenticator.py
 src/aa/business_logic/authorizer.py
 src/aa/business_logic/report_generator.py
 src/aa/business_logic/report_status.py
 src/aa/business_logic/report_validator.py
 src/aa/plugs/aa_report_persistence_plug_in.py
```

### Comparing `monad_aa-0.0.8/tests/test_business_scenarios.py` & `monad_aa-0.0.9/tests/test_business_scenarios.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 print("lets test as we code")
 
 
 def test_blocking_synchronous_case():
     # this is the case where the report is synchronously generated (no async or event or queue yet)
     authentication_identifier = "cookie_value"
 
-    import aa.main_interactors
-    report_id = aa.main_interactors.request_report(authentication_identifier, "1234567001", "2021-04-08")
+    import aa.entry_points
+    report_id = aa.entry_points.request_report(authentication_identifier, "1234567001", "2021-04-08")
     assert report_id is not None
 
     wait_time = 2
     count = 0
     file = None
     while True:
-        status, file = aa.main_interactors.is_report_ready(authentication_identifier, report_id)
+        status, file = aa.entry_points.is_report_ready(authentication_identifier, report_id)
         if status:
             print(f'{os.getpid()}:{threading.get_ident()}: client: {status=}. {file=}')
             break
         else:
             print(f'{os.getpid()}:{threading.get_ident()}: client: {status=}. try again in {wait_time} seconds')
             count += 1
             if count > 10:
```

