# Comparing `tmp/effluent-1.1.tar.gz` & `tmp/effluent-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "effluent-1.1.tar", last modified: Tue Nov 29 10:37:19 2022, max compression
+gzip compressed data, was "effluent-1.2.tar", last modified: Fri Apr 14 08:50:33 2023, max compression
```

## Comparing `effluent-1.1.tar` & `effluent-1.2.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-29 10:37:19.035280 effluent-1.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2022-11-29 10:37:06.000000 effluent-1.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1895 2022-11-29 10:37:19.035280 effluent-1.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1058 2022-11-29 10:37:06.000000 effluent-1.1/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2022-11-29 10:37:06.000000 effluent-1.1/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1077 2022-11-29 10:37:19.035280 effluent-1.1/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-29 10:37:19.031280 effluent-1.1/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-29 10:37:19.035280 effluent-1.1/src/effluent/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2022-11-29 10:37:06.000000 effluent-1.1/src/effluent/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2022-11-29 10:37:06.000000 effluent-1.1/src/effluent/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12346 2022-11-29 10:37:06.000000 effluent-1.1/src/effluent/io.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3940 2022-11-29 10:37:06.000000 effluent-1.1/src/effluent/jet.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1055 2022-11-29 10:37:06.000000 effluent-1.1/src/effluent/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9187 2022-11-29 10:37:06.000000 effluent-1.1/src/effluent/modeldata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      639 2022-11-29 10:37:06.000000 effluent-1.1/src/effluent/script.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4754 2022-11-29 10:37:06.000000 effluent-1.1/src/effluent/solver.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2289 2022-11-29 10:37:06.000000 effluent-1.1/src/effluent/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-29 10:37:19.035280 effluent-1.1/src/effluent.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1895 2022-11-29 10:37:19.000000 effluent-1.1/src/effluent.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      426 2022-11-29 10:37:19.000000 effluent-1.1/src/effluent.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2022-11-29 10:37:19.000000 effluent-1.1/src/effluent.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2022-11-29 10:37:19.000000 effluent-1.1/src/effluent.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2022-11-29 10:37:19.000000 effluent-1.1/src/effluent.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 08:50:33.854498 effluent-1.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-04-14 08:50:20.000000 effluent-1.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1808 2023-04-14 08:50:33.854498 effluent-1.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2023-04-14 08:50:20.000000 effluent-1.2/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2023-04-14 08:50:20.000000 effluent-1.2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1077 2023-04-14 08:50:33.858497 effluent-1.2/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 08:50:33.846497 effluent-1.2/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 08:50:33.854498 effluent-1.2/src/effluent/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-04-14 08:50:20.000000 effluent-1.2/src/effluent/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-04-14 08:50:20.000000 effluent-1.2/src/effluent/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2975 2023-04-14 08:50:20.000000 effluent-1.2/src/effluent/eos.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14551 2023-04-14 08:50:20.000000 effluent-1.2/src/effluent/io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2408 2023-04-14 08:50:20.000000 effluent-1.2/src/effluent/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1975 2023-04-14 08:50:20.000000 effluent-1.2/src/effluent/numerics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3604 2023-04-14 08:50:20.000000 effluent-1.2/src/effluent/roms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      894 2023-04-14 08:50:20.000000 effluent-1.2/src/effluent/script.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7665 2023-04-14 08:50:20.000000 effluent-1.2/src/effluent/solver.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 08:50:33.854498 effluent-1.2/src/effluent.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1808 2023-04-14 08:50:33.000000 effluent-1.2/src/effluent.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2023-04-14 08:50:33.000000 effluent-1.2/src/effluent.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-14 08:50:33.000000 effluent-1.2/src/effluent.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-04-14 08:50:33.000000 effluent-1.2/src/effluent.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-04-14 08:50:33.000000 effluent-1.2/src/effluent.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 08:50:33.854498 effluent-1.2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2023-04-14 08:50:20.000000 effluent-1.2/tests/test_effluent.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1359 2023-04-14 08:50:20.000000 effluent-1.2/tests/test_eos.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1769 2023-04-14 08:50:20.000000 effluent-1.2/tests/test_examples.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13115 2023-04-14 08:50:20.000000 effluent-1.2/tests/test_io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1060 2023-04-14 08:50:20.000000 effluent-1.2/tests/test_numerics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2023-04-14 08:50:20.000000 effluent-1.2/tests/test_roms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7848 2023-04-14 08:50:20.000000 effluent-1.2/tests/test_solver.py
```

### Comparing `effluent-1.1/LICENSE` & `effluent-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `effluent-1.1/PKG-INFO` & `effluent-1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effluent
-Version: 1.1
+Version: 1.2
 Summary: Simulate effluent discharges from wastewater pipes
 Home-page: https://github.com/pnsaevik/effluent
 Author: Pål Næverlid Sævik
 Author-email: paal.naeverlid.saevik@hi.no
 Project-URL: Documentation, https://effluent.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/pnsaevik/effluent/blob/main/CHANGELOG.md
 Keywords: pipes turbulent jets plumes ocean
@@ -17,17 +17,14 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # effluent
 
-**NOTE**: This package is under development and not all features are
-implemented yet.
-
 Effluent is a python package for simulating the dispersion of effluent
 discharges from wastewater pipes. The underlying model is based on
 Lee, Joseph H. W., and Chu, Vincent H.: *Turbulent Jets and Plumes*.
 Boston, MA: Springer US, 2003.
 [doi:10.1007/978-1-4615-0407-8](https://doi.org/10.1007/978-1-4615-0407-8>).
 
 The package is mainly intended for research purposes, and does not contain
```

