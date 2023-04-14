# Comparing `tmp/hart-protocol-2023.3.0.tar.gz` & `tmp/hart-protocol-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hart-protocol-2023.3.0.tar", last modified: Fri Mar 10 18:31:19 2023, max compression
+gzip compressed data, was "hart-protocol-2023.4.0.tar", last modified: Fri Apr 14 16:44:54 2023, max compression
```

## Comparing `hart-protocol-2023.3.0.tar` & `hart-protocol-2023.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      429 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/.github/workflows/python-mypy.yml
--rw-r--r--   0        0        0      793 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      447 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/.gitignore
--rw-r--r--   0        0        0      649 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      988 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1100 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/LICENSE
--rw-r--r--   0        0        0     8501 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/README.md
--rw-r--r--   0        0        0        9 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/hart_protocol/VERSION
--rw-r--r--   0        0        0      212 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/hart_protocol/__init__.py
--rw-r--r--   0        0        0      493 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/hart_protocol/__version__.py
--rw-r--r--   0        0        0     7840 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/hart_protocol/_parsing.py
--rw-r--r--   0        0        0     4087 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/hart_protocol/_unpacker.py
--rw-r--r--   0        0        0     1348 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/hart_protocol/common.py
--rw-r--r--   0        0        0        0 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/hart_protocol/py.typed
--rw-r--r--   0        0        0     1576 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/hart_protocol/tools.py
--rw-r--r--   0        0        0     2205 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/hart_protocol/universal.py
--rw-r--r--   0        0        0     1220 2023-03-10 18:31:11.444795 hart-protocol-2023.3.0/pyproject.toml
--rw-r--r--   0        0        0     9558 1970-01-01 00:00:00.000000 hart-protocol-2023.3.0/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/.github/workflows/python-mypy.yml
+-rw-r--r--   0        0        0      793 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      447 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/.gitignore
+-rw-r--r--   0        0        0      649 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1155 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1100 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/LICENSE
+-rw-r--r--   0        0        0     8501 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/README.md
+-rw-r--r--   0        0        0        9 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/VERSION
+-rw-r--r--   0        0        0      212 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/__init__.py
+-rw-r--r--   0        0        0      493 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/__version__.py
+-rw-r--r--   0        0        0     7840 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/_parsing.py
+-rw-r--r--   0        0        0     4087 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/_unpacker.py
+-rw-r--r--   0        0        0     1348 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/common.py
+-rw-r--r--   0        0        0        0 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/py.typed
+-rw-r--r--   0        0        0     1576 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/tools.py
+-rw-r--r--   0        0        0     2205 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/hart_protocol/universal.py
+-rw-r--r--   0        0        0     1220 2023-04-14 16:44:50.237508 hart-protocol-2023.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9558 1970-01-01 00:00:00.000000 hart-protocol-2023.4.0/PKG-INFO
```

### Comparing `hart-protocol-2023.3.0/.github/workflows/python-publish.yml` & `hart-protocol-2023.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.3.0/.pre-commit-config.yaml` & `hart-protocol-2023.4.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -4,24 +4,24 @@
     hooks:
     -   id: trailing-whitespace
     -   id: check-toml
     -   id: no-commit-to-branch
         args: [-b, master]
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
         entry: black
         require_serial: true
         types: [python]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.0.1
+    rev: v1.2.0
     hooks:
       - id: mypy
         exclude: ^docs/conf.py
 
   - repo: https://gitlab.com/yaq/yaq-traits
     rev: v2022.3.0
     hooks:
```

### Comparing `hart-protocol-2023.3.0/CHANGELOG.md` & `hart-protocol-2023.4.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/).
 
 ## [Unreleased]
 
+## [2023.4.0]
+
+### Fixed
+- missing final byte from messages 12, 13, 14, 17, 18
+
 ## [2023.3.0]
 
 ### Changed
 - in responses, device_status and response_code are now unpacked as two separate bytes
 - data with bytecount of 2 has status only, and now returns immediately
 
 ## [2022.8.2]
