# Comparing `tmp/plone.stringinterp-2.0.0.tar.gz` & `tmp/plone.stringinterp-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.stringinterp-2.0.0.tar", last modified: Tue Mar 21 22:53:47 2023, max compression
+gzip compressed data, was "plone.stringinterp-2.0.1.tar", last modified: Thu Apr 13 23:10:38 2023, max compression
```

## Comparing `plone.stringinterp-2.0.0.tar` & `plone.stringinterp-2.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:53:47.569575 plone.stringinterp-2.0.0/
--rw-r--r--   0 maurits    (501) staff       (20)     4021 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     7034 2023-03-21 22:53:47.569677 plone.stringinterp-2.0.0/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2086 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:53:47.562406 plone.stringinterp-2.0.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      712 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:53:47.562658 plone.stringinterp-2.0.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:53:47.567294 plone.stringinterp-2.0.0/plone/stringinterp/
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/plone/stringinterp/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    20529 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/plone/stringinterp/adapters.py
--rw-r--r--   0 maurits    (501) staff       (20)     1741 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/plone/stringinterp/browser.py
--rw-r--r--   0 maurits    (501) staff       (20)     9473 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/plone/stringinterp/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1452 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/plone/stringinterp/dollarReplace.py
--rw-r--r--   0 maurits    (501) staff       (20)     1292 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/plone/stringinterp/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:53:47.569359 plone.stringinterp-2.0.0/plone/stringinterp/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/plone/stringinterp/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1708 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/plone/stringinterp/tests/interpolationTests.txt
--rw-r--r--   0 maurits    (501) staff       (20)    12286 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/plone/stringinterp/tests/moreSubstitutionTests.txt
--rw-r--r--   0 maurits    (501) staff       (20)    11090 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/plone/stringinterp/tests/substitutionTests.txt
--rw-r--r--   0 maurits    (501) staff       (20)      728 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/plone/stringinterp/tests/testDocTests.py
--rw-r--r--   0 maurits    (501) staff       (20)    13149 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/plone/stringinterp/tests/wrapperTests.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:53:47.565503 plone.stringinterp-2.0.0/plone.stringinterp.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     7034 2023-03-21 22:53:47.000000 plone.stringinterp-2.0.0/plone.stringinterp.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      944 2023-03-21 22:53:47.000000 plone.stringinterp-2.0.0/plone.stringinterp.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 22:53:47.000000 plone.stringinterp-2.0.0/plone.stringinterp.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-03-21 22:53:47.000000 plone.stringinterp-2.0.0/plone.stringinterp.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-21 22:53:47.000000 plone.stringinterp-2.0.0/plone.stringinterp.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 22:53:47.000000 plone.stringinterp-2.0.0/plone.stringinterp.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      109 2023-03-21 22:53:47.000000 plone.stringinterp-2.0.0/plone.stringinterp.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-21 22:53:47.000000 plone.stringinterp-2.0.0/plone.stringinterp.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       92 2023-03-21 22:53:47.570068 plone.stringinterp-2.0.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1600 2023-03-21 22:53:46.000000 plone.stringinterp-2.0.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:10:38.036750 plone.stringinterp-2.0.1/
+-rw-r--r--   0 maurits    (501) staff       (20)     4130 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     7166 2023-04-13 23:10:38.036956 plone.stringinterp-2.0.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2086 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:10:38.028760 plone.stringinterp-2.0.1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      712 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:10:38.029062 plone.stringinterp-2.0.1/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:10:38.034407 plone.stringinterp-2.0.1/plone/stringinterp/
+-rw-r--r--   0 maurits    (501) staff       (20)       54 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone/stringinterp/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20529 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone/stringinterp/adapters.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1741 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone/stringinterp/browser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9473 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone/stringinterp/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1452 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone/stringinterp/dollarReplace.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1284 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone/stringinterp/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:10:38.036547 plone.stringinterp-2.0.1/plone/stringinterp/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone/stringinterp/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1708 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone/stringinterp/tests/interpolationTests.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    12170 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone/stringinterp/tests/moreSubstitutionTests.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    10974 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone/stringinterp/tests/substitutionTests.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      728 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone/stringinterp/tests/testDocTests.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13033 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone/stringinterp/tests/wrapperTests.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:10:38.031951 plone.stringinterp-2.0.1/plone.stringinterp.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     7166 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone.stringinterp.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      944 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone.stringinterp.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone.stringinterp.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone.stringinterp.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone.stringinterp.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone.stringinterp.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      133 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone.stringinterp.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/plone.stringinterp.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1643 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-13 23:10:38.037546 plone.stringinterp-2.0.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1664 2023-04-13 23:10:37.000000 plone.stringinterp-2.0.1/setup.py
```

### Comparing `plone.stringinterp-2.0.0/CHANGES.rst` & `plone.stringinterp-2.0.1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.1 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (93e1ab65)
+
+
 2.0.0 (2023-03-21)
 ------------------
 
 Breaking changes:
 
 
 - pyupgrade, drop support for Python < 3.8.
