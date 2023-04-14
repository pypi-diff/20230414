# Comparing `tmp/pipeline_csv-1.2.tar.gz` & `tmp/pipeline_csv-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_csv-1.2.tar", last modified: Wed Mar 29 13:56:03 2023, max compression
+gzip compressed data, was "pipeline_csv-1.3.tar", last modified: Fri Apr 14 08:12:18 2023, max compression
```

## Comparing `pipeline_csv-1.2.tar` & `pipeline_csv-1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 13:56:03.722203 pipeline_csv-1.2/
--rw-rw-rw-   0        0        0     1094 2023-03-13 10:59:03.000000 pipeline_csv-1.2/LICENSE
--rw-rw-rw-   0        0        0       60 2023-03-14 17:31:18.000000 pipeline_csv-1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     9267 2023-03-29 13:56:03.722203 pipeline_csv-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6631 2023-03-14 17:56:41.000000 pipeline_csv-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 13:56:03.690952 pipeline_csv-1.2/pipeline_csv/
--rw-rw-rw-   0        0        0      701 2023-03-15 17:59:16.000000 pipeline_csv-1.2/pipeline_csv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 13:56:03.722203 pipeline_csv-1.2/pipeline_csv/csvfile/
--rw-rw-rw-   0        0        0    10771 2023-03-14 17:31:18.000000 pipeline_csv-1.2/pipeline_csv/csvfile/README.md
--rw-rw-rw-   0        0        0     9438 2023-03-16 14:20:59.000000 pipeline_csv-1.2/pipeline_csv/csvfile/__init__.py
--rw-rw-rw-   0        0        0    15094 2023-03-29 13:42:39.000000 pipeline_csv-1.2/pipeline_csv/csvfile/row.py
--rw-rw-rw-   0        0        0     4461 2023-03-23 18:46:32.000000 pipeline_csv-1.2/pipeline_csv/csvfile/tubes.py
--rw-rw-rw-   0        0        0     5965 2023-03-29 13:25:05.000000 pipeline_csv-1.2/pipeline_csv/oegiv.py
--rw-rw-rw-   0        0        0     2259 2023-03-29 11:46:35.000000 pipeline_csv-1.2/pipeline_csv/orientation.py
-drwxrwxrwx   0        0        0        0 2023-03-29 13:56:03.706577 pipeline_csv-1.2/pipeline_csv.egg-info/
--rw-rw-rw-   0        0        0     9267 2023-03-29 13:56:03.000000 pipeline_csv-1.2/pipeline_csv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-03-29 13:56:03.000000 pipeline_csv-1.2/pipeline_csv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 13:56:03.000000 pipeline_csv-1.2/pipeline_csv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-29 13:56:03.000000 pipeline_csv-1.2/pipeline_csv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-03-14 17:31:18.000000 pipeline_csv-1.2/pyproject.toml
--rw-rw-rw-   0        0        0      664 2023-03-29 13:56:03.722203 pipeline_csv-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 08:12:18.635825 pipeline_csv-1.3/
+-rw-rw-rw-   0        0        0     1094 2023-03-13 10:59:03.000000 pipeline_csv-1.3/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-03-14 17:31:18.000000 pipeline_csv-1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     9222 2023-04-14 08:12:18.651449 pipeline_csv-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6634 2023-03-30 05:04:13.000000 pipeline_csv-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 08:12:18.588945 pipeline_csv-1.3/pipeline_csv/
+-rw-rw-rw-   0        0        0      701 2023-03-15 17:59:16.000000 pipeline_csv-1.3/pipeline_csv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:12:18.620198 pipeline_csv-1.3/pipeline_csv/csvfile/
+-rw-rw-rw-   0        0        0    10771 2023-03-14 17:31:18.000000 pipeline_csv-1.3/pipeline_csv/csvfile/README.md
+-rw-rw-rw-   0        0        0     9651 2023-03-30 11:58:25.000000 pipeline_csv-1.3/pipeline_csv/csvfile/__init__.py
+-rw-rw-rw-   0        0        0    15597 2023-03-30 11:58:25.000000 pipeline_csv-1.3/pipeline_csv/csvfile/row.py
+-rw-rw-rw-   0        0        0     4461 2023-03-23 18:46:32.000000 pipeline_csv-1.3/pipeline_csv/csvfile/tubes.py
+-rw-rw-rw-   0        0        0     5965 2023-03-29 13:25:05.000000 pipeline_csv-1.3/pipeline_csv/oegiv.py
+-rw-rw-rw-   0        0        0     2267 2023-04-14 04:49:03.000000 pipeline_csv-1.3/pipeline_csv/orientation.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:12:18.604573 pipeline_csv-1.3/pipeline_csv.egg-info/
+-rw-rw-rw-   0        0        0     9222 2023-04-14 08:12:18.000000 pipeline_csv-1.3/pipeline_csv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-04-14 08:12:18.000000 pipeline_csv-1.3/pipeline_csv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 08:12:18.000000 pipeline_csv-1.3/pipeline_csv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 08:12:18.000000 pipeline_csv-1.3/pipeline_csv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2023-03-14 17:31:18.000000 pipeline_csv-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      664 2023-04-14 08:12:18.651449 pipeline_csv-1.3/setup.cfg
```

### Comparing `pipeline_csv-1.2/LICENSE` & `pipeline_csv-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.2/PKG-INFO` & `pipeline_csv-1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline_csv
-Version: 1.2
+Version: 1.3
 Summary: Pipeline inline inspection data as CSV file.
 Home-page: https://github.com/vb64/pipeline.csv
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/vb64/pipeline.csv/issues
 Description: # PipelineCsv library
