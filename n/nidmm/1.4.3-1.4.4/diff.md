# Comparing `tmp/nidmm-1.4.3.tar.gz` & `tmp/nidmm-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nidmm-1.4.3.tar", last modified: Fri Dec 16 18:56:02 2022, max compression
+gzip compressed data, was "nidmm-1.4.4.tar", last modified: Fri Apr 14 16:08:19 2023, max compression
```

## Comparing `nidmm-1.4.3.tar` & `nidmm-1.4.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:02.825315 nidmm-1.4.3/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8737 2022-12-16 18:56:02.825315 nidmm-1.4.3/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     7734 2022-12-16 18:55:15.000000 nidmm-1.4.3/README.rst
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:02.815315 nidmm-1.4.3/nidmm/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        7 2022-12-16 18:55:11.000000 nidmm-1.4.3/nidmm/VERSION
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     3023 2022-12-16 18:55:11.000000 nidmm-1.4.3/nidmm/__init__.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     5432 2022-12-16 18:55:08.000000 nidmm-1.4.3/nidmm/_attributes.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    13869 2022-12-16 18:55:11.000000 nidmm-1.4.3/nidmm/_converters.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    16344 2022-12-16 18:55:12.000000 nidmm-1.4.3/nidmm/_grpc_stub_interpreter.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    31587 2022-12-16 18:55:09.000000 nidmm-1.4.3/nidmm/_library.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    34303 2022-12-16 18:55:09.000000 nidmm-1.4.3/nidmm/_library_interpreter.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     1605 2022-12-16 18:55:09.000000 nidmm-1.4.3/nidmm/_library_singleton.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      659 2022-12-16 18:55:13.000000 nidmm-1.4.3/nidmm/_visatype.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8301 2022-12-16 18:55:08.000000 nidmm-1.4.3/nidmm/enums.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     4348 2022-12-16 18:55:10.000000 nidmm-1.4.3/nidmm/errors.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     3450 2022-12-16 18:55:12.000000 nidmm-1.4.3/nidmm/grpc_session_options.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     1895 2022-12-16 18:55:12.000000 nidmm-1.4.3/nidmm/nidevice_pb2.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      159 2022-12-16 18:55:12.000000 nidmm-1.4.3/nidmm/nidevice_pb2_grpc.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    81655 2022-12-16 18:55:12.000000 nidmm-1.4.3/nidmm/nidmm_pb2.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)   141552 2022-12-16 18:55:12.000000 nidmm-1.4.3/nidmm/nidmm_pb2_grpc.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)   126794 2022-12-16 18:55:10.000000 nidmm-1.4.3/nidmm/session.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     4196 2022-12-16 18:55:13.000000 nidmm-1.4.3/nidmm/session_pb2.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8907 2022-12-16 18:55:13.000000 nidmm-1.4.3/nidmm/session_pb2_grpc.py
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:02.815315 nidmm-1.4.3/nidmm.egg-info/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8737 2022-12-16 18:56:02.000000 nidmm-1.4.3/nidmm.egg-info/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      605 2022-12-16 18:56:02.000000 nidmm-1.4.3/nidmm.egg-info/SOURCES.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:02.000000 nidmm-1.4.3/nidmm.egg-info/dependency_links.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       65 2022-12-16 18:56:02.000000 nidmm-1.4.3/nidmm.egg-info/requires.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        6 2022-12-16 18:56:02.000000 nidmm-1.4.3/nidmm.egg-info/top_level.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:02.000000 nidmm-1.4.3/nidmm.egg-info/zip-safe
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       38 2022-12-16 18:56:02.825315 nidmm-1.4.3/setup.cfg
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     2033 2022-12-16 18:55:15.000000 nidmm-1.4.3/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:29.933237 nidmm-1.4.4/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8758 2023-04-14 16:08:29.931235 nidmm-1.4.4/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7774 2023-04-14 16:05:28.000000 nidmm-1.4.4/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:29.852233 nidmm-1.4.4/nidmm/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:05:18.000000 nidmm-1.4.4/nidmm/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3023 2023-04-14 16:05:16.000000 nidmm-1.4.4/nidmm/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5432 2023-04-14 16:05:09.000000 nidmm-1.4.4/nidmm/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13869 2023-04-14 16:05:17.000000 nidmm-1.4.4/nidmm/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    16344 2023-04-14 16:05:19.000000 nidmm-1.4.4/nidmm/_grpc_stub_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    31587 2023-04-14 16:05:10.000000 nidmm-1.4.4/nidmm/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    33945 2023-04-14 16:05:11.000000 nidmm-1.4.4/nidmm/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1605 2023-04-14 16:05:12.000000 nidmm-1.4.4/nidmm/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:05:22.000000 nidmm-1.4.4/nidmm/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8301 2023-04-14 16:05:10.000000 nidmm-1.4.4/nidmm/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4348 2023-04-14 16:05:14.000000 nidmm-1.4.4/nidmm/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3450 2023-04-14 16:05:19.000000 nidmm-1.4.4/nidmm/grpc_session_options.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-04-14 16:05:21.000000 nidmm-1.4.4/nidmm/nidevice_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-04-14 16:05:21.000000 nidmm-1.4.4/nidmm/nidevice_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    81655 2023-04-14 16:05:20.000000 nidmm-1.4.4/nidmm/nidmm_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   141552 2023-04-14 16:05:20.000000 nidmm-1.4.4/nidmm/nidmm_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   126794 2023-04-14 16:05:13.000000 nidmm-1.4.4/nidmm/session.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-04-14 16:05:22.000000 nidmm-1.4.4/nidmm/session_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-04-14 16:05:22.000000 nidmm-1.4.4/nidmm/session_pb2_grpc.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:29.919235 nidmm-1.4.4/nidmm.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8758 2023-04-14 16:08:29.000000 nidmm-1.4.4/nidmm.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      605 2023-04-14 16:08:29.000000 nidmm-1.4.4/nidmm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:08:29.000000 nidmm-1.4.4/nidmm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      154 2023-04-14 16:08:29.000000 nidmm-1.4.4/nidmm.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        6 2023-04-14 16:08:29.000000 nidmm-1.4.4/nidmm.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:08:29.000000 nidmm-1.4.4/nidmm.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:08:29.934235 nidmm-1.4.4/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2188 2023-04-14 16:05:29.000000 nidmm-1.4.4/setup.py
```

### Comparing `nidmm-1.4.3/PKG-INFO` & `nidmm-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nidmm
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI-DMM Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Description-Content-Type: text/x-rst
+Provides-Extra: grpc
 
 Overall Status
 --------------
 
 +----------------------+------------------------------------------------------------------------------------------------------------------------------------+
 | master branch status | |BuildStatus| |Docs| |MITLicense| |CoverageStatus|                                                                                 |
 +----------------------+------------------------------------------------------------------------------------------------------------------------------------+
