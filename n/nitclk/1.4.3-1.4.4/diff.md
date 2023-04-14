# Comparing `tmp/nitclk-1.4.3.tar.gz` & `tmp/nitclk-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitclk-1.4.3.tar", last modified: Fri Dec 16 18:56:11 2022, max compression
+gzip compressed data, was "nitclk-1.4.4.tar", last modified: Fri Apr 14 16:09:53 2023, max compression
```

## Comparing `nitclk-1.4.3.tar` & `nitclk-1.4.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:11.735315 nitclk-1.4.3/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8502 2022-12-16 18:56:11.735315 nitclk-1.4.3/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     7496 2022-12-16 18:55:55.000000 nitclk-1.4.3/README.rst
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:11.735315 nitclk-1.4.3/nitclk/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        7 2022-12-16 18:55:54.000000 nitclk-1.4.3/nitclk/VERSION
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     3461 2022-12-16 18:55:54.000000 nitclk-1.4.3/nitclk/__init__.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     5436 2022-12-16 18:55:52.000000 nitclk-1.4.3/nitclk/_attributes.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    14604 2022-12-16 18:55:54.000000 nitclk-1.4.3/nitclk/_converters.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    10861 2022-12-16 18:55:52.000000 nitclk-1.4.3/nitclk/_library.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    12538 2022-12-16 18:55:53.000000 nitclk-1.4.3/nitclk/_library_interpreter.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     1608 2022-12-16 18:55:53.000000 nitclk-1.4.3/nitclk/_library_singleton.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      659 2022-12-16 18:55:54.000000 nitclk-1.4.3/nitclk/_visatype.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     3281 2022-12-16 18:55:53.000000 nitclk-1.4.3/nitclk/errors.py
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)    45940 2022-12-16 18:55:53.000000 nitclk-1.4.3/nitclk/session.py
-drwxr-xr-x   0 tgordon   (1000) tgordon   (1000)        0 2022-12-16 18:56:11.735315 nitclk-1.4.3/nitclk.egg-info/
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     8502 2022-12-16 18:56:11.000000 nitclk-1.4.3/nitclk.egg-info/PKG-INFO
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)      405 2022-12-16 18:56:11.000000 nitclk-1.4.3/nitclk.egg-info/SOURCES.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:11.000000 nitclk-1.4.3/nitclk.egg-info/dependency_links.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       65 2022-12-16 18:56:11.000000 nitclk-1.4.3/nitclk.egg-info/requires.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        7 2022-12-16 18:56:11.000000 nitclk-1.4.3/nitclk.egg-info/top_level.txt
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)        1 2022-12-16 18:56:11.000000 nitclk-1.4.3/nitclk.egg-info/zip-safe
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)       38 2022-12-16 18:56:11.735315 nitclk-1.4.3/setup.cfg
--rw-r--r--   0 tgordon   (1000) tgordon   (1000)     2037 2022-12-16 18:55:55.000000 nitclk-1.4.3/setup.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:10:04.067100 nitclk-1.4.4/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8502 2023-04-14 16:10:04.065103 nitclk-1.4.4/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     7536 2023-04-14 16:07:20.000000 nitclk-1.4.4/README.rst
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:10:03.982102 nitclk-1.4.4/nitclk/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        9 2023-04-14 16:07:16.000000 nitclk-1.4.4/nitclk/VERSION
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3461 2023-04-14 16:07:14.000000 nitclk-1.4.4/nitclk/__init__.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     5436 2023-04-14 16:07:09.000000 nitclk-1.4.4/nitclk/_attributes.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    14604 2023-04-14 16:07:15.000000 nitclk-1.4.4/nitclk/_converters.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    10861 2023-04-14 16:07:09.000000 nitclk-1.4.4/nitclk/_library.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    12538 2023-04-14 16:07:10.000000 nitclk-1.4.4/nitclk/_library_interpreter.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1608 2023-04-14 16:07:11.000000 nitclk-1.4.4/nitclk/_library_singleton.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      688 2023-04-14 16:07:16.000000 nitclk-1.4.4/nitclk/_visatype.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     3281 2023-04-14 16:07:12.000000 nitclk-1.4.4/nitclk/errors.py
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)    45940 2023-04-14 16:07:12.000000 nitclk-1.4.4/nitclk/session.py
+drwxrwxrwx   0 nitest    (1000) nitest    (1000)        0 2023-04-14 16:10:04.052101 nitclk-1.4.4/nitclk.egg-info/
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     8502 2023-04-14 16:10:03.000000 nitclk-1.4.4/nitclk.egg-info/PKG-INFO
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)      405 2023-04-14 16:10:03.000000 nitclk-1.4.4/nitclk.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:10:03.000000 nitclk-1.4.4/nitclk.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       16 2023-04-14 16:10:03.000000 nitclk-1.4.4/nitclk.egg-info/requires.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        7 2023-04-14 16:10:03.000000 nitclk-1.4.4/nitclk.egg-info/top_level.txt
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)        1 2023-04-14 16:10:03.000000 nitclk-1.4.4/nitclk.egg-info/zip-safe
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)       38 2023-04-14 16:10:04.068101 nitclk-1.4.4/setup.cfg
+-rwxrwxrwx   0 nitest    (1000) nitest    (1000)     1951 2023-04-14 16:07:20.000000 nitclk-1.4.4/setup.py
```

### Comparing `nitclk-1.4.3/PKG-INFO` & `nitclk-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitclk
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI-TClk Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -93,15 +93,15 @@
 
 NI-TClk Python API Status
 -------------------------
 
 +-------------------------------+-----------------------+
 | NI-TClk (nitclk)              |                       |
 +===============================+=======================+
