# Comparing `tmp/aiven-client-2.8.0.tar.gz` & `tmp/aiven-client-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiven-client-2.8.0.tar", last modified: Fri Dec  4 04:27:42 2020, max compression
+gzip compressed data, was "dist/aiven-client-2.9.0.tar", last modified: Thu Dec 17 14:39:02 2020, max compression
```

## Comparing `aiven-client-2.8.0.tar` & `aiven-client-2.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 mts       (1000) mts       (1000)        0 2020-12-04 04:27:42.803398 aiven-client-2.8.0/
--rw-rw-r--   0 mts       (1000) mts       (1000)    11358 2020-11-09 09:34:55.000000 aiven-client-2.8.0/LICENSE
--rw-rw-r--   0 mts       (1000) mts       (1000)      206 2020-11-09 09:34:55.000000 aiven-client-2.8.0/MANIFEST.in
--rw-rw-r--   0 mts       (1000) mts       (1000)    13143 2020-12-04 04:27:42.803398 aiven-client-2.8.0/PKG-INFO
--rw-rw-r--   0 mts       (1000) mts       (1000)     9706 2020-11-09 09:34:55.000000 aiven-client-2.8.0/README.rst
-drwxrwxr-x   0 mts       (1000) mts       (1000)        0 2020-12-04 04:27:42.800398 aiven-client-2.8.0/aiven/
--rw-rw-r--   0 mts       (1000) mts       (1000)       76 2020-11-09 09:34:55.000000 aiven-client-2.8.0/aiven/__init__.py
-drwxrwxr-x   0 mts       (1000) mts       (1000)        0 2020-12-04 04:27:42.801398 aiven-client-2.8.0/aiven/client/
--rw-rw-r--   0 mts       (1000) mts       (1000)      178 2020-11-09 09:34:55.000000 aiven-client-2.8.0/aiven/client/__init__.py
--rw-rw-r--   0 mts       (1000) mts       (1000)      102 2020-11-09 09:34:55.000000 aiven-client-2.8.0/aiven/client/__main__.py
--rw-rw-r--   0 mts       (1000) mts       (1000)     9849 2020-11-13 11:20:53.000000 aiven-client-2.8.0/aiven/client/argx.py
--rw-rw-r--   0 mts       (1000) mts       (1000)   148826 2020-12-04 03:18:14.000000 aiven-client-2.8.0/aiven/client/cli.py
--rw-rw-r--   0 mts       (1000) mts       (1000)     6017 2020-12-01 13:22:36.000000 aiven-client-2.8.0/aiven/client/cliarg.py
--rw-rw-r--   0 mts       (1000) mts       (1000)    63812 2020-12-02 10:32:10.000000 aiven-client-2.8.0/aiven/client/client.py
--rw-rw-r--   0 mts       (1000) mts       (1000)      779 2020-11-09 09:34:55.000000 aiven-client-2.8.0/aiven/client/envdefault.py
--rw-rw-r--   0 mts       (1000) mts       (1000)     5214 2020-11-09 09:34:55.000000 aiven-client-2.8.0/aiven/client/pretty.py
--rw-rw-r--   0 mts       (1000) mts       (1000)       22 2020-12-04 04:27:42.000000 aiven-client-2.8.0/aiven/client/version.py
-drwxrwxr-x   0 mts       (1000) mts       (1000)        0 2020-12-04 04:27:42.801398 aiven-client-2.8.0/aiven_client.egg-info/
--rw-rw-r--   0 mts       (1000) mts       (1000)    13143 2020-12-04 04:27:42.000000 aiven-client-2.8.0/aiven_client.egg-info/PKG-INFO
--rw-rw-r--   0 mts       (1000) mts       (1000)      585 2020-12-04 04:27:42.000000 aiven-client-2.8.0/aiven_client.egg-info/SOURCES.txt
--rw-rw-r--   0 mts       (1000) mts       (1000)        1 2020-12-04 04:27:42.000000 aiven-client-2.8.0/aiven_client.egg-info/dependency_links.txt
--rw-rw-r--   0 mts       (1000) mts       (1000)       52 2020-12-04 04:27:42.000000 aiven-client-2.8.0/aiven_client.egg-info/entry_points.txt
--rw-rw-r--   0 mts       (1000) mts       (1000)       16 2020-12-04 04:27:42.000000 aiven-client-2.8.0/aiven_client.egg-info/requires.txt
--rw-rw-r--   0 mts       (1000) mts       (1000)        6 2020-12-04 04:27:42.000000 aiven-client-2.8.0/aiven_client.egg-info/top_level.txt
-drwxrwxr-x   0 mts       (1000) mts       (1000)        0 2020-12-04 04:27:42.802399 aiven-client-2.8.0/scripts/
--rwxrwxr-x   0 mts       (1000) mts       (1000)      105 2020-11-09 09:34:55.000000 aiven-client-2.8.0/scripts/avn
--rw-rw-r--   0 mts       (1000) mts       (1000)       38 2020-12-04 04:27:42.803398 aiven-client-2.8.0/setup.cfg
--rw-rw-r--   0 mts       (1000) mts       (1000)     1657 2020-11-09 09:34:55.000000 aiven-client-2.8.0/setup.py
-drwxrwxr-x   0 mts       (1000) mts       (1000)        0 2020-12-04 04:27:42.802399 aiven-client-2.8.0/tests/
--rw-rw-r--   0 mts       (1000) mts       (1000)        0 2020-11-09 09:34:55.000000 aiven-client-2.8.0/tests/__init__.py
--rw-rw-r--   0 mts       (1000) mts       (1000)     1202 2020-11-09 09:34:55.000000 aiven-client-2.8.0/tests/test_argx.py
--rw-rw-r--   0 mts       (1000) mts       (1000)     2185 2020-11-09 09:34:55.000000 aiven-client-2.8.0/tests/test_cli.py
--rw-rw-r--   0 mts       (1000) mts       (1000)     1044 2020-11-09 09:34:55.000000 aiven-client-2.8.0/tests/test_pretty.py
--rw-rw-r--   0 mts       (1000) mts       (1000)     1203 2020-11-09 09:34:55.000000 aiven-client-2.8.0/version.py
+drwxrwxr-x   0 rdpo      (1000) rdpo      (1000)        0 2020-12-17 14:39:02.000000 aiven-client-2.9.0/
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)    11358 2020-12-15 14:43:36.000000 aiven-client-2.9.0/LICENSE
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)      206 2020-12-15 14:43:36.000000 aiven-client-2.9.0/MANIFEST.in
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)    13143 2020-12-17 14:39:02.000000 aiven-client-2.9.0/PKG-INFO
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)     9706 2020-12-15 14:43:36.000000 aiven-client-2.9.0/README.rst
+drwxrwxr-x   0 rdpo      (1000) rdpo      (1000)        0 2020-12-17 14:39:02.000000 aiven-client-2.9.0/aiven/
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)       76 2020-12-15 14:43:36.000000 aiven-client-2.9.0/aiven/__init__.py
+drwxrwxr-x   0 rdpo      (1000) rdpo      (1000)        0 2020-12-17 14:39:02.000000 aiven-client-2.9.0/aiven/client/
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)      178 2020-12-15 14:43:36.000000 aiven-client-2.9.0/aiven/client/__init__.py
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)      102 2020-12-15 14:43:36.000000 aiven-client-2.9.0/aiven/client/__main__.py
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)     9973 2020-12-16 22:08:25.000000 aiven-client-2.9.0/aiven/client/argx.py
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)   148824 2020-12-17 14:19:13.000000 aiven-client-2.9.0/aiven/client/cli.py
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)     6017 2020-12-15 14:43:36.000000 aiven-client-2.9.0/aiven/client/cliarg.py
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)    63812 2020-12-15 14:43:36.000000 aiven-client-2.9.0/aiven/client/client.py
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)      779 2020-12-15 14:43:36.000000 aiven-client-2.9.0/aiven/client/envdefault.py
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)     5214 2020-12-15 14:43:36.000000 aiven-client-2.9.0/aiven/client/pretty.py
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)       22 2020-12-17 14:37:50.000000 aiven-client-2.9.0/aiven/client/version.py
+drwxrwxr-x   0 rdpo      (1000) rdpo      (1000)        0 2020-12-17 14:39:02.000000 aiven-client-2.9.0/aiven_client.egg-info/
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)    13143 2020-12-17 14:39:02.000000 aiven-client-2.9.0/aiven_client.egg-info/PKG-INFO
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)      585 2020-12-17 14:39:02.000000 aiven-client-2.9.0/aiven_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)        1 2020-12-17 14:39:02.000000 aiven-client-2.9.0/aiven_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)       52 2020-12-17 14:39:02.000000 aiven-client-2.9.0/aiven_client.egg-info/entry_points.txt
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)       16 2020-12-17 14:39:02.000000 aiven-client-2.9.0/aiven_client.egg-info/requires.txt
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)        6 2020-12-17 14:39:02.000000 aiven-client-2.9.0/aiven_client.egg-info/top_level.txt
+drwxrwxr-x   0 rdpo      (1000) rdpo      (1000)        0 2020-12-17 14:39:02.000000 aiven-client-2.9.0/scripts/
+-rwxrwxr-x   0 rdpo      (1000) rdpo      (1000)      105 2020-12-15 14:43:36.000000 aiven-client-2.9.0/scripts/avn
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)       38 2020-12-17 14:39:02.000000 aiven-client-2.9.0/setup.cfg
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)     1657 2020-12-15 14:43:36.000000 aiven-client-2.9.0/setup.py
+drwxrwxr-x   0 rdpo      (1000) rdpo      (1000)        0 2020-12-17 14:39:02.000000 aiven-client-2.9.0/tests/
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)        0 2020-12-15 14:43:36.000000 aiven-client-2.9.0/tests/__init__.py
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)     1202 2020-12-15 14:43:36.000000 aiven-client-2.9.0/tests/test_argx.py
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)     2308 2020-12-17 14:19:13.000000 aiven-client-2.9.0/tests/test_cli.py
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)     1044 2020-12-15 14:43:36.000000 aiven-client-2.9.0/tests/test_pretty.py
+-rw-rw-r--   0 rdpo      (1000) rdpo      (1000)     1203 2020-12-15 14:43:36.000000 aiven-client-2.9.0/version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `aiven-client-2.8.0/LICENSE` & `aiven-client-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiven-client-2.8.0/PKG-INFO` & `aiven-client-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aiven-client
-Version: 2.8.0
+Version: 2.9.0
 Summary: Aiven.io client library / command-line client
 Home-page: https://aiven.io/
 Author: Aiven
 Author-email: support@aiven.io
 License: Apache 2.0
 Description: Aiven Client |BuildStatus|_
         ===========================
```