@@ -93,15 +94,15 @@
 
 NI-DMM Python API Status
 ------------------------
 
 +-------------------------------+----------------------+
 | NI-DMM (nidmm)                |                      |
 +===============================+======================+
-| Driver Version Tested Against | 2022 Q3              |
+| Driver Version Tested Against | 2023 Q1.1            |
 +-------------------------------+----------------------+
 | PyPI Version                  | |nidmmLatestVersion| |
 +-------------------------------+----------------------+
 | Supported Python Version      | |nidmmPythonVersion| |
 +-------------------------------+----------------------+
 | Open Issues                   | |nidmmOpenIssues|    |
 +-------------------------------+----------------------+
@@ -135,15 +136,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nidmm module, you must install the NI-DMM runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-DMM**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nidmm~=1.4.3
+  $ python -m pip install nidmm~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install nidmm
```

### Comparing `nidmm-1.4.3/README.rst` & `nidmm-1.4.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 NI-DMM Python API Status
 ------------------------
 
 +-------------------------------+----------------------+
 | NI-DMM (nidmm)                |                      |
 +===============================+======================+
-| Driver Version Tested Against | 2022 Q3              |
+| Driver Version Tested Against | 2023 Q1.1            |
 +-------------------------------+----------------------+
 | PyPI Version                  | |nidmmLatestVersion| |
 +-------------------------------+----------------------+
 | Supported Python Version      | |nidmmPythonVersion| |
 +-------------------------------+----------------------+
 | Open Issues                   | |nidmmOpenIssues|    |
 +-------------------------------+----------------------+
