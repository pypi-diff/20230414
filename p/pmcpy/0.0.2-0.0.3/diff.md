# Comparing `tmp/pmcpy-0.0.2.tar.gz` & `tmp/pmcpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmcpy-0.0.2.tar", last modified: Sun Apr 17 01:38:16 2022, max compression
+gzip compressed data, was "pmcpy-0.0.3.tar", last modified: Fri Apr 14 10:03:30 2023, max compression
```

## Comparing `pmcpy-0.0.2.tar` & `pmcpy-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhonghuazheng   (501) staff       (20)        0 2022-04-17 01:38:16.677752 pmcpy-0.0.2/
--rw-r--r--   0 zhonghuazheng   (501) staff       (20)     1071 2021-09-23 03:13:26.000000 pmcpy-0.0.2/LICENSE
--rw-r--r--   0 zhonghuazheng   (501) staff       (20)     2694 2022-04-17 01:38:16.677536 pmcpy-0.0.2/PKG-INFO
--rw-r--r--   0 zhonghuazheng   (501) staff       (20)     2076 2022-04-17 01:24:09.000000 pmcpy-0.0.2/README.rst
-drwxr-xr-x   0 zhonghuazheng   (501) staff       (20)        0 2022-04-17 01:38:16.676432 pmcpy-0.0.2/pmcpy/
--rw-r--r--   0 zhonghuazheng   (501) staff       (20)       41 2021-09-23 03:20:03.000000 pmcpy-0.0.2/pmcpy/__init__.py
--rw-r--r--   0 zhonghuazheng   (501) staff       (20)    10858 2022-04-16 21:46:04.000000 pmcpy-0.0.2/pmcpy/pmcpy.py
-drwxr-xr-x   0 zhonghuazheng   (501) staff       (20)        0 2022-04-17 01:38:16.677323 pmcpy-0.0.2/pmcpy.egg-info/
--rw-r--r--   0 zhonghuazheng   (501) staff       (20)     2694 2022-04-17 01:38:16.000000 pmcpy-0.0.2/pmcpy.egg-info/PKG-INFO
--rw-r--r--   0 zhonghuazheng   (501) staff       (20)      204 2022-04-17 01:38:16.000000 pmcpy-0.0.2/pmcpy.egg-info/SOURCES.txt
--rw-r--r--   0 zhonghuazheng   (501) staff       (20)        1 2022-04-17 01:38:16.000000 pmcpy-0.0.2/pmcpy.egg-info/dependency_links.txt
--rw-r--r--   0 zhonghuazheng   (501) staff       (20)       28 2022-04-17 01:38:16.000000 pmcpy-0.0.2/pmcpy.egg-info/requires.txt
--rw-r--r--   0 zhonghuazheng   (501) staff       (20)        6 2022-04-17 01:38:16.000000 pmcpy-0.0.2/pmcpy.egg-info/top_level.txt
--rw-r--r--   0 zhonghuazheng   (501) staff       (20)       38 2022-04-17 01:38:16.677811 pmcpy-0.0.2/setup.cfg
--rw-r--r--   0 zhonghuazheng   (501) staff       (20)      890 2022-04-17 01:16:04.000000 pmcpy-0.0.2/setup.py
+drwxr-xr-x   0 zhonghuazheng   (501) staff       (20)        0 2023-04-14 10:03:30.002089 pmcpy-0.0.3/
+-rw-r--r--   0 zhonghuazheng   (501) staff       (20)     1071 2023-04-14 10:00:47.000000 pmcpy-0.0.3/LICENSE
+-rw-r--r--   0 zhonghuazheng   (501) staff       (20)     2700 2023-04-14 10:03:30.001748 pmcpy-0.0.3/PKG-INFO
+-rw-r--r--   0 zhonghuazheng   (501) staff       (20)     2076 2023-04-14 10:00:47.000000 pmcpy-0.0.3/README.rst
+drwxr-xr-x   0 zhonghuazheng   (501) staff       (20)        0 2023-04-14 10:03:30.000171 pmcpy-0.0.3/pmcpy/
+-rw-r--r--   0 zhonghuazheng   (501) staff       (20)       41 2023-04-14 10:00:47.000000 pmcpy-0.0.3/pmcpy/__init__.py
+-rw-r--r--   0 zhonghuazheng   (501) staff       (20)    11947 2023-04-14 10:00:47.000000 pmcpy-0.0.3/pmcpy/pmcpy.py
+drwxr-xr-x   0 zhonghuazheng   (501) staff       (20)        0 2023-04-14 10:03:30.001468 pmcpy-0.0.3/pmcpy.egg-info/
+-rw-r--r--   0 zhonghuazheng   (501) staff       (20)     2700 2023-04-14 10:03:29.000000 pmcpy-0.0.3/pmcpy.egg-info/PKG-INFO
+-rw-r--r--   0 zhonghuazheng   (501) staff       (20)      204 2023-04-14 10:03:29.000000 pmcpy-0.0.3/pmcpy.egg-info/SOURCES.txt
+-rw-r--r--   0 zhonghuazheng   (501) staff       (20)        1 2023-04-14 10:03:29.000000 pmcpy-0.0.3/pmcpy.egg-info/dependency_links.txt
+-rw-r--r--   0 zhonghuazheng   (501) staff       (20)       28 2023-04-14 10:03:29.000000 pmcpy-0.0.3/pmcpy.egg-info/requires.txt
+-rw-r--r--   0 zhonghuazheng   (501) staff       (20)        6 2023-04-14 10:03:29.000000 pmcpy-0.0.3/pmcpy.egg-info/top_level.txt
+-rw-r--r--   0 zhonghuazheng   (501) staff       (20)       38 2023-04-14 10:03:30.002177 pmcpy-0.0.3/setup.cfg
+-rw-r--r--   0 zhonghuazheng   (501) staff       (20)      896 2023-04-14 10:00:47.000000 pmcpy-0.0.3/setup.py
```

### Comparing `pmcpy-0.0.2/LICENSE` & `pmcpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pmcpy-0.0.2/PKG-INFO` & `pmcpy-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pmcpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for PartMC post-processing
-Home-page: https://github.com/zzheng93/pmcpy
+Home-page: https://github.com/zhonghua-zheng/pmcpy
 Author: Zhonghua Zheng
 Author-email: zhonghua.zheng@outlook.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pmcpy-0.0.2/README.rst` & `pmcpy-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pmcpy-0.0.2/pmcpy/pmcpy.py` & `pmcpy-0.0.3/pmcpy/pmcpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,40 @@
         # calcuate the number concentration per particle, then add them up
         if part_cond is not None:
             # apply the additional condition
             return (self.ds["aero_num_conc"].values[part_cond]).sum()
         else:
             return self.ds["aero_num_conc"].values.sum()
     
