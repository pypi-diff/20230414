# Comparing `tmp/pyscancf-1.0.7-py3-none-any.whl.zip` & `tmp/pyscancf-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3965 bytes, number of entries: 6
+Zip file size: 5526 bytes, number of entries: 6
 -rw-r--r--  2.0 unx        0 b- defN 21-Oct-16 17:39 pyscancf/__init__.py
--rw-r--r--  2.0 unx     5034 b- defN 21-Oct-17 21:30 pyscancf/pyscancf.py
--rw-r--r--  2.0 unx     2342 b- defN 21-Oct-17 21:39 pyscancf-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Oct-17 21:39 pyscancf-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 21-Oct-17 21:39 pyscancf-1.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      452 b- defN 21-Oct-17 21:39 pyscancf-1.0.7.dist-info/RECORD
-6 files, 7929 bytes uncompressed, 3143 bytes compressed:  60.4%
+-rw-r--r--  2.0 unx    10444 b- defN 21-Oct-18 11:16 pyscancf/pyscancf.py
+-rw-r--r--  2.0 unx     2375 b- defN 21-Oct-18 11:20 pyscancf-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Oct-18 11:20 pyscancf-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 21-Oct-18 11:20 pyscancf-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      453 b- defN 21-Oct-18 11:20 pyscancf-1.0.9.dist-info/RECORD
+6 files, 13373 bytes uncompressed, 4704 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pyscancf/__init__.py
 Comment: 
 
 Filename: pyscancf/pyscancf.py
 Comment: 
 
-Filename: pyscancf-1.0.7.dist-info/METADATA
+Filename: pyscancf-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pyscancf-1.0.7.dist-info/WHEEL
+Filename: pyscancf-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pyscancf-1.0.7.dist-info/top_level.txt
+Filename: pyscancf-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pyscancf-1.0.7.dist-info/RECORD
+Filename: pyscancf-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyscancf/pyscancf.py

