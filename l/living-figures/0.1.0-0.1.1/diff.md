# Comparing `tmp/living-figures-0.1.0.tar.gz` & `tmp/living-figures-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "living-figures-0.1.0.tar", last modified: Thu Apr 13 21:35:53 2023, max compression
+gzip compressed data, was "living-figures-0.1.1.tar", last modified: Fri Apr 14 18:17:29 2023, max compression
```

## Comparing `living-figures-0.1.0.tar` & `living-figures-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.633656 living-figures-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-13 21:35:08.000000 living-figures-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 21:35:08.000000 living-figures-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-13 21:35:53.633656 living-figures-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-13 21:35:08.000000 living-figures-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-13 21:35:08.000000 living-figures-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 21:35:08.000000 living-figures-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:35:53.633656 living-figures-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-13 21:35:08.000000 living-figures-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.625656 living-figures-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.629656 living-figures-0.1.0/src/living_figures/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.629656 living-figures-0.1.0/src/living_figures/bio/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.629656 living-figures-0.1.0/src/living_figures/bio/epigenome/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.629656 living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/pacbio_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/parse_rebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/rebase_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.633656 living-figures-0.1.0/src/living_figures/bio/epigenome/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/widgets/panepibrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.633656 living-figures-0.1.0/src/living_figures/bio/fom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/fom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.633656 living-figures-0.1.0/src/living_figures/bio/volcano/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/volcano/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/volcano/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/volcano/make_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.633656 living-figures-0.1.0/src/living_figures/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/helpers/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/helpers/sorting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.629656 living-figures-0.1.0/src/living_figures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-13 21:35:53.000000 living-figures-0.1.0/src/living_figures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-13 21:35:53.000000 living-figures-0.1.0/src/living_figures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:35:53.000000 living-figures-0.1.0/src/living_figures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 21:35:53.000000 living-figures-0.1.0/src/living_figures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 21:35:53.000000 living-figures-0.1.0/src/living_figures.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.633656 living-figures-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-13 21:35:08.000000 living-figures-0.1.0/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:29.623239 living-figures-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-14 18:16:43.000000 living-figures-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 18:16:43.000000 living-figures-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-14 18:17:29.623239 living-figures-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-14 18:16:43.000000 living-figures-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-14 18:16:43.000000 living-figures-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 18:16:43.000000 living-figures-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:17:29.623239 living-figures-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-14 18:16:43.000000 living-figures-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:29.619239 living-figures-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:29.619239 living-figures-0.1.1/src/living_figures/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:29.623239 living-figures-0.1.1/src/living_figures/bio/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/bio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:29.623239 living-figures-0.1.1/src/living_figures/bio/epigenome/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/bio/epigenome/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:29.623239 living-figures-0.1.1/src/living_figures/bio/epigenome/test_data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2606 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/bio/epigenome/test_data/download_from_ncbi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:29.623239 living-figures-0.1.1/src/living_figures/bio/epigenome/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/bio/epigenome/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/bio/epigenome/utilities/pacbio_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/bio/epigenome/utilities/parse_rebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/bio/epigenome/utilities/rebase_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:29.623239 living-figures-0.1.1/src/living_figures/bio/epigenome/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/bio/epigenome/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27529 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/bio/epigenome/widgets/panepibrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:29.623239 living-figures-0.1.1/src/living_figures/bio/fom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/bio/fom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:29.623239 living-figures-0.1.1/src/living_figures/bio/volcano/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/bio/volcano/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/bio/volcano/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/bio/volcano/make_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:29.623239 living-figures-0.1.1/src/living_figures/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/helpers/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-14 18:16:43.000000 living-figures-0.1.1/src/living_figures/helpers/sorting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:29.623239 living-figures-0.1.1/src/living_figures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-14 18:17:29.000000 living-figures-0.1.1/src/living_figures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-14 18:17:29.000000 living-figures-0.1.1/src/living_figures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:17:29.000000 living-figures-0.1.1/src/living_figures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 18:17:29.000000 living-figures-0.1.1/src/living_figures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 18:17:29.000000 living-figures-0.1.1/src/living_figures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:29.623239 living-figures-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-14 18:16:43.000000 living-figures-0.1.1/tests/test_import.py
```

### Comparing `living-figures-0.1.0/LICENSE` & `living-figures-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.0/PKG-INFO` & `living-figures-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: living-figures
-Version: 0.1.0
+Version: 0.1.1
 Summary: Resource of interactive data widgets
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets-store
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets-store/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `living-figures-0.1.0/README.md` & `living-figures-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.0/pyproject.toml` & `living-figures-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/pacbio_file.py` & `living-figures-0.1.1/src/living_figures/bio/epigenome/utilities/pacbio_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,29 @@
 
 
 class StPBMotif(StFile):
     """Process epigenetic data from PacBio motifs.csv format."""
 
     value = pd.DataFrame()
 
+    cname_map = {
+        "Motif": "motifString",
+        "Modified Position": "centerPos",
+        "Motification Type": "modificationType",
+        "% of Motifs Detected": "fraction",
+        "# of Motifs Detected": "nDetected",
+        "# of Motifs in Genome": "nGenome",
+        "Mean QV": "meanScore",
+        "Mean Coverage": "meanCoverage",
+        "Partner Motif": "partnerMotifString",
+        "Mean IPD ratio": "meanIpdRatio",
+        "Group Tag": "groupTag",
+        "Objective Score": "objectiveScore"
+    }
+
     def __init__(
         self,
         id="pacbio_motif",
         value=None,
         label="PacBio Motifs",
         help: Union[str, None] = None,
         disabled: bool = False,
@@ -83,14 +98,19 @@
                     self.parse_csv(file)
 
     def parse_csv(self, file):
 
         # Read the CSV file
         motifs = pd.read_csv(file)
 
+        # Apply the column mappings
+        motifs = motifs.rename(
+            columns=self.cname_map
+        )
+
         # Make sure that the expected columns are present
         expected_cnames = [
             "motifString",
             "centerPos",
             "modificationType",
             "fraction",
             "nDetected",
@@ -108,17 +128,19 @@
             for cname in expected_cnames
             if cname not in motifs.columns.values
         ]
 
         # If any of those columns are missing
         if len(missing_cnames) > 0:
             # Warn the user
-            self.main_container.warning(
-                f"Did not find expected columns - {', '.join(missing_cnames)}"
-            )
+            msg = f"Did not find expected columns - {', '.join(missing_cnames)} in {file.name}" # noqa
+            if self.main_container is not None:
+                self.main_container.warning(msg)
+            else:
+                raise Exception(msg)
             # Take no further action
             return
 
         # Add a unique ID for the motif + position + modification
         # Also add the motif length
         motifs = motifs.assign(
             text=motifs.apply(
```

