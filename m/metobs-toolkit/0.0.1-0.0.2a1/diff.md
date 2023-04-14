# Comparing `tmp/metobs_toolkit-0.0.1.tar.gz` & `tmp/metobs_toolkit-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metobs_toolkit-0.0.1.tar", max compression
+gzip compressed data, was "metobs_toolkit-0.0.2a1.tar", max compression
```

## Comparing `metobs_toolkit-0.0.1.tar` & `metobs_toolkit-0.0.2a1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1074 2022-09-22 07:29:20.660989 metobs_toolkit-0.0.1/LICENSE
--rw-r--r--   0        0        0     1307 2023-04-13 14:10:35.608176 metobs_toolkit-0.0.1/README.md
--rw-r--r--   0        0        0     1030 2023-04-13 14:47:55.332214 metobs_toolkit-0.0.1/metobs_toolkit/__init__.py
--rw-r--r--   0        0        0     2596 2023-04-13 14:10:35.612176 metobs_toolkit-0.0.1/metobs_toolkit/convertors.py
--rw-r--r--   0        0        0    11411 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/data_import.py
--rw-r--r--   0        0        0     3066 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/data_templates/db_templates.py
--rw-r--r--   0        0        0     1435 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/data_templates/import_templates.py
--rw-r--r--   0        0        0      931 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/data_templates/template_defaults/default_template.csv
--rw-r--r--   0        0        0    50192 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/dataset.py
--rw-r--r--   0        0        0     6522 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/df_helpers.py
--rw-r--r--   0        0        0    22588 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/gap.py
--rw-r--r--   0        0        0    14894 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/gap_filling.py
--rw-r--r--   0        0        0      686 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/geometry_functions.py
--rw-r--r--   0        0        0    18373 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/landcover_functions.py
--rw-r--r--   0        0        0     3884 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/missingobs.py
--rw-r--r--   0        0        0     4950 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/modeldata.py
--rw-r--r--   0        0        0    14086 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/plotting_functions.py
--rw-r--r--   0        0        0     1587 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/printing.py
--rw-r--r--   0        0        0    23064 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/qc_checks.py
--rw-r--r--   0        0        0     3381 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/qc_statistics.py
--rw-r--r--   0        0        0    12958 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/settings.py
--rw-r--r--   0        0        0       73 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/settings_files/app_print_settings.json
--rw-r--r--   0        0        0      114 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/settings_files/dataset_resolution_settings.json
--rw-r--r--   0        0        0     4176 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/settings_files/default_formats_settings.py
--rw-r--r--   0        0        0     1567 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/settings_files/gaps_settings.py
--rw-r--r--   0        0        0     4823 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/settings_files/gee_settings.py
--rw-r--r--   0        0        0     3982 2023-04-13 14:10:35.616176 metobs_toolkit-0.0.1/metobs_toolkit/settings_files/qc_settings.py
--rw-r--r--   0        0        0      132 2023-03-15 07:36:53.806317 metobs_toolkit-0.0.1/metobs_toolkit/settings_files/server_login.json
--rw-r--r--   0        0        0  8385556 2023-04-13 14:10:35.676176 metobs_toolkit-0.0.1/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp
--rw-r--r--   0        0        0     2108 2023-04-13 14:10:35.676176 metobs_toolkit-0.0.1/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx
--rw-r--r--   0        0        0     2599 2023-04-13 14:10:35.676176 metobs_toolkit-0.0.1/metobs_toolkit/writing_files.py
--rw-r--r--   0        0        0      832 2023-04-13 14:45:45.260212 metobs_toolkit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 metobs_toolkit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-09-22 07:29:20.660989 metobs_toolkit-0.0.2a1/LICENSE
+-rw-r--r--   0        0        0      403 2023-04-14 14:06:24.419816 metobs_toolkit-0.0.2a1/README.md
+-rw-r--r--   0        0        0     1032 2023-04-14 14:41:28.643473 metobs_toolkit-0.0.2a1/metobs_toolkit/__init__.py
+-rw-r--r--   0        0        0     2596 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/convertors.py
+-rw-r--r--   0        0        0    11411 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/data_import.py
+-rw-r--r--   0        0        0     3066 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/data_templates/db_templates.py
+-rw-r--r--   0        0        0     1435 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/data_templates/import_templates.py
+-rw-r--r--   0        0        0      931 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/data_templates/template_defaults/default_template.csv
+-rw-r--r--   0        0        0    51034 2023-04-14 14:28:43.809424 metobs_toolkit-0.0.2a1/metobs_toolkit/dataset.py
+-rw-r--r--   0        0        0     6522 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/df_helpers.py
+-rw-r--r--   0        0        0    22588 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/gap.py
+-rw-r--r--   0        0        0    14894 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/gap_filling.py
+-rw-r--r--   0        0        0      686 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/geometry_functions.py
+-rw-r--r--   0        0        0    18373 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/landcover_functions.py
+-rw-r--r--   0        0        0     3884 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/missingobs.py
+-rw-r--r--   0        0        0     4950 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/modeldata.py
+-rw-r--r--   0        0        0    14086 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/plotting_functions.py
+-rw-r--r--   0        0        0     1587 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/printing.py
+-rw-r--r--   0        0        0    23064 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/qc_checks.py
+-rw-r--r--   0        0        0     3381 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/qc_statistics.py
+-rw-r--r--   0        0        0    13092 2023-04-14 14:21:45.347574 metobs_toolkit-0.0.2a1/metobs_toolkit/settings.py
+-rw-r--r--   0        0        0       73 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/app_print_settings.json
+-rw-r--r--   0        0        0      114 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/dataset_resolution_settings.json
+-rw-r--r--   0        0        0     4182 2023-04-14 14:20:24.511222 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/default_formats_settings.py
+-rw-r--r--   0        0        0     1567 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/gaps_settings.py
+-rw-r--r--   0        0        0     4823 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/gee_settings.py
+-rw-r--r--   0        0        0     3982 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/qc_settings.py
+-rw-r--r--   0        0        0      132 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/server_login.json
+-rw-r--r--   0        0        0  8385556 2023-04-14 14:06:24.563817 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp
+-rw-r--r--   0        0        0     2108 2023-04-14 14:06:24.563817 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx
+-rw-r--r--   0        0        0     2599 2023-04-14 14:06:24.563817 metobs_toolkit-0.0.2a1/metobs_toolkit/writing_files.py
+-rw-r--r--   0        0        0      834 2023-04-14 14:41:28.563471 metobs_toolkit-0.0.2a1/pyproject.toml
+-rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 metobs_toolkit-0.0.2a1/PKG-INFO
```

### Comparing `metobs_toolkit-0.0.1/LICENSE` & `metobs_toolkit-0.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/__init__.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,9 +31,9 @@
 sys.path.append(BASE_PATH)
 
 
 from metobs_toolkit.dataset import Dataset
 from metobs_toolkit.modeldata import Modeldata
 
 #DO not change this manually!
