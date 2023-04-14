# Comparing `tmp/pandamesh-0.1.1.tar.gz` & `tmp/pandamesh-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandamesh-0.1.1.tar", last modified: Sat Mar 18 21:21:13 2023, max compression
+gzip compressed data, was "pandamesh-0.1.2.tar", last modified: Fri Apr 14 09:57:22 2023, max compression
```

## Comparing `pandamesh-0.1.1.tar` & `pandamesh-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-03-18 21:21:13.362444 pandamesh-0.1.1/
--rw-rw-rw-   0        0        0     1086 2022-11-11 12:12:58.000000 pandamesh-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6110 2023-03-18 21:21:13.362444 pandamesh-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5025 2023-03-18 21:06:27.000000 pandamesh-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-18 21:21:13.325487 pandamesh-0.1.1/pandamesh/
--rw-rw-rw-   0        0        0      462 2023-03-18 20:48:28.000000 pandamesh-0.1.1/pandamesh/__init__.py
--rw-rw-rw-   0        0        0     6692 2023-03-18 17:37:50.000000 pandamesh-0.1.1/pandamesh/common.py
-drwxrwxrwx   0        0        0        0 2023-03-18 21:21:13.340441 pandamesh-0.1.1/pandamesh/data/
--rw-rw-rw-   0        0        0       53 2023-03-18 20:19:17.000000 pandamesh-0.1.1/pandamesh/data/__init__.py
--rw-rw-rw-   0        0        0      601 2023-03-18 20:53:00.000000 pandamesh-0.1.1/pandamesh/data/sample_data.py
--rw-rw-rw-   0        0        0     4522 2023-03-18 20:45:06.000000 pandamesh-0.1.1/pandamesh/gmsh_fields.py
--rw-rw-rw-   0        0        0     9735 2023-03-18 20:45:06.000000 pandamesh-0.1.1/pandamesh/gmsh_geometry.py
--rw-rw-rw-   0        0        0    18482 2023-03-18 20:45:06.000000 pandamesh-0.1.1/pandamesh/gmsh_mesher.py
--rw-rw-rw-   0        0        0      731 2023-03-18 20:44:54.000000 pandamesh-0.1.1/pandamesh/plot.py
--rw-rw-rw-   0        0        0     3529 2023-03-18 20:45:06.000000 pandamesh-0.1.1/pandamesh/triangle_geometry.py
--rw-rw-rw-   0        0        0     7443 2023-03-18 20:45:06.000000 pandamesh-0.1.1/pandamesh/triangle_mesher.py
-drwxrwxrwx   0        0        0        0 2023-03-18 21:21:13.335438 pandamesh-0.1.1/pandamesh.egg-info/
--rw-rw-rw-   0        0        0     6110 2023-03-18 21:21:13.000000 pandamesh-0.1.1/pandamesh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      602 2023-03-18 21:21:13.000000 pandamesh-0.1.1/pandamesh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-18 21:21:13.000000 pandamesh-0.1.1/pandamesh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      208 2023-03-18 21:21:13.000000 pandamesh-0.1.1/pandamesh.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-18 21:21:13.000000 pandamesh-0.1.1/pandamesh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1918 2023-03-18 21:16:06.000000 pandamesh-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      159 2023-03-18 21:21:13.363443 pandamesh-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-18 21:21:13.360440 pandamesh-0.1.1/tests/
--rw-rw-rw-   0        0        0     6077 2023-03-18 17:35:14.000000 pandamesh-0.1.1/tests/test_common.py
--rw-rw-rw-   0        0        0      161 2023-03-18 20:49:53.000000 pandamesh-0.1.1/tests/test_data.py
--rw-rw-rw-   0        0        0     5251 2022-11-11 12:12:58.000000 pandamesh-0.1.1/tests/test_gmsh_geometry.py
--rw-rw-rw-   0        0        0     5028 2022-11-11 12:12:58.000000 pandamesh-0.1.1/tests/test_meshers.py
--rw-rw-rw-   0        0        0      825 2022-11-11 12:12:58.000000 pandamesh-0.1.1/tests/test_plot.py
--rw-rw-rw-   0        0        0     3258 2022-11-11 12:13:49.000000 pandamesh-0.1.1/tests/test_triangle_geometry.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:57:22.634745 pandamesh-0.1.2/
+-rw-rw-rw-   0        0        0     1086 2022-11-11 12:12:58.000000 pandamesh-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6110 2023-04-14 09:57:22.634745 pandamesh-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5025 2023-03-18 21:06:27.000000 pandamesh-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-14 09:57:22.598758 pandamesh-0.1.2/pandamesh/
+-rw-rw-rw-   0        0        0      462 2023-03-18 20:48:28.000000 pandamesh-0.1.2/pandamesh/__init__.py
+-rw-rw-rw-   0        0        0     7438 2023-04-14 09:47:25.000000 pandamesh-0.1.2/pandamesh/common.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:57:22.613746 pandamesh-0.1.2/pandamesh/data/
+-rw-rw-rw-   0        0        0       53 2023-03-18 20:19:17.000000 pandamesh-0.1.2/pandamesh/data/__init__.py
+-rw-rw-rw-   0        0        0      601 2023-03-18 20:53:00.000000 pandamesh-0.1.2/pandamesh/data/sample_data.py
+-rw-rw-rw-   0        0        0     4515 2023-04-14 09:41:10.000000 pandamesh-0.1.2/pandamesh/gmsh_fields.py
+-rw-rw-rw-   0        0        0     9728 2023-04-14 09:41:38.000000 pandamesh-0.1.2/pandamesh/gmsh_geometry.py
+-rw-rw-rw-   0        0        0    18480 2023-04-14 09:41:22.000000 pandamesh-0.1.2/pandamesh/gmsh_mesher.py
+-rw-rw-rw-   0        0        0      731 2023-03-18 20:44:54.000000 pandamesh-0.1.2/pandamesh/plot.py
+-rw-rw-rw-   0        0        0     3529 2023-03-18 20:45:06.000000 pandamesh-0.1.2/pandamesh/triangle_geometry.py
+-rw-rw-rw-   0        0        0     7443 2023-03-18 20:45:06.000000 pandamesh-0.1.2/pandamesh/triangle_mesher.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:57:22.608745 pandamesh-0.1.2/pandamesh.egg-info/
+-rw-rw-rw-   0        0        0     6110 2023-04-14 09:57:22.000000 pandamesh-0.1.2/pandamesh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2023-04-14 09:57:22.000000 pandamesh-0.1.2/pandamesh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:57:22.000000 pandamesh-0.1.2/pandamesh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      203 2023-04-14 09:57:22.000000 pandamesh-0.1.2/pandamesh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 09:57:22.000000 pandamesh-0.1.2/pandamesh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1905 2023-04-14 09:55:32.000000 pandamesh-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      159 2023-04-14 09:57:22.636744 pandamesh-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 09:57:22.632746 pandamesh-0.1.2/tests/
+-rw-rw-rw-   0        0        0     6679 2023-04-14 09:06:51.000000 pandamesh-0.1.2/tests/test_common.py
+-rw-rw-rw-   0        0        0      161 2023-03-18 20:49:53.000000 pandamesh-0.1.2/tests/test_data.py
+-rw-rw-rw-   0        0        0     5251 2023-04-14 09:41:25.000000 pandamesh-0.1.2/tests/test_gmsh_geometry.py
+-rw-rw-rw-   0        0        0     5028 2022-11-11 12:12:58.000000 pandamesh-0.1.2/tests/test_meshers.py
+-rw-rw-rw-   0        0        0      825 2022-11-11 12:12:58.000000 pandamesh-0.1.2/tests/test_plot.py
+-rw-rw-rw-   0        0        0     3258 2022-11-11 12:13:49.000000 pandamesh-0.1.2/tests/test_triangle_geometry.py
```

### Comparing `pandamesh-0.1.1/LICENSE` & `pandamesh-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandamesh-0.1.1/PKG-INFO` & `pandamesh-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandamesh
-Version: 0.1.1
+Version: 0.1.2
 Summary: From geodataframe to mesh
 Maintainer-email: Huite Bootsma <huite.bootsma@deltares.nl>
 License: MIT
 Project-URL: Home, https://github.com/deltares/pandamesh
 Project-URL: Code, https://github.com/deltares/pandamesh
 Project-URL: Issues, https://github.com/deltares/pandamesh/issues
 Keywords: mesh,geopandas,unstructured grid
