# Comparing `tmp/oglio-0.6.0.tar.gz` & `tmp/oglio-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oglio-0.6.0.tar", last modified: Fri Mar 31 00:05:29 2023, max compression
+gzip compressed data, was "oglio-0.7.0.tar", last modified: Fri Apr 14 20:32:52 2023, max compression
```

## Comparing `oglio-0.6.0.tar` & `oglio-0.7.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-31 00:05:29.718515 oglio-0.6.0/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-20 17:57:30.000000 oglio-0.6.0/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1971 2023-03-31 00:05:29.718389 oglio-0.6.0/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1647 2023-01-12 22:07:39.000000 oglio-0.6.0/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-31 00:05:29.715331 oglio-0.6.0/oglio/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       82 2023-02-13 18:01:45.000000 oglio-0.6.0/oglio/OglVersion.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4580 2023-02-13 18:12:30.000000 oglio-0.6.0/oglio/Reader.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3826 2023-01-01 21:43:45.000000 oglio-0.6.0/oglio/Types.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      123 2022-10-13 12:50:37.000000 oglio-0.6.0/oglio/UnsupportedFileTypeException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2111 2022-10-13 16:59:06.000000 oglio-0.6.0/oglio/Writer.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-09 17:46:52.000000 oglio-0.6.0/oglio/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.6.0/oglio/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-31 00:05:29.718214 oglio-0.6.0/oglio/toXmlV10/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1913 2022-08-26 20:55:45.000000 oglio-0.6.0/oglio/toXmlV10/BaseOglToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      569 2022-08-26 20:55:45.000000 oglio-0.6.0/oglio/toXmlV10/BasePyutToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1103 2023-03-30 23:17:17.000000 oglio-0.6.0/oglio/toXmlV10/BaseToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1646 2022-08-29 20:41:51.000000 oglio-0.6.0/oglio/toXmlV10/OglClassesToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5803 2023-03-22 15:11:37.000000 oglio-0.6.0/oglio/toXmlV10/OglLinksToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1598 2022-08-29 20:41:51.000000 oglio-0.6.0/oglio/toXmlV10/OglNotesToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2622 2023-02-12 20:42:00.000000 oglio-0.6.0/oglio/toXmlV10/OglSequenceToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1569 2022-08-29 20:41:51.000000 oglio-0.6.0/oglio/toXmlV10/OglTextsToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6676 2022-10-13 16:38:44.000000 oglio-0.6.0/oglio/toXmlV10/OglToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2787 2022-08-29 20:41:51.000000 oglio-0.6.0/oglio/toXmlV10/OglUseCasesToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13996 2023-02-12 20:43:55.000000 oglio-0.6.0/oglio/toXmlV10/PyutToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3831 2022-08-19 17:25:32.000000 oglio-0.6.0/oglio/toXmlV10/XmlConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-16 17:46:46.000000 oglio-0.6.0/oglio/toXmlV10/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.6.0/oglio/toXmlV10/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-31 00:05:29.716042 oglio-0.6.0/oglio.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1971 2023-03-31 00:05:29.000000 oglio-0.6.0/oglio.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      736 2023-03-31 00:05:29.000000 oglio-0.6.0/oglio.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-03-31 00:05:29.000000 oglio-0.6.0/oglio.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      105 2023-03-31 00:05:29.000000 oglio-0.6.0/oglio.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        6 2023-03-31 00:05:29.000000 oglio-0.6.0/oglio.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-03-31 00:05:29.718546 oglio-0.6.0/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)      964 2023-03-30 23:18:14.000000 oglio-0.6.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-14 20:32:52.375722 oglio-0.7.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-20 17:57:30.000000 oglio-0.7.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-04-14 20:32:52.375592 oglio-0.7.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2011 2023-04-13 20:29:58.000000 oglio-0.7.0/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-14 20:32:52.371967 oglio-0.7.0/oglio/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       82 2023-02-13 18:01:45.000000 oglio-0.7.0/oglio/OglVersion.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4580 2023-02-13 18:12:30.000000 oglio-0.7.0/oglio/Reader.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3826 2023-01-01 21:43:45.000000 oglio-0.7.0/oglio/Types.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      123 2022-10-13 12:50:37.000000 oglio-0.7.0/oglio/UnsupportedFileTypeException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2111 2022-10-13 16:59:06.000000 oglio-0.7.0/oglio/Writer.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-09 17:46:52.000000 oglio-0.7.0/oglio/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.7.0/oglio/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-14 20:32:52.375472 oglio-0.7.0/oglio/toXmlV10/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1913 2022-08-26 20:55:45.000000 oglio-0.7.0/oglio/toXmlV10/BaseOglToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      569 2022-08-26 20:55:45.000000 oglio-0.7.0/oglio/toXmlV10/BasePyutToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1103 2023-03-30 23:17:17.000000 oglio-0.7.0/oglio/toXmlV10/BaseToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1646 2022-08-29 20:41:51.000000 oglio-0.7.0/oglio/toXmlV10/OglClassesToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5803 2023-03-22 15:11:37.000000 oglio-0.7.0/oglio/toXmlV10/OglLinksToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1598 2022-08-29 20:41:51.000000 oglio-0.7.0/oglio/toXmlV10/OglNotesToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2622 2023-02-12 20:42:00.000000 oglio-0.7.0/oglio/toXmlV10/OglSequenceToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1569 2022-08-29 20:41:51.000000 oglio-0.7.0/oglio/toXmlV10/OglTextsToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6676 2022-10-13 16:38:44.000000 oglio-0.7.0/oglio/toXmlV10/OglToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2787 2022-08-29 20:41:51.000000 oglio-0.7.0/oglio/toXmlV10/OglUseCasesToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13996 2023-02-12 20:43:55.000000 oglio-0.7.0/oglio/toXmlV10/PyutToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3831 2022-08-19 17:25:32.000000 oglio-0.7.0/oglio/toXmlV10/XmlConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-16 17:46:46.000000 oglio-0.7.0/oglio/toXmlV10/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.7.0/oglio/toXmlV10/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-14 20:32:52.372522 oglio-0.7.0/oglio.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-04-14 20:32:52.000000 oglio-0.7.0/oglio.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      736 2023-04-14 20:32:52.000000 oglio-0.7.0/oglio.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-14 20:32:52.000000 oglio-0.7.0/oglio.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      105 2023-04-14 20:32:52.000000 oglio-0.7.0/oglio.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        6 2023-04-14 20:32:52.000000 oglio-0.7.0/oglio.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-14 20:32:52.375753 oglio-0.7.0/setup.cfg
+-rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)      964 2023-04-14 19:04:55.000000 oglio-0.7.0/setup.py
```

### Comparing `oglio-0.6.0/LICENSE` & `oglio-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/PKG-INFO` & `oglio-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6f67 6c69  : 2.1.Name: ogli
-00000020: 6f0a 5665 7273 696f 6e3a 2030 2e36 2e30  o.Version: 0.6.0
+00000020: 6f0a 5665 7273 696f 6e3a 2030 2e37 2e30  o.Version: 0.7.0
 00000030: 0a53 756d 6d61 7279 3a20 4578 7465 726e  .Summary: Extern
 00000040: 616c 2050 7975 7420 5065 7273 6973 7465  al Pyut Persiste
 00000050: 6e63 650a 486f 6d65 2d70 6167 653a 2068  nce.Home-page: h
 00000060: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 00000070: 6d2f 6861 7369 6932 3031 312f 6f67 6c69  m/hasii2011/ogli
 00000080: 6f0a 4175 7468 6f72 2d65 6d61 696c 3a20  o.Author-email: 
 00000090: 4875 6d62 6572 746f 2e41 2e53 616e 6368  Humberto.A.Sanch
