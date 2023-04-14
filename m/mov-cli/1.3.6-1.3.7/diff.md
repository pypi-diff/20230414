# Comparing `tmp/mov_cli-1.3.6.tar.gz` & `tmp/mov_cli-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-1.3.6.tar", max compression
+gzip compressed data, was "mov_cli-1.3.7.tar", max compression
```

## Comparing `mov_cli-1.3.6.tar` & `mov_cli-1.3.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0    35149 2023-04-14 17:59:26.855614 mov_cli-1.3.6/LICENSE
--rw-r--r--   0        0        0     6941 2023-04-14 17:59:26.855614 mov_cli-1.3.6/README.md
--rw-r--r--   0        0        0        0 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/__init__.py
--rw-r--r--   0        0        0     2701 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/__main__.py
--rw-r--r--   0        0        0       19 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/__version__.py
--rw-r--r--   0        0        0        1 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/__init__.py
--rw-r--r--   0        0        0      823 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/doodstream.py
--rw-r--r--   0        0        0       71 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/NOTICE
--rw-r--r--   0        0        0        1 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/__init__.py
--rw-r--r--   0        0        0      169 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/allsportsdaily.py
--rw-r--r--   0        0        0      957 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/cr7sports.py
--rw-r--r--   0        0        0      256 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/enjoy4hd.py
--rw-r--r--   0        0        0      141 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/fabtech.py
--rw-r--r--   0        0        0      218 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/gameshdlive.py
--rw-r--r--   0        0        0      443 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/livestreames.py
--rw-r--r--   0        0        0      320 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/methstreams.py
--rw-r--r--   0        0        0      156 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/motornews.py
--rw-r--r--   0        0        0      873 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/onestream.py
--rw-r--r--   0        0        0      891 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/onionlive.py
--rw-r--r--   0        0        0      615 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/onionstream.py
--rw-r--r--   0        0        0      457 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/poscitech.py
--rw-r--r--   0        0        0      638 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/rainostreams.py
--rw-r--r--   0        0        0      358 2023-04-14 17:59:26.855614 mov_cli-1.3.6/mov_cli/extractors/scdn/ripple.py
--rw-r--r--   0        0        0      406 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/extractors/scdn/techclips.py
--rw-r--r--   0        0        0      417 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/extractors/scdn/techstips.py
--rw-r--r--   0        0        0     1333 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/extractors/scdn/weakstream.py
--rw-r--r--   0        0        0        0 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/players/__init__.py
--rw-r--r--   0        0        0     2227 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/players/mpv.py
--rw-r--r--   0        0        0     1669 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/players/vlc.py
--rw-r--r--   0        0        0        0 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/utils/__init__.py
--rw-r--r--   0        0        0     2246 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/utils/dbs.py
--rw-r--r--   0        0        0     2731 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/utils/httpclient.py
--rw-r--r--   0        0        0     6133 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/utils/jsunpack.py
--rw-r--r--   0        0        0     2269 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/utils/lang.py
--rw-r--r--   0        0        0     1465 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/utils/player.py
--rw-r--r--   0        0        0     1009 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/utils/provider.py
--rw-r--r--   0        0        0     8808 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/utils/scraper.py
--rw-r--r--   0        0        0        0 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/__init__.py
--rw-r--r--   0        0        0    10930 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/actvid.py
--rw-r--r--   0        0        0     4129 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/animefox.py
--rw-r--r--   0        0        0     4058 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/dopebox.py
--rw-r--r--   0        0        0     1931 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/einthusan.py
--rw-r--r--   0        0        0     1718 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/eja.py
--rw-r--r--   0        0        0     2978 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/gogoanime.py
--rw-r--r--   0        0        0     7104 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/kinox.py
--rw-r--r--   0        0        0     3718 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/kisscartoon.py
--rw-r--r--   0        0        0     4875 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/olgply.py
--rw-r--r--   0        0        0     2491 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/openloadmov.py
--rw-r--r--   0        0        0     2545 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/redundant_kimcartoon.py
--rw-r--r--   0        0        0     4524 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/remotestream.py
--rw-r--r--   0        0        0     4416 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/scdn.py
--rw-r--r--   0        0        0     4067 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/sflix.py
--rw-r--r--   0        0        0     1604 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/solar.py
--rw-r--r--   0        0        0     2120 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/streamblasters.py
--rw-r--r--   0        0        0     1346 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/tamilyogi.py
--rw-r--r--   0        0        0     2877 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/turkish123.py
--rw-r--r--   0        0        0     4474 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/viewasian.py
--rw-r--r--   0        0        0     3365 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/watchasian.py
--rw-r--r--   0        0        0     3947 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/wlext.py
--rw-r--r--   0        0        0     3479 2023-04-14 17:59:26.859614 mov_cli-1.3.6/mov_cli/websites/yoturkish.py
--rw-r--r--   0        0        0      734 2023-04-14 17:59:26.859614 mov_cli-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     7877 1970-01-01 00:00:00.000000 mov_cli-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-14 21:52:28.594490 mov_cli-1.3.7/LICENSE
+-rw-r--r--   0        0        0     6941 2023-04-14 21:52:28.594490 mov_cli-1.3.7/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/__init__.py
+-rw-r--r--   0        0        0     2701 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/__main__.py
+-rw-r--r--   0        0        0       19 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/__version__.py
+-rw-r--r--   0        0        0        1 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/__init__.py
+-rw-r--r--   0        0        0      823 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/doodstream.py
+-rw-r--r--   0        0        0       71 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/NOTICE
+-rw-r--r--   0        0        0        1 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/allsportsdaily.py
+-rw-r--r--   0        0        0      957 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/cr7sports.py
+-rw-r--r--   0        0        0      256 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/enjoy4hd.py
+-rw-r--r--   0        0        0      141 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/fabtech.py
+-rw-r--r--   0        0        0      218 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/gameshdlive.py
+-rw-r--r--   0        0        0      443 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/livestreames.py
+-rw-r--r--   0        0        0      320 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/methstreams.py
+-rw-r--r--   0        0        0      156 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/motornews.py
+-rw-r--r--   0        0        0      873 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/onestream.py
+-rw-r--r--   0        0        0      891 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/onionlive.py
+-rw-r--r--   0        0        0      615 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/onionstream.py
+-rw-r--r--   0        0        0      457 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/poscitech.py
+-rw-r--r--   0        0        0      638 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/rainostreams.py
+-rw-r--r--   0        0        0      358 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/ripple.py
+-rw-r--r--   0        0        0      406 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/techclips.py
+-rw-r--r--   0        0        0      417 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/techstips.py
+-rw-r--r--   0        0        0     1333 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/extractors/scdn/weakstream.py
+-rw-r--r--   0        0        0        0 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/players/__init__.py
+-rw-r--r--   0        0        0     2227 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/players/mpv.py
+-rw-r--r--   0        0        0     1669 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/players/vlc.py
+-rw-r--r--   0        0        0        0 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2246 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/utils/dbs.py
+-rw-r--r--   0        0        0     2731 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/utils/httpclient.py
+-rw-r--r--   0        0        0     6133 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/utils/jsunpack.py
+-rw-r--r--   0        0        0     2269 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/utils/lang.py
+-rw-r--r--   0        0        0     1465 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/utils/player.py
+-rw-r--r--   0        0        0     1009 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/utils/provider.py
+-rw-r--r--   0        0        0     8808 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/utils/scraper.py
+-rw-r--r--   0        0        0        0 2023-04-14 21:52:28.594490 mov_cli-1.3.7/mov_cli/websites/__init__.py
+-rw-r--r--   0        0        0    10948 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/actvid.py
+-rw-r--r--   0        0        0     4129 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/animefox.py
+-rw-r--r--   0        0        0     4058 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/dopebox.py
+-rw-r--r--   0        0        0     1931 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/einthusan.py
+-rw-r--r--   0        0        0     1718 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/eja.py
+-rw-r--r--   0        0        0     2978 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/gogoanime.py
+-rw-r--r--   0        0        0     7104 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/kinox.py
+-rw-r--r--   0        0        0     3718 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/kisscartoon.py
+-rw-r--r--   0        0        0     4875 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/olgply.py
+-rw-r--r--   0        0        0     2491 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/openloadmov.py
+-rw-r--r--   0        0        0     2545 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/redundant_kimcartoon.py
+-rw-r--r--   0        0        0     4524 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/remotestream.py
+-rw-r--r--   0        0        0     4416 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/scdn.py
+-rw-r--r--   0        0        0     4067 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/sflix.py
+-rw-r--r--   0        0        0     1604 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/solar.py
+-rw-r--r--   0        0        0     2120 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/streamblasters.py
+-rw-r--r--   0        0        0     1346 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/tamilyogi.py
+-rw-r--r--   0        0        0     2877 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/turkish123.py
+-rw-r--r--   0        0        0     4474 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/viewasian.py
+-rw-r--r--   0        0        0     3365 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/watchasian.py
+-rw-r--r--   0        0        0     3947 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/wlext.py
+-rw-r--r--   0        0        0     3479 2023-04-14 21:52:28.598490 mov_cli-1.3.7/mov_cli/websites/yoturkish.py
+-rw-r--r--   0        0        0      734 2023-04-14 21:52:28.598490 mov_cli-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     7877 1970-01-01 00:00:00.000000 mov_cli-1.3.7/PKG-INFO
```

### Comparing `mov_cli-1.3.6/LICENSE` & `mov_cli-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/README.md` & `mov_cli-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/__main__.py` & `mov_cli-1.3.7/mov_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/extractors/doodstream.py` & `mov_cli-1.3.7/mov_cli/extractors/doodstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/extractors/scdn/cr7sports.py` & `mov_cli-1.3.7/mov_cli/extractors/scdn/cr7sports.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/extractors/scdn/onestream.py` & `mov_cli-1.3.7/mov_cli/extractors/scdn/onestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/extractors/scdn/onionlive.py` & `mov_cli-1.3.7/mov_cli/extractors/scdn/onionlive.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/extractors/scdn/onionstream.py` & `mov_cli-1.3.7/mov_cli/extractors/scdn/onionstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/extractors/scdn/rainostreams.py` & `mov_cli-1.3.7/mov_cli/extractors/scdn/rainostreams.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/extractors/scdn/weakstream.py` & `mov_cli-1.3.7/mov_cli/extractors/scdn/weakstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/players/mpv.py` & `mov_cli-1.3.7/mov_cli/players/mpv.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/players/vlc.py` & `mov_cli-1.3.7/mov_cli/players/vlc.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/utils/dbs.py` & `mov_cli-1.3.7/mov_cli/utils/dbs.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/utils/httpclient.py` & `mov_cli-1.3.7/mov_cli/utils/httpclient.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/utils/jsunpack.py` & `mov_cli-1.3.7/mov_cli/utils/jsunpack.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/utils/lang.py` & `mov_cli-1.3.7/mov_cli/utils/lang.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/utils/player.py` & `mov_cli-1.3.7/mov_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/utils/provider.py` & `mov_cli-1.3.7/mov_cli/utils/provider.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/utils/scraper.py` & `mov_cli-1.3.7/mov_cli/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/actvid.py` & `mov_cli-1.3.7/mov_cli/websites/actvid.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,16 @@
         return bytes(u, "utf-8")
 
     def md5(self, data):
         return hashlib.md5(data).digest()
 
     def get_key(self, salt, key):
         x = self.md5(key + salt)
