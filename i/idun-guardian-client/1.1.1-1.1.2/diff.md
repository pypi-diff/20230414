# Comparing `tmp/idun_guardian_client-1.1.1.tar.gz` & `tmp/idun_guardian_client-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idun_guardian_client-1.1.1.tar", last modified: Tue Apr 11 14:23:37 2023, max compression
+gzip compressed data, was "idun_guardian_client-1.1.2.tar", last modified: Fri Apr 14 12:02:51 2023, max compression
```

## Comparing `idun_guardian_client-1.1.1.tar` & `idun_guardian_client-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 14:23:37.118718 idun_guardian_client-1.1.1/
--rw-r--r--   0 waddaben   (501) staff       (20)     8991 2023-04-11 14:23:37.118496 idun_guardian_client-1.1.1/PKG-INFO
--rw-r--r--   0 waddaben   (501) staff       (20)     8426 2023-04-11 13:19:07.000000 idun_guardian_client-1.1.1/README.md
--rw-r--r--   0 waddaben   (501) staff       (20)      864 2023-04-11 13:19:07.000000 idun_guardian_client-1.1.1/pyproject.toml
--rw-r--r--   0 waddaben   (501) staff       (20)       38 2023-04-11 14:23:37.118768 idun_guardian_client-1.1.1/setup.cfg
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 14:23:37.112035 idun_guardian_client-1.1.1/src/
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 14:23:37.116237 idun_guardian_client-1.1.1/src/idun_guardian_client/
--rw-r--r--   0 waddaben   (501) staff       (20)      339 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.1/src/idun_guardian_client/__init__.py
--rw-r--r--   0 waddaben   (501) staff       (20)        0 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.1/src/idun_guardian_client/__main__.py
--rw-r--r--   0 waddaben   (501) staff       (20)     8661 2023-04-11 13:19:07.000000 idun_guardian_client-1.1.1/src/idun_guardian_client/client.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1797 2023-04-07 12:29:46.000000 idun_guardian_client-1.1.1/src/idun_guardian_client/config.py
--rw-r--r--   0 waddaben   (501) staff       (20)    11623 2023-04-11 13:19:07.000000 idun_guardian_client-1.1.1/src/idun_guardian_client/debug_logs.py
--rw-r--r--   0 waddaben   (501) staff       (20)    20783 2023-04-11 13:19:07.000000 idun_guardian_client-1.1.1/src/idun_guardian_client/igeb_api.py
--rw-r--r--   0 waddaben   (501) staff       (20)    30514 2023-04-11 13:35:16.000000 idun_guardian_client-1.1.1/src/idun_guardian_client/igeb_bluetooth.py
--rw-r--r--   0 waddaben   (501) staff       (20)     2846 2023-04-07 11:46:38.000000 idun_guardian_client-1.1.1/src/idun_guardian_client/igeb_utils.py
--rw-r--r--   0 waddaben   (501) staff       (20)      191 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.1/src/idun_guardian_client/mock_utils.py
--rw-r--r--   0 waddaben   (501) staff       (20)      164 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.1/src/idun_guardian_client/setup.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1214 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.1/src/idun_guardian_client/test_producer_consumer.py
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 14:23:37.117437 idun_guardian_client-1.1.1/src/idun_guardian_client.egg-info/
--rw-r--r--   0 waddaben   (501) staff       (20)     8991 2023-04-11 14:23:37.000000 idun_guardian_client-1.1.1/src/idun_guardian_client.egg-info/PKG-INFO
--rw-r--r--   0 waddaben   (501) staff       (20)      752 2023-04-11 14:23:37.000000 idun_guardian_client-1.1.1/src/idun_guardian_client.egg-info/SOURCES.txt
--rw-r--r--   0 waddaben   (501) staff       (20)        1 2023-04-11 14:23:37.000000 idun_guardian_client-1.1.1/src/idun_guardian_client.egg-info/dependency_links.txt
--rw-r--r--   0 waddaben   (501) staff       (20)      137 2023-04-11 14:23:37.000000 idun_guardian_client-1.1.1/src/idun_guardian_client.egg-info/requires.txt
--rw-r--r--   0 waddaben   (501) staff       (20)       21 2023-04-11 14:23:37.000000 idun_guardian_client-1.1.1/src/idun_guardian_client.egg-info/top_level.txt
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 14:23:37.118173 idun_guardian_client-1.1.1/tests/
--rw-r--r--   0 waddaben   (501) staff       (20)     1940 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.1/tests/test_ble.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1672 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.1/tests/test_ble_record.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1106 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.1/tests/test_utils.py
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-14 12:02:51.053560 idun_guardian_client-1.1.2/
+-rw-r--r--   0 waddaben   (501) staff       (20)     8991 2023-04-14 12:02:51.053375 idun_guardian_client-1.1.2/PKG-INFO
+-rw-r--r--   0 waddaben   (501) staff       (20)     8426 2023-04-11 13:19:07.000000 idun_guardian_client-1.1.2/README.md
+-rw-r--r--   0 waddaben   (501) staff       (20)      864 2023-04-14 12:01:14.000000 idun_guardian_client-1.1.2/pyproject.toml
+-rw-r--r--   0 waddaben   (501) staff       (20)       38 2023-04-14 12:02:51.053604 idun_guardian_client-1.1.2/setup.cfg
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-14 12:02:51.047223 idun_guardian_client-1.1.2/src/
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-14 12:02:51.051267 idun_guardian_client-1.1.2/src/idun_guardian_client/
+-rw-r--r--   0 waddaben   (501) staff       (20)      339 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/__init__.py
+-rw-r--r--   0 waddaben   (501) staff       (20)        0 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/__main__.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     8921 2023-04-14 12:01:14.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/client.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1797 2023-04-07 12:29:46.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/config.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    11765 2023-04-14 12:01:14.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/debug_logs.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    20723 2023-04-14 12:01:14.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/igeb_api.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    31141 2023-04-14 12:01:14.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/igeb_bluetooth.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     2846 2023-04-14 11:38:29.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/igeb_utils.py
+-rw-r--r--   0 waddaben   (501) staff       (20)      191 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/mock_utils.py
+-rw-r--r--   0 waddaben   (501) staff       (20)      164 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/setup.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1214 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/src/idun_guardian_client/test_producer_consumer.py
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-14 12:02:51.052429 idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/
+-rw-r--r--   0 waddaben   (501) staff       (20)     8991 2023-04-14 12:02:51.000000 idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/PKG-INFO
+-rw-r--r--   0 waddaben   (501) staff       (20)      752 2023-04-14 12:02:51.000000 idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/SOURCES.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)        1 2023-04-14 12:02:51.000000 idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/dependency_links.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)      137 2023-04-14 12:02:51.000000 idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/requires.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)       21 2023-04-14 12:02:51.000000 idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/top_level.txt
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-14 12:02:51.053109 idun_guardian_client-1.1.2/tests/
+-rw-r--r--   0 waddaben   (501) staff       (20)     1940 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/tests/test_ble.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1672 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/tests/test_ble_record.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1106 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.2/tests/test_utils.py
```

### Comparing `idun_guardian_client-1.1.1/PKG-INFO` & `idun_guardian_client-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idun_guardian_client
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
 Author-email: IDUN Technologies <contact@iduntechnologies.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `idun_guardian_client-1.1.1/README.md` & `idun_guardian_client-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.1/pyproject.toml` & `idun_guardian_client-1.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "idun_guardian_client"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="IDUN Technologies", email="contact@iduntechnologies.com" },
 ]
 description = "Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud"
 readme = "README.md"
 requires-python = ">=3.10"
 
@@ -21,15 +21,15 @@
     "Natural Language :: English",
 
 ]
 dependencies = [
 
   "asyncio ~= 3.4.3",
   "pycryptodome ~= 3.15.0",
-  "bleak ~= 0.18.1",
+  "bleak ~= 0.20.1",
   "python-dotenv ~= 0.21.0",
   "websockets ~= 10.3",
   "requests ~= 2.28.1",
   "numpy ~= 1.23.3",
   "pydantic ~= 1.10.2",
 ]
```

