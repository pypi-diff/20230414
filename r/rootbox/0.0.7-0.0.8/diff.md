# Comparing `tmp/rootbox-0.0.7.tar.gz` & `tmp/rootbox-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rootbox-0.0.7.tar", last modified: Thu Apr 13 18:01:59 2023, max compression
+gzip compressed data, was "rootbox-0.0.8.tar", last modified: Fri Apr 14 17:50:05 2023, max compression
```

## Comparing `rootbox-0.0.7.tar` & `rootbox-0.0.8.tar`

### file list

```diff
@@ -1,62 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.924170 rootbox-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.916169 rootbox-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.920169 rootbox-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-13 18:01:51.000000 rootbox-0.0.7/.github/workflows/multi-test.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-04-13 18:01:51.000000 rootbox-0.0.7/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-04-13 18:01:51.000000 rootbox-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-04-13 18:01:51.000000 rootbox-0.0.7/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.920169 rootbox-0.0.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-04-13 18:01:51.000000 rootbox-0.0.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-04-13 18:01:51.000000 rootbox-0.0.7/CREDITS.md
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-13 18:01:51.000000 rootbox-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-13 18:01:51.000000 rootbox-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-04-13 18:01:59.924170 rootbox-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-13 18:01:51.000000 rootbox-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.920169 rootbox-0.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-04-13 18:01:51.000000 rootbox-0.0.7/docs/LXC.md
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-04-13 18:01:51.000000 rootbox-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-04-13 18:01:51.000000 rootbox-0.0.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-13 18:01:51.000000 rootbox-0.0.7/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.920169 rootbox-0.0.7/rootbox/
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.924170 rootbox-0.0.7/rootbox/cli/
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/cli/cmd_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/cli/cmd_exec.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/cli/cmd_lxc.py
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/cli/cmd_pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/cli/cmd_run.py
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/colorhelper.py
--rw-r--r--   0 runner    (1001) docker     (122)      793 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/download.py
--rw-r--r--   0 runner    (1001) docker     (122)      985 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/enter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.924170 rootbox-0.0.7/rootbox/images/
--rw-r--r--   0 runner    (1001) docker     (122)     1103 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/images/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     4313 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/images/lxc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/images_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/mount.py
--rw-r--r--   0 runner    (1001) docker     (122)      258 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/path.py
--rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/process.py
--rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/rootfs.py
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/size.py
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/socket.py
--rw-r--r--   0 runner    (1001) docker     (122)      433 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/tar.py
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/unshare.py
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/verbose.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.924170 rootbox-0.0.7/rootbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.924170 rootbox-0.0.7/samples/
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-04-13 18:01:51.000000 rootbox-0.0.7/samples/test.py
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-04-13 18:01:59.924170 rootbox-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      714 2023-04-13 18:01:51.000000 rootbox-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.924170 rootbox-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      611 2023-04-13 18:01:51.000000 rootbox-0.0.7/tests/test_cmd_pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-04-13 18:01:51.000000 rootbox-0.0.7/tests/test_image_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-04-13 18:01:51.000000 rootbox-0.0.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.226235 rootbox-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.218235 rootbox-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-14 17:49:59.000000 rootbox-0.0.8/.github/workflows/multi-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-04-14 17:49:59.000000 rootbox-0.0.8/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-04-14 17:49:59.000000 rootbox-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-04-14 17:49:59.000000 rootbox-0.0.8/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-04-14 17:49:59.000000 rootbox-0.0.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (122)      449 2023-04-14 17:49:59.000000 rootbox-0.0.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-04-14 17:49:59.000000 rootbox-0.0.8/CREDITS.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-14 17:49:59.000000 rootbox-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-14 17:49:59.000000 rootbox-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-14 17:50:05.226235 rootbox-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-04-14 17:49:59.000000 rootbox-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-04-14 17:49:59.000000 rootbox-0.0.8/docs/LXC.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/docs/img/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    24714 2023-04-14 17:49:59.000000 rootbox-0.0.8/docs/img/rootbox_0.0.8.png
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-04-14 17:49:59.000000 rootbox-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-04-14 17:49:59.000000 rootbox-0.0.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-14 17:49:59.000000 rootbox-0.0.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/rootbox/
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/rootbox/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/cli/cmd_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/cli/cmd_exec.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/cli/cmd_lxc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/cli/cmd_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/cli/cmd_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/colorhelper.py
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)      985 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/enter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.226235 rootbox-0.0.8/rootbox/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     1103 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/images/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4315 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/images/lxc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/images_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/mount.py
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/process.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/rootfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/shell.py
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/size.py
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/socket.py
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/tar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1142 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/unshare.py
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-14 17:49:59.000000 rootbox-0.0.8/rootbox/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.222235 rootbox-0.0.8/rootbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-14 17:50:05.000000 rootbox-0.0.8/rootbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.226235 rootbox-0.0.8/samples/
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-14 17:49:59.000000 rootbox-0.0.8/samples/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-04-14 17:50:05.226235 rootbox-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      714 2023-04-14 17:49:59.000000 rootbox-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 17:50:05.226235 rootbox-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-04-14 17:49:59.000000 rootbox-0.0.8/tests/test_cmd_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-04-14 17:49:59.000000 rootbox-0.0.8/tests/test_image_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-04-14 17:49:59.000000 rootbox-0.0.8/tox.ini
```

### Comparing `rootbox-0.0.7/.github/workflows/multi-test.yaml` & `rootbox-0.0.8/.github/workflows/multi-test.yaml`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/.github/workflows/release.yaml` & `rootbox-0.0.8/.github/workflows/release.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -26,17 +26,18 @@
 
       - name: Publish distribution 📦 to PyPI
         if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@master
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
 
-  # https://github.com/marketplace/actions/create-release
+  # https://github.com/softprops/action-gh-release
   create-release:
     runs-on: ubuntu-latest
     permissions:
       contents: write
     steps:
     - uses: actions/checkout@v3
-    - uses: ncipollo/release-action@v1
+    - name: Release
+      uses: softprops/action-gh-release@v1
       with:
-        generateReleaseNotes: true
+        body_path: ${{ github.workspace }}/CHANGELOG.md
```

