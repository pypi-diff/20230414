# Comparing `tmp/ligo-raven-3.1.tar.gz` & `tmp/ligo-raven-3.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo-raven-3.1.tar", last modified: Fri Apr 14 17:06:43 2023, max compression
+gzip compressed data, was "ligo-raven-3.1.dev0.tar", last modified: Fri Mar 24 20:26:25 2023, max compression
```

## Comparing `ligo-raven-3.1.tar` & `ligo-raven-3.1.dev0.tar`

### file list

```diff
@@ -1,61 +1,30 @@
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2023-04-14 17:06:43.656147 ligo-raven-3.1/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)       47 2019-05-08 18:43:01.000000 ligo-raven-3.1/.gitignore
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     2525 2023-04-14 16:49:55.000000 ligo-raven-3.1/.gitlab-ci.yml
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      211 2023-04-14 16:49:55.000000 ligo-raven-3.1/.readthedocs.yml
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     8606 2023-04-14 16:58:28.000000 ligo-raven-3.1/CHANGES.rst
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    35147 2019-05-08 18:43:01.000000 ligo-raven-3.1/COPYING
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     1102 2019-07-01 02:15:39.000000 ligo-raven-3.1/INSTALL
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      113 2022-08-15 18:05:41.000000 ligo-raven-3.1/MANIFEST.in
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      638 2023-04-14 17:06:43.656225 ligo-raven-3.1/PKG-INFO
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     1331 2022-05-04 18:11:57.000000 ligo-raven-3.1/README.md
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2023-04-14 17:06:43.621677 ligo-raven-3.1/bin/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     6013 2023-03-27 15:19:23.000000 ligo-raven-3.1/bin/raven_calc_signif_gracedb
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     5980 2023-03-27 15:19:23.000000 ligo-raven-3.1/bin/raven_coinc_far
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     3721 2023-02-14 19:35:16.000000 ligo-raven-3.1/bin/raven_query
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     3600 2022-11-18 21:23:10.000000 ligo-raven-3.1/bin/raven_search
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     4018 2022-05-04 17:24:08.000000 ligo-raven-3.1/bin/raven_skymap_overlap
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      120 2023-04-14 16:31:15.000000 ligo-raven-3.1/doc-requirements.txt
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2023-04-14 17:06:43.622079 ligo-raven-3.1/ligo/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)       56 2019-07-01 02:15:39.000000 ligo-raven-3.1/ligo/__init__.py
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2023-04-14 17:06:43.622635 ligo-raven-3.1/ligo/raven/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)        0 2019-07-01 02:15:39.000000 ligo-raven-3.1/ligo/raven/__init__.py
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     9718 2023-03-27 15:19:23.000000 ligo-raven-3.1/ligo/raven/gracedb_events.py
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    27219 2023-04-14 16:49:55.000000 ligo-raven-3.1/ligo/raven/search.py
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2023-04-14 17:06:43.624890 ligo-raven-3.1/ligo/raven/tests/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     9571 2022-11-18 21:23:10.000000 ligo-raven-3.1/ligo/raven/tests/FAR_study.py
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2023-04-14 17:06:43.626917 ligo-raven-3.1/ligo/raven/tests/FAR_study_results/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    32459 2022-11-18 21:23:10.000000 ligo-raven-3.1/ligo/raven/tests/FAR_study_results/Coincidence_far.png
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    30448 2022-11-18 21:23:10.000000 ligo-raven-3.1/ligo/raven/tests/FAR_study_results/Coincidence_spat_far.png
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    30028 2022-11-18 21:23:10.000000 ligo-raven-3.1/ligo/raven/tests/FAR_study_results/Gravitational_far.png
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    50193 2022-11-18 21:23:10.000000 ligo-raven-3.1/ligo/raven/tests/FAR_study_results/all_far.png
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      522 2022-11-18 21:23:10.000000 ligo-raven-3.1/ligo/raven/tests/FAR_study_results/output_log.txt
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     9745 2022-11-18 21:23:10.000000 ligo-raven-3.1/ligo/raven/tests/FAR_subgrb_study.py
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2023-04-14 17:06:43.628157 ligo-raven-3.1/ligo/raven/tests/FAR_subgrb_study_results/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    32583 2022-11-18 21:23:10.000000 ligo-raven-3.1/ligo/raven/tests/FAR_subgrb_study_results/Coincidence_far.png
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    30738 2022-11-18 21:23:10.000000 ligo-raven-3.1/ligo/raven/tests/FAR_subgrb_study_results/Coincidence_spat_far.png
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    30571 2022-11-18 21:23:10.000000 ligo-raven-3.1/ligo/raven/tests/FAR_subgrb_study_results/Gravitational_far.png
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    50085 2022-11-18 21:23:10.000000 ligo-raven-3.1/ligo/raven/tests/FAR_subgrb_study_results/all_far.png
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      524 2022-11-18 21:23:10.000000 ligo-raven-3.1/ligo/raven/tests/FAR_subgrb_study_results/output_log.txt
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-15 18:05:41.000000 ligo-raven-3.1/ligo/raven/tests/__init__.py
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2023-04-14 17:06:43.616858 ligo-raven-3.1/ligo/raven/tests/data/
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2023-04-14 17:06:43.648871 ligo-raven-3.1/ligo/raven/tests/data/GW170817/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)  4576512 2022-05-04 17:24:08.000000 ligo-raven-3.1/ligo/raven/tests/data/GW170817/GW170817.fits.gz
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)   777600 2022-05-04 17:24:08.000000 ligo-raven-3.1/ligo/raven/tests/data/GW170817/GW170817.multiorder.fits
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)  1630337 2022-01-14 21:58:51.000000 ligo-raven-3.1/ligo/raven/tests/data/GW170817/bayestar.fits.gz
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)  1586880 2022-01-14 21:58:51.000000 ligo-raven-3.1/ligo/raven/tests/data/GW170817/glg_healpix_all_bn_v00.fit
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)  1255680 2022-05-04 17:24:08.000000 ligo-raven-3.1/ligo/raven/tests/data/GW170817/glg_healpix_all_bn_v00.multiorder.fits
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2023-04-14 17:06:43.655761 ligo-raven-3.1/ligo/raven/tests/data/basic_skymaps/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)   777600 2022-05-04 17:24:08.000000 ligo-raven-3.1/ligo/raven/tests/data/basic_skymaps/bayestar.multiorder.fits
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    96908 2022-05-04 17:24:08.000000 ligo-raven-3.1/ligo/raven/tests/data/basic_skymaps/fermi_test_skymap.fits.gz
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      591 2022-05-04 17:24:08.000000 ligo-raven-3.1/ligo/raven/tests/data/basic_skymaps/flat-skymap.fits.gz
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     8640 2022-05-04 17:24:08.000000 ligo-raven-3.1/ligo/raven/tests/data/basic_skymaps/flat-skymap.multiorder.fits
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    51720 2022-05-04 17:24:08.000000 ligo-raven-3.1/ligo/raven/tests/data/basic_skymaps/swift_test_skymap.fits.gz
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     7403 2023-03-27 15:19:23.000000 ligo-raven-3.1/ligo/raven/tests/mock_gracedb_rest.py
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     7530 2023-03-27 15:19:23.000000 ligo-raven-3.1/ligo/raven/tests/mock_gracedb_sdk.py
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     9995 2022-05-17 17:30:23.000000 ligo-raven-3.1/ligo/raven/tests/test_overlap_integral.py
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    30184 2023-03-27 15:19:23.000000 ligo-raven-3.1/ligo/raven/tests/test_raven_search.py
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     7811 2022-11-18 21:23:10.000000 ligo-raven-3.1/ligo/raven/tests/test_search_window.py
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2023-04-14 17:06:43.656053 ligo-raven-3.1/ligo_raven.egg-info/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     1790 2023-04-14 17:06:43.000000 ligo-raven-3.1/ligo_raven.egg-info/SOURCES.txt
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      254 2023-04-14 17:06:43.656544 ligo-raven-3.1/setup.cfg
--rwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)     2241 2023-04-14 17:03:44.000000 ligo-raven-3.1/setup.py
+drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-03-24 20:26:25.135446 ligo-raven-3.1.dev0/
+-rw-r--r--   0 naresh     (505) staff       (20)    35147 2023-03-06 14:54:32.000000 ligo-raven-3.1.dev0/COPYING
+-rw-r--r--   0 naresh     (505) staff       (20)      113 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/MANIFEST.in
+-rw-r--r--   0 naresh     (505) staff       (20)      671 2023-03-24 20:26:25.135635 ligo-raven-3.1.dev0/PKG-INFO
+-rw-r--r--   0 naresh     (505) staff       (20)     1331 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/README.md
+drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-03-24 20:26:25.125741 ligo-raven-3.1.dev0/bin/
+-rw-r--r--   0 naresh     (505) staff       (20)     6013 2023-03-24 20:19:19.000000 ligo-raven-3.1.dev0/bin/raven_calc_signif_gracedb
+-rw-r--r--   0 naresh     (505) staff       (20)     5980 2023-03-24 20:19:19.000000 ligo-raven-3.1.dev0/bin/raven_coinc_far
+-rw-r--r--   0 naresh     (505) staff       (20)     3721 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/bin/raven_query
+-rw-r--r--   0 naresh     (505) staff       (20)     3600 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/bin/raven_search
+-rw-r--r--   0 naresh     (505) staff       (20)     4018 2023-03-06 14:54:32.000000 ligo-raven-3.1.dev0/bin/raven_skymap_overlap
+drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-03-24 20:26:25.126322 ligo-raven-3.1.dev0/ligo/
+-rw-r--r--   0 naresh     (505) staff       (20)       56 2023-03-06 14:54:32.000000 ligo-raven-3.1.dev0/ligo/__init__.py
+drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-03-24 20:26:25.127725 ligo-raven-3.1.dev0/ligo/raven/
+-rw-r--r--   0 naresh     (505) staff       (20)        0 2023-03-06 14:54:32.000000 ligo-raven-3.1.dev0/ligo/raven/__init__.py
+-rw-r--r--   0 naresh     (505) staff       (20)     9718 2023-03-24 20:19:19.000000 ligo-raven-3.1.dev0/ligo/raven/gracedb_events.py
+-rw-r--r--   0 naresh     (505) staff       (20)    27451 2023-03-24 20:19:19.000000 ligo-raven-3.1.dev0/ligo/raven/search.py
+drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-03-24 20:26:25.134263 ligo-raven-3.1.dev0/ligo/raven/tests/
+-rw-r--r--   0 naresh     (505) staff       (20)     9571 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/FAR_study.py
+-rw-r--r--   0 naresh     (505) staff       (20)     9745 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/FAR_subgrb_study.py
+-rw-r--r--   0 naresh     (505) staff       (20)        0 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/__init__.py
+-rw-r--r--   0 naresh     (505) staff       (20)     7403 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/mock_gracedb_rest.py
+-rw-r--r--   0 naresh     (505) staff       (20)     7530 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/mock_gracedb_sdk.py
+-rw-r--r--   0 naresh     (505) staff       (20)     9995 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/test_overlap_integral.py
+-rw-r--r--   0 naresh     (505) staff       (20)    30184 2023-03-24 20:19:19.000000 ligo-raven-3.1.dev0/ligo/raven/tests/test_raven_search.py
+-rw-r--r--   0 naresh     (505) staff       (20)     7811 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/test_search_window.py
+drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-03-24 20:26:25.135088 ligo-raven-3.1.dev0/ligo_raven.egg-info/
+-rw-r--r--   0 naresh     (505) staff       (20)      536 2023-03-24 20:26:25.000000 ligo-raven-3.1.dev0/ligo_raven.egg-info/SOURCES.txt
+-rw-r--r--   0 naresh     (505) staff       (20)      254 2023-03-24 20:26:25.136417 ligo-raven-3.1.dev0/setup.cfg
+-rwxr-xr-x   0 naresh     (505) staff       (20)     2220 2023-03-24 20:22:37.000000 ligo-raven-3.1.dev0/setup.py
```

### Comparing `ligo-raven-3.1/COPYING` & `ligo-raven-3.1.dev0/COPYING`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/README.md` & `ligo-raven-3.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/bin/raven_calc_signif_gracedb` & `ligo-raven-3.1.dev0/bin/raven_calc_signif_gracedb`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/bin/raven_coinc_far` & `ligo-raven-3.1.dev0/bin/raven_coinc_far`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/bin/raven_query` & `ligo-raven-3.1.dev0/bin/raven_query`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/bin/raven_search` & `ligo-raven-3.1.dev0/bin/raven_search`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/bin/raven_skymap_overlap` & `ligo-raven-3.1.dev0/bin/raven_skymap_overlap`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/ligo/raven/gracedb_events.py` & `ligo-raven-3.1.dev0/ligo/raven/gracedb_events.py`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/ligo/raven/search.py` & `ligo-raven-3.1.dev0/ligo/raven/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 __author__ = "Alex Urban <alexander.urban@ligo.org>"
 
 
 # Imports.
 import json
 import re
 import sys
+import warnings
 
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 import astropy_healpix as ah
 import healpy as hp
 import numpy as np
 
@@ -309,17 +310,17 @@
     se_order = 'nested' if se_nested or any(se_skymap_uniq) else 'ring'
     ext_order = 'nested' if ext_nested or any(ext_skymap_uniq) else 'ring'
 
     # Enforce the sky maps to be non-negative
     se_skymap = np.abs(se_skymap)
     exttrig_skymap = np.abs(exttrig_skymap)
 
-    if not any(exttrig_skymap) and not (ra is not None and dec is not None):
+    if not any(exttrig_skymap) and not (ra and dec):
         # Raise error if external info not given
-        raise ValueError("Please provide external sky map or ra/dec")
+        raise AssertionError('Provide external sky map or ra/dec')
 
     # Use multi-ordered GW sky map
     if any(se_skymap_uniq):
         # gw_skymap is the probability density instead of probability
         # convert GW sky map uniq to ra and dec
         level, ipix = ah.uniq_to_level_ipix(se_skymap_uniq)
         nsides = ah.level_to_nside(level)
@@ -340,55 +341,61 @@
                                      order=ext_order)
             # Find closest external pixels to gw pixels
             c = SkyCoord(ra=ra_gw, dec=dec_gw)
             catalog = SkyCoord(ra=ra_ext, dec=dec_ext)
             ext_ind, d2d, d3d = c.match_to_catalog_sky(catalog)
             ext_norm = np.sum(exttrig_skymap * ah.nside_to_pixel_area(nsides))
 
-            return np.sum(se_skymap * areas * exttrig_skymap[ext_ind] /
-                          sky_prior / se_norm / ext_norm).to(1).value
+            skymap_overlap_integral = \
+                np.sum(se_skymap * areas *
+                       exttrig_skymap[ext_ind] /
+                       sky_prior / se_norm / ext_norm).to(1).value
 
-        elif ra is not None and dec is not None:
+        elif ra and dec:
             # Use multi-ordered gw sky map and one external point
             # Relevant for very well localized experiments
             # such as Swift
             c = SkyCoord(ra=ra*u.degree, dec=dec*u.degree)
             catalog = SkyCoord(ra=ra_gw, dec=dec_gw)
             ind, d2d, d3d = c.match_to_catalog_sky(catalog)
 
-            return (se_skymap[ind] / u.sr / sky_prior / se_norm).to(1).value
+            skymap_overlap_integral = \
+                (se_skymap[ind] / u.sr / sky_prior / se_norm).to(1).value
 
         elif any(exttrig_skymap):
             # Use multi-ordered gw sky map and flat external sky map
             # Find matching external sky map indices using GW ra/dec
             ext_nside = ah.npix_to_nside(len(exttrig_skymap))
             ext_ind = \
                 ah.lonlat_to_healpix(ra_gw, dec_gw, ext_nside,
                                      order=ext_order)
 
             ext_norm = np.sum(exttrig_skymap)
 
-            return np.sum(se_skymap * areas * exttrig_skymap[ext_ind] /
-                          ah.nside_to_pixel_area(ext_nside) /
-                          sky_prior / se_norm / ext_norm).to(1).value
+            skymap_overlap_integral = \
+                np.sum(se_skymap * areas *
+                       exttrig_skymap[ext_ind] /
+                       ah.nside_to_pixel_area(ext_nside) /
+                       sky_prior / se_norm / ext_norm).to(1).value
 
     # Use flat GW sky map
     else:
-        if ra is not None and dec is not None:
+        if ra and dec:
             # Use flat gw sky and one external point
             se_nside = ah.npix_to_nside(len(se_skymap))
             ind = ah.lonlat_to_healpix(ra * u.deg, dec * u.deg, se_nside,
                                        order=se_order)
             se_norm = sum(se_skymap)
-            return se_skymap[ind] * len(se_skymap) / se_norm
+            skymap_overlap_integral = se_skymap[ind] * len(se_skymap) / se_norm
 
         elif any(exttrig_skymap):
             if se_nested != ext_nested:
-                raise ValueError("Sky maps must both use nested or ring"
-                                 "ordering")
+                warnings.warn('Sky maps not both using the same ordering '
+                              '(nested or ring). Result is likely '
+                              'incorrect.')
             # Use two flat sky maps
             nside_s = hp.npix2nside(len(se_skymap))
             nside_e = hp.npix2nside(len(exttrig_skymap))
             if nside_s > nside_e:
                 exttrig_skymap = hp.ud_grade(exttrig_skymap,
                                              nside_out=nside_s,
                                              order_in=('NESTED' if ext_nested
@@ -397,21 +404,24 @@
                 se_skymap = hp.ud_grade(se_skymap,
                                         nside_out=nside_e,
                                         order_in=('NESTED' if se_nested
                                                   else 'RING'))
             se_norm = se_skymap.sum()
             exttrig_norm = exttrig_skymap.sum()
             if se_norm > 0 and exttrig_norm > 0:
-                return (np.dot(se_skymap, exttrig_skymap) / se_norm /
-                        exttrig_norm * len(se_skymap))
+                skymap_overlap_integral = (
+                    np.dot(se_skymap, exttrig_skymap)
+                    / se_norm / exttrig_norm
+                    * len(se_skymap))
             else:
-                return ("RAVEN: ERROR: At least one sky map has a "
-                        "probability density that sums to zero or less.")
+                message = ("RAVEN: ERROR: At least one sky map has a "
+                           "probability density that sums to zero or less.")
+                return message
 
-    raise ValueError("Please provide both GW and external sky map info")
+    return skymap_overlap_integral
 
 
 def coinc_far(se_id, ext_id, tl, th, grb_search='GRB', se_fitsfile=None,
               ext_fitsfile=None, incl_sky=False,
               gracedb=None, far_grb=None, em_rate=None,
               far_gw_thresh=None, far_grb_thresh=None,
               se_dict=None, ext_dict=None,
```

