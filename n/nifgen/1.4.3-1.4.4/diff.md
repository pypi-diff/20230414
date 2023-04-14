# Comparing `tmp/nifgen-1.4.3.tar.gz` & `tmp/nifgen-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifgen-1.4.3.tar", last modified: Fri Dec 16 18:56:04 2022, max compression
+gzip compressed data, was "nifgen-1.4.4.tar", last modified: Fri Apr 14 16:08:35 2023, max compression
```

## Comparing `nifgen-1.4.3.tar` & `nifgen-1.4.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:04.545315 nifgen-1.4.3/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8898 2022-12-16 18:56:04.545315 nifgen-1.4.3/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     7892 2022-12-16 18:55:25.000000 nifgen-1.4.3/README.rst
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:04.545315 nifgen-1.4.3/nifgen/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        7 2022-12-16 18:55:20.000000 nifgen-1.4.3/nifgen/VERSION
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     3031 2022-12-16 18:55:19.000000 nifgen-1.4.3/nifgen/__init__.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     5436 2022-12-16 18:55:16.000000 nifgen-1.4.3/nifgen/_attributes.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    13871 2022-12-16 18:55:20.000000 nifgen-1.4.3/nifgen/_converters.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    23011 2022-12-16 18:55:21.000000 nifgen-1.4.3/nifgen/_grpc_stub_interpreter.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    47920 2022-12-16 18:55:17.000000 nifgen-1.4.3/nifgen/_library.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    53551 2022-12-16 18:55:17.000000 nifgen-1.4.3/nifgen/_library_interpreter.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     1611 2022-12-16 18:55:17.000000 nifgen-1.4.3/nifgen/_library_singleton.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      659 2022-12-16 18:55:22.000000 nifgen-1.4.3/nifgen/_visatype.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    10338 2022-12-16 18:55:16.000000 nifgen-1.4.3/nifgen/enums.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     4359 2022-12-16 18:55:18.000000 nifgen-1.4.3/nifgen/errors.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     3452 2022-12-16 18:55:21.000000 nifgen-1.4.3/nifgen/grpc_session_options.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     1895 2022-12-16 18:55:22.000000 nifgen-1.4.3/nifgen/nidevice_pb2.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      159 2022-12-16 18:55:22.000000 nifgen-1.4.3/nifgen/nidevice_pb2_grpc.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)   123775 2022-12-16 18:55:21.000000 nifgen-1.4.3/nifgen/nifgen_pb2.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)   216324 2022-12-16 18:55:21.000000 nifgen-1.4.3/nifgen/nifgen_pb2_grpc.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)   212642 2022-12-16 18:55:18.000000 nifgen-1.4.3/nifgen/session.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     4196 2022-12-16 18:55:22.000000 nifgen-1.4.3/nifgen/session_pb2.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8907 2022-12-16 18:55:22.000000 nifgen-1.4.3/nifgen/session_pb2_grpc.py
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:04.545315 nifgen-1.4.3/nifgen.egg-info/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8898 2022-12-16 18:56:04.000000 nifgen-1.4.3/nifgen.egg-info/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      632 2022-12-16 18:56:04.000000 nifgen-1.4.3/nifgen.egg-info/SOURCES.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:04.000000 nifgen-1.4.3/nifgen.egg-info/dependency_links.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       72 2022-12-16 18:56:04.000000 nifgen-1.4.3/nifgen.egg-info/requires.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        7 2022-12-16 18:56:04.000000 nifgen-1.4.3/nifgen.egg-info/top_level.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:04.000000 nifgen-1.4.3/nifgen.egg-info/zip-safe
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       38 2022-12-16 18:56:04.545315 nifgen-1.4.3/setup.cfg
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     2055 2022-12-16 18:55:26.000000 nifgen-1.4.3/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:45.541828 nifgen-1.4.4/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8919 2023-04-14 16:08:45.539828 nifgen-1.4.4/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7932 2023-04-14 16:05:52.000000 nifgen-1.4.4/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:45.456827 nifgen-1.4.4/nifgen/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:05:40.000000 nifgen-1.4.4/nifgen/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3031 2023-04-14 16:05:39.000000 nifgen-1.4.4/nifgen/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5436 2023-04-14 16:05:30.000000 nifgen-1.4.4/nifgen/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13871 2023-04-14 16:05:39.000000 nifgen-1.4.4/nifgen/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    23011 2023-04-14 16:05:41.000000 nifgen-1.4.4/nifgen/_grpc_stub_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    47920 2023-04-14 16:05:32.000000 nifgen-1.4.4/nifgen/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    53193 2023-04-14 16:05:33.000000 nifgen-1.4.4/nifgen/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1611 2023-04-14 16:05:34.000000 nifgen-1.4.4/nifgen/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:05:45.000000 nifgen-1.4.4/nifgen/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10347 2023-04-14 16:05:31.000000 nifgen-1.4.4/nifgen/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4359 2023-04-14 16:05:36.000000 nifgen-1.4.4/nifgen/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3452 2023-04-14 16:05:42.000000 nifgen-1.4.4/nifgen/grpc_session_options.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1895 2023-04-14 16:05:44.000000 nifgen-1.4.4/nifgen/nidevice_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      159 2023-04-14 16:05:44.000000 nifgen-1.4.4/nifgen/nidevice_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   123775 2023-04-14 16:05:43.000000 nifgen-1.4.4/nifgen/nifgen_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   216324 2023-04-14 16:05:43.000000 nifgen-1.4.4/nifgen/nifgen_pb2_grpc.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)   212642 2023-04-14 16:05:35.000000 nifgen-1.4.4/nifgen/session.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4196 2023-04-14 16:05:45.000000 nifgen-1.4.4/nifgen/session_pb2.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8913 2023-04-14 16:05:45.000000 nifgen-1.4.4/nifgen/session_pb2_grpc.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:08:45.526828 nifgen-1.4.4/nifgen.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8919 2023-04-14 16:08:45.000000 nifgen-1.4.4/nifgen.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      632 2023-04-14 16:08:45.000000 nifgen-1.4.4/nifgen.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:08:45.000000 nifgen-1.4.4/nifgen.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      161 2023-04-14 16:08:45.000000 nifgen-1.4.4/nifgen.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        7 2023-04-14 16:08:45.000000 nifgen-1.4.4/nifgen.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:08:45.000000 nifgen-1.4.4/nifgen.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:08:45.542828 nifgen-1.4.4/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2210 2023-04-14 16:05:53.000000 nifgen-1.4.4/setup.py
```

### Comparing `nifgen-1.4.3/PKG-INFO` & `nifgen-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifgen
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI-FGEN Python API
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
 
 NI-FGEN Python API Status
 -------------------------
 
 +-------------------------------+-----------------------+
 | NI-FGEN (nifgen)              |                       |
 +===============================+=======================+
