# Comparing `tmp/shinyswatch-0.1.1.tar.gz` & `tmp/shinyswatch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinyswatch-0.1.1.tar", last modified: Wed Apr 12 17:31:41 2023, max compression
+gzip compressed data, was "shinyswatch-0.2.0.tar", last modified: Fri Apr 14 20:43:52 2023, max compression
```

## Comparing `shinyswatch-0.1.1.tar` & `shinyswatch-0.2.0.tar`

### file list

```diff
@@ -1,100 +1,80 @@
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.958611 shinyswatch-0.1.1/
--rw-r--r--   0 barret     (502) staff       (20)     1067 2023-03-29 18:28:41.000000 shinyswatch-0.1.1/LICENSE
--rw-r--r--   0 barret     (502) staff       (20)      216 2023-04-12 17:30:44.000000 shinyswatch-0.1.1/MANIFEST.in
--rw-r--r--   0 barret     (502) staff       (20)     2429 2023-04-12 17:31:41.958757 shinyswatch-0.1.1/PKG-INFO
--rw-r--r--   0 barret     (502) staff       (20)     1179 2023-04-11 21:01:32.000000 shinyswatch-0.1.1/README.md
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.923027 shinyswatch-0.1.1/docs/
--rw-r--r--   0 barret     (502) staff       (20)      638 2023-04-11 20:37:32.000000 shinyswatch-0.1.1/docs/Makefile
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.916098 shinyswatch-0.1.1/docs/build/
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.916402 shinyswatch-0.1.1/docs/build/html/
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.923404 shinyswatch-0.1.1/docs/build/html/_sources/
--rw-r--r--   0 barret     (502) staff       (20)      792 2023-04-12 13:21:09.000000 shinyswatch-0.1.1/docs/build/html/_sources/index.rst
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.923788 shinyswatch-0.1.1/docs/build/html/_sources/reference/
--rw-r--r--   0 barret     (502) staff       (20)       95 2023-04-12 13:34:05.000000 shinyswatch-0.1.1/docs/build/html/_sources/reference/shinyswatch.theme.rst
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.925467 shinyswatch-0.1.1/docs/build/html/_static/
--rw-r--r--   0 barret     (502) staff       (20)    30784 2023-04-12 13:39:56.000000 shinyswatch-0.1.1/docs/build/html/_static/bootswatch.png
--rw-r--r--   0 barret     (502) staff       (20)      286 2023-04-11 20:40:59.000000 shinyswatch-0.1.1/docs/build/html/_static/file.png
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.925831 shinyswatch-0.1.1/docs/build/html/_static/images/
--rw-r--r--   0 barret     (502) staff       (20)     7601 2023-04-11 20:45:27.000000 shinyswatch-0.1.1/docs/build/html/_static/images/logo_colab.png
--rw-r--r--   0 barret     (502) staff       (20)       90 2023-04-11 20:40:59.000000 shinyswatch-0.1.1/docs/build/html/_static/minus.png
--rw-r--r--   0 barret     (502) staff       (20)       90 2023-04-11 20:40:59.000000 shinyswatch-0.1.1/docs/build/html/_static/plus.png
--rw-r--r--   0 barret     (502) staff       (20)       70 2023-04-12 16:47:04.000000 shinyswatch-0.1.1/docs/modules.rst
--rw-r--r--   0 barret     (502) staff       (20)      156 2023-04-12 16:47:04.000000 shinyswatch-0.1.1/docs/shinyswatch.rst
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.927252 shinyswatch-0.1.1/docs/source/
--rw-r--r--   0 barret     (502) staff       (20)     3778 2023-04-12 13:38:51.000000 shinyswatch-0.1.1/docs/source/conf.py
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.928211 shinyswatch-0.1.1/docs/source/images/
--rw-r--r--   0 barret     (502) staff       (20)    17879 2023-04-12 13:38:59.000000 shinyswatch-0.1.1/docs/source/images/bootswatch copy.png
--rw-r--r--   0 barret     (502) staff       (20)    30784 2023-04-12 13:39:56.000000 shinyswatch-0.1.1/docs/source/images/bootswatch.png
--rw-r--r--   0 barret     (502) staff       (20)      792 2023-04-12 13:21:09.000000 shinyswatch-0.1.1/docs/source/index.rst
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.928673 shinyswatch-0.1.1/docs/source/reference/
--rw-r--r--   0 barret     (502) staff       (20)       95 2023-04-12 13:34:05.000000 shinyswatch-0.1.1/docs/source/reference/shinyswatch.theme.rst
--rw-r--r--   0 barret     (502) staff       (20)     1956 2023-04-12 17:31:41.959311 shinyswatch-0.1.1/setup.cfg
--rw-r--r--   0 barret     (502) staff       (20)       38 2023-03-23 14:55:23.000000 shinyswatch-0.1.1/setup.py
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.931944 shinyswatch-0.1.1/shinyswatch/
--rw-r--r--   0 barret     (502) staff       (20)      120 2023-04-12 17:31:09.000000 shinyswatch-0.1.1/shinyswatch/__init__.py
--rw-r--r--   0 barret     (502) staff       (20)      991 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/_assert.py
--rw-r--r--   0 barret     (502) staff       (20)     2941 2023-04-12 13:19:08.000000 shinyswatch-0.1.1/shinyswatch/_theme.py
--rw-r--r--   0 barret     (502) staff       (20)      584 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/_themes.py
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.920858 shinyswatch-0.1.1/shinyswatch/bsw5/
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.933840 shinyswatch-0.1.1/shinyswatch/bsw5/cerulean/
--rw-r--r--   0 barret     (502) staff       (20)   241305 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/cerulean/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.934678 shinyswatch-0.1.1/shinyswatch/bsw5/cosmo/
--rw-r--r--   0 barret     (502) staff       (20)   228137 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/cosmo/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.935328 shinyswatch-0.1.1/shinyswatch/bsw5/cyborg/
--rw-r--r--   0 barret     (502) staff       (20)   239795 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/cyborg/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.936090 shinyswatch-0.1.1/shinyswatch/bsw5/darkly/
--rw-r--r--   0 barret     (502) staff       (20)   244211 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/darkly/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.936561 shinyswatch-0.1.1/shinyswatch/bsw5/flatly/
--rw-r--r--   0 barret     (502) staff       (20)   240774 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/flatly/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.937325 shinyswatch-0.1.1/shinyswatch/bsw5/journal/
--rw-r--r--   0 barret     (502) staff       (20)   238362 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/journal/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.937913 shinyswatch-0.1.1/shinyswatch/bsw5/litera/
--rw-r--r--   0 barret     (502) staff       (20)   240358 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/litera/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.938639 shinyswatch-0.1.1/shinyswatch/bsw5/lumen/
--rw-r--r--   0 barret     (502) staff       (20)   245474 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/lumen/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.939173 shinyswatch-0.1.1/shinyswatch/bsw5/lux/
--rw-r--r--   0 barret     (502) staff       (20)   229679 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/lux/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.940246 shinyswatch-0.1.1/shinyswatch/bsw5/materia/
--rw-r--r--   0 barret     (502) staff       (20)   268868 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/materia/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.941115 shinyswatch-0.1.1/shinyswatch/bsw5/minty/
--rw-r--r--   0 barret     (502) staff       (20)   239411 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/minty/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.942160 shinyswatch-0.1.1/shinyswatch/bsw5/morph/
--rw-r--r--   0 barret     (502) staff       (20)   264987 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/morph/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.943232 shinyswatch-0.1.1/shinyswatch/bsw5/pulse/
--rw-r--r--   0 barret     (502) staff       (20)   231184 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/pulse/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.945299 shinyswatch-0.1.1/shinyswatch/bsw5/quartz/
--rw-r--r--   0 barret     (502) staff       (20)   275083 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/quartz/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.946305 shinyswatch-0.1.1/shinyswatch/bsw5/sandstone/
--rw-r--r--   0 barret     (502) staff       (20)   241171 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/sandstone/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.947005 shinyswatch-0.1.1/shinyswatch/bsw5/simplex/
--rw-r--r--   0 barret     (502) staff       (20)   241660 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/simplex/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.947767 shinyswatch-0.1.1/shinyswatch/bsw5/sketchy/
--rw-r--r--   0 barret     (502) staff       (20)   245207 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/sketchy/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.948423 shinyswatch-0.1.1/shinyswatch/bsw5/slate/
--rw-r--r--   0 barret     (502) staff       (20)   253193 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/slate/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.949296 shinyswatch-0.1.1/shinyswatch/bsw5/solar/
--rw-r--r--   0 barret     (502) staff       (20)   239224 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/solar/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.951368 shinyswatch-0.1.1/shinyswatch/bsw5/spacelab/
--rw-r--r--   0 barret     (502) staff       (20)   242824 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/spacelab/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.952086 shinyswatch-0.1.1/shinyswatch/bsw5/superhero/
--rw-r--r--   0 barret     (502) staff       (20)   239767 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/superhero/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.952863 shinyswatch-0.1.1/shinyswatch/bsw5/united/
--rw-r--r--   0 barret     (502) staff       (20)   237981 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/united/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.953585 shinyswatch-0.1.1/shinyswatch/bsw5/vapor/
--rw-r--r--   0 barret     (502) staff       (20)   256498 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/vapor/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.954064 shinyswatch-0.1.1/shinyswatch/bsw5/yeti/
--rw-r--r--   0 barret     (502) staff       (20)   249497 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/yeti/bootswatch.min.css
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.954861 shinyswatch-0.1.1/shinyswatch/bsw5/zephyr/
--rw-r--r--   0 barret     (502) staff       (20)   246162 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/shinyswatch/bsw5/zephyr/bootswatch.min.css
--rw-r--r--   0 barret     (502) staff       (20)        0 2023-03-23 14:55:23.000000 shinyswatch-0.1.1/shinyswatch/py.typed
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.933637 shinyswatch-0.1.1/shinyswatch.egg-info/
--rw-r--r--   0 barret     (502) staff       (20)     2429 2023-04-12 17:31:41.000000 shinyswatch-0.1.1/shinyswatch.egg-info/PKG-INFO
--rw-r--r--   0 barret     (502) staff       (20)     1988 2023-04-12 17:31:41.000000 shinyswatch-0.1.1/shinyswatch.egg-info/SOURCES.txt
--rw-r--r--   0 barret     (502) staff       (20)        1 2023-04-12 17:31:41.000000 shinyswatch-0.1.1/shinyswatch.egg-info/dependency_links.txt
--rw-r--r--   0 barret     (502) staff       (20)        1 2023-04-12 17:31:41.000000 shinyswatch-0.1.1/shinyswatch.egg-info/not-zip-safe
--rw-r--r--   0 barret     (502) staff       (20)      369 2023-04-12 17:31:41.000000 shinyswatch-0.1.1/shinyswatch.egg-info/requires.txt
--rw-r--r--   0 barret     (502) staff       (20)       12 2023-04-12 17:31:41.000000 shinyswatch-0.1.1/shinyswatch.egg-info/top_level.txt
-drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-12 17:31:41.958105 shinyswatch-0.1.1/tests/
--rw-r--r--   0 barret     (502) staff       (20)     6148 2023-03-29 18:47:46.000000 shinyswatch-0.1.1/tests/.DS_Store
--rw-r--r--   0 barret     (502) staff       (20)       33 2023-03-29 18:42:55.000000 shinyswatch-0.1.1/tests/__init__.py
--rw-r--r--   0 barret     (502) staff       (20)      474 2023-04-06 16:37:13.000000 shinyswatch-0.1.1/tests/test_themes.py
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.133769 shinyswatch-0.2.0/
+-rw-r--r--   0 barret     (502) staff       (20)     1067 2023-03-29 18:28:41.000000 shinyswatch-0.2.0/LICENSE
+-rw-r--r--   0 barret     (502) staff       (20)      252 2023-04-12 20:21:07.000000 shinyswatch-0.2.0/MANIFEST.in
+-rw-r--r--   0 barret     (502) staff       (20)     2729 2023-04-14 20:43:52.133902 shinyswatch-0.2.0/PKG-INFO
+-rw-r--r--   0 barret     (502) staff       (20)     1479 2023-04-14 20:41:01.000000 shinyswatch-0.2.0/README.md
+-rw-r--r--   0 barret     (502) staff       (20)     1891 2023-04-14 20:43:52.134356 shinyswatch-0.2.0/setup.cfg
+-rw-r--r--   0 barret     (502) staff       (20)       38 2023-03-23 14:55:23.000000 shinyswatch-0.2.0/setup.py
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.104700 shinyswatch-0.2.0/shinyswatch/
+-rw-r--r--   0 barret     (502) staff       (20)      171 2023-04-14 20:41:18.000000 shinyswatch-0.2.0/shinyswatch/__init__.py
+-rw-r--r--   0 barret     (502) staff       (20)      491 2023-04-12 20:21:07.000000 shinyswatch-0.2.0/shinyswatch/_assert.py
+-rw-r--r--   0 barret     (502) staff       (20)      890 2023-04-14 18:14:54.000000 shinyswatch-0.2.0/shinyswatch/_bsw5.py
+-rw-r--r--   0 barret     (502) staff       (20)     9336 2023-04-14 20:41:01.000000 shinyswatch-0.2.0/shinyswatch/_get_theme.py
+-rw-r--r--   0 barret     (502) staff       (20)     2583 2023-04-14 20:41:01.000000 shinyswatch-0.2.0/shinyswatch/_shiny_theme.py
+-rw-r--r--   0 barret     (502) staff       (20)      917 2023-04-12 20:21:07.000000 shinyswatch-0.2.0/shinyswatch/_typing_extensions.py
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.106504 shinyswatch-0.2.0/shinyswatch/bs5/
+-rw-r--r--   0 barret     (502) staff       (20)    80496 2023-04-14 18:14:46.000000 shinyswatch-0.2.0/shinyswatch/bs5/bootstrap.bundle.min.js
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.101947 shinyswatch-0.2.0/shinyswatch/bsw5/
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.107313 shinyswatch-0.2.0/shinyswatch/bsw5/cerulean/
+-rw-r--r--   0 barret     (502) staff       (20)   241305 2023-04-14 18:14:46.000000 shinyswatch-0.2.0/shinyswatch/bsw5/cerulean/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.108151 shinyswatch-0.2.0/shinyswatch/bsw5/cosmo/
+-rw-r--r--   0 barret     (502) staff       (20)   228137 2023-04-14 18:14:47.000000 shinyswatch-0.2.0/shinyswatch/bsw5/cosmo/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.108633 shinyswatch-0.2.0/shinyswatch/bsw5/cyborg/
+-rw-r--r--   0 barret     (502) staff       (20)   239795 2023-04-14 18:14:47.000000 shinyswatch-0.2.0/shinyswatch/bsw5/cyborg/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.109704 shinyswatch-0.2.0/shinyswatch/bsw5/darkly/
+-rw-r--r--   0 barret     (502) staff       (20)   244211 2023-04-14 18:14:47.000000 shinyswatch-0.2.0/shinyswatch/bsw5/darkly/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.110914 shinyswatch-0.2.0/shinyswatch/bsw5/flatly/
+-rw-r--r--   0 barret     (502) staff       (20)   240774 2023-04-14 18:14:48.000000 shinyswatch-0.2.0/shinyswatch/bsw5/flatly/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.112146 shinyswatch-0.2.0/shinyswatch/bsw5/journal/
+-rw-r--r--   0 barret     (502) staff       (20)   238362 2023-04-14 18:14:48.000000 shinyswatch-0.2.0/shinyswatch/bsw5/journal/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.113019 shinyswatch-0.2.0/shinyswatch/bsw5/litera/
+-rw-r--r--   0 barret     (502) staff       (20)   240358 2023-04-14 18:14:48.000000 shinyswatch-0.2.0/shinyswatch/bsw5/litera/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.114056 shinyswatch-0.2.0/shinyswatch/bsw5/lumen/
+-rw-r--r--   0 barret     (502) staff       (20)   245474 2023-04-14 18:14:48.000000 shinyswatch-0.2.0/shinyswatch/bsw5/lumen/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.114877 shinyswatch-0.2.0/shinyswatch/bsw5/lux/
+-rw-r--r--   0 barret     (502) staff       (20)   229679 2023-04-14 18:14:49.000000 shinyswatch-0.2.0/shinyswatch/bsw5/lux/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.115688 shinyswatch-0.2.0/shinyswatch/bsw5/materia/
+-rw-r--r--   0 barret     (502) staff       (20)   268868 2023-04-14 18:14:49.000000 shinyswatch-0.2.0/shinyswatch/bsw5/materia/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.116608 shinyswatch-0.2.0/shinyswatch/bsw5/minty/
+-rw-r--r--   0 barret     (502) staff       (20)   239411 2023-04-14 18:14:49.000000 shinyswatch-0.2.0/shinyswatch/bsw5/minty/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.117389 shinyswatch-0.2.0/shinyswatch/bsw5/morph/
+-rw-r--r--   0 barret     (502) staff       (20)   264987 2023-04-14 18:14:50.000000 shinyswatch-0.2.0/shinyswatch/bsw5/morph/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.118492 shinyswatch-0.2.0/shinyswatch/bsw5/pulse/
+-rw-r--r--   0 barret     (502) staff       (20)   231184 2023-04-14 18:14:50.000000 shinyswatch-0.2.0/shinyswatch/bsw5/pulse/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.120425 shinyswatch-0.2.0/shinyswatch/bsw5/quartz/
+-rw-r--r--   0 barret     (502) staff       (20)   275083 2023-04-14 18:14:50.000000 shinyswatch-0.2.0/shinyswatch/bsw5/quartz/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.121416 shinyswatch-0.2.0/shinyswatch/bsw5/sandstone/
+-rw-r--r--   0 barret     (502) staff       (20)   241171 2023-04-14 18:14:51.000000 shinyswatch-0.2.0/shinyswatch/bsw5/sandstone/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.122402 shinyswatch-0.2.0/shinyswatch/bsw5/simplex/
+-rw-r--r--   0 barret     (502) staff       (20)   241660 2023-04-14 18:14:51.000000 shinyswatch-0.2.0/shinyswatch/bsw5/simplex/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.122935 shinyswatch-0.2.0/shinyswatch/bsw5/sketchy/
+-rw-r--r--   0 barret     (502) staff       (20)   245207 2023-04-14 18:14:51.000000 shinyswatch-0.2.0/shinyswatch/bsw5/sketchy/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.124424 shinyswatch-0.2.0/shinyswatch/bsw5/slate/
+-rw-r--r--   0 barret     (502) staff       (20)   253193 2023-04-14 18:14:52.000000 shinyswatch-0.2.0/shinyswatch/bsw5/slate/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.126164 shinyswatch-0.2.0/shinyswatch/bsw5/solar/
+-rw-r--r--   0 barret     (502) staff       (20)   239224 2023-04-14 18:14:52.000000 shinyswatch-0.2.0/shinyswatch/bsw5/solar/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.127695 shinyswatch-0.2.0/shinyswatch/bsw5/spacelab/
+-rw-r--r--   0 barret     (502) staff       (20)   242824 2023-04-14 18:14:52.000000 shinyswatch-0.2.0/shinyswatch/bsw5/spacelab/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.128676 shinyswatch-0.2.0/shinyswatch/bsw5/superhero/
+-rw-r--r--   0 barret     (502) staff       (20)   239767 2023-04-14 18:14:52.000000 shinyswatch-0.2.0/shinyswatch/bsw5/superhero/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.129465 shinyswatch-0.2.0/shinyswatch/bsw5/united/
+-rw-r--r--   0 barret     (502) staff       (20)   237981 2023-04-14 18:14:53.000000 shinyswatch-0.2.0/shinyswatch/bsw5/united/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.130418 shinyswatch-0.2.0/shinyswatch/bsw5/vapor/
+-rw-r--r--   0 barret     (502) staff       (20)   256498 2023-04-14 18:14:53.000000 shinyswatch-0.2.0/shinyswatch/bsw5/vapor/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.131201 shinyswatch-0.2.0/shinyswatch/bsw5/yeti/
+-rw-r--r--   0 barret     (502) staff       (20)   249497 2023-04-14 18:14:53.000000 shinyswatch-0.2.0/shinyswatch/bsw5/yeti/bootswatch.min.css
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.132006 shinyswatch-0.2.0/shinyswatch/bsw5/zephyr/
+-rw-r--r--   0 barret     (502) staff       (20)   246162 2023-04-14 18:14:54.000000 shinyswatch-0.2.0/shinyswatch/bsw5/zephyr/bootswatch.min.css
+-rw-r--r--   0 barret     (502) staff       (20)        0 2023-03-23 14:55:23.000000 shinyswatch-0.2.0/shinyswatch/py.typed
+-rw-r--r--   0 barret     (502) staff       (20)    28215 2023-04-14 20:41:01.000000 shinyswatch-0.2.0/shinyswatch/theme.py
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.106302 shinyswatch-0.2.0/shinyswatch.egg-info/
+-rw-r--r--   0 barret     (502) staff       (20)     2729 2023-04-14 20:43:51.000000 shinyswatch-0.2.0/shinyswatch.egg-info/PKG-INFO
+-rw-r--r--   0 barret     (502) staff       (20)     1625 2023-04-14 20:43:52.000000 shinyswatch-0.2.0/shinyswatch.egg-info/SOURCES.txt
+-rw-r--r--   0 barret     (502) staff       (20)        1 2023-04-14 20:43:51.000000 shinyswatch-0.2.0/shinyswatch.egg-info/dependency_links.txt
+-rw-r--r--   0 barret     (502) staff       (20)        1 2023-04-14 20:43:51.000000 shinyswatch-0.2.0/shinyswatch.egg-info/not-zip-safe
+-rw-r--r--   0 barret     (502) staff       (20)      308 2023-04-14 20:43:51.000000 shinyswatch-0.2.0/shinyswatch.egg-info/requires.txt
+-rw-r--r--   0 barret     (502) staff       (20)       12 2023-04-14 20:43:51.000000 shinyswatch-0.2.0/shinyswatch.egg-info/top_level.txt
+drwxr-xr-x   0 barret     (502) staff       (20)        0 2023-04-14 20:43:52.133538 shinyswatch-0.2.0/tests/
+-rw-r--r--   0 barret     (502) staff       (20)     6148 2023-03-29 18:47:46.000000 shinyswatch-0.2.0/tests/.DS_Store
+-rw-r--r--   0 barret     (502) staff       (20)       33 2023-03-29 18:42:55.000000 shinyswatch-0.2.0/tests/__init__.py
+-rw-r--r--   0 barret     (502) staff       (20)      571 2023-04-14 20:41:01.000000 shinyswatch-0.2.0/tests/test_themes.py
```

### Comparing `shinyswatch-0.1.1/LICENSE` & `shinyswatch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/PKG-INFO` & `shinyswatch-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinyswatch
-Version: 0.1.1
+Version: 0.2.0
 Summary: Bootswatch + Bootstrap 5 themes for Shiny.
 Home-page: https://github.com/schloerke/py-shinyswatch
 Author: Barret Schloerke
 Author-email: barret@posit.co
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schloerke/py-shinyswatch/issues
 Project-URL: Source Code, https://github.com/schloerke/py-shinyswatch