-__version__="0.0.1"
+__version__="0.0.2a1"
```

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/convertors.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/convertors.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/data_import.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/data_import.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/data_templates/db_templates.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/data_templates/db_templates.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/data_templates/import_templates.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/data_templates/import_templates.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/data_templates/template_defaults/default_template.csv` & `metobs_toolkit-0.0.2a1/metobs_toolkit/data_templates/template_defaults/default_template.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/dataset.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,28 @@
         :param timezonestr: Timezone string of the input observations.
         :type timezonestr: String
         :return: None
         :rtype: None
         """
         self.settings.update_timezone(timezonestr)
 
+    def update_default_name(self, default_name):
+        """
+        Update the default name (the name of the station). This name will be
+        used when no names are found in the observational dataset.
+
+        (All observations are assumed to come from one station.)
+
+        :param default_name: Default name to use when no names are present in the data.
+        :type default_name: String
+        :return: None
+        :rtype: None
+
+        """
+        self.settings.app['default_name'] = str(default_name)
 
     def show_settings(self):
         """
         A function that prints out all the settings, structured per thematic.
         :return: No return
         :rtype: No return
 
@@ -969,14 +983,20 @@
 
         logger.debug(f'Data from {self.settings.IO["input_data_file"]} \
                      imported to dataframe.')
 
         # drop Nat datetimes if present
         df = df.loc[pd.notnull(df.index)]
 
+        if not 'name' in df.columns:
+            logger.warning(f'No station names find in the observations! \
+                           Assume the dataset is for ONE station with the \
+                         default name: {self.settings.app["default_name"]}.')
+            df['name'] =str(self.settings.app["default_name"])
+
         if isinstance(self.settings.IO['input_metadata_file'], type(None)):
             print('WARNING: No metadata file is defined.\
                   Add your settings object.')
             logger.warning('No metadata file is defined,\
                     no metadata attributes can be set!')
         else:
             logger.info(f'Importing metadata from file:\
```

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/df_helpers.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/df_helpers.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/gap.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/gap.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/gap_filling.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/gap_filling.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/geometry_functions.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/geometry_functions.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/landcover_functions.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/landcover_functions.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/missingobs.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/missingobs.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/modeldata.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/modeldata.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/plotting_functions.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/plotting_functions.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/printing.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/printing.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/qc_checks.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/qc_checks.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/qc_statistics.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/qc_statistics.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/settings.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     def _update_app_settings(self):
         """
         Update prefered display, print, plot and staticinfo settings of self using the default settings templates.
         :return: No return
         :rtype: No return
         """
         logger.debug('Updating app settings.')
