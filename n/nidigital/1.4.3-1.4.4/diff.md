# Comparing `tmp/nidigital-1.4.3.tar.gz` & `tmp/nidigital-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nidigital-1.4.3.tar", last modified: Fri Dec 16 18:56:01 2022, max compression
+gzip compressed data, was "nidigital-1.4.4.tar", last modified: Fri Apr 14 16:08:03 2023, max compression
```

## Comparing `nidigital-1.4.3.tar` & `nidigital-1.4.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:01.225315 nidigital-1.4.3/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    10535 2022-12-16 18:56:01.225315 nidigital-1.4.3/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     9505 2022-12-16 18:55:07.000000 nidigital-1.4.3/README.rst
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:01.225315 nidigital-1.4.3/nidigital/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        7 2022-12-16 18:55:02.000000 nidigital-1.4.3/nidigital/VERSION
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     3179 2022-12-16 18:55:01.000000 nidigital-1.4.3/nidigital/__init__.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     5448 2022-12-16 18:54:56.000000 nidigital-1.4.3/nidigital/_attributes.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    13877 2022-12-16 18:55:01.000000 nidigital-1.4.3/nidigital/_converters.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    29543 2022-12-16 18:55:02.000000 nidigital-1.4.3/nidigital/_grpc_stub_interpreter.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    65575 2022-12-16 18:54:58.000000 nidigital-1.4.3/nidigital/_library.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    73909 2022-12-16 18:54:58.000000 nidigital-1.4.3/nidigital/_library_interpreter.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     1629 2022-12-16 18:54:59.000000 nidigital-1.4.3/nidigital/_library_singleton.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      659 2022-12-16 18:55:03.000000 nidigital-1.4.3/nidigital/_visatype.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     7810 2022-12-16 18:54:57.000000 nidigital-1.4.3/nidigital/enums.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     4512 2022-12-16 18:55:00.000000 nidigital-1.4.3/nidigital/errors.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     3458 2022-12-16 18:55:02.000000 nidigital-1.4.3/nidigital/grpc_session_options.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     2890 2022-12-16 18:55:03.000000 nidigital-1.4.3/nidigital/history_ram_cycle_information.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     1895 2022-12-16 18:55:03.000000 nidigital-1.4.3/nidigital/nidevice_pb2.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      159 2022-12-16 18:55:03.000000 nidigital-1.4.3/nidigital/nidevice_pb2_grpc.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)   105590 2022-12-16 18:55:03.000000 nidigital-1.4.3/nidigital/nidigitalpattern_pb2.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)   226597 2022-12-16 18:55:03.000000 nidigital-1.4.3/nidigital/nidigitalpattern_pb2_grpc.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)   234062 2022-12-16 18:54:59.000000 nidigital-1.4.3/nidigital/session.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     4196 2022-12-16 18:55:03.000000 nidigital-1.4.3/nidigital/session_pb2.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8907 2022-12-16 18:55:03.000000 nidigital-1.4.3/nidigital/session_pb2_grpc.py
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:01.225315 nidigital-1.4.3/nidigital.egg-info/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    10535 2022-12-16 18:56:01.000000 nidigital-1.4.3/nidigital.egg-info/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      770 2022-12-16 18:56:01.000000 nidigital-1.4.3/nidigital.egg-info/SOURCES.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:01.000000 nidigital-1.4.3/nidigital.egg-info/dependency_links.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       72 2022-12-16 18:56:01.000000 nidigital-1.4.3/nidigital.egg-info/requires.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       10 2022-12-16 18:56:01.000000 nidigital-1.4.3/nidigital.egg-info/top_level.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:01.000000 nidigital-1.4.3/nidigital.egg-info/zip-safe
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       38 2022-12-16 18:56:01.225315 nidigital-1.4.3/setup.cfg
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     2082 2022-12-16 18:55:07.000000 nidigital-1.4.3/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:14.106667 nidigital-1.4.4/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10556 2023-04-14 16:08:14.104666 nidigital-1.4.4/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     9545 2023-04-14 16:05:06.000000 nidigital-1.4.4/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:14.025665 nidigital-1.4.4/nidigital/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:04:52.000000 nidigital-1.4.4/nidigital/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3179 2023-04-14 16:04:50.000000 nidigital-1.4.4/nidigital/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5448 2023-04-14 16:04:42.000000 nidigital-1.4.4/nidigital/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13877 2023-04-14 16:04:51.000000 nidigital-1.4.4/nidigital/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    29543 2023-04-14 16:04:53.000000 nidigital-1.4.4/nidigital/_grpc_stub_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    65575 2023-04-14 16:04:43.000000 nidigital-1.4.4/nidigital/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    73551 2023-04-14 16:04:44.000000 nidigital-1.4.4/nidigital/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1629 2023-04-14 16:04:45.000000 nidigital-1.4.4/nidigital/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:04:57.000000 nidigital-1.4.4/nidigital/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7810 2023-04-14 16:04:42.000000 nidigital-1.4.4/nidigital/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4512 2023-04-14 16:04:47.000000 nidigital-1.4.4/nidigital/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3465 2023-04-14 16:04:54.000000 nidigital-1.4.4/nidigital/grpc_session_options.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2890 2023-04-14 16:04:57.000000 nidigital-1.4.4/nidigital/history_ram_cycle_information.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-04-14 16:04:56.000000 nidigital-1.4.4/nidigital/nidevice_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-04-14 16:04:56.000000 nidigital-1.4.4/nidigital/nidevice_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   105590 2023-04-14 16:04:55.000000 nidigital-1.4.4/nidigital/nidigitalpattern_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   226597 2023-04-14 16:04:55.000000 nidigital-1.4.4/nidigital/nidigitalpattern_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   234062 2023-04-14 16:04:47.000000 nidigital-1.4.4/nidigital/session.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-04-14 16:04:57.000000 nidigital-1.4.4/nidigital/session_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-04-14 16:04:57.000000 nidigital-1.4.4/nidigital/session_pb2_grpc.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:14.092666 nidigital-1.4.4/nidigital.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10556 2023-04-14 16:08:13.000000 nidigital-1.4.4/nidigital.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      770 2023-04-14 16:08:13.000000 nidigital-1.4.4/nidigital.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:08:13.000000 nidigital-1.4.4/nidigital.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      161 2023-04-14 16:08:13.000000 nidigital-1.4.4/nidigital.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       10 2023-04-14 16:08:13.000000 nidigital-1.4.4/nidigital.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:08:13.000000 nidigital-1.4.4/nidigital.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:08:14.107666 nidigital-1.4.4/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2237 2023-04-14 16:05:07.000000 nidigital-1.4.4/setup.py
```

### Comparing `nidigital-1.4.3/PKG-INFO` & `nidigital-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nidigital
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI-Digital Pattern Driver Python API
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
 
 NI-Digital Pattern Driver Python API Status
 -------------------------------------------
 
 +---------------------------------------+--------------------------+
 | NI-Digital Pattern Driver (nidigital) |                          |
 +=======================================+==========================+
