# Comparing `tmp/pyroscope_gridtools-0.0.3.tar.gz` & `tmp/Pyroscope-gridtools-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroscope_gridtools-0.0.3.tar", last modified: Fri Apr 14 15:10:13 2023, max compression
+gzip compressed data, was "dist/Pyroscope-gridtools-0.1.tar", last modified: Thu Apr  6 23:23:40 2023, max compression
```

## Comparing `pyroscope_gridtools-0.0.3.tar` & `Pyroscope-gridtools-0.1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 15:10:13.906706 pyroscope_gridtools-0.0.3/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      775 2023-04-14 15:10:13.900699 pyroscope_gridtools-0.0.3/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscope_gridtools-0.0.3/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 15:10:13.699459 pyroscope_gridtools-0.0.3/pyroscope_gridtools/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2022-02-04 10:40:28.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     2636 2023-04-14 14:22:50.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10387 2023-04-14 14:22:50.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33637 2023-04-14 14:32:01.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10462 2023-04-14 14:22:50.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26242 2023-04-14 15:03:08.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9309 2023-04-14 14:25:01.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10932 2023-04-14 14:22:50.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     4779 2023-04-14 14:22:50.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 15:10:13.871013 pyroscope_gridtools-0.0.3/pyroscope_gridtools.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      775 2023-04-14 15:10:13.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      622 2023-04-14 15:10:13.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-14 15:10:13.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       73 2023-04-14 15:10:13.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       57 2023-04-14 15:10:13.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       20 2023-04-14 15:10:13.000000 pyroscope_gridtools-0.0.3/pyroscope_gridtools.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-14 15:10:13.908572 pyroscope_gridtools-0.0.3/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1789 2023-04-14 15:10:04.000000 pyroscope_gridtools-0.0.3/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-06 23:23:40.200537 Pyroscope-gridtools-0.1/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-06 23:23:40.191071 Pyroscope-gridtools-0.1/PKG-INFO
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-06 23:23:39.975088 Pyroscope-gridtools-0.1/Pyroscope-gridtools/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2022-02-04 10:40:28.000000 Pyroscope-gridtools-0.1/Pyroscope-gridtools/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     2106 2023-04-06 22:27:16.000000 Pyroscope-gridtools-0.1/Pyroscope-gridtools/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     6434 2023-04-06 22:28:48.000000 Pyroscope-gridtools-0.1/Pyroscope-gridtools/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    28897 2023-04-06 22:47:52.000000 Pyroscope-gridtools-0.1/Pyroscope-gridtools/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10251 2023-04-06 23:12:45.000000 Pyroscope-gridtools-0.1/Pyroscope-gridtools/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26095 2023-04-06 22:47:32.000000 Pyroscope-gridtools-0.1/Pyroscope-gridtools/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     8250 2023-04-06 22:40:51.000000 Pyroscope-gridtools-0.1/Pyroscope-gridtools/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     8107 2023-04-06 23:14:16.000000 Pyroscope-gridtools-0.1/Pyroscope-gridtools/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     7531 2023-04-06 23:14:29.000000 Pyroscope-gridtools-0.1/Pyroscope-gridtools/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3166 2023-04-06 22:45:00.000000 Pyroscope-gridtools-0.1/Pyroscope-gridtools/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-06 23:23:40.155487 Pyroscope-gridtools-0.1/Pyroscope_gridtools.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-06 23:23:38.000000 Pyroscope-gridtools-0.1/Pyroscope_gridtools.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      576 2023-04-06 23:23:39.000000 Pyroscope-gridtools-0.1/Pyroscope_gridtools.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-06 23:23:38.000000 Pyroscope-gridtools-0.1/Pyroscope_gridtools.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       57 2023-04-06 23:23:38.000000 Pyroscope-gridtools-0.1/Pyroscope_gridtools.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       20 2023-04-06 23:23:38.000000 Pyroscope-gridtools-0.1/Pyroscope_gridtools.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 Pyroscope-gridtools-0.1/README.md
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-06 23:23:40.203396 Pyroscope-gridtools-0.1/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1614 2023-04-06 23:23:23.000000 Pyroscope-gridtools-0.1/setup.py
```

### Comparing `pyroscope_gridtools-0.0.3/PKG-INFO` & `Pyroscope-gridtools-0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: pyroscope_gridtools
-Version: 0.0.3
+Name: Pyroscope-gridtools
+Version: 0.1
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscope_gridtools-0.0.3/README.md` & `Pyroscope-gridtools-0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyroscope_gridtools-0.0.3/pyroscope_gridtools/fileparser.py` & `Pyroscope-gridtools-0.1/Pyroscope-gridtools/fileparser.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 # given path to text file contaings paths to files to read read out as list of files within
 def read_file_sat_data(fileloc):
     lines = []
 
     with open(fileloc) as f:
         lines = [line.rstrip('\n') for line in f]
 
-    #print(lines)
     return lines
 
 # given folder path with files inside, read out list of files within
 def read_folder_sat_data(folderloc):
     files = os.listdir(folderloc)
     lines = [folderloc+"/"+f for f in files]
     
@@ -49,40 +48,24 @@
 
     geo_list = cmds[7].split(" ")
     phy_list = cmds[8].split(" ")
 
     return filelist, gsize, time_interval, start, end, output, geo_list, phy_list
 
 def read_config(yfile):
-    #print("FILE: ", yfile)
-    #print("OS: ", os.getcwd())
     with open(yfile, "r") as yamlfile:
         data = yaml.load(yamlfile, Loader=yaml.FullLoader)
 
     grid_settings = data["grid_settings"]
     variables = data["variables"]
     file_io = data["file_io"]
 
-    #print(grid_settings)
-    #print(variables)
-    #print(file_io)
-
     return grid_settings, variables, file_io
 
 def read_directory_sat_data(path):
     f = []
     filelist = []
     for (dirpath, dirnames, filenames) in walk(path):
-        #print(dirpath)
-        #print(dirnames)
-        #print(filenames)
         filenames_path = [dirpath+"/"+f if dirpath[-1]!="/" else dirpath+f for f in filenames]
         filelist = filelist + filenames_path
         
     return filelist
-
-if __name__ == '__main__':
-    path = "/mnt/c/Users/bobgr/Desktop/NASA Spring 2023/Gridtools Package (Code, README, inputs, outputs, examples, verification)/"
-    folder = "LAADSemulation/"
-    f = read_directory_sat_data(path+folder)
-    f = read_folder_sat_data(path+folder)
-    print(f)
```

### Comparing `pyroscope_gridtools-0.0.3/pyroscope_gridtools/grid_ncf.py` & `Pyroscope-gridtools-0.1/Pyroscope-gridtools/grid_ncf.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 import gridding
 import sat_data_input
 import filter_data
 import naming_conventions
 import solar_zenith
 import datetime
 
+import logging
+
 # full satellite list 
 # used to check if any satellites are missing
-#full_satellite_list = ['AERDT_L2_ABI_G16', 'AERDT_L2_ABI_G17', 'AERDT_L2_AHI_H08', 'AERDT_L2_VIIRS_SNPP', 'MOD04_L2', 'MYD04_L2']
-full_satellite_list = ['ABI_G16', 'ABI_G17', 'AHI_H08', 'VIIRS_SNPP', 'MOD04', 'MYD04']
-
+full_satellite_list = ['AERDT_L2_ABI_G16', 'AERDT_L2_ABI_G17', 'AERDT_L2_AHI_H08', 'AERDT_L2_VIIRS_SNPP', 'MOD04_L2', 'MYD04_L2']
 
 # takes in dictionary 
 # keys are satellite names, values = array of filepaths
 # returns 1D array of satellite file inputs
 def sat_list_name_concat(file_list):
     file_inputs = []
     
@@ -65,16 +65,14 @@
     maxlat=float(limit[1])
     minlon=float(limit[2])
     maxlon=float(limit[3])
     
     # pixel dimensions
     lat_dim = int(1+round(((maxlat-minlat)/gsize))) #int(1+round(((maxlat-minlat)/gsize)))
     lon_dim = int(1+round(((maxlon-minlon)/gsize))) #int(1+round(((maxlon-minlon)/gsize)))
-    print("LAT:" ,lat_dim)
-    print("LON:" ,lon_dim)
     
     #set target netcdf file
     ds = netCDF4.Dataset(filename, 'w',format='NETCDF4')
     
     #start_timer = time.time()
     time_date = time_start.strftime('%Y-%m-%d')
     time_time = time_start.strftime('%H:%M:%S.%f')[:-4]