@@ -44,23 +44,26 @@
 
 ```sh
 pip install https://github.com/schloerke/py-shinyswatch/tarball/main
 ```
 
 ## Usage
 
-Add your theme **anywhere** within your App's UI defintion. For example:
+Add your theme within your App's top level UI defintion. For example:
 
-```py
+```python
+# File: app.py
 from shiny import App, Inputs, Outputs, Session, render, ui
 
 import shinyswatch
 
 app_ui = ui.page_fluid(
-    shinyswatch.theme("darkly"),
+    # Theme code - start
+    shinyswatch.theme.darkly(),
+    # Theme code - end
     ui.input_slider("num", "Number:", min=10, max=100, value=30),
     ui.output_text_verbatim("slider_val"),
 )
 
 
 def server(input: Inputs, output: Outputs, session: Session):
     @output
@@ -70,22 +73,24 @@
 
 
 app = App(app_ui, server)
 ```
 
 ## Examples
 
-There are two examples in the shinyswatch repo. After checking out the repo, you can run them by calling:
+There are two examples in the shinyswatch repo. You can view them online at: [shinyswatch.theme.darkly](http://rstudio.github.io/py-shinyswatch/reference/theme.darkly.html) and [get_theme](http://rstudio.github.io/py-shinyswatch/reference/get_theme.html).
+
+To run the demos locally, you can clone the repo and run the examples by calling:
 
 ```sh
 python3 -m shiny run examples/basic-darkly/app.py