-| Driver Version Tested Against         | 2022 Q4                  |
+| Driver Version Tested Against         | 2023 Q2                  |
 +---------------------------------------+--------------------------+
 | PyPI Version                          | |nidigitalLatestVersion| |
 +---------------------------------------+--------------------------+
 | Supported Python Version              | |nidigitalPythonVersion| |
 +---------------------------------------+--------------------------+
 | Open Issues                           | |nidigitalOpenIssues|    |
 +---------------------------------------+--------------------------+
@@ -135,15 +136,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nidigital module, you must install the NI-Digital Pattern Driver runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-Digital Pattern Driver**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nidigital~=1.4.3
+  $ python -m pip install nidigital~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install nidigital
```

### Comparing `nidigital-1.4.3/README.rst` & `nidigital-1.4.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 NI-Digital Pattern Driver Python API Status
 -------------------------------------------
 
 +---------------------------------------+--------------------------+
 | NI-Digital Pattern Driver (nidigital) |                          |
 +=======================================+==========================+
-| Driver Version Tested Against         | 2022 Q4                  |
+| Driver Version Tested Against         | 2023 Q2                  |
 +---------------------------------------+--------------------------+
 | PyPI Version                          | |nidigitalLatestVersion| |
 +---------------------------------------+--------------------------+
 | Supported Python Version              | |nidigitalPythonVersion| |
 +---------------------------------------+--------------------------+
 | Open Issues                           | |nidigitalOpenIssues|    |
 +---------------------------------------+--------------------------+
