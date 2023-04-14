# Comparing `tmp/collective.mailchimp-3.1.1.tar.gz` & `tmp/collective.mailchimp-4.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.mailchimp-3.1.1.tar", last modified: Fri Apr 14 09:09:56 2023, max compression
+gzip compressed data, was "collective.mailchimp-4.0.0a1.tar", last modified: Fri Apr 14 09:33:21 2023, max compression
```

## Comparing `collective.mailchimp-3.1.1.tar` & `collective.mailchimp-4.0.0a1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.523363 collective.mailchimp-3.1.1/
--rw-r--r--   0 maurits    (501) staff       (20)     5765 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)      169 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/CONTRIBUTORS.rst
--rw-r--r--   0 maurits    (501) staff       (20)      133 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    13040 2023-04-14 09:09:56.523481 collective.mailchimp-3.1.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     5916 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)       37 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/TODO.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.505353 collective.mailchimp-3.1.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1513 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      737 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)      138 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/requirements.txt
--rw-r--r--   0 maurits    (501) staff       (20)      297 2023-04-14 09:09:56.523965 collective.mailchimp-3.1.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2180 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.498453 collective.mailchimp-3.1.1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.505730 collective.mailchimp-3.1.1/src/collective/
--rw-r--r--   0 maurits    (501) staff       (20)      269 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.510357 collective.mailchimp-3.1.1/src/collective/mailchimp/
--rw-r--r--   0 maurits    (501) staff       (20)      115 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.513560 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1494 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5789 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2618 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     1409 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/extender.py
--rw-r--r--   0 maurits    (501) staff       (20)      381 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/extender.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.513811 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/images/
--rw-r--r--   0 maurits    (501) staff       (20)      998 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/images/mailchimp.gif
--rw-r--r--   0 maurits    (501) staff       (20)    11188 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/newsletter.py
--rw-r--r--   0 maurits    (501) staff       (20)      596 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/portlet.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3299 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/portlet.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.514134 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/stylesheets/
--rw-r--r--   0 maurits    (501) staff       (20)      170 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/stylesheets/mailchimp.css
--rw-r--r--   0 maurits    (501) staff       (20)     3371 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/browser/z3cformhelpers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1702 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1765 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/exceptions.py
--rw-r--r--   0 maurits    (501) staff       (20)     7898 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.514455 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/
--rw-r--r--   0 maurits    (501) staff       (20)     9642 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/collective.mailchimp.pot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.499834 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/de/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.514713 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/de/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    10455 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/de/LC_MESSAGES/collective.mailchimp.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.500090 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/fr/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.514967 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/fr/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    11768 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/fr/LC_MESSAGES/collective.mailchimp.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.500348 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/it/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.515222 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/it/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    11997 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/it/LC_MESSAGES/collective.mailchimp.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.500721 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/nl/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.515605 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/nl/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    12577 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/nl/LC_MESSAGES/collective.mailchimp.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.501021 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/pt_BR/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.515905 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    12196 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/collective.mailchimp.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.501320 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/ro/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.516174 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/ro/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    10354 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locales/ro/LC_MESSAGES/collective.mailchimp.po
--rw-r--r--   0 maurits    (501) staff       (20)    13365 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/locator.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.501769 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.517825 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      135 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      625 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      177 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/cssregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      165 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      172 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/portlets.xml
--rw-r--r--   0 maurits    (501) staff       (20)      724 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/registry.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.518832 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)       85 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      295 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      380 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/uninstall/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     5212 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.521279 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.523153 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/
--rw-r--r--   0 maurits    (501) staff       (20)     2780 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/account.json
--rw-r--r--   0 maurits    (501) staff       (20)     8457 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/interests.json
--rw-r--r--   0 maurits    (501) staff       (20)     6458 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/lists.json
--rw-r--r--   0 maurits    (501) staff       (20)     2787 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/lists_interest_categories.json
--rw-r--r--   0 maurits    (501) staff       (20)     3262 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/member.json
--rw-r--r--   0 maurits    (501) staff       (20)     2586 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     1566 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_exceptions.py
--rw-r--r--   0 maurits    (501) staff       (20)     4015 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_locator.py
--rw-r--r--   0 maurits    (501) staff       (20)     2410 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_mock_requests.py
--rw-r--r--   0 maurits    (501) staff       (20)     5905 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_newsletter.py
--rw-r--r--   0 maurits    (501) staff       (20)     7115 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_portlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     3637 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     1162 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     1150 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/upgrades.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1806 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective/mailchimp/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:09:56.507869 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    13040 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3156 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      135 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-04-14 09:09:56.000000 collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.086766 collective.mailchimp-4.0.0a1/
+-rw-r--r--   0 maurits    (501) staff       (20)     7097 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      169 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/CONTRIBUTORS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      133 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    14220 2023-04-14 09:33:21.086899 collective.mailchimp-4.0.0a1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     5861 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       37 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/TODO.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.067863 collective.mailchimp-4.0.0a1/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1513 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      737 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      152 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/requirements.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      297 2023-04-14 09:33:21.087374 collective.mailchimp-4.0.0a1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2151 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.060561 collective.mailchimp-4.0.0a1/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.068589 collective.mailchimp-4.0.0a1/src/collective/
+-rw-r--r--   0 maurits    (501) staff       (20)      269 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.074046 collective.mailchimp-4.0.0a1/src/collective/mailchimp/
+-rw-r--r--   0 maurits    (501) staff       (20)      115 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.077167 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1786 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1471 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/controlpanel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2843 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5420 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/data.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1409 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/extender.py
+-rw-r--r--   0 maurits    (501) staff       (20)      381 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/extender.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.077481 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/images/
+-rw-r--r--   0 maurits    (501) staff       (20)      998 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/images/mailchimp.gif
+-rw-r--r--   0 maurits    (501) staff       (20)    11353 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/newsletter.py
+-rw-r--r--   0 maurits    (501) staff       (20)      533 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/portlet.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2980 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/portlet.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.077794 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/stylesheets/
+-rw-r--r--   0 maurits    (501) staff       (20)      170 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/stylesheets/mailchimp.css
+-rw-r--r--   0 maurits    (501) staff       (20)     1702 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1765 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/exceptions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8292 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.078114 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/
+-rw-r--r--   0 maurits    (501) staff       (20)     9642 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/collective.mailchimp.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.061834 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/de/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.078456 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/de/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    10455 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/de/LC_MESSAGES/collective.mailchimp.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.062179 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/fr/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.078794 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    11768 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/fr/LC_MESSAGES/collective.mailchimp.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.062518 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/it/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.079128 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/it/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    11997 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/it/LC_MESSAGES/collective.mailchimp.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.062850 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.079440 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    12577 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/nl/LC_MESSAGES/collective.mailchimp.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.063187 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/pt_BR/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.079777 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    12196 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/collective.mailchimp.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.063522 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/ro/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.080123 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/ro/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    10354 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/ro/LC_MESSAGES/collective.mailchimp.po
+-rw-r--r--   0 maurits    (501) staff       (20)    14427 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/locator.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.064042 collective.mailchimp-4.0.0a1/src/collective/mailchimp/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.081661 collective.mailchimp-4.0.0a1/src/collective/mailchimp/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      135 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      625 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      165 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      172 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/profiles/default/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1113 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/profiles/default/registry.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.082855 collective.mailchimp-4.0.0a1/src/collective/mailchimp/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      295 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      190 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/profiles/uninstall/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      530 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/profiles/uninstall/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     5295 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.085083 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.086555 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/data/
+-rw-r--r--   0 maurits    (501) staff       (20)     2780 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/data/account.json
+-rw-r--r--   0 maurits    (501) staff       (20)     8457 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/data/interests.json
+-rw-r--r--   0 maurits    (501) staff       (20)     6458 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/data/lists.json
+-rw-r--r--   0 maurits    (501) staff       (20)     2787 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/data/lists_interest_categories.json
+-rw-r--r--   0 maurits    (501) staff       (20)     3262 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/data/member.json
+-rw-r--r--   0 maurits    (501) staff       (20)     2586 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1566 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_exceptions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4057 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_locator.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2410 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_mock_requests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5906 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_newsletter.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7115 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_portlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3704 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1747 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1620 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/upgrades.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1806 2023-04-14 09:33:20.000000 collective.mailchimp-4.0.0a1/src/collective/mailchimp/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-14 09:33:21.071166 collective.mailchimp-4.0.0a1/src/collective.mailchimp.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    14220 2023-04-14 09:33:21.000000 collective.mailchimp-4.0.0a1/src/collective.mailchimp.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3145 2023-04-14 09:33:21.000000 collective.mailchimp-4.0.0a1/src/collective.mailchimp.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-14 09:33:21.000000 collective.mailchimp-4.0.0a1/src/collective.mailchimp.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-14 09:33:21.000000 collective.mailchimp-4.0.0a1/src/collective.mailchimp.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-04-14 09:33:21.000000 collective.mailchimp-4.0.0a1/src/collective.mailchimp.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-14 09:33:21.000000 collective.mailchimp-4.0.0a1/src/collective.mailchimp.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      135 2023-04-14 09:33:21.000000 collective.mailchimp-4.0.0a1/src/collective.mailchimp.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-04-14 09:33:21.000000 collective.mailchimp-4.0.0a1/src/collective.mailchimp.egg-info/top_level.txt
```

### Comparing `collective.mailchimp-3.1.1/CHANGES.rst` & `collective.mailchimp-4.0.0a1/CHANGES.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,49 @@
 Changelog
 =========
 