```

### Comparing `pandamesh-0.1.1/README.rst` & `pandamesh-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pandamesh-0.1.1/pandamesh/common.py` & `pandamesh-0.1.2/pandamesh/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,38 @@
 from enum import Enum
 from itertools import combinations
 from typing import Any, Sequence, Tuple
 
 import geopandas as gpd
 import numpy as np
 
+
+class MaybeGmsh:
+    """
+    Gmsh is an optional dependency.
+    """
+
+    def __init__(self):
+        try:
+            import gmsh
+
+            self.gmsh = gmsh
+            self.ok = True
+        except ImportError:
+            self.gmsh = None
+            self.ok = False
+
+    def __getattr__(self, name: str):
+        if self.ok:
+            return getattr(self.gmsh, name)
+        else:
+            raise ImportError("Gmsh is required for this functionality")
+
+
+gmsh = MaybeGmsh()
 IntArray = np.ndarray
 FloatArray = np.ndarray
 coord_dtype = np.dtype([("x", np.float64), ("y", np.float64)])
 
 
 def repr(obj: Any) -> str:
     strings = [type(obj).__name__]
@@ -38,14 +62,19 @@
 
 
 def check_geodataframe(features: gpd.GeoDataFrame) -> None:
     if not isinstance(features, gpd.GeoDataFrame):
         raise TypeError(
             f"Expected GeoDataFrame, received instead: {type(features).__name__}"
         )