### Comparing `idun_guardian_client-1.1.1/src/idun_guardian_client/client.py` & `idun_guardian_client-1.1.2/src/idun_guardian_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import logging
 from datetime import datetime
 from .igeb_bluetooth import GuardianBLE
 from .igeb_api import GuardianAPI
 from .igeb_utils import check_platform, check_valid_mac, check_valid_uuid
 import uuid
 from typing import Union
+from bleak import exc
 
 
 class GuardianClient:
     """
     Class object for the communication between Guardian Earbuds and Cloud API
     """
 
@@ -152,52 +153,56 @@
             ValueError: If the recording timer is not valid
         """
         # set the timers
         self.guardian_api.runtime_receipt_timeout = sending_timout
         self.guardian_api.runtime_bi_directional_timeout = (
             bi_directional_receiving_timeout
         )
-
-        if self.debug:
-            logging.info(
-                "[CLIENT]: Recording timer set to: %s seconds", recording_timer
+        try:
+            if self.debug:
+                logging.info(
+                    "[CLIENT]: Recording timer set to: %s seconds", recording_timer
+                )
+                logging.info("[CLIENT]: Start recording")
+
+            print(f"[CLIENT]: Recording timer set to: {recording_timer} seconds")
+            print("-----Recording starting------")
+
+            data_queue: asyncio.Queue = asyncio.Queue(maxsize=86400)
+
+            recording_id = "py-" + str(
+                uuid.uuid4()
+            )  # the recordingID is a unique ID for each recording
+            logging.info("[CLIENT] Recording ID: %s", recording_id)
+            # log the experiment name in bold using the logging module
+            logging.info("[CLIENT] Experiment description: %s", experiment)
+            mac_id = await self.guardian_ble.get_device_mac()
+
+            tasks = []
+            tasks.append(
+                self.guardian_ble.run_ble_record(
+                    data_queue,
+                    recording_timer,
+                    mac_id,
+                    led_sleep,
+                    impedance_measurement,
+                    mains_freq_60hz,
+                )
+            )
+            tasks.append(
+                self.guardian_api.connect_ws_api(
+                    data_queue, mac_id, recording_id, impedance_measurement
+                )
             )
-            logging.info("[CLIENT]: Start recording")
-
-        print(f"[CLIENT]: Recording timer set to: {recording_timer} seconds")
-        print("-----Recording starting------")
 
-        data_queue: asyncio.Queue = asyncio.Queue(maxsize=86400)
+            await asyncio.wait(tasks)
 
-        recording_id = "py-" + str(
-            uuid.uuid4()
-        )  # the recordingID is a unique ID for each recording
-        logging.info("[CLIENT] Recording ID: %s", recording_id)
-        # log the experiment name in bold using the logging module
-        logging.info("[CLIENT] Experiment description: %s", experiment)
-        mac_id = await self.guardian_ble.get_device_mac()
-
-        tasks = []
-        tasks.append(
-            self.guardian_ble.run_ble_record(
-                data_queue,
-                recording_timer,
-                mac_id,
-                led_sleep,
-                impedance_measurement,
-                mains_freq_60hz,
-            )
-        )
-        tasks.append(
-            self.guardian_api.connect_ws_api(
-                data_queue, mac_id, recording_id, impedance_measurement
-            )
-        )
+        except exc.BleakError as err:
+            logging.error("[CLIENT]: BLE error: %s", err)
 
-        await asyncio.wait(tasks)
         if self.debug:
             logging.info("[CLIENT]: -----------  All tasks are COMPLETED -----------")
         print(f"-----Recording ID {recording_id}------")
         print(f"-----Device ID {mac_id}------")
         print("-----Recording stopped------")
 
     def stop_recording(self):
```

### Comparing `idun_guardian_client-1.1.1/src/idun_guardian_client/config.py` & `idun_guardian_client-1.1.2/src/idun_guardian_client/config.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.1/src/idun_guardian_client/debug_logs.py` & `idun_guardian_client-1.1.2/src/idun_guardian_client/debug_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """
 This module contains the functions that are used to log the debug messages.
 """
 import logging
 import time
 
 
+def log_device_not_connected_cannot_stop(debug):
+    if debug:
+        logging.info("[API]: Device not connected, cannot stop")
+
+
 def log_first_message(data_model, package_receipt, debug):
     if debug:
         logging.info("[API]: First package sent")
         logging.info(
             "[API]: data_model.stop = %s",
             data_model.stop,
         )
@@ -135,20 +140,17 @@
         logging.info("[API]: Interruption in connecting to the cloud: %s", error)
         logging.info(
             "Cannot connect to API endpoint. Please check the URL and try again."
         )
         logging.info("Retrying connection in {} seconds".format(retry_time))
 
 
-def logging_cancelled_error(error, debug):
+def logging_cancelled_error(debug):
     if debug:
-        logging.info(
-            "[API]: Error in sending data to the cloud: %s",
-            error,
-        )
+        logging.info("[API]: Error in sending data to the cloud: %s")
         logging.info("[API]: Re-establishing cloud connection in exeption")
         logging.info("[API]: Fetching last package from queue")
 
 
 def logging_connecting_to_cloud(debug):
     if debug:
         logging.info("[API]: Connecting to cloud...")
@@ -176,17 +178,19 @@
 
 def logging_device_info(debug, mac_address, firmware_decoded):
     if debug:
         logging.info("[BLE] Device ID (based on MAC address is): %s", mac_address)
         logging.info("[BLE]: Firmware version: %s", firmware_decoded)
 
 
-def logging_device_not_found(debug):
+def logging_device_not_found(debug, break_time):
     if debug:
-        logging.info("[BLE]: No IGEB device found, exiting ..")
+        logging.info(
+            f"[BLE]: No IGEB device found, trying again in {break_time} seconds"
+        )
 
 
 def logging_device_found(debug, ble_device_list):
     if debug:
         logging.info(
             "[BLE]: One IGEB device found, assinging address %s", ble_device_list[0]
         )
```

### Comparing `idun_guardian_client-1.1.1/src/idun_guardian_client/igeb_api.py` & `idun_guardian_client-1.1.2/src/idun_guardian_client/igeb_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,34 +244,34 @@
 
         def on_connection_initialise_variables():
             self.first_message_check = True
             self.connected = True
             self.bi_directional_timeout = self.initial_bi_directional_timeout
             self.current_timeout = self.initial_receipt_timeout
 
-        async def handle_cancelled_error(error):
+        async def handle_cancelled_error():
             while True:
                 try:
                     async with websockets.connect(  # type: ignore
                         settings.WS_IDENTIFIER
                     ) as self.websocket:
-                        logging_cancelled_error(error, self.debug)
+                        logging_cancelled_error(self.debug)
                         await unpack_and_load_data_termination()
                         await self.websocket.send(json.dumps(asdict(self.data_model)))
                         package_receipt = await self.websocket.recv()
                         log_final_message(
                             self.data_model,
                             package_receipt,
                             self.debug,
                         )
                         self.final_message_sent = True
                         break
-                except Exception as error:
+                except Exception as err:
                     await asyncio.sleep(self.ping_timeout)
-                    log_error_in_sending_stop(error, self.debug)
+                    log_error_in_sending_stop(err, self.debug)
                     continue
 
         once_initialise_variables()
 
         while True:
             logging_connecting_to_cloud(self.debug)
             try:
@@ -292,32 +292,32 @@
                             self.connected = False
                             await asyncio.shield(asyncio.sleep(self.ping_timeout))
                             logging_reconnection(self.debug)
                             self.bi_directional_timeout = (
                                 self.initial_bi_directional_timeout
                             )
                             continue
-                        except asyncio.CancelledError as error:
-                            await handle_cancelled_error(error)
+                        except asyncio.CancelledError:
+                            await handle_cancelled_error()
 
-                    except (asyncio.TimeoutError) as error:
+                    except asyncio.TimeoutError as error:
                         try:
                             log_interrupt_error(error, self.debug)
                             self.connected = False
                             await asyncio.shield(asyncio.sleep(self.ping_timeout))
                             logging_reconnection(self.debug)
                             self.bi_directional_timeout = (
                                 self.initial_bi_directional_timeout
                             )
                             continue
-                        except asyncio.CancelledError as error:
-                            await handle_cancelled_error(error)
+                        except asyncio.CancelledError:
+                            await handle_cancelled_error()
 
-                    except asyncio.CancelledError as error:
-                        await handle_cancelled_error(error)
+                    except asyncio.CancelledError:
+                        await handle_cancelled_error()
 
                     finally:
                         # Otherwise new tasks will be created which is a problem
                         try:
                             if not send_task.done():
                                 send_task.cancel()
                             if not receive_task.done():
```

### Comparing `idun_guardian_client-1.1.1/src/idun_guardian_client/igeb_bluetooth.py` & `idun_guardian_client-1.1.2/src/idun_guardian_client/igeb_bluetooth.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import base64
 import datetime
 from bleak import BleakClient, BleakScanner, exc
 
 from .config import settings
 from .debug_logs import *
 
+SEARCH_BREAK = 3
+
 
 class GuardianBLE:
     """Main Guardian BLE client."""
 
     def __init__(self, address: str = "", debug: bool = True) -> None:
         """Initialize the Guardian BLE client.
 
