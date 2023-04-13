# Comparing `tmp/plone.app.iterate-5.0.1.tar.gz` & `tmp/plone.app.iterate-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.iterate-5.0.1.tar", last modified: Tue Mar 21 23:15:42 2023, max compression
+gzip compressed data, was "plone.app.iterate-5.0.2.tar", last modified: Thu Apr 13 22:50:23 2023, max compression
```

## Comparing `plone.app.iterate-5.0.1.tar` & `plone.app.iterate-5.0.2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.104580 plone.app.iterate-5.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)    13616 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    18057 2023-03-21 23:15:42.104707 plone.app.iterate-5.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3453 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.082074 plone.app.iterate-5.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      679 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4019 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/docs/developer.txt
--rw-r--r--   0 maurits    (501) staff       (20)      649 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/docs/install.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2248 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/docs/references.txt
--rw-r--r--   0 maurits    (501) staff       (20)      755 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/docs/todo.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5119 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/docs/workflow.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.082323 plone.app.iterate-5.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)      269 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.084987 plone.app.iterate-5.0.1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)      269 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.088338 plone.app.iterate-5.0.1/plone/app/iterate/
--rw-r--r--   0 maurits    (501) staff       (20)     1362 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1930 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/archiver.py
--rw-r--r--   0 maurits    (501) staff       (20)     5822 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/base.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.093242 plone.app.iterate-5.0.1/plone/app/iterate/browser/
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      324 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/cancel.png
--rw-r--r--   0 maurits    (501) staff       (20)     1493 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/cancel.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2411 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/cancel.py
--rw-r--r--   0 maurits    (501) staff       (20)      296 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/checkin.png
--rw-r--r--   0 maurits    (501) staff       (20)     2138 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/checkin.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2407 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/checkin.py
--rw-r--r--   0 maurits    (501) staff       (20)      545 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/checkout.png
--rw-r--r--   0 maurits    (501) staff       (20)     2785 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/checkout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3653 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/checkout.py
--rw-r--r--   0 maurits    (501) staff       (20)     2258 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3317 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/control.py
--rw-r--r--   0 maurits    (501) staff       (20)     5256 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/diff.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1046 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/diff.py
--rw-r--r--   0 maurits    (501) staff       (20)     4450 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/info.py
--rw-r--r--   0 maurits    (501) staff       (20)     1035 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/info_baseline.pt
--rw-r--r--   0 maurits    (501) staff       (20)      900 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/browser/info_checkout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4052 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2462 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/containers.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.095306 plone.app.iterate-5.0.1/plone/app/iterate/dexterity/
--rw-r--r--   0 maurits    (501) staff       (20)       72 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/dexterity/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      960 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/dexterity/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9997 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/dexterity/copier.py
--rw-r--r--   0 maurits    (501) staff       (20)      247 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/dexterity/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2808 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/dexterity/policy.py
--rw-r--r--   0 maurits    (501) staff       (20)     1055 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/dexterity/relation.py
--rw-r--r--   0 maurits    (501) staff       (20)     1606 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/dexterity/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2660 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/event.py
--rw-r--r--   0 maurits    (501) staff       (20)     8160 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1630 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/lock.py
--rw-r--r--   0 maurits    (501) staff       (20)     1296 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/permissions.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.077784 plone.app.iterate-5.0.1/plone/app/iterate/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.096314 plone.app.iterate-5.0.1/plone/app/iterate/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)     2032 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/default/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)       71 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      119 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/default/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.097136 plone.app.iterate-5.0.1/plone/app/iterate/profiles/test/
--rw-r--r--   0 maurits    (501) staff       (20)      152 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/test/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.097499 plone.app.iterate-5.0.1/plone/app/iterate/profiles/test/portal_placeful_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)      340 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/test/portal_placeful_workflow/working-copy.xml
--rw-r--r--   0 maurits    (501) staff       (20)      275 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/test/portal_placeful_workflow.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.077212 plone.app.iterate-5.0.1/plone/app/iterate/profiles/test/workflows/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.097754 plone.app.iterate-5.0.1/plone/app/iterate/profiles/test/workflows/workingcopy_workflow/
--rw-r--r--   0 maurits    (501) staff       (20)     8031 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/test/workflows/workingcopy_workflow/definition.xml
--rw-r--r--   0 maurits    (501) staff       (20)      179 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/test/workflows.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.098424 plone.app.iterate-5.0.1/plone/app/iterate/profiles/testingdx/
--rw-r--r--   0 maurits    (501) staff       (20)      242 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/testingdx/repositorytool.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.098765 plone.app.iterate-5.0.1/plone/app/iterate/profiles/testingdx/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2495 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/testingdx/types/FolderishDocument.xml
--rw-r--r--   0 maurits    (501) staff       (20)      156 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/testingdx/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.099051 plone.app.iterate-5.0.1/plone/app/iterate/profiles/to1000/
--rw-r--r--   0 maurits    (501) staff       (20)      710 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/to1000/actions.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.100010 plone.app.iterate-5.0.1/plone/app/iterate/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      393 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/uninstall/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)       71 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/uninstall/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      133 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/profiles/uninstall/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      775 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/setuphandlers.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.102102 plone.app.iterate-5.0.1/plone/app/iterate/subscribers/
--rw-r--r--   0 maurits    (501) staff       (20)       78 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/subscribers/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1670 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/subscribers/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1928 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/subscribers/locking.py
--rw-r--r--   0 maurits    (501) staff       (20)     1552 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/subscribers/marker.py
--rw-r--r--   0 maurits    (501) staff       (20)     1462 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/subscribers/metadata.py
--rw-r--r--   0 maurits    (501) staff       (20)     1318 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/subscribers/versioning.py
--rw-r--r--   0 maurits    (501) staff       (20)     3025 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/subscribers/workflow.py
--rw-r--r--   0 maurits    (501) staff       (20)     2526 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.104378 plone.app.iterate-5.0.1/plone/app/iterate/tests/
--rw-r--r--   0 maurits    (501) staff       (20)       26 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2290 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/tests/dexterity.rst
--rw-r--r--   0 maurits    (501) staff       (20)      435 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/tests/dxtypes.py
--rw-r--r--   0 maurits    (501) staff       (20)     2795 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/tests/test_annotations.py
--rw-r--r--   0 maurits    (501) staff       (20)    12064 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/tests/test_containers.py
--rw-r--r--   0 maurits    (501) staff       (20)      567 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     3637 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/tests/test_interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    12076 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/tests/test_iterate.py
--rw-r--r--   0 maurits    (501) staff       (20)     1354 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone/app/iterate/util.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 23:15:42.084740 plone.app.iterate-5.0.1/plone.app.iterate.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    18057 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone.app.iterate.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3288 2023-03-21 23:15:42.000000 plone.app.iterate-5.0.1/plone.app.iterate.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone.app.iterate.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone.app.iterate.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone.app.iterate.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone.app.iterate.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      395 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone.app.iterate.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/plone.app.iterate.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      116 2023-03-21 23:15:42.105200 plone.app.iterate-5.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2168 2023-03-21 23:15:41.000000 plone.app.iterate-5.0.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.067074 plone.app.iterate-5.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)    13723 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    18164 2023-04-13 22:50:23.067216 plone.app.iterate-5.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3453 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.044389 plone.app.iterate-5.0.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      679 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4021 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/docs/developer.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      649 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/docs/install.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2248 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/docs/references.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      755 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/docs/todo.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     5119 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/docs/workflow.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.044697 plone.app.iterate-5.0.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.047502 plone.app.iterate-5.0.2/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.051246 plone.app.iterate-5.0.2/plone/app/iterate/
+-rw-r--r--   0 maurits    (501) staff       (20)     1132 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1897 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/archiver.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5782 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/base.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.056338 plone.app.iterate-5.0.2/plone/app/iterate/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      324 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/cancel.png
+-rw-r--r--   0 maurits    (501) staff       (20)     1802 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/cancel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2383 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/cancel.py
+-rw-r--r--   0 maurits    (501) staff       (20)      296 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/checkin.png
+-rw-r--r--   0 maurits    (501) staff       (20)     2471 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/checkin.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2380 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/checkin.py
+-rw-r--r--   0 maurits    (501) staff       (20)      545 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/checkout.png
+-rw-r--r--   0 maurits    (501) staff       (20)     3140 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/checkout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3626 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/checkout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2133 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3293 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/control.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6073 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/diff.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      965 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/diff.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4347 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/info.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1065 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/info_baseline.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      913 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/browser/info_checkout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4146 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2420 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/containers.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.058477 plone.app.iterate-5.0.2/plone/app/iterate/dexterity/
+-rw-r--r--   0 maurits    (501) staff       (20)       47 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/dexterity/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      921 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/dexterity/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9965 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/dexterity/copier.py
+-rw-r--r--   0 maurits    (501) staff       (20)      223 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/dexterity/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2784 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/dexterity/policy.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1031 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/dexterity/relation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1582 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/dexterity/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2611 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/event.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8017 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1557 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/lock.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1273 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/permissions.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.039742 plone.app.iterate-5.0.2/plone/app/iterate/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.059357 plone.app.iterate-5.0.2/plone/app/iterate/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)     2372 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/default/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       88 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      134 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/default/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.060245 plone.app.iterate-5.0.2/plone/app/iterate/profiles/test/
+-rw-r--r--   0 maurits    (501) staff       (20)      191 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/test/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.060525 plone.app.iterate-5.0.2/plone/app/iterate/profiles/test/portal_placeful_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)      346 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/test/portal_placeful_workflow/working-copy.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      309 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/test/portal_placeful_workflow.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.039082 plone.app.iterate-5.0.2/plone/app/iterate/profiles/test/workflows/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.060819 plone.app.iterate-5.0.2/plone/app/iterate/profiles/test/workflows/workingcopy_workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)     8195 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/test/workflows/workingcopy_workflow/definition.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      196 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/test/workflows.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.061403 plone.app.iterate-5.0.2/plone/app/iterate/profiles/testingdx/
+-rw-r--r--   0 maurits    (501) staff       (20)      237 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/testingdx/repositorytool.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.061675 plone.app.iterate-5.0.2/plone/app/iterate/profiles/testingdx/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2671 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/testingdx/types/FolderishDocument.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      194 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/testingdx/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.061949 plone.app.iterate-5.0.2/plone/app/iterate/profiles/to1000/
+-rw-r--r--   0 maurits    (501) staff       (20)      864 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/to1000/actions.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.062747 plone.app.iterate-5.0.2/plone/app/iterate/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      480 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/uninstall/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       88 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/uninstall/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      161 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/profiles/uninstall/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      746 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/setuphandlers.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.064724 plone.app.iterate-5.0.2/plone/app/iterate/subscribers/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/subscribers/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1591 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/subscribers/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1844 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/subscribers/locking.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1469 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/subscribers/marker.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1377 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/subscribers/metadata.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1285 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/subscribers/versioning.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2913 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/subscribers/workflow.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2336 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.066875 plone.app.iterate-5.0.2/plone/app/iterate/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2293 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/tests/dexterity.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      411 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/tests/dxtypes.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2757 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/tests/test_annotations.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11998 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/tests/test_containers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      567 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3531 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/tests/test_interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12012 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/tests/test_iterate.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1330 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone/app/iterate/util.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:50:23.047194 plone.app.iterate-5.0.2/plone.app.iterate.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    18164 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone.app.iterate.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3288 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone.app.iterate.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone.app.iterate.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone.app.iterate.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone.app.iterate.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone.app.iterate.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      467 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone.app.iterate.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/plone.app.iterate.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1687 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-13 22:50:23.067676 plone.app.iterate-5.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2282 2023-04-13 22:50:22.000000 plone.app.iterate-5.0.2/setup.py
```

### Comparing `plone.app.iterate-5.0.1/CHANGES.rst` & `plone.app.iterate-5.0.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.2 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5623f8b3)
+
+
 5.0.1 (2023-03-22)
 ------------------
 
 Bug fixes:
 
 
 - Use proper action icons in Plone 6.
@@ -373,15 +383,15 @@
 3.1.0 (2015-07-18)
 ------------------
 
 - Merge plone.app.stagingbehavior into plone.app.iterate without the
   behavior implementation. This is for Plone 5 iterate support.
   [vangheem]
 
-- Don't remove aquisition on object for getToolByName call.
+- Don't remove acquisition on object for getToolByName call.
   [tomgross]
 
 
 3.0.1 (2015-03-12)
 ------------------
 
 - Add permission names zcml/z3 style and load permission settings explicit
@@ -420,15 +430,15 @@
 - Replaced the "Locked" label with "Warning"
   [rristow]
 
 
 2.1.11 (2014-01-27)
 -------------------
 
-- setted lock timeout to MAX_TIMEOUT to avoid baseline unwanted unlock after 10 minutes
+- set lock timeout to MAX_TIMEOUT to avoid baseline unwanted unlock after 10 minutes
   [parruc]
 
 
 2.1.10 (2013-03-05)
 -------------------
 
 - Fixed error on checking in the working copy of an object linked in it's
```

### Comparing `plone.app.iterate-5.0.1/PKG-INFO` & `plone.app.iterate-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.iterate
-Version: 5.0.1
+Version: 5.0.2
 Summary: check-out/check-in staging for Plone
 Home-page: https://pypi.org/project/plone.app.iterate
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: check-out check-in staging
 Classifier: Development Status :: 5 - Production/Stable
@@ -132,14 +132,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.2 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5623f8b3)
+
+
 5.0.1 (2023-03-22)
 ------------------
 
 Bug fixes:
 
 
 - Use proper action icons in Plone 6.
@@ -501,15 +511,15 @@
 3.1.0 (2015-07-18)
 ------------------
 
 - Merge plone.app.stagingbehavior into plone.app.iterate without the
   behavior implementation. This is for Plone 5 iterate support.
   [vangheem]
 
-- Don't remove aquisition on object for getToolByName call.
+- Don't remove acquisition on object for getToolByName call.
   [tomgross]
 
 
 3.0.1 (2015-03-12)
 ------------------
 
 - Add permission names zcml/z3 style and load permission settings explicit
@@ -548,15 +558,15 @@
 - Replaced the "Locked" label with "Warning"
   [rristow]
 
 
 2.1.11 (2014-01-27)
 -------------------
 