-3.1.1 (2023-04-14)
-------------------
+4.0.0a1 (2023-04-14)
+--------------------
+
+Breaking changes:
+
+- Dropped support for Plone 5.1 and older.  [maurits]
+
+- Dropped support for Python 2.  [maurits]
+
+New features:
+
+- Split the controlpanel into two separate pages: settings and data.
+  Until now, if the settings resulted in an error while fetching the data from mailchimp,
+  you could not fix this because the whole control panel would fail to load.
+  Fixes `issue 26 <https://github.com/collective/collective.mailchimp/issues/26>`_.
+  [maurits]
+
+- Updated tests and infrastructure for Plone 5.2, Python 3.
+  Plone 6 should work, but it not tested yet.
+  [maurits]
+
+Bug fixes:
+
+- Reinitialize the locator when called on a different Plone Site.
+  Fixes `issue 31 <https://github.com/collective/collective.mailchimp/issues/31>`_.
+  [maurits]
+
+- Register resource bundle so our css is loaded on Plone 5.2 and higher.  [maurits]
+
+- Increase limit to 50 (by default) when retrieving lists from mailchimp.
+  The API default was getting only 10 lists, which is really too few (and can
+  prevent you from selecting the correct default list for example).
+  The limit is a setting that can be changed on a per-site basis.
+  [laulaz]
+
+- Update portlet template and fix portlet code for Plone 5.2/6. [fredvd]
+
+- Fix posting of interests to the mailchimp API, interest_groups were transformed to bytes string.
+  [fredvd]
 
 - Fix controlpanel field validation for Plone 6
   [agitator]
 
 
 3.1.0 (2020-01-13)
 ------------------
```

### Comparing `collective.mailchimp-3.1.1/PKG-INFO` & `collective.mailchimp-4.0.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 Metadata-Version: 2.1
 Name: collective.mailchimp
-Version: 3.1.1
+Version: 4.0.0a1
 Summary: MailChimp integration for Plone.
-Home-page: https://pypi.python.org/pypi/collective.mailchimp
+Home-page: https://pypi.org/project/collective.mailchimp/
 Author: kitconcept GmbH (Timo Stollenwerk)
 Author-email: stollenwerk@kitconcept.com
 License: GPL version 2
 Keywords: Python Plone MailChimp Mail Newsletter
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 4.0
-Classifier: Framework :: Plone :: 4.1
-Classifier: Framework :: Plone :: 4.2
-Classifier: Framework :: Plone :: 4.3
-Classifier: Framework :: Plone :: 5.0
-Classifier: Framework :: Plone :: 5.1
+Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Plone
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
+Requires-Python: >=3.6
 Provides-Extra: test
 
-.. image:: https://secure.travis-ci.org/collective/collective.mailchimp.png
-    :target: http://travis-ci.org/collective/collective.mailchimp
-
 .. image:: https://img.shields.io/coveralls/collective/collective.mailchimp/master.svg
     :target: https://coveralls.io/r/collective/collective.mailchimp
 
 .. image:: https://landscape.io/github/collective/collective.mailchimp/master/landscape.svg
    :target: https://landscape.io/github/collective/collective.mailchimp/master
    :alt: Code Health
 
@@ -56,15 +51,16 @@
 Introduction
 ============
 
 .. image:: https://raw.githubusercontent.com/collective/collective.mailchimp/master/kitconcept.png
    :alt: kitconcept
    :target: https://kitconcept.com/
 
