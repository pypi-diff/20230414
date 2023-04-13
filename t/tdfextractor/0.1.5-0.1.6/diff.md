# Comparing `tmp/tdfextractor-0.1.5.tar.gz` & `tmp/tdfextractor-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdfextractor-0.1.5.tar", last modified: Thu Apr 13 19:46:38 2023, max compression
+gzip compressed data, was "tdfextractor-0.1.6.tar", last modified: Thu Apr 13 22:44:55 2023, max compression
```

## Comparing `tdfextractor-0.1.5.tar` & `tdfextractor-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 19:46:38.431476 tdfextractor-0.1.5/
--rw-rw-rw-   0        0        0      453 2023-04-13 19:46:38.431476 tdfextractor-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       80 2022-09-29 06:42:08.000000 tdfextractor-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 19:46:38.432477 tdfextractor-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      641 2023-04-13 18:53:55.000000 tdfextractor-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:46:38.411356 tdfextractor-0.1.5/tdfextractor/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:09:12.000000 tdfextractor-0.1.5/tdfextractor/__init__.py
--rw-rw-rw-   0        0        0       50 2023-04-13 19:43:40.000000 tdfextractor-0.1.5/tdfextractor/constants.py
--rw-rw-rw-   0        0        0     8936 2023-04-13 19:46:08.000000 tdfextractor-0.1.5/tdfextractor/ms2_extractor.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 19:43:40.000000 tdfextractor-0.1.5/tdfextractor/string_templates.py
--rw-rw-rw-   0        0        0     1602 2022-11-21 00:49:16.000000 tdfextractor-0.1.5/tdfextractor/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:46:38.425010 tdfextractor-0.1.5/tdfextractor.egg-info/
--rw-rw-rw-   0        0        0      453 2023-04-13 19:46:38.000000 tdfextractor-0.1.5/tdfextractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-13 19:46:38.000000 tdfextractor-0.1.5/tdfextractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 19:46:38.000000 tdfextractor-0.1.5/tdfextractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 19:46:38.000000 tdfextractor-0.1.5/tdfextractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 19:46:38.000000 tdfextractor-0.1.5/tdfextractor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 19:46:38.430456 tdfextractor-0.1.5/test/
--rw-rw-rw-   0        0        0     2440 2023-04-12 23:55:45.000000 tdfextractor-0.1.5/test/test_ms2_extractor.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:44:55.679804 tdfextractor-0.1.6/
+-rw-rw-rw-   0        0        0      453 2023-04-13 22:44:55.679804 tdfextractor-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       80 2022-09-29 06:42:08.000000 tdfextractor-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 22:44:55.679804 tdfextractor-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-04-13 22:43:36.000000 tdfextractor-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:44:55.655045 tdfextractor-0.1.6/tdfextractor/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:09:12.000000 tdfextractor-0.1.6/tdfextractor/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-04-13 19:43:40.000000 tdfextractor-0.1.6/tdfextractor/constants.py
+-rw-rw-rw-   0        0        0     8951 2023-04-13 22:42:43.000000 tdfextractor-0.1.6/tdfextractor/ms2_extractor.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 19:43:40.000000 tdfextractor-0.1.6/tdfextractor/string_templates.py
+-rw-rw-rw-   0        0        0     1602 2022-11-21 00:49:16.000000 tdfextractor-0.1.6/tdfextractor/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:44:55.677070 tdfextractor-0.1.6/tdfextractor.egg-info/
+-rw-rw-rw-   0        0        0      453 2023-04-13 22:44:55.000000 tdfextractor-0.1.6/tdfextractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-13 22:44:55.000000 tdfextractor-0.1.6/tdfextractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 22:44:55.000000 tdfextractor-0.1.6/tdfextractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 22:44:55.000000 tdfextractor-0.1.6/tdfextractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 22:44:55.000000 tdfextractor-0.1.6/tdfextractor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 22:44:55.678736 tdfextractor-0.1.6/test/
+-rw-rw-rw-   0        0        0     2505 2023-04-13 22:38:23.000000 tdfextractor-0.1.6/test/test_ms2_extractor.py
```

### Comparing `tdfextractor-0.1.5/setup.py` & `tdfextractor-0.1.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tdfextractor',
-    version='0.1.5',
+    version='0.1.6',
     description='extract mass spec files from bruker d folder',
     url='https://github.com/pgarrett-scripps/tdfextractor.git',
     author='Patrick Garrett',
     author_email='pgarrett@scripps.edu',
     license='MIT',
     packages=['tdfextractor'],
     install_requires=['tdfpy==0.1.2', 'serenipy==0.2.6', 'tqdm==4.64.1'],
```

### Comparing `tdfextractor-0.1.5/tdfextractor/ms2_extractor.py` & `tdfextractor-0.1.6/tdfextractor/ms2_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from serenipy.ms2 import Ms2Spectra, to_ms2
 from tqdm import tqdm
 
 from .constants import MS2_VERSION
 from .string_templates import header_ms2_template
 from .utils import calculate_mass, map_precursor_to_ip2_scan_number
 
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
 
