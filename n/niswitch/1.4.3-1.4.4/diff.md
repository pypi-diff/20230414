# Comparing `tmp/niswitch-1.4.3.tar.gz` & `tmp/niswitch-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niswitch-1.4.3.tar", last modified: Fri Dec 16 18:56:07 2022, max compression
+gzip compressed data, was "niswitch-1.4.4.tar", last modified: Fri Apr 14 16:09:08 2023, max compression
```

## Comparing `niswitch-1.4.3.tar` & `niswitch-1.4.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:07.595315 niswitch-1.4.3/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8740 2022-12-16 18:56:07.595315 niswitch-1.4.3/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     7728 2022-12-16 18:55:44.000000 niswitch-1.4.3/README.rst
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:07.595315 niswitch-1.4.3/niswitch/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        7 2022-12-16 18:55:41.000000 niswitch-1.4.3/niswitch/VERSION
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     3047 2022-12-16 18:55:40.000000 niswitch-1.4.3/niswitch/__init__.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     5444 2022-12-16 18:55:38.000000 niswitch-1.4.3/niswitch/_attributes.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    13875 2022-12-16 18:55:41.000000 niswitch-1.4.3/niswitch/_converters.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    12650 2022-12-16 18:55:41.000000 niswitch-1.4.3/niswitch/_grpc_stub_interpreter.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    24762 2022-12-16 18:55:38.000000 niswitch-1.4.3/niswitch/_library.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    25697 2022-12-16 18:55:39.000000 niswitch-1.4.3/niswitch/_library_interpreter.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     1623 2022-12-16 18:55:39.000000 niswitch-1.4.3/niswitch/_library_singleton.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      659 2022-12-16 18:55:42.000000 niswitch-1.4.3/niswitch/_visatype.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    13707 2022-12-16 18:55:38.000000 niswitch-1.4.3/niswitch/enums.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     4381 2022-12-16 18:55:40.000000 niswitch-1.4.3/niswitch/errors.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     3456 2022-12-16 18:55:41.000000 niswitch-1.4.3/niswitch/grpc_session_options.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     1895 2022-12-16 18:55:42.000000 niswitch-1.4.3/niswitch/nidevice_pb2.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      159 2022-12-16 18:55:42.000000 niswitch-1.4.3/niswitch/nidevice_pb2_grpc.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    55730 2022-12-16 18:55:42.000000 niswitch-1.4.3/niswitch/niswitch_pb2.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    96817 2022-12-16 18:55:42.000000 niswitch-1.4.3/niswitch/niswitch_pb2_grpc.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)   114951 2022-12-16 18:55:39.000000 niswitch-1.4.3/niswitch/session.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     4196 2022-12-16 18:55:42.000000 niswitch-1.4.3/niswitch/session_pb2.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8907 2022-12-16 18:55:42.000000 niswitch-1.4.3/niswitch/session_pb2_grpc.py
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:07.595315 niswitch-1.4.3/niswitch.egg-info/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8740 2022-12-16 18:56:07.000000 niswitch-1.4.3/niswitch.egg-info/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      686 2022-12-16 18:56:07.000000 niswitch-1.4.3/niswitch.egg-info/SOURCES.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:07.000000 niswitch-1.4.3/niswitch.egg-info/dependency_links.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       65 2022-12-16 18:56:07.000000 niswitch-1.4.3/niswitch.egg-info/requires.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        9 2022-12-16 18:56:07.000000 niswitch-1.4.3/niswitch.egg-info/top_level.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:07.000000 niswitch-1.4.3/niswitch.egg-info/zip-safe
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       38 2022-12-16 18:56:07.595315 niswitch-1.4.3/setup.cfg
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     2045 2022-12-16 18:55:45.000000 niswitch-1.4.3/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:18.410721 niswitch-1.4.4/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8761 2023-04-14 16:09:18.408721 niswitch-1.4.4/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7768 2023-04-14 16:06:40.000000 niswitch-1.4.4/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:18.324720 niswitch-1.4.4/niswitch/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:06:29.000000 niswitch-1.4.4/niswitch/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3047 2023-04-14 16:06:27.000000 niswitch-1.4.4/niswitch/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5444 2023-04-14 16:06:20.000000 niswitch-1.4.4/niswitch/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13875 2023-04-14 16:06:28.000000 niswitch-1.4.4/niswitch/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12650 2023-04-14 16:06:30.000000 niswitch-1.4.4/niswitch/_grpc_stub_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    24762 2023-04-14 16:06:22.000000 niswitch-1.4.4/niswitch/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    25339 2023-04-14 16:06:23.000000 niswitch-1.4.4/niswitch/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1623 2023-04-14 16:06:24.000000 niswitch-1.4.4/niswitch/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:06:33.000000 niswitch-1.4.4/niswitch/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13707 2023-04-14 16:06:21.000000 niswitch-1.4.4/niswitch/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4381 2023-04-14 16:06:25.000000 niswitch-1.4.4/niswitch/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3456 2023-04-14 16:06:31.000000 niswitch-1.4.4/niswitch/grpc_session_options.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-04-14 16:06:32.000000 niswitch-1.4.4/niswitch/nidevice_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-04-14 16:06:32.000000 niswitch-1.4.4/niswitch/nidevice_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    55730 2023-04-14 16:06:31.000000 niswitch-1.4.4/niswitch/niswitch_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    96817 2023-04-14 16:06:31.000000 niswitch-1.4.4/niswitch/niswitch_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   114951 2023-04-14 16:06:24.000000 niswitch-1.4.4/niswitch/session.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-04-14 16:06:33.000000 niswitch-1.4.4/niswitch/session_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-04-14 16:06:33.000000 niswitch-1.4.4/niswitch/session_pb2_grpc.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:18.396722 niswitch-1.4.4/niswitch.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8761 2023-04-14 16:09:17.000000 niswitch-1.4.4/niswitch.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      686 2023-04-14 16:09:18.000000 niswitch-1.4.4/niswitch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:17.000000 niswitch-1.4.4/niswitch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      154 2023-04-14 16:09:17.000000 niswitch-1.4.4/niswitch.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:09:17.000000 niswitch-1.4.4/niswitch.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:17.000000 niswitch-1.4.4/niswitch.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:09:18.410721 niswitch-1.4.4/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2200 2023-04-14 16:06:40.000000 niswitch-1.4.4/setup.py
```

### Comparing `niswitch-1.4.3/PKG-INFO` & `niswitch-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niswitch
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI-SWITCH Python API
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
 
 NI-SWITCH Python API Status
 ---------------------------
 
 +-------------------------------+-------------------------+
 | NI-SWITCH (niswitch)          |                         |
 +===============================+=========================+