-        from .settings_files.default_formats_settings import plot_settings, print_settings, vars_display
+        from .settings_files.default_formats_settings import plot_settings, print_settings, vars_display, default_name
         from .settings_files.default_formats_settings import static_fields, categorical_fields, observation_types, location_info
 
         # 1. Print settings
         self.app['print_fmt_datetime'] = print_settings['fmt_datetime']
         self.app['print_max_n'] = int(print_settings["max_print_per_line"])
         # 2. Plot settings
         self.app['plot_settings'] = plot_settings
@@ -121,14 +121,17 @@
         # fields without timeevolution
         self.app['static_fields'] = static_fields
         self.app['categorical_fields'] = categorical_fields  # wind and lcz
         # order of all possible observations
         self.app['observation_types'] = observation_types
         self.app['location_info'] = location_info  # all possible metadata
 
+        #5. default name (when station name is not present in dataset)
+        self.app['default_name'] = default_name
+
     def _update_qc_settings(self):
         """
         Update quality control settings of self using the default settings templates.
         :return: No return
         :rtype: No return
         """
         logger.debug('Updating QC settings.')
```

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/settings_files/default_formats_settings.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/default_formats_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # =============================================================================
 
 # =============================================================================
 # Default obs and metadata settings
 # =============================================================================
 
 #Static fields are fields (attributes and observations) that do not change in time
-static_fields = ['network', 'name', 
-                'lat', 'lon', #TODO make these dynamic, now used as static 
+static_fields = ['network', 'name',
+                'lat', 'lon', #TODO make these dynamic, now used as static
                 'call_name', 'location',
                 'lcz']
 
 #Categorical fields are fields with values that are assumed to be categorical.
 #Note: (there are static and dynamic fields that are categorical)
 categorical_fields = ['wind_direction', 'lcz']
 
@@ -30,49 +30,49 @@
 observation_types = ['temp', 'radiation_temp', 'humidity', 'precip',
                      'precip_sum', 'wind_speed', 'wind_gust', 'wind_direction',
                      'pressure', 'pressure_at_sea_level']
 
 location_info = ['network', 'lat', 'lon', 'lcz', 'call_name', 'location' ]
 
 
-
+default_name = 'unknown_name' #used when no station names are available
 
 # =============================================================================
 # Timeseries plots
 # =============================================================================
 plot_settings['time_series'] = {
-    
+
     #shape
     'figsize' : (10,5),
     'linewidth': 2, #
     'linezorder': 1, #for ok obs
     'scattersize': 4, #for outliers
     'scatterzorder': 2, #for outliers
-    'dashedzorder': 2, #for gapfills 
-    
+    'dashedzorder': 2, #for gapfills
+
     }
 # =============================================================================
 # Spatial plot settings
 # =============================================================================
 
 plot_settings['spatial_geo'] = {
     #projection
     # 'proj' : 'Orthographic', #Orthographic or AlbersEqualArea
     'extent' : [ 2.260609, 49.25,  6.118359, 52.350618], #used if observatioons are within
-    
+
     #colors
     # 'cmap' : 'Set1',
     'cmap' : 'inferno_r',
-    'n_for_categorical' : 5, #number of quantiles for cat data (not for LCZ) 
-    
+    'n_for_categorical' : 5, #number of quantiles for cat data (not for LCZ)
+
     #shape
     'figsize': (10,15),
-    
+
     #datetime
-    'fmt': "%d/%m/%Y %H:%M:%S UTC" 
+    'fmt': "%d/%m/%Y %H:%M:%S UTC"
     }
 
 # =============================================================================
 # Stats plot settings
 # =============================================================================
 
 plot_settings['pie_charts'] = {
@@ -90,31 +90,31 @@
     'duplicated_timestamp': '#a32a1f',
     'invalid_input': '#900357',
     'gross_value': '#f1ff2b',
     'persistance':'#f0051c',
     'repetitions':'#056ff0',
     'step':'#05d4f0',
     'window_variation':'#05f0c9',
-    
+
     #missing and gap
     'gap': '#f00592',
     'missing_timestamp':'#e86bb6',
-    
+
     #Gap filling
     'linear': '#d406c6',
     'model_debias': '#6e1868',
 
-    
+
     #common
     'ok': '#07f72b',
     'not checked': '#f7cf07',
-    
+
     #Aggregated
     'outlier': '#f20000'
-    
+
     }
 
 
 
 
 print_settings = {
     "fmt_datetime":"%d/%m/%Y %H:%M:%S",
@@ -126,26 +126,26 @@
 # variables display strings
 # =============================================================================
 vars_display = {
     'network': 'network',
     'name': 'station name',
     'call_name': 'pseudo name',
     'location': 'region',
-    
-    
+
+
     'lat': 'latitude',
     'lon': 'longtitude',
-    
+
     'temp': 'temperature',
     'radiation_temp': 'radiation temperature',
     'humidity': 'humidity',
     'precip': 'precipitation intensity',
     'precip_sum': 'cummulated precipitation',
     'wind_speed': 'wind speed',
     'wind_gust': 'wind gust speed',
     'wind_direction': 'wind direction',
     'pressure': 'air pressure',
     'pressure_at_sea_level': 'corrected pressure at sea level',
-    
+
     'lcz':'LCZ'
-    
+
     }
```

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/settings_files/gaps_settings.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/gaps_settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/settings_files/gee_settings.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/gee_settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/settings_files/qc_settings.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/qc_settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp` & `metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx` & `metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/metobs_toolkit/writing_files.py` & `metobs_toolkit-0.0.2a1/metobs_toolkit/writing_files.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.1/pyproject.toml` & `metobs_toolkit-0.0.2a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MetObs-toolkit"
-version = "0.0.1"
+version = "0.0.2a1"
 description = "A Meteorological observations toolkit for scientists"
 authors = ["Thomas Vergauwen <thomas.vergauwen@meteo.be>"]
 maintainers = ["Thomas Vergauwen <thomas.vergauwen@meteo.be>"]
 license = "LICENSE"
 readme = "README.md"
 documentation = "https://python-poetry.org/docs/"
 packages = [{include = "metobs_toolkit"}]