+# or
 python3 -m shiny run examples/big-sketchy/app.py
 ```
 
-
 ## Development
 
 If you want to do development on shinyswatch for Python:
 
 ```sh
 pip install -e ".[dev,test]"
 ```
```

### Comparing `shinyswatch-0.1.1/README.md` & `shinyswatch-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,23 +12,26 @@
 
 ```sh
 pip install https://github.com/schloerke/py-shinyswatch/tarball/main
 ```
 
 ## Usage
 
-Add your theme **anywhere** within your App's UI defintion. For example:
+Add your theme within your App's top level UI defintion. For example:
 
-```py
+```python
+# File: app.py
 from shiny import App, Inputs, Outputs, Session, render, ui
 
 import shinyswatch
 
 app_ui = ui.page_fluid(
-    shinyswatch.theme("darkly"),
+    # Theme code - start
+    shinyswatch.theme.darkly(),
+    # Theme code - end
     ui.input_slider("num", "Number:", min=10, max=100, value=30),
     ui.output_text_verbatim("slider_val"),
 )
 
 
 def server(input: Inputs, output: Outputs, session: Session):
     @output
@@ -38,22 +41,24 @@
 
 
 app = App(app_ui, server)
 ```
 
 ## Examples
 
-There are two examples in the shinyswatch repo. After checking out the repo, you can run them by calling:
+There are two examples in the shinyswatch repo. You can view them online at: [shinyswatch.theme.darkly](http://rstudio.github.io/py-shinyswatch/reference/theme.darkly.html) and [get_theme](http://rstudio.github.io/py-shinyswatch/reference/get_theme.html).
+
+To run the demos locally, you can clone the repo and run the examples by calling:
 
 ```sh
 python3 -m shiny run examples/basic-darkly/app.py
