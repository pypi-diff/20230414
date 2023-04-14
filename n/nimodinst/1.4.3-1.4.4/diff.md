# Comparing `tmp/nimodinst-1.4.3.tar.gz` & `tmp/nimodinst-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimodinst-1.4.3.tar", last modified: Fri Dec 16 18:56:10 2022, max compression
+gzip compressed data, was "nimodinst-1.4.4.tar", last modified: Fri Apr 14 16:09:39 2023, max compression
```

## Comparing `nimodinst-1.4.3.tar` & `nimodinst-1.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:10.385315 nimodinst-1.4.3/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8905 2022-12-16 18:56:10.385315 nimodinst-1.4.3/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     7890 2022-12-16 18:55:51.000000 nimodinst-1.4.3/README.rst
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:10.385315 nimodinst-1.4.3/nimodinst/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        7 2022-12-16 18:55:50.000000 nimodinst-1.4.3/nimodinst/VERSION
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     2932 2022-12-16 18:55:50.000000 nimodinst-1.4.3/nimodinst/__init__.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    13877 2022-12-16 18:55:50.000000 nimodinst-1.4.3/nimodinst/_converters.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     4561 2022-12-16 18:55:49.000000 nimodinst-1.4.3/nimodinst/_library.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     7235 2022-12-16 18:55:49.000000 nimodinst-1.4.3/nimodinst/_library_interpreter.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     1626 2022-12-16 18:55:49.000000 nimodinst-1.4.3/nimodinst/_library_singleton.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      659 2022-12-16 18:55:50.000000 nimodinst-1.4.3/nimodinst/_visatype.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     3314 2022-12-16 18:55:50.000000 nimodinst-1.4.3/nimodinst/errors.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    14066 2022-12-16 18:55:49.000000 nimodinst-1.4.3/nimodinst/session.py
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:10.385315 nimodinst-1.4.3/nimodinst.egg-info/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8905 2022-12-16 18:56:10.000000 nimodinst-1.4.3/nimodinst.egg-info/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      428 2022-12-16 18:56:10.000000 nimodinst-1.4.3/nimodinst.egg-info/SOURCES.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:10.000000 nimodinst-1.4.3/nimodinst.egg-info/dependency_links.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       65 2022-12-16 18:56:10.000000 nimodinst-1.4.3/nimodinst.egg-info/requires.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       10 2022-12-16 18:56:10.000000 nimodinst-1.4.3/nimodinst.egg-info/top_level.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:10.000000 nimodinst-1.4.3/nimodinst.egg-info/zip-safe
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       38 2022-12-16 18:56:10.385315 nimodinst-1.4.3/setup.cfg
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     2049 2022-12-16 18:55:52.000000 nimodinst-1.4.3/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:49.608416 nimodinst-1.4.4/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8905 2023-04-14 16:09:49.607416 nimodinst-1.4.4/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7930 2023-04-14 16:07:07.000000 nimodinst-1.4.4/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:49.526415 nimodinst-1.4.4/nimodinst/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:07:03.000000 nimodinst-1.4.4/nimodinst/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2932 2023-04-14 16:07:01.000000 nimodinst-1.4.4/nimodinst/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13877 2023-04-14 16:07:02.000000 nimodinst-1.4.4/nimodinst/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     4561 2023-04-14 16:06:56.000000 nimodinst-1.4.4/nimodinst/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7235 2023-04-14 16:06:57.000000 nimodinst-1.4.4/nimodinst/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1626 2023-04-14 16:06:57.000000 nimodinst-1.4.4/nimodinst/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:07:03.000000 nimodinst-1.4.4/nimodinst/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3314 2023-04-14 16:06:59.000000 nimodinst-1.4.4/nimodinst/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    14066 2023-04-14 16:06:58.000000 nimodinst-1.4.4/nimodinst/session.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:49.594416 nimodinst-1.4.4/nimodinst.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8905 2023-04-14 16:09:49.000000 nimodinst-1.4.4/nimodinst.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      428 2023-04-14 16:09:49.000000 nimodinst-1.4.4/nimodinst.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:49.000000 nimodinst-1.4.4/nimodinst.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2023-04-14 16:09:49.000000 nimodinst-1.4.4/nimodinst.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       10 2023-04-14 16:09:49.000000 nimodinst-1.4.4/nimodinst.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:49.000000 nimodinst-1.4.4/nimodinst.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:09:49.609417 nimodinst-1.4.4/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1963 2023-04-14 16:07:07.000000 nimodinst-1.4.4/setup.py
```

### Comparing `nimodinst-1.4.3/PKG-INFO` & `nimodinst-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimodinst
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI-ModInst Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -93,15 +93,15 @@
 
 NI-ModInst Python API Status
 ----------------------------
 
 +-------------------------------+--------------------------+
 | NI-ModInst (nimodinst)        |                          |
 +===============================+==========================+
-| Driver Version Tested Against | 2022 Q4                  |
+| Driver Version Tested Against | 2023 Q2                  |
 +-------------------------------+--------------------------+
 | PyPI Version                  | |nimodinstLatestVersion| |
 +-------------------------------+--------------------------+
 | Supported Python Version      | |nimodinstPythonVersion| |
 +-------------------------------+--------------------------+
 | Open Issues                   | |nimodinstOpenIssues|    |
 +-------------------------------+--------------------------+
