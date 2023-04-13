# Comparing `tmp/plone.app.dexterity-3.0.4.tar.gz` & `tmp/plone.app.dexterity-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.dexterity-3.0.4.tar", last modified: Tue Feb  7 23:03:44 2023, max compression
+gzip compressed data, was "plone.app.dexterity-3.0.5.tar", last modified: Thu Apr 13 23:00:21 2023, max compression
```

## Comparing `plone.app.dexterity-3.0.4.tar` & `plone.app.dexterity-3.0.5.tar`

### file list

```diff
@@ -1,196 +1,197 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.981512 plone.app.dexterity-3.0.4/
--rw-r--r--   0 maurits    (501) staff       (20)    31823 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    44145 2023-02-07 23:03:44.981757 plone.app.dexterity-3.0.4/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     6519 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4640 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/RELEASE_NOTES.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.917278 plone.app.dexterity-3.0.4/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      760 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3310 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/Makefile
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.924006 plone.app.dexterity-3.0.4/docs/advanced/
--rw-r--r--   0 maurits    (501) staff       (20)     1951 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/behaviours.rst
--rw-r--r--   0 maurits    (501) staff       (20)    14910 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/catalog-indexing-strategies.rst
--rw-r--r--   0 maurits    (501) staff       (20)     9635 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/custom-add-and-edit-forms.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3181 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/custom-content-classes.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2145 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/defaults.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5190 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/event-handlers.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4599 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/files-and-images.rst
--rw-r--r--   0 maurits    (501) staff       (20)      492 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6970 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/permissions.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7155 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/references.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7451 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/rich-text-markup-transformations.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5276 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/static-resources.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3814 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/validators.rst
--rw-r--r--   0 maurits    (501) staff       (20)    13226 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/vocabularies.rst
--rw-r--r--   0 maurits    (501) staff       (20)    21829 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/webdav-and-other-file-representations.rst
--rw-r--r--   0 maurits    (501) staff       (20)    16315 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/advanced/workflow.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.927167 plone.app.dexterity-3.0.4/docs/behaviors/
--rw-r--r--   0 maurits    (501) staff       (20)     1931 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/behaviors/behavior-basics.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5438 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/behaviors/creating-and-registering-behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)      278 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/behaviors/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2083 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/behaviors/intro.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10191 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/behaviors/providing-marker-interfaces.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5855 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/behaviors/schema-only-behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)    11007 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/behaviors/testing-behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7118 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)    10738 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/custom-views.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2354 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/designing.rst
--rw-r--r--   0 maurits    (501) staff       (20)      460 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)      943 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/install.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5693 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/intro.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3973 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/model-driven-types.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6303 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/prerequisite.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.930597 plone.app.dexterity-3.0.4/docs/reference/
--rw-r--r--   0 maurits    (501) staff       (20)     9806 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/reference/dexterity-xml.rst
--rw-r--r--   0 maurits    (501) staff       (20)    14982 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/reference/fields.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8261 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/reference/form-schema-hints.rst
--rw-r--r--   0 maurits    (501) staff       (20)      270 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/reference/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)    35076 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/reference/manipulating-content-objects.rst
--rw-r--r--   0 maurits    (501) staff       (20)      871 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/reference/misc.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6133 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/reference/standard-behaviours.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3419 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/reference/widgets.rst
--rw-r--r--   0 maurits    (501) staff       (20)    16976 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/schema-driven-types.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.932261 plone.app.dexterity-3.0.4/docs/testing/
--rw-r--r--   0 maurits    (501) staff       (20)      186 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/testing/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)    14392 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/testing/integration-tests.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10941 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/testing/mock-testing.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5860 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/docs/testing/unit-tests.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.932669 plone.app.dexterity-3.0.4/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.936533 plone.app.dexterity-3.0.4/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.941027 plone.app.dexterity-3.0.4/plone/app/dexterity/
--rw-r--r--   0 maurits    (501) staff       (20)      672 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/TODO.txt
--rw-r--r--   0 maurits    (501) staff       (20)      113 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.945153 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5076 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6908 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/constrains.py
--rw-r--r--   0 maurits    (501) staff       (20)     1103 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/discussion.py
--rw-r--r--   0 maurits    (501) staff       (20)     1759 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/exclfromnav.py
--rw-r--r--   0 maurits    (501) staff       (20)      963 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/filename.py
--rw-r--r--   0 maurits    (501) staff       (20)     1809 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/id.py
--rw-r--r--   0 maurits    (501) staff       (20)    12304 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/metadata.py
--rw-r--r--   0 maurits    (501) staff       (20)     4533 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/nextprevious.py
--rw-r--r--   0 maurits    (501) staff       (20)      441 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/related.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.946867 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2827 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/tests/test_contrains.py
--rw-r--r--   0 maurits    (501) staff       (20)     5129 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/tests/test_id.py
--rw-r--r--   0 maurits    (501) staff       (20)     4370 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/tests/test_metadata.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.957420 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1752 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/add_type.py
--rw-r--r--   0 maurits    (501) staff       (20)     1255 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/behaviors.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4443 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/blank.css
--rw-r--r--   0 maurits    (501) staff       (20)     1224 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/clone_type.py
--rw-r--r--   0 maurits    (501) staff       (20)     4136 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1471 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/container.pt
--rw-r--r--   0 maurits    (501) staff       (20)      597 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/default_page_warning.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4540 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/export.py
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)     5288 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/folder_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3408 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/folder_listing.py
--rw-r--r--   0 maurits    (501) staff       (20)     6393 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/import_types.py
--rw-r--r--   0 maurits    (501) staff       (20)     1145 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/item.pt
--rw-r--r--   0 maurits    (501) staff       (20)      430 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     2083 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/modeleditor.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5644 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/modeleditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     1899 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/overview.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1177 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/overview.py
--rw-r--r--   0 maurits    (501) staff       (20)     1153 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/tabbed_forms.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10143 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/types.py
--rw-r--r--   0 maurits    (501) staff       (20)     1011 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/types_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1193 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/types_listing_row.pt
--rw-r--r--   0 maurits    (501) staff       (20)      622 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/typesformwrapper.pt
--rw-r--r--   0 maurits    (501) staff       (20)      249 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/browser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2826 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      542 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/events.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2218 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/factories.py
--rw-r--r--   0 maurits    (501) staff       (20)     3668 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      435 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      248 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/overrides.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4664 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/permissions.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.906973 plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.958261 plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      441 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      168 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/default/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.959086 plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/testing/
--rw-r--r--   0 maurits    (501) staff       (20)      231 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/testing/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.959916 plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/testing/types/
--rw-r--r--   0 maurits    (501) staff       (20)     1993 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/testing/types/Document.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2237 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/testing/types/Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      282 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/testing/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1661 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/serialize.py
--rw-r--r--   0 maurits    (501) staff       (20)     1074 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.966674 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/discussion.txt
--rw-r--r--   0 maurits    (501) staff       (20)    22664 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/editing.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1851 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/filename.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.967093 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/import/
--rw-r--r--   0 maurits    (501) staff       (20)     5804 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/import/dexterity_export.zip
--rw-r--r--   0 maurits    (501) staff       (20)     2498 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/metadata.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1777 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/namefromtitle.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3592 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/nextprevious.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.967547 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)     1082 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/robot/test_types.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1458 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/schema_events.txt
--rw-r--r--   0 maurits    (501) staff       (20)    19024 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_constrains.py
--rw-r--r--   0 maurits    (501) staff       (20)      788 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     1857 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_export.py
--rw-r--r--   0 maurits    (501) staff       (20)     2851 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_import.py
--rw-r--r--   0 maurits    (501) staff       (20)     8202 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_nextprevious.py
--rw-r--r--   0 maurits    (501) staff       (20)     9192 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_permissions.py
--rw-r--r--   0 maurits    (501) staff       (20)      826 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)     2320 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_upgrades.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.972163 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/
--rw-r--r--   0 maurits    (501) staff       (20)      555 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      293 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/behavior.py
--rw-r--r--   0 maurits    (501) staff       (20)     2215 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5029 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/converters.py
--rw-r--r--   0 maurits    (501) staff       (20)      890 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     5292 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/indexer.py
--rw-r--r--   0 maurits    (501) staff       (20)     1046 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2340 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     1340 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/supermodel.py
--rw-r--r--   0 maurits    (501) staff       (20)     2664 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.976954 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3000 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)     9879 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2516 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      376 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/helpers.py
--rw-r--r--   0 maurits    (501) staff       (20)      434 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/test_basic_behavior.py
--rw-r--r--   0 maurits    (501) staff       (20)      793 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/test_behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)     1610 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/test_directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     3657 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/test_schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     3737 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py
--rw-r--r--   0 maurits    (501) staff       (20)     1794 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1170 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.981167 plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2398 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      249 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/to1.py
--rw-r--r--   0 maurits    (501) staff       (20)      195 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/to2.py
--rw-r--r--   0 maurits    (501) staff       (20)      221 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/to2000.py
--rw-r--r--   0 maurits    (501) staff       (20)      631 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/to2001.py
--rw-r--r--   0 maurits    (501) staff       (20)      268 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/to2002.py
--rw-r--r--   0 maurits    (501) staff       (20)      606 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/to2003.py
--rw-r--r--   0 maurits    (501) staff       (20)      978 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/to2004.py
--rw-r--r--   0 maurits    (501) staff       (20)     1444 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/to2005.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:03:44.936130 plone.app.dexterity-3.0.4/plone.app.dexterity.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    44145 2023-02-07 23:03:44.000000 plone.app.dexterity-3.0.4/plone.app.dexterity.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     6585 2023-02-07 23:03:44.000000 plone.app.dexterity-3.0.4/plone.app.dexterity.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-07 23:03:44.000000 plone.app.dexterity-3.0.4/plone.app.dexterity.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-02-07 23:03:44.000000 plone.app.dexterity-3.0.4/plone.app.dexterity.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-02-07 23:03:44.000000 plone.app.dexterity-3.0.4/plone.app.dexterity.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-07 23:03:44.000000 plone.app.dexterity-3.0.4/plone.app.dexterity.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      704 2023-02-07 23:03:44.000000 plone.app.dexterity-3.0.4/plone.app.dexterity.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-02-07 23:03:44.000000 plone.app.dexterity-3.0.4/plone.app.dexterity.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      245 2023-02-07 23:03:44.982513 plone.app.dexterity-3.0.4/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2991 2023-02-07 23:03:43.000000 plone.app.dexterity-3.0.4/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.884066 plone.app.dexterity-3.0.5/
+-rw-r--r--   0 maurits    (501) staff       (20)    32040 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    44362 2023-04-13 23:00:21.884211 plone.app.dexterity-3.0.5/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     6519 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4640 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/RELEASE_NOTES.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.837452 plone.app.dexterity-3.0.5/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      760 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3310 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/Makefile
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.842091 plone.app.dexterity-3.0.5/docs/advanced/
+-rw-r--r--   0 maurits    (501) staff       (20)     1951 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/behaviours.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    14910 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/catalog-indexing-strategies.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     9635 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/custom-add-and-edit-forms.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3181 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/custom-content-classes.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2145 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/defaults.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5191 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/event-handlers.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4599 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/files-and-images.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      492 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6971 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/permissions.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7156 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/references.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7451 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/rich-text-markup-transformations.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5276 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/static-resources.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3814 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/validators.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    13226 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/vocabularies.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    21829 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/webdav-and-other-file-representations.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    16315 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/workflow.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.844355 plone.app.dexterity-3.0.5/docs/behaviors/
+-rw-r--r--   0 maurits    (501) staff       (20)     1931 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/behavior-basics.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5438 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/creating-and-registering-behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      278 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2083 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/intro.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10191 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/providing-marker-interfaces.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5855 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/schema-only-behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    11007 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/testing-behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7095 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10739 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/custom-views.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2354 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/designing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      460 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      943 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/install.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5693 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/intro.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3973 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/model-driven-types.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6303 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/prerequisite.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.846612 plone.app.dexterity-3.0.5/docs/reference/
+-rw-r--r--   0 maurits    (501) staff       (20)     9806 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/dexterity-xml.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    14982 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/fields.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8261 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/form-schema-hints.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      270 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    35076 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/manipulating-content-objects.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      871 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/misc.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6133 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/standard-behaviours.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3419 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/widgets.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    16977 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/schema-driven-types.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.847821 plone.app.dexterity-3.0.5/docs/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)      186 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/testing/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    14392 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/testing/integration-tests.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10941 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/testing/mock-testing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5860 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/testing/unit-tests.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.848084 plone.app.dexterity-3.0.5/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.851495 plone.app.dexterity-3.0.5/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.854796 plone.app.dexterity-3.0.5/plone/app/dexterity/
+-rw-r--r--   0 maurits    (501) staff       (20)      672 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       76 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.857800 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5114 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6908 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/constrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1102 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/discussion.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1759 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/exclfromnav.py
+-rw-r--r--   0 maurits    (501) staff       (20)      963 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/filename.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1808 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/id.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12317 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/metadata.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4533 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/nextprevious.py
+-rw-r--r--   0 maurits    (501) staff       (20)      441 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/related.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.858899 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2827 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/test_contrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5128 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/test_id.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4370 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/test_metadata.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.866950 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1751 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/add_type.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1597 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/behaviors.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4442 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/blank.css
+-rw-r--r--   0 maurits    (501) staff       (20)     1223 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/clone_type.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4177 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1740 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/container.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      661 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/default_page_warning.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4539 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/export.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6792 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/folder_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3408 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/folder_listing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6391 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/import_types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1307 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/item.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      429 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2493 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/modeleditor.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5644 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/modeleditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2264 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/overview.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1177 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/overview.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1297 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/tabbed_forms.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10142 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1098 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/types_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1350 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/types_listing_row.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      710 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/typesformwrapper.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      249 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2770 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      547 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/events.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2219 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/factories.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3667 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      482 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/meta.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      271 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/overrides.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4664 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/permissions.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.830563 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.867606 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      591 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      186 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/default/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.868126 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)      248 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.868654 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2214 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types/Document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2467 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types/Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      356 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1661 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/serialize.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1074 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.873270 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/discussion.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    22722 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/editing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1851 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/filename.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.873619 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/import/
+-rw-r--r--   0 maurits    (501) staff       (20)     5804 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/import/dexterity_export.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     2498 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/metadata.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1777 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/namefromtitle.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3592 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/nextprevious.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.873892 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)     1082 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/robot/test_types.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1458 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/schema_events.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    19024 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_constrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)      778 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1857 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_export.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2851 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_import.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8202 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_nextprevious.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9191 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_permissions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      826 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1586 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_upgrades.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.877166 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/
+-rw-r--r--   0 maurits    (501) staff       (20)      555 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      293 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/behavior.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2066 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5051 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/converters.py
+-rw-r--r--   0 maurits    (501) staff       (20)      890 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/directives.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5290 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/indexer.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1046 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2339 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1340 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/supermodel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2662 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.880573 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3249 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11423 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2524 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    21311 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/file.pdf
+-rw-r--r--   0 maurits    (501) staff       (20)      376 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/helpers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      434 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_basic_behavior.py
+-rw-r--r--   0 maurits    (501) staff       (20)      792 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1610 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_directives.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3767 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1793 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1170 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.883795 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2416 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      249 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to1.py
+-rw-r--r--   0 maurits    (501) staff       (20)      195 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2.py
+-rw-r--r--   0 maurits    (501) staff       (20)      221 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2000.py
+-rw-r--r--   0 maurits    (501) staff       (20)      631 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2001.py
+-rw-r--r--   0 maurits    (501) staff       (20)      268 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2002.py
+-rw-r--r--   0 maurits    (501) staff       (20)      606 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2003.py
+-rw-r--r--   0 maurits    (501) staff       (20)      976 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2004.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1444 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2005.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.851255 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    44362 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     6632 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      829 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1889 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      287 2023-04-13 23:00:21.884672 plone.app.dexterity-3.0.5/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     3209 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/setup.py
```

### Comparing `plone.app.dexterity-3.0.4/CHANGES.rst` & `plone.app.dexterity-3.0.5/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.5 (2023-04-14)
+------------------
+
+Bug fixes:
+
+
+- Fix for searchable Named(Blob)File indexer. Safely convert to str.
+  [petschki] (#362)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (#47959565)
+
+
 3.0.4 (2023-02-08)
 ------------------
 
 Bug fixes:
 
 
 - Restore and deprecate "ModelEditorView.modelSource".
@@ -91,15 +108,15 @@
 ---------------------
 
 Bug fixes:
 
 
 - Rename "Dexterity Content Types" to just "Content Types"
   [tisto] (#331)
-- Don't acquire lanuage from portal root default_language for ICategorization.language.
+- Don't acquire language from portal root default_language for ICategorization.language.
   Fixes https://github.com/plone/plone.app.dexterity/issues/258
   [jaroel] (#350)
 
 
 3.0.0a10 (2022-05-09)
 ---------------------
 
@@ -488,15 +505,15 @@
   New: For add forms use the "Add portal content" permission as default field permission.
   As great side effect vocabularies for i.e. AjaxSelectWidget from ``plone.app.content``,
   which are using the check, are working on add forms in a context w/o "Modify portal content".
   [jensens]
 - removed deprecated getIcon() from documentation
   [fgrcon]
 
-- JavaScript formating according to style guides.
+- JavaScript formatting according to style guides.
   [thet]
 
 
 2.4.1 (2017-03-26)
 ------------------
 
 Bug fixes:
@@ -871,15 +888,15 @@
   from Plone transifex organization [macagua].
 
 - Updated Spanish translation [flamelcanto, macagua].
 
 - Add validator to ensure expires date is after effective date.
   [benniboy]
 
-- Remove line feeds and carrige returns from meta description and
+- Remove line feeds and carriage returns from meta description and
   added upgrade step to do it for existing content
   [bosim]
 
 - Fixed issue.
   Multiple (two or more) acquisition from parent was failing when
   user didn't have add permission on parent.
   [keul, cekk]
```

### Comparing `plone.app.dexterity-3.0.4/PKG-INFO` & `plone.app.dexterity-3.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.dexterity
-Version: 3.0.4
+Version: 3.0.5
 Summary: Dexterity is a content type framework for CMF  applications, with particular emphasis on Plone. It can be viewed as an alternative to Archetypes that is more light-weight and modular.
 Home-page: http://plone.org/products/dexterity
 Author: Martin Aspeli, David Glick, et al
 Author-email: dexterity-development@googlegroups.com
 License: GPL
 Keywords: plone ttw dexterity schema interface
 Classifier: Development Status :: 5 - Production/Stable
@@ -327,14 +327,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.5 (2023-04-14)
+------------------
+
+Bug fixes:
+
+
+- Fix for searchable Named(Blob)File indexer. Safely convert to str.
+  [petschki] (#362)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (#47959565)
+
+
 3.0.4 (2023-02-08)
 ------------------
 
 Bug fixes:
 
 
 - Restore and deprecate "ModelEditorView.modelSource".
@@ -414,15 +431,15 @@
 ---------------------
 
 Bug fixes:
 
 
 - Rename "Dexterity Content Types" to just "Content Types"
   [tisto] (#331)
-- Don't acquire lanuage from portal root default_language for ICategorization.language.
+- Don't acquire language from portal root default_language for ICategorization.language.
   Fixes https://github.com/plone/plone.app.dexterity/issues/258
   [jaroel] (#350)
 
 
 3.0.0a10 (2022-05-09)
 ---------------------
 
@@ -811,15 +828,15 @@
   New: For add forms use the "Add portal content" permission as default field permission.
   As great side effect vocabularies for i.e. AjaxSelectWidget from ``plone.app.content``,
   which are using the check, are working on add forms in a context w/o "Modify portal content".
   [jensens]
 - removed deprecated getIcon() from documentation
   [fgrcon]
 
-- JavaScript formating according to style guides.
+- JavaScript formatting according to style guides.
   [thet]
 
 
 2.4.1 (2017-03-26)
 ------------------
 
 Bug fixes:
@@ -1194,15 +1211,15 @@
   from Plone transifex organization [macagua].
 
 - Updated Spanish translation [flamelcanto, macagua].
 
 - Add validator to ensure expires date is after effective date.
   [benniboy]
 
-- Remove line feeds and carrige returns from meta description and
+- Remove line feeds and carriage returns from meta description and
   added upgrade step to do it for existing content
   [bosim]
 
 - Fixed issue.
   Multiple (two or more) acquisition from parent was failing when
   user didn't have add permission on parent.
   [keul, cekk]
```

### Comparing `plone.app.dexterity-3.0.4/README.rst` & `plone.app.dexterity-3.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/RELEASE_NOTES.rst` & `plone.app.dexterity-3.0.5/RELEASE_NOTES.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/LICENSE.GPL` & `plone.app.dexterity-3.0.5/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/LICENSE.txt` & `plone.app.dexterity-3.0.5/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/Makefile` & `plone.app.dexterity-3.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/behaviours.rst` & `plone.app.dexterity-3.0.5/docs/advanced/behaviours.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/catalog-indexing-strategies.rst` & `plone.app.dexterity-3.0.5/docs/advanced/catalog-indexing-strategies.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/custom-add-and-edit-forms.rst` & `plone.app.dexterity-3.0.5/docs/advanced/custom-add-and-edit-forms.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/custom-content-classes.rst` & `plone.app.dexterity-3.0.5/docs/advanced/custom-content-classes.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/defaults.rst` & `plone.app.dexterity-3.0.5/docs/advanced/defaults.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/event-handlers.rst` & `plone.app.dexterity-3.0.5/docs/advanced/event-handlers.rst`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 ``zope.lifecycleevent.interfaces.IObjectRemovedEvent``
     fired when an object has been removed from its container.
     The container is available as the ``oldParent`` attribute.
     The name the item held in the container is available as ``oldName``.
 
 ``OFS.interfaces.IObjectWillBeRemovedEvent``
-    fired before an object is removed. Until here no deletion has happend.
+    fired before an object is removed. Until here no deletion has happened.
     It is also fired on move of an object (copy/paste).
 
 ``zope.lifecycleevent.interfaces.IObjectMovedEvent``
     fired when an object is added to, removed from, renamed in, or moved between containers.
     This event is a super-type of ``IObjectAddedEvent`` and ``IObjectRemovedEvent``, shown above.
     An event handler registered for this interface will be invoked for the ‘added’ and ‘removed’ cases as well.
     When an object is moved or renamed, all of ``oldParent``, ``newParent``, ``oldName`` and ``newName`` will be set.
```

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/files-and-images.rst` & `plone.app.dexterity-3.0.5/docs/advanced/files-and-images.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/permissions.rst` & `plone.app.dexterity-3.0.5/docs/advanced/permissions.rst`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 (if you use custom views that access the attribute directly, you’ll need to perform your own checks).
 Write permissions can be used to control whether or not a given field appears on a type’s add and edit forms.
 
 In both cases,
 read and write permissions are annotated onto the schema using directives similar to those we’ve already seen for form widget hints.
 The ``read_permission()`` and ``write_permission()`` directives are found in the `plone.autoform`_ package.
 
-If XML-schemas are used for defintion see :ref:`Dexterity XML: security attributes <dexterity-xml-security>`.
+If XML-schemas are used for definition see :ref:`Dexterity XML: security attributes <dexterity-xml-security>`.
 
 Simple example protecting a field to be readable for Site Administrators only::
 
     from zope import schema
     from plone.supermodel import model
     from plone.autoform.directives import read_permission, write_permission
```

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/references.rst` & `plone.app.dexterity-3.0.5/docs/advanced/references.rst`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             title=_(u"Presenter"),
             source=ObjPathSourceBinder(object_provides=IPresenter.__identifier__),
             required=False,
         )
 
 .. Note::
 
-    Remeber that `plone.app.relationfield`_ needs to be installed to use any
+    Remember that `plone.app.relationfield`_ needs to be installed to use any
     RelationChoice or RelationList field.
 
 To allow multiple items to be selected, we could have used a
 ``RelationList`` like::
 
     relatedItems = RelationList(
         title=u"Related Items",
```

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/rich-text-markup-transformations.rst` & `plone.app.dexterity-3.0.5/docs/advanced/rich-text-markup-transformations.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/static-resources.rst` & `plone.app.dexterity-3.0.5/docs/advanced/static-resources.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/validators.rst` & `plone.app.dexterity-3.0.5/docs/advanced/validators.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/vocabularies.rst` & `plone.app.dexterity-3.0.5/docs/advanced/vocabularies.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/webdav-and-other-file-representations.rst` & `plone.app.dexterity-3.0.5/docs/advanced/webdav-and-other-file-representations.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/advanced/workflow.rst` & `plone.app.dexterity-3.0.5/docs/advanced/workflow.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/behaviors/behavior-basics.rst` & `plone.app.dexterity-3.0.5/docs/behaviors/behavior-basics.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/behaviors/creating-and-registering-behaviors.rst` & `plone.app.dexterity-3.0.5/docs/behaviors/creating-and-registering-behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/behaviors/intro.rst` & `plone.app.dexterity-3.0.5/docs/behaviors/intro.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/behaviors/providing-marker-interfaces.rst` & `plone.app.dexterity-3.0.5/docs/behaviors/providing-marker-interfaces.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/behaviors/schema-only-behaviors.rst` & `plone.app.dexterity-3.0.5/docs/behaviors/schema-only-behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/behaviors/testing-behaviors.rst` & `plone.app.dexterity-3.0.5/docs/behaviors/testing-behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/conf.py` & `plone.app.dexterity-3.0.5/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,14 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import os
-import sys
-
-
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 # sys.path.append(os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
```

### Comparing `plone.app.dexterity-3.0.4/docs/custom-views.rst` & `plone.app.dexterity-3.0.5/docs/custom-views.rst`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 We have added ``sessions``, a helper method which will be used in the view.
 
 You can add any methods to the view.
 They will be available to the template via the ``view`` variable.
 The content object is available via ``context``.
 
-Finaly add a template in ``templates/programview.pt``:
+Finally add a template in ``templates/programview.pt``:
 
 .. code-block:: html
 
     <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
           xmlns:tal="http://xml.zope.org/namespaces/tal"
           xmlns:metal="http://xml.zope.org/namespaces/metal"
           xmlns:i18n="http://xml.zope.org/namespaces/i18n"
```

### Comparing `plone.app.dexterity-3.0.4/docs/designing.rst` & `plone.app.dexterity-3.0.5/docs/designing.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/install.rst` & `plone.app.dexterity-3.0.5/docs/install.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/intro.rst` & `plone.app.dexterity-3.0.5/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/model-driven-types.rst` & `plone.app.dexterity-3.0.5/docs/model-driven-types.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/prerequisite.rst` & `plone.app.dexterity-3.0.5/docs/prerequisite.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/reference/dexterity-xml.rst` & `plone.app.dexterity-3.0.5/docs/reference/dexterity-xml.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/reference/fields.rst` & `plone.app.dexterity-3.0.5/docs/reference/fields.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/reference/form-schema-hints.rst` & `plone.app.dexterity-3.0.5/docs/reference/form-schema-hints.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/reference/manipulating-content-objects.rst` & `plone.app.dexterity-3.0.5/docs/reference/manipulating-content-objects.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/reference/misc.rst` & `plone.app.dexterity-3.0.5/docs/reference/misc.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/reference/standard-behaviours.rst` & `plone.app.dexterity-3.0.5/docs/reference/standard-behaviours.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/reference/widgets.rst` & `plone.app.dexterity-3.0.5/docs/reference/widgets.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/schema-driven-types.rst` & `plone.app.dexterity-3.0.5/docs/schema-driven-types.rst`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
 -  The schema interface is referenced by the ``schema`` property.
 -  The ``klass`` property designates the base class of the content type.
    Use ``plone.dexterity.content.Item`` or ``plone.dexterity.content.Container`` for a basic Dexterity Item (non-container) or Container for a type that acts like a folder.
    You may also use your own class declarations if you wish to add class members or methods.
    These are usually derived from Item or Container.
 -  We specify the name of an add permission.
    The default ``cmf.AddPortalContent`` should be used unless you configure a custom permission.
-   Custom permissions are convered later in this manual.
+   Custom permissions are converted later in this manual.
 -  We add a *behavior*.
    Behaviors are re-usable aspects providing semantics and/or schema fields.
    Here, we add the ``INameFromTitle`` behavior, which will give our content object a readable id based on the ``title`` property. We’ll cover other behaviors later.
 
 The ``Program``, in ``program.xml``, looks like this:
 
 .. code-block:: xml
```

### Comparing `plone.app.dexterity-3.0.4/docs/testing/integration-tests.rst` & `plone.app.dexterity-3.0.5/docs/testing/integration-tests.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/testing/mock-testing.rst` & `plone.app.dexterity-3.0.5/docs/testing/mock-testing.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/docs/testing/unit-tests.rst` & `plone.app.dexterity-3.0.5/docs/testing/unit-tests.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/TODO.txt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/TODO.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/configure.zcml` & `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/configure.zcml`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:plone="http://namespaces.plone.org/plone"
     xmlns:zcml="http://namespaces.zope.org/zcml"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
-  <include package="plone.behavior" file="meta.zcml"/>
+  <include
+      package="plone.behavior"
+      file="meta.zcml"
+      />
 
   <!-- vocabularies -->
-  <include package="plone.app.vocabularies"/>
+  <include package="plone.app.vocabularies" />
 
   <!-- Metadata -->
   <plone:behavior
       name="plone.basic"
       title="Basic metadata"
       description="Adds title and description fields."
-      provides=".metadata.IBasic"
       factory=".metadata.Basic"
+      provides=".metadata.IBasic"
       for="plone.dexterity.interfaces.IDexterityContent"
       />
   <plone:behavior
-      title="Categorization"
       name="plone.categorization"
+      title="Categorization"
       description="Adds keywords and language fields."
-      provides=".metadata.ICategorization"
       factory=".metadata.Categorization"
+      provides=".metadata.ICategorization"
       for="plone.dexterity.interfaces.IDexterityContent"
       />
   <plone:behavior
       name="plone.publication"
       title="Date range"
       description="Adds effective date and expiration date fields."
-      provides=".metadata.IPublication"
       factory=".metadata.Publication"
+      provides=".metadata.IPublication"
       for="plone.dexterity.interfaces.IDexterityContent"
       />
   <plone:behavior
       name="plone.ownership"
       title="Ownership"
       description="Adds creator, contributor, and rights fields."
-      provides=".metadata.IOwnership"
       factory=".metadata.Ownership"
+      provides=".metadata.IOwnership"
       for="plone.dexterity.interfaces.IDexterityContent"
       />
   <adapter
-      name="default"
       factory=".metadata.CreatorsDefaultValue"
+      name="default"
       />
   <plone:behavior
       name="plone.dublincore"
       title="Dublin Core metadata"
       description="Adds standard metadata fields (equals Basic metadata + Categorization + Effective range + Ownership)"
-      provides=".metadata.IDublinCore"
       factory=".metadata.DublinCore"
+      provides=".metadata.IDublinCore"
       for="plone.dexterity.interfaces.IDexterityContent"
       />
 
   <!-- Title-to-id -->
   <plone:behavior
       name="plone.namefromtitle"
       title="Name from title"
@@ -85,16 +89,16 @@
   <plone:behavior
       name="plone.excludefromnavigation"
       title="Exclude From navigation"
       description="Allow items to be excluded from navigation"
       provides=".exclfromnav.IExcludeFromNavigation"
       />
   <adapter
-      for="*"
       factory=".exclfromnav.default_exclude_false"
+      for="*"
       />
 
   <!-- Next previous -->
   <plone:behavior
       name="plone.nextprevioustoggle"
       title="Next previous navigation toggle"
       description="Allow items to have next previous navigation enabled"
@@ -109,15 +113,16 @@
       provides=".discussion.IAllowDiscussion"
       />
 
   <adapter factory=".nextprevious.NextPreviousToggle" />
 
   <adapter
       factory=".nextprevious.DefaultNextPreviousEnabled"
-      name="default" />
+      name="default"
+      />
 
   <plone:behavior
       name="plone.nextpreviousenabled"
       title="Next previous navigation"
       description="Enable next previous navigation for all items of this type"
       provides=".nextprevious.INextPreviousEnabled"
       />
@@ -125,16 +130,16 @@
   <adapter factory=".nextprevious.NextPreviousEnabled" />
 
   <!-- Constrain container allowed content types -->
   <plone:behavior
       name="plone.constraintypes"
       title="Folder Addable Constrains"
       description="Restrict the content types that can be added to folderish content"
-      provides="plone.base.interfaces.constrains.ISelectableConstrainTypes"
       factory=".constrains.ConstrainTypesBehavior"
+      provides="plone.base.interfaces.constrains.ISelectableConstrainTypes"
       for="plone.dexterity.interfaces.IDexterityContainer"
       />
 
   <!-- Short name -->
   <plone:behavior
       name="plone.shortname"
       title="Short name"
@@ -143,13 +148,15 @@
       provides=".id.IShortName"
       for="plone.dexterity.interfaces.IDexterityContent"
       />
 
   <!-- BBB -->
   <configure zcml:condition="installed plone.app.relationfield">
     <include package="plone.app.relationfield" />
-    <utility factory=".related.related_items_behavior_BBB"
-             provides="plone.behavior.interfaces.IBehavior"
-             name="plone.app.dexterity.behaviors.related.IRelatedItems"/>
+    <utility
+        factory=".related.related_items_behavior_BBB"
+        provides="plone.behavior.interfaces.IBehavior"
+        name="plone.app.dexterity.behaviors.related.IRelatedItems"
+        />
   </configure>
 
 </configure>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/constrains.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/constrains.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/discussion.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/discussion.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         SimpleTerm(value=False, title=_("No")),
     ]
 )
 
 
 @provider(IFormFieldProvider)
 class IAllowDiscussion(model.Schema):
-
     model.fieldset(
         "settings",
         label=_("Settings"),
         fields=["allow_discussion"],
     )
 
     allow_discussion = schema.Choice(
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/exclfromnav.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/exclfromnav.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/filename.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/filename.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/id.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/id.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from zope.interface import provider
 
 import transaction
 
 
 @provider(IFormFieldProvider)
 class IShortName(model.Schema):
-
     model.fieldset(
         "settings",
         label=_("Settings"),
         fields=["id"],
     )
 
     id = schema.ASCIILine(
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/metadata.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,40 +35,41 @@
 @provider(IContextAwareDefaultFactory)
 def default_language(context):
     # If we are adding a new object, context will be the folderish object where
     # this new content is being added
     language = None
 
     # Try to get the language from context or parent(s)
-    while not language and context is not None and not IPloneSiteRoot.providedBy(context):
-        language = getattr(context.aq_base, 'language', None)
+    while (
+        not language and context is not None and not IPloneSiteRoot.providedBy(context)
+    ):
+        language = getattr(context.aq_base, "language", None)
 
         if not language:
             # If we are here, it means we were editing an object that didn't
             # have its language set or that the container where we were adding
             # the new content didn't have a language set. So we check its
             # parent.
             context = context.__parent__
 
-    language_tool = getToolByName(getSite(), 'portal_languages')
+    language_tool = getToolByName(getSite(), "portal_languages")
     default_language = language_tool.getDefaultLanguage()
 
     if not language:
         language = default_language
 
     # Is the language supported/enabled at all?
     if language not in language_tool.getAvailableLanguages():
         language = default_language
 
     return language
 
 
 @provider(IFormFieldProvider)
 class IBasic(model.Schema):
-
     # default fieldset
     title = schema.TextLine(title=_("label_title", default="Title"), required=True)
 
     description = schema.Text(
         title=_("label_description", default="Summary"),
         description=_(
             "help_description", default="Used in item listings and search results."
@@ -83,15 +84,14 @@
     directives.omitted("title", "description")
     directives.no_omit(IEditForm, "title", "description")
     directives.no_omit(IAddForm, "title", "description")
 
 
 @provider(IFormFieldProvider)
 class ICategorization(model.Schema):
-
     # categorization fieldset
     model.fieldset(
         "categorization",
         label=_("label_schema_categorization", default="Categorization"),
         fields=["subjects", "language"],
     )
 
@@ -173,15 +173,14 @@
     directives.omitted("effective", "expires")
     directives.no_omit(IEditForm, "effective", "expires")
     directives.no_omit(IAddForm, "effective", "expires")
 
 
 @provider(IFormFieldProvider)
 class IOwnership(model.Schema):
-
     # ownership fieldset
     model.fieldset(
         "ownership",
         label=_("label_schema_ownership", default="Ownership"),
         fields=["creators", "contributors", "rights"],
     )
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/nextprevious.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/nextprevious.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/tests/test_contrains.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/test_contrains.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/tests/test_id.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/test_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from plone.testing.zope import Browser
 
 import transaction
 import unittest
 
 
 class TestShortNameBehavior(unittest.TestCase):
-
     layer = DEXTERITY_FUNCTIONAL_TESTING
 
     def setUp(self):
         # add IShortName behavior to Page
         behaviors = list(self.layer["portal"].portal_types.Document.behaviors)
         behaviors.append("plone.app.dexterity.behaviors.id.IShortName")
         self.layer["portal"].portal_types.Document.behaviors = tuple(behaviors)
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/behaviors/tests/test_metadata.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/add_type.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/add_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from plone.z3cform.layout import wrap_form
 from Products.CMFCore.utils import getToolByName
 from z3c.form import field
 from z3c.form import form
 
 
 class TypeAddForm(form.AddForm):
-
     label = _("Add Content Type")
     fields = field.Fields(ITypeSettings).select("title", "id", "description")
     id = "add-type-form"
     fti_id = None
 
     def create(self, data):
         id = data.pop("id")
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/behaviors.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/behaviors.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,14 @@
             if reg.name:
                 yield safe_text(reg.name)
             else:
                 yield name
 
 
 class TypeBehaviorsForm(form.EditForm):
-
     template = ViewPageTemplateFile("behaviors.pt")
     label = _("Behaviors")
     description = _("Select the behaviors to enable for this content type.")
     successMessage = _("Behaviors successfully updated.")
     noChangesMessage = _("No changes were made.")
     buttons = deepcopy(form.EditForm.buttons)
     buttons["apply"].title = _("Save")
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/clone_type.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/clone_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from plone.z3cform.layout import wrap_form
 from Products.CMFCore.utils import getToolByName
 from z3c.form import field
 from z3c.form import form
 
 
 class TypeCloneForm(form.AddForm):
-
     label = _("Clone Content Type")
     fields = field.Fields(ITypeSettings).select("title", "id")
     id = "clone-type-form"
 
     def create(self, data):
         type_id = data.pop("id")
         props = dict(self.context.fti.propertyItems())
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/configure.zcml` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/configure.zcml`

 * *Files 3% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:zcml="http://namespaces.zope.org/zcml"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
   <!-- Default view for Dexterity types in Plone  4 -->
   <browser:page
-      for="plone.dexterity.interfaces.IDexterityItem"
       name="view"
+      for="plone.dexterity.interfaces.IDexterityItem"
       class="plone.dexterity.browser.view.DefaultView"
       template="item.pt"
       permission="zope2.View"
       />
 
   <browser:page
-      for="plone.dexterity.interfaces.IDexterityContainer"
       name="view"
+      for="plone.dexterity.interfaces.IDexterityContainer"
       class="plone.dexterity.browser.view.DefaultView"
       template="container.pt"
       permission="zope2.View"
       />
 
   <browser:page
-      for="plone.dexterity.interfaces.IDexterityContainer"
       name="folder_listing"
+      for="plone.dexterity.interfaces.IDexterityContainer"
       class=".folder_listing.FolderView"
       template="folder_listing.pt"
       permission="zope2.View"
       />
 
   <browser:page
-      for="plone.base.interfaces.IPloneSiteRoot"
       name="folder_listing"
+      for="plone.base.interfaces.IPloneSiteRoot"
       class=".folder_listing.FolderView"
       template="folder_listing.pt"
       permission="zope2.View"
       />
 
   <!-- warning when editing default pages -->
   <browser:viewlet
       name="plone.app.dexterity.defaultpagewarning"
       view="plone.dexterity.interfaces.IDexterityEditForm"
+      manager="plone.app.layout.viewlets.interfaces.IGlobalStatusMessage"
       template="default_page_warning.pt"
       permission="cmf.ModifyPortalContent"
-      manager="plone.app.layout.viewlets.interfaces.IGlobalStatusMessage"
       />
 
   <!-- Control panel -->
 
   <browser:page
       name="dexterity-types"
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".types.TypesContext"
+      allowed_interface="OFS.interfaces.IItem"
       permission="plone.schemaeditor.ManageSchemata"
-      allowed_interface="OFS.interfaces.IItem" />
+      />
 
   <adapter
       factory=".types.TypeSettingsAdapter"
       provides="..interfaces.ITypeSettings"
       for="plone.dexterity.interfaces.IDexterityFTI"
       />
 
@@ -67,15 +69,16 @@
       for="plone.dexterity.interfaces.IDexterityFTI"
       />
 
   <browser:page
       name="edit"
       for="plone.app.dexterity.interfaces.ITypesContext"
       class=".types.TypesListingPage"
-      permission="plone.schemaeditor.ManageSchemata" />
+      permission="plone.schemaeditor.ManageSchemata"
+      />
 
   <browser:page
       name="add-type"
       for="plone.app.dexterity.interfaces.ITypesContext"
       class=".add_type.TypeAddFormPage"
       permission="plone.schemaeditor.ManageSchemata"
       />
@@ -87,33 +90,37 @@
       permission="plone.schemaeditor.ManageSchemata"
       />
 
   <browser:page
       name="overview"
       for="plone.app.dexterity.interfaces.ITypeSchemaContext"
       class=".overview.TypeOverviewPage"
-      permission="plone.schemaeditor.ManageSchemata" />
+      permission="plone.schemaeditor.ManageSchemata"
+      />
 
   <browser:page
       name="fields"
       for="plone.app.dexterity.interfaces.ITypeSchemaContext"
       class=".fields.TypeFieldsPage"
-      permission="plone.schemaeditor.ManageSchemata" />
+      permission="plone.schemaeditor.ManageSchemata"
+      />
 
   <browser:page
       name="behaviors"
       for="plone.app.dexterity.interfaces.ITypeSchemaContext"
       class=".behaviors.TypeBehaviorsPage"
-      permission="plone.schemaeditor.ManageSchemata" />
+      permission="plone.schemaeditor.ManageSchemata"
+      />
 
   <browser:page
       name="clone"
       for="plone.app.dexterity.interfaces.ITypeSchemaContext"
       class=".clone_type.TypeCloneFormPage"
-      permission="plone.schemaeditor.ManageSchemata" />
+      permission="plone.schemaeditor.ManageSchemata"
+      />
 
   <browser:page
       name="types-export"
       for="plone.app.dexterity.interfaces.ITypesContext"
       class=".export.TypesExport"
       permission="plone.schemaeditor.ManageSchemata"
       />
@@ -126,13 +133,13 @@
       />
 
   <configure zcml:condition="installed plone.resourceeditor">
     <browser:page
         name="modeleditor"
         for="plone.schemaeditor.interfaces.ISchemaContext"
         class=".modeleditor.ModelEditorView"
-        permission="plone.schemaeditor.ManageSchemata"
         template="modeleditor.pt"
+        permission="plone.schemaeditor.ManageSchemata"
         />
   </configure>
 
 </configure>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/container.pt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/container.pt`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,48 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
       lang="en"
       metal:use-macro="context/@@main_template/macros/master"
-      i18n:domain="plone">
-<body>
-
-<metal:main fill-slot="content-core">
-<metal:content-core define-macro="content-core">
-
-  <tal:block repeat="widget view/widgets/values|nothing">
-      <tal:block tal:condition="python:widget.__name__ not in ('IBasic.title', 'IBasic.description', 'title', 'description',)">
-          <tal:widget tal:replace="structure widget/@@ploneform-render-widget"/>
-      </tal:block>
-  </tal:block>
-
-  <fieldset tal:repeat="group view/groups|nothing"
-            tal:attributes="id python:''.join((group.prefix, 'groups.', group.__name__)).replace('.', '-')">
-      <legend tal:content="group/label" />
-      <tal:block tal:repeat="widget group/widgets/values">
-          <tal:widget tal:replace="structure widget/@@ploneform-render-widget"/>
-      </tal:block>
-  </fieldset>
-
-  <fieldset id="folder-listing">
-      <legend i18n:translate="" i18n:domain="plone">Contents</legend>
-      <tal:block define="view nocall:context/folder_listing; listing_macro view/macros/listing|view/index/macros/listing">
-          <metal:use_macro use-macro="listing_macro" />
-      </tal:block>
-  </fieldset>
+      xml:lang="en"
+      i18n:domain="plone"
+>
+  <body>
+
+    <metal:main fill-slot="content-core">
+      <metal:content-core define-macro="content-core">
+
+        <tal:block repeat="widget view/widgets/values|nothing">
+          <tal:block tal:condition="python:widget.__name__ not in ('IBasic.title', 'IBasic.description', 'title', 'description',)">
+            <tal:widget tal:replace="structure widget/@@ploneform-render-widget" />
+          </tal:block>
+        </tal:block>
+
+        <fieldset tal:repeat="group view/groups|nothing"
+                  tal:attributes="
+                    id python:''.join((group.prefix, 'groups.', group.__name__)).replace('.', '-');
+                  "
+        >
+          <legend tal:content="group/label"></legend>
+          <tal:block tal:repeat="widget group/widgets/values">
+            <tal:widget tal:replace="structure widget/@@ploneform-render-widget" />
+          </tal:block>
+        </fieldset>
+
+        <fieldset id="folder-listing">
+          <legend i18n:domain="plone"
+                  i18n:translate=""
+          >Contents</legend>
+          <tal:block define="
+                       view nocall:context/folder_listing;
+                       listing_macro view/macros/listing|view/index/macros/listing;
+                     ">
+            <metal:use_macro use-macro="listing_macro" />
+          </tal:block>
+        </fieldset>
 
-</metal:content-core>
-</metal:main>
+      </metal:content-core>
+    </metal:main>
 
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/default_page_warning.pt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/default_page_warning.pt`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-<tal:info
- xmlns:i18n="http://xml.zope.org/namespaces/i18n"
- i18n:domain="plone">
-<div class="alert alert-info" role="alert"
-    tal:condition="context/@@plone_context_state/is_default_page|nothing">
-  <span i18n:translate="label_edit_default_view_container">
+<tal:info xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+          i18n:domain="plone"
+>
+  <div class="alert alert-info"
+       role="alert"
+       tal:condition="context/@@plone_context_state/is_default_page|nothing"
+  >
+    <span i18n:translate="label_edit_default_view_container">
       You are editing the default view of a container. If you wanted to edit the container itself,
-     <a href=""
-        i18n:name="go_here"
-        i18n:translate="label_edit_default_view_container_go_here"
-        tal:attributes="href string:${context/aq_inner/aq_parent/absolute_url}/edit">go here</a>.
-  </span>
-</div>
+      <a href=""
+         tal:attributes="
+           href string:${context/aq_inner/aq_parent/absolute_url}/edit;
+         "
+         i18n:name="go_here"
+         i18n:translate="label_edit_default_view_container_go_here"
+      >go here</a>.
+    </span>
+  </div>
 </tal:info>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/export.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from zipfile import ZipFile
 
 import time
 
 
 class SelectiveZipExportContext(TarballExportContext):
     def __init__(self, tool, typelist, encoding=None, base_name="setup_tool"):
-
         BaseContext.__init__(self, tool, encoding)
 
         self.typelist = typelist
         self.filenames = ["types.xml"]
         for tn in typelist:
             self.filenames.append(f"types/{tn}.xml")
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/fields.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/fields.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/folder_listing.pt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/folder_listing.pt`

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,147 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-    xmlns:tal="http://xml.zope.org/namespaces/tal"
-    xmlns:metal="http://xml.zope.org/namespaces/metal"
-    xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    metal:use-macro="context/@@main_template/macros/master"
-    i18n:domain="plone">
-<body>
-
-<metal:content-core fill-slot="content-core">
-<metal:block define-macro="content-core">
-
-  <metal:listingmacro define-macro="listing">
-    <tal:results define="batch view/batch">
-      <tal:listing condition="batch">
-        <div class="entries" metal:define-slot="entries">
-          <tal:repeat repeat="item batch" metal:define-macro="entries">
-            <tal:block tal:define="obj item/getObject;
-                item_url item/getURL;
-                item_id item/getId;
-                item_title item/Title;
-                item_description item/Description;
-                item_type item/PortalType;
-                item_modified item/ModificationDate;
-                item_created item/CreationDate;
-                item_type_class python:'contenttype-' + view.normalizeString(item_type);
-                item_wf_state item/review_state;
-                item_wf_state_class python:'state-' + view.normalizeString(item_wf_state);
-                item_creator item/Creator;
-                item_link python:item_type in view.use_view_action and item_url+'/view' or item_url;
-                item_has_image python:item.getIcon">
-              <metal:block define-slot="entry">
-                <article class="entry">
-                  <header metal:define-macro="listitem">
-                    <span class="summary" tal:attributes="title item_type">
-                     <a tal:attributes="href item_link">
-                      <img class="image-tile"
-                             tal:condition="item_has_image"
-                             tal:attributes="src  string:$item_url/@@images/image/tile">
-                      </a>
-                      <a tal:attributes="href item_link;
-                                         class string:$item_type_class $item_wf_state_class url;
-                                         title item_type"
-                          tal:content="python: item_title or item_id">
+<html xmlns="http://www.w3.org/1999/xhtml"
+      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      metal:use-macro="context/@@main_template/macros/master"
+      xml:lang="en"
+      i18n:domain="plone"
+>
+  <body>
+
+    <metal:content-core fill-slot="content-core">
+      <metal:block define-macro="content-core">
+
+        <metal:listingmacro define-macro="listing">
+          <tal:results define="
+                         batch view/batch;
+                       ">
+            <tal:listing condition="batch">
+              <div class="entries"
+                   metal:define-slot="entries"
+              >
+                <tal:repeat metal:define-macro="entries"
+                            repeat="item batch"
+                >
+                  <tal:block tal:define="
+                               obj item/getObject;
+                               item_url item/getURL;
+                               item_id item/getId;
+                               item_title item/Title;
+                               item_description item/Description;
+                               item_type item/PortalType;
+                               item_modified item/ModificationDate;
+                               item_created item/CreationDate;
+                               item_type_class python:'contenttype-' + view.normalizeString(item_type);
+                               item_wf_state item/review_state;
+                               item_wf_state_class python:'state-' + view.normalizeString(item_wf_state);
+                               item_creator item/Creator;
+                               item_link python:item_type in view.use_view_action and item_url+'/view' or item_url;
+                               item_has_image python:item.getIcon;
+                             ">
+                    <metal:block define-slot="entry">
+                      <article class="entry">
+                        <header metal:define-macro="listitem">
+                          <span class="summary"
+                                tal:attributes="
+                                  title item_type;
+                                "
+                          >
+                            <a tal:attributes="
+                                 href item_link;
+                               ">
+                              <img class="image-tile"
+                                   tal:condition="item_has_image"
+                                   tal:attributes="
+                                     src  string:$item_url/@@images/image/tile;
+                                   "
+                              />
+                            </a>
+                            <a tal:content="python: item_title or item_id"
+                               tal:attributes="
+                                 href item_link;
+                                 class string:$item_type_class $item_wf_state_class url;
+                                 title item_type;
+                               "
+                            >
 
                              Item Title
-                      </a>
-                     </span>
-                    <metal:block metal:define-macro="document_byline">
-                      <div class="documentByLine">
-                        <tal:byline condition="view/show_about">
+                            </a>
+                          </span>
+                          <metal:block metal:define-macro="document_byline">
+                            <div class="documentByLine">
+                              <tal:byline condition="view/show_about">
                           &mdash;
-                          <tal:name tal:condition="item_creator"
-                              tal:define="author python:view.pas_member.info(item_creator);
-                                          creator_short_form author/username;
-                                          creator_long_form string:?author=${author/username};
-                                          creator_is_openid python:'/' in creator_short_form;
-                                          creator_id python:(creator_short_form, creator_long_form)[creator_is_openid];">
-                          <span i18n:translate="label_by_author">
+                                <tal:name tal:define="
+                                            author python:view.pas_member.info(item_creator);
+                                            creator_short_form author/username;
+                                            creator_long_form string:?author=${author/username};
+                                            creator_is_openid python:'/' in creator_short_form;
+                                            creator_id python:(creator_short_form, creator_long_form)[creator_is_openid];
+                                          "
+                                          tal:condition="item_creator"
+                                >
+                                  <span i18n:translate="label_by_author">
                             by
-                            <a tal:attributes="href string:${view/navigation_root_url}/author/${item_creator}"
-                                tal:content="author/name_or_id"
-                                tal:omit-tag="not:author"
-                                i18n:name="author">
+                                    <a tal:content="author/name_or_id"
+                                       tal:omit-tag="not:author"
+                                       tal:attributes="
+                                         href string:${view/navigation_root_url}/author/${item_creator};
+                                       "
+                                       i18n:name="author"
+                                    >
                               Bob Dobalina
-                            </a>
-                          </span>
-                          </tal:name>
+                                    </a>
+                                  </span>
+                                </tal:name>
 
-                          <tal:modified>
+                                <tal:modified>
                             &mdash;
-                            <tal:mod i18n:translate="box_last_modified">last modified</tal:mod>
-                            <span tal:replace="python:view.toLocalizedTime(item_modified,long_format=1)">
+                                  <tal:mod i18n:translate="box_last_modified">last modified</tal:mod>
+                                  <span tal:replace="python:view.toLocalizedTime(item_modified,long_format=1)">
                               August 16, 2001 at 23:35:59
-                            </span>
-                          </tal:modified>
+                                  </span>
+                                </tal:modified>
 
-                          <metal:description define-slot="description_slot">
-                            <tal:comment replace="nothing">
+                                <metal:description define-slot="description_slot">
+                                  <tal:comment replace="nothing">
                               Place custom listing info for custom types here
-                            </tal:comment>
-                          </metal:description>
-                        </tal:byline>
-                      </div>
-                    </metal:block>
-                  </header>
-                  <p class="description discreet"
-                      tal:condition="item_description"
-                      tal:content="item_description">
+                                  </tal:comment>
+                                </metal:description>
+                              </tal:byline>
+                            </div>
+                          </metal:block>
+                        </header>
+                        <p class="description discreet"
+                           tal:condition="item_description"
+                           tal:content="item_description"
+                        >
                     description
-                  </p>
-                </article>
-              </metal:block>
-            </tal:block>
-          </tal:repeat>
-        </div>
-
-        <div metal:use-macro="context/batch_macros/macros/navigation" />
-
-      </tal:listing>
-
-      <metal:empty metal:define-slot="no_items_in_listing">
-        <p class="discreet"
-            tal:condition="not: view/batch"
-            tal:content="view/no_items_message">
+                        </p>
+                      </article>
+                    </metal:block>
+                  </tal:block>
+                </tal:repeat>
+              </div>
+
+              <div metal:use-macro="context/batch_macros/macros/navigation"></div>
+
+            </tal:listing>
+
+            <metal:empty metal:define-slot="no_items_in_listing">
+              <p class="discreet"
+                 tal:condition="not: view/batch"
+                 tal:content="view/no_items_message"
+              >
           There are currently no items in this folder.
-        </p>
-      </metal:empty>
+              </p>
+            </metal:empty>
 
-    </tal:results>
-  </metal:listingmacro>
+          </tal:results>
+        </metal:listingmacro>
 
-</metal:block>
-</metal:content-core>
+      </metal:block>
+    </metal:content-core>
 
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/folder_listing.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/folder_listing.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/import_types.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/import_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,14 @@
     )
 
     def __init__(self, profile_file):
         self.profile_file = profile_file
 
 
 class TypeProfileImportForm(form.AddForm):
-
     label = _("Import Content Types")
     description = _(
         "You may import types by uploading a zip archive containing type "
         "profiles. The import archive should contain a types.xml file and a "
         "types directory containing one or more Dexterity type information "
         "files. For a sample, create a content type and export it from the "
         "Dexterity Content Types page."
@@ -141,15 +140,14 @@
     def __init__(self, tool, archive_bits, encoding=None, should_purge=False):
         super().__init__(tool, encoding)
         self._archive = ZipFile(archive_bits, "r")
         self._should_purge = bool(should_purge)
         self.name_list = self._archive.namelist()
 
     def readDataFile(self, filename, subdir=None):
-
         if subdir is not None:
             filename = "/".join((subdir, filename))
 
         try:
             file = self._archive.open(filename, "r")
         except KeyError:
             return None
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/item.pt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/item.pt`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,36 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
       lang="en"
       metal:use-macro="context/@@main_template/macros/master"
-      i18n:domain="plone">
-<body>
+      xml:lang="en"
+      i18n:domain="plone"
+>
+  <body>
 
-<metal:main fill-slot="content-core">
-<metal:content-core define-macro="content-core">
+    <metal:main fill-slot="content-core">
+      <metal:content-core define-macro="content-core">
 
-  <tal:block repeat="widget view/widgets/values|nothing">
-    <tal:block tal:condition="python:widget.__name__ not in ('IBasic.title', 'IBasic.description', 'title', 'description',)">
-      <tal:widget tal:replace="structure widget/@@ploneform-render-widget"/>
-    </tal:block>
-  </tal:block>
+        <tal:block repeat="widget view/widgets/values|nothing">
+          <tal:block tal:condition="python:widget.__name__ not in ('IBasic.title', 'IBasic.description', 'title', 'description',)">
+            <tal:widget tal:replace="structure widget/@@ploneform-render-widget" />
+          </tal:block>
+        </tal:block>
 
-  <fieldset tal:repeat="group view/groups|nothing"
-            tal:attributes="id python:''.join((group.prefix, 'groups.', group.__name__)).replace('.', '-')">
-    <legend tal:content="group/label" />
-    <tal:block tal:repeat="widget group/widgets/values|nothing">
-      <tal:widget tal:replace="structure widget/@@ploneform-render-widget"/>
-    </tal:block>
-  </fieldset>
+        <fieldset tal:repeat="group view/groups|nothing"
+                  tal:attributes="
+                    id python:''.join((group.prefix, 'groups.', group.__name__)).replace('.', '-');
+                  "
+        >
+          <legend tal:content="group/label"></legend>
+          <tal:block tal:repeat="widget group/widgets/values|nothing">
+            <tal:widget tal:replace="structure widget/@@ploneform-render-widget" />
+          </tal:block>
+        </fieldset>
 
-</metal:content-core>
-</metal:main>
+      </metal:content-core>
+    </metal:main>
 
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/modeleditor.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/modeleditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/overview.pt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/overview.pt`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,54 @@
-<tal:form metal:use-macro="context/@@ploneform-macros/titlelessform"
-    xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    i18n:domain="plone">
-<tal:fields metal:fill-slot="fields">
-  <tal:field tal:replace="structure view/widgets/title/@@ploneform-render-widget" />
-  <tal:field tal:replace="structure view/widgets/description/@@ploneform-render-widget" />
+<tal:form xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+          metal:use-macro="context/@@ploneform-macros/titlelessform"
+          i18n:domain="plone"
+>
+  <tal:fields metal:fill-slot="fields">
+    <tal:field tal:replace="structure view/widgets/title/@@ploneform-render-widget" />
+    <tal:field tal:replace="structure view/widgets/description/@@ploneform-render-widget" />
 
-  <fieldset tal:condition="python:'filter_content_types' in view.fields">
-    <legend i18n:translate="label_contained_items">Contained items</legend>
-    <tal:block tal:define="context nocall:view/widgets/filter_content_types;
-                           value context/value">
-      <tal:fieldwrapper metal:use-macro="context/@@ploneform-render-widget/widget-wrapper">
-      <tal:field metal:fill-slot="widget">
-        <label>
-          <input type="radio" value="none"
-               tal:attributes="name context/name;
-                               checked python:'checked' if 'none' in value else None"/>
-          <tal:block i18n:translate="label_no_content_types">No content types</tal:block>
-        </label><br />
-        <label>
-          <input type="radio" value="all"
-                 tal:attributes="name context/name;
-                               checked python:'checked' if 'all' in value else None"/>
-          <tal:block i18n:translate="label_all_content_types">All content types</tal:block>
-        </label><br />
-        <label>
-          <input type="radio" value="some"
-                 tal:attributes="name context/name;
-                               checked python:'checked' if 'some' in value else None"/>
-          <tal:block i18n:translate="label_some_content_types">Some content types:</tal:block>
-          <tal:field tal:replace="structure view/widgets/allowed_content_types/render" />
-        </label>
-      </tal:field>
-      </tal:fieldwrapper>
-    </tal:block>
-  </fieldset>
+    <fieldset tal:condition="python:'filter_content_types' in view.fields">
+      <legend i18n:translate="label_contained_items">Contained items</legend>
+      <tal:block tal:define="
+                   context nocall:view/widgets/filter_content_types;
+                   value context/value;
+                 ">
+        <tal:fieldwrapper metal:use-macro="context/@@ploneform-render-widget/widget-wrapper">
+          <tal:field metal:fill-slot="widget">
+            <label>
+              <input type="radio"
+                     value="none"
+                     tal:attributes="
+                       name context/name;
+                       checked python:'checked' if 'none' in value else None;
+                     "
+              />
+              <tal:block i18n:translate="label_no_content_types">No content types</tal:block>
+            </label><br />
+            <label>
+              <input type="radio"
+                     value="all"
+                     tal:attributes="
+                       name context/name;
+                       checked python:'checked' if 'all' in value else None;
+                     "
+              />
+              <tal:block i18n:translate="label_all_content_types">All content types</tal:block>
+            </label><br />
+            <label>
+              <input type="radio"
+                     value="some"
+                     tal:attributes="
+                       name context/name;
+                       checked python:'checked' if 'some' in value else None;
+                     "
+              />
+              <tal:block i18n:translate="label_some_content_types">Some content types:</tal:block>
+              <tal:field tal:replace="structure view/widgets/allowed_content_types/render" />
+            </label>
+          </tal:field>
+        </tal:fieldwrapper>
+      </tal:block>
+    </fieldset>
 
-</tal:fields>
+  </tal:fields>
 </tal:form>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/overview.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/overview.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/tabbed_forms.pt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/tabbed_forms.pt`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
+      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
       metal:use-macro="here/prefs_main_template/macros/master"
-      i18n:domain="plone.z3cform">
-<body>
-<metal:slot metal:fill-slot="prefs_configlet_main">
+      i18n:domain="plone.z3cform"
+>
+  <body>
+    <metal:slot metal:fill-slot="prefs_configlet_main">
 
-  <header class="mb-4"> 
+      <header class="mb-4">
 
-    <div metal:use-macro="context/global_statusmessage/macros/portal_message">
+        <div metal:use-macro="context/global_statusmessage/macros/portal_message">
       Portal status message
-    </div>
+        </div>
 
-    <h1 class="documentFirstHeading"><tal:block tal:content="context/Title"/> (<tal:block tal:content="python:context.__name__" />)</h1>
+        <h1 class="documentFirstHeading"><tal:block tal:content="context/Title" />
+          (<tal:block tal:content="python:context.__name__" />)</h1>
 
-    <ul class="nav nav-tabs">
-      <li class="nav-item" tal:repeat="tab view/tabs">
-        <a class="nav-link"
-            tal:attributes="href python:context.absolute_url() + '/' + tab[1];
-                            class python: 'nav-link ' + ('active' if tab[0] == view.label else '')"
-            tal:content="python:tab[0]" />
-      </li>
-    </ul>
-  </header>
-  <div id="content-core">
-      <tal:block tal:replace="structure view/contents|view/render"/>
-  </div>
+        <ul class="nav nav-tabs">
+          <li class="nav-item"
+              tal:repeat="tab view/tabs"
+          >
+            <a class="nav-link"
+               tal:content="python:tab[0]"
+               tal:attributes="
+                 href python:context.absolute_url() + '/' + tab[1];
+                 class python: 'nav-link ' + ('active' if tab[0] == view.label else '');
+               "
+            ></a>
+          </li>
+        </ul>
+      </header>
+      <div id="content-core">
+        <tal:block tal:replace="structure view/contents|view/render" />
+      </div>
 
-</metal:slot>
-</body>
+    </metal:slot>
+  </body>
 </html>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/types.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,14 @@
 TypesListingPage = layout.wrap_form(
     TypesListing, __wrapper_class=TypesEditFormWrapper, label=_("Content Types")
 )
 
 
 @implementer(ITypeSchemaContext)
 class TypeSchemaContext(SchemaContext):
-
     fti = None
     schemaName = ""
     schemaEditorView = "fields"
     allowedFields = ALLOWED_FIELDS
 
     def browserDefault(self, request):
         return self, ("@@overview",)
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/types_listing.pt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/types_listing.pt`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,48 @@
-<tal:root
-    i18n:domain="plone">
+<tal:root i18n:domain="plone">
 
-  <div class="alert alert-info" role="alert"
-       tal:condition="view/status">
+  <div class="alert alert-info"
+       role="alert"
+       tal:condition="view/status"
+  >
     <span tal:content="view/status">
       Status
     </span>
   </div>
 
   <p class="crud-description documentDescription"
-      tal:condition="view/description"
-      tal:content="structure view/description">
+     tal:condition="view/description"
+     tal:content="structure view/description"
+  >
   </p>
   <header class="mb-4">
     <a class="pat-plone-modal"
-        href="${context/absolute_url}/@@add-type">
-      <button class="btn btn-primary" i18n:translate="">Add New Content Type&hellip;</button>
+       href="${context/absolute_url}/@@add-type"
+    >
+      <button class="btn btn-primary"
+              i18n:translate=""
+      >Add New Content Type&hellip;</button>
     </a>
 
     <a class="pat-plone-modal"
-        href="${context/absolute_url}/@@import-types">
-      <button class="btn btn-primary" i18n:translate="">Import Type Profiles&hellip;</button>
+       href="${context/absolute_url}/@@import-types"
+    >
+      <button class="btn btn-primary"
+              i18n:translate=""
+      >Import Type Profiles&hellip;</button>
     </a>
   </header>
 
   <div class="crud-form"
-      tal:repeat="form view/subforms"
-      tal:content="structure form/render">
+       tal:repeat="form view/subforms"
+       tal:content="structure form/render"
+  >
   </div>
 
-  <div class="action" tal:repeat="action view/actions/values">
-    <input type="submit" tal:replace="structure action/render" />
+  <div class="action"
+       tal:repeat="action view/actions/values"
+  >
+    <input type="submit"
+           tal:replace="structure action/render"
+    />
   </div>
 </tal:root>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/types_listing_row.pt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/types_listing_row.pt`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,50 @@
-<tal:block define="tups view/getCombinedWidgets;
-                   portal context/@@plone_portal_state/portal;
-                   layout portal/@@plone_layout;
-                   niceTitles view/getNiceTitles"
-           repeat="tup tups">
-
-  <td tal:define="error python:tup[0].error;
-                  idx repeat/tup/index;
-                  normalize nocall: context/@@plone/normalizeString;"
-      tal:attributes="class python:'field' + (error and ' error' or '') + (tup[0].__name__ == 'view_item_count' and ' count' or '')">
+<tal:block define="
+             tups view/getCombinedWidgets;
+             portal context/@@plone_portal_state/portal;
+             layout portal/@@plone_layout;
+             niceTitles view/getNiceTitles;
+           "
+           repeat="tup tups"
+>
+
+  <td tal:define="
+        error python:tup[0].error;
+        idx repeat/tup/index;
+        normalize nocall: context/@@plone/normalizeString;
+      "
+      tal:attributes="
+        class python:'field' + (error and ' error' or '') + (tup[0].__name__ == 'view_item_count' and ' count' or '');
+      "
+  >
     <tal:block repeat="widget tup">
 
 
 
-    <a href=""
-       tal:define="link python:view.context.context.link(view.getContent(), widget.field.__name__);
-                   item_type_class python:'contenttype-' + normalize(view.getContent().id)"
-       tal:omit-tag="python:widget.mode == 'input' or link is None"
-       tal:attributes="href link;
-                       class string:$item_type_class">
-
-      <span class="error" tal:omit-tag="not:error">
-        <div tal:condition="error" tal:replace="structure error/render" />
-        <input type="text" tal:replace="structure widget/render" />
-      </span>
+      <a href=""
+         tal:define="
+           link python:view.context.context.link(view.getContent(), widget.field.__name__);
+           item_type_class python:'contenttype-' + normalize(view.getContent().id);
+         "
+         tal:omit-tag="python:widget.mode == 'input' or link is None"
+         tal:attributes="
+           href link;
+           class string:$item_type_class;
+         "
+      >
+
+        <span class="error"
+              tal:omit-tag="not:error"
+        >
+          <div tal:condition="error"
+               tal:replace="structure error/render"
+          ></div>
+          <input type="text"
+                 tal:replace="structure widget/render"
+          />
+        </span>
 
-    </a>
+      </a>
     </tal:block>
 
   </td>
 </tal:block>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/browser/typesformwrapper.pt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/typesformwrapper.pt`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
       lang="en"
       metal:use-macro="here/prefs_main_template/macros/master"
-      i18n:domain="plone">
-<body>
-<metal:main fill-slot="prefs_configlet_main">
-<tal:main-macro metal:define-macro="main">
-  <h1 class="documentFirstHeading" tal:content="view/label">Title</h1>
-  <div id="skel-contents">
-    <span tal:replace="structure view/contents" />
-  </div>
-</tal:main-macro>
-</metal:main>
-</html>
+      xml:lang="en"
+      i18n:domain="plone"
+>
+  <body>
+    <metal:main fill-slot="prefs_configlet_main">
+      <tal:main-macro metal:define-macro="main">
+        <h1 class="documentFirstHeading"
+            tal:content="view/label"
+        >Title</h1>
+        <div id="skel-contents">
+          <span tal:replace="structure view/contents"></span>
+        </div>
+      </tal:main-macro>
+    </metal:main>
+  </body></html>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/configure.zcml` & `plone.app.dexterity-3.0.5/plone/app/dexterity/configure.zcml`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:five="http://namespaces.zope.org/five"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
-    xmlns:zcml="http://namespaces.zope.org/zcml"
     xmlns:i18n="http://namespaces.zope.org/i18n"
-    i18n_domain="plone">
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    i18n_domain="plone"
+    >
 
-  <include package="plone.app.imaging" zcml:condition="installed plone.app.imaging"/>
   <include package="plone.app.vocabularies" />
   <include package="plone.app.z3cform" />
   <include package="plone.app.textfield" />
   <include package="plone.app.uuid" />
   <include package="plone.formwidget.namedfile" />
   <include package="plone.schemaeditor" />
-  <include package="plone.directives.dexterity" zcml:condition="installed plone.directives.dexterity" />
+  <include
+      package="plone.directives.dexterity"
+      zcml:condition="installed plone.directives.dexterity"
+      />
   <include package="plone.dexterity" />
   <include package="plone.behavior" />
 
   <genericsetup:registerProfile
       name="default"
       title="Dexterity Content Types"
       description="Configures various components needed for full Dexterity support."
-      directory="profiles/default"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       for="plone.base.interfaces.IPloneSiteRoot"
+      directory="profiles/default"
       />
 
   <genericsetup:registerProfile
       name="testing"
       title="Dexterity Content Types"
       description="Adds Dexterity-based Folder and Document types for testing."
-      directory="profiles/testing"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       for="plone.base.interfaces.ITestCasePloneSiteRoot"
+      directory="profiles/testing"
       />
 
   <include package=".browser" />
   <include package=".behaviors" />
   <include package=".textindexer" />
   <include package=".upgrades" />
 
@@ -59,11 +62,13 @@
 
   <adapter factory=".interfaces.TypeIdValidator" />
   <adapter factory=".interfaces.TypeTitleValidator" />
 
   <adapter factory=".factories.DXFileFactory" />
   <adapter factory=".permissions.DXFieldPermissionChecker" />
   <adapter factory=".permissions.GenericFormFieldPermissionChecker" />
-  <adapter factory=".permissions.GenericFormFieldPermissionChecker"
-           for="plone.z3cform.interfaces.IFormWrapper" />
+  <adapter
+      factory=".permissions.GenericFormFieldPermissionChecker"
+      for="plone.z3cform.interfaces.IFormWrapper"
+      />
 
 </configure>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/events.zcml` & `plone.app.dexterity-3.0.5/plone/app/dexterity/events.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
   <!-- Register schema/field modify handlers -->
   <subscriber
       for="plone.app.dexterity.interfaces.ITypeSchemaContext
            plone.schemaeditor.interfaces.ISchemaModifiedEvent"
       handler=".serialize.serializeSchemaContext"
       />
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/factories.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         upload_lock.acquire()
         try:
             newid = chooser.chooseName(name, self.context.aq_parent)
             # Try to determine which kind of NamedBlob we need
             # This will suffice for standard p.a.contenttypes File/Image
             # and any other custom type that would have 'File' or 'Image' in
             # its type name
-            # XXX heuristics are harmful behavior, here a better implemenation
+            # XXX heuristics are harmful behavior, here a better implementation
             #     is needed
             filename = name
             if "Image" in type_:
                 image = NamedBlobImage(
                     data=data, filename=filename, contentType=content_type
                 )
                 obj = createContentInContainer(
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/interfaces.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
         value_type=schema.Choice(
             vocabulary="plone.app.vocabularies.ReallyUserFriendlyTypes", required=False
         ),
     )
 
 
 class ITypeStats(Interface):
-
     item_count = schema.Int(
         title=_("# of items"),
     )
 
 
 class TypeIdValidator(validator.SimpleFieldValidator):
     def validate(self, value):
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/permissions.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/permissions.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/testing/types/Document.xml` & `plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types/Folder.xml`

 * *Files 8% similar despite different names*

#### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/testing/types/Document.xml` & `plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types/Folder.xml`

```diff
@@ -1,38 +1,43 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="Document" meta_type="Dexterity FTI" i18n:domain="plone">
-  <property name="title" i18n:translate="">Page</property>
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="Folder" i18n:domain="plone">
+  <property name="title" i18n:translate="">Folder</property>
   <property name="description" i18n:translate=""/>
   <property name="icon_expr"/>
-  <property name="factory">Document</property>
-  <property name="add_view_expr">string:${folder_url}/++add++Document</property>
+  <property name="factory">Folder</property>
+  <property name="add_view_expr">string:${folder_url}/++add++Folder</property>
   <property name="link_target"/>
+  <property name="immediate_view">view</property>
   <property name="global_allow">True</property>
-  <property name="filter_content_types">True</property>
+  <property name="filter_content_types">False</property>
   <property name="allowed_content_types"/>
   <property name="allow_discussion">False</property>
-  <property name="default_view">view</property>
-  <property name="immediate_view"/>
+  <property name="default_view">folder_listing</property>
   <property name="view_methods">
-    <element value="view"/>
+    <element value="folder_summary_view"/>
+    <element value="folder_full_view"/>
+    <element value="folder_tabular_view"/>
+    <element value="atct_album_view"/>
+    <element value="folder_listing"/>
   </property>
   <property name="default_view_fallback">False</property>
   <property name="add_permission">cmf.AddPortalContent</property>
-  <property name="klass">plone.dexterity.content.Item</property>
+  <property name="klass">plone.dexterity.content.Container</property>
   <property name="behaviors">
+    <element value="plone.dublincore"/>
+    <element value="plone.excludefromnavigation"/>
     <element value="plone.namefromtitle"/>
     <element value="plone.allowdiscussion"/>
-    <element value="plone.excludefromnavigation"/>
-    <element value="plone.dublincore"/>
+    <element value="plone.nextprevioustoggle"/>
   </property>
   <property name="schema">zope.interface.Interface</property>
   <alias from="(Default)" to="(dynamic view)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
-  <action title="View" action_id="view" category="object" condition_expr="" icon_expr="" link_target="" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
+  <action action_id="view" category="object" condition_expr="" icon_expr="" link_target="" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action title="Edit" action_id="edit" category="object" condition_expr="" icon_expr="" link_target="" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
+  <action action_id="edit" category="object" condition_expr="" icon_expr="" link_target="" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/testing/types/Folder.xml` & `plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types/Document.xml`

 * *Files 20% similar despite different names*

#### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/profiles/testing/types/Folder.xml` & `plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types/Document.xml`

```diff
@@ -1,43 +1,38 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="Folder" meta_type="Dexterity FTI" i18n:domain="plone">
-  <property name="title" i18n:translate="">Folder</property>
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="Document" i18n:domain="plone">
+  <property name="title" i18n:translate="">Page</property>
   <property name="description" i18n:translate=""/>
   <property name="icon_expr"/>
-  <property name="factory">Folder</property>
-  <property name="add_view_expr">string:${folder_url}/++add++Folder</property>
+  <property name="factory">Document</property>
+  <property name="add_view_expr">string:${folder_url}/++add++Document</property>
   <property name="link_target"/>
-  <property name="immediate_view">view</property>
   <property name="global_allow">True</property>
-  <property name="filter_content_types">False</property>
+  <property name="filter_content_types">True</property>
   <property name="allowed_content_types"/>
   <property name="allow_discussion">False</property>
-  <property name="default_view">folder_listing</property>
+  <property name="default_view">view</property>
+  <property name="immediate_view"/>
   <property name="view_methods">
-    <element value="folder_summary_view"/>
-    <element value="folder_full_view"/>
-    <element value="folder_tabular_view"/>
-    <element value="atct_album_view"/>
-    <element value="folder_listing"/>
+    <element value="view"/>
   </property>
   <property name="default_view_fallback">False</property>
   <property name="add_permission">cmf.AddPortalContent</property>
-  <property name="klass">plone.dexterity.content.Container</property>
+  <property name="klass">plone.dexterity.content.Item</property>
   <property name="behaviors">
-    <element value="plone.dublincore"/>
-    <element value="plone.excludefromnavigation"/>
     <element value="plone.namefromtitle"/>
     <element value="plone.allowdiscussion"/>
-    <element value="plone.nextprevioustoggle"/>
+    <element value="plone.excludefromnavigation"/>
+    <element value="plone.dublincore"/>
   </property>
   <property name="schema">zope.interface.Interface</property>
   <alias from="(Default)" to="(dynamic view)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
-  <action title="View" action_id="view" category="object" condition_expr="" icon_expr="" link_target="" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
+  <action action_id="view" category="object" condition_expr="" icon_expr="" link_target="" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action title="Edit" action_id="edit" category="object" condition_expr="" icon_expr="" link_target="" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
+  <action action_id="edit" category="object" condition_expr="" icon_expr="" link_target="" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/serialize.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/serialize.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/testing.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/discussion.txt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/discussion.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/editing.rst` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/editing.rst`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
   >>> browser.url
   'http://nohost/plone/dexterity-types/plonista/@@modeleditor'
 
 Go there and find the XML model source in a textarea, ready to be edited
 (with JavaScript enabled, this should show pat-code-editor instead of the textarea)::
 
   >>> browser.open('http://nohost/plone/dexterity-types/plonista/@@modeleditor')
-  >>> '<textarea name="source"' in browser.contents
+  >>> '<textarea class="modeleditor__source pat-code-editor language-xml" name="source">' in browser.contents
   True
 
   >>> '&lt;schema&gt;' in browser.contents
   True
 
   >>> model_source = portal.portal_types.plonista.model_source
   >>> escaped_model_source = escape(model_source, quote=False)
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/filename.txt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/filename.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/import/dexterity_export.zip` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/import/dexterity_export.zip`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/metadata.txt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/metadata.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/namefromtitle.txt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/namefromtitle.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/nextprevious.txt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/nextprevious.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/robot/test_types.robot` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/robot/test_types.robot`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/schema_events.txt` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/schema_events.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_constrains.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_constrains.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     fti.klass = "plone.dexterity.content.Item"
     fti.filter_content_types = False
     fti.behaviors = "plone.basic"
     return fti
 
 
 class DocumentIntegrationTest(unittest.TestCase):
-
     layer = DEXTERITY_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.request["ACTUAL_URL"] = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
@@ -338,15 +337,14 @@
         good.allowed_types = ["1"]
         good.secondary_types = []
         self.assertTrue(IConstrainForm.validateInvariants(good) is None)
         self.assertRaises(Invalid, IConstrainForm.validateInvariants, bad)
 
 
 class FolderConstrainViewFunctionalText(unittest.TestCase):
-
     layer = DEXTERITY_FUNCTIONAL_TESTING
 
     def setUp(self):
         app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
@@ -418,15 +416,14 @@
         ctrl("form.widgets.secondary_types:list").value = ["Document", "Folder"]
         self.browser.getControl("Save").click()
         self.assertEqual(constraint_before, aspect.getConstrainTypesMode())
         self.assertTrue("There were some errors" in self.browser.contents)
 
 
 class ConstrainControlFunctionalText(unittest.TestCase):
-
     layer = DEXTERITY_FUNCTIONAL_TESTING
 
     def setUp(self):
         app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
@@ -458,28 +455,28 @@
         url = "/dexterity-types/item/@@overview"
         self.browser.open(self.portal_url + url)
         self.assertFalse("Filter Contained Types" in self.browser.contents)
         self.assertFalse("No content types" in self.browser.contents)
 
     def test_overview_folder_item_view(self):
         # First we access folder content types and check
-        # that is possible to fiter content types (as it is a container)
+        # that is possible to filter content types (as it is a container)
         url = "/dexterity-types/folder/@@overview"
         self.browser.open(self.portal_url + url)
         self.assertTrue("Filter Contained Types" in self.browser.contents)
         self.assertTrue("No content types" in self.browser.contents)
 
         # Then we access item content types and check
-        # that is NOT possible to fiter content types
+        # that is NOT possible to filter content types
         url = "/dexterity-types/item/@@overview"
         self.browser.open(self.portal_url + url)
         self.assertFalse("Filter Contained Types" in self.browser.contents)
         self.assertFalse("No content types" in self.browser.contents)
 
-        # Acessing folder content types again
+        # Accessing folder content types again
         # and it should be possible to filter content types
         url = "/dexterity-types/folder/@@overview"
         self.browser.open(self.portal_url + url)
         self.assertTrue("Filter Contained Types" in self.browser.contents)
         self.assertTrue("No content types" in self.browser.contents)
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_doctests.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_doctests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from plone.app.dexterity.testing import DEXTERITY_FUNCTIONAL_TESTING
 from plone.testing import layered
 
 import doctest
-import re
 import unittest
 
 
 tests = (
     "discussion.txt",
     "editing.rst",
     "namefromtitle.txt",
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_export.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_import.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_nextprevious.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_nextprevious.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_permissions.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
             IPloneFormLayer,
         ),
         provided=IFieldWidget,
     )
 
 
 class DexterityVocabularyPermissionTests(unittest.TestCase):
-
     layer = PAZ3CForm_INTEGRATION_TESTING
 
     def setUp(self):
         self.request = TestRequest(environ={"HTTP_ACCEPT_LANGUAGE": "en"})
         setRequest(self.request)
         self.portal = self.layer["portal"]
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_robot.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/tests/test_upgrades.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_upgrades.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from plone.app.dexterity.testing import DEXTERITY_INTEGRATION_TESTING
 
 import unittest
 
 
 class TestUpgrades(unittest.TestCase):
-
     layer = DEXTERITY_INTEGRATION_TESTING
 
     def test_add_missing_uuids(self):
         from plone.app.dexterity.upgrades.to2001 import add_missing_uuids
         from plone.dexterity.fti import DexterityFTI
         from plone.dexterity.utils import createContentInContainer
         from plone.uuid.interfaces import ATTRIBUTE_NAME
@@ -35,28 +34,7 @@
         )[0]
         self.assertTrue(b.UID == uuid)
 
         # make sure running the upgrade again doesn't change the UUID
         add_missing_uuids(self.layer["portal"])
         uuid2 = IUUID(page, None)
         self.assertEqual(uuid2, uuid, "Upgrade changes existing uuids.")
-
-    def test_upgrade_2003(self):
-        from plone.app.dexterity.upgrades.to2003 import fix_installed_products
-        from Products.CMFCore.utils import getToolByName
-
-        try:
-            from Products.CMFQuickInstallerTool.InstalledProduct import InstalledProduct
-        except ImportError:
-            # nothing to test
-            return
-        qi = getToolByName(self.layer["portal"], "portal_quickinstaller", None)
-        if qi is None:
-            # nothing to test
-            return
-        ip = InstalledProduct("foo")
-        ip.utilities = [("zope.intid.interfaces.IIntIds", "")]
-        qi._setObject("foo", ip)
-
-        fix_installed_products(self.layer["portal"])
-
-        self.assertEqual([], ip.utilities)
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/__init__.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/configure.zcml` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/configure.zcml`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,59 @@
-<configure xmlns="http://namespaces.zope.org/zope"
-           xmlns:i18n="http://namespaces.zope.org/i18n"
-           xmlns:plone="http://namespaces.plone.org/plone"
-           xmlns:zcml="http://namespaces.zope.org/zcml"
-           i18n_domain="plone.app.dexterity.textindexer">
-
-    <!-- marker behavior for enabling indexer -->
-    <plone:behavior
-          title="Full-Text Indexing"
-          name="plone.textindexer"
-          description="Enables the enhanced full-text indexing for a content type ('plone.textindexer'). If a field is marked 'searchable', its content gets added to the 'SearchableText' index in the catalog."
-          provides="plone.app.dexterity.textindexer.behavior.IDexterityTextIndexer"
-          />
-
-    <utility
-        factory=".supermodel.IndexerSchema"
-        name="plone.textindexer.indexer"
-        />
-
-    <adapter
-        factory="plone.app.dexterity.textindexer.indexer.dynamic_searchable_text_indexer"
-        name="SearchableText" />
-
-    <!-- field converters -->
-    <adapter
-        factory="plone.app.dexterity.textindexer.converters.DefaultDexterityTextIndexFieldConverter"
-        />
-
-    <adapter
-        zcml:condition="installed plone.namedfile"
-        factory="plone.app.dexterity.textindexer.converters.NamedfileFieldConverter"
-        />
-
-    <adapter
-        zcml:condition="installed plone.app.textfield"
-        factory="plone.app.dexterity.textindexer.converters.DexterityRichTextIndexFieldConverter"
-        />
-
-    <adapter
-        factory="plone.app.dexterity.textindexer.converters.IntFieldConverter"
-        />
-
-    <adapter
-        factory="plone.app.dexterity.textindexer.converters.TupleFieldConverter"
-        />
-
-    <!-- plone.schemaeditor adapter -->
-    <adapter
-        provides="plone.schemaeditor.interfaces.IFieldEditorExtender"
-        for="plone.schemaeditor.interfaces.ISchemaContext
-             zope.schema.interfaces.IField"
-        name="plone.schemaeditor.searchabletext"
-        factory=".schemaeditor.get_searchabletext_schema"
-        />
-
-    <adapter
-        provides=".schemaeditor.ISearchableTextField"
-        for="zope.schema.interfaces.IField"
-        factory=".schemaeditor.SearchableTextField"
-        />
+<configure
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:i18n="http://namespaces.zope.org/i18n"
+    xmlns:plone="http://namespaces.plone.org/plone"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    i18n_domain="plone.app.dexterity.textindexer"
+    >
+
+  <!-- marker behavior for enabling indexer -->
+  <plone:behavior
+      name="plone.textindexer"
+      title="Full-Text Indexing"
+      description="Enables the enhanced full-text indexing for a content type ('plone.textindexer'). If a field is marked 'searchable', its content gets added to the 'SearchableText' index in the catalog."
+      provides="plone.app.dexterity.textindexer.behavior.IDexterityTextIndexer"
+      />
+
+  <utility
+      factory=".supermodel.IndexerSchema"
+      name="plone.textindexer.indexer"
+      />
+
+  <adapter
+      factory="plone.app.dexterity.textindexer.indexer.dynamic_searchable_text_indexer"
+      name="SearchableText"
+      />
+
+  <!-- field converters -->
+  <adapter factory="plone.app.dexterity.textindexer.converters.DefaultDexterityTextIndexFieldConverter" />
+
+  <adapter
+      factory="plone.app.dexterity.textindexer.converters.NamedfileFieldConverter"
+      zcml:condition="installed plone.namedfile"
+      />
+
+  <adapter
+      factory="plone.app.dexterity.textindexer.converters.DexterityRichTextIndexFieldConverter"
+      zcml:condition="installed plone.app.textfield"
+      />
+
+  <adapter factory="plone.app.dexterity.textindexer.converters.IntFieldConverter" />
+
+  <adapter factory="plone.app.dexterity.textindexer.converters.TupleFieldConverter" />
+
+  <!-- plone.schemaeditor adapter -->
+  <adapter
+      factory=".schemaeditor.get_searchabletext_schema"
+      provides="plone.schemaeditor.interfaces.IFieldEditorExtender"
+      for="plone.schemaeditor.interfaces.ISchemaContext
+           zope.schema.interfaces.IField"
+      name="plone.schemaeditor.searchabletext"
+      />
+
+  <adapter
+      factory=".schemaeditor.SearchableTextField"
+      provides=".schemaeditor.ISearchableTextField"
+      for="zope.schema.interfaces.IField"
+      />
 
 </configure>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/converters.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
         # if there is no data, do nothing
         if not data or data.getSize() == 0:
             return ""
 
         # if data is already in text/plain, just return it
         if data.contentType == "text/plain":
-            return data.data
+            return safe_text(data.data)
 
         # if there is no path to text/plain, do nothing
         transforms = getToolByName(self.context, "portal_transforms")
 
         # pylint: disable=W0212
         # W0212: Access to a protected member _findPath of a client class
         if not transforms._findPath(data.contentType, "text/plain"):
@@ -99,15 +99,15 @@
         try:
             datastream = transforms.convertTo(
                 "text/plain",
                 data.data,
                 mimetype=data.contentType,
                 filename=data.filename,
             )
-            return datastream.getData()
+            return safe_text(datastream.getData())
 
         except (ConflictError, KeyboardInterrupt):
             raise
 
         except Exception as e:
             LOGGER.error(
                 "Error while trying to convert file contents " 'to "text/plain": %s',
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/directives.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/indexer.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/indexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,25 +51,24 @@
     view = FakeView(obj, request)
     z2.switch_on(view, request_layer=IFormLayer)
 
     indexed = []
 
     for _storage, fields in get_searchable_contexts_and_fields(obj):
         for field in fields:
-
             # we need the form-field, not the schema-field we
             # already have..
             form_field = Field(field, interface=field.interface, prefix="")
 
             # get the widget
             try:
                 widget = get_field_widget(obj, form_field, request)
             except TypeError:
                 # Some times the field value is wrong, then the converter
-                # failes. We should not fail, so we catch this error.
+                # fails. We should not fail, so we catch this error.
                 continue
 
             # get the converter for this field / widget
             converter = getMultiAdapter(
                 (obj, field, widget), interfaces.IDexterityTextIndexFieldConverter
             )
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/interfaces.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/interfaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 IDexterityTextIndexFieldConverter  field converter adapter interface
-IDynamicTextIndexExtender          dynmaic text extender adapter interface
+IDynamicTextIndexExtender          dynamic text extender adapter interface
 """
 
 from zope.interface import Interface
 
 
 # Supermodel namespace and prefix
 INDEXER_NAMESPACE = "http://namespaces.plone.org/supermodel/indexer"
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/schemaeditor.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/schemaeditor.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 class ISearchableTextField(Interface):
     searchable = schema.Bool(title=_("Searchable"), required=False)
 
 
 @adapter(IField)
 @implementer(ISearchableTextField)
 class SearchableTextField:
-
     namespace = INDEXER_NAMESPACE
     prefix = INDEXER_PREFIX
 
     def __init__(self, field):
         self.field = field
         self.schema = field.interface
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/supermodel.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/supermodel.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/testing.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 
 import logging
 
 
 class TextIndexerLayer(PloneSandboxLayer):
-
     defaultBases = (PLONE_FIXTURE,)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.log = None
         self.log_handler = None
 
@@ -61,15 +60,14 @@
 TEXT_INDEXER_FIXTURE = TextIndexerLayer()
 TEXT_INTEXER_INTEGRATION_TESTING = IntegrationTesting(
     bases=(TEXT_INDEXER_FIXTURE,), name="plone.app.dexterity.textindexer:Integration"
 )
 
 
 class TextIndexerFunctionalLayer(PloneSandboxLayer):
-
     defaultBases = (TEXT_INDEXER_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         import plone.app.dexterity
 
         self.loadZCML(package=plone.app.dexterity, context=configurationContext)
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/behaviors.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/behaviors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Contains different behaviors needed for testing.
 """
 from plone.app.dexterity import textindexer
 from plone.app.textfield import RichText
 from plone.autoform.interfaces import IFormFieldProvider
+from plone.namedfile.field import NamedFile
 from plone.supermodel import model
 from zope import schema
 from zope.interface import provider
 
 
 @provider(IFormFieldProvider)
 class ISimpleBehavior(model.Schema):
@@ -106,7 +107,15 @@
 class IMissingFieldBehavior(model.Schema):
     """A behavior defining a field as searchable which does not exist."""
 
     textindexer.searchable("foo")
     foo = schema.TextLine(title="Foo")
 
     textindexer.searchable("bar")
+
+
+@provider(IFormFieldProvider)
+class INamedFileFieldBehavior(model.Schema):
+    """a behavior with indexable file content"""
+
+    textindexer.searchable("foo")
+    foo = NamedFile(title="Indexable File")
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/behaviors.rst` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/behaviors.rst`

 * *Files 10% similar despite different names*

```diff
@@ -300,7 +300,47 @@
     ...                                 checkContstraints=False,
     ...                                 foo='foo value',
     ...                                 bar='bar value')
     >>> obj1
     <Item at /plone/inheritedfti>
     >>> getSearchableText(obj1)
     ['foo', 'value']
+
+
+Test, if an indexable file has been indexed::
+
+    >>> from plone.app.dexterity.textindexer.tests.behaviors import INamedFileFieldBehavior
+    >>> from plone.namedfile.file import NamedFile
+    >>> import os
+
+    >>> fti = DexterityFTI('NamedFileFTI')
+    >>> fti.behaviors = (
+    ...     'plone.textindexer',
+    ...     'plone.app.dexterity.textindexer.tests.behaviors.INamedFileFieldBehavior',
+    ... )
+    >>> portal.portal_types._setObject('NamedFileFTI', fti)
+    'NamedFileFTI'
+    >>> schema = fti.lookupSchema()
+
+    >>> obj_txtfile = createContentInContainer(portal, 'NamedFileFTI',
+    ...                                 checkContstraints=False,
+    ...                                 foo=NamedFile(b"foo bar", "text/plain", "foo.txt"))
+    >>> obj_txtfile
+    <Item at /plone/namedfilefti>
+    >>> getSearchableText(obj_txtfile)
+    ['foo', 'bar']
+
+    >>> with open(os.path.join(os.path.dirname(__file__), "file.pdf"), "rb") as f:
+    ...     foo_pdf = NamedFile(f.read(), "application/pdf", "foo.pdf")
+
+    >>> obj_pdffile = createContentInContainer(portal, 'NamedFileFTI',
+    ...                                 checkContstraints=False,
+    ...                                 foo=foo_pdf)
+
+Check if we have `pdftotext` binary. Otherwise the indexed test is empty::
+
+    >>> indexed_text = getSearchableText(obj_pdffile)
+    >>> has_pdftotext = "pdf_to_text" in portal.portal_transforms
+    >>> expected_text = ['test', 'plone', 'app', 'dexterity'] if has_pdftotext else []
+    >>> expected_text == indexed_text
+    True
+
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/configure.zcml` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/configure.zcml`

 * *Files 6% similar despite different names*

```diff
@@ -1,77 +1,87 @@
-<configure xmlns="http://namespaces.zope.org/zope"
-           xmlns:plone="http://namespaces.plone.org/plone"
-           i18n_domain="plone.app.dexterity.textindexer">
-
-    <plone:behavior
-          name="tests.textindexer.simple_behavior"
-          title="simple behavior"
-          description=""
-          provides=".behaviors.ISimpleBehavior"
-          for="plone.dexterity.interfaces.IDexterityContent"
-          />
-
-    <plone:behavior
-          name="tests.textindexer.list_behavior"
-          title="list behavior"
-          description=""
-          provides=".behaviors.IListBehavior"
-          for="plone.dexterity.interfaces.IDexterityContent"
-          />
-
-    <plone:behavior
-          name="tests.textindexer.int_behavior"
-          title="int behavior"
-          description=""
-          provides=".behaviors.IIntBehavior"
-          for="plone.dexterity.interfaces.IDexterityContent"
-          />
-
-    <plone:behavior
-          name="tests.textindexer.richtext_behavior"
-          title="richtext behavior"
-          description=""
-          provides=".behaviors.IRichTextBehavior"
-          for="plone.dexterity.interfaces.IDexterityContent"
-          />
-
-    <plone:behavior
-          name="tests.textindexer.empty_richtext_behavior"
-          title="empty richtext behavior"
-          description=""
-          provides=".behaviors.IEmptyRichTextBehavior"
-          for="plone.dexterity.interfaces.IDexterityContent"
-          />
-
-    <plone:behavior
-          name="tests.textindexer.tuple_behavior"
-          title="tuple behavior"
-          description=""
-          provides=".behaviors.ITupleBehavior"
-          for="plone.dexterity.interfaces.IDexterityContent"
-          />
-
-    <plone:behavior
-          name="tests.textindexer.tuple_choice_behavior"
-          title="tuple choice behavior"
-          description=""
-          provides=".behaviors.ITupleChoiceBehavior"
-          for="plone.dexterity.interfaces.IDexterityContent"
-          />
-
-    <plone:behavior
-          name="tests.textindexer.inherited_behavior"
-          title="inherited behavior"
-          description=""
-          provides=".behaviors.IInheritedBehavior"
-          for="plone.dexterity.interfaces.IDexterityContent"
-          />
-
-    <plone:behavior
-          name="tests.textindexer.missing_field_behavior"
-          title="missing field behavior"
-          description=""
-          provides=".behaviors.IMissingFieldBehavior"
-          for="plone.dexterity.interfaces.IDexterityContent"
-          />
+<configure
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:plone="http://namespaces.plone.org/plone"
+    i18n_domain="plone.app.dexterity.textindexer"
+    >
+
+  <plone:behavior
+      name="tests.textindexer.simple_behavior"
+      title="simple behavior"
+      description=""
+      provides=".behaviors.ISimpleBehavior"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      />
+
+  <plone:behavior
+      name="tests.textindexer.list_behavior"
+      title="list behavior"
+      description=""
+      provides=".behaviors.IListBehavior"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      />
+
+  <plone:behavior
+      name="tests.textindexer.int_behavior"
+      title="int behavior"
+      description=""
+      provides=".behaviors.IIntBehavior"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      />
+
+  <plone:behavior
+      name="tests.textindexer.richtext_behavior"
+      title="richtext behavior"
+      description=""
+      provides=".behaviors.IRichTextBehavior"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      />
+
+  <plone:behavior
+      name="tests.textindexer.empty_richtext_behavior"
+      title="empty richtext behavior"
+      description=""
+      provides=".behaviors.IEmptyRichTextBehavior"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      />
+
+  <plone:behavior
+      name="tests.textindexer.tuple_behavior"
+      title="tuple behavior"
+      description=""
+      provides=".behaviors.ITupleBehavior"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      />
+
+  <plone:behavior
+      name="tests.textindexer.tuple_choice_behavior"
+      title="tuple choice behavior"
+      description=""
+      provides=".behaviors.ITupleChoiceBehavior"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      />
+
+  <plone:behavior
+      name="tests.textindexer.inherited_behavior"
+      title="inherited behavior"
+      description=""
+      provides=".behaviors.IInheritedBehavior"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      />
+
+  <plone:behavior
+      name="tests.textindexer.missing_field_behavior"
+      title="missing field behavior"
+      description=""
+      provides=".behaviors.IMissingFieldBehavior"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      />
+
+  <plone:behavior
+      name="tests.textindexer.namedfile_behavior"
+      title="namedfile field behavior"
+      description=""
+      provides=".behaviors.INamedFileFieldBehavior"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      />
 
 </configure>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/test_behaviors.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_behaviors.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,9 @@
             ),
         ]
     )
     return suite
 
 
 class ITestingSchema(model.Schema):
-
     searchable("testing_field")
     testing_field = schema.TextLine(title="Testing field")
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/test_directives.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/test_schemaeditor.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_schemaeditor.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from plone.testing.z2 import Browser
 
 import transaction
 import unittest
 
 
 class TestSchemaEditor(unittest.TestCase):
-
     layer = TEXT_INDEXER_FUNCTIONAL_TESTING
 
     def setUp(self):
         portal_types = api.portal.get_tool("portal_types")
 
         # Define new portal type without behavior
         fti = DexterityFTI("without_behavior", title="Without Behavior")
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,9 +102,9 @@
         handler.write(field_node, IDummy, IDummy["dummy"])
 
         self.assertEqual(None, field_node.get(ns("searchable", self.namespace)))
 
 
 def test_suite():
     suite = unittest.TestSuite()
-    suite.addTest(unittest.makeSuite(TestIndexerSchema))
+    suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(TestIndexerSchema))
     return suite
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/tests/test_utils.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from plone.app.dexterity.textindexer.utils import searchable
 from plone.supermodel import model
 from unittest import TestCase
 from zope import schema
 
 
 class IExample(model.Schema):
-
     foo = schema.TextLine(title="foo")
 
 
 class IBar(model.Schema):
     pass
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/textindexer/utils.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/configure.zcml` & `plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/configure.zcml`

 * *Files 7% similar despite different names*

```diff
@@ -1,85 +1,88 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:genericsetup="http://namespaces.zope.org/genericsetup">
+    xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
+    >
 
   <genericsetup:upgradeStep
-      source="0.1"
-      destination="1"
       title="Install plone.app.z3cform browser layer"
       profile="plone.app.dexterity:default"
+      source="0.1"
+      destination="1"
       handler=".to1.install_z3cform_profile"
       />
 
   <genericsetup:upgradeStep
-      source="1"
-      destination="5"
       title="Unregister schemaeditor.css"
       profile="plone.app.dexterity:default"
+      source="1"
+      destination="5"
       handler=".to2.remove_stylesheet"
       />
 
   <!-- Dexterity 2.0 -->
 
   <genericsetup:upgradeStep
-      source="5"
-      destination="2000"
       title="Remove overlays.css from CSS registry"
       profile="plone.app.dexterity:default"
+      source="5"
+      destination="2000"
       handler=".to2000.remove_overlays_css"
       />
 
   <genericsetup:upgradeStep
-      source="2000"
-      destination="2001"
       title="Add missing UUIDs to Dexterity content"
       profile="plone.app.dexterity:default"
+      source="2000"
+      destination="2001"
       handler=".to2001.add_missing_uuids"
       />
 
   <genericsetup:upgradeStep
-      source="2000"
-      destination="2002"
       title="Install JQuery Tools date picker resources"
       profile="plone.app.dexterity:default"
+      source="2000"
+      destination="2002"
       handler=".to2002.install_datepicker_profile"
       />
 
   <genericsetup:upgradeStep
-      source="2002"
-      destination="2003"
       title="Make sure uninstalling products won't destroy the intid catalog"
       profile="plone.app.dexterity:default"
+      source="2002"
+      destination="2003"
       handler=".to2003.fix_installed_products"
       />
 
   <genericsetup:upgradeStep
+      title="Remove line feeds and carriage returns from the description"
+      profile="plone.app.dexterity:default"
       source="2003"
       destination="2004"
-      title="Remove line feeds and carrige returns from the description"
-      profile="plone.app.dexterity:default"
       handler=".to2004.remove_cr_and_lf_description"
       />
 
   <genericsetup:upgradeStep
-      source="2004"
-      destination="2005"
       title="Remove dexterity-types from portal_actions"
       profile="plone.app.dexterity:default"
+      source="2004"
+      destination="2005"
       handler=".to2005.cleanup_portal_actions"
       />
 
   <genericsetup:upgradeDepends
+      title="Update controlpanel icon"
+      profile="plone.app.dexterity:default"
       source="2005"
       destination="2006"
-      profile="plone.app.dexterity:default"
-      title="Update controlpanel icon"
-      import_steps="controlpanel" />
+      import_steps="controlpanel"
+      />
 
   <genericsetup:upgradeDepends
+      title="Rename Dexterity control panel"
+      profile="plone.app.dexterity:default"
       source="2006"
       destination="2007"
-      profile="plone.app.dexterity:default"
-      title="Rename Dexterity control panel"
-      import_steps="controlpanel" />
+      import_steps="controlpanel"
+      />
 
 </configure>
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/to2001.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2001.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/to2003.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2003.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/to2004.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2004.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     behaviors = [
         "plone.app.dexterity.behaviors.metadata.IBasic",
         "plone.app.dexterity.behaviors.metadata.IDublinCore",
     ]
 
     context = context.aq_parent
     sm = context.getSiteManager()
-    for (name, fti) in sm.getUtilitiesFor(IDexterityFTI):
+    for name, fti in sm.getUtilitiesFor(IDexterityFTI):
         for behavior in behaviors:
             if behavior in fti.behaviors:
                 types.append(name)
 
     catalog = getToolByName(context, "portal_catalog")
 
     for portal_type in types:
```

### Comparing `plone.app.dexterity-3.0.4/plone/app/dexterity/upgrades/to2005.py` & `plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2005.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.4/plone.app.dexterity.egg-info/PKG-INFO` & `plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.dexterity
-Version: 3.0.4
+Version: 3.0.5
 Summary: Dexterity is a content type framework for CMF  applications, with particular emphasis on Plone. It can be viewed as an alternative to Archetypes that is more light-weight and modular.
 Home-page: http://plone.org/products/dexterity
 Author: Martin Aspeli, David Glick, et al
 Author-email: dexterity-development@googlegroups.com
 License: GPL
 Keywords: plone ttw dexterity schema interface
 Classifier: Development Status :: 5 - Production/Stable
@@ -327,14 +327,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.5 (2023-04-14)
+------------------
+
+Bug fixes:
+
+
+- Fix for searchable Named(Blob)File indexer. Safely convert to str.
+  [petschki] (#362)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (#47959565)
+
+
 3.0.4 (2023-02-08)
 ------------------
 
 Bug fixes:
 
 
 - Restore and deprecate "ModelEditorView.modelSource".
@@ -414,15 +431,15 @@
 ---------------------
 
 Bug fixes:
 
 
 - Rename "Dexterity Content Types" to just "Content Types"
   [tisto] (#331)
-- Don't acquire lanuage from portal root default_language for ICategorization.language.
+- Don't acquire language from portal root default_language for ICategorization.language.
   Fixes https://github.com/plone/plone.app.dexterity/issues/258
   [jaroel] (#350)
 
 
 3.0.0a10 (2022-05-09)
 ---------------------
 
@@ -811,15 +828,15 @@
   New: For add forms use the "Add portal content" permission as default field permission.
   As great side effect vocabularies for i.e. AjaxSelectWidget from ``plone.app.content``,
   which are using the check, are working on add forms in a context w/o "Modify portal content".
   [jensens]
 - removed deprecated getIcon() from documentation
   [fgrcon]
 
-- JavaScript formating according to style guides.
+- JavaScript formatting according to style guides.
   [thet]
 
 
 2.4.1 (2017-03-26)
 ------------------
 
 Bug fixes:
@@ -1194,15 +1211,15 @@
   from Plone transifex organization [macagua].
 
 - Updated Spanish translation [flamelcanto, macagua].
 
 - Add validator to ensure expires date is after effective date.
   [benniboy]
 
-- Remove line feeds and carrige returns from meta description and
+- Remove line feeds and carriage returns from meta description and
   added upgrade step to do it for existing content
   [bosim]
 
 - Fixed issue.
   Multiple (two or more) acquisition from parent was failing when
   user didn't have add permission on parent.
   [keul, cekk]
```

### Comparing `plone.app.dexterity-3.0.4/plone.app.dexterity.egg-info/SOURCES.txt` & `plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
 plone/app/dexterity/textindexer/supermodel.py
 plone/app/dexterity/textindexer/testing.py
 plone/app/dexterity/textindexer/utils.py
 plone/app/dexterity/textindexer/tests/__init__.py
 plone/app/dexterity/textindexer/tests/behaviors.py
 plone/app/dexterity/textindexer/tests/behaviors.rst
 plone/app/dexterity/textindexer/tests/configure.zcml
+plone/app/dexterity/textindexer/tests/file.pdf
 plone/app/dexterity/textindexer/tests/helpers.py
 plone/app/dexterity/textindexer/tests/test_basic_behavior.py
 plone/app/dexterity/textindexer/tests/test_behaviors.py
 plone/app/dexterity/textindexer/tests/test_directives.py
 plone/app/dexterity/textindexer/tests/test_schemaeditor.py
 plone/app/dexterity/textindexer/tests/test_supermodel_handler.py
 plone/app/dexterity/textindexer/tests/test_utils.py
```

### Comparing `plone.app.dexterity-3.0.4/setup.py` & `plone.app.dexterity-3.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.4"
+version = "3.0.5"
 
 short_description = (
     "Dexterity is a content type framework for CMF  applications, "
     "with particular emphasis on Plone. It can be viewed as an "
     "alternative to Archetypes that is more light-weight and modular."
 )
 
@@ -53,40 +53,47 @@
         "plone.dexterity>=2.2.2",
         "plone.formwidget.namedfile",
         "plone.namedfile>=1.0.0",
         "plone.rfc822",
         "plone.schemaeditor >1.3.3",
         # Plone/Zope core
         "lxml",
+        "plone.base",
         "plone.app.content",
         "plone.app.layout",
         "plone.app.uuid",
         "plone.app.z3cform>=1.1.0",
         "plone.autoform>=1.1",
         "plone.contentrules",
-        "plone.portlets",
         "plone.schema>=1.1.0",
         "plone.supermodel>=1.1",
         "plone.z3cform>=0.6.0",
-        "Products.CMFCore",
         "Products.GenericSetup",
         "setuptools",
         "Zope",
         "zope.browserpage",
-        "zope.interface",
-        "zope.component",
-        "zope.deprecation",
-        "zope.schema",
-        "zope.publisher",
         "z3c.form>=3.0.0",
+        "Products.statusmessages",
+        "plone.app.vocabularies",
+        "plone.indexer",
+        "plone.locking",
+        "plone.registry",
+        "plone.uuid",
+        "zope.cachedescriptors",
+        "zope.dottedname",
+        "zope.filerepresentation",
     ],
     extras_require={
         "test": [
             "plone.app.robotframework",
             "plone.app.testing",
+            "plone.app.discussion",
+            "plone.i18n",
+            "plone.testing",
+            "robotsuite",
         ],
         "grok": [
             "five.grok",
             "plone.directives.dexterity",
             "plone.directives.form>=1.1",
         ],
         "relations": [
```

