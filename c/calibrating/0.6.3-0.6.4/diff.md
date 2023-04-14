# Comparing `tmp/calibrating-0.6.3.tar.gz` & `tmp/calibrating-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/calibrating-0.6.3.tar", last modified: Mon Mar 20 13:07:14 2023, max compression
+gzip compressed data, was "dist/calibrating-0.6.4.tar", last modified: Fri Apr 14 07:58:52 2023, max compression
```

## Comparing `calibrating-0.6.3.tar` & `calibrating-0.6.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-03-20 13:07:14.000000 calibrating-0.6.3/
--rw-rw-r--   0 dl        (1000) dl        (1000)       35 2021-08-19 08:36:59.000000 calibrating-0.6.3/MANIFEST.in
--rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-03-20 13:07:14.000000 calibrating-0.6.3/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)     5544 2023-01-11 07:48:52.000000 calibrating-0.6.3/README.md
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-03-20 13:07:14.000000 calibrating-0.6.3/calibrating/
--rw-rw-r--   0 dl        (1000) dl        (1000)      643 2023-03-20 13:05:17.000000 calibrating-0.6.3/calibrating/__info__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      249 2022-12-22 13:24:45.000000 calibrating-0.6.3/calibrating/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    18302 2022-12-22 17:59:36.000000 calibrating-0.6.3/calibrating/boards.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    21801 2022-12-22 17:59:18.000000 calibrating-0.6.3/calibrating/camera.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     1521 2022-12-22 17:59:18.000000 calibrating-0.6.3/calibrating/feature_libs.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     4730 2023-02-07 10:00:28.000000 calibrating-0.6.3/calibrating/multi_boards.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     3200 2022-12-22 13:14:32.000000 calibrating-0.6.3/calibrating/reconstruction.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    21212 2023-03-20 13:05:47.000000 calibrating-0.6.3/calibrating/stereo.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    24603 2023-03-20 13:03:23.000000 calibrating-0.6.3/calibrating/utils.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-03-20 13:07:14.000000 calibrating-0.6.3/calibrating.egg-info/
--rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-03-20 13:07:14.000000 calibrating-0.6.3/calibrating.egg-info/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)      442 2023-03-20 13:07:14.000000 calibrating-0.6.3/calibrating.egg-info/SOURCES.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-03-20 13:07:14.000000 calibrating-0.6.3/calibrating.egg-info/dependency_links.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       54 2023-03-20 13:07:14.000000 calibrating-0.6.3/calibrating.egg-info/requires.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-03-20 13:07:14.000000 calibrating-0.6.3/calibrating.egg-info/top_level.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       54 2022-09-30 10:04:15.000000 calibrating-0.6.3/requirements.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-03-20 13:07:14.000000 calibrating-0.6.3/setup.cfg
--rw-rw-r--   0 dl        (1000) dl        (1000)      853 2021-08-19 08:44:30.000000 calibrating-0.6.3/setup.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-14 07:58:52.000000 calibrating-0.6.4/
+-rw-rw-r--   0 dl        (1000) dl        (1000)       35 2021-08-19 08:36:59.000000 calibrating-0.6.4/MANIFEST.in
+-rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-14 07:58:52.000000 calibrating-0.6.4/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)     5544 2023-01-11 07:48:52.000000 calibrating-0.6.4/README.md
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      643 2023-04-14 07:58:23.000000 calibrating-0.6.4/calibrating/__info__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      249 2022-12-22 13:24:45.000000 calibrating-0.6.4/calibrating/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    18329 2023-04-14 05:58:51.000000 calibrating-0.6.4/calibrating/boards.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    21801 2023-04-14 05:38:18.000000 calibrating-0.6.4/calibrating/camera.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1521 2022-12-22 17:59:18.000000 calibrating-0.6.4/calibrating/feature_libs.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     4730 2023-02-07 10:00:28.000000 calibrating-0.6.4/calibrating/multi_boards.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     3200 2022-12-22 13:14:32.000000 calibrating-0.6.4/calibrating/reconstruction.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    21305 2023-04-13 11:51:43.000000 calibrating-0.6.4/calibrating/stereo.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    25439 2023-04-14 05:50:57.000000 calibrating-0.6.4/calibrating/utils.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating.egg-info/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      647 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating.egg-info/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)      442 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating.egg-info/SOURCES.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating.egg-info/dependency_links.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       54 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating.egg-info/requires.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       12 2023-04-14 07:58:52.000000 calibrating-0.6.4/calibrating.egg-info/top_level.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       54 2022-09-30 10:04:15.000000 calibrating-0.6.4/requirements.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-04-14 07:58:52.000000 calibrating-0.6.4/setup.cfg
+-rw-rw-r--   0 dl        (1000) dl        (1000)      853 2021-08-19 08:44:30.000000 calibrating-0.6.4/setup.py
```

### Comparing `calibrating-0.6.3/PKG-INFO` & `calibrating-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrating
-Version: 0.6.3
+Version: 0.6.4
 Summary: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Home-page: https://github.com/DIYer22/calibrating
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Platform: UNKNOWN
```

### Comparing `calibrating-0.6.3/README.md` & `calibrating-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.3/calibrating/__info__.py` & `calibrating-0.6.4/calibrating/__info__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.3"
+__version__ = "0.6.4"
 __description__ = "Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python."
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `calibrating-0.6.3/calibrating/boards.py` & `calibrating-0.6.4/calibrating/boards.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,23 +222,25 @@
         self.object_points = dict(enumerate(self.all_object_points.reshape(-1, 4, 3)))
         self.aruco_dict_tag = cv2.aruco.DICT_6X6_250
         self.object_points = self.set_origin_to_center(self.object_points)
 
     def find_image_points(self, d):
         img = d["img"]
         gray = img if img.ndim == 2 else cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
-        parameters = cv2.aruco.DetectorParameters_create()
+        parameters = cv2.aruco.DetectorParameters()
         self.detector_parameters.setdefault("polygonalApproxAccuracyRate", 0.008)
         [
             setattr(parameters, key, value)
             for key, value in self.detector_parameters.items()
         ]
 
         d["corners"], d["ids"], rejectedImgPoints = cv2.aruco.detectMarkers(
-            gray, cv2.aruco.Dictionary_get(self.aruco_dict_tag), parameters=parameters
+            gray,
+            cv2.aruco.getPredefinedDictionary(self.aruco_dict_tag),
+            parameters=parameters,
         )
         d["valid"] = d["ids"] is not None and (
             len(d["ids"]) == len(self.object_points) or self.occlusion
         )
         if d["valid"]:
             d["ids"] = d["ids"][:, 0] if d["ids"].ndim == 2 else d["ids"]
             d["image_points"] = dict(
```