-| Driver Version Tested Against | 21.8.0                |
+| Driver Version Tested Against | 2023 Q1.1             |
 +-------------------------------+-----------------------+
 | PyPI Version                  | |nifgenLatestVersion| |
 +-------------------------------+-----------------------+
 | Supported Python Version      | |nifgenPythonVersion| |
 +-------------------------------+-----------------------+
 | Open Issues                   | |nifgenOpenIssues|    |
 +-------------------------------+-----------------------+
@@ -135,15 +136,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nifgen module, you must install the NI-FGEN runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-FGEN**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nifgen~=1.4.3
+  $ python -m pip install nifgen~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install nifgen
```

### Comparing `nifgen-1.4.3/README.rst` & `nifgen-1.4.4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 NI-FGEN Python API Status
 -------------------------
 
 +-------------------------------+-----------------------+
 | NI-FGEN (nifgen)              |                       |
 +===============================+=======================+
-| Driver Version Tested Against | 21.8.0                |
+| Driver Version Tested Against | 2023 Q1.1             |
 +-------------------------------+-----------------------+
 | PyPI Version                  | |nifgenLatestVersion| |
 +-------------------------------+-----------------------+
 | Supported Python Version      | |nifgenPythonVersion| |
 +-------------------------------+-----------------------+
 | Open Issues                   | |nifgenOpenIssues|    |
 +-------------------------------+-----------------------+
