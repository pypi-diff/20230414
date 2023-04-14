# Comparing `tmp/zope.component-5.1.0.tar.gz` & `tmp/zope.component-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.component-5.1.0.tar", last modified: Tue Jan  3 11:27:22 2023, max compression
+gzip compressed data, was "zope.component-6.0.tar", last modified: Fri Apr 14 06:04:42 2023, max compression
```

## Comparing `zope.component-5.1.0.tar` & `zope.component-6.0.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-03 11:27:22.124440 zope.component-5.1.0/
--rw-r--r--   0 jens       (501) staff       (20)    14107 2023-01-03 11:23:33.000000 zope.component-5.1.0/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:53:23.000000 zope.component-5.1.0/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:53:23.000000 zope.component-5.1.0/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      241 2021-11-02 08:53:23.000000 zope.component-5.1.0/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)    17450 2023-01-03 11:27:22.124531 zope.component-5.1.0/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     1524 2021-11-02 08:53:23.000000 zope.component-5.1.0/README.rst
--rw-r--r--   0 jens       (501) staff       (20)      660 2023-01-03 11:24:57.000000 zope.component-5.1.0/buildout.cfg
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-03 11:27:22.117248 zope.component-5.1.0/docs/
--rw-r--r--   0 jens       (501) staff       (20)     5608 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/Makefile
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-03 11:27:22.118438 zope.component-5.1.0/docs/api/
--rw-r--r--   0 jens       (501) staff       (20)    11280 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/api/adapter.rst
--rw-r--r--   0 jens       (501) staff       (20)      403 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/api/factory.rst
--rw-r--r--   0 jens       (501) staff       (20)      299 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/api/hooks.rst
--rw-r--r--   0 jens       (501) staff       (20)     5050 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/api/interface.rst
--rw-r--r--   0 jens       (501) staff       (20)      114 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/api/interfaces.rst
--rw-r--r--   0 jens       (501) staff       (20)      455 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/api/module.rst
--rw-r--r--   0 jens       (501) staff       (20)     6166 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/api/persistent.rst
--rw-r--r--   0 jens       (501) staff       (20)     2607 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/api/security.rst
--rw-r--r--   0 jens       (501) staff       (20)     2337 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/api/sitemanager.rst
--rw-r--r--   0 jens       (501) staff       (20)     7594 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/api/utility.rst
--rw-r--r--   0 jens       (501) staff       (20)      302 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/api.rst
--rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/changelog.rst
--rw-r--r--   0 jens       (501) staff       (20)     9600 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/conf.py
--rw-r--r--   0 jens       (501) staff       (20)     1079 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/configure.rst
--rw-r--r--   0 jens       (501) staff       (20)     4114 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/event.rst
--rw-r--r--   0 jens       (501) staff       (20)     3234 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/factory.rst
--rw-r--r--   0 jens       (501) staff       (20)    10562 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/hacking.rst
--rw-r--r--   0 jens       (501) staff       (20)     3797 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/hooks.rst
--rw-r--r--   0 jens       (501) staff       (20)      350 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/index.rst
--rw-r--r--   0 jens       (501) staff       (20)     5118 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/make.bat
--rw-r--r--   0 jens       (501) staff       (20)    12845 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/narr.rst
--rw-r--r--   0 jens       (501) staff       (20)      424 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/persistentregistry.rst
--rw-r--r--   0 jens       (501) staff       (20)    22265 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/socketexample.rst
--rw-r--r--   0 jens       (501) staff       (20)     4200 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/testlayer.rst
--rw-r--r--   0 jens       (501) staff       (20)    33667 2021-11-02 08:53:23.000000 zope.component-5.1.0/docs/zcml.rst
--rw-r--r--   0 jens       (501) staff       (20)      186 2021-11-02 08:53:23.000000 zope.component-5.1.0/rtd.txt
--rw-r--r--   0 jens       (501) staff       (20)      328 2023-01-03 11:27:22.124828 zope.component-5.1.0/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     4162 2023-01-03 11:23:40.000000 zope.component-5.1.0/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-03 11:27:22.113898 zope.component-5.1.0/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-03 11:27:22.118551 zope.component-5.1.0/src/zope/
--rw-r--r--   0 jens       (501) staff       (20)       56 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-03 11:27:22.121905 zope.component-5.1.0/src/zope/component/
--rw-r--r--   0 jens       (501) staff       (20)     3182 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     8742 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/_api.py
--rw-r--r--   0 jens       (501) staff       (20)     1670 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/_compat.py
--rw-r--r--   0 jens       (501) staff       (20)     2242 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/_declaration.py
--rw-r--r--   0 jens       (501) staff       (20)      444 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/configure.zcml
--rw-r--r--   0 jens       (501) staff       (20)     1233 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/event.py
--rw-r--r--   0 jens       (501) staff       (20)     1955 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/eventtesting.py
--rw-r--r--   0 jens       (501) staff       (20)     1756 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/factory.py
--rw-r--r--   0 jens       (501) staff       (20)     2772 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/globalregistry.py
--rw-r--r--   0 jens       (501) staff       (20)     5422 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/hooks.py
--rw-r--r--   0 jens       (501) staff       (20)     3923 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/interface.py
--rw-r--r--   0 jens       (501) staff       (20)    14169 2023-01-03 11:20:30.000000 zope.component-5.1.0/src/zope/component/interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)     1151 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/meta.zcml
--rw-r--r--   0 jens       (501) staff       (20)     5349 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/persistentregistry.py
--rw-r--r--   0 jens       (501) staff       (20)     1692 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/registry.py
--rw-r--r--   0 jens       (501) staff       (20)     4196 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/security.py
--rw-r--r--   0 jens       (501) staff       (20)     1153 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/standalonetests.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-03 11:27:22.122536 zope.component-5.1.0/src/zope/component/testfiles/
--rw-r--r--   0 jens       (501) staff       (20)       16 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/testfiles/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     1469 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/testfiles/adapter.py
--rw-r--r--   0 jens       (501) staff       (20)     1574 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/testfiles/components.py
--rw-r--r--   0 jens       (501) staff       (20)      306 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/testfiles/testlayer.zcml
--rw-r--r--   0 jens       (501) staff       (20)      730 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/testfiles/views.py
--rw-r--r--   0 jens       (501) staff       (20)     1244 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/testing.py
--rw-r--r--   0 jens       (501) staff       (20)     4195 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/testlayer.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-03 11:27:22.124310 zope.component-5.1.0/src/zope/component/tests/
--rw-r--r--   0 jens       (501) staff       (20)      877 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     3108 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/examples.py
--rw-r--r--   0 jens       (501) staff       (20)     3045 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/test___init__.py
--rw-r--r--   0 jens       (501) staff       (20)    41363 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/test__api.py
--rw-r--r--   0 jens       (501) staff       (20)     6364 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/test__declaration.py
--rw-r--r--   0 jens       (501) staff       (20)     2203 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/test_event.py
--rw-r--r--   0 jens       (501) staff       (20)     3790 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/test_factory.py
--rw-r--r--   0 jens       (501) staff       (20)     9579 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/test_globalregistry.py
--rw-r--r--   0 jens       (501) staff       (20)    11605 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/test_hooks.py
--rw-r--r--   0 jens       (501) staff       (20)    16097 2023-01-03 11:20:30.000000 zope.component-5.1.0/src/zope/component/tests/test_interface.py
--rw-r--r--   0 jens       (501) staff       (20)     1001 2023-01-02 19:07:50.000000 zope.component-5.1.0/src/zope/component/tests/test_interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)     9413 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/test_persistentregistry.py
--rw-r--r--   0 jens       (501) staff       (20)     4295 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/test_registry.py
--rw-r--r--   0 jens       (501) staff       (20)     9247 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/test_security.py
--rw-r--r--   0 jens       (501) staff       (20)     2179 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/test_standalone.py
--rw-r--r--   0 jens       (501) staff       (20)    53506 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/tests/test_zcml.py
--rw-r--r--   0 jens       (501) staff       (20)    20742 2021-11-02 08:53:23.000000 zope.component-5.1.0/src/zope/component/zcml.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-01-03 11:27:22.119399 zope.component-5.1.0/src/zope.component.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)    17450 2023-01-03 11:27:22.000000 zope.component-5.1.0/src/zope.component.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     2436 2023-01-03 11:27:22.000000 zope.component-5.1.0/src/zope.component.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2023-01-03 11:27:22.000000 zope.component-5.1.0/src/zope.component.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)        5 2023-01-03 11:27:22.000000 zope.component-5.1.0/src/zope.component.egg-info/namespace_packages.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2023-01-02 16:57:36.000000 zope.component-5.1.0/src/zope.component.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)      457 2023-01-03 11:27:22.000000 zope.component-5.1.0/src/zope.component.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)        5 2023-01-03 11:27:22.000000 zope.component-5.1.0/src/zope.component.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)     1757 2023-01-03 11:22:05.000000 zope.component-5.1.0/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:04:42.169971 zope.component-6.0/
+-rw-r--r--   0 mac        (513) staff       (20)    14185 2023-04-14 06:04:41.000000 zope.component-6.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-04-14 06:04:41.000000 zope.component-6.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-04-14 06:04:41.000000 zope.component-6.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-04-14 06:04:41.000000 zope.component-6.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      373 2023-04-14 06:04:41.000000 zope.component-6.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)    17323 2023-04-14 06:04:42.170116 zope.component-6.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1524 2023-04-14 06:04:41.000000 zope.component-6.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      660 2023-04-14 06:04:41.000000 zope.component-6.0/buildout.cfg
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:04:42.146810 zope.component-6.0/docs/
+-rw-r--r--   0 mac        (513) staff       (20)     5608 2023-04-14 06:04:41.000000 zope.component-6.0/docs/Makefile
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:04:42.151448 zope.component-6.0/docs/api/
+-rw-r--r--   0 mac        (513) staff       (20)    11280 2023-04-14 06:04:41.000000 zope.component-6.0/docs/api/adapter.rst
+-rw-r--r--   0 mac        (513) staff       (20)      403 2023-04-14 06:04:41.000000 zope.component-6.0/docs/api/factory.rst
+-rw-r--r--   0 mac        (513) staff       (20)      299 2023-04-14 06:04:41.000000 zope.component-6.0/docs/api/hooks.rst
+-rw-r--r--   0 mac        (513) staff       (20)     5050 2023-04-14 06:04:41.000000 zope.component-6.0/docs/api/interface.rst
+-rw-r--r--   0 mac        (513) staff       (20)      114 2023-04-14 06:04:41.000000 zope.component-6.0/docs/api/interfaces.rst
+-rw-r--r--   0 mac        (513) staff       (20)      455 2023-04-14 06:04:41.000000 zope.component-6.0/docs/api/module.rst
+-rw-r--r--   0 mac        (513) staff       (20)     6166 2023-04-14 06:04:41.000000 zope.component-6.0/docs/api/persistent.rst
+-rw-r--r--   0 mac        (513) staff       (20)     2607 2023-04-14 06:04:41.000000 zope.component-6.0/docs/api/security.rst
+-rw-r--r--   0 mac        (513) staff       (20)     2337 2023-04-14 06:04:41.000000 zope.component-6.0/docs/api/sitemanager.rst
+-rw-r--r--   0 mac        (513) staff       (20)     7594 2023-04-14 06:04:41.000000 zope.component-6.0/docs/api/utility.rst
+-rw-r--r--   0 mac        (513) staff       (20)      302 2023-04-14 06:04:41.000000 zope.component-6.0/docs/api.rst
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-04-14 06:04:41.000000 zope.component-6.0/docs/changelog.rst
+-rw-r--r--   0 mac        (513) staff       (20)     9600 2023-04-14 06:04:41.000000 zope.component-6.0/docs/conf.py
+-rw-r--r--   0 mac        (513) staff       (20)     1079 2023-04-14 06:04:41.000000 zope.component-6.0/docs/configure.rst
+-rw-r--r--   0 mac        (513) staff       (20)     4114 2023-04-14 06:04:41.000000 zope.component-6.0/docs/event.rst
+-rw-r--r--   0 mac        (513) staff       (20)     3234 2023-04-14 06:04:41.000000 zope.component-6.0/docs/factory.rst
+-rw-r--r--   0 mac        (513) staff       (20)    10562 2023-04-14 06:04:41.000000 zope.component-6.0/docs/hacking.rst
+-rw-r--r--   0 mac        (513) staff       (20)     3797 2023-04-14 06:04:41.000000 zope.component-6.0/docs/hooks.rst
+-rw-r--r--   0 mac        (513) staff       (20)      350 2023-04-14 06:04:41.000000 zope.component-6.0/docs/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)     5118 2023-04-14 06:04:41.000000 zope.component-6.0/docs/make.bat
+-rw-r--r--   0 mac        (513) staff       (20)    12845 2023-04-14 06:04:41.000000 zope.component-6.0/docs/narr.rst
+-rw-r--r--   0 mac        (513) staff       (20)      424 2023-04-14 06:04:41.000000 zope.component-6.0/docs/persistentregistry.rst
+-rw-r--r--   0 mac        (513) staff       (20)    22265 2023-04-14 06:04:41.000000 zope.component-6.0/docs/socketexample.rst
+-rw-r--r--   0 mac        (513) staff       (20)     4200 2023-04-14 06:04:41.000000 zope.component-6.0/docs/testlayer.rst
+-rw-r--r--   0 mac        (513) staff       (20)    33667 2023-04-14 06:04:41.000000 zope.component-6.0/docs/zcml.rst
+-rw-r--r--   0 mac        (513) staff       (20)      186 2023-04-14 06:04:41.000000 zope.component-6.0/rtd.txt
+-rw-r--r--   0 mac        (513) staff       (20)      561 2023-04-14 06:04:42.170732 zope.component-6.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     3949 2023-04-14 06:04:41.000000 zope.component-6.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:04:42.133971 zope.component-6.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:04:42.151746 zope.component-6.0/src/zope/
+-rw-r--r--   0 mac        (513) staff       (20)       56 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:04:42.162912 zope.component-6.0/src/zope/component/
+-rw-r--r--   0 mac        (513) staff       (20)     3175 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     8767 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/_api.py
+-rw-r--r--   0 mac        (513) staff       (20)      793 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/_compat.py
+-rw-r--r--   0 mac        (513) staff       (20)     2180 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/_declaration.py
+-rw-r--r--   0 mac        (513) staff       (20)      444 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/configure.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     1234 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/event.py
+-rw-r--r--   0 mac        (513) staff       (20)     1963 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/eventtesting.py
+-rw-r--r--   0 mac        (513) staff       (20)     1742 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/factory.py
+-rw-r--r--   0 mac        (513) staff       (20)     2754 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/globalregistry.py
+-rw-r--r--   0 mac        (513) staff       (20)     5429 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/hooks.py
+-rw-r--r--   0 mac        (513) staff       (20)     3881 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/interface.py
+-rw-r--r--   0 mac        (513) staff       (20)    14213 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)     1151 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/meta.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     5291 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/persistentregistry.py
+-rw-r--r--   0 mac        (513) staff       (20)     1696 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/registry.py
+-rw-r--r--   0 mac        (513) staff       (20)     4204 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/security.py
+-rw-r--r--   0 mac        (513) staff       (20)     1057 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/standalonetests.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:04:42.164432 zope.component-6.0/src/zope/component/testfiles/
+-rw-r--r--   0 mac        (513) staff       (20)       17 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/testfiles/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     1559 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/testfiles/adapter.py
+-rw-r--r--   0 mac        (513) staff       (20)     1595 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/testfiles/components.py
+-rw-r--r--   0 mac        (513) staff       (20)      306 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/testfiles/testlayer.zcml
+-rw-r--r--   0 mac        (513) staff       (20)      731 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/testfiles/views.py
+-rw-r--r--   0 mac        (513) staff       (20)     1275 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/testing.py
+-rw-r--r--   0 mac        (513) staff       (20)     4225 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/testlayer.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:04:42.169658 zope.component-6.0/src/zope/component/tests/
+-rw-r--r--   0 mac        (513) staff       (20)      914 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     3086 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/examples.py
+-rw-r--r--   0 mac        (513) staff       (20)     3072 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test___init__.py
+-rw-r--r--   0 mac        (513) staff       (20)    41575 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test__api.py
+-rw-r--r--   0 mac        (513) staff       (20)     6281 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test__declaration.py
+-rw-r--r--   0 mac        (513) staff       (20)     2204 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test_event.py
+-rw-r--r--   0 mac        (513) staff       (20)     3800 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test_factory.py
+-rw-r--r--   0 mac        (513) staff       (20)     9679 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test_globalregistry.py
+-rw-r--r--   0 mac        (513) staff       (20)    10988 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test_hooks.py
+-rw-r--r--   0 mac        (513) staff       (20)    16400 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test_interface.py
+-rw-r--r--   0 mac        (513) staff       (20)     1002 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test_interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)     9457 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test_persistentregistry.py
+-rw-r--r--   0 mac        (513) staff       (20)     4416 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test_registry.py
+-rw-r--r--   0 mac        (513) staff       (20)     9172 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test_security.py
+-rw-r--r--   0 mac        (513) staff       (20)     2192 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test_standalone.py
+-rw-r--r--   0 mac        (513) staff       (20)    53369 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/tests/test_zcml.py
+-rw-r--r--   0 mac        (513) staff       (20)    20496 2023-04-14 06:04:41.000000 zope.component-6.0/src/zope/component/zcml.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-14 06:04:42.154597 zope.component-6.0/src/zope.component.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)    17323 2023-04-14 06:04:42.000000 zope.component-6.0/src/zope.component.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     2452 2023-04-14 06:04:42.000000 zope.component-6.0/src/zope.component.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-14 06:04:42.000000 zope.component-6.0/src/zope.component.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-14 06:04:42.000000 zope.component-6.0/src/zope.component.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-14 06:04:42.000000 zope.component-6.0/src/zope.component.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      453 2023-04-14 06:04:42.000000 zope.component-6.0/src/zope.component.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-14 06:04:42.000000 zope.component-6.0/src/zope.component.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2053 2023-04-14 06:04:41.000000 zope.component-6.0/tox.ini
```

### Comparing `zope.component-5.1.0/CHANGES.rst` & `zope.component-6.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
  Changes
 =========
 
+6.0 (2023-04-14)
+================
+
+
+
+- Drop support for Python 2.7, 3.5, 3.6.
 
 5.1.0 (2023-01-03)
 ==================
 
 - Fix crash when the environment variable `PYTHONOPTIMIZED` is set to `2`
   and docstrings are set to `None` by the interpreter.
   (`#67 <https://github.com/zopefoundation/zope.component/issues/67>`_)
```

### Comparing `zope.component-5.1.0/LICENSE.txt` & `zope.component-6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/PKG-INFO` & `zope.component-6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 Metadata-Version: 2.1
 Name: zope.component
-Version: 5.1.0
+Version: 6.0
 Summary: Zope Component Architecture
 Home-page: https://github.com/zopefoundation/zope.component
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Documentation, https://zopecomponent.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.component/issues
 Project-URL: Sources, https://github.com/zopefoundation/zope.component
 Keywords: interface component coupling loose utility adapter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: Zope :: 3
+Classifier: Framework :: Zope :: 5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: hook
 Provides-Extra: persistentregistry
 Provides-Extra: security
 Provides-Extra: zcml
 Provides-Extra: mintests
 Provides-Extra: test
 Provides-Extra: docs
@@ -79,14 +76,20 @@
 
 .. _zope.interface: https://github.com/zopefoundation/zope.interface
 
 =========
  Changes
 =========
 
+6.0 (2023-04-14)
+================
+
+
+
+- Drop support for Python 2.7, 3.5, 3.6.
 
 5.1.0 (2023-01-03)
 ==================
 
 - Fix crash when the environment variable `PYTHONOPTIMIZED` is set to `2`
   and docstrings are set to `None` by the interpreter.
   (`#67 <https://github.com/zopefoundation/zope.component/issues/67>`_)
```

### Comparing `zope.component-5.1.0/README.rst` & `zope.component-6.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/buildout.cfg` & `zope.component-6.0/buildout.cfg`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/Makefile` & `zope.component-6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/api/adapter.rst` & `zope.component-6.0/docs/api/adapter.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/api/interface.rst` & `zope.component-6.0/docs/api/interface.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/api/persistent.rst` & `zope.component-6.0/docs/api/persistent.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/api/security.rst` & `zope.component-6.0/docs/api/security.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/api/sitemanager.rst` & `zope.component-6.0/docs/api/sitemanager.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/api/utility.rst` & `zope.component-6.0/docs/api/utility.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/conf.py` & `zope.component-6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/configure.rst` & `zope.component-6.0/docs/configure.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/event.rst` & `zope.component-6.0/docs/event.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/factory.rst` & `zope.component-6.0/docs/factory.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/hacking.rst` & `zope.component-6.0/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/hooks.rst` & `zope.component-6.0/docs/hooks.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/make.bat` & `zope.component-6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/narr.rst` & `zope.component-6.0/docs/narr.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/socketexample.rst` & `zope.component-6.0/docs/socketexample.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/testlayer.rst` & `zope.component-6.0/docs/testlayer.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/docs/zcml.rst` & `zope.component-6.0/docs/zcml.rst`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/setup.py` & `zope.component-6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.component package
 """
 
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
+
 
 HOOK_REQUIRES = [
 ]
 
 PERSISTENTREGISTRY_REQUIRES = [
     'persistent',
 ]
@@ -56,28 +59,29 @@
 )
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
+
 setup(
     name='zope.component',
-    version='5.1.0',
+    version='6.0',
     url='https://github.com/zopefoundation/zope.component',
     project_urls={
         'Documentation': 'https://zopecomponent.readthedocs.io/',
         'Issue Tracker': ('https://github.com/zopefoundation/'
                           'zope.component/issues'),
         'Sources': 'https://github.com/zopefoundation/zope.component',
     },
     license='ZPL 2.1',
     description='Zope Component Architecture',
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     long_description=(
         read('README.rst')
         + '\n' +
         read('CHANGES.rst')
     ),
     keywords="interface component coupling loose utility adapter",
     packages=find_packages('src'),
@@ -85,37 +89,33 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved",
         "License :: OSI Approved :: Zope Public License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Framework :: Zope :: 3",
+        "Framework :: Zope :: 5",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    namespace_packages=['zope',],
-    python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*',
-    tests_require=TESTS_REQUIRE,
+    namespace_packages=['zope', ],
+    python_requires='>=3.7',
     install_requires=[
         'setuptools',
         'zope.event',
         'zope.hookable >= 4.2.0',
-        'zope.interface >= 5.3.0a1',
+        'zope.interface >= 5.3',
     ],
     include_package_data=True,
     zip_safe=False,
     extras_require={
         'hook': HOOK_REQUIRES,  # BBB
         'persistentregistry': PERSISTENTREGISTRY_REQUIRES,
         'security': SECURITY_REQUIRES,
```

### Comparing `zope.component-5.1.0/src/zope/component/__init__.py` & `zope.component-6.0/src/zope/component/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,53 +23,48 @@
 using the `global site manager <getGlobalSiteManager>`_.
 """
 from zope.interface import Interface
 from zope.interface import implementedBy
 from zope.interface import moduleProvides
 from zope.interface import named
 from zope.interface import providedBy
-
 from zope.interface.interfaces import ComponentLookupError
-from zope.component.interfaces import IComponentArchitecture
 from zope.interface.interfaces import IComponentLookup
-from zope.component.interfaces import IComponentRegistrationConvenience
-from zope.component.interfaces import IFactory
-
-from zope.component.globalregistry import getGlobalSiteManager
-from zope.component.globalregistry import globalSiteManager
-from zope.component.globalregistry import provideAdapter
-from zope.component.globalregistry import provideHandler
-from zope.component.globalregistry import provideSubscriptionAdapter
-from zope.component.globalregistry import provideUtility
 
 from zope.component._api import adapter_hook
 from zope.component._api import createObject
 from zope.component._api import getAdapter
 from zope.component._api import getAdapterInContext
 from zope.component._api import getAdapters
 from zope.component._api import getAllUtilitiesRegisteredFor
 from zope.component._api import getFactoriesFor
 from zope.component._api import getFactoryInterfaces
 from zope.component._api import getMultiAdapter
+from zope.component._api import getNextUtility
 from zope.component._api import getSiteManager
 from zope.component._api import getUtilitiesFor
 from zope.component._api import getUtility
-from zope.component._api import getNextUtility
 from zope.component._api import handle
 from zope.component._api import queryAdapter
 from zope.component._api import queryAdapterInContext
 from zope.component._api import queryMultiAdapter
-from zope.component._api import queryUtility
 from zope.component._api import queryNextUtility
+from zope.component._api import queryUtility
 from zope.component._api import subscribers
-
 from zope.component._declaration import adaptedBy
 from zope.component._declaration import adapter
 from zope.component._declaration import adapts
+from zope.component.globalregistry import getGlobalSiteManager
+from zope.component.globalregistry import globalSiteManager
+from zope.component.globalregistry import provideAdapter
+from zope.component.globalregistry import provideHandler
+from zope.component.globalregistry import provideSubscriptionAdapter
+from zope.component.globalregistry import provideUtility
+from zope.component.interfaces import IComponentArchitecture
+from zope.component.interfaces import IComponentRegistrationConvenience
+from zope.component.interfaces import IFactory
+
 
 moduleProvides(IComponentArchitecture, IComponentRegistrationConvenience)