-| Driver Version Tested Against | 2022 Q4               |
+| Driver Version Tested Against | 2023 Q2               |
 +-------------------------------+-----------------------+
 | PyPI Version                  | |nitclkLatestVersion| |
 +-------------------------------+-----------------------+
 | Supported Python Version      | |nitclkPythonVersion| |
 +-------------------------------+-----------------------+
 | Open Issues                   | |nitclkOpenIssues|    |
 +-------------------------------+-----------------------+
@@ -135,15 +135,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nitclk module, you must install the NI-TClk runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-TClk**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nitclk~=1.4.3
+  $ python -m pip install nitclk~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install nitclk
```

### Comparing `nitclk-1.4.3/README.rst` & `nitclk-1.4.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 NI-TClk Python API Status
 -------------------------
 
 +-------------------------------+-----------------------+
 | NI-TClk (nitclk)              |                       |
 +===============================+=======================+
-| Driver Version Tested Against | 2022 Q4               |
+| Driver Version Tested Against | 2023 Q2               |
 +-------------------------------+-----------------------+
 | PyPI Version                  | |nitclkLatestVersion| |
 +-------------------------------+-----------------------+
 | Supported Python Version      | |nitclkPythonVersion| |
 +-------------------------------+-----------------------+
 | Open Issues                   | |nitclkOpenIssues|    |
 +-------------------------------+-----------------------+
@@ -98,32 +98,32 @@
 
 
 .. |nitclkOpenPRs| image:: https://img.shields.io/github/issues-pr/ni/nimi-python/nitclk.svg
     :alt: Pull Requests for NI-TClk
     :target: https://github.com/ni/nimi-python/pulls?q=is%3Aopen+is%3Aissue+label%3Anitclk
 
 
