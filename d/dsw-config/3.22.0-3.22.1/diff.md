# Comparing `tmp/dsw-config-3.22.0.tar.gz` & `tmp/dsw-config-3.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-config-3.22.0.tar", last modified: Tue Apr  4 15:01:38 2023, max compression
+gzip compressed data, was "dsw-config-3.22.1.tar", last modified: Fri Apr 14 12:55:22 2023, max compression
```

## Comparing `dsw-config-3.22.0.tar` & `dsw-config-3.22.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:38.329535 dsw-config-3.22.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-04 15:01:32.000000 dsw-config-3.22.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-04 15:01:38.329535 dsw-config-3.22.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-04 15:01:32.000000 dsw-config-3.22.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:38.329535 dsw-config-3.22.0/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:38.329535 dsw-config-3.22.0/dsw/config/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-04 15:01:32.000000 dsw-config-3.22.0/dsw/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-04 15:01:37.000000 dsw-config-3.22.0/dsw/config/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-04 15:01:32.000000 dsw-config-3.22.0/dsw/config/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-04 15:01:32.000000 dsw-config-3.22.0/dsw/config/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-04 15:01:32.000000 dsw-config-3.22.0/dsw/config/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:01:38.329535 dsw-config-3.22.0/dsw_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-04 15:01:38.000000 dsw-config-3.22.0/dsw_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-04 15:01:38.000000 dsw-config-3.22.0/dsw_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:01:38.000000 dsw-config-3.22.0/dsw_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:01:38.000000 dsw-config-3.22.0/dsw_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-04 15:01:38.000000 dsw-config-3.22.0/dsw_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-04 15:01:38.000000 dsw-config-3.22.0/dsw_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-04 15:01:32.000000 dsw-config-3.22.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:01:38.329535 dsw-config-3.22.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:01:32.000000 dsw-config-3.22.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:22.036068 dsw-config-3.22.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-14 12:55:16.000000 dsw-config-3.22.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-14 12:55:22.036068 dsw-config-3.22.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-14 12:55:16.000000 dsw-config-3.22.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:22.028068 dsw-config-3.22.1/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:22.032068 dsw-config-3.22.1/dsw/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-14 12:55:16.000000 dsw-config-3.22.1/dsw/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-14 12:55:21.000000 dsw-config-3.22.1/dsw/config/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-14 12:55:16.000000 dsw-config-3.22.1/dsw/config/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-14 12:55:16.000000 dsw-config-3.22.1/dsw/config/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-14 12:55:16.000000 dsw-config-3.22.1/dsw/config/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:55:22.036068 dsw-config-3.22.1/dsw_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-14 12:55:22.000000 dsw-config-3.22.1/dsw_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-14 12:55:22.000000 dsw-config-3.22.1/dsw_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:22.000000 dsw-config-3.22.1/dsw_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:55:22.000000 dsw-config-3.22.1/dsw_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 12:55:22.000000 dsw-config-3.22.1/dsw_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 12:55:22.000000 dsw-config-3.22.1/dsw_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-14 12:55:16.000000 dsw-config-3.22.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:22.036068 dsw-config-3.22.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:55:16.000000 dsw-config-3.22.1/setup.py
```

### Comparing `dsw-config-3.22.0/LICENSE` & `dsw-config-3.22.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-config-3.22.0/PKG-INFO` & `dsw-config-3.22.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-config
-Version: 3.22.0
+Version: 3.22.1
 Summary: Library for DSW config manipulation
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
```

### Comparing `dsw-config-3.22.0/README.md` & `dsw-config-3.22.1/README.md`

 * *Files identical despite different names*

### Comparing `dsw-config-3.22.0/dsw/config/keys.py` & `dsw-config-3.22.1/dsw/config/keys.py`

 * *Files identical despite different names*

### Comparing `dsw-config-3.22.0/dsw/config/model.py` & `dsw-config-3.22.1/dsw/config/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,16 @@
 class MailConfig(ConfigModel):
 
     def __init__(self, enabled: bool, ssl: Optional[bool], name: str, email: str,
                  host: str, port: Optional[int], security: Optional[str],
                  auth: Optional[bool], username: Optional[str],
                  password: Optional[str], rate_limit_window: int,
                  rate_limit_count: int, timeout: int,
-                 dkim_selector: Optional[str], dkim_privkey_file: Optional[str]):
+                 dkim_selector: Optional[str] = None,
+                 dkim_privkey_file: Optional[str] = None):
         self.enabled = enabled
         self.name = name
         self.email = email
         self.host = host
         self.security = 'plain'
         if security is not None:
             self.security = security.lower()
```

### Comparing `dsw-config-3.22.0/dsw/config/parser.py` & `dsw-config-3.22.1/dsw/config/parser.py`

 * *Files identical despite different names*

### Comparing `dsw-config-3.22.0/dsw_config.egg-info/PKG-INFO` & `dsw-config-3.22.1/dsw_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-config
-Version: 3.22.0
+Version: 3.22.1
 Summary: Library for DSW config manipulation
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
```

### Comparing `dsw-config-3.22.0/pyproject.toml` & `dsw-config-3.22.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-config'
-version = "3.22.0"
+version = "3.22.1"
 description = 'Library for DSW config manipulation'
 readme = 'README.md'
 keywords = ['dsw', 'config', 'yaml', 'parser']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
```

