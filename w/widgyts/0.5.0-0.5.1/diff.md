# Comparing `tmp/widgyts-0.5.0.tar.gz` & `tmp/widgyts-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widgyts-0.5.0.tar", last modified: Wed Apr 12 16:28:34 2023, max compression
+gzip compressed data, was "widgyts-0.5.1.tar", last modified: Fri Apr 14 15:26:17 2023, max compression
```

## Comparing `widgyts-0.5.0.tar` & `widgyts-0.5.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.955372 widgyts-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 16:27:17.000000 widgyts-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-12 16:27:17.000000 widgyts-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-12 16:28:34.955372 widgyts-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-12 16:27:17.000000 widgyts-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 16:27:17.000000 widgyts-0.5.0/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.947372 widgyts-0.5.0/jupyter-config/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 16:27:17.000000 widgyts-0.5.0/jupyter-config/widgyts.json
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-12 16:27:17.000000 widgyts-0.5.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-12 16:27:17.000000 widgyts-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-12 16:28:34.955372 widgyts-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-12 16:27:17.000000 widgyts-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/src/@types/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/@types/jupyter-threejs.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/colormap_container.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/fixed_res_buffer.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/fullscreen.ts
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/plugin.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/utils.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/variable_mesh.ts
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/widgyts.ts
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-04-12 16:27:17.000000 widgyts-0.5.0/src/widgyts_canvas.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:27:17.000000 widgyts-0.5.0/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 16:27:17.000000 widgyts-0.5.0/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 16:27:17.000000 widgyts-0.5.0/style/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-12 16:27:17.000000 widgyts-0.5.0/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/widgyts/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    28666 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/dataset_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/image_canvas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/widgyts/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/widgyts/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)    67838 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/353.b96de7a6ab53ee83a3e3.js
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/353.b96de7a6ab53ee83a3e3.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   109061 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/35962d9a369f94cd12dc.module.wasm
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/480.f221211101f033161e08.js
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/568.dc67e4d4b7ec920ad835.js
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/7.578ca98bdcc06909a72d.js
--rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/724.68ad0e0a95918b09cc71.js
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/776.034dd82e5586eada2301.js
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/818.070644e61f231f18d729.js
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/remoteEntry.59b399c5575c4621e134.js
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 16:28:31.000000 widgyts-0.5.0/widgyts/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.955372 widgyts-0.5.0/widgyts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-12 16:27:17.000000 widgyts-0.5.0/widgyts/tests/test_widgyts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:28:34.951372 widgyts-0.5.0/widgyts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:27:44.000000 widgyts-0.5.0/widgyts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 16:28:34.000000 widgyts-0.5.0/widgyts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)   411000 2023-04-12 16:28:24.000000 widgyts-0.5.0/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:17.073726 widgyts-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-14 15:24:59.000000 widgyts-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-14 15:24:59.000000 widgyts-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-14 15:26:17.073726 widgyts-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-14 15:24:59.000000 widgyts-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-14 15:24:59.000000 widgyts-0.5.1/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:17.069726 widgyts-0.5.1/jupyter-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-14 15:24:59.000000 widgyts-0.5.1/jupyter-config/widgyts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-14 15:24:59.000000 widgyts-0.5.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-14 15:24:59.000000 widgyts-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-14 15:26:17.073726 widgyts-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-14 15:24:59.000000 widgyts-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:17.069726 widgyts-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:17.069726 widgyts-0.5.1/src/@types/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-14 15:24:59.000000 widgyts-0.5.1/src/@types/jupyter-threejs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-14 15:24:59.000000 widgyts-0.5.1/src/colormap_container.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-14 15:24:59.000000 widgyts-0.5.1/src/fixed_res_buffer.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-14 15:24:59.000000 widgyts-0.5.1/src/fullscreen.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 15:24:59.000000 widgyts-0.5.1/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-14 15:24:59.000000 widgyts-0.5.1/src/plugin.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-14 15:24:59.000000 widgyts-0.5.1/src/utils.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-14 15:24:59.000000 widgyts-0.5.1/src/variable_mesh.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-14 15:24:59.000000 widgyts-0.5.1/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 15:24:59.000000 widgyts-0.5.1/src/widgyts.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-04-14 15:24:59.000000 widgyts-0.5.1/src/widgyts_canvas.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:17.069726 widgyts-0.5.1/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:24:59.000000 widgyts-0.5.1/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 15:24:59.000000 widgyts-0.5.1/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 15:24:59.000000 widgyts-0.5.1/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-14 15:24:59.000000 widgyts-0.5.1/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:17.069726 widgyts-0.5.1/widgyts/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-14 15:24:59.000000 widgyts-0.5.1/widgyts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-14 15:24:59.000000 widgyts-0.5.1/widgyts/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-14 15:24:59.000000 widgyts-0.5.1/widgyts/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28980 2023-04-14 15:24:59.000000 widgyts-0.5.1/widgyts/dataset_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-14 15:24:59.000000 widgyts-0.5.1/widgyts/image_canvas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:17.069726 widgyts-0.5.1/widgyts/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-14 15:26:16.000000 widgyts-0.5.1/widgyts/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:17.073726 widgyts-0.5.1/widgyts/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    67838 2023-04-14 15:26:16.000000 widgyts-0.5.1/widgyts/labextension/static/353.b96de7a6ab53ee83a3e3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 15:26:16.000000 widgyts-0.5.1/widgyts/labextension/static/353.b96de7a6ab53ee83a3e3.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   109061 2023-04-14 15:26:16.000000 widgyts-0.5.1/widgyts/labextension/static/35962d9a369f94cd12dc.module.wasm
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-14 15:26:16.000000 widgyts-0.5.1/widgyts/labextension/static/480.f221211101f033161e08.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-14 15:26:16.000000 widgyts-0.5.1/widgyts/labextension/static/568.dc67e4d4b7ec920ad835.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-14 15:26:16.000000 widgyts-0.5.1/widgyts/labextension/static/7.578ca98bdcc06909a72d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-04-14 15:26:16.000000 widgyts-0.5.1/widgyts/labextension/static/724.1d0ec7e99e0045b1da9c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-14 15:26:16.000000 widgyts-0.5.1/widgyts/labextension/static/776.034dd82e5586eada2301.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-14 15:26:16.000000 widgyts-0.5.1/widgyts/labextension/static/818.070644e61f231f18d729.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-04-14 15:26:16.000000 widgyts-0.5.1/widgyts/labextension/static/remoteEntry.5d4e0ace3da9f461d3dc.js
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-14 15:26:13.000000 widgyts-0.5.1/widgyts/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-04-14 15:26:16.000000 widgyts-0.5.1/widgyts/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:17.073726 widgyts-0.5.1/widgyts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:24:59.000000 widgyts-0.5.1/widgyts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-14 15:24:59.000000 widgyts-0.5.1/widgyts/tests/test_widgyts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:17.069726 widgyts-0.5.1/widgyts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-14 15:26:17.000000 widgyts-0.5.1/widgyts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-14 15:26:17.000000 widgyts-0.5.1/widgyts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:26:17.000000 widgyts-0.5.1/widgyts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:25:26.000000 widgyts-0.5.1/widgyts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 15:26:17.000000 widgyts-0.5.1/widgyts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 15:26:17.000000 widgyts-0.5.1/widgyts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   411000 2023-04-14 15:26:07.000000 widgyts-0.5.1/yarn.lock
```

### Comparing `widgyts-0.5.0/LICENSE` & `widgyts-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/PKG-INFO` & `widgyts-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgyts
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Custom Jupyter Widget Library for Interactive Visualization with yt
 Home-page: https://github.com/yt-project/widgyts
 Author: The yt Project
 Author-email: yt-dev@python.org
 License: BSD-3-Clause
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://widgyts.readthedocs.org/
@@ -84,15 +84,15 @@
 recent enough version of Jupyterlab, preferably 0.35 or above.  For a
 development installation, do:
 
     $ jupyter labextension install js
 
 To install the latest released version,
 
