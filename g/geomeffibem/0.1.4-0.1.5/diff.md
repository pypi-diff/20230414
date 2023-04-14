# Comparing `tmp/geomeffibem-0.1.4.tar.gz` & `tmp/geomeffibem-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomeffibem-0.1.4.tar", max compression
+gzip compressed data, was "geomeffibem-0.1.5.tar", max compression
```

## Comparing `geomeffibem-0.1.4.tar` & `geomeffibem-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1071 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/LICENSE
--rw-r--r--   0        0        0     1648 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/README.md
--rw-r--r--   0        0        0      539 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/geomeffibem/__init__.py
--rw-r--r--   0        0        0     2396 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/geomeffibem/boundingbox.py
--rw-r--r--   0        0        0     1517 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/geomeffibem/plane.py
--rw-r--r--   0        0        0     7651 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/geomeffibem/polyhedron.py
--rw-r--r--   0        0        0    16566 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/geomeffibem/surface.py
--rw-r--r--   0        0        0     6865 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/geomeffibem/transformation.py
--rw-r--r--   0        0        0     8034 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/geomeffibem/vertex.py
--rw-r--r--   0        0        0     3134 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       41 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      543 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/tests/test_geomeffibem.py
--rw-r--r--   0        0        0     1005 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/tests/test_plane.py
--rw-r--r--   0        0        0     4177 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/tests/test_polyhedron.py
--rw-r--r--   0        0        0     8788 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/tests/test_surface.py
--rw-r--r--   0        0        0     3100 2023-01-03 09:24:21.782988 geomeffibem-0.1.4/tests/test_vertex.py
--rw-r--r--   0        0        0     3331 1970-01-01 00:00:00.000000 geomeffibem-0.1.4/setup.py
--rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 geomeffibem-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-14 09:07:35.168235 geomeffibem-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1648 2023-04-14 09:07:35.168235 geomeffibem-0.1.5/README.md
+-rw-r--r--   0        0        0      587 2023-04-14 09:07:35.168235 geomeffibem-0.1.5/geomeffibem/__init__.py
+-rw-r--r--   0        0        0     2748 2023-04-14 09:07:35.168235 geomeffibem-0.1.5/geomeffibem/boundingbox.py
+-rw-r--r--   0        0        0     1562 2023-04-14 09:07:35.168235 geomeffibem-0.1.5/geomeffibem/plane.py
+-rw-r--r--   0        0        0     8186 2023-04-14 09:07:35.168235 geomeffibem-0.1.5/geomeffibem/polyhedron.py
+-rw-r--r--   0        0        0    18823 2023-04-14 09:07:35.172235 geomeffibem-0.1.5/geomeffibem/surface.py
+-rw-r--r--   0        0        0     6997 2023-04-14 09:07:35.172235 geomeffibem-0.1.5/geomeffibem/transformation.py
+-rw-r--r--   0        0        0     8034 2023-04-14 09:07:35.172235 geomeffibem-0.1.5/geomeffibem/vertex.py
+-rw-r--r--   0        0        0     3088 2023-04-14 09:07:35.172235 geomeffibem-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-04-14 09:07:35.172235 geomeffibem-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      543 2023-04-14 09:07:35.172235 geomeffibem-0.1.5/tests/test_geomeffibem.py
+-rw-r--r--   0        0        0      986 2023-04-14 09:07:35.172235 geomeffibem-0.1.5/tests/test_plane.py
+-rw-r--r--   0        0        0     4158 2023-04-14 09:07:35.172235 geomeffibem-0.1.5/tests/test_polyhedron.py
+-rw-r--r--   0        0        0     8750 2023-04-14 09:07:35.172235 geomeffibem-0.1.5/tests/test_surface.py
+-rw-r--r--   0        0        0     3100 2023-04-14 09:07:35.172235 geomeffibem-0.1.5/tests/test_vertex.py
+-rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 geomeffibem-0.1.5/PKG-INFO
```

### Comparing `geomeffibem-0.1.4/LICENSE` & `geomeffibem-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `geomeffibem-0.1.4/README.md` & `geomeffibem-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `geomeffibem-0.1.4/geomeffibem/__init__.py` & `geomeffibem-0.1.5/geomeffibem/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Top-level package for GeomEffiBEM."""
 
 __author__ = """Julien Marrec"""
 __email__ = 'contact@effibem.com'
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
+from geomeffibem.boundingbox import BoundingBox
 from geomeffibem.plane import Plane
 from geomeffibem.polyhedron import Polyhedron
 from geomeffibem.surface import Surface, Surface3dEge, plot_vertices
 from geomeffibem.transformation import Transformation
 from geomeffibem.vertex import (
     Vertex,
     distance,
```

### Comparing `geomeffibem-0.1.4/geomeffibem/boundingbox.py` & `geomeffibem-0.1.5/geomeffibem/boundingbox.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Bounding Box."""
 
