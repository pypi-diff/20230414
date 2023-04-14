# Comparing `tmp/zope.contentprovider-4.2.1.tar.gz` & `tmp/zope.contentprovider-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zope.contentprovider-4.2.1.tar", last modified: Thu Nov  8 15:32:39 2018, max compression
+gzip compressed data, was "zope.contentprovider-5.0.tar", last modified: Fri Apr 14 06:28:16 2023, max compression
```

## Comparing `zope.contentprovider-4.2.1.tar` & `zope.contentprovider-5.0.tar`

### file list

```diff
@@ -1,42 +1,39 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/
--rw-r--r--   0 mac        (501) staff       (20)     7458 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/bootstrap.py
--rw-r--r--   0 mac        (501) staff       (20)     6415 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)       32 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/COPYRIGHT.txt
--rw-r--r--   0 mac        (501) staff       (20)      109 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/buildout.cfg
--rw-r--r--   0 mac        (501) staff       (20)      223 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      197 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/.coveragerc
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/docs/
--rw-r--r--   0 mac        (501) staff       (20)      228 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/docs/index.rst
--rw-r--r--   0 mac        (501) staff       (20)     4775 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/docs/motivation.rst
--rw-r--r--   0 mac        (501) staff       (20)     9306 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/docs/conf.py
--rw-r--r--   0 mac        (501) staff       (20)     9753 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/docs/tales.rst
--rw-r--r--   0 mac        (501) staff       (20)     7902 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/docs/narr.rst
--rw-r--r--   0 mac        (501) staff       (20)       28 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/docs/changelog.rst
--rw-r--r--   0 mac        (501) staff       (20)     1447 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/docs/api_provider.rst
--rw-r--r--   0 mac        (501) staff       (20)     3238 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/setup.py
--rw-r--r--   0 mac        (501) staff       (20)      117 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/.gitignore
--rw-r--r--   0 mac        (501) staff       (20)      898 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/tox.ini
--rw-r--r--   0 mac        (501) staff       (20)       67 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1367 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/README.rst
--rw-r--r--   0 mac        (501) staff       (20)     2070 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     2600 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/CHANGES.rst
--rw-r--r--   0 mac        (501) staff       (20)        8 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/doc-requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)      539 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/.travis.yml
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope.contentprovider.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     6415 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope.contentprovider.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)        1 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope.contentprovider.egg-info/not-zip-safe
--rw-r--r--   0 mac        (501) staff       (20)        5 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope.contentprovider.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (501) staff       (20)      872 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope.contentprovider.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)      212 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope.contentprovider.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        5 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope.contentprovider.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope.contentprovider.egg-info/dependency_links.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope/
--rw-r--r--   0 mac        (501) staff       (20)       76 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope/contentprovider/
--rw-r--r--   0 mac        (501) staff       (20)     5637 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope/contentprovider/interfaces.py
--rw-r--r--   0 mac        (501) staff       (20)      652 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope/contentprovider/configure.zcml
--rw-r--r--   0 mac        (501) staff       (20)     1440 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope/contentprovider/provider.py
--rw-r--r--   0 mac        (501) staff       (20)      636 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope/contentprovider/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3045 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope/contentprovider/tales.py
--rw-r--r--   0 mac        (501) staff       (20)      910 2018-11-08 15:32:39.000000 zope.contentprovider-4.2.1/src/zope/contentprovider/tests.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:28:16.179208 zope.contentprovider-5.0/
+-rw-r--r--   0 mac        (513) staff       (20)     2788 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      344 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     5405 2023-04-14 06:28:16.179381 zope.contentprovider-5.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1367 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      109 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/buildout.cfg
+-rw-r--r--   0 mac        (513) staff       (20)        8 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/doc-requirements.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:28:16.171321 zope.contentprovider-5.0/docs/
+-rw-r--r--   0 mac        (513) staff       (20)     1447 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/docs/api_provider.rst
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/docs/changelog.rst
+-rw-r--r--   0 mac        (513) staff       (20)     9306 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/docs/conf.py
+-rw-r--r--   0 mac        (513) staff       (20)      228 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/docs/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)     4775 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/docs/motivation.rst
+-rw-r--r--   0 mac        (513) staff       (20)     7902 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/docs/narr.rst
+-rw-r--r--   0 mac        (513) staff       (20)     9753 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/docs/tales.rst
+-rw-r--r--   0 mac        (513) staff       (20)      470 2023-04-14 06:28:16.180072 zope.contentprovider-5.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     3156 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:28:16.163320 zope.contentprovider-5.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:28:16.171782 zope.contentprovider-5.0/src/zope/
+-rw-r--r--   0 mac        (513) staff       (20)       76 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/src/zope/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:28:16.178861 zope.contentprovider-5.0/src/zope/contentprovider/
+-rw-r--r--   0 mac        (513) staff       (20)      636 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/src/zope/contentprovider/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      652 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/src/zope/contentprovider/configure.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     5630 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/src/zope/contentprovider/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)     1441 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/src/zope/contentprovider/provider.py
+-rw-r--r--   0 mac        (513) staff       (20)     3016 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/src/zope/contentprovider/tales.py
+-rw-r--r--   0 mac        (513) staff       (20)      910 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/src/zope/contentprovider/tests.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:28:16.176425 zope.contentprovider-5.0/src/zope.contentprovider.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     5405 2023-04-14 06:28:16.000000 zope.contentprovider-5.0/src/zope.contentprovider.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      840 2023-04-14 06:28:16.000000 zope.contentprovider-5.0/src/zope.contentprovider.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-14 06:28:16.000000 zope.contentprovider-5.0/src/zope.contentprovider.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-14 06:28:16.000000 zope.contentprovider-5.0/src/zope.contentprovider.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-14 06:28:16.000000 zope.contentprovider-5.0/src/zope.contentprovider.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      212 2023-04-14 06:28:16.000000 zope.contentprovider-5.0/src/zope.contentprovider.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-14 06:28:16.000000 zope.contentprovider-5.0/src/zope.contentprovider.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1832 2023-04-14 06:28:15.000000 zope.contentprovider-5.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zope.contentprovider-4.2.1/docs/motivation.rst` & `zope.contentprovider-5.0/docs/motivation.rst`

 * *Files identical despite different names*

### Comparing `zope.contentprovider-4.2.1/docs/conf.py` & `zope.contentprovider-5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.contentprovider-4.2.1/docs/tales.rst` & `zope.contentprovider-5.0/docs/tales.rst`

 * *Files identical despite different names*

### Comparing `zope.contentprovider-4.2.1/docs/narr.rst` & `zope.contentprovider-5.0/docs/narr.rst`

 * *Files identical despite different names*

### Comparing `zope.contentprovider-4.2.1/docs/api_provider.rst` & `zope.contentprovider-5.0/docs/api_provider.rst`

 * *Files identical despite different names*

### Comparing `zope.contentprovider-4.2.1/setup.py` & `zope.contentprovider-5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 # This package is developed by the Zope Toolkit project, documented here:
-# http://docs.zope.org/zopetoolkit
+# http://zopetoolkit.readthedocs.io/
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.contentprovider package"""
 
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
@@ -32,49 +34,49 @@
     'zope.testing',
     'zope.testrunner',
 ]
 
 
 setup(
     name='zope.contentprovider',
-    version='4.2.1',
+    version='5.0',
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     description='Content Provider Framework for Zope Templates',
     long_description=(
         read('README.rst')
         + '\n\n' +
         read('CHANGES.rst')
     ),
     keywords="zope3 content provider",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Topic :: Internet :: WWW/HTTP',
         'Framework :: Zope :: 3',
     ],
     url='https://github.com/zopefoundation/zope.contentprovider',
     license='ZPL 2.1',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['zope'],
+    python_requires='>=3.7',
     extras_require={
         'test': TESTS_REQUIRE,
         'docs': [
             'Sphinx',
             'repoze.sphinx.autointerface',
         ],
     },
@@ -85,11 +87,9 @@
         'zope.interface >= 3.8',
         'zope.location',
         'zope.publisher',
         'zope.schema',
         'zope.tales',
     ],
     include_package_data=True,
-    tests_require=TESTS_REQUIRE,
-    test_suite='zope.contentprovider.tests.test_suite',
     zip_safe=False,
 )
```

### Comparing `zope.contentprovider-4.2.1/README.rst` & `zope.contentprovider-5.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
         :target: https://pypi.python.org/pypi/zope.contentprovider/
         :alt: Latest release
 
 .. image:: https://img.shields.io/pypi/pyversions/zope.contentprovider.svg
         :target: https://pypi.org/project/zope.contentprovider/
         :alt: Supported Python versions
 
-.. image:: https://travis-ci.org/zopefoundation/zope.contentprovider.svg?branch=master
-        :target: https://travis-ci.org/zopefoundation/zope.contentprovider
+.. image:: https://travis-ci.com/zopefoundation/zope.contentprovider.svg?branch=master
+        :target: https://travis-ci.com/zopefoundation/zope.contentprovider
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/zope.contentprovider/badge.svg?branch=master
         :target: https://coveralls.io/github/zopefoundation/zope.contentprovider?branch=master
 
 .. image:: https://readthedocs.org/projects/zopecontentprovider/badge/?version=latest
         :target: https://zopecontentprovider.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
```

### Comparing `zope.contentprovider-4.2.1/LICENSE.txt` & `zope.contentprovider-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.contentprovider-4.2.1/CHANGES.rst` & `zope.contentprovider-5.0/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =========
  Changes
 =========
 
+5.0 (2023-04-14)
+================
+
+- Drop support for Python 2.7, 3.4, 3.5, 3.6.
+
+- Drop support for deprecated ``python setup.py test``.
+
+- Add support for Python 3.8, 3.9, 3.10, 3.11.
+
+
 4.2.1 (2018-11-08)
 ==================
 
 - Fix deprecation warnings.
 
 
 4.2 (2018-10-05)
```

### Comparing `zope.contentprovider-4.2.1/src/zope.contentprovider.egg-info/SOURCES.txt` & `zope.contentprovider-5.0/src/zope.contentprovider.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-.coveragerc
-.gitignore
-.travis.yml
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
-bootstrap.py
 buildout.cfg
 doc-requirements.txt
 setup.cfg
 setup.py
 tox.ini
 docs/api_provider.rst
 docs/changelog.rst
```

### Comparing `zope.contentprovider-4.2.1/src/zope/contentprovider/interfaces.py` & `zope.contentprovider-5.0/src/zope/contentprovider/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Content provider interfaces"""
 
 import zope.component
 import zope.interface
