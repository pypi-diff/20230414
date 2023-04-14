# Comparing `tmp/statscend-0.1.6.tar.gz` & `tmp/statscend-0.1.7.tar.gz`

## Comparing `statscend-0.1.6.tar` & `statscend-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 statscend-0.1.6/.DS_Store
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 statscend-0.1.6/statscend/__init__.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 statscend-0.1.6/statscend/bn_logistic_regression.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 statscend-0.1.6/statscend/datasets.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 statscend-0.1.6/statscend/linear_regression.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 statscend-0.1.6/statscend/mn_logistic_regression.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 statscend-0.1.6/statscend/ordinal_regression.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 statscend-0.1.6/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 statscend-0.1.6/LICENSE
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 statscend-0.1.6/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 statscend-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    10207 2020-02-02 00:00:00.000000 statscend-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 statscend-0.1.7/.DS_Store
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 statscend-0.1.7/statscend/__init__.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 statscend-0.1.7/statscend/bn_logistic_regression.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 statscend-0.1.7/statscend/datasets.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 statscend-0.1.7/statscend/linear_regression.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 statscend-0.1.7/statscend/mn_logistic_regression.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 statscend-0.1.7/statscend/ordinal_regression.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 statscend-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 statscend-0.1.7/LICENSE
+-rw-r--r--   0        0        0    13214 2020-02-02 00:00:00.000000 statscend-0.1.7/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 statscend-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    15140 2020-02-02 00:00:00.000000 statscend-0.1.7/PKG-INFO
```

### Comparing `statscend-0.1.6/.DS_Store` & `statscend-0.1.7/.DS_Store`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 040a 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0006  ................
-00000050: 0000 0001 0000 1000 0073 0063 0065 006e  .........s.c.e.n
-00000060: 0064 6277 0000 0000 0000 0000 0000 0000  .dbw............
+00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
+00000050: 0000 0001 0000 1000 6277 7370 626c 6f62  ........bwspblob
+00000060: 0000 00c9 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,90 +26,90 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0006 0000 0009  ................
-00000210: 0073 0074 0061 0074 0073 0063 0065 006e  .s.t.a.t.s.c.e.n
-00000220: 0064 6277 7370 626c 6f62 0000 00c9 6270  .dbwspblob....bp
-00000230: 6c69 7374 3030 d701 0203 0405 0607 0809  list00..........
-00000240: 0909 090d 095d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00000250: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-00000260: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00000270: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00000280: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00000290: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-000002a0: 5369 6465 6261 7208 0909 0909 5f10 187b  Sidebar....._..{
-000002b0: 7b31 3537 2c20 3230 307d 2c20 7b37 3730  {157, 200}, {770
-000002c0: 2c20 3530 357d 7d09 0817 2531 3d49 606d  , 505}}...%1=I`m
-000002d0: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-000002e0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-000002f0: 0000 0000 0000 9a00 0000 0900 7300 7400  ............s.t.
-00000300: 6100 7400 7300 6300 6500 6e00 646c 6731  a.t.s.c.e.n.dlg1
-00000310: 5363 6f6d 7000 0000 0000 0000 0000 0000  Scomp...........
-00000320: 0900 7300 7400 6100 7400 7300 6300 6500  ..s.t.a.t.s.c.e.
-00000330: 6e00 646d 6f44 4462 6c6f 6200 0000 08a3  n.dmoDDblob.....
-00000340: 25a8 d15e edc4 4100 0000 0900 7300 7400  %..^..A.....s.t.
-00000350: 6100 7400 7300 6300 6500 6e00 646d 6f64  a.t.s.c.e.n.dmod
-00000360: 4462 6c6f 6200 0000 08a3 25a8 d15e edc4  Dblob.....%..^..
-00000370: 4100 0000 0900 7300 7400 6100 7400 7300  A.....s.t.a.t.s.
-00000380: 6300 6500 6e00 6470 6831 5363 6f6d 7000  c.e.n.dph1Scomp.
-00000390: 0000 0000 0000 0000 0000 0900 7300 7400  ............s.t.
-000003a0: 6100 7400 7300 6300 6500 6e00 6476 5372  a.t.s.c.e.n.dvSr
-000003b0: 6e6c 6f6e 6700 0000 0100 0000 0000 0000  nlong...........
+00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000400: 0000 0000 0000 0000 0000 0008 0000 0004  ................
+00000410: 0064 0069 0073 0074 6277 7370 626c 6f62  .d.i.s.tbwspblob
+00000420: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
+00000430: 0405 0607 0809 0909 090d 095d 5368 6f77  ...........]Show
+00000440: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+00000450: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+00000460: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00000470: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00000480: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00000490: 735b 5368 6f77 5369 6465 6261 7208 0909  s[ShowSidebar...
+000004a0: 0909 5f10 187b 7b32 3639 2c20 3134 367d  .._..{{269, 146}
+000004b0: 2c20 7b37 3730 2c20 3530 357d 7d09 0817  , {770, 505}}...
+000004c0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
+000004d0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
+000004e0: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
+000004f0: 0400 6400 6900 7300 7476 5372 6e6c 6f6e  ..d.i.s.tvSrnlon
+00000500: 6700 0000 0100 0000 0900 7300 7400 6100  g.........s.t.a.
+00000510: 7400 7300 6300 6500 6e00 6462 7773 7062  t.s.c.e.n.dbwspb
+00000520: 6c6f 6200 0000 c962 706c 6973 7430 30d7  lob....bplist00.
+00000530: 0102 0304 0506 0708 0909 0909 0d09 5d53  ..............]S
+00000540: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
+00000550: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
+00000560: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
+00000570: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
+00000580: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
+00000590: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
+000005a0: 0809 0909 095f 1018 7b7b 3135 372c 2032  ....._..{{157, 2
+000005b0: 3030 7d2c 207b 3737 302c 2035 3035 7d7d  00}, {770, 505}}
+000005c0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e99  ...%1=I`myz{|}~.
+000005d0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
+000005e0: 0000 0000 0000 0000 0000 0000 0000 009a  ................
+000005f0: 0000 0009 0073 0074 0061 0074 0073 0063  .....s.t.a.t.s.c
+00000600: 0065 006e 0064 6c67 3153 636f 6d70 0000  .e.n.dlg1Scomp..
+00000610: 0000 0000 0000 0000 0009 0073 0074 0061  ...........s.t.a
+00000620: 0074 0073 0063 0065 006e 0064 6d6f 4444  .t.s.c.e.n.dmoDD
+00000630: 626c 6f62 0000 0008 a325 a8d1 5eed c441  blob.....%..^..A
+00000640: 0000 0009 0073 0074 0061 0074 0073 0063  .....s.t.a.t.s.c
+00000650: 0065 006e 0064 6d6f 6444 626c 6f62 0000  .e.n.dmodDblob..
+00000660: 0008 a325 a8d1 5eed c441 0000 0009 0073  ...%..^..A.....s
+00000670: 0074 0061 0074 0073 0063 0065 006e 0064  .t.a.t.s.c.e.n.d
+00000680: 7068 3153 636f 6d70 0000 0000 0000 0000  ph1Scomp........
+00000690: 0000 0009 0073 0074 0061 0074 0073 0063  .....s.t.a.t.s.c
+000006a0: 0065 006e 0064 7653 726e 6c6f 6e67 0000  .e.n.dvSrnlong..
+000006b0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 000006c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 040a 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -319,15 +319,15 @@
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
 00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
+00001450: 0100 0002 0000 0000 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 000014c0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
```

