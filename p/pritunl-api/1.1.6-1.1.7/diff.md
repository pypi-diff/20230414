# Comparing `tmp/pritunl_api-1.1.6.tar.gz` & `tmp/pritunl_api-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pritunl_api-1.1.6.tar", max compression
+gzip compressed data, was "pritunl_api-1.1.7.tar", max compression
```

## Comparing `pritunl_api-1.1.6.tar` & `pritunl_api-1.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1097 2023-03-20 04:19:29.857393 pritunl_api-1.1.6/LICENSE
--rw-r--r--   0        0        0     5498 2023-03-27 16:22:56.214332 pritunl_api-1.1.6/README.md
--rw-r--r--   0        0        0    15532 2023-03-28 07:11:20.906890 pritunl_api-1.1.6/pritunl_api/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 16:22:56.215232 pritunl_api-1.1.6/pritunl_api/utils/__init__.py
--rw-r--r--   0        0        0      413 2023-03-27 16:22:56.215533 pritunl_api-1.1.6/pritunl_api/utils/genkey.py
--rw-r--r--   0        0        0      603 2023-03-27 16:22:56.215737 pritunl_api-1.1.6/pritunl_api/utils/query.py
--rw-r--r--   0        0        0      952 2023-03-27 16:22:56.216443 pritunl_api-1.1.6/pritunl_api_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 07:11:20.907060 pritunl_api-1.1.6/pritunl_api_cli/commands/__init__.py
--rw-r--r--   0        0        0     5323 2023-03-27 16:22:56.216735 pritunl_api-1.1.6/pritunl_api_cli/commands/users.py
--rw-r--r--   0        0        0     1953 2023-03-28 07:11:20.907569 pritunl_api-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     7442 1970-01-01 00:00:00.000000 pritunl_api-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-03-20 04:19:29.857393 pritunl_api-1.1.7/LICENSE
+-rw-r--r--   0        0        0     5539 2023-04-14 19:31:59.444906 pritunl_api-1.1.7/README.md
+-rw-r--r--   0        0        0    15607 2023-04-14 16:33:56.576948 pritunl_api-1.1.7/pritunl_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 16:22:56.215232 pritunl_api-1.1.7/pritunl_api/utils/__init__.py
+-rw-r--r--   0        0        0      413 2023-03-27 16:22:56.215533 pritunl_api-1.1.7/pritunl_api/utils/genkey.py
+-rw-r--r--   0        0        0      603 2023-03-27 16:22:56.215737 pritunl_api-1.1.7/pritunl_api/utils/query.py
+-rw-r--r--   0        0        0     1079 2023-04-14 17:13:49.659799 pritunl_api-1.1.7/pritunl_api_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-28 07:11:20.907060 pritunl_api-1.1.7/pritunl_api_cli/commands/__init__.py
+-rw-r--r--   0        0        0     7268 2023-04-14 19:31:59.445306 pritunl_api-1.1.7/pritunl_api_cli/commands/users.py
+-rw-r--r--   0        0        0     1953 2023-04-14 19:32:45.517421 pritunl_api-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     7483 1970-01-01 00:00:00.000000 pritunl_api-1.1.7/PKG-INFO
```

### Comparing `pritunl_api-1.1.6/LICENSE` & `pritunl_api-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pritunl_api-1.1.6/README.md` & `pritunl_api-1.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -170,49 +170,50 @@
 
 ```bash
 pritunl-api-cli delete-user \
   --org-name develop-network \
   --user-name developer_1
 ```
 
-#### Get User Information
+#### Get User Information with Profile Key
 
 ```bash
 pritunl-api-cli get-user \
   --org-name develop-network \
   --user-name developer_1
 ```
 
-> Or get (regenerate) the profile key of a user
+> Or get user profile advanced information
 
 ```bash
 pritunl-api-cli get-user \
   --org-name develop-network \
   --user-name developer_1 \
-  --get-profile-key-only
+  --show-advanced-details
 ```
 
 #### Update a User
 
 To disable a user
 
 ```bash
 pritunl-api-cli update-user \
   --org-name develop-network \
   --user-name developer_1 \
   --disable
 ```
 
