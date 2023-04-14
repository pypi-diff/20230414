# Comparing `tmp/jupylet-0.8.9.tar.gz` & `tmp/jupylet-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupylet-0.8.9.tar", last modified: Sat Dec 24 16:07:23 2022, max compression
+gzip compressed data, was "jupylet-0.9.0.tar", last modified: Fri Apr 14 09:38:19 2023, max compression
```

## Comparing `jupylet-0.8.9.tar` & `jupylet-0.9.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 naides     (502) staff       (20)        0 2022-12-24 16:07:23.414355 jupylet-0.8.9/
--rw-r--r--   0 naides     (502) staff       (20)     1319 2022-12-24 16:07:00.000000 jupylet-0.8.9/LICENSE.txt
--rw-r--r--   0 naides     (502) staff       (20)     8615 2022-12-24 16:07:23.414458 jupylet-0.8.9/PKG-INFO
--rw-r--r--   0 naides     (502) staff       (20)     7197 2022-12-24 16:07:00.000000 jupylet-0.8.9/README.md
-drwxr-xr-x   0 naides     (502) staff       (20)        0 2022-12-24 16:07:23.408728 jupylet-0.8.9/jupylet/
--rw-r--r--   0 naides     (502) staff       (20)     4111 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/__init__.py
--rw-r--r--   0 naides     (502) staff       (20)    17152 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/app.py
-drwxr-xr-x   0 naides     (502) staff       (20)        0 2022-12-24 16:07:23.402553 jupylet-0.8.9/jupylet/assets/
-drwxr-xr-x   0 naides     (502) staff       (20)        0 2022-12-24 16:07:23.409976 jupylet-0.8.9/jupylet/assets/fonts/
--rw-r--r--   0 naides     (502) staff       (20)     4519 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/assets/fonts/SIL Open Font License.txt
--rw-r--r--   0 naides     (502) staff       (20)   228024 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/assets/fonts/SourceSerifPro-Bold.otf
-drwxr-xr-x   0 naides     (502) staff       (20)        0 2022-12-24 16:07:23.411025 jupylet-0.8.9/jupylet/assets/shaders/
--rw-r--r--   0 naides     (502) staff       (20)     8802 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/assets/shaders/default-fragment-shader.glsl
--rw-r--r--   0 naides     (502) staff       (20)     2854 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/assets/shaders/default-vertex-shader.glsl
--rw-r--r--   0 naides     (502) staff       (20)     1825 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/assets/shaders/shadertoy-wrapper.glsl
--rw-r--r--   0 naides     (502) staff       (20)      801 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/assets/shaders/sprite.glsl
-drwxr-xr-x   0 naides     (502) staff       (20)        0 2022-12-24 16:07:23.402607 jupylet-0.8.9/jupylet/assets/sounds/
-drwxr-xr-x   0 naides     (502) staff       (20)        0 2022-12-24 16:07:23.412020 jupylet-0.8.9/jupylet/assets/sounds/impulses/
--rw-r--r--   0 naides     (502) staff       (20)    77860 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/assets/sounds/impulses/InsidePiano.flac
--rw-r--r--   0 naides     (502) staff       (20)    19937 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/assets/sounds/impulses/MaesHowe.flac
--rw-r--r--   0 naides     (502) staff       (20)     2272 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/assets/sounds/impulses/README.md
--rw-r--r--   0 naides     (502) staff       (20)    46202 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/assets/sounds/impulses/StAndrewsChurch.flac
-drwxr-xr-x   0 naides     (502) staff       (20)        0 2022-12-24 16:07:23.414175 jupylet-0.8.9/jupylet/audio/
--rw-r--r--   0 naides     (502) staff       (20)     5748 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/audio/__init__.py
--rw-r--r--   0 naides     (502) staff       (20)     1558 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/audio/bundle.py
--rw-r--r--   0 naides     (502) staff       (20)     8458 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/audio/device.py
--rw-r--r--   0 naides     (502) staff       (20)     9216 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/audio/effects.py
--rw-r--r--   0 naides     (502) staff       (20)     7190 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/audio/filters.py
--rw-r--r--   0 naides     (502) staff       (20)     4015 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/audio/midi.py
--rw-r--r--   0 naides     (502) staff       (20)     2706 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/audio/note.py
--rw-r--r--   0 naides     (502) staff       (20)     8887 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/audio/sample.py
--rw-r--r--   0 naides     (502) staff       (20)    38189 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/audio/sound.py
--rw-r--r--   0 naides     (502) staff       (20)     7878 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/audio/synth.py
--rw-r--r--   0 naides     (502) staff       (20)    12700 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/clock.py
--rw-r--r--   0 naides     (502) staff       (20)     4908 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/collision.py
--rw-r--r--   0 naides     (502) staff       (20)     1860 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/color.py
--rw-r--r--   0 naides     (502) staff       (20)     3977 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/env.py
--rw-r--r--   0 naides     (502) staff       (20)    19155 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/event.py
--rw-r--r--   0 naides     (502) staff       (20)     6613 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/label.py
--rw-r--r--   0 naides     (502) staff       (20)     9832 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/loader.py
--rw-r--r--   0 naides     (502) staff       (20)     3354 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/lru.py
--rw-r--r--   0 naides     (502) staff       (20)    23028 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/model.py
--rw-r--r--   0 naides     (502) staff       (20)     6967 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/node.py
--rw-r--r--   0 naides     (502) staff       (20)     7832 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/resource.py
--rw-r--r--   0 naides     (502) staff       (20)     7889 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/rl.py
--rw-r--r--   0 naides     (502) staff       (20)    18197 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/shadertoy.py
--rw-r--r--   0 naides     (502) staff       (20)    16044 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/sprite.py
--rw-r--r--   0 naides     (502) staff       (20)     1864 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/state.py
--rw-r--r--   0 naides     (502) staff       (20)     6192 2022-12-24 16:07:00.000000 jupylet-0.8.9/jupylet/utils.py
-drwxr-xr-x   0 naides     (502) staff       (20)        0 2022-12-24 16:07:23.409651 jupylet-0.8.9/jupylet.egg-info/
--rw-r--r--   0 naides     (502) staff       (20)     8615 2022-12-24 16:07:23.000000 jupylet-0.8.9/jupylet.egg-info/PKG-INFO
--rw-r--r--   0 naides     (502) staff       (20)     1205 2022-12-24 16:07:23.000000 jupylet-0.8.9/jupylet.egg-info/SOURCES.txt
--rw-r--r--   0 naides     (502) staff       (20)        1 2022-12-24 16:07:23.000000 jupylet-0.8.9/jupylet.egg-info/dependency_links.txt
--rw-r--r--   0 naides     (502) staff       (20)      245 2022-12-24 16:07:23.000000 jupylet-0.8.9/jupylet.egg-info/requires.txt
--rw-r--r--   0 naides     (502) staff       (20)        8 2022-12-24 16:07:23.000000 jupylet-0.8.9/jupylet.egg-info/top_level.txt
--rw-r--r--   0 naides     (502) staff       (20)      107 2022-12-24 16:07:23.414766 jupylet-0.8.9/setup.cfg
--rw-r--r--   0 naides     (502) staff       (20)     2396 2022-12-24 16:07:00.000000 jupylet-0.8.9/setup.py
+drwxr-xr-x   0 naides     (502) staff       (20)        0 2023-04-14 09:38:19.277433 jupylet-0.9.0/
+-rw-r--r--   0 naides     (502) staff       (20)     1319 2022-12-16 21:08:22.000000 jupylet-0.9.0/LICENSE.txt
+-rw-r--r--   0 naides     (502) staff       (20)     8831 2023-04-14 09:38:19.277538 jupylet-0.9.0/PKG-INFO
+-rw-r--r--   0 naides     (502) staff       (20)     7413 2023-04-14 09:37:42.000000 jupylet-0.9.0/README.md
+drwxr-xr-x   0 naides     (502) staff       (20)        0 2023-04-14 09:38:19.268805 jupylet-0.9.0/jupylet/
+-rw-r--r--   0 naides     (502) staff       (20)     4111 2023-04-14 04:37:44.000000 jupylet-0.9.0/jupylet/__init__.py
+-rw-r--r--   0 naides     (502) staff       (20)    17152 2022-12-24 10:59:03.000000 jupylet-0.9.0/jupylet/app.py
+drwxr-xr-x   0 naides     (502) staff       (20)        0 2023-04-14 09:38:19.260654 jupylet-0.9.0/jupylet/assets/
+drwxr-xr-x   0 naides     (502) staff       (20)        0 2023-04-14 09:38:19.270266 jupylet-0.9.0/jupylet/assets/fonts/
+-rw-r--r--   0 naides     (502) staff       (20)     4519 2021-10-14 09:16:45.000000 jupylet-0.9.0/jupylet/assets/fonts/SIL Open Font License.txt
+-rw-r--r--   0 naides     (502) staff       (20)   228024 2021-10-14 09:16:45.000000 jupylet-0.9.0/jupylet/assets/fonts/SourceSerifPro-Bold.otf
+drwxr-xr-x   0 naides     (502) staff       (20)        0 2023-04-14 09:38:19.271999 jupylet-0.9.0/jupylet/assets/shaders/
+-rw-r--r--   0 naides     (502) staff       (20)     8802 2021-10-14 09:16:45.000000 jupylet-0.9.0/jupylet/assets/shaders/default-fragment-shader.glsl
+-rw-r--r--   0 naides     (502) staff       (20)     2854 2021-10-14 09:16:45.000000 jupylet-0.9.0/jupylet/assets/shaders/default-vertex-shader.glsl
+-rw-r--r--   0 naides     (502) staff       (20)     1825 2021-10-14 09:16:45.000000 jupylet-0.9.0/jupylet/assets/shaders/shadertoy-wrapper.glsl
+-rw-r--r--   0 naides     (502) staff       (20)      801 2021-10-14 09:16:45.000000 jupylet-0.9.0/jupylet/assets/shaders/sprite.glsl
+drwxr-xr-x   0 naides     (502) staff       (20)        0 2023-04-14 09:38:19.260844 jupylet-0.9.0/jupylet/assets/sounds/
+drwxr-xr-x   0 naides     (502) staff       (20)        0 2023-04-14 09:38:19.272989 jupylet-0.9.0/jupylet/assets/sounds/impulses/
+-rw-r--r--   0 naides     (502) staff       (20)    77860 2021-10-14 09:16:45.000000 jupylet-0.9.0/jupylet/assets/sounds/impulses/InsidePiano.flac
+-rw-r--r--   0 naides     (502) staff       (20)    19937 2021-10-14 09:16:45.000000 jupylet-0.9.0/jupylet/assets/sounds/impulses/MaesHowe.flac
+-rw-r--r--   0 naides     (502) staff       (20)     2272 2021-10-14 09:16:45.000000 jupylet-0.9.0/jupylet/assets/sounds/impulses/README.md
+-rw-r--r--   0 naides     (502) staff       (20)    46202 2021-10-14 09:16:45.000000 jupylet-0.9.0/jupylet/assets/sounds/impulses/StAndrewsChurch.flac
+drwxr-xr-x   0 naides     (502) staff       (20)        0 2023-04-14 09:38:19.277188 jupylet-0.9.0/jupylet/audio/
+-rw-r--r--   0 naides     (502) staff       (20)     5748 2022-12-16 21:02:10.000000 jupylet-0.9.0/jupylet/audio/__init__.py
+-rw-r--r--   0 naides     (502) staff       (20)     1558 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/audio/bundle.py
+-rw-r--r--   0 naides     (502) staff       (20)     8458 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/audio/device.py
+-rw-r--r--   0 naides     (502) staff       (20)     9216 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/audio/effects.py
+-rw-r--r--   0 naides     (502) staff       (20)     7190 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/audio/filters.py
+-rw-r--r--   0 naides     (502) staff       (20)     4015 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/audio/midi.py
+-rw-r--r--   0 naides     (502) staff       (20)     2706 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/audio/note.py
+-rw-r--r--   0 naides     (502) staff       (20)     8887 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/audio/sample.py
+-rw-r--r--   0 naides     (502) staff       (20)    38189 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/audio/sound.py
+-rw-r--r--   0 naides     (502) staff       (20)     7878 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/audio/synth.py
+-rw-r--r--   0 naides     (502) staff       (20)    12700 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/clock.py
+-rw-r--r--   0 naides     (502) staff       (20)     4908 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/collision.py
+-rw-r--r--   0 naides     (502) staff       (20)     1860 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/color.py
+-rw-r--r--   0 naides     (502) staff       (20)     3977 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/env.py
+-rw-r--r--   0 naides     (502) staff       (20)    19155 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/event.py
+-rw-r--r--   0 naides     (502) staff       (20)     6613 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/label.py
+-rw-r--r--   0 naides     (502) staff       (20)     9832 2022-12-17 16:45:43.000000 jupylet-0.9.0/jupylet/loader.py
+-rw-r--r--   0 naides     (502) staff       (20)     3354 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/lru.py
+-rw-r--r--   0 naides     (502) staff       (20)    23028 2022-12-17 13:48:44.000000 jupylet-0.9.0/jupylet/model.py
+-rw-r--r--   0 naides     (502) staff       (20)     6967 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/node.py
+-rw-r--r--   0 naides     (502) staff       (20)     7832 2022-12-20 20:34:31.000000 jupylet-0.9.0/jupylet/resource.py
+-rw-r--r--   0 naides     (502) staff       (20)     7889 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/rl.py
+-rw-r--r--   0 naides     (502) staff       (20)    18197 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/shadertoy.py
+-rw-r--r--   0 naides     (502) staff       (20)    16044 2022-12-17 21:30:34.000000 jupylet-0.9.0/jupylet/sprite.py
+-rw-r--r--   0 naides     (502) staff       (20)     1864 2022-12-16 21:02:09.000000 jupylet-0.9.0/jupylet/state.py
+-rw-r--r--   0 naides     (502) staff       (20)     6192 2022-12-18 19:55:32.000000 jupylet-0.9.0/jupylet/utils.py
+drwxr-xr-x   0 naides     (502) staff       (20)        0 2023-04-14 09:38:19.269769 jupylet-0.9.0/jupylet.egg-info/
+-rw-r--r--   0 naides     (502) staff       (20)     8831 2023-04-14 09:38:19.000000 jupylet-0.9.0/jupylet.egg-info/PKG-INFO
+-rw-r--r--   0 naides     (502) staff       (20)     1205 2023-04-14 09:38:19.000000 jupylet-0.9.0/jupylet.egg-info/SOURCES.txt
+-rw-r--r--   0 naides     (502) staff       (20)        1 2023-04-14 09:38:19.000000 jupylet-0.9.0/jupylet.egg-info/dependency_links.txt
+-rw-r--r--   0 naides     (502) staff       (20)      258 2023-04-14 09:38:19.000000 jupylet-0.9.0/jupylet.egg-info/requires.txt
+-rw-r--r--   0 naides     (502) staff       (20)        8 2023-04-14 09:38:19.000000 jupylet-0.9.0/jupylet.egg-info/top_level.txt
+-rw-r--r--   0 naides     (502) staff       (20)      107 2023-04-14 09:38:19.277943 jupylet-0.9.0/setup.cfg
+-rw-r--r--   0 naides     (502) staff       (20)     2536 2023-04-14 09:26:43.000000 jupylet-0.9.0/setup.py
```

### Comparing `jupylet-0.8.9/LICENSE.txt` & `jupylet-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/PKG-INFO` & `jupylet-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jupylet
-Version: 0.8.9
+Version: 0.9.0
 Summary: Python game programming in Jupyter notebooks.
 Home-page: https://github.com/nir/jupylet