-
-.. _nitclk_installation-section:
-
-Installation
-------------
-
-As a prerequisite to using the nitclk module, you must install the NI-TClk runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
-
-The nimi-python modules (i.e. for **NI-TClk**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
-
-  $ python -m pip install nitclk~=1.4.3
-
-Or **easy_install** from
-`setuptools <http://pypi.python.org/pypi/setuptools>`_::
-
-  $ python -m easy_install nitclk
-
-
+
+.. _nitclk_installation-section:
+
+Installation
+------------
+
+As a prerequisite to using the nitclk module, you must install the NI-TClk runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
+
+The nimi-python modules (i.e. for **NI-TClk**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
+
+  $ python -m pip install nitclk~=1.4.4
+
+Or **easy_install** from
+`setuptools <http://pypi.python.org/pypi/setuptools>`_::
+
+  $ python -m easy_install nitclk
+
+
 Contributing
 ============
 
 We welcome contributions! You can clone the project repository, build it, and install it by `following these instructions <https://github.com/ni/nimi-python/blob/master/CONTRIBUTING.md>`_.
 
 Usage
 ------
@@ -132,36 +132,36 @@
 
 .. code-block:: python
 
     import nitclk
 
 `Other usage examples can be found on GitHub. <https://github.com/ni/nimi-python/tree/master/src/nitclk/examples>`_
 
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

### Comparing `nitclk-1.4.3/nitclk/__init__.py` & `nitclk-1.4.4/nitclk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # This file was generated
 
 
-__version__ = '1.4.3'
+__version__ = '1.4.4'
 
 from nitclk.errors import DriverWarning  # noqa: F401
 from nitclk.errors import Error  # noqa: F401
 from nitclk.session import SessionReference  # noqa: F401
 
 # Function imports
 from nitclk.session import configure_for_homogeneous_triggers  # noqa: F401
@@ -69,15 +69,15 @@
 
     info['os']['name'] = os_name
     info['os']['version'] = platform.version()
     info['os']['bits'] = '64' if is_os_64bit() else '32'
     info['driver']['name'] = "NI-TClk"
     info['driver']['version'] = driver_version
     info['module']['name'] = 'nitclk'
-    info['module']['version'] = "1.4.3"
+    info['module']['version'] = "1.4.4"
     info['python']['version'] = sys.version
     info['python']['bits'] = '64' if is_python_64bit() else '32'
     info['python']['is_venv'] = is_venv()
     info['python']['packages'] = installed_packages_list
 
     return info
```

### Comparing `nitclk-1.4.3/nitclk/_attributes.py` & `nitclk-1.4.4/nitclk/_attributes.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.3/nitclk/_converters.py` & `nitclk-1.4.4/nitclk/_converters.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.3/nitclk/_library.py` & `nitclk-1.4.4/nitclk/_library.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.3/nitclk/_library_interpreter.py` & `nitclk-1.4.4/nitclk/_library_interpreter.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.3/nitclk/_library_singleton.py` & `nitclk-1.4.4/nitclk/_library_singleton.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.3/nitclk/errors.py` & `nitclk-1.4.4/nitclk/errors.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.3/nitclk/session.py` & `nitclk-1.4.4/nitclk/session.py`

 * *Files identical despite different names*

### Comparing `nitclk-1.4.3/nitclk.egg-info/PKG-INFO` & `nitclk-1.4.4/nitclk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitclk
-Version: 1.4.3
+Version: 1.4.4
 Summary: NI-TClk Python API
 Home-page: https://github.com/ni/nimi-python
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: NI
 Maintainer-email: opensource@ni.com
 License: MIT
@@ -93,15 +93,15 @@
 
 NI-TClk Python API Status
 -------------------------
 
 +-------------------------------+-----------------------+
 | NI-TClk (nitclk)              |                       |
 +===============================+=======================+
-| Driver Version Tested Against | 2022 Q4               |
+| Driver Version Tested Against | 2023 Q2               |
 +-------------------------------+-----------------------+
 | PyPI Version                  | |nitclkLatestVersion| |
 +-------------------------------+-----------------------+
 | Supported Python Version      | |nitclkPythonVersion| |
 +-------------------------------+-----------------------+
 | Open Issues                   | |nitclkOpenIssues|    |
 +-------------------------------+-----------------------+
@@ -135,15 +135,15 @@
 Installation
 ------------
 
 As a prerequisite to using the nitclk module, you must install the NI-TClk runtime on your system. Visit `ni.com/downloads <http://www.ni.com/downloads/>`_ to download the driver runtime for your devices.
 
 The nimi-python modules (i.e. for **NI-TClk**) can be installed with `pip <http://pypi.python.org/pypi/pip>`_::
 
-  $ python -m pip install nitclk~=1.4.3
+  $ python -m pip install nitclk~=1.4.4
 
 Or **easy_install** from
 `setuptools <http://pypi.python.org/pypi/setuptools>`_::
 
   $ python -m easy_install nitclk
```

### Comparing `nitclk-1.4.3/setup.py` & `nitclk-1.4.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,30 +25,28 @@
     with open(file_to_read, 'r') as f:
         return f.read()
 
 
 setup(
     name=pypi_name,
     zip_safe=True,
-    version='1.4.3',
+    version='1.4.4',
     description='NI-TClk Python API',
     long_description=read_contents('README.rst'),
     long_description_content_type='text/x-rst',
     author='NI',
     author_email="opensource@ni.com",
     url="https://github.com/ni/nimi-python",
     maintainer="NI",
     maintainer_email="opensource@ni.com",
     keywords=['nitclk'],
     license='MIT',
     include_package_data=True,
     packages=['nitclk'],
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