### Comparing `ligo-raven-3.1/ligo/raven/tests/FAR_study.py` & `ligo-raven-3.1.dev0/ligo/raven/tests/FAR_study.py`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/ligo/raven/tests/FAR_subgrb_study.py` & `ligo-raven-3.1.dev0/ligo/raven/tests/FAR_subgrb_study.py`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/ligo/raven/tests/mock_gracedb_rest.py` & `ligo-raven-3.1.dev0/ligo/raven/tests/mock_gracedb_rest.py`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/ligo/raven/tests/mock_gracedb_sdk.py` & `ligo-raven-3.1.dev0/ligo/raven/tests/mock_gracedb_sdk.py`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/ligo/raven/tests/test_overlap_integral.py` & `ligo-raven-3.1.dev0/ligo/raven/tests/test_overlap_integral.py`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/ligo/raven/tests/test_raven_search.py` & `ligo-raven-3.1.dev0/ligo/raven/tests/test_raven_search.py`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/ligo/raven/tests/test_search_window.py` & `ligo-raven-3.1.dev0/ligo/raven/tests/test_search_window.py`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1/setup.py` & `ligo-raven-3.1.dev0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,22 +23,21 @@
 
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='ligo-raven',
-    version='3.1',
+    version='3.1.dev0',
     url='http://gracedb.ligo.org',
     author='Alex Urban',
     author_email='alexander.urban@ligo.org',
     maintainer="Brandon Piotrzkowski",
     maintainer_email="brandon.piotrzkowski@ligo.org",
     description='Low-latency coincidence search between external triggers and GW candidates',
-    readme = "README.md",
     license='GNU General Public License Version 3',
     classifiers=(
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Topic :: Internet",
         "Topic :: Scientific/Engineering :: Astronomy",
         "Topic :: Scientific/Engineering :: Physics"
```

