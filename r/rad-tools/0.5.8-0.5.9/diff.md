# Comparing `tmp/rad-tools-0.5.8.tar.gz` & `tmp/rad-tools-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-tools-0.5.8.tar", last modified: Fri Mar  3 14:31:24 2023, max compression
+gzip compressed data, was "rad-tools-0.5.9.tar", last modified: Fri Mar  3 15:58:13 2023, max compression
```

## Comparing `rad-tools-0.5.8.tar` & `rad-tools-0.5.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 14:31:24.187809 rad-tools-0.5.8/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.5.8/LICENSE.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1230 2023-03-03 14:31:24.187513 rad-tools-0.5.8/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      545 2022-11-15 22:40:46.000000 rad-tools-0.5.8/README.rst
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 14:31:24.158558 rad-tools-0.5.8/rad_tools/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       60 2023-03-03 12:55:44.000000 rad-tools-0.5.8/rad_tools/__init__.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 14:31:24.165824 rad-tools-0.5.8/rad_tools/exchange/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      196 2023-02-23 16:19:10.000000 rad-tools-0.5.8/rad_tools/exchange/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7583 2023-02-24 16:56:38.000000 rad-tools-0.5.8/rad_tools/exchange/bond.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    27284 2023-02-24 17:23:45.000000 rad-tools-0.5.8/rad_tools/exchange/model.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1171 2022-12-15 15:38:31.000000 rad-tools-0.5.8/rad_tools/exchange/template.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 14:31:24.169095 rad-tools-0.5.8/rad_tools/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      149 2023-01-18 13:16:00.000000 rad-tools-0.5.8/rad_tools/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1928 2022-12-15 15:43:18.000000 rad-tools-0.5.8/rad_tools/io/internal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3944 2023-02-24 16:56:38.000000 rad-tools-0.5.8/rad_tools/io/tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 14:31:24.173193 rad-tools-0.5.8/rad_tools/kpoints/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      600 2023-02-23 16:19:10.000000 rad-tools-0.5.8/rad_tools/kpoints/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    29021 2023-02-23 16:19:10.000000 rad-tools-0.5.8/rad_tools/kpoints/high_symmetry_point.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3775 2023-02-23 16:19:10.000000 rad-tools-0.5.8/rad_tools/kpoints/kpoints.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1357 2022-12-15 17:25:30.000000 rad-tools-0.5.8/rad_tools/map.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     6817 2023-02-24 16:56:38.000000 rad-tools-0.5.8/rad_tools/routines.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 14:31:24.176496 rad-tools-0.5.8/rad_tools/score/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      266 2023-02-24 16:56:38.000000 rad-tools-0.5.8/rad_tools/score/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    37572 2023-03-03 13:25:21.000000 rad-tools-0.5.8/rad_tools/score/rad_dos_plotter_core.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5097 2023-03-03 13:21:07.000000 rad-tools-0.5.8/rad_tools/score/rad_make_template_core.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5474 2023-03-03 13:20:04.000000 rad-tools-0.5.8/rad_tools/score/tb2j_extractor_core.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    10167 2023-03-03 13:16:39.000000 rad-tools-0.5.8/rad_tools/score/tb2j_plotter_core.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 14:31:24.161392 rad-tools-0.5.8/rad_tools.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1230 2023-03-03 14:31:24.000000 rad-tools-0.5.8/rad_tools.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      927 2023-03-03 14:31:24.000000 rad-tools-0.5.8/rad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-03-03 14:31:24.000000 rad-tools-0.5.8/rad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       17 2023-03-03 14:31:24.000000 rad-tools-0.5.8/rad_tools.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       10 2023-03-03 14:31:24.000000 rad-tools-0.5.8/rad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 14:31:24.186349 rad-tools-0.5.8/scripts/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3167 2023-02-23 16:19:10.000000 rad-tools-0.5.8/scripts/compute-energies.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5014 2023-03-03 14:19:40.000000 rad-tools-0.5.8/scripts/identify-wannier-centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3051 2023-02-23 16:19:10.000000 rad-tools-0.5.8/scripts/phonopy-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      207 2023-03-03 00:32:48.000000 rad-tools-0.5.8/scripts/rad-dos-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      209 2023-02-24 16:56:38.000000 rad-tools-0.5.8/scripts/rad-make-template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      206 2023-02-24 16:56:38.000000 rad-tools-0.5.8/scripts/tb2j-extractor.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      204 2023-02-24 16:56:38.000000 rad-tools-0.5.8/scripts/tb2j-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-03-03 14:31:24.187901 rad-tools-0.5.8/setup.cfg
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1369 2023-02-23 16:19:10.000000 rad-tools-0.5.8/setup.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.609304 rad-tools-0.5.9/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.5.9/LICENSE.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1230 2023-03-03 15:58:13.608927 rad-tools-0.5.9/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      545 2022-11-15 22:40:46.000000 rad-tools-0.5.9/README.rst
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.584511 rad-tools-0.5.9/rad_tools/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       60 2023-03-03 15:56:31.000000 rad-tools-0.5.9/rad_tools/__init__.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.593174 rad-tools-0.5.9/rad_tools/exchange/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      196 2023-02-23 16:19:10.000000 rad-tools-0.5.9/rad_tools/exchange/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7583 2023-02-24 16:56:38.000000 rad-tools-0.5.9/rad_tools/exchange/bond.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    27284 2023-02-24 17:23:45.000000 rad-tools-0.5.9/rad_tools/exchange/model.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1171 2022-12-15 15:38:31.000000 rad-tools-0.5.9/rad_tools/exchange/template.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.595674 rad-tools-0.5.9/rad_tools/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      149 2023-01-18 13:16:00.000000 rad-tools-0.5.9/rad_tools/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1928 2022-12-15 15:43:18.000000 rad-tools-0.5.9/rad_tools/io/internal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3944 2023-02-24 16:56:38.000000 rad-tools-0.5.9/rad_tools/io/tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.598597 rad-tools-0.5.9/rad_tools/kpoints/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      600 2023-02-23 16:19:10.000000 rad-tools-0.5.9/rad_tools/kpoints/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    29021 2023-02-23 16:19:10.000000 rad-tools-0.5.9/rad_tools/kpoints/high_symmetry_point.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3775 2023-02-23 16:19:10.000000 rad-tools-0.5.9/rad_tools/kpoints/kpoints.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1357 2022-12-15 17:25:30.000000 rad-tools-0.5.9/rad_tools/map.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     6817 2023-02-24 16:56:38.000000 rad-tools-0.5.9/rad_tools/routines.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.601355 rad-tools-0.5.9/rad_tools/score/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      266 2023-02-24 16:56:38.000000 rad-tools-0.5.9/rad_tools/score/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    38005 2023-03-03 15:47:48.000000 rad-tools-0.5.9/rad_tools/score/rad_dos_plotter_core.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5097 2023-03-03 13:21:07.000000 rad-tools-0.5.9/rad_tools/score/rad_make_template_core.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5474 2023-03-03 13:20:04.000000 rad-tools-0.5.9/rad_tools/score/tb2j_extractor_core.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    10167 2023-03-03 13:16:39.000000 rad-tools-0.5.9/rad_tools/score/tb2j_plotter_core.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.588383 rad-tools-0.5.9/rad_tools.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1230 2023-03-03 15:58:13.000000 rad-tools-0.5.9/rad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      927 2023-03-03 15:58:13.000000 rad-tools-0.5.9/rad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-03-03 15:58:13.000000 rad-tools-0.5.9/rad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       17 2023-03-03 15:58:13.000000 rad-tools-0.5.9/rad_tools.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       10 2023-03-03 15:58:13.000000 rad-tools-0.5.9/rad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-03-03 15:58:13.607980 rad-tools-0.5.9/scripts/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3167 2023-02-23 16:19:10.000000 rad-tools-0.5.9/scripts/compute-energies.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5014 2023-03-03 14:19:40.000000 rad-tools-0.5.9/scripts/identify-wannier-centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3051 2023-02-23 16:19:10.000000 rad-tools-0.5.9/scripts/phonopy-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      207 2023-03-03 00:32:48.000000 rad-tools-0.5.9/scripts/rad-dos-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      209 2023-02-24 16:56:38.000000 rad-tools-0.5.9/scripts/rad-make-template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      206 2023-02-24 16:56:38.000000 rad-tools-0.5.9/scripts/tb2j-extractor.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      204 2023-02-24 16:56:38.000000 rad-tools-0.5.9/scripts/tb2j-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-03-03 15:58:13.609394 rad-tools-0.5.9/setup.cfg
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1369 2023-02-23 16:19:10.000000 rad-tools-0.5.9/setup.py
```

### Comparing `rad-tools-0.5.8/LICENSE.txt` & `rad-tools-0.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/PKG-INFO` & `rad-tools-0.5.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.5.8
+Version: 0.5.9
 Summary: Collection of scripts from my PhD
 Home-page: https://github.com/adrybakov/rad-tools
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.5.8/README.rst` & `rad-tools-0.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools/exchange/bond.py` & `rad-tools-0.5.9/rad_tools/exchange/bond.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools/exchange/model.py` & `rad-tools-0.5.9/rad_tools/exchange/model.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools/exchange/template.py` & `rad-tools-0.5.9/rad_tools/exchange/template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools/io/internal.py` & `rad-tools-0.5.9/rad_tools/io/internal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools/io/tb2j.py` & `rad-tools-0.5.9/rad_tools/io/tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools/kpoints/__init__.py` & `rad-tools-0.5.9/rad_tools/kpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools/kpoints/high_symmetry_point.py` & `rad-tools-0.5.9/rad_tools/kpoints/high_symmetry_point.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools/kpoints/kpoints.py` & `rad-tools-0.5.9/rad_tools/kpoints/kpoints.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools/map.py` & `rad-tools-0.5.9/rad_tools/map.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools/routines.py` & `rad-tools-0.5.9/rad_tools/routines.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools/score/rad_dos_plotter_core.py` & `rad-tools-0.5.9/rad_tools/score/rad_dos_plotter_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,16 @@
                 filenames.append(filename)
         files = filenames
         filpdos = [filpdos]
         filenames = [filenames]
     else:
         filpdos = set()
         for filename in files:
-            if ".pdos_tot" in filename:
-                filpdos.add(filename.split(".pdos_tot")[0])
+            if ".pdos_tot" in filename and ".pdos_tot" == filename[-9:]:
+                filpdos.add(filename[:-9])
                 filenames.append(filename)
             elif ".pdos_atm#" in filename:
                 filpdos.add(filename.split(".pdos_atm#")[0])
                 filenames.append(filename)
         filpdos = list(filpdos)
 
         print(f"Following DOS seednames (filpdos) are detected:{YELLOW}")
@@ -136,14 +136,15 @@
         .. code-block:: python
 
             wfcs = {(atom1, atom1_number): (wfc_label, wfc_number)}
     """
 
     atoms = {}
     wfcs = {}
+    print(filenames)
     for filename in filenames:
 
         # Detect names and numbers
         atom_number = int(filename.split(".pdos_atm#")[1].split("(")[0])
         atom_symbol = filename.split("(")[1].split(")")[0]
         wfc_number = int(filename.split(")_wfc#")[1].split("(")[0])
         wfc_symbol = filename.split(")_wfc#")[1].split("(")[1].split(")")[0]
@@ -539,15 +540,15 @@
             try:
                 makedirs(join(output_path, seedname,
                               "individual-plots", "wfc-in-atoms"))
             except FileExistsError:
                 pass
 
         atoms, wfcs = decompose_filenames(
-            [file for file in files[s_i] if ".pdos_tot" not in file])
+            [file for file in files[s_i] if ".pdos_tot" != file[-9:]])
 
         # Plot PDOS vs DOS
         total_dos = np.loadtxt(join(input_path, f"{seedname}.pdos_tot"),
                                skiprows=1).T
         plot_pdos_tot(total_dos,
                       join(output_path, seedname, "pdos-vs-dos"),
                       case,
@@ -646,14 +647,18 @@
                         custom_dos[1] += wfs_dos[1]
                     custom_dos.append(wfs_dos[1])
                 elif case in [1, 2]:
                     if len(custom_dos) == 1:
                         custom_dos.append(deepcopy(wfs_dos[1]))
                         custom_dos.append(deepcopy(wfs_dos[2]))
                     else:
+                        print(np.array(custom_dos).shape, wfs_dos.shape, join(input_path,
+                                                                              seedname,
+                                                                              "summed-by-atom",
+                                                                              f"{atom}_wfc#{wfc_number}({wfc_symbol})"))
                         custom_dos[1] += wfs_dos[1]
                         custom_dos[2] += wfs_dos[2]
                     custom_dos.append(wfs_dos[1])
                     custom_dos.append(wfs_dos[2])
             if efermi == 0:
                 title = f"wfc contribution to {atom} (0 is 0)"
             else:
```

### Comparing `rad-tools-0.5.8/rad_tools/score/rad_make_template_core.py` & `rad-tools-0.5.9/rad_tools/score/rad_make_template_core.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools/score/tb2j_extractor_core.py` & `rad-tools-0.5.9/rad_tools/score/tb2j_extractor_core.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools/score/tb2j_plotter_core.py` & `rad-tools-0.5.9/rad_tools/score/tb2j_plotter_core.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/rad_tools.egg-info/PKG-INFO` & `rad-tools-0.5.9/rad_tools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.5.8
+Version: 0.5.9
 Summary: Collection of scripts from my PhD
 Home-page: https://github.com/adrybakov/rad-tools
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.5.8/rad_tools.egg-info/SOURCES.txt` & `rad-tools-0.5.9/rad_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/scripts/compute-energies.py` & `rad-tools-0.5.9/scripts/compute-energies.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/scripts/identify-wannier-centres.py` & `rad-tools-0.5.9/scripts/identify-wannier-centres.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/scripts/phonopy-plotter.py` & `rad-tools-0.5.9/scripts/phonopy-plotter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.5.8/setup.py` & `rad-tools-0.5.9/setup.py`

 * *Files identical despite different names*