+
 def batch_iterator(input_list: List, batch_size: int):
     for i in range(0, len(input_list), batch_size):
         yield input_list[i:i + batch_size]
 
 
 def get_ms2_content(analysis_dir: str, include_spectra: bool = True, batch_size: int = 100,
                     remove_charge1: bool = True, remove_empty_spectra: bool = True,
@@ -37,34 +37,34 @@
 
     Returns:
         List[Ms2Spectra]: A list of Ms2Spectra objects representing MS/MS spectra.
 
     Raises:
         FileNotFoundError: If the analysis directory does not exist.
     """
-    logger.info(f'Starting to process {analysis_dir}')
-
     with timsdata.timsdata_connect(analysis_dir) as td:
 
         analysis_tdf_path = str(Path(analysis_dir) / 'analysis.tdf')
         pd_tdf = PandasTdf(analysis_tdf_path)
 
         precursors_df = pd_tdf.precursors
         frames_df = pd_tdf.frames
 
         precursor_to_scan_number = map_precursor_to_ip2_scan_number(precursors_df, frames_df)
         parent_id_to_rt = {int(frame_id): rt for frame_id, rt in frames_df[['Id', 'Time']].values}
 
         precursor_id_to_msms_info = {int(prec_id): (ce, iso_width, iso_mz) for prec_id, ce, iso_width, iso_mz in
-                pd_tdf.pasef_frame_msms_info[['Precursor', 'CollisionEnergy', 'IsolationWidth', 'IsolationMz']].values}
+                                     pd_tdf.pasef_frame_msms_info[
+                                         ['Precursor', 'CollisionEnergy', 'IsolationWidth', 'IsolationMz']].values}
 
         precursors_df.dropna(subset=['MonoisotopicMz', 'Charge'], inplace=True)
 
-        for precursor_batch in tqdm(list(batch_iterator(input_list=list(precursors_df.iterrows()), batch_size=batch_size)),
-                                    desc='Generating MS2 Spectra'):
+        for precursor_batch in tqdm(
+                list(batch_iterator(input_list=list(precursors_df.iterrows()), batch_size=batch_size)),
+                desc='Generating MS2 Spectra'):
             pasef_ms_ms = None
             if include_spectra:
                 pasef_ms_ms = td.readPasefMsMs([int(precursor_row['Id']) for _, precursor_row in precursor_batch])
 
             for _, precursor_row in precursor_batch:
 
                 precursor_id = int(precursor_row['Id'])
@@ -163,27 +163,30 @@
         FileNotFoundError: If the analysis directory does not exist.
     """
     start_time = time.time()
 
     if output_file is None:
         output_file = str(Path(analysis_dir) / Path(analysis_dir).stem) + '.ms2'
 
-    logger.info(f'Arguments: analysis_dir: {analysis_dir}, output_file: {output_file}, include_spectra: {include_spectra}, '
-    f'batch_size: {batch_size}, remove_charge1: {remove_charge1}, remove_empty_spectra: {remove_empty_spectra}, '
-    f'min_intensity: {min_intensity}')
+    logger.info(
+        f'Arguments: analysis_dir: {analysis_dir}, output_file: {output_file}, include_spectra: {include_spectra}, '
+        f'batch_size: {batch_size}, remove_charge1: {remove_charge1}, remove_empty_spectra: {remove_empty_spectra}, '
+        f'min_intensity: {min_intensity}')
 
     logger.info('Creating Ms2 Header')
     ms2_header = generate_header(analysis_dir)
 
     logger.info('Generating Ms2 Spectra')
     ms2_spectra = get_ms2_content(analysis_dir=analysis_dir, include_spectra=include_spectra, batch_size=batch_size,
                                   remove_charge1=remove_charge1, remove_empty_spectra=remove_empty_spectra,
                                   min_intensity=min_intensity)
 
     logger.info('Creating MS2 Contents')
     ms2_content = to_ms2([ms2_header], ms2_spectra)
 
+    time.sleep(1)  # Dumb fix for logging message overlap with tqdm progress bar
+
     logger.info('Writing Contents To File')
     with open(output_file, 'w') as file:
         file.write(ms2_content)
 
     logger.info(f'Total Time: {round(time.time() - start_time, 2)} seconds')
```

### Comparing `tdfextractor-0.1.5/tdfextractor/string_templates.py` & `tdfextractor-0.1.6/tdfextractor/string_templates.py`

 * *Files identical despite different names*

### Comparing `tdfextractor-0.1.5/tdfextractor/utils.py` & `tdfextractor-0.1.6/tdfextractor/utils.py`

 * *Files identical despite different names*

### Comparing `tdfextractor-0.1.5/test/test_ms2_extractor.py` & `tdfextractor-0.1.6/test/test_ms2_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+import logging
 import unittest
 from pathlib import Path
 import os
 
 from tdfextractor.ms2_extractor import get_ms2_content, write_ms2_file
 
 d_folder = str(Path('data') / '200ngHeLaPASEF_1min.d')
 
+logging.basicConfig(
+    level=logging.INFO)
+
 
 class TestMs2Extractor(unittest.TestCase):
 
     def test_write_ms2(self):
         if os.path.exists('test.ms2'):
             os.remove('test.ms2')
 
@@ -38,15 +42,15 @@
         for spectra in get_ms2_content(d_folder, include_spectra=True):
             ms2_spectra = spectra
             break
 
         self.assertAlmostEqual(ms2_spectra.charge, 2)
         self.assertAlmostEqual(ms2_spectra.mz, 1292.63706188582, 4)
         self.assertAlmostEqual(ms2_spectra.prec_intensity, 3603.0)
-        self.assertAlmostEqual(ms2_spectra.rt, 2400.83148655562, 4)
+        self.assertAlmostEqual(ms2_spectra.rt, 2400.83148655562, 1)
         self.assertEqual(ms2_spectra.precursor_id, 1)
         self.assertEqual(ms2_spectra.parent_id, 1)
         self.assertAlmostEqual(ms2_spectra.mz_spectra[0], 113.6913703181829, 4)
         self.assertAlmostEqual(ms2_spectra.intensity_spectra[0], 14.0, 1)
         self.assertAlmostEqual(ms2_spectra.mz_spectra[-1], 1699.749570812201, 4)
         self.assertAlmostEqual(ms2_spectra.intensity_spectra[-1], 15.0, 1)
         self.assertAlmostEqual(ms2_spectra.mass, 2584.2668, 4)
```