-from zope.interface.interfaces import ObjectEvent, IObjectEvent
+from zope.interface.interfaces import IObjectEvent
+from zope.interface.interfaces import ObjectEvent
 from zope.publisher.interfaces import browser
 from zope.tales import interfaces
 
 
 class IUpdateNotCalled(zope.interface.common.interfaces.IRuntimeError):
     """Update Not Called
 
@@ -30,15 +31,15 @@
 
 class UpdateNotCalled(RuntimeError):
     """Default implementation of `IUpdateNotCalled`."""
 
     def __init__(self, *args):
         if not args:
             args = ('``update()`` was not called yet.',)
-        super(UpdateNotCalled, self).__init__(*args)
+        super().__init__(*args)
 
 
 class IBeforeUpdateEvent(IObjectEvent):
     """A content provider will be updated"""
 
     request = zope.interface.Attribute(
         """The request in which the object is udpated, might also be
@@ -46,15 +47,15 @@
 
 
 @zope.interface.implementer(IBeforeUpdateEvent)
 class BeforeUpdateEvent(ObjectEvent):
     """Default implementation of `IBeforeUpdateEvent`."""
 
     def __init__(self, provider, request=None):
-        super(BeforeUpdateEvent, self).__init__(provider)
+        super().__init__(provider)
         self.request = request
 
 
 class IContentProvider(browser.IBrowserView):
     """A piece of content to be shown on a page.
 
     Objects implementing this interface are providing HTML content when they
```

### Comparing `zope.contentprovider-4.2.1/src/zope/contentprovider/configure.zcml` & `zope.contentprovider-5.0/src/zope/contentprovider/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.contentprovider-4.2.1/src/zope/contentprovider/provider.py` & `zope.contentprovider-5.0/src/zope/contentprovider/provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Simple base class for implementing content providers
 """
 from zope.component import adapter