-- setted lock timeout to MAX_TIMEOUT to avoid baseline unwanted unlock after 10 minutes
+- set lock timeout to MAX_TIMEOUT to avoid baseline unwanted unlock after 10 minutes
   [parruc]
 
 
 2.1.10 (2013-03-05)
 -------------------
 
 - Fixed error on checking in the working copy of an object linked in it's
```

### Comparing `plone.app.iterate-5.0.1/README.rst` & `plone.app.iterate-5.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.iterate-5.0.1/docs/LICENSE.GPL` & `plone.app.iterate-5.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.iterate-5.0.1/docs/LICENSE.txt` & `plone.app.iterate-5.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.iterate-5.0.1/docs/developer.txt` & `plone.app.iterate-5.0.2/docs/developer.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
  Baseline
    the original version of the content object, that the checkout was performed on.
 
  Working Copy (WC)
    a copy of the baseline, placed in a selectable container.
 
 The default policy adapter its meant to be easily subclassed, see policy.py for details,
-it does however have alot of responsibilities and maintains a series of invariants which
+it does however have a lot of responsibilities and maintains a series of invariants which
 any replacement must also maintain, described below. if your business logic can be
 encapsulated in an event subscriber it is much better to integrate it via that mechanism.
 
 A policy's adapter adaptation context is a content object, by registered for by default
 AT IBaseObject. Adapter configuration changes can be specified via zcml.
 
 Checkin/Checkout Invariants
@@ -59,15 +59,15 @@
 
 When a working copy is checked out a dav lock is taken out on the baseline, to prevent
 mutation of the baseline. other forms of locking are available, but dav locks are the only common
 infrastructure between different frameworks. this means currently only one checkout of
 a given content object at a time.
 
 A custom reference class ( see relation.py ) is used to track
-bookeeping information regarding the checkout via the archetypes
+bookkeeping information regarding the checkout via the archetypes
 reference engine, and to serve as an annotation property bag to
 store (custom) information about the checkout. it is utilized as a
 reference between the working copy to the baseline ( backref wc ).
 
 Reference Adapters
 ------------------
```

### Comparing `plone.app.iterate-5.0.1/docs/install.txt` & `plone.app.iterate-5.0.2/docs/install.txt`

 * *Files identical despite different names*

### Comparing `plone.app.iterate-5.0.1/docs/references.txt` & `plone.app.iterate-5.0.2/docs/references.txt`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 copied to the working copy, but would be kept when the working copy is checked in. this
 adapter also keeps reference state.
 
 
 Backreferences
 --------------
 
-Developers utilizing semantically signifigant backreferences that can
+Developers utilizing semantically significant backreferences that can
 be modified on the working copy are expected to write a custom
 reference adapter ( see ICheckinCheckoutReference in interfaces.py )
 with implementations for checkoutBackReference and
 checkinBackReference, the default adapter implementation does nothing with
 backreferences.
 
 Custom Reference Adapters
```

### Comparing `plone.app.iterate-5.0.1/docs/todo.txt` & `plone.app.iterate-5.0.2/docs/todo.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ----
 Todo
 ----
 
 Short Term
 ----------
 
- - always increment version on checkout (iff doc is not upto date )
+ - always increment version on checkout (if doc is not up to date )
    - better offer form option.
 
  - default event adapter for setting workflow on checked out content
 
  - refactor policy, move all invariants to event subscribers
    [ locking, event marking, versioning ]
```

### Comparing `plone.app.iterate-5.0.1/docs/workflow.txt` & `plone.app.iterate-5.0.2/docs/workflow.txt`

 * *Files identical despite different names*

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/__init__.py` & `plone.app.iterate-5.0.2/plone/app/iterate/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -16,27 +15,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with iterate; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 ##################################################################
-"""
-"""
-
-from plone.app.iterate import permissions  # noqa
+from plone.app.iterate import permissions  # noqa: F401
 from zope.i18nmessageid import MessageFactory
 
 import logging
 
 
 PloneMessageFactory = MessageFactory("plone")
 logger = logging.getLogger("plone.app.iterate")
-
-
-try:
-    import plone.app.relationfield  # noqa
-except ImportError:
-    logger.warn(
-        "Dexterity support for iterate is not available. "
-        "You must install plone.app.relationfield"
-    )
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/archiver.py` & `plone.app.iterate-5.0.2/plone/app/iterate/archiver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006-2007 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -16,24 +15,23 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with CMFDeployment; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 ##################################################################
+from . import interfaces
 from Products.CMFCore.utils import getToolByName
 from zope.component import adapter
 from zope.interface import implementer
 
-from . import interfaces
-
 
 @implementer(interfaces.IObjectArchiver)
 @adapter(interfaces.IIterateAware)
-class ContentArchiver(object):
+class ContentArchiver:
     def __init__(self, context):
         self.context = context
         self.repository = getToolByName(context, "portal_repository")
 
     def save(self, checkin_message):
         self.repository.save(self.context, checkin_message)
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/base.py` & `plone.app.iterate-5.0.2/plone/app/iterate/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006-2007 ObjectRealms, LLC
 # (C) Copyright 2007-2017 Plone Foundation
 # All Rights Reserved
 #
 # This file is part of iterate.
@@ -41,15 +40,15 @@
 from zope import component
 from zope.component import queryAdapter
 from zope.event import notify
 from zope.interface import implementer
 
 
 @implementer(ICheckinCheckoutPolicy)
-class CheckinCheckoutBasePolicyAdapter(object):
+class CheckinCheckoutBasePolicyAdapter:
     """Base Checkin Checkout Policy For Content
 
     - on checkout context is the baseline
     - on checkin context is the working copy.
 
     """
 
@@ -107,15 +106,15 @@
 
     def getProperties(self, obj, default=None):
         return get_storage(obj, default=default)
 
 
 @implementer(interfaces.IObjectCopier)
 @component.adapter(interfaces.IIterateAware)
-class BaseContentCopier(object):
+class BaseContentCopier:
     def __init__(self, context):
         self.context = context
 
     def _recursivelyReattachUIDs(self, baseline, new_baseline):
         original_refs = len(new_baseline.getRefs())
         original_back_refs = len(new_baseline.getBRefs())
         new_baseline._setUID(baseline.UID())
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/cancel.pt` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/cancel.pt`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,61 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-    xmlns:tal="http://xml.zope.org/namespaces/tal"
-    xmlns:metal="http://xml.zope.org/namespaces/metal"
-    xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    metal:use-macro="context/main_template/macros/master"
-    i18n:domain="plone">
-<body>
-
-<metal:content fill-slot="content">
-<metal:content define-macro="content">
-<article id="content">
-    <form action="#"
-        method="post"
-        tal:attributes="action string:${context/absolute_url}/@@content-cancel-checkout">
-
-      <h1 class="documentFirstHeading"
-          i18n:translate="title_cancel">
-        Cancel check-out of <span i18n:name="object_title" tal:content="context/Title" />.
-      </h1>
+<html xmlns="http://www.w3.org/1999/xhtml"
+      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      metal:use-macro="context/main_template/macros/master"
+      xml:lang="en"
+      i18n:domain="plone"
+>
+  <body>
+
+    <metal:content fill-slot="content">
+      <metal:content define-macro="content">
+        <article id="content">
+          <form action="#"
+                method="post"
+                tal:attributes="
+                  action string:${context/absolute_url}/@@content-cancel-checkout;
+                "
+          >
+
+            <h1 class="documentFirstHeading"
+                i18n:translate="title_cancel"
+            >
+        Cancel check-out of
+              <span tal:content="context/Title"
+                    i18n:name="object_title"
+              ></span>.
+            </h1>
 
-      <p i18n:translate="description_cancel">
+            <p i18n:translate="description_cancel">
         Canceling the check-out will delete this working copy, and any modifications
         made to it will be lost. The existing version of the content will become
         unlocked.
-      </p>
+            </p>
 
-      <div class="formControls">
+            <div class="formControls">
 
-        <input
-            class="destructive"
-            type="submit"
-            name="form.button.Cancel"
-            value="Cancel checkout"
-            i18n:attributes="value"
-            />
-
-        <input
-            class="standalone"
-            type="submit"
-            name="form.button.Keep"
-            value="Keep checkout"
-            i18n:attributes="value"
-            />
-
-      </div>
-
-    </form>
-</article>
-</metal:content>
-</metal:content>
+              <input class="destructive"
+                     name="form.button.Cancel"
+                     type="submit"
+                     value="Cancel checkout"
+                     i18n:attributes="value"
+              />
+
+              <input class="standalone"
+                     name="form.button.Keep"
+                     type="submit"
+                     value="Keep checkout"
+                     i18n:attributes="value"
+              />
+
+            </div>
+
+          </form>
+        </article>
+      </metal:content>
+    </metal:content>
 
-</body>
-</html>
+  </body>
+</html>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/cancel.py` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/cancel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -28,31 +27,30 @@
 from Products.Five.browser import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from Products.statusmessages.interfaces import IStatusMessage
 from zope.component import getMultiAdapter
 
 
 class Cancel(BrowserView):
-
     index = ViewPageTemplateFile("cancel.pt")
 
     def __call__(self):
         context = aq_inner(self.context)
 
         if "form.button.Cancel" in self.request.form:
-            control = getMultiAdapter((context, self.request), name=u"iterate_control")
+            control = getMultiAdapter((context, self.request), name="iterate_control")
             if not control.cancel_allowed():
-                raise CheckoutException(u"Not a checkout")
+                raise CheckoutException("Not a checkout")
 
             policy = ICheckinCheckoutPolicy(context)
             baseline = policy.cancelCheckout()
             baseline.reindexObject()
 
             IStatusMessage(self.request).addStatusMessage(
-                _(u"Checkout cancelled"), type="info"
+                _("Checkout cancelled"), type="info"
             )
             view_url = baseline.restrictedTraverse("@@plone_context_state").view_url()
             self.request.response.redirect(view_url)
         elif "form.button.Keep" in self.request.form:
             view_url = context.restrictedTraverse("@@plone_context_state").view_url()
             self.request.response.redirect(view_url)
         else:
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/checkin.pt` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/checkin.pt`

 * *Files 5% similar despite different names*

```diff
@@ -1,72 +1,83 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-    xmlns:tal="http://xml.zope.org/namespaces/tal"
-    xmlns:metal="http://xml.zope.org/namespaces/metal"
-    xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    metal:use-macro="context/main_template/macros/master"
-    i18n:domain="plone">
-<body>
-
-<metal:content fill-slot="content">
-<metal:content define-macro="content">
-<article id="content">
-
-    <form action="#"
-        method="post"
-        tal:attributes="action string:${context/absolute_url}/@@content-checkin">
-
-    <h1 class="documentFirstHeading"
-        i18n:translate="title_checkin">
-        Check in <span i18n:name="object_title" tal:content="here/Title" />
-    </h1>
+<html xmlns="http://www.w3.org/1999/xhtml"
+      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      metal:use-macro="context/main_template/macros/master"
+      xml:lang="en"
+      i18n:domain="plone"
+>
+  <body>
+
+    <metal:content fill-slot="content">
+      <metal:content define-macro="content">
+        <article id="content">
+
+          <form action="#"
+                method="post"
+                tal:attributes="
+                  action string:${context/absolute_url}/@@content-checkin;
+                "
+          >
+
+            <h1 class="documentFirstHeading"
+                i18n:translate="title_checkin"
+            >
+        Check in
+              <span tal:content="here/Title"
+                    i18n:name="object_title"
+              ></span>
+            </h1>
 
-    <p i18n:translate="description_checkin">
+            <p i18n:translate="description_checkin">
         Checking in this working copy will replace the existing item
         with the working copy.
-    </p>
+            </p>
 
-    <fieldset>
+            <fieldset>
 
-            <div class="field">
-              <label for="description"
-                    i18n:translate="label_checkin_message">Check-in Message
-               </label>
-
-              <div class="formHelp" i18n:translate="help_checkin_message">
+              <div class="field">
+                <label for="description"
+                       i18n:translate="label_checkin_message"
+                >Check-in Message
+                </label>
+
+                <div class="formHelp"
+                     i18n:translate="help_checkin_message"
+                >
                   Enter a message to be saved alongside the check-in. This
                   should explain what was changed, for audit purposes.
+                </div>
+
+                <textarea id="checkin_message"
+                          cols="60"
+                          name="checkin_message"
+                          rows="3"
+                ></textarea>
               </div>
 
-              <textarea cols="60"
-                        rows="3"
-                        id="checkin_message"
-                        name="checkin_message"></textarea>
-            </div>
-
-            <div class="formControls">
-                <input
-                    class="context"
-                    type="submit"
-                    name="form.button.Checkin"
-                    value="Check in"
-                    i18n:attributes="value"
-                    />
-
-                <input
-                    class="standalone"
-                    type="submit"
-                    name="form.button.Cancel"
-                    value="Cancel"
-                    i18n:attributes="value label_cancel"
-                    />
-            </div>
-
-    </fieldset>
-
-    </form>
-</article>
-</metal:content>
-</metal:content>
+              <div class="formControls">
+                <input class="context"
+                       name="form.button.Checkin"
+                       type="submit"
+                       value="Check in"
+                       i18n:attributes="value"
+                />
+
+                <input class="standalone"
+                       name="form.button.Cancel"
+                       type="submit"
+                       value="Cancel"
+                       i18n:attributes="value label_cancel"
+                />
+              </div>
+
+            </fieldset>
+
+          </form>
+        </article>
+      </metal:content>
+    </metal:content>
 
-</body>
-</html>
+  </body>
+</html>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/checkin.py` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/checkin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -28,24 +27,23 @@
 from Products.Five.browser import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from Products.statusmessages.interfaces import IStatusMessage
 from zope.component import getMultiAdapter
 
 
 class Checkin(BrowserView):
-
     index = ViewPageTemplateFile("checkin.pt")
 
     def __call__(self):
         context = aq_inner(self.context)
 
         if "form.button.Checkin" in self.request.form:
-            control = getMultiAdapter((context, self.request), name=u"iterate_control")
+            control = getMultiAdapter((context, self.request), name="iterate_control")
             if not control.checkin_allowed():
