# Comparing `tmp/imio.migrator-1.8.tar.gz` & `tmp/imio.migrator-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.migrator-1.8.tar", last modified: Thu Oct 18 11:46:15 2018, max compression
+gzip compressed data, was "dist/imio.migrator-1.9.tar", last modified: Thu Jan 17 09:05:18 2019, max compression
```

## Comparing `imio.migrator-1.8.tar` & `imio.migrator-1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-10-18 11:46:15.000000 imio.migrator-1.8/
--rw-rw-r--   0 sge       (1000) sge       (1000)       38 2018-10-18 11:46:15.000000 imio.migrator-1.8/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     3293 2018-10-18 11:46:15.000000 imio.migrator-1.8/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)      279 2018-10-18 11:46:14.000000 imio.migrator-1.8/versions.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)      171 2018-10-18 11:46:14.000000 imio.migrator-1.8/sources.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     1338 2018-10-18 11:46:14.000000 imio.migrator-1.8/setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      479 2018-10-18 11:46:14.000000 imio.migrator-1.8/dev.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)       47 2018-10-18 11:46:14.000000 imio.migrator-1.8/buildout.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     5705 2018-10-18 11:46:14.000000 imio.migrator-1.8/bootstrap.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      585 2018-10-18 11:46:14.000000 imio.migrator-1.8/base.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)      154 2018-10-18 11:46:14.000000 imio.migrator-1.8/README.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      436 2018-10-18 11:46:14.000000 imio.migrator-1.8/Makefile
--rw-rw-r--   0 sge       (1000) sge       (1000)      161 2018-10-18 11:46:14.000000 imio.migrator-1.8/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)       21 2018-10-18 11:46:14.000000 imio.migrator-1.8/CONTRIBUTORS.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)     1981 2018-10-18 11:46:14.000000 imio.migrator-1.8/CHANGES.rst
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-10-18 11:46:15.000000 imio.migrator-1.8/src/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-10-18 11:46:15.000000 imio.migrator-1.8/src/imio.migrator.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)        5 2018-10-18 11:46:15.000000 imio.migrator-1.8/src/imio.migrator.egg-info/top_level.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       43 2018-10-18 11:46:15.000000 imio.migrator-1.8/src/imio.migrator.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2018-10-18 11:46:15.000000 imio.migrator-1.8/src/imio.migrator.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)        5 2018-10-18 11:46:15.000000 imio.migrator-1.8/src/imio.migrator.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       53 2018-10-18 11:46:15.000000 imio.migrator-1.8/src/imio.migrator.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2018-10-18 11:46:15.000000 imio.migrator-1.8/src/imio.migrator.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      686 2018-10-18 11:46:15.000000 imio.migrator-1.8/src/imio.migrator.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)     3293 2018-10-18 11:46:15.000000 imio.migrator-1.8/src/imio.migrator.egg-info/PKG-INFO
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-10-18 11:46:15.000000 imio.migrator-1.8/src/imio/
--rw-rw-r--   0 sge       (1000) sge       (1000)      244 2018-10-18 11:46:14.000000 imio.migrator-1.8/src/imio/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-10-18 11:46:15.000000 imio.migrator-1.8/src/imio/migrator/
--rw-rw-r--   0 sge       (1000) sge       (1000)      167 2018-10-18 11:46:14.000000 imio.migrator-1.8/src/imio/migrator/testing.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)      802 2018-10-18 11:46:14.000000 imio.migrator-1.8/src/imio/migrator/testing.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     9479 2018-10-18 11:46:14.000000 imio.migrator-1.8/src/imio/migrator/migrator.py
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2018-10-18 11:46:14.000000 imio.migrator-1.8/src/imio/migrator/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-10-18 11:46:15.000000 imio.migrator-1.8/src/imio/migrator/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2018-10-18 11:46:14.000000 imio.migrator-1.8/src/imio/migrator/tests/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2018-10-18 11:46:15.000000 imio.migrator-1.8/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)      732 2018-10-18 11:46:14.000000 imio.migrator-1.8/docs/LICENSE.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2018-10-18 11:46:14.000000 imio.migrator-1.8/docs/LICENSE.GPL
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2019-01-17 09:05:18.000000 imio.migrator-1.9/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       38 2019-01-17 09:05:18.000000 imio.migrator-1.9/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3439 2019-01-17 09:05:18.000000 imio.migrator-1.9/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)      279 2019-01-17 09:05:18.000000 imio.migrator-1.9/versions.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)      171 2019-01-17 09:05:18.000000 imio.migrator-1.9/sources.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1338 2019-01-17 09:05:18.000000 imio.migrator-1.9/setup.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      479 2019-01-17 09:05:18.000000 imio.migrator-1.9/dev.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)       47 2019-01-17 09:05:18.000000 imio.migrator-1.9/buildout.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5705 2019-01-17 09:05:18.000000 imio.migrator-1.9/bootstrap.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      585 2019-01-17 09:05:18.000000 imio.migrator-1.9/base.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)      154 2019-01-17 09:05:18.000000 imio.migrator-1.9/README.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      436 2019-01-17 09:05:18.000000 imio.migrator-1.9/Makefile
+-rw-rw-r--   0 sge       (1000) sge       (1000)      161 2019-01-17 09:05:18.000000 imio.migrator-1.9/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)       21 2019-01-17 09:05:18.000000 imio.migrator-1.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2079 2019-01-17 09:05:18.000000 imio.migrator-1.9/CHANGES.rst
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio.migrator.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        5 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio.migrator.egg-info/top_level.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       43 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio.migrator.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio.migrator.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)        5 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio.migrator.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       53 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio.migrator.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio.migrator.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      686 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio.migrator.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3439 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio.migrator.egg-info/PKG-INFO
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      244 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio/migrator/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      167 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio/migrator/testing.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      802 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio/migrator/testing.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     9732 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio/migrator/migrator.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio/migrator/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio/migrator/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2019-01-17 09:05:18.000000 imio.migrator-1.9/src/imio/migrator/tests/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2019-01-17 09:05:18.000000 imio.migrator-1.9/docs/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      732 2019-01-17 09:05:18.000000 imio.migrator-1.9/docs/LICENSE.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2019-01-17 09:05:18.000000 imio.migrator-1.9/docs/LICENSE.GPL
```

### Comparing `imio.migrator-1.8/PKG-INFO` & `imio.migrator-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.migrator
-Version: 1.8
+Version: 1.9
 Summary: Migration helper tool
 Home-page: http://pypi.imio.be/imio/imio/imio.migrator
 Author: IMIO
 Author-email: dev@imio.be
 License: GPL
 Description: ====================
         imio.migrator
