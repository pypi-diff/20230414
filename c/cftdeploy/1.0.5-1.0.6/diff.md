# Comparing `tmp/cftdeploy-1.0.5.tar.gz` & `tmp/cftdeploy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cftdeploy-1.0.5.tar", last modified: Fri Jan 13 00:54:03 2023, max compression
+gzip compressed data, was "cftdeploy-1.0.6.tar", last modified: Fri Apr 14 12:11:10 2023, max compression
```

## Comparing `cftdeploy-1.0.5.tar` & `cftdeploy-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-01-13 00:54:03.066193 cftdeploy-1.0.5/
--rw-r--r--   0 chris      (501) staff       (20)    11357 2019-04-06 19:02:14.000000 cftdeploy-1.0.5/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)       15 2019-04-13 22:31:50.000000 cftdeploy-1.0.5/MANIFEST.in
--rw-r--r--   0 chris      (501) staff       (20)     8975 2023-01-13 00:54:03.066258 cftdeploy-1.0.5/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     8629 2019-04-13 21:28:10.000000 cftdeploy-1.0.5/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-01-13 00:54:03.065180 cftdeploy-1.0.5/cftdeploy/
--rw-r--r--   0 chris      (501) staff       (20)      302 2019-12-30 01:13:59.000000 cftdeploy-1.0.5/cftdeploy/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      137 2022-03-02 22:25:03.000000 cftdeploy-1.0.5/cftdeploy/_version.py
--rw-r--r--   0 chris      (501) staff       (20)    19611 2022-03-02 22:34:29.000000 cftdeploy-1.0.5/cftdeploy/entry_points.py
--rw-r--r--   0 chris      (501) staff       (20)    10417 2020-12-11 14:51:29.000000 cftdeploy-1.0.5/cftdeploy/manifest.py
--rw-r--r--   0 chris      (501) staff       (20)     2068 2019-12-30 01:13:59.000000 cftdeploy-1.0.5/cftdeploy/skeleton.py
--rw-r--r--   0 chris      (501) staff       (20)    12426 2020-12-24 15:31:43.000000 cftdeploy-1.0.5/cftdeploy/stack.py
--rw-r--r--   0 chris      (501) staff       (20)     7496 2020-12-11 01:47:04.000000 cftdeploy-1.0.5/cftdeploy/template.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-01-13 00:54:03.066099 cftdeploy-1.0.5/cftdeploy.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     8975 2023-01-13 00:54:03.000000 cftdeploy-1.0.5/cftdeploy.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      403 2023-01-13 00:54:03.000000 cftdeploy-1.0.5/cftdeploy.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-01-13 00:54:03.000000 cftdeploy-1.0.5/cftdeploy.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)      430 2023-01-13 00:54:03.000000 cftdeploy-1.0.5/cftdeploy.egg-info/entry_points.txt
--rw-r--r--   0 chris      (501) staff       (20)       31 2023-01-13 00:54:03.000000 cftdeploy-1.0.5/cftdeploy.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       10 2023-01-13 00:54:03.000000 cftdeploy-1.0.5/cftdeploy.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)      131 2023-01-13 00:54:03.066536 cftdeploy-1.0.5/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)     1324 2019-12-30 01:13:59.000000 cftdeploy-1.0.5/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-14 12:11:10.076722 cftdeploy-1.0.6/
+-rw-r--r--   0 chris      (501) staff       (20)    11357 2019-04-06 19:02:14.000000 cftdeploy-1.0.6/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)       15 2019-04-13 22:31:50.000000 cftdeploy-1.0.6/MANIFEST.in
+-rw-r--r--   0 chris      (501) staff       (20)     8975 2023-04-14 12:11:10.076797 cftdeploy-1.0.6/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     8629 2019-04-13 21:28:10.000000 cftdeploy-1.0.6/README.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-14 12:11:10.075942 cftdeploy-1.0.6/cftdeploy/
+-rw-r--r--   0 chris      (501) staff       (20)      302 2019-12-30 01:13:59.000000 cftdeploy-1.0.6/cftdeploy/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      137 2023-04-14 12:06:08.000000 cftdeploy-1.0.6/cftdeploy/_version.py
+-rw-r--r--   0 chris      (501) staff       (20)    19631 2023-01-13 01:09:20.000000 cftdeploy-1.0.6/cftdeploy/entry_points.py
+-rw-r--r--   0 chris      (501) staff       (20)    10417 2020-12-11 14:51:29.000000 cftdeploy-1.0.6/cftdeploy/manifest.py
+-rw-r--r--   0 chris      (501) staff       (20)     2068 2019-12-30 01:13:59.000000 cftdeploy-1.0.6/cftdeploy/skeleton.py
+-rw-r--r--   0 chris      (501) staff       (20)    12426 2020-12-24 15:31:43.000000 cftdeploy-1.0.6/cftdeploy/stack.py
+-rw-r--r--   0 chris      (501) staff       (20)     7496 2020-12-11 01:47:04.000000 cftdeploy-1.0.6/cftdeploy/template.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-14 12:11:10.076614 cftdeploy-1.0.6/cftdeploy.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     8975 2023-04-14 12:11:10.000000 cftdeploy-1.0.6/cftdeploy.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      403 2023-04-14 12:11:10.000000 cftdeploy-1.0.6/cftdeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-04-14 12:11:10.000000 cftdeploy-1.0.6/cftdeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)      430 2023-04-14 12:11:10.000000 cftdeploy-1.0.6/cftdeploy.egg-info/entry_points.txt
+-rw-r--r--   0 chris      (501) staff       (20)       38 2023-04-14 12:11:10.000000 cftdeploy-1.0.6/cftdeploy.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       10 2023-04-14 12:11:10.000000 cftdeploy-1.0.6/cftdeploy.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)      131 2023-04-14 12:11:10.077071 cftdeploy-1.0.6/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)     1339 2023-04-14 12:02:59.000000 cftdeploy-1.0.6/setup.py
```

### Comparing `cftdeploy-1.0.5/LICENSE` & `cftdeploy-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cftdeploy-1.0.5/PKG-INFO` & `cftdeploy-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cftdeploy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tools and modules for managing CloudFormation Templates & Stacks
 Home-page: http://github.com/jchrisfarris/cft-deploy
 Author: Chris Farris
 Author-email: chris@room17.com
 License: Apache License 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cftdeploy-1.0.5/README.md` & `cftdeploy-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cftdeploy-1.0.5/cftdeploy/entry_points.py` & `cftdeploy-1.0.6/cftdeploy/entry_points.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,15 +438,15 @@
 def do_args(parser):
 
     parser.add_argument("--debug", help="print debugging info", action='store_true')
     parser.add_argument("-s", "--silent", help="Be Silent. Print error info only", action='store_true')
     parser.add_argument("--json", help="Return Data in json format", action='store_true')
     parser.add_argument("--env", help="Return data in bash env format", action='store_true')
     parser.add_argument("--version", help="print cft-deploy version", action='store_true')
