# Comparing `tmp/pyblhost-1.3.0.tar.gz` & `tmp/pyblhost-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblhost-1.3.0.tar", last modified: Thu Feb  2 08:23:27 2023, max compression
+gzip compressed data, was "pyblhost-1.4.0.tar", last modified: Fri Apr 14 16:06:54 2023, max compression
```

## Comparing `pyblhost-1.3.0.tar` & `pyblhost-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 08:23:27.475914 pyblhost-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-02-02 08:23:22.000000 pyblhost-1.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-02-02 08:23:22.000000 pyblhost-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-02-02 08:23:22.000000 pyblhost-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4296 2023-02-02 08:23:27.475914 pyblhost-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-02-02 08:23:22.000000 pyblhost-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 08:23:27.475914 pyblhost-1.3.0/pyblhost/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-02-02 08:23:22.000000 pyblhost-1.3.0/pyblhost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-02-02 08:23:22.000000 pyblhost-1.3.0/pyblhost/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-02 08:23:22.000000 pyblhost-1.3.0/pyblhost/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    40782 2023-02-02 08:23:22.000000 pyblhost-1.3.0/pyblhost/pyblhost.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-02 08:23:27.475914 pyblhost-1.3.0/pyblhost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4296 2023-02-02 08:23:27.000000 pyblhost-1.3.0/pyblhost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      353 2023-02-02 08:23:27.000000 pyblhost-1.3.0/pyblhost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-02 08:23:27.000000 pyblhost-1.3.0/pyblhost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-02-02 08:23:27.000000 pyblhost-1.3.0/pyblhost.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-02 08:23:27.000000 pyblhost-1.3.0/pyblhost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-02-02 08:23:27.000000 pyblhost-1.3.0/pyblhost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-02-02 08:23:22.000000 pyblhost-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-02 08:23:22.000000 pyblhost-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-02 08:23:27.475914 pyblhost-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-02-02 08:23:22.000000 pyblhost-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:06:54.824110 pyblhost-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-14 16:06:50.000000 pyblhost-1.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-14 16:06:50.000000 pyblhost-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-14 16:06:50.000000 pyblhost-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4296 2023-04-14 16:06:54.824110 pyblhost-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3740 2023-04-14 16:06:50.000000 pyblhost-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:06:54.824110 pyblhost-1.4.0/pyblhost/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-14 16:06:50.000000 pyblhost-1.4.0/pyblhost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-04-14 16:06:50.000000 pyblhost-1.4.0/pyblhost/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 16:06:50.000000 pyblhost-1.4.0/pyblhost/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    40994 2023-04-14 16:06:50.000000 pyblhost-1.4.0/pyblhost/pyblhost.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:06:54.824110 pyblhost-1.4.0/pyblhost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4296 2023-04-14 16:06:54.000000 pyblhost-1.4.0/pyblhost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      353 2023-04-14 16:06:54.000000 pyblhost-1.4.0/pyblhost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 16:06:54.000000 pyblhost-1.4.0/pyblhost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-04-14 16:06:54.000000 pyblhost-1.4.0/pyblhost.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-14 16:06:54.000000 pyblhost-1.4.0/pyblhost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-14 16:06:54.000000 pyblhost-1.4.0/pyblhost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-04-14 16:06:50.000000 pyblhost-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-14 16:06:50.000000 pyblhost-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-14 16:06:54.824110 pyblhost-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-04-14 16:06:50.000000 pyblhost-1.4.0/setup.py
```

### Comparing `pyblhost-1.3.0/LICENSE` & `pyblhost-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyblhost-1.3.0/PKG-INFO` & `pyblhost-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblhost
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python implementation of blhost used to communicate with the NXP MCUBOOT/KBOOT bootloader
 Home-page: https://github.com/Lauszus/pyblhost
 Author: Kristian Sloth Lauszus
 Author-email: lauszus@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pyblhost-1.3.0/README.md` & `pyblhost-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyblhost-1.3.0/pyblhost/__init__.py` & `pyblhost-1.4.0/pyblhost/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 #
 # Contact information
 # -------------------
 # Kristian Sloth Lauszus
 # Web      :  https://www.lauszus.com
 # e-mail   :  lauszus@gmail.com
 