-MailChimp integration for Plone 4 and 5.
+MailChimp integration for Plone 5.2 and 6.0 on Python 3.
+Use ``collective.mailchimp`` 3.x for earlier Plone and Python versions.
 
 MailChimp helps you design email newsletters, share them on social networks, integrate with services you already use, and track your results.
 
 collective.mailchimp provides a @newsletter view to let visitors subscribe to one or more MailChimp mailing lists. It also provides a MailChimp portlet in case you want to display your newsletter subscription as part of an existing site.
 
 The newsletter subscriptions forms in both the view and the portlet are extendable, so you can add custom fields that can be stored in your MailChimp subscriber list.
 
@@ -194,16 +190,53 @@
 - Jean-Michel Francois
 - Carsten Senger
 - Peter Holzer
 
 Changelog
 =========
 
-3.1.1 (2023-04-14)
-------------------
+4.0.0a1 (2023-04-14)
+--------------------
+
+Breaking changes:
+
+- Dropped support for Plone 5.1 and older.  [maurits]
+
+- Dropped support for Python 2.  [maurits]
+
+New features:
+
+- Split the controlpanel into two separate pages: settings and data.
+  Until now, if the settings resulted in an error while fetching the data from mailchimp,
+  you could not fix this because the whole control panel would fail to load.
+  Fixes `issue 26 <https://github.com/collective/collective.mailchimp/issues/26>`_.
+  [maurits]
+
+- Updated tests and infrastructure for Plone 5.2, Python 3.
+  Plone 6 should work, but it not tested yet.
+  [maurits]
+
+Bug fixes:
+
+- Reinitialize the locator when called on a different Plone Site.
+  Fixes `issue 31 <https://github.com/collective/collective.mailchimp/issues/31>`_.
+  [maurits]
+
+- Register resource bundle so our css is loaded on Plone 5.2 and higher.  [maurits]
+
+- Increase limit to 50 (by default) when retrieving lists from mailchimp.
+  The API default was getting only 10 lists, which is really too few (and can
+  prevent you from selecting the correct default list for example).
+  The limit is a setting that can be changed on a per-site basis.
+  [laulaz]
+
+- Update portlet template and fix portlet code for Plone 5.2/6. [fredvd]
+
+- Fix posting of interests to the mailchimp API, interest_groups were transformed to bytes string.
+  [fredvd]
 
 - Fix controlpanel field validation for Plone 6
   [agitator]
 
 
 3.1.0 (2020-01-13)
 ------------------
```

### Comparing `collective.mailchimp-3.1.1/README.rst` & `collective.mailchimp-4.0.0a1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-.. image:: https://secure.travis-ci.org/collective/collective.mailchimp.png
-    :target: http://travis-ci.org/collective/collective.mailchimp
-
 .. image:: https://img.shields.io/coveralls/collective/collective.mailchimp/master.svg
     :target: https://coveralls.io/r/collective/collective.mailchimp
 
 .. image:: https://landscape.io/github/collective/collective.mailchimp/master/landscape.svg
    :target: https://landscape.io/github/collective/collective.mailchimp/master
    :alt: Code Health
 
@@ -27,15 +24,16 @@
 Introduction
 ============
 
 .. image:: https://raw.githubusercontent.com/collective/collective.mailchimp/master/kitconcept.png
    :alt: kitconcept
    :target: https://kitconcept.com/
 
-MailChimp integration for Plone 4 and 5.
+MailChimp integration for Plone 5.2 and 6.0 on Python 3.
+Use ``collective.mailchimp`` 3.x for earlier Plone and Python versions.
 
 MailChimp helps you design email newsletters, share them on social networks, integrate with services you already use, and track your results.
 
 collective.mailchimp provides a @newsletter view to let visitors subscribe to one or more MailChimp mailing lists. It also provides a MailChimp portlet in case you want to display your newsletter subscription as part of an existing site.
 
 The newsletter subscriptions forms in both the view and the portlet are extendable, so you can add custom fields that can be stored in your MailChimp subscriber list.