### Comparing `calibrating-0.6.3/calibrating/camera.py` & `calibrating-0.6.4/calibrating/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from glob import glob
 from tqdm import tqdm
 
 with boxx.inpkg():
     from . import utils
     from .stereo import Stereo
     from .__info__ import __version__
-    from .utils import r_t_to_T, intrinsic_format_conversion
+    from .utils import r_t_to_T, intrinsic_format_conversion, prepare_example_data_dir
     from .reconstruction import convert_cam_to_nerf_json
     from .boards import Chessboard, BaseBoard
 
 TEMP = __import__("tempfile").gettempdir()
 
 
 class Cam(dict):
@@ -506,46 +506,43 @@
         right_idx = -1
         while all([paths[0][right_idx] == path[right_idx] for path in paths]):
             right_idx -= 1
         return left_idx, right_idx + 1
 
     @staticmethod
     def get_test_cams():
-        root = os.path.abspath(
-            os.path.join(
-                __file__,
-                "../../../calibrating_example_data/paired_stereo_and_depth_cams_checkboard",
-            )
+        example_data_dir = os.path.join(
+            prepare_example_data_dir(), "paired_stereo_and_depth_cams_checkboard"
         )
         board = Chessboard(checkboard=(7, 10), size_mm=22.564)
         caml = Cam(
-            glob(os.path.join(root, "*", "stereo_l.jpg")),
+            glob(os.path.join(example_data_dir, "*", "stereo_l.jpg")),
             board,
             name="left",
             enable_cache=True,
         )
         camr = Cam(
-            glob(os.path.join(root, "*", "stereo_r.jpg")),
+            glob(os.path.join(example_data_dir, "*", "stereo_r.jpg")),
             board,
             name="right",
             enable_cache=True,
         )
         camd = Cam(
-            glob(os.path.join(root, "*", "depth_cam_color.jpg")),
+            glob(os.path.join(example_data_dir, "*", "depth_cam_color.jpg")),
             board,
             name="depth",
             enable_cache=True,
         )
         built_in_intrinsics = dict(
             fx=1474.1182177692722,
             fy=1474.125874583105,
             cx=1037.599716850734,
             cy=758.3072639103259,
         )
-        # depth need to be used in pairs with camera's built-in intrinsics
+        # depth need to be used in pairs with depth camera's built-in intrinsics
         camd.load(built_in_intrinsics)
         return caml, camr, camd
 
     @classmethod
     def get_example_720p(cls):
         return cls.load(
             dict(
```

### Comparing `calibrating-0.6.3/calibrating/feature_libs.py` & `calibrating-0.6.4/calibrating/feature_libs.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.3/calibrating/multi_boards.py` & `calibrating-0.6.4/calibrating/multi_boards.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.3/calibrating/reconstruction.py` & `calibrating-0.6.4/calibrating/reconstruction.py`

 * *Files identical despite different names*

### Comparing `calibrating-0.6.3/calibrating/stereo.py` & `calibrating-0.6.4/calibrating/stereo.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,16 @@
         self._get_undistort_rectify_map()
 
     def get_conjoint_points(self):
         for d in self.cam1.values():
             if "image_points" in d:
                 image_points = d["image_points"]
                 break
+        else:
+            raise AssertionError("No valid image that could det image_points")
         # "image_points" is checkboard type: shape(n, 2)
         if isinstance(image_points, np.ndarray):
             keys = self.cam1.valid_keys_intersection(self.cam2)
             conjoint_image_points1 = [self.cam1[key]["image_points"] for key in keys]
             conjoint_image_points2 = [self.cam2[key]["image_points"] for key in keys]
             conjoint_object_points = [self.cam1[key]["object_points"] for key in keys]
 
@@ -240,15 +242,15 @@
         if hasattr(self, "cam1"):
             self.cam1.load(dic.pop("cam1"))
             self.cam2.load(dic.pop("cam2"))
         else:
             self.cam1 = Cam.load(dic.pop("cam1"))
             self.cam2 = Cam.load(dic.pop("cam2"))
         self.__dict__.update(
-            {k: np.array(v) if k in self.DUMP_ATTRS else v for k, v in dic.items()}
+            {k: boxx.npa(v) if k in self.DUMP_ATTRS else v for k, v in dic.items()}
         )
         self._get_undistort_rectify_map()
         return self
 
     def copy(self):
         new = type(self)()
         new.load(self.dump())
```

### Comparing `calibrating-0.6.3/calibrating/utils.py` & `calibrating-0.6.4/calibrating/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import time
 import boxx
 import numpy as np
 from glob import glob
 from boxx import imread, imsave, shows, show, showb, tree, loga, pi
 
 inv = np.linalg.inv
+eps = 1e-8
 
 
 def R_t_to_T(R, t=None):
     if t is None:
         t = np.zeros((3,))
     T = np.zeros((4, 4))
     T[:3, :3] = R
@@ -81,15 +82,15 @@
 def project_vec_on_plane(v, plane_v):
     return v - np.dot(v, plane_v) / (np.linalg.norm(plane_v) ** 2) * plane_v
 
 
 def rotate_shortest_of_two_vecs(v1, v2, return_rodrigues=False):
     cross = np.cross(v1, v2)
     rad = np.arccos((v1 * v2).sum() / np.linalg.norm(v1) / np.linalg.norm(v2))
-    r = rad * cross / np.linalg.norm(cross)
+    r = rad * cross / (np.linalg.norm(cross) + eps)
     if return_rodrigues:
         return r
     return cv2.Rodrigues(r)[0]
 
 
 def apply_T_to_point_cloud(T, point_cloud):
     """
@@ -584,42 +585,59 @@
     )
     viss = [vis[:y, :x], vis[:y, x:], vis[y:, :x], vis[y:, x:]]
     if shows:
         boxx.shows(viss)
     return viss
 
 
+def prepare_example_data_dir():
+    example_data_dir = os.path.abspath(
+        os.path.join(
+            __file__,
+            "../../../calibrating_example_data",
+        )
+    )
+    if not os.path.exists(example_data_dir):
+        example_data_dir = os.path.join(
+            __import__("tempfile").gettempdir(), "calibrating_example_data"
+        )
+        if not os.path.exists(example_data_dir):
+            cmd = f"git clone https://github.com/yl-data/calibrating_example_data '{example_data_dir}' --depth 1"
+            print(
+                f"INFO from calibrating: \n\tThe calibrating_example_data does not exist. \n\tThe example_data will be automatically cloned which may take a few minutes. \n\tThe following command will be executed: \n\t\t{cmd}"
+            )
+            assert not os.system(cmd), cmd
+    return example_data_dir
+
+
 def get_test_cams(feature_type="checkboard"):
     from calibrating import Cam, PredifinedArucoBoard1
 
     if feature_type == "checkboard":
         caml, camr, camd = Cam.get_test_cams()
         return dict(caml=caml, camr=camr, camd=camd)
     elif feature_type == "aruco":
-        root = os.path.abspath(
-            os.path.join(
-                __file__,
-                "../../../calibrating_example_data/paired_stereo_and_depth_cams_aruco",
-            )
+        example_data_dir = os.path.join(
+            prepare_example_data_dir(), "paired_stereo_and_depth_cams_aruco"
         )
         board = PredifinedArucoBoard1()
         caml = Cam(
-            glob(os.path.join(root, "*", "stereo_l.jpg")),
+            glob(os.path.join(example_data_dir, "*", "stereo_l.jpg")),
             board,
             name="caml",
             enable_cache=True,
         )
         camr = Cam(
-            glob(os.path.join(root, "*", "stereo_r.jpg")),
+            glob(os.path.join(example_data_dir, "*", "stereo_r.jpg")),
             board,
             name="camr",
             enable_cache=True,
         )
         camd = Cam(
-            glob(os.path.join(root, "*", "depth_cam_color.jpg")),
+            glob(os.path.join(example_data_dir, "*", "depth_cam_color.jpg")),
             board,
             name="camd",
             enable_cache=True,
         )
         built_in_intrinsics = dict(
             fx=1474.1182177692722,
             fy=1474.125874583105,
```

### Comparing `calibrating-0.6.3/calibrating.egg-info/PKG-INFO` & `calibrating-0.6.4/calibrating.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrating
-Version: 0.6.3
+Version: 0.6.4
 Summary: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Home-page: https://github.com/DIYer22/calibrating
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: Calibrate camera's intrinsic/extristric, and build stereo depth camera with OpenCV python.
 Platform: UNKNOWN
```

### Comparing `calibrating-0.6.3/setup.py` & `calibrating-0.6.4/setup.py`

 * *Files identical despite different names*