@@ -22,12 +27,13 @@
 - unpacker was broken in an async context
 
 ## [2022.8.0]
 
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/yaq-project/hart-protocol/compare/v2023.3.0...main
+[Unreleased]: https://github.com/yaq-project/hart-protocol/compare/v2023.4.0...main
+[2023.4.0]: https://github.com/yaq-project/hart-protocol/compare/v2023.3.0...v2023.4.0
 [2023.3.0]: https://github.com/yaq-project/hart-protocol/compare/v2022.8.2...v2023.3.0
 [2022.8.2]: https://github.com/yaq-project/hart-protocol/compare/v2022.8.1...v2022.8.2
 [2022.8.1]: https://github.com/yaq-project/hart-protocol/compare/v2022.8.0...v2022.8.1
 [2022.8.0]: https://gitlab.com/yaq/yaqd-picotech/tags/v2022.8.0
```

### Comparing `hart-protocol-2023.3.0/LICENSE` & `hart-protocol-2023.4.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 The MIT License (MIT)
 
-Copyright © 2022 hart-protocol contributors
+Copyright © 2023 hart-protocol contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `hart-protocol-2023.3.0/README.md` & `hart-protocol-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.3.0/hart_protocol/_parsing.py` & `hart-protocol-2023.4.0/hart_protocol/_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,23 +61,23 @@
         out["secondary_variable"] = secondary_variable
     elif command in [6]:
         out["command_name"] = "write_polling_address"
         polling_address = struct.unpack_from(">B", data)[0]
         out["polling_address"] = polling_address
     elif command in [12]:
         out["command_name"] = "read_message"
-        out["message"] = data[0:23]
+        out["message"] = data[0:24]
     elif command in [13]:
         out["command_name"] = "read_tag_descriptor_date"
-        out["device_tag_name"] = data[0:5]
-        out["device_descriptor"] = data[6:17]
-        out["date"] = data[18:20]
+        out["device_tag_name"] = data[0:6]
+        out["device_descriptor"] = data[6:18]
+        out["date"] = data[18:21]
     elif command in [14]:
         out["command_name"] = "read_primary_variable_information"
-        out["serial_no"] = data[0:2]
+        out["serial_no"] = data[0:3]
         sensor_limits_code, upper_limit, lower_limit, min_span = struct.unpack_from(
             ">xxxBfff", data
         )
         out["sensor_limits_code"] = sensor_limits_code
         out["upper_limit"] = upper_limit
         out["lower_limit"] = lower_limit
         out["min_span"] = min_span
@@ -102,20 +102,20 @@
         out["write_protect"] = write_protect
         out["private_label"] = private_label
     elif command in [16]:
         out["command_name"] = "read_final_assembly_number"
         out["final_assembly_no"] = int.from_bytes(data[0:2], "big")
     elif command in [17]:
         out["command_name"] = "write_message"
-        out["message"] = data[0:23]
+        out["message"] = data[0:24]
     elif command in [18]:
         out["command_name"] = "write_tag_descriptor_date"
-        out["device_tag_name"] = data[0:5]
-        out["device_descriptor"] = data[6:17]
-        out["date"] = data[18:20]
+        out["device_tag_name"] = data[0:6]
+        out["device_descriptor"] = data[6:18]
+        out["date"] = data[18:21]
     elif command in [19]:
         out["command_name"] = "write_final_assembly_number"
         out["final_assembly_no"] = int.from_bytes(data[0:2], "big")
 
     # COMMON COMMANDS
 
     # elif command in [37]:
```

### Comparing `hart-protocol-2023.3.0/hart_protocol/_unpacker.py` & `hart-protocol-2023.4.0/hart_protocol/_unpacker.py`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.3.0/hart_protocol/common.py` & `hart-protocol-2023.4.0/hart_protocol/common.py`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.3.0/hart_protocol/tools.py` & `hart-protocol-2023.4.0/hart_protocol/tools.py`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.3.0/hart_protocol/universal.py` & `hart-protocol-2023.4.0/hart_protocol/universal.py`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.3.0/pyproject.toml` & `hart-protocol-2023.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hart-protocol-2023.3.0/PKG-INFO` & `hart-protocol-2023.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hart-protocol
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: A sans-io python implementation of the Highway Addressable Remote Transducer Protocol.
 Home-page: https://github.com/yaq-project/hart-protocol
 Author: Blaise Thompson
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