+# or
 python3 -m shiny run examples/big-sketchy/app.py
 ```
 
-
 ## Development
 
 If you want to do development on shinyswatch for Python:
 
 ```sh
 pip install -e ".[dev,test]"
 ```
```

### Comparing `shinyswatch-0.1.1/setup.cfg` & `shinyswatch-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -52,21 +52,17 @@
 dev = 
 	black>=23.1.0
 	flake8==5.0.4;python_version<="3.7"
 	flake8>=6.0.0;python_version>"3.7"
 	isort>=5.11.2
 	pyright>=1.1.301
 	pre-commit>=2.15.0
-	twine
 	wheel
 docs = 
-	sphinx_autodoc_typehints
 	shinylive
-	myst_parser
-	sphinx_book_theme
 
 [options.packages.find]
 include = shinyswatch
 
 [options.package_data]
 shinyswatch = py.typed
```

### Comparing `shinyswatch-0.1.1/shinyswatch/_theme.py` & `shinyswatch-0.2.0/shinyswatch/_shiny_theme.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,64 @@
+# TODO-barret; If the version does not start with a 5, raise a warning fi the major version is not 5
+# TODO-barret; Make a test to check if the shiny version of bootstrap is not v5
+# TODO-barret; make the themes into methods that return the theme object
+# def cerulean():
+#     return get_theme("cerulean")
+# TODO-barret; Remind users that they will need internet access to get the fonts
+
 from __future__ import annotations
 
 import os
 from copy import deepcopy
 
 from htmltools import HTMLDependency
 from shiny.ui import page_bootstrap as shiny_page_bootstrap
 
