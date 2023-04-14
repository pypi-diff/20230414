# Comparing `tmp/segment-reshape-qgis-plugin-0.1.3.tar.gz` & `tmp/segment-reshape-qgis-plugin-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-reshape-qgis-plugin-0.1.3.tar", last modified: Thu Mar 23 11:03:45 2023, max compression
+gzip compressed data, was "segment-reshape-qgis-plugin-0.1.4.tar", last modified: Fri Apr 14 06:19:21 2023, max compression
```

## Comparing `segment-reshape-qgis-plugin-0.1.3.tar` & `segment-reshape-qgis-plugin-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:45.482654 segment-reshape-qgis-plugin-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-03-23 11:03:45.482654 segment-reshape-qgis-plugin-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-23 11:03:45.482654 segment-reshape-qgis-plugin-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:45.478654 segment-reshape-qgis-plugin-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:45.482654 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:45.482654 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/geometry/reshape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:45.482654 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/map_tool/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/map_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/map_tool/segment_reshape_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:45.482654 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/topology/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/topology/find_related.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:45.482654 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:45.482654 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/metadata.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:45.478654 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:45.482654 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/resources/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/resources/i18n/fi.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:45.482654 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-03-23 11:03:31.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/resources/icons/segment_reshape.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 11:03:45.482654 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_qgis_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-03-23 11:03:45.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_qgis_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-23 11:03:45.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_qgis_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 11:03:45.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_qgis_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-23 11:03:45.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_qgis_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-23 11:03:45.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_qgis_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-23 11:03:45.000000 segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_qgis_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:21.809183 segment-reshape-qgis-plugin-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-04-14 06:19:21.809183 segment-reshape-qgis-plugin-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-14 06:19:21.809183 segment-reshape-qgis-plugin-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:21.805183 segment-reshape-qgis-plugin-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:21.805183 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:21.805183 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/geometry/reshape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:21.805183 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/map_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/map_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/map_tool/segment_reshape_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:21.805183 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/topology/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/topology/find_related.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:21.809183 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/utils/geometry_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:21.809183 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/metadata.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:21.805183 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:21.809183 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/resources/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/resources/i18n/fi.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:21.809183 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-14 06:19:12.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/resources/icons/segment_reshape.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:19:21.809183 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_qgis_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-04-14 06:19:21.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_qgis_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-14 06:19:21.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_qgis_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:19:21.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_qgis_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 06:19:21.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_qgis_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 06:19:21.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_qgis_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 06:19:21.000000 segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_qgis_plugin.egg-info/top_level.txt
```

### Comparing `segment-reshape-qgis-plugin-0.1.3/CHANGELOG.md` & `segment-reshape-qgis-plugin-0.1.4/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # CHANGELOG
 
+## [0.1.4] - 2023-04-14
+
+- Feature: Change the mouse cursor to the wait cursor when finding common segment os editing is in progress
+- Performance improvments. Finding a common segment should now be a magnitude faster with large geometries.
+
 ## [0.1.3] - 2023-03-23
 
 - Feature: Digitizing the new geometry for a segment behaves now as the native QGIS digitizing tools. It supports etc. snapping, tracing and advanced cad tools.
 - Feature: Map tool button is enabled only when a line or polygon layer is active. This is implemented through MapToolHandler which ensures that the tool behaves like rest of the map tools. This means also that the tool can be deactivated only by selecting another map tool.
 - Fix: Color of the start point indicator line was changed to grey to make difference to the digitized line.
 
 ## [0.1.2] - 2023-02-23
@@ -39,7 +44,8 @@
 [0.0.1]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.0.1
 [0.0.2]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.0.2
 [0.0.3]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.0.3
 [0.1.0]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.0
 [0.1.1]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.1
 [0.1.2]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.2
 [0.1.3]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.3
+[0.1.4]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.4
```

### Comparing `segment-reshape-qgis-plugin-0.1.3/LICENSE` & `segment-reshape-qgis-plugin-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-reshape-qgis-plugin-0.1.3/PKG-INFO` & `segment-reshape-qgis-plugin-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-reshape-qgis-plugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: QGIS plugin with a map tool to reshape a continuous segment topogically.
 Home-page: https://github.com/nlsfi/segment-reshape-qgis-plugin
 Author: National Land Survey of Finland
 Author-email: eero.hietanen@maanmittauslaitos.fi
 License: GNU GPL v3.0
 Project-URL: Changelog, https://github.com/nlsfi/segment-reshape-qgis-plugin/blob/main/CHANGELOG.md
 Keywords: qgis