-                raise CheckinException(u"Not a checkout")
+                raise CheckinException("Not a checkout")
 
             message = self.request.form.get("checkin_message", "")
 
             policy = ICheckinCheckoutPolicy(context)
             baseline = policy.checkin(message)
 
             IStatusMessage(self.request).addStatusMessage(_("Checked in"), type="info")
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/checkout.png` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/checkout.png`

 * *Files identical despite different names*

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/checkout.pt` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/checkout.pt`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,114 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-    xmlns:tal="http://xml.zope.org/namespaces/tal"
-    xmlns:metal="http://xml.zope.org/namespaces/metal"
-    xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    metal:use-macro="context/main_template/macros/master"
-    i18n:domain="plone">
-<body>
-
-<div id="content" metal:fill-slot="body"
-     tal:define="containers python:list(view.containers())">
-
-    <form action="#"
-        method="post"
-        name="checkout"
-        tal:attributes="action string:${context/absolute_url}/@@content-checkout">
-
-    <h1 i18n:translate="title_checkout">
-        Check out <span i18n:name="object_title" tal:content="here/Title" />
-    </h1>
+<html xmlns="http://www.w3.org/1999/xhtml"
+      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      metal:use-macro="context/main_template/macros/master"
+      xml:lang="en"
+      i18n:domain="plone"
+>
+  <body>
+
+    <div id="content"
+         metal:fill-slot="body"
+         tal:define="
+           containers python:list(view.containers());
+         "
+    >
+
+      <form action="#"
+            method="post"
+            name="checkout"
+            tal:attributes="
+              action string:${context/absolute_url}/@@content-checkout;
+            "
+      >
+
+        <h1 i18n:translate="title_checkout">
+        Check out
+          <span tal:content="here/Title"
+                i18n:name="object_title"
+          ></span>
+        </h1>
 
-    <p i18n:translate="description_checkout">
+        <p i18n:translate="description_checkout">
         On check-out, a working copy of the content item will be created in the selected
         container, and the original will be locked to prevent other users from
         editing it.
-    </p>
+        </p>
 
-    <tal:one_container tal:condition="python:len(containers)==1">
-    <input
-        type="hidden"
-        name="checkout_location"
-        tal:define = "item python:containers[0]"
-        tal:attributes="id string:checkout_location_${item/name};
-                        value item/name"
-        />
-    </tal:one_container>
-
-    <fieldset tal:condition="python:len(containers)!=1">
-
-        <legend i18n:translate="legend_details">Details</legend>
-
-            <div class="field">
-
-            <label for="checkout_folder" i18n:translate="label_checkout_folder">
+        <tal:one_container tal:condition="python:len(containers)==1">
+          <input name="checkout_location"
+                 type="hidden"
+                 tal:define="
+                   item python:containers[0];
+                 "
+                 tal:attributes="
+                   id string:checkout_location_${item/name};
+                   value item/name;
+                 "
+          />
+        </tal:one_container>
+
+        <fieldset tal:condition="python:len(containers)!=1">
+
+          <legend i18n:translate="legend_details">Details</legend>
+
+          <div class="field">
+
+            <label for="checkout_folder"
+                   i18n:translate="label_checkout_folder"
+            >
                 Checkout Folder
             </label>
-            <div class="formHelp" i18n:translate="help_checkout_folder">
+            <div class="formHelp"
+                 i18n:translate="help_checkout_folder"
+            >
                 Select the folder to checkout to.
             </div>
 
             <div tal:repeat="item view/containers">
 
-                <input
-                    type="radio"
-                    name="checkout_location"
-                    tal:attributes="id string:checkout_location_${item/name};
-                                    value item/name"
-                    />
-
-                <label
-                    tal:attributes="for string:checkout_location_${item/name}"
-                    tal:content="item/locator/title"
-                    />
-
-           </div>
+              <input name="checkout_location"
+                     type="radio"
+                     tal:attributes="
+                       id string:checkout_location_${item/name};
+                       value item/name;
+                     "
+              />
+
+              <label tal:content="item/locator/title"
+                     tal:attributes="
+                       for string:checkout_location_${item/name};
+                     "
+              ></label>
 
             </div>
 
+          </div>
+
         </fieldset>
 
         <div class="formControls">
 
-            <input
-                class="context"
-                type="submit"
-                name="form.button.Checkout"
-                value="Check out"
-                i18n:attributes="value"
-                />
-
-            <input
-                class="standalone"
-                type="submit"
-                name="form.button.Cancel"
-                value="Cancel"
-                i18n:attributes="value label_cancel"
-                />
+          <input class="context"
+                 name="form.button.Checkout"
+                 type="submit"
+                 value="Check out"
+                 i18n:attributes="value"
+          />
+
+          <input class="standalone"
+                 name="form.button.Cancel"
+                 type="submit"
+                 value="Cancel"
+                 i18n:attributes="value label_cancel"
+          />
 
         </div>
 
-    </form>
+      </form>
 
-</div>
+    </div>
 
-</html>
+  </body></html>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/checkout.py` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/checkout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -30,15 +29,14 @@
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from Products.statusmessages.interfaces import IStatusMessage
 from zope.component import getAdapters
 from zope.component import getMultiAdapter
 
 
 class Checkout(BrowserView):
-
     index = ViewPageTemplateFile("checkout.pt")
 
     def containers(self):
         """Get a list of potential containers"""
         context = aq_inner(self.context)
         for name, locator in getAdapters((context,), IWCContainerLocator):
             if locator.available:
@@ -46,17 +44,17 @@
 
     def __call__(self):
         context = aq_inner(self.context)
 
         # We want to redirect to a specific template, else we might
         # end up downloading a file
         if "form.button.Checkout" in self.request.form:
-            control = getMultiAdapter((context, self.request), name=u"iterate_control")
+            control = getMultiAdapter((context, self.request), name="iterate_control")
             if not control.checkout_allowed():
-                raise CheckoutException(u"Not allowed")
+                raise CheckoutException("Not allowed")
 
             location = self.request.form.get("checkout_location", None)
             locator = None
             try:
                 locator = [
                     c["locator"] for c in self.containers() if c["name"] == location
                 ][0]
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/configure.zcml` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/configure.zcml`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:browser="http://namespaces.zope.org/browser">
+    xmlns:browser="http://namespaces.zope.org/browser"
+    >
 
-    <!-- Control view (public) -->
+  <!-- Control view (public) -->
 
-    <browser:page
-        for="*"
-        name="iterate_control"
-        class=".control.Control"
-        permission="zope2.View"
-        allowed_attributes="checkin_allowed checkout_allowed cancel_allowed"
-        />
-
-    <!-- Forms -->
-
-    <browser:page
-        for="..interfaces.IIterateAware"
-        name="content-checkout"
-        class=".checkout.Checkout"
-        template="checkout.pt"
-        permission="zope2.View"
-        />
-
-    <browser:page
-        for="..interfaces.IIterateAware"
-        name="content-checkin"
-        class=".checkin.Checkin"
-        template="checkin.pt"
-        permission="cmf.ModifyPortalContent"
-        />
-
-    <browser:page
-        for="..interfaces.IIterateAware"
-        name="content-cancel-checkout"
-        class=".cancel.Cancel"
-        template="cancel.pt"
-        permission="cmf.ModifyPortalContent"
-        />
-
-    <!-- Information -->
-
-    <browser:page
-       for="..interfaces.IIterateManagedContent"
-       class=".diff.DiffView"
-       name="iterate_diff"
-       template="diff.pt"
-       permission="zope2.View"
-       />
-
-    <browser:viewlet
-        name="plone.app.iterate.baseline_info"
-        manager="plone.app.layout.viewlets.interfaces.IAboveContent"
-        class=".info.BaselineInfoViewlet"
-        permission="zope2.View"
-        for="..interfaces.IBaseline"
-        view="plone.app.layout.globals.interfaces.IViewView"
-        />
-
-    <browser:viewlet
-        name="plone.app.iterate.checkout_info"
-        manager="plone.app.layout.viewlets.interfaces.IAboveContent"
-        class=".info.CheckoutInfoViewlet"
-        permission="zope2.View"
-        for="..interfaces.IWorkingCopy"
-        view="plone.app.layout.globals.interfaces.IViewView"
-        />
-
-    <!-- Resources -->
-    <!-- These resources are deprecated.  Remove them in Plone 7. -->
-    <browser:resource
-        name="checkin.png"
-        image="checkin.png"
-        />
-
-    <browser:resource
-        name="checkout.png"
-        image="checkout.png"
-        />
-
-    <browser:resource
-        name="cancel-checkout.png"
-        image="cancel.png"
-        />
+  <browser:page
+      name="iterate_control"
+      for="*"
+      class=".control.Control"
+      allowed_attributes="checkin_allowed checkout_allowed cancel_allowed"
+      permission="zope2.View"
+      />
+
+  <!-- Forms -->
+
+  <browser:page
+      name="content-checkout"
+      for="..interfaces.IIterateAware"
+      class=".checkout.Checkout"
+      template="checkout.pt"
+      permission="zope2.View"
+      />
+
+  <browser:page
+      name="content-checkin"
+      for="..interfaces.IIterateAware"
+      class=".checkin.Checkin"
+      template="checkin.pt"
+      permission="cmf.ModifyPortalContent"
+      />
+
+  <browser:page
+      name="content-cancel-checkout"
+      for="..interfaces.IIterateAware"
+      class=".cancel.Cancel"
+      template="cancel.pt"
+      permission="cmf.ModifyPortalContent"
+      />
+
+  <!-- Information -->
+
+  <browser:page
+      name="iterate_diff"
+      for="..interfaces.IIterateManagedContent"
+      class=".diff.DiffView"
+      template="diff.pt"
+      permission="zope2.View"
+      />
+
+  <browser:viewlet
+      name="plone.app.iterate.baseline_info"
+      for="..interfaces.IBaseline"
+      view="plone.app.layout.globals.interfaces.IViewView"
+      manager="plone.app.layout.viewlets.interfaces.IAboveContent"
+      class=".info.BaselineInfoViewlet"
+      permission="zope2.View"
+      />
+
+  <browser:viewlet
+      name="plone.app.iterate.checkout_info"
+      for="..interfaces.IWorkingCopy"
+      view="plone.app.layout.globals.interfaces.IViewView"
+      manager="plone.app.layout.viewlets.interfaces.IAboveContent"
+      class=".info.CheckoutInfoViewlet"
+      permission="zope2.View"
+      />
+
+  <!-- Resources -->
+  <!-- These resources are deprecated.  Remove them in Plone 7. -->
+  <browser:resource
+      name="checkin.png"
+      image="checkin.png"
+      />
+
+  <browser:resource
+      name="checkout.png"
+      image="checkout.png"
+      />
+
+  <browser:resource
+      name="cancel-checkout.png"
+      image="cancel.png"
+      />
 
 </configure>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/control.py` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/diff.pt` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/diff.pt`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,181 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
 "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en-US" lang="en-US"
-    metal:use-macro="context/main_template/macros/master"
-    i18n:domain="plone">
+<html xmlns="http://www.w3.org/1999/xhtml"
+      lang="en-US"
+      metal:use-macro="context/main_template/macros/master"
+      xml:lang="en-US"
+      i18n:domain="plone"
+>
 
-<tal:block metal:fill-slot="base">
+  <tal:block metal:fill-slot="base">
     <base href=""
-          tal:define="current_page_url context/@@plone_context_state/current_page_url"
-          tal:attributes="href current_page_url" />
-</tal:block>
-<tal:block metal:fill-slot="head_slot">
-    <link rel="stylesheet" type="text/css" href="compare.css"
-          tal:attributes="href string:${portal_url}/compare.css"/>
-</tal:block>
-
-<body>
-  <metal:main metal:fill-slot="main"
-       tal:define="diffs view/diffs;
-                   diff_url string:${context/absolute_url}/@@iterate_diff">
-
-    <h1 class="documentFirstHeading" i18n:translate="">
+          tal:define="
+            current_page_url context/@@plone_context_state/current_page_url;
+          "
+          tal:attributes="
+            href current_page_url;
+          "
+    />
+  </tal:block>
+  <tal:block metal:fill-slot="head_slot">
+    <link href="compare.css"
+          rel="stylesheet"
+          type="text/css"
+          tal:attributes="
+            href string:${portal_url}/compare.css;
+          "
+    />
+  </tal:block>
+
+  <body>
+    <metal:main metal:fill-slot="main"
+                tal:define="
+                  diffs view/diffs;
+                  diff_url string:${context/absolute_url}/@@iterate_diff;
+                "
+    >
+
+      <h1 class="documentFirstHeading"
+          i18n:translate=""
+      >
         Changes to
-        <span tal:replace="context/title_or_id" i18n:name="title"/>
-    </h1>
-
-    <div id="content-core">
-        <em tal:condition="diffs/same" i18n:translate="">
+        <span tal:replace="context/title_or_id"
+              i18n:name="title"
+        ></span>
+      </h1>
+
+      <div id="content-core">
+        <em tal:condition="diffs/same"
+            i18n:translate=""
+        >
             No significant changes found.
         </em>
 
         <div tal:condition="not:diffs/same">
-            <div metal:use-macro="context/diff_legend/macros/diff_legend" />
+          <div metal:use-macro="context/diff_legend/macros/diff_legend"></div>
 
