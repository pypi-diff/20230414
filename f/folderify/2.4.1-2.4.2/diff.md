# Comparing `tmp/folderify-2.4.1.tar.gz` & `tmp/folderify-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folderify-2.4.1.tar", last modified: Thu Apr 13 22:02:16 2023, max compression
+gzip compressed data, was "folderify-2.4.2.tar", last modified: Thu Apr 13 22:30:19 2023, max compression
```

## Comparing `folderify-2.4.1.tar` & `folderify-2.4.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.160872 folderify-2.4.1/
--rw-r--r--   0 lgarron    (501) staff       (20)     1022 2023-04-07 03:42:18.000000 folderify-2.4.1/LICENSE.md
--rw-r--r--   0 lgarron    (501) staff       (20)       55 2023-04-13 21:50:34.000000 folderify-2.4.1/MANIFEST.in
--rw-r--r--   0 lgarron    (501) staff       (20)     6757 2023-04-13 22:02:16.160713 folderify-2.4.1/PKG-INFO
--rw-r--r--   0 lgarron    (501) staff       (20)     5884 2023-04-13 22:01:19.000000 folderify-2.4.1/README.md
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.151302 folderify-2.4.1/folderify/
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.153881 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/
--rw-r--r--   0 lgarron    (501) staff       (20)    17603 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128.png
--rw-r--r--   0 lgarron    (501) staff       (20)    60552 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)      554 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1305 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)    60552 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256.png
--rw-r--r--   0 lgarron    (501) staff       (20)   191981 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1305 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32.png
--rw-r--r--   0 lgarron    (501) staff       (20)     4514 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)   191981 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512.png
--rw-r--r--   0 lgarron    (501) staff       (20)   528334 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512@2x.png
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.155808 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/
--rw-r--r--   0 lgarron    (501) staff       (20)    20653 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128.png
--rw-r--r--   0 lgarron    (501) staff       (20)    76804 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)      692 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1461 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)    76804 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256.png
--rw-r--r--   0 lgarron    (501) staff       (20)   261575 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1473 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32.png
--rw-r--r--   0 lgarron    (501) staff       (20)     5870 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)   261575 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512.png
--rw-r--r--   0 lgarron    (501) staff       (20)   787589 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512@2x.png
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.157922 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/
--rw-r--r--   0 lgarron    (501) staff       (20)    21366 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128.png
--rw-r--r--   0 lgarron    (501) staff       (20)    68009 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)     3176 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16.png
--rw-r--r--   0 lgarron    (501) staff       (20)     4045 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)    68009 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256.png
--rw-r--r--   0 lgarron    (501) staff       (20)   268431 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)     4029 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32.png
--rw-r--r--   0 lgarron    (501) staff       (20)     7708 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)   268431 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512.png
--rw-r--r--   0 lgarron    (501) staff       (20)  1089689 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512@2x.png
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.159974 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/
--rw-r--r--   0 lgarron    (501) staff       (20)    17304 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128.png
--rw-r--r--   0 lgarron    (501) staff       (20)    64503 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)      564 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1470 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)    64503 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256.png
--rw-r--r--   0 lgarron    (501) staff       (20)   220247 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1475 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32.png
--rw-r--r--   0 lgarron    (501) staff       (20)     4734 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)   220247 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512.png
--rw-r--r--   0 lgarron    (501) staff       (20)   697357 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)        0 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/__init__.py
--rw-r--r--   0 lgarron    (501) staff       (20)    21698 2023-04-13 22:01:19.000000 folderify-2.4.1/folderify/__main__.py
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.160457 folderify-2.4.1/folderify/lib/
--rwxr-xr-x   0 lgarron    (501) staff       (20)    58892 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/lib/seticon
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.151919 folderify-2.4.1/folderify.egg-info/
--rw-r--r--   0 lgarron    (501) staff       (20)     6757 2023-04-13 22:02:16.000000 folderify-2.4.1/folderify.egg-info/PKG-INFO
--rw-r--r--   0 lgarron    (501) staff       (20)     2783 2023-04-13 22:02:16.000000 folderify-2.4.1/folderify.egg-info/SOURCES.txt
--rw-r--r--   0 lgarron    (501) staff       (20)        1 2023-04-13 22:02:16.000000 folderify-2.4.1/folderify.egg-info/dependency_links.txt
--rw-r--r--   0 lgarron    (501) staff       (20)       55 2023-04-13 22:02:16.000000 folderify-2.4.1/folderify.egg-info/entry_points.txt
--rw-r--r--   0 lgarron    (501) staff       (20)       10 2023-04-13 22:02:16.000000 folderify-2.4.1/folderify.egg-info/top_level.txt
--rw-r--r--   0 lgarron    (501) staff       (20)       38 2023-04-13 22:02:16.160921 folderify-2.4.1/setup.cfg
--rw-r--r--   0 lgarron    (501) staff       (20)     1964 2023-04-13 22:01:22.000000 folderify-2.4.1/setup.py
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:30:19.436671 folderify-2.4.2/
+-rw-r--r--   0 lgarron    (501) staff       (20)     1022 2023-04-07 03:42:18.000000 folderify-2.4.2/LICENSE.md
+-rw-r--r--   0 lgarron    (501) staff       (20)       55 2023-04-13 21:50:34.000000 folderify-2.4.2/MANIFEST.in
+-rw-r--r--   0 lgarron    (501) staff       (20)     6757 2023-04-13 22:30:19.436518 folderify-2.4.2/PKG-INFO
+-rw-r--r--   0 lgarron    (501) staff       (20)     5884 2023-04-13 22:01:19.000000 folderify-2.4.2/README.md
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:30:19.425054 folderify-2.4.2/folderify/
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:30:19.427950 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/
+-rw-r--r--   0 lgarron    (501) staff       (20)    17603 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    60552 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)      554 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     1305 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    60552 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   191981 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     1305 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     4514 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   191981 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   528334 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512@2x.png
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:30:19.429980 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/
+-rw-r--r--   0 lgarron    (501) staff       (20)    20653 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    76804 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)      692 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     1461 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    76804 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   261575 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     1473 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     5870 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   261575 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   787589 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512@2x.png
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:30:19.433386 folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/
+-rw-r--r--   0 lgarron    (501) staff       (20)    21366 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    68009 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     3176 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     4045 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    68009 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   268431 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     4029 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     7708 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   268431 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512.png
+-rw-r--r--   0 lgarron    (501) staff       (20)  1089689 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512@2x.png
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:30:19.435755 folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/
+-rw-r--r--   0 lgarron    (501) staff       (20)    17304 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    64503 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)      564 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     1470 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    64503 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   220247 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     1475 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     4734 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   220247 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   697357 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)        0 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/__init__.py
+-rw-r--r--   0 lgarron    (501) staff       (20)    21669 2023-04-13 22:29:31.000000 folderify-2.4.2/folderify/__main__.py
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:30:19.436278 folderify-2.4.2/folderify/lib/
+-rwxr-xr-x   0 lgarron    (501) staff       (20)    58892 2023-04-13 21:50:34.000000 folderify-2.4.2/folderify/lib/seticon
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:30:19.425721 folderify-2.4.2/folderify.egg-info/
+-rw-r--r--   0 lgarron    (501) staff       (20)     6757 2023-04-13 22:30:19.000000 folderify-2.4.2/folderify.egg-info/PKG-INFO
+-rw-r--r--   0 lgarron    (501) staff       (20)     2783 2023-04-13 22:30:19.000000 folderify-2.4.2/folderify.egg-info/SOURCES.txt
+-rw-r--r--   0 lgarron    (501) staff       (20)        1 2023-04-13 22:30:19.000000 folderify-2.4.2/folderify.egg-info/dependency_links.txt
+-rw-r--r--   0 lgarron    (501) staff       (20)       58 2023-04-13 22:30:19.000000 folderify-2.4.2/folderify.egg-info/entry_points.txt
+-rw-r--r--   0 lgarron    (501) staff       (20)       10 2023-04-13 22:30:19.000000 folderify-2.4.2/folderify.egg-info/top_level.txt
+-rw-r--r--   0 lgarron    (501) staff       (20)       38 2023-04-13 22:30:19.436714 folderify-2.4.2/setup.cfg
+-rw-r--r--   0 lgarron    (501) staff       (20)     1967 2023-04-13 22:29:54.000000 folderify-2.4.2/setup.py
```

### Comparing `folderify-2.4.1/LICENSE.md` & `folderify-2.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/PKG-INFO` & `folderify-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folderify
-Version: 2.4.1
+Version: 2.4.2
 Summary: Generate pixel-perfect macOS folder icons in the native style.
 Home-page: https://github.com/lgarron/folderify
 Author: Lucas Garron
 Author-email: code@garron.net
 License: MIT
 Keywords: icon macOS OSX Mac Darwin graphics folder imagemagick
 Platform: UNKNOWN
