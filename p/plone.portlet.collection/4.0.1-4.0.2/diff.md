# Comparing `tmp/plone.portlet.collection-4.0.1.tar.gz` & `tmp/plone.portlet.collection-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.portlet.collection-4.0.1.tar", last modified: Tue Mar 21 22:46:26 2023, max compression
+gzip compressed data, was "plone.portlet.collection-4.0.2.tar", last modified: Thu Apr 13 23:41:48 2023, max compression
```

## Comparing `plone.portlet.collection-4.0.1.tar` & `plone.portlet.collection-4.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:46:26.647317 plone.portlet.collection-4.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)     9178 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      162 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    10230 2023-03-21 22:46:26.647623 plone.portlet.collection-4.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)       77 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:46:26.639260 plone.portlet.collection-4.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      686 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:46:26.639665 plone.portlet.collection-4.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:46:26.642962 plone.portlet.collection-4.0.1/plone/portlet/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/plone/portlet/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:46:26.644793 plone.portlet.collection-4.0.1/plone/portlet/collection/
--rw-r--r--   0 maurits    (501) staff       (20)      395 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/plone/portlet/collection/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3986 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/plone/portlet/collection/collection.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10066 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/plone/portlet/collection/collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     1141 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/plone/portlet/collection/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:46:26.634957 plone.portlet.collection-4.0.1/plone/portlet/collection/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:46:26.645672 plone.portlet.collection-4.0.1/plone/portlet/collection/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      187 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/plone/portlet/collection/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      415 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/plone/portlet/collection/profiles/default/portlets.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1501 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/plone/portlet/collection/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:46:26.646904 plone.portlet.collection-4.0.1/plone/portlet/collection/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/plone/portlet/collection/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5970 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/plone/portlet/collection/tests/functional.txt
--rw-r--r--   0 maurits    (501) staff       (20)      947 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/plone/portlet/collection/tests/test_functional_doctest.py
--rw-r--r--   0 maurits    (501) staff       (20)    16311 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/plone/portlet/collection/tests/test_portlet_collection.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:46:26.642614 plone.portlet.collection-4.0.1/plone.portlet.collection.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    10230 2023-03-21 22:46:26.000000 plone.portlet.collection-4.0.1/plone.portlet.collection.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1035 2023-03-21 22:46:26.000000 plone.portlet.collection-4.0.1/plone.portlet.collection.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 22:46:26.000000 plone.portlet.collection-4.0.1/plone.portlet.collection.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       20 2023-03-21 22:46:26.000000 plone.portlet.collection-4.0.1/plone.portlet.collection.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 22:46:26.000000 plone.portlet.collection-4.0.1/plone.portlet.collection.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      327 2023-03-21 22:46:26.000000 plone.portlet.collection-4.0.1/plone.portlet.collection.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-21 22:46:26.000000 plone.portlet.collection-4.0.1/plone.portlet.collection.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1682 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       62 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/requirements-6.0.x.txt
--rw-r--r--   0 maurits    (501) staff       (20)      237 2023-03-21 22:46:26.648399 plone.portlet.collection-4.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1937 2023-03-21 22:46:25.000000 plone.portlet.collection-4.0.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.024917 plone.portlet.collection-4.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)     9287 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      162 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    10339 2023-04-13 23:41:48.025063 plone.portlet.collection-4.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)       77 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.018319 plone.portlet.collection-4.0.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      686 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.018635 plone.portlet.collection-4.0.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.021289 plone.portlet.collection-4.0.2/plone/portlet/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.022804 plone.portlet.collection-4.0.2/plone/portlet/collection/
+-rw-r--r--   0 maurits    (501) staff       (20)      395 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3986 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/collection.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10066 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1141 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.015086 plone.portlet.collection-4.0.2/plone/portlet/collection/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.023435 plone.portlet.collection-4.0.2/plone/portlet/collection/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      187 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      415 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/profiles/default/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1501 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.024640 plone.portlet.collection-4.0.2/plone/portlet/collection/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5876 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/tests/functional.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      947 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/tests/test_functional_doctest.py
+-rw-r--r--   0 maurits    (501) staff       (20)    16311 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/tests/test_portlet_collection.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.020982 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    10339 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1035 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       20 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      327 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1682 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       62 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/requirements-6.0.x.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      224 2023-04-13 23:41:48.025613 plone.portlet.collection-4.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1937 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/setup.py
```

### Comparing `plone.portlet.collection-4.0.1/CHANGES.rst` & `plone.portlet.collection-4.0.2/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.2 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (c79ab88f)
+
+
 4.0.1 (2023-03-21)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.portlet.collection-4.0.1/PKG-INFO` & `plone.portlet.collection-4.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.portlet.collection