```

### Comparing `metobs_toolkit-0.0.1/PKG-INFO` & `metobs_toolkit-0.0.2a1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metobs-toolkit
-Version: 0.0.1
+Version: 0.0.2a1
 Summary: A Meteorological observations toolkit for scientists
 License: LICENSE
 Keywords: meteorology,observations,urban climate
 Author: Thomas Vergauwen
 Author-email: thomas.vergauwen@meteo.be
 Maintainer: Thomas Vergauwen
 Maintainer-email: thomas.vergauwen@meteo.be
@@ -26,31 +26,14 @@
 Description-Content-Type: text/markdown
 
 # MetObs-toolkit
 
 This repo contains all the software for the [metobs_toolkit](https://test.pypi.org/project/metobs-toolkit/).
 The MetObs-toolkit is a package for scientists who make use meteorological observations.
 ## Documentation ##
-Documentation can be found [here](https://vergauwenthomas.github.io/vlinder_toolkit/).
+Documentation can be found [here](https://vergauwenthomas.github.io/MetObs_toolkit/).
 
 ## Installing the package
 Install the package by:
 
-`pip3 install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple metobs_toolkit --upgrade`
-
-
-### Using the database
-In order to use the database for importing data, you need to have an active VPN connection with the UGent network or working from within the UGent network.
-In addition you need a specific **USER** and **PASSWORD** to connect with the database. (Contact thomas.vergauwen@meteo.be for this account).
-
-To give the user and password to the vlinder toolkit, you need to set them as envrionment variables:
-(on linux execute in terminal (or better add them in  `.bashrc`:)
-
- `     export VLINDER_DB_USER_NAME="...."` (no spaces, fill in the username for the Database)
-
-
- `     export VLINDER_DB_USER_PASW="...."` (no spaces, fill in the password for the Database)
-
-
- # Overview
- ![alt text](https://github.com/vergauwenthomas/vlinder_toolkit/blob/master/examples/overview_fig.png?raw=true)
+`pip install metobs-toolkit`
```

