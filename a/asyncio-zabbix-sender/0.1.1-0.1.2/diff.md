# Comparing `tmp/asyncio_zabbix_sender-0.1.1.tar.gz` & `tmp/asyncio_zabbix_sender-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncio_zabbix_sender-0.1.1.tar", max compression
+gzip compressed data, was "asyncio_zabbix_sender-0.1.2.tar", max compression
```

## Comparing `asyncio_zabbix_sender-0.1.1.tar` & `asyncio_zabbix_sender-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-01 19:03:10.210130 asyncio_zabbix_sender-0.1.1/LICENSE
--rw-r--r--   0        0        0     3494 2023-04-04 12:53:38.647189 asyncio_zabbix_sender-0.1.1/README.md
--rw-r--r--   0        0        0      912 2023-04-03 20:52:44.134655 asyncio_zabbix_sender-0.1.1/asyncio_zabbix_sender/__init__.py
--rw-r--r--   0        0        0     4230 2023-04-04 07:27:55.015576 asyncio_zabbix_sender-0.1.1/asyncio_zabbix_sender/_measurements.py
--rw-r--r--   0        0        0     2460 2023-04-04 08:24:28.793275 asyncio_zabbix_sender-0.1.1/asyncio_zabbix_sender/_protocol.py
--rw-r--r--   0        0        0     1388 2023-04-03 20:35:29.725103 asyncio_zabbix_sender-0.1.1/asyncio_zabbix_sender/_response.py
--rw-r--r--   0        0        0      883 2023-04-04 08:09:33.737985 asyncio_zabbix_sender-0.1.1/asyncio_zabbix_sender/_util.py
--rw-r--r--   0        0        0     3674 2023-04-04 08:24:28.777275 asyncio_zabbix_sender-0.1.1/asyncio_zabbix_sender/_zabbix_sender.py
--rw-r--r--   0        0        0      585 2023-04-04 12:54:24.607299 asyncio_zabbix_sender-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4309 1970-01-01 00:00:00.000000 asyncio_zabbix_sender-0.1.1/setup.py
--rw-r--r--   0        0        0     4225 1970-01-01 00:00:00.000000 asyncio_zabbix_sender-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-01 19:03:10.210130 asyncio_zabbix_sender-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3494 2023-04-04 12:53:38.647189 asyncio_zabbix_sender-0.1.2/README.md
+-rw-r--r--   0        0        0      912 2023-04-03 20:52:44.134655 asyncio_zabbix_sender-0.1.2/asyncio_zabbix_sender/__init__.py
+-rw-r--r--   0        0        0     5425 2023-04-14 08:21:37.524874 asyncio_zabbix_sender-0.1.2/asyncio_zabbix_sender/_measurements.py
+-rw-r--r--   0        0        0     2460 2023-04-04 08:24:28.793275 asyncio_zabbix_sender-0.1.2/asyncio_zabbix_sender/_protocol.py
+-rw-r--r--   0        0        0     1388 2023-04-03 20:35:29.725103 asyncio_zabbix_sender-0.1.2/asyncio_zabbix_sender/_response.py
+-rw-r--r--   0        0        0      883 2023-04-04 08:09:33.737985 asyncio_zabbix_sender-0.1.2/asyncio_zabbix_sender/_util.py
+-rw-r--r--   0        0        0     3674 2023-04-04 08:24:28.777275 asyncio_zabbix_sender-0.1.2/asyncio_zabbix_sender/_zabbix_sender.py
+-rw-r--r--   0        0        0      585 2023-04-14 08:25:24.662258 asyncio_zabbix_sender-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4309 1970-01-01 00:00:00.000000 asyncio_zabbix_sender-0.1.2/setup.py
+-rw-r--r--   0        0        0     4225 1970-01-01 00:00:00.000000 asyncio_zabbix_sender-0.1.2/PKG-INFO
```

### Comparing `asyncio_zabbix_sender-0.1.1/LICENSE` & `asyncio_zabbix_sender-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncio_zabbix_sender-0.1.1/README.md` & `asyncio_zabbix_sender-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `asyncio_zabbix_sender-0.1.1/asyncio_zabbix_sender/__init__.py` & `asyncio_zabbix_sender-0.1.2/asyncio_zabbix_sender/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncio_zabbix_sender-0.1.1/asyncio_zabbix_sender/_measurements.py` & `asyncio_zabbix_sender-0.1.2/asyncio_zabbix_sender/_measurements.py`

 * *Files 17% similar despite different names*