-| Driver Version Tested Against | 2022 Q4                 |
+| Driver Version Tested Against | 2023 Q1                 |
 +-------------------------------+-------------------------+
 | PyPI Version                  | |niswitchLatestVersion| |
 +-------------------------------+-------------------------+
 | Supported Python Version      | |niswitchPythonVersion| |
 +-------------------------------+-------------------------+
 | Open Issues                   | |niswitchOpenIssues|    |
 +-------------------------------+-------------------------+
@@ -135,15 +136,15 @@
 Installation
 ------------
 
 As a prerequisite to using the niswitch module, you must install the NI-SWITCH runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-SWITCH**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install niswitch~=1.4.3
+  $ python -m pip install niswitch~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install niswitch
```

### Comparing `niswitch-1.4.3/README.rst` & `niswitch-1.4.4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 NI-SWITCH Python API Status
 ---------------------------
 
 +-------------------------------+-------------------------+
 | NI-SWITCH (niswitch)          |                         |
 +===============================+=========================+
-| Driver Version Tested Against | 2022 Q4                 |
+| Driver Version Tested Against | 2023 Q1                 |
 +-------------------------------+-------------------------+
 | PyPI Version                  | |niswitchLatestVersion| |
 +-------------------------------+-------------------------+
 | Supported Python Version      | |niswitchPythonVersion| |
 +-------------------------------+-------------------------+
 | Open Issues                   | |niswitchOpenIssues|    |
 +-------------------------------+-------------------------+
@@ -98,32 +98,32 @@
 
 
 .. |niswitchOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/niswitch.svg
     :alt: Pull Requests for NI-SWITCH
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Aniswitch
 
 
-
-.. _niswitch_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the niswitch module, you must install the NI-SWITCH runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI-SWITCH**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install niswitch~=1.4.3
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install niswitch
-
-
+
+.. _niswitch_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the niswitch module, you must install the NI-SWITCH runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI-SWITCH**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install niswitch~=1.4.4
+
+Or **easy_install** from
+`setuptools <http://pypi.python.org/pypi/setuptools>`_::
+
+  $ python -m easy_install niswitch
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -134,36 +134,36 @@
 
     import niswitch
     with niswitch.Session("Dev1") as session:
         session.connect(channel1='r0', channel2='c0')
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/niswitch/examples>`_
 
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

### Comparing `niswitch-1.4.3/niswitch/__init__.py` & `niswitch-1.4.4/niswitch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.3'
+__version__ = '1.4.4'
 
 from niswitch.enums import *  # noqa: F403,F401,H303
 from niswitch.errors import DriverWarning  # noqa: F401
 from niswitch.errors import Error  # noqa: F401
 from niswitch.grpc_session_options import *  # noqa: F403,F401,H303
 from niswitch.session import Session  # noqa: F401
 
@@ -61,15 +61,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-SWITCH"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'niswitch'
-    info['module']['version'] = "1.4.3"
+    info['module']['version'] = "1.4.4"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `niswitch-1.4.3/niswitch/_attributes.py` & `niswitch-1.4.4/niswitch/_attributes.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/niswitch/_converters.py` & `niswitch-1.4.4/niswitch/_converters.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/niswitch/_grpc_stub_interpreter.py` & `niswitch-1.4.4/niswitch/_grpc_stub_interpreter.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/niswitch/_library.py` & `niswitch-1.4.4/niswitch/_library.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/niswitch/_library_interpreter.py` & `niswitch-1.4.4/niswitch/_library_interpreter.py`

 * *Files 3% similar despite different names*