### Comparing `statscend-0.1.6/statscend/bn_logistic_regression.py` & `statscend-0.1.7/statscend/bn_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.6/statscend/datasets.py` & `statscend-0.1.7/statscend/datasets.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.6/statscend/linear_regression.py` & `statscend-0.1.7/statscend/linear_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.6/statscend/mn_logistic_regression.py` & `statscend-0.1.7/statscend/mn_logistic_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     dv_levels = np.sort(y_var.unique())[1:]
     dv_levels = pd.Series(dv_levels)
 
     coefficients_table = pd.concat(
         [df for df in coefficients_tables], keys=dv_levels)
 
-    return {'summary_table': summary_table, 'coefficients_table': coefficients_table}
+    return {'summary_table': summary_table, 'model_coefficients': coefficients_table}
```

### Comparing `statscend-0.1.6/statscend/ordinal_regression.py` & `statscend-0.1.7/statscend/ordinal_regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import pandas as pd
 from statsmodels.miscmodels.ordinal_model import OrderedModel
 
 
-def ordinal_regression(data, x, y, method='bfgs', distr='logit'):
+def ordinal_regression(data, x, y, distr='logit'):
     if not pd.api.types.is_categorical_dtype(data[y]):
         raise ValueError(
             f"Endogenous variable {y} is not categorical. Please convert the dtype of data['{y}'] to categorical. Please also ensure that the order of levels is correct.")
     mod = OrderedModel(data[y], data[x], distr=distr)
