# Comparing `tmp/fookebox-0.7.3.tar.gz` & `tmp/fookebox-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fookebox-0.7.3.tar", last modified: Sun Dec 13 03:12:12 2015, max compression
+gzip compressed data, was "fookebox-1.0.0.tar", last modified: Fri Apr 14 00:56:09 2023, max compression
```

## Comparing `fookebox-0.7.3.tar` & `fookebox-1.0.0.tar`

### file list

```diff
@@ -1,122 +1,50 @@
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/docs/
--rw-r--r--   0 stefan    (1027) stefan    (1027)     5451 2015-12-13 03:10:15.000000 fookebox-0.7.3/docs/changes.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)     6647 2015-02-15 00:31:02.000000 fookebox-0.7.3/docs/config.txt
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/config/
--rw-r--r--   0 stefan    (1027) stefan    (1027)        0 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/config/__init__.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     2817 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/config/deployment.ini_tmpl
--rw-r--r--   0 stefan    (1027) stefan    (1027)     2668 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/config/environment.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     2418 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/config/middleware.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1509 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/config/routing.py
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/controllers/
--rw-r--r--   0 stefan    (1027) stefan    (1027)        0 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/controllers/__init__.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     2519 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/controllers/error.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     8418 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/controllers/jukebox.py
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/i18n/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/i18n/de/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/i18n/de/LC_MESSAGES/
--rw-r--r--   0 stefan    (1027) stefan    (1027)     2050 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/i18n/de/LC_MESSAGES/fookebox.mo
--rw-r--r--   0 stefan    (1027) stefan    (1027)     4421 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/i18n/de/LC_MESSAGES/fookebox.po
--rw-r--r--   0 stefan    (1027) stefan    (1027)     3847 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/i18n/fookebox.pot
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/lib/
--rw-r--r--   0 stefan    (1027) stefan    (1027)        0 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/lib/__init__.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)      594 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/lib/app_globals.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)      530 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/lib/base.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)      273 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/lib/helpers.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1019 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/lib/util.py
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/model/
--rw-r--r--   0 stefan    (1027) stefan    (1027)        0 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/model/__init__.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     3194 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/model/albumart.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     5649 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/model/jukebox.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     4694 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/model/mpdconn.py
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/css/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/css/bootstrap/
--rw-r--r--   0 stefan    (1027) stefan    (1027)   121260 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/public/css/bootstrap/bootstrap.css
--rw-r--r--   0 stefan    (1027) stefan    (1027)    54416 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/public/css/bootstrap/bootstrap.css.map
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/css/classic/
--rw-r--r--   0 stefan    (1027) stefan    (1027)      384 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/css/classic/style-mobile.css
--rw-r--r--   0 stefan    (1027) stefan    (1027)     5158 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/css/classic/style.css
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/css/fonts/
--rw-r--r--   0 stefan    (1027) stefan    (1027)    20127 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/public/css/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 stefan    (1027) stefan    (1027)   108738 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/public/css/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 stefan    (1027) stefan    (1027)    45404 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/public/css/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 stefan    (1027) stefan    (1027)    23424 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/public/css/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 stefan    (1027) stefan    (1027)    18028 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/public/css/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/css/fookstrap/
--rw-r--r--   0 stefan    (1027) stefan    (1027)     3722 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/public/css/fookstrap/fookebox.css
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/img/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/img/classic/
--rw-r--r--   0 stefan    (1027) stefan    (1027)      741 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/artist.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      607 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/control_next.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      598 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/control_pause.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      592 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/control_play.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      614 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/control_prev.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      770 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/control_rebuild.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      634 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/control_voldown.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      650 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/control_volup.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      715 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/delete.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      240 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/li.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      206 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/msg-bl.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      201 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/msg-br.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      203 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/msg-tl.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      210 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/msg-tr.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      385 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/music.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      346 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/nocover.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      673 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/progress.gif
--rw-r--r--   0 stefan    (1027) stefan    (1027)      704 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/queue.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      610 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/sound.png
--rw-r--r--   0 stefan    (1027) stefan    (1027)      793 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/img/classic/time.png
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/js/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/js/bootstrap/
--rw-r--r--   0 stefan    (1027) stefan    (1027)    36868 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/public/js/bootstrap/bootstrap.js
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/js/fookebox/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/js/fookebox/classic/
--rw-r--r--   0 stefan    (1027) stefan    (1027)    16545 2015-12-13 02:22:29.000000 fookebox-0.7.3/fookebox/public/js/fookebox/classic/client.js
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/js/fookebox/fookstrap/
--rw-r--r--   0 stefan    (1027) stefan    (1027)    13374 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/public/js/fookebox/fookstrap/fookebox.js
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/js/fookebox/i18n/
--rw-r--r--   0 stefan    (1027) stefan    (1027)      367 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/js/fookebox/i18n/de.js
--rw-r--r--   0 stefan    (1027) stefan    (1027)       98 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/js/fookebox/i18n/i18n.js
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/js/jquery/
--rw-r--r--   0 stefan    (1027) stefan    (1027)    95957 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/public/js/jquery/jquery-1.11.3.min.js
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/public/js/jquery-ui/
--rw-r--r--   0 stefan    (1027) stefan    (1027)   469356 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/js/jquery-ui/jquery-ui.js
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1150 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/public/favicon.ico
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/templates/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/templates/classic/
--rw-r--r--   0 stefan    (1027) stefan    (1027)      992 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/templates/classic/base.tpl
--rw-r--r--   0 stefan    (1027) stefan    (1027)     2100 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/templates/classic/browse-menu.tpl
--rw-r--r--   0 stefan    (1027) stefan    (1027)      604 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/templates/classic/client.tpl
--rw-r--r--   0 stefan    (1027) stefan    (1027)      370 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/templates/classic/error.tpl
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1273 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/templates/classic/playing.tpl
--rw-r--r--   0 stefan    (1027) stefan    (1027)      185 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/templates/classic/playlist.tpl
--rw-r--r--   0 stefan    (1027) stefan    (1027)       63 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/templates/classic/status.tpl
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/templates/fookstrap/
--rw-r--r--   0 stefan    (1027) stefan    (1027)     4717 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/templates/fookstrap/client.tpl
--rw-r--r--   0 stefan    (1027) stefan    (1027)      631 2015-12-13 03:10:15.000000 fookebox-0.7.3/fookebox/templates/fookstrap/error.tpl
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/tests/
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox/tests/functional/
--rw-r--r--   0 stefan    (1027) stefan    (1027)        0 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/tests/functional/__init__.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)      195 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/tests/functional/test_jukebox.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1018 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/tests/__init__.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)    15630 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/tests/test_models.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)        0 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/__init__.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)      440 2015-02-15 00:31:02.000000 fookebox-0.7.3/fookebox/websetup.py
-drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox.egg-info/
--rw-r--r--   0 stefan    (1027) stefan    (1027)      997 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox.egg-info/PKG-INFO
--rw-r--r--   0 stefan    (1027) stefan    (1027)     3141 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox.egg-info/SOURCES.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)        1 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox.egg-info/dependency_links.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)      125 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox.egg-info/entry_points.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)        1 2015-02-15 01:36:09.000000 fookebox-0.7.3/fookebox.egg-info/not-zip-safe
--rw-r--r--   0 stefan    (1027) stefan    (1027)       19 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox.egg-info/paster_plugins.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)       24 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox.egg-info/requires.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)        9 2015-12-13 03:12:12.000000 fookebox-0.7.3/fookebox.egg-info/top_level.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)    35147 2015-02-15 00:31:02.000000 fookebox-0.7.3/COPYING
--rw-r--r--   0 stefan    (1027) stefan    (1027)      128 2015-02-15 00:31:02.000000 fookebox-0.7.3/CREDITS.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)      274 2015-02-15 00:31:02.000000 fookebox-0.7.3/MANIFEST.in
--rw-r--r--   0 stefan    (1027) stefan    (1027)      315 2015-02-15 00:31:02.000000 fookebox-0.7.3/README.txt
--rw-r--r--   0 stefan    (1027) stefan    (1027)     1709 2015-12-13 03:10:15.000000 fookebox-0.7.3/setup.py
--rw-r--r--   0 stefan    (1027) stefan    (1027)      997 2015-12-13 03:12:12.000000 fookebox-0.7.3/PKG-INFO
--rw-r--r--   0 stefan    (1027) stefan    (1027)      559 2015-12-13 03:12:12.000000 fookebox-0.7.3/setup.cfg
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    34523 2023-04-14 00:54:11.000000 fookebox-1.0.0/COPYING
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1762 2023-04-14 00:56:09.432418 fookebox-1.0.0/PKG-INFO
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      886 2023-04-14 00:54:11.000000 fookebox-1.0.0/README.md
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       89 2023-04-14 00:54:11.000000 fookebox-1.0.0/pyproject.toml
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1735 2023-04-14 00:56:09.432418 fookebox-1.0.0/setup.cfg
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      720 2023-04-14 00:54:40.000000 fookebox-1.0.0/src/fookebox/__init__.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     4529 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/autoqueue.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1991 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/config.py
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/css/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)   121457 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/css/bootstrap.min.css
+-rw-r--r--   0 stefan    (1027) stefan    (1027)   540434 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/css/bootstrap.min.css.map
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     6178 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/css/fookebox.css
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/fonts/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    20127 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 stefan    (1027) stefan    (1027)   108738 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    45404 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    23424 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    18028 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     3860 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/fookebox.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    13514 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/handlers.py
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/i18n/
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/i18n/de/
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/i18n/de/LC_MESSAGES/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1106 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/i18n/de/LC_MESSAGES/fookebox.mo
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/js/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    39680 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/js/bootstrap.min.js
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    13894 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/js/fookebox.js
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      958 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/js/i18n-de.js
+-rw-r--r--   0 stefan    (1027) stefan    (1027)      832 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/js/i18n.js
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    97163 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/js/jquery-1.12.4.min.js
+-rw-r--r--   0 stefan    (1027) stefan    (1027)   255084 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/js/jquery-ui.min.js
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1895 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/mpd.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/py.typed
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox/templates/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     5302 2023-04-14 00:54:11.000000 fookebox-1.0.0/src/fookebox/templates/client.html
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/src/fookebox.egg-info/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1762 2023-04-14 00:56:09.000000 fookebox-1.0.0/src/fookebox.egg-info/PKG-INFO
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     1147 2023-04-14 00:56:09.000000 fookebox-1.0.0/src/fookebox.egg-info/SOURCES.txt
+-rw-r--r--   0 stefan    (1027) stefan    (1027)        1 2023-04-14 00:56:09.000000 fookebox-1.0.0/src/fookebox.egg-info/dependency_links.txt
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       52 2023-04-14 00:56:09.000000 fookebox-1.0.0/src/fookebox.egg-info/entry_points.txt
+-rw-r--r--   0 stefan    (1027) stefan    (1027)       87 2023-04-14 00:56:09.000000 fookebox-1.0.0/src/fookebox.egg-info/requires.txt
+-rw-r--r--   0 stefan    (1027) stefan    (1027)        9 2023-04-14 00:56:09.000000 fookebox-1.0.0/src/fookebox.egg-info/top_level.txt
+drwxr-xr-x   0 stefan    (1027) stefan    (1027)        0 2023-04-14 00:56:09.432418 fookebox-1.0.0/tests/
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    13312 2023-04-14 00:54:11.000000 fookebox-1.0.0/tests/test_auto_queue.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     4864 2023-04-14 00:54:11.000000 fookebox-1.0.0/tests/test_config.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)    24552 2023-04-14 00:54:11.000000 fookebox-1.0.0/tests/test_handlers.py
+-rw-r--r--   0 stefan    (1027) stefan    (1027)     6389 2023-04-14 00:54:11.000000 fookebox-1.0.0/tests/test_template.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fookebox-0.7.3/fookebox/lib/util.py` & `fookebox-1.0.0/src/fookebox/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,16 @@
-# fookebox, https://github.com/cockroach/fookebox
-#
-# Copyright (C) 2007-2014 Stefan Ott. All rights reserved.
+# fookebox, https://code.ott.net/fookebox/
+# Copyright (c) 2007-2023 Stefan Ott. all rights reserved.
 #
 # This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, version 3.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# GNU Affero General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-import os
-
-class FileSystem(object):
-	@staticmethod
-	def exists(path):
-		return os.path.exists(path.encode('utf8'))
-
-	@staticmethod
-	def isdir(path):
-		return os.path.isdir(path.encode('utf8'))
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-	@staticmethod
-	def listdir(path):
-		return os.listdir(path.encode('utf8'))
+__version__ = '1.0.0'
```

### Comparing `fookebox-0.7.3/fookebox/public/css/bootstrap/bootstrap.css` & `fookebox-1.0.0/src/fookebox/css/bootstrap.min.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 /*!
- * Bootstrap v3.3.6 (http://getbootstrap.com)
- * Copyright 2011-2015 Twitter, Inc.
+ * Bootstrap v3.4.1 (https://getbootstrap.com/)
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
- *//*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */html{font-family:sans-serif;-webkit-text-size-adjust:100%;-ms-text-size-adjust:100%}body{margin:0}article,aside,details,figcaption,figure,footer,header,hgroup,main,menu,nav,section,summary{display:block}audio,canvas,progress,video{display:inline-block;vertical-align:baseline}audio:not([controls]){display:none;height:0}[hidden],template{display:none}a{background-color:transparent}a:active,a:hover{outline:0}abbr[title]{border-bottom:1px dotted}b,strong{font-weight:700}dfn{font-style:italic}h1{margin:.67em 0;font-size:2em}mark{color:#000;background:#ff0}small{font-size:80%}sub,sup{position:relative;font-size:75%;line-height:0;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}img{border:0}svg:not(:root){overflow:hidden}figure{margin:1em 40px}hr{height:0;-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box}pre{overflow:auto}code,kbd,pre,samp{font-family:monospace,monospace;font-size:1em}button,input,optgroup,select,textarea{margin:0;font:inherit;color:inherit}button{overflow:visible}button,select{text-transform:none}button,html input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer}button[disabled],html input[disabled]{cursor:default}button::-moz-focus-inner,input::-moz-focus-inner{padding:0;border:0}input{line-height:normal}input[type=checkbox],input[type=radio]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;padding:0}input[type=number]::-webkit-inner-spin-button,input[type=number]::-webkit-outer-spin-button{height:auto}input[type=search]{-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;-webkit-appearance:textfield}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}fieldset{padding:.35em .625em .75em;margin:0 2px;border:1px solid silver}legend{padding:0;border:0}textarea{overflow:auto}optgroup{font-weight:700}table{border-spacing:0;border-collapse:collapse}td,th{padding:0}/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */@media print{*,:after,:before{color:#000!important;text-shadow:none!important;background:0 0!important;-webkit-box-shadow:none!important;box-shadow:none!important}a,a:visited{text-decoration:underline}a[href]:after{content:" (" attr(href) ")"}abbr[title]:after{content:" (" attr(title) ")"}a[href^="javascript:"]:after,a[href^="#"]:after{content:""}blockquote,pre{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}img,tr{page-break-inside:avoid}img{max-width:100%!important}h2,h3,p{orphans:3;widows:3}h2,h3{page-break-after:avoid}.navbar{display:none}.btn>.caret,.dropup>.btn>.caret{border-top-color:#000!important}.label{border:1px solid #000}.table{border-collapse:collapse!important}.table td,.table th{background-color:#fff!important}.table-bordered td,.table-bordered th{border:1px solid #ddd!important}}@font-face{font-family:'Glyphicons Halflings';src:url(../fonts/glyphicons-halflings-regular.eot);src:url(../fonts/glyphicons-halflings-regular.eot?#iefix) format('embedded-opentype'),url(../fonts/glyphicons-halflings-regular.woff2) format('woff2'),url(../fonts/glyphicons-halflings-regular.woff) format('woff'),url(../fonts/glyphicons-halflings-regular.ttf) format('truetype'),url(../fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular) format('svg')}.glyphicon{position:relative;top:1px;display:inline-block;font-family:'Glyphicons Halflings';font-style:normal;font-weight:400;line-height:1;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.glyphicon-asterisk:before{content:"\002a"}.glyphicon-plus:before{content:"\002b"}.glyphicon-eur:before,.glyphicon-euro:before{content:"\20ac"}.glyphicon-minus:before{content:"\2212"}.glyphicon-cloud:before{content:"\2601"}.glyphicon-envelope:before{content:"\2709"}.glyphicon-pencil:before{content:"\270f"}.glyphicon-glass:before{content:"\e001"}.glyphicon-music:before{content:"\e002"}.glyphicon-search:before{content:"\e003"}.glyphicon-heart:before{content:"\e005"}.glyphicon-star:before{content:"\e006"}.glyphicon-star-empty:before{content:"\e007"}.glyphicon-user:before{content:"\e008"}.glyphicon-film:before{content:"\e009"}.glyphicon-th-large:before{content:"\e010"}.glyphicon-th:before{content:"\e011"}.glyphicon-th-list:before{content:"\e012"}.glyphicon-ok:before{content:"\e013"}.glyphicon-remove:before{content:"\e014"}.glyphicon-zoom-in:before{content:"\e015"}.glyphicon-zoom-out:before{content:"\e016"}.glyphicon-off:before{content:"\e017"}.glyphicon-signal:before{content:"\e018"}.glyphicon-cog:before{content:"\e019"}.glyphicon-trash:before{content:"\e020"}.glyphicon-home:before{content:"\e021"}.glyphicon-file:before{content:"\e022"}.glyphicon-time:before{content:"\e023"}.glyphicon-road:before{content:"\e024"}.glyphicon-download-alt:before{content:"\e025"}.glyphicon-download:before{content:"\e026"}.glyphicon-upload:before{content:"\e027"}.glyphicon-inbox:before{content:"\e028"}.glyphicon-play-circle:before{content:"\e029"}.glyphicon-repeat:before{content:"\e030"}.glyphicon-refresh:before{content:"\e031"}.glyphicon-list-alt:before{content:"\e032"}.glyphicon-lock:before{content:"\e033"}.glyphicon-flag:before{content:"\e034"}.glyphicon-headphones:before{content:"\e035"}.glyphicon-volume-off:before{content:"\e036"}.glyphicon-volume-down:before{content:"\e037"}.glyphicon-volume-up:before{content:"\e038"}.glyphicon-qrcode:before{content:"\e039"}.glyphicon-barcode:before{content:"\e040"}.glyphicon-tag:before{content:"\e041"}.glyphicon-tags:before{content:"\e042"}.glyphicon-book:before{content:"\e043"}.glyphicon-bookmark:before{content:"\e044"}.glyphicon-print:before{content:"\e045"}.glyphicon-camera:before{content:"\e046"}.glyphicon-font:before{content:"\e047"}.glyphicon-bold:before{content:"\e048"}.glyphicon-italic:before{content:"\e049"}.glyphicon-text-height:before{content:"\e050"}.glyphicon-text-width:before{content:"\e051"}.glyphicon-align-left:before{content:"\e052"}.glyphicon-align-center:before{content:"\e053"}.glyphicon-align-right:before{content:"\e054"}.glyphicon-align-justify:before{content:"\e055"}.glyphicon-list:before{content:"\e056"}.glyphicon-indent-left:before{content:"\e057"}.glyphicon-indent-right:before{content:"\e058"}.glyphicon-facetime-video:before{content:"\e059"}.glyphicon-picture:before{content:"\e060"}.glyphicon-map-marker:before{content:"\e062"}.glyphicon-adjust:before{content:"\e063"}.glyphicon-tint:before{content:"\e064"}.glyphicon-edit:before{content:"\e065"}.glyphicon-share:before{content:"\e066"}.glyphicon-check:before{content:"\e067"}.glyphicon-move:before{content:"\e068"}.glyphicon-step-backward:before{content:"\e069"}.glyphicon-fast-backward:before{content:"\e070"}.glyphicon-backward:before{content:"\e071"}.glyphicon-play:before{content:"\e072"}.glyphicon-pause:before{content:"\e073"}.glyphicon-stop:before{content:"\e074"}.glyphicon-forward:before{content:"\e075"}.glyphicon-fast-forward:before{content:"\e076"}.glyphicon-step-forward:before{content:"\e077"}.glyphicon-eject:before{content:"\e078"}.glyphicon-chevron-left:before{content:"\e079"}.glyphicon-chevron-right:before{content:"\e080"}.glyphicon-plus-sign:before{content:"\e081"}.glyphicon-minus-sign:before{content:"\e082"}.glyphicon-remove-sign:before{content:"\e083"}.glyphicon-ok-sign:before{content:"\e084"}.glyphicon-question-sign:before{content:"\e085"}.glyphicon-info-sign:before{content:"\e086"}.glyphicon-screenshot:before{content:"\e087"}.glyphicon-remove-circle:before{content:"\e088"}.glyphicon-ok-circle:before{content:"\e089"}.glyphicon-ban-circle:before{content:"\e090"}.glyphicon-arrow-left:before{content:"\e091"}.glyphicon-arrow-right:before{content:"\e092"}.glyphicon-arrow-up:before{content:"\e093"}.glyphicon-arrow-down:before{content:"\e094"}.glyphicon-share-alt:before{content:"\e095"}.glyphicon-resize-full:before{content:"\e096"}.glyphicon-resize-small:before{content:"\e097"}.glyphicon-exclamation-sign:before{content:"\e101"}.glyphicon-gift:before{content:"\e102"}.glyphicon-leaf:before{content:"\e103"}.glyphicon-fire:before{content:"\e104"}.glyphicon-eye-open:before{content:"\e105"}.glyphicon-eye-close:before{content:"\e106"}.glyphicon-warning-sign:before{content:"\e107"}.glyphicon-plane:before{content:"\e108"}.glyphicon-calendar:before{content:"\e109"}.glyphicon-random:before{content:"\e110"}.glyphicon-comment:before{content:"\e111"}.glyphicon-magnet:before{content:"\e112"}.glyphicon-chevron-up:before{content:"\e113"}.glyphicon-chevron-down:before{content:"\e114"}.glyphicon-retweet:before{content:"\e115"}.glyphicon-shopping-cart:before{content:"\e116"}.glyphicon-folder-close:before{content:"\e117"}.glyphicon-folder-open:before{content:"\e118"}.glyphicon-resize-vertical:before{content:"\e119"}.glyphicon-resize-horizontal:before{content:"\e120"}.glyphicon-hdd:before{content:"\e121"}.glyphicon-bullhorn:before{content:"\e122"}.glyphicon-bell:before{content:"\e123"}.glyphicon-certificate:before{content:"\e124"}.glyphicon-thumbs-up:before{content:"\e125"}.glyphicon-thumbs-down:before{content:"\e126"}.glyphicon-hand-right:before{content:"\e127"}.glyphicon-hand-left:before{content:"\e128"}.glyphicon-hand-up:before{content:"\e129"}.glyphicon-hand-down:before{content:"\e130"}.glyphicon-circle-arrow-right:before{content:"\e131"}.glyphicon-circle-arrow-left:before{content:"\e132"}.glyphicon-circle-arrow-up:before{content:"\e133"}.glyphicon-circle-arrow-down:before{content:"\e134"}.glyphicon-globe:before{content:"\e135"}.glyphicon-wrench:before{content:"\e136"}.glyphicon-tasks:before{content:"\e137"}.glyphicon-filter:before{content:"\e138"}.glyphicon-briefcase:before{content:"\e139"}.glyphicon-fullscreen:before{content:"\e140"}.glyphicon-dashboard:before{content:"\e141"}.glyphicon-paperclip:before{content:"\e142"}.glyphicon-heart-empty:before{content:"\e143"}.glyphicon-link:before{content:"\e144"}.glyphicon-phone:before{content:"\e145"}.glyphicon-pushpin:before{content:"\e146"}.glyphicon-usd:before{content:"\e148"}.glyphicon-gbp:before{content:"\e149"}.glyphicon-sort:before{content:"\e150"}.glyphicon-sort-by-alphabet:before{content:"\e151"}.glyphicon-sort-by-alphabet-alt:before{content:"\e152"}.glyphicon-sort-by-order:before{content:"\e153"}.glyphicon-sort-by-order-alt:before{content:"\e154"}.glyphicon-sort-by-attributes:before{content:"\e155"}.glyphicon-sort-by-attributes-alt:before{content:"\e156"}.glyphicon-unchecked:before{content:"\e157"}.glyphicon-expand:before{content:"\e158"}.glyphicon-collapse-down:before{content:"\e159"}.glyphicon-collapse-up:before{content:"\e160"}.glyphicon-log-in:before{content:"\e161"}.glyphicon-flash:before{content:"\e162"}.glyphicon-log-out:before{content:"\e163"}.glyphicon-new-window:before{content:"\e164"}.glyphicon-record:before{content:"\e165"}.glyphicon-save:before{content:"\e166"}.glyphicon-open:before{content:"\e167"}.glyphicon-saved:before{content:"\e168"}.glyphicon-import:before{content:"\e169"}.glyphicon-export:before{content:"\e170"}.glyphicon-send:before{content:"\e171"}.glyphicon-floppy-disk:before{content:"\e172"}.glyphicon-floppy-saved:before{content:"\e173"}.glyphicon-floppy-remove:before{content:"\e174"}.glyphicon-floppy-save:before{content:"\e175"}.glyphicon-floppy-open:before{content:"\e176"}.glyphicon-credit-card:before{content:"\e177"}.glyphicon-transfer:before{content:"\e178"}.glyphicon-cutlery:before{content:"\e179"}.glyphicon-header:before{content:"\e180"}.glyphicon-compressed:before{content:"\e181"}.glyphicon-earphone:before{content:"\e182"}.glyphicon-phone-alt:before{content:"\e183"}.glyphicon-tower:before{content:"\e184"}.glyphicon-stats:before{content:"\e185"}.glyphicon-sd-video:before{content:"\e186"}.glyphicon-hd-video:before{content:"\e187"}.glyphicon-subtitles:before{content:"\e188"}.glyphicon-sound-stereo:before{content:"\e189"}.glyphicon-sound-dolby:before{content:"\e190"}.glyphicon-sound-5-1:before{content:"\e191"}.glyphicon-sound-6-1:before{content:"\e192"}.glyphicon-sound-7-1:before{content:"\e193"}.glyphicon-copyright-mark:before{content:"\e194"}.glyphicon-registration-mark:before{content:"\e195"}.glyphicon-cloud-download:before{content:"\e197"}.glyphicon-cloud-upload:before{content:"\e198"}.glyphicon-tree-conifer:before{content:"\e199"}.glyphicon-tree-deciduous:before{content:"\e200"}.glyphicon-cd:before{content:"\e201"}.glyphicon-save-file:before{content:"\e202"}.glyphicon-open-file:before{content:"\e203"}.glyphicon-level-up:before{content:"\e204"}.glyphicon-copy:before{content:"\e205"}.glyphicon-paste:before{content:"\e206"}.glyphicon-alert:before{content:"\e209"}.glyphicon-equalizer:before{content:"\e210"}.glyphicon-king:before{content:"\e211"}.glyphicon-queen:before{content:"\e212"}.glyphicon-pawn:before{content:"\e213"}.glyphicon-bishop:before{content:"\e214"}.glyphicon-knight:before{content:"\e215"}.glyphicon-baby-formula:before{content:"\e216"}.glyphicon-tent:before{content:"\26fa"}.glyphicon-blackboard:before{content:"\e218"}.glyphicon-bed:before{content:"\e219"}.glyphicon-apple:before{content:"\f8ff"}.glyphicon-erase:before{content:"\e221"}.glyphicon-hourglass:before{content:"\231b"}.glyphicon-lamp:before{content:"\e223"}.glyphicon-duplicate:before{content:"\e224"}.glyphicon-piggy-bank:before{content:"\e225"}.glyphicon-scissors:before{content:"\e226"}.glyphicon-bitcoin:before{content:"\e227"}.glyphicon-btc:before{content:"\e227"}.glyphicon-xbt:before{content:"\e227"}.glyphicon-yen:before{content:"\00a5"}.glyphicon-jpy:before{content:"\00a5"}.glyphicon-ruble:before{content:"\20bd"}.glyphicon-rub:before{content:"\20bd"}.glyphicon-scale:before{content:"\e230"}.glyphicon-ice-lolly:before{content:"\e231"}.glyphicon-ice-lolly-tasted:before{content:"\e232"}.glyphicon-education:before{content:"\e233"}.glyphicon-option-horizontal:before{content:"\e234"}.glyphicon-option-vertical:before{content:"\e235"}.glyphicon-menu-hamburger:before{content:"\e236"}.glyphicon-modal-window:before{content:"\e237"}.glyphicon-oil:before{content:"\e238"}.glyphicon-grain:before{content:"\e239"}.glyphicon-sunglasses:before{content:"\e240"}.glyphicon-text-size:before{content:"\e241"}.glyphicon-text-color:before{content:"\e242"}.glyphicon-text-background:before{content:"\e243"}.glyphicon-object-align-top:before{content:"\e244"}.glyphicon-object-align-bottom:before{content:"\e245"}.glyphicon-object-align-horizontal:before{content:"\e246"}.glyphicon-object-align-left:before{content:"\e247"}.glyphicon-object-align-vertical:before{content:"\e248"}.glyphicon-object-align-right:before{content:"\e249"}.glyphicon-triangle-right:before{content:"\e250"}.glyphicon-triangle-left:before{content:"\e251"}.glyphicon-triangle-bottom:before{content:"\e252"}.glyphicon-triangle-top:before{content:"\e253"}.glyphicon-console:before{content:"\e254"}.glyphicon-superscript:before{content:"\e255"}.glyphicon-subscript:before{content:"\e256"}.glyphicon-menu-left:before{content:"\e257"}.glyphicon-menu-right:before{content:"\e258"}.glyphicon-menu-down:before{content:"\e259"}.glyphicon-menu-up:before{content:"\e260"}*{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}:after,:before{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html{font-size:10px;-webkit-tap-highlight-color:rgba(0,0,0,0)}body{font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:14px;line-height:1.42857143;color:#333;background-color:#fff}button,input,select,textarea{font-family:inherit;font-size:inherit;line-height:inherit}a{color:#337ab7;text-decoration:none}a:focus,a:hover{color:#23527c;text-decoration:underline}a:focus{outline:thin dotted;outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}figure{margin:0}img{vertical-align:middle}.carousel-inner>.item>a>img,.carousel-inner>.item>img,.img-responsive,.thumbnail a>img,.thumbnail>img{display:block;max-width:100%;height:auto}.img-rounded{border-radius:6px}.img-thumbnail{display:inline-block;max-width:100%;height:auto;padding:4px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:all .2s ease-in-out;-o-transition:all .2s ease-in-out;transition:all .2s ease-in-out}.img-circle{border-radius:50%}hr{margin-top:20px;margin-bottom:20px;border:0;border-top:1px solid #eee}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.sr-only-focusable:active,.sr-only-focusable:focus{position:static;width:auto;height:auto;margin:0;overflow:visible;clip:auto}[role=button]{cursor:pointer}.h1,.h2,.h3,.h4,.h5,.h6,h1,h2,h3,h4,h5,h6{font-family:inherit;font-weight:500;line-height:1.1;color:inherit}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-weight:400;line-height:1;color:#777}.h1,.h2,.h3,h1,h2,h3{margin-top:20px;margin-bottom:10px}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small{font-size:65%}.h4,.h5,.h6,h4,h5,h6{margin-top:10px;margin-bottom:10px}.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-size:75%}.h1,h1{font-size:36px}.h2,h2{font-size:30px}.h3,h3{font-size:24px}.h4,h4{font-size:18px}.h5,h5{font-size:14px}.h6,h6{font-size:12px}p{margin:0 0 10px}.lead{margin-bottom:20px;font-size:16px;font-weight:300;line-height:1.4}@media (min-width:768px){.lead{font-size:21px}}.small,small{font-size:85%}.mark,mark{padding:.2em;background-color:#fcf8e3}.text-left{text-align:left}.text-right{text-align:right}.text-center{text-align:center}.text-justify{text-align:justify}.text-nowrap{white-space:nowrap}.text-lowercase{text-transform:lowercase}.text-uppercase{text-transform:uppercase}.text-capitalize{text-transform:capitalize}.text-muted{color:#777}.text-primary{color:#337ab7}a.text-primary:focus,a.text-primary:hover{color:#286090}.text-success{color:#3c763d}a.text-success:focus,a.text-success:hover{color:#2b542c}.text-info{color:#31708f}a.text-info:focus,a.text-info:hover{color:#245269}.text-warning{color:#8a6d3b}a.text-warning:focus,a.text-warning:hover{color:#66512c}.text-danger{color:#a94442}a.text-danger:focus,a.text-danger:hover{color:#843534}.bg-primary{color:#fff;background-color:#337ab7}a.bg-primary:focus,a.bg-primary:hover{background-color:#286090}.bg-success{background-color:#dff0d8}a.bg-success:focus,a.bg-success:hover{background-color:#c1e2b3}.bg-info{background-color:#d9edf7}a.bg-info:focus,a.bg-info:hover{background-color:#afd9ee}.bg-warning{background-color:#fcf8e3}a.bg-warning:focus,a.bg-warning:hover{background-color:#f7ecb5}.bg-danger{background-color:#f2dede}a.bg-danger:focus,a.bg-danger:hover{background-color:#e4b9b9}.page-header{padding-bottom:9px;margin:40px 0 20px;border-bottom:1px solid #eee}ol,ul{margin-top:0;margin-bottom:10px}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}.list-unstyled{padding-left:0;list-style:none}.list-inline{padding-left:0;margin-left:-5px;list-style:none}.list-inline>li{display:inline-block;padding-right:5px;padding-left:5px}dl{margin-top:0;margin-bottom:20px}dd,dt{line-height:1.42857143}dt{font-weight:700}dd{margin-left:0}@media (min-width:768px){.dl-horizontal dt{float:left;width:160px;overflow:hidden;clear:left;text-align:right;text-overflow:ellipsis;white-space:nowrap}.dl-horizontal dd{margin-left:180px}}abbr[data-original-title],abbr[title]{cursor:help;border-bottom:1px dotted #777}.initialism{font-size:90%;text-transform:uppercase}blockquote{padding:10px 20px;margin:0 0 20px;font-size:17.5px;border-left:5px solid #eee}blockquote ol:last-child,blockquote p:last-child,blockquote ul:last-child{margin-bottom:0}blockquote .small,blockquote footer,blockquote small{display:block;font-size:80%;line-height:1.42857143;color:#777}blockquote .small:before,blockquote footer:before,blockquote small:before{content:'\2014 \00A0'}.blockquote-reverse,blockquote.pull-right{padding-right:15px;padding-left:0;text-align:right;border-right:5px solid #eee;border-left:0}.blockquote-reverse .small:before,.blockquote-reverse footer:before,.blockquote-reverse small:before,blockquote.pull-right .small:before,blockquote.pull-right footer:before,blockquote.pull-right small:before{content:''}.blockquote-reverse .small:after,.blockquote-reverse footer:after,.blockquote-reverse small:after,blockquote.pull-right .small:after,blockquote.pull-right footer:after,blockquote.pull-right small:after{content:'\00A0 \2014'}address{margin-bottom:20px;font-style:normal;line-height:1.42857143}code,kbd,pre,samp{font-family:Menlo,Monaco,Consolas,"Courier New",monospace}code{padding:2px 4px;font-size:90%;color:#c7254e;background-color:#f9f2f4;border-radius:4px}kbd{padding:2px 4px;font-size:90%;color:#fff;background-color:#333;border-radius:3px;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.25);box-shadow:inset 0 -1px 0 rgba(0,0,0,.25)}kbd kbd{padding:0;font-size:100%;font-weight:700;-webkit-box-shadow:none;box-shadow:none}pre{display:block;padding:9.5px;margin:0 0 10px;font-size:13px;line-height:1.42857143;color:#333;word-break:break-all;word-wrap:break-word;background-color:#f5f5f5;border:1px solid #ccc;border-radius:4px}pre code{padding:0;font-size:inherit;color:inherit;white-space:pre-wrap;background-color:transparent;border-radius:0}.pre-scrollable{max-height:340px;overflow-y:scroll}.container{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}@media (min-width:768px){.container{width:750px}}@media (min-width:992px){.container{width:970px}}@media (min-width:1200px){.container{width:1170px}}.container-fluid{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}.row{margin-right:-15px;margin-left:-15px}.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9,.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9,.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9,.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{position:relative;min-height:1px;padding-right:15px;padding-left:15px}.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{float:left}.col-xs-12{width:100%}.col-xs-11{width:91.66666667%}.col-xs-10{width:83.33333333%}.col-xs-9{width:75%}.col-xs-8{width:66.66666667%}.col-xs-7{width:58.33333333%}.col-xs-6{width:50%}.col-xs-5{width:41.66666667%}.col-xs-4{width:33.33333333%}.col-xs-3{width:25%}.col-xs-2{width:16.66666667%}.col-xs-1{width:8.33333333%}.col-xs-pull-12{right:100%}.col-xs-pull-11{right:91.66666667%}.col-xs-pull-10{right:83.33333333%}.col-xs-pull-9{right:75%}.col-xs-pull-8{right:66.66666667%}.col-xs-pull-7{right:58.33333333%}.col-xs-pull-6{right:50%}.col-xs-pull-5{right:41.66666667%}.col-xs-pull-4{right:33.33333333%}.col-xs-pull-3{right:25%}.col-xs-pull-2{right:16.66666667%}.col-xs-pull-1{right:8.33333333%}.col-xs-pull-0{right:auto}.col-xs-push-12{left:100%}.col-xs-push-11{left:91.66666667%}.col-xs-push-10{left:83.33333333%}.col-xs-push-9{left:75%}.col-xs-push-8{left:66.66666667%}.col-xs-push-7{left:58.33333333%}.col-xs-push-6{left:50%}.col-xs-push-5{left:41.66666667%}.col-xs-push-4{left:33.33333333%}.col-xs-push-3{left:25%}.col-xs-push-2{left:16.66666667%}.col-xs-push-1{left:8.33333333%}.col-xs-push-0{left:auto}.col-xs-offset-12{margin-left:100%}.col-xs-offset-11{margin-left:91.66666667%}.col-xs-offset-10{margin-left:83.33333333%}.col-xs-offset-9{margin-left:75%}.col-xs-offset-8{margin-left:66.66666667%}.col-xs-offset-7{margin-left:58.33333333%}.col-xs-offset-6{margin-left:50%}.col-xs-offset-5{margin-left:41.66666667%}.col-xs-offset-4{margin-left:33.33333333%}.col-xs-offset-3{margin-left:25%}.col-xs-offset-2{margin-left:16.66666667%}.col-xs-offset-1{margin-left:8.33333333%}.col-xs-offset-0{margin-left:0}@media (min-width:768px){.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9{float:left}.col-sm-12{width:100%}.col-sm-11{width:91.66666667%}.col-sm-10{width:83.33333333%}.col-sm-9{width:75%}.col-sm-8{width:66.66666667%}.col-sm-7{width:58.33333333%}.col-sm-6{width:50%}.col-sm-5{width:41.66666667%}.col-sm-4{width:33.33333333%}.col-sm-3{width:25%}.col-sm-2{width:16.66666667%}.col-sm-1{width:8.33333333%}.col-sm-pull-12{right:100%}.col-sm-pull-11{right:91.66666667%}.col-sm-pull-10{right:83.33333333%}.col-sm-pull-9{right:75%}.col-sm-pull-8{right:66.66666667%}.col-sm-pull-7{right:58.33333333%}.col-sm-pull-6{right:50%}.col-sm-pull-5{right:41.66666667%}.col-sm-pull-4{right:33.33333333%}.col-sm-pull-3{right:25%}.col-sm-pull-2{right:16.66666667%}.col-sm-pull-1{right:8.33333333%}.col-sm-pull-0{right:auto}.col-sm-push-12{left:100%}.col-sm-push-11{left:91.66666667%}.col-sm-push-10{left:83.33333333%}.col-sm-push-9{left:75%}.col-sm-push-8{left:66.66666667%}.col-sm-push-7{left:58.33333333%}.col-sm-push-6{left:50%}.col-sm-push-5{left:41.66666667%}.col-sm-push-4{left:33.33333333%}.col-sm-push-3{left:25%}.col-sm-push-2{left:16.66666667%}.col-sm-push-1{left:8.33333333%}.col-sm-push-0{left:auto}.col-sm-offset-12{margin-left:100%}.col-sm-offset-11{margin-left:91.66666667%}.col-sm-offset-10{margin-left:83.33333333%}.col-sm-offset-9{margin-left:75%}.col-sm-offset-8{margin-left:66.66666667%}.col-sm-offset-7{margin-left:58.33333333%}.col-sm-offset-6{margin-left:50%}.col-sm-offset-5{margin-left:41.66666667%}.col-sm-offset-4{margin-left:33.33333333%}.col-sm-offset-3{margin-left:25%}.col-sm-offset-2{margin-left:16.66666667%}.col-sm-offset-1{margin-left:8.33333333%}.col-sm-offset-0{margin-left:0}}@media (min-width:992px){.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9{float:left}.col-md-12{width:100%}.col-md-11{width:91.66666667%}.col-md-10{width:83.33333333%}.col-md-9{width:75%}.col-md-8{width:66.66666667%}.col-md-7{width:58.33333333%}.col-md-6{width:50%}.col-md-5{width:41.66666667%}.col-md-4{width:33.33333333%}.col-md-3{width:25%}.col-md-2{width:16.66666667%}.col-md-1{width:8.33333333%}.col-md-pull-12{right:100%}.col-md-pull-11{right:91.66666667%}.col-md-pull-10{right:83.33333333%}.col-md-pull-9{right:75%}.col-md-pull-8{right:66.66666667%}.col-md-pull-7{right:58.33333333%}.col-md-pull-6{right:50%}.col-md-pull-5{right:41.66666667%}.col-md-pull-4{right:33.33333333%}.col-md-pull-3{right:25%}.col-md-pull-2{right:16.66666667%}.col-md-pull-1{right:8.33333333%}.col-md-pull-0{right:auto}.col-md-push-12{left:100%}.col-md-push-11{left:91.66666667%}.col-md-push-10{left:83.33333333%}.col-md-push-9{left:75%}.col-md-push-8{left:66.66666667%}.col-md-push-7{left:58.33333333%}.col-md-push-6{left:50%}.col-md-push-5{left:41.66666667%}.col-md-push-4{left:33.33333333%}.col-md-push-3{left:25%}.col-md-push-2{left:16.66666667%}.col-md-push-1{left:8.33333333%}.col-md-push-0{left:auto}.col-md-offset-12{margin-left:100%}.col-md-offset-11{margin-left:91.66666667%}.col-md-offset-10{margin-left:83.33333333%}.col-md-offset-9{margin-left:75%}.col-md-offset-8{margin-left:66.66666667%}.col-md-offset-7{margin-left:58.33333333%}.col-md-offset-6{margin-left:50%}.col-md-offset-5{margin-left:41.66666667%}.col-md-offset-4{margin-left:33.33333333%}.col-md-offset-3{margin-left:25%}.col-md-offset-2{margin-left:16.66666667%}.col-md-offset-1{margin-left:8.33333333%}.col-md-offset-0{margin-left:0}}@media (min-width:1200px){.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9{float:left}.col-lg-12{width:100%}.col-lg-11{width:91.66666667%}.col-lg-10{width:83.33333333%}.col-lg-9{width:75%}.col-lg-8{width:66.66666667%}.col-lg-7{width:58.33333333%}.col-lg-6{width:50%}.col-lg-5{width:41.66666667%}.col-lg-4{width:33.33333333%}.col-lg-3{width:25%}.col-lg-2{width:16.66666667%}.col-lg-1{width:8.33333333%}.col-lg-pull-12{right:100%}.col-lg-pull-11{right:91.66666667%}.col-lg-pull-10{right:83.33333333%}.col-lg-pull-9{right:75%}.col-lg-pull-8{right:66.66666667%}.col-lg-pull-7{right:58.33333333%}.col-lg-pull-6{right:50%}.col-lg-pull-5{right:41.66666667%}.col-lg-pull-4{right:33.33333333%}.col-lg-pull-3{right:25%}.col-lg-pull-2{right:16.66666667%}.col-lg-pull-1{right:8.33333333%}.col-lg-pull-0{right:auto}.col-lg-push-12{left:100%}.col-lg-push-11{left:91.66666667%}.col-lg-push-10{left:83.33333333%}.col-lg-push-9{left:75%}.col-lg-push-8{left:66.66666667%}.col-lg-push-7{left:58.33333333%}.col-lg-push-6{left:50%}.col-lg-push-5{left:41.66666667%}.col-lg-push-4{left:33.33333333%}.col-lg-push-3{left:25%}.col-lg-push-2{left:16.66666667%}.col-lg-push-1{left:8.33333333%}.col-lg-push-0{left:auto}.col-lg-offset-12{margin-left:100%}.col-lg-offset-11{margin-left:91.66666667%}.col-lg-offset-10{margin-left:83.33333333%}.col-lg-offset-9{margin-left:75%}.col-lg-offset-8{margin-left:66.66666667%}.col-lg-offset-7{margin-left:58.33333333%}.col-lg-offset-6{margin-left:50%}.col-lg-offset-5{margin-left:41.66666667%}.col-lg-offset-4{margin-left:33.33333333%}.col-lg-offset-3{margin-left:25%}.col-lg-offset-2{margin-left:16.66666667%}.col-lg-offset-1{margin-left:8.33333333%}.col-lg-offset-0{margin-left:0}}table{background-color:transparent}caption{padding-top:8px;padding-bottom:8px;color:#777;text-align:left}th{text-align:left}.table{width:100%;max-width:100%;margin-bottom:20px}.table>tbody>tr>td,.table>tbody>tr>th,.table>tfoot>tr>td,.table>tfoot>tr>th,.table>thead>tr>td,.table>thead>tr>th{padding:8px;line-height:1.42857143;vertical-align:top;border-top:1px solid #ddd}.table>thead>tr>th{vertical-align:bottom;border-bottom:2px solid #ddd}.table>caption+thead>tr:first-child>td,.table>caption+thead>tr:first-child>th,.table>colgroup+thead>tr:first-child>td,.table>colgroup+thead>tr:first-child>th,.table>thead:first-child>tr:first-child>td,.table>thead:first-child>tr:first-child>th{border-top:0}.table>tbody+tbody{border-top:2px solid #ddd}.table .table{background-color:#fff}.table-condensed>tbody>tr>td,.table-condensed>tbody>tr>th,.table-condensed>tfoot>tr>td,.table-condensed>tfoot>tr>th,.table-condensed>thead>tr>td,.table-condensed>thead>tr>th{padding:5px}.table-bordered{border:1px solid #ddd}.table-bordered>tbody>tr>td,.table-bordered>tbody>tr>th,.table-bordered>tfoot>tr>td,.table-bordered>tfoot>tr>th,.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border:1px solid #ddd}.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border-bottom-width:2px}.table-striped>tbody>tr:nth-of-type(odd){background-color:#f9f9f9}.table-hover>tbody>tr:hover{background-color:#f5f5f5}table col[class*=col-]{position:static;display:table-column;float:none}table td[class*=col-],table th[class*=col-]{position:static;display:table-cell;float:none}.table>tbody>tr.active>td,.table>tbody>tr.active>th,.table>tbody>tr>td.active,.table>tbody>tr>th.active,.table>tfoot>tr.active>td,.table>tfoot>tr.active>th,.table>tfoot>tr>td.active,.table>tfoot>tr>th.active,.table>thead>tr.active>td,.table>thead>tr.active>th,.table>thead>tr>td.active,.table>thead>tr>th.active{background-color:#f5f5f5}.table-hover>tbody>tr.active:hover>td,.table-hover>tbody>tr.active:hover>th,.table-hover>tbody>tr:hover>.active,.table-hover>tbody>tr>td.active:hover,.table-hover>tbody>tr>th.active:hover{background-color:#e8e8e8}.table>tbody>tr.success>td,.table>tbody>tr.success>th,.table>tbody>tr>td.success,.table>tbody>tr>th.success,.table>tfoot>tr.success>td,.table>tfoot>tr.success>th,.table>tfoot>tr>td.success,.table>tfoot>tr>th.success,.table>thead>tr.success>td,.table>thead>tr.success>th,.table>thead>tr>td.success,.table>thead>tr>th.success{background-color:#dff0d8}.table-hover>tbody>tr.success:hover>td,.table-hover>tbody>tr.success:hover>th,.table-hover>tbody>tr:hover>.success,.table-hover>tbody>tr>td.success:hover,.table-hover>tbody>tr>th.success:hover{background-color:#d0e9c6}.table>tbody>tr.info>td,.table>tbody>tr.info>th,.table>tbody>tr>td.info,.table>tbody>tr>th.info,.table>tfoot>tr.info>td,.table>tfoot>tr.info>th,.table>tfoot>tr>td.info,.table>tfoot>tr>th.info,.table>thead>tr.info>td,.table>thead>tr.info>th,.table>thead>tr>td.info,.table>thead>tr>th.info{background-color:#d9edf7}.table-hover>tbody>tr.info:hover>td,.table-hover>tbody>tr.info:hover>th,.table-hover>tbody>tr:hover>.info,.table-hover>tbody>tr>td.info:hover,.table-hover>tbody>tr>th.info:hover{background-color:#c4e3f3}.table>tbody>tr.warning>td,.table>tbody>tr.warning>th,.table>tbody>tr>td.warning,.table>tbody>tr>th.warning,.table>tfoot>tr.warning>td,.table>tfoot>tr.warning>th,.table>tfoot>tr>td.warning,.table>tfoot>tr>th.warning,.table>thead>tr.warning>td,.table>thead>tr.warning>th,.table>thead>tr>td.warning,.table>thead>tr>th.warning{background-color:#fcf8e3}.table-hover>tbody>tr.warning:hover>td,.table-hover>tbody>tr.warning:hover>th,.table-hover>tbody>tr:hover>.warning,.table-hover>tbody>tr>td.warning:hover,.table-hover>tbody>tr>th.warning:hover{background-color:#faf2cc}.table>tbody>tr.danger>td,.table>tbody>tr.danger>th,.table>tbody>tr>td.danger,.table>tbody>tr>th.danger,.table>tfoot>tr.danger>td,.table>tfoot>tr.danger>th,.table>tfoot>tr>td.danger,.table>tfoot>tr>th.danger,.table>thead>tr.danger>td,.table>thead>tr.danger>th,.table>thead>tr>td.danger,.table>thead>tr>th.danger{background-color:#f2dede}.table-hover>tbody>tr.danger:hover>td,.table-hover>tbody>tr.danger:hover>th,.table-hover>tbody>tr:hover>.danger,.table-hover>tbody>tr>td.danger:hover,.table-hover>tbody>tr>th.danger:hover{background-color:#ebcccc}.table-responsive{min-height:.01%;overflow-x:auto}@media screen and (max-width:767px){.table-responsive{width:100%;margin-bottom:15px;overflow-y:hidden;-ms-overflow-style:-ms-autohiding-scrollbar;border:1px solid #ddd}.table-responsive>.table{margin-bottom:0}.table-responsive>.table>tbody>tr>td,.table-responsive>.table>tbody>tr>th,.table-responsive>.table>tfoot>tr>td,.table-responsive>.table>tfoot>tr>th,.table-responsive>.table>thead>tr>td,.table-responsive>.table>thead>tr>th{white-space:nowrap}.table-responsive>.table-bordered{border:0}.table-responsive>.table-bordered>tbody>tr>td:first-child,.table-responsive>.table-bordered>tbody>tr>th:first-child,.table-responsive>.table-bordered>tfoot>tr>td:first-child,.table-responsive>.table-bordered>tfoot>tr>th:first-child,.table-responsive>.table-bordered>thead>tr>td:first-child,.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.table-responsive>.table-bordered>tbody>tr>td:last-child,.table-responsive>.table-bordered>tbody>tr>th:last-child,.table-responsive>.table-bordered>tfoot>tr>td:last-child,.table-responsive>.table-bordered>tfoot>tr>th:last-child,.table-responsive>.table-bordered>thead>tr>td:last-child,.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.table-responsive>.table-bordered>tbody>tr:last-child>td,.table-responsive>.table-bordered>tbody>tr:last-child>th,.table-responsive>.table-bordered>tfoot>tr:last-child>td,.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}}fieldset{min-width:0;padding:0;margin:0;border:0}legend{display:block;width:100%;padding:0;margin-bottom:20px;font-size:21px;line-height:inherit;color:#333;border:0;border-bottom:1px solid #e5e5e5}label{display:inline-block;max-width:100%;margin-bottom:5px;font-weight:700}input[type=search]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}input[type=checkbox],input[type=radio]{margin:4px 0 0;margin-top:1px\9;line-height:normal}input[type=file]{display:block}input[type=range]{display:block;width:100%}select[multiple],select[size]{height:auto}input[type=file]:focus,input[type=checkbox]:focus,input[type=radio]:focus{outline:thin dotted;outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}output{display:block;padding-top:7px;font-size:14px;line-height:1.42857143;color:#555}.form-control{display:block;width:100%;height:34px;padding:6px 12px;font-size:14px;line-height:1.42857143;color:#555;background-color:#fff;background-image:none;border:1px solid #ccc;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075);-webkit-transition:border-color ease-in-out .15s,-webkit-box-shadow ease-in-out .15s;-o-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s}.form-control:focus{border-color:#66afe9;outline:0;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6);box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6)}.form-control::-moz-placeholder{color:#999;opacity:1}.form-control:-ms-input-placeholder{color:#999}.form-control::-webkit-input-placeholder{color:#999}.form-control::-ms-expand{background-color:transparent;border:0}.form-control[disabled],.form-control[readonly],fieldset[disabled] .form-control{background-color:#eee;opacity:1}.form-control[disabled],fieldset[disabled] .form-control{cursor:not-allowed}textarea.form-control{height:auto}input[type=search]{-webkit-appearance:none}@media screen and (-webkit-min-device-pixel-ratio:0){input[type=date].form-control,input[type=time].form-control,input[type=datetime-local].form-control,input[type=month].form-control{line-height:34px}.input-group-sm input[type=date],.input-group-sm input[type=time],.input-group-sm input[type=datetime-local],.input-group-sm input[type=month],input[type=date].input-sm,input[type=time].input-sm,input[type=datetime-local].input-sm,input[type=month].input-sm{line-height:30px}.input-group-lg input[type=date],.input-group-lg input[type=time],.input-group-lg input[type=datetime-local],.input-group-lg input[type=month],input[type=date].input-lg,input[type=time].input-lg,input[type=datetime-local].input-lg,input[type=month].input-lg{line-height:46px}}.form-group{margin-bottom:15px}.checkbox,.radio{position:relative;display:block;margin-top:10px;margin-bottom:10px}.checkbox label,.radio label{min-height:20px;padding-left:20px;margin-bottom:0;font-weight:400;cursor:pointer}.checkbox input[type=checkbox],.checkbox-inline input[type=checkbox],.radio input[type=radio],.radio-inline input[type=radio]{position:absolute;margin-top:4px\9;margin-left:-20px}.checkbox+.checkbox,.radio+.radio{margin-top:-5px}.checkbox-inline,.radio-inline{position:relative;display:inline-block;padding-left:20px;margin-bottom:0;font-weight:400;vertical-align:middle;cursor:pointer}.checkbox-inline+.checkbox-inline,.radio-inline+.radio-inline{margin-top:0;margin-left:10px}fieldset[disabled] input[type=checkbox],fieldset[disabled] input[type=radio],input[type=checkbox].disabled,input[type=checkbox][disabled],input[type=radio].disabled,input[type=radio][disabled]{cursor:not-allowed}.checkbox-inline.disabled,.radio-inline.disabled,fieldset[disabled] .checkbox-inline,fieldset[disabled] .radio-inline{cursor:not-allowed}.checkbox.disabled label,.radio.disabled label,fieldset[disabled] .checkbox label,fieldset[disabled] .radio label{cursor:not-allowed}.form-control-static{min-height:34px;padding-top:7px;padding-bottom:7px;margin-bottom:0}.form-control-static.input-lg,.form-control-static.input-sm{padding-right:0;padding-left:0}.input-sm{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-sm{height:30px;line-height:30px}select[multiple].input-sm,textarea.input-sm{height:auto}.form-group-sm .form-control{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.form-group-sm select.form-control{height:30px;line-height:30px}.form-group-sm select[multiple].form-control,.form-group-sm textarea.form-control{height:auto}.form-group-sm .form-control-static{height:30px;min-height:32px;padding:6px 10px;font-size:12px;line-height:1.5}.input-lg{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-lg{height:46px;line-height:46px}select[multiple].input-lg,textarea.input-lg{height:auto}.form-group-lg .form-control{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.form-group-lg select.form-control{height:46px;line-height:46px}.form-group-lg select[multiple].form-control,.form-group-lg textarea.form-control{height:auto}.form-group-lg .form-control-static{height:46px;min-height:38px;padding:11px 16px;font-size:18px;line-height:1.3333333}.has-feedback{position:relative}.has-feedback .form-control{padding-right:42.5px}.form-control-feedback{position:absolute;top:0;right:0;z-index:2;display:block;width:34px;height:34px;line-height:34px;text-align:center;pointer-events:none}.form-group-lg .form-control+.form-control-feedback,.input-group-lg+.form-control-feedback,.input-lg+.form-control-feedback{width:46px;height:46px;line-height:46px}.form-group-sm .form-control+.form-control-feedback,.input-group-sm+.form-control-feedback,.input-sm+.form-control-feedback{width:30px;height:30px;line-height:30px}.has-success .checkbox,.has-success .checkbox-inline,.has-success .control-label,.has-success .help-block,.has-success .radio,.has-success .radio-inline,.has-success.checkbox label,.has-success.checkbox-inline label,.has-success.radio label,.has-success.radio-inline label{color:#3c763d}.has-success .form-control{border-color:#3c763d;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-success .form-control:focus{border-color:#2b542c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168}.has-success .input-group-addon{color:#3c763d;background-color:#dff0d8;border-color:#3c763d}.has-success .form-control-feedback{color:#3c763d}.has-warning .checkbox,.has-warning .checkbox-inline,.has-warning .control-label,.has-warning .help-block,.has-warning .radio,.has-warning .radio-inline,.has-warning.checkbox label,.has-warning.checkbox-inline label,.has-warning.radio label,.has-warning.radio-inline label{color:#8a6d3b}.has-warning .form-control{border-color:#8a6d3b;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-warning .form-control:focus{border-color:#66512c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b}.has-warning .input-group-addon{color:#8a6d3b;background-color:#fcf8e3;border-color:#8a6d3b}.has-warning .form-control-feedback{color:#8a6d3b}.has-error .checkbox,.has-error .checkbox-inline,.has-error .control-label,.has-error .help-block,.has-error .radio,.has-error .radio-inline,.has-error.checkbox label,.has-error.checkbox-inline label,.has-error.radio label,.has-error.radio-inline label{color:#a94442}.has-error .form-control{border-color:#a94442;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-error .form-control:focus{border-color:#843534;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483}.has-error .input-group-addon{color:#a94442;background-color:#f2dede;border-color:#a94442}.has-error .form-control-feedback{color:#a94442}.has-feedback label~.form-control-feedback{top:25px}.has-feedback label.sr-only~.form-control-feedback{top:0}.help-block{display:block;margin-top:5px;margin-bottom:10px;color:#737373}@media (min-width:768px){.form-inline .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.form-inline .form-control{display:inline-block;width:auto;vertical-align:middle}.form-inline .form-control-static{display:inline-block}.form-inline .input-group{display:inline-table;vertical-align:middle}.form-inline .input-group .form-control,.form-inline .input-group .input-group-addon,.form-inline .input-group .input-group-btn{width:auto}.form-inline .input-group>.form-control{width:100%}.form-inline .control-label{margin-bottom:0;vertical-align:middle}.form-inline .checkbox,.form-inline .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.form-inline .checkbox label,.form-inline .radio label{padding-left:0}.form-inline .checkbox input[type=checkbox],.form-inline .radio input[type=radio]{position:relative;margin-left:0}.form-inline .has-feedback .form-control-feedback{top:0}}.form-horizontal .checkbox,.form-horizontal .checkbox-inline,.form-horizontal .radio,.form-horizontal .radio-inline{padding-top:7px;margin-top:0;margin-bottom:0}.form-horizontal .checkbox,.form-horizontal .radio{min-height:27px}.form-horizontal .form-group{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.form-horizontal .control-label{padding-top:7px;margin-bottom:0;text-align:right}}.form-horizontal .has-feedback .form-control-feedback{right:15px}@media (min-width:768px){.form-horizontal .form-group-lg .control-label{padding-top:11px;font-size:18px}}@media (min-width:768px){.form-horizontal .form-group-sm .control-label{padding-top:6px;font-size:12px}}.btn{display:inline-block;padding:6px 12px;margin-bottom:0;font-size:14px;font-weight:400;line-height:1.42857143;text-align:center;white-space:nowrap;vertical-align:middle;-ms-touch-action:manipulation;touch-action:manipulation;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;background-image:none;border:1px solid transparent;border-radius:4px}.btn.active.focus,.btn.active:focus,.btn.focus,.btn:active.focus,.btn:active:focus,.btn:focus{outline:thin dotted;outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}.btn.focus,.btn:focus,.btn:hover{color:#333;text-decoration:none}.btn.active,.btn:active{background-image:none;outline:0;-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn.disabled,.btn[disabled],fieldset[disabled] .btn{cursor:not-allowed;filter:alpha(opacity=65);-webkit-box-shadow:none;box-shadow:none;opacity:.65}a.btn.disabled,fieldset[disabled] a.btn{pointer-events:none}.btn-default{color:#333;background-color:#fff;border-color:#ccc}.btn-default.focus,.btn-default:focus{color:#333;background-color:#e6e6e6;border-color:#8c8c8c}.btn-default:hover{color:#333;background-color:#e6e6e6;border-color:#adadad}.btn-default.active,.btn-default:active,.open>.dropdown-toggle.btn-default{color:#333;background-color:#e6e6e6;border-color:#adadad}.btn-default.active.focus,.btn-default.active:focus,.btn-default.active:hover,.btn-default:active.focus,.btn-default:active:focus,.btn-default:active:hover,.open>.dropdown-toggle.btn-default.focus,.open>.dropdown-toggle.btn-default:focus,.open>.dropdown-toggle.btn-default:hover{color:#333;background-color:#d4d4d4;border-color:#8c8c8c}.btn-default.active,.btn-default:active,.open>.dropdown-toggle.btn-default{background-image:none}.btn-default.disabled.focus,.btn-default.disabled:focus,.btn-default.disabled:hover,.btn-default[disabled].focus,.btn-default[disabled]:focus,.btn-default[disabled]:hover,fieldset[disabled] .btn-default.focus,fieldset[disabled] .btn-default:focus,fieldset[disabled] .btn-default:hover{background-color:#fff;border-color:#ccc}.btn-default .badge{color:#fff;background-color:#333}.btn-primary{color:#fff;background-color:#337ab7;border-color:#2e6da4}.btn-primary.focus,.btn-primary:focus{color:#fff;background-color:#286090;border-color:#122b40}.btn-primary:hover{color:#fff;background-color:#286090;border-color:#204d74}.btn-primary.active,.btn-primary:active,.open>.dropdown-toggle.btn-primary{color:#fff;background-color:#286090;border-color:#204d74}.btn-primary.active.focus,.btn-primary.active:focus,.btn-primary.active:hover,.btn-primary:active.focus,.btn-primary:active:focus,.btn-primary:active:hover,.open>.dropdown-toggle.btn-primary.focus,.open>.dropdown-toggle.btn-primary:focus,.open>.dropdown-toggle.btn-primary:hover{color:#fff;background-color:#204d74;border-color:#122b40}.btn-primary.active,.btn-primary:active,.open>.dropdown-toggle.btn-primary{background-image:none}.btn-primary.disabled.focus,.btn-primary.disabled:focus,.btn-primary.disabled:hover,.btn-primary[disabled].focus,.btn-primary[disabled]:focus,.btn-primary[disabled]:hover,fieldset[disabled] .btn-primary.focus,fieldset[disabled] .btn-primary:focus,fieldset[disabled] .btn-primary:hover{background-color:#337ab7;border-color:#2e6da4}.btn-primary .badge{color:#337ab7;background-color:#fff}.btn-success{color:#fff;background-color:#5cb85c;border-color:#4cae4c}.btn-success.focus,.btn-success:focus{color:#fff;background-color:#449d44;border-color:#255625}.btn-success:hover{color:#fff;background-color:#449d44;border-color:#398439}.btn-success.active,.btn-success:active,.open>.dropdown-toggle.btn-success{color:#fff;background-color:#449d44;border-color:#398439}.btn-success.active.focus,.btn-success.active:focus,.btn-success.active:hover,.btn-success:active.focus,.btn-success:active:focus,.btn-success:active:hover,.open>.dropdown-toggle.btn-success.focus,.open>.dropdown-toggle.btn-success:focus,.open>.dropdown-toggle.btn-success:hover{color:#fff;background-color:#398439;border-color:#255625}.btn-success.active,.btn-success:active,.open>.dropdown-toggle.btn-success{background-image:none}.btn-success.disabled.focus,.btn-success.disabled:focus,.btn-success.disabled:hover,.btn-success[disabled].focus,.btn-success[disabled]:focus,.btn-success[disabled]:hover,fieldset[disabled] .btn-success.focus,fieldset[disabled] .btn-success:focus,fieldset[disabled] .btn-success:hover{background-color:#5cb85c;border-color:#4cae4c}.btn-success .badge{color:#5cb85c;background-color:#fff}.btn-info{color:#fff;background-color:#5bc0de;border-color:#46b8da}.btn-info.focus,.btn-info:focus{color:#fff;background-color:#31b0d5;border-color:#1b6d85}.btn-info:hover{color:#fff;background-color:#31b0d5;border-color:#269abc}.btn-info.active,.btn-info:active,.open>.dropdown-toggle.btn-info{color:#fff;background-color:#31b0d5;border-color:#269abc}.btn-info.active.focus,.btn-info.active:focus,.btn-info.active:hover,.btn-info:active.focus,.btn-info:active:focus,.btn-info:active:hover,.open>.dropdown-toggle.btn-info.focus,.open>.dropdown-toggle.btn-info:focus,.open>.dropdown-toggle.btn-info:hover{color:#fff;background-color:#269abc;border-color:#1b6d85}.btn-info.active,.btn-info:active,.open>.dropdown-toggle.btn-info{background-image:none}.btn-info.disabled.focus,.btn-info.disabled:focus,.btn-info.disabled:hover,.btn-info[disabled].focus,.btn-info[disabled]:focus,.btn-info[disabled]:hover,fieldset[disabled] .btn-info.focus,fieldset[disabled] .btn-info:focus,fieldset[disabled] .btn-info:hover{background-color:#5bc0de;border-color:#46b8da}.btn-info .badge{color:#5bc0de;background-color:#fff}.btn-warning{color:#fff;background-color:#f0ad4e;border-color:#eea236}.btn-warning.focus,.btn-warning:focus{color:#fff;background-color:#ec971f;border-color:#985f0d}.btn-warning:hover{color:#fff;background-color:#ec971f;border-color:#d58512}.btn-warning.active,.btn-warning:active,.open>.dropdown-toggle.btn-warning{color:#fff;background-color:#ec971f;border-color:#d58512}.btn-warning.active.focus,.btn-warning.active:focus,.btn-warning.active:hover,.btn-warning:active.focus,.btn-warning:active:focus,.btn-warning:active:hover,.open>.dropdown-toggle.btn-warning.focus,.open>.dropdown-toggle.btn-warning:focus,.open>.dropdown-toggle.btn-warning:hover{color:#fff;background-color:#d58512;border-color:#985f0d}.btn-warning.active,.btn-warning:active,.open>.dropdown-toggle.btn-warning{background-image:none}.btn-warning.disabled.focus,.btn-warning.disabled:focus,.btn-warning.disabled:hover,.btn-warning[disabled].focus,.btn-warning[disabled]:focus,.btn-warning[disabled]:hover,fieldset[disabled] .btn-warning.focus,fieldset[disabled] .btn-warning:focus,fieldset[disabled] .btn-warning:hover{background-color:#f0ad4e;border-color:#eea236}.btn-warning .badge{color:#f0ad4e;background-color:#fff}.btn-danger{color:#fff;background-color:#d9534f;border-color:#d43f3a}.btn-danger.focus,.btn-danger:focus{color:#fff;background-color:#c9302c;border-color:#761c19}.btn-danger:hover{color:#fff;background-color:#c9302c;border-color:#ac2925}.btn-danger.active,.btn-danger:active,.open>.dropdown-toggle.btn-danger{color:#fff;background-color:#c9302c;border-color:#ac2925}.btn-danger.active.focus,.btn-danger.active:focus,.btn-danger.active:hover,.btn-danger:active.focus,.btn-danger:active:focus,.btn-danger:active:hover,.open>.dropdown-toggle.btn-danger.focus,.open>.dropdown-toggle.btn-danger:focus,.open>.dropdown-toggle.btn-danger:hover{color:#fff;background-color:#ac2925;border-color:#761c19}.btn-danger.active,.btn-danger:active,.open>.dropdown-toggle.btn-danger{background-image:none}.btn-danger.disabled.focus,.btn-danger.disabled:focus,.btn-danger.disabled:hover,.btn-danger[disabled].focus,.btn-danger[disabled]:focus,.btn-danger[disabled]:hover,fieldset[disabled] .btn-danger.focus,fieldset[disabled] .btn-danger:focus,fieldset[disabled] .btn-danger:hover{background-color:#d9534f;border-color:#d43f3a}.btn-danger .badge{color:#d9534f;background-color:#fff}.btn-link{font-weight:400;color:#337ab7;border-radius:0}.btn-link,.btn-link.active,.btn-link:active,.btn-link[disabled],fieldset[disabled] .btn-link{background-color:transparent;-webkit-box-shadow:none;box-shadow:none}.btn-link,.btn-link:active,.btn-link:focus,.btn-link:hover{border-color:transparent}.btn-link:focus,.btn-link:hover{color:#23527c;text-decoration:underline;background-color:transparent}.btn-link[disabled]:focus,.btn-link[disabled]:hover,fieldset[disabled] .btn-link:focus,fieldset[disabled] .btn-link:hover{color:#777;text-decoration:none}.btn-group-lg>.btn,.btn-lg{padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.btn-group-sm>.btn,.btn-sm{padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.btn-group-xs>.btn,.btn-xs{padding:1px 5px;font-size:12px;line-height:1.5;border-radius:3px}.btn-block{display:block;width:100%}.btn-block+.btn-block{margin-top:5px}input[type=button].btn-block,input[type=reset].btn-block,input[type=submit].btn-block{width:100%}.fade{opacity:0;-webkit-transition:opacity .15s linear;-o-transition:opacity .15s linear;transition:opacity .15s linear}.fade.in{opacity:1}.collapse{display:none}.collapse.in{display:block}tr.collapse.in{display:table-row}tbody.collapse.in{display:table-row-group}.collapsing{position:relative;height:0;overflow:hidden;-webkit-transition-timing-function:ease;-o-transition-timing-function:ease;transition-timing-function:ease;-webkit-transition-duration:.35s;-o-transition-duration:.35s;transition-duration:.35s;-webkit-transition-property:height,visibility;-o-transition-property:height,visibility;transition-property:height,visibility}.caret{display:inline-block;width:0;height:0;margin-left:2px;vertical-align:middle;border-top:4px dashed;border-top:4px solid\9;border-right:4px solid transparent;border-left:4px solid transparent}.dropdown,.dropup{position:relative}.dropdown-toggle:focus{outline:0}.dropdown-menu{position:absolute;top:100%;left:0;z-index:1000;display:none;float:left;min-width:160px;padding:5px 0;margin:2px 0 0;font-size:14px;text-align:left;list-style:none;background-color:#fff;-webkit-background-clip:padding-box;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.15);border-radius:4px;-webkit-box-shadow:0 6px 12px rgba(0,0,0,.175);box-shadow:0 6px 12px rgba(0,0,0,.175)}.dropdown-menu.pull-right{right:0;left:auto}.dropdown-menu .divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.dropdown-menu>li>a{display:block;padding:3px 20px;clear:both;font-weight:400;line-height:1.42857143;color:#333;white-space:nowrap}.dropdown-menu>li>a:focus,.dropdown-menu>li>a:hover{color:#262626;text-decoration:none;background-color:#f5f5f5}.dropdown-menu>.active>a,.dropdown-menu>.active>a:focus,.dropdown-menu>.active>a:hover{color:#fff;text-decoration:none;background-color:#337ab7;outline:0}.dropdown-menu>.disabled>a,.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{color:#777}.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{text-decoration:none;cursor:not-allowed;background-color:transparent;background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled=false)}.open>.dropdown-menu{display:block}.open>a{outline:0}.dropdown-menu-right{right:0;left:auto}.dropdown-menu-left{right:auto;left:0}.dropdown-header{display:block;padding:3px 20px;font-size:12px;line-height:1.42857143;color:#777;white-space:nowrap}.dropdown-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:990}.pull-right>.dropdown-menu{right:0;left:auto}.dropup .caret,.navbar-fixed-bottom .dropdown .caret{content:"";border-top:0;border-bottom:4px dashed;border-bottom:4px solid\9}.dropup .dropdown-menu,.navbar-fixed-bottom .dropdown .dropdown-menu{top:auto;bottom:100%;margin-bottom:2px}@media (min-width:768px){.navbar-right .dropdown-menu{right:0;left:auto}.navbar-right .dropdown-menu-left{right:auto;left:0}}.btn-group,.btn-group-vertical{position:relative;display:inline-block;vertical-align:middle}.btn-group-vertical>.btn,.btn-group>.btn{position:relative;float:left}.btn-group-vertical>.btn.active,.btn-group-vertical>.btn:active,.btn-group-vertical>.btn:focus,.btn-group-vertical>.btn:hover,.btn-group>.btn.active,.btn-group>.btn:active,.btn-group>.btn:focus,.btn-group>.btn:hover{z-index:2}.btn-group .btn+.btn,.btn-group .btn+.btn-group,.btn-group .btn-group+.btn,.btn-group .btn-group+.btn-group{margin-left:-1px}.btn-toolbar{margin-left:-5px}.btn-toolbar .btn,.btn-toolbar .btn-group,.btn-toolbar .input-group{float:left}.btn-toolbar>.btn,.btn-toolbar>.btn-group,.btn-toolbar>.input-group{margin-left:5px}.btn-group>.btn:not(:first-child):not(:last-child):not(.dropdown-toggle){border-radius:0}.btn-group>.btn:first-child{margin-left:0}.btn-group>.btn:first-child:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn:last-child:not(:first-child),.btn-group>.dropdown-toggle:not(:first-child){border-top-left-radius:0;border-bottom-left-radius:0}.btn-group>.btn-group{float:left}.btn-group>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-bottom-left-radius:0}.btn-group .dropdown-toggle:active,.btn-group.open .dropdown-toggle{outline:0}.btn-group>.btn+.dropdown-toggle{padding-right:8px;padding-left:8px}.btn-group>.btn-lg+.dropdown-toggle{padding-right:12px;padding-left:12px}.btn-group.open .dropdown-toggle{-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn-group.open .dropdown-toggle.btn-link{-webkit-box-shadow:none;box-shadow:none}.btn .caret{margin-left:0}.btn-lg .caret{border-width:5px 5px 0;border-bottom-width:0}.dropup .btn-lg .caret{border-width:0 5px 5px}.btn-group-vertical>.btn,.btn-group-vertical>.btn-group,.btn-group-vertical>.btn-group>.btn{display:block;float:none;width:100%;max-width:100%}.btn-group-vertical>.btn-group>.btn{float:none}.btn-group-vertical>.btn+.btn,.btn-group-vertical>.btn+.btn-group,.btn-group-vertical>.btn-group+.btn,.btn-group-vertical>.btn-group+.btn-group{margin-top:-1px;margin-left:0}.btn-group-vertical>.btn:not(:first-child):not(:last-child){border-radius:0}.btn-group-vertical>.btn:first-child:not(:last-child){border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn:last-child:not(:first-child){border-top-left-radius:0;border-top-right-radius:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.btn-group-vertical>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group-vertical>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group-vertical>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-top-right-radius:0}.btn-group-justified{display:table;width:100%;table-layout:fixed;border-collapse:separate}.btn-group-justified>.btn,.btn-group-justified>.btn-group{display:table-cell;float:none;width:1%}.btn-group-justified>.btn-group .btn{width:100%}.btn-group-justified>.btn-group .dropdown-menu{left:auto}[data-toggle=buttons]>.btn input[type=checkbox],[data-toggle=buttons]>.btn input[type=radio],[data-toggle=buttons]>.btn-group>.btn input[type=checkbox],[data-toggle=buttons]>.btn-group>.btn input[type=radio]{position:absolute;clip:rect(0,0,0,0);pointer-events:none}.input-group{position:relative;display:table;border-collapse:separate}.input-group[class*=col-]{float:none;padding-right:0;padding-left:0}.input-group .form-control{position:relative;z-index:2;float:left;width:100%;margin-bottom:0}.input-group .form-control:focus{z-index:3}.input-group-lg>.form-control,.input-group-lg>.input-group-addon,.input-group-lg>.input-group-btn>.btn{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-group-lg>.form-control,select.input-group-lg>.input-group-addon,select.input-group-lg>.input-group-btn>.btn{height:46px;line-height:46px}select[multiple].input-group-lg>.form-control,select[multiple].input-group-lg>.input-group-addon,select[multiple].input-group-lg>.input-group-btn>.btn,textarea.input-group-lg>.form-control,textarea.input-group-lg>.input-group-addon,textarea.input-group-lg>.input-group-btn>.btn{height:auto}.input-group-sm>.form-control,.input-group-sm>.input-group-addon,.input-group-sm>.input-group-btn>.btn{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-group-sm>.form-control,select.input-group-sm>.input-group-addon,select.input-group-sm>.input-group-btn>.btn{height:30px;line-height:30px}select[multiple].input-group-sm>.form-control,select[multiple].input-group-sm>.input-group-addon,select[multiple].input-group-sm>.input-group-btn>.btn,textarea.input-group-sm>.form-control,textarea.input-group-sm>.input-group-addon,textarea.input-group-sm>.input-group-btn>.btn{height:auto}.input-group .form-control,.input-group-addon,.input-group-btn{display:table-cell}.input-group .form-control:not(:first-child):not(:last-child),.input-group-addon:not(:first-child):not(:last-child),.input-group-btn:not(:first-child):not(:last-child){border-radius:0}.input-group-addon,.input-group-btn{width:1%;white-space:nowrap;vertical-align:middle}.input-group-addon{padding:6px 12px;font-size:14px;font-weight:400;line-height:1;color:#555;text-align:center;background-color:#eee;border:1px solid #ccc;border-radius:4px}.input-group-addon.input-sm{padding:5px 10px;font-size:12px;border-radius:3px}.input-group-addon.input-lg{padding:10px 16px;font-size:18px;border-radius:6px}.input-group-addon input[type=checkbox],.input-group-addon input[type=radio]{margin-top:0}.input-group .form-control:first-child,.input-group-addon:first-child,.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group>.btn,.input-group-btn:first-child>.dropdown-toggle,.input-group-btn:last-child>.btn-group:not(:last-child)>.btn,.input-group-btn:last-child>.btn:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.input-group-addon:first-child{border-right:0}.input-group .form-control:last-child,.input-group-addon:last-child,.input-group-btn:first-child>.btn-group:not(:first-child)>.btn,.input-group-btn:first-child>.btn:not(:first-child),.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group>.btn,.input-group-btn:last-child>.dropdown-toggle{border-top-left-radius:0;border-bottom-left-radius:0}.input-group-addon:last-child{border-left:0}.input-group-btn{position:relative;font-size:0;white-space:nowrap}.input-group-btn>.btn{position:relative}.input-group-btn>.btn+.btn{margin-left:-1px}.input-group-btn>.btn:active,.input-group-btn>.btn:focus,.input-group-btn>.btn:hover{z-index:2}.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group{margin-right:-1px}.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group{z-index:2;margin-left:-1px}.nav{padding-left:0;margin-bottom:0;list-style:none}.nav>li{position:relative;display:block}.nav>li>a{position:relative;display:block;padding:10px 15px}.nav>li>a:focus,.nav>li>a:hover{text-decoration:none;background-color:#eee}.nav>li.disabled>a{color:#777}.nav>li.disabled>a:focus,.nav>li.disabled>a:hover{color:#777;text-decoration:none;cursor:not-allowed;background-color:transparent}.nav .open>a,.nav .open>a:focus,.nav .open>a:hover{background-color:#eee;border-color:#337ab7}.nav .nav-divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.nav>li>a>img{max-width:none}.nav-tabs{border-bottom:1px solid #ddd}.nav-tabs>li{float:left;margin-bottom:-1px}.nav-tabs>li>a{margin-right:2px;line-height:1.42857143;border:1px solid transparent;border-radius:4px 4px 0 0}.nav-tabs>li>a:hover{border-color:#eee #eee #ddd}.nav-tabs>li.active>a,.nav-tabs>li.active>a:focus,.nav-tabs>li.active>a:hover{color:#555;cursor:default;background-color:#fff;border:1px solid #ddd;border-bottom-color:transparent}.nav-tabs.nav-justified{width:100%;border-bottom:0}.nav-tabs.nav-justified>li{float:none}.nav-tabs.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-tabs.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-tabs.nav-justified>li{display:table-cell;width:1%}.nav-tabs.nav-justified>li>a{margin-bottom:0}}.nav-tabs.nav-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs.nav-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border-bottom-color:#fff}}.nav-pills>li{float:left}.nav-pills>li>a{border-radius:4px}.nav-pills>li+li{margin-left:2px}.nav-pills>li.active>a,.nav-pills>li.active>a:focus,.nav-pills>li.active>a:hover{color:#fff;background-color:#337ab7}.nav-stacked>li{float:none}.nav-stacked>li+li{margin-top:2px;margin-left:0}.nav-justified{width:100%}.nav-justified>li{float:none}.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-justified>li{display:table-cell;width:1%}.nav-justified>li>a{margin-bottom:0}}.nav-tabs-justified{border-bottom:0}.nav-tabs-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border-bottom-color:#fff}}.tab-content>.tab-pane{display:none}.tab-content>.active{display:block}.nav-tabs .dropdown-menu{margin-top:-1px;border-top-left-radius:0;border-top-right-radius:0}.navbar{position:relative;min-height:50px;margin-bottom:20px;border:1px solid transparent}@media (min-width:768px){.navbar{border-radius:4px}}@media (min-width:768px){.navbar-header{float:left}}.navbar-collapse{padding-right:15px;padding-left:15px;overflow-x:visible;-webkit-overflow-scrolling:touch;border-top:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1)}.navbar-collapse.in{overflow-y:auto}@media (min-width:768px){.navbar-collapse{width:auto;border-top:0;-webkit-box-shadow:none;box-shadow:none}.navbar-collapse.collapse{display:block!important;height:auto!important;padding-bottom:0;overflow:visible!important}.navbar-collapse.in{overflow-y:visible}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse,.navbar-static-top .navbar-collapse{padding-right:0;padding-left:0}}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:340px}@media (max-device-width:480px) and (orientation:landscape){.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:200px}}.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:0;margin-left:0}}.navbar-static-top{z-index:1000;border-width:0 0 1px}@media (min-width:768px){.navbar-static-top{border-radius:0}}.navbar-fixed-bottom,.navbar-fixed-top{position:fixed;right:0;left:0;z-index:1030}@media (min-width:768px){.navbar-fixed-bottom,.navbar-fixed-top{border-radius:0}}.navbar-fixed-top{top:0;border-width:0 0 1px}.navbar-fixed-bottom{bottom:0;margin-bottom:0;border-width:1px 0 0}.navbar-brand{float:left;height:50px;padding:15px 15px;font-size:18px;line-height:20px}.navbar-brand:focus,.navbar-brand:hover{text-decoration:none}.navbar-brand>img{display:block}@media (min-width:768px){.navbar>.container .navbar-brand,.navbar>.container-fluid .navbar-brand{margin-left:-15px}}.navbar-toggle{position:relative;float:right;padding:9px 10px;margin-top:8px;margin-right:15px;margin-bottom:8px;background-color:transparent;background-image:none;border:1px solid transparent;border-radius:4px}.navbar-toggle:focus{outline:0}.navbar-toggle .icon-bar{display:block;width:22px;height:2px;border-radius:1px}.navbar-toggle .icon-bar+.icon-bar{margin-top:4px}@media (min-width:768px){.navbar-toggle{display:none}}.navbar-nav{margin:7.5px -15px}.navbar-nav>li>a{padding-top:10px;padding-bottom:10px;line-height:20px}@media (max-width:767px){.navbar-nav .open .dropdown-menu{position:static;float:none;width:auto;margin-top:0;background-color:transparent;border:0;-webkit-box-shadow:none;box-shadow:none}.navbar-nav .open .dropdown-menu .dropdown-header,.navbar-nav .open .dropdown-menu>li>a{padding:5px 15px 5px 25px}.navbar-nav .open .dropdown-menu>li>a{line-height:20px}.navbar-nav .open .dropdown-menu>li>a:focus,.navbar-nav .open .dropdown-menu>li>a:hover{background-image:none}}@media (min-width:768px){.navbar-nav{float:left;margin:0}.navbar-nav>li{float:left}.navbar-nav>li>a{padding-top:15px;padding-bottom:15px}}.navbar-form{padding:10px 15px;margin-top:8px;margin-right:-15px;margin-bottom:8px;margin-left:-15px;border-top:1px solid transparent;border-bottom:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1)}@media (min-width:768px){.navbar-form .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.navbar-form .form-control{display:inline-block;width:auto;vertical-align:middle}.navbar-form .form-control-static{display:inline-block}.navbar-form .input-group{display:inline-table;vertical-align:middle}.navbar-form .input-group .form-control,.navbar-form .input-group .input-group-addon,.navbar-form .input-group .input-group-btn{width:auto}.navbar-form .input-group>.form-control{width:100%}.navbar-form .control-label{margin-bottom:0;vertical-align:middle}.navbar-form .checkbox,.navbar-form .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.navbar-form .checkbox label,.navbar-form .radio label{padding-left:0}.navbar-form .checkbox input[type=checkbox],.navbar-form .radio input[type=radio]{position:relative;margin-left:0}.navbar-form .has-feedback .form-control-feedback{top:0}}@media (max-width:767px){.navbar-form .form-group{margin-bottom:5px}.navbar-form .form-group:last-child{margin-bottom:0}}@media (min-width:768px){.navbar-form{width:auto;padding-top:0;padding-bottom:0;margin-right:0;margin-left:0;border:0;-webkit-box-shadow:none;box-shadow:none}}.navbar-nav>li>.dropdown-menu{margin-top:0;border-top-left-radius:0;border-top-right-radius:0}.navbar-fixed-bottom .navbar-nav>li>.dropdown-menu{margin-bottom:0;border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.navbar-btn{margin-top:8px;margin-bottom:8px}.navbar-btn.btn-sm{margin-top:10px;margin-bottom:10px}.navbar-btn.btn-xs{margin-top:14px;margin-bottom:14px}.navbar-text{margin-top:15px;margin-bottom:15px}@media (min-width:768px){.navbar-text{float:left;margin-right:15px;margin-left:15px}}@media (min-width:768px){.navbar-left{float:left!important}.navbar-right{float:right!important;margin-right:-15px}.navbar-right~.navbar-right{margin-right:0}}.navbar-default{background-color:#f8f8f8;border-color:#e7e7e7}.navbar-default .navbar-brand{color:#777}.navbar-default .navbar-brand:focus,.navbar-default .navbar-brand:hover{color:#5e5e5e;background-color:transparent}.navbar-default .navbar-text{color:#777}.navbar-default .navbar-nav>li>a{color:#777}.navbar-default .navbar-nav>li>a:focus,.navbar-default .navbar-nav>li>a:hover{color:#333;background-color:transparent}.navbar-default .navbar-nav>.active>a,.navbar-default .navbar-nav>.active>a:focus,.navbar-default .navbar-nav>.active>a:hover{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav>.disabled>a,.navbar-default .navbar-nav>.disabled>a:focus,.navbar-default .navbar-nav>.disabled>a:hover{color:#ccc;background-color:transparent}.navbar-default .navbar-toggle{border-color:#ddd}.navbar-default .navbar-toggle:focus,.navbar-default .navbar-toggle:hover{background-color:#ddd}.navbar-default .navbar-toggle .icon-bar{background-color:#888}.navbar-default .navbar-collapse,.navbar-default .navbar-form{border-color:#e7e7e7}.navbar-default .navbar-nav>.open>a,.navbar-default .navbar-nav>.open>a:focus,.navbar-default .navbar-nav>.open>a:hover{color:#555;background-color:#e7e7e7}@media (max-width:767px){.navbar-default .navbar-nav .open .dropdown-menu>li>a{color:#777}.navbar-default .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>li>a:hover{color:#333;background-color:transparent}.navbar-default .navbar-nav .open .dropdown-menu>.active>a,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:hover{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#ccc;background-color:transparent}}.navbar-default .navbar-link{color:#777}.navbar-default .navbar-link:hover{color:#333}.navbar-default .btn-link{color:#777}.navbar-default .btn-link:focus,.navbar-default .btn-link:hover{color:#333}.navbar-default .btn-link[disabled]:focus,.navbar-default .btn-link[disabled]:hover,fieldset[disabled] .navbar-default .btn-link:focus,fieldset[disabled] .navbar-default .btn-link:hover{color:#ccc}.navbar-inverse{background-color:#222;border-color:#080808}.navbar-inverse .navbar-brand{color:#9d9d9d}.navbar-inverse .navbar-brand:focus,.navbar-inverse .navbar-brand:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-text{color:#9d9d9d}.navbar-inverse .navbar-nav>li>a{color:#9d9d9d}.navbar-inverse .navbar-nav>li>a:focus,.navbar-inverse .navbar-nav>li>a:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav>.active>a,.navbar-inverse .navbar-nav>.active>a:focus,.navbar-inverse .navbar-nav>.active>a:hover{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav>.disabled>a,.navbar-inverse .navbar-nav>.disabled>a:focus,.navbar-inverse .navbar-nav>.disabled>a:hover{color:#444;background-color:transparent}.navbar-inverse .navbar-toggle{border-color:#333}.navbar-inverse .navbar-toggle:focus,.navbar-inverse .navbar-toggle:hover{background-color:#333}.navbar-inverse .navbar-toggle .icon-bar{background-color:#fff}.navbar-inverse .navbar-collapse,.navbar-inverse .navbar-form{border-color:#101010}.navbar-inverse .navbar-nav>.open>a,.navbar-inverse .navbar-nav>.open>a:focus,.navbar-inverse .navbar-nav>.open>a:hover{color:#fff;background-color:#080808}@media (max-width:767px){.navbar-inverse .navbar-nav .open .dropdown-menu>.dropdown-header{border-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu .divider{background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a{color:#9d9d9d}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:hover{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#444;background-color:transparent}}.navbar-inverse .navbar-link{color:#9d9d9d}.navbar-inverse .navbar-link:hover{color:#fff}.navbar-inverse .btn-link{color:#9d9d9d}.navbar-inverse .btn-link:focus,.navbar-inverse .btn-link:hover{color:#fff}.navbar-inverse .btn-link[disabled]:focus,.navbar-inverse .btn-link[disabled]:hover,fieldset[disabled] .navbar-inverse .btn-link:focus,fieldset[disabled] .navbar-inverse .btn-link:hover{color:#444}.breadcrumb{padding:8px 15px;margin-bottom:20px;list-style:none;background-color:#f5f5f5;border-radius:4px}.breadcrumb>li{display:inline-block}.breadcrumb>li+li:before{padding:0 5px;color:#ccc;content:"/\00a0"}.breadcrumb>.active{color:#777}.pagination{display:inline-block;padding-left:0;margin:20px 0;border-radius:4px}.pagination>li{display:inline}.pagination>li>a,.pagination>li>span{position:relative;float:left;padding:6px 12px;margin-left:-1px;line-height:1.42857143;color:#337ab7;text-decoration:none;background-color:#fff;border:1px solid #ddd}.pagination>li:first-child>a,.pagination>li:first-child>span{margin-left:0;border-top-left-radius:4px;border-bottom-left-radius:4px}.pagination>li:last-child>a,.pagination>li:last-child>span{border-top-right-radius:4px;border-bottom-right-radius:4px}.pagination>li>a:focus,.pagination>li>a:hover,.pagination>li>span:focus,.pagination>li>span:hover{z-index:2;color:#23527c;background-color:#eee;border-color:#ddd}.pagination>.active>a,.pagination>.active>a:focus,.pagination>.active>a:hover,.pagination>.active>span,.pagination>.active>span:focus,.pagination>.active>span:hover{z-index:3;color:#fff;cursor:default;background-color:#337ab7;border-color:#337ab7}.pagination>.disabled>a,.pagination>.disabled>a:focus,.pagination>.disabled>a:hover,.pagination>.disabled>span,.pagination>.disabled>span:focus,.pagination>.disabled>span:hover{color:#777;cursor:not-allowed;background-color:#fff;border-color:#ddd}.pagination-lg>li>a,.pagination-lg>li>span{padding:10px 16px;font-size:18px;line-height:1.3333333}.pagination-lg>li:first-child>a,.pagination-lg>li:first-child>span{border-top-left-radius:6px;border-bottom-left-radius:6px}.pagination-lg>li:last-child>a,.pagination-lg>li:last-child>span{border-top-right-radius:6px;border-bottom-right-radius:6px}.pagination-sm>li>a,.pagination-sm>li>span{padding:5px 10px;font-size:12px;line-height:1.5}.pagination-sm>li:first-child>a,.pagination-sm>li:first-child>span{border-top-left-radius:3px;border-bottom-left-radius:3px}.pagination-sm>li:last-child>a,.pagination-sm>li:last-child>span{border-top-right-radius:3px;border-bottom-right-radius:3px}.pager{padding-left:0;margin:20px 0;text-align:center;list-style:none}.pager li{display:inline}.pager li>a,.pager li>span{display:inline-block;padding:5px 14px;background-color:#fff;border:1px solid #ddd;border-radius:15px}.pager li>a:focus,.pager li>a:hover{text-decoration:none;background-color:#eee}.pager .next>a,.pager .next>span{float:right}.pager .previous>a,.pager .previous>span{float:left}.pager .disabled>a,.pager .disabled>a:focus,.pager .disabled>a:hover,.pager .disabled>span{color:#777;cursor:not-allowed;background-color:#fff}.label{display:inline;padding:.2em .6em .3em;font-size:75%;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:.25em}a.label:focus,a.label:hover{color:#fff;text-decoration:none;cursor:pointer}.label:empty{display:none}.btn .label{position:relative;top:-1px}.label-default{background-color:#777}.label-default[href]:focus,.label-default[href]:hover{background-color:#5e5e5e}.label-primary{background-color:#337ab7}.label-primary[href]:focus,.label-primary[href]:hover{background-color:#286090}.label-success{background-color:#5cb85c}.label-success[href]:focus,.label-success[href]:hover{background-color:#449d44}.label-info{background-color:#5bc0de}.label-info[href]:focus,.label-info[href]:hover{background-color:#31b0d5}.label-warning{background-color:#f0ad4e}.label-warning[href]:focus,.label-warning[href]:hover{background-color:#ec971f}.label-danger{background-color:#d9534f}.label-danger[href]:focus,.label-danger[href]:hover{background-color:#c9302c}.badge{display:inline-block;min-width:10px;padding:3px 7px;font-size:12px;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:middle;background-color:#777;border-radius:10px}.badge:empty{display:none}.btn .badge{position:relative;top:-1px}.btn-group-xs>.btn .badge,.btn-xs .badge{top:0;padding:1px 5px}a.badge:focus,a.badge:hover{color:#fff;text-decoration:none;cursor:pointer}.list-group-item.active>.badge,.nav-pills>.active>a>.badge{color:#337ab7;background-color:#fff}.list-group-item>.badge{float:right}.list-group-item>.badge+.badge{margin-right:5px}.nav-pills>li>a>.badge{margin-left:3px}.jumbotron{padding-top:30px;padding-bottom:30px;margin-bottom:30px;color:inherit;background-color:#eee}.jumbotron .h1,.jumbotron h1{color:inherit}.jumbotron p{margin-bottom:15px;font-size:21px;font-weight:200}.jumbotron>hr{border-top-color:#d5d5d5}.container .jumbotron,.container-fluid .jumbotron{padding-right:15px;padding-left:15px;border-radius:6px}.jumbotron .container{max-width:100%}@media screen and (min-width:768px){.jumbotron{padding-top:48px;padding-bottom:48px}.container .jumbotron,.container-fluid .jumbotron{padding-right:60px;padding-left:60px}.jumbotron .h1,.jumbotron h1{font-size:63px}}.thumbnail{display:block;padding:4px;margin-bottom:20px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:border .2s ease-in-out;-o-transition:border .2s ease-in-out;transition:border .2s ease-in-out}.thumbnail a>img,.thumbnail>img{margin-right:auto;margin-left:auto}a.thumbnail.active,a.thumbnail:focus,a.thumbnail:hover{border-color:#337ab7}.thumbnail .caption{padding:9px;color:#333}.alert{padding:15px;margin-bottom:20px;border:1px solid transparent;border-radius:4px}.alert h4{margin-top:0;color:inherit}.alert .alert-link{font-weight:700}.alert>p,.alert>ul{margin-bottom:0}.alert>p+p{margin-top:5px}.alert-dismissable,.alert-dismissible{padding-right:35px}.alert-dismissable .close,.alert-dismissible .close{position:relative;top:-2px;right:-21px;color:inherit}.alert-success{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.alert-success hr{border-top-color:#c9e2b3}.alert-success .alert-link{color:#2b542c}.alert-info{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.alert-info hr{border-top-color:#a6e1ec}.alert-info .alert-link{color:#245269}.alert-warning{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.alert-warning hr{border-top-color:#f7e1b5}.alert-warning .alert-link{color:#66512c}.alert-danger{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.alert-danger hr{border-top-color:#e4b9c0}.alert-danger .alert-link{color:#843534}@-webkit-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@-o-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}.progress{height:20px;margin-bottom:20px;overflow:hidden;background-color:#f5f5f5;border-radius:4px;-webkit-box-shadow:inset 0 1px 2px rgba(0,0,0,.1);box-shadow:inset 0 1px 2px rgba(0,0,0,.1)}.progress-bar{float:left;width:0;height:100%;font-size:12px;line-height:20px;color:#fff;text-align:center;background-color:#337ab7;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);-webkit-transition:width .6s ease;-o-transition:width .6s ease;transition:width .6s ease}.progress-bar-striped,.progress-striped .progress-bar{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);-webkit-background-size:40px 40px;background-size:40px 40px}.progress-bar.active,.progress.active .progress-bar{-webkit-animation:progress-bar-stripes 2s linear infinite;-o-animation:progress-bar-stripes 2s linear infinite;animation:progress-bar-stripes 2s linear infinite}.progress-bar-success{background-color:#5cb85c}.progress-striped .progress-bar-success{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-info{background-color:#5bc0de}.progress-striped .progress-bar-info{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-warning{background-color:#f0ad4e}.progress-striped .progress-bar-warning{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-danger{background-color:#d9534f}.progress-striped .progress-bar-danger{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.media{margin-top:15px}.media:first-child{margin-top:0}.media,.media-body{overflow:hidden;zoom:1}.media-body{width:10000px}.media-object{display:block}.media-object.img-thumbnail{max-width:none}.media-right,.media>.pull-right{padding-left:10px}.media-left,.media>.pull-left{padding-right:10px}.media-body,.media-left,.media-right{display:table-cell;vertical-align:top}.media-middle{vertical-align:middle}.media-bottom{vertical-align:bottom}.media-heading{margin-top:0;margin-bottom:5px}.media-list{padding-left:0;list-style:none}.list-group{padding-left:0;margin-bottom:20px}.list-group-item{position:relative;display:block;padding:10px 15px;margin-bottom:-1px;background-color:#fff;border:1px solid #ddd}.list-group-item:first-child{border-top-left-radius:4px;border-top-right-radius:4px}.list-group-item:last-child{margin-bottom:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}a.list-group-item,button.list-group-item{color:#555}a.list-group-item .list-group-item-heading,button.list-group-item .list-group-item-heading{color:#333}a.list-group-item:focus,a.list-group-item:hover,button.list-group-item:focus,button.list-group-item:hover{color:#555;text-decoration:none;background-color:#f5f5f5}button.list-group-item{width:100%;text-align:left}.list-group-item.disabled,.list-group-item.disabled:focus,.list-group-item.disabled:hover{color:#777;cursor:not-allowed;background-color:#eee}.list-group-item.disabled .list-group-item-heading,.list-group-item.disabled:focus .list-group-item-heading,.list-group-item.disabled:hover .list-group-item-heading{color:inherit}.list-group-item.disabled .list-group-item-text,.list-group-item.disabled:focus .list-group-item-text,.list-group-item.disabled:hover .list-group-item-text{color:#777}.list-group-item.active,.list-group-item.active:focus,.list-group-item.active:hover{z-index:2;color:#fff;background-color:#337ab7;border-color:#337ab7}.list-group-item.active .list-group-item-heading,.list-group-item.active .list-group-item-heading>.small,.list-group-item.active .list-group-item-heading>small,.list-group-item.active:focus .list-group-item-heading,.list-group-item.active:focus .list-group-item-heading>.small,.list-group-item.active:focus .list-group-item-heading>small,.list-group-item.active:hover .list-group-item-heading,.list-group-item.active:hover .list-group-item-heading>.small,.list-group-item.active:hover .list-group-item-heading>small{color:inherit}.list-group-item.active .list-group-item-text,.list-group-item.active:focus .list-group-item-text,.list-group-item.active:hover .list-group-item-text{color:#c7ddef}.list-group-item-success{color:#3c763d;background-color:#dff0d8}a.list-group-item-success,button.list-group-item-success{color:#3c763d}a.list-group-item-success .list-group-item-heading,button.list-group-item-success .list-group-item-heading{color:inherit}a.list-group-item-success:focus,a.list-group-item-success:hover,button.list-group-item-success:focus,button.list-group-item-success:hover{color:#3c763d;background-color:#d0e9c6}a.list-group-item-success.active,a.list-group-item-success.active:focus,a.list-group-item-success.active:hover,button.list-group-item-success.active,button.list-group-item-success.active:focus,button.list-group-item-success.active:hover{color:#fff;background-color:#3c763d;border-color:#3c763d}.list-group-item-info{color:#31708f;background-color:#d9edf7}a.list-group-item-info,button.list-group-item-info{color:#31708f}a.list-group-item-info .list-group-item-heading,button.list-group-item-info .list-group-item-heading{color:inherit}a.list-group-item-info:focus,a.list-group-item-info:hover,button.list-group-item-info:focus,button.list-group-item-info:hover{color:#31708f;background-color:#c4e3f3}a.list-group-item-info.active,a.list-group-item-info.active:focus,a.list-group-item-info.active:hover,button.list-group-item-info.active,button.list-group-item-info.active:focus,button.list-group-item-info.active:hover{color:#fff;background-color:#31708f;border-color:#31708f}.list-group-item-warning{color:#8a6d3b;background-color:#fcf8e3}a.list-group-item-warning,button.list-group-item-warning{color:#8a6d3b}a.list-group-item-warning .list-group-item-heading,button.list-group-item-warning .list-group-item-heading{color:inherit}a.list-group-item-warning:focus,a.list-group-item-warning:hover,button.list-group-item-warning:focus,button.list-group-item-warning:hover{color:#8a6d3b;background-color:#faf2cc}a.list-group-item-warning.active,a.list-group-item-warning.active:focus,a.list-group-item-warning.active:hover,button.list-group-item-warning.active,button.list-group-item-warning.active:focus,button.list-group-item-warning.active:hover{color:#fff;background-color:#8a6d3b;border-color:#8a6d3b}.list-group-item-danger{color:#a94442;background-color:#f2dede}a.list-group-item-danger,button.list-group-item-danger{color:#a94442}a.list-group-item-danger .list-group-item-heading,button.list-group-item-danger .list-group-item-heading{color:inherit}a.list-group-item-danger:focus,a.list-group-item-danger:hover,button.list-group-item-danger:focus,button.list-group-item-danger:hover{color:#a94442;background-color:#ebcccc}a.list-group-item-danger.active,a.list-group-item-danger.active:focus,a.list-group-item-danger.active:hover,button.list-group-item-danger.active,button.list-group-item-danger.active:focus,button.list-group-item-danger.active:hover{color:#fff;background-color:#a94442;border-color:#a94442}.list-group-item-heading{margin-top:0;margin-bottom:5px}.list-group-item-text{margin-bottom:0;line-height:1.3}.panel{margin-bottom:20px;background-color:#fff;border:1px solid transparent;border-radius:4px;-webkit-box-shadow:0 1px 1px rgba(0,0,0,.05);box-shadow:0 1px 1px rgba(0,0,0,.05)}.panel-body{padding:15px}.panel-heading{padding:10px 15px;border-bottom:1px solid transparent;border-top-left-radius:3px;border-top-right-radius:3px}.panel-heading>.dropdown .dropdown-toggle{color:inherit}.panel-title{margin-top:0;margin-bottom:0;font-size:16px;color:inherit}.panel-title>.small,.panel-title>.small>a,.panel-title>a,.panel-title>small,.panel-title>small>a{color:inherit}.panel-footer{padding:10px 15px;background-color:#f5f5f5;border-top:1px solid #ddd;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.list-group,.panel>.panel-collapse>.list-group{margin-bottom:0}.panel>.list-group .list-group-item,.panel>.panel-collapse>.list-group .list-group-item{border-width:1px 0;border-radius:0}.panel>.list-group:first-child .list-group-item:first-child,.panel>.panel-collapse>.list-group:first-child .list-group-item:first-child{border-top:0;border-top-left-radius:3px;border-top-right-radius:3px}.panel>.list-group:last-child .list-group-item:last-child,.panel>.panel-collapse>.list-group:last-child .list-group-item:last-child{border-bottom:0;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.panel-heading+.panel-collapse>.list-group .list-group-item:first-child{border-top-left-radius:0;border-top-right-radius:0}.panel-heading+.list-group .list-group-item:first-child{border-top-width:0}.list-group+.panel-footer{border-top-width:0}.panel>.panel-collapse>.table,.panel>.table,.panel>.table-responsive>.table{margin-bottom:0}.panel>.panel-collapse>.table caption,.panel>.table caption,.panel>.table-responsive>.table caption{padding-right:15px;padding-left:15px}.panel>.table-responsive:first-child>.table:first-child,.panel>.table:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child,.panel>.table:first-child>thead:first-child>tr:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table:first-child>thead:first-child>tr:first-child th:first-child{border-top-left-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table:first-child>thead:first-child>tr:first-child th:last-child{border-top-right-radius:3px}.panel>.table-responsive:last-child>.table:last-child,.panel>.table:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:first-child{border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:last-child{border-bottom-right-radius:3px}.panel>.panel-body+.table,.panel>.panel-body+.table-responsive,.panel>.table+.panel-body,.panel>.table-responsive+.panel-body{border-top:1px solid #ddd}.panel>.table>tbody:first-child>tr:first-child td,.panel>.table>tbody:first-child>tr:first-child th{border-top:0}.panel>.table-bordered,.panel>.table-responsive>.table-bordered{border:0}.panel>.table-bordered>tbody>tr>td:first-child,.panel>.table-bordered>tbody>tr>th:first-child,.panel>.table-bordered>tfoot>tr>td:first-child,.panel>.table-bordered>tfoot>tr>th:first-child,.panel>.table-bordered>thead>tr>td:first-child,.panel>.table-bordered>thead>tr>th:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:first-child,.panel>.table-responsive>.table-bordered>thead>tr>td:first-child,.panel>.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.panel>.table-bordered>tbody>tr>td:last-child,.panel>.table-bordered>tbody>tr>th:last-child,.panel>.table-bordered>tfoot>tr>td:last-child,.panel>.table-bordered>tfoot>tr>th:last-child,.panel>.table-bordered>thead>tr>td:last-child,.panel>.table-bordered>thead>tr>th:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:last-child,.panel>.table-responsive>.table-bordered>thead>tr>td:last-child,.panel>.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.panel>.table-bordered>tbody>tr:first-child>td,.panel>.table-bordered>tbody>tr:first-child>th,.panel>.table-bordered>thead>tr:first-child>td,.panel>.table-bordered>thead>tr:first-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>th,.panel>.table-responsive>.table-bordered>thead>tr:first-child>td,.panel>.table-responsive>.table-bordered>thead>tr:first-child>th{border-bottom:0}.panel>.table-bordered>tbody>tr:last-child>td,.panel>.table-bordered>tbody>tr:last-child>th,.panel>.table-bordered>tfoot>tr:last-child>td,.panel>.table-bordered>tfoot>tr:last-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>th,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>td,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}.panel>.table-responsive{margin-bottom:0;border:0}.panel-group{margin-bottom:20px}.panel-group .panel{margin-bottom:0;border-radius:4px}.panel-group .panel+.panel{margin-top:5px}.panel-group .panel-heading{border-bottom:0}.panel-group .panel-heading+.panel-collapse>.list-group,.panel-group .panel-heading+.panel-collapse>.panel-body{border-top:1px solid #ddd}.panel-group .panel-footer{border-top:0}.panel-group .panel-footer+.panel-collapse .panel-body{border-bottom:1px solid #ddd}.panel-default{border-color:#ddd}.panel-default>.panel-heading{color:#333;background-color:#f5f5f5;border-color:#ddd}.panel-default>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ddd}.panel-default>.panel-heading .badge{color:#f5f5f5;background-color:#333}.panel-default>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ddd}.panel-primary{border-color:#337ab7}.panel-primary>.panel-heading{color:#fff;background-color:#337ab7;border-color:#337ab7}.panel-primary>.panel-heading+.panel-collapse>.panel-body{border-top-color:#337ab7}.panel-primary>.panel-heading .badge{color:#337ab7;background-color:#fff}.panel-primary>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#337ab7}.panel-success{border-color:#d6e9c6}.panel-success>.panel-heading{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.panel-success>.panel-heading+.panel-collapse>.panel-body{border-top-color:#d6e9c6}.panel-success>.panel-heading .badge{color:#dff0d8;background-color:#3c763d}.panel-success>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#d6e9c6}.panel-info{border-color:#bce8f1}.panel-info>.panel-heading{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.panel-info>.panel-heading+.panel-collapse>.panel-body{border-top-color:#bce8f1}.panel-info>.panel-heading .badge{color:#d9edf7;background-color:#31708f}.panel-info>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#bce8f1}.panel-warning{border-color:#faebcc}.panel-warning>.panel-heading{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.panel-warning>.panel-heading+.panel-collapse>.panel-body{border-top-color:#faebcc}.panel-warning>.panel-heading .badge{color:#fcf8e3;background-color:#8a6d3b}.panel-warning>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#faebcc}.panel-danger{border-color:#ebccd1}.panel-danger>.panel-heading{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.panel-danger>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ebccd1}.panel-danger>.panel-heading .badge{color:#f2dede;background-color:#a94442}.panel-danger>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ebccd1}.embed-responsive{position:relative;display:block;height:0;padding:0;overflow:hidden}.embed-responsive .embed-responsive-item,.embed-responsive embed,.embed-responsive iframe,.embed-responsive object,.embed-responsive video{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;border:0}.embed-responsive-16by9{padding-bottom:56.25%}.embed-responsive-4by3{padding-bottom:75%}.well{min-height:20px;padding:19px;margin-bottom:20px;background-color:#f5f5f5;border:1px solid #e3e3e3;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.05);box-shadow:inset 0 1px 1px rgba(0,0,0,.05)}.well blockquote{border-color:#ddd;border-color:rgba(0,0,0,.15)}.well-lg{padding:24px;border-radius:6px}.well-sm{padding:9px;border-radius:3px}.close{float:right;font-size:21px;font-weight:700;line-height:1;color:#000;text-shadow:0 1px 0 #fff;filter:alpha(opacity=20);opacity:.2}.close:focus,.close:hover{color:#000;text-decoration:none;cursor:pointer;filter:alpha(opacity=50);opacity:.5}button.close{-webkit-appearance:none;padding:0;cursor:pointer;background:0 0;border:0}.modal-open{overflow:hidden}.modal{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1050;display:none;overflow:hidden;-webkit-overflow-scrolling:touch;outline:0}.modal.fade .modal-dialog{-webkit-transition:-webkit-transform .3s ease-out;-o-transition:-o-transform .3s ease-out;transition:transform .3s ease-out;-webkit-transform:translate(0,-25%);-ms-transform:translate(0,-25%);-o-transform:translate(0,-25%);transform:translate(0,-25%)}.modal.in .modal-dialog{-webkit-transform:translate(0,0);-ms-transform:translate(0,0);-o-transform:translate(0,0);transform:translate(0,0)}.modal-open .modal{overflow-x:hidden;overflow-y:auto}.modal-dialog{position:relative;width:auto;margin:10px}.modal-content{position:relative;background-color:#fff;-webkit-background-clip:padding-box;background-clip:padding-box;border:1px solid #999;border:1px solid rgba(0,0,0,.2);border-radius:6px;outline:0;-webkit-box-shadow:0 3px 9px rgba(0,0,0,.5);box-shadow:0 3px 9px rgba(0,0,0,.5)}.modal-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1040;background-color:#000}.modal-backdrop.fade{filter:alpha(opacity=0);opacity:0}.modal-backdrop.in{filter:alpha(opacity=50);opacity:.5}.modal-header{padding:15px;border-bottom:1px solid #e5e5e5}.modal-header .close{margin-top:-2px}.modal-title{margin:0;line-height:1.42857143}.modal-body{position:relative;padding:15px}.modal-footer{padding:15px;text-align:right;border-top:1px solid #e5e5e5}.modal-footer .btn+.btn{margin-bottom:0;margin-left:5px}.modal-footer .btn-group .btn+.btn{margin-left:-1px}.modal-footer .btn-block+.btn-block{margin-left:0}.modal-scrollbar-measure{position:absolute;top:-9999px;width:50px;height:50px;overflow:scroll}@media (min-width:768px){.modal-dialog{width:600px;margin:30px auto}.modal-content{-webkit-box-shadow:0 5px 15px rgba(0,0,0,.5);box-shadow:0 5px 15px rgba(0,0,0,.5)}.modal-sm{width:300px}}@media (min-width:992px){.modal-lg{width:900px}}.tooltip{position:absolute;z-index:1070;display:block;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:12px;font-style:normal;font-weight:400;line-height:1.42857143;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;filter:alpha(opacity=0);opacity:0;line-break:auto}.tooltip.in{filter:alpha(opacity=90);opacity:.9}.tooltip.top{padding:5px 0;margin-top:-3px}.tooltip.right{padding:0 5px;margin-left:3px}.tooltip.bottom{padding:5px 0;margin-top:3px}.tooltip.left{padding:0 5px;margin-left:-3px}.tooltip-inner{max-width:200px;padding:3px 8px;color:#fff;text-align:center;background-color:#000;border-radius:4px}.tooltip-arrow{position:absolute;width:0;height:0;border-color:transparent;border-style:solid}.tooltip.top .tooltip-arrow{bottom:0;left:50%;margin-left:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-left .tooltip-arrow{right:5px;bottom:0;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-right .tooltip-arrow{bottom:0;left:5px;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.right .tooltip-arrow{top:50%;left:0;margin-top:-5px;border-width:5px 5px 5px 0;border-right-color:#000}.tooltip.left .tooltip-arrow{top:50%;right:0;margin-top:-5px;border-width:5px 0 5px 5px;border-left-color:#000}.tooltip.bottom .tooltip-arrow{top:0;left:50%;margin-left:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-left .tooltip-arrow{top:0;right:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-right .tooltip-arrow{top:0;left:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.popover{position:absolute;top:0;left:0;z-index:1060;display:none;max-width:276px;padding:1px;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:14px;font-style:normal;font-weight:400;line-height:1.42857143;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;background-color:#fff;-webkit-background-clip:padding-box;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,.2);box-shadow:0 5px 10px rgba(0,0,0,.2);line-break:auto}.popover.top{margin-top:-10px}.popover.right{margin-left:10px}.popover.bottom{margin-top:10px}.popover.left{margin-left:-10px}.popover-title{padding:8px 14px;margin:0;font-size:14px;background-color:#f7f7f7;border-bottom:1px solid #ebebeb;border-radius:5px 5px 0 0}.popover-content{padding:9px 14px}.popover>.arrow,.popover>.arrow:after{position:absolute;display:block;width:0;height:0;border-color:transparent;border-style:solid}.popover>.arrow{border-width:11px}.popover>.arrow:after{content:"";border-width:10px}.popover.top>.arrow{bottom:-11px;left:50%;margin-left:-11px;border-top-color:#999;border-top-color:rgba(0,0,0,.25);border-bottom-width:0}.popover.top>.arrow:after{bottom:1px;margin-left:-10px;content:" ";border-top-color:#fff;border-bottom-width:0}.popover.right>.arrow{top:50%;left:-11px;margin-top:-11px;border-right-color:#999;border-right-color:rgba(0,0,0,.25);border-left-width:0}.popover.right>.arrow:after{bottom:-10px;left:1px;content:" ";border-right-color:#fff;border-left-width:0}.popover.bottom>.arrow{top:-11px;left:50%;margin-left:-11px;border-top-width:0;border-bottom-color:#999;border-bottom-color:rgba(0,0,0,.25)}.popover.bottom>.arrow:after{top:1px;margin-left:-10px;content:" ";border-top-width:0;border-bottom-color:#fff}.popover.left>.arrow{top:50%;right:-11px;margin-top:-11px;border-right-width:0;border-left-color:#999;border-left-color:rgba(0,0,0,.25)}.popover.left>.arrow:after{right:1px;bottom:-10px;content:" ";border-right-width:0;border-left-color:#fff}.carousel{position:relative}.carousel-inner{position:relative;width:100%;overflow:hidden}.carousel-inner>.item{position:relative;display:none;-webkit-transition:.6s ease-in-out left;-o-transition:.6s ease-in-out left;transition:.6s ease-in-out left}.carousel-inner>.item>a>img,.carousel-inner>.item>img{line-height:1}@media all and (transform-3d),(-webkit-transform-3d){.carousel-inner>.item{-webkit-transition:-webkit-transform .6s ease-in-out;-o-transition:-o-transform .6s ease-in-out;transition:transform .6s ease-in-out;-webkit-backface-visibility:hidden;backface-visibility:hidden;-webkit-perspective:1000px;perspective:1000px}.carousel-inner>.item.active.right,.carousel-inner>.item.next{left:0;-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0)}.carousel-inner>.item.active.left,.carousel-inner>.item.prev{left:0;-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0)}.carousel-inner>.item.active,.carousel-inner>.item.next.left,.carousel-inner>.item.prev.right{left:0;-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0)}}.carousel-inner>.active,.carousel-inner>.next,.carousel-inner>.prev{display:block}.carousel-inner>.active{left:0}.carousel-inner>.next,.carousel-inner>.prev{position:absolute;top:0;width:100%}.carousel-inner>.next{left:100%}.carousel-inner>.prev{left:-100%}.carousel-inner>.next.left,.carousel-inner>.prev.right{left:0}.carousel-inner>.active.left{left:-100%}.carousel-inner>.active.right{left:100%}.carousel-control{position:absolute;top:0;bottom:0;left:0;width:15%;font-size:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6);background-color:rgba(0,0,0,0);filter:alpha(opacity=50);opacity:.5}.carousel-control.left{background-image:-webkit-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.5)),to(rgba(0,0,0,.0001)));background-image:linear-gradient(to right,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);background-repeat:repeat-x}.carousel-control.right{right:0;left:auto;background-image:-webkit-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.0001)),to(rgba(0,0,0,.5)));background-image:linear-gradient(to right,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);background-repeat:repeat-x}.carousel-control:focus,.carousel-control:hover{color:#fff;text-decoration:none;filter:alpha(opacity=90);outline:0;opacity:.9}.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{position:absolute;top:50%;z-index:5;display:inline-block;margin-top:-10px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{left:50%;margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{right:50%;margin-right:-10px}.carousel-control .icon-next,.carousel-control .icon-prev{width:20px;height:20px;font-family:serif;line-height:1}.carousel-control .icon-prev:before{content:'\2039'}.carousel-control .icon-next:before{content:'\203a'}.carousel-indicators{position:absolute;bottom:10px;left:50%;z-index:15;width:60%;padding-left:0;margin-left:-30%;text-align:center;list-style:none}.carousel-indicators li{display:inline-block;width:10px;height:10px;margin:1px;text-indent:-999px;cursor:pointer;background-color:#000\9;background-color:rgba(0,0,0,0);border:1px solid #fff;border-radius:10px}.carousel-indicators .active{width:12px;height:12px;margin:0;background-color:#fff}.carousel-caption{position:absolute;right:15%;bottom:20px;left:15%;z-index:10;padding-top:20px;padding-bottom:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6)}.carousel-caption .btn{text-shadow:none}@media screen and (min-width:768px){.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{width:30px;height:30px;margin-top:-10px;font-size:30px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{margin-right:-10px}.carousel-caption{right:20%;left:20%;padding-bottom:30px}.carousel-indicators{bottom:20px}}.btn-group-vertical>.btn-group:after,.btn-group-vertical>.btn-group:before,.btn-toolbar:after,.btn-toolbar:before,.clearfix:after,.clearfix:before,.container-fluid:after,.container-fluid:before,.container:after,.container:before,.dl-horizontal dd:after,.dl-horizontal dd:before,.form-horizontal .form-group:after,.form-horizontal .form-group:before,.modal-footer:after,.modal-footer:before,.modal-header:after,.modal-header:before,.nav:after,.nav:before,.navbar-collapse:after,.navbar-collapse:before,.navbar-header:after,.navbar-header:before,.navbar:after,.navbar:before,.pager:after,.pager:before,.panel-body:after,.panel-body:before,.row:after,.row:before{display:table;content:" "}.btn-group-vertical>.btn-group:after,.btn-toolbar:after,.clearfix:after,.container-fluid:after,.container:after,.dl-horizontal dd:after,.form-horizontal .form-group:after,.modal-footer:after,.modal-header:after,.nav:after,.navbar-collapse:after,.navbar-header:after,.navbar:after,.pager:after,.panel-body:after,.row:after{clear:both}.center-block{display:block;margin-right:auto;margin-left:auto}.pull-right{float:right!important}.pull-left{float:left!important}.hide{display:none!important}.show{display:block!important}.invisible{visibility:hidden}.text-hide{font:0/0 a;color:transparent;text-shadow:none;background-color:transparent;border:0}.hidden{display:none!important}.affix{position:fixed}@-ms-viewport{width:device-width}.visible-lg,.visible-md,.visible-sm,.visible-xs{display:none!important}.visible-lg-block,.visible-lg-inline,.visible-lg-inline-block,.visible-md-block,.visible-md-inline,.visible-md-inline-block,.visible-sm-block,.visible-sm-inline,.visible-sm-inline-block,.visible-xs-block,.visible-xs-inline,.visible-xs-inline-block{display:none!important}@media (max-width:767px){.visible-xs{display:block!important}table.visible-xs{display:table!important}tr.visible-xs{display:table-row!important}td.visible-xs,th.visible-xs{display:table-cell!important}}@media (max-width:767px){.visible-xs-block{display:block!important}}@media (max-width:767px){.visible-xs-inline{display:inline!important}}@media (max-width:767px){.visible-xs-inline-block{display:inline-block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm{display:block!important}table.visible-sm{display:table!important}tr.visible-sm{display:table-row!important}td.visible-sm,th.visible-sm{display:table-cell!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-block{display:block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline{display:inline!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline-block{display:inline-block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md{display:block!important}table.visible-md{display:table!important}tr.visible-md{display:table-row!important}td.visible-md,th.visible-md{display:table-cell!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-block{display:block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline{display:inline!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline-block{display:inline-block!important}}@media (min-width:1200px){.visible-lg{display:block!important}table.visible-lg{display:table!important}tr.visible-lg{display:table-row!important}td.visible-lg,th.visible-lg{display:table-cell!important}}@media (min-width:1200px){.visible-lg-block{display:block!important}}@media (min-width:1200px){.visible-lg-inline{display:inline!important}}@media (min-width:1200px){.visible-lg-inline-block{display:inline-block!important}}@media (max-width:767px){.hidden-xs{display:none!important}}@media (min-width:768px) and (max-width:991px){.hidden-sm{display:none!important}}@media (min-width:992px) and (max-width:1199px){.hidden-md{display:none!important}}@media (min-width:1200px){.hidden-lg{display:none!important}}.visible-print{display:none!important}@media print{.visible-print{display:block!important}table.visible-print{display:table!important}tr.visible-print{display:table-row!important}td.visible-print,th.visible-print{display:table-cell!important}}.visible-print-block{display:none!important}@media print{.visible-print-block{display:block!important}}.visible-print-inline{display:none!important}@media print{.visible-print-inline{display:inline!important}}.visible-print-inline-block{display:none!important}@media print{.visible-print-inline-block{display:inline-block!important}}@media print{.hidden-print{display:none!important}}
+ *//*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */html{font-family:sans-serif;-ms-text-size-adjust:100%;-webkit-text-size-adjust:100%}body{margin:0}article,aside,details,figcaption,figure,footer,header,hgroup,main,menu,nav,section,summary{display:block}audio,canvas,progress,video{display:inline-block;vertical-align:baseline}audio:not([controls]){display:none;height:0}[hidden],template{display:none}a{background-color:transparent}a:active,a:hover{outline:0}abbr[title]{border-bottom:none;text-decoration:underline;-webkit-text-decoration:underline dotted;-moz-text-decoration:underline dotted;text-decoration:underline dotted}b,strong{font-weight:700}dfn{font-style:italic}h1{font-size:2em;margin:.67em 0}mark{background:#ff0;color:#000}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sup{top:-.5em}sub{bottom:-.25em}img{border:0}svg:not(:root){overflow:hidden}figure{margin:1em 40px}hr{-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;height:0}pre{overflow:auto}code,kbd,pre,samp{font-family:monospace,monospace;font-size:1em}button,input,optgroup,select,textarea{color:inherit;font:inherit;margin:0}button{overflow:visible}button,select{text-transform:none}button,html input[type=button],input[type=reset],input[type=submit]{-webkit-appearance:button;cursor:pointer}button[disabled],html input[disabled]{cursor:default}button::-moz-focus-inner,input::-moz-focus-inner{border:0;padding:0}input{line-height:normal}input[type=checkbox],input[type=radio]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;padding:0}input[type=number]::-webkit-inner-spin-button,input[type=number]::-webkit-outer-spin-button{height:auto}input[type=search]{-webkit-appearance:textfield;-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box}input[type=search]::-webkit-search-cancel-button,input[type=search]::-webkit-search-decoration{-webkit-appearance:none}fieldset{border:1px solid silver;margin:0 2px;padding:.35em .625em .75em}legend{border:0;padding:0}textarea{overflow:auto}optgroup{font-weight:700}table{border-collapse:collapse;border-spacing:0}td,th{padding:0}/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */@media print{*,:after,:before{color:#000!important;text-shadow:none!important;background:0 0!important;-webkit-box-shadow:none!important;box-shadow:none!important}a,a:visited{text-decoration:underline}a[href]:after{content:" (" attr(href) ")"}abbr[title]:after{content:" (" attr(title) ")"}a[href^="#"]:after,a[href^="javascript:"]:after{content:""}blockquote,pre{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}img,tr{page-break-inside:avoid}img{max-width:100%!important}h2,h3,p{orphans:3;widows:3}h2,h3{page-break-after:avoid}.navbar{display:none}.btn>.caret,.dropup>.btn>.caret{border-top-color:#000!important}.label{border:1px solid #000}.table{border-collapse:collapse!important}.table td,.table th{background-color:#fff!important}.table-bordered td,.table-bordered th{border:1px solid #ddd!important}}@font-face{font-family:"Glyphicons Halflings";src:url(../fonts/glyphicons-halflings-regular.eot);src:url(../fonts/glyphicons-halflings-regular.eot?#iefix) format("embedded-opentype"),url(../fonts/glyphicons-halflings-regular.woff2) format("woff2"),url(../fonts/glyphicons-halflings-regular.woff) format("woff"),url(../fonts/glyphicons-halflings-regular.ttf) format("truetype"),url(../fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular) format("svg")}.glyphicon{position:relative;top:1px;display:inline-block;font-family:"Glyphicons Halflings";font-style:normal;font-weight:400;line-height:1;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.glyphicon-asterisk:before{content:"\002a"}.glyphicon-plus:before{content:"\002b"}.glyphicon-eur:before,.glyphicon-euro:before{content:"\20ac"}.glyphicon-minus:before{content:"\2212"}.glyphicon-cloud:before{content:"\2601"}.glyphicon-envelope:before{content:"\2709"}.glyphicon-pencil:before{content:"\270f"}.glyphicon-glass:before{content:"\e001"}.glyphicon-music:before{content:"\e002"}.glyphicon-search:before{content:"\e003"}.glyphicon-heart:before{content:"\e005"}.glyphicon-star:before{content:"\e006"}.glyphicon-star-empty:before{content:"\e007"}.glyphicon-user:before{content:"\e008"}.glyphicon-film:before{content:"\e009"}.glyphicon-th-large:before{content:"\e010"}.glyphicon-th:before{content:"\e011"}.glyphicon-th-list:before{content:"\e012"}.glyphicon-ok:before{content:"\e013"}.glyphicon-remove:before{content:"\e014"}.glyphicon-zoom-in:before{content:"\e015"}.glyphicon-zoom-out:before{content:"\e016"}.glyphicon-off:before{content:"\e017"}.glyphicon-signal:before{content:"\e018"}.glyphicon-cog:before{content:"\e019"}.glyphicon-trash:before{content:"\e020"}.glyphicon-home:before{content:"\e021"}.glyphicon-file:before{content:"\e022"}.glyphicon-time:before{content:"\e023"}.glyphicon-road:before{content:"\e024"}.glyphicon-download-alt:before{content:"\e025"}.glyphicon-download:before{content:"\e026"}.glyphicon-upload:before{content:"\e027"}.glyphicon-inbox:before{content:"\e028"}.glyphicon-play-circle:before{content:"\e029"}.glyphicon-repeat:before{content:"\e030"}.glyphicon-refresh:before{content:"\e031"}.glyphicon-list-alt:before{content:"\e032"}.glyphicon-lock:before{content:"\e033"}.glyphicon-flag:before{content:"\e034"}.glyphicon-headphones:before{content:"\e035"}.glyphicon-volume-off:before{content:"\e036"}.glyphicon-volume-down:before{content:"\e037"}.glyphicon-volume-up:before{content:"\e038"}.glyphicon-qrcode:before{content:"\e039"}.glyphicon-barcode:before{content:"\e040"}.glyphicon-tag:before{content:"\e041"}.glyphicon-tags:before{content:"\e042"}.glyphicon-book:before{content:"\e043"}.glyphicon-bookmark:before{content:"\e044"}.glyphicon-print:before{content:"\e045"}.glyphicon-camera:before{content:"\e046"}.glyphicon-font:before{content:"\e047"}.glyphicon-bold:before{content:"\e048"}.glyphicon-italic:before{content:"\e049"}.glyphicon-text-height:before{content:"\e050"}.glyphicon-text-width:before{content:"\e051"}.glyphicon-align-left:before{content:"\e052"}.glyphicon-align-center:before{content:"\e053"}.glyphicon-align-right:before{content:"\e054"}.glyphicon-align-justify:before{content:"\e055"}.glyphicon-list:before{content:"\e056"}.glyphicon-indent-left:before{content:"\e057"}.glyphicon-indent-right:before{content:"\e058"}.glyphicon-facetime-video:before{content:"\e059"}.glyphicon-picture:before{content:"\e060"}.glyphicon-map-marker:before{content:"\e062"}.glyphicon-adjust:before{content:"\e063"}.glyphicon-tint:before{content:"\e064"}.glyphicon-edit:before{content:"\e065"}.glyphicon-share:before{content:"\e066"}.glyphicon-check:before{content:"\e067"}.glyphicon-move:before{content:"\e068"}.glyphicon-step-backward:before{content:"\e069"}.glyphicon-fast-backward:before{content:"\e070"}.glyphicon-backward:before{content:"\e071"}.glyphicon-play:before{content:"\e072"}.glyphicon-pause:before{content:"\e073"}.glyphicon-stop:before{content:"\e074"}.glyphicon-forward:before{content:"\e075"}.glyphicon-fast-forward:before{content:"\e076"}.glyphicon-step-forward:before{content:"\e077"}.glyphicon-eject:before{content:"\e078"}.glyphicon-chevron-left:before{content:"\e079"}.glyphicon-chevron-right:before{content:"\e080"}.glyphicon-plus-sign:before{content:"\e081"}.glyphicon-minus-sign:before{content:"\e082"}.glyphicon-remove-sign:before{content:"\e083"}.glyphicon-ok-sign:before{content:"\e084"}.glyphicon-question-sign:before{content:"\e085"}.glyphicon-info-sign:before{content:"\e086"}.glyphicon-screenshot:before{content:"\e087"}.glyphicon-remove-circle:before{content:"\e088"}.glyphicon-ok-circle:before{content:"\e089"}.glyphicon-ban-circle:before{content:"\e090"}.glyphicon-arrow-left:before{content:"\e091"}.glyphicon-arrow-right:before{content:"\e092"}.glyphicon-arrow-up:before{content:"\e093"}.glyphicon-arrow-down:before{content:"\e094"}.glyphicon-share-alt:before{content:"\e095"}.glyphicon-resize-full:before{content:"\e096"}.glyphicon-resize-small:before{content:"\e097"}.glyphicon-exclamation-sign:before{content:"\e101"}.glyphicon-gift:before{content:"\e102"}.glyphicon-leaf:before{content:"\e103"}.glyphicon-fire:before{content:"\e104"}.glyphicon-eye-open:before{content:"\e105"}.glyphicon-eye-close:before{content:"\e106"}.glyphicon-warning-sign:before{content:"\e107"}.glyphicon-plane:before{content:"\e108"}.glyphicon-calendar:before{content:"\e109"}.glyphicon-random:before{content:"\e110"}.glyphicon-comment:before{content:"\e111"}.glyphicon-magnet:before{content:"\e112"}.glyphicon-chevron-up:before{content:"\e113"}.glyphicon-chevron-down:before{content:"\e114"}.glyphicon-retweet:before{content:"\e115"}.glyphicon-shopping-cart:before{content:"\e116"}.glyphicon-folder-close:before{content:"\e117"}.glyphicon-folder-open:before{content:"\e118"}.glyphicon-resize-vertical:before{content:"\e119"}.glyphicon-resize-horizontal:before{content:"\e120"}.glyphicon-hdd:before{content:"\e121"}.glyphicon-bullhorn:before{content:"\e122"}.glyphicon-bell:before{content:"\e123"}.glyphicon-certificate:before{content:"\e124"}.glyphicon-thumbs-up:before{content:"\e125"}.glyphicon-thumbs-down:before{content:"\e126"}.glyphicon-hand-right:before{content:"\e127"}.glyphicon-hand-left:before{content:"\e128"}.glyphicon-hand-up:before{content:"\e129"}.glyphicon-hand-down:before{content:"\e130"}.glyphicon-circle-arrow-right:before{content:"\e131"}.glyphicon-circle-arrow-left:before{content:"\e132"}.glyphicon-circle-arrow-up:before{content:"\e133"}.glyphicon-circle-arrow-down:before{content:"\e134"}.glyphicon-globe:before{content:"\e135"}.glyphicon-wrench:before{content:"\e136"}.glyphicon-tasks:before{content:"\e137"}.glyphicon-filter:before{content:"\e138"}.glyphicon-briefcase:before{content:"\e139"}.glyphicon-fullscreen:before{content:"\e140"}.glyphicon-dashboard:before{content:"\e141"}.glyphicon-paperclip:before{content:"\e142"}.glyphicon-heart-empty:before{content:"\e143"}.glyphicon-link:before{content:"\e144"}.glyphicon-phone:before{content:"\e145"}.glyphicon-pushpin:before{content:"\e146"}.glyphicon-usd:before{content:"\e148"}.glyphicon-gbp:before{content:"\e149"}.glyphicon-sort:before{content:"\e150"}.glyphicon-sort-by-alphabet:before{content:"\e151"}.glyphicon-sort-by-alphabet-alt:before{content:"\e152"}.glyphicon-sort-by-order:before{content:"\e153"}.glyphicon-sort-by-order-alt:before{content:"\e154"}.glyphicon-sort-by-attributes:before{content:"\e155"}.glyphicon-sort-by-attributes-alt:before{content:"\e156"}.glyphicon-unchecked:before{content:"\e157"}.glyphicon-expand:before{content:"\e158"}.glyphicon-collapse-down:before{content:"\e159"}.glyphicon-collapse-up:before{content:"\e160"}.glyphicon-log-in:before{content:"\e161"}.glyphicon-flash:before{content:"\e162"}.glyphicon-log-out:before{content:"\e163"}.glyphicon-new-window:before{content:"\e164"}.glyphicon-record:before{content:"\e165"}.glyphicon-save:before{content:"\e166"}.glyphicon-open:before{content:"\e167"}.glyphicon-saved:before{content:"\e168"}.glyphicon-import:before{content:"\e169"}.glyphicon-export:before{content:"\e170"}.glyphicon-send:before{content:"\e171"}.glyphicon-floppy-disk:before{content:"\e172"}.glyphicon-floppy-saved:before{content:"\e173"}.glyphicon-floppy-remove:before{content:"\e174"}.glyphicon-floppy-save:before{content:"\e175"}.glyphicon-floppy-open:before{content:"\e176"}.glyphicon-credit-card:before{content:"\e177"}.glyphicon-transfer:before{content:"\e178"}.glyphicon-cutlery:before{content:"\e179"}.glyphicon-header:before{content:"\e180"}.glyphicon-compressed:before{content:"\e181"}.glyphicon-earphone:before{content:"\e182"}.glyphicon-phone-alt:before{content:"\e183"}.glyphicon-tower:before{content:"\e184"}.glyphicon-stats:before{content:"\e185"}.glyphicon-sd-video:before{content:"\e186"}.glyphicon-hd-video:before{content:"\e187"}.glyphicon-subtitles:before{content:"\e188"}.glyphicon-sound-stereo:before{content:"\e189"}.glyphicon-sound-dolby:before{content:"\e190"}.glyphicon-sound-5-1:before{content:"\e191"}.glyphicon-sound-6-1:before{content:"\e192"}.glyphicon-sound-7-1:before{content:"\e193"}.glyphicon-copyright-mark:before{content:"\e194"}.glyphicon-registration-mark:before{content:"\e195"}.glyphicon-cloud-download:before{content:"\e197"}.glyphicon-cloud-upload:before{content:"\e198"}.glyphicon-tree-conifer:before{content:"\e199"}.glyphicon-tree-deciduous:before{content:"\e200"}.glyphicon-cd:before{content:"\e201"}.glyphicon-save-file:before{content:"\e202"}.glyphicon-open-file:before{content:"\e203"}.glyphicon-level-up:before{content:"\e204"}.glyphicon-copy:before{content:"\e205"}.glyphicon-paste:before{content:"\e206"}.glyphicon-alert:before{content:"\e209"}.glyphicon-equalizer:before{content:"\e210"}.glyphicon-king:before{content:"\e211"}.glyphicon-queen:before{content:"\e212"}.glyphicon-pawn:before{content:"\e213"}.glyphicon-bishop:before{content:"\e214"}.glyphicon-knight:before{content:"\e215"}.glyphicon-baby-formula:before{content:"\e216"}.glyphicon-tent:before{content:"\26fa"}.glyphicon-blackboard:before{content:"\e218"}.glyphicon-bed:before{content:"\e219"}.glyphicon-apple:before{content:"\f8ff"}.glyphicon-erase:before{content:"\e221"}.glyphicon-hourglass:before{content:"\231b"}.glyphicon-lamp:before{content:"\e223"}.glyphicon-duplicate:before{content:"\e224"}.glyphicon-piggy-bank:before{content:"\e225"}.glyphicon-scissors:before{content:"\e226"}.glyphicon-bitcoin:before{content:"\e227"}.glyphicon-btc:before{content:"\e227"}.glyphicon-xbt:before{content:"\e227"}.glyphicon-yen:before{content:"\00a5"}.glyphicon-jpy:before{content:"\00a5"}.glyphicon-ruble:before{content:"\20bd"}.glyphicon-rub:before{content:"\20bd"}.glyphicon-scale:before{content:"\e230"}.glyphicon-ice-lolly:before{content:"\e231"}.glyphicon-ice-lolly-tasted:before{content:"\e232"}.glyphicon-education:before{content:"\e233"}.glyphicon-option-horizontal:before{content:"\e234"}.glyphicon-option-vertical:before{content:"\e235"}.glyphicon-menu-hamburger:before{content:"\e236"}.glyphicon-modal-window:before{content:"\e237"}.glyphicon-oil:before{content:"\e238"}.glyphicon-grain:before{content:"\e239"}.glyphicon-sunglasses:before{content:"\e240"}.glyphicon-text-size:before{content:"\e241"}.glyphicon-text-color:before{content:"\e242"}.glyphicon-text-background:before{content:"\e243"}.glyphicon-object-align-top:before{content:"\e244"}.glyphicon-object-align-bottom:before{content:"\e245"}.glyphicon-object-align-horizontal:before{content:"\e246"}.glyphicon-object-align-left:before{content:"\e247"}.glyphicon-object-align-vertical:before{content:"\e248"}.glyphicon-object-align-right:before{content:"\e249"}.glyphicon-triangle-right:before{content:"\e250"}.glyphicon-triangle-left:before{content:"\e251"}.glyphicon-triangle-bottom:before{content:"\e252"}.glyphicon-triangle-top:before{content:"\e253"}.glyphicon-console:before{content:"\e254"}.glyphicon-superscript:before{content:"\e255"}.glyphicon-subscript:before{content:"\e256"}.glyphicon-menu-left:before{content:"\e257"}.glyphicon-menu-right:before{content:"\e258"}.glyphicon-menu-down:before{content:"\e259"}.glyphicon-menu-up:before{content:"\e260"}*{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}:after,:before{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box}html{font-size:10px;-webkit-tap-highlight-color:rgba(0,0,0,0)}body{font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-size:14px;line-height:1.42857143;color:#333;background-color:#fff}button,input,select,textarea{font-family:inherit;font-size:inherit;line-height:inherit}a{color:#337ab7;text-decoration:none}a:focus,a:hover{color:#23527c;text-decoration:underline}a:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}figure{margin:0}img{vertical-align:middle}.carousel-inner>.item>a>img,.carousel-inner>.item>img,.img-responsive,.thumbnail a>img,.thumbnail>img{display:block;max-width:100%;height:auto}.img-rounded{border-radius:6px}.img-thumbnail{padding:4px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:all .2s ease-in-out;-o-transition:all .2s ease-in-out;transition:all .2s ease-in-out;display:inline-block;max-width:100%;height:auto}.img-circle{border-radius:50%}hr{margin-top:20px;margin-bottom:20px;border:0;border-top:1px solid #eee}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);border:0}.sr-only-focusable:active,.sr-only-focusable:focus{position:static;width:auto;height:auto;margin:0;overflow:visible;clip:auto}[role=button]{cursor:pointer}.h1,.h2,.h3,.h4,.h5,.h6,h1,h2,h3,h4,h5,h6{font-family:inherit;font-weight:500;line-height:1.1;color:inherit}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-weight:400;line-height:1;color:#777}.h1,.h2,.h3,h1,h2,h3{margin-top:20px;margin-bottom:10px}.h1 .small,.h1 small,.h2 .small,.h2 small,.h3 .small,.h3 small,h1 .small,h1 small,h2 .small,h2 small,h3 .small,h3 small{font-size:65%}.h4,.h5,.h6,h4,h5,h6{margin-top:10px;margin-bottom:10px}.h4 .small,.h4 small,.h5 .small,.h5 small,.h6 .small,.h6 small,h4 .small,h4 small,h5 .small,h5 small,h6 .small,h6 small{font-size:75%}.h1,h1{font-size:36px}.h2,h2{font-size:30px}.h3,h3{font-size:24px}.h4,h4{font-size:18px}.h5,h5{font-size:14px}.h6,h6{font-size:12px}p{margin:0 0 10px}.lead{margin-bottom:20px;font-size:16px;font-weight:300;line-height:1.4}@media (min-width:768px){.lead{font-size:21px}}.small,small{font-size:85%}.mark,mark{padding:.2em;background-color:#fcf8e3}.text-left{text-align:left}.text-right{text-align:right}.text-center{text-align:center}.text-justify{text-align:justify}.text-nowrap{white-space:nowrap}.text-lowercase{text-transform:lowercase}.text-uppercase{text-transform:uppercase}.text-capitalize{text-transform:capitalize}.text-muted{color:#777}.text-primary{color:#337ab7}a.text-primary:focus,a.text-primary:hover{color:#286090}.text-success{color:#3c763d}a.text-success:focus,a.text-success:hover{color:#2b542c}.text-info{color:#31708f}a.text-info:focus,a.text-info:hover{color:#245269}.text-warning{color:#8a6d3b}a.text-warning:focus,a.text-warning:hover{color:#66512c}.text-danger{color:#a94442}a.text-danger:focus,a.text-danger:hover{color:#843534}.bg-primary{color:#fff;background-color:#337ab7}a.bg-primary:focus,a.bg-primary:hover{background-color:#286090}.bg-success{background-color:#dff0d8}a.bg-success:focus,a.bg-success:hover{background-color:#c1e2b3}.bg-info{background-color:#d9edf7}a.bg-info:focus,a.bg-info:hover{background-color:#afd9ee}.bg-warning{background-color:#fcf8e3}a.bg-warning:focus,a.bg-warning:hover{background-color:#f7ecb5}.bg-danger{background-color:#f2dede}a.bg-danger:focus,a.bg-danger:hover{background-color:#e4b9b9}.page-header{padding-bottom:9px;margin:40px 0 20px;border-bottom:1px solid #eee}ol,ul{margin-top:0;margin-bottom:10px}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}.list-unstyled{padding-left:0;list-style:none}.list-inline{padding-left:0;list-style:none;margin-left:-5px}.list-inline>li{display:inline-block;padding-right:5px;padding-left:5px}dl{margin-top:0;margin-bottom:20px}dd,dt{line-height:1.42857143}dt{font-weight:700}dd{margin-left:0}@media (min-width:768px){.dl-horizontal dt{float:left;width:160px;clear:left;text-align:right;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.dl-horizontal dd{margin-left:180px}}abbr[data-original-title],abbr[title]{cursor:help}.initialism{font-size:90%;text-transform:uppercase}blockquote{padding:10px 20px;margin:0 0 20px;font-size:17.5px;border-left:5px solid #eee}blockquote ol:last-child,blockquote p:last-child,blockquote ul:last-child{margin-bottom:0}blockquote .small,blockquote footer,blockquote small{display:block;font-size:80%;line-height:1.42857143;color:#777}blockquote .small:before,blockquote footer:before,blockquote small:before{content:"\2014 \00A0"}.blockquote-reverse,blockquote.pull-right{padding-right:15px;padding-left:0;text-align:right;border-right:5px solid #eee;border-left:0}.blockquote-reverse .small:before,.blockquote-reverse footer:before,.blockquote-reverse small:before,blockquote.pull-right .small:before,blockquote.pull-right footer:before,blockquote.pull-right small:before{content:""}.blockquote-reverse .small:after,.blockquote-reverse footer:after,.blockquote-reverse small:after,blockquote.pull-right .small:after,blockquote.pull-right footer:after,blockquote.pull-right small:after{content:"\00A0 \2014"}address{margin-bottom:20px;font-style:normal;line-height:1.42857143}code,kbd,pre,samp{font-family:Menlo,Monaco,Consolas,"Courier New",monospace}code{padding:2px 4px;font-size:90%;color:#c7254e;background-color:#f9f2f4;border-radius:4px}kbd{padding:2px 4px;font-size:90%;color:#fff;background-color:#333;border-radius:3px;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.25);box-shadow:inset 0 -1px 0 rgba(0,0,0,.25)}kbd kbd{padding:0;font-size:100%;font-weight:700;-webkit-box-shadow:none;box-shadow:none}pre{display:block;padding:9.5px;margin:0 0 10px;font-size:13px;line-height:1.42857143;color:#333;word-break:break-all;word-wrap:break-word;background-color:#f5f5f5;border:1px solid #ccc;border-radius:4px}pre code{padding:0;font-size:inherit;color:inherit;white-space:pre-wrap;background-color:transparent;border-radius:0}.pre-scrollable{max-height:340px;overflow-y:scroll}.container{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}@media (min-width:768px){.container{width:750px}}@media (min-width:992px){.container{width:970px}}@media (min-width:1200px){.container{width:1170px}}.container-fluid{padding-right:15px;padding-left:15px;margin-right:auto;margin-left:auto}.row{margin-right:-15px;margin-left:-15px}.row-no-gutters{margin-right:0;margin-left:0}.row-no-gutters [class*=col-]{padding-right:0;padding-left:0}.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9,.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9,.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9,.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{position:relative;min-height:1px;padding-right:15px;padding-left:15px}.col-xs-1,.col-xs-10,.col-xs-11,.col-xs-12,.col-xs-2,.col-xs-3,.col-xs-4,.col-xs-5,.col-xs-6,.col-xs-7,.col-xs-8,.col-xs-9{float:left}.col-xs-12{width:100%}.col-xs-11{width:91.66666667%}.col-xs-10{width:83.33333333%}.col-xs-9{width:75%}.col-xs-8{width:66.66666667%}.col-xs-7{width:58.33333333%}.col-xs-6{width:50%}.col-xs-5{width:41.66666667%}.col-xs-4{width:33.33333333%}.col-xs-3{width:25%}.col-xs-2{width:16.66666667%}.col-xs-1{width:8.33333333%}.col-xs-pull-12{right:100%}.col-xs-pull-11{right:91.66666667%}.col-xs-pull-10{right:83.33333333%}.col-xs-pull-9{right:75%}.col-xs-pull-8{right:66.66666667%}.col-xs-pull-7{right:58.33333333%}.col-xs-pull-6{right:50%}.col-xs-pull-5{right:41.66666667%}.col-xs-pull-4{right:33.33333333%}.col-xs-pull-3{right:25%}.col-xs-pull-2{right:16.66666667%}.col-xs-pull-1{right:8.33333333%}.col-xs-pull-0{right:auto}.col-xs-push-12{left:100%}.col-xs-push-11{left:91.66666667%}.col-xs-push-10{left:83.33333333%}.col-xs-push-9{left:75%}.col-xs-push-8{left:66.66666667%}.col-xs-push-7{left:58.33333333%}.col-xs-push-6{left:50%}.col-xs-push-5{left:41.66666667%}.col-xs-push-4{left:33.33333333%}.col-xs-push-3{left:25%}.col-xs-push-2{left:16.66666667%}.col-xs-push-1{left:8.33333333%}.col-xs-push-0{left:auto}.col-xs-offset-12{margin-left:100%}.col-xs-offset-11{margin-left:91.66666667%}.col-xs-offset-10{margin-left:83.33333333%}.col-xs-offset-9{margin-left:75%}.col-xs-offset-8{margin-left:66.66666667%}.col-xs-offset-7{margin-left:58.33333333%}.col-xs-offset-6{margin-left:50%}.col-xs-offset-5{margin-left:41.66666667%}.col-xs-offset-4{margin-left:33.33333333%}.col-xs-offset-3{margin-left:25%}.col-xs-offset-2{margin-left:16.66666667%}.col-xs-offset-1{margin-left:8.33333333%}.col-xs-offset-0{margin-left:0}@media (min-width:768px){.col-sm-1,.col-sm-10,.col-sm-11,.col-sm-12,.col-sm-2,.col-sm-3,.col-sm-4,.col-sm-5,.col-sm-6,.col-sm-7,.col-sm-8,.col-sm-9{float:left}.col-sm-12{width:100%}.col-sm-11{width:91.66666667%}.col-sm-10{width:83.33333333%}.col-sm-9{width:75%}.col-sm-8{width:66.66666667%}.col-sm-7{width:58.33333333%}.col-sm-6{width:50%}.col-sm-5{width:41.66666667%}.col-sm-4{width:33.33333333%}.col-sm-3{width:25%}.col-sm-2{width:16.66666667%}.col-sm-1{width:8.33333333%}.col-sm-pull-12{right:100%}.col-sm-pull-11{right:91.66666667%}.col-sm-pull-10{right:83.33333333%}.col-sm-pull-9{right:75%}.col-sm-pull-8{right:66.66666667%}.col-sm-pull-7{right:58.33333333%}.col-sm-pull-6{right:50%}.col-sm-pull-5{right:41.66666667%}.col-sm-pull-4{right:33.33333333%}.col-sm-pull-3{right:25%}.col-sm-pull-2{right:16.66666667%}.col-sm-pull-1{right:8.33333333%}.col-sm-pull-0{right:auto}.col-sm-push-12{left:100%}.col-sm-push-11{left:91.66666667%}.col-sm-push-10{left:83.33333333%}.col-sm-push-9{left:75%}.col-sm-push-8{left:66.66666667%}.col-sm-push-7{left:58.33333333%}.col-sm-push-6{left:50%}.col-sm-push-5{left:41.66666667%}.col-sm-push-4{left:33.33333333%}.col-sm-push-3{left:25%}.col-sm-push-2{left:16.66666667%}.col-sm-push-1{left:8.33333333%}.col-sm-push-0{left:auto}.col-sm-offset-12{margin-left:100%}.col-sm-offset-11{margin-left:91.66666667%}.col-sm-offset-10{margin-left:83.33333333%}.col-sm-offset-9{margin-left:75%}.col-sm-offset-8{margin-left:66.66666667%}.col-sm-offset-7{margin-left:58.33333333%}.col-sm-offset-6{margin-left:50%}.col-sm-offset-5{margin-left:41.66666667%}.col-sm-offset-4{margin-left:33.33333333%}.col-sm-offset-3{margin-left:25%}.col-sm-offset-2{margin-left:16.66666667%}.col-sm-offset-1{margin-left:8.33333333%}.col-sm-offset-0{margin-left:0}}@media (min-width:992px){.col-md-1,.col-md-10,.col-md-11,.col-md-12,.col-md-2,.col-md-3,.col-md-4,.col-md-5,.col-md-6,.col-md-7,.col-md-8,.col-md-9{float:left}.col-md-12{width:100%}.col-md-11{width:91.66666667%}.col-md-10{width:83.33333333%}.col-md-9{width:75%}.col-md-8{width:66.66666667%}.col-md-7{width:58.33333333%}.col-md-6{width:50%}.col-md-5{width:41.66666667%}.col-md-4{width:33.33333333%}.col-md-3{width:25%}.col-md-2{width:16.66666667%}.col-md-1{width:8.33333333%}.col-md-pull-12{right:100%}.col-md-pull-11{right:91.66666667%}.col-md-pull-10{right:83.33333333%}.col-md-pull-9{right:75%}.col-md-pull-8{right:66.66666667%}.col-md-pull-7{right:58.33333333%}.col-md-pull-6{right:50%}.col-md-pull-5{right:41.66666667%}.col-md-pull-4{right:33.33333333%}.col-md-pull-3{right:25%}.col-md-pull-2{right:16.66666667%}.col-md-pull-1{right:8.33333333%}.col-md-pull-0{right:auto}.col-md-push-12{left:100%}.col-md-push-11{left:91.66666667%}.col-md-push-10{left:83.33333333%}.col-md-push-9{left:75%}.col-md-push-8{left:66.66666667%}.col-md-push-7{left:58.33333333%}.col-md-push-6{left:50%}.col-md-push-5{left:41.66666667%}.col-md-push-4{left:33.33333333%}.col-md-push-3{left:25%}.col-md-push-2{left:16.66666667%}.col-md-push-1{left:8.33333333%}.col-md-push-0{left:auto}.col-md-offset-12{margin-left:100%}.col-md-offset-11{margin-left:91.66666667%}.col-md-offset-10{margin-left:83.33333333%}.col-md-offset-9{margin-left:75%}.col-md-offset-8{margin-left:66.66666667%}.col-md-offset-7{margin-left:58.33333333%}.col-md-offset-6{margin-left:50%}.col-md-offset-5{margin-left:41.66666667%}.col-md-offset-4{margin-left:33.33333333%}.col-md-offset-3{margin-left:25%}.col-md-offset-2{margin-left:16.66666667%}.col-md-offset-1{margin-left:8.33333333%}.col-md-offset-0{margin-left:0}}@media (min-width:1200px){.col-lg-1,.col-lg-10,.col-lg-11,.col-lg-12,.col-lg-2,.col-lg-3,.col-lg-4,.col-lg-5,.col-lg-6,.col-lg-7,.col-lg-8,.col-lg-9{float:left}.col-lg-12{width:100%}.col-lg-11{width:91.66666667%}.col-lg-10{width:83.33333333%}.col-lg-9{width:75%}.col-lg-8{width:66.66666667%}.col-lg-7{width:58.33333333%}.col-lg-6{width:50%}.col-lg-5{width:41.66666667%}.col-lg-4{width:33.33333333%}.col-lg-3{width:25%}.col-lg-2{width:16.66666667%}.col-lg-1{width:8.33333333%}.col-lg-pull-12{right:100%}.col-lg-pull-11{right:91.66666667%}.col-lg-pull-10{right:83.33333333%}.col-lg-pull-9{right:75%}.col-lg-pull-8{right:66.66666667%}.col-lg-pull-7{right:58.33333333%}.col-lg-pull-6{right:50%}.col-lg-pull-5{right:41.66666667%}.col-lg-pull-4{right:33.33333333%}.col-lg-pull-3{right:25%}.col-lg-pull-2{right:16.66666667%}.col-lg-pull-1{right:8.33333333%}.col-lg-pull-0{right:auto}.col-lg-push-12{left:100%}.col-lg-push-11{left:91.66666667%}.col-lg-push-10{left:83.33333333%}.col-lg-push-9{left:75%}.col-lg-push-8{left:66.66666667%}.col-lg-push-7{left:58.33333333%}.col-lg-push-6{left:50%}.col-lg-push-5{left:41.66666667%}.col-lg-push-4{left:33.33333333%}.col-lg-push-3{left:25%}.col-lg-push-2{left:16.66666667%}.col-lg-push-1{left:8.33333333%}.col-lg-push-0{left:auto}.col-lg-offset-12{margin-left:100%}.col-lg-offset-11{margin-left:91.66666667%}.col-lg-offset-10{margin-left:83.33333333%}.col-lg-offset-9{margin-left:75%}.col-lg-offset-8{margin-left:66.66666667%}.col-lg-offset-7{margin-left:58.33333333%}.col-lg-offset-6{margin-left:50%}.col-lg-offset-5{margin-left:41.66666667%}.col-lg-offset-4{margin-left:33.33333333%}.col-lg-offset-3{margin-left:25%}.col-lg-offset-2{margin-left:16.66666667%}.col-lg-offset-1{margin-left:8.33333333%}.col-lg-offset-0{margin-left:0}}table{background-color:transparent}table col[class*=col-]{position:static;display:table-column;float:none}table td[class*=col-],table th[class*=col-]{position:static;display:table-cell;float:none}caption{padding-top:8px;padding-bottom:8px;color:#777;text-align:left}th{text-align:left}.table{width:100%;max-width:100%;margin-bottom:20px}.table>tbody>tr>td,.table>tbody>tr>th,.table>tfoot>tr>td,.table>tfoot>tr>th,.table>thead>tr>td,.table>thead>tr>th{padding:8px;line-height:1.42857143;vertical-align:top;border-top:1px solid #ddd}.table>thead>tr>th{vertical-align:bottom;border-bottom:2px solid #ddd}.table>caption+thead>tr:first-child>td,.table>caption+thead>tr:first-child>th,.table>colgroup+thead>tr:first-child>td,.table>colgroup+thead>tr:first-child>th,.table>thead:first-child>tr:first-child>td,.table>thead:first-child>tr:first-child>th{border-top:0}.table>tbody+tbody{border-top:2px solid #ddd}.table .table{background-color:#fff}.table-condensed>tbody>tr>td,.table-condensed>tbody>tr>th,.table-condensed>tfoot>tr>td,.table-condensed>tfoot>tr>th,.table-condensed>thead>tr>td,.table-condensed>thead>tr>th{padding:5px}.table-bordered{border:1px solid #ddd}.table-bordered>tbody>tr>td,.table-bordered>tbody>tr>th,.table-bordered>tfoot>tr>td,.table-bordered>tfoot>tr>th,.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border:1px solid #ddd}.table-bordered>thead>tr>td,.table-bordered>thead>tr>th{border-bottom-width:2px}.table-striped>tbody>tr:nth-of-type(odd){background-color:#f9f9f9}.table-hover>tbody>tr:hover{background-color:#f5f5f5}.table>tbody>tr.active>td,.table>tbody>tr.active>th,.table>tbody>tr>td.active,.table>tbody>tr>th.active,.table>tfoot>tr.active>td,.table>tfoot>tr.active>th,.table>tfoot>tr>td.active,.table>tfoot>tr>th.active,.table>thead>tr.active>td,.table>thead>tr.active>th,.table>thead>tr>td.active,.table>thead>tr>th.active{background-color:#f5f5f5}.table-hover>tbody>tr.active:hover>td,.table-hover>tbody>tr.active:hover>th,.table-hover>tbody>tr:hover>.active,.table-hover>tbody>tr>td.active:hover,.table-hover>tbody>tr>th.active:hover{background-color:#e8e8e8}.table>tbody>tr.success>td,.table>tbody>tr.success>th,.table>tbody>tr>td.success,.table>tbody>tr>th.success,.table>tfoot>tr.success>td,.table>tfoot>tr.success>th,.table>tfoot>tr>td.success,.table>tfoot>tr>th.success,.table>thead>tr.success>td,.table>thead>tr.success>th,.table>thead>tr>td.success,.table>thead>tr>th.success{background-color:#dff0d8}.table-hover>tbody>tr.success:hover>td,.table-hover>tbody>tr.success:hover>th,.table-hover>tbody>tr:hover>.success,.table-hover>tbody>tr>td.success:hover,.table-hover>tbody>tr>th.success:hover{background-color:#d0e9c6}.table>tbody>tr.info>td,.table>tbody>tr.info>th,.table>tbody>tr>td.info,.table>tbody>tr>th.info,.table>tfoot>tr.info>td,.table>tfoot>tr.info>th,.table>tfoot>tr>td.info,.table>tfoot>tr>th.info,.table>thead>tr.info>td,.table>thead>tr.info>th,.table>thead>tr>td.info,.table>thead>tr>th.info{background-color:#d9edf7}.table-hover>tbody>tr.info:hover>td,.table-hover>tbody>tr.info:hover>th,.table-hover>tbody>tr:hover>.info,.table-hover>tbody>tr>td.info:hover,.table-hover>tbody>tr>th.info:hover{background-color:#c4e3f3}.table>tbody>tr.warning>td,.table>tbody>tr.warning>th,.table>tbody>tr>td.warning,.table>tbody>tr>th.warning,.table>tfoot>tr.warning>td,.table>tfoot>tr.warning>th,.table>tfoot>tr>td.warning,.table>tfoot>tr>th.warning,.table>thead>tr.warning>td,.table>thead>tr.warning>th,.table>thead>tr>td.warning,.table>thead>tr>th.warning{background-color:#fcf8e3}.table-hover>tbody>tr.warning:hover>td,.table-hover>tbody>tr.warning:hover>th,.table-hover>tbody>tr:hover>.warning,.table-hover>tbody>tr>td.warning:hover,.table-hover>tbody>tr>th.warning:hover{background-color:#faf2cc}.table>tbody>tr.danger>td,.table>tbody>tr.danger>th,.table>tbody>tr>td.danger,.table>tbody>tr>th.danger,.table>tfoot>tr.danger>td,.table>tfoot>tr.danger>th,.table>tfoot>tr>td.danger,.table>tfoot>tr>th.danger,.table>thead>tr.danger>td,.table>thead>tr.danger>th,.table>thead>tr>td.danger,.table>thead>tr>th.danger{background-color:#f2dede}.table-hover>tbody>tr.danger:hover>td,.table-hover>tbody>tr.danger:hover>th,.table-hover>tbody>tr:hover>.danger,.table-hover>tbody>tr>td.danger:hover,.table-hover>tbody>tr>th.danger:hover{background-color:#ebcccc}.table-responsive{min-height:.01%;overflow-x:auto}@media screen and (max-width:767px){.table-responsive{width:100%;margin-bottom:15px;overflow-y:hidden;-ms-overflow-style:-ms-autohiding-scrollbar;border:1px solid #ddd}.table-responsive>.table{margin-bottom:0}.table-responsive>.table>tbody>tr>td,.table-responsive>.table>tbody>tr>th,.table-responsive>.table>tfoot>tr>td,.table-responsive>.table>tfoot>tr>th,.table-responsive>.table>thead>tr>td,.table-responsive>.table>thead>tr>th{white-space:nowrap}.table-responsive>.table-bordered{border:0}.table-responsive>.table-bordered>tbody>tr>td:first-child,.table-responsive>.table-bordered>tbody>tr>th:first-child,.table-responsive>.table-bordered>tfoot>tr>td:first-child,.table-responsive>.table-bordered>tfoot>tr>th:first-child,.table-responsive>.table-bordered>thead>tr>td:first-child,.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.table-responsive>.table-bordered>tbody>tr>td:last-child,.table-responsive>.table-bordered>tbody>tr>th:last-child,.table-responsive>.table-bordered>tfoot>tr>td:last-child,.table-responsive>.table-bordered>tfoot>tr>th:last-child,.table-responsive>.table-bordered>thead>tr>td:last-child,.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.table-responsive>.table-bordered>tbody>tr:last-child>td,.table-responsive>.table-bordered>tbody>tr:last-child>th,.table-responsive>.table-bordered>tfoot>tr:last-child>td,.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}}fieldset{min-width:0;padding:0;margin:0;border:0}legend{display:block;width:100%;padding:0;margin-bottom:20px;font-size:21px;line-height:inherit;color:#333;border:0;border-bottom:1px solid #e5e5e5}label{display:inline-block;max-width:100%;margin-bottom:5px;font-weight:700}input[type=search]{-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;-webkit-appearance:none;-moz-appearance:none;appearance:none}input[type=checkbox],input[type=radio]{margin:4px 0 0;margin-top:1px\9;line-height:normal}fieldset[disabled] input[type=checkbox],fieldset[disabled] input[type=radio],input[type=checkbox].disabled,input[type=checkbox][disabled],input[type=radio].disabled,input[type=radio][disabled]{cursor:not-allowed}input[type=file]{display:block}input[type=range]{display:block;width:100%}select[multiple],select[size]{height:auto}input[type=checkbox]:focus,input[type=file]:focus,input[type=radio]:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}output{display:block;padding-top:7px;font-size:14px;line-height:1.42857143;color:#555}.form-control{display:block;width:100%;height:34px;padding:6px 12px;font-size:14px;line-height:1.42857143;color:#555;background-color:#fff;background-image:none;border:1px solid #ccc;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075);-webkit-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;-o-transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;-webkit-transition:border-color ease-in-out .15s,-webkit-box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,-webkit-box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s;transition:border-color ease-in-out .15s,box-shadow ease-in-out .15s,-webkit-box-shadow ease-in-out .15s}.form-control:focus{border-color:#66afe9;outline:0;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6);box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 8px rgba(102,175,233,.6)}.form-control::-moz-placeholder{color:#999;opacity:1}.form-control:-ms-input-placeholder{color:#999}.form-control::-webkit-input-placeholder{color:#999}.form-control::-ms-expand{background-color:transparent;border:0}.form-control[disabled],.form-control[readonly],fieldset[disabled] .form-control{background-color:#eee;opacity:1}.form-control[disabled],fieldset[disabled] .form-control{cursor:not-allowed}textarea.form-control{height:auto}@media screen and (-webkit-min-device-pixel-ratio:0){input[type=date].form-control,input[type=datetime-local].form-control,input[type=month].form-control,input[type=time].form-control{line-height:34px}.input-group-sm input[type=date],.input-group-sm input[type=datetime-local],.input-group-sm input[type=month],.input-group-sm input[type=time],input[type=date].input-sm,input[type=datetime-local].input-sm,input[type=month].input-sm,input[type=time].input-sm{line-height:30px}.input-group-lg input[type=date],.input-group-lg input[type=datetime-local],.input-group-lg input[type=month],.input-group-lg input[type=time],input[type=date].input-lg,input[type=datetime-local].input-lg,input[type=month].input-lg,input[type=time].input-lg{line-height:46px}}.form-group{margin-bottom:15px}.checkbox,.radio{position:relative;display:block;margin-top:10px;margin-bottom:10px}.checkbox.disabled label,.radio.disabled label,fieldset[disabled] .checkbox label,fieldset[disabled] .radio label{cursor:not-allowed}.checkbox label,.radio label{min-height:20px;padding-left:20px;margin-bottom:0;font-weight:400;cursor:pointer}.checkbox input[type=checkbox],.checkbox-inline input[type=checkbox],.radio input[type=radio],.radio-inline input[type=radio]{position:absolute;margin-top:4px\9;margin-left:-20px}.checkbox+.checkbox,.radio+.radio{margin-top:-5px}.checkbox-inline,.radio-inline{position:relative;display:inline-block;padding-left:20px;margin-bottom:0;font-weight:400;vertical-align:middle;cursor:pointer}.checkbox-inline.disabled,.radio-inline.disabled,fieldset[disabled] .checkbox-inline,fieldset[disabled] .radio-inline{cursor:not-allowed}.checkbox-inline+.checkbox-inline,.radio-inline+.radio-inline{margin-top:0;margin-left:10px}.form-control-static{min-height:34px;padding-top:7px;padding-bottom:7px;margin-bottom:0}.form-control-static.input-lg,.form-control-static.input-sm{padding-right:0;padding-left:0}.input-sm{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-sm{height:30px;line-height:30px}select[multiple].input-sm,textarea.input-sm{height:auto}.form-group-sm .form-control{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.form-group-sm select.form-control{height:30px;line-height:30px}.form-group-sm select[multiple].form-control,.form-group-sm textarea.form-control{height:auto}.form-group-sm .form-control-static{height:30px;min-height:32px;padding:6px 10px;font-size:12px;line-height:1.5}.input-lg{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-lg{height:46px;line-height:46px}select[multiple].input-lg,textarea.input-lg{height:auto}.form-group-lg .form-control{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.form-group-lg select.form-control{height:46px;line-height:46px}.form-group-lg select[multiple].form-control,.form-group-lg textarea.form-control{height:auto}.form-group-lg .form-control-static{height:46px;min-height:38px;padding:11px 16px;font-size:18px;line-height:1.3333333}.has-feedback{position:relative}.has-feedback .form-control{padding-right:42.5px}.form-control-feedback{position:absolute;top:0;right:0;z-index:2;display:block;width:34px;height:34px;line-height:34px;text-align:center;pointer-events:none}.form-group-lg .form-control+.form-control-feedback,.input-group-lg+.form-control-feedback,.input-lg+.form-control-feedback{width:46px;height:46px;line-height:46px}.form-group-sm .form-control+.form-control-feedback,.input-group-sm+.form-control-feedback,.input-sm+.form-control-feedback{width:30px;height:30px;line-height:30px}.has-success .checkbox,.has-success .checkbox-inline,.has-success .control-label,.has-success .help-block,.has-success .radio,.has-success .radio-inline,.has-success.checkbox label,.has-success.checkbox-inline label,.has-success.radio label,.has-success.radio-inline label{color:#3c763d}.has-success .form-control{border-color:#3c763d;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-success .form-control:focus{border-color:#2b542c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #67b168}.has-success .input-group-addon{color:#3c763d;background-color:#dff0d8;border-color:#3c763d}.has-success .form-control-feedback{color:#3c763d}.has-warning .checkbox,.has-warning .checkbox-inline,.has-warning .control-label,.has-warning .help-block,.has-warning .radio,.has-warning .radio-inline,.has-warning.checkbox label,.has-warning.checkbox-inline label,.has-warning.radio label,.has-warning.radio-inline label{color:#8a6d3b}.has-warning .form-control{border-color:#8a6d3b;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-warning .form-control:focus{border-color:#66512c;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #c0a16b}.has-warning .input-group-addon{color:#8a6d3b;background-color:#fcf8e3;border-color:#8a6d3b}.has-warning .form-control-feedback{color:#8a6d3b}.has-error .checkbox,.has-error .checkbox-inline,.has-error .control-label,.has-error .help-block,.has-error .radio,.has-error .radio-inline,.has-error.checkbox label,.has-error.checkbox-inline label,.has-error.radio label,.has-error.radio-inline label{color:#a94442}.has-error .form-control{border-color:#a94442;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075);box-shadow:inset 0 1px 1px rgba(0,0,0,.075)}.has-error .form-control:focus{border-color:#843534;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483;box-shadow:inset 0 1px 1px rgba(0,0,0,.075),0 0 6px #ce8483}.has-error .input-group-addon{color:#a94442;background-color:#f2dede;border-color:#a94442}.has-error .form-control-feedback{color:#a94442}.has-feedback label~.form-control-feedback{top:25px}.has-feedback label.sr-only~.form-control-feedback{top:0}.help-block{display:block;margin-top:5px;margin-bottom:10px;color:#737373}@media (min-width:768px){.form-inline .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.form-inline .form-control{display:inline-block;width:auto;vertical-align:middle}.form-inline .form-control-static{display:inline-block}.form-inline .input-group{display:inline-table;vertical-align:middle}.form-inline .input-group .form-control,.form-inline .input-group .input-group-addon,.form-inline .input-group .input-group-btn{width:auto}.form-inline .input-group>.form-control{width:100%}.form-inline .control-label{margin-bottom:0;vertical-align:middle}.form-inline .checkbox,.form-inline .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.form-inline .checkbox label,.form-inline .radio label{padding-left:0}.form-inline .checkbox input[type=checkbox],.form-inline .radio input[type=radio]{position:relative;margin-left:0}.form-inline .has-feedback .form-control-feedback{top:0}}.form-horizontal .checkbox,.form-horizontal .checkbox-inline,.form-horizontal .radio,.form-horizontal .radio-inline{padding-top:7px;margin-top:0;margin-bottom:0}.form-horizontal .checkbox,.form-horizontal .radio{min-height:27px}.form-horizontal .form-group{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.form-horizontal .control-label{padding-top:7px;margin-bottom:0;text-align:right}}.form-horizontal .has-feedback .form-control-feedback{right:15px}@media (min-width:768px){.form-horizontal .form-group-lg .control-label{padding-top:11px;font-size:18px}}@media (min-width:768px){.form-horizontal .form-group-sm .control-label{padding-top:6px;font-size:12px}}.btn{display:inline-block;margin-bottom:0;font-weight:400;text-align:center;white-space:nowrap;vertical-align:middle;-ms-touch-action:manipulation;touch-action:manipulation;cursor:pointer;background-image:none;border:1px solid transparent;padding:6px 12px;font-size:14px;line-height:1.42857143;border-radius:4px;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.btn.active.focus,.btn.active:focus,.btn.focus,.btn:active.focus,.btn:active:focus,.btn:focus{outline:5px auto -webkit-focus-ring-color;outline-offset:-2px}.btn.focus,.btn:focus,.btn:hover{color:#333;text-decoration:none}.btn.active,.btn:active{background-image:none;outline:0;-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn.disabled,.btn[disabled],fieldset[disabled] .btn{cursor:not-allowed;filter:alpha(opacity=65);opacity:.65;-webkit-box-shadow:none;box-shadow:none}a.btn.disabled,fieldset[disabled] a.btn{pointer-events:none}.btn-default{color:#333;background-color:#fff;border-color:#ccc}.btn-default.focus,.btn-default:focus{color:#333;background-color:#e6e6e6;border-color:#8c8c8c}.btn-default:hover{color:#333;background-color:#e6e6e6;border-color:#adadad}.btn-default.active,.btn-default:active,.open>.dropdown-toggle.btn-default{color:#333;background-color:#e6e6e6;background-image:none;border-color:#adadad}.btn-default.active.focus,.btn-default.active:focus,.btn-default.active:hover,.btn-default:active.focus,.btn-default:active:focus,.btn-default:active:hover,.open>.dropdown-toggle.btn-default.focus,.open>.dropdown-toggle.btn-default:focus,.open>.dropdown-toggle.btn-default:hover{color:#333;background-color:#d4d4d4;border-color:#8c8c8c}.btn-default.disabled.focus,.btn-default.disabled:focus,.btn-default.disabled:hover,.btn-default[disabled].focus,.btn-default[disabled]:focus,.btn-default[disabled]:hover,fieldset[disabled] .btn-default.focus,fieldset[disabled] .btn-default:focus,fieldset[disabled] .btn-default:hover{background-color:#fff;border-color:#ccc}.btn-default .badge{color:#fff;background-color:#333}.btn-primary{color:#fff;background-color:#337ab7;border-color:#2e6da4}.btn-primary.focus,.btn-primary:focus{color:#fff;background-color:#286090;border-color:#122b40}.btn-primary:hover{color:#fff;background-color:#286090;border-color:#204d74}.btn-primary.active,.btn-primary:active,.open>.dropdown-toggle.btn-primary{color:#fff;background-color:#286090;background-image:none;border-color:#204d74}.btn-primary.active.focus,.btn-primary.active:focus,.btn-primary.active:hover,.btn-primary:active.focus,.btn-primary:active:focus,.btn-primary:active:hover,.open>.dropdown-toggle.btn-primary.focus,.open>.dropdown-toggle.btn-primary:focus,.open>.dropdown-toggle.btn-primary:hover{color:#fff;background-color:#204d74;border-color:#122b40}.btn-primary.disabled.focus,.btn-primary.disabled:focus,.btn-primary.disabled:hover,.btn-primary[disabled].focus,.btn-primary[disabled]:focus,.btn-primary[disabled]:hover,fieldset[disabled] .btn-primary.focus,fieldset[disabled] .btn-primary:focus,fieldset[disabled] .btn-primary:hover{background-color:#337ab7;border-color:#2e6da4}.btn-primary .badge{color:#337ab7;background-color:#fff}.btn-success{color:#fff;background-color:#5cb85c;border-color:#4cae4c}.btn-success.focus,.btn-success:focus{color:#fff;background-color:#449d44;border-color:#255625}.btn-success:hover{color:#fff;background-color:#449d44;border-color:#398439}.btn-success.active,.btn-success:active,.open>.dropdown-toggle.btn-success{color:#fff;background-color:#449d44;background-image:none;border-color:#398439}.btn-success.active.focus,.btn-success.active:focus,.btn-success.active:hover,.btn-success:active.focus,.btn-success:active:focus,.btn-success:active:hover,.open>.dropdown-toggle.btn-success.focus,.open>.dropdown-toggle.btn-success:focus,.open>.dropdown-toggle.btn-success:hover{color:#fff;background-color:#398439;border-color:#255625}.btn-success.disabled.focus,.btn-success.disabled:focus,.btn-success.disabled:hover,.btn-success[disabled].focus,.btn-success[disabled]:focus,.btn-success[disabled]:hover,fieldset[disabled] .btn-success.focus,fieldset[disabled] .btn-success:focus,fieldset[disabled] .btn-success:hover{background-color:#5cb85c;border-color:#4cae4c}.btn-success .badge{color:#5cb85c;background-color:#fff}.btn-info{color:#fff;background-color:#5bc0de;border-color:#46b8da}.btn-info.focus,.btn-info:focus{color:#fff;background-color:#31b0d5;border-color:#1b6d85}.btn-info:hover{color:#fff;background-color:#31b0d5;border-color:#269abc}.btn-info.active,.btn-info:active,.open>.dropdown-toggle.btn-info{color:#fff;background-color:#31b0d5;background-image:none;border-color:#269abc}.btn-info.active.focus,.btn-info.active:focus,.btn-info.active:hover,.btn-info:active.focus,.btn-info:active:focus,.btn-info:active:hover,.open>.dropdown-toggle.btn-info.focus,.open>.dropdown-toggle.btn-info:focus,.open>.dropdown-toggle.btn-info:hover{color:#fff;background-color:#269abc;border-color:#1b6d85}.btn-info.disabled.focus,.btn-info.disabled:focus,.btn-info.disabled:hover,.btn-info[disabled].focus,.btn-info[disabled]:focus,.btn-info[disabled]:hover,fieldset[disabled] .btn-info.focus,fieldset[disabled] .btn-info:focus,fieldset[disabled] .btn-info:hover{background-color:#5bc0de;border-color:#46b8da}.btn-info .badge{color:#5bc0de;background-color:#fff}.btn-warning{color:#fff;background-color:#f0ad4e;border-color:#eea236}.btn-warning.focus,.btn-warning:focus{color:#fff;background-color:#ec971f;border-color:#985f0d}.btn-warning:hover{color:#fff;background-color:#ec971f;border-color:#d58512}.btn-warning.active,.btn-warning:active,.open>.dropdown-toggle.btn-warning{color:#fff;background-color:#ec971f;background-image:none;border-color:#d58512}.btn-warning.active.focus,.btn-warning.active:focus,.btn-warning.active:hover,.btn-warning:active.focus,.btn-warning:active:focus,.btn-warning:active:hover,.open>.dropdown-toggle.btn-warning.focus,.open>.dropdown-toggle.btn-warning:focus,.open>.dropdown-toggle.btn-warning:hover{color:#fff;background-color:#d58512;border-color:#985f0d}.btn-warning.disabled.focus,.btn-warning.disabled:focus,.btn-warning.disabled:hover,.btn-warning[disabled].focus,.btn-warning[disabled]:focus,.btn-warning[disabled]:hover,fieldset[disabled] .btn-warning.focus,fieldset[disabled] .btn-warning:focus,fieldset[disabled] .btn-warning:hover{background-color:#f0ad4e;border-color:#eea236}.btn-warning .badge{color:#f0ad4e;background-color:#fff}.btn-danger{color:#fff;background-color:#d9534f;border-color:#d43f3a}.btn-danger.focus,.btn-danger:focus{color:#fff;background-color:#c9302c;border-color:#761c19}.btn-danger:hover{color:#fff;background-color:#c9302c;border-color:#ac2925}.btn-danger.active,.btn-danger:active,.open>.dropdown-toggle.btn-danger{color:#fff;background-color:#c9302c;background-image:none;border-color:#ac2925}.btn-danger.active.focus,.btn-danger.active:focus,.btn-danger.active:hover,.btn-danger:active.focus,.btn-danger:active:focus,.btn-danger:active:hover,.open>.dropdown-toggle.btn-danger.focus,.open>.dropdown-toggle.btn-danger:focus,.open>.dropdown-toggle.btn-danger:hover{color:#fff;background-color:#ac2925;border-color:#761c19}.btn-danger.disabled.focus,.btn-danger.disabled:focus,.btn-danger.disabled:hover,.btn-danger[disabled].focus,.btn-danger[disabled]:focus,.btn-danger[disabled]:hover,fieldset[disabled] .btn-danger.focus,fieldset[disabled] .btn-danger:focus,fieldset[disabled] .btn-danger:hover{background-color:#d9534f;border-color:#d43f3a}.btn-danger .badge{color:#d9534f;background-color:#fff}.btn-link{font-weight:400;color:#337ab7;border-radius:0}.btn-link,.btn-link.active,.btn-link:active,.btn-link[disabled],fieldset[disabled] .btn-link{background-color:transparent;-webkit-box-shadow:none;box-shadow:none}.btn-link,.btn-link:active,.btn-link:focus,.btn-link:hover{border-color:transparent}.btn-link:focus,.btn-link:hover{color:#23527c;text-decoration:underline;background-color:transparent}.btn-link[disabled]:focus,.btn-link[disabled]:hover,fieldset[disabled] .btn-link:focus,fieldset[disabled] .btn-link:hover{color:#777;text-decoration:none}.btn-group-lg>.btn,.btn-lg{padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}.btn-group-sm>.btn,.btn-sm{padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}.btn-group-xs>.btn,.btn-xs{padding:1px 5px;font-size:12px;line-height:1.5;border-radius:3px}.btn-block{display:block;width:100%}.btn-block+.btn-block{margin-top:5px}input[type=button].btn-block,input[type=reset].btn-block,input[type=submit].btn-block{width:100%}.fade{opacity:0;-webkit-transition:opacity .15s linear;-o-transition:opacity .15s linear;transition:opacity .15s linear}.fade.in{opacity:1}.collapse{display:none}.collapse.in{display:block}tr.collapse.in{display:table-row}tbody.collapse.in{display:table-row-group}.collapsing{position:relative;height:0;overflow:hidden;-webkit-transition-property:height,visibility;-o-transition-property:height,visibility;transition-property:height,visibility;-webkit-transition-duration:.35s;-o-transition-duration:.35s;transition-duration:.35s;-webkit-transition-timing-function:ease;-o-transition-timing-function:ease;transition-timing-function:ease}.caret{display:inline-block;width:0;height:0;margin-left:2px;vertical-align:middle;border-top:4px dashed;border-top:4px solid\9;border-right:4px solid transparent;border-left:4px solid transparent}.dropdown,.dropup{position:relative}.dropdown-toggle:focus{outline:0}.dropdown-menu{position:absolute;top:100%;left:0;z-index:1000;display:none;float:left;min-width:160px;padding:5px 0;margin:2px 0 0;font-size:14px;text-align:left;list-style:none;background-color:#fff;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.15);border-radius:4px;-webkit-box-shadow:0 6px 12px rgba(0,0,0,.175);box-shadow:0 6px 12px rgba(0,0,0,.175)}.dropdown-menu.pull-right{right:0;left:auto}.dropdown-menu .divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.dropdown-menu>li>a{display:block;padding:3px 20px;clear:both;font-weight:400;line-height:1.42857143;color:#333;white-space:nowrap}.dropdown-menu>li>a:focus,.dropdown-menu>li>a:hover{color:#262626;text-decoration:none;background-color:#f5f5f5}.dropdown-menu>.active>a,.dropdown-menu>.active>a:focus,.dropdown-menu>.active>a:hover{color:#fff;text-decoration:none;background-color:#337ab7;outline:0}.dropdown-menu>.disabled>a,.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{color:#777}.dropdown-menu>.disabled>a:focus,.dropdown-menu>.disabled>a:hover{text-decoration:none;cursor:not-allowed;background-color:transparent;background-image:none;filter:progid:DXImageTransform.Microsoft.gradient(enabled=false)}.open>.dropdown-menu{display:block}.open>a{outline:0}.dropdown-menu-right{right:0;left:auto}.dropdown-menu-left{right:auto;left:0}.dropdown-header{display:block;padding:3px 20px;font-size:12px;line-height:1.42857143;color:#777;white-space:nowrap}.dropdown-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:990}.pull-right>.dropdown-menu{right:0;left:auto}.dropup .caret,.navbar-fixed-bottom .dropdown .caret{content:"";border-top:0;border-bottom:4px dashed;border-bottom:4px solid\9}.dropup .dropdown-menu,.navbar-fixed-bottom .dropdown .dropdown-menu{top:auto;bottom:100%;margin-bottom:2px}@media (min-width:768px){.navbar-right .dropdown-menu{right:0;left:auto}.navbar-right .dropdown-menu-left{right:auto;left:0}}.btn-group,.btn-group-vertical{position:relative;display:inline-block;vertical-align:middle}.btn-group-vertical>.btn,.btn-group>.btn{position:relative;float:left}.btn-group-vertical>.btn.active,.btn-group-vertical>.btn:active,.btn-group-vertical>.btn:focus,.btn-group-vertical>.btn:hover,.btn-group>.btn.active,.btn-group>.btn:active,.btn-group>.btn:focus,.btn-group>.btn:hover{z-index:2}.btn-group .btn+.btn,.btn-group .btn+.btn-group,.btn-group .btn-group+.btn,.btn-group .btn-group+.btn-group{margin-left:-1px}.btn-toolbar{margin-left:-5px}.btn-toolbar .btn,.btn-toolbar .btn-group,.btn-toolbar .input-group{float:left}.btn-toolbar>.btn,.btn-toolbar>.btn-group,.btn-toolbar>.input-group{margin-left:5px}.btn-group>.btn:not(:first-child):not(:last-child):not(.dropdown-toggle){border-radius:0}.btn-group>.btn:first-child{margin-left:0}.btn-group>.btn:first-child:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn:last-child:not(:first-child),.btn-group>.dropdown-toggle:not(:first-child){border-top-left-radius:0;border-bottom-left-radius:0}.btn-group>.btn-group{float:left}.btn-group>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-top-right-radius:0;border-bottom-right-radius:0}.btn-group>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-bottom-left-radius:0}.btn-group .dropdown-toggle:active,.btn-group.open .dropdown-toggle{outline:0}.btn-group>.btn+.dropdown-toggle{padding-right:8px;padding-left:8px}.btn-group>.btn-lg+.dropdown-toggle{padding-right:12px;padding-left:12px}.btn-group.open .dropdown-toggle{-webkit-box-shadow:inset 0 3px 5px rgba(0,0,0,.125);box-shadow:inset 0 3px 5px rgba(0,0,0,.125)}.btn-group.open .dropdown-toggle.btn-link{-webkit-box-shadow:none;box-shadow:none}.btn .caret{margin-left:0}.btn-lg .caret{border-width:5px 5px 0;border-bottom-width:0}.dropup .btn-lg .caret{border-width:0 5px 5px}.btn-group-vertical>.btn,.btn-group-vertical>.btn-group,.btn-group-vertical>.btn-group>.btn{display:block;float:none;width:100%;max-width:100%}.btn-group-vertical>.btn-group>.btn{float:none}.btn-group-vertical>.btn+.btn,.btn-group-vertical>.btn+.btn-group,.btn-group-vertical>.btn-group+.btn,.btn-group-vertical>.btn-group+.btn-group{margin-top:-1px;margin-left:0}.btn-group-vertical>.btn:not(:first-child):not(:last-child){border-radius:0}.btn-group-vertical>.btn:first-child:not(:last-child){border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn:last-child:not(:first-child){border-top-left-radius:0;border-top-right-radius:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.btn-group-vertical>.btn-group:not(:first-child):not(:last-child)>.btn{border-radius:0}.btn-group-vertical>.btn-group:first-child:not(:last-child)>.btn:last-child,.btn-group-vertical>.btn-group:first-child:not(:last-child)>.dropdown-toggle{border-bottom-right-radius:0;border-bottom-left-radius:0}.btn-group-vertical>.btn-group:last-child:not(:first-child)>.btn:first-child{border-top-left-radius:0;border-top-right-radius:0}.btn-group-justified{display:table;width:100%;table-layout:fixed;border-collapse:separate}.btn-group-justified>.btn,.btn-group-justified>.btn-group{display:table-cell;float:none;width:1%}.btn-group-justified>.btn-group .btn{width:100%}.btn-group-justified>.btn-group .dropdown-menu{left:auto}[data-toggle=buttons]>.btn input[type=checkbox],[data-toggle=buttons]>.btn input[type=radio],[data-toggle=buttons]>.btn-group>.btn input[type=checkbox],[data-toggle=buttons]>.btn-group>.btn input[type=radio]{position:absolute;clip:rect(0,0,0,0);pointer-events:none}.input-group{position:relative;display:table;border-collapse:separate}.input-group[class*=col-]{float:none;padding-right:0;padding-left:0}.input-group .form-control{position:relative;z-index:2;float:left;width:100%;margin-bottom:0}.input-group .form-control:focus{z-index:3}.input-group-lg>.form-control,.input-group-lg>.input-group-addon,.input-group-lg>.input-group-btn>.btn{height:46px;padding:10px 16px;font-size:18px;line-height:1.3333333;border-radius:6px}select.input-group-lg>.form-control,select.input-group-lg>.input-group-addon,select.input-group-lg>.input-group-btn>.btn{height:46px;line-height:46px}select[multiple].input-group-lg>.form-control,select[multiple].input-group-lg>.input-group-addon,select[multiple].input-group-lg>.input-group-btn>.btn,textarea.input-group-lg>.form-control,textarea.input-group-lg>.input-group-addon,textarea.input-group-lg>.input-group-btn>.btn{height:auto}.input-group-sm>.form-control,.input-group-sm>.input-group-addon,.input-group-sm>.input-group-btn>.btn{height:30px;padding:5px 10px;font-size:12px;line-height:1.5;border-radius:3px}select.input-group-sm>.form-control,select.input-group-sm>.input-group-addon,select.input-group-sm>.input-group-btn>.btn{height:30px;line-height:30px}select[multiple].input-group-sm>.form-control,select[multiple].input-group-sm>.input-group-addon,select[multiple].input-group-sm>.input-group-btn>.btn,textarea.input-group-sm>.form-control,textarea.input-group-sm>.input-group-addon,textarea.input-group-sm>.input-group-btn>.btn{height:auto}.input-group .form-control,.input-group-addon,.input-group-btn{display:table-cell}.input-group .form-control:not(:first-child):not(:last-child),.input-group-addon:not(:first-child):not(:last-child),.input-group-btn:not(:first-child):not(:last-child){border-radius:0}.input-group-addon,.input-group-btn{width:1%;white-space:nowrap;vertical-align:middle}.input-group-addon{padding:6px 12px;font-size:14px;font-weight:400;line-height:1;color:#555;text-align:center;background-color:#eee;border:1px solid #ccc;border-radius:4px}.input-group-addon.input-sm{padding:5px 10px;font-size:12px;border-radius:3px}.input-group-addon.input-lg{padding:10px 16px;font-size:18px;border-radius:6px}.input-group-addon input[type=checkbox],.input-group-addon input[type=radio]{margin-top:0}.input-group .form-control:first-child,.input-group-addon:first-child,.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group>.btn,.input-group-btn:first-child>.dropdown-toggle,.input-group-btn:last-child>.btn-group:not(:last-child)>.btn,.input-group-btn:last-child>.btn:not(:last-child):not(.dropdown-toggle){border-top-right-radius:0;border-bottom-right-radius:0}.input-group-addon:first-child{border-right:0}.input-group .form-control:last-child,.input-group-addon:last-child,.input-group-btn:first-child>.btn-group:not(:first-child)>.btn,.input-group-btn:first-child>.btn:not(:first-child),.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group>.btn,.input-group-btn:last-child>.dropdown-toggle{border-top-left-radius:0;border-bottom-left-radius:0}.input-group-addon:last-child{border-left:0}.input-group-btn{position:relative;font-size:0;white-space:nowrap}.input-group-btn>.btn{position:relative}.input-group-btn>.btn+.btn{margin-left:-1px}.input-group-btn>.btn:active,.input-group-btn>.btn:focus,.input-group-btn>.btn:hover{z-index:2}.input-group-btn:first-child>.btn,.input-group-btn:first-child>.btn-group{margin-right:-1px}.input-group-btn:last-child>.btn,.input-group-btn:last-child>.btn-group{z-index:2;margin-left:-1px}.nav{padding-left:0;margin-bottom:0;list-style:none}.nav>li{position:relative;display:block}.nav>li>a{position:relative;display:block;padding:10px 15px}.nav>li>a:focus,.nav>li>a:hover{text-decoration:none;background-color:#eee}.nav>li.disabled>a{color:#777}.nav>li.disabled>a:focus,.nav>li.disabled>a:hover{color:#777;text-decoration:none;cursor:not-allowed;background-color:transparent}.nav .open>a,.nav .open>a:focus,.nav .open>a:hover{background-color:#eee;border-color:#337ab7}.nav .nav-divider{height:1px;margin:9px 0;overflow:hidden;background-color:#e5e5e5}.nav>li>a>img{max-width:none}.nav-tabs{border-bottom:1px solid #ddd}.nav-tabs>li{float:left;margin-bottom:-1px}.nav-tabs>li>a{margin-right:2px;line-height:1.42857143;border:1px solid transparent;border-radius:4px 4px 0 0}.nav-tabs>li>a:hover{border-color:#eee #eee #ddd}.nav-tabs>li.active>a,.nav-tabs>li.active>a:focus,.nav-tabs>li.active>a:hover{color:#555;cursor:default;background-color:#fff;border:1px solid #ddd;border-bottom-color:transparent}.nav-tabs.nav-justified{width:100%;border-bottom:0}.nav-tabs.nav-justified>li{float:none}.nav-tabs.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-tabs.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-tabs.nav-justified>li{display:table-cell;width:1%}.nav-tabs.nav-justified>li>a{margin-bottom:0}}.nav-tabs.nav-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs.nav-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs.nav-justified>.active>a,.nav-tabs.nav-justified>.active>a:focus,.nav-tabs.nav-justified>.active>a:hover{border-bottom-color:#fff}}.nav-pills>li{float:left}.nav-pills>li>a{border-radius:4px}.nav-pills>li+li{margin-left:2px}.nav-pills>li.active>a,.nav-pills>li.active>a:focus,.nav-pills>li.active>a:hover{color:#fff;background-color:#337ab7}.nav-stacked>li{float:none}.nav-stacked>li+li{margin-top:2px;margin-left:0}.nav-justified{width:100%}.nav-justified>li{float:none}.nav-justified>li>a{margin-bottom:5px;text-align:center}.nav-justified>.dropdown .dropdown-menu{top:auto;left:auto}@media (min-width:768px){.nav-justified>li{display:table-cell;width:1%}.nav-justified>li>a{margin-bottom:0}}.nav-tabs-justified{border-bottom:0}.nav-tabs-justified>li>a{margin-right:0;border-radius:4px}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border:1px solid #ddd}@media (min-width:768px){.nav-tabs-justified>li>a{border-bottom:1px solid #ddd;border-radius:4px 4px 0 0}.nav-tabs-justified>.active>a,.nav-tabs-justified>.active>a:focus,.nav-tabs-justified>.active>a:hover{border-bottom-color:#fff}}.tab-content>.tab-pane{display:none}.tab-content>.active{display:block}.nav-tabs .dropdown-menu{margin-top:-1px;border-top-left-radius:0;border-top-right-radius:0}.navbar{position:relative;min-height:50px;margin-bottom:20px;border:1px solid transparent}@media (min-width:768px){.navbar{border-radius:4px}}@media (min-width:768px){.navbar-header{float:left}}.navbar-collapse{padding-right:15px;padding-left:15px;overflow-x:visible;border-top:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1);-webkit-overflow-scrolling:touch}.navbar-collapse.in{overflow-y:auto}@media (min-width:768px){.navbar-collapse{width:auto;border-top:0;-webkit-box-shadow:none;box-shadow:none}.navbar-collapse.collapse{display:block!important;height:auto!important;padding-bottom:0;overflow:visible!important}.navbar-collapse.in{overflow-y:visible}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse,.navbar-static-top .navbar-collapse{padding-right:0;padding-left:0}}.navbar-fixed-bottom,.navbar-fixed-top{position:fixed;right:0;left:0;z-index:1030}.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:340px}@media (max-device-width:480px) and (orientation:landscape){.navbar-fixed-bottom .navbar-collapse,.navbar-fixed-top .navbar-collapse{max-height:200px}}@media (min-width:768px){.navbar-fixed-bottom,.navbar-fixed-top{border-radius:0}}.navbar-fixed-top{top:0;border-width:0 0 1px}.navbar-fixed-bottom{bottom:0;margin-bottom:0;border-width:1px 0 0}.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:-15px;margin-left:-15px}@media (min-width:768px){.container-fluid>.navbar-collapse,.container-fluid>.navbar-header,.container>.navbar-collapse,.container>.navbar-header{margin-right:0;margin-left:0}}.navbar-static-top{z-index:1000;border-width:0 0 1px}@media (min-width:768px){.navbar-static-top{border-radius:0}}.navbar-brand{float:left;height:50px;padding:15px 15px;font-size:18px;line-height:20px}.navbar-brand:focus,.navbar-brand:hover{text-decoration:none}.navbar-brand>img{display:block}@media (min-width:768px){.navbar>.container .navbar-brand,.navbar>.container-fluid .navbar-brand{margin-left:-15px}}.navbar-toggle{position:relative;float:right;padding:9px 10px;margin-right:15px;margin-top:8px;margin-bottom:8px;background-color:transparent;background-image:none;border:1px solid transparent;border-radius:4px}.navbar-toggle:focus{outline:0}.navbar-toggle .icon-bar{display:block;width:22px;height:2px;border-radius:1px}.navbar-toggle .icon-bar+.icon-bar{margin-top:4px}@media (min-width:768px){.navbar-toggle{display:none}}.navbar-nav{margin:7.5px -15px}.navbar-nav>li>a{padding-top:10px;padding-bottom:10px;line-height:20px}@media (max-width:767px){.navbar-nav .open .dropdown-menu{position:static;float:none;width:auto;margin-top:0;background-color:transparent;border:0;-webkit-box-shadow:none;box-shadow:none}.navbar-nav .open .dropdown-menu .dropdown-header,.navbar-nav .open .dropdown-menu>li>a{padding:5px 15px 5px 25px}.navbar-nav .open .dropdown-menu>li>a{line-height:20px}.navbar-nav .open .dropdown-menu>li>a:focus,.navbar-nav .open .dropdown-menu>li>a:hover{background-image:none}}@media (min-width:768px){.navbar-nav{float:left;margin:0}.navbar-nav>li{float:left}.navbar-nav>li>a{padding-top:15px;padding-bottom:15px}}.navbar-form{padding:10px 15px;margin-right:-15px;margin-left:-15px;border-top:1px solid transparent;border-bottom:1px solid transparent;-webkit-box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);box-shadow:inset 0 1px 0 rgba(255,255,255,.1),0 1px 0 rgba(255,255,255,.1);margin-top:8px;margin-bottom:8px}@media (min-width:768px){.navbar-form .form-group{display:inline-block;margin-bottom:0;vertical-align:middle}.navbar-form .form-control{display:inline-block;width:auto;vertical-align:middle}.navbar-form .form-control-static{display:inline-block}.navbar-form .input-group{display:inline-table;vertical-align:middle}.navbar-form .input-group .form-control,.navbar-form .input-group .input-group-addon,.navbar-form .input-group .input-group-btn{width:auto}.navbar-form .input-group>.form-control{width:100%}.navbar-form .control-label{margin-bottom:0;vertical-align:middle}.navbar-form .checkbox,.navbar-form .radio{display:inline-block;margin-top:0;margin-bottom:0;vertical-align:middle}.navbar-form .checkbox label,.navbar-form .radio label{padding-left:0}.navbar-form .checkbox input[type=checkbox],.navbar-form .radio input[type=radio]{position:relative;margin-left:0}.navbar-form .has-feedback .form-control-feedback{top:0}}@media (max-width:767px){.navbar-form .form-group{margin-bottom:5px}.navbar-form .form-group:last-child{margin-bottom:0}}@media (min-width:768px){.navbar-form{width:auto;padding-top:0;padding-bottom:0;margin-right:0;margin-left:0;border:0;-webkit-box-shadow:none;box-shadow:none}}.navbar-nav>li>.dropdown-menu{margin-top:0;border-top-left-radius:0;border-top-right-radius:0}.navbar-fixed-bottom .navbar-nav>li>.dropdown-menu{margin-bottom:0;border-top-left-radius:4px;border-top-right-radius:4px;border-bottom-right-radius:0;border-bottom-left-radius:0}.navbar-btn{margin-top:8px;margin-bottom:8px}.navbar-btn.btn-sm{margin-top:10px;margin-bottom:10px}.navbar-btn.btn-xs{margin-top:14px;margin-bottom:14px}.navbar-text{margin-top:15px;margin-bottom:15px}@media (min-width:768px){.navbar-text{float:left;margin-right:15px;margin-left:15px}}@media (min-width:768px){.navbar-left{float:left!important}.navbar-right{float:right!important;margin-right:-15px}.navbar-right~.navbar-right{margin-right:0}}.navbar-default{background-color:#f8f8f8;border-color:#e7e7e7}.navbar-default .navbar-brand{color:#777}.navbar-default .navbar-brand:focus,.navbar-default .navbar-brand:hover{color:#5e5e5e;background-color:transparent}.navbar-default .navbar-text{color:#777}.navbar-default .navbar-nav>li>a{color:#777}.navbar-default .navbar-nav>li>a:focus,.navbar-default .navbar-nav>li>a:hover{color:#333;background-color:transparent}.navbar-default .navbar-nav>.active>a,.navbar-default .navbar-nav>.active>a:focus,.navbar-default .navbar-nav>.active>a:hover{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav>.disabled>a,.navbar-default .navbar-nav>.disabled>a:focus,.navbar-default .navbar-nav>.disabled>a:hover{color:#ccc;background-color:transparent}.navbar-default .navbar-nav>.open>a,.navbar-default .navbar-nav>.open>a:focus,.navbar-default .navbar-nav>.open>a:hover{color:#555;background-color:#e7e7e7}@media (max-width:767px){.navbar-default .navbar-nav .open .dropdown-menu>li>a{color:#777}.navbar-default .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>li>a:hover{color:#333;background-color:transparent}.navbar-default .navbar-nav .open .dropdown-menu>.active>a,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.active>a:hover{color:#555;background-color:#e7e7e7}.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-default .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#ccc;background-color:transparent}}.navbar-default .navbar-toggle{border-color:#ddd}.navbar-default .navbar-toggle:focus,.navbar-default .navbar-toggle:hover{background-color:#ddd}.navbar-default .navbar-toggle .icon-bar{background-color:#888}.navbar-default .navbar-collapse,.navbar-default .navbar-form{border-color:#e7e7e7}.navbar-default .navbar-link{color:#777}.navbar-default .navbar-link:hover{color:#333}.navbar-default .btn-link{color:#777}.navbar-default .btn-link:focus,.navbar-default .btn-link:hover{color:#333}.navbar-default .btn-link[disabled]:focus,.navbar-default .btn-link[disabled]:hover,fieldset[disabled] .navbar-default .btn-link:focus,fieldset[disabled] .navbar-default .btn-link:hover{color:#ccc}.navbar-inverse{background-color:#222;border-color:#080808}.navbar-inverse .navbar-brand{color:#9d9d9d}.navbar-inverse .navbar-brand:focus,.navbar-inverse .navbar-brand:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-text{color:#9d9d9d}.navbar-inverse .navbar-nav>li>a{color:#9d9d9d}.navbar-inverse .navbar-nav>li>a:focus,.navbar-inverse .navbar-nav>li>a:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav>.active>a,.navbar-inverse .navbar-nav>.active>a:focus,.navbar-inverse .navbar-nav>.active>a:hover{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav>.disabled>a,.navbar-inverse .navbar-nav>.disabled>a:focus,.navbar-inverse .navbar-nav>.disabled>a:hover{color:#444;background-color:transparent}.navbar-inverse .navbar-nav>.open>a,.navbar-inverse .navbar-nav>.open>a:focus,.navbar-inverse .navbar-nav>.open>a:hover{color:#fff;background-color:#080808}@media (max-width:767px){.navbar-inverse .navbar-nav .open .dropdown-menu>.dropdown-header{border-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu .divider{background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a{color:#9d9d9d}.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>li>a:hover{color:#fff;background-color:transparent}.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.active>a:hover{color:#fff;background-color:#080808}.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:focus,.navbar-inverse .navbar-nav .open .dropdown-menu>.disabled>a:hover{color:#444;background-color:transparent}}.navbar-inverse .navbar-toggle{border-color:#333}.navbar-inverse .navbar-toggle:focus,.navbar-inverse .navbar-toggle:hover{background-color:#333}.navbar-inverse .navbar-toggle .icon-bar{background-color:#fff}.navbar-inverse .navbar-collapse,.navbar-inverse .navbar-form{border-color:#101010}.navbar-inverse .navbar-link{color:#9d9d9d}.navbar-inverse .navbar-link:hover{color:#fff}.navbar-inverse .btn-link{color:#9d9d9d}.navbar-inverse .btn-link:focus,.navbar-inverse .btn-link:hover{color:#fff}.navbar-inverse .btn-link[disabled]:focus,.navbar-inverse .btn-link[disabled]:hover,fieldset[disabled] .navbar-inverse .btn-link:focus,fieldset[disabled] .navbar-inverse .btn-link:hover{color:#444}.breadcrumb{padding:8px 15px;margin-bottom:20px;list-style:none;background-color:#f5f5f5;border-radius:4px}.breadcrumb>li{display:inline-block}.breadcrumb>li+li:before{padding:0 5px;color:#ccc;content:"/\00a0"}.breadcrumb>.active{color:#777}.pagination{display:inline-block;padding-left:0;margin:20px 0;border-radius:4px}.pagination>li{display:inline}.pagination>li>a,.pagination>li>span{position:relative;float:left;padding:6px 12px;margin-left:-1px;line-height:1.42857143;color:#337ab7;text-decoration:none;background-color:#fff;border:1px solid #ddd}.pagination>li>a:focus,.pagination>li>a:hover,.pagination>li>span:focus,.pagination>li>span:hover{z-index:2;color:#23527c;background-color:#eee;border-color:#ddd}.pagination>li:first-child>a,.pagination>li:first-child>span{margin-left:0;border-top-left-radius:4px;border-bottom-left-radius:4px}.pagination>li:last-child>a,.pagination>li:last-child>span{border-top-right-radius:4px;border-bottom-right-radius:4px}.pagination>.active>a,.pagination>.active>a:focus,.pagination>.active>a:hover,.pagination>.active>span,.pagination>.active>span:focus,.pagination>.active>span:hover{z-index:3;color:#fff;cursor:default;background-color:#337ab7;border-color:#337ab7}.pagination>.disabled>a,.pagination>.disabled>a:focus,.pagination>.disabled>a:hover,.pagination>.disabled>span,.pagination>.disabled>span:focus,.pagination>.disabled>span:hover{color:#777;cursor:not-allowed;background-color:#fff;border-color:#ddd}.pagination-lg>li>a,.pagination-lg>li>span{padding:10px 16px;font-size:18px;line-height:1.3333333}.pagination-lg>li:first-child>a,.pagination-lg>li:first-child>span{border-top-left-radius:6px;border-bottom-left-radius:6px}.pagination-lg>li:last-child>a,.pagination-lg>li:last-child>span{border-top-right-radius:6px;border-bottom-right-radius:6px}.pagination-sm>li>a,.pagination-sm>li>span{padding:5px 10px;font-size:12px;line-height:1.5}.pagination-sm>li:first-child>a,.pagination-sm>li:first-child>span{border-top-left-radius:3px;border-bottom-left-radius:3px}.pagination-sm>li:last-child>a,.pagination-sm>li:last-child>span{border-top-right-radius:3px;border-bottom-right-radius:3px}.pager{padding-left:0;margin:20px 0;text-align:center;list-style:none}.pager li{display:inline}.pager li>a,.pager li>span{display:inline-block;padding:5px 14px;background-color:#fff;border:1px solid #ddd;border-radius:15px}.pager li>a:focus,.pager li>a:hover{text-decoration:none;background-color:#eee}.pager .next>a,.pager .next>span{float:right}.pager .previous>a,.pager .previous>span{float:left}.pager .disabled>a,.pager .disabled>a:focus,.pager .disabled>a:hover,.pager .disabled>span{color:#777;cursor:not-allowed;background-color:#fff}.label{display:inline;padding:.2em .6em .3em;font-size:75%;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:baseline;border-radius:.25em}a.label:focus,a.label:hover{color:#fff;text-decoration:none;cursor:pointer}.label:empty{display:none}.btn .label{position:relative;top:-1px}.label-default{background-color:#777}.label-default[href]:focus,.label-default[href]:hover{background-color:#5e5e5e}.label-primary{background-color:#337ab7}.label-primary[href]:focus,.label-primary[href]:hover{background-color:#286090}.label-success{background-color:#5cb85c}.label-success[href]:focus,.label-success[href]:hover{background-color:#449d44}.label-info{background-color:#5bc0de}.label-info[href]:focus,.label-info[href]:hover{background-color:#31b0d5}.label-warning{background-color:#f0ad4e}.label-warning[href]:focus,.label-warning[href]:hover{background-color:#ec971f}.label-danger{background-color:#d9534f}.label-danger[href]:focus,.label-danger[href]:hover{background-color:#c9302c}.badge{display:inline-block;min-width:10px;padding:3px 7px;font-size:12px;font-weight:700;line-height:1;color:#fff;text-align:center;white-space:nowrap;vertical-align:middle;background-color:#777;border-radius:10px}.badge:empty{display:none}.btn .badge{position:relative;top:-1px}.btn-group-xs>.btn .badge,.btn-xs .badge{top:0;padding:1px 5px}a.badge:focus,a.badge:hover{color:#fff;text-decoration:none;cursor:pointer}.list-group-item.active>.badge,.nav-pills>.active>a>.badge{color:#337ab7;background-color:#fff}.list-group-item>.badge{float:right}.list-group-item>.badge+.badge{margin-right:5px}.nav-pills>li>a>.badge{margin-left:3px}.jumbotron{padding-top:30px;padding-bottom:30px;margin-bottom:30px;color:inherit;background-color:#eee}.jumbotron .h1,.jumbotron h1{color:inherit}.jumbotron p{margin-bottom:15px;font-size:21px;font-weight:200}.jumbotron>hr{border-top-color:#d5d5d5}.container .jumbotron,.container-fluid .jumbotron{padding-right:15px;padding-left:15px;border-radius:6px}.jumbotron .container{max-width:100%}@media screen and (min-width:768px){.jumbotron{padding-top:48px;padding-bottom:48px}.container .jumbotron,.container-fluid .jumbotron{padding-right:60px;padding-left:60px}.jumbotron .h1,.jumbotron h1{font-size:63px}}.thumbnail{display:block;padding:4px;margin-bottom:20px;line-height:1.42857143;background-color:#fff;border:1px solid #ddd;border-radius:4px;-webkit-transition:border .2s ease-in-out;-o-transition:border .2s ease-in-out;transition:border .2s ease-in-out}.thumbnail a>img,.thumbnail>img{margin-right:auto;margin-left:auto}a.thumbnail.active,a.thumbnail:focus,a.thumbnail:hover{border-color:#337ab7}.thumbnail .caption{padding:9px;color:#333}.alert{padding:15px;margin-bottom:20px;border:1px solid transparent;border-radius:4px}.alert h4{margin-top:0;color:inherit}.alert .alert-link{font-weight:700}.alert>p,.alert>ul{margin-bottom:0}.alert>p+p{margin-top:5px}.alert-dismissable,.alert-dismissible{padding-right:35px}.alert-dismissable .close,.alert-dismissible .close{position:relative;top:-2px;right:-21px;color:inherit}.alert-success{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.alert-success hr{border-top-color:#c9e2b3}.alert-success .alert-link{color:#2b542c}.alert-info{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.alert-info hr{border-top-color:#a6e1ec}.alert-info .alert-link{color:#245269}.alert-warning{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.alert-warning hr{border-top-color:#f7e1b5}.alert-warning .alert-link{color:#66512c}.alert-danger{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.alert-danger hr{border-top-color:#e4b9c0}.alert-danger .alert-link{color:#843534}@-webkit-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@-o-keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}@keyframes progress-bar-stripes{from{background-position:40px 0}to{background-position:0 0}}.progress{height:20px;margin-bottom:20px;overflow:hidden;background-color:#f5f5f5;border-radius:4px;-webkit-box-shadow:inset 0 1px 2px rgba(0,0,0,.1);box-shadow:inset 0 1px 2px rgba(0,0,0,.1)}.progress-bar{float:left;width:0%;height:100%;font-size:12px;line-height:20px;color:#fff;text-align:center;background-color:#337ab7;-webkit-box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);box-shadow:inset 0 -1px 0 rgba(0,0,0,.15);-webkit-transition:width .6s ease;-o-transition:width .6s ease;transition:width .6s ease}.progress-bar-striped,.progress-striped .progress-bar{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);-webkit-background-size:40px 40px;background-size:40px 40px}.progress-bar.active,.progress.active .progress-bar{-webkit-animation:progress-bar-stripes 2s linear infinite;-o-animation:progress-bar-stripes 2s linear infinite;animation:progress-bar-stripes 2s linear infinite}.progress-bar-success{background-color:#5cb85c}.progress-striped .progress-bar-success{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-info{background-color:#5bc0de}.progress-striped .progress-bar-info{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-warning{background-color:#f0ad4e}.progress-striped .progress-bar-warning{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.progress-bar-danger{background-color:#d9534f}.progress-striped .progress-bar-danger{background-image:-webkit-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:-o-linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent);background-image:linear-gradient(45deg,rgba(255,255,255,.15) 25%,transparent 25%,transparent 50%,rgba(255,255,255,.15) 50%,rgba(255,255,255,.15) 75%,transparent 75%,transparent)}.media{margin-top:15px}.media:first-child{margin-top:0}.media,.media-body{overflow:hidden;zoom:1}.media-body{width:10000px}.media-object{display:block}.media-object.img-thumbnail{max-width:none}.media-right,.media>.pull-right{padding-left:10px}.media-left,.media>.pull-left{padding-right:10px}.media-body,.media-left,.media-right{display:table-cell;vertical-align:top}.media-middle{vertical-align:middle}.media-bottom{vertical-align:bottom}.media-heading{margin-top:0;margin-bottom:5px}.media-list{padding-left:0;list-style:none}.list-group{padding-left:0;margin-bottom:20px}.list-group-item{position:relative;display:block;padding:10px 15px;margin-bottom:-1px;background-color:#fff;border:1px solid #ddd}.list-group-item:first-child{border-top-left-radius:4px;border-top-right-radius:4px}.list-group-item:last-child{margin-bottom:0;border-bottom-right-radius:4px;border-bottom-left-radius:4px}.list-group-item.disabled,.list-group-item.disabled:focus,.list-group-item.disabled:hover{color:#777;cursor:not-allowed;background-color:#eee}.list-group-item.disabled .list-group-item-heading,.list-group-item.disabled:focus .list-group-item-heading,.list-group-item.disabled:hover .list-group-item-heading{color:inherit}.list-group-item.disabled .list-group-item-text,.list-group-item.disabled:focus .list-group-item-text,.list-group-item.disabled:hover .list-group-item-text{color:#777}.list-group-item.active,.list-group-item.active:focus,.list-group-item.active:hover{z-index:2;color:#fff;background-color:#337ab7;border-color:#337ab7}.list-group-item.active .list-group-item-heading,.list-group-item.active .list-group-item-heading>.small,.list-group-item.active .list-group-item-heading>small,.list-group-item.active:focus .list-group-item-heading,.list-group-item.active:focus .list-group-item-heading>.small,.list-group-item.active:focus .list-group-item-heading>small,.list-group-item.active:hover .list-group-item-heading,.list-group-item.active:hover .list-group-item-heading>.small,.list-group-item.active:hover .list-group-item-heading>small{color:inherit}.list-group-item.active .list-group-item-text,.list-group-item.active:focus .list-group-item-text,.list-group-item.active:hover .list-group-item-text{color:#c7ddef}a.list-group-item,button.list-group-item{color:#555}a.list-group-item .list-group-item-heading,button.list-group-item .list-group-item-heading{color:#333}a.list-group-item:focus,a.list-group-item:hover,button.list-group-item:focus,button.list-group-item:hover{color:#555;text-decoration:none;background-color:#f5f5f5}button.list-group-item{width:100%;text-align:left}.list-group-item-success{color:#3c763d;background-color:#dff0d8}a.list-group-item-success,button.list-group-item-success{color:#3c763d}a.list-group-item-success .list-group-item-heading,button.list-group-item-success .list-group-item-heading{color:inherit}a.list-group-item-success:focus,a.list-group-item-success:hover,button.list-group-item-success:focus,button.list-group-item-success:hover{color:#3c763d;background-color:#d0e9c6}a.list-group-item-success.active,a.list-group-item-success.active:focus,a.list-group-item-success.active:hover,button.list-group-item-success.active,button.list-group-item-success.active:focus,button.list-group-item-success.active:hover{color:#fff;background-color:#3c763d;border-color:#3c763d}.list-group-item-info{color:#31708f;background-color:#d9edf7}a.list-group-item-info,button.list-group-item-info{color:#31708f}a.list-group-item-info .list-group-item-heading,button.list-group-item-info .list-group-item-heading{color:inherit}a.list-group-item-info:focus,a.list-group-item-info:hover,button.list-group-item-info:focus,button.list-group-item-info:hover{color:#31708f;background-color:#c4e3f3}a.list-group-item-info.active,a.list-group-item-info.active:focus,a.list-group-item-info.active:hover,button.list-group-item-info.active,button.list-group-item-info.active:focus,button.list-group-item-info.active:hover{color:#fff;background-color:#31708f;border-color:#31708f}.list-group-item-warning{color:#8a6d3b;background-color:#fcf8e3}a.list-group-item-warning,button.list-group-item-warning{color:#8a6d3b}a.list-group-item-warning .list-group-item-heading,button.list-group-item-warning .list-group-item-heading{color:inherit}a.list-group-item-warning:focus,a.list-group-item-warning:hover,button.list-group-item-warning:focus,button.list-group-item-warning:hover{color:#8a6d3b;background-color:#faf2cc}a.list-group-item-warning.active,a.list-group-item-warning.active:focus,a.list-group-item-warning.active:hover,button.list-group-item-warning.active,button.list-group-item-warning.active:focus,button.list-group-item-warning.active:hover{color:#fff;background-color:#8a6d3b;border-color:#8a6d3b}.list-group-item-danger{color:#a94442;background-color:#f2dede}a.list-group-item-danger,button.list-group-item-danger{color:#a94442}a.list-group-item-danger .list-group-item-heading,button.list-group-item-danger .list-group-item-heading{color:inherit}a.list-group-item-danger:focus,a.list-group-item-danger:hover,button.list-group-item-danger:focus,button.list-group-item-danger:hover{color:#a94442;background-color:#ebcccc}a.list-group-item-danger.active,a.list-group-item-danger.active:focus,a.list-group-item-danger.active:hover,button.list-group-item-danger.active,button.list-group-item-danger.active:focus,button.list-group-item-danger.active:hover{color:#fff;background-color:#a94442;border-color:#a94442}.list-group-item-heading{margin-top:0;margin-bottom:5px}.list-group-item-text{margin-bottom:0;line-height:1.3}.panel{margin-bottom:20px;background-color:#fff;border:1px solid transparent;border-radius:4px;-webkit-box-shadow:0 1px 1px rgba(0,0,0,.05);box-shadow:0 1px 1px rgba(0,0,0,.05)}.panel-body{padding:15px}.panel-heading{padding:10px 15px;border-bottom:1px solid transparent;border-top-left-radius:3px;border-top-right-radius:3px}.panel-heading>.dropdown .dropdown-toggle{color:inherit}.panel-title{margin-top:0;margin-bottom:0;font-size:16px;color:inherit}.panel-title>.small,.panel-title>.small>a,.panel-title>a,.panel-title>small,.panel-title>small>a{color:inherit}.panel-footer{padding:10px 15px;background-color:#f5f5f5;border-top:1px solid #ddd;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.list-group,.panel>.panel-collapse>.list-group{margin-bottom:0}.panel>.list-group .list-group-item,.panel>.panel-collapse>.list-group .list-group-item{border-width:1px 0;border-radius:0}.panel>.list-group:first-child .list-group-item:first-child,.panel>.panel-collapse>.list-group:first-child .list-group-item:first-child{border-top:0;border-top-left-radius:3px;border-top-right-radius:3px}.panel>.list-group:last-child .list-group-item:last-child,.panel>.panel-collapse>.list-group:last-child .list-group-item:last-child{border-bottom:0;border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.panel-heading+.panel-collapse>.list-group .list-group-item:first-child{border-top-left-radius:0;border-top-right-radius:0}.panel-heading+.list-group .list-group-item:first-child{border-top-width:0}.list-group+.panel-footer{border-top-width:0}.panel>.panel-collapse>.table,.panel>.table,.panel>.table-responsive>.table{margin-bottom:0}.panel>.panel-collapse>.table caption,.panel>.table caption,.panel>.table-responsive>.table caption{padding-right:15px;padding-left:15px}.panel>.table-responsive:first-child>.table:first-child,.panel>.table:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child,.panel>.table:first-child>thead:first-child>tr:first-child{border-top-left-radius:3px;border-top-right-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:first-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:first-child,.panel>.table:first-child>thead:first-child>tr:first-child td:first-child,.panel>.table:first-child>thead:first-child>tr:first-child th:first-child{border-top-left-radius:3px}.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table-responsive:first-child>.table:first-child>thead:first-child>tr:first-child th:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child td:last-child,.panel>.table:first-child>tbody:first-child>tr:first-child th:last-child,.panel>.table:first-child>thead:first-child>tr:first-child td:last-child,.panel>.table:first-child>thead:first-child>tr:first-child th:last-child{border-top-right-radius:3px}.panel>.table-responsive:last-child>.table:last-child,.panel>.table:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child{border-bottom-right-radius:3px;border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:first-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:first-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:first-child{border-bottom-left-radius:3px}.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table-responsive:last-child>.table:last-child>tfoot:last-child>tr:last-child th:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child td:last-child,.panel>.table:last-child>tbody:last-child>tr:last-child th:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child td:last-child,.panel>.table:last-child>tfoot:last-child>tr:last-child th:last-child{border-bottom-right-radius:3px}.panel>.panel-body+.table,.panel>.panel-body+.table-responsive,.panel>.table+.panel-body,.panel>.table-responsive+.panel-body{border-top:1px solid #ddd}.panel>.table>tbody:first-child>tr:first-child td,.panel>.table>tbody:first-child>tr:first-child th{border-top:0}.panel>.table-bordered,.panel>.table-responsive>.table-bordered{border:0}.panel>.table-bordered>tbody>tr>td:first-child,.panel>.table-bordered>tbody>tr>th:first-child,.panel>.table-bordered>tfoot>tr>td:first-child,.panel>.table-bordered>tfoot>tr>th:first-child,.panel>.table-bordered>thead>tr>td:first-child,.panel>.table-bordered>thead>tr>th:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:first-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:first-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:first-child,.panel>.table-responsive>.table-bordered>thead>tr>td:first-child,.panel>.table-responsive>.table-bordered>thead>tr>th:first-child{border-left:0}.panel>.table-bordered>tbody>tr>td:last-child,.panel>.table-bordered>tbody>tr>th:last-child,.panel>.table-bordered>tfoot>tr>td:last-child,.panel>.table-bordered>tfoot>tr>th:last-child,.panel>.table-bordered>thead>tr>td:last-child,.panel>.table-bordered>thead>tr>th:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>td:last-child,.panel>.table-responsive>.table-bordered>tbody>tr>th:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>td:last-child,.panel>.table-responsive>.table-bordered>tfoot>tr>th:last-child,.panel>.table-responsive>.table-bordered>thead>tr>td:last-child,.panel>.table-responsive>.table-bordered>thead>tr>th:last-child{border-right:0}.panel>.table-bordered>tbody>tr:first-child>td,.panel>.table-bordered>tbody>tr:first-child>th,.panel>.table-bordered>thead>tr:first-child>td,.panel>.table-bordered>thead>tr:first-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:first-child>th,.panel>.table-responsive>.table-bordered>thead>tr:first-child>td,.panel>.table-responsive>.table-bordered>thead>tr:first-child>th{border-bottom:0}.panel>.table-bordered>tbody>tr:last-child>td,.panel>.table-bordered>tbody>tr:last-child>th,.panel>.table-bordered>tfoot>tr:last-child>td,.panel>.table-bordered>tfoot>tr:last-child>th,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>td,.panel>.table-responsive>.table-bordered>tbody>tr:last-child>th,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>td,.panel>.table-responsive>.table-bordered>tfoot>tr:last-child>th{border-bottom:0}.panel>.table-responsive{margin-bottom:0;border:0}.panel-group{margin-bottom:20px}.panel-group .panel{margin-bottom:0;border-radius:4px}.panel-group .panel+.panel{margin-top:5px}.panel-group .panel-heading{border-bottom:0}.panel-group .panel-heading+.panel-collapse>.list-group,.panel-group .panel-heading+.panel-collapse>.panel-body{border-top:1px solid #ddd}.panel-group .panel-footer{border-top:0}.panel-group .panel-footer+.panel-collapse .panel-body{border-bottom:1px solid #ddd}.panel-default{border-color:#ddd}.panel-default>.panel-heading{color:#333;background-color:#f5f5f5;border-color:#ddd}.panel-default>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ddd}.panel-default>.panel-heading .badge{color:#f5f5f5;background-color:#333}.panel-default>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ddd}.panel-primary{border-color:#337ab7}.panel-primary>.panel-heading{color:#fff;background-color:#337ab7;border-color:#337ab7}.panel-primary>.panel-heading+.panel-collapse>.panel-body{border-top-color:#337ab7}.panel-primary>.panel-heading .badge{color:#337ab7;background-color:#fff}.panel-primary>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#337ab7}.panel-success{border-color:#d6e9c6}.panel-success>.panel-heading{color:#3c763d;background-color:#dff0d8;border-color:#d6e9c6}.panel-success>.panel-heading+.panel-collapse>.panel-body{border-top-color:#d6e9c6}.panel-success>.panel-heading .badge{color:#dff0d8;background-color:#3c763d}.panel-success>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#d6e9c6}.panel-info{border-color:#bce8f1}.panel-info>.panel-heading{color:#31708f;background-color:#d9edf7;border-color:#bce8f1}.panel-info>.panel-heading+.panel-collapse>.panel-body{border-top-color:#bce8f1}.panel-info>.panel-heading .badge{color:#d9edf7;background-color:#31708f}.panel-info>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#bce8f1}.panel-warning{border-color:#faebcc}.panel-warning>.panel-heading{color:#8a6d3b;background-color:#fcf8e3;border-color:#faebcc}.panel-warning>.panel-heading+.panel-collapse>.panel-body{border-top-color:#faebcc}.panel-warning>.panel-heading .badge{color:#fcf8e3;background-color:#8a6d3b}.panel-warning>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#faebcc}.panel-danger{border-color:#ebccd1}.panel-danger>.panel-heading{color:#a94442;background-color:#f2dede;border-color:#ebccd1}.panel-danger>.panel-heading+.panel-collapse>.panel-body{border-top-color:#ebccd1}.panel-danger>.panel-heading .badge{color:#f2dede;background-color:#a94442}.panel-danger>.panel-footer+.panel-collapse>.panel-body{border-bottom-color:#ebccd1}.embed-responsive{position:relative;display:block;height:0;padding:0;overflow:hidden}.embed-responsive .embed-responsive-item,.embed-responsive embed,.embed-responsive iframe,.embed-responsive object,.embed-responsive video{position:absolute;top:0;bottom:0;left:0;width:100%;height:100%;border:0}.embed-responsive-16by9{padding-bottom:56.25%}.embed-responsive-4by3{padding-bottom:75%}.well{min-height:20px;padding:19px;margin-bottom:20px;background-color:#f5f5f5;border:1px solid #e3e3e3;border-radius:4px;-webkit-box-shadow:inset 0 1px 1px rgba(0,0,0,.05);box-shadow:inset 0 1px 1px rgba(0,0,0,.05)}.well blockquote{border-color:#ddd;border-color:rgba(0,0,0,.15)}.well-lg{padding:24px;border-radius:6px}.well-sm{padding:9px;border-radius:3px}.close{float:right;font-size:21px;font-weight:700;line-height:1;color:#000;text-shadow:0 1px 0 #fff;filter:alpha(opacity=20);opacity:.2}.close:focus,.close:hover{color:#000;text-decoration:none;cursor:pointer;filter:alpha(opacity=50);opacity:.5}button.close{padding:0;cursor:pointer;background:0 0;border:0;-webkit-appearance:none;-moz-appearance:none;appearance:none}.modal-open{overflow:hidden}.modal{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1050;display:none;overflow:hidden;-webkit-overflow-scrolling:touch;outline:0}.modal.fade .modal-dialog{-webkit-transform:translate(0,-25%);-ms-transform:translate(0,-25%);-o-transform:translate(0,-25%);transform:translate(0,-25%);-webkit-transition:-webkit-transform .3s ease-out;-o-transition:-o-transform .3s ease-out;transition:-webkit-transform .3s ease-out;transition:transform .3s ease-out;transition:transform .3s ease-out,-webkit-transform .3s ease-out,-o-transform .3s ease-out}.modal.in .modal-dialog{-webkit-transform:translate(0,0);-ms-transform:translate(0,0);-o-transform:translate(0,0);transform:translate(0,0)}.modal-open .modal{overflow-x:hidden;overflow-y:auto}.modal-dialog{position:relative;width:auto;margin:10px}.modal-content{position:relative;background-color:#fff;background-clip:padding-box;border:1px solid #999;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 3px 9px rgba(0,0,0,.5);box-shadow:0 3px 9px rgba(0,0,0,.5);outline:0}.modal-backdrop{position:fixed;top:0;right:0;bottom:0;left:0;z-index:1040;background-color:#000}.modal-backdrop.fade{filter:alpha(opacity=0);opacity:0}.modal-backdrop.in{filter:alpha(opacity=50);opacity:.5}.modal-header{padding:15px;border-bottom:1px solid #e5e5e5}.modal-header .close{margin-top:-2px}.modal-title{margin:0;line-height:1.42857143}.modal-body{position:relative;padding:15px}.modal-footer{padding:15px;text-align:right;border-top:1px solid #e5e5e5}.modal-footer .btn+.btn{margin-bottom:0;margin-left:5px}.modal-footer .btn-group .btn+.btn{margin-left:-1px}.modal-footer .btn-block+.btn-block{margin-left:0}.modal-scrollbar-measure{position:absolute;top:-9999px;width:50px;height:50px;overflow:scroll}@media (min-width:768px){.modal-dialog{width:600px;margin:30px auto}.modal-content{-webkit-box-shadow:0 5px 15px rgba(0,0,0,.5);box-shadow:0 5px 15px rgba(0,0,0,.5)}.modal-sm{width:300px}}@media (min-width:992px){.modal-lg{width:900px}}.tooltip{position:absolute;z-index:1070;display:block;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-style:normal;font-weight:400;line-height:1.42857143;line-break:auto;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;font-size:12px;filter:alpha(opacity=0);opacity:0}.tooltip.in{filter:alpha(opacity=90);opacity:.9}.tooltip.top{padding:5px 0;margin-top:-3px}.tooltip.right{padding:0 5px;margin-left:3px}.tooltip.bottom{padding:5px 0;margin-top:3px}.tooltip.left{padding:0 5px;margin-left:-3px}.tooltip.top .tooltip-arrow{bottom:0;left:50%;margin-left:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-left .tooltip-arrow{right:5px;bottom:0;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.top-right .tooltip-arrow{bottom:0;left:5px;margin-bottom:-5px;border-width:5px 5px 0;border-top-color:#000}.tooltip.right .tooltip-arrow{top:50%;left:0;margin-top:-5px;border-width:5px 5px 5px 0;border-right-color:#000}.tooltip.left .tooltip-arrow{top:50%;right:0;margin-top:-5px;border-width:5px 0 5px 5px;border-left-color:#000}.tooltip.bottom .tooltip-arrow{top:0;left:50%;margin-left:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-left .tooltip-arrow{top:0;right:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip.bottom-right .tooltip-arrow{top:0;left:5px;margin-top:-5px;border-width:0 5px 5px;border-bottom-color:#000}.tooltip-inner{max-width:200px;padding:3px 8px;color:#fff;text-align:center;background-color:#000;border-radius:4px}.tooltip-arrow{position:absolute;width:0;height:0;border-color:transparent;border-style:solid}.popover{position:absolute;top:0;left:0;z-index:1060;display:none;max-width:276px;padding:1px;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;font-style:normal;font-weight:400;line-height:1.42857143;line-break:auto;text-align:left;text-align:start;text-decoration:none;text-shadow:none;text-transform:none;letter-spacing:normal;word-break:normal;word-spacing:normal;word-wrap:normal;white-space:normal;font-size:14px;background-color:#fff;background-clip:padding-box;border:1px solid #ccc;border:1px solid rgba(0,0,0,.2);border-radius:6px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,.2);box-shadow:0 5px 10px rgba(0,0,0,.2)}.popover.top{margin-top:-10px}.popover.right{margin-left:10px}.popover.bottom{margin-top:10px}.popover.left{margin-left:-10px}.popover>.arrow{border-width:11px}.popover>.arrow,.popover>.arrow:after{position:absolute;display:block;width:0;height:0;border-color:transparent;border-style:solid}.popover>.arrow:after{content:"";border-width:10px}.popover.top>.arrow{bottom:-11px;left:50%;margin-left:-11px;border-top-color:#999;border-top-color:rgba(0,0,0,.25);border-bottom-width:0}.popover.top>.arrow:after{bottom:1px;margin-left:-10px;content:" ";border-top-color:#fff;border-bottom-width:0}.popover.right>.arrow{top:50%;left:-11px;margin-top:-11px;border-right-color:#999;border-right-color:rgba(0,0,0,.25);border-left-width:0}.popover.right>.arrow:after{bottom:-10px;left:1px;content:" ";border-right-color:#fff;border-left-width:0}.popover.bottom>.arrow{top:-11px;left:50%;margin-left:-11px;border-top-width:0;border-bottom-color:#999;border-bottom-color:rgba(0,0,0,.25)}.popover.bottom>.arrow:after{top:1px;margin-left:-10px;content:" ";border-top-width:0;border-bottom-color:#fff}.popover.left>.arrow{top:50%;right:-11px;margin-top:-11px;border-right-width:0;border-left-color:#999;border-left-color:rgba(0,0,0,.25)}.popover.left>.arrow:after{right:1px;bottom:-10px;content:" ";border-right-width:0;border-left-color:#fff}.popover-title{padding:8px 14px;margin:0;font-size:14px;background-color:#f7f7f7;border-bottom:1px solid #ebebeb;border-radius:5px 5px 0 0}.popover-content{padding:9px 14px}.carousel{position:relative}.carousel-inner{position:relative;width:100%;overflow:hidden}.carousel-inner>.item{position:relative;display:none;-webkit-transition:.6s ease-in-out left;-o-transition:.6s ease-in-out left;transition:.6s ease-in-out left}.carousel-inner>.item>a>img,.carousel-inner>.item>img{line-height:1}@media all and (transform-3d),(-webkit-transform-3d){.carousel-inner>.item{-webkit-transition:-webkit-transform .6s ease-in-out;-o-transition:-o-transform .6s ease-in-out;transition:-webkit-transform .6s ease-in-out;transition:transform .6s ease-in-out;transition:transform .6s ease-in-out,-webkit-transform .6s ease-in-out,-o-transform .6s ease-in-out;-webkit-backface-visibility:hidden;backface-visibility:hidden;-webkit-perspective:1000px;perspective:1000px}.carousel-inner>.item.active.right,.carousel-inner>.item.next{-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0);left:0}.carousel-inner>.item.active.left,.carousel-inner>.item.prev{-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0);left:0}.carousel-inner>.item.active,.carousel-inner>.item.next.left,.carousel-inner>.item.prev.right{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0);left:0}}.carousel-inner>.active,.carousel-inner>.next,.carousel-inner>.prev{display:block}.carousel-inner>.active{left:0}.carousel-inner>.next,.carousel-inner>.prev{position:absolute;top:0;width:100%}.carousel-inner>.next{left:100%}.carousel-inner>.prev{left:-100%}.carousel-inner>.next.left,.carousel-inner>.prev.right{left:0}.carousel-inner>.active.left{left:-100%}.carousel-inner>.active.right{left:100%}.carousel-control{position:absolute;top:0;bottom:0;left:0;width:15%;font-size:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6);background-color:rgba(0,0,0,0);filter:alpha(opacity=50);opacity:.5}.carousel-control.left{background-image:-webkit-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.5)),to(rgba(0,0,0,.0001)));background-image:linear-gradient(to right,rgba(0,0,0,.5) 0,rgba(0,0,0,.0001) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);background-repeat:repeat-x}.carousel-control.right{right:0;left:auto;background-image:-webkit-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-o-linear-gradient(left,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);background-image:-webkit-gradient(linear,left top,right top,from(rgba(0,0,0,.0001)),to(rgba(0,0,0,.5)));background-image:linear-gradient(to right,rgba(0,0,0,.0001) 0,rgba(0,0,0,.5) 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);background-repeat:repeat-x}.carousel-control:focus,.carousel-control:hover{color:#fff;text-decoration:none;outline:0;filter:alpha(opacity=90);opacity:.9}.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{position:absolute;top:50%;z-index:5;display:inline-block;margin-top:-10px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{left:50%;margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{right:50%;margin-right:-10px}.carousel-control .icon-next,.carousel-control .icon-prev{width:20px;height:20px;font-family:serif;line-height:1}.carousel-control .icon-prev:before{content:"\2039"}.carousel-control .icon-next:before{content:"\203a"}.carousel-indicators{position:absolute;bottom:10px;left:50%;z-index:15;width:60%;padding-left:0;margin-left:-30%;text-align:center;list-style:none}.carousel-indicators li{display:inline-block;width:10px;height:10px;margin:1px;text-indent:-999px;cursor:pointer;background-color:#000\9;background-color:rgba(0,0,0,0);border:1px solid #fff;border-radius:10px}.carousel-indicators .active{width:12px;height:12px;margin:0;background-color:#fff}.carousel-caption{position:absolute;right:15%;bottom:20px;left:15%;z-index:10;padding-top:20px;padding-bottom:20px;color:#fff;text-align:center;text-shadow:0 1px 2px rgba(0,0,0,.6)}.carousel-caption .btn{text-shadow:none}@media screen and (min-width:768px){.carousel-control .glyphicon-chevron-left,.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next,.carousel-control .icon-prev{width:30px;height:30px;margin-top:-10px;font-size:30px}.carousel-control .glyphicon-chevron-left,.carousel-control .icon-prev{margin-left:-10px}.carousel-control .glyphicon-chevron-right,.carousel-control .icon-next{margin-right:-10px}.carousel-caption{right:20%;left:20%;padding-bottom:30px}.carousel-indicators{bottom:20px}}.btn-group-vertical>.btn-group:after,.btn-group-vertical>.btn-group:before,.btn-toolbar:after,.btn-toolbar:before,.clearfix:after,.clearfix:before,.container-fluid:after,.container-fluid:before,.container:after,.container:before,.dl-horizontal dd:after,.dl-horizontal dd:before,.form-horizontal .form-group:after,.form-horizontal .form-group:before,.modal-footer:after,.modal-footer:before,.modal-header:after,.modal-header:before,.nav:after,.nav:before,.navbar-collapse:after,.navbar-collapse:before,.navbar-header:after,.navbar-header:before,.navbar:after,.navbar:before,.pager:after,.pager:before,.panel-body:after,.panel-body:before,.row:after,.row:before{display:table;content:" "}.btn-group-vertical>.btn-group:after,.btn-toolbar:after,.clearfix:after,.container-fluid:after,.container:after,.dl-horizontal dd:after,.form-horizontal .form-group:after,.modal-footer:after,.modal-header:after,.nav:after,.navbar-collapse:after,.navbar-header:after,.navbar:after,.pager:after,.panel-body:after,.row:after{clear:both}.center-block{display:block;margin-right:auto;margin-left:auto}.pull-right{float:right!important}.pull-left{float:left!important}.hide{display:none!important}.show{display:block!important}.invisible{visibility:hidden}.text-hide{font:0/0 a;color:transparent;text-shadow:none;background-color:transparent;border:0}.hidden{display:none!important}.affix{position:fixed}@-ms-viewport{width:device-width}.visible-lg,.visible-md,.visible-sm,.visible-xs{display:none!important}.visible-lg-block,.visible-lg-inline,.visible-lg-inline-block,.visible-md-block,.visible-md-inline,.visible-md-inline-block,.visible-sm-block,.visible-sm-inline,.visible-sm-inline-block,.visible-xs-block,.visible-xs-inline,.visible-xs-inline-block{display:none!important}@media (max-width:767px){.visible-xs{display:block!important}table.visible-xs{display:table!important}tr.visible-xs{display:table-row!important}td.visible-xs,th.visible-xs{display:table-cell!important}}@media (max-width:767px){.visible-xs-block{display:block!important}}@media (max-width:767px){.visible-xs-inline{display:inline!important}}@media (max-width:767px){.visible-xs-inline-block{display:inline-block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm{display:block!important}table.visible-sm{display:table!important}tr.visible-sm{display:table-row!important}td.visible-sm,th.visible-sm{display:table-cell!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-block{display:block!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline{display:inline!important}}@media (min-width:768px) and (max-width:991px){.visible-sm-inline-block{display:inline-block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md{display:block!important}table.visible-md{display:table!important}tr.visible-md{display:table-row!important}td.visible-md,th.visible-md{display:table-cell!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-block{display:block!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline{display:inline!important}}@media (min-width:992px) and (max-width:1199px){.visible-md-inline-block{display:inline-block!important}}@media (min-width:1200px){.visible-lg{display:block!important}table.visible-lg{display:table!important}tr.visible-lg{display:table-row!important}td.visible-lg,th.visible-lg{display:table-cell!important}}@media (min-width:1200px){.visible-lg-block{display:block!important}}@media (min-width:1200px){.visible-lg-inline{display:inline!important}}@media (min-width:1200px){.visible-lg-inline-block{display:inline-block!important}}@media (max-width:767px){.hidden-xs{display:none!important}}@media (min-width:768px) and (max-width:991px){.hidden-sm{display:none!important}}@media (min-width:992px) and (max-width:1199px){.hidden-md{display:none!important}}@media (min-width:1200px){.hidden-lg{display:none!important}}.visible-print{display:none!important}@media print{.visible-print{display:block!important}table.visible-print{display:table!important}tr.visible-print{display:table-row!important}td.visible-print,th.visible-print{display:table-cell!important}}.visible-print-block{display:none!important}@media print{.visible-print-block{display:block!important}}.visible-print-inline{display:none!important}@media print{.visible-print-inline{display:inline!important}}.visible-print-inline-block{display:none!important}@media print{.visible-print-inline-block{display:inline-block!important}}@media print{.hidden-print{display:none!important}}
 /*# sourceMappingURL=bootstrap.min.css.map */
```

### Comparing `fookebox-0.7.3/fookebox/public/css/fonts/glyphicons-halflings-regular.eot` & `fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `fookebox-0.7.3/fookebox/public/css/fonts/glyphicons-halflings-regular.svg` & `fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `fookebox-0.7.3/fookebox/public/css/fonts/glyphicons-halflings-regular.ttf` & `fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `fookebox-0.7.3/fookebox/public/css/fonts/glyphicons-halflings-regular.woff` & `fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `fookebox-0.7.3/fookebox/public/css/fonts/glyphicons-halflings-regular.woff2` & `fookebox-1.0.0/src/fookebox/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `fookebox-0.7.3/fookebox/public/js/bootstrap/bootstrap.js` & `fookebox-1.0.0/src/fookebox/js/bootstrap.min.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,945 +1,1043 @@
 /*!
- * Bootstrap v3.3.6 (http://getbootstrap.com)
- * Copyright 2011-2015 Twitter, Inc.
+ * Bootstrap v3.4.1 (https://getbootstrap.com/)
+ * Copyright 2011-2019 Twitter, Inc.
  * Licensed under the MIT license
  */
-if ("undefined" == typeof jQuery) throw new Error("Bootstrap's JavaScript requires jQuery"); + function(a) {
+if ("undefined" == typeof jQuery) throw new Error("Bootstrap's JavaScript requires jQuery");
+! function(t) {
     "use strict";
-    var b = a.fn.jquery.split(" ")[0].split(".");
-    if (b[0] < 2 && b[1] < 9 || 1 == b[0] && 9 == b[1] && b[2] < 1 || b[0] > 2) throw new Error("Bootstrap's JavaScript requires jQuery version 1.9.1 or higher, but lower than version 3")
-}(jQuery), + function(a) {
+    var e = jQuery.fn.jquery.split(" ")[0].split(".");
+    if (e[0] < 2 && e[1] < 9 || 1 == e[0] && 9 == e[1] && e[2] < 1 || 3 < e[0]) throw new Error("Bootstrap's JavaScript requires jQuery version 1.9.1 or higher, but lower than version 4")
+}(),
+function(n) {
     "use strict";
-
-    function b() {
-        var a = document.createElement("bootstrap"),
-            b = {
-                WebkitTransition: "webkitTransitionEnd",
-                MozTransition: "transitionend",
-                OTransition: "oTransitionEnd otransitionend",
-                transition: "transitionend"
-            };
-        for (var c in b)
-            if (void 0 !== a.style[c]) return {
-                end: b[c]
-            };
-        return !1
-    }
-    a.fn.emulateTransitionEnd = function(b) {
-        var c = !1,
-            d = this;
-        a(this).one("bsTransitionEnd", function() {
-            c = !0
+    n.fn.emulateTransitionEnd = function(t) {
+        var e = !1,
+            i = this;
+        n(this).one("bsTransitionEnd", function() {
+            e = !0
         });
-        var e = function() {
-            c || a(d).trigger(a.support.transition.end)
-        };
-        return setTimeout(e, b), this
-    }, a(function() {
-        a.support.transition = b(), a.support.transition && (a.event.special.bsTransitionEnd = {
-            bindType: a.support.transition.end,
-            delegateType: a.support.transition.end,
-            handle: function(b) {
-                return a(b.target).is(this) ? b.handleObj.handler.apply(this, arguments) : void 0
+        return setTimeout(function() {
+            e || n(i).trigger(n.support.transition.end)
+        }, t), this
+    }, n(function() {
+        n.support.transition = function o() {
+            var t = document.createElement("bootstrap"),
+                e = {
+                    WebkitTransition: "webkitTransitionEnd",
+                    MozTransition: "transitionend",
+                    OTransition: "oTransitionEnd otransitionend",
+                    transition: "transitionend"
+                };
+            for (var i in e)
+                if (t.style[i] !== undefined) return {
+                    end: e[i]
+                };
+            return !1
+        }(), n.support.transition && (n.event.special.bsTransitionEnd = {
+            bindType: n.support.transition.end,
+            delegateType: n.support.transition.end,
+            handle: function(t) {
+                if (n(t.target).is(this)) return t.handleObj.handler.apply(this, arguments)
             }
         })
     })
-}(jQuery), + function(a) {
+}(jQuery),
+function(s) {
     "use strict";
-
-    function b(b) {
-        return this.each(function() {
-            var c = a(this),
-                e = c.data("bs.alert");
-            e || c.data("bs.alert", e = new d(this)), "string" == typeof b && e[b].call(c)
-        })
-    }
-    var c = '[data-dismiss="alert"]',
-        d = function(b) {
-            a(b).on("click", c, this.close)
+    var e = '[data-dismiss="alert"]',
+        a = function(t) {
+            s(t).on("click", e, this.close)
         };
-    d.VERSION = "3.3.6", d.TRANSITION_DURATION = 150, d.prototype.close = function(b) {
-        function c() {
-            g.detach().trigger("closed.bs.alert").remove()
+    a.VERSION = "3.4.1", a.TRANSITION_DURATION = 150, a.prototype.close = function(t) {
+        var e = s(this),
+            i = e.attr("data-target");
+        i || (i = (i = e.attr("href")) && i.replace(/.*(?=#[^\s]*$)/, "")), i = "#" === i ? [] : i;
+        var o = s(document).find(i);
+
+        function n() {
+            o.detach().trigger("closed.bs.alert").remove()
         }
-        var e = a(this),
-            f = e.attr("data-target");
-        f || (f = e.attr("href"), f = f && f.replace(/.*(?=#[^\s]*$)/, ""));
-        var g = a(f);
-        b && b.preventDefault(), g.length || (g = e.closest(".alert")), g.trigger(b = a.Event("close.bs.alert")), b.isDefaultPrevented() || (g.removeClass("in"), a.support.transition && g.hasClass("fade") ? g.one("bsTransitionEnd", c).emulateTransitionEnd(d.TRANSITION_DURATION) : c())
+        t && t.preventDefault(), o.length || (o = e.closest(".alert")), o.trigger(t = s.Event("close.bs.alert")), t.isDefaultPrevented() || (o.removeClass("in"), s.support.transition && o.hasClass("fade") ? o.one("bsTransitionEnd", n).emulateTransitionEnd(a.TRANSITION_DURATION) : n())
     };
-    var e = a.fn.alert;
-    a.fn.alert = b, a.fn.alert.Constructor = d, a.fn.alert.noConflict = function() {
-        return a.fn.alert = e, this
-    }, a(document).on("click.bs.alert.data-api", c, d.prototype.close)
-}(jQuery), + function(a) {
+    var t = s.fn.alert;
+    s.fn.alert = function o(i) {
+        return this.each(function() {
+            var t = s(this),
+                e = t.data("bs.alert");
+            e || t.data("bs.alert", e = new a(this)), "string" == typeof i && e[i].call(t)
+        })
+    }, s.fn.alert.Constructor = a, s.fn.alert.noConflict = function() {
+        return s.fn.alert = t, this
+    }, s(document).on("click.bs.alert.data-api", e, a.prototype.close)
+}(jQuery),
+function(s) {
     "use strict";
+    var n = function(t, e) {
+        this.$element = s(t), this.options = s.extend({}, n.DEFAULTS, e), this.isLoading = !1
+    };
 
-    function b(b) {
+    function i(o) {
         return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.button"),
-                f = "object" == typeof b && b;
-            e || d.data("bs.button", e = new c(this, f)), "toggle" == b ? e.toggle() : b && e.setState(b)
+            var t = s(this),
+                e = t.data("bs.button"),
+                i = "object" == typeof o && o;
+            e || t.data("bs.button", e = new n(this, i)), "toggle" == o ? e.toggle() : o && e.setState(o)
         })
     }
-    var c = function(b, d) {
-        this.$element = a(b), this.options = a.extend({}, c.DEFAULTS, d), this.isLoading = !1
-    };
-    c.VERSION = "3.3.6", c.DEFAULTS = {
+    n.VERSION = "3.4.1", n.DEFAULTS = {
         loadingText: "loading..."
-    }, c.prototype.setState = function(b) {
-        var c = "disabled",
-            d = this.$element,
-            e = d.is("input") ? "val" : "html",
-            f = d.data();
-        b += "Text", null == f.resetText && d.data("resetText", d[e]()), setTimeout(a.proxy(function() {
-            d[e](null == f[b] ? this.options[b] : f[b]), "loadingText" == b ? (this.isLoading = !0, d.addClass(c).attr(c, c)) : this.isLoading && (this.isLoading = !1, d.removeClass(c).removeAttr(c))
+    }, n.prototype.setState = function(t) {
+        var e = "disabled",
+            i = this.$element,
+            o = i.is("input") ? "val" : "html",
+            n = i.data();
+        t += "Text", null == n.resetText && i.data("resetText", i[o]()), setTimeout(s.proxy(function() {
+            i[o](null == n[t] ? this.options[t] : n[t]), "loadingText" == t ? (this.isLoading = !0, i.addClass(e).attr(e, e).prop(e, !0)) : this.isLoading && (this.isLoading = !1, i.removeClass(e).removeAttr(e).prop(e, !1))
         }, this), 0)
-    }, c.prototype.toggle = function() {
-        var a = !0,
-            b = this.$element.closest('[data-toggle="buttons"]');
-        if (b.length) {
-            var c = this.$element.find("input");
-            "radio" == c.prop("type") ? (c.prop("checked") && (a = !1), b.find(".active").removeClass("active"), this.$element.addClass("active")) : "checkbox" == c.prop("type") && (c.prop("checked") !== this.$element.hasClass("active") && (a = !1), this.$element.toggleClass("active")), c.prop("checked", this.$element.hasClass("active")), a && c.trigger("change")
+    }, n.prototype.toggle = function() {
+        var t = !0,
+            e = this.$element.closest('[data-toggle="buttons"]');
+        if (e.length) {
+            var i = this.$element.find("input");
+            "radio" == i.prop("type") ? (i.prop("checked") && (t = !1), e.find(".active").removeClass("active"), this.$element.addClass("active")) : "checkbox" == i.prop("type") && (i.prop("checked") !== this.$element.hasClass("active") && (t = !1), this.$element.toggleClass("active")), i.prop("checked", this.$element.hasClass("active")), t && i.trigger("change")
         } else this.$element.attr("aria-pressed", !this.$element.hasClass("active")), this.$element.toggleClass("active")
     };
-    var d = a.fn.button;
-    a.fn.button = b, a.fn.button.Constructor = c, a.fn.button.noConflict = function() {
-        return a.fn.button = d, this
-    }, a(document).on("click.bs.button.data-api", '[data-toggle^="button"]', function(c) {
-        var d = a(c.target);
-        d.hasClass("btn") || (d = d.closest(".btn")), b.call(d, "toggle"), a(c.target).is('input[type="radio"]') || a(c.target).is('input[type="checkbox"]') || c.preventDefault()
-    }).on("focus.bs.button.data-api blur.bs.button.data-api", '[data-toggle^="button"]', function(b) {
-        a(b.target).closest(".btn").toggleClass("focus", /^focus(in)?$/.test(b.type))
+    var t = s.fn.button;
+    s.fn.button = i, s.fn.button.Constructor = n, s.fn.button.noConflict = function() {
+        return s.fn.button = t, this
+    }, s(document).on("click.bs.button.data-api", '[data-toggle^="button"]', function(t) {
+        var e = s(t.target).closest(".btn");
+        i.call(e, "toggle"), s(t.target).is('input[type="radio"], input[type="checkbox"]') || (t.preventDefault(), e.is("input,button") ? e.trigger("focus") : e.find("input:visible,button:visible").first().trigger("focus"))
+    }).on("focus.bs.button.data-api blur.bs.button.data-api", '[data-toggle^="button"]', function(t) {
+        s(t.target).closest(".btn").toggleClass("focus", /^focus(in)?$/.test(t.type))
     })
-}(jQuery), + function(a) {
+}(jQuery),
+function(p) {
     "use strict";
+    var c = function(t, e) {
+        this.$element = p(t), this.$indicators = this.$element.find(".carousel-indicators"), this.options = e, this.paused = null, this.sliding = null, this.interval = null, this.$active = null, this.$items = null, this.options.keyboard && this.$element.on("keydown.bs.carousel", p.proxy(this.keydown, this)), "hover" == this.options.pause && !("ontouchstart" in document.documentElement) && this.$element.on("mouseenter.bs.carousel", p.proxy(this.pause, this)).on("mouseleave.bs.carousel", p.proxy(this.cycle, this))
+    };
 
-    function b(b) {
+    function r(n) {
         return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.carousel"),
-                f = a.extend({}, c.DEFAULTS, d.data(), "object" == typeof b && b),
-                g = "string" == typeof b ? b : f.slide;
-            e || d.data("bs.carousel", e = new c(this, f)), "number" == typeof b ? e.to(b) : g ? e[g]() : f.interval && e.pause().cycle()
+            var t = p(this),
+                e = t.data("bs.carousel"),
+                i = p.extend({}, c.DEFAULTS, t.data(), "object" == typeof n && n),
+                o = "string" == typeof n ? n : i.slide;
+            e || t.data("bs.carousel", e = new c(this, i)), "number" == typeof n ? e.to(n) : o ? e[o]() : i.interval && e.pause().cycle()
         })
     }
-    var c = function(b, c) {
-        this.$element = a(b), this.$indicators = this.$element.find(".carousel-indicators"), this.options = c, this.paused = null, this.sliding = null, this.interval = null, this.$active = null, this.$items = null, this.options.keyboard && this.$element.on("keydown.bs.carousel", a.proxy(this.keydown, this)), "hover" == this.options.pause && !("ontouchstart" in document.documentElement) && this.$element.on("mouseenter.bs.carousel", a.proxy(this.pause, this)).on("mouseleave.bs.carousel", a.proxy(this.cycle, this))
-    };
-    c.VERSION = "3.3.6", c.TRANSITION_DURATION = 600, c.DEFAULTS = {
+    c.VERSION = "3.4.1", c.TRANSITION_DURATION = 600, c.DEFAULTS = {
         interval: 5e3,
         pause: "hover",
         wrap: !0,
         keyboard: !0
-    }, c.prototype.keydown = function(a) {
-        if (!/input|textarea/i.test(a.target.tagName)) {
-            switch (a.which) {
+    }, c.prototype.keydown = function(t) {
+        if (!/input|textarea/i.test(t.target.tagName)) {
+            switch (t.which) {
                 case 37:
                     this.prev();
                     break;
                 case 39:
                     this.next();
                     break;
                 default:
                     return
             }
-            a.preventDefault()
+            t.preventDefault()
         }
-    }, c.prototype.cycle = function(b) {
-        return b || (this.paused = !1), this.interval && clearInterval(this.interval), this.options.interval && !this.paused && (this.interval = setInterval(a.proxy(this.next, this), this.options.interval)), this
-    }, c.prototype.getItemIndex = function(a) {
-        return this.$items = a.parent().children(".item"), this.$items.index(a || this.$active)
-    }, c.prototype.getItemForDirection = function(a, b) {
-        var c = this.getItemIndex(b),
-            d = "prev" == a && 0 === c || "next" == a && c == this.$items.length - 1;
-        if (d && !this.options.wrap) return b;
-        var e = "prev" == a ? -1 : 1,
-            f = (c + e) % this.$items.length;
-        return this.$items.eq(f)
-    }, c.prototype.to = function(a) {
-        var b = this,
-            c = this.getItemIndex(this.$active = this.$element.find(".item.active"));
-        return a > this.$items.length - 1 || 0 > a ? void 0 : this.sliding ? this.$element.one("slid.bs.carousel", function() {
-            b.to(a)
-        }) : c == a ? this.pause().cycle() : this.slide(a > c ? "next" : "prev", this.$items.eq(a))
-    }, c.prototype.pause = function(b) {
-        return b || (this.paused = !0), this.$element.find(".next, .prev").length && a.support.transition && (this.$element.trigger(a.support.transition.end), this.cycle(!0)), this.interval = clearInterval(this.interval), this
+    }, c.prototype.cycle = function(t) {
+        return t || (this.paused = !1), this.interval && clearInterval(this.interval), this.options.interval && !this.paused && (this.interval = setInterval(p.proxy(this.next, this), this.options.interval)), this
+    }, c.prototype.getItemIndex = function(t) {
+        return this.$items = t.parent().children(".item"), this.$items.index(t || this.$active)
+    }, c.prototype.getItemForDirection = function(t, e) {
+        var i = this.getItemIndex(e);
+        if (("prev" == t && 0 === i || "next" == t && i == this.$items.length - 1) && !this.options.wrap) return e;
+        var o = (i + ("prev" == t ? -1 : 1)) % this.$items.length;
+        return this.$items.eq(o)
+    }, c.prototype.to = function(t) {
+        var e = this,
+            i = this.getItemIndex(this.$active = this.$element.find(".item.active"));
+        if (!(t > this.$items.length - 1 || t < 0)) return this.sliding ? this.$element.one("slid.bs.carousel", function() {
+            e.to(t)
+        }) : i == t ? this.pause().cycle() : this.slide(i < t ? "next" : "prev", this.$items.eq(t))
+    }, c.prototype.pause = function(t) {
+        return t || (this.paused = !0), this.$element.find(".next, .prev").length && p.support.transition && (this.$element.trigger(p.support.transition.end), this.cycle(!0)), this.interval = clearInterval(this.interval), this
     }, c.prototype.next = function() {
-        return this.sliding ? void 0 : this.slide("next")
+        if (!this.sliding) return this.slide("next")
     }, c.prototype.prev = function() {
-        return this.sliding ? void 0 : this.slide("prev")
-    }, c.prototype.slide = function(b, d) {
-        var e = this.$element.find(".item.active"),
-            f = d || this.getItemForDirection(b, e),
-            g = this.interval,
-            h = "next" == b ? "left" : "right",
-            i = this;
-        if (f.hasClass("active")) return this.sliding = !1;
-        var j = f[0],
-            k = a.Event("slide.bs.carousel", {
-                relatedTarget: j,
-                direction: h
+        if (!this.sliding) return this.slide("prev")
+    }, c.prototype.slide = function(t, e) {
+        var i = this.$element.find(".item.active"),
+            o = e || this.getItemForDirection(t, i),
+            n = this.interval,
+            s = "next" == t ? "left" : "right",
+            a = this;
+        if (o.hasClass("active")) return this.sliding = !1;
+        var r = o[0],
+            l = p.Event("slide.bs.carousel", {
+                relatedTarget: r,
+                direction: s
             });
-        if (this.$element.trigger(k), !k.isDefaultPrevented()) {
-            if (this.sliding = !0, g && this.pause(), this.$indicators.length) {
+        if (this.$element.trigger(l), !l.isDefaultPrevented()) {
+            if (this.sliding = !0, n && this.pause(), this.$indicators.length) {
                 this.$indicators.find(".active").removeClass("active");
-                var l = a(this.$indicators.children()[this.getItemIndex(f)]);
-                l && l.addClass("active")
+                var h = p(this.$indicators.children()[this.getItemIndex(o)]);
+                h && h.addClass("active")
             }
-            var m = a.Event("slid.bs.carousel", {
-                relatedTarget: j,
-                direction: h
+            var d = p.Event("slid.bs.carousel", {
+                relatedTarget: r,
+                direction: s
             });
-            return a.support.transition && this.$element.hasClass("slide") ? (f.addClass(b), f[0].offsetWidth, e.addClass(h), f.addClass(h), e.one("bsTransitionEnd", function() {
-                f.removeClass([b, h].join(" ")).addClass("active"), e.removeClass(["active", h].join(" ")), i.sliding = !1, setTimeout(function() {
-                    i.$element.trigger(m)
+            return p.support.transition && this.$element.hasClass("slide") ? (o.addClass(t), "object" == typeof o && o.length && o[0].offsetWidth, i.addClass(s), o.addClass(s), i.one("bsTransitionEnd", function() {
+                o.removeClass([t, s].join(" ")).addClass("active"), i.removeClass(["active", s].join(" ")), a.sliding = !1, setTimeout(function() {
+                    a.$element.trigger(d)
                 }, 0)
-            }).emulateTransitionEnd(c.TRANSITION_DURATION)) : (e.removeClass("active"), f.addClass("active"), this.sliding = !1, this.$element.trigger(m)), g && this.cycle(), this
+            }).emulateTransitionEnd(c.TRANSITION_DURATION)) : (i.removeClass("active"), o.addClass("active"), this.sliding = !1, this.$element.trigger(d)), n && this.cycle(), this
         }
     };
-    var d = a.fn.carousel;
-    a.fn.carousel = b, a.fn.carousel.Constructor = c, a.fn.carousel.noConflict = function() {
-        return a.fn.carousel = d, this
-    };
-    var e = function(c) {
-        var d, e = a(this),
-            f = a(e.attr("data-target") || (d = e.attr("href")) && d.replace(/.*(?=#[^\s]+$)/, ""));
-        if (f.hasClass("carousel")) {
-            var g = a.extend({}, f.data(), e.data()),
-                h = e.attr("data-slide-to");
-            h && (g.interval = !1), b.call(f, g), h && f.data("bs.carousel").to(h), c.preventDefault()
-        }
-    };
-    a(document).on("click.bs.carousel.data-api", "[data-slide]", e).on("click.bs.carousel.data-api", "[data-slide-to]", e), a(window).on("load", function() {
-        a('[data-ride="carousel"]').each(function() {
-            var c = a(this);
-            b.call(c, c.data())
+    var t = p.fn.carousel;
+    p.fn.carousel = r, p.fn.carousel.Constructor = c, p.fn.carousel.noConflict = function() {
+        return p.fn.carousel = t, this
+    };
+    var e = function(t) {
+        var e = p(this),
+            i = e.attr("href");
+        i && (i = i.replace(/.*(?=#[^\s]+$)/, ""));
+        var o = e.attr("data-target") || i,
+            n = p(document).find(o);
+        if (n.hasClass("carousel")) {
+            var s = p.extend({}, n.data(), e.data()),
+                a = e.attr("data-slide-to");
+            a && (s.interval = !1), r.call(n, s), a && n.data("bs.carousel").to(a), t.preventDefault()
+        }
+    };
+    p(document).on("click.bs.carousel.data-api", "[data-slide]", e).on("click.bs.carousel.data-api", "[data-slide-to]", e), p(window).on("load", function() {
+        p('[data-ride="carousel"]').each(function() {
+            var t = p(this);
+            r.call(t, t.data())
         })
     })
-}(jQuery), + function(a) {
+}(jQuery),
+function(a) {
     "use strict";
+    var r = function(t, e) {
+        this.$element = a(t), this.options = a.extend({}, r.DEFAULTS, e), this.$trigger = a('[data-toggle="collapse"][href="#' + t.id + '"],[data-toggle="collapse"][data-target="#' + t.id + '"]'), this.transitioning = null, this.options.parent ? this.$parent = this.getParent() : this.addAriaAndCollapsedClass(this.$element, this.$trigger), this.options.toggle && this.toggle()
+    };
 
-    function b(b) {
-        var c, d = b.attr("data-target") || (c = b.attr("href")) && c.replace(/.*(?=#[^\s]+$)/, "");
-        return a(d)
+    function n(t) {
+        var e, i = t.attr("data-target") || (e = t.attr("href")) && e.replace(/.*(?=#[^\s]+$)/, "");
+        return a(document).find(i)
     }
 
-    function c(b) {
+    function l(o) {
         return this.each(function() {
-            var c = a(this),
-                e = c.data("bs.collapse"),
-                f = a.extend({}, d.DEFAULTS, c.data(), "object" == typeof b && b);
-            !e && f.toggle && /show|hide/.test(b) && (f.toggle = !1), e || c.data("bs.collapse", e = new d(this, f)), "string" == typeof b && e[b]()
+            var t = a(this),
+                e = t.data("bs.collapse"),
+                i = a.extend({}, r.DEFAULTS, t.data(), "object" == typeof o && o);
+            !e && i.toggle && /show|hide/.test(o) && (i.toggle = !1), e || t.data("bs.collapse", e = new r(this, i)), "string" == typeof o && e[o]()
         })
     }
-    var d = function(b, c) {
-        this.$element = a(b), this.options = a.extend({}, d.DEFAULTS, c), this.$trigger = a('[data-toggle="collapse"][href="#' + b.id + '"],[data-toggle="collapse"][data-target="#' + b.id + '"]'), this.transitioning = null, this.options.parent ? this.$parent = this.getParent() : this.addAriaAndCollapsedClass(this.$element, this.$trigger), this.options.toggle && this.toggle()
-    };
-    d.VERSION = "3.3.6", d.TRANSITION_DURATION = 350, d.DEFAULTS = {
+    r.VERSION = "3.4.1", r.TRANSITION_DURATION = 350, r.DEFAULTS = {
         toggle: !0
-    }, d.prototype.dimension = function() {
-        var a = this.$element.hasClass("width");
-        return a ? "width" : "height"
-    }, d.prototype.show = function() {
+    }, r.prototype.dimension = function() {
+        return this.$element.hasClass("width") ? "width" : "height"
+    }, r.prototype.show = function() {
         if (!this.transitioning && !this.$element.hasClass("in")) {
-            var b, e = this.$parent && this.$parent.children(".panel").children(".in, .collapsing");
-            if (!(e && e.length && (b = e.data("bs.collapse"), b && b.transitioning))) {
-                var f = a.Event("show.bs.collapse");
-                if (this.$element.trigger(f), !f.isDefaultPrevented()) {
-                    e && e.length && (c.call(e, "hide"), b || e.data("bs.collapse", null));
-                    var g = this.dimension();
-                    this.$element.removeClass("collapse").addClass("collapsing")[g](0).attr("aria-expanded", !0), this.$trigger.removeClass("collapsed").attr("aria-expanded", !0), this.transitioning = 1;
-                    var h = function() {
-                        this.$element.removeClass("collapsing").addClass("collapse in")[g](""), this.transitioning = 0, this.$element.trigger("shown.bs.collapse")
+            var t, e = this.$parent && this.$parent.children(".panel").children(".in, .collapsing");
+            if (!(e && e.length && (t = e.data("bs.collapse")) && t.transitioning)) {
+                var i = a.Event("show.bs.collapse");
+                if (this.$element.trigger(i), !i.isDefaultPrevented()) {
+                    e && e.length && (l.call(e, "hide"), t || e.data("bs.collapse", null));
+                    var o = this.dimension();
+                    this.$element.removeClass("collapse").addClass("collapsing")[o](0).attr("aria-expanded", !0), this.$trigger.removeClass("collapsed").attr("aria-expanded", !0), this.transitioning = 1;
+                    var n = function() {
+                        this.$element.removeClass("collapsing").addClass("collapse in")[o](""), this.transitioning = 0, this.$element.trigger("shown.bs.collapse")
                     };
-                    if (!a.support.transition) return h.call(this);
-                    var i = a.camelCase(["scroll", g].join("-"));
-                    this.$element.one("bsTransitionEnd", a.proxy(h, this)).emulateTransitionEnd(d.TRANSITION_DURATION)[g](this.$element[0][i])
+                    if (!a.support.transition) return n.call(this);
+                    var s = a.camelCase(["scroll", o].join("-"));
+                    this.$element.one("bsTransitionEnd", a.proxy(n, this)).emulateTransitionEnd(r.TRANSITION_DURATION)[o](this.$element[0][s])
                 }
             }
         }
-    }, d.prototype.hide = function() {
+    }, r.prototype.hide = function() {
         if (!this.transitioning && this.$element.hasClass("in")) {
-            var b = a.Event("hide.bs.collapse");
-            if (this.$element.trigger(b), !b.isDefaultPrevented()) {
-                var c = this.dimension();
-                this.$element[c](this.$element[c]())[0].offsetHeight, this.$element.addClass("collapsing").removeClass("collapse in").attr("aria-expanded", !1), this.$trigger.addClass("collapsed").attr("aria-expanded", !1), this.transitioning = 1;
-                var e = function() {
+            var t = a.Event("hide.bs.collapse");
+            if (this.$element.trigger(t), !t.isDefaultPrevented()) {
+                var e = this.dimension();
+                this.$element[e](this.$element[e]())[0].offsetHeight, this.$element.addClass("collapsing").removeClass("collapse in").attr("aria-expanded", !1), this.$trigger.addClass("collapsed").attr("aria-expanded", !1), this.transitioning = 1;
+                var i = function() {
                     this.transitioning = 0, this.$element.removeClass("collapsing").addClass("collapse").trigger("hidden.bs.collapse")
                 };
-                return a.support.transition ? void this.$element[c](0).one("bsTransitionEnd", a.proxy(e, this)).emulateTransitionEnd(d.TRANSITION_DURATION) : e.call(this)
+                if (!a.support.transition) return i.call(this);
+                this.$element[e](0).one("bsTransitionEnd", a.proxy(i, this)).emulateTransitionEnd(r.TRANSITION_DURATION)
             }
         }
-    }, d.prototype.toggle = function() {
+    }, r.prototype.toggle = function() {
         this[this.$element.hasClass("in") ? "hide" : "show"]()
-    }, d.prototype.getParent = function() {
-        return a(this.options.parent).find('[data-toggle="collapse"][data-parent="' + this.options.parent + '"]').each(a.proxy(function(c, d) {
-            var e = a(d);
-            this.addAriaAndCollapsedClass(b(e), e)
+    }, r.prototype.getParent = function() {
+        return a(document).find(this.options.parent).find('[data-toggle="collapse"][data-parent="' + this.options.parent + '"]').each(a.proxy(function(t, e) {
+            var i = a(e);
+            this.addAriaAndCollapsedClass(n(i), i)
         }, this)).end()
-    }, d.prototype.addAriaAndCollapsedClass = function(a, b) {
-        var c = a.hasClass("in");
-        a.attr("aria-expanded", c), b.toggleClass("collapsed", !c).attr("aria-expanded", c)
-    };
-    var e = a.fn.collapse;
-    a.fn.collapse = c, a.fn.collapse.Constructor = d, a.fn.collapse.noConflict = function() {
-        return a.fn.collapse = e, this
-    }, a(document).on("click.bs.collapse.data-api", '[data-toggle="collapse"]', function(d) {
+    }, r.prototype.addAriaAndCollapsedClass = function(t, e) {
+        var i = t.hasClass("in");
+        t.attr("aria-expanded", i), e.toggleClass("collapsed", !i).attr("aria-expanded", i)
+    };
+    var t = a.fn.collapse;
+    a.fn.collapse = l, a.fn.collapse.Constructor = r, a.fn.collapse.noConflict = function() {
+        return a.fn.collapse = t, this
+    }, a(document).on("click.bs.collapse.data-api", '[data-toggle="collapse"]', function(t) {
         var e = a(this);
-        e.attr("data-target") || d.preventDefault();
-        var f = b(e),
-            g = f.data("bs.collapse"),
-            h = g ? "toggle" : e.data();
-        c.call(f, h)
+        e.attr("data-target") || t.preventDefault();
+        var i = n(e),
+            o = i.data("bs.collapse") ? "toggle" : e.data();
+        l.call(i, o)
     })
-}(jQuery), + function(a) {
+}(jQuery),
+function(a) {
     "use strict";
+    var r = '[data-toggle="dropdown"]',
+        o = function(t) {
+            a(t).on("click.bs.dropdown", this.toggle)
+        };
 
-    function b(b) {
-        var c = b.attr("data-target");
-        c || (c = b.attr("href"), c = c && /#[A-Za-z]/.test(c) && c.replace(/.*(?=#[^\s]*$)/, ""));
-        var d = c && a(c);
-        return d && d.length ? d : b.parent()
+    function l(t) {
+        var e = t.attr("data-target");
+        e || (e = (e = t.attr("href")) && /#[A-Za-z]/.test(e) && e.replace(/.*(?=#[^\s]*$)/, ""));
+        var i = "#" !== e ? a(document).find(e) : null;
+        return i && i.length ? i : t.parent()
     }
 
-    function c(c) {
-        c && 3 === c.which || (a(e).remove(), a(f).each(function() {
-            var d = a(this),
-                e = b(d),
-                f = {
+    function s(o) {
+        o && 3 === o.which || (a(".dropdown-backdrop").remove(), a(r).each(function() {
+            var t = a(this),
+                e = l(t),
+                i = {
                     relatedTarget: this
                 };
-            e.hasClass("open") && (c && "click" == c.type && /input|textarea/i.test(c.target.tagName) && a.contains(e[0], c.target) || (e.trigger(c = a.Event("hide.bs.dropdown", f)), c.isDefaultPrevented() || (d.attr("aria-expanded", "false"), e.removeClass("open").trigger(a.Event("hidden.bs.dropdown", f)))))
+            e.hasClass("open") && (o && "click" == o.type && /input|textarea/i.test(o.target.tagName) && a.contains(e[0], o.target) || (e.trigger(o = a.Event("hide.bs.dropdown", i)), o.isDefaultPrevented() || (t.attr("aria-expanded", "false"), e.removeClass("open").trigger(a.Event("hidden.bs.dropdown", i)))))
         }))
     }
-
-    function d(b) {
-        return this.each(function() {
-            var c = a(this),
-                d = c.data("bs.dropdown");
-            d || c.data("bs.dropdown", d = new g(this)), "string" == typeof b && d[b].call(c)
-        })
-    }
-    var e = ".dropdown-backdrop",
-        f = '[data-toggle="dropdown"]',
-        g = function(b) {
-            a(b).on("click.bs.dropdown", this.toggle)
-        };
-    g.VERSION = "3.3.6", g.prototype.toggle = function(d) {
+    o.VERSION = "3.4.1", o.prototype.toggle = function(t) {
         var e = a(this);
         if (!e.is(".disabled, :disabled")) {
-            var f = b(e),
-                g = f.hasClass("open");
-            if (c(), !g) {
-                "ontouchstart" in document.documentElement && !f.closest(".navbar-nav").length && a(document.createElement("div")).addClass("dropdown-backdrop").insertAfter(a(this)).on("click", c);
-                var h = {
+            var i = l(e),
+                o = i.hasClass("open");
+            if (s(), !o) {
+                "ontouchstart" in document.documentElement && !i.closest(".navbar-nav").length && a(document.createElement("div")).addClass("dropdown-backdrop").insertAfter(a(this)).on("click", s);
+                var n = {
                     relatedTarget: this
                 };
-                if (f.trigger(d = a.Event("show.bs.dropdown", h)), d.isDefaultPrevented()) return;
-                e.trigger("focus").attr("aria-expanded", "true"), f.toggleClass("open").trigger(a.Event("shown.bs.dropdown", h))
+                if (i.trigger(t = a.Event("show.bs.dropdown", n)), t.isDefaultPrevented()) return;
+                e.trigger("focus").attr("aria-expanded", "true"), i.toggleClass("open").trigger(a.Event("shown.bs.dropdown", n))
             }
             return !1
         }
-    }, g.prototype.keydown = function(c) {
-        if (/(38|40|27|32)/.test(c.which) && !/input|textarea/i.test(c.target.tagName)) {
-            var d = a(this);
-            if (c.preventDefault(), c.stopPropagation(), !d.is(".disabled, :disabled")) {
-                var e = b(d),
-                    g = e.hasClass("open");
-                if (!g && 27 != c.which || g && 27 == c.which) return 27 == c.which && e.find(f).trigger("focus"), d.trigger("click");
-                var h = " li:not(.disabled):visible a",
-                    i = e.find(".dropdown-menu" + h);
-                if (i.length) {
-                    var j = i.index(c.target);
-                    38 == c.which && j > 0 && j--, 40 == c.which && j < i.length - 1 && j++, ~j || (j = 0), i.eq(j).trigger("focus")
+    }, o.prototype.keydown = function(t) {
+        if (/(38|40|27|32)/.test(t.which) && !/input|textarea/i.test(t.target.tagName)) {
+            var e = a(this);
+            if (t.preventDefault(), t.stopPropagation(), !e.is(".disabled, :disabled")) {
+                var i = l(e),
+                    o = i.hasClass("open");
+                if (!o && 27 != t.which || o && 27 == t.which) return 27 == t.which && i.find(r).trigger("focus"), e.trigger("click");
+                var n = i.find(".dropdown-menu li:not(.disabled):visible a");
+                if (n.length) {
+                    var s = n.index(t.target);
+                    38 == t.which && 0 < s && s--, 40 == t.which && s < n.length - 1 && s++, ~s || (s = 0), n.eq(s).trigger("focus")
                 }
             }
         }
     };
-    var h = a.fn.dropdown;
-    a.fn.dropdown = d, a.fn.dropdown.Constructor = g, a.fn.dropdown.noConflict = function() {
-        return a.fn.dropdown = h, this
-    }, a(document).on("click.bs.dropdown.data-api", c).on("click.bs.dropdown.data-api", ".dropdown form", function(a) {
-        a.stopPropagation()
-    }).on("click.bs.dropdown.data-api", f, g.prototype.toggle).on("keydown.bs.dropdown.data-api", f, g.prototype.keydown).on("keydown.bs.dropdown.data-api", ".dropdown-menu", g.prototype.keydown)
-}(jQuery), + function(a) {
-    "use strict";
-
-    function b(b, d) {
+    var t = a.fn.dropdown;
+    a.fn.dropdown = function e(i) {
         return this.each(function() {
-            var e = a(this),
-                f = e.data("bs.modal"),
-                g = a.extend({}, c.DEFAULTS, e.data(), "object" == typeof b && b);
-            f || e.data("bs.modal", f = new c(this, g)), "string" == typeof b ? f[b](d) : g.show && f.show(d)
+            var t = a(this),
+                e = t.data("bs.dropdown");
+            e || t.data("bs.dropdown", e = new o(this)), "string" == typeof i && e[i].call(t)
         })
-    }
-    var c = function(b, c) {
-        this.options = c, this.$body = a(document.body), this.$element = a(b), this.$dialog = this.$element.find(".modal-dialog"), this.$backdrop = null, this.isShown = null, this.originalBodyPad = null, this.scrollbarWidth = 0, this.ignoreBackdropClick = !1, this.options.remote && this.$element.find(".modal-content").load(this.options.remote, a.proxy(function() {
+    }, a.fn.dropdown.Constructor = o, a.fn.dropdown.noConflict = function() {
+        return a.fn.dropdown = t, this
+    }, a(document).on("click.bs.dropdown.data-api", s).on("click.bs.dropdown.data-api", ".dropdown form", function(t) {
+        t.stopPropagation()
+    }).on("click.bs.dropdown.data-api", r, o.prototype.toggle).on("keydown.bs.dropdown.data-api", r, o.prototype.keydown).on("keydown.bs.dropdown.data-api", ".dropdown-menu", o.prototype.keydown)
+}(jQuery),
+function(a) {
+    "use strict";
+    var s = function(t, e) {
+        this.options = e, this.$body = a(document.body), this.$element = a(t), this.$dialog = this.$element.find(".modal-dialog"), this.$backdrop = null, this.isShown = null, this.originalBodyPad = null, this.scrollbarWidth = 0, this.ignoreBackdropClick = !1, this.fixedContent = ".navbar-fixed-top, .navbar-fixed-bottom", this.options.remote && this.$element.find(".modal-content").load(this.options.remote, a.proxy(function() {
             this.$element.trigger("loaded.bs.modal")
         }, this))
     };
-    c.VERSION = "3.3.6", c.TRANSITION_DURATION = 300, c.BACKDROP_TRANSITION_DURATION = 150, c.DEFAULTS = {
+
+    function r(o, n) {
+        return this.each(function() {
+            var t = a(this),
+                e = t.data("bs.modal"),
+                i = a.extend({}, s.DEFAULTS, t.data(), "object" == typeof o && o);
+            e || t.data("bs.modal", e = new s(this, i)), "string" == typeof o ? e[o](n) : i.show && e.show(n)
+        })
+    }
+    s.VERSION = "3.4.1", s.TRANSITION_DURATION = 300, s.BACKDROP_TRANSITION_DURATION = 150, s.DEFAULTS = {
         backdrop: !0,
         keyboard: !0,
         show: !0
-    }, c.prototype.toggle = function(a) {
-        return this.isShown ? this.hide() : this.show(a)
-    }, c.prototype.show = function(b) {
-        var d = this,
-            e = a.Event("show.bs.modal", {
-                relatedTarget: b
+    }, s.prototype.toggle = function(t) {
+        return this.isShown ? this.hide() : this.show(t)
+    }, s.prototype.show = function(i) {
+        var o = this,
+            t = a.Event("show.bs.modal", {
+                relatedTarget: i
             });
-        this.$element.trigger(e), this.isShown || e.isDefaultPrevented() || (this.isShown = !0, this.checkScrollbar(), this.setScrollbar(), this.$body.addClass("modal-open"), this.escape(), this.resize(), this.$element.on("click.dismiss.bs.modal", '[data-dismiss="modal"]', a.proxy(this.hide, this)), this.$dialog.on("mousedown.dismiss.bs.modal", function() {
-            d.$element.one("mouseup.dismiss.bs.modal", function(b) {
-                a(b.target).is(d.$element) && (d.ignoreBackdropClick = !0)
+        this.$element.trigger(t), this.isShown || t.isDefaultPrevented() || (this.isShown = !0, this.checkScrollbar(), this.setScrollbar(), this.$body.addClass("modal-open"), this.escape(), this.resize(), this.$element.on("click.dismiss.bs.modal", '[data-dismiss="modal"]', a.proxy(this.hide, this)), this.$dialog.on("mousedown.dismiss.bs.modal", function() {
+            o.$element.one("mouseup.dismiss.bs.modal", function(t) {
+                a(t.target).is(o.$element) && (o.ignoreBackdropClick = !0)
             })
         }), this.backdrop(function() {
-            var e = a.support.transition && d.$element.hasClass("fade");
-            d.$element.parent().length || d.$element.appendTo(d.$body), d.$element.show().scrollTop(0), d.adjustDialog(), e && d.$element[0].offsetWidth, d.$element.addClass("in"), d.enforceFocus();
-            var f = a.Event("shown.bs.modal", {
-                relatedTarget: b
+            var t = a.support.transition && o.$element.hasClass("fade");
+            o.$element.parent().length || o.$element.appendTo(o.$body), o.$element.show().scrollTop(0), o.adjustDialog(), t && o.$element[0].offsetWidth, o.$element.addClass("in"), o.enforceFocus();
+            var e = a.Event("shown.bs.modal", {
+                relatedTarget: i
             });
-            e ? d.$dialog.one("bsTransitionEnd", function() {
-                d.$element.trigger("focus").trigger(f)
-            }).emulateTransitionEnd(c.TRANSITION_DURATION) : d.$element.trigger("focus").trigger(f)
+            t ? o.$dialog.one("bsTransitionEnd", function() {
+                o.$element.trigger("focus").trigger(e)
+            }).emulateTransitionEnd(s.TRANSITION_DURATION) : o.$element.trigger("focus").trigger(e)
         }))
-    }, c.prototype.hide = function(b) {
-        b && b.preventDefault(), b = a.Event("hide.bs.modal"), this.$element.trigger(b), this.isShown && !b.isDefaultPrevented() && (this.isShown = !1, this.escape(), this.resize(), a(document).off("focusin.bs.modal"), this.$element.removeClass("in").off("click.dismiss.bs.modal").off("mouseup.dismiss.bs.modal"), this.$dialog.off("mousedown.dismiss.bs.modal"), a.support.transition && this.$element.hasClass("fade") ? this.$element.one("bsTransitionEnd", a.proxy(this.hideModal, this)).emulateTransitionEnd(c.TRANSITION_DURATION) : this.hideModal())
-    }, c.prototype.enforceFocus = function() {
-        a(document).off("focusin.bs.modal").on("focusin.bs.modal", a.proxy(function(a) {
-            this.$element[0] === a.target || this.$element.has(a.target).length || this.$element.trigger("focus")
+    }, s.prototype.hide = function(t) {
+        t && t.preventDefault(), t = a.Event("hide.bs.modal"), this.$element.trigger(t), this.isShown && !t.isDefaultPrevented() && (this.isShown = !1, this.escape(), this.resize(), a(document).off("focusin.bs.modal"), this.$element.removeClass("in").off("click.dismiss.bs.modal").off("mouseup.dismiss.bs.modal"), this.$dialog.off("mousedown.dismiss.bs.modal"), a.support.transition && this.$element.hasClass("fade") ? this.$element.one("bsTransitionEnd", a.proxy(this.hideModal, this)).emulateTransitionEnd(s.TRANSITION_DURATION) : this.hideModal())
+    }, s.prototype.enforceFocus = function() {
+        a(document).off("focusin.bs.modal").on("focusin.bs.modal", a.proxy(function(t) {
+            document === t.target || this.$element[0] === t.target || this.$element.has(t.target).length || this.$element.trigger("focus")
         }, this))
-    }, c.prototype.escape = function() {
-        this.isShown && this.options.keyboard ? this.$element.on("keydown.dismiss.bs.modal", a.proxy(function(a) {
-            27 == a.which && this.hide()
+    }, s.prototype.escape = function() {
+        this.isShown && this.options.keyboard ? this.$element.on("keydown.dismiss.bs.modal", a.proxy(function(t) {
+            27 == t.which && this.hide()
         }, this)) : this.isShown || this.$element.off("keydown.dismiss.bs.modal")
-    }, c.prototype.resize = function() {
+    }, s.prototype.resize = function() {
         this.isShown ? a(window).on("resize.bs.modal", a.proxy(this.handleUpdate, this)) : a(window).off("resize.bs.modal")
-    }, c.prototype.hideModal = function() {
-        var a = this;
+    }, s.prototype.hideModal = function() {
+        var t = this;
         this.$element.hide(), this.backdrop(function() {
-            a.$body.removeClass("modal-open"), a.resetAdjustments(), a.resetScrollbar(), a.$element.trigger("hidden.bs.modal")
+            t.$body.removeClass("modal-open"), t.resetAdjustments(), t.resetScrollbar(), t.$element.trigger("hidden.bs.modal")
         })
-    }, c.prototype.removeBackdrop = function() {
+    }, s.prototype.removeBackdrop = function() {
         this.$backdrop && this.$backdrop.remove(), this.$backdrop = null
-    }, c.prototype.backdrop = function(b) {
-        var d = this,
-            e = this.$element.hasClass("fade") ? "fade" : "";
+    }, s.prototype.backdrop = function(t) {
+        var e = this,
+            i = this.$element.hasClass("fade") ? "fade" : "";
         if (this.isShown && this.options.backdrop) {
-            var f = a.support.transition && e;
-            if (this.$backdrop = a(document.createElement("div")).addClass("modal-backdrop " + e).appendTo(this.$body), this.$element.on("click.dismiss.bs.modal", a.proxy(function(a) {
-                    return this.ignoreBackdropClick ? void(this.ignoreBackdropClick = !1) : void(a.target === a.currentTarget && ("static" == this.options.backdrop ? this.$element[0].focus() : this.hide()))
-                }, this)), f && this.$backdrop[0].offsetWidth, this.$backdrop.addClass("in"), !b) return;
-            f ? this.$backdrop.one("bsTransitionEnd", b).emulateTransitionEnd(c.BACKDROP_TRANSITION_DURATION) : b()
+            var o = a.support.transition && i;
+            if (this.$backdrop = a(document.createElement("div")).addClass("modal-backdrop " + i).appendTo(this.$body), this.$element.on("click.dismiss.bs.modal", a.proxy(function(t) {
+                    this.ignoreBackdropClick ? this.ignoreBackdropClick = !1 : t.target === t.currentTarget && ("static" == this.options.backdrop ? this.$element[0].focus() : this.hide())
+                }, this)), o && this.$backdrop[0].offsetWidth, this.$backdrop.addClass("in"), !t) return;
+            o ? this.$backdrop.one("bsTransitionEnd", t).emulateTransitionEnd(s.BACKDROP_TRANSITION_DURATION) : t()
         } else if (!this.isShown && this.$backdrop) {
             this.$backdrop.removeClass("in");
-            var g = function() {
-                d.removeBackdrop(), b && b()
+            var n = function() {
+                e.removeBackdrop(), t && t()
             };
-            a.support.transition && this.$element.hasClass("fade") ? this.$backdrop.one("bsTransitionEnd", g).emulateTransitionEnd(c.BACKDROP_TRANSITION_DURATION) : g()
-        } else b && b()
-    }, c.prototype.handleUpdate = function() {
+            a.support.transition && this.$element.hasClass("fade") ? this.$backdrop.one("bsTransitionEnd", n).emulateTransitionEnd(s.BACKDROP_TRANSITION_DURATION) : n()
+        } else t && t()
+    }, s.prototype.handleUpdate = function() {
         this.adjustDialog()
-    }, c.prototype.adjustDialog = function() {
-        var a = this.$element[0].scrollHeight > document.documentElement.clientHeight;
+    }, s.prototype.adjustDialog = function() {
+        var t = this.$element[0].scrollHeight > document.documentElement.clientHeight;
         this.$element.css({
-            paddingLeft: !this.bodyIsOverflowing && a ? this.scrollbarWidth : "",
-            paddingRight: this.bodyIsOverflowing && !a ? this.scrollbarWidth : ""
+            paddingLeft: !this.bodyIsOverflowing && t ? this.scrollbarWidth : "",
+            paddingRight: this.bodyIsOverflowing && !t ? this.scrollbarWidth : ""
         })
-    }, c.prototype.resetAdjustments = function() {
+    }, s.prototype.resetAdjustments = function() {
         this.$element.css({
             paddingLeft: "",
             paddingRight: ""
         })
-    }, c.prototype.checkScrollbar = function() {
-        var a = window.innerWidth;
-        if (!a) {
-            var b = document.documentElement.getBoundingClientRect();
-            a = b.right - Math.abs(b.left)
-        }
-        this.bodyIsOverflowing = document.body.clientWidth < a, this.scrollbarWidth = this.measureScrollbar()
-    }, c.prototype.setScrollbar = function() {
-        var a = parseInt(this.$body.css("padding-right") || 0, 10);
-        this.originalBodyPad = document.body.style.paddingRight || "", this.bodyIsOverflowing && this.$body.css("padding-right", a + this.scrollbarWidth)
-    }, c.prototype.resetScrollbar = function() {
-        this.$body.css("padding-right", this.originalBodyPad)
-    }, c.prototype.measureScrollbar = function() {
-        var a = document.createElement("div");
-        a.className = "modal-scrollbar-measure", this.$body.append(a);
-        var b = a.offsetWidth - a.clientWidth;
-        return this.$body[0].removeChild(a), b
-    };
-    var d = a.fn.modal;
-    a.fn.modal = b, a.fn.modal.Constructor = c, a.fn.modal.noConflict = function() {
-        return a.fn.modal = d, this
-    }, a(document).on("click.bs.modal.data-api", '[data-toggle="modal"]', function(c) {
-        var d = a(this),
-            e = d.attr("href"),
-            f = a(d.attr("data-target") || e && e.replace(/.*(?=#[^\s]+$)/, "")),
-            g = f.data("bs.modal") ? "toggle" : a.extend({
-                remote: !/#/.test(e) && e
-            }, f.data(), d.data());
-        d.is("a") && c.preventDefault(), f.one("show.bs.modal", function(a) {
-            a.isDefaultPrevented() || f.one("hidden.bs.modal", function() {
-                d.is(":visible") && d.trigger("focus")
+    }, s.prototype.checkScrollbar = function() {
+        var t = window.innerWidth;
+        if (!t) {
+            var e = document.documentElement.getBoundingClientRect();
+            t = e.right - Math.abs(e.left)
+        }
+        this.bodyIsOverflowing = document.body.clientWidth < t, this.scrollbarWidth = this.measureScrollbar()
+    }, s.prototype.setScrollbar = function() {
+        var t = parseInt(this.$body.css("padding-right") || 0, 10);
+        this.originalBodyPad = document.body.style.paddingRight || "";
+        var n = this.scrollbarWidth;
+        this.bodyIsOverflowing && (this.$body.css("padding-right", t + n), a(this.fixedContent).each(function(t, e) {
+            var i = e.style.paddingRight,
+                o = a(e).css("padding-right");
+            a(e).data("padding-right", i).css("padding-right", parseFloat(o) + n + "px")
+        }))
+    }, s.prototype.resetScrollbar = function() {
+        this.$body.css("padding-right", this.originalBodyPad), a(this.fixedContent).each(function(t, e) {
+            var i = a(e).data("padding-right");
+            a(e).removeData("padding-right"), e.style.paddingRight = i || ""
+        })
+    }, s.prototype.measureScrollbar = function() {
+        var t = document.createElement("div");
+        t.className = "modal-scrollbar-measure", this.$body.append(t);
+        var e = t.offsetWidth - t.clientWidth;
+        return this.$body[0].removeChild(t), e
+    };
+    var t = a.fn.modal;
+    a.fn.modal = r, a.fn.modal.Constructor = s, a.fn.modal.noConflict = function() {
+        return a.fn.modal = t, this
+    }, a(document).on("click.bs.modal.data-api", '[data-toggle="modal"]', function(t) {
+        var e = a(this),
+            i = e.attr("href"),
+            o = e.attr("data-target") || i && i.replace(/.*(?=#[^\s]+$)/, ""),
+            n = a(document).find(o),
+            s = n.data("bs.modal") ? "toggle" : a.extend({
+                remote: !/#/.test(i) && i
+            }, n.data(), e.data());
+        e.is("a") && t.preventDefault(), n.one("show.bs.modal", function(t) {
+            t.isDefaultPrevented() || n.one("hidden.bs.modal", function() {
+                e.is(":visible") && e.trigger("focus")
             })
-        }), b.call(f, g, this)
+        }), r.call(n, s, this)
     })
-}(jQuery), + function(a) {
+}(jQuery),
+function(g) {
     "use strict";
+    var o = ["sanitize", "whiteList", "sanitizeFn"],
+        a = ["background", "cite", "href", "itemtype", "longdesc", "poster", "src", "xlink:href"],
+        t = {
+            "*": ["class", "dir", "id", "lang", "role", /^aria-[\w-]*$/i],
+            a: ["target", "href", "title", "rel"],
+            area: [],
+            b: [],
+            br: [],
+            col: [],
+            code: [],
+            div: [],
+            em: [],
+            hr: [],
+            h1: [],
+            h2: [],
+            h3: [],
+            h4: [],
+            h5: [],
+            h6: [],
+            i: [],
+            img: ["src", "alt", "title", "width", "height"],
+            li: [],
+            ol: [],
+            p: [],
+            pre: [],
+            s: [],
+            small: [],
+            span: [],
+            sub: [],
+            sup: [],
+            strong: [],
+            u: [],
+            ul: []
+        },
+        r = /^(?:(?:https?|mailto|ftp|tel|file):|[^&:/?#]*(?:[/?#]|$))/gi,
+        l = /^data:(?:image\/(?:bmp|gif|jpeg|jpg|png|tiff|webp)|video\/(?:mpeg|mp4|ogg|webm)|audio\/(?:mp3|oga|ogg|opus));base64,[a-z0-9+/]+=*$/i;
 
-    function b(b) {
-        return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.tooltip"),
-                f = "object" == typeof b && b;
-            (e || !/destroy|hide/.test(b)) && (e || d.data("bs.tooltip", e = new c(this, f)), "string" == typeof b && e[b]())
-        })
+    function u(t, e) {
+        var i = t.nodeName.toLowerCase();
+        if (-1 !== g.inArray(i, e)) return -1 === g.inArray(i, a) || Boolean(t.nodeValue.match(r) || t.nodeValue.match(l));
+        for (var o = g(e).filter(function(t, e) {
+                return e instanceof RegExp
+            }), n = 0, s = o.length; n < s; n++)
+            if (i.match(o[n])) return !0;
+        return !1
     }
-    var c = function(a, b) {
-        this.type = null, this.options = null, this.enabled = null, this.timeout = null, this.hoverState = null, this.$element = null, this.inState = null, this.init("tooltip", a, b)
+
+    function n(t, e, i) {
+        if (0 === t.length) return t;
+        if (i && "function" == typeof i) return i(t);
+        if (!document.implementation || !document.implementation.createHTMLDocument) return t;
+        var o = document.implementation.createHTMLDocument("sanitization");
+        o.body.innerHTML = t;
+        for (var n = g.map(e, function(t, e) {
+                return e
+            }), s = g(o.body).find("*"), a = 0, r = s.length; a < r; a++) {
+            var l = s[a],
+                h = l.nodeName.toLowerCase();
+            if (-1 !== g.inArray(h, n))
+                for (var d = g.map(l.attributes, function(t) {
+                        return t
+                    }), p = [].concat(e["*"] || [], e[h] || []), c = 0, f = d.length; c < f; c++) u(d[c], p) || l.removeAttribute(d[c].nodeName);
+            else l.parentNode.removeChild(l)
+        }
+        return o.body.innerHTML
+    }
+    var m = function(t, e) {
+        this.type = null, this.options = null, this.enabled = null, this.timeout = null, this.hoverState = null, this.$element = null, this.inState = null, this.init("tooltip", t, e)
     };
-    c.VERSION = "3.3.6", c.TRANSITION_DURATION = 150, c.DEFAULTS = {
+    m.VERSION = "3.4.1", m.TRANSITION_DURATION = 150, m.DEFAULTS = {
         animation: !0,
         placement: "top",
         selector: !1,
         template: '<div class="tooltip" role="tooltip"><div class="tooltip-arrow"></div><div class="tooltip-inner"></div></div>',
         trigger: "hover focus",
         title: "",
         delay: 0,
         html: !1,
         container: !1,
         viewport: {
             selector: "body",
             padding: 0
-        }
-    }, c.prototype.init = function(b, c, d) {
-        if (this.enabled = !0, this.type = b, this.$element = a(c), this.options = this.getOptions(d), this.$viewport = this.options.viewport && a(a.isFunction(this.options.viewport) ? this.options.viewport.call(this, this.$element) : this.options.viewport.selector || this.options.viewport), this.inState = {
+        },
+        sanitize: !0,
+        sanitizeFn: null,
+        whiteList: t
+    }, m.prototype.init = function(t, e, i) {
+        if (this.enabled = !0, this.type = t, this.$element = g(e), this.options = this.getOptions(i), this.$viewport = this.options.viewport && g(document).find(g.isFunction(this.options.viewport) ? this.options.viewport.call(this, this.$element) : this.options.viewport.selector || this.options.viewport), this.inState = {
                 click: !1,
                 hover: !1,
                 focus: !1
             }, this.$element[0] instanceof document.constructor && !this.options.selector) throw new Error("`selector` option must be specified when initializing " + this.type + " on the window.document object!");
-        for (var e = this.options.trigger.split(" "), f = e.length; f--;) {
-            var g = e[f];
-            if ("click" == g) this.$element.on("click." + this.type, this.options.selector, a.proxy(this.toggle, this));
-            else if ("manual" != g) {
-                var h = "hover" == g ? "mouseenter" : "focusin",
-                    i = "hover" == g ? "mouseleave" : "focusout";
-                this.$element.on(h + "." + this.type, this.options.selector, a.proxy(this.enter, this)), this.$element.on(i + "." + this.type, this.options.selector, a.proxy(this.leave, this))
+        for (var o = this.options.trigger.split(" "), n = o.length; n--;) {
+            var s = o[n];
+            if ("click" == s) this.$element.on("click." + this.type, this.options.selector, g.proxy(this.toggle, this));
+            else if ("manual" != s) {
+                var a = "hover" == s ? "mouseenter" : "focusin",
+                    r = "hover" == s ? "mouseleave" : "focusout";
+                this.$element.on(a + "." + this.type, this.options.selector, g.proxy(this.enter, this)), this.$element.on(r + "." + this.type, this.options.selector, g.proxy(this.leave, this))
             }
         }
-        this.options.selector ? this._options = a.extend({}, this.options, {
+        this.options.selector ? this._options = g.extend({}, this.options, {
             trigger: "manual",
             selector: ""
         }) : this.fixTitle()
-    }, c.prototype.getDefaults = function() {
-        return c.DEFAULTS
-    }, c.prototype.getOptions = function(b) {
-        return b = a.extend({}, this.getDefaults(), this.$element.data(), b), b.delay && "number" == typeof b.delay && (b.delay = {
-            show: b.delay,
-            hide: b.delay
-        }), b
-    }, c.prototype.getDelegateOptions = function() {
-        var b = {},
-            c = this.getDefaults();
-        return this._options && a.each(this._options, function(a, d) {
-            c[a] != d && (b[a] = d)
-        }), b
-    }, c.prototype.enter = function(b) {
-        var c = b instanceof this.constructor ? b : a(b.currentTarget).data("bs." + this.type);
-        return c || (c = new this.constructor(b.currentTarget, this.getDelegateOptions()), a(b.currentTarget).data("bs." + this.type, c)), b instanceof a.Event && (c.inState["focusin" == b.type ? "focus" : "hover"] = !0), c.tip().hasClass("in") || "in" == c.hoverState ? void(c.hoverState = "in") : (clearTimeout(c.timeout), c.hoverState = "in", c.options.delay && c.options.delay.show ? void(c.timeout = setTimeout(function() {
-            "in" == c.hoverState && c.show()
-        }, c.options.delay.show)) : c.show())
-    }, c.prototype.isInStateTrue = function() {
-        for (var a in this.inState)
-            if (this.inState[a]) return !0;
+    }, m.prototype.getDefaults = function() {
+        return m.DEFAULTS
+    }, m.prototype.getOptions = function(t) {
+        var e = this.$element.data();
+        for (var i in e) e.hasOwnProperty(i) && -1 !== g.inArray(i, o) && delete e[i];
+        return (t = g.extend({}, this.getDefaults(), e, t)).delay && "number" == typeof t.delay && (t.delay = {
+            show: t.delay,
+            hide: t.delay
+        }), t.sanitize && (t.template = n(t.template, t.whiteList, t.sanitizeFn)), t
+    }, m.prototype.getDelegateOptions = function() {
+        var i = {},
+            o = this.getDefaults();
+        return this._options && g.each(this._options, function(t, e) {
+            o[t] != e && (i[t] = e)
+        }), i
+    }, m.prototype.enter = function(t) {
+        var e = t instanceof this.constructor ? t : g(t.currentTarget).data("bs." + this.type);
+        if (e || (e = new this.constructor(t.currentTarget, this.getDelegateOptions()), g(t.currentTarget).data("bs." + this.type, e)), t instanceof g.Event && (e.inState["focusin" == t.type ? "focus" : "hover"] = !0), e.tip().hasClass("in") || "in" == e.hoverState) e.hoverState = "in";
+        else {
+            if (clearTimeout(e.timeout), e.hoverState = "in", !e.options.delay || !e.options.delay.show) return e.show();
+            e.timeout = setTimeout(function() {
+                "in" == e.hoverState && e.show()
+            }, e.options.delay.show)
+        }
+    }, m.prototype.isInStateTrue = function() {
+        for (var t in this.inState)
+            if (this.inState[t]) return !0;
         return !1
-    }, c.prototype.leave = function(b) {
-        var c = b instanceof this.constructor ? b : a(b.currentTarget).data("bs." + this.type);
-        return c || (c = new this.constructor(b.currentTarget, this.getDelegateOptions()), a(b.currentTarget).data("bs." + this.type, c)), b instanceof a.Event && (c.inState["focusout" == b.type ? "focus" : "hover"] = !1), c.isInStateTrue() ? void 0 : (clearTimeout(c.timeout), c.hoverState = "out", c.options.delay && c.options.delay.hide ? void(c.timeout = setTimeout(function() {
-            "out" == c.hoverState && c.hide()
-        }, c.options.delay.hide)) : c.hide())
-    }, c.prototype.show = function() {
-        var b = a.Event("show.bs." + this.type);
+    }, m.prototype.leave = function(t) {
+        var e = t instanceof this.constructor ? t : g(t.currentTarget).data("bs." + this.type);
+        if (e || (e = new this.constructor(t.currentTarget, this.getDelegateOptions()), g(t.currentTarget).data("bs." + this.type, e)), t instanceof g.Event && (e.inState["focusout" == t.type ? "focus" : "hover"] = !1), !e.isInStateTrue()) {
+            if (clearTimeout(e.timeout), e.hoverState = "out", !e.options.delay || !e.options.delay.hide) return e.hide();
+            e.timeout = setTimeout(function() {
+                "out" == e.hoverState && e.hide()
+            }, e.options.delay.hide)
+        }
+    }, m.prototype.show = function() {
+        var t = g.Event("show.bs." + this.type);
         if (this.hasContent() && this.enabled) {
-            this.$element.trigger(b);
-            var d = a.contains(this.$element[0].ownerDocument.documentElement, this.$element[0]);
-            if (b.isDefaultPrevented() || !d) return;
-            var e = this,
-                f = this.tip(),
-                g = this.getUID(this.type);
-            this.setContent(), f.attr("id", g), this.$element.attr("aria-describedby", g), this.options.animation && f.addClass("fade");
-            var h = "function" == typeof this.options.placement ? this.options.placement.call(this, f[0], this.$element[0]) : this.options.placement,
-                i = /\s?auto?\s?/i,
-                j = i.test(h);
-            j && (h = h.replace(i, "") || "top"), f.detach().css({
+            this.$element.trigger(t);
+            var e = g.contains(this.$element[0].ownerDocument.documentElement, this.$element[0]);
+            if (t.isDefaultPrevented() || !e) return;
+            var i = this,
+                o = this.tip(),
+                n = this.getUID(this.type);
+            this.setContent(), o.attr("id", n), this.$element.attr("aria-describedby", n), this.options.animation && o.addClass("fade");
+            var s = "function" == typeof this.options.placement ? this.options.placement.call(this, o[0], this.$element[0]) : this.options.placement,
+                a = /\s?auto?\s?/i,
+                r = a.test(s);
+            r && (s = s.replace(a, "") || "top"), o.detach().css({
                 top: 0,
                 left: 0,
                 display: "block"
-            }).addClass(h).data("bs." + this.type, this), this.options.container ? f.appendTo(this.options.container) : f.insertAfter(this.$element), this.$element.trigger("inserted.bs." + this.type);
-            var k = this.getPosition(),
-                l = f[0].offsetWidth,
-                m = f[0].offsetHeight;
-            if (j) {
-                var n = h,
-                    o = this.getPosition(this.$viewport);
-                h = "bottom" == h && k.bottom + m > o.bottom ? "top" : "top" == h && k.top - m < o.top ? "bottom" : "right" == h && k.right + l > o.width ? "left" : "left" == h && k.left - l < o.left ? "right" : h, f.removeClass(n).addClass(h)
-            }
-            var p = this.getCalculatedOffset(h, k, l, m);
-            this.applyPlacement(p, h);
-            var q = function() {
-                var a = e.hoverState;
-                e.$element.trigger("shown.bs." + e.type), e.hoverState = null, "out" == a && e.leave(e)
+            }).addClass(s).data("bs." + this.type, this), this.options.container ? o.appendTo(g(document).find(this.options.container)) : o.insertAfter(this.$element), this.$element.trigger("inserted.bs." + this.type);
+            var l = this.getPosition(),
+                h = o[0].offsetWidth,
+                d = o[0].offsetHeight;
+            if (r) {
+                var p = s,
+                    c = this.getPosition(this.$viewport);
+                s = "bottom" == s && l.bottom + d > c.bottom ? "top" : "top" == s && l.top - d < c.top ? "bottom" : "right" == s && l.right + h > c.width ? "left" : "left" == s && l.left - h < c.left ? "right" : s, o.removeClass(p).addClass(s)
+            }
+            var f = this.getCalculatedOffset(s, l, h, d);
+            this.applyPlacement(f, s);
+            var u = function() {
+                var t = i.hoverState;
+                i.$element.trigger("shown.bs." + i.type), i.hoverState = null, "out" == t && i.leave(i)
             };
-            a.support.transition && this.$tip.hasClass("fade") ? f.one("bsTransitionEnd", q).emulateTransitionEnd(c.TRANSITION_DURATION) : q()
+            g.support.transition && this.$tip.hasClass("fade") ? o.one("bsTransitionEnd", u).emulateTransitionEnd(m.TRANSITION_DURATION) : u()
         }
-    }, c.prototype.applyPlacement = function(b, c) {
-        var d = this.tip(),
-            e = d[0].offsetWidth,
-            f = d[0].offsetHeight,
-            g = parseInt(d.css("margin-top"), 10),
-            h = parseInt(d.css("margin-left"), 10);
-        isNaN(g) && (g = 0), isNaN(h) && (h = 0), b.top += g, b.left += h, a.offset.setOffset(d[0], a.extend({
-            using: function(a) {
-                d.css({
-                    top: Math.round(a.top),
-                    left: Math.round(a.left)
+    }, m.prototype.applyPlacement = function(t, e) {
+        var i = this.tip(),
+            o = i[0].offsetWidth,
+            n = i[0].offsetHeight,
+            s = parseInt(i.css("margin-top"), 10),
+            a = parseInt(i.css("margin-left"), 10);
+        isNaN(s) && (s = 0), isNaN(a) && (a = 0), t.top += s, t.left += a, g.offset.setOffset(i[0], g.extend({
+            using: function(t) {
+                i.css({
+                    top: Math.round(t.top),
+                    left: Math.round(t.left)
                 })
             }
-        }, b), 0), d.addClass("in");
-        var i = d[0].offsetWidth,
-            j = d[0].offsetHeight;
-        "top" == c && j != f && (b.top = b.top + f - j);
-        var k = this.getViewportAdjustedDelta(c, b, i, j);
-        k.left ? b.left += k.left : b.top += k.top;
-        var l = /top|bottom/.test(c),
-            m = l ? 2 * k.left - e + i : 2 * k.top - f + j,
-            n = l ? "offsetWidth" : "offsetHeight";
-        d.offset(b), this.replaceArrow(m, d[0][n], l)
-    }, c.prototype.replaceArrow = function(a, b, c) {
-        this.arrow().css(c ? "left" : "top", 50 * (1 - a / b) + "%").css(c ? "top" : "left", "")
-    }, c.prototype.setContent = function() {
-        var a = this.tip(),
-            b = this.getTitle();
-        a.find(".tooltip-inner")[this.options.html ? "html" : "text"](b), a.removeClass("fade in top bottom left right")
-    }, c.prototype.hide = function(b) {
-        function d() {
-            "in" != e.hoverState && f.detach(), e.$element.removeAttr("aria-describedby").trigger("hidden.bs." + e.type), b && b()
-        }
+        }, t), 0), i.addClass("in");
+        var r = i[0].offsetWidth,
+            l = i[0].offsetHeight;
+        "top" == e && l != n && (t.top = t.top + n - l);
+        var h = this.getViewportAdjustedDelta(e, t, r, l);
+        h.left ? t.left += h.left : t.top += h.top;
+        var d = /top|bottom/.test(e),
+            p = d ? 2 * h.left - o + r : 2 * h.top - n + l,
+            c = d ? "offsetWidth" : "offsetHeight";
+        i.offset(t), this.replaceArrow(p, i[0][c], d)
+    }, m.prototype.replaceArrow = function(t, e, i) {
+        this.arrow().css(i ? "left" : "top", 50 * (1 - t / e) + "%").css(i ? "top" : "left", "")
+    }, m.prototype.setContent = function() {
+        var t = this.tip(),
+            e = this.getTitle();
+        this.options.html ? (this.options.sanitize && (e = n(e, this.options.whiteList, this.options.sanitizeFn)), t.find(".tooltip-inner").html(e)) : t.find(".tooltip-inner").text(e), t.removeClass("fade in top bottom left right")
+    }, m.prototype.hide = function(t) {
         var e = this,
-            f = a(this.$tip),
-            g = a.Event("hide.bs." + this.type);
-        return this.$element.trigger(g), g.isDefaultPrevented() ? void 0 : (f.removeClass("in"), a.support.transition && f.hasClass("fade") ? f.one("bsTransitionEnd", d).emulateTransitionEnd(c.TRANSITION_DURATION) : d(), this.hoverState = null, this)
-    }, c.prototype.fixTitle = function() {
-        var a = this.$element;
-        (a.attr("title") || "string" != typeof a.attr("data-original-title")) && a.attr("data-original-title", a.attr("title") || "").attr("title", "")
-    }, c.prototype.hasContent = function() {
+            i = g(this.$tip),
+            o = g.Event("hide.bs." + this.type);
+
+        function n() {
+            "in" != e.hoverState && i.detach(), e.$element && e.$element.removeAttr("aria-describedby").trigger("hidden.bs." + e.type), t && t()
+        }
+        if (this.$element.trigger(o), !o.isDefaultPrevented()) return i.removeClass("in"), g.support.transition && i.hasClass("fade") ? i.one("bsTransitionEnd", n).emulateTransitionEnd(m.TRANSITION_DURATION) : n(), this.hoverState = null, this
+    }, m.prototype.fixTitle = function() {
+        var t = this.$element;
+        (t.attr("title") || "string" != typeof t.attr("data-original-title")) && t.attr("data-original-title", t.attr("title") || "").attr("title", "")
+    }, m.prototype.hasContent = function() {
         return this.getTitle()
-    }, c.prototype.getPosition = function(b) {
-        b = b || this.$element;
-        var c = b[0],
-            d = "BODY" == c.tagName,
-            e = c.getBoundingClientRect();
-        null == e.width && (e = a.extend({}, e, {
-            width: e.right - e.left,
-            height: e.bottom - e.top
+    }, m.prototype.getPosition = function(t) {
+        var e = (t = t || this.$element)[0],
+            i = "BODY" == e.tagName,
+            o = e.getBoundingClientRect();
+        null == o.width && (o = g.extend({}, o, {
+            width: o.right - o.left,
+            height: o.bottom - o.top
         }));
-        var f = d ? {
+        var n = window.SVGElement && e instanceof window.SVGElement,
+            s = i ? {
                 top: 0,
                 left: 0
-            } : b.offset(),
-            g = {
-                scroll: d ? document.documentElement.scrollTop || document.body.scrollTop : b.scrollTop()
+            } : n ? null : t.offset(),
+            a = {
+                scroll: i ? document.documentElement.scrollTop || document.body.scrollTop : t.scrollTop()
             },
-            h = d ? {
-                width: a(window).width(),
-                height: a(window).height()
+            r = i ? {
+                width: g(window).width(),
+                height: g(window).height()
             } : null;
-        return a.extend({}, e, g, h, f)
-    }, c.prototype.getCalculatedOffset = function(a, b, c, d) {
-        return "bottom" == a ? {
-            top: b.top + b.height,
-            left: b.left + b.width / 2 - c / 2
-        } : "top" == a ? {
-            top: b.top - d,
-            left: b.left + b.width / 2 - c / 2
-        } : "left" == a ? {
-            top: b.top + b.height / 2 - d / 2,
-            left: b.left - c
+        return g.extend({}, o, a, r, s)
+    }, m.prototype.getCalculatedOffset = function(t, e, i, o) {
+        return "bottom" == t ? {
+            top: e.top + e.height,
+            left: e.left + e.width / 2 - i / 2
+        } : "top" == t ? {
+            top: e.top - o,
+            left: e.left + e.width / 2 - i / 2
+        } : "left" == t ? {
+            top: e.top + e.height / 2 - o / 2,
+            left: e.left - i
         } : {
-            top: b.top + b.height / 2 - d / 2,
-            left: b.left + b.width
+            top: e.top + e.height / 2 - o / 2,
+            left: e.left + e.width
         }
-    }, c.prototype.getViewportAdjustedDelta = function(a, b, c, d) {
-        var e = {
+    }, m.prototype.getViewportAdjustedDelta = function(t, e, i, o) {
+        var n = {
             top: 0,
             left: 0
         };
-        if (!this.$viewport) return e;
-        var f = this.options.viewport && this.options.viewport.padding || 0,
-            g = this.getPosition(this.$viewport);
-        if (/right|left/.test(a)) {
-            var h = b.top - f - g.scroll,
-                i = b.top + f - g.scroll + d;
-            h < g.top ? e.top = g.top - h : i > g.top + g.height && (e.top = g.top + g.height - i)
+        if (!this.$viewport) return n;
+        var s = this.options.viewport && this.options.viewport.padding || 0,
+            a = this.getPosition(this.$viewport);
+        if (/right|left/.test(t)) {
+            var r = e.top - s - a.scroll,
+                l = e.top + s - a.scroll + o;
+            r < a.top ? n.top = a.top - r : l > a.top + a.height && (n.top = a.top + a.height - l)
         } else {
-            var j = b.left - f,
-                k = b.left + f + c;
-            j < g.left ? e.left = g.left - j : k > g.right && (e.left = g.left + g.width - k)
-        }
-        return e
-    }, c.prototype.getTitle = function() {
-        var a, b = this.$element,
-            c = this.options;
-        return a = b.attr("data-original-title") || ("function" == typeof c.title ? c.title.call(b[0]) : c.title)
-    }, c.prototype.getUID = function(a) {
-        do a += ~~(1e6 * Math.random()); while (document.getElementById(a));
-        return a
-    }, c.prototype.tip = function() {
-        if (!this.$tip && (this.$tip = a(this.options.template), 1 != this.$tip.length)) throw new Error(this.type + " `template` option must consist of exactly 1 top-level element!");
+            var h = e.left - s,
+                d = e.left + s + i;
+            h < a.left ? n.left = a.left - h : d > a.right && (n.left = a.left + a.width - d)
+        }
+        return n
+    }, m.prototype.getTitle = function() {
+        var t = this.$element,
+            e = this.options;
+        return t.attr("data-original-title") || ("function" == typeof e.title ? e.title.call(t[0]) : e.title)
+    }, m.prototype.getUID = function(t) {
+        for (; t += ~~(1e6 * Math.random()), document.getElementById(t););
+        return t
+    }, m.prototype.tip = function() {
+        if (!this.$tip && (this.$tip = g(this.options.template), 1 != this.$tip.length)) throw new Error(this.type + " `template` option must consist of exactly 1 top-level element!");
         return this.$tip
-    }, c.prototype.arrow = function() {
+    }, m.prototype.arrow = function() {
         return this.$arrow = this.$arrow || this.tip().find(".tooltip-arrow")
-    }, c.prototype.enable = function() {
+    }, m.prototype.enable = function() {
         this.enabled = !0
-    }, c.prototype.disable = function() {
+    }, m.prototype.disable = function() {
         this.enabled = !1
-    }, c.prototype.toggleEnabled = function() {
+    }, m.prototype.toggleEnabled = function() {
         this.enabled = !this.enabled
-    }, c.prototype.toggle = function(b) {
-        var c = this;
-        b && (c = a(b.currentTarget).data("bs." + this.type), c || (c = new this.constructor(b.currentTarget, this.getDelegateOptions()), a(b.currentTarget).data("bs." + this.type, c))), b ? (c.inState.click = !c.inState.click, c.isInStateTrue() ? c.enter(c) : c.leave(c)) : c.tip().hasClass("in") ? c.leave(c) : c.enter(c)
-    }, c.prototype.destroy = function() {
-        var a = this;
+    }, m.prototype.toggle = function(t) {
+        var e = this;
+        t && ((e = g(t.currentTarget).data("bs." + this.type)) || (e = new this.constructor(t.currentTarget, this.getDelegateOptions()), g(t.currentTarget).data("bs." + this.type, e))), t ? (e.inState.click = !e.inState.click, e.isInStateTrue() ? e.enter(e) : e.leave(e)) : e.tip().hasClass("in") ? e.leave(e) : e.enter(e)
+    }, m.prototype.destroy = function() {
+        var t = this;
         clearTimeout(this.timeout), this.hide(function() {
-            a.$element.off("." + a.type).removeData("bs." + a.type), a.$tip && a.$tip.detach(), a.$tip = null, a.$arrow = null, a.$viewport = null
+            t.$element.off("." + t.type).removeData("bs." + t.type), t.$tip && t.$tip.detach(), t.$tip = null, t.$arrow = null, t.$viewport = null, t.$element = null
         })
+    }, m.prototype.sanitizeHtml = function(t) {
+        return n(t, this.options.whiteList, this.options.sanitizeFn)
     };
-    var d = a.fn.tooltip;
-    a.fn.tooltip = b, a.fn.tooltip.Constructor = c, a.fn.tooltip.noConflict = function() {
-        return a.fn.tooltip = d, this
-    }
-}(jQuery), + function(a) {
-    "use strict";
-
-    function b(b) {
+    var e = g.fn.tooltip;
+    g.fn.tooltip = function i(o) {
         return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.popover"),
-                f = "object" == typeof b && b;
-            (e || !/destroy|hide/.test(b)) && (e || d.data("bs.popover", e = new c(this, f)), "string" == typeof b && e[b]())
+            var t = g(this),
+                e = t.data("bs.tooltip"),
+                i = "object" == typeof o && o;
+            !e && /destroy|hide/.test(o) || (e || t.data("bs.tooltip", e = new m(this, i)), "string" == typeof o && e[o]())
         })
+    }, g.fn.tooltip.Constructor = m, g.fn.tooltip.noConflict = function() {
+        return g.fn.tooltip = e, this
     }
-    var c = function(a, b) {
-        this.init("popover", a, b)
+}(jQuery),
+function(n) {
+    "use strict";
+    var s = function(t, e) {
+        this.init("popover", t, e)
     };
-    if (!a.fn.tooltip) throw new Error("Popover requires tooltip.js");
-    c.VERSION = "3.3.6", c.DEFAULTS = a.extend({}, a.fn.tooltip.Constructor.DEFAULTS, {
+    if (!n.fn.tooltip) throw new Error("Popover requires tooltip.js");
+    s.VERSION = "3.4.1", s.DEFAULTS = n.extend({}, n.fn.tooltip.Constructor.DEFAULTS, {
         placement: "right",
         trigger: "click",
         content: "",
         template: '<div class="popover" role="tooltip"><div class="arrow"></div><h3 class="popover-title"></h3><div class="popover-content"></div></div>'
-    }), c.prototype = a.extend({}, a.fn.tooltip.Constructor.prototype), c.prototype.constructor = c, c.prototype.getDefaults = function() {
-        return c.DEFAULTS
-    }, c.prototype.setContent = function() {
-        var a = this.tip(),
-            b = this.getTitle(),
-            c = this.getContent();
-        a.find(".popover-title")[this.options.html ? "html" : "text"](b), a.find(".popover-content").children().detach().end()[this.options.html ? "string" == typeof c ? "html" : "append" : "text"](c), a.removeClass("fade top bottom left right in"), a.find(".popover-title").html() || a.find(".popover-title").hide()
-    }, c.prototype.hasContent = function() {
+    }), ((s.prototype = n.extend({}, n.fn.tooltip.Constructor.prototype)).constructor = s).prototype.getDefaults = function() {
+        return s.DEFAULTS
+    }, s.prototype.setContent = function() {
+        var t = this.tip(),
+            e = this.getTitle(),
+            i = this.getContent();
+        if (this.options.html) {
+            var o = typeof i;
+            this.options.sanitize && (e = this.sanitizeHtml(e), "string" === o && (i = this.sanitizeHtml(i))), t.find(".popover-title").html(e), t.find(".popover-content").children().detach().end()["string" === o ? "html" : "append"](i)
+        } else t.find(".popover-title").text(e), t.find(".popover-content").children().detach().end().text(i);
+        t.removeClass("fade top bottom left right in"), t.find(".popover-title").html() || t.find(".popover-title").hide()
+    }, s.prototype.hasContent = function() {
         return this.getTitle() || this.getContent()
-    }, c.prototype.getContent = function() {
-        var a = this.$element,
-            b = this.options;
-        return a.attr("data-content") || ("function" == typeof b.content ? b.content.call(a[0]) : b.content)
-    }, c.prototype.arrow = function() {
+    }, s.prototype.getContent = function() {
+        var t = this.$element,
+            e = this.options;
+        return t.attr("data-content") || ("function" == typeof e.content ? e.content.call(t[0]) : e.content)
+    }, s.prototype.arrow = function() {
         return this.$arrow = this.$arrow || this.tip().find(".arrow")
     };
-    var d = a.fn.popover;
-    a.fn.popover = b, a.fn.popover.Constructor = c, a.fn.popover.noConflict = function() {
-        return a.fn.popover = d, this
+    var t = n.fn.popover;
+    n.fn.popover = function e(o) {
+        return this.each(function() {
+            var t = n(this),
+                e = t.data("bs.popover"),
+                i = "object" == typeof o && o;
+            !e && /destroy|hide/.test(o) || (e || t.data("bs.popover", e = new s(this, i)), "string" == typeof o && e[o]())
+        })
+    }, n.fn.popover.Constructor = s, n.fn.popover.noConflict = function() {
+        return n.fn.popover = t, this
     }
-}(jQuery), + function(a) {
+}(jQuery),
+function(s) {
     "use strict";
 
-    function b(c, d) {
-        this.$body = a(document.body), this.$scrollElement = a(a(c).is(document.body) ? window : c), this.options = a.extend({}, b.DEFAULTS, d), this.selector = (this.options.target || "") + " .nav li > a", this.offsets = [], this.targets = [], this.activeTarget = null, this.scrollHeight = 0, this.$scrollElement.on("scroll.bs.scrollspy", a.proxy(this.process, this)), this.refresh(), this.process()
+    function n(t, e) {
+        this.$body = s(document.body), this.$scrollElement = s(t).is(document.body) ? s(window) : s(t), this.options = s.extend({}, n.DEFAULTS, e), this.selector = (this.options.target || "") + " .nav li > a", this.offsets = [], this.targets = [], this.activeTarget = null, this.scrollHeight = 0, this.$scrollElement.on("scroll.bs.scrollspy", s.proxy(this.process, this)), this.refresh(), this.process()
     }
 
-    function c(c) {
+    function e(o) {
         return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.scrollspy"),
-                f = "object" == typeof c && c;
-            e || d.data("bs.scrollspy", e = new b(this, f)), "string" == typeof c && e[c]()
+            var t = s(this),
+                e = t.data("bs.scrollspy"),
+                i = "object" == typeof o && o;
+            e || t.data("bs.scrollspy", e = new n(this, i)), "string" == typeof o && e[o]()
         })
     }
-    b.VERSION = "3.3.6", b.DEFAULTS = {
+    n.VERSION = "3.4.1", n.DEFAULTS = {
         offset: 10
-    }, b.prototype.getScrollHeight = function() {
+    }, n.prototype.getScrollHeight = function() {
         return this.$scrollElement[0].scrollHeight || Math.max(this.$body[0].scrollHeight, document.documentElement.scrollHeight)
-    }, b.prototype.refresh = function() {
-        var b = this,
-            c = "offset",
-            d = 0;
-        this.offsets = [], this.targets = [], this.scrollHeight = this.getScrollHeight(), a.isWindow(this.$scrollElement[0]) || (c = "position", d = this.$scrollElement.scrollTop()), this.$body.find(this.selector).map(function() {
-            var b = a(this),
-                e = b.data("target") || b.attr("href"),
-                f = /^#./.test(e) && a(e);
-            return f && f.length && f.is(":visible") && [
-                [f[c]().top + d, e]
+    }, n.prototype.refresh = function() {
+        var t = this,
+            o = "offset",
+            n = 0;
+        this.offsets = [], this.targets = [], this.scrollHeight = this.getScrollHeight(), s.isWindow(this.$scrollElement[0]) || (o = "position", n = this.$scrollElement.scrollTop()), this.$body.find(this.selector).map(function() {
+            var t = s(this),
+                e = t.data("target") || t.attr("href"),
+                i = /^#./.test(e) && s(e);
+            return i && i.length && i.is(":visible") && [
+                [i[o]().top + n, e]
             ] || null
-        }).sort(function(a, b) {
-            return a[0] - b[0]
+        }).sort(function(t, e) {
+            return t[0] - e[0]
         }).each(function() {
-            b.offsets.push(this[0]), b.targets.push(this[1])
+            t.offsets.push(this[0]), t.targets.push(this[1])
         })
-    }, b.prototype.process = function() {
-        var a, b = this.$scrollElement.scrollTop() + this.options.offset,
-            c = this.getScrollHeight(),
-            d = this.options.offset + c - this.$scrollElement.height(),
-            e = this.offsets,
-            f = this.targets,
-            g = this.activeTarget;
-        if (this.scrollHeight != c && this.refresh(), b >= d) return g != (a = f[f.length - 1]) && this.activate(a);
-        if (g && b < e[0]) return this.activeTarget = null, this.clear();
-        for (a = e.length; a--;) g != f[a] && b >= e[a] && (void 0 === e[a + 1] || b < e[a + 1]) && this.activate(f[a])
-    }, b.prototype.activate = function(b) {
-        this.activeTarget = b, this.clear();
-        var c = this.selector + '[data-target="' + b + '"],' + this.selector + '[href="' + b + '"]',
-            d = a(c).parents("li").addClass("active");
-        d.parent(".dropdown-menu").length && (d = d.closest("li.dropdown").addClass("active")), d.trigger("activate.bs.scrollspy")
-    }, b.prototype.clear = function() {
-        a(this.selector).parentsUntil(this.options.target, ".active").removeClass("active")
-    };
-    var d = a.fn.scrollspy;
-    a.fn.scrollspy = c, a.fn.scrollspy.Constructor = b, a.fn.scrollspy.noConflict = function() {
-        return a.fn.scrollspy = d, this
-    }, a(window).on("load.bs.scrollspy.data-api", function() {
-        a('[data-spy="scroll"]').each(function() {
-            var b = a(this);
-            c.call(b, b.data())
+    }, n.prototype.process = function() {
+        var t, e = this.$scrollElement.scrollTop() + this.options.offset,
+            i = this.getScrollHeight(),
+            o = this.options.offset + i - this.$scrollElement.height(),
+            n = this.offsets,
+            s = this.targets,
+            a = this.activeTarget;
+        if (this.scrollHeight != i && this.refresh(), o <= e) return a != (t = s[s.length - 1]) && this.activate(t);
+        if (a && e < n[0]) return this.activeTarget = null, this.clear();
+        for (t = n.length; t--;) a != s[t] && e >= n[t] && (n[t + 1] === undefined || e < n[t + 1]) && this.activate(s[t])
+    }, n.prototype.activate = function(t) {
+        this.activeTarget = t, this.clear();
+        var e = this.selector + '[data-target="' + t + '"],' + this.selector + '[href="' + t + '"]',
+            i = s(e).parents("li").addClass("active");
+        i.parent(".dropdown-menu").length && (i = i.closest("li.dropdown").addClass("active")), i.trigger("activate.bs.scrollspy")
+    }, n.prototype.clear = function() {
+        s(this.selector).parentsUntil(this.options.target, ".active").removeClass("active")
+    };
+    var t = s.fn.scrollspy;
+    s.fn.scrollspy = e, s.fn.scrollspy.Constructor = n, s.fn.scrollspy.noConflict = function() {
+        return s.fn.scrollspy = t, this
+    }, s(window).on("load.bs.scrollspy.data-api", function() {
+        s('[data-spy="scroll"]').each(function() {
+            var t = s(this);
+            e.call(t, t.data())
         })
     })
-}(jQuery), + function(a) {
+}(jQuery),
+function(r) {
     "use strict";
+    var a = function(t) {
+        this.element = r(t)
+    };
 
-    function b(b) {
+    function e(i) {
         return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.tab");
-            e || d.data("bs.tab", e = new c(this)), "string" == typeof b && e[b]()
+            var t = r(this),
+                e = t.data("bs.tab");
+            e || t.data("bs.tab", e = new a(this)), "string" == typeof i && e[i]()
         })
     }
-    var c = function(b) {
-        this.element = a(b)
-    };
-    c.VERSION = "3.3.6", c.TRANSITION_DURATION = 150, c.prototype.show = function() {
-        var b = this.element,
-            c = b.closest("ul:not(.dropdown-menu)"),
-            d = b.data("target");
-        if (d || (d = b.attr("href"), d = d && d.replace(/.*(?=#[^\s]*$)/, "")), !b.parent("li").hasClass("active")) {
-            var e = c.find(".active:last a"),
-                f = a.Event("hide.bs.tab", {
-                    relatedTarget: b[0]
+    a.VERSION = "3.4.1", a.TRANSITION_DURATION = 150, a.prototype.show = function() {
+        var t = this.element,
+            e = t.closest("ul:not(.dropdown-menu)"),
+            i = t.data("target");
+        if (i || (i = (i = t.attr("href")) && i.replace(/.*(?=#[^\s]*$)/, "")), !t.parent("li").hasClass("active")) {
+            var o = e.find(".active:last a"),
+                n = r.Event("hide.bs.tab", {
+                    relatedTarget: t[0]
                 }),
-                g = a.Event("show.bs.tab", {
-                    relatedTarget: e[0]
+                s = r.Event("show.bs.tab", {
+                    relatedTarget: o[0]
                 });
-            if (e.trigger(f), b.trigger(g), !g.isDefaultPrevented() && !f.isDefaultPrevented()) {
-                var h = a(d);
-                this.activate(b.closest("li"), c), this.activate(h, h.parent(), function() {
-                    e.trigger({
+            if (o.trigger(n), t.trigger(s), !s.isDefaultPrevented() && !n.isDefaultPrevented()) {
+                var a = r(document).find(i);
+                this.activate(t.closest("li"), e), this.activate(a, a.parent(), function() {
+                    o.trigger({
                         type: "hidden.bs.tab",
-                        relatedTarget: b[0]
-                    }), b.trigger({
+                        relatedTarget: t[0]
+                    }), t.trigger({
                         type: "shown.bs.tab",
-                        relatedTarget: e[0]
+                        relatedTarget: o[0]
                     })
                 })
             }
         }
-    }, c.prototype.activate = function(b, d, e) {
-        function f() {
-            g.removeClass("active").find("> .dropdown-menu > .active").removeClass("active").end().find('[data-toggle="tab"]').attr("aria-expanded", !1), b.addClass("active").find('[data-toggle="tab"]').attr("aria-expanded", !0), h ? (b[0].offsetWidth, b.addClass("in")) : b.removeClass("fade"), b.parent(".dropdown-menu").length && b.closest("li.dropdown").addClass("active").end().find('[data-toggle="tab"]').attr("aria-expanded", !0), e && e()
+    }, a.prototype.activate = function(t, e, i) {
+        var o = e.find("> .active"),
+            n = i && r.support.transition && (o.length && o.hasClass("fade") || !!e.find("> .fade").length);
+
+        function s() {
+            o.removeClass("active").find("> .dropdown-menu > .active").removeClass("active").end().find('[data-toggle="tab"]').attr("aria-expanded", !1), t.addClass("active").find('[data-toggle="tab"]').attr("aria-expanded", !0), n ? (t[0].offsetWidth, t.addClass("in")) : t.removeClass("fade"), t.parent(".dropdown-menu").length && t.closest("li.dropdown").addClass("active").end().find('[data-toggle="tab"]').attr("aria-expanded", !0), i && i()
         }
-        var g = d.find("> .active"),
-            h = e && a.support.transition && (g.length && g.hasClass("fade") || !!d.find("> .fade").length);
-        g.length && h ? g.one("bsTransitionEnd", f).emulateTransitionEnd(c.TRANSITION_DURATION) : f(), g.removeClass("in")
+        o.length && n ? o.one("bsTransitionEnd", s).emulateTransitionEnd(a.TRANSITION_DURATION) : s(), o.removeClass("in")
     };
-    var d = a.fn.tab;
-    a.fn.tab = b, a.fn.tab.Constructor = c, a.fn.tab.noConflict = function() {
-        return a.fn.tab = d, this
-    };
-    var e = function(c) {
-        c.preventDefault(), b.call(a(this), "show")
-    };
-    a(document).on("click.bs.tab.data-api", '[data-toggle="tab"]', e).on("click.bs.tab.data-api", '[data-toggle="pill"]', e)
-}(jQuery), + function(a) {
+    var t = r.fn.tab;
+    r.fn.tab = e, r.fn.tab.Constructor = a, r.fn.tab.noConflict = function() {
+        return r.fn.tab = t, this
+    };
+    var i = function(t) {
+        t.preventDefault(), e.call(r(this), "show")
+    };
+    r(document).on("click.bs.tab.data-api", '[data-toggle="tab"]', i).on("click.bs.tab.data-api", '[data-toggle="pill"]', i)
+}(jQuery),
+function(l) {
     "use strict";
+    var h = function(t, e) {
+        this.options = l.extend({}, h.DEFAULTS, e);
+        var i = this.options.target === h.DEFAULTS.target ? l(this.options.target) : l(document).find(this.options.target);
+        this.$target = i.on("scroll.bs.affix.data-api", l.proxy(this.checkPosition, this)).on("click.bs.affix.data-api", l.proxy(this.checkPositionWithEventLoop, this)), this.$element = l(t), this.affixed = null, this.unpin = null, this.pinnedOffset = null, this.checkPosition()
+    };
 
-    function b(b) {
+    function i(o) {
         return this.each(function() {
-            var d = a(this),
-                e = d.data("bs.affix"),
-                f = "object" == typeof b && b;
-            e || d.data("bs.affix", e = new c(this, f)), "string" == typeof b && e[b]()
+            var t = l(this),
+                e = t.data("bs.affix"),
+                i = "object" == typeof o && o;
+            e || t.data("bs.affix", e = new h(this, i)), "string" == typeof o && e[o]()
         })
     }
-    var c = function(b, d) {
-        this.options = a.extend({}, c.DEFAULTS, d), this.$target = a(this.options.target).on("scroll.bs.affix.data-api", a.proxy(this.checkPosition, this)).on("click.bs.affix.data-api", a.proxy(this.checkPositionWithEventLoop, this)), this.$element = a(b), this.affixed = null, this.unpin = null, this.pinnedOffset = null, this.checkPosition()
-    };
-    c.VERSION = "3.3.6", c.RESET = "affix affix-top affix-bottom", c.DEFAULTS = {
+    h.VERSION = "3.4.1", h.RESET = "affix affix-top affix-bottom", h.DEFAULTS = {
         offset: 0,
         target: window
-    }, c.prototype.getState = function(a, b, c, d) {
-        var e = this.$target.scrollTop(),
-            f = this.$element.offset(),
-            g = this.$target.height();
-        if (null != c && "top" == this.affixed) return c > e ? "top" : !1;
-        if ("bottom" == this.affixed) return null != c ? e + this.unpin <= f.top ? !1 : "bottom" : a - d >= e + g ? !1 : "bottom";
-        var h = null == this.affixed,
-            i = h ? e : f.top,
-            j = h ? g : b;
-        return null != c && c >= e ? "top" : null != d && i + j >= a - d ? "bottom" : !1
-    }, c.prototype.getPinnedOffset = function() {
+    }, h.prototype.getState = function(t, e, i, o) {
+        var n = this.$target.scrollTop(),
+            s = this.$element.offset(),
+            a = this.$target.height();
+        if (null != i && "top" == this.affixed) return n < i && "top";
+        if ("bottom" == this.affixed) return null != i ? !(n + this.unpin <= s.top) && "bottom" : !(n + a <= t - o) && "bottom";
+        var r = null == this.affixed,
+            l = r ? n : s.top;
+        return null != i && n <= i ? "top" : null != o && t - o <= l + (r ? a : e) && "bottom"
+    }, h.prototype.getPinnedOffset = function() {
         if (this.pinnedOffset) return this.pinnedOffset;
-        this.$element.removeClass(c.RESET).addClass("affix");
-        var a = this.$target.scrollTop(),
-            b = this.$element.offset();
-        return this.pinnedOffset = b.top - a
-    }, c.prototype.checkPositionWithEventLoop = function() {
-        setTimeout(a.proxy(this.checkPosition, this), 1)
-    }, c.prototype.checkPosition = function() {
+        this.$element.removeClass(h.RESET).addClass("affix");
+        var t = this.$target.scrollTop(),
+            e = this.$element.offset();
+        return this.pinnedOffset = e.top - t
+    }, h.prototype.checkPositionWithEventLoop = function() {
+        setTimeout(l.proxy(this.checkPosition, this), 1)
+    }, h.prototype.checkPosition = function() {
         if (this.$element.is(":visible")) {
-            var b = this.$element.height(),
-                d = this.options.offset,
-                e = d.top,
-                f = d.bottom,
-                g = Math.max(a(document).height(), a(document.body).height());
-            "object" != typeof d && (f = e = d), "function" == typeof e && (e = d.top(this.$element)), "function" == typeof f && (f = d.bottom(this.$element));
-            var h = this.getState(g, b, e, f);
-            if (this.affixed != h) {
+            var t = this.$element.height(),
+                e = this.options.offset,
+                i = e.top,
+                o = e.bottom,
+                n = Math.max(l(document).height(), l(document.body).height());
+            "object" != typeof e && (o = i = e), "function" == typeof i && (i = e.top(this.$element)), "function" == typeof o && (o = e.bottom(this.$element));
+            var s = this.getState(n, t, i, o);
+            if (this.affixed != s) {
                 null != this.unpin && this.$element.css("top", "");
-                var i = "affix" + (h ? "-" + h : ""),
-                    j = a.Event(i + ".bs.affix");
-                if (this.$element.trigger(j), j.isDefaultPrevented()) return;
-                this.affixed = h, this.unpin = "bottom" == h ? this.getPinnedOffset() : null, this.$element.removeClass(c.RESET).addClass(i).trigger(i.replace("affix", "affixed") + ".bs.affix")
+                var a = "affix" + (s ? "-" + s : ""),
+                    r = l.Event(a + ".bs.affix");
+                if (this.$element.trigger(r), r.isDefaultPrevented()) return;
+                this.affixed = s, this.unpin = "bottom" == s ? this.getPinnedOffset() : null, this.$element.removeClass(h.RESET).addClass(a).trigger(a.replace("affix", "affixed") + ".bs.affix")
             }
-            "bottom" == h && this.$element.offset({
-                top: g - b - f
+            "bottom" == s && this.$element.offset({
+                top: n - t - o
             })
         }
     };
-    var d = a.fn.affix;
-    a.fn.affix = b, a.fn.affix.Constructor = c, a.fn.affix.noConflict = function() {
-        return a.fn.affix = d, this
-    }, a(window).on("load", function() {
-        a('[data-spy="affix"]').each(function() {
-            var c = a(this),
-                d = c.data();
-            d.offset = d.offset || {}, null != d.offsetBottom && (d.offset.bottom = d.offsetBottom), null != d.offsetTop && (d.offset.top = d.offsetTop), b.call(c, d)
+    var t = l.fn.affix;
+    l.fn.affix = i, l.fn.affix.Constructor = h, l.fn.affix.noConflict = function() {
+        return l.fn.affix = t, this
+    }, l(window).on("load", function() {
+        l('[data-spy="affix"]').each(function() {
+            var t = l(this),
+                e = t.data();
+            e.offset = e.offset || {}, null != e.offsetBottom && (e.offset.bottom = e.offsetBottom), null != e.offsetTop && (e.offset.top = e.offsetTop), i.call(t, e)
         })
     })
 }(jQuery);
```

### Comparing `fookebox-0.7.3/fookebox/public/js/fookebox/classic/client.js` & `fookebox-1.0.0/src/fookebox/js/fookebox.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,711 +1,632 @@
+"use strict";
+
 /*
- * fookebox, https://github.com/cockroach/fookebox
- *
- * Copyright (C) 2007-2014 Stefan Ott. All rights reserved.
+ * fookebox, https://code.ott.net/fookebox/
+ * Copyright (c) 2007-2023 Stefan Ott. all rights reserved.
  *
  * This program is free software: you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation, either version 3 of the License, or
- * (at your option) any later version.
+ * it under the terms of the GNU Affero General Public License as published by
+ * the Free Software Foundation, version 3.
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
- * GNU General Public License for more details.
+ * GNU Affero General Public License for more details.
  *
- * You should have received a copy of the GNU General Public License
- * along with this program.  If not, see <http://www.gnu.org/licenses/>.
+ * You should have received a copy of the GNU Affero General Public License
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-"use strict";
-
-function Message(text) {
-    this.text = text;
-}
-
-Message.prototype.show = function() {
-    if ($('#messageText').data('timeout')) {
-        clearTimeout($('#messageText').data('timeout'));
-    }
+/* HTML elements */
 
-    $('#messageText').text(this.text);
-    $('#messageText').data('timeout', setTimeout(this.hide, 3000));
-    $('#message').show();
-}
+function PlayAlbumButton(album) {
+    var div = document.createElement("div");
+    div.classList.add("pull-right");
+
+    var button = document.createElement("button");
+    button.classList.add("btn");
+    button.classList.add("btn-default");
+    button.classList.add("btn-md");
+    div.append(button);
+
+    var span = document.createElement("span");
+    span.classList.add("glyphicon");
+    span.classList.add("glyphicon-play");
+    button.append(span);
 
-Message.prototype.hide = function() {
-    $('#message').fadeOut('slow');
-}
+    var text = " " + _("Play album");
+    button.append(text);
 
-function AjaxView() {}
+    div.onclick = function(event) {
+        album.play()
+    };
 
-AjaxView.prototype.get = function(url, cb) {
-    $.ajax({
-        url: url,
-        type: 'GET',
-        success: $.proxy(cb, this),
-        error: $.proxy(this.ajaxError, this)
-    });
+    return div;
 }
 
-AjaxView.prototype.post = function(url, data, cb, fcb) {
-    if (!cb)
-        cb = this.ignore;
-
-    if (!fcb)
-        fcb = this.ajaxError;
+function AlbumHeader(album, enablePlayAlbum) {
+    var div = document.createElement("div");
+    div.classList.add("panel-heading");
+    div.classList.add("album-heading");
 
-    $.ajax({
-        url: url,
-        type: 'POST',
-        data: JSON.stringify(data),
-        contentType: 'application/json; charset=utf-8',
-        success: $.proxy(cb, this),
-        error: $.proxy(fcb, this)
-    });
-}
+    var h4 = document.createElement("h4");
+    h4.classList.add("panel-title");
+    div.append(h4);
 
-AjaxView.prototype.ajaxError = function(data) {
-    new Message(data.statusText).show();
-    $('#progress').hide();
-}
+    if (enablePlayAlbum) {
+        h4.append(new PlayAlbumButton(album));
+    }
 
-AjaxView.prototype.ignore = function(data) {}
+    var name = document.createElement("div");
+    name.classList.add("albumTitle");
+    name.innerText = album.name;
+    h4.append(name);
 
-function QueueView(songRemoval) {
-    this.songRemoval = songRemoval;
-    this.queueLength = -1;
-    this.queueView = $('#playlist');
-    this.template = '<span class="artist"></span> - <span class="title"></span>';
-}
+    var artist = document.createElement("div");
+    artist.classList.add("albumArtist");
+    artist.innerText = album.artist;
+    h4.append(artist);
 
-QueueView.prototype = new AjaxView();
+    var cover = new AlbumCover(album);
+    cover.load(div);
 
-QueueView.prototype.sync = function() {
-    this.get('queue', this.update);
-    $('#progress').hide();
+    return div;
 }
 
-QueueView.prototype.update = function(data) {
-    var queue = data.queue;
-    this.queueLength = queue.length;
+function TrackList(tracks, jukebox) {
+    var body = document.createElement("div");
+    body.classList.add("panel-body");
 
-    var playlist = this.queueView.find('li');
+    var list = document.createElement("ul");
+    list.classList.add("list-unstyled");
+    body.append(list);
 
-    playlist.each(function(i, li) {
-        var item = queue[i];
+    for (var i = 0; i < tracks.length; i++) {
+        var track = tracks[i];
+        list.append(new Track(track, jukebox))
+    }
 
-        if (item) {
-            this.updateSlot($(li), i, item);
-        } else {
-            $(li).html('<span class="freeSlot">-- ' +
-                _('empty') + ' --</span>');
-        }
-    }.bind(this));
+    return body;
 }
 
-QueueView.prototype.updateSlot = function(element, position, track) {
-    if (!track.artist || (track.artist == ''))
-        track.artist = _('Unknown artist');
-    if (!track.title || (track.title == ''))
-        track.title = _('Unnamed track');
-
-    element.html(this.template);
-    element.find('.artist').text(track.artist);
-    element.find('.title').text(track.title);
-
-    if (this.songRemoval) {
-        var link = $('<a href="#"></a>');
-        link.click($.proxy(function() {
-            this.unqueue(position + 1);
-            return false;
-        }, this));
+function Track(t, jukebox) {
+    var li = document.createElement("li");
 
-        var img = $('<img src="img/classic/delete.png" alt="x" />');
-        img.attr('title', _('Remove from the queue'));
-        link.append(img);
-        element.append(link);
-    }
-}
+    var link = document.createElement("a");
+    link.href = "#";
+    link.innerHTML = `${t.track} &ndash; ${t.artist} &ndash; ${t.title}`
+    li.append(link);
 
-QueueView.prototype.setLength = function(length) {
-    if (length != this.queueLength)
-        this.sync();
-}
+    link.onclick = function(event) {
+        event.preventDefault();
+        jukebox.play([t]);
+    };
 
-QueueView.prototype.unqueue = function(id) {
-    $('#progress').show();
-    this.post('remove', {
-        'id': id
-    }, this.sync);
+    return li;
 }
 
-function TrackView() {
-    this.artist = "";
-    this.track = "";
-    this.timeTotal = "00:00";
-    this.playing = false;
-
-    this.time = new Date(0, 0, 0);
+function AlbumCover(album) {
+    this.album = album;
 }
 
-TrackView.prototype.attach = function(jukebox) {
-    this.artistView = $('#artist');
-    this.trackView = $('#track');
-    this.timeView = $('#timeTotal');
-    this.timePassedView = $('#timePassed');
-
-    function addControl(key) {
-        $('#control-' + key).click(function() {
-            jukebox.control(key);
-            return false;
-        });
-    }
+/* RFC3986-compliant version of encodeURIComponent
+ *
+ * With the normal encodeURIComponent function, parentheses are not encoded.
+ * This would lead to URLs that *can* be downloaded with $.ajax but that won't
+ * work in CSS rules.
+ *
+ * Taken from https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/encodeURIComponent
+ */
+function encodeRFC3986URIComponent(str) {
+    return encodeURIComponent(str)
+        .replace(
+            /[!'()*]/g,
+            (c) => `%${c.charCodeAt(0).toString(16).toUpperCase()}`
+        );
+}
+
+AlbumCover.prototype.load = function(target) {
+    const file = encodeRFC3986URIComponent(this.album.tracks[0].file);
+    const url = `cover/${file}`;
 
-    if ($('#control')) {
-        addControl('prev');
-        addControl('pause');
-        addControl('play');
-        addControl('next');
-        addControl('voldown');
-        addControl('volup');
-        addControl('rebuild');
-    }
-}
+    const req = $.ajax(url);
 
-TrackView.prototype.updateTime = function() {
-    var seconds = this.time.getSeconds();
-    var minutes = this.time.getMinutes();
-
-    if (seconds < 10)
-        seconds = "0" + seconds;
-    if (minutes < 10)
-        minutes = "0" + minutes;
-
-    this.timePassedView.text(minutes + ":" + seconds);
-}
-
-TrackView.prototype.tick = function() {
-    if (this.playing)
-        this.time.setSeconds(this.time.getSeconds() + 1);
-    this.updateTime();
-}
-
-TrackView.prototype.adjustTime = function(time) {
-    // sync our client-side track time with the one from the
-    // server. update the seconds only if we differ by more than
-    // one second (force-update the display in that case).
-    //
-    // this should fix the 'jumpy' track time display
-    var parts = time.split(':');
-    if (parts.length == 2) {
-        var minutes = parts[0];
-        var seconds = parts[1];
-
-        var diff = seconds - this.time.getSeconds();
-
-        this.time.setMinutes(minutes);
-
-        if (diff > 1 || diff < -1) {
-            this.time.setSeconds(seconds);
-            this.updateTime();
-        }
-    }
+    req.done(function(data) {
+        target.style.backgroundImage = `url(${url})`;
+    });
+    req.fail(function(data) {
+        target.classList.add("no-cover");
+    });
 }
 
-TrackView.prototype.update = function(artist, track, timeTotal, playing) {
-    this.artist = artist;
-    this.track = track;
-    this.timeTotal = timeTotal;
-    this.playing = playing;
-
-    if (!this.playing)
-        $('#timePassed').addClass('paused');
-    else
-        $('#timePassed').removeClass('paused');
-
-    if (this.artist != this.artistView.text())
-        this.artistView.text(this.artist);
-    if (this.track != this.trackView.text())
-        this.trackView.text(this.track);
-    if (this.timeTotal != this.timeView.text())
-        this.timeView.text(this.timeTotal);
-}
-
-function CoverView() {
-    this.img = $('#nowPlayingCover');
-}
-
-CoverView.prototype.setCover = function(hasCover, coverURI) {
-    if (hasCover) {
-        this.img.attr('src', 'cover/' + coverURI);
-        this.img.show();
-    } else {
-        this.img.hide();
-    }
-}
+/* End of HTML elements */
 
-function MusicView(jukebox) {
+function WindowHandler(jukebox) {
     this.jukebox = jukebox;
-}
-
-MusicView.prototype = new AjaxView();
-
-MusicView.prototype.attach = function() {
-    $('.artistLink').each(function(link) {
-        link.onclick = function() {
-            var target = event.target;
-            var artist = target.id.substring(7, target.id.length);
-            this.showArtist(artist);
-            return false;
-        }.bind(this);
-    }.bind(this));
-
-    $('.genreLink').each(function(link) {
-        link.onclick = function() {
-            var target = event.target;
-            var genre = target.id.substring(6, target.id.length);
-            this.showGenre(genre);
-            return false;
-        }.bind(this);
-    }.bind(this));
-
-    var searchForm = $('#searchForm');
+    this.skipval = null;
 
-    if (searchForm) {
-        searchForm.submit($.proxy(function(event) {
-            var form = event.target;
-            this.search(form);
-            return false;
-        }, this));
-    }
+    $(window).on("hashchange", $.proxy(this.loadhash, this));
+    this.loadhash(this);
 }
 
-MusicView.prototype.showArtist = function(artist) {
-    $('#progress').show();
+WindowHandler.prototype.loadhash = function(e) {
+    var hash = window.location.hash;
 
-    // TODO: the page control should actually do this
-    window.location = "#artist=" + artist;
-    this.jukebox.page.url = window.location.href;
-
-    this.get('artist/' + artist, this.showSearchResult);
-}
+    if (!hash) {
+        this.jukebox.showSearch();
+        return;
+    }
 
-MusicView.prototype.showGenre = function(genre) {
-    $('#progress').show();
+    if (hash == this.skipval) {
+        this.skipval = null;
+        return;
+    }
+    this.skipval = null;
 
-    // TODO: the page control should actually do this
-    window.location = "#genre=" + genre;
-    this.jukebox.page.url = window.location.href;
+    var m = hash.match(/([a-z]+)=(.*)$/);
 
-    this.get('genre/' + genre, this.showSearchResult);
-}
+    if (!m || (m.length != 3))
+        return;
 
-MusicView.prototype.search = function(form) {
-    $('#progress').show();
+    var key = m[1];
+    var val = decodeURIComponent(m[2]);
 
-    var data = {
-        'where': $('#searchType').val(),
-        'what': $('#searchTerm').val(),
-        'forceSearch': true
-    };
+    this.jukebox.showItems(key, val);
 
-    this.post('search', data, this.showSearchResult);
+    if (key == 'artist')
+        $('#showArtists').tab('show');
+    else if (key == 'genre')
+        $('#showGenres').tab('show');
 }
 
-MusicView.prototype.showSearchResult = function(transport) {
-    var result = new SearchResult(this.jukebox, transport);
-    result.show();
-
-    $('#progress').hide();
+WindowHandler.prototype.skip = function(val) {
+    this.skipval = val;
 }
 
-function AlbumCover(album, target) {
-    this.album = album;
-    this.target = target;
-}
+function QueueView() {
+    var getMaxLength = function() {
+        return $('#queue').find('li').length;
+    }
 
-AlbumCover.prototype = new AjaxView();
+    var getCurrentLength = function() {
+        return $('#queue').find('li:not(.disabled)').length;
+    }
 
-AlbumCover.prototype.load = function() {
-    var data = {
-        'artist': this.album.artist,
-        'album': this.album.name
-    };
+    Object.defineProperty(this, 'maxLength', {
+        get: getMaxLength
+    });
 
-    this.post('findcover', data, this.loaded, this.hide);
+    Object.defineProperty(this, 'currentLength', {
+        get: getCurrentLength
+    });
 }
 
-AlbumCover.prototype.loaded = function(response) {
-    this.target.attr('src', 'cover/' + response.uri);
-    this.target.show();
-}
+QueueView.prototype.update = function() {
+    var req = $.get('queue');
+    req.done($.proxy(this.load, this));
+}
+
+QueueView.prototype.updateLabel = function(flash) {
+    var len = this.currentLength;
+    var qlen = this.maxLength;
+    var label = $('#queueStatus');
+
+    if (len == qlen) {
+        label.text(_('full'));
+        label.removeClass('label-success');
+        label.addClass('label-warning');
+        label.removeClass('label-info');
+    } else if (len == 0) {
+        label.text(_('empty'));
+        label.addClass('label-success');
+        label.removeClass('label-warning');
+        label.removeClass('label-info');
+    } else {
+        label.text(len + '/' + qlen);
+        label.removeClass('label-success');
+        label.removeClass('label-warning');
+        label.addClass('label-info');
+    }
 
-AlbumCover.prototype.hide = function(transport) {
-    this.target.hide();
+    if (flash) {
+        this.pulsate();
+    }
 }
 
-function SearchResult(jukebox, data) {
-    this.jukebox = jukebox;
-
-    this.tracks = data.tracks;
-    this.what = data.meta.what;
-
-    if (!this.what || (this.what == ''))
-        this.what = _('(none)');
+QueueView.prototype.pulsate = function() {
+    var label = $('#queueStatus');
+    label.hide();
+    label.show('highlight');
+}
 
-    this.albums = {}
+QueueView.prototype.delete = function(i) {
+    return function(event) {
+        var req = $.ajax("queue/" + (i + 1), {
+            "type": "DELETE",
+        });
 
-    this.albumTemplate = '<span class="artist"></span> - <span class="name"></span>';
-    this.albumDiscTemplate = '<span class="artist"><span> - <span class="name"></span> (Disc#<span class="disc"></span>';
+        req.done($.proxy(function() {
+            this.update();
+        }, this));
 
-    this.parseAlbums();
+        return false;
+    }.bind(this);
 }
 
-SearchResult.prototype.parseAlbums = function() {
-    function mkstring(input) {
-        if (typeof input == "object") {
-            if (input.length > 0)
-                return input[0];
-            return "";
-        } else
-            return input;
+QueueView.prototype.load = function(data) {
+    if (!("queue" in data)) {
+        return;
     }
 
-    for (var key in this.tracks) {
-        var track = this.tracks[key];
-        // Yes, this sucks: python-mpd enjoys returning arrays
-        // when multiple tags are present. We need to unpack
-        // them here.
-
-        track.album = mkstring(track.album);
-        track.artist = mkstring(track.artist);
-        track.title = mkstring(track.title);
-        track.track = mkstring(track.track);
+    var len = data.queue.length;
+    var prevlen = this.currentLength;
+    var els = $("#queue li");
+
+    for (var i = 0; i < this.maxLength; i++) {
+        var el = $(els[i]);
+        var link = el.find("a");
+
+        link.off("click");
+
+        if (i >= len) {
+            el.addClass("disabled");
+            link.find(".artist").text("");
+            link.find(".title").text("");
+            link.click(function(event) {
+                return false
+            });
+            continue;
+        }
 
-        var key = track.album + "-" + track.disc;
-        var album = this.albums[key];
+        var track = data.queue[i];
+        link.find(".artist").text(track.artist);
+        link.find(".title").text(track.title);
+        el.removeClass("disabled");
 
-        if (album == null) {
-            album = new Album(track.artist, track.album,
-                track.disc);
-            this.albums[key] = album;
+        if (el.find("span.controls").length > 0) {
+            link.click(this.delete(i));
+        } else {
+            link.click(function(event) {
+                return false
+            });
         }
-
-        album.add(track);
     }
-}
-
-SearchResult.prototype.showTrack = function(track) {
-    var node = $('<li class="track"></li>');
-    var link = $('<a href="#"></a>');
-
-    var template = '<span class="track"></span> - <span class="artist"></span> - <span class="title"></span>';
-    link.html(template);
-
-    link.find('.track').text(track.track);
-    link.find('.artist').text(track.artist);
-    link.find('.title').text(track.title);
 
-    link.click($.proxy(function(event) {
-        this.jukebox.queue(track);
-        return false;
-    }, this));
-
-    node.append(link);
-    return node;
+    this.updateLabel(len != prevlen);
 }
 
-SearchResult.prototype.showAlbum = function(album) {
-    var node = $('<li class="searchResultItem"></li>');
-    var header = $('<h3 class="album"></h3>');
-    var tracks = $('<ul class="trackList"></ul>');
-    var coverArt = $('<img class="coverArt" width="200" />');
+function AlbumList() {
+    this.albums = new Object();
+}
 
-    if (this.jukebox.config.enable_queue_album) {
-        var link = $('<a href="#"></a>');
+AlbumList.prototype.contains = function(album) {
+    return (album.hash() in this.albums);
+}
 
-        link.click($.proxy(function(event) {
-            this.jukebox.queueAlbum(album);
-            return false;
-        }, this));
+AlbumList.prototype.add = function(album) {
+    this.albums[album.hash()] = album;
+}
 
-        var template = album.disc ? this.albumDiscTemplate :
-            this.albumTemplate;
-        link.html(template);
-
-        link.find('.artist').text(album.artist);
-        link.find('.name').text(album.name);
-        link.find('.disc').text(album.disc);
+AlbumList.prototype.get = function(album) {
+    return this.albums[album.hash()];
+}
 
-        header.append(link);
-    } else {
-        header.html(this.albumTemplate);
-        header.find('.artist').text(album.artist);
-        header.find('.name').text(album.name);
-    }
-
-    album.getTracks().forEach(function(track) {
-        tracks.append(this.showTrack(track));
-    }, this);
-
-    if (this.jukebox.config.show_cover_art)
-        new AlbumCover(album, coverArt).load();
-
-    node.append(coverArt);
-    node.append(header);
-    node.append(tracks);
-    return node;
+AlbumList.prototype.sortAll = function() {
+    for (var key in this.albums) {
+        var album = this.albums[key];
+        album.sort(function(a, b) {
+            return Number(a.track) - Number(b.track);
+        });
+    }
 }
 
-SearchResult.prototype.show = function() {
-    // TODO: this, right
-    $('#searchResult').empty();
+AlbumList.prototype.render = function() {
+    var queueAlbums = false;
+    var albums = new Array();
+    var body = $("body");
 
-    var header = $('<h2></h2>');
-    header.text(this.what);
-    var ul = $('<ul id="searchResultList"></ul>');
+    if (body.attr("queue-albums")) {
+        queueAlbums = true;
+    }
 
-    var albums = new Array();
     for (var key in this.albums) {
         albums.push(this.albums[key]);
     }
 
-    var sorted = albums.sort(function(a, b) {
-        var strA = a.artist + ' - ' + a.name;
-        var strB = b.artist + ' - ' + b.name;
-
-        return strA > strB;
+    albums.sort(function(a, b) {
+        return a.name > b.name;
     });
 
-    sorted.forEach(function(album) {
-        ul.append(this.showAlbum(album));
-    }, this);
-
-    $('#searchResult').append(header);
-    $('#searchResult').append(ul);
+    $(albums).each(function(i, album) {
+        album.render(queueAlbums);
+    });
 }
 
-function Album(artist, name, disc) {
-    this.artist = artist;
+function Album(jukebox, path, name) {
+    this.jukebox = jukebox;
+    this.path = path;
     this.name = name;
-    this.disc = disc;
-    this.tracks = {};
+    this.artist = '';
+    this.tracks = new Array();
+}
 
-    if (!this.artist || (this.artist == ""))
-        this.artist = _('Unknown artist');
-    if (!this.name || (this.name == ""))
-        this.name = _('Unnamed album');
+Album.prototype.hash = function() {
+    return btoa(escape('' + this.name + this.path));
 }
 
 Album.prototype.add = function(track) {
-    if (!track.track || (track.track == ''))
-        track.track = '00';
-    else if (track.track.indexOf('/') >= 0)
-        track.track = track.track.replace(/\/.*/, '');
-    else if (track.track.length < 2)
-        track.track = '0' + track.track;
-
-    if (!track.artist || (track.artist == ""))
-        track.artist = _('Unknown artist');
-    if (!track.title || (track.title == ""))
-        track.title = _('Unnamed track');
-
-    if ((track.artist != this.artist) &&
-        !(track.artist.indexOf(this.artist) == 0)) {
-        if (this.artist.indexOf(track.artist) == 0)
-            this.artist = track.artist;
-        else
-            this.artist = _('Various artists');
+    this.tracks.push(track);
+
+    if (this.artist == '') {
+        this.artist = track.artist;
+    } else if ((this.artist.indexOf(track.artist) < 0) &&
+        (track.artist.indexOf(this.artist) < 0)) {
+        this.artist = _('Various artists');
     }
+}
 
-    this.tracks[track.file] = track;
+Album.prototype.sort = function(f) {
+    this.tracks.sort(f);
 }
 
-Album.prototype.getTracks = function() {
-    var tracks = new Array();
+Album.prototype.play = function(f) {
+    this.jukebox.play(this.tracks);
+}
 
-    for (var key in this.tracks) {
-        tracks.push(this.tracks[key]);
-    }
+Album.prototype.render = function(enablePlayAlbum) {
+    $('#result').append(new AlbumHeader(this, enablePlayAlbum));
+    $('#result').append(new TrackList(this.tracks, this.jukebox));
+}
 
-    tracks.sort(function(a, b) {
-        return a.track - b.track;
-    });
+function SearchResult(jukebox, tracks) {
+    this.tracks = tracks;
+    this.jukebox = jukebox;
+    this.albums = new AlbumList();
 
-    return tracks;
-}
+    function tracknum(input) {
+        if ((input == '') || !input)
+            return '00';
+        else if (input.indexOf('/') >= 0)
+            return tracknum(input.replace(/\/.*/, ''));
+        else if (input.length < 2)
+            return '0' + input;
+        else
+            return input
+    }
 
-function JukeboxView(config) {
-    this.config = {};
-    this.loadconfig();
+    function mkstring(input, type) {
+        if (typeof input == "string") {
+            return input;
+        } else if (typeof input == "object") {
+            if (input.length > 0)
+                return input[0];
+        }
 
-    this.queueView = new QueueView(this.config.enable_song_removal);
-    this.trackView = new TrackView();
-    this.coverView = new CoverView();
-    this.musicView = new MusicView(this);
-    this.page = new PageControl(this);
-    this.page.watch();
-}
+        return _('Unnamed ' + type);
+    }
 
-JukeboxView.prototype = new AjaxView();
+    $(this.tracks).each(function(i, track) {
+        track.track = tracknum(track.track);
+        track.album = mkstring(track.album, 'album');
+    });
 
-JukeboxView.prototype.loadconfig = function() {
-    var body = $('body');
-    this.config.enable_queue_album = (body.data('enablequeuealbum') == 'True');
-    this.config.show_cover_art = (body.data('showcoverart') == 'True');
-    this.config.enable_song_removal = (body.data('enablesongremoval') == 'True');
+    this.parseAlbums();
 }
 
-JukeboxView.prototype.attach = function() {
-    this.trackView.attach(this);
-    this.musicView.attach();
-}
+SearchResult.prototype.parseAlbums = function() {
+    $(this.tracks).each($.proxy(function(i, track) {
+        var album;
+        var file = track.file;
+        var dir = file.substring(0, file.lastIndexOf("/") + 1);
+        var fn = file.substring(file.lastIndexOf("/") + 1);
+
+        if (!track.artist)
+            track.artist = _('Unknown artist');
+        if (!track.title)
+            track.title = _('Unnamed track') + ' [' + fn + ']';
 
-JukeboxView.prototype.readStatus = function(data) {
-    this.trackView.update(data.artist, data.track, data.timeTotal,
-        data.playing);
-    this.trackView.adjustTime(data.timePassed);
-    this.coverView.setCover(data.has_cover, data.cover_uri);
-    this.queueView.setLength(data.queueLength);
-}
+        album = new Album(this.jukebox, dir, track.album);
 
-JukeboxView.prototype.sync = function() {
-    window.setTimeout(this.sync.bind(this), 1000);
+        if (!this.albums.contains(album)) {
+            this.albums.add(album);
+        }
 
-    // update time
-    this.trackView.tick();
+        album = this.albums.get(album);
+        album.add(track);
+    }, this));
 
-    this.get('status', this.readStatus);
+    this.albums.sortAll();
 }
 
-JukeboxView.prototype.control = function(action) {
-    this.post('control', {
-        'action': action
-    });
+SearchResult.prototype.show = function() {
+    $('#result').empty();
+    this.albums.render();
 }
 
-JukeboxView.prototype.queue = function(track) {
-    this.queueAll(new Array(track.file));
+function Jukebox() {
+    this.queue = new QueueView();
+    this.queue.update();
 }
 
-JukeboxView.prototype.queueAlbum = function(album) {
-    window.x = album.getTracks();
-    this.queueAll(album.getTracks().map(function(item) {
-        return item.file;
-    }));
+Jukebox.prototype.showSearch = function() {
+    $('.navbar-toggle').removeClass('hidden-xs');
+    $('.sidebar').removeClass('hidden-xs');
+    $('.main').addClass('hidden-xs');
 }
 
-JukeboxView.prototype.queueAll = function(tracks) {
-    $.ajax({
-        url: 'queue',
-        type: 'POST',
-        data: JSON.stringify({
-            'files': tracks
-        }),
-        contentType: 'application/json; charset=utf-8',
-        headers: {
-            accept: "application/json; charset=utf-8",
-        },
-        success: $.proxy(this.queueView.sync, this.queueView),
-        error: this.ajaxError
-    });
+Jukebox.prototype.showResult = function() {
+    $('.navbar-toggle').addClass('hidden-xs');
+    $('.sidebar').addClass('hidden-xs');
+    $('.main').removeClass('hidden-xs');
+    window.scrollTo(0, 0);
+    $('.main').scrollTop(0);
 }
 
-JukeboxView.prototype.showArtist = function(artist) {
-    // TODO: remove this
-    this.musicView.showArtist(artist);
-}
+Jukebox.prototype.sync = function() {
+    window.setTimeout($.proxy(this.sync, this), 1000);
 
-JukeboxView.prototype.showGenre = function(genre) {
-    // TODO: remove this
-    this.musicView.showGenre(genre);
-}
+    var req = $.get('status');
+    req.done($.proxy(function(data) {
+        if ('artist' in data) {
+            $('.currentArtist').text(data.artist);
+        } else if (data.state == 'play') {
+            $('.currentArtist').text(_('Unknown artist'));
+        } else {
+            $('.currentArtist').empty();
+        }
 
-function PageControl(jukebox) {
-    this.tab = 'artist';
-    this.url = '';
-    this.jukebox = jukebox;
+        if ('title' in data) {
+            $('.currentTitle').text(data.title);
+        } else if (data.state == 'play') {
+            $('.currentTitle').text(_('Unnamed track'));
+        } else {
+            $('.currentTitle').empty();
+        }
+
+        if ('queueLength' in data) {
+            if (data.queueLength != this.queue.currentLength)
+                this.queue.update();
+        }
+    }, this));
 }
 
-PageControl.prototype.watch = function() {
-    this.url = window.location.href;
-    this.apply();
-    this.update();
+Jukebox.prototype.showItems = function(type, name) {
+    const name_encoded = encodeRFC3986URIComponent(name);
+    const req = $.getJSON(type + "/" + name_encoded);
+
+    const well = $('<div class="well"></div>');
+    well.text(_("Loading, please wait..."));
+    const panel = $('<div class="panel panel-default"><div class="panel-body"></div></div>');
+    panel.append(well);
+
+    panel.fadeIn(400);
+    $('#result').empty();
+    $('#result').append(panel);
+
+    this.showResult();
+
+    req.done($.proxy(function(data) {
+        const result = new SearchResult(this, data.tracks);
+        result.show();
+    }, this));
 
-    this.attachToTab('artist');
-    this.attachToTab('genre');
-    this.attachToTab('search');
+    req.fail(function() {
+        console.error("failed");
+    });
 }
 
-PageControl.prototype.attachToTab = function(tab) {
-    var li = $(tab + 'Tab');
+Jukebox.prototype.play = function(tracks) {
+    var files = tracks.map(function(obj) {
+        return obj.file
+    });
 
-    if (!li)
-        return;
+    var req = $.ajax("queue", {
+        "data": JSON.stringify({
+            "files": files
+        }),
+        "type": "POST",
+        "processData": false,
+        "contentType": "application/json"
+    });
 
-    var a = li.select('a');
+    req.done($.proxy(function() {
+        this.queue.update();
+    }, this));
 
-    if (a.length > 0) {
-        a[0].onclick = function() {
-            this.setTab(tab);
-            return false;
-        }.bind(this);
-    }
+    req.error($.proxy(function(data) {
+        switch (data.status) {
+            case 409:
+                this.queue.pulsate();
+                break;
+            default:
+                console.error(data);
+        }
+    }, this));
 }
 
-PageControl.prototype.update = function() {
-    setTimeout(this.update.bind(this), 400);
-
-    var url = window.location.href;
+Jukebox.prototype.showGenre = function(name) {
+    this.showItems('genre', name);
+}
 
-    if (url != this.url) {
-        this.url = url;
-        this.apply();
-    }
+Jukebox.prototype.showArtist = function(name) {
+    this.showItems('artist', name);
 }
 
-PageControl.prototype.apply = function() {
-        var url = unescape(this.url);
+Jukebox.prototype.control = function(action) {
+    var data = {
+        'action': action
+    };
 
-        if (url.indexOf("#") > -1) {
-            var parts = url.split('#');
-            var params = parts[1].split('=');
-            var key = params[0];
-            var value = parts[1].substring(key.length + 1);
+    $.ajax({
+        url: 'control',
+        type: 'POST',
+        data: JSON.stringify(data),
+        contentType: 'application/json; charset=utf-8'
+    });
+}
 
-            if (key == 'artist') {
-                this.setTab(key);
-                this.jukebox.showArtist(value);
-            } else if (key == 'genre') {
-                this.setTab(key);
-                this.jukebox.showGenre(value);
-            } else if (key == 'tab') {
-                this.setTab(value);
-            }
+$(document).ready(function() {
+    function filter(list) {
+        return function(event) {
+            var el = $(event.currentTarget);
+            var val = el.val().toLowerCase();
+
+            list.each(function(i, item) {
+                var link = $(item).find('a');
+                var text = link.text().toLowerCase();
+
+                if (text.indexOf(val) > -1)
+                    link.show();
+                else
+                    link.hide();
+            });
         }
-    },
+    };
 
-    PageControl.prototype.setTab = function(name) {
-        if (name == this.tab) return;
+    function noop(event) {
+        event.preventDefault();
+    };
 
-        $('#' + name + 'List').show();
-        $('#' + this.tab + 'List').hide();
+    function show(hashPrefix, showFunc) {
+        return function(event) {
+            event.preventDefault();
+
+            const target = $(event.target);
+            const val = target.data('value');
+            const hash = hashPrefix + encodeRFC3986URIComponent(val);
+            wh.skip(hash);
+            window.location.hash = hash;
 
-        $('#' + name + 'Tab').removeClass('inactive');
-        $('#' + name + 'Tab').addClass('active');
+            showFunc(val);
+        };
+    };
 
-        $('#' + this.tab + 'Tab').removeClass('active');
-        $('#' + this.tab + 'Tab').addClass('inactive');
+    var jukebox = new Jukebox();
+    jukebox.sync();
 
-        this.tab = name;
+    var wh = new WindowHandler(jukebox);
 
-        window.location = "#tab=" + name;
-        this.url = window.location.href;
+    $('#artistSearch').keyup(filter($('li.artist')));
+    $('#genreSearch').keyup(filter($('li.genre')));
+    $('#artistSearchForm').submit(noop);
+    $('#genreSearchForm').submit(noop);
+    $('li.artist a').click(show('#artist=', $.proxy(jukebox.showArtist, jukebox)));
+    $('li.genre a').click(show('#genre=', $.proxy(jukebox.showGenre, jukebox)));
+
+    function addControl(key) {
+        $('#control-' + key).click(function() {
+            jukebox.control(key);
+            return false;
+        });
     }
 
-$(document).ready(function() {
-    var jukebox = new JukeboxView();
-    jukebox.attach();
-    jukebox.sync();
+    if ($('#controls')) {
+        addControl('prev');
+        addControl('pause');
+        addControl('play');
+        addControl('next');
+        addControl('voldown');
+        addControl('volup');
+        addControl('rebuild');
+    }
 });
```

### Comparing `fookebox-0.7.3/fookebox/public/js/jquery/jquery-1.11.3.min.js` & `fookebox-1.0.0/src/fookebox/js/jquery-1.12.4.min.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,165 +1,158 @@
-/*! jQuery v1.11.3 | (c) 2005, 2015 jQuery Foundation, Inc. | jquery.org/license */ ! function(a, b) {
+/*! jQuery v1.12.4 | (c) jQuery Foundation | jquery.org/license */ ! function(a, b) {
     "object" == typeof module && "object" == typeof module.exports ? module.exports = a.document ? b(a, !0) : function(a) {
         if (!a.document) throw new Error("jQuery requires a window with a document");
         return b(a)
     } : b(a)
 }("undefined" != typeof window ? window : this, function(a, b) {
     var c = [],
-        d = c.slice,
-        e = c.concat,
-        f = c.push,
-        g = c.indexOf,
-        h = {},
-        i = h.toString,
-        j = h.hasOwnProperty,
-        k = {},
-        l = "1.11.3",
-        m = function(a, b) {
-            return new m.fn.init(a, b)
-        },
-        n = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g,
-        o = /^-ms-/,
-        p = /-([\da-z])/gi,
-        q = function(a, b) {
+        d = a.document,
+        e = c.slice,
+        f = c.concat,
+        g = c.push,
+        h = c.indexOf,
+        i = {},
+        j = i.toString,
+        k = i.hasOwnProperty,
+        l = {},
+        m = "1.12.4",
+        n = function(a, b) {
+            return new n.fn.init(a, b)
+        },
+        o = /^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g,
+        p = /^-ms-/,
+        q = /-([\da-z])/gi,
+        r = function(a, b) {
             return b.toUpperCase()
         };
-    m.fn = m.prototype = {
-        jquery: l,
-        constructor: m,
+    n.fn = n.prototype = {
+        jquery: m,
+        constructor: n,
         selector: "",
         length: 0,
         toArray: function() {
-            return d.call(this)
+            return e.call(this)
         },
         get: function(a) {
-            return null != a ? 0 > a ? this[a + this.length] : this[a] : d.call(this)
+            return null != a ? 0 > a ? this[a + this.length] : this[a] : e.call(this)
         },
         pushStack: function(a) {
-            var b = m.merge(this.constructor(), a);
+            var b = n.merge(this.constructor(), a);
             return b.prevObject = this, b.context = this.context, b
         },
-        each: function(a, b) {
-            return m.each(this, a, b)
+        each: function(a) {
+            return n.each(this, a)
         },
         map: function(a) {
-            return this.pushStack(m.map(this, function(b, c) {
+            return this.pushStack(n.map(this, function(b, c) {
                 return a.call(b, c, b)
             }))
         },
         slice: function() {
-            return this.pushStack(d.apply(this, arguments))
+            return this.pushStack(e.apply(this, arguments))
         },
         first: function() {
             return this.eq(0)
         },
         last: function() {
             return this.eq(-1)
         },
         eq: function(a) {
             var b = this.length,
                 c = +a + (0 > a ? b : 0);
             return this.pushStack(c >= 0 && b > c ? [this[c]] : [])
         },
         end: function() {
-            return this.prevObject || this.constructor(null)
+            return this.prevObject || this.constructor()
         },
-        push: f,
+        push: g,
         sort: c.sort,
         splice: c.splice
-    }, m.extend = m.fn.extend = function() {
+    }, n.extend = n.fn.extend = function() {
         var a, b, c, d, e, f, g = arguments[0] || {},
             h = 1,
             i = arguments.length,
             j = !1;
-        for ("boolean" == typeof g && (j = g, g = arguments[h] || {}, h++), "object" == typeof g || m.isFunction(g) || (g = {}), h === i && (g = this, h--); i > h; h++)
+        for ("boolean" == typeof g && (j = g, g = arguments[h] || {}, h++), "object" == typeof g || n.isFunction(g) || (g = {}), h === i && (g = this, h--); i > h; h++)
             if (null != (e = arguments[h]))
-                for (d in e) a = g[d], c = e[d], g !== c && (j && c && (m.isPlainObject(c) || (b = m.isArray(c))) ? (b ? (b = !1, f = a && m.isArray(a) ? a : []) : f = a && m.isPlainObject(a) ? a : {}, g[d] = m.extend(j, f, c)) : void 0 !== c && (g[d] = c));
+                for (d in e) a = g[d], c = e[d], g !== c && (j && c && (n.isPlainObject(c) || (b = n.isArray(c))) ? (b ? (b = !1, f = a && n.isArray(a) ? a : []) : f = a && n.isPlainObject(a) ? a : {}, g[d] = n.extend(j, f, c)) : void 0 !== c && (g[d] = c));
         return g
-    }, m.extend({
-        expando: "jQuery" + (l + Math.random()).replace(/\D/g, ""),
+    }, n.extend({
+        expando: "jQuery" + (m + Math.random()).replace(/\D/g, ""),
         isReady: !0,
         error: function(a) {
             throw new Error(a)
         },
         noop: function() {},
         isFunction: function(a) {
-            return "function" === m.type(a)
+            return "function" === n.type(a)
         },
         isArray: Array.isArray || function(a) {
-            return "array" === m.type(a)
+            return "array" === n.type(a)
         },
         isWindow: function(a) {
             return null != a && a == a.window
         },
         isNumeric: function(a) {
-            return !m.isArray(a) && a - parseFloat(a) + 1 >= 0
+            var b = a && a.toString();
+            return !n.isArray(a) && b - parseFloat(b) + 1 >= 0
         },
         isEmptyObject: function(a) {
             var b;
             for (b in a) return !1;
             return !0
         },
         isPlainObject: function(a) {
             var b;
-            if (!a || "object" !== m.type(a) || a.nodeType || m.isWindow(a)) return !1;
+            if (!a || "object" !== n.type(a) || a.nodeType || n.isWindow(a)) return !1;
             try {
-                if (a.constructor && !j.call(a, "constructor") && !j.call(a.constructor.prototype, "isPrototypeOf")) return !1
+                if (a.constructor && !k.call(a, "constructor") && !k.call(a.constructor.prototype, "isPrototypeOf")) return !1
             } catch (c) {
                 return !1
             }
-            if (k.ownLast)
-                for (b in a) return j.call(a, b);
+            if (!l.ownFirst)
+                for (b in a) return k.call(a, b);
             for (b in a);
-            return void 0 === b || j.call(a, b)
+            return void 0 === b || k.call(a, b)
         },
         type: function(a) {
-            return null == a ? a + "" : "object" == typeof a || "function" == typeof a ? h[i.call(a)] || "object" : typeof a
+            return null == a ? a + "" : "object" == typeof a || "function" == typeof a ? i[j.call(a)] || "object" : typeof a
         },
         globalEval: function(b) {
-            b && m.trim(b) && (a.execScript || function(b) {
+            b && n.trim(b) && (a.execScript || function(b) {
                 a.eval.call(a, b)
             })(b)
         },
         camelCase: function(a) {
-            return a.replace(o, "ms-").replace(p, q)
+            return a.replace(p, "ms-").replace(q, r)
         },
         nodeName: function(a, b) {
             return a.nodeName && a.nodeName.toLowerCase() === b.toLowerCase()
         },
-        each: function(a, b, c) {
-            var d, e = 0,
-                f = a.length,
-                g = r(a);
-            if (c) {
-                if (g) {
-                    for (; f > e; e++)
-                        if (d = b.apply(a[e], c), d === !1) break
-                } else
-                    for (e in a)
-                        if (d = b.apply(a[e], c), d === !1) break
-            } else if (g) {
-                for (; f > e; e++)
-                    if (d = b.call(a[e], e, a[e]), d === !1) break
+        each: function(a, b) {
+            var c, d = 0;
+            if (s(a)) {
+                for (c = a.length; c > d; d++)
+                    if (b.call(a[d], d, a[d]) === !1) break
             } else
-                for (e in a)
-                    if (d = b.call(a[e], e, a[e]), d === !1) break;
+                for (d in a)
+                    if (b.call(a[d], d, a[d]) === !1) break;
             return a
         },
         trim: function(a) {
-            return null == a ? "" : (a + "").replace(n, "")
+            return null == a ? "" : (a + "").replace(o, "")
         },
         makeArray: function(a, b) {
             var c = b || [];
-            return null != a && (r(Object(a)) ? m.merge(c, "string" == typeof a ? [a] : a) : f.call(c, a)), c
+            return null != a && (s(Object(a)) ? n.merge(c, "string" == typeof a ? [a] : a) : g.call(c, a)), c
         },
         inArray: function(a, b, c) {
             var d;
             if (b) {
-                if (g) return g.call(b, a, c);
+                if (h) return h.call(b, a, c);
                 for (d = b.length, c = c ? 0 > c ? Math.max(0, d + c) : c : 0; d > c; c++)
                     if (c in b && b[c] === a) return c
             }
             return -1
         },
         merge: function(a, b) {
             var c = +b.length,
@@ -171,52 +164,50 @@
             return a.length = e, a
         },
         grep: function(a, b, c) {
             for (var d, e = [], f = 0, g = a.length, h = !c; g > f; f++) d = !b(a[f], f), d !== h && e.push(a[f]);
             return e
         },
         map: function(a, b, c) {
-            var d, f = 0,
-                g = a.length,
-                h = r(a),
-                i = [];
-            if (h)
-                for (; g > f; f++) d = b(a[f], f, c), null != d && i.push(d);
+            var d, e, g = 0,
+                h = [];
+            if (s(a))
+                for (d = a.length; d > g; g++) e = b(a[g], g, c), null != e && h.push(e);
             else
-                for (f in a) d = b(a[f], f, c), null != d && i.push(d);
-            return e.apply([], i)
+                for (g in a) e = b(a[g], g, c), null != e && h.push(e);
+            return f.apply([], h)
         },
         guid: 1,
         proxy: function(a, b) {
-            var c, e, f;
-            return "string" == typeof b && (f = a[b], b = a, a = f), m.isFunction(a) ? (c = d.call(arguments, 2), e = function() {
-                return a.apply(b || this, c.concat(d.call(arguments)))
-            }, e.guid = a.guid = a.guid || m.guid++, e) : void 0
+            var c, d, f;
+            return "string" == typeof b && (f = a[b], b = a, a = f), n.isFunction(a) ? (c = e.call(arguments, 2), d = function() {
+                return a.apply(b || this, c.concat(e.call(arguments)))
+            }, d.guid = a.guid = a.guid || n.guid++, d) : void 0
         },
         now: function() {
             return +new Date
         },
-        support: k
-    }), m.each("Boolean Number String Function Array Date RegExp Object Error".split(" "), function(a, b) {
-        h["[object " + b + "]"] = b.toLowerCase()
+        support: l
+    }), "function" == typeof Symbol && (n.fn[Symbol.iterator] = c[Symbol.iterator]), n.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), function(a, b) {
+        i["[object " + b + "]"] = b.toLowerCase()
     });
 
-    function r(a) {
-        var b = "length" in a && a.length,
-            c = m.type(a);
-        return "function" === c || m.isWindow(a) ? !1 : 1 === a.nodeType && b ? !0 : "array" === c || 0 === b || "number" == typeof b && b > 0 && b - 1 in a
+    function s(a) {
+        var b = !!a && "length" in a && a.length,
+            c = n.type(a);
+        return "function" === c || n.isWindow(a) ? !1 : "array" === c || 0 === b || "number" == typeof b && b > 0 && b - 1 in a
     }
-    var s = function(a) {
+    var t = function(a) {
         var b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u = "sizzle" + 1 * new Date,
             v = a.document,
             w = 0,
             x = 0,
-            y = ha(),
-            z = ha(),
-            A = ha(),
+            y = ga(),
+            z = ga(),
+            A = ga(),
             B = function(a, b) {
                 return a === b && (l = !0), 0
             },
             C = 1 << 31,
             D = {}.hasOwnProperty,
             E = [],
             F = E.pop,
@@ -227,182 +218,183 @@
                 for (var c = 0, d = a.length; d > c; c++)
                     if (a[c] === b) return c;
                 return -1
             },
             K = "checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",
             L = "[\\x20\\t\\r\\n\\f]",
             M = "(?:\\\\.|[\\w-]|[^\\x00-\\xa0])+",
-            N = M.replace("w", "w#"),
-            O = "\\[" + L + "*(" + M + ")(?:" + L + "*([*^$|!~]?=)" + L + "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + N + "))|)" + L + "*\\]",
-            P = ":(" + M + ")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|" + O + ")*)|.*)\\)|)",
-            Q = new RegExp(L + "+", "g"),
-            R = new RegExp("^" + L + "+|((?:^|[^\\\\])(?:\\\\.)*)" + L + "+$", "g"),
-            S = new RegExp("^" + L + "*," + L + "*"),
-            T = new RegExp("^" + L + "*([>+~]|" + L + ")" + L + "*"),
-            U = new RegExp("=" + L + "*([^\\]'\"]*?)" + L + "*\\]", "g"),
-            V = new RegExp(P),
-            W = new RegExp("^" + N + "$"),
-            X = {
+            N = "\\[" + L + "*(" + M + ")(?:" + L + "*([*^$|!~]?=)" + L + "*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|(" + M + "))|)" + L + "*\\]",
+            O = ":(" + M + ")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|" + N + ")*)|.*)\\)|)",
+            P = new RegExp(L + "+", "g"),
+            Q = new RegExp("^" + L + "+|((?:^|[^\\\\])(?:\\\\.)*)" + L + "+$", "g"),
+            R = new RegExp("^" + L + "*," + L + "*"),
+            S = new RegExp("^" + L + "*([>+~]|" + L + ")" + L + "*"),
+            T = new RegExp("=" + L + "*([^\\]'\"]*?)" + L + "*\\]", "g"),
+            U = new RegExp(O),
+            V = new RegExp("^" + M + "$"),
+            W = {
                 ID: new RegExp("^#(" + M + ")"),
                 CLASS: new RegExp("^\\.(" + M + ")"),
-                TAG: new RegExp("^(" + M.replace("w", "w*") + ")"),
-                ATTR: new RegExp("^" + O),
-                PSEUDO: new RegExp("^" + P),
+                TAG: new RegExp("^(" + M + "|[*])"),
+                ATTR: new RegExp("^" + N),
+                PSEUDO: new RegExp("^" + O),
                 CHILD: new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\(" + L + "*(even|odd|(([+-]|)(\\d*)n|)" + L + "*(?:([+-]|)" + L + "*(\\d+)|))" + L + "*\\)|)", "i"),
                 bool: new RegExp("^(?:" + K + ")$", "i"),
                 needsContext: new RegExp("^" + L + "*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\(" + L + "*((?:-\\d)?\\d*)" + L + "*\\)|)(?=[^-]|$)", "i")
             },
-            Y = /^(?:input|select|textarea|button)$/i,
-            Z = /^h\d$/i,
-            $ = /^[^{]+\{\s*\[native \w/,
-            _ = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
-            aa = /[+~]/,
-            ba = /'|\\/g,
-            ca = new RegExp("\\\\([\\da-f]{1,6}" + L + "?|(" + L + ")|.)", "ig"),
-            da = function(a, b, c) {
+            X = /^(?:input|select|textarea|button)$/i,
+            Y = /^h\d$/i,
+            Z = /^[^{]+\{\s*\[native \w/,
+            $ = /^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,
+            _ = /[+~]/,
+            aa = /'|\\/g,
+            ba = new RegExp("\\\\([\\da-f]{1,6}" + L + "?|(" + L + ")|.)", "ig"),
+            ca = function(a, b, c) {
                 var d = "0x" + b - 65536;
                 return d !== d || c ? b : 0 > d ? String.fromCharCode(d + 65536) : String.fromCharCode(d >> 10 | 55296, 1023 & d | 56320)
             },
-            ea = function() {
+            da = function() {
                 m()
             };
         try {
             H.apply(E = I.call(v.childNodes), v.childNodes), E[v.childNodes.length].nodeType
-        } catch (fa) {
+        } catch (ea) {
             H = {
                 apply: E.length ? function(a, b) {
                     G.apply(a, I.call(b))
                 } : function(a, b) {
                     var c = a.length,
                         d = 0;
                     while (a[c++] = b[d++]);
                     a.length = c - 1
                 }
             }
         }
 
-        function ga(a, b, d, e) {
-            var f, h, j, k, l, o, r, s, w, x;
-            if ((b ? b.ownerDocument || b : v) !== n && m(b), b = b || n, d = d || [], k = b.nodeType, "string" != typeof a || !a || 1 !== k && 9 !== k && 11 !== k) return d;
-            if (!e && p) {
-                if (11 !== k && (f = _.exec(a)))
-                    if (j = f[1]) {
-                        if (9 === k) {
-                            if (h = b.getElementById(j), !h || !h.parentNode) return d;
-                            if (h.id === j) return d.push(h), d
-                        } else if (b.ownerDocument && (h = b.ownerDocument.getElementById(j)) && t(b, h) && h.id === j) return d.push(h), d
+        function fa(a, b, d, e) {
+            var f, h, j, k, l, o, r, s, w = b && b.ownerDocument,
+                x = b ? b.nodeType : 9;
+            if (d = d || [], "string" != typeof a || !a || 1 !== x && 9 !== x && 11 !== x) return d;
+            if (!e && ((b ? b.ownerDocument || b : v) !== n && m(b), b = b || n, p)) {
+                if (11 !== x && (o = $.exec(a)))
+                    if (f = o[1]) {
+                        if (9 === x) {
+                            if (!(j = b.getElementById(f))) return d;
+                            if (j.id === f) return d.push(j), d
+                        } else if (w && (j = w.getElementById(f)) && t(b, j) && j.id === f) return d.push(j), d
                     } else {
-                        if (f[2]) return H.apply(d, b.getElementsByTagName(a)), d;
-                        if ((j = f[3]) && c.getElementsByClassName) return H.apply(d, b.getElementsByClassName(j)), d
-                    } if (c.qsa && (!q || !q.test(a))) {
-                    if (s = r = u, w = b, x = 1 !== k && a, 1 === k && "object" !== b.nodeName.toLowerCase()) {
-                        o = g(a), (r = b.getAttribute("id")) ? s = r.replace(ba, "\\$&") : b.setAttribute("id", s), s = "[id='" + s + "'] ", l = o.length;
-                        while (l--) o[l] = s + ra(o[l]);
-                        w = aa.test(a) && pa(b.parentNode) || b, x = o.join(",")
+                        if (o[2]) return H.apply(d, b.getElementsByTagName(a)), d;
+                        if ((f = o[3]) && c.getElementsByClassName && b.getElementsByClassName) return H.apply(d, b.getElementsByClassName(f)), d
+                    } if (c.qsa && !A[a + " "] && (!q || !q.test(a))) {
+                    if (1 !== x) w = b, s = a;
+                    else if ("object" !== b.nodeName.toLowerCase()) {
+                        (k = b.getAttribute("id")) ? k = k.replace(aa, "\\$&"): b.setAttribute("id", k = u), r = g(a), h = r.length, l = V.test(k) ? "#" + k : "[id='" + k + "']";
+                        while (h--) r[h] = l + " " + qa(r[h]);
+                        s = r.join(","), w = _.test(a) && oa(b.parentNode) || b
                     }
-                    if (x) try {
-                        return H.apply(d, w.querySelectorAll(x)), d
+                    if (s) try {
+                        return H.apply(d, w.querySelectorAll(s)), d
                     } catch (y) {} finally {
-                        r || b.removeAttribute("id")
+                        k === u && b.removeAttribute("id")
                     }
                 }
             }
-            return i(a.replace(R, "$1"), b, d, e)
+            return i(a.replace(Q, "$1"), b, d, e)
         }
 
-        function ha() {
+        function ga() {
             var a = [];
 
             function b(c, e) {
                 return a.push(c + " ") > d.cacheLength && delete b[a.shift()], b[c + " "] = e
             }
             return b
         }
 
-        function ia(a) {
+        function ha(a) {
             return a[u] = !0, a
         }
 
-        function ja(a) {
+        function ia(a) {
             var b = n.createElement("div");
             try {
                 return !!a(b)
             } catch (c) {
                 return !1
             } finally {
                 b.parentNode && b.parentNode.removeChild(b), b = null
             }
         }
 
-        function ka(a, b) {
+        function ja(a, b) {
             var c = a.split("|"),
-                e = a.length;
+                e = c.length;
             while (e--) d.attrHandle[c[e]] = b
         }
 
-        function la(a, b) {
+        function ka(a, b) {
             var c = b && a,
                 d = c && 1 === a.nodeType && 1 === b.nodeType && (~b.sourceIndex || C) - (~a.sourceIndex || C);
             if (d) return d;
             if (c)
                 while (c = c.nextSibling)
                     if (c === b) return -1;
             return a ? 1 : -1
         }
 
-        function ma(a) {
+        function la(a) {
             return function(b) {
                 var c = b.nodeName.toLowerCase();
                 return "input" === c && b.type === a
             }
         }
 
-        function na(a) {
+        function ma(a) {
             return function(b) {
                 var c = b.nodeName.toLowerCase();
                 return ("input" === c || "button" === c) && b.type === a
             }
         }
 
-        function oa(a) {
-            return ia(function(b) {
-                return b = +b, ia(function(c, d) {
+        function na(a) {
+            return ha(function(b) {
+                return b = +b, ha(function(c, d) {
                     var e, f = a([], c.length, b),
                         g = f.length;
                     while (g--) c[e = f[g]] && (c[e] = !(d[e] = c[e]))
                 })
             })
         }
 
-        function pa(a) {
+        function oa(a) {
             return a && "undefined" != typeof a.getElementsByTagName && a
         }
-        c = ga.support = {}, f = ga.isXML = function(a) {
+        c = fa.support = {}, f = fa.isXML = function(a) {
             var b = a && (a.ownerDocument || a).documentElement;
             return b ? "HTML" !== b.nodeName : !1
-        }, m = ga.setDocument = function(a) {
+        }, m = fa.setDocument = function(a) {
             var b, e, g = a ? a.ownerDocument || a : v;
-            return g !== n && 9 === g.nodeType && g.documentElement ? (n = g, o = g.documentElement, e = g.defaultView, e && e !== e.top && (e.addEventListener ? e.addEventListener("unload", ea, !1) : e.attachEvent && e.attachEvent("onunload", ea)), p = !f(g), c.attributes = ja(function(a) {
+            return g !== n && 9 === g.nodeType && g.documentElement ? (n = g, o = n.documentElement, p = !f(n), (e = n.defaultView) && e.top !== e && (e.addEventListener ? e.addEventListener("unload", da, !1) : e.attachEvent && e.attachEvent("onunload", da)), c.attributes = ia(function(a) {
                 return a.className = "i", !a.getAttribute("className")
-            }), c.getElementsByTagName = ja(function(a) {
-                return a.appendChild(g.createComment("")), !a.getElementsByTagName("*").length
-            }), c.getElementsByClassName = $.test(g.getElementsByClassName), c.getById = ja(function(a) {
-                return o.appendChild(a).id = u, !g.getElementsByName || !g.getElementsByName(u).length
+            }), c.getElementsByTagName = ia(function(a) {
+                return a.appendChild(n.createComment("")), !a.getElementsByTagName("*").length
+            }), c.getElementsByClassName = Z.test(n.getElementsByClassName), c.getById = ia(function(a) {
+                return o.appendChild(a).id = u, !n.getElementsByName || !n.getElementsByName(u).length
             }), c.getById ? (d.find.ID = function(a, b) {
                 if ("undefined" != typeof b.getElementById && p) {
                     var c = b.getElementById(a);
-                    return c && c.parentNode ? [c] : []
+                    return c ? [c] : []
                 }
             }, d.filter.ID = function(a) {
-                var b = a.replace(ca, da);
+                var b = a.replace(ba, ca);
                 return function(a) {
                     return a.getAttribute("id") === b
                 }
             }) : (delete d.find.ID, d.filter.ID = function(a) {
-                var b = a.replace(ca, da);
+                var b = a.replace(ba, ca);
                 return function(a) {
                     var c = "undefined" != typeof a.getAttributeNode && a.getAttributeNode("id");
                     return c && c.value === b
                 }
             }), d.find.TAG = c.getElementsByTagName ? function(a, b) {
                 return "undefined" != typeof b.getElementsByTagName ? b.getElementsByTagName(a) : c.qsa ? b.querySelectorAll(a) : void 0
             } : function(a, b) {
@@ -411,93 +403,93 @@
                     f = b.getElementsByTagName(a);
                 if ("*" === a) {
                     while (c = f[e++]) 1 === c.nodeType && d.push(c);
                     return d
                 }
                 return f
             }, d.find.CLASS = c.getElementsByClassName && function(a, b) {
-                return p ? b.getElementsByClassName(a) : void 0
-            }, r = [], q = [], (c.qsa = $.test(g.querySelectorAll)) && (ja(function(a) {
-                o.appendChild(a).innerHTML = "<a id='" + u + "'></a><select id='" + u + "-\f]' msallowcapture=''><option selected=''></option></select>", a.querySelectorAll("[msallowcapture^='']").length && q.push("[*^$]=" + L + "*(?:''|\"\")"), a.querySelectorAll("[selected]").length || q.push("\\[" + L + "*(?:value|" + K + ")"), a.querySelectorAll("[id~=" + u + "-]").length || q.push("~="), a.querySelectorAll(":checked").length || q.push(":checked"), a.querySelectorAll("a#" + u + "+*").length || q.push(".#.+[+~]")
-            }), ja(function(a) {
-                var b = g.createElement("input");
+                return "undefined" != typeof b.getElementsByClassName && p ? b.getElementsByClassName(a) : void 0
+            }, r = [], q = [], (c.qsa = Z.test(n.querySelectorAll)) && (ia(function(a) {
+                o.appendChild(a).innerHTML = "<a id='" + u + "'></a><select id='" + u + "-\r\\' msallowcapture=''><option selected=''></option></select>", a.querySelectorAll("[msallowcapture^='']").length && q.push("[*^$]=" + L + "*(?:''|\"\")"), a.querySelectorAll("[selected]").length || q.push("\\[" + L + "*(?:value|" + K + ")"), a.querySelectorAll("[id~=" + u + "-]").length || q.push("~="), a.querySelectorAll(":checked").length || q.push(":checked"), a.querySelectorAll("a#" + u + "+*").length || q.push(".#.+[+~]")
+            }), ia(function(a) {
+                var b = n.createElement("input");
                 b.setAttribute("type", "hidden"), a.appendChild(b).setAttribute("name", "D"), a.querySelectorAll("[name=d]").length && q.push("name" + L + "*[*^$|!~]?="), a.querySelectorAll(":enabled").length || q.push(":enabled", ":disabled"), a.querySelectorAll("*,:x"), q.push(",.*:")
-            })), (c.matchesSelector = $.test(s = o.matches || o.webkitMatchesSelector || o.mozMatchesSelector || o.oMatchesSelector || o.msMatchesSelector)) && ja(function(a) {
-                c.disconnectedMatch = s.call(a, "div"), s.call(a, "[s!='']:x"), r.push("!=", P)
-            }), q = q.length && new RegExp(q.join("|")), r = r.length && new RegExp(r.join("|")), b = $.test(o.compareDocumentPosition), t = b || $.test(o.contains) ? function(a, b) {
+            })), (c.matchesSelector = Z.test(s = o.matches || o.webkitMatchesSelector || o.mozMatchesSelector || o.oMatchesSelector || o.msMatchesSelector)) && ia(function(a) {
+                c.disconnectedMatch = s.call(a, "div"), s.call(a, "[s!='']:x"), r.push("!=", O)
+            }), q = q.length && new RegExp(q.join("|")), r = r.length && new RegExp(r.join("|")), b = Z.test(o.compareDocumentPosition), t = b || Z.test(o.contains) ? function(a, b) {
                 var c = 9 === a.nodeType ? a.documentElement : a,
                     d = b && b.parentNode;
                 return a === d || !(!d || 1 !== d.nodeType || !(c.contains ? c.contains(d) : a.compareDocumentPosition && 16 & a.compareDocumentPosition(d)))
             } : function(a, b) {
                 if (b)
                     while (b = b.parentNode)
                         if (b === a) return !0;
                 return !1
             }, B = b ? function(a, b) {
                 if (a === b) return l = !0, 0;
                 var d = !a.compareDocumentPosition - !b.compareDocumentPosition;
-                return d ? d : (d = (a.ownerDocument || a) === (b.ownerDocument || b) ? a.compareDocumentPosition(b) : 1, 1 & d || !c.sortDetached && b.compareDocumentPosition(a) === d ? a === g || a.ownerDocument === v && t(v, a) ? -1 : b === g || b.ownerDocument === v && t(v, b) ? 1 : k ? J(k, a) - J(k, b) : 0 : 4 & d ? -1 : 1)
+                return d ? d : (d = (a.ownerDocument || a) === (b.ownerDocument || b) ? a.compareDocumentPosition(b) : 1, 1 & d || !c.sortDetached && b.compareDocumentPosition(a) === d ? a === n || a.ownerDocument === v && t(v, a) ? -1 : b === n || b.ownerDocument === v && t(v, b) ? 1 : k ? J(k, a) - J(k, b) : 0 : 4 & d ? -1 : 1)
             } : function(a, b) {
                 if (a === b) return l = !0, 0;
                 var c, d = 0,
                     e = a.parentNode,
                     f = b.parentNode,
-                    h = [a],
-                    i = [b];
-                if (!e || !f) return a === g ? -1 : b === g ? 1 : e ? -1 : f ? 1 : k ? J(k, a) - J(k, b) : 0;
-                if (e === f) return la(a, b);
+                    g = [a],
+                    h = [b];
+                if (!e || !f) return a === n ? -1 : b === n ? 1 : e ? -1 : f ? 1 : k ? J(k, a) - J(k, b) : 0;
+                if (e === f) return ka(a, b);
                 c = a;
-                while (c = c.parentNode) h.unshift(c);
+                while (c = c.parentNode) g.unshift(c);
                 c = b;
-                while (c = c.parentNode) i.unshift(c);
-                while (h[d] === i[d]) d++;
-                return d ? la(h[d], i[d]) : h[d] === v ? -1 : i[d] === v ? 1 : 0
-            }, g) : n
-        }, ga.matches = function(a, b) {
-            return ga(a, null, null, b)
-        }, ga.matchesSelector = function(a, b) {
-            if ((a.ownerDocument || a) !== n && m(a), b = b.replace(U, "='$1']"), !(!c.matchesSelector || !p || r && r.test(b) || q && q.test(b))) try {
+                while (c = c.parentNode) h.unshift(c);
+                while (g[d] === h[d]) d++;
+                return d ? ka(g[d], h[d]) : g[d] === v ? -1 : h[d] === v ? 1 : 0
+            }, n) : n
+        }, fa.matches = function(a, b) {
+            return fa(a, null, null, b)
+        }, fa.matchesSelector = function(a, b) {
+            if ((a.ownerDocument || a) !== n && m(a), b = b.replace(T, "='$1']"), c.matchesSelector && p && !A[b + " "] && (!r || !r.test(b)) && (!q || !q.test(b))) try {
                 var d = s.call(a, b);
                 if (d || c.disconnectedMatch || a.document && 11 !== a.document.nodeType) return d
             } catch (e) {}
-            return ga(b, n, null, [a]).length > 0
-        }, ga.contains = function(a, b) {
+            return fa(b, n, null, [a]).length > 0
+        }, fa.contains = function(a, b) {
             return (a.ownerDocument || a) !== n && m(a), t(a, b)
-        }, ga.attr = function(a, b) {
+        }, fa.attr = function(a, b) {
             (a.ownerDocument || a) !== n && m(a);
             var e = d.attrHandle[b.toLowerCase()],
                 f = e && D.call(d.attrHandle, b.toLowerCase()) ? e(a, b, !p) : void 0;
             return void 0 !== f ? f : c.attributes || !p ? a.getAttribute(b) : (f = a.getAttributeNode(b)) && f.specified ? f.value : null
-        }, ga.error = function(a) {
+        }, fa.error = function(a) {
             throw new Error("Syntax error, unrecognized expression: " + a)
-        }, ga.uniqueSort = function(a) {
+        }, fa.uniqueSort = function(a) {
             var b, d = [],
                 e = 0,
                 f = 0;
             if (l = !c.detectDuplicates, k = !c.sortStable && a.slice(0), a.sort(B), l) {
                 while (b = a[f++]) b === a[f] && (e = d.push(f));
                 while (e--) a.splice(d[e], 1)
             }
             return k = null, a
-        }, e = ga.getText = function(a) {
+        }, e = fa.getText = function(a) {
             var b, c = "",
                 d = 0,
                 f = a.nodeType;
             if (f) {
                 if (1 === f || 9 === f || 11 === f) {
                     if ("string" == typeof a.textContent) return a.textContent;
                     for (a = a.firstChild; a; a = a.nextSibling) c += e(a)
                 } else if (3 === f || 4 === f) return a.nodeValue
             } else
                 while (b = a[d++]) c += e(b);
             return c
-        }, d = ga.selectors = {
+        }, d = fa.selectors = {
             cacheLength: 50,
-            createPseudo: ia,
-            match: X,
+            createPseudo: ha,
+            match: W,
             attrHandle: {},
             find: {},
             relative: {
                 ">": {
                     dir: "parentNode",
                     first: !0
                 },
@@ -510,118 +502,118 @@
                 },
                 "~": {
                     dir: "previousSibling"
                 }
             },
             preFilter: {
                 ATTR: function(a) {
-                    return a[1] = a[1].replace(ca, da), a[3] = (a[3] || a[4] || a[5] || "").replace(ca, da), "~=" === a[2] && (a[3] = " " + a[3] + " "), a.slice(0, 4)
+                    return a[1] = a[1].replace(ba, ca), a[3] = (a[3] || a[4] || a[5] || "").replace(ba, ca), "~=" === a[2] && (a[3] = " " + a[3] + " "), a.slice(0, 4)
                 },
                 CHILD: function(a) {
-                    return a[1] = a[1].toLowerCase(), "nth" === a[1].slice(0, 3) ? (a[3] || ga.error(a[0]), a[4] = +(a[4] ? a[5] + (a[6] || 1) : 2 * ("even" === a[3] || "odd" === a[3])), a[5] = +(a[7] + a[8] || "odd" === a[3])) : a[3] && ga.error(a[0]), a
+                    return a[1] = a[1].toLowerCase(), "nth" === a[1].slice(0, 3) ? (a[3] || fa.error(a[0]), a[4] = +(a[4] ? a[5] + (a[6] || 1) : 2 * ("even" === a[3] || "odd" === a[3])), a[5] = +(a[7] + a[8] || "odd" === a[3])) : a[3] && fa.error(a[0]), a
                 },
                 PSEUDO: function(a) {
                     var b, c = !a[6] && a[2];
-                    return X.CHILD.test(a[0]) ? null : (a[3] ? a[2] = a[4] || a[5] || "" : c && V.test(c) && (b = g(c, !0)) && (b = c.indexOf(")", c.length - b) - c.length) && (a[0] = a[0].slice(0, b), a[2] = c.slice(0, b)), a.slice(0, 3))
+                    return W.CHILD.test(a[0]) ? null : (a[3] ? a[2] = a[4] || a[5] || "" : c && U.test(c) && (b = g(c, !0)) && (b = c.indexOf(")", c.length - b) - c.length) && (a[0] = a[0].slice(0, b), a[2] = c.slice(0, b)), a.slice(0, 3))
                 }
             },
             filter: {
                 TAG: function(a) {
-                    var b = a.replace(ca, da).toLowerCase();
+                    var b = a.replace(ba, ca).toLowerCase();
                     return "*" === a ? function() {
                         return !0
                     } : function(a) {
                         return a.nodeName && a.nodeName.toLowerCase() === b
                     }
                 },
                 CLASS: function(a) {
                     var b = y[a + " "];
                     return b || (b = new RegExp("(^|" + L + ")" + a + "(" + L + "|$)")) && y(a, function(a) {
                         return b.test("string" == typeof a.className && a.className || "undefined" != typeof a.getAttribute && a.getAttribute("class") || "")
                     })
                 },
                 ATTR: function(a, b, c) {
                     return function(d) {
-                        var e = ga.attr(d, a);
-                        return null == e ? "!=" === b : b ? (e += "", "=" === b ? e === c : "!=" === b ? e !== c : "^=" === b ? c && 0 === e.indexOf(c) : "*=" === b ? c && e.indexOf(c) > -1 : "$=" === b ? c && e.slice(-c.length) === c : "~=" === b ? (" " + e.replace(Q, " ") + " ").indexOf(c) > -1 : "|=" === b ? e === c || e.slice(0, c.length + 1) === c + "-" : !1) : !0
+                        var e = fa.attr(d, a);
+                        return null == e ? "!=" === b : b ? (e += "", "=" === b ? e === c : "!=" === b ? e !== c : "^=" === b ? c && 0 === e.indexOf(c) : "*=" === b ? c && e.indexOf(c) > -1 : "$=" === b ? c && e.slice(-c.length) === c : "~=" === b ? (" " + e.replace(P, " ") + " ").indexOf(c) > -1 : "|=" === b ? e === c || e.slice(0, c.length + 1) === c + "-" : !1) : !0
                     }
                 },
                 CHILD: function(a, b, c, d, e) {
                     var f = "nth" !== a.slice(0, 3),
                         g = "last" !== a.slice(-4),
                         h = "of-type" === b;
                     return 1 === d && 0 === e ? function(a) {
                         return !!a.parentNode
                     } : function(b, c, i) {
                         var j, k, l, m, n, o, p = f !== g ? "nextSibling" : "previousSibling",
                             q = b.parentNode,
                             r = h && b.nodeName.toLowerCase(),
-                            s = !i && !h;
+                            s = !i && !h,
+                            t = !1;
                         if (q) {
                             if (f) {
                                 while (p) {
-                                    l = b;
-                                    while (l = l[p])
-                                        if (h ? l.nodeName.toLowerCase() === r : 1 === l.nodeType) return !1;
+                                    m = b;
+                                    while (m = m[p])
+                                        if (h ? m.nodeName.toLowerCase() === r : 1 === m.nodeType) return !1;
                                     o = p = "only" === a && !o && "nextSibling"
                                 }
                                 return !0
                             }
                             if (o = [g ? q.firstChild : q.lastChild], g && s) {
-                                k = q[u] || (q[u] = {}), j = k[a] || [], n = j[0] === w && j[1], m = j[0] === w && j[2], l = n && q.childNodes[n];
-                                while (l = ++n && l && l[p] || (m = n = 0) || o.pop())
-                                    if (1 === l.nodeType && ++m && l === b) {
-                                        k[a] = [w, n, m];
+                                m = q, l = m[u] || (m[u] = {}), k = l[m.uniqueID] || (l[m.uniqueID] = {}), j = k[a] || [], n = j[0] === w && j[1], t = n && j[2], m = n && q.childNodes[n];
+                                while (m = ++n && m && m[p] || (t = n = 0) || o.pop())
+                                    if (1 === m.nodeType && ++t && m === b) {
+                                        k[a] = [w, n, t];
                                         break
                                     }
-                            } else if (s && (j = (b[u] || (b[u] = {}))[a]) && j[0] === w) m = j[1];
-                            else
-                                while (l = ++n && l && l[p] || (m = n = 0) || o.pop())
-                                    if ((h ? l.nodeName.toLowerCase() === r : 1 === l.nodeType) && ++m && (s && ((l[u] || (l[u] = {}))[a] = [w, m]), l === b)) break;
-                            return m -= e, m === d || m % d === 0 && m / d >= 0
+                            } else if (s && (m = b, l = m[u] || (m[u] = {}), k = l[m.uniqueID] || (l[m.uniqueID] = {}), j = k[a] || [], n = j[0] === w && j[1], t = n), t === !1)
+                                while (m = ++n && m && m[p] || (t = n = 0) || o.pop())
+                                    if ((h ? m.nodeName.toLowerCase() === r : 1 === m.nodeType) && ++t && (s && (l = m[u] || (m[u] = {}), k = l[m.uniqueID] || (l[m.uniqueID] = {}), k[a] = [w, t]), m === b)) break;
+                            return t -= e, t === d || t % d === 0 && t / d >= 0
                         }
                     }
                 },
                 PSEUDO: function(a, b) {
-                    var c, e = d.pseudos[a] || d.setFilters[a.toLowerCase()] || ga.error("unsupported pseudo: " + a);
-                    return e[u] ? e(b) : e.length > 1 ? (c = [a, a, "", b], d.setFilters.hasOwnProperty(a.toLowerCase()) ? ia(function(a, c) {
+                    var c, e = d.pseudos[a] || d.setFilters[a.toLowerCase()] || fa.error("unsupported pseudo: " + a);
+                    return e[u] ? e(b) : e.length > 1 ? (c = [a, a, "", b], d.setFilters.hasOwnProperty(a.toLowerCase()) ? ha(function(a, c) {
                         var d, f = e(a, b),
                             g = f.length;
                         while (g--) d = J(a, f[g]), a[d] = !(c[d] = f[g])
                     }) : function(a) {
                         return e(a, 0, c)
                     }) : e
                 }
             },
             pseudos: {
-                not: ia(function(a) {
+                not: ha(function(a) {
                     var b = [],
                         c = [],
-                        d = h(a.replace(R, "$1"));
-                    return d[u] ? ia(function(a, b, c, e) {
+                        d = h(a.replace(Q, "$1"));
+                    return d[u] ? ha(function(a, b, c, e) {
                         var f, g = d(a, null, e, []),
                             h = a.length;
                         while (h--)(f = g[h]) && (a[h] = !(b[h] = f))
                     }) : function(a, e, f) {
                         return b[0] = a, d(b, null, f, c), b[0] = null, !c.pop()
                     }
                 }),
-                has: ia(function(a) {
+                has: ha(function(a) {
                     return function(b) {
-                        return ga(a, b).length > 0
+                        return fa(a, b).length > 0
                     }
                 }),
-                contains: ia(function(a) {
-                    return a = a.replace(ca, da),
+                contains: ha(function(a) {
+                    return a = a.replace(ba, ca),
                         function(b) {
                             return (b.textContent || b.innerText || e(b)).indexOf(a) > -1
                         }
                 }),
-                lang: ia(function(a) {
-                    return W.test(a || "") || ga.error("unsupported lang: " + a), a = a.replace(ca, da).toLowerCase(),
+                lang: ha(function(a) {
+                    return V.test(a || "") || fa.error("unsupported lang: " + a), a = a.replace(ba, ca).toLowerCase(),
                         function(b) {
                             var c;
                             do
                                 if (c = p ? b.lang : b.getAttribute("xml:lang") || b.getAttribute("lang")) return c = c.toLowerCase(), c === a || 0 === c.indexOf(a + "-"); while ((b = b.parentNode) && 1 === b.nodeType);
                             return !1
                         }
                 }),
@@ -653,2182 +645,2209 @@
                         if (a.nodeType < 6) return !1;
                     return !0
                 },
                 parent: function(a) {
                     return !d.pseudos.empty(a)
                 },
                 header: function(a) {
-                    return Z.test(a.nodeName)
+                    return Y.test(a.nodeName)
                 },
                 input: function(a) {
-                    return Y.test(a.nodeName)
+                    return X.test(a.nodeName)
                 },
                 button: function(a) {
                     var b = a.nodeName.toLowerCase();
                     return "input" === b && "button" === a.type || "button" === b
                 },
                 text: function(a) {
                     var b;
                     return "input" === a.nodeName.toLowerCase() && "text" === a.type && (null == (b = a.getAttribute("type")) || "text" === b.toLowerCase())
                 },
-                first: oa(function() {
+                first: na(function() {
                     return [0]
                 }),
-                last: oa(function(a, b) {
+                last: na(function(a, b) {
                     return [b - 1]
                 }),
-                eq: oa(function(a, b, c) {
+                eq: na(function(a, b, c) {
                     return [0 > c ? c + b : c]
                 }),
-                even: oa(function(a, b) {
+                even: na(function(a, b) {
                     for (var c = 0; b > c; c += 2) a.push(c);
                     return a
                 }),
-                odd: oa(function(a, b) {
+                odd: na(function(a, b) {
                     for (var c = 1; b > c; c += 2) a.push(c);
                     return a
                 }),
-                lt: oa(function(a, b, c) {
+                lt: na(function(a, b, c) {
                     for (var d = 0 > c ? c + b : c; --d >= 0;) a.push(d);
                     return a
                 }),
-                gt: oa(function(a, b, c) {
+                gt: na(function(a, b, c) {
                     for (var d = 0 > c ? c + b : c; ++d < b;) a.push(d);
                     return a
                 })
             }
         }, d.pseudos.nth = d.pseudos.eq;
         for (b in {
                 radio: !0,
                 checkbox: !0,
                 file: !0,
                 password: !0,
                 image: !0
-            }) d.pseudos[b] = ma(b);
+            }) d.pseudos[b] = la(b);
         for (b in {
                 submit: !0,
                 reset: !0
-            }) d.pseudos[b] = na(b);
+            }) d.pseudos[b] = ma(b);
 
-        function qa() {}
-        qa.prototype = d.filters = d.pseudos, d.setFilters = new qa, g = ga.tokenize = function(a, b) {
+        function pa() {}
+        pa.prototype = d.filters = d.pseudos, d.setFilters = new pa, g = fa.tokenize = function(a, b) {
             var c, e, f, g, h, i, j, k = z[a + " "];
             if (k) return b ? 0 : k.slice(0);
             h = a, i = [], j = d.preFilter;
             while (h) {
-                (!c || (e = S.exec(h))) && (e && (h = h.slice(e[0].length) || h), i.push(f = [])), c = !1, (e = T.exec(h)) && (c = e.shift(), f.push({
+                c && !(e = R.exec(h)) || (e && (h = h.slice(e[0].length) || h), i.push(f = [])), c = !1, (e = S.exec(h)) && (c = e.shift(), f.push({
                     value: c,
-                    type: e[0].replace(R, " ")
+                    type: e[0].replace(Q, " ")
                 }), h = h.slice(c.length));
-                for (g in d.filter) !(e = X[g].exec(h)) || j[g] && !(e = j[g](e)) || (c = e.shift(), f.push({
+                for (g in d.filter) !(e = W[g].exec(h)) || j[g] && !(e = j[g](e)) || (c = e.shift(), f.push({
                     value: c,
                     type: g,
                     matches: e
                 }), h = h.slice(c.length));
                 if (!c) break
             }
-            return b ? h.length : h ? ga.error(a) : z(a, i).slice(0)
+            return b ? h.length : h ? fa.error(a) : z(a, i).slice(0)
         };
 
-        function ra(a) {
+        function qa(a) {
             for (var b = 0, c = a.length, d = ""; c > b; b++) d += a[b].value;
             return d
         }
 
-        function sa(a, b, c) {
+        function ra(a, b, c) {
             var d = b.dir,
                 e = c && "parentNode" === d,
                 f = x++;
             return b.first ? function(b, c, f) {
                 while (b = b[d])
                     if (1 === b.nodeType || e) return a(b, c, f)
             } : function(b, c, g) {
-                var h, i, j = [w, f];
+                var h, i, j, k = [w, f];
                 if (g) {
                     while (b = b[d])
                         if ((1 === b.nodeType || e) && a(b, c, g)) return !0
                 } else
                     while (b = b[d])
                         if (1 === b.nodeType || e) {
-                            if (i = b[u] || (b[u] = {}), (h = i[d]) && h[0] === w && h[1] === f) return j[2] = h[2];
-                            if (i[d] = j, j[2] = a(b, c, g)) return !0
+                            if (j = b[u] || (b[u] = {}), i = j[b.uniqueID] || (j[b.uniqueID] = {}), (h = i[d]) && h[0] === w && h[1] === f) return k[2] = h[2];
+                            if (i[d] = k, k[2] = a(b, c, g)) return !0
                         }
             }
         }
 
-        function ta(a) {
+        function sa(a) {
             return a.length > 1 ? function(b, c, d) {
                 var e = a.length;
                 while (e--)
                     if (!a[e](b, c, d)) return !1;
                 return !0
             } : a[0]
         }
 
-        function ua(a, b, c) {
-            for (var d = 0, e = b.length; e > d; d++) ga(a, b[d], c);
+        function ta(a, b, c) {
+            for (var d = 0, e = b.length; e > d; d++) fa(a, b[d], c);
             return c
         }
 
-        function va(a, b, c, d, e) {
-            for (var f, g = [], h = 0, i = a.length, j = null != b; i > h; h++)(f = a[h]) && (!c || c(f, d, e)) && (g.push(f), j && b.push(h));
+        function ua(a, b, c, d, e) {
+            for (var f, g = [], h = 0, i = a.length, j = null != b; i > h; h++)(f = a[h]) && (c && !c(f, d, e) || (g.push(f), j && b.push(h)));
             return g
         }
 
-        function wa(a, b, c, d, e, f) {
-            return d && !d[u] && (d = wa(d)), e && !e[u] && (e = wa(e, f)), ia(function(f, g, h, i) {
+        function va(a, b, c, d, e, f) {
+            return d && !d[u] && (d = va(d)), e && !e[u] && (e = va(e, f)), ha(function(f, g, h, i) {
                 var j, k, l, m = [],
                     n = [],
                     o = g.length,
-                    p = f || ua(b || "*", h.nodeType ? [h] : h, []),
-                    q = !a || !f && b ? p : va(p, m, a, h, i),
+                    p = f || ta(b || "*", h.nodeType ? [h] : h, []),
+                    q = !a || !f && b ? p : ua(p, m, a, h, i),
                     r = c ? e || (f ? a : o || d) ? [] : g : q;
                 if (c && c(q, r, h, i), d) {
-                    j = va(r, n), d(j, [], h, i), k = j.length;
+                    j = ua(r, n), d(j, [], h, i), k = j.length;
                     while (k--)(l = j[k]) && (r[n[k]] = !(q[n[k]] = l))
                 }
                 if (f) {
                     if (e || a) {
                         if (e) {
                             j = [], k = r.length;
                             while (k--)(l = r[k]) && j.push(q[k] = l);
                             e(null, r = [], j, i)
                         }
                         k = r.length;
                         while (k--)(l = r[k]) && (j = e ? J(f, l) : m[k]) > -1 && (f[j] = !(g[j] = l))
                     }
-                } else r = va(r === g ? r.splice(o, r.length) : r), e ? e(null, g, r, i) : H.apply(g, r)
+                } else r = ua(r === g ? r.splice(o, r.length) : r), e ? e(null, g, r, i) : H.apply(g, r)
             })
         }
 
-        function xa(a) {
-            for (var b, c, e, f = a.length, g = d.relative[a[0].type], h = g || d.relative[" "], i = g ? 1 : 0, k = sa(function(a) {
+        function wa(a) {
+            for (var b, c, e, f = a.length, g = d.relative[a[0].type], h = g || d.relative[" "], i = g ? 1 : 0, k = ra(function(a) {
                     return a === b
-                }, h, !0), l = sa(function(a) {
+                }, h, !0), l = ra(function(a) {
                     return J(b, a) > -1
                 }, h, !0), m = [function(a, c, d) {
                     var e = !g && (d || c !== j) || ((b = c).nodeType ? k(a, c, d) : l(a, c, d));
                     return b = null, e
                 }]; f > i; i++)
-                if (c = d.relative[a[i].type]) m = [sa(ta(m), c)];
+                if (c = d.relative[a[i].type]) m = [ra(sa(m), c)];
                 else {
                     if (c = d.filter[a[i].type].apply(null, a[i].matches), c[u]) {
                         for (e = ++i; f > e; e++)
                             if (d.relative[a[e].type]) break;
-                        return wa(i > 1 && ta(m), i > 1 && ra(a.slice(0, i - 1).concat({
+                        return va(i > 1 && sa(m), i > 1 && qa(a.slice(0, i - 1).concat({
                             value: " " === a[i - 2].type ? "*" : ""
-                        })).replace(R, "$1"), c, e > i && xa(a.slice(i, e)), f > e && xa(a = a.slice(e)), f > e && ra(a))
+                        })).replace(Q, "$1"), c, e > i && wa(a.slice(i, e)), f > e && wa(a = a.slice(e)), f > e && qa(a))
                     }
                     m.push(c)
-                } return ta(m)
+                } return sa(m)
         }
 
-        function ya(a, b) {
+        function xa(a, b) {
             var c = b.length > 0,
                 e = a.length > 0,
                 f = function(f, g, h, i, k) {
-                    var l, m, o, p = 0,
-                        q = "0",
-                        r = f && [],
-                        s = [],
-                        t = j,
-                        u = f || e && d.find.TAG("*", k),
-                        v = w += null == t ? 1 : Math.random() || .1,
-                        x = u.length;
-                    for (k && (j = g !== n && g); q !== x && null != (l = u[q]); q++) {
+                    var l, o, q, r = 0,
+                        s = "0",
+                        t = f && [],
+                        u = [],
+                        v = j,
+                        x = f || e && d.find.TAG("*", k),
+                        y = w += null == v ? 1 : Math.random() || .1,
+                        z = x.length;
+                    for (k && (j = g === n || g || k); s !== z && null != (l = x[s]); s++) {
                         if (e && l) {
-                            m = 0;
-                            while (o = a[m++])
-                                if (o(l, g, h)) {
+                            o = 0, g || l.ownerDocument === n || (m(l), h = !p);
+                            while (q = a[o++])
+                                if (q(l, g || n, h)) {
                                     i.push(l);
                                     break
-                                } k && (w = v)
+                                } k && (w = y)
                         }
-                        c && ((l = !o && l) && p--, f && r.push(l))
+                        c && ((l = !q && l) && r--, f && t.push(l))
                     }
-                    if (p += q, c && q !== p) {
-                        m = 0;
-                        while (o = b[m++]) o(r, s, g, h);
+                    if (r += s, c && s !== r) {
+                        o = 0;
+                        while (q = b[o++]) q(t, u, g, h);
                         if (f) {
-                            if (p > 0)
-                                while (q--) r[q] || s[q] || (s[q] = F.call(i));
-                            s = va(s)
+                            if (r > 0)
+                                while (s--) t[s] || u[s] || (u[s] = F.call(i));
+                            u = ua(u)
                         }
-                        H.apply(i, s), k && !f && s.length > 0 && p + b.length > 1 && ga.uniqueSort(i)
+                        H.apply(i, u), k && !f && u.length > 0 && r + b.length > 1 && fa.uniqueSort(i)
                     }
-                    return k && (w = v, j = t), r
+                    return k && (w = y, j = v), t
                 };
-            return c ? ia(f) : f
+            return c ? ha(f) : f
         }
-        return h = ga.compile = function(a, b) {
+        return h = fa.compile = function(a, b) {
             var c, d = [],
                 e = [],
                 f = A[a + " "];
             if (!f) {
                 b || (b = g(a)), c = b.length;
-                while (c--) f = xa(b[c]), f[u] ? d.push(f) : e.push(f);
-                f = A(a, ya(e, d)), f.selector = a
+                while (c--) f = wa(b[c]), f[u] ? d.push(f) : e.push(f);
+                f = A(a, xa(e, d)), f.selector = a
             }
             return f
-        }, i = ga.select = function(a, b, e, f) {
+        }, i = fa.select = function(a, b, e, f) {
             var i, j, k, l, m, n = "function" == typeof a && a,
                 o = !f && g(a = n.selector || a);
             if (e = e || [], 1 === o.length) {
                 if (j = o[0] = o[0].slice(0), j.length > 2 && "ID" === (k = j[0]).type && c.getById && 9 === b.nodeType && p && d.relative[j[1].type]) {
-                    if (b = (d.find.ID(k.matches[0].replace(ca, da), b) || [])[0], !b) return e;
+                    if (b = (d.find.ID(k.matches[0].replace(ba, ca), b) || [])[0], !b) return e;
                     n && (b = b.parentNode), a = a.slice(j.shift().value.length)
                 }
-                i = X.needsContext.test(a) ? 0 : j.length;
+                i = W.needsContext.test(a) ? 0 : j.length;
                 while (i--) {
                     if (k = j[i], d.relative[l = k.type]) break;
-                    if ((m = d.find[l]) && (f = m(k.matches[0].replace(ca, da), aa.test(j[0].type) && pa(b.parentNode) || b))) {
-                        if (j.splice(i, 1), a = f.length && ra(j), !a) return H.apply(e, f), e;
+                    if ((m = d.find[l]) && (f = m(k.matches[0].replace(ba, ca), _.test(j[0].type) && oa(b.parentNode) || b))) {
+                        if (j.splice(i, 1), a = f.length && qa(j), !a) return H.apply(e, f), e;
                         break
                     }
                 }
             }
-            return (n || h(a, o))(f, b, !p, e, aa.test(a) && pa(b.parentNode) || b), e
-        }, c.sortStable = u.split("").sort(B).join("") === u, c.detectDuplicates = !!l, m(), c.sortDetached = ja(function(a) {
+            return (n || h(a, o))(f, b, !p, e, !b || _.test(a) && oa(b.parentNode) || b), e
+        }, c.sortStable = u.split("").sort(B).join("") === u, c.detectDuplicates = !!l, m(), c.sortDetached = ia(function(a) {
             return 1 & a.compareDocumentPosition(n.createElement("div"))
-        }), ja(function(a) {
+        }), ia(function(a) {
             return a.innerHTML = "<a href='#'></a>", "#" === a.firstChild.getAttribute("href")
-        }) || ka("type|href|height|width", function(a, b, c) {
+        }) || ja("type|href|height|width", function(a, b, c) {
             return c ? void 0 : a.getAttribute(b, "type" === b.toLowerCase() ? 1 : 2)
-        }), c.attributes && ja(function(a) {
+        }), c.attributes && ia(function(a) {
             return a.innerHTML = "<input/>", a.firstChild.setAttribute("value", ""), "" === a.firstChild.getAttribute("value")
-        }) || ka("value", function(a, b, c) {
+        }) || ja("value", function(a, b, c) {
             return c || "input" !== a.nodeName.toLowerCase() ? void 0 : a.defaultValue
-        }), ja(function(a) {
+        }), ia(function(a) {
             return null == a.getAttribute("disabled")
-        }) || ka(K, function(a, b, c) {
+        }) || ja(K, function(a, b, c) {
             var d;
             return c ? void 0 : a[b] === !0 ? b.toLowerCase() : (d = a.getAttributeNode(b)) && d.specified ? d.value : null
-        }), ga
+        }), fa
     }(a);
-    m.find = s, m.expr = s.selectors, m.expr[":"] = m.expr.pseudos, m.unique = s.uniqueSort, m.text = s.getText, m.isXMLDoc = s.isXML, m.contains = s.contains;
-    var t = m.expr.match.needsContext,
-        u = /^<(\w+)\s*\/?>(?:<\/\1>|)$/,
-        v = /^.[^:#\[\.,]*$/;
+    n.find = t, n.expr = t.selectors, n.expr[":"] = n.expr.pseudos, n.uniqueSort = n.unique = t.uniqueSort, n.text = t.getText, n.isXMLDoc = t.isXML, n.contains = t.contains;
+    var u = function(a, b, c) {
+            var d = [],
+                e = void 0 !== c;
+            while ((a = a[b]) && 9 !== a.nodeType)
+                if (1 === a.nodeType) {
+                    if (e && n(a).is(c)) break;
+                    d.push(a)
+                } return d
+        },
+        v = function(a, b) {
+            for (var c = []; a; a = a.nextSibling) 1 === a.nodeType && a !== b && c.push(a);
+            return c
+        },
+        w = n.expr.match.needsContext,
+        x = /^<([\w-]+)\s*\/?>(?:<\/\1>|)$/,
+        y = /^.[^:#\[\.,]*$/;
 
-    function w(a, b, c) {
-        if (m.isFunction(b)) return m.grep(a, function(a, d) {
+    function z(a, b, c) {
+        if (n.isFunction(b)) return n.grep(a, function(a, d) {
             return !!b.call(a, d, a) !== c
         });
-        if (b.nodeType) return m.grep(a, function(a) {
+        if (b.nodeType) return n.grep(a, function(a) {
             return a === b !== c
         });
         if ("string" == typeof b) {
-            if (v.test(b)) return m.filter(b, a, c);
-            b = m.filter(b, a)
+            if (y.test(b)) return n.filter(b, a, c);
+            b = n.filter(b, a)
         }
-        return m.grep(a, function(a) {
-            return m.inArray(a, b) >= 0 !== c
+        return n.grep(a, function(a) {
+            return n.inArray(a, b) > -1 !== c
         })
     }
-    m.filter = function(a, b, c) {
+    n.filter = function(a, b, c) {
         var d = b[0];
-        return c && (a = ":not(" + a + ")"), 1 === b.length && 1 === d.nodeType ? m.find.matchesSelector(d, a) ? [d] : [] : m.find.matches(a, m.grep(b, function(a) {
+        return c && (a = ":not(" + a + ")"), 1 === b.length && 1 === d.nodeType ? n.find.matchesSelector(d, a) ? [d] : [] : n.find.matches(a, n.grep(b, function(a) {
             return 1 === a.nodeType
         }))
-    }, m.fn.extend({
+    }, n.fn.extend({
         find: function(a) {
             var b, c = [],
                 d = this,
                 e = d.length;
-            if ("string" != typeof a) return this.pushStack(m(a).filter(function() {
+            if ("string" != typeof a) return this.pushStack(n(a).filter(function() {
                 for (b = 0; e > b; b++)
-                    if (m.contains(d[b], this)) return !0
+                    if (n.contains(d[b], this)) return !0
             }));
-            for (b = 0; e > b; b++) m.find(a, d[b], c);
-            return c = this.pushStack(e > 1 ? m.unique(c) : c), c.selector = this.selector ? this.selector + " " + a : a, c
+            for (b = 0; e > b; b++) n.find(a, d[b], c);
+            return c = this.pushStack(e > 1 ? n.unique(c) : c), c.selector = this.selector ? this.selector + " " + a : a, c
         },
         filter: function(a) {
-            return this.pushStack(w(this, a || [], !1))
+            return this.pushStack(z(this, a || [], !1))
         },
         not: function(a) {
-            return this.pushStack(w(this, a || [], !0))
+            return this.pushStack(z(this, a || [], !0))
         },
         is: function(a) {
-            return !!w(this, "string" == typeof a && t.test(a) ? m(a) : a || [], !1).length
+            return !!z(this, "string" == typeof a && w.test(a) ? n(a) : a || [], !1).length
         }
     });
-    var x, y = a.document,
-        z = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]*))$/,
-        A = m.fn.init = function(a, b) {
-            var c, d;
+    var A, B = /^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]*))$/,
+        C = n.fn.init = function(a, b, c) {
+            var e, f;
             if (!a) return this;
-            if ("string" == typeof a) {
-                if (c = "<" === a.charAt(0) && ">" === a.charAt(a.length - 1) && a.length >= 3 ? [null, a, null] : z.exec(a), !c || !c[1] && b) return !b || b.jquery ? (b || x).find(a) : this.constructor(b).find(a);
-                if (c[1]) {
-                    if (b = b instanceof m ? b[0] : b, m.merge(this, m.parseHTML(c[1], b && b.nodeType ? b.ownerDocument || b : y, !0)), u.test(c[1]) && m.isPlainObject(b))
-                        for (c in b) m.isFunction(this[c]) ? this[c](b[c]) : this.attr(c, b[c]);
+            if (c = c || A, "string" == typeof a) {
+                if (e = "<" === a.charAt(0) && ">" === a.charAt(a.length - 1) && a.length >= 3 ? [null, a, null] : B.exec(a), !e || !e[1] && b) return !b || b.jquery ? (b || c).find(a) : this.constructor(b).find(a);
+                if (e[1]) {
+                    if (b = b instanceof n ? b[0] : b, n.merge(this, n.parseHTML(e[1], b && b.nodeType ? b.ownerDocument || b : d, !0)), x.test(e[1]) && n.isPlainObject(b))
+                        for (e in b) n.isFunction(this[e]) ? this[e](b[e]) : this.attr(e, b[e]);
                     return this
                 }
-                if (d = y.getElementById(c[2]), d && d.parentNode) {
-                    if (d.id !== c[2]) return x.find(a);
-                    this.length = 1, this[0] = d
+                if (f = d.getElementById(e[2]), f && f.parentNode) {
+                    if (f.id !== e[2]) return A.find(a);
+                    this.length = 1, this[0] = f
                 }
-                return this.context = y, this.selector = a, this
+                return this.context = d, this.selector = a, this
             }
-            return a.nodeType ? (this.context = this[0] = a, this.length = 1, this) : m.isFunction(a) ? "undefined" != typeof x.ready ? x.ready(a) : a(m) : (void 0 !== a.selector && (this.selector = a.selector, this.context = a.context), m.makeArray(a, this))
+            return a.nodeType ? (this.context = this[0] = a, this.length = 1, this) : n.isFunction(a) ? "undefined" != typeof c.ready ? c.ready(a) : a(n) : (void 0 !== a.selector && (this.selector = a.selector, this.context = a.context), n.makeArray(a, this))
         };
-    A.prototype = m.fn, x = m(y);
-    var B = /^(?:parents|prev(?:Until|All))/,
-        C = {
+    C.prototype = n.fn, A = n(d);
+    var D = /^(?:parents|prev(?:Until|All))/,
+        E = {
             children: !0,
             contents: !0,
             next: !0,
             prev: !0
         };
-    m.extend({
-        dir: function(a, b, c) {
-            var d = [],
-                e = a[b];
-            while (e && 9 !== e.nodeType && (void 0 === c || 1 !== e.nodeType || !m(e).is(c))) 1 === e.nodeType && d.push(e), e = e[b];
-            return d
-        },
-        sibling: function(a, b) {
-            for (var c = []; a; a = a.nextSibling) 1 === a.nodeType && a !== b && c.push(a);
-            return c
-        }
-    }), m.fn.extend({
+    n.fn.extend({
         has: function(a) {
-            var b, c = m(a, this),
+            var b, c = n(a, this),
                 d = c.length;
             return this.filter(function() {
                 for (b = 0; d > b; b++)
-                    if (m.contains(this, c[b])) return !0
+                    if (n.contains(this, c[b])) return !0
             })
         },
         closest: function(a, b) {
-            for (var c, d = 0, e = this.length, f = [], g = t.test(a) || "string" != typeof a ? m(a, b || this.context) : 0; e > d; d++)
+            for (var c, d = 0, e = this.length, f = [], g = w.test(a) || "string" != typeof a ? n(a, b || this.context) : 0; e > d; d++)
                 for (c = this[d]; c && c !== b; c = c.parentNode)
-                    if (c.nodeType < 11 && (g ? g.index(c) > -1 : 1 === c.nodeType && m.find.matchesSelector(c, a))) {
+                    if (c.nodeType < 11 && (g ? g.index(c) > -1 : 1 === c.nodeType && n.find.matchesSelector(c, a))) {
                         f.push(c);
                         break
-                    } return this.pushStack(f.length > 1 ? m.unique(f) : f)
+                    } return this.pushStack(f.length > 1 ? n.uniqueSort(f) : f)
         },
         index: function(a) {
-            return a ? "string" == typeof a ? m.inArray(this[0], m(a)) : m.inArray(a.jquery ? a[0] : a, this) : this[0] && this[0].parentNode ? this.first().prevAll().length : -1
+            return a ? "string" == typeof a ? n.inArray(this[0], n(a)) : n.inArray(a.jquery ? a[0] : a, this) : this[0] && this[0].parentNode ? this.first().prevAll().length : -1
         },
         add: function(a, b) {
-            return this.pushStack(m.unique(m.merge(this.get(), m(a, b))))
+            return this.pushStack(n.uniqueSort(n.merge(this.get(), n(a, b))))
         },
         addBack: function(a) {
             return this.add(null == a ? this.prevObject : this.prevObject.filter(a))
         }
     });
 
-    function D(a, b) {
+    function F(a, b) {
         do a = a[b]; while (a && 1 !== a.nodeType);
         return a
     }
-    m.each({
+    n.each({
         parent: function(a) {
             var b = a.parentNode;
             return b && 11 !== b.nodeType ? b : null
         },
         parents: function(a) {
-            return m.dir(a, "parentNode")
+            return u(a, "parentNode")
         },
         parentsUntil: function(a, b, c) {
-            return m.dir(a, "parentNode", c)
+            return u(a, "parentNode", c)
         },
         next: function(a) {
-            return D(a, "nextSibling")
+            return F(a, "nextSibling")
         },
         prev: function(a) {
-            return D(a, "previousSibling")
+            return F(a, "previousSibling")
         },
         nextAll: function(a) {
-            return m.dir(a, "nextSibling")
+            return u(a, "nextSibling")
         },
         prevAll: function(a) {
-            return m.dir(a, "previousSibling")
+            return u(a, "previousSibling")
         },
         nextUntil: function(a, b, c) {
-            return m.dir(a, "nextSibling", c)
+            return u(a, "nextSibling", c)
         },
         prevUntil: function(a, b, c) {
-            return m.dir(a, "previousSibling", c)
+            return u(a, "previousSibling", c)
         },
         siblings: function(a) {
-            return m.sibling((a.parentNode || {}).firstChild, a)
+            return v((a.parentNode || {}).firstChild, a)
         },
         children: function(a) {
-            return m.sibling(a.firstChild)
+            return v(a.firstChild)
         },
         contents: function(a) {
-            return m.nodeName(a, "iframe") ? a.contentDocument || a.contentWindow.document : m.merge([], a.childNodes)
+            return n.nodeName(a, "iframe") ? a.contentDocument || a.contentWindow.document : n.merge([], a.childNodes)
         }
     }, function(a, b) {
-        m.fn[a] = function(c, d) {
-            var e = m.map(this, b, c);
-            return "Until" !== a.slice(-5) && (d = c), d && "string" == typeof d && (e = m.filter(d, e)), this.length > 1 && (C[a] || (e = m.unique(e)), B.test(a) && (e = e.reverse())), this.pushStack(e)
+        n.fn[a] = function(c, d) {
+            var e = n.map(this, b, c);
+            return "Until" !== a.slice(-5) && (d = c), d && "string" == typeof d && (e = n.filter(d, e)), this.length > 1 && (E[a] || (e = n.uniqueSort(e)), D.test(a) && (e = e.reverse())), this.pushStack(e)
         }
     });
-    var E = /\S+/g,
-        F = {};
+    var G = /\S+/g;
 
-    function G(a) {
-        var b = F[a] = {};
-        return m.each(a.match(E) || [], function(a, c) {
+    function H(a) {
+        var b = {};
+        return n.each(a.match(G) || [], function(a, c) {
             b[c] = !0
         }), b
     }
-    m.Callbacks = function(a) {
-        a = "string" == typeof a ? F[a] || G(a) : m.extend({}, a);
-        var b, c, d, e, f, g, h = [],
-            i = !a.once && [],
-            j = function(l) {
-                for (c = a.memory && l, d = !0, f = g || 0, g = 0, e = h.length, b = !0; h && e > f; f++)
-                    if (h[f].apply(l[0], l[1]) === !1 && a.stopOnFalse) {
-                        c = !1;
-                        break
-                    } b = !1, h && (i ? i.length && j(i.shift()) : c ? h = [] : k.disable())
+    n.Callbacks = function(a) {
+        a = "string" == typeof a ? H(a) : n.extend({}, a);
+        var b, c, d, e, f = [],
+            g = [],
+            h = -1,
+            i = function() {
+                for (e = a.once, d = b = !0; g.length; h = -1) {
+                    c = g.shift();
+                    while (++h < f.length) f[h].apply(c[0], c[1]) === !1 && a.stopOnFalse && (h = f.length, c = !1)
+                }
+                a.memory || (c = !1), b = !1, e && (f = c ? [] : "")
             },
-            k = {
+            j = {
                 add: function() {
-                    if (h) {
-                        var d = h.length;
-                        ! function f(b) {
-                            m.each(b, function(b, c) {
-                                var d = m.type(c);
-                                "function" === d ? a.unique && k.has(c) || h.push(c) : c && c.length && "string" !== d && f(c)
-                            })
-                        }(arguments), b ? e = h.length : c && (g = d, j(c))
-                    }
-                    return this
+                    return f && (c && !b && (h = f.length - 1, g.push(c)), function d(b) {
+                        n.each(b, function(b, c) {
+                            n.isFunction(c) ? a.unique && j.has(c) || f.push(c) : c && c.length && "string" !== n.type(c) && d(c)
+                        })
+                    }(arguments), c && !b && i()), this
                 },
                 remove: function() {
-                    return h && m.each(arguments, function(a, c) {
-                        var d;
-                        while ((d = m.inArray(c, h, d)) > -1) h.splice(d, 1), b && (e >= d && e--, f >= d && f--)
+                    return n.each(arguments, function(a, b) {
+                        var c;
+                        while ((c = n.inArray(b, f, c)) > -1) f.splice(c, 1), h >= c && h--
                     }), this
                 },
                 has: function(a) {
-                    return a ? m.inArray(a, h) > -1 : !(!h || !h.length)
+                    return a ? n.inArray(a, f) > -1 : f.length > 0
                 },
                 empty: function() {
-                    return h = [], e = 0, this
+                    return f && (f = []), this
                 },
                 disable: function() {
-                    return h = i = c = void 0, this
+                    return e = g = [], f = c = "", this
                 },
                 disabled: function() {
-                    return !h
+                    return !f
                 },
                 lock: function() {
-                    return i = void 0, c || k.disable(), this
+                    return e = !0, c || j.disable(), this
                 },
                 locked: function() {
-                    return !i
+                    return !!e
                 },
                 fireWith: function(a, c) {
-                    return !h || d && !i || (c = c || [], c = [a, c.slice ? c.slice() : c], b ? i.push(c) : j(c)), this
+                    return e || (c = c || [], c = [a, c.slice ? c.slice() : c], g.push(c), b || i()), this
                 },
                 fire: function() {
-                    return k.fireWith(this, arguments), this
+                    return j.fireWith(this, arguments), this
                 },
                 fired: function() {
                     return !!d
                 }
             };
-        return k
-    }, m.extend({
+        return j
+    }, n.extend({
         Deferred: function(a) {
             var b = [
-                    ["resolve", "done", m.Callbacks("once memory"), "resolved"],
-                    ["reject", "fail", m.Callbacks("once memory"), "rejected"],
-                    ["notify", "progress", m.Callbacks("memory")]
+                    ["resolve", "done", n.Callbacks("once memory"), "resolved"],
+                    ["reject", "fail", n.Callbacks("once memory"), "rejected"],
+                    ["notify", "progress", n.Callbacks("memory")]
                 ],
                 c = "pending",
                 d = {
                     state: function() {
                         return c
                     },
                     always: function() {
                         return e.done(arguments).fail(arguments), this
                     },
                     then: function() {
                         var a = arguments;
-                        return m.Deferred(function(c) {
-                            m.each(b, function(b, f) {
-                                var g = m.isFunction(a[b]) && a[b];
+                        return n.Deferred(function(c) {
+                            n.each(b, function(b, f) {
+                                var g = n.isFunction(a[b]) && a[b];
                                 e[f[1]](function() {
                                     var a = g && g.apply(this, arguments);
-                                    a && m.isFunction(a.promise) ? a.promise().done(c.resolve).fail(c.reject).progress(c.notify) : c[f[0] + "With"](this === d ? c.promise() : this, g ? [a] : arguments)
+                                    a && n.isFunction(a.promise) ? a.promise().progress(c.notify).done(c.resolve).fail(c.reject) : c[f[0] + "With"](this === d ? c.promise() : this, g ? [a] : arguments)
                                 })
                             }), a = null
                         }).promise()
                     },
                     promise: function(a) {
-                        return null != a ? m.extend(a, d) : d
+                        return null != a ? n.extend(a, d) : d
                     }
                 },
                 e = {};
-            return d.pipe = d.then, m.each(b, function(a, f) {
+            return d.pipe = d.then, n.each(b, function(a, f) {
                 var g = f[2],
                     h = f[3];
                 d[f[1]] = g.add, h && g.add(function() {
                     c = h
                 }, b[1 ^ a][2].disable, b[2][2].lock), e[f[0]] = function() {
                     return e[f[0] + "With"](this === e ? d : this, arguments), this
                 }, e[f[0] + "With"] = g.fireWith
             }), d.promise(e), a && a.call(e, e), e
         },
         when: function(a) {
             var b = 0,
-                c = d.call(arguments),
-                e = c.length,
-                f = 1 !== e || a && m.isFunction(a.promise) ? e : 0,
-                g = 1 === f ? a : m.Deferred(),
+                c = e.call(arguments),
+                d = c.length,
+                f = 1 !== d || a && n.isFunction(a.promise) ? d : 0,
+                g = 1 === f ? a : n.Deferred(),
                 h = function(a, b, c) {
-                    return function(e) {
-                        b[a] = this, c[a] = arguments.length > 1 ? d.call(arguments) : e, c === i ? g.notifyWith(b, c) : --f || g.resolveWith(b, c)
+                    return function(d) {
+                        b[a] = this, c[a] = arguments.length > 1 ? e.call(arguments) : d, c === i ? g.notifyWith(b, c) : --f || g.resolveWith(b, c)
                     }
                 },
                 i, j, k;
-            if (e > 1)
-                for (i = new Array(e), j = new Array(e), k = new Array(e); e > b; b++) c[b] && m.isFunction(c[b].promise) ? c[b].promise().done(h(b, k, c)).fail(g.reject).progress(h(b, j, i)) : --f;
+            if (d > 1)
+                for (i = new Array(d), j = new Array(d), k = new Array(d); d > b; b++) c[b] && n.isFunction(c[b].promise) ? c[b].promise().progress(h(b, j, i)).done(h(b, k, c)).fail(g.reject) : --f;
             return f || g.resolveWith(k, c), g.promise()
         }
     });
-    var H;
-    m.fn.ready = function(a) {
-        return m.ready.promise().done(a), this
-    }, m.extend({
+    var I;
+    n.fn.ready = function(a) {
+        return n.ready.promise().done(a), this
+    }, n.extend({
         isReady: !1,
         readyWait: 1,
         holdReady: function(a) {
-            a ? m.readyWait++ : m.ready(!0)
+            a ? n.readyWait++ : n.ready(!0)
         },
         ready: function(a) {
-            if (a === !0 ? !--m.readyWait : !m.isReady) {
-                if (!y.body) return setTimeout(m.ready);
-                m.isReady = !0, a !== !0 && --m.readyWait > 0 || (H.resolveWith(y, [m]), m.fn.triggerHandler && (m(y).triggerHandler("ready"), m(y).off("ready")))
-            }
+            (a === !0 ? --n.readyWait : n.isReady) || (n.isReady = !0, a !== !0 && --n.readyWait > 0 || (I.resolveWith(d, [n]), n.fn.triggerHandler && (n(d).triggerHandler("ready"), n(d).off("ready"))))
         }
     });
 
-    function I() {
-        y.addEventListener ? (y.removeEventListener("DOMContentLoaded", J, !1), a.removeEventListener("load", J, !1)) : (y.detachEvent("onreadystatechange", J), a.detachEvent("onload", J))
+    function J() {
+        d.addEventListener ? (d.removeEventListener("DOMContentLoaded", K), a.removeEventListener("load", K)) : (d.detachEvent("onreadystatechange", K), a.detachEvent("onload", K))
     }
 
-    function J() {
-        (y.addEventListener || "load" === event.type || "complete" === y.readyState) && (I(), m.ready())
+    function K() {
+        (d.addEventListener || "load" === a.event.type || "complete" === d.readyState) && (J(), n.ready())
     }
-    m.ready.promise = function(b) {
-        if (!H)
-            if (H = m.Deferred(), "complete" === y.readyState) setTimeout(m.ready);
-            else if (y.addEventListener) y.addEventListener("DOMContentLoaded", J, !1), a.addEventListener("load", J, !1);
+    n.ready.promise = function(b) {
+        if (!I)
+            if (I = n.Deferred(), "complete" === d.readyState || "loading" !== d.readyState && !d.documentElement.doScroll) a.setTimeout(n.ready);
+            else if (d.addEventListener) d.addEventListener("DOMContentLoaded", K), a.addEventListener("load", K);
         else {
-            y.attachEvent("onreadystatechange", J), a.attachEvent("onload", J);
+            d.attachEvent("onreadystatechange", K), a.attachEvent("onload", K);
             var c = !1;
             try {
-                c = null == a.frameElement && y.documentElement
-            } catch (d) {}
-            c && c.doScroll && ! function e() {
-                if (!m.isReady) {
+                c = null == a.frameElement && d.documentElement
+            } catch (e) {}
+            c && c.doScroll && ! function f() {
+                if (!n.isReady) {
                     try {
                         c.doScroll("left")
-                    } catch (a) {
-                        return setTimeout(e, 50)
+                    } catch (b) {
+                        return a.setTimeout(f, 50)
                     }
-                    I(), m.ready()
+                    J(), n.ready()
                 }
             }()
         }
-        return H.promise(b)
-    };
-    var K = "undefined",
-        L;
-    for (L in m(k)) break;
-    k.ownLast = "0" !== L, k.inlineBlockNeedsLayout = !1, m(function() {
-            var a, b, c, d;
-            c = y.getElementsByTagName("body")[0], c && c.style && (b = y.createElement("div"), d = y.createElement("div"), d.style.cssText = "position:absolute;border:0;width:0;height:0;top:0;left:-9999px", c.appendChild(d).appendChild(b), typeof b.style.zoom !== K && (b.style.cssText = "display:inline;margin:0;border:0;padding:1px;width:1px;zoom:1", k.inlineBlockNeedsLayout = a = 3 === b.offsetWidth, a && (c.style.zoom = 1)), c.removeChild(d))
+        return I.promise(b)
+    }, n.ready.promise();
+    var L;
+    for (L in n(l)) break;
+    l.ownFirst = "0" === L, l.inlineBlockNeedsLayout = !1, n(function() {
+            var a, b, c, e;
+            c = d.getElementsByTagName("body")[0], c && c.style && (b = d.createElement("div"), e = d.createElement("div"), e.style.cssText = "position:absolute;border:0;width:0;height:0;top:0;left:-9999px", c.appendChild(e).appendChild(b), "undefined" != typeof b.style.zoom && (b.style.cssText = "display:inline;margin:0;border:0;padding:1px;width:1px;zoom:1", l.inlineBlockNeedsLayout = a = 3 === b.offsetWidth, a && (c.style.zoom = 1)), c.removeChild(e))
         }),
         function() {
-            var a = y.createElement("div");
-            if (null == k.deleteExpando) {
-                k.deleteExpando = !0;
-                try {
-                    delete a.test
-                } catch (b) {
-                    k.deleteExpando = !1
-                }
+            var a = d.createElement("div");
+            l.deleteExpando = !0;
+            try {
+                delete a.test
+            } catch (b) {
+                l.deleteExpando = !1
             }
             a = null
-        }(), m.acceptData = function(a) {
-            var b = m.noData[(a.nodeName + " ").toLowerCase()],
+        }();
+    var M = function(a) {
+            var b = n.noData[(a.nodeName + " ").toLowerCase()],
                 c = +a.nodeType || 1;
             return 1 !== c && 9 !== c ? !1 : !b || b !== !0 && a.getAttribute("classid") === b
-        };
-    var M = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
-        N = /([A-Z])/g;
+        },
+        N = /^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,
+        O = /([A-Z])/g;
 
-    function O(a, b, c) {
+    function P(a, b, c) {
         if (void 0 === c && 1 === a.nodeType) {
-            var d = "data-" + b.replace(N, "-$1").toLowerCase();
+            var d = "data-" + b.replace(O, "-$1").toLowerCase();
             if (c = a.getAttribute(d), "string" == typeof c) {
                 try {
-                    c = "true" === c ? !0 : "false" === c ? !1 : "null" === c ? null : +c + "" === c ? +c : M.test(c) ? m.parseJSON(c) : c
+                    c = "true" === c ? !0 : "false" === c ? !1 : "null" === c ? null : +c + "" === c ? +c : N.test(c) ? n.parseJSON(c) : c
                 } catch (e) {}
-                m.data(a, b, c)
-            } else c = void 0
+                n.data(a, b, c)
+            } else c = void 0;
         }
         return c
     }
 
-    function P(a) {
+    function Q(a) {
         var b;
         for (b in a)
-            if (("data" !== b || !m.isEmptyObject(a[b])) && "toJSON" !== b) return !1;
-
+            if (("data" !== b || !n.isEmptyObject(a[b])) && "toJSON" !== b) return !1;
         return !0
     }
 
-    function Q(a, b, d, e) {
-        if (m.acceptData(a)) {
-            var f, g, h = m.expando,
+    function R(a, b, d, e) {
+        if (M(a)) {
+            var f, g, h = n.expando,
                 i = a.nodeType,
-                j = i ? m.cache : a,
+                j = i ? n.cache : a,
                 k = i ? a[h] : a[h] && h;
-            if (k && j[k] && (e || j[k].data) || void 0 !== d || "string" != typeof b) return k || (k = i ? a[h] = c.pop() || m.guid++ : h), j[k] || (j[k] = i ? {} : {
-                toJSON: m.noop
-            }), ("object" == typeof b || "function" == typeof b) && (e ? j[k] = m.extend(j[k], b) : j[k].data = m.extend(j[k].data, b)), g = j[k], e || (g.data || (g.data = {}), g = g.data), void 0 !== d && (g[m.camelCase(b)] = d), "string" == typeof b ? (f = g[b], null == f && (f = g[m.camelCase(b)])) : f = g, f
+            if (k && j[k] && (e || j[k].data) || void 0 !== d || "string" != typeof b) return k || (k = i ? a[h] = c.pop() || n.guid++ : h), j[k] || (j[k] = i ? {} : {
+                toJSON: n.noop
+            }), "object" != typeof b && "function" != typeof b || (e ? j[k] = n.extend(j[k], b) : j[k].data = n.extend(j[k].data, b)), g = j[k], e || (g.data || (g.data = {}), g = g.data), void 0 !== d && (g[n.camelCase(b)] = d), "string" == typeof b ? (f = g[b], null == f && (f = g[n.camelCase(b)])) : f = g, f
         }
     }
 
-    function R(a, b, c) {
-        if (m.acceptData(a)) {
+    function S(a, b, c) {
+        if (M(a)) {
             var d, e, f = a.nodeType,
-                g = f ? m.cache : a,
-                h = f ? a[m.expando] : m.expando;
+                g = f ? n.cache : a,
+                h = f ? a[n.expando] : n.expando;
             if (g[h]) {
                 if (b && (d = c ? g[h] : g[h].data)) {
-                    m.isArray(b) ? b = b.concat(m.map(b, m.camelCase)) : b in d ? b = [b] : (b = m.camelCase(b), b = b in d ? [b] : b.split(" ")), e = b.length;
+                    n.isArray(b) ? b = b.concat(n.map(b, n.camelCase)) : b in d ? b = [b] : (b = n.camelCase(b), b = b in d ? [b] : b.split(" ")), e = b.length;
                     while (e--) delete d[b[e]];
-                    if (c ? !P(d) : !m.isEmptyObject(d)) return
-                }(c || (delete g[h].data, P(g[h]))) && (f ? m.cleanData([a], !0) : k.deleteExpando || g != g.window ? delete g[h] : g[h] = null)
+                    if (c ? !Q(d) : !n.isEmptyObject(d)) return
+                }(c || (delete g[h].data, Q(g[h]))) && (f ? n.cleanData([a], !0) : l.deleteExpando || g != g.window ? delete g[h] : g[h] = void 0)
             }
         }
     }
-    m.extend({
-        cache: {},
-        noData: {
-            "applet ": !0,
-            "embed ": !0,
-            "object ": "clsid:D27CDB6E-AE6D-11cf-96B8-444553540000"
-        },
-        hasData: function(a) {
-            return a = a.nodeType ? m.cache[a[m.expando]] : a[m.expando], !!a && !P(a)
-        },
-        data: function(a, b, c) {
-            return Q(a, b, c)
-        },
-        removeData: function(a, b) {
-            return R(a, b)
-        },
-        _data: function(a, b, c) {
-            return Q(a, b, c, !0)
-        },
-        _removeData: function(a, b) {
-            return R(a, b, !0)
-        }
-    }), m.fn.extend({
-        data: function(a, b) {
-            var c, d, e, f = this[0],
-                g = f && f.attributes;
-            if (void 0 === a) {
-                if (this.length && (e = m.data(f), 1 === f.nodeType && !m._data(f, "parsedAttrs"))) {
-                    c = g.length;
-                    while (c--) g[c] && (d = g[c].name, 0 === d.indexOf("data-") && (d = m.camelCase(d.slice(5)), O(f, d, e[d])));
-                    m._data(f, "parsedAttrs", !0)
-                }
-                return e
+    n.extend({
+            cache: {},
+            noData: {
+                "applet ": !0,
+                "embed ": !0,
+                "object ": "clsid:D27CDB6E-AE6D-11cf-96B8-444553540000"
+            },
+            hasData: function(a) {
+                return a = a.nodeType ? n.cache[a[n.expando]] : a[n.expando], !!a && !Q(a)
+            },
+            data: function(a, b, c) {
+                return R(a, b, c)
+            },
+            removeData: function(a, b) {
+                return S(a, b)
+            },
+            _data: function(a, b, c) {
+                return R(a, b, c, !0)
+            },
+            _removeData: function(a, b) {
+                return S(a, b, !0)
+            }
+        }), n.fn.extend({
+            data: function(a, b) {
+                var c, d, e, f = this[0],
+                    g = f && f.attributes;
+                if (void 0 === a) {
+                    if (this.length && (e = n.data(f), 1 === f.nodeType && !n._data(f, "parsedAttrs"))) {
+                        c = g.length;
+                        while (c--) g[c] && (d = g[c].name, 0 === d.indexOf("data-") && (d = n.camelCase(d.slice(5)), P(f, d, e[d])));
+                        n._data(f, "parsedAttrs", !0)
+                    }
+                    return e
+                }
+                return "object" == typeof a ? this.each(function() {
+                    n.data(this, a)
+                }) : arguments.length > 1 ? this.each(function() {
+                    n.data(this, a, b)
+                }) : f ? P(f, a, n.data(f, a)) : void 0
+            },
+            removeData: function(a) {
+                return this.each(function() {
+                    n.removeData(this, a)
+                })
             }
-            return "object" == typeof a ? this.each(function() {
-                m.data(this, a)
-            }) : arguments.length > 1 ? this.each(function() {
-                m.data(this, a, b)
-            }) : f ? O(f, a, m.data(f, a)) : void 0
-        },
-        removeData: function(a) {
-            return this.each(function() {
-                m.removeData(this, a)
-            })
-        }
-    }), m.extend({
-        queue: function(a, b, c) {
-            var d;
-            return a ? (b = (b || "fx") + "queue", d = m._data(a, b), c && (!d || m.isArray(c) ? d = m._data(a, b, m.makeArray(c)) : d.push(c)), d || []) : void 0
-        },
-        dequeue: function(a, b) {
-            b = b || "fx";
-            var c = m.queue(a, b),
-                d = c.length,
-                e = c.shift(),
-                f = m._queueHooks(a, b),
-                g = function() {
-                    m.dequeue(a, b)
-                };
-            "inprogress" === e && (e = c.shift(), d--), e && ("fx" === b && c.unshift("inprogress"), delete f.stop, e.call(a, g, f)), !d && f && f.empty.fire()
-        },
-        _queueHooks: function(a, b) {
-            var c = b + "queueHooks";
-            return m._data(a, c) || m._data(a, c, {
-                empty: m.Callbacks("once memory").add(function() {
-                    m._removeData(a, b + "queue"), m._removeData(a, c)
+        }), n.extend({
+            queue: function(a, b, c) {
+                var d;
+                return a ? (b = (b || "fx") + "queue", d = n._data(a, b), c && (!d || n.isArray(c) ? d = n._data(a, b, n.makeArray(c)) : d.push(c)), d || []) : void 0
+            },
+            dequeue: function(a, b) {
+                b = b || "fx";
+                var c = n.queue(a, b),
+                    d = c.length,
+                    e = c.shift(),
+                    f = n._queueHooks(a, b),
+                    g = function() {
+                        n.dequeue(a, b)
+                    };
+                "inprogress" === e && (e = c.shift(), d--), e && ("fx" === b && c.unshift("inprogress"), delete f.stop, e.call(a, g, f)), !d && f && f.empty.fire()
+            },
+            _queueHooks: function(a, b) {
+                var c = b + "queueHooks";
+                return n._data(a, c) || n._data(a, c, {
+                    empty: n.Callbacks("once memory").add(function() {
+                        n._removeData(a, b + "queue"), n._removeData(a, c)
+                    })
                 })
-            })
-        }
-    }), m.fn.extend({
-        queue: function(a, b) {
-            var c = 2;
-            return "string" != typeof a && (b = a, a = "fx", c--), arguments.length < c ? m.queue(this[0], a) : void 0 === b ? this : this.each(function() {
-                var c = m.queue(this, a, b);
-                m._queueHooks(this, a), "fx" === a && "inprogress" !== c[0] && m.dequeue(this, a)
-            })
-        },
-        dequeue: function(a) {
-            return this.each(function() {
-                m.dequeue(this, a)
-            })
-        },
-        clearQueue: function(a) {
-            return this.queue(a || "fx", [])
-        },
-        promise: function(a, b) {
-            var c, d = 1,
-                e = m.Deferred(),
-                f = this,
-                g = this.length,
-                h = function() {
-                    --d || e.resolveWith(f, [f])
-                };
-            "string" != typeof a && (b = a, a = void 0), a = a || "fx";
-            while (g--) c = m._data(f[g], a + "queueHooks"), c && c.empty && (d++, c.empty.add(h));
-            return h(), e.promise(b)
+            }
+        }), n.fn.extend({
+            queue: function(a, b) {
+                var c = 2;
+                return "string" != typeof a && (b = a, a = "fx", c--), arguments.length < c ? n.queue(this[0], a) : void 0 === b ? this : this.each(function() {
+                    var c = n.queue(this, a, b);
+                    n._queueHooks(this, a), "fx" === a && "inprogress" !== c[0] && n.dequeue(this, a)
+                })
+            },
+            dequeue: function(a) {
+                return this.each(function() {
+                    n.dequeue(this, a)
+                })
+            },
+            clearQueue: function(a) {
+                return this.queue(a || "fx", [])
+            },
+            promise: function(a, b) {
+                var c, d = 1,
+                    e = n.Deferred(),
+                    f = this,
+                    g = this.length,
+                    h = function() {
+                        --d || e.resolveWith(f, [f])
+                    };
+                "string" != typeof a && (b = a, a = void 0), a = a || "fx";
+                while (g--) c = n._data(f[g], a + "queueHooks"), c && c.empty && (d++, c.empty.add(h));
+                return h(), e.promise(b)
+            }
+        }),
+        function() {
+            var a;
+            l.shrinkWrapBlocks = function() {
+                if (null != a) return a;
+                a = !1;
+                var b, c, e;
+                return c = d.getElementsByTagName("body")[0], c && c.style ? (b = d.createElement("div"), e = d.createElement("div"), e.style.cssText = "position:absolute;border:0;width:0;height:0;top:0;left:-9999px", c.appendChild(e).appendChild(b), "undefined" != typeof b.style.zoom && (b.style.cssText = "-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;display:block;margin:0;border:0;padding:1px;width:1px;zoom:1", b.appendChild(d.createElement("div")).style.width = "5px", a = 3 !== b.offsetWidth), c.removeChild(e), a) : void 0
+            }
+        }();
+    var T = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
+        U = new RegExp("^(?:([+-])=|)(" + T + ")([a-z%]*)$", "i"),
+        V = ["Top", "Right", "Bottom", "Left"],
+        W = function(a, b) {
+            return a = b || a, "none" === n.css(a, "display") || !n.contains(a.ownerDocument, a)
+        };
+
+    function X(a, b, c, d) {
+        var e, f = 1,
+            g = 20,
+            h = d ? function() {
+                return d.cur()
+            } : function() {
+                return n.css(a, b, "")
+            },
+            i = h(),
+            j = c && c[3] || (n.cssNumber[b] ? "" : "px"),
+            k = (n.cssNumber[b] || "px" !== j && +i) && U.exec(n.css(a, b));
+        if (k && k[3] !== j) {
+            j = j || k[3], c = c || [], k = +i || 1;
+            do f = f || ".5", k /= f, n.style(a, b, k + j); while (f !== (f = h() / i) && 1 !== f && --g)
         }
-    });
-    var S = /[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,
-        T = ["Top", "Right", "Bottom", "Left"],
-        U = function(a, b) {
-            return a = b || a, "none" === m.css(a, "display") || !m.contains(a.ownerDocument, a)
-        },
-        V = m.access = function(a, b, c, d, e, f, g) {
+        return c && (k = +k || +i || 0, e = c[1] ? k + (c[1] + 1) * c[2] : +c[2], d && (d.unit = j, d.start = k, d.end = e)), e
+    }
+    var Y = function(a, b, c, d, e, f, g) {
             var h = 0,
                 i = a.length,
                 j = null == c;
-            if ("object" === m.type(c)) {
+            if ("object" === n.type(c)) {
                 e = !0;
-                for (h in c) m.access(a, b, h, c[h], !0, f, g)
-            } else if (void 0 !== d && (e = !0, m.isFunction(d) || (g = !0), j && (g ? (b.call(a, d), b = null) : (j = b, b = function(a, b, c) {
-                    return j.call(m(a), c)
+                for (h in c) Y(a, b, h, c[h], !0, f, g)
+            } else if (void 0 !== d && (e = !0, n.isFunction(d) || (g = !0), j && (g ? (b.call(a, d), b = null) : (j = b, b = function(a, b, c) {
+                    return j.call(n(a), c)
                 })), b))
                 for (; i > h; h++) b(a[h], c, g ? d : d.call(a[h], h, b(a[h], c)));
             return e ? a : j ? b.call(a) : i ? b(a[0], c) : f
         },
-        W = /^(?:checkbox|radio)$/i;
-    ! function() {
-        var a = y.createElement("input"),
-            b = y.createElement("div"),
-            c = y.createDocumentFragment();
-        if (b.innerHTML = "  <link/><table></table><a href='/a'>a</a><input type='checkbox'/>", k.leadingWhitespace = 3 === b.firstChild.nodeType, k.tbody = !b.getElementsByTagName("tbody").length, k.htmlSerialize = !!b.getElementsByTagName("link").length, k.html5Clone = "<:nav></:nav>" !== y.createElement("nav").cloneNode(!0).outerHTML, a.type = "checkbox", a.checked = !0, c.appendChild(a), k.appendChecked = a.checked, b.innerHTML = "<textarea>x</textarea>", k.noCloneChecked = !!b.cloneNode(!0).lastChild.defaultValue, c.appendChild(b), b.innerHTML = "<input type='radio' checked='checked' name='t'/>", k.checkClone = b.cloneNode(!0).cloneNode(!0).lastChild.checked, k.noCloneEvent = !0, b.attachEvent && (b.attachEvent("onclick", function() {
-                k.noCloneEvent = !1
-            }), b.cloneNode(!0).click()), null == k.deleteExpando) {
-            k.deleteExpando = !0;
-            try {
-                delete b.test
-            } catch (d) {
-                k.deleteExpando = !1
-            }
+        Z = /^(?:checkbox|radio)$/i,
+        $ = /<([\w:-]+)/,
+        _ = /^$|\/(?:java|ecma)script/i,
+        aa = /^\s+/,
+        ba = "abbr|article|aside|audio|bdi|canvas|data|datalist|details|dialog|figcaption|figure|footer|header|hgroup|main|mark|meter|nav|output|picture|progress|section|summary|template|time|video";
+
+    function ca(a) {
+        var b = ba.split("|"),
+            c = a.createDocumentFragment();
+        if (c.createElement)
+            while (b.length) c.createElement(b.pop());
+        return c
+    }! function() {
+        var a = d.createElement("div"),
+            b = d.createDocumentFragment(),
+            c = d.createElement("input");
+        a.innerHTML = "  <link/><table></table><a href='/a'>a</a><input type='checkbox'/>", l.leadingWhitespace = 3 === a.firstChild.nodeType, l.tbody = !a.getElementsByTagName("tbody").length, l.htmlSerialize = !!a.getElementsByTagName("link").length, l.html5Clone = "<:nav></:nav>" !== d.createElement("nav").cloneNode(!0).outerHTML, c.type = "checkbox", c.checked = !0, b.appendChild(c), l.appendChecked = c.checked, a.innerHTML = "<textarea>x</textarea>", l.noCloneChecked = !!a.cloneNode(!0).lastChild.defaultValue, b.appendChild(a), c = d.createElement("input"), c.setAttribute("type", "radio"), c.setAttribute("checked", "checked"), c.setAttribute("name", "t"), a.appendChild(c), l.checkClone = a.cloneNode(!0).cloneNode(!0).lastChild.checked, l.noCloneEvent = !!a.addEventListener, a[n.expando] = 1, l.attributes = !a.getAttribute(n.expando)
+    }();
+    var da = {
+        option: [1, "<select multiple='multiple'>", "</select>"],
+        legend: [1, "<fieldset>", "</fieldset>"],
+        area: [1, "<map>", "</map>"],
+        param: [1, "<object>", "</object>"],
+        thead: [1, "<table>", "</table>"],
+        tr: [2, "<table><tbody>", "</tbody></table>"],
+        col: [2, "<table><tbody></tbody><colgroup>", "</colgroup></table>"],
+        td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
+        _default: l.htmlSerialize ? [0, "", ""] : [1, "X<div>", "</div>"]
+    };
+    da.optgroup = da.option, da.tbody = da.tfoot = da.colgroup = da.caption = da.thead, da.th = da.td;
+
+    function ea(a, b) {
+        var c, d, e = 0,
+            f = "undefined" != typeof a.getElementsByTagName ? a.getElementsByTagName(b || "*") : "undefined" != typeof a.querySelectorAll ? a.querySelectorAll(b || "*") : void 0;
+        if (!f)
+            for (f = [], c = a.childNodes || a; null != (d = c[e]); e++) !b || n.nodeName(d, b) ? f.push(d) : n.merge(f, ea(d, b));
+        return void 0 === b || b && n.nodeName(a, b) ? n.merge([a], f) : f
+    }
+
+    function fa(a, b) {
+        for (var c, d = 0; null != (c = a[d]); d++) n._data(c, "globalEval", !b || n._data(b[d], "globalEval"))
+    }
+    var ga = /<|&#?\w+;/,
+        ha = /<tbody/i;
+
+    function ia(a) {
+        Z.test(a.type) && (a.defaultChecked = a.checked)
+    }
+
+    function ja(a, b, c, d, e) {
+        for (var f, g, h, i, j, k, m, o = a.length, p = ca(b), q = [], r = 0; o > r; r++)
+            if (g = a[r], g || 0 === g)
+                if ("object" === n.type(g)) n.merge(q, g.nodeType ? [g] : g);
+                else if (ga.test(g)) {
+            i = i || p.appendChild(b.createElement("div")), j = ($.exec(g) || ["", ""])[1].toLowerCase(), m = da[j] || da._default, i.innerHTML = m[1] + n.htmlPrefilter(g) + m[2], f = m[0];
+            while (f--) i = i.lastChild;
+            if (!l.leadingWhitespace && aa.test(g) && q.push(b.createTextNode(aa.exec(g)[0])), !l.tbody) {
+                g = "table" !== j || ha.test(g) ? "<table>" !== m[1] || ha.test(g) ? 0 : i : i.firstChild, f = g && g.childNodes.length;
+                while (f--) n.nodeName(k = g.childNodes[f], "tbody") && !k.childNodes.length && g.removeChild(k)
+            }
+            n.merge(q, i.childNodes), i.textContent = "";
+            while (i.firstChild) i.removeChild(i.firstChild);
+            i = p.lastChild
+        } else q.push(b.createTextNode(g));
+        i && p.removeChild(i), l.appendChecked || n.grep(ea(q, "input"), ia), r = 0;
+        while (g = q[r++])
+            if (d && n.inArray(g, d) > -1) e && e.push(g);
+            else if (h = n.contains(g.ownerDocument, g), i = ea(p.appendChild(g), "script"), h && fa(i), c) {
+            f = 0;
+            while (g = i[f++]) _.test(g.type || "") && c.push(g)
         }
-    }(),
-    function() {
-        var b, c, d = y.createElement("div");
+        return i = null, p
+    }! function() {
+        var b, c, e = d.createElement("div");
         for (b in {
                 submit: !0,
                 change: !0,
                 focusin: !0
-            }) c = "on" + b, (k[b + "Bubbles"] = c in a) || (d.setAttribute(c, "t"), k[b + "Bubbles"] = d.attributes[c].expando === !1);
-        d = null
+            }) c = "on" + b, (l[b] = c in a) || (e.setAttribute(c, "t"), l[b] = e.attributes[c].expando === !1);
+        e = null
     }();
-    var X = /^(?:input|select|textarea)$/i,
-        Y = /^key/,
-        Z = /^(?:mouse|pointer|contextmenu)|click/,
-        $ = /^(?:focusinfocus|focusoutblur)$/,
-        _ = /^([^.]*)(?:\.(.+)|)$/;
+    var ka = /^(?:input|select|textarea)$/i,
+        la = /^key/,
+        ma = /^(?:mouse|pointer|contextmenu|drag|drop)|click/,
+        na = /^(?:focusinfocus|focusoutblur)$/,
+        oa = /^([^.]*)(?:\.(.+)|)/;
 
-    function aa() {
+    function pa() {
         return !0
     }
 
-    function ba() {
+    function qa() {
         return !1
     }
 
-    function ca() {
+    function ra() {
         try {
-            return y.activeElement
+            return d.activeElement
         } catch (a) {}
     }
-    m.event = {
+
+    function sa(a, b, c, d, e, f) {
+        var g, h;
+        if ("object" == typeof b) {
+            "string" != typeof c && (d = d || c, c = void 0);
+            for (h in b) sa(a, h, c, d, b[h], f);
+            return a
+        }
+        if (null == d && null == e ? (e = c, d = c = void 0) : null == e && ("string" == typeof c ? (e = d, d = void 0) : (e = d, d = c, c = void 0)), e === !1) e = qa;
+        else if (!e) return a;
+        return 1 === f && (g = e, e = function(a) {
+            return n().off(a), g.apply(this, arguments)
+        }, e.guid = g.guid || (g.guid = n.guid++)), a.each(function() {
+            n.event.add(this, b, e, d, c)
+        })
+    }
+    n.event = {
         global: {},
         add: function(a, b, c, d, e) {
-            var f, g, h, i, j, k, l, n, o, p, q, r = m._data(a);
+            var f, g, h, i, j, k, l, m, o, p, q, r = n._data(a);
             if (r) {
-                c.handler && (i = c, c = i.handler, e = i.selector), c.guid || (c.guid = m.guid++), (g = r.events) || (g = r.events = {}), (k = r.handle) || (k = r.handle = function(a) {
-                    return typeof m === K || a && m.event.triggered === a.type ? void 0 : m.event.dispatch.apply(k.elem, arguments)
-                }, k.elem = a), b = (b || "").match(E) || [""], h = b.length;
-                while (h--) f = _.exec(b[h]) || [], o = q = f[1], p = (f[2] || "").split(".").sort(), o && (j = m.event.special[o] || {}, o = (e ? j.delegateType : j.bindType) || o, j = m.event.special[o] || {}, l = m.extend({
+                c.handler && (i = c, c = i.handler, e = i.selector), c.guid || (c.guid = n.guid++), (g = r.events) || (g = r.events = {}), (k = r.handle) || (k = r.handle = function(a) {
+                    return "undefined" == typeof n || a && n.event.triggered === a.type ? void 0 : n.event.dispatch.apply(k.elem, arguments)
+                }, k.elem = a), b = (b || "").match(G) || [""], h = b.length;
+                while (h--) f = oa.exec(b[h]) || [], o = q = f[1], p = (f[2] || "").split(".").sort(), o && (j = n.event.special[o] || {}, o = (e ? j.delegateType : j.bindType) || o, j = n.event.special[o] || {}, l = n.extend({
                     type: o,
                     origType: q,
                     data: d,
                     handler: c,
                     guid: c.guid,
                     selector: e,
-                    needsContext: e && m.expr.match.needsContext.test(e),
+                    needsContext: e && n.expr.match.needsContext.test(e),
                     namespace: p.join(".")
-                }, i), (n = g[o]) || (n = g[o] = [], n.delegateCount = 0, j.setup && j.setup.call(a, d, p, k) !== !1 || (a.addEventListener ? a.addEventListener(o, k, !1) : a.attachEvent && a.attachEvent("on" + o, k))), j.add && (j.add.call(a, l), l.handler.guid || (l.handler.guid = c.guid)), e ? n.splice(n.delegateCount++, 0, l) : n.push(l), m.event.global[o] = !0);
+                }, i), (m = g[o]) || (m = g[o] = [], m.delegateCount = 0, j.setup && j.setup.call(a, d, p, k) !== !1 || (a.addEventListener ? a.addEventListener(o, k, !1) : a.attachEvent && a.attachEvent("on" + o, k))), j.add && (j.add.call(a, l), l.handler.guid || (l.handler.guid = c.guid)), e ? m.splice(m.delegateCount++, 0, l) : m.push(l), n.event.global[o] = !0);
                 a = null
             }
         },
         remove: function(a, b, c, d, e) {
-            var f, g, h, i, j, k, l, n, o, p, q, r = m.hasData(a) && m._data(a);
+            var f, g, h, i, j, k, l, m, o, p, q, r = n.hasData(a) && n._data(a);
             if (r && (k = r.events)) {
-                b = (b || "").match(E) || [""], j = b.length;
+                b = (b || "").match(G) || [""], j = b.length;
                 while (j--)
-                    if (h = _.exec(b[j]) || [], o = q = h[1], p = (h[2] || "").split(".").sort(), o) {
-                        l = m.event.special[o] || {}, o = (d ? l.delegateType : l.bindType) || o, n = k[o] || [], h = h[2] && new RegExp("(^|\\.)" + p.join("\\.(?:.*\\.|)") + "(\\.|$)"), i = f = n.length;
-                        while (f--) g = n[f], !e && q !== g.origType || c && c.guid !== g.guid || h && !h.test(g.namespace) || d && d !== g.selector && ("**" !== d || !g.selector) || (n.splice(f, 1), g.selector && n.delegateCount--, l.remove && l.remove.call(a, g));
-                        i && !n.length && (l.teardown && l.teardown.call(a, p, r.handle) !== !1 || m.removeEvent(a, o, r.handle), delete k[o])
+                    if (h = oa.exec(b[j]) || [], o = q = h[1], p = (h[2] || "").split(".").sort(), o) {
+                        l = n.event.special[o] || {}, o = (d ? l.delegateType : l.bindType) || o, m = k[o] || [], h = h[2] && new RegExp("(^|\\.)" + p.join("\\.(?:.*\\.|)") + "(\\.|$)"), i = f = m.length;
+                        while (f--) g = m[f], !e && q !== g.origType || c && c.guid !== g.guid || h && !h.test(g.namespace) || d && d !== g.selector && ("**" !== d || !g.selector) || (m.splice(f, 1), g.selector && m.delegateCount--, l.remove && l.remove.call(a, g));
+                        i && !m.length && (l.teardown && l.teardown.call(a, p, r.handle) !== !1 || n.removeEvent(a, o, r.handle), delete k[o])
                     } else
-                        for (o in k) m.event.remove(a, o + b[j], c, d, !0);
-                m.isEmptyObject(k) && (delete r.handle, m._removeData(a, "events"))
+                        for (o in k) n.event.remove(a, o + b[j], c, d, !0);
+                n.isEmptyObject(k) && (delete r.handle, n._removeData(a, "events"))
             }
         },
-        trigger: function(b, c, d, e) {
-            var f, g, h, i, k, l, n, o = [d || y],
-                p = j.call(b, "type") ? b.type : b,
-                q = j.call(b, "namespace") ? b.namespace.split(".") : [];
-            if (h = l = d = d || y, 3 !== d.nodeType && 8 !== d.nodeType && !$.test(p + m.event.triggered) && (p.indexOf(".") >= 0 && (q = p.split("."), p = q.shift(), q.sort()), g = p.indexOf(":") < 0 && "on" + p, b = b[m.expando] ? b : new m.Event(p, "object" == typeof b && b), b.isTrigger = e ? 2 : 3, b.namespace = q.join("."), b.namespace_re = b.namespace ? new RegExp("(^|\\.)" + q.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, b.result = void 0, b.target || (b.target = d), c = null == c ? [b] : m.makeArray(c, [b]), k = m.event.special[p] || {}, e || !k.trigger || k.trigger.apply(d, c) !== !1)) {
-                if (!e && !k.noBubble && !m.isWindow(d)) {
-                    for (i = k.delegateType || p, $.test(i + p) || (h = h.parentNode); h; h = h.parentNode) o.push(h), l = h;
-                    l === (d.ownerDocument || y) && o.push(l.defaultView || l.parentWindow || a)
-                }
-                n = 0;
-                while ((h = o[n++]) && !b.isPropagationStopped()) b.type = n > 1 ? i : k.bindType || p, f = (m._data(h, "events") || {})[b.type] && m._data(h, "handle"), f && f.apply(h, c), f = g && h[g], f && f.apply && m.acceptData(h) && (b.result = f.apply(h, c), b.result === !1 && b.preventDefault());
-                if (b.type = p, !e && !b.isDefaultPrevented() && (!k._default || k._default.apply(o.pop(), c) === !1) && m.acceptData(d) && g && d[p] && !m.isWindow(d)) {
-                    l = d[g], l && (d[g] = null), m.event.triggered = p;
+        trigger: function(b, c, e, f) {
+            var g, h, i, j, l, m, o, p = [e || d],
+                q = k.call(b, "type") ? b.type : b,
+                r = k.call(b, "namespace") ? b.namespace.split(".") : [];
+            if (i = m = e = e || d, 3 !== e.nodeType && 8 !== e.nodeType && !na.test(q + n.event.triggered) && (q.indexOf(".") > -1 && (r = q.split("."), q = r.shift(), r.sort()), h = q.indexOf(":") < 0 && "on" + q, b = b[n.expando] ? b : new n.Event(q, "object" == typeof b && b), b.isTrigger = f ? 2 : 3, b.namespace = r.join("."), b.rnamespace = b.namespace ? new RegExp("(^|\\.)" + r.join("\\.(?:.*\\.|)") + "(\\.|$)") : null, b.result = void 0, b.target || (b.target = e), c = null == c ? [b] : n.makeArray(c, [b]), l = n.event.special[q] || {}, f || !l.trigger || l.trigger.apply(e, c) !== !1)) {
+                if (!f && !l.noBubble && !n.isWindow(e)) {
+                    for (j = l.delegateType || q, na.test(j + q) || (i = i.parentNode); i; i = i.parentNode) p.push(i), m = i;
+                    m === (e.ownerDocument || d) && p.push(m.defaultView || m.parentWindow || a)
+                }
+                o = 0;
+                while ((i = p[o++]) && !b.isPropagationStopped()) b.type = o > 1 ? j : l.bindType || q, g = (n._data(i, "events") || {})[b.type] && n._data(i, "handle"), g && g.apply(i, c), g = h && i[h], g && g.apply && M(i) && (b.result = g.apply(i, c), b.result === !1 && b.preventDefault());
+                if (b.type = q, !f && !b.isDefaultPrevented() && (!l._default || l._default.apply(p.pop(), c) === !1) && M(e) && h && e[q] && !n.isWindow(e)) {
+                    m = e[h], m && (e[h] = null), n.event.triggered = q;
                     try {
-                        d[p]()
-                    } catch (r) {}
-                    m.event.triggered = void 0, l && (d[g] = l)
+                        e[q]()
+                    } catch (s) {}
+                    n.event.triggered = void 0, m && (e[h] = m)
                 }
                 return b.result
             }
         },
         dispatch: function(a) {
-            a = m.event.fix(a);
-            var b, c, e, f, g, h = [],
-                i = d.call(arguments),
-                j = (m._data(this, "events") || {})[a.type] || [],
-                k = m.event.special[a.type] || {};
+            a = n.event.fix(a);
+            var b, c, d, f, g, h = [],
+                i = e.call(arguments),
+                j = (n._data(this, "events") || {})[a.type] || [],
+                k = n.event.special[a.type] || {};
             if (i[0] = a, a.delegateTarget = this, !k.preDispatch || k.preDispatch.call(this, a) !== !1) {
-                h = m.event.handlers.call(this, a, j), b = 0;
+                h = n.event.handlers.call(this, a, j), b = 0;
                 while ((f = h[b++]) && !a.isPropagationStopped()) {
-                    a.currentTarget = f.elem, g = 0;
-                    while ((e = f.handlers[g++]) && !a.isImmediatePropagationStopped())(!a.namespace_re || a.namespace_re.test(e.namespace)) && (a.handleObj = e, a.data = e.data, c = ((m.event.special[e.origType] || {}).handle || e.handler).apply(f.elem, i), void 0 !== c && (a.result = c) === !1 && (a.preventDefault(), a.stopPropagation()))
+                    a.currentTarget = f.elem, c = 0;
+                    while ((g = f.handlers[c++]) && !a.isImmediatePropagationStopped()) a.rnamespace && !a.rnamespace.test(g.namespace) || (a.handleObj = g, a.data = g.data, d = ((n.event.special[g.origType] || {}).handle || g.handler).apply(f.elem, i), void 0 !== d && (a.result = d) === !1 && (a.preventDefault(), a.stopPropagation()))
                 }
                 return k.postDispatch && k.postDispatch.call(this, a), a.result
             }
         },
         handlers: function(a, b) {
             var c, d, e, f, g = [],
                 h = b.delegateCount,
                 i = a.target;
-            if (h && i.nodeType && (!a.button || "click" !== a.type))
+            if (h && i.nodeType && ("click" !== a.type || isNaN(a.button) || a.button < 1))
                 for (; i != this; i = i.parentNode || this)
                     if (1 === i.nodeType && (i.disabled !== !0 || "click" !== a.type)) {
-                        for (e = [], f = 0; h > f; f++) d = b[f], c = d.selector + " ", void 0 === e[c] && (e[c] = d.needsContext ? m(c, this).index(i) >= 0 : m.find(c, this, null, [i]).length), e[c] && e.push(d);
-                        e.length && g.push({
+                        for (d = [], c = 0; h > c; c++) f = b[c], e = f.selector + " ", void 0 === d[e] && (d[e] = f.needsContext ? n(e, this).index(i) > -1 : n.find(e, this, null, [i]).length), d[e] && d.push(f);
+                        d.length && g.push({
                             elem: i,
-                            handlers: e
+                            handlers: d
                         })
                     } return h < b.length && g.push({
                 elem: this,
                 handlers: b.slice(h)
             }), g
         },
         fix: function(a) {
-            if (a[m.expando]) return a;
-            var b, c, d, e = a.type,
-                f = a,
-                g = this.fixHooks[e];
-            g || (this.fixHooks[e] = g = Z.test(e) ? this.mouseHooks : Y.test(e) ? this.keyHooks : {}), d = g.props ? this.props.concat(g.props) : this.props, a = new m.Event(f), b = d.length;
-            while (b--) c = d[b], a[c] = f[c];
-            return a.target || (a.target = f.srcElement || y), 3 === a.target.nodeType && (a.target = a.target.parentNode), a.metaKey = !!a.metaKey, g.filter ? g.filter(a, f) : a
+            if (a[n.expando]) return a;
+            var b, c, e, f = a.type,
+                g = a,
+                h = this.fixHooks[f];
+            h || (this.fixHooks[f] = h = ma.test(f) ? this.mouseHooks : la.test(f) ? this.keyHooks : {}), e = h.props ? this.props.concat(h.props) : this.props, a = new n.Event(g), b = e.length;
+            while (b--) c = e[b], a[c] = g[c];
+            return a.target || (a.target = g.srcElement || d), 3 === a.target.nodeType && (a.target = a.target.parentNode), a.metaKey = !!a.metaKey, h.filter ? h.filter(a, g) : a
         },
-        props: "altKey bubbles cancelable ctrlKey currentTarget eventPhase metaKey relatedTarget shiftKey target timeStamp view which".split(" "),
+        props: "altKey bubbles cancelable ctrlKey currentTarget detail eventPhase metaKey relatedTarget shiftKey target timeStamp view which".split(" "),
         fixHooks: {},
         keyHooks: {
             props: "char charCode key keyCode".split(" "),
             filter: function(a, b) {
                 return null == a.which && (a.which = null != b.charCode ? b.charCode : b.keyCode), a
             }
         },
         mouseHooks: {
             props: "button buttons clientX clientY fromElement offsetX offsetY pageX pageY screenX screenY toElement".split(" "),
             filter: function(a, b) {
-                var c, d, e, f = b.button,
-                    g = b.fromElement;
-                return null == a.pageX && null != b.clientX && (d = a.target.ownerDocument || y, e = d.documentElement, c = d.body, a.pageX = b.clientX + (e && e.scrollLeft || c && c.scrollLeft || 0) - (e && e.clientLeft || c && c.clientLeft || 0), a.pageY = b.clientY + (e && e.scrollTop || c && c.scrollTop || 0) - (e && e.clientTop || c && c.clientTop || 0)), !a.relatedTarget && g && (a.relatedTarget = g === a.target ? b.toElement : g), a.which || void 0 === f || (a.which = 1 & f ? 1 : 2 & f ? 3 : 4 & f ? 2 : 0), a
+                var c, e, f, g = b.button,
+                    h = b.fromElement;
+                return null == a.pageX && null != b.clientX && (e = a.target.ownerDocument || d, f = e.documentElement, c = e.body, a.pageX = b.clientX + (f && f.scrollLeft || c && c.scrollLeft || 0) - (f && f.clientLeft || c && c.clientLeft || 0), a.pageY = b.clientY + (f && f.scrollTop || c && c.scrollTop || 0) - (f && f.clientTop || c && c.clientTop || 0)), !a.relatedTarget && h && (a.relatedTarget = h === a.target ? b.toElement : h), a.which || void 0 === g || (a.which = 1 & g ? 1 : 2 & g ? 3 : 4 & g ? 2 : 0), a
             }
         },
         special: {
             load: {
                 noBubble: !0
             },
             focus: {
                 trigger: function() {
-                    if (this !== ca() && this.focus) try {
+                    if (this !== ra() && this.focus) try {
                         return this.focus(), !1
                     } catch (a) {}
                 },
                 delegateType: "focusin"
             },
             blur: {
                 trigger: function() {
-                    return this === ca() && this.blur ? (this.blur(), !1) : void 0
+                    return this === ra() && this.blur ? (this.blur(), !1) : void 0
                 },
                 delegateType: "focusout"
             },
             click: {
                 trigger: function() {
-                    return m.nodeName(this, "input") && "checkbox" === this.type && this.click ? (this.click(), !1) : void 0
+                    return n.nodeName(this, "input") && "checkbox" === this.type && this.click ? (this.click(), !1) : void 0
                 },
                 _default: function(a) {
-                    return m.nodeName(a.target, "a")
+                    return n.nodeName(a.target, "a")
                 }
             },
             beforeunload: {
                 postDispatch: function(a) {
                     void 0 !== a.result && a.originalEvent && (a.originalEvent.returnValue = a.result)
                 }
             }
         },
-        simulate: function(a, b, c, d) {
-            var e = m.extend(new m.Event, c, {
+        simulate: function(a, b, c) {
+            var d = n.extend(new n.Event, c, {
                 type: a,
-                isSimulated: !0,
-                originalEvent: {}
+                isSimulated: !0
             });
-            d ? m.event.trigger(e, null, b) : m.event.dispatch.call(b, e), e.isDefaultPrevented() && c.preventDefault()
+            n.event.trigger(d, null, b), d.isDefaultPrevented() && c.preventDefault()
         }
-    }, m.removeEvent = y.removeEventListener ? function(a, b, c) {
-        a.removeEventListener && a.removeEventListener(b, c, !1)
+    }, n.removeEvent = d.removeEventListener ? function(a, b, c) {
+        a.removeEventListener && a.removeEventListener(b, c)
     } : function(a, b, c) {
         var d = "on" + b;
-        a.detachEvent && (typeof a[d] === K && (a[d] = null), a.detachEvent(d, c))
-    }, m.Event = function(a, b) {
-        return this instanceof m.Event ? (a && a.type ? (this.originalEvent = a, this.type = a.type, this.isDefaultPrevented = a.defaultPrevented || void 0 === a.defaultPrevented && a.returnValue === !1 ? aa : ba) : this.type = a, b && m.extend(this, b), this.timeStamp = a && a.timeStamp || m.now(), void(this[m.expando] = !0)) : new m.Event(a, b)
-    }, m.Event.prototype = {
-        isDefaultPrevented: ba,
-        isPropagationStopped: ba,
-        isImmediatePropagationStopped: ba,
+        a.detachEvent && ("undefined" == typeof a[d] && (a[d] = null), a.detachEvent(d, c))
+    }, n.Event = function(a, b) {
+        return this instanceof n.Event ? (a && a.type ? (this.originalEvent = a, this.type = a.type, this.isDefaultPrevented = a.defaultPrevented || void 0 === a.defaultPrevented && a.returnValue === !1 ? pa : qa) : this.type = a, b && n.extend(this, b), this.timeStamp = a && a.timeStamp || n.now(), void(this[n.expando] = !0)) : new n.Event(a, b)
+    }, n.Event.prototype = {
+        constructor: n.Event,
+        isDefaultPrevented: qa,
+        isPropagationStopped: qa,
+        isImmediatePropagationStopped: qa,
         preventDefault: function() {
             var a = this.originalEvent;
-            this.isDefaultPrevented = aa, a && (a.preventDefault ? a.preventDefault() : a.returnValue = !1)
+            this.isDefaultPrevented = pa, a && (a.preventDefault ? a.preventDefault() : a.returnValue = !1)
         },
         stopPropagation: function() {
             var a = this.originalEvent;
-            this.isPropagationStopped = aa, a && (a.stopPropagation && a.stopPropagation(), a.cancelBubble = !0)
+            this.isPropagationStopped = pa, a && !this.isSimulated && (a.stopPropagation && a.stopPropagation(), a.cancelBubble = !0)
         },
         stopImmediatePropagation: function() {
             var a = this.originalEvent;
-            this.isImmediatePropagationStopped = aa, a && a.stopImmediatePropagation && a.stopImmediatePropagation(), this.stopPropagation()
+            this.isImmediatePropagationStopped = pa, a && a.stopImmediatePropagation && a.stopImmediatePropagation(), this.stopPropagation()
         }
-    }, m.each({
+    }, n.each({
         mouseenter: "mouseover",
         mouseleave: "mouseout",
         pointerenter: "pointerover",
         pointerleave: "pointerout"
     }, function(a, b) {
-        m.event.special[a] = {
+        n.event.special[a] = {
             delegateType: b,
             bindType: b,
             handle: function(a) {
                 var c, d = this,
                     e = a.relatedTarget,
                     f = a.handleObj;
-                return (!e || e !== d && !m.contains(d, e)) && (a.type = f.origType, c = f.handler.apply(this, arguments), a.type = b), c
+                return e && (e === d || n.contains(d, e)) || (a.type = f.origType, c = f.handler.apply(this, arguments), a.type = b), c
             }
         }
-    }), k.submitBubbles || (m.event.special.submit = {
+    }), l.submit || (n.event.special.submit = {
         setup: function() {
-            return m.nodeName(this, "form") ? !1 : void m.event.add(this, "click._submit keypress._submit", function(a) {
+            return n.nodeName(this, "form") ? !1 : void n.event.add(this, "click._submit keypress._submit", function(a) {
                 var b = a.target,
-                    c = m.nodeName(b, "input") || m.nodeName(b, "button") ? b.form : void 0;
-                c && !m._data(c, "submitBubbles") && (m.event.add(c, "submit._submit", function(a) {
-                    a._submit_bubble = !0
-                }), m._data(c, "submitBubbles", !0))
+                    c = n.nodeName(b, "input") || n.nodeName(b, "button") ? n.prop(b, "form") : void 0;
+                c && !n._data(c, "submit") && (n.event.add(c, "submit._submit", function(a) {
+                    a._submitBubble = !0
+                }), n._data(c, "submit", !0))
             })
         },
         postDispatch: function(a) {
-            a._submit_bubble && (delete a._submit_bubble, this.parentNode && !a.isTrigger && m.event.simulate("submit", this.parentNode, a, !0))
+            a._submitBubble && (delete a._submitBubble, this.parentNode && !a.isTrigger && n.event.simulate("submit", this.parentNode, a))
         },
         teardown: function() {
-            return m.nodeName(this, "form") ? !1 : void m.event.remove(this, "._submit")
+            return n.nodeName(this, "form") ? !1 : void n.event.remove(this, "._submit")
         }
-    }), k.changeBubbles || (m.event.special.change = {
+    }), l.change || (n.event.special.change = {
         setup: function() {
-            return X.test(this.nodeName) ? (("checkbox" === this.type || "radio" === this.type) && (m.event.add(this, "propertychange._change", function(a) {
-                "checked" === a.originalEvent.propertyName && (this._just_changed = !0)
-            }), m.event.add(this, "click._change", function(a) {
-                this._just_changed && !a.isTrigger && (this._just_changed = !1), m.event.simulate("change", this, a, !0)
-            })), !1) : void m.event.add(this, "beforeactivate._change", function(a) {
+            return ka.test(this.nodeName) ? ("checkbox" !== this.type && "radio" !== this.type || (n.event.add(this, "propertychange._change", function(a) {
+                "checked" === a.originalEvent.propertyName && (this._justChanged = !0)
+            }), n.event.add(this, "click._change", function(a) {
+                this._justChanged && !a.isTrigger && (this._justChanged = !1), n.event.simulate("change", this, a)
+            })), !1) : void n.event.add(this, "beforeactivate._change", function(a) {
                 var b = a.target;
-                X.test(b.nodeName) && !m._data(b, "changeBubbles") && (m.event.add(b, "change._change", function(a) {
-                    !this.parentNode || a.isSimulated || a.isTrigger || m.event.simulate("change", this.parentNode, a, !0)
-                }), m._data(b, "changeBubbles", !0))
+                ka.test(b.nodeName) && !n._data(b, "change") && (n.event.add(b, "change._change", function(a) {
+                    !this.parentNode || a.isSimulated || a.isTrigger || n.event.simulate("change", this.parentNode, a)
+                }), n._data(b, "change", !0))
             })
         },
         handle: function(a) {
             var b = a.target;
             return this !== b || a.isSimulated || a.isTrigger || "radio" !== b.type && "checkbox" !== b.type ? a.handleObj.handler.apply(this, arguments) : void 0
         },
         teardown: function() {
-            return m.event.remove(this, "._change"), !X.test(this.nodeName)
+            return n.event.remove(this, "._change"), !ka.test(this.nodeName)
         }
-    }), k.focusinBubbles || m.each({
+    }), l.focusin || n.each({
         focus: "focusin",
         blur: "focusout"
     }, function(a, b) {
         var c = function(a) {
-            m.event.simulate(b, a.target, m.event.fix(a), !0)
+            n.event.simulate(b, a.target, n.event.fix(a))
         };
-        m.event.special[b] = {
+        n.event.special[b] = {
             setup: function() {
                 var d = this.ownerDocument || this,
-                    e = m._data(d, b);
-                e || d.addEventListener(a, c, !0), m._data(d, b, (e || 0) + 1)
+                    e = n._data(d, b);
+                e || d.addEventListener(a, c, !0), n._data(d, b, (e || 0) + 1)
             },
             teardown: function() {
                 var d = this.ownerDocument || this,
-                    e = m._data(d, b) - 1;
-                e ? m._data(d, b, e) : (d.removeEventListener(a, c, !0), m._removeData(d, b))
+                    e = n._data(d, b) - 1;
+                e ? n._data(d, b, e) : (d.removeEventListener(a, c, !0), n._removeData(d, b))
             }
         }
-    }), m.fn.extend({
-        on: function(a, b, c, d, e) {
-            var f, g;
-            if ("object" == typeof a) {
-                "string" != typeof b && (c = c || b, b = void 0);
-                for (f in a) this.on(f, b, c, a[f], e);
-                return this
-            }
-            if (null == c && null == d ? (d = b, c = b = void 0) : null == d && ("string" == typeof b ? (d = c, c = void 0) : (d = c, c = b, b = void 0)), d === !1) d = ba;
-            else if (!d) return this;
-            return 1 === e && (g = d, d = function(a) {
-                return m().off(a), g.apply(this, arguments)
-            }, d.guid = g.guid || (g.guid = m.guid++)), this.each(function() {
-                m.event.add(this, a, d, c, b)
-            })
+    }), n.fn.extend({
+        on: function(a, b, c, d) {
+            return sa(this, a, b, c, d)
         },
         one: function(a, b, c, d) {
-            return this.on(a, b, c, d, 1)
+            return sa(this, a, b, c, d, 1)
         },
         off: function(a, b, c) {
             var d, e;
-            if (a && a.preventDefault && a.handleObj) return d = a.handleObj, m(a.delegateTarget).off(d.namespace ? d.origType + "." + d.namespace : d.origType, d.selector, d.handler), this;
+            if (a && a.preventDefault && a.handleObj) return d = a.handleObj, n(a.delegateTarget).off(d.namespace ? d.origType + "." + d.namespace : d.origType, d.selector, d.handler), this;
             if ("object" == typeof a) {
                 for (e in a) this.off(e, b, a[e]);
                 return this
             }
-            return (b === !1 || "function" == typeof b) && (c = b, b = void 0), c === !1 && (c = ba), this.each(function() {
-                m.event.remove(this, a, c, b)
+            return b !== !1 && "function" != typeof b || (c = b, b = void 0), c === !1 && (c = qa), this.each(function() {
+                n.event.remove(this, a, c, b)
             })
         },
         trigger: function(a, b) {
             return this.each(function() {
-                m.event.trigger(a, b, this)
+                n.event.trigger(a, b, this)
             })
         },
         triggerHandler: function(a, b) {
             var c = this[0];
-            return c ? m.event.trigger(a, b, c, !0) : void 0
+            return c ? n.event.trigger(a, b, c, !0) : void 0
         }
     });
-
-    function da(a) {
-        var b = ea.split("|"),
-            c = a.createDocumentFragment();
-        if (c.createElement)
-            while (b.length) c.createElement(b.pop());
-        return c
-    }
-    var ea = "abbr|article|aside|audio|bdi|canvas|data|datalist|details|figcaption|figure|footer|header|hgroup|mark|meter|nav|output|progress|section|summary|time|video",
-        fa = / jQuery\d+="(?:null|\d+)"/g,
-        ga = new RegExp("<(?:" + ea + ")[\\s/>]", "i"),
-        ha = /^\s+/,
-        ia = /<(?!area|br|col|embed|hr|img|input|link|meta|param)(([\w:]+)[^>]*)\/>/gi,
-        ja = /<([\w:]+)/,
-        ka = /<tbody/i,
-        la = /<|&#?\w+;/,
-        ma = /<(?:script|style|link)/i,
-        na = /checked\s*(?:[^=]|=\s*.checked.)/i,
-        oa = /^$|\/(?:java|ecma)script/i,
-        pa = /^true\/(.*)/,
-        qa = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g,
-        ra = {
-            option: [1, "<select multiple='multiple'>", "</select>"],
-            legend: [1, "<fieldset>", "</fieldset>"],
-            area: [1, "<map>", "</map>"],
-            param: [1, "<object>", "</object>"],
-            thead: [1, "<table>", "</table>"],
-            tr: [2, "<table><tbody>", "</tbody></table>"],
-            col: [2, "<table><tbody></tbody><colgroup>", "</colgroup></table>"],
-            td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
-            _default: k.htmlSerialize ? [0, "", ""] : [1, "X<div>", "</div>"]
-        },
-        sa = da(y),
-        ta = sa.appendChild(y.createElement("div"));
-    ra.optgroup = ra.option, ra.tbody = ra.tfoot = ra.colgroup = ra.caption = ra.thead, ra.th = ra.td;
-
-    function ua(a, b) {
-        var c, d, e = 0,
-            f = typeof a.getElementsByTagName !== K ? a.getElementsByTagName(b || "*") : typeof a.querySelectorAll !== K ? a.querySelectorAll(b || "*") : void 0;
-        if (!f)
-            for (f = [], c = a.childNodes || a; null != (d = c[e]); e++) !b || m.nodeName(d, b) ? f.push(d) : m.merge(f, ua(d, b));
-        return void 0 === b || b && m.nodeName(a, b) ? m.merge([a], f) : f
-    }
-
-    function va(a) {
-        W.test(a.type) && (a.defaultChecked = a.checked)
-    }
-
-    function wa(a, b) {
-        return m.nodeName(a, "table") && m.nodeName(11 !== b.nodeType ? b : b.firstChild, "tr") ? a.getElementsByTagName("tbody")[0] || a.appendChild(a.ownerDocument.createElement("tbody")) : a
+    var ta = / jQuery\d+="(?:null|\d+)"/g,
+        ua = new RegExp("<(?:" + ba + ")[\\s/>]", "i"),
+        va = /<(?!area|br|col|embed|hr|img|input|link|meta|param)(([\w:-]+)[^>]*)\/>/gi,
+        wa = /<script|<style|<link/i,
+        xa = /checked\s*(?:[^=]|=\s*.checked.)/i,
+        ya = /^true\/(.*)/,
+        za = /^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g,
+        Aa = ca(d),
+        Ba = Aa.appendChild(d.createElement("div"));
+
+    function Ca(a, b) {
+        return n.nodeName(a, "table") && n.nodeName(11 !== b.nodeType ? b : b.firstChild, "tr") ? a.getElementsByTagName("tbody")[0] || a.appendChild(a.ownerDocument.createElement("tbody")) : a
     }
 
-    function xa(a) {
-        return a.type = (null !== m.find.attr(a, "type")) + "/" + a.type, a
+    function Da(a) {
+        return a.type = (null !== n.find.attr(a, "type")) + "/" + a.type, a
     }
 
-    function ya(a) {
-        var b = pa.exec(a.type);
+    function Ea(a) {
+        var b = ya.exec(a.type);
         return b ? a.type = b[1] : a.removeAttribute("type"), a
     }
 
-    function za(a, b) {
-        for (var c, d = 0; null != (c = a[d]); d++) m._data(c, "globalEval", !b || m._data(b[d], "globalEval"))
-    }
-
-    function Aa(a, b) {
-        if (1 === b.nodeType && m.hasData(a)) {
-            var c, d, e, f = m._data(a),
-                g = m._data(b, f),
+    function Fa(a, b) {
+        if (1 === b.nodeType && n.hasData(a)) {
+            var c, d, e, f = n._data(a),
+                g = n._data(b, f),
                 h = f.events;
             if (h) {
                 delete g.handle, g.events = {};
                 for (c in h)
-                    for (d = 0, e = h[c].length; e > d; d++) m.event.add(b, c, h[c][d])
+                    for (d = 0, e = h[c].length; e > d; d++) n.event.add(b, c, h[c][d])
             }
-            g.data && (g.data = m.extend({}, g.data))
+            g.data && (g.data = n.extend({}, g.data))
         }
     }
 
-    function Ba(a, b) {
+    function Ga(a, b) {
         var c, d, e;
         if (1 === b.nodeType) {
-            if (c = b.nodeName.toLowerCase(), !k.noCloneEvent && b[m.expando]) {
-                e = m._data(b);
-                for (d in e.events) m.removeEvent(b, d, e.handle);
-                b.removeAttribute(m.expando)
-            }
-            "script" === c && b.text !== a.text ? (xa(b).text = a.text, ya(b)) : "object" === c ? (b.parentNode && (b.outerHTML = a.outerHTML), k.html5Clone && a.innerHTML && !m.trim(b.innerHTML) && (b.innerHTML = a.innerHTML)) : "input" === c && W.test(a.type) ? (b.defaultChecked = b.checked = a.checked, b.value !== a.value && (b.value = a.value)) : "option" === c ? b.defaultSelected = b.selected = a.defaultSelected : ("input" === c || "textarea" === c) && (b.defaultValue = a.defaultValue)
+            if (c = b.nodeName.toLowerCase(), !l.noCloneEvent && b[n.expando]) {
+                e = n._data(b);
+                for (d in e.events) n.removeEvent(b, d, e.handle);
+                b.removeAttribute(n.expando)
+            }
+            "script" === c && b.text !== a.text ? (Da(b).text = a.text, Ea(b)) : "object" === c ? (b.parentNode && (b.outerHTML = a.outerHTML), l.html5Clone && a.innerHTML && !n.trim(b.innerHTML) && (b.innerHTML = a.innerHTML)) : "input" === c && Z.test(a.type) ? (b.defaultChecked = b.checked = a.checked, b.value !== a.value && (b.value = a.value)) : "option" === c ? b.defaultSelected = b.selected = a.defaultSelected : "input" !== c && "textarea" !== c || (b.defaultValue = a.defaultValue)
         }
     }
-    m.extend({
+
+    function Ha(a, b, c, d) {
+        b = f.apply([], b);
+        var e, g, h, i, j, k, m = 0,
+            o = a.length,
+            p = o - 1,
+            q = b[0],
+            r = n.isFunction(q);
+        if (r || o > 1 && "string" == typeof q && !l.checkClone && xa.test(q)) return a.each(function(e) {
+            var f = a.eq(e);
+            r && (b[0] = q.call(this, e, f.html())), Ha(f, b, c, d)
+        });
+        if (o && (k = ja(b, a[0].ownerDocument, !1, a, d), e = k.firstChild, 1 === k.childNodes.length && (k = e), e || d)) {
+            for (i = n.map(ea(k, "script"), Da), h = i.length; o > m; m++) g = k, m !== p && (g = n.clone(g, !0, !0), h && n.merge(i, ea(g, "script"))), c.call(a[m], g, m);
+            if (h)
+                for (j = i[i.length - 1].ownerDocument, n.map(i, Ea), m = 0; h > m; m++) g = i[m], _.test(g.type || "") && !n._data(g, "globalEval") && n.contains(j, g) && (g.src ? n._evalUrl && n._evalUrl(g.src) : n.globalEval((g.text || g.textContent || g.innerHTML || "").replace(za, "")));
+            k = e = null
+        }
+        return a
+    }
+
+    function Ia(a, b, c) {
+        for (var d, e = b ? n.filter(b, a) : a, f = 0; null != (d = e[f]); f++) c || 1 !== d.nodeType || n.cleanData(ea(d)), d.parentNode && (c && n.contains(d.ownerDocument, d) && fa(ea(d, "script")), d.parentNode.removeChild(d));
+        return a
+    }
+    n.extend({
+        htmlPrefilter: function(a) {
+            return a.replace(va, "<$1></$2>")
+        },
         clone: function(a, b, c) {
-            var d, e, f, g, h, i = m.contains(a.ownerDocument, a);
-            if (k.html5Clone || m.isXMLDoc(a) || !ga.test("<" + a.nodeName + ">") ? f = a.cloneNode(!0) : (ta.innerHTML = a.outerHTML, ta.removeChild(f = ta.firstChild)), !(k.noCloneEvent && k.noCloneChecked || 1 !== a.nodeType && 11 !== a.nodeType || m.isXMLDoc(a)))
-                for (d = ua(f), h = ua(a), g = 0; null != (e = h[g]); ++g) d[g] && Ba(e, d[g]);
+            var d, e, f, g, h, i = n.contains(a.ownerDocument, a);
+            if (l.html5Clone || n.isXMLDoc(a) || !ua.test("<" + a.nodeName + ">") ? f = a.cloneNode(!0) : (Ba.innerHTML = a.outerHTML, Ba.removeChild(f = Ba.firstChild)), !(l.noCloneEvent && l.noCloneChecked || 1 !== a.nodeType && 11 !== a.nodeType || n.isXMLDoc(a)))
+                for (d = ea(f), h = ea(a), g = 0; null != (e = h[g]); ++g) d[g] && Ga(e, d[g]);
             if (b)
                 if (c)
-                    for (h = h || ua(a), d = d || ua(f), g = 0; null != (e = h[g]); g++) Aa(e, d[g]);
-                else Aa(a, f);
-            return d = ua(f, "script"), d.length > 0 && za(d, !i && ua(a, "script")), d = h = e = null, f
-        },
-        buildFragment: function(a, b, c, d) {
-            for (var e, f, g, h, i, j, l, n = a.length, o = da(b), p = [], q = 0; n > q; q++)
-                if (f = a[q], f || 0 === f)
-                    if ("object" === m.type(f)) m.merge(p, f.nodeType ? [f] : f);
-                    else if (la.test(f)) {
-                h = h || o.appendChild(b.createElement("div")), i = (ja.exec(f) || ["", ""])[1].toLowerCase(), l = ra[i] || ra._default, h.innerHTML = l[1] + f.replace(ia, "<$1></$2>") + l[2], e = l[0];
-                while (e--) h = h.lastChild;
-                if (!k.leadingWhitespace && ha.test(f) && p.push(b.createTextNode(ha.exec(f)[0])), !k.tbody) {
-                    f = "table" !== i || ka.test(f) ? "<table>" !== l[1] || ka.test(f) ? 0 : h : h.firstChild, e = f && f.childNodes.length;
-                    while (e--) m.nodeName(j = f.childNodes[e], "tbody") && !j.childNodes.length && f.removeChild(j)
-                }
-                m.merge(p, h.childNodes), h.textContent = "";
-                while (h.firstChild) h.removeChild(h.firstChild);
-                h = o.lastChild
-            } else p.push(b.createTextNode(f));
-            h && o.removeChild(h), k.appendChecked || m.grep(ua(p, "input"), va), q = 0;
-            while (f = p[q++])
-                if ((!d || -1 === m.inArray(f, d)) && (g = m.contains(f.ownerDocument, f), h = ua(o.appendChild(f), "script"), g && za(h), c)) {
-                    e = 0;
-                    while (f = h[e++]) oa.test(f.type || "") && c.push(f)
-                } return h = null, o
+                    for (h = h || ea(a), d = d || ea(f), g = 0; null != (e = h[g]); g++) Fa(e, d[g]);
+                else Fa(a, f);
+            return d = ea(f, "script"), d.length > 0 && fa(d, !i && ea(a, "script")), d = h = e = null, f
         },
         cleanData: function(a, b) {
-            for (var d, e, f, g, h = 0, i = m.expando, j = m.cache, l = k.deleteExpando, n = m.event.special; null != (d = a[h]); h++)
-                if ((b || m.acceptData(d)) && (f = d[i], g = f && j[f])) {
+            for (var d, e, f, g, h = 0, i = n.expando, j = n.cache, k = l.attributes, m = n.event.special; null != (d = a[h]); h++)
+                if ((b || M(d)) && (f = d[i], g = f && j[f])) {
                     if (g.events)
-                        for (e in g.events) n[e] ? m.event.remove(d, e) : m.removeEvent(d, e, g.handle);
-                    j[f] && (delete j[f], l ? delete d[i] : typeof d.removeAttribute !== K ? d.removeAttribute(i) : d[i] = null, c.push(f))
+                        for (e in g.events) m[e] ? n.event.remove(d, e) : n.removeEvent(d, e, g.handle);
+                    j[f] && (delete j[f], k || "undefined" == typeof d.removeAttribute ? d[i] = void 0 : d.removeAttribute(i), c.push(f))
                 }
         }
-    }), m.fn.extend({
+    }), n.fn.extend({
+        domManip: Ha,
+        detach: function(a) {
+            return Ia(this, a, !0)
+        },
+        remove: function(a) {
+            return Ia(this, a)
+        },
         text: function(a) {
-            return V(this, function(a) {
-                return void 0 === a ? m.text(this) : this.empty().append((this[0] && this[0].ownerDocument || y).createTextNode(a))
+            return Y(this, function(a) {
+                return void 0 === a ? n.text(this) : this.empty().append((this[0] && this[0].ownerDocument || d).createTextNode(a))
             }, null, a, arguments.length)
         },
         append: function() {
-            return this.domManip(arguments, function(a) {
+            return Ha(this, arguments, function(a) {
                 if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
-                    var b = wa(this, a);
+                    var b = Ca(this, a);
                     b.appendChild(a)
                 }
             })
         },
         prepend: function() {
-            return this.domManip(arguments, function(a) {
+            return Ha(this, arguments, function(a) {
                 if (1 === this.nodeType || 11 === this.nodeType || 9 === this.nodeType) {
-                    var b = wa(this, a);
+                    var b = Ca(this, a);
                     b.insertBefore(a, b.firstChild)
                 }
             })
         },
         before: function() {
-            return this.domManip(arguments, function(a) {
+            return Ha(this, arguments, function(a) {
                 this.parentNode && this.parentNode.insertBefore(a, this)
             })
         },
         after: function() {
-            return this.domManip(arguments, function(a) {
+            return Ha(this, arguments, function(a) {
                 this.parentNode && this.parentNode.insertBefore(a, this.nextSibling)
             })
         },
-        remove: function(a, b) {
-            for (var c, d = a ? m.filter(a, this) : this, e = 0; null != (c = d[e]); e++) b || 1 !== c.nodeType || m.cleanData(ua(c)), c.parentNode && (b && m.contains(c.ownerDocument, c) && za(ua(c, "script")), c.parentNode.removeChild(c));
-            return this
-        },
         empty: function() {
             for (var a, b = 0; null != (a = this[b]); b++) {
-                1 === a.nodeType && m.cleanData(ua(a, !1));
+                1 === a.nodeType && n.cleanData(ea(a, !1));
                 while (a.firstChild) a.removeChild(a.firstChild);
-                a.options && m.nodeName(a, "select") && (a.options.length = 0)
+                a.options && n.nodeName(a, "select") && (a.options.length = 0)
             }
             return this
         },
         clone: function(a, b) {
             return a = null == a ? !1 : a, b = null == b ? a : b, this.map(function() {
-                return m.clone(this, a, b)
+                return n.clone(this, a, b)
             })
         },
         html: function(a) {
-            return V(this, function(a) {
+            return Y(this, function(a) {
                 var b = this[0] || {},
                     c = 0,
                     d = this.length;
-                if (void 0 === a) return 1 === b.nodeType ? b.innerHTML.replace(fa, "") : void 0;
-                if (!("string" != typeof a || ma.test(a) || !k.htmlSerialize && ga.test(a) || !k.leadingWhitespace && ha.test(a) || ra[(ja.exec(a) || ["", ""])[1].toLowerCase()])) {
-                    a = a.replace(ia, "<$1></$2>");
+                if (void 0 === a) return 1 === b.nodeType ? b.innerHTML.replace(ta, "") : void 0;
+                if ("string" == typeof a && !wa.test(a) && (l.htmlSerialize || !ua.test(a)) && (l.leadingWhitespace || !aa.test(a)) && !da[($.exec(a) || ["", ""])[1].toLowerCase()]) {
+                    a = n.htmlPrefilter(a);
                     try {
-                        for (; d > c; c++) b = this[c] || {}, 1 === b.nodeType && (m.cleanData(ua(b, !1)), b.innerHTML = a);
+                        for (; d > c; c++) b = this[c] || {}, 1 === b.nodeType && (n.cleanData(ea(b, !1)), b.innerHTML = a);
                         b = 0
                     } catch (e) {}
                 }
                 b && this.empty().append(a)
             }, null, a, arguments.length)
         },
         replaceWith: function() {
-            var a = arguments[0];
-            return this.domManip(arguments, function(b) {
-                a = this.parentNode, m.cleanData(ua(this)), a && a.replaceChild(b, this)
-            }), a && (a.length || a.nodeType) ? this : this.remove()
-        },
-        detach: function(a) {
-            return this.remove(a, !0)
-        },
-        domManip: function(a, b) {
-            a = e.apply([], a);
-            var c, d, f, g, h, i, j = 0,
-                l = this.length,
-                n = this,
-                o = l - 1,
-                p = a[0],
-                q = m.isFunction(p);
-            if (q || l > 1 && "string" == typeof p && !k.checkClone && na.test(p)) return this.each(function(c) {
-                var d = n.eq(c);
-                q && (a[0] = p.call(this, c, d.html())), d.domManip(a, b)
-            });
-            if (l && (i = m.buildFragment(a, this[0].ownerDocument, !1, this), c = i.firstChild, 1 === i.childNodes.length && (i = c), c)) {
-                for (g = m.map(ua(i, "script"), xa), f = g.length; l > j; j++) d = i, j !== o && (d = m.clone(d, !0, !0), f && m.merge(g, ua(d, "script"))), b.call(this[j], d, j);
-                if (f)
-                    for (h = g[g.length - 1].ownerDocument, m.map(g, ya), j = 0; f > j; j++) d = g[j], oa.test(d.type || "") && !m._data(d, "globalEval") && m.contains(h, d) && (d.src ? m._evalUrl && m._evalUrl(d.src) : m.globalEval((d.text || d.textContent || d.innerHTML || "").replace(qa, "")));
-                i = c = null
-            }
-            return this
+            var a = [];
+            return Ha(this, arguments, function(b) {
+                var c = this.parentNode;
+                n.inArray(this, a) < 0 && (n.cleanData(ea(this)), c && c.replaceChild(b, this))
+            }, a)
         }
-    }), m.each({
+    }), n.each({
         appendTo: "append",
         prependTo: "prepend",
         insertBefore: "before",
         insertAfter: "after",
         replaceAll: "replaceWith"
     }, function(a, b) {
-        m.fn[a] = function(a) {
-            for (var c, d = 0, e = [], g = m(a), h = g.length - 1; h >= d; d++) c = d === h ? this : this.clone(!0), m(g[d])[b](c), f.apply(e, c.get());
+        n.fn[a] = function(a) {
+            for (var c, d = 0, e = [], f = n(a), h = f.length - 1; h >= d; d++) c = d === h ? this : this.clone(!0), n(f[d])[b](c), g.apply(e, c.get());
             return this.pushStack(e)
         }
     });
-    var Ca, Da = {};
-
-    function Ea(b, c) {
-        var d, e = m(c.createElement(b)).appendTo(c.body),
-            f = a.getDefaultComputedStyle && (d = a.getDefaultComputedStyle(e[0])) ? d.display : m.css(e[0], "display");
-        return e.detach(), f
-    }
-
-    function Fa(a) {
-        var b = y,
-            c = Da[a];
-        return c || (c = Ea(a, b), "none" !== c && c || (Ca = (Ca || m("<iframe frameborder='0' width='0' height='0'/>")).appendTo(b.documentElement), b = (Ca[0].contentWindow || Ca[0].contentDocument).document, b.write(), b.close(), c = Ea(a, b), Ca.detach()), Da[a] = c), c
-    }! function() {
-        var a;
-        k.shrinkWrapBlocks = function() {
-            if (null != a) return a;
-            a = !1;
-            var b, c, d;
-            return c = y.getElementsByTagName("body")[0], c && c.style ? (b = y.createElement("div"), d = y.createElement("div"), d.style.cssText = "position:absolute;border:0;width:0;height:0;top:0;left:-9999px", c.appendChild(d).appendChild(b), typeof b.style.zoom !== K && (b.style.cssText = "-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;display:block;margin:0;border:0;padding:1px;width:1px;zoom:1", b.appendChild(y.createElement("div")).style.width = "5px", a = 3 !== b.offsetWidth), c.removeChild(d), a) : void 0
-        }
-    }();
-    var Ga = /^margin/,
-        Ha = new RegExp("^(" + S + ")(?!px)[a-z%]+$", "i"),
-        Ia, Ja, Ka = /^(top|right|bottom|left)$/;
-    a.getComputedStyle ? (Ia = function(b) {
-        return b.ownerDocument.defaultView.opener ? b.ownerDocument.defaultView.getComputedStyle(b, null) : a.getComputedStyle(b, null)
-    }, Ja = function(a, b, c) {
-        var d, e, f, g, h = a.style;
-        return c = c || Ia(a), g = c ? c.getPropertyValue(b) || c[b] : void 0, c && ("" !== g || m.contains(a.ownerDocument, a) || (g = m.style(a, b)), Ha.test(g) && Ga.test(b) && (d = h.width, e = h.minWidth, f = h.maxWidth, h.minWidth = h.maxWidth = h.width = g, g = c.width, h.width = d, h.minWidth = e, h.maxWidth = f)), void 0 === g ? g : g + ""
-    }) : y.documentElement.currentStyle && (Ia = function(a) {
-        return a.currentStyle
-    }, Ja = function(a, b, c) {
-        var d, e, f, g, h = a.style;
-        return c = c || Ia(a), g = c ? c[b] : void 0, null == g && h && h[b] && (g = h[b]), Ha.test(g) && !Ka.test(b) && (d = h.left, e = a.runtimeStyle, f = e && e.left, f && (e.left = a.currentStyle.left), h.left = "fontSize" === b ? "1em" : g, g = h.pixelLeft + "px", h.left = d, f && (e.left = f)), void 0 === g ? g : g + "" || "auto"
-    });
+    var Ja, Ka = {
+        HTML: "block",
+        BODY: "block"
+    };
 
     function La(a, b) {
-        return {
-            get: function() {
-                var c = a();
-                if (null != c) return c ? void delete this.get : (this.get = b).apply(this, arguments)
-            }
-        }
-    }! function() {
-        var b, c, d, e, f, g, h;
-        if (b = y.createElement("div"), b.innerHTML = "  <link/><table></table><a href='/a'>a</a><input type='checkbox'/>", d = b.getElementsByTagName("a")[0], c = d && d.style) {
-            c.cssText = "float:left;opacity:.5", k.opacity = "0.5" === c.opacity, k.cssFloat = !!c.cssFloat, b.style.backgroundClip = "content-box", b.cloneNode(!0).style.backgroundClip = "", k.clearCloneStyle = "content-box" === b.style.backgroundClip, k.boxSizing = "" === c.boxSizing || "" === c.MozBoxSizing || "" === c.WebkitBoxSizing, m.extend(k, {
+        var c = n(b.createElement(a)).appendTo(b.body),
+            d = n.css(c[0], "display");
+        return c.detach(), d
+    }
+
+    function Ma(a) {
+        var b = d,
+            c = Ka[a];
+        return c || (c = La(a, b), "none" !== c && c || (Ja = (Ja || n("<iframe frameborder='0' width='0' height='0'/>")).appendTo(b.documentElement), b = (Ja[0].contentWindow || Ja[0].contentDocument).document, b.write(), b.close(), c = La(a, b), Ja.detach()), Ka[a] = c), c
+    }
+    var Na = /^margin/,
+        Oa = new RegExp("^(" + T + ")(?!px)[a-z%]+$", "i"),
+        Pa = function(a, b, c, d) {
+            var e, f, g = {};
+            for (f in b) g[f] = a.style[f], a.style[f] = b[f];
+            e = c.apply(a, d || []);
+            for (f in b) a.style[f] = g[f];
+            return e
+        },
+        Qa = d.documentElement;
+    ! function() {
+        var b, c, e, f, g, h, i = d.createElement("div"),
+            j = d.createElement("div");
+        if (j.style) {
+            j.style.cssText = "float:left;opacity:.5", l.opacity = "0.5" === j.style.opacity, l.cssFloat = !!j.style.cssFloat, j.style.backgroundClip = "content-box", j.cloneNode(!0).style.backgroundClip = "", l.clearCloneStyle = "content-box" === j.style.backgroundClip, i = d.createElement("div"), i.style.cssText = "border:0;width:8px;height:0;top:0;left:-9999px;padding:0;margin-top:1px;position:absolute", j.innerHTML = "", i.appendChild(j), l.boxSizing = "" === j.style.boxSizing || "" === j.style.MozBoxSizing || "" === j.style.WebkitBoxSizing, n.extend(l, {
                 reliableHiddenOffsets: function() {
-                    return null == g && i(), g
+                    return null == b && k(), f
                 },
                 boxSizingReliable: function() {
-                    return null == f && i(), f
+                    return null == b && k(), e
+                },
+                pixelMarginRight: function() {
+                    return null == b && k(), c
                 },
                 pixelPosition: function() {
-                    return null == e && i(), e
+                    return null == b && k(), b
                 },
                 reliableMarginRight: function() {
-                    return null == h && i(), h
+                    return null == b && k(), g
+                },
+                reliableMarginLeft: function() {
+                    return null == b && k(), h
                 }
             });
 
-            function i() {
-                var b, c, d, i;
-                c = y.getElementsByTagName("body")[0], c && c.style && (b = y.createElement("div"), d = y.createElement("div"), d.style.cssText = "position:absolute;border:0;width:0;height:0;top:0;left:-9999px", c.appendChild(d).appendChild(b), b.style.cssText = "-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;display:block;margin-top:1%;top:1%;border:1px;padding:1px;width:4px;position:absolute", e = f = !1, h = !0, a.getComputedStyle && (e = "1%" !== (a.getComputedStyle(b, null) || {}).top, f = "4px" === (a.getComputedStyle(b, null) || {
+            function k() {
+                var k, l, m = d.documentElement;
+                m.appendChild(i), j.style.cssText = "-webkit-box-sizing:border-box;box-sizing:border-box;position:relative;display:block;margin:auto;border:1px;padding:1px;top:1%;width:50%", b = e = h = !1, c = g = !0, a.getComputedStyle && (l = a.getComputedStyle(j), b = "1%" !== (l || {}).top, h = "2px" === (l || {}).marginLeft, e = "4px" === (l || {
                     width: "4px"
-                }).width, i = b.appendChild(y.createElement("div")), i.style.cssText = b.style.cssText = "-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;display:block;margin:0;border:0;padding:0", i.style.marginRight = i.style.width = "0", b.style.width = "1px", h = !parseFloat((a.getComputedStyle(i, null) || {}).marginRight), b.removeChild(i)), b.innerHTML = "<table><tr><td></td><td>t</td></tr></table>", i = b.getElementsByTagName("td"), i[0].style.cssText = "margin:0;border:0;padding:0;display:none", g = 0 === i[0].offsetHeight, g && (i[0].style.display = "", i[1].style.display = "none", g = 0 === i[0].offsetHeight), c.removeChild(d))
+                }).width, j.style.marginRight = "50%", c = "4px" === (l || {
+                    marginRight: "4px"
+                }).marginRight, k = j.appendChild(d.createElement("div")), k.style.cssText = j.style.cssText = "-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;display:block;margin:0;border:0;padding:0", k.style.marginRight = k.style.width = "0", j.style.width = "1px", g = !parseFloat((a.getComputedStyle(k) || {}).marginRight), j.removeChild(k)), j.style.display = "none", f = 0 === j.getClientRects().length, f && (j.style.display = "", j.innerHTML = "<table><tr><td></td><td>t</td></tr></table>", j.childNodes[0].style.borderCollapse = "separate", k = j.getElementsByTagName("td"), k[0].style.cssText = "margin:0;border:0;padding:0;display:none", f = 0 === k[0].offsetHeight, f && (k[0].style.display = "", k[1].style.display = "none", f = 0 === k[0].offsetHeight)), m.removeChild(i)
             }
         }
-    }(), m.swap = function(a, b, c, d) {
-        var e, f, g = {};
-        for (f in b) g[f] = a.style[f], a.style[f] = b[f];
-        e = c.apply(a, d || []);
-        for (f in b) a.style[f] = g[f];
-        return e
-    };
-    var Ma = /alpha\([^)]*\)/i,
-        Na = /opacity\s*=\s*([^)]*)/,
-        Oa = /^(none|table(?!-c[ea]).+)/,
-        Pa = new RegExp("^(" + S + ")(.*)$", "i"),
-        Qa = new RegExp("^([+-])=(" + S + ")", "i"),
-        Ra = {
+    }();
+    var Ra, Sa, Ta = /^(top|right|bottom|left)$/;
+    a.getComputedStyle ? (Ra = function(b) {
+        var c = b.ownerDocument.defaultView;
+        return c && c.opener || (c = a), c.getComputedStyle(b)
+    }, Sa = function(a, b, c) {
+        var d, e, f, g, h = a.style;
+        return c = c || Ra(a), g = c ? c.getPropertyValue(b) || c[b] : void 0, "" !== g && void 0 !== g || n.contains(a.ownerDocument, a) || (g = n.style(a, b)), c && !l.pixelMarginRight() && Oa.test(g) && Na.test(b) && (d = h.width, e = h.minWidth, f = h.maxWidth, h.minWidth = h.maxWidth = h.width = g, g = c.width, h.width = d, h.minWidth = e, h.maxWidth = f), void 0 === g ? g : g + ""
+    }) : Qa.currentStyle && (Ra = function(a) {
+        return a.currentStyle
+    }, Sa = function(a, b, c) {
+        var d, e, f, g, h = a.style;
+        return c = c || Ra(a), g = c ? c[b] : void 0, null == g && h && h[b] && (g = h[b]), Oa.test(g) && !Ta.test(b) && (d = h.left, e = a.runtimeStyle, f = e && e.left, f && (e.left = a.currentStyle.left), h.left = "fontSize" === b ? "1em" : g, g = h.pixelLeft + "px", h.left = d, f && (e.left = f)), void 0 === g ? g : g + "" || "auto"
+    });
+
+    function Ua(a, b) {
+        return {
+            get: function() {
+                return a() ? void delete this.get : (this.get = b).apply(this, arguments)
+            }
+        }
+    }
+    var Va = /alpha\([^)]*\)/i,
+        Wa = /opacity\s*=\s*([^)]*)/i,
+        Xa = /^(none|table(?!-c[ea]).+)/,
+        Ya = new RegExp("^(" + T + ")(.*)$", "i"),
+        Za = {
             position: "absolute",
             visibility: "hidden",
             display: "block"
         },
-        Sa = {
+        $a = {
             letterSpacing: "0",
             fontWeight: "400"
         },
-        Ta = ["Webkit", "O", "Moz", "ms"];
+        _a = ["Webkit", "O", "Moz", "ms"],
+        ab = d.createElement("div").style;
 
-    function Ua(a, b) {
-        if (b in a) return b;
-        var c = b.charAt(0).toUpperCase() + b.slice(1),
-            d = b,
-            e = Ta.length;
-        while (e--)
-            if (b = Ta[e] + c, b in a) return b;
-        return d
+    function bb(a) {
+        if (a in ab) return a;
+        var b = a.charAt(0).toUpperCase() + a.slice(1),
+            c = _a.length;
+        while (c--)
+            if (a = _a[c] + b, a in ab) return a
     }
 
-    function Va(a, b) {
-        for (var c, d, e, f = [], g = 0, h = a.length; h > g; g++) d = a[g], d.style && (f[g] = m._data(d, "olddisplay"), c = d.style.display, b ? (f[g] || "none" !== c || (d.style.display = ""), "" === d.style.display && U(d) && (f[g] = m._data(d, "olddisplay", Fa(d.nodeName)))) : (e = U(d), (c && "none" !== c || !e) && m._data(d, "olddisplay", e ? c : m.css(d, "display"))));
+    function cb(a, b) {
+        for (var c, d, e, f = [], g = 0, h = a.length; h > g; g++) d = a[g], d.style && (f[g] = n._data(d, "olddisplay"), c = d.style.display, b ? (f[g] || "none" !== c || (d.style.display = ""), "" === d.style.display && W(d) && (f[g] = n._data(d, "olddisplay", Ma(d.nodeName)))) : (e = W(d), (c && "none" !== c || !e) && n._data(d, "olddisplay", e ? c : n.css(d, "display"))));
         for (g = 0; h > g; g++) d = a[g], d.style && (b && "none" !== d.style.display && "" !== d.style.display || (d.style.display = b ? f[g] || "" : "none"));
         return a
     }
 
-    function Wa(a, b, c) {
-        var d = Pa.exec(b);
+    function db(a, b, c) {
+        var d = Ya.exec(b);
         return d ? Math.max(0, d[1] - (c || 0)) + (d[2] || "px") : b
     }
 
-    function Xa(a, b, c, d, e) {
-        for (var f = c === (d ? "border" : "content") ? 4 : "width" === b ? 1 : 0, g = 0; 4 > f; f += 2) "margin" === c && (g += m.css(a, c + T[f], !0, e)), d ? ("content" === c && (g -= m.css(a, "padding" + T[f], !0, e)), "margin" !== c && (g -= m.css(a, "border" + T[f] + "Width", !0, e))) : (g += m.css(a, "padding" + T[f], !0, e), "padding" !== c && (g += m.css(a, "border" + T[f] + "Width", !0, e)));
+    function eb(a, b, c, d, e) {
+        for (var f = c === (d ? "border" : "content") ? 4 : "width" === b ? 1 : 0, g = 0; 4 > f; f += 2) "margin" === c && (g += n.css(a, c + V[f], !0, e)), d ? ("content" === c && (g -= n.css(a, "padding" + V[f], !0, e)), "margin" !== c && (g -= n.css(a, "border" + V[f] + "Width", !0, e))) : (g += n.css(a, "padding" + V[f], !0, e), "padding" !== c && (g += n.css(a, "border" + V[f] + "Width", !0, e)));
         return g
     }
 
-    function Ya(a, b, c) {
+    function fb(a, b, c) {
         var d = !0,
             e = "width" === b ? a.offsetWidth : a.offsetHeight,
-            f = Ia(a),
-            g = k.boxSizing && "border-box" === m.css(a, "boxSizing", !1, f);
+            f = Ra(a),
+            g = l.boxSizing && "border-box" === n.css(a, "boxSizing", !1, f);
         if (0 >= e || null == e) {
-            if (e = Ja(a, b, f), (0 > e || null == e) && (e = a.style[b]), Ha.test(e)) return e;
-            d = g && (k.boxSizingReliable() || e === a.style[b]), e = parseFloat(e) || 0
+            if (e = Sa(a, b, f), (0 > e || null == e) && (e = a.style[b]), Oa.test(e)) return e;
+            d = g && (l.boxSizingReliable() || e === a.style[b]), e = parseFloat(e) || 0
         }
-        return e + Xa(a, b, c || (g ? "border" : "content"), d, f) + "px"
+        return e + eb(a, b, c || (g ? "border" : "content"), d, f) + "px"
     }
-    m.extend({
+    n.extend({
         cssHooks: {
             opacity: {
                 get: function(a, b) {
                     if (b) {
-                        var c = Ja(a, "opacity");
+                        var c = Sa(a, "opacity");
                         return "" === c ? "1" : c
                     }
                 }
             }
         },
         cssNumber: {
+            animationIterationCount: !0,
             columnCount: !0,
             fillOpacity: !0,
             flexGrow: !0,
             flexShrink: !0,
             fontWeight: !0,
             lineHeight: !0,
             opacity: !0,
             order: !0,
             orphans: !0,
             widows: !0,
             zIndex: !0,
             zoom: !0
         },
         cssProps: {
-            "float": k.cssFloat ? "cssFloat" : "styleFloat"
+            "float": l.cssFloat ? "cssFloat" : "styleFloat"
         },
         style: function(a, b, c, d) {
             if (a && 3 !== a.nodeType && 8 !== a.nodeType && a.style) {
-                var e, f, g, h = m.camelCase(b),
+                var e, f, g, h = n.camelCase(b),
                     i = a.style;
-                if (b = m.cssProps[h] || (m.cssProps[h] = Ua(i, h)), g = m.cssHooks[b] || m.cssHooks[h], void 0 === c) return g && "get" in g && void 0 !== (e = g.get(a, !1, d)) ? e : i[b];
-                if (f = typeof c, "string" === f && (e = Qa.exec(c)) && (c = (e[1] + 1) * e[2] + parseFloat(m.css(a, b)), f = "number"), null != c && c === c && ("number" !== f || m.cssNumber[h] || (c += "px"), k.clearCloneStyle || "" !== c || 0 !== b.indexOf("background") || (i[b] = "inherit"), !(g && "set" in g && void 0 === (c = g.set(a, c, d))))) try {
+                if (b = n.cssProps[h] || (n.cssProps[h] = bb(h) || h), g = n.cssHooks[b] || n.cssHooks[h], void 0 === c) return g && "get" in g && void 0 !== (e = g.get(a, !1, d)) ? e : i[b];
+                if (f = typeof c, "string" === f && (e = U.exec(c)) && e[1] && (c = X(a, b, e), f = "number"), null != c && c === c && ("number" === f && (c += e && e[3] || (n.cssNumber[h] ? "" : "px")), l.clearCloneStyle || "" !== c || 0 !== b.indexOf("background") || (i[b] = "inherit"), !(g && "set" in g && void 0 === (c = g.set(a, c, d))))) try {
                     i[b] = c
                 } catch (j) {}
             }
         },
         css: function(a, b, c, d) {
-            var e, f, g, h = m.camelCase(b);
-            return b = m.cssProps[h] || (m.cssProps[h] = Ua(a.style, h)), g = m.cssHooks[b] || m.cssHooks[h], g && "get" in g && (f = g.get(a, !0, c)), void 0 === f && (f = Ja(a, b, d)), "normal" === f && b in Sa && (f = Sa[b]), "" === c || c ? (e = parseFloat(f), c === !0 || m.isNumeric(e) ? e || 0 : f) : f
+            var e, f, g, h = n.camelCase(b);
+            return b = n.cssProps[h] || (n.cssProps[h] = bb(h) || h), g = n.cssHooks[b] || n.cssHooks[h], g && "get" in g && (f = g.get(a, !0, c)), void 0 === f && (f = Sa(a, b, d)), "normal" === f && b in $a && (f = $a[b]), "" === c || c ? (e = parseFloat(f), c === !0 || isFinite(e) ? e || 0 : f) : f
         }
-    }), m.each(["height", "width"], function(a, b) {
-        m.cssHooks[b] = {
+    }), n.each(["height", "width"], function(a, b) {
+        n.cssHooks[b] = {
             get: function(a, c, d) {
-                return c ? Oa.test(m.css(a, "display")) && 0 === a.offsetWidth ? m.swap(a, Ra, function() {
-                    return Ya(a, b, d)
-                }) : Ya(a, b, d) : void 0
+                return c ? Xa.test(n.css(a, "display")) && 0 === a.offsetWidth ? Pa(a, Za, function() {
+                    return fb(a, b, d)
+                }) : fb(a, b, d) : void 0
             },
             set: function(a, c, d) {
-                var e = d && Ia(a);
-                return Wa(a, c, d ? Xa(a, b, d, k.boxSizing && "border-box" === m.css(a, "boxSizing", !1, e), e) : 0)
+                var e = d && Ra(a);
+                return db(a, c, d ? eb(a, b, d, l.boxSizing && "border-box" === n.css(a, "boxSizing", !1, e), e) : 0)
             }
         }
-    }), k.opacity || (m.cssHooks.opacity = {
+    }), l.opacity || (n.cssHooks.opacity = {
         get: function(a, b) {
-            return Na.test((b && a.currentStyle ? a.currentStyle.filter : a.style.filter) || "") ? .01 * parseFloat(RegExp.$1) + "" : b ? "1" : ""
+            return Wa.test((b && a.currentStyle ? a.currentStyle.filter : a.style.filter) || "") ? .01 * parseFloat(RegExp.$1) + "" : b ? "1" : ""
         },
         set: function(a, b) {
             var c = a.style,
                 d = a.currentStyle,
-                e = m.isNumeric(b) ? "alpha(opacity=" + 100 * b + ")" : "",
+                e = n.isNumeric(b) ? "alpha(opacity=" + 100 * b + ")" : "",
                 f = d && d.filter || c.filter || "";
-            c.zoom = 1, (b >= 1 || "" === b) && "" === m.trim(f.replace(Ma, "")) && c.removeAttribute && (c.removeAttribute("filter"), "" === b || d && !d.filter) || (c.filter = Ma.test(f) ? f.replace(Ma, e) : f + " " + e)
+            c.zoom = 1, (b >= 1 || "" === b) && "" === n.trim(f.replace(Va, "")) && c.removeAttribute && (c.removeAttribute("filter"), "" === b || d && !d.filter) || (c.filter = Va.test(f) ? f.replace(Va, e) : f + " " + e)
         }
-    }), m.cssHooks.marginRight = La(k.reliableMarginRight, function(a, b) {
-        return b ? m.swap(a, {
+    }), n.cssHooks.marginRight = Ua(l.reliableMarginRight, function(a, b) {
+        return b ? Pa(a, {
             display: "inline-block"
-        }, Ja, [a, "marginRight"]) : void 0
-    }), m.each({
+        }, Sa, [a, "marginRight"]) : void 0
+    }), n.cssHooks.marginLeft = Ua(l.reliableMarginLeft, function(a, b) {
+        return b ? (parseFloat(Sa(a, "marginLeft")) || (n.contains(a.ownerDocument, a) ? a.getBoundingClientRect().left - Pa(a, {
+            marginLeft: 0
+        }, function() {
+            return a.getBoundingClientRect().left
+        }) : 0)) + "px" : void 0
+    }), n.each({
         margin: "",
         padding: "",
         border: "Width"
     }, function(a, b) {
-        m.cssHooks[a + b] = {
+        n.cssHooks[a + b] = {
             expand: function(c) {
-                for (var d = 0, e = {}, f = "string" == typeof c ? c.split(" ") : [c]; 4 > d; d++) e[a + T[d] + b] = f[d] || f[d - 2] || f[0];
+                for (var d = 0, e = {}, f = "string" == typeof c ? c.split(" ") : [c]; 4 > d; d++) e[a + V[d] + b] = f[d] || f[d - 2] || f[0];
                 return e
             }
-        }, Ga.test(a) || (m.cssHooks[a + b].set = Wa)
-    }), m.fn.extend({
+        }, Na.test(a) || (n.cssHooks[a + b].set = db)
+    }), n.fn.extend({
         css: function(a, b) {
-            return V(this, function(a, b, c) {
+            return Y(this, function(a, b, c) {
                 var d, e, f = {},
                     g = 0;
-                if (m.isArray(b)) {
-                    for (d = Ia(a), e = b.length; e > g; g++) f[b[g]] = m.css(a, b[g], !1, d);
+                if (n.isArray(b)) {
+                    for (d = Ra(a), e = b.length; e > g; g++) f[b[g]] = n.css(a, b[g], !1, d);
                     return f
                 }
-                return void 0 !== c ? m.style(a, b, c) : m.css(a, b)
+                return void 0 !== c ? n.style(a, b, c) : n.css(a, b)
             }, a, b, arguments.length > 1)
         },
         show: function() {
-            return Va(this, !0)
+            return cb(this, !0)
         },
         hide: function() {
-            return Va(this)
+            return cb(this)
         },
         toggle: function(a) {
             return "boolean" == typeof a ? a ? this.show() : this.hide() : this.each(function() {
-                U(this) ? m(this).show() : m(this).hide()
+                W(this) ? n(this).show() : n(this).hide()
             })
         }
     });
 
-    function Za(a, b, c, d, e) {
-        return new Za.prototype.init(a, b, c, d, e)
+    function gb(a, b, c, d, e) {
+        return new gb.prototype.init(a, b, c, d, e)
     }
-    m.Tween = Za, Za.prototype = {
-        constructor: Za,
+    n.Tween = gb, gb.prototype = {
+        constructor: gb,
         init: function(a, b, c, d, e, f) {
-            this.elem = a, this.prop = c, this.easing = e || "swing", this.options = b, this.start = this.now = this.cur(), this.end = d, this.unit = f || (m.cssNumber[c] ? "" : "px")
+            this.elem = a, this.prop = c, this.easing = e || n.easing._default, this.options = b, this.start = this.now = this.cur(), this.end = d, this.unit = f || (n.cssNumber[c] ? "" : "px")
         },
         cur: function() {
-            var a = Za.propHooks[this.prop];
-            return a && a.get ? a.get(this) : Za.propHooks._default.get(this)
+            var a = gb.propHooks[this.prop];
+            return a && a.get ? a.get(this) : gb.propHooks._default.get(this)
         },
         run: function(a) {
-            var b, c = Za.propHooks[this.prop];
-            return this.options.duration ? this.pos = b = m.easing[this.easing](a, this.options.duration * a, 0, 1, this.options.duration) : this.pos = b = a, this.now = (this.end - this.start) * b + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), c && c.set ? c.set(this) : Za.propHooks._default.set(this), this
+            var b, c = gb.propHooks[this.prop];
+            return this.options.duration ? this.pos = b = n.easing[this.easing](a, this.options.duration * a, 0, 1, this.options.duration) : this.pos = b = a, this.now = (this.end - this.start) * b + this.start, this.options.step && this.options.step.call(this.elem, this.now, this), c && c.set ? c.set(this) : gb.propHooks._default.set(this), this
         }
-    }, Za.prototype.init.prototype = Za.prototype, Za.propHooks = {
+    }, gb.prototype.init.prototype = gb.prototype, gb.propHooks = {
         _default: {
             get: function(a) {
                 var b;
-                return null == a.elem[a.prop] || a.elem.style && null != a.elem.style[a.prop] ? (b = m.css(a.elem, a.prop, ""), b && "auto" !== b ? b : 0) : a.elem[a.prop]
+                return 1 !== a.elem.nodeType || null != a.elem[a.prop] && null == a.elem.style[a.prop] ? a.elem[a.prop] : (b = n.css(a.elem, a.prop, ""), b && "auto" !== b ? b : 0)
             },
             set: function(a) {
-                m.fx.step[a.prop] ? m.fx.step[a.prop](a) : a.elem.style && (null != a.elem.style[m.cssProps[a.prop]] || m.cssHooks[a.prop]) ? m.style(a.elem, a.prop, a.now + a.unit) : a.elem[a.prop] = a.now
+                n.fx.step[a.prop] ? n.fx.step[a.prop](a) : 1 !== a.elem.nodeType || null == a.elem.style[n.cssProps[a.prop]] && !n.cssHooks[a.prop] ? a.elem[a.prop] = a.now : n.style(a.elem, a.prop, a.now + a.unit)
             }
         }
-    }, Za.propHooks.scrollTop = Za.propHooks.scrollLeft = {
+    }, gb.propHooks.scrollTop = gb.propHooks.scrollLeft = {
         set: function(a) {
             a.elem.nodeType && a.elem.parentNode && (a.elem[a.prop] = a.now)
         }
-    }, m.easing = {
+    }, n.easing = {
         linear: function(a) {
             return a
         },
         swing: function(a) {
             return .5 - Math.cos(a * Math.PI) / 2
-        }
-    }, m.fx = Za.prototype.init, m.fx.step = {};
-    var $a, _a, ab = /^(?:toggle|show|hide)$/,
-        bb = new RegExp("^(?:([+-])=|)(" + S + ")([a-z%]*)$", "i"),
-        cb = /queueHooks$/,
-        db = [ib],
-        eb = {
-            "*": [function(a, b) {
-                var c = this.createTween(a, b),
-                    d = c.cur(),
-                    e = bb.exec(b),
-                    f = e && e[3] || (m.cssNumber[a] ? "" : "px"),
-                    g = (m.cssNumber[a] || "px" !== f && +d) && bb.exec(m.css(c.elem, a)),
-                    h = 1,
-                    i = 20;
-                if (g && g[3] !== f) {
-                    f = f || g[3], e = e || [], g = +d || 1;
-                    do h = h || ".5", g /= h, m.style(c.elem, a, g + f); while (h !== (h = c.cur() / d) && 1 !== h && --i)
-                }
-                return e && (g = c.start = +g || +d || 0, c.unit = f, c.end = e[1] ? g + (e[1] + 1) * e[2] : +e[2]), c
-            }]
-        };
-
-    function fb() {
-        return setTimeout(function() {
-            $a = void 0
-        }), $a = m.now()
+        },
+        _default: "swing"
+    }, n.fx = gb.prototype.init, n.fx.step = {};
+    var hb, ib, jb = /^(?:toggle|show|hide)$/,
+        kb = /queueHooks$/;
+
+    function lb() {
+        return a.setTimeout(function() {
+            hb = void 0
+        }), hb = n.now()
     }
 
-    function gb(a, b) {
+    function mb(a, b) {
         var c, d = {
                 height: a
             },
             e = 0;
-        for (b = b ? 1 : 0; 4 > e; e += 2 - b) c = T[e], d["margin" + c] = d["padding" + c] = a;
+        for (b = b ? 1 : 0; 4 > e; e += 2 - b) c = V[e], d["margin" + c] = d["padding" + c] = a;
         return b && (d.opacity = d.width = a), d
     }
 
-    function hb(a, b, c) {
-        for (var d, e = (eb[b] || []).concat(eb["*"]), f = 0, g = e.length; g > f; f++)
+    function nb(a, b, c) {
+        for (var d, e = (qb.tweeners[b] || []).concat(qb.tweeners["*"]), f = 0, g = e.length; g > f; f++)
             if (d = e[f].call(c, b, a)) return d
     }
 
-    function ib(a, b, c) {
-        var d, e, f, g, h, i, j, l, n = this,
+    function ob(a, b, c) {
+        var d, e, f, g, h, i, j, k, m = this,
             o = {},
             p = a.style,
-            q = a.nodeType && U(a),
-            r = m._data(a, "fxshow");
-        c.queue || (h = m._queueHooks(a, "fx"), null == h.unqueued && (h.unqueued = 0, i = h.empty.fire, h.empty.fire = function() {
+            q = a.nodeType && W(a),
+            r = n._data(a, "fxshow");
+        c.queue || (h = n._queueHooks(a, "fx"), null == h.unqueued && (h.unqueued = 0, i = h.empty.fire, h.empty.fire = function() {
             h.unqueued || i()
-        }), h.unqueued++, n.always(function() {
-            n.always(function() {
-                h.unqueued--, m.queue(a, "fx").length || h.empty.fire()
+        }), h.unqueued++, m.always(function() {
+            m.always(function() {
+                h.unqueued--, n.queue(a, "fx").length || h.empty.fire()
             })
-        })), 1 === a.nodeType && ("height" in b || "width" in b) && (c.overflow = [p.overflow, p.overflowX, p.overflowY], j = m.css(a, "display"), l = "none" === j ? m._data(a, "olddisplay") || Fa(a.nodeName) : j, "inline" === l && "none" === m.css(a, "float") && (k.inlineBlockNeedsLayout && "inline" !== Fa(a.nodeName) ? p.zoom = 1 : p.display = "inline-block")), c.overflow && (p.overflow = "hidden", k.shrinkWrapBlocks() || n.always(function() {
+        })), 1 === a.nodeType && ("height" in b || "width" in b) && (c.overflow = [p.overflow, p.overflowX, p.overflowY], j = n.css(a, "display"), k = "none" === j ? n._data(a, "olddisplay") || Ma(a.nodeName) : j, "inline" === k && "none" === n.css(a, "float") && (l.inlineBlockNeedsLayout && "inline" !== Ma(a.nodeName) ? p.zoom = 1 : p.display = "inline-block")), c.overflow && (p.overflow = "hidden", l.shrinkWrapBlocks() || m.always(function() {
             p.overflow = c.overflow[0], p.overflowX = c.overflow[1], p.overflowY = c.overflow[2]
         }));
         for (d in b)
-            if (e = b[d], ab.exec(e)) {
+            if (e = b[d], jb.exec(e)) {
                 if (delete b[d], f = f || "toggle" === e, e === (q ? "hide" : "show")) {
                     if ("show" !== e || !r || void 0 === r[d]) continue;
                     q = !0
                 }
-                o[d] = r && r[d] || m.style(a, d)
+                o[d] = r && r[d] || n.style(a, d)
             } else j = void 0;
-        if (m.isEmptyObject(o)) "inline" === ("none" === j ? Fa(a.nodeName) : j) && (p.display = j);
+        if (n.isEmptyObject(o)) "inline" === ("none" === j ? Ma(a.nodeName) : j) && (p.display = j);
         else {
-            r ? "hidden" in r && (q = r.hidden) : r = m._data(a, "fxshow", {}), f && (r.hidden = !q), q ? m(a).show() : n.done(function() {
-                m(a).hide()
-            }), n.done(function() {
+            r ? "hidden" in r && (q = r.hidden) : r = n._data(a, "fxshow", {}), f && (r.hidden = !q), q ? n(a).show() : m.done(function() {
+                n(a).hide()
+            }), m.done(function() {
                 var b;
-                m._removeData(a, "fxshow");
-                for (b in o) m.style(a, b, o[b])
+                n._removeData(a, "fxshow");
+                for (b in o) n.style(a, b, o[b])
             });
-            for (d in o) g = hb(q ? r[d] : 0, d, n), d in r || (r[d] = g.start, q && (g.end = g.start, g.start = "width" === d || "height" === d ? 1 : 0))
+            for (d in o) g = nb(q ? r[d] : 0, d, m), d in r || (r[d] = g.start, q && (g.end = g.start, g.start = "width" === d || "height" === d ? 1 : 0))
         }
     }
 
-    function jb(a, b) {
+    function pb(a, b) {
         var c, d, e, f, g;
         for (c in a)
-            if (d = m.camelCase(c), e = b[d], f = a[c], m.isArray(f) && (e = f[1], f = a[c] = f[0]), c !== d && (a[d] = f, delete a[c]), g = m.cssHooks[d], g && "expand" in g) {
+            if (d = n.camelCase(c), e = b[d], f = a[c], n.isArray(f) && (e = f[1], f = a[c] = f[0]), c !== d && (a[d] = f, delete a[c]), g = n.cssHooks[d], g && "expand" in g) {
                 f = g.expand(f), delete a[d];
                 for (c in f) c in a || (a[c] = f[c], b[c] = e)
             } else b[d] = e
     }
 
-    function kb(a, b, c) {
+    function qb(a, b, c) {
         var d, e, f = 0,
-            g = db.length,
-            h = m.Deferred().always(function() {
+            g = qb.prefilters.length,
+            h = n.Deferred().always(function() {
                 delete i.elem
             }),
             i = function() {
                 if (e) return !1;
-                for (var b = $a || fb(), c = Math.max(0, j.startTime + j.duration - b), d = c / j.duration || 0, f = 1 - d, g = 0, i = j.tweens.length; i > g; g++) j.tweens[g].run(f);
+                for (var b = hb || lb(), c = Math.max(0, j.startTime + j.duration - b), d = c / j.duration || 0, f = 1 - d, g = 0, i = j.tweens.length; i > g; g++) j.tweens[g].run(f);
                 return h.notifyWith(a, [j, f, c]), 1 > f && i ? c : (h.resolveWith(a, [j]), !1)
             },
             j = h.promise({
                 elem: a,
-                props: m.extend({}, b),
-                opts: m.extend(!0, {
-                    specialEasing: {}
+                props: n.extend({}, b),
+                opts: n.extend(!0, {
+                    specialEasing: {},
+                    easing: n.easing._default
                 }, c),
                 originalProperties: b,
                 originalOptions: c,
-                startTime: $a || fb(),
+                startTime: hb || lb(),
                 duration: c.duration,
                 tweens: [],
                 createTween: function(b, c) {
-                    var d = m.Tween(a, j.opts, b, c, j.opts.specialEasing[b] || j.opts.easing);
+                    var d = n.Tween(a, j.opts, b, c, j.opts.specialEasing[b] || j.opts.easing);
                     return j.tweens.push(d), d
                 },
                 stop: function(b) {
                     var c = 0,
                         d = b ? j.tweens.length : 0;
                     if (e) return this;
                     for (e = !0; d > c; c++) j.tweens[c].run(1);
-                    return b ? h.resolveWith(a, [j, b]) : h.rejectWith(a, [j, b]), this
+                    return b ? (h.notifyWith(a, [j, 1, 0]), h.resolveWith(a, [j, b])) : h.rejectWith(a, [j, b]), this
                 }
             }),
             k = j.props;
-        for (jb(k, j.opts.specialEasing); g > f; f++)
-            if (d = db[f].call(j, a, k, j.opts)) return d;
-        return m.map(k, hb, j), m.isFunction(j.opts.start) && j.opts.start.call(a, j), m.fx.timer(m.extend(i, {
+        for (pb(k, j.opts.specialEasing); g > f; f++)
+            if (d = qb.prefilters[f].call(j, a, k, j.opts)) return n.isFunction(d.stop) && (n._queueHooks(j.elem, j.opts.queue).stop = n.proxy(d.stop, d)), d;
+        return n.map(k, nb, j), n.isFunction(j.opts.start) && j.opts.start.call(a, j), n.fx.timer(n.extend(i, {
             elem: a,
             anim: j,
             queue: j.opts.queue
         })), j.progress(j.opts.progress).done(j.opts.done, j.opts.complete).fail(j.opts.fail).always(j.opts.always)
     }
-    m.Animation = m.extend(kb, {
+    n.Animation = n.extend(qb, {
+            tweeners: {
+                "*": [function(a, b) {
+                    var c = this.createTween(a, b);
+                    return X(c.elem, a, U.exec(b), c), c
+                }]
+            },
             tweener: function(a, b) {
-                m.isFunction(a) ? (b = a, a = ["*"]) : a = a.split(" ");
-                for (var c, d = 0, e = a.length; e > d; d++) c = a[d], eb[c] = eb[c] || [], eb[c].unshift(b)
+                n.isFunction(a) ? (b = a, a = ["*"]) : a = a.match(G);
+                for (var c, d = 0, e = a.length; e > d; d++) c = a[d], qb.tweeners[c] = qb.tweeners[c] || [], qb.tweeners[c].unshift(b)
             },
+            prefilters: [ob],
             prefilter: function(a, b) {
-                b ? db.unshift(a) : db.push(a)
+                b ? qb.prefilters.unshift(a) : qb.prefilters.push(a)
             }
-        }), m.speed = function(a, b, c) {
-            var d = a && "object" == typeof a ? m.extend({}, a) : {
-                complete: c || !c && b || m.isFunction(a) && a,
+        }), n.speed = function(a, b, c) {
+            var d = a && "object" == typeof a ? n.extend({}, a) : {
+                complete: c || !c && b || n.isFunction(a) && a,
                 duration: a,
-                easing: c && b || b && !m.isFunction(b) && b
+                easing: c && b || b && !n.isFunction(b) && b
             };
-            return d.duration = m.fx.off ? 0 : "number" == typeof d.duration ? d.duration : d.duration in m.fx.speeds ? m.fx.speeds[d.duration] : m.fx.speeds._default, (null == d.queue || d.queue === !0) && (d.queue = "fx"), d.old = d.complete, d.complete = function() {
-                m.isFunction(d.old) && d.old.call(this), d.queue && m.dequeue(this, d.queue)
+            return d.duration = n.fx.off ? 0 : "number" == typeof d.duration ? d.duration : d.duration in n.fx.speeds ? n.fx.speeds[d.duration] : n.fx.speeds._default, null != d.queue && d.queue !== !0 || (d.queue = "fx"), d.old = d.complete, d.complete = function() {
+                n.isFunction(d.old) && d.old.call(this), d.queue && n.dequeue(this, d.queue)
             }, d
-        }, m.fn.extend({
+        }, n.fn.extend({
             fadeTo: function(a, b, c, d) {
-                return this.filter(U).css("opacity", 0).show().end().animate({
+                return this.filter(W).css("opacity", 0).show().end().animate({
                     opacity: b
                 }, a, c, d)
             },
             animate: function(a, b, c, d) {
-                var e = m.isEmptyObject(a),
-                    f = m.speed(b, c, d),
+                var e = n.isEmptyObject(a),
+                    f = n.speed(b, c, d),
                     g = function() {
-                        var b = kb(this, m.extend({}, a), f);
-                        (e || m._data(this, "finish")) && b.stop(!0)
+                        var b = qb(this, n.extend({}, a), f);
+                        (e || n._data(this, "finish")) && b.stop(!0)
                     };
                 return g.finish = g, e || f.queue === !1 ? this.each(g) : this.queue(f.queue, g)
             },
             stop: function(a, b, c) {
                 var d = function(a) {
                     var b = a.stop;
                     delete a.stop, b(c)
                 };
                 return "string" != typeof a && (c = b, b = a, a = void 0), b && a !== !1 && this.queue(a || "fx", []), this.each(function() {
                     var b = !0,
                         e = null != a && a + "queueHooks",
-                        f = m.timers,
-                        g = m._data(this);
+                        f = n.timers,
+                        g = n._data(this);
                     if (e) g[e] && g[e].stop && d(g[e]);
                     else
-                        for (e in g) g[e] && g[e].stop && cb.test(e) && d(g[e]);
+                        for (e in g) g[e] && g[e].stop && kb.test(e) && d(g[e]);
                     for (e = f.length; e--;) f[e].elem !== this || null != a && f[e].queue !== a || (f[e].anim.stop(c), b = !1, f.splice(e, 1));
-                    (b || !c) && m.dequeue(this, a)
+                    !b && c || n.dequeue(this, a)
                 })
             },
             finish: function(a) {
                 return a !== !1 && (a = a || "fx"), this.each(function() {
-                    var b, c = m._data(this),
+                    var b, c = n._data(this),
                         d = c[a + "queue"],
                         e = c[a + "queueHooks"],
-                        f = m.timers,
+                        f = n.timers,
                         g = d ? d.length : 0;
-                    for (c.finish = !0, m.queue(this, a, []), e && e.stop && e.stop.call(this, !0), b = f.length; b--;) f[b].elem === this && f[b].queue === a && (f[b].anim.stop(!0), f.splice(b, 1));
+                    for (c.finish = !0, n.queue(this, a, []), e && e.stop && e.stop.call(this, !0), b = f.length; b--;) f[b].elem === this && f[b].queue === a && (f[b].anim.stop(!0), f.splice(b, 1));
                     for (b = 0; g > b; b++) d[b] && d[b].finish && d[b].finish.call(this);
                     delete c.finish
                 })
             }
-        }), m.each(["toggle", "show", "hide"], function(a, b) {
-            var c = m.fn[b];
-            m.fn[b] = function(a, d, e) {
-                return null == a || "boolean" == typeof a ? c.apply(this, arguments) : this.animate(gb(b, !0), a, d, e)
-            }
-        }), m.each({
-            slideDown: gb("show"),
-            slideUp: gb("hide"),
-            slideToggle: gb("toggle"),
+        }), n.each(["toggle", "show", "hide"], function(a, b) {
+            var c = n.fn[b];
+            n.fn[b] = function(a, d, e) {
+                return null == a || "boolean" == typeof a ? c.apply(this, arguments) : this.animate(mb(b, !0), a, d, e)
+            }
+        }), n.each({
+            slideDown: mb("show"),
+            slideUp: mb("hide"),
+            slideToggle: mb("toggle"),
             fadeIn: {
                 opacity: "show"
             },
             fadeOut: {
                 opacity: "hide"
             },
             fadeToggle: {
                 opacity: "toggle"
             }
         }, function(a, b) {
-            m.fn[a] = function(a, c, d) {
+            n.fn[a] = function(a, c, d) {
                 return this.animate(b, a, c, d)
             }
-        }), m.timers = [], m.fx.tick = function() {
-            var a, b = m.timers,
+        }), n.timers = [], n.fx.tick = function() {
+            var a, b = n.timers,
                 c = 0;
-            for ($a = m.now(); c < b.length; c++) a = b[c], a() || b[c] !== a || b.splice(c--, 1);
-            b.length || m.fx.stop(), $a = void 0
-        }, m.fx.timer = function(a) {
-            m.timers.push(a), a() ? m.fx.start() : m.timers.pop()
-        }, m.fx.interval = 13, m.fx.start = function() {
-            _a || (_a = setInterval(m.fx.tick, m.fx.interval))
-        }, m.fx.stop = function() {
-            clearInterval(_a), _a = null
-        }, m.fx.speeds = {
+            for (hb = n.now(); c < b.length; c++) a = b[c], a() || b[c] !== a || b.splice(c--, 1);
+            b.length || n.fx.stop(), hb = void 0
+        }, n.fx.timer = function(a) {
+            n.timers.push(a), a() ? n.fx.start() : n.timers.pop()
+        }, n.fx.interval = 13, n.fx.start = function() {
+            ib || (ib = a.setInterval(n.fx.tick, n.fx.interval))
+        }, n.fx.stop = function() {
+            a.clearInterval(ib), ib = null
+        }, n.fx.speeds = {
             slow: 600,
             fast: 200,
             _default: 400
-        }, m.fn.delay = function(a, b) {
-            return a = m.fx ? m.fx.speeds[a] || a : a, b = b || "fx", this.queue(b, function(b, c) {
-                var d = setTimeout(b, a);
-                c.stop = function() {
-                    clearTimeout(d)
+        }, n.fn.delay = function(b, c) {
+            return b = n.fx ? n.fx.speeds[b] || b : b, c = c || "fx", this.queue(c, function(c, d) {
+                var e = a.setTimeout(c, b);
+                d.stop = function() {
+                    a.clearTimeout(e)
                 }
             })
         },
         function() {
-            var a, b, c, d, e;
-            b = y.createElement("div"), b.setAttribute("className", "t"), b.innerHTML = "  <link/><table></table><a href='/a'>a</a><input type='checkbox'/>", d = b.getElementsByTagName("a")[0], c = y.createElement("select"), e = c.appendChild(y.createElement("option")), a = b.getElementsByTagName("input")[0], d.style.cssText = "top:1px", k.getSetAttribute = "t" !== b.className, k.style = /top/.test(d.getAttribute("style")), k.hrefNormalized = "/a" === d.getAttribute("href"), k.checkOn = !!a.value, k.optSelected = e.selected, k.enctype = !!y.createElement("form").enctype, c.disabled = !0, k.optDisabled = !e.disabled, a = y.createElement("input"), a.setAttribute("value", ""), k.input = "" === a.getAttribute("value"), a.value = "t", a.setAttribute("type", "radio"), k.radioValue = "t" === a.value
+            var a, b = d.createElement("input"),
+                c = d.createElement("div"),
+                e = d.createElement("select"),
+                f = e.appendChild(d.createElement("option"));
+            c = d.createElement("div"), c.setAttribute("className", "t"), c.innerHTML = "  <link/><table></table><a href='/a'>a</a><input type='checkbox'/>", a = c.getElementsByTagName("a")[0], b.setAttribute("type", "checkbox"), c.appendChild(b), a = c.getElementsByTagName("a")[0], a.style.cssText = "top:1px", l.getSetAttribute = "t" !== c.className, l.style = /top/.test(a.getAttribute("style")), l.hrefNormalized = "/a" === a.getAttribute("href"), l.checkOn = !!b.value, l.optSelected = f.selected, l.enctype = !!d.createElement("form").enctype, e.disabled = !0, l.optDisabled = !f.disabled, b = d.createElement("input"), b.setAttribute("value", ""), l.input = "" === b.getAttribute("value"), b.value = "t", b.setAttribute("type", "radio"), l.radioValue = "t" === b.value
         }();
-    var lb = /\r/g;
-    m.fn.extend({
+    var rb = /\r/g,
+        sb = /[\x20\t\r\n\f]+/g;
+    n.fn.extend({
         val: function(a) {
             var b, c, d, e = this[0]; {
-                if (arguments.length) return d = m.isFunction(a), this.each(function(c) {
+                if (arguments.length) return d = n.isFunction(a), this.each(function(c) {
                     var e;
-                    1 === this.nodeType && (e = d ? a.call(this, c, m(this).val()) : a, null == e ? e = "" : "number" == typeof e ? e += "" : m.isArray(e) && (e = m.map(e, function(a) {
+                    1 === this.nodeType && (e = d ? a.call(this, c, n(this).val()) : a, null == e ? e = "" : "number" == typeof e ? e += "" : n.isArray(e) && (e = n.map(e, function(a) {
                         return null == a ? "" : a + ""
-                    })), b = m.valHooks[this.type] || m.valHooks[this.nodeName.toLowerCase()], b && "set" in b && void 0 !== b.set(this, e, "value") || (this.value = e))
+                    })), b = n.valHooks[this.type] || n.valHooks[this.nodeName.toLowerCase()], b && "set" in b && void 0 !== b.set(this, e, "value") || (this.value = e))
                 });
-                if (e) return b = m.valHooks[e.type] || m.valHooks[e.nodeName.toLowerCase()], b && "get" in b && void 0 !== (c = b.get(e, "value")) ? c : (c = e.value, "string" == typeof c ? c.replace(lb, "") : null == c ? "" : c)
+                if (e) return b = n.valHooks[e.type] || n.valHooks[e.nodeName.toLowerCase()], b && "get" in b && void 0 !== (c = b.get(e, "value")) ? c : (c = e.value, "string" == typeof c ? c.replace(rb, "") : null == c ? "" : c)
             }
         }
-    }), m.extend({
+    }), n.extend({
         valHooks: {
             option: {
                 get: function(a) {
-                    var b = m.find.attr(a, "value");
-                    return null != b ? b : m.trim(m.text(a))
+                    var b = n.find.attr(a, "value");
+                    return null != b ? b : n.trim(n.text(a)).replace(sb, " ")
                 }
             },
             select: {
                 get: function(a) {
                     for (var b, c, d = a.options, e = a.selectedIndex, f = "select-one" === a.type || 0 > e, g = f ? null : [], h = f ? e + 1 : d.length, i = 0 > e ? h : f ? e : 0; h > i; i++)
-                        if (c = d[i], !(!c.selected && i !== e || (k.optDisabled ? c.disabled : null !== c.getAttribute("disabled")) || c.parentNode.disabled && m.nodeName(c.parentNode, "optgroup"))) {
-                            if (b = m(c).val(), f) return b;
+                        if (c = d[i], (c.selected || i === e) && (l.optDisabled ? !c.disabled : null === c.getAttribute("disabled")) && (!c.parentNode.disabled || !n.nodeName(c.parentNode, "optgroup"))) {
+                            if (b = n(c).val(), f) return b;
                             g.push(b)
                         } return g
                 },
                 set: function(a, b) {
                     var c, d, e = a.options,
-                        f = m.makeArray(b),
+                        f = n.makeArray(b),
                         g = e.length;
                     while (g--)
-                        if (d = e[g], m.inArray(m.valHooks.option.get(d), f) >= 0) try {
+                        if (d = e[g], n.inArray(n.valHooks.option.get(d), f) > -1) try {
                             d.selected = c = !0
                         } catch (h) {
                             d.scrollHeight
                         } else d.selected = !1;
                     return c || (a.selectedIndex = -1), e
                 }
             }
         }
-    }), m.each(["radio", "checkbox"], function() {
-        m.valHooks[this] = {
+    }), n.each(["radio", "checkbox"], function() {
+        n.valHooks[this] = {
             set: function(a, b) {
-                return m.isArray(b) ? a.checked = m.inArray(m(a).val(), b) >= 0 : void 0
+                return n.isArray(b) ? a.checked = n.inArray(n(a).val(), b) > -1 : void 0
             }
-        }, k.checkOn || (m.valHooks[this].get = function(a) {
+        }, l.checkOn || (n.valHooks[this].get = function(a) {
             return null === a.getAttribute("value") ? "on" : a.value
         })
     });
-    var mb, nb, ob = m.expr.attrHandle,
-        pb = /^(?:checked|selected)$/i,
-        qb = k.getSetAttribute,
-        rb = k.input;
-    m.fn.extend({
+    var tb, ub, vb = n.expr.attrHandle,
+        wb = /^(?:checked|selected)$/i,
+        xb = l.getSetAttribute,
+        yb = l.input;
+    n.fn.extend({
         attr: function(a, b) {
-            return V(this, m.attr, a, b, arguments.length > 1)
+            return Y(this, n.attr, a, b, arguments.length > 1)
         },
         removeAttr: function(a) {
             return this.each(function() {
-                m.removeAttr(this, a)
+                n.removeAttr(this, a)
             })
         }
-    }), m.extend({
+    }), n.extend({
         attr: function(a, b, c) {
             var d, e, f = a.nodeType;
-            if (a && 3 !== f && 8 !== f && 2 !== f) return typeof a.getAttribute === K ? m.prop(a, b, c) : (1 === f && m.isXMLDoc(a) || (b = b.toLowerCase(), d = m.attrHooks[b] || (m.expr.match.bool.test(b) ? nb : mb)), void 0 === c ? d && "get" in d && null !== (e = d.get(a, b)) ? e : (e = m.find.attr(a, b), null == e ? void 0 : e) : null !== c ? d && "set" in d && void 0 !== (e = d.set(a, c, b)) ? e : (a.setAttribute(b, c + ""), c) : void m.removeAttr(a, b))
-        },
-        removeAttr: function(a, b) {
-            var c, d, e = 0,
-                f = b && b.match(E);
-            if (f && 1 === a.nodeType)
-                while (c = f[e++]) d = m.propFix[c] || c, m.expr.match.bool.test(c) ? rb && qb || !pb.test(c) ? a[d] = !1 : a[m.camelCase("default-" + c)] = a[d] = !1 : m.attr(a, c, ""), a.removeAttribute(qb ? c : d)
+            if (3 !== f && 8 !== f && 2 !== f) return "undefined" == typeof a.getAttribute ? n.prop(a, b, c) : (1 === f && n.isXMLDoc(a) || (b = b.toLowerCase(), e = n.attrHooks[b] || (n.expr.match.bool.test(b) ? ub : tb)), void 0 !== c ? null === c ? void n.removeAttr(a, b) : e && "set" in e && void 0 !== (d = e.set(a, c, b)) ? d : (a.setAttribute(b, c + ""), c) : e && "get" in e && null !== (d = e.get(a, b)) ? d : (d = n.find.attr(a, b), null == d ? void 0 : d))
         },
         attrHooks: {
             type: {
                 set: function(a, b) {
-                    if (!k.radioValue && "radio" === b && m.nodeName(a, "input")) {
+                    if (!l.radioValue && "radio" === b && n.nodeName(a, "input")) {
                         var c = a.value;
                         return a.setAttribute("type", b), c && (a.value = c), b
                     }
                 }
             }
+        },
+        removeAttr: function(a, b) {
+            var c, d, e = 0,
+                f = b && b.match(G);
+            if (f && 1 === a.nodeType)
+                while (c = f[e++]) d = n.propFix[c] || c, n.expr.match.bool.test(c) ? yb && xb || !wb.test(c) ? a[d] = !1 : a[n.camelCase("default-" + c)] = a[d] = !1 : n.attr(a, c, ""), a.removeAttribute(xb ? c : d)
         }
-    }), nb = {
+    }), ub = {
         set: function(a, b, c) {
-            return b === !1 ? m.removeAttr(a, c) : rb && qb || !pb.test(c) ? a.setAttribute(!qb && m.propFix[c] || c, c) : a[m.camelCase("default-" + c)] = a[c] = !0, c
+            return b === !1 ? n.removeAttr(a, c) : yb && xb || !wb.test(c) ? a.setAttribute(!xb && n.propFix[c] || c, c) : a[n.camelCase("default-" + c)] = a[c] = !0, c
         }
-    }, m.each(m.expr.match.bool.source.match(/\w+/g), function(a, b) {
-        var c = ob[b] || m.find.attr;
-        ob[b] = rb && qb || !pb.test(b) ? function(a, b, d) {
+    }, n.each(n.expr.match.bool.source.match(/\w+/g), function(a, b) {
+        var c = vb[b] || n.find.attr;
+        yb && xb || !wb.test(b) ? vb[b] = function(a, b, d) {
             var e, f;
-            return d || (f = ob[b], ob[b] = e, e = null != c(a, b, d) ? b.toLowerCase() : null, ob[b] = f), e
-        } : function(a, b, c) {
-            return c ? void 0 : a[m.camelCase("default-" + b)] ? b.toLowerCase() : null
+            return d || (f = vb[b], vb[b] = e, e = null != c(a, b, d) ? b.toLowerCase() : null, vb[b] = f), e
+        } : vb[b] = function(a, b, c) {
+            return c ? void 0 : a[n.camelCase("default-" + b)] ? b.toLowerCase() : null
         }
-    }), rb && qb || (m.attrHooks.value = {
+    }), yb && xb || (n.attrHooks.value = {
         set: function(a, b, c) {
-            return m.nodeName(a, "input") ? void(a.defaultValue = b) : mb && mb.set(a, b, c)
+            return n.nodeName(a, "input") ? void(a.defaultValue = b) : tb && tb.set(a, b, c)
         }
-    }), qb || (mb = {
+    }), xb || (tb = {
         set: function(a, b, c) {
             var d = a.getAttributeNode(c);
             return d || a.setAttributeNode(d = a.ownerDocument.createAttribute(c)), d.value = b += "", "value" === c || b === a.getAttribute(c) ? b : void 0
         }
-    }, ob.id = ob.name = ob.coords = function(a, b, c) {
+    }, vb.id = vb.name = vb.coords = function(a, b, c) {
         var d;
         return c ? void 0 : (d = a.getAttributeNode(b)) && "" !== d.value ? d.value : null
-    }, m.valHooks.button = {
+    }, n.valHooks.button = {
         get: function(a, b) {
             var c = a.getAttributeNode(b);
             return c && c.specified ? c.value : void 0
         },
-        set: mb.set
-    }, m.attrHooks.contenteditable = {
+        set: tb.set
+    }, n.attrHooks.contenteditable = {
         set: function(a, b, c) {
-            mb.set(a, "" === b ? !1 : b, c)
+            tb.set(a, "" === b ? !1 : b, c)
         }
-    }, m.each(["width", "height"], function(a, b) {
-        m.attrHooks[b] = {
+    }, n.each(["width", "height"], function(a, b) {
+        n.attrHooks[b] = {
             set: function(a, c) {
                 return "" === c ? (a.setAttribute(b, "auto"), c) : void 0
             }
         }
-    })), k.style || (m.attrHooks.style = {
+    })), l.style || (n.attrHooks.style = {
         get: function(a) {
             return a.style.cssText || void 0
         },
         set: function(a, b) {
             return a.style.cssText = b + ""
         }
     });
-    var sb = /^(?:input|select|textarea|button|object)$/i,
-        tb = /^(?:a|area)$/i;
-    m.fn.extend({
+    var zb = /^(?:input|select|textarea|button|object)$/i,
+        Ab = /^(?:a|area)$/i;
+    n.fn.extend({
         prop: function(a, b) {
-            return V(this, m.prop, a, b, arguments.length > 1)
+            return Y(this, n.prop, a, b, arguments.length > 1)
         },
         removeProp: function(a) {
-            return a = m.propFix[a] || a, this.each(function() {
+            return a = n.propFix[a] || a, this.each(function() {
                 try {
                     this[a] = void 0, delete this[a]
                 } catch (b) {}
             })
         }
-    }), m.extend({
-        propFix: {
-            "for": "htmlFor",
-            "class": "className"
-        },
+    }), n.extend({
         prop: function(a, b, c) {
-            var d, e, f, g = a.nodeType;
-            if (a && 3 !== g && 8 !== g && 2 !== g) return f = 1 !== g || !m.isXMLDoc(a), f && (b = m.propFix[b] || b, e = m.propHooks[b]), void 0 !== c ? e && "set" in e && void 0 !== (d = e.set(a, c, b)) ? d : a[b] = c : e && "get" in e && null !== (d = e.get(a, b)) ? d : a[b]
+            var d, e, f = a.nodeType;
+            if (3 !== f && 8 !== f && 2 !== f) return 1 === f && n.isXMLDoc(a) || (b = n.propFix[b] || b, e = n.propHooks[b]), void 0 !== c ? e && "set" in e && void 0 !== (d = e.set(a, c, b)) ? d : a[b] = c : e && "get" in e && null !== (d = e.get(a, b)) ? d : a[b]
         },
         propHooks: {
             tabIndex: {
                 get: function(a) {
-                    var b = m.find.attr(a, "tabindex");
-                    return b ? parseInt(b, 10) : sb.test(a.nodeName) || tb.test(a.nodeName) && a.href ? 0 : -1
+                    var b = n.find.attr(a, "tabindex");
+                    return b ? parseInt(b, 10) : zb.test(a.nodeName) || Ab.test(a.nodeName) && a.href ? 0 : -1
                 }
             }
+        },
+        propFix: {
+            "for": "htmlFor",
+            "class": "className"
         }
-    }), k.hrefNormalized || m.each(["href", "src"], function(a, b) {
-        m.propHooks[b] = {
+    }), l.hrefNormalized || n.each(["href", "src"], function(a, b) {
+        n.propHooks[b] = {
             get: function(a) {
                 return a.getAttribute(b, 4)
             }
         }
-    }), k.optSelected || (m.propHooks.selected = {
+    }), l.optSelected || (n.propHooks.selected = {
         get: function(a) {
             var b = a.parentNode;
             return b && (b.selectedIndex, b.parentNode && b.parentNode.selectedIndex), null
+        },
+        set: function(a) {
+            var b = a.parentNode;
+            b && (b.selectedIndex, b.parentNode && b.parentNode.selectedIndex)
         }
-    }), m.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
-        m.propFix[this.toLowerCase()] = this
-    }), k.enctype || (m.propFix.enctype = "encoding");
-    var ub = /[\t\r\n\f]/g;
-    m.fn.extend({
+    }), n.each(["tabIndex", "readOnly", "maxLength", "cellSpacing", "cellPadding", "rowSpan", "colSpan", "useMap", "frameBorder", "contentEditable"], function() {
+        n.propFix[this.toLowerCase()] = this
+    }), l.enctype || (n.propFix.enctype = "encoding");
+    var Bb = /[\t\r\n\f]/g;
+
+    function Cb(a) {
+        return n.attr(a, "class") || ""
+    }
+    n.fn.extend({
         addClass: function(a) {
-            var b, c, d, e, f, g, h = 0,
-                i = this.length,
-                j = "string" == typeof a && a;
-            if (m.isFunction(a)) return this.each(function(b) {
-                m(this).addClass(a.call(this, b, this.className))
+            var b, c, d, e, f, g, h, i = 0;
+            if (n.isFunction(a)) return this.each(function(b) {
+                n(this).addClass(a.call(this, b, Cb(this)))
             });
-            if (j)
-                for (b = (a || "").match(E) || []; i > h; h++)
-                    if (c = this[h], d = 1 === c.nodeType && (c.className ? (" " + c.className + " ").replace(ub, " ") : " ")) {
-                        f = 0;
-                        while (e = b[f++]) d.indexOf(" " + e + " ") < 0 && (d += e + " ");
-                        g = m.trim(d), c.className !== g && (c.className = g)
-                    } return this
+            if ("string" == typeof a && a) {
+                b = a.match(G) || [];
+                while (c = this[i++])
+                    if (e = Cb(c), d = 1 === c.nodeType && (" " + e + " ").replace(Bb, " ")) {
+                        g = 0;
+                        while (f = b[g++]) d.indexOf(" " + f + " ") < 0 && (d += f + " ");
+                        h = n.trim(d), e !== h && n.attr(c, "class", h)
+                    }
+            }
+            return this
         },
         removeClass: function(a) {
-            var b, c, d, e, f, g, h = 0,
-                i = this.length,
-                j = 0 === arguments.length || "string" == typeof a && a;
-            if (m.isFunction(a)) return this.each(function(b) {
-                m(this).removeClass(a.call(this, b, this.className))
+            var b, c, d, e, f, g, h, i = 0;
+            if (n.isFunction(a)) return this.each(function(b) {
+                n(this).removeClass(a.call(this, b, Cb(this)))
             });
-            if (j)
-                for (b = (a || "").match(E) || []; i > h; h++)
-                    if (c = this[h], d = 1 === c.nodeType && (c.className ? (" " + c.className + " ").replace(ub, " ") : "")) {
-                        f = 0;
-                        while (e = b[f++])
-                            while (d.indexOf(" " + e + " ") >= 0) d = d.replace(" " + e + " ", " ");
-                        g = a ? m.trim(d) : "", c.className !== g && (c.className = g)
-                    } return this
+            if (!arguments.length) return this.attr("class", "");
+            if ("string" == typeof a && a) {
+                b = a.match(G) || [];
+                while (c = this[i++])
+                    if (e = Cb(c), d = 1 === c.nodeType && (" " + e + " ").replace(Bb, " ")) {
+                        g = 0;
+                        while (f = b[g++])
+                            while (d.indexOf(" " + f + " ") > -1) d = d.replace(" " + f + " ", " ");
+                        h = n.trim(d), e !== h && n.attr(c, "class", h)
+                    }
+            }
+            return this
         },
         toggleClass: function(a, b) {
             var c = typeof a;
-            return "boolean" == typeof b && "string" === c ? b ? this.addClass(a) : this.removeClass(a) : this.each(m.isFunction(a) ? function(c) {
-                m(this).toggleClass(a.call(this, c, this.className, b), b)
-            } : function() {
+            return "boolean" == typeof b && "string" === c ? b ? this.addClass(a) : this.removeClass(a) : n.isFunction(a) ? this.each(function(c) {
+                n(this).toggleClass(a.call(this, c, Cb(this), b), b)
+            }) : this.each(function() {
+                var b, d, e, f;
                 if ("string" === c) {
-                    var b, d = 0,
-                        e = m(this),
-                        f = a.match(E) || [];
+                    d = 0, e = n(this), f = a.match(G) || [];
                     while (b = f[d++]) e.hasClass(b) ? e.removeClass(b) : e.addClass(b)
-                } else(c === K || "boolean" === c) && (this.className && m._data(this, "__className__", this.className), this.className = this.className || a === !1 ? "" : m._data(this, "__className__") || "")
+                } else void 0 !== a && "boolean" !== c || (b = Cb(this), b && n._data(this, "__className__", b), n.attr(this, "class", b || a === !1 ? "" : n._data(this, "__className__") || ""))
             })
         },
         hasClass: function(a) {
-            for (var b = " " + a + " ", c = 0, d = this.length; d > c; c++)
-                if (1 === this[c].nodeType && (" " + this[c].className + " ").replace(ub, " ").indexOf(b) >= 0) return !0;
+            var b, c, d = 0;
+            b = " " + a + " ";
+            while (c = this[d++])
+                if (1 === c.nodeType && (" " + Cb(c) + " ").replace(Bb, " ").indexOf(b) > -1) return !0;
             return !1
         }
-    }), m.each("blur focus focusin focusout load resize scroll unload click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup error contextmenu".split(" "), function(a, b) {
-        m.fn[b] = function(a, c) {
+    }), n.each("blur focus focusin focusout load resize scroll unload click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup error contextmenu".split(" "), function(a, b) {
+        n.fn[b] = function(a, c) {
             return arguments.length > 0 ? this.on(b, null, a, c) : this.trigger(b)
         }
-    }), m.fn.extend({
+    }), n.fn.extend({
         hover: function(a, b) {
             return this.mouseenter(a).mouseleave(b || a)
-        },
-        bind: function(a, b, c) {
-            return this.on(a, null, b, c)
-        },
-        unbind: function(a, b) {
-            return this.off(a, null, b)
-        },
-        delegate: function(a, b, c, d) {
-            return this.on(b, a, c, d)
-        },
-        undelegate: function(a, b, c) {
-            return 1 === arguments.length ? this.off(a, "**") : this.off(b, a || "**", c)
         }
     });
-    var vb = m.now(),
-        wb = /\?/,
-        xb = /(,)|(\[|{)|(}|])|"(?:[^"\\\r\n]|\\["\\\/bfnrt]|\\u[\da-fA-F]{4})*"\s*:?|true|false|null|-?(?!0\d)\d+(?:\.\d+|)(?:[eE][+-]?\d+|)/g;
-    m.parseJSON = function(b) {
+    var Db = a.location,
+        Eb = n.now(),
+        Fb = /\?/,
+        Gb = /(,)|(\[|{)|(}|])|"(?:[^"\\\r\n]|\\["\\\/bfnrt]|\\u[\da-fA-F]{4})*"\s*:?|true|false|null|-?(?!0\d)\d+(?:\.\d+|)(?:[eE][+-]?\d+|)/g;
+    n.parseJSON = function(b) {
         if (a.JSON && a.JSON.parse) return a.JSON.parse(b + "");
         var c, d = null,
-            e = m.trim(b + "");
-        return e && !m.trim(e.replace(xb, function(a, b, e, f) {
+            e = n.trim(b + "");
+        return e && !n.trim(e.replace(Gb, function(a, b, e, f) {
             return c && b && (d = 0), 0 === d ? a : (c = e || b, d += !f - !e, "")
-        })) ? Function("return " + e)() : m.error("Invalid JSON: " + b)
-    }, m.parseXML = function(b) {
+        })) ? Function("return " + e)() : n.error("Invalid JSON: " + b)
+    }, n.parseXML = function(b) {
         var c, d;
         if (!b || "string" != typeof b) return null;
         try {
-            a.DOMParser ? (d = new DOMParser, c = d.parseFromString(b, "text/xml")) : (c = new ActiveXObject("Microsoft.XMLDOM"), c.async = "false", c.loadXML(b))
+            a.DOMParser ? (d = new a.DOMParser, c = d.parseFromString(b, "text/xml")) : (c = new a.ActiveXObject("Microsoft.XMLDOM"), c.async = "false", c.loadXML(b))
         } catch (e) {
             c = void 0
         }
-        return c && c.documentElement && !c.getElementsByTagName("parsererror").length || m.error("Invalid XML: " + b), c
+        return c && c.documentElement && !c.getElementsByTagName("parsererror").length || n.error("Invalid XML: " + b), c
     };
-    var yb, zb, Ab = /#.*$/,
-        Bb = /([?&])_=[^&]*/,
-        Cb = /^(.*?):[ \t]*([^\r\n]*)\r?$/gm,
-        Db = /^(?:about|app|app-storage|.+-extension|file|res|widget):$/,
-        Eb = /^(?:GET|HEAD)$/,
-        Fb = /^\/\//,
-        Gb = /^([\w.+-]+:)(?:\/\/(?:[^\/?#]*@|)([^\/?#:]*)(?::(\d+)|)|)/,
-        Hb = {},
-        Ib = {},
-        Jb = "*/".concat("*");
-    try {
-        zb = location.href
-    } catch (Kb) {
-        zb = y.createElement("a"), zb.href = "", zb = zb.href
-    }
-    yb = Gb.exec(zb.toLowerCase()) || [];
+    var Hb = /#.*$/,
+        Ib = /([?&])_=[^&]*/,
+        Jb = /^(.*?):[ \t]*([^\r\n]*)\r?$/gm,
+        Kb = /^(?:about|app|app-storage|.+-extension|file|res|widget):$/,
+        Lb = /^(?:GET|HEAD)$/,
+        Mb = /^\/\//,
+        Nb = /^([\w.+-]+:)(?:\/\/(?:[^\/?#]*@|)([^\/?#:]*)(?::(\d+)|)|)/,
+        Ob = {},
+        Pb = {},
+        Qb = "*/".concat("*"),
+        Rb = Db.href,
+        Sb = Nb.exec(Rb.toLowerCase()) || [];
 
-    function Lb(a) {
+    function Tb(a) {
         return function(b, c) {
             "string" != typeof b && (c = b, b = "*");
             var d, e = 0,
-                f = b.toLowerCase().match(E) || [];
-            if (m.isFunction(c))
+                f = b.toLowerCase().match(G) || [];
+            if (n.isFunction(c))
                 while (d = f[e++]) "+" === d.charAt(0) ? (d = d.slice(1) || "*", (a[d] = a[d] || []).unshift(c)) : (a[d] = a[d] || []).push(c)
         }
     }
 
-    function Mb(a, b, c, d) {
+    function Ub(a, b, c, d) {
         var e = {},
-            f = a === Ib;
+            f = a === Pb;
 
         function g(h) {
             var i;
-            return e[h] = !0, m.each(a[h] || [], function(a, h) {
+            return e[h] = !0, n.each(a[h] || [], function(a, h) {
                 var j = h(b, c, d);
                 return "string" != typeof j || f || e[j] ? f ? !(i = j) : void 0 : (b.dataTypes.unshift(j), g(j), !1)
             }), i
         }
         return g(b.dataTypes[0]) || !e["*"] && g("*")
     }
 
-    function Nb(a, b) {
-        var c, d, e = m.ajaxSettings.flatOptions || {};
+    function Vb(a, b) {
+        var c, d, e = n.ajaxSettings.flatOptions || {};
         for (d in b) void 0 !== b[d] && ((e[d] ? a : c || (c = {}))[d] = b[d]);
-        return c && m.extend(!0, a, c), a
+        return c && n.extend(!0, a, c), a
     }
 
-    function Ob(a, b, c) {
+    function Wb(a, b, c) {
         var d, e, f, g, h = a.contents,
             i = a.dataTypes;
         while ("*" === i[0]) i.shift(), void 0 === e && (e = a.mimeType || b.getResponseHeader("Content-Type"));
         if (e)
             for (g in h)
                 if (h[g] && h[g].test(e)) {
                     i.unshift(g);
@@ -2843,15 +2862,15 @@
                 d || (d = g)
             }
             f = f || d
         }
         return f ? (f !== i[0] && i.unshift(f), c[f]) : void 0
     }
 
-    function Pb(a, b, c, d) {
+    function Xb(a, b, c, d) {
         var e, f, g, h, i, j = {},
             k = a.dataTypes.slice();
         if (k[1])
             for (g in a.converters) j[g.toLowerCase()] = a.converters[g];
         f = k.shift();
         while (f)
             if (a.responseFields[f] && (c[a.responseFields[f]] = b), !i && d && a.dataFilter && (b = a.dataFilter(b, a.dataType)), i = f, f = k.shift())
@@ -2874,464 +2893,494 @@
                 }
         }
         return {
             state: "success",
             data: b
         }
     }
-    m.extend({
+    n.extend({
         active: 0,
         lastModified: {},
         etag: {},
         ajaxSettings: {
-            url: zb,
+            url: Rb,
             type: "GET",
-            isLocal: Db.test(yb[1]),
+            isLocal: Kb.test(Sb[1]),
             global: !0,
             processData: !0,
             async: !0,
             contentType: "application/x-www-form-urlencoded; charset=UTF-8",
             accepts: {
-                "*": Jb,
+                "*": Qb,
                 text: "text/plain",
                 html: "text/html",
                 xml: "application/xml, text/xml",
                 json: "application/json, text/javascript"
             },
             contents: {
-                xml: /xml/,
-                html: /html/,
-                json: /json/
+                xml: /\bxml\b/,
+                html: /\bhtml/,
+                json: /\bjson\b/
             },
             responseFields: {
                 xml: "responseXML",
                 text: "responseText",
                 json: "responseJSON"
             },
             converters: {
                 "* text": String,
                 "text html": !0,
-                "text json": m.parseJSON,
-                "text xml": m.parseXML
+                "text json": n.parseJSON,
+                "text xml": n.parseXML
             },
             flatOptions: {
                 url: !0,
                 context: !0
             }
         },
         ajaxSetup: function(a, b) {
-            return b ? Nb(Nb(a, m.ajaxSettings), b) : Nb(m.ajaxSettings, a)
+            return b ? Vb(Vb(a, n.ajaxSettings), b) : Vb(n.ajaxSettings, a)
         },
-        ajaxPrefilter: Lb(Hb),
-        ajaxTransport: Lb(Ib),
-        ajax: function(a, b) {
-            "object" == typeof a && (b = a, a = void 0), b = b || {};
-            var c, d, e, f, g, h, i, j, k = m.ajaxSetup({}, b),
-                l = k.context || k,
-                n = k.context && (l.nodeType || l.jquery) ? m(l) : m.event,
-                o = m.Deferred(),
-                p = m.Callbacks("once memory"),
-                q = k.statusCode || {},
-                r = {},
+        ajaxPrefilter: Tb(Ob),
+        ajaxTransport: Tb(Pb),
+        ajax: function(b, c) {
+            "object" == typeof b && (c = b, b = void 0), c = c || {};
+            var d, e, f, g, h, i, j, k, l = n.ajaxSetup({}, c),
+                m = l.context || l,
+                o = l.context && (m.nodeType || m.jquery) ? n(m) : n.event,
+                p = n.Deferred(),
+                q = n.Callbacks("once memory"),
+                r = l.statusCode || {},
                 s = {},
-                t = 0,
-                u = "canceled",
-                v = {
+                t = {},
+                u = 0,
+                v = "canceled",
+                w = {
                     readyState: 0,
                     getResponseHeader: function(a) {
                         var b;
-                        if (2 === t) {
-                            if (!j) {
-                                j = {};
-                                while (b = Cb.exec(f)) j[b[1].toLowerCase()] = b[2]
+                        if (2 === u) {
+                            if (!k) {
+                                k = {};
+                                while (b = Jb.exec(g)) k[b[1].toLowerCase()] = b[2]
                             }
-                            b = j[a.toLowerCase()]
+                            b = k[a.toLowerCase()]
                         }
                         return null == b ? null : b
                     },
                     getAllResponseHeaders: function() {
-                        return 2 === t ? f : null
+                        return 2 === u ? g : null
                     },
                     setRequestHeader: function(a, b) {
                         var c = a.toLowerCase();
-                        return t || (a = s[c] = s[c] || a, r[a] = b), this
+                        return u || (a = t[c] = t[c] || a, s[a] = b), this
                     },
                     overrideMimeType: function(a) {
-                        return t || (k.mimeType = a), this
+                        return u || (l.mimeType = a), this
                     },
                     statusCode: function(a) {
                         var b;
                         if (a)
-                            if (2 > t)
-                                for (b in a) q[b] = [q[b], a[b]];
-                            else v.always(a[v.status]);
+                            if (2 > u)
+                                for (b in a) r[b] = [r[b], a[b]];
+                            else w.always(a[w.status]);
                         return this
                     },
                     abort: function(a) {
-                        var b = a || u;
-                        return i && i.abort(b), x(0, b), this
+                        var b = a || v;
+                        return j && j.abort(b), y(0, b), this
                     }
                 };
-            if (o.promise(v).complete = p.add, v.success = v.done, v.error = v.fail, k.url = ((a || k.url || zb) + "").replace(Ab, "").replace(Fb, yb[1] + "//"), k.type = b.method || b.type || k.method || k.type, k.dataTypes = m.trim(k.dataType || "*").toLowerCase().match(E) || [""], null == k.crossDomain && (c = Gb.exec(k.url.toLowerCase()), k.crossDomain = !(!c || c[1] === yb[1] && c[2] === yb[2] && (c[3] || ("http:" === c[1] ? "80" : "443")) === (yb[3] || ("http:" === yb[1] ? "80" : "443")))), k.data && k.processData && "string" != typeof k.data && (k.data = m.param(k.data, k.traditional)), Mb(Hb, k, b, v), 2 === t) return v;
-            h = m.event && k.global, h && 0 === m.active++ && m.event.trigger("ajaxStart"), k.type = k.type.toUpperCase(), k.hasContent = !Eb.test(k.type), e = k.url, k.hasContent || (k.data && (e = k.url += (wb.test(e) ? "&" : "?") + k.data, delete k.data), k.cache === !1 && (k.url = Bb.test(e) ? e.replace(Bb, "$1_=" + vb++) : e + (wb.test(e) ? "&" : "?") + "_=" + vb++)), k.ifModified && (m.lastModified[e] && v.setRequestHeader("If-Modified-Since", m.lastModified[e]), m.etag[e] && v.setRequestHeader("If-None-Match", m.etag[e])), (k.data && k.hasContent && k.contentType !== !1 || b.contentType) && v.setRequestHeader("Content-Type", k.contentType), v.setRequestHeader("Accept", k.dataTypes[0] && k.accepts[k.dataTypes[0]] ? k.accepts[k.dataTypes[0]] + ("*" !== k.dataTypes[0] ? ", " + Jb + "; q=0.01" : "") : k.accepts["*"]);
-            for (d in k.headers) v.setRequestHeader(d, k.headers[d]);
-            if (k.beforeSend && (k.beforeSend.call(l, v, k) === !1 || 2 === t)) return v.abort();
-            u = "abort";
-            for (d in {
+            if (p.promise(w).complete = q.add, w.success = w.done, w.error = w.fail, l.url = ((b || l.url || Rb) + "").replace(Hb, "").replace(Mb, Sb[1] + "//"), l.type = c.method || c.type || l.method || l.type, l.dataTypes = n.trim(l.dataType || "*").toLowerCase().match(G) || [""], null == l.crossDomain && (d = Nb.exec(l.url.toLowerCase()), l.crossDomain = !(!d || d[1] === Sb[1] && d[2] === Sb[2] && (d[3] || ("http:" === d[1] ? "80" : "443")) === (Sb[3] || ("http:" === Sb[1] ? "80" : "443")))), l.data && l.processData && "string" != typeof l.data && (l.data = n.param(l.data, l.traditional)), Ub(Ob, l, c, w), 2 === u) return w;
+            i = n.event && l.global, i && 0 === n.active++ && n.event.trigger("ajaxStart"), l.type = l.type.toUpperCase(), l.hasContent = !Lb.test(l.type), f = l.url, l.hasContent || (l.data && (f = l.url += (Fb.test(f) ? "&" : "?") + l.data, delete l.data), l.cache === !1 && (l.url = Ib.test(f) ? f.replace(Ib, "$1_=" + Eb++) : f + (Fb.test(f) ? "&" : "?") + "_=" + Eb++)), l.ifModified && (n.lastModified[f] && w.setRequestHeader("If-Modified-Since", n.lastModified[f]), n.etag[f] && w.setRequestHeader("If-None-Match", n.etag[f])), (l.data && l.hasContent && l.contentType !== !1 || c.contentType) && w.setRequestHeader("Content-Type", l.contentType), w.setRequestHeader("Accept", l.dataTypes[0] && l.accepts[l.dataTypes[0]] ? l.accepts[l.dataTypes[0]] + ("*" !== l.dataTypes[0] ? ", " + Qb + "; q=0.01" : "") : l.accepts["*"]);
+            for (e in l.headers) w.setRequestHeader(e, l.headers[e]);
+            if (l.beforeSend && (l.beforeSend.call(m, w, l) === !1 || 2 === u)) return w.abort();
+            v = "abort";
+            for (e in {
                     success: 1,
                     error: 1,
                     complete: 1
-                }) v[d](k[d]);
-            if (i = Mb(Ib, k, b, v)) {
-                v.readyState = 1, h && n.trigger("ajaxSend", [v, k]), k.async && k.timeout > 0 && (g = setTimeout(function() {
-                    v.abort("timeout")
-                }, k.timeout));
+                }) w[e](l[e]);
+            if (j = Ub(Pb, l, c, w)) {
+                if (w.readyState = 1, i && o.trigger("ajaxSend", [w, l]), 2 === u) return w;
+                l.async && l.timeout > 0 && (h = a.setTimeout(function() {
+                    w.abort("timeout")
+                }, l.timeout));
                 try {
-                    t = 1, i.send(r, x)
-                } catch (w) {
-                    if (!(2 > t)) throw w;
-                    x(-1, w)
-                }
-            } else x(-1, "No Transport");
-
-            function x(a, b, c, d) {
-                var j, r, s, u, w, x = b;
-                2 !== t && (t = 2, g && clearTimeout(g), i = void 0, f = d || "", v.readyState = a > 0 ? 4 : 0, j = a >= 200 && 300 > a || 304 === a, c && (u = Ob(k, v, c)), u = Pb(k, u, v, j), j ? (k.ifModified && (w = v.getResponseHeader("Last-Modified"), w && (m.lastModified[e] = w), w = v.getResponseHeader("etag"), w && (m.etag[e] = w)), 204 === a || "HEAD" === k.type ? x = "nocontent" : 304 === a ? x = "notmodified" : (x = u.state, r = u.data, s = u.error, j = !s)) : (s = x, (a || !x) && (x = "error", 0 > a && (a = 0))), v.status = a, v.statusText = (b || x) + "", j ? o.resolveWith(l, [r, x, v]) : o.rejectWith(l, [v, x, s]), v.statusCode(q), q = void 0, h && n.trigger(j ? "ajaxSuccess" : "ajaxError", [v, k, j ? r : s]), p.fireWith(l, [v, x]), h && (n.trigger("ajaxComplete", [v, k]), --m.active || m.event.trigger("ajaxStop")))
+                    u = 1, j.send(s, y)
+                } catch (x) {
+                    if (!(2 > u)) throw x;
+                    y(-1, x)
+                }
+            } else y(-1, "No Transport");
+
+            function y(b, c, d, e) {
+                var k, s, t, v, x, y = c;
+                2 !== u && (u = 2, h && a.clearTimeout(h), j = void 0, g = e || "", w.readyState = b > 0 ? 4 : 0, k = b >= 200 && 300 > b || 304 === b, d && (v = Wb(l, w, d)), v = Xb(l, v, w, k), k ? (l.ifModified && (x = w.getResponseHeader("Last-Modified"), x && (n.lastModified[f] = x), x = w.getResponseHeader("etag"), x && (n.etag[f] = x)), 204 === b || "HEAD" === l.type ? y = "nocontent" : 304 === b ? y = "notmodified" : (y = v.state, s = v.data, t = v.error, k = !t)) : (t = y, !b && y || (y = "error", 0 > b && (b = 0))), w.status = b, w.statusText = (c || y) + "", k ? p.resolveWith(m, [s, y, w]) : p.rejectWith(m, [w, y, t]), w.statusCode(r), r = void 0, i && o.trigger(k ? "ajaxSuccess" : "ajaxError", [w, l, k ? s : t]), q.fireWith(m, [w, y]), i && (o.trigger("ajaxComplete", [w, l]), --n.active || n.event.trigger("ajaxStop")))
             }
-            return v
+            return w
         },
         getJSON: function(a, b, c) {
-            return m.get(a, b, c, "json")
+            return n.get(a, b, c, "json")
         },
         getScript: function(a, b) {
-            return m.get(a, void 0, b, "script")
+            return n.get(a, void 0, b, "script")
         }
-    }), m.each(["get", "post"], function(a, b) {
-        m[b] = function(a, c, d, e) {
-            return m.isFunction(c) && (e = e || d, d = c, c = void 0), m.ajax({
+    }), n.each(["get", "post"], function(a, b) {
+        n[b] = function(a, c, d, e) {
+            return n.isFunction(c) && (e = e || d, d = c, c = void 0), n.ajax(n.extend({
                 url: a,
                 type: b,
                 dataType: e,
                 data: c,
                 success: d
-            })
+            }, n.isPlainObject(a) && a))
         }
-    }), m._evalUrl = function(a) {
-        return m.ajax({
+    }), n._evalUrl = function(a) {
+        return n.ajax({
             url: a,
             type: "GET",
             dataType: "script",
+            cache: !0,
             async: !1,
             global: !1,
             "throws": !0
         })
-    }, m.fn.extend({
+    }, n.fn.extend({
         wrapAll: function(a) {
-            if (m.isFunction(a)) return this.each(function(b) {
-                m(this).wrapAll(a.call(this, b))
+            if (n.isFunction(a)) return this.each(function(b) {
+                n(this).wrapAll(a.call(this, b))
             });
             if (this[0]) {
-                var b = m(a, this[0].ownerDocument).eq(0).clone(!0);
+                var b = n(a, this[0].ownerDocument).eq(0).clone(!0);
                 this[0].parentNode && b.insertBefore(this[0]), b.map(function() {
                     var a = this;
                     while (a.firstChild && 1 === a.firstChild.nodeType) a = a.firstChild;
                     return a
                 }).append(this)
             }
             return this
         },
         wrapInner: function(a) {
-            return this.each(m.isFunction(a) ? function(b) {
-                m(this).wrapInner(a.call(this, b))
-            } : function() {
-                var b = m(this),
+            return n.isFunction(a) ? this.each(function(b) {
+                n(this).wrapInner(a.call(this, b))
+            }) : this.each(function() {
+                var b = n(this),
                     c = b.contents();
                 c.length ? c.wrapAll(a) : b.append(a)
             })
         },
         wrap: function(a) {
-            var b = m.isFunction(a);
+            var b = n.isFunction(a);
             return this.each(function(c) {
-                m(this).wrapAll(b ? a.call(this, c) : a)
+                n(this).wrapAll(b ? a.call(this, c) : a)
             })
         },
         unwrap: function() {
             return this.parent().each(function() {
-                m.nodeName(this, "body") || m(this).replaceWith(this.childNodes)
+                n.nodeName(this, "body") || n(this).replaceWith(this.childNodes)
             }).end()
         }
-    }), m.expr.filters.hidden = function(a) {
-        return a.offsetWidth <= 0 && a.offsetHeight <= 0 || !k.reliableHiddenOffsets() && "none" === (a.style && a.style.display || m.css(a, "display"))
-    }, m.expr.filters.visible = function(a) {
-        return !m.expr.filters.hidden(a)
+    });
+
+    function Yb(a) {
+        return a.style && a.style.display || n.css(a, "display")
+    }
+
+    function Zb(a) {
+        if (!n.contains(a.ownerDocument || d, a)) return !0;
+        while (a && 1 === a.nodeType) {
+            if ("none" === Yb(a) || "hidden" === a.type) return !0;
+            a = a.parentNode
+        }
+        return !1
+    }
+    n.expr.filters.hidden = function(a) {
+        return l.reliableHiddenOffsets() ? a.offsetWidth <= 0 && a.offsetHeight <= 0 && !a.getClientRects().length : Zb(a)
+    }, n.expr.filters.visible = function(a) {
+        return !n.expr.filters.hidden(a)
     };
-    var Qb = /%20/g,
-        Rb = /\[\]$/,
-        Sb = /\r?\n/g,
-        Tb = /^(?:submit|button|image|reset|file)$/i,
-        Ub = /^(?:input|select|textarea|keygen)/i;
+    var $b = /%20/g,
+        _b = /\[\]$/,
+        ac = /\r?\n/g,
+        bc = /^(?:submit|button|image|reset|file)$/i,
+        cc = /^(?:input|select|textarea|keygen)/i;
 
-    function Vb(a, b, c, d) {
+    function dc(a, b, c, d) {
         var e;
-        if (m.isArray(b)) m.each(b, function(b, e) {
-            c || Rb.test(a) ? d(a, e) : Vb(a + "[" + ("object" == typeof e ? b : "") + "]", e, c, d)
+        if (n.isArray(b)) n.each(b, function(b, e) {
+            c || _b.test(a) ? d(a, e) : dc(a + "[" + ("object" == typeof e && null != e ? b : "") + "]", e, c, d)
         });
-        else if (c || "object" !== m.type(b)) d(a, b);
+        else if (c || "object" !== n.type(b)) d(a, b);
         else
-            for (e in b) Vb(a + "[" + e + "]", b[e], c, d)
+            for (e in b) dc(a + "[" + e + "]", b[e], c, d)
     }
-    m.param = function(a, b) {
+    n.param = function(a, b) {
         var c, d = [],
             e = function(a, b) {
-                b = m.isFunction(b) ? b() : null == b ? "" : b, d[d.length] = encodeURIComponent(a) + "=" + encodeURIComponent(b)
+                b = n.isFunction(b) ? b() : null == b ? "" : b, d[d.length] = encodeURIComponent(a) + "=" + encodeURIComponent(b)
             };
-        if (void 0 === b && (b = m.ajaxSettings && m.ajaxSettings.traditional), m.isArray(a) || a.jquery && !m.isPlainObject(a)) m.each(a, function() {
+        if (void 0 === b && (b = n.ajaxSettings && n.ajaxSettings.traditional), n.isArray(a) || a.jquery && !n.isPlainObject(a)) n.each(a, function() {
             e(this.name, this.value)
         });
         else
-            for (c in a) Vb(c, a[c], b, e);
-        return d.join("&").replace(Qb, "+")
-    }, m.fn.extend({
+            for (c in a) dc(c, a[c], b, e);
+        return d.join("&").replace($b, "+")
+    }, n.fn.extend({
         serialize: function() {
-            return m.param(this.serializeArray())
+            return n.param(this.serializeArray())
         },
         serializeArray: function() {
             return this.map(function() {
-                var a = m.prop(this, "elements");
-                return a ? m.makeArray(a) : this
+                var a = n.prop(this, "elements");
+                return a ? n.makeArray(a) : this
             }).filter(function() {
                 var a = this.type;
-                return this.name && !m(this).is(":disabled") && Ub.test(this.nodeName) && !Tb.test(a) && (this.checked || !W.test(a))
+                return this.name && !n(this).is(":disabled") && cc.test(this.nodeName) && !bc.test(a) && (this.checked || !Z.test(a))
             }).map(function(a, b) {
-                var c = m(this).val();
-                return null == c ? null : m.isArray(c) ? m.map(c, function(a) {
+                var c = n(this).val();
+                return null == c ? null : n.isArray(c) ? n.map(c, function(a) {
                     return {
                         name: b.name,
-                        value: a.replace(Sb, "\r\n")
+                        value: a.replace(ac, "\r\n")
                     }
                 }) : {
                     name: b.name,
-                    value: c.replace(Sb, "\r\n")
+                    value: c.replace(ac, "\r\n")
                 }
             }).get()
         }
-    }), m.ajaxSettings.xhr = void 0 !== a.ActiveXObject ? function() {
-        return !this.isLocal && /^(get|post|head|put|delete|options)$/i.test(this.type) && Zb() || $b()
-    } : Zb;
-    var Wb = 0,
-        Xb = {},
-        Yb = m.ajaxSettings.xhr();
+    }), n.ajaxSettings.xhr = void 0 !== a.ActiveXObject ? function() {
+        return this.isLocal ? ic() : d.documentMode > 8 ? hc() : /^(get|post|head|put|delete|options)$/i.test(this.type) && hc() || ic()
+    } : hc;
+    var ec = 0,
+        fc = {},
+        gc = n.ajaxSettings.xhr();
     a.attachEvent && a.attachEvent("onunload", function() {
-        for (var a in Xb) Xb[a](void 0, !0)
-    }), k.cors = !!Yb && "withCredentials" in Yb, Yb = k.ajax = !!Yb, Yb && m.ajaxTransport(function(a) {
-        if (!a.crossDomain || k.cors) {
-            var b;
+        for (var a in fc) fc[a](void 0, !0)
+    }), l.cors = !!gc && "withCredentials" in gc, gc = l.ajax = !!gc, gc && n.ajaxTransport(function(b) {
+        if (!b.crossDomain || l.cors) {
+            var c;
             return {
-                send: function(c, d) {
-                    var e, f = a.xhr(),
-                        g = ++Wb;
-                    if (f.open(a.type, a.url, a.async, a.username, a.password), a.xhrFields)
-                        for (e in a.xhrFields) f[e] = a.xhrFields[e];
-                    a.mimeType && f.overrideMimeType && f.overrideMimeType(a.mimeType), a.crossDomain || c["X-Requested-With"] || (c["X-Requested-With"] = "XMLHttpRequest");
-                    for (e in c) void 0 !== c[e] && f.setRequestHeader(e, c[e] + "");
-                    f.send(a.hasContent && a.data || null), b = function(c, e) {
-                        var h, i, j;
-                        if (b && (e || 4 === f.readyState))
-                            if (delete Xb[g], b = void 0, f.onreadystatechange = m.noop, e) 4 !== f.readyState && f.abort();
+                send: function(d, e) {
+                    var f, g = b.xhr(),
+                        h = ++ec;
+                    if (g.open(b.type, b.url, b.async, b.username, b.password), b.xhrFields)
+                        for (f in b.xhrFields) g[f] = b.xhrFields[f];
+                    b.mimeType && g.overrideMimeType && g.overrideMimeType(b.mimeType), b.crossDomain || d["X-Requested-With"] || (d["X-Requested-With"] = "XMLHttpRequest");
+                    for (f in d) void 0 !== d[f] && g.setRequestHeader(f, d[f] + "");
+                    g.send(b.hasContent && b.data || null), c = function(a, d) {
+                        var f, i, j;
+                        if (c && (d || 4 === g.readyState))
+                            if (delete fc[h], c = void 0, g.onreadystatechange = n.noop, d) 4 !== g.readyState && g.abort();
                             else {
-                                j = {}, h = f.status, "string" == typeof f.responseText && (j.text = f.responseText);
+                                j = {}, f = g.status, "string" == typeof g.responseText && (j.text = g.responseText);
                                 try {
-                                    i = f.statusText
+                                    i = g.statusText
                                 } catch (k) {
                                     i = ""
                                 }
-                                h || !a.isLocal || a.crossDomain ? 1223 === h && (h = 204) : h = j.text ? 200 : 404
-                            } j && d(h, i, j, f.getAllResponseHeaders())
-                    }, a.async ? 4 === f.readyState ? setTimeout(b) : f.onreadystatechange = Xb[g] = b : b()
+                                f || !b.isLocal || b.crossDomain ? 1223 === f && (f = 204) : f = j.text ? 200 : 404
+                            } j && e(f, i, j, g.getAllResponseHeaders())
+                    }, b.async ? 4 === g.readyState ? a.setTimeout(c) : g.onreadystatechange = fc[h] = c : c()
                 },
                 abort: function() {
-                    b && b(void 0, !0)
+                    c && c(void 0, !0)
                 }
             }
         }
     });
 
-    function Zb() {
+    function hc() {
         try {
             return new a.XMLHttpRequest
         } catch (b) {}
     }
 
-    function $b() {
+    function ic() {
         try {
             return new a.ActiveXObject("Microsoft.XMLHTTP")
         } catch (b) {}
     }
-    m.ajaxSetup({
+    n.ajaxSetup({
         accepts: {
             script: "text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"
         },
         contents: {
-            script: /(?:java|ecma)script/
+            script: /\b(?:java|ecma)script\b/
         },
         converters: {
             "text script": function(a) {
-                return m.globalEval(a), a
+                return n.globalEval(a), a
             }
         }
-    }), m.ajaxPrefilter("script", function(a) {
+    }), n.ajaxPrefilter("script", function(a) {
         void 0 === a.cache && (a.cache = !1), a.crossDomain && (a.type = "GET", a.global = !1)
-    }), m.ajaxTransport("script", function(a) {
+    }), n.ajaxTransport("script", function(a) {
         if (a.crossDomain) {
-            var b, c = y.head || m("head")[0] || y.documentElement;
+            var b, c = d.head || n("head")[0] || d.documentElement;
             return {
-                send: function(d, e) {
-                    b = y.createElement("script"), b.async = !0, a.scriptCharset && (b.charset = a.scriptCharset), b.src = a.url, b.onload = b.onreadystatechange = function(a, c) {
-                        (c || !b.readyState || /loaded|complete/.test(b.readyState)) && (b.onload = b.onreadystatechange = null, b.parentNode && b.parentNode.removeChild(b), b = null, c || e(200, "success"))
+                send: function(e, f) {
+                    b = d.createElement("script"), b.async = !0, a.scriptCharset && (b.charset = a.scriptCharset), b.src = a.url, b.onload = b.onreadystatechange = function(a, c) {
+                        (c || !b.readyState || /loaded|complete/.test(b.readyState)) && (b.onload = b.onreadystatechange = null, b.parentNode && b.parentNode.removeChild(b), b = null, c || f(200, "success"))
                     }, c.insertBefore(b, c.firstChild)
                 },
                 abort: function() {
                     b && b.onload(void 0, !0)
                 }
             }
         }
     });
-    var _b = [],
-        ac = /(=)\?(?=&|$)|\?\?/;
-    m.ajaxSetup({
+    var jc = [],
+        kc = /(=)\?(?=&|$)|\?\?/;
+    n.ajaxSetup({
         jsonp: "callback",
         jsonpCallback: function() {
-            var a = _b.pop() || m.expando + "_" + vb++;
+            var a = jc.pop() || n.expando + "_" + Eb++;
             return this[a] = !0, a
         }
-    }), m.ajaxPrefilter("json jsonp", function(b, c, d) {
-        var e, f, g, h = b.jsonp !== !1 && (ac.test(b.url) ? "url" : "string" == typeof b.data && !(b.contentType || "").indexOf("application/x-www-form-urlencoded") && ac.test(b.data) && "data");
-        return h || "jsonp" === b.dataTypes[0] ? (e = b.jsonpCallback = m.isFunction(b.jsonpCallback) ? b.jsonpCallback() : b.jsonpCallback, h ? b[h] = b[h].replace(ac, "$1" + e) : b.jsonp !== !1 && (b.url += (wb.test(b.url) ? "&" : "?") + b.jsonp + "=" + e), b.converters["script json"] = function() {
-            return g || m.error(e + " was not called"), g[0]
+    }), n.ajaxPrefilter("json jsonp", function(b, c, d) {
+        var e, f, g, h = b.jsonp !== !1 && (kc.test(b.url) ? "url" : "string" == typeof b.data && 0 === (b.contentType || "").indexOf("application/x-www-form-urlencoded") && kc.test(b.data) && "data");
+        return h || "jsonp" === b.dataTypes[0] ? (e = b.jsonpCallback = n.isFunction(b.jsonpCallback) ? b.jsonpCallback() : b.jsonpCallback, h ? b[h] = b[h].replace(kc, "$1" + e) : b.jsonp !== !1 && (b.url += (Fb.test(b.url) ? "&" : "?") + b.jsonp + "=" + e), b.converters["script json"] = function() {
+            return g || n.error(e + " was not called"), g[0]
         }, b.dataTypes[0] = "json", f = a[e], a[e] = function() {
             g = arguments
         }, d.always(function() {
-            a[e] = f, b[e] && (b.jsonpCallback = c.jsonpCallback, _b.push(e)), g && m.isFunction(f) && f(g[0]), g = f = void 0
+            void 0 === f ? n(a).removeProp(e) : a[e] = f, b[e] && (b.jsonpCallback = c.jsonpCallback, jc.push(e)), g && n.isFunction(f) && f(g[0]), g = f = void 0
         }), "script") : void 0
-    }), m.parseHTML = function(a, b, c) {
+    }), n.parseHTML = function(a, b, c) {
         if (!a || "string" != typeof a) return null;
-        "boolean" == typeof b && (c = b, b = !1), b = b || y;
-        var d = u.exec(a),
-            e = !c && [];
-        return d ? [b.createElement(d[1])] : (d = m.buildFragment([a], b, e), e && e.length && m(e).remove(), m.merge([], d.childNodes))
+        "boolean" == typeof b && (c = b, b = !1), b = b || d;
+        var e = x.exec(a),
+            f = !c && [];
+        return e ? [b.createElement(e[1])] : (e = ja([a], b, f), f && f.length && n(f).remove(), n.merge([], e.childNodes))
     };
-    var bc = m.fn.load;
-    m.fn.load = function(a, b, c) {
-        if ("string" != typeof a && bc) return bc.apply(this, arguments);
+    var lc = n.fn.load;
+    n.fn.load = function(a, b, c) {
+        if ("string" != typeof a && lc) return lc.apply(this, arguments);
         var d, e, f, g = this,
             h = a.indexOf(" ");
-        return h >= 0 && (d = m.trim(a.slice(h, a.length)), a = a.slice(0, h)), m.isFunction(b) ? (c = b, b = void 0) : b && "object" == typeof b && (f = "POST"), g.length > 0 && m.ajax({
+        return h > -1 && (d = n.trim(a.slice(h, a.length)), a = a.slice(0, h)), n.isFunction(b) ? (c = b, b = void 0) : b && "object" == typeof b && (e = "POST"), g.length > 0 && n.ajax({
             url: a,
-            type: f,
+            type: e || "GET",
             dataType: "html",
             data: b
         }).done(function(a) {
-            e = arguments, g.html(d ? m("<div>").append(m.parseHTML(a)).find(d) : a)
-        }).complete(c && function(a, b) {
-            g.each(c, e || [a.responseText, b, a])
+            f = arguments, g.html(d ? n("<div>").append(n.parseHTML(a)).find(d) : a)
+        }).always(c && function(a, b) {
+            g.each(function() {
+                c.apply(this, f || [a.responseText, b, a])
+            })
         }), this
-    }, m.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(a, b) {
-        m.fn[b] = function(a) {
+    }, n.each(["ajaxStart", "ajaxStop", "ajaxComplete", "ajaxError", "ajaxSuccess", "ajaxSend"], function(a, b) {
+        n.fn[b] = function(a) {
             return this.on(b, a)
         }
-    }), m.expr.filters.animated = function(a) {
-        return m.grep(m.timers, function(b) {
+    }), n.expr.filters.animated = function(a) {
+        return n.grep(n.timers, function(b) {
             return a === b.elem
         }).length
     };
-    var cc = a.document.documentElement;
 
-    function dc(a) {
-        return m.isWindow(a) ? a : 9 === a.nodeType ? a.defaultView || a.parentWindow : !1
+    function mc(a) {
+        return n.isWindow(a) ? a : 9 === a.nodeType ? a.defaultView || a.parentWindow : !1
     }
-    m.offset = {
+    n.offset = {
         setOffset: function(a, b, c) {
-            var d, e, f, g, h, i, j, k = m.css(a, "position"),
-                l = m(a),
-                n = {};
-            "static" === k && (a.style.position = "relative"), h = l.offset(), f = m.css(a, "top"), i = m.css(a, "left"), j = ("absolute" === k || "fixed" === k) && m.inArray("auto", [f, i]) > -1, j ? (d = l.position(), g = d.top, e = d.left) : (g = parseFloat(f) || 0, e = parseFloat(i) || 0), m.isFunction(b) && (b = b.call(a, c, h)), null != b.top && (n.top = b.top - h.top + g), null != b.left && (n.left = b.left - h.left + e), "using" in b ? b.using.call(a, n) : l.css(n)
+            var d, e, f, g, h, i, j, k = n.css(a, "position"),
+                l = n(a),
+                m = {};
+            "static" === k && (a.style.position = "relative"), h = l.offset(), f = n.css(a, "top"), i = n.css(a, "left"), j = ("absolute" === k || "fixed" === k) && n.inArray("auto", [f, i]) > -1, j ? (d = l.position(), g = d.top, e = d.left) : (g = parseFloat(f) || 0, e = parseFloat(i) || 0), n.isFunction(b) && (b = b.call(a, c, n.extend({}, h))), null != b.top && (m.top = b.top - h.top + g), null != b.left && (m.left = b.left - h.left + e), "using" in b ? b.using.call(a, m) : l.css(m)
         }
-    }, m.fn.extend({
+    }, n.fn.extend({
         offset: function(a) {
             if (arguments.length) return void 0 === a ? this : this.each(function(b) {
-                m.offset.setOffset(this, a, b)
+                n.offset.setOffset(this, a, b)
             });
             var b, c, d = {
                     top: 0,
                     left: 0
                 },
                 e = this[0],
                 f = e && e.ownerDocument;
-            if (f) return b = f.documentElement, m.contains(b, e) ? (typeof e.getBoundingClientRect !== K && (d = e.getBoundingClientRect()), c = dc(f), {
+            if (f) return b = f.documentElement, n.contains(b, e) ? ("undefined" != typeof e.getBoundingClientRect && (d = e.getBoundingClientRect()), c = mc(f), {
                 top: d.top + (c.pageYOffset || b.scrollTop) - (b.clientTop || 0),
                 left: d.left + (c.pageXOffset || b.scrollLeft) - (b.clientLeft || 0)
             }) : d
         },
         position: function() {
             if (this[0]) {
                 var a, b, c = {
                         top: 0,
                         left: 0
                     },
                     d = this[0];
-                return "fixed" === m.css(d, "position") ? b = d.getBoundingClientRect() : (a = this.offsetParent(), b = this.offset(), m.nodeName(a[0], "html") || (c = a.offset()), c.top += m.css(a[0], "borderTopWidth", !0), c.left += m.css(a[0], "borderLeftWidth", !0)), {
-                    top: b.top - c.top - m.css(d, "marginTop", !0),
-                    left: b.left - c.left - m.css(d, "marginLeft", !0)
+                return "fixed" === n.css(d, "position") ? b = d.getBoundingClientRect() : (a = this.offsetParent(), b = this.offset(), n.nodeName(a[0], "html") || (c = a.offset()), c.top += n.css(a[0], "borderTopWidth", !0), c.left += n.css(a[0], "borderLeftWidth", !0)), {
+                    top: b.top - c.top - n.css(d, "marginTop", !0),
+                    left: b.left - c.left - n.css(d, "marginLeft", !0)
                 }
             }
         },
         offsetParent: function() {
             return this.map(function() {
-                var a = this.offsetParent || cc;
-                while (a && !m.nodeName(a, "html") && "static" === m.css(a, "position")) a = a.offsetParent;
-                return a || cc
+                var a = this.offsetParent;
+                while (a && !n.nodeName(a, "html") && "static" === n.css(a, "position")) a = a.offsetParent;
+                return a || Qa
             })
         }
-    }), m.each({
+    }), n.each({
         scrollLeft: "pageXOffset",
         scrollTop: "pageYOffset"
     }, function(a, b) {
         var c = /Y/.test(b);
-        m.fn[a] = function(d) {
-            return V(this, function(a, d, e) {
-                var f = dc(a);
-                return void 0 === e ? f ? b in f ? f[b] : f.document.documentElement[d] : a[d] : void(f ? f.scrollTo(c ? m(f).scrollLeft() : e, c ? e : m(f).scrollTop()) : a[d] = e)
+        n.fn[a] = function(d) {
+            return Y(this, function(a, d, e) {
+                var f = mc(a);
+                return void 0 === e ? f ? b in f ? f[b] : f.document.documentElement[d] : a[d] : void(f ? f.scrollTo(c ? n(f).scrollLeft() : e, c ? e : n(f).scrollTop()) : a[d] = e)
             }, a, d, arguments.length, null)
         }
-    }), m.each(["top", "left"], function(a, b) {
-        m.cssHooks[b] = La(k.pixelPosition, function(a, c) {
-            return c ? (c = Ja(a, b), Ha.test(c) ? m(a).position()[b] + "px" : c) : void 0
+    }), n.each(["top", "left"], function(a, b) {
+        n.cssHooks[b] = Ua(l.pixelPosition, function(a, c) {
+            return c ? (c = Sa(a, b), Oa.test(c) ? n(a).position()[b] + "px" : c) : void 0
         })
-    }), m.each({
+    }), n.each({
         Height: "height",
         Width: "width"
     }, function(a, b) {
-        m.each({
+        n.each({
             padding: "inner" + a,
             content: b,
             "": "outer" + a
         }, function(c, d) {
-            m.fn[d] = function(d, e) {
+            n.fn[d] = function(d, e) {
                 var f = arguments.length && (c || "boolean" != typeof d),
                     g = c || (d === !0 || e === !0 ? "margin" : "border");
-                return V(this, function(b, c, d) {
+                return Y(this, function(b, c, d) {
                     var e;
-                    return m.isWindow(b) ? b.document.documentElement["client" + a] : 9 === b.nodeType ? (e = b.documentElement, Math.max(b.body["scroll" + a], e["scroll" + a], b.body["offset" + a], e["offset" + a], e["client" + a])) : void 0 === d ? m.css(b, c, g) : m.style(b, c, d, g)
+                    return n.isWindow(b) ? b.document.documentElement["client" + a] : 9 === b.nodeType ? (e = b.documentElement, Math.max(b.body["scroll" + a], e["scroll" + a], b.body["offset" + a], e["offset" + a], e["client" + a])) : void 0 === d ? n.css(b, c, g) : n.style(b, c, d, g)
                 }, b, f ? d : void 0, f, null)
             }
         })
-    }), m.fn.size = function() {
+    }), n.fn.extend({
+        bind: function(a, b, c) {
+            return this.on(a, null, b, c)
+        },
+        unbind: function(a, b) {
+            return this.off(a, null, b)
+        },
+        delegate: function(a, b, c, d) {
+            return this.on(b, a, c, d)
+        },
+        undelegate: function(a, b, c) {
+            return 1 === arguments.length ? this.off(a, "**") : this.off(b, a || "**", c)
+        }
+    }), n.fn.size = function() {
         return this.length
-    }, m.fn.andSelf = m.fn.addBack, "function" == typeof define && define.amd && define("jquery", [], function() {
-        return m
+    }, n.fn.andSelf = n.fn.addBack, "function" == typeof define && define.amd && define("jquery", [], function() {
+        return n
     });
-    var ec = a.jQuery,
-        fc = a.$;
-    return m.noConflict = function(b) {
-        return a.$ === m && (a.$ = fc), b && a.jQuery === m && (a.jQuery = ec), m
-    }, typeof b === K && (a.jQuery = a.$ = m), m
+    var nc = a.jQuery,
+        oc = a.$;
+    return n.noConflict = function(b) {
+        return a.$ === n && (a.$ = oc), b && a.jQuery === n && (a.jQuery = nc), n
+    }, b || (a.jQuery = a.$ = n), n
 });
```

### Comparing `fookebox-0.7.3/COPYING` & `fookebox-1.0.0/COPYING`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,70 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
 
   The licenses for most software and other practical works are designed
 to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
+our General Public Licenses are intended to guarantee your freedom to
 share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
+software for all its users.
 
   When we speak of free software, we are referring to freedom, not
 price.  Our General Public Licenses are designed to make sure that you
 have the freedom to distribute copies of free software (and charge for
 them if you wish), that you receive source code or can get it if you
 want it, that you can change the software or use pieces of it in new
 free programs, and that you know you can do these things.
 
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
 
   The precise terms and conditions for copying, distribution and
 modification follow.
 
                        TERMS AND CONDITIONS
 
   0. Definitions.
 
-  "This License" refers to version 3 of the GNU General Public License.
+  "This License" refers to version 3 of the GNU Affero General Public License.
 
   "Copyright" also means copyright-like laws that apply to other kinds of
 works, such as semiconductor masks.
 
   "The Program" refers to any copyrightable work licensed under this
 License.  Each licensee is addressed as "you".  "Licensees" and
 "recipients" may be individuals or organizations.
@@ -545,43 +533,53 @@
 covered work so as to satisfy simultaneously your obligations under this
 License and any other pertinent obligations, then as a consequence you may
 not convey it at all.  For example, if you agree to terms that obligate you
 to collect a royalty for further conveying from those to whom you convey
 the Program, the only way you could satisfy both those terms and this
 License would be to refrain entirely from conveying the Program.
 
-  13. Use with the GNU Affero General Public License.
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
 
   Notwithstanding any other provision of this License, you have
 permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
+under version 3 of the GNU General Public License into a single
 combined work, and to convey the resulting work.  The terms of this
 License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
 
   14. Revised Versions of this License.
 
   The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
 address new problems or concerns.
 
   Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
+Program specifies that a certain numbered version of the GNU Affero General
 Public License "or any later version" applies to it, you have the
 option of following the terms and conditions either of that numbered
 version or of any later version published by the Free Software
 Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
+GNU Affero General Public License, you may choose any version ever published
 by the Free Software Foundation.
 
   If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
+versions of the GNU Affero General Public License can be used, that proxy's
 public statement of acceptance of a version permanently authorizes you
 to choose that version for the Program.
 
   Later license versions may give you additional or different
 permissions.  However, no additional obligations are imposed on any
 author or copyright holder as a result of your choosing to follow a
 later version.
@@ -631,44 +629,33 @@
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
     <one line to give the program's name and a brief idea of what it does.>
     Copyright (C) <year>  <name of author>
 
     This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
+    it under the terms of the GNU Affero General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+    GNU Affero General Public License for more details.
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<https://www.gnu.org/licenses/>.
```