@@ -98,32 +98,32 @@
 
 
 .. |nidmmOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/nidmm.svg
     :alt: Pull Requests for NI-DMM
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Anidmm
 
 
-
-.. _nidmm_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the nidmm module, you must install the NI-DMM runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI-DMM**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install nidmm~=1.4.3
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nidmm
-
-
+
+.. _nidmm_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the nidmm module, you must install the NI-DMM runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI-DMM**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install nidmm~=1.4.4
+
+Or **easy_install** from
+`setuptools <http://pypi.python.org/pypi/setuptools>`_::
+
+  $ python -m easy_install nidmm
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -135,36 +135,36 @@
     import nidmm
     with nidmm.Session("Dev1") as session:
         session.configureMeasurementDigits(nidmm.Function.DC_VOLTS, 10, 5.5)
         print("Measurement: " + str(session.read()))
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nidmm/examples>`_
 
-.. _support-section:
-
-Support / Feedback
-==================
-
-The packages included in **nimi-python** package are supported by NI. For support, open
-a request through the NI support portal at `ni.com <http://www.ni.com>`_.
-
-.. _bugs-section:
-
-Bugs / Feature Requests
-=======================
-
-To report a bug or submit a feature request specific to NI Modular Instruments Python bindings (nimi-python), please use the
-`GitHub issues page <https://github.com/ni/nimi-python/issues>`_.
-
-Fill in the issue template as completely as possible and we will respond as soon
-as we can.
-
-For hardware support or any other questions not specific to this GitHub project, please visit `NI Community Forums <https://forums.ni.com/>`_.
-
-
+.. _support-section:
+
+Support / Feedback
+==================
+
+The packages included in **nimi-python** package are supported by NI. For support, open
+a request through the NI support portal at `ni.com <http://www.ni.com>`_.
+
+.. _bugs-section:
+
+Bugs / Feature Requests
+=======================
+
+To report a bug or submit a feature request specific to NI Modular Instruments Python bindings (nimi-python), please use the
+`GitHub issues page <https://github.com/ni/nimi-python/issues>`_.
+
+Fill in the issue template as completely as possible and we will respond as soon
+as we can.
+
+For hardware support or any other questions not specific to this GitHub project, please visit `NI Community Forums <https://forums.ni.com/>`_.
+
+
 .. _documentation-section:
 
 Documentation
 =============
 
 Documentation is available `here <http://nimi-python.readthedocs.io>`_.
```

### Comparing `nidmm-1.4.3/nidmm/__init__.py` & `nidmm-1.4.4/nidmm/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.3'
+__version__ = '1.4.4'
 
 from nidmm.enums import *  # noqa: F403,F401,H303
 from nidmm.errors import DriverWarning  # noqa: F401
 from nidmm.errors import Error  # noqa: F401
 from nidmm.grpc_session_options import *  # noqa: F403,F401,H303
 from nidmm.session import Session  # noqa: F401
 