-from zope.interface import Interface, implementer
+from zope.interface import Interface
+from zope.interface import implementer
 from zope.publisher.browser import BrowserView
 from zope.publisher.interfaces.browser import IBrowserRequest
 
 from zope.contentprovider.interfaces import IContentProvider
 
 
 @implementer(IContentProvider)
 @adapter(Interface, IBrowserRequest, Interface)
 class ContentProviderBase(BrowserView):
     """Base class for content providers"""
 
     def __init__(self, context, request, view):
-        super(ContentProviderBase, self).__init__(context, request)
+        super().__init__(context, request)
         self.__parent__ = view
 
     def update(self):
         pass
 
     def render(self, *args, **kwargs):
         raise NotImplementedError(
```

### Comparing `zope.contentprovider-4.2.1/src/zope/contentprovider/__init__.py` & `zope.contentprovider-5.0/src/zope/contentprovider/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.contentprovider-4.2.1/src/zope/contentprovider/tales.py` & `zope.contentprovider-5.0/src/zope/contentprovider/tales.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Provider TALES expression"""
 import zope.component
+import zope.event
 import zope.interface
 import zope.schema
-import zope.event
 from zope.location.interfaces import ILocation
 from zope.tales import expressions
 
 from zope.contentprovider import interfaces
 
 
 def addTALNamespaceData(provider, context):
@@ -47,15 +47,15 @@
     implementation such as zope.viewlet that will complete all content
     providers' stage one before rendering any of them.
 
     Implements `zope.contentprovider.interfaces.ITALESProviderExpression`
     """
 
     def __call__(self, econtext):
-        name = super(TALESProviderExpression, self).__call__(econtext)
+        name = super().__call__(econtext)
         context = econtext.vars['context']
         request = econtext.vars['request']
         view = econtext.vars['view']
 
         # Try to look up the provider.
         provider = zope.component.queryMultiAdapter(
             (context, request, view), interfaces.IContentProvider, name)
```

### Comparing `zope.contentprovider-4.2.1/src/zope/contentprovider/tests.py` & `zope.contentprovider-5.0/src/zope/contentprovider/tests.py`

 * *Files identical despite different names*

