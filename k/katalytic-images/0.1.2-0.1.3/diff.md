# Comparing `tmp/katalytic-images-0.1.2.tar.gz` & `tmp/katalytic-images-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-images-0.1.2.tar", last modified: Fri Apr 14 07:28:35 2023, max compression
+gzip compressed data, was "katalytic-images-0.1.3.tar", last modified: Fri Apr 14 07:46:55 2023, max compression
```

## Comparing `katalytic-images-0.1.2.tar` & `katalytic-images-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      109 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/.gitignore
--rw-r--r--   0        0        0      841 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/.gitlab-ci.yml
--rw-r--r--   0        0        0      486 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/.travis.yml
--rw-r--r--   0        0        0      524 2023-04-14 07:28:20.433268 katalytic-images-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     2165 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/README.md
--rw-r--r--   0        0        0     1800 2023-04-14 07:28:19.973498 katalytic-images-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      228 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/cleanup.sh
--rw-r--r--   0        0        0     1262 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/pytest.sh
--rw-r--r--   0        0        0     2867 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/release.sh
--rw-r--r--   0        0        0      470 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/setup.sh
--rw-r--r--   0        0        0      144 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/should_skip_release.sh
--rw-r--r--   0        0        0      239 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/should_skip_travis_build.sh
--rw-r--r--   0        0        0     1699 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/venv.sh
--rw-r--r--   0        0        0     2825 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/src/katalytic/images.py
--rw-r--r--   0        0        0     7796 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/tests/test_images.py
--rw-r--r--   0        0        0     3557 1970-01-01 00:00:00.000000 katalytic-images-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      109 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0      486 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/.travis.yml
+-rw-r--r--   0        0        0      675 2023-04-14 07:46:40.322644 katalytic-images-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     2165 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/README.md
+-rw-r--r--   0        0        0     1805 2023-04-14 07:46:39.866416 katalytic-images-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      228 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1262 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/pytest.sh
+-rw-r--r--   0        0        0     2867 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/release.sh
+-rw-r--r--   0        0        0      470 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/setup.sh
+-rw-r--r--   0        0        0      144 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/should_skip_release.sh
+-rw-r--r--   0        0        0      239 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/should_skip_travis_build.sh
+-rw-r--r--   0        0        0     1699 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/scripts/venv.sh
+-rw-r--r--   0        0        0     2825 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/src/katalytic/images.py
+-rw-r--r--   0        0        0     7796 2023-04-14 07:45:57.004997 katalytic-images-0.1.3/tests/test_images.py
+-rw-r--r--   0        0        0     3562 1970-01-01 00:00:00.000000 katalytic-images-0.1.3/PKG-INFO
```

### Comparing `katalytic-images-0.1.2/.gitignore` & `katalytic-images-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.1.2/.gitlab-ci.yml` & `katalytic-images-0.1.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.1.2/CHANGELOG.md` & `katalytic-images-0.1.3/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.1.3 (2023-04-14)
+### Fix
+* Release ([`b05f06a`](https://github.com/katalytic/katalytic-images/commit/b05f06a0562caaaecb3ae78dd6167f6efd7bfdd9))
+
+
 ## 0.1.2 (2023-04-14)
 ### Fix
 * Release ([`d8dcc26`](https://github.com/katalytic/katalytic-images/commit/d8dcc26a40c78db399546ed6b03d759de46c5368))
 * Release ([`ca4c3a4`](https://github.com/katalytic/katalytic-images/commit/ca4c3a46dc9c845be9829176346a1a5e14c7eb09))
 * Prep for travis ([`4533802`](https://github.com/katalytic/katalytic-images/commit/45338021cb605202ec63645780951545a28408e9))
 * Prep for travis ([`a7ab07a`](https://github.com/katalytic/katalytic-images/commit/a7ab07abb5e2bbf5001f85039820ced1cbeec541))
```

### Comparing `katalytic-images-0.1.2/LICENSE.txt` & `katalytic-images-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.1.2/README.md` & `katalytic-images-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.1.2/pyproject.toml` & `katalytic-images-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-images"
-version = "0.1.2"
+version = "0.1.3"
 description = "This plugin adds utilities for working with images and videos to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -27,15 +27,15 @@
 authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
 
 requires-python = ">=3.6"
 dependencies = [
     "katalytic-files>=0.3.0",
     "katalytic-pkg>=0.2.0",
     "numpy>=1.14",
-    "opencv-python>=4.0.0",
+    "opencv-python>=4.0.0,<4.7",
     "pillow>=8.4.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov",
```

### Comparing `katalytic-images-0.1.2/scripts/conda.sh` & `katalytic-images-0.1.3/scripts/conda.sh`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.1.2/scripts/find_requirements.py` & `katalytic-images-0.1.3/scripts/find_requirements.py`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.1.2/scripts/release.sh` & `katalytic-images-0.1.3/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.1.2/scripts/venv.sh` & `katalytic-images-0.1.3/scripts/venv.sh`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.1.2/src/katalytic/images.py` & `katalytic-images-0.1.3/src/katalytic/images.py`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.1.2/tests/test_images.py` & `katalytic-images-0.1.3/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.1.2/PKG-INFO` & `katalytic-images-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-images
-Version: 0.1.2
+Version: 0.1.3
 Summary: This plugin adds utilities for working with images and videos to the katalytic namespace
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -17,15 +17,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Dist: katalytic-files>=0.3.0
 Requires-Dist: katalytic-pkg>=0.2.0
 Requires-Dist: numpy>=1.14
-Requires-Dist: opencv-python>=4.0.0
+Requires-Dist: opencv-python>=4.0.0,<4.7
 Requires-Dist: pillow>=8.4.0
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-images.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-images.git
 Provides-Extra: dev
```