@@ -63,62 +63,84 @@
 000003e0: 7920 7665 7273 696f 6e20 7468 6520 6c69  y version the li
 000003f0: 6272 6172 792e 2020 4675 7274 6865 726d  brary.  Furtherm
 00000400: 6f72 652c 2061 6c6c 6f77 730a 7468 6520  ore, allows.the 
 00000410: 6465 7665 6c6f 706d 656e 7420 6f66 2061  development of a
 00000420: 6e20 494f 586d 6c20 706c 7567 696e 2066  n IOXml plugin f
 00000430: 6f72 2050 7975 7420 7769 7468 2063 6f6d  or Pyut with com
 00000440: 6d6f 6e20 636f 6465 0a0a 2320 4f76 6572  mon code..# Over
-00000450: 7669 6577 0a0a 0a0a 2d2d 2d2d 2d2d 0a0a  view....------..
-00000460: 0a21 5b48 756d 6265 7274 6f27 7320 4d6f  .![Humberto's Mo
-00000470: 6469 6669 6564 204c 6f67 6f5d 2868 7474  dified Logo](htt
-00000480: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00000490: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f77  sercontent.com/w
-000004a0: 696b 692f 6861 7369 6932 3031 312f 6769  iki/hasii2011/gi
-000004b0: 7474 6f64 6f69 7374 636c 6f6e 652f 696d  ttodoistclone/im
-000004c0: 6167 6573 2f53 696c 6c79 4769 7448 7562  ages/SillyGitHub
-000004d0: 2e70 6e67 290a 0a49 2061 6d20 636f 6e63  .png)..I am conc
-000004e0: 6572 6e65 6420 6162 6f75 7420 4769 7448  erned about GitH
-000004f0: 7562 2773 2043 6f70 696c 6f74 2070 726f  ub's Copilot pro
-00000500: 6a65 6374 0a0a 0a0a 4920 7572 6765 2079  ject....I urge y
-00000510: 6f75 2074 6f20 7265 6164 2061 626f 7574  ou to read about
-00000520: 2074 6865 0a5b 4769 7665 2075 7020 4769   the.[Give up Gi
-00000530: 7448 7562 5d28 6874 7470 733a 2f2f 4769  tHub](https://Gi
-00000540: 7665 5570 4769 7448 7562 2e6f 7267 2920  veUpGitHub.org) 
-00000550: 6361 6d70 6169 676e 2066 726f 6d0a 5b74  campaign from.[t
-00000560: 6865 2053 6f66 7477 6172 6520 4672 6565  he Software Free
-00000570: 646f 6d20 436f 6e73 6572 7661 6e63 795d  dom Conservancy]
-00000580: 2868 7474 7073 3a2f 2f73 6663 6f6e 7365  (https://sfconse
-00000590: 7276 616e 6379 2e6f 7267 292e 0a0a 5768  rvancy.org)...Wh
-000005a0: 696c 6520 4920 646f 206e 6f74 2061 6476  ile I do not adv
-000005b0: 6f63 6174 6520 666f 7220 616c 6c20 7468  ocate for all th
-000005c0: 6520 6973 7375 6573 206c 6973 7465 6420  e issues listed 
-000005d0: 7468 6572 6520 4920 646f 206e 6f74 206c  there I do not l
-000005e0: 696b 6520 7468 6174 0a61 2063 6f6d 7061  ike that.a compa
-000005f0: 6e79 206c 696b 6520 4d69 6372 6f73 6f66  ny like Microsof
-00000600: 7420 6d61 7920 7072 6f66 6974 2066 726f  t may profit fro
-00000610: 6d20 6f70 656e 2073 6f75 7263 6520 7072  m open source pr
-00000620: 6f6a 6563 7473 2e0a 0a49 2063 6f6e 7469  ojects...I conti
-00000630: 6e75 6520 746f 2075 7365 2047 6974 4875  nue to use GitHu
-00000640: 6220 6265 6361 7573 6520 6974 206f 6666  b because it off
-00000650: 6572 7320 7468 6520 7365 7276 6963 6573  ers the services
-00000660: 2049 206e 6565 6420 666f 7220 6672 6565   I need for free
-00000670: 2e20 2042 7574 2c20 4920 636f 6e74 696e  .  But, I contin
-00000680: 7565 0a74 6f20 6d6f 6e69 746f 7220 7468  ue.to monitor th
-00000690: 6569 7220 7465 726d 7320 6f66 2073 6572  eir terms of ser
-000006a0: 7669 6365 2e0a 0a41 6e79 2075 7365 206f  vice...Any use o
-000006b0: 6620 7468 6973 2070 726f 6a65 6374 2773  f this project's
-000006c0: 2063 6f64 6520 6279 2047 6974 4875 6220   code by GitHub 
-000006d0: 436f 7069 6c6f 742c 2070 6173 7420 6f72  Copilot, past or
-000006e0: 2070 7265 7365 6e74 2c20 6973 2064 6f6e   present, is don
-000006f0: 650a 7769 7468 6f75 7420 6d79 2070 6572  e.without my per
-00000700: 6d69 7373 696f 6e2e 2020 4920 646f 206e  mission.  I do n
-00000710: 6f74 2063 6f6e 7365 6e74 2074 6f20 4769  ot consent to Gi
-00000720: 7448 7562 2773 2075 7365 206f 6620 7468  tHub's use of th
-00000730: 6973 2070 726f 6a65 6374 2773 0a63 6f64  is project's.cod
-00000740: 6520 696e 2043 6f70 696c 6f74 2e0a 0a41  e in Copilot...A
-00000750: 2072 6570 6f73 6974 6f72 7920 6f77 6e65   repository owne
-00000760: 7220 6d61 7920 6f70 7420 6f75 7420 6f66  r may opt out of
-00000770: 2043 6f70 696c 6f74 2062 7920 6368 616e   Copilot by chan
-00000780: 6769 6e67 2053 6574 7469 6e67 7320 2d2d  ging Settings --
-00000790: 3e20 4769 7448 7562 2043 6f70 696c 6f74  > GitHub Copilot
-000007a0: 2e0a 0a49 2068 6176 6520 646f 6e65 2073  ...I have done s
-000007b0: 6f2e 0a                                  o..
+00000450: 7669 6577 0a0a 5f5f 5f0a 0a23 2320 4465  view..___..## De
+00000460: 7665 6c6f 7065 7220 4e6f 7465 730a 5468  veloper Notes.Th
+00000470: 6973 2070 726f 6a65 6374 2075 7365 7320  is project uses 
+00000480: 5b62 7569 6c64 6c61 636b 6579 5d28 6874  [buildlackey](ht
+00000490: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000004a0: 2f68 6173 6969 3230 3131 2f62 7569 6c64  /hasii2011/build
+000004b0: 6c61 636b 6579 2920 666f 7220 6461 7920  lackey) for day 
+000004c0: 746f 2064 6179 2064 6576 656c 6f70 6d65  to day developme
+000004d0: 6e74 2062 7569 6c64 730a 0a5f 5f5f 0a0a  nt builds..___..
+000004e0: 5772 6974 7465 6e20 6279 203c 6120 6872  Written by <a hr
+000004f0: 6566 3d22 6d61 696c 746f 3a65 6d61 696c  ef="mailto:email
+00000500: 4068 756d 6265 7274 6f2e 612e 7361 6e63  @humberto.a.sanc
+00000510: 6865 7a2e 6969 4067 6d61 696c 2e63 6f6d  hez.ii@gmail.com
+00000520: 3f73 7562 6a65 6374 3d48 656c 6c6f 2048  ?subject=Hello H
+00000530: 756d 6265 7274 6f22 3e48 756d 6265 7274  umberto">Humbert
+00000540: 6f20 412e 2053 616e 6368 657a 2049 493c  o A. Sanchez II<
+00000550: 2f61 3e20 2028 4329 2032 3032 330a 0a23  /a>  (C) 2023..#
+00000560: 2320 4e6f 7465 0a46 6f72 2061 6c6c 206b  # Note.For all k
+00000570: 696e 6420 6f66 2070 726f 626c 656d 732c  ind of problems,
+00000580: 2072 6571 7565 7374 732c 2065 6e68 616e   requests, enhan
+00000590: 6365 6d65 6e74 732c 2062 7567 2072 6570  cements, bug rep
+000005a0: 6f72 7473 2c20 6574 632e 2c0a 706c 6561  orts, etc.,.plea
+000005b0: 7365 2064 726f 7020 6d65 2061 6e20 652d  se drop me an e-
+000005c0: 6d61 696c 2e0a 200a 5f5f 5f0a 0a21 5b48  mail.. .___..![H
+000005d0: 756d 6265 7274 6f27 7320 4d6f 6469 6669  umberto's Modifi
+000005e0: 6564 204c 6f67 6f5d 2868 7474 7073 3a2f  ed Logo](https:/
+000005f0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00000600: 6f6e 7465 6e74 2e63 6f6d 2f77 696b 692f  ontent.com/wiki/
+00000610: 6861 7369 6932 3031 312f 6769 7474 6f64  hasii2011/gittod
+00000620: 6f69 7374 636c 6f6e 652f 696d 6167 6573  oistclone/images
+00000630: 2f53 696c 6c79 4769 7448 7562 2e70 6e67  /SillyGitHub.png
+00000640: 290a 0a49 2061 6d20 636f 6e63 6572 6e65  )..I am concerne
+00000650: 6420 6162 6f75 7420 4769 7448 7562 2773  d about GitHub's
+00000660: 2043 6f70 696c 6f74 2070 726f 6a65 6374   Copilot project
+00000670: 0a0a 0a0a 4920 7572 6765 2079 6f75 2074  ....I urge you t
+00000680: 6f20 7265 6164 2061 626f 7574 2074 6865  o read about the
+00000690: 0a5b 4769 7665 2075 7020 4769 7448 7562  .[Give up GitHub
+000006a0: 5d28 6874 7470 733a 2f2f 4769 7665 5570  ](https://GiveUp
+000006b0: 4769 7448 7562 2e6f 7267 2920 6361 6d70  GitHub.org) camp
+000006c0: 6169 676e 2066 726f 6d0a 5b74 6865 2053  aign from.[the S
+000006d0: 6f66 7477 6172 6520 4672 6565 646f 6d20  oftware Freedom 
+000006e0: 436f 6e73 6572 7661 6e63 795d 2868 7474  Conservancy](htt
+000006f0: 7073 3a2f 2f73 6663 6f6e 7365 7276 616e  ps://sfconservan
+00000700: 6379 2e6f 7267 292e 0a0a 5768 696c 6520  cy.org)...While 
+00000710: 4920 646f 206e 6f74 2061 6476 6f63 6174  I do not advocat
+00000720: 6520 666f 7220 616c 6c20 7468 6520 6973  e for all the is
+00000730: 7375 6573 206c 6973 7465 6420 7468 6572  sues listed ther
+00000740: 6520 4920 646f 206e 6f74 206c 696b 6520  e I do not like 
+00000750: 7468 6174 0a61 2063 6f6d 7061 6e79 206c  that.a company l
+00000760: 696b 6520 4d69 6372 6f73 6f66 7420 6d61  ike Microsoft ma
+00000770: 7920 7072 6f66 6974 2066 726f 6d20 6f70  y profit from op
+00000780: 656e 2073 6f75 7263 6520 7072 6f6a 6563  en source projec
+00000790: 7473 2e0a 0a49 2063 6f6e 7469 6e75 6520  ts...I continue 
+000007a0: 746f 2075 7365 2047 6974 4875 6220 6265  to use GitHub be
+000007b0: 6361 7573 6520 6974 206f 6666 6572 7320  cause it offers 
+000007c0: 7468 6520 7365 7276 6963 6573 2049 206e  the services I n
+000007d0: 6565 6420 666f 7220 6672 6565 2e20 2042  eed for free.  B
+000007e0: 7574 2c20 4920 636f 6e74 696e 7565 0a74  ut, I continue.t
+000007f0: 6f20 6d6f 6e69 746f 7220 7468 6569 7220  o monitor their 
+00000800: 7465 726d 7320 6f66 2073 6572 7669 6365  terms of service
+00000810: 2e0a 0a41 6e79 2075 7365 206f 6620 7468  ...Any use of th
+00000820: 6973 2070 726f 6a65 6374 2773 2063 6f64  is project's cod
+00000830: 6520 6279 2047 6974 4875 6220 436f 7069  e by GitHub Copi
+00000840: 6c6f 742c 2070 6173 7420 6f72 2070 7265  lot, past or pre
+00000850: 7365 6e74 2c20 6973 2064 6f6e 650a 7769  sent, is done.wi
+00000860: 7468 6f75 7420 6d79 2070 6572 6d69 7373  thout my permiss
+00000870: 696f 6e2e 2020 4920 646f 206e 6f74 2063  ion.  I do not c
+00000880: 6f6e 7365 6e74 2074 6f20 4769 7448 7562  onsent to GitHub
+00000890: 2773 2075 7365 206f 6620 7468 6973 2070  's use of this p
+000008a0: 726f 6a65 6374 2773 0a63 6f64 6520 696e  roject's.code in
+000008b0: 2043 6f70 696c 6f74 2e0a 0a41 2072 6570   Copilot...A rep
+000008c0: 6f73 6974 6f72 7920 6f77 6e65 7220 6d61  ository owner ma
+000008d0: 7920 6f70 7420 6f75 7420 6f66 2043 6f70  y opt out of Cop
+000008e0: 696c 6f74 2062 7920 6368 616e 6769 6e67  ilot by changing
+000008f0: 2053 6574 7469 6e67 7320 2d2d 3e20 4769   Settings --> Gi
+00000900: 7448 7562 2043 6f70 696c 6f74 2e0a 0a49  tHub Copilot...I
+00000910: 2068 6176 6520 646f 6e65 2073 6f2e 0a     have done so..
```

### Comparing `oglio-0.6.0/README.md` & `oglio-0.7.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -43,61 +43,84 @@
 000002a0: 7273 696f 6e20 7468 6520 6c69 6272 6172  rsion the librar
 000002b0: 792e 2020 4675 7274 6865 726d 6f72 652c  y.  Furthermore,
 000002c0: 2061 6c6c 6f77 730a 7468 6520 6465 7665   allows.the deve
 000002d0: 6c6f 706d 656e 7420 6f66 2061 6e20 494f  lopment of an IO
 000002e0: 586d 6c20 706c 7567 696e 2066 6f72 2050  Xml plugin for P
 000002f0: 7975 7420 7769 7468 2063 6f6d 6d6f 6e20  yut with common 
 00000300: 636f 6465 0a0a 2320 4f76 6572 7669 6577  code..# Overview
