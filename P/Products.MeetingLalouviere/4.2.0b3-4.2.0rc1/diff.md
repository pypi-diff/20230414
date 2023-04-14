# Comparing `tmp/Products.MeetingLalouviere-4.2.0b3.tar.gz` & `tmp/Products.MeetingLalouviere-4.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.MeetingLalouviere-4.2.0b3.tar", last modified: Thu Apr 13 14:13:15 2023, max compression
+gzip compressed data, was "Products.MeetingLalouviere-4.2.0rc1.tar", last modified: Fri Apr 14 12:41:59 2023, max compression
```

## Comparing `Products.MeetingLalouviere-4.2.0b3.tar` & `Products.MeetingLalouviere-4.2.0rc1.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.256526 Products.MeetingLalouviere-4.2.0b3/
--rw-rw-r--   0 oli       (1000) oli       (1000)     3902 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/CHANGES.rst
--rw-rw-r--   0 oli       (1000) oli       (1000)      354 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/MANIFEST.in
--rw-rw-r--   0 oli       (1000) oli       (1000)     4578 2023-04-13 14:13:15.256526 Products.MeetingLalouviere-4.2.0b3/PKG-INFO
--rw-rw-r--   0 oli       (1000) oli       (1000)       24 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/README.rst
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.240526 Products.MeetingLalouviere-4.2.0b3/docs/
--rw-rw-r--   0 oli       (1000) oli       (1000)     2970 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/docs/HISTORY.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)    18092 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/docs/LICENSE.GPL
--rw-rw-r--   0 oli       (1000) oli       (1000)      736 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/docs/LICENSE.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)      534 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/docs/MIGRATION.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)       38 2023-04-13 14:13:15.256526 Products.MeetingLalouviere-4.2.0b3/setup.cfg
--rw-rw-r--   0 oli       (1000) oli       (1000)     1236 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/setup.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.236526 Products.MeetingLalouviere-4.2.0b3/src/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.240526 Products.MeetingLalouviere-4.2.0b3/src/Products/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.240526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/
--rw-rw-r--   0 oli       (1000) oli       (1000)      973 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/README.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)     1803 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)    33038 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/adapters.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.240526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/browser/
--rw-rw-r--   0 oli       (1000) oli       (1000)       21 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/browser/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1229 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/browser/configure.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)     2220 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/browser/overrides.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.240526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/browser/template/
--rw-rw-r--   0 oli       (1000) oli       (1000)    15578 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/browser/template/meeting_before_faceted_infos.pt
--rw-rw-r--   0 oli       (1000) oli       (1000)     4513 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/browser/views.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     7919 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/config.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      782 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/configure.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)      590 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/events.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      482 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/events.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)      164 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/interfaces.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.244526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/
--rw-rw-r--   0 oli       (1000) oli       (1000)    14405 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/PloneMeeting.pot
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.236526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/en/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.244526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/en/LC_MESSAGES/
--rw-rw-r--   0 oli       (1000) oli       (1000)      750 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/en/LC_MESSAGES/plone.po
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.236526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/fr/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.244526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 oli       (1000) oli       (1000)    22175 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 oli       (1000) oli       (1000)     6551 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 oli       (1000) oli       (1000)     2397 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 oli       (1000) oli       (1000)    10219 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 oli       (1000) oli       (1000)     4344 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/imio.actionspanel.pot
--rw-rw-r--   0 oli       (1000) oli       (1000)     1721 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/imio.history.pot
--rw-rw-r--   0 oli       (1000) oli       (1000)     7851 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/plone.pot
--rwxrwxr-x   0 oli       (1000) oli       (1000)      295 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/sync_pos.sh
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.244526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/migrations/
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/migrations/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1208 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/migrations/add_searches.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     5433 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/migrations/migrate_to_4161.py
--rw-rw-r--   0 oli       (1000) oli       (1000)    54510 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/migrations/migrate_to_4200.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     4299 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/migrations/migrate_to_4_1.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.244526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/model/
--rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/model/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     5039 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/model/pm_updates.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1564 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/overrides.zcml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.244526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/
--rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.244526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/MeetingLalouviere_marker.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      208 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/browserlayer.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      743 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/cssregistry.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      807 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/import_steps.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      246 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/metadata.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      831 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/registry.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      950 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/skins.xml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.244526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/workflows/
--rw-rw-r--   0 oli       (1000) oli       (1000)    21914 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_college.odg
--rw-rw-r--   0 oli       (1000) oli       (1000)    21939 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_council.odg
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.244526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/MeetingLalouviere_testing_marker.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.244526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/
--rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/attach.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/budget.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/budgetAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/cahier.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/decisionAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/financialAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/itemAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/legalAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     3555 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/logo.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)      411 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/negative.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      305 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/nil.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/overheadAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     1147 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/positive.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      355 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/remarks.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      730 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/secretary_remarks.png
--rwxrwxr-x   0 oli       (1000) oli       (1000)     4699 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/import_data.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)      349 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/import_steps.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      176 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/metadata.xml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.244526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/templates/
--rw-rw-r--   0 oli       (1000) oli       (1000)    33545 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/templates/council-oj.odt
--rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/toolset.xml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.248526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/
--rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/MeetingLalouviere_lalouviere_marker.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      760 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/heldpositions.csv
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.248526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/
--rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/attach.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/budget.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/budgetAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     1032 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/decisionAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/financialAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/itemAnnex.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      761 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/legalAdvice.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/legalAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      885 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/negative.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      305 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/nil.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/overheadAnalysis.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      583 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/positive.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      705 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/remarks.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      730 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/secretary_remarks.png
--rw-rw-r--   0 oli       (1000) oli       (1000)    11528 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/import_data.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)      632 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/import_steps.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)      266 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/organizations.csv
--rw-rw-r--   0 oli       (1000) oli       (1000)      726 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/persons.csv
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.252526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/
--rw-rw-r--   0 oli       (1000) oli       (1000)     9511 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)     9909 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib_recto_verso.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)     9605 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_pv.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12386 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendance-stats.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    17906 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendees.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    18854 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/avis-df.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    22380 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-oj.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    22958 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-pv.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12890 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-rapport.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    13154 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/dashboard.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    32698 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    32449 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation_recto_verso.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)     9652 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/history.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12705 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/meeting_assemblies.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    24785 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-annexes.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    24316 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-table-des-matieres.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    24585 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12170 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/organizations-export.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    16342 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/publications.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    23881 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/pv.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12630 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    11565 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    13706 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/report.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    10369 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles1.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    12815 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles2.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    18137 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-avis-df.odt
--rw-rw-r--   0 oli       (1000) oli       (1000)    14290 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-df-tb.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    13865 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/users-groups-export.ods
--rw-rw-r--   0 oli       (1000) oli       (1000)    14862 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/votes.odt
--rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/toolset.xml
--rw-rw-r--   0 oli       (1000) oli       (1000)     1110 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/refresh.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)     4216 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/setuphandlers.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.240526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.252526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/
--rw-rw-r--   0 oli       (1000) oli       (1000)      636 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToAlderman.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      595 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDg.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      646 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDirector.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      662 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDivisionHead.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      583 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToOfficeManager.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToServiceHead.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     6337 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      699 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_no.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      722 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_provided.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      737 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_yes.png
--rw-rw-r--   0 oli       (1000) oli       (1000)     1082 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/not_printed_in_dashboard.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)     1035 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/printed_in_dashboard.gif
--rw-rw-r--   0 oli       (1000) oli       (1000)      651 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToAlderman.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      737 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToBudgetImpactReviewer.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      575 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDg.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      613 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDirector.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      626 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDivisionHead.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      608 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToOfficeManager.png
--rw-rw-r--   0 oli       (1000) oli       (1000)      638 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToServiceHead.png
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.252526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_styles/
--rw-rw-r--   0 oli       (1000) oli       (1000)     3521 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_styles/meetinglalouviere.css.dtml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.252526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/
--rw-rw-r--   0 oli       (1000) oli       (1000)     8366 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_edit.pt
--rw-rw-r--   0 oli       (1000) oli       (1000)    42987 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_view.pt
--rw-rw-r--   0 oli       (1000) oli       (1000)     1023 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/testing.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      593 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/testing.zcml
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.256526 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/
--rwxrwxr-x   0 oli       (1000) oli       (1000)     2161 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/MeetingLalouviereTestCase.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1049 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/__init__.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     6699 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/helpers.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1243 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testAdvices.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1380 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testAnnexes.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1362 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testChangeItemOrderView.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1244 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testColumns.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     3920 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testContacts.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)      551 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1373 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomMeetingConfig.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     7858 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomMeetingItem.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      349 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomSearches.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1360 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomToolPloneMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     3100 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomUtils.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1510 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomViews.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      481 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomWFAdaptations.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1396 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomWorkflows.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1369 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testFaceted.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1300 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1339 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testMeetingCategory.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     6630 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testMeetingConfig.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)     8894 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testMeetingItem.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1290 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testPortlets.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     9778 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testSearches.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1281 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testSetup.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     2279 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testToolPloneMeeting.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     2958 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testUtils.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1293 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testValidators.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     2071 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testViews.py
--rw-rw-r--   0 oli       (1000) oli       (1000)     1239 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testVotes.py
--rw-rw-r--   0 oli       (1000) oli       (1000)    17680 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testWFAdaptations.py
--rwxrwxr-x   0 oli       (1000) oli       (1000)    21049 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testWorkflows.py
--rw-rw-r--   0 oli       (1000) oli       (1000)        7 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/version.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)     1585 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/vocabularies.py
--rw-rw-r--   0 oli       (1000) oli       (1000)      445 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/vocabularies.zcml
--rw-rw-r--   0 oli       (1000) oli       (1000)       56 2023-04-13 14:13:14.000000 Products.MeetingLalouviere-4.2.0b3/src/Products/__init__.py
-drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-13 14:13:15.240526 Products.MeetingLalouviere-4.2.0b3/src/Products.MeetingLalouviere.egg-info/
--rw-rw-r--   0 oli       (1000) oli       (1000)     4578 2023-04-13 14:13:15.000000 Products.MeetingLalouviere-4.2.0b3/src/Products.MeetingLalouviere.egg-info/PKG-INFO
--rw-rw-r--   0 oli       (1000) oli       (1000)    12596 2023-04-13 14:13:15.000000 Products.MeetingLalouviere-4.2.0b3/src/Products.MeetingLalouviere.egg-info/SOURCES.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-04-13 14:13:15.000000 Products.MeetingLalouviere-4.2.0b3/src/Products.MeetingLalouviere.egg-info/dependency_links.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-04-13 14:13:15.000000 Products.MeetingLalouviere-4.2.0b3/src/Products.MeetingLalouviere.egg-info/namespace_packages.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-04-13 14:13:15.000000 Products.MeetingLalouviere-4.2.0b3/src/Products.MeetingLalouviere.egg-info/not-zip-safe
--rw-rw-r--   0 oli       (1000) oli       (1000)      139 2023-04-13 14:13:15.000000 Products.MeetingLalouviere-4.2.0b3/src/Products.MeetingLalouviere.egg-info/requires.txt
--rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-04-13 14:13:15.000000 Products.MeetingLalouviere-4.2.0b3/src/Products.MeetingLalouviere.egg-info/top_level.txt
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.889227 Products.MeetingLalouviere-4.2.0rc1/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4033 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/CHANGES.rst
+-rw-rw-r--   0 oli       (1000) oli       (1000)      354 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/MANIFEST.in
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4710 2023-04-14 12:41:59.889227 Products.MeetingLalouviere-4.2.0rc1/PKG-INFO
+-rw-rw-r--   0 oli       (1000) oli       (1000)       24 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/README.rst
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.865228 Products.MeetingLalouviere-4.2.0rc1/docs/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2970 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/docs/HISTORY.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    18092 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/docs/LICENSE.GPL
+-rw-rw-r--   0 oli       (1000) oli       (1000)      736 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/docs/LICENSE.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)      534 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/docs/MIGRATION.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)       38 2023-04-14 12:41:59.889227 Products.MeetingLalouviere-4.2.0rc1/setup.cfg
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1237 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/setup.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.861228 Products.MeetingLalouviere-4.2.0rc1/src/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.865228 Products.MeetingLalouviere-4.2.0rc1/src/Products/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.865228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      973 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/README.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1803 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)    32845 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/adapters.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.869228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/browser/
+-rw-rw-r--   0 oli       (1000) oli       (1000)       21 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/browser/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1229 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/browser/configure.zcml
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2220 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/browser/overrides.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.869228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/browser/template/
+-rw-rw-r--   0 oli       (1000) oli       (1000)    15578 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/browser/template/meeting_before_faceted_infos.pt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4513 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/browser/views.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     7744 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/config.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      782 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/configure.zcml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      590 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/events.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      482 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/events.zcml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      164 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/interfaces.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.869228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/
+-rw-rw-r--   0 oli       (1000) oli       (1000)    14227 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/PloneMeeting.pot
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.861228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/en/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.869228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      750 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/en/LC_MESSAGES/plone.po
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.861228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/fr/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.869228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 oli       (1000) oli       (1000)    21979 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 oli       (1000) oli       (1000)     6551 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2397 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 oli       (1000) oli       (1000)    10219 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4344 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/imio.actionspanel.pot
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1721 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/imio.history.pot
+-rw-rw-r--   0 oli       (1000) oli       (1000)     7851 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/plone.pot
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      295 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/sync_pos.sh
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.869228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/migrations/
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/migrations/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1208 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/migrations/add_searches.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     5433 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/migrations/migrate_to_4161.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)    54528 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/migrations/migrate_to_4200.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4299 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/migrations/migrate_to_4_1.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.869228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/model/
+-rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/model/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4170 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/model/pm_updates.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1564 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/overrides.zcml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.869228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/
+-rw-rw-r--   0 oli       (1000) oli       (1000)       23 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/__init__.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.869228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/MeetingLalouviere_marker.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      208 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/browserlayer.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      743 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/cssregistry.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      807 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/import_steps.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      246 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/metadata.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      831 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/registry.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      950 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/skins.xml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.869228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/workflows/
+-rw-rw-r--   0 oli       (1000) oli       (1000)    21914 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_college.odg
+-rw-rw-r--   0 oli       (1000) oli       (1000)    21939 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_council.odg
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.873228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/MeetingLalouviere_testing_marker.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/__init__.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.873228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/attach.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/budget.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/budgetAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/cahier.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/decisionAnnex.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/financialAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/itemAnnex.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/legalAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3555 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/logo.gif
+-rw-rw-r--   0 oli       (1000) oli       (1000)      411 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/negative.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      305 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/nil.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/overheadAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1147 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/positive.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      355 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/remarks.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      730 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/secretary_remarks.png
+-rwxrwxr-x   0 oli       (1000) oli       (1000)     4680 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/import_data.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      349 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/import_steps.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      176 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/metadata.xml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.873228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/templates/
+-rw-rw-r--   0 oli       (1000) oli       (1000)    33545 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/templates/council-oj.odt
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/toolset.xml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.877228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      177 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/MeetingLalouviere_lalouviere_marker.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      760 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/heldpositions.csv
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.877228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3352 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/attach.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      630 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/budget.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      492 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/budgetAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1032 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.gif
+-rw-rw-r--   0 oli       (1000) oli       (1000)      731 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/decisionAnnex.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      742 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/financialAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      216 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/itemAnnex.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      761 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/legalAdvice.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      332 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/legalAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      885 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/negative.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      305 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/nil.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      880 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/overheadAnalysis.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      583 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/positive.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      705 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/remarks.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      730 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/secretary_remarks.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)    11505 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/import_data.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      632 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/import_steps.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)      266 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/organizations.csv
+-rw-rw-r--   0 oli       (1000) oli       (1000)      726 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/persons.csv
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.881228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9511 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9909 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib_recto_verso.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9605 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_pv.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12386 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendance-stats.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    17906 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendees.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    18854 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/avis-df.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    22380 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-oj.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    22958 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-pv.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12890 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-rapport.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    13154 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/dashboard.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    32698 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    32449 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation_recto_verso.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9652 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/history.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12705 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/meeting_assemblies.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    24785 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-annexes.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    24316 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-table-des-matieres.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    24585 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12170 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/organizations-export.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    16342 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/publications.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    23881 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/pv.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12630 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    11565 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    13706 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/report.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    10369 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles1.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12815 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles2.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    18137 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-avis-df.odt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    14290 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-df-tb.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    13865 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/users-groups-export.ods
+-rw-rw-r--   0 oli       (1000) oli       (1000)    14862 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/votes.odt
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      167 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/toolset.xml
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1110 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles.zcml
+-rw-rw-r--   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/refresh.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4705 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/setuphandlers.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.861228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.881228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/
+-rw-rw-r--   0 oli       (1000) oli       (1000)      636 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToAlderman.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      595 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDg.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      646 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDirector.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      662 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDivisionHead.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      583 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToOfficeManager.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      649 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToServiceHead.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     6337 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      699 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_no.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      722 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_provided.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      737 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_yes.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1082 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/not_printed_in_dashboard.gif
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1035 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/printed_in_dashboard.gif
+-rw-rw-r--   0 oli       (1000) oli       (1000)      651 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToAlderman.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      737 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToBudgetImpactReviewer.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      575 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDg.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      613 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDirector.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      626 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDivisionHead.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      608 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToOfficeManager.png
+-rw-rw-r--   0 oli       (1000) oli       (1000)      638 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToServiceHead.png
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.881228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_styles/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3521 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_styles/meetinglalouviere.css.dtml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.881228 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     8155 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_edit.pt
+-rw-rw-r--   0 oli       (1000) oli       (1000)    42603 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_view.pt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1023 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/testing.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      593 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/testing.zcml
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.889227 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/
+-rwxrwxr-x   0 oli       (1000) oli       (1000)     2161 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/MeetingLalouviereTestCase.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1049 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/__init__.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     6699 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/helpers.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1243 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testAdvices.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1380 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testAnnexes.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1362 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testChangeItemOrderView.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1244 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testColumns.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3920 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testContacts.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)      551 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomMeeting.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1373 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomMeetingConfig.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     7858 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomMeetingItem.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      349 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomSearches.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1360 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomToolPloneMeeting.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     3100 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomUtils.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1510 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomViews.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      481 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomWFAdaptations.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1396 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomWorkflows.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1369 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testFaceted.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1300 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testMeeting.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1339 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testMeetingCategory.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     6630 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testMeetingConfig.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)     8876 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testMeetingItem.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1290 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testPortlets.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     9778 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testSearches.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1281 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testSetup.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2279 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testToolPloneMeeting.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2958 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testUtils.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1293 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testValidators.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     2071 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testViews.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1239 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testVotes.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)    17680 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testWFAdaptations.py
+-rwxrwxr-x   0 oli       (1000) oli       (1000)    20361 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testWorkflows.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)        7 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/version.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)     1585 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/vocabularies.py
+-rw-rw-r--   0 oli       (1000) oli       (1000)      445 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/vocabularies.zcml
+-rw-rw-r--   0 oli       (1000) oli       (1000)       56 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products/__init__.py
+drwxrwxr-x   0 oli       (1000) oli       (1000)        0 2023-04-14 12:41:59.865228 Products.MeetingLalouviere-4.2.0rc1/src/Products.MeetingLalouviere.egg-info/
+-rw-rw-r--   0 oli       (1000) oli       (1000)     4710 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products.MeetingLalouviere.egg-info/PKG-INFO
+-rw-rw-r--   0 oli       (1000) oli       (1000)    12596 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products.MeetingLalouviere.egg-info/SOURCES.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products.MeetingLalouviere.egg-info/dependency_links.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products.MeetingLalouviere.egg-info/namespace_packages.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        1 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products.MeetingLalouviere.egg-info/not-zip-safe
+-rw-rw-r--   0 oli       (1000) oli       (1000)      139 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products.MeetingLalouviere.egg-info/requires.txt
+-rw-rw-r--   0 oli       (1000) oli       (1000)        9 2023-04-14 12:41:59.000000 Products.MeetingLalouviere-4.2.0rc1/src/Products.MeetingLalouviere.egg-info/top_level.txt
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/CHANGES.rst` & `Products.MeetingLalouviere-4.2.0rc1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 Products.MeetingLalouviere Changelog
 ====================================
 
 The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
 
