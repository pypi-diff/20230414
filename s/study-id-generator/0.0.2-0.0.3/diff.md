# Comparing `tmp/study_id_generator-0.0.2.tar.gz` & `tmp/study_id_generator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "study_id_generator-0.0.2.tar", last modified: Fri Apr 14 01:43:25 2023, max compression
+gzip compressed data, was "study_id_generator-0.0.3.tar", last modified: Fri Apr 14 12:29:04 2023, max compression
```

## Comparing `study_id_generator-0.0.2.tar` & `study_id_generator-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 01:43:25.312641 study_id_generator-0.0.2/
--rw-rw-rw-   0        0        0     1380 2023-04-14 01:43:25.312641 study_id_generator-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      798 2023-04-14 01:28:57.000000 study_id_generator-0.0.2/README.md
--rw-rw-rw-   0        0        0      873 2023-04-14 01:42:56.000000 study_id_generator-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 01:43:25.312641 study_id_generator-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 01:43:25.283053 study_id_generator-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 01:43:25.295918 study_id_generator-0.0.2/src/study_id_generator/
--rw-rw-rw-   0        0        0        0 2023-04-13 18:17:34.000000 study_id_generator-0.0.2/src/study_id_generator/__init__.py
--rw-rw-rw-   0        0        0     5676 2023-04-14 01:31:11.000000 study_id_generator-0.0.2/src/study_id_generator/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 01:43:25.304622 study_id_generator-0.0.2/src/study_id_generator.egg-info/
--rw-rw-rw-   0        0        0     1380 2023-04-14 01:43:25.000000 study_id_generator-0.0.2/src/study_id_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-04-14 01:43:25.000000 study_id_generator-0.0.2/src/study_id_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 01:43:25.000000 study_id_generator-0.0.2/src/study_id_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-04-14 01:43:25.000000 study_id_generator-0.0.2/src/study_id_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-14 01:43:25.000000 study_id_generator-0.0.2/src/study_id_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 12:29:04.983619 study_id_generator-0.0.3/
+-rw-rw-rw-   0        0        0     1380 2023-04-14 12:29:04.982890 study_id_generator-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-04-14 01:28:57.000000 study_id_generator-0.0.3/README.md
+-rw-rw-rw-   0        0        0      873 2023-04-14 12:26:47.000000 study_id_generator-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 12:29:04.984269 study_id_generator-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 12:29:04.966441 study_id_generator-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 12:29:04.972479 study_id_generator-0.0.3/src/study_id_generator/
+-rw-rw-rw-   0        0        0        0 2023-04-13 18:17:34.000000 study_id_generator-0.0.3/src/study_id_generator/__init__.py
+-rw-rw-rw-   0        0        0     5742 2023-04-14 12:11:38.000000 study_id_generator-0.0.3/src/study_id_generator/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:29:04.981229 study_id_generator-0.0.3/src/study_id_generator.egg-info/
+-rw-rw-rw-   0        0        0     1380 2023-04-14 12:29:04.000000 study_id_generator-0.0.3/src/study_id_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-04-14 12:29:04.000000 study_id_generator-0.0.3/src/study_id_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 12:29:04.000000 study_id_generator-0.0.3/src/study_id_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-04-14 12:29:04.000000 study_id_generator-0.0.3/src/study_id_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-14 12:29:04.000000 study_id_generator-0.0.3/src/study_id_generator.egg-info/top_level.txt
```

### Comparing `study_id_generator-0.0.2/PKG-INFO` & `study_id_generator-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: study_id_generator
-Version: 0.0.2
+Version: 0.0.3
 Summary: Study ID Generator.
 Author-email: Sushant Obeja <sobeja@umich.edu>, Adam Patterson <adpatter@umich.edu>
 Project-URL: Homepage, https://git.umms.med.umich.edu/feldman-lab/study_id_generator
 Project-URL: Bug Tracker, https://git.umms.med.umich.edu/feldman-lab/study_id_generator/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `study_id_generator-0.0.2/README.md` & `study_id_generator-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `study_id_generator-0.0.2/pyproject.toml` & `study_id_generator-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "study_id_generator"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Sushant Obeja", email="sobeja@umich.edu" },
     { name="Adam Patterson", email="adpatter@umich.edu" },
 ]
 description = "Study ID Generator."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `study_id_generator-0.0.2/src/study_id_generator/__main__.py` & `study_id_generator-0.0.3/src/study_id_generator/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,26 +46,25 @@
         config = configparser.ConfigParser()
         config.read(config_path)
 
         self._MIN_ID = int(config['DEFAULT']['MIN_ID'])
         self._MAX_ID = int(config['DEFAULT']['MAX_ID'])
         self._ID_WIDTH = int(config['DEFAULT']['ID_WIDTH'])
         self._ID_FILLCHAR = config['DEFAULT']['ID_FILLCHAR']
+        self._SAMPLE_FRAC = float(config['DEFAULT']['SAMPLE_FRAC'])
 
         self._section = {section:config[section] for section in config.sections()}
 
     def on_press(self, event):
 
         try:
             self.panel.SetCursor(wx.Cursor(wx.CURSOR_ARROWWAIT))
 
             self.study_id_window.Clear()
             self.study_id_window.Update()
-            self.log_window.Clear()
-            self.log_window.Update()
 
             ids = []
 
             for section_name, section in self._section.items():
                 data = {
                     'token': section['API_KEY'],
                     'content': 'record',
@@ -96,14 +95,16 @@
 
             id_variants = pd.Series(range(self._MIN_ID, self._MAX_ID))
 
             id_variants = id_variants.astype(str).str.pad(self._ID_WIDTH, side='left', fillchar=self._ID_FILLCHAR)
 
             id_variants = id_variants.loc[~id_variants.isin(df['id'])]
 
+            id_variants = id_variants.sample(frac=self._SAMPLE_FRAC)
+
             df['id_variant'] = [id_variants.tolist()] * df.shape[0]
 
             df = df.explode('id_variant')
 
             self.log_window.AppendText(f"Calculating pairwise distance between {df.shape[0]} pairs of identifiers...\n")
 
             df['id_vector'] = df['id'].apply(lambda x: [int(i) for i in list(x)])
```

### Comparing `study_id_generator-0.0.2/src/study_id_generator.egg-info/PKG-INFO` & `study_id_generator-0.0.3/src/study_id_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: study-id-generator
-Version: 0.0.2
+Version: 0.0.3
 Summary: Study ID Generator.
 Author-email: Sushant Obeja <sobeja@umich.edu>, Adam Patterson <adpatter@umich.edu>
 Project-URL: Homepage, https://git.umms.med.umich.edu/feldman-lab/study_id_generator
 Project-URL: Bug Tracker, https://git.umms.med.umich.edu/feldman-lab/study_id_generator/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

