# Comparing `tmp/katalytic-pkg-0.2.0.tar.gz` & `tmp/katalytic-pkg-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-pkg-0.2.0.tar", last modified: Sun Apr  9 04:07:02 2023, max compression
+gzip compressed data, was "katalytic-pkg-0.2.3.tar", last modified: Fri Apr 14 07:04:22 2023, max compression
```

## Comparing `katalytic-pkg-0.2.0.tar` & `katalytic-pkg-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/
--rw-rw-r--   0 wip       (1000) wip       (1000)     1066 2023-04-07 08:03:04.000000 katalytic-pkg-0.2.0/LICENSE.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)     2815 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/PKG-INFO
--rw-rw-r--   0 wip       (1000) wip       (1000)      877 2023-04-07 08:03:04.000000 katalytic-pkg-0.2.0/README.md
--rw-rw-r--   0 wip       (1000) wip       (1000)      881 2023-04-09 04:01:05.000000 katalytic-pkg-0.2.0/pyproject.toml
--rw-rw-r--   0 wip       (1000) wip       (1000)       38 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/setup.cfg
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/src/
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/src/katalytic/
--rw-rw-r--   0 wip       (1000) wip       (1000)     4091 2023-04-09 03:58:18.000000 katalytic-pkg-0.2.0/src/katalytic/pkg.py
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/src/katalytic_pkg.egg-info/
--rw-rw-r--   0 wip       (1000) wip       (1000)     2815 2023-04-09 04:07:02.000000 katalytic-pkg-0.2.0/src/katalytic_pkg.egg-info/PKG-INFO
--rw-rw-r--   0 wip       (1000) wip       (1000)      239 2023-04-09 04:07:02.000000 katalytic-pkg-0.2.0/src/katalytic_pkg.egg-info/SOURCES.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)        1 2023-04-09 04:07:02.000000 katalytic-pkg-0.2.0/src/katalytic_pkg.egg-info/dependency_links.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)       10 2023-04-09 04:07:02.000000 katalytic-pkg-0.2.0/src/katalytic_pkg.egg-info/top_level.txt
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/tests/
--rw-rw-r--   0 wip       (1000) wip       (1000)     2604 2023-04-08 13:56:04.000000 katalytic-pkg-0.2.0/tests/test_pkg.py
+-rw-r--r--   0        0        0       54 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0      486 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/.travis.yml
+-rw-r--r--   0        0        0      644 2023-04-14 07:04:18.415191 katalytic-pkg-0.2.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     1542 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/README.md
+-rw-r--r--   0        0        0     1399 2023-04-14 07:04:17.990979 katalytic-pkg-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      228 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1262 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/pytest.sh
+-rw-r--r--   0        0        0     2823 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/release.sh
+-rw-r--r--   0        0        0      470 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/setup.sh
+-rw-r--r--   0        0        0      144 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/should_skip_release.sh
+-rw-r--r--   0        0        0      239 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/should_skip_travis_build.sh
+-rw-r--r--   0        0        0     1699 2023-04-14 07:03:41.648817 katalytic-pkg-0.2.3/scripts/venv.sh
+-rw-r--r--   0        0        0     4226 2023-04-14 07:03:41.648817 katalytic-pkg-0.2.3/src/katalytic/pkg.py
+-rw-r--r--   0        0        0     2925 2023-04-14 07:03:41.648817 katalytic-pkg-0.2.3/tests/test_pkg.py
+-rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 katalytic-pkg-0.2.3/PKG-INFO
```

### Comparing `katalytic-pkg-0.2.0/LICENSE.txt` & `katalytic-pkg-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.0/pyproject.toml` & `katalytic-pkg-0.2.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,61 @@
+[build-system]
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
+
 [project]
 name = "katalytic-pkg"
-version = "0.2.0"
+version = "0.2.3"
 description = "This plugin provides some metaprogramming magic for the other katalytic plugins"
-
 license = {file = "LICENSE.txt"}
 readme = "README.md"
-requires-python = ">=3.6"
 
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries",
 ]
 keywords = [
     "high-level",
     "metaprogramming",
 ]