+4.2.0rc1 (2023-04-14)
+---------------------
+
+- Fix missing getFolloUp index.
+  [odelaere]
+- Deleted neededFollowUp.
+  [odelaere]
+
+
 4.2.0b3 (2023-04-13)
 --------------------
 
 - Added full committees to apply.
   [odelaere]
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/PKG-INFO` & `Products.MeetingLalouviere-4.2.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingLalouviere
-Version: 4.2.0b3
+Version: 4.2.0rc1
 Summary: Official meetings management for college and council custom profile for La Louvière
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Olivier Delaere
 Author-email: olivier.delaere@imio.be
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -19,14 +19,23 @@
 Check 'docs/README.txt'
 
 Products.MeetingLalouviere Changelog
 ====================================
 
 The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
 
+4.2.0rc1 (2023-04-14)
+---------------------
+
+- Fix missing getFolloUp index.
+  [odelaere]
+- Deleted neededFollowUp.
+  [odelaere]
+
+
 4.2.0b3 (2023-04-13)
 --------------------
 
 - Added full committees to apply.
   [odelaere]
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/docs/HISTORY.txt` & `Products.MeetingLalouviere-4.2.0rc1/docs/HISTORY.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/docs/LICENSE.GPL` & `Products.MeetingLalouviere-4.2.0rc1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/docs/LICENSE.txt` & `Products.MeetingLalouviere-4.2.0rc1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/docs/MIGRATION.txt` & `Products.MeetingLalouviere-4.2.0rc1/docs/MIGRATION.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/setup.py` & `Products.MeetingLalouviere-4.2.0rc1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding=utf-8
 from setuptools import setup, find_packages
 
