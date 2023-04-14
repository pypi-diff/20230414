# Comparing `tmp/seagal-2.1.tar.gz` & `tmp/seagal-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagal-2.1.tar", last modified: Wed Apr  5 19:57:40 2023, max compression
+gzip compressed data, was "seagal-2.2.tar", last modified: Fri Apr 14 14:13:57 2023, max compression
```

## Comparing `seagal-2.1.tar` & `seagal-2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-04-05 19:57:40.413605 seagal-2.1/
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     1068 2023-02-11 05:25:59.000000 seagal-2.1/LICENSE
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3623 2023-04-05 19:57:40.409605 seagal-2.1/PKG-INFO
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3231 2023-02-11 05:37:25.000000 seagal-2.1/README.md
-drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-04-05 19:57:40.409605 seagal-2.1/seagal/
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        0 2023-02-11 05:26:14.000000 seagal-2.1/seagal/__init__.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3089 2023-02-11 05:26:14.000000 seagal-2.1/seagal/_gmod.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     4228 2023-04-05 19:57:00.000000 seagal-2.1/seagal/_plotting.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)    15538 2023-04-05 19:57:02.000000 seagal-2.1/seagal/_utils.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)    11553 2023-02-11 05:26:14.000000 seagal-2.1/seagal/lee_vec.py
-drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-04-05 19:57:40.409605 seagal-2.1/seagal/modules/
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        0 2023-02-11 05:26:14.000000 seagal-2.1/seagal/modules/__init__.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3113 2023-02-11 05:26:14.000000 seagal-2.1/seagal/modules/gmod.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)      978 2023-02-11 05:26:14.000000 seagal-2.1/seagal/seagal.py
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     6442 2023-02-11 05:26:14.000000 seagal-2.1/seagal/spatial_measure.py
-drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-04-05 19:57:40.409605 seagal-2.1/seagal.egg-info/
--rw-rw-r--   0 linhua    (1008) linhua    (1010)     3623 2023-04-05 19:57:40.000000 seagal-2.1/seagal.egg-info/PKG-INFO
--rw-rw-r--   0 linhua    (1008) linhua    (1010)      387 2023-04-05 19:57:40.000000 seagal-2.1/seagal.egg-info/SOURCES.txt
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        1 2023-04-05 19:57:40.000000 seagal-2.1/seagal.egg-info/dependency_links.txt
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        1 2023-02-11 05:26:14.000000 seagal-2.1/seagal.egg-info/not-zip-safe
--rw-rw-r--   0 linhua    (1008) linhua    (1010)       98 2023-04-05 19:57:40.000000 seagal-2.1/seagal.egg-info/requires.txt
--rw-rw-r--   0 linhua    (1008) linhua    (1010)        7 2023-04-05 19:57:40.000000 seagal-2.1/seagal.egg-info/top_level.txt
--rw-rw-r--   0 linhua    (1008) linhua    (1010)       38 2023-04-05 19:57:40.413605 seagal-2.1/setup.cfg
--rw-rw-r--   0 linhua    (1008) linhua    (1010)      824 2023-04-05 19:56:59.000000 seagal-2.1/setup.py
+drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-04-14 14:13:57.214665 seagal-2.2/
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     1068 2023-02-11 05:25:59.000000 seagal-2.2/LICENSE
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3623 2023-04-14 14:13:57.214665 seagal-2.2/PKG-INFO
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3231 2023-02-11 05:37:25.000000 seagal-2.2/README.md
+drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-04-14 14:13:57.214665 seagal-2.2/seagal/
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        0 2023-02-11 05:26:14.000000 seagal-2.2/seagal/__init__.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3089 2023-02-11 05:26:14.000000 seagal-2.2/seagal/_gmod.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     4228 2023-04-05 19:57:00.000000 seagal-2.2/seagal/_plotting.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)    15595 2023-04-10 19:15:59.000000 seagal-2.2/seagal/_utils.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)    11553 2023-02-11 05:26:14.000000 seagal-2.2/seagal/lee_vec.py
+drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-04-14 14:13:57.214665 seagal-2.2/seagal/modules/
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        0 2023-02-11 05:26:14.000000 seagal-2.2/seagal/modules/__init__.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3113 2023-02-11 05:26:14.000000 seagal-2.2/seagal/modules/gmod.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)      978 2023-02-11 05:26:14.000000 seagal-2.2/seagal/seagal.py
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     6633 2023-04-10 19:11:32.000000 seagal-2.2/seagal/spatial_measure.py
+drwxrwxr-x   0 linhua    (1008) linhua    (1010)        0 2023-04-14 14:13:57.214665 seagal-2.2/seagal.egg-info/
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)     3623 2023-04-14 14:13:57.000000 seagal-2.2/seagal.egg-info/PKG-INFO
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)      387 2023-04-14 14:13:57.000000 seagal-2.2/seagal.egg-info/SOURCES.txt
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        1 2023-04-14 14:13:57.000000 seagal-2.2/seagal.egg-info/dependency_links.txt
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        1 2023-02-11 05:26:14.000000 seagal-2.2/seagal.egg-info/not-zip-safe
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)       98 2023-04-14 14:13:57.000000 seagal-2.2/seagal.egg-info/requires.txt
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)        7 2023-04-14 14:13:57.000000 seagal-2.2/seagal.egg-info/top_level.txt
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)       38 2023-04-14 14:13:57.214665 seagal-2.2/setup.cfg
+-rw-rw-r--   0 linhua    (1008) linhua    (1010)      824 2023-04-10 21:45:04.000000 seagal-2.2/setup.py
```

### Comparing `seagal-2.1/LICENSE` & `seagal-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seagal-2.1/PKG-INFO` & `seagal-2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagal
-Version: 2.1
+Version: 2.2
 Summary: Spatial Enrichment Analysis of Gene Association using L-index
 Home-page: https://github.com/linhuawang/SEAGAL
 Author: Linhua Wang
 Author-email: linhuaw@bcm.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seagal-2.1/README.md` & `seagal-2.2/README.md`

 * *Files identical despite different names*

### Comparing `seagal-2.1/seagal/_gmod.py` & `seagal-2.2/seagal/_gmod.py`

 * *Files identical despite different names*

### Comparing `seagal-2.1/seagal/_plotting.py` & `seagal-2.2/seagal/_plotting.py`

 * *Files identical despite different names*

### Comparing `seagal-2.1/seagal/_utils.py` & `seagal-2.2/seagal/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     plt.close()
     self.histI = f
     self.adata = adata
     return f
 
 def spatial_association(self, grouped_only=True, use_pattern_genes=True,
                         genes=None, n_permutation=99, permute_ratio=0.2,
-                        FDR_cutoff = 0.05, L_cutoff = 0.1):
+                        FDR_cutoff = 0.05, L_cutoff = 0.1, indep=True):
     """ Calculate spatial associations
     
         Prameters:
         ----------
         grouped_only: bool, if True, only use it for gene sets previously defined and other parameters are irrelevant.
         use_pattern_genees: bool, if True, only calculate L for genes that have spatial patterns (based on Moran's I).
         genes: list of gene names, if not None, calculate L for this list of genes only.
@@ -101,15 +101,16 @@
         
         Return:
         ----------
         The spatial correlation data frame will be saved to self.co_expression.   
     """
     if grouped_only:
         grouped_data = self.grouped_adata.copy()