```diff
@@ -279,18 +279,17 @@
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         error_code = self._library.niSwitch_InitiateScan(vi_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
     def lock(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
-        caller_has_lock_ctype = _visatype.ViBoolean()  # case S220
-        error_code = self._library.niSwitch_LockSession(vi_ctype, None if caller_has_lock_ctype is None else (ctypes.pointer(caller_has_lock_ctype)))
+        error_code = self._library.niSwitch_LockSession(vi_ctype, None)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
-        return bool(caller_has_lock_ctype.value)
+        return
 
     def relay_control(self, relay_name, relay_action):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         relay_name_ctype = ctypes.create_string_buffer(relay_name.encode(self._encoding))  # case C020
         relay_action_ctype = _visatype.ViInt32(relay_action.value)  # case S130
         error_code = self._library.niSwitch_RelayControl(vi_ctype, relay_name_ctype, relay_action_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
@@ -367,18 +366,17 @@
         path_list_ctype = ctypes.create_string_buffer(path_list.encode(self._encoding))  # case C020
         error_code = self._library.niSwitch_SetPath(vi_ctype, path_list_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
     def unlock(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
-        caller_has_lock_ctype = _visatype.ViBoolean()  # case S220
-        error_code = self._library.niSwitch_UnlockSession(vi_ctype, None if caller_has_lock_ctype is None else (ctypes.pointer(caller_has_lock_ctype)))
+        error_code = self._library.niSwitch_UnlockSession(vi_ctype, None)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
-        return bool(caller_has_lock_ctype.value)
+        return
 
     def wait_for_debounce(self, maximum_time_ms):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         maximum_time_ms_ctype = _visatype.ViInt32(maximum_time_ms)  # case S150
         error_code = self._library.niSwitch_WaitForDebounce(vi_ctype, maximum_time_ms_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
```

### Comparing `niswitch-1.4.3/niswitch/_library_singleton.py` & `niswitch-1.4.4/niswitch/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/niswitch/enums.py` & `niswitch-1.4.4/niswitch/enums.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/niswitch/errors.py` & `niswitch-1.4.4/niswitch/errors.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/niswitch/grpc_session_options.py` & `niswitch-1.4.4/niswitch/grpc_session_options.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/niswitch/nidevice_pb2.py` & `niswitch-1.4.4/niswitch/nidevice_pb2.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/niswitch/niswitch_pb2.py` & `niswitch-1.4.4/niswitch/niswitch_pb2.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/niswitch/niswitch_pb2_grpc.py` & `niswitch-1.4.4/niswitch/niswitch_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/niswitch/session.py` & `niswitch-1.4.4/niswitch/session.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/niswitch/session_pb2.py` & `niswitch-1.4.4/niswitch/session_pb2.py`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/niswitch/session_pb2_grpc.py` & `niswitch-1.4.4/niswitch/session_pb2_grpc.py`

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

### Comparing `niswitch-1.4.3/niswitch.egg-info/PKG-INFO` & `niswitch-1.4.4/niswitch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niswitch
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI-SWITCH Python API
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
 
 NI-SWITCH Python API Status
 ---------------------------
 
 +-------------------------------+-------------------------+
 | NI-SWITCH (niswitch)          |                         |
 +===============================+=========================+
-| Driver Version Tested Against | 2022 Q4                 |
+| Driver Version Tested Against | 2023 Q1                 |
 +-------------------------------+-------------------------+
 | PyPI Version                  | |niswitchLatestVersion| |
 +-------------------------------+-------------------------+
 | Supported Python Version      | |niswitchPythonVersion| |
 +-------------------------------+-------------------------+
 | Open Issues                   | |niswitchOpenIssues|    |
 +-------------------------------+-------------------------+
@@ -135,15 +136,15 @@
 Installation
 ------------
 
 As a prerequisite to using the niswitch module, you must install the NI-SWITCH runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-SWITCH**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install niswitch~=1.4.3
+  $ python -m pip install niswitch~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install niswitch
```

### Comparing `niswitch-1.4.3/niswitch.egg-info/SOURCES.txt` & `niswitch-1.4.4/niswitch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niswitch-1.4.3/setup.py` & `niswitch-1.4.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,32 +25,37 @@
     with open(file_to_read, 'r') as f:
         return f.read()
 
 
 setup(
     name=pypi_name,
     zip_safe=True,
-    version='1.4.3',
+    version='1.4.4',
     description='NI-SWITCH Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
     maintainer_email="opensource@ni.com",
     keywords=['niswitch'],
     license='MIT',
     include_package_data=True,
     packages=['niswitch'],
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