-version = "4.2.0b3"
+version = "4.2.0rc1"
 
 setup(
     name="Products.MeetingLalouviere",
     version=version,
     description="Official meetings management for college and council custom profile for La Louvière",
     long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
     classifiers=[
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/README.txt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/README.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/__init__.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/adapters.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,17 +126,14 @@
     MeetingItem.getLabelDescription = getLabelDescription
 
     security.declarePublic("activateFollowUp")
 
     def activateFollowUp(self):
         """Activate follow-up by setting followUp to 'follow_up_yes'."""
         self.setFollowUp("follow_up_yes")
-        # initialize the neededFollowUp field with the available content of the 'decision' field
-        if not self.getNeededFollowUp():
-            self.setNeededFollowUp(self.getDecision())
         self.reindexObject(
             idxs=["getFollowUp",]
         )
         return self.REQUEST.RESPONSE.redirect(self.absolute_url() + "#followup")
 
     MeetingItem.activateFollowUp = activateFollowUp
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/browser/configure.zcml` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/browser/overrides.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/browser/overrides.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/browser/template/meeting_before_faceted_infos.pt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/browser/template/meeting_before_faceted_infos.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/browser/views.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/browser/views.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/config.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,14 @@
 
 PROJECTNAME = "MeetingLalouviere"
 
 # Permissions
 DEFAULT_WRITE_FOLLOWUP_PERMISSION = "MeetingLalouviere: Write followUp"
 setDefaultRoles(DEFAULT_WRITE_FOLLOWUP_PERMISSION, ('Manager', 'MeetingManager'))
 
-DEFAULT_WRITE_NEEDED_FOLLOWUP_PERMISSION = "MeetingLalouviere: Write neededFollowUp"
-setDefaultRoles(DEFAULT_WRITE_NEEDED_FOLLOWUP_PERMISSION, ('Manager', 'MeetingManager'))
-
 DEFAULT_WRITE_PROVIDED_FOLLOWUP_PERMISSION = "MeetingLalouviere: Write providedFollowUp"
 setDefaultRoles(DEFAULT_WRITE_PROVIDED_FOLLOWUP_PERMISSION, ('Manager', 'MeetingManager', 'MeetingFollowUpWriter'))
 
 product_globals = globals()
 
 DG_GROUP_ID = "direction-generale"
 FALLBACK_DG_GROUP_ID = "dirgen"
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/configure.zcml` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/events.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/events.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/PloneMeeting.pot` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/PloneMeeting.pot`

 * *Files 2% similar despite different names*

```diff
@@ -158,22 +158,14 @@
 msgid "MeetingLalouviere_label_followUp"
 msgstr ""
 
 #. Default: "Follow-up"
 msgid "MeetingLalouviere_descr_followUp"
 msgstr ""
 
-#. Default: "Needed follow-up"
-msgid "MeetingLalouviere_label_neededFollowUp"
-msgstr ""
-
-#. Default: "Needed follow-up"
-msgid "MeetingLalouviere_descr_neededFollowUp"
-msgstr ""
-
 #. Default: "Provided follow-up"
 msgid "MeetingLalouviere_label_providedFollowUp"
 msgstr ""
 
 #. Default: "Provided follow-up"
 msgid "MeetingLalouviere_descr_providedFollowUp"
 msgstr ""
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/en/LC_MESSAGES/plone.po` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/PloneMeeting.po`

 * *Files 1% similar despite different names*

```diff
@@ -36,18 +36,14 @@
 msgid "MeetingLalouviere_descr_followUp"
 msgstr " "
 
 #. Default: "Transcription of interventions"
 msgid "MeetingLalouviere_descr_interventions"
 msgstr "Retranscription des interventions"
 
-#. Default: "Needed follow-up"
-msgid "MeetingLalouviere_descr_neededFollowUp"
-msgstr " "
-
 #. Default: "Provided follow-up"
 msgid "MeetingLalouviere_descr_providedFollowUp"
 msgstr " "
 
 #. Default: "Reference"
 msgid "MeetingLalouviere_label_advice_reference"
 msgstr "Référence"
@@ -76,18 +72,14 @@
 msgid "MeetingLalouviere_label_itemAssembly"
 msgstr "Assemblée spécifique liée à ce point"
 
 #. Default: "Premeeting observations"
 msgid "MeetingLalouviere_label_meetingcouncilobservations"
 msgstr "Avant-séance"
 
-#. Default: "Needed follow-up"
-msgid "MeetingLalouviere_label_neededFollowUp"
-msgstr "Suivi à apporter"
-
 #. Default: "Assembly"
 msgid "MeetingLalouviere_label_preMeetingAssembly"
 msgstr "Assemblée de la Commission"
 
 #. Default: "Assembly"
 msgid "MeetingLalouviere_label_preMeetingAssembly_2"
 msgstr "Assemblée de la Commission"
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.history.po` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/plone.po` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/imio.actionspanel.pot` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/imio.actionspanel.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/imio.history.pot` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/locales/plone.pot` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/migrations/add_searches.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/migrations/add_searches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/migrations/migrate_to_4161.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/migrations/migrate_to_4161.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/migrations/migrate_to_4200.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/migrations/migrate_to_4200.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
                         new_group.addMember(member)
                 group_tool.removeGroup(group.getId())
 
     def _applyMeetingConfig_fixtures(self):
         logger.info('applying meetingconfig fixtures...')
         self.updateTALConditions("year()", "year")
         self.updateTALConditions("month()", "month")
-        self.cleanUsedItemAttributes(['classifier', 'commissionTranscript'])
+        self.cleanUsedItemAttributes(['classifier', 'commissionTranscript', 'neededFollowUp'])
         self.cleanUsedMeetingAttributes(["preMeetingDate", "preMeetingPlace", "preMeetingAssembly",
                                          "preMeetingDate_2", "preMeetingPlace_2", "preMeetingAssembly_2",
                                          "preMeetingDate_3", "preMeetingPlace_3", "preMeetingAssembly_3",
                                          "preMeetingDate_4", "preMeetingPlace_4", "preMeetingAssembly_4",
                                          "preMeetingDate_5", "preMeetingPlace_5", "preMeetingAssembly_5",
                                          "preMeetingDate_6", "preMeetingPlace_6", "preMeetingAssembly_6",
                                          "preMeetingDate_7", "preMeetingPlace_7", "preMeetingAssembly_7",
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/migrations/migrate_to_4_1.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/migrations/migrate_to_4_1.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/model/pm_updates.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/model/pm_updates.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,44 +41,25 @@
         ),
         # here above are 3 specific fields for managing item follow-up
         StringField(
             name='followUp',
             default="follow_up_no",
             widget=SelectionWidget(
                 condition="python: not here.isDefinedInTool() "
-                          "and here.attribute_is_used('neededFollowUp') and here.adapted().showFollowUp()",
+                          "and here.attribute_is_used('providedFollowUp') and here.adapted().showFollowUp()",
                 description="A follow up is needed : no, yes, provided?",
                 description_msgid="MeetingLalouviere_descr_followUp",
                 label='FollowUp',
                 label_msgid='MeetingLalouviere_label_followUp',
                 i18n_domain='PloneMeeting',
             ),
             vocabulary_factory='Products.MeetingLalouviere.vocabularies.listFollowUps',
             write_permission="MeetingLalouviere: Write followUp",
         ),
         TextField(
-            name='neededFollowUp',
-            optional=True,
-            widget=RichWidget(
-                rows=15,
-                condition="python: not here.isDefinedInTool() "
-                          "and here.attribute_is_used('neededFollowUp') and here.adapted().showFollowUp()",
-                label='NeededFollowUp',
-                label_msgid='MeetingLalouviere_label_neededFollowUp',
-                description='Follow-up needed for this item',
-                description_msgid='MeetingLalouviere_descr_neededFollowUp',
-                i18n_domain='PloneMeeting',
-            ),
-            default_content_type="text/html",
-            searchable=True,
-            allowable_content_types=('text/html',),
-            default_output_type="text/html",
-            write_permission="MeetingLalouviere: Write neededFollowUp",
-        ),
-        TextField(
             name='providedFollowUp',
             optional=True,
             widget=RichWidget(
                 rows=15,
                 condition="python: not here.isDefinedInTool() "
                           "and here.attribute_is_used('providedFollowUp') and here.adapted().showFollowUp()",
                 label='ProvidedFollowUp',
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/overrides.zcml` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/overrides.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/cssregistry.xml` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/import_steps.xml` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/registry.xml` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/skins.xml` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_college.odg` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_college.odg`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_council.odg` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/default/workflows/LLO-item_council.odg`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/attach.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/budget.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/cahier.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/financialAnalysis.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/logo.gif` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/logo.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/overheadAnalysis.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/positive.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/images/secretary_remarks.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/images/secretary_remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/import_data.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/import_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 collegeMeeting.itemAdviceStates = [
     "proposed_to_alderman",
 ]
 collegeMeeting.itemAdviceEditStates = [
     "proposed_to_alderman",
     "validated"
 ]
-usedItemAttributes = list(collegeMeeting.usedItemAttributes) + [u"neededFollowUp", u"providedFollowUp",]
+usedItemAttributes = list(collegeMeeting.usedItemAttributes) + [u"providedFollowUp",]
 collegeMeeting.usedItemAttributes = tuple(usedItemAttributes)
 
 # COUNCIL
 councilMeeting = deepcopy(mc_import_data.councilMeeting)
 councilMeeting.itemWFValidationLevels = deepcopy(LLO_ITEM_COUNCIL_WF_VALIDATION_LEVELS)
 councilMeeting.itemAdviceStates = [
     "proposed_to_director",
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/testing/templates/council-oj.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/testing/templates/council-oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/heldpositions.csv` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/heldpositions.csv`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/attach.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/budget.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.gif` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/financialAnalysis.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/legalAdvice.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/negative.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/overheadAnalysis.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/positive.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/remarks.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/images/secretary_remarks.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/images/secretary_remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/import_data.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/import_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,14 @@
     u"proposingGroupWithGroupInCharge",
     u"motivation",
     u"decisionSuite",
     u"internalNotes",
     u"observations",
     u"manuallyLinkedItems",
     u"textCheckList",
-    u"neededFollowUp",
     u"providedFollowUp",
 )
 
 collegeMeeting.usedMeetingAttributes = (
     u"start_date",
     u"end_date",
     u"assembly_guests",
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/import_steps.xml` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/persons.csv` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/persons.csv`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib_recto_verso.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_delib_recto_verso.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_pv.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/all_pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendance-stats.ods` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendance-stats.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendees.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/attendees.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/avis-df.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/avis-df.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-oj.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-pv.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-rapport.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/council-rapport.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/dashboard.ods` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/dashboard.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation_recto_verso.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/deliberation_recto_verso.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/history.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/history.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/meeting_assemblies.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/meeting_assemblies.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-annexes.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-annexes.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-table-des-matieres.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj-avec-table-des-matieres.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/organizations-export.ods` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/organizations-export.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/publications.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/publications.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/pv.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.ods` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/recapitulatif-tb.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/report.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/report.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles1.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles1.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles2.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/styles2.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-avis-df.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-avis-df.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-df-tb.ods` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/synthese-df-tb.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/users-groups-export.ods` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/users-groups-export.ods`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/votes.odt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles/zlalouviere/templates/votes.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/profiles.zcml` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/setuphandlers.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/setuphandlers.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #            http://plone.org/products/archgenxml
 #
 # GNU General Public License (GPL)
 #
 
 import logging
 import os
-
+from imio.helpers.catalog import addOrUpdateIndexes
 from Products.MeetingLalouviere.config import PROJECTNAME
 from Products.PloneMeeting.exportimport.content import ToolInitializer
 
 logger = logging.getLogger('MeetingLalouviere: setuphandlers')
 
 
 def isNotMeetingLalouviereProfile(context):
@@ -27,14 +27,16 @@
     # the right place for your custom code
     if isNotMeetingLalouviereProfile(context):
         return
     logStep("postInstall", context)
     site = context.getSite()
     # need to reinstall PloneMeeting after reinstalling MC workflows to re-apply wfAdaptations
     reinstallPloneMeeting(context, site)
+    # Add additional indexes
+    addAdditionalIndexes(context, site)
     showHomeTab(context, site)
     reorderSkinsLayers(context, site)
 
 
 def logStep(method, context):
     logger.info("Applying '%s' in profile '%s'" %
                 (method, '/'.join(context._profile_path.split(os.sep)[-3:])))
@@ -64,14 +66,30 @@
     # PloneMeeting is no more a dependency to avoid
     # magic between quickinstaller and portal_setup
     # so install it manually
     _installPloneMeeting(context)
     return ToolInitializer(context, PROJECTNAME).run()
 
 
+def addAdditionalIndexes(context, portal):
+    '''
+       Add some specific indexes used by MeetingLalouviere
+    '''
+    if isNotMeetingLalouviereProfile(context):
+        return
+
+    indexInfo = {
+        'getFollowUp': ('FieldIndex', {}),
+    }
+
+    logStep("addAdditionalIndexes", context)
+    # Create or update indexes
+    addOrUpdateIndexes(portal, indexInfo)
+
+
 def reinstallPloneMeeting(context, site):
     '''Reinstall PloneMeeting so after install methods are called and applied,
        like performWorkflowAdaptations for example.'''
 
     if isNotMeetingLalouviereProfile(context):
         return
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToAlderman.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToAlderman.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDg.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDg.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDirector.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDirector.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDivisionHead.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToDivisionHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToOfficeManager.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToOfficeManager.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToServiceHead.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backToProposedToServiceHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/backTo_itemcreated_from_proposed_to_budget_reviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_no.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_no.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_provided.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_provided.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_yes.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/follow_up_yes.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/not_printed_in_dashboard.gif` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/not_printed_in_dashboard.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/printed_in_dashboard.gif` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/printed_in_dashboard.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToAlderman.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToAlderman.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToBudgetImpactReviewer.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToBudgetImpactReviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDg.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDg.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDirector.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDirector.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDivisionHead.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToDivisionHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToOfficeManager.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToOfficeManager.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToServiceHead.png` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_images/proposeToServiceHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_styles/meetinglalouviere.css.dtml` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_styles/meetinglalouviere.css.dtml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_edit.pt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_edit.pt`

 * *Files 1% similar despite different names*

```diff
@@ -134,18 +134,14 @@
     <tal:field define="fieldName python: 'interventions'">
       <metal:f use-macro="context/@@pm-macros/editContentField"/>
     </tal:field>
 
     <tal:comment replace="nothing">XXX followUp</tal:comment>
     <metal:field use-macro="python:here.widget('followUp', mode='edit')"/>
 
-    <tal:comment replace="nothing">XXX neededFollowUp</tal:comment>
-    <tal:field define="fieldName python: 'neededFollowUp'">
-      <metal:f use-macro="context/@@pm-macros/editContentField"/>
-    </tal:field>
     <tal:comment replace="nothing">XXX providedFollowUp</tal:comment>
     <tal:field define="fieldName python: 'providedFollowUp'">
       <metal:f use-macro="context/@@pm-macros/editContentField"/>
     </tal:field>
 
     <metal:field use-macro="python:here.widget('templateUsingGroups', mode='edit')"/>
     <metal:field use-macro="python:here.widget('meetingTransitionInsertingMe', mode='edit')"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 
   Warning
 
  Title and description(s)    Proposing group, category, classifier, toDiscuss
 Clonable to other cfg when not using extra fields                    Budget-
 related information  Budget
              Clonable to other cfg when using extra fields
-XXX Interventions    XXX followUp  XXX neededFollowUp    XXX providedFollowUp
+XXX Interventions    XXX followUp  XXX providedFollowUp
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_view.pt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/skins/meetinglalouviere_templates/meetingitem_view.pt`

 * *Files 1% similar despite different names*

```diff
@@ -646,40 +646,34 @@
 
     <tal:comment replace="nothing">XXX Interventions</tal:comment>
     <tal:field define="fieldName python: 'interventions'; ajaxEdit python:True">
        <metal:f use-macro="context/@@pm-macros/viewContentField"/>
     </tal:field>
 
     <tal:comment replace="nothing">XXX follow-up</tal:comment>
-    <tal:followUp condition="python: 'neededFollowUp' in usedAttrs and here.adapted().showFollowUp()">
+    <tal:followUp condition="python: 'providedFollowUp' in usedAttrs and here.adapted().showFollowUp()">
     <tal:defines define="followUp context/getFollowUp">
      <a name="followup"></a>
      <tal:noFollowUp condition="python: followUp == 'follow_up_no'">
       <tal:translate i18n:translate="no_followup_needed_itemview">No follow-up needed.</tal:translate>
       <tal:translate condition="python: tool.isManager(cfg)" i18n:translate="no_followup_needed_actions_itemview">Actions.</tal:translate>
      </tal:noFollowUp>
      <tal:showFollowUp condition="python: not followUp == 'follow_up_no'">
       <tal:yesFollowUp condition="python: followUp == 'follow_up_yes'">
        <tal:translate i18n:translate="yes_followup_needed_itemview">A follow-up is needed.</tal:translate>
        <tal:translate condition="python: tool.isManager(cfg)" i18n:translate="yes_followup_needed_actions_itemview">Actions.</tal:translate>
-       <tal:field define="fieldName python: 'neededFollowUp'; ajaxEdit python:True">
-         <metal:f use-macro="context/@@pm-macros/viewContentField"/>
-       </tal:field>
        <tal:field define="fieldName python: 'providedFollowUp'; ajaxEdit python:True">
          <metal:f use-macro="context/@@pm-macros/viewContentField"/>
        </tal:field>
       </tal:yesFollowUp>
       <tal:providedFollowUp condition="python: followUp in ['follow_up_provided', 'follow_up_provided_not_printed']">
        <tal:translate tal:condition="python: followUp == 'follow_up_provided'" i18n:translate="provided_followup_itemview">The needed follow-up has been provided.  Click here if you want to define that a follow-up is still needed or click here to deactivate needed follow-up.</tal:translate>
        <tal:translate condition="python: followUp == 'follow_up_provided' and tool.isManager(cfg)" i18n:translate="provided_followup_actions_itemview">Actions.</tal:translate>
        <tal:translate tal:condition="python: followUp == 'follow_up_provided_not_printed'" i18n:translate="provided_followup_not_printed_itemview">The needed follow-up has been provided.  Click here if you want to define that a follow-up is still needed or click here to deactivate needed follow-up.</tal:translate>
        <tal:translate condition="python: followUp == 'follow_up_provided_not_printed' and tool.isManager(cfg)" i18n:translate="provided_followup_not_printed_actions_itemview">Actions.</tal:translate>
-       <fieldset><legend i18n:translate="MeetingLalouviere_label_neededFollowUp">Needed follow-up</legend>
-        <span metal:use-macro="python: here.widget('neededFollowUp', mode='view')" />
-       </fieldset>
        <fieldset><legend i18n:translate="MeetingLalouviere_label_providedFollowUp">Provided follow-up</legend>
         <span metal:use-macro="python: here.widget('providedFollowUp', mode='view')" />
        </fieldset>
       </tal:providedFollowUp>
      </tal:showFollowUp>
      <p>&nbsp;</p>
     </tal:defines>
```

#### html2text {}

```diff
@@ -53,19 +53,19 @@
    Advices
  Text check list
 Text check list Nothing to display.
  In and out moves    Notes    Committee observations    Committee transcript
 Votes observations    Meeting managers notes    Meeting managers notes suite
 Meeting managers notes end    Poll type observations    Observations
 Marginal notes    Internal notes    XXX Interventions    XXX follow-up     No
-follow-up needed. Actions.    A follow-up is needed. Actions.         The
+follow-up needed. Actions.    A follow-up is needed. Actions.      The needed
+follow-up has been provided. Click here if you want to define that a follow-up
+is still needed or click here to deactivate needed follow-up. Actions. The
 needed follow-up has been provided. Click here if you want to define that a
 follow-up is still needed or click here to deactivate needed follow-up.
-Actions. The needed follow-up has been provided. Click here if you want to
-define that a follow-up is still needed or click here to deactivate needed
-follow-up. Actions. Needed follow-up   Provided follow-up
+Actions. Provided follow-up
  
       Fields that appear only if the item is defined in a configuration
 Template using groups:  
 
 Meeting transition inserting me:
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/testing.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/testing.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/testing.zcml` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/MeetingLalouviereTestCase.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/MeetingLalouviereTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/__init__.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/helpers.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testAdvices.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testAnnexes.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testAnnexes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testChangeItemOrderView.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testChangeItemOrderView.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testColumns.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testColumns.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testContacts.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testContacts.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomMeeting.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomMeetingConfig.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomMeetingItem.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomToolPloneMeeting.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomUtils.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomViews.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testCustomWorkflows.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testCustomWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testFaceted.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testFaceted.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testMeeting.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testMeetingCategory.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testMeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testMeetingConfig.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testMeetingItem.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testMeetingItem.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     """
         Tests the MeetingItem class methods.
     """
 
     def _extraNeutralFields(self):
         """This method is made to be overrided by subplugins that added
            neutral fields to the MeetingItem schema."""
-        return ["followUp", "neededFollowUp", "providedFollowUp"]
+        return ["followUp", "providedFollowUp"]
 
     def _get_developers_all_reviewers_groups(self):
         return [self.developers_officemanagers,
                 self.developers_serviceheads,
                 self.developers_divisionheads,
                 self.developers_directors,
                 self.developers_reviewers,
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testPortlets.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testPortlets.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testSearches.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testSearches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testSetup.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testToolPloneMeeting.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testUtils.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testValidators.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testViews.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testVotes.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testVotes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testWFAdaptations.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testWFAdaptations.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/tests/testWorkflows.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/tests/testWorkflows.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,48 +161,37 @@
         self.addAnnex(item2)
         # So now we should have 3 normal item (no recurring items) and one late item in the meeting
         self.assertEqual(len(meeting.get_items(list_types=["normal"])), 3)
         self.assertEqual(len(meeting.get_items(list_types=["late"])), 1)
         self.assertEqual(meeting.get_items(list_types=["late"])[0], item2)
         self.do(meeting, "decide")
         item1.activateFollowUp()
-        self.assertEqual(item1.getDecision(), item1.getNeededFollowUp())
-        item2.activateFollowUp()
-        self.assertEqual(item2.getDecision(), item2.getNeededFollowUp())
         # followup writer cannot edit follow up on frozen items
         self.changeUser("pmFollowup1")
-        self.assertFalse(item1.mayQuickEdit("neededFollowUp"))
         self.assertFalse(item1.mayQuickEdit("providedFollowUp"))
-        # manager can edit neededfollowup for frozen and decided items
         self.changeUser("pmManager")
-        self.assertTrue(item1.mayQuickEdit("neededFollowUp"))
         self.assertTrue(item1.mayQuickEdit("providedFollowUp"))
 
         self.assertEquals(item2.query_state(), "itemfrozen")
-        self.assertTrue(item2.mayQuickEdit("neededFollowUp"))
         self.assertTrue(item2.mayQuickEdit("providedFollowUp"))
 
         self.do(item1, "accept")
         self.assertEquals(item1.query_state(), "accepted")
-        self.assertTrue(item1.mayQuickEdit("neededFollowUp"))
         self.assertTrue(item1.mayQuickEdit("providedFollowUp"))
         self.changeUser("pmFollowup1")
-        self.assertFalse(item1.mayQuickEdit("neededFollowUp"))
         self.assertTrue(item1.mayQuickEdit("providedFollowUp"))
         item1.setProvidedFollowUp("<p>Followed</p>")
         self.changeUser("pmManager")
         item1.confirmFollowUp()
         item1.deactivateFollowUp()
         self.do(meeting, "close")
         # every items without a decision are automatically accepted
         self.assertEquals(item2.query_state(), "accepted")
-        self.assertFalse(item2.mayQuickEdit("neededFollowUp"))
         self.assertFalse(item2.mayQuickEdit("providedFollowUp"))
         self.changeUser("pmFollowup2")
-        self.assertFalse(item2.mayQuickEdit("neededFollowUp"))
         self.assertFalse(item2.mayQuickEdit("providedFollowUp"))
 
     def _testWholeDecisionProcessCouncil(self):
         """
             This test covers the whole decision workflow. It begins with the
             creation of some items, and ends by closing a meeting.
         """
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products/MeetingLalouviere/vocabularies.py` & `Products.MeetingLalouviere-4.2.0rc1/src/Products/MeetingLalouviere/vocabularies.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products.MeetingLalouviere.egg-info/PKG-INFO` & `Products.MeetingLalouviere-4.2.0rc1/src/Products.MeetingLalouviere.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingLalouviere
-Version: 4.2.0b3
+Version: 4.2.0rc1
 Summary: Official meetings management for college and council custom profile for La Louvière
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Olivier Delaere
 Author-email: olivier.delaere@imio.be
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -19,14 +19,23 @@
 Check 'docs/README.txt'
 
 Products.MeetingLalouviere Changelog
 ====================================
 
 The Products.MeetingCommunes version must be the same as the Products.PloneMeeting version
 
+4.2.0rc1 (2023-04-14)
+---------------------
+
+- Fix missing getFolloUp index.
+  [odelaere]
+- Deleted neededFollowUp.
+  [odelaere]
+
+
 4.2.0b3 (2023-04-13)
 --------------------
 
 - Added full committees to apply.
   [odelaere]
```

### Comparing `Products.MeetingLalouviere-4.2.0b3/src/Products.MeetingLalouviere.egg-info/SOURCES.txt` & `Products.MeetingLalouviere-4.2.0rc1/src/Products.MeetingLalouviere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