-__all__ = tuple(IComponentArchitecture) + tuple(IComponentRegistrationConvenience) + (
-    'named',
-    'adapts',
-    'adapter',
-    'adaptedBy',
-)
+__all__ = tuple(IComponentArchitecture) \
+    + tuple(IComponentRegistrationConvenience) \
+    + ('named', 'adapts', 'adapter', 'adaptedBy', )
```

### Comparing `zope.component-5.1.0/src/zope/component/_api.py` & `zope.component-6.0/src/zope/component/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,30 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Zope 3 Component Architecture
 """
 import sys
 
+import zope.interface.interface
 from zope.hookable import hookable
 from zope.interface import Interface
 from zope.interface.interfaces import ComponentLookupError
 from zope.interface.interfaces import IComponentLookup
 
 from zope.component.interfaces import IFactory
 from zope.component.interfaces import inherits_arch_docs as inherits_docs
 
 
 # getSiteManager() returns a component registry.  Although the term
 # "site manager" is deprecated in favor of "component registry",
 # the old term is kept around to maintain a stable API.
 base = None
+
+
 @hookable
 @inherits_docs
 def getSiteManager(context=None):
     """ See IComponentArchitecture.
     """
     global base
     if context is None:
@@ -43,21 +46,24 @@
         # to avoid the recursion implied by using a local `getAdapter()` call.
         try:
             return IComponentLookup(context)
         except TypeError as error:
             raise ComponentLookupError(*error.args)
 
 # Adapter API
+
+
 @inherits_docs
 def getAdapterInContext(object, interface, context):
     adapter = queryAdapterInContext(object, interface, context)
     if adapter is None:
         raise ComponentLookupError(object, interface)
     return adapter
 
+
 @inherits_docs
 def queryAdapterInContext(object, interface, context, default=None):
     conform = getattr(object, '__conform__', None)
     if conform is not None:
         try:
             adapter = conform(interface)
         except TypeError:
@@ -78,111 +84,124 @@
                 return adapter
 
     if interface.providedBy(object):
         return object
 
     return getSiteManager(context).queryAdapter(object, interface, '', default)
 
+
 @inherits_docs
-def getAdapter(object, interface=Interface, name=u'', context=None):
+def getAdapter(object, interface=Interface, name='', context=None):
     adapter = queryAdapter(object, interface, name, None, context)
     if adapter is None:
         raise ComponentLookupError(object, interface, name)
     return adapter
 
+
 @inherits_docs
-def queryAdapter(object, interface=Interface, name=u'', default=None,
+def queryAdapter(object, interface=Interface, name='', default=None,
                  context=None):
     if context is None:
         return adapter_hook(interface, object, name, default)
     return getSiteManager(context).queryAdapter(object, interface, name,
                                                 default)
 
+
 @inherits_docs
-def getMultiAdapter(objects, interface=Interface, name=u'', context=None):
+def getMultiAdapter(objects, interface=Interface, name='', context=None):
     adapter = queryMultiAdapter(objects, interface, name, context=context)
     if adapter is None:
         raise ComponentLookupError(objects, interface, name)
     return adapter
 
+
 @inherits_docs
-def queryMultiAdapter(objects, interface=Interface, name=u'', default=None,
+def queryMultiAdapter(objects, interface=Interface, name='', default=None,
                       context=None):
     try:
         sitemanager = getSiteManager(context)
     except ComponentLookupError:
         # Oh blast, no site manager. This should *never* happen!
         return default
 
     return sitemanager.queryMultiAdapter(objects, interface, name, default)
 
+
 @inherits_docs
 def getAdapters(objects, provided, context=None):
     try:
         sitemanager = getSiteManager(context)
     except ComponentLookupError:
         # Oh blast, no site manager. This should *never* happen!
         return []
     return sitemanager.getAdapters(objects, provided)
 
+
 @inherits_docs
 def subscribers(objects, interface, context=None):
     try:
         sitemanager = getSiteManager(context)
     except ComponentLookupError:
         # Oh blast, no site manager. This should *never* happen!
         return []
     return sitemanager.subscribers(objects, interface)
 
+
 @inherits_docs
 def handle(*objects):
     getSiteManager(None).subscribers(objects, None)
 
 #############################################################################
 # Register the component architectures adapter hook, with the adapter hook
 # registry of the `zope.inteface` package. This way we will be able to call
 # interfaces to create adapters for objects. For example, `I1(ob)` is
 # equvalent to `getAdapterInContext(I1, ob, '')`.
+
+
 @hookable
 def adapter_hook(interface, object, name='', default=None):
     try:
         sitemanager = getSiteManager()
-    except ComponentLookupError: #pragma NO COVER w/o context, cannot test
+    except ComponentLookupError:  # pragma: no cover w/o context, cannot test
         # Oh blast, no site manager. This should *never* happen!
         return None
     return sitemanager.queryAdapter(object, interface, name, default)
 
-import zope.interface.interface
+
 zope.interface.interface.adapter_hooks.append(adapter_hook)
 #############################################################################
 
 
 # Utility API
 @inherits_docs
 def getUtility(interface, name='', context=None):
     utility = queryUtility(interface, name, context=context)
     if utility is not None:
         return utility
     raise ComponentLookupError(interface, name)
 
+
 @inherits_docs
 def queryUtility(interface, name='', default=None, context=None):
     return getSiteManager(context).queryUtility(interface, name, default)
 
+
 @inherits_docs
 def getUtilitiesFor(interface, context=None):
     return getSiteManager(context).getUtilitiesFor(interface)
 
+
 @inherits_docs
 def getAllUtilitiesRegisteredFor(interface, context=None):
     return getSiteManager(context).getAllUtilitiesRegisteredFor(interface)
 
 
 _marker = object()
 
+
 @inherits_docs
 def queryNextUtility(context, interface, name='', default=None):
     """Query for the next available utility.
 
     Find the next available utility providing `interface` and having the
     specified name. If no utility was found, return the specified `default`
     value.
@@ -194,24 +213,25 @@
     bases = sm.__bases__
     for base in bases:
         util = base.queryUtility(interface, name, _marker)
         if util is not _marker:
             return util
     return default
 
+
 @inherits_docs
 def getNextUtility(context, interface, name=''):
     """Get the next available utility.
 
     If no utility was found, a `ComponentLookupError` is raised.
     """
     util = queryNextUtility(context, interface, name, _marker)
     if util is _marker:
         raise ComponentLookupError(
-            "No more utilities for %s, '%s' have been found." % (
+            "No more utilities for {}, '{}' have been found.".format(
                 interface, name))
     return util
 
 
 # Factories
 
 @inherits_docs
@@ -219,22 +239,24 @@
     """Invoke the named factory and return the result.
 
     ``__factory_name`` is a positional-only argument.
     """
     context = kwargs.pop('context', None)
     return getUtility(IFactory, __factory_name, context)(*args, **kwargs)
 
+
 @inherits_docs
 def getFactoryInterfaces(name, context=None):
     """Return the interface provided by the named factory's objects
 
     Result might be a single interface. XXX
     """
     return getUtility(IFactory, name, context).getInterfaces()
 
+
 @inherits_docs
 def getFactoriesFor(interface, context=None):
     """Return info on all factories implementing the given interface.
     """
     utils = getSiteManager(context)
     for (name, factory) in utils.getUtilitiesFor(IFactory):
         interfaces = factory.getInterfaces()
```

### Comparing `zope.component-5.1.0/src/zope/component/_declaration.py` & `zope.component-6.0/src/zope/component/_declaration.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,58 +11,63 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Adapter declarations
 """
 import sys
 
-from zope.component._compat import CLASS_TYPES
 
-class adapter(object):
+class adapter:
     """
     Decorator that declares that the decorated object adapts the given
     *interfaces*.
 
     This is commonly used in conjunction with :obj:`zope.interface.implementer`
     to declare what adapting the *interfaces* will provide.
     """
+
     def __init__(self, *interfaces):
         self.interfaces = interfaces
 
     def __call__(self, ob):
-        if isinstance(ob, CLASS_TYPES):
+        if isinstance(ob, type):
             ob.__component_adapts__ = _adapts_descr(self.interfaces)
         else:
             ob.__component_adapts__ = self.interfaces
 
         return ob
 
+
 def adapts(*interfaces):
     frame = sys._getframe(1)
     locals = frame.f_locals
 
     # Ensure we were called from a class def.
     if locals is frame.f_globals or '__module__' not in locals:
         raise TypeError("adapts can be used only from a class definition.")
 
     if '__component_adapts__' in locals:
         raise TypeError("adapts can be used only once in a class definition.")
 
     locals['__component_adapts__'] = _adapts_descr(interfaces)
 
+
 def adaptedBy(ob):
     """
-    Return the *interfaces* that *ob* will adapt, as declared by :obj:`adapter`.
+    Return the *interfaces* that *ob* will adapt, as declared by
+    :obj:`adapter`.
     """
     return getattr(ob, '__component_adapts__', None)
 
+
 def getName(ob):
-    return getattr(ob, '__component_name__', u'')
+    return getattr(ob, '__component_name__', '')
+
 
-class _adapts_descr(object):
+class _adapts_descr:
     def __init__(self, interfaces):
         self.interfaces = interfaces
 
     def __get__(self, inst, cls):
         if inst is None:
             return self.interfaces
         raise AttributeError('__component_adapts__')
```

### Comparing `zope.component-5.1.0/src/zope/component/event.py` & `zope.component-6.0/src/zope/component/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 ##############################################################################
 """Component Architecture-specific event dispatching
 
 Based on subscription adapters / handlers.
 """
 
 from zope.event import subscribers as event_subscribers
-
 from zope.interface.interfaces import IObjectEvent
+
 from zope.component._api import subscribers as component_subscribers
 from zope.component._declaration import adapter
 
 
 def dispatch(*event):
     component_subscribers(event, None)
 
+
 event_subscribers.append(dispatch)
 
 
 @adapter(IObjectEvent)
 def objectEventNotify(event):
     """Dispatch ObjectEvents to interested adapters.
     """
```

### Comparing `zope.component-5.1.0/src/zope/component/eventtesting.py` & `zope.component-6.0/src/zope/component/eventtesting.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,46 +12,55 @@
 #
 ##############################################################################
 """Placeless Test Setup
 """
 
 from zope.component import provideHandler
 from zope.component.event import objectEventNotify
-from zope.component.registry import dispatchUtilityRegistrationEvent
 from zope.component.registry import dispatchAdapterRegistrationEvent
-from zope.component.registry import (
-    dispatchSubscriptionAdapterRegistrationEvent)
 from zope.component.registry import dispatchHandlerRegistrationEvent
+from zope.component.registry import \
+    dispatchSubscriptionAdapterRegistrationEvent
+from zope.component.registry import dispatchUtilityRegistrationEvent
+
+
 try:
     from zope.testing.cleanup import addCleanUp
 except ImportError:
     def addCleanUp(x):
         pass
 
 events = []
+
+
 def getEvents(event_type=None, filter=None):
     r = []
     for event in events:
         if event_type is not None and not event_type.providedBy(event):
             continue
         if filter is not None and not filter(event):
             continue
         r.append(event)
 
     return r
 
+
 def clearEvents():
     del events[:]
+
+
 addCleanUp(clearEvents)
 
+
 class PlacelessSetup:
 
     def setUp(self):
         provideHandler(objectEventNotify)
         provideHandler(dispatchUtilityRegistrationEvent)
         provideHandler(dispatchAdapterRegistrationEvent)
         provideHandler(dispatchSubscriptionAdapterRegistrationEvent)
         provideHandler(dispatchHandlerRegistrationEvent)
         provideHandler(events.append, (None,))
 
+
 def setUp(test=None):
     PlacelessSetup().setUp()
```

### Comparing `zope.component-5.1.0/src/zope/component/factory.py` & `zope.component-6.0/src/zope/component/factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Factory object
 """
-from zope.interface import implementer
 from zope.interface import implementedBy
+from zope.interface import implementer
 from zope.interface.declarations import Implements
+
 from zope.component.interfaces import IFactory
 
 
 @implementer(IFactory)
-class Factory(object):
+class Factory:
     """Generic factory implementation.
 
     The purpose of this implementation is to provide a quick way of creating
     factories for classes, functions and other objects.
     """
 
     def __init__(self, callable, title='', description='', interfaces=None):
@@ -39,9 +40,9 @@
     def getInterfaces(self):
         if self._interfaces is not None:
             spec = Implements(*self._interfaces)
             spec.__name__ = getattr(self._callable, '__name__', '[callable]')
             return spec
         return implementedBy(self._callable)
 
-    def __repr__(self): #pragma NO COVER
-        return '<%s for %s>' % (self.__class__.__name__, repr(self._callable))
+    def __repr__(self):  # pragma: no cover
+        return f'<{self.__class__.__name__} for {self._callable!r}>'
```

### Comparing `zope.component-5.1.0/src/zope/component/globalregistry.py` & `zope.component-6.0/src/zope/component/globalregistry.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,24 +19,25 @@
 from zope.component.interfaces import inherits_arch_docs
 from zope.component.interfaces import inherits_reg_docs
 
 
 def GAR(components, registryName):
     return getattr(components, registryName)
 
+
 class GlobalAdapterRegistry(AdapterRegistry):
     """A global adapter registry
 
     This adapter registry's main purpose is to be picklable in combination
     with a site manager."""
 
     def __init__(self, parent, name):
         self.__parent__ = parent
         self.__name__ = name
-        super(GlobalAdapterRegistry, self).__init__()
+        super().__init__()
 
     def __reduce__(self):
         return GAR, (self.__parent__, self.__name__)
 
 
 class BaseGlobalComponents(Components):
 
@@ -44,41 +45,48 @@
         self.adapters = GlobalAdapterRegistry(self, 'adapters')
         self.utilities = GlobalAdapterRegistry(self, 'utilities')
 
     def __reduce__(self):
         # Global site managers are pickled as global objects
         return self.__name__
 
+
 base = BaseGlobalComponents('base')
 
 try:
     from zope.testing.cleanup import addCleanUp
-except ImportError: #pragma NO COVER
+except ImportError:  # pragma: no cover
     pass
 else:
     addCleanUp(lambda: base.__init__('base'))
     del addCleanUp
 
 globalSiteManager = base
+
+
 @inherits_arch_docs
 def getGlobalSiteManager():
     return globalSiteManager
 
 # The following APIs provide global registration support for Python code.
 # We eventually want to deprecate these in favor of using the global
 # component registry directly.
 
+
 @inherits_reg_docs
-def provideUtility(component, provides=None, name=u''):
+def provideUtility(component, provides=None, name=''):
     base.registerUtility(component, provides, name, event=False)
 
+
 @inherits_reg_docs
-def provideAdapter(factory, adapts=None, provides=None, name=u''):
+def provideAdapter(factory, adapts=None, provides=None, name=''):
     base.registerAdapter(factory, adapts, provides, name, event=False)
 
+
 @inherits_reg_docs
 def provideSubscriptionAdapter(factory, adapts=None, provides=None):
     base.registerSubscriptionAdapter(factory, adapts, provides, event=False)
 
+
 @inherits_reg_docs
 def provideHandler(factory, adapts=None):
     base.registerHandler(factory, adapts, event=False)
```

### Comparing `zope.component-5.1.0/src/zope/component/hooks.py` & `zope.component-6.0/src/zope/component/hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,60 +16,68 @@
 __docformat__ = 'restructuredtext'
 
 import contextlib
 import threading
 
 from zope.component._compat import ZOPE_SECURITY_NOT_AVAILABLE_EX
 
+
 try:
     from zope.security.proxy import removeSecurityProxy
-except ZOPE_SECURITY_NOT_AVAILABLE_EX: # pragma: no cover
+except ZOPE_SECURITY_NOT_AVAILABLE_EX:  # pragma: no cover
     def removeSecurityProxy(x):
         return x
 
-from zope.component.globalregistry import getGlobalSiteManager
 from zope.interface.interfaces import ComponentLookupError
 from zope.interface.interfaces import IComponentLookup
 
+from zope.component.globalregistry import getGlobalSiteManager
+
+
 __all__ = [
     'setSite',
     'getSite',
     'site',
     'getSiteManager',
     'setHooks',
     'resetHooks',
 ]
 
-class read_property(object):
+
+class read_property:
     """Descriptor for property-like computed attributes.
 
     Unlike the standard 'property', this descriptor allows assigning a
     value to the instance, shadowing the property getter function.
     """
+
     def __init__(self, func):
         self.func = func
 
     def __get__(self, inst, cls):
         if inst is None:
             return self
 
         return self.func(inst)
 
+
 class SiteInfo(threading.local):
     site = None
     sm = getGlobalSiteManager()
 
     @read_property
     def adapter_hook(self):
         adapter_hook = self.sm.adapters.adapter_hook
         self.adapter_hook = adapter_hook
         return adapter_hook
 
+
 siteinfo = SiteInfo()
 
+
 def setSite(site=None):
     if site is None:
         sm = getGlobalSiteManager()
     else:
 
         # We remove the security proxy because there's no way for
         # untrusted code to get at it without it being proxied again.
@@ -85,14 +93,15 @@
     siteinfo.site = site
     siteinfo.sm = sm
     try:
         del siteinfo.adapter_hook
     except AttributeError:
         pass
 
+
 def getSite():
     return siteinfo.site
 
 
 @contextlib.contextmanager
 def site(site):
     """
@@ -148,14 +157,15 @@
 
     .. seealso:: :mod:`zope.component.testlayer`
     """
     from zope.component import _api
     _api.adapter_hook.sethook(adapter_hook)
     _api.getSiteManager.sethook(getSiteManager)
 
+
 def resetHooks():
     """
     Reset `zope.component.getSiteManager` and interface adaptation to
     their original implementations that are unaware of the current
     site.
 
     Use caution when calling this; most code will not need to call
@@ -171,15 +181,16 @@
     # be sure the old adapter hook isn't cached, since
     # it is derived from the SiteManager
     try:
         del siteinfo.adapter_hook
     except AttributeError:
         pass
 
+
 # Clear the site thread global
 clearSite = setSite
 try:
     from zope.testing.cleanup import addCleanUp
-except ImportError: #pragma NO COVER
+except ImportError:  # pragma: no cover
     pass
 else:
     addCleanUp(resetHooks)
```

### Comparing `zope.component-5.1.0/src/zope/component/interface.py` & `zope.component-6.0/src/zope/component/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,35 +10,34 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Interface utility functions
 """
 from zope.interface import alsoProvides
+from zope.interface.interfaces import ComponentLookupError
 from zope.interface.interfaces import IInterface
 
-from zope.interface.interfaces import ComponentLookupError
 from zope.component._api import getSiteManager
 from zope.component._api import queryUtility
-from zope.component._compat import CLASS_TYPES
 
 
 def provideInterface(id, interface, iface_type=None, info=''):
     """
     Mark *interface* as a named utility providing *iface_type*'.
 
     .. versionchanged:: 5.0.0
        The named utility is registered in the current site manager.
        Previously it was always registered in the global site manager.
     """
     if not id:
-        id = "%s.%s" % (interface.__module__, interface.__name__)
+        id = "{}.{}".format(interface.__module__, interface.__name__)
 
     if not IInterface.providedBy(interface):
-        if not isinstance(interface, CLASS_TYPES):
+        if not isinstance(interface, type):
             raise TypeError(id, "is not an interface or class")
         return
 
     if iface_type is not None:
         if not iface_type.extends(IInterface):
             raise TypeError(iface_type, "is not an interface type")
         alsoProvides(interface, iface_type)
@@ -92,15 +91,15 @@
                if iface_util[1].isOrExtends(base)]
     else:
         res = list(iface_utilities)
     return res
 
 
 def getInterfaceAllDocs(interface):
-    iface_id = '%s.%s' % (interface.__module__, interface.__name__)
+    iface_id = '{}.{}'.format(interface.__module__, interface.__name__)
     docs = [str(iface_id).lower(),
             str(interface.__doc__).lower()]
 
     if IInterface.providedBy(interface):
         for name in sorted(interface):
             docs.append(
                 str(interface.getDescriptionFor(name).__doc__).lower())
@@ -114,8 +113,8 @@
     iface = getInterface(context, id)
     return iface
 
 
 def interfaceToName(context, interface):
     if interface is None:
         return 'None'
-    return '%s.%s' % (interface.__module__, interface.__name__)
+    return '{}.{}'.format(interface.__module__, interface.__name__)
```

### Comparing `zope.component-5.1.0/src/zope/component/interfaces.py` & `zope.component-6.0/src/zope/component/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 The `IComponentArchitecture` and `IComponentRegistrationConvenience` interfaces
 are provided by `zope.component` directly.
 """
 from zope.interface import Attribute
 from zope.interface import Interface
 
+
 # pylint:disable=inherit-non-class,no-self-argument,no-method-argument
 
 class IComponentArchitecture(Interface):
     """The Component Architecture is defined by two key components: Adapters
     and Utiltities. Both are managed by site managers. All other components
     build on top of them.
     """
@@ -72,15 +73,16 @@
         specified name. If no utility was found, return the specified *default*
         value.
         """
 
     def getNextUtility(context, interface, name=''):
         """Get the next available utility.
 
-        If no utility was found, a `~zope.interface.interfaces.ComponentLookupError` is raised.
+        If no utility was found, a
+        `~zope.interface.interfaces.ComponentLookupError` is raised.
         """
 
     def getUtilitiesFor(interface, context=None):
         """Return the utilities that provide an interface
 
         An iterable of utility name-value pairs is returned.
         """
@@ -93,20 +95,21 @@
         An iterable of utility instances is returned.  No names are
         returned.
         """
 
     # Adapter API
 
     def getAdapter(object,
-                   interface=Interface, name=u'',
+                   interface=Interface, name='',
                    context=None):
         """Get a named adapter to an interface for an object
 
         Returns an adapter that can adapt object to interface.  If a matching
-        adapter cannot be found, raises `~zope.interface.interfaces.ComponentLookupError`.
+        adapter cannot be found, raises
+        `~zope.interface.interfaces.ComponentLookupError`.
         """
 
     def getAdapterInContext(object, interface, context):
         """Get a special adapter to an interface for an object
 
         .. note::
             This method should only be used if a custom context
