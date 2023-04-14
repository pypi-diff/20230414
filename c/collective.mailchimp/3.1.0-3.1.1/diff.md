# Comparing `tmp/collective.mailchimp-3.1.0.tar.gz` & `tmp/collective.mailchimp-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.mailchimp-3.1.0.tar", last modified: Mon Jan 13 13:13:53 2020, max compression
+gzip compressed data, was "collective.mailchimp-3.1.1.tar", last modified: Fri Apr 14 09:09:56 2023, max compression
```

## Comparing `collective.mailchimp-3.1.0.tar` & `collective.mailchimp-3.1.1.tar`

### file list

```diff
@@ -1,104 +1,98 @@
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/
--rw-r--r--   0 timo       (501) staff       (20)     5663 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/CHANGES.rst
--rw-r--r--   0 timo       (501) staff       (20)      154 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/CONTRIBUTORS.rst
--rw-r--r--   0 timo       (501) staff       (20)      133 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/MANIFEST.in
--rw-r--r--   0 timo       (501) staff       (20)    16655 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/PKG-INFO
--rw-r--r--   0 timo       (501) staff       (20)     5968 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/README.rst
--rw-r--r--   0 timo       (501) staff       (20)       37 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/TODO.txt
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/docs/
--rw-r--r--   0 timo       (501) staff       (20)     1513 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/docs/INSTALL.txt
--rw-r--r--   0 timo       (501) staff       (20)    17987 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/docs/LICENSE.GPL
--rw-r--r--   0 timo       (501) staff       (20)      737 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/docs/LICENSE.txt
--rw-r--r--   0 timo       (501) staff       (20)      138 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/requirements.txt
--rw-r--r--   0 timo       (501) staff       (20)      297 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/setup.cfg
--rw-r--r--   0 timo       (501) staff       (20)     2103 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/setup.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/
--rw-r--r--   0 timo       (501) staff       (20)      269 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/__init__.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/
--rw-r--r--   0 timo       (501) staff       (20)      115 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/__init__.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/
--rw-r--r--   0 timo       (501) staff       (20)        0 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/__init__.py
--rw-r--r--   0 timo       (501) staff       (20)     1494 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/configure.zcml
--rw-r--r--   0 timo       (501) staff       (20)     5789 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/controlpanel.pt
--rw-r--r--   0 timo       (501) staff       (20)     2618 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/controlpanel.py
--rw-r--r--   0 timo       (501) staff       (20)     1409 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/extender.py
--rw-r--r--   0 timo       (501) staff       (20)      381 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/extender.zcml
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/images/
--rw-r--r--   0 timo       (501) staff       (20)      998 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/images/mailchimp.gif
--rw-r--r--   0 timo       (501) staff       (20)    10988 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/newsletter.py
--rw-r--r--   0 timo       (501) staff       (20)      596 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/portlet.pt
--rw-r--r--   0 timo       (501) staff       (20)     3299 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/portlet.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/stylesheets/
--rw-r--r--   0 timo       (501) staff       (20)      170 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/stylesheets/mailchimp.css
--rw-r--r--   0 timo       (501) staff       (20)     3371 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/browser/z3cformhelpers.py
--rw-r--r--   0 timo       (501) staff       (20)     1702 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/configure.zcml
--rw-r--r--   0 timo       (501) staff       (20)     1765 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/exceptions.py
--rw-r--r--   0 timo       (501) staff       (20)     7700 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/interfaces.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/
--rw-r--r--   0 timo       (501) staff       (20)     9642 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/collective.mailchimp.pot
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/de/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/de/LC_MESSAGES/
--rw-r--r--   0 timo       (501) staff       (20)     2601 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/de/LC_MESSAGES/collective.mailchimp.mo
--rw-r--r--   0 timo       (501) staff       (20)    10455 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/de/LC_MESSAGES/collective.mailchimp.po
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/fr/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/fr/LC_MESSAGES/
--rw-r--r--   0 timo       (501) staff       (20)     4170 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/fr/LC_MESSAGES/collective.mailchimp.mo
--rw-r--r--   0 timo       (501) staff       (20)    11768 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/fr/LC_MESSAGES/collective.mailchimp.po
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/it/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/it/LC_MESSAGES/
--rw-r--r--   0 timo       (501) staff       (20)     5449 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/it/LC_MESSAGES/collective.mailchimp.mo
--rw-r--r--   0 timo       (501) staff       (20)    11997 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/it/LC_MESSAGES/collective.mailchimp.po
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/nl/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/nl/LC_MESSAGES/
--rw-r--r--   0 timo       (501) staff       (20)     6274 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/nl/LC_MESSAGES/collective.mailchimp.mo
--rw-r--r--   0 timo       (501) staff       (20)    12577 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/nl/LC_MESSAGES/collective.mailchimp.po
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/pt_BR/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 timo       (501) staff       (20)     5677 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/collective.mailchimp.mo
--rw-r--r--   0 timo       (501) staff       (20)    12196 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/collective.mailchimp.po
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/ro/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/ro/LC_MESSAGES/
--rw-r--r--   0 timo       (501) staff       (20)     2181 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/ro/LC_MESSAGES/collective.mailchimp.mo
--rw-r--r--   0 timo       (501) staff       (20)    10354 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locales/ro/LC_MESSAGES/collective.mailchimp.po
--rw-r--r--   0 timo       (501) staff       (20)    13365 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/locator.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/default/
--rw-r--r--   0 timo       (501) staff       (20)      135 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/default/browserlayer.xml
--rw-r--r--   0 timo       (501) staff       (20)      625 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/default/controlpanel.xml
--rw-r--r--   0 timo       (501) staff       (20)      177 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/default/cssregistry.xml
--rw-r--r--   0 timo       (501) staff       (20)      165 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/default/metadata.xml
--rw-r--r--   0 timo       (501) staff       (20)      172 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/default/portlets.xml
--rw-r--r--   0 timo       (501) staff       (20)      724 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/default/registry.xml
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/uninstall/
--rw-r--r--   0 timo       (501) staff       (20)       85 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 timo       (501) staff       (20)      295 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 timo       (501) staff       (20)      380 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/uninstall/registry.xml
--rw-r--r--   0 timo       (501) staff       (20)     5212 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/testing.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/
--rw-r--r--   0 timo       (501) staff       (20)        0 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/__init__.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/data/
--rw-r--r--   0 timo       (501) staff       (20)     2780 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/data/account.json
--rw-r--r--   0 timo       (501) staff       (20)     8457 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/data/interests.json
--rw-r--r--   0 timo       (501) staff       (20)     6458 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/data/lists.json
--rw-r--r--   0 timo       (501) staff       (20)     2787 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/data/lists_interest_categories.json
--rw-r--r--   0 timo       (501) staff       (20)     3262 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/data/member.json
--rw-r--r--   0 timo       (501) staff       (20)     2586 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_controlpanel.py
--rw-r--r--   0 timo       (501) staff       (20)     1566 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_exceptions.py
--rw-r--r--   0 timo       (501) staff       (20)     4015 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_locator.py
--rw-r--r--   0 timo       (501) staff       (20)     2410 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_mock_requests.py
--rw-r--r--   0 timo       (501) staff       (20)     5905 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_newsletter.py
--rw-r--r--   0 timo       (501) staff       (20)     7115 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_portlet.py
--rw-r--r--   0 timo       (501) staff       (20)     3637 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_setup.py
--rw-r--r--   0 timo       (501) staff       (20)     1162 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/upgrades.py
--rw-r--r--   0 timo       (501) staff       (20)     1150 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/upgrades.zcml
--rw-r--r--   0 timo       (501) staff       (20)     1806 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective/mailchimp/vocabularies.py
-drwxr-xr-x   0 timo       (501) staff       (20)        0 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective.mailchimp.egg-info/
--rw-r--r--   0 timo       (501) staff       (20)    16655 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective.mailchimp.egg-info/PKG-INFO
--rw-r--r--   0 timo       (501) staff       (20)     3591 2020-01-13 13:13:53.000000 collective.mailchimp-3.1.0/src/collective.mailchimp.egg-info/SOURCES.txt
--rw-r--r--   0 timo       (501) staff       (20)        1 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective.mailchimp.egg-info/dependency_links.txt
--rw-r--r--   0 timo       (501) staff       (20)       53 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective.mailchimp.egg-info/entry_points.txt
--rw-r--r--   0 timo       (501) staff       (20)       11 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective.mailchimp.egg-info/namespace_packages.txt
--rw-r--r--   0 timo       (501) staff       (20)        1 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective.mailchimp.egg-info/not-zip-safe
--rw-r--r--   0 timo       (501) staff       (20)      135 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective.mailchimp.egg-info/requires.txt
--rw-r--r--   0 timo       (501) staff       (20)       11 2020-01-13 13:13:52.000000 collective.mailchimp-3.1.0/src/collective.mailchimp.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.523363 collective.mailchimp-3.1.1/
+-rw-r--r--   0 maurits    (501) staff       (20)     5765 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      169 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/CONTRIBUTORS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      133 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    13040 2023-04-14 09:09:56.523481 collective.mailchimp-3.1.1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     5916 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       37 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/TODO.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.505353 collective.mailchimp-3.1.1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1513 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      737 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      138 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/requirements.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      297 2023-04-14 09:09:56.523965 collective.mailchimp-3.1.1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2180 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.498453 collective.mailchimp-3.1.1/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.505730 collective.mailchimp-3.1.1/src/collective/
+-rw-r--r--   0 maurits    (501) staff       (20)      269 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.510357 collective.mailchimp-3.1.1/src/collective/mailchimp/
+-rw-r--r--   0 maurits    (501) staff       (20)      115 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.513560 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1494 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5789 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/controlpanel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2618 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1409 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/extender.py
+-rw-r--r--   0 maurits    (501) staff       (20)      381 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/extender.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.513811 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/images/
+-rw-r--r--   0 maurits    (501) staff       (20)      998 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/images/mailchimp.gif
+-rw-r--r--   0 maurits    (501) staff       (20)    11188 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/newsletter.py
+-rw-r--r--   0 maurits    (501) staff       (20)      596 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/portlet.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3299 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/portlet.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.514134 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/stylesheets/
+-rw-r--r--   0 maurits    (501) staff       (20)      170 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/stylesheets/mailchimp.css
+-rw-r--r--   0 maurits    (501) staff       (20)     3371 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/z3cformhelpers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1702 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1765 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/exceptions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7898 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.514455 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/
+-rw-r--r--   0 maurits    (501) staff       (20)     9642 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/collective.mailchimp.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.499834 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/de/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.514713 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/de/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    10455 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/de/LC_MESSAGES/collective.mailchimp.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.500090 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/fr/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.514967 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    11768 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/fr/LC_MESSAGES/collective.mailchimp.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.500348 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/it/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.515222 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/it/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    11997 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/it/LC_MESSAGES/collective.mailchimp.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.500721 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.515605 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    12577 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/nl/LC_MESSAGES/collective.mailchimp.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.501021 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/pt_BR/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.515905 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    12196 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/collective.mailchimp.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.501320 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/ro/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.516174 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/ro/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    10354 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/ro/LC_MESSAGES/collective.mailchimp.po
+-rw-r--r--   0 maurits    (501) staff       (20)    13365 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locator.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.501769 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.517825 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      135 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      625 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      177 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/cssregistry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      165 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      172 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      724 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.518832 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      295 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      380 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/uninstall/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     5212 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.521279 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.523153 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/
+-rw-r--r--   0 maurits    (501) staff       (20)     2780 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/account.json
+-rw-r--r--   0 maurits    (501) staff       (20)     8457 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/interests.json
+-rw-r--r--   0 maurits    (501) staff       (20)     6458 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/lists.json
+-rw-r--r--   0 maurits    (501) staff       (20)     2787 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/lists_interest_categories.json
+-rw-r--r--   0 maurits    (501) staff       (20)     3262 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/member.json
+-rw-r--r--   0 maurits    (501) staff       (20)     2586 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1566 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_exceptions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4015 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_locator.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2410 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_mock_requests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5905 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_newsletter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7115 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_portlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3637 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1162 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1150 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/upgrades.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1806 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.507869 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    13040 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3156 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      135 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.mailchimp-3.1.0/CHANGES.rst` & `collective.mailchimp-3.1.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+3.1.1 (2023-04-14)
+------------------
+
+- Fix controlpanel field validation for Plone 6
+  [agitator]
+
+
 3.1.0 (2020-01-13)
 ------------------
 
 New Features:
 
 - Add Plone 5.2 and Python 3.7 classifiers.
   [timo]