@@ -188,81 +186,60 @@
         for name, dimension in src.dimensions.items():
             ds.createDimension(
                 name, (len(dimension) if not dimension.isunlimited() else None))
         """
         # copy all file data in the specified variables
         for name, variable in src.variables.items():
             if name in static_vars:
-                print(name)
                 dimensions = ('time', 'lat', 'lon',)
                 x = ds.createVariable(name, variable.datatype, dimensions) #variable.dimensions)
                 #ds[name][:] = src[name][:]
                 ds[name][0, :, :] = src[name][:]
-                #print(ds[name][:])
                 # copy variable attributes all at once via dictionary
                 ds[name].setncatts(src[name].__dict__)
                 
                 # add manual metadata
                 if name == "Topographic_Altitude":
                     ds[name].long_name = "Averaged topographic altitude (in km) for Land"
                     ds[name].units = "km"
                 else:
                     ds[name].long_name = "Land_Sea_Flag (based on MOD03 Landsea mask 0 = Ocean, 1 = Land and ephemeral water 2 = Coastal)"
                     
         src.close()
     
-    print("Done with static file transfer")
+    logging.info("Static file transfer complete")
     
     # Solar zenith angle 
     name = "Solar_Zenith_Angle"
     solar_zenith_variable = ds.createVariable(name, 'f4', ('time', 'lat', 'lon', ), fill_value=int(-9999))
     solar_zenith_variable.long_name = "Solar Zenith Angle at the center of grid calculated for central time of the file"
     solar_zenith_variable.units = "degree"
     solar_zenith_variable.valid_range = [ 0, 18000]
     solar_zenith_variable.scale_factor = 0.01
     solar_zenith_variable.add_offset = float(0)
     #netCDF4.nc_put_att(ds, solar_zenith_variable, 'add_offset', 'f4', 1, 0)
     
     solar_zenith_variable[0, :, :] = solar_zenith.get_SZA_parallelized(limit, gsize, time_start, time_diff)
     #copy solar_zenith
     
+    logging.info("Solar zenith calculations complete")
     
-    #path = "/mnt/c/Users/bobgr/Desktop/NASA Spring 2023/Gridtools Package (Code, README, inputs, outputs, examples, verification)/"
-    #fn = path + "SampleOutputs 0000-0059 01-01-2020/XAERDT_L3_MEASURES_QD_HH.20200101.0000.V0.20230307.nc"
-    #src = netCDF4.Dataset(fn)
-    #for name, variable in src.variables.items():
-    #    if name == "Solar_Zenith_Angle":
-    #        print("metadata: ", src[name].__dict__)
-    #solar_zenith_variable[0, :, :] = src["Solar_Zenith_Angle"][:]
-    #src.close()
-    
-    
-    print("solar zenith done")
     # for calculating LEOGEO statistics
     # LEOGEO: Mean, STD, NumberOfSensors, SensorWeighting, TotalPixels
     # index of value corresponds to individual sensor
     #leogeo_stats = {"Mean": [], "STD": [], "TotalPixels":[]}
     leogeo_stats_arr = {} #contains leogeo_stats as value, geophys as key
     #sensor_idx_stats = {"NumberOfSensors":[], "SensorWeighting":[]}
     #sensor_idx = {} #key = sensor name, value = sensoridx
     sensor_idx_arr = {} #key = geophys value, value = sensor_idx
     
     # instantiate the satellites that are not present
     # no inputs for these satellites, blank data for their netCDF4 output variables
     
-    #not_present_satellites = [s for s in full_satellite_list if s not in list(filelist.keys())]
-    
-    # accounts for abbreviations
-    present_satellites = []
-    for s in full_satellite_list: #check all satellites
-        for present_s in list(filelist.keys()):
-            if s in present_s: #satellite is present
-                present_satellites.append(s)
-                
-    not_present_satellites = [s for s in full_satellite_list if s not in present_satellites]
+    not_present_satellites = [s for s in full_satellite_list if s not in list(filelist.keys())]
     
     for s_name in not_present_satellites: 
         for j, p_vars in enumerate(phy_list):
             if not("Sensor_Zenith" in p_vars or "Scattering_Angle" in p_vars):
                 aod_statistics = ["Mean", "STD", "Pixels"]
                 
                 for aod_stat in aod_statistics:
@@ -281,15 +258,15 @@
     # filenames are in the form:
     # [[time0: [sat1], [sat2], ... ], ...[timek: [sat1], [sat2], ....]] 
     # we assume we receive a signle dict for a time interval though
     for i, s_name in enumerate(filelist.keys()): 
         start_timer = time.time()
 
         for s in filelist.get(s_name):
-            print("WORK SENSOR: ", s_name)
+            logging.info("Current sensor calculations: ", s_name)
 
             L2FID,GeoID,PhyID = sat_data_input.open_file(str(s))
 
             # check for hdf files 
             if (str(s).split(".")[-1] == "hdf"):
                 geo_list = ['Latitude', 'Longitude']
                 lat,lon,phy_vars, meta = filter_data.filter_data_hdf(GeoID, PhyID, geo_list, phy_list, phy_hdf)
@@ -367,91 +344,74 @@
                         sensors[p_vars] = []
                     
                     if not p_vars in sensor_idx_arr:
                         sensor_idx_arr[p_vars] = {}
                     
                     #statistics to be added
                     if aod_stat== "Mean":
-                        rotated = list(zip(*avgtau))[::-1] # check why zipped
-                        #print("AFTER GRIDDING: ", rotated)
+                        rotated = list(zip(*avgtau))[::-1] 
                         leogeo_stats_arr[p_vars] ["Mean"].append(np.flipud(rotated)) #for leogeo calculation later
                         
                         #sensor idx (Sensor Weighting)
                         temp_a = np.flipud(rotated)
-                        """
-                        print("\nBEFORE SENSOR IDX \n")
-                        print(temp_a)
-                        print("Fill Value: ", meta[j]["_FillValue"])"""
+                        
                         temp_a[temp_a > -9999] = 1
                         temp_a[temp_a <= meta[j]["_FillValue"]] = 0 #get rid of this 2/1
                         temp_a[np.isnan(temp_a)] = 0
                         #sensor_idx[naming_conventions.get_sensor(s_name)] = temp_a
                         sensor_idx_arr[p_vars][naming_conventions.get_sensor(s_name)] = temp_a
-                        """
-                        print("\nSENSOR IDX\n")
-                        print(sensor_idx[naming_conventions.get_sensor(s_name)])
-                        print("\n")
-                        """
+                        
                     
                          
                     elif aod_stat == "STD":
                         rotated = list(zip(*stdtau))[::-1]
                         
                         leogeo_stats_arr[p_vars]["STD"].append(np.flipud(rotated))
-                        #print("AOD STD", rotated)
-                        
+                                                
                         #leogeo_stats["STD"].append(np.flipud(rotated)) #for leogeo calculation later
                     elif aod_stat == "Pixels":
                         rotated = list(zip(*count))[::-1]
                         
                         leogeo_stats_arr[p_vars]["TotalPixels"].append(np.flipud(rotated))
                         #leogeo_stats["TotalPixels"].append(np.flipud(rotated)) #for leogeo calculation later
                     else:
                         rotated = list(zip(*avgtau))[::-1]
                         
                         leogeo_stats_arr[p_vars]["Mean"].append(np.flipud(rotated))
                         #leogeo_stats["Mean"].append(np.flipud(rotated)) #for leogeo calculation later
-                        print("STATISTIC ERROR")
+                        logging.exception("Statistic Exception: Unknown statistic")
+                    
+                    logging.info("Calculated value for ", aod_stat, ":", np.flipud(rotated))
                     
-                    print("ROTATED AOD for", aod_stat)
-                    #print(np.flipud(rotated))
                     
                     #manually set to fill_value
                     rotated = np.array(rotated)
-                    print("VALID RANGE:", meta[j]["valid_range"][0], " TO ", meta[j]["valid_range"][1])
                     rotated[rotated > meta[j]["valid_range"][1]+1] = -800#meta[j]["_FillValue"]
                     rotated[rotated < meta[j]["valid_range"][0]-1] = -800 #meta[j]["_FillValue"]
                     
                     final_input = np.flipud(rotated)#.astype(np.short)
                     final_input = final_input #/meta[j]["scale_factor"]
-                    print(final_input)
                     #curr_sensor_value = values[index]
                     #values[index][0, :, :] = values[index][0, :, :].astype(np.short)
                     values[index][0, :, :] = final_input 
                     values[index][0, :, :] = values[index][0, :, :].astype("f4")
                     #values[index][0, :, :] = (values[index][0, :, :]*meta[j]["scale_factor"]).astype(np.short)
-
-                    # AOD print
-                    print("AFTER ASSIGNMENT: ",final_input)
-                    print("TYPE: ", values[index][0, :, :].dtype)
-                    print("AOD nc check: ", np.array(values[index][0, :, :] ))
                     
                     sensors[p_vars].append(np.flipud(rotated)) #add it to complete dataset for LEOGEO calculations
                     
                 #time
                 end_timer = time.time()
-                print("Sensor: ",s_name ," time: ", end_timer - start_timer)
+                logging.info("Sensor: ",s_name ," time: ", end_timer - start_timer)
                 
             else:  #phy_var is NOT AOD
 
                 avgtau,stdtau,grdlat,grdlon,mintau,maxtau,count,sumtau = gridding.grid(limit,float(gsize),indata_temp[j],inlat_temp[j],inlon_temp[j])
 
                 index = len(values) #i * len(phy_list) + j
                 name = naming_conventions.nc_var_name(p_vars, s_name) #str(s_name+"_"+p_vars)
-                
                 values.append(ds.createVariable(name, np.short, ('time', 'lat', 'lon', ), fill_value=meta[j]["_FillValue"]))
                 
                 # metadata
                 values[index].units = "degree"#meta[j]["units"]
                 values[index].valid_range = meta[j]["valid_range"]
                 values[index].long_name = naming_conventions.nc_long_name(p_vars, s_name)#meta[j]["long_name"]
                 values[index].scale_factor = round(meta[j]["scale_factor"], 3)
@@ -462,30 +422,27 @@
                 # make sure key is in dict 
                 # instantiation
                 if not p_vars in sensors:
                     sensors[p_vars] = []
                 """
                 
                 rotated = list(zip(*avgtau))[::-1]