```

### Comparing `plone.stringinterp-2.0.0/PKG-INFO` & `plone.stringinterp-2.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.stringinterp
-Version: 2.0.0
+Version: 2.0.1
 Summary: Adaptable string interpolation
 Home-page: https://github.com/plone/plone.stringinterp
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Plone Zope Interpolation
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Provides ``${id}`` style string interpolation using named adapters to look up variables.
 This is meant to provide a trivially simple template system for clients like plone.app.contentrules.
 
 To interpolate a string in context, just follow the pattern::
 
@@ -125,14 +126,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.1 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (93e1ab65)
+
+
 2.0.0 (2023-03-21)
 ------------------
 
 Breaking changes:
 
 
 - pyupgrade, drop support for Python < 3.8.
```

### Comparing `plone.stringinterp-2.0.0/README.rst` & `plone.stringinterp-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `plone.stringinterp-2.0.0/docs/LICENSE.GPL` & `plone.stringinterp-2.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.stringinterp-2.0.0/docs/LICENSE.txt` & `plone.stringinterp-2.0.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.stringinterp-2.0.0/plone/stringinterp/adapters.py` & `plone.stringinterp-2.0.1/plone/stringinterp/adapters.py`

 * *Files identical despite different names*

### Comparing `plone.stringinterp-2.0.0/plone/stringinterp/browser.py` & `plone.stringinterp-2.0.1/plone/stringinterp/browser.py`

 * *Files identical despite different names*

### Comparing `plone.stringinterp-2.0.0/plone/stringinterp/configure.zcml` & `plone.stringinterp-2.0.1/plone/stringinterp/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.stringinterp-2.0.0/plone/stringinterp/dollarReplace.py` & `plone.stringinterp-2.0.1/plone/stringinterp/dollarReplace.py`

 * *Files identical despite different names*

### Comparing `plone.stringinterp-2.0.0/plone/stringinterp/interfaces.py` & `plone.stringinterp-2.0.1/plone/stringinterp/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,14 @@
 class IContextWrapper(Interface):
     """
     Wrap context in order to be able to provide custom strings
     not stored on context
 
     Usage:
 
-    >>> wrapper = IContextWrapper(obj)(m1='A message', m2="Another one")
-    >>> notify(CustomEvent(wrapper))
+    wrapper = IContextWrapper(obj)(m1='A message', m2="Another one")
+    notify(CustomEvent(wrapper))
     """
 
     def __call__(kwargs):
         """ "
         Return wrapped context"""
```

### Comparing `plone.stringinterp-2.0.0/plone/stringinterp/tests/interpolationTests.txt` & `plone.stringinterp-2.0.1/plone/stringinterp/tests/interpolationTests.txt`

 * *Files identical despite different names*

### Comparing `plone.stringinterp-2.0.0/plone/stringinterp/tests/moreSubstitutionTests.txt` & `plone.stringinterp-2.0.1/plone/stringinterp/tests/moreSubstitutionTests.txt`

 * *Files 1% similar despite different names*

```diff
@@ -164,19 +164,15 @@
 
     >>> getAdapter(apage, IStringSubstitution, 'type')()
     'Page'
 
 
 Let's try some non-ASCII::
 