+    if "cellsize" not in features:
+        colnames = list(features.columns)
+        raise ValueError(f'Missing column "cellsize" in columns: {colnames}')
+    if len(features) == 0:
+        raise ValueError("Dataframe is empty")
     if not features.index.is_integer():
         raise ValueError(
             f"geodataframe index is not integer typed, received: {features.index.dtype}"
         )
     if features.index.duplicated().any():
         raise ValueError("geodataframe index contains duplicates")
 
@@ -182,16 +211,17 @@
     acceptable = ["Polygon", "LineString", "Point"]
     if not geom_type.isin(acceptable).all():
         raise TypeError(f"Geometry should be one of {acceptable}")
 
     polygons = gdf[geom_type == "Polygon"].copy()
     linestrings = gdf[geom_type == "LineString"].copy()
     points = gdf[geom_type == "Point"].copy()
-    # Set crs to None to avoid crs warnings on joins and overlays
-    polygons.crs = linestrings.crs = points.crs = None
+    for df in (polygons, linestrings, points):
+        df["cellsize"] = df["cellsize"].astype(float)
+        df.crs = None
 
     check_polygons(polygons.geometry)
     check_linestrings(linestrings.geometry, polygons.geometry)
     check_points(points.geometry, polygons.geometry)
 
     return polygons, linestrings, points
```

### Comparing `pandamesh-0.1.1/pandamesh/data/sample_data.py` & `pandamesh-0.1.2/pandamesh/data/sample_data.py`

 * *Files identical despite different names*

### Comparing `pandamesh-0.1.1/pandamesh/gmsh_fields.py` & `pandamesh-0.1.2/pandamesh/gmsh_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pathlib
 import struct
 from typing import List, Tuple, Union
 
-import gmsh
 import numpy as np
 