@@ -135,15 +135,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nimodinst module, you must install the NI-ModInst runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-ModInst**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nimodinst~=1.4.3
+  $ python -m pip install nimodinst~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install nimodinst
```

### Comparing `nimodinst-1.4.3/README.rst` & `nimodinst-1.4.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 NI-ModInst Python API Status
 ----------------------------
 
 +-------------------------------+--------------------------+
 | NI-ModInst (nimodinst)        |                          |
 +===============================+==========================+
-| Driver Version Tested Against | 2022 Q4                  |
+| Driver Version Tested Against | 2023 Q2                  |
 +-------------------------------+--------------------------+
 | PyPI Version                  | |nimodinstLatestVersion| |
 +-------------------------------+--------------------------+
 | Supported Python Version      | |nimodinstPythonVersion| |
 +-------------------------------+--------------------------+
 | Open Issues                   | |nimodinstOpenIssues|    |
 +-------------------------------+--------------------------+
@@ -98,32 +98,32 @@
 
 
 .. |nimodinstOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/nimodinst.svg
     :alt: Pull Requests for NI-ModInst
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Animodinst
 
 
-
-.. _nimodinst_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the nimodinst module, you must install the NI-ModInst runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI-ModInst**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install nimodinst~=1.4.3
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nimodinst
-
-
+
+.. _nimodinst_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the nimodinst module, you must install the NI-ModInst runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI-ModInst**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install nimodinst~=1.4.4
+
+Or **easy_install** from
+`setuptools <http://pypi.python.org/pypi/setuptools>`_::
+
+  $ python -m easy_install nimodinst
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -135,36 +135,36 @@
     import nimodinst
     with nimodinst.Session("niscope") as session:
         for device in session:
             print("{: >20} {: >15} {: >10}".format(device.device_name, device.device_model, device.serial_number))
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nimodinst/examples>`_
 
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

### Comparing `nimodinst-1.4.3/nimodinst/__init__.py` & `nimodinst-1.4.4/nimodinst/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.3'
+__version__ = '1.4.4'
 
 from nimodinst.errors import DriverWarning  # noqa: F401
 from nimodinst.errors import Error  # noqa: F401
 from nimodinst.session import Session  # noqa: F401
 
 
 def get_diagnostic_information():
@@ -59,15 +59,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-ModInst"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nimodinst'
-    info['module']['version'] = "1.4.3"
+    info['module']['version'] = "1.4.4"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nimodinst-1.4.3/nimodinst/_converters.py` & `nimodinst-1.4.4/nimodinst/_converters.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.3/nimodinst/_library.py` & `nimodinst-1.4.4/nimodinst/_library.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.3/nimodinst/_library_interpreter.py` & `nimodinst-1.4.4/nimodinst/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.3/nimodinst/_library_singleton.py` & `nimodinst-1.4.4/nimodinst/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.3/nimodinst/errors.py` & `nimodinst-1.4.4/nimodinst/errors.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.3/nimodinst/session.py` & `nimodinst-1.4.4/nimodinst/session.py`

 * *Files identical despite different names*

### Comparing `nimodinst-1.4.3/nimodinst.egg-info/PKG-INFO` & `nimodinst-1.4.4/nimodinst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimodinst
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI-ModInst Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -93,15 +93,15 @@
 
 NI-ModInst Python API Status
 ----------------------------
 
 +-------------------------------+--------------------------+
 | NI-ModInst (nimodinst)        |                          |
 +===============================+==========================+
-| Driver Version Tested Against | 2022 Q4                  |
+| Driver Version Tested Against | 2023 Q2                  |
 +-------------------------------+--------------------------+
 | PyPI Version                  | |nimodinstLatestVersion| |
 +-------------------------------+--------------------------+
 | Supported Python Version      | |nimodinstPythonVersion| |
 +-------------------------------+--------------------------+
 | Open Issues                   | |nimodinstOpenIssues|    |
 +-------------------------------+--------------------------+
@@ -135,15 +135,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nimodinst module, you must install the NI-ModInst runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-ModInst**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nimodinst~=1.4.3
+  $ python -m pip install nimodinst~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install nimodinst
```

### Comparing `nimodinst-1.4.3/setup.py` & `nimodinst-1.4.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,30 +25,28 @@
     with open(file_to_read, 'r') as f:
         return f.read()
 
 
 setup(
     name=pypi_name,
     zip_safe=True,
-    version='1.4.3',
+    version='1.4.4',
     description='NI-ModInst Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
     maintainer_email="opensource@ni.com",
     keywords=['nimodinst'],
     license='MIT',
     include_package_data=True,
     packages=['nimodinst'],
     install_requires=[
-        'enum34;python_version<"3.4"',
-        'singledispatch;python_version<"3.4"',
         'hightime>=0.2.0',
     ],
     setup_requires=['pytest-runner', ],
     tests_require=['pytest'],
     test_suite='tests',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

