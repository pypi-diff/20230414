# Comparing `tmp/katalytic-pkg-0.2.3.tar.gz` & `tmp/katalytic-pkg-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-pkg-0.2.3.tar", last modified: Fri Apr 14 07:04:22 2023, max compression
+gzip compressed data, was "katalytic-pkg-0.2.4.tar", last modified: Fri Apr 14 17:25:27 2023, max compression
```

## Comparing `katalytic-pkg-0.2.3.tar` & `katalytic-pkg-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       54 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/.gitignore
--rw-r--r--   0        0        0      841 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/.gitlab-ci.yml
--rw-r--r--   0        0        0      486 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/.travis.yml
--rw-r--r--   0        0        0      644 2023-04-14 07:04:18.415191 katalytic-pkg-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/LICENSE.txt
--rw-r--r--   0        0        0     1542 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/README.md
--rw-r--r--   0        0        0     1399 2023-04-14 07:04:17.990979 katalytic-pkg-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      228 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/cleanup.sh
--rw-r--r--   0        0        0     1262 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/conda.sh
--rw-r--r--   0        0        0      792 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/find_requirements.py
--rw-r--r--   0        0        0      114 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/pytest.sh
--rw-r--r--   0        0        0     2823 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/release.sh
--rw-r--r--   0        0        0      470 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/setup.sh
--rw-r--r--   0        0        0      144 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/should_skip_release.sh
--rw-r--r--   0        0        0      239 2023-04-14 07:03:41.644815 katalytic-pkg-0.2.3/scripts/should_skip_travis_build.sh
--rw-r--r--   0        0        0     1699 2023-04-14 07:03:41.648817 katalytic-pkg-0.2.3/scripts/venv.sh
--rw-r--r--   0        0        0     4226 2023-04-14 07:03:41.648817 katalytic-pkg-0.2.3/src/katalytic/pkg.py
--rw-r--r--   0        0        0     2925 2023-04-14 07:03:41.648817 katalytic-pkg-0.2.3/tests/test_pkg.py
--rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 katalytic-pkg-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       54 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/.coveragerc
+-rw-r--r--   0        0        0      641 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/.gitignore
+-rw-r--r--   0        0        0      841 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0      486 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/.travis.yml
+-rw-r--r--   0        0        0      848 2023-04-14 17:25:20.636802 katalytic-pkg-0.2.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/LICENSE.txt
+-rw-r--r--   0        0        0     1542 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/README.md
+-rw-r--r--   0        0        0     1399 2023-04-14 17:25:20.152560 katalytic-pkg-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      228 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/scripts/cleanup.sh
+-rw-r--r--   0        0        0     1262 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/scripts/conda.sh
+-rw-r--r--   0        0        0      792 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/scripts/find_requirements.py
+-rw-r--r--   0        0        0      114 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/scripts/pytest.sh
+-rw-r--r--   0        0        0     2867 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/scripts/release.sh
+-rw-r--r--   0        0        0      470 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/scripts/setup.sh
+-rw-r--r--   0        0        0      144 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/scripts/should_skip_release.sh
+-rw-r--r--   0        0        0      239 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/scripts/should_skip_travis_build.sh
+-rw-r--r--   0        0        0     1699 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/scripts/venv.sh
+-rw-r--r--   0        0        0     4226 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/src/katalytic/pkg.py
+-rw-r--r--   0        0        0     2829 2023-04-14 17:24:40.540766 katalytic-pkg-0.2.4/tests/test_pkg.py
+-rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 katalytic-pkg-0.2.4/PKG-INFO
```

### Comparing `katalytic-pkg-0.2.3/.gitignore` & `katalytic-pkg-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.3/.gitlab-ci.yml` & `katalytic-pkg-0.2.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.3/CHANGELOG.md` & `katalytic-pkg-0.2.4/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.2.4 (2023-04-14)
+### Fix
+* **get_version:** Return the correct version on py3.7 or earlier ([`139bf5c`](https://github.com/katalytic/katalytic-pkg/commit/139bf5cbbf661c23b8f375fea9a149709f88ecee))
+
+
 ## 0.2.3 (2023-04-14)
 ### Fix
 * Release ([`30cf44b`](https://github.com/katalytic/katalytic-pkg/commit/30cf44b10d0b13108cd966b45a634408d6593f1b))
 * Release ([`2948d17`](https://github.com/katalytic/katalytic-pkg/commit/2948d172dcc6be49bdf6adddef5061e33b93f08f))
 * Release ([`f35c82f`](https://github.com/katalytic/katalytic-pkg/commit/f35c82fbeabfd61de83e616744f714968d71a6b0))
```

### Comparing `katalytic-pkg-0.2.3/LICENSE.txt` & `katalytic-pkg-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.3/README.md` & `katalytic-pkg-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.3/pyproject.toml` & `katalytic-pkg-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-pkg"
-version = "0.2.3"
+version = "0.2.4"
 description = "This plugin provides some metaprogramming magic for the other katalytic plugins"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-pkg-0.2.3/scripts/conda.sh` & `katalytic-pkg-0.2.4/scripts/conda.sh`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.3/scripts/find_requirements.py` & `katalytic-pkg-0.2.4/scripts/find_requirements.py`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.3/scripts/release.sh` & `katalytic-pkg-0.2.4/scripts/release.sh`

 * *Files 5% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 		command cat CHANGELOG.md
 	else
 		echo "No version bump. Exiting ..."
 		sleep 2
 		exit 0
 	fi
 
+	# without this, flit won't build the sdist
 	git update-index --assume-unchanged pyproject.toml
 	git update-index --assume-unchanged CHANGELOG.md
 
 	flit build --format sdist --setup-py
 	flit build --format wheel --setup-py
 	check_build "$pkg"
```

### Comparing `katalytic-pkg-0.2.3/scripts/venv.sh` & `katalytic-pkg-0.2.4/scripts/venv.sh`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.2.3/src/katalytic/pkg.py` & `katalytic-pkg-0.2.4/src/katalytic/pkg.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,15 @@
     pkg2 = pkg.replace('-', '.').replace('_', '.')
     prefix = '[^/]+'.join(pkg2.split('.'))
 
     for p in sys.path:
         if not Path(p).is_dir():
             continue
 
-        for p2 in iglob(f'{p}**', recursive=True):
-
+        for p2 in iglob(f'{p}/**', recursive=True):
             if '__pycache__' in p2:
                 continue
 
             if re.search(f'{prefix}.*[.]dist-info', p2):
                 yield p2
                 if Path(f'{p2}/METADATA').is_file():
                     yield p2
```

### Comparing `katalytic-pkg-0.2.3/tests/test_pkg.py` & `katalytic-pkg-0.2.4/tests/test_pkg.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         found = get_functions_in_group('__test_2')
         found = [(name, groups) for name, _, groups in found]
         assert found == [
             ('__test', ['__test_2']),
             ('__test_2', ['__test_2'])
         ]
 
-@pytest.mark.skipif(sys.version_info < (3, 8), reason="In some cases it fails on python < 3.8")
 class Test_version:
     def test_is_ok(self):
         v, v_info = get_version('katalytic.pkg')
 
         assert pkg_version is not None
         assert v is not None
         assert v_info is not None
```

### Comparing `katalytic-pkg-0.2.3/PKG-INFO` & `katalytic-pkg-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-pkg
-Version: 0.2.3
+Version: 0.2.4
 Summary: This plugin provides some metaprogramming magic for the other katalytic plugins
 Keywords: high-level,metaprogramming
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

