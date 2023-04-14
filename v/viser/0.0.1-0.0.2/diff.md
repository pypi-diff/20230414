# Comparing `tmp/viser-0.0.1.tar.gz` & `tmp/viser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viser-0.0.1.tar", max compression
+gzip compressed data, was "viser-0.0.2.tar", max compression
```

## Comparing `viser-0.0.1.tar` & `viser-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1791 2023-04-14 19:34:02.302478 viser-0.0.1/README.md
--rw-r--r--   0        0        0      647 2023-04-14 19:34:02.302478 viser-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      578 2023-04-14 19:34:02.302478 viser-0.0.1/viser/__init__.py
--rw-r--r--   0        0        0     5503 2023-04-14 19:34:02.302478 viser-0.0.1/viser/_gui.py
--rw-r--r--   0        0        0    21128 2023-04-14 19:34:02.302478 viser-0.0.1/viser/_message_api.py
--rw-r--r--   0        0        0     5918 2023-04-14 19:34:02.302478 viser-0.0.1/viser/_messages.py
--rw-r--r--   0        0        0     3249 2023-04-14 19:34:02.302478 viser-0.0.1/viser/_scene_handle.py
--rw-r--r--   0        0        0     4146 2023-04-14 19:34:02.302478 viser-0.0.1/viser/_viser.py
--rw-r--r--   0        0        0     1115 2023-04-14 19:34:02.302478 viser-0.0.1/viser/client/.eslintrc.js
--rw-r--r--   0        0        0      289 2023-04-14 19:34:02.302478 viser-0.0.1/viser/client/.gitignore
--rw-r--r--   0        0        0     2117 2023-04-14 19:34:02.302478 viser-0.0.1/viser/client/README.md
--rw-r--r--   0        0        0      369 2023-04-14 19:34:02.302478 viser-0.0.1/viser/client/build/asset-manifest.json
--rw-r--r--   0        0        0     1800 2023-04-14 19:34:02.302478 viser-0.0.1/viser/client/build/favicon.svg
--rw-r--r--   0        0        0      640 2023-04-14 19:34:02.302478 viser-0.0.1/viser/client/build/index.html
--rw-r--r--   0        0        0      286 2023-04-14 19:34:02.302478 viser-0.0.1/viser/client/build/manifest.json
--rw-r--r--   0        0        0       67 2023-04-14 19:34:02.302478 viser-0.0.1/viser/client/build/robots.txt
--rw-r--r--   0        0        0      441 2023-04-14 19:34:02.302478 viser-0.0.1/viser/client/build/static/css/main.992126cd.css
--rw-r--r--   0        0        0      843 2023-04-14 19:34:02.302478 viser-0.0.1/viser/client/build/static/css/main.992126cd.css.map
--rw-r--r--   0        0        0  1510463 2023-04-14 19:34:02.310479 viser-0.0.1/viser/client/build/static/js/main.721d9a9f.js
--rw-r--r--   0        0        0     4434 2023-04-14 19:34:02.314478 viser-0.0.1/viser/client/build/static/js/main.721d9a9f.js.LICENSE.txt
--rw-r--r--   0        0        0  5161937 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/build/static/js/main.721d9a9f.js.map
--rw-r--r--   0        0        0     1910 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/package.json
--rw-r--r--   0        0        0     1800 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/public/favicon.svg
--rw-r--r--   0        0        0     1717 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/public/index.html
--rw-r--r--   0        0        0      286 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/public/manifest.json
--rw-r--r--   0        0        0       67 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/public/robots.txt
--rw-r--r--   0        0        0     7126 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/CameraControls.tsx
--rw-r--r--   0        0        0    11080 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/ControlPanel/ControlPanel.tsx
--rw-r--r--   0        0        0     5790 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/ControlPanel/Generated.tsx
--rw-r--r--   0        0        0     2307 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/ControlPanel/GuiState.tsx
--rw-r--r--   0        0        0     3802 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/ControlPanel/SceneTreeUI.tsx
--rw-r--r--   0        0        0     2154 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/ControlPanel/Server.tsx
--rw-r--r--   0        0        0     1120 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/LabelRenderer.tsx
--rw-r--r--   0        0        0     7338 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/SceneTree.tsx
--rw-r--r--   0        0        0     1678 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/SearchParamsUtils.tsx
--rw-r--r--   0        0        0     3840 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/ThreeAssets.tsx
--rw-r--r--   0        0        0    14773 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/WebsocketInterface.tsx
--rw-r--r--   0        0        0     3548 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/WebsocketMessages.tsx
--rw-r--r--   0        0        0      509 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/index.css
--rw-r--r--   0        0        0     6406 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/index.tsx
--rw-r--r--   0        0        0       40 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/src/react-app-env.d.ts
--rw-r--r--   0        0        0      503 2023-04-14 19:34:02.338479 viser-0.0.1/viser/client/tsconfig.json
--rw-r--r--   0        0        0   495759 2023-04-14 19:34:02.342479 viser-0.0.1/viser/client/yarn.lock
--rw-r--r--   0        0        0      160 2023-04-14 19:34:02.342479 viser-0.0.1/viser/extras/__init__.py
--rw-r--r--   0        0        0     4099 2023-04-14 19:34:02.342479 viser-0.0.1/viser/extras/_record3d.py
--rw-r--r--   0        0        0      898 2023-04-14 19:34:02.342479 viser-0.0.1/viser/infra/__init__.py
--rw-r--r--   0        0        0     2994 2023-04-14 19:34:02.342479 viser-0.0.1/viser/infra/_async_message_buffer.py
--rw-r--r--   0        0        0    11095 2023-04-14 19:34:02.342479 viser-0.0.1/viser/infra/_infra.py
--rw-r--r--   0        0        0     2775 2023-04-14 19:34:02.342479 viser-0.0.1/viser/infra/_messages.py
--rw-r--r--   0        0        0     3110 2023-04-14 19:34:02.342479 viser-0.0.1/viser/infra/_typescript_interface_gen.py
--rw-r--r--   0        0        0        0 2023-04-14 19:34:02.342479 viser-0.0.1/viser/py.typed
--rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 viser-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1791 2023-04-14 20:35:30.495308 viser-0.0.2/README.md
+-rw-r--r--   0        0        0      655 2023-04-14 20:35:30.495308 viser-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      578 2023-04-14 20:35:30.495308 viser-0.0.2/viser/__init__.py
+-rw-r--r--   0        0        0     5503 2023-04-14 20:35:30.495308 viser-0.0.2/viser/_gui.py
+-rw-r--r--   0        0        0    21128 2023-04-14 20:35:30.495308 viser-0.0.2/viser/_message_api.py
+-rw-r--r--   0        0        0     5918 2023-04-14 20:35:30.495308 viser-0.0.2/viser/_messages.py
+-rw-r--r--   0        0        0     3249 2023-04-14 20:35:30.495308 viser-0.0.2/viser/_scene_handle.py
+-rw-r--r--   0        0        0     4146 2023-04-14 20:35:30.495308 viser-0.0.2/viser/_viser.py
+-rw-r--r--   0        0        0     1115 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/.eslintrc.js
+-rw-r--r--   0        0        0      289 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/.gitignore
+-rw-r--r--   0        0        0     2117 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/README.md
+-rw-r--r--   0        0        0      369 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/asset-manifest.json
+-rw-r--r--   0        0        0     1800 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/favicon.svg
+-rw-r--r--   0        0        0      640 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/index.html
+-rw-r--r--   0        0        0      286 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/robots.txt
+-rw-r--r--   0        0        0      441 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/static/css/main.992126cd.css
+-rw-r--r--   0        0        0      843 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/static/css/main.992126cd.css.map
+-rw-r--r--   0        0        0  1510463 2023-04-14 20:35:30.503308 viser-0.0.2/viser/client/build/static/js/main.721d9a9f.js
+-rw-r--r--   0        0        0     4434 2023-04-14 20:35:30.503308 viser-0.0.2/viser/client/build/static/js/main.721d9a9f.js.LICENSE.txt
+-rw-r--r--   0        0        0  5161937 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/build/static/js/main.721d9a9f.js.map
+-rw-r--r--   0        0        0     1910 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/package.json
+-rw-r--r--   0        0        0     1800 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/public/favicon.svg
+-rw-r--r--   0        0        0     1717 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/public/index.html
+-rw-r--r--   0        0        0      286 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/public/manifest.json
+-rw-r--r--   0        0        0       67 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/public/robots.txt
+-rw-r--r--   0        0        0     7126 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/CameraControls.tsx
+-rw-r--r--   0        0        0    11080 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/ControlPanel/ControlPanel.tsx
+-rw-r--r--   0        0        0     5790 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/ControlPanel/Generated.tsx
+-rw-r--r--   0        0        0     2307 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/ControlPanel/GuiState.tsx
+-rw-r--r--   0        0        0     3802 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/ControlPanel/SceneTreeUI.tsx
+-rw-r--r--   0        0        0     2154 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/ControlPanel/Server.tsx
+-rw-r--r--   0        0        0     1120 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/LabelRenderer.tsx
+-rw-r--r--   0        0        0     7338 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/SceneTree.tsx
+-rw-r--r--   0        0        0     1678 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/SearchParamsUtils.tsx
+-rw-r--r--   0        0        0     3840 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/ThreeAssets.tsx
+-rw-r--r--   0        0        0    14773 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/WebsocketInterface.tsx
+-rw-r--r--   0        0        0     3548 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/WebsocketMessages.tsx
+-rw-r--r--   0        0        0      509 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/index.css
+-rw-r--r--   0        0        0     6406 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      503 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/tsconfig.json
+-rw-r--r--   0        0        0   495759 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/yarn.lock
+-rw-r--r--   0        0        0      160 2023-04-14 20:35:30.531309 viser-0.0.2/viser/extras/__init__.py
+-rw-r--r--   0        0        0     4099 2023-04-14 20:35:30.531309 viser-0.0.2/viser/extras/_record3d.py
+-rw-r--r--   0        0        0      898 2023-04-14 20:35:30.531309 viser-0.0.2/viser/infra/__init__.py
+-rw-r--r--   0        0        0     2994 2023-04-14 20:35:30.531309 viser-0.0.2/viser/infra/_async_message_buffer.py
+-rw-r--r--   0        0        0    11095 2023-04-14 20:35:30.531309 viser-0.0.2/viser/infra/_infra.py
+-rw-r--r--   0        0        0     2775 2023-04-14 20:35:30.531309 viser-0.0.2/viser/infra/_messages.py
+-rw-r--r--   0        0        0     3110 2023-04-14 20:35:30.531309 viser-0.0.2/viser/infra/_typescript_interface_gen.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:35:30.535308 viser-0.0.2/viser/py.typed
+-rw-r--r--   0        0        0     2623 1970-01-01 00:00:00.000000 viser-0.0.2/PKG-INFO
```

### Comparing `viser-0.0.1/README.md` & `viser-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/pyproject.toml` & `viser-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "viser"
-version = "0.0.1"
+version = "0.0.2"
 description = "3D visualization helper"
 authors = ["brentyi <brentyi@berkeley.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-websockets = "^10.4"
-numpy = ">1.0.0"
-msgpack = ">1.0.0"
-imageio = "^2.26.1"
-pyliblzfse = "^0.4.1"
-scikit-image = ">0.18.0"
-tqdm = "^4.65.0"
-tyro = "^0.4.2"
-gdown = "^4.6.6"
-rich = "^13.3.3"
+websockets = ">=10.4"
+numpy = ">=1.0.0"
+msgpack = ">=1.0.0"
+imageio = ">=2.0.0"
+pyliblzfse = ">=0.4.1"
+scikit-image = ">=0.18.0"
+tqdm = ">=4.0.0"
+tyro = ">=0.2.0"
+gdown = ">=4.6.6"
+rich = ">=13.3.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `viser-0.0.1/viser/__init__.py` & `viser-0.0.2/viser/__init__.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/_gui.py` & `viser-0.0.2/viser/_gui.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/_message_api.py` & `viser-0.0.2/viser/_message_api.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/_messages.py` & `viser-0.0.2/viser/_messages.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/_scene_handle.py` & `viser-0.0.2/viser/_scene_handle.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/_viser.py` & `viser-0.0.2/viser/_viser.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/.eslintrc.js` & `viser-0.0.2/viser/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/README.md` & `viser-0.0.2/viser/client/README.md`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/build/favicon.svg` & `viser-0.0.2/viser/client/build/favicon.svg`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/build/index.html` & `viser-0.0.2/viser/client/build/index.html`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/build/static/css/main.992126cd.css.map` & `viser-0.0.2/viser/client/build/static/css/main.992126cd.css.map`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/build/static/js/main.721d9a9f.js` & `viser-0.0.2/viser/client/build/static/js/main.721d9a9f.js`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/build/static/js/main.721d9a9f.js.LICENSE.txt` & `viser-0.0.2/viser/client/build/static/js/main.721d9a9f.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/build/static/js/main.721d9a9f.js.map` & `viser-0.0.2/viser/client/build/static/js/main.721d9a9f.js.map`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/package.json` & `viser-0.0.2/viser/client/package.json`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/public/favicon.svg` & `viser-0.0.2/viser/client/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/public/index.html` & `viser-0.0.2/viser/client/public/index.html`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/src/CameraControls.tsx` & `viser-0.0.2/viser/client/src/CameraControls.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/src/ControlPanel/ControlPanel.tsx` & `viser-0.0.2/viser/client/src/ControlPanel/ControlPanel.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/src/ControlPanel/Generated.tsx` & `viser-0.0.2/viser/client/src/ControlPanel/Generated.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/src/ControlPanel/GuiState.tsx` & `viser-0.0.2/viser/client/src/ControlPanel/GuiState.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/src/ControlPanel/SceneTreeUI.tsx` & `viser-0.0.2/viser/client/src/ControlPanel/SceneTreeUI.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/src/ControlPanel/Server.tsx` & `viser-0.0.2/viser/client/src/ControlPanel/Server.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/src/LabelRenderer.tsx` & `viser-0.0.2/viser/client/src/LabelRenderer.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/src/SceneTree.tsx` & `viser-0.0.2/viser/client/src/SceneTree.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/src/SearchParamsUtils.tsx` & `viser-0.0.2/viser/client/src/SearchParamsUtils.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/src/ThreeAssets.tsx` & `viser-0.0.2/viser/client/src/ThreeAssets.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/src/WebsocketInterface.tsx` & `viser-0.0.2/viser/client/src/WebsocketInterface.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/src/WebsocketMessages.tsx` & `viser-0.0.2/viser/client/src/WebsocketMessages.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/src/index.tsx` & `viser-0.0.2/viser/client/src/index.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/client/yarn.lock` & `viser-0.0.2/viser/client/yarn.lock`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/extras/_record3d.py` & `viser-0.0.2/viser/extras/_record3d.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/infra/__init__.py` & `viser-0.0.2/viser/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/infra/_async_message_buffer.py` & `viser-0.0.2/viser/infra/_async_message_buffer.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/infra/_infra.py` & `viser-0.0.2/viser/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/infra/_messages.py` & `viser-0.0.2/viser/infra/_messages.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/viser/infra/_typescript_interface_gen.py` & `viser-0.0.2/viser/infra/_typescript_interface_gen.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.1/PKG-INFO` & `viser-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: viser
-Version: 0.0.1
+Version: 0.0.2
 Summary: 3D visualization helper
 Author: brentyi
 Author-email: brentyi@berkeley.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: gdown (>=4.6.6,<5.0.0)
-Requires-Dist: imageio (>=2.26.1,<3.0.0)
-Requires-Dist: msgpack (>1.0.0)
-Requires-Dist: numpy (>1.0.0)
-Requires-Dist: pyliblzfse (>=0.4.1,<0.5.0)
-Requires-Dist: rich (>=13.3.3,<14.0.0)
-Requires-Dist: scikit-image (>0.18.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: tyro (>=0.4.2,<0.5.0)
-Requires-Dist: websockets (>=10.4,<11.0)
+Requires-Dist: gdown (>=4.6.6)
+Requires-Dist: imageio (>=2.0.0)
+Requires-Dist: msgpack (>=1.0.0)
+Requires-Dist: numpy (>=1.0.0)
+Requires-Dist: pyliblzfse (>=0.4.1)
+Requires-Dist: rich (>=13.3.3)
+Requires-Dist: scikit-image (>=0.18.0)
+Requires-Dist: tqdm (>=4.0.0)
+Requires-Dist: tyro (>=0.2.0)
+Requires-Dist: websockets (>=10.4)
 Description-Content-Type: text/markdown
 
 # viser
 
 **[ [API Reference](https://brentyi.github.io/viser) ]** &nbsp;&nbsp;&bull;&nbsp;&nbsp; `pip install viser`
 
 ![pyright](https://github.com/brentyi/viser/workflows/pyright/badge.svg)
```