### Comparing `rootbox-0.0.7/.gitignore` & `rootbox-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/.pre-commit-config.yaml` & `rootbox-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/LICENSE` & `rootbox-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/PKG-INFO` & `rootbox-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rootbox
-Version: 0.0.7
+Version: 0.0.8
 Summary: Portable reproducible environments for Linux applications
 Home-page: https://github.com/joaompinto/rootbox
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,14 +15,17 @@
 ![License](https://img.shields.io/github/license/joaompinto/rootbox?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 ## What is rootbox?
 
 Rootbox is a tool for Linux and WSL that allows regular (unprivileged) users to deploy applications in a portable and reproducible way.
 
+![Rootbox in action](docs/img/rootbox_0.0.8.png)
+
+
 ## How does it work
 Rootbox uses Linux kernel namespaces to create contained environments.
 
 ## What is the difference between rootbox and Docker?
 The focus of rootbox is to provide a tool that can be used to run applications without the need to install dependencies on the host system. Rootbox does **NOT** aim to provide full isolation between environemtns and the host, for such use cases please consider using Docker or Podman.
 
 ## What is nedded to run rootbox?
```

### Comparing `rootbox-0.0.7/README.md` & `rootbox-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 ![License](https://img.shields.io/github/license/joaompinto/rootbox?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 ## What is rootbox?
 
 Rootbox is a tool for Linux and WSL that allows regular (unprivileged) users to deploy applications in a portable and reproducible way.
 
+![Rootbox in action](docs/img/rootbox_0.0.8.png)
+
+
 ## How does it work
 Rootbox uses Linux kernel namespaces to create contained environments.
 
 ## What is the difference between rootbox and Docker?
 The focus of rootbox is to provide a tool that can be used to run applications without the need to install dependencies on the host system. Rootbox does **NOT** aim to provide full isolation between environemtns and the host, for such use cases please consider using Docker or Podman.
 
 ## What is nedded to run rootbox?
```

### Comparing `rootbox-0.0.7/docs/LXC.md` & `rootbox-0.0.8/docs/LXC.md`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/__main__.py` & `rootbox-0.0.8/rootbox/__main__.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/cli/cmd_create.py` & `rootbox-0.0.8/rootbox/cli/cmd_create.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/cli/cmd_pull.py` & `rootbox-0.0.8/rootbox/cli/cmd_pull.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/cli/cmd_run.py` & `rootbox-0.0.8/rootbox/cli/cmd_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """  Create a new environment  """
-import os
 from typing import Optional
 
 import typer
 
 from ..download import download_image
 from ..images import parse_image_url
 from ..rootfs import prepare_rootfs
+from ..shell import raw_execute, shell_execute
 from ..unshare import CLONE_NEWNET, unshare
 
 
 def run(
     image_name: str = typer.Argument(...),
-    no_shell: bool = typer.Option(False, "--no-sh"),
+    no_shell: bool = typer.Option(False, "--no-sh", "--no-shell"),
     no_net: bool = typer.Option(
         False, "--no-network", "-N", help="Disable network in the container"
     ),
-    command: Optional[str] = typer.Argument("/bin/sh", help="Command to be run"),
+    command: Optional[str] = typer.Argument(None, help="Command to be run"),
     only_from_cache: bool = typer.Option(False, "--only-from-cache"),
 ):
+    if no_shell and command == "/bin/sh":
+        raise typer.BadParameter("--no-shell was provided but no command was given")
+
     image = parse_image_url(image_name)
     image_fname = download_image(image, only_from_cache=only_from_cache)
-    prepare_rootfs(image_fname, in_memory=True, perform_chroot=True)
+    mount_dir = prepare_rootfs(image_fname, in_memory=True, perform_chroot=True)
     if no_net:
         unshare(CLONE_NEWNET)
     if no_shell:
-        command = command.split()
-        os.execvp(command[0], command[:])
+        raw_execute(image_name, mount_dir, command)
     else:
-        os.execvp("/bin/sh", ["sh", "-c", command])
+        shell_execute(image_name, mount_dir, command)
```

### Comparing `rootbox-0.0.7/rootbox/colorhelper.py` & `rootbox-0.0.8/rootbox/colorhelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def print_warn(message):
     return cprint(message, "yellow", attrs=["bold"], file=sys.stderr)
 
 
 def info(message):
-    return colored(message, "cyan")
+    return colored(message, "cyan", attrs=["bold"])
 
 
 def info_header(message):
     return colored(message, "cyan", attrs=["bold"])
 
 
 def warning(message):
```

### Comparing `rootbox-0.0.7/rootbox/download.py` & `rootbox-0.0.8/rootbox/download.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/enter.py` & `rootbox-0.0.8/rootbox/enter.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/http.py` & `rootbox-0.0.8/rootbox/http.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/images/__init__.py` & `rootbox-0.0.8/rootbox/images/__init__.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/images/docker.py` & `rootbox-0.0.8/rootbox/images/docker.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/images/lxc.py` & `rootbox-0.0.8/rootbox/images/lxc.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             f"lxc_{self.name}_{self.version}_{self.arch}_{self.variant}_{self.build or ''}"
         )
 
     def download(self):
         return download_url(get_lcx_distro_url(self))
 
 
-class NotSingleVersonError(Exception):
+class NotSingleVersionError(Exception):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
 class LCXMetaData:
     def __init__(self):
         verbose(f"Fetching LXC metadata from {LCX_INDEX}")
@@ -94,15 +94,15 @@
             image_name, distro_version, distro_arch, distro_variant
         )
         if len(matching_versions) == 0:
             raise ValueError(
                 f"No image found matching {image_name} {distro_version} {distro_arch} {distro_variant}"
             )
         if len(matching_versions) > 1:
-            raise NotSingleVersonError(
+            raise NotSingleVersionError(
                 f"Found multiple versions for {image_name} {distro_version} {distro_arch}",
                 matching_versions,
             )
         matching_version = matching_versions[0]
         matchin_builds = self.builds(
             image_name, matching_version, distro_arch, distro_variant, distro_build
         )
```

### Comparing `rootbox-0.0.7/rootbox/images_cache.py` & `rootbox-0.0.8/rootbox/images_cache.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/mount.py` & `rootbox-0.0.8/rootbox/mount.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/process.py` & `rootbox-0.0.8/rootbox/process.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/rootfs.py` & `rootbox-0.0.8/rootbox/rootfs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import os
 from pathlib import Path
 from tempfile import mkdtemp
 
 from .mount import MS_BIND, MS_PRIVATE, MS_REC, mount
 from .path import path_is_parent
 from .tar import extract_tar
-from .unshare import set_user_level_root
+from .unshare import setup_user_level_root
 
 STD_MOUNTS = [
     ("/proc", "proc/", None, MS_BIND | MS_REC),
     ("/dev", "dev/", None, MS_BIND | MS_REC),
     ("/sys", "sys/", None, MS_BIND | MS_REC),
     ("tmpfs", "run/", "tmpfs"),
 ]
 
 
-def prepare_rootfs(rootfs_filename: Path, in_memory, perform_chroot=True) -> Path:
-    set_user_level_root()
+def prepare_rootfs(
+    rootfs_filename: Path, in_memory: bool = True, perform_chroot=True
+) -> Path:
+    """Preate a new root mount directory"""
+    setup_user_level_root()
     current_path = os.getcwd()
     restore_path = None
     if path_is_parent(os.path.expanduser("~"), current_path):
         restore_path = current_path
 
     mount(None, "/", None, MS_REC | MS_PRIVATE)
     mount_dir = Path(mkdtemp())
     if in_memory:
-        mount("tmpfs", mount_dir, "tmpfs")
+        mount("tmpfs", mount_dir, "tmpfs", options="size=1G")
     if ".tar" in rootfs_filename.suffixes:
         extract_tar(rootfs_filename, mount_dir)
     else:
         raise NotImplementedError(f"Unsupported rootfs format: {rootfs_filename}")
     os.chdir(mount_dir)
     for mount_args in STD_MOUNTS:
         os.makedirs(mount_args[1], exist_ok=True)
```

### Comparing `rootbox-0.0.7/rootbox/size.py` & `rootbox-0.0.8/rootbox/size.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/socket.py` & `rootbox-0.0.8/rootbox/socket.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/rootbox/unshare.py` & `rootbox-0.0.8/rootbox/unshare.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,12 +35,12 @@
     Path("/proc/self/uid_map").write_text(f"0 {uid} 1")
     Path("/proc/self/setgroups").write_text("deny")
     Path("/proc/self/gid_map").write_text(f"0 {gid} 1")
     # wait for the uid/gid mapping to take effect
     time.sleep(0.1)
 
 
-def set_user_level_root():
+def setup_user_level_root():
     uid, gid = os.geteuid(), os.getegid()
     verbose("Creating user and mount namespaces")
     unshare(CLONE_NEWNS | CLONE_NEWUSER)
     rewrite_uid_map(uid, gid)
```

### Comparing `rootbox-0.0.7/rootbox.egg-info/PKG-INFO` & `rootbox-0.0.8/rootbox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rootbox
-Version: 0.0.7
+Version: 0.0.8
 Summary: Portable reproducible environments for Linux applications
 Home-page: https://github.com/joaompinto/rootbox
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,14 +15,17 @@
 ![License](https://img.shields.io/github/license/joaompinto/rootbox?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 ## What is rootbox?
 
 Rootbox is a tool for Linux and WSL that allows regular (unprivileged) users to deploy applications in a portable and reproducible way.
 
+![Rootbox in action](docs/img/rootbox_0.0.8.png)
+
+
 ## How does it work
 Rootbox uses Linux kernel namespaces to create contained environments.
 
 ## What is the difference between rootbox and Docker?
 The focus of rootbox is to provide a tool that can be used to run applications without the need to install dependencies on the host system. Rootbox does **NOT** aim to provide full isolation between environemtns and the host, for such use cases please consider using Docker or Podman.
 
 ## What is nedded to run rootbox?
```

### Comparing `rootbox-0.0.7/rootbox.egg-info/SOURCES.txt` & `rootbox-0.0.8/rootbox.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 .gitignore
 .pre-commit-config.yaml
+CHANGELOG.md
 CREDITS.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/multi-test.yaml
 .github/workflows/release.yaml
 .vscode/settings.json
 docs/LXC.md
+docs/img/rootbox_0.0.8.png
 rootbox/__main__.py
 rootbox/colorhelper.py
 rootbox/download.py
 rootbox/enter.py
 rootbox/http.py
 rootbox/images_cache.py
 rootbox/mount.py
 rootbox/path.py
 rootbox/process.py
 rootbox/rootfs.py
+rootbox/shell.py
 rootbox/size.py
 rootbox/socket.py
 rootbox/tar.py
 rootbox/unshare.py
 rootbox/verbose.py
 rootbox/version.py
 rootbox.egg-info/PKG-INFO
```

### Comparing `rootbox-0.0.7/samples/test.py` & `rootbox-0.0.8/samples/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from rootbox.mount import MS_BIND, MS_PRIVATE, MS_REC, mount
-from rootbox.unshare import set_user_level_root
+from rootbox.unshare import setup_user_level_root
 
-set_user_level_root()
+setup_user_level_root()
 
 # remount / as private to make subsequent mounts visible only to the current process and its descendants.
 mount(None, "/", None, MS_REC | MS_PRIVATE)
 
 os.chdir("/tmp/alpine")
 mount("/proc", "proc/", None, MS_BIND | MS_REC)
 mount("/dev", "dev/", None, MS_BIND | MS_REC)
```

### Comparing `rootbox-0.0.7/setup.py` & `rootbox-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.7/tests/test_cmd_pull.py` & `rootbox-0.0.8/tests/test_cmd_pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typer.testing import CliRunner
 
 from rootbox.__main__ import app
-from rootbox.images.lxc import NotSingleVersonError
+from rootbox.images.lxc import NotSingleVersionError
 
 runner = CliRunner()
 
 
 def test_pull_remote():
     result = runner.invoke(app, ["pull", "bananas"])
     assert "Only remote images are supported" in result.stdout
     assert result.exit_code == 2
 
     result = runner.invoke(app, ["pull", "bananas:"])
     assert "Unknown image handler" in result.stdout
     assert result.exit_code == 2
 
     result = runner.invoke(app, ["pull", "lxc:alpine"])
-    assert isinstance(result.exception, NotSingleVersonError)
+    assert isinstance(result.exception, NotSingleVersionError)
     assert result.exit_code == 1
```

### Comparing `rootbox-0.0.7/tests/test_image_url.py` & `rootbox-0.0.8/tests/test_image_url.py`

 * *Files identical despite different names*

