# Comparing `tmp/plone.app.contenttypes-3.0.1.tar.gz` & `tmp/plone.app.contenttypes-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.contenttypes-3.0.1.tar", last modified: Thu Jan 26 21:17:45 2023, max compression
+gzip compressed data, was "plone.app.contenttypes-3.0.2.tar", last modified: Thu Apr 13 23:44:06 2023, max compression
```

## Comparing `plone.app.contenttypes-3.0.1.tar` & `plone.app.contenttypes-3.0.2.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.428930 plone.app.contenttypes-3.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)    45770 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      122 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    53750 2023-01-26 21:17:45.429062 plone.app.contenttypes-3.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     7006 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.392065 plone.app.contenttypes-3.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1334 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      737 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     7006 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/docs/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.392550 plone.app.contenttypes-3.0.1/docs/source/
--rw-r--r--   0 maurits    (501) staff       (20)     8053 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/docs/source/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)      471 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/docs/source/index.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.392899 plone.app.contenttypes-3.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)      265 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.395313 plone.app.contenttypes-3.0.1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)      265 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.400360 plone.app.contenttypes-3.0.1/plone/app/contenttypes/
--rw-r--r--   0 maurits    (501) staff       (20)      127 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.403228 plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     6219 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     2670 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      478 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/leadimage.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1321 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/leadimage.py
--rw-r--r--   0 maurits    (501) staff       (20)     1313 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/richtext.py
--rw-r--r--   0 maurits    (501) staff       (20)       58 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/richtext_gettext.pt
--rw-r--r--   0 maurits    (501) staff       (20)      729 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/tableofcontents.py
--rw-r--r--   0 maurits    (501) staff       (20)     2788 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/thumb_icon.py
--rw-r--r--   0 maurits    (501) staff       (20)      340 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/viewlets.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.405685 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2931 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     6695 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1091 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/file.py
--rw-r--r--   0 maurits    (501) staff       (20)     8783 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/folder.py
--rw-r--r--   0 maurits    (501) staff       (20)      991 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/full_view.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.406344 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/images/
--rw-r--r--   0 maurits    (501) staff       (20)      414 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/images/icon_export_ical.png
--rw-r--r--   0 maurits    (501) staff       (20)      427 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/images/icon_export_vcal.png
--rw-r--r--   0 maurits    (501) staff       (20)     3811 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/link_redirect_view.py
--rw-r--r--   0 maurits    (501) staff       (20)     4932 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/migration.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.409786 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)      871 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/document.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2781 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/file.pt
--rw-r--r--   0 maurits    (501) staff       (20)      968 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/full_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2263 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/full_view_item.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3151 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/image.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1783 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/image_view_fullscreen.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2106 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/link.pt
--rw-r--r--   0 maurits    (501) staff       (20)     6920 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2912 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/listing_album.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2044 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/listing_summary.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5360 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/listing_tabular.pt
--rw-r--r--   0 maurits    (501) staff       (20)      890 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/newsitem.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1964 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1722 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6481 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/content.py
--rw-r--r--   0 maurits    (501) staff       (20)     5847 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/indexers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1048 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/indexers.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1018 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      912 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/permissions.py
--rw-r--r--   0 maurits    (501) staff       (20)     1168 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.387979 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.410434 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/content/
--rw-r--r--   0 maurits    (501) staff       (20)      147 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/content/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      513 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/content/portlets.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.412213 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      145 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      873 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/diff_tool.xml
--rw-r--r--   0 maurits    (501) staff       (20)      468 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1917 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.414993 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     3040 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Collection.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2891 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Document.xml
--rw-r--r--   0 maurits    (501) staff       (20)     3113 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Event.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2748 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/File.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2917 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2782 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Image.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2640 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Link.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2895 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/News_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)      626 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Plone_Site.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1646 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)      940 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.417760 plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)       97 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/collection.xml
--rw-r--r--   0 maurits    (501) staff       (20)       97 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/document.xml
--rw-r--r--   0 maurits    (501) staff       (20)       97 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/event.xml
--rw-r--r--   0 maurits    (501) staff       (20)      774 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/file.xml
--rw-r--r--   0 maurits    (501) staff       (20)       97 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      778 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/image.xml
--rw-r--r--   0 maurits    (501) staff       (20)      825 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/link.xml
--rw-r--r--   0 maurits    (501) staff       (20)       97 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/news_item.xml
--rw-r--r--   0 maurits    (501) staff       (20)    12354 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)      585 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)      381 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/subscribers.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2670 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.426333 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     9216 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/file.doc
--rw-r--r--   0 maurits    (501) staff       (20)     9338 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/file.odt
--rw-r--r--   0 maurits    (501) staff       (20)     8561 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/file.pdf
--rw-r--r--   0 maurits    (501) staff       (20)     5131 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/image.jpg
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/image.png
--rw-r--r--   0 maurits    (501) staff       (20)     9344 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/image.svg
--rw-r--r--   0 maurits    (501) staff       (20)     4063 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/oldtypes.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.428732 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5167 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/keywords.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2152 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/test_collection_creator_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     4137 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/test_collection_location_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2123 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/test_collection_review_state_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1904 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/test_collection_short_name_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1853 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/test_collection_type_criterion.robot
--rw-r--r--   0 maurits    (501) staff       (20)    12051 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/test_folderlisting.robot
--rw-r--r--   0 maurits    (501) staff       (20)      339 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/variables.py
--rw-r--r--   0 maurits    (501) staff       (20)     3889 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_behaviors_collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     3278 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_behaviors_leadimage.py
--rw-r--r--   0 maurits    (501) staff       (20)     2205 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_behaviors_richtext.py
--rw-r--r--   0 maurits    (501) staff       (20)     2525 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_behaviors_table_of_contents.py
--rw-r--r--   0 maurits    (501) staff       (20)     1524 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_browser_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    14846 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     2522 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_collection_rss.py
--rw-r--r--   0 maurits    (501) staff       (20)     5259 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_content_profile.py
--rw-r--r--   0 maurits    (501) staff       (20)     4323 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_document.py
--rw-r--r--   0 maurits    (501) staff       (20)     4348 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_event.py
--rw-r--r--   0 maurits    (501) staff       (20)     8998 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_file.py
--rw-r--r--   0 maurits    (501) staff       (20)     8916 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_folder.py
--rw-r--r--   0 maurits    (501) staff       (20)     7363 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_image.py
--rw-r--r--   0 maurits    (501) staff       (20)    11960 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_indexes.py
--rw-r--r--   0 maurits    (501) staff       (20)    13554 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_link.py
--rw-r--r--   0 maurits    (501) staff       (20)     5556 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_news_item.py
--rw-r--r--   0 maurits    (501) staff       (20)      965 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)     8348 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_security.py
--rw-r--r--   0 maurits    (501) staff       (20)     1543 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     2318 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_webdav.py
--rw-r--r--   0 maurits    (501) staff       (20)     4530 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)      381 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/upgrades.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4071 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/plone/app/contenttypes/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-01-26 21:17:45.394983 plone.app.contenttypes-3.0.1/plone.app.contenttypes.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    53750 2023-01-26 21:17:45.000000 plone.app.contenttypes-3.0.1/plone.app.contenttypes.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     5930 2023-01-26 21:17:45.000000 plone.app.contenttypes-3.0.1/plone.app.contenttypes.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-01-26 21:17:45.000000 plone.app.contenttypes-3.0.1/plone.app.contenttypes.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-01-26 21:17:45.000000 plone.app.contenttypes-3.0.1/plone.app.contenttypes.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-01-26 21:17:45.000000 plone.app.contenttypes-3.0.1/plone.app.contenttypes.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      440 2023-01-26 21:17:45.000000 plone.app.contenttypes-3.0.1/plone.app.contenttypes.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-01-26 21:17:45.000000 plone.app.contenttypes-3.0.1/plone.app.contenttypes.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      234 2023-01-26 21:17:45.429544 plone.app.contenttypes-3.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2461 2023-01-26 21:17:44.000000 plone.app.contenttypes-3.0.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.818029 plone.app.contenttypes-3.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)    46077 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    54057 2023-04-13 23:44:06.818167 plone.app.contenttypes-3.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     7006 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.783993 plone.app.contenttypes-3.0.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1334 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      737 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     7006 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/docs/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.784697 plone.app.contenttypes-3.0.2/docs/source/
+-rw-r--r--   0 maurits    (501) staff       (20)     8036 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/docs/source/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      471 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/docs/source/index.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.784951 plone.app.contenttypes-3.0.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.787284 plone.app.contenttypes-3.0.2/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.791550 plone.app.contenttypes-3.0.2/plone/app/contenttypes/
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.794484 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6169 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2809 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      548 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/leadimage.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1320 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/leadimage.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1312 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/richtext.py
+-rw-r--r--   0 maurits    (501) staff       (20)       63 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/richtext_gettext.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      728 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/tableofcontents.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2787 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/thumb_icon.py
+-rw-r--r--   0 maurits    (501) staff       (20)      340 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/viewlets.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.796958 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2931 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6737 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1091 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/file.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8782 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/folder.py
+-rw-r--r--   0 maurits    (501) staff       (20)      991 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/full_view.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.797596 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/images/
+-rw-r--r--   0 maurits    (501) staff       (20)      414 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/images/icon_export_ical.png
+-rw-r--r--   0 maurits    (501) staff       (20)      427 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/images/icon_export_vcal.png
+-rw-r--r--   0 maurits    (501) staff       (20)     3810 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/link_redirect_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4092 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/migration.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.801274 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     1045 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/document.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3434 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/file.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1264 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/full_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2497 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/full_view_item.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3669 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/image.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2069 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/image_view_fullscreen.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2552 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/link.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     8869 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4474 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing_album.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2926 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing_summary.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     7518 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing_tabular.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1091 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/newsitem.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1964 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1781 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6481 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5847 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/indexers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1251 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/indexers.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1018 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      912 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/permissions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1227 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.780225 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.801770 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/content/
+-rw-r--r--   0 maurits    (501) staff       (20)      191 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/content/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      591 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/content/portlets.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.803093 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      184 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1031 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/diff_tool.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      522 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2113 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.805497 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     3097 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Collection.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2943 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     3175 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Event.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2810 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/File.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2974 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2844 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Image.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2692 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Link.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2947 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/News_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      648 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Plone_Site.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1957 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      963 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.807733 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/collection.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/event.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      865 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/file.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      869 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/image.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      880 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/link.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      131 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/news_item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)    12355 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      585 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/subscribers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      401 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/subscribers.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2669 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.815409 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9216 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/file.doc
+-rw-r--r--   0 maurits    (501) staff       (20)     9338 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/file.odt
+-rw-r--r--   0 maurits    (501) staff       (20)     8561 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/file.pdf
+-rw-r--r--   0 maurits    (501) staff       (20)     5131 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/image.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/image.png
+-rw-r--r--   0 maurits    (501) staff       (20)     9344 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/image.svg
+-rw-r--r--   0 maurits    (501) staff       (20)     4063 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/oldtypes.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.817816 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5132 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/keywords.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2117 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_creator_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     4067 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_location_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2088 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_review_state_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1869 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_short_name_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1818 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_type_criterion.robot
+-rw-r--r--   0 maurits    (501) staff       (20)    11981 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_folderlisting.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      339 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/variables.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3888 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3277 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_leadimage.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2205 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_richtext.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2278 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_table_of_contents.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1524 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_browser_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14842 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2521 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_collection_rss.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5127 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_content_profile.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4321 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_document.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4346 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_event.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8996 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_file.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8912 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_folder.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7360 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_image.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11959 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_indexes.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13550 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_link.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5554 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_news_item.py
+-rw-r--r--   0 maurits    (501) staff       (20)      965 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8278 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_security.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1542 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2318 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_webdav.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4530 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)      392 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/upgrades.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4071 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone/app/contenttypes/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:44:06.786918 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    54057 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     5930 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      848 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1707 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-13 23:44:06.818623 plone.app.contenttypes-3.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     3164 2023-04-13 23:44:06.000000 plone.app.contenttypes-3.0.2/setup.py
```

### Comparing `plone.app.contenttypes-3.0.1/CHANGES.rst` & `plone.app.contenttypes-3.0.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,38 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2023-04-14)
+------------------
+
+Bug fixes:
+
+
+- Fix test_behaviors_table_of_contents: ordering of attrtributes changed.
+  @jensens (fix-test_behaviors_table_of_contents)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (#47959565)
+
+
+Tests
+
+
+- Run the robot tests.
+  [maurits] (#69)
+
+
 3.0.1 (2023-01-26)
 ------------------
 
 Bug fixes:
 
 
 - Fix error in News Item view when it doesn't have a text field. [davisagli] (#652)
@@ -782,15 +806,15 @@
 
 New features:
 
 - New metadata catalog column MimeType
   https://github.com/plone/Products.CMFPlone/issues/1995
   [fgrcon]
 
-- new behavior: IThumbIconHandling, supress thumbs /icons, adjust thumb size, templates adapted
+- new behavior: IThumbIconHandling, suppress thumbs /icons, adjust thumb size, templates adapted
   https://github.com/plone/Products.CMFPlone/issues/1734 (PLIP)
 
 Bug fixes:
 
 - fixed css-classes for thumb scales ...
   https://github.com/plone/Products.CMFPlone/issues/2077
   [fgrcon]
@@ -900,15 +924,15 @@
 -------------------
 
 New features:
 
 - Configure edit urls for locking support, where locking support is enabled.
   [thet]
 
-- Add ``i18n:attribute`` properies to all action nodes for FTI types.
+- Add ``i18n:attribute`` properties to all action nodes for FTI types.
   [thet]
 
 - added few pypi links in 'Migration' section
   [kkhan]
 
 Bug fixes:
 
@@ -1141,15 +1165,15 @@
 
 1.2.4 (2015-09-27)
 ------------------
 
 - Fixed full_view error when collection contains itself.
   [vangheem]
 
-- test_content_profile: do not appy Products.CMFPlone:plone.
+- test_content_profile: do not apply Products.CMFPlone:plone.
   [maurits]
 
 
 1.2.3 (2015-09-20)
 ------------------
 
 - Do not raise an exception for items where @@full_view_item throws an
@@ -1158,26 +1182,26 @@
 
 - Do not raise errors when IPrimaryFieldInfo(obj) fails (e.g. when the
   Schema-Cache is gone).
   Fixes https://github.com/plone/Products.CMFPlone/issues/839
   [pbauer]
 
 - Fix an error with logging an exception on indexing SearchableText for files
-  and concating utf-8 encoded strings.
+  and concatenating utf-8 encoded strings.
   [thet]
 
 - Make consistent use of LeadImage behavior everywhere. Related to
   plone/plone.app.contenttypes#1012. Contentleadimages no longer show up in
   full_view since they are a viewlet.
   [sneridagh, pbauer]
 
 - Fixed the summary_view styling
   [sneridagh]
 - redirect_links property has moved to the configuration registry.
-- redirect_links, types_view_action_in_listings properies have moved to the
+- redirect_links, types_view_action_in_listings properties have moved to the
   configuration registry.
   [esteele]
 
 
 1.2.2 (2015-09-15)
 ------------------
 
@@ -1436,15 +1460,15 @@
 
 1.2a5 (2014-10-23)
 ------------------
 
 - Code modernization: sorted imports, use decorators, utf8 headers.
   [jensens]
 
-- Fix: Added missing types to CMFDiffTool configuraion.
+- Fix: Added missing types to CMFDiffTool configuration.
   [jensens]
 
 - Integration of the new markup update and CSS for both Plone and Barceloneta
   theme. This is the work done in the GSOC Barceloneta theme project. Fix
   several templates.
   [albertcasado, sneridagh]
 
@@ -1476,15 +1500,15 @@
   The previous release of p.a.c got an implicit Plone 5 dependency through a
   previous version of plone.app.event.
   [thet]
 
 - Replace AT-fti with DX-fti when migrating a type.
   [esteele, pbauer]
 
-- Only show migrateable types (fixes #155)
+- Only show migratable types (fixes #155)
   [pbauer]
 
 - Add logging during and after migration (fixes #156)
   [pbauer]
 
 - When replacing the default news and events collections, reverse the
   sort order correctly.
@@ -1575,15 +1599,15 @@
 
 - Don't remove custom behaviors on reinstalling.
   [pbauer]
 
 - Remove enabling simple_publication_workflow from testing fixture.
   [timo]
 
-- Only show migrateable types (fixes #155)
+- Only show migratable types (fixes #155)
   [pbauer]
 
 - Add logging during and after migration (fixes #156)
   [pbauer]
 
 - Remove 'robot-test-folder' from p.a.contenttypes test setup. It is bad to
   add content to test layers, especially if those test layers are used by
@@ -1741,30 +1765,30 @@
 
 - Its possible to upload non-image data into a newsitem. The view was broken
   then. Now it shows the uploaded file for download below the content. Its no
   longer broken.
   [jensens]
 
 - Add contributor role as default for all add permissions in order to
-  work together with the different plone worklfows, which assume it is
+  work together with the different plone workflows, which assume it is
   set this way.
   [jensens]
 
 - fix #60: File Type has no mimetype specific icon in catalog metadata.
   Also fixed for Image.
   [jensens]
 
 - fix #58: Migration ignores "Exclude from Navigation".
   [jensens]
 
 - disable LinkIntegrityNotifications during migrations, closes #40.
   [jensens]
 
 - Fix Bug on SearchableText_file indexer when input stream contains
-  characters not convertable in ASCII. Assumes now utf-8 and replaces
+  characters not convertible in ASCII. Assumes now utf-8 and replaces
   all unknown. Even if search can not find the words with special
   characters in, indexer does not break completely on those items.
   [jensens]
 
 - Remove dependency on plone.app.referenceablebehavior, as it depends on
   Products.Archetypes which installs the uid_catalog.
   [thet]
```

### Comparing `plone.app.contenttypes-3.0.1/PKG-INFO` & `plone.app.contenttypes-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contenttypes
-Version: 3.0.1
+Version: 3.0.2
 Summary: Default content types for Plone based on Dexterity
 Home-page: https://github.com/plone/plone.app.contenttypes
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: plone content types dexterity
 Classifier: Development Status :: 5 - Production/Stable
@@ -218,14 +218,38 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2023-04-14)
+------------------
+
+Bug fixes:
+
+
+- Fix test_behaviors_table_of_contents: ordering of attrtributes changed.
+  @jensens (fix-test_behaviors_table_of_contents)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (#47959565)
+
+
+Tests
+
+
+- Run the robot tests.
+  [maurits] (#69)
+
+
 3.0.1 (2023-01-26)
 ------------------
 
 Bug fixes:
 
 
 - Fix error in News Item view when it doesn't have a text field. [davisagli] (#652)
@@ -996,15 +1020,15 @@
 
 New features:
 
 - New metadata catalog column MimeType
   https://github.com/plone/Products.CMFPlone/issues/1995
   [fgrcon]
 
-- new behavior: IThumbIconHandling, supress thumbs /icons, adjust thumb size, templates adapted
+- new behavior: IThumbIconHandling, suppress thumbs /icons, adjust thumb size, templates adapted
   https://github.com/plone/Products.CMFPlone/issues/1734 (PLIP)
 
 Bug fixes:
 
 - fixed css-classes for thumb scales ...
   https://github.com/plone/Products.CMFPlone/issues/2077
   [fgrcon]
@@ -1114,15 +1138,15 @@
 -------------------
 
 New features:
 
 - Configure edit urls for locking support, where locking support is enabled.
   [thet]
 
-- Add ``i18n:attribute`` properies to all action nodes for FTI types.
+- Add ``i18n:attribute`` properties to all action nodes for FTI types.
   [thet]
 
 - added few pypi links in 'Migration' section
   [kkhan]
 
 Bug fixes:
 
@@ -1355,15 +1379,15 @@
 
 1.2.4 (2015-09-27)
 ------------------
 
 - Fixed full_view error when collection contains itself.
   [vangheem]
 
-- test_content_profile: do not appy Products.CMFPlone:plone.
+- test_content_profile: do not apply Products.CMFPlone:plone.
   [maurits]
 
 
 1.2.3 (2015-09-20)
 ------------------
 
 - Do not raise an exception for items where @@full_view_item throws an
@@ -1372,26 +1396,26 @@
 
 - Do not raise errors when IPrimaryFieldInfo(obj) fails (e.g. when the
   Schema-Cache is gone).
   Fixes https://github.com/plone/Products.CMFPlone/issues/839
   [pbauer]
 
 - Fix an error with logging an exception on indexing SearchableText for files
-  and concating utf-8 encoded strings.
+  and concatenating utf-8 encoded strings.
   [thet]
 
 - Make consistent use of LeadImage behavior everywhere. Related to
   plone/plone.app.contenttypes#1012. Contentleadimages no longer show up in
   full_view since they are a viewlet.
   [sneridagh, pbauer]
 
 - Fixed the summary_view styling
   [sneridagh]
 - redirect_links property has moved to the configuration registry.
-- redirect_links, types_view_action_in_listings properies have moved to the
+- redirect_links, types_view_action_in_listings properties have moved to the
   configuration registry.
   [esteele]
 
 
 1.2.2 (2015-09-15)
 ------------------
 
@@ -1650,15 +1674,15 @@
 
 1.2a5 (2014-10-23)
 ------------------
 
 - Code modernization: sorted imports, use decorators, utf8 headers.
   [jensens]
 
-- Fix: Added missing types to CMFDiffTool configuraion.
+- Fix: Added missing types to CMFDiffTool configuration.
   [jensens]
 
 - Integration of the new markup update and CSS for both Plone and Barceloneta
   theme. This is the work done in the GSOC Barceloneta theme project. Fix
   several templates.
   [albertcasado, sneridagh]
 
@@ -1690,15 +1714,15 @@
   The previous release of p.a.c got an implicit Plone 5 dependency through a
   previous version of plone.app.event.
   [thet]
 
 - Replace AT-fti with DX-fti when migrating a type.
   [esteele, pbauer]
 
-- Only show migrateable types (fixes #155)
+- Only show migratable types (fixes #155)
   [pbauer]
 
 - Add logging during and after migration (fixes #156)
   [pbauer]
 
 - When replacing the default news and events collections, reverse the
   sort order correctly.
@@ -1789,15 +1813,15 @@
 
 - Don't remove custom behaviors on reinstalling.
   [pbauer]
 
 - Remove enabling simple_publication_workflow from testing fixture.
   [timo]
 
-- Only show migrateable types (fixes #155)
+- Only show migratable types (fixes #155)
   [pbauer]
 
 - Add logging during and after migration (fixes #156)
   [pbauer]
 
 - Remove 'robot-test-folder' from p.a.contenttypes test setup. It is bad to
   add content to test layers, especially if those test layers are used by
@@ -1955,30 +1979,30 @@
 
 - Its possible to upload non-image data into a newsitem. The view was broken
   then. Now it shows the uploaded file for download below the content. Its no
   longer broken.
   [jensens]
 
 - Add contributor role as default for all add permissions in order to
-  work together with the different plone worklfows, which assume it is
+  work together with the different plone workflows, which assume it is
   set this way.
   [jensens]
 
 - fix #60: File Type has no mimetype specific icon in catalog metadata.
   Also fixed for Image.
   [jensens]
 
 - fix #58: Migration ignores "Exclude from Navigation".
   [jensens]
 
 - disable LinkIntegrityNotifications during migrations, closes #40.
   [jensens]
 
 - Fix Bug on SearchableText_file indexer when input stream contains
-  characters not convertable in ASCII. Assumes now utf-8 and replaces
+  characters not convertible in ASCII. Assumes now utf-8 and replaces
   all unknown. Even if search can not find the words with special
   characters in, indexer does not break completely on those items.
   [jensens]
 
 - Remove dependency on plone.app.referenceablebehavior, as it depends on
   Products.Archetypes which installs the uid_catalog.
   [thet]
```

### Comparing `plone.app.contenttypes-3.0.1/README.rst` & `plone.app.contenttypes-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/docs/INSTALL.txt` & `plone.app.contenttypes-3.0.2/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/docs/LICENSE.GPL` & `plone.app.contenttypes-3.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/docs/LICENSE.txt` & `plone.app.contenttypes-3.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/docs/README.rst` & `plone.app.contenttypes-3.0.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/docs/source/conf.py` & `plone.app.contenttypes-3.0.2/docs/source/conf.py`

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
 # sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
 
@@ -167,20 +163,20 @@
 # Output file base name for HTML help builder.
 htmlhelp_basename = "ploneappcontenttypesdoc"
 
 
 # -- Options for LaTeX output --------------------------------------------------
 
 latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #'papersize': 'letterpaper',
-    # The font size ('10pt', '11pt' or '12pt').
-    #'pointsize': '10pt',
-    # Additional stuff for the LaTeX preamble.
-    #'preamble': '',
+    #  The paper size ('letterpaper' or 'a4paper').
+    # 'papersize': 'letterpaper',
+    #  The font size ('10pt', '11pt' or '12pt').
+    # 'pointsize': '10pt',
+    #  Additional stuff for the LaTeX preamble.
+    # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
     (
         "index",
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/collection.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from plone.app.z3cform.widget import QueryStringFieldWidget
 from plone.autoform import directives as form
 from plone.autoform.interfaces import IFormFieldProvider
 from plone.base.interfaces.syndication import IFeed
 from plone.base.interfaces.syndication import ISyndicatable
 from plone.dexterity.interfaces import IDexterityContent
 from plone.supermodel import model
-from Products.CMFCore.utils import getToolByName
 from Products.CMFPlone.browser.syndication.adapters import (
     CollectionFeed as BaseCollectionFeed,
 )
 from zope import schema
 from zope.component import adapter
 from zope.component import getMultiAdapter
 from zope.component import getUtility
@@ -30,15 +29,14 @@
     "Import from plone.app.vocabularies.metadatafields instead (this compatibility layer will be removed in Plone 6)",
     MetaDataFieldsVocabularyFactory="plone.app.vocabularies.metadatafields:MetaDataFieldsVocabularyFactory",
 )
 
 
 @provider(IFormFieldProvider, ISyndicatable)
 class ICollection(model.Schema):
-
     query = schema.List(
         title=_("Search terms"),
         description=_(
             "Define the search terms for the items you want "
             "to list by choosing what to match on. "
             "The list of results will be dynamically updated"
         ),
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/configure.zcml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/configure.zcml`

 * *Files 4% similar despite different names*

```diff
@@ -1,84 +1,91 @@
 <configure
-  xmlns="http://namespaces.zope.org/zope"
-  xmlns:browser="http://namespaces.zope.org/browser"
-  xmlns:plone="http://namespaces.plone.org/plone"
-  xmlns:zcml="http://namespaces.zope.org/zcml"
-  i18n_domain="plone">
-
-  <include package="plone.behavior" file="meta.zcml"/>
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:browser="http://namespaces.zope.org/browser"
+    xmlns:plone="http://namespaces.plone.org/plone"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    i18n_domain="plone"
+    >
+
+  <include
+      package="plone.behavior"
+      file="meta.zcml"
+      />
 
   <plone:behavior
-    name="plone.leadimage"
-    title="Lead Image"
-    description="Adds image and image caption fields"
-    provides=".leadimage.ILeadImageBehavior"
-    factory=".leadimage.LeadImage"
-    for="plone.dexterity.interfaces.IDexterityContent"
-    marker=".leadimage.ILeadImage"
-    former_dotted_names="plone.app.contenttypes.behaviors.leadimage.ILeadImage"
-    />
+      name="plone.leadimage"
+      title="Lead Image"
+      description="Adds image and image caption fields"
+      factory=".leadimage.LeadImage"
+      provides=".leadimage.ILeadImageBehavior"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      marker=".leadimage.ILeadImage"
+      former_dotted_names="plone.app.contenttypes.behaviors.leadimage.ILeadImage"
+      />
 
   <browser:viewlet
-    name="contentleadimage"
-    for=".leadimage.ILeadImage"
-    view="plone.app.layout.globals.interfaces.IViewView"
-    class=".viewlets.LeadImageViewlet"
-    manager="plone.app.layout.viewlets.interfaces.IAboveContentTitle"
-    template="leadimage.pt"
-    permission="zope2.View"
-    />
+      name="contentleadimage"
+      for=".leadimage.ILeadImage"
+      view="plone.app.layout.globals.interfaces.IViewView"
+      manager="plone.app.layout.viewlets.interfaces.IAboveContentTitle"
+      class=".viewlets.LeadImageViewlet"
+      template="leadimage.pt"
+      permission="zope2.View"
+      />
 
   <plone:behavior
-    name="plone.tableofcontents"
-    title="Table of contents"
-    description="Adds a table of contents"
-    provides=".tableofcontents.ITableOfContents"
-    marker=".tableofcontents.ITableOfContents"
-    />
+      name="plone.tableofcontents"
+      title="Table of contents"
+      description="Adds a table of contents"
+      provides=".tableofcontents.ITableOfContents"
+      marker=".tableofcontents.ITableOfContents"
+      />
 
   <plone:behavior
-    name="plone.collection"
-    title="Collection"
-    description="Adds collection behavior"
-    provides=".collection.ICollection"
-    factory=".collection.Collection"
-    for="plone.dexterity.interfaces.IDexterityContent"
-    marker=".collection.ISyndicatableCollection"
-    />
+      name="plone.collection"
+      title="Collection"
+      description="Adds collection behavior"
+      factory=".collection.Collection"
+      provides=".collection.ICollection"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      marker=".collection.ISyndicatableCollection"
+      />
 
   <plone:behavior
-    name="plone.richtext"
-    title="RichText"
-    description="Adds richtext behavior"
-    provides=".richtext.IRichTextBehavior"
-    factory=".richtext.RichText"
-    for="plone.dexterity.interfaces.IDexterityContent"
-    marker=".richtext.IRichText"
-    former_dotted_names="plone.app.contenttypes.behaviors.richtext.IRichText"
-    />
+      name="plone.richtext"
+      title="RichText"
+      description="Adds richtext behavior"
+      factory=".richtext.RichText"
+      provides=".richtext.IRichTextBehavior"
+      for="plone.dexterity.interfaces.IDexterityContent"
+      marker=".richtext.IRichText"
+      former_dotted_names="plone.app.contenttypes.behaviors.richtext.IRichText"
+      />
 
   <plone:behavior
       name="plone.thumb_icon"
       title="Thumbs and icon handling"
       description="Options to suppress thumbs and/or icons and to override thumb size in listings, tables etc."
       provides=".thumb_icon.IThumbIconHandling"
       />
 
   <browser:page
-    name="getText"
-    for=".richtext.IRichText"
-    class=".richtext.WidgetView"
-    permission="zope2.View"
-    template="richtext_gettext.pt"
-    />
+      name="getText"
+      for=".richtext.IRichText"
+      class=".richtext.WidgetView"
+      template="richtext_gettext.pt"
+      permission="zope2.View"
+      />
 
   <!-- Register the plone.app.vocabularies.MetadataFields under the old
        name for backward compatibility. -->
   <utility
+      name="plone.app.contenttypes.metadatafields"
       component="plone.app.vocabularies.metadatafields.MetaDataFieldsVocabularyFactory"
-      name="plone.app.contenttypes.metadatafields" />
+      />
 
-  <adapter factory=".collection.CollectionFeed"
-           for=".collection.ISyndicatableCollection" />
+  <adapter
+      factory=".collection.CollectionFeed"
+      for=".collection.ISyndicatableCollection"
+      />
 
 </configure>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/leadimage.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/leadimage.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 class ILeadImage(Interface):
     pass
 
 
 @provider(IFormFieldProvider)
 class ILeadImageBehavior(model.Schema):
-
     image = namedfile.NamedBlobImage(
         title=_("label_leadimage", default="Lead Image"),
         description="",
         required=False,
     )
 
     image_caption = schema.TextLine(
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/richtext.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/richtext.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 class IRichText(Interface):
     pass
 
 
 @provider(IFormFieldProvider)
 class IRichTextBehavior(model.Schema):
-
     text = RichTextField(
         title=_("Text"),
         description="",
         required=False,
     )
     form.widget("text", RichTextFieldWidget)
     model.primary("text")
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/tableofcontents.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/tableofcontents.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 
 _ = MessageFactory("plone")
 
 
 @provider(IFormFieldProvider)
 class ITableOfContents(model.Schema):
-
     model.fieldset("settings", label=_("Settings"), fields=["table_of_contents"])
 
     table_of_contents = schema.Bool(
         title=_("help_enable_table_of_contents", default="Table of contents"),
         description=_(
             "help_enable_table_of_contents_description",
             default="If selected, this will show a table of contents"
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/behaviors/thumb_icon.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/behaviors/thumb_icon.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from z3c.form.interfaces import IEditForm
 from zope import schema
 from zope.interface import provider
 
 
 @provider(IFormFieldProvider)
 class IThumbIconHandling(model.Schema):
-
     model.fieldset(
         "settings",
         label=_("Settings"),
         fields=[
             "thumb_scale_list",
             "thumb_scale_table",
             "thumb_scale_summary",
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/collection.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/collection.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/configure.zcml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 <configure
-  xmlns="http://namespaces.zope.org/zope"
-  xmlns:browser="http://namespaces.zope.org/browser"
-  xmlns:z3c="http://namespaces.zope.org/z3c"
-  xmlns:zcml="http://namespaces.zope.org/zcml"
-  i18n_domain="plone">
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:browser="http://namespaces.zope.org/browser"
+    xmlns:z3c="http://namespaces.zope.org/z3c"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    i18n_domain="plone"
+    >
 
   <include package="plone.app.contentmenu" />
 
   <!-- VIEWS FOR PLONE SITE ROOT -->
   <browser:pages
       for="plone.base.interfaces.IPloneSiteRoot"
       class=".folder.FolderView"
-      permission="zope2.View">
+      permission="zope2.View"
+      >
     <browser:page
         name="listing_view"
         template="templates/listing.pt"
         menu="plone_displayviews"
         title="Standard view"
         />
     <browser:page
@@ -45,15 +47,16 @@
   </browser:pages>
 
 
   <!-- VIEWS FOR FOLDERS -->
   <browser:pages
       for="plone.dexterity.interfaces.IDexterityContainer"
       class=".folder.FolderView"
-      permission="zope2.View">
+      permission="zope2.View"
+      >
     <browser:page
         name="listing_view"
         template="templates/listing.pt"
         menu="plone_displayviews"
         title="Standard view"
         />
     <browser:page
@@ -95,15 +98,16 @@
   <!-- VIEWS FOR ANYTHING WITH THE COLLECTION BEHAVIOR.
        Note that these ignore other fields, but integrators should
        create other themplates if they want that.  Or improve the
        query view widget.  -->
   <browser:pages
       for="plone.app.contenttypes.behaviors.collection.ISyndicatableCollection"
       class=".collection.CollectionView"
-      permission="zope2.View">
+      permission="zope2.View"
+      >
     <browser:page
         name="listing_view"
         template="templates/listing.pt"
         menu="plone_displayviews"
         title="Standard view"
         />
     <browser:page
@@ -135,87 +139,88 @@
 
   <!-- OTHER VIEWS -->
   <browser:page
       name="full_view_item"
       for="*"
       class=".full_view.FullViewItem"
       template="templates/full_view_item.pt"
-      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       permission="zope2.View"
+      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       />
   <browser:page
       name="document_view"
       template="templates/document.pt"
-      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       permission="zope2.View"
+      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       menu="plone_displayviews"
       title="View Document"
       />
   <browser:page
       name="file_view"
       for="plone.app.contenttypes.interfaces.IFile"
       class=".file.FileView"
       template="templates/file.pt"
-      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       permission="zope2.View"
+      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       menu="plone_displayviews"
       title="View File"
       />
   <browser:page
       name="image_view"
       for="plone.app.contenttypes.interfaces.IImage"
       template="templates/image.pt"
-      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       permission="zope2.View"
+      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       menu="plone_displayviews"
       title="View Image"
       />
   <browser:page
       name="image_view_fullscreen"
       for="plone.app.contenttypes.interfaces.IImage"
       template="templates/image_view_fullscreen.pt"
-      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       permission="zope2.View"
+      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       menu="plone_displayviews"
       title="View Image Fullscreen"
       />
   <browser:page
       name="link_redirect_view"
       for="plone.app.contenttypes.interfaces.ILink"
       class=".link_redirect_view.LinkRedirectView"
-      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       permission="zope2.View"
+      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       menu="plone_displayviews"
       title="View Link"
       />
   <browser:page
       name="newsitem_view"
       for="plone.app.contenttypes.interfaces.INewsItem"
       template="templates/newsitem.pt"
-      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       permission="zope2.View"
+      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       menu="plone_displayviews"
       title="View News Item"
       />
   <browser:page
       name="contenttype_utils"
       for="*"
       class=".utils.Utils"
       allowed_interface="plone.app.contenttypes.browser.utils.IUtils"
-      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       permission="zope2.View"
+      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       />
 
   <browser:page
       name="base_class_migrator_form"
       for="plone.base.interfaces.IPloneSiteRoot"
       class="plone.app.contenttypes.browser.migration.BaseClassMigrator"
-      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       permission="cmf.ManagePortal"
+      layer="plone.app.contenttypes.interfaces.IPloneAppContenttypesLayer"
       />
 
   <utility
       factory="plone.app.contenttypes.browser.migration.ChangedBaseClasses"
+      provides="zope.schema.interfaces.IVocabularyFactory"
       name="plone.app.contenttypes.migration.changed_base_classes"
-      provides="zope.schema.interfaces.IVocabularyFactory" />
+      />
 
 </configure>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/file.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/file.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/folder.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from zope.component import getUtility
 from zope.contentprovider.interfaces import IContentProvider
 
 import random
 
 
 class FolderView(BrowserView):
-
     text_class = None
     _plone_view = None
     _portal_state = None
     _pas_member = None
 
     @property
     def plone_view(self):
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/full_view.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/full_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/link_redirect_view.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/link_redirect_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 NON_RESOLVABLE_URL_SCHEMES = NON_REDIRECTABLE_URL_SCHEMES + [
     "file:",
     "ftp:",
 ]
 
 
 class LinkRedirectView(BrowserView):
-
     index = ViewPageTemplateFile("templates/link.pt")
 
     def _url_uses_scheme(self, schemes, url=None):
         url = url or self.context.remoteUrl.strip()
         for scheme in schemes:
             if url.startswith(scheme):
                 return True
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/document.pt` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/newsitem.pt`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,35 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-    xmlns:tal="http://xml.zope.org/namespaces/tal"
-    xmlns:metal="http://xml.zope.org/namespaces/metal"
-    xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    metal:use-macro="context/@@main_template/macros/master"
-    i18n:domain="plone">
-<body>
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
 
-<metal:content-core fill-slot="content-core">
-<metal:content-core define-macro="content-core"
-                    tal:define="toc python:  getattr(context, 'table_of_contents', False);">
+    <metal:content-core fill-slot="content-core">
+      <metal:content-core define-macro="content-core"
+                          tal:define="
+                            toc python: getattr(context, 'table_of_contents', False);
+                          "
+      >
 
-  <section id="section-text">
-    <div id="parent-fieldname-text" class="${python: toc and 'pat-autotoc' or ''}"
-         tal:condition="python:getattr(context, 'text', None)"
-         tal:content="structure python:context.text.output_relative_to(view.context)">
+        <section id="section-text">
+          <div id="parent-fieldname-text"
+               tal:condition="python:getattr(context, 'text', None)"
+               tal:content="structure python:context.text.output_relative_to(view.context)"
+               tal:attributes="
+                 class python: toc and 'pat-autotoc' or '';
+               "
+          >
       Text
-    </div>
-  </section>
+          </div>
+        </section>
 
-</metal:content-core>
-</metal:content-core>
+      </metal:content-core>
+    </metal:content-core>
 
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/file.pt` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/file.pt`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,89 @@
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
-<metal:block define-macro="content-core"
-             tal:define="content_type python: context.file.contentType;
-                         filename python: context.file.filename;
-                         mimetype_icon python: 'mimetype-' + content_type;
-                         download_url python: '{}/@@download/file/{}'.format(context.absolute_url(), filename)">
-
-  <section class="section section-main">
-
-    <div tal:condition="python: not view.is_videotype() and not view.is_audiotype()">
-      <tal:icon tal:replace="structure python:icons.tag(mimetype_icon, tag_class='icon-x4 mb-2')" />
-    </div>
-
-    <video class="w-100 mb-3" controls="controls" tal:condition="python: view.is_videotype()">
-      <source src="${python:download_url}" type="${python:content_type}"></source>
-      <tal:icon tal:replace="structure python:icons.tag(mimetype_icon, tag_class='icon-x4 mb-2')" />
-      <div i18n:translate="embedded_video_not_supported" class="small text-muted">Sorry, your browser doesn't support embedded videos.</div>
-    </video>
-
-    <audio class="w-100 mb-3" controls="controls" tal:condition="python:view.is_audiotype()">
-      <source tal:attributes="src python: download_url; type python: content_type"></source>
-      <tal:icon tal:replace="structure python:icons.tag(mimetype_icon, tag_class='icon-x4 mb-2')" />
-      <div i18n:translate="embedded_audio_not_supported" class="small text-muted">Sorry, your browser doesn't support embedded audio.</div>
-    </audio>
-
-    <div class="h5 mb-2">
-      <a href="${python:download_url}" tal:content="python: filename">Filename</a>
-    </div>
-
-    <div class="metadata d-flex justify-content-center text-muted small">
-      <div class="px-2">
-        <tal:icon tal:replace="structure python:icons.tag(mimetype_icon, tag_class='icon-inline', tag_alt=content_type)" />
-        <span tal:replace="python: content_type">image/jpeg</span>
-      </div>
-      <div class="px-2">
-        <tal:icon tal:replace="structure python:icons.tag('file-binary', tag_class='icon-inline', tag_alt='Size')" />
-        <span tal:define="size python: view.human_readable_size()" tal:content="python: size">1000 kB</span>
-      </div>
-    </div>
-
-  </section>
-
-  <section class="section section-actions">
-    <a class="btn btn-primary download" href="${python:download_url}" i18n:translate="">Download</a>
-  </section>
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
+      <metal:block define-macro="content-core"
+                   tal:define="
+                     content_type python: context.file.contentType;
+                     filename python: context.file.filename;
+                     mimetype_icon python: 'mimetype-' + content_type;
+                     download_url python: '{}/@@download/file/{}'.format(context.absolute_url(), filename);
+                   "
+      >
+
+        <section class="section section-main">
+
+          <div tal:condition="python: not view.is_videotype() and not view.is_audiotype()">
+            <tal:icon tal:replace="structure python:icons.tag(mimetype_icon, tag_class='icon-x4 mb-2')" />
+          </div>
+
+          <video class="w-100 mb-3"
+                 controls="controls"
+                 tal:condition="python: view.is_videotype()"
+          >
+            <source src="${python:download_url}"
+                    type="${python:content_type}"
+            />
+            <tal:icon tal:replace="structure python:icons.tag(mimetype_icon, tag_class='icon-x4 mb-2')" />
+            <div class="small text-muted"
+                 i18n:translate="embedded_video_not_supported"
+            >Sorry, your browser doesn't support embedded videos.</div>
+          </video>
+
+          <audio class="w-100 mb-3"
+                 controls="controls"
+                 tal:condition="python:view.is_audiotype()"
+          >
+            <source tal:attributes="
+                      src python: download_url;
+                      type python: content_type;
+                    " />
+            <tal:icon tal:replace="structure python:icons.tag(mimetype_icon, tag_class='icon-x4 mb-2')" />
+            <div class="small text-muted"
+                 i18n:translate="embedded_audio_not_supported"
+            >Sorry, your browser doesn't support embedded audio.</div>
+          </audio>
+
+          <div class="h5 mb-2">
+            <a href="${python:download_url}"
+               tal:content="python: filename"
+            >Filename</a>
+          </div>
+
+          <div class="metadata d-flex justify-content-center text-muted small">
+            <div class="px-2">
+              <tal:icon tal:replace="structure python:icons.tag(mimetype_icon, tag_class='icon-inline', tag_alt=content_type)" />
+              <span tal:replace="python: content_type">image/jpeg</span>
+            </div>
+            <div class="px-2">
+              <tal:icon tal:replace="structure python:icons.tag('file-binary', tag_class='icon-inline', tag_alt='Size')" />
+              <span tal:define="
+                      size python: view.human_readable_size();
+                    "
+                    tal:content="python: size"
+              >1000 kB</span>
+            </div>
+          </div>
+
+        </section>
+
+        <section class="section section-actions">
+          <a class="btn btn-primary download"
+             href="${python:download_url}"
+             i18n:translate=""
+          >Download</a>
+        </section>
 
-</metal:block>
-</metal:content-core>
+      </metal:block>
+    </metal:content-core>
 
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/full_view.pt` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/document.pt`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-    xmlns:tal="http://xml.zope.org/namespaces/tal"
-    xmlns:metal="http://xml.zope.org/namespaces/metal"
-    xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    metal:use-macro="context/@@main_template/macros/master"
-    i18n:domain="plone">
-<body>
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
+      <metal:content-core define-macro="content-core"
+                          tal:define="
+                            toc python:  getattr(context, 'table_of_contents', False);
+                          "
+      >
+
+        <section id="section-text">
+          <div class="${python: toc and 'pat-autotoc' or ''}"
+               id="parent-fieldname-text"
+               tal:condition="python:getattr(context, 'text', None)"
+               tal:content="structure python:context.text.output_relative_to(view.context)"
+          >
+      Text
+          </div>
+        </section>
 
-<metal:content-core fill-slot="content-core">
-<metal:block define-macro="content-core" tal:define="uuid context/@@uuid | nothing">
+      </metal:content-core>
+    </metal:content-core>
 
-  <metal:listing use-macro="context/@@listing_view/macros/content-core">
-    <metal:entries fill-slot="entries">
-
-      <metal:block use-macro="context/@@listing_view/macros/entries">
-
-        <metal:entry fill-slot="entry" tal:condition="python: item.UID != uuid">
-          <div tal:define="obj item/getObject;" tal:replace="structure obj/@@full_view_item | nothing" />
-        </metal:entry>
-
-      </metal:block>
-
-    </metal:entries>
-  </metal:listing>
-
-</metal:block>
-</metal:content-core>
-
-</body>
+  </body>
 </html>
```

#### html2text {}

```diff
@@ -1,2 +1,3 @@
 
+Text
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/full_view_item.pt` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/full_view_item.pt`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,91 @@
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-    xmlns:tal="http://xml.zope.org/namespaces/tal"
-    xmlns:metal="http://xml.zope.org/namespaces/metal"
-    xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    i18n:domain="plone"
-    tal:omit-tag="">
-<body tal:omit-tag="">
-
-  <div class="item"
-       tal:define="item_macro nocall:view/item_macros/content-core|nothing;
-                   item_url view/item_url;
-                   rendering_error python:[];">
-
-    <div tal:replace="structure provider:plone.abovecontenttitle" />
-
-    <h1>
-      <a class="summary url" tal:content="context/Title" tal:attributes="href item_url;">
+<html xmlns="http://www.w3.org/1999/xhtml"
+      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      xml:lang="en"
+      tal:omit-tag=""
+      i18n:domain="plone"
+>
+  <body tal:omit-tag="">
+
+    <div class="item"
+         tal:define="
+           item_macro nocall:view/item_macros/content-core|nothing;
+           item_url view/item_url;
+           rendering_error python:[];
+         "
+    >
+
+      <div tal:replace="structure provider:plone.abovecontenttitle"></div>
+
+      <h1>
+        <a class="summary url"
+           tal:content="context/Title"
+           tal:attributes="
+             href item_url;
+           "
+        >
         Title
-      </a>
-    </h1>
+        </a>
+      </h1>
 
-    <div tal:replace="structure provider:plone.belowcontenttitle" />
+      <div tal:replace="structure provider:plone.belowcontenttitle"></div>
 
-    <p class="lead" tal:content="context/Description" tal:condition="context/Description">
+      <p class="lead"
+         tal:condition="context/Description"
+         tal:content="context/Description"
+      >
       Description
-    </p>
-
-    <section id="section-item" class="mb-5" tal:condition="item_macro">
-
-      <div tal:replace="structure provider:plone.abovecontentbody" />
+      </p>
 
-      <div tal:define="view nocall:view/default_view;
-                       plone_view context/@@plone;
-                       icons python:context.restrictedTraverse('@@iconresolver');
-                       portal_state context/@@plone_portal_state;
-                       context_state context/@@plone_context_state;
-                       plone_layout context/@@plone_layout;
-                       lang portal_state/language;
-                       dummy python: plone_layout.mark_view(view);
-                       portal_url portal_state/portal_url;
-                       checkPermission nocall: context/portal_membership/checkPermission;
-                       site_properties context/portal_properties/site_properties;">
+      <section class="mb-5"
+               id="section-item"
+               tal:condition="item_macro"
+      >
+
+        <div tal:replace="structure provider:plone.abovecontentbody"></div>
+
+        <div tal:define="
+               view nocall:view/default_view;
+               plone_view context/@@plone;
+               icons python:context.restrictedTraverse('@@iconresolver');
+               portal_state context/@@plone_portal_state;
+               context_state context/@@plone_context_state;
+               plone_layout context/@@plone_layout;
+               lang portal_state/language;
+               dummy python: plone_layout.mark_view(view);
+               portal_url portal_state/portal_url;
+               checkPermission nocall: context/portal_membership/checkPermission;
+               site_properties context/portal_properties/site_properties;
+             ">
 
-        <div metal:use-macro="item_macro">
+          <div metal:use-macro="item_macro">
           content
-        </div>
-
-      </div>
+          </div>
 
-      <div tal:replace="structure provider:plone.belowcontentbody" />
+        </div>
 
-    </section>
+        <div tal:replace="structure provider:plone.belowcontentbody"></div>
 
-    <tal:block tal:condition="rendering_error">
-      <!-- Error rendering item macro -->
-    </tal:block>
+      </section>
 
-    <p class="more" tal:condition="python:not(item_macro) or rendering_error">
-      <a tal:attributes="href item_url" i18n:translate="read_more">
+      <tal:block tal:condition="rendering_error">
+        <!-- Error rendering item macro -->
+      </tal:block>
+
+      <p class="more"
+         tal:condition="python:not(item_macro) or rendering_error"
+      >
+        <a tal:attributes="
+             href item_url;
+           "
+           i18n:translate="read_more"
+        >
         Read More&hellip;
-      </a>
-    </p>
+        </a>
+      </p>
 
-  </div>
-</body>
+    </div>
+  </body>
 </html>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/image.pt` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/image.pt`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,88 @@
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
-<metal:block define-macro="content-core"
-             tal:define="content_type python: context.image.contentType;
-                         size context/image/getSize;
-                         image_dimension context/image/getImageSize;
-                         use_MB python: size > 1024*1024;
-                         dimension python: str(image_dimension[0])+'x'+str(image_dimension[1]);
-                         filename python: context.image.filename;
-                         mimetype_icon python: 'mimetype-' + content_type;
-                         download_url python: '{}/@@download/image/{}'.format(context.absolute_url(), filename)
-                                                     ">
-
-  <section class="section section-main">
-    <figure class="figure">
-      <a tal:attributes="href string:${context/@@plone_context_state/object_url}/image_view_fullscreen"
-         tal:define="scale context/@@images; img_tag python:scale.tag('image', scale='large', css_class='figure-img img-fluid')"
-         tal:on-error="string: Image cannot be displayed">
-        <img tal:replace="structure img_tag" />
-      </a>
-    </figure>
-
-    <div class="h5 mb-2">
-      <a href="${python:download_url}" tal:content="python: filename">Filename</a>
-    </div>
-    <div class="metadata d-flex justify-content-center text-muted small">
-      <div class="px-2">
-        <tal:icon tal:replace="structure python:icons.tag(mimetype_icon, tag_class='icon-inline', tag_alt=content_type)" />
-        <span i18n:translate="image_kind_label" class="d-none">Type</span>
-        <span tal:replace="python: content_type">image/jpeg</span>
-      </div>
-      <div class="px-2">
-        <tal:icon tal:replace="structure python:icons.tag('aspect-ratio', tag_class='icon-inline', tag_alt='Dimension')" />
-        <span i18n:translate="image_dimension_label" class="d-none">Dimension</span>
-        <span tal:replace="python: dimension">400x300</span>
-      </div>
-      <div class="px-2">
-        <tal:icon tal:replace="structure python:icons.tag('file-binary', tag_class='icon-inline', tag_alt='Size')" />
-        <span i18n:translate="image_size_label" class="d-none">File size</span>
-        <tal:MB condition="use_MB">${python:round(size/1024/1024, 1)} MB</tal:MB>
-        <tal:KB condition="not: use_MB">${python:round(size/1024, 1)} KB</tal:KB>
-      </div>
-    </div>
-
-  </section>
-
-  <section class="section section-actions">
-    <a class="btn btn-primary download" href="${python:download_url}" i18n:translate="">Download</a>
-    <a class="btn btn-primary fullscreen" href="${context/@@plone_context_state/object_url}/image_view_fullscreen"><span i18n:translate="label_click_to_view_full_image">View full-size image</span></a>
-  </section>
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
+      <metal:block define-macro="content-core"
+                   tal:define="
+                     content_type python: context.image.contentType;
+                     size context/image/getSize;
+                     image_dimension context/image/getImageSize;
+                     use_MB python: size &gt; 1024*1024;
+                     dimension python: str(image_dimension[0])+'x'+str(image_dimension[1]);
+                     filename python: context.image.filename;
+                     mimetype_icon python: 'mimetype-' + content_type;
+                     download_url python: '{}/@@download/image/{}'.format(context.absolute_url(), filename);
+                   "
+      >
+
+        <section class="section section-main">
+          <figure class="figure">
+            <a tal:define="
+                 scale context/@@images;
+                 img_tag python:scale.tag('image', scale='large', css_class='figure-img img-fluid');
+               "
+               tal:attributes="
+                 href string:${context/@@plone_context_state/object_url}/image_view_fullscreen;
+               "
+               tal:on-error="string: Image cannot be displayed"
+            >
+              <img tal:replace="structure img_tag" />
+            </a>
+          </figure>
+
+          <div class="h5 mb-2">
+            <a href="${python:download_url}"
+               tal:content="python: filename"
+            >Filename</a>
+          </div>
+          <div class="metadata d-flex justify-content-center text-muted small">
+            <div class="px-2">
+              <tal:icon tal:replace="structure python:icons.tag(mimetype_icon, tag_class='icon-inline', tag_alt=content_type)" />
+              <span class="d-none"
+                    i18n:translate="image_kind_label"
+              >Type</span>
+              <span tal:replace="python: content_type">image/jpeg</span>
+            </div>
+            <div class="px-2">
+              <tal:icon tal:replace="structure python:icons.tag('aspect-ratio', tag_class='icon-inline', tag_alt='Dimension')" />
+              <span class="d-none"
+                    i18n:translate="image_dimension_label"
+              >Dimension</span>
+              <span tal:replace="python: dimension">400x300</span>
+            </div>
+            <div class="px-2">
+              <tal:icon tal:replace="structure python:icons.tag('file-binary', tag_class='icon-inline', tag_alt='Size')" />
+              <span class="d-none"
+                    i18n:translate="image_size_label"
+              >File size</span>
+              <tal:mb condition="use_MB">${python:round(size/1024/1024, 1)} MB</tal:mb>
+              <tal:kb condition="not: use_MB">${python:round(size/1024, 1)} KB</tal:kb>
+            </div>
+          </div>
+
+        </section>
+
+        <section class="section section-actions">
+          <a class="btn btn-primary download"
+             href="${python:download_url}"
+             i18n:translate=""
+          >Download</a>
+          <a class="btn btn-primary fullscreen"
+             href="${context/@@plone_context_state/object_url}/image_view_fullscreen"
+          ><span i18n:translate="label_click_to_view_full_image">View full-size image</span></a>
+        </section>
 
 
-</metal:block>
-</metal:content-core>
+      </metal:block>
+    </metal:content-core>
 
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/image_view_fullscreen.pt` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/image_view_fullscreen.pt`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 <!DOCTYPE html>
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-    xmlns:tal="http://xml.zope.org/namespaces/tal"
-    xmlns:metal="http://xml.zope.org/namespaces/metal"
-    xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-    lang="en"
-    i18n:domain="plone">
-<head>
-  <metal:block tal:define="dummy python:request.RESPONSE.setHeader('Content-Type', 'text/html;;charset=utf-8')" />
-  <meta name="viewport" content="width=device-width, initial-scale=1">
-  <title tal:content="context/Title">Title</title>
-  <style type="text/css" media="screen">
+<html xmlns="http://www.w3.org/1999/xhtml"
+      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
+      lang="en"
+      xml:lang="en"
+      i18n:domain="plone"
+>
+  <head>
+    <metal:block tal:define="
+                   dummy python:request.RESPONSE.setHeader('Content-Type', 'text/html;;charset=utf-8');
+                 " />
+    <meta name="viewport"
+          content="width=device-width, initial-scale=1"
+    />
+    <title tal:content="context/Title">Title</title>
+    <style media="screen"
+           type="text/css"
+    >
 
     body {
       font-family: Helvetica, Arial, sans-serif;
       font-size: 14px;
       padding: 0;
       margin: 0;
     }
@@ -38,28 +46,40 @@
       border: 0;
       display: block;
       margin: 0 auto;
       max-width: 100%;
       height: auto;
     }
 
-  </style>
-</head>
+    </style>
+  </head>
 
-<body>
-  <div id="content-core" tal:condition="context/@@images">
-    <tal:block define="referer request/HTTP_REFERER;
-                       url_tool nocall:context/portal_url;
-                       referer python:referer if referer and url_tool.isURLInPortal(referer) else '';">
-    <a tal:attributes="href referer" tal:condition="referer">
-      <tal:block replace="structure context/@@images/image" />
-      <span i18n:translate="label_back_to_site">Back to site</span>
-    </a>
-    <a tal:attributes="href python:url_tool()" tal:condition="not: referer">
-      <tal:block replace="structure context/@@images/image" />
-      <span i18n:translate="label_home">Home</span>
-    </a>
-  </tal:block>
-  </div>
-</body>
+  <body>
+    <div id="content-core"
+         tal:condition="context/@@images"
+    >
+      <tal:block define="
+                   referer request/HTTP_REFERER;
+                   url_tool nocall:context/portal_url;
+                   referer python:referer if referer and url_tool.isURLInPortal(referer) else '';
+                 ">
+        <a tal:condition="referer"
+           tal:attributes="
+             href referer;
+           "
+        >
+          <tal:block replace="structure context/@@images/image" />
+          <span i18n:translate="label_back_to_site">Back to site</span>
+        </a>
+        <a tal:condition="not: referer"
+           tal:attributes="
+             href python:url_tool();
+           "
+        >
+          <tal:block replace="structure context/@@images/image" />
+          <span i18n:translate="label_home">Home</span>
+        </a>
+      </tal:block>
+    </div>
+  </body>
 
 </html>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/link.pt` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/link.pt`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,69 @@
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
-<metal:block define-macro="content-core"
-             tal:define="external python:view.url().startswith('http');
-                         mail python:view.url().startswith('mailto');
-                         link python: not external and not mail;
-                         display_link python: view.display_link()">
-
-
-  <section class="section section-main">
-    <div>
-      <tal:icon tal:condition="link"
-        tal:replace="structure python:icons.tag('plone-link', tag_class='icon-x4 mb-2')" />
-      <tal:icon tal:condition="external"
-        tal:replace="structure python:icons.tag('plone-link/external', tag_class='icon-x4 mb-2')" />
-      <tal:icon tal:condition="mail"
-        tal:replace="structure python:icons.tag('plone-link/mail', tag_class='icon-x4 mb-2')" />
-    </div>
-    <div class="h5 mb-2">
-      <a href="" tal:attributes="href python: view.absolute_target_url()" 
-         tal:content="python: display_link['title']">remote url</a>
-    </div>
-    <div class="metadata d-flex justify-content-center text-muted small"
-        tal:condition="python: display_link['meta']">
-      <div tal:replace="python: display_link['meta']"></div>
-    </div>
-
-    <div class="info-redirect small text-muted mt-4" 
-      tal:define="redirect_links python:context.portal_registry['plone.redirect_links']" 
-      tal:condition="python: redirect_links and checkPermission('Modify portal content', context)">
-      <span tal:omit-tag="" i18n:translate="message_permissions_blocking_link_redirect">
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
+      <metal:block define-macro="content-core"
+                   tal:define="
+                     external python:view.url().startswith('http');
+                     mail python:view.url().startswith('mailto');
+                     link python: not external and not mail;
+                     display_link python: view.display_link();
+                   "
+      >
+
+
+        <section class="section section-main">
+          <div>
+            <tal:icon tal:condition="link"
+                      tal:replace="structure python:icons.tag('plone-link', tag_class='icon-x4 mb-2')"
+            />
+            <tal:icon tal:condition="external"
+                      tal:replace="structure python:icons.tag('plone-link/external', tag_class='icon-x4 mb-2')"
+            />
+            <tal:icon tal:condition="mail"
+                      tal:replace="structure python:icons.tag('plone-link/mail', tag_class='icon-x4 mb-2')"
+            />
+          </div>
+          <div class="h5 mb-2">
+            <a href=""
+               tal:content="python: display_link['title']"
+               tal:attributes="
+                 href python: view.absolute_target_url();
+               "
+            >remote url</a>
+          </div>
+          <div class="metadata d-flex justify-content-center text-muted small"
+               tal:condition="python: display_link['meta']"
+          >
+            <div tal:replace="python: display_link['meta']"></div>
+          </div>
+
+          <div class="info-redirect small text-muted mt-4"
+               tal:define="
+                 redirect_links python:context.portal_registry['plone.redirect_links'];
+               "
+               tal:condition="python: redirect_links and checkPermission('Modify portal content', context)"
+          >
+            <span tal:omit-tag=""
+                  i18n:translate="message_permissions_blocking_link_redirect"
+            >
         You see this page because you have permission to edit this link.
         Others will be immediately redirected to the link's target URL.
-      </span>
-    </div>
+            </span>
+          </div>
 
-  </section>
+        </section>
 
-</metal:block>
-</metal:content-core>
+      </metal:block>
+    </metal:content-core>
 
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/listing.pt` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing.pt`

 * *Files 13% similar despite different names*

```diff
@@ -1,148 +1,194 @@
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
-  <div metal:define-macro="text-field-view"
-      id="parent-fieldname-text" class="stx"
-      tal:define="text python:view.text"
-      tal:condition="python:text"
-      tal:attributes="class python:view.text_class">
-    <div metal:define-slot="inside" tal:replace="structure text">The body</div>
-  </div>
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
+        <div class="stx"
+             id="parent-fieldname-text"
+             metal:define-macro="text-field-view"
+             tal:define="
+               text python:view.text;
+             "
+             tal:condition="python:text"
+             tal:attributes="
+               class python:view.text_class;
+             "
+        >
+          <div metal:define-slot="inside"
+               tal:replace="structure text"
+          >The body</div>
+        </div>
 
 
-  <metal:listingmacro define-macro="listing">
-    <tal:results define="batch python:view.batch();
+        <metal:listingmacro define-macro="listing">
+          <tal:results define="
+                         batch python:view.batch();
                          thumb_scale_list python:view.get_thumb_scale_list();
                          thumb_scale_table python:view.get_thumb_scale_table();
                          thumb_scale_summary python:view.get_thumb_scale_summary();
                          img_class python:'thumb-{} image-responsive'.format(thumb_scale_list);
-                         showicons python:view.show_icons()">
-      <tal:listing condition="python:batch">
-        <div class="entries" metal:define-slot="entries"
-            tal:define="portal python:portal_state.portal();
-                        image_scale portal/@@image_scale">
-
-          <tal:repeat repeat="item python:batch" metal:define-macro="entries">
-            <tal:block tal:define="obj python:item.getObject();
-                item_url python:item.getURL();
-                item_id python:item.getId();
-                item_title python:item.Title();
-                item_title python:item_title or item_id;
-                item_description python:item.Description();
-                item_type python:item.PortalType();
-                item_modified python:item.ModificationDate();
-                item_created python:item.CreationDate();
-                item_wf_state python:item.review_state();
-                item_wf_state_class python:'state-' + view.normalizeString(item_wf_state);
-                item_creator python:item.Creator();
-                item_link python:item_type in view.use_view_action and item_url+'/view' or item_url;
-                item_is_event python:view.is_event(obj);
-                item_has_image python:item.getIcon;
-                item_type_class python:('contenttype-' + view.normalizeString(item_type)) if showicons else '' ;
-                ">
-              <metal:block define-slot="entry">
-
-                <article class="mb-3 row">
-
-                  <div class="col" metal:define-macro="listitem">
-
-                      <div class="mb-1">
-                        <a tal:attributes="href python:item_link; class string:$item_type_class $item_wf_state_class url; title item_type" tal:content="python:item_title">
+                         showicons python:view.show_icons();
+                       ">
+            <tal:listing condition="python:batch">
+              <div class="entries"
+                   metal:define-slot="entries"
+                   tal:define="
+                     portal python:portal_state.portal();
+                     image_scale portal/@@image_scale;
+                   "
+              >
+
+                <tal:repeat metal:define-macro="entries"
+                            repeat="item python:batch"
+                >
+                  <tal:block tal:define="
+                               obj python:item.getObject();
+                               item_url python:item.getURL();
+                               item_id python:item.getId();
+                               item_title python:item.Title();
+                               item_title python:item_title or item_id;
+                               item_description python:item.Description();
+                               item_type python:item.PortalType();
+                               item_modified python:item.ModificationDate();
+                               item_created python:item.CreationDate();
+                               item_wf_state python:item.review_state();
+                               item_wf_state_class python:'state-' + view.normalizeString(item_wf_state);
+                               item_creator python:item.Creator();
+                               item_link python:item_type in view.use_view_action and item_url+'/view' or item_url;
+                               item_is_event python:view.is_event(obj);
+                               item_has_image python:item.getIcon;
+                               item_type_class python:('contenttype-' + view.normalizeString(item_type)) if showicons else '';
+                             ">
+                    <metal:block define-slot="entry">
+
+                      <article class="mb-3 row">
+
+                        <div class="col"
+                             metal:define-macro="listitem"
+                        >
+
+                          <div class="mb-1">
+                            <a tal:content="python:item_title"
+                               tal:attributes="
+                                 href python:item_link;
+                                 class string:$item_type_class $item_wf_state_class url;
+                                 title item_type;
+                               "
+                            >
                           Item Title
-                        </a>
-                      </div>
+                            </a>
+                          </div>
 
-                      <metal:block metal:define-macro="document_byline">
-                      <div class="mb-1">
+                          <metal:block metal:define-macro="document_byline">
+                            <div class="mb-1">
 
-                        <tal:event condition="python:item_is_event">
-                          <tal:date tal:replace="structure python:view.formatted_date(obj)"/>
-                          <span tal:condition="python:obj.location" i18n:translate="label_event_byline_location">
+                              <tal:event condition="python:item_is_event">
+                                <tal:date tal:replace="structure python:view.formatted_date(obj)" />
+                                <span tal:condition="python:obj.location"
+                                      i18n:translate="label_event_byline_location"
+                                >
                             &mdash;
-                            <span tal:content="python:obj.location" class="location" i18n:name="location">Oslo</span>
-                          </span>
+                                  <span class="location"
+                                        tal:content="python:obj.location"
+                                        i18n:name="location"
+                                  >Oslo</span>
+                                </span>
                           &mdash;
-                        </tal:event>
+                              </tal:event>
 
-                        <tal:byline condition="python:view.show_about">
-                          <tal:name tal:condition="python:item_creator"
-                              tal:define="author python:view.pas_member.info(item_creator);
-                                          creator_short_form python:author.get('username');
-                                          creator_long_form string:?author=$${python:author.username};
-                                          creator_is_openid python:'/' in creator_short_form;
-                                          creator_id python:(creator_short_form, creator_long_form)[creator_is_openid];">
-                          <span i18n:translate="label_by_author">
+                              <tal:byline condition="python:view.show_about">
+                                <tal:name tal:define="
+                                            author python:view.pas_member.info(item_creator);
+                                            creator_short_form python:author.get('username');
+                                            creator_long_form string:?author=$${python:author.username};
+                                            creator_is_openid python:'/' in creator_short_form;
+                                            creator_id python:(creator_short_form, creator_long_form)[creator_is_openid];
+                                          "
+                                          tal:condition="python:item_creator"
+                                >
+                                  <span i18n:translate="label_by_author">
                             by
-                            <a tal:attributes="href string:${view/navigation_root_url}/author/${item_creator}"
-                                tal:content="python: author.get('name_or_id')"
-                                tal:omit-tag="python: not author"
-                                i18n:name="author">
+                                    <a tal:content="python: author.get('name_or_id')"
+                                       tal:omit-tag="python: not author"
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
 
-                          <tal:modified condition="python:item_type != 'Event'">
+                                <tal:modified condition="python:item_type != 'Event'">
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
+                                  </tal:comment>
+                                </metal:description>
 
-                        </tal:byline>
-                      </div>
-                      </metal:block>
-
-                      <p class="me-3" tal:condition="python:item_description" tal:content="python:item_description">
+                              </tal:byline>
+                            </div>
+                          </metal:block>
+
+                          <p class="me-3"
+                             tal:condition="python:item_description"
+                             tal:content="python:item_description"
+                          >
                         description
-                      </p>
-                  </div>
-
-                  <div class="col-3 text-end" tal:condition="python:item_has_image and thumb_scale_list">
-                    <a tal:attributes="href python:item_link;">
-                      <img tal:replace="structure python:image_scale.tag(item, 'image', scale=thumb_scale_list, css_class=img_class, loading='lazy')" />
-                    </a>
-                  </div>
-                </article>
-
-              </metal:block>
-            </tal:block>
-          </tal:repeat>
-        </div>
-
-        <div metal:use-macro="context/batch_macros/macros/navigation" />
-
-      </tal:listing>
+                          </p>
+                        </div>
 
-      <metal:empty metal:define-slot="no_items_in_listing">
-        <p class="discreet"
-            tal:condition="python: not batch"
-            tal:content="python: view.no_items_message">
+                        <div class="col-3 text-end"
+                             tal:condition="python:item_has_image and thumb_scale_list"
+                        >
+                          <a tal:attributes="
+                               href python:item_link;
+                             ">
+                            <img tal:replace="structure python:image_scale.tag(item, 'image', scale=thumb_scale_list, css_class=img_class, loading='lazy')" />
+                          </a>
+                        </div>
+                      </article>
+
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
+                 tal:condition="python: not batch"
+                 tal:content="python: view.no_items_message"
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

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/listing_summary.pt` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing_summary.pt`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,91 @@
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
-<metal:block use-macro="context/@@listing_view/macros/content-core">
-
-  <metal:entries fill-slot="entries">
-    <metal:block use-macro="context/@@listing_view/macros/entries" tal:define="portal context/@@plone_portal_state/portal; image_scale portal/@@image_scale">
-
-      <metal:entry fill-slot="entry">
-
-        <article class="row mb-3">
-
-          <div class="col">
-
-          <h2 metal:define-macro="listitem">
-            <a class="summary url" tal:attributes="href item_link; title item_type" tal:content="item_title">
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
+        <metal:block use-macro="context/@@listing_view/macros/content-core">
+
+          <metal:entries fill-slot="entries">
+            <metal:block use-macro="context/@@listing_view/macros/entries"
+                         tal:define="
+                           portal context/@@plone_portal_state/portal;
+                           image_scale portal/@@image_scale;
+                         "
+            >
+
+              <metal:entry fill-slot="entry">
+
+                <article class="row mb-3">
+
+                  <div class="col">
+
+                    <h2 metal:define-macro="listitem">
+                      <a class="summary url"
+                         tal:content="item_title"
+                         tal:attributes="
+                           href item_link;
+                           title item_type;
+                         "
+                      >
               Item Title
-            </a>
-          </h2>
-
-          <div class="mb-3">
-            <div metal:use-macro="context/@@listing_view/macros/document_byline"></div>
-          </div>
+                      </a>
+                    </h2>
 
-          <div class="mb-1" tal:condition="item_description">
-            <span class="description" tal:content="item_description">
+                    <div class="mb-3">
+                      <div metal:use-macro="context/@@listing_view/macros/document_byline"></div>
+                    </div>
+
+                    <div class="mb-1"
+                         tal:condition="item_description"
+                    >
+                      <span class="description"
+                            tal:content="item_description"
+                      >
               description
-            </span>
-          </div>
+                      </span>
+                    </div>
 
-          <div class="mb-1">
-            <a tal:attributes="href item_link" i18n:translate="read_more">
+                    <div class="mb-1">
+                      <a tal:attributes="
+                           href item_link;
+                         "
+                         i18n:translate="read_more"
+                      >
               Read More&hellip;
-            </a>
-          </div>
+                      </a>
+                    </div>
 
-          </div>
+                  </div>
 
-          <div class="col-3"
-               tal:condition="python: item_has_image and thumb_scale_summary">
-            <a tal:attributes="href item_link">
-              <img tal:replace="structure python:image_scale.tag(item, 'image', scale=thumb_scale_summary, css_class='image-responsive thumb-' + thumb_scale_summary, loading='lazy')" />
-            </a>
-          </div>
+                  <div class="col-3"
+                       tal:condition="python: item_has_image and thumb_scale_summary"
+                  >
+                    <a tal:attributes="
+                         href item_link;
+                       ">
+                      <img tal:replace="structure python:image_scale.tag(item, 'image', scale=thumb_scale_summary, css_class='image-responsive thumb-' + thumb_scale_summary, loading='lazy')" />
+                    </a>
+                  </div>
 
-        </article>
+                </article>
 
-      </metal:entry>
-    </metal:block>
-  </metal:entries>
+              </metal:entry>
+            </metal:block>
+          </metal:entries>
 
-</metal:block>
+        </metal:block>
 
-</metal:block>
-</metal:content-core>
+      </metal:block>
+    </metal:content-core>
 
-</body>
+  </body>
 </html>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/templates/listing_tabular.pt` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/templates/listing_tabular.pt`

 * *Files 25% similar despite different names*

```diff
@@ -1,111 +1,177 @@
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
-  <div metal:define-macro="text-field-view" id="parent-fieldname-text" class="stx" tal:define="text python:view.text" tal:condition="python:text" tal:attributes="class python:view.text_class">
-    <div metal:define-slot="inside" tal:replace="structure python:text">The body</div>
-  </div>
-
-  <metal:listingmacro define-macro="listing">
-  <tal:results define="batch python:view.batch()">
-    <tal:listing condition="python:batch">
-
-      <div metal:use-macro="context/batch_macros/macros/navigation" />
-
-      <div class="table-responsive">
-
-        <table class="table table-striped" tal:define="tabular_fields view/tabular_fields; thumb_scale_table python:view.get_thumb_scale_table(); img_class python:'thumb-%s float-end' % thumb_scale_table; showicons  python:view.show_icons();" summary="Content listing" i18n:attributes="summary summary_content_listing;">
-
-          <thead>
-            <tr>
-              <th class="text-nowrap"></th>
-              <th class="text-nowrap" tal:repeat="field tabular_fields" tal:content="python:view.tabular_field_label(field)">Field name</th>
-              <th class="text-nowrap" i18n:translate="image" tal:condition="python:thumb_scale_table">Image</th>
-            </tr>
-          </thead>
-
-          <tbody tal:define="portal python:portal_state.portal(); image_scale portal/@@image_scale">
-            <tal:entries tal:repeat="item python:batch">
-              <tal:block tal:define="item_url python:item.getURL();
-                                      item_id python:item.getId();
-                                      item_title python:item.Title();
-                                      item_title python:item_title or item_id;
-                                      item_type python:item.PortalType();
-                                      item_type_class python:'contenttype/' + view.normalizeString(item_type) if showicons else '';
-                                      item_wf_state python:item.review_state();
-                                      item_wf_state_class python:'state-' + view.normalizeString(item_wf_state);
-                                      item_creator python:item.Creator();
-                                      item_has_image python:item.getIcon;
-                                      item_link python:item_type in view.use_view_action and item_url+'/view' or item_url;
-                                      item_mime_type python:item.mime_type;
-                                      item_mime_type_icon python: 'mimetype-' + item_mime_type;
-                                      ">
-
-                <tr metal:define-macro="listitem">
-
-                  <td>
-                    <tal:icon tal:condition="python: item_type == 'File'" tal:replace="structure python:icons.tag(item_mime_type_icon)" />
-                    <tal:icon tal:condition="python: item_type != 'File'" tal:replace="structure python:icons.tag(item_type_class)" />
-                  </td>
-
-                  <tal:block tal:repeat="field python:tabular_fields">
-
-                  <td class="text-nowrap" tal:condition="python:field not in ['Title', 'Creator', 'getIcon']" tal:define="field_data python:view.tabular_fielddata(item, field)">
-                    <tal:block tal:replace="python: field_data.get('value')" />
-                  </td>
-
-                  <td class="text-nowrap" tal:condition="python:field == 'Title'">
-                    <a tal:attributes="href python:item_link; class string:$item_type_class $item_wf_state_class url; title python:item_type" tal:content="python: item_title">
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
+        <div class="stx"
+             id="parent-fieldname-text"
+             metal:define-macro="text-field-view"
+             tal:define="
+               text python:view.text;
+             "
+             tal:condition="python:text"
+             tal:attributes="
+               class python:view.text_class;
+             "
+        >
+          <div metal:define-slot="inside"
+               tal:replace="structure python:text"
+          >The body</div>
+        </div>
+
+        <metal:listingmacro define-macro="listing">
+          <tal:results define="
+                         batch python:view.batch();
+                       ">
+            <tal:listing condition="python:batch">
+
+              <div metal:use-macro="context/batch_macros/macros/navigation"></div>
+
+              <div class="table-responsive">
+
+                <table class="table table-striped"
+                       summary="Content listing"
+                       tal:define="
+                         tabular_fields view/tabular_fields;
+                         thumb_scale_table python:view.get_thumb_scale_table();
+                         img_class python:'thumb-%s float-end' % thumb_scale_table;
+                         showicons  python:view.show_icons();
+                       "
+                       i18n:attributes="summary summary_content_listing;"
+                >
+
+                  <thead>
+                    <tr>
+                      <th class="text-nowrap"></th>
+                      <th class="text-nowrap"
+                          tal:repeat="field tabular_fields"
+                          tal:content="python:view.tabular_field_label(field)"
+                      >Field name</th>
+                      <th class="text-nowrap"
+                          tal:condition="python:thumb_scale_table"
+                          i18n:translate="image"
+                      >Image</th>
+                    </tr>
+                  </thead>
+
+                  <tbody tal:define="
+                           portal python:portal_state.portal();
+                           image_scale portal/@@image_scale;
+                         ">
+                    <tal:entries tal:repeat="item python:batch">
+                      <tal:block tal:define="
+                                   item_url python:item.getURL();
+                                   item_id python:item.getId();
+                                   item_title python:item.Title();
+                                   item_title python:item_title or item_id;
+                                   item_type python:item.PortalType();
+                                   item_type_class python:'contenttype/' + view.normalizeString(item_type) if showicons else '';
+                                   item_wf_state python:item.review_state();
+                                   item_wf_state_class python:'state-' + view.normalizeString(item_wf_state);
+                                   item_creator python:item.Creator();
+                                   item_has_image python:item.getIcon;
+                                   item_link python:item_type in view.use_view_action and item_url+'/view' or item_url;
+                                   item_mime_type python:item.mime_type;
+                                   item_mime_type_icon python: 'mimetype-' + item_mime_type;
+                                 ">
+
+                        <tr metal:define-macro="listitem">
+
+                          <td>
+                            <tal:icon tal:condition="python: item_type == 'File'"
+                                      tal:replace="structure python:icons.tag(item_mime_type_icon)"
+                            />
+                            <tal:icon tal:condition="python: item_type != 'File'"
+                                      tal:replace="structure python:icons.tag(item_type_class)"
+                            />
+                          </td>
+
+                          <tal:block tal:repeat="field python:tabular_fields">
+
+                            <td class="text-nowrap"
+                                tal:define="
+                                  field_data python:view.tabular_fielddata(item, field);
+                                "
+                                tal:condition="python:field not in ['Title', 'Creator', 'getIcon']"
+                            >
+                              <tal:block tal:replace="python: field_data.get('value')" />
+                            </td>
+
+                            <td class="text-nowrap"
+                                tal:condition="python:field == 'Title'"
+                            >
+                              <a tal:content="python: item_title"
+                                 tal:attributes="
+                                   href python:item_link;
+                                   class string:$item_type_class $item_wf_state_class url;
+                                   title python:item_type;
+                                 "
+                              >
                       Item Title
-                    </a>
-                  </td>
+                              </a>
+                            </td>
 
-                  <td class="text-nowrap" tal:condition="python:field == 'Creator'" tal:define="author python:view.pas_member.info(item_creator); name python:author['fullname'] or author['username']">
-                    <a tal:condition="python: author" href="${view/navigation_root_url}/author/${item_creator}">
+                            <td class="text-nowrap"
+                                tal:define="
+                                  author python:view.pas_member.info(item_creator);
+                                  name python:author['fullname'] or author['username'];
+                                "
+                                tal:condition="python:field == 'Creator'"
+                            >
+                              <a href="${view/navigation_root_url}/author/${item_creator}"
+                                 tal:condition="python: author"
+                              >
                       ${name}
-                    </a>
-                  </td>
-
-                  </tal:block>
-
-                  <td>
-                    <a tal:condition="python:item_has_image and thumb_scale_table">
-                      <img tal:attributes="href python: item_link" tal:replace="structure python:image_scale.tag(item, 'image', scale=thumb_scale_table, css_class=img_class, loading='lazy')" />
-                    </a>
-                  </td>
-
-                </tr>
-
-              </tal:block>
-            </tal:entries>
-          </tbody>
-        </table>
-
-      </div>
-
-      <div metal:use-macro="context/batch_macros/macros/navigation" />
+                              </a>
+                            </td>
 
-    </tal:listing>
+                          </tal:block>
 
-    <metal:empty metal:define-slot="no_items_in_listing">
-    <p tal:condition="python: not batch" tal:content="python: view.no_items_message">
+                          <td>
+                            <a tal:condition="python:item_has_image and thumb_scale_table">
+                              <img tal:replace="structure python:image_scale.tag(item, 'image', scale=thumb_scale_table, css_class=img_class, loading='lazy')"
+                                   tal:attributes="
+                                     href python: item_link;
+                                   "
+                              />
+                            </a>
+                          </td>
+
+                        </tr>
+
+                      </tal:block>
+                    </tal:entries>
+                  </tbody>
+                </table>
+
+              </div>
+
+              <div metal:use-macro="context/batch_macros/macros/navigation"></div>
+
+            </tal:listing>
+
+            <metal:empty metal:define-slot="no_items_in_listing">
+              <p tal:condition="python: not batch"
+                 tal:content="python: view.no_items_message"
+              >
       There are currently no items in this folder.
-    </p>
-    </metal:empty>
+              </p>
+            </metal:empty>
 
-  </tal:results>
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

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/browser/utils.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/browser/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/configure.zcml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/configure.zcml`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,38 @@
-<configure xmlns="http://namespaces.zope.org/zope"
-           xmlns:zcml="http://namespaces.zope.org/zcml"
-           xmlns:five="http://namespaces.zope.org/five"
-           xmlns:i18n="http://namespaces.zope.org/i18n"
-           xmlns:gs="http://namespaces.zope.org/genericsetup"
-           xmlns:cmf="http://namespaces.zope.org/cmf"
-           xmlns:plone="http://namespaces.plone.org/plone"
-           i18n_domain="plone">
-
-  <include package="Products.CMFCore" file="meta.zcml" />
-  <include package="Products.GenericSetup" file="meta.zcml" />
-  <include package="plone.behavior" file="meta.zcml"/>
-  <include package="plone.dexterity" file="meta.zcml"/>
-  <include package="plone.app.dexterity" file="meta.zcml"/>
+<configure
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:cmf="http://namespaces.zope.org/cmf"
+    xmlns:five="http://namespaces.zope.org/five"
+    xmlns:gs="http://namespaces.zope.org/genericsetup"
+    xmlns:i18n="http://namespaces.zope.org/i18n"
+    xmlns:plone="http://namespaces.plone.org/plone"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    i18n_domain="plone"
+    >
+
+  <include
+      package="Products.CMFCore"
+      file="meta.zcml"
+      />
+  <include
+      package="Products.GenericSetup"
+      file="meta.zcml"
+      />
+  <include
+      package="plone.behavior"
+      file="meta.zcml"
+      />
+  <include
+      package="plone.dexterity"
+      file="meta.zcml"
+      />
+  <include
+      package="plone.app.dexterity"
+      file="meta.zcml"
+      />
 
   <include package="plone.behavior" />
   <include package="plone.dexterity" />
   <include package="plone.namedfile" />
   <include package="plone.app.contentmenu" />
   <include package="plone.app.dexterity" />
   <include package="plone.app.event" />
@@ -36,11 +53,12 @@
   <include file="permissions.zcml" />
   <include file="subscribers.zcml" />
   <include file="upgrades.zcml" />
 
 
   <utility
       factory=".setuphandlers.HiddenProfiles"
+      provides="plone.base.interfaces.INonInstallable"
       name="plone.app.contenttypes"
-      provides="plone.base.interfaces.INonInstallable" />
+      />
 
 </configure>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/content.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/content.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/indexers.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/indexers.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/indexers.zcml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/indexers.zcml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,54 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:five="http://namespaces.zope.org/five"
-    xmlns:i18n="http://namespaces.zope.org/i18n"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
-    i18n_domain="plone">
+    xmlns:i18n="http://namespaces.zope.org/i18n"
+    i18n_domain="plone"
+    >
 
-  <adapter name="SearchableText" factory=".indexers.SearchableText_collection" />
-  <adapter name="SearchableText" factory=".indexers.SearchableText_document" />
-  <adapter name="SearchableText" factory=".indexers.SearchableText_file" />
-  <adapter name="SearchableText" factory=".indexers.SearchableText_folder" />
-  <adapter name="SearchableText" factory=".indexers.SearchableText_link" />
-  <adapter name="SearchableText" factory=".indexers.SearchableText_news" />
-  <adapter name="getRemoteUrl" factory=".indexers.getRemoteUrl" />
-  <adapter name="getObjSize" factory=".indexers.getObjSize_image" />
-  <adapter name="getObjSize" factory=".indexers.getObjSize_file" />
-  <adapter name="getIcon" factory=".indexers.getIcon" />
-  <adapter name="mime_type" factory=".indexers.mime_type" />
+  <adapter
+      factory=".indexers.SearchableText_collection"
+      name="SearchableText"
+      />
+  <adapter
+      factory=".indexers.SearchableText_document"
+      name="SearchableText"
+      />
+  <adapter
+      factory=".indexers.SearchableText_file"
+      name="SearchableText"
+      />
+  <adapter
+      factory=".indexers.SearchableText_folder"
+      name="SearchableText"
+      />
+  <adapter
+      factory=".indexers.SearchableText_link"
+      name="SearchableText"
+      />
+  <adapter
+      factory=".indexers.SearchableText_news"
+      name="SearchableText"
+      />
+  <adapter
+      factory=".indexers.getRemoteUrl"
+      name="getRemoteUrl"
+      />
+  <adapter
+      factory=".indexers.getObjSize_image"
+      name="getObjSize"
+      />
+  <adapter
+      factory=".indexers.getObjSize_file"
+      name="getObjSize"
+      />
+  <adapter
+      factory=".indexers.getIcon"
+      name="getIcon"
+      />
+  <adapter
+      factory=".indexers.mime_type"
+      name="mime_type"
+      />
 
 </configure>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/interfaces.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/permissions.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/permissions.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/permissions.zcml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/permissions.zcml`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 <configure
-  xmlns="http://namespaces.zope.org/zope"
-  xmlns:zcml="http://namespaces.zope.org/zcml"
-  i18n_domain="plone">
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    i18n_domain="plone"
+    >
 
   <configure zcml:condition="installed AccessControl.security">
 
     <permission
-      id="plone.app.contenttypes.addCollection"
-      title="plone.app.contenttypes: Add Collection"
-      />
-    <permission
-      id="plone.app.contenttypes.addDocument"
-      title="plone.app.contenttypes: Add Document"
-      />
-    <permission
-      id="plone.app.contenttypes.addEvent"
-      title="plone.app.contenttypes: Add Event"
-      />
-    <permission
-      id="plone.app.contenttypes.addFile"
-      title="plone.app.contenttypes: Add File"
-      />
-    <permission
-      id="plone.app.contenttypes.addFolder"
-      title="plone.app.contenttypes: Add Folder"
-      />
-    <permission
-      id="plone.app.contenttypes.addImage"
-      title="plone.app.contenttypes: Add Image"
-      />
-    <permission
-      id="plone.app.contenttypes.addLink"
-      title="plone.app.contenttypes: Add Link"
-      />
-    <permission
-      id="plone.app.contenttypes.addNewsItem"
-      title="plone.app.contenttypes: Add News Item"
-      />
+        id="plone.app.contenttypes.addCollection"
+        title="plone.app.contenttypes: Add Collection"
+        />
+    <permission
+        id="plone.app.contenttypes.addDocument"
+        title="plone.app.contenttypes: Add Document"
+        />
+    <permission
+        id="plone.app.contenttypes.addEvent"
+        title="plone.app.contenttypes: Add Event"
+        />
+    <permission
+        id="plone.app.contenttypes.addFile"
+        title="plone.app.contenttypes: Add File"
+        />
+    <permission
+        id="plone.app.contenttypes.addFolder"
+        title="plone.app.contenttypes: Add Folder"
+        />
+    <permission
+        id="plone.app.contenttypes.addImage"
+        title="plone.app.contenttypes: Add Image"
+        />
+    <permission
+        id="plone.app.contenttypes.addLink"
+        title="plone.app.contenttypes: Add Link"
+        />
+    <permission
+        id="plone.app.contenttypes.addNewsItem"
+        title="plone.app.contenttypes: Add News Item"
+        />
 
   </configure>
 
 </configure>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/content/portlets.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/content/portlets.xml`

 * *Files 26% similar despite different names*

#### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/content/portlets.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/content/portlets.xml`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <portlets>
   <!-- Assign the standard portlets -->
-  <assignment manager="plone.leftcolumn" category="context" key="/" type="portlets.Navigation" name="navigation"/>
-  <assignment manager="plone.rightcolumn" category="context" key="/" type="portlets.News" name="news"/>
+  <assignment category="context" key="/" manager="plone.leftcolumn" name="navigation" type="portlets.Navigation"/>
+  <assignment category="context" key="/" manager="plone.rightcolumn" name="news" type="portlets.News"/>
   <!--  <assignment
      manager="plone.rightcolumn"
      category="context"
      key="/"
      type="portlets.Events"
      name="events"
      />
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/rolemap.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/rolemap.xml`

 * *Files 13% similar despite different names*

#### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/rolemap.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/rolemap.xml`

```diff
@@ -1,56 +1,56 @@
 <?xml version="1.0" encoding="utf-8"?>
 <rolemap>
   <roles>
     <role name="Manager"/>
   </roles>
   <permissions>
-    <permission name="plone.app.contenttypes: Add Collection" acquire="True">
+    <permission acquire="True" name="plone.app.contenttypes: Add Collection">
       <role name="Manager"/>
       <role name="Site Administrator"/>
       <role name="Owner"/>
       <role name="Contributor"/>
     </permission>
-    <permission name="plone.app.contenttypes: Add Document" acquire="True">
+    <permission acquire="True" name="plone.app.contenttypes: Add Document">
       <role name="Manager"/>
       <role name="Site Administrator"/>
       <role name="Owner"/>
       <role name="Contributor"/>
     </permission>
-    <permission name="plone.app.contenttypes: Add Event" acquire="True">
+    <permission acquire="True" name="plone.app.contenttypes: Add Event">
       <role name="Manager"/>
       <role name="Site Administrator"/>
       <role name="Owner"/>
       <role name="Contributor"/>
     </permission>
-    <permission name="plone.app.contenttypes: Add File" acquire="True">
+    <permission acquire="True" name="plone.app.contenttypes: Add File">
       <role name="Manager"/>
       <role name="Site Administrator"/>
       <role name="Owner"/>
       <role name="Contributor"/>
     </permission>
-    <permission name="plone.app.contenttypes: Add Folder" acquire="True">
+    <permission acquire="True" name="plone.app.contenttypes: Add Folder">
       <role name="Manager"/>
       <role name="Site Administrator"/>
       <role name="Owner"/>
       <role name="Contributor"/>
     </permission>
-    <permission name="plone.app.contenttypes: Add Image" acquire="True">
+    <permission acquire="True" name="plone.app.contenttypes: Add Image">
       <role name="Manager"/>
       <role name="Site Administrator"/>
       <role name="Owner"/>
       <role name="Contributor"/>
     </permission>
-    <permission name="plone.app.contenttypes: Add Link" acquire="True">
+    <permission acquire="True" name="plone.app.contenttypes: Add Link">
       <role name="Manager"/>
       <role name="Site Administrator"/>
       <role name="Owner"/>
       <role name="Contributor"/>
     </permission>
-    <permission name="plone.app.contenttypes: Add News Item" acquire="True">
+    <permission acquire="True" name="plone.app.contenttypes: Add News Item">
       <role name="Manager"/>
       <role name="Site Administrator"/>
       <role name="Owner"/>
       <role name="Contributor"/>
     </permission>
   </permissions>
 </rolemap>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Collection.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Folder.xml`

 * *Files 8% similar despite different names*

#### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Collection.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Folder.xml`

```diff
@@ -1,40 +1,39 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="Collection" meta_type="Dexterity FTI" i18n:domain="plone">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="Folder" i18n:domain="plone">
   <!-- Basic properties -->
-  <property i18n:translate="" name="title">Collection</property>
-  <property i18n:translate="" name="description"/>
+  <property name="title" i18n:translate="">Folder</property>
+  <property name="description" i18n:translate=""/>
   <property name="allow_discussion">False</property>
-  <property name="factory">Collection</property>
-  <property name="icon_expr">string:contenttype/collection</property>
+  <property name="factory">Folder</property>
+  <property name="icon_expr">string:contenttype/folder</property>
   <property name="link_target"/>
   <!-- Hierarchy control -->
   <property name="allowed_content_types"/>
   <property name="filter_content_types">False</property>
   <property name="global_allow">True</property>
   <!-- Schema, class and security -->
-  <property name="add_permission">plone.app.contenttypes.addCollection</property>
-  <property name="klass">plone.app.contenttypes.content.Collection</property>
-  <property name="model_file">plone.app.contenttypes.schema:collection.xml</property>
+  <property name="add_permission">plone.app.contenttypes.addFolder</property>
+  <property name="klass">plone.app.contenttypes.content.Folder</property>
+  <property name="model_file">plone.app.contenttypes.schema:folder.xml</property>
   <property name="model_source"/>
   <property name="schema"/>
   <!-- Enabled behaviors -->
   <property name="behaviors" purge="false">
+    <element value="plone.dublincore"/>
     <element value="plone.namefromtitle"/>
-    <element value="plone.collection"/>
     <element value="plone.allowdiscussion"/>
-    <element value="plone.shortname"/>
     <element value="plone.excludefromnavigation"/>
-    <element value="plone.dublincore"/>
-    <element value="plone.richtext"/>
+    <element value="plone.shortname"/>
+    <element value="plone.constraintypes"/>
     <element value="plone.relateditems"/>
-    <element value="plone.locking"/>
+    <element value="plone.nextprevioustoggle"/>
   </property>
   <!-- View information -->
-  <property name="add_view_expr">string:${folder_url}/++add++Collection</property>
+  <property name="add_view_expr">string:${folder_url}/++add++Folder</property>
   <property name="default_view">listing_view</property>
   <property name="default_view_fallback">False</property>
   <property name="immediate_view">view</property>
   <property name="view_methods">
     <element value="album_view"/>
     <element value="event_listing"/>
     <element value="full_view"/>
@@ -44,14 +43,14 @@
   </property>
   <!-- Method aliases -->
   <alias from="(Default)" to="(dynamic view)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
   <!-- Actions -->
-  <action action_id="view" category="object" condition_expr="" i18n:attributes="title" title="View" url_expr="string:${object_url}" icon_expr="string:toolbar-action/view" visible="True">
+  <action action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action action_id="edit" category="object" condition_expr="not:object/@@plone_lock_info/is_locked_for_current_user|python:True" i18n:attributes="title" title="Edit" url_expr="string:${object_url}/edit" icon_expr="string:toolbar-action/edit" visible="True">
+  <action action_id="edit" category="object" condition_expr="" icon_expr="string:toolbar-action/edit" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Document.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Document.xml`

 * *Files 5% similar despite different names*

#### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Document.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Document.xml`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="plone" meta_type="Dexterity FTI" name="Document">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="Document" i18n:domain="plone">
   <!-- Basic properties -->
-  <property i18n:translate="" name="title">Page</property>
-  <property i18n:translate="" name="description"/>
+  <property name="title" i18n:translate="">Page</property>
+  <property name="description" i18n:translate=""/>
   <property name="allow_discussion">False</property>
   <property name="factory">Document</property>
   <property name="icon_expr">string:contenttype/document</property>
   <property name="link_target"/>
   <!-- Hierarchy control -->
   <property name="allowed_content_types"/>
   <property name="filter_content_types">True</property>
@@ -40,14 +40,14 @@
   </property>
   <!-- Method aliases -->
   <alias from="(Default)" to="(dynamic view)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
   <!-- Actions -->
-  <action action_id="view" category="object" condition_expr="" i18n:attributes="title" title="View" url_expr="string:${object_url}" icon_expr="string:toolbar-action/view" visible="True">
+  <action action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action action_id="edit" category="object" condition_expr="not:object/@@plone_lock_info/is_locked_for_current_user|python:True" i18n:attributes="title" title="Edit" url_expr="string:${object_url}/edit" icon_expr="string:toolbar-action/edit" visible="True">
+  <action action_id="edit" category="object" condition_expr="not:object/@@plone_lock_info/is_locked_for_current_user|python:True" icon_expr="string:toolbar-action/edit" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Event.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Event.xml`

 * *Files 4% similar despite different names*

#### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Event.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Event.xml`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="plone" meta_type="Dexterity FTI" name="Event">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="Event" i18n:domain="plone">
   <!-- Basic properties -->
-  <property i18n:translate="" name="title">Event</property>
-  <property i18n:translate="" name="description">Events can be shown in calendars.</property>
+  <property name="title" i18n:translate="">Event</property>
+  <property name="description" i18n:translate="">Events can be shown in calendars.</property>
   <property name="allow_discussion">False</property>
   <property name="factory">Event</property>
   <property name="icon_expr">string:contenttype/event</property>
   <property name="link_target"/>
   <!-- Hierarchy control -->
   <property name="allowed_content_types"/>
   <property name="filter_content_types">True</property>
@@ -45,14 +45,14 @@
   </property>
   <!-- Method aliases -->
   <alias from="(Default)" to="(dynamic view)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
   <!-- Actions -->
-  <action action_id="view" category="object" condition_expr="" i18n:attributes="title" title="View" url_expr="string:${object_url}" icon_expr="string:toolbar-action/view" visible="True">
+  <action action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action action_id="edit" category="object" condition_expr="not:object/@@plone_lock_info/is_locked_for_current_user|python:True" i18n:attributes="title" title="Edit" url_expr="string:${object_url}/edit" icon_expr="string:toolbar-action/edit" visible="True">
+  <action action_id="edit" category="object" condition_expr="not:object/@@plone_lock_info/is_locked_for_current_user|python:True" icon_expr="string:toolbar-action/edit" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/File.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/File.xml`

 * *Files 11% similar despite different names*

#### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/File.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/File.xml`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="plone" meta_type="Dexterity FTI" name="File">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="File" i18n:domain="plone">
   <!-- Basic properties -->
-  <property i18n:translate="" name="title">File</property>
-  <property i18n:translate="" name="description">Lets you upload a file to the site.</property>
+  <property name="title" i18n:translate="">File</property>
+  <property name="description" i18n:translate="">Lets you upload a file to the site.</property>
   <property name="allow_discussion">False</property>
   <property name="factory">File</property>
   <property name="icon_expr">string:contenttype/file</property>
   <property name="link_target"/>
   <!-- Hierarchy control -->
   <property name="allowed_content_types"/>
   <property name="filter_content_types">True</property>
@@ -38,14 +38,14 @@
   </property>
   <!-- Method aliases -->
   <alias from="(Default)" to="@@display-file"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
   <!-- Actions -->
-  <action action_id="view" category="object" condition_expr="" i18n:attributes="title" title="View" url_expr="string:${object_url}" icon_expr="string:toolbar-action/view" visible="True">
+  <action action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action action_id="edit" category="object" condition_expr="" i18n:attributes="title" title="Edit" url_expr="string:${object_url}/edit" icon_expr="string:toolbar-action/edit" visible="True">
+  <action action_id="edit" category="object" condition_expr="" icon_expr="string:toolbar-action/edit" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Folder.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Image.xml`

 * *Files 14% similar despite different names*

#### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Folder.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Image.xml`

```diff
@@ -1,56 +1,51 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="plone" meta_type="Dexterity FTI" name="Folder">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="Image" i18n:domain="plone">
   <!-- Basic properties -->
-  <property i18n:translate="" name="title">Folder</property>
-  <property i18n:translate="" name="description"/>
+  <property name="title" i18n:translate="">Image</property>
+  <property name="description" i18n:translate="">Images can be referenced in pages or displayed in an album.</property>
   <property name="allow_discussion">False</property>
-  <property name="factory">Folder</property>
-  <property name="icon_expr">string:contenttype/folder</property>
+  <property name="factory">Image</property>
+  <property name="icon_expr">string:contenttype/image</property>
   <property name="link_target"/>
   <!-- Hierarchy control -->
   <property name="allowed_content_types"/>
-  <property name="filter_content_types">False</property>
+  <property name="filter_content_types">True</property>
   <property name="global_allow">True</property>
   <!-- Schema, class and security -->
-  <property name="add_permission">plone.app.contenttypes.addFolder</property>
-  <property name="klass">plone.app.contenttypes.content.Folder</property>
-  <property name="model_file">plone.app.contenttypes.schema:folder.xml</property>
+  <property name="add_permission">plone.app.contenttypes.addImage</property>
+  <property name="klass">plone.app.contenttypes.content.Image</property>
+  <property name="model_file">plone.app.contenttypes.schema:image.xml</property>
   <property name="model_source"/>
   <property name="schema"/>
   <!-- Enabled behaviors -->
   <property name="behaviors" purge="false">
-    <element value="plone.dublincore"/>
-    <element value="plone.namefromtitle"/>
+    <element value="plone.categorization"/>
+    <element value="plone.publication"/>
+    <element value="plone.ownership"/>
     <element value="plone.allowdiscussion"/>
-    <element value="plone.excludefromnavigation"/>
     <element value="plone.shortname"/>
-    <element value="plone.constraintypes"/>
+    <element value="plone.namefromfilename"/>
+    <element value="plone.excludefromnavigation"/>
     <element value="plone.relateditems"/>
-    <element value="plone.nextprevioustoggle"/>
   </property>
   <!-- View information -->
-  <property name="add_view_expr">string:${folder_url}/++add++Folder</property>
-  <property name="default_view">listing_view</property>
+  <property name="add_view_expr">string:${folder_url}/++add++Image</property>
+  <property name="default_view">image_view</property>
   <property name="default_view_fallback">False</property>
   <property name="immediate_view">view</property>
   <property name="view_methods">
-    <element value="album_view"/>
-    <element value="event_listing"/>
-    <element value="full_view"/>
-    <element value="listing_view"/>
-    <element value="summary_view"/>
-    <element value="tabular_view"/>
+    <element value="image_view"/>
   </property>
   <!-- Method aliases -->
-  <alias from="(Default)" to="(dynamic view)"/>
+  <alias from="(Default)" to="@@display-file"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
   <!-- Actions -->
-  <action action_id="view" category="object" condition_expr="" i18n:attributes="title" title="View" url_expr="string:${object_url}" icon_expr="string:toolbar-action/view" visible="True">
+  <action action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action action_id="edit" category="object" condition_expr="" i18n:attributes="title" title="Edit" url_expr="string:${object_url}/edit" icon_expr="string:toolbar-action/edit" visible="True">
+  <action action_id="edit" category="object" condition_expr="" icon_expr="string:toolbar-action/edit" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Image.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/News_Item.xml`

 * *Files 11% similar despite different names*

#### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Image.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/News_Item.xml`

```diff
@@ -1,51 +1,53 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="plone" meta_type="Dexterity FTI" name="Image">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="News Item" i18n:domain="plone">
   <!-- Basic properties -->
-  <property i18n:translate="" name="title">Image</property>
-  <property i18n:translate="" name="description">Images can be referenced in pages or displayed in an album.</property>
+  <property name="title" i18n:translate="">News Item</property>
+  <property name="description" i18n:translate=""/>
   <property name="allow_discussion">False</property>
-  <property name="factory">Image</property>
-  <property name="icon_expr">string:contenttype/image</property>
+  <property name="factory">News Item</property>
+  <property name="icon_expr">string:contenttype/news-item</property>
   <property name="link_target"/>
   <!-- Hierarchy control -->
   <property name="allowed_content_types"/>
   <property name="filter_content_types">True</property>
   <property name="global_allow">True</property>
   <!-- Schema, class and security -->
-  <property name="add_permission">plone.app.contenttypes.addImage</property>
-  <property name="klass">plone.app.contenttypes.content.Image</property>
-  <property name="model_file">plone.app.contenttypes.schema:image.xml</property>
+  <property name="add_permission">plone.app.contenttypes.addNewsItem</property>
+  <property name="klass">plone.app.contenttypes.content.NewsItem</property>
+  <property name="model_file">plone.app.contenttypes.schema:news_item.xml</property>
   <property name="model_source"/>
   <property name="schema"/>
   <!-- Enabled behaviors -->
   <property name="behaviors" purge="false">
-    <element value="plone.categorization"/>
-    <element value="plone.publication"/>
-    <element value="plone.ownership"/>
+    <element value="plone.dublincore"/>
+    <element value="plone.richtext"/>
+    <element value="plone.namefromtitle"/>
     <element value="plone.allowdiscussion"/>
     <element value="plone.shortname"/>
-    <element value="plone.namefromfilename"/>
     <element value="plone.excludefromnavigation"/>
     <element value="plone.relateditems"/>
+    <element value="plone.leadimage"/>
+    <element value="plone.versioning"/>
+    <element value="plone.locking"/>
   </property>
   <!-- View information -->
-  <property name="add_view_expr">string:${folder_url}/++add++Image</property>
-  <property name="default_view">image_view</property>
+  <property name="add_view_expr">string:${folder_url}/++add++News Item</property>
+  <property name="default_view">newsitem_view</property>
   <property name="default_view_fallback">False</property>
   <property name="immediate_view">view</property>
   <property name="view_methods">
-    <element value="image_view"/>
+    <element value="newsitem_view"/>
   </property>
   <!-- Method aliases -->
-  <alias from="(Default)" to="@@display-file"/>
+  <alias from="(Default)" to="(dynamic view)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
   <!-- Actions -->
-  <action action_id="view" category="object" condition_expr="" i18n:attributes="title" title="View" url_expr="string:${object_url}" icon_expr="string:toolbar-action/view" visible="True">
+  <action action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action action_id="edit" category="object" condition_expr="" i18n:attributes="title" title="Edit" url_expr="string:${object_url}/edit" icon_expr="string:toolbar-action/edit" visible="True">
+  <action action_id="edit" category="object" condition_expr="not:object/@@plone_lock_info/is_locked_for_current_user|python:True" icon_expr="string:toolbar-action/edit" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Link.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Link.xml`

 * *Files 14% similar despite different names*

#### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/Link.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Link.xml`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="plone" meta_type="Dexterity FTI" name="Link">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="Link" i18n:domain="plone">
   <!-- Basic properties -->
-  <property i18n:translate="" name="title">Link</property>
-  <property i18n:translate="" name="description"/>
+  <property name="title" i18n:translate="">Link</property>
+  <property name="description" i18n:translate=""/>
   <property name="allow_discussion">False</property>
   <property name="factory">Link</property>
   <property name="icon_expr">string:contenttype/link</property>
   <property name="link_target"/>
   <!-- Hierarchy control -->
   <property name="allowed_content_types"/>
   <property name="filter_content_types">True</property>
@@ -36,14 +36,14 @@
   </property>
   <!-- Method aliases -->
   <alias from="(Default)" to="(dynamic view)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
   <!-- Actions -->
-  <action action_id="view" category="object" condition_expr="" i18n:attributes="title" title="View" url_expr="string:${object_url}" icon_expr="string:toolbar-action/view" visible="True">
+  <action action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action action_id="edit" category="object" condition_expr="" i18n:attributes="title" title="Edit" url_expr="string:${object_url}/edit" icon_expr="string:toolbar-action/edit" visible="True">
+  <action action_id="edit" category="object" condition_expr="" icon_expr="string:toolbar-action/edit" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/News_Item.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Collection.xml`

 * *Files 24% similar despite different names*

#### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles/default/types/News_Item.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles/default/types/Collection.xml`

```diff
@@ -1,53 +1,57 @@
 <?xml version="1.0" encoding="utf-8"?>
-<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="plone" meta_type="Dexterity FTI" name="News Item">
+<object xmlns:i18n="http://xml.zope.org/namespaces/i18n" meta_type="Dexterity FTI" name="Collection" i18n:domain="plone">
   <!-- Basic properties -->
-  <property i18n:translate="" name="title">News Item</property>
-  <property i18n:translate="" name="description"/>
+  <property name="title" i18n:translate="">Collection</property>
+  <property name="description" i18n:translate=""/>
   <property name="allow_discussion">False</property>
-  <property name="factory">News Item</property>
-  <property name="icon_expr">string:contenttype/news-item</property>
+  <property name="factory">Collection</property>
+  <property name="icon_expr">string:contenttype/collection</property>
   <property name="link_target"/>
   <!-- Hierarchy control -->
   <property name="allowed_content_types"/>
-  <property name="filter_content_types">True</property>
+  <property name="filter_content_types">False</property>
   <property name="global_allow">True</property>
   <!-- Schema, class and security -->
-  <property name="add_permission">plone.app.contenttypes.addNewsItem</property>
-  <property name="klass">plone.app.contenttypes.content.NewsItem</property>
-  <property name="model_file">plone.app.contenttypes.schema:news_item.xml</property>
+  <property name="add_permission">plone.app.contenttypes.addCollection</property>
+  <property name="klass">plone.app.contenttypes.content.Collection</property>
+  <property name="model_file">plone.app.contenttypes.schema:collection.xml</property>
   <property name="model_source"/>
   <property name="schema"/>
   <!-- Enabled behaviors -->
   <property name="behaviors" purge="false">
-    <element value="plone.dublincore"/>
-    <element value="plone.richtext"/>
     <element value="plone.namefromtitle"/>
+    <element value="plone.collection"/>
     <element value="plone.allowdiscussion"/>
     <element value="plone.shortname"/>
     <element value="plone.excludefromnavigation"/>
+    <element value="plone.dublincore"/>
+    <element value="plone.richtext"/>
     <element value="plone.relateditems"/>
-    <element value="plone.leadimage"/>
-    <element value="plone.versioning"/>
     <element value="plone.locking"/>
   </property>
   <!-- View information -->
-  <property name="add_view_expr">string:${folder_url}/++add++News Item</property>
-  <property name="default_view">newsitem_view</property>
+  <property name="add_view_expr">string:${folder_url}/++add++Collection</property>
+  <property name="default_view">listing_view</property>
   <property name="default_view_fallback">False</property>
   <property name="immediate_view">view</property>
   <property name="view_methods">
-    <element value="newsitem_view"/>
+    <element value="album_view"/>
+    <element value="event_listing"/>
+    <element value="full_view"/>
+    <element value="listing_view"/>
+    <element value="summary_view"/>
+    <element value="tabular_view"/>
   </property>
   <!-- Method aliases -->
   <alias from="(Default)" to="(dynamic view)"/>
   <alias from="edit" to="@@edit"/>
   <alias from="sharing" to="@@sharing"/>
   <alias from="view" to="(selected layout)"/>
   <!-- Actions -->
-  <action action_id="view" category="object" condition_expr="" i18n:attributes="title" title="View" url_expr="string:${object_url}" icon_expr="string:toolbar-action/view" visible="True">
+  <action action_id="view" category="object" condition_expr="" icon_expr="string:toolbar-action/view" title="View" url_expr="string:${object_url}" visible="True" i18n:attributes="title">
     <permission value="View"/>
   </action>
-  <action action_id="edit" category="object" condition_expr="not:object/@@plone_lock_info/is_locked_for_current_user|python:True" i18n:attributes="title" title="Edit" url_expr="string:${object_url}/edit" icon_expr="string:toolbar-action/edit" visible="True">
+  <action action_id="edit" category="object" condition_expr="not:object/@@plone_lock_info/is_locked_for_current_user|python:True" icon_expr="string:toolbar-action/edit" title="Edit" url_expr="string:${object_url}/edit" visible="True" i18n:attributes="title">
     <permission value="Modify portal content"/>
   </action>
 </object>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/profiles.zcml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/profiles.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-<configure xmlns="http://namespaces.zope.org/zope"
-           xmlns:gs="http://namespaces.zope.org/genericsetup"
-           xmlns:zcml="http://namespaces.zope.org/zcml">
+<configure
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:gs="http://namespaces.zope.org/genericsetup"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    >
 
   <!-- Default plone content (frontpage etc.), depends default -->
   <gs:registerProfile
-    name="plone-content"
-    title="Content-types plus example content (plone.app.contenttypes)"
-    directory="profiles/content"
-    description="Plone default content-types (plone.app.contenttypes)"
-    provides="Products.GenericSetup.interfaces.EXTENSION"
-    post_handler=".setuphandlers.import_content"
-    />
+      name="plone-content"
+      title="Content-types plus example content (plone.app.contenttypes)"
+      description="Plone default content-types (plone.app.contenttypes)"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/content"
+      post_handler=".setuphandlers.import_content"
+      />
 
   <!-- All types, no sample content. -->
   <gs:registerProfile
-    name="default"
-    title="Content-types (plone.app.contenttypes)"
-    directory="profiles/default"
-    description="Plone default content-types (plone.app.contenttypes)"
-    provides="Products.GenericSetup.interfaces.EXTENSION"
-    post_handler=".setuphandlers.setup_various"
-    />
+      name="default"
+      title="Content-types (plone.app.contenttypes)"
+      description="Plone default content-types (plone.app.contenttypes)"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/default"
+      post_handler=".setuphandlers.setup_various"
+      />
 
 </configure>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/file.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/file.xml`

 * *Files 19% similar despite different names*

#### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/file.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/file.xml`

```diff
@@ -1,19 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
-<model xmlns="http://namespaces.plone.org/supermodel/schema" xmlns:marshal="http://namespaces.plone.org/supermodel/marshal" xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="plone">
+<model xmlns="http://namespaces.plone.org/supermodel/schema" xmlns:i18n="http://xml.zope.org/namespaces/i18n" xmlns:marshal="http://namespaces.plone.org/supermodel/marshal" i18n:domain="plone">
   <schema>
     <field name="title" type="zope.schema.TextLine">
       <description/>
       <required>False</required>
       <title i18n:translate="">Title</title>
     </field>
     <field name="description" type="zope.schema.Text">
       <description/>
       <required>False</required>
       <title i18n:translate="">Description</title>
     </field>
-    <field name="file" type="plone.namedfile.field.NamedBlobFile" marshal:primary="true">
+    <field marshal:primary="true" name="file" type="plone.namedfile.field.NamedBlobFile">
       <description/>
       <title i18n:translate="label_file">File</title>
     </field>
   </schema>
 </model>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/link.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/link.xml`

 * *Files 8% similar despite different names*

#### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/schema/link.xml` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/schema/link.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<model xmlns="http://namespaces.plone.org/supermodel/schema" xmlns:form="http://namespaces.plone.org/supermodel/form" xmlns:marshal="http://namespaces.plone.org/supermodel/marshal" xmlns:i18n="http://xml.zope.org/namespaces/i18n" i18n:domain="plone">
+<model xmlns="http://namespaces.plone.org/supermodel/schema" xmlns:form="http://namespaces.plone.org/supermodel/form" xmlns:i18n="http://xml.zope.org/namespaces/i18n" xmlns:marshal="http://namespaces.plone.org/supermodel/marshal" i18n:domain="plone">
   <schema>
-    <field name="remoteUrl" type="zope.schema.TextLine" form:widget="plone.app.z3cform.widget.LinkFieldWidget">
+    <field form:widget="plone.app.z3cform.widget.LinkFieldWidget" name="remoteUrl" type="zope.schema.TextLine">
       <description i18n:translate="description_linktype_url">The link is used almost verbatim, relative links become absolute and the strings &quot;${navigation_root_url}&quot; and &quot;${portal_url}&quot; get replaced with the real navigation_root_url or portal_url. If in doubt which one to use, please use navigation_root_url.</description>
       <title i18n:translate="">URL</title>
     </field>
   </schema>
 </model>
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/setuphandlers.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/setuphandlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
             container,
             id="aggregator",
             title=title,
             description=description,
         )
         aggregator = container["aggregator"]
 
-        # Constain types
+        # Constrain types
         allowed_types = [
             "Event",
         ]
 
         _setup_constrains(container, allowed_types)
 
         container.setOrdering("unordered")
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/subscribers.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/subscribers.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/testing.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     We have to set the browserlayer manually, since importing the profile alone
     doesn't do it in tests.
     """
     alsoProvides(request, IPloneAppContenttypesLayer)
 
 
 class PloneAppContenttypes(PloneSandboxLayer):
-
     defaultBases = (
         PAEvent_FIXTURE,
         PLONE_FIXTURE,
     )
 
     def setUpZope(self, app, configurationContext):
         import plone.app.contenttypes
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/file.doc` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/file.doc`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/file.odt` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/file.odt`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/file.pdf` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/file.pdf`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/image.jpg` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/image.jpg`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/image.png` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/image.png`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/image.svg` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/image.svg`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/oldtypes.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/oldtypes.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/keywords.txt` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/keywords.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 *** Settings ***
 
 Library  Remote  ${PLONE_URL}/RobotRemote
 
-Variables  plone/app/contenttypes/tests/robot/variables.py
+Variables  variables.py
 
 *** Keywords ***
 
 I am logged in as site owner
   Enable autologin as  Site Administrator
 
 Click Edit
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/test_collection_creator_criterion.robot` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_creator_criterion.robot`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # ============================================================================
 
 *** Settings *****************************************************************
 
 Resource  plone/app/robotframework/keywords.robot
 Resource  plone/app/robotframework/saucelabs.robot
 Resource  plone/app/robotframework/selenium.robot
-Resource  plone/app/contenttypes/tests/robot/keywords.txt
+Resource  keywords.txt
 
 Library  Remote  ${PLONE_URL}/RobotRemote
 
 Test Setup  Run Keywords  Plone test setup
 Test Teardown  Run keywords  Plone test teardown
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/test_collection_location_criterion.robot` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_location_criterion.robot`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # ============================================================================
 
 *** Settings *****************************************************************
 
 Resource  plone/app/robotframework/keywords.robot
 Resource  plone/app/robotframework/saucelabs.robot
 Resource  plone/app/robotframework/selenium.robot
-Resource  plone/app/contenttypes/tests/robot/keywords.txt
+Resource  keywords.txt
 
-Variables  plone/app/contenttypes/tests/robot/variables.py
+Variables  variables.py
 
 Test Setup  Run Keywords  Plone test setup
 Test Teardown  Run keywords  Plone test teardown
 
 
 *** Test cases ***************************************************************
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/test_collection_review_state_criterion.robot` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_review_state_criterion.robot`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # ============================================================================
 
 *** Settings *****************************************************************
 
 Resource  plone/app/robotframework/keywords.robot
 Resource  plone/app/robotframework/saucelabs.robot
 Resource  plone/app/robotframework/selenium.robot
-Resource  plone/app/contenttypes/tests/robot/keywords.txt
+Resource  keywords.txt
 
 Test Setup  Run Keywords  Plone test setup
 Test Teardown  Run keywords  Plone test teardown
 
 
 *** Test cases ***************************************************************
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/test_collection_short_name_criterion.robot` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_short_name_criterion.robot`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # ============================================================================
 
 *** Settings *****************************************************************
 
 Resource  plone/app/robotframework/keywords.robot
 Resource  plone/app/robotframework/saucelabs.robot
 Resource  plone/app/robotframework/selenium.robot
-Resource  plone/app/contenttypes/tests/robot/keywords.txt
+Resource  keywords.txt
 
 Test Setup  Run Keywords  Plone test setup
 Test Teardown  Run keywords  Plone test teardown
 
 
 *** Test cases ***************************************************************
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/test_collection_type_criterion.robot` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_collection_type_criterion.robot`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # ============================================================================
 
 *** Settings *****************************************************************
 
 Resource  plone/app/robotframework/keywords.robot
 Resource  plone/app/robotframework/saucelabs.robot
 Resource  plone/app/robotframework/selenium.robot
-Resource  plone/app/contenttypes/tests/robot/keywords.txt
+Resource  keywords.txt
 
 Test Setup  Run Keywords  Plone test setup
 Test Teardown  Run keywords  Plone test teardown
 
 
 *** Test cases ***************************************************************
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/robot/test_folderlisting.robot` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/robot/test_folderlisting.robot`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 *** Settings ***
 
 Resource  plone/app/robotframework/keywords.robot
 Resource  plone/app/robotframework/saucelabs.robot
 Resource  plone/app/robotframework/selenium.robot
-Resource  plone/app/contenttypes/tests/robot/keywords.txt
+Resource  keywords.txt
 
-Variables  plone/app/contenttypes/tests/robot/variables.py
+Variables  variables.py
 
 
 Test Setup  Run Keywords  Setup Testcontent  Plone test setup
 Test Teardown  Run keywords  Plone test teardown
 
 *** Variables ***
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_behaviors_collection.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         "o": "plone.app.querystring.operation.string.contains",
         "v": "Collection Test Page",
     }
 ]
 
 
 class CollectionBehaviorFunctionalTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.portal_url = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_behaviors_leadimage.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_leadimage.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 import io
 import os
 import unittest
 
 
 class LeadImageBehaviorFunctionalTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
         app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.portal_url = self.portal.absolute_url()
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_behaviors_richtext.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_richtext.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_behaviors_table_of_contents.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_behaviors_table_of_contents.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,37 +10,32 @@
 from plone.testing.zope import Browser
 from zope.interface import alsoProvides
 
 import unittest
 
 
 class TableOfContentsBehaviorFunctionalTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
         app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.portal_url = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Contributor"])
         fti = DexterityFTI("tocdocument")
         self.portal.portal_types._setObject("tocdocument", fti)
         fti.klass = "plone.dexterity.content.Item"
-        fti.behaviors = (
-            "plone.app.contenttypes.behaviors.tableofcontents." "ITableOfContents",
-        )
+        fti.behaviors = ("plone.tableofcontents", "plone.richtext")
         self.fti = fti
-        alsoProvides(self.portal.REQUEST, IPloneAppContenttypesLayer)
         alsoProvides(self.request, IPloneAppContenttypesLayer)
-        from plone.app.contenttypes.behaviors.tableofcontents import ITableOfContents
-
-        alsoProvides(self.request, ITableOfContents)
         self.portal.invokeFactory(
-            "tocdocument", id="tocdoc", title="Document with a table of contents"
+            "tocdocument",
+            id="tocdoc",
+            title="Document with a table of contents",
         )
         import transaction
 
         transaction.commit()
         # Set up browser
         self.browser = Browser(app)
         self.browser.handleErrors = False
@@ -62,8 +57,8 @@
             name="form.widgets.ITableOfContents.table_of_contents:list"
         )
         toc_ctl.value = [
             "selected",
         ]
         # Submit form
         self.browser.getControl("Save").click()
-        self.assertTrue('<section id="document-toc"' in self.browser.contents)
+        self.assertTrue('id="document-toc"' in self.browser.contents)
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_browser_utils.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_browser_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,28 +20,27 @@
 
     def __init__(self, contentType, filename):
         self.contentType = contentType
         self.filename = filename
 
 
 class MimeTypeIconIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         portal = self.layer["portal"]
         request = self.layer["request"]
         self.view = getMultiAdapter((portal, request), name="contenttype_utils")
 
     def test_none(self):
         self.assertEqual(self.view.getMimeTypeIcon(DummyFile(None, None)), FALLBACK)
 
     def test_unknown(self):
         self.assertEqual(
-            self.view.getMimeTypeIcon(DummyFile("some/unknown", "unkown.unknown")),
+            self.view.getMimeTypeIcon(DummyFile("some/unknown", "unknown.unknown")),
             FALLBACK,
         )
 
     def test_contenttype_pdf(self):
         self.assertEqual(
             self.view.getMimeTypeIcon(DummyFile("application/pdf", None)),
             PREFIX + "pdf.png",
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_collection.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     filename = os.path.join(os.path.dirname(__file__), "image.png")
     with open(filename, "rb") as f:
         image_data = f.read()
     return NamedBlobImage(data=image_data, filename=filename)
 
 
 class PloneAppCollectionClassTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         login(self.portal, TEST_USER_NAME)
         self.portal.invokeFactory("Collection", "collection")
@@ -59,15 +58,14 @@
     def test_syndicatable(self):
         from plone.base.interfaces.syndication import ISyndicatable
 
         self.assertTrue(ISyndicatable.providedBy(self.collection))
 
 
 class PloneAppCollectionIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
 
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         login(self.portal, TEST_USER_NAME)
@@ -92,15 +90,14 @@
     def test_adding(self):
         self.folder.invokeFactory("Collection", "collection1")
         p1 = self.folder["collection1"]
         self.assertTrue(ICollection.providedBy(p1))
 
 
 class PloneAppCollectionViewsIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.browser = Browser(self.layer["app"])
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         set_browserlayer(self.request)
@@ -374,15 +371,14 @@
         # navigation root.
         items = wrapped.results(batch=False)
         ids = [i.getId() for i in items]
         self.assertListEqual(ids, ["item_in_folder1"])
 
 
 class PloneAppCollectionEditViewsIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         set_browserlayer(self.request)
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_collection_rss.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_collection_rss.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         "o": "plone.app.querystring.operation.string.is",
         "v": "Collection Test Page",
     }
 ]
 
 
 class RSSViewTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         login(self.portal, TEST_USER_NAME)
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_content_profile.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_content_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PloneSandboxLayer
-from plone.base.interfaces.constrains import ISelectableConstrainTypes
 from plone.portlets.interfaces import ILocalPortletAssignmentManager
 from plone.portlets.interfaces import IPortletManager
 from Products.CMFCore.utils import getToolByName
-from Products.PythonScripts.PythonScript import PythonScript
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 
 import unittest
 
 
 class PloneAppContenttypesContent(PloneSandboxLayer):
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_document.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from zope.component import queryUtility
 from zope.interface import alsoProvides
 
 import unittest
 
 
 class DocumentIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.request["ACTUAL_URL"] = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Contributor"])
@@ -72,15 +71,14 @@
 
     def tearDown(self):
         if "document" in self.portal.objectIds():
             self.portal.manage_delObjects(ids="document")
 
 
 class DocumentFunctionalTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
         app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.portal_url = self.portal.absolute_url()
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_event.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from zope.component import queryUtility
 from zope.interface import alsoProvides
 
 import unittest
 
 
 class EventIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.request["ACTUAL_URL"] = self.portal.absolute_url()
         self.request["LANGUAGE"] = "en"
@@ -68,15 +67,14 @@
         self.assertTrue(view())
         self.assertEqual(view.request.response.status, 200)
         self.assertTrue("My Event" in view())
         self.assertTrue("This is my event." in view())
 
 
 class EventFunctionalTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
         app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.portal_url = self.portal.absolute_url()
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_file.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import io
 import os.path
 import transaction
 import unittest
 
 
 class FileIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.request["ACTUAL_URL"] = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Contributor"])
@@ -97,15 +96,14 @@
         alsoProvides(self.request, IPloneAppContenttypesLayer)
         view = file.restrictedTraverse("@@file_view")
         rendered = view()
         self.assertTrue("</video>" in rendered)
 
 
 class FileFunctionalTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
         app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.portal_url = self.portal.absolute_url()
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_folder.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from zope.component import createObject
 from zope.component import queryUtility
 
 import unittest
 
 
 class FolderIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.request["ACTUAL_URL"] = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Contributor"])
@@ -46,15 +45,14 @@
 
     def test_adding(self):
         self.portal.invokeFactory("Folder", "doc1")
         self.assertTrue(IFolder.providedBy(self.portal["doc1"]))
 
 
 class FolderViewIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.request["ACTUAL_URL"] = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Contributor"])
@@ -115,15 +113,14 @@
         self.assertEqual(batch.length, 5)
         self.assertEqual(len([item for item in batch]), 5)
         self.assertTrue(batch.has_next)
         self.assertEqual(batch.next_item_count, 2)
 
 
 class FolderFunctionalTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
         app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.portal_url = self.portal.absolute_url()
         self.browser = Browser(app)
@@ -158,15 +155,14 @@
         widget = "form.widgets.IShortName.id"
         self.browser.getControl(name=widget).value = "my-special-folder"
         self.browser.getControl("Save").click()
         self.assertTrue(self.browser.url.endswith("my-special-folder/view"))
 
 
 class FolderViewFunctionalTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
         app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_image.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     filename = os.path.join(os.path.dirname(__file__), filename)
     with open(filename, "rb") as f:
         image_data = f.read()
     return NamedBlobImage(data=image_data, filename=filename)
 
 
 class ImageIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.request["ACTUAL_URL"] = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Contributor"])
@@ -57,15 +56,14 @@
 
     def test_adding(self):
         self.portal.invokeFactory("Image", "doc1")
         self.assertTrue(IImage.providedBy(self.portal["doc1"]))
 
 
 class ImageViewIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.request["ACTUAL_URL"] = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
@@ -105,15 +103,14 @@
         self.assertRegex(
             scale.tag("image", scale="large"),
             r'<img src="http://nohost/plone/image/@@images/[a-z0-9\-]*.svg" alt="My Image" title="My Image" height="[a-z0-9\-]*" width="[a-z0-9\-]*" />',  # noqa: E501
         )
 
 
 class ImageFunctionalTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
         app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.portal_url = self.portal.absolute_url()
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_indexes.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_indexes.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from Products.CMFCore.utils import getToolByName
 
 import os
 import unittest
 
 
 class CatalogIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.portal.invokeFactory("Folder", "folder")
         self.folder = self.portal.folder
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_link.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_link.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from zope.schema import TextLine
 from zope.traversing.interfaces import BeforeTraverseEvent
 
 import unittest
 
 
 class LinkIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.request["ACTUAL_URL"] = self.portal.absolute_url()
         setRoles(self.portal, TEST_USER_ID, ["Contributor"])
@@ -56,15 +55,14 @@
 
     def test_adding(self):
         self.portal.invokeFactory("Link", "doc1")
         self.assertTrue(ILink.providedBy(self.portal["doc1"]))
 
 
 class LinkViewIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.request["ACTUAL_URL"] = self.portal.absolute_url()
         self.response = self.request.response
@@ -244,15 +242,14 @@
         self.assertEqual(self.response.status, 200)
 
     def _get_link_redirect_view(self, obj):
         return getMultiAdapter((obj, self.request), name="link_redirect_view")
 
 
 class LinkFunctionalTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
         app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.portal_url = self.portal.absolute_url()
@@ -283,15 +280,14 @@
 
         self.assertTrue(self.browser.url.endswith("my-special-link/view"))
         self.assertTrue("My link" in self.browser.contents)
         self.assertTrue("This is my link" in self.browser.contents)
 
 
 class LinkWidgetIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     default_result = {
         "internal": "",
         "external": "",
         "email": "",
         "email_subject": "",
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_news_item.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_news_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from zope.interface import alsoProvides
 from zope.viewlet.interfaces import IViewletManager
 
 import unittest
 
 
 class NewsItemIntegrationTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.request["ACTUAL_URL"] = self.portal.absolute_url()
         from plone.app.contenttypes.interfaces import IPloneAppContenttypesLayer
@@ -89,15 +88,14 @@
         leadimage_viewlet = [
             v for v in manager.viewlets if v.__name__ == "contentleadimage"
         ]
         self.assertEqual(len(leadimage_viewlet), 0)
 
 
 class NewsItemFunctionalTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING
 
     def setUp(self):
         app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.portal_url = self.portal.absolute_url()
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_robot.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_security.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_security.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,16 @@
     PLONE_APP_CONTENTTYPES_FUNCTIONAL_TESTING,
 )
 from plone.app.testing import login
 from plone.app.testing import logout
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import TEST_USER_NAME
-from plone.testing.zope import Browser
 
 import base64
-import os
-import pkg_resources
 import re
 import sys
 import transaction
 import unittest
 
 
 # List various possibly read methods.
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_setup.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 
 import unittest
 
 
 class PloneAppContenttypesSetupTest(unittest.TestCase):
-
     layer = PLONE_APP_CONTENTTYPES_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.types = self.portal.portal_types
```

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/tests/test_webdav.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/tests/test_webdav.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/upgrades.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone/app/contenttypes/utils.py` & `plone.app.contenttypes-3.0.2/plone/app/contenttypes/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.contenttypes-3.0.1/plone.app.contenttypes.egg-info/PKG-INFO` & `plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contenttypes
-Version: 3.0.1
+Version: 3.0.2
 Summary: Default content types for Plone based on Dexterity
 Home-page: https://github.com/plone/plone.app.contenttypes
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: plone content types dexterity
 Classifier: Development Status :: 5 - Production/Stable
@@ -218,14 +218,38 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2023-04-14)
+------------------
+
+Bug fixes:
+
+
+- Fix test_behaviors_table_of_contents: ordering of attrtributes changed.
+  @jensens (fix-test_behaviors_table_of_contents)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (#47959565)
+
+
+Tests
+
+
+- Run the robot tests.
+  [maurits] (#69)
+
+
 3.0.1 (2023-01-26)
 ------------------
 
 Bug fixes:
 
 
 - Fix error in News Item view when it doesn't have a text field. [davisagli] (#652)
@@ -996,15 +1020,15 @@
 
 New features:
 
 - New metadata catalog column MimeType
   https://github.com/plone/Products.CMFPlone/issues/1995
   [fgrcon]
 
-- new behavior: IThumbIconHandling, supress thumbs /icons, adjust thumb size, templates adapted
+- new behavior: IThumbIconHandling, suppress thumbs /icons, adjust thumb size, templates adapted
   https://github.com/plone/Products.CMFPlone/issues/1734 (PLIP)
 
 Bug fixes:
 
 - fixed css-classes for thumb scales ...
   https://github.com/plone/Products.CMFPlone/issues/2077
   [fgrcon]
@@ -1114,15 +1138,15 @@
 -------------------
 
 New features:
 
 - Configure edit urls for locking support, where locking support is enabled.
   [thet]
 
-- Add ``i18n:attribute`` properies to all action nodes for FTI types.
+- Add ``i18n:attribute`` properties to all action nodes for FTI types.
   [thet]
 
 - added few pypi links in 'Migration' section
   [kkhan]
 
 Bug fixes:
 
@@ -1355,15 +1379,15 @@
 
 1.2.4 (2015-09-27)
 ------------------
 
 - Fixed full_view error when collection contains itself.
   [vangheem]
 
-- test_content_profile: do not appy Products.CMFPlone:plone.
+- test_content_profile: do not apply Products.CMFPlone:plone.
   [maurits]
 
 
 1.2.3 (2015-09-20)
 ------------------
 
 - Do not raise an exception for items where @@full_view_item throws an
@@ -1372,26 +1396,26 @@
 
 - Do not raise errors when IPrimaryFieldInfo(obj) fails (e.g. when the
   Schema-Cache is gone).
   Fixes https://github.com/plone/Products.CMFPlone/issues/839
   [pbauer]
 
 - Fix an error with logging an exception on indexing SearchableText for files
-  and concating utf-8 encoded strings.
+  and concatenating utf-8 encoded strings.
   [thet]
 
 - Make consistent use of LeadImage behavior everywhere. Related to
   plone/plone.app.contenttypes#1012. Contentleadimages no longer show up in
   full_view since they are a viewlet.
   [sneridagh, pbauer]
 
 - Fixed the summary_view styling
   [sneridagh]
 - redirect_links property has moved to the configuration registry.
-- redirect_links, types_view_action_in_listings properies have moved to the
+- redirect_links, types_view_action_in_listings properties have moved to the
   configuration registry.
   [esteele]
 
 
 1.2.2 (2015-09-15)
 ------------------
 
@@ -1650,15 +1674,15 @@
 
 1.2a5 (2014-10-23)
 ------------------
 
 - Code modernization: sorted imports, use decorators, utf8 headers.
   [jensens]
 
-- Fix: Added missing types to CMFDiffTool configuraion.
+- Fix: Added missing types to CMFDiffTool configuration.
   [jensens]
 
 - Integration of the new markup update and CSS for both Plone and Barceloneta
   theme. This is the work done in the GSOC Barceloneta theme project. Fix
   several templates.
   [albertcasado, sneridagh]
 
@@ -1690,15 +1714,15 @@
   The previous release of p.a.c got an implicit Plone 5 dependency through a
   previous version of plone.app.event.
   [thet]
 
 - Replace AT-fti with DX-fti when migrating a type.
   [esteele, pbauer]
 
-- Only show migrateable types (fixes #155)
+- Only show migratable types (fixes #155)
   [pbauer]
 
 - Add logging during and after migration (fixes #156)
   [pbauer]
 
 - When replacing the default news and events collections, reverse the
   sort order correctly.
@@ -1789,15 +1813,15 @@
 
 - Don't remove custom behaviors on reinstalling.
   [pbauer]
 
 - Remove enabling simple_publication_workflow from testing fixture.
   [timo]
 
-- Only show migrateable types (fixes #155)
+- Only show migratable types (fixes #155)
   [pbauer]
 
 - Add logging during and after migration (fixes #156)
   [pbauer]
 
 - Remove 'robot-test-folder' from p.a.contenttypes test setup. It is bad to
   add content to test layers, especially if those test layers are used by
@@ -1955,30 +1979,30 @@
 
 - Its possible to upload non-image data into a newsitem. The view was broken
   then. Now it shows the uploaded file for download below the content. Its no
   longer broken.
   [jensens]
 
 - Add contributor role as default for all add permissions in order to
-  work together with the different plone worklfows, which assume it is
+  work together with the different plone workflows, which assume it is
   set this way.
   [jensens]
 
 - fix #60: File Type has no mimetype specific icon in catalog metadata.
   Also fixed for Image.
   [jensens]
 
 - fix #58: Migration ignores "Exclude from Navigation".
   [jensens]
 
 - disable LinkIntegrityNotifications during migrations, closes #40.
   [jensens]
 
 - Fix Bug on SearchableText_file indexer when input stream contains
-  characters not convertable in ASCII. Assumes now utf-8 and replaces
+  characters not convertible in ASCII. Assumes now utf-8 and replaces
   all unknown. Even if search can not find the words with special
   characters in, indexer does not break completely on those items.
   [jensens]
 
 - Remove dependency on plone.app.referenceablebehavior, as it depends on
   Products.Archetypes which installs the uid_catalog.
   [thet]
```

### Comparing `plone.app.contenttypes-3.0.1/plone.app.contenttypes.egg-info/SOURCES.txt` & `plone.app.contenttypes-3.0.2/plone.app.contenttypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