-                #print("ROTATED NON AOD")
-                #print(np.flipud(rotated)) # print what is input into the variable
                 
                 #manually set to fill_value
                 rotated = np.array(rotated)
-                print("VALID RANGE:", meta[j]["valid_range"][0], " TO ", meta[j]["valid_range"][1])
                 rotated[rotated > meta[j]["valid_range"][1]+1] = meta[j]["_FillValue"]
                 rotated[rotated < meta[j]["valid_range"][0]-1] = meta[j]["_FillValue"]
                 
                 
                 values[index][0, :, :] = np.flipud(rotated) # put into variable
                 #sensors[p_vars].append(np.flipud(rotated)) #add it to complete dataset for LEOGEO calculations
 
                 #time
                 end_timer = time.time()
-                print("Sensor: ",s_name ," time: ", end_timer - start_timer)
+                logging.info("Sensor: ",s_name ," time: ", end_timer - start_timer)
         
         # reset
         indata_temp = []
         inlat_temp = []
         inlon_temp = []
         
     # end individual sensor gridding and adding to nc
@@ -495,17 +452,14 @@
     # index of value corresponds to individual sensor
     # leogeo_stats = {"Mean": [[g16], [g17], [viirs], [modis]], "STD": [], "TotalPixels":[]}
     # sensor_idx = {} #key = sensor name, value = sensoridx
     leogeo_calculated_statistics = []
     number_of_sensors_variable = []
     sensor_idx_variable = []
     
-    #print("\nLEOGEO STATS\n")
-    #print(leogeo_stats)
-    
     # FilteredQA_550
     # Mean, STD, and TotalPixels stat calculations
     j = 0
     leogeo_index = 0 #index for leogeo statistics array where nc variables are appended to
     leogeo_meta_index = 0
     for p_var in phy_list:
         if p_var in leogeo_stats_arr: #go through each geophysical variable
@@ -529,26 +483,24 @@
                 else:
                     stat_values = naming_conventions.calculate_statistic(statistic, 
                                                                     leogeo_stats["Mean"],
                                                                     leogeo_stats["STD"],
                                                                     leogeo_stats["TotalPixels"])
                 leogeo_calculated_statistics[leogeo_index].append(ds.createVariable(name, np.short, ('time', 'lat', 'lon', ), fill_value = -9999 )) #1/29/2023 - added fill value
                 leogeo_calculated_statistics[leogeo_index][i][0, :, :] = stat_values
-                #print("MAX STAT VALUE for ", statistic, ":", stat_values.max())
                 leogeo_long = meta[leogeo_meta_index]["long_name"]
                 
                 if (("Filtered" in name) or ("filtered" in name)) and (statistic == "Mean"):
                     leogeo_calculated_statistics[leogeo_index][i].long_name = naming_conventions.nc_long_name(p_var, "LEOGEO", 
-                                                                                          statistic, None, True) + " for the grid. " + "It is average of individual sensor gridded AODs (i.e. AOD_FilteredQA_550_*_*_Mean)" #statistics_references_long
+                                                                                          statistic) + " for the grid. " + "It is average of individual sensor gridded AODs (i.e. AOD_FilteredQA_550_*_*_Mean)" #statistics_references_long
                 else:
                     leogeo_calculated_statistics[leogeo_index][i].long_name = naming_conventions.nc_long_name(p_var, "LEOGEO", 
                                                                                           statistic) + " for the grid"
                 # metadata
                 leogeo_calculated_statistics[leogeo_index][i].units = "1"#"degree"#meta[leogeo_meta_index]["units"]
-                #print("LEOGEO STAT: ", meta[leogeo_meta_index])
                 if not("Pixels" in statistic) or not("TotalPixels" in statistic):
                     leogeo_calculated_statistics[leogeo_index][i].scale_factor = round(meta[leogeo_meta_index]["scale_factor"], 3)
                     leogeo_calculated_statistics[leogeo_index][i].add_offset = meta[leogeo_meta_index]["add_offset"]
                     leogeo_calculated_statistics[leogeo_index][i].valid_range = meta[leogeo_meta_index]["valid_range"]
                 else:
                     #Total pixels does nott have scale_factor, add_offset
                     leogeo_calculated_statistics[leogeo_index][i].valid_range = [0, 100]
@@ -608,69 +560,13 @@
             #number_of_sensors_variable[leogeo_index].scale_factor = float(1/6)
             
             leogeo_index+=1    
         j += 1
         leogeo_meta_index += 1
     
     
-    """
-    # put in gridded statistics
-    # avgtau,stdtau,grdlat,grdlon,mintau,maxtau,count,sumtau = gridding.grid(limit,float(gsize),indata_stat,inlat_stat,inlon_stat)
-    sensor_id = []
-    shape = (len(np.arange(0,lat_dim)*gsize+minlat), len(np.arange(0,lon_dim)*gsize+minlon))
-    avg = []
-    # all sensors combined statistics (LEOGEO)
-    for k, p_vars in enumerate(phy_list):
-        # averages
-        try:
-            avgtau = np.nanmean(np.array(sensors.get(p_vars)), axis=0 )
-            # other statistics nan
-            # Number of Sensors
-            sensor_id_x = np.zeros(shape)
-            for i in range(len(sensors[p_vars])):
-                sensor_id_x = sensor_id_x + (np.array(sensors.get(p_vars)[i])*0+1)
-                #print(np.nan_to_num(np.array(sensors.get(p_vars)[i])*0+1, -1))
-            avg_name = str("merge_avgtau_" + p_vars)
-            avg.append(ds.createVariable(avg_name, 'f4', ('time', 'lat', 'lon', )))
-            avg[k][0, :, :] = avgtau
-            # metadata
-            # naming convention, units should be consistent
-            # read from configuration file
-            # follow netcdf conventions
-            # avg[k].units = meta["units"]
-            # avg[k].valid_range = meta["valid_range"]
-            # avg[k]._FillValue = meta["_FillValue"]
-            # avg[k].long_name = meta["long_name"]
-            # avg[k].scale_factor = meta["scale_factor"]
-            # avg[k].add_offset = meta["add_offset"]
-            # avg[k].Parameter_Type = meta["Parameter_Type"]
-            sensor_id_name = str("sensor_id_x_" + p_vars)
-            sensor_id.append(ds.createVariable(sensor_id_name, 'f4', ('time', 'lat', 'lon', )))
-            sensor_id[k].units = 'unknown'
-            sensor_id[k][0, :, :] = sensor_id_x
-        except:
-            #print("There are: ", len(sensors.get(p_vars)), " sensors for the var")
-            print(p_vars)
-            print(sensors.get(p_vars))
-    """
-
-    # print modis mean again
-    #print(values)
-    #print(values[0])
-    #print(values[0].long_name)
-    print("CHECK 1")
-    #close file
-    #ds.close()
-    #grid_close(ds)s
-    print("CHECK 2")
-    
-    
     return ds
     # output = 1 netcdf with six variables (one for each sensor) 
     # merge = run two loops (lat lon) (xdim, ydim from grid) 
     # merge aod equal to average of six sensors making sure no nan
     # identify which sensors are availabe - sensor ID variable 0 or 1 (unavailable vs available)
-    # byte type array, keep n-dimensional for now
-    # minimum number of things to merge: in the future
-
-    # future capabilities:
-    # minimum number, flagging system, use higher quality data (prefiltered)
+
```

### Comparing `pyroscope_gridtools-0.0.3/pyroscope_gridtools/gridding.py` & `Pyroscope-gridtools-0.1/Pyroscope-gridtools/gridding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+__author__ = "Sally Zhao"
+__copyright__ = "Copyright 2023, Pyroscope"
+__credits__ = ["Neil Gutkin", "Jennifer Wei", "Pawan Gupta", "Robert Levy", "Xiaohua Pan", "Zhaohui Zhang"]
+__version__ = "1.0.0"
+__maintainer__ = "Sally Zhao"
+__email__ = "zhaosally0@gmail.com"
+__status__ = "Production"
 # Gridding
 
 # To transform the level 2 data into level 3 data, the derived geophysical variables from the L2 data are:
 # 
 # 1. mapped to uniform space-time grid scales
 # 2. weighted based on data quality (for control, consistency, and completeness)
 # 
@@ -74,15 +81,14 @@
                     sqrtau[i,j]=sqrtau[i,j]+(indata[ii])**2
                     count[i,j]+=1
                     if indata[ii] < mintau[i,j]:
                         mintau[i,j]=indata[ii]
                     if indata[ii] > maxtau[i,j]:
                         maxtau[i,j]=indata[ii]
                     
-                #print("updated: ", sumtau[i,j], mintau[i,j], maxtau[i,j])
 
         for i in range(xdim):
             for j in range(ydim):
                 grdlon[i,j]=dx*i+minlon
                 grdlat[i,j]=dx*j+minlat
                 if count[i,j] > 0:
                     avgtau[i,j]=sumtau[i,j]/count[i,j]