-00000310: 0a0a 0a0a 2d2d 2d2d 2d2d 0a0a 0a21 5b48  ....------...![H
-00000320: 756d 6265 7274 6f27 7320 4d6f 6469 6669  umberto's Modifi
-00000330: 6564 204c 6f67 6f5d 2868 7474 7073 3a2f  ed Logo](https:/
-00000340: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00000350: 6f6e 7465 6e74 2e63 6f6d 2f77 696b 692f  ontent.com/wiki/
-00000360: 6861 7369 6932 3031 312f 6769 7474 6f64  hasii2011/gittod
-00000370: 6f69 7374 636c 6f6e 652f 696d 6167 6573  oistclone/images
-00000380: 2f53 696c 6c79 4769 7448 7562 2e70 6e67  /SillyGitHub.png
-00000390: 290a 0a49 2061 6d20 636f 6e63 6572 6e65  )..I am concerne
-000003a0: 6420 6162 6f75 7420 4769 7448 7562 2773  d about GitHub's
-000003b0: 2043 6f70 696c 6f74 2070 726f 6a65 6374   Copilot project
-000003c0: 0a0a 0a0a 4920 7572 6765 2079 6f75 2074  ....I urge you t
-000003d0: 6f20 7265 6164 2061 626f 7574 2074 6865  o read about the
-000003e0: 0a5b 4769 7665 2075 7020 4769 7448 7562  .[Give up GitHub
-000003f0: 5d28 6874 7470 733a 2f2f 4769 7665 5570  ](https://GiveUp
-00000400: 4769 7448 7562 2e6f 7267 2920 6361 6d70  GitHub.org) camp
-00000410: 6169 676e 2066 726f 6d0a 5b74 6865 2053  aign from.[the S
-00000420: 6f66 7477 6172 6520 4672 6565 646f 6d20  oftware Freedom 
-00000430: 436f 6e73 6572 7661 6e63 795d 2868 7474  Conservancy](htt
-00000440: 7073 3a2f 2f73 6663 6f6e 7365 7276 616e  ps://sfconservan
-00000450: 6379 2e6f 7267 292e 0a0a 5768 696c 6520  cy.org)...While 
-00000460: 4920 646f 206e 6f74 2061 6476 6f63 6174  I do not advocat
-00000470: 6520 666f 7220 616c 6c20 7468 6520 6973  e for all the is
-00000480: 7375 6573 206c 6973 7465 6420 7468 6572  sues listed ther
-00000490: 6520 4920 646f 206e 6f74 206c 696b 6520  e I do not like 
-000004a0: 7468 6174 0a61 2063 6f6d 7061 6e79 206c  that.a company l
-000004b0: 696b 6520 4d69 6372 6f73 6f66 7420 6d61  ike Microsoft ma
-000004c0: 7920 7072 6f66 6974 2066 726f 6d20 6f70  y profit from op
-000004d0: 656e 2073 6f75 7263 6520 7072 6f6a 6563  en source projec
-000004e0: 7473 2e0a 0a49 2063 6f6e 7469 6e75 6520  ts...I continue 
-000004f0: 746f 2075 7365 2047 6974 4875 6220 6265  to use GitHub be
-00000500: 6361 7573 6520 6974 206f 6666 6572 7320  cause it offers 
-00000510: 7468 6520 7365 7276 6963 6573 2049 206e  the services I n
-00000520: 6565 6420 666f 7220 6672 6565 2e20 2042  eed for free.  B
-00000530: 7574 2c20 4920 636f 6e74 696e 7565 0a74  ut, I continue.t
-00000540: 6f20 6d6f 6e69 746f 7220 7468 6569 7220  o monitor their 
-00000550: 7465 726d 7320 6f66 2073 6572 7669 6365  terms of service
-00000560: 2e0a 0a41 6e79 2075 7365 206f 6620 7468  ...Any use of th
-00000570: 6973 2070 726f 6a65 6374 2773 2063 6f64  is project's cod
-00000580: 6520 6279 2047 6974 4875 6220 436f 7069  e by GitHub Copi
-00000590: 6c6f 742c 2070 6173 7420 6f72 2070 7265  lot, past or pre
-000005a0: 7365 6e74 2c20 6973 2064 6f6e 650a 7769  sent, is done.wi
-000005b0: 7468 6f75 7420 6d79 2070 6572 6d69 7373  thout my permiss
-000005c0: 696f 6e2e 2020 4920 646f 206e 6f74 2063  ion.  I do not c
-000005d0: 6f6e 7365 6e74 2074 6f20 4769 7448 7562  onsent to GitHub
-000005e0: 2773 2075 7365 206f 6620 7468 6973 2070  's use of this p
-000005f0: 726f 6a65 6374 2773 0a63 6f64 6520 696e  roject's.code in
-00000600: 2043 6f70 696c 6f74 2e0a 0a41 2072 6570   Copilot...A rep
-00000610: 6f73 6974 6f72 7920 6f77 6e65 7220 6d61  ository owner ma
-00000620: 7920 6f70 7420 6f75 7420 6f66 2043 6f70  y opt out of Cop
-00000630: 696c 6f74 2062 7920 6368 616e 6769 6e67  ilot by changing
-00000640: 2053 6574 7469 6e67 7320 2d2d 3e20 4769   Settings --> Gi
-00000650: 7448 7562 2043 6f70 696c 6f74 2e0a 0a49  tHub Copilot...I
-00000660: 2068 6176 6520 646f 6e65 2073 6f2e 0a     have done so..
+00000310: 0a0a 5f5f 5f0a 0a23 2320 4465 7665 6c6f  ..___..## Develo
+00000320: 7065 7220 4e6f 7465 730a 5468 6973 2070  per Notes.This p
+00000330: 726f 6a65 6374 2075 7365 7320 5b62 7569  roject uses [bui
+00000340: 6c64 6c61 636b 6579 5d28 6874 7470 733a  ldlackey](https:
+00000350: 2f2f 6769 7468 7562 2e63 6f6d 2f68 6173  //github.com/has
+00000360: 6969 3230 3131 2f62 7569 6c64 6c61 636b  ii2011/buildlack
+00000370: 6579 2920 666f 7220 6461 7920 746f 2064  ey) for day to d
+00000380: 6179 2064 6576 656c 6f70 6d65 6e74 2062  ay development b
+00000390: 7569 6c64 730a 0a5f 5f5f 0a0a 5772 6974  uilds..___..Writ
+000003a0: 7465 6e20 6279 203c 6120 6872 6566 3d22  ten by <a href="
+000003b0: 6d61 696c 746f 3a65 6d61 696c 4068 756d  mailto:email@hum
+000003c0: 6265 7274 6f2e 612e 7361 6e63 6865 7a2e  berto.a.sanchez.
+000003d0: 6969 4067 6d61 696c 2e63 6f6d 3f73 7562  ii@gmail.com?sub
+000003e0: 6a65 6374 3d48 656c 6c6f 2048 756d 6265  ject=Hello Humbe
+000003f0: 7274 6f22 3e48 756d 6265 7274 6f20 412e  rto">Humberto A.
+00000400: 2053 616e 6368 657a 2049 493c 2f61 3e20   Sanchez II</a> 
+00000410: 2028 4329 2032 3032 330a 0a23 2320 4e6f   (C) 2023..## No
+00000420: 7465 0a46 6f72 2061 6c6c 206b 696e 6420  te.For all kind 
+00000430: 6f66 2070 726f 626c 656d 732c 2072 6571  of problems, req
+00000440: 7565 7374 732c 2065 6e68 616e 6365 6d65  uests, enhanceme
+00000450: 6e74 732c 2062 7567 2072 6570 6f72 7473  nts, bug reports
+00000460: 2c20 6574 632e 2c0a 706c 6561 7365 2064  , etc.,.please d
+00000470: 726f 7020 6d65 2061 6e20 652d 6d61 696c  rop me an e-mail
+00000480: 2e0a 200a 5f5f 5f0a 0a21 5b48 756d 6265  .. .___..![Humbe
+00000490: 7274 6f27 7320 4d6f 6469 6669 6564 204c  rto's Modified L
+000004a0: 6f67 6f5d 2868 7474 7073 3a2f 2f72 6177  ogo](https://raw
+000004b0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000004c0: 6e74 2e63 6f6d 2f77 696b 692f 6861 7369  nt.com/wiki/hasi
+000004d0: 6932 3031 312f 6769 7474 6f64 6f69 7374  i2011/gittodoist
+000004e0: 636c 6f6e 652f 696d 6167 6573 2f53 696c  clone/images/Sil
+000004f0: 6c79 4769 7448 7562 2e70 6e67 290a 0a49  lyGitHub.png)..I
+00000500: 2061 6d20 636f 6e63 6572 6e65 6420 6162   am concerned ab
+00000510: 6f75 7420 4769 7448 7562 2773 2043 6f70  out GitHub's Cop
+00000520: 696c 6f74 2070 726f 6a65 6374 0a0a 0a0a  ilot project....
+00000530: 4920 7572 6765 2079 6f75 2074 6f20 7265  I urge you to re
+00000540: 6164 2061 626f 7574 2074 6865 0a5b 4769  ad about the.[Gi
+00000550: 7665 2075 7020 4769 7448 7562 5d28 6874  ve up GitHub](ht
+00000560: 7470 733a 2f2f 4769 7665 5570 4769 7448  tps://GiveUpGitH
+00000570: 7562 2e6f 7267 2920 6361 6d70 6169 676e  ub.org) campaign
+00000580: 2066 726f 6d0a 5b74 6865 2053 6f66 7477   from.[the Softw
+00000590: 6172 6520 4672 6565 646f 6d20 436f 6e73  are Freedom Cons
+000005a0: 6572 7661 6e63 795d 2868 7474 7073 3a2f  ervancy](https:/
+000005b0: 2f73 6663 6f6e 7365 7276 616e 6379 2e6f  /sfconservancy.o
+000005c0: 7267 292e 0a0a 5768 696c 6520 4920 646f  rg)...While I do
+000005d0: 206e 6f74 2061 6476 6f63 6174 6520 666f   not advocate fo
+000005e0: 7220 616c 6c20 7468 6520 6973 7375 6573  r all the issues
+000005f0: 206c 6973 7465 6420 7468 6572 6520 4920   listed there I 
+00000600: 646f 206e 6f74 206c 696b 6520 7468 6174  do not like that
+00000610: 0a61 2063 6f6d 7061 6e79 206c 696b 6520  .a company like 
+00000620: 4d69 6372 6f73 6f66 7420 6d61 7920 7072  Microsoft may pr
+00000630: 6f66 6974 2066 726f 6d20 6f70 656e 2073  ofit from open s
+00000640: 6f75 7263 6520 7072 6f6a 6563 7473 2e0a  ource projects..
+00000650: 0a49 2063 6f6e 7469 6e75 6520 746f 2075  .I continue to u
+00000660: 7365 2047 6974 4875 6220 6265 6361 7573  se GitHub becaus
+00000670: 6520 6974 206f 6666 6572 7320 7468 6520  e it offers the 
+00000680: 7365 7276 6963 6573 2049 206e 6565 6420  services I need 
+00000690: 666f 7220 6672 6565 2e20 2042 7574 2c20  for free.  But, 
+000006a0: 4920 636f 6e74 696e 7565 0a74 6f20 6d6f  I continue.to mo
+000006b0: 6e69 746f 7220 7468 6569 7220 7465 726d  nitor their term
+000006c0: 7320 6f66 2073 6572 7669 6365 2e0a 0a41  s of service...A
+000006d0: 6e79 2075 7365 206f 6620 7468 6973 2070  ny use of this p
+000006e0: 726f 6a65 6374 2773 2063 6f64 6520 6279  roject's code by
+000006f0: 2047 6974 4875 6220 436f 7069 6c6f 742c   GitHub Copilot,
+00000700: 2070 6173 7420 6f72 2070 7265 7365 6e74   past or present
+00000710: 2c20 6973 2064 6f6e 650a 7769 7468 6f75  , is done.withou
+00000720: 7420 6d79 2070 6572 6d69 7373 696f 6e2e  t my permission.
+00000730: 2020 4920 646f 206e 6f74 2063 6f6e 7365    I do not conse
+00000740: 6e74 2074 6f20 4769 7448 7562 2773 2075  nt to GitHub's u
+00000750: 7365 206f 6620 7468 6973 2070 726f 6a65  se of this proje
+00000760: 6374 2773 0a63 6f64 6520 696e 2043 6f70  ct's.code in Cop
+00000770: 696c 6f74 2e0a 0a41 2072 6570 6f73 6974  ilot...A reposit
+00000780: 6f72 7920 6f77 6e65 7220 6d61 7920 6f70  ory owner may op
+00000790: 7420 6f75 7420 6f66 2043 6f70 696c 6f74  t out of Copilot
+000007a0: 2062 7920 6368 616e 6769 6e67 2053 6574   by changing Set
+000007b0: 7469 6e67 7320 2d2d 3e20 4769 7448 7562  tings --> GitHub
+000007c0: 2043 6f70 696c 6f74 2e0a 0a49 2068 6176   Copilot...I hav
+000007d0: 6520 646f 6e65 2073 6f2e 0a              e done so..
```

### Comparing `oglio-0.6.0/oglio/Reader.py` & `oglio-0.7.0/oglio/Reader.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/Types.py` & `oglio-0.7.0/oglio/Types.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/Writer.py` & `oglio-0.7.0/oglio/Writer.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/toXmlV10/BaseOglToDom.py` & `oglio-0.7.0/oglio/toXmlV10/BaseOglToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/toXmlV10/BasePyutToDom.py` & `oglio-0.7.0/oglio/toXmlV10/BasePyutToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/toXmlV10/BaseToDom.py` & `oglio-0.7.0/oglio/toXmlV10/BaseToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/toXmlV10/OglClassesToDom.py` & `oglio-0.7.0/oglio/toXmlV10/OglClassesToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/toXmlV10/OglLinksToDom.py` & `oglio-0.7.0/oglio/toXmlV10/OglLinksToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/toXmlV10/OglNotesToDom.py` & `oglio-0.7.0/oglio/toXmlV10/OglNotesToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/toXmlV10/OglSequenceToDom.py` & `oglio-0.7.0/oglio/toXmlV10/OglSequenceToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/toXmlV10/OglTextsToDom.py` & `oglio-0.7.0/oglio/toXmlV10/OglTextsToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/toXmlV10/OglToDom.py` & `oglio-0.7.0/oglio/toXmlV10/OglToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/toXmlV10/OglUseCasesToDom.py` & `oglio-0.7.0/oglio/toXmlV10/OglUseCasesToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/toXmlV10/PyutToDom.py` & `oglio-0.7.0/oglio/toXmlV10/PyutToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio/toXmlV10/XmlConstants.py` & `oglio-0.7.0/oglio/toXmlV10/XmlConstants.py`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/oglio.egg-info/PKG-INFO` & `oglio-0.7.0/oglio.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6f67 6c69  : 2.1.Name: ogli
-00000020: 6f0a 5665 7273 696f 6e3a 2030 2e36 2e30  o.Version: 0.6.0
+00000020: 6f0a 5665 7273 696f 6e3a 2030 2e37 2e30  o.Version: 0.7.0
 00000030: 0a53 756d 6d61 7279 3a20 4578 7465 726e  .Summary: Extern
 00000040: 616c 2050 7975 7420 5065 7273 6973 7465  al Pyut Persiste
 00000050: 6e63 650a 486f 6d65 2d70 6167 653a 2068  nce.Home-page: h
 00000060: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 00000070: 6d2f 6861 7369 6932 3031 312f 6f67 6c69  m/hasii2011/ogli
 00000080: 6f0a 4175 7468 6f72 2d65 6d61 696c 3a20  o.Author-email: 
 00000090: 4875 6d62 6572 746f 2e41 2e53 616e 6368  Humberto.A.Sanch
@@ -63,62 +63,84 @@
 000003e0: 7920 7665 7273 696f 6e20 7468 6520 6c69  y version the li
 000003f0: 6272 6172 792e 2020 4675 7274 6865 726d  brary.  Furtherm
 00000400: 6f72 652c 2061 6c6c 6f77 730a 7468 6520  ore, allows.the 
 00000410: 6465 7665 6c6f 706d 656e 7420 6f66 2061  development of a
 00000420: 6e20 494f 586d 6c20 706c 7567 696e 2066  n IOXml plugin f
 00000430: 6f72 2050 7975 7420 7769 7468 2063 6f6d  or Pyut with com
 00000440: 6d6f 6e20 636f 6465 0a0a 2320 4f76 6572  mon code..# Over
-00000450: 7669 6577 0a0a 0a0a 2d2d 2d2d 2d2d 0a0a  view....------..
-00000460: 0a21 5b48 756d 6265 7274 6f27 7320 4d6f  .![Humberto's Mo
-00000470: 6469 6669 6564 204c 6f67 6f5d 2868 7474  dified Logo](htt
-00000480: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00000490: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f77  sercontent.com/w
-000004a0: 696b 692f 6861 7369 6932 3031 312f 6769  iki/hasii2011/gi
-000004b0: 7474 6f64 6f69 7374 636c 6f6e 652f 696d  ttodoistclone/im
-000004c0: 6167 6573 2f53 696c 6c79 4769 7448 7562  ages/SillyGitHub
-000004d0: 2e70 6e67 290a 0a49 2061 6d20 636f 6e63  .png)..I am conc
-000004e0: 6572 6e65 6420 6162 6f75 7420 4769 7448  erned about GitH
-000004f0: 7562 2773 2043 6f70 696c 6f74 2070 726f  ub's Copilot pro
-00000500: 6a65 6374 0a0a 0a0a 4920 7572 6765 2079  ject....I urge y
-00000510: 6f75 2074 6f20 7265 6164 2061 626f 7574  ou to read about
-00000520: 2074 6865 0a5b 4769 7665 2075 7020 4769   the.[Give up Gi
-00000530: 7448 7562 5d28 6874 7470 733a 2f2f 4769  tHub](https://Gi
-00000540: 7665 5570 4769 7448 7562 2e6f 7267 2920  veUpGitHub.org) 
-00000550: 6361 6d70 6169 676e 2066 726f 6d0a 5b74  campaign from.[t
-00000560: 6865 2053 6f66 7477 6172 6520 4672 6565  he Software Free
-00000570: 646f 6d20 436f 6e73 6572 7661 6e63 795d  dom Conservancy]
-00000580: 2868 7474 7073 3a2f 2f73 6663 6f6e 7365  (https://sfconse
-00000590: 7276 616e 6379 2e6f 7267 292e 0a0a 5768  rvancy.org)...Wh
-000005a0: 696c 6520 4920 646f 206e 6f74 2061 6476  ile I do not adv
-000005b0: 6f63 6174 6520 666f 7220 616c 6c20 7468  ocate for all th
-000005c0: 6520 6973 7375 6573 206c 6973 7465 6420  e issues listed 
-000005d0: 7468 6572 6520 4920 646f 206e 6f74 206c  there I do not l
-000005e0: 696b 6520 7468 6174 0a61 2063 6f6d 7061  ike that.a compa
-000005f0: 6e79 206c 696b 6520 4d69 6372 6f73 6f66  ny like Microsof
-00000600: 7420 6d61 7920 7072 6f66 6974 2066 726f  t may profit fro
-00000610: 6d20 6f70 656e 2073 6f75 7263 6520 7072  m open source pr
-00000620: 6f6a 6563 7473 2e0a 0a49 2063 6f6e 7469  ojects...I conti
-00000630: 6e75 6520 746f 2075 7365 2047 6974 4875  nue to use GitHu
-00000640: 6220 6265 6361 7573 6520 6974 206f 6666  b because it off
-00000650: 6572 7320 7468 6520 7365 7276 6963 6573  ers the services
-00000660: 2049 206e 6565 6420 666f 7220 6672 6565   I need for free
-00000670: 2e20 2042 7574 2c20 4920 636f 6e74 696e  .  But, I contin
-00000680: 7565 0a74 6f20 6d6f 6e69 746f 7220 7468  ue.to monitor th
-00000690: 6569 7220 7465 726d 7320 6f66 2073 6572  eir terms of ser
-000006a0: 7669 6365 2e0a 0a41 6e79 2075 7365 206f  vice...Any use o
-000006b0: 6620 7468 6973 2070 726f 6a65 6374 2773  f this project's
-000006c0: 2063 6f64 6520 6279 2047 6974 4875 6220   code by GitHub 
-000006d0: 436f 7069 6c6f 742c 2070 6173 7420 6f72  Copilot, past or
-000006e0: 2070 7265 7365 6e74 2c20 6973 2064 6f6e   present, is don
-000006f0: 650a 7769 7468 6f75 7420 6d79 2070 6572  e.without my per
-00000700: 6d69 7373 696f 6e2e 2020 4920 646f 206e  mission.  I do n
-00000710: 6f74 2063 6f6e 7365 6e74 2074 6f20 4769  ot consent to Gi
-00000720: 7448 7562 2773 2075 7365 206f 6620 7468  tHub's use of th
-00000730: 6973 2070 726f 6a65 6374 2773 0a63 6f64  is project's.cod
-00000740: 6520 696e 2043 6f70 696c 6f74 2e0a 0a41  e in Copilot...A
-00000750: 2072 6570 6f73 6974 6f72 7920 6f77 6e65   repository owne
-00000760: 7220 6d61 7920 6f70 7420 6f75 7420 6f66  r may opt out of
-00000770: 2043 6f70 696c 6f74 2062 7920 6368 616e   Copilot by chan
-00000780: 6769 6e67 2053 6574 7469 6e67 7320 2d2d  ging Settings --
-00000790: 3e20 4769 7448 7562 2043 6f70 696c 6f74  > GitHub Copilot
-000007a0: 2e0a 0a49 2068 6176 6520 646f 6e65 2073  ...I have done s
-000007b0: 6f2e 0a                                  o..
+00000450: 7669 6577 0a0a 5f5f 5f0a 0a23 2320 4465  view..___..## De
+00000460: 7665 6c6f 7065 7220 4e6f 7465 730a 5468  veloper Notes.Th
+00000470: 6973 2070 726f 6a65 6374 2075 7365 7320  is project uses 
+00000480: 5b62 7569 6c64 6c61 636b 6579 5d28 6874  [buildlackey](ht
+00000490: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000004a0: 2f68 6173 6969 3230 3131 2f62 7569 6c64  /hasii2011/build
+000004b0: 6c61 636b 6579 2920 666f 7220 6461 7920  lackey) for day 
+000004c0: 746f 2064 6179 2064 6576 656c 6f70 6d65  to day developme
+000004d0: 6e74 2062 7569 6c64 730a 0a5f 5f5f 0a0a  nt builds..___..
+000004e0: 5772 6974 7465 6e20 6279 203c 6120 6872  Written by <a hr
+000004f0: 6566 3d22 6d61 696c 746f 3a65 6d61 696c  ef="mailto:email
+00000500: 4068 756d 6265 7274 6f2e 612e 7361 6e63  @humberto.a.sanc
+00000510: 6865 7a2e 6969 4067 6d61 696c 2e63 6f6d  hez.ii@gmail.com
+00000520: 3f73 7562 6a65 6374 3d48 656c 6c6f 2048  ?subject=Hello H
+00000530: 756d 6265 7274 6f22 3e48 756d 6265 7274  umberto">Humbert
+00000540: 6f20 412e 2053 616e 6368 657a 2049 493c  o A. Sanchez II<
+00000550: 2f61 3e20 2028 4329 2032 3032 330a 0a23  /a>  (C) 2023..#
+00000560: 2320 4e6f 7465 0a46 6f72 2061 6c6c 206b  # Note.For all k
+00000570: 696e 6420 6f66 2070 726f 626c 656d 732c  ind of problems,
+00000580: 2072 6571 7565 7374 732c 2065 6e68 616e   requests, enhan
+00000590: 6365 6d65 6e74 732c 2062 7567 2072 6570  cements, bug rep
+000005a0: 6f72 7473 2c20 6574 632e 2c0a 706c 6561  orts, etc.,.plea
+000005b0: 7365 2064 726f 7020 6d65 2061 6e20 652d  se drop me an e-
+000005c0: 6d61 696c 2e0a 200a 5f5f 5f0a 0a21 5b48  mail.. .___..![H
+000005d0: 756d 6265 7274 6f27 7320 4d6f 6469 6669  umberto's Modifi
+000005e0: 6564 204c 6f67 6f5d 2868 7474 7073 3a2f  ed Logo](https:/
+000005f0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00000600: 6f6e 7465 6e74 2e63 6f6d 2f77 696b 692f  ontent.com/wiki/
+00000610: 6861 7369 6932 3031 312f 6769 7474 6f64  hasii2011/gittod
+00000620: 6f69 7374 636c 6f6e 652f 696d 6167 6573  oistclone/images
+00000630: 2f53 696c 6c79 4769 7448 7562 2e70 6e67  /SillyGitHub.png
+00000640: 290a 0a49 2061 6d20 636f 6e63 6572 6e65  )..I am concerne
+00000650: 6420 6162 6f75 7420 4769 7448 7562 2773  d about GitHub's
+00000660: 2043 6f70 696c 6f74 2070 726f 6a65 6374   Copilot project
+00000670: 0a0a 0a0a 4920 7572 6765 2079 6f75 2074  ....I urge you t
+00000680: 6f20 7265 6164 2061 626f 7574 2074 6865  o read about the
+00000690: 0a5b 4769 7665 2075 7020 4769 7448 7562  .[Give up GitHub
+000006a0: 5d28 6874 7470 733a 2f2f 4769 7665 5570  ](https://GiveUp
+000006b0: 4769 7448 7562 2e6f 7267 2920 6361 6d70  GitHub.org) camp
+000006c0: 6169 676e 2066 726f 6d0a 5b74 6865 2053  aign from.[the S
+000006d0: 6f66 7477 6172 6520 4672 6565 646f 6d20  oftware Freedom 
+000006e0: 436f 6e73 6572 7661 6e63 795d 2868 7474  Conservancy](htt
+000006f0: 7073 3a2f 2f73 6663 6f6e 7365 7276 616e  ps://sfconservan
+00000700: 6379 2e6f 7267 292e 0a0a 5768 696c 6520  cy.org)...While 
+00000710: 4920 646f 206e 6f74 2061 6476 6f63 6174  I do not advocat
+00000720: 6520 666f 7220 616c 6c20 7468 6520 6973  e for all the is
+00000730: 7375 6573 206c 6973 7465 6420 7468 6572  sues listed ther
+00000740: 6520 4920 646f 206e 6f74 206c 696b 6520  e I do not like 
+00000750: 7468 6174 0a61 2063 6f6d 7061 6e79 206c  that.a company l
+00000760: 696b 6520 4d69 6372 6f73 6f66 7420 6d61  ike Microsoft ma
+00000770: 7920 7072 6f66 6974 2066 726f 6d20 6f70  y profit from op
+00000780: 656e 2073 6f75 7263 6520 7072 6f6a 6563  en source projec
+00000790: 7473 2e0a 0a49 2063 6f6e 7469 6e75 6520  ts...I continue 
+000007a0: 746f 2075 7365 2047 6974 4875 6220 6265  to use GitHub be
+000007b0: 6361 7573 6520 6974 206f 6666 6572 7320  cause it offers 
+000007c0: 7468 6520 7365 7276 6963 6573 2049 206e  the services I n
+000007d0: 6565 6420 666f 7220 6672 6565 2e20 2042  eed for free.  B
+000007e0: 7574 2c20 4920 636f 6e74 696e 7565 0a74  ut, I continue.t
+000007f0: 6f20 6d6f 6e69 746f 7220 7468 6569 7220  o monitor their 
+00000800: 7465 726d 7320 6f66 2073 6572 7669 6365  terms of service
+00000810: 2e0a 0a41 6e79 2075 7365 206f 6620 7468  ...Any use of th
+00000820: 6973 2070 726f 6a65 6374 2773 2063 6f64  is project's cod
+00000830: 6520 6279 2047 6974 4875 6220 436f 7069  e by GitHub Copi
+00000840: 6c6f 742c 2070 6173 7420 6f72 2070 7265  lot, past or pre
+00000850: 7365 6e74 2c20 6973 2064 6f6e 650a 7769  sent, is done.wi
+00000860: 7468 6f75 7420 6d79 2070 6572 6d69 7373  thout my permiss
+00000870: 696f 6e2e 2020 4920 646f 206e 6f74 2063  ion.  I do not c
+00000880: 6f6e 7365 6e74 2074 6f20 4769 7448 7562  onsent to GitHub
+00000890: 2773 2075 7365 206f 6620 7468 6973 2070  's use of this p
+000008a0: 726f 6a65 6374 2773 0a63 6f64 6520 696e  roject's.code in
+000008b0: 2043 6f70 696c 6f74 2e0a 0a41 2072 6570   Copilot...A rep
+000008c0: 6f73 6974 6f72 7920 6f77 6e65 7220 6d61  ository owner ma
+000008d0: 7920 6f70 7420 6f75 7420 6f66 2043 6f70  y opt out of Cop
+000008e0: 696c 6f74 2062 7920 6368 616e 6769 6e67  ilot by changing
+000008f0: 2053 6574 7469 6e67 7320 2d2d 3e20 4769   Settings --> Gi
+00000900: 7448 7562 2043 6f70 696c 6f74 2e0a 0a49  tHub Copilot...I
+00000910: 2068 6176 6520 646f 6e65 2073 6f2e 0a     have done so..
```

### Comparing `oglio-0.6.0/oglio.egg-info/SOURCES.txt` & `oglio-0.7.0/oglio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oglio-0.6.0/setup.py` & `oglio-0.7.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="oglio",
-    version="0.6.0",
+    version="0.7.0",
     author_email='Humberto.A.Sanchez.II@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='External Pyut Persistence',
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/hasii2011/oglio",
@@ -23,14 +23,14 @@
     ],
     package_data={
         'oglio':          ['py.typed'],
         'oglio.toXmlV10': ['py.typed']
     },
     install_requires=[
         'wxPython==4.2.0',
-        'hasiihelper~=0.1.0',
-        'hasiicommon~=0.2.1',
-        'pyutmodel~=1.4.2',
-        'ogl~=0.70.22',
-        'untanglepyut~=0.6.41',
+        'hasiihelper~=0.2.0',
+        'hasiicommon~=0.2.2',
+        'pyutmodel~=1.4.3',
+        'ogl~=0.70.26',
+        'untanglepyut~=0.6.50',
     ],
 )
```

