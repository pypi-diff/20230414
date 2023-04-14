# Comparing `tmp/NREL-farms-1.0.4.tar.gz` & `tmp/NREL-farms-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NREL-farms-1.0.4.tar", last modified: Tue Nov 16 21:32:52 2021, max compression
+gzip compressed data, was "NREL-farms-1.0.5.tar", last modified: Fri Apr 14 15:19:53 2023, max compression
```

## Comparing `NREL-farms-1.0.4.tar` & `NREL-farms-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 21:32:52.799136 NREL-farms-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2021-11-16 21:32:42.000000 NREL-farms-1.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 21:32:52.795136 NREL-farms-1.0.4/NREL_farms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3553 2021-11-16 21:32:52.000000 NREL-farms-1.0.4/NREL_farms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      312 2021-11-16 21:32:52.000000 NREL-farms-1.0.4/NREL_farms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-16 21:32:52.000000 NREL-farms-1.0.4/NREL_farms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-16 21:32:52.000000 NREL-farms-1.0.4/NREL_farms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-11-16 21:32:52.000000 NREL-farms-1.0.4/NREL_farms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-11-16 21:32:52.000000 NREL-farms-1.0.4/NREL_farms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3553 2021-11-16 21:32:52.799136 NREL-farms-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2849 2021-11-16 21:32:42.000000 NREL-farms-1.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 21:32:52.799136 NREL-farms-1.0.4/farms/
--rw-r--r--   0 runner    (1001) docker     (121)      678 2021-11-16 21:32:42.000000 NREL-farms-1.0.4/farms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3239 2021-11-16 21:32:42.000000 NREL-farms-1.0.4/farms/disc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8410 2021-11-16 21:32:42.000000 NREL-farms-1.0.4/farms/farms.py
--rw-r--r--   0 runner    (1001) docker     (121)    16982 2021-11-16 21:32:42.000000 NREL-farms-1.0.4/farms/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-11-16 21:32:42.000000 NREL-farms-1.0.4/farms/version.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-16 21:32:52.799136 NREL-farms-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2021-11-16 21:32:42.000000 NREL-farms-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:19:53.593688 NREL-farms-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-14 15:19:44.000000 NREL-farms-1.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:19:53.589688 NREL-farms-1.0.5/NREL_farms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-14 15:19:53.000000 NREL-farms-1.0.5/NREL_farms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-14 15:19:53.000000 NREL-farms-1.0.5/NREL_farms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:19:53.000000 NREL-farms-1.0.5/NREL_farms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:19:53.000000 NREL-farms-1.0.5/NREL_farms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 15:19:53.000000 NREL-farms-1.0.5/NREL_farms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 15:19:53.000000 NREL-farms-1.0.5/NREL_farms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-04-14 15:19:53.593688 NREL-farms-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-14 15:19:44.000000 NREL-farms-1.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:19:53.593688 NREL-farms-1.0.5/farms/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-14 15:19:44.000000 NREL-farms-1.0.5/farms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-14 15:19:44.000000 NREL-farms-1.0.5/farms/disc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-04-14 15:19:44.000000 NREL-farms-1.0.5/farms/farms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18980 2023-04-14 15:19:44.000000 NREL-farms-1.0.5/farms/farms_dni.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-04-14 15:19:44.000000 NREL-farms-1.0.5/farms/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 15:19:44.000000 NREL-farms-1.0.5/farms/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:19:53.593688 NREL-farms-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-14 15:19:44.000000 NREL-farms-1.0.5/setup.py
```

### Comparing `NREL-farms-1.0.4/LICENSE` & `NREL-farms-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `NREL-farms-1.0.4/NREL_farms.egg-info/PKG-INFO` & `NREL-farms-1.0.5/NREL_farms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-farms
-Version: 1.0.4
+Version: 1.0.5
 Summary: The Fast All-sky Radiation Model for Solar applications (FARMS)
 Home-page: https://github.com/NREL/farms
 Author: Grant Buster
 Author-email: grant.buster@nrel.gov
 License: BSD 3-Clause
 Keywords: farms
 Platform: UNKNOWN
```

### Comparing `NREL-farms-1.0.4/PKG-INFO` & `NREL-farms-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-farms
-Version: 1.0.4
+Version: 1.0.5
 Summary: The Fast All-sky Radiation Model for Solar applications (FARMS)
 Home-page: https://github.com/NREL/farms
 Author: Grant Buster
 Author-email: grant.buster@nrel.gov
 License: BSD 3-Clause
 Keywords: farms
 Platform: UNKNOWN
```

### Comparing `NREL-farms-1.0.4/README.rst` & `NREL-farms-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `NREL-farms-1.0.4/farms/__init__.py` & `NREL-farms-1.0.5/farms/__init__.py`

 * *Files identical despite different names*

