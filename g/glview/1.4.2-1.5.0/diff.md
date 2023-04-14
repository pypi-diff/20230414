# Comparing `tmp/glview-1.4.2.tar.gz` & `tmp/glview-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glview-1.4.2.tar", last modified: Wed Mar 15 12:17:12 2023, max compression
+gzip compressed data, was "glview-1.5.0.tar", last modified: Fri Apr 14 14:05:09 2023, max compression
```

## Comparing `glview-1.4.2.tar` & `glview-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-03-15 12:17:12.160288 glview-1.4.2/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2022-04-04 11:40:47.000000 glview-1.4.2/LICENSE
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       99 2022-04-04 11:40:47.000000 glview-1.4.2/MANIFEST.in
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      963 2023-03-15 12:17:12.159304 glview-1.4.2/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      361 2023-03-15 11:16:49.000000 glview-1.4.2/README.md
-drwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-03-15 12:17:12.145708 glview-1.4.2/glview/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      332 2023-03-15 12:13:48.000000 glview-1.4.2/glview/__init__.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15417 2023-03-15 11:16:49.000000 glview-1.4.2/glview/argv.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    10110 2023-03-15 11:16:49.000000 glview-1.4.2/glview/glrenderer.py
--rwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)     8145 2023-03-15 12:10:12.000000 glview-1.4.2/glview/glview.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     6950 2023-03-15 11:16:49.000000 glview-1.4.2/glview/imageprovider.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      285 2022-04-04 11:40:47.000000 glview-1.4.2/glview/panzoom.vs
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    16148 2023-03-15 11:16:49.000000 glview-1.4.2/glview/pygletui.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1728 2023-03-15 11:16:49.000000 glview-1.4.2/glview/texture.fs
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       22 2023-03-15 11:56:40.000000 glview-1.4.2/glview/version.py
-drwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-03-15 12:17:12.157849 glview-1.4.2/glview.egg-info/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      963 2023-03-15 12:17:11.000000 glview-1.4.2/glview.egg-info/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      431 2023-03-15 12:17:12.000000 glview-1.4.2/glview.egg-info/SOURCES.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-03-15 12:17:11.000000 glview-1.4.2/glview.egg-info/dependency_links.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       40 2023-03-15 12:17:11.000000 glview-1.4.2/glview.egg-info/entry_points.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-03-15 12:17:11.000000 glview-1.4.2/glview.egg-info/requires.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)        7 2023-03-15 12:17:11.000000 glview-1.4.2/glview.egg-info/top_level.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-03-15 12:17:11.000000 glview-1.4.2/glview.egg-info/zip-safe
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      163 2023-03-15 11:16:49.000000 glview-1.4.2/requirements.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-03-15 12:17:12.160288 glview-1.4.2/setup.cfg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1200 2023-03-15 11:55:59.000000 glview-1.4.2/setup.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-14 14:05:09.602748 glview-1.5.0/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 glview-1.5.0/LICENSE
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       99 2023-03-13 15:45:56.000000 glview-1.5.0/MANIFEST.in
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      830 2023-04-14 14:05:09.602748 glview-1.5.0/PKG-INFO
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      361 2023-03-13 15:45:56.000000 glview-1.5.0/README.md
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-14 14:05:09.598748 glview-1.5.0/glview/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      332 2023-03-15 12:51:16.000000 glview-1.5.0/glview/__init__.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15417 2023-03-13 15:45:56.000000 glview-1.5.0/glview/argv.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    11494 2023-04-14 14:01:57.000000 glview-1.5.0/glview/glrenderer.py
+-rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)     9035 2023-04-14 08:09:07.000000 glview-1.5.0/glview/glview.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     6950 2023-03-13 15:45:56.000000 glview-1.5.0/glview/imageprovider.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      285 2023-03-13 15:45:56.000000 glview-1.5.0/glview/panzoom.vs
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    17213 2023-04-14 13:56:12.000000 glview-1.5.0/glview/pygletui.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     4478 2023-04-14 11:24:45.000000 glview-1.5.0/glview/texture.fs
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       22 2023-03-16 09:59:41.000000 glview-1.5.0/glview/version.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-04-14 14:05:09.602748 glview-1.5.0/glview.egg-info/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      830 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/PKG-INFO
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      431 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/SOURCES.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/dependency_links.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       40 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/entry_points.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/requires.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        7 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/top_level.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-04-14 14:05:09.000000 glview-1.5.0/glview.egg-info/zip-safe
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      163 2023-03-14 15:45:52.000000 glview-1.5.0/requirements.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-04-14 14:05:09.602748 glview-1.5.0/setup.cfg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1200 2023-03-13 15:45:56.000000 glview-1.5.0/setup.py
```

### Comparing `glview-1.4.2/LICENSE` & `glview-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glview-1.4.2/PKG-INFO` & `glview-1.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: glview
-Version: 1.4.2
+Version: 1.5.0
 Summary: Lightning-fast image viewer with smooth zooming & panning.
 Home-page: http://github.com/toaarnio/glview
 Author: Tomi Aarnio
 Author-email: tomi.p.aarnio@gmail.com
 License: MIT