-    $ jupyter labextension install @data-exp-lab/yt-widgets
+    $ jupyter labextension install @yt-project/yt-widgets
 
 Using
 -----
 
 To use this, you will need to have yt installed.  Importing it monkeypatches
 the Slice and Projection objects, so you are now able to do:
```

### Comparing `widgyts-0.5.0/README.md` & `widgyts-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 recent enough version of Jupyterlab, preferably 0.35 or above.  For a
 development installation, do:
 
     $ jupyter labextension install js
 
 To install the latest released version,
 
-    $ jupyter labextension install @data-exp-lab/yt-widgets
+    $ jupyter labextension install @yt-project/yt-widgets
 
 Using
 -----
 
 To use this, you will need to have yt installed.  Importing it monkeypatches
 the Slice and Projection objects, so you are now able to do:
```

### Comparing `widgyts-0.5.0/package.json` & `widgyts-0.5.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.5.1'"}*

```diff
@@ -130,9 +130,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.5.0"
+    "version": "0.5.1"
 }
```

### Comparing `widgyts-0.5.0/pyproject.toml` & `widgyts-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/setup.cfg` & `widgyts-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = widgyts
-version = 0.5.0
+version = 0.5.1
 description = A Custom Jupyter Widget Library for Interactive Visualization with yt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yt-project/widgyts
 author = Data Exploration Lab
 license = BSD-3-Clause
 license_file = LICENSE
```

### Comparing `widgyts-0.5.0/setup.py` & `widgyts-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/src/colormap_container.ts` & `widgyts-0.5.1/src/colormap_container.ts`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/src/fixed_res_buffer.ts` & `widgyts-0.5.1/src/fixed_res_buffer.ts`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/src/fullscreen.ts` & `widgyts-0.5.1/src/fullscreen.ts`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/src/plugin.ts` & `widgyts-0.5.1/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/src/utils.ts` & `widgyts-0.5.1/src/utils.ts`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/src/variable_mesh.ts` & `widgyts-0.5.1/src/variable_mesh.ts`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/src/widgyts_canvas.ts` & `widgyts-0.5.1/src/widgyts_canvas.ts`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/tsconfig.json` & `widgyts-0.5.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/widgyts/__init__.py` & `widgyts-0.5.1/widgyts/__init__.py`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/widgyts/colormaps.py` & `widgyts-0.5.1/widgyts/colormaps.py`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/widgyts/dataset_viewer.py` & `widgyts-0.5.1/widgyts/dataset_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,21 +88,21 @@
             new_children.extend(c.view)
         self.renderer.scene.children = self.renderer.scene.children[:2] + tuple(
             new_children
         )
 
     @traitlets.default("renderer")
     def _renderer_default(self):