```

### Comparing `collective.mailchimp-3.1.0/README.rst` & `collective.mailchimp-3.1.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -133,17 +133,14 @@
 Please report bugs to the `issue tracker on github`_.
 
 
 Credits
 =======
 
 .. image:: https://raw.githubusercontent.com/collective/collective.mailchimp/master/kitconcept.png
-   :height: 461px
-   :width: 100px
-   :scale: 100 %
    :alt: kitconcept
    :align: center
    :target: https://www.kitconcept.com/
 
 This plugin is developed and maintained by `kitconcept`_.
 
 If you are having issues, please let us know.
```

### Comparing `collective.mailchimp-3.1.0/docs/INSTALL.txt` & `collective.mailchimp-3.1.1/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/docs/LICENSE.GPL` & `collective.mailchimp-3.1.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/docs/LICENSE.txt` & `collective.mailchimp-3.1.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/setup.py` & `collective.mailchimp-3.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     + open('CHANGES.rst').read()
     + '\n'
 )
 
 
 setup(
     name='collective.mailchimp',
-    version='3.1.0',
+    version='3.1.1',
     description="MailChimp integration for Plone.",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
@@ -49,14 +49,15 @@
     url='https://pypi.python.org/pypi/collective.mailchimp',
     license='GPL version 2',
     packages=find_packages('src', exclude=['ez_setup']),
     namespace_packages=['collective'],
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
+    python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*',
     install_requires=[
         'setuptools',
         'Products.CMFPlone',
         'plone.app.portlets',
         'plone.app.registry',
         'plone.app.upgrade',
         'requests',
```

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/browser/configure.zcml` & `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/browser/controlpanel.pt` & `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/browser/controlpanel.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/browser/extender.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/extender.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/browser/images/mailchimp.gif` & `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/images/mailchimp.gif`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/browser/newsletter.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/newsletter.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,26 +85,29 @@
         if errors:
             self.status = self.formErrorsMessage
             return
 
         # Retrieve list_id either from a hidden field in the form or fetch
         # the first list from mailchimp.
         list_id = data.get('list_id') or self.mailchimp.default_list_id()
+        # list_id has to be updated for merge_fields=data to work if None
+        if "list_id" in data and not data.get('list_id'):
+            data['list_id'] = list_id
 
         # interest groups
         interests = {}
         interest_groups = data.pop('interest_groups', [])
         if self.available_interest_groups and interest_groups:
             # Create dictionary with as keys the interest groups, and as
             # values always True.
             interests = dict.fromkeys(interest_groups, True)
 
         # Use email_type if one is provided by the form, if not choose the
         # default email type from the control panel settings.
-        email_type = data.get('email_type', 'HTML')
+        email_type = data.get('email_type') or self.mailchimp_settings.email_type
 
         # Subscribe to MailChimp list
         try:
             self.mailchimp.subscribe(
                 list_id=list_id,
                 email_address=data['email'],
                 email_type=email_type,
```

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/browser/portlet.pt` & `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/portlet.pt`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/browser/portlet.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/portlet.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/browser/z3cformhelpers.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/z3cformhelpers.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/configure.zcml` & `collective.mailchimp-3.1.1/src/collective/mailchimp/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/exceptions.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/exceptions.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/interfaces.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/interfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         ),
         required=False,
     )
 
     email_type = schema.Choice(
         title=_(u"Mail format"),
         vocabulary="collective.mailchimp.vocabularies.EmailType",
-        default="text",
+        default="html",
         required=False,
     )
 
     list_id = schema.TextLine(title=_(u"List ID"), required=False)
 
 
 class INewsletterUnsubscribe(Interface):
@@ -156,94 +156,94 @@
             + u"Authorized Apps and copy the API Key to this field.",
         ),
         default=u"",
         required=True,
     )
 
     email_type = schema.Choice(
-        title=_(u"email_type"),
+        title=_(u"email_type", default=u"Email type"),
         description=_(
             u"help_email_type",
             default=u"Email type preference for the email (html, text, or "
             u"mobile defaults to html)",
         ),
         vocabulary="collective.mailchimp.vocabularies.EmailType",
         default="html",
-        required=True,
+        required=False,
     )
 
     email_type_is_optional = schema.Bool(
-        title=_(u"email_type_is_optional"),
+        title=_(u"email_type_is_optional", default=u"Email type is optional"),
         description=_(
             u"help_email_type_is_optional",
             default=u"Let users choose their email type preference in the "
             u"newsletter subscription form.",
         ),
-        required=True,
+        required=False,
         default=False,
     )
 
     default_list = schema.Choice(
-        title=_(u"default_list"),
+        title=_(u"default_list", default=u"Default list"),
         description=_(
             u"help_default_list",
             default=u"Default list which is used in the @@newsletter view if "
             u"no list_id param is provided.",
         ),
         vocabulary="collective.mailchimp.vocabularies.AvailableLists",
         required=False,
     )
 
     double_optin = schema.Bool(
-        title=_(u"double_optin"),
+        title=_(u"double_optin", default=u"Double opt-in"),
         description=_(
             u"help_double_optin",
             default=u"Flag to control whether a double opt-in confirmation "
             u"message is sent, defaults to true. Abusing this may "
             u"cause your account to be suspended.",
         ),
-        required=True,
+        required=False,
         default=True,
     )
 
     update_existing = schema.Bool(
-        title=_(u"update_existing"),
+        title=_(u"update_existing", default=u"Update existing"),
         description=_(
             u"help_update_existing",
             default=u"Flag to control whether existing subscribers should be "
             u"updated instead of throwing an error, defaults to false",
         ),
-        required=True,
+        required=False,
         default=False,
     )
 
     replace_interests = schema.Bool(
-        title=_(u"replace_interests"),
+        title=_(u"replace_interests", default=u"Replace interests"),
         description=_(
             u"help_replace_interests",
             default=u"Flag to determine whether we replace the interest "
             u"groups with the groups provided or we add the provided"
             u"groups to the member's interest groups (optional, "
             u"defaults to true)",
         ),
-        required=True,
+        required=False,
         default=True,
     )
 
     send_welcome = schema.Bool(
-        title=_(u"send_welcome"),
+        title=_(u"send_welcome", default=u"Send welcome"),
         description=_(
             u"help_send_welcome",
             default=u"If your double_optin is false and this is true, we "
             u"will send your lists Welcome Email if this subscribe "
             u"succeeds - this will *not* fire if we end up updating "
             u"an existing subscriber. If double_optin is true, this "
             u"has no effect. defaults to false.",
         ),
-        required=True,
+        required=False,
         default=False,
     )
 
     @invariant
     def valid_api_key(data):
         if len(data.api_key) == 0:
             return