-from typing import Tuple
+from typing import Optional, Tuple
 
 import numpy as np
 
 from geomeffibem.vertex import Vertex
 
 
 class BoundingBox:
@@ -23,15 +23,15 @@
         self.maxZ = None
 
     def get_figsize(self, width=12) -> Tuple[float, float]:
         """Figure out a figure size (Broken)."""
         (x, y, z) = self.dimensions().to_numpy()
         return (width, width * x / y)
 
-    def corners(self) -> np.ndarray:
+    def corners(self) -> Optional[np.ndarray]:
         """Returns an  of all 8 corner Points."""
         # TODO: make it return Vertex?
         if self.isEmpty():
             return None
         return np.array(
             [
                 [self.minX, self.minY, self.minZ],
@@ -41,14 +41,21 @@
                 [self.minX, self.minY, self.maxZ],
                 [self.maxX, self.minY, self.maxZ],
                 [self.minX, self.maxY, self.maxZ],
                 [self.maxX, self.maxY, self.maxZ],
             ]
         )
 
+    def centerPoint(self) -> Vertex:
+        """Get center of the bounding box, as the midpoint of the min/max coordinates."""
+        if self.minX is None:
+            raise ValueError("You need to add some points")
+
+        return Vertex(x=(self.minX + self.maxX) / 2.0, y=(self.minY + self.maxY) / 2.0, z=(self.minZ + self.maxZ) / 2.0)
+
     def isEmpty(self) -> bool:
         """Checks if the bounding box is initialized."""
         return self.minX is None
 
     def addPoint(self, vertex) -> None:
         """Adds a single point and updates the min/max x, y, z."""
         if self.isEmpty():
@@ -59,18 +66,18 @@
             self.maxY = vertex.y
             self.maxZ = vertex.z
         else:
             self.minX = min(self.minX, vertex.x)
             self.minY = min(self.minY, vertex.y)
             self.minZ = min(self.minZ, vertex.z)
 
-            self.maxX = max(self.minX, vertex.x)
+            self.maxX = max(self.maxX, vertex.x)
             self.maxY = max(self.maxY, vertex.y)
             self.maxZ = max(self.maxZ, vertex.z)
 
-    def addPoints(self, vertices) -> None:
+    def addPoints(self, vertices):
         """Adds multiple points and updates the min/max x, y, z."""
         [self.addPoint(v) for v in vertices]
 
     def dimensions(self) -> Vertex:
         """Returns the dimensions of the bounding box."""
         return Vertex(self.maxX - self.minX, self.maxY - self.minY, self.maxZ - self.minZ)
```

### Comparing `geomeffibem-0.1.4/geomeffibem/plane.py` & `geomeffibem-0.1.5/geomeffibem/plane.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 
 import numpy as np
 
 from geomeffibem.vertex import Vertex, distance
 
 
 class Plane:
-    """A 3D Plane."""
+    """A 3D Plane.
+
+    Equation is `ax + by + cz + d = 0`
+    """
 
     def __init__(self, a, b, c, d):
         """Plane constructor."""
         self.a = a
         self.b = b
         self.c = c
         self.d = d
```

### Comparing `geomeffibem-0.1.4/geomeffibem/polyhedron.py` & `geomeffibem-0.1.5/geomeffibem/polyhedron.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import copy
 from typing import List, Tuple
 
 import numpy as np
 
 from geomeffibem.surface import Surface, Surface3dEge
-from geomeffibem.vertex import Vertex
+from geomeffibem.vertex import Vertex, getNewellVector
 
 
 class Polyhedron:
     """A collection of Surfaces, meant to represent a Volume."""
 
     def __init__(self, surfaces: List[Surface]):
         """Constructor from a list of Surface objects."""