-            <form id="diffs"
-                  action="#"
-                  tal:repeat="d diffs/getDiffs">
-              <div class="field"
-                   tal:condition="not:d/same"
-                   tal:define="field_label d/label;
-                               unified exists:d/unified_diff;
-                               html exists:d/html_diff;
-                               inline exists:d/inline_diff;
-                               ndiff exists:d/ndiff;
-                               inline python: inline and not request.get('no_inline', 0);
-                               html python: html and not request.get('show_unified', 0)">
-                <label tal:content="field_label" />
-
-                <tal:html condition="inline">
-                    <br />
-                    <a href="#"
-                       tal:attributes="href string:${diff_url}?no_inline:int=1" i18n:translate="">Show code differences</a>
-                    <br />
-                    <br />
-                    <div class="inline-diff"
-                         tal:content="structure d/inline_diff">[inline diff]</div>
-                </tal:html>
-                <tal:html condition="python: html and not inline">
-                    <br />
-                    <tal:visual-only tal:condition="exists:d/inline_diff">
-                        <a href="#"
-                           tal:attributes="href string:${diff_url}" i18n:translate="">Show visual differences</a>
-                        <br />
-                    </tal:visual-only>
-                    <a href="#"
-                       tal:attributes="href string:${diff_url}?no_inline:int=1&amp;show_unified:int=1" i18n:translate="">Unified diff format</a>
-                    <pre tal:content="structure d/html_diff">[html diff]</pre>
-                </tal:html>
-                <tal:unified condition="python:unified and not html">
-                    <br />
-                    <a href="#"
-                        tal:condition="exists:d/inline_diff"
-                        tal:attributes="href string:${diff_url}" i18n:translate="">Show visual differences</a>
-                    <br />
-                    <a href="#"
-                       tal:condition="exists:d/html_diff"
-                       tal:attributes="href string:${diff_url}?no_inline:int=1" i18n:translate="">Show side by side</a>
-                    <pre tal:content="d/unified_diff">[unified diff]</pre>
-                </tal:unified>
-                <tal:ndiff condition="python:ndiff and not (unified or html)">
-                    <pre tal:content="d/ndiff">[ndiff]</pre>
-                </tal:ndiff>
-                <tal:nodiff condition="python:not (unified or html or ndiff)">
-                    <span class="diff_chg" i18n:translate="">Field Changed</span>
-                    <br /><br />
-                </tal:nodiff>
-              </div>
-            </form>
+          <form id="diffs"
+                action="#"
+                tal:repeat="d diffs/getDiffs"
+          >
+            <div class="field"
+                 tal:define="
+                   field_label d/label;
+                   unified exists:d/unified_diff;
+                   html exists:d/html_diff;
+                   inline exists:d/inline_diff;
+                   ndiff exists:d/ndiff;
+                   inline python: inline and not request.get('no_inline', 0);
+                   html python: html and not request.get('show_unified', 0);
+                 "
+                 tal:condition="not:d/same"
+            >
+              <label tal:content="field_label"></label>
+
+              <tal:html condition="inline">
+                <br />
+                <a href="#"
+                   tal:attributes="
+                     href string:${diff_url}?no_inline:int=1;
+                   "
+                   i18n:translate=""
+                >Show code differences</a>
+                <br />
+                <br />
+                <div class="inline-diff"
+                     tal:content="structure d/inline_diff"
+                >[inline diff]</div>
+              </tal:html>
+              <tal:html condition="python: html and not inline">
+                <br />
+                <tal:visual-only tal:condition="exists:d/inline_diff">
+                  <a href="#"
+                     tal:attributes="
+                       href string:${diff_url};
+                     "
+                     i18n:translate=""
+                  >Show visual differences</a>
+                  <br />
+                </tal:visual-only>
+                <a href="#"
+                   tal:attributes="
+                     href string:${diff_url}?no_inline:int=1&amp;show_unified:int=1;
+                   "
+                   i18n:translate=""
+                >Unified diff format</a>
+                <pre tal:content="structure d/html_diff">[html diff]</pre>
+              </tal:html>
+              <tal:unified condition="python:unified and not html">
+                <br />
+                <a href="#"
+                   tal:condition="exists:d/inline_diff"
+                   tal:attributes="
+                     href string:${diff_url};
+                   "
+                   i18n:translate=""
+                >Show visual differences</a>
+                <br />
+                <a href="#"
+                   tal:condition="exists:d/html_diff"
+                   tal:attributes="
+                     href string:${diff_url}?no_inline:int=1;
+                   "
+                   i18n:translate=""
+                >Show side by side</a>
+                <pre tal:content="d/unified_diff">[unified diff]</pre>
+              </tal:unified>
+              <tal:ndiff condition="python:ndiff and not (unified or html)">
+                <pre tal:content="d/ndiff">[ndiff]</pre>
+              </tal:ndiff>
+              <tal:nodiff condition="python:not (unified or html or ndiff)">
+                <span class="diff_chg"
+                      i18n:translate=""
+                >Field Changed</span>
+                <br /><br />
+              </tal:nodiff>
+            </div>
+          </form>
         </div>
 
         <tal:block tal:condition="diffs/recursive">
-        <h2 i18n:translate="">Changed files</h2>
-        <i tal:condition="not:diffs/getSubDiffs">None</i>
-        <ul tal:condition="diffs/getSubDiffs">
+          <h2 i18n:translate="">Changed files</h2>
+          <i tal:condition="not:diffs/getSubDiffs">None</i>
+          <ul tal:condition="diffs/getSubDiffs">
             <li tal:repeat="cs diffs/getSubDiffs">
-                <tal:check condition="not:cs/same">
-                    <a tal:content="cs/id" tal:attributes="href cs/id">[filename]</a>
-               </tal:check>
-           </li>
-        </ul>
-
-        <h2 i18n:translate="">Removed files</h2>
-        <em tal:condition="not:diffs/getRemovedItems" i18n:translate="">None</em>
-        <ul tal:condition="diffs/getRemovedItems">
-        <li tal:repeat="id diffs/getRemovedItems" tal:content="id">[filename]</li>
-        </ul>
-
-        <h2 i18n:translate="">Added files</h2>
-        <em tal:condition="not:diffs/getAddedItems" i18n:translate="">None</em>
-        <ul tal:condition="diffs/getAddedItems">
-        <li tal:repeat="id diffs/getAddedItems"><a tal:content="id" tal:attributes="href id">[filename]</a></li>
-        </ul>
+              <tal:check condition="not:cs/same">
+                <a tal:content="cs/id"
+                   tal:attributes="
+                     href cs/id;
+                   "
+                >[filename]</a>
+              </tal:check>
+            </li>
+          </ul>
+
+          <h2 i18n:translate="">Removed files</h2>
+          <em tal:condition="not:diffs/getRemovedItems"
+              i18n:translate=""
+          >None</em>
+          <ul tal:condition="diffs/getRemovedItems">
+            <li tal:repeat="id diffs/getRemovedItems"
+                tal:content="id"
+            >[filename]</li>
+          </ul>
+
+          <h2 i18n:translate="">Added files</h2>
+          <em tal:condition="not:diffs/getAddedItems"
+              i18n:translate=""
+          >None</em>
+          <ul tal:condition="diffs/getAddedItems">
+            <li tal:repeat="id diffs/getAddedItems"><a tal:content="id"
+                 tal:attributes="
+                   href id;
+                 "
+              >[filename]</a></li>
+          </ul>
         </tal:block>
-    </div>
-  </metal:main>
-</body>
+      </div>
+    </metal:main>
+  </body>
 </html>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/diff.py` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/diff.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-# -*- coding: utf-8 -*-
-"""
-$Id: diff.py 1807 2007-02-06 06:52:46Z hazmat $
-"""
-
 from plone.app.iterate.interfaces import IBaseline
 from plone.app.iterate.interfaces import ICheckinCheckoutPolicy
 from plone.app.iterate.interfaces import IWorkingCopy
 from Products.CMFCore.utils import getToolByName
 from Products.Five.browser import BrowserView
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/info.py` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# -*- coding: utf-8 -*-
-"""
-$Id: base.py 1808 2007-02-06 11:39:11Z hazmat $
-"""
-
 from AccessControl import getSecurityManager
 from DateTime import DateTime
 from plone.app.iterate.interfaces import IBaseline
 from plone.app.iterate.interfaces import ICheckinCheckoutPolicy
 from plone.app.iterate.interfaces import keys
 from plone.app.iterate.permissions import CheckoutPermission
 from plone.memoize.instance import memoize
 from Products.CMFCore.permissions import ModifyPortalContent
 from Products.CMFCore.utils import getToolByName
-from Products.CMFPlone.log import logger
 from Products.Five.browser import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from zope.interface import implementer
 from zope.viewlet.interfaces import IViewlet
 
+import logging
+
+
+logger = logging.getLogger("Plone")
+
 
 @implementer(IViewlet)
 class BaseInfoViewlet(BrowserView):
     def __init__(self, context, request, view, manager):
-        super(BaseInfoViewlet, self).__init__(context, request)
+        super().__init__(context, request)
         self.__parent__ = view
         self.view = view
         self.manager = manager
 
     def update(self):
         pass
 
@@ -57,15 +56,15 @@
         return membership.getMemberById(user_id)
 
     @memoize
     def creator_url(self):
         creator = self.creator()
         if creator is not None:
             portal_url = getToolByName(self.context, "portal_url")
-            return "{0}/author/{1}".format(portal_url(), creator.getId())
+            return f"{portal_url()}/author/{creator.getId()}"
 
     @memoize
     def creator_name(self):
         creator = self.creator()
         if creator is not None:
             return creator.getProperty("fullname") or creator.getId()
         # User is not known by PAS. This may be due to LDAP issues, so we keep
@@ -95,15 +94,14 @@
             return {}
 
     def _getReference(self):
         raise NotImplementedError
 
 
 class BaselineInfoViewlet(BaseInfoViewlet):