```

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/locales/collective.mailchimp.pot` & `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/collective.mailchimp.pot`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/locales/de/LC_MESSAGES/collective.mailchimp.po` & `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/de/LC_MESSAGES/collective.mailchimp.po`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/locales/fr/LC_MESSAGES/collective.mailchimp.po` & `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/fr/LC_MESSAGES/collective.mailchimp.po`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/locales/it/LC_MESSAGES/collective.mailchimp.po` & `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/it/LC_MESSAGES/collective.mailchimp.po`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/locales/nl/LC_MESSAGES/collective.mailchimp.po` & `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/nl/LC_MESSAGES/collective.mailchimp.po`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/collective.mailchimp.po` & `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/collective.mailchimp.po`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/locales/ro/LC_MESSAGES/collective.mailchimp.po` & `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/ro/LC_MESSAGES/collective.mailchimp.po`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/locator.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/locator.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/default/controlpanel.xml` & `collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/profiles/default/registry.xml` & `collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/testing.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/testing.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/tests/data/account.json` & `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/account.json`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/tests/data/interests.json` & `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/interests.json`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/tests/data/lists.json` & `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/lists.json`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/tests/data/lists_interest_categories.json` & `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/lists_interest_categories.json`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/tests/data/member.json` & `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/member.json`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_controlpanel.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_exceptions.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_locator.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_locator.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_mock_requests.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_mock_requests.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_newsletter.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_newsletter.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_portlet.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_portlet.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/tests/test_setup.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/upgrades.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/upgrades.zcml` & `collective.mailchimp-3.1.1/src/collective/mailchimp/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective/mailchimp/vocabularies.py` & `collective.mailchimp-3.1.1/src/collective/mailchimp/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.0/src/collective.mailchimp.egg-info/SOURCES.txt` & `collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -36,25 +36,19 @@
 src/collective/mailchimp/browser/newsletter.py
 src/collective/mailchimp/browser/portlet.pt
 src/collective/mailchimp/browser/portlet.py
 src/collective/mailchimp/browser/z3cformhelpers.py
 src/collective/mailchimp/browser/images/mailchimp.gif
 src/collective/mailchimp/browser/stylesheets/mailchimp.css
 src/collective/mailchimp/locales/collective.mailchimp.pot
-src/collective/mailchimp/locales/de/LC_MESSAGES/collective.mailchimp.mo
 src/collective/mailchimp/locales/de/LC_MESSAGES/collective.mailchimp.po
-src/collective/mailchimp/locales/fr/LC_MESSAGES/collective.mailchimp.mo
 src/collective/mailchimp/locales/fr/LC_MESSAGES/collective.mailchimp.po
-src/collective/mailchimp/locales/it/LC_MESSAGES/collective.mailchimp.mo
 src/collective/mailchimp/locales/it/LC_MESSAGES/collective.mailchimp.po
-src/collective/mailchimp/locales/nl/LC_MESSAGES/collective.mailchimp.mo
 src/collective/mailchimp/locales/nl/LC_MESSAGES/collective.mailchimp.po
-src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/collective.mailchimp.mo
 src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/collective.mailchimp.po
-src/collective/mailchimp/locales/ro/LC_MESSAGES/collective.mailchimp.mo
 src/collective/mailchimp/locales/ro/LC_MESSAGES/collective.mailchimp.po
 src/collective/mailchimp/profiles/default/browserlayer.xml
 src/collective/mailchimp/profiles/default/controlpanel.xml
 src/collective/mailchimp/profiles/default/cssregistry.xml
 src/collective/mailchimp/profiles/default/metadata.xml
 src/collective/mailchimp/profiles/default/portlets.xml
 src/collective/mailchimp/profiles/default/registry.xml
```