```diff
@@ -114,7 +114,44 @@
 
     def __bytes__(self) -> bytes:
         """Represent the measurements as a Zabbix request.
 
         :return: Zabbix request as bytes.
         """
         return str(self).encode("utf-8")
+
+    def __repr__(self) -> str:
+        """Represent the measurements as the object in the current state.
+
+        :return: Representation of the current state
+        """
+        parts = [type(self).__name__, "("]
+        if len(self._measurements) > 0:
+            parts.append("measurements=[")
+            parts.append(
+                ", ".join([repr(measurement) for measurement in self._measurements])
+            )
+            parts.append("], ")
+        if self.clock is not None:
+            parts.append(f"clock={self.clock}")
+            parts.append(", ")
+        if self.ns is not None:
+            parts.append(f"ns={self.ns}")
+        if parts[-1] == ", ":
+            parts.pop()
+        parts.append(")")
+        return "".join(parts)
+
+    def __len__(self) -> int:
+        """Return the number of measurements currently in the collection.
+
+        :return: Number of measurements
+        """
+        return len(self._measurements)
+
+    def __iter__(self) -> typing.Generator[Measurement, None, None]:
+        """Iterate all measurements
+
+        :return: Generator with all measurements
+        """
+        for measurement in self._measurements:
+            yield measurement
```

### Comparing `asyncio_zabbix_sender-0.1.1/asyncio_zabbix_sender/_protocol.py` & `asyncio_zabbix_sender-0.1.2/asyncio_zabbix_sender/_protocol.py`

 * *Files identical despite different names*

### Comparing `asyncio_zabbix_sender-0.1.1/asyncio_zabbix_sender/_response.py` & `asyncio_zabbix_sender-0.1.2/asyncio_zabbix_sender/_response.py`

 * *Files identical despite different names*

### Comparing `asyncio_zabbix_sender-0.1.1/asyncio_zabbix_sender/_util.py` & `asyncio_zabbix_sender-0.1.2/asyncio_zabbix_sender/_util.py`

 * *Files identical despite different names*

### Comparing `asyncio_zabbix_sender-0.1.1/asyncio_zabbix_sender/_zabbix_sender.py` & `asyncio_zabbix_sender-0.1.2/asyncio_zabbix_sender/_zabbix_sender.py`

 * *Files identical despite different names*