```

### Comparing `collective.mailchimp-3.1.1/docs/INSTALL.txt` & `collective.mailchimp-4.0.0a1/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/docs/LICENSE.GPL` & `collective.mailchimp-4.0.0a1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/docs/LICENSE.txt` & `collective.mailchimp-4.0.0a1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/setup.py` & `collective.mailchimp-4.0.0a1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,48 +16,47 @@
     + open('CHANGES.rst').read()
     + '\n'
 )
 
 
 setup(
     name='collective.mailchimp',
-    version='3.1.1',
+    version='4.0.0a1',
     description="MailChimp integration for Plone.",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
-        "Framework :: Plone :: 4.0",
-        "Framework :: Plone :: 4.1",
-        "Framework :: Plone :: 4.2",
-        "Framework :: Plone :: 4.3",
-        "Framework :: Plone :: 5.0",
-        "Framework :: Plone :: 5.1",
+        "Framework :: Plone :: Addon",
         "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.6",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Framework :: Plone",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords='Python Plone MailChimp Mail Newsletter',
     author='kitconcept GmbH (Timo Stollenwerk)',
     author_email='stollenwerk@kitconcept.com',
-    url='https://pypi.python.org/pypi/collective.mailchimp',
+    url='https://pypi.org/project/collective.mailchimp/',
     license='GPL version 2',
     packages=find_packages('src', exclude=['ez_setup']),
     namespace_packages=['collective'],
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
-    python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*',
+    # Python 3.6 is EOL, but I don't want to break it needlessly.
+    python_requires=">=3.6",
     install_requires=[
         'setuptools',
         'Products.CMFPlone',
         'plone.app.portlets',
         'plone.app.registry',
         'plone.app.upgrade',
         'requests',
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/configure.zcml` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/configure.zcml`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,21 @@
   <include package="plone.app.registry" />
   <browser:page
     name="mailchimp-settings"
     for="Products.CMFPlone.interfaces.IPloneSiteRoot"
     class=".controlpanel.MailchimpSettingsControlPanel"
     permission="cmf.ManagePortal"
     />
+  <browser:page
+    name="mailchimp-data"
+    for="Products.CMFPlone.interfaces.IPloneSiteRoot"
+    class=".controlpanel.MailchimpData"
+    template="data.pt"
+    permission="cmf.ManagePortal"
+    />
 
   <!-- Portlet -->
   <include package="plone.app.portlets" />
   <plone:portlet
     name="portlet.MailChimp"
     interface=".portlet.IMailChimpPortlet"
     assignment=".portlet.Assignment"
@@ -39,20 +46,22 @@
     />
 
   <!-- Newsletter -->
   <browser:page
     name="newsletter"
     for="*"
     class=".newsletter.NewsletterView"
+    layer="..interfaces.ICollectiveMailchimp"
     permission="zope2.View"
     />
 
   <browser:page
     name="unsubscribe-newsletter"
     for="*"
     class=".newsletter.UnsubscribeNewsletterView"
+    layer="..interfaces.ICollectiveMailchimp"
     permission="zope2.View"
     />
 
   <!-- <include file="extender.zcml" /> -->
 
 </configure>
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/controlpanel.pt` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/data.pt`

 * *Files 5% similar despite different names*

```diff
@@ -13,33 +13,32 @@
 
     <div metal:use-macro="context/global_statusmessage/macros/portal_message">
       Portal status message
     </div>
 
     <a href=""
        id="setup-link"
-       tal:attributes="href string:$portal_url/plone_control_panel"
+       tal:attributes="href string:$portal_url/@@overview-controlpanel"
        i18n:translate="">
         Site Setup
     </a> &rsaquo;
 
     <h1 class="documentFirstHeading" tal:content="view/label">View Title</h1>
+    <p><a href=""
+      tal:attributes="href string:$portal_url/@@mailchimp-settings"
+      i18n:translate="">View MailChimp settings</a></p>
 
     <div id="layout-contents"
          class="enableUnloadProtection enableAutoFocus enableFormTabbing enableUnlockProtection"
          tal:define="account view/mailchimp_account|nothing;
                      empty string:-">
-      <fieldset id="fieldset-send">
-        <legend id="fieldsetlegend-send" i18n:translate="">Standard</legend>
-        <div id="mailchimp-no-valid-account" class="warning" tal:condition="not:account"
-             i18n:translate="msg_mailchimp_no_account">
-          Your account has not been saved yet or is not valid.
-        </div>
-        <span tal:replace="structure view/contents" />
-      </fieldset>
+      <div id="mailchimp-no-valid-account" class="warning" tal:condition="not:account"
+            i18n:translate="msg_mailchimp_no_account">
+        Your account has not been saved yet or is not valid.
+      </div>
       <fieldset id="fieldset-account" tal:condition="account">
         <legend id="fieldsetlegend-account" i18n:translate="">MailChimp Account</legend>
         Account
         <table class="listing">
           <thead>
             <tr>
               <th i18n:translate="">Key</th>
@@ -128,19 +127,10 @@
             </tr>
           </tbody>
         </table>
 
       </fieldset>
     </div>
 
-    <script type="text/javascript">
-// Disable inline validation.  It may change the cache based on a new
-// api key that the user has not yet saved.
-// Plone 4:
-$('.z3cformInlineValidation').removeClass('z3cformInlineValidation');
-// Plone 5
-$('.pat-inlinevalidation').removeClass('pat-inlinevalidation');
-    </script>
-
   </div>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 Portal status message
 Site Setup ›
 ****** View Title ******
- Standard
+View MailChimp settings
 Your account has not been saved yet or is not valid.
-   MailChimp Account Account
+ MailChimp Account Account
 Key         Value
 Username:
 Last login:
 Company:
 Address 1:
 Address 2:
 Zip:
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/controlpanel.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/controlpanel.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ..exceptions import MailChimpException
 from ..exceptions import PostRequestError
 from collective.mailchimp import _
 from collective.mailchimp.interfaces import IMailchimpLocator
 from collective.mailchimp.interfaces import IMailchimpSettings
 from plone.app.registry.browser import controlpanel
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
+from Products.Five.browser import BrowserView
 from z3c.form.interfaces import WidgetActionExecutionError
 from zope.component import getUtility
 from zope.interface import alsoProvides
 from zope.interface import Invalid
 
 
 try:
@@ -32,22 +33,28 @@
     def updateFields(self):
         super(MailchimpSettingsEditForm, self).updateFields()
 
     def updateWidgets(self):
         super(MailchimpSettingsEditForm, self).updateWidgets()
 
     def updateCache(self):
+        if IDisableCSRFProtection is not None:
+            alsoProvides(self.request, IDisableCSRFProtection)
         mailchimp = getUtility(IMailchimpLocator)
         mailchimp.updateCache()
 
 
 class MailchimpSettingsControlPanel(controlpanel.ControlPanelFormWrapper):
     form = MailchimpSettingsEditForm
     index = ViewPageTemplateFile('controlpanel.pt')
 
+
+class MailchimpData(BrowserView):
+    label = _(u"MailChimp data")
+
     def mailchimp_account(self):
         if IDisableCSRFProtection is not None:
             alsoProvides(self.request, IDisableCSRFProtection)
         mailchimp = getUtility(IMailchimpLocator)
         try:
             return mailchimp.account()
         except PostRequestError:
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/extender.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/extender.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/images/mailchimp.gif` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/images/mailchimp.gif`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/newsletter.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/newsletter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
-from Products.CMFCore.utils import getToolByName
 from collective.mailchimp import _
 from collective.mailchimp.exceptions import MailChimpException
 from collective.mailchimp.interfaces import IMailchimpLocator
 from collective.mailchimp.interfaces import IMailchimpSettings
 from collective.mailchimp.interfaces import INewsletterSubscribe
 from collective.mailchimp.interfaces import INewsletterUnsubscribe
 from plone.app.layout.navigation.root import getNavigationRootObject
 from plone.registry.interfaces import IRegistry
 from plone.z3cform.fieldsets import extensible
 from plone.z3cform.layout import wrap_form
+from Products.CMFCore.utils import getToolByName
+from Products.CMFPlone.utils import safe_text
 from Products.statusmessages.interfaces import IStatusMessage
 from z3c.form import button
 from z3c.form import field
 from z3c.form import form
 from z3c.form.browser.checkbox import CheckBoxFieldWidget
 from z3c.form.browser.radio import RadioFieldWidget
 from z3c.form.interfaces import ActionExecutionError
@@ -46,15 +47,19 @@
         self.fields['interest_groups'].widgetFactory = CheckBoxFieldWidget
         self.fields['email_type'].widgetFactory = RadioFieldWidget
 
     def updateWidgets(self):
         super(NewsletterSubscriberForm, self).updateWidgets()
         widgets = self.widgets
         registry = getUtility(IRegistry)
-        self.mailchimp_settings = registry.forInterface(IMailchimpSettings)
+        try:
+            self.mailchimp_settings = registry.forInterface(IMailchimpSettings)
+        except KeyError:
+            self.mailchimp_settings = None
+            return
         self.mailchimp = getUtility(IMailchimpLocator)
 
         # Show/hide mail format option widget
         if not self.mailchimp_settings.email_type_is_optional:
             widgets['email_type'].mode = HIDDEN_MODE
 
         # Retrieve the list id either from the request/form or fall back to
@@ -95,16 +100,15 @@
 
         # interest groups
         interests = {}
         interest_groups = data.pop('interest_groups', [])
         if self.available_interest_groups and interest_groups:
             # Create dictionary with as keys the interest groups, and as
             # values always True.
-            interests = dict.fromkeys(interest_groups, True)
-
+            interests = dict.fromkeys(map(safe_text, interest_groups), True)
         # Use email_type if one is provided by the form, if not choose the
         # default email type from the control panel settings.
         email_type = data.get('email_type') or self.mailchimp_settings.email_type
 
         # Subscribe to MailChimp list
         try:
             self.mailchimp.subscribe(
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/browser/portlet.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/browser/portlet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
-from .z3cformhelpers import AddForm
-from .z3cformhelpers import EditForm
 from Acquisition import aq_inner
 from collective.mailchimp.browser.newsletter import NewsletterSubscriberForm
 from collective.mailchimp.interfaces import INewsletterSubscribe
 from plone.app.portlets.portlets import base
+from plone.autoform.directives import widget
 from plone.memoize.compress import xhtml_compress
 from plone.memoize.instance import memoize
 from plone.portlets.interfaces import IPortletDataProvider
 from plone.z3cform import z2
 from plone.z3cform.interfaces import IWrappedForm
 from Products.CMFCore.utils import getToolByName
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
@@ -26,14 +25,15 @@
 
 class IMailChimpPortlet(IPortletDataProvider):
 
     name = schema.TextLine(
         title=_(u'Title'), description=_(u'Title of the portlet')
     )
 
+    widget(available_lists=CheckBoxFieldWidget)
     available_lists = schema.List(
         title=_(u'Available lists'),
         description=_(u'Select available lists to subscribe to.'),
         required=True,
         min_length=1,
         value_type=schema.Choice(
             source='collective.mailchimp.vocabularies.AvailableLists'
@@ -64,44 +64,37 @@
     def render(self):
         return xhtml_compress(self._template())
 
     @property
     def name(self):
         return self.data.name or _(u"Subscribe to newsletter")
 
-    @memoize
-    def _data(self):
-        catalog = getToolByName(self.context, 'portal_catalog')
-        return catalog(portal_type='MailChimp Item')
 
     def update(self):
         super(Renderer, self).update()
-        z2.switch_on(self, request_layer=IFormLayer)
-        self.form = self.form(aq_inner(self.context), self.request)
+        self.form = NewsletterSubscriberForm(aq_inner(self.context), self.request)
         alsoProvides(self.form, IWrappedForm)
         self.form.update()
 
 
-class AddForm(AddForm):
-    fields = field.Fields(IMailChimpPortlet)
-    fields['available_lists'].widgetFactory = CheckBoxFieldWidget
+class AddForm(base.AddForm):
+    schema = IMailChimpPortlet
     label = _(u"Add MailChimp Portlet")
     description = _(
         u"This portlet displays a subscription form for a "
         + u"MailChimp newsletter."
     )
 
     def create(self, data):
         return Assignment(
             name=data.get('name', u''),
             available_lists=data.get('available_lists', []),
         )
 
 
-class EditForm(EditForm):
-    fields = field.Fields(IMailChimpPortlet)
-    fields['available_lists'].widgetFactory = CheckBoxFieldWidget
+class EditForm(base.EditForm):
+    schema = IMailChimpPortlet
     label = _(u"Edit MailChimp Portlet")
     description = _(
         u"This portlet displays a subscription form for a "
         + u"MailChimp newsletter."
     )
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/configure.zcml` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/exceptions.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/exceptions.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/interfaces.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,27 @@
             default=u"Default list which is used in the @@newsletter view if "
             u"no list_id param is provided.",
         ),
         vocabulary="collective.mailchimp.vocabularies.AvailableLists",
         required=False,
     )
 
