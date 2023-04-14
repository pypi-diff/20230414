# Comparing `tmp/python_ember_mug-0.6.0b9.tar.gz` & `tmp/python_ember_mug-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ember_mug-0.6.0b9.tar", max compression
+gzip compressed data, was "python_ember_mug-0.6.1.tar", max compression
```

## Comparing `python_ember_mug-0.6.0b9.tar` & `python_ember_mug-0.6.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-02-18 15:31:48.049208 python_ember_mug-0.6.0b9/LICENSE
--rw-r--r--   0        0        0     5012 2023-02-18 15:31:48.049208 python_ember_mug-0.6.0b9/README.md
--rwxr-xr-x   0        0        0      189 2023-02-18 15:31:48.049208 python_ember_mug-0.6.0b9/ember_mug/__init__.py
--rw-r--r--   0        0        0      106 2023-02-18 15:31:48.049208 python_ember_mug-0.6.0b9/ember_mug/__main__.py
--rw-r--r--   0        0        0      296 2023-02-18 15:31:48.049208 python_ember_mug-0.6.0b9/ember_mug/cli/__init__.py
--rw-r--r--   0        0        0     7736 2023-02-18 15:31:48.049208 python_ember_mug-0.6.0b9/ember_mug/cli/commands.py
--rw-r--r--   0        0        0     2910 2023-02-18 15:31:48.049208 python_ember_mug-0.6.0b9/ember_mug/cli/helpers.py
--rw-r--r--   0        0        0     4818 2023-02-18 15:31:48.049208 python_ember_mug-0.6.0b9/ember_mug/consts.py
--rw-r--r--   0        0        0     6264 2023-02-18 15:31:48.049208 python_ember_mug-0.6.0b9/ember_mug/data.py
--rw-r--r--   0        0        0      605 2023-02-18 15:31:48.049208 python_ember_mug-0.6.0b9/ember_mug/formatting.py
--rw-r--r--   0        0        0    17666 2023-02-18 15:31:48.049208 python_ember_mug-0.6.0b9/ember_mug/mug.py
--rw-r--r--   0        0        0     2090 2023-02-18 15:31:48.049208 python_ember_mug-0.6.0b9/ember_mug/scanner.py
--rw-r--r--   0        0        0     1352 2023-02-18 15:31:48.049208 python_ember_mug-0.6.0b9/ember_mug/utils.py
--rw-r--r--   0        0        0     2852 2023-02-18 15:31:48.053208 python_ember_mug-0.6.0b9/pyproject.toml
--rw-r--r--   0        0        0       46 2023-02-18 15:31:48.053208 python_ember_mug-0.6.0b9/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-18 15:31:48.053208 python_ember_mug-0.6.0b9/tests/cli/__init__.py
--rw-r--r--   0        0        0     7758 2023-02-18 15:31:48.053208 python_ember_mug-0.6.0b9/tests/cli/test_commands.py
--rw-r--r--   0        0        0     2645 2023-02-18 15:31:48.053208 python_ember_mug-0.6.0b9/tests/cli/test_helpers.py
--rw-r--r--   0        0        0     1117 2023-02-18 15:31:48.053208 python_ember_mug-0.6.0b9/tests/conftest.py
--rw-r--r--   0        0        0    19112 2023-02-18 15:31:48.053208 python_ember_mug-0.6.0b9/tests/test_connection.py
--rw-r--r--   0        0        0      776 2023-02-18 15:31:48.053208 python_ember_mug-0.6.0b9/tests/test_consts.py
--rw-r--r--   0        0        0     1299 2023-02-18 15:31:48.053208 python_ember_mug-0.6.0b9/tests/test_data.py
--rw-r--r--   0        0        0      534 2023-02-18 15:31:48.053208 python_ember_mug-0.6.0b9/tests/test_formatting.py
--rw-r--r--   0        0        0     3294 2023-02-18 15:31:48.053208 python_ember_mug-0.6.0b9/tests/test_mug_data.py
--rw-r--r--   0        0        0     1972 2023-02-18 15:31:48.053208 python_ember_mug-0.6.0b9/tests/test_scanner.py
--rw-r--r--   0        0        0      801 2023-02-18 15:31:48.053208 python_ember_mug-0.6.0b9/tests/test_utils.py
--rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 python_ember_mug-0.6.0b9/setup.py
--rw-r--r--   0        0        0     6220 1970-01-01 00:00:00.000000 python_ember_mug-0.6.0b9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/LICENSE
+-rw-r--r--   0        0        0     5219 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/README.md
+-rwxr-xr-x   0        0        0      187 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/__init__.py
+-rw-r--r--   0        0        0      106 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/__main__.py
+-rw-r--r--   0        0        0      296 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/cli/__init__.py
+-rw-r--r--   0        0        0     8471 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/cli/commands.py
+-rw-r--r--   0        0        0     2910 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/cli/helpers.py
+-rw-r--r--   0        0        0     4698 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/consts.py
+-rw-r--r--   0        0        0     6264 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/data.py
+-rw-r--r--   0        0        0      605 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/formatting.py
+-rw-r--r--   0        0        0    17156 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/mug.py
+-rw-r--r--   0        0        0     2112 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/scanner.py
+-rw-r--r--   0        0        0     1963 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/utils.py
+-rw-r--r--   0        0        0     2894 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/cli/__init__.py
+-rw-r--r--   0        0        0     7832 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/cli/test_commands.py
+-rw-r--r--   0        0        0     2645 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/cli/test_helpers.py
+-rw-r--r--   0        0        0     1156 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/conftest.py
+-rw-r--r--   0        0        0    19148 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_connection.py
+-rw-r--r--   0        0        0      776 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_consts.py
+-rw-r--r--   0        0        0     1299 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_data.py
+-rw-r--r--   0        0        0      534 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_formatting.py
+-rw-r--r--   0        0        0     3294 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_mug_data.py
+-rw-r--r--   0        0        0     2012 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_scanner.py
+-rw-r--r--   0        0        0      801 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_utils.py
+-rw-r--r--   0        0        0     6425 1970-01-01 00:00:00.000000 python_ember_mug-0.6.1/PKG-INFO
```

### Comparing `python_ember_mug-0.6.0b9/LICENSE` & `python_ember_mug-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.0b9/README.md` & `python_ember_mug-0.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 
 ## Summary
 
 This is an *unofficial* library to attempt to interact with Ember Mugs via Bluetooth.
 This was created for use with my [Home Assistant integration](https://github.com/sopelj/hass-ember-mug-component),
 but could be useful separately and has a simple CLI interface too.
 
-**Note**: Should work with the standard Ember Mugs (1 and 2), but the thermoses have not been tested.
+**Note**: Works with the standard Ember Mug (1 and 2). The Cup and Thermos may work, but have not been tested.
 
 ## Features
 
-* Finding mugs
-* Connecting to Mugs
+* Finding devices
+* Connecting to devices
 * Reading Information (Colour, temp, liquid level, etc.)
 * Writing (Desired temp, colour, temperature unit)*
 * Polling for changes
 
-*** Writing only works if the mug has been set up in the app previously
+*** Writing only works if the devices has been set up in the app previously
 
 ## Usage
 
 ### Python
 
 ```python
 from ember_mug.scanner import find_mug, discover_mugs
@@ -41,18 +41,24 @@
 
 # if first time with mug in pairing
 mugs = await discover_mugs()
 device = mugs[0]
 # after paired you can simply use
 device = await find_mug()
 mug = EmberMug(device)
-async with mug.connection() as con:
+await mug.update_all()
+print(mug.data.formatted)
+await mug.disconnect()
+
+# You can also use connection as a context manager
+# if you want to ensure connection before starting and cleanup on exit
+async with mug.connection():
     print('Connected.\nFetching Info')
-    await con.update_all()
-    print(mug.formatted_data)
+    await mug.update_all()
+    print(mug.data.formatted)
 ```
 
 ### CLI
 
 It can also be run via command line either directly with `ember-mug --help` or as a module with `python -m ember_mug --help`
 There are four options with different subsections. You can see them by specifying them before help. eg `ember-mug poll --help`
```

### Comparing `python_ember_mug-0.6.0b9/ember_mug/cli/commands.py` & `python_ember_mug-0.6.1/ember_mug/cli/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """CLI Interface."""
 from __future__ import annotations
 
 import asyncio
 import contextlib
+import logging
 import platform
 import re
 import sys
-from argparse import ArgumentParser, ArgumentTypeError, Namespace
+from argparse import ArgumentParser, ArgumentTypeError, FileType, Namespace
 from typing import TYPE_CHECKING
 
 from bleak import BleakError
 
 from ..consts import ATTR_LABELS, EXTRA_ATTRS
 from ..data import Colour
 from ..mug import EmberMug
@@ -23,15 +24,15 @@
 all_attrs = list(ATTR_LABELS) + list(EXTRA_ATTRS)
 get_attribute_names = [n.replace('_', '-') for n in all_attrs]
 
 
 async def get_mug(args: Namespace) -> EmberMug:
     """Helper to get the mug based on args."""
     device = await find_device(args)
-    mug = EmberMug(device, use_metric=not args.imperial, include_extra=args.extra)
+    mug = EmberMug(device, use_metric=not args.imperial, include_extra=args.extra, debug=args.debug)
     if not args.raw:
         print('Connecting...')
     return mug
 
 
 async def find_device(args: Namespace) -> BLEDevice:
     """Find a single device that has already been paired."""
@@ -163,14 +164,27 @@
         shared_parser.add_argument(
             '-m',
             '--mac',
             action='store',
             type=validate_mac,
             help='Only look for this specific address',
         )
+        shared_parser.add_argument(
+            '-d',
+            '--debug',
+            action='store_true',
+            help='Print extra information for development or debugging issues',
+        )
+        shared_parser.add_argument(
+            '--log-file',
+            type=FileType('w', encoding='utf-8'),
+            nargs='?',
+            default=sys.stdout,
+            help='File to write logs too (Will be overwritten)',
+        )
         shared_parser.add_argument('-r', '--raw', help='No formatting. One value per line.', action='store_true')
         if platform.system() == 'Linux':
             # Only works on Linux with BlueZ so don't add for others.
             shared_parser.add_argument(
                 '-a',
                 '--adapter',
                 action='store',
@@ -191,8 +205,14 @@
         set_parser.add_argument('--target-temp', help='Target Temperature', type=float, required=False)
         set_parser.add_argument('--temperature-unit', help='Temperature Unit', choices=['C', 'F'], required=False)
         set_parser.add_argument('--led-colour', help='LED Colour', type=colour_type, required=False)
 
     async def run(self) -> None:
         """Run the specified command based on subparser."""
         args = self.parser.parse_args()
+        if args.debug:
+            logging.basicConfig(
+                stream=args.log_file,
+                level=logging.DEBUG,
+                format='[%(asctime)s] %(levelname)s [%(filename)s.%(funcName)s:%(lineno)d] %(message)s',
+            )
         await self._commands[args.command](args)
```

### Comparing `python_ember_mug-0.6.0b9/ember_mug/cli/helpers.py` & `python_ember_mug-0.6.1/ember_mug/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.0b9/ember_mug/consts.py` & `python_ember_mug-0.6.1/ember_mug/consts.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,35 +5,32 @@
 import re
 from enum import Enum, IntEnum
 from functools import cached_property
 from typing import Literal
 from uuid import UUID
 
 # Bluetooth names of supported mugs
-EMBER_BLUETOOTH_NAMES: tuple[str, ...] = ("Ember Ceramic Mug",)
+EMBER_BLUETOOTH_NAMES: tuple[str, ...] = (
+    "Ember Ceramic Mug",
+    "Ember Travel Mug",
+    "Ember Cup",
+    "Ember Cup 2",
+)
 
 # Format for all the mug's Bluetooth UUIDs
 UUID_TEMPLATE = "fc54{:0>4x}-236c-4c94-8fa9-944a3e5353fa"
 
 
 class TemperatureUnit(str, Enum):
     """Temperature Units."""
 
     CELSIUS: Literal["°C"] = "°C"
     FAHRENHEIT: Literal["°F"] = "°F"
 
 
-class DisconnectReason(str, Enum):
-    """Helper to differentiate disconnect reasons for debugging."""
-
-    TIMEOUT = "timeout"
-    EXPECTED = "expected"
-    UNEXPECTED = "unexpected"
-
-
 class MugCharacteristic(IntEnum):
     """Characteristic IDs for the Mug."""
 
     # Name of mug in byte string (Read/Write)
     MUG_NAME = 1
     # Current Mug Temp (Read)
     CURRENT_TEMPERATURE = 2
```

### Comparing `python_ember_mug-0.6.0b9/ember_mug/data.py` & `python_ember_mug-0.6.1/ember_mug/data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.0b9/ember_mug/formatting.py` & `python_ember_mug-0.6.1/ember_mug/formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.0b9/ember_mug/mug.py` & `python_ember_mug-0.6.1/ember_mug/mug.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import asyncio
 import contextlib
 import logging
 from collections.abc import AsyncIterator
 from datetime import datetime, timezone
 from enum import Enum
-from functools import partial
 from time import time
 from typing import Any, Callable, Literal
 
 from bleak import BleakClient, BleakError
 from bleak.backends.characteristic import BleakGATTCharacteristic
 from bleak.backends.device import BLEDevice
 from bleak_retry_connector import establish_connection
@@ -19,49 +18,55 @@
 from .consts import (
     EXTRA_ATTRS,
     INITIAL_ATTRS,
     IS_LINUX,
     MUG_NAME_REGEX,
     PUSH_EVENT_BATTERY_IDS,
     UPDATE_ATTRS,
-    DisconnectReason,
     LiquidState,
     MugCharacteristic,
     PushEvent,
     TemperatureUnit,
 )
 from .data import BatteryInfo, Change, Colour, MugData, MugFirmwareInfo, MugMeta
-from .utils import bytes_to_big_int, bytes_to_little_int, decode_byte_string, encode_byte_string, temp_from_bytes
+from .utils import (
+    bytes_to_big_int,
+    bytes_to_little_int,
+    decode_byte_string,
+    encode_byte_string,
+    log_services,
+    temp_from_bytes,
+)
 
 logger = logging.getLogger(__name__)
 
 DISCONNECT_DELAY = 120
 
 
 class EmberMug:
     """Handle actual the actual mug connection and update states."""
 
     def __init__(
         self,
         ble_device: BLEDevice,
         include_extra: bool = False,
         use_metric: bool = True,
+        debug: bool = False,
         **kwargs: Any,
     ) -> None:
         """Initialize connection manager."""
         self.device = ble_device
-        self.data = MugData(ble_device.name, include_extra=include_extra, use_metric=use_metric)
+        self.data = MugData(ble_device.name or 'EMBER', include_extra=include_extra, use_metric=use_metric)
 
+        self.debug = debug
         self._connect_lock = asyncio.Lock()
         self._operation_lock = asyncio.Lock()
         self._expected_disconnect = False
         self._callbacks: dict[Callable[[MugData], None], Callable[[], None]] = {}
         self._client: BleakClient = None  # type: ignore[assignment]
-        self._loop = asyncio.get_running_loop()
-        self._disconnect_timer: asyncio.TimerHandle | None = None
         self._queued_updates: set[str] = set()
         self._latest_events: dict[int, float] = {}
         self._client_kwargs: dict[str, str] = {}
         self._initial_attrs = INITIAL_ATTRS if include_extra else (INITIAL_ATTRS - EXTRA_ATTRS)
         self._update_attrs = UPDATE_ATTRS if include_extra else (UPDATE_ATTRS - EXTRA_ATTRS)
 
         logger.debug("New mug connection initialized.")
@@ -71,35 +76,35 @@
         """Set the ble device."""
         logger.debug("Set new device from %s to %s", self.device, ble_device)
         self.device = ble_device
 
     async def _ensure_connection(self) -> None:
         """Connect to mug."""
         if self._connect_lock.locked():
-            logger.debug("Connection to %s already in progress. Waiting first.", self.data.name)
+            logger.debug("Connection to %s already in progress. Waiting first.", self.device.name)
 
         if self._client is not None and self._client.is_connected:
-            self._reset_disconnect_timer()
             return
 
         async with self._connect_lock:
             # Also check after lock is acquired
             if self._client is not None and self._client.is_connected:
-                self._reset_disconnect_timer()
                 return
             try:
                 logger.debug("Establishing a new connection from mug (ID: %s) to %s", id(self), self.device)
                 client = await establish_connection(
                     client_class=BleakClient,
                     device=self.device,
                     name=f'{self.data.name} ({self.device.address})',
                     use_services_cache=True,
                     disconnected_callback=self._disconnect_callback,  # type: ignore
                     ble_device_callback=lambda: self.device,
                 )
+                if self.debug is True:
+                    log_services(client.services)
                 self._expected_disconnect = False
             except (asyncio.TimeoutError, BleakError) as error:
                 logger.error("%s: Failed to connect to the mug: %s", self.device, error)
                 raise error
             # Attempt to pair for good measure
             try:
                 await client.pair()
@@ -108,27 +113,16 @@
             except NotImplementedError:
                 # workaround for Home Assistant ESPHome Proxy backend which does not allow pairing.
                 logger.warning(
                     'Pairing not implemented. '
                     'If your mug is still in pairing mode (blinking blue) tap the button on the bottom to exit.',
                 )
             self._client = client
-            self._reset_disconnect_timer()
             await self.subscribe()
 
-    def _reset_disconnect_timer(self) -> None:
-        """Reset disconnect timer."""
-        if self._disconnect_timer:
-            self._disconnect_timer.cancel()
-        self._expected_disconnect = False
-        self._disconnect_timer = self._loop.call_later(
-            DISCONNECT_DELAY,
-            partial(self.disconnect, reason=DisconnectReason.TIMEOUT),
-        )
-
     async def _read(self, characteristic: MugCharacteristic) -> bytearray:
         """Helper to read characteristic from Mug."""
         if self._operation_lock.locked():
             logger.debug("Operation already in progress. waiting for it to complete")
         async with self._operation_lock:
             data = await self._client.read_gatt_char(characteristic.uuid)
             logger.debug("Read attribute '%s' with value '%s'", characteristic, data)
@@ -143,18 +137,18 @@
             try:
                 await self._client.write_gatt_char(characteristic.uuid, data)
                 logger.debug("Wrote '%s' to attribute '%s'", data, characteristic)
             except BleakError as e:
                 logger.error("Failed to write '%s' to attribute '%s': %s", data, characteristic, e)
                 raise
 
-    async def disconnect(self, reason: DisconnectReason = DisconnectReason.EXPECTED) -> None:
+    async def disconnect(self, expected: bool = True) -> None:
         """Disconnect from mug and stop listening to notifications."""
-        logger.debug("%s disconnect called", reason.value.title())
-        self._expected_disconnect = reason != DisconnectReason.EXPECTED
+        logger.debug("%s disconnect called", "Expected" if expected else "Unexpected")
+        self._expected_disconnect = expected
         if self._client and self._client.is_connected:
             async with self._connect_lock:
                 await self.unsubscribe()
                 await self._client.disconnect()
         self._client = None  # type: ignore[assignment]
         self._expected_disconnect = False
```

### Comparing `python_ember_mug-0.6.0b9/ember_mug/scanner.py` & `python_ember_mug-0.6.1/ember_mug/scanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     """Create a filter for finding the mug by name and or mac address."""
     known_names = [n.lower() for n in EMBER_BLUETOOTH_NAMES]
 
     def mug_filter(device: BLEDevice, advertisement: AdvertisementData) -> bool:
         """Filter by mac if specified else just check the name."""
         if mac is not None and device.address.lower() != mac:
             return False
-        return device.name.lower() in known_names
+        return bool(device.name and device.name.lower() in known_names)
 
     return mug_filter
 
 
 async def find_mug(mac: str | None = None, adapter: str | None = None) -> BLEDevice | None:
     """Find a mug."""
     if mac is not None:
```

### Comparing `python_ember_mug-0.6.0b9/pyproject.toml` & `python_ember_mug-0.6.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "python-ember-mug"
-version = "0.6.0b9"
+version = "0.6.1"
 homepage = "https://github.com/sopelj/python-ember-mug"
 description = "Python Library for Ember Mugs."
 authors = ["Jesse Sopel <jesse.sopel@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -28,32 +28,32 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 bleak-retry-connector = ">=2.13.0"
 bleak = ">=0.19.5"
 
 [tool.poetry.group.dev.dependencies]
-black  = { version = "^22.6.0" }
+black  = { version = ">=22.6,<24.0" }
 isort  = { version = "^5.8.0" }
-flake8  = { version = "^5.0" }
+flake8  = { version = ">=5,<7" }
 flake8-docstrings = { version = "^1.6.0" }
-mypy = { version = "^0.971" }
+mypy = { version = ">=0.971,<1.2" }
 pytest  = { version = "^7.2.1" }
-pytest-cov  = { version = "^3.0.0" }
-pytest-asyncio =  { version = "^0.19.0" }
+pytest-cov  = { version = ">=3,<5" }
+pytest-asyncio =  { version = ">=0.19,<0.22" }
 tox  = { version = "^3.20.1" }
 virtualenv  = { version = "^20.2.2" }
 mkdocs  = { version = "^1.1.2" }
-mkdocs-include-markdown-plugin  = { version = "^3.6.1" }
-mkdocs-material  = { version = "^8.4.1" }
-mkdocstrings  = { version = "^0.19.0",  extras = ["python"]}
+mkdocs-include-markdown-plugin  = { version = ">=3.6.1,<5.0.0" }
+mkdocs-material  = { version = ">=8.4.1,<10.0.0" }
+mkdocstrings  = { version = ">=0.19,<0.22",  extras = ["python"]}
 mkdocs-material-extensions  = { version = "^1.0.1" }
 twine  = { version = "^4.0.0" }
 mkdocs-autorefs = {version = "^0.4.1" }
-pre-commit = "^2.12.0"
+pre-commit = ">=2.12,<4.0"
 toml = "^0.10.2"
 bump2version = "^1.0.1"
 tox-gh-actions = "^2.9.1"
 
 [tool.poetry.extras]
 test = [
     "pytest",
```

### Comparing `python_ember_mug-0.6.0b9/tests/cli/test_commands.py` & `python_ember_mug-0.6.1/tests/cli/test_commands.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from argparse import Namespace
 from collections.abc import Generator
+from typing import Any
 from unittest.mock import AsyncMock, MagicMock, Mock, patch
 
 import pytest
 from bleak import BleakError, BLEDevice
 from pytest import CaptureFixture
 
 from ember_mug import EmberMug
@@ -21,43 +22,55 @@
     with patch('ember_mug.cli.commands.get_mug') as mock:
         mock_mug = AsyncMock()
         mock_mug.connection = Mock(return_value=mock_connection)
         mock.return_value = mock_mug
         yield mock_mug
 
 
+def mock_namespace(**kwargs: Any) -> Namespace:
+    defaults = {
+        'imperial': False,
+        'extra': False,
+        'raw': False,
+        'debug': False,
+        'adapter': None,
+    }
+    defaults.update(**kwargs)
+    return Namespace(**defaults)
+
+
 @patch('ember_mug.cli.commands.EmberMug', spec=EmberMug)
 @patch('ember_mug.cli.commands.find_device')
 async def test_get_mug(
     mock_find_device: AsyncMock,
     mock_ember_mug: AsyncMock,
     capsys: CaptureFixture,
     ble_device: BLEDevice,
 ) -> None:
     mock_find_device.return_value = ble_device
-    args = Namespace(imperial=False, extra=True, raw=False)
+    args = mock_namespace(extra=True)
     mug = await get_mug(args)
     assert mug is not None
     mock_find_device.assert_called_once_with(args)
-    mock_ember_mug.assert_called_once_with(ble_device, use_metric=True, include_extra=True)
+    mock_ember_mug.assert_called_once_with(ble_device, use_metric=True, include_extra=True, debug=False)
     captured = capsys.readouterr()
     assert captured.out == "Connecting...\n"
 
     # Raw prints nothing
-    args = Namespace(imperial=False, extra=True, raw=True)
+    args = mock_namespace(extra=True, raw=True)
     mug = await get_mug(args)
     assert mug is not None
     captured = capsys.readouterr()
     assert captured.out == ""
 
 
 @patch('ember_mug.cli.commands.find_mug')
 async def test_find_device(mock_find_mug: AsyncMock, capsys: CaptureFixture, ble_device: BLEDevice) -> None:
     mock_find_mug.return_value = ble_device
-    args = Namespace(mac=ble_device.address, adapter=None, raw=False)
+    args = mock_namespace(mac=ble_device.address)
     device = await find_device(args)
     assert device == ble_device
     mock_find_mug.assert_called_once_with(mac=ble_device.address, adapter=None)
     captured = capsys.readouterr()
     assert captured.out == f"Found mug: {ble_device}\n"
 
     # Raw prints nothing
@@ -66,89 +79,89 @@
     captured = capsys.readouterr()
     assert captured.out == f""
 
 
 @patch('ember_mug.cli.commands.find_mug')
 async def test_find_device_no_device(mock_find_mug: AsyncMock, capsys: CaptureFixture) -> None:
     mock_find_mug.return_value = None
-    args = Namespace(mac=TEST_MAC, adapter=None, raw=False)
+    args = mock_namespace(mac=TEST_MAC)
     with pytest.raises(SystemExit):
         await find_device(args)
     mock_find_mug.assert_called_once_with(mac=TEST_MAC, adapter=None)
     captured = capsys.readouterr()
     assert captured.out == "No mug was found.\n"
 
 
 @patch('ember_mug.cli.commands.find_mug')
 async def test_find_device_bleak_error(mock_find_mug: AsyncMock, capsys: CaptureFixture) -> None:
     mock_find_mug.side_effect = BleakError('Test Error')
-    args = Namespace(mac=TEST_MAC, adapter=None, raw=False)
+    args = mock_namespace(mac=TEST_MAC)
     with pytest.raises(SystemExit):
         await find_device(args)
     mock_find_mug.assert_called_once_with(mac=TEST_MAC, adapter=None)
     captured = capsys.readouterr()
     assert captured.out == "An error occurred trying to find a mug: Test Error\n"
 
 
 @patch('ember_mug.cli.commands.discover_mugs')
 async def test_discover(mock_discover_mugs: AsyncMock, capsys: CaptureFixture, ble_device: BLEDevice) -> None:
     mock_discover_mugs.return_value = [ble_device]
-    args = Namespace(mac=TEST_MAC, adapter=None, raw=False)
+    args = mock_namespace(mac=TEST_MAC)
     mugs = await discover(args)
     assert mugs == [ble_device]
     mock_discover_mugs.assert_called_once_with(mac=TEST_MAC)
     captured = capsys.readouterr()
     assert captured.out == f"Found mug: {ble_device}\n"
 
     mock_discover_mugs.reset_mock()
-    args = Namespace(mac=TEST_MAC, adapter=None, raw=True)
+    args = mock_namespace(mac=TEST_MAC, raw=True)
     mugs = await discover(args)
     assert mugs == [ble_device]
     mock_discover_mugs.assert_called_once_with(mac=TEST_MAC)
     captured = capsys.readouterr()
     assert captured.out == f"{TEST_MAC}\n"
 
 
 @patch('ember_mug.cli.commands.discover_mugs')
 async def test_discover_no_device(mock_discover_mugs: AsyncMock, capsys: CaptureFixture) -> None:
     mock_discover_mugs.return_value = []
-    args = Namespace(mac=TEST_MAC, adapter=None, raw=False)
+    args = mock_namespace(mac=TEST_MAC)
     with pytest.raises(SystemExit):
         await discover(args)
     mock_discover_mugs.assert_called_once_with(mac=TEST_MAC)
     captured = capsys.readouterr()
     assert captured.out == "No mugs were found. Be sure it is in pairing mode. Or use \"find\" if already paired.\n"
 
 
 @patch('ember_mug.cli.commands.discover_mugs')
 async def test_discover_bleak_error(mock_discover_mugs: AsyncMock, capsys: CaptureFixture) -> None:
     mock_discover_mugs.side_effect = BleakError('Test Error')
-    args = Namespace(mac=TEST_MAC, adapter=None, raw=False)
+    args = mock_namespace(mac=TEST_MAC)
     with pytest.raises(SystemExit):
         await discover(args)
     mock_discover_mugs.assert_called_once_with(mac=TEST_MAC)
     captured = capsys.readouterr()
     assert captured.out == "An error occurred trying to discover mugs: Test Error\n"
 
 
 @patch('ember_mug.cli.commands.print_info')
 async def test_fetch_info(
     mock_print_info: AsyncMock,
     mock_mug_with_connection: AsyncMock,
     capsys: CaptureFixture,
 ) -> None:
     # Test normal
-    args = Namespace(mac=TEST_MAC, adapter=None, raw=False)
+    args = mock_namespace(mac=TEST_MAC)
     await fetch_info(args)
     captured = capsys.readouterr()
     assert captured.out == "Connected.\nFetching Info\n"
     mock_print_info.assert_called_once_with(mock_mug_with_connection)
 
     # Test with Raw
-    args = Namespace(mac=TEST_MAC, adapter=None, raw=True)
+    args = mock_namespace(mac=TEST_MAC, raw=True)
     await fetch_info(args)
     captured = capsys.readouterr()
     assert captured.out == ""
 
 
 @patch('ember_mug.cli.commands.print_table')
 async def test_get_mug_value(
@@ -156,21 +169,21 @@
     mock_mug_with_connection: AsyncMock,
     capsys: CaptureFixture,
 ) -> None:
     mock_mug_with_connection.data = MugData('test')
     mock_mug_with_connection.data.get_formatted_attr = Mock(return_value='test')  # type: ignore[assignment]
     mock_mug_with_connection.get_target_temp.return_value = 55.5
     mock_mug_with_connection.get_name.return_value = 'test'
-    args = Namespace(adapter=None, raw=False, attributes=['target_temp', 'name'])
+    args = mock_namespace(attributes=['target_temp', 'name'])
     await get_mug_value(args)
     mock_mug_with_connection.get_target_temp.assert_called_once()
     mocked_print_table.assert_called_once_with([('Target Temp', "test"), ('Mug Name', "test")])
 
     mock_mug_with_connection.get_led_colour.return_value = 55.5
-    args = Namespace(adapter=None, raw=True, attributes=['led_colour', 'name'])
+    args = mock_namespace(attributes=['led_colour', 'name'], raw=True)
     await get_mug_value(args)
     captured = capsys.readouterr()
     assert captured.out == "55.5\ntest\n"
 
 
 def test_ember_cli():
     cli = EmberMugCli()
```

### Comparing `python_ember_mug-0.6.0b9/tests/cli/test_helpers.py` & `python_ember_mug-0.6.1/tests/cli/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.0b9/tests/conftest.py` & `python_ember_mug-0.6.1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 
 
 mock_connection = MagicMock(AsyncContextManager)
 
 
 @pytest.fixture(name='ble_device')
 def ble_device_fixture() -> Generator[BLEDevice, None, None]:
-    yield BLEDevice(address=TEST_MAC, name=TEST_MODEL_NAME)
+    yield BLEDevice(address=TEST_MAC, name=TEST_MODEL_NAME, details={}, rssi=1)
 
 
 @pytest.fixture
 def mug_data(ble_device: BLEDevice) -> Generator[MugData, None, None]:
-    yield MugData(ble_device.name)
+    yield MugData(ble_device.name or TEST_MODEL_NAME)
 
 
 @pytest_asyncio.fixture
 async def ember_mug(ble_device: BLEDevice) -> AsyncGenerator[EmberMug | AsyncMock, None]:
     mug = EmberMug(ble_device)
     mug._client = AsyncMock()
     yield mug
```

### Comparing `python_ember_mug-0.6.0b9/tests/test_connection.py` & `python_ember_mug-0.6.1/tests/test_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,16 @@
         assert isinstance(exception, BleakError)
 
 
 def test_set_device(ember_mug: AsyncMock) -> None:
     new_device = BLEDevice(
         address='BA:36:a5:be:88:cb',
         name='Ember Ceramic Mug',
+        details={},
+        rssi=1,
     )
     assert ember_mug.device.address != new_device.address
     ember_mug.set_device(new_device)
     assert ember_mug.device.address == new_device.address
 
 
 async def test_get_mug_meta(ember_mug: AsyncMock):
```

### Comparing `python_ember_mug-0.6.0b9/tests/test_consts.py` & `python_ember_mug-0.6.1/tests/test_consts.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.0b9/tests/test_data.py` & `python_ember_mug-0.6.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.0b9/tests/test_formatting.py` & `python_ember_mug-0.6.1/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.0b9/tests/test_mug_data.py` & `python_ember_mug-0.6.1/tests/test_mug_data.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.0b9/tests/test_scanner.py` & `python_ember_mug-0.6.1/tests/test_scanner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from unittest.mock import AsyncMock, patch
 
 import pytest
 from bleak.backends.device import BLEDevice
 
 from ember_mug.scanner import build_find_filter, build_scanner_kwargs, discover_mugs, find_mug
 
-MUG_1 = BLEDevice(address='32:36:a5:be:88:cb', name='Ember Ceramic Mug')
-MUG_2 = BLEDevice(address='9c:da:8c:19:27:da', name='Ember Ceramic Mug')
+MUG_1 = BLEDevice(address='32:36:a5:be:88:cb', name='Ember Ceramic Mug', details={}, rssi=1)
+MUG_2 = BLEDevice(address='9c:da:8c:19:27:da', name='Ember Ceramic Mug', details={}, rssi=1)
 EXAMPLE_MUGS = [MUG_1, MUG_2]
 
 
 @patch('ember_mug.scanner.IS_LINUX', True)
 def test_build_scanner_kwargs_linux() -> None:
     assert build_scanner_kwargs() == {}
     assert build_scanner_kwargs(adapter='hci0') == {'adapter': 'hci0'}
```

### Comparing `python_ember_mug-0.6.0b9/tests/test_utils.py` & `python_ember_mug-0.6.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.0b9/setup.py` & `python_ember_mug-0.6.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,142 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: python-ember-mug
+Version: 0.6.1
+Summary: Python Library for Ember Mugs.
+Home-page: https://github.com/sopelj/python-ember-mug
+License: MIT
+Author: Jesse Sopel
+Author-email: jesse.sopel@gmail.com
+Requires-Python: >=3.9,<3.12
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: build
+Provides-Extra: dev
+Provides-Extra: doc
+Provides-Extra: test
+Requires-Dist: bleak (>=0.19.5)
+Requires-Dist: bleak-retry-connector (>=2.13.0)
+Project-URL: Bug Tracker, https://github.com/sopelj/python-ember-mug/issues
+Project-URL: Changelog, https://github.com/sopelj/python-ember-mug/blob/main/CHANGELOG.md
+Description-Content-Type: text/markdown
+
+# Python Ember Mug
+
+[![pypi](https://img.shields.io/pypi/v/python-ember-mug.svg)](https://pypi.org/project/python-ember-mug/)
+[![python](https://img.shields.io/pypi/pyversions/python-ember-mug.svg)](https://pypi.org/project/python-ember-mug/)
+[![Build Status](https://github.com/sopelj/python-ember-mug/actions/workflows/dev.yml/badge.svg)](https://github.com/sopelj/python-ember-mug/actions/workflows/dev.yml)
+[![codecov](https://codecov.io/gh/sopelj/python-ember-mug/branch/main/graphs/badge.svg)](https://codecov.io/github/sopelj/python-ember-mug)
+![Project Maintenance](https://img.shields.io/maintenance/yes/2023.svg?style=for-the-badge)
+
+Python Library for interacting with Ember Mugs over Bluetooth
+
+* Documentation: <https://sopelj.github.io/python-ember-mug>
+* GitHub: <https://github.com/sopelj/python-ember-mug>
+* PyPI: <https://pypi.org/project/python-ember-mug/>
+* Free software: MIT
+
+## Summary
+
+This is an *unofficial* library to attempt to interact with Ember Mugs via Bluetooth.
+This was created for use with my [Home Assistant integration](https://github.com/sopelj/hass-ember-mug-component),
+but could be useful separately and has a simple CLI interface too.
+
+**Note**: Works with the standard Ember Mug (1 and 2). The Cup and Thermos may work, but have not been tested.
+
+## Features
+
+* Finding devices
+* Connecting to devices
+* Reading Information (Colour, temp, liquid level, etc.)
+* Writing (Desired temp, colour, temperature unit)*
+* Polling for changes
+
+*** Writing only works if the devices has been set up in the app previously
+
+## Usage
+
+### Python
+
+```python
+from ember_mug.scanner import find_mug, discover_mugs
+from ember_mug.mug import EmberMug
+
+# if first time with mug in pairing
+mugs = await discover_mugs()
+device = mugs[0]
+# after paired you can simply use
+device = await find_mug()
+mug = EmberMug(device)
+await mug.update_all()
+print(mug.data.formatted)
+await mug.disconnect()
+
+# You can also use connection as a context manager
+# if you want to ensure connection before starting and cleanup on exit
+async with mug.connection():
+    print('Connected.\nFetching Info')
+    await mug.update_all()
+    print(mug.data.formatted)
+```
+
+### CLI
+
+It can also be run via command line either directly with `ember-mug --help` or as a module with `python -m ember_mug --help`
+There are four options with different subsections. You can see them by specifying them before help. eg `ember-mug poll --help`
+
+```bash
+ember-mug discover  # Finds the mug in pairing mode for the first time
+ember-mug poll  # fetches info and keeps listening for notifications
+ember-mug get name target-temp  # Prints name and target temp of mug
+ember-mug set --name "My mug" --target-temp 56.8  # Sets the name and target temp to specified values
+```
+
+Basic options:
+
+| Command     | Use                                                                            |
+|-------------|--------------------------------------------------------------------------------|
+| `discover`  | Find/List all detected unpaired mugs in pairing mode                           |
+| `find`      | Find *one* already paired mugs                                                 |
+| `info`      | Connect to *one* mug and print its current state                               |
+| `poll`      | Connect to *one* mug and print its current state and keep watching for changes |
+| `get`       | Get the value(s) of one or more attribute(s) by name                           |
+| `set`       | Set one or more values on the mug                                              |
+
+
+![CLI Example](./docs/images/cli-example.png)
+
+## Caveats
+
+- Since this api is not public, a lot of guesswork and reverse engineering is involved, so it's not perfect.
+- If the mug has not been set up in the app since it was reset, writing is not allowed. I don't know what they set in the app, but it changes something, and it doesn't work without it.
+- Once that mug has been set up in the app, you should ideally forget the device or at least turn off bluetooth whilst using it here, or you will probably get disconnected often
+- I haven't figured out some attributes like udsk, dsk, location and timezone.
+
+## Troubleshooting
+
+### 'Operation failed with ATT error: 0x0e' or another connection error
+This seems to be caused by the bluetooth adaptor being in some sort of passive mode. I have not yet figured out how to wake it programmatically so sadly, you need to manually open `bluetoothctl` to do so.
+Please ensure the mug is in pairing mode (ie the light is flashing blue) and run the `bluetoothctl` command. You don,t need to type anything. run it and wait until the mug connects.
+
+## Todo
+- Test with other devices. Please let me know if you have tried it with others.
+
+## Credits
 
-packages = \
-['ember_mug', 'ember_mug.cli', 'tests', 'tests.cli']
+This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [waynerv/cookiecutter-pypackage](https://github.com/waynerv/cookiecutter-pypackage) project template.
 
-package_data = \
-{'': ['*']}
+## Notice of Non-Affiliation and Disclaimer
 
-install_requires = \
-['bleak-retry-connector>=2.13.0', 'bleak>=0.19.5']
-
-entry_points = \
-{'console_scripts': ['ember-mug = ember_mug.cli:run_cli']}
-
-setup_kwargs = {
-    'name': 'python-ember-mug',
-    'version': '0.6.0b9',
-    'description': 'Python Library for Ember Mugs.',
-    'long_description': '# Python Ember Mug\n\n[![pypi](https://img.shields.io/pypi/v/python-ember-mug.svg)](https://pypi.org/project/python-ember-mug/)\n[![python](https://img.shields.io/pypi/pyversions/python-ember-mug.svg)](https://pypi.org/project/python-ember-mug/)\n[![Build Status](https://github.com/sopelj/python-ember-mug/actions/workflows/dev.yml/badge.svg)](https://github.com/sopelj/python-ember-mug/actions/workflows/dev.yml)\n[![codecov](https://codecov.io/gh/sopelj/python-ember-mug/branch/main/graphs/badge.svg)](https://codecov.io/github/sopelj/python-ember-mug)\n![Project Maintenance](https://img.shields.io/maintenance/yes/2023.svg?style=for-the-badge)\n\nPython Library for interacting with Ember Mugs over Bluetooth\n\n* Documentation: <https://sopelj.github.io/python-ember-mug>\n* GitHub: <https://github.com/sopelj/python-ember-mug>\n* PyPI: <https://pypi.org/project/python-ember-mug/>\n* Free software: MIT\n\n## Summary\n\nThis is an *unofficial* library to attempt to interact with Ember Mugs via Bluetooth.\nThis was created for use with my [Home Assistant integration](https://github.com/sopelj/hass-ember-mug-component),\nbut could be useful separately and has a simple CLI interface too.\n\n**Note**: Should work with the standard Ember Mugs (1 and 2), but the thermoses have not been tested.\n\n## Features\n\n* Finding mugs\n* Connecting to Mugs\n* Reading Information (Colour, temp, liquid level, etc.)\n* Writing (Desired temp, colour, temperature unit)*\n* Polling for changes\n\n*** Writing only works if the mug has been set up in the app previously\n\n## Usage\n\n### Python\n\n```python\nfrom ember_mug.scanner import find_mug, discover_mugs\nfrom ember_mug.mug import EmberMug\n\n# if first time with mug in pairing\nmugs = await discover_mugs()\ndevice = mugs[0]\n# after paired you can simply use\ndevice = await find_mug()\nmug = EmberMug(device)\nasync with mug.connection() as con:\n    print(\'Connected.\\nFetching Info\')\n    await con.update_all()\n    print(mug.formatted_data)\n```\n\n### CLI\n\nIt can also be run via command line either directly with `ember-mug --help` or as a module with `python -m ember_mug --help`\nThere are four options with different subsections. You can see them by specifying them before help. eg `ember-mug poll --help`\n\n```bash\nember-mug discover  # Finds the mug in pairing mode for the first time\nember-mug poll  # fetches info and keeps listening for notifications\nember-mug get name target-temp  # Prints name and target temp of mug\nember-mug set --name "My mug" --target-temp 56.8  # Sets the name and target temp to specified values\n```\n\nBasic options:\n\n| Command     | Use                                                                            |\n|-------------|--------------------------------------------------------------------------------|\n| `discover`  | Find/List all detected unpaired mugs in pairing mode                           |\n| `find`      | Find *one* already paired mugs                                                 |\n| `info`      | Connect to *one* mug and print its current state                               |\n| `poll`      | Connect to *one* mug and print its current state and keep watching for changes |\n| `get`       | Get the value(s) of one or more attribute(s) by name                           |\n| `set`       | Set one or more values on the mug                                              |\n\n\n![CLI Example](./docs/images/cli-example.png)\n\n## Caveats\n\n- Since this api is not public, a lot of guesswork and reverse engineering is involved, so it\'s not perfect.\n- If the mug has not been set up in the app since it was reset, writing is not allowed. I don\'t know what they set in the app, but it changes something, and it doesn\'t work without it.\n- Once that mug has been set up in the app, you should ideally forget the device or at least turn off bluetooth whilst using it here, or you will probably get disconnected often\n- I haven\'t figured out some attributes like udsk, dsk, location and timezone.\n\n## Troubleshooting\n\n### \'Operation failed with ATT error: 0x0e\' or another connection error\nThis seems to be caused by the bluetooth adaptor being in some sort of passive mode. I have not yet figured out how to wake it programmatically so sadly, you need to manually open `bluetoothctl` to do so.\nPlease ensure the mug is in pairing mode (ie the light is flashing blue) and run the `bluetoothctl` command. You don,t need to type anything. run it and wait until the mug connects.\n\n## Todo\n- Test with other devices. Please let me know if you have tried it with others.\n\n## Credits\n\nThis package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [waynerv/cookiecutter-pypackage](https://github.com/waynerv/cookiecutter-pypackage) project template.\n\n## Notice of Non-Affiliation and Disclaimer\n\nThis project is not affiliated, associated, authorized, endorsed by, or in any way officially connected with Ember.\n\nThe name Ember as well as related names, marks, emblems and images are registered trademarks of their respective owners.\n',
-    'author': 'Jesse Sopel',
-    'author_email': 'jesse.sopel@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/sopelj/python-ember-mug',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<3.12',
-}
+This project is not affiliated, associated, authorized, endorsed by, or in any way officially connected with Ember.
 
+The name Ember as well as related names, marks, emblems and images are registered trademarks of their respective owners.
 
-setup(**setup_kwargs)
```