@@ -97,14 +97,19 @@
 Copyright (C) 2022 [National Land Survey of Finland].
 
 [National Land Survey of Finland]: https://www.maanmittauslaitos.fi/en
 [qgis-plugin-dev-tools]: https://github.com/nlsfi/qgis-plugin-dev-tools
 
 # CHANGELOG
 
+## [0.1.4] - 2023-04-14
+
+- Feature: Change the mouse cursor to the wait cursor when finding common segment os editing is in progress
+- Performance improvments. Finding a common segment should now be a magnitude faster with large geometries.
+
 ## [0.1.3] - 2023-03-23
 
 - Feature: Digitizing the new geometry for a segment behaves now as the native QGIS digitizing tools. It supports etc. snapping, tracing and advanced cad tools.
 - Feature: Map tool button is enabled only when a line or polygon layer is active. This is implemented through MapToolHandler which ensures that the tool behaves like rest of the map tools. This means also that the tool can be deactivated only by selecting another map tool.
 - Fix: Color of the start point indicator line was changed to grey to make difference to the digitized line.
 
 ## [0.1.2] - 2023-02-23
@@ -140,7 +145,8 @@
 [0.0.1]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.0.1
 [0.0.2]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.0.2
 [0.0.3]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.0.3
 [0.1.0]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.0
 [0.1.1]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.1
 [0.1.2]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.2
 [0.1.3]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.3
