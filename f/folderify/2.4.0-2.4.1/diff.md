# Comparing `tmp/folderify-2.4.0.tar.gz` & `tmp/folderify-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folderify-2.4.0.tar", last modified: Wed Mar  8 05:29:05 2023, max compression
+gzip compressed data, was "folderify-2.4.1.tar", last modified: Thu Apr 13 22:02:16 2023, max compression
```

## Comparing `folderify-2.4.0.tar` & `folderify-2.4.1.tar`

### file list

```diff
@@ -1,149 +1,62 @@
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.337971 folderify-2.4.0/
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.275262 folderify-2.4.0/.github/
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.279564 folderify-2.4.0/.github/workflows/
--rw-r--r--   0 lgarron    (501) staff       (20)      684 2021-10-21 21:15:48.000000 folderify-2.4.0/.github/workflows/github-release.yml
--rw-r--r--   0 lgarron    (501) staff       (20)      554 2022-09-14 19:09:38.000000 folderify-2.4.0/.github/workflows/test.yml
--rw-r--r--   0 lgarron    (501) staff       (20)      114 2021-10-21 21:15:48.000000 folderify-2.4.0/.gitignore
--rw-r--r--   0 lgarron    (501) staff       (20)     1022 2021-10-21 21:15:48.000000 folderify-2.4.0/LICENSE.md
--rw-r--r--   0 lgarron    (501) staff       (20)       55 2021-10-21 21:15:48.000000 folderify-2.4.0/MANIFEST.in
--rw-r--r--   0 lgarron    (501) staff       (20)      218 2023-03-08 05:08:24.000000 folderify-2.4.0/Makefile
--rw-r--r--   0 lgarron    (501) staff       (20)     6451 2023-03-08 05:29:05.337774 folderify-2.4.0/PKG-INFO
--rw-r--r--   0 lgarron    (501) staff       (20)     5578 2023-03-08 05:28:16.000000 folderify-2.4.0/README.md
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.275770 folderify-2.4.0/examples/
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.284485 folderify-2.4.0/examples/png/
--rw-r--r--   0 lgarron    (501) staff       (20)   872913 2021-10-21 21:15:48.000000 folderify-2.4.0/examples/png/apple.gif
--rw-r--r--   0 lgarron    (501) staff       (20)    60003 2021-10-21 21:15:48.000000 folderify-2.4.0/examples/png/apple_folder_256.png
--rw-r--r--   0 lgarron    (501) staff       (20)    65282 2021-10-21 21:15:48.000000 folderify-2.4.0/examples/png/cube_folder_256.png
--rw-r--r--   0 lgarron    (501) staff       (20)    94243 2021-10-21 21:15:48.000000 folderify-2.4.0/examples/png/explanation.png
--rw-r--r--   0 lgarron    (501) staff       (20)    63164 2021-10-21 21:15:48.000000 folderify-2.4.0/examples/png/octocat_folder_256.png
--rw-r--r--   0 lgarron    (501) staff       (20)    64245 2021-10-21 21:15:48.000000 folderify-2.4.0/examples/png/rhombic_hexecontahedron_folder_256.png
--rw-r--r--   0 lgarron    (501) staff       (20)    63056 2021-10-21 21:15:48.000000 folderify-2.4.0/examples/png/sysprefs_folder_256.png
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.286774 folderify-2.4.0/examples/png-Yosemite/
--rw-r--r--   0 lgarron    (501) staff       (20)    55218 2021-10-21 21:15:48.000000 folderify-2.4.0/examples/png-Yosemite/apple_folder_256.png
--rw-r--r--   0 lgarron    (501) staff       (20)    63211 2021-10-21 21:15:48.000000 folderify-2.4.0/examples/png-Yosemite/cube_folder_256.png
--rw-r--r--   0 lgarron    (501) staff       (20)    59495 2021-10-21 21:15:48.000000 folderify-2.4.0/examples/png-Yosemite/octocat_folder_256.png
--rw-r--r--   0 lgarron    (501) staff       (20)    61699 2021-10-21 21:15:48.000000 folderify-2.4.0/examples/png-Yosemite/rhombic_hexecontahedron_folder_256.png
--rw-r--r--   0 lgarron    (501) staff       (20)    60280 2021-10-21 21:15:48.000000 folderify-2.4.0/examples/png-Yosemite/sysprefs_folder_256.png
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.289996 folderify-2.4.0/examples/src/
--rw-r--r--   0 lgarron    (501) staff       (20)       16 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/.gitignore
--rw-r--r--   0 lgarron    (501) staff       (20)    57339 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.302787 folderify-2.4.0/examples/src/apple.png-folderify-debug/
--rw-r--r--   0 lgarron    (501) staff       (20)     1058 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/128x128_1.0_SIZED_MASK.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1499 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/128x128_1.1_FILL_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1283 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/128x128_1.2_FILL.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1246 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/128x128_2.1_BLACK_NEGATED.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1563 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/128x128_2.2_BLACK_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      439 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16@2x_1.0_SIZED_MASK.png
--rw-r--r--   0 lgarron    (501) staff       (20)      588 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16@2x_1.1_FILL_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      560 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16@2x_1.2_FILL.png
--rw-r--r--   0 lgarron    (501) staff       (20)      459 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16@2x_2.1_BLACK_NEGATED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      595 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16@2x_2.2_BLACK_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      625 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16@2x_2.3_BLACK_BLURRED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      632 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16@2x_2.4_BLACK_MASKED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      600 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16@2x_2.5_BLACK_SHADOW.png
--rw-r--r--   0 lgarron    (501) staff       (20)      588 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16@2x_3.1_WHITE_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      956 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16@2x_3.2_WHITE_BLURRED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      760 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16@2x_3.3_WHITE_MASKED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      668 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16@2x_3.4_WHITE_SHADOW.png
--rw-r--r--   0 lgarron    (501) staff       (20)      358 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16_1.0_SIZED_MASK.png
--rw-r--r--   0 lgarron    (501) staff       (20)      433 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16_1.1_FILL_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      429 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16_1.2_FILL.png
--rw-r--r--   0 lgarron    (501) staff       (20)      366 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16_2.1_BLACK_NEGATED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      436 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16_2.2_BLACK_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      465 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16_2.3_BLACK_BLURRED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      465 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16_2.4_BLACK_MASKED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      461 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16_2.5_BLACK_SHADOW.png
--rw-r--r--   0 lgarron    (501) staff       (20)      433 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16_3.1_WHITE_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      518 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16_3.2_WHITE_BLURRED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      501 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16_3.3_WHITE_MASKED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      467 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/16x16_3.4_WHITE_SHADOW.png
--rw-r--r--   0 lgarron    (501) staff       (20)      624 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32@2x_1.0_SIZED_MASK.png
--rw-r--r--   0 lgarron    (501) staff       (20)      956 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32@2x_1.1_FILL_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      859 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32@2x_1.2_FILL.png
--rw-r--r--   0 lgarron    (501) staff       (20)      693 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32@2x_2.1_BLACK_NEGATED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      975 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32@2x_2.2_BLACK_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1006 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32@2x_2.3_BLACK_BLURRED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      938 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32@2x_2.4_BLACK_MASKED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      842 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32@2x_2.5_BLACK_SHADOW.png
--rw-r--r--   0 lgarron    (501) staff       (20)      956 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32@2x_3.1_WHITE_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1508 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32@2x_3.2_WHITE_BLURRED.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1131 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32@2x_3.3_WHITE_MASKED.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1011 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32@2x_3.4_WHITE_SHADOW.png
--rw-r--r--   0 lgarron    (501) staff       (20)      439 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32_1.0_SIZED_MASK.png
--rw-r--r--   0 lgarron    (501) staff       (20)      588 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32_1.1_FILL_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      560 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32_1.2_FILL.png
--rw-r--r--   0 lgarron    (501) staff       (20)      459 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32_2.1_BLACK_NEGATED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      595 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32_2.2_BLACK_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      625 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32_2.3_BLACK_BLURRED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      632 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32_2.4_BLACK_MASKED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      600 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32_2.5_BLACK_SHADOW.png
--rw-r--r--   0 lgarron    (501) staff       (20)      588 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32_3.1_WHITE_COLORIZED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      956 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32_3.2_WHITE_BLURRED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      760 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32_3.3_WHITE_MASKED.png
--rw-r--r--   0 lgarron    (501) staff       (20)      668 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/apple.png-folderify-debug/32x32_3.4_WHITE_SHADOW.png
--rw-r--r--   0 lgarron    (501) staff       (20)    66350 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/cube.png
--rw-r--r--   0 lgarron    (501) staff       (20)    15290 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/folder_outline.png
--rw-r--r--   0 lgarron    (501) staff       (20)    66649 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/octocat.png
--rw-r--r--   0 lgarron    (501) staff       (20)   102544 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/rhombic_hexecontahedron.png
--rw-r--r--   0 lgarron    (501) staff       (20)    23136 2022-03-18 02:03:18.000000 folderify-2.4.0/examples/src/sysprefs.png
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.303169 folderify-2.4.0/folderify/
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.308892 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/
--rw-r--r--   0 lgarron    (501) staff       (20)    17603 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128.png
--rw-r--r--   0 lgarron    (501) staff       (20)    60552 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)      554 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1305 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)    60552 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256.png
--rw-r--r--   0 lgarron    (501) staff       (20)   191981 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1305 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32.png
--rw-r--r--   0 lgarron    (501) staff       (20)     4514 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)   191981 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512.png
--rw-r--r--   0 lgarron    (501) staff       (20)   528334 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512@2x.png
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.316756 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/
--rw-r--r--   0 lgarron    (501) staff       (20)    20653 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128.png
--rw-r--r--   0 lgarron    (501) staff       (20)    76804 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)      692 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1461 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)    76804 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256.png
--rw-r--r--   0 lgarron    (501) staff       (20)   261575 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1473 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32.png
--rw-r--r--   0 lgarron    (501) staff       (20)     5870 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)   261575 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512.png
--rw-r--r--   0 lgarron    (501) staff       (20)   787589 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512@2x.png
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.325950 folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/
--rw-r--r--   0 lgarron    (501) staff       (20)    21366 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128.png
--rw-r--r--   0 lgarron    (501) staff       (20)    68009 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)     3176 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16.png
--rw-r--r--   0 lgarron    (501) staff       (20)     4045 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)    68009 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256.png
--rw-r--r--   0 lgarron    (501) staff       (20)   268431 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)     4029 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32.png
--rw-r--r--   0 lgarron    (501) staff       (20)     7708 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)   268431 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512.png
--rw-r--r--   0 lgarron    (501) staff       (20)  1089689 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512@2x.png
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.333668 folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/
--rw-r--r--   0 lgarron    (501) staff       (20)    17304 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128.png
--rw-r--r--   0 lgarron    (501) staff       (20)    64503 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)      564 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1470 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)    64503 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256.png
--rw-r--r--   0 lgarron    (501) staff       (20)   220247 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)     1475 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32.png
--rw-r--r--   0 lgarron    (501) staff       (20)     4734 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)   220247 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512.png
--rw-r--r--   0 lgarron    (501) staff       (20)   697357 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512@2x.png
--rw-r--r--   0 lgarron    (501) staff       (20)        0 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/__init__.py
--rw-r--r--   0 lgarron    (501) staff       (20)    21364 2023-03-08 05:23:14.000000 folderify-2.4.0/folderify/__main__.py
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.336095 folderify-2.4.0/folderify/lib/
--rw-r--r--   0 lgarron    (501) staff       (20)      261 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/lib/osxiconutils.webloc
--rwxr-xr-x   0 lgarron    (501) staff       (20)    58892 2021-10-21 21:15:48.000000 folderify-2.4.0/folderify/lib/seticon
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.305452 folderify-2.4.0/folderify.egg-info/
--rw-r--r--   0 lgarron    (501) staff       (20)     6451 2023-03-08 05:29:05.000000 folderify-2.4.0/folderify.egg-info/PKG-INFO
--rw-r--r--   0 lgarron    (501) staff       (20)     7184 2023-03-08 05:29:05.000000 folderify-2.4.0/folderify.egg-info/SOURCES.txt
--rw-r--r--   0 lgarron    (501) staff       (20)        1 2023-03-08 05:29:05.000000 folderify-2.4.0/folderify.egg-info/dependency_links.txt
--rw-r--r--   0 lgarron    (501) staff       (20)       55 2023-03-08 05:29:05.000000 folderify-2.4.0/folderify.egg-info/entry_points.txt
--rw-r--r--   0 lgarron    (501) staff       (20)       10 2023-03-08 05:29:05.000000 folderify-2.4.0/folderify.egg-info/top_level.txt
--rw-r--r--   0 lgarron    (501) staff       (20)       38 2023-03-08 05:29:05.338048 folderify-2.4.0/setup.cfg
--rw-r--r--   0 lgarron    (501) staff       (20)     1964 2023-03-08 05:28:19.000000 folderify-2.4.0/setup.py
-drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-03-08 05:29:05.337182 folderify-2.4.0/test/
--rw-r--r--   0 lgarron    (501) staff       (20)     1197 2021-10-21 21:15:48.000000 folderify-2.4.0/test/helpers.sh
--rwxr-xr-x   0 lgarron    (501) staff       (20)     1881 2021-10-27 19:27:56.000000 folderify-2.4.0/test/test.sh
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.160872 folderify-2.4.1/
+-rw-r--r--   0 lgarron    (501) staff       (20)     1022 2023-04-07 03:42:18.000000 folderify-2.4.1/LICENSE.md
+-rw-r--r--   0 lgarron    (501) staff       (20)       55 2023-04-13 21:50:34.000000 folderify-2.4.1/MANIFEST.in
+-rw-r--r--   0 lgarron    (501) staff       (20)     6757 2023-04-13 22:02:16.160713 folderify-2.4.1/PKG-INFO
+-rw-r--r--   0 lgarron    (501) staff       (20)     5884 2023-04-13 22:01:19.000000 folderify-2.4.1/README.md
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.151302 folderify-2.4.1/folderify/
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.153881 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/
+-rw-r--r--   0 lgarron    (501) staff       (20)    17603 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    60552 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)      554 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     1305 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    60552 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   191981 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     1305 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     4514 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   191981 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   528334 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512@2x.png
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.155808 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/
+-rw-r--r--   0 lgarron    (501) staff       (20)    20653 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    76804 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)      692 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     1461 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    76804 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   261575 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     1473 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     5870 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   261575 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   787589 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512@2x.png
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.157922 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/
+-rw-r--r--   0 lgarron    (501) staff       (20)    21366 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    68009 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     3176 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     4045 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    68009 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   268431 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     4029 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     7708 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   268431 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512.png
+-rw-r--r--   0 lgarron    (501) staff       (20)  1089689 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512@2x.png
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.159974 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/
+-rw-r--r--   0 lgarron    (501) staff       (20)    17304 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    64503 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)      564 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     1470 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)    64503 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   220247 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     1475 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32.png
+-rw-r--r--   0 lgarron    (501) staff       (20)     4734 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   220247 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512.png
+-rw-r--r--   0 lgarron    (501) staff       (20)   697357 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512@2x.png
+-rw-r--r--   0 lgarron    (501) staff       (20)        0 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/__init__.py
+-rw-r--r--   0 lgarron    (501) staff       (20)    21698 2023-04-13 22:01:19.000000 folderify-2.4.1/folderify/__main__.py
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.160457 folderify-2.4.1/folderify/lib/
+-rwxr-xr-x   0 lgarron    (501) staff       (20)    58892 2023-04-13 21:50:34.000000 folderify-2.4.1/folderify/lib/seticon
+drwxr-xr-x   0 lgarron    (501) staff       (20)        0 2023-04-13 22:02:16.151919 folderify-2.4.1/folderify.egg-info/
+-rw-r--r--   0 lgarron    (501) staff       (20)     6757 2023-04-13 22:02:16.000000 folderify-2.4.1/folderify.egg-info/PKG-INFO
+-rw-r--r--   0 lgarron    (501) staff       (20)     2783 2023-04-13 22:02:16.000000 folderify-2.4.1/folderify.egg-info/SOURCES.txt
+-rw-r--r--   0 lgarron    (501) staff       (20)        1 2023-04-13 22:02:16.000000 folderify-2.4.1/folderify.egg-info/dependency_links.txt
+-rw-r--r--   0 lgarron    (501) staff       (20)       55 2023-04-13 22:02:16.000000 folderify-2.4.1/folderify.egg-info/entry_points.txt
+-rw-r--r--   0 lgarron    (501) staff       (20)       10 2023-04-13 22:02:16.000000 folderify-2.4.1/folderify.egg-info/top_level.txt
+-rw-r--r--   0 lgarron    (501) staff       (20)       38 2023-04-13 22:02:16.160921 folderify-2.4.1/setup.cfg
+-rw-r--r--   0 lgarron    (501) staff       (20)     1964 2023-04-13 22:01:22.000000 folderify-2.4.1/setup.py
```

### Comparing `folderify-2.4.0/LICENSE.md` & `folderify-2.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/PKG-INFO` & `folderify-2.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folderify
-Version: 2.4.0
+Version: 2.4.1
 Summary: Generate pixel-perfect macOS folder icons in the native style.
 Home-page: https://github.com/lgarron/folderify
 Author: Lucas Garron
 Author-email: code@garron.net
 License: MIT
 Keywords: icon macOS OSX Mac Darwin graphics folder imagemagick
 Platform: UNKNOWN