@@ -98,32 +98,32 @@
 
 
 .. |nifgenOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/nifgen.svg
     :alt: Pull Requests for NI-FGEN
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Anifgen
 
 
-
-.. _nifgen_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the nifgen module, you must install the NI-FGEN runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI-FGEN**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install nifgen~=1.4.3
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nifgen
-
-
+
+.. _nifgen_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the nifgen module, you must install the NI-FGEN runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI-FGEN**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install nifgen~=1.4.4
+
+Or **easy_install** from
+`setuptools <http://pypi.python.org/pypi/setuptools>`_::
+
+  $ python -m easy_install nifgen
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -138,36 +138,36 @@
         session.output_mode = nifgen.OutputMode.FUNC
         session.configure_standard_waveform(waveform=nifgen.Waveform.SINE, amplitude=1.0, frequency=10000000, dc_offset=0.0, start_phase=0.0)
         with session.initiate():
             time.sleep(5)
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nifgen/examples>`_
 
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

### Comparing `nifgen-1.4.3/nifgen/__init__.py` & `nifgen-1.4.4/nifgen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.3'
+__version__ = '1.4.4'
 
 from nifgen.enums import *  # noqa: F403,F401,H303
 from nifgen.errors import DriverWarning  # noqa: F401
 from nifgen.errors import Error  # noqa: F401
 from nifgen.grpc_session_options import *  # noqa: F403,F401,H303
 from nifgen.session import Session  # noqa: F401
 