@@ -112,14 +112,27 @@
         updatedZonePoly = self.updateZonePolygonsForMissingColinearPoints()
         edgeNot2again, _ = Polyhedron.edgesNotTwoForEnclosedVolumeTest(updatedZonePoly)
         if not edgeNot2again:
             return True, []
 
         return False, edgesInBoth(edgeNot2orig, edgeNot2again)
 
+    def calcPolyhedronVolume(self) -> float:
+        """Calculates the Volume of an ENCLOSED Polyhedron."""
+        volume = 0.0
+        for surface in self.surfaces:
+            vertices = surface.vertices
+            p3FaceOrigin = vertices[1] - Vertex(0, 0, 0)
+            newellAreaVector = getNewellVector(vertices)
+            pyramidVolume = newellAreaVector.dot(p3FaceOrigin)
+            volume += pyramidVolume
+        # Our newellArea vector has twice the length
+        volume /= 6.0
+        return volume
+
     def to_os_cpp_code(self):
         """For my own convenience when writting OpenStudio tests."""
         for i, sf in enumerate(self.surfaces):
             if sf.name is not None:
                 name = sf.name
             else:
                 name = f"Surface {i+1}"
```

### Comparing `geomeffibem-0.1.4/geomeffibem/surface.py` & `geomeffibem-0.1.5/geomeffibem/surface.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,28 +107,85 @@
             raise ValueError("Expected an openstudio.model.Surface")
         return Surface(
             vertices=[Vertex.from_Point3d(x) for x in openstudio_surface.vertices()],
             name=openstudio_surface.nameString(),
         )
 
     @staticmethod
-    def Rectangle(min_x=0.0, max_x=10.0, min_y=0.0, max_y=10.0, min_z=0.0, max_z=0.0) -> Surface:
-        """Factory method to easily create an rectangle Surface."""
+    def Floor(min_x=0.0, max_x=10.0, min_y=0.0, max_y=10.0, z=0.0) -> Surface:
+        """Create a rectangular floor Surface (outward normal pointing down)."""
+        # Counterclockwise, ULC convention, except here we want to create a floor so
+        # outward normal must be pointing DOWN, so clockwise order
         vertices_arr = np.array(
             [
-                [min_x, min_y, max_z],
-                [min_x, max_y, min_z],
-                [max_x, max_y, min_z],
-                [max_x, min_y, max_z],
+                [max_x, max_y, z],
+                [max_x, min_y, z],
+                [min_x, min_y, z],
+                [min_x, max_y, z],
             ]
         )
         vertices = [Vertex.from_numpy(x) for x in vertices_arr]
 
         return Surface(vertices=vertices)
 
+    @staticmethod
+    def Rectangle(min_x=0.0, max_x=10.0, min_y=0.0, max_y=10.0, min_z=0.0, max_z=0.0) -> Surface:
+        """Factory method to easily create a rectangular Surface, with ULC convention."""
+        if abs(max_z - min_z) < 0.01:
+            z = min_z
+            if abs(z) < 0.01:
+                print(
+                    "Looks like you're trying to create a Floor surface... "
+                    "use the Surface.Floor factory method if that's the case so outwardNormal points down."
+                )
+
+            vertices_arr = np.array(
+                [
+                    [min_x, max_y, z],  # Upper Left Corner
+                    [min_x, min_y, z],  # Lower Left Corner
+                    [max_x, min_y, z],  # Lower Right Corner
+                    [max_x, max_y, z],  # Upper Right Corner
+                ]
+            )
+        elif abs(max_x - min_x) < 0.01:
+            x = min_x
+            vertices_arr = np.array(
+                [
+                    [x, min_y, max_z],  # Upper Left Corner
+                    [x, min_y, min_z],  # Lower Left Corner
+                    [x, max_y, min_z],  # Lower Right Corner
+                    [x, max_y, max_z],  # Upper Right Corner
+                ]
+            )
+
+        elif abs(max_y - max_y) < 0.01:
+            y = min_y
+            vertices_arr = np.array(
+                [
+                    [min_x, y, max_z],  # Upper Left Corner
+                    [min_x, y, min_z],  # Lower Left Corner
+                    [max_x, y, min_z],  # Lower Right Corne
+                    [max_x, y, max_z],  # Upper Right Corner
+                ]
+            )
+        else:
+            print("We expected at least one of x, y, z to be fixed, results are not guaranteed to work")
+            vertices_arr = np.array(
+                [
+                    [min_x, min_y, max_z],
+                    [min_x, max_y, min_z],
+                    [max_x, max_y, min_z],
+                    [max_x, min_y, max_z],
+                ]
+            )
+
+        vertices = [Vertex.from_numpy(x) for x in vertices_arr]
+
+        return Surface(vertices=vertices)
+
     def __init__(self, vertices, name=None):
         """Surface constructor."""
         if not isinstance(vertices, np.ndarray) and not isinstance(vertices, list):
             raise ValueError("Expected a list or numpy array of Vertex")
 
         for i, vertex in enumerate(vertices):
             if not isinstance(vertex, Vertex):