@@ -259,24 +265,8 @@
 def multi_sensor_grid(filelist, gsize, limit, phy_list, geo_list=['latitude', 'longitude']):
     # get gridding parameters
     inlat,inlon,indata = multi_sensor_grid_data(filelist, phy_list, geo_list)
     
     #return gridded statistics
     avgtau,stdtau,grdlat,grdlon,mintau,maxtau,count,sumtau = grid(limit,gsize,indata,inlat,inlon)
     
-    return avgtau,stdtau,grdlat,grdlon,mintau,maxtau,count,sumtau
-
-#grid(limit,gsize,indata,inlat,inlon)
-if __name__ == '__main__':
-    limit = [-90., 90., -180., 180.]
-    limit= [1, 10, 1, 10]
-    limit = [1, 2, 1, 3]
-    gsize = 1# 0.25
-    indata = [0] * 10
-    inlat = [1,2,3,4,5,6,7,8,9,90]
-    inlon = [1,2,3,4,5,6,7,8,9,180]
-    
-    avgtau,stdtau,grdlat,grdlon,mintau,maxtau,count,sumtau = grid(limit,gsize,indata,inlat,inlon)
-    #print(avgtau)
-    
-    print(avgtau)
-    
+    return avgtau,stdtau,grdlat,grdlon,mintau,maxtau,count,sumtau
```

### Comparing `pyroscope_gridtools-0.0.3/pyroscope_gridtools/gtools.py` & `Pyroscope-gridtools-0.1/Pyroscope-gridtools/gtools.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,22 +20,24 @@
 import time_conv
 
 import os
 import argparse
 import numpy as np
 import datetime
 import time
+
+import logging
 """
 # python3 gtools.py -r -fn "C:/Users/swzhao/Desktop/Old Code and Satellite Inputs/Satellite Sensor Data/AERDT_L2_VIIRS_SNPP.A2021008.2018.001.2021009072852.nc" -gl "latitude longitude" -gp "Optical_Depth_Land_And_Ocean"
 def read(filename, geo_list, phy_list, verbose = False):
 
     geo_list = geo_list.split(" ")
-    print("Geolocation variables: ", geo_list)
+    logging.info("Geolocation variables: ", geo_list)
     phy_list = phy_list.split(" ")
-    print("Geophysical variables: ", phy_list)
+    logging.info("Geophysical variables: ", phy_list)
     # open file
     L2FID,GeoID,PhyID =sat_data_input.open_file(filename)
 
     geo = sat_data_input.read_geo_data(GeoID, var_list=geo_list)
     phy = sat_data_input.read_phy_data(PhyID, GeoID, var_list=phy_list, var_nc=phy_list, var_hdf=phy_list)
     lat = geo['data'][0][:,:]
     lon = geo['data'][1][:,:]
@@ -48,50 +50,50 @@
     lat1=lat[aod>0]
     lon1=lon[aod>0]
     aod1=aod[aod>0]
 
     L2FID.close()
 
     if verbose:
-        print("Gridding: " + str(filename) + "\nGeolocation:" + str(geo_list)+ "\nGeophysical:" + str(phy_list))
+        logging.info("Gridding: " + str(filename) + "\nGeolocation:" + str(geo_list)+ "\nGeophysical:" + str(phy_list))
 
-        print("dims:", row, col)
-        #PRINTS
+        logging.info("dims:", row, col)
+        #logging.infoS
         for i in range(10): #(aod1.size):
-            print('(lat,lon)=({0:.2f}, {1:.2f}) aod= {2:.3f}'.\
+            logging.info('(lat,lon)=({0:.2f}, {1:.2f}) aod= {2:.3f}'.\
                 format(lat1[i], lon1[i], aod1[i]))
     
     return lat1, lon1, aod1
 
 # python3 gtools.py -f -fn "C:/Users/swzhao/Desktop/Old Code and Satellite Inputs/Satellite Sensor Data/AERDT_L2_VIIRS_SNPP.A2021008.2018.001.2021009072852.nc" -gl "latitude longitude" -gp "Optical_Depth_Land_And_Ocean"
 def filter(filename, geo_list, phy_list, verbose = False):
     geo_list = geo_list.split(" ")
-    print(geo_list)
+    logging.info(geo_list)
     phy_list = phy_list.split(" ")
-    print(phy_list)
+    logging.info(phy_list)
 
     # open file
     L2FID,GeoID,PhyID = sat_data_input.open_file(filename)
     #filter
     lat,lon,phy_vars, metadata = filter_data.filter_data(GeoID, PhyID, geo_list, phy_list, phy_nc=phy_list, phy_hdf=phy_list)
     # close file
     L2FID.close()
     
     if verbose:
-        print("Latitude: ", lat)
-        print("Latitude: ", lon)
-        print("Geophysical: ", phy_vars)
+        logging.info("Latitude: ", lat)
+        logging.info("Latitude: ", lon)
+        logging.info("Geophysical: ", phy_vars)
 
     return lat,lon,phy_vars, metadata
 
 def grid(filename, geo_list, phy_list, verbose = False):
     geo_list = geo_list.split(" ")
-    print(geo_list)
+    logging.info(geo_list)
     phy_list = phy_list.split(" ")
-    print(phy_list)
+    logging.info(phy_list)
 
     L2FID,GeoID,PhyID = sat_data_input.open_file(filename)
 
     lat,lon,phy_vars, metadata = filter_data.filter_data(GeoID, PhyID, geo_list, phy_list, phy_nc=phy_list, phy_hdf=phy_list)
 
     L2FID.close()
 
@@ -101,80 +103,80 @@
     indata = phy_vars[0]
     inlat=lat[0]
     inlon = lon[0]
 
     avgtau,stdtau,grdlat,grdlon,mintau,maxtau,count,sumtau = gridding.grid(limit,gsize,indata,inlat,inlon)
 
     if verbose:
-        print(avgtau)
+        logging.info(avgtau)
 
     return avgtau,stdtau,grdlat,grdlon,mintau,maxtau,count,sumtau
 """
 """
 def netCDF_single(filename, geo_list, phy_list, output):
     geo_list = geo_list.split(" ")
-    print(geo_list)
+    logging.info(geo_list)
     phy_list = phy_list.split(" ")
-    print(phy_list)
+    logging.info(phy_list)
 
     #L2FID,GeoID,PhyID = sat_data_input.open_file(filename)
 
     #,lon,phy_vars, metadata = filter_data.filter_data(GeoID, PhyID, geo_list, phy_list, phy_nc=phy_list, phy_hdf=phy_list)
 
     #L2FID.close()
 
     #grid parameters
     limit = [min(lat[0]), max(lat[0]), min(lon[0]),  max(lon[0])]
     gsize = 0.25
     indata = phy_vars[0]
     inlat=lat[0]
     inlon = lon[0]
 
-    print("Results at: " + output)
+    logging.info("Results at: " + output)
 
     grid_ncf.gridNC_single(limit, gsize, indata, inlat, inlon, output)
 """
 #gridNC_time(limit, gsize, indata, inlat, inlon, 1, phy_list, geo_list, sat_files[:10], fpath + "viirs_time_compv1.nc")
 def netCDF_multi(filelist, geo_list, phy_list, output):
     geo_list = geo_list.split(" ")
-    print(geo_list)
+    logging.info(geo_list)
     phy_list = phy_list.split(" ")
-    print(phy_list)
+    logging.info(phy_list)
     filelist = fileparser.read_file_sat_data(filelist)
 
-    print(filelist)
+    logging.info(filelist)
 
     lat,lon,phy_vars = gridding.multi_sensor_grid_data(filelist, phy_list, geo_list)
 
-    print(lat)
-    print(lon)
-    print(phy_vars)
+    logging.info(lat)
+    logging.info(lon)
+    logging.info(phy_vars)
 
     #grid parameters
     limit = [min(lat), max(lat), min(lon),  max(lon)]
     gsize = 0.25
     indata = phy_vars
     inlat=lat
     inlon = lon
 
-    print("Results at: " + output)
+    logging.info("Results at: " + output)
 
     #grid_ncf.gridNC_time(limit, gsize, indata, inlat, inlon, 1, phy_list, geo_list, filelist, output)
     
     #grid_ncf.gridNC_time(limit, gsize, indata, inlat, inlon, output)
 
 
     
 def netCDF_multi_time(filelist, gsize, geo_list, phy_list, output, time_interval, time_start, time_end):
     start_timer = time.time()
 
     geo_list = geo_list.split(" ")
-    print(geo_list)
+    logging.info(geo_list)
     phy_list = phy_list.split(" ")
-    print(phy_list)
+    logging.info(phy_list)
     filelist = fileparser.read_file_sat_data(filelist)
 
     start = time_conv.to_datetime(time_start)
     end = time_conv.to_datetime(time_end)
 
     split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
 
@@ -185,24 +187,24 @@
     indata = phy_vars
     inlat=lat
     inlon = lon
 
     #grid_ncf.grid_nc_mult_files_time(limit, gsize, indata, inlat, inlon, phy_list, geo_list, split_files, output)
 
     end_timer = time.time()