-
     index = ViewPageTemplateFile("info_baseline.pt")
 
     def render(self):
         sm = getSecurityManager()
         working_copy = self.working_copy()
         if working_copy is not None and (
             sm.checkPermission(ModifyPortalContent, self.context)
@@ -119,15 +117,14 @@
         return self.policy.getWorkingCopy()
 
     def _getReference(self):
         return self.working_copy()
 
 
 class CheckoutInfoViewlet(BaseInfoViewlet):
-
     index = ViewPageTemplateFile("info_checkout.pt")
 
     def render(self):
         sm = getSecurityManager()
         baseline = self.baseline()
         if baseline is not None and (
             sm.checkPermission(ModifyPortalContent, self.context)
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/info_baseline.pt` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/info_baseline.pt`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,40 @@
 <div class="portalMessage warning"
-     tal:define="working_copy view/working_copy;
-                 isAnon context/@@plone_portal_state/anonymous;"
+     tal:define="
+       working_copy view/working_copy;
+       isAnon context/@@plone_portal_state/anonymous;
+     "
+     tal:condition="python: not isAnon"
      i18n:domain="plone"
-     tal:condition="python: not isAnon">
+>
 
-    <strong i18n:translate="">Warning</strong>
-    <tal:block i18n:translate="working_copy_info">
+  <strong i18n:translate="">Warning</strong>
+  <tal:block i18n:translate="working_copy_info">
         This item is being edited by
-        <a i18n:name="creator"
-           tal:attributes="href view/creator_url"
-           tal:omit-tag="not: view/creator_url"
-           tal:content="view/creator_name">john smith</a>
+    <a tal:content="view/creator_name"
+       tal:omit-tag="not: view/creator_url"
+       tal:attributes="
+         href view/creator_url;
+       "
+       i18n:name="creator"
+    >john smith</a>
         in
-        <a i18n:name="working_copy"
-           i18n:translate="label_working_copy"
-           tal:attributes="href working_copy/@@plone_context_state/view_url;
-                           title working_copy/Description">a working copy</a>
+    <a tal:attributes="
+         href working_copy/@@plone_context_state/view_url;
+         title working_copy/Description;
+       "
+       i18n:name="working_copy"
+       i18n:translate="label_working_copy"
+    >a working copy</a>
         created on
-        <span i18n:name="created" tal:content="view/created"/>.
+    <span tal:content="view/created"
+          i18n:name="created"
+    ></span>.
 
-    </tal:block>
+  </tal:block>
 
-    (<a i18n:translate="label_view_changes"
-         tal:attributes="href string:${context/absolute_url}/@@iterate_diff">View changes</a>)
+  (<a tal:attributes="
+       href string:${context/absolute_url}/@@iterate_diff;
+     "
+     i18n:translate="label_view_changes"
+  >View changes</a>)
 </div>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/browser/info_checkout.pt` & `plone.app.iterate-5.0.2/plone/app/iterate/browser/info_checkout.pt`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 <div class="portalMessage info"
-     tal:define="baseline view/baseline;"
-     i18n:domain="plone">
+     tal:define="
+       baseline view/baseline;
+     "
+     i18n:domain="plone"
+>
 
-    <strong i18n:translate="">Warning</strong>
-    <tal:block i18n:translate="checkout_info">
+  <strong i18n:translate="">Warning</strong>
+  <tal:block i18n:translate="checkout_info">
 
         This is a working copy of
-        <a i18n:name="baseline_title"
-            tal:attributes="href baseline/@@plone_context_state/view_url;
-                            title baseline/Description"
-            tal:content="baseline/Title"/>, made by
-
-        <a i18n:name="creator"
-            tal:attributes="href view/creator_url"
-            tal:omit-tag="not: view/creator_url"
-            tal:content="view/creator_name">john smith</a>
+    <a tal:content="baseline/Title"
+       tal:attributes="
+         href baseline/@@plone_context_state/view_url;
+         title baseline/Description;
+       "
+       i18n:name="baseline_title"
+    ></a>, made by
+
+    <a tal:content="view/creator_name"
+       tal:omit-tag="not: view/creator_url"
+       tal:attributes="
+         href view/creator_url;
+       "
+       i18n:name="creator"
+    >john smith</a>
 
         on
 
-        <span
-            i18n:name="created"
-            tal:content="view/created"/>.
-    </tal:block>
-
-    (<a i18n:translate="view_changes"
-         tal:attributes="href string:${context/absolute_url}/@@iterate_diff">View changes</a>)
+    <span tal:content="view/created"
+          i18n:name="created"
+    ></span>.
+  </tal:block>
+
+  (<a tal:attributes="
+       href string:${context/absolute_url}/@@iterate_diff;
+     "
+     i18n:translate="view_changes"
+  >View changes</a>)
 </div>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/configure.zcml` & `plone.app.iterate-5.0.2/plone/app/iterate/configure.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -1,100 +1,114 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:five="http://namespaces.zope.org/five"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     xmlns:zcml="http://namespaces.zope.org/zcml"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
-  <include package="Products.CMFCore" file="meta.zcml"/>
-  <include package="Products.GenericSetup" file="meta.zcml"/>
-  <include package="zope.component" file="meta.zcml"/>
-  <include package="zope.viewlet" file="meta.zcml"/>
+  <include
+      package="Products.CMFCore"
+      file="meta.zcml"
+      />
+  <include
+      package="Products.GenericSetup"
+      file="meta.zcml"
+      />
+  <include
+      package="zope.component"
+      file="meta.zcml"
+      />
+  <include
+      package="zope.viewlet"
+      file="meta.zcml"
+      />
 
   <include package="plone.locking" />
   <include package="plone.memoize" />
   <include package="Products.CMFCore" />
   <include package="Products.CMFEditions" />
   <include package="Products.CMFPlacefulWorkflow" />
   <include package="Products.DCWorkflow" />
   <include package="Products.GenericSetup" />
   <include package="Products.statusmessages" />
   <include package="zope.annotation" />
   <include package="zope.component" />
   <include package="zope.viewlet" />
 
-  <include package=".subscribers"/>
-  <include package=".browser"/>
+  <include package=".subscribers" />
+  <include package=".browser" />
+  <include package=".dexterity" />
 
   <genericsetup:registerProfile
-    name="default"
-    title="Working Copy Support (Iterate)"
-    directory="profiles/default"
-    description="Adds working copy support (aka. in-place staging) to Plone."
-    provides="Products.GenericSetup.interfaces.EXTENSION"
-    />
+      name="default"
+      title="Working Copy Support (Iterate)"
+      description="Adds working copy support (aka. in-place staging) to Plone."
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/default"
+      />
 
   <!--
-    Remove, when CMFPlone no more depends on this profile.
-    Products.CMFPlone/Products/CMFPlone/MigrationTool.py:99:
-    Addon(profile_id=u'plone.app.iterate:plone.app.iterate')
+    The plone.app.iterate:plone.app.iterate profile is deprecated.
+    Remove either in Plone 6.1 or 7.0, I am on the fence here.
+    See https://github.com/plone/plone.app.iterate/issues/99#issuecomment-1484686642
   -->
   <genericsetup:registerProfile
-    name="plone.app.iterate"
-    title="Working Copy Support (Iterate)"
-    directory="profiles/default"
-    description="Adds working copy support (aka. in-place staging) to Plone."
-    provides="Products.GenericSetup.interfaces.EXTENSION"
-    post_handler=".setuphandlers.deprecate_profile"
-    />
+      name="plone.app.iterate"
+      title="Working Copy Support (Iterate)"
+      description="Adds working copy support (aka. in-place staging) to Plone."
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/default"
+      post_handler=".setuphandlers.deprecate_profile"
+      />
 
   <genericsetup:registerProfile
       name="test"
       title="plone.app.iterate: Test fixture"
-      directory="profiles/test"
       description="Extension profile to configure a test fixture"
-      for="Products.CMFPlone.interfaces.ITestCasePloneSiteRoot"
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      for="plone.base.interfaces.ITestCasePloneSiteRoot"
+      directory="profiles/test"
       />
 
   <genericsetup:registerProfile
       name="testingdx"
       title="plone.app.iterate: Test fixture for DX"
-      directory="profiles/testingdx"
       description="Adds sample content types for testing"
       provides="Products.GenericSetup.interfaces.EXTENSION"
-      for="Products.CMFPlone.interfaces.ITestCasePloneSiteRoot"
+      for="plone.base.interfaces.ITestCasePloneSiteRoot"
+      directory="profiles/testingdx"
       />
 
   <genericsetup:registerProfile
       name="uninstall"
       title="Working Copy Support (Iterate) [uninstall]"
-      directory="profiles/uninstall"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       for="plone.base.interfaces.IMigratingPloneSiteRoot"
+      directory="profiles/uninstall"
       />
 
   <genericsetup:registerProfile
       name="to1000"
       title="Use new icons"
-      directory="profiles/to1000"
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/to1000"
       />
 
   <genericsetup:upgradeDepends
-      source="121"
-      destination="1000"
       title="Use new icons"
       profile="plone.app.iterate:default"
+      source="121"
+      destination="1000"
       import_profile="plone.app.iterate:to1000"
       />
 
   <utility
-      name="plone.app.iterate"
       factory=".setuphandlers.HiddenProfiles"
+      name="plone.app.iterate"
       />
 
   <adapter factory=".archiver.ContentArchiver" />
 
   <!-- Checkout folder locators -->
   <adapter
       factory=".containers.HomeFolderLocator"
@@ -104,25 +118,24 @@
   <adapter
       factory=".containers.ParentFolderLocator"
       name="plone.app.iterate.parent"
       />
 
   <!-- Handle deletions of working copies -->
   <subscriber
-     for=".interfaces.IWorkingCopyRelation
-          zope.lifecycleevent.interfaces.IObjectRemovedEvent"
-     handler=".event.handleDeletion"
-     />
+      for=".interfaces.IWorkingCopyRelation
+           zope.lifecycleevent.interfaces.IObjectRemovedEvent"
+      handler=".event.handleDeletion"
+      />
 
   <permission
-    id="plone.app.iterate.CheckInContent"
-    title="iterate : Check in content"
-    />
+      id="plone.app.iterate.CheckInContent"
+      title="iterate : Check in content"
+      />
 
   <permission
-    id="plone.app.iterate.CheckOutContent"
-    title="iterate : Check out content"
-    />
+      id="plone.app.iterate.CheckOutContent"
+      title="iterate : Check out content"
+      />
 
-  <include package=".dexterity" zcml:condition="installed plone.app.relationfield" />
 
 </configure>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/containers.py` & `plone.app.iterate-5.0.2/plone/app/iterate/containers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -31,41 +30,41 @@
 from Products.CMFCore.utils import getToolByName
 from zope.component import adapter
 from zope.interface import implementer
 
 
 @implementer(IWCContainerLocator)
 @adapter(IDynamicType)
-class HomeFolderLocator(object):
+class HomeFolderLocator:
     """Locate the current user's home folder, if possible."""
 
     def __init__(self, context):
         self.context = context
 
-    title = _(u"Home folder")
+    title = _("Home folder")
 
     @property
     def available(self):
         return self() is not None
 
     def __call__(self):
         return getToolByName(self.context, "portal_membership").getHomeFolder()
 
 
 @implementer(IWCContainerLocator)
 @adapter(IDynamicType)
-class ParentFolderLocator(object):
+class ParentFolderLocator:
     """Locate the parent of the context, if the user has the
     Add portal content permission.
     """
 
     def __init__(self, context):
         self.context = context
 
-    title = _(u"Parent folder")
+    title = _("Parent folder")
 
     @property
     def available(self):
         return bool(
             getSecurityManager().checkPermission(
                 AddPortalContent, aq_parent(aq_inner(self.context))
             )
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/dexterity/configure.zcml` & `plone.app.iterate-5.0.2/plone/app/iterate/dexterity/configure.zcml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 <configure
-        xmlns="http://namespaces.zope.org/zope"
-        xmlns:zcml="http://namespaces.zope.org/zcml"
-        xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
-        xmlns:plone="http://namespaces.plone.org/plone">
-
-    <subscriber
-       for="plone.app.iterate.interfaces.IAfterCheckinEvent"
-       handler="plone.app.iterate.subscribers.locking.handleCheckin"
-       />
-
-    <adapter
-       for="plone.dexterity.interfaces.IDexterityContent"
-       factory=".copier.ContentCopier"
-       />
-
-    <adapter
-       for="plone.dexterity.interfaces.IDexterityContainer"
-       factory=".copier.FolderishContentCopier"
-       />
-
-    <adapter
-       for=".interfaces.IDexterityIterateAware"
-       factory=".policy.CheckinCheckoutPolicyAdapter"
-       />
-
-    <class class="plone.dexterity.content.DexterityContent">
-        <implements interface="plone.app.iterate.dexterity.interfaces.IDexterityIterateAware" />
-    </class>
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
+    xmlns:plone="http://namespaces.plone.org/plone"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    >
+
+  <subscriber
+      for="plone.app.iterate.interfaces.IAfterCheckinEvent"
+      handler="plone.app.iterate.subscribers.locking.handleCheckin"
+      />
+
+  <adapter
+      factory=".copier.ContentCopier"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      />
+
+  <adapter
+      factory=".copier.FolderishContentCopier"
+      for="plone.dexterity.interfaces.IDexterityContainer"
+      />
+
+  <adapter
+      factory=".policy.CheckinCheckoutPolicyAdapter"
+      for=".interfaces.IDexterityIterateAware"
+      />
+
+  <class class="plone.dexterity.content.DexterityContent">
+    <implements interface="plone.app.iterate.dexterity.interfaces.IDexterityIterateAware" />
+  </class>
 
 </configure>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/dexterity/copier.py` & `plone.app.iterate-5.0.2/plone/app/iterate/dexterity/copier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# -*- coding: utf-8 -*-
 from Acquisition import aq_inner
 from Acquisition import aq_parent
-from plone.app.iterate.base import BaseContentCopier
 from plone.app.iterate import interfaces
+from plone.app.iterate.base import BaseContentCopier
 from plone.app.iterate.dexterity import ITERATE_RELATION_NAME
 from plone.app.iterate.dexterity.relation import StagingRelationValue
 from plone.app.iterate.event import AfterCheckinEvent
+from plone.dexterity.utils import createContentInContainer
 from plone.dexterity.utils import iterSchemata
 from Products.CMFCore.utils import getToolByName
 from Products.DCWorkflow.DCWorkflow import DCWorkflowDefinition
 from z3c.relationfield import event
 from zc.relation.interfaces import ICatalog
 from ZODB.PersistentMapping import PersistentMapping
 from zope import component
 from zope.annotation.interfaces import IAnnotations
 from zope.event import notify
 from zope.intid.interfaces import IIntIds
 from zope.schema import getFieldsInOrder
-from plone.dexterity.utils import createContentInContainer
 
 
 class ContentCopier(BaseContentCopier):
     def copyTo(self, container):
         context = aq_inner(self.context)
         wc = self._copyBaseline(container)
         # get id of objects
@@ -166,15 +165,15 @@
 
 
 class FolderishContentCopier(ContentCopier):
     def _copyBaseline(self, container):
         obj = createContentInContainer(
             container,
             self.context.portal_type,
-            id="working_copy_of_{}".format(self.context.id),
+            id=f"working_copy_of_{self.context.id}",
         )
 
         # copy all field values from the baseline to the working copy
         for schema in iterSchemata(self.context):
             for name, field in getFieldsInOrder(schema):
                 # Skip read-only fields
                 if field.readonly:
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/dexterity/policy.py` & `plone.app.iterate-5.0.2/plone/app/iterate/dexterity/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.app.iterate.base import CheckinCheckoutBasePolicyAdapter
 from plone.app.iterate.dexterity.interfaces import IDexterityIterateAware
 from plone.app.iterate.dexterity.utils import get_baseline
 from plone.app.iterate.dexterity.utils import get_checkout_relation
 from plone.app.iterate.dexterity.utils import get_relations
 from plone.app.iterate.dexterity.utils import get_working_copy
 from plone.app.iterate.event import AfterCheckinEvent
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/dexterity/relation.py` & `plone.app.iterate-5.0.2/plone/app/iterate/dexterity/relation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.app.iterate.dexterity.interfaces import IStagingRelationValue
 from z3c.relationfield import relation
 from zc.relation.interfaces import ICatalog
 from zope.annotation.interfaces import IAttributeAnnotatable
 from zope.component import getUtility
 from zope.interface import implementer
 from zope.intid.interfaces import IIntIds
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/dexterity/utils.py` & `plone.app.iterate-5.0.2/plone/app/iterate/dexterity/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from Acquisition import aq_base
 from Acquisition import aq_inner
 from plone.app.iterate.dexterity import ITERATE_RELATION_NAME
 from zc.relation.interfaces import ICatalog
 from zope import component
 from zope.intid.interfaces import IIntIds
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/event.py` & `plone.app.iterate-5.0.2/plone/app/iterate/event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -18,19 +17,18 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with CMFDeployment; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 ##################################################################
 """
 """
-from zope.interface.interfaces import ObjectEvent
+from . import interfaces
 from zope.event import notify
 from zope.interface import implementer
-
-from . import interfaces
+from zope.interface.interfaces import ObjectEvent
 
 
 @implementer(interfaces.ICheckoutEvent)
 class CheckoutEvent(ObjectEvent):
     def __init__(self, baseline, wc, relation):
         ObjectEvent.__init__(self, baseline)
         self.working_copy = wc
@@ -45,15 +43,15 @@
         self.relation = relation
         self.message = message
 
 
 @implementer(interfaces.IAfterCheckinEvent)
 class AfterCheckinEvent(ObjectEvent):
     def __init__(self, new_baseline, checkin_message):
-        super(AfterCheckinEvent, self).__init__(new_baseline)
+        super().__init__(new_baseline)
         self.message = checkin_message
 
 
 @implementer(interfaces.ICancelCheckoutEvent)
 class CancelCheckoutEvent(ObjectEvent):
     def __init__(self, wc, baseline):
         ObjectEvent.__init__(self, wc)
@@ -66,15 +64,14 @@
         ObjectEvent.__init__(self, wc)
         self.baseline = baseline
         self.relation = relation
 
 
 @implementer(interfaces.IBeforeCheckoutEvent)
 class BeforeCheckoutEvent(ObjectEvent):
-
     pass
 
 
 def handleDeletion(reference, event):
     # a filtering/enriching event rebroadcaster for working copy deletions
     workingCopy = reference.getSourceObject()
     baseline = reference.getTargetObject()
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/interfaces.py` & `plone.app.iterate-5.0.2/plone/app/iterate/interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -16,27 +15,21 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with CMFDeployment; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 ##################################################################
-"""
-$Id: interfaces.py 1811 2007-02-06 18:40:02Z hazmat $
-"""
-
 from plone.app.iterate import PloneMessageFactory as _
 from plone.locking.interfaces import LockType
 from plone.locking.interfaces import MAX_TIMEOUT
 from zope import schema
-from zope.interface.interfaces import IObjectEvent
 from zope.interface import Attribute
 from zope.interface import Interface
-
-import pkg_resources
+from zope.interface.interfaces import IObjectEvent
 
 
 class IReference(Interface):
     pass
 
 
 ################################
@@ -47,16 +40,16 @@
     """An object that can be used for check-in/check-out operations."""
 
 
 #################################
 #  Lock types
 
 ITERATE_LOCK = LockType(
-    u"iterate.lock", stealable=False, user_unlockable=False, timeout=MAX_TIMEOUT
-)  # noqa
+    "iterate.lock", stealable=False, user_unlockable=False, timeout=MAX_TIMEOUT
+)
 
 #################################
 #  Exceptions
 
 
 class CociException(Exception):
     pass
@@ -75,15 +68,15 @@
 
 
 #################################
 # Annotation Key
 annotation_key = "ore.iterate"
 
 
-class keys(object):
+class keys:
     # various common keys
     checkout_user = "checkout_user"
     checkout_time = "checkout_time"
 
 
 #################################
 #  Event Interfaces
@@ -96,32 +89,32 @@
 
     baseline = Attribute("The Working Copy's baseline")
     relation = Attribute("The Working Copy Relation Object")
     checkin_message = Attribute("checkin message")
 
 
 class IAfterCheckinEvent(IObjectEvent):
-    """ sent out after an object is checked in """
+    """sent out after an object is checked in"""
 
     checkin_message = Attribute("checkin message")
 
 
 class IBeforeCheckoutEvent(IObjectEvent):
-    """ sent out before a working copy is created """
+    """sent out before a working copy is created"""
 
 
 class ICheckoutEvent(IObjectEvent):
-    """ an object is being checked out, event.object is the baseline """
+    """an object is being checked out, event.object is the baseline"""
 
     working_copy = Attribute("The object's working copy")
     relation = Attribute("The Working Copy Relation Object")
 
 
 class ICancelCheckoutEvent(IObjectEvent):
-    """ a working copy is being cancelled """
+    """a working copy is being cancelled"""
 
     baseline = Attribute("The working copy's baseline")
 
 
 class IWorkingCopyDeletedEvent(IObjectEvent):
     """a working copy is being deleted, this gets called multiple times at
     different states.
@@ -162,18 +155,18 @@
 
 class IWCContainerLocator(Interface):
     """A named adapter capable of discovering containers where working
     copies can be created.
     """
 
     available = schema.Bool(
-        title=u"Available", description=u"Whether location will be available."
+        title="Available", description="Whether location will be available."
     )
 
-    title = schema.TextLine(title=u"Title", description=u"Title of this location")
+    title = schema.TextLine(title="Title", description="Title of this location")
 
     def __call__():
         """Return a container object, or None if available() is False"""
 
 
 #################################
 #  Interfaces
@@ -295,21 +288,20 @@
         """"""
 
     def checkinBackReferences(baseline, wc, references, storage):
         """"""
 
 
 class IIterateSettings(Interface):
-
     enable_checkout_workflow = schema.Bool(
-        title=_(u"Enable checkout workflow"),
-        description=u"",
+        title=_("Enable checkout workflow"),
+        description="",
         default=False,
         required=False,
     )
 
     checkout_workflow_policy = schema.ASCIILine(
-        title=_(u"Checkout workflow policy"),
-        description=u"",
+        title=_("Checkout workflow policy"),
+        description="",
         default="checkout_workflow_policy",
         required=True,
     )
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/lock.py` & `plone.app.iterate-5.0.2/plone/app/iterate/lock.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -18,16 +17,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with iterate; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 ##################################################################
 """
 Checkin / Checkout Specific DAV Lock Manipulation and Introspection
-
-$Id: lock.py 1392 2006-06-20 01:02:17Z hazmat $
 """
 
 from .interfaces import ITERATE_LOCK
 from plone.locking.interfaces import ILockable
 
 
 __all__ = ["lockContext", "unlockContext", "isLocked"]
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/permissions.py` & `plone.app.iterate-5.0.2/plone/app/iterate/permissions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -19,13 +18,14 @@
 # You should have received a copy of the GNU General Public License
 # along with CMFDeployment; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 ##################################################################
 
 from AccessControl.Permission import addPermission
 
+
 CheckinPermission = "iterate : Check in content"
 CheckoutPermission = "iterate : Check out content"
 
 DEFAULT_ROLES = ("Manager", "Owner", "Site Administrator", "Editor")
 addPermission(CheckinPermission, default_roles=DEFAULT_ROLES)
 addPermission(CheckoutPermission, default_roles=DEFAULT_ROLES)
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/profiles/default/actions.xml` & `plone.app.iterate-5.0.2/plone/app/iterate/profiles/default/actions.xml`

 * *Files 12% similar despite different names*

#### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/profiles/default/actions.xml` & `plone.app.iterate-5.0.2/plone/app/iterate/profiles/default/actions.xml`

```diff
@@ -1,33 +1,33 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="portal_actions" meta_type="Plone Actions Tool">
-  <object name="object_buttons" meta_type="CMF Action Category">
-    <object name="iterate_checkin" meta_type="CMF Action" i18n:domain="plone">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Plone Actions Tool" name="portal_actions">
+  <object meta_type="CMF Action Category" name="object_buttons">
+    <object meta_type="CMF Action" name="iterate_checkin" i18n:domain="plone">
       <property name="title" i18n:translate="">Check in</property>
       <property name="description" i18n:translate=""/>
       <property name="url_expr">string:${object_url}/@@content-checkin</property>
       <property name="icon_expr">string:box-arrow-in-up-right</property>
       <property name="available_expr">python:path('object/@@iterate_control').checkin_allowed()</property>
       <property name="permissions">
         <element value="View"/>
       </property>
       <property name="visible">True</property>
     </object>
-    <object name="iterate_checkout" meta_type="CMF Action" i18n:domain="plone">
+    <object meta_type="CMF Action" name="iterate_checkout" i18n:domain="plone">
       <property name="title" i18n:translate="">Check out</property>
       <property name="description" i18n:translate=""/>
       <property name="url_expr">string:${object_url}/@@content-checkout</property>
       <property name="icon_expr">string:box-arrow-down-left</property>
       <property name="available_expr">python:path('object/@@iterate_control').checkout_allowed()</property>
       <property name="permissions">
         <element value="View"/>
       </property>
       <property name="visible">True</property>
     </object>
-    <object name="iterate_checkout_cancel" meta_type="CMF Action" i18n:domain="plone">
+    <object meta_type="CMF Action" name="iterate_checkout_cancel" i18n:domain="plone">
       <property name="title" i18n:translate="">Cancel check-out</property>
       <property name="description" i18n:translate=""/>
       <property name="url_expr">string:${object_url}/@@content-cancel-checkout</property>
       <property name="icon_expr">string:arrow-counterclockwise</property>
       <property name="available_expr">python:path('object/@@iterate_control').cancel_allowed()</property>
       <property name="permissions">
         <element value="Modify portal content"/>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/profiles/test/workflows/workingcopy_workflow/definition.xml` & `plone.app.iterate-5.0.2/plone/app/iterate/profiles/test/workflows/workingcopy_workflow/definition.xml`

 * *Files 23% similar despite different names*

#### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/profiles/test/workflows/workingcopy_workflow/definition.xml` & `plone.app.iterate-5.0.2/plone/app/iterate/profiles/test/workflows/workingcopy_workflow/definition.xml`

```diff
@@ -1,137 +1,137 @@
 <?xml version="1.0" encoding="utf-8"?>
-<dc-workflow xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="plone" workflow_id="workingcopy_workflow" title="test wc workflow" state_variable="review_state" initial_state="draft-copy" i18n:attributes="title">
+<dc-workflow xmlns:i18n="http://xml.zope.org/namespaces/i18n" initial_state="draft-copy" state_variable="review_state" title="test wc workflow" workflow_id="workingcopy_workflow" i18n:attributes="title" i18n:domain="plone">
   <!-- These are the permissions being managed -->
   <permission>Delete objects</permission>
   <permission>iterate : Check in content</permission>
   <permission>iterate : Check out content</permission>
   <permission>View</permission>
   <permission>Access contents information</permission>
   <permission>Modify portal content</permission>
   <permission>Copy or Move</permission>
   <!-- The various workflow states, with their permission maps -->
   <state state_id="draft-copy" title="Draft (copy)" i18n:attributes="title">
     <description i18n:translate="">New version created but not ready for publication</description>
     <exit-transition transition_id="submit-copy-for-publication"/>
-    <permission-map name="Access contents information" acquired="False">
+    <permission-map acquired="False" name="Access contents information">
       <permission-role>Editor</permission-role>
       <permission-role>Contributor</permission-role>
       <permission-role>Site Administrator</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
+    <permission-map acquired="False" name="Modify portal content">
       <permission-role>Editor</permission-role>
       <permission-role>Contributor</permission-role>
       <permission-role>Site Administrator</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="View" acquired="False">
+    <permission-map acquired="False" name="View">
       <permission-role>Editor</permission-role>
       <permission-role>Contributor</permission-role>
       <permission-role>Site Administrator</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="iterate : Check in content" acquired="False"/>
-    <permission-map name="iterate : Check out content" acquired="False"/>
-    <permission-map name="Copy or Move" acquired="False"/>
-    <permission-map name="Delete objects" acquired="False">
+    <permission-map acquired="False" name="iterate : Check in content"/>
+    <permission-map acquired="False" name="iterate : Check out content"/>
+    <permission-map acquired="False" name="Copy or Move"/>
+    <permission-map acquired="False" name="Delete objects">
       <permission-role>Editor</permission-role>
       <permission-role>Contributor</permission-role>
       <permission-role>Site Administrator</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <state state_id="pending-copy" title="Pending (copy)" i18n:attributes="title">
     <description i18n:translate="">Copy submitted for publication - pending approval</description>
     <exit-transition transition_id="withdraw-submitted-copy"/>
     <exit-transition transition_id="reject-submitted-copy"/>
-    <permission-map name="Access contents information" acquired="False">
+    <permission-map acquired="False" name="Access contents information">
       <permission-role>Editor</permission-role>
       <permission-role>Contributor</permission-role>
       <permission-role>Site Administrator</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="Modify portal content" acquired="False">
+    <permission-map acquired="False" name="Modify portal content">
       <permission-role>Editor</permission-role>
       <permission-role>Site Administrator</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="View" acquired="False">
+    <permission-map acquired="False" name="View">
       <permission-role>Editor</permission-role>
       <permission-role>Contributor</permission-role>
       <permission-role>Site Administrator</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="iterate : Check in content" acquired="False">
+    <permission-map acquired="False" name="iterate : Check in content">
       <permission-role>Editor</permission-role>
       <permission-role>Site Administrator</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
-    <permission-map name="iterate : Check out content" acquired="False"/>
-    <permission-map name="Copy or Move" acquired="False"/>
-    <permission-map name="Delete objects" acquired="False">
+    <permission-map acquired="False" name="iterate : Check out content"/>
+    <permission-map acquired="False" name="Copy or Move"/>
+    <permission-map acquired="False" name="Delete objects">
       <permission-role>Editor</permission-role>
       <permission-role>Site Administrator</permission-role>
       <permission-role>Contributor</permission-role>
       <permission-role>Manager</permission-role>
     </permission-map>
   </state>
   <!-- Transitions between states, including guard conditions -->
-  <transition transition_id="submit-copy-for-publication" new_state="pending-copy" title="Submit draft content for publication" trigger="USER" before_script="" after_script="" i18n:attributes="title">
+  <transition after_script="" before_script="" new_state="pending-copy" title="Submit draft content for publication" transition_id="submit-copy-for-publication" trigger="USER" i18n:attributes="title">
     <description i18n:translate="">Move the content to the pending state where it will be reviewed by an editor by publication.</description>
-    <action url="%(content_url)s/content_status_modify?workflow_action=submit-copy-for-publication" category="workflow" i18n:translate="">Submit</action>
+    <action category="workflow" url="%(content_url)s/content_status_modify?workflow_action=submit-copy-for-publication" i18n:translate="">Submit</action>
     <guard>
       <guard-permission>Modify portal content</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="reject-submitted-copy" new_state="draft-copy" title="Editor rejects submitted content" trigger="USER" before_script="" after_script="" i18n:attributes="title">
+  <transition after_script="" before_script="" new_state="draft-copy" title="Editor rejects submitted content" transition_id="reject-submitted-copy" trigger="USER" i18n:attributes="title">
     <description i18n:translate="">Revert to draft.</description>
     <guard>
       <guard-permission>Review portal content</guard-permission>
     </guard>
   </transition>
-  <transition transition_id="withdraw-submitted-copy" new_state="draft-copy" title="Contributor withdraws submitted content" trigger="USER" before_script="" after_script="" i18n:attributes="title">
+  <transition after_script="" before_script="" new_state="draft-copy" title="Contributor withdraws submitted content" transition_id="withdraw-submitted-copy" trigger="USER" i18n:attributes="title">
     <description i18n:translate="">Revert to draft.</description>
     <guard>
       <guard-role>Contributor</guard-role>
     </guard>
   </transition>
   <!-- Workflow variables, managed as part of workflow history -->
-  <variable variable_id="action" for_catalog="False" for_status="True" update_always="True">
+  <variable for_catalog="False" for_status="True" update_always="True" variable_id="action">
     <description>The last transition</description>
     <default>
       <expression>transition/getId|nothing</expression>
     </default>
     <guard/>
   </variable>
-  <variable variable_id="actor" for_catalog="False" for_status="True" update_always="True">
+  <variable for_catalog="False" for_status="True" update_always="True" variable_id="actor">
     <description>The ID of the user who performed the last transition</description>
     <default>
       <expression>user/getId</expression>
     </default>
     <guard/>
   </variable>
-  <variable variable_id="comments" for_catalog="False" for_status="True" update_always="True">
+  <variable for_catalog="False" for_status="True" update_always="True" variable_id="comments">
     <description>Comments about the last transition</description>
     <default>
       <expression>python:state_change.kwargs.get('comment', '')</expression>
     </default>
     <guard/>
   </variable>
-  <variable variable_id="review_history" for_catalog="False" for_status="False" update_always="False">
+  <variable for_catalog="False" for_status="False" update_always="False" variable_id="review_history">
     <description>Provides access to workflow history</description>
     <default>
       <expression>state_change/getHistory</expression>
     </default>
     <guard>
       <guard-permission>Request review</guard-permission>
       <guard-permission>Review portal content</guard-permission>
     </guard>
   </variable>
-  <variable variable_id="time" for_catalog="False" for_status="True" update_always="True">
+  <variable for_catalog="False" for_status="True" update_always="True" variable_id="time">
     <description>Time of the last transition</description>
     <default>
       <expression>state_change/getDateTime</expression>
     </default>
     <guard/>
   </variable>
 </dc-workflow>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/profiles/testingdx/types/FolderishDocument.xml` & `plone.app.iterate-5.0.2/plone/app/iterate/profiles/testingdx/types/FolderishDocument.xml`

 * *Files 9% similar despite different names*

#### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/profiles/testingdx/types/FolderishDocument.xml` & `plone.app.iterate-5.0.2/plone/app/iterate/profiles/testingdx/types/FolderishDocument.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="FolderishDocument" meta_type="Dexterity FTI" i18n:domain="plone">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="FolderishDocument" i18n:domain="plone">
   <!-- Basic metadata -->
   <property name="title" i18n:translate="">DX Test Folderish Document</property>
   <property name="description" i18n:translate=""/>
   <property name="icon_expr"/>
   <property name="factory">FolderishDocument</property>
   <property name="add_view_expr">string:${folder_url}/++add++FolderishDocument</property>
   <property name="global_allow">True</property>
@@ -39,14 +39,14 @@
   <property name="add_permission">cmf.AddPortalContent</property>
   <!-- Method aliases -->
   <alias from="(Default)" to="(dynamic view)"/>
   <alias from="view" to="(selected layout)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <!-- Actions -->
-  <action title="View" action_id="view" category="object" condition_expr="" url_expr="string:${object_url}/" visible="True">
+  <action action_id="view" category="object" condition_expr="" title="View" url_expr="string:${object_url}/" visible="True">
     <permission value="View"/>
   </action>
-  <action title="Edit" action_id="edit" category="object" condition_expr="" url_expr="string:${object_url}/edit" visible="True">
+  <action action_id="edit" category="object" condition_expr="" title="Edit" url_expr="string:${object_url}/edit" visible="True">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/profiles/to1000/actions.xml` & `plone.app.iterate-5.0.2/plone/app/iterate/profiles/to1000/actions.xml`

 * *Files 16% similar despite different names*

#### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/profiles/to1000/actions.xml` & `plone.app.iterate-5.0.2/plone/app/iterate/profiles/to1000/actions.xml`

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="portal_actions" meta_type="Plone Actions Tool">
-  <object name="object_buttons" meta_type="CMF Action Category">
-    <object name="iterate_checkin" meta_type="CMF Action" i18n:domain="plone">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Plone Actions Tool" name="portal_actions">
+  <object meta_type="CMF Action Category" name="object_buttons">
+    <object meta_type="CMF Action" name="iterate_checkin" i18n:domain="plone">
       <property name="icon_expr">string:box-arrow-in-up-right</property>
     </object>
-    <object name="iterate_checkout" meta_type="CMF Action" i18n:domain="plone">
+    <object meta_type="CMF Action" name="iterate_checkout" i18n:domain="plone">
       <property name="icon_expr">string:box-arrow-down-left</property>
     </object>
-    <object name="iterate_checkout_cancel" meta_type="CMF Action" i18n:domain="plone">
+    <object meta_type="CMF Action" name="iterate_checkout_cancel" i18n:domain="plone">
       <property name="icon_expr">string:arrow-counterclockwise</property>
     </object>
   </object>
 </object>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/setuphandlers.py` & `plone.app.iterate-5.0.2/plone/app/iterate/setuphandlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# -*- coding: utf-8 -*-
-from Products.CMFPlone.interfaces import INonInstallable
+from plone.base.interfaces.installable import INonInstallable
 from zope.interface import implementer
 
 import warnings
 
 
 @implementer(INonInstallable)
-class HiddenProfiles(object):
+class HiddenProfiles:
     def getNonInstallableProfiles(self):
         """Prevents uninstall profile from showing up in the profile list
         when creating a Plone site.
 
         """
         return [
-            u"plone.app.iterate:uninstall",
-            u"plone.app.iterate:plone.app.iterate",
+            "plone.app.iterate:uninstall",
+            "plone.app.iterate:plone.app.iterate",
         ]
 
 
 def deprecate_profile(tool):
     """Deprecation profile plone.app.iterate.
 
     Deprecation warning for plone.app.iterate:plone.app.iterate profile.
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/subscribers/configure.zcml` & `plone.app.iterate-5.0.2/plone/app/iterate/subscribers/configure.zcml`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,81 @@
-<configure
-    xmlns="http://namespaces.zope.org/zope">
+<configure xmlns="http://namespaces.zope.org/zope">
 
 
-    <!-- Locking -->
+  <!-- Locking -->
 
-    <subscriber
-       for="..interfaces.ICheckoutEvent"
-       handler=".locking.handleCheckout"
-       />
+  <subscriber
+      for="..interfaces.ICheckoutEvent"
+      handler=".locking.handleCheckout"
+      />
 
-    <subscriber
-       for="..interfaces.ICheckinEvent"
-       handler=".locking.handleCheckin"
-       />
+  <subscriber
+      for="..interfaces.ICheckinEvent"
+      handler=".locking.handleCheckin"
+      />
 
-    <subscriber
-       for="..interfaces.ICancelCheckoutEvent"
-       handler=".locking.handleCancelCheckout"
-       />
+  <subscriber
+      for="..interfaces.ICancelCheckoutEvent"
+      handler=".locking.handleCancelCheckout"
+      />
 
-    <subscriber
-       for="..interfaces.IWorkingCopyDeletedEvent"
-       handler=".locking.handleWCDeleted"
-       />
+  <subscriber
+      for="..interfaces.IWorkingCopyDeletedEvent"
+      handler=".locking.handleWCDeleted"
+      />
 
-    <!-- Marker  -->
+  <!-- Marker  -->
 
-    <subscriber
-       for="..interfaces.ICheckoutEvent"
-       handler=".marker.handleCheckout"
-       />
+  <subscriber
+      for="..interfaces.ICheckoutEvent"
+      handler=".marker.handleCheckout"
+      />
 
-    <subscriber
-       for="..interfaces.ICheckinEvent"
-       handler=".marker.handleCheckin"
-       />
+  <subscriber
+      for="..interfaces.ICheckinEvent"
+      handler=".marker.handleCheckin"
+      />
 
-    <subscriber
-       for="..interfaces.ICancelCheckoutEvent"
-       handler=".marker.handleCancelCheckout"
-       />
+  <subscriber
+      for="..interfaces.ICancelCheckoutEvent"
+      handler=".marker.handleCancelCheckout"
+      />
 
-    <subscriber
-       for="..interfaces.IWorkingCopyDeletedEvent"
-       handler=".marker.handleWCDeleted"
-       />
+  <subscriber
+      for="..interfaces.IWorkingCopyDeletedEvent"
+      handler=".marker.handleWCDeleted"
+      />
 
 
-    <!-- Metadata -->
+  <!-- Metadata -->
 
-    <subscriber
-       for="..interfaces.ICheckoutEvent"
-       handler=".metadata.handleCheckout"
-       />
+  <subscriber
+      for="..interfaces.ICheckoutEvent"
+      handler=".metadata.handleCheckout"
+      />
 
-    <!-- Versioning -->
+  <!-- Versioning -->
 
-    <subscriber
-       for="..interfaces.IBeforeCheckoutEvent"
-       handler=".versioning.handleBeforeCheckout"
-       />
+  <subscriber
+      for="..interfaces.IBeforeCheckoutEvent"
+      handler=".versioning.handleBeforeCheckout"
+      />
 
-    <subscriber
-       for="..interfaces.IAfterCheckinEvent"
-       handler=".versioning.handleAfterCheckin"
-       />
+  <subscriber
+      for="..interfaces.IAfterCheckinEvent"
+      handler=".versioning.handleAfterCheckin"
+      />
 
 
-    <!-- Workflow -->
+  <!-- Workflow -->
 
-    <subscriber
-       for="..interfaces.ICheckoutEvent"
-       handler=".workflow.handleCheckout"
-       />
+  <subscriber
+      for="..interfaces.ICheckoutEvent"
+      handler=".workflow.handleCheckout"
+      />
 
-    <subscriber
-       for="..interfaces.ICheckinEvent"
-       handler=".workflow.handleCheckin"
-       />
+  <subscriber
+      for="..interfaces.ICheckinEvent"
+      handler=".workflow.handleCheckin"
+      />
 
 </configure>
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/subscribers/locking.py` & `plone.app.iterate-5.0.2/plone/app/iterate/subscribers/locking.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006-2007 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -16,18 +15,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with CMFDeployment; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 ##################################################################
-"""
-$Id: locking.py 1824 2007-02-08 17:59:41Z hazmat $
-"""
-
 from plone.app.iterate import lock
 from plone.locking.interfaces import ILockable
 
 
 def handleWCDeleted(event):
     # may be called multiple times, must be reentrant
     lock.unlockContext(event.baseline)
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/subscribers/marker.py` & `plone.app.iterate-5.0.2/plone/app/iterate/subscribers/marker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006-2007 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -16,18 +15,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with CMFDeployment; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 ##################################################################
-"""
-$Id: marker.py 1824 2007-02-08 17:59:41Z hazmat $
-"""
-
 from plone.app.iterate import interfaces
 from Products.Five.utilities import marker
 
 
 def handleCheckout(event):
     marker.mark(event.working_copy, interfaces.IWorkingCopy)
     marker.mark(event.object, interfaces.IBaseline)
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/subscribers/metadata.py` & `plone.app.iterate-5.0.2/plone/app/iterate/subscribers/metadata.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006-2007 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -16,18 +15,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with CMFDeployment; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 ##################################################################
-"""
-$Id: metadata.py 1824 2007-02-08 17:59:41Z hazmat $
-"""
-
 from AccessControl import getSecurityManager
 from DateTime import DateTime
 from plone.app.iterate.interfaces import keys
 from plone.app.iterate.util import get_storage
 
 
 def handleCheckout(event):
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/subscribers/versioning.py` & `plone.app.iterate-5.0.2/plone/app/iterate/subscribers/versioning.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006-2007 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -16,17 +15,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with CMFDeployment; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 ##################################################################
-"""
-"""
-
 from plone.app.iterate import interfaces
 
 
 def handleBeforeCheckout(event):
     archiver = interfaces.IObjectArchiver(event.object)
     if archiver.isModified() or not archiver.isVersioned():
         archiver.save("Baseline created")
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/subscribers/workflow.py` & `plone.app.iterate-5.0.2/plone/app/iterate/subscribers/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006-2007 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -17,30 +16,23 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with CMFDeployment; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 ##################################################################
 """
-$Id: workflow.py 1824 2007-02-08 17:59:41Z hazmat $
-
 Applies new checkout specific workflows to content that is checked out.
-
 """
 
 from Acquisition import aq_base
 from plone.app.iterate.interfaces import IIterateSettings
 from plone.app.iterate.util import get_storage
 from plone.registry.interfaces import IRegistry
-from Products.CMFPlacefulWorkflow.PlacefulWorkflowTool import (
-    WorkflowPolicyConfig_id,
-)  # noqa
-from Products.CMFPlacefulWorkflow.WorkflowPolicyConfig import (
-    WorkflowPolicyConfig,
-)  # noqa
+from Products.CMFPlacefulWorkflow.PlacefulWorkflowTool import WorkflowPolicyConfig_id
+from Products.CMFPlacefulWorkflow.WorkflowPolicyConfig import WorkflowPolicyConfig
 from zope.component import getUtility
 
 
 USE_WORKFLOW = "checkout_workflow_policy"
 
 policy_storage = "previous_wf_policy"
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/testing.py` & `plone.app.iterate-5.0.2/plone/app/iterate/testing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Testing setup for integration and functional tests."""
 from plone.app.contenttypes.testing import PloneAppContenttypes
 from plone.app.testing import applyProfile
-from plone.app.testing import PLONE_FIXTURE
-from plone.app.testing import PloneSandboxLayer
 from plone.app.testing.layers import FunctionalTesting
 from plone.app.testing.layers import IntegrationTesting
 
 
 ADMIN = {
     "id": "admin",
     "password": "secret",
@@ -34,32 +32,30 @@
 
 
 class DexPloneAppIterateLayer(PloneAppContenttypes):
     """Dexterity based Plone Sandbox Layer for plone.app.iterate."""
 
     def setUpZope(self, app, configurationContext):
         """Setup Zope with Addons."""
-        super(DexPloneAppIterateLayer, self).setUpZope(app, configurationContext)
+        super().setUpZope(app, configurationContext)
 
         import plone.app.iterate
 
         self.loadZCML(package=plone.app.iterate)
 
     def setUpPloneSite(self, portal):
         """Setup Plone Site with Addons."""
-        super(DexPloneAppIterateLayer, self).setUpPloneSite(portal)
+        super().setUpPloneSite(portal)
         applyProfile(portal, "plone.app.iterate:default")
         applyProfile(portal, "plone.app.iterate:testingdx")
         # with named AND dotted behaviors we need to take care of both
-        versioning_behavior = set(
-            [
-                "plone.app.versioningbehavior.behaviors.IVersionable",
-                "plone.versioning",
-            ],
-        )
+        versioning_behavior = {
+            "plone.app.versioningbehavior.behaviors.IVersionable",
+            "plone.versioning",
+        }
 
         # Disable automatic versioning of core content types
         for name in ("Document", "Event", "Link", "News Item"):
             fti = portal.portal_types[name]
             # write back the behaviors without the versioning behaviors
             # using a Set to keep it simple
             # a = set((1,2,3))
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/tests/dexterity.rst` & `plone.app.iterate-5.0.2/plone/app/iterate/tests/dexterity.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     >>> browser = Browser(layer["app"])
     >>> browser.handleErrors = False
     >>> portal = layer["portal"]
     >>> portal_url = "http://nohost/plone"
     >>> from plone.app.testing.interfaces import SITE_OWNER_NAME, SITE_OWNER_PASSWORD
     >>> browser.addHeader("Authorization", "Basic %s:%s" % (SITE_OWNER_NAME, SITE_OWNER_PASSWORD))
 
-KeyError with aquisition wrapper
+KeyError with acquisition wrapper
 =========================================
 
 When an item provides IBaseline (has been checked in at least once) and it is accessed through an
-Aquisition wrapper you get a KeyError from zope.intid, originating from five.intid.
+Acquisition wrapper you get a KeyError from zope.intid, originating from five.intid.
 
     >>> browser.open(portal_url + "/folder_factories")
     >>> browser.getControl("Folder").click()
     >>> browser.getControl("Add").click()
     >>> browser.getControl(name="form.widgets.IDublinCore.title").value = "My Folder"
     >>> browser.getControl(name="form.buttons.save").click()
     >>> browser.url
@@ -49,12 +49,12 @@
     >>> browser.getLink("Check in").click()
     >>> browser.contents
     '...Check in...'
     >>> browser.getControl(name="form.button.Checkin").click()
     >>> browser.url
     'http://nohost/plone/my-folder/my-sub-object'
 
-Test can view through Aquisition wrapper (repeating test_folder is deliberate here)
+Test can view through Acquisition wrapper (repeating test_folder is deliberate here)
 
     >>> browser.open("http://nohost/plone/my-folder/my-sub-object")
     >>> browser.contents
     '...My Sub-object...'
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/tests/test_annotations.py` & `plone.app.iterate-5.0.2/plone/app/iterate/tests/test_annotations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-# -*- coding: utf-8 -*-
-
 from plone.app.iterate.interfaces import ICheckinCheckoutPolicy
 from plone.app.iterate.interfaces import IWCContainerLocator
 from plone.app.iterate.testing import PLONEAPPITERATEDEX_INTEGRATION_TESTING
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from zope.annotation.interfaces import IAnnotatable
 from zope.annotation.interfaces import IAnnotations
 from zope.component import getAdapters
 
 import unittest
 
 
 class AnnotationsTestCase(unittest.TestCase):
-
     layer = PLONEAPPITERATEDEX_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.portal.invokeFactory("Document", "s1")
         self.s1 = self.portal["s1"]
@@ -26,50 +23,50 @@
         self.assertTrue(IAnnotatable.providedBy(self.s1))
 
     def test_annotation_saved_on_checkin(self):
         # First we get and save a custom annotation to the existing object
         obj_annotations = IAnnotations(self.s1)
         self.assertEqual(obj_annotations, {})
 
-        obj_annotations["key1"] = u"value1"
+        obj_annotations["key1"] = "value1"
         obj_annotations = IAnnotations(self.s1)
-        self.assertEqual(obj_annotations, {"key1": u"value1"})
+        self.assertEqual(obj_annotations, {"key1": "value1"})
 
         # Now, let's get a working copy for it.
         locators = getAdapters((self.s1,), IWCContainerLocator)
-        location = u"plone.app.iterate.parent"
+        location = "plone.app.iterate.parent"
         locator = [c[1] for c in locators if c[0] == location][0]
 
         policy = ICheckinCheckoutPolicy(self.s1)
 
         wc = policy.checkout(locator())
 
         # Annotations should be the same
         new_annotations = IAnnotations(wc)
-        self.assertEqual(new_annotations["key1"], u"value1")
+        self.assertEqual(new_annotations["key1"], "value1")
 
         # Now, let's modify the existing one, and create a new one
-        new_annotations["key1"] = u"value2"
-        new_annotations["key2"] = u"value1"
+        new_annotations["key1"] = "value2"
+        new_annotations["key2"] = "value1"
 
         # Check that annotations were stored correctly and original ones were
         # not overriten
         new_annotations = IAnnotations(wc)
-        self.assertEqual(new_annotations["key1"], u"value2")
-        self.assertEqual(new_annotations["key2"], u"value1")
+        self.assertEqual(new_annotations["key1"], "value2")
+        self.assertEqual(new_annotations["key2"], "value1")
 
         obj_annotations = IAnnotations(self.s1)
-        self.assertEqual(obj_annotations["key1"], u"value1")
+        self.assertEqual(obj_annotations["key1"], "value1")
         self.assertFalse("key2" in obj_annotations)
 
         # Now, we do a checkin
         policy = ICheckinCheckoutPolicy(wc)
-        policy.checkin(u"Commit message")
+        policy.checkin("Commit message")
 
         # And finally check that the old object has the same annotations as
         # its working copy
 
         obj_annotations = IAnnotations(self.s1)
         self.assertTrue("key1" in obj_annotations)
         self.assertTrue("key2" in obj_annotations)
-        self.assertEqual(obj_annotations["key1"], u"value2")
-        self.assertEqual(obj_annotations["key2"], u"value1")
+        self.assertEqual(obj_annotations["key1"], "value2")
+        self.assertEqual(obj_annotations["key2"], "value1")
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/tests/test_containers.py` & `plone.app.iterate-5.0.2/plone/app/iterate/tests/test_containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -25,24 +24,23 @@
 from plone.app.iterate.browser.control import Control
 from plone.app.iterate.interfaces import ICheckinCheckoutPolicy
 from plone.app.iterate.testing import PLONEAPPITERATEDEX_INTEGRATION_TESTING
 from plone.app.testing import login
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import TEST_USER_NAME
+from plone.dexterity.utils import createContentInContainer
 from zc.relation.interfaces import ICatalog
-from zope.intid.interfaces import IIntIds
 from zope import component
-from plone.dexterity.utils import createContentInContainer
+from zope.intid.interfaces import IIntIds
 
 import unittest
 
 
 class TestIterations(unittest.TestCase):
-
     layer = PLONEAPPITERATEDEX_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         login(self.portal, TEST_USER_NAME)
 
@@ -85,25 +83,25 @@
 
         self.assertNotEqual(state, wc_state)
 
         baseline = ICheckinCheckoutPolicy(wc).checkin("modified")
         bstate = self.wf.getInfoFor(baseline, "review_state")
         self.assertEqual(bstate, "published")
 
-        self.assertEquals(len(self.portal.workarea.objectIds()), 0)
+        self.assertEqual(len(self.portal.workarea.objectIds()), 0)
         setRoles(self.portal, TEST_USER_ID, ["Owner"])
 
     def test_container_baselineCreated(self):
         # if a baseline has no version ensure that one is created on checkout
         doc = self.portal.docs.doc1
         self.assertTrue(self.repo.isVersionable(doc))
 
         wc = ICheckinCheckoutPolicy(doc).checkout(self.portal.workarea)
 
-        self.assertEquals(wc.id, "working_copy_of_doc1")
+        self.assertEqual(wc.id, "working_copy_of_doc1")
         self.assertIn("working_copy_of_doc1", self.portal.workarea.objectIds())
 
     def test_container_folderOrder(self):
         """When an item is checked out and then back in, the original
         folder order is preserved."""
         container = self.portal.docs
         doc = container.doc1
@@ -198,17 +196,15 @@
         self.assertEqual(baseline["copy_of_an-image"].UID(), image_uid)
 
     def test_container_default_page_is_kept_in_folder(self):
         # Ensure that a default page that is checked out and back in is still
         # the default page.
         folder = self.portal.docs
         doc = folder.doc1
-        from Products.CMFDynamicViewFTI.interfaces import (
-            ISelectableBrowserDefault,
-        )  # noqa: C901
+        from Products.CMFDynamicViewFTI.interfaces import ISelectableBrowserDefault
 
         ISelectableBrowserDefault(folder).setDefaultPage("doc1")
         self.assertEqual(folder.getProperty("default_page", ""), "doc1")
         self.assertEqual(folder.getDefaultPage(), "doc1")
         # Note: when checking out to self.portal.workarea it surprisingly works
         # without changes.  But the default behavior in Plone is to check a
         # document out in its original folder, so that is what we check here.
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/tests/test_doctests.py` & `plone.app.iterate-5.0.2/plone/app/iterate/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/tests/test_interfaces.py` & `plone.app.iterate-5.0.2/plone/app/iterate/tests/test_interfaces.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.app.iterate.interfaces import IBaseline
 from plone.app.iterate.interfaces import ICheckinCheckoutPolicy
 from plone.app.iterate.interfaces import IIterateAware
 from plone.app.iterate.interfaces import IWorkingCopy
 from plone.app.iterate.testing import PLONEAPPITERATEDEX_INTEGRATION_TESTING
 from plone.app.testing import login
 from plone.app.testing import logout
@@ -23,15 +22,15 @@
 
     See: https://dev.plone.org/ticket/13163
     """
 
     layer = PLONEAPPITERATEDEX_INTEGRATION_TESTING
 
     def setUp(self):
-        super(TestObjectsProvideCorrectInterfaces, self).setUp()
+        super().setUp()
 
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         login(self.portal, TEST_USER_NAME)
 
         # create a folder where everything of this test suite should happen
         self.assertNotIn("test-folder", self.portal.objectIds())
@@ -41,15 +40,15 @@
 
         self.obj = createContentInContainer(self.folder, "Document")
 
     def tearDown(self):
         self.portal.manage_delObjects([self.folder.id])
         logout()
         setRoles(self.portal, TEST_USER_ID, ["Member"])
-        super(TestObjectsProvideCorrectInterfaces, self).tearDown()
+        super().tearDown()
 
     def do_checkout(self):
         policy = ICheckinCheckoutPolicy(self.obj)
         working_copy = policy.checkout(self.folder)
         return working_copy
 
     def do_cancel(self, working_copy):
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/tests/test_iterate.py` & `plone.app.iterate-5.0.2/plone/app/iterate/tests/test_iterate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
@@ -26,22 +25,21 @@
 from plone.app.iterate.interfaces import ICheckinCheckoutPolicy
 from plone.app.iterate.testing import PLONEAPPITERATEDEX_INTEGRATION_TESTING
 from plone.app.testing import login
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import TEST_USER_NAME
 from zc.relation.interfaces import ICatalog
-from zope.intid.interfaces import IIntIds
 from zope import component
+from zope.intid.interfaces import IIntIds
 
 import unittest
 
 
 class TestIterations(unittest.TestCase):
-
     layer = PLONEAPPITERATEDEX_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         login(self.portal, TEST_USER_NAME)
 
@@ -106,17 +104,15 @@
         self.assertEqual(new_position, original_position)
 
     def test_default_page_is_kept_in_folder(self):
         # Ensure that a default page that is checked out and back in is still
         # the default page.
         folder = self.portal.docs
         doc = folder.doc1
-        from Products.CMFDynamicViewFTI.interfaces import (
-            ISelectableBrowserDefault,
-        )  # noqa: C901
+        from Products.CMFDynamicViewFTI.interfaces import ISelectableBrowserDefault
 
         ISelectableBrowserDefault(folder).setDefaultPage("doc1")
         self.assertEqual(folder.getProperty("default_page", ""), "doc1")
         self.assertEqual(folder.getDefaultPage(), "doc1")
         # Note: when checking out to self.portal.workarea it surprisingly works
         # without changes.  But the default behavior in Plone is to check a
         # document out in its original folder, so that is what we check here.
@@ -216,17 +212,17 @@
         rels = list(catalog.findRelations({"from_id": obj_id}))
 
         self.assertEqual(len(rels), 0)
 
     def test_baseline_relations_updated_on_checkin(self):
         # Ensure that relations between the baseline and
         # and other objects are up-to-date on checkin
+        from z3c.relationfield import RelationValue
         from zope.event import notify
         from zope.lifecycleevent import ObjectModifiedEvent
-        from z3c.relationfield import RelationValue
 
         folder = self.portal.docs
         baseline = folder.doc1
         target = folder.doc2
 
         intids = component.getUtility(IIntIds)
         catalog = component.getUtility(ICatalog)
```

### Comparing `plone.app.iterate-5.0.1/plone/app/iterate/util.py` & `plone.app.iterate-5.0.2/plone/app/iterate/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##################################################################
 #
 # (C) Copyright 2006-2007 ObjectRealms, LLC
 # All Rights Reserved
 #
 # This file is part of iterate.
 #
```

### Comparing `plone.app.iterate-5.0.1/plone.app.iterate.egg-info/PKG-INFO` & `plone.app.iterate-5.0.2/plone.app.iterate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.iterate
-Version: 5.0.1
+Version: 5.0.2
 Summary: check-out/check-in staging for Plone
 Home-page: https://pypi.org/project/plone.app.iterate
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: check-out check-in staging
 Classifier: Development Status :: 5 - Production/Stable
@@ -132,14 +132,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.2 (2023-04-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5623f8b3)
+
+
 5.0.1 (2023-03-22)
 ------------------
 
 Bug fixes:
 
 
 - Use proper action icons in Plone 6.
@@ -501,15 +511,15 @@
 3.1.0 (2015-07-18)
 ------------------
 
 - Merge plone.app.stagingbehavior into plone.app.iterate without the
   behavior implementation. This is for Plone 5 iterate support.
   [vangheem]
 
-- Don't remove aquisition on object for getToolByName call.
+- Don't remove acquisition on object for getToolByName call.
   [tomgross]
 
 
 3.0.1 (2015-03-12)
 ------------------
 
 - Add permission names zcml/z3 style and load permission settings explicit
@@ -548,15 +558,15 @@
 - Replaced the "Locked" label with "Warning"
   [rristow]
 
 
 2.1.11 (2014-01-27)
 -------------------
 
-- setted lock timeout to MAX_TIMEOUT to avoid baseline unwanted unlock after 10 minutes
+- set lock timeout to MAX_TIMEOUT to avoid baseline unwanted unlock after 10 minutes
   [parruc]
 
 
 2.1.10 (2013-03-05)
 -------------------
 
 - Fixed error on checking in the working copy of an object linked in it's
```

### Comparing `plone.app.iterate-5.0.1/plone.app.iterate.egg-info/SOURCES.txt` & `plone.app.iterate-5.0.2/plone.app.iterate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.iterate-5.0.1/setup.py` & `plone.app.iterate-5.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
 
 LONG_DESCRIPTION = open("README.rst").read() + "\n" + open("CHANGES.rst").read() + "\n"
 
 setup(
     name="plone.app.iterate",
-    version="5.0.1",
+    version="5.0.2",
     description="check-out/check-in staging for Plone",
     long_description=LONG_DESCRIPTION,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
@@ -37,35 +36,41 @@
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
         "Acquisition",
         "DateTime",
         "plone.locking",
         "plone.memoize",
-        "Products.CMFCore",
         "Products.CMFEditions",
         "Products.CMFPlacefulWorkflow",
         "Products.DCWorkflow",
         "Products.GenericSetup>=1.8.2",
         "Products.statusmessages",
         "setuptools",
         "zope.annotation",
         "zope.component",
         "zope.event",
         "zope.i18nmessageid",
         "zope.interface",
         "zope.lifecycleevent",
         "zope.schema",
         "zope.viewlet",
+        "persistent",
+        "plone.base",
+        "plone.dexterity",
+        "plone.registry",
+        "z3c.relationfield",
+        "zc.relation",
+        "zope.intid",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
-            "plone.app.contenttypes",
-            "plone.app.robotframework",
+            "plone.app.contenttypes[test]",
+            "plone.testing",
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     """,
 )
```