-Version: 4.0.1
+Version: 4.0.2
 Summary: A portlet that fetches results from a collection
 Home-page: https://pypi.org/project/plone.portlet.collection/
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: collection portlet
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,14 +34,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.2 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (c79ab88f)
+
+
 4.0.1 (2023-03-21)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.portlet.collection-4.0.1/docs/LICENSE.GPL` & `plone.portlet.collection-4.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.1/docs/LICENSE.txt` & `plone.portlet.collection-4.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.1/plone/portlet/collection/collection.pt` & `plone.portlet.collection-4.0.2/plone/portlet/collection/collection.pt`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.1/plone/portlet/collection/collection.py` & `plone.portlet.collection-4.0.2/plone/portlet/collection/collection.py`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.1/plone/portlet/collection/configure.zcml` & `plone.portlet.collection-4.0.2/plone/portlet/collection/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.1/plone/portlet/collection/testing.py` & `plone.portlet.collection-4.0.2/plone/portlet/collection/testing.py`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.1/plone/portlet/collection/tests/functional.txt` & `plone.portlet.collection-4.0.2/plone/portlet/collection/tests/functional.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,15 @@
     ...         return authenticator.createToken()
     ...     except:  # no plone.protect auto csrf, so no worries
     ...         return ''
 
     >>> from plone.app.testing import login
     >>> login(layer['portal'], 'admin')
     >>> app = layer['app']
-    >>> try:
-    ...     from plone.testing.zope import Browser
-    ... except ImportError:
-    ...     from plone.testing.z2 import Browser
+    >>> from plone.testing.zope import Browser
     >>> browser = Browser(app)
     >>> browser.handleErrors = False
     >>> browser.addHeader('Authorization', 'Basic admin:secret')
     >>> portal = layer['portal']
     >>> portal_url = 'http://nohost/plone'
 
     >>> browser.open(portal_url)
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
 ==================== A functional doctest ==================== Set up
 testbrowser:: >>> def getAuth(): ... try: ... from plone.protect import
 authenticator ... return authenticator.createToken() ... except: # no
 plone.protect auto csrf, so no worries ... return '' >>> from plone.app.testing
 import login >>> login(layer['portal'], 'admin') >>> app = layer['app'] >>>
-try: ... from plone.testing.zope import Browser ... except ImportError: ...
-from plone.testing.z2 import Browser >>> browser = Browser(app) >>>
+from plone.testing.zope import Browser >>> browser = Browser(app) >>>
 browser.handleErrors = False >>> browser.addHeader('Authorization', 'Basic
 admin:secret') >>> portal = layer['portal'] >>> portal_url = 'http://nohost/
 plone' >>> browser.open(portal_url) >>> browser.getLink(url=portal_url + "/
 folder_factories").click() >>> browser.getControl(label="Page").selected = True
 >>> browser.getControl(name="form.button.Add").click() >>> browser.getControl
 (name="form.widgets.IDublinCore.title").value = "Test Document" >>>
 browser.getControl("Save").click() >>> 'Item created' in browser.contents True
```

### Comparing `plone.portlet.collection-4.0.1/plone/portlet/collection/tests/test_functional_doctest.py` & `plone.portlet.collection-4.0.2/plone/portlet/collection/tests/test_functional_doctest.py`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.1/plone/portlet/collection/tests/test_portlet_collection.py` & `plone.portlet.collection-4.0.2/plone/portlet/collection/tests/test_portlet_collection.py`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.1/plone.portlet.collection.egg-info/PKG-INFO` & `plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.portlet.collection
-Version: 4.0.1
+Version: 4.0.2
 Summary: A portlet that fetches results from a collection
 Home-page: https://pypi.org/project/plone.portlet.collection/
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: collection portlet
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,14 +34,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.2 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (c79ab88f)
+
+
 4.0.1 (2023-03-21)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.portlet.collection-4.0.1/plone.portlet.collection.egg-info/SOURCES.txt` & `plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.1/pyproject.toml` & `plone.portlet.collection-4.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.1/setup.py` & `plone.portlet.collection-4.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.1"
+version = "4.0.2"
 
 setup(
     name="plone.portlet.collection",
     version=version,
     description="A portlet that fetches results from a collection",
     long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
     classifiers=[
```

