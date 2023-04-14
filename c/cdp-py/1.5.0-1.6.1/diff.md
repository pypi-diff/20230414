# Comparing `tmp/cdp-py-1.5.0.tar.gz` & `tmp/cdp-py-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cdp-py-1.5.0.tar", last modified: Tue Aug 25 16:36:23 2020, max compression
+gzip compressed data, was "cdp-py-1.6.1.tar", last modified: Fri Apr 14 14:59:11 2023, max compression
```

## Comparing `cdp-py-1.5.0.tar` & `cdp-py-1.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-25 16:36:23.000000 cdp-py-1.5.0/
--rw-r--r--   0 root         (0) root         (0)     2277 2020-08-25 16:36:23.000000 cdp-py-1.5.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-25 16:36:23.000000 cdp-py-1.5.0/cdp/
--rw-rw-rw-   0 root         (0) root         (0)    23077 2020-08-25 16:31:04.000000 cdp-py-1.5.0/cdp/cdp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-25 16:36:23.000000 cdp-py-1.5.0/cdp/data_items/
--rw-rw-rw-   0 root         (0) root         (0)    82862 2020-08-25 16:31:04.000000 cdp-py-1.5.0/cdp/data_items/data_items.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2020-08-25 16:31:04.000000 cdp-py-1.5.0/cdp/data_items/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       46 2020-08-25 16:31:04.000000 cdp-py-1.5.0/cdp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2020-08-25 16:31:04.000000 cdp-py-1.5.0/cdp/ciholas_serial_number.py
--rw-rw-rw-   0 root         (0) root         (0)      650 2020-08-25 16:31:04.000000 cdp-py-1.5.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1511 2020-08-25 16:35:31.000000 cdp-py-1.5.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2020-08-25 16:36:23.000000 cdp-py-1.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-25 16:36:23.000000 cdp-py-1.5.0/cdp_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2277 2020-08-25 16:36:23.000000 cdp-py-1.5.0/cdp_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2020-08-25 16:36:23.000000 cdp-py-1.5.0/cdp_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      250 2020-08-25 16:36:23.000000 cdp-py-1.5.0/cdp_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        4 2020-08-25 16:36:23.000000 cdp-py-1.5.0/cdp_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:59:11.774792 cdp-py-1.6.1/
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-04-14 14:59:11.774792 cdp-py-1.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2023-04-14 14:59:10.000000 cdp-py-1.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:59:11.738791 cdp-py-1.6.1/cdp/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-04-11 17:33:12.000000 cdp-py-1.6.1/cdp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23077 2023-04-11 17:33:12.000000 cdp-py-1.6.1/cdp/cdp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2023-04-11 17:33:12.000000 cdp-py-1.6.1/cdp/ciholas_serial_number.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:59:11.750791 cdp-py-1.6.1/cdp/data_items/
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-04-11 17:33:12.000000 cdp-py-1.6.1/cdp/data_items/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    99211 2023-04-11 17:33:12.000000 cdp-py-1.6.1/cdp/data_items/data_items.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 14:59:11.774792 cdp-py-1.6.1/cdp_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-04-14 14:59:11.000000 cdp-py-1.6.1/cdp_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2023-04-14 14:59:11.000000 cdp-py-1.6.1/cdp_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 14:59:11.000000 cdp-py-1.6.1/cdp_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-14 14:59:11.000000 cdp-py-1.6.1/cdp_py.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 14:59:11.774792 cdp-py-1.6.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-04-14 14:59:10.000000 cdp-py-1.6.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cdp-py-1.5.0/PKG-INFO` & `cdp-py-1.6.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: cdp-py
-Version: 1.5.0
+Version: 1.6.1
 Summary: Ciholas Data Protocol
 Home-page: https://github.com/ciholas/cdp-py
 Author: Ciholas, Inc.
 Author-email: cuwb.support@ciholas.com
 License: CC BY 4.0