-    print("Full execution time: ", end_timer - start_timer)
+    logging.info("Full execution time: ", end_timer - start_timer)
 
 # output - folder location
 def netCDF_sensor_statistics(filelist, limit, gsize, geo_list, phy_list, outputfolder, outputname, time_interval, time_start, time_end):
     start_timer = time.time()
     
     geo_list = geo_list.split(" ")
-    print(geo_list)
+    logging.info(geo_list)
     phy_list = phy_list.split(" ")
-    print(phy_list)
+    logging.info(phy_list)
     limit = [float(item) for item in limit.split(" ")]
     filelist = fileparser.read_file_sat_data(filelist)
 
     start = time_conv.to_datetime(time_start)
     end = time_conv.to_datetime(time_end)
 
     split_files = time_conv.split_filetimes(filelist, start, end, int(time_interval))
@@ -214,25 +216,25 @@
         name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
 
         # grid files
         #grid_ncf.grid_nc_single_statistics(limit, gsize, geo_list, phy_list, f, name)
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
-    print("Full execution time: ", end_timer - start_timer)
+    logging.info("Full execution time: ", end_timer - start_timer)
 
 # output - folder location
 def netCDF_sensor_statistics_split(filelist, limit, gsize, geo_list, phy_list, outputfolder, outputname, time_interval, time_start, time_end):
 
     start_timer = time.time()
 
     geo_list = geo_list.split(" ")
-    print(geo_list)
+    logging.info(geo_list)
     phy_list = phy_list.split(" ")
-    print(phy_list)
+    logging.info(phy_list)
     limit = [float(item) for item in limit.split(" ")]
     filelist = fileparser.read_file_sat_data(filelist)
 
     start = time_conv.to_datetime(time_start)
     end = time_conv.to_datetime(time_end)
 
     # [[filenames for a time interval] , [], []]
@@ -250,25 +252,23 @@
         name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
 
         # grid files
         #grid_ncf.grid_nc_statistics(limit, gsize, geo_list, phy_list, f, name)
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
-    print("Full execution time: ", end_timer - start_timer)
+    logging.info("Full execution time: ", end_timer - start_timer)
 
 # output - folder location
 def netCDF_sensor_statistics_id(filelist, limit, gsize, geo_list, phy_list, outputfolder, outputname, time_interval, time_start, time_end):
 
     start_timer = time.time()
 
     geo_list = geo_list.split(" ")
-    print(geo_list)
     phy_list = phy_list.split(" ")
-    print(phy_list)
     limit = [float(item) for item in limit.split(" ")]
     filelist = fileparser.read_file_sat_data(filelist)
 
     start = time_conv.to_datetime(time_start)
     end = time_conv.to_datetime(time_end)
 
     # [[filenames for a time interval] , [], []]
@@ -280,24 +280,24 @@
     split_files = time_conv.split_filenames(split_files)
 
     gsize = float(gsize)
 
     curr = start
     for f in split_files:
         name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
-        #print(f)
-        # print(split_files)
+        #logging.info(f)
+        # logging.info(split_files)
         
         # grid files
         #grid_nc_sensor_statistics_metadata
         #grid_ncf.grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, phy_nc=phy_list, phy_hdf=phy_list)
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
-    print("Full execution time: ", end_timer - start_timer)
+    logging.info("Full execution time: ", end_timer - start_timer)
 
 # output - folder location
 def netCDF_yaml_config(file_name):
 
     grid_settings, variables, file_io = fileparser.read_config(file_name)
 
     start_timer = time.time()
@@ -317,15 +317,14 @@
             filelist = fileparser.read_folder_sat_data(file_io["file_location_folder"])
     else:
         filelist = fileparser.read_directory_sat_data(file_io["file_directory_folder"])
         
         
     #static file for Land_Sea_Mask and Topographic_Altitude
     static_file = file_io["static_file"]
-    print("static file:", static_file)
 
     time_start = grid_settings["time_start"]
     time_end = grid_settings["time_end"]
     start = time_conv.to_datetime(time_start)
     end = time_conv.to_datetime(time_end)
 
     # [[filenames for a time interval] , [], []]
@@ -348,30 +347,20 @@
         #name = outputfolder + outputname + str(curr).replace(":", "-")+".nc"
         #XAERDT_L3_MEASURES_QD_HH.YYYYMMDD.HHMM.V0.ProcessingDate.nc
         time_string = str(curr).replace(":", "").replace("-", "").replace(" ", "")
         time_string = time_string[:8] + '.' + time_string[8:-2]
         processing_date = time_conv.sys_time()
         name = outputfolder + "XAERDT_L3_MEASURES_QD_HH." + time_string+ ".V0." +processing_date+ ".nc"
         
-        #print(f) f = dict (key: sensor, values: array of filelocs)
-        # print(split_files)
-        
-        #print("\n\nNAME:", name)
-        #print("\n\TIME STRING:", curr)
-        #print("\n\PROCESS DATE:", time_interval)
-        
-        # grid files
-        #grid_nc_sensor_statistics_metadata
-        
         ds = grid_ncf.grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
         ds.close()
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
-    print("Full execution time: ", end_timer - start_timer)
+    logging.info("Full execution time: ", end_timer - start_timer)
     
 # output - folder location
 def netCDF_yaml_config_time(file_name, time_start, time_end):
 
     grid_settings, variables, file_io = fileparser.read_config(file_name)
 
     start_timer = time.time()
@@ -388,18 +377,17 @@
         if file_io["file_location_folder"] == "NA":
             filelist = fileparser.read_file_sat_data(file_io["file_location_file"])
         else:
             filelist = fileparser.read_folder_sat_data(file_io["file_location_folder"])
     else:
         filelist = fileparser.read_directory_sat_data(file_io["file_directory_folder"])
         
-    print("FILELIST: ", filelist)
+    logging.info("FILELIST: ", filelist)
     #static file for Land_Sea_Mask and Topographic_Altitude
     static_file = file_io["static_file"]
-    print("static file:", static_file)
 
     #time_start = grid_settings["time_start"]
     #time_end = grid_settings["time_end"]
     start = time_conv.to_datetime(time_start)
     end = time_conv.to_datetime(time_end)
     
 
@@ -428,15 +416,15 @@
         name = outputfolder + "XAERDT_L3_MEASURES_QD_HH." + time_string+ ".V0." +processing_date+ ".nc"
         
         ds = grid_ncf.grid_nc_sensor_statistics_metadata(limit, gsize, geo_list, phy_list, f, name, curr, time_interval, phy_nc, phy_hdf, static_file, pixel_range)
         ds.close()
         curr = curr + datetime.timedelta(minutes = int(time_interval))
 
     end_timer = time.time()
-    print("Full execution time: ", end_timer - start_timer)
+    logging.info("Full execution time: ", end_timer - start_timer)
 
     
 
 def execute_file(filename):
     filelist, gsize, time_interval, start, end, output, geo_list, phy_list = fileparser.read_in_commands(filename)
     lat,lon,phy_vars = gridding.multi_sensor_grid_data(filelist, phy_list, geo_list)
     #grid parameters
@@ -544,15 +532,15 @@
     elif args.configtime:
         # yaml config 
         # python gtools.py -cfg -fn "C:\Users\swzhao\Desktop\repos\gridtools\config.yml"
         # "C:\Users\bobgr\Desktop\Spring 2022 NASA\Gridtools Package (Code, README, inputs, outputs, examples, verification)\gridtools\config.yml"
         # "C:/Users/bobgr/Desktop/Spring 2022 NASA/Gridtools Package (Code, README, inputs, outputs, examples, verification)/gridtools/config.yml"
         netCDF_yaml_config_time(str(args.filename), str(args.time_start), str(args.time_end))
     else:
-        print("No command given")
+        logging.info("No command given")
         
 
 if __name__ == '__main__':
     control()
```

### Comparing `pyroscope_gridtools-0.0.3/pyroscope_gridtools/naming_conventions.py` & `Pyroscope-gridtools-0.1/Pyroscope-gridtools/naming_conventions.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             name = name + "_" + sensor_references[sensor_key] 
     
     if statistic:
         name = name + "_" + statistic
     
     return name
 
-def nc_long_name(geophys_name, sensor_name, statistic = None, aod_long = None, filtered=False):
+def nc_long_name(geophys_name, sensor_name, statistic = None, aod_long = None):
     name = ""
     if statistic == None:
         for sensor_key in sensor_references_long: #add appropriate sensor name
             if sensor_key in sensor_name:
                 name = name + " " + sensor_references_long[sensor_key] 
         if geophys_name == "Sensor_Zenith":
             name = name + " Sensor Viewing Angle, mean for the grid"
@@ -93,18 +93,15 @@
     else:
         curr_stat = ""
         for stat in statistics_references_long_LEOGEO:
             if statistic == stat:
                 name = statistics_references_long_LEOGEO[stat]
                 curr_stat = statistic
                 if statistic =="Mean" or statistic =="STD" or statistic =="Pixels" or statistic == "TotalPixels":