@@ -42,53 +42,47 @@
         from pipeline_csv.csvfile.row import Row
         
         class TypeMarker:
             VALVE = 0
             CASE_START = 1
             CASE_END = 2
         
-        LINEOBJ = {
-          TypeMarker.VALVE: "Valve",
-          TypeMarker.CASE_START: "Casing start",
-          TypeMarker.CASE_END: "Casing end",
-        }
-        
         class TypeDefekt:
             CORROZ = 0
             DENT = 1
         
-        DEFEKTS = {
-          TypeDefekt.CORROZ: "Corrosion",
-          TypeDefekt.DENT: "Dent",
-        }
-        
         class MyRow(Row):
         
             @staticmethod
             def defekts_dict():
-                return DEFEKTS
+                return {
+                  TypeDefekt.CORROZ: "Corrosion",
+                  TypeDefekt.DENT: "Dent",
+                }
         
             @staticmethod
             def lineobj_dict():
-                return LINEOBJ
+                return {
+                  TypeMarker.VALVE: "Valve",
+                  TypeMarker.CASE_START: "Casing start",
+                  TypeMarker.CASE_END: "Casing end",
+                }
         ```
         
         For the data mirroring operation, you need to override the `markers_reverse` method, which returns a dictionary that specifies the rules for replacing when mirroring.
         
         ```python
-        REVERSE_MARKER = {
-          TypeMarker.CASE_START: TypeMarker.CASE_END,
-          TypeMarker.CASE_END: TypeMarker.CASE_START,
-        }
-        
         class MyRow(Row):
         
             @staticmethod
             def markers_reverse():
-                return REVERSE_MARKER
+                return {
+                  TypeMarker.CASE_START: TypeMarker.CASE_END,
+                  TypeMarker.CASE_END: TypeMarker.CASE_START,
+                }
         ```
         
         Further, the MyRow class can be used in operations with data of CSV files.
         
         ### Creating a CSV file
         
         Construct new csv file from scratch.
```

### Comparing `pipeline_csv-1.2/README.md` & `pipeline_csv-1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -33,53 +33,47 @@
 from pipeline_csv.csvfile.row import Row
 
 class TypeMarker:
     VALVE = 0
     CASE_START = 1
     CASE_END = 2
 
-LINEOBJ = {
-  TypeMarker.VALVE: "Valve",
-  TypeMarker.CASE_START: "Casing start",
-  TypeMarker.CASE_END: "Casing end",
-}
-
 class TypeDefekt:
     CORROZ = 0
     DENT = 1
 
-DEFEKTS = {
-  TypeDefekt.CORROZ: "Corrosion",
-  TypeDefekt.DENT: "Dent",
-}
-
 class MyRow(Row):
 
     @staticmethod
     def defekts_dict():
-        return DEFEKTS
+        return {
+          TypeDefekt.CORROZ: "Corrosion",
+          TypeDefekt.DENT: "Dent",
+        }
 
     @staticmethod
     def lineobj_dict():
-        return LINEOBJ
+        return {
+          TypeMarker.VALVE: "Valve",
+          TypeMarker.CASE_START: "Casing start",
+          TypeMarker.CASE_END: "Casing end",
+        }
 ```
 
 For the data mirroring operation, you need to override the `markers_reverse` method, which returns a dictionary that specifies the rules for replacing when mirroring.
 
 ```python