+    method = 'bfgs'
     res = mod.fit(method=method)
 
     # create an empty dictionary
     results = {}
 
     # extract the first table and save it to the dictionary
     summary_table = res.summary().tables[0]
```

### Comparing `statscend-0.1.6/LICENSE` & `statscend-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `statscend-0.1.6/pyproject.toml` & `statscend-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statscend"
-version = "0.1.6"
+version = "0.1.7"
 license = {file = "LICENSE"}
 authors = [
   { name="Hashim Puthiyakath", email="hashputhiyakath@gmail.com" },
 ]
 description = "A Python package for performing various statistical analyses"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `statscend-0.1.6/PKG-INFO` & `statscend-0.1.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,7 @@
-Metadata-Version: 2.1
-Name: statscend
-Version: 0.1.6
-Summary: A Python package for performing various statistical analyses
-Project-URL: Homepage, https://github.com/hashimputhiyakath/statscend
-Project-URL: Bug Tracker, https://github.com/hashimputhiyakath/statscend/issues
-Author-email: Hashim Puthiyakath <hashputhiyakath@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Hashim Puthiyakath
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in
-        all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-        THE SOFTWARE.
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: seaborn
-Requires-Dist: sklearn
-Requires-Dist: statsmodels
-Description-Content-Type: text/markdown
-
 # StatScend
 
 The **statscend** package is a Python library designed to provide a convenient and user-friendly interface for performing statistical analysis. Currently, the library includes a set of functions for fitting and evaluating regression models. More functions will be added soon.
 
 The package is designed to be user-friendly, with intuitive syntax and clear output. It is intended for use by researchers, data scientists.
 Under the hood, **statscend** utiize the `statsmodels` and `sklearn` libraries to provide a range of data analysis and modeling functions. Essentially, this library provides a high-level interface that abstracts away many of the complexities of working with statistical models, making it easy to get started with data analysis in Python.
 
@@ -88,15 +48,15 @@
 This package is licensed under the MIT License.
 
 ---
 
 ## Functions
 
 <details>
-<summary>linear_regression(data, x, y)</summary>
+<summary>linear_regression()</summary>
 The `linear_regression()` function computes a linear regression on one or more predictor variables against a response variable in a given dataset. The function uses the statsmodels package to perform the linear regression analysis and returns a dictionary of four dataframes containing overall model fit measures, regression coefficients, regression summary, and regression diagnostics.
 
 #### Parameters:
 
 - data : pandas DataFrame<br/>
   The data on which to perform the regression.
 