-        center = tuple(self.ds.domain_center.in_units("code_length").d)
+        center = tuple(self.ds.domain_center.in_units("unitary").d)
         right = tuple(
             (
                 self.ds.domain_right_edge
                 + (self.ds.domain_right_edge - self.ds.domain_center) * 2.0
             )
-            .in_units("code_length")
+            .in_units("unitary")
             .d
         )
         camera = pythreejs.PerspectiveCamera(
             position=right,
             fov=20,
             children=[pythreejs.AmbientLight()],
             near=1e-2,
@@ -229,23 +229,22 @@
         select = ipywidgets.Select(options=[], disabled=False)
 
         def on_selection_changed(change):
             self.parent.renderer.camera.set_state(change["new"])
 
         select.observe(on_selection_changed, ["value"])
 
-        center = self.parent.ds.domain_center.in_units("code_length").d
+        center = self.parent.ds.domain_center.in_units("unitary").d
 
         def _create_clicked(axi, ax):
             def view_button_clicked(button):
                 vec = [0, 0, 0]
                 vec[axi] = 2.0
                 self.parent.renderer.camera.position = tuple(
-                    center
-                    + (self.parent.ds.domain_width.in_units("code_length").d * vec)
+                    center + (self.parent.ds.domain_width.in_units("unitary").d * vec)
                 )
                 self.parent.renderer.camera.lookAt(center)
 
             return view_button_clicked
 
         view_buttons = []
         for axi, ax in enumerate("XYZ"):
@@ -257,15 +256,15 @@
 
             view_buttons[-1].on_click(_create_clicked(axi, ax))
 
         # This could probably be stuck into the _create_clicked function, but my
         # first attempt didn't work, so I'm writing it out here.
         def view_isometric(button):
             self.parent.renderer.camera.position = tuple(
-                center + (self.parent.ds.domain_width.in_units("code_length").d * 2)
+                center + (self.parent.ds.domain_width.in_units("unitary").d * 2)
             )
             self.parent.renderer.camera.lookAt(center)
 
         view_buttons.append(
             ipywidgets.Button(
                 description="◆",
             )
@@ -318,23 +317,23 @@
     display_name = "Axes"
     domain_axes = traitlets.Instance(pythreejs.AxesHelper)
 
     @traitlets.default("domain_axes")
     def _domain_axes_default(self):
         offset_vector = (
             self.parent.ds.domain_left_edge - self.parent.ds.domain_center
-        ) * 0.1
+        ).in_units("unitary") * 0.1
         position = tuple(
-            (self.parent.ds.domain_left_edge + offset_vector).in_units("code_length").d
+            (self.parent.ds.domain_left_edge + offset_vector).in_units("unitary").d
         )
         # We probably don't want to use the AxesHelper as it doesn't expose the
         # material, which can result in it not being easy to see.  But for now...
         ah = pythreejs.AxesHelper(
             position=position,
-            scale=tuple(self.parent.ds.domain_width.in_units("code_length").d),
+            scale=tuple(self.parent.ds.domain_width.in_units("unitary").d),
         )
         return ah
 
     @property
     def view(self):
         return [self.domain_axes]
 
@@ -453,17 +452,22 @@
             # We truncate at half of the colormap so that we just get a slight
             # linear progression
             color = mcolors.to_hex(
                 cmap(self.cmap_truncate * level / self.parent.ds.max_level)
             )
             # Corners is shaped like 8, 3, NGrids
             this_level = self.parent.ds.index.grid_levels[:, 0] == level
-            corners = np.rollaxis(
-                self.parent.ds.index.grid_corners[:, :, this_level], 2
-            ).astype("float32")
+            level_corners = self.parent.ds.index.grid_corners[:, :, this_level]
+            # We don't know if level_corners will be unyt-ful or not, but if it *is*
+            # it will be in the units of the grid_left_edges
+            uq = self.parent.ds.index.grid_left_edge.uq
+            level_corners = (getattr(level_corners, "d", level_corners) * uq).in_units(
+                "unitary"
+            )
+            corners = np.rollaxis(level_corners, 2).astype("float32")
             indices = (
                 ((np.arange(corners.shape[0]) * 8)[:, None] + _CORNER_INDICES[None, :])
                 .ravel()
                 .astype("uint32")
             )
             corners.shape = (corners.size // 3, 3)
             geometry = pythreejs.BufferGeometry(
```

### Comparing `widgyts-0.5.0/widgyts/image_canvas.py` & `widgyts-0.5.1/widgyts/image_canvas.py`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/widgyts/labextension/package.json` & `widgyts-0.5.1/widgyts/labextension/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9746527777777778%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.5d4e0ace3da9f461d3dc.js'}}",*

 * * "'version'": "'0.5.1'"}*

```diff
@@ -76,15 +76,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf,wasm}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/yt-project/widgyts",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.59b399c5575c4621e134.js",
+            "load": "static/remoteEntry.5d4e0ace3da9f461d3dc.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "widgyts"
                 },
@@ -135,9 +135,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.5.0"
+    "version": "0.5.1"
 }
