# Comparing `tmp/katalytic-pkg-0.2.5.tar.gz` & `tmp/katalytic-pkg-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-pkg-0.2.5.tar", last modified: Fri Apr 14 17:47:10 2023, max compression
+gzip compressed data, was "katalytic-pkg-0.2.6.tar", last modified: Fri Apr 14 18:15:14 2023, max compression
```

## Comparing `katalytic-pkg-0.2.5.tar` & `katalytic-pkg-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       54 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/.gitignore
--rw-r--r--   0        0        0      841 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/.gitlab-ci.yml
--rw-r--r--   0        0        0      486 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/.travis.yml
--rw-r--r--   0        0        0     1317 2023-04-14 17:47:06.390334 katalytic-pkg-0.2.5/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/LICENSE.txt
--rw-r--r--   0        0        0     1542 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/README.md
--rw-r--r--   0        0        0     1399 2023-04-14 17:47:05.946334 katalytic-pkg-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      228 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/scripts/cleanup.sh
--rw-r--r--   0        0        0     1262 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/scripts/pytest.sh
--rw-r--r--   0        0        0     2867 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/scripts/release.sh
--rw-r--r--   0        0        0      470 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/scripts/setup.sh
--rw-r--r--   0        0        0      144 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/scripts/should_skip_release.sh
--rw-r--r--   0        0        0      239 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/scripts/should_skip_travis_build.sh
--rw-r--r--   0        0        0     1699 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/scripts/venv.sh
--rw-r--r--   0        0        0     4366 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/src/katalytic/pkg.py
--rw-r--r--   0        0        0     2829 2023-04-14 17:46:27.530329 katalytic-pkg-0.2.5/tests/test_pkg.py
--rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 katalytic-pkg-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       54 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/.gitlab-ci.yml
+-rw-r--r--   0        0        0      486 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/.travis.yml
+-rw-r--r--   0        0        0     1726 2023-04-14 18:15:09.736616 katalytic-pkg-0.2.6/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/LICENSE.txt
+-rw-r--r--   0        0        0     1542 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/README.md
+-rw-r--r--   0        0        0     1399 2023-04-14 18:15:09.232868 katalytic-pkg-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      228 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1262 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/pytest.sh
+-rw-r--r--   0        0        0     2867 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/release.sh
+-rw-r--r--   0        0        0      470 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/setup.sh
+-rw-r--r--   0        0        0      144 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/should_skip_release.sh
+-rw-r--r--   0        0        0      239 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/should_skip_travis_build.sh
+-rw-r--r--   0        0        0     1699 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/scripts/venv.sh
+-rw-r--r--   0        0        0     4107 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/src/katalytic/pkg.py
+-rw-r--r--   0        0        0     2829 2023-04-14 18:14:30.164410 katalytic-pkg-0.2.6/tests/test_pkg.py
+-rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 katalytic-pkg-0.2.6/PKG-INFO
```

### Comparing `katalytic-pkg-0.2.5/.gitignore` & `katalytic-pkg-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.5/.gitlab-ci.yml` & `katalytic-pkg-0.2.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.5/CHANGELOG.md` & `katalytic-pkg-0.2.6/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.2.6 (2023-04-14)
+### Fix
+* Merge branch 'main' of gitlab.com:katalytic/katalytic-pkg ([`1710c63`](https://github.com/katalytic/katalytic-pkg/commit/1710c6341d1f367d56ec673afd4bf588067fb484))
+* **get_version:** Return the correct version for katalytic instead of the one of the first plugin found ([`577cc8e`](https://github.com/katalytic/katalytic-pkg/commit/577cc8ebb588fd63172b97b5811b379a3395a531))
+
+
 ## 0.2.5 (2023-04-14)
 ### Fix
 * **get_version:** Retry build ([`c9ef45d`](https://github.com/katalytic/katalytic-pkg/commit/c9ef45d3ee1850510263da7fee50b9f11b1f14a8))
 * **get_version:** Retry build ([`1d27e2d`](https://github.com/katalytic/katalytic-pkg/commit/1d27e2d364afc3f2628e0c623a15f9d317a83cec))
 * **get_version:** Prevent infinite loop in an edge case ([`d6669f6`](https://github.com/katalytic/katalytic-pkg/commit/d6669f6c647d10ca470056bb9a9c65b2b38b7468))
```

### Comparing `katalytic-pkg-0.2.5/LICENSE.txt` & `katalytic-pkg-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.5/README.md` & `katalytic-pkg-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.5/pyproject.toml` & `katalytic-pkg-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-pkg"
-version = "0.2.5"
+version = "0.2.6"
 description = "This plugin provides some metaprogramming magic for the other katalytic plugins"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-pkg-0.2.5/scripts/conda.sh` & `katalytic-pkg-0.2.6/scripts/conda.sh`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.5/scripts/find_requirements.py` & `katalytic-pkg-0.2.6/scripts/find_requirements.py`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.5/scripts/release.sh` & `katalytic-pkg-0.2.6/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.5/scripts/venv.sh` & `katalytic-pkg-0.2.6/scripts/venv.sh`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.5/src/katalytic/pkg.py` & `katalytic-pkg-0.2.6/src/katalytic/pkg.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,33 +14,27 @@
     with open(path, 'r') as f:
         for line in f:
             if line.startswith('Version:'):
                 return line.split(':')[-1].strip()
 
 
 def __find_paths(pkg):
-    pkg2 = pkg.replace('-', '.').replace('_', '.')
-    prefix = '[^/]+'.join(pkg2.split('.'))
-
+    pkg = pkg.replace('-', '_').replace('.', '_')
     for p in sys.path:
         if not Path(p).is_dir():
             continue
 
         for p2 in iglob(f'{p}/**.dist-info', recursive=True):
-            if '__pycache__' in p2:
-                continue
-            elif re.search(f'{prefix}[^/]*[.]dist-info', p2):
+            if re.search(f'{pkg}-[^/]*[.]dist-info', p2):
                 yield p2
                 if Path(f'{p2}/METADATA').is_file():
                     yield p2
 
         for p2 in iglob(f'{p}/**.egg-info', recursive=True):
-            if '__pycache__' in p2:
-                continue
-            elif re.search(f'{prefix}[^/]*[.]egg-info', p2):
+            if re.search(f'{pkg}-[^/]*[.]egg-info', p2):
                 yield p2
                 if Path(f'{p2}/PKG-INFO').is_file():
                     yield f'{p2}/PKG-INFO'
 
 
 def get_version(dunder_name):  # pragma: no cover -- I can't test all branches at the same time
     if sys.version_info >= (3, 8):
@@ -68,18 +62,16 @@
                 break
 
     if version:
         version_info = tuple(map(int, version.split('.')))
     else:
         version_info = None
 
-    # If nothing worked and version is None, I would rather not raise an exception.
-    # The package can be used without the version
-    # This could happen if the package is installed on python 3.6
-    # python 3.8 works fine
+    # If nothing worked, I would rather return None than raise an exception
+    # This could happen if the package is installed on python < 3.8
     return version, version_info
 
 
 __version__, __version_info__ = get_version(__name__)
 
 
 def _get_stacktrace(e):
```

### Comparing `katalytic-pkg-0.2.5/tests/test_pkg.py` & `katalytic-pkg-0.2.6/tests/test_pkg.py`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.5/PKG-INFO` & `katalytic-pkg-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-pkg
-Version: 0.2.5
+Version: 0.2.6
 Summary: This plugin provides some metaprogramming magic for the other katalytic plugins
 Keywords: high-level,metaprogramming
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