@@ -61,15 +61,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-DMM"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nidmm'
-    info['module']['version'] = "1.4.3"
+    info['module']['version'] = "1.4.4"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nidmm-1.4.3/nidmm/_attributes.py` & `nidmm-1.4.4/nidmm/_attributes.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/nidmm/_converters.py` & `nidmm-1.4.4/nidmm/_converters.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/nidmm/_grpc_stub_interpreter.py` & `nidmm-1.4.4/nidmm/_grpc_stub_interpreter.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/nidmm/_library.py` & `nidmm-1.4.4/nidmm/_library.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/nidmm/_library_interpreter.py` & `nidmm-1.4.4/nidmm/_library_interpreter.py`

 * *Files 5% similar despite different names*

```diff
@@ -373,18 +373,17 @@
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         error_code = self._library.niDMM_Initiate(vi_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
     def lock(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
-        caller_has_lock_ctype = _visatype.ViBoolean()  # case S220
-        error_code = self._library.niDMM_LockSession(vi_ctype, None if caller_has_lock_ctype is None else (ctypes.pointer(caller_has_lock_ctype)))
+        error_code = self._library.niDMM_LockSession(vi_ctype, None)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
-        return bool(caller_has_lock_ctype.value)
+        return
 
     def perform_open_cable_comp(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         conductance_ctype = _visatype.ViReal64()  # case S220
         susceptance_ctype = _visatype.ViReal64()  # case S220
         error_code = self._library.niDMM_PerformOpenCableComp(vi_ctype, None if conductance_ctype is None else (ctypes.pointer(conductance_ctype)), None if susceptance_ctype is None else (ctypes.pointer(susceptance_ctype)))
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
@@ -490,18 +489,17 @@
         attribute_value_ctype = ctypes.create_string_buffer(attribute_value.encode(self._encoding))  # case C020
         error_code = self._library.niDMM_SetAttributeViString(vi_ctype, channel_name_ctype, attribute_id_ctype, attribute_value_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
     def unlock(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
-        caller_has_lock_ctype = _visatype.ViBoolean()  # case S220
-        error_code = self._library.niDMM_UnlockSession(vi_ctype, None if caller_has_lock_ctype is None else (ctypes.pointer(caller_has_lock_ctype)))
+        error_code = self._library.niDMM_UnlockSession(vi_ctype, None)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
-        return bool(caller_has_lock_ctype.value)
+        return
 
     def close(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         error_code = self._library.niDMM_close(vi_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
```

### Comparing `nidmm-1.4.3/nidmm/_library_singleton.py` & `nidmm-1.4.4/nidmm/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/nidmm/enums.py` & `nidmm-1.4.4/nidmm/enums.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/nidmm/errors.py` & `nidmm-1.4.4/nidmm/errors.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/nidmm/grpc_session_options.py` & `nidmm-1.4.4/nidmm/grpc_session_options.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/nidmm/nidevice_pb2.py` & `nidmm-1.4.4/nidmm/nidevice_pb2.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/nidmm/nidmm_pb2.py` & `nidmm-1.4.4/nidmm/nidmm_pb2.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/nidmm/nidmm_pb2_grpc.py` & `nidmm-1.4.4/nidmm/nidmm_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/nidmm/session.py` & `nidmm-1.4.4/nidmm/session.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/nidmm/session_pb2.py` & `nidmm-1.4.4/nidmm/session_pb2.py`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/nidmm/session_pb2_grpc.py` & `nidmm-1.4.4/nidmm/session_pb2_grpc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -41,44 +41,44 @@
                 )
 
 
 class SessionUtilitiesServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def EnumerateDevices(self, request, context):
-        """Provides a list of devices or chassis connected to server under localhost
+        """Provides a list of devices or chassis connected to server under localhost
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Reserve(self, request, context):
-        """Reserve a set of client defined resources for exclusive use
+        """Reserve a set of client defined resources for exclusive use
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def IsReservedByClient(self, request, context):
-        """Determines if a set of client defined resources is currently reserved by a
-        specific client
+        """Determines if a set of client defined resources is currently reserved by a
+        specific client
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Unreserve(self, request, context):
-        """Unreserves a previously reserved resource
+        """Unreserves a previously reserved resource
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ResetServer(self, request, context):
-        """Resets the server to a default state with no open sessions
+        """Resets the server to a default state with no open sessions
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_SessionUtilitiesServicer_to_server(servicer, server):
```

### Comparing `nidmm-1.4.3/nidmm.egg-info/PKG-INFO` & `nidmm-1.4.4/nidmm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nidmm
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI-DMM Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Description-Content-Type: text/x-rst
+Provides-Extra: grpc
 
 Overall Status
 --------------
 
 +----------------------+------------------------------------------------------------------------------------------------------------------------------------+
 | master branch status | |BuildStatus| |Docs| |MITLicense| |CoverageStatus|                                                                                 |
 +----------------------+------------------------------------------------------------------------------------------------------------------------------------+
@@ -93,15 +94,15 @@
 
 NI-DMM Python API Status
 ------------------------
 
 +-------------------------------+----------------------+
 | NI-DMM (nidmm)                |                      |
 +===============================+======================+
-| Driver Version Tested Against | 2022 Q3              |
+| Driver Version Tested Against | 2023 Q1.1            |
 +-------------------------------+----------------------+
 | PyPI Version                  | |nidmmLatestVersion| |
 +-------------------------------+----------------------+
 | Supported Python Version      | |nidmmPythonVersion| |
 +-------------------------------+----------------------+
 | Open Issues                   | |nidmmOpenIssues|    |
 +-------------------------------+----------------------+
@@ -135,15 +136,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nidmm module, you must install the NI-DMM runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-DMM**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nidmm~=1.4.3
+  $ python -m pip install nidmm~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install nidmm
```

### Comparing `nidmm-1.4.3/nidmm.egg-info/SOURCES.txt` & `nidmm-1.4.4/nidmm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nidmm-1.4.3/setup.py` & `nidmm-1.4.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,32 +25,37 @@
     with open(file_to_read, 'r') as f:
         return f.read()
 
 
 setup(
     name=pypi_name,
     zip_safe=True,
-    version='1.4.3',
+    version='1.4.4',
     description='NI-DMM Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
     maintainer_email="opensource@ni.com",
     keywords=['nidmm'],
     license='MIT',
     include_package_data=True,
     packages=['nidmm'],
     install_requires=[
-        'enum34;python_version<"3.4"',
-        'singledispatch;python_version<"3.4"',
         'hightime>=0.2.0',
     ],
+    extras_require={
+        'grpc': [
+            'grpcio>=1.49.1,<2.0,!=1.53;python_version=="3.7"',  # no 32-bit wheel for 1.53.0
+            'grpcio>=1.49.1,<2.0;python_version>"3.7"',
+            'protobuf>=4.21,<5.0'
+        ],
+    },
     setup_requires=['pytest-runner', ],
     tests_require=['pytest'],
     test_suite='tests',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Manufacturing",
```