```

### Comparing `widgyts-0.5.0/widgyts/labextension/static/353.b96de7a6ab53ee83a3e3.js` & `widgyts-0.5.1/widgyts/labextension/static/353.b96de7a6ab53ee83a3e3.js`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/widgyts/labextension/static/35962d9a369f94cd12dc.module.wasm` & `widgyts-0.5.1/widgyts/labextension/static/35962d9a369f94cd12dc.module.wasm`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/widgyts/labextension/static/480.f221211101f033161e08.js` & `widgyts-0.5.1/widgyts/labextension/static/480.f221211101f033161e08.js`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/widgyts/labextension/static/568.dc67e4d4b7ec920ad835.js` & `widgyts-0.5.1/widgyts/labextension/static/568.dc67e4d4b7ec920ad835.js`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/widgyts/labextension/static/7.578ca98bdcc06909a72d.js` & `widgyts-0.5.1/widgyts/labextension/static/7.578ca98bdcc06909a72d.js`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/widgyts/labextension/static/724.68ad0e0a95918b09cc71.js` & `widgyts-0.5.1/widgyts/labextension/static/724.1d0ec7e99e0045b1da9c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -401,11 +401,11 @@
                     const e = this.model.frb_model.get("width"),
                         t = this.model.frb_model.get("height");
                     this.image_bitmap = await createImageBitmap(this.image_data, 0, 0, e, t), this.model.set("_dirty_bitmap", !1)
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"name":"@yt-project/yt-widgets","version":"0.5.0","description":"A Custom Jupyter Widget Library for Interactive Visualization with yt","author":{"name":"The yt Project","email":"yt-dev@python.org"},"contributors":[{"name":"Nathanael Claussen","email":"nclauss2@illinois.edu"},{"name":"Madicken Munk","email":"madicken.munk@gmail.com"},{"name":"Matthew Turk","email":"matthewturk@gmail.com"}],"keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/yt-project/widgyts","bugs":{"url":"https://github.com/yt-project/widgyts/issues"},"license":"BSD-3-Clause","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf,wasm}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/yt-project/widgyts.git"},"scripts":{"build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf jupyterlab_nodeeditor/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jlpm run build","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@data-exp-lab/yt-tools":"^0.4.1","@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4","@jupyterlab/application":"^3.0.4","@jupyterlab/coreutils":"^5.0.2","@jupyterlab/mainmenu":"^3.0.3","@jupyterlab/services":"^6.0.3","@types/fscreen":"^1.0.1","@types/node":"^10.11.6","@types/three":"^0.141.0","fscreen":"^1.2.0","ipycanvas":"^0.8.2","jupyter-threejs":"^2.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@phosphor/application":"^1.6.0","@phosphor/widgets":"^1.6.0","@types/expect.js":"^0.3.29","@types/mocha":"^5.2.5","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","expect.js":"^0.3.1","fs-extra":"^7.0.0","karma":"^3.1.0","karma-chrome-launcher":"^2.2.0","karma-firefox-launcher":"^1.1.0","karma-ie-launcher":"^1.0.0","karma-mocha":"^1.3.0","karma-mocha-reporter":"^2.2.5","karma-typescript":"^5.0.3","karma-typescript-es6-transform":"^5.0.3","mkdirp":"^0.5.1","mocha":"^5.2.0","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^1.0.0","ts-loader":"^5.2.1","typescript":"^4.1.3","webpack":"^4.20.2","webpack-cli":"^3.1.2"},"sideEffects":["style/*.css","style/index.js"],"jupyterlab":{"discovery":{"server":{"managers":["pip"],"base":{"name":"widgyts"}}},"extension":"lib/plugin","outputDir":"widgyts/labextension","webpackConfig":"./webpack.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"styleModule":"style/index.js"}')
+            e.exports = JSON.parse('{"name":"@yt-project/yt-widgets","version":"0.5.1","description":"A Custom Jupyter Widget Library for Interactive Visualization with yt","author":{"name":"The yt Project","email":"yt-dev@python.org"},"contributors":[{"name":"Nathanael Claussen","email":"nclauss2@illinois.edu"},{"name":"Madicken Munk","email":"madicken.munk@gmail.com"},{"name":"Matthew Turk","email":"matthewturk@gmail.com"}],"keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/yt-project/widgyts","bugs":{"url":"https://github.com/yt-project/widgyts/issues"},"license":"BSD-3-Clause","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf,wasm}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/yt-project/widgyts.git"},"scripts":{"build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf jupyterlab_nodeeditor/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jlpm run build","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@data-exp-lab/yt-tools":"^0.4.1","@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4","@jupyterlab/application":"^3.0.4","@jupyterlab/coreutils":"^5.0.2","@jupyterlab/mainmenu":"^3.0.3","@jupyterlab/services":"^6.0.3","@types/fscreen":"^1.0.1","@types/node":"^10.11.6","@types/three":"^0.141.0","fscreen":"^1.2.0","ipycanvas":"^0.8.2","jupyter-threejs":"^2.3.0"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@phosphor/application":"^1.6.0","@phosphor/widgets":"^1.6.0","@types/expect.js":"^0.3.29","@types/mocha":"^5.2.5","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","expect.js":"^0.3.1","fs-extra":"^7.0.0","karma":"^3.1.0","karma-chrome-launcher":"^2.2.0","karma-firefox-launcher":"^1.1.0","karma-ie-launcher":"^1.0.0","karma-mocha":"^1.3.0","karma-mocha-reporter":"^2.2.5","karma-typescript":"^5.0.3","karma-typescript-es6-transform":"^5.0.3","mkdirp":"^0.5.1","mocha":"^5.2.0","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^1.0.0","ts-loader":"^5.2.1","typescript":"^4.1.3","webpack":"^4.20.2","webpack-cli":"^3.1.2"},"sideEffects":["style/*.css","style/index.js"],"jupyterlab":{"discovery":{"server":{"managers":["pip"],"base":{"name":"widgyts"}}},"extension":"lib/plugin","outputDir":"widgyts/labextension","webpackConfig":"./webpack.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"styleModule":"style/index.js"}')
         }
     }
 ]);
```

### Comparing `widgyts-0.5.0/widgyts/labextension/static/776.034dd82e5586eada2301.js` & `widgyts-0.5.1/widgyts/labextension/static/776.034dd82e5586eada2301.js`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/widgyts/labextension/static/818.070644e61f231f18d729.js` & `widgyts-0.5.1/widgyts/labextension/static/818.070644e61f231f18d729.js`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/widgyts/labextension/static/remoteEntry.59b399c5575c4621e134.js` & `widgyts-0.5.1/widgyts/labextension/static/remoteEntry.5d4e0ace3da9f461d3dc.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, f, s, u, c, l, d, p, h, b, v, y, m, g, w, _, j, S, P = {
+    var e, r, t, n, a, o, i, f, s, u, c, l, d, p, h, b, v, y, m, g, w, _, j, S, P = {
             338: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(724), t.e(568)]).then((() => () => t(568))),
                         "./extension": () => Promise.all([t.e(724), t.e(480)]).then((() => () => t(480))),
                         "./style": () => t.e(776).then((() => () => t(776)))
                     },
