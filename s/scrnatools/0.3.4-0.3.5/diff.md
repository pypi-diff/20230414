# Comparing `tmp/scrnatools-0.3.4.tar.gz` & `tmp/scrnatools-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrnatools-0.3.4.tar", last modified: Thu Mar 30 17:07:56 2023, max compression
+gzip compressed data, was "scrnatools-0.3.5.tar", last modified: Fri Apr 14 18:13:26 2023, max compression
```

## Comparing `scrnatools-0.3.4.tar` & `scrnatools-0.3.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-03-30 17:07:56.253529 scrnatools-0.3.4/
--rw-r--r--   0 joe       (1001) joe       (1001)     1479 2022-11-12 02:35:58.000000 scrnatools-0.3.4/LICENSE.txt
--rw-rw-r--   0 joe       (1001) joe       (1001)      244 2023-03-30 17:07:56.253529 scrnatools-0.3.4/PKG-INFO
--rw-rw-r--   0 joe       (1001) joe       (1001)     1942 2023-03-08 17:54:42.000000 scrnatools-0.3.4/README.md
-drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-03-30 17:07:56.249529 scrnatools-0.3.4/scrnatools/
--rw-r--r--   0 joe       (1001) joe       (1001)      217 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/__init__.py
--rw-r--r--   0 joe       (1001) joe       (1001)     7105 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/_configs.py
-drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-03-30 17:07:56.253529 scrnatools-0.3.4/scrnatools/_utils/
--rw-r--r--   0 joe       (1001) joe       (1001)      306 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/_utils/__init__.py
--rw-r--r--   0 joe       (1001) joe       (1001)      574 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/_utils/_check_path.py
--rw-r--r--   0 joe       (1001) joe       (1001)     2018 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/_utils/_debug.py
--rw-r--r--   0 joe       (1001) joe       (1001)     1547 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/_utils/_fill_array.py
--rw-r--r--   0 joe       (1001) joe       (1001)      746 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/_utils/_type_check.py
-drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-03-30 17:07:56.253529 scrnatools-0.3.4/scrnatools/plotting/
--rw-rw-r--   0 joe       (1001) joe       (1001)      398 2023-03-30 16:56:02.000000 scrnatools-0.3.4/scrnatools/plotting/__init__.py
--rw-r--r--   0 joe       (1001) joe       (1001)     5413 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/plotting/_gene_density_plot.py
--rw-r--r--   0 joe       (1001) joe       (1001)     3885 2023-02-17 17:21:26.000000 scrnatools-0.3.4/scrnatools/plotting/_gene_embedding.py
--rw-rw-r--   0 joe       (1001) joe       (1001)     5770 2023-03-30 16:56:02.000000 scrnatools-0.3.4/scrnatools/plotting/_gene_heatmap.py
--rw-rw-r--   0 joe       (1001) joe       (1001)     6956 2023-03-30 16:56:02.000000 scrnatools-0.3.4/scrnatools/plotting/_gene_violinplot.py
--rw-r--r--   0 joe       (1001) joe       (1001)     2488 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/plotting/_isoform_qc_plot.py
--rw-r--r--   0 joe       (1001) joe       (1001)     5151 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/plotting/_qc_plotting.py
-drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-03-30 17:07:56.253529 scrnatools-0.3.4/scrnatools/qc/
--rw-r--r--   0 joe       (1001) joe       (1001)      202 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/qc/__init__.py
--rw-r--r--   0 joe       (1001) joe       (1001)     2145 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/qc/_filter_cells.py
--rw-r--r--   0 joe       (1001) joe       (1001)     2790 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/qc/_scrublet.py
-drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-03-30 17:07:56.253529 scrnatools-0.3.4/scrnatools/tools/
--rw-r--r--   0 joe       (1001) joe       (1001)      810 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/tools/__init__.py
--rw-r--r--   0 joe       (1001) joe       (1001)     4166 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/tools/_cell_type_similarity.py
--rw-r--r--   0 joe       (1001) joe       (1001)     3086 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/tools/_cluster_de.py
--rw-r--r--   0 joe       (1001) joe       (1001)     3198 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/tools/_create_cell_type_signature.py
--rw-r--r--   0 joe       (1001) joe       (1001)     3976 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/tools/_create_isoform_lookup_tables.py
--rw-r--r--   0 joe       (1001) joe       (1001)     2442 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/tools/_get_expression_matrix.py
--rw-r--r--   0 joe       (1001) joe       (1001)     2742 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/tools/_get_immgen_similarity_signatures.py
--rw-r--r--   0 joe       (1001) joe       (1001)     1433 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/tools/_isoform_preprocessing.py
--rw-r--r--   0 joe       (1001) joe       (1001)     1335 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/tools/_load_isoform_lookup_tables.py
--rw-r--r--   0 joe       (1001) joe       (1001)     2844 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/tools/_log_density_ratio.py
--rw-r--r--   0 joe       (1001) joe       (1001)     1336 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/tools/_read_kallisto_tcc_matrix.py
--rw-r--r--   0 joe       (1001) joe       (1001)     1466 2022-11-12 02:35:58.000000 scrnatools-0.3.4/scrnatools/tools/_save_isoform_lookup_tables.py
-drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-03-30 17:07:56.249529 scrnatools-0.3.4/scrnatools.egg-info/
--rw-rw-r--   0 joe       (1001) joe       (1001)      244 2023-03-30 17:07:56.000000 scrnatools-0.3.4/scrnatools.egg-info/PKG-INFO
--rw-rw-r--   0 joe       (1001) joe       (1001)     1284 2023-03-30 17:07:56.000000 scrnatools-0.3.4/scrnatools.egg-info/SOURCES.txt
--rw-rw-r--   0 joe       (1001) joe       (1001)        1 2023-03-30 17:07:56.000000 scrnatools-0.3.4/scrnatools.egg-info/dependency_links.txt
--rw-rw-r--   0 joe       (1001) joe       (1001)      108 2023-03-30 17:07:56.000000 scrnatools-0.3.4/scrnatools.egg-info/requires.txt
--rw-rw-r--   0 joe       (1001) joe       (1001)       11 2023-03-30 17:07:56.000000 scrnatools-0.3.4/scrnatools.egg-info/top_level.txt
--rw-r--r--   0 joe       (1001) joe       (1001)      107 2023-03-30 17:07:56.253529 scrnatools-0.3.4/setup.cfg
--rw-r--r--   0 joe       (1001) joe       (1001)      648 2023-03-30 17:00:52.000000 scrnatools-0.3.4/setup.py
+drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-04-14 18:13:26.281265 scrnatools-0.3.5/
+-rw-r--r--   0 joe       (1001) joe       (1001)     1479 2022-11-12 02:35:58.000000 scrnatools-0.3.5/LICENSE.txt
+-rw-rw-r--   0 joe       (1001) joe       (1001)      244 2023-04-14 18:13:26.281265 scrnatools-0.3.5/PKG-INFO
+-rw-rw-r--   0 joe       (1001) joe       (1001)     2355 2023-04-14 18:12:31.000000 scrnatools-0.3.5/README.md
+drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-04-14 18:13:26.277265 scrnatools-0.3.5/scrnatools/
+-rw-r--r--   0 joe       (1001) joe       (1001)      217 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/__init__.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     7105 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/_configs.py
+drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-04-14 18:13:26.277265 scrnatools-0.3.5/scrnatools/_utils/
+-rw-r--r--   0 joe       (1001) joe       (1001)      306 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/_utils/__init__.py
+-rw-r--r--   0 joe       (1001) joe       (1001)      574 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/_utils/_check_path.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     2018 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/_utils/_debug.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     1547 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/_utils/_fill_array.py
+-rw-r--r--   0 joe       (1001) joe       (1001)      746 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/_utils/_type_check.py
+drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-04-14 18:13:26.277265 scrnatools-0.3.5/scrnatools/plotting/
+-rw-rw-r--   0 joe       (1001) joe       (1001)      398 2023-03-30 16:56:02.000000 scrnatools-0.3.5/scrnatools/plotting/__init__.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     5413 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/plotting/_gene_density_plot.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     3885 2023-02-17 17:21:26.000000 scrnatools-0.3.5/scrnatools/plotting/_gene_embedding.py
+-rw-rw-r--   0 joe       (1001) joe       (1001)     5778 2023-04-14 18:12:31.000000 scrnatools-0.3.5/scrnatools/plotting/_gene_heatmap.py
+-rw-rw-r--   0 joe       (1001) joe       (1001)     6945 2023-04-14 18:12:31.000000 scrnatools-0.3.5/scrnatools/plotting/_gene_violinplot.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     2488 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/plotting/_isoform_qc_plot.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     5151 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/plotting/_qc_plotting.py
+drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-04-14 18:13:26.281265 scrnatools-0.3.5/scrnatools/qc/
+-rw-r--r--   0 joe       (1001) joe       (1001)      202 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/qc/__init__.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     2145 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/qc/_filter_cells.py
+-rw-rw-r--   0 joe       (1001) joe       (1001)     2747 2023-04-14 18:12:31.000000 scrnatools-0.3.5/scrnatools/qc/_scrublet.py
+drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-04-14 18:13:26.281265 scrnatools-0.3.5/scrnatools/tools/
+-rw-r--r--   0 joe       (1001) joe       (1001)      810 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/tools/__init__.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     4166 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/tools/_cell_type_similarity.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     3086 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/tools/_cluster_de.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     3198 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/tools/_create_cell_type_signature.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     3976 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/tools/_create_isoform_lookup_tables.py
+-rw-rw-r--   0 joe       (1001) joe       (1001)     2494 2023-04-14 18:12:31.000000 scrnatools-0.3.5/scrnatools/tools/_get_expression_matrix.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     2742 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/tools/_get_immgen_similarity_signatures.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     1433 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/tools/_isoform_preprocessing.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     1335 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/tools/_load_isoform_lookup_tables.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     2844 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/tools/_log_density_ratio.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     1336 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/tools/_read_kallisto_tcc_matrix.py
+-rw-r--r--   0 joe       (1001) joe       (1001)     1466 2022-11-12 02:35:58.000000 scrnatools-0.3.5/scrnatools/tools/_save_isoform_lookup_tables.py
+drwxrwxr-x   0 joe       (1001) joe       (1001)        0 2023-04-14 18:13:26.277265 scrnatools-0.3.5/scrnatools.egg-info/
+-rw-rw-r--   0 joe       (1001) joe       (1001)      244 2023-04-14 18:13:26.000000 scrnatools-0.3.5/scrnatools.egg-info/PKG-INFO
+-rw-rw-r--   0 joe       (1001) joe       (1001)     1284 2023-04-14 18:13:26.000000 scrnatools-0.3.5/scrnatools.egg-info/SOURCES.txt
+-rw-rw-r--   0 joe       (1001) joe       (1001)        1 2023-04-14 18:13:26.000000 scrnatools-0.3.5/scrnatools.egg-info/dependency_links.txt
+-rw-rw-r--   0 joe       (1001) joe       (1001)      108 2023-04-14 18:13:26.000000 scrnatools-0.3.5/scrnatools.egg-info/requires.txt
+-rw-rw-r--   0 joe       (1001) joe       (1001)       11 2023-04-14 18:13:26.000000 scrnatools-0.3.5/scrnatools.egg-info/top_level.txt
+-rw-r--r--   0 joe       (1001) joe       (1001)      107 2023-04-14 18:13:26.281265 scrnatools-0.3.5/setup.cfg
+-rw-r--r--   0 joe       (1001) joe       (1001)      648 2023-04-14 18:12:56.000000 scrnatools-0.3.5/setup.py
```

### Comparing `scrnatools-0.3.4/LICENSE.txt` & `scrnatools-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/README.md` & `scrnatools-0.3.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 # Contents:
 
 ## Plotting methods (rna.pl)
 **gene_embedding** - Plots gene expression on a UMAP/TSNE with quantile thresholds for the colorbar mapping<br/>
 **gene_density plot** - Plots the desity of a gene's expression on a UMAP/TSNE<br/>
 **qc_plotting** - general QC plots showing read/cell, num genes/cell, percent mito reads, etc.<br/>
