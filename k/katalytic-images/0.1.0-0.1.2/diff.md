# Comparing `tmp/katalytic-images-0.1.0.tar.gz` & `tmp/katalytic-images-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-images-0.1.0.tar", last modified: Sun Apr  9 18:35:27 2023, max compression
+gzip compressed data, was "katalytic-images-0.1.2.tar", last modified: Fri Apr 14 07:28:35 2023, max compression
```

## Comparing `katalytic-images-0.1.0.tar` & `katalytic-images-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 18:35:27.688315 katalytic-images-0.1.0/
--rw-rw-r--   0 wip       (1000) wip       (1000)     1066 2023-04-06 18:07:34.000000 katalytic-images-0.1.0/LICENSE.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)     3561 2023-04-09 18:35:27.688315 katalytic-images-0.1.0/PKG-INFO
--rw-rw-r--   0 wip       (1000) wip       (1000)     1476 2023-04-06 18:07:34.000000 katalytic-images-0.1.0/README.md
--rw-rw-r--   0 wip       (1000) wip       (1000)     1226 2023-04-09 18:11:10.000000 katalytic-images-0.1.0/pyproject.toml
--rw-rw-r--   0 wip       (1000) wip       (1000)       38 2023-04-09 18:35:27.688315 katalytic-images-0.1.0/setup.cfg
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 18:35:27.688315 katalytic-images-0.1.0/src/
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 18:35:27.688315 katalytic-images-0.1.0/src/katalytic/
--rw-rw-r--   0 wip       (1000) wip       (1000)     2825 2023-04-09 13:46:15.000000 katalytic-images-0.1.0/src/katalytic/images.py
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 18:35:27.688315 katalytic-images-0.1.0/src/katalytic_images.egg-info/
--rw-rw-r--   0 wip       (1000) wip       (1000)     3561 2023-04-09 18:35:27.000000 katalytic-images-0.1.0/src/katalytic_images.egg-info/PKG-INFO
--rw-rw-r--   0 wip       (1000) wip       (1000)      300 2023-04-09 18:35:27.000000 katalytic-images-0.1.0/src/katalytic_images.egg-info/SOURCES.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)        1 2023-04-09 18:35:27.000000 katalytic-images-0.1.0/src/katalytic_images.egg-info/dependency_links.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)      146 2023-04-09 18:35:27.000000 katalytic-images-0.1.0/src/katalytic_images.egg-info/requires.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)       10 2023-04-09 18:35:27.000000 katalytic-images-0.1.0/src/katalytic_images.egg-info/top_level.txt
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 18:35:27.688315 katalytic-images-0.1.0/tests/
--rw-rw-r--   0 wip       (1000) wip       (1000)     7796 2023-04-09 14:21:03.000000 katalytic-images-0.1.0/tests/test_images.py
+-rw-r--r--   0        0        0      109 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      486 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/.travis.yml
+-rw-r--r--   0        0        0      524 2023-04-14 07:28:20.433268 katalytic-images-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     2165 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/README.md
+-rw-r--r--   0        0        0     1800 2023-04-14 07:28:19.973498 katalytic-images-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      228 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1262 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/pytest.sh
+-rw-r--r--   0        0        0     2867 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/release.sh
+-rw-r--r--   0        0        0      470 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/setup.sh
+-rw-r--r--   0        0        0      144 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/should_skip_release.sh
+-rw-r--r--   0        0        0      239 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/should_skip_travis_build.sh
+-rw-r--r--   0        0        0     1699 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/scripts/venv.sh
+-rw-r--r--   0        0        0     2825 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/src/katalytic/images.py
+-rw-r--r--   0        0        0     7796 2023-04-14 07:27:35.983502 katalytic-images-0.1.2/tests/test_images.py
+-rw-r--r--   0        0        0     3557 1970-01-01 00:00:00.000000 katalytic-images-0.1.2/PKG-INFO
```

### Comparing `katalytic-images-0.1.0/LICENSE.txt` & `katalytic-images-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.1.0/pyproject.toml` & `katalytic-images-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,70 @@
+[build-system]
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
+
 [project]
 name = "katalytic-images"
-version = "0.1.0"
+version = "0.1.2"
 description = "This plugin adds utilities for working with images and videos to the katalytic namespace"
-
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
-requires-python = ">=3.6"
-dependencies = [
-    "katalytic-files>=0.3.0",
-    "katalytic-pkg>=0.2.0",
-    "numpy>=1.14",
-    "opencv-python>=4.0.0",
-    "pillow>=8.4.0",
-]
-
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Image Processing",
+    "Topic :: Scientific/Engineering :: Visualization",
+    "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
 ]
 authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
 
+requires-python = ">=3.6"
+dependencies = [
+    "katalytic-files>=0.3.0",
+    "katalytic-pkg>=0.2.0",
+    "numpy>=1.14",
+    "opencv-python>=4.0.0",
+    "pillow>=8.4.0",
+]
+
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov",
     "pytest-randomly",
-    "pytest-repeat",
 ]
 
 [project.urls]
 homepage = "https://gitlab.com/katalytic/katalytic-images.git"
 repository = "https://gitlab.com/katalytic/katalytic-images.git"
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
+
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+env_list = py36, py37, py38, py39
+isolated_build = True
+
+[testenv]
+extras = dev
+deps = -e .
+
+commands = pytest --cov-fail-under=100 --cov=katalytic --cov-report term-missing
+"""
+
+[tool.semantic_release]
+version_variable = "pyproject.toml:version"
+branch = "main"
+
+[tool.flit.module]
+name = "katalytic.images"
```

### Comparing `katalytic-images-0.1.0/src/katalytic/images.py` & `katalytic-images-0.1.2/src/katalytic/images.py`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.1.0/tests/test_images.py` & `katalytic-images-0.1.2/tests/test_images.py`

 * *Files identical despite different names*