-                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    o = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                o = t.S[n];
-                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                a = t.S[n];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => o,
-                    init: () => a
+                    get: () => a,
+                    init: () => o
                 })
             }
         },
         x = {};
 
     function E(e) {
         var r = x[e];
@@ -34,158 +34,158 @@
             id: e,
             exports: {}
         };
         return P[e].call(t.exports, t, t.exports, E), t.exports
     }
     E.m = P, E.c = x, e = "function" == typeof Symbol ? Symbol("webpack queues") : "__webpack_queues__", r = "function" == typeof Symbol ? Symbol("webpack exports") : "__webpack_exports__", t = "function" == typeof Symbol ? Symbol("webpack error") : "__webpack_error__", n = e => {
         e && !e.d && (e.d = 1, e.forEach((e => e.r--)), e.forEach((e => e.r-- ? e.r++ : e())))
-    }, E.a = (o, a, i) => {
+    }, E.a = (a, o, i) => {
         var f;
         i && ((f = []).d = 1);
         var s, u, c, l = new Set,
-            d = o.exports,
+            d = a.exports,
             p = new Promise(((e, r) => {
                 c = r, u = e
             }));
-        p[r] = d, p[e] = e => (f && e(f), l.forEach(e), p.catch((e => {}))), o.exports = p, a((o => {
-            var a;
-            s = (o => o.map((o => {
-                if (null !== o && "object" == typeof o) {
-                    if (o[e]) return o;
-                    if (o.then) {
-                        var a = [];
-                        a.d = 0, o.then((e => {
-                            i[r] = e, n(a)
+        p[r] = d, p[e] = e => (f && e(f), l.forEach(e), p.catch((e => {}))), a.exports = p, o((a => {
+            var o;
+            s = (a => a.map((a => {
+                if (null !== a && "object" == typeof a) {
+                    if (a[e]) return a;
+                    if (a.then) {
+                        var o = [];
+                        o.d = 0, a.then((e => {
+                            i[r] = e, n(o)
                         }), (e => {
-                            i[t] = e, n(a)
+                            i[t] = e, n(o)
                         }));
                         var i = {};
-                        return i[e] = e => e(a), i
+                        return i[e] = e => e(o), i
                     }
                 }
                 var f = {};
-                return f[e] = e => {}, f[r] = o, f
-            })))(o);
+                return f[e] = e => {}, f[r] = a, f
+            })))(a);
             var i = () => s.map((e => {
                     if (e[t]) throw e[t];
                     return e[r]
                 })),
                 u = new Promise((r => {
-                    (a = () => r(i)).r = 0;
-                    var t = e => e !== f && !l.has(e) && (l.add(e), e && !e.d && (a.r++, e.push(a)));
+                    (o = () => r(i)).r = 0;
+                    var t = e => e !== f && !l.has(e) && (l.add(e), e && !e.d && (o.r++, e.push(o)));
                     s.map((r => r[e](t)))
                 }));
-            return a.r ? u : i()
+            return o.r ? u : i()
         }), (e => (e ? c(p[t] = e) : u(d), n(f)))), f && (f.d = 0)
     }, E.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return E.d(r, {
             a: r
         }), r
-    }, a = Object.getPrototypeOf ? e => Object.getPrototypeOf(e) : e => e.__proto__, E.t = function(e, r) {
+    }, o = Object.getPrototypeOf ? e => Object.getPrototypeOf(e) : e => e.__proto__, E.t = function(e, r) {
         if (1 & r && (e = this(e)), 8 & r) return e;
         if ("object" == typeof e && e) {
             if (4 & r && e.__esModule) return e;
             if (16 & r && "function" == typeof e.then) return e
         }
         var t = Object.create(null);
         E.r(t);
         var n = {};
-        o = o || [null, a({}), a([]), a(a)];
+        a = a || [null, o({}), o([]), o(o)];
         for (var i = 2 & r && e;
-            "object" == typeof i && !~o.indexOf(i); i = a(i)) Object.getOwnPropertyNames(i).forEach((r => n[r] = () => e[r]));
+            "object" == typeof i && !~a.indexOf(i); i = o(i)) Object.getOwnPropertyNames(i).forEach((r => n[r] = () => e[r]));
         return n.default = () => e, E.d(t, n), t
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
         7: "578ca98bdcc06909a72d",
         353: "b96de7a6ab53ee83a3e3",
         480: "f221211101f033161e08",
         568: "dc67e4d4b7ec920ad835",
         648: "5c4efee2a858d0525b7d",
-        724: "68ad0e0a95918b09cc71",
+        724: "1d0ec7e99e0045b1da9c",
         776: "034dd82e5586eada2301",
         818: "070644e61f231f18d729"
     } [e] + ".js?v=" + {
         7: "578ca98bdcc06909a72d",
         353: "b96de7a6ab53ee83a3e3",
         480: "f221211101f033161e08",
         568: "dc67e4d4b7ec920ad835",
         648: "5c4efee2a858d0525b7d",
-        724: "68ad0e0a95918b09cc71",
+        724: "1d0ec7e99e0045b1da9c",
         776: "034dd82e5586eada2301",
         818: "070644e61f231f18d729"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), i = {}, f = "@yt-project/yt-widgets:", E.l = (e, r, t, n) => {
         if (i[e]) i[e].push(r);
         else {
-            var o, a;
+            var a, o;
             if (void 0 !== t)
                 for (var s = document.getElementsByTagName("script"), u = 0; u < s.length; u++) {
                     var c = s[u];
                     if (c.getAttribute("src") == e || c.getAttribute("data-webpack") == f + t) {
-                        o = c;
+                        a = c;
                         break
                     }
                 }
-            o || (a = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, E.nc && o.setAttribute("nonce", E.nc), o.setAttribute("data-webpack", f + t), o.src = e), i[e] = [r];
+            a || (o = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, E.nc && a.setAttribute("nonce", E.nc), a.setAttribute("data-webpack", f + t), a.src = e), i[e] = [r];
             var l = (r, t) => {
-                    o.onerror = o.onload = null, clearTimeout(d);
+                    a.onerror = a.onload = null, clearTimeout(d);
                     var n = i[e];
-                    if (delete i[e], o.parentNode && o.parentNode.removeChild(o), n && n.forEach((e => e(t))), r) return r(t)
+                    if (delete i[e], a.parentNode && a.parentNode.removeChild(a), n && n.forEach((e => e(t))), r) return r(t)
                 },
                 d = setTimeout(l.bind(null, void 0, {
                     type: "timeout",
-                    target: o
+                    target: a
                 }), 12e4);
-            o.onerror = l.bind(null, o.onerror), o.onload = l.bind(null, o.onload), a && document.head.appendChild(o)
+            a.onerror = l.bind(null, a.onerror), a.onload = l.bind(null, a.onload), o && document.head.appendChild(a)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         E.S = {};
         var e = {},
             r = {};
         E.I = (t, n) => {
             n || (n = []);
-            var o = r[t];
-            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
-                if (n.push(o), e[t]) return e[t];
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
+                if (n.push(a), e[t]) return e[t];
                 E.o(E.S, t) || (E.S[t] = {});
-                var a = E.S[t],
+                var o = E.S[t],
                     i = "@yt-project/yt-widgets",
                     f = (e, r, t, n) => {
-                        var o = a[e] = a[e] || {},
-                            f = o[r];
-                        (!f || !f.loaded && (!n != !f.eager ? n : i > f.from)) && (o[r] = {
+                        var a = o[e] = o[e] || {},
+                            f = a[r];
+                        (!f || !f.loaded && (!n != !f.eager ? n : i > f.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     s = [];
-                return "default" === t && (f("@data-exp-lab/yt-tools", "0.4.1", (() => E.e(818).then((() => () => E(818))))), f("@yt-project/yt-widgets", "0.5.0", (() => Promise.all([E.e(724), E.e(568)]).then((() => () => E(568))))), f("fscreen", "1.2.0", (() => E.e(7).then((() => () => E(7))))), f("ipycanvas", "0.8.2", (() => Promise.all([E.e(353), E.e(648)]).then((() => () => E(353)))))), e[t] = s.length ? Promise.all(s).then((() => e[t] = 1)) : 1
+                return "default" === t && (f("@data-exp-lab/yt-tools", "0.4.1", (() => E.e(818).then((() => () => E(818))))), f("@yt-project/yt-widgets", "0.5.1", (() => Promise.all([E.e(724), E.e(568)]).then((() => () => E(568))))), f("fscreen", "1.2.0", (() => E.e(7).then((() => () => E(7))))), f("ipycanvas", "0.8.2", (() => Promise.all([E.e(353), E.e(648)]).then((() => () => E(353)))))), e[t] = s.length ? Promise.all(s).then((() => e[t] = 1)) : 1
             }
         }
     })(), E.v = (e, r, t, n) => {
-        var o = fetch(E.p + "" + t + ".module.wasm");
-        return "function" == typeof WebAssembly.instantiateStreaming ? WebAssembly.instantiateStreaming(o, n).then((r => Object.assign(e, r.instance.exports))) : o.then((e => e.arrayBuffer())).then((e => WebAssembly.instantiate(e, n))).then((r => Object.assign(e, r.instance.exports)))
+        var a = fetch(E.p + "" + t + ".module.wasm");
+        return "function" == typeof WebAssembly.instantiateStreaming ? WebAssembly.instantiateStreaming(a, n).then((r => Object.assign(e, r.instance.exports))) : a.then((e => e.arrayBuffer())).then((e => WebAssembly.instantiate(e, n))).then((r => Object.assign(e, r.instance.exports)))
     }, (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             t.length && (e = t[t.length - 1].src)
@@ -198,95 +198,95 @@
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, u = (e, r) => {
         e = s(e), r = s(r);
         for (var t = 0;;) {
             if (t >= e.length) return t < r.length && "u" != (typeof r[t])[0];
             var n = e[t],
-                o = (typeof n)[0];
-            if (t >= r.length) return "u" == o;
-            var a = r[t],
-                i = (typeof a)[0];
-            if (o != i) return "o" == o && "n" == i || "s" == i || "u" == o;
-            if ("o" != o && "u" != o && n != a) return n < a;
+                a = (typeof n)[0];
+            if (t >= r.length) return "u" == a;
+            var o = r[t],
+                i = (typeof o)[0];
+            if (a != i) return "o" == a && "n" == i || "s" == i || "u" == a;
+            if ("o" != a && "u" != a && n != o) return n < o;
             t++
         }
     }, c = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(i = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, i);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(i = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, i);
             return t
         }
-        var a = [];
-        for (o = 1; o < e.length; o++) {
-            var i = e[o];
-            a.push(0 === i ? "not(" + f() + ")" : 1 === i ? "(" + f() + " || " + f() + ")" : 2 === i ? a.pop() + " " + a.pop() : c(i))
+        var o = [];
+        for (a = 1; a < e.length; a++) {
+            var i = e[a];
+            o.push(0 === i ? "not(" + f() + ")" : 1 === i ? "(" + f() + " || " + f() + ")" : 2 === i ? o.pop() + " " + o.pop() : c(i))
         }
         return f();
 
         function f() {
-            return a.pop().replace(/^\((.+)\)$/, "$1")
+            return o.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, l = (e, r) => {
         if (0 in e) {
             r = s(r);
             var t = e[0],
                 n = t < 0;
             n && (t = -t - 1);
-            for (var o = 0, a = 1, i = !0;; a++, o++) {
-                var f, u, c = a < e.length ? (typeof e[a])[0] : "";
-                if (o >= r.length || "o" == (u = (typeof(f = r[o]))[0])) return !i || ("u" == c ? a > t && !n : "" == c != n);
+            for (var a = 0, o = 1, i = !0;; o++, a++) {
+                var f, u, c = o < e.length ? (typeof e[o])[0] : "";
+                if (a >= r.length || "o" == (u = (typeof(f = r[a]))[0])) return !i || ("u" == c ? o > t && !n : "" == c != n);
                 if ("u" == u) {
                     if (!i || "u" != c) return !1
                 } else if (i)
                     if (c == u)
-                        if (a <= t) {
-                            if (f != e[a]) return !1
+                        if (o <= t) {
+                            if (f != e[o]) return !1
                         } else {
-                            if (n ? f > e[a] : f < e[a]) return !1;
-                            f != e[a] && (i = !1)
+                            if (n ? f > e[o] : f < e[o]) return !1;
+                            f != e[o] && (i = !1)
                         }
                 else if ("s" != c && "n" != c) {
-                    if (n || a <= t) return !1;
-                    i = !1, a--
+                    if (n || o <= t) return !1;
+                    i = !1, o--
                 } else {
-                    if (a <= t || u < c != n) return !1;
+                    if (o <= t || u < c != n) return !1;
                     i = !1
-                } else "s" != c && "n" != c && (i = !1, a--)
+                } else "s" != c && "n" != c && (i = !1, o--)
             }
         }
         var d = [],
             p = d.pop.bind(d);
-        for (o = 1; o < e.length; o++) {
-            var h = e[o];
+        for (a = 1; a < e.length; a++) {
+            var h = e[a];
             d.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? l(h, r) : !p())
         }
         return !!p()
     }, d = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, p = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && u(e, r) ? r : e), 0)
     }, h = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + c(n) + ")", b = (e, r, t, n) => {
-        var o = p(e, t);
-        return l(n, o) || "undefined" != typeof console && console.warn && console.warn(h(e, t, o, n)), y(e[t][o])
+        var a = p(e, t);
+        return l(n, a) || "undefined" != typeof console && console.warn && console.warn(h(e, t, a, n)), y(e[t][a])
     }, v = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !l(t, r) || e && !u(e, r) ? e : r), 0)) && n[r]
-    }, y = e => (e.loaded = 1, e.get()), g = (m = e => function(r, t, n, o) {
-        var a = E.I(r);
-        return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (d(e, t), b(r, 0, t, n)))), w = m(((e, r, t, n, o) => {
-        var a = r && E.o(r, t) && v(r, t, n);
-        return a ? y(a) : o()
+    }, y = e => (e.loaded = 1, e.get()), g = (m = e => function(r, t, n, a) {
+        var o = E.I(r);
+        return o && o.then ? o.then(e.bind(e, r, E.S[r], t, n, a)) : e(r, E.S[r], t, n, a)
+    })(((e, r, t, n) => (d(e, t), b(r, 0, t, n)))), w = m(((e, r, t, n, a) => {
+        var o = r && E.o(r, t) && v(r, t, n);
+        return o ? y(o) : a()
     })), _ = {}, j = {
         44: () => w("default", "ipycanvas", [2, 0, 8, 2], (() => Promise.all([E.e(353), E.e(648)]).then((() => () => E(353))))),
         216: () => g("default", "@jupyter-widgets/base", [, [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1, 10], 1, 1, 1
         ]),
@@ -309,50 +309,50 @@
                 },
                 n = r => {
                     delete _[e], E.m[e] = t => {
                         throw delete E.c[e], r
                     }
                 };
             try {
-                var o = j[e]();
-                o.then ? r.push(_[e] = o.then(t).catch(n)) : t(o)
+                var a = j[e]();
+                a.then ? r.push(_[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             957: 0
         };
         E.f.j = (r, t) => {
             var n = E.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (648 != r) {
-                var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                t.push(n[2] = o);
-                var a = E.p + E.u(r),
+                var a = new Promise(((t, a) => n = e[r] = [t, a]));
+                t.push(n[2] = a);
+                var o = E.p + E.u(r),
                     i = new Error;
-                E.l(a, (t => {
+                E.l(o, (t => {
                     if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var o = t && ("load" === t.type ? "missing" : t.type),
-                            a = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                        var a = t && ("load" === t.type ? "missing" : t.type),
+                            o = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, o, [a, i, f] = t,
+                var n, a, [o, i, f] = t,
                     s = 0;
-                if (a.some((r => 0 !== e[r]))) {
+                if (o.some((r => 0 !== e[r]))) {
                     for (n in i) E.o(i, n) && (E.m[n] = i[n]);
                     f && f(E)
                 }
-                for (r && r(t); s < a.length; s++) o = a[s], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); s < o.length; s++) a = o[s], E.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_yt_project_yt_widgets = self.webpackChunk_yt_project_yt_widgets || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
     var k = E(338);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@yt-project/yt-widgets"] = k
 })();
```

### Comparing `widgyts-0.5.0/widgyts/labextension/static/third-party-licenses.json` & `widgyts-0.5.1/widgyts/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/widgyts/tests/test_widgyts.py` & `widgyts-0.5.1/widgyts/tests/test_widgyts.py`

 * *Files identical despite different names*

### Comparing `widgyts-0.5.0/widgyts.egg-info/PKG-INFO` & `widgyts-0.5.1/widgyts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgyts
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Custom Jupyter Widget Library for Interactive Visualization with yt
 Home-page: https://github.com/yt-project/widgyts
 Author: The yt Project
 Author-email: yt-dev@python.org
 License: BSD-3-Clause
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://widgyts.readthedocs.org/
@@ -84,15 +84,15 @@
 recent enough version of Jupyterlab, preferably 0.35 or above.  For a
 development installation, do:
 
     $ jupyter labextension install js
 
 To install the latest released version,
 
-    $ jupyter labextension install @data-exp-lab/yt-widgets
+    $ jupyter labextension install @yt-project/yt-widgets
 
 Using
 -----
 
 To use this, you will need to have yt installed.  Importing it monkeypatches
 the Slice and Projection objects, so you are now able to do:
```

### Comparing `widgyts-0.5.0/widgyts.egg-info/SOURCES.txt` & `widgyts-0.5.1/widgyts.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 widgyts/labextension/package.json
 widgyts/labextension/static/353.b96de7a6ab53ee83a3e3.js
 widgyts/labextension/static/353.b96de7a6ab53ee83a3e3.js.LICENSE.txt
 widgyts/labextension/static/35962d9a369f94cd12dc.module.wasm
 widgyts/labextension/static/480.f221211101f033161e08.js
 widgyts/labextension/static/568.dc67e4d4b7ec920ad835.js
 widgyts/labextension/static/7.578ca98bdcc06909a72d.js
-widgyts/labextension/static/724.68ad0e0a95918b09cc71.js
+widgyts/labextension/static/724.1d0ec7e99e0045b1da9c.js
 widgyts/labextension/static/776.034dd82e5586eada2301.js
 widgyts/labextension/static/818.070644e61f231f18d729.js
-widgyts/labextension/static/remoteEntry.59b399c5575c4621e134.js
+widgyts/labextension/static/remoteEntry.5d4e0ace3da9f461d3dc.js
 widgyts/labextension/static/style.js
 widgyts/labextension/static/third-party-licenses.json
 widgyts/tests/__init__.py
 widgyts/tests/test_widgyts.py
```

### Comparing `widgyts-0.5.0/yarn.lock` & `widgyts-0.5.1/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1807,17 +1807,17 @@
 
 "@types/json-schema@*", "@types/json-schema@^7.0.3", "@types/json-schema@^7.0.5", "@types/json-schema@^7.0.7", "@types/json-schema@^7.0.8":
   version "7.0.11"
   resolved "https://registry.yarnpkg.com/@types/json-schema/-/json-schema-7.0.11.tgz#d421b6c527a3037f7c84433fd2c4229e016863d3"
   integrity sha512-wOuvG1SN4Us4rez+tylwwwCV1psiNVOkJeM3AUWUNWg/jDQY2+HE/444y5gc+jBmRqASOm2Oeh5c1axHobwRKQ==
 
 "@types/lodash@^4.14.134":
-  version "4.14.192"
-  resolved "https://registry.yarnpkg.com/@types/lodash/-/lodash-4.14.192.tgz#5790406361a2852d332d41635d927f1600811285"
-  integrity sha512-km+Vyn3BYm5ytMO13k9KTp27O75rbQ0NFw+U//g+PX7VZyjCioXaRFisqSIJRECljcTv73G3i6BpglNGHgUQ5A==
+  version "4.14.194"
+  resolved "https://registry.yarnpkg.com/@types/lodash/-/lodash-4.14.194.tgz#b71eb6f7a0ff11bff59fc987134a093029258a76"
+  integrity sha512-r22s9tAS7imvBt2lyHC9B8AGwWnXaYb1tY09oyLkXDs4vArpYJzw09nj8MLx5VfciBPGIb+ZwG0ssYnEPJxn/g==
 
 "@types/mocha@^5.2.5":
   version "5.2.7"
   resolved "https://registry.yarnpkg.com/@types/mocha/-/mocha-5.2.7.tgz#315d570ccb56c53452ff8638738df60726d5b6ea"
   integrity sha512-NYrtPht0wGzhwe9+/idPaBB+TqkY9AhTvOLMkThm0IoEfLaiVQZwBwyJ5puCkO3AUCWrmcoePjp2mbFocKy4SQ==
 
 "@types/node@*":
@@ -3262,24 +3262,24 @@
 
 copy-descriptor@^0.1.0:
   version "0.1.1"
   resolved "https://registry.yarnpkg.com/copy-descriptor/-/copy-descriptor-0.1.1.tgz#676f6eb3c39997c2ee1ac3a924fd6124748f578d"
   integrity sha512-XgZ0pFcakEUlbwQEVNg3+QAis1FyTL3Qel9FYy8pSkQqoG3PNoT0bOCQtOXcOkur21r2Eq2kI+IE+gsmAEVlYw==
 
 core-js-compat@^3.25.1:
-  version "3.30.0"
-  resolved "https://registry.yarnpkg.com/core-js-compat/-/core-js-compat-3.30.0.tgz#99aa2789f6ed2debfa1df3232784126ee97f4d80"
-  integrity sha512-P5A2h/9mRYZFIAP+5Ab8ns6083IyVpSclU74UNvbGVQ8VM7n3n3/g2yF3AkKQ9NXz2O+ioxLbEWKnDtgsFamhg==
+  version "3.30.1"
+  resolved "https://registry.yarnpkg.com/core-js-compat/-/core-js-compat-3.30.1.tgz#961541e22db9c27fc48bfc13a3cafa8734171dfe"
+  integrity sha512-d690npR7MC6P0gq4npTl5n2VQeNAmUrJ90n+MHiKS7W2+xno4o3F5GDEuylSdi6EJ3VssibSGXOa1r3YXD3Mhw==
   dependencies:
     browserslist "^4.21.5"
 
 core-js-pure@^3.6.5:
-  version "3.30.0"
-  resolved "https://registry.yarnpkg.com/core-js-pure/-/core-js-pure-3.30.0.tgz#41b6c42e5f363bd53d79999bd35093b17e42e1bf"
-  integrity sha512-+2KbMFGeBU0ln/csoPqTe0i/yfHbrd2EUhNMObsGtXMKS/RTtlkYyi+/3twLcevbgNR0yM/r0Psa3TEoQRpFMQ==
+  version "3.30.1"
+  resolved "https://registry.yarnpkg.com/core-js-pure/-/core-js-pure-3.30.1.tgz#7d93dc89e7d47b8ef05d7e79f507b0e99ea77eec"
+  integrity sha512-nXBEVpmUnNRhz83cHd9JRQC52cTMcuXAmR56+9dSMpRdpeA4I1PX6yjmhd71Eyc/wXNsdBdUDIj1QTIeZpU5Tg==
 
 core-js@^2.2.0:
   version "2.6.12"
   resolved "https://registry.yarnpkg.com/core-js/-/core-js-2.6.12.tgz#d9333dfa7b065e347cc5682219d6f690859cc2ec"
   integrity sha512-Kb2wC0fvsWfQrgk8HU5lW6U/Lcs8+9aaYcy4ZFc6DDlo4nZ7n70dEgE5rtR0oG6ufKDUnrwfWL1mXR5ljDatrQ==
 
 core-util-is@~1.0.0:
@@ -3682,17 +3682,17 @@
 
 ee-first@1.1.1:
   version "1.1.1"
   resolved "https://registry.yarnpkg.com/ee-first/-/ee-first-1.1.1.tgz#590c61156b0ae2f4f0255732a158b266bc56b21d"
   integrity sha512-WMwm9LhRUo+WUaRN+vRuETqG89IgZphVSNkdFgeb6sS/E4OrDIN7t48CAewSHXc6C8lefD8KKfr5vY61brQlow==
 
 electron-to-chromium@^1.4.284:
-  version "1.4.359"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.359.tgz#5c4d13cb08032469fcd6bd36457915caa211356b"
-  integrity sha512-OoVcngKCIuNXtZnsYoqlCvr0Cf3NIPzDIgwUfI9bdTFjXCrr79lI0kwQstLPZ7WhCezLlGksZk/BFAzoXC7GDw==
+  version "1.4.363"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.363.tgz#a3d51d16169d8f212f00bafb78cf0667e24c3647"
+  integrity sha512-ReX5qgmSU7ybhzMuMdlJAdYnRhT90UB3k9M05O5nF5WH3wR5wgdJjXw0uDeFyKNhmglmQiOxkAbzrP0hMKM59g==
 
 elliptic@^6.5.3:
   version "6.5.4"
   resolved "https://registry.yarnpkg.com/elliptic/-/elliptic-6.5.4.tgz#da37cebd31e79a1367e941b592ed1fbebd58abbb"
   integrity sha512-iLhC6ULemrljPZb+QutR5TQGB+pdW6KGD5RSegS+8sorOZT+rdQFbsQFJgvN3eRqNALqJer4oQ16YvJHlU8hzQ==
   dependencies:
     bn.js "^4.11.9"
```