-                    if filtered:
-                        name = name + " " + "AOD at 0.55 micron (Optical_Depth_Land_And_Ocean) for both ocean (Average) and land (corrected) with all quality data (Quality flag = 0, 1, 2, 3)"
-                    else:
-                        name = name + " " + "AOD at 0.55 micron (Image_Optical_Depth_Land_And_Ocean) for both ocean (Average) and land (corrected) with all quality data (Quality flag = 0, 1, 2, 3)"
+                    name = name + " " + "AOD at 0.55 micron (Image_Optical_Depth_Land_And_Ocean) for both ocean (Average) and land (corrected) with all quality data (Quality flag = 0, 1, 2, 3)"
         for sensor_key in sensor_references_long: #add appropriate sensor name
             if sensor_key in sensor_name:
                 #name = name + " " + sensor_references_long[sensor_key] 
                 if aod_long != None:
                     name = name + " " + aod_long
                 if curr_stat == "SensorWeighting":
                     name = name + ", the default value is 1.0 if sensor is available and 0.0 if sensor is not available, the sensor dimension order is MODIS-T, MODIS-A, VIIRS-SNP, ABI-G16, ABI-G17, AHI-H08"
@@ -135,24 +132,20 @@
         """
         
         data = np.array(data)
         data[data<=-9999.] = np.nan # fill_value
         
         avgtau = np.nanmean(data, axis=0 ) # [ [avgtau for modis a], [avgtau .. ]  ]
         avgtau = np.nan_to_num(avgtau, nan=-9999) # fill_value
-        #print(avgtau.flatten())
-        #print("ORIGINAL DATA2:", data)
         
         #avgtau = np.nanmean(np.array(data), axis=0 )
         avgtau = avgtau/scale_factor
         
         avgtau[avgtau > 5001] = -9999
         avgtau[avgtau < -101] = -9999
-        
-        print("AVGTAU LEOGEO TYPE: ", avgtau.dtype)
     
         return avgtau
     
     # https://stats.stackexchange.com/questions/55999/is-it-possible-to-find-the-combined-standard-deviation
     if statistic == "STD":
         
         # [[std g16], [ g17], []]
@@ -192,19 +185,8 @@
     data = [[[3., 2], 
              [0, -10000000]], 
             [[1, 4], 
              [1, 1]]]
     data2 = [[[10, 10], [10, 10]], [[0, 10], [10, 10]], [[10, 10], [10, 10]]]
     data3 = [[[3, 2], [0, 0]], [[1, 4], [1, -5]], [[1, 0], [0, 0]]]
     
-    #print(nc_long_name("Optical_Depth_Land_And_Ocean", "LEOGEO", "TotalPixels"))
-    #data = np.array([[[0,1],[2,3]], [[1,2], [3, 4]]])
-    #print(np.nanmean(np.array(data), axis=0 ))
-    
-    #path = "/mnt/c/Users/bobgr/Desktop/NASA Spring 2023/Gridtools Package (Code, README, inputs, outputs, examples, verification)/SampleOutputs 0000-0059 01-01-2020/"
-    #filename = "XAERDT_L3_MEASURES_QD_HH.20200101.0000.V0.20230130.nc"
-    #L2FID = netCDF4.Dataset(path+filename,'r',format='NETCDF4')
-    #L2FID.close()
-    
-    print(data)
-    print("MEAN:", calculate_statistic("Mean", data))
-    print("STD:", calculate_statistic("STD", data))
+
```

### Comparing `pyroscope_gridtools-0.0.3/pyroscope_gridtools/sat_data_input.py` & `Pyroscope-gridtools-0.1/Pyroscope-gridtools/sat_data_input.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,45 +15,35 @@
 # 1. open_file : opens the netCDF4 file, expecting a geolocation and geophysical group
 # 2. read_geo_data : reads the open_file's return geo 
 # 3. read_phy_data : reads the open_file's return phy 
 
 # imports
 import netCDF4
 import os
-import sys
 import numpy as np
 
 import pyhdf
 from pyhdf import SD
 
+import logging
+
 # Opens file through file path
 # Reads in two separate groups, geolocation and geophysical
 # Opens file through file path
 # Reads in two separate groups, geolocation and geophysical
 def open_file(L2FileName):
    if not os.path.isfile(L2FileName):
       err = "Error: file not exis {} ... ".format(L2FileName)
-      print(err)
+      logging.info(err)
 
       return(False)
    try: # netcdf
-      #print("OPENED AS NETCDF")
       L2FID = netCDF4.Dataset(L2FileName,'r',format='NETCDF4')
    except:
-      """
-      try: # hdf
-         print("OPENED AS HDF")
-         #L2FID = SD.SD(L2FileName)
-         L2FID = netCDF4.Dataset(L2FileName,'r',format='HDF') 
-      except:
-         #print("touching")
-         os.touch(L2FileName)
-      """
       L2FID = SD.SD(L2FileName)
-      print("HDF\n:", L2FID)
       #L2FID = netCDF4.Dataset(L2FileName,'r')#,format='HDF') 
       
    ftype = os.path.splitext(L2FileName)[1]
    GeoGroupID = L2FID
    PhyGroupID = L2FID
     
    if ftype != '.hdf':
@@ -100,187 +90,57 @@
       #make same as convention
       geo['data'].append(data)
       geo['scale_factor'].append(metadata["scale_factor"])
       geo['add_offset'].append(metadata["add_offset"])
       geo['_FillValue'].append(metadata["_FillValue"])
    
    return geo
-   """
-   if var_list is None:
-      var_list = ['Latitude', 'Longitude']
-
-   GeoGroup = L2GeoGroup.variables      
-   geo = {"data":[], "scale_factor":[], "add_offset":[], "_FillValue":[]}   
-   
-   for var in var_list:
-      geo['data'].append(GeoGroup[var])
-      geo['scale_factor'].append(GeoGroup[var].scale_factor)
-      geo['add_offset'].append(GeoGroup[var].add_offset)
-      geo['_FillValue'].append(GeoGroup[var]._FillValue)
-         
-   return geo
-   """
-
-
-"""
-# Parses the geolocation group after file is read
-# Variables are latitude and longitude by default only
-def read_geo_data(L2GeoGroup, var_list=None):
-   if var_list is None:
-      var_list = ['latitude', 'longitude']
-
-   try: # netcdf file
-      GeoGroup = L2GeoGroup.variables      
-      geo = {"data":[], "scale_factor":[], "add_offset":[], "_FillValue":[]}   
-      for var in var_list:
-         geo['data'].append(GeoGroup[var])
-         geo['scale_factor'].append(GeoGroup[var].scale_factor)
-         geo['add_offset'].append(GeoGroup[var].add_offset)
-         geo['_FillValue'].append(GeoGroup[var]._FillValue)
-         
-   except: # hdf file
-      geo = {"data":[], "scale_factor":[], "add_offset":[], "_FillValue":[]}
-      var_list=[]
-      var_list.extend(['Latitude', 'Longitude'])
-
-      for var in var_list:
-         sds = L2GeoGroup.select(var)
-         data = sds.get()
-         metadata = sds.attributes()
-         
-         #make same as convention
-         geo['data'].append(data)
-         geo['scale_factor'].append(metadata["scale_factor"])
-         geo['add_offset'].append(metadata["add_offset"])
-         geo['_FillValue'].append(metadata["_FillValue"])
-      
-      
-   return(geo)
-"""
-"""
-# Parses the geophysical group after file is read
-# Variables are aod by default only
-def read_phy_data(L2PhyGroup, L2GeoGroup, var_list=None, var_nc=None, var_hdf=None):
-   if var_list is None:
-      var_list = ['Optical_Depth_Land_And_Ocean']
-
-   #try: # netcdf
    