+**gene_heatmap** - Plots gene expression of a given list of gene values based on an annotated categorical variable (cell type, genotype, etc.) on a heatmap<br/>
+**gene_violinplot** - Plots a number of violin plots where each violinplot displays a gene's expression from a given list of gene values based on an annotated categorical variable which can be colored by a different annotated categorical variable<br/>
 
 ## QC methods (rna.qc)
 **scrublet** - Uses scrublet to filter doublets from data based on a doublet score threshold<br/>
 **filter_cells** - filter cells from data based on total counts, num genes, and percent mito reads thresholds<br/>
 
 ## Tools (rna.tl)
 **cell_type_similarity** - Calculates cosine similarity per cell to samples in a reference dataset <br/>
```

### Comparing `scrnatools-0.3.4/scrnatools/_configs.py` & `scrnatools-0.3.5/scrnatools/_configs.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/_utils/_check_path.py` & `scrnatools-0.3.5/scrnatools/_utils/_check_path.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/_utils/_debug.py` & `scrnatools-0.3.5/scrnatools/_utils/_debug.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/_utils/_fill_array.py` & `scrnatools-0.3.5/scrnatools/_utils/_fill_array.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/_utils/_type_check.py` & `scrnatools-0.3.5/scrnatools/_utils/_type_check.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/plotting/_gene_density_plot.py` & `scrnatools-0.3.5/scrnatools/plotting/_gene_density_plot.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/plotting/_gene_embedding.py` & `scrnatools-0.3.5/scrnatools/plotting/_gene_embedding.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/plotting/_gene_heatmap.py` & `scrnatools-0.3.5/scrnatools/plotting/_gene_heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     layer
         The type of the expression data to use for the heatmap, can be a layer in 'adata.layers' or 'X'
         to use the data stored in adata.X. Default 'X'.
     obs_values
         Values from obs key group to display on heatmap. Default displays all values in obs key.
     cbar_args
         List of integers to position color bar on heatmap. [x position, y position, width, height].