-Description: # cdp-py
-        
-        The Ciholas Data Protocol (CDP) provides a method of communication between devices and services. CDP data is transmitted over Ethernet as User Datagram Protocol (UDP) packets. _cdp-py_ contains a set of structural definitions of the CDP data items that make up these UDP packets.
-        
-        To get started with CDP, see the official [documentation](http://cuwb.io/docs/v3.3/software-integration/cdp-output-definition/). For more information regarding the individual data items, visit the [data items documentation](https://github.com/ciholas/cdp-py/blob/master/DATA_ITEMS.md).
-        
-        ## Getting Started
-        
-        ### Prerequisites
-        
-        You need Python 3 or higher to use _cdp-py_. Make sure you have Python installed and that the expected version is available from your command line. You can check this by running:
-        
-        ```
-        $ python --version
-        ```
-        
-        ### Installing
-        
-        _cdp-py_ can be installed using pip. To install the latest version use:
-        
-        ```
-        $ pip install cdp-py
-        ```
-        
-        Now that _cdp-py_ package is installed, you can start using the _cdp_ module by adding the following import statement to your Python script:
-        
-        ```python
-        import cdp
-        ```
-        For a tutorial about how to use the _cdp_ module, visit: [Using CDP - Python](http://cuwb.io/docs/v3.3/application-notes/using-cdp-python/#using-cdp-python).
-        
-        ### Upgrading
-        
-        To upgrade to the latest version use:
-        
-        ```
-        $ pip install --upgrade cdp-py
-        ```
-        
-        ## License
-        
-        This work is licensed under the [Creative Commons Attribution 4.0 International](http://creativecommons.org/licenses/by/4.0/) License.
-        
 Keywords: cdp ciholas data protocol
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+# cdp-py
+
+The Ciholas Data Protocol (CDP) provides a method of communication between devices and services. CDP data is transmitted over Ethernet as User Datagram Protocol (UDP) packets. _cdp-py_ contains a set of structural definitions of the CDP data items that make up these UDP packets.
+
+To get started with CDP, see the official [documentation](http://cuwb.io/docs/v3.3/software-integration/cdp-output-definition/). For more information regarding the individual data items, visit the [data items documentation](https://github.com/ciholas/cdp-py/blob/master/DATA_ITEMS.md).
+
+## Getting Started
+
+### Prerequisites
+
+You need Python 3 or higher to use _cdp-py_. Make sure you have Python installed and that the expected version is available from your command line. You can check this by running:
+
+```
+$ python --version
+```
+
+### Installing
+
+_cdp-py_ can be installed using pip. To install the latest version use:
+
+```
+$ pip install cdp-py
+```
+
+Now that _cdp-py_ package is installed, you can start using the _cdp_ module by adding the following import statement to your Python script:
+
+```python
+import cdp
+```
+For a tutorial about how to use the _cdp_ module, visit: [Using CDP - Python](http://cuwb.io/docs/v3.3/application-notes/using-cdp-python/#using-cdp-python).
+
+### Upgrading
+
+To upgrade to the latest version use:
+
+```
+$ pip install --upgrade cdp-py
+```
+
+## License
+
+This work is licensed under the [Creative Commons Attribution 4.0 International](http://creativecommons.org/licenses/by/4.0/) License.
```

### Comparing `cdp-py-1.5.0/cdp/cdp.py` & `cdp-py-1.6.1/cdp/cdp.py`

 * *Files identical despite different names*

### Comparing `cdp-py-1.5.0/cdp/data_items/data_items.py` & `cdp-py-1.6.1/cdp/data_items/data_items.py`

 * *Files 8% similar despite different names*

```diff
@@ -581,15 +581,15 @@
 class TemperatureV1(CDPDataItem):
     """CDP Data Item: Ciholas Data Protocol Temperature V1 Definition. Replaced by 0x012E in v3.2.
        This data type is used to report the temperature measured by an onboard LPS25H."""
 
     type = 0x012E
     definition = [DIUInt64Attr('network_time'), # The timestamp when the sensor recorded the data. This value is represented in Network Time, which is roughly 15.65 picoseconds per tick.
                   DIInt16Attr('temperature'), # The two's complement temperature value.
-                  DIUInt32Attr('scale')] # The full-scale representation in degrees Celsius.
+                  DIUInt16Attr('scale')] # The full-scale representation in degrees Celsius.
 
 
 class PositionV2(CDPDataItem):
     """CDP Data Item: Ciholas Data Protocol Position V2 Data Item Definition. Replaced by 0x013E in v3.2.
        This data type is used to report the 3 dimensional position of the reporting device."""
 
     type = 0x012F
@@ -746,41 +746,41 @@
                   DIUInt8Attr('battery_percentage'), # Percentage of battery charge left from 0-100. A value of 255 means no measurable battery is present.
                   DIInt8Attr('temperature'), # The two's complement temperature in degrees Celsius.
                   DIUInt8Attr('processor_usage'), # Percentage of processor usage from 0-100. A value of 255 represents an unknown value.
                   DIListAttr('error_patterns', ErrorPattern)]  # Array of current error states by their LED pattern.
 
 
 class AccelerometerV2(CDPDataItem):
-    """CDP Data Item: Ciholas Data Protocol Accelerometer V2 Data Item Definition. Current in v3.3.
+    """CDP Data Item: Ciholas Data Protocol Accelerometer V2 Data Item Definition. Replaced by 0x17A in v4.5.
        This data type is used to report the accelerometer data from an onboard MPU-9250."""
 
     type = 0x0139
     definition = [DISerialNumberAttr('serial_number'), # The serial number of the reporting device.
                   DIUInt64Attr('network_time'), # The timestamp when the sensor recorded the data. This value is represented in Network Time, which is roughly 15.65 picoseconds per tick.
                   DIInt32Attr('x'), # The two's complement X accelerometer value.
                   DIInt32Attr('y'), # The two's complement Y accelerometer value.
                   DIInt32Attr('z'), # The two's complement Z accelerometer value.
                   DIUInt8Attr('scale')] # The full-scale representation in Gs.
 
 
 class GyroscopeV2(CDPDataItem):
-    """CDP Data Item: Ciholas Data Protocol Gyroscope V2 Data Item Definition. Current in v3.3.
+    """CDP Data Item: Ciholas Data Protocol Gyroscope V2 Data Item Definition. Replaced by 0x17B in v4.5.
        This data type is used to report the gyroscope data from an onboard MPU-9250."""
 
     type = 0x013A
     definition = [DISerialNumberAttr('serial_number'), # The serial number of the reporting device.
                   DIUInt64Attr('network_time'), # The timestamp when the sensor recorded the data. This value is represented in Network Time, which is roughly 15.65 picoseconds per tick.
                   DIInt32Attr('x'), # The two's complement X gyroscope value.
                   DIInt32Attr('y'), # The two's complement Y gyroscope value.
                   DIInt32Attr('z'), # The two's complement Z gyroscope value.
                   DIUInt16Attr('scale')] # The full-scale representation in Degrees Per Second.
 
 
 class MagnetometerV2(CDPDataItem):
-    """CDP Data Item: Ciholas Data Protocol Magnetometer V2 Data Item Definition. Current in v3.3.
+    """CDP Data Item: Ciholas Data Protocol Magnetometer V2 Data Item Definition. Replaced by 0x17C in v4.5.
        This data type is used to report the magnetometer data from an onboard MPU-9250."""
 
     type = 0x013B
     definition = [DISerialNumberAttr('serial_number'), # The serial number of the reporting device.
                   DIUInt64Attr('network_time'), # The timestamp when the sensor recorded the data. This value is represented in Network Time, which is roughly 15.65 picoseconds per tick.
                   DIInt32Attr('x'), # The two's complement X magnetometer value.
                   DIInt32Attr('y'), # The two's complement Y magnetometer value.
@@ -1156,14 +1156,93 @@
                   DIUInt8Attr('poe_p2_pair_polarity_2'), # POE port 2 PR36 polarity. 0 = OPEN, 1 = NEGATIVE, 2 = POSITIVE.
                   DIUInt8Attr('poe_p2_pair_polarity_3'), # POE port 2 PR45 polarity. 0 = OPEN, 1 = NEGATIVE, 2 = POSITIVE.
                   DIUInt8Attr('poe_p2_pair_polarity_4'), # POE port 2 PR78 polarity. 0 = OPEN, 1 = NEGATIVE, 2 = POSITIVE.
                   DIUInt8Attr('poe_p1_source'), # Port 1 POE source. 0 = UNKNOWN, 1 = INJECTOR, 2 = PSE, 3 = INVALID.
                   DIUInt8Attr('poe_p2_source')] # Port 2 POE source. 0 = UNKNOWN, 1 = INJECTOR, 2 = PSE, 3 = INVALID.
 
 
+class ImageV2:
+    """Image Class V2 Definition. Public."""
+
+    definition = [DIUInt8Attr('image_type'), # The type of image this data represents.
+                  DIFixedLengthStrAttr('version', 32), # The version string of the image, null-terminated. If the string is less than the max (32B), it is padded with junk data.
+                  DIFixedLengthBytesAttr('sha1', 20), # The IVSHA1 of the image with a maximum size of 20B.
+                  DIUInt32Attr('image_length'), # The number of bytes the image contains.
+                  DIUInt16Attr('flags'), # Flags that can extend the meaning of this image information.
+                  DIVariableLengthBytesAttr('options')] # Additional information will be stored here, per the flags.
+
+    def __init__(self, type=0, version=0, sha1=0, image_length=0, flags=0, options=b'', data=None):
+        if data:
+            self._decode(data)
+        else:
+            self.image_type = type
+            self.version = version
+            self.sha1 = sha1
+            self.image_length = image_length
+            self.flags = flags
+            self.options = options
+
+    def __str__(self):
+        return "{}, {}, {}, {}, {}, {}".format(self.image_type, self.version, self.sha1.hex(), self.image_length, self.flags, self.options)
+
+    def _decode(self, data):
+        """Decodes a byte array as the ImageV2 object."""
+        for attr in ImageV2.definition:
+            value, size = attr._decode(data)
+            data = data[size:]
+            setattr(self, attr.name, value)
+
+class BoundingBoxReport(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol Bounding Box Report Data Item Definition. Public.
+       This data type is used to report the bounding box parameters."""
+
+    type = 0x016A
+    definition = [DIUInt32Attr('min_x'), # The minimum x-coordinate of the bounding zone in millimeters.
+                  DIUInt32Attr('min_y'), # The minimum y-coordinate of the bounding zone in millimeters.
+                  DIUInt32Attr('min_z'), # The minimum z-coordinate of the bounding zone in millimeters.
+                  DIUInt32Attr('max_x'), # The maximum x-coordinate of the bounding zone in millimeters.
+                  DIUInt32Attr('max_y'), # The maximum y-coordinate of the bounding zone in millimeters.
+                  DIUInt32Attr('max_z')] # The maximum z-coordinate of the bounding zone in millimeters.
+
+
+class BoundingCylinderReport(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol Bounding Cylinder Report Data Item Definition. Public.
+       This data type is used to report the bounding cylinder parameters."""
+
+    type = 0x016B
+    definition = [DIUInt32Attr('x'), # The x-coordinate of the bottom center of the cylinder in millimeters.
+                  DIUInt32Attr('y'), # The y-coordinate of the bottom center of the cylinder in millimeters.
+                  DIUInt32Attr('z'), # The z-coordinate of the bottom center of the cylinder in millimeters.
+                  DIUInt32Attr('radius'), # The radius of the cylinder in millimeters.
+                  DIUInt32Attr('height')] # The height of the cylinder in millimeters.
+
+
+class ImageDiscoveryV2(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol Image Discovery V2 Data Item Definition. Public.
+    This data type contains information to inform the CUWB Network about the images the device is currently running. The CUWB network will use this information to determine if the device needs a firmware upgrade."""
+
+    type = 0x0171
+    definition = [DIUInt8Attr('vid'), # Virtual Vendor ID for device images.
+                  DIUInt8Attr('pid'), # Virtual Product ID for device images.
+                  DIUInt8Attr('running_image_type'), # Type of the current running image.
+                  DIVariableLengthBytesAttr('tlvs')] # An array of TLV (Type Length Value) entries. Every entry will be prefixed with one byte for Type and one byte for Length.
+                                                     # 1 = Sector size (size 2 bytes). 2 = No Change Echo (size 0 bytes). 3 = Bootloading Timeout (size 1 byte). 4 = Image Information V2 (size varies).
+
+def ImageNotificationV2(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol Image Notification V2 Data Item Definition. Public.
+    This data type notifies a device or device group of what images the CUWB Network can upload to them."""
+
+    type = 0x0172
+    definition = [DIUInt8Attr('vid'), # Virtual Vendor ID for device images.
+                  DIUInt8Attr('pid'), # Virtual Product ID for device images.
+                  DIUInt8Attr('running_image_type'), # Type of the current running image.
+                  DIVariableLengthBytesAttr('tlvs')] # An array of TLV (Type Length Value) entries. Every entry will be prefixed with one byte for Type and one byte for Length.
+                                                     # 1 = Sector size (size 2 bytes). 2 = No Change Echo (size 0 bytes). 3 = Bootloading Timeout (size 1 byte). 4 = Image Information V2 (size varies).
+
+
 class Image:
     """Image Class Definition. Public."""
 
     definition = [DIUInt8Attr('type'),  # The type of image this data represents. 0 = Recover. 1 = Bootloader. 2 = Firmware. 3 = Almanac. 4 = Application.
                   DIFixedLengthStrAttr('version', 32),  # The version string of the image, null-terminated. If the string is less than the max (32B), it is padded with junk data.
                   DIFixedLengthBytesAttr('sha1', 20)]  # The IVSHA1 of the image with a maximum size of 20B.
 
@@ -1172,14 +1251,158 @@
         self.version = version
         self.sha1 = sha1
 
     def __str__(self):
         return "{}, {}, {}".format(self.type, self.version, self.sha1.hex())
 
 
+class PoeSystemStatsV2(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol POE MCU System Status V2 Data Item Definition. Protected.
+        This data type is used to report POE system status."""
+
+    type = 0x0173
+    definition = [DIUInt64Attr('last_power_outage'),  # Time since last power outage in ms.
+                  DIUInt64Attr('system_uptime'), # System uptime in ms.
+                  DIUInt32Attr('power_limit_in'), # Power limit of input in mW.
+                  DIUInt32Attr('power_limit_out'), # Power limit of output in mW.
+                  DIUInt32Attr('power_limit_local'), # Local power limit in mW.
+                  DIInt32Attr('p1_pair_voltage_1'), # Ethernet port 1 PR12 voltage in mV.
+                  DIInt32Attr('p1_pair_voltage_2'), # Ethernet port 1 PR36 voltage in mV.
+                  DIInt32Attr('p1_pair_voltage_3'), # Ethernet port 1 PR45 voltage in mV.
+                  DIInt32Attr('p1_pair_voltage_4'), # Ethernet port 1 PR78 voltage in mV.
+                  DIInt32Attr('p2_pair_voltage_1'), # Ethernet port 2 PR12 voltage in mV.
+                  DIInt32Attr('p2_pair_voltage_2'), # Ethernet port 2 PR36 voltage in mV.
+                  DIInt32Attr('p2_pair_voltage_3'), # Ethernet port 2 PR45 voltage in mV.
+                  DIInt32Attr('p2_pair_voltage_4'), # Ethernet port 2 PR78 voltage in mV.
+                  DIInt32Attr('p1_current'), # Ethernet port 1 current in uA.
+                  DIInt32Attr('p2_current'), # Ethernet port 2 current in uA.
+                  DIInt32Attr('local_current'), # Local current in uA.
+                  DIUInt16Attr('veth'), # Ethernet voltage in mV.
+                  DIUInt16Attr('power_outage_count'), # Number of power outages since boot.
+                  DIUInt8Attr('fets_status'), # Top and Bottom FET status formatted as a port mask. P2-PR78, P2-PR12, P1-PR78, P1-PR12, P2-PR45, P2-PR36, P1-PR45, P1-PR36.
+                  DIUInt8Attr('desired_class'), # Class requested by the device.
+                  DIUInt8Attr('granted_class'), # Class granted to the device.
+                  DIUInt8Attr('downstream_requested_class'), # Downstream requested class.
+                  DIUInt8Attr('downstream_granted_class'), # Downstream granted class.
+                  DIUInt8Attr('mps_mode'), # MPS mode. MPS mode. 0 = UNKNOWN, 1 = OFF, 2 = TYPE 1/2, 3 = TYPE 3/4 CLASS 1-4, 4 = TYPE 3/4 CLASS 5-8.
+                  DIUInt8Attr('state'), # State machine state.
+                  DIUInt8Attr('upstream_port'), # Port to treat as upstream.
+                  DIUInt8Attr('mps_active_last_log'), # Power measurement MPS state.
+                  DIUInt8Attr('poe_p1_mode'), # POE Port 1 mode. 0 = BOOT, 1 = OFF, 2 = INPUT, 3 = OUTPUT, 4 = CLASSIFYING.
+                  DIUInt8Attr('poe_p2_mode'), # POE Port 2 mode. 0 = BOOT, 1 = OFF, 2 = INPUT, 3 = OUTPUT, 4 = CLASSIFYING.
+                  DIUInt8Attr('poe_p1_pair_polarity_1'), # POE port 1 PR12 polarity. 0 = OPEN/NEGATIVE, 1 = POSITIVE.
+                  DIUInt8Attr('poe_p1_pair_polarity_2'), # POE port 1 PR36 polarity. 0 = OPEN/NEGATIVE, 1 = POSITIVE.
+                  DIUInt8Attr('poe_p1_pair_polarity_3'), # POE port 1 PR45 polarity. 0 = OPEN/NEGATIVE, 1 = POSITIVE.
+                  DIUInt8Attr('poe_p1_pair_polarity_4'), # POE port 1 PR78 polarity. 0 = OPEN/NEGATIVE, 1 = POSITIVE.
+                  DIUInt8Attr('poe_p2_pair_polarity_1'), # POE port 2 PR12 polarity. 0 = OPEN/NEGATIVE, 1 = POSITIVE.
+                  DIUInt8Attr('poe_p2_pair_polarity_2'), # POE port 2 PR36 polarity. 0 = OPEN/NEGATIVE, 1 = POSITIVE.
+                  DIUInt8Attr('poe_p2_pair_polarity_3'), # POE port 2 PR45 polarity. 0 = OPEN/NEGATIVE, 1 = POSITIVE.
+                  DIUInt8Attr('poe_p2_pair_polarity_4'), # POE port 2 PR78 polarity. 0 = OPEN/NEGATIVE, 1 = POSITIVE.
+                  DIUInt8Attr('poe_p1_source'), # Port 1 POE source. 0 = UNKNOWN, 1 = INJECTOR, 2 = PSE, 3 = PSE3+, 4 = INVALID.
+                  DIUInt8Attr('poe_p2_source')] # Port 2 POE source. 0 = UNKNOWN, 1 = INJECTOR, 2 = PSE, 3 = PSE3+, 4 = INVALID.
+
+
+class BoundaryStatus(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol Boundary Status Data Item Definition. Protected.
+        This data type is used to report boundary status of the system."""
+
+    type = 0x0176
+    definition = [DIUInt64Attr('network_time'),  # The timestamp when the sensor recorded the data. This value is represented in Network Time, which is roughly 15.65 picoseconds per tick.
+                 DIInt32Attr('x'),  # The signed x-coordinate in millimeters.
+                 DIInt32Attr('y'),  # The signed y-coordinate in millimeters.
+                 DIInt32Attr('z'),  # The signed z-coordinate in millimeters.
+                 DIUInt8Attr('status')]     # Current boundary status. 0 = NORMAL, 1 = WARNING, 2 = BREACHED.
+
+
+class PositionlessBoundaryStatus(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol Positionless Boundary Status Data Item Definition. Protected.
+        This data type is used to report positionless boundary status of the system."""
+
+    type = 0x0177
+    definition = [DIUInt64Attr('network_time'),  # The timestamp when the sensor recorded the data. This value is represented in Network Time, which is roughly 15.65 picoseconds per tick.
+                 DIUInt8Attr('status')]     # Current boundary status. 0 = NORMAL, 1 = WARNING, 2 = BREACHED.
+
+
+class QuaternionV3(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol Quaternion V3 Data Item Definition. Current in v4.0.
+       This data type is used to report quaternion data, either from on-chip sensors or other sources."""
+
+    type = 0x0178
+    definition = [DISerialNumberAttr('serial_number'), # The serial number of the reporting device.
+                  DIUInt64Attr('network_time'), # The timestamp when the sensor recorded the data. This value is represented in Network Time, which is roughly 15.65 picoseconds per tick.
+                  DIInt32Attr('x'), # The two's complement X quaternion value.
+                  DIInt32Attr('y'), # The two's complement Y quaternion value.
+                  DIInt32Attr('z'), # The two's complement Z quaternion value.
+                  DIInt32Attr('w'), # The two's complement W quaternion value.
+                  DIUInt8Attr('quaternion_type'), # An enumeration of all different types of quaternions. 0 = Using accelerometer and gyroscope not normalized. 1 = Using accelerometer and gyroscope normalized. 2 = Using accelerometer, gyroscope, and magnetometer normalized.  3 = Using phase data normalized.
+                  DIUInt16Attr('quality')] # The quality of the assessed quaternion from 0 to 10000.  If the quaternion is computed using an algorithm that does not support a quality calculation, then this value will be 0x4000.
+
+
+class UserDefinedV3(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol User Defined V3 Data Item Definition. Public.
+       This data type is used to report any user defined data bytes."""
+
+    type = 0x0179
+    definition = [DISerialNumberAttr('serial_number'),  # The serial number of the device sending the user-defined data.
+                  DIUInt64Attr('network_time'), # The network time of the user-defined data.
+                  DIVariableLengthBytesAttr('payload')]  # The format of the contents are defined by the user.
+
+
+class AccelerometerV3(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol Accelerometer V3 Data Item Definition. Current in v4.5.
+       This data type is used to report the accelerometer data from any accelerometer agnostic of chip placement."""
+
+    type = 0x017A
+    definition = [DISerialNumberAttr('serial_number'), # The serial number of the reporting device.
+                  DIUInt64Attr('network_time'), # The timestamp when the sensor recorded the data. This value is represented in Network Time, which is roughly 15.65 picoseconds per tick.
+                  DIInt32Attr('x'), # The two's complement X accelerometer value.
+                  DIInt32Attr('y'), # The two's complement Y accelerometer value.
+                  DIInt32Attr('z'), # The two's complement Z accelerometer value.
+                  DIUInt8Attr('scale')] # The full-scale representation in Gs.
+
+
+class GyroscopeV3(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol Gyroscope V2 Data Item Definition. Current in v4.5.
+       This data type is used to report the gyroscope data from any gyroscope agnostic of chip placement."""
+
+    type = 0x017B
+    definition = [DISerialNumberAttr('serial_number'), # The serial number of the reporting device.
+                  DIUInt64Attr('network_time'), # The timestamp when the sensor recorded the data. This value is represented in Network Time, which is roughly 15.65 picoseconds per tick.
+                  DIInt32Attr('x'), # The two's complement X gyroscope value.
+                  DIInt32Attr('y'), # The two's complement Y gyroscope value.
+                  DIInt32Attr('z'), # The two's complement Z gyroscope value.
+                  DIUInt16Attr('scale')] # The full-scale representation in Degrees Per Second.
+
+
+class MagnetometerV3(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol Magnetometer V3 Data Item Definition. Current in v4.5.
+       This data type is used to report the magnetometer data from any magnetometer agnostic of chip placement."""
+
+    type = 0x017C
+    definition = [DISerialNumberAttr('serial_number'), # The serial number of the reporting device.
+                  DIUInt64Attr('network_time'), # The timestamp when the sensor recorded the data. This value is represented in Network Time, which is roughly 15.65 picoseconds per tick.
+                  DIInt32Attr('x'), # The two's complement X magnetometer value.
+                  DIInt32Attr('y'), # The two's complement Y magnetometer value.
+                  DIInt32Attr('z'), # The two's complement Z magnetometer value.
+                  DIUInt16Attr('scale')] # The full-scale representation in microtesla.
+
+
+class CommandWindowUsageReport(CDPDataItem):
+    """CDP Data Item: Ciholas Data Protocol Command Window Usage Report Data Item Definition.  Protected.
+       This data type is used to report information related to the transmission of command packets. Includes info on the command windows as well."""
+    
+    type = 0x017D
+    definition = [DIFloatAttr('average_used_windows'),   # The average number of command windows that have a preallocated use at any given time.
+                  DIFloatAttr('average_reused_transmissions'),   # The average number of simultaneous transmissions occurring to support spatially reused transmissions. a value of 1.0 indicates that on average only 1 transmission is occurring per command window where a command is actually available.
+                  DIFloatAttr('average_bytes_per_packet'),   # The average number of bytes in transmitted command packets.
+                  DIFloatAttr('average_command_drops_per_second'),   # Average number of commands that have been dropped per second because no command windows were available.
+                  DIUInt16Attr('preschedule_size'),  # The maximum number of command windows that the network will preallocate a use for.
+                  DIUInt16Attr('current_used_preschedule_slots')] # The number of command windows that currently have a preallocated use.
+
+
 class ImageDiscoveryV1(CDPDataItem):
     """CDP Data Item: Ciholas Data Protocol Image Discovery V1 Data Item Definition. Public.
        This data type contains information to inform the CUWB Network about the images the device is currently running. The CUWB network will use this information to determine if the device needs a firmware upgrade."""
 
     type = 0x8009
     definition = [DIFixedLengthStrAttr('manufacturer', 64),  # The manufacturer in a null-terminated string format. If the string is less than the max (64B), it is padded with junk data.
                   DIFixedLengthStrAttr('product', 32),  # The product type in a null-terminated string format. If the string is less than the max (32B), it is padded with junk data.
```

### Comparing `cdp-py-1.5.0/cdp/data_items/__init__.py` & `cdp-py-1.6.1/cdp/data_items/__init__.py`

 * *Files identical despite different names*

### Comparing `cdp-py-1.5.0/setup.py` & `cdp-py-1.6.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import os
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+ver_string = os.environ['CI_COMMIT_TAG'][1:]
+
 setuptools.setup(
     name="cdp-py",
-    version="1.5.0",
+    version=ver_string,
     author="Ciholas, Inc.",
     author_email="cuwb.support@ciholas.com",
     description="Ciholas Data Protocol",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ciholas/cdp-py",
     license="CC BY 4.0",
```

### Comparing `cdp-py-1.5.0/README.md` & `cdp-py-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cdp-py-1.5.0/cdp_py.egg-info/PKG-INFO` & `cdp-py-1.6.1/cdp_py.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: cdp-py
-Version: 1.5.0
+Version: 1.6.1
 Summary: Ciholas Data Protocol
 Home-page: https://github.com/ciholas/cdp-py
 Author: Ciholas, Inc.
 Author-email: cuwb.support@ciholas.com
 License: CC BY 4.0
-Description: # cdp-py
-        
-        The Ciholas Data Protocol (CDP) provides a method of communication between devices and services. CDP data is transmitted over Ethernet as User Datagram Protocol (UDP) packets. _cdp-py_ contains a set of structural definitions of the CDP data items that make up these UDP packets.
-        
-        To get started with CDP, see the official [documentation](http://cuwb.io/docs/v3.3/software-integration/cdp-output-definition/). For more information regarding the individual data items, visit the [data items documentation](https://github.com/ciholas/cdp-py/blob/master/DATA_ITEMS.md).
-        
-        ## Getting Started
-        
-        ### Prerequisites
-        
-        You need Python 3 or higher to use _cdp-py_. Make sure you have Python installed and that the expected version is available from your command line. You can check this by running:
-        
-        ```
-        $ python --version
-        ```
-        
-        ### Installing
-        
-        _cdp-py_ can be installed using pip. To install the latest version use:
-        
-        ```
-        $ pip install cdp-py
-        ```
-        
-        Now that _cdp-py_ package is installed, you can start using the _cdp_ module by adding the following import statement to your Python script:
-        
-        ```python
-        import cdp
-        ```
-        For a tutorial about how to use the _cdp_ module, visit: [Using CDP - Python](http://cuwb.io/docs/v3.3/application-notes/using-cdp-python/#using-cdp-python).
-        
-        ### Upgrading
-        
-        To upgrade to the latest version use:
-        
-        ```
-        $ pip install --upgrade cdp-py
-        ```
-        
-        ## License
-        
-        This work is licensed under the [Creative Commons Attribution 4.0 International](http://creativecommons.org/licenses/by/4.0/) License.
-        
 Keywords: cdp ciholas data protocol
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+# cdp-py
+
+The Ciholas Data Protocol (CDP) provides a method of communication between devices and services. CDP data is transmitted over Ethernet as User Datagram Protocol (UDP) packets. _cdp-py_ contains a set of structural definitions of the CDP data items that make up these UDP packets.
+
+To get started with CDP, see the official [documentation](http://cuwb.io/docs/v3.3/software-integration/cdp-output-definition/). For more information regarding the individual data items, visit the [data items documentation](https://github.com/ciholas/cdp-py/blob/master/DATA_ITEMS.md).
+
+## Getting Started
+
+### Prerequisites
+
+You need Python 3 or higher to use _cdp-py_. Make sure you have Python installed and that the expected version is available from your command line. You can check this by running:
+
+```
+$ python --version
+```
+
+### Installing
+
+_cdp-py_ can be installed using pip. To install the latest version use:
+
+```
+$ pip install cdp-py
+```
+
+Now that _cdp-py_ package is installed, you can start using the _cdp_ module by adding the following import statement to your Python script:
+
+```python
+import cdp
+```
+For a tutorial about how to use the _cdp_ module, visit: [Using CDP - Python](http://cuwb.io/docs/v3.3/application-notes/using-cdp-python/#using-cdp-python).
+
+### Upgrading
+
+To upgrade to the latest version use:
+
+```
+$ pip install --upgrade cdp-py
+```
+
+## License
+
+This work is licensed under the [Creative Commons Attribution 4.0 International](http://creativecommons.org/licenses/by/4.0/) License.
```