-REVERSE_MARKER = {
-  TypeMarker.CASE_START: TypeMarker.CASE_END,
-  TypeMarker.CASE_END: TypeMarker.CASE_START,
-}
-
 class MyRow(Row):
 
     @staticmethod
     def markers_reverse():
-        return REVERSE_MARKER
+        return {
+          TypeMarker.CASE_START: TypeMarker.CASE_END,
+          TypeMarker.CASE_END: TypeMarker.CASE_START,
+        }
 ```
 
 Further, the MyRow class can be used in operations with data of CSV files.
 
 ### Creating a CSV file
 
 Construct new csv file from scratch.
```

### Comparing `pipeline_csv-1.2/pipeline_csv/__init__.py` & `pipeline_csv-1.3/pipeline_csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.2/pipeline_csv/csvfile/README.md` & `pipeline_csv-1.3/pipeline_csv/csvfile/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.2/pipeline_csv/csvfile/__init__.py` & `pipeline_csv-1.3/pipeline_csv/csvfile/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Interfaces for csv file."""
+import os
 import csv
 from .. import Error
 from .row import Row as BaseRow
 
 
 def transform_length(dist_od, length_od, table, table_index):
     """Modify length at given dist according table.
@@ -94,14 +95,15 @@
     ]
 
 
 class File:
     """Export/import csv file."""
 
     RowCls = BaseRow
+    file_name = 'DefTable.csv'
     ENCODING = 'utf-8'
     DELIMETER = ';'
     COLUMN_HEADS = [
       'DistOd',
       'TypeObject',
       'Object_Code',
       'ObjectName',
@@ -140,14 +142,19 @@
 
     @classmethod
     def open_file(cls, file_path, mode):
         """Open file wrapper."""
         return open(file_path, mode + 't', encoding=cls.ENCODING)
 
     @classmethod
+    def at_folder(cls, folder):
+        """Restore from file in given folder."""
+        return cls.from_file(os.path.join(folder, cls.file_name))
+
+    @classmethod
     def from_file(cls, file_path, float_delimiter=FloatDelimiter.Point):
         """Construct from export csv file."""
         obj = cls(float_delimiter=float_delimiter)
         reader = csv.reader(cls.open_file(file_path, 'r'), delimiter=cls.DELIMETER)
         next(reader)  # skip column titles row
         for row in reader:
```

### Comparing `pipeline_csv-1.2/pipeline_csv/csvfile/row.py` & `pipeline_csv-1.3/pipeline_csv/csvfile/row.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     def __init__(self):
         """Create empty csv row object."""
         self.dist_od = None
         self.type_object = None
         self.object_code = 0
         self.object_name = ''
         self.object_code_t = ''
-        self.marker = self.get_bool(False)
+        self.is_marker_int = False
         self.length = ''
         self.width = ''
         self.depth_min = ''
         self.depth_max = ''
         self.orient_td = ''
         self.orient_bd = ''
         self.mpoint_orient = ''
@@ -153,14 +153,31 @@
         self.altitude = ''
 
     def __str__(self):
         """String representation for row object."""
         return ';'.join([str(i) for i in self.values()])
 
     @property
+    def marker(self):
+        """Return string for marker feature."""
+        return self.get_bool(self.is_marker_int)
+
+    @marker.setter
+    def marker(self, val):
+        """Set internal field based on string for marker feature."""
+        self.is_marker_int = False
+        if val == self.get_bool(True):
+            self.is_marker_int = True
+
+    @property
+    def is_marker(self):
+        """Return marker feature as bool."""
+        return self.is_lineobj and self.is_marker_int
+
+    @property
     def dist(self):
         """Return object distance as integer mm."""
         return int(self.dist_od)
 
     @staticmethod
     def get_minutes(text):
         """Restore full integer minute from text 'hours,minites'."""
@@ -257,15 +274,15 @@
             raise Error("Wrong lineobj type: {}".format(typ))
 
         obj = cls.with_dist(distanse, latitude, longtitude, altitude)
         obj.type_object = ObjectClass.MARKER
         obj.object_code = typ
         obj.object_code_t = lineobj[obj.object_code]
         obj.object_name = name
-        obj.marker = cls.get_bool(is_marker)
+        obj.is_marker_int = is_marker
         obj.comments = comment
 
         return obj
 
     @classmethod
     def as_defekt(  # pylint: disable=too-many-locals
       cls, distanse, typ, side, length, width, depth, orient1, orient2, mp_orient, mp_dist, comment,
```

### Comparing `pipeline_csv-1.2/pipeline_csv/csvfile/tubes.py` & `pipeline_csv-1.3/pipeline_csv/csvfile/tubes.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.2/pipeline_csv/oegiv.py` & `pipeline_csv-1.3/pipeline_csv/oegiv.py`

 * *Files identical despite different names*

### Comparing `pipeline_csv-1.2/pipeline_csv/orientation.py` & `pipeline_csv-1.3/pipeline_csv/orientation.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             minutes = '0{}'.format(minutes)
 
         return "{},{}".format(hours, minutes)
 
     @property
     def as_minutes(self):
         """Return orientation as integer minutes."""
-        return self.hours * 60 + self.minutes
+        return (self.hours * 60 + self.minutes) % 720
 
     @classmethod
     def from_hour_float(cls, hour_float):
         """Construct object from hours as float."""
         parttial_hour, hours = math.modf(hour_float)
         minutes = parttial_hour * 60
         return cls(int(hours), int(minutes))
```

### Comparing `pipeline_csv-1.2/pipeline_csv.egg-info/PKG-INFO` & `pipeline_csv-1.3/pipeline_csv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-csv
-Version: 1.2
+Version: 1.3
 Summary: Pipeline inline inspection data as CSV file.
 Home-page: https://github.com/vb64/pipeline.csv
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/vb64/pipeline.csv/issues
 Description: # PipelineCsv library
@@ -42,53 +42,47 @@
         from pipeline_csv.csvfile.row import Row
         
         class TypeMarker:
             VALVE = 0
             CASE_START = 1
             CASE_END = 2
         
-        LINEOBJ = {
-          TypeMarker.VALVE: "Valve",
-          TypeMarker.CASE_START: "Casing start",
-          TypeMarker.CASE_END: "Casing end",
-        }
-        
         class TypeDefekt:
             CORROZ = 0
             DENT = 1
         
-        DEFEKTS = {
-          TypeDefekt.CORROZ: "Corrosion",
-          TypeDefekt.DENT: "Dent",
-        }
-        
         class MyRow(Row):
         
             @staticmethod
             def defekts_dict():
-                return DEFEKTS
+                return {
+                  TypeDefekt.CORROZ: "Corrosion",
+                  TypeDefekt.DENT: "Dent",
+                }
         
             @staticmethod
             def lineobj_dict():
-                return LINEOBJ
+                return {
+                  TypeMarker.VALVE: "Valve",
+                  TypeMarker.CASE_START: "Casing start",
+                  TypeMarker.CASE_END: "Casing end",
+                }
         ```
         
         For the data mirroring operation, you need to override the `markers_reverse` method, which returns a dictionary that specifies the rules for replacing when mirroring.
         
         ```python
-        REVERSE_MARKER = {
-          TypeMarker.CASE_START: TypeMarker.CASE_END,
-          TypeMarker.CASE_END: TypeMarker.CASE_START,
-        }
-        
         class MyRow(Row):
         
             @staticmethod
             def markers_reverse():
-                return REVERSE_MARKER
+                return {
+                  TypeMarker.CASE_START: TypeMarker.CASE_END,
+                  TypeMarker.CASE_END: TypeMarker.CASE_START,
+                }
         ```
         
         Further, the MyRow class can be used in operations with data of CSV files.
         
         ### Creating a CSV file
         
         Construct new csv file from scratch.
```

### Comparing `pipeline_csv-1.2/setup.cfg` & `pipeline_csv-1.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6970 656c 696e 655f 6373 760d   = pipeline_csv.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e32 0d0a  .version = 1.2..
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e33 0d0a  .version = 1.3..
 00000030: 6175 7468 6f72 203d 2056 6974 616c 7920  author = Vitaly 
 00000040: 426f 676f 6d6f 6c6f 760d 0a61 7574 686f  Bogomolov..autho
 00000050: 725f 656d 6169 6c20 3d20 6d61 696c 4076  r_email = mail@v
 00000060: 6974 616c 792d 626f 676f 6d6f 6c6f 762e  italy-bogomolov.
 00000070: 7275 0d0a 6465 7363 7269 7074 696f 6e20  ru..description 
 00000080: 3d20 5069 7065 6c69 6e65 2069 6e6c 696e  = Pipeline inlin
 00000090: 6520 696e 7370 6563 7469 6f6e 2064 6174  e inspection dat
```

