# Comparing `tmp/optim3d-0.2.9.tar.gz` & `tmp/optim3d-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\optim3d-0.2.9.tar", last modified: Thu Apr 13 14:16:25 2023, max compression
+gzip compressed data, was "dist\optim3d-0.3.0.tar", last modified: Thu Apr 13 15:49:15 2023, max compression
```

## Comparing `optim3d-0.2.9.tar` & `optim3d-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 14:16:25.000000 optim3d-0.2.9/
--rw-rw-rw-   0        0        0     1243 2023-04-06 13:43:27.000000 optim3d-0.2.9/COPYING
--rw-rw-rw-   0        0        0     1613 2023-04-06 13:43:27.000000 optim3d-0.2.9/LICENSE
--rw-rw-rw-   0        0        0       34 2023-04-13 13:09:55.000000 optim3d-0.2.9/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d/
-drwxrwxrwx   0        0        0        0 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d/config/
--rw-rw-rw-   0        0        0    20163 2023-04-06 13:43:27.000000 optim3d-0.2.9/optim3d/config/reconstruct.json
--rw-rw-rw-   0        0        0    43428 2023-04-06 13:43:27.000000 optim3d-0.2.9/optim3d/config/reconstruct_.json
--rw-rw-rw-   0        0        0    21873 2023-04-13 14:15:19.000000 optim3d-0.2.9/optim3d/main.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:09:44.000000 optim3d-0.2.9/optim3d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    14880 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0      335 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14880 2023-04-13 14:16:25.000000 optim3d-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0    13797 2023-04-13 14:15:40.000000 optim3d-0.2.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 14:16:25.000000 optim3d-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      841 2023-04-13 14:16:09.000000 optim3d-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:49:15.000000 optim3d-0.3.0/
+-rw-rw-rw-   0        0        0     1243 2023-04-06 13:43:27.000000 optim3d-0.3.0/COPYING
+-rw-rw-rw-   0        0        0     1613 2023-04-06 13:43:27.000000 optim3d-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-04-13 13:09:55.000000 optim3d-0.3.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-04-13 15:49:15.000000 optim3d-0.3.0/optim3d/
+drwxrwxrwx   0        0        0        0 2023-04-13 15:49:15.000000 optim3d-0.3.0/optim3d/config/
+-rw-rw-rw-   0        0        0    20163 2023-04-06 13:43:27.000000 optim3d-0.3.0/optim3d/config/reconstruct.json
+-rw-rw-rw-   0        0        0    43428 2023-04-06 13:43:27.000000 optim3d-0.3.0/optim3d/config/reconstruct_.json
+-rw-rw-rw-   0        0        0    21855 2023-04-13 15:47:56.000000 optim3d-0.3.0/optim3d/main.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:09:44.000000 optim3d-0.3.0/optim3d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:49:15.000000 optim3d-0.3.0/optim3d.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-13 15:49:15.000000 optim3d-0.3.0/optim3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-13 15:49:15.000000 optim3d-0.3.0/optim3d.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0    14880 2023-04-13 15:49:15.000000 optim3d-0.3.0/optim3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-04-13 15:49:15.000000 optim3d-0.3.0/optim3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      335 2023-04-13 15:49:15.000000 optim3d-0.3.0/optim3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 15:49:15.000000 optim3d-0.3.0/optim3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14880 2023-04-13 15:49:15.000000 optim3d-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13797 2023-04-13 14:15:40.000000 optim3d-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 15:49:15.000000 optim3d-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      841 2023-04-13 15:48:54.000000 optim3d-0.3.0/setup.py
```

### Comparing `optim3d-0.2.9/COPYING` & `optim3d-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.9/LICENSE` & `optim3d-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.9/optim3d/config/reconstruct.json` & `optim3d-0.3.0/optim3d/config/reconstruct.json`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.9/optim3d/config/reconstruct_.json` & `optim3d-0.3.0/optim3d/config/reconstruct_.json`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.9/optim3d/main.py` & `optim3d-0.3.0/optim3d/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,15 @@
 
 @click.group(cls=OrderedGroup, help="CLI tool to manage full optimized reconstruction of large-scale 3D building models.")
 def cli():
     pass
 
 @click.command()
 @click.argument('footprints', type=click.Path(exists=True), required=False)