@@ -136,15 +139,15 @@
         `~zope.interface.interfaces.ComponentLookupError`.
 
         The name consisting of an empty string is reserved for unnamed
         adapters. The unnamed adapter methods will often call the
         named adapter methods with an empty string for a name.
         """
 
-    def queryAdapter(object, interface=Interface, name=u'',
+    def queryAdapter(object, interface=Interface, name='',
                      default=None, context=None):
         """Look for a named adapter to an interface for an object
 
         Returns an adapter that can adapt object to interface. If a
         matching adapter cannot be found, returns the default.
         """
 
@@ -167,15 +170,15 @@
         called with the requested interface. If the method returns a
         non-None value, that value will be returned. Otherwise, if the
         object already implements the interface, the object will be
         returned.
         """
 
     def queryMultiAdapter(objects,
-                          interface=Interface, name=u'',
+                          interface=Interface, name='',
                           default=None,
                           context=None):
         """Look for a multi-adapter to an interface for objects
 
         Returns a multi-adapter that can adapt objects to interface.  If a
         matching adapter cannot be found, returns the default.
 
@@ -252,35 +255,36 @@
     """Object that supports component registry
     """
 
     def registrations():
         """Return an iterable of component registrations
         """
 
+
 class IComponentRegistrationConvenience(Interface):
     """API for registering components.
 
     .. caution::
         This API should only be used from test or
         application-setup code. This api shouldn't be used by regular
         library modules, as component registration is a configuration
         activity.
     """
 
-    def provideUtility(component, provides=None, name=u''):
+    def provideUtility(component, provides=None, name=''):
         """Register a utility globally
 
         A utility is registered to provide an interface with a
         name. If a component provides only one interface, then the
         provides argument can be omitted and the provided interface
         will be used. (In this case, provides argument can still be
         provided to provide a less specific interface.)
         """
 
-    def provideAdapter(factory, adapts=None, provides=None, name=u''):
+    def provideAdapter(factory, adapts=None, provides=None, name=''):
         """Register an adapter globally
 
         An adapter is registered to provide an interface with a name
         for some number of object types. If a factory implements only
         one interface, then the provides argument can be omitted and
         the provided interface will be used. (In this case, a provides
         argument can still be provided to provide a less specific
@@ -329,32 +333,33 @@
 
     def getSiteManager():
         """Returns the site manager contained in this object.
 
         If there isn't a site manager, raise a component lookup.
         """
 
+
 class ISite(IPossibleSite):
     """Marker interface to indicate that we have a site"""
 
+
 class Misused(Exception):
     """A component is being used (registered) for the wrong interface."""
 
 
 class IFactory(Interface):
     """A factory is responsible for creating other components."""
 
     title = Attribute("The factory title.")
 
     description = Attribute("A brief description of the factory.")
 
     def __call__(*args, **kw):
         """Return an instance of the objects we're a factory for."""
 
-
     def getInterfaces():
         """Get the interfaces implemented by the factory
 
         Return the interface(s), as an instance of Implements, that objects
         created by this factory will implement. If the callable's Implements
         instance cannot be created, an empty Implements instance is returned.
         """
@@ -363,25 +368,28 @@
 # Internal helpers
 
 def _inherits_docs(func, iface):
     doc = iface[func.__name__].__doc__
 
     # doc can be None if the interpreter drops all docstrings when the
     # environment variable PYTHONOPTIMIZE is set 2.
-    if not doc:
-        return func
+    if doc is None:
+        return func  # pragma: no cover
 
     # By adding the ..seealso:: we get a link from our overview page
     # to the specific narrative place where the function is described, because
     # our overview page uses :noindex:
     doc += "\n        .. seealso::"
-    doc += "\n           Function `~zope.component.%s` for notes, and " % (func.__name__,)
-    doc += "\n           `~zope.component.interfaces.%s` for the defining interface." % (iface.__name__,)
-    doc += "\n"
+    doc += f"\n           Function `~zope.component.{func.__name__}` for"
+    doc += " notes, and "
+    doc += f"\n           `~zope.component.interfaces.{iface.__name__}` for"
+    doc += " the defining interface.\n"
     func.__doc__ = doc
     return func
 
+
 def inherits_arch_docs(func):
     return _inherits_docs(func, IComponentArchitecture)
 
+
 def inherits_reg_docs(func):
     return _inherits_docs(func, IComponentRegistrationConvenience)
```

### Comparing `zope.component-5.1.0/src/zope/component/meta.zcml` & `zope.component-6.0/src/zope/component/meta.zcml`

 * *Files identical despite different names*

### Comparing `zope.component-5.1.0/src/zope/component/persistentregistry.py` & `zope.component-6.0/src/zope/component/persistentregistry.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Persistent component managers.
 """
 from persistent import Persistent
-from persistent.mapping import PersistentMapping
 from persistent.list import PersistentList
+from persistent.mapping import PersistentMapping
 from zope.interface.adapter import VerifyingAdapterRegistry
 from zope.interface.registry import Components
 
+
 class PersistentAdapterRegistry(VerifyingAdapterRegistry, Persistent):
     """
     An adapter registry that is also a persistent object.
 
     .. versionchanged:: 5.0.0
         Internal data structures are now composed of
         :class:`persistent.mapping.PersistentMapping` and
@@ -59,22 +60,24 @@
     # migrate it, but not otherwise (we don't want to write in an
     # otherwise read-only transaction).
     def _addValueToLeaf(self, existing_leaf_sequence, new_item):
         if not existing_leaf_sequence:
             existing_leaf_sequence = self._leafSequenceType()
         elif isinstance(existing_leaf_sequence, tuple):
             # Converting from old state.
-            existing_leaf_sequence = self._leafSequenceType(existing_leaf_sequence)
+            existing_leaf_sequence = self._leafSequenceType(
+                existing_leaf_sequence)
         existing_leaf_sequence.append(new_item)
         return existing_leaf_sequence
 
     def _removeValueFromLeaf(self, existing_leaf_sequence, to_remove):
         if isinstance(existing_leaf_sequence, tuple):
             # Converting from old state
-            existing_leaf_sequence = self._leafSequenceType(existing_leaf_sequence)
+            existing_leaf_sequence = self._leafSequenceType(
+                existing_leaf_sequence)
 
         without_removed = VerifyingAdapterRegistry._removeValueFromLeaf(
             self,
             existing_leaf_sequence,
             to_remove)
         existing_leaf_sequence[:] = without_removed
         return existing_leaf_sequence
@@ -86,26 +89,26 @@
             # because the super class will now increment the ``_generation``
             # attribute to keep caches in sync. For this same reason,
             # it's not worth trying to "optimize" for the case that we're a
             # new or rebuilt object containing only Persistent sub-objects:
             # the changed() mechanism will still result in mutating this
             # object via ``_generation``.
             self._p_changed = True
-        super(PersistentAdapterRegistry, self).changed(originally_changed)
+        super().changed(originally_changed)
 
     def __getstate__(self):
-        state = super(PersistentAdapterRegistry, self).__getstate__().copy()
+        state = super().__getstate__().copy()
         for name in self._delegated:
             state.pop(name, 0)
         state.pop('ro', None)
         return state
 
     def __setstate__(self, state):
         bases = state.pop('__bases__', ())
-        super(PersistentAdapterRegistry, self).__setstate__(state)
+        super().__setstate__(state)
         self._createLookup()
         self.__bases__ = bases
         self._v_lookup.changed(self)
 
 
 class PersistentComponents(Components):
     """
```

### Comparing `zope.component-5.1.0/src/zope/component/registry.py` & `zope.component-6.0/src/zope/component/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,31 +10,35 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Basic components support
 """
 
-from zope.component._api import handle
-from zope.component._declaration import adapter
-
 from zope.interface.interfaces import IAdapterRegistration
 from zope.interface.interfaces import IHandlerRegistration
 from zope.interface.interfaces import IRegistrationEvent
 from zope.interface.interfaces import ISubscriptionAdapterRegistration
 from zope.interface.interfaces import IUtilityRegistration
 
+from zope.component._api import handle
+from zope.component._declaration import adapter
+
+
 @adapter(IUtilityRegistration, IRegistrationEvent)
 def dispatchUtilityRegistrationEvent(registration, event):
     handle(registration.component, event)
 
+
 @adapter(IAdapterRegistration, IRegistrationEvent)
 def dispatchAdapterRegistrationEvent(registration, event):
     handle(registration.factory, event)
 
+
 @adapter(ISubscriptionAdapterRegistration, IRegistrationEvent)
 def dispatchSubscriptionAdapterRegistrationEvent(registration, event):
     handle(registration.factory, event)
 
+
 @adapter(IHandlerRegistration, IRegistrationEvent)
 def dispatchHandlerRegistrationEvent(registration, event):
     handle(registration.handler, event)
```

### Comparing `zope.component-5.1.0/src/zope/component/security.py` & `zope.component-6.0/src/zope/component/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 """
 from zope.interface import providedBy
 from zope.proxy import ProxyBase
 from zope.proxy import getProxiedObject
 
 from zope.component._compat import ZOPE_SECURITY_NOT_AVAILABLE_EX
 
+
 try:
     from zope.security.adapter import LocatingTrustedAdapterFactory
     from zope.security.adapter import LocatingUntrustedAdapterFactory
     from zope.security.adapter import TrustedAdapterFactory
     from zope.security.checker import Checker
     from zope.security.checker import CheckerPublic
     from zope.security.checker import InterfaceChecker
     from zope.security.proxy import Proxy
-except ZOPE_SECURITY_NOT_AVAILABLE_EX: # pragma: no cover
+except ZOPE_SECURITY_NOT_AVAILABLE_EX:  # pragma: no cover
     def _no_security(*args, **kw):
         raise TypeError(
             "security proxied components are not "
             "supported because zope.security is not available")
 
     LocatingTrustedAdapterFactory = _no_security
     LocatingUntrustedAdapterFactory = _no_security
@@ -39,22 +40,24 @@
     Checker = _no_security
     CheckerPublic = _no_security
     InterfaceChecker = _no_security
 
 
 PublicPermission = 'zope.Public'
 
+
 class PermissionProxy(ProxyBase):
 
     __slots__ = ('__Security_checker__', )
 
     def __providedBy__(self):
         return providedBy(getProxiedObject(self))
     __providedBy__ = property(__providedBy__)
 
+
 def _checker(_context, permission, allowed_interface, allowed_attributes):
     if (not allowed_attributes) and (not allowed_interface):
         allowed_attributes = ["__call__"]
 
     if permission == PublicPermission:
         permission = CheckerPublic
 
@@ -66,14 +69,15 @@
         for i in allowed_interface:
             for name in i.names(all=True):
                 require[name] = permission
 
     checker = Checker(require)
     return checker
 
+
 def proxify(ob, checker=None, provides=None, permission=None):
     """Try to get the object proxied with the `checker`, but not too soon
 
     We really don't want to proxy the object unless we need to.
     """
 
     if checker is None:
@@ -83,29 +87,32 @@
         if permission == PublicPermission:
             permission = CheckerPublic
         checker = InterfaceChecker(provides, permission)
     ob = PermissionProxy(ob)
     ob.__Security_checker__ = checker
     return ob
 
+
 def protectedFactory(original_factory, provides, permission):
     if permission == PublicPermission:
         permission = CheckerPublic
     checker = InterfaceChecker(provides, permission)
     # This has to be named 'factory', aparently, so as not to confuse apidoc :(
+
     def factory(*args):
         ob = original_factory(*args)
         try:
             ob.__Security_checker__ = checker
         except AttributeError:
             ob = Proxy(ob, checker)
         return ob
     factory.factory = original_factory
     return factory
 
+
 def securityAdapterFactory(factory, permission, locate, trusted):
     if permission == PublicPermission:
         permission = CheckerPublic
     if locate or (permission is not None and permission is not CheckerPublic):
         if trusted:
             return LocatingTrustedAdapterFactory(factory)
         else:
```

### Comparing `zope.component-5.1.0/src/zope/component/standalonetests.py` & `zope.component-6.0/src/zope/component/standalonetests.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 """
 See: https://bugs.launchpad.net/zope3/+bug/98401
 """
 
-import sys
 import pickle
+import sys
+
 
 def write(x):
     sys.stdout.write('%s\n' % x)
 
+
 if __name__ == "__main__":
-    if sys.version_info[0] >= 3:
-        # TextIO? Are you kidding me?
-        data = sys.stdin.buffer.read()
-    else:
-        data = sys.stdin.read()
+    # TextIO? Are you kidding me?
+    data = sys.stdin.buffer.read()
     sys.path = pickle.loads(data)
     write('XXXXXXXXXX')
     for p in sys.path:
         write('- %s' % p)
     write('XXXXXXXXXX')
 
-    import zope
     from zope.interface import Interface
     from zope.interface import implementer
 
+    import zope
+
     class I1(Interface):
         pass
 
     class I2(Interface):
         pass
 
     @implementer(I1)
-    class Ob(object):
+    class Ob:
         def __repr__(self):
             return '<instance Ob>'
 
     ob = Ob()
 
     @implementer(I2)
-    class Comp(object):
+    class Comp:
         def __init__(self, context):
             self.context = context
 
     write('YYYYYYYYY')
     for p in zope.__path__:
         write('- %s' % p)
     write('YYYYYYYYY')
```

### Comparing `zope.component-5.1.0/src/zope/component/testfiles/adapter.py` & `zope.component-6.0/src/zope/component/testfiles/adapter.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,53 +16,70 @@
 
 from zope.interface import Interface
 from zope.interface import implementer
 
 from zope.component import adapter
 from zope.component.testfiles import components
 
+
 class I1(Interface):
     pass
 
+
 class I2(Interface):
     pass
 
+
 class I3(Interface):
-    def f1(): pass
-    def f2(): pass
-    def f3(): pass
+    def f1():
+        pass  # pragma: no cover
+
+    def f2():
+        pass  # pragma: no cover
+
+    def f3():
+        pass  # pragma: no cover
+
 
 class IS(Interface):
     pass
 
 
-class Adapter(object):
+class Adapter:
     def __init__(self, *args):
         self.context = args
 
+
 @implementer(I1)
 class A1(Adapter):
     pass
 
+
 @implementer(I2)
 class A2(Adapter):
     pass
 
+
 @adapter(components.IContent, I1, I2)
 @implementer(I3)
 class A3(Adapter):
     pass
 
+
 class A4:
     pass
 
+
 a4 = A4()
 
+
 @implementer(I1, I2)
 class A5:
     pass
 
+
 a5 = A5()
 
+
 def Handler(content, *args):
     # uninteresting handler
     content.args = getattr(content, 'args', ()) + (args, )
```

### Comparing `zope.component-5.1.0/src/zope/component/testfiles/components.py` & `zope.component-6.0/src/zope/component/testfiles/components.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,58 +9,74 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Components for testing
 """
-from zope.interface import Interface
 from zope.interface import Attribute
+from zope.interface import Interface
 from zope.interface import implementer
+
 from zope.component import adapter
 from zope.component import named
 
+
 class IAppb(Interface):
     a = Attribute('test attribute')
-    def f(): "test func"
+
+    def f():
+        "test func"
+
 
 class IApp(IAppb):
     pass
 
+
 class IApp2(IAppb):
     pass
 
+
 class IApp3(IAppb):
     pass
 
-class IContent(Interface): pass
+
+class IContent(Interface):
+    pass
+
 
 @implementer(IContent)
-class Content(object):
+class Content:
     pass
 
+
 @adapter(IContent)
 @implementer(IApp)
-class Comp(object):
+class Comp:
 
     def __init__(self, *args):
         # Ignore arguments passed to constructor
         pass
 
     a = 1
-    def f(): pass
 
-class Comp2(object):
+    def f():
+        pass  # pragma: no cover
+
+
+class Comp2:
     def __init__(self, context):
         self.context = context
 
+
 @adapter(IContent)
 @implementer(IApp)
 @named('app')
-class Comp4(object):
+class Comp4:
     def __init__(self, context=None):
         self.context = context
 
+
 comp = Comp()
 comp4 = Comp4()
 
 content = Content()
```

### Comparing `zope.component-5.1.0/src/zope/component/testfiles/views.py` & `zope.component-6.0/src/zope/component/testfiles/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 #
 ##############################################################################
 """Views test.
 """
 
 from zope.interface import Interface
 
+
 class IC(Interface):
     pass
```

### Comparing `zope.component-5.1.0/src/zope/component/testing.py` & `zope.component-6.0/src/zope/component/testing.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,27 +11,31 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Placeless Test Setup
 """
 
 # HACK to make sure basicmost event subscriber is installed
-import zope.component.event
+import zope.component.event  # noqa: F401 imported but unused
+
 
 # we really don't need special setup now:
-class _PlacelessSetupFallback(object):
+class _PlacelessSetupFallback:
     def cleanUp(self):
         from zope.component.globalregistry import base
         base.__init__('base')
 
     setUp = tearDown = cleanUp
 
+
 try:
     from zope.testing.cleanup import CleanUp as PlacelessSetup
-except ImportError: # pragma: no cover
+except ImportError:  # pragma: no cover
     PlacelessSetup = _PlacelessSetupFallback
 
+
 def setUp(test=None):
     PlacelessSetup().setUp()
 
+
 def tearDown(test=None):
     PlacelessSetup().tearDown()
```

### Comparing `zope.component-5.1.0/src/zope/component/testlayer.py` & `zope.component-6.0/src/zope/component/testlayer.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,27 +10,31 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 import os
 
-from zope.configuration import xmlconfig, config
+from zope.configuration import config
+from zope.configuration import xmlconfig
+
+
 try:
     from zope.testing.cleanup import cleanUp
-except ImportError: # pragma: no cover
+except ImportError:  # pragma: no cover
     def cleanUp():
         pass
 
 from zope.component import provideHandler
+from zope.component.eventtesting import clearEvents
+from zope.component.eventtesting import events
 from zope.component.hooks import setHooks
-from zope.component.eventtesting import events, clearEvents
 
 
-class LayerBase(object):
+class LayerBase:
     """Sane layer base class.
 
     zope.testing implements an advanced mechanism so that layer setUp,
     tearDown, testSetUp and testTearDown code gets called in the right
     order. These methods are supposed to be @classmethods and should
     not use super() as the test runner is supposed to take care of that.
 
@@ -71,19 +75,21 @@
 
     def testSetUp(self):
         pass
 
     def testTearDown(self):
         pass
 
+
 class ZCMLLayerBase(LayerBase):
     """Base class to load up some ZCML.
     """
+
     def __init__(self, package, name=None, features=None):
-        super(ZCMLLayerBase, self).__init__(package, name)
+        super().__init__(package, name)
         self.features = features or []
 
     def setUp(self):
         setHooks()
         context = config.ConfigurationMachine()
         xmlconfig.registerCommonDirectives(context)
         for feature in self.features:
@@ -96,25 +102,27 @@
 
     def tearDown(self):
         cleanUp()
 
     def _load_zcml(self, context):
         raise NotImplementedError
 
+
 class ZCMLFileLayer(ZCMLLayerBase):
     """This layer can be used to run tests with a ZCML file loaded.
 
     The ZCML file is assumed to include sufficient (meta)configuration
     so that it can be interpreted itself. I.e. to create a ZCMLLayer
     based on another ZCMLLayer's ZCML, just use a ZCML include
     statement in your own ZCML to load it.
     """
+
     def __init__(self, package, zcml_file='ftesting.zcml',
                  name=None, features=None):
-        super(ZCMLFileLayer, self).__init__(package, name, features)
+        super().__init__(package, name, features)
         self.zcml_file = os.path.join(os.path.dirname(package.__file__),
                                       zcml_file)
 
     def _load_zcml(self, context):
         return xmlconfig.file(self.zcml_file,
                               package=self.package,
                               context=context, execute=True)
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/__init__.py` & `zope.component-6.0/src/zope/component/tests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import unittest
 
+
 def skipIfNoSecurity(testfunc):
     from zope.component._compat import ZOPE_SECURITY_NOT_AVAILABLE_EX
 
     try:
-        import zope.security
-    except ZOPE_SECURITY_NOT_AVAILABLE_EX: # pragma: no cover
+        import zope.security  # noqa: F401 imported but unused
+    except ZOPE_SECURITY_NOT_AVAILABLE_EX:  # pragma: no cover
         return unittest.skip("zope.security not installed")(testfunc)
     return testfunc
 
+
 def fails_if_called(test, msg="This function must not be called.",
                     arguments=True):
     """
     Return a new function (accepting any arguments)
     that will call test.fail(msg) if it is called.
 
     :keyword bool arguments: If set to ``False``, then we will
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/examples.py` & `zope.component-6.0/src/zope/component/tests/examples.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,127 +16,152 @@
 import sys
 
 from zope.interface import Interface
 from zope.interface import implementer
 from zope.interface.interfaces import IInterface
 
 from zope.component._declaration import adapter
+from zope.component.globalregistry import GlobalAdapterRegistry
 from zope.component.testfiles.views import IC
 
+
 def write(x):
     sys.stdout.write('%s\n' % x)
 
+
 class ITestType(IInterface):
     pass
 
 
 class I1(Interface):
     pass
 
+
 class I2(Interface):
     pass
 
+
 class I3(Interface):
     pass
 
+
 class I4(Interface):
     pass
 
+
 class IGI(Interface):
     pass
 
+
 class IQI(Interface):
     pass
 
+
 class ISI(Interface):
     pass
 
+
 class ISII(Interface):
     pass
 
-class U(object):
+
+class U:
 
     def __init__(self, name):
         self.__name__ = name
 
     def __repr__(self):
-        return "%s(%s)" % (self.__class__.__name__, self.__name__)
+        return "{}({})".format(self.__class__.__name__, self.__name__)
+
 
 @implementer(I1)
 class U1(U):
     pass
 
+
 @implementer(I1, I2)
 class U12(U):
     pass
 
+
 @adapter(I1)
 def handle1(x):
     write('handle1 %s' % x)
 
+
 def handle2(*objects):
-    write( 'handle2 ' + repr(objects))
+    write('handle2 ' + repr(objects))
+
 
 @adapter(I1)
 def handle3(x):
-    write( 'handle3 %s' % x)
+    write('handle3 %s' % x)
+
 
 @adapter(I1)
 def handle4(x):
-    write( 'handle4 %s' % x)
+    write('handle4 %s' % x)
+
 
 class GlobalRegistry:
     pass
 
-from zope.component.globalregistry import GlobalAdapterRegistry
+
 base = GlobalAdapterRegistry(GlobalRegistry, 'adapters')
 GlobalRegistry.adapters = base
+
+
 def clear_base():
     base.__init__(GlobalRegistry, 'adapters')
 
 
 @implementer(I1)
-class Ob(object):
+class Ob:
     def __repr__(self):
         return '<instance Ob>'
 
 
 ob = Ob()
 
+
 @implementer(I2)
-class Ob2(object):
+class Ob2:
     def __repr__(self):
         return '<instance Ob2>'
 
+
 @implementer(IC)
-class Ob3(object):
+class Ob3:
     pass
 
+
 @implementer(I2)
-class Comp(object):
+class Comp:
     def __init__(self, context):
         self.context = context
 
+
 comp = Comp(1)
 
 
-class ConformsToIComponentLookup(object):
+class ConformsToIComponentLookup:
     """Allow a dummy sitemanager to conform/adapt to `IComponentLookup`."""
 
     def __init__(self, sitemanager):
         self.sitemanager = sitemanager
 
     def __conform__(self, interface):
         """This method is specified by the adapter PEP to do the adaptation."""
         from zope.interface.interfaces import IComponentLookup
         if interface is IComponentLookup:
             return self.sitemanager
 
 
 def clearZCML(test=None):
     from zope.configuration.xmlconfig import XMLConfig
+
     import zope.component
     from zope.component.testing import setUp
     from zope.component.testing import tearDown
     tearDown()
     setUp()
     XMLConfig('meta.zcml', zope.component)()
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test___init__.py` & `zope.component-6.0/src/zope/component/tests/test___init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,75 +10,89 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 import unittest
 
+
 class Test_package(unittest.TestCase):
 
     def test_module_conforms_to_IComponentArchitecture(self):
         from zope.interface.verify import verifyObject
-        from zope.component.interfaces import IComponentArchitecture
+
         import zope.component as zc
+        from zope.component.interfaces import IComponentArchitecture
         verifyObject(IComponentArchitecture, zc)
 
     def test_module_conforms_to_IComponentRegistrationConvenience(self):
         from zope.interface.verify import verifyObject
-        from zope.component.interfaces import IComponentRegistrationConvenience
+
         import zope.component as zc
+        from zope.component.interfaces import IComponentRegistrationConvenience
         verifyObject(IComponentRegistrationConvenience, zc)
 
 
 class Test_Interface_call(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def test_miss(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         self.assertRaises(TypeError, IFoo, object())
 
     def test_miss_w_default(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         marker = object()
         self.assertTrue(IFoo(object(), marker) is marker)
 
     def test_hit(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         @implementer(IFoo)
-        class Baz(object):
+        class Baz:
             def __init__(self, context):
                 self.context = context
         getGlobalSiteManager().registerAdapter(Baz, (IBar,), IFoo, '')
         bar = Bar()
         adapted = IFoo(bar)
         self.assertTrue(adapted.__class__ is Baz)
         self.assertTrue(adapted.context is bar)
 
     def test_hit_registered_for_None(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         @implementer(IFoo)
-        class Baz(object):
+        class Baz:
             def __init__(self, context):
                 self.context = context
         getGlobalSiteManager().registerAdapter(Baz, (None,), IFoo, '')
         ctx = object()
         adapted = IFoo(ctx)
         self.assertTrue(adapted.__class__ is Baz)
         self.assertTrue(adapted.context is ctx)
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test__api.py` & `zope.component-6.0/src/zope/component/tests/test__api.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 ##############################################################################
 """ Tests for z.c._api
 """
 import unittest
 
 from zope.component.tests import fails_if_called
 
+
 class Test_getSiteManager(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component._api import getSiteManager
         return getSiteManager(*args, **kw)
 
     def test_sm_is_IComponentLookup(self):
         from zope.interface.interfaces import IComponentLookup
@@ -47,60 +49,71 @@
 
     def test_getSiteManager_w_invalid_context_no_adapter(self):
         from zope.interface.interfaces import ComponentLookupError
         self.assertRaises(ComponentLookupError, self._callFUT, object())
 
     def test_getSiteManager_w_invalid_context_w_adapter(self):
         from zope.interface import Interface
-        from zope.component.globalregistry import getGlobalSiteManager
         from zope.interface.interfaces import IComponentLookup
+
+        from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
         sm = object()
+
         def _adapt(x):
             return sm
         gsm.registerAdapter(_adapt, (Interface,), IComponentLookup, '')
         self.assertTrue(self._callFUT(object()) is sm)
 
 
 class Test_getAdapterInContext(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import getAdapterInContext
         return getAdapterInContext(*args, **kw)
 
     def test_miss(self):
         from zope.interface import Interface
         from zope.interface.interfaces import ComponentLookupError
+
         class IFoo(Interface):
             pass
         self.assertRaises(ComponentLookupError,
                           self._callFUT, object(), IFoo, context=None)
 
     def test_hit_via_sm(self):
         from zope.interface import Interface
         from zope.interface import implementer
         from zope.interface.registry import Components
+
         from zope.component import getGlobalSiteManager
         from zope.component.tests.examples import ConformsToIComponentLookup
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @implementer(IFoo)
-        class Global(object):
+        class Global:
             __init__ = fails_if_called(self)
+
         @implementer(IFoo)
-        class Local(object):
+        class Local:
             def __init__(self, context):
                 self.context = context
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         class Context(ConformsToIComponentLookup):
             def __init__(self, sm):
                 self.sitemanager = sm
         gsm = getGlobalSiteManager()
         gsm.registerAdapter(Global, (IBar,), IFoo, '')
         sm1 = Components('sm1', bases=(gsm, ))
         sm1.registerAdapter(Local, (IBar,), IFoo, '')
@@ -108,15 +121,16 @@
         adapted = self._callFUT(bar, IFoo, context=Context(sm1))
         self.assertTrue(adapted.__class__ is Local)
         self.assertTrue(adapted.context is bar)
 
 
 class Test_queryAdapterInContext(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import queryAdapterInContext
         return queryAdapterInContext(*args, **kw)
 
     def test_miss(self):
         from zope.interface import Interface
@@ -124,227 +138,267 @@
         class IFoo(Interface):
             pass
         self.assertEqual(
             self._callFUT(object(), IFoo, context=None), None)
 
     def test_w_object_conforming(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         _adapted = object()
-        class Foo(object):
+
+        class Foo:
             def __conform__(self, iface, default=None, _test=self):
                 _test.assertIs(iface, IFoo)
                 return _adapted
 
         self.assertTrue(
-                self._callFUT(Foo(), IFoo, context=None) is _adapted)
+            self._callFUT(Foo(), IFoo, context=None) is _adapted)
 
     def test___conform___raises_TypeError_via_class(self):
         from zope.interface import Interface
 
         class IFoo(Interface):
             pass
-        _adapted = object()
-        class Foo(object):
+
+        class Foo:
             __conform__ = fails_if_called(self, arguments=False)
         # call via class, triggering TypeError
         self.assertEqual(self._callFUT(Foo, IFoo, context=None), None)
 
     def test___conform___raises_TypeError_via_inst(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
-        _adapted = object()
-        class Foo(object):
+
+        class Foo:
             def __conform__(self, iface, default=None):
                 raise TypeError
         self.assertRaises(TypeError,
                           self._callFUT, Foo(), IFoo, context=None)
 
     def test_w_object_implementing(self):
         from zope.interface import Interface
         from zope.interface import implementer
 
         class IFoo(Interface):
             pass
+
         @implementer(IFoo)
-        class Foo(object):
-              pass
+        class Foo:
+            pass
         foo = Foo()
         self.assertIs(
-                self._callFUT(foo, IFoo, context=None), foo)
+            self._callFUT(foo, IFoo, context=None), foo)
 
 
 class Test_getAdapter(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import getAdapter
         return getAdapter(*args, **kw)
 
     def test_anonymous_nonesuch(self):
         from zope.interface import Interface
         from zope.interface.interfaces import ComponentLookupError
+
         class IFoo(Interface):
             pass
         self.assertRaises(ComponentLookupError,
                           self._callFUT, object(), IFoo, '')
 
     def test_named_nonesuch(self):
         from zope.interface import Interface
         from zope.interface.interfaces import ComponentLookupError
+
         class IFoo(Interface):
             pass
         self.assertRaises(ComponentLookupError,
                           self._callFUT, object(), IFoo, 'bar')
 
     def test_anonymous_hit(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         @implementer(IFoo)
-        class Baz(object):
+        class Baz:
             def __init__(self, context):
                 self.context = context
         getGlobalSiteManager().registerAdapter(Baz, (IBar,), IFoo, '')
         bar = Bar()
         adapted = self._callFUT(bar, IFoo, '')
         self.assertTrue(adapted.__class__ is Baz)
         self.assertTrue(adapted.context is bar)
 
     def test_anonymous_hit_registered_for_None(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         @implementer(IFoo)
-        class Baz(object):
+        class Baz:
             def __init__(self, context):
                 self.context = context
         getGlobalSiteManager().registerAdapter(Baz, (None,), IFoo, '')
         ctx = object()
         adapted = self._callFUT(ctx, IFoo, '')
         self.assertTrue(adapted.__class__ is Baz)
         self.assertTrue(adapted.context is ctx)
 
     def test_named_hit(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         @implementer(IFoo)
-        class Baz(object):
+        class Baz:
             def __init__(self, context):
                 self.context = context
         getGlobalSiteManager().registerAdapter(Baz, (IBar,), IFoo, 'named')
         bar = Bar()
         adapted = self._callFUT(bar, IFoo, 'named')
         self.assertTrue(adapted.__class__ is Baz)
         self.assertTrue(adapted.context is bar)
 
 
 class Test_queryAdapter(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import queryAdapter
         return queryAdapter(*args, **kw)
 
     def test_anonymous_nonesuch(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         self.assertEqual(self._callFUT(object(), IFoo, '', '<default>'),
                          '<default>')
 
     def test_named_nonesuch(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         self.assertEqual(self._callFUT(object(), IFoo, 'bar'), None)
 
     def test_anonymous_hit(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         @implementer(IFoo)
-        class Baz(object):
+        class Baz:
             def __init__(self, context):
                 self.context = context
         getGlobalSiteManager().registerAdapter(Baz, (IBar,), IFoo, '')
         bar = Bar()
         adapted = self._callFUT(bar, IFoo, '')
         self.assertTrue(adapted.__class__ is Baz)
         self.assertTrue(adapted.context is bar)
 
     def test_named_hit(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         @implementer(IFoo)
-        class Baz(object):
+        class Baz:
             def __init__(self, context):
                 self.context = context
         getGlobalSiteManager().registerAdapter(Baz, (IBar,), IFoo, 'named')
         bar = Bar()
         adapted = self._callFUT(bar, IFoo, 'named')
         self.assertTrue(adapted.__class__ is Baz)
         self.assertTrue(adapted.context is bar)
 
     def test_nested(self):
         from zope.interface import Interface
         from zope.interface import implementer
         from zope.interface.registry import Components
+
         from zope.component import getGlobalSiteManager
         from zope.component.tests.examples import ConformsToIComponentLookup
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @implementer(IFoo)
-        class Global(object):
+        class Global:
             __init__ = fails_if_called(self)
+
         @implementer(IFoo)
-        class Local(object):
+        class Local:
             def __init__(self, context):
                 self.context = context
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         class Context(ConformsToIComponentLookup):
             def __init__(self, sm):
                 self.sitemanager = sm
         gsm = getGlobalSiteManager()
         gsm.registerAdapter(Global, (IBar,), IFoo, '')
         sm1 = Components('sm1', bases=(gsm, ))
         sm1.registerAdapter(Local, (IBar,), IFoo, '')
@@ -352,227 +406,276 @@
         adapted = self._callFUT(bar, IFoo, '', context=Context(sm1))
         self.assertTrue(adapted.__class__ is Local)
         self.assertTrue(adapted.context is bar)
 
 
 class Test_getMultiAdapter(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import getMultiAdapter
         return getMultiAdapter(*args, **kw)
 
     def test_anonymous_nonesuch(self):
         from zope.interface import Interface
         from zope.interface.interfaces import ComponentLookupError
+
         class IFoo(Interface):
             pass
         self.assertRaises(ComponentLookupError,
                           self._callFUT, (object(), object()), IFoo, '')
 
     def test_named_nonesuch(self):
         from zope.interface import Interface
         from zope.interface.interfaces import ComponentLookupError
+
         class IFoo(Interface):
             pass
         self.assertRaises(ComponentLookupError,
                           self._callFUT, (object(), object()), IFoo, 'bar')
 
     def test_anonymous_hit(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         class IBaz(Interface):
             pass
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         @implementer(IBaz)
-        class Baz(object):
+        class Baz:
             pass
+
         @implementer(IFoo)
-        class FooAdapter(object):
+        class FooAdapter:
             def __init__(self, first, second):
                 self.first, self.second = first, second
         getGlobalSiteManager().registerAdapter(
-                                FooAdapter, (IBar, IBaz), IFoo, '')
+            FooAdapter, (IBar, IBaz), IFoo, '')
         bar = Bar()
         baz = Baz()
         adapted = self._callFUT((bar, baz), IFoo, '')
         self.assertTrue(adapted.__class__ is FooAdapter)
         self.assertTrue(adapted.first is bar)
         self.assertTrue(adapted.second is baz)
 
     def test_anonymous_hit_registered_for_None(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         class IBaz(Interface):
             pass
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         @implementer(IFoo)
-        class FooAdapter(object):
+        class FooAdapter:
             def __init__(self, first, second):
                 self.first, self.second = first, second
         getGlobalSiteManager().registerAdapter(
-                                FooAdapter, (IBar, None), IFoo, '')
+            FooAdapter, (IBar, None), IFoo, '')
         bar = Bar()
         baz = object()
         adapted = self._callFUT((bar, baz), IFoo, '')
         self.assertTrue(adapted.__class__ is FooAdapter)
         self.assertTrue(adapted.first is bar)
         self.assertTrue(adapted.second is baz)
 
     def test_named_hit(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         class IBaz(Interface):
             pass
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         @implementer(IBaz)
-        class Baz(object):
+        class Baz:
             pass
+
         @implementer(IFoo)
-        class FooAdapter(object):
+        class FooAdapter:
             def __init__(self, first, second):
                 self.first, self.second = first, second
         getGlobalSiteManager().registerAdapter(
-                                    FooAdapter, (IBar, IBaz), IFoo, 'named')
+            FooAdapter, (IBar, IBaz), IFoo, 'named')
         bar = Bar()
         baz = Baz()
         adapted = self._callFUT((bar, baz), IFoo, 'named')
         self.assertTrue(adapted.__class__ is FooAdapter)
         self.assertTrue(adapted.first is bar)
         self.assertTrue(adapted.second is baz)
 
 
 class Test_queryMultiAdapter(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import queryMultiAdapter
         return queryMultiAdapter(*args, **kw)
 
     def test_anonymous_nonesuch(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         self.assertEqual(self._callFUT((object(), object()), IFoo, '',
-                                            '<default>'),
+                                       '<default>'),
                          '<default>')
 
     def test_named_nonesuch(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         self.assertEqual(self._callFUT((object(), object()), IFoo, 'bar'),
                          None)
 
     def test_anonymous_hit(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         class IBaz(Interface):
             pass
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         @implementer(IBaz)
-        class Baz(object):
+        class Baz:
             pass
+
         @implementer(IFoo)
-        class FooAdapter(object):
+        class FooAdapter:
             def __init__(self, first, second):
                 self.first, self.second = first, second
         getGlobalSiteManager().registerAdapter(
-                                    FooAdapter, (IBar, IBaz), IFoo, '')
+            FooAdapter, (IBar, IBaz), IFoo, '')
         bar = Bar()
         baz = Baz()
         adapted = self._callFUT((bar, baz), IFoo, '')
         self.assertTrue(adapted.__class__ is FooAdapter)
         self.assertTrue(adapted.first is bar)
         self.assertTrue(adapted.second is baz)
 
     def test_named_hit(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         class IBaz(Interface):
             pass
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         @implementer(IBaz)
-        class Baz(object):
+        class Baz:
             pass
+
         @implementer(IFoo)
-        class FooAdapter(object):
+        class FooAdapter:
             def __init__(self, first, second):
                 self.first, self.second = first, second
         getGlobalSiteManager().registerAdapter(
-                                    FooAdapter, (IBar, IBaz), IFoo, 'named')
+            FooAdapter, (IBar, IBaz), IFoo, 'named')
         bar = Bar()
         baz = Baz()
         adapted = self._callFUT((bar, baz), IFoo, 'named')
         self.assertTrue(adapted.__class__ is FooAdapter)
         self.assertTrue(adapted.first is bar)
         self.assertTrue(adapted.second is baz)
 
     def test_nested(self):
         from zope.interface import Interface
         from zope.interface import implementer
         from zope.interface.registry import Components
+
         from zope.component import getGlobalSiteManager
         from zope.component.tests.examples import ConformsToIComponentLookup
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         class IBaz(Interface):
             pass
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         @implementer(IBaz)
-        class Baz(object):
+        class Baz:
             pass
+
         @implementer(IFoo)
-        class Global(object):
+        class Global:
             __init__ = fails_if_called(self)
+
         @implementer(IFoo)
-        class Local(object):
+        class Local:
             def __init__(self, first, second):
                 self.first, self.second = first, second
+
         class Context(ConformsToIComponentLookup):
             def __init__(self, sm):
                 self.sitemanager = sm
         gsm = getGlobalSiteManager()
         gsm.registerAdapter(Global, (IBar, IBaz), IFoo, '')
         sm1 = Components('sm1', bases=(gsm, ))
         sm1.registerAdapter(Local, (IBar, IBaz), IFoo, '')
@@ -583,58 +686,70 @@
         self.assertTrue(adapted.first is bar)
         self.assertTrue(adapted.second is baz)
 
     def test_wo_sitemanager(self):
         from zope.interface import Interface
         from zope.interface import implementer
         from zope.interface.interfaces import ComponentLookupError
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         class IBaz(Interface):
             pass
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         @implementer(IBaz)
-        class Baz(object):
+        class Baz:
             pass
-        class Context(object):
+
+        class Context:
             def __conform__(self, iface):
                 raise ComponentLookupError
         bar = Bar()
         baz = Baz()
         adapted = self._callFUT((bar, baz), IFoo, '', context=Context())
         self.assertTrue(adapted is None)
 
 
 class Test_getAdapters(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import getAdapters
         return getAdapters(*args, **kw)
 
     def test_nonesuch(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         self.assertEqual(list(self._callFUT((object(),), IFoo)), [])
 
     def test_hit(self):
         from zope.interface import Interface
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
-        class BarAdapter(object):
+
+        class BarAdapter:
             def __init__(self, context):
                 self.context = context
-        class BazAdapter(object):
+
+        class BazAdapter:
             def __init__(self, context):
                 self.context = context
         gsm = getGlobalSiteManager()
         gsm.registerAdapter(BarAdapter, (None,), IFoo)
         gsm.registerAdapter(BazAdapter, (None,), IFoo, name='bar')
         tuples = list(self._callFUT((object(),), IFoo))
         self.assertEqual(len(tuples), 2)
@@ -642,298 +757,352 @@
         self.assertTrue(('', 'BarAdapter') in names)
         self.assertTrue(('bar', 'BazAdapter') in names)
 
     def test_wo_sitemanager(self):
         from zope.interface import Interface
         from zope.interface import implementer
         from zope.interface.interfaces import ComponentLookupError
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         class IBaz(Interface):
             pass
+
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             pass
+
         @implementer(IBaz)
-        class Baz(object):
+        class Baz:
             pass
-        class Context(object):
+
+        class Context:
             def __conform__(self, iface):
                 raise ComponentLookupError
         bar = Bar()
         baz = Baz()
         adapted = self._callFUT((bar, baz), IFoo, context=Context())
         self.assertEqual(adapted, [])
 
 
 class Test_subscribers(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import subscribers
         return subscribers(*args, **kw)
 
     def test_nonesuch(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         subscribers = self._callFUT((object,), IFoo)
         self.assertEqual(subscribers, [])
 
     def test_hit(self):
         from zope.interface import Interface
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
-        class BarAdapter(object):
+
+        class BarAdapter:
             def __init__(self, context):
                 self.context = context
-        class BazAdapter(object):
+
+        class BazAdapter:
             def __init__(self, context):
                 self.context = context
         gsm = getGlobalSiteManager()
         gsm.registerSubscriptionAdapter(BarAdapter, (None,), IFoo)
         gsm.registerSubscriptionAdapter(BazAdapter, (None,), IFoo)
         subscribers = self._callFUT((object(),), IFoo)
         self.assertEqual(len(subscribers), 2)
         names = [(x.__class__.__name__) for x in subscribers]
         self.assertTrue('BarAdapter' in names)
         self.assertTrue('BazAdapter' in names)
 
     def test_wo_sitemanager(self):
         from zope.interface import Interface
         from zope.interface.interfaces import ComponentLookupError
+
         class IFoo(Interface):
             pass
-        class Context(object):
+
+        class Context:
             def __conform__(self, iface):
                 raise ComponentLookupError
         subscribers = self._callFUT((object,), IFoo, context=Context())
         self.assertEqual(subscribers, [])
 
 
 class Test_handle(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import handle
         return handle(*args, **kw)
 
     def test_nonesuch(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
-        subscribers = self._callFUT((object,), IFoo) #doesn't raise
+        self._callFUT((object,), IFoo)  # doesn't raise
 
     def test_hit(self):
-        from zope.component import getGlobalSiteManager
         from zope.interface import Interface
         from zope.interface import implementer
+
+        from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         @implementer(IFoo)
-        class Foo(object):
+        class Foo:
             pass
         _called = []
+
         def _bar(context):
-                _called.append('_bar')
+            _called.append('_bar')
+
         def _baz(context):
-                _called.append('_baz')
+            _called.append('_baz')
         gsm = getGlobalSiteManager()
         gsm.registerHandler(_bar, (IFoo,))
         gsm.registerHandler(_baz, (IFoo,))
         self._callFUT(Foo())
         self.assertEqual(len(_called), 2, _called)
         self.assertTrue('_bar' in _called)
         self.assertTrue('_baz' in _called)
 
 
 class Test_getUtility(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component._api import getUtility
         return getUtility(*args, **kw)
 
     def test_anonymous_nonesuch(self):
         from zope.interface import Interface
         from zope.interface.interfaces import ComponentLookupError
+
         class IFoo(Interface):
             pass
         self.assertRaises(ComponentLookupError, self._callFUT, IFoo)
 
     def test_named_nonesuch(self):
         from zope.interface import Interface
         from zope.interface.interfaces import ComponentLookupError
+
         class IFoo(Interface):
             pass
         self.assertRaises(ComponentLookupError,
                           self._callFUT, IFoo, name='bar')
 
     def test_anonymous_hit(self):
         from zope.interface import Interface
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
         obj = object()
         getGlobalSiteManager().registerUtility(obj, IFoo)
         self.assertTrue(self._callFUT(IFoo) is obj)
 
     def test_named_hit(self):
         from zope.interface import Interface
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
         obj = object()
         getGlobalSiteManager().registerUtility(obj, IFoo, name='bar')
         self.assertTrue(self._callFUT(IFoo, name='bar') is obj)
 
     def test_w_conforming_context(self):
         from zope.interface import Interface
+
         from zope.component import getGlobalSiteManager
         from zope.component.tests.examples import ConformsToIComponentLookup
-        class SM(object):
+
+        class SM:
             def __init__(self, obj):
                 self._obj = obj
+
             def queryUtility(self, interface, name, default):
                 return self._obj
+
         class IFoo(Interface):
             pass
         obj1 = object()
         obj2 = object()
         sm = SM(obj2)
         context = ConformsToIComponentLookup(sm)
         getGlobalSiteManager().registerUtility(obj1, IFoo)
         self.assertTrue(self._callFUT(IFoo, context=context) is obj2)
 
 
 class Test_queryUtility(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component._api import queryUtility
         return queryUtility(*args, **kw)
 
     def test_anonymous_nonesuch(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         self.assertEqual(self._callFUT(IFoo), None)
 
     def test_anonymous_nonesuch_w_default(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         obj = object()
         self.assertTrue(self._callFUT(IFoo, default=obj) is obj)
 
     def test_named_nonesuch(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         self.assertEqual(self._callFUT(IFoo, name='bar'), None)
 
     def test_named_nonesuch_w_default(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         obj = object()
         self.assertTrue(self._callFUT(IFoo, name='bar', default=obj) is obj)
 
     def test_anonymous_hit(self):
         from zope.interface import Interface
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
         obj = object()
         getGlobalSiteManager().registerUtility(obj, IFoo)
         self.assertTrue(self._callFUT(IFoo) is obj)
 
     def test_named_hit(self):
         from zope.interface import Interface
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
         obj = object()
         getGlobalSiteManager().registerUtility(obj, IFoo, name='bar')
         self.assertTrue(self._callFUT(IFoo, name='bar') is obj)
 
     def test_w_conforming_context(self):
         from zope.interface import Interface
+
         from zope.component import getGlobalSiteManager
         from zope.component.tests.examples import ConformsToIComponentLookup
-        class SM(object):
+
+        class SM:
             def __init__(self, obj):
                 self._obj = obj
+
             def queryUtility(self, interface, name, default):
                 return self._obj
+
         class IFoo(Interface):
             pass
         obj1 = object()
         obj2 = object()
         sm = SM(obj2)
         context = ConformsToIComponentLookup(sm)
         getGlobalSiteManager().registerUtility(obj1, IFoo)
         self.assertTrue(self._callFUT(IFoo, context=context) is obj2)
 
 
 class Test_getUtilitiesFor(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component._api import getUtilitiesFor
         return getUtilitiesFor(*args, **kw)
 
     def test_nonesuch(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         self.assertEqual(list(self._callFUT(IFoo)), [])
 
     def test_hit(self):
         from zope.interface import Interface
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
         obj = object()
         obj1 = object()
         getGlobalSiteManager().registerUtility(obj, IFoo)
         getGlobalSiteManager().registerUtility(obj1, IFoo, name='bar')
         tuples = list(self._callFUT(IFoo))
         self.assertEqual(len(tuples), 2)
         self.assertTrue(('', obj) in tuples)
         self.assertTrue(('bar', obj1) in tuples)
 
 
 class Test_getAllUtilitiesRegisteredFor(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import getAllUtilitiesRegisteredFor
         return getAllUtilitiesRegisteredFor(*args, **kw)
 
     def test_nonesuch(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         self.assertEqual(list(self._callFUT(IFoo)), [])
 
     def test_hit(self):
         from zope.interface import Interface
+
         from zope.component import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(IFoo):
             pass
         obj = object()
         obj1 = object()
         obj2 = object()
         getGlobalSiteManager().registerUtility(obj, IFoo)
         getGlobalSiteManager().registerUtility(obj1, IFoo, name='bar')
@@ -943,15 +1112,16 @@
         self.assertTrue(obj in uts)
         self.assertTrue(obj1 in uts)
         self.assertTrue(obj2 in uts)
 
 
 class Test_getNextUtility(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import getNextUtility
         return getNextUtility(*args, **kw)
 
     def test_global(self):
         from zope.component import getGlobalSiteManager
@@ -959,17 +1129,18 @@
         gsm = getGlobalSiteManager()
         gutil = _makeMyUtility('global', gsm)
         gsm.registerUtility(gutil, IMyUtility, 'myutil')
         self.assertRaises(ComponentLookupError,
                           self._callFUT, gutil, IMyUtility, 'myutil')
 
     def test_nested(self):
-        from zope.component import getGlobalSiteManager
         from zope.interface.interfaces import IComponentLookup
         from zope.interface.registry import Components
+
+        from zope.component import getGlobalSiteManager
         gsm = getGlobalSiteManager()
         gutil = _makeMyUtility('global', gsm)
         gsm.registerUtility(gutil, IMyUtility, 'myutil')
         sm1 = Components('sm1', bases=(gsm, ))
         sm1_1 = Components('sm1_1', bases=(sm1, ))
         util1 = _makeMyUtility('one', sm1)
         sm1.registerUtility(util1, IMyUtility, 'myutil')
@@ -979,30 +1150,32 @@
         sm1_1.registerUtility(util1_1, IMyUtility, 'myutil')
         self.assertTrue(IComponentLookup(util1_1) is sm1_1)
         self.assertTrue(self._callFUT(util1_1, IMyUtility, 'myutil') is util1)
 
 
 class Test_queryNextUtility(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import queryNextUtility
         return queryNextUtility(*args, **kw)
 
     def test_global(self):
         from zope.component import getGlobalSiteManager
         gsm = getGlobalSiteManager()
         gutil = _makeMyUtility('global', gsm)
         gsm.registerUtility(gutil, IMyUtility, 'myutil')
         self.assertEqual(self._callFUT(gutil, IMyUtility, 'myutil'), None)
 
     def test_nested(self):
-        from zope.component import getGlobalSiteManager
         from zope.interface.registry import Components
+
+        from zope.component import getGlobalSiteManager
         gsm = getGlobalSiteManager()
         gutil = _makeMyUtility('global', gsm)
         gsm.registerUtility(gutil, IMyUtility, 'myutil')
         sm1 = Components('sm1', bases=(gsm, ))
         sm1_1 = Components('sm1_1', bases=(sm1, ))
         util1 = _makeMyUtility('one', sm1)
         sm1.registerUtility(util1, IMyUtility, 'myutil')
@@ -1010,159 +1183,188 @@
         sm1_1.registerUtility(util1_1, IMyUtility, 'myutil')
         myregistry = Components()
         custom_util = _makeMyUtility('my_custom_util', myregistry)
         myregistry.registerUtility(custom_util, IMyUtility, 'my_custom_util')
         sm1.__bases__ = (myregistry,) + sm1.__bases__
         # Both the ``myregistry`` and global utilities should be available:
         self.assertTrue(self._callFUT(sm1, IMyUtility, 'my_custom_util')
-                                            is custom_util)
+                        is custom_util)
         self.assertTrue(self._callFUT(sm1, IMyUtility, 'myutil') is gutil)
 
     def test_wo_sitemanager(self):
         from zope.interface import Interface
         from zope.interface.interfaces import ComponentLookupError
+
         class IFoo(Interface):
             pass
-        class Context(object):
+
+        class Context:
             def __conform__(self, iface):
                 raise ComponentLookupError
         self.assertEqual(self._callFUT(Context(), IFoo, 'myutil'), None)
 
 
 class Test_createObject(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import createObject
         return createObject(*args, **kw)
 
     def test_miss(self):
         from zope.interface.interfaces import ComponentLookupError
         self.assertRaises(ComponentLookupError, self._callFUT, 'nonesuch')
 
     def test_hit(self):
         from zope.component.interfaces import IFactory
         _object = object()
         _factory_called = []
+
         def _factory(*args, **kw):
             _factory_called.append((args, kw))
             return _object
-        class Context(object):
+
+        class Context:
             def __conform__(self, iface):
                 return self
+
             def queryUtility(self, iface, name, default, _test=self):
                 _test.assertIs(iface, IFactory)
                 _test.assertEqual(name, 'test')
                 return _factory
 
         context = Context()
         self.assertTrue(self._callFUT('test', context=context) is _object)
         self.assertEqual(_factory_called, [((), {})])
 
 
 class Test_getFactoryInterfaces(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import getFactoryInterfaces
         return getFactoryInterfaces(*args, **kw)
 
     def test_miss(self):
         from zope.interface.interfaces import ComponentLookupError
         self.assertRaises(ComponentLookupError, self._callFUT, 'nonesuch')
 
     def test_hit(self):
-        from zope.component.interfaces import IFactory
         from zope.interface import Interface
+
+        from zope.component.interfaces import IFactory
+
         class IFoo(Interface):
             pass
-        class _Factory(object):
+
+        class _Factory:
             def getInterfaces(self):
                 return [IFoo]
-        class Context(object):
+
+        class Context:
             def __conform__(self, iface):
                 return self
+
             def queryUtility(self, iface, name, default, _test=self):
                 _test.assertIs(iface, IFactory)
                 _test.assertEqual(name, 'test')
                 return _Factory()
 
         context = Context()
         self.assertEqual(self._callFUT('test', context=context), [IFoo])
 
 
 class Test_getFactoriesFor(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component import getFactoriesFor
         return getFactoriesFor(*args, **kw)
 
     def test_no_factories_registered(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         self.assertEqual(list(self._callFUT(IFoo)), [])
 
     def test_w_factory_returning_spec(self):
         from zope.interface import Interface
         from zope.interface import implementer
         from zope.interface import providedBy
+
         from zope.component.interfaces import IFactory
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @implementer(IFoo, IBar)
-        class _Factory(object):
+        class _Factory:
             def getInterfaces(self):
                 return providedBy(self)
         _factory = _Factory()
-        class Context(object):
+
+        class Context:
             def __conform__(self, iface):
                 return self
+
             def getUtilitiesFor(self, iface):
                 if iface is IFactory:
                     return [('test', _factory)]
         self.assertEqual(list(self._callFUT(IFoo, context=Context())),
                          [('test', _factory)])
         self.assertEqual(list(self._callFUT(IBar, context=Context())),
                          [('test', _factory)])
 
     def test_w_factory_returning_list_of_interfaces(self):
         from zope.interface import Interface
+
         from zope.component.interfaces import IFactory
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
-        class _Factory(object):
+
+        class _Factory:
             def getInterfaces(self):
                 return [IFoo, IBar]
         _factory = _Factory()
-        class Context(object):
+
+        class Context:
             def __conform__(self, iface):
                 return self
+
             def getUtilitiesFor(self, iface):
                 if iface is IFactory:
                     return [('test', _factory)]
         self.assertEqual(list(self._callFUT(IFoo, context=Context())),
                          [('test', _factory)])
         self.assertEqual(list(self._callFUT(IBar, context=Context())),
                          [('test', _factory)])
 
 
 IMyUtility = None
+
+
 def _makeMyUtility(name, sm):
     global IMyUtility
     from zope.interface import Interface
     from zope.interface import implementer
+
     from zope.component.tests.examples import ConformsToIComponentLookup
 
     if IMyUtility is None:
         class IMyUtility(Interface):
             pass
 
     @implementer(IMyUtility)
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test__declaration.py` & `zope.component-6.0/src/zope/component/tests/test__declaration.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test adapter declaration helpers
 """
 import unittest
 
+
 class Test_adapter(unittest.TestCase):
 
     def _getTargetClass(self):
         from zope.component._declaration import adapter
         return adapter
 
     def _makeOne(self, *interfaces):
@@ -26,130 +27,151 @@
 
     def test_ctor_no_interfaces(self):
         deco = self._makeOne()
         self.assertEqual(list(deco.interfaces), [])
 
     def test_ctor_w_interfaces(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
         deco = self._makeOne(IFoo, IBar)
         self.assertEqual(list(deco.interfaces), [IFoo, IBar])
 
     def test__call___w_class(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @self._makeOne(IFoo, IBar)
-        class Baz(object):
+        class Baz:
             pass
         self.assertEqual(Baz.__component_adapts__, (IFoo, IBar))
 
     def test__call___w_inst_of_decorated_class(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @self._makeOne(IFoo, IBar)
-        class Baz(object):
+        class Baz:
             pass
         baz = Baz()
         self.assertRaises(AttributeError,
                           getattr, baz, '__component_adapts_')
 
     def test__call___w_non_class(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
-        class Baz(object):
+
+        class Baz:
             pass
         deco = self._makeOne(IFoo, IBar)
         baz = deco(Baz())
         self.assertEqual(baz.__component_adapts__, (IFoo, IBar))
 
 
 class Test_adapts(unittest.TestCase):
 
     def _run_generated_code(self, code, globs, locs):
         import warnings
         with warnings.catch_warnings(record=True) as log:
             warnings.resetwarnings()
             exec(code, globs, locs)
-            self.assertEqual(len(log), 0) # no longer warn
+            self.assertEqual(len(log), 0)  # no longer warn
             return True
 
     def test_instances_not_affected(self):
         from zope.component._declaration import adapts
-        class C(object):
+
+        class C:
             adapts()
 
         self.assertEqual(C.__component_adapts__, ())
+
         def _try():
             return C().__component_adapts__
         self.assertRaises(AttributeError, _try)
 
     def test_called_from_function(self):
         import warnings
-        from zope.component._declaration import adapts
+
         from zope.interface import Interface
+
+        from zope.component._declaration import adapts
+
         class IFoo(Interface):
             pass
         globs = {'adapts': adapts, 'IFoo': IFoo}
         locs = {}
         CODE = "\n".join([
             'def foo():',
             '    adapts(IFoo)'
-            ])
+        ])
         self._run_generated_code(CODE, globs, locs)
         foo = locs['foo']
         with warnings.catch_warnings(record=True) as log:
             warnings.resetwarnings()
             self.assertRaises(TypeError, foo)
-            self.assertEqual(len(log), 0) # no longer warn
+            self.assertEqual(len(log), 0)  # no longer warn
 
     def test_called_twice_from_class(self):
         import warnings
-        from zope.component._declaration import adapts
+
         from zope.interface import Interface
-        from zope.interface._compat import PYTHON3
+
+        from zope.component._declaration import adapts
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
         globs = {'adapts': adapts, 'IFoo': IFoo, 'IBar': IBar}
         locs = {}
         CODE = "\n".join([
             'class Foo(object):',
             '    adapts(IFoo)',
             '    adapts(IBar)',
-            ])
+        ])
         with warnings.catch_warnings(record=True) as log:
             warnings.resetwarnings()
             with self.assertRaises(TypeError):
                 exec(CODE, globs, locs)
-            self.assertEqual(len(log), 0) # no longer warn
+            self.assertEqual(len(log), 0)  # no longer warn
 
     def test_called_once_from_class(self):
-        from zope.component._declaration import adapts
         from zope.interface import Interface
+
+        from zope.component._declaration import adapts
+
         class IFoo(Interface):
             pass
         globs = {'adapts': adapts, 'IFoo': IFoo}
         locs = {}
         CODE = "\n".join([
             'class Foo(object):',
             '    adapts(IFoo)',
-            ])
+        ])
         self._run_generated_code(CODE, globs, locs)
         Foo = locs['Foo']
         spec = Foo.__component_adapts__
         self.assertEqual(list(spec), [IFoo])
 
 
 class Test_adaptedBy(unittest.TestCase):