### Comparing `effluent-1.1/README.md` & `effluent-1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # effluent
 
-**NOTE**: This package is under development and not all features are
-implemented yet.
-
 Effluent is a python package for simulating the dispersion of effluent
 discharges from wastewater pipes. The underlying model is based on
 Lee, Joseph H. W., and Chu, Vincent H.: *Turbulent Jets and Plumes*.
 Boston, MA: Springer US, 2003.
 [doi:10.1007/978-1-4615-0407-8](https://doi.org/10.1007/978-1-4615-0407-8>).
 
 The package is mainly intended for research purposes, and does not contain
```

### Comparing `effluent-1.1/setup.cfg` & `effluent-1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `effluent-1.1/src/effluent/io.py` & `effluent-1.2/src/effluent/io.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,20 @@
 import abc
 
 import netCDF4 as nc
 import numpy as np
 import pandas as pd
-import tomli as toml
 import xarray as xr
 
 
-def load_config(fname_or_dict):
-    """Load and parse input config, and convert to internal config format"""
-
-    if isinstance(fname_or_dict, dict):
-        input_conf = fname_or_dict
-    else:
-        with open(fname_or_dict, 'rb') as fp:
-            input_conf = toml.load(fp)
-
-    # noinspection PyDictCreation
-    conf = {}
-    conf['pipe'] = input_conf['pipe']
-    conf['ambient'] = input_conf['ambient']
-    conf['output'] = input_conf['output']
-
-    # --- Solver ---
-
-    conf['solver'] = {}
-    # Copy a selection of output parameters
-    for k in ['stagnation', 'resolution']:
-        conf['solver'][k] = input_conf['output'][k]
-    # Copy model parameters
-    for k, v in input_conf.get('model', {}).items():
-        conf['solver'][k] = v
-    # Copy solver parameters
-    for k, v in input_conf.get('solver', {}).items():
-        conf['solver'][k] = v
-
-    # --- Time stepper ---
-
-    conf['timestepper'] = {}
-    conf['timestepper']['frequency'] = input_conf['output']['frequency']
-    conf['timestepper']['stop'] = input_conf['output']['stop']
-
-    return conf
-
-
 class Pipe:
     def __init__(self, dset):
         self._dset = dset
-        self._time_min = dset.time[0].values.item()
-        self._time_max = dset.time[-1].values.item()
+        self._time_min = dset.time[0].values
+        self._time_max = dset.time[-1].values
 
     @staticmethod
     def from_config(conf):
         if 'csv' in conf:
             return Pipe.from_csv_file(**conf['csv'])
         elif 'nc' in conf:
             return Pipe.from_nc_file(**conf['nc'])
@@ -62,121 +24,166 @@
     @staticmethod
     def from_nc_file(file):
         dset = xr.load_dataset(file)
         return Pipe.from_dataset(dset)
 
     @staticmethod
     def from_csv_file(file):
-        df = pd.read_csv(
-            file,
-            sep=',',
-            index_col='time',
-            header=0,
-            skipinitialspace=True,
-            skip_blank_lines=True,
-            comment='#',
-        )
+        df = read_csv(file)
         return Pipe.from_dataframe(df)
 
     @staticmethod
-    def _compute_uw(flow, decline):
+    def _compute_uw(flow, decline, diam):
+        area = np.pi * diam * diam * 0.25
+        speed = flow / area
         theta = decline * np.pi / 180
-        u = flow * np.cos(theta)
-        w = flow * np.sin(theta)
+        u = speed * np.cos(theta)
+        w = speed * np.sin(theta)
         return u, w
 
     @staticmethod
     def from_dataframe(df):
+        df['time'] = df['time'].values.astype('datetime64')
+        df = df.set_index('time')
         dset = xr.Dataset.from_dataframe(df)
         return Pipe.from_dataset(dset)
 
     @staticmethod
     def from_dataset(dset):
-        time = dset.time.values
-        assert np.all(np.diff(time) > 0), "time values must be strictly increasing"
-        u, w = Pipe._compute_uw(dset.flow.values, dset.decline.values)
+        u, w = Pipe._compute_uw(dset.flow.values, dset.decline.values, dset.diam.values)
         dset['u'] = xr.Variable('time', u)
         dset['w'] = xr.Variable('time', w)
+
+        # Compute density from temp and salt if not present
+        if 'dens' not in dset:
+            from . import eos
+            dens = eos.roms_rho(
+                temp=dset['temp'].values,
+                salt=dset['salt'].values,
+                depth=dset['depth'].values,
+            )
+            dset = dset.assign(dens=xr.Variable(dset['temp'].dims, dens))
         return Pipe(dset)
 
     @staticmethod
-    def from_mapping(time, flow, dens, decline, diam, depth):
-        index = pd.Index(data=time, name='time')
-        data = dict(flow=flow, dens=dens, diam=diam, depth=depth, decline=decline)
-        df = pd.DataFrame(data, index=index)
+    def from_mapping(time, flow, decline, diam, depth, dens=None, salt=None, temp=None):
+        data = dict(time=time, flow=flow, diam=diam, depth=depth, decline=decline)
+        if salt is not None:
+            data['salt'] = salt
+        if temp is not None:
+            data['temp'] = temp
+        if dens is not None:
+            data['dens'] = dens
+        df = pd.DataFrame(data)
         return Pipe.from_dataframe(df)
 
     def select(self, time):
+        if self._dset.dims['time'] == 1:
+            # No interpolation is possible if there is only 1 time entry
+            return self._dset.isel(time=0)
+
         clipped_time = np.clip(time, self._time_min, self._time_max)
         return self._dset.interp(time=clipped_time)
 
 
+def read_csv(file):
+    return pd.read_csv(
+        file,
+        sep=',',
+        header=0,
+        skipinitialspace=True,
+        skip_blank_lines=True,
+        comment='#',
+        converters=dict(time=np.datetime64),
+    )
+
+
 class Ambient:
-    def __init__(self, dset):
-        self._dset = dset
-        self._tmin = dset.time[0].values.item()
-        self._tmax = dset.time[-1].values.item()
+    @abc.abstractmethod
+    def select(self, time):
+        return NotImplementedError
 
     @staticmethod
     def from_config(conf):
         if 'csv' in conf:
             return Ambient.from_csv_file(**conf['csv'])
         elif 'nc' in conf:
             return Ambient.from_nc_file(**conf['nc'])
+        elif 'roms' in conf:
+            return AmbientRoms(**conf['roms'])
         else:
             return Ambient.from_mapping(**conf)
 
     @staticmethod
     def from_nc_file(file):
         dset = xr.load_dataset(file)
         return Ambient.from_dataset(dset)
 
     @staticmethod
     def from_dataframe(df):
+        df['time'] = df['time'].values.astype('datetime64')
+        df = df.set_index(['time', 'depth'])
+
         dset = xr.Dataset.from_dataframe(df)
         return Ambient.from_dataset(dset)
 
     @staticmethod
     def from_dataset(dset):
         dset = dset.rename_vars(coflow='u', crossflow='v')
         time = dset.time.values
-        assert np.all(np.diff(time) > 0), "time values must be strictly increasing"
-        return Ambient(dset)
+        assert np.all(np.diff(time).astype('int64') > 0), "time values must be strictly increasing"
+
+        # Compute density from temp and salt if not present
+        if 'dens' not in dset:
+            from . import eos
+            data = eos.roms_rho(
+                temp=dset['temp'].values,
+                salt=dset['salt'].values,
+                depth=dset['depth'].values,
+            )
+            dset = dset.assign(dens=xr.Variable(dset['temp'].dims, data))
+
+        return AmbientXarray(dset)
 
     @staticmethod
     def from_csv_file(file):
-        df = pd.read_csv(
-            file,
-            sep=',',
-            index_col=('time', 'depth'),
-            header=0,
-            skipinitialspace=True,
-            skip_blank_lines=True,
-            comment='#',
-        )
+        df = read_csv(file)
         return Ambient.from_dataframe(df)
 
     @staticmethod
-    def from_mapping(time, depth, coflow, crossflow, dens):
+    def from_mapping(time, depth, coflow, crossflow, dens=None, salt=None, temp=None):
         shp = (len(time), len(depth))
-        u = np.broadcast_to(coflow, shp)
-        v = np.broadcast_to(crossflow, shp)
-        d = np.broadcast_to(dens, shp)
-
-        dset = xr.Dataset(
-            coords=dict(time=time, depth=depth),
-            data_vars=dict(
-                coflow=xr.Variable(('time', 'depth'), u),
-                crossflow=xr.Variable(('time', 'depth'), v),
-                dens=xr.Variable(('time', 'depth'), d),
-            ),
-        )
+
+        variables = dict(coflow=coflow, crossflow=crossflow, dens=dens, salt=salt,
+                         temp=temp)
+
+        dset = xr.Dataset(coords=dict(time=time, depth=depth))
+        for k, v in variables.items():
+            if v is None:
+                continue
+            data = np.broadcast_to(v, shp)
+            dset = dset.assign(**{k: xr.Variable(('time', 'depth'), data)})
+
         return Ambient.from_dataset(dset)
 
+    def close(self):
+        pass
+
+
+class AmbientXarray(Ambient):
+    def __init__(self, dset):
+        self._dset = dset
+        self._tmin = dset.time[0].values
+        self._tmax = dset.time[-1].values
+
     def select(self, time):
+        if self._dset.dims['time'] == 1:
+            # No interpolation is possible if there is only 1 time entry
+            return self._dset.isel(time=0)
+
         clipped_time = np.clip(time, self._tmin, self._tmax)
         return self._dset.interp(time=clipped_time)
 
 
 class Output:
     @staticmethod
     def from_config(conf):
@@ -187,18 +194,23 @@
         else:
             raise ValueError("No output file name given")
 
     @abc.abstractmethod
     def write(self, time, result):
         return NotImplementedError
 
+    def close(self):
+        pass
+
 
 class OutputCSV(Output):
-    def __init__(self, file, variables):
+    def __init__(self, file, variables, float_format, separator):
         self.variables = variables
+        self.float_format = float_format
+        self.separator = separator
         self._blank_file = True
 
         if isinstance(file, str):
             self.file = file
             self.dset = None
 
         elif hasattr(file, 'write') and callable(file.write):
@@ -206,50 +218,57 @@
             self.file = None
             self.dset = file
 
         else:
             raise TypeError(f'Expected file name or stream, found "{type(file)}"')
 
     def __enter__(self):
-        if self.dset is None:
-            self.dset = open(self.file, 'w', encoding='utf-8', newline='\n')
-            self._blank_file = True
+        self.open()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
+    def open(self):
+        if self.dset is None:
+            self.dset = open(self.file, 'w', encoding='utf-8', newline='\n')
+            self._blank_file = True
+
     def close(self):
         if self.dset is not None:
             self.dset.close()
             self.dset = None
 
     @staticmethod
     def from_config(conf):
         out = OutputCSV(
             file=conf['csv']['file'],
-            variables=conf.get('variables', None)
+            variables=conf.get('variables', None),
+            float_format=conf['csv'].get('float_format', '%.10g'),
+            separator=conf.get('separator', ','),
         )
         return out
 
     def write(self, time, result):
+        self.open()  # Lazy opening: Only effective if first time
+
         df = result.to_dataframe()
         df['release_time'] = time
         df = df.reset_index().set_index(['release_time', 't']).reset_index()
 
         # Drop non-output variables
         if self.variables is not None:
             df = df[self.variables]
 
         # Append result to file, write headers only if blank file
         df.to_csv(
             self.dset,
-            line_terminator='\n',
+            lineterminator='\n',
             header=self._blank_file,
-            float_format='%.10g',
+            float_format=self.float_format,
             index=False,
         )
         self._blank_file = False
 
 
 class OutputNC(Output):
     def __init__(self, file, variables):
@@ -269,21 +288,25 @@
             self.diskless = True
             self.xr_dset = file
 
         else:
             raise TypeError(f'Unknown file type: {type(file)}')
 
     def __enter__(self):
-        self.dset = nc.Dataset(filename=self.fname, mode='w', diskless=self.diskless)
-        self._blank_file = True
+        self.open()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
+    def open(self):
+        if self.dset is None:
+            self.dset = nc.Dataset(filename=self.fname, mode='w', diskless=self.diskless)
+            self._blank_file = True
+
     def close(self):
         if self.dset is not None:
             if self.xr_dset is not None:
                 write_nc_to_xr(self.dset, self.xr_dset)
 
             self.dset.close()
             self.dset = None
@@ -293,14 +316,16 @@
         out = OutputNC(
             file=conf['nc']['file'],
             variables=conf.get('variables', None)
         )
         return out
 
     def write(self, time, result):
+        self.open()  # Lazy opening: Only effective if first time
+
         result = result.assign_coords(release_time=time)
         result = result.expand_dims('release_time')
 
         if self._blank_file:
             self._append_attributes(result)
 
         # Drop non-output variables
@@ -400,7 +425,58 @@
     num_items = num_old_items + num_new_items
 
     # Append data
     for name in unlim_vars:
         xr_var = xr_dset[name]
         nc_var = nc_dset.variables[name]
         nc_var[num_old_items:num_items] = xr_var.values
+
+
+class AmbientRoms(Ambient):
+    def __init__(self, file, latitude, longitude, azimuth):
+        self.file = file
+        self.latitude = latitude
+        self.longitude = longitude
+        self.azimuth = azimuth
+
+        self.dset = None
+        self._tmin = None
+        self._tmax = None
+
+    def __enter__(self):
+        self.open()
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
+
+    def __del__(self):
+        self.close()
+
+    def open(self):
+        if self.dset is None:
+            import effluent.roms
+            dset = effluent.roms.open_location(
+                file=self.file,
+                latitude=self.latitude,
+                longitude=self.longitude,
+                azimuth=self.azimuth,
+            )
+
+            keep_vars = ['time', 'depth', 'u', 'v', 'dens']
+            drop_vars = [v for v in dset.variables if v not in keep_vars]
+            dset = dset.drop_vars(drop_vars)
+
+            self.dset = dset
+            self._tmin = dset.time[0].values
+            self._tmax = dset.time[-1].values
+
+    def close(self):
+        if self.dset is not None:
+            self.dset.close()
+            self.dset = None
+
+    def select(self, time):
+        self.open()
+
+        clipped_time = np.clip(time, self._tmin, self._tmax)
+        return self.dset.interp(time=clipped_time)
```

### Comparing `effluent-1.1/src/effluent/solver.py` & `effluent-1.2/src/effluent/solver.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,60 +17,133 @@
         self.method = "RK45"
         self.rtol = 1e-3
         self.atol = 1e-6
         self.first_step = 0
         self.max_step = 0
 
         # Output parameters
-        self.resolution = None
-        self.stagnation = None
-
-        self.data = None
+        self.start = 0
+        self.stop = 60
+        self.step = 1
+
+        self._data = None
+        self._zmin = None
+        self._zmax = None
+
+    @property
+    def data(self):
+        return self._data
+
+    @data.setter
+    def data(self, value):
+        self._data = value
+        ambient = self.data[1]
+        self._zmin = ambient.depth[0].values
+        self._zmax = ambient.depth[-1].values
 
     @staticmethod
     def from_config(conf):
         s = Solver()
         option_names = [
             'beta_n', 'beta_t', 'mass_n', 'mass_t', 'method', 'rtol', 'atol',
-            'first_step', 'max_step', 'resolution', 'stagnation',
+            'first_step', 'max_step', 'start', 'stop', 'step',
         ]
         for k, v in conf.items():
             if k in option_names:
                 setattr(s, k, v)
 
         return s
 
+    def volume_change_ratio(self, t, y):
+        # Rename input variables
+        # noinspection PyUnusedLocal
+        t = t
+        y_in = y
+        x, y, z, u, v, w, rho, R = y_in
+
+        # Define coefficients
+        beta_t = self.beta_t          # Entrainment coefficient, co-flow
+        beta_n = self.beta_n          # Entrainment coefficient, cross-flow
+        K_t = 1 / (1 + self.mass_t)   # Added mass coefficient, tangential gravity pull
+        K_n = 1 / (1 + self.mass_n)   # Added mass coefficient, normal gravity pull
+        g = 9.81                      # Acceleration of gravity
+
+        # Extract ambient velocity and density
+        ambient = self.ambient_data(z)
+        u_a = ambient.u.values
+        v_a = ambient.v.values
+        rho_a = ambient.dens.values
+
+        # Compute added mass coefficient
+        squared_horizontal_speed = u*u + v*v
+        w2 = w*w
+        squared_speed = squared_horizontal_speed + w2
+        K = (K_n * squared_horizontal_speed + K_t * w2) / squared_speed
+
+        # Compute flow difference in tangential and normal direction
+        delta_u = u - u_a
+        delta_v = v - v_a
+        squared_excess_speed = delta_u*delta_u + delta_v*delta_v + w2
+        speed = np.sqrt(squared_speed)
+        delta_u_t = np.abs(speed - (u * u_a + v * v_a) / speed)
+        sq_delta_u_n = squared_excess_speed - delta_u_t * delta_u_t
+        delta_u_n = np.sqrt(np.maximum(0, sq_delta_u_n))
+
+        # Jet expansion rate (entrainment rate)
+        ddt_R = beta_t * delta_u_t + beta_n * delta_u_n
+
+        # Conservation of volume
+        ddt_log_R2 = 2 * ddt_R / R
+        rho_ratio = rho_a / rho
+        gravity_factor = K * (1 - rho_ratio) * g
+        nominator = ddt_log_R2 + gravity_factor * w / squared_speed
+        denominator = rho_ratio * (1 - (u * u_a + v * v_a) / squared_speed) + 1
+        ddt_log_V = nominator / denominator
+
+        return ddt_log_V
+
     def solve(self):
-        steps = np.arange(0, self.stagnation + 0.5 * self.resolution, self.resolution)
+        steps = np.arange(self.start, self.stop + 0.5 * self.step, self.step)
+
+        event = lambda t, y: self.volume_change_ratio(t, y)
+        event.terminal = True
+        event.direction = -1
 
         result = solve_ivp(
             fun=self.odefunc,
             t_span=steps[[0, -1]],
             y0=self.initial_conditions(),
             t_eval=steps,
             vectorized=True,
             method=self.method,
             rtol=self.rtol,
             atol=self.atol,
             first_step=self.first_step or None,
             max_step=self.max_step or np.inf,
+            events=event,
         )
 
         # noinspection PyUnresolvedReferences
-        res_t, res_y = result.t, result.y
+        res_t, res_y, evt_t, evt_y = result.t, result.y, result.t_events, result.y_events
+
+        # Append the end result, if integration was stopped
+        if len(evt_t[0]) > 0:
+            res_t = np.concatenate([res_t, evt_t[0]])
+            res_y = np.concatenate([res_y, evt_y[0].T], axis=1)
 
         # Organize result
         data_vars = {v: xr.Variable('t', res_y[i]) for i, v in enumerate(self.varnames)}
         return xr.Dataset(data_vars=data_vars, coords=dict(t=res_t))
 
     def ambient_data(self, depth):
         ambient = self.data[1]
-        zmin = ambient.depth[0].values
-        zmax = ambient.depth[-1].values
-        clipped_depth = np.clip(depth, zmin, zmax)
+        # Cannot interpolate if there is only one entry
+        if ambient.dims['depth'] == 1:
+            return ambient.isel(depth=0)
+        clipped_depth = np.clip(depth, self._zmin, self._zmax)
         return ambient.interp(depth=clipped_depth)
 
     def pipe_data(self):
         return self.data[0]
 
     def initial_conditions(self):
         pipe = self.pipe_data()
@@ -101,14 +174,15 @@
         x, y, z, u, v, w, rho, R = y_in
 
         # Define coefficients
         beta_t = self.beta_t          # Entrainment coefficient, co-flow
         beta_n = self.beta_n          # Entrainment coefficient, cross-flow
         K_t = 1 / (1 + self.mass_t)   # Added mass coefficient, tangential gravity pull
         K_n = 1 / (1 + self.mass_n)   # Added mass coefficient, normal gravity pull
+        g = 9.81                      # Acceleration of gravity
 
         # Extract ambient velocity and density
         ambient = self.ambient_data(z)
         u_a = ambient.u.values
         v_a = ambient.v.values
         rho_a = ambient.dens.values
 
@@ -134,20 +208,23 @@
 
         # Jet expansion rate (entrainment rate)
         ddt_R = beta_t * delta_u_t + beta_n * delta_u_n
 
         # Conservation of volume
         ddt_log_R2 = 2 * ddt_R / R
         rho_ratio = rho_a / rho
-        ddt_log_V = ddt_log_R2 * u / (u + rho_ratio * delta_u)
+        gravity_factor = K * (1 - rho_ratio) * g
+        nominator = ddt_log_R2 + gravity_factor * w / squared_speed
+        denominator = rho_ratio * (1 - (u * u_a + v * v_a) / squared_speed) + 1
+        ddt_log_V = nominator / denominator
 
         # Conservation of mass
         ddt_rho = ddt_log_V * (rho_a - rho)
 
         # Conservation of momentum
         prefix = -ddt_log_V * rho_ratio
         ddt_u = prefix * delta_u
         ddt_v = prefix * delta_v
-        ddt_w = prefix * w + K * (1 - rho_ratio) * 9.81
+        ddt_w = prefix * w + gravity_factor
 
         ddt_y = np.stack([ddt_x, ddt_y, ddt_z, ddt_u, ddt_v, ddt_w, ddt_rho, ddt_R])
         return ddt_y
```

### Comparing `effluent-1.1/src/effluent/utils.py` & `effluent-1.2/src/effluent/numerics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,10 @@
 import numpy as np
 
 
-def xr_to_csv(dset, csv_stream):
-    df = dset.to_dataframe()
-    df.to_csv(csv_stream, line_terminator='\n')
-
-
-def csv_to_xr(csv_stream, index_cols):
-    import pandas as pd
-    import xarray as xr
-
-    df = pd.read_csv(csv_stream, index_col=index_cols)
-    dset = xr.Dataset.from_dataframe(df)
-    return dset
-
-
 def bilin_inv(f, g, F, G, maxiter=7, tol=1.0e-7):
     """Inverse bilinear interpolation
 
     f, g : scalars or arrays of same shape
     F, G : 2D arrays of the same shape
 
     returns x, y : shaped like f and g
```

### Comparing `effluent-1.1/src/effluent.egg-info/PKG-INFO` & `effluent-1.2/src/effluent.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effluent
-Version: 1.1
+Version: 1.2
 Summary: Simulate effluent discharges from wastewater pipes
 Home-page: https://github.com/pnsaevik/effluent
 Author: Pål Næverlid Sævik
 Author-email: paal.naeverlid.saevik@hi.no
 Project-URL: Documentation, https://effluent.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/pnsaevik/effluent/blob/main/CHANGELOG.md
 Keywords: pipes turbulent jets plumes ocean
@@ -17,17 +17,14 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # effluent
 
-**NOTE**: This package is under development and not all features are
-implemented yet.
-
 Effluent is a python package for simulating the dispersion of effluent
 discharges from wastewater pipes. The underlying model is based on
 Lee, Joseph H. W., and Chu, Vincent H.: *Turbulent Jets and Plumes*.
 Boston, MA: Springer US, 2003.
 [doi:10.1007/978-1-4615-0407-8](https://doi.org/10.1007/978-1-4615-0407-8>).
 
 The package is mainly intended for research purposes, and does not contain
```

