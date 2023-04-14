# Comparing `tmp/pyroscopegridding-0.0.3.tar.gz` & `tmp/pyroscopegridding-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroscopegridding-0.0.3.tar", last modified: Fri Apr 14 15:22:35 2023, max compression
+gzip compressed data, was "dist/pyroscopegridding-0.0.8.tar", last modified: Fri Apr 14 16:07:51 2023, max compression
```

## Comparing `pyroscopegridding-0.0.3.tar` & `pyroscopegridding-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 15:22:35.099973 pyroscopegridding-0.0.3/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-14 15:22:35.092828 pyroscopegridding-0.0.3/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.0.3/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 15:22:34.840959 pyroscopegridding-0.0.3/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2022-02-04 10:40:28.000000 pyroscopegridding-0.0.3/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     2636 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.3/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10387 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.3/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33637 2023-04-14 14:32:01.000000 pyroscopegridding-0.0.3/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10462 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.3/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26242 2023-04-14 15:03:08.000000 pyroscopegridding-0.0.3/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9309 2023-04-14 14:25:01.000000 pyroscopegridding-0.0.3/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.3/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10932 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.3/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     4779 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.3/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 15:22:35.046656 pyroscopegridding-0.0.3/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-14 15:22:34.000000 pyroscopegridding-0.0.3/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-14 15:22:34.000000 pyroscopegridding-0.0.3/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-14 15:22:34.000000 pyroscopegridding-0.0.3/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-14 15:22:34.000000 pyroscopegridding-0.0.3/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-14 15:22:34.000000 pyroscopegridding-0.0.3/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-14 15:22:34.000000 pyroscopegridding-0.0.3/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-14 15:22:35.105749 pyroscopegridding-0.0.3/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1762 2023-04-14 15:22:19.000000 pyroscopegridding-0.0.3/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 16:07:51.449628 pyroscopegridding-0.0.8/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-14 16:07:51.446629 pyroscopegridding-0.0.8/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.0.8/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 16:07:51.300626 pyroscopegridding-0.0.8/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-04-14 15:47:03.000000 pyroscopegridding-0.0.8/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     2637 2023-04-14 15:49:58.000000 pyroscopegridding-0.0.8/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10388 2023-04-14 15:50:51.000000 pyroscopegridding-0.0.8/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33643 2023-04-14 16:03:37.000000 pyroscopegridding-0.0.8/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10464 2023-04-14 16:03:48.000000 pyroscopegridding-0.0.8/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26242 2023-04-14 16:07:35.000000 pyroscopegridding-0.0.8/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9309 2023-04-14 14:25:01.000000 pyroscopegridding-0.0.8/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.8/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10938 2023-04-14 16:04:35.000000 pyroscopegridding-0.0.8/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     4779 2023-04-14 16:04:41.000000 pyroscopegridding-0.0.8/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 16:07:51.418630 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-14 16:07:50.000000 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-14 16:07:50.000000 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-14 16:07:50.000000 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       69 2023-04-14 16:07:50.000000 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-14 16:07:50.000000 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-14 16:07:50.000000 pyroscopegridding-0.0.8/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-14 16:07:51.450628 pyroscopegridding-0.0.8/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1764 2023-04-14 16:07:42.000000 pyroscopegridding-0.0.8/setup.py
```

### Comparing `pyroscopegridding-0.0.3/PKG-INFO` & `pyroscopegridding-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.0.3
+Version: 0.0.8
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.0.3/README.md` & `pyroscopegridding-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.3/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.0.8/pyroscopegridding/fileparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 __status__ = "Production"
 # FileParser
 #
 # Aids in parsing file names and paths
 # Controls directory read in
 #
 
-import time_conv
+#import time_conv
 import yaml
 import os
 from os import walk
 
 # given path to text file contaings paths to files to read read out as list of files within
 def read_file_sat_data(fileloc):
     lines = []
```

### Comparing `pyroscopegridding-0.0.3/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.0.8/pyroscopegridding/filter_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # 
 # Luckily, the metadata and attributes of the netcdf4 variables gives us an idea of what we should be looking for through:
 # 
 # 1. valid_range
 # 2. units
 # 3. scale_factor
 
-import sat_data_input
+#import sat_data_input
 import numpy as np
 
 # nc
 # given GeoID,PhyID (this is read in with open_file) and their corresponding var_lists (variables we care about)
 # output lat, lon, and variables we care about (filtered based on metadata)
 # lat lon are n size arrays containing lat, long variables for variable n
 # phy_vars is n size array containing netcdf4.variables
```

### Comparing `pyroscopegridding-0.0.3/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.0.8/pyroscopegridding/grid_ncf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 
 from http.client import MOVED_PERMANENTLY
 import netCDF4
 import numpy as np
 import numpy.ma as ma
 import time
 