-   phy = {"data":[], "scale_factor":[], "add_offset":[], "_FillValue":[], "valid_range":[], "long_name":[], "units":[], "Parameter_Type":[]}   
-   for i in range(len(var_nc)):
-      try:
-            PhyGroup = L2PhyGroup.variables
-            var = var_nc[i]
-
-            #print("NETCDF VARIABLE: ", var)
-            phy['data'].append(PhyGroup[var] )
-            #print("Read physical in: ", phy['data'])
-
-            phy['valid_range'].append(PhyGroup[var].valid_range)
-            phy['_FillValue'].append(PhyGroup[var]._FillValue)
-            phy['long_name'].append(PhyGroup[var].long_name)
-            phy['units'].append(PhyGroup[var].units)
-            phy['scale_factor'].append(PhyGroup[var].scale_factor)
-            phy['add_offset'].append(PhyGroup[var].add_offset)
-            phy['Parameter_Type'].append(PhyGroup[var].Parameter_Type)
-      except:
-            # variable not found in PhyGroup
-            #print("Physical Var Error: ", AttributeError)
-
-            try: # look now in geolocation variables
-               # mainly for variables such as solar_zenith or scatter_angle
-               #print("INDEX?: ", i)
-               var = var_nc[i]
-
-               GeoGroup = L2GeoGroup.variables 
-               #print("GEO VARIABLE: ", var)
-
-               phy['data'].append(GeoGroup[var] )
-               #print("Read in: ", phy['data'])
-
-               phy['valid_range'].append(GeoGroup[var].valid_range)
-               phy['_FillValue'].append(GeoGroup[var]._FillValue)
-               phy['long_name'].append(GeoGroup[var].long_name)
-               phy['units'].append(GeoGroup[var].units)
-               phy['scale_factor'].append(GeoGroup[var].scale_factor)
-               phy['add_offset'].append(GeoGroup[var].add_offset)
-               phy['Parameter_Type'].append(GeoGroup[var].Parameter_Type)
-
-            except: # not here, treat as HDF file
-               try: 
-                  var = var_hdf[i]
-                  
-                  sds = L2PhyGroup.select(var)
-                  data = sds.get()
-                  metadata = sds.attributes()
-                  
-                  #make same as convention
-                  phy['data'].append(data)
-
-                  phy['valid_range'].append(metadata["valid_range"])
-                  phy['_FillValue'].append(metadata["_FillValue"])
-                  phy['long_name'].append(metadata["long_name"])
-                  phy['units'].append(metadata["units"])
-                  phy['scale_factor'].append(metadata["scale_factor"])
-                  phy['add_offset'].append(metadata["add_offset"])
-                  phy['Parameter_Type'].append(metadata["Parameter_Type"])
-                  
-               except: # varaible not found
-                  raise AttributeError("No such variable", var_list[i])      
-         
-   return(phy)
-"""
 # nc
 # Parses the geophysical group after file is read
 # Variables are aod by default only
 def read_phy_data_nc(L2PhyGroup, L2GeoGroup, var_list=None, var_nc=None):
    if var_list is None:
       var_list = ['Optical_Depth_Land_And_Ocean']
 
    phy = {"data":[], "scale_factor":[], "add_offset":[], "_FillValue":[], "valid_range":[], "long_name":[], "units":[], "Parameter_Type":[]}   
    for i in range(len(var_nc)):
       try:
             PhyGroup = L2PhyGroup.variables
             var = var_nc[i]
 
-            #print("NETCDF VARIABLE: ", var)
             phy['data'].append(PhyGroup[var] )
-            #print("Read physical in: ", phy['data'])
 
             phy['valid_range'].append(PhyGroup[var].valid_range)
             phy['_FillValue'].append(PhyGroup[var]._FillValue)
             phy['long_name'].append(PhyGroup[var].long_name)
             phy['units'].append(PhyGroup[var].units)
             phy['scale_factor'].append(PhyGroup[var].scale_factor)
             phy['add_offset'].append(PhyGroup[var].add_offset)
             phy['Parameter_Type'].append(PhyGroup[var].Parameter_Type)
       except:
             # variable not found in PhyGroup
-            #print("Physical Var Error: ", AttributeError)
 
             try: # look now in geolocation variables
                # mainly for variables such as solar_zenith or scatter_angle
-               #print("INDEX?: ", i)
                var = var_nc[i]
 
                GeoGroup = L2GeoGroup.variables 
-               #print("GEO VARIABLE: ", var)
 
                phy['data'].append(GeoGroup[var] )
-               #print("Read in: ", phy['data'])
 
                phy['valid_range'].append(GeoGroup[var].valid_range)
                phy['_FillValue'].append(GeoGroup[var]._FillValue)
                phy['long_name'].append(GeoGroup[var].long_name)
                phy['units'].append(GeoGroup[var].units)
                phy['scale_factor'].append(GeoGroup[var].scale_factor)
                phy['add_offset'].append(GeoGroup[var].add_offset)
                phy['Parameter_Type'].append(GeoGroup[var].Parameter_Type)
             except:
-               print("PHY DATA NOT FOUND: NC")
+               logging.info("PHY DATA NOT FOUND: NC")
 
    return(phy)
 
 # HDF
 # Parses the geophysical group after file is read
 # Variables are aod by default only
 def read_phy_data_hdf(L2PhyGroup, L2GeoGroup, var_list=None, var_hdf=None):
@@ -293,39 +153,30 @@
    
    for i in range(len(var_hdf)):
       try: 
          var = var_hdf[i]
          
          sds = L2PhyGroup.select(var)
          data = sds.get()
-         #print("HDF DATA: ", data)
          metadata = sds.attributes()
          
          #make same as convention
          phy['data'].append(data)
 
          phy['valid_range'].append(metadata["valid_range"])
          phy['_FillValue'].append(metadata["_FillValue"])
          phy['long_name'].append(metadata["long_name"])
          phy['units'].append(metadata["units"])
          phy['scale_factor'].append(metadata["scale_factor"])
          phy['add_offset'].append(metadata["add_offset"])
          phy['Parameter_Type'].append(metadata["Parameter_Type"])
          
-         #display data
-         print("DATA")
-         data2 = np.array(data).flatten()
-         print(data2[data2!=-9999])
-         
-         
-         
       except: # varaible not found
-         raise AttributeError("No such variable", var_list[i])      
-     
-   print("HDF:", phy)    
+         logging.info("No such variable", var_list[i])      
+      
    return(phy)
 
 # nc
 # Parses the geophysical group after file is read
 # Variables are aod by default only
 def read_phy_data_hdf_vnew(L2PhyGroup, L2GeoGroup, var_list=None, var_hdf=None):
    if var_list is None:
@@ -333,44 +184,38 @@
 
    phy = {"data":[], "scale_factor":[], "add_offset":[], "_FillValue":[], "valid_range":[], "long_name":[], "units":[], "Parameter_Type":[]}   
    for i in range(len(var_hdf)):
       try:
             PhyGroup = L2PhyGroup.variables
             var = var_hdf[i]
 
-            #print("NETCDF VARIABLE: ", var)
             phy['data'].append(PhyGroup[var] )
-            #print("Read physical in: ", phy['data'])
 
             phy['valid_range'].append(PhyGroup[var].valid_range)
             phy['_FillValue'].append(PhyGroup[var]._FillValue)
             phy['long_name'].append(PhyGroup[var].long_name)
             phy['units'].append(PhyGroup[var].units)
             phy['scale_factor'].append(PhyGroup[var].scale_factor)
             phy['add_offset'].append(PhyGroup[var].add_offset)
             phy['Parameter_Type'].append(PhyGroup[var].Parameter_Type)
       except:
             # variable not found in PhyGroup
-            #print("Physical Var Error: ", AttributeError)
 
             try: # look now in geolocation variables
                # mainly for variables such as solar_zenith or scatter_angle
-               #print("INDEX?: ", i)
                var = var_hdf[i]
 
                GeoGroup = L2GeoGroup.variables 
-               #print("GEO VARIABLE: ", var)
 
                phy['data'].append(GeoGroup[var] )
-               #print("Read in: ", phy['data'])
 
                phy['valid_range'].append(GeoGroup[var].valid_range)
                phy['_FillValue'].append(GeoGroup[var]._FillValue)
                phy['long_name'].append(GeoGroup[var].long_name)
                phy['units'].append(GeoGroup[var].units)
                phy['scale_factor'].append(GeoGroup[var].scale_factor)
                phy['add_offset'].append(GeoGroup[var].add_offset)
                phy['Parameter_Type'].append(GeoGroup[var].Parameter_Type)
             except:
-               print("PHY DATA NOT FOUND: NC")
+               logging.info("PHY DATA NOT FOUND: NC")
 
    return(phy)
```

### Comparing `pyroscope_gridtools-0.0.3/pyroscope_gridtools/solar_zenith.py` & `Pyroscope-gridtools-0.1/Pyroscope-gridtools/solar_zenith.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 __status__ = "Production"
 # Solar Zenith
 #
 # Calculates solar zenith and azimuth angles. 
 # Contains manual code calculations validated against pysolar
 #
 
-from pysolar.solar import get_altitude
-import time
+#from pysolar.solar import get_altitude
 import math
-
+import logging
+"""
 from sunpy.coordinates import frames
 #from sunpy.time import Time
 from astropy.coordinates import EarthLocation
 from pvlib import solarposition
 import pytz
-
+"""
 
 import datetime
 import numpy as np
 import pandas as pd
 
 import numba as nb
 from numba import jit
@@ -57,26 +57,23 @@
 	  - 0.154527*COS(3.0*theta_0) 				$
 	  + 0.084798*SIN(3.0*theta_0)
 
 declin = declin / rad	;convert to radians
 """
 def solar_declination_angle(D):
     theta_0 = (360.0 * (D - 1) / 365.0) / rad #converts to radians
-    declin  = (0.396372 - 22.91327*math.cos(theta_0)
-            + 4.02543*math.sin(theta_0) 
-            - 0.387205*math.cos(2.0*theta_0)
-            + 0.051967*math.sin(2.0*theta_0) 
-            - 0.154527*math.cos(3.0*theta_0) 
-            + 0.084798*math.sin(3.0*theta_0))
-    declin = declin / rad  #converts to radians
-    return theta_0, declin
 
-@cuda.jit(device=True)
-def sda_gpu(D, rad):
-    theta_0 = (360.0 * (D - 1) / 365.0) / rad #converts to radians
+    # theta_0 is currently in radians
+    declin  = (0.396372 - 22.91327*math.degrees(math.cos(theta_0))
+            + 4.02543*math.degrees(math.sin(theta_0) )
+            - 0.387205*math.degrees(math.cos(2.0*theta_0))
+            + 0.051967*math.degrees(math.sin(2.0*theta_0) )
+            - 0.154527*math.degrees(math.cos(3.0*theta_0) )
+            + 0.084798*math.degrees(math.sin(3.0*theta_0)))
+    
     declin  = (0.396372 - 22.91327*math.cos(theta_0)
             + 4.02543*math.sin(theta_0) 
             - 0.387205*math.cos(2.0*theta_0)
             + 0.051967*math.sin(2.0*theta_0) 
             - 0.154527*math.cos(3.0*theta_0) 
             + 0.084798*math.sin(3.0*theta_0))
     declin = declin / rad  #converts to radians