-__version__ = '1.3.0'
+__version__ = '1.4.0'
 
 __all__ = ['BlhostCan', 'BlhostSerial']
 
 from .pyblhost import BlhostCan, BlhostSerial
```

### Comparing `pyblhost-1.3.0/pyblhost/__main__.py` & `pyblhost-1.4.0/pyblhost/__main__.py`

 * *Files identical despite different names*

### Comparing `pyblhost-1.3.0/pyblhost/pyblhost.py` & `pyblhost-1.4.0/pyblhost/pyblhost.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         for _ in range(attempts):
             try:
                 # Yield a progress while uploading and store the return value
                 upload_result = yield from self._upload(binary_data, start_address, erase_byte_count, timeout, ping_repeat)
 
                 # We need to clear the backup region if uploading fails.
                 if not upload_result:
-                    self.logger.info('BlhostBase: Uploading failed. Erasing flash region: 0x{:X} -> 0x{:X}'.format(
+                    self.logger.error('BlhostBase: Uploading failed. Erasing flash region: 0x{:X} -> 0x{:X}'.format(
                         start_address, start_address + erase_byte_count))
                     self._flash_erase_region_response_event.clear()
                     self._flash_erase_region(start_address, erase_byte_count)
                     if not self._flash_erase_region_response_event.wait(timeout):
                         self.logger.error('BlhostBase: Timed out waiting for flash erase region response after the upload failed')
             finally:
                 # Make sure the target is always reset
@@ -302,14 +302,15 @@
 
         if self._write_memory_response_event.wait(timeout):
             # "The target returns a GenericResponse packet with a status code set to
             # kStatus_Success upon successful execution of the command, or to an appropriate error
             # status code."
             return True
 
+        self.logger.warning('BlhostBase: Timed out waiting for write memory response')
         return False
 
     def _ack(self):
         data = [self.FramingPacketConstants.StartByte, self.FramingPacketConstants.Type_Ack]
         self._send(data)
 
     @staticmethod
@@ -535,15 +536,15 @@
             self._data_event.set()
         elif data[1] == self.FramingPacketConstants.Type_PingResponse:
             self._ping_response_event.set()
 
             protocol_bugfix, protocol_minor, protocol_major, protocol_name, options = struct.Struct('<BBBBH').unpack(data[2:8])
             protocol_version = '{}{}.{}.{}'.format(chr(protocol_name), protocol_major, protocol_minor, protocol_bugfix)
             self.logger.info('BlhostBase: Ping response: version: {}, options: {}'.format(protocol_version, options))
-            if protocol_version != 'P1.2.0':
+            if protocol_version not in ['P1.2.0', 'P1.3.0']:
                 self.logger.error('BlhostBase: Unsupported protocol version: {}'.format(protocol_version))
         else:
             self.logger.info('BlhostBase: Unhandled command type: {}'.format(data[1]))
 
 
 class BlhostDataParser(object):
 
@@ -562,14 +563,15 @@
         :return: Returns the parsed data when the messages has been parsed.
         """
         # Append the incoming data to the buffer
         self._data += data
 
         # The packet type will always start with the start byte
         while len(self._data) > 0 and self._data[0] != BlhostBase.FramingPacketConstants.StartByte:
+            self._logger.warning('BootloaderDataParser: Discarding invalid data: {}'.format(self._data[0]))
             self._data = self._data[1:]  # Discard the fist byte
 
         if len(self._data) < 2:
             # We need more data before we can determine the type and what to do with it
             return None
 
         if self._data[1] in [BlhostBase.FramingPacketConstants.Type_Ack,
```

### Comparing `pyblhost-1.3.0/pyblhost.egg-info/PKG-INFO` & `pyblhost-1.4.0/pyblhost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblhost
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python implementation of blhost used to communicate with the NXP MCUBOOT/KBOOT bootloader
 Home-page: https://github.com/Lauszus/pyblhost
 Author: Kristian Sloth Lauszus
 Author-email: lauszus@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pyblhost-1.3.0/setup.py` & `pyblhost-1.4.0/setup.py`

 * *Files identical despite different names*