-import gridding
-import sat_data_input
-import filter_data
-import naming_conventions
-import solar_zenith
-import datetime
+#import gridding
+#import sat_data_input
+#import filter_data
+#import naming_conventions
+#import solar_zenith
+#import datetime
 
 # full satellite list 
 # used to check if any satellites are missing
 #full_satellite_list = ['AERDT_L2_ABI_G16', 'AERDT_L2_ABI_G17', 'AERDT_L2_AHI_H08', 'AERDT_L2_VIIRS_SNPP', 'MOD04_L2', 'MYD04_L2']
 full_satellite_list = ['ABI_G16', 'ABI_G17', 'AHI_H08', 'VIIRS_SNPP', 'MOD04', 'MYD04']
```

### Comparing `pyroscopegridding-0.0.3/pyroscopegridding/gridding.py` & `pyroscopegridding-0.0.8/pyroscopegridding/gridding.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 # - https://oceancolor.gsfc.nasa.gov/docs/format/l2nc/
 # - https://oceancolor.gsfc.nasa.gov/docs/format/l2nc_viirs/
 
 import numpy as np
 import numpy.ma as ma
 from numba import cuda
 import math
-import sat_data_input
-import filter_data
+#import sat_data_input
+#import filter_data
 
 
 # limit - [lat1,lat2,lon1,lon2]
 # gsize - pixel size
 # indata - inputs
 # inlat - list of latitudes we map for
 # inlon - list of longitudes we map for
```

### Comparing `pyroscopegridding-0.0.3/pyroscopegridding/gtools.py` & `pyroscopegridding-0.0.8/pyroscopegridding/gtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 # Gtools
 #
 # the control for the file. It parses command line arguments and calls to grid_ncf
 #
 
 #import other module files
 from concurrent.futures import process
-import sat_data_input
-import filter_data
-import gridding
-import grid_ncf
-import fileparser # comment for specific file functions
-import time_conv
+#import sat_data_input
+#import filter_data
+#import gridding
+#import grid_ncf
+#import fileparser # comment for specific file functions
+#import time_conv
 
 import os
 import argparse
 import numpy as np
 import datetime
 import time
 """
@@ -448,15 +448,15 @@
 
     split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
 
     #grid_ncf.grid_nc_mult_files_time(limit, gsize, indata, inlat, inlon, phy_list, geo_list, split_files, output)
 
 
 
-def control():
+def main():
     # parser object
     parser = argparse.ArgumentParser()
 
     # reads in commands as mutually exclusive group
     cmd_group = parser.add_mutually_exclusive_group()
     cmd_group.add_argument("-r", "--read", action="store_true", help="Reads raw data given file")
     cmd_group.add_argument("-f", "--filter", action="store_true", help="Reads and filters data given file")
@@ -548,11 +548,11 @@
         # "C:/Users/bobgr/Desktop/Spring 2022 NASA/Gridtools Package (Code, README, inputs, outputs, examples, verification)/gridtools/config.yml"
         netCDF_yaml_config_time(str(args.filename), str(args.time_start), str(args.time_end))
     else:
         print("No command given")
         
 
 if __name__ == '__main__':
-    control()
+    main()
```

### Comparing `pyroscopegridding-0.0.3/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.0.8/pyroscopegridding/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.3/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.0.8/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.3/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.0.8/pyroscopegridding/solar_zenith.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 __status__ = "Production"
 # Solar Zenith
 #
 # Calculates solar zenith and azimuth angles. 
 # Contains manual code calculations validated against pysolar
 #
 
-from pysolar.solar import get_altitude
+#from pysolar.solar import get_altitude
 import time
 import math
 
-from sunpy.coordinates import frames
+#from sunpy.coordinates import frames
 #from sunpy.time import Time
-from astropy.coordinates import EarthLocation
-from pvlib import solarposition
-import pytz
+#from astropy.coordinates import EarthLocation
+#from pvlib import solarposition
+##import pytz
 
 
 import datetime
 import numpy as np
 import pandas as pd
 
 import numba as nb
```

### Comparing `pyroscopegridding-0.0.3/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.0.8/pyroscopegridding/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.3/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.0.8/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.0.3
+Version: 0.0.8
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.0.3/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.0.8/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.3/setup.py` & `pyroscopegridding-0.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.8'
 DESCRIPTION = 'Data fusion package for satellite data transformation.'
 LONG_DESCRIPTION = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data.'
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.0.3',      # Initial version
+    version = '0.0.8',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository  
     keywords = ['data fusion', 'satellite', 'L2', 'L3'],   # Keywords
     #packages = find_packages(),
     entry_points ={
         'console_scripts': [
-            'pyroscopegridding = pyroscopegridding.gtools:main'
-        ]
+            'pyroscopegridding = pyroscopegridding.gtools:main',
+        ],
     },
     install_requires=[            
             'numpy',
             'joblib',
             #'cuda',
             'netCDF4',
             'pyhdf',
```