@@ -94,36 +91,20 @@
 
 lat_rad = lat / rad
 lon_rad = lon / rad
 
 angle_rad  = angle / rad
 """
 def time_correction_solar_angle(theta_0, time, lat, lon): #assume theta_0 in radians
-    correct = (0.004297 + 0.107029*math.cos(theta_0)
-                - 1.837877*math.sin(theta_0)
-                - 0.837378*math.cos(2.0*theta_0)
-                - 2.342824*math.sin(2.0*theta_0))
-                    
-                
-    angle = (time - 12.0) * 15.0 + lon + correct
     
-    if angle > 180:
-        angle = angle - 360
-    if angle < -180:
-        angle = angle + 360
-        
-    lat_rad = lat / rad
-    lon_rad = lon / rad
-
-    angle_rad  = angle / rad
+    correct  = (0.004297 + 0.107029*math.degrees(math.cos(theta_0)) 
+                - 1.837877*math.degrees(math.sin(theta_0))
+                - 0.837378*math.degrees(math.cos(2.0*theta_0))
+                - 2.342824*math.degrees(math.sin(2.0*theta_0)))
     
-    return angle, angle_rad, lat_rad, lon_rad
-
-@cuda.jit(device=True)
-def tcsa_gpu(theta_0, time, lat, lon, rad): #assume theta_0 in radians
     correct = (0.004297 + 0.107029*math.cos(theta_0)
                 - 1.837877*math.sin(theta_0)
                 - 0.837378*math.cos(2.0*theta_0)
                 - 2.342824*math.sin(2.0*theta_0))
                     
                 
     angle = (time - 12.0) * 15.0 + lon + correct
@@ -136,15 +117,14 @@
     lat_rad = lat / rad
     lon_rad = lon / rad
 
     angle_rad  = angle / rad
     
     return angle, angle_rad, lat_rad, lon_rad
 
-
 ### Sun zenith
 """
 tmp1 = SIN(lat_rad)*SIN(declin) + COS(lat_rad)*COS(declin)*COS(angle_rad)
 tmp2   = ABS(tmp1)
 
 IF tmp2 GT 1.1 THEN BEGIN
     PRINT, 'Error in acos argument in sun zenith'
@@ -160,40 +140,18 @@
 """
 def sun_zenith(lat_rad, lon_rad, angle_rad, declin):
     
     #tmps are in radians
     tmp1 = math.sin(lat_rad)*math.sin(declin) + math.cos(lat_rad)*math.cos(declin)*math.cos(angle_rad)
     #tmp1 = (math.degrees(math.sin(lat_rad))* math.degrees(math.sin(declin)) 
     #        + math.degrees(math.cos(lat_rad)) * math.degrees(math.cos(declin)) * math.degrees(math.cos(angle_rad)))
-    tmp2 = abs(tmp1)
-    
-    if tmp2 > 1.1:
-        print("Error in acos argument in sun zenith: ", tmp1)
-    else:
-        if tmp2 > 1.0:
-            if tmp1 > 0:
-                tmp1 = 1.0
-            if tmp1 < 0:
-                tmp1 = -1.0
-                
-    theta_rad = math.acos(tmp1)
-    
-    return theta_rad
-
-@cuda.jit(device=True)
-def sz_gpu(lat_rad, lon_rad, angle_rad, declin):
-    
-    #tmps are in radians
-    tmp1 = math.sin(lat_rad)*math.sin(declin) + math.cos(lat_rad)*math.cos(declin)*math.cos(angle_rad)
-    #tmp1 = (math.degrees(math.sin(lat_rad))* math.degrees(math.sin(declin)) 
-    #        + math.degrees(math.cos(lat_rad)) * math.degrees(math.cos(declin)) * math.degrees(math.cos(angle_rad)))
     tmp2   = abs(tmp1)
     
     if tmp2 > 1.1:
-        print("Error in acos argument in sun zenith: ", tmp1)
+        logging.infoor("Error in acos argument in sun zenith: ", tmp1)
     else:
         if tmp2 > 1.0:
             if tmp1 > 0:
                 tmp1 = 1.0
             if tmp1 < 0:
                 tmp1 = -1.0
                 
@@ -236,34 +194,14 @@
     
     theta_0, declin = solar_declination_angle(D)
     angle, angle_rad, lat_rad, lon_rad = time_correction_solar_angle(theta_0, time, lat, lon)
     theta_rad = sun_zenith(lat_rad, lon_rad, angle_rad, declin)
     #azimuth_rad = sun_azimuth(lat, lon, angle, angle_rad, theta_rad, declin)
     
     return math.degrees(theta_rad)
-
-@cuda.jit
-def get_SZA_GPU(lats, lons, N, D, time, sza, rad):
-    # Establish thread and block indices
-    t = cuda.threadIdx.x
-    #-------------------------
-    d = cuda.blockDim.x
-    #-------------------------
-    b = cuda.blockIdx.x
-
-    # Compute global array index
-    idx = t + b*d
-
-    if idx < N:
-        theta_0, declin = sda_gpu(D, rad)
-        angle, angle_rad, lat_rad, lon_rad = tcsa_gpu(theta_0, time, lats[idx], lons[idx], rad)
-        theta_rad = sz_gpu(lat_rad, lon_rad, angle_rad, declin)
-
-        sza[idx] = theta_rad * rad # to degrees
-
 """
 # uses pysolar library
 def get_SZA(lat, lon, time_start, time_diff):
     time_obj = pd.to_datetime(time_start) + pd.to_timedelta(time_diff, unit="minute")
     time_obj = time_obj.replace(tzinfo=datetime.timezone.utc)
     
     #return get_altitude(lat, lon, time_obj.to_pydatetime())
@@ -274,59 +212,15 @@
 def get_SZA_parallelized(limit, gsize, time_start, time_diff,num_cores=1):
     # limit = [min lat, max lat, min lon, max lon]
     max_lat = int(1+round(((limit[1]-limit[0])/gsize)))
     max_lon = int(1+round(((limit[3]-limit[2])/gsize)))
             
     #solar_zenith = Parallel(n_jobs=num_cores)([get_SZA(limit[0] +  i * gsize, limit[2] + j * gsize, time_start, time_diff) for j in range(0, max_lon)] for i in range(0, max_lat))
     #res = Parallel(n_jobs=1)(delayed(math.sqrt)(i**2) for i in range(10))
-    if (len(cuda.list_devices()) != 0):
-        datetime_obj = pd.to_datetime(time_start)
-        datetime_obj = datetime_obj.replace(tzinfo=datetime.timezone.utc)   
-        D, time = date_to_num(datetime_obj)
-
-        lats = np.array([[limit[0] +  i * gsize for j in range(0, max_lon)] for i in range(0, max_lat)]).flatten()
-        lons = np.array([[limit[2] +  j * gsize for j in range(0, max_lon)] for i in range(0, max_lat)]).flatten()
-        N = len(lats)
-        sza = np.zeros(N)
-
-        d_lats = cuda.to_device(lats)
-        d_lons = cuda.to_device(lons)
-        d_sza = cuda.to_device(sza)
-
-        tpb = (256)
-        bpg = (int(np.ceil(N / tpb)))
-        get_SZA_GPU[bpg, tpb](d_lats, d_lons, N, D, time, d_sza, rad)
-
-        sza = d_sza.copy_to_host()
-        return sza
-
-        
     res = Parallel(n_jobs = num_cores)( 
             delayed( get_SZA )(limit[0] +  i * gsize, limit[2] + j * gsize, time_start, time_diff) 
                                     for i in range(0, max_lat)
                                     for j in range(0, max_lon)
         )
     
     res = np.reshape(res, (-1, max_lon))
     return res #solar_zenith
-
-if __name__ == '__main__':
-    limit = [-90, 90, -180, 180]
-    #limit = [-10, 10, -20, 20]
-    gsize = 0.25
-    time_start = "2020-01-01 00:00:00"
-    time_diff = 30
-    
-    time_obj = pd.to_datetime(time_start) + pd.to_timedelta(time_diff, unit="minute")
-    print(time_obj)
-    
-    #testing manual pysolar calculations
-    latitude = 39.01#37.7749 # San Francisco latitude
-    longitude = -77.01#-122.4194 # San Francisco longitude
-    datetime_obj = datetime.datetime(2023, 2, 23, 10, 14, 0) # February 17, 2023 at 12:00 PM
-
-    theta = get_SZA(latitude, longitude, datetime_obj)
-    print("Solar zenith angle (manual):", theta, "degrees")
-    datetime_obj = datetime_obj.replace(tzinfo=datetime.timezone.utc)
-    print("Solar zenith angle (pysolar): ", 90 - get_altitude(latitude, longitude, datetime_obj))
-    
-
```

### Comparing `pyroscope_gridtools-0.0.3/pyroscope_gridtools.egg-info/PKG-INFO` & `Pyroscope-gridtools-0.1/Pyroscope_gridtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: pyroscope-gridtools
-Version: 0.0.3
+Name: Pyroscope-gridtools
+Version: 0.1
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

