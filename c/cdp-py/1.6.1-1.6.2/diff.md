# Comparing `tmp/cdp-py-1.6.1.tar.gz` & `tmp/cdp-py-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdp-py-1.6.1.tar", last modified: Fri Apr 14 14:59:11 2023, max compression
+gzip compressed data, was "cdp-py-1.6.2.tar", last modified: Fri Apr 14 16:02:52 2023, max compression
```

## Comparing `cdp-py-1.6.1.tar` & `cdp-py-1.6.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:59:11.774792 cdp-py-1.6.1/
--rw-r--r--   0 root         (0) root         (0)     1910 2023-04-14 14:59:11.774792 cdp-py-1.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1511 2023-04-14 14:59:10.000000 cdp-py-1.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:59:11.738791 cdp-py-1.6.1/cdp/
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-04-11 17:33:12.000000 cdp-py-1.6.1/cdp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23077 2023-04-11 17:33:12.000000 cdp-py-1.6.1/cdp/cdp.py
--rw-rw-rw-   0 root         (0) root         (0)     1350 2023-04-11 17:33:12.000000 cdp-py-1.6.1/cdp/ciholas_serial_number.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:59:11.750791 cdp-py-1.6.1/cdp/data_items/
--rw-rw-rw-   0 root         (0) root         (0)      975 2023-04-11 17:33:12.000000 cdp-py-1.6.1/cdp/data_items/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    99211 2023-04-11 17:33:12.000000 cdp-py-1.6.1/cdp/data_items/data_items.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:59:11.774792 cdp-py-1.6.1/cdp_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1910 2023-04-14 14:59:11.000000 cdp-py-1.6.1/cdp_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      250 2023-04-14 14:59:11.000000 cdp-py-1.6.1/cdp_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 14:59:11.000000 cdp-py-1.6.1/cdp_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-14 14:59:11.000000 cdp-py-1.6.1/cdp_py.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 14:59:11.774792 cdp-py-1.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-04-14 14:59:10.000000 cdp-py-1.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:02:52.112553 cdp-py-1.6.2/
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-04-14 16:02:52.112553 cdp-py-1.6.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2023-04-14 16:02:51.000000 cdp-py-1.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:02:52.108553 cdp-py-1.6.2/cdp/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-03-13 13:38:02.000000 cdp-py-1.6.2/cdp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23077 2023-03-13 13:38:02.000000 cdp-py-1.6.2/cdp/cdp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2023-03-13 13:38:02.000000 cdp-py-1.6.2/cdp/ciholas_serial_number.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:02:52.108553 cdp-py-1.6.2/cdp/data_items/
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-03-13 13:38:02.000000 cdp-py-1.6.2/cdp/data_items/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    99871 2023-04-14 16:02:31.000000 cdp-py-1.6.2/cdp/data_items/data_items.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 16:02:52.108553 cdp-py-1.6.2/cdp_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-04-14 16:02:52.000000 cdp-py-1.6.2/cdp_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2023-04-14 16:02:52.000000 cdp-py-1.6.2/cdp_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 16:02:52.000000 cdp-py-1.6.2/cdp_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-14 16:02:52.000000 cdp-py-1.6.2/cdp_py.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 16:02:52.112553 cdp-py-1.6.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-04-14 16:02:51.000000 cdp-py-1.6.2/setup.py
```

### Comparing `cdp-py-1.6.1/PKG-INFO` & `cdp-py-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdp-py
-Version: 1.6.1
+Version: 1.6.2
 Summary: Ciholas Data Protocol
 Home-page: https://github.com/ciholas/cdp-py
 Author: Ciholas, Inc.
 Author-email: cuwb.support@ciholas.com
 License: CC BY 4.0
 Keywords: cdp ciholas data protocol
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cdp-py-1.6.1/README.md` & `cdp-py-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `cdp-py-1.6.1/cdp/cdp.py` & `cdp-py-1.6.2/cdp/cdp.py`

 * *Files identical despite different names*

### Comparing `cdp-py-1.6.1/cdp/ciholas_serial_number.py` & `cdp-py-1.6.2/cdp/ciholas_serial_number.py`

 * *Files identical despite different names*

### Comparing `cdp-py-1.6.1/cdp/data_items/__init__.py` & `cdp-py-1.6.2/cdp/data_items/__init__.py`

 * *Files identical despite different names*

### Comparing `cdp-py-1.6.1/cdp/data_items/data_items.py` & `cdp-py-1.6.2/cdp/data_items/data_items.py`

 * *Files 1% similar despite different names*

```diff
@@ -1491,14 +1491,25 @@
     def add_led_states(self, start_time_offset=0, led_duration=0,
                        led_period=0, red=0, green=0, blue=0):
         """Adds an LED State object to the LED states list."""
         self.led_states.append(LEDStates(start_time_offset, led_duration,
                                          led_period, red, green, blue))
 
 
+class DeviceData(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol Device Data Data Item Definition. Protected.
+       This data type contains general and specific info for device data types."""
+
+    type = 0x8042
+    definition = [DIUInt64Attr('nt64'), # Reception time at the anchor.
+                  DISignalStrengthAttr('signal_strength'), # Signal Strength of the reception.
+                  DIUInt8Attr('interface_id'), # Interface ID of the receiver.
+                  DIUInt8Attr('nt_quality'), # The quality of the reported Network Time.
+                  DIVariableLengthBytesAttr('device_data')] # Contents of the Device Data UWB packet.
+
 
 # When adding a new data item to cdp-py, follow the template given below.
 # class <classname>(CDPDataItem):
 #     """CDP Data Item: Ciholas Data Protocol <description> Data Item Definition. <version description (current in v3.3, deprecated, protected, etc.)>.
 #        This data type <more detailed description (optional)>."""
 #
 #     type = <typename (0x0000)>
```

### Comparing `cdp-py-1.6.1/cdp_py.egg-info/PKG-INFO` & `cdp-py-1.6.2/cdp_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdp-py
-Version: 1.6.1
+Version: 1.6.2
 Summary: Ciholas Data Protocol
 Home-page: https://github.com/ciholas/cdp-py
 Author: Ciholas, Inc.
 Author-email: cuwb.support@ciholas.com
 License: CC BY 4.0
 Keywords: cdp ciholas data protocol
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cdp-py-1.6.1/setup.py` & `cdp-py-1.6.2/setup.py`

 * *Files identical despite different names*