-        Default adjusts to be on right middle of headmap.
+        Default automatically adjusts to right middle of heatmap.
     reverse_axis
         A boolean to reverse x and y axes. Default False.
     cell_size
         Integer specifying the size of each cell in the heatmap. Default 50.
     save_path
         The path to save the figure. Default None.
     dpi
```

### Comparing `scrnatools-0.3.4/scrnatools/plotting/_gene_violinplot.py` & `scrnatools-0.3.5/scrnatools/plotting/_gene_violinplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,17 @@
         The categorical grouping to display on the x axis of the violinplot.
     layer
         The type of the expression data to use for the violinplot, can be a layer in 'adata.layers' or 'X'
         to use the data stored in adata.X. Default 'X'.
     x_values
         Values from x key group to display on violinplot. Default displays all values in x key.
     hue_key
-        The categorical grouping to color the grouped violin plots by. Default None.
+        The categorical grouping to color the grouped violin plots by. Values will appear in legend. Default None.
     hue_values
-        Values from hue_key to display on violinplot. Values will show up in legend. Default displays all values in hue key.
+        Values from hue_key to display on violinplot. Default displays all values in hue key.
     ncols
         Number of columns to display the violinplots.
     nrows
         Number of rows to display the violinplots.
     save_path
         The path to save the figure. Default None.
     dpi
