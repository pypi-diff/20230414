# Comparing `tmp/plone.api-2.0.1.tar.gz` & `tmp/plone.api-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.api-2.0.1.tar", last modified: Thu Jan 26 21:41:40 2023, max compression
+gzip compressed data, was "plone.api-2.0.2.tar", last modified: Thu Apr 13 22:55:19 2023, max compression
```

## Comparing `plone.api-2.0.1.tar` & `plone.api-2.0.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:41:40.817965 plone.api-2.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)    21134 2023-01-26 21:41:39.000000 plone.api-2.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       73 2023-01-26 21:41:39.000000 plone.api-2.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      679 2023-01-26 21:41:39.000000 plone.api-2.0.1/LICENSE
--rw-r--r--   0 maurits    (501) staff       (20)      357 2023-01-26 21:41:39.000000 plone.api-2.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    24696 2023-01-26 21:41:40.818080 plone.api-2.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1936 2023-01-26 21:41:39.000000 plone.api-2.0.1/README.md
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:41:40.804304 plone.api-2.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     6015 2023-01-26 21:41:39.000000 plone.api-2.0.1/docs/about.md
--rw-r--r--   0 maurits    (501) staff       (20)    13950 2023-01-26 21:41:39.000000 plone.api-2.0.1/docs/content.md
--rw-r--r--   0 maurits    (501) staff       (20)     3311 2023-01-26 21:41:39.000000 plone.api-2.0.1/docs/env.md
--rw-r--r--   0 maurits    (501) staff       (20)     9491 2023-01-26 21:41:39.000000 plone.api-2.0.1/docs/group.md
--rw-r--r--   0 maurits    (501) staff       (20)     2295 2023-01-26 21:41:39.000000 plone.api-2.0.1/docs/index.md
--rw-r--r--   0 maurits    (501) staff       (20)    11162 2023-01-26 21:41:39.000000 plone.api-2.0.1/docs/portal.md
--rw-r--r--   0 maurits    (501) staff       (20)     3938 2023-01-26 21:41:39.000000 plone.api-2.0.1/docs/relation.md
--rw-r--r--   0 maurits    (501) staff       (20)    10599 2023-01-26 21:41:39.000000 plone.api-2.0.1/docs/user.md
--rw-r--r--   0 maurits    (501) staff       (20)      578 2023-01-26 21:41:39.000000 plone.api-2.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      654 2023-01-26 21:41:40.818655 plone.api-2.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2004 2023-01-26 21:41:39.000000 plone.api-2.0.1/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:41:40.798060 plone.api-2.0.1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:41:40.804580 plone.api-2.0.1/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:41:40.810246 plone.api-2.0.1/src/plone/api/
--rw-r--r--   0 maurits    (501) staff       (20)      193 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)       98 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    22260 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/content.py
--rw-r--r--   0 maurits    (501) staff       (20)     8042 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/env.py
--rw-r--r--   0 maurits    (501) staff       (20)     1051 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/exc.py
--rw-r--r--   0 maurits    (501) staff       (20)    11142 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/group.py
--rw-r--r--   0 maurits    (501) staff       (20)    13910 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/portal.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:41:40.798457 plone.api-2.0.1/src/plone/api/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:41:40.811007 plone.api-2.0.1/src/plone/api/profiles/testfixture/
--rw-r--r--   0 maurits    (501) staff       (20)      229 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/profiles/testfixture/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:41:40.811593 plone.api-2.0.1/src/plone/api/profiles/testfixture/types/
--rw-r--r--   0 maurits    (501) staff       (20)     1734 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1722 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)      210 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/profiles/testfixture/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)    11367 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/relation.py
--rw-r--r--   0 maurits    (501) staff       (20)      578 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/testing.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:41:40.815545 plone.api-2.0.1/src/plone/api/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      106 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/Dexterity_Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      106 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/Dexterity_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1659 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/base.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:41:40.817767 plone.api-2.0.1/src/plone/api/tests/doctests/
--rw-r--r--   0 maurits    (501) staff       (20)     6015 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/doctests/about.md
--rw-r--r--   0 maurits    (501) staff       (20)    13950 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/doctests/content.md
--rw-r--r--   0 maurits    (501) staff       (20)     3311 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/doctests/env.md
--rw-r--r--   0 maurits    (501) staff       (20)     9491 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/doctests/group.md
--rw-r--r--   0 maurits    (501) staff       (20)    11162 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/doctests/portal.md
--rw-r--r--   0 maurits    (501) staff       (20)     3938 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/doctests/relation.md
--rw-r--r--   0 maurits    (501) staff       (20)    10599 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/doctests/user.md
--rw-r--r--   0 maurits    (501) staff       (20)    48875 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/test_content.py
--rw-r--r--   0 maurits    (501) staff       (20)     3318 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)    17634 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/test_env.py
--rw-r--r--   0 maurits    (501) staff       (20)    26958 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/test_group.py
--rw-r--r--   0 maurits    (501) staff       (20)    30940 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/test_portal.py
--rw-r--r--   0 maurits    (501) staff       (20)    14255 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/test_relation.py
--rw-r--r--   0 maurits    (501) staff       (20)    35670 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/test_user.py
--rw-r--r--   0 maurits    (501) staff       (20)     9812 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/tests/test_validation.py
--rw-r--r--   0 maurits    (501) staff       (20)    14825 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/user.py
--rw-r--r--   0 maurits    (501) staff       (20)     4862 2023-01-26 21:41:39.000000 plone.api-2.0.1/src/plone/api/validation.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:41:40.806829 plone.api-2.0.1/src/plone.api.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    24696 2023-01-26 21:41:40.000000 plone.api-2.0.1/src/plone.api.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1682 2023-01-26 21:41:40.000000 plone.api-2.0.1/src/plone.api.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-01-26 21:41:40.000000 plone.api-2.0.1/src/plone.api.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-01-26 21:41:40.000000 plone.api-2.0.1/src/plone.api.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-01-26 21:41:40.000000 plone.api-2.0.1/src/plone.api.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      272 2023-01-26 21:41:40.000000 plone.api-2.0.1/src/plone.api.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-01-26 21:41:40.000000 plone.api-2.0.1/src/plone.api.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3625 2023-01-26 21:41:39.000000 plone.api-2.0.1/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.839508 plone.api-2.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)    21316 2023-04-13 22:55:19.000000 plone.api-2.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       73 2023-04-13 22:55:19.000000 plone.api-2.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      679 2023-04-13 22:55:19.000000 plone.api-2.0.2/LICENSE
+-rw-r--r--   0 maurits    (501) staff       (20)      357 2023-04-13 22:55:19.000000 plone.api-2.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    24878 2023-04-13 22:55:19.839653 plone.api-2.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1936 2023-04-13 22:55:19.000000 plone.api-2.0.2/README.md
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.825780 plone.api-2.0.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     6015 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/about.md
+-rw-r--r--   0 maurits    (501) staff       (20)    13950 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/content.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3311 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/env.md
+-rw-r--r--   0 maurits    (501) staff       (20)     9491 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/group.md
+-rw-r--r--   0 maurits    (501) staff       (20)     2295 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/index.md
+-rw-r--r--   0 maurits    (501) staff       (20)    11162 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/portal.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/relation.md
+-rw-r--r--   0 maurits    (501) staff       (20)    10599 2023-04-13 22:55:19.000000 plone.api-2.0.2/docs/user.md
+-rw-r--r--   0 maurits    (501) staff       (20)      578 2023-04-13 22:55:19.000000 plone.api-2.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      654 2023-04-13 22:55:19.840304 plone.api-2.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2004 2023-04-13 22:55:19.000000 plone.api-2.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.818556 plone.api-2.0.2/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.826110 plone.api-2.0.2/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.831939 plone.api-2.0.2/src/plone/api/
+-rw-r--r--   0 maurits    (501) staff       (20)      193 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)       98 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    22260 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8042 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/env.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1051 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/exc.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11142 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/group.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13908 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/portal.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.818908 plone.api-2.0.2/src/plone/api/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.832653 plone.api-2.0.2/src/plone/api/profiles/testfixture/
+-rw-r--r--   0 maurits    (501) staff       (20)      229 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/profiles/testfixture/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.833123 plone.api-2.0.2/src/plone/api/profiles/testfixture/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     1734 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1722 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      210 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/profiles/testfixture/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)    11428 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/relation.py
+-rw-r--r--   0 maurits    (501) staff       (20)      578 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/testing.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.836864 plone.api-2.0.2/src/plone/api/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)      106 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/Dexterity_Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      106 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/Dexterity_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1658 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/base.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.839284 plone.api-2.0.2/src/plone/api/tests/doctests/
+-rw-r--r--   0 maurits    (501) staff       (20)     6015 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/about.md
+-rw-r--r--   0 maurits    (501) staff       (20)    13950 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/content.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3311 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/env.md
+-rw-r--r--   0 maurits    (501) staff       (20)     9491 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/group.md
+-rw-r--r--   0 maurits    (501) staff       (20)    11162 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/portal.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/relation.md
+-rw-r--r--   0 maurits    (501) staff       (20)    10599 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/doctests/user.md
+-rw-r--r--   0 maurits    (501) staff       (20)    48874 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3318 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17633 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_env.py
+-rw-r--r--   0 maurits    (501) staff       (20)    26958 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_group.py
+-rw-r--r--   0 maurits    (501) staff       (20)    30938 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_portal.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18992 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_relation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    35670 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_user.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9812 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/tests/test_validation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14825 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/user.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4862 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone/api/validation.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 22:55:19.828464 plone.api-2.0.2/src/plone.api.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    24878 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1682 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      272 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 22:55:19.000000 plone.api-2.0.2/src/plone.api.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3625 2023-04-13 22:55:19.000000 plone.api-2.0.2/tox.ini
```

### Comparing `plone.api-2.0.1/CHANGES.rst` & `plone.api-2.0.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,29 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.2 (2023-04-14)
+------------------
+
+Bug fixes:
+
+
+- Fix deletion of relations by relation name. @ksuess (#501)
+
+
+Documentation:
+
+
+- Update link for Training. @stevepiercy (#503)
+
+
 2.0.1 (2023-01-26)
 ------------------
 
 Documentation:
 
 
 - Switch to 6.docs.plone.org (was 6.dev-docs.plone.org)
```

### Comparing `plone.api-2.0.1/LICENSE` & `plone.api-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/PKG-INFO` & `plone.api-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.api
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Plone API.
 Home-page: https://github.com/plone/plone.api
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone api
 Platform: Any
@@ -79,14 +79,29 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.2 (2023-04-14)
+------------------
+
+Bug fixes:
+
+
+- Fix deletion of relations by relation name. @ksuess (#501)
+
+
+Documentation:
+
+
+- Update link for Training. @stevepiercy (#503)
+
+
 2.0.1 (2023-01-26)
 ------------------
 
 Documentation:
 
 
 - Switch to 6.docs.plone.org (was 6.dev-docs.plone.org)
```

### Comparing `plone.api-2.0.1/README.md` & `plone.api-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/docs/about.md` & `plone.api-2.0.2/docs/about.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/docs/content.md` & `plone.api-2.0.2/docs/content.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/docs/env.md` & `plone.api-2.0.2/docs/env.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/docs/group.md` & `plone.api-2.0.2/docs/group.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/docs/index.md` & `plone.api-2.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/docs/portal.md` & `plone.api-2.0.2/docs/portal.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/docs/relation.md` & `plone.api-2.0.2/docs/relation.md`

 * *Files 0% similar despite different names*

```diff
@@ -135,8 +135,8 @@
 ```
 
 If a deleted relation is based on a `RelationChoice` or `RelationList` field on the source object, the value of the field is removed/updated accordingly.
 
 ## Further reading
 
 For more information on possible flags and usage options please see the full {ref}`plone-api-relation` specification.
-For more information on relations read the relevant [chapter in the Mastering Plone training](https://training.plone.org/5/mastering-plone/relations.html).
+For more information on relations read the relevant [chapter in the Mastering Plone training](https://training.plone.org/mastering-plone/relations.html).
```

### Comparing `plone.api-2.0.1/docs/user.md` & `plone.api-2.0.2/docs/user.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/pyproject.toml` & `plone.api-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/setup.cfg` & `plone.api-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/setup.py` & `plone.api-2.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 long_description = (
     read("README.md") + "\n\n" + read("CHANGES.rst") + "\n\n" + read("LICENSE")
 )
 
-version = "2.0.1"
+version = "2.0.2"
 
 setup(
     name="plone.api",
     version=version,
     description="A Plone API.",
     long_description=long_description,
     author="Plone Foundation",
```

### Comparing `plone.api-2.0.1/src/plone/api/content.py` & `plone.api-2.0.2/src/plone/api/content.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/env.py` & `plone.api-2.0.2/src/plone/api/env.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/exc.py` & `plone.api-2.0.2/src/plone/api/exc.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/group.py` & `plone.api-2.0.2/src/plone/api/group.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/portal.py` & `plone.api-2.0.2/src/plone/api/portal.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,14 @@
         :class:`~plone.api.exc.MissingParameterError`,
         :class:`~plone.api.exc.InvalidParameterError`
     :Example: :ref:`portal-get-tool-example`
     """
     try:
         return getToolByName(get(), name)
     except AttributeError:
-
         # get a list of all tools to display their names in the error msg
         portal = get()
         tools = []
         for id in portal.objectIds():
             if id.startswith("portal_"):
                 tools.append(id)
 
@@ -361,15 +360,14 @@
                     name=name,
                     of_class=str(field_type.__class__),
                     of_type=type(value),
                 ),
             )
 
     elif isinstance(name, str):
-
         # confirm that the record exists before setting the value
         get_registry_record(name)
 
         registry[name] = value
 
 
 def get_default_language():
```

### Comparing `plone.api-2.0.1/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml` & `plone.api-2.0.2/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml` & `plone.api-2.0.2/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/relation.py` & `plone.api-2.0.2/src/plone/api/relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,26 +277,27 @@
     intids = getUtility(IIntIds)
     if source is not None:
         query["from_id"] = intids.getId(source)
     if target is not None:
         query["to_id"] = intids.getId(target)
     if relationship is not None:
         query["from_attribute"] = relationship
-    for rel in relation_catalog.findRelations(query):
+    # We'll change the bucket in the loop
+    for rel in [rel for rel in relation_catalog.findRelations(query)]:
         source = rel.from_object
         from_attribute = rel.from_attribute
         field_and_schema = _get_field_and_schema_for_fieldname(
             from_attribute,
             source.portal_type,
         )
         if field_and_schema is None:
             # The relationship is not the name of a dexterity field.
             # Only purge relation from relation-catalog.
             relation_catalog.unindex(rel)
-            return
+            continue
 
         target = rel.to_object
         field, _schema = field_and_schema
         if isinstance(field, RelationList):
             logger.info(
                 "Remove relation from %s to %s from relationlist %s",
                 source.absolute_url(),
```

### Comparing `plone.api-2.0.1/src/plone/api/testing.zcml` & `plone.api-2.0.2/src/plone/api/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/tests/base.py` & `plone.api-2.0.2/src/plone/api/tests/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from plone.app.testing import PloneSandboxLayer
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import TEST_USER_NAME
 
 
 class PloneApiLayer(PloneSandboxLayer):
-
     defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         """Prepare Zope instance by loading appropriate ZCMLs."""
         import plone.app.dexterity
 
         self.loadZCML(package=plone.app.dexterity)
```

### Comparing `plone.api-2.0.1/src/plone/api/tests/doctests/about.md` & `plone.api-2.0.2/src/plone/api/tests/doctests/about.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/tests/doctests/content.md` & `plone.api-2.0.2/src/plone/api/tests/doctests/content.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/tests/doctests/env.md` & `plone.api-2.0.2/src/plone/api/tests/doctests/env.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/tests/doctests/group.md` & `plone.api-2.0.2/src/plone/api/tests/doctests/group.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/tests/doctests/portal.md` & `plone.api-2.0.2/src/plone/api/tests/doctests/portal.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/tests/doctests/relation.md` & `plone.api-2.0.2/src/plone/api/tests/doctests/relation.md`

 * *Files 0% similar despite different names*

```diff
@@ -135,8 +135,8 @@
 ```
 
 If a deleted relation is based on a `RelationChoice` or `RelationList` field on the source object, the value of the field is removed/updated accordingly.
 
 ## Further reading
 
 For more information on possible flags and usage options please see the full {ref}`plone-api-relation` specification.
-For more information on relations read the relevant [chapter in the Mastering Plone training](https://training.plone.org/5/mastering-plone/relations.html).
+For more information on relations read the relevant [chapter in the Mastering Plone training](https://training.plone.org/mastering-plone/relations.html).
```

### Comparing `plone.api-2.0.1/src/plone/api/tests/doctests/user.md` & `plone.api-2.0.2/src/plone/api/tests/doctests/user.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/tests/test_content.py` & `plone.api-2.0.2/src/plone/api/tests/test_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -1125,15 +1125,14 @@
             "portal_type": "Document",
             "path": {"query": path},
         }
         documents = api.content.find(**query)
         self.assertEqual(len(documents), 0)
 
     def test_find_parse_object_provides_query(self):
-
         parse = api.content._parse_object_provides_query
 
         # single interface
         self.assertDictEqual(
             parse(IContentish),
             {
                 "query": [IContentish.__identifier__],
```

### Comparing `plone.api-2.0.1/src/plone/api/tests/test_doctests.py` & `plone.api-2.0.2/src/plone/api/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/tests/test_env.py` & `plone.api-2.0.2/src/plone/api/tests/test_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 
 class TestException(Exception):
     """Test exception."""
 
 
 class HasProtectedMethods(SimpleItem):
-
     security = AccessControl.ClassSecurityInfo()
 
     def __init__(self, id):
         self.id = id
 
     @security.public
     def public_method(self):
```

### Comparing `plone.api-2.0.1/src/plone/api/tests/test_group.py` & `plone.api-2.0.2/src/plone/api/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/tests/test_portal.py` & `plone.api-2.0.2/src/plone/api/tests/test_portal.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,28 +33,26 @@
     from email import message_from_string as message_from_bytes
 
 
 HAS_PLONE5 = parse_version(env.plone_version()) >= parse_version("5.0b2")
 
 
 class IMyRegistrySettings(Interface):
-
     field_one = schema.TextLine(
         title="something",
         description="something else",
     )
 
     field_two = schema.TextLine(
         title="something",
         description="something else",
     )
 
 
 class IMyOtherRegistrySettings(Interface):
-
     field_three = schema.TextLine(
         title="something",
         description="something else",
     )
 
 
 class ImNotAnInterface:
```

### Comparing `plone.api-2.0.1/src/plone/api/tests/test_user.py` & `plone.api-2.0.2/src/plone/api/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/tests/test_validation.py` & `plone.api-2.0.2/src/plone/api/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/user.py` & `plone.api-2.0.2/src/plone/api/user.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone/api/validation.py` & `plone.api-2.0.2/src/plone/api/validation.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/src/plone.api.egg-info/PKG-INFO` & `plone.api-2.0.2/src/plone.api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.api
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Plone API.
 Home-page: https://github.com/plone/plone.api
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone api
 Platform: Any
@@ -79,14 +79,29 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.2 (2023-04-14)
+------------------
+
+Bug fixes:
+
+
+- Fix deletion of relations by relation name. @ksuess (#501)
+
+
+Documentation:
+
+
+- Update link for Training. @stevepiercy (#503)
+
+
 2.0.1 (2023-01-26)
 ------------------
 
 Documentation:
 
 
 - Switch to 6.docs.plone.org (was 6.dev-docs.plone.org)
```

### Comparing `plone.api-2.0.1/src/plone.api.egg-info/SOURCES.txt` & `plone.api-2.0.2/src/plone.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.1/tox.ini` & `plone.api-2.0.2/tox.ini`

 * *Files identical despite different names*