### Comparing `asyncio_zabbix_sender-0.1.1/pyproject.toml` & `asyncio_zabbix_sender-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncio-zabbix-sender"
-version = "0.1.1"
+version = "0.1.2"
 description = "Asyncio implementation of the Zabbix Sender protocol"
 repository = "https://github.com/mastdi/asyncio-zabbix-sender"
 authors = ["Martin Storgaard Dieu <martin@storgaarddieu.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "asyncio_zabbix_sender"}]
```

### Comparing `asyncio_zabbix_sender-0.1.1/setup.py` & `asyncio_zabbix_sender-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['asyncio_zabbix_sender']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'asyncio-zabbix-sender',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Asyncio implementation of the Zabbix Sender protocol',
     'long_description': '# Zabbix sender\nDependency free implementation of the Zabbix Sender protocol using asyncio.\n\nKey features:\n- **Full specification** implemented compared to other Zabbix sender implementations\n- **Compression** is enabled as default\n- **Asynchronous** implementation allows the program to continue while waiting for a response from Zabbix\n\n## Installation\nThe package can be found on PyPI and installed using pip:\n```commandline\npip install asyncio-zabbix-sender\n```\n\n## Usage\n\nThe measurements for the [Zabbix trapper item(s)](https://www.zabbix.com/documentation/6.0/en/manual/config/items/itemtypes/trapper) can be sent using a high-level API.\nThe `Measurements` object is a collection of measurements.\nThe measurements can both be added via the constructor (as per the example below), but also dynamically via the `add_measurement` method.\n```python\nimport datetime\nfrom asyncio_zabbix_sender import ZabbixSender, Measurements, Measurement\n\nsender = ZabbixSender("example.com")\n\nmeasurements = Measurements([\n    Measurement(\n        "vm-game-server", "cheat.used[doom,player1]", "idkfa", datetime.datetime.utcnow()\n    )\n])\n\nresponse = await sender.send(measurements)\n```\n\nThis package can also be used on a lower level to send packets directly.\n```python\nfrom asyncio_zabbix_sender import create_packet, ZabbixSender\n\npacket = create_packet(\n    request=b\'{"request":"sender data","data":[{"host":"<hostname>","key":"trap","value":"test value"}]}\',\n    use_compression=True\n)\n\nsender = ZabbixSender("example.com")\nresponse = await sender.send_packet(packet)\n```\n\n## Logging\nThe logger can be configured by using the name `asyncio-zabbix-sender`:\n\n```python\nimport logging\n\nlogger = logging.getLogger("asyncio-zabbix-sender")\nlogger.setLevel(logging.DEBUG)\n```\n\nExample from the `test_send` unit test by running pytest with `--log-cli-level=DEBUG`:\n```text\n\nDEBUG    asyncio-zabbix-sender:_protocol.py:47 Compressed packet: 40 bytes. Original 35.\nDEBUG    asyncio-zabbix-sender:_zabbix_sender.py:63 Created packet from measurements. Used compression: True.\nDEBUG    asyncio-zabbix-sender:_zabbix_sender.py:78 Sending packet: b\'ZBXD\\x03(\\x00\\x00\\x00#\\x00\\x00\\x00x\\x9c\\xabVJI,IT\\xb2\\x8a\\x8e\\xd5Q*J-,M-.Q\\xb2R*N\\xcdKI-R\\x00K\\xd5\\x02\\x00\\xd3\\xc2\\x0b\\xfb\'\nDEBUG    asyncio-zabbix-sender:_zabbix_sender.py:84 Got response: b\'x\\x9c\\x15\\xc8\\xc1\\n\\x80 \\x0c\\x00\\xd0_\\x19;G\\xa0\\xd9!\\xfd\\x1a\\xd1\\t\\x82l\\xe2\\xec\\x14\\xfd{y{\\xbc\\x07\\x07i\\x17VB\\x0f\\xa8wJ\\xa4\\x8a\\x1b`\\xe5"\\xab\\xfa\\x90U\\x94=8\\x13\\xa0\\xc4\\xda\\x96m\\x80)3\\xb6\\x7f\\x8f\\x00JI8+h\\\'\\x9e\\x1e\\x0e\\xb3;s^\\x16\\xdf\\x0f\\xc8\\xd6\\x1d\\xb5\'\nINFO     asyncio-zabbix-sender:_zabbix_sender.py:87 Packet sent: 53 bytes. Response data received: 88 bytes. Response flags 3.\nDEBUG    asyncio-zabbix-sender:_zabbix_sender.py:97 Parsed response payload: {\'response\': \'success\', \'info\': \'processed: 41; failed: 2; total: 43; seconds spent: 31.41592\'}\n```\n\nNote that only a summary of the packet that are send and the response received are logged as informational.\nEverything else is logged at debug level.\n\nThe INFO log entry contains the response flags.\nA response flag are set by:\n- 0x01 - Zabbix communications protocol\n- 0x02 - If compression is used\n- 0x04 - If the response is a large packet\n\n## Road map\nThe following improvements are planned (not necessary in order):\n\n- Encryption between the sender and Zabbix\n  - connection using TLS and a pre-shared key (psk)\n  - connection using TLS and a certificate (cert)\n- Better error handling\n- More documentation\n',
     'author': 'Martin Storgaard Dieu',
     'author_email': 'martin@storgaarddieu.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mastdi/asyncio-zabbix-sender',
```

### Comparing `asyncio_zabbix_sender-0.1.1/PKG-INFO` & `asyncio_zabbix_sender-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio-zabbix-sender
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asyncio implementation of the Zabbix Sender protocol
 Home-page: https://github.com/mastdi/asyncio-zabbix-sender
 License: Apache-2.0
 Author: Martin Storgaard Dieu
 Author-email: martin@storgaarddieu.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