@@ -136,19 +136,19 @@
     
     expression_matrix[x_key] = subsetAdata.obs[x_key]
     if hue_key != None:
         expression_matrix[hue_key] = subsetAdata.obs[hue_key]
     
     #check inputted x values and hue values are in subsetted data
     for i in x_values:
-        if i not in expression_matrix[x_key].unique().categories:
+        if i not in list(expression_matrix[x_key].unique()):
             raise ValueError(f"{i} is not in adata's x_key {x_key}.\nPossible {x_key}s: {list(adata.obs[x_key].unique())}")
     if hue_key != None:
         for i in hue_values:
-            if i not in expression_matrix[hue_key].unique().categories:
+            if i not in list(expression_matrix[hue_key].unique()):
                 raise ValueError(f"{i} is not in adata's hue_key {hue_key}.\nPossible {hue_key}s: {list(adata.obs[hue_key].unique())}")
 
     #generate violin plots
     for plt_num, gene in enumerate(gene_list):
         plt.subplot(nrows, ncols, plt_num + 1)
         ax = sns.violinplot(
             expression_matrix,
```

### Comparing `scrnatools-0.3.4/scrnatools/plotting/_isoform_qc_plot.py` & `scrnatools-0.3.5/scrnatools/plotting/_isoform_qc_plot.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/plotting/_qc_plotting.py` & `scrnatools-0.3.5/scrnatools/plotting/_qc_plotting.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/qc/_filter_cells.py` & `scrnatools-0.3.5/scrnatools/qc/_filter_cells.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/qc/_scrublet.py` & `scrnatools-0.3.5/scrnatools/qc/_scrublet.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,8 +69,8 @@
         scrublet_predictions = pd.concat([scrublet_predictions, scrublet_prediction])
     # Add scrublet scores to adata.obs and filter out cells with a score > doublet_threshold
     adata.obs["scrublet_score"] = scrublet_predictions.scrublet_score
     adata.obs["scrublet_called_doublet"] = adata.obs.scrublet_score > doublet_threshold
     num_doublets = adata.obs.scrublet_called_doublet.sum()
     pct_doublets = round(num_doublets / len(adata) * 100, 3)
     logger.info(f"{pct_doublets}% of cells classified as doublets ({num_doublets} cells)")
-    return adata[~adata.obs.scrublet_called_doublet].copy()
+    return adata
```

### Comparing `scrnatools-0.3.4/scrnatools/tools/__init__.py` & `scrnatools-0.3.5/scrnatools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/tools/_cell_type_similarity.py` & `scrnatools-0.3.5/scrnatools/tools/_cell_type_similarity.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/tools/_cluster_de.py` & `scrnatools-0.3.5/scrnatools/tools/_cluster_de.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/tools/_create_cell_type_signature.py` & `scrnatools-0.3.5/scrnatools/tools/_create_cell_type_signature.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/tools/_create_isoform_lookup_tables.py` & `scrnatools-0.3.5/scrnatools/tools/_create_isoform_lookup_tables.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/tools/_get_expression_matrix.py` & `scrnatools-0.3.5/scrnatools/tools/_get_expression_matrix.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,11 +60,11 @@
             matrix = DataFrame(raw_data.X.todense(), index=anndata.obs.index, columns=anndata.raw.var_names)
         else:
             matrix = DataFrame(raw_data.X, index=anndata.obs.index, columns=anndata.raw.var_names)
     elif gene_data in anndata.layers:
         if issparse(anndata.layers[gene_data]):
             matrix = DataFrame(anndata.layers[gene_data].todense(), index=anndata.obs.index, columns=anndata.var_names)
         else:
-            matrix = DataFrame(anndata.layers[gene_data])
+            matrix = DataFrame(anndata.layers[gene_data], index=anndata.obs.index, columns=anndata.var_names)
     else:
         raise ValueError(f"{gene_data} is not 'X', 'raw', or a valid layer name in '{anndata.layers}'")
     return matrix
```

### Comparing `scrnatools-0.3.4/scrnatools/tools/_get_immgen_similarity_signatures.py` & `scrnatools-0.3.5/scrnatools/tools/_get_immgen_similarity_signatures.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/tools/_isoform_preprocessing.py` & `scrnatools-0.3.5/scrnatools/tools/_isoform_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/tools/_load_isoform_lookup_tables.py` & `scrnatools-0.3.5/scrnatools/tools/_load_isoform_lookup_tables.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/tools/_log_density_ratio.py` & `scrnatools-0.3.5/scrnatools/tools/_log_density_ratio.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/tools/_read_kallisto_tcc_matrix.py` & `scrnatools-0.3.5/scrnatools/tools/_read_kallisto_tcc_matrix.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools/tools/_save_isoform_lookup_tables.py` & `scrnatools-0.3.5/scrnatools/tools/_save_isoform_lookup_tables.py`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/scrnatools.egg-info/SOURCES.txt` & `scrnatools-0.3.5/scrnatools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrnatools-0.3.4/setup.py` & `scrnatools-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scrnatools",
-    version="0.3.4",
+    version="0.3.5",
     author="Joe Germino",
     author_email="joe.germino@ucsf.edu",
     description="Tools for single cell RNA sequencing pipelines",
     url="https://github.com/j-germino/sc-rna-tools",
     packages=setuptools.find_packages(),
     install_requires=[
         "scanpy",
```