+    def get_aero_mass_conc(self, aero_species_ls, part_cond=None):
+        """get aerosol mass concentration of the selected species
+
+        Parameters
+        ----------
+        aero_species_ls : a list of string
+            a list of aerosol species, e.g., ["BC","OC"]
+
+        part_cond : a boolean numpy array, optional
+            a bolleann numpy with the same length of "aero_particle", by default None
+
+        Returns
+        -------
+        numpy.float64
+            [kg m^{-3}], aerosol mass concentration of the selected species
+        """
+        # get the mass per particle [kg]
+        mass_per_particle = self.ds["aero_particle_mass"].sel(aero_species = self.aero_species_to_idx(aero_species_ls)).values  
+        
+        # calcuate the mass concentration per particle, then add them up
+        if part_cond is not None:
+            # apply the additional condition
+            return (((self.ds["aero_num_conc"].values)*(mass_per_particle))[:,part_cond]).sum(axis=1)
+        else:
+            return ((self.ds["aero_num_conc"].values)*(mass_per_particle)).sum(axis=1)
+
     def get_mass_conc(self, dry=True, part_cond=None):
         """get mass concentration of the population
 
         Parameters
         ----------
         dry : bool, optional
             consider H2O or not, by default True
```

### Comparing `pmcpy-0.0.2/pmcpy.egg-info/PKG-INFO` & `pmcpy-0.0.3/pmcpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pmcpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for PartMC post-processing
-Home-page: https://github.com/zzheng93/pmcpy
+Home-page: https://github.com/zhonghua-zheng/pmcpy
 Author: Zhonghua Zheng
 Author-email: zhonghua.zheng@outlook.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pmcpy-0.0.2/setup.py` & `pmcpy-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,18 @@
     ]
 
 with open("README.rst", "r") as fp:
     long_description = fp.read()
 
 setup(
     name="pmcpy",
-    version="0.0.2",
+    version="0.0.3",
     author="Zhonghua Zheng",
     author_email="zhonghua.zheng@outlook.com",
-    url="https://github.com/zzheng93/pmcpy",
+    url="https://github.com/zhonghua-zheng/pmcpy",
     description="A Python package for PartMC post-processing",
     long_description=long_description,
     license="MIT",
     classifiers=classifiers,
     install_requires=['numpy', 'pandas', 'netcdf4', 'xarray'],
     packages=find_packages(),
     )
```

