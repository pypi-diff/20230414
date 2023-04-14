# Comparing `tmp/python_plus-2.0.5.tar.gz` & `tmp/python_plus-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python_plus-2.0.5.tar", last modified: Fri Jan 13 17:51:02 2023, max compression
+gzip compressed data, was "python_plus-2.0.6.tar", last modified: Fri Apr 14 17:17:42 2023, max compression
```

## Comparing `python_plus-2.0.5.tar` & `python_plus-2.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:51:02.000000 python_plus-2.0.5/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:51:02.000000 python_plus-2.0.5/python_plus/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1177 2023-01-09 05:20:14.000000 python_plus-2.0.5/python_plus/__main__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:51:02.000000 python_plus-2.0.5/python_plus/scripts/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7532 2022-12-26 08:19:41.000000 python_plus-2.0.5/python_plus/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6398 2023-01-09 05:20:14.000000 python_plus-2.0.5/python_plus/scripts/main.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 python_plus-2.0.5/python_plus/scripts/vem.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    47273 2023-01-09 05:20:08.000000 python_plus-2.0.5/python_plus/scripts/list_requirements.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    66027 2023-01-09 05:20:14.000000 python_plus-2.0.5/python_plus/scripts/vem.sh
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       93 2022-12-09 05:08:44.000000 python_plus-2.0.5/python_plus/scripts/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8668 2023-01-09 05:20:14.000000 python_plus-2.0.5/python_plus/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3696 2022-12-09 05:08:44.000000 python_plus-2.0.5/python_plus/vem.man
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-01-13 17:51:02.000000 python_plus-2.0.5/python_plus.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       12 2023-01-13 17:51:02.000000 python_plus-2.0.5/python_plus.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-13 17:51:02.000000 python_plus-2.0.5/python_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:33:53.000000 python_plus-2.0.5/python_plus.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      169 2023-01-13 17:51:02.000000 python_plus-2.0.5/python_plus.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      519 2023-01-13 17:51:02.000000 python_plus-2.0.5/python_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        6 2023-01-13 17:51:02.000000 python_plus-2.0.5/python_plus.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8054 2023-01-13 17:51:02.000000 python_plus-2.0.5/python_plus.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-01-13 17:51:02.000000 python_plus-2.0.5/setup.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7581 2023-01-09 05:20:14.000000 python_plus-2.0.5/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8054 2023-01-13 17:51:02.000000 python_plus-2.0.5/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14796 2023-01-13 17:51:02.000000 python_plus-2.0.5/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:17:42.490855 python_plus-2.0.6/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6979 2023-04-14 17:17:42.490855 python_plus-2.0.6/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15133 2023-04-14 17:17:41.000000 python_plus-2.0.6/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:17:42.490855 python_plus-2.0.6/python_plus/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8668 2023-03-25 15:58:03.000000 python_plus-2.0.6/python_plus/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1177 2023-03-25 15:58:03.000000 python_plus-2.0.6/python_plus/__main__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:17:42.490855 python_plus-2.0.6/python_plus/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       93 2022-12-09 05:08:44.000000 python_plus-2.0.6/python_plus/scripts/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    48185 2023-04-14 13:58:36.000000 python_plus-2.0.6/python_plus/scripts/list_requirements.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6398 2023-03-25 15:58:03.000000 python_plus-2.0.6/python_plus/scripts/main.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7581 2023-04-14 17:17:01.000000 python_plus-2.0.6/python_plus/scripts/setup.info
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 python_plus-2.0.6/python_plus/scripts/vem.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    66051 2023-04-14 17:14:36.000000 python_plus-2.0.6/python_plus/scripts/vem.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3696 2022-12-09 05:08:44.000000 python_plus-2.0.6/python_plus/vem.man
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-04-14 17:17:42.490855 python_plus-2.0.6/python_plus.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6979 2023-04-14 17:17:42.000000 python_plus-2.0.6/python_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      519 2023-04-14 17:17:42.000000 python_plus-2.0.6/python_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-04-14 17:17:42.000000 python_plus-2.0.6/python_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      169 2023-04-14 17:17:42.000000 python_plus-2.0.6/python_plus.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:33:53.000000 python_plus-2.0.6/python_plus.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        6 2023-04-14 17:17:42.000000 python_plus-2.0.6/python_plus.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       12 2023-04-14 17:17:42.000000 python_plus-2.0.6/python_plus.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-04-14 17:17:42.490855 python_plus-2.0.6/setup.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7581 2023-03-25 15:58:03.000000 python_plus-2.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python_plus-2.0.5/python_plus/__main__.py` & `python_plus-2.0.6/python_plus/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import os
 import subprocess
 import sys
 
 from zerobug import Z0BUG
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 STS_FAILED = 1
 STS_SUCCESS = 0
 
 if __name__ == "__main__":
     action = False
     if len(sys.argv) > 1:
         action = sys.argv[1]
```

### Comparing `python_plus-2.0.5/python_plus/scripts/setup.info` & `python_plus-2.0.6/python_plus/scripts/setup.info`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='python_plus',
-    version='2.0.4',
+    version='2.0.6',
     description='python useful function',
     long_description="""
 Python supplemental features
 ----------------------------
 
 python-plus adds various features to python 2 and python 3 programs.
 It is designed to be used as integration of pypi future to help to port your code from Python 2 to Python 3 and still have it run on Python 2.
@@ -142,14 +142,15 @@
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: System :: System Shells',
     ],
     keywords='unit test virtual environment venv',
     project_urls={
```