-   >>> import six
-   >>> if six.PY2:
-   ...     apage.setTitle('Plone in Español'.decode('utf8'))
-   ... else:
-   ...     apage.setTitle('Plone in Español')
+   >>> apage.setTitle('Plone in Español')
    >>> getAdapter(apage, IStringSubstitution, 'title')()
    'Plone in Espa\xf1ol'
 
 
 
 Workflow Aware
 --------------
```

### Comparing `plone.stringinterp-2.0.0/plone/stringinterp/tests/substitutionTests.txt` & `plone.stringinterp-2.0.1/plone/stringinterp/tests/substitutionTests.txt`

 * *Files 1% similar despite different names*

```diff
@@ -149,19 +149,15 @@
 
     >>> getAdapter(apage, IStringSubstitution, 'type')()
     'Page'
 
 
 Let's try some non-ASCII::
 
-   >>> import six
-   >>> if six.PY2:
-   ...     apage.setTitle('Plone in Español'.decode('utf8'))
-   ... else:
-   ...     apage.setTitle('Plone in Español')
+   >>> apage.setTitle('Plone in Español')
    >>> getAdapter(apage, IStringSubstitution, 'title')()
    'Plone in Espa\xf1ol'
 
 Workflow Aware
 --------------
 
 Review State
```

### Comparing `plone.stringinterp-2.0.0/plone/stringinterp/tests/testDocTests.py` & `plone.stringinterp-2.0.1/plone/stringinterp/tests/testDocTests.py`

 * *Files identical despite different names*

### Comparing `plone.stringinterp-2.0.0/plone/stringinterp/tests/wrapperTests.txt` & `plone.stringinterp-2.0.1/plone/stringinterp/tests/wrapperTests.txt`

 * *Files 2% similar despite different names*

```diff
@@ -198,19 +198,15 @@
 
     >>> getAdapter(apage, IStringSubstitution, 'type')()
     'Page'
 
 
 Let's try some non-ASCII::
 
-   >>> import six
-   >>> if six.PY2:
-   ...     apage.setTitle('Plone in Español'.decode('utf8'))
-   ... else:
-   ...     apage.setTitle('Plone in Español')
+   >>> apage.setTitle('Plone in Español')
    >>> getAdapter(apage, IStringSubstitution, 'title')()
    'Plone in Espa\xf1ol'
 
 
 
 Workflow Aware
 --------------
```

### Comparing `plone.stringinterp-2.0.0/plone.stringinterp.egg-info/PKG-INFO` & `plone.stringinterp-2.0.1/plone.stringinterp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.stringinterp
-Version: 2.0.0
+Version: 2.0.1
 Summary: Adaptable string interpolation
 Home-page: https://github.com/plone/plone.stringinterp
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Plone Zope Interpolation
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: test
 
 Provides ``${id}`` style string interpolation using named adapters to look up variables.
 This is meant to provide a trivially simple template system for clients like plone.app.contentrules.
 
 To interpolate a string in context, just follow the pattern::
 
@@ -125,14 +126,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.1 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (93e1ab65)
+
+
 2.0.0 (2023-03-21)
 ------------------
 
 Breaking changes:
 
 
 - pyupgrade, drop support for Python < 3.8.
```

### Comparing `plone.stringinterp-2.0.0/plone.stringinterp.egg-info/SOURCES.txt` & `plone.stringinterp-2.0.1/plone.stringinterp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.stringinterp-2.0.0/setup.py` & `plone.stringinterp-2.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.0.0"
+version = "2.0.1"
 
 setup(
     name="plone.stringinterp",
     version=version,
     description="Adaptable string interpolation",
     long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
     classifiers=[
@@ -29,23 +29,25 @@
     author_email="plone-developers@lists.sourceforge.net",
     url="https://github.com/plone/plone.stringinterp",
     license="GPL version 2",
     packages=find_packages(),
     namespace_packages=["plone"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     install_requires=[
         "setuptools",
         "plone.base",
         "plone.memoize",
         "zope.i18n",
+        "Products.PlonePAS",
     ],
     extras_require={
         "test": [
-            "plone.app.contenttypes",
+            "plone.app.contenttypes[test]",
             "plone.app.testing",
             "plone.testing",
         ],
     },
     entry_points="""
         [z3c.autoinclude.plugin]
         target = plone
```