### Comparing `living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/parse_rebase.py` & `living-figures-0.1.1/src/living_figures/bio/epigenome/utilities/parse_rebase.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/rebase_file.py` & `living-figures-0.1.1/src/living_figures/bio/epigenome/utilities/rebase_file.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.0/src/living_figures/bio/epigenome/widgets/panepibrowser.py` & `living-figures-0.1.1/src/living_figures/bio/epigenome/widgets/panepibrowser.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,15 +569,15 @@
             go.Heatmap(
                 x=value_df.columns.values,
                 y=value_df.index.values,
                 z=value_df.values,
                 colorscale=formatting["heatmap_cpal"],
                 text=text_df.values,
                 hoverinfo="text",
-                colorbar_title="Percent<br>Detection<br>of Motif"
+                colorbar_title="Fractional<br>Detection<br>of Motif"
             ),
             row=2,
             col=2
         )
 
         # Add the marginal annotation on the rows
         fig.append_trace(
```

### Comparing `living-figures-0.1.0/src/living_figures/bio/volcano/app.py` & `living-figures-0.1.1/src/living_figures/bio/volcano/app.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.0/src/living_figures/bio/volcano/make_test_data.py` & `living-figures-0.1.1/src/living_figures/bio/volcano/make_test_data.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.0/src/living_figures/helpers/sorting.py` & `living-figures-0.1.1/src/living_figures/helpers/sorting.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.1.0/src/living_figures.egg-info/PKG-INFO` & `living-figures-0.1.1/src/living_figures.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: living-figures
-Version: 0.1.0
+Version: 0.1.1
 Summary: Resource of interactive data widgets
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets-store
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets-store/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `living-figures-0.1.0/src/living_figures.egg-info/SOURCES.txt` & `living-figures-0.1.1/src/living_figures.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/living_figures.egg-info/PKG-INFO
 src/living_figures.egg-info/SOURCES.txt
 src/living_figures.egg-info/dependency_links.txt
 src/living_figures.egg-info/requires.txt
 src/living_figures.egg-info/top_level.txt
 src/living_figures/bio/__init__.py
 src/living_figures/bio/epigenome/__init__.py
+src/living_figures/bio/epigenome/test_data/download_from_ncbi.py
 src/living_figures/bio/epigenome/utilities/__init__.py
 src/living_figures/bio/epigenome/utilities/pacbio_file.py
 src/living_figures/bio/epigenome/utilities/parse_rebase.py
 src/living_figures/bio/epigenome/utilities/rebase_file.py
 src/living_figures/bio/epigenome/widgets/__init__.py
 src/living_figures/bio/epigenome/widgets/panepibrowser.py
 src/living_figures/bio/fom/__init__.py
```

### Comparing `living-figures-0.1.0/tests/test_import.py` & `living-figures-0.1.1/tests/test_import.py`

 * *Files identical despite different names*