```

### Comparing `folderify-2.4.1/README.md` & `folderify-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512@2x.png` & `folderify-2.4.2/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify/__main__.py` & `folderify-2.4.2/folderify/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import os.path
 import platform
 import shutil
 import subprocess
 import sys
 import tempfile
 import time
-import warnings
 
 from string import Template
 
 ################################################################
 
 DEBUG = "FOLDERIFY_DEBUG" in os.environ and os.environ["FOLDERIFY_DEBUG"] == "1"
 OLD_IMPLEMENTATION_FOLDER_STYLES = ["Yosemite", "Leopard"]
@@ -100,23 +99,24 @@
   parser.add_argument(
     "--verbose", "-v",
     action="store_true",
     help="Detailed output.")
 
   ################################################################
 
-  warnings.warn("""
+  print("""\033[93m
 --------
 
-You are using folderify v2, which is no longer officially supported. Unless you need folder icons for macOS 10.15 or earlier, please consider updating to folderify v3:
+You are using folderify v2, which is no longer officially supported.
+Unless you need folder icons for macOS 10.15 or earlier, please consider updating to folderify v3:
 
 https://github.com/lgarron/folderify/tree/main#install
 
 --------
-""", DeprecationWarning)
+\033[0m""")
   time.sleep(2)
 
   args = parser.parse_args()
 
   if args.mask and not os.path.exists(args.mask):
     parser.error("Mask file does not exist: %s" % args.mask)
```

### Comparing `folderify-2.4.1/folderify/lib/seticon` & `folderify-2.4.2/folderify/lib/seticon`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/folderify.egg-info/PKG-INFO` & `folderify-2.4.2/folderify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folderify
-Version: 2.4.1
+Version: 2.4.2
 Summary: Generate pixel-perfect macOS folder icons in the native style.
 Home-page: https://github.com/lgarron/folderify
 Author: Lucas Garron
 Author-email: code@garron.net
 License: MIT
 Keywords: icon macOS OSX Mac Darwin graphics folder imagemagick
 Platform: UNKNOWN
```

### Comparing `folderify-2.4.1/folderify.egg-info/SOURCES.txt` & `folderify-2.4.2/folderify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `folderify-2.4.1/setup.py` & `folderify-2.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Get the long description from the relevant file
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="folderify",
-    version="2.4.1",
+    version="2.4.2",
     description="Generate pixel-perfect macOS folder icons in the native style.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/lgarron/folderify",
 
     author="Lucas Garron",
     author_email="code@garron.net",
@@ -57,11 +57,11 @@
 
 
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # pip to create the appropriate form of executable for the target platform.
     entry_points={
         "console_scripts": [
-            "folderify = folderify.__main__:main",
+            "folderify-v2 = folderify.__main__:main",
         ],
     },
 )
```