@@ -17,14 +17,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
+# ⚠️ `folderify` v2 ⚠️
+
+This is folderify v2 (implemented in Python and published to PyPI), which is no longer officially supported. Unless you need folder icons for macOS 10.15 or earlier, please consider updating to folderify v3: https://github.com/lgarron/folderify/tree/main#install
+
+--------
+
 # folderify
 
 ![mask.png + folder = folderified!](examples/png/explanation.png)
 
 Generate pixel-perfect macOS folder icons in the native style.
 
 - Works for OS X 10.5 (Leopard) through macOS 13 (Ventura).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `folderify-2.4.0/README.md` & `folderify-2.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# ⚠️ `folderify` v2 ⚠️
+
+This is folderify v2 (implemented in Python and published to PyPI), which is no longer officially supported. Unless you need folder icons for macOS 10.15 or earlier, please consider updating to folderify v3: https://github.com/lgarron/folderify/tree/main#install
+
+--------
+
 # folderify
 
 ![mask.png + folder = folderified!](examples/png/explanation.png)
 
 Generate pixel-perfect macOS folder icons in the native style.
 
 - Works for OS X 10.5 (Leopard) through macOS 13 (Ventura).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_128x128@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_16x16@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_256x256@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_32x32@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.dark.iconset/icon_512x512@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_128x128@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_16x16@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_256x256@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_32x32@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.BigSur.iconset/icon_512x512@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_128x128@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_16x16@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_256x256@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_32x32@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Leopard.iconset/icon_512x512@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_128x128@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_16x16@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_256x256@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_32x32@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512@2x.png` & `folderify-2.4.1/folderify/GenericFolderIcon.Yosemite.iconset/icon_512x512@2x.png`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify/__main__.py` & `folderify-2.4.1/folderify/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import os
 import os.path
 import platform
 import shutil
 import subprocess
 import sys
 import tempfile