### Comparing `python_plus-2.0.5/python_plus/scripts/main.py` & `python_plus-2.0.6/python_plus/scripts/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
```

### Comparing `python_plus-2.0.5/python_plus/scripts/vem.py` & `python_plus-2.0.6/python_plus/scripts/vem.py`

 * *Files identical despite different names*

### Comparing `python_plus-2.0.5/python_plus/scripts/list_requirements.py` & `python_plus-2.0.6/python_plus/scripts/list_requirements.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,39 +20,40 @@
     import python_plus
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 python_version = "%s.%s" % (sys.version_info[0], sys.version_info[1])
 
 #
 # known incompatibilities:
 # - requests: oca-maintainers-tools -> '==2.3.0',
 #             codecov -> '>=2.7.9'
 # Here we assume: Odoo 11.0 use python 3.5, Odoo 12.0 uses python 3.7
 # If version is 2.7 or 3.5 or 3.6 or 3.7 or 3.8 or 3.9 then it refers to python version
 REQVERSION = {
     "acme_tiny": {"6.1": ">=4.0.3"},
     "argparse": {"0": "==1.2.1"},
     "astroid": {"2.7": "==1.6.5", "3.5": "==2.2.0"},  # Version by test pkgs
     "autopep8": {"0": "==1.2"},
-    "Babel": {"6.1": "==1.3", "8.0": "==2.3.4"},
+    "Babel": {"6.1": "==1.3", "8.0": "==2.3.4", "16.0": ">=2.6.0<=2.9.1"},
     "beautifulsoup": {"6.1": "==3.2.1"},
     "bokeh": {
         "11.0": "==0.12.7", "12.0": "==1.1.0", "14.0": "==2.3.1", "15.0": "2.4.2"
     },
     "codicefiscale": {"6.1": "==0.9"},
     "coverage": {"2.7": "<5.6.0", "3.5": ">=5.0.0"},
-    "cryptography": {"2.7": ">=2.2.2", "3.7": ">=38.0"},
+    "cryptography": {"2.7": ">=2.2.2", "3.7": ">=38.0<39.0"},
     "decorator": {"6.1": "==3.4.0", "10.0": "==4.0.10"},
     "docutils": {"6.1": "==0.12", "0": "==0.14", "3.7": "==0.16"},       # By test pkgs
     "ebaysdk": {"6.1": "==2.1.4"},
+    "email_validator": {"10.0": "<1.3.0", "12.0": ">=1.3"},
     "ERPpeek": {"0": "==1.6.1"},
     "feedparser": {"6.1": "==5.1.3", "10.0": "==5.2.1"},
     "flake8": {
         "6.1": "==3.4.1"     # Tested 3.5.0; 3.6.0 does not work
     },
     "gdata": {"6.1": "==2.0.18"},
     "gevent": {
@@ -74,27 +75,28 @@
     "jupyter-server": {"0": "<1.20.0"},
     "lessc": {"0": ">=3.0.0"},
     "lxml": {"6.1": ">=3.4.1", "3.6": "==3.7.1", "3.7": "==4.2.3", "3.8": "==4.6.1"},
     "mccabe": {"0": "<0.7.0,>=0.6.0"},
     "Mako": {
         "6.1": "==1.0.0", "7.0": "==1.0.1", "8.0": "==1.0.4", "10.0": ">=1.0.4",
     },
-    "MarkupSafe": {"6.1": ">=0.23", "0": "<2.1.0"},  # Tested 1.0
+    "MarkupSafe": {"6.1": "==0.23", "14.0": "==1.1.0", "0": "<2.1.0"},  # Tested 1.0
     "matplotlib": {
         "10.0": "==3.0.3",
-        "13.0": "==3.4.1",
-        # "3.6": "==3.0.3",
+        # "13.0": "==3.4.1",
+        "3.6": "==3.0.3",
         # "3.7": "==3.4.1"
+        "3.7": "<3.4.0"     # Experimental!
     },
     "mock": {"6.1": "==1.0.1", "8.0": "==2.0.0"},
     "nbconvert": {"0": "==6.0.7"},
     "odoo_score": {"6.1": "==1.0.1", "10.0": ">=2.0.0"},
     "ofxparse": {"6.1": "==0.16"},
     "pandas": {"3.7": ">=0.22.0,<=1.1.0"},
-    "passlib": {"6.1": "==1.6.2", "10.0": "==1.6.5"},
+    "passlib": {"6.1": "==1.6.2", "10.0": "==1.6.5", "16.0": ">=1.7.0"},
     "Pillow": {
         "6.1": "==3.4.1",
         "7.0": "==3.4.2",
         "8.0": "==3.4.1",
         "11.0": "==4.0.0",
         "15.0": ">=7.0.0",
         "3.6": "==4.0.0",
@@ -110,37 +112,37 @@
         "12.0": ">=2.8.3",
         "0": ">=2.7.4",
     },
     "pycodestyle": {"0": "==2.3.1"},
     "pydot": {"6.1": "==1.0.2", "8.0": "==1.2.3"},
     "pyflakes": {"0": "pyflakes<1.6.0,>=1.5.0"},
     "Pygments": {
-        "2.7": "<2.6.0",
+        "10.0": "==2.2.0",
         "3.5": ">=2.7.0"
     },
     "pygount": {"3.7": "==1.2.0"},
     "pylint": {
         "2.7": "<2.0.0",
         "3.5": "<2.7.0",
         "3.6": "<2.14.0",
         "3.7": "<2.15.0",
     },
     "pylint-odoo": {
         "2.7": "==3.5.0",
         "3.5": "<=8.0.0",
-        "3.8": ">=3.5.0",
+        "3.8": ">=3.5.0<=8.0.0",
     },
     "pylint-plugin-utils": {
         "2.7": "==0.2.6",
         "3.5": "==0.5",
         "3.6": ">=0.7",
     },
     "pyopenssl": {"0": ">=16.2.0"},  # by MQT
     "pyotp": {"2.7": "==2.3.0", "3.5": ">=2.4.0"},
-    "pyPDF2": {"2.7": "==1.28.4", "3.5": ">=2.0", "3.6": ">=2.0", "3.7": ">=2.0"},
+    "pyPDF2": {"2.7": "==1.28.4", "3.5": "<2.0"},
     "pysftp": {"6.1": ">=0.2.9"},
     "pyparsing": {"6.1": "==1.5.7", "7.0": "==2.0.3", "10.0": "==2.1.10"},
     "pyPdf": {"6.1": "==1.13"},
     "pyserial": {"6.1": "==2.7", "10.0": ">=3.1.1"},
     "Python-Chart": {"6.1": "==1.39"},
     "python-dateutil": {
         "6.1": "==1.5", "7.0": "==2.4.0", "8.0": "==2.5.3", "11.0": "==2.5.3"
@@ -159,24 +161,26 @@
     "pyxb": {"6.1": "==1.2.5", "12.0": "==1.2.6"},
     "PyWebDAV": {"6.1": "<0.9.8"},
     "PyYAML": {"6.1": "==3.11", "8.0": "==3.12", "3.7": "==3.13"},
     "qrcode": {"6.1": "==5.0.1", "7.0": "==5.1", "10.0": "==5.3"},
     "readme-renderer" : {"2.7": "<25.0", "3.5": "<29.0", "3.6": ">=30.0"},
     "restructuredtext_lint": {"6.1": "==0.12.2", "0": "==1.1.3"},
     "reportlab": {"6.1": "==3.1.44", "10.0": "==3.3.0"},
-    "requests": {"6.1": "==2.6.0", "10.0": "==2.11.1"},
+    "requests": {"6.1": "==2.6.0", "10.0": ">=2.11.1"},
+    "sentry-sdk": {"0": "<1.12.0"},
     "simplejson": {"6.1": "==3.5.3", "10.0": ">=3.5.3"},
     "six": {"6.1": "==1.7.3", "7.0": "==1.9.0", "10.0": ">=1.10.0"},
     "Sphinx": {"2.7": "==1.2.3", "3.7": ">=2.4.0"},
     "suds": {"6.1": "==0.4"},
     "suds-jurko": {"6.1": "==0.6"},
-    "translators": {"3.7": "<5.2.0"},
+    "translators": {"0": "<5.1.0"},
     "unicodecsv": {"6.1": ">=0.14.1"},
     "unidecode": {"6.1": "==0.4.17", "10.0": "<=1.2.0", "11.0": ">1.2.0"},
     "unittest2": {"6.1": "==0.5.1", "11.0": ">=1.0.0"},
+    "urllib3": {"3.5": "<1.26"},
     "validate_email": {"6.1": ">=1.3"},
     "vatnumber": {"6.1": "==1.2"},
     "vobject": {"6.1": "==0.6.6", "7.0": "==0.9.3"},  # Tested 0.9.5
     "Werkzeug": {
         "6.1": "==0.9.6",
         "10.0": "==0.11.11",
         "11.0": "==0.11.15",
@@ -184,14 +188,15 @@
     },
     "wkhtmltopdf": {"6.1": "==0.12.1", "10.0": "==0.12.4", "12.0": "==0.12.5"},
     "wsgiref": {"6.1": "==0.1.2"},
     "XlsxWriter": {"6.1": "==0.9.3"},  # Tested 1.0.2
     "xlrd": {"6.1": "==1.0.0"},
     "xlwt": {"6.1": "==0.7.5", "10.0": "==1.1.2", "12.0": "==1.3"},
     "z0bug_odoo": {"6.1": "==1.0.1", "10.0": ">=2.0.0"},
+    "zeep": {"0": "==2.4.0"},
     "zerobug": {"6.1": "==1.0.1", "10.0": ">=2.0.0"},
 }
 ALIAS = {
     "babel": "Babel",
     "click": "Click",
     "crypto": "pycrypto",
     "crypto.cipher": "pycrypto",
@@ -225,15 +230,15 @@
     "stdnum": "python-stdnum",
     "usb": "pyusb",
     "werkzeug": "Werkzeug",
     "xlsxwriter": "XlsxWriter",
 }
 ALIAS3 = {
     "PyWebDAV": "PyWebDAV3",
-    "pyPdf": "pyPDF2",
+    # "pyPdf": "pyPDF2",
     # "python-ldap": "pyldap",  # pyldap is a fork!
     "python-dev": "python3-dev",
     "python3-ldap": "ldap3",
 }
 FORCE_ALIAS2 = {
     "docutils==0.12": "docutils==0.14",
     "pytz==2014.4": "pytz>=2014.4",
@@ -242,48 +247,45 @@
     "zeep==4.0.0": "zeep==2.4.0",
     "python-ldap": "python-ldap==3.1.0",
     "Mako==1.0.4": "Mako>=1.0.4",
     "rich": "rich<=12.0.0",
     "importlib-metadata": "importlib-metadata==4.8.3",
     "pygount": "pygount<=1.2.0",
     "pandas": "pandas>=0.22.0,<=1.1.0",
-    "matplotlib": "matplotlib==3.4.1",
 }
 FORCE_ALIAS3 = {
     "docutils==0.12": "docutils==0.16",
     "pytz==2014.4": "pytz>=2014.4",
     "pytz==2014.10": "pytz>=2014.10",
     "pytz==2016.7": "pytz>=2016.7",
     "pytz==2019.3": "pytz>=2019.3",
     "zeep==4.0.0": "zeep==2.4.0",
     "python-ldap": "python-ldap==3.1.0",
-    "translators": "translators<5.2.0",
     "Mako==1.0.4": "Mako>=1.0.4",
     "rich": "rich<=12.0.0",
     "importlib-metadata": "importlib-metadata==4.8.3",
     "pygount": "pygount<=1.2.0",
     "pandas": "pandas>=0.22.0,<=1.1.0",
-    "matplotlib": "matplotlib==3.4.1",
 }
 PIP_SECURE_PACKAGES = [
     "urllib3[secure]",
     "cryptography",
     "pyOpenSSL",
     "idna",
     "certifi",
     "asn1crypto",
     "pyasn1",
 ]
 PIP_TEST_PACKAGES = [
     "astroid",
     "Click",
     "configparser",
-    "codecov",
+    # "codecov",
     "coverage",
-    "coveralls",
+    # "coveralls",
     "docopt",
     "docutils",
     "flake8",
     "GitPython",
     "isort",
     "lazy_object_proxy",
     "lxml",
@@ -316,17 +318,17 @@
     "z0bug_odoo",
     "zerobug",
 ]
 PIP3_TEST_PACKAGES = [
     "astroid",
     "Click",
     "configparser",
-    "codecov",
+    # "codecov",
     "coverage",
-    "coveralls",
+    # "coveralls",
     "docopt",
     "docutils",
     "flake8",
     "GitPython",
     "isort",
     "lazy_object_proxy",
     "lxml",
@@ -425,15 +427,15 @@
     "Python-Chart",
     "python-ldap",
     "python-dateutil",
     "python-openid",
     "python-plus",
     "pydot",
     "pyparsing",
-    "pypdf",  # with PY3 becomes pyPDF2
+    "pyPdf",
     "pyserial",
     "pytz",
     "reportlab",
     "simplejson",
     "six",
     "stdnum",
     "vatnumber",
@@ -668,15 +670,17 @@
                             break
                     elif v == odoo_ver:
                         valid_ver = True
                         if min_v:
                             break
             if min_v:
                 full_item = merge_item_version(
-                    full_item, "%s%s" % (item, REQVERSION[item][min_v]))
+                    full_item,
+                    "%s%s" % (item, REQVERSION[item][min_v]),
+                    ignore_error=True)
     item = python_plus.qsplit(item)[0].strip()
     full_item = python_plus.qsplit(full_item)[0].strip()
     full_item = re.sub(' *([<=>]+) *', r'\1', full_item.strip())
     if pyver and pyver.startswith("2"):
         if full_item in FORCE_ALIAS2:
             full_item = FORCE_ALIAS2[full_item]
         else:
@@ -718,39 +722,49 @@
             ix += x.end()
         else:
             items.append(full_item[ix:])
             ix = len(full_item)
     return items
 
 
-def merge_item_version(left, right):
+def merge_item_version(left, right, ignore_error=False):
     split_left = split_versions(left)
     split_right = split_versions(right)
     ix_right = 1
     while ix_right < len(split_right):
         op = split_right[ix_right]
         if op not in split_left:
-            split_left.append(op)
-            ix_right += 1
-            split_left.append(split_right[ix_right])
+            if op == "==" and any([x for x in split_left if ("<" in x or ">" in x)]):
+                ix_right += 1
+                split_left = [split_left[0], op, split_right[ix_right]]
+            elif (">" not in op and "<" not in op) or "==" not in split_left:
+                split_left.append(op)
+                ix_right += 1
+                split_left.append(split_right[ix_right])
+            else:
+                ix_right += 1
             ix_right += 1
             if ix_right < len(split_right) and split_right[ix_right] == ",":
                 split_left.append(split_right[ix_right])
                 ix_right += 1
         else:
             ix_right += 1
             ver_right = split_right[ix_right]
             ix_right += 2
             ix_left = split_left.index(op) + 1
             ver_left = split_left[ix_left]
 
             if op == "==":
                 if ver_left != ver_right:
-                    sys.stderr.write("Version mismatch: %s %s\n" % (left, right))
-
+                    if not ignore_error:
+                        sys.stderr.write(
+                            "Modules version requirements mismatch: <%s> <%s>\n"
+                            % (left, right))
+                    if ver_right > ver_left:
+                        split_left[ix_left] = ver_right
             elif "<" in op:
                 split_left[ix_left] = maxver(ver_left, ver_right)
 
             else:
                 split_left[ix_left] = minver(ver_left, ver_right)
 
     if split_left[-1] == ",":
@@ -1083,15 +1097,18 @@
     ctx["with_version"] = True
     ctx["itypes"] = "python"
     ctx["opt_verbose"] = False
     ctx["base_pkgs"] = False
     ctx["rpc_pkgs"] = False
     ctx["test_pkgs"] = False
     ctx["oca_dependencies"] = False
-    ctx["opt_fn"] = "/".join([ctx["odoo_dir"], "requirements.txt"])
+    if os.path.isdir(os.path.join(ctx["odoo_dir"], "venv_odoo")):
+        ctx["opt_fn"] = os.path.join(ctx["odoo_dir"], "venv_odoo", "requirements.txt")
+    else:
+        ctx["opt_fn"] = os.path.join(ctx["odoo_dir"], "requirements.txt")
     return ctx
 
 
 def search_4_odoo_dir(ctx):
     for ldir in ("~/odoo/%s", "~/odoo_%s", "~/odoo-%s", "~/odoo%s", "~/%s"):
         if os.path.isdir(os.path.join(os.path.expanduser(ldir % ctx["odoo_ver"]))):
             ctx["odoo_dir"] = os.path.join(os.path.expanduser(ldir % ctx["odoo_ver"]))
```

### Comparing `python_plus-2.0.5/python_plus/scripts/vem.sh` & `python_plus-2.0.6/python_plus/scripts/vem.sh`

 * *Files 1% similar despite different names*

```diff
@@ -45,19 +45,19 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.5
+__version__=2.0.6
 
 declare -A PY3_PKGS
 NEEDING_PKGS="future clodoo configparser os0 z0lib"
-DEV_PKGS="click coveralls codecov flake8 pycodestyle pylint"
+DEV_PKGS="click flake8 pycodestyle pylint"
 SUP_PKGS="future python-plus"
 SECURE_PKGS="urllib3[secure] cryptography pyOpenSSL idna certifi asn1crypto pyasn1"
 EI_PKGS="(distribute)"
 BZR_PKGS="(aeroolib)"
 WGET_PKGS="(pychart|python-chart)"
 GIT_PKGS="(openupgradelib|prestapyt)"
 PYBIN_PKGS="(dateutil|ldap|openid)"
@@ -199,15 +199,15 @@
     local cmd fn mime tt wh x
     fn="$1"
     tt="$2"
     [[ -z $3 ]] && wh="all" || wh="$3"
 
     cmd="$LIST_REQ"
     [[ -n $tt ]] && cmd="$cmd -qt $tt -BP" || cmd="$cmd -qt python -BP"
-    [[ $opt_dev -ne 0 && $wh =~ (all|dev)  ]] && cmd="${cmd}TR"
+    [[ $opt_dev -ne 0 && $wh =~ (all|dev) ]] && cmd="${cmd}TR"
     [[ $wh =~ "cur" ]] && cmd="${cmd}C"
     [[ -n "$opt_pyver" ]] && cmd="$cmd -y$opt_pyver"
     [[ -n "$opt_oever" && $wh =~ (all|oe) ]] && cmd="$cmd -b$opt_oever"
     [[ -n "$opt_oepath" && $wh =~ (all|oe) ]] && cmd="$cmd -p$opt_oepath"
     x="$opt_deps"
     [[ -d $HOME/OCA ]] && x="$x,${HOME}/OCA"
     [[ -d $HOME/maintainer-tools ]] && x="$x,${HOME}/maintainer-tools"
@@ -1344,16 +1344,17 @@
 SAVED_HOME=$HOME
 SAVED_HOME_DEVEL=$HOME_DEVEL
 SAVED_PYTHONPATH=$PYTHONPATH
 PRINTED_PIPVER=0
 [[ $opt_alone -ne 0 ]] && PYTHONPATH=""
 FLAG=">"
 [[ $opt_dry_run -eq 0 ]] && FLAG="\$"
-[[ -f $TDIR/list_requirements.py ]] && LIST_REQ="$TDIR/list_requirements.py" || LIST_REQ=$(which list_requirements.py 2>/dev/null)
+[[ -f $TDIR/list_requirements.py ]] && LIST_REQ="$TDIR/list_requirements.py" || LIST_REQ=$(whereis list_requirements.py|head -n1|cut -d: -f2|tr -d " ")
 [[ -z $LIST_REQ ]] && echo "Command list_requirements.py not found!" && exit 1
+chmod -c +x $LIST_REQ
 
 if [[ $action == "rm" ]]; then
   [[ $PWD == $(readlink -f $p2) ]] && cd
   rm -fR $p2
   [[ -n "${BASH-}" || -n "${ZSH_VERSION-}" ]] && hash -r 2>/dev/null
   unset PYTHON PIP
   exit 0
```

### Comparing `python_plus-2.0.5/python_plus/__init__.py` & `python_plus-2.0.6/python_plus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 __author__ = 'Antonio Maria Vigliotti'
 __license__ = 'L-GPL'
 __copyright__ = 'Copyright 2018-2023 SHS-AV srl'
 __ver_major__ = 0
 __ver_minor__ = 1
 __ver_patch__ = 3
 __ver_sub__ = '6'
-__version__ = '2.0.5'
+__version__ = '2.0.6'
 
 PYCODESET = 'utf-8'
 if PY3:
     text_type = unicode = str
     bytestr_type = bytes
 elif PY2:
     # unicode exist only for python2
```

### Comparing `python_plus-2.0.5/python_plus/vem.man` & `python_plus-2.0.6/python_plus/vem.man`

 * *Files identical despite different names*

### Comparing `python_plus-2.0.5/python_plus.egg-info/SOURCES.txt` & `python_plus-2.0.6/python_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_plus-2.0.5/python_plus.egg-info/PKG-INFO` & `python_plus-2.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,158 +1,160 @@
-Metadata-Version: 1.2
-Name: python-plus
-Version: 2.0.5
+Metadata-Version: 2.1
+Name: python_plus
+Version: 2.0.6
 Summary: python useful function
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        Python supplemental features
-        ----------------------------
-        
-        python-plus adds various features to python 2 and python 3 programs.
-        It is designed to be used as integration of pypi future to help to port your code from Python 2 to Python 3 and still have it run on Python 2.
-        
-        
-        list_requirements.py: list environment requirements
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        This command is an internal command of python-plus but may be used as own command.
-        list_requirements.py dispays the pypi and binaries packages needed to create a virtual environment.
-        It is specially designed to show Odoo requirements.
-        Passing Odoo path it reads requirements.txt files in path and setup directories of OCA repositories.
-        
-        vem: virtual environment manager
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        This command is an interactive tool with some nice features to manage standard virtual environment.
-        Mainly it works ad standard pip but inside a specific virtual environment.
-        
-        vem: virtual environment manager
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            Usage: vem.sh [-h][-a list][-BCD][-d paths][-E distro][-f][-F name][-gkIi][-l iso][-n][-O version][-o dir][-p pyver][-q][-r file][-stVvy] p3 p4 p5 p6 p7 p8 p9
-            Manage virtual environment
-            action may be: help amend cp check create exec info inspect install merge mv python shell rm show uninstall update test
-             -h --help            this help
-             -a list              bin packages to install (* means wkhtmltopdf,lessc)
-             -B                   use unstable packages: -B testpypi / -BB from ~/tools / -BBB from ~/pypi / -BBBB link to local ~/pypi
-             -C                   clear cache before executing pip command
-             -D --devel           create v.environment with development packages
-             -d --dep-path paths
-                                  odoo dependencies paths (comma separated)
-             -E --distro distro
-                                  simulate Linux distro: like Ubuntu20 Centos7 etc (requires -n switch)
-             -f --force           force v.environment create, even if exists or inside another virtual env
-             -F name              simulate Linux family: may be RHEL or Debian (requires -n switch)
-             -g --global          install npm packages globally
-             -k --keep            keep python2 executable as python (deprecated)
-             -I --indipendent     run pip in an isolated mode and set home virtual directory
-             -i --isolated        run pip in an isolated mode, ignoring environment variables and user configuration
-             -l --lang iso
-                                  set default language
-             -n --dry_run         do nothing (dry-run)
-             -O --odoo-ver version
-                                  install pypi required by odoo version (amend or create)
-             -o --odoo-path dir
-                                  odoo path used to search odoo requirements
-             -p --python pyver
-                                  python version
-             -q --quiet           silent mode
-             -r --requirement file
-                                  after created v.environment install from the given requirements file
-             -s --system-site-pack
-                                  create v.environment with access to the global site-packages
-             -t --travis          activate environment for travis test
-             -V --version         show version
-             -v --verbose         verbose mode
-             -y --yes             assume yes
-        
-        vem is an interactive tool with some nice features to manage standard virtual environment.
-        
-        Action is one of:
-        
-        * help
-        * amend [OPTIONS] [SRC_VENV]
-        * check [OPTIONS] [SRC_VENV]
-        * cp [OPTIONS] SRC_VENV TGT_ENV
-        * create -p PYVER [OPTIONS] [VENV]
-        * exec [OPTIONS] [VENV] CMD
-        * info [OPTIONS] [VENV] PKG
-        * install [OPTIONS] [VENV] PKG
-        * merge [OPTIONS] SRC_VENV TGT_ENV
-        * mv [OPTIONS] SRC_VENV TGT_ENV
-        * update [OPTIONS] [VENV] PKG
-        * uninstall [OPTIONS] [VENV] PKG
-        * test [OPTIONS] [VENV]
-        * reset [OPTIONS] [VENV]
-        * show [OPTIONS] [VENV] PKG
-        
-        amend [OPTIONS] [SRC_VENV]
-              Amend package versions against requirements.  May used after 'create' or 'reset' when requirements are changed.
-        
-        check [OPTIONS] [SRC_VENV]
-              Compare package versions against requirements.  May be used after 'create' or 'reset' to check virtual environment
-              consistency.
-        
-        cp [OPTIONS] SRC_VENV TGT_ENV
-              Copy SOURCE environment directory to TGT_ENV, like the bash command 'cp' and  set  relative  path  inside  virtual
-              environment to aim the new directory name.
-              Copying virtual environments is not well supported.
-              Each virtualenv has path information hard-coded into it, and there may be cases where the copy code does not know it needs to update a particular file.
-              Use with caution.
-        
-        create -p PYVER [OPTIONS] VENV
-              Create  a  new  virtual environment directory VENV like virtualenv command but with some nice features.  Switch -p
-              declare which python version will be used to create new environment.
-              This action can install various python packages to create a ready to use environment directory.
-              See -I -D -O -o -r switches to furthermore information.
-        
-        exec [OPTIONS] [SRC_VENV] CMD ...
-              Execute a command in virtual environment. Enclose command by quotes.
-        
-        info [OPTIONS] [SRC_VENV] PKG
-              Show information about pypi package if installed in virtual environment (alias of show)
-        
-        install [OPTIONS] [SRC_VENV] PKG
-              Install pypi package or bin package into virtual environment.
-              Warning! currently just 2 bin packages can be installed: wkhtmltopdf and lessc
-        
-        show [OPTIONS] [SRC_VENV] PKG
-              Show information about pypi package if installed in virtual environment (alias of info)
-        
-        uninstall [OPTIONS] [SRC_VENV] PKG
-              Uninstall pypi package from virtual environment.
-        
-        update [OPTIONS] [SRC_VENV] PKG
-              Upgrade pypi package in virtual environment.
-        
-        History
-        -------
-        
-        2.0.4 (2022-12-15)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * [IMP] Package version adjustment
-        * [IMP] vem: amend show current package version
-        * [IMP] vem: no python2 warning in linux kernel 3
-        * [FIX] vem: best recognition of python version
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: unit test virtual environment venv
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
+
+
+Python supplemental features
+----------------------------
+
+python-plus adds various features to python 2 and python 3 programs.
+It is designed to be used as integration of pypi future to help to port your code from Python 2 to Python 3 and still have it run on Python 2.
+
+
+list_requirements.py: list environment requirements
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+This command is an internal command of python-plus but may be used as own command.
+list_requirements.py dispays the pypi and binaries packages needed to create a virtual environment.
+It is specially designed to show Odoo requirements.
+Passing Odoo path it reads requirements.txt files in path and setup directories of OCA repositories.
+
+vem: virtual environment manager
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+This command is an interactive tool with some nice features to manage standard virtual environment.
+Mainly it works ad standard pip but inside a specific virtual environment.
+
+vem: virtual environment manager
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    Usage: vem.sh [-h][-a list][-BCD][-d paths][-E distro][-f][-F name][-gkIi][-l iso][-n][-O version][-o dir][-p pyver][-q][-r file][-stVvy] p3 p4 p5 p6 p7 p8 p9
+    Manage virtual environment
+    action may be: help amend cp check create exec info inspect install merge mv python shell rm show uninstall update test
+     -h --help            this help
+     -a list              bin packages to install (* means wkhtmltopdf,lessc)
+     -B                   use unstable packages: -B testpypi / -BB from ~/tools / -BBB from ~/pypi / -BBBB link to local ~/pypi
+     -C                   clear cache before executing pip command
+     -D --devel           create v.environment with development packages
+     -d --dep-path paths
+                          odoo dependencies paths (comma separated)
+     -E --distro distro
+                          simulate Linux distro: like Ubuntu20 Centos7 etc (requires -n switch)
+     -f --force           force v.environment create, even if exists or inside another virtual env
+     -F name              simulate Linux family: may be RHEL or Debian (requires -n switch)
+     -g --global          install npm packages globally
+     -k --keep            keep python2 executable as python (deprecated)
+     -I --indipendent     run pip in an isolated mode and set home virtual directory
+     -i --isolated        run pip in an isolated mode, ignoring environment variables and user configuration
+     -l --lang iso
+                          set default language
+     -n --dry_run         do nothing (dry-run)
+     -O --odoo-ver version
+                          install pypi required by odoo version (amend or create)
+     -o --odoo-path dir
+                          odoo path used to search odoo requirements
+     -p --python pyver
+                          python version
+     -q --quiet           silent mode
+     -r --requirement file
+                          after created v.environment install from the given requirements file
+     -s --system-site-pack
+                          create v.environment with access to the global site-packages
+     -t --travis          activate environment for travis test
+     -V --version         show version
+     -v --verbose         verbose mode
+     -y --yes             assume yes
+
+vem is an interactive tool with some nice features to manage standard virtual environment.
+
+Action is one of:
+
+* help
+* amend [OPTIONS] [SRC_VENV]
+* check [OPTIONS] [SRC_VENV]
+* cp [OPTIONS] SRC_VENV TGT_ENV
+* create -p PYVER [OPTIONS] [VENV]
+* exec [OPTIONS] [VENV] CMD
+* info [OPTIONS] [VENV] PKG
+* install [OPTIONS] [VENV] PKG
+* merge [OPTIONS] SRC_VENV TGT_ENV
+* mv [OPTIONS] SRC_VENV TGT_ENV
+* update [OPTIONS] [VENV] PKG
+* uninstall [OPTIONS] [VENV] PKG
+* test [OPTIONS] [VENV]
+* reset [OPTIONS] [VENV]
+* show [OPTIONS] [VENV] PKG
+
+amend [OPTIONS] [SRC_VENV]
+      Amend package versions against requirements.  May used after 'create' or 'reset' when requirements are changed.
+
+check [OPTIONS] [SRC_VENV]
+      Compare package versions against requirements.  May be used after 'create' or 'reset' to check virtual environment
+      consistency.
+
+cp [OPTIONS] SRC_VENV TGT_ENV
+      Copy SOURCE environment directory to TGT_ENV, like the bash command 'cp' and  set  relative  path  inside  virtual
+      environment to aim the new directory name.
+      Copying virtual environments is not well supported.
+      Each virtualenv has path information hard-coded into it, and there may be cases where the copy code does not know it needs to update a particular file.
+      Use with caution.
+
+create -p PYVER [OPTIONS] VENV
+      Create  a  new  virtual environment directory VENV like virtualenv command but with some nice features.  Switch -p
+      declare which python version will be used to create new environment.
+      This action can install various python packages to create a ready to use environment directory.
+      See -I -D -O -o -r switches to furthermore information.
+
+exec [OPTIONS] [SRC_VENV] CMD ...
+      Execute a command in virtual environment. Enclose command by quotes.
+
+info [OPTIONS] [SRC_VENV] PKG
+      Show information about pypi package if installed in virtual environment (alias of show)
+
+install [OPTIONS] [SRC_VENV] PKG
+      Install pypi package or bin package into virtual environment.
+      Warning! currently just 2 bin packages can be installed: wkhtmltopdf and lessc
+
+show [OPTIONS] [SRC_VENV] PKG
+      Show information about pypi package if installed in virtual environment (alias of info)
+
+uninstall [OPTIONS] [SRC_VENV] PKG
+      Uninstall pypi package from virtual environment.
+
+update [OPTIONS] [SRC_VENV] PKG
+      Upgrade pypi package in virtual environment.
+
+History
+-------
+
+2.0.4 (2022-12-15)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] Package version adjustment
+* [IMP] vem: amend show current package version
+* [IMP] vem: no python2 warning in linux kernel 3
+* [FIX] vem: best recognition of python version
+
+
```

### Comparing `python_plus-2.0.5/setup.py` & `python_plus-2.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='python_plus',
-    version='2.0.5',
+    version='2.0.6',
     description='python useful function',
     long_description="""
 Python supplemental features
 ----------------------------
 
 python-plus adds various features to python 2 and python 3 programs.
 It is designed to be used as integration of pypi future to help to port your code from Python 2 to Python 3 and still have it run on Python 2.
```

### Comparing `python_plus-2.0.5/PKG-INFO` & `python_plus-2.0.6/python_plus.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,158 +1,160 @@
-Metadata-Version: 1.2
-Name: python_plus
-Version: 2.0.5
+Metadata-Version: 2.1
+Name: python-plus
+Version: 2.0.6
 Summary: python useful function
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
-Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
-Description: 
-        Python supplemental features
-        ----------------------------
-        
-        python-plus adds various features to python 2 and python 3 programs.
-        It is designed to be used as integration of pypi future to help to port your code from Python 2 to Python 3 and still have it run on Python 2.
-        
-        
-        list_requirements.py: list environment requirements
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        This command is an internal command of python-plus but may be used as own command.
-        list_requirements.py dispays the pypi and binaries packages needed to create a virtual environment.
-        It is specially designed to show Odoo requirements.
-        Passing Odoo path it reads requirements.txt files in path and setup directories of OCA repositories.
-        
-        vem: virtual environment manager
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        This command is an interactive tool with some nice features to manage standard virtual environment.
-        Mainly it works ad standard pip but inside a specific virtual environment.
-        
-        vem: virtual environment manager
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        ::
-        
-            Usage: vem.sh [-h][-a list][-BCD][-d paths][-E distro][-f][-F name][-gkIi][-l iso][-n][-O version][-o dir][-p pyver][-q][-r file][-stVvy] p3 p4 p5 p6 p7 p8 p9
-            Manage virtual environment
-            action may be: help amend cp check create exec info inspect install merge mv python shell rm show uninstall update test
-             -h --help            this help
-             -a list              bin packages to install (* means wkhtmltopdf,lessc)
-             -B                   use unstable packages: -B testpypi / -BB from ~/tools / -BBB from ~/pypi / -BBBB link to local ~/pypi
-             -C                   clear cache before executing pip command
-             -D --devel           create v.environment with development packages
-             -d --dep-path paths
-                                  odoo dependencies paths (comma separated)
-             -E --distro distro
-                                  simulate Linux distro: like Ubuntu20 Centos7 etc (requires -n switch)
-             -f --force           force v.environment create, even if exists or inside another virtual env
-             -F name              simulate Linux family: may be RHEL or Debian (requires -n switch)
-             -g --global          install npm packages globally
-             -k --keep            keep python2 executable as python (deprecated)
-             -I --indipendent     run pip in an isolated mode and set home virtual directory
-             -i --isolated        run pip in an isolated mode, ignoring environment variables and user configuration
-             -l --lang iso
-                                  set default language
-             -n --dry_run         do nothing (dry-run)
-             -O --odoo-ver version
-                                  install pypi required by odoo version (amend or create)
-             -o --odoo-path dir
-                                  odoo path used to search odoo requirements
-             -p --python pyver
-                                  python version
-             -q --quiet           silent mode
-             -r --requirement file
-                                  after created v.environment install from the given requirements file
-             -s --system-site-pack
-                                  create v.environment with access to the global site-packages
-             -t --travis          activate environment for travis test
-             -V --version         show version
-             -v --verbose         verbose mode
-             -y --yes             assume yes
-        
-        vem is an interactive tool with some nice features to manage standard virtual environment.
-        
-        Action is one of:
-        
-        * help
-        * amend [OPTIONS] [SRC_VENV]
-        * check [OPTIONS] [SRC_VENV]
-        * cp [OPTIONS] SRC_VENV TGT_ENV
-        * create -p PYVER [OPTIONS] [VENV]
-        * exec [OPTIONS] [VENV] CMD
-        * info [OPTIONS] [VENV] PKG
-        * install [OPTIONS] [VENV] PKG
-        * merge [OPTIONS] SRC_VENV TGT_ENV
-        * mv [OPTIONS] SRC_VENV TGT_ENV
-        * update [OPTIONS] [VENV] PKG
-        * uninstall [OPTIONS] [VENV] PKG
-        * test [OPTIONS] [VENV]
-        * reset [OPTIONS] [VENV]
-        * show [OPTIONS] [VENV] PKG
-        
-        amend [OPTIONS] [SRC_VENV]
-              Amend package versions against requirements.  May used after 'create' or 'reset' when requirements are changed.
-        
-        check [OPTIONS] [SRC_VENV]
-              Compare package versions against requirements.  May be used after 'create' or 'reset' to check virtual environment
-              consistency.
-        
-        cp [OPTIONS] SRC_VENV TGT_ENV
-              Copy SOURCE environment directory to TGT_ENV, like the bash command 'cp' and  set  relative  path  inside  virtual
-              environment to aim the new directory name.
-              Copying virtual environments is not well supported.
-              Each virtualenv has path information hard-coded into it, and there may be cases where the copy code does not know it needs to update a particular file.
-              Use with caution.
-        
-        create -p PYVER [OPTIONS] VENV
-              Create  a  new  virtual environment directory VENV like virtualenv command but with some nice features.  Switch -p
-              declare which python version will be used to create new environment.
-              This action can install various python packages to create a ready to use environment directory.
-              See -I -D -O -o -r switches to furthermore information.
-        
-        exec [OPTIONS] [SRC_VENV] CMD ...
-              Execute a command in virtual environment. Enclose command by quotes.
-        
-        info [OPTIONS] [SRC_VENV] PKG
-              Show information about pypi package if installed in virtual environment (alias of show)
-        
-        install [OPTIONS] [SRC_VENV] PKG
-              Install pypi package or bin package into virtual environment.
-              Warning! currently just 2 bin packages can be installed: wkhtmltopdf and lessc
-        
-        show [OPTIONS] [SRC_VENV] PKG
-              Show information about pypi package if installed in virtual environment (alias of info)
-        
-        uninstall [OPTIONS] [SRC_VENV] PKG
-              Uninstall pypi package from virtual environment.
-        
-        update [OPTIONS] [SRC_VENV] PKG
-              Upgrade pypi package in virtual environment.
-        
-        History
-        -------
-        
-        2.0.4 (2022-12-15)
-        ~~~~~~~~~~~~~~~~~~
-        
-        * [IMP] Package version adjustment
-        * [IMP] vem: amend show current package version
-        * [IMP] vem: no python2 warning in linux kernel 3
-        * [FIX] vem: best recognition of python version
-        
+Project-URL: Source, https://github.com/zeroincombenze/tools
 Keywords: unit test virtual environment venv
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: System Shells
+
+
+Python supplemental features
+----------------------------
+
+python-plus adds various features to python 2 and python 3 programs.
+It is designed to be used as integration of pypi future to help to port your code from Python 2 to Python 3 and still have it run on Python 2.
+
+
+list_requirements.py: list environment requirements
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+This command is an internal command of python-plus but may be used as own command.
+list_requirements.py dispays the pypi and binaries packages needed to create a virtual environment.
+It is specially designed to show Odoo requirements.
+Passing Odoo path it reads requirements.txt files in path and setup directories of OCA repositories.
+
+vem: virtual environment manager
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+This command is an interactive tool with some nice features to manage standard virtual environment.
+Mainly it works ad standard pip but inside a specific virtual environment.
+
+vem: virtual environment manager
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+::
+
+    Usage: vem.sh [-h][-a list][-BCD][-d paths][-E distro][-f][-F name][-gkIi][-l iso][-n][-O version][-o dir][-p pyver][-q][-r file][-stVvy] p3 p4 p5 p6 p7 p8 p9
+    Manage virtual environment
+    action may be: help amend cp check create exec info inspect install merge mv python shell rm show uninstall update test
+     -h --help            this help
+     -a list              bin packages to install (* means wkhtmltopdf,lessc)
+     -B                   use unstable packages: -B testpypi / -BB from ~/tools / -BBB from ~/pypi / -BBBB link to local ~/pypi
+     -C                   clear cache before executing pip command
+     -D --devel           create v.environment with development packages
+     -d --dep-path paths
+                          odoo dependencies paths (comma separated)
+     -E --distro distro
+                          simulate Linux distro: like Ubuntu20 Centos7 etc (requires -n switch)
+     -f --force           force v.environment create, even if exists or inside another virtual env
+     -F name              simulate Linux family: may be RHEL or Debian (requires -n switch)
+     -g --global          install npm packages globally
+     -k --keep            keep python2 executable as python (deprecated)
+     -I --indipendent     run pip in an isolated mode and set home virtual directory
+     -i --isolated        run pip in an isolated mode, ignoring environment variables and user configuration
+     -l --lang iso
+                          set default language
+     -n --dry_run         do nothing (dry-run)
+     -O --odoo-ver version
+                          install pypi required by odoo version (amend or create)
+     -o --odoo-path dir
+                          odoo path used to search odoo requirements
+     -p --python pyver
+                          python version
+     -q --quiet           silent mode
+     -r --requirement file
+                          after created v.environment install from the given requirements file
+     -s --system-site-pack
+                          create v.environment with access to the global site-packages
+     -t --travis          activate environment for travis test
+     -V --version         show version
+     -v --verbose         verbose mode
+     -y --yes             assume yes
+
+vem is an interactive tool with some nice features to manage standard virtual environment.
+
+Action is one of:
+
+* help
+* amend [OPTIONS] [SRC_VENV]
+* check [OPTIONS] [SRC_VENV]
+* cp [OPTIONS] SRC_VENV TGT_ENV
+* create -p PYVER [OPTIONS] [VENV]
+* exec [OPTIONS] [VENV] CMD
+* info [OPTIONS] [VENV] PKG
+* install [OPTIONS] [VENV] PKG
+* merge [OPTIONS] SRC_VENV TGT_ENV
+* mv [OPTIONS] SRC_VENV TGT_ENV
+* update [OPTIONS] [VENV] PKG
+* uninstall [OPTIONS] [VENV] PKG
+* test [OPTIONS] [VENV]
+* reset [OPTIONS] [VENV]
+* show [OPTIONS] [VENV] PKG
+
+amend [OPTIONS] [SRC_VENV]
+      Amend package versions against requirements.  May used after 'create' or 'reset' when requirements are changed.
+
+check [OPTIONS] [SRC_VENV]
+      Compare package versions against requirements.  May be used after 'create' or 'reset' to check virtual environment
+      consistency.
+
+cp [OPTIONS] SRC_VENV TGT_ENV
+      Copy SOURCE environment directory to TGT_ENV, like the bash command 'cp' and  set  relative  path  inside  virtual
+      environment to aim the new directory name.
+      Copying virtual environments is not well supported.
+      Each virtualenv has path information hard-coded into it, and there may be cases where the copy code does not know it needs to update a particular file.
+      Use with caution.
+
+create -p PYVER [OPTIONS] VENV
+      Create  a  new  virtual environment directory VENV like virtualenv command but with some nice features.  Switch -p
+      declare which python version will be used to create new environment.
+      This action can install various python packages to create a ready to use environment directory.
+      See -I -D -O -o -r switches to furthermore information.
+
+exec [OPTIONS] [SRC_VENV] CMD ...
+      Execute a command in virtual environment. Enclose command by quotes.
+
+info [OPTIONS] [SRC_VENV] PKG
+      Show information about pypi package if installed in virtual environment (alias of show)
+
+install [OPTIONS] [SRC_VENV] PKG
+      Install pypi package or bin package into virtual environment.
+      Warning! currently just 2 bin packages can be installed: wkhtmltopdf and lessc
+
+show [OPTIONS] [SRC_VENV] PKG
+      Show information about pypi package if installed in virtual environment (alias of info)
+
+uninstall [OPTIONS] [SRC_VENV] PKG
+      Uninstall pypi package from virtual environment.
+
+update [OPTIONS] [SRC_VENV] PKG
+      Upgrade pypi package in virtual environment.
+
+History
+-------
+
+2.0.4 (2022-12-15)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] Package version adjustment
+* [IMP] vem: amend show current package version
+* [IMP] vem: no python2 warning in linux kernel 3
+* [FIX] vem: best recognition of python version
+
+
```

### Comparing `python_plus-2.0.5/README.rst` & `python_plus-2.0.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 =================
-python_plus 2.0.4
+python_plus 2.0.6
 =================
 
 
 
 |Maturity| |Build Status| |Coverage Status| |license gpl|
 
 
@@ -288,16 +288,24 @@
     ./install_tools.sh -Ud
     source /opt/odoo/devel/activate_tools
 
 
 History
 -------
 
-2.0.4.1 (2022-12-23)
-~~~~~~~~~~~~~~~~~~~~
+2.0.6 (2023-03-24)
+~~~~~~~~~~~~~~~~~~
+
+* [IMP] list_requirements.py: cryptography, pypdf2, requests & urllib3 version adjustment
+* [IMP] list_requirements.py: pypdf and pypdf2 version adjustment
+* [IMP] list_requirements.py: best resolution when versions conflict
+* [IMP] vem: set list_requirements.py executable
+
+2.0.5 (2022-12-23)
+~~~~~~~~~~~~~~~~~~
 
 * [IMP] list_requirements.py: refactoring version control
 * [IMP] vem: now amend can check current version (with -f switch)
 
 2.0.4 (2022-12-15)
 ~~~~~~~~~~~~~~~~~~
 
@@ -365,21 +373,24 @@
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
 * Antonio Maria Vigliotti <info@shs-av.com>
+Contributors
+------------
+
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2022-12-26
+Last Update / Ultimo aggiornamento: 2023-04-14
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Mature-green.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
 .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
     :target: https://travis-ci.com/zeroincombenze/tools
     :alt: github.com
```