+[0.1.4]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.4
```

### Comparing `segment-reshape-qgis-plugin-0.1.3/README.md` & `segment-reshape-qgis-plugin-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `segment-reshape-qgis-plugin-0.1.3/setup.cfg` & `segment-reshape-qgis-plugin-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/__init__.py` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 #  of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with segment-reshape-qgis-plugin. If not, see <https://www.gnu.org/licenses/>.
 
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/geometry/__init__.py` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/geometry/reshape.py` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/geometry/reshape.py`

 * *Files identical despite different names*

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/map_tool/__init__.py` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/map_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/map_tool/segment_reshape_tool.py` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/map_tool/segment_reshape_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,24 @@
 #
 #  You should have received a copy of the GNU General Public License
 #  along with segment-reshape-qgis-plugin. If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 from contextlib import contextmanager
 from enum import Enum, IntEnum
-from typing import TYPE_CHECKING, Iterator, Optional, Tuple, Union, cast, overload
+from typing import (
+    TYPE_CHECKING,
+    Generator,
+    Iterator,
+    Optional,
+    Tuple,
+    Union,
+    cast,
+    overload,
+)
 
 from qgis.core import (
     QgsApplication,
     QgsGeometry,
     QgsLineString,
     QgsPoint,
     QgsPointLocator,
@@ -39,14 +48,15 @@
     QgsMapMouseEvent,
     QgsMapToolCapture,
     QgsMapToolIdentify,
     QgsRubberBand,
 )
 from qgis.PyQt.QtCore import Qt
 from qgis.PyQt.QtGui import QColor, QKeyEvent
+from qgis.PyQt.QtWidgets import QApplication
 from qgis.utils import iface as iface_
 from qgis_plugin_tools.tools.decorations import log_if_fails
 from qgis_plugin_tools.tools.i18n import tr
 from qgis_plugin_tools.tools.messages import MsgBar
 
 from segment_reshape.geometry import reshape
 from segment_reshape.topology import find_related
@@ -74,14 +84,23 @@
         tool = QgsMapToolIdentify(iface.mapCanvas())
         try:
             yield tool
         finally:
             tool.deleteLater()
 
 
+@contextmanager
+def override_cursor(cursor: Qt.CursorShape) -> Generator[None, None, None]:
+    QApplication.setOverrideCursor(cursor)
+    try:
+        yield
+    finally:
+        QApplication.restoreOverrideCursor()
+
+
 COLOR_BLUE = QColor(10, 20, 150)
 COLOR_GREY = QColor(211, 211, 211)
 
 
 class ToolMode(Enum):
     PICK_SEGMENT = "pick_segment"
     RESHAPE = "reshape"
@@ -235,57 +254,58 @@
 
     def cadCanvasMoveEvent(self, mouse_event: QgsMapMouseEvent) -> None:  # noqa: N802
         if self._tool_mode == ToolMode.RESHAPE and self.size() == 0:
             self.start_point_indicator_rubber_band.movePoint(mouse_event.mapPoint())
         return super().cadCanvasMoveEvent(mouse_event)
 
     def _handle_pick_segment_left_click(self, location: QgsPointXY) -> None:
-        common_segment, layer = self._find_common_segment(location)
-
-        # No active layer or active layer feature found
-        if layer is None:
-            return
+        with override_cursor(Qt.WaitCursor):
+            common_segment, layer = self._find_common_segment(location)
+            # No active layer or active layer feature found
+            if layer is None:
+                return
+
+            if common_segment is None:
+                MsgBar.info(
+                    tr("No common segment found at location"),
+                    tr(
+                        "Features are not topologically connected "
+                        "or a single vertex was clicked"
+                    ),
+                )
+                return
 
-        if common_segment is None:
             MsgBar.info(
-                tr("No common segment found at location"),
-                tr(
-                    "Features are not topologically connected "
-                    "or a single vertex was clicked"
-                ),
+                tr("Common segment found, changing to reshape mode"),
+                success=True,
             )
-            return
-
-        MsgBar.info(
-            tr("Common segment found, changing to reshape mode"),
-            success=True,
-        )
-        self._change_to_reshape_mode_for_geom(QgsGeometry(common_segment), layer)
+            self._change_to_reshape_mode_for_geom(QgsGeometry(common_segment), layer)
 
     def _handle_reshape_right_click(self) -> None:
-        new_geometry = self.captureCurve().curveToLine()
-        self.stopCapturing()
+        with override_cursor(Qt.WaitCursor):
+            new_geometry = self.captureCurve().curveToLine()
+            self.stopCapturing()
 
-        if new_geometry.isEmpty():
-            self._change_to_pick_location_mode()
-            return
+            if new_geometry.isEmpty():
+                self._change_to_pick_location_mode()
+                return
 
-        new_geometry.addZValue(self.defaultZValue())
-        reshape_geom: Union[QgsPoint, QgsLineString] = new_geometry
-        if new_geometry.numPoints() == 1:
-            reshape_geom = new_geometry.pointN(0)
-
-        reshape.make_reshape_edits(
-            self.find_segment_results.common_parts,
-            self.find_segment_results.edges,
-            reshape_geom,
-        )
+            new_geometry.addZValue(self.defaultZValue())
+            reshape_geom: Union[QgsPoint, QgsLineString] = new_geometry
+            if new_geometry.numPoints() == 1:
+                reshape_geom = new_geometry.pointN(0)
+
+            reshape.make_reshape_edits(
+                self.find_segment_results.common_parts,
+                self.find_segment_results.edges,
+                reshape_geom,
+            )
 
-        self._change_to_pick_location_mode()
-        self.canvas().refresh()
+            self._change_to_pick_location_mode()
+            self.canvas().refresh()
 
     def _find_common_segment(
         self, location: QgsPointXY
     ) -> Tuple[Optional[QgsLineString], Optional[QgsVectorLayer]]:
         LOGGER.info("Calculating common segment")
 
         active_layer = iface.activeLayer()
```

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/topology/__init__.py` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/topology/__init__.py`

 * *Files identical despite different names*

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/topology/find_related.py` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/topology/find_related.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,40 +13,31 @@
 #  useful, but WITHOUT ANY WARRANTY; without even the implied warranty
 #  of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with segment-reshape-qgis-plugin. If not, see <https://www.gnu.org/licenses/>.
 
-from typing import (
-    FrozenSet,
-    Iterable,
-    Iterator,
-    List,
-    NamedTuple,
-    Optional,
-    Set,
-    Tuple,
-    cast,
-)
+from typing import FrozenSet, Iterable, Iterator, List, NamedTuple, Optional, Set, Tuple
 
 from qgis.core import (
+    QgsAbstractGeometry,
     QgsFeature,
     QgsFeatureRequest,
     QgsGeometry,
     QgsLineString,
     QgsPoint,
-    QgsPointXY,
     QgsPolygon,
     QgsProject,
     QgsVectorLayer,
     QgsWkbTypes,
 )
 
 from segment_reshape.geometry.reshape import ReshapeCommonPart, ReshapeEdge
+from segment_reshape.utils.geometry_utils import vertices
 
 Point = Tuple[float, float]
 Segment = FrozenSet[Point]
 
 
 class CommonGeometriesResult(NamedTuple):
     segment: Optional[QgsLineString]
@@ -98,34 +89,40 @@
     return layer.id() == other_layer.id() and feature.id() == other_feature.id()
 
 
 def find_related_features(
     layer: QgsVectorLayer,
     feature: QgsFeature,
     candidate_layers: Optional[List[QgsVectorLayer]] = None,
-) -> List[Tuple[QgsVectorLayer, QgsFeature]]:
+) -> Iterator[Tuple[QgsVectorLayer, QgsFeature]]:
     if candidate_layers is None:
         candidate_layers = _find_topologically_related_project_layers(layer)
 
-    # distance within 0 should work, bbox rect would return excess stuff,
-    # feature must have equal vertex anyway for it be considered
+    feature_geometry = feature.geometry()
+
+    feature_geometry_engine = QgsGeometry.createGeometryEngine(
+        feature_geometry.constGet()
+    )
+    feature_geometry_engine.prepareGeometry()
+
     request = QgsFeatureRequest()
-    request.setDistanceWithin(feature.geometry(), 0)
+    request.setFilterRect(feature_geometry.boundingBox())  # noqa: SC200
 
-    return [
+    return (
         (candidate_layer, candidate_feature)
         for candidate_layer in candidate_layers
         for candidate_feature in candidate_layer.getFeatures(request)
         if not _is_same_feature(
             candidate_layer,
             candidate_feature,
             layer,
             feature,
         )
-    ]
+        and feature_geometry_engine.intersects(candidate_feature.geometry().constGet())
+    )
 
 
 def _as_point_or_line_components(geom: QgsGeometry) -> Iterator[QgsGeometry]:
     for part in geom.constParts():
         if isinstance(part, QgsPolygon):
             yield QgsGeometry(part.exteriorRing().clone())
             for ring_index in range(part.numInteriorRings()):
@@ -164,22 +161,48 @@
             return QgsGeometry(part.exteriorRing().clone())
         else:
             return QgsGeometry(part.interiorRing(vertex_details.ring - 1).clone())
     else:
         return QgsGeometry(part.clone())
 
 
-def _find_vertex_indices(geom: QgsGeometry, positions: Iterable[QgsPoint]) -> List[int]:
-    indices: List[int] = []
-    for position in positions:
-        distance, vertex_index = geom.closestVertexWithContext(QgsPointXY(position))
-        if distance != 0:
-            raise ValueError(f"could not find vertex index for {position} from {geom}")
-        indices.append(vertex_index)
-    return indices
+def _find_vertex_indices(
+    geom: QgsGeometry, segment: "QgsAbstractGeometry"
+) -> List[int]:
+    """Returns vertex indices of the geometry for matching vertices in the segment
+
+    Args:
+        geom (QgsGeometry): Geometry whose indices are requested
+        segment (QgsAbstractGeometry): Segment geometry (usually QgsPolyline
+            or QgsPoint) we want to match
+
+    Raises:
+        ValueError: Raises ValueError if some vertex from segment is not found
+            from the geom.
+
+    Returns:
+        List[int]: List of vertex indices of the geometry in every matcing vertex
+            of the segment
+    """
+
+    # Loop geometry only once and "cache" indices
+    vertex_to_id_map = {
+        (vertex.x(), vertex.y()): vertex_id for vertex_id, vertex in vertices(geom)
+    }
+
+    result: List[int] = []
+    for segment_vertex in segment.vertices():
+        try:
+            result.append(vertex_to_id_map[(segment_vertex.x(), segment_vertex.y())])
+        except KeyError:
+            raise ValueError(
+                f"could not find vertex index for {segment_vertex} from {geom}"
+            )
+
+    return result
 
 
 def _check_if_vertices_are_reversed(vertex_indices: List[int]) -> bool:
     first, second = vertex_indices[:2]
     return any(
         [
             (abs(first - second) == 1 and first > second),
@@ -187,15 +210,15 @@
         ]
     )
 
 
 def get_common_geometries(
     main_feature_layer: QgsVectorLayer,
     main_feature: QgsFeature,
-    related_features_by_layer: List[Tuple[QgsVectorLayer, QgsFeature]],
+    related_features_by_layer: Iterable[Tuple[QgsVectorLayer, QgsFeature]],
     main_feature_segment: Tuple[int, int],
 ) -> CommonGeometriesResult:
     # for now lines and polygons are supported as the trigger
     if main_feature.geometry().type() not in [
         QgsWkbTypes.GeometryType.LineGeometry,
         QgsWkbTypes.GeometryType.PolygonGeometry,
     ]:
@@ -266,61 +289,59 @@
 
     start, end = QgsGeometry(segment.startPoint()), QgsGeometry(segment.endPoint())
 
     common_parts: List[ReshapeCommonPart] = [
         ReshapeCommonPart(
             main_feature_layer,
             main_feature,
-            _find_vertex_indices(main_feature.geometry(), segment.vertices()),
+            _find_vertex_indices(main_feature.geometry(), segment),
             is_reversed=False,
         )
     ]
     for common_part_candidate in common_part_candidates:
         layer, feature = common_part_candidate
-        indices = _find_vertex_indices(feature.geometry(), segment.vertices())
+        indices = _find_vertex_indices(feature.geometry(), segment)
         common_parts.append(
             ReshapeCommonPart(
                 layer,
                 feature,
                 indices,
                 is_reversed=_check_if_vertices_are_reversed(indices),
             )
         )
 
     edges: List[ReshapeEdge] = []
     for possible_edge_candidate in possible_edge_candidates:
         layer, feature, component = possible_edge_candidate
         if start.intersects(component):
-            indices = _find_vertex_indices(feature.geometry(), [segment.startPoint()])
+            indices = _find_vertex_indices(feature.geometry(), segment.startPoint())
             edges.append(
                 ReshapeEdge(
                     layer,
                     feature,
                     indices[0],
                     is_start=True,
                 )
             )
         if end.intersects(component):
-            indices = _find_vertex_indices(feature.geometry(), [segment.endPoint()])
+            indices = _find_vertex_indices(feature.geometry(), segment.endPoint())
             edges.append(
                 ReshapeEdge(
                     layer,
                     feature,
                     indices[0],
                     is_start=False,
                 )
             )
 
     return CommonGeometriesResult(segment, common_parts, edges)
 
 
 def _as_line_segments(geometry: QgsGeometry) -> Set[Segment]:
-    vertices = [
-        (point.x(), point.y()) for point in cast(QgsLineString, geometry.asPolyline())
-    ]
+    vertices = [(point.x(), point.y()) for point in geometry.vertices()]
     return {frozenset(line) for line in zip(vertices, vertices[1:])}
 
 
 def _build_line_from_line_segment_set(
     trigger_part: QgsGeometry,
     line_segments_to_keep: Set[Segment],
     trigger_segment: Segment,
```

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape/utils/__init__.py` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape/utils/geometry_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,22 +13,37 @@
 #  useful, but WITHOUT ANY WARRANTY; without even the implied warranty
 #  of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with segment-reshape-qgis-plugin. If not, see <https://www.gnu.org/licenses/>.
 
-from typing import Union
 
-from qgis.core import QgsAbstractGeometry, QgsGeometry
+from typing import Iterator, Tuple, Union
+
+from qgis.core import QgsAbstractGeometry, QgsGeometry, QgsPoint
 
 
 def clone_geometry_safely(
     geometry: Union[QgsGeometry, QgsAbstractGeometry]
 ) -> QgsGeometry:
     if isinstance(geometry, QgsGeometry):
         original_abstract_geometry = geometry.get()
         cloned_original_abstract_geometry = original_abstract_geometry.clone()
         return QgsGeometry(cloned_original_abstract_geometry)
     else:
         cloned_original_abstract_geometry = geometry.clone()
         return QgsGeometry(cloned_original_abstract_geometry)
+
+
+def vertices(geometry: QgsGeometry) -> Iterator[Tuple[int, QgsPoint]]:
+    """Generator for vertex_ids and vertices of the geometry
+
+    Args:
+        geometry (QgsGeometry): Input geometry
+
+    Yields:
+        Iterator[Tuple[int, QgsPoint]]: Tuple contains vertex_id and vertex point
+    """
+
+    for vertex_id, vertex in enumerate(geometry.vertices()):
+        yield (vertex_id, vertex)
```

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/__init__.py` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/metadata.txt` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/metadata.txt`

 * *Files identical despite different names*

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/plugin.py` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/resources/i18n/fi.ts` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/resources/i18n/fi.ts`

 * *Files identical despite different names*

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_plugin/resources/icons/segment_reshape.svg` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_plugin/resources/icons/segment_reshape.svg`

 * *Files identical despite different names*

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_qgis_plugin.egg-info/PKG-INFO` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_qgis_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-reshape-qgis-plugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: QGIS plugin with a map tool to reshape a continuous segment topogically.
 Home-page: https://github.com/nlsfi/segment-reshape-qgis-plugin
 Author: National Land Survey of Finland
 Author-email: eero.hietanen@maanmittauslaitos.fi
 License: GNU GPL v3.0
 Project-URL: Changelog, https://github.com/nlsfi/segment-reshape-qgis-plugin/blob/main/CHANGELOG.md
 Keywords: qgis
@@ -97,14 +97,19 @@
 Copyright (C) 2022 [National Land Survey of Finland].
 
 [National Land Survey of Finland]: https://www.maanmittauslaitos.fi/en
 [qgis-plugin-dev-tools]: https://github.com/nlsfi/qgis-plugin-dev-tools
 
 # CHANGELOG
 
+## [0.1.4] - 2023-04-14
+
+- Feature: Change the mouse cursor to the wait cursor when finding common segment os editing is in progress
+- Performance improvments. Finding a common segment should now be a magnitude faster with large geometries.
+
 ## [0.1.3] - 2023-03-23
 
 - Feature: Digitizing the new geometry for a segment behaves now as the native QGIS digitizing tools. It supports etc. snapping, tracing and advanced cad tools.
 - Feature: Map tool button is enabled only when a line or polygon layer is active. This is implemented through MapToolHandler which ensures that the tool behaves like rest of the map tools. This means also that the tool can be deactivated only by selecting another map tool.
 - Fix: Color of the start point indicator line was changed to grey to make difference to the digitized line.
 
 ## [0.1.2] - 2023-02-23
@@ -140,7 +145,8 @@
 [0.0.1]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.0.1
 [0.0.2]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.0.2
 [0.0.3]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.0.3
 [0.1.0]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.0
 [0.1.1]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.1
 [0.1.2]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.2
 [0.1.3]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.3
+[0.1.4]: https://github.com/nlsfi/segment-reshape-qgis-plugin/releases/tag/v0.1.4
```

### Comparing `segment-reshape-qgis-plugin-0.1.3/src/segment_reshape_qgis_plugin.egg-info/SOURCES.txt` & `segment-reshape-qgis-plugin-0.1.4/src/segment_reshape_qgis_plugin.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/segment_reshape/geometry/__init__.py
 src/segment_reshape/geometry/reshape.py
 src/segment_reshape/map_tool/__init__.py
 src/segment_reshape/map_tool/segment_reshape_tool.py
 src/segment_reshape/topology/__init__.py
 src/segment_reshape/topology/find_related.py
 src/segment_reshape/utils/__init__.py
+src/segment_reshape/utils/geometry_utils.py
 src/segment_reshape_plugin/__init__.py
 src/segment_reshape_plugin/metadata.txt
 src/segment_reshape_plugin/plugin.py
 src/segment_reshape_plugin/py.typed
 src/segment_reshape_plugin/resources/i18n/fi.ts
 src/segment_reshape_plugin/resources/icons/segment_reshape.svg
 src/segment_reshape_qgis_plugin.egg-info/PKG-INFO
```

