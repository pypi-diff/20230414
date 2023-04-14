# Comparing `tmp/cfr-0.4.4.tar.gz` & `tmp/cfr-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-0.4.4.tar", last modified: Thu Apr  6 07:47:03 2023, max compression
+gzip compressed data, was "cfr-0.4.5.tar", last modified: Fri Apr 14 08:23:26 2023, max compression
```

## Comparing `cfr-0.4.4.tar` & `cfr-0.4.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-06 07:47:03.312850 cfr-0.4.4/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1516 2023-03-03 14:30:05.000000 cfr-0.4.4/LICENSE
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1693 2023-04-06 07:47:03.312221 cfr-0.4.4/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1129 2023-03-03 14:30:05.000000 cfr-0.4.4/README.rst
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-06 07:47:03.157213 cfr-0.4.4/bin/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3905 2023-03-03 14:30:05.000000 cfr-0.4.4/bin/cfr
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-06 07:47:03.232855 cfr-0.4.4/cfr/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      640 2023-03-24 19:14:09.000000 cfr-0.4.4/cfr/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    18218 2023-04-06 07:21:11.000000 cfr-0.4.4/cfr/climate.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-06 07:47:03.310996 cfr-0.4.4/cfr/da/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       22 2023-03-03 14:30:05.000000 cfr-0.4.4/cfr/da/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    16319 2023-03-26 05:47:23.000000 cfr-0.4.4/cfr/da/enkf.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    16745 2023-04-04 01:21:41.000000 cfr-0.4.4/cfr/gcm.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7623 2023-03-03 14:30:05.000000 cfr-0.4.4/cfr/ml.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    60787 2023-04-06 03:07:13.000000 cfr-0.4.4/cfr/proxy.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    44966 2023-04-06 02:13:26.000000 cfr-0.4.4/cfr/psm.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    50022 2023-03-26 21:55:53.000000 cfr-0.4.4/cfr/reconjob.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2311 2023-03-26 06:27:24.000000 cfr-0.4.4/cfr/reconres.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    17830 2023-04-06 07:20:24.000000 cfr-0.4.4/cfr/ts.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    20677 2023-03-27 06:51:18.000000 cfr-0.4.4/cfr/utils.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    54810 2023-04-06 07:30:44.000000 cfr-0.4.4/cfr/visual.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-06 07:47:03.308933 cfr-0.4.4/cfr.egg-info/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1693 2023-04-06 07:47:02.000000 cfr-0.4.4/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      374 2023-04-06 07:47:02.000000 cfr-0.4.4/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-04-06 07:47:02.000000 cfr-0.4.4/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-03-03 14:35:18.000000 cfr-0.4.4/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      203 2023-04-06 07:47:02.000000 cfr-0.4.4/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-04-06 07:47:02.000000 cfr-0.4.4/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-04-06 07:47:03.313030 cfr-0.4.4/setup.cfg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1415 2023-04-06 03:09:34.000000 cfr-0.4.4/setup.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-14 08:23:26.180477 cfr-0.4.5/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1516 2023-03-03 14:30:05.000000 cfr-0.4.5/LICENSE
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1693 2023-04-14 08:23:26.180080 cfr-0.4.5/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1129 2023-03-03 14:30:05.000000 cfr-0.4.5/README.rst
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-14 08:23:25.856174 cfr-0.4.5/bin/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3905 2023-03-03 14:30:05.000000 cfr-0.4.5/bin/cfr
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-14 08:23:26.073004 cfr-0.4.5/cfr/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      640 2023-03-24 19:14:09.000000 cfr-0.4.5/cfr/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    18148 2023-04-14 08:22:21.000000 cfr-0.4.5/cfr/climate.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-14 08:23:26.179292 cfr-0.4.5/cfr/da/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       22 2023-03-03 14:30:05.000000 cfr-0.4.5/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    16319 2023-03-26 05:47:23.000000 cfr-0.4.5/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    18762 2023-04-12 21:07:20.000000 cfr-0.4.5/cfr/gcm.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7623 2023-03-03 14:30:05.000000 cfr-0.4.5/cfr/ml.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    60727 2023-04-14 08:22:33.000000 cfr-0.4.5/cfr/proxy.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    44966 2023-04-06 02:13:26.000000 cfr-0.4.5/cfr/psm.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    49933 2023-04-09 06:47:02.000000 cfr-0.4.5/cfr/reconjob.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2311 2023-03-26 06:27:24.000000 cfr-0.4.5/cfr/reconres.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    17830 2023-04-06 07:20:24.000000 cfr-0.4.5/cfr/ts.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    20677 2023-03-27 06:51:18.000000 cfr-0.4.5/cfr/utils.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    54810 2023-04-06 07:30:44.000000 cfr-0.4.5/cfr/visual.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-14 08:23:26.178239 cfr-0.4.5/cfr.egg-info/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1693 2023-04-14 08:23:25.000000 cfr-0.4.5/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      374 2023-04-14 08:23:25.000000 cfr-0.4.5/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-04-14 08:23:25.000000 cfr-0.4.5/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-03-03 14:35:18.000000 cfr-0.4.5/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      203 2023-04-14 08:23:25.000000 cfr-0.4.5/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-04-14 08:23:25.000000 cfr-0.4.5/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-04-14 08:23:26.180574 cfr-0.4.5/setup.cfg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1415 2023-04-14 08:21:20.000000 cfr-0.4.5/setup.py
```

### Comparing `cfr-0.4.4/LICENSE` & `cfr-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-0.4.4/PKG-INFO` & `cfr-0.4.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.4.4
+Version: 0.4.5
 Summary: cfr: the Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: paleocliamte reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.4.4/README.rst` & `cfr-0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `cfr-0.4.4/bin/cfr` & `cfr-0.4.5/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-0.4.4/cfr/__init__.py` & `cfr-0.4.5/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.4/cfr/climate.py` & `cfr-0.4.5/cfr/climate.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,14 @@
 
     def to_nc(self, path, verbose=True, compress_params=None):
         ''' Convert the climate field to a netCDF file.
 
         Args:
             path (str): the path where to save
         '''
-        # _comp_params = {'zlib': True, 'least_significant_digit': 2}
         _comp_params = {'zlib': True}
 
         encoding_dict = {}
         if compress_params is not None:
             _comp_params.update(compress_params)
 
         encoding_dict[self.da.name] = _comp_params
```

