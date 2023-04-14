# Comparing `tmp/nise-1.4.3.tar.gz` & `tmp/nise-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nise-1.4.3.tar", last modified: Fri Dec 16 18:56:08 2022, max compression
+gzip compressed data, was "nise-1.4.4.tar", last modified: Fri Apr 14 16:09:23 2023, max compression
```

## Comparing `nise-1.4.3.tar` & `nise-1.4.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:08.985315 nise-1.4.3/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8719 2022-12-16 18:56:08.985315 nise-1.4.3/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     7705 2022-12-16 18:55:48.000000 nise-1.4.3/README.rst
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:08.985315 nise-1.4.3/nise/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        7 2022-12-16 18:55:47.000000 nise-1.4.3/nise/VERSION
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     2976 2022-12-16 18:55:46.000000 nise-1.4.3/nise/__init__.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    13867 2022-12-16 18:55:47.000000 nise-1.4.3/nise/_converters.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8599 2022-12-16 18:55:45.000000 nise-1.4.3/nise/_library.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    10784 2022-12-16 18:55:45.000000 nise-1.4.3/nise/_library_interpreter.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     1593 2022-12-16 18:55:46.000000 nise-1.4.3/nise/_library_singleton.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      659 2022-12-16 18:55:47.000000 nise-1.4.3/nise/_visatype.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     1160 2022-12-16 18:55:45.000000 nise-1.4.3/nise/enums.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     3729 2022-12-16 18:55:46.000000 nise-1.4.3/nise/errors.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    36136 2022-12-16 18:55:46.000000 nise-1.4.3/nise/session.py
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:08.985315 nise-1.4.3/nise.egg-info/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8719 2022-12-16 18:56:08.000000 nise-1.4.3/nise.egg-info/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      367 2022-12-16 18:56:08.000000 nise-1.4.3/nise.egg-info/SOURCES.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:08.000000 nise-1.4.3/nise.egg-info/dependency_links.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       65 2022-12-16 18:56:08.000000 nise-1.4.3/nise.egg-info/requires.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        5 2022-12-16 18:56:08.000000 nise-1.4.3/nise.egg-info/top_level.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:08.000000 nise-1.4.3/nise.egg-info/zip-safe
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       38 2022-12-16 18:56:08.985315 nise-1.4.3/setup.cfg
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     2043 2022-12-16 18:55:48.000000 nise-1.4.3/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:34.087863 nise-1.4.4/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8719 2023-04-14 16:09:34.085863 nise-1.4.4/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7745 2023-04-14 16:06:54.000000 nise-1.4.4/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:34.004862 nise-1.4.4/nise/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:06:49.000000 nise-1.4.4/nise/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     2976 2023-04-14 16:06:48.000000 nise-1.4.4/nise/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    13867 2023-04-14 16:06:49.000000 nise-1.4.4/nise/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8599 2023-04-14 16:06:43.000000 nise-1.4.4/nise/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10784 2023-04-14 16:06:44.000000 nise-1.4.4/nise/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1593 2023-04-14 16:06:44.000000 nise-1.4.4/nise/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:06:49.000000 nise-1.4.4/nise/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1160 2023-04-14 16:06:42.000000 nise-1.4.4/nise/enums.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3729 2023-04-14 16:06:46.000000 nise-1.4.4/nise/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    36136 2023-04-14 16:06:45.000000 nise-1.4.4/nise/session.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:09:34.072863 nise-1.4.4/nise.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8719 2023-04-14 16:09:33.000000 nise-1.4.4/nise.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      367 2023-04-14 16:09:33.000000 nise-1.4.4/nise.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:33.000000 nise-1.4.4/nise.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2023-04-14 16:09:33.000000 nise-1.4.4/nise.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        5 2023-04-14 16:09:33.000000 nise-1.4.4/nise.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:09:33.000000 nise-1.4.4/nise.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:09:34.088863 nise-1.4.4/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1957 2023-04-14 16:06:54.000000 nise-1.4.4/setup.py
```

### Comparing `nise-1.4.3/PKG-INFO` & `nise-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nise
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI Switch Executive Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -93,15 +93,15 @@
 
 NI Switch Executive Python API Status
 -------------------------------------
 
 +-------------------------------+---------------------+
 | NI Switch Executive (nise)    |                     |
 +===============================+=====================+