@@ -159,38 +181,48 @@
         return adaptedBy(obj)
 
     def test_obj_w_no_attr(self):
         self.assertEqual(self._callFUT(object()), None)
 
     def test__call___w_class(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
-        class Baz(object):
+
+        class Baz:
             __component_adapts__ = (IFoo, IBar)
         self.assertEqual(self._callFUT(Baz), (IFoo, IBar))
 
     def test__call___w_inst_of_decorated_class(self):
         from zope.interface import Interface
+
         from zope.component._declaration import _adapts_descr
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
-        class Baz(object):
+
+        class Baz:
             __component_adapts__ = _adapts_descr((IFoo, IBar))
         baz = Baz()
         self.assertEqual(self._callFUT(baz), None)
 
     def test__call___w_non_class(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
-        class Baz(object):
+
+        class Baz:
             pass
         baz = Baz()
         baz.__component_adapts__ = (IFoo, IBar)
         self.assertEqual(self._callFUT(baz), (IFoo, IBar))
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test_event.py` & `zope.component-6.0/src/zope/component/tests/test_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,47 +11,54 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test adapter declaration helpers
 """
 import unittest
 
+
 class Test_dispatch(unittest.TestCase):
 
     def test_it(self):
         from zope.interface import Interface
-        from zope.component.globalregistry import getGlobalSiteManager
+
         from zope.component.event import dispatch
+        from zope.component.globalregistry import getGlobalSiteManager
         _adapted = []
+
         def _adapter(context):
             _adapted.append(context)
             return object()
         gsm = getGlobalSiteManager()
         gsm.registerHandler(_adapter, (Interface,))
-        del _adapted[:] # clear handler reg
+        del _adapted[:]  # clear handler reg
         event = object()
         dispatch(event)
         self.assertEqual(_adapted, [event])
 
+
 class Test_objectEventNotify(unittest.TestCase):
 
     def test_it(self):
         from zope.interface import Interface
         from zope.interface import implementer
-        from zope.component.globalregistry import getGlobalSiteManager
         from zope.interface.interfaces import IObjectEvent
+
         from zope.component.event import objectEventNotify
+        from zope.component.globalregistry import getGlobalSiteManager
         _adapted = []
+
         def _adapter(context, event):
             _adapted.append((context, event))
             return object()
         gsm = getGlobalSiteManager()
         gsm.registerHandler(_adapter, (Interface, IObjectEvent))
-        del _adapted[:] # clear handler reg
+        del _adapted[:]  # clear handler reg
+
         @implementer(IObjectEvent)
-        class _ObjectEvent(object):
+        class _ObjectEvent:
             def __init__(self, object):
                 self.object = object
         context = object()
         event = _ObjectEvent(context)
         objectEventNotify(event)
         self.assertEqual(_adapted, [(context, event)])
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test_factory.py` & `zope.component-6.0/src/zope/component/tests/test_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,32 +13,35 @@
 ##############################################################################
 """Tests for z.c.factory
 """
 import unittest
 
 from zope.component.tests import fails_if_called
 
+
 class FactoryTests(unittest.TestCase):
 
     def _getTargetClass(self):
         from zope.component.factory import Factory
         return Factory
 
     def _makeOne(self, callable=None, *args, **kw):
         if callable is None:
             callable = fails_if_called(self)
         return self._getTargetClass()(callable, *args, **kw)
 
     def test_class_conforms_to_IFactory(self):
         from zope.interface.verify import verifyClass
+
         from zope.component.interfaces import IFactory
         verifyClass(IFactory, self._getTargetClass())
 
     def test_instance_conforms_to_IFactory(self):
         from zope.interface.verify import verifyObject
+
         from zope.component.interfaces import IFactory
         verifyObject(IFactory, self._makeOne())
 
     def test_ctor_defaults(self):
         func = fails_if_called(self)
         factory = self._makeOne(func)
         self.assertEqual(factory._callable, func)
@@ -49,55 +52,62 @@
     def test_ctor_expclit(self):
         factory = self._makeOne(fails_if_called(self), 'TITLE', 'DESCRIPTION')
         self.assertEqual(factory.title, 'TITLE')
         self.assertEqual(factory.description, 'DESCRIPTION')
 
     def test___call___no_args(self):
         _called = []
+
         def _callable(*args, **kw):
             _called.append((args, kw))
         factory = self._makeOne(_callable)
         factory()
         self.assertEqual(_called, [((), {})])
 
     def test___call___positional_args(self):
         _called = []
+
         def _callable(*args, **kw):
             _called.append((args, kw))
         factory = self._makeOne(_callable)
         factory('one', 'two')
         self.assertEqual(_called, [(('one', 'two'), {})])
 
     def test___call___keyword_args(self):
         _called = []
+
         def _callable(*args, **kw):
             _called.append((args, kw))
         factory = self._makeOne(_callable)
         factory(foo='bar')
         self.assertEqual(_called, [((), {'foo': 'bar'})])
 
     def test_getInterfaces_explicit(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         class IBaz(Interface):
             pass
         _callable = fails_if_called(self)
         _callable.__name__ = '_callable'
         _callable = implementer(IBaz)(_callable)
         factory = self._makeOne(_callable, interfaces=(IFoo, IBar))
         spec = factory.getInterfaces()
         self.assertEqual(spec.__name__, '_callable')
         self.assertEqual(list(spec), [IFoo, IBar])
 
     def test_getInterfaces_implicit(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         class IBaz(Interface):
             pass
         _callable = implementer(IBaz)(fails_if_called(self))
         factory = self._makeOne(_callable)
         spec = factory.getInterfaces()
         self.assertEqual(list(spec), [IBaz])
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test_globalregistry.py` & `zope.component-6.0/src/zope/component/tests/test_globalregistry.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,230 +13,267 @@
 ##############################################################################
 """ Tests for z.c._api
 """
 import unittest
 
 from zope.component.tests import fails_if_called
 
+
 class Test_getGlobalSiteManager(unittest.TestCase):
 
     def _callFUT(self):
         from zope.component.globalregistry import getGlobalSiteManager
         return getGlobalSiteManager()
 
     def test_gsm_is_IComponentLookup(self):
-        from zope.component.globalregistry import base
         from zope.interface.interfaces import IComponentLookup
+
+        from zope.component.globalregistry import base
         gsm = self._callFUT()
         self.assertTrue(gsm is base)
         self.assertTrue(IComponentLookup.providedBy(gsm))
 
     def test_gsm_is_singleton(self):
         gsm = self._callFUT()
         self.assertTrue(self._callFUT() is gsm)
 
     def test_gsm_pickling(self):
-        from zope.component._compat import _pickle
+        import pickle
         gsm = self._callFUT()
-        dumped = _pickle.dumps(gsm)
-        loaded = _pickle.loads(dumped)
+        dumped = pickle.dumps(gsm)
+        loaded = pickle.loads(dumped)
         self.assertTrue(loaded is gsm)
 
-        dumped_utilities = _pickle.dumps(gsm.utilities)
-        loaded_utilities = _pickle.loads(dumped_utilities)
+        dumped_utilities = pickle.dumps(gsm.utilities)
+        loaded_utilities = pickle.loads(dumped_utilities)
         self.assertTrue(loaded_utilities is gsm.utilities)
 
-        dumped_adapters = _pickle.dumps(gsm.adapters)
-        loaded_adapters = _pickle.loads(dumped_adapters)
+        dumped_adapters = pickle.dumps(gsm.adapters)
+        loaded_adapters = pickle.loads(dumped_adapters)
         self.assertTrue(loaded_adapters is gsm.adapters)
 
 
 class Test_provideUtility(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.globalregistry import provideUtility
         return provideUtility(*args, **kw)
 
     def test_anonymous_no_provides(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component.globalregistry import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         @implementer(IFoo)
-        class Foo(object):
+        class Foo:
             pass
         foo = Foo()
         self._callFUT(foo)
         gsm = getGlobalSiteManager()
         self.assertIs(gsm.getUtility(IFoo, ''), foo)
 
         # We can clean it up using the fallback and it will be gone
         from zope.component.testing import _PlacelessSetupFallback
         _PlacelessSetupFallback().cleanUp()
         self.assertIsNone(gsm.queryUtility(IFoo, ''))
 
     def test_named_w_provides(self):
         from zope.interface import Interface
+
         from zope.component.globalregistry import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
         foo = Foo()
         self._callFUT(foo, IFoo, 'named')
         gsm = getGlobalSiteManager()
         self.assertTrue(gsm.getUtility(IFoo, 'named') is foo)
 
 
 class Test_provideAdapter(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.globalregistry import provideAdapter
         return provideAdapter(*args, **kw)
 
     def test_anonymous_no_provides_no_adapts(self):
         from zope.interface import Interface
         from zope.interface import implementer
-        from zope.component.globalregistry import getGlobalSiteManager
+
         from zope.component._declaration import adapter
+        from zope.component.globalregistry import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @implementer(IFoo)
-        class Foo(object):
+        class Foo:
             pass
+
         @adapter(IFoo)
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             def __init__(self, context):
                 self.context = context
         self._callFUT(Bar)
         gsm = getGlobalSiteManager()
         foo = Foo()
         adapted = gsm.getAdapter(foo, IBar)
         self.assertTrue(isinstance(adapted, Bar))
         self.assertTrue(adapted.context is foo)
 
     def test_named_w_provides_w_adapts(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component.globalregistry import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @implementer(IFoo)
-        class Foo(object):
+        class Foo:
             pass
-        class Bar(object):
+
+        class Bar:
             def __init__(self, context):
                 self.context = context
         self._callFUT(Bar, (IFoo,), IBar, 'test')
         gsm = getGlobalSiteManager()
         foo = Foo()
         adapted = gsm.getAdapter(foo, IBar, name='test')
         self.assertTrue(isinstance(adapted, Bar))
         self.assertTrue(adapted.context is foo)
 
 
 class Test_provideSubscriptionAdapter(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.globalregistry import provideSubscriptionAdapter
         return provideSubscriptionAdapter(*args, **kw)
 
     def test_no_provides_no_adapts(self):
         from zope.interface import Interface
         from zope.interface import implementer
-        from zope.component.globalregistry import getGlobalSiteManager
+
         from zope.component._declaration import adapter
+        from zope.component.globalregistry import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @implementer(IFoo)
-        class Foo(object):
+        class Foo:
             pass
+
         @adapter(IFoo)
         @implementer(IBar)
-        class Bar(object):
+        class Bar:
             def __init__(self, context):
                 self.context = context
         self._callFUT(Bar)
         gsm = getGlobalSiteManager()
         foo = Foo()
         adapted = gsm.subscribers((foo,), IBar)
         self.assertEqual(len(adapted), 1)
         self.assertTrue(isinstance(adapted[0], Bar))
         self.assertTrue(adapted[0].context is foo)
 
     def test_w_provides_w_adapts(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component.globalregistry import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
+
         @implementer(IFoo)
-        class Foo(object):
+        class Foo:
             pass
-        class Bar(object):
+
+        class Bar:
             def __init__(self, context):
                 self.context = context
         self._callFUT(Bar, (IFoo,), IBar)
         gsm = getGlobalSiteManager()
         foo = Foo()
         adapted = gsm.subscribers((foo,), IBar)
         self.assertEqual(len(adapted), 1)
         self.assertTrue(isinstance(adapted[0], Bar))
         self.assertTrue(adapted[0].context is foo)
 
 
 class Test_provideHandler(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.globalregistry import provideHandler
         return provideHandler(*args, **kw)
 
     def test_no_adapts(self):
         from zope.interface import Interface
         from zope.interface import implementer
         from zope.interface import providedBy
-        from zope.component.globalregistry import getGlobalSiteManager
+
         from zope.component._declaration import adapter
+        from zope.component.globalregistry import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
+
         @implementer(IFoo)
-        class Foo(object):
+        class Foo:
             pass
         _handler = adapter(IFoo)(fails_if_called(self))
 
         self._callFUT(_handler)
         gsm = getGlobalSiteManager()
         regs = list(gsm.registeredHandlers())
         self.assertEqual(len(regs), 1)
         hr = regs[0]
         self.assertEqual(list(hr.required), list(providedBy(Foo())))
         self.assertEqual(hr.name, '')
         self.assertTrue(hr.factory is _handler)
 
     def test_w_adapts(self):
         from zope.interface import Interface
+
         from zope.component.globalregistry import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
         _handler = fails_if_called(self)
         self._callFUT(_handler, (IFoo,))
         gsm = getGlobalSiteManager()
         regs = list(gsm.registeredHandlers())
         self.assertEqual(len(regs), 1)
@@ -244,24 +281,25 @@
         self.assertEqual(list(hr.required), [IFoo])
         self.assertEqual(hr.name, '')
         self.assertTrue(hr.factory is _handler)
 
 
 class TestBaseGlobalComponents(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _getTargetClass(self):
         from zope.component.globalregistry import BaseGlobalComponents
         return BaseGlobalComponents
 
     def _getTargetInterfaces(self):
         from zope.interface.interfaces import IComponentLookup
-        from zope.interface.interfaces import IComponents
         from zope.interface.interfaces import IComponentRegistry
+        from zope.interface.interfaces import IComponents
         return [IComponents, IComponentLookup, IComponentRegistry]
 
     def _makeOne(self):
         return self._getTargetClass()()
 
     def test_verifyInstance(self):
         from zope.interface.verify import verifyObject
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test_hooks.py` & `zope.component-6.0/src/zope/component/tests/test_hooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,27 +19,27 @@
 class Test_read_property(unittest.TestCase):
 
     def _getTargetClass(self):
         from zope.component.hooks import read_property
         return read_property
 
     def test_via_instance(self):
-        class Foo(object):
+        class Foo:
             @self._getTargetClass()
             def bar(self):
                 return 'BAR'
         foo = Foo()
         self.assertEqual(foo.bar, 'BAR')
         foo.bar = 'BAZ'
         self.assertEqual(foo.bar, 'BAZ')
         del foo.bar
         self.assertEqual(foo.bar, 'BAR')
 
     def test_via_class(self):
-        class Foo(object):
+        class Foo:
             @self._getTargetClass()
             def bar(self):
                 return 'BAR'
         bar = Foo.bar
         self.assertTrue(isinstance(bar, self._getTargetClass()))
         self.assertEqual(bar.func(object()), 'BAR')
 
@@ -58,17 +58,19 @@
         gsm = getGlobalSiteManager()
         si = self._makeOne()
         self.assertEqual(si.site, None)
         self.assertTrue(si.sm is gsm)
 
     def test_adapter_hook(self):
         _hook = object()
-        class _Registry(object):
+
+        class _Registry:
             adapter_hook = _hook
-        class _SiteManager(object):
+
+        class _SiteManager:
             adapters = _Registry()
         si = self._makeOne()
         si.sm = _SiteManager()
         self.assertFalse('adapter_hook' in si.__dict__)
         self.assertTrue(si.adapter_hook is _hook)
         self.assertTrue('adapter_hook' in si.__dict__)
         del si.adapter_hook
@@ -97,15 +99,16 @@
         self.assertTrue(siteinfo.sm is gsm)
         self.assertTrue(siteinfo.site is None)
         self.assertFalse('adapter_hook' in siteinfo.__dict__)
 
     def test_w_site(self):
         from zope.component import hooks
         _SM2 = object()
-        class _Site(object):
+
+        class _Site:
             def getSiteManager(self):
                 return _SM2
         siteinfo = _DummySiteInfo()
         _site = _Site()
         with _Monkey(hooks, siteinfo=siteinfo):
             self._callFUT(_site)
         self.assertTrue(siteinfo.sm is _SM2)
@@ -117,24 +120,20 @@
 
     def _callFUT(self):
         from zope.component.hooks import getSite
         return getSite()
 
     def test_w_None(self):
         from zope.component import hooks
-        from zope.component.globalregistry import getGlobalSiteManager
-        gsm = getGlobalSiteManager()
         siteinfo = _DummySiteInfo()
         with _Monkey(hooks, siteinfo=siteinfo):
             self.assertTrue(self._callFUT() is None)
 
     def test_w_site(self):
         from zope.component import hooks
-        from zope.component.globalregistry import getGlobalSiteManager
-        gsm = getGlobalSiteManager()
         _SM2 = object()
         _SITE = object()
         siteinfo = _DummySiteInfo()
         siteinfo.sm = _SM2
         siteinfo.site = _SITE
         with _Monkey(hooks, siteinfo=siteinfo):
             self.assertTrue(self._callFUT() is _SITE)
@@ -147,15 +146,16 @@
         return site(new_site)
 
     def test_it(self):
         from zope.component import hooks
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
         _SM2 = object()
-        class _Site(object):
+
+        class _Site:
             def getSiteManager(self):
                 return _SM2
         _site = _Site()
         siteinfo = _DummySiteInfo()
         self.assertTrue(siteinfo.site is None)
         self.assertTrue(siteinfo.sm is _SM)
         with _Monkey(hooks, siteinfo=siteinfo):
@@ -170,16 +170,14 @@
 
     def _callFUT(self, context=None):
         from zope.component.hooks import getSiteManager
         return getSiteManager(context)
 
     def test_default(self):
         from zope.component import hooks
-        from zope.component.globalregistry import getGlobalSiteManager
-        gsm = getGlobalSiteManager()
         _SM2 = object()
         siteinfo = _DummySiteInfo()
         siteinfo.sm = _SM2
         with _Monkey(hooks, siteinfo=siteinfo):
             self.assertTrue(self._callFUT() is _SM2)
 
     def test_w_explicit_context_no_IComponentLookup(self):
@@ -190,18 +188,20 @@
         siteinfo = _DummySiteInfo()
         siteinfo.sm = _SM2
         with _Monkey(hooks, siteinfo=siteinfo):
             self.assertTrue(self._callFUT(object()) is gsm)
 
     def test_w_explicit_context_w_IComponentLookup(self):
         from zope.interface import Interface
+        from zope.interface.interfaces import IComponentLookup
+
         from zope.component import hooks
         from zope.component.globalregistry import getGlobalSiteManager
-        from zope.interface.interfaces import IComponentLookup
-        class _Lookup(object):
+
+        class _Lookup:
             def __init__(self, context):
                 self.context = context
         gsm = getGlobalSiteManager()
         gsm.registerAdapter(_Lookup, (Interface,), IComponentLookup, '')
         _SM2 = object()
         siteinfo = _DummySiteInfo()
         siteinfo.sm = _SM2
@@ -216,44 +216,46 @@
 
     def _callFUT(self, interface, object, name='', default=None):
         from zope.component.hooks import adapter_hook
         return adapter_hook(interface, object, name, default)
 
     def test_success(self):
         from zope.interface import Interface
+
         from zope.component import hooks
-        from zope.component.globalregistry import getGlobalSiteManager
+
         class IFoo(Interface):
             pass
-        gsm = getGlobalSiteManager()
         _ADAPTER = object()
         _DEFAULT = object()
         _CONTEXT = object()
         _called = []
+
         def _adapter_hook(interface, object, name, default):
             _called.append((interface, object, name, default))
             return _ADAPTER
         siteinfo = _DummySiteInfo()
         siteinfo.adapter_hook = _adapter_hook
         with _Monkey(hooks, siteinfo=siteinfo):
             adapter = self._callFUT(IFoo, _CONTEXT, 'bar', _DEFAULT)
         self.assertTrue(adapter is _ADAPTER)
         self.assertEqual(_called, [(IFoo, _CONTEXT, 'bar', _DEFAULT)])
 
     def test_hook_raises(self):
         from zope.interface import Interface
-        from zope.component import hooks
-        from zope.component.globalregistry import getGlobalSiteManager
         from zope.interface.interfaces import ComponentLookupError
+
+        from zope.component import hooks
+
         class IFoo(Interface):
             pass
-        gsm = getGlobalSiteManager()
         _DEFAULT = object()
         _CONTEXT = object()
         _called = []
+
         def _adapter_hook(interface, object, name, default):
             _called.append((interface, object, name, default))
             raise ComponentLookupError('testing')
         siteinfo = _DummySiteInfo()
         siteinfo.adapter_hook = _adapter_hook
         with _Monkey(hooks, siteinfo=siteinfo):
             adapter = self._callFUT(IFoo, _CONTEXT, 'bar', _DEFAULT)
@@ -266,17 +268,19 @@
     def _callFUT(self):
         from zope.component.hooks import setHooks
         return setHooks()
 
     def test_it(self):
         import zope.component._api
         from zope.component import hooks
-        class _Hook(object):
+
+        class _Hook:
             def __init__(self):
                 self._hooked = None
+
             def sethook(self, value):
                 self._hooked = value
         adapter_hook = _Hook()
         getSiteManager = _Hook()
         with _Monkey(zope.component._api,
                      adapter_hook=adapter_hook,
                      getSiteManager=getSiteManager):
@@ -290,17 +294,19 @@
     def _callFUT(self):
         from zope.component.hooks import resetHooks
         return resetHooks()
 
     def test_it(self):
         import zope.component._api
         from zope.component import hooks
-        class _Hook(object):
+
+        class _Hook:
             def __init__(self):
                 self._reset = False
+
             def reset(self):
                 self._reset = True
         adapter_hook = _Hook()
         getSiteManager = _Hook()
         with _Monkey(zope.component._api,
                      adapter_hook=adapter_hook,
                      getSiteManager=getSiteManager):
@@ -314,23 +320,26 @@
         self.assertTrue(adapter_hook._reset)
         self.assertTrue(getSiteManager._reset)
         # adapter_hook cache also reset
         self.assertFalse('adapter_hook' in hooks.siteinfo.__dict__)
 
 
 _SM = object()
-class _DummySiteInfo(object):
+
+
+class _DummySiteInfo:
     sm = _SM
     site = None
 
-class _Monkey(object):
+
+class _Monkey:
     # context-manager for replacing module names in the scope of a test.
     def __init__(self, module, **kw):
         self.module = module
-        self.to_restore = dict([(key, getattr(module, key)) for key in kw])
+        self.to_restore = {key: getattr(module, key) for key in kw}
         for key, value in kw.items():
             setattr(module, key, value)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test_interface.py` & `zope.component-6.0/src/zope/component/tests/test_interface.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,221 +13,248 @@
 ##############################################################################
 """Tests for z.c.interface
 """
 import os
 import unittest
 
 
-DOCSTRINGS_REMOVED = False
-if os.environ.get('PYTHONOPTIMIZE') == '2':
-    DOCSTRINGS_REMOVED = True
+DOCSTRINGS_REMOVED = os.environ.get('PYTHONOPTIMIZE') == '2'
 
 # pylint:disable=inherit-non-class,blacklisted-name
 
+
 class Test_provideInterface(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.interface import provideInterface
         return provideInterface(*args, **kw)
 
     def test_w_interface_not_IInterface(self):
         self.assertRaises(TypeError, self._callFUT, 'xxx', object())
 
     def test_w_iface_type_not_IInterface(self):
         from zope.interface import Interface
         from zope.interface.interface import InterfaceClass
+
         class IFoo(Interface):
             pass
         IBar = InterfaceClass('IBar')
         self.assertRaises(TypeError, self._callFUT, 'xxx', IFoo, IBar)
 
     def test_w_class(self):
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IBar(IInterface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
         self._callFUT('', Foo, IBar)
         self.assertFalse(IBar.providedBy(Foo))
         self.assertEqual(len(list(gsm.getUtilitiesFor(IBar))), 0)
 
     def test_wo_name_w_iface_type(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IFoo(Interface):
             pass
+
         class IBar(IInterface):
             pass
         self._callFUT('', IFoo, IBar)
         self.assertTrue(IBar.providedBy(IFoo))
         nm = 'zope.component.tests.test_interface.IFoo'
         self.assertTrue(gsm.getUtility(IBar, nm) is IFoo)
 
     def test_w_name_wo_ifact_type(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IFoo(Interface):
             pass
         self._callFUT('foo', IFoo)
         self.assertTrue(IInterface.providedBy(IFoo))
         registered = gsm.getUtility(IInterface, name='foo')
         self.assertIs(registered, IFoo)
 
     def test_register_in_current_site(self):
-        from zope.component._api import getSiteManager
-        from zope.component.globalregistry import getGlobalSiteManager
-        from zope.interface.registry import Components
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+        from zope.interface.registry import Components
+
+        from zope.component._api import getSiteManager
+        from zope.component.globalregistry import getGlobalSiteManager
 
         class IFoo(Interface):
             pass
 
         site_man = Components()
+
         def get(_context=None):
             return site_man
         getSiteManager.sethook(get)
         self.addCleanup(getSiteManager.reset)
 
         self._callFUT('foo', IFoo)
 
         self.assertIs(site_man.getUtility(IInterface, name='foo'),
                       IFoo)
         self.assertIsNone(
             getGlobalSiteManager().queryUtility(IInterface, name='foo')
         )
 
 
-
 class Test_getInterface(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.interface import getInterface
         return getInterface(*args, **kw)
 
     def test_miss(self):
         from zope.interface.interfaces import ComponentLookupError
         self.assertRaises(ComponentLookupError,
                           self._callFUT, object(), 'nonesuch')
 
     def test_hit(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IFoo(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         self.assertTrue(self._callFUT(object(), 'foo') is IFoo)
 
 
 class Test_queryInterface(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.interface import queryInterface
         return queryInterface(*args, **kw)
 
     def test_miss(self):
         _DEFAULT = object()
         self.assertTrue(
             self._callFUT('nonesuch', default=_DEFAULT) is _DEFAULT)
 
     def test_hit(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IFoo(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         self.assertTrue(self._callFUT('foo') is IFoo)
 
 
 class Test_searchInterface(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.interface import searchInterface
         return searchInterface(*args, **kw)
 
     def test_empty(self):
         self.assertEqual(self._callFUT(object()), [])
 
     def test_no_search_string_no_base(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IFoo(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         self.assertEqual(self._callFUT(object()), [IFoo])
 
     def test_w_search_string_no_base(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         gsm.registerUtility(IBar, IInterface, 'bar')
         self.assertEqual(self._callFUT(object(), 'IFoo'), [IFoo])
 
     def test_no_search_string_w_base(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IBase(Interface):
             pass
+
         class IFoo(IBase):
             pass
+
         class IBar(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         gsm.registerUtility(IBar, IInterface, 'bar')
         self.assertEqual(self._callFUT(object(), base=IBase), [IFoo])
 
     def test_hit_in_current_site(self):
-        from zope.component._api import getSiteManager
-        from zope.component.globalregistry import getGlobalSiteManager
-        from zope.interface.registry import Components
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+        from zope.interface.registry import Components
+
+        from zope.component._api import getSiteManager
+        from zope.component.globalregistry import getGlobalSiteManager
 
         class ILocal(Interface):
             pass
 
         class IGlobal(Interface):
             pass
 
         gsm = getGlobalSiteManager()
         site_man = Components(bases=(gsm,))
+
         def get(_context=None):
             return site_man
         getSiteManager.sethook(get)
         self.addCleanup(getSiteManager.reset)
 
-
         gsm.registerUtility(IGlobal, IInterface, 'foo')
         site_man.registerUtility(ILocal, IInterface, 'bar')
 
         result = self._callFUT(None)
         self.assertEqual(len(result), 2)
         self.assertIn(ILocal, result)
         self.assertIn(IGlobal, result)
@@ -237,118 +264,141 @@
         result = self._callFUT(None)
         self.assertEqual(len(result), 1)
         self.assertIn(IGlobal, result)
 
 
 class Test_searchInterfaceIds(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.interface import searchInterfaceIds
         return searchInterfaceIds(*args, **kw)
 
     def test_empty(self):
         self.assertEqual(self._callFUT(object()), [])
 
     def test_no_search_string_no_base(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IFoo(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         self.assertEqual(self._callFUT(object()), ['foo'])
 
     def test_w_search_string_no_base(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         gsm.registerUtility(IBar, IInterface, 'bar')
         self.assertEqual(self._callFUT(object(), 'IFoo'), ['foo'])
 
     def test_no_search_string_w_base(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IBase(Interface):
             pass
+
         class IFoo(IBase):
             pass
+
         class IBar(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         gsm.registerUtility(IBar, IInterface, 'bar')
         self.assertEqual(self._callFUT(object(), base=IBase), ['foo'])
 
 
 class Test_searchInterfaceUtilities(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.interface import searchInterfaceUtilities
         return searchInterfaceUtilities(*args, **kw)
 
     def test_empty(self):
         self.assertEqual(self._callFUT(object()), [])
 
     def test_no_search_string_no_base(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IFoo(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         self.assertEqual(self._callFUT(object()), [('foo', IFoo)])
 
     def test_w_search_string_no_base(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         gsm.registerUtility(IBar, IInterface, 'bar')
         self.assertEqual(self._callFUT(object(), 'IFoo'), [('foo', IFoo)])
 
     def test_no_search_string_w_base(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IBase(Interface):
             pass
+
         class IFoo(IBase):
             pass
+
         class IBar(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         gsm.registerUtility(IBar, IInterface, 'bar')
         self.assertEqual(self._callFUT(object(), base=IBase), [('foo', IFoo)])
 
     def test_no_search_string_w_base_is_same(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         gsm.registerUtility(IBar, IInterface, 'bar')
         self.assertEqual(self._callFUT(object(), base=IFoo), [('foo', IFoo)])
 
 
@@ -357,49 +407,54 @@
 class Test_getInterfaceAllDocs(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.component.interface import getInterfaceAllDocs
         return getInterfaceAllDocs(*args, **kw)
 
     def test_w_class(self):
-        class Foo(object):
+        class Foo:
             """DOCSTRING"""
             bar = None
+
             def baz(self):
                 """BAZ"""
         self.assertEqual(self._callFUT(Foo),
                          'zope.component.tests.test_interface.foo\n' +
                          'docstring')
 
     def test_w_interface_no_members(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             """DOCSTRING"""
         self.assertEqual(self._callFUT(IFoo),
                          'zope.component.tests.test_interface.ifoo\n' +
                          'docstring')
 
     def test_w_interface_w_members(self):
         from zope.interface import Attribute
         from zope.interface import Interface
+
         class IFoo(Interface):
             """DOCSTRING"""
             bar = Attribute('bar', 'Do bar')
+
             def baz(self):
                 """BAZ"""
         self.assertEqual(self._callFUT(IFoo),
                          'zope.component.tests.test_interface.ifoo\n' +
                          'docstring\n' +
                          'do bar\n' +
                          'baz')
 
 
 class Test_nameToInterface(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.interface import nameToInterface
         return nameToInterface(*args, **kw)
 
     def test_w_None(self):
         self.assertTrue(self._callFUT(object(), 'None') is None)
@@ -408,44 +463,50 @@
         from zope.interface.interfaces import ComponentLookupError
         self.assertRaises(ComponentLookupError,
                           self._callFUT, object(), 'nonesuch')
 
     def test_hit(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IFoo(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         found = self._callFUT(object(), 'foo')
         self.assertTrue(found is IFoo)
 
 
 class Test_interfaceToName(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.interface import interfaceToName
         return interfaceToName(*args, **kw)
 
     def test_w_None(self):
         self.assertEqual(self._callFUT(object(), None), 'None')
 
     def test_w_unregistered(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         self.assertEqual(self._callFUT(object(), IFoo),
                          'zope.component.tests.test_interface.IFoo')
 
     def test_w_registered(self):
         from zope.interface import Interface
         from zope.interface.interfaces import IInterface
+
         from zope.component.globalregistry import getGlobalSiteManager
         gsm = getGlobalSiteManager()
+
         class IFoo(Interface):
             pass
         gsm.registerUtility(IFoo, IInterface, 'foo')
         self.assertEqual(self._callFUT(object(), IFoo),
                          'zope.component.tests.test_interface.IFoo')
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test_interfaces.py` & `zope.component-6.0/src/zope/component/tests/test_interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 ##############################################################################
 """
 Tests for zope.component.interfaces
 """
 
 import unittest
 
+
 class TestInterfaces(unittest.TestCase):
 
     def test_nothing(self):
         """
         This exists only so that zope.testrunner doesn't complain this
         module has no tests.
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test_persistentregistry.py` & `zope.component-6.0/src/zope/component/tests/test_persistentregistry.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,75 +11,82 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Tests for z.c.hooks
 """
 import unittest
 
-from zope.interface.tests.test_adapter import CustomTypesBaseAdapterRegistryTests
+from zope.interface.tests.test_adapter import \
+    CustomTypesBaseAdapterRegistryTests
+
 
 def skipIfNoPersistent(testfunc):
     try:
-        import persistent
-    except ImportError: # pragma: no cover
+        import persistent  # noqa: F401 imported but unused
+    except ImportError:  # pragma: no cover
         return unittest.skip("persistent not installed")(testfunc)
     return testfunc
 
+
 @skipIfNoPersistent
 class PersistentAdapterRegistryTests(unittest.TestCase):
 
     def _getTargetClass(self):
         from zope.component.persistentregistry import PersistentAdapterRegistry
         return PersistentAdapterRegistry
 
     def _makeOne(self, *args, **kw):
         return self._getTargetClass()(*args, **kw)
 
     def _makeCache(self, jar):
         # Borrowed from persistent.tests.test_pyPersistence.
 
-        class _Cache(object):
+        class _Cache:
             def __init__(self, jar):
                 self._jar = jar
                 self._mru = []
                 # mru(oid) is only called in pure-Python runs
                 self.mru = self._mru.append
+
             def new_ghost(self, oid, obj):
                 obj._p_jar = self._jar
                 obj._p_oid = oid
+
             def update_object_size_estimation(self, oid, size):
                 "This is only called in pure-Python runs"
 
         return _Cache(jar)
 
     def _makeJar(self):
         # Borrowed from persistent.tests.test_pyPersistence.
-        from zope.interface import implementer
         from persistent.interfaces import IPersistentDataManager
+        from zope.interface import implementer
 
         @implementer(IPersistentDataManager)
-        class _Jar(object):
+        class _Jar:
             def __init__(self):
                 self._loaded = []
                 self._registered = []
+
             def setstate(self, obj):
                 self._loaded.append(obj._p_oid)
+
             def register(self, obj):
                 self._registered.append(obj._p_oid)
 
         jar = _Jar()
         jar._cache = self._makeCache(jar)
         return jar
 
     def _makeOneWithJar(self, dirty=False, **kw):
         # Borrowed from persistent.tests.test_pyPersistence.
         OID = _makeOctets('\x01' * 8)
         inst = self._makeOne(**kw)
         jar = self._makeJar()
-        jar._cache.new_ghost(OID, inst) # assigns _p_jar, _p_oid
+        jar._cache.new_ghost(OID, inst)  # assigns _p_jar, _p_oid
         return inst, jar, OID
 
     def test_changed_original_is_not_us(self):
         registry, jar, OID = self._makeOneWithJar()
         self.assertEqual(registry._generation, 1)
         registry.changed(object())
         # 'originally_changed' is not us, but we are still dirty because
@@ -115,15 +122,15 @@
         registry.names = lambda *args: ['a', 'b', 'c']
         self.assertFalse('names' in registry.__getstate__())
 
     def test___setstate___rebuilds__v_lookup(self):
         registry, jar, OID = self._makeOneWithJar()
         state = registry.__getstate__()
         self.assertTrue('_v_lookup' in registry.__dict__)
-        registry._p_changed = None # clears volatile '_v_lookup'
+        registry._p_changed = None  # clears volatile '_v_lookup'
         self.assertFalse('_v_lookup' in registry.__dict__)
         registry.__setstate__(state)
         self.assertTrue('_v_lookup' in registry.__dict__)
 
     def test___setstate___rebuilds__ro(self):
         from zope.component import globalSiteManager
         bases = (globalSiteManager.adapters, globalSiteManager.utilities)
@@ -187,16 +194,17 @@
         from zope.component.persistentregistry import PersistentComponents
         return PersistentComponents
 
     def _makeOne(self, *args, **kw):
         return self._getTargetClass()(*args, **kw)
 
     def test_ctor_initializes_registries_and_registrations(self):
-        from persistent.mapping import PersistentMapping
         from persistent.list import PersistentList
+        from persistent.mapping import PersistentMapping
+
         from zope.component.persistentregistry import PersistentAdapterRegistry
         registry = self._makeOne()
         self.assertTrue(isinstance(registry.adapters,
                                    PersistentAdapterRegistry))
         self.assertTrue(isinstance(registry.utilities,
                                    PersistentAdapterRegistry))
         self.assertTrue(isinstance(registry._adapter_registrations,
@@ -204,20 +212,22 @@
         self.assertTrue(isinstance(registry._utility_registrations,
                                    PersistentMapping))
         self.assertTrue(isinstance(registry._subscription_registrations,
                                    PersistentList))
         self.assertTrue(isinstance(registry._handler_registrations,
                                    PersistentList))
 
+
 def _makeOctets(s):
     return bytes(s) if bytes is str else bytes(s, 'ascii')
 
 
 @skipIfNoPersistent
-class PersistentAdapterRegistryCustomTypesTest(CustomTypesBaseAdapterRegistryTests):
+class PersistentAdapterRegistryCustomTypesTest(
+        CustomTypesBaseAdapterRegistryTests):
 
     def _getMappingType(self):
         from persistent.mapping import PersistentMapping
         return PersistentMapping
 
     def _getProvidedType(self):
         return self._getMappingType()
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test_registry.py` & `zope.component-6.0/src/zope/component/tests/test_registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,103 +13,116 @@
 ##############################################################################
 """Tests for z.c.registry
 """
 import unittest
 
 from zope.component.tests import fails_if_called
 
+
 class Test_dispatchUtilityRegistrationEvent(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.registry import dispatchUtilityRegistrationEvent
         return dispatchUtilityRegistrationEvent(*args, **kw)
 
     def test_it(self):
         from zope.component import registry
-        class _Registration(object):
+
+        class _Registration:
             component = object()
         _EVENT = object()
         _handled = []
+
         def _handle(*args):
             _handled.append(args)
         with _Monkey(registry, handle=_handle):
             self._callFUT(_Registration(), _EVENT)
         self.assertEqual(_handled, [(_Registration.component, _EVENT)])
 
 
 class Test_dispatchAdapterRegistrationEvent(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.registry import dispatchAdapterRegistrationEvent
         return dispatchAdapterRegistrationEvent(*args, **kw)
 
     def test_it(self):
         from zope.component import registry
-        class _Registration(object):
+
+        class _Registration:
             factory = fails_if_called(self)
         _registration = _Registration()
         _EVENT = object()
         _handled = []
+
         def _handle(*args):
             _handled.append(args)
         with _Monkey(registry, handle=_handle):
             self._callFUT(_registration, _EVENT)
         self.assertEqual(_handled, [(_registration.factory, _EVENT)])
 
 
 class Test_dispatchSubscriptionAdapterRegistrationEvent(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
-        from zope.component.registry \
-            import dispatchSubscriptionAdapterRegistrationEvent
+        from zope.component.registry import \
+            dispatchSubscriptionAdapterRegistrationEvent
         return dispatchSubscriptionAdapterRegistrationEvent(*args, **kw)
 
     def test_it(self):
         from zope.component import registry
-        class _Registration(object):
+
+        class _Registration:
             factory = fails_if_called(self)
         _registration = _Registration()
         _EVENT = object()
         _handled = []
+
         def _handle(*args):
             _handled.append(args)
         with _Monkey(registry, handle=_handle):
             self._callFUT(_registration, _EVENT)
         self.assertEqual(_handled, [(_registration.factory, _EVENT)])
 
 
 class Test_dispatchHandlerRegistrationEvent(unittest.TestCase):
 
-    from zope.component.testing import setUp, tearDown
+    from zope.component.testing import setUp
+    from zope.component.testing import tearDown
 
     def _callFUT(self, *args, **kw):
         from zope.component.registry import dispatchHandlerRegistrationEvent
         return dispatchHandlerRegistrationEvent(*args, **kw)
 
     def test_it(self):
         from zope.component import registry
-        class _Registration(object):
+
+        class _Registration:
             handler = fails_if_called(self)
         _registration = _Registration()
         _EVENT = object()
         _handled = []
+
         def _handle(*args):
             _handled.append(args)
         with _Monkey(registry, handle=_handle):
             self._callFUT(_registration, _EVENT)
         self.assertEqual(_handled, [(_registration.handler, _EVENT)])
 
 
-class _Monkey(object):
+class _Monkey:
     # context-manager for replacing module names in the scope of a test.
     def __init__(self, module, **kw):
         self.module = module
         self.to_restore = {key: getattr(module, key) for key in kw}
         for key, value in kw.items():
             setattr(module, key, value)
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test_security.py` & `zope.component-6.0/src/zope/component/tests/test_security.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 #
 ##############################################################################
 """
 Tests for zope.component.security
 """
 import unittest
 
-from zope.component.tests import skipIfNoSecurity
 from zope.component.tests import fails_if_called
+from zope.component.tests import skipIfNoSecurity
+
 
 @skipIfNoSecurity
 class PermissionProxyTests(unittest.TestCase):
 
     def _getTargetClass(self):
         from zope.component.security import PermissionProxy
         return PermissionProxy
@@ -29,23 +30,26 @@
     def _makeOne(self, wrapped):
         return self._getTargetClass()(wrapped)
 
     def test_proxy_delegates___provided_by__(self):
         from zope.interface import Interface
         from zope.interface import implementer
         from zope.interface import providedBy
+
         class IFoo(Interface):
             pass
+
         @implementer(IFoo)
-        class Foo(object):
+        class Foo:
             pass
         foo = Foo()
         proxy = self._makeOne(foo)
         self.assertEqual(providedBy(proxy), providedBy(foo))
 
+
 @skipIfNoSecurity
 class Test__checker(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.component.security import _checker
         return _checker(*args, **kw)
 
@@ -53,74 +57,81 @@
         from zope.security.checker import CheckerPublic
         checker = self._callFUT(object(), 'zope.Public', (), ())
         self.assertEqual(checker.get_permissions, {'__call__': CheckerPublic})
         self.assertFalse(checker.set_permissions)
 
     def test_w_allowed_interfaces(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             def bar(self):
                 "bar"
+
             def baz(self):
                 "baz"
         class ISpam(Interface):
             def qux(self):
                 "qux"
         checker = self._callFUT(object(), 'testing', (IFoo, ISpam), ())
-        self.assertEqual(checker.get_permissions,
-                        {'bar': 'testing', 'baz': 'testing', 'qux': 'testing'})
+        self.assertEqual(
+            checker.get_permissions, {
+                'bar': 'testing', 'baz': 'testing', 'qux': 'testing'})
         self.assertFalse(checker.set_permissions)
 
     def test_w_allowed_attributes(self):
         checker = self._callFUT(object(), 'testing', (), ('foo', 'bar'))
         self.assertEqual(checker.get_permissions,
-                        {'foo': 'testing', 'bar': 'testing'})
+                         {'foo': 'testing', 'bar': 'testing'})
         self.assertFalse(checker.set_permissions)
 
+
 @skipIfNoSecurity
 class Test_proxify(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.component.security import proxify
         return proxify(*args, **kw)
 
     def _makeContext(self):
-        class _Context(object):
+        class _Context:
             bar = fails_if_called(self)
         return _Context()
 
     def test_no_checker_no_provides(self):
         ctx = self._makeContext()
         self.assertRaises(ValueError, self._callFUT, ctx, permission='testing')
 
     def test_no_checker_no_permission(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             def bar(self):
                 "bar"
         ctx = self._makeContext()
         self.assertRaises(ValueError, self._callFUT, ctx, provides=IFoo)
 
     def test_no_checker_w_provides_and_permission_public(self):
         from zope.interface import Interface
-        from zope.security.checker import CheckerPublic
         from zope.proxy import getProxiedObject
+        from zope.security.checker import CheckerPublic
+
         class IFoo(Interface):
             def bar(self):
                 "bar"
         ctx = self._makeContext()
         proxy = self._callFUT(ctx, provides=IFoo, permission='zope.Public')
         self.assertTrue(getProxiedObject(proxy) is ctx)
         checker = proxy.__Security_checker__
         self.assertEqual(checker.get_permissions, {'bar': CheckerPublic})
         self.assertFalse(checker.set_permissions)
 
     def test_no_checker_w_provides_and_permission_protected(self):
         from zope.interface import Interface
         from zope.proxy import getProxiedObject
+
         class IFoo(Interface):
             def bar(self):
                 "bar"
         ctx = self._makeContext()
         proxy = self._callFUT(ctx, provides=IFoo, permission='testing')
         self.assertTrue(getProxiedObject(proxy) is ctx)
         checker = proxy.__Security_checker__
@@ -131,110 +142,121 @@
         from zope.proxy import getProxiedObject
         _CHECKER = object()
         ctx = self._makeContext()
         proxy = self._callFUT(ctx, _CHECKER)
         self.assertTrue(getProxiedObject(proxy) is ctx)
         self.assertTrue(proxy.__Security_checker__ is _CHECKER)
 
+
 @skipIfNoSecurity
 class Test_protectedFactory(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.component.security import protectedFactory
         return protectedFactory(*args, **kw)
 
     def test_public_not_already_proxied(self):
         from zope.interface import Interface
         from zope.security.checker import CheckerPublic
+
         class IFoo(Interface):
             def bar(self):
                 "bar"
-        class _Factory(object):
+        class _Factory:
             bar = fails_if_called(self)
         protected = self._callFUT(_Factory, IFoo, 'zope.Public')
         self.assertTrue(protected.factory is _Factory)
         foo = protected()
         self.assertEqual(foo.__Security_checker__.get_permissions,
-                        {'bar': CheckerPublic})
+                         {'bar': CheckerPublic})
 
     def test_nonpublic_already_proxied(self):
         from zope.interface import Interface
         from zope.security.proxy import getTestProxyItems
+
         class IFoo(Interface):
             def bar(self):
                 "bar"
-        class _Factory(object):
+        class _Factory:
             __slots__ = ('one',)
             bar = fails_if_called(self)
         protected = self._callFUT(_Factory, IFoo, 'testing')
         self.assertTrue(protected.factory is _Factory)
         foo = protected()
         self.assertEqual(getTestProxyItems(foo), [('bar', 'testing')])
 
+
 @skipIfNoSecurity
 class Test_securityAdapterFactory(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.component.security import securityAdapterFactory
         return securityAdapterFactory(*args, **kw)
 
     def test_no_permission_untrusted_no_location(self):
-        class _Factory(object):
+        class _Factory:
             pass
         self.assertTrue(self._callFUT(_Factory, None, False, False)
                         is _Factory)
 
     def test_public_untrusted_no_location(self):
-        class _Factory(object):
+        class _Factory:
             pass
         self.assertTrue(self._callFUT(_Factory, 'zope.Public', False, False)
                         is _Factory)
 
     def test_CheckerPublic_untrusted_no_location(self):
         from zope.security.checker import CheckerPublic
-        class _Factory(object):
+
+        class _Factory:
             pass
         self.assertTrue(self._callFUT(_Factory, CheckerPublic, False, False)
                         is _Factory)
 
     def test_protected_untrusted_no_location(self):
         from zope.security.adapter import LocatingUntrustedAdapterFactory
-        class _Factory(object):
+
+        class _Factory:
             pass
         proxy = self._callFUT(_Factory, 'testing', False, False)
         self.assertTrue(isinstance(proxy, LocatingUntrustedAdapterFactory))
 
     def test_no_permission_trusted_no_location(self):
         from zope.security.adapter import LocatingTrustedAdapterFactory
-        class _Factory(object):
+
+        class _Factory:
             pass
         proxy = self._callFUT(_Factory, None, False, True)
         self.assertTrue(isinstance(proxy, LocatingTrustedAdapterFactory))
 
     def test_public_trusted_no_location(self):
         from zope.security.adapter import LocatingTrustedAdapterFactory
-        class _Factory(object):
+
+        class _Factory:
             pass
         proxy = self._callFUT(_Factory, 'zope.Public', False, True)
         self.assertTrue(isinstance(proxy, LocatingTrustedAdapterFactory))
 
     def test_CheckerPublic_trusted_no_location(self):
         from zope.security.adapter import LocatingTrustedAdapterFactory
         from zope.security.checker import CheckerPublic
-        class _Factory(object):
+
+        class _Factory:
             pass
         proxy = self._callFUT(_Factory, CheckerPublic, False, True)
         self.assertTrue(isinstance(proxy, LocatingTrustedAdapterFactory))
 
     def test_protected_trusted_no_location(self):
         from zope.security.adapter import LocatingTrustedAdapterFactory
-        class _Factory(object):
+
+        class _Factory:
             pass
         proxy = self._callFUT(_Factory, 'testing', False, True)
         self.assertTrue(isinstance(proxy, LocatingTrustedAdapterFactory))
 
     def test_protected_trusted_w_location(self):
         from zope.security.adapter import LocatingTrustedAdapterFactory
-        class _Factory(object):
+
+        class _Factory:
             pass
         proxy = self._callFUT(_Factory, 'testing', True, True)
         self.assertTrue(isinstance(proxy, LocatingTrustedAdapterFactory))
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test_standalone.py` & `zope.component-6.0/src/zope/component/tests/test_standalone.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,41 +13,42 @@
 ##############################################################################
 """Component Architecture Tests
 """
 import unittest
 
 from zope.component.tests import skipIfNoSecurity
 
+
 @skipIfNoSecurity
 class StandaloneTests(unittest.TestCase):
     def testStandalone(self):
         # See: https://bugs.launchpad.net/zope3/+bug/98401
-        import subprocess
-        import sys
         import os
         import pickle
+        import subprocess
+        import sys
 
         executable = os.path.abspath(sys.executable)
         where = os.path.dirname(os.path.dirname(__file__))
         program = os.path.join(where, 'standalonetests.py')
         process = subprocess.Popen([executable, program],
-                                stdout=subprocess.PIPE,
-                                stderr=subprocess.STDOUT,
-                                stdin=subprocess.PIPE)
+                                   stdout=subprocess.PIPE,
+                                   stderr=subprocess.STDOUT,
+                                   stdin=subprocess.PIPE)
         try:
             pickle.dump(sys.path, process.stdin)
             process.stdin.close()
 
             try:
                 rc = process.wait()
-            except OSError as e: # pragma: no cover
+            except OSError as e:  # pragma: no cover
                 # MacIntel raises apparently unimportant EINTR?
                 if e.errno != 4:
-                    raise # TODO verify sanity of a pass on EINTR :-/
-            if rc != 0: # pragma: no cover
+                    raise  # TODO verify sanity of a pass on EINTR :-/
+            if rc != 0:  # pragma: no cover
                 output = process.stdout.read()
                 if isinstance(output, bytes):
                     output = output.decode()
                 sys.stderr.write('#' * 80 + '\n')
                 sys.stdout.write(output)
                 sys.stderr.write('#' * 80 + '\n')
                 self.fail('Output code: %d' % rc)
```

### Comparing `zope.component-5.1.0/src/zope/component/tests/test_zcml.py` & `zope.component-6.0/src/zope/component/tests/test_zcml.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,61 +14,69 @@
 """Tests for ZCML directives.
 """
 import unittest
 
 from zope.component.tests import fails_if_called
 from zope.component.tests import skipIfNoSecurity
 
+
 class Test_handler(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.component.zcml import handler
         return handler(*args, **kw)
 
     def test_uses_configured_site_manager(self):
         from zope.interface.registry import Components
+
         from zope.component import getSiteManager
-        from zope.component.testfiles.components import comp, IApp
+        from zope.component.testfiles.components import IApp
+        from zope.component.testfiles.components import comp
 
         registry = Components()
+
         def dummy(context=None):
             return registry
         getSiteManager.sethook(dummy)
 
         try:
-            self._callFUT('registerUtility', comp, IApp, u'')
+            self._callFUT('registerUtility', comp, IApp, '')
             self.assertTrue(registry.getUtility(IApp) is comp)
         finally:
             getSiteManager.reset()
 
 
 class Test__rolledUpFactory(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.component.zcml import _rolledUpFactory
         return _rolledUpFactory(*args, **kw)
 
     def test_with_one(self):
         _OBJ = object()
         _CREATED = object()
+
         def _factory(obj):
             return _CREATED
         rolled = self._callFUT([_factory])
         self.assertTrue(rolled.factory is _factory)
         self.assertTrue(rolled(_OBJ) is _CREATED)
 
     def test_with_multiple(self):
         _OBJ = object()
         _CREATED1 = object()
         _CREATED2 = object()
         _CREATED3 = object()
+
         def _factory1(obj):
             return _CREATED1
+
         def _factory2(obj):
             return _CREATED2
+
         def _factory3(obj):
             return _CREATED3
         rolled = self._callFUT([_factory1, _factory2, _factory3])
         self.assertTrue(rolled.factory is _factory1)
         self.assertTrue(rolled(_OBJ) is _CREATED3)
 
 
@@ -76,125 +84,146 @@
 
     def _callFUT(self, *args, **kw):
         from zope.component.zcml import adapter
         return adapter(*args, **kw)
 
     def test_empty_factory(self):
         from zope.interface import Interface
+
         from zope.component.zcml import ComponentConfigurationError
+
         class IFoo(Interface):
             pass
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(ComponentConfigurationError,
                           self._callFUT, _cfg_ctx, [], [Interface], IFoo)
 
     def test_multiple_factory_multiple_for_(self):
         from zope.interface import Interface
+
         from zope.component.zcml import ComponentConfigurationError
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
-        class Bar(object):
+
+        class Bar:
             pass
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(ComponentConfigurationError,
                           self._callFUT, _cfg_ctx, [Foo, Bar],
-                                         [Interface, IBar], IFoo)
+                          [Interface, IBar], IFoo)
 
     def test_no_for__factory_not_adapts(self):
-        #@adapter(IFoo)
-        class _Factory(object):
+        # @adapter(IFoo)
+        class _Factory:
             __init__ = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(TypeError, self._callFUT, _cfg_ctx, [_Factory])
 
     def test_no_name(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
-        from zope.component import adapter, named
         from zope.interface import implementer
+
+        from zope.component import adapter
+        from zope.component import named
+
         @adapter(IFoo)
         @implementer(IBar)
         @named('bar')
-        class _Factory(object):
+        class _Factory:
             __init__ = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, [_Factory])
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['args'][4], 'bar')
 
     def test_no_for__factory_adapts_no_provides_factory_not_implements(self):
         from zope.interface import Interface
+
         from zope.component._declaration import adapter
+
         @adapter(Interface)
-        class _Factory(object):
+        class _Factory:
             __init__ = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(TypeError, self._callFUT, _cfg_ctx, [_Factory])
 
     def test_multiple_factory_single_for__w_name(self):
         from zope.interface import Interface
+
         from zope.component.interface import provideInterface
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
-        class Bar(object):
+
+        class Bar:
             pass
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, [Foo, Bar], IFoo, [Interface], name='test')
         self.assertEqual(len(_cfg_ctx._actions), 3)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'],
                          ('adapter', (Interface,), IFoo, 'test'))
         self.assertEqual(action['args'][0], 'registerAdapter')
-        self.assertEqual(action['args'][1].factory, Foo) #rolled up
+        self.assertEqual(action['args'][1].factory, Foo)  # rolled up
         self.assertEqual(action['args'][2], (Interface,))
         self.assertEqual(action['args'][3], IFoo)
         self.assertEqual(action['args'][4], 'test')
         self.assertEqual(action['args'][5], 'TESTING')
         # Register the provided interface
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IFoo))
         # Register the required interface(s)
         self.assertEqual(_cfg_ctx._actions[2][0], ())
-        action =_cfg_ctx._actions[2][1]
+        action = _cfg_ctx._actions[2][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', Interface))
 
     @skipIfNoSecurity
     def test_single_factory_single_for_w_permission(self):
         from zope.interface import Interface
         from zope.security.adapter import LocatingUntrustedAdapterFactory
+
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, [Foo], IFoo, [Interface], permission='testing')
         self.assertEqual(len(_cfg_ctx._actions), 3)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'],
                          ('adapter', (Interface,), IFoo, ''))
         self.assertEqual(action['args'][0], 'registerAdapter')
         factory_proxy = action['args'][1]
         # Foo wraped by 'protected_factory' plus
         # 'LocatingUntrustedAdapterFactory'
@@ -206,25 +235,28 @@
         self.assertEqual(action['args'][4], '')
         self.assertEqual(action['args'][5], 'TESTING')
 
     @skipIfNoSecurity
     def test_single_factory_single_for_w_locate_no_permission(self):
         from zope.interface import Interface
         from zope.security.adapter import LocatingUntrustedAdapterFactory
+
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, [Foo], IFoo, [Interface], locate=True)
         self.assertEqual(len(_cfg_ctx._actions), 3)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'],
                          ('adapter', (Interface,), IFoo, ''))
         self.assertEqual(action['args'][0], 'registerAdapter')
         factory_proxy = action['args'][1]
         # Foo wraped by 'LocatingUntrustedAdapterFactory'
         self.assertTrue(isinstance(factory_proxy,
@@ -235,25 +267,28 @@
         self.assertEqual(action['args'][4], '')
         self.assertEqual(action['args'][5], 'TESTING')
 
     @skipIfNoSecurity
     def test_single_factory_single_for_w_trusted_no_permission(self):
         from zope.interface import Interface
         from zope.security.adapter import TrustedAdapterFactory
+
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, [Foo], IFoo, [Interface], trusted=True)
         self.assertEqual(len(_cfg_ctx._actions), 3)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'],
                          ('adapter', (Interface,), IFoo, ''))
         self.assertEqual(action['args'][0], 'registerAdapter')
         factory_proxy = action['args'][1]
         # Foo wraped by 'LocatingUntrustedAdapterFactory'
         self.assertTrue(isinstance(factory_proxy, TrustedAdapterFactory))
@@ -262,35 +297,39 @@
         self.assertEqual(action['args'][3], IFoo)
         self.assertEqual(action['args'][4], '')
         self.assertEqual(action['args'][5], 'TESTING')
 
     def test_no_for__no_provides_factory_adapts_factory_implements(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component._declaration import adapter
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
+
         @adapter(Interface)
         @implementer(IFoo)
-        class _Factory(object):
+        class _Factory:
             __init__ = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, [_Factory])
         self.assertEqual(len(_cfg_ctx._actions), 3)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'],
                          ('adapter', (Interface,), IFoo, ''))
         self.assertEqual(action['args'],
                          ('registerAdapter', _Factory, (Interface,), IFoo,
                           '', 'TESTING'))
 
+
 class Test_zcml_functional(unittest.TestCase):
     # These mimic the snippets in the zcml.rst doctests
 
     def setUp(self):
         from zope.component.tests.examples import clearZCML
         clearZCML()
     tearDown = setUp
@@ -301,23 +340,24 @@
         <configure xmlns='http://namespaces.zope.org/zope'
                    i18n_domain="zope">
            <include package="zope.component" file="meta.zcml" />
            %s
         </configure>""" % snippet
         xmlconfig.string(template)
 
-
     @skipIfNoSecurity
     def test_with_proxy_factory_public_permission(self):
         # Using the public permission doesn't give you a location proxy
         from zope.proxy import isProxy
+        from zope.security.checker import ProxyFactory
         from zope.security.proxy import removeSecurityProxy
+
+        from zope.component.testfiles.adapter import A1
+        from zope.component.testfiles.adapter import I1
         from zope.component.testfiles.components import Content
-        from zope.component.testfiles.adapter import I1, A1
-        from zope.security.checker import ProxyFactory
 
         self._runSnippet('''
             <adapter
             for="zope.component.testfiles.components.IContent"
             provides="zope.component.testfiles.adapter.I1"
             factory="zope.component.testfiles.adapter.A1"
             permission="zope.Public"
@@ -326,25 +366,26 @@
         ob = Content()
         p = ProxyFactory(ob)
 
         a = I1(p)
 
         self.assertTrue(isProxy(a))
 
-        self.assertTrue(type(removeSecurityProxy(a)) is A1)
+        self.assertTrue(isinstance(removeSecurityProxy(a), A1))
 
     @skipIfNoSecurity
     def test_located_proxy_factory(self):
         # Passing locate results in a security proxy around a location proxy
+        from zope.location.location import LocationProxy
         from zope.proxy import isProxy
+        from zope.security.checker import ProxyFactory
         from zope.security.proxy import removeSecurityProxy
-        from zope.component.testfiles.components import Content
+
         from zope.component.testfiles.adapter import I1
-        from zope.security.checker import ProxyFactory
-        from zope.location.location import LocationProxy
+        from zope.component.testfiles.components import Content
 
         self._runSnippet('''
         <adapter
           for="zope.component.testfiles.components.IContent"
           provides="zope.component.testfiles.adapter.I1"
           factory="zope.component.testfiles.adapter.A1"
           trusted="yes"
@@ -353,15 +394,16 @@
         ''')
         ob = Content()
         p = ProxyFactory(ob)
         a = I1(p)
 
         self.assertTrue(isProxy(a))
 
-        self.assertTrue(type(removeSecurityProxy(a)) is LocationProxy)
+        self.assertTrue(isinstance(removeSecurityProxy(a), LocationProxy))
+
 
 class Test_subscriber(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.component.zcml import subscriber
         return subscriber(*args, **kw)
 
@@ -369,129 +411,141 @@
         from zope.interface import Interface
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(TypeError,
                           self._callFUT, _cfg_ctx, (Interface,))
 
     def test_no_factory_w_handler_w_provides(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
         _handler = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(TypeError,
                           self._callFUT, _cfg_ctx, (Interface,),
-                                         handler=_handler, provides=IFoo)
+                          handler=_handler, provides=IFoo)
 
     def test_w_factory_w_handler(self):
         from zope.interface import Interface
-        class Foo(object):
+
+        class Foo:
             pass
         _handler = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(TypeError,
                           self._callFUT, _cfg_ctx, (Interface,), Foo,
-                                         handler=_handler)
+                          handler=_handler)
 
     def test_w_factory_no_provides(self):
         from zope.interface import Interface
-        class Foo(object):
+
+        class Foo:
             pass
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(TypeError,
                           self._callFUT, _cfg_ctx, (Interface,), Foo)
 
     def test_w_factory_w_provides_no_for_factory_wo_adapter(self):
         from zope.interface import Interface
+
         class IFoo(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(TypeError,
                           self._callFUT, _cfg_ctx,
-                                         factory=Foo, provides=IFoo)
+                          factory=Foo, provides=IFoo)
 
     def test_no_factory_w_handler_no_provides(self):
         from zope.interface import Interface
+
         from zope.component.interface import provideInterface
         from zope.component.zcml import handler
         _handler = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, (Interface,), handler=_handler)
         self.assertEqual(len(_cfg_ctx._actions), 2)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'][0], 'registerHandler')
         self.assertEqual(action['args'][1], _handler)
         self.assertEqual(action['args'][2], (Interface,))
         self.assertEqual(action['args'][3], '')
         self.assertEqual(action['args'][4], 'TESTING')
         # Register the required interface(s)
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', Interface))
 
     def test_w_factory_w_provides(self):
         from zope.interface import Interface
+
         from zope.component.interface import provideInterface
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
-        _handler = fails_if_called(self)
+        fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, (Interface,), Foo, provides=IFoo)
         self.assertEqual(len(_cfg_ctx._actions), 3)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'][0], 'registerSubscriptionAdapter')
         self.assertEqual(action['args'][1], Foo)
         self.assertEqual(action['args'][2], (Interface,))
         self.assertEqual(action['args'][3], IFoo)
         self.assertEqual(action['args'][4], '')
         self.assertEqual(action['args'][5], 'TESTING')
         # Register the provided interface
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IFoo))
         # Register the required interface(s)
         self.assertEqual(_cfg_ctx._actions[2][0], ())
-        action =_cfg_ctx._actions[2][1]
+        action = _cfg_ctx._actions[2][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', Interface))
 
     @skipIfNoSecurity
     def test_w_factory_w_provides_w_permission(self):
         from zope.interface import Interface
         from zope.security.adapter import LocatingUntrustedAdapterFactory
+
         from zope.component.interface import provideInterface
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, (Interface,), Foo,
                       provides=IFoo, permission='testing')
         self.assertEqual(len(_cfg_ctx._actions), 3)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'][0], 'registerSubscriptionAdapter')
         factory_proxy = action['args'][1]
         # Foo wraped by 'protected_factory' plus
         # 'LocatingUntrustedAdapterFactory'
         self.assertTrue(isinstance(factory_proxy,
@@ -499,41 +553,44 @@
         self.assertTrue(factory_proxy.factory.factory is Foo)
         self.assertEqual(action['args'][2], (Interface,))
         self.assertEqual(action['args'][3], IFoo)
         self.assertEqual(action['args'][4], '')
         self.assertEqual(action['args'][5], 'TESTING')
         # Register the provided interface
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IFoo))
         # Register the required interface(s)
         self.assertEqual(_cfg_ctx._actions[2][0], ())
-        action =_cfg_ctx._actions[2][1]
+        action = _cfg_ctx._actions[2][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', Interface))
 
     @skipIfNoSecurity
     def test_w_factory_w_provides_wo_permission_w_locate(self):
         from zope.interface import Interface
         from zope.security.adapter import LocatingUntrustedAdapterFactory
+
         from zope.component.interface import provideInterface
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, (Interface,), Foo, provides=IFoo, locate=True)
         self.assertEqual(len(_cfg_ctx._actions), 3)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'][0], 'registerSubscriptionAdapter')
         factory_proxy = action['args'][1]
         # Foo wraped by 'protected_factory' plus
         # 'LocatingUntrustedAdapterFactory'
         self.assertTrue(isinstance(factory_proxy,
@@ -541,41 +598,44 @@
         self.assertTrue(factory_proxy.factory is Foo)
         self.assertEqual(action['args'][2], (Interface,))
         self.assertEqual(action['args'][3], IFoo)
         self.assertEqual(action['args'][4], '')
         self.assertEqual(action['args'][5], 'TESTING')
         # Register the provided interface
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IFoo))
         # Register the required interface(s)
         self.assertEqual(_cfg_ctx._actions[2][0], ())
-        action =_cfg_ctx._actions[2][1]
+        action = _cfg_ctx._actions[2][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', Interface))
 
     @skipIfNoSecurity
     def test_w_factory_w_provides_wo_permission_w_trusted(self):
         from zope.interface import Interface
         from zope.security.adapter import TrustedAdapterFactory
+
         from zope.component.interface import provideInterface
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, (Interface,), Foo, provides=IFoo, trusted=True)
         self.assertEqual(len(_cfg_ctx._actions), 3)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'][0], 'registerSubscriptionAdapter')
         factory_proxy = action['args'][1]
         # Foo wraped by 'protected_factory' plus
         # 'TrustedAdapterFactory'
         self.assertTrue(isinstance(factory_proxy,
@@ -583,267 +643,296 @@
         self.assertTrue(factory_proxy.factory is Foo)
         self.assertEqual(action['args'][2], (Interface,))
         self.assertEqual(action['args'][3], IFoo)
         self.assertEqual(action['args'][4], '')
         self.assertEqual(action['args'][5], 'TESTING')
         # Register the provided interface
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IFoo))
         # Register the required interface(s)
         self.assertEqual(_cfg_ctx._actions[2][0], ())
-        action =_cfg_ctx._actions[2][1]
+        action = _cfg_ctx._actions[2][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', Interface))
 
     def test_no_for__no_provides_subscriber_adapts_subscriber_implements(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component._declaration import adapter
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
+
         @adapter(Interface)
         @implementer(IFoo)
-        class _Factory(object):
+        class _Factory:
             def __init__(self, context):
-                self.context = context
+                self.context = context  # pragma: no cover
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, factory=_Factory)
         self.assertEqual(len(_cfg_ctx._actions), 3)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the subscriber
         action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertIsNone(action['discriminator'])
-        self.assertEqual(action['args'],
-                         ('registerSubscriptionAdapter', _Factory, (Interface,), IFoo,
-                          '', 'TESTING'))
+        self.assertEqual(
+            action['args'],
+            ('registerSubscriptionAdapter',
+             _Factory,
+             (Interface,
+              ),
+                IFoo,
+                '',
+                'TESTING'))
+
 
 class Test_utility(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.component.zcml import utility
         return utility(*args, **kw)
 
     def test_w_factory_w_component(self):
-        class _Factory(object):
+        class _Factory:
             pass
         _COMPONENT = object
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(TypeError, self._callFUT, _cfg_ctx,
-                                         factory=_Factory,
-                                         component=_COMPONENT)
+                          factory=_Factory,
+                          component=_COMPONENT)
 
     def test_w_factory_wo_provides_factory_no_implements(self):
-        class _Factory(object):
+        class _Factory:
             pass
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(TypeError,
                           self._callFUT, _cfg_ctx, factory=_Factory)
 
     def test_w_component_wo_provides_component_no_provides(self):
         _COMPONENT = object
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(TypeError,
                           self._callFUT, _cfg_ctx, component=_COMPONENT)
 
     def test_w_factory_w_provides(self):
         from zope.interface import Interface
+
         from zope.component.interface import provideInterface
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, factory=Foo, provides=IFoo)
         self.assertEqual(len(_cfg_ctx._actions), 2)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the utility
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'], ('utility', IFoo, ''))
         self.assertEqual(action['args'][0], 'registerUtility')
         self.assertEqual(action['args'][1], None)
         self.assertEqual(action['args'][2], IFoo)
         self.assertEqual(action['args'][3], '')
         self.assertEqual(action['args'][4], 'TESTING')
         self.assertEqual(action['kw'], {'factory': Foo})
         # Register the provided interface
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IFoo))
 
     def test_w_factory_wo_provides_factory_implements(self):
         from zope.interface import Interface
         from zope.interface import implementer
+
         from zope.component.interface import provideInterface
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
+
         @implementer(IFoo)
-        class Foo(object):
+        class Foo:
             pass
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, factory=Foo)
         self.assertEqual(len(_cfg_ctx._actions), 2)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the utility
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'], ('utility', IFoo, ''))
         self.assertEqual(action['args'][0], 'registerUtility')
         self.assertEqual(action['args'][1], None)
         self.assertEqual(action['args'][2], IFoo)
         self.assertEqual(action['args'][3], '')
         self.assertEqual(action['args'][4], 'TESTING')
         self.assertEqual(action['kw'], {'factory': Foo})
         # Register the provided interface
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IFoo))
 
     def test_w_component_w_provides_w_name(self):
         from zope.interface import Interface
+
         from zope.component.interface import provideInterface
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
         _COMPONENT = object()
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, component=_COMPONENT,
                       name='test', provides=IFoo)
         self.assertEqual(len(_cfg_ctx._actions), 2)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the utility
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'], ('utility', IFoo, 'test'))
         self.assertEqual(action['args'][0], 'registerUtility')
         self.assertEqual(action['args'][1], _COMPONENT)
         self.assertEqual(action['args'][2], IFoo)
         self.assertEqual(action['args'][3], 'test')
         self.assertEqual(action['args'][4], 'TESTING')
         # Register the provided interface
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IFoo))
 
     def test_w_component_wo_provides_wo_name(self):
-        from zope.interface import Interface, implementer, named
-        from zope.component.zcml import handler
+        from zope.interface import Interface
+        from zope.interface import implementer
+        from zope.interface import named
+
         class IFoo(Interface):
             pass
+
         @implementer(IFoo)
         @named('foo')
-        class Foo(object):
+        class Foo:
             pass
         foo = Foo()
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, component=foo)
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['args'][1], foo)
         self.assertEqual(action['args'][2], IFoo)
         self.assertEqual(action['args'][3], 'foo')
 
     def test_w_component_wo_provides_component_provides(self):
         from zope.interface import Interface
         from zope.interface import directlyProvides
+
         from zope.component.interface import provideInterface
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
         _COMPONENT = Foo()
         directlyProvides(_COMPONENT, IFoo)
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, component=_COMPONENT)
         self.assertEqual(len(_cfg_ctx._actions), 2)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the utility
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'], ('utility', IFoo, ''))
         self.assertEqual(action['args'][0], 'registerUtility')
         self.assertEqual(action['args'][1], _COMPONENT)
         self.assertEqual(action['args'][2], IFoo)
         self.assertEqual(action['args'][3], '')
         self.assertEqual(action['args'][4], 'TESTING')
         # Register the provided interface
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IFoo))
 
     @skipIfNoSecurity
     def test_w_component_w_provides_w_permission(self):
         from zope.interface import Interface
         from zope.proxy import removeAllProxies
+
         from zope.component.interface import provideInterface
         from zope.component.security import PermissionProxy
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             def bar(self):
                 "bar"
-        class Foo(object):
+        class Foo:
             bar = fails_if_called(self)
         _COMPONENT = Foo()
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, component=_COMPONENT,
-                                provides=IFoo, permission='testing')
+                      provides=IFoo, permission='testing')
         self.assertEqual(len(_cfg_ctx._actions), 2)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the utility
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'], ('utility', IFoo, ''))
         self.assertEqual(action['args'][0], 'registerUtility')
         component_proxy = action['args'][1]
         self.assertTrue(isinstance(component_proxy, PermissionProxy))
         self.assertTrue(removeAllProxies(component_proxy) is _COMPONENT)
         self.assertEqual(component_proxy.__Security_checker__.get_permissions,
                          {'bar': 'testing'})
         self.assertEqual(action['args'][2], IFoo)
         self.assertEqual(action['args'][3], '')
         self.assertEqual(action['args'][4], 'TESTING')
         # Register the provided interface
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IFoo))
 
     @skipIfNoSecurity
     def test_w_factory_w_provides_w_permission(self):
         from zope.interface import Interface
+
         from zope.component.interface import provideInterface
         from zope.component.zcml import handler
+
         class IFoo(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, factory=Foo,
                       provides=IFoo, permission='testing')
         self.assertEqual(len(_cfg_ctx._actions), 2)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the utility
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'], ('utility', IFoo, ''))
         self.assertEqual(action['args'][0], 'registerUtility')
         self.assertEqual(action['args'][1], None)
         self.assertEqual(action['args'][2], IFoo)
         self.assertEqual(action['args'][3], '')
         self.assertEqual(action['args'][4], 'TESTING')
@@ -851,193 +940,220 @@
         # Factory is wrapped
         self.assertNotEqual(fctry, Foo)
         self.assertEqual(fctry.factory, Foo)
         secured = fctry()
         self.assertIsInstance(secured, Foo)
         # Register the provided interface
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IFoo))
 
 
 class Test_interface(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.component.zcml import interface
         return interface(*args, **kw)
 
     def test_wo_name_wo_type(self):
         from zope.interface import Interface
+
         from zope.component.interface import provideInterface
+
         class IFoo(Interface):
             pass
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, IFoo)
         self.assertEqual(len(_cfg_ctx._actions), 1)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IFoo, None))
 
     def test_w_name_w_type(self):
         from zope.interface import Interface
+
         from zope.component.interface import provideInterface
+
         class IFoo(Interface):
             pass
+
         class IBar(Interface):
             pass
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, IFoo, name='foo', type=IBar)
         self.assertEqual(len(_cfg_ctx._actions), 1)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('foo', IFoo, IBar))
 
 
 class Test_view(unittest.TestCase):
 
     def _callFUT(self, *args, **kw):
         from zope.component.zcml import view
         return view(*args, **kw)
 
     def test_w_allowed_interface_wo_permission(self):
         from zope.interface import Interface
+
         from zope.component.zcml import ComponentConfigurationError
+
         class IViewType(Interface):
             pass
+
         class IView(Interface):
             def foo():
                 "foo"
             def bar():
                 "bar"
-        class _View(object):
+        class _View:
             __init__ = fails_if_called(self)
             foo = fails_if_called(self)
             bar = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(ComponentConfigurationError,
                           self._callFUT, _cfg_ctx, (_View,), IViewType, '',
-                                         for_=(Interface, Interface),
-                                         allowed_interface=IView)
+                          for_=(Interface, Interface),
+                          allowed_interface=IView)
 
     def test_w_allowed_attributes_wo_permission(self):
         from zope.interface import Interface
+
         from zope.component.zcml import ComponentConfigurationError
+
         class IViewType(Interface):
             pass
-        class _View(object):
+
+        class _View:
             __init__ = fails_if_called(self)
             foo = fails_if_called(self)
             bar = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(ComponentConfigurationError,
                           self._callFUT, _cfg_ctx, (_View,), IViewType, '',
-                                         for_=(Interface, Interface),
-                                         allowed_attributes=('foo', 'bar'))
+                          for_=(Interface, Interface),
+                          allowed_attributes=('foo', 'bar'))
 
     def test_w_factory_as_empty(self):
         from zope.interface import Interface
+
         from zope.component.zcml import ComponentConfigurationError
+
         class IViewType(Interface):
             pass
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(ComponentConfigurationError,
                           self._callFUT, _cfg_ctx, (), IViewType, '',
-                                         for_=(Interface, Interface))
+                          for_=(Interface, Interface))
 
     def test_w_multiple_factory_multiple_for_(self):
         from zope.interface import Interface
+
         from zope.component.zcml import ComponentConfigurationError
+
         class IViewType(Interface):
             pass
-        class Foo(object):
+
+        class Foo:
             pass
-        class Bar(object):
+
+        class Bar:
             pass
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(ComponentConfigurationError,
                           self._callFUT, _cfg_ctx, (Foo, Bar), IViewType, '',
-                                         for_=(Interface, Interface))
+                          for_=(Interface, Interface))
 
     def test_w_for__as_empty(self):
         from zope.interface import Interface
+
         from zope.component.zcml import ComponentConfigurationError
+
         class IViewType(Interface):
             pass
-        class _View(object):
+
+        class _View:
             __init__ = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(ComponentConfigurationError,
                           self._callFUT, _cfg_ctx, (_View,), IViewType, '',
-                                         for_=())
+                          for_=())
 
     def test_w_single_factory_single_for__wo_permission_w_name(self):
         from zope.interface import Interface
-        from zope.component.zcml import handler
+
         from zope.component.interface import provideInterface
+        from zope.component.zcml import handler
+
         class IViewType(Interface):
             pass
-        class _View(object):
+
+        class _View:
             __init__ = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, (_View,), IViewType, 'test', for_=(Interface,))
         self.assertEqual(len(_cfg_ctx._actions), 4)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'],
                          ('view', (Interface, IViewType), 'test', Interface))
         self.assertEqual(action['args'][0], 'registerAdapter')
         self.assertEqual(action['args'][1], _View)
         self.assertEqual(action['args'][2], (Interface, IViewType))
         self.assertEqual(action['args'][3], Interface)
         self.assertEqual(action['args'][4], 'test')
         self.assertEqual(action['args'][5], 'TESTING')
         # Register the provided interface
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', Interface))
         # Register the required interface(s)
         self.assertEqual(_cfg_ctx._actions[2][0], ())
-        action =_cfg_ctx._actions[2][1]
+        action = _cfg_ctx._actions[2][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', Interface))
         self.assertEqual(_cfg_ctx._actions[3][0], ())
-        action =_cfg_ctx._actions[3][1]
+        action = _cfg_ctx._actions[3][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IViewType))
 
     def test_w_multiple_factory_single_for__wo_permission(self):
         from zope.interface import Interface
+
         from zope.component.zcml import handler
+
         class IViewType(Interface):
             pass
-        class _View(object):
+
+        class _View:
             def __init__(self, context):
                 self.context = context
-        class _View2(object):
+
+        class _View2:
             def __init__(self, context, request):
                 self.context = context
                 self.request = request
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, [_View, _View2], IViewType, '',
                       for_=(Interface,))
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'],
                          ('view', (Interface, IViewType), '', Interface))
         self.assertEqual(action['args'][0], 'registerAdapter')
         factory = action['args'][1]
         self.assertTrue(factory.factory is _View)
         context = object()
@@ -1051,27 +1167,30 @@
         self.assertEqual(action['args'][3], Interface)
         self.assertEqual(action['args'][4], '')
         self.assertEqual(action['args'][5], 'TESTING')
 
     @skipIfNoSecurity
     def test_w_single_factory_single_for__w_permission(self):
         from zope.interface import Interface
+
         from zope.component.zcml import handler
+
         class IViewType(Interface):
             pass
-        class _View(object):
+
+        class _View:
             def __init__(self, context, request):
                 self.context = context
                 self.request = request
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, [_View], IViewType, '', for_=(Interface,),
                       permission='testing')
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'],
                          ('view', (Interface, IViewType), '', Interface))
         self.assertEqual(action['args'][0], 'registerAdapter')
         factory = action['args'][1]
         context = object()
         request = object()
@@ -1083,50 +1202,55 @@
         self.assertEqual(action['args'][3], Interface)
         self.assertEqual(action['args'][4], '')
         self.assertEqual(action['args'][5], 'TESTING')
 
     @skipIfNoSecurity
     def test_w_single_factory_single_for__w_permission_and_allowed_attrs(self):
         from zope.interface import Interface
+
         from zope.component.zcml import handler
+
         class IViewType(Interface):
             pass
-        class _View(object):
+
+        class _View:
             __init__ = fails_if_called(self)
             bar = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, [_View], IViewType, '', for_=(Interface,),
                       permission='testing', allowed_attributes=('bar',))
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'],
                          ('view', (Interface, IViewType), '', Interface))
         self.assertEqual(action['args'][0], 'registerAdapter')
         factory = action['args'][1]
         checker = factory.checker
         self.assertEqual(checker.get_permissions, {'bar': 'testing'})
 
     @skipIfNoSecurity
     def test_w_single_factory_single_for__w_permission_and_allowed_iface(self):
         from zope.interface import Interface
+
         from zope.component.zcml import handler
+
         class IViewType(Interface):
             def bar(self):
                 "bar"
-        class _View(object):
+        class _View:
             __init__ = fails_if_called(self)
             bar = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, [_View], IViewType, '', for_=(Interface,),
                       permission='testing', allowed_interface=(IViewType,))
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the adapter
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'],
                          ('view', (Interface, IViewType), '', Interface))
         self.assertEqual(action['args'][0], 'registerAdapter')
         factory = action['args'][1]
         checker = factory.checker
         self.assertEqual(checker.get_permissions, {'bar': 'testing'})
@@ -1136,103 +1260,115 @@
 
     def _callFUT(self, *args, **kw):
         from zope.component.zcml import resource
         return resource(*args, **kw)
 
     def test_w_allowed_interface_wo_permission(self):
         from zope.interface import Interface
+
         from zope.component.zcml import ComponentConfigurationError
+
         class IResourceType(Interface):
             pass
+
         class IView(Interface):
             def foo():
                 "foo"
             def bar():
                 "bar"
-        class _Resource(object):
+        class _Resource:
             __init__ = fails_if_called(self)
             foo = fails_if_called(self)
             bar = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(ComponentConfigurationError,
                           self._callFUT,
-                            _cfg_ctx, (_Resource,), IResourceType, '',
-                            allowed_interface=IView)
+                          _cfg_ctx, (_Resource,), IResourceType, '',
+                          allowed_interface=IView)
 
     def test_w_allowed_attributes_wo_permission(self):
         from zope.interface import Interface
+
         from zope.component.zcml import ComponentConfigurationError
+
         class IResourceType(Interface):
             pass
-        class _Resource(object):
+
+        class _Resource:
             __init__ = fails_if_called(self)
             foo = fails_if_called(self)
             bar = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self.assertRaises(ComponentConfigurationError,
                           self._callFUT,
-                            _cfg_ctx, (_Resource,), IResourceType, '',
-                            allowed_attributes=('foo', 'bar'))
+                          _cfg_ctx, (_Resource,), IResourceType, '',
+                          allowed_attributes=('foo', 'bar'))
 
     def test_wo_permission_w_name(self):
         from zope.interface import Interface
+
         from zope.component.interface import provideInterface
         from zope.component.zcml import handler
+
         class IResourceType(Interface):
             pass
-        class _Resource(object):
+
+        class _Resource:
             __init__ = fails_if_called(self)
             foo = fails_if_called(self)
             bar = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, _Resource, IResourceType, 'test')
         self.assertEqual(len(_cfg_ctx._actions), 3)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the resource
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'],
                          ('resource', 'test', IResourceType, Interface))
         self.assertEqual(action['args'][0], 'registerAdapter')
         self.assertEqual(action['args'][1], _Resource)
         self.assertEqual(action['args'][2], (IResourceType,))
         self.assertEqual(action['args'][3], Interface)
         self.assertEqual(action['args'][4], 'test')
         self.assertEqual(action['args'][5], 'TESTING')
         # Register the 'type' interface
         self.assertEqual(_cfg_ctx._actions[1][0], ())
-        action =_cfg_ctx._actions[1][1]
+        action = _cfg_ctx._actions[1][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', IResourceType))
         # Register the required interface(s)
         self.assertEqual(_cfg_ctx._actions[2][0], ())
-        action =_cfg_ctx._actions[2][1]
+        action = _cfg_ctx._actions[2][1]
         self.assertEqual(action['callable'], provideInterface)
         self.assertEqual(action['discriminator'], None)
         self.assertEqual(action['args'], ('', Interface))
 
     @skipIfNoSecurity
     def test_w_permission(self):
         from zope.interface import Interface
+
         from zope.component.zcml import handler
+
         class IResourceType(Interface):
             pass
-        class _Resource(object):
+
+        class _Resource:
             def __init__(self, context):
                 self.context = context
             foo = fails_if_called(self)
             bar = fails_if_called(self)
         _cfg_ctx = _makeConfigContext()
         self._callFUT(_cfg_ctx, _Resource, IResourceType, 'test',
                       permission='testing', allowed_attributes=('foo',))
         self.assertEqual(len(_cfg_ctx._actions), 3)
         self.assertEqual(_cfg_ctx._actions[0][0], ())
         # Register the resource
-        action =_cfg_ctx._actions[0][1]
+        action = _cfg_ctx._actions[0][1]
         self.assertEqual(action['callable'], handler)
         self.assertEqual(action['discriminator'],
                          ('resource', 'test', IResourceType, Interface))
         self.assertEqual(action['args'][0], 'registerAdapter')
         factory = action['args'][1]
         self.assertTrue(factory.factory is _Resource)
         context = object()
@@ -1243,14 +1379,16 @@
         self.assertEqual(action['args'][2], (IResourceType,))
         self.assertEqual(action['args'][3], Interface)
         self.assertEqual(action['args'][4], 'test')
         self.assertEqual(action['args'][5], 'TESTING')
 
 
 def _makeConfigContext():
-    class _Context(object):
+    class _Context:
         info = 'TESTING'
+
         def __init__(self):
             self._actions = []
+
         def action(self, *args, **kw):
             self._actions.append((args, kw))
     return _Context()
```

### Comparing `zope.component-5.1.0/src/zope/component/zcml.py` & `zope.component-6.0/src/zope/component/zcml.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,87 +23,93 @@
 from zope.interface import Interface
 from zope.interface import implementedBy
 from zope.interface import providedBy
 from zope.schema import TextLine
 
 from zope.component._api import getSiteManager
 from zope.component._compat import ZOPE_SECURITY_NOT_AVAILABLE_EX
-from zope.component._declaration import adaptedBy, getName
+from zope.component._declaration import adaptedBy
+from zope.component._declaration import getName
 from zope.component.interface import provideInterface
 
+
 try:
     from zope.security.zcml import Permission
-except ZOPE_SECURITY_NOT_AVAILABLE_EX: # pragma: no cover
+except ZOPE_SECURITY_NOT_AVAILABLE_EX:  # pragma: no cover
     def _no_security(*args, **kw):
         raise ConfigurationError(
             "security proxied components are not "
             "supported because zope.security is not available")
     _checker = proxify = protectedFactory = security = _no_security
     Permission = TextLine
 else:
     from zope.component.security import _checker
-    from zope.component.security import proxify
     from zope.component.security import protectedFactory
+    from zope.component.security import proxify
     from zope.component.security import securityAdapterFactory
 
 _ = MessageFactory('zope')
 
+
 class ComponentConfigurationError(ValueError, ConfigurationError):
     pass
 
+
 def handler(methodName, *args, **kwargs):
     method = getattr(getSiteManager(), methodName)
     method(*args, **kwargs)
 
+
 class IBasicComponentInformation(Interface):
 
     component = GlobalObject(
         title=_("Component to use"),
         description=_("Python name of the implementation object.  This"
                       " must identify an object in a module using the"
                       " full dotted name.  If specified, the"
                       " ``factory`` field must be left blank."),
         required=False,
-        )
+    )
 
     permission = Permission(
         title=_("Permission"),
         description=_("Permission required to use this component."),
         required=False,
-        )
+    )
 
     factory = GlobalObject(
         title=_("Factory"),
         description=_("Python name of a factory which can create the"
                       " implementation object.  This must identify an"
                       " object in a module using the full dotted name."
                       " If specified, the ``component`` field must"
                       " be left blank."),
         required=False,
-        )
+    )
+
 
 class IAdapterDirective(Interface):
     """
     Register an adapter
     """
 
     factory = Tokens(
         title=_("Adapter factory/factories"),
         description=_("A list of factories (usually just one) that create"
                       " the adapter instance."),
         required=True,
         value_type=GlobalObject()
-        )
+    )
 
     provides = GlobalInterface(
         title=_("Interface the component provides"),
         description=_("This attribute specifies the interface the adapter"
                       " instance must provide."),
         required=False,
-        )
+    )
 
     for_ = Tokens(
         title=_("Specifications to be adapted"),
         description=_("This should be a list of interfaces or classes"),
         required=False,
         value_type=GlobalObject(
             missing_value=object(),
@@ -111,60 +117,62 @@
     )
 
     permission = Permission(
         title=_("Permission"),
         description=_("This adapter is only available, if the principal"
                       " has this permission."),
         required=False,
-        )
+    )
 
     name = TextLine(
         title=_("Name"),
         description=_("Adapters can have names.\n\n"
                       "This attribute allows you to specify the name for"
                       " this adapter."),
         required=False,
-        )
+    )
 
     trusted = Bool(
         title=_("Trusted"),
         description=_("""Make the adapter a trusted adapter
 
         Trusted adapters have unfettered access to the objects they
         adapt.  If asked to adapt security-proxied objects, then,
         rather than getting an unproxied adapter of security-proxied
         objects, you get a security-proxied adapter of unproxied
         objects.
         """),
         required=False,
         default=False,
-        )
+    )
 
     locate = Bool(
         title=_("Locate"),
         description=_("""Make the adapter a locatable adapter
 
         Located adapter should be used if a non-public permission
         is used.
         """),
         required=False,
         default=False,
-        )
+    )
+
 
 def _rolledUpFactory(factories):
     # This has to be named 'factory', aparently, so as not to confuse
     # apidoc :(
     def factory(ob):
         for f in factories:
             ob = f(ob)
         return ob
     # Store the original factory for documentation
     factory.factory = factories[0]
     return factory
 
+
 def adapter(_context, factory, provides=None, for_=None, permission=None,
             name='', trusted=False, locate=False):
 
     if for_ is None:
         if len(factory) == 1:
             for_ = adaptedBy(factory[0])
 
@@ -203,99 +211,103 @@
         factory = protectedFactory(factory, provides, permission)
 
     # invoke custom adapter factories
     if locate or permission is not None or trusted:
         factory = securityAdapterFactory(factory, permission, locate, trusted)
 
     _context.action(
-        discriminator = ('adapter', for_, provides, name),
-        callable = handler,
-        args = ('registerAdapter',
-                factory, for_, provides, name, _context.info),
-        )
+        discriminator=('adapter', for_, provides, name),
+        callable=handler,
+        args=('registerAdapter',
+              factory, for_, provides, name, _context.info),
+    )
     _context.action(
-        discriminator = None,
-        callable = provideInterface,
-        args = ('', provides)
-               )
+        discriminator=None,
+        callable=provideInterface,
+        args=('', provides)
+    )
     if for_:
         for iface in for_:
             if iface is not None:
                 _context.action(
-                    discriminator = None,
-                    callable = provideInterface,
-                    args = ('', iface)
-                    )
+                    discriminator=None,
+                    callable=provideInterface,
+                    args=('', iface)
+                )
+
 
 class ISubscriberDirective(Interface):
     """
     Register a subscriber
     """
 
     factory = GlobalObject(
         title=_("Subscriber factory"),
         description=_("A factory used to create the subscriber instance."),
         required=False,
-        )
+    )
 
     handler = GlobalObject(
         title=_("Handler"),
         description=_("A callable object that handles events."),
         required=False,
-        )
+    )
 
     provides = GlobalInterface(
         title=_("Interface the component provides"),
         description=_("This attribute specifies the interface the adapter"
                       " instance must provide."),
         required=False,
-        )
+    )
 
     for_ = Tokens(
         title=_("Interfaces or classes that this subscriber depends on"),
         description=_("This should be a list of interfaces or classes"),
         required=False,
         value_type=GlobalObject(
-          missing_value = object(),
-          ),
-        )
+            missing_value=object(),
+        ),
+    )
 
     permission = Permission(
         title=_("Permission"),
         description=_("This subscriber is only available, if the"
                       " principal has this permission."),
         required=False,
-        )
+    )
 
     trusted = Bool(
         title=_("Trusted"),
         description=_("""Make the subscriber a trusted subscriber
 
         Trusted subscribers have unfettered access to the objects they
         adapt.  If asked to adapt security-proxied objects, then,
         rather than getting an unproxied subscriber of security-proxied
         objects, you get a security-proxied subscriber of unproxied
         objects.
         """),
         required=False,
         default=False,
-        )
+    )
 
     locate = Bool(
         title=_("Locate"),
         description=_("""Make the subscriber a locatable subscriber
 
         Located subscribers should be used if a non-public permission
         is used.
         """),
         required=False,
         default=False,
-        )
+    )
+
 
 _handler = handler
+
+
 def subscriber(_context, for_=None, factory=None, handler=None, provides=None,
                permission=None, trusted=False, locate=False):
     if factory is None:
         if handler is None:
             raise TypeError("No factory or handler provided")
         if provides is not None:
             raise TypeError("Cannot use handler with provides")
@@ -325,58 +337,60 @@
 
     # invoke custom adapter factories
     if locate or permission is not None or trusted:
         factory = securityAdapterFactory(factory, permission, locate, trusted)
 
     if handler is not None:
         _context.action(
-            discriminator = None,
-            callable = _handler,
-            args = ('registerHandler',
-                    handler, for_, u'', _context.info),
-            )
+            discriminator=None,
+            callable=_handler,
+            args=('registerHandler',
+                  handler, for_, '', _context.info),
+        )
     else:
         _context.action(
-            discriminator = None,
-            callable = _handler,
-            args = ('registerSubscriptionAdapter',
-                    factory, for_, provides, u'', _context.info),
-            )
+            discriminator=None,
+            callable=_handler,
+            args=('registerSubscriptionAdapter',
+                  factory, for_, provides, '', _context.info),
+        )
 
     if provides is not None:
         _context.action(
-            discriminator = None,
-            callable = provideInterface,
-            args = ('', provides)
-            )
+            discriminator=None,
+            callable=provideInterface,
+            args=('', provides)
+        )
 
     # For each interface, state that the adapter provides that interface.
     for iface in for_:
         if iface is not None:
             _context.action(
-                discriminator = None,
-                callable = provideInterface,
-                args = ('', iface)
-                )
+                discriminator=None,
+                callable=provideInterface,
+                args=('', iface)
+            )
+
 
 class IUtilityDirective(IBasicComponentInformation):
     """Register a utility."""
 
     provides = GlobalInterface(
         title=_("Provided interface"),
         description=_("Interface provided by the utility."),
         required=False,
-        )
+    )
 
     name = TextLine(
         title=_("Name"),
         description=_("Name of the registration.  This is used by"
                       " application code when locating a utility."),
         required=False,
-        )
+    )
+
 
 def utility(_context, provides=None, component=None, factory=None,
             permission=None, name=''):
     if factory and component:
         raise TypeError("Can't specify factory and component.")
 
     if provides is None:
@@ -399,172 +413,176 @@
         if component:
             component = proxify(component, provides=provides,
                                 permission=permission)
         if factory:
             factory = protectedFactory(factory, provides, permission)
 
     _context.action(
-        discriminator = ('utility', provides, name),
-        callable = handler,
-        args = ('registerUtility', component, provides, name, _context.info),
-        kw = dict(factory=factory),
-        )
+        discriminator=('utility', provides, name),
+        callable=handler,
+        args=('registerUtility', component, provides, name, _context.info),
+        kw=dict(factory=factory),
+    )
     _context.action(
-        discriminator = None,
-        callable = provideInterface,
-        args = ('', provides),
-        )
+        discriminator=None,
+        callable=provideInterface,
+        args=('', provides),
+    )
+
 
 class IInterfaceDirective(Interface):
     """
     Define an interface
     """
 
     interface = GlobalInterface(
         title=_("Interface"),
         required=True,
-        )
+    )
 
     type = GlobalInterface(
         title=_("Interface type"),
         required=False,
-        )
+    )
 
     name = TextLine(
         title=_("Name"),
         required=False,
-        )
+    )
+
 
 def interface(_context, interface, type=None, name=''):
     _context.action(
-        discriminator = None,
-        callable = provideInterface,
-        args = (name, interface, type)
-        )
+        discriminator=None,
+        callable=provideInterface,
+        args=(name, interface, type)
+    )
+
 
 class IBasicViewInformation(Interface):
     """This is the basic information for all views."""
 
     for_ = Tokens(
         title=_("Specifications of the objects to be viewed"),
         description=_("""This should be a list of interfaces or classes
         """),
         required=True,
         value_type=GlobalObject(
-          missing_value=object(),
-          ),
-        )
+            missing_value=object(),
+        ),
+    )
 
     permission = Permission(
         title=_("Permission"),
         description=_("The permission needed to use the view."),
         required=False,
-        )
+    )
 
     class_ = GlobalObject(
         title=_("Class"),
         description=_("A class that provides attributes used by the view."),
         required=False,
-        )
+    )
 
     allowed_interface = Tokens(
         title=_("Interface that is also allowed if user has permission."),
         description=_("""
         By default, 'permission' only applies to viewing the view and
         any possible sub views. By specifying this attribute, you can
         make the permission also apply to everything described in the
         supplied interface.
 
         Multiple interfaces can be provided, separated by
         whitespace."""),
         required=False,
         value_type=GlobalInterface(),
-        )
+    )
 
     allowed_attributes = Tokens(
         title=_("View attributes that are also allowed if the user"
                 " has permission."),
         description=_("""
         By default, 'permission' only applies to viewing the view and
         any possible sub views. By specifying 'allowed_attributes',
         you can make the permission also apply to the extra attributes
         on the view object."""),
         required=False,
         value_type=PythonIdentifier(),
-        )
+    )
+
 
 class IBasicResourceInformation(Interface):
     """
     Basic information for resources
     """
 
     name = TextLine(
         title=_("The name of the resource."),
         description=_("The name shows up in URLs/paths. For example 'foo'."),
         required=True,
-        default=u'',
-        )
+        default='',
+    )
 
     provides = GlobalInterface(
         title=_("The interface this component provides."),
         description=_("""
         A view can provide an interface.  This would be used for
         views that support other views."""),
         required=False,
         default=Interface,
-        )
+    )
 
     type = GlobalInterface(
         title=_("Request type"),
         required=True
-        )
+    )
 
 
 class IViewDirective(IBasicViewInformation, IBasicResourceInformation):
     """Register a view for a component"""
 
     factory = Tokens(
         title=_("Factory"),
         required=False,
         value_type=GlobalObject(),
-        )
+    )
+
 
 def view(_context, factory, type, name, for_,
          permission=None,
          allowed_interface=None,
          allowed_attributes=None,
          provides=Interface,
-        ):
+         ):
 
     if ((allowed_attributes or allowed_interface)
-        and (not permission)):
+            and (not permission)):
         raise ComponentConfigurationError(
             "'permission' required with 'allowed_interface' or "
             "'allowed_attributes'")
 
     if permission is not None:
 
         checker = _checker(_context, permission,
                            allowed_interface, allowed_attributes)
 
-        class ProxyView(object):
+        class ProxyView:
             """Class to create simple proxy views."""
 
             def __init__(self, factory, checker):
                 self.factory = factory
                 self.checker = checker
 
             def __call__(self, *objects):
                 return proxify(self.factory(*objects), self.checker)
 
         factory[-1] = ProxyView(factory[-1], checker)
 
-
     if not for_:
-        raise ComponentConfigurationError("No for interfaces specified");
+        raise ComponentConfigurationError("No for interfaces specified")
     for_ = tuple(for_)
 
     # Generate a single factory from multiple factories:
     factories = factory
     if len(factories) == 1:
         factory = factories[0]
     elif len(factories) < 1:
@@ -578,82 +596,83 @@
                 ob = f(ob)
             return factories[-1](ob, request)
         factory.factory = factories[0]
 
     for_ = for_ + (type,)
 
     _context.action(
-        discriminator = ('view', for_, name, provides),
-        callable = handler,
-        args = ('registerAdapter',
-                factory, for_, provides, name, _context.info),
-        )
+        discriminator=('view', for_, name, provides),
+        callable=handler,
+        args=('registerAdapter',
+              factory, for_, provides, name, _context.info),
+    )
 
     _context.action(
-        discriminator = None,
-        callable = provideInterface,
-        args = ('', provides)
-        )
+        discriminator=None,
+        callable=provideInterface,
+        args=('', provides)
+    )
 
     if for_ is not None:
         for iface in for_:
             if iface is not None:
                 _context.action(
-                    discriminator = None,
-                    callable = provideInterface,
-                    args = ('', iface)
-                    )
+                    discriminator=None,
+                    callable=provideInterface,
+                    args=('', iface)
+                )
 
 
 class IResourceDirective(IBasicComponentInformation,
                          IBasicResourceInformation):
     """Register a resource"""
 
     allowed_interface = Tokens(
         title=_("Interface that is also allowed if user has permission."),
         required=False,
         value_type=GlobalInterface(),
-        )
+    )
 
     allowed_attributes = Tokens(
         title=_("View attributes that are also allowed if user"
                 " has permission."),
         required=False,
         value_type=PythonIdentifier(),
-        )
+    )
+
 
 def resource(_context, factory, type, name,
              permission=None,
              allowed_interface=None, allowed_attributes=None,
              provides=Interface):
 
     if ((allowed_attributes or allowed_interface)
-        and (not permission)):
+            and (not permission)):
         raise ComponentConfigurationError(
             "Must use name attribute with allowed_interface or "
             "allowed_attributes"
-            )
+        )
 
     if permission is not None:
 
         checker = _checker(_context, permission,
                            allowed_interface, allowed_attributes)
 
         def proxyResource(request, factory=factory, checker=checker):
             return proxify(factory(request), checker)
         proxyResource.factory = factory
 
         factory = proxyResource
 
     _context.action(
-        discriminator = ('resource', name, type, provides),
-        callable = handler,
-        args = ('registerAdapter',
-                factory, (type,), provides, name, _context.info))
+        discriminator=('resource', name, type, provides),
+        callable=handler,
+        args=('registerAdapter',
+              factory, (type,), provides, name, _context.info))
     _context.action(
-        discriminator = None,
-        callable = provideInterface,
-        args = ('', type))
+        discriminator=None,
+        callable=provideInterface,
+        args=('', type))
     _context.action(
-        discriminator = None,
-        callable = provideInterface,
-        args = ('', provides))
+        discriminator=None,
+        callable=provideInterface,
+        args=('', provides))
```

### Comparing `zope.component-5.1.0/src/zope.component.egg-info/PKG-INFO` & `zope.component-6.0/src/zope.component.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 Metadata-Version: 2.1
 Name: zope.component
-Version: 5.1.0
+Version: 6.0
 Summary: Zope Component Architecture
 Home-page: https://github.com/zopefoundation/zope.component
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Documentation, https://zopecomponent.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.component/issues
 Project-URL: Sources, https://github.com/zopefoundation/zope.component
 Keywords: interface component coupling loose utility adapter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: Zope :: 3
+Classifier: Framework :: Zope :: 5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: hook
 Provides-Extra: persistentregistry
 Provides-Extra: security
 Provides-Extra: zcml
 Provides-Extra: mintests
 Provides-Extra: test
 Provides-Extra: docs
@@ -79,14 +76,20 @@
 
 .. _zope.interface: https://github.com/zopefoundation/zope.interface
 
 =========
  Changes
 =========
 
+6.0 (2023-04-14)
+================
+
+
+
+- Drop support for Python 2.7, 3.5, 3.6.
 
 5.1.0 (2023-01-03)
 ==================
 
 - Fix crash when the environment variable `PYTHONOPTIMIZED` is set to `2`
   and docstrings are set to `None` by the interpreter.
   (`#67 <https://github.com/zopefoundation/zope.component/issues/67>`_)
```

### Comparing `zope.component-5.1.0/src/zope.component.egg-info/SOURCES.txt` & `zope.component-6.0/src/zope.component.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
 buildout.cfg
 rtd.txt
 setup.cfg
```

### Comparing `zope.component-5.1.0/tox.ini` & `zope.component-6.0/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,96 @@
+# Generated from:
+# https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
-    py27
-    py35
-    py36
+    lint
     py37
     py38
     py39
     py310
     py311
-    py27-minimal
-    py310-optimized
-    pypy
     pypy3
     docs
     coverage
+    py310-optimized
 
-[mindeps]
+[testenv]
+usedevelop = true
 deps =
-    .[mintests]
+setenv =
+    ZOPE_INTERFACE_STRICT_IRO=1
+    optimized: PYTHONOPTIMIZE=2
+commands =
+    zope-testrunner --test-path=src {posargs:-vc}
+    sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
+extras =
+    test
+    docs
 
-[fulldeps]
+[testenv:lint]
+basepython = python3
+skip_install = true
+commands =
+    isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
+    flake8 src setup.py
+    check-manifest
+    check-python-versions
 deps =
-    .[test]
-
-[testenv]
-usedevelop = true
+    check-manifest
+    check-python-versions >= 0.19.1
+    wheel
+    flake8
+    isort
+
+[testenv:isort-apply]
+basepython = python3
+skip_install = true
+commands_pre =
 deps =
-    !minimal: {[fulldeps]deps}
-    minimal: {[mindeps]deps}
-    .[docs]
+    isort
 commands =
-# Temporary workaround. Avoid zope.testrunner pending
-# IRO fixes in zope.security. https://github.com/zopefoundation/zope.security/issues/71
-    python -m unittest discover -s src
-    !minimal: sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
-setenv =
-    ZOPE_INTERFACE_STRICT_IRO = 1
-    pure: PURE_PYTHON = 1
-    optimized: PYTHONOPTIMIZE = 2
+    isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:docs]
-basepython =
-    python3
+basepython = python3
+skip_install = false
+commands_pre =
 commands =
     sphinx-build -b html -d docs/_build/doctrees docs docs/_build/html
     sphinx-build -b doctest -d docs/_build/doctrees docs docs/_build/doctest
-deps =
-    {[fulldeps]deps}
-    .[docs]
-setenv =
-    ZOPE_INTERFACE_STRICT_IRO = 0
 
 [testenv:coverage]
-basepython =
-    python3
-usedevelop = true
-commands =
-    coverage run -m unittest discover -s src
-    coverage run -a -m sphinx -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
-    coverage report --fail-under=99
+basepython = python3
+allowlist_externals =
+    mkdir
 deps =
-    {[testenv]deps}
     coverage
-    coverage-python-version
+commands =
+    mkdir -p {toxinidir}/parts/htmlcov
+    coverage run -m zope.testrunner --test-path=src {posargs:-vc}
+    coverage run -a -m sphinx -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=99.5
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.component
 omit =
-    # Runs in a subprocess
+    # Runs in a subprocess:
     src/zope/component/standalonetests.py
-    # Not used
-    src/zope/component/hookable.py
+    # Not used:
     src/zope/component/eventtesting.py
 
 [coverage:report]
+precision = 2
 exclude_lines =
     pragma: no cover
-    pragma NO COVER
-    if __name__ == '__main__':
+    pragma: nocover
+    except ImportError:
     raise NotImplementedError
+    if __name__ == '__main__':
     self.fail
+    raise AssertionError
+
+[coverage:html]
+directory = parts/htmlcov
```