```diff
@@ -1,50 +1,170 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-# In[2]:
-
-
-#!/usr/bin/env python
-# coding: utf-8
-
 # ### Author: Syed Hamid Ali - hamidsyed37@gmail.com
 # #### Importing Libraries
-print('If you are using this software for publication please cite, \nHA Syed, Imran Sayyed, & MCR Kalapureddy. (2021). PyScanCf - \nThe library for IMD radar single sweep data (1.0.6). Zenodo. https://doi.org/10.5281/zenodo.5574160')
 print('Importing Libraries')
 import warnings
 warnings.filterwarnings('ignore')
 import datetime as dt
 tstart = dt.datetime.now()
 import numpy as np
+import matplotlib.pyplot as plt
+plt.style.use("dark_background")
 from netCDF4 import Dataset
+from netCDF4 import num2date
 import glob
 import os
 import pyart
 from pyart.config import get_metadata
-import warnings
+from matplotlib import axes
+from matplotlib.ticker import NullFormatter
+import cartopy.crs as ccrs
+import cartopy.feature as feat
+from cartopy.mpl.gridliner import LONGITUDE_FORMATTER, LATITUDE_FORMATTER
 warnings.filterwarnings('ignore')
 print('Importing Libraries Done')
 
+def plot_cappi(grid,prod,**kwargs):
+    max_c = grid.fields[prod]['data'].max(axis=0)
+    max_x = grid.fields[prod]['data'].max(axis=1)
+    max_y = grid.fields[prod]['data'].max(axis=2).T
+    trgx = grid.x['data']
+    trgy = grid.y['data']
+    trgz = grid.z['data']
+    
+    if prod == 'REF':
+        cmap='pyart_NWSRef'
+        levels=range(10,60)
+        stitle='Max-Z'
+        munit = 'dBZ'
+        
+    if prod == 'VELH':
+        cmap='pyart_NWSVel'
+        levels=range(-30,31)
+        stitle='Max-V'
+        munit = 'm/s'
+
+    if  prod == 'WIDTHH':
+        cmap='pyart_NWS_SPW'
+        levels=np.linspace(0,5,9)
+        stitle='Max-W'
+        munit = 'm/s'
+
+    print('Generating Figures of Max-CAPPI, please be patient!')
+    fig = plt.figure(figsize=(10.3,10))
+    # define axes
+    left, bottom, width, height = 0.1, 0.1, 0.6, 0.2
+    left, bottom, width, height = 0.1, 0.1, 0.6, 0.2
+    ax_xy = plt.axes((left, bottom, width, width),
+                     projection=ccrs.AzimuthalEquidistant(
+                         grid.origin_longitude['data'][0],
+                         grid.origin_latitude['data'][0]))
+    ax_x = plt.axes((left, bottom + width, width, height))
+    ax_y = plt.axes((left + width, bottom, height, width))
+    ax_cnr = plt.axes((left+width, bottom + width, left+left,height))
+    ax_cb = plt.axes((left + width + height + 0.02, bottom, 0.02, width))
+
+    # set axis label formatters
+    ax_x.xaxis.set_major_formatter(NullFormatter())
+    ax_y.yaxis.set_major_formatter(NullFormatter())
+    ax_cnr.yaxis.set_major_formatter(NullFormatter())
+    ax_cnr.xaxis.set_major_formatter(NullFormatter())
 
-# In[3]:
+    # label axes
+    # ax_xy.set_xlabel("Longitude [°E]",fontsize=15)
+    # ax_xy.set_ylabel("Latitude [°N]",fontsize=15)
+    # ax_x.set_xlabel("")
+    ax_x.set_ylabel("Height AMSL (km)",fontsize=15)
+    # ax_y.set_ylabel("")
+    ax_y.set_xlabel("Height AMSL (km)",fontsize=15)
 
+    # draw CAPPI
+    plt.sca(ax_xy)
+    xy = ax_xy.contourf(trgx,trgy,max_c,cmap=cmap,levels=levels,**kwargs)
+    gl = ax_xy.gridlines(crs=ccrs.PlateCarree(), linewidth=1, color='black', alpha=0.5, 
+                         linestyle='--', draw_labels=True)
+    gl.xlabels_top = False
+    gl.ylabels_left = True
+    gl.ylabels_right=False
+    gl.xlines = False
+    gl.ylines = False
+    gl.xformatter = LONGITUDE_FORMATTER
+    gl.yformatter = LATITUDE_FORMATTER
+    gl.xlabel_style = {'weight': 'bold'}
+    gl.ylabel_style = {'weight': 'bold'}
+
+    # ax_xy.add_feature(shape_feature)
+    ax_xy.add_feature(feat.COASTLINE,color='w',alpha=0.7)
+    [ax_xy.plot(r * np.cos(np.arange(0,360) * np.pi / 180), 
+             r * np.sin(np.arange(0,360) * np.pi / 180), 'w--', 
+                linewidth=1, alpha=0.5) for r in np.arange(5e4,30e4,5e4)]
+    ax_xy.set_xlim(-2.5e5,2.5e5)
+    ax_xy.set_ylim(-2.5e5,2.5e5)
+    ax_xy.plot([0,0],[-10e3,10e3],'w-')
+    ax_xy.plot([-10e3,10e3],[0,0],'w-')
+
+    # draw colorbar
+    cb = plt.colorbar(xy, cax=ax_cb)
+    cb.set_label(munit,fontsize=15)
+
+    plt.sca(ax_x)
+    plt.contourf(trgx/1e3,trgz/1e3,max_x,cmap=cmap,levels=levels)
+    # plt.ylim(0,20)
+    # plt.yticks([0,5,10,15,20])
+    # plt.grid(axis='y')
+    ax_x.set_xlim(-250,250)
+
+    plt.sca(ax_y)
+    plt.contourf(trgz/1e3,trgy/1e3,max_y,cmap=cmap,levels=levels)
+    # plt.xlim(0,20)
+    ax_y.set_xticks([5,10,15,20])
+    # plt.grid(axis='x')
+    ax_y.set_ylim(-250,250)
+
+    plt.sca(ax_cnr)
+    plt.tick_params(
+        axis='both',          # changes apply to the x-axis
+        which='both',      # both major and minor ticks are affected
+        bottom=False,      # ticks along the bottom edge are off
+        top=False,         # ticks along the top edge are off
+        left=False,
+        right=False,
+        labelbottom=False)
+    # labels along the bottom edge are off
+    plt.text(0.34,0.8, stitle, size=14, weight='bold')
+    plt.text(0.09,0.65,'Max Range: 200 km',fontsize=12)
+    plt.text(0.12,0.5,'VPR Height: 20 km',fontsize=12)
+    plt.text(0.15,0.3,num2date(grid.time['data'],
+                                grid.time['units'])[0].strftime('%H:%M:%S Z'),
+             weight='bold',fontsize=17)
+    plt.text(0.06,0.15,num2date(grid.time['data'],
+                                grid.time['units'])[0].strftime('%d %b, %Y UTC'),
+             fontsize=14)
+    ax_xy.set_aspect('auto')
+    plt.savefig(out_dir+'//'+stitle+'_'+grid.metadata['instrument_name']+num2date(grid.time['data'],
+                                                 grid.time['units'])[0].strftime('%Y%m%d%H%M%S')+'.jpg',
+                dpi=100,bbox_inches='tight')
+    print(f'Figures saved in {out_dir} directory',)
 
 def get_grid(radar):
     """ Returns grid object from radar object. """
     grid = pyart.map.grid_from_radars(
         radar, grid_shape=(40, 500, 500),
         grid_limits=((radar.altitude['data'][0], 2e4), (-2.5e5, 2.5e5), (-2.5e5, 2.5e5)),
         fields=radar.fields.keys(), weighting_function='Barnes2', min_radius=250.)
     return grid
 
-def cfrad(input_dir,output_dir):
+def cfrad(input_dir,output_dir,gridder=True,plot=None):
     '''
-        input_dir = str, Enter path of single sweep data directory
-        output_dir = str, Enter the path for output data
+        input_dir --> str - Enter path of single sweep data directory,
+        output_dir --> str - Enter the path for output data,
+        gridder --> bool - True, False,
+        plot --> 'REF', 'VELH', 'WIDTHH', 'ALL',
     '''
     in_dir=input_dir
     out_dir=output_dir
     files = sorted(glob.glob(in_dir+'//'+'*nc*'))
     print('Number of files: ', len(files))
     bb = list()
     for i in range(0,len(files),10):
@@ -68,16 +188,22 @@
             t1.extend(time)
             e1.extend(ele)
             Z1.extend(Z)
             T1.extend(T)
             V1.extend(V)
             W1.extend(W)
             en.append(EN)
+
+        if len(bb[i][0].split('/')[-1]) < 30:
+            fname = bb[i][0].split('/')[-1].split('-')[0]
+        else:
+            fname = bb[i][0].split('\\')[-1].split('-')[0]
+
         radar = pyart.testing.make_empty_ppi_radar(ds.dimensions['bin'].size,
-                                               ds.dimensions['radial'].size*10, 1)
+                                                   ds.dimensions['radial'].size*10, 1)
         radar.nsweeps = 10
         radar.time['data'] = np.array(t1)
         radar.time['units'] = ds.variables['radialTime'].units#'seconds since 1970-01-01T00:00:00Z'
         radar.latitude['data'] = np.array([ds.variables['siteLat'][:]])
         radar.longitude['data'] = np.array([ds.variables['siteLon'][:]])
         radar.altitude['data'] = np.array([ds.variables['siteAlt'][:]])
         radar.range['data'] = np.arange(0,
@@ -85,32 +211,47 @@
                                         int(ds.variables['gateSize'][:].data))
         radar.fixed_angle['data'] = ds.variables['elevationList']
         radar.sweep_number['data'] = np.array(en)
         radar.sweep_start_ray_index['data'] = np.arange(0,
                                                         ds.dimensions['radial'].size*10,
                                                         ds.dimensions['radial'].size)
         radar.sweep_end_ray_index['data'] = np.arange(ds.dimensions['radial'].size-1,
-                                                    ds.dimensions['radial'].size*10,
-                                                    ds.dimensions['radial'].size)
+                                                      ds.dimensions['radial'].size*10,
+                                                      ds.dimensions['radial'].size)
         radar.azimuth['data'] = np.ma.array(a1)
         radar.elevation['data'] = np.ma.array(e1)
-        radar.metadata['instrument_name'] = files[0][-24:-21]
+        radar.metadata['instrument_name'] = fname[:3]
         radar.init_gate_altitude()
         radar.init_gate_longitude_latitude()
         ref_dict = get_metadata('reflectivity')
         ref_dict['data'] = np.ma.array(Z1)
         ref_dict['units'] = 'dBZ'
         radar.fields = {'REF': ref_dict}
-        radar.metadata['instrument_name'] = 'GOA'
         VELH_dict = {'units':'m/s','standard_name':'Radial Velocity','data':np.ma.array(V1),}
         radar.add_field('VELH',VELH_dict,replace_existing=True)
         W_dict = {'units':'m/s','standard_name':'Spectral Width','data':np.ma.array(W1),}
         radar.add_field('WIDTHH',W_dict,replace_existing=True)
         T_dict = {'units':'dBT','standard_name':'Total Power','data':np.ma.array(T1),}
         radar.add_field('TP',T_dict,replace_existing=True)
-        pyart.io.write_cfradial(out_dir+'/Polar_'+bb[i][0][-24:], radar, 
+        pyart.io.write_cfradial(out_dir+'//'+'polar_'+fname+'.nc', radar, 
                                 format = 'NETCDF4',time_reference=None, arm_time_variables=False)
-        grid = get_grid(radar)
-        pyart.io.write_grid(out_dir+'/grid_'+bb[i][0][-24:], grid)
-        del radar, grid 
-    print('Data merging done \nAll Done \nTotal Time Elapsed: ', dt.datetime.now()-tstart)
-
+        if gridder == True:
+            grid = get_grid(radar)
+            
+            if plot != None:
+                if plot == 'REF':
+                    plot_cappi(grid,'REF')
+                if plot == 'VELH':
+                    plot_cappi(grid,'VELH')
+                if plot == 'WIDTHH':
+                    plot_cappi(grid,'WIDTHH')
+                if plot == 'ALL':
+                    plot_cappi(grid,'REF')
+                    plot_cappi(grid,'VELH')
+                    plot_cappi(grid,'WIDTHH')                
+            else:
+                pass
+            pyart.io.write_grid(out_dir+'//'+'grid_'+fname+'.nc', grid)
+            del radar, grid
+        else:
+            pass
+    print('Data merging done \nTotal Time Elapsed: ', dt.datetime.now()-tstart)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `pyscancf-1.0.7.dist-info/METADATA` & `pyscancf-1.0.9.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pyscancf
-Version: 1.0.7
+Version: 1.0.9
 Summary: Creates PyArt compatible cf-radial data from single scans of IMD Radar data
 Home-page: https://github.com/syedhamidali/PyScanCf
 Author: Syed Hamid Ali
 License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/RBhupi/PyREClass/issues