@@ -98,32 +98,32 @@
 
 
 .. |nidigitalOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/nidigital.svg
     :alt: Pull Requests for NI-Digital Pattern Driver
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Anidigital
 
 
-
-.. _nidigital_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the nidigital module, you must install the NI-Digital Pattern Driver runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI-Digital Pattern Driver**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install nidigital~=1.4.3
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nidigital
-
-
+
+.. _nidigital_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the nidigital module, you must install the NI-Digital Pattern Driver runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI-Digital Pattern Driver**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install nidigital~=1.4.4
+
+Or **easy_install** from
+`setuptools <http://pypi.python.org/pypi/setuptools>`_::
+
+  $ python -m easy_install nidigital
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -166,36 +166,36 @@
             print('{:<20} {:<10f} {:<10f}'.format(channel, current, voltage))
 
         # Disconnect all channels using programmable onboard switching
         session.channels[channels].selected_function = nidigital.SelectedFunction.DISCONNECT
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nidigital/examples>`_
 
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

### Comparing `nidigital-1.4.3/nidigital/__init__.py` & `nidigital-1.4.4/nidigital/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.3'
+__version__ = '1.4.4'
 
 from nidigital.enums import *  # noqa: F403,F401,H303
 from nidigital.errors import DriverWarning  # noqa: F401
 from nidigital.errors import Error  # noqa: F401
 from nidigital.grpc_session_options import *  # noqa: F403,F401,H303
 from nidigital.session import Session  # noqa: F401
 