-from ._assert import assert_theme
-from ._themes import versions
+from ._bsw5 import bsw5_version
+
+_bs5_path = os.path.join(os.path.dirname(__file__), "bs5")
+
 
+# Overwrite the bootstrap dependency with a custom one that disables the stylesheet
+bs_dep_no_files = None
 
-def _shiny_theme(html_dep: HTMLDependency) -> list[HTMLDependency]:
-    bs_no_style = None
+# Get a vanilla bootstrap page to extract the bootstrap dependency
+shiny_deps = shiny_page_bootstrap().get_dependencies()
+for dep in shiny_deps:
+    if dep.name != "bootstrap":
+        continue
+    # Copy the dependency,
+    # and disable the stylesheet (to be overwritten by shinyswatch)
+    # and disable the JS to make sure the BS's JS files match (to be overwritten by shinyswatch)
+    # There could be `meta` or `head` information in the dependency that we want to keep
+    bs_dep_no_files = deepcopy(dep)
+    # Disable bootstrap.min.css as it is included in bootswatch bundle
+    bs_dep_no_files.stylesheet = []
+    # Disable bootstrap.min.js as it is included at end of function
+    bs_dep_no_files.script = []
+    # Rename to convey intent (and to disable it below)
+    bs_dep_no_files.name = "bootstrap-no-files"
 