-        grouped_data = Global_L(grouped_data, permutations=n_permutation, percent=permute_ratio, max_RAM=32)
+        grouped_data = Global_L(grouped_data, permutations=n_permutation,
+                                indep=indep, percent=permute_ratio, max_RAM=32)
         df = grouped_data.uns['co_expression'].copy()
         df['pair'] = df.gene_1 + "&" + df.gene_2
         vals  = df['L.FDR'].copy()
         vals = vals[vals > 0]
         if len(vals) > 0:
             nonzeromin = min(vals)
             df['-log10(FDR)'] = -np.log10(df['L.FDR'] + nonzeromin)
```

### Comparing `seagal-2.1/seagal/lee_vec.py` & `seagal-2.2/seagal/lee_vec.py`

 * *Files identical despite different names*

### Comparing `seagal-2.1/seagal/modules/gmod.py` & `seagal-2.2/seagal/modules/gmod.py`

 * *Files identical despite different names*

### Comparing `seagal-2.1/seagal/seagal.py` & `seagal-2.2/seagal/seagal.py`

 * *Files identical despite different names*

### Comparing `seagal-2.1/seagal/spatial_measure.py` & `seagal-2.2/seagal/spatial_measure.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 #=========================================================================================
 # Graph/Embedding related measuring functions
 #=========================================================================================
 
 
-def Global_L(anndat_sp, features=None, permutations=0, percent=0.1, seed=1, max_RAM=16):
+def Global_L(anndat_sp, features=None, permutations=0, indep=True, percent=0.1, seed=1, max_RAM=16):
     random.seed(seed)
     np.random.seed(seed)
 
     print("Calculating global graph-based correlation value...")
     cong_mtx = anndat_sp.obsp['spatial_connectivities'].toarray()
 
     eSP = Spatial_Pearson(cong_mtx, permutations=permutations)
@@ -54,16 +54,21 @@
     
 
     eSP = eSP.fit(features_1_X, features_2_X, percent=percent, seed=seed, max_RAM=max_RAM)
     coexp_df['L'] = eSP.association_
     coexp_df['L.p_value'] = eSP.significance_ if permutations else 1.0
 
     if permutations:
-        _,coexp_df['L.FDR'] = fdrcorrection(coexp_df['L.p_value'],
+        if indep:
+            fdrs = fdrcorrection(coexp_df['L.p_value'],
                                             alpha=0.05, method='indep')
+        else:
+            fdrs =fdrcorrection(coexp_df['L.p_value'],
+                                            alpha=0.05, method='n')
+        _,coexp_df['L.FDR'] = fdrs
     else:
         coexp_df['L.FDR'] = 1.0
 
     #peaks_nearby['gene.pct'] = anndat_sp.var.loc[anndat_sp.var_names[gene_index],'Frac.all'].to_numpy()
     #peaks_nearby['peak.pct'] = anndat_sp.var.loc[anndat_sp.var_names[peak_index],'Frac.all'].to_numpy()
     anndat_sp.uns['co_expression'] = coexp_df
```

### Comparing `seagal-2.1/seagal.egg-info/PKG-INFO` & `seagal-2.2/seagal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagal
-Version: 2.1
+Version: 2.2
 Summary: Spatial Enrichment Analysis of Gene Association using L-index
 Home-page: https://github.com/linhuawang/SEAGAL
 Author: Linhua Wang
 Author-email: linhuaw@bcm.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seagal-2.1/setup.py` & `seagal-2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='seagal',
-    version='2.1',
+    version='2.2',
     description='Spatial Enrichment Analysis of Gene Association using L-index',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/linhuawang/SEAGAL',
     author='Linhua Wang',
     author_email='linhuaw@bcm.edu',
     license='MIT',
```