@@ -17,14 +17,20 @@
         
         - IMIO, dev@imio.be
         
         
         Changelog
         =========
         
+        1.9 (2019-01-17)
+        ----------------
+        
+        - Improved and simplified upgradeProfile method
+          [sgeulette]
+        
         1.8 (2018-10-18)
         ----------------
         
         - Make REQUEST available thru self.request.
           [gbastien]
         - Added methods `removeUnusedColumns` and `removeUnusedIndexes` to easily remove
           columns or indexes from portal_catalog.
```

### Comparing `imio.migrator-1.8/setup.py` & `imio.migrator-1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     + '\n' +
     open('CHANGES.rst').read()
     + '\n')
 
 
 setup(
     name='imio.migrator',
-    version='1.8',
+    version='1.9',
     description="Migration helper tool",
     long_description=long_description,
     # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
```

### Comparing `imio.migrator-1.8/bootstrap.py` & `imio.migrator-1.9/bootstrap.py`

 * *Files identical despite different names*

### Comparing `imio.migrator-1.8/base.cfg` & `imio.migrator-1.9/base.cfg`

 * *Files identical despite different names*

### Comparing `imio.migrator-1.8/CHANGES.rst` & `imio.migrator-1.9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+1.9 (2019-01-17)
+----------------
+
+- Improved and simplified upgradeProfile method
+  [sgeulette]
+
 1.8 (2018-10-18)
 ----------------
 
 - Make REQUEST available thru self.request.
   [gbastien]
 - Added methods `removeUnusedColumns` and `removeUnusedIndexes` to easily remove
   columns or indexes from portal_catalog.
```

### Comparing `imio.migrator-1.8/src/imio.migrator.egg-info/SOURCES.txt` & `imio.migrator-1.9/src/imio.migrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imio.migrator-1.8/src/imio.migrator.egg-info/PKG-INFO` & `imio.migrator-1.9/src/imio.migrator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.migrator
-Version: 1.8
+Version: 1.9
 Summary: Migration helper tool
 Home-page: http://pypi.imio.be/imio/imio/imio.migrator
 Author: IMIO
 Author-email: dev@imio.be
 License: GPL
 Description: ====================
         imio.migrator
@@ -17,14 +17,20 @@
         
         - IMIO, dev@imio.be
         
         
         Changelog
         =========
         
+        1.9 (2019-01-17)
+        ----------------
+        
+        - Improved and simplified upgradeProfile method
+          [sgeulette]
+        
         1.8 (2018-10-18)
         ----------------
         
         - Make REQUEST available thru self.request.
           [gbastien]
         - Added methods `removeUnusedColumns` and `removeUnusedIndexes` to easily remove
           columns or indexes from portal_catalog.
```

### Comparing `imio.migrator-1.8/src/imio/migrator/testing.py` & `imio.migrator-1.9/src/imio/migrator/testing.py`

 * *Files identical despite different names*

### Comparing `imio.migrator-1.8/src/imio/migrator/migrator.py` & `imio.migrator-1.9/src/imio/migrator/migrator.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # ------------------------------------------------------------------------------
 '''This module, borrowed from Products.PloneMeeting, defines helper methods
    to ease migration process.'''
 
 from imio.helpers.catalog import removeColumns
 from imio.helpers.catalog import removeIndexes
 from Products.CMFPlone.utils import base_hasattr
+from Products.GenericSetup.upgrade import normalize_version
 
 import logging
 import time
 
 
 logger = logging.getLogger('imio.migrator')
 
@@ -141,47 +142,48 @@
             except KeyError:
                 logger.error('Profile %s not found!' % profile)
         logger.info('Done.')
 
     def upgradeProfile(self, profile, olds=[]):
         """ Get upgrade steps and run it. olds can contain a list of dest upgrades to run. """
 
-        def run_upgrade_step(step, source, dest, last_flag):
+        def run_upgrade_step(step, source, dest):
             logger.info('Running upgrade step %s (%s -> %s): %s' % (profile, source, dest, step.title))
             step.doStep(self.ps)
-            self.ps.setLastVersionForProfile(profile, dest)
-            # we update portal_quickinstaller if the current step is the last one
-            if last_flag:
+
+        # if olds, we get all steps.
+        upgrades = self.ps.listUpgrades(profile, show_old=bool(olds))
+        applied_dests = []
+        for container in upgrades:
+            if isinstance(container, dict):
+                if not olds or container['sdest'] in olds:
+                    applied_dests.append((normalize_version(container['sdest']), container['sdest']))
+                    run_upgrade_step(container['step'], container['ssource'], container['sdest'])
+            elif isinstance(container, list):
+                for dic in container:
+                    if not olds or dic['sdest'] in olds:
+                        applied_dests.append((normalize_version(dic['sdest']), dic['sdest']))
+                        run_upgrade_step(dic['step'], dic['ssource'], dic['sdest'])
+        if applied_dests:
+            current_version = normalize_version(self.ps.getLastVersionForProfile(profile))
+            highest_version, dest = sorted(applied_dests)[-1]
+            # check if highest applied version is higher than current version
+            if highest_version > current_version:
+                self.ps.setLastVersionForProfile(profile, dest)
+                # we update portal_quickinstaller version
                 pqi = self.portal.portal_quickinstaller
                 try:
                     product = profile.split(':')[0]
                     prod = pqi.get(product)
                     setattr(prod, 'installedversion', pqi.getProductVersion(product))
                 except IndexError, e:
                     logger.error("Cannot extract product from profile '%s': %s" % (profile, e))
                 except AttributeError, e:
                     logger.error("Cannot get product '%s' from portal_quickinstaller: %s" % (product, e))
 
-        upgrades = self.ps.listUpgrades(profile, show_old=bool(olds))
-        last_i = len(upgrades)-1
-        for i, container in enumerate(upgrades):
-            last_flag = False
-            if isinstance(container, dict):
-                if i == last_i:
-                    last_flag = True
-                if not olds or container['sdest'] in olds:
-                    run_upgrade_step(container['step'], container['ssource'], container['sdest'], last_flag)
-            elif isinstance(container, list):
-                last_j = len(container)-1
-                for j, dic in enumerate(container):
-                    if i == last_i and j == last_j:
-                        last_flag = True
-                    if not olds or dic['sdest'] in olds:
-                        run_upgrade_step(dic['step'], dic['ssource'], dic['sdest'], last_flag)
-
     def upgradeAll(self, omit=[]):
         """ Upgrade all upgrade profiles except those in omit parameter list """
         if self.portal.REQUEST.get('profile_id'):
             omit.append(self.portal.REQUEST.get('profile_id'))
         for profile in self.ps.listProfilesWithUpgrades():
             # make sure the profile isn't the current (or must be avoided) and
             # the profile is well installed
```

### Comparing `imio.migrator-1.8/docs/LICENSE.rst` & `imio.migrator-1.9/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.migrator-1.8/docs/LICENSE.GPL` & `imio.migrator-1.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