-from pandamesh.common import FloatArray
+from pandamesh.common import FloatArray, gmsh
 
 
 def write_structured_field_file(
     path: Union[pathlib.Path, str],
     cellsize: FloatArray,
     xmin: float,
     ymin: float,
```

### Comparing `pandamesh-0.1.1/pandamesh/gmsh_geometry.py` & `pandamesh-0.1.2/pandamesh/gmsh_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import List, NamedTuple, Tuple, Union
 
 import geopandas as gpd
-import gmsh
 import numpy as np
 import pandas as pd
 import shapely.geometry as sg
 
-from pandamesh.common import FloatArray, IntArray, coord_dtype, flatten, separate
+from pandamesh.common import FloatArray, IntArray, coord_dtype, flatten, gmsh, separate
 
 Z_DEFAULT = 0.0
 POINT_DIM = 0
 LINE_DIM = 1
 PLANE_DIM = 2
```

### Comparing `pandamesh-0.1.1/pandamesh/gmsh_mesher.py` & `pandamesh-0.1.2/pandamesh/gmsh_mesher.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import pathlib
 import tempfile
 from contextlib import contextmanager
 from enum import Enum, IntEnum
 from typing import List, Tuple, Union
 
 import geopandas as gpd
-import gmsh
 import numpy as np
 import pandas as pd
 
 from pandamesh.common import (
     FloatArray,
     IntArray,
     check_geodataframe,
+    gmsh,
     invalid_option,
     repr,
     separate,
     to_ugrid,
 )
 from pandamesh.gmsh_fields import (
     FIELDS,
```

### Comparing `pandamesh-0.1.1/pandamesh/plot.py` & `pandamesh-0.1.2/pandamesh/plot.py`

 * *Files identical despite different names*

### Comparing `pandamesh-0.1.1/pandamesh/triangle_geometry.py` & `pandamesh-0.1.2/pandamesh/triangle_geometry.py`

 * *Files identical despite different names*

### Comparing `pandamesh-0.1.1/pandamesh/triangle_mesher.py` & `pandamesh-0.1.2/pandamesh/triangle_mesher.py`

 * *Files identical despite different names*

### Comparing `pandamesh-0.1.1/pandamesh.egg-info/PKG-INFO` & `pandamesh-0.1.2/pandamesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandamesh
-Version: 0.1.1
+Version: 0.1.2
 Summary: From geodataframe to mesh
 Maintainer-email: Huite Bootsma <huite.bootsma@deltares.nl>
 License: MIT
 Project-URL: Home, https://github.com/deltares/pandamesh
 Project-URL: Code, https://github.com/deltares/pandamesh
 Project-URL: Issues, https://github.com/deltares/pandamesh/issues
 Keywords: mesh,geopandas,unstructured grid
```

### Comparing `pandamesh-0.1.1/pandamesh.egg-info/SOURCES.txt` & `pandamesh-0.1.2/pandamesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandamesh-0.1.1/pyproject.toml` & `pandamesh-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pandamesh"
 description = "From geodataframe to mesh"
 license = { text = "MIT" }
 readme = { file = "README.rst", content-type = "text/x-rst" }
-version = "0.1.1"
+version = "0.1.2"
 maintainers = [{ name = "Huite Bootsma", email = "huite.bootsma@deltares.nl" }]
 requires-python = ">=3.8"
 dependencies = [
     'geopandas',  
-    'gmsh',
     'pooch',
     'triangle',
     'shapely >= 2.0',
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Science/Research',
```

### Comparing `pandamesh-0.1.1/tests/test_common.py` & `pandamesh-0.1.2/tests/test_common.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,18 +131,26 @@
 
 
 def test_check_geodataframe():
     with pytest.raises(TypeError, match="Expected GeoDataFrame"):
         common.check_geodataframe([1, 2, 3])
 
     gdf = gpd.GeoDataFrame(geometry=[pa, pb])
+    with pytest.raises(ValueError, match='Missing column "cellsize" in columns'):
+        common.check_geodataframe(gdf)
+
+    gdf["cellsize"] = 1.0
     gdf.index = [0, "1"]
     with pytest.raises(ValueError, match="geodataframe index is not integer typed"):
         common.check_geodataframe(gdf)
 
+    empty = gdf.loc[[]]
+    with pytest.raises(ValueError, match="Dataframe is empty"):
+        common.check_geodataframe(empty)
+
     gdf.index = [0, 0]
     with pytest.raises(ValueError, match="geodataframe index contains duplicates"):
         common.check_geodataframe(gdf)
 
     gdf.index = [0, 1]
     common.check_geodataframe(gdf)
 
@@ -219,18 +227,28 @@
     polygons = gpd.GeoSeries(data=[a, b, c, d, e], index=[0, 1, 2, 3, 4])
     with pytest.raises(ValueError, match="1 points detected outside"):
         common.check_points(points, polygons)
 
 
 def test_separate():
     gdf = gpd.GeoDataFrame(geometry=[a, c, d, La, Lc, pa])
+    gdf["cellsize"] = 1.0
     polygons, linestrings, points = common.separate(gdf)
     assert isinstance(polygons.geometry.iloc[0], sg.Polygon)
     assert isinstance(linestrings.geometry.iloc[0], sg.LineString)
     assert isinstance(points.geometry.iloc[0], sg.Point)
 
     # Make sure it works for single elements
     gdf = gpd.GeoDataFrame(geometry=[a])
+    gdf["cellsize"] = 1.0
     common.separate(gdf)
 
     gdf = gpd.GeoDataFrame(geometry=[a, La])
+    gdf["cellsize"] = 1.0
     polygons, linestrings, points = common.separate(gdf)
+
+    # Make sure cellsize is cast to float
+    gdf = gpd.GeoDataFrame(geometry=[a, La])
+    gdf["cellsize"] = "1"
+    dfs = common.separate(gdf)
+    for df in dfs:
+        assert np.issubdtype(df["cellsize"].dtype, np.floating)
```

### Comparing `pandamesh-0.1.1/tests/test_gmsh_geometry.py` & `pandamesh-0.1.2/tests/test_gmsh_geometry.py`

 * *Files identical despite different names*

### Comparing `pandamesh-0.1.1/tests/test_meshers.py` & `pandamesh-0.1.2/tests/test_meshers.py`

 * *Files identical despite different names*

### Comparing `pandamesh-0.1.1/tests/test_plot.py` & `pandamesh-0.1.2/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `pandamesh-0.1.1/tests/test_triangle_geometry.py` & `pandamesh-0.1.2/tests/test_triangle_geometry.py`

 * *Files identical despite different names*