+import time
+import warnings
 
 from string import Template
 
 ################################################################
 
 DEBUG = "FOLDERIFY_DEBUG" in os.environ and os.environ["FOLDERIFY_DEBUG"] == "1"
 OLD_IMPLEMENTATION_FOLDER_STYLES = ["Yosemite", "Leopard"]
@@ -98,14 +100,25 @@
   parser.add_argument(
     "--verbose", "-v",
     action="store_true",
     help="Detailed output.")
 
   ################################################################
 
+  warnings.warn("""
+--------
+
+You are using folderify v2, which is no longer officially supported. Unless you need folder icons for macOS 10.15 or earlier, please consider updating to folderify v3:
+
+https://github.com/lgarron/folderify/tree/main#install
+
+--------
+""", DeprecationWarning)
+  time.sleep(2)
+
   args = parser.parse_args()
 
   if args.mask and not os.path.exists(args.mask):
     parser.error("Mask file does not exist: %s" % args.mask)
 
   if args.target and not os.path.exists(args.target):
     parser.error("Target file/folder does not exist: %s" % args.target)
```

### Comparing `folderify-2.4.0/folderify/lib/seticon` & `folderify-2.4.1/folderify/lib/seticon`

 * *Files identical despite different names*

### Comparing `folderify-2.4.0/folderify.egg-info/PKG-INFO` & `folderify-2.4.1/folderify.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folderify
-Version: 2.4.0
+Version: 2.4.1
 Summary: Generate pixel-perfect macOS folder icons in the native style.
 Home-page: https://github.com/lgarron/folderify
 Author: Lucas Garron
 Author-email: code@garron.net
 License: MIT
 Keywords: icon macOS OSX Mac Darwin graphics folder imagemagick
 Platform: UNKNOWN
@@ -17,14 +17,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
+# ⚠️ `folderify` v2 ⚠️
+
+This is folderify v2 (implemented in Python and published to PyPI), which is no longer officially supported. Unless you need folder icons for macOS 10.15 or earlier, please consider updating to folderify v3: https://github.com/lgarron/folderify/tree/main#install
+
+--------
+
 # folderify
 
 ![mask.png + folder = folderified!](examples/png/explanation.png)
 
 Generate pixel-perfect macOS folder icons in the native style.
 
 - Works for OS X 10.5 (Leopard) through macOS 13 (Ventura).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `folderify-2.4.0/setup.py` & `folderify-2.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Get the long description from the relevant file
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="folderify",
-    version="2.4.0",
+    version="2.4.1",
     description="Generate pixel-perfect macOS folder icons in the native style.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/lgarron/folderify",
 
     author="Lucas Garron",
     author_email="code@garron.net",
```