@@ -141,30 +143,36 @@
         it asks the user to select the device. If one device is found, it returns the
         address of the device.
 
         Returns:
             _type_: _description_
         """
 
-        ble_device_list = await self.get_ble_devices()
+        while True:
+
+            ble_device_list = await self.get_ble_devices()
+            if len(ble_device_list) == 0:
+                logging_device_not_found(self.debug, SEARCH_BREAK)
+                await asyncio.sleep(SEARCH_BREAK)
+
+            elif len(ble_device_list) == 1:
+                logging_device_found(self.debug, ble_device_list)
+                self.address = ble_device_list[0]
+                break
+            else:
+                index_str = input(
+                    "Enter the index of the GDK device you want to connect to \
+                    \nIf cannot find the device, please restart the program and try again: "
+                )
+                index = int(index_str)
+                self.address = ble_device_list[index]
+                break
 
-        if len(ble_device_list) == 0:
-            logging_device_not_found(self.debug)
-            self.exit_system()
-        elif len(ble_device_list) == 1:
-            logging_device_found(self.debug, ble_device_list)
-            self.address = ble_device_list[0]
-        else:
-            index_str = input(
-                "Enter the index of the GDK device you want to connect to \
-                \nIf cannot find the device, please restart the program and try again: "
-            )
-            index = int(index_str)
-            self.address = ble_device_list[index]
         logging_device_address(self.debug, self.address)
+
         return self.address
 
     def exit_system(self) -> None:
         """Exit the system."""
         try:
             sys.exit(0)
         except SystemExit:
@@ -468,17 +476,20 @@
             await asyncio.sleep(
                 self.sent_final_package_time
             )  # Give API time to send last package
             # With its own interupt handling
             # ------------------ Send stop EEG recording command ------------------
             logging_sending_stop_device(self.debug)
             await asyncio.sleep(self.ble_delay)
-            await self.client.write_gatt_char(
-                self.command_id, utf_8_encode(self.stop_imp_cmd)[0]
-            )
+            try:
+                await self.client.write_gatt_char(
+                    self.command_id, utf_8_encode(self.stop_imp_cmd)[0]
+                )
+            except AttributeError:
+                log_device_not_connected_cannot_stop(self.debug)
 
             # ------------------ Disconnecting commands ------------------
             logging_sending_disconnect(self.debug)
             await asyncio.sleep(self.ble_stop_delay)
             await self.client.disconnect()
             await asyncio.sleep(self.ble_stop_delay)
             # ------------------ Closing file  ------------------
@@ -501,17 +512,21 @@
             await asyncio.sleep(
                 self.sent_final_package_time
             )  # Give API time to send last package
             # With its own interupt handling
             # ------------------ Send stop EEG recording command ------------------
             logging_sending_stop_device(self.debug)
             await asyncio.sleep(self.ble_delay)
-            await self.client.write_gatt_char(
-                self.command_id, utf_8_encode(self.stop_cmd)[0]
-            )
+            try:
+                await self.client.write_gatt_char(
+                    self.command_id, utf_8_encode(self.stop_cmd)[0]
+                )
+            except AttributeError:
+                log_device_not_connected_cannot_stop(self.debug)
+
             # ------------------ Configuring LED back on ------------------
             if led_sleep:
                 logging_turn_led_on(self.debug)
                 await asyncio.sleep(self.ble_delay)
                 await self.client.write_gatt_char(
                     self.cfg_id, utf_8_encode(self.led_on_cfg)[0]
                 )
@@ -709,36 +724,40 @@
 
         except exc.BleakError as err:
             logging_device_connection_failed(self.debug, err)
 
     async def read_battery_level(self) -> None:
         """Read the battery level of the device given pre-defined interval."""
         logging_reading_battery_level(self.debug)
-
-        async with BleakClient(self.address) as client:
-            logging_device_connected_general(self.debug)
-
+        while True:
             try:
-                await asyncio.sleep(self.ble_delay)
-                value = int.from_bytes(
-                    (await client.read_gatt_char(self.battery_id)), byteorder="little"
-                )
-                print("-----------------------------")
-                print(f"\nBattery level: {value}%\n")
-                print("-----------------------------")
-                logging_batterylevel_int(self.debug, value)
+                async with BleakClient(self.address) as client:
+                    logging_device_connected_general(self.debug)
 
-                await asyncio.sleep(self.ble_stop_delay)
-                await client.disconnect()
-                await asyncio.sleep(self.ble_stop_delay)
-                logging_sending_disconnect(self.debug)
+                    await asyncio.sleep(self.ble_delay)
+                    value = int.from_bytes(
+                        (await client.read_gatt_char(self.battery_id)),
+                        byteorder="little",
+                    )
+                    print("-----------------------------")
+                    print(f"\nBattery level: {value}%\n")
+                    print("-----------------------------")
+                    logging_batterylevel_int(self.debug, value)
+
+                    await asyncio.sleep(self.ble_stop_delay)
+                    await client.disconnect()
+                    await asyncio.sleep(self.ble_stop_delay)
+                    logging_sending_disconnect(self.debug)
+                    break
 
             except exc.BleakError as err:
                 # log the error
                 logging_device_connection_failed(self.debug, err)
+                await asyncio.sleep(3)
+                continue
 
     async def get_device_information(self) -> dict:
         """Read the device information of the device."""
 
         device_info = {}
 
         async with BleakClient(self.address) as client:
```

### Comparing `idun_guardian_client-1.1.1/src/idun_guardian_client/igeb_utils.py` & `idun_guardian_client-1.1.2/src/idun_guardian_client/igeb_utils.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.1/src/idun_guardian_client/test_producer_consumer.py` & `idun_guardian_client-1.1.2/src/idun_guardian_client/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.1/src/idun_guardian_client.egg-info/PKG-INFO` & `idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idun-guardian-client
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
 Author-email: IDUN Technologies <contact@iduntechnologies.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `idun_guardian_client-1.1.1/src/idun_guardian_client.egg-info/SOURCES.txt` & `idun_guardian_client-1.1.2/src/idun_guardian_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.1/tests/test_ble.py` & `idun_guardian_client-1.1.2/tests/test_ble.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.1/tests/test_ble_record.py` & `idun_guardian_client-1.1.2/tests/test_ble_record.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.1/tests/test_utils.py` & `idun_guardian_client-1.1.2/tests/test_utils.py`

 * *Files identical despite different names*