-authors = [
-    {name="Valentin Neagu", email="vali19th@protonmail.com"}
+authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
+
+requires-python = ">=3.6"
+
+[project.optional-dependencies]
+dev = [
+    "pytest",
+    "pytest-cov",
+    "pytest-randomly",
 ]
 
 [project.urls]
 homepage = "https://gitlab.com/katalytic/katalytic-pkg.git"
 repository = "https://gitlab.com/katalytic/katalytic-pkg.git"
 
 [tool.pytest.ini_options]
-addopts = [
-    "--import-mode=importlib",
-]
+addopts = ["--import-mode=importlib"]
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
+name = "katalytic.pkg"
```

### Comparing `katalytic-pkg-0.2.0/src/katalytic/pkg.py` & `katalytic-pkg-0.2.3/src/katalytic/pkg.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,49 +5,54 @@
 
 from glob import iglob
 from pathlib import Path
 from importlib import import_module
 
 # NOTE: __version__ and __version_info__ are defined below get_version()
 
+
 def __get_version_from_metadata(path):
     with open(path, 'r') as f:
         for line in f:
             if line.startswith('Version:'):
                 return line.split(':')[-1].strip()
 
 
 def __find_paths(pkg):
+    pkg2 = pkg.replace('-', '.').replace('_', '.')
+    prefix = '[^/]+'.join(pkg2.split('.'))
+
     for p in sys.path:
         if not Path(p).is_dir():
             continue
 
         for p2 in iglob(f'{p}**', recursive=True):
-            if pkg not in p2:
-                continue
-            elif '__pycache__' in p2:
+
+            if '__pycache__' in p2:
                 continue
 
-            if p2.endswith('.dist-info'):
+            if re.search(f'{prefix}.*[.]dist-info', p2):
                 yield p2
                 if Path(f'{p2}/METADATA').is_file():
                     yield p2
-            elif p2.endswith('.egg-info') and Path(f'{p2}/PKG-INFO').is_file():
+            elif re.search(f'{prefix}.*[.]egg-info', p2):
                 yield p2
+                if Path(f'{p2}/PKG-INFO').is_file():
+                    yield f'{p2}/PKG-INFO'
 
 
 def get_version(dunder_name):  # pragma: no cover -- I can't test all branches at the same time
     if sys.version_info >= (3, 8):
         from importlib import metadata
         version = metadata.version(dunder_name.replace('.', '-'))
         version_info = tuple(map(int, version.split('.')))
         return version, version_info
 
     version = None
-    for p in __find_paths(dunder_name.split('.')[0]):
+    for p in __find_paths(dunder_name):
         if p.endswith('.dist-info'):
             version = re.search(r'\w+-(\d+\.\d+\.\d+)', p)
             if version:
                 version = version.group(1)
                 break
 
         if p.endswith('.dist-info/METADATA'):
@@ -61,15 +66,15 @@
                 break
 
     if version:
         version_info = tuple(map(int, version.split('.')))
     else:
         version_info = None
 
-    # Nothing worked, but I would rather not raise an exception.
+    # If nothing worked and version is None, I would rather not raise an exception.
     # The package can be used without the version
     # This could happen if the package is installed on python 3.6
     # python 3.8 works fine
     return version, version_info
 
 
 __version__, __version_info__ = get_version(__name__)
@@ -135,11 +140,12 @@
 
 
 @mark('__test_1')
 @mark('__test_2')
 @mark('__test_300')
 def __test(): pass
 
+
 @mark('__test_3::a')
 @mark('__test_3::b')
 @mark('__test_2')
 def __test_2(): pass
```

### Comparing `katalytic-pkg-0.2.0/tests/test_pkg.py` & `katalytic-pkg-0.2.3/tests/test_pkg.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import sys
+
 import pytest
 
-from katalytic.pkg import _check, get_functions_in_group, get_modules, mark
+from katalytic.pkg import _check, get_functions_in_group, get_modules, get_version, mark
 from katalytic.pkg import __version__ as pkg_version
 
 
 class Test_check:
     def test_all(self):
         assert _check(None, '') is False
         assert _check('load', 'save') is False
@@ -75,10 +77,17 @@
         found = get_functions_in_group('__test_2')
         found = [(name, groups) for name, _, groups in found]
         assert found == [
             ('__test', ['__test_2']),
             ('__test_2', ['__test_2'])
         ]
 
+@pytest.mark.skipif(sys.version_info < (3, 8), reason="In some cases it fails on python < 3.8")
 class Test_version:
-    def test_all(self):
+    def test_is_ok(self):
+        v, v_info = get_version('katalytic.pkg')
+
         assert pkg_version is not None
+        assert v is not None
+        assert v_info is not None
+        assert v == '.'.join(str(i) for i in v_info)
+        assert v == pkg_version
```