### Comparing `cfr-0.4.4/cfr/da/enkf.py` & `cfr-0.4.5/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.4/cfr/gcm.py` & `cfr-0.4.5/cfr/gcm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import glob
 import xarray as xr
 import numpy as np
 from tqdm import tqdm
 import datetime
+import cftime
 import matplotlib.pyplot as plt
 from matplotlib import gridspec
 from . import visual
 from .ts import EnsTS
 from .climate import ClimateField
 from .utils import (
     coefficient_efficiency,
@@ -68,15 +69,15 @@
     def get_ds(self, idx=0):
         ''' Get a `xarray.Dataset` from a certain file
         '''
         with xr.open_dataset(self.paths[idx]) as ds:
             return ds
 
     def load(self, vars=None, time_name='time', z_name='z_t', z_val=None,
-             adjust_month=False, mode='time-slice',
+             adjust_month=False, mode='timeslice',
              save_dirpath=None, compress_params=None, verbose=False):
         ''' Load variables.
 
         Args:
             vars (list): list of variable names.
             time_name (str): the name of the time dimension.
             z_name (str): the name of the z dimension (e.g., for ocean output).
@@ -144,56 +145,63 @@
             
             else:
                 self.ts[vn] = self.fd[vn[2:]].annualize().geo_mean()
 
             if verbose:
                 p_success(f'>>> GCMCase.ts["{vn}"] created')
 
-    def to_ds(self):
+    def to_ds(self, mode='ts'):
         ''' Convert to a `xarray.Dataset`
         '''
         da_dict = {}
-        for k, v in self.fd.items():
-            da_dict[k] = v.da
-
-        for k, v in self.ts.items():
-            time_name = v.time.name
-            da_dict[k] = xr.DataArray(v.value[:, 0], dims=[time_name], coords={time_name: v.time}, name=k)
+        if mode == 'fd':
+            for k, v in self.fd.items():
+                da_dict[k] = v.da
+
+        elif mode == 'ts':
+            for k, v in self.ts.items():
+                time_name = v.time.name
+                da_dict[k] = xr.DataArray(v.value[:, 0], dims=[time_name], coords={time_name: v.time}, name=k)
 
         ds = xr.Dataset(da_dict)
         if self.name is not None:
             ds.attrs['casename'] = self.name
 
         return ds
 
-    def to_nc(self, path, verbose=True, compress_params=None):
+    def to_nc(self, path, mode='ts', verbose=True, compress_params=None):
         ''' Output the GCM case to a netCDF file.
 
         Args:
             path (str): the path where to save
         '''
-        _comp_params = {'zlib': True, 'least_significant_digit': 2}
+        _comp_params = {'zlib': True}
         encoding_dict = {}
         if compress_params is not None:
             _comp_params.update(compress_params)
 
-        for k, v in self.fd.items():
-            encoding_dict[k] = _comp_params
-
-        for k, v in self.ts.items():
-            encoding_dict[k] = _comp_params
+        if mode == 'fd':
+            for k, v in self.fd.items():
+                encoding_dict[k] = _comp_params
+
+        elif mode == 'ts':
+            for k, v in self.ts.items():
+                encoding_dict[k] = _comp_params
 
         try:
             dirpath = os.path.dirname(path)
             os.makedirs(dirpath, exist_ok=True)
         except:
             pass
 
-        ds = self.to_ds()
+        ds = self.to_ds(mode=mode)
 
+        if os.path.exists(path):
+            os.remove(path)
+            
         ds.to_netcdf(path, encoding=encoding_dict)
         if verbose: p_success(f'>>> GCMCase saved to: {path}')
 
     def load_nc(self, path, verbose=False):
         case = GCMCase()
         ds = xr.open_dataset(path)
         if 'casename' in ds.attrs:
@@ -299,18 +307,20 @@
             return fig, ax
         else:
             return ax
             
     def calc_slab_ocn_forcing(self, ds_clim, time_name='month', lat_name='TLAT', lon_name='TLONG',
                               z_name='z_t', hblt_name='HBLT', temp_name='TEMP', salt_name='SALT',
                               uvel_name='UVEL', vvel_name='VVEL', shf_name='SHF', qflux_name='QFLUX',
-                              anglet_name='ANGLET', region_mask_name='REGION_MASK', save_path=None):
+                              anglet_name='ANGLET', region_mask_name='REGION_MASK',
+                              save_path=None, save_format='NETCDF4_CLASSIC'):
         ''' Calculate the slab ocean forcing
         '''
-        ds_clim = ds_clim.rename({time_name: 'time'})
+        ds_clim = ds_clim.rename({time_name: 'time', 'nlat': 'nj', 'nlon': 'ni'})
+        ds_clim.coords['time'] = [cftime.DatetimeNoLeap(1,i,1,0,0,0,0, has_year_zero=True) for i in range(1, 13)]
 
         hbltin = ds_clim[hblt_name]
         hblt_avg = hbltin.mean('time')
         hblttmp = hblt_avg.expand_dims({'time': 12})/100
 
         z_t = ds_clim[z_name]
         zint = (z_t.values[:-1] + z_t.values[1:])/2/100
@@ -438,29 +448,68 @@
                 dhdx[j] += invM[j, i]*dhdxin[i]
                 dhdy[j] += invM[j, i]*dhdyin[i]
                 hblt[j] += invM[j, i]*hblttmp[i]
                 qdp[j] += invM[j, i]*ocnheat[i]
 
         ds_out = xr.Dataset()
         ds_out['time'] = ds_clim['time']
+        ds_out['time'].attrs['long_name'] = 'days since 0001-01-01 00:00:00'
+        ds_out['time'].attrs['units'] = 'observation time'
+        ds_out['time'].attrs['calendar'] = 'noleap'
+
         ds_out['xc'] = xc
+        ds_out['xc'].attrs['long_name'] = 'longitude of grid cell center'
+        ds_out['xc'].attrs['units'] = 'degrees east'
+
         ds_out['yc'] = yc
+        ds_out['yc'].attrs['long_name'] = 'latitude of grid cell center'
+        ds_out['yc'].attrs['units'] = 'degrees north'
+
         ds_out['T'] = T.where(~np.isnan(ds_clim['TEMP'][0,0,:,:]))
+        ds_out['T'].attrs['long_name'] = 'temperature'
+        ds_out['T'].attrs['units'] = 'degC'
+
         ds_out['S'] = S.where(~np.isnan(ds_clim['TEMP'][0,0,:,:]))
+        ds_out['S'].attrs['long_name'] = 'salinity'
+        ds_out['S'].attrs['units'] = 'ppt'
+
         ds_out['U'] = U.where(~np.isnan(ds_clim['TEMP'][0,0,:,:]))
+        ds_out['U'].attrs['long_name'] = 'u ocean current'
+        ds_out['U'].attrs['units'] = 'm/s'
+
         ds_out['V'] = V.where(~np.isnan(ds_clim['TEMP'][0,0,:,:]))
+        ds_out['V'].attrs['long_name'] = 'v ocean current'
+        ds_out['V'].attrs['units'] = 'm/s'
+
         ds_out['dhdx'] = dhdx.where(~np.isnan(ds_clim['TEMP'][0,0,:,:]))
+        ds_out['dhdx'].attrs['long_name'] = 'ocean surface slope: zonal'
+        ds_out['dhdx'].attrs['units'] = 'm/m'
+
         ds_out['dhdy'] = dhdy.where(~np.isnan(ds_clim['TEMP'][0,0,:,:]))
+        ds_out['dhdy'].attrs['long_name'] = 'ocean surface slope: meridional'
+        ds_out['dhdy'].attrs['units'] = 'm/m'
+
         ds_out['hblt'] = hblt.where(~np.isnan(ds_clim['TEMP'][0,0,:,:]))
+        ds_out['hblt'].attrs['long_name'] = 'boundary layer depth'
+        ds_out['hblt'].attrs['units'] = 'm'
+
         ds_out['qdp'] = qdp.where(~np.isnan(ds_clim['TEMP'][0,0,:,:]))
+        ds_out['qdp'].attrs['long_name'] = 'ocean heat flux convergence'
+        ds_out['qdp'].attrs['units'] = 'W/m^2'
+
         ds_out['area'] = tarea
+        ds_out['area'].attrs['long_name'] = 'area of grid cell in radians squared'
+        ds_out['area'].attrs['units'] = 'area'
+
         ds_out['mask'] = ds_clim[region_mask_name]
+        ds_out['mask'].attrs['long_name'] = 'domain maskr'
+        ds_out['mask'].attrs['units'] = 'unitless'
 
         if save_path is not None:
-            ds_out.to_netcdf(save_path)
+            ds_out.to_netcdf(save_path, format=save_format)
 
         return ds_out
                 
 
 class GCMCases:
     ''' The class for postprocessing multiple GCM simulation cases (e.g., CESM)
     '''
```

### Comparing `cfr-0.4.4/cfr/ml.py` & `cfr-0.4.5/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.4/cfr/proxy.py` & `cfr-0.4.5/cfr/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1445,15 +1445,15 @@
             da = ds[vn]
             new.records[vn] = ProxyRecord().from_da(da)
 
         new.refresh()
         return new
         
 
-    def to_nc(self, path, annualize=False, months=None, verbose=True, compress_params={'zlib': True, 'least_significant_digit': 2}):
+    def to_nc(self, path, annualize=False, months=None, verbose=True, compress_params={'zlib': True}):
         ''' Convert the database to a netCDF file.
 
         Args:
             path (str): the path to save the file.
             annualize (bool): annualize the proxy records with `months`
             months (list): months for annulization
             verbose (bool, optional): print verbose information. Defaults to False.
@@ -1467,15 +1467,15 @@
         if verbose: utils.p_success(f'ProxyDatabase saved to: {path}')
 
     def load_nc(self, path, use_cftime=True, **kwargs):
         ds = xr.open_dataset(path, use_cftime=use_cftime, **kwargs)
         pdb = ProxyDatabase().from_ds(ds)
         return pdb
 
-    def to_multi_nc(self, dirpath, verbose=True, compress_params={'zlib': True, 'least_significant_digit': 2}):
+    def to_multi_nc(self, dirpath, verbose=True, compress_params={'zlib': True}):
         ''' Convert the proxy database to multiple netCDF files. One for each record.
 
         Args:
             dirpath (str): the directory path of the multiple .nc files
         '''
         os.makedirs(dirpath, exist_ok=True)
         pid_truncated = []
```

### Comparing `cfr-0.4.4/cfr/psm.py` & `cfr-0.4.5/cfr/psm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.4/cfr/reconjob.py` & `cfr-0.4.5/cfr/reconjob.py`

 * *Files 1% similar despite different names*

```diff
@@ -560,15 +560,15 @@
         recon_timescale = self.io_cfg('recon_timescale', recon_timescale, default=1, verbose=verbose)  # unit: yr
         recon_vars = self.io_cfg('recon_vars', recon_vars, default=['tas'], verbose=verbose)
         nens = self.io_cfg('nens', nens, default=100, verbose=verbose)
         recon_seeds = self.io_cfg('recon_seeds', recon_seeds, default=np.arange(0, 20), verbose=verbose)
         assim_frac = self.io_cfg('assim_frac', assim_frac, default=0.75, verbose=verbose)
         save_dirpath = self.io_cfg('save_dirpath', save_dirpath, verbose=verbose)
         os.makedirs(save_dirpath, exist_ok=True)
-        compress_params = self.io_cfg('compress_params', compress_params, default={'zlib': True, 'least_significant_digit': 2}, verbose=verbose)
+        compress_params = self.io_cfg('compress_params', compress_params, default={'zlib': True}, verbose=verbose)
         output_full_ens = self.io_cfg('output_full_ens', output_full_ens, default=False, verbose=verbose)
         recon_sampling_mode = self.io_cfg('recon_sampling_mode', recon_sampling_mode, default='fixed', verbose=verbose)
         trim_prior = self.io_cfg('trim_prior', trim_prior, default=True, verbose=verbose)
         allownan = self.io_cfg('allownan', allownan, default=False, verbose=verbose)
         if recon_sampling_mode == 'rolling':
             normal_sampling_sigma = self.io_cfg('normal_sampling_sigma', normal_sampling_sigma, verbose=verbose)
             normal_sampling_cutoff_factor = self.io_cfg('normal_sampling_cutoff_factor', normal_sampling_cutoff_factor, default=3, verbose=verbose)
@@ -589,15 +589,15 @@
 
             recon_savepath = os.path.join(save_dirpath, f'job_r{seed:02d}_recon.nc')
             self.save_recon(recon_savepath, compress_params=compress_params, mark_assim_pids=True,
                             verbose=verbose, output_full_ens=output_full_ens, grid='prior')
 
         t_e = time.time()
         t_used = t_e - t_s
-        p_success(f'>>> DONE! Total time used: {t_used/60:.2f} mins.')
+        p_success(f'>>> DONE! Total time spent: {t_used/60:.2f} mins.')
 
 
     def save(self, save_dirpath=None, filename='job.pkl', verbose=False):
         ''' Save the ReconJob object to a pickle file.
 
         Args:
             save_dirpath (str): the directory path for saving the :py:mod:`cfr.ReconJob` object.
@@ -664,15 +664,15 @@
                 * 'wp'
             compress_params (dict): the paramters for compression when storing the reconstruction results to netCDF files.
             verbose (bool, optional): print verbose information. Defaults to False.
         '''
 
         compress_params = self.io_cfg(
             'compress_params', compress_params,
-            default={'zlib': True, 'least_significant_digit': 2},
+            default={'zlib': True},
             verbose=False)
 
         output_indices = self.io_cfg(
             'output_indices', output_indices,
             default=['gm', 'nhm', 'shm', 'nino3.4'],
             verbose=False)
 
@@ -973,15 +973,15 @@
             verbose (bool, optional): print verbose information. Defaults to False.
             fit_kws (dict): the arguments for :py:meth: `GraphEM.solver.GraphEM.fit`
 
         See also:
             cfr.graphem.solver.GraphEM.fit : fitting the GraphEM method
 
         '''
-        compress_params = self.io_cfg('compress_params', compress_params, default={'zlib': True, 'least_significant_digit': 1}, verbose=verbose)
+        compress_params = self.io_cfg('compress_params', compress_params, default={'zlib': True}, verbose=verbose)
 
         if save_recon:
             save_dirpath = self.io_cfg('save_dirpath', save_dirpath, verbose=verbose)
             save_filename = self.io_cfg('save_filename', save_filename, default='job_r01_recon.nc', verbose=verbose)
             os.makedirs(save_dirpath, exist_ok=True)
 
         if load_precalc_solver:
```

### Comparing `cfr-0.4.4/cfr/reconres.py` & `cfr-0.4.5/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.4/cfr/ts.py` & `cfr-0.4.5/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.4/cfr/utils.py` & `cfr-0.4.5/cfr/utils.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.4/cfr/visual.py` & `cfr-0.4.5/cfr/visual.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.4/cfr.egg-info/PKG-INFO` & `cfr-0.4.5/cfr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.4.4
+Version: 0.4.5
 Summary: cfr: the Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: paleocliamte reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.4.4/setup.py` & `cfr-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='0.4.4',
+    version='0.4.5',
     description='cfr: the Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