-Project-URL: Source, https://github.com/RBhupi/PyREClass/
+Project-URL: Bug Reports, https://github.com/syedhamidali/PyScanCf/issues
+Project-URL: Source, https://github.com/syedhamidali/PyScanCf/
 Keywords: IMD Radar cf-radial single sweeps radar weather meteorology
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: arm-pyart
 Requires-Dist: netCDF4
+Requires-Dist: cartopy
 
 # PyScanCf
 
 Creates PyArt compatible cf-radial data from single scans of IMD Radar data
 
 ## Description
 
@@ -46,10 +47,10 @@
     git clone https://github.com/syedhamidali/PyScanCf.git
     python setup.py install --user
 
 ## Reference
 [![DOI](https://zenodo.org/badge/417933645.svg)](https://zenodo.org/badge/latestdoi/417933645)
 
 ### Cite as
-HA Syed, Imran Sayyed, & MCR Kalapureddy. (2021). PyScanCf - The library for IMD radar single sweep data (1.0.6). Zenodo. https://doi.org/10.5281/zenodo.5574305
+HA Syed, Imran Sayyed, & MCR Kalapureddy. (2021). PyScanCf - The library for IMD radar single sweep data (1.0.9). Zenodo. https://doi.org/10.5281/zenodo.5574305
```