-@click.option('--output', help='Output directory.', type=click.Path(exists=False), default="./output", show_default=True)
+@click.option('--output', help='Output directory.', type=click.Path(exists=False), default="output", show_default=True)
 @click.option('--osm', help='Download and work with building footprints from OpenStreetMap [west, north, est, south].', nargs=4, type=click.Tuple([float, float, float, float]), default=(-1, -1, -1, -1))
 @click.option('--crs', help='Specify the Coordinate Reference System (EPSG).', type=click.INT)
 @click.option('--max', help='Maximum number of buildings per tile.', type=click.INT, default=3500, show_default=True)
 
 def index2d(footprints, output, osm, crs, max):
     '''
     QuadTree indexing and tiling of 2D building footprints.
@@ -403,15 +403,15 @@
     processTime = end - start
 
     print("All tiles generated successfully")
     click.echo("Time: {}".format(time.strftime("%H:%M:%S", time.gmtime(processTime))))
 
 @click.command()
 @click.argument('pointcloud', type=click.Path(exists=True), required=True)
-@click.option('--output', help='Output directory.', type=click.Path(exists=False), default="./output", show_default=True)
+@click.option('--output', help='Output directory.', type=click.Path(exists=False), default="output", show_default=True)
 
 def index3d(pointcloud, output):
     '''
     OcTree indexing of 3D point cloud using Entwine.
     '''
 
     if (os.path.exists(output)==False):
@@ -427,17 +427,17 @@
     config_file = os.path.join(tmp, "config.json")
     with open(config_file, "w") as f:
         json.dump(config, f, indent=2)
 
     os.system('entwine build -c {}'.format(config_file))
 
 @click.command()
-@click.option('--areas', help='The calculated processing areas.', type=click.Path(exists=True), default="./output/processing_areas.gpkg", show_default=True)
-@click.option('--indexed', help='Indexed 3D point cloud directory.', type=click.Path(exists=True), default="./output/indexed_pointcloud", show_default=True)
-@click.option('--output', help='Output directory.', type=click.Path(exists=False), default="./output", show_default=True)
+@click.option('--areas', help='The calculated processing areas.', type=click.Path(exists=True), default="output/processing_areas.gpkg", show_default=True)
+@click.option('--indexed', help='Indexed 3D point cloud directory.', type=click.Path(exists=True), default="output/indexed_pointcloud", show_default=True)
+@click.option('--output', help='Output directory.', type=click.Path(exists=False), default="output", show_default=True)
 
 def tiler3d(areas, indexed, output):
     '''
     Tiling of point cloud using the calculated processing areas.
     '''
     start = time.time()
 
@@ -459,17 +459,17 @@
     end = time.time()
     processTime = end - start
 
     print('All tiles generated successfully')
     click.echo("Time: {}".format(time.strftime("%H:%M:%S", time.gmtime(processTime))))
 
 @click.command()
-@click.option('--pointcloud', help='3D point cloud tiles directory.', type=click.Path(exists=True), default="./output/pointcloud_tiles", show_default=True)
-@click.option('--footprints', help='2D building footprints tiles directory.', type=click.Path(exists=True), default="./output/footprint_tiles", show_default=True)
-@click.option('--output', help='Output directory.', type=click.Path(exists=False), default="./output", show_default=True)
+@click.option('--pointcloud', help='3D point cloud tiles directory.', type=click.Path(exists=True), default="output/pointcloud_tiles", show_default=True)
+@click.option('--footprints', help='2D building footprints tiles directory.', type=click.Path(exists=True), default="output/footprint_tiles", show_default=True)
+@click.option('--output', help='Output directory.', type=click.Path(exists=False), default="output", show_default=True)
 
 def reconstruct(footprints, pointcloud, output):
     '''
     Optimized 3D reconstruction of buildings using GeoFlow.
     '''
 
     start = time.time()
@@ -535,15 +535,15 @@
     end = time.time()
     processTime = end - start
 
     print("All buildings reconstructed successfully")
     click.echo("Time: {}".format(time.strftime("%H:%M:%S", time.gmtime(processTime))))
 
 @click.command()
-@click.option('--cityjson', help='CityJSON files directory.', type=click.Path(exists=True), default="./output/model/cityjson", show_default=True)
+@click.option('--cityjson', help='CityJSON files directory.', type=click.Path(exists=True), default="output/model/cityjson", show_default=True)
 
 def post(cityjson):
     '''
     Postprocess the generated CityJSON files.
     '''
     start = time.time()
```

### Comparing `optim3d-0.2.9/optim3d.egg-info/PKG-INFO` & `optim3d-0.3.0/optim3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim3d
-Version: 0.2.9
+Version: 0.3.0
 Summary: CLI application for efficient and optimized reconstruction of large-scale 3D building models.
 Home-page: https://github.com/Yarroudh/Optim3D
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause BSD 3-Clause "New" or "Revised" License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `optim3d-0.2.9/PKG-INFO` & `optim3d-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim3d
-Version: 0.2.9
+Version: 0.3.0
 Summary: CLI application for efficient and optimized reconstruction of large-scale 3D building models.
 Home-page: https://github.com/Yarroudh/Optim3D
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause BSD 3-Clause "New" or "Revised" License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `optim3d-0.2.9/README.md` & `optim3d-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.9/setup.py` & `optim3d-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="optim3d",
-    version='0.2.9',
+    version='0.3.0',
     description="CLI application for efficient and optimized reconstruction of large-scale 3D building models.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='BSD 3-Clause BSD 3-Clause "New" or "Revised" License',
     author = 'Anass Yarroudh',
     author_email = 'ayarroudh@uliege.be',
     url = 'https://github.com/Yarroudh/Optim3D',
```