@@ -169,15 +226,15 @@
     def plane(self) -> Plane:
         """Compute the plane from outwardNormal and the first point, not using OpenStudio."""
         normalVector = self.outwardNormal()
         if not np.isclose(normalVector.length(), 1.0):
             raise ValueError("Normal Unit Vector doesn't appear to be a unit vector")
         self.vertices[0]
 
-        # d = -thisNormal.x() * point.x() - thisNormal.y() * point.y() - thisNormal.z() * point.z();
+        # d = -normalVector.x() * point.x() - normalVector.y() * point.y() - normalVector.z() * point.z();
         d = (-normalVector).dot(self.vertices[0])
 
         p = Plane(normalVector.x, normalVector.y, normalVector.z, d)
         for i, v in enumerate(self.vertices):
             if not p.pointOnPlane(v):
                 print(f"Vertex {i} is not on the plane")
         return p
```

### Comparing `geomeffibem-0.1.4/geomeffibem/transformation.py` & `geomeffibem-0.1.5/geomeffibem/transformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,18 @@
 
         # check if face normal is up or down
         if abs(zp.dot(zAxis)) < 0.99:
             # not facing up or down, set yPrime along zAxis
             yp = zAxis - (zp * zp.dot(zAxis))
             yp = yp.normalize()
             xp = yp.cross(zp)
+            print("Not facing up or down, set yPrime along zAxis")
         else:
             # facing up or down, set xPrime along -xAxis
+            print("Facing up or down, set xPrime along -xAxis")
             xp = negXAxis - (zp * zp.dot(negXAxis))
             xp = xp.normalize()
             yp = zp.cross(xp)
 
         storage = np.identity(4)
         storage[0, 0] = xp.x
         storage[1, 0] = xp.y
@@ -129,15 +131,15 @@
         return self.matrix[:-1, :-1]
 
     def translation(self) -> Vertex:
         """Returns the translation portion of the Transformation."""
         return Vertex(self.matrix[0, 3], self.matrix[1, 3], self.matrix[2, 3])
 
     def inverse(self) -> Transformation:
-        """Returns a transformation which is the inverse of this"""
+        """Returns a transformation which is the inverse of this."""
         t = Transformation()
         t.matrix = np.linalg.inv(self.matrix)
         return t
 
     def __mul__(self, other):  # -> Union[Vertex, Transformation, np.ndarray, Surface, Plane]:
         """Multiplies self by other.
```

### Comparing `geomeffibem-0.1.4/geomeffibem/vertex.py` & `geomeffibem-0.1.5/geomeffibem/vertex.py`

 * *Files identical despite different names*

### Comparing `geomeffibem-0.1.4/pyproject.toml` & `geomeffibem-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "geomeffibem"
-version = "0.1.4"
+version = "0.1.5"
 homepage = "https://github.com/jmarrec/geomeffibem"
 description = "A small library to facilitate some building energy modeling geometry operations with OpenStudio and EnergyPlus in mind."
 authors = ["Julien Marrec <contact@effibem.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -34,15 +34,14 @@
 flake8  = {version = "^4.0.1", optional = true}
 flake8-docstrings = {version = "^1.6.0", optional = true}
 mypy = {version = "^0.960", optional = true}
 pytest  = {version = "^7.1.2", optional = true}
 pytest-cov  = {version = "^3.0.0", optional = true}
 tox  = {version = "^3.25.0", optional = true}
 virtualenv  = {version = "^20.14.1", optional = true}
-pip  = {version = "^22.1.1", optional = true}
 mkdocs  = {version = "^1.3.0", optional = true}
 mkdocs-include-markdown-plugin  = {version = "^3.5.1", optional = true}
 mkdocs-material  = {version = "^8.2.16", optional = true}
 mkdocstrings  = {version = "^0.19.0", optional = true}
 mkdocstrings-python = {version = "^0.7.0", optional = true}
 mkdocs-material-extensions  = {version = "^1.0.3", optional = true}
 twine  = {version = "^4.0.0", optional = true}
```

### Comparing `geomeffibem-0.1.4/tests/test_geomeffibem.py` & `geomeffibem-0.1.5/tests/test_geomeffibem.py`

 * *Files identical despite different names*

### Comparing `geomeffibem-0.1.4/tests/test_polyhedron.py` & `geomeffibem-0.1.5/tests/test_polyhedron.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from geomeffibem.polyhedron import Polyhedron, edgesInBoth
 from geomeffibem.surface import Surface
 
 
 @pytest.fixture
 def zonePoly():
     """A fixture to create a Zone Polyhedron."""
-    floor_surface = Surface.Rectangle(min_x=0.0, max_x=10.0, min_y=0.0, max_y=10.0, min_z=0.0, max_z=0.0)
+    floor_surface = Surface.Floor(min_x=0.0, max_x=10.0, min_y=0.0, max_y=10.0, z=0.0)
     m = openstudio.model.Model()
     space = openstudio.model.Space.fromFloorPrint(floor_surface.to_Point3dVector(), 3.0, m).get()
     for sf in space.surfaces():
         if sf.surfaceType() == 'Floor':
             sf.setName("FLOOR")
         elif sf.surfaceType() == 'RoofCeiling':
             sf.setName("ROOF")
```

### Comparing `geomeffibem-0.1.4/tests/test_surface.py` & `geomeffibem-0.1.5/tests/test_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 
 from geomeffibem.surface import Surface, Surface3dEge, get_surface_from_surface_like, plot_vertices
 from geomeffibem.vertex import Vertex
 
 
 def test_surface_rectangle():
     """Tests Surface.Rectangle factory."""
-    surface = Surface.Rectangle(min_x=0.0, max_x=10.0, min_y=0.0, max_y=10.0, min_z=0.0, max_z=0.0)
+    z = 0.0
+    surface = Surface.Rectangle(min_x=0.0, max_x=10.0, min_y=0.0, max_y=10.0, min_z=z, max_z=z)
     assert np.array_equal(
         surface.to_numpy(),
         np.array(
             [
-                [0.0, 0.0, 0.0],
-                [0.0, 10.0, 0.0],
-                [10.0, 10.0, 0.0],
-                [10.0, 0.0, 0.0],
+                [0.0, 10.0, z],
+                [0.0, 0.0, z],
+                [10.0, 0.0, z],
+                [10.0, 10.0, z],
             ]
         ),
     )
     assert surface.get_plot_axis() == 'xy'
 
     surface = Surface.Rectangle(min_x=0.0, max_x=10.0, min_y=5.0, max_y=5.0, min_z=10.0, max_z=20.0)
     assert np.array_equal(
@@ -133,42 +134,42 @@
     surface = Surface.Rectangle(min_x=0.0, max_x=0.0, min_y=0.0, max_y=0.0, min_z=0.0, max_z=0.0)
     with pytest.raises(ValueError):
         surface.os_centroid()
 
 
 def test_Surface_split():
     """Test splitting a surface."""
-    surface = Surface.Rectangle(min_x=0.0, max_x=10.0, min_y=0.0, max_y=10.0, min_z=0.0, max_z=0.0)
+    surface = Surface.Floor(min_x=0.0, max_x=10.0, min_y=0.0, max_y=10.0, z=0.0)
     surface.name = "Surface"
     surface.os_centroid() == Vertex(+5.0000, +5.0000, +0.0000)
 
     s1, s2 = surface.split_into_n_segments(n_segments=2, axis=None, plot=False)
     assert s1.name == "Surface-1"
     assert np.array_equal(
-        s1.to_numpy(), np.array([[0.0, 0.0, 0.0], [0.0, 10.0, 0.0], [5.0, 10.0, 0.0], [5.0, 0.0, 0.0]])
+        s1.to_numpy(), np.array([[5.0, 10.0, 0.0], [5.0, 0.0, 0.0], [0.0, 0.0, 0.0], [0.0, 10.0, 0.0]])
     )
 
     assert s2.name == "Surface-2"
     assert np.array_equal(
-        s2.to_numpy(), np.array([[5.0, 0.0, 0.0], [5.0, 10.0, 0.0], [10.0, 10.0, 0.0], [10.0, 0.0, 0.0]])
+        s2.to_numpy(), np.array([[10.0, 10.0, 0.0], [10.0, 0.0, 0.0], [5.0, 0.0, 0.0], [5.0, 10.0, 0.0]])
     )
 
     with pytest.raises(ValueError):
         surface.split_into_n_segments(n_segments=2, axis='z', plot=False)
 
     surface.name = None
     s1, s2 = surface.split_into_n_segments(n_segments=2, axis='y', plot=False)
     assert s1.name is None
     assert np.array_equal(
-        s1.to_numpy(), np.array([[0.0, 0.0, 0.0], [0.0, 5.0, 0.0], [10.0, 5.0, 0.0], [10.0, 0.0, 0.0]])
+        s1.to_numpy(), np.array([[10.0, 5.0, 0.0], [10.0, 0.0, 0.0], [0.0, 0.0, 0.0], [0.0, 5.0, 0.0]])
     )
 
     assert s2.name is None
     assert np.array_equal(
-        s2.to_numpy(), np.array([[0.0, 5.0, 0.0], [0.0, 10.0, 0.0], [10.0, 10.0, 0.0], [10.0, 5.0, 0.0]])
+        s2.to_numpy(), np.array([[10.0, 10.0, 0.0], [10.0, 5.0, 0.0], [0.0, 5.0, 0.0], [0.0, 10.0, 0.0]])
     )
 
     with pytest.raises(ValueError):
         surface.split_into_n_segments(n_segments=1, axis='x', plot=False)
 
 
 def test_split_plot():
@@ -176,29 +177,29 @@
     surface = Surface.Rectangle(min_x=0.0, max_x=10.0, min_y=0.0, max_y=10.0, min_z=0.0, max_z=0.0)
     surface.name = "Surface"
     surface.split_into_n_segments(n_segments=2, axis='y', plot=True)
 
 
 def test_Surface_rotate():
     """Test rotate."""
-    surface = Surface.Rectangle(min_x=0.0, max_x=10.0, min_y=0.0, max_y=10.0, min_z=0.0, max_z=0.0)
+    surface = Surface.Floor(min_x=0.0, max_x=10.0, min_y=0.0, max_y=10.0, z=0.0)
 
     surface_rot = surface.rotate(degrees=-25.0)
     assert np.isclose(surface.os_area(), surface_rot.os_area())
 
     surface_rot = surface.rotate(degrees=-90.0)
 
     assert np.allclose(
         surface_rot.to_numpy(),
         np.array(
             [
-                [+0.0, +0.0, +0.0],
-                [-10.0, +0.0, +0.0],
                 [-10.0, +10.0, +0.0],
                 [+0.0, +10.0, +0.0],
+                [+0.0, +0.0, +0.0],
+                [-10.0, +0.0, +0.0],
             ]
         ),
     )
 
 
 def test_surface_plot():
     """Test plotting."""
```

### Comparing `geomeffibem-0.1.4/tests/test_vertex.py` & `geomeffibem-0.1.5/tests/test_vertex.py`

 * *Files identical despite different names*

### Comparing `geomeffibem-0.1.4/PKG-INFO` & `geomeffibem-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomeffibem
-Version: 0.1.4
+Version: 0.1.5
 Summary: A small library to facilitate some building energy modeling geometry operations with OpenStudio and EnergyPlus in mind.
 Home-page: https://github.com/jmarrec/geomeffibem
 License: MIT
 Author: Julien Marrec
 Author-email: contact@effibem.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -35,15 +35,14 @@
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0)
 Requires-Dist: mkdocstrings (>=0.19.0,<0.20.0) ; extra == "doc"
 Requires-Dist: mkdocstrings-python (>=0.7.0,<0.8.0) ; extra == "doc"
 Requires-Dist: mypy (>=0.960,<0.961) ; extra == "test"
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: openstudio (>=3.4.0,<4.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
-Requires-Dist: pip (>=22.1.1,<23.0.0) ; extra == "dev"
 Requires-Dist: pre-commit (>=2.19.0,<3.0.0) ; extra == "dev"
 Requires-Dist: pytest (>=7.1.2,<8.0.0) ; extra == "test"
 Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "test"
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
 Requires-Dist: tox (>=3.25.0,<4.0.0) ; extra == "dev"
 Requires-Dist: twine (>=4.0.0,<5.0.0) ; extra == "dev"
 Requires-Dist: virtualenv (>=20.14.1,<21.0.0) ; extra == "dev"
```