-        while len(currentkey := x) < 48:
+        currentkey = x
+        while len(currentkey) < 48:
             x = self.md5(x + key + salt)
             currentkey += x
         return currentkey
 
     def unpad(self, s):
         return s[: -ord(s[len(s) - 1 :])]
```

### Comparing `mov_cli-1.3.6/mov_cli/websites/animefox.py` & `mov_cli-1.3.7/mov_cli/websites/animefox.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/dopebox.py` & `mov_cli-1.3.7/mov_cli/websites/dopebox.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/einthusan.py` & `mov_cli-1.3.7/mov_cli/websites/einthusan.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/eja.py` & `mov_cli-1.3.7/mov_cli/websites/eja.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/gogoanime.py` & `mov_cli-1.3.7/mov_cli/websites/gogoanime.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/kinox.py` & `mov_cli-1.3.7/mov_cli/websites/kinox.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/kisscartoon.py` & `mov_cli-1.3.7/mov_cli/websites/kisscartoon.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/olgply.py` & `mov_cli-1.3.7/mov_cli/websites/olgply.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/openloadmov.py` & `mov_cli-1.3.7/mov_cli/websites/openloadmov.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/redundant_kimcartoon.py` & `mov_cli-1.3.7/mov_cli/websites/redundant_kimcartoon.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/remotestream.py` & `mov_cli-1.3.7/mov_cli/websites/remotestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/scdn.py` & `mov_cli-1.3.7/mov_cli/websites/scdn.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/sflix.py` & `mov_cli-1.3.7/mov_cli/websites/sflix.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/solar.py` & `mov_cli-1.3.7/mov_cli/websites/solar.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/streamblasters.py` & `mov_cli-1.3.7/mov_cli/websites/streamblasters.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/tamilyogi.py` & `mov_cli-1.3.7/mov_cli/websites/tamilyogi.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/turkish123.py` & `mov_cli-1.3.7/mov_cli/websites/turkish123.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/viewasian.py` & `mov_cli-1.3.7/mov_cli/websites/viewasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/watchasian.py` & `mov_cli-1.3.7/mov_cli/websites/watchasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/wlext.py` & `mov_cli-1.3.7/mov_cli/websites/wlext.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/mov_cli/websites/yoturkish.py` & `mov_cli-1.3.7/mov_cli/websites/yoturkish.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.3.6/pyproject.toml` & `mov_cli-1.3.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mov-cli"
-version = "1.3.6"
+version = "1.3.7"
 description = "A cli tool to browse and watch Movies/Shows/TV/Sports. "
 authors = ["Pain <painedposeidon444@gmail.com>"]
 maintainers = ["Ananas <r3tr0ananas@hotmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "mov_cli"}]
 repository = "https://github.com/mov-cli/mov-cli"
```

### Comparing `mov_cli-1.3.6/PKG-INFO` & `mov_cli-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 1.3.6
+Version: 1.3.7
 Summary: A cli tool to browse and watch Movies/Shows/TV/Sports. 
 Home-page: https://github.com/mov-cli/mov-cli
 License: GPLv3
 Author: Pain
 Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas
 Maintainer-email: r3tr0ananas@hotmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 1.3.6 Summary: A cli tool to
+Metadata-Version: 2.1 Name: mov-cli Version: 1.3.7 Summary: A cli tool to
 browse and watch Movies/Shows/TV/Sports. Home-page: https://github.com/mov-cli/
 mov-cli License: GPLv3 Author: Pain Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas Maintainer-email: r3tr0ananas@hotmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 beautifulsoup4 (>=4.11.2,<5.0.0) Requires-Dist: httpx (>=0.24.0,<0.25.0)
```

