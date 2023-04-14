# Comparing `tmp/jumpthegun-0.0.2.tar.gz` & `tmp/jumpthegun-0.0.3.tar.gz`

## Comparing `jumpthegun-0.0.2.tar` & `jumpthegun-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/.flake8
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/test_requirements.txt
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tox.ini
--rwxr-xr-x   0        0        0     3343 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun.sh
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/__version__.py
--rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/jumpthegunctl.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/output_redirect.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/project.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/testutils.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/tools.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/__init__.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/LICENSE
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/README.md
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/VERSION
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/__init__.py
--rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/_api.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/_error.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/_soft.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/_unix.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/_util.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/_windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/test_jumpthegun.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/test_tools.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/testproj/.flake8
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/testproj/bad.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/testproj/good.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/testproj/pyproject.toml
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/LICENSE
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/README.md
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/.flake8
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/test_requirements.txt
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tox.ini
+-rwxr-xr-x   0        0        0     3343 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun.sh
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/__version__.py
+-rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/jumpthegunctl.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/output_redirect.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/project.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/testutils.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/tools.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/__init__.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/LICENSE
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/README.md
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/VERSION
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/__init__.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/_api.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/_error.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/_soft.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/_unix.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/_util.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/_windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/test_jumpthegun.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/test_tools.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/testproj/.flake8
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/testproj/bad.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/testproj/good.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/testproj/pyproject.toml
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/README.md
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/PKG-INFO
```

### Comparing `jumpthegun-0.0.2/src/jumpthegun.sh` & `jumpthegun-0.0.3/src/jumpthegun.sh`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/src/jumpthegun/jumpthegunctl.py` & `jumpthegun-0.0.3/src/jumpthegun/jumpthegunctl.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/src/jumpthegun/output_redirect.py` & `jumpthegun-0.0.3/src/jumpthegun/output_redirect.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/src/jumpthegun/project.py` & `jumpthegun-0.0.3/src/jumpthegun/project.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/src/jumpthegun/tools.py` & `jumpthegun-0.0.3/src/jumpthegun/tools.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/src/jumpthegun/utils.py` & `jumpthegun-0.0.3/src/jumpthegun/utils.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/src/vendor/filelock/LICENSE` & `jumpthegun-0.0.3/src/vendor/filelock/LICENSE`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/src/vendor/filelock/README.md` & `jumpthegun-0.0.3/src/vendor/filelock/README.md`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/src/vendor/filelock/__init__.py` & `jumpthegun-0.0.3/src/vendor/filelock/__init__.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/src/vendor/filelock/_api.py` & `jumpthegun-0.0.3/src/vendor/filelock/_api.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/src/vendor/filelock/_soft.py` & `jumpthegun-0.0.3/src/vendor/filelock/_soft.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/src/vendor/filelock/_unix.py` & `jumpthegun-0.0.3/src/vendor/filelock/_unix.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/src/vendor/filelock/_util.py` & `jumpthegun-0.0.3/src/vendor/filelock/_util.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/src/vendor/filelock/_windows.py` & `jumpthegun-0.0.3/src/vendor/filelock/_windows.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/tests/test_jumpthegun.py` & `jumpthegun-0.0.3/tests/test_jumpthegun.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/tests/test_tools.py` & `jumpthegun-0.0.3/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/.gitignore` & `jumpthegun-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/LICENSE` & `jumpthegun-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/README.md` & `jumpthegun-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -20,30 +20,61 @@
 
 # Installation
 
 Install into the same Python env where you have tools like black or flake8
 installed:
 
 ```shell
-pip install git+https://github.com/taleinat/jumpthegun.git
+pip install jumpthegun
 ```
 
 
 # Usage
 
 Example:
 
 ```shell
-jumpthegun start black
+jumpthegun run black --help
+
+time black --help
 time jumpthegun run black --help
+
 time black --check .
 time jumpthegun run black --check .
-jumpthegun stop black
 ```
 
+## With pre-commit
+
+[pre-commit](https://pre-commit.com/) is awesome, but it makes commits slower.
+JumpTheGun fixes that!
+
+Example config (`.pre-commit-config.yaml`):
+```yaml
+repos:
+- repo: https://github.com/PyCQA/flake8
+  rev: 6.0.0
+  hooks:
+  - id: flake8
+    entry: jumpthegun run flake8
+    additional_dependencies:
+    - jumpthegun
+```
+
+You may need to run `pre-commit install --install-hooks` if you've changed the
+config in an existing working copy of a project.
+
+Then, edit your `.git/hooks/pre-commit` and make this change:
+
+```shell
+if [ -x "$INSTALL_PYTHON" ]; then
+    #exec "$INSTALL_PYTHON" -mpre_commit "${ARGS[@]}"
+    exec jumpthegun run pre-commit "${ARGS[@]}"
+```
+
+
 # Copyright & License
 
 Copyright 2022-2023 Tal Einat.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `jumpthegun-0.0.2/pyproject.toml` & `jumpthegun-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.2/PKG-INFO` & `jumpthegun-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jumpthegun
-Version: 0.0.2
+Version: 0.0.3
 Summary: Make Python CLI tools win the speed race, by cheating!
 Project-URL: Homepage, https://github.com/taleinat/jumpthegun
 Author-email: Tal Einat <taleinat@gmail.com>
 License: Apache-2.0
 License-File: LICENSE
 Keywords: cli
 Classifier: Development Status :: 1 - Planning
@@ -49,30 +49,61 @@
 
 # Installation
 
 Install into the same Python env where you have tools like black or flake8
 installed:
 
 ```shell
-pip install git+https://github.com/taleinat/jumpthegun.git
+pip install jumpthegun
 ```
 
 
 # Usage
 
 Example:
 
 ```shell
-jumpthegun start black
+jumpthegun run black --help
+
+time black --help
 time jumpthegun run black --help
+
 time black --check .
 time jumpthegun run black --check .
-jumpthegun stop black
 ```
 
+## With pre-commit
+
+[pre-commit](https://pre-commit.com/) is awesome, but it makes commits slower.
+JumpTheGun fixes that!
+
+Example config (`.pre-commit-config.yaml`):
+```yaml
+repos:
+- repo: https://github.com/PyCQA/flake8
+  rev: 6.0.0
+  hooks:
+  - id: flake8
+    entry: jumpthegun run flake8
+    additional_dependencies:
+    - jumpthegun
+```
+
+You may need to run `pre-commit install --install-hooks` if you've changed the
+config in an existing working copy of a project.
+
+Then, edit your `.git/hooks/pre-commit` and make this change:
+
+```shell
+if [ -x "$INSTALL_PYTHON" ]; then
+    #exec "$INSTALL_PYTHON" -mpre_commit "${ARGS[@]}"
+    exec jumpthegun run pre-commit "${ARGS[@]}"
+```
+
+
 # Copyright & License
 
 Copyright 2022-2023 Tal Einat.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