+    max_lists_number = schema.Int(
+        title=_(u"max_lists_number", default=u"Maximum lists number"),
+        description=_(
+            u"help_max_lists_number",
+            default=u"Maximum number of lists you want to retrieve from "
+            u"MailChimp API (maximum supported is 1000).",
+        ),
+        default=50,
+        min=1,
+        max=1000,
+        required=True,
+    )
+
     double_optin = schema.Bool(
         title=_(u"double_optin", default=u"Double opt-in"),
         description=_(
             u"help_double_optin",
             default=u"Flag to control whether a double opt-in confirmation "
             u"message is sent, defaults to true. Abusing this may "
             u"cause your account to be suspended.",
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/collective.mailchimp.pot` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/collective.mailchimp.pot`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/de/LC_MESSAGES/collective.mailchimp.po` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/de/LC_MESSAGES/collective.mailchimp.po`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/fr/LC_MESSAGES/collective.mailchimp.po` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/fr/LC_MESSAGES/collective.mailchimp.po`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/it/LC_MESSAGES/collective.mailchimp.po` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/it/LC_MESSAGES/collective.mailchimp.po`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/nl/LC_MESSAGES/collective.mailchimp.po` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/nl/LC_MESSAGES/collective.mailchimp.po`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/collective.mailchimp.po` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/collective.mailchimp.po`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/locales/ro/LC_MESSAGES/collective.mailchimp.po` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/locales/ro/LC_MESSAGES/collective.mailchimp.po`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/locator.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/locator.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 from .exceptions import MailChimpException
 from .exceptions import PostRequestError
 from .exceptions import SerializationError
 from collective.mailchimp.interfaces import IMailchimpLocator
 from collective.mailchimp.interfaces import IMailchimpSettings
 from plone.registry.interfaces import IRegistry
 from zope.component import getUtility
+from zope.component.hooks import getSite
 from zope.interface import implementer
 
 import hashlib
 import json
 import logging
 import requests
 import six.moves
 
 
 try:
     import urlparse
+    from urllib import urlencode
 except ImportError:
     from urllib import parse as urlparse
+    from urllib.parse import urlencode
 
 _marker = object()
 logger = logging.getLogger('collective.mailchimp')
 
 
 @implementer(IMailchimpLocator)
 class MailchimpLocator(object):
@@ -31,27 +34,44 @@
     """
 
     key_account = "collective.mailchimp.cache.account"
     key_groups = "collective.mailchimp.cache.groups"
     key_lists = "collective.mailchimp.cache.lists"
 
     def __init__(self, settings={}):
-        """ Use settings if provided """
+        """ Use settings if provided
+
+        Note that the __init__ method is only called once at startup.
+        settings can only be passed when you directly instantiate a
+        MailchimpLocator, for example in tests.
+        """
         self.registry = None
         self.settings = None
         self.api_root = None
         if settings:
             self.settings = settings
+        self.site_path = ""
 
     def initialize(self):
         """ Load settings from registry and construct api root"""
+        site_path = "/".join(getSite().getPhysicalPath())
+        if self.site_path != site_path:
+            # Settings are for a different Plone Site.
+            # See https://github.com/collective/collective.mailchimp/issues/31
+            self.site_path = site_path
+            self.registry = None
+            self.settings = None
+            self.api_root = None
         if self.registry is None:
             self.registry = getUtility(IRegistry)
         if self.settings is None:
-            self.settings = self.registry.forInterface(IMailchimpSettings)
+            try:
+                self.settings = self.registry.forInterface(IMailchimpSettings)
+            except KeyError:
+                return
         self.apikey = self.settings.api_key
         if not self.apikey:
             return
         parts = self.apikey.split('-')
         if not len(parts) > 1:
             # bad api key, allow to fix
             return
@@ -97,21 +117,23 @@
         elif 'status' in response and 'detail' in response:
             exc = MailChimpException(
                 response['status'], response['detail'], response.get('errors')
             )
             logger.warn(exc)
             raise exc
 
-    def api_request(self, endpoint='', request_type='get', **kwargs):
+    def api_request(self, endpoint='', request_type='get', query_params={}, **kwargs):
         """ construct the request and do a get/post.
         """
         if not self.api_root:
             return []
         headers = {'content-type': 'application/json'}
         url = urlparse.urljoin(self.api_root, endpoint)
+        if query_params:
+            url = "{}?{}".format(url, urlencode(query_params))
 
         # we provide a json structure with the parameters.
         payload = json.dumps(kwargs)
 
         assert request_type in ['get', 'post', 'put', 'delete', 'patch']
         request_method = getattr(requests, request_type)
 
@@ -135,17 +157,18 @@
         cache = self.registry.get(self.key_lists, _marker)
         if cache and cache is not _marker:
             return cache
         return self._lists()
 
     def _lists(self):
         """ The actual API call for lists. """
+        count = self.settings.max_lists_number
         try:
             # lists returns a dict with 'total' and 'data'. we just need data
-            response = self.api_request('lists')
+            response = self.api_request('lists', query_params={"count": count})
         except PostRequestError:
             return []
         if 'lists' in response:
             return response['lists']
         return []
 
     def default_list_id(self):
@@ -230,25 +253,27 @@
                 email_address=email_address,
                 email_type=email_type,
                 **kwargs
             )
         except MailChimpException:
             raise
         except Exception as e:
-            raise PostRequestError(e)
+           raise PostRequestError(e)
         logger.info(
             "Subscribed %s to list with id: %s." % (email_address, list_id)
         )
         logger.debug(
             "Subscribed %s to list with id: %s.\n\n %s"
             % (email_address, list_id, response)
         )
         return response
 
     def get_email_hash(self, email_address):
+        if isinstance(email_address, str):
+            email_address = email_address.encode("utf-8")
         return hashlib.md5(email_address).hexdigest()
 
     def update_subscriber(self, list_id, email_address, **kwargs):
         """API call to update a member's data"""
         self.initialize()
 
         email_hash = self.get_email_hash(email_address)
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/profiles/default/controlpanel.xml` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/testing.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,16 @@
         # Check url
         url = args[0]
         mailchimp_url = 'api.mailchimp.com/3.0/'
         if mailchimp_url not in url:
             raise MockRequestsException(
                 'Expected {0} in url {1}'.format(mailchimp_url, url)
             )
-        endpoint = url.split(mailchimp_url)[1]
+        # Remove mailchimp & query from url to get only the endpoint
+        endpoint = url.split(mailchimp_url)[1].split("?")[0]
         # Check auth
         auth = kwargs.get('auth')
         if not auth:
             raise MockRequestsException('Expected auth in keyword arguments.')
         expected_auth = ('apikey', DUMMY_API_KEY)
         if (
             not isinstance(auth, tuple)
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/account.json` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/data/account.json`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/interests.json` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/data/interests.json`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/lists.json` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/data/lists.json`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/lists_interest_categories.json` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/data/lists_interest_categories.json`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/data/member.json` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/data/member.json`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_controlpanel.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_exceptions.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_locator.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_locator.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,25 +81,26 @@
         locator.updateCache()
         account = locator.registry[locator.key_account]
         self.assertTrue(isinstance(account, dict))
         self.assertEqual(account[u'account_id'], u'8d3a3db4d97663a9074efcc16')
         self.assertEqual(account[u'account_name'], u"Freddie's Jokes")
         groups = locator.registry[locator.key_groups]
         self.assertTrue(isinstance(groups, dict))
+        group_keys = list(groups.keys())
         self.assertEqual(
-            groups.keys(), [u'f6257645gs', u'f6267645gs', u'57afe96172']
+            group_keys, ['f6257645gs', 'f6267645gs', '57afe96172']
         )
         self.assertEqual(
-            groups[groups.keys()[0]].keys(),
+            sorted(list(groups[group_keys[0]].keys())),
             [
-                u'total_items',
+                '_links',
+                'categories',
                 'interests',
-                u'_links',
-                u'categories',
-                u'list_id',
+                'list_id',
+                'total_items',
             ],
         )
 
         self.assertTrue(isinstance(locator.registry[locator.key_lists], tuple))
         self.assertEqual(len(locator.registry[locator.key_lists]), 3)
         # It does not complain when there is no api key
         locator.settings.api_key = None
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_mock_requests.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_mock_requests.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_newsletter.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_newsletter.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         self.browser.open("%s/unsubscribe-newsletter" % self.portal_url)
         self.browser.getControl(
             name="form.widgets.email"
         ).value = "freddy@freddiesjokes.com"
         unsub_all_checkbox = self.browser.getControl(
             name='form.widgets.unsubscribe:list', index=0
         )
-        unsub_all_checkbox.value = ['checked']
+        unsub_all_checkbox.value = ['selected']
         self.browser.getControl(name="form.buttons.unsubscribe").click()
 
         from collective.mailchimp.locator import requests
 
         self.assertEqual(
             requests.last_call,
             {
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_portlet.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_portlet.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/tests/test_setup.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/tests/test_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,52 +35,33 @@
 
     def test_browserlayer_available(self):
         from plone.browserlayer import utils
         from collective.mailchimp.interfaces import ICollectiveMailchimp
 
         self.failUnless(ICollectiveMailchimp in utils.registered_layers())
 
-    def test_mailchimp_css_available(self):
-        if not PLONE_5:
-            # Plone 4
-            cssreg = getToolByName(self.portal, "portal_css")
-            stylesheets_ids = cssreg.getResourceIds()
-            self.assertTrue(
-                '++resource++collective.mailchimp.stylesheets/mailchimp.css'
-                in stylesheets_ids
-            )
-        else:
-            # Plone 5
-            from zope.component import getUtility
-            from plone.registry.interfaces import IRegistry
-            from Products.CMFPlone.interfaces import IResourceRegistry
-
-            reg = getUtility(IRegistry)
-            resources = reg.collectionOfInterface(
-                IResourceRegistry, prefix="plone.resources", check=False
-            )
-            key = 'resource-collective-mailchimp-stylesheets'
-            self.assertIn(key, resources.keys())
-            self.assertEqual(
-                resources[key].css,
-                ['++resource++collective.mailchimp.stylesheets/mailchimp.css'],
-            )
+    def test_mailchimp_resource_bundle_available(self):
+        from zope.component import getUtility
+        from plone.registry.interfaces import IRegistry
+        from Products.CMFPlone.interfaces import IResourceRegistry
+
+        reg = getUtility(IRegistry)
+        resources = reg.collectionOfInterface(
+            IResourceRegistry, prefix="plone.bundles", check=False
+        )
+        key = 'collective.mailchimp'
+        self.assertIn(key, resources.keys())
 
     def test_mailchimp_css_enabled(self):
-        if not PLONE_5:
-            # Plone 4
-            cssreg = getToolByName(self.portal, "portal_css")
-            self.assertTrue(
-                cssreg.getResource(
-                    '++resource++collective.mailchimp.stylesheets/mailchimp.css'  # noqa
-                ).getEnabled()
-            )
-        else:
-            # Don't know how to test this in Plone 5.
-            pass
+        portal_url = self.portal.absolute_url()
+        css = "++resource++collective.mailchimp.stylesheets/mailchimp.css"
+        url = f"{portal_url}/{css}"
+        # render the homepage
+        html = self.portal()
+        self.assertIn(url, html)
 
 
 class TestUninstall(unittest.TestCase):
 
     layer = COLLECTIVE_MAILCHIMP_INTEGRATION_TESTING
 
     def setUp(self):
@@ -103,10 +84,30 @@
     def test_browserlayer_removed(self):
         """Test that ICollectiveMailchimp is removed."""
         from collective.mailchimp.interfaces import ICollectiveMailchimp
         from plone.browserlayer import utils
 
         self.assertNotIn(ICollectiveMailchimp, utils.registered_layers())
 
+    def test_mailchimp_resource_bundle_removed(self):
+        from zope.component import getUtility
+        from plone.registry.interfaces import IRegistry
+        from Products.CMFPlone.interfaces import IResourceRegistry
+
+        reg = getUtility(IRegistry)
+        resources = reg.collectionOfInterface(
+            IResourceRegistry, prefix="plone.bundles", check=False
+        )
+        key = 'collective.mailchimp'
+        self.assertNotIn(key, resources.keys())
+
+    def test_mailchimp_css_disabled(self):
+        portal_url = self.portal.absolute_url()
+        css = "++resource++collective.mailchimp.stylesheets/mailchimp.css"
+        url = f"{portal_url}/{css}"
+        # render the homepage
+        html = self.portal()
+        self.assertNotIn(url, html)
+
 
 def test_suite():
     return unittest.defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/upgrades.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/upgrades.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 def update_registry(context):
     registry = getUtility(IRegistry)
     registry.registerInterface(IMailchimpSettings)
 
 
 def install_mailchimp_stylesheet(context):
     csstool = getToolByName(context, 'portal_css', None)
+    if csstool is None:
+        return
     stylesheet_id = (
         '++resource++collective.mailchimp.stylesheets/mailchimp.css'
     )
     if stylesheet_id not in csstool.getResourceIds():
         csstool.manage_addStylesheet(
             id=stylesheet_id,
             rel='stylesheet',
@@ -32,7 +34,26 @@
 def install_mailchimp_cache(context):
     setup = getToolByName(context, 'portal_setup')
     setup.runImportStepFromProfile(PROFILE_ID, 'plone.app.registry')
 
 
 def reload_profile(context):
     loadMigrationProfile(context, 'profile-collective.mailchimp:default')
+
+
+def add_max_lists_number_setting(context):
+    registry = getUtility(IRegistry)
+    # we need to omit other fields because vocabularies (ex: available_lists)
+    # use our new (not existing) field and cause traceback
+    registry.registerInterface(
+        IMailchimpSettings,
+        omit=(
+            'api_key',
+            'default_list',
+            'double_optin',
+            'email_type',
+            'email_type_is_optional',
+            'replace_interests',
+            'send_welcome',
+            'update_existing',
+        ),
+    )
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/upgrades.zcml` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/upgrades.zcml`

 * *Files 14% similar despite different names*

```diff
@@ -34,8 +34,25 @@
       destination="2000"
       title="Re-install collective.mailchimp to load new src folder."
       description=""
       profile="collective.mailchimp:default"
       handler=".upgrades.reload_profile"
       />
 
+  <genericsetup:upgradeStep
+      source="2000"
+      destination="2001"
+      title="Add maximum lists number setting in registry"
+      description=""
+      profile="collective.mailchimp:default"
+      handler=".upgrades.add_max_lists_number_setting"
+      />
+
+  <genericsetup:upgradeDepends
+      source="2001"
+      destination="3000"
+      title="Register css resource"
+      profile="collective.mailchimp:default"
+      import_steps="plone.app.registry"
+      />
+
 </configure>
```

### Comparing `collective.mailchimp-3.1.1/src/collective/mailchimp/vocabularies.py` & `collective.mailchimp-4.0.0a1/src/collective/mailchimp/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/PKG-INFO` & `collective.mailchimp-4.0.0a1/src/collective.mailchimp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 Metadata-Version: 2.1
 Name: collective.mailchimp
-Version: 3.1.1
+Version: 4.0.0a1
 Summary: MailChimp integration for Plone.
-Home-page: https://pypi.python.org/pypi/collective.mailchimp
+Home-page: https://pypi.org/project/collective.mailchimp/
 Author: kitconcept GmbH (Timo Stollenwerk)
 Author-email: stollenwerk@kitconcept.com
 License: GPL version 2
 Keywords: Python Plone MailChimp Mail Newsletter
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 4.0
-Classifier: Framework :: Plone :: 4.1
-Classifier: Framework :: Plone :: 4.2
-Classifier: Framework :: Plone :: 4.3
-Classifier: Framework :: Plone :: 5.0
-Classifier: Framework :: Plone :: 5.1
+Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Plone
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
+Requires-Python: >=3.6
 Provides-Extra: test
 
-.. image:: https://secure.travis-ci.org/collective/collective.mailchimp.png
-    :target: http://travis-ci.org/collective/collective.mailchimp
-
 .. image:: https://img.shields.io/coveralls/collective/collective.mailchimp/master.svg
     :target: https://coveralls.io/r/collective/collective.mailchimp
 
 .. image:: https://landscape.io/github/collective/collective.mailchimp/master/landscape.svg
    :target: https://landscape.io/github/collective/collective.mailchimp/master
    :alt: Code Health
 
@@ -56,15 +51,16 @@
 Introduction
 ============
 
 .. image:: https://raw.githubusercontent.com/collective/collective.mailchimp/master/kitconcept.png
    :alt: kitconcept
    :target: https://kitconcept.com/
 
-MailChimp integration for Plone 4 and 5.
+MailChimp integration for Plone 5.2 and 6.0 on Python 3.
+Use ``collective.mailchimp`` 3.x for earlier Plone and Python versions.
 
 MailChimp helps you design email newsletters, share them on social networks, integrate with services you already use, and track your results.
 
 collective.mailchimp provides a @newsletter view to let visitors subscribe to one or more MailChimp mailing lists. It also provides a MailChimp portlet in case you want to display your newsletter subscription as part of an existing site.
 
 The newsletter subscriptions forms in both the view and the portlet are extendable, so you can add custom fields that can be stored in your MailChimp subscriber list.
 
@@ -194,16 +190,53 @@
 - Jean-Michel Francois
 - Carsten Senger
 - Peter Holzer
 
 Changelog
 =========
 
-3.1.1 (2023-04-14)
-------------------
+4.0.0a1 (2023-04-14)
+--------------------
+
+Breaking changes:
+
+- Dropped support for Plone 5.1 and older.  [maurits]
+
+- Dropped support for Python 2.  [maurits]
+
+New features:
+
+- Split the controlpanel into two separate pages: settings and data.
+  Until now, if the settings resulted in an error while fetching the data from mailchimp,
+  you could not fix this because the whole control panel would fail to load.
+  Fixes `issue 26 <https://github.com/collective/collective.mailchimp/issues/26>`_.
+  [maurits]
+
+- Updated tests and infrastructure for Plone 5.2, Python 3.
+  Plone 6 should work, but it not tested yet.
+  [maurits]
+
+Bug fixes:
+
+- Reinitialize the locator when called on a different Plone Site.
+  Fixes `issue 31 <https://github.com/collective/collective.mailchimp/issues/31>`_.
+  [maurits]
+
+- Register resource bundle so our css is loaded on Plone 5.2 and higher.  [maurits]
+
+- Increase limit to 50 (by default) when retrieving lists from mailchimp.
+  The API default was getting only 10 lists, which is really too few (and can
+  prevent you from selecting the correct default list for example).
+  The limit is a setting that can be changed on a per-site basis.
+  [laulaz]
+
+- Update portlet template and fix portlet code for Plone 5.2/6. [fredvd]
+
+- Fix posting of interests to the mailchimp API, interest_groups were transformed to bytes string.
+  [fredvd]
 
 - Fix controlpanel field validation for Plone 6
   [agitator]
 
 
 3.1.0 (2020-01-13)
 ------------------
```

### Comparing `collective.mailchimp-3.1.1/src/collective.mailchimp.egg-info/SOURCES.txt` & `collective.mailchimp-4.0.0a1/src/collective.mailchimp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,37 +27,37 @@
 src/collective/mailchimp/upgrades.py
 src/collective/mailchimp/upgrades.zcml
 src/collective/mailchimp/vocabularies.py
 src/collective/mailchimp/browser/__init__.py
 src/collective/mailchimp/browser/configure.zcml
 src/collective/mailchimp/browser/controlpanel.pt
 src/collective/mailchimp/browser/controlpanel.py
+src/collective/mailchimp/browser/data.pt
 src/collective/mailchimp/browser/extender.py
 src/collective/mailchimp/browser/extender.zcml
 src/collective/mailchimp/browser/newsletter.py
 src/collective/mailchimp/browser/portlet.pt
 src/collective/mailchimp/browser/portlet.py
-src/collective/mailchimp/browser/z3cformhelpers.py
 src/collective/mailchimp/browser/images/mailchimp.gif
 src/collective/mailchimp/browser/stylesheets/mailchimp.css
 src/collective/mailchimp/locales/collective.mailchimp.pot
 src/collective/mailchimp/locales/de/LC_MESSAGES/collective.mailchimp.po
 src/collective/mailchimp/locales/fr/LC_MESSAGES/collective.mailchimp.po
 src/collective/mailchimp/locales/it/LC_MESSAGES/collective.mailchimp.po
 src/collective/mailchimp/locales/nl/LC_MESSAGES/collective.mailchimp.po
 src/collective/mailchimp/locales/pt_BR/LC_MESSAGES/collective.mailchimp.po
 src/collective/mailchimp/locales/ro/LC_MESSAGES/collective.mailchimp.po
 src/collective/mailchimp/profiles/default/browserlayer.xml
 src/collective/mailchimp/profiles/default/controlpanel.xml
-src/collective/mailchimp/profiles/default/cssregistry.xml
 src/collective/mailchimp/profiles/default/metadata.xml
 src/collective/mailchimp/profiles/default/portlets.xml
 src/collective/mailchimp/profiles/default/registry.xml
 src/collective/mailchimp/profiles/uninstall/browserlayer.xml
 src/collective/mailchimp/profiles/uninstall/controlpanel.xml
+src/collective/mailchimp/profiles/uninstall/portlets.xml
 src/collective/mailchimp/profiles/uninstall/registry.xml
 src/collective/mailchimp/tests/__init__.py
 src/collective/mailchimp/tests/test_controlpanel.py
 src/collective/mailchimp/tests/test_exceptions.py
 src/collective/mailchimp/tests/test_locator.py
 src/collective/mailchimp/tests/test_mock_requests.py
 src/collective/mailchimp/tests/test_newsletter.py
```