-Download-URL: https://github.com/nir/jupylet/archive/v0.8.9.tar.gz
+Download-URL: https://github.com/nir/jupylet/archive/v0.9.0.tar.gz
 Author: Nir Aides
 Author-email: nir.8bit@gmail.com
 License: bsd-2-clause
 Keywords: reinforcement learning,deep learning,synthesizers,moderngl,children,jupyter,python,games,midi,kids,RL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
@@ -40,16 +40,16 @@
 * Computer scientists, researchers, and students of deep reinforcement learning.
 * Musicians interested in sound synthesis and live music coding.
 * Kids and their parents interested in learning to program.
 
 &nbsp;
 
 <p float="left">
-    <img src="docs/images/spaceship.gif" width="256" />
-    <img src="docs/images/spaceship_3d.gif" width="384" />
+    <img src="https://github.com/nir/jupylet/raw/master/docs/images/spaceship.gif" width="256" />
+    <img src="https://github.com/nir/jupylet/raw/master/docs/images/spaceship_3d.gif" width="384" />
 </p>
 
 ## Jupylet for Kids
 
 A Jupyter notebook is in essence a laboratory for programming. It is the ideal
 environment for playing around with code, experimenting, and exploring ideas.
 It is used by professional machine learning scientists who come every day to
@@ -92,50 +92,51 @@
 
 Check out the [*Programming Sound and Music*](https://jupylet.readthedocs.io/en/latest/programmers_reference_guide/sound.html) 
 and the [*Programming Synthesizers*](https://jupylet.readthedocs.io/en/latest/programmers_reference_guide/synthesis.html)
 chapters in the Jupylet Programmer's Reference Guide.
 
 ## Requirements
 
-*Jupylet* should run on Python 3.6 and up on Windows, Mac, and Linux.
+*Jupylet* should run on Python 3.7 and up on Windows, Mac, and Linux.
 
 ## How to Install and Run Jupylet
 
 If you are new to Python, I recommend that you install and use the
 [Miniconda Python](https://docs.conda.io/en/latest/miniconda.html)
 distribution. 
 
-**On Windows** download and run the 64-bit installer for Python 3.9. Once 
+**On Windows** &ndash; download and run the 64-bit installer for Python 3.10. Once 
 Miniconda is installed press the `⊞ Winkey` and then type *Miniconda* and 
 press the `Enter` key. This should open a small window that programmers call 
 *console* or *shell* in which you can enter commands and run programs.
 
-**On macOS with Intel processor** download and run "Miniconda3 macOS Intel x86 64-bit pkg" 
-for Python 3.9. Once installed click the Spotlight icon `🔍` and in the search 
+**On macOS with Intel processor** &ndash; download and run "Miniconda3 macOS Intel x86 64-bit pkg" 
+for Python 3.10. Once installed click the Spotlight icon `🔍` and in the search 
 field type *terminal* and press the `Enter` key to open the console.
 
-**On macOS with M1 processor** download and run "Miniconda3 macOS Apple M1 64-bit pkg" 
-for Python 3.9. Once installed click the Spotlight icon `🔍` and in the search 
+**On macOS with M1 processor** &ndash; download and run "Miniconda3 macOS Apple M1 64-bit pkg" 
+for Python 3.10. Once installed click the Spotlight icon `🔍` and in the search 
 field type *terminal* and press the `Enter` key to open the console. Then
 you need to run the following two commands:
 
     conda install -c conda-forge numpy "libblas=*=*accelerate"
     pip install --pre -i https://pypi.anaconda.org/scipy-wheels-nightly/simple scipy
 
-These two commands are only needed if you have a macOS with an M1 processor.
+**On Linux** &ndash; download "Miniconda3 Linux 64-bit". This should download the file
+Miniconda3-latest-Linux-x86_64.sh. Install it by running the following command 
+in a bash shell (once installed start a new bash shell):
 
-Finally, to run *jupylet* first install it by typing the following command in 
-the console:
+    bash Miniconda3-latest-Linux-x86_64.sh
 
-    pip install jupylet
+---
 
-If you are using an old installation of Python 3.8 or 3.9 on Windows you may 
-also need to run following command:
+Once Miniconda is installed it is time to install *jupylet* by typing the 
+following command in the console:
 
-    python -m jupylet postinstall
+    pip install jupylet
 
 Next, to run the example notebooks, download the *jupylet* source code. 
 If you have [Git](https://git-scm.com/) installed type the following command:
 
     git clone https://github.com/nir/jupylet.git
 
 Alternatively, you can download the source code with the following command:
@@ -150,15 +151,15 @@
 And start a jupyter notebook with:
 
     jupyter notebook 11-spaceship.ipynb
 
 Run the notebook by following the instructions in the notebook and a game
 canvas should appear with the spaceship example:
 
-<img src="docs/images/spaceship.gif" width="256" height="256" />
+<img src="https://github.com/nir/jupylet/raw/master/docs/images/spaceship.gif" width="256" height="256" />
 
 Alternatively, you can run the same game as a Python script from the console 
 with:
 
     python spaceship.py
 
 ## Documentation
```

### Comparing `jupylet-0.8.9/README.md` & `jupylet-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 * Computer scientists, researchers, and students of deep reinforcement learning.
 * Musicians interested in sound synthesis and live music coding.
 * Kids and their parents interested in learning to program.
 
 &nbsp;
 
 <p float="left">
-    <img src="docs/images/spaceship.gif" width="256" />
-    <img src="docs/images/spaceship_3d.gif" width="384" />
+    <img src="https://github.com/nir/jupylet/raw/master/docs/images/spaceship.gif" width="256" />
+    <img src="https://github.com/nir/jupylet/raw/master/docs/images/spaceship_3d.gif" width="384" />
 </p>
 
 ## Jupylet for Kids
 
 A Jupyter notebook is in essence a laboratory for programming. It is the ideal
 environment for playing around with code, experimenting, and exploring ideas.
 It is used by professional machine learning scientists who come every day to
@@ -59,50 +59,51 @@
 
 Check out the [*Programming Sound and Music*](https://jupylet.readthedocs.io/en/latest/programmers_reference_guide/sound.html) 
 and the [*Programming Synthesizers*](https://jupylet.readthedocs.io/en/latest/programmers_reference_guide/synthesis.html)
 chapters in the Jupylet Programmer's Reference Guide.
 
 ## Requirements
 
-*Jupylet* should run on Python 3.6 and up on Windows, Mac, and Linux.
+*Jupylet* should run on Python 3.7 and up on Windows, Mac, and Linux.
 
 ## How to Install and Run Jupylet
 
 If you are new to Python, I recommend that you install and use the
 [Miniconda Python](https://docs.conda.io/en/latest/miniconda.html)
 distribution. 
 
-**On Windows** download and run the 64-bit installer for Python 3.9. Once 
+**On Windows** &ndash; download and run the 64-bit installer for Python 3.10. Once 
 Miniconda is installed press the `⊞ Winkey` and then type *Miniconda* and 
 press the `Enter` key. This should open a small window that programmers call 
 *console* or *shell* in which you can enter commands and run programs.
 
-**On macOS with Intel processor** download and run "Miniconda3 macOS Intel x86 64-bit pkg" 
-for Python 3.9. Once installed click the Spotlight icon `🔍` and in the search 
+**On macOS with Intel processor** &ndash; download and run "Miniconda3 macOS Intel x86 64-bit pkg" 
+for Python 3.10. Once installed click the Spotlight icon `🔍` and in the search 
 field type *terminal* and press the `Enter` key to open the console.
 
-**On macOS with M1 processor** download and run "Miniconda3 macOS Apple M1 64-bit pkg" 
-for Python 3.9. Once installed click the Spotlight icon `🔍` and in the search 
+**On macOS with M1 processor** &ndash; download and run "Miniconda3 macOS Apple M1 64-bit pkg" 
+for Python 3.10. Once installed click the Spotlight icon `🔍` and in the search 
 field type *terminal* and press the `Enter` key to open the console. Then
 you need to run the following two commands:
 
     conda install -c conda-forge numpy "libblas=*=*accelerate"
     pip install --pre -i https://pypi.anaconda.org/scipy-wheels-nightly/simple scipy
 
-These two commands are only needed if you have a macOS with an M1 processor.
+**On Linux** &ndash; download "Miniconda3 Linux 64-bit". This should download the file
+Miniconda3-latest-Linux-x86_64.sh. Install it by running the following command 
+in a bash shell (once installed start a new bash shell):
 
-Finally, to run *jupylet* first install it by typing the following command in 
-the console:
+    bash Miniconda3-latest-Linux-x86_64.sh
 
-    pip install jupylet
+---
 
-If you are using an old installation of Python 3.8 or 3.9 on Windows you may 
-also need to run following command:
+Once Miniconda is installed it is time to install *jupylet* by typing the 
+following command in the console:
 
-    python -m jupylet postinstall
+    pip install jupylet
 
 Next, to run the example notebooks, download the *jupylet* source code. 
 If you have [Git](https://git-scm.com/) installed type the following command:
 
     git clone https://github.com/nir/jupylet.git
 
 Alternatively, you can download the source code with the following command:
@@ -117,15 +118,15 @@
 And start a jupyter notebook with:
 
     jupyter notebook 11-spaceship.ipynb
 
 Run the notebook by following the instructions in the notebook and a game
 canvas should appear with the spaceship example:
 
-<img src="docs/images/spaceship.gif" width="256" height="256" />
+<img src="https://github.com/nir/jupylet/raw/master/docs/images/spaceship.gif" width="256" height="256" />
 
 Alternatively, you can run the same game as a Python script from the console 
 with:
 
     python spaceship.py
 
 ## Documentation
```

### Comparing `jupylet-0.8.9/jupylet/__init__.py` & `jupylet-0.9.0/jupylet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import sys
 import os
 import re
 
 from .env import is_remote, has_display, is_numpy_openblas
 
 
-VERSION = '0.8.9'
+VERSION = '0.9.0'
 
 
 if platform.system() == 'Linux' and not has_display():
     setattr(sys, 'is_pyglet_doc_run', True)
     
 
 #
```

### Comparing `jupylet-0.8.9/jupylet/app.py` & `jupylet-0.9.0/jupylet/app.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/assets/fonts/SIL Open Font License.txt` & `jupylet-0.9.0/jupylet/assets/fonts/SIL Open Font License.txt`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/assets/fonts/SourceSerifPro-Bold.otf` & `jupylet-0.9.0/jupylet/assets/fonts/SourceSerifPro-Bold.otf`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/assets/shaders/default-fragment-shader.glsl` & `jupylet-0.9.0/jupylet/assets/shaders/default-fragment-shader.glsl`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/assets/shaders/default-vertex-shader.glsl` & `jupylet-0.9.0/jupylet/assets/shaders/default-vertex-shader.glsl`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/assets/shaders/shadertoy-wrapper.glsl` & `jupylet-0.9.0/jupylet/assets/shaders/shadertoy-wrapper.glsl`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/assets/shaders/sprite.glsl` & `jupylet-0.9.0/jupylet/assets/shaders/sprite.glsl`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/assets/sounds/impulses/InsidePiano.flac` & `jupylet-0.9.0/jupylet/assets/sounds/impulses/InsidePiano.flac`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/assets/sounds/impulses/MaesHowe.flac` & `jupylet-0.9.0/jupylet/assets/sounds/impulses/MaesHowe.flac`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/assets/sounds/impulses/README.md` & `jupylet-0.9.0/jupylet/assets/sounds/impulses/README.md`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/assets/sounds/impulses/StAndrewsChurch.flac` & `jupylet-0.9.0/jupylet/assets/sounds/impulses/StAndrewsChurch.flac`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/audio/__init__.py` & `jupylet-0.9.0/jupylet/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/audio/bundle.py` & `jupylet-0.9.0/jupylet/audio/bundle.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/audio/device.py` & `jupylet-0.9.0/jupylet/audio/device.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/audio/effects.py` & `jupylet-0.9.0/jupylet/audio/effects.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/audio/filters.py` & `jupylet-0.9.0/jupylet/audio/filters.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/audio/midi.py` & `jupylet-0.9.0/jupylet/audio/midi.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/audio/note.py` & `jupylet-0.9.0/jupylet/audio/note.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/audio/sample.py` & `jupylet-0.9.0/jupylet/audio/sample.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/audio/sound.py` & `jupylet-0.9.0/jupylet/audio/sound.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/audio/synth.py` & `jupylet-0.9.0/jupylet/audio/synth.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/clock.py` & `jupylet-0.9.0/jupylet/clock.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/collision.py` & `jupylet-0.9.0/jupylet/collision.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/color.py` & `jupylet-0.9.0/jupylet/color.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/env.py` & `jupylet-0.9.0/jupylet/env.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/event.py` & `jupylet-0.9.0/jupylet/event.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/label.py` & `jupylet-0.9.0/jupylet/label.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/loader.py` & `jupylet-0.9.0/jupylet/loader.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/lru.py` & `jupylet-0.9.0/jupylet/lru.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/model.py` & `jupylet-0.9.0/jupylet/model.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/node.py` & `jupylet-0.9.0/jupylet/node.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/resource.py` & `jupylet-0.9.0/jupylet/resource.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/rl.py` & `jupylet-0.9.0/jupylet/rl.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/shadertoy.py` & `jupylet-0.9.0/jupylet/shadertoy.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/sprite.py` & `jupylet-0.9.0/jupylet/sprite.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/state.py` & `jupylet-0.9.0/jupylet/state.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet/utils.py` & `jupylet-0.9.0/jupylet/utils.py`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/jupylet.egg-info/PKG-INFO` & `jupylet-0.9.0/jupylet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jupylet
-Version: 0.8.9
+Version: 0.9.0
 Summary: Python game programming in Jupyter notebooks.
 Home-page: https://github.com/nir/jupylet
-Download-URL: https://github.com/nir/jupylet/archive/v0.8.9.tar.gz
+Download-URL: https://github.com/nir/jupylet/archive/v0.9.0.tar.gz
 Author: Nir Aides
 Author-email: nir.8bit@gmail.com
 License: bsd-2-clause
 Keywords: reinforcement learning,deep learning,synthesizers,moderngl,children,jupyter,python,games,midi,kids,RL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
@@ -40,16 +40,16 @@
 * Computer scientists, researchers, and students of deep reinforcement learning.
 * Musicians interested in sound synthesis and live music coding.
 * Kids and their parents interested in learning to program.
 
 &nbsp;
 
 <p float="left">
-    <img src="docs/images/spaceship.gif" width="256" />
-    <img src="docs/images/spaceship_3d.gif" width="384" />
+    <img src="https://github.com/nir/jupylet/raw/master/docs/images/spaceship.gif" width="256" />
+    <img src="https://github.com/nir/jupylet/raw/master/docs/images/spaceship_3d.gif" width="384" />
 </p>
 
 ## Jupylet for Kids
 
 A Jupyter notebook is in essence a laboratory for programming. It is the ideal
 environment for playing around with code, experimenting, and exploring ideas.
 It is used by professional machine learning scientists who come every day to
@@ -92,50 +92,51 @@
 
 Check out the [*Programming Sound and Music*](https://jupylet.readthedocs.io/en/latest/programmers_reference_guide/sound.html) 
 and the [*Programming Synthesizers*](https://jupylet.readthedocs.io/en/latest/programmers_reference_guide/synthesis.html)
 chapters in the Jupylet Programmer's Reference Guide.
 
 ## Requirements
 
-*Jupylet* should run on Python 3.6 and up on Windows, Mac, and Linux.
+*Jupylet* should run on Python 3.7 and up on Windows, Mac, and Linux.
 
 ## How to Install and Run Jupylet
 
 If you are new to Python, I recommend that you install and use the
 [Miniconda Python](https://docs.conda.io/en/latest/miniconda.html)
 distribution. 
 
-**On Windows** download and run the 64-bit installer for Python 3.9. Once 
+**On Windows** &ndash; download and run the 64-bit installer for Python 3.10. Once 
 Miniconda is installed press the `⊞ Winkey` and then type *Miniconda* and 
 press the `Enter` key. This should open a small window that programmers call 
 *console* or *shell* in which you can enter commands and run programs.
 
-**On macOS with Intel processor** download and run "Miniconda3 macOS Intel x86 64-bit pkg" 
-for Python 3.9. Once installed click the Spotlight icon `🔍` and in the search 
+**On macOS with Intel processor** &ndash; download and run "Miniconda3 macOS Intel x86 64-bit pkg" 
+for Python 3.10. Once installed click the Spotlight icon `🔍` and in the search 
 field type *terminal* and press the `Enter` key to open the console.
 
-**On macOS with M1 processor** download and run "Miniconda3 macOS Apple M1 64-bit pkg" 
-for Python 3.9. Once installed click the Spotlight icon `🔍` and in the search 
+**On macOS with M1 processor** &ndash; download and run "Miniconda3 macOS Apple M1 64-bit pkg" 
+for Python 3.10. Once installed click the Spotlight icon `🔍` and in the search 
 field type *terminal* and press the `Enter` key to open the console. Then
 you need to run the following two commands:
 
     conda install -c conda-forge numpy "libblas=*=*accelerate"
     pip install --pre -i https://pypi.anaconda.org/scipy-wheels-nightly/simple scipy
 
-These two commands are only needed if you have a macOS with an M1 processor.
+**On Linux** &ndash; download "Miniconda3 Linux 64-bit". This should download the file
+Miniconda3-latest-Linux-x86_64.sh. Install it by running the following command 
+in a bash shell (once installed start a new bash shell):
 
-Finally, to run *jupylet* first install it by typing the following command in 
-the console:
+    bash Miniconda3-latest-Linux-x86_64.sh
 
-    pip install jupylet
+---
 
-If you are using an old installation of Python 3.8 or 3.9 on Windows you may 
-also need to run following command:
+Once Miniconda is installed it is time to install *jupylet* by typing the 
+following command in the console:
 
-    python -m jupylet postinstall
+    pip install jupylet
 
 Next, to run the example notebooks, download the *jupylet* source code. 
 If you have [Git](https://git-scm.com/) installed type the following command:
 
     git clone https://github.com/nir/jupylet.git
 
 Alternatively, you can download the source code with the following command:
@@ -150,15 +151,15 @@
 And start a jupyter notebook with:
 
     jupyter notebook 11-spaceship.ipynb
 
 Run the notebook by following the instructions in the notebook and a game
 canvas should appear with the spaceship example:
 
-<img src="docs/images/spaceship.gif" width="256" height="256" />
+<img src="https://github.com/nir/jupylet/raw/master/docs/images/spaceship.gif" width="256" height="256" />
 
 Alternatively, you can run the same game as a Python script from the console 
 with:
 
     python spaceship.py
 
 ## Documentation
```

### Comparing `jupylet-0.8.9/jupylet.egg-info/SOURCES.txt` & `jupylet-0.9.0/jupylet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupylet-0.8.9/setup.py` & `jupylet-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 setuptools.setup(
     name = 'jupylet',
     packages = ['jupylet', 'jupylet.audio'],
     package_data={
        'jupylet': ['assets/*', 'assets/*/*', 'assets/*/*/*'],
     },
-    version = '0.8.9',
+    version = '0.9.0',
     license='bsd-2-clause',
     description = 'Python game programming in Jupyter notebooks.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author = 'Nir Aides',
     author_email = 'nir.8bit@gmail.com',
     url = 'https://github.com/nir/jupylet',
-    download_url = 'https://github.com/nir/jupylet/archive/v0.8.9.tar.gz',
+    download_url = 'https://github.com/nir/jupylet/archive/v0.9.0.tar.gz',
     keywords = [
         'reinforcement learning', 
         'deep learning', 
         'synthesizers',
         'moderngl', 
         'children',
         'jupyter', 
@@ -52,14 +52,15 @@
         'webcolors', 
         'ipyevents', 
         'ipywidgets', 
         'matplotlib', 
         'sounddevice', 
         'python-rtmidi ; platform_system!="Linux" and python_version<"3.10"',
         'moderngl-window',
+        'tornado==6.1', # workaround bug https://discourse.jupyter.org/t/jupyter-notebook-zmq-message-arrived-on-closed-channel-error/17869
     ],
     extras_require = {
         'midi': ['python-rtmidi']
     },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Education',
```

