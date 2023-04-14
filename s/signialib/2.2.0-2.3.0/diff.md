# Comparing `tmp/signialib-2.2.0.tar.gz` & `tmp/signialib-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signialib-2.2.0.tar", max compression
+gzip compressed data, was "signialib-2.3.0.tar", max compression
```

## Comparing `signialib-2.2.0.tar` & `signialib-2.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1073 2023-03-13 20:06:45.336745 signialib-2.2.0/LICENSE
--rw-r--r--   0        0        0     1805 2023-03-13 20:06:45.336745 signialib-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      584 2023-03-13 20:06:45.336745 signialib-2.2.0/signialib/__init__.py
--rw-r--r--   0        0        0     3998 2023-03-13 20:06:45.336745 signialib-2.2.0/signialib/_session_base.py
--rw-r--r--   0        0        0     2113 2023-03-13 20:06:45.336745 signialib-2.2.0/signialib/calibrations/001/Ferraris/2022-07-24_16-00/001_2022-01-10_10-48.json
--rw-r--r--   0        0        0     2117 2023-03-13 20:06:45.336745 signialib-2.2.0/signialib/calibrations/002/Ferraris/2022-07-24_16-00/002_2022-01-10_10-48.json
--rw-r--r--   0        0        0      600 2023-03-13 20:06:45.336745 signialib-2.2.0/signialib/consts.py
--rwxr-xr-x   0        0        0    27447 2023-03-13 20:06:45.336745 signialib-2.2.0/signialib/dataset.py
--rw-r--r--   0        0        0      265 2023-03-13 20:06:45.336745 signialib-2.2.0/signialib/exceptions.py
--rw-r--r--   0        0        0    11384 2023-03-13 20:06:45.336745 signialib-2.2.0/signialib/header.py
--rwxr-xr-x   0        0        0    10263 2023-03-13 20:06:45.336745 signialib-2.2.0/signialib/session.py
--rwxr-xr-x   0        0        0     1695 2023-03-13 20:06:45.336745 signialib-2.2.0/signialib/utils.py
--rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 signialib-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-14 11:54:46.848297 signialib-2.3.0/LICENSE
+-rw-r--r--   0        0        0     1805 2023-04-14 11:54:46.852297 signialib-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      584 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/__init__.py
+-rw-r--r--   0        0        0     3998 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/_session_base.py
+-rw-r--r--   0        0        0     2113 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/calibrations/001/Ferraris/2022-07-24_16-00/001_2022-01-10_10-48.json
+-rw-r--r--   0        0        0     2117 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/calibrations/002/Ferraris/2022-07-24_16-00/002_2022-01-10_10-48.json
+-rw-r--r--   0        0        0      600 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/consts.py
+-rwxr-xr-x   0        0        0    28466 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/dataset.py
+-rw-r--r--   0        0        0      265 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/exceptions.py
+-rw-r--r--   0        0        0    11384 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/header.py
+-rwxr-xr-x   0        0        0    10263 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/session.py
+-rwxr-xr-x   0        0        0     1695 2023-04-14 11:54:46.852297 signialib-2.3.0/signialib/utils.py
+-rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 signialib-2.3.0/PKG-INFO
```

### Comparing `signialib-2.2.0/LICENSE` & `signialib-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `signialib-2.2.0/pyproject.toml` & `signialib-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "signialib"
-version = "2.2.0"
+version = "2.3.0"
 description = "Data handling of the IMUs integrated into Signia hearing aids"
 authors = ["Ann-Kristin Seifer <ann-kristin.seifer@fau.de>", 
         "Arne Küderle <arne.kuederle@fau.de>",
         "Nils Roth <nils.roth@fau.de>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `signialib-2.2.0/signialib/__init__.py` & `signialib-2.3.0/signialib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 
 from .dataset import Dataset  # noqa: F401
 from .session import Session  # noqa: F401
 
 SIGNIA_CAL_PATH = Path(__file__).parent / "calibrations"
 
 __all__ = ["Dataset", "Session", "SIGNIA_CAL_PATH"]