-To enable a user
+To enable a user with new PIN
 
 ```bash
 pritunl-api-cli update-user \
   --org-name developer-network \
   --user-name developer_1 \
   --enable
+  --pin 123456
 ```
 
 ## API Development
 
 ### Using Virtual Environment
 
 Create a virtual environment and activate it.
```

### Comparing `pritunl_api-1.1.6/pritunl_api/__init__.py` & `pritunl_api-1.1.7/pritunl_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-__version__ = "1.1.6"
+from pkg_resources import get_distribution
+__version__ = get_distribution('pritunl-api').version
 
 import json
 import logging as log
 import sys
 import base64
 import hashlib
 import hmac
```

### Comparing `pritunl_api-1.1.6/pritunl_api/utils/query.py` & `pritunl_api-1.1.7/pritunl_api/utils/query.py`

 * *Files identical despite different names*

### Comparing `pritunl_api-1.1.6/pritunl_api_cli/__init__.py` & `pritunl_api-1.1.7/pritunl_api_cli/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import click
 
 # Pritunl
 from .commands import users
 
 @click.group()
-def run():
+@click.version_option(package_name='pritunl-api')
+@click.pass_context
+def run(ctx):
     pass
 
 # Get User
 @run.command()
 @click.option('--org-name')
 @click.option('--user-name')
-@click.option('--get-profile-key-only', is_flag=True)
+@click.option('--show-advanced-details', is_flag=True)
 def get_user(**kwargs):
     users.get_user(**kwargs)
 
 # Create User
 @run.command()
 @click.option('--org-name')
 @click.option('--user-name')
@@ -26,14 +28,16 @@
 def create_user(**kwargs):
     users.create_user(**kwargs)
 
 # Update User
 @run.command()
 @click.option('--org-name')
 @click.option('--user-name')
+@click.option('--pin')
+@click.option('--yubikey-id')
 @click.option('--disable/--enable', default=False)
 def update_user(**kwargs):
     users.update_user(**kwargs)
 
 # Delete User
 @run.command()
 @click.option('--org-name')
```

### Comparing `pritunl_api-1.1.6/pyproject.toml` & `pritunl_api-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pritunl-api"
-version = "1.1.6"
+version = "1.1.7"
 description = "Pritunl API Client for Python"
 authors = ["Nathaniel Varona <nathaniel.varona+pypi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `pritunl_api-1.1.6/PKG-INFO` & `pritunl_api-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pritunl-api
-Version: 1.1.6
+Version: 1.1.7
 Summary: Pritunl API Client for Python
 License: MIT
 Author: Nathaniel Varona
 Author-email: nathaniel.varona+pypi@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -213,49 +213,50 @@
 
 ```bash
 pritunl-api-cli delete-user \
   --org-name develop-network \
   --user-name developer_1
 ```
 
-#### Get User Information
+#### Get User Information with Profile Key
 
 ```bash
 pritunl-api-cli get-user \
   --org-name develop-network \
   --user-name developer_1
 ```
 
-> Or get (regenerate) the profile key of a user
+> Or get user profile advanced information
 
 ```bash
 pritunl-api-cli get-user \
   --org-name develop-network \
   --user-name developer_1 \
-  --get-profile-key-only
+  --show-advanced-details
 ```
 
 #### Update a User
 
 To disable a user
 
 ```bash
 pritunl-api-cli update-user \
   --org-name develop-network \
   --user-name developer_1 \
   --disable
 ```
 
-To enable a user
+To enable a user with new PIN
 
 ```bash
 pritunl-api-cli update-user \
   --org-name developer-network \
   --user-name developer_1 \
   --enable
+  --pin 123456
 ```
 
 ## API Development
 
 ### Using Virtual Environment
 
 Create a virtual environment and activate it.
```

