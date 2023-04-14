# Comparing `tmp/create_docker_compose-0.2.tar.gz` & `tmp/create_docker_compose-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create_docker_compose-0.2.tar", last modified: Fri Apr 14 12:48:55 2023, max compression
+gzip compressed data, was "create_docker_compose-0.3.tar", last modified: Fri Apr 14 12:51:45 2023, max compression
```

## Comparing `create_docker_compose-0.2.tar` & `create_docker_compose-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 12:48:55.228325 create_docker_compose-0.2/
--rw-rw-rw-   0        0        0     4094 2023-04-14 12:48:55.227323 create_docker_compose-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3879 2023-04-14 12:42:11.000000 create_docker_compose-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 12:48:55.193324 create_docker_compose-0.2/create_docker_compose/
--rw-rw-rw-   0        0        0        0 2023-04-14 10:39:37.000000 create_docker_compose-0.2/create_docker_compose/__init__.py
--rw-rw-rw-   0        0        0     1427 2023-04-14 10:38:15.000000 create_docker_compose-0.2/create_docker_compose/create_docker_compose.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:48:55.224324 create_docker_compose-0.2/create_docker_compose.egg-info/
--rw-rw-rw-   0        0        0     4094 2023-04-14 12:48:55.000000 create_docker_compose-0.2/create_docker_compose.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-04-14 12:48:55.000000 create_docker_compose-0.2/create_docker_compose.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 12:48:55.000000 create_docker_compose-0.2/create_docker_compose.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2023-04-14 12:48:55.000000 create_docker_compose-0.2/create_docker_compose.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 12:48:55.000000 create_docker_compose-0.2/create_docker_compose.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-04-14 12:48:55.000000 create_docker_compose-0.2/create_docker_compose.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 12:48:55.226324 create_docker_compose-0.2/create_env_file/
--rw-rw-rw-   0        0        0        0 2023-04-14 10:39:37.000000 create_docker_compose-0.2/create_env_file/__init__.py
--rw-rw-rw-   0        0        0     1361 2023-04-14 10:38:23.000000 create_docker_compose-0.2/create_env_file/create_env_file.py
--rw-rw-rw-   0        0        0       42 2023-04-14 12:48:55.229324 create_docker_compose-0.2/setup.cfg
--rw-rw-rw-   0        0        0      582 2023-04-14 12:48:35.000000 create_docker_compose-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:51:45.291115 create_docker_compose-0.3/
+-rw-rw-rw-   0        0        0     4000 2023-04-14 12:51:45.290115 create_docker_compose-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3785 2023-04-14 12:51:34.000000 create_docker_compose-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 12:51:45.270115 create_docker_compose-0.3/create_docker_compose/
+-rw-rw-rw-   0        0        0        0 2023-04-14 10:39:37.000000 create_docker_compose-0.3/create_docker_compose/__init__.py
+-rw-rw-rw-   0        0        0     1427 2023-04-14 10:38:15.000000 create_docker_compose-0.3/create_docker_compose/create_docker_compose.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:51:45.288116 create_docker_compose-0.3/create_docker_compose.egg-info/
+-rw-rw-rw-   0        0        0     4000 2023-04-14 12:51:45.000000 create_docker_compose-0.3/create_docker_compose.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-04-14 12:51:45.000000 create_docker_compose-0.3/create_docker_compose.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 12:51:45.000000 create_docker_compose-0.3/create_docker_compose.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2023-04-14 12:51:45.000000 create_docker_compose-0.3/create_docker_compose.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 12:51:45.000000 create_docker_compose-0.3/create_docker_compose.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-04-14 12:51:45.000000 create_docker_compose-0.3/create_docker_compose.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 12:51:45.289116 create_docker_compose-0.3/create_env_file/
+-rw-rw-rw-   0        0        0        0 2023-04-14 10:39:37.000000 create_docker_compose-0.3/create_env_file/__init__.py
+-rw-rw-rw-   0        0        0     1361 2023-04-14 10:38:23.000000 create_docker_compose-0.3/create_env_file/create_env_file.py
+-rw-rw-rw-   0        0        0       42 2023-04-14 12:51:45.291115 create_docker_compose-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      582 2023-04-14 12:51:40.000000 create_docker_compose-0.3/setup.py
```

### Comparing `create_docker_compose-0.2/PKG-INFO` & `create_docker_compose-0.3/create_docker_compose.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: create_docker_compose
-Version: 0.2
+Name: create-docker-compose
+Version: 0.3
 Description-Content-Type: text/markdown
 
 ## Index
 - 1 [Description](#1-description)
 - 2 [Version History](#2-version-history)
 - 3 [How to install](#3-how-to-install)
 - 4 [How it works](#4-how-it-works)
@@ -96,10 +96,10 @@
             "localhost",
             "neura-dbms-backend"
         ],
         "DJANGO_ALLOWED_ORIGINS": [
             "http://localhost:7003",
             "http://localhost:3003"
         ],
-        "SECRET_KEY_DBMS": "'!>&xW28tExZjhfjkknmnfslkl67jkhbgYE6H]wsX>VvC1a5ZKg'",
-        "JWT_KEY": "'21F81E7C253C4856103AD7CDB8D12D1E20D408AAA640ECCD4F9F6FC8A9983D64'"
+        "SECRET_KEY_DBMS": "'secret_key'",
+        "JWT_KEY": "'secret_key'"
     }
```

### Comparing `create_docker_compose-0.2/README.md` & `create_docker_compose-0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -91,10 +91,10 @@
             "localhost",
             "neura-dbms-backend"
         ],
         "DJANGO_ALLOWED_ORIGINS": [
             "http://localhost:7003",
             "http://localhost:3003"
         ],
-        "SECRET_KEY_DBMS": "'!>&xW28tExZjhfjkknmnfslkl67jkhbgYE6H]wsX>VvC1a5ZKg'",
-        "JWT_KEY": "'21F81E7C253C4856103AD7CDB8D12D1E20D408AAA640ECCD4F9F6FC8A9983D64'"
+        "SECRET_KEY_DBMS": "'secret_key'",
+        "JWT_KEY": "'secret_key'"
     }