-__version__ = "2.2.0"
+__version__ = "2.3.0"
```

### Comparing `signialib-2.2.0/signialib/_session_base.py` & `signialib-2.3.0/signialib/_session_base.py`

 * *Files identical despite different names*

### Comparing `signialib-2.2.0/signialib/calibrations/001/Ferraris/2022-07-24_16-00/001_2022-01-10_10-48.json` & `signialib-2.3.0/signialib/calibrations/001/Ferraris/2022-07-24_16-00/001_2022-01-10_10-48.json`

 * *Files identical despite different names*

### Comparing `signialib-2.2.0/signialib/calibrations/002/Ferraris/2022-07-24_16-00/002_2022-01-10_10-48.json` & `signialib-2.3.0/signialib/calibrations/002/Ferraris/2022-07-24_16-00/002_2022-01-10_10-48.json`

 * *Files identical despite different names*

### Comparing `signialib-2.2.0/signialib/consts.py` & `signialib-2.3.0/signialib/consts.py`

 * *Files identical despite different names*

### Comparing `signialib-2.2.0/signialib/dataset.py` & `signialib-2.3.0/signialib/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -556,25 +556,28 @@
         The session header
     labels:
         Labels from app.
 
     """
     # read in data
     lines = read_in_txt_file(path)
-    data_raw = read_in_txt_file_as_df(path)
-    imu_sensor = get_sensor_type(data_raw)
+    imu_sensor = get_sensor_type(path)
+    data_raw, start_label = read_in_txt_file_as_df(path, imu_sensor)
 
     session_header = Header.from_list_txt(lines[0:9], lines[-1][0:12], imu_sensor)
 
     data_matrix = get_data_matrix(data_raw)
 
     counter, sensor_data, local_datetime_counter = get_sensor_data_txt(data_matrix, session_header)
 
     # get labels
-    labels = data_raw.loc[data_raw[1] != "accelerometer"][1]
+    labels = data_raw.loc[(data_raw[1] != "accelerometer") & (data_raw[1] != "motion sensor")][1]
+
+    if start_label is not None:
+        labels = _add_first_label_to_label_list(labels, start_label)
 
     return sensor_data, counter, session_header, local_datetime_counter, labels
 
 
 def read_in_txt_file(path):
     with open(path, encoding="utf-8-sig") as f:
         lines = [line.strip() for line in f.readlines()]
@@ -583,29 +586,47 @@
             "Raw .txt format of old app version containing hexadezimal values for sensor data is used. "
             "Importer for old format does not exists. "
             "Please use the format, in which sensor data is converted to floats."
         )
     return lines
 
 
-def read_in_txt_file_as_df(path):
-    data_raw = pd.read_csv(path, skiprows=9, header=None, engine="python", sep=r" - |: |, |] |]", index_col=0).iloc[
-        :, :-1
-    ]
+def read_in_txt_file_as_df(path, imu_sensor):
+
+    if imu_sensor == "BMA400":
+        skiprow = 9
+    else:
+        skiprow = 10
+    try:
+        data_raw = pd.read_csv(
+            path, skiprows=skiprow, header=None, engine="python", sep=r" - |: |, |] |]", index_col=0
+        ).iloc[:, :-1]
+        label = None
+    except pd.errors.ParserError:
+        data_raw = pd.read_csv(
+            path, skiprows=skiprow + 1, header=None, engine="python", sep=r" - |: |, |] |]", index_col=0
+        ).iloc[:, :-1]
+        label = pd.read_csv(
+            path, skiprows=skiprow, nrows=1, engine="python", header=None, index_col=0, sep="- "
+        ).squeeze(axis=1)
+
     if data_raw.shape[0] == 0:
         raise ValueError(
             "Raw .txt format of old app version containing hexadezimal values for sensor data is used. "
             "Importer for old format does not exists. "
             "Please use the format, in which sensor data is converted to floats."
         )
-    return data_raw
+    return data_raw, label
 
 
-def get_sensor_type(data_raw):
-    name = data_raw.iloc[0].iloc[0]
+def get_sensor_type(path):
+    data_raw = pd.read_csv(path, skiprows=12, header=None, engine="python", sep=r" - |: |, |] |]", index_col=0).iloc[
+        :, :-1
+    ]
+    name = data_raw[1].value_counts().index[0]
     if name == "motion sensor":
         return "BMA400"
     if name == "accelerometer":
         return "BMI270"
     return None
 
 
@@ -721,14 +742,22 @@
     for i in range(no_packages):
         package = data_matrix[[i * 6 + 3, i * 6 + 5, i * 6 + 7]]
         package.columns = ["x", "y", "z"]
         df = pd.concat([df, package])
     return df.reset_index(drop=True)
 
 
+def _add_first_label_to_label_list(labels, start_label):
+    if labels.shape[0] == 0:
+        return_labels = start_label
+    else:
+        return_labels = pd.concat([start_label, labels])
+    return return_labels
+
+
 def _create_local_datetime_counter_unsorted(
     time_index: np.ndarray, session_header: Header, no_packages: int
 ) -> np.ndarray:
     """Expand Datetime Index to fit number of sample points.
 
     For each package a fixed number of sample point are transmitted.
     Datetime index is expanded to fit the number of sample points: len = len(time_index)*no_packages.
```

### Comparing `signialib-2.2.0/signialib/header.py` & `signialib-2.3.0/signialib/header.py`

 * *Files identical despite different names*

### Comparing `signialib-2.2.0/signialib/session.py` & `signialib-2.3.0/signialib/session.py`

 * *Files identical despite different names*

### Comparing `signialib-2.2.0/signialib/utils.py` & `signialib-2.3.0/signialib/utils.py`

 * *Files identical despite different names*

### Comparing `signialib-2.2.0/PKG-INFO` & `signialib-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signialib
-Version: 2.2.0
+Version: 2.3.0
 Summary: Data handling of the IMUs integrated into Signia hearing aids
 Author: Ann-Kristin Seifer
 Author-email: ann-kristin.seifer@fau.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

