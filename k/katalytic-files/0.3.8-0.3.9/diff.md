# Comparing `tmp/katalytic-files-0.3.8.tar.gz` & `tmp/katalytic-files-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-files-0.3.8.tar", last modified: Wed Apr 12 17:54:56 2023, max compression
+gzip compressed data, was "katalytic-files-0.3.9.tar", last modified: Wed Apr 12 18:10:32 2023, max compression
```

## Comparing `katalytic-files-0.3.8.tar` & `katalytic-files-0.3.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0       87 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/.gitignore
--rw-r--r--   0        0        0      841 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/.gitlab-ci.yml
--rw-r--r--   0        0        0      376 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/.travis.yml
--rw-r--r--   0        0        0      349 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/LICENSE.txt
--rw-r--r--   0        0        0     1905 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/README.md
--rw-r--r--   0        0        0     1609 2023-04-12 17:54:50.784596 katalytic-files-0.3.8/pyproject.toml
--rw-r--r--   0        0        0       14 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/requirements.txt
--rw-r--r--   0        0        0      234 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/cleanup.sh
--rw-r--r--   0        0        0     1270 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/pytest.sh
--rw-r--r--   0        0        0     2209 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/release.sh
--rw-r--r--   0        0        0      403 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/setup.sh
--rw-r--r--   0        0        0     1707 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/scripts/venv.sh
--rw-r--r--   0        0        0    11060 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/src/katalytic/files.py
--rw-r--r--   0        0        0    39566 2023-04-12 17:54:34.688647 katalytic-files-0.3.8/tests/test_files.py
--rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 katalytic-files-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/.gitlab-ci.yml
+-rw-r--r--   0        0        0      399 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/.travis.yml
+-rw-r--r--   0        0        0      349 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/LICENSE.txt
+-rw-r--r--   0        0        0     1905 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/README.md
+-rw-r--r--   0        0        0     1609 2023-04-12 18:10:26.961470 katalytic-files-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0       14 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/requirements.txt
+-rw-r--r--   0        0        0      234 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1270 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/pytest.sh
+-rw-r--r--   0        0        0     2209 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/release.sh
+-rw-r--r--   0        0        0      403 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/setup.sh
+-rw-r--r--   0        0        0      233 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/should_skip.sh
+-rw-r--r--   0        0        0     1707 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/scripts/venv.sh
+-rw-r--r--   0        0        0    11060 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/src/katalytic/files.py
+-rw-r--r--   0        0        0    39566 2023-04-12 18:10:11.697842 katalytic-files-0.3.9/tests/test_files.py
+-rw-r--r--   0        0        0     3046 1970-01-01 00:00:00.000000 katalytic-files-0.3.9/PKG-INFO
```

### Comparing `katalytic-files-0.3.8/.gitignore` & `katalytic-files-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.8/.gitlab-ci.yml` & `katalytic-files-0.3.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.8/LICENSE.txt` & `katalytic-files-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.8/README.md` & `katalytic-files-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.8/pyproject.toml` & `katalytic-files-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-files"
-version = "0.3.8"
+version = "0.3.9"
 
 description = "This plugin adds utilities for working with files to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `katalytic-files-0.3.8/scripts/conda.sh` & `katalytic-files-0.3.9/scripts/conda.sh`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.8/scripts/find_requirements.py` & `katalytic-files-0.3.9/scripts/find_requirements.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.8/scripts/release.sh` & `katalytic-files-0.3.9/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.8/scripts/venv.sh` & `katalytic-files-0.3.9/scripts/venv.sh`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.8/src/katalytic/files.py` & `katalytic-files-0.3.9/src/katalytic/files.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.8/tests/test_files.py` & `katalytic-files-0.3.9/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.8/PKG-INFO` & `katalytic-files-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-files
-Version: 0.3.8
+Version: 0.3.9
 Summary: This plugin adds utilities for working with files to the katalytic namespace
 Keywords: automation,filesystem
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