@@ -61,15 +61,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-FGEN"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nifgen'
-    info['module']['version'] = "1.4.3"
+    info['module']['version'] = "1.4.4"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nifgen-1.4.3/nifgen/_attributes.py` & `nifgen-1.4.4/nifgen/_attributes.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.3/nifgen/_converters.py` & `nifgen-1.4.4/nifgen/_converters.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.3/nifgen/_grpc_stub_interpreter.py` & `nifgen-1.4.4/nifgen/_grpc_stub_interpreter.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.3/nifgen/_library.py` & `nifgen-1.4.4/nifgen/_library.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.3/nifgen/_library_interpreter.py` & `nifgen-1.4.4/nifgen/_library_interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,18 +497,17 @@
         done_ctype = _visatype.ViBoolean()  # case S220
         error_code = self._library.niFgen_IsDone(vi_ctype, None if done_ctype is None else (ctypes.pointer(done_ctype)))
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return bool(done_ctype.value)
 
     def lock(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
-        caller_has_lock_ctype = _visatype.ViBoolean()  # case S220
-        error_code = self._library.niFgen_LockSession(vi_ctype, None if caller_has_lock_ctype is None else (ctypes.pointer(caller_has_lock_ctype)))
+        error_code = self._library.niFgen_LockSession(vi_ctype, None)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
-        return bool(caller_has_lock_ctype.value)
+        return
 
     def query_arb_seq_capabilities(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         maximum_number_of_sequences_ctype = _visatype.ViInt32()  # case S220
         minimum_sequence_length_ctype = _visatype.ViInt32()  # case S220
         maximum_sequence_length_ctype = _visatype.ViInt32()  # case S220
         maximum_loop_count_ctype = _visatype.ViInt32()  # case S220
@@ -625,18 +624,17 @@
         offset_ctype = _visatype.ViInt32(offset)  # case S150
         error_code = self._library.niFgen_SetWaveformNextWritePosition(vi_ctype, channel_name_ctype, waveform_handle_ctype, relative_to_ctype, offset_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
 
     def unlock(self):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
-        caller_has_lock_ctype = _visatype.ViBoolean()  # case S220
-        error_code = self._library.niFgen_UnlockSession(vi_ctype, None if caller_has_lock_ctype is None else (ctypes.pointer(caller_has_lock_ctype)))
+        error_code = self._library.niFgen_UnlockSession(vi_ctype, None)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
-        return bool(caller_has_lock_ctype.value)
+        return
 
     def wait_until_done(self, max_time):  # noqa: N802
         vi_ctype = _visatype.ViSession(self._vi)  # case S110
         max_time_ctype = _visatype.ViInt32(max_time)  # case S150
         error_code = self._library.niFgen_WaitUntilDone(vi_ctype, max_time_ctype)
         errors.handle_error(self, error_code, ignore_warnings=False, is_error_handling=False)
         return
```

### Comparing `nifgen-1.4.3/nifgen/_library_singleton.py` & `nifgen-1.4.4/nifgen/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.3/nifgen/enums.py` & `nifgen-1.4.4/nifgen/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     ONBOARD_REFERENCE_CLOCK = 'OnboardRefClk'
     r'''
     Specifies that the onboard Reference Clock is used as the Reference
     Clock source.
     '''
     PXI_CLOCK = 'PXI_Clk'
     r'''
-    Specifies the PXI Clock is used as the Reference Clock source.
+    Specifies that the PXI Clock is used as the Reference Clock source.
     '''
     RTSI_7 = 'RTSI7'
     r'''
     Specifies that the RTSI line 7 is used as the Reference Clock source.
     '''
 
 
@@ -162,15 +162,15 @@
     CLOCK_IN = 'ClkIn'
     r'''
     Specifies that the signal at the CLK IN front panel connector is used as
     the Sample Clock source.
     '''
     DDC_CLOCK_IN = 'DDC_ClkIn'
     r'''
-    Specifies that the Sample Clock from DDC connector is used as the Sample
+    Specifies that the Sample Clock from the DDC connector is used as the Sample
     Clock source.
     '''
     ONBOARD_CLOCK = 'OnboardClock'
     r'''
     Specifies that the onboard clock is used as the Sample Clock source.
     '''
     PXI_STAR_LINE = 'PXI_Star'
```

### Comparing `nifgen-1.4.3/nifgen/errors.py` & `nifgen-1.4.4/nifgen/errors.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.3/nifgen/grpc_session_options.py` & `nifgen-1.4.4/nifgen/grpc_session_options.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.3/nifgen/nidevice_pb2.py` & `nifgen-1.4.4/nifgen/nidevice_pb2.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.3/nifgen/nifgen_pb2.py` & `nifgen-1.4.4/nifgen/nifgen_pb2.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.3/nifgen/nifgen_pb2_grpc.py` & `nifgen-1.4.4/nifgen/nifgen_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.3/nifgen/session.py` & `nifgen-1.4.4/nifgen/session.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.3/nifgen/session_pb2.py` & `nifgen-1.4.4/nifgen/session_pb2.py`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.3/nifgen/session_pb2_grpc.py` & `nifgen-1.4.4/nifgen/session_pb2_grpc.py`

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

### Comparing `nifgen-1.4.3/nifgen.egg-info/PKG-INFO` & `nifgen-1.4.4/nifgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifgen
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI-FGEN Python API
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
 
 NI-FGEN Python API Status
 -------------------------
 
 +-------------------------------+-----------------------+
 | NI-FGEN (nifgen)              |                       |
 +===============================+=======================+
-| Driver Version Tested Against | 21.8.0                |
+| Driver Version Tested Against | 2023 Q1.1             |
 +-------------------------------+-----------------------+
 | PyPI Version                  | |nifgenLatestVersion| |
 +-------------------------------+-----------------------+
 | Supported Python Version      | |nifgenPythonVersion| |
 +-------------------------------+-----------------------+
 | Open Issues                   | |nifgenOpenIssues|    |
 +-------------------------------+-----------------------+
@@ -135,15 +136,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nifgen module, you must install the NI-FGEN runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-FGEN**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nifgen~=1.4.3
+  $ python -m pip install nifgen~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install nifgen
```

### Comparing `nifgen-1.4.3/nifgen.egg-info/SOURCES.txt` & `nifgen-1.4.4/nifgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nifgen-1.4.3/setup.py` & `nifgen-1.4.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,33 +25,38 @@
     with open(file_to_read, 'r') as f:
         return f.read()
 
 
 setup(
     name=pypi_name,
     zip_safe=True,
-    version='1.4.3',
+    version='1.4.4',
     description='NI-FGEN Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
     maintainer_email="opensource@ni.com",
     keywords=['nifgen'],
     license='MIT',
     include_package_data=True,
     packages=['nifgen'],
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