-    parser.add_argument("--region", help="AWS Region", default=os.environ['AWS_DEFAULT_REGION'])
+    parser.add_argument("--region", help="AWS Region", default=os.getenv('AWS_DEFAULT_REGION', default='us-east-1'))
     args = parser.parse_args()
 
     if args.version:
         version()
 
     # Logging idea stolen from: https://docs.python.org/3/howto/logging.html#configuring-logging
     # create console handler and set level to debug
```

### Comparing `cftdeploy-1.0.5/cftdeploy/manifest.py` & `cftdeploy-1.0.6/cftdeploy/manifest.py`

 * *Files identical despite different names*

### Comparing `cftdeploy-1.0.5/cftdeploy/skeleton.py` & `cftdeploy-1.0.6/cftdeploy/skeleton.py`

 * *Files identical despite different names*

### Comparing `cftdeploy-1.0.5/cftdeploy/stack.py` & `cftdeploy-1.0.6/cftdeploy/stack.py`

 * *Files identical despite different names*

### Comparing `cftdeploy-1.0.5/cftdeploy/template.py` & `cftdeploy-1.0.6/cftdeploy/template.py`

 * *Files identical despite different names*

### Comparing `cftdeploy-1.0.5/cftdeploy.egg-info/PKG-INFO` & `cftdeploy-1.0.6/cftdeploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cftdeploy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tools and modules for managing CloudFormation Templates & Stacks
 Home-page: http://github.com/jchrisfarris/cft-deploy
 Author: Chris Farris
 Author-email: chris@room17.com
 License: Apache License 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cftdeploy-1.0.5/setup.py` & `cftdeploy-1.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,16 @@
   packages=find_packages(),
   py_modules=['cftdeploy'],
   url='http://github.com/jchrisfarris/cft-deploy',
   python_requires='>=3.6',
   include_package_data=True,
   install_requires=[
     'boto3 >= 1.10.0',
-    'botocore >= 1.13.0'
+    'botocore >= 1.13.0',
+    'pyyaml',
   ],
   entry_points={
     'console_scripts': [
       "cft-deploy = cftdeploy:cft_deploy",
       "cft-get-resource = cftdeploy:cft_get_resource",
       "cft-validate = cftdeploy:cft_validate",
       "cft-validate-manifest = cftdeploy:cft_validate_manifest",
```