-| Driver Version Tested Against | 21.5.0              |
+| Driver Version Tested Against | 2023 Q1             |
 +-------------------------------+---------------------+
 | PyPI Version                  | |niseLatestVersion| |
 +-------------------------------+---------------------+
 | Supported Python Version      | |nisePythonVersion| |
 +-------------------------------+---------------------+
 | Open Issues                   | |niseOpenIssues|    |
 +-------------------------------+---------------------+
@@ -135,15 +135,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nise module, you must install the NI Switch Executive runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI Switch Executive**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nise~=1.4.3
+  $ python -m pip install nise~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install nise
```

### Comparing `nise-1.4.3/README.rst` & `nise-1.4.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 NI Switch Executive Python API Status
 -------------------------------------
 
 +-------------------------------+---------------------+
 | NI Switch Executive (nise)    |                     |
 +===============================+=====================+
-| Driver Version Tested Against | 21.5.0              |
+| Driver Version Tested Against | 2023 Q1             |
 +-------------------------------+---------------------+
 | PyPI Version                  | |niseLatestVersion| |
 +-------------------------------+---------------------+
 | Supported Python Version      | |nisePythonVersion| |
 +-------------------------------+---------------------+
 | Open Issues                   | |niseOpenIssues|    |
 +-------------------------------+---------------------+
@@ -98,32 +98,32 @@
 
 
 .. |niseOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/nise.svg
     :alt: Pull Requests for NI Switch Executive
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Anise
 
 
-
-.. _nise_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the nise module, you must install the NI Switch Executive runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI Switch Executive**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install nise~=1.4.3
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nise
-
-
+
+.. _nise_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the nise module, you must install the NI Switch Executive runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI Switch Executive**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install nise~=1.4.4
+
+Or **easy_install** from
+`setuptools <http://pypi.python.org/pypi/setuptools>`_::
+
+  $ python -m easy_install nise
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -134,36 +134,36 @@
 
     import nise
     with nise.Session('SwitchExecutiveExample') as session:
         session.connect('DIOToUUT')
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nise/examples>`_
 
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

### Comparing `nise-1.4.3/nise/__init__.py` & `nise-1.4.4/nise/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.3'
+__version__ = '1.4.4'
 
 from nise.enums import *  # noqa: F403,F401,H303
 from nise.errors import DriverWarning  # noqa: F401
 from nise.errors import Error  # noqa: F401
 from nise.session import Session  # noqa: F401
 
 
@@ -60,15 +60,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI Switch Executive"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nise'
-    info['module']['version'] = "1.4.3"
+    info['module']['version'] = "1.4.4"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nise-1.4.3/nise/_converters.py` & `nise-1.4.4/nise/_converters.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.3/nise/_library.py` & `nise-1.4.4/nise/_library.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.3/nise/_library_interpreter.py` & `nise-1.4.4/nise/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.3/nise/_library_singleton.py` & `nise-1.4.4/nise/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.3/nise/enums.py` & `nise-1.4.4/nise/enums.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.3/nise/errors.py` & `nise-1.4.4/nise/errors.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.3/nise/session.py` & `nise-1.4.4/nise/session.py`

 * *Files identical despite different names*

### Comparing `nise-1.4.3/nise.egg-info/PKG-INFO` & `nise-1.4.4/nise.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nise
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI Switch Executive Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -93,15 +93,15 @@
 
 NI Switch Executive Python API Status
 -------------------------------------
 
 +-------------------------------+---------------------+
 | NI Switch Executive (nise)    |                     |
 +===============================+=====================+
-| Driver Version Tested Against | 21.5.0              |
+| Driver Version Tested Against | 2023 Q1             |
 +-------------------------------+---------------------+
 | PyPI Version                  | |niseLatestVersion| |
 +-------------------------------+---------------------+
 | Supported Python Version      | |nisePythonVersion| |
 +-------------------------------+---------------------+
 | Open Issues                   | |niseOpenIssues|    |
 +-------------------------------+---------------------+
@@ -135,15 +135,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nise module, you must install the NI Switch Executive runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI Switch Executive**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nise~=1.4.3
+  $ python -m pip install nise~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install nise
```

### Comparing `nise-1.4.3/setup.py` & `nise-1.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,30 +25,28 @@
     with open(file_to_read, 'r') as f:
         return f.read()
 
 
 setup(
     name=pypi_name,
     zip_safe=True,
-    version='1.4.3',
+    version='1.4.4',
     description='NI Switch Executive Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
     maintainer_email="opensource@ni.com",
     keywords=['nise'],
     license='MIT',
     include_package_data=True,
     packages=['nise'],
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