### Comparing `aiven-client-2.8.0/README.rst` & `aiven-client-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiven-client-2.8.0/aiven/client/argx.py` & `aiven-client-2.9.0/aiven/client/argx.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,16 @@
         file=None,
     ):  # pylint: disable=redefined-builtin
         """print request response in chosen format"""
         if file is None:
             file = sys.stdout
 
         if format is not None:
+            if single_item:
+                result = [result]
             for item in result:
                 print(format.format(**item), file=file)
         elif json:
             print(
                 jsonlib.dumps(result, indent=4, sort_keys=True, cls=pretty.CustomJsonEncoder),
                 file=file,
             )
@@ -233,14 +235,16 @@
                     fields.append(field)
                 else:
                     fields.extend(field)
 
             writer = csvlib.DictWriter(file, extrasaction="ignore", fieldnames=fields)
             if header:
                 writer.writeheader()
+            if single_item:
+                result = [result]
             for item in result:
                 writer.writerow(item)
         else:
             if single_item:
                 result = [result]
 
             pretty.print_table(
```

### Comparing `aiven-client-2.8.0/aiven/client/cli.py` & `aiven-client-2.9.0/aiven/client/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1144,15 +1144,15 @@
     def service__user_create(self):
         """Create service user"""
         arg_vars = vars(self.args)
         extra_params = {}
         acl_params = {
             key: arg_vars[key].split()
             for key in {"redis_acl_keys", "redis_acl_commands", "redis_acl_categories"}
-            if key in arg_vars
+            if arg_vars[key]
         }
         if acl_params:
             extra_params = {"access_control": acl_params}
         self.client.create_service_user(
             project=self.get_project(),
             service=self.args.service_name,
             username=self.args.username,
```

### Comparing `aiven-client-2.8.0/aiven/client/cliarg.py` & `aiven-client-2.9.0/aiven/client/cliarg.py`

 * *Files identical despite different names*

### Comparing `aiven-client-2.8.0/aiven/client/client.py` & `aiven-client-2.9.0/aiven/client/client.py`

 * *Files identical despite different names*

### Comparing `aiven-client-2.8.0/aiven/client/envdefault.py` & `aiven-client-2.9.0/aiven/client/envdefault.py`

 * *Files identical despite different names*

### Comparing `aiven-client-2.8.0/aiven/client/pretty.py` & `aiven-client-2.9.0/aiven/client/pretty.py`

 * *Files identical despite different names*

### Comparing `aiven-client-2.8.0/aiven_client.egg-info/PKG-INFO` & `aiven-client-2.9.0/aiven_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aiven-client
-Version: 2.8.0
+Version: 2.9.0
 Summary: Aiven.io client library / command-line client
 Home-page: https://aiven.io/
 Author: Aiven
 Author-email: support@aiven.io
 License: Apache 2.0
 Description: Aiven Client |BuildStatus|_
         ===========================
```

### Comparing `aiven-client-2.8.0/aiven_client.egg-info/SOURCES.txt` & `aiven-client-2.9.0/aiven_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiven-client-2.8.0/setup.py` & `aiven-client-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `aiven-client-2.8.0/tests/test_argx.py` & `aiven-client-2.9.0/tests/test_argx.py`

 * *Files identical despite different names*

### Comparing `aiven-client-2.8.0/tests/test_cli.py` & `aiven-client-2.9.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,18 @@
     AivenCLI().run(args=["service", "plans"])
 
 
 def test_service_types_v():
     AivenCLI().run(args=["service", "types", "-v"])
 
 
+def test_service_user_create():
+    AivenCLI().run(args=["service", "user-create", "service", "--username", "username"])
+
+
 def test_help():
     AivenCLI().run(args=["help"])
 
 
 def test_create_user_config():
     cli = AivenCLI()
     cli.args = namedtuple("args", ["user_config", "user_option_remove"])
```

### Comparing `aiven-client-2.8.0/tests/test_pretty.py` & `aiven-client-2.9.0/tests/test_pretty.py`

 * *Files identical despite different names*

### Comparing `aiven-client-2.8.0/version.py` & `aiven-client-2.9.0/version.py`

 * *Files identical despite different names*