-    # Get a vanilla bootstrap page to extract the bootstrap dependency
-    shiny_deps = shiny_page_bootstrap().get_dependencies()
-    for dep in shiny_deps:
-        if dep.name == "bootstrap":
-            # Copy the dependency, but only disable the stylesheet (to keep the JS files)
-            bs_no_style = deepcopy(dep)
-            # Disable bootstrap.min.css as it is included in bootswatch bundle
-            bs_no_style.stylesheet = []
-            # Rename to convey intent (and to disable it below)
-            bs_no_style.name = "bootstrap-no-style"
+if bs_dep_no_files is None:
+    raise ValueError("Could not find bootstrap dependency")
 
-    if bs_no_style is None:
-        raise ValueError("Could not find bootstrap dependency")
 
+# This is to prevent the Shiny bootstrap stylesheet from being loaded and instead load the bootswatch + bootstrap stylesheet
+def shiny_theme(html_dep: HTMLDependency) -> list[HTMLDependency]:
     return [
-        # Use a custom version of bootstrap with no stylesheets
-        bs_no_style,
+        # Use a custom version of bootstrap with no stylesheets/JS
+        bs_dep_no_files,
         # _Disable_ bootstrap html dep
         # Prevents  bootstrap from being loaded at a later time (Ex: shiny.ui.card() https://github.com/rstudio/py-shiny/blob/d08af1a8534677c7026b60559cd5eafc5f6608d7/shiny/ui/_navs.py#L983)
         HTMLDependency(
             name="bootstrap",
             version="9999",
         ),
+        # Add in the matching JS files
+        HTMLDependency(
+            name="bootstrap-js",
+            version=bsw5_version,
+            source={"package": "shinyswatch", "subdir": _bs5_path},
+            script={"src": "bootstrap.bundle.min.js"},
+        ),
         html_dep,
     ]