-Description: # glview
-        
-        [![Build Status](https://travis-ci.com/toaarnio/glview.svg?branch=master)](https://travis-ci.com/github/toaarnio/glview)
-        
-        Lightning-fast image viewer with smooth zooming &amp; panning + HDR exposure control.
-        
-        **Installing:**
-        ```
-        pip install glview
-        ```
-        
-        **Usage:**
-        ```
-        glview --help
-        ```
-        
-        **Building &amp; installing from source:**
-        ```
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# glview
+
+[![Build Status](https://travis-ci.com/toaarnio/glview.svg?branch=master)](https://travis-ci.com/github/toaarnio/glview)
+
+Lightning-fast image viewer with smooth zooming &amp; panning + HDR exposure control.
+
+**Installing:**
+```
+pip install glview
+```
+
+**Usage:**
+```
+glview --help
+```
+
+**Building &amp; installing from source:**
+```
+
+
```

### Comparing `glview-1.4.2/glview/argv.py` & `glview-1.5.0/glview/argv.py`

 * *Files identical despite different names*

### Comparing `glview-1.4.2/glview/glrenderer.py` & `glview-1.5.0/glview/glrenderer.py`

 * *Files 12% similar despite different names*

```diff
@@ -79,72 +79,104 @@
             self.prog['mousepos'].value = tuple(self.ui.mousepos)
             self.prog['orientation'].value = orientation
             self.prog['aspect'].value = self._get_aspect_ratio(vpw, vph, texw, texh)
             self.prog['scale'].value = self.ui.scale
             self.prog['grayscale'].value = (texture.components == 1)
             self.prog['gamma'].value = self.ui.gamma
             self.prog['ev'].value = self.ui.ev
-            self.prog['gamut.power'].value = self.ui.gamut_power
+            self.prog['gamut.compress'].value = self.ui.gamut_fit
+            self.prog['gamut.power'].value = self.ui.gamut_pow
             self.prog['gamut.thr'].value = self.ui.gamut_thr
-            self.prog['gamut.scale'].value = self._gamut_curve(self.ui.gamut_power, self.ui.gamut_thr, self.ui.gamut_lim)
+            self.prog['gamut.scale'].value = self._gamut(imgidx)
+            self.prog['debug'].value = self.ui.debug_mode
             self.vao.render(moderngl.TRIANGLE_STRIP)
         self.ctx.finish()
         elapsed = (time.time() - t0) * 1000
         interval = (time.time() - self.tprev) * 1000
         w, h = self.ui.window.get_size()
         self.tprev = time.time()
         self._vprint(f"rendering {w} x {h} pixels took {elapsed:.1f} ms, frame-to-frame interval was {interval:.1f} ms", log_level=2)
         return elapsed
 
+    def _gamut(self, imgidx):
+        """
+        Calculate per-color-channel scale factors as required by the shader for gamut
+        compression. The calculation is based on a user-defined 'power' controlling the
+        curve slope, and 'thr' and 'limit' values that are currently hardcoded at 0.8
+        and 1.2, respectively. Gamut distance values are compressed from [thr, lim] to
+        [thr, 1].
+        """
+        gamut_lim = self.files.metadata[imgidx]['gamut_bounds']  # per-channel limits
+        gamut_lim = np.clip(gamut_lim, 1.01, np.inf)  # >1.01 to ensure no overflows
+        scale = self._gamut_curve(self.ui.gamut_pow, self.ui.gamut_thr, gamut_lim)
+        return scale
+
     def _gamut_curve(self, power, thr, lim):
-        invp = 1 / power
-        src_domain = lim - thr  # range on the x axis to compress from; always > 0
-        dst_domain = 1.0 - thr  # range on the x axis to compress to; >= src_domain
-        rel_domain = src_domain / dst_domain  # always >= 1, typically 1..10
-        pow_domain = rel_domain ** power  # always >= 1, can be very large if p >> 1
-        pow_domain = (pow_domain - 1) ** invp  # ~rel_domain, if p >> 1 or lim >> 1
-        with np.errstate(divide="ignore"):  # divide-by-zero => inf, no warning
-            s = src_domain / pow_domain  # > dst_domain; ~dst_domain, if p >> 1 or lim >> 1
-        return s
-
-    def _fit_gamut(self, rgb):
-
-        # grayscale images have no color gamut
-
-        is_grayscale = rgb.ndim == 2 or rgb.shape[2] == 1
-        if is_grayscale:
-            max_dist = np.zeros(3)
-            return max_dist
-
-        # pick every Nth pixel to speed up processing for very large images;
-        # for example, a 100MP image will be downscaled by 8x in both x & y
-
-        magnitude = np.log10(rgb.size / 3)
-        N = max(np.rint(magnitude) - 5, 0)  # 0, 1, 2, 3
-        N = int(2 ** N)  # 1, 2, 4, 8
-        rgb = rgb[::N, ::N]  # 1MP => 2x, 10MP => 4x, 100MP => 8x
-
-        # convert to float32 to avoid overflows, underflows & dtype issues
-
-        rgb = rgb.astype(np.float32)
-
-        # distance is relative to per-pixel maximum color; >1.0 means out of gamut
-
-        max_rgb = np.max(rgb, axis=-1, keepdims=True)  # (H, W, 1)
-        valid = np.abs(max_rgb) > 0.0
-        zeros = np.zeros_like(rgb)  # (H, W, 3)
-        dist = np.divide(max_rgb - rgb, max_rgb, out=zeros, where=valid)
-
-        # determine the maximum distance from the gray axis that will be squeezed
-        # into gamut; colors further than that will remain out of gamut, but less
-        # than before
-
-        all_but_last = tuple(np.arange(rgb.ndim - 1))  # (0,) or (0, 1)
-        max_dist = np.max(dist, axis=all_but_last)  # global RGB-wise maximum
-        return max_dist
+        """
+        Calculate a curve shaping scale factor for each color channel, based on the given
+        power, threshold and limit.
+
+        Arguments:
+          - power: curve exponent; higher value = steeper curve
+          - thr: percentage of core gamut to leave unmodified
+          - lim: upper bound for values to compress into gamut
+
+        Returns:
+          - scale: compression curve global scale factor, required by the shader
+        """
+
+        assert np.all(thr <= 0.95), thr  # must be < 1.0 to avoid infs and nans
+        assert np.all(lim >= 1.01), lim  # must be > 1.0 to avoid infs and nans
+        assert np.all(thr >= 0.0), thr  # not strictly necessary, but helps range analysis
+        assert np.all(lim <= 3.0), lim  # not an exact bound, but safe at float32
+        assert np.all(power >= 1.0), power  # not an exact bound, but safe at float32
+        assert np.all(power <= 20.0), power  # not an exact bound, but safe at float32
+
+        # range analysis for inputs yielding the smallest scale (~0.05):
+        #   thr = 0.95
+        #   lim = 3.0
+        #   pow = 1.0
+        #   src_domain = 3.0 - 0.95 = 2.05
+        #   dst_domain = 1.0 - 0.95 = 0.05
+        #   rel_domain = 2.05 / 0.05 = 2.05 * 20 = 41
+        #   pow_domain = 41 ^ 1 = 41
+        #   ipow_domain = (41 - 1) ^ (1 / 1) = 40
+        #   scale = 2.05 / 40 = 0.05125 > 0.05 = dst_domain
+
+        # range analysis for inputs yielding the largest intermediate value (~1e32):
+        #   thr = 0.95
+        #   lim = 3.0
+        #   pow = 20.0
+        #   src_domain = 2.05
+        #   dst_domain = 0.05
+        #   rel_domain = 2.05 / 0.05 = 41
+        #   pow_domain = 41 ^ 20 < 1e33 < inf
+        #   ipow_domain = (41 ^ 20 - 1) / (1 / 20) ~ 41
+        #   scale = 2.05 / 41 = 0.05 = dst_domain
+
+        # range analysis for inputs minimizing ipow_domain (0.2):
+        #   thr = 0.95
+        #   lim = 1.01
+        #   pow = 1.0
+        #   src_domain = 1.01 - 0.95 = 0.06
+        #   dst_domain = 1.00 - 0.95 = 0.05
+        #   rel_domain = 0.06 / 0.05 = 1.2
+        #   pow_domain = 1.2 ^ 1 = 1.2
+        #   ipow_domain = 1.2 - 1 = 0.2
+        #   scale = 0.06 / 0.2 = 0.30 >> dst_domain
+
+        invp = 1 / power  # [1/20, 1]
+        src_domain = lim - thr  # range on the x axis to compress from; [0.06, 3.0]
+        dst_domain = 1.0 - thr  # range on the x axis to compress to; [0.05, 1.0]
+        rel_domain = src_domain / dst_domain  # [1.01, 41]
+        pow_domain = rel_domain ** power  # max = 41^20 < 1e33 < inf
+        ipow_domain = (pow_domain - 1) ** invp  # [0.01, 41]
+        scale = src_domain / ipow_domain  # [dst_domain, 101 * dst_domain]
+        assert np.all(1.01 * scale >= dst_domain), f"{1.01 * scale} vs. {dst_domain}"
+        return scale
 
     def _create_texture(self, img):
         # ModernGL texture dtypes that actually work:
         #   'f1': fixed-point [0, 1] internal format (GL_RGB8), uint8 input
         #   'f2': float16 internal format (GL_RGB16F), float16 input
         #   'f4': float32 internal format (GL_RGB32F), float32 input
         #
@@ -170,19 +202,17 @@
         return texture
 
     def _load_texture(self, idx):
         img = self.loader.get_image(idx)
         assert isinstance(img, (np.ndarray, str))
         if isinstance(img, np.ndarray):  # success
             texture = self._create_texture(img)
-            gamut_bounds = self._fit_gamut(img)
             self.files.textures[idx] = texture
-            self.files.metadata[idx] = {'gamut_bounds': gamut_bounds}
+            self.files.metadata[idx] = {'gamut_bounds': np.ones(3) * 1.2}
             self.loader.release_image(idx)
-            self._vprint(f"{self.files.filespecs[idx]} gamut extents = {gamut_bounds.round(3).tolist()}")
         else:  # PENDING | INVALID | RELEASED
             texture = self.files.textures[idx]
             if texture is None:
                 texture = self._create_dummy_texture()
                 self.files.textures[idx] = texture
                 self.files.metadata[idx] = {'gamut_bounds': np.ones(3)}
         if self.ui.texture_filter != "NEAREST":
```

### Comparing `glview-1.4.2/glview/glview.py` & `glview-1.5.0/glview/glview.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 The 'glview' command-line application.
 """
 
 import sys                     # built-in library
 import os                      # built-in library
 import time                    # built-in library
 import threading               # built-in library
+import numpy as np             # pip install numpy
 import natsort                 # pip install natsort
 import psutil                  # pip install psutil
 
 try:
     # package mode
     from glview import version        # local import
     from glview import argv           # local import
@@ -44,53 +45,57 @@
         self.orientations = [0] * self.numfiles
         self.images = ["PENDING"] * self.numfiles  # PENDING | RELEASED | INVALID
         self.textures = [None] * self.numfiles     # None | <Texture>
         self.metadata = [None] * self.numfiles
         self.is_url = [None] * self.numfiles
         self._update()
 
-    def remove(self, idx):
-        """ Remove the given image from this FileList, do not delete the file. """
+    def drop(self, indices):
+        """ Drop the given images from this FileList, do not delete the files. """
         with self.mutex:
             try:
-                self.filespecs.pop(idx)
-                self.orientations.pop(idx)
-                self.textures.pop(idx)
-                self.metadata.pop(idx)
-                self.images.pop(idx)
+                self.filespecs = self._drop(self.filespecs, indices)
+                self.orientations = self._drop(self.orientations, indices)
+                self.textures = self._drop(self.textures, indices)
+                self.metadata = self._drop(self.metadata, indices)
+                self.images = self._drop(self.images, indices)
                 self._update()
+                print(f"[{threading.current_thread().name}] Dropped images {indices}")
             except IndexError:
                 pass
 
     def delete(self, idx):
         """ Remove the given image from this FileList and delete the file from disk. """
         with self.mutex:
             try:
-                filespec = self.filespecs.pop(idx)
-                self.orientations.pop(idx)
-                self.textures.pop(idx)
-                self.metadata.pop(idx)
-                self.images.pop(idx)
-                self._update()
-                print(f"[{threading.current_thread().name}] Deleting {filespec}...")
+                filespec = self.filespecs[idx]
+                self.drop([idx])
                 os.remove(filespec)
+                print(f"[{threading.current_thread().name}] Deleted {filespec}")
             except IndexError:
                 pass
 
+    def _drop(self, arr, indices):
+        arr = np.asarray(arr, dtype=object)
+        arr = np.delete(arr, indices)
+        arr = arr.tolist()
+        return arr
+
     def _update(self):
         self.numfiles = len(self.filespecs)
         self.is_url = ["://" in f for f in self.filespecs]
 
 
 def main():
     """ Parse command-line arguments and run the application. """
     fullscreen = argv.exists("--fullscreen")
     numtiles = argv.intval("--split", default=1, accepted=[1, 2, 3, 4])
     url = argv.stringval("--url", default=None)
     smooth = argv.exists("--filter")
+    debug = argv.intval("--debug", default=1, accepted=[1, 2, 3])
     verbose = argv.exists("--verbose")
     verbose += argv.exists("--verbose")
     show_version = argv.exists("--version")
     show_help = argv.exists("--help")
     argv.exitIfAnyUnparsedOptions()
     if show_version:
         print(f"glview version {version.__version__}")
@@ -99,14 +104,15 @@
         print("Usage: glview [options] [image.(pgm|ppm|pnm|png|jpg|..)] ...")
         print()
         print("  options:")
         print("    --fullscreen            start in full-screen mode; default = windowed")
         print("    --split 1|2|3|4         display images in N separate tiles")
         print("    --url <address>         load image from the given web address")
         print("    --filter                use linear filtering; default = nearest")
+        print("    --debug N               select debug rendering mode; default = 1")
         print("    --verbose               print extra traces to the console")
         print("    --verbose               print even more traces to the console")
         print("    --version               show glview version number & exit")
         print("    --help                  show this help message")
         print()
         print("  runtime:")
         print("    mouse wheel             zoom in/out; synchronized if multiple tiles")
@@ -121,38 +127,45 @@
         print("    w                       write current tile(s) to a PNG")
         print("    h                       reset zoom/pan/exposure to initial state")
         print("    f                       toggle fullscreen <-> windowed")
         print("    t                       toggle nearest <-> linear filtering")
         print("    g                       toggle sRGB gamma correction on/off")
         print("    e                       slide exposure from -2EV to +2EV & back")
         print("    b                       toggle between HDR/LDR exposure control")
-        print("    c                       toggle gamut compression on/off")
+        print("    k                       toggle gamut compression on/off")
+        print("    c                       adjust gamut compression strength")
         print("    i                       print image information (EXIF)")
         print("    d                       drop the currently shown image")
         print("    del                     delete the currently shown image")
+        print("    space                   toggle debug rendering on/off")
         print("    q / esc / ctrl+c        terminate")
         print()
         print("  supported file types:")
         print("   ", '\n    '.join(IMAGE_TYPES))
         print()
+        print("  available debug rendering modes (--debug N):")
+        print("    1 - red => overexposed; blue => out of gamut; magenta => both")
+        print("    2 - shades of green => out-of-gamut distance")
+        print("    3 - normalized color: rgb' = rgb / max(rgb)")
+        print()
         print(f"  glview version {version.__version__}.")
         print()
         sys.exit(-1)
     else:
         print("See 'glview --help' for command-line options and keyboard commands.")
 
     filepatterns = sys.argv[1:] or url or ["*"]
     filenames = argv.filenames(filepatterns, IMAGE_TYPES, allowAllCaps=True)
     filenames = natsort.natsorted(filenames)
     filenames += [url] if url is not None else []
     numfiles = len(filenames)
     enforce(numfiles > 0, "No valid images to show. Terminating.")
 
     files = FileList(filenames)
-    ui = pygletui.PygletUI(files, bool(verbose))
+    ui = pygletui.PygletUI(files, debug, bool(verbose))
     loader = imageprovider.ImageProvider(files, bool(verbose))
     renderer = glrenderer.GLRenderer(ui, files, loader, verbose)
     ui.texture_filter = "LINEAR" if smooth else "NEAREST"
     ui.fullscreen = fullscreen
     ui.numtiles = numtiles
     ui.start(renderer)
     loader.start()
```

### Comparing `glview-1.4.2/glview/imageprovider.py` & `glview-1.5.0/glview/imageprovider.py`

 * *Files identical despite different names*

### Comparing `glview-1.4.2/glview/pygletui.py` & `glview-1.5.0/glview/pygletui.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 import numpy as np             # pip install numpy
 import imsize                  # pip install imsize
 
 
 class PygletUI:
     """ A graphical user interface for glview, based on Pyglet and ModernGL. """
 
-    def __init__(self, files, verbose=False):
+    def __init__(self, files, debug, verbose=False):
         """ Create a new PygletUI with the given (hardcoded) FileList instance. """
         self.thread_name = "UIThread"
+        self.debug_selected = debug  # selected debug rendering mode: 1|2|3|...
+        self.debug_mode = 0  # start in normal mode, toggle on/off with space
         self.verbose = verbose
         self.files = files
         self.fullscreen = False
         self.numtiles = 1
         self.running = None
         self.need_redraw = True
         self.was_resized = True
@@ -39,18 +41,18 @@
         self.renderer = None
         self.texture_filter = "NEAREST"
         self.img_per_tile = [0, 1, 2, 3]
         self.gamma = False
         self.ev_range = 2
         self.ev_linear = 0.0
         self.ev = 0.0
-        self.gamut = False
-        self.gamut_lim = np.ones(3)
-        self.gamut_thr = np.zeros(3)
-        self.gamut_power = np.ones(3)
+        self.gamut_fit = False  # on/off toggle
+        self.gamut_lin = 0.0  # adjusted dynamically
+        self.gamut_pow = np.ones(3)  # derived from self.gamut_lin
+        self.gamut_thr = np.ones(3) * 0.8  # hardcoded preset
 
     def start(self, renderer):
         """ Start the UI thread. """
         self._vprint(f"spawning {self.thread_name}...")
         self.renderer = renderer
         self.running = True
         self.ui_thread = threading.Thread(target=lambda: self._try(self._pyglet_runner), name=self.thread_name)
@@ -102,15 +104,15 @@
         self._setup_events()
         self.key_state = pyglet.window.key.KeyStateHandler()
         self.window.push_handlers(self.key_state)
         self._vprint("Pyglet & native OpenGL initialized")
 
     def _caption(self):
         fps = pyglet.clock.get_frequency()
-        gamut = "on" if self.gamut else "off"
+        gamut = "off" if not self.gamut_fit else f"p = {self.gamut_pow[0]:.1f}"
         caption = f"glview [{self.ev:+1.2f}EV | gamut fit {gamut} | {fps:.1f} fps]"
         for tileidx in range(self.numtiles):
             imgidx = self.img_per_tile[tileidx]
             basename = os.path.basename(self.files.filespecs[imgidx])
             caption = f"{caption} | {basename} [{imgidx+1}/{self.files.numfiles}]"
         return caption
 
@@ -164,32 +166,42 @@
             dxdy = dxdy * self.keyboard_pan_speed
             dxdy = dxdy / self.scale
             dxdy = dxdy / self.mouse_canvas_width
             self.mousepos = np.clip(self.mousepos + dxdy, -1.0, 1.0)
             if np.any(dxdy != 0.0) or self.scale != prev_scale:
                 self.need_redraw = True
 
+    def _triangle_wave(self, x, amplitude):
+        # [0, 1] => [-amplitude, +amplitude]
+        y = 4 * amplitude * np.abs((x - 0.25) % 1 - 0.5) - amplitude
+        return y
+
     def _smooth_exposure(self):
         # this is invoked 50 times per second, so exposure control is pretty fast
         keys = pyglet.window.key
-        def triangle_wave(x, amplitude):
-            # [0, 1] => [-amplitude, +amplitude]
-            y = 4 * amplitude * np.abs((x - 0.25) % 1 - 0.5) - amplitude
-            return y
         self.ev_linear += 0.005 * self.key_state[keys.E]
-        self.ev = triangle_wave(self.ev_linear, self.ev_range)
+        self.ev = self._triangle_wave(self.ev_linear, self.ev_range)
+        self.need_redraw = True
+
+    def _smooth_gamut_fit(self):
+        # this is invoked 50 times per second, so gamut fit control is pretty fast
+        keys = pyglet.window.key
+        self.gamut_lin += 0.005 * self.key_state[keys.C]
+        power = self._triangle_wave(self.gamut_lin, 2) + 3  # [0, 1] => [-2, 2] => [1, 5]
+        self.gamut_pow = np.ones(3) * power
         self.need_redraw = True
 
     def _setup_events(self):
         self._vprint("setting up Pyglet window event handlers...")
 
         @self.window.event
         def on_draw():
             self._keyboard_zoom_pan()
             self._smooth_exposure()
+            self._smooth_gamut_fit()
             if self.need_redraw:
                 self.renderer.redraw()
                 self.window.set_caption(self._caption())
                 self.window.flip()
                 if self.was_resized:
                     # ensure that both buffers (back & front) are filled
                     # with the same image after a resize event, or else
@@ -254,62 +266,69 @@
                     self.window.set_fullscreen(self.fullscreen)
                     self.window.set_mouse_visible(not self.fullscreen)
                     self.need_redraw = True
                 if symbol == keys.H:  # reset exposure + zoom & pan ("home")
                     self.scale = 1.0
                     self.mousepos = np.zeros(2)
                     self.ev_linear = 0.0
+                    self.gamut_lin = 0.0
+                    self.gamut_fit = False
                     self.need_redraw = True
                 if symbol == keys.G:  # gamma
                     self.gamma = not self.gamma
                     self.need_redraw = True
                 if symbol == keys.B:  # toggle between narrow/wide (LDR/HDR) exposure control
                     self.ev_range = (self.ev_range + 6) % 12
                     self.need_redraw = True
-                if symbol == keys.C:  # toggle gamut compression on/off
-                    self.gamut = not self.gamut
-                    self.gamut_lim = np.ones(3) * (2.0 if self.gamut else 1.0)
-                    self.gamut_thr = np.ones(3) * 0.5
-                    self.gamut_power = np.ones(3) * 10.0
+                if symbol == keys.K: # toggle gamut compression on/off
+                    self.gamut_fit = not self.gamut_fit
                     self.need_redraw = True
                 if symbol == keys.T:  # texture filtering
                     self.texture_filter = "LINEAR" if self.texture_filter == "NEAREST" else "NEAREST"
                     self.need_redraw = True
                 if symbol == keys.S:  # split
                     self.numtiles = (self.numtiles % 4) + 1
                     self.tileidx = min(self.tileidx, self.numtiles - 1)
                     self.img_per_tile = np.clip(self.img_per_tile, 0, self.files.numfiles - 1)
                     self.viewports = self._retile(self.numtiles, self.winsize)
                     self.window.set_caption(self._caption())
                     self.need_redraw = True
                 if symbol == keys.R:  # rotate
-                    imgidx = self.img_per_tile[self.tileidx]
-                    self.files.orientations[imgidx] += 90
-                    self.files.orientations[imgidx] %= 360
+                    for imgidx in self.img_per_tile[:self.numtiles]:
+                        self.files.orientations[imgidx] += 90
+                        self.files.orientations[imgidx] %= 360
                     self.need_redraw = True
                 if symbol == keys.I:  # image info
                     imgidx = self.img_per_tile[self.tileidx]
                     filespec = self.files.filespecs[imgidx]
                     fileinfo = imsize.read(filespec)
                     print(fileinfo)
                     self._print_exif(filespec)
-                if symbol in [keys.D, keys.DELETE]:  # drop and/or delete
-                    if self.numtiles == 1:  # only in single-tile mode
-                        imgidx = self.img_per_tile[self.tileidx]
-                        if symbol == keys.D:
-                            self.files.remove(imgidx)  # drop
-                        else:
-                            self.files.delete(imgidx)  # delete
-                        if self.files.numfiles == 0:
-                            self.running = False
-                            self.event_loop.has_exit = True
-                        else:
-                            self.img_per_tile[self.tileidx] = (imgidx - 1) % self.files.numfiles
-                            self.window.set_caption(self._caption())
-                            self.need_redraw = True
+                if symbol == keys.SPACE:  # toggle debug mode on/off
+                    N = self.debug_selected
+                    self.debug_mode = (self.debug_mode + N) % (N * 2)
+                    self._vprint(f"debug rendering mode {self.debug_mode}")
+                    self.need_redraw = True
+                if symbol in [keys.D, keys.DELETE]:
+                    if symbol == keys.D:  # drop
+                        indices = self.img_per_tile[:self.numtiles]
+                        self.files.drop(indices)
+                    if symbol == keys.DELETE:  # delete
+                        if self.numtiles == 1:  # only in single-tile mode
+                            imgidx = self.img_per_tile[self.tileidx]
+                            self.files.delete(imgidx)
+                    if self.files.numfiles == 0:
+                        self.running = False
+                        self.event_loop.has_exit = True
+                    else:
+                        N = self.numtiles
+                        visible_images = np.asarray(self.img_per_tile[:N]) - N
+                        self.img_per_tile[:N] = visible_images % self.files.numfiles
+                        self.window.set_caption(self._caption())
+                        self.need_redraw = True
                 # pylint: disable=protected-access
                 if symbol in [keys._1, keys._2, keys._3, keys._4]:
                     tileidx = symbol - keys._1
                     self.tileidx = tileidx if tileidx < self.numtiles else self.tileidx
                     self.need_redraw = True
 
         @self.window.event
```

### Comparing `glview-1.4.2/glview.egg-info/PKG-INFO` & `glview-1.5.0/glview.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: glview
-Version: 1.4.2
+Version: 1.5.0
 Summary: Lightning-fast image viewer with smooth zooming & panning.
 Home-page: http://github.com/toaarnio/glview
 Author: Tomi Aarnio
 Author-email: tomi.p.aarnio@gmail.com
 License: MIT
-Description: # glview
-        
-        [![Build Status](https://travis-ci.com/toaarnio/glview.svg?branch=master)](https://travis-ci.com/github/toaarnio/glview)
-        
-        Lightning-fast image viewer with smooth zooming &amp; panning + HDR exposure control.
-        
-        **Installing:**
-        ```
-        pip install glview
-        ```
-        
-        **Usage:**
-        ```
-        glview --help
-        ```
-        
-        **Building &amp; installing from source:**
-        ```
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# glview
+
+[![Build Status](https://travis-ci.com/toaarnio/glview.svg?branch=master)](https://travis-ci.com/github/toaarnio/glview)
+
+Lightning-fast image viewer with smooth zooming &amp; panning + HDR exposure control.
+
+**Installing:**
+```
+pip install glview
+```
+
+**Usage:**
+```
+glview --help
+```
+
+**Building &amp; installing from source:**
+```
+
+
```

### Comparing `glview-1.4.2/setup.py` & `glview-1.5.0/setup.py`

 * *Files identical despite different names*