@@ -213,7 +173,127 @@
 
 
 ```
 
 #### Notes
 
 </details>
+
+<details>
+
+<summary>ordinal_regression()</summary>
+
+### ordinal_regression(data, x, y, distr='logit')
+
+The `bi_logistic_regression()` function perform ordinal logistic regression on the specified data.
+
+#### Parameters:
+
+- data : pandas DataFrame<br/>
+  The dataset to use for the regression. It must contain the dependent variable (y) and at least one independent variable (x).
+- x : str<br/>
+  The name of the column in the `data` DataFrame containing the independent variable(s).
+- y : str<br/>
+  The name of the column in the `data` DataFrame containing the dependent variable. The `y` variable must be a pandas categorical variable with an ordered category. If the y variable is not a categorical variable or if the category is not ordered, a ValueError will be raised.
+- distr : str, optional<br/>
+  The distribution to use for the model. Supported values are `probit` or `logit`. Default is `logit`.
+
+#### Returns
+
+The ordinal_logistic_regression function returns a dictionary containing three keys:
+
+- `summary_table`: This key contains a summary table for the regression. The summary table provides information such as the coefficients for the independent variables, the coefficients for the thresholds (i.e., the values that separate the different levels of the dependent variable), the standard errors for the coefficients, the z-scores, and the p-values.
+
+- `model_coefficients`: This key contains the coefficients for the independent variables in the regression. These coefficients represent the estimated effect of each independent variable on the dependent variable, while controlling for the other variables in the model.
+
+-`model_thresholds`: This key contains the coefficients for the dependent variable levels, along with their standard errors, z-scores, and p-values. These coefficients represent the values that separate the different levels of the dependent variable, and are specific to the distribution that was used in the model (`probit` or `logit`).
+
+The output of the function can be saved to a variable. This variable will contain a dictionary with three tables.
+
+`result = ss.ordinal_regression(data=penguins, x='bill_length_mm', y='species')`
+
+To access the dictionary keys, you can use the keys() method.
+`print(results.keys())`
+
+In Jupyter Notebook, you don't need to use print()
+`(results.keys()`
+
+Once you have the dictionary keys, you can display each table by using the key to index into the dictionary. Here's an example:
+
+`print(result['summary_table'])`
+
+`print(result['model_coefficients'])`
+
+`print(result['model_thresholds'])`
+
+#### Examples
+
+```
+
+species_order = ['Adelie', 'Chinstrap', 'Gentoo']
+
+penguins['species'] = pd.Categorical(penguins['species'], categories=species_order, ordered=True)
+
+x = ['bill_length_mm', 'bill_depth_mm]
+y = 'species'
+
+result = ordinal_regression(data=penguins, x=x, y=y)
+
+print(result['model_coefficients'])
+
+```
+
+</details>
+
+<details>
+<summary>mn_logistic_regression()</summary>
+
+### mn_logistic_regression(data, x, y)
+
+The `mn_logistic_regression` function performs multinomial logistic regression analysis on a given dataset.
+
+#### Parameters:
+
+- data: Pandas DataFrame <br/>
+  A Pandas DataFrame containing the data to be analyzed. This data should include both the independent variable(s) and the dependent variable.
+- x: str or list of str<br/>
+  The x argument specifies the column name or names of the independent variable(s) in the data DataFrame. It can be a single column name or a list of column names representing multiple independent variables.
+- y: str <br/>
+  The column name of the dependent variable in the data DataFrame. The y argument is required and must be specified.
+
+#### Returns
+
+The mn_logistic_regression function returns a dictionary containing two keys:
+
+- summary_table: a Pandas DataFrame containing the summary statistics for the analysis. The table includes information such as the number of observations, the model used, and the log-likelihood of the model.
+- model_coefficients: a Pandas DataFrame containing the coefficients for the analysis. The table includes information such as the variable name, the coefficient value, standard error, z-score, p-value, and confidence intervals.
+
+The output of the function can be saved to a variable. This variable will contain a dictionary with two tables.
+
+`result = ss.mn_logistic_regression(data=penguins, x='bill_length_mm', y='species')`
+
+To access the dictionary keys, you can use the keys() method.
+`print(results.keys())`
+
+In Jupyter Notebook, you don't need to use print()
+`(results.keys()`
+
+Once you have the dictionary keys, you can display each table by using the key to index into the dictionary. Here's an example:
+
+`print(result['summary_table'])`
+
+`print(result['model_coefficients'])`
+
+#### Examples
+
+```
+
+x = ['bill_length_mm', 'bill_depth_mm]
+y = 'species'
+
+result = mn_logistic_regression(data=penguins, x=x, y=y)
+
+print(result['model_coefficients'])
+
+```
+
+</details>
```