### Comparing `NREL-farms-1.0.4/farms/disc.py` & `NREL-farms-1.0.5/farms/disc.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     4) Water and Pressure were changed to vectors from scalers
 """
 import numpy as np
 
 from farms import SOLAR_CONSTANT
 
 
-def disc(ghi, sza, doy, pressure=101325, sza_lim=87):
+def disc(ghi, sza, doy, pressure=1013.25, sza_lim=87):
     """Estimate DNI from GHI using the DISC model.
 
     *Warning: should only be used for cloudy FARMS data.
 
     The DISC algorithm converts global horizontal irradiance to direct
     normal irradiance through empirical relationships between the global
     and direct clearness indices.
```

### Comparing `NREL-farms-1.0.4/farms/farms.py` & `NREL-farms-1.0.5/farms/farms.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     (http://www.sciencedirect.com/science/article/pii/S0038092X16301827)
 """
 import collections
 import numpy as np
 
 from farms import CLEAR_TYPES, ICE_TYPES, WATER_TYPES, SOLAR_CONSTANT
 import farms.utilities as ut
+from farms import farms_dni
 
 
 def water_phase(tau, De, solar_zenith_angle):
     """Get cloudy Tducld and Ruucld for the water phase."""
     # enforce water phase particle size between 5 and 120 micron
     # as per advice from yu xie
     De = np.maximum(De, 5)
@@ -153,22 +154,40 @@
     albedo : np.ndarray
         Ground albedo.
     debug : bool
         Flag to output additional transmission/reflectance variables.
 
     Returns
     -------
-    ghi : np.ndarray
-        FARMS GHI values (this is the only output if debug is False).
-    fast_data : collections.namedtuple
-        Additional debugging variables if debug is True.
-        Named tuple with irradiance data. Attributes:
-            ghi : global horizontal irradiance (w/m2)
-            dni : direct normal irradiance (w/m2)
-            dhi : diffuse horizontal irradiance (w/m2)
+    If debug == True:
+        fast_data : collections.namedtuple
+            Named tuple with irradiance data with the following attributes:
+                ghi : np.ndarray
+                    global horizontal irradiance (W/m2)
+                dni : np.ndarray
+                    direct normal irradiance (W/m2)
+                dhi : np.ndarray
+                    diffuse horizontal irradiance (W/m2)
+                Ruucld : np.ndarray
+                    Aerosol reflectance for diffuse fluxes for cloudy
+                    atmosphere.
+                Tddcld : np.ndarray
+                    Transmittance of the cloudy atmosphere for direct incident
+                    and direct outgoing fluxes (dd).
+                Tducld : np.ndarray
+                    Transmittance of the cloudy atmosphere for direct incident
+                    and diffuse outgoing fluxes (du).
+    else:
+        ghi: np.ndarray
+            Global horizontal irradiance (W/m2)
+        dni_farmsdni: np.ndarray
+            DNI computed by FARMS-DNI (W/m2).
+        dni0: np.ndarray
+            DNI computed by the Lambert law (W/m2). It only includes the narrow
+            beam in the circumsolar region.
     """
     # disable divide by zero warnings
     np.seterr(divide='ignore')
 
     ut.check_range(Tddclr, 'Tddclr')
     ut.check_range(Tduclr, 'Tduclr')
     ut.check_range(Ruuclr, 'Ruuclr')
@@ -204,14 +223,18 @@
                                     + Tducld * Tuuclr)  # eq 3 from [1]
 
     # ghi eqn 6 from [1]
     ghi = F1 / (1.0 - albedo * (Ruuclr + Ruucld * Tuuclr * Tuuclr))
     dni = Fd / solar_zenith_angle  # eq 2b from [1]
     dhi = ghi - Fd  # eq 7 from [1]
 
+    Fd, dni_farmsdni, dni0 = farms_dni.farms_dni(F0, tau, solar_zenith_angle,
+                                                 De, phase, phase1, phase2,
+                                                 Tddclr, ghi, F1)
+
     clear_mask = np.in1d(cloud_type, CLEAR_TYPES).reshape(cloud_type.shape)
     if debug:
         # Return NaN if clear-sky, else return cloudy sky data
         fast_data = collections.namedtuple('fast_data', ['ghi', 'dni', 'dhi',
                                                          'Tddcld', 'Tducld',
                                                          'Ruucld'])
         fast_data.Tddcld = np.where(clear_mask, np.nan, Tddcld)
@@ -219,9 +242,11 @@
         fast_data.Ruucld = np.where(clear_mask, np.nan, Ruucld)
         fast_data.ghi = np.where(clear_mask, np.nan, ghi)
         fast_data.dni = np.where(clear_mask, np.nan, dni)
         fast_data.dhi = np.where(clear_mask, np.nan, dhi)
 
         return fast_data
     else:
-        # return only GHI
-        return np.where(clear_mask, np.nan, ghi)
+        out = (np.where(clear_mask, np.nan, ghi),
+               np.where(clear_mask, np.nan, dni_farmsdni),
+               np.where(clear_mask, np.nan, dni0))
+        return out
```

### Comparing `NREL-farms-1.0.4/farms/utilities.py` & `NREL-farms-1.0.5/farms/utilities.py`

 * *Files identical despite different names*

### Comparing `NREL-farms-1.0.4/setup.py` & `NREL-farms-1.0.5/setup.py`

 * *Files identical despite different names*