```

### Comparing `create_docker_compose-0.2/create_docker_compose/create_docker_compose.py` & `create_docker_compose-0.3/create_docker_compose/create_docker_compose.py`

 * *Files identical despite different names*

### Comparing `create_docker_compose-0.2/create_docker_compose.egg-info/PKG-INFO` & `create_docker_compose-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: create-docker-compose
-Version: 0.2
+Name: create_docker_compose
+Version: 0.3
 Description-Content-Type: text/markdown
 
 ## Index
 - 1 [Description](#1-description)
 - 2 [Version History](#2-version-history)
 - 3 [How to install](#3-how-to-install)
 - 4 [How it works](#4-how-it-works)
@@ -96,10 +96,10 @@
             "localhost",
             "neura-dbms-backend"
         ],
         "DJANGO_ALLOWED_ORIGINS": [
             "http://localhost:7003",
             "http://localhost:3003"
         ],
-        "SECRET_KEY_DBMS": "'!>&xW28tExZjhfjkknmnfslkl67jkhbgYE6H]wsX>VvC1a5ZKg'",
-        "JWT_KEY": "'21F81E7C253C4856103AD7CDB8D12D1E20D408AAA640ECCD4F9F6FC8A9983D64'"
+        "SECRET_KEY_DBMS": "'secret_key'",
+        "JWT_KEY": "'secret_key'"
     }
```

### Comparing `create_docker_compose-0.2/create_env_file/create_env_file.py` & `create_docker_compose-0.3/create_env_file/create_env_file.py`

 * *Files identical despite different names*

### Comparing `create_docker_compose-0.2/setup.py` & `create_docker_compose-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='create_docker_compose',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
         'PyYAML'
     ],
     entry_points={
         'console_scripts': [
             'create_docker_compose = create_docker_compose.create_docker_compose:main',
```