@@ -63,15 +63,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-Digital Pattern Driver"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nidigital'
-    info['module']['version'] = "1.4.3"
+    info['module']['version'] = "1.4.4"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nidigital-1.4.3/nidigital/_attributes.py` & `nidigital-1.4.4/nidigital/_attributes.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/nidigital/_converters.py` & `nidigital-1.4.4/nidigital/_converters.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/nidigital/_grpc_stub_interpreter.py` & `nidigital-1.4.4/nidigital/_grpc_stub_interpreter.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/nidigital/_library.py` & `nidigital-1.4.4/nidigital/_library.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/nidigital/_library_interpreter.py` & `nidigital-1.4.4/nidigital/_library_interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -743,18 +743,17 @@
         file_path_ctype = ctypes.create_string_buffer(file_path.encode(self._encoding))  # case C020
         error_code = self._library.niDigital_LoadTiming(vi_ctype, file_path_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
     def lock(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
-        caller_has_lock_ctype = _visatype.ViBoolean()  # case S220
-        error_code = self._library.niDigital_LockSession(vi_ctype, None if caller_has_lock_ctype is None else (ctypes.pointer(caller_has_lock_ctype)))
+        error_code = self._library.niDigital_LockSession(vi_ctype, None)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
-        return bool(caller_has_lock_ctype.value)
+        return
 
     def ppmu_measure(self, channel_list, measurement_type):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         channel_list_ctype = ctypes.create_string_buffer(channel_list.encode(self._encoding))  # case C010
         measurement_type_ctype = _visatype.ViInt32(measurement_type.value)  # case S130
         buffer_size_ctype = _visatype.ViInt32(0)  # case S190
         measurements_ctype = None  # case B610
@@ -899,18 +898,17 @@
         file_path_ctype = ctypes.create_string_buffer(file_path.encode(self._encoding))  # case C020
         error_code = self._library.niDigital_UnloadSpecifications(vi_ctype, file_path_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
     def unlock(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
-        caller_has_lock_ctype = _visatype.ViBoolean()  # case S220
-        error_code = self._library.niDigital_UnlockSession(vi_ctype, None if caller_has_lock_ctype is None else (ctypes.pointer(caller_has_lock_ctype)))
+        error_code = self._library.niDigital_UnlockSession(vi_ctype, None)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
-        return bool(caller_has_lock_ctype.value)
+        return
 
     def wait_until_done(self, timeout):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         timeout_ctype = _visatype.ViReal64(timeout)  # case S150
         error_code = self._library.niDigital_WaitUntilDone(vi_ctype, timeout_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
```

### Comparing `nidigital-1.4.3/nidigital/_library_singleton.py` & `nidigital-1.4.4/nidigital/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/nidigital/enums.py` & `nidigital-1.4.4/nidigital/enums.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/nidigital/errors.py` & `nidigital-1.4.4/nidigital/errors.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/nidigital/grpc_session_options.py` & `nidigital-1.4.4/nidigital/grpc_session_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file was generated
 
 from enum import IntEnum
 
 
 # This constant specifies the gRPC package and service used by this API.
 # Customers can pass this value to the MeasurementLink discovery service to resolve the server instance that provides this interface.
-GRPC_SERVICE_INTERFACE_NAME = 'nidigital_grpc.NiDigital'
+GRPC_SERVICE_INTERFACE_NAME = 'nidigitalpattern_grpc.NiDigital'
 
 # This constant specifies the API license key required by the NI gRPC Device Server that comes with
 # MeasurementLink 2023 Q1.
 MEASUREMENTLINK_23Q1_NIMI_PYTHON_API_KEY = 'DE10751B-3EE0-44EC-A93B-800E6A3C89E4'
 
 
 class SessionInitializationBehavior(IntEnum):
```

### Comparing `nidigital-1.4.3/nidigital/history_ram_cycle_information.py` & `nidigital-1.4.4/nidigital/history_ram_cycle_information.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/nidigital/nidevice_pb2.py` & `nidigital-1.4.4/nidigital/nidevice_pb2.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/nidigital/nidigitalpattern_pb2.py` & `nidigital-1.4.4/nidigital/nidigitalpattern_pb2.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/nidigital/nidigitalpattern_pb2_grpc.py` & `nidigital-1.4.4/nidigital/nidigitalpattern_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/nidigital/session.py` & `nidigital-1.4.4/nidigital/session.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/nidigital/session_pb2.py` & `nidigital-1.4.4/nidigital/session_pb2.py`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/nidigital/session_pb2_grpc.py` & `nidigital-1.4.4/nidigital/session_pb2_grpc.py`

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

### Comparing `nidigital-1.4.3/nidigital.egg-info/PKG-INFO` & `nidigital-1.4.4/nidigital.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nidigital
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI-Digital Pattern Driver Python API
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
 
 NI-Digital Pattern Driver Python API Status
 -------------------------------------------
 
 +---------------------------------------+--------------------------+
 | NI-Digital Pattern Driver (nidigital) |                          |
 +=======================================+==========================+
-| Driver Version Tested Against         | 2022 Q4                  |
+| Driver Version Tested Against         | 2023 Q2                  |
 +---------------------------------------+--------------------------+
 | PyPI Version                          | |nidigitalLatestVersion| |
 +---------------------------------------+--------------------------+
 | Supported Python Version              | |nidigitalPythonVersion| |
 +---------------------------------------+--------------------------+
 | Open Issues                           | |nidigitalOpenIssues|    |
 +---------------------------------------+--------------------------+
@@ -135,15 +136,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nidigital module, you must install the NI-Digital Pattern Driver runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-Digital Pattern Driver**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nidigital~=1.4.3
+  $ python -m pip install nidigital~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install nidigital
```

### Comparing `nidigital-1.4.3/nidigital.egg-info/SOURCES.txt` & `nidigital-1.4.4/nidigital.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nidigital-1.4.3/setup.py` & `nidigital-1.4.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,33 +25,38 @@
     with open(file_to_read, 'r') as f:
         return f.read()
 
 
 setup(
     name=pypi_name,
     zip_safe=True,
-    version='1.4.3',
+    version='1.4.4',
     description='NI-Digital Pattern Driver Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
     maintainer_email="opensource@ni.com",
     keywords=['nidigital'],
     license='MIT',
     include_package_data=True,
     packages=['nidigital'],
     install_requires=[
-        'enum34;python_version<"3.4"',
-        'singledispatch;python_version<"3.4"',
         'hightime>=0.2.0',
         'nitclk',
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