-
-
-def theme(name: str) -> list[HTMLDependency]:
-    """
-    Create a Bootswatch and Bootstrap 5 theme for Shiny.
-
-    Parameters
-    ----------
-    name
-        A Bootswatch theme name.
-
-    Returns
-    -------
-    A list of HTML dependencies.
-
-    Example
-    --------
-
-    .. code-block:: python
-
-        # File: app.py
-        from shiny import App, Inputs, Outputs, Session, render, ui
-
-        import shinyswatch
-
-        app_ui = ui.page_fluid(
-            # Theme code - start
-            shinyswatch.theme("darkly"),
-            # Theme code - end
-            ui.input_slider("num", "Number:", min=10, max=100, value=30),
-            ui.output_text_verbatim("slider_val"),
-        )
-
-        def server(input: Inputs, output: Outputs, session: Session):
-            @output
-            @render.text
-            def slider_val():
-                return f"{input.num()}"
-
-
-        app = App(app_ui, server)
-
-
-
-    >>> from shinyswatch import theme
-    """
-
-    bs_ver = "5"
-    assert_theme(name=name, bs_ver=bs_ver)
-
-    subdir = os.path.join(os.path.dirname(__file__), "bsw" + bs_ver, name)
-
-    # Contains both bootstrap and bootswatch css
-    html_dep = HTMLDependency(
-        name=f"bootstrap-and-bootswatch-{name}",
-        version=versions[bs_ver],
-        source={
-            "package": "shinyswatch",
-            "subdir": subdir,
-        },
-        stylesheet=[
-            {
-                "href": "bootswatch.min.css",
-            }
-        ],
-    )
-
-    return _shiny_theme(html_dep=html_dep)
```

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/cerulean/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/cerulean/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/cosmo/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/cosmo/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/cyborg/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/cyborg/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/darkly/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/darkly/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/flatly/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/flatly/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/journal/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/journal/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/litera/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/litera/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/lumen/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/lumen/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/lux/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/lux/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/materia/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/materia/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/minty/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/minty/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/morph/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/morph/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/pulse/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/pulse/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/quartz/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/quartz/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/sandstone/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/sandstone/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/simplex/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/simplex/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/sketchy/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/sketchy/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/slate/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/slate/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/solar/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/solar/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/spacelab/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/spacelab/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/superhero/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/superhero/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/united/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/united/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/vapor/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/vapor/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/yeti/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/yeti/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch/bsw5/zephyr/bootswatch.min.css` & `shinyswatch-0.2.0/shinyswatch/bsw5/zephyr/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.1.1/shinyswatch.egg-info/PKG-INFO` & `shinyswatch-0.2.0/shinyswatch.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinyswatch
-Version: 0.1.1
+Version: 0.2.0
 Summary: Bootswatch + Bootstrap 5 themes for Shiny.
 Home-page: https://github.com/schloerke/py-shinyswatch
 Author: Barret Schloerke
 Author-email: barret@posit.co
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schloerke/py-shinyswatch/issues
 Project-URL: Source Code, https://github.com/schloerke/py-shinyswatch
@@ -44,23 +44,26 @@
 
 ```sh
 pip install https://github.com/schloerke/py-shinyswatch/tarball/main
 ```
 
 ## Usage
 
-Add your theme **anywhere** within your App's UI defintion. For example:
+Add your theme within your App's top level UI defintion. For example:
 
-```py
+```python
+# File: app.py
 from shiny import App, Inputs, Outputs, Session, render, ui
 
 import shinyswatch
 
 app_ui = ui.page_fluid(
-    shinyswatch.theme("darkly"),
+    # Theme code - start
+    shinyswatch.theme.darkly(),
+    # Theme code - end
     ui.input_slider("num", "Number:", min=10, max=100, value=30),
     ui.output_text_verbatim("slider_val"),
 )
 
 
 def server(input: Inputs, output: Outputs, session: Session):
     @output
@@ -70,22 +73,24 @@
 
 
 app = App(app_ui, server)
 ```
 
 ## Examples
 
-There are two examples in the shinyswatch repo. After checking out the repo, you can run them by calling:
+There are two examples in the shinyswatch repo. You can view them online at: [shinyswatch.theme.darkly](http://rstudio.github.io/py-shinyswatch/reference/theme.darkly.html) and [get_theme](http://rstudio.github.io/py-shinyswatch/reference/get_theme.html).
+
+To run the demos locally, you can clone the repo and run the examples by calling:
 
 ```sh
 python3 -m shiny run examples/basic-darkly/app.py
+# or
 python3 -m shiny run examples/big-sketchy/app.py
 ```
 
-
 ## Development
 
 If you want to do development on shinyswatch for Python:
 
 ```sh
 pip install -e ".[dev,test]"
 ```
```

### Comparing `shinyswatch-0.1.1/tests/.DS_Store` & `shinyswatch-0.2.0/tests/.DS_Store`

 * *Files identical despite different names*

