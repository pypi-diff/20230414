# Comparing `tmp/asrl-pyboreas-1.0.4.tar.gz` & `tmp/asrl-pyboreas-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asrl-pyboreas-1.0.4.tar", last modified: Thu Nov 25 01:16:17 2021, max compression
+gzip compressed data, was "asrl-pyboreas-1.0.5.tar", last modified: Thu Apr 13 22:25:56 2023, max compression
```

## Comparing `asrl-pyboreas-1.0.4.tar` & `asrl-pyboreas-1.0.5.tar`

### file list

```diff
@@ -1,40 +1,46 @@
-drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2021-11-25 01:16:17.758226 asrl-pyboreas-1.0.4/
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     1544 2021-06-10 18:13:11.000000 asrl-pyboreas-1.0.4/LICENSE
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     7015 2021-11-25 01:16:17.758226 asrl-pyboreas-1.0.4/PKG-INFO
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     6588 2021-11-22 04:21:06.000000 asrl-pyboreas-1.0.4/README.md
-drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2021-11-25 01:16:17.754226 asrl-pyboreas-1.0.4/asrl_pyboreas.egg-info/
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     7015 2021-11-25 01:16:17.000000 asrl-pyboreas-1.0.4/asrl_pyboreas.egg-info/PKG-INFO
--rw-rw-r--   0 keenan    (1000) keenan    (1000)      796 2021-11-25 01:16:17.000000 asrl-pyboreas-1.0.4/asrl_pyboreas.egg-info/SOURCES.txt
--rw-rw-r--   0 keenan    (1000) keenan    (1000)        1 2021-11-25 01:16:17.000000 asrl-pyboreas-1.0.4/asrl_pyboreas.egg-info/dependency_links.txt
--rw-rw-r--   0 keenan    (1000) keenan    (1000)      126 2021-11-25 01:16:17.000000 asrl-pyboreas-1.0.4/asrl_pyboreas.egg-info/requires.txt
--rw-rw-r--   0 keenan    (1000) keenan    (1000)        9 2021-11-25 01:16:17.000000 asrl-pyboreas-1.0.4/asrl_pyboreas.egg-info/top_level.txt
-drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2021-11-25 01:16:17.754226 asrl-pyboreas-1.0.4/pyboreas/
--rw-rw-r--   0 keenan    (1000) keenan    (1000)       33 2021-10-08 02:02:35.000000 asrl-pyboreas-1.0.4/pyboreas/__init__.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     2487 2021-10-29 02:55:00.000000 asrl-pyboreas-1.0.4/pyboreas/boreas.py
-drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2021-11-25 01:16:17.754226 asrl-pyboreas-1.0.4/pyboreas/data/
--rw-rw-r--   0 keenan    (1000) keenan    (1000)        0 2021-10-08 02:02:35.000000 asrl-pyboreas-1.0.4/pyboreas/data/__init__.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     8459 2021-11-25 01:07:45.000000 asrl-pyboreas-1.0.4/pyboreas/data/bounding_boxes.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)      772 2021-10-18 20:19:56.000000 asrl-pyboreas-1.0.4/pyboreas/data/calib.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     6247 2021-11-23 00:15:21.000000 asrl-pyboreas-1.0.4/pyboreas/data/pointcloud.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     6102 2021-11-25 00:20:24.000000 asrl-pyboreas-1.0.4/pyboreas/data/sensors.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     8823 2021-11-24 23:20:38.000000 asrl-pyboreas-1.0.4/pyboreas/data/sequence.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     5560 2021-11-24 21:48:54.000000 asrl-pyboreas-1.0.4/pyboreas/data/splits.py
-drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2021-11-25 01:16:17.758226 asrl-pyboreas-1.0.4/pyboreas/eval/
--rw-rw-r--   0 keenan    (1000) keenan    (1000)        0 2021-10-18 00:24:17.000000 asrl-pyboreas-1.0.4/pyboreas/eval/__init__.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     2435 2021-11-25 01:14:24.000000 asrl-pyboreas-1.0.4/pyboreas/eval/odometry_benchmark.py
-drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2021-11-25 01:16:17.758226 asrl-pyboreas-1.0.4/pyboreas/test/
--rw-rw-r--   0 keenan    (1000) keenan    (1000)        0 2021-10-18 00:24:17.000000 asrl-pyboreas-1.0.4/pyboreas/test/__init__.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     4403 2021-11-25 01:14:24.000000 asrl-pyboreas-1.0.4/pyboreas/test/test_odometry.py
-drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2021-11-25 01:16:17.758226 asrl-pyboreas-1.0.4/pyboreas/utils/
--rw-rw-r--   0 keenan    (1000) keenan    (1000)        0 2021-10-08 02:02:35.000000 asrl-pyboreas-1.0.4/pyboreas/utils/__init__.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)    26297 2021-11-25 01:14:24.000000 asrl-pyboreas-1.0.4/pyboreas/utils/odometry.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     4773 2021-11-09 04:42:50.000000 asrl-pyboreas-1.0.4/pyboreas/utils/radar.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)    12244 2021-11-25 00:22:44.000000 asrl-pyboreas-1.0.4/pyboreas/utils/utils.py
-drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2021-11-25 01:16:17.758226 asrl-pyboreas-1.0.4/pyboreas/vis/
--rw-rw-r--   0 keenan    (1000) keenan    (1000)        0 2021-10-08 02:02:35.000000 asrl-pyboreas-1.0.4/pyboreas/vis/__init__.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     2216 2021-11-22 04:21:06.000000 asrl-pyboreas-1.0.4/pyboreas/vis/map_utils.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     3954 2021-11-08 21:44:57.000000 asrl-pyboreas-1.0.4/pyboreas/vis/plot_processed_error.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)     5957 2021-11-22 21:58:37.000000 asrl-pyboreas-1.0.4/pyboreas/vis/vis_utils.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)    16784 2021-11-22 04:21:06.000000 asrl-pyboreas-1.0.4/pyboreas/vis/visualizer.py
--rw-rw-r--   0 keenan    (1000) keenan    (1000)       38 2021-11-25 01:16:17.758226 asrl-pyboreas-1.0.4/setup.cfg
--rw-rw-r--   0 keenan    (1000) keenan    (1000)      887 2021-11-25 01:11:37.000000 asrl-pyboreas-1.0.4/setup.py
+drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2023-04-13 22:25:56.862415 asrl-pyboreas-1.0.5/
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     1544 2021-06-10 18:13:11.000000 asrl-pyboreas-1.0.5/LICENSE
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     6232 2023-04-13 22:25:56.862415 asrl-pyboreas-1.0.5/PKG-INFO
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     5805 2023-04-13 16:31:29.000000 asrl-pyboreas-1.0.5/README.md
+drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2023-04-13 22:25:56.854415 asrl-pyboreas-1.0.5/asrl_pyboreas.egg-info/
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     6232 2023-04-13 22:25:56.000000 asrl-pyboreas-1.0.5/asrl_pyboreas.egg-info/PKG-INFO
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)      972 2023-04-13 22:25:56.000000 asrl-pyboreas-1.0.5/asrl_pyboreas.egg-info/SOURCES.txt
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)        1 2023-04-13 22:25:56.000000 asrl-pyboreas-1.0.5/asrl_pyboreas.egg-info/dependency_links.txt
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)       76 2023-04-13 22:25:56.000000 asrl-pyboreas-1.0.5/asrl_pyboreas.egg-info/requires.txt
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)        9 2023-04-13 22:25:56.000000 asrl-pyboreas-1.0.5/asrl_pyboreas.egg-info/top_level.txt
+drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2023-04-13 22:25:56.854415 asrl-pyboreas-1.0.5/pyboreas/
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)       33 2021-10-08 02:02:35.000000 asrl-pyboreas-1.0.5/pyboreas/__init__.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     2237 2023-04-13 22:20:15.000000 asrl-pyboreas-1.0.5/pyboreas/boreas.py
+drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2023-04-13 22:25:56.858415 asrl-pyboreas-1.0.5/pyboreas/data/
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)        0 2021-10-08 02:02:35.000000 asrl-pyboreas-1.0.5/pyboreas/data/__init__.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     9504 2023-04-13 16:28:17.000000 asrl-pyboreas-1.0.5/pyboreas/data/bounding_boxes.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     1044 2023-04-13 22:20:15.000000 asrl-pyboreas-1.0.5/pyboreas/data/calib.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     6214 2023-04-13 16:47:15.000000 asrl-pyboreas-1.0.5/pyboreas/data/pointcloud.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     6387 2023-04-13 16:47:04.000000 asrl-pyboreas-1.0.5/pyboreas/data/sensors.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     9807 2023-04-13 22:20:15.000000 asrl-pyboreas-1.0.5/pyboreas/data/sequence.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     6473 2023-04-13 16:28:50.000000 asrl-pyboreas-1.0.5/pyboreas/data/splits.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     1880 2023-04-13 17:33:45.000000 asrl-pyboreas-1.0.5/pyboreas/download_task.py
+drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2023-04-13 22:25:56.858415 asrl-pyboreas-1.0.5/pyboreas/eval/
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)        0 2021-10-18 00:24:17.000000 asrl-pyboreas-1.0.5/pyboreas/eval/__init__.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     9809 2023-04-13 16:28:06.000000 asrl-pyboreas-1.0.5/pyboreas/eval/detection.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     1788 2023-04-13 16:28:07.000000 asrl-pyboreas-1.0.5/pyboreas/eval/interpolate.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     7500 2023-04-13 16:44:09.000000 asrl-pyboreas-1.0.5/pyboreas/eval/localization.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     1405 2023-04-13 16:28:13.000000 asrl-pyboreas-1.0.5/pyboreas/eval/odometry.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     5917 2023-04-13 16:47:36.000000 asrl-pyboreas-1.0.5/pyboreas/eval/odometry_aeva.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     4395 2023-04-13 16:28:14.000000 asrl-pyboreas-1.0.5/pyboreas/eval/submission_checker.py
+drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2023-04-13 22:25:56.858415 asrl-pyboreas-1.0.5/pyboreas/test/
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)        0 2021-10-18 00:24:17.000000 asrl-pyboreas-1.0.5/pyboreas/test/__init__.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     3832 2023-04-13 16:39:54.000000 asrl-pyboreas-1.0.5/pyboreas/test/test_localization.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     4664 2023-04-13 02:47:13.000000 asrl-pyboreas-1.0.5/pyboreas/test/test_odometry.py
+drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2023-04-13 22:25:56.862415 asrl-pyboreas-1.0.5/pyboreas/utils/
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)        0 2021-10-08 02:02:35.000000 asrl-pyboreas-1.0.5/pyboreas/utils/__init__.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     6035 2023-04-13 02:47:27.000000 asrl-pyboreas-1.0.5/pyboreas/utils/lgmath.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)    34791 2023-04-13 16:55:52.000000 asrl-pyboreas-1.0.5/pyboreas/utils/odometry.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     4830 2023-04-13 02:49:08.000000 asrl-pyboreas-1.0.5/pyboreas/utils/radar.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)    10861 2023-04-13 16:32:09.000000 asrl-pyboreas-1.0.5/pyboreas/utils/utils.py
+drwxrwxr-x   0 keenan    (1000) keenan    (1000)        0 2023-04-13 22:25:56.862415 asrl-pyboreas-1.0.5/pyboreas/vis/
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)        0 2021-10-08 02:02:35.000000 asrl-pyboreas-1.0.5/pyboreas/vis/__init__.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     3802 2023-04-13 02:49:38.000000 asrl-pyboreas-1.0.5/pyboreas/vis/plot_processed_error.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)     6200 2023-04-13 16:27:23.000000 asrl-pyboreas-1.0.5/pyboreas/vis/vis_utils.py
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)       38 2023-04-13 22:25:56.862415 asrl-pyboreas-1.0.5/setup.cfg
+-rw-rw-r--   0 keenan    (1000) keenan    (1000)      788 2023-04-13 22:23:49.000000 asrl-pyboreas-1.0.5/setup.py
```

### Comparing `asrl-pyboreas-1.0.4/LICENSE` & `asrl-pyboreas-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asrl-pyboreas-1.0.4/PKG-INFO` & `asrl-pyboreas-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,92 @@
 Metadata-Version: 2.1
 Name: asrl-pyboreas
-Version: 1.0.4
+Version: 1.0.5
 Summary: A toolkit for working with the Boreas dataset in Python
 Home-page: https://github.com/utiasASRL/boreas-devkit
 Author: Keenan Burnett, Andrew Li, Shichen Lu, Jingxing Qian, Yuchen Wu, David Yoon
 Author-email: boreas@robotics.utias.utoronto.ca
 License: BSD
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyboreas
+
 ![Boreas](https://github.com/utiasASRL/pyboreas/blob/master/pyboreas/figs/pyboreas.png)
 
-This devkit provides tools for working with the Boreas Dataset, an all-weather autonomous driving dataset which includes a 128-beam Velodyne Alpha-Prime lidar, a 5MP Blackfly camera, a 360 degree Navtech radar, and post-processed Applanix POS LV GNSS data. Our dataset currently suports benchmarking odometry. We are working towards providing an online benchmark for odometry, localization, and more. We plan to provide an HD map of each driven route. We are also in the process of acquiring 3D labels and hope to be able to provide a challenging object detection benchmark in the future.
+This devkit provides tools for working with the Boreas Dataset, an all-weather autonomous driving dataset which includes a 128-beam Velodyne Alpha-Prime lidar, a 5MP Blackfly camera, a 360 degree Navtech radar, and post-processed Applanix POS LV GNSS data. Our dataset currently suports benchmarking odometry, localization, and 3D object detection.
+
+Our leaderboard is now live! Baseline implementations for each leaderboard are coming soon.
+
+If you find our dataset useful in your research, please cite our dataset paper:
+
+[Boreas: A Multi-Season Autonomous Driving Dataset](https://arxiv.org/abs/2203.10168)
+
+```
+@article{burnett_ijrr23,
+author = {Keenan Burnett and David J Yoon and Yuchen Wu and Andrew Z Li and Haowei Zhang and Shichen Lu and Jingxing Qian and Wei-Kang Tseng and Andrew Lambert and Keith YK Leung and Angela P Schoellig and Timothy D Barfoot},
+title ={Boreas: A multi-season autonomous driving dataset},
+journal = {The International Journal of Robotics Research},
+volume = {42},
+number = {1-2},
+pages = {33-42},
+year = {2023},
+doi = {10.1177/02783649231160195},
+}
 
-Please note that our website is currently under construction. A live benchmark and a browser for downloading sequences will be available via the website soon.
+```
 
 ## Installation
 
 ### Using pip
+
 ```
 pip install asrl-pyboreas
 ```
 
 ### From source
+
 ```
 git clone https://github.com/utiasASRL/pyboreas.git
 pip install -e pyboreas
 ```
 
 ## Download Instructions
-1. [Create an AWS account (optional)](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)
+
+1. [Create an AWS account (OPTIONAL)](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)
 2. [Install the AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
 3. Create a `root` folder to store the dataset, example: `/path/to/data/boreas/` Each sequence will then be a folder under `root`.
-4. Use the AWS CLI to download either the entire dataset or only the desired sequences and sensors. Add `--no-sign-request` after each of the following commands if you're not going to use an AWS account. For example, the following command will download the entire Boreas dataset:
+4. Use the AWS CLI to download either the entire dataset or only the desired sequences and sensors.
+
+**Don't have an AWS Account?** Add `--no-sign-request` after each AWS CLI command.
+
+The following command will download the entire Boreas dataset:
 
-```bash
+```text
 root=/path/to/data/boreas/
 aws s3 sync s3://boreas $root
 ```
 
 The following command will list all the top-level prefixes (sequences):
 
-```bash
+```text
 root=/path/to/data/boreas/
 aws s3 ls s3://boreas
 ```
 
 Alternatively, [boreas.utias.utoronto.ca (Work In Progress)](https://www.boreas.utias.utoronto.ca/#/download) can be used to browse through sequences so as to pick and choose what data to download. The website will then generate a list of AWS CLI commands that can be run as a bash script. These commands will look something like:
 
-```bash
+```text
 root=/path/to/data/boreas/
 cd $root
 aws s3 sync s3://boreas/boreas-2020-11-26-13-58 boreas-2020-11-26-13-58 --exclude "*" \
-    --include "lidar/" --include "radar/" \
-    --include "applanix/" --include "calib/"
+    --include "lidar/*" --include "radar/*" \
+    --include "applanix/*" --include "calib/*"
 ```
 
 ## Example Usage
 
 ```Python
 import numpy as np
 from pyboreas import BoreasDataset
@@ -113,48 +139,22 @@
 # (4x4 homogeneous transform) wrt a global coordinate frame (ENU),
 # and groundtruth velocity information. Unless it's a part of the test set,
 # in that case, ground truth poses will be missing. However we still provide IMU
 # data (in the applanix frame) through the imu.csv files.
 lidar_frame = bd.get_lidar(0)
 t = lidar_frame.timestamp  # timestamp in seconds
 T_enu_lidar = lidar_frame.pose  # 4x4 homogenous transform [R t; 0 0 0 1]
-vbar = lidar_frame.velocity  # 6x1 vel in ENU frame [v_se_in_e; w_se_in_e] 
+vbar = lidar_frame.velocity  # 6x1 vel in ENU frame [v_se_in_e; w_se_in_e]
 varpi = lidar_frame.body_rate  # 6x1 vel in sensor frame [v_se_in_s; w_se_in_s]
 ```
-## Data Visualizer
-We provide a tool for visualization of sequence frames. Currently, the visualizer supports BEV lidar visualization, BEV radar visualization, Perspective camera + lidar visualization, and 3D lidar point visualization.
 
-```Python
-from pyboreas import BoreasDataset
-from pyboreas.vis.visualizer import BoreasVisualizer
-
-root = '/path/to/data/boreas/'
-bd = BoreasDataset(root)
-seq = bd.sequences[0]
-
-bv = BoreasVisualizer(seq)
-bv.visualize(starting_frame_idx=0)
-```
-Running the above code will start a local web server that visualizes the selected sequence.
-```
-Dash is running on http://127.0.0.1:8050/
-
- * Serving Flask app 'pyboreas.vis.visualizer' (lazy loading)
- * Environment: production
-   WARNING: This is a development server. Do not use it in a production deployment.
-   Use a production WSGI server instead.
- * Debug mode: off
- * Running on http://127.0.0.1:8050/ (Press CTRL+C to quit)
-```
-Open a web browser and navigate to the provided ip (in this case 127.0.0.1:8050) to view the sequence visualization.
 ## Tutorials
+
 Note that we provide a few simple tutorials for getting started with the Boreas dataset. Also note that we provide instructions for using this dataset using an AWS SageMaker instance, instructions at: pyboreas/tutorials/aws/README.md.
 
 **NOTE:** ground truth poses have dtype=np.float64, but PyTorch defaults to float32. Avoid using implicit type conversion as this will result in significant quantization error. Implicit conversion is only safe when the translation values are small, such as a pose with respect to a sensor frame or with respect to a starting position, but NOT with respect to ENU (very large).
 
 TODO:
-- Tutorials (pose interp)
-- Ground plane removal
+
 - Pointcloud voxelization
-- 3D Bounding boxes
```

### Comparing `asrl-pyboreas-1.0.4/README.md` & `asrl-pyboreas-1.0.5/asrl_pyboreas.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,92 @@
+Metadata-Version: 2.1
+Name: asrl-pyboreas
+Version: 1.0.5
+Summary: A toolkit for working with the Boreas dataset in Python
+Home-page: https://github.com/utiasASRL/boreas-devkit
+Author: Keenan Burnett, Andrew Li, Shichen Lu, Jingxing Qian, Yuchen Wu, David Yoon
+Author-email: boreas@robotics.utias.utoronto.ca
+License: BSD
+Platform: UNKNOWN
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pyboreas
+
 ![Boreas](https://github.com/utiasASRL/pyboreas/blob/master/pyboreas/figs/pyboreas.png)
 
-This devkit provides tools for working with the Boreas Dataset, an all-weather autonomous driving dataset which includes a 128-beam Velodyne Alpha-Prime lidar, a 5MP Blackfly camera, a 360 degree Navtech radar, and post-processed Applanix POS LV GNSS data. Our dataset currently suports benchmarking odometry. We are working towards providing an online benchmark for odometry, localization, and more. We plan to provide an HD map of each driven route. We are also in the process of acquiring 3D labels and hope to be able to provide a challenging object detection benchmark in the future.
+This devkit provides tools for working with the Boreas Dataset, an all-weather autonomous driving dataset which includes a 128-beam Velodyne Alpha-Prime lidar, a 5MP Blackfly camera, a 360 degree Navtech radar, and post-processed Applanix POS LV GNSS data. Our dataset currently suports benchmarking odometry, localization, and 3D object detection.
+
+Our leaderboard is now live! Baseline implementations for each leaderboard are coming soon.
+
+If you find our dataset useful in your research, please cite our dataset paper:
+
+[Boreas: A Multi-Season Autonomous Driving Dataset](https://arxiv.org/abs/2203.10168)
+
+```
+@article{burnett_ijrr23,
+author = {Keenan Burnett and David J Yoon and Yuchen Wu and Andrew Z Li and Haowei Zhang and Shichen Lu and Jingxing Qian and Wei-Kang Tseng and Andrew Lambert and Keith YK Leung and Angela P Schoellig and Timothy D Barfoot},
+title ={Boreas: A multi-season autonomous driving dataset},
+journal = {The International Journal of Robotics Research},
+volume = {42},
+number = {1-2},
+pages = {33-42},
+year = {2023},
+doi = {10.1177/02783649231160195},
+}
 
-Please note that our website is currently under construction. A live benchmark and a browser for downloading sequences will be available via the website soon.
+```
 
 ## Installation
 
 ### Using pip
+
 ```
 pip install asrl-pyboreas
 ```
 
 ### From source
+
 ```
 git clone https://github.com/utiasASRL/pyboreas.git
 pip install -e pyboreas
 ```
 
 ## Download Instructions
-1. [Create an AWS account (optional)](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)
+
+1. [Create an AWS account (OPTIONAL)](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)
 2. [Install the AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
 3. Create a `root` folder to store the dataset, example: `/path/to/data/boreas/` Each sequence will then be a folder under `root`.
-4. Use the AWS CLI to download either the entire dataset or only the desired sequences and sensors. Add `--no-sign-request` after each of the following commands if you're not going to use an AWS account. For example, the following command will download the entire Boreas dataset:
+4. Use the AWS CLI to download either the entire dataset or only the desired sequences and sensors.
 
-```bash
+**Don't have an AWS Account?** Add `--no-sign-request` after each AWS CLI command.
+
+The following command will download the entire Boreas dataset:
+
+```text
 root=/path/to/data/boreas/
 aws s3 sync s3://boreas $root
 ```
 
 The following command will list all the top-level prefixes (sequences):
 
-```bash
+```text
 root=/path/to/data/boreas/
 aws s3 ls s3://boreas
 ```
 
 Alternatively, [boreas.utias.utoronto.ca (Work In Progress)](https://www.boreas.utias.utoronto.ca/#/download) can be used to browse through sequences so as to pick and choose what data to download. The website will then generate a list of AWS CLI commands that can be run as a bash script. These commands will look something like:
 
-```bash
+```text
 root=/path/to/data/boreas/
 cd $root
 aws s3 sync s3://boreas/boreas-2020-11-26-13-58 boreas-2020-11-26-13-58 --exclude "*" \
-    --include "lidar/" --include "radar/" \
-    --include "applanix/" --include "calib/"
+    --include "lidar/*" --include "radar/*" \
+    --include "applanix/*" --include "calib/*"
 ```
 
 ## Example Usage
 
 ```Python
 import numpy as np
 from pyboreas import BoreasDataset
@@ -100,46 +139,22 @@
 # (4x4 homogeneous transform) wrt a global coordinate frame (ENU),
 # and groundtruth velocity information. Unless it's a part of the test set,
 # in that case, ground truth poses will be missing. However we still provide IMU
 # data (in the applanix frame) through the imu.csv files.
 lidar_frame = bd.get_lidar(0)
 t = lidar_frame.timestamp  # timestamp in seconds
 T_enu_lidar = lidar_frame.pose  # 4x4 homogenous transform [R t; 0 0 0 1]
-vbar = lidar_frame.velocity  # 6x1 vel in ENU frame [v_se_in_e; w_se_in_e] 
+vbar = lidar_frame.velocity  # 6x1 vel in ENU frame [v_se_in_e; w_se_in_e]
 varpi = lidar_frame.body_rate  # 6x1 vel in sensor frame [v_se_in_s; w_se_in_s]
 ```
-## Data Visualizer
-We provide a tool for visualization of sequence frames. Currently, the visualizer supports BEV lidar visualization, BEV radar visualization, Perspective camera + lidar visualization, and 3D lidar point visualization.
 
-```Python
-from pyboreas import BoreasDataset
-from pyboreas.vis.visualizer import BoreasVisualizer
-
-root = '/path/to/data/boreas/'
-bd = BoreasDataset(root)
-seq = bd.sequences[0]
-
-bv = BoreasVisualizer(seq)
-bv.visualize(starting_frame_idx=0)
-```
-Running the above code will start a local web server that visualizes the selected sequence.
-```
-Dash is running on http://127.0.0.1:8050/
-
- * Serving Flask app 'pyboreas.vis.visualizer' (lazy loading)
- * Environment: production
-   WARNING: This is a development server. Do not use it in a production deployment.
-   Use a production WSGI server instead.
- * Debug mode: off
- * Running on http://127.0.0.1:8050/ (Press CTRL+C to quit)
-```
-Open a web browser and navigate to the provided ip (in this case 127.0.0.1:8050) to view the sequence visualization.
 ## Tutorials
+
 Note that we provide a few simple tutorials for getting started with the Boreas dataset. Also note that we provide instructions for using this dataset using an AWS SageMaker instance, instructions at: pyboreas/tutorials/aws/README.md.
 
 **NOTE:** ground truth poses have dtype=np.float64, but PyTorch defaults to float32. Avoid using implicit type conversion as this will result in significant quantization error. Implicit conversion is only safe when the translation values are small, such as a pose with respect to a sensor frame or with respect to a starting position, but NOT with respect to ENU (very large).
 
 TODO:
-- Tutorials (pose interp)
-- Ground plane removal
+
 - Pointcloud voxelization
-- 3D Bounding boxes
+
+
```

### Comparing `asrl-pyboreas-1.0.4/asrl_pyboreas.egg-info/PKG-INFO` & `asrl-pyboreas-1.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,79 @@
-Metadata-Version: 2.1
-Name: asrl-pyboreas
-Version: 1.0.4
-Summary: A toolkit for working with the Boreas dataset in Python
-Home-page: https://github.com/utiasASRL/boreas-devkit
-Author: Keenan Burnett, Andrew Li, Shichen Lu, Jingxing Qian, Yuchen Wu, David Yoon
-Author-email: boreas@robotics.utias.utoronto.ca
-License: BSD
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pyboreas
+
 ![Boreas](https://github.com/utiasASRL/pyboreas/blob/master/pyboreas/figs/pyboreas.png)
 
-This devkit provides tools for working with the Boreas Dataset, an all-weather autonomous driving dataset which includes a 128-beam Velodyne Alpha-Prime lidar, a 5MP Blackfly camera, a 360 degree Navtech radar, and post-processed Applanix POS LV GNSS data. Our dataset currently suports benchmarking odometry. We are working towards providing an online benchmark for odometry, localization, and more. We plan to provide an HD map of each driven route. We are also in the process of acquiring 3D labels and hope to be able to provide a challenging object detection benchmark in the future.
+This devkit provides tools for working with the Boreas Dataset, an all-weather autonomous driving dataset which includes a 128-beam Velodyne Alpha-Prime lidar, a 5MP Blackfly camera, a 360 degree Navtech radar, and post-processed Applanix POS LV GNSS data. Our dataset currently suports benchmarking odometry, localization, and 3D object detection.
+
+Our leaderboard is now live! Baseline implementations for each leaderboard are coming soon.
+
+If you find our dataset useful in your research, please cite our dataset paper:
+
+[Boreas: A Multi-Season Autonomous Driving Dataset](https://arxiv.org/abs/2203.10168)
+
+```
+@article{burnett_ijrr23,
+author = {Keenan Burnett and David J Yoon and Yuchen Wu and Andrew Z Li and Haowei Zhang and Shichen Lu and Jingxing Qian and Wei-Kang Tseng and Andrew Lambert and Keith YK Leung and Angela P Schoellig and Timothy D Barfoot},
+title ={Boreas: A multi-season autonomous driving dataset},
+journal = {The International Journal of Robotics Research},
+volume = {42},
+number = {1-2},
+pages = {33-42},
+year = {2023},
+doi = {10.1177/02783649231160195},
+}
 
-Please note that our website is currently under construction. A live benchmark and a browser for downloading sequences will be available via the website soon.
+```
 
 ## Installation
 
 ### Using pip
+
 ```
 pip install asrl-pyboreas
 ```
 
 ### From source
+
 ```
 git clone https://github.com/utiasASRL/pyboreas.git
 pip install -e pyboreas
 ```
 
 ## Download Instructions
-1. [Create an AWS account (optional)](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)
+
+1. [Create an AWS account (OPTIONAL)](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/)
 2. [Install the AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
 3. Create a `root` folder to store the dataset, example: `/path/to/data/boreas/` Each sequence will then be a folder under `root`.
-4. Use the AWS CLI to download either the entire dataset or only the desired sequences and sensors. Add `--no-sign-request` after each of the following commands if you're not going to use an AWS account. For example, the following command will download the entire Boreas dataset:
+4. Use the AWS CLI to download either the entire dataset or only the desired sequences and sensors.
 
-```bash
+**Don't have an AWS Account?** Add `--no-sign-request` after each AWS CLI command.
+
+The following command will download the entire Boreas dataset:
+
+```text
 root=/path/to/data/boreas/
 aws s3 sync s3://boreas $root
 ```
 
 The following command will list all the top-level prefixes (sequences):
 
-```bash
+```text
 root=/path/to/data/boreas/
 aws s3 ls s3://boreas
 ```
 
 Alternatively, [boreas.utias.utoronto.ca (Work In Progress)](https://www.boreas.utias.utoronto.ca/#/download) can be used to browse through sequences so as to pick and choose what data to download. The website will then generate a list of AWS CLI commands that can be run as a bash script. These commands will look something like:
 
-```bash
+```text
 root=/path/to/data/boreas/
 cd $root
 aws s3 sync s3://boreas/boreas-2020-11-26-13-58 boreas-2020-11-26-13-58 --exclude "*" \
-    --include "lidar/" --include "radar/" \
-    --include "applanix/" --include "calib/"
+    --include "lidar/*" --include "radar/*" \
+    --include "applanix/*" --include "calib/*"
 ```
 
 ## Example Usage
 
 ```Python
 import numpy as np
 from pyboreas import BoreasDataset
@@ -113,48 +126,20 @@
 # (4x4 homogeneous transform) wrt a global coordinate frame (ENU),
 # and groundtruth velocity information. Unless it's a part of the test set,
 # in that case, ground truth poses will be missing. However we still provide IMU
 # data (in the applanix frame) through the imu.csv files.
 lidar_frame = bd.get_lidar(0)
 t = lidar_frame.timestamp  # timestamp in seconds
 T_enu_lidar = lidar_frame.pose  # 4x4 homogenous transform [R t; 0 0 0 1]
-vbar = lidar_frame.velocity  # 6x1 vel in ENU frame [v_se_in_e; w_se_in_e] 
+vbar = lidar_frame.velocity  # 6x1 vel in ENU frame [v_se_in_e; w_se_in_e]
 varpi = lidar_frame.body_rate  # 6x1 vel in sensor frame [v_se_in_s; w_se_in_s]
 ```
-## Data Visualizer
-We provide a tool for visualization of sequence frames. Currently, the visualizer supports BEV lidar visualization, BEV radar visualization, Perspective camera + lidar visualization, and 3D lidar point visualization.
 
-```Python
-from pyboreas import BoreasDataset
-from pyboreas.vis.visualizer import BoreasVisualizer
-
-root = '/path/to/data/boreas/'
-bd = BoreasDataset(root)
-seq = bd.sequences[0]
-
-bv = BoreasVisualizer(seq)
-bv.visualize(starting_frame_idx=0)
-```
-Running the above code will start a local web server that visualizes the selected sequence.
-```
-Dash is running on http://127.0.0.1:8050/
-
- * Serving Flask app 'pyboreas.vis.visualizer' (lazy loading)
- * Environment: production
-   WARNING: This is a development server. Do not use it in a production deployment.
-   Use a production WSGI server instead.
- * Debug mode: off
- * Running on http://127.0.0.1:8050/ (Press CTRL+C to quit)
-```
-Open a web browser and navigate to the provided ip (in this case 127.0.0.1:8050) to view the sequence visualization.
 ## Tutorials
+
 Note that we provide a few simple tutorials for getting started with the Boreas dataset. Also note that we provide instructions for using this dataset using an AWS SageMaker instance, instructions at: pyboreas/tutorials/aws/README.md.
 
 **NOTE:** ground truth poses have dtype=np.float64, but PyTorch defaults to float32. Avoid using implicit type conversion as this will result in significant quantization error. Implicit conversion is only safe when the translation values are small, such as a pose with respect to a sensor frame or with respect to a starting position, but NOT with respect to ENU (very large).
 
 TODO:
-- Tutorials (pose interp)
-- Ground plane removal
-- Pointcloud voxelization
-- 3D Bounding boxes
-
 
+- Pointcloud voxelization
```

### Comparing `asrl-pyboreas-1.0.4/asrl_pyboreas.egg-info/SOURCES.txt` & `asrl-pyboreas-1.0.5/asrl_pyboreas.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,33 @@
 asrl_pyboreas.egg-info/PKG-INFO
 asrl_pyboreas.egg-info/SOURCES.txt
 asrl_pyboreas.egg-info/dependency_links.txt
 asrl_pyboreas.egg-info/requires.txt
 asrl_pyboreas.egg-info/top_level.txt
 pyboreas/__init__.py
 pyboreas/boreas.py
+pyboreas/download_task.py
 pyboreas/data/__init__.py
 pyboreas/data/bounding_boxes.py
 pyboreas/data/calib.py
 pyboreas/data/pointcloud.py
 pyboreas/data/sensors.py
 pyboreas/data/sequence.py
 pyboreas/data/splits.py
 pyboreas/eval/__init__.py
-pyboreas/eval/odometry_benchmark.py
+pyboreas/eval/detection.py
+pyboreas/eval/interpolate.py
+pyboreas/eval/localization.py
+pyboreas/eval/odometry.py
+pyboreas/eval/odometry_aeva.py
+pyboreas/eval/submission_checker.py
 pyboreas/test/__init__.py
+pyboreas/test/test_localization.py
 pyboreas/test/test_odometry.py
 pyboreas/utils/__init__.py
+pyboreas/utils/lgmath.py
 pyboreas/utils/odometry.py
 pyboreas/utils/radar.py
 pyboreas/utils/utils.py
 pyboreas/vis/__init__.py
-pyboreas/vis/map_utils.py
 pyboreas/vis/plot_processed_error.py
-pyboreas/vis/vis_utils.py
-pyboreas/vis/visualizer.py
+pyboreas/vis/vis_utils.py
```

### Comparing `asrl-pyboreas-1.0.4/pyboreas/data/bounding_boxes.py` & `asrl-pyboreas-1.0.5/pyboreas/data/bounding_boxes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,100 +1,145 @@
 import os.path as osp
+
 import numpy as np
-from pyboreas.utils.utils import get_time_from_filename, yawPitchRollToRot, rotToYawPitchRoll, get_transform2
-from pyboreas.utils.utils import se3ToSE3, get_inverse_tf
-from pyboreas.vis.vis_utils import draw_boxes
+
 from pyboreas.data.pointcloud import PointCloud
+from pyboreas.utils.utils import (
+    get_inverse_tf,
+    get_time_from_filename,
+    get_transform2,
+    rotToYawPitchRoll,
+    se3ToSE3,
+    yawPitchRollToRot,
+)
+from pyboreas.vis.vis_utils import draw_boxes
+
 
 class BoundingBoxes:
     def __init__(self):
         self.timestamp = None
         self.bbs = []
         self.path = None
 
     def load_from_file(self, path):
-        assert(osp.exists(path))
+        assert osp.exists(path), path
         self.bbs = []
         self.path = path
         with open(path) as f:
             self.timestamp = get_time_from_filename(path)
             for line in f:
                 parts = line.split()
                 uuid = parts[0]
                 label = parts[1]
-                ext = np.array([float(parts[2]), float(parts[3]), float(parts[4])]).reshape(-3, 1) # TODO: fix
-                pos = np.array([float(parts[5]), float(parts[6]), float(parts[7])]).reshape(-3, 1)
+                ext = np.array(
+                    [float(parts[2]), float(parts[3]), float(parts[4])]
+                ).reshape(-3, 1)
+                pos = np.array(
+                    [float(parts[5]), float(parts[6]), float(parts[7])]
+                ).reshape(-3, 1)
                 yaw = float(parts[8])
                 rot = yawPitchRollToRot(yaw, 0, 0)
-                if parts[9] == 'None':
+                if parts[9] == "None":
                     numPoints = 0
                 else:
                     numPoints = int(parts[9])
-                self.bbs.append(BoundingBox(pos, ext, rot, label, uuid, numPoints))
+                score = -1
+                if len(parts) >= 11:
+                    score = float(parts[10])
+                self.bbs.append(
+                    BoundingBox(pos, ext, rot, label, uuid, numPoints, score)
+                )
 
     def save_to_file(self, path):
-        with open(path, 'w') as f:
+        with open(path, "w") as f:
             for bb in self.bbs:
                 yaw, _, _ = rotToYawPitchRoll(bb.rot)
-                f.write('{} {} {} {} {} {} {} {} {} {}\n'.format(bb.uuid,
-                    bb.label, bb.extent[0, 0], bb.extent[1, 0], bb.extent[2, 0],
-                    bb.pos[0, 0], bb.pos[1, 0], bb.pos[2, 0], yaw, bb.numPoints))
+                s = "{} {} {} {} {} {} {} {} {} {}".format(
+                    bb.uuid,
+                    bb.label,
+                    bb.extent[0, 0],
+                    bb.extent[1, 0],
+                    bb.extent[2, 0],
+                    bb.pos[0, 0],
+                    bb.pos[1, 0],
+                    bb.pos[2, 0],
+                    yaw,
+                    bb.numPoints,
+                )
+                if bb.score >= 0:
+                    s += " {}".format(bb.score)
+                f.write(s + "\n")
 
-    def render_2d(self, ax, color='r', **kwargs):
+    def render_2d(self, ax, color="r", **kwargs):
         for bb in self.bbs:
-            bb.render_2d(ax, color=color, **kwargs)
+            bb.render_2d(ax, color, **kwargs)
 
     def transform(self, T):
-        for bb in self.bbs: 
+        for bb in self.bbs:
             bb.transform(T)
 
     def remove_motion(self, body_rate, tref):
         for bb in self.bbs:
             bb.remove_motion(body_rate, tref)
 
-    def project(self, P, width=2448, height=2048, checkdims=False):
+    def project(self, P, width=2448, height=2048, checkdims=False, filterCamFront=True):
         # assumes bounding boxes have already been transformed into the camera coordinates
         # does not modify points in place, returns list of np.array points (pixel coords for box corners)
         UV = []
         for bb in self.bbs:
-            if bb.pos[2] < 0: # only keep bounding boxes in front of the camera
+            if (
+                bb.pos[2] < 0 and filterCamFront
+            ):  # only keep bounding boxes in front of the camera
                 continue
             uv = bb.project(P, width, height, checkdims)
             if uv is not None:
                 UV.append(uv)
         return UV
 
-    def visualize(self, img, P, width=2448, height=2048, checkdims=False, color=[0,255,0],
-        line_width=2, draw_corners=False):
+    def visualize(
+        self,
+        img,
+        P,
+        width=2448,
+        height=2048,
+        checkdims=False,
+        color=[0, 255, 0],
+        line_width=2,
+        draw_corners=False,
+    ):
         UV = self.project(P, width, height, checkdims)
         draw_boxes(img, UV, color, line_width, draw_corners)
 
     def filter_empty(self):
         for i in range(len(self.bbs) - 1, -1, -1):
             if self.bbs[i].numPoints == 0:
                 del self.bbs[i]
 
     def passthrough(self, bounds):
         # xmin, xmax, ymin, ymax, zmin, zmax
         for i in range(len(self.bbs) - 1, -1, -1):
-            if self.bbs[i].pos[0, 0] < bounds[0] or \
-                self.bbs[i].pos[0, 0] > bounds[1] or \
-                self.bbs[i].pos[1, 0] < bounds[2] or \
-                self.bbs[i].pos[1, 0] > bounds[3] or \
-                self.bbs[i].pos[2, 0] < bounds[4] or \
-                self.bbs[i].pos[2, 0] > bounds[5]:
+            if (
+                self.bbs[i].pos[0, 0] < bounds[0]
+                or self.bbs[i].pos[0, 0] > bounds[1]
+                or self.bbs[i].pos[1, 0] < bounds[2]
+                or self.bbs[i].pos[1, 0] > bounds[3]
+                or self.bbs[i].pos[2, 0] < bounds[4]
+                or self.bbs[i].pos[2, 0] > bounds[5]
+            ):
                 del self.bbs[i]
 
     def index_from_uuid(self, uuid):
         for i, bb in enumerate(self.bbs):
             if bb.uuid == uuid:
                 return i
         return -1
 
-    def interpolate(self, idx, timestamp, spose, seqLabelFiles, seqLabelTimes, seqLabelPoses):
+    def interpolate(
+        self, idx, timestamp, spose, seqLabelFiles, seqLabelTimes, seqLabelPoses
+    ):
         if seqLabelTimes[idx] < timestamp:
             lower = idx
             upper = idx + 1
         elif seqLabelTimes[idx] > timestamp:
             lower = idx - 1
             upper = idx
         bb2 = BoundingBoxes()
@@ -109,102 +154,131 @@
         t2 = seqLabelTimes[upper]
         alpha1 = (t2 - timestamp) / (t2 - t1 + 1e-14)
         alpha2 = (timestamp - t1) / (t2 - t1 + 1e-14)
         self._interpolate(alpha1, bb2, alpha2)
         T = np.matmul(get_inverse_tf(spose), T_enu_l1)
         self.transform(T)
 
-    # may delete non-overlapping boxes 
+    # may delete non-overlapping boxes
     def _interpolate(self, alpha1, bb2, alpha2):
         for i in range(len(self.bbs) - 1, -1, -1):
             idx = bb2.index_from_uuid(self.bbs[i].uuid)
             if idx < 0:
                 del self.bbs[i]
                 continue
             self.bbs[i]._interpolate(alpha1, bb2.bbs[idx], alpha2)
 
+
 class BoundingBox:
-    def __init__(self, position=np.zeros((3, 1)), extent=np.zeros((3, 1)),
-        rotation=np.identity(3), label=None, uuid=None, numPoints=None):
+    def __init__(
+        self,
+        position=np.zeros((3, 1)),
+        extent=np.zeros((3, 1)),
+        rotation=np.identity(3),
+        label=None,
+        uuid=None,
+        numPoints=None,
+        score=None,
+    ):
         """Checks dimensional consistency of inputs and constructs points array
 
         Args:
             position: (x,y,z) position of bbox centroid
             extent: (width, length, height) of the bbox
             rotation: rotation matrix for bbox orientation
             label: bounding box label (class)
             uuid: unique ID for a bounding box track
             numPoints: number of lidar points associated with this bounding box
         """
-        assert(position.shape[0] == 3 and position.shape[1] == 1)
-        assert(extent.shape[0] == 3 and extent.shape[1] == 1)
-        assert(rotation.shape[0] == 3 and rotation.shape[1] == 3)
+        assert position.shape[0] == 3 and position.shape[1] == 1
+        assert extent.shape[0] == 3 and extent.shape[1] == 1
+        assert rotation.shape[0] == 3 and rotation.shape[1] == 3
         self.pos = position
         self.extent = extent
         self.rot = rotation
         self.label = label
         self.uuid = uuid
         self.numPoints = numPoints
         self.timestamp = None
+        self.score = score
 
         # Construct array to extract points from extent
         # self.corner_map = {'ftr':0, 'ftl':1, 'btl':2, 'btr':3,
         #               'fbr':4, 'fbl':5, 'bbl':6, 'bbr':7}
-        dims = [[1, 1, 1], [-1, 1, 1], [-1, -1, 1], [1, -1, 1],
-                [1, 1, -1], [-1, 1, -1], [-1, -1, -1], [1, -1, -1]]
+        dims = [
+            [1, 1, 1],
+            [-1, 1, 1],
+            [-1, -1, 1],
+            [1, -1, 1],
+            [1, 1, -1],
+            [-1, 1, -1],
+            [-1, -1, -1],
+            [1, -1, -1],
+        ]
 
         def _get_point_with_offset(pose, offset):
-            p = np.array([offset[0],offset[1],offset[2], 1]).reshape(-1, 1)
+            p = np.array([offset[0], offset[1], offset[2], 1]).reshape(-1, 1)
             return np.matmul(pose, p)[:3, 0]
 
         pose = get_transform2(self.rot, self.pos)
         points = []
         for i in range(len(dims)):
-            points.append(_get_point_with_offset(pose, self.extent.squeeze() * np.array(dims[i]) / 2))
+            points.append(
+                _get_point_with_offset(
+                    pose, self.extent.squeeze() * np.array(dims[i]) / 2
+                )
+            )
         self.pc = PointCloud(np.array(points))
 
     def render_2d(self, ax, color="r", **kwargs):
         """Render the bbox into a top-down 2d view
 
         Args:
             ax: the axis to render the bbox onto
         """
         prev_pt = self.pc.points[3, :]
         for i in range(4):  # Just draw top 4 points of bbox
-            ax.plot([prev_pt[0], self.pc.points[i, 0]], [prev_pt[1], self.pc.points[i, 1]], color=color, **kwargs)
+            ax.plot(
+                [prev_pt[0], self.pc.points[i, 0]],
+                [prev_pt[1], self.pc.points[i, 1]],
+                color=color,
+                **kwargs
+            )
             prev_pt = self.pc.points[i, :]
 
     def project(self, P, width=2448, height=2048, checkdims=False) -> np.ndarray:
         """
         Project bounding boxes corners onto 2D image plane using camera matrix P
         """
 
-        uv, _, _ = self.pc.project_onto_image(P=P, width=width, height=height, checkdims=checkdims)
+        uv, _, _ = self.pc.project_onto_image(
+            P=P, width=width, height=height, checkdims=checkdims
+        )
         if checkdims and uv.shape[0] < self.pc.points.shape[0]:
             return None
 
         return uv
 
     def transform(self, T):
-        assert(T.shape[0] == 4 and T.shape[1] == 4)
+        assert T.shape[0] == 4 and T.shape[1] == 4
         pose = get_transform2(self.rot, self.pos)
         pose = np.matmul(T, pose)
         self.pos = pose[:3, 3:]
         self.rot = pose[:3, :3]
         self.pc.transform(T)
 
     def remove_motion(self, body_rate, tref):
         # tref should be set to max time from associated pointcloud
-        assert(self.timestamp is not None)
+        assert self.timestamp is not None
         T_undistort = se3ToSE3((self.timestamp - tref) * body_rate)
         self.transform(T_undistort)
 
     def _interpolate(self, alpha1, b2, alpha2):
         # linear interpolation
         self.pos = alpha1 * self.pos + alpha2 * b2.pos
         y1, p1, r1 = rotToYawPitchRoll(self.rot)
         y2, p2, r2 = rotToYawPitchRoll(b2.rot)
         y = alpha1 * y1 + alpha2 * y2
         p = alpha1 * p1 + alpha2 * p2
         r = alpha1 * r1 + alpha2 * r2
         self.rot = yawPitchRollToRot(y, p, r)
-        self.pc.points = alpha1 * self.pc.points + alpha2 * b2.pc.points
+        self.pc.points = alpha1 * self.pc.points + alpha2 * b2.pc.points
```

### Comparing `asrl-pyboreas-1.0.4/pyboreas/data/calib.py` & `asrl-pyboreas-1.0.5/pyboreas/data/calib.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import os.path as osp
+
 import numpy as np
 
 
 class Calib:
     """
     Class for loading and storing calibration matrices.
     """
+
     def __init__(self, calib_root):
-        self.P0 = np.loadtxt(osp.join(calib_root, 'P_camera.txt'))
-        self.T_applanix_lidar = np.loadtxt(osp.join(calib_root, 'T_applanix_lidar.txt'))
-        self.T_camera_lidar = np.loadtxt(osp.join(calib_root, 'T_camera_lidar.txt'))
-        self.T_radar_lidar = np.loadtxt(osp.join(calib_root, 'T_radar_lidar.txt'))
+        self.P0 = np.loadtxt(osp.join(calib_root, "P_camera.txt"))
+        self.T_applanix_aeva = np.eye(4)
+        if osp.exists(osp.join(calib_root, "T_applanix_aeva.txt")):
+            self.T_applanix_aeva = np.loadtxt(osp.join(calib_root, "T_applanix_aeva.txt"))
+        self.T_applanix_lidar = np.loadtxt(osp.join(calib_root, "T_applanix_lidar.txt"))
+        self.T_camera_lidar = np.loadtxt(osp.join(calib_root, "T_camera_lidar.txt"))
+        self.T_radar_lidar = np.loadtxt(osp.join(calib_root, "T_radar_lidar.txt"))
 
     def print_calibration(self):
-        print('P0:')
+        print("P0:")
         print(self.P0)
-        print('T_applanix_lidar:')
+        print("T_applanix_aeva:")
+        print(self.T_applanix_aeva)
+        print("T_applanix_lidar:")
         print(self.T_applanix_lidar)
-        print('T_camera_lidar:')
+        print("T_camera_lidar:")
         print(self.T_camera_lidar)
-        print('T_radar_lidar:')
+        print("T_radar_lidar:")
         print(self.T_radar_lidar)
```

### Comparing `asrl-pyboreas-1.0.4/pyboreas/data/pointcloud.py` & `asrl-pyboreas-1.0.5/pyboreas/data/pointcloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-import numpy as np
 import multiprocessing
 from multiprocessing import Pool
-from pyboreas.utils.utils import se3ToSE3, is_sorted
+
+import numpy as np
+
+from pyboreas.utils.utils import is_sorted, se3ToSE3
 
 
 class PointCloud:
     """
     Class for working with (lidar) pointclouds.
     """
+
     def __init__(self, points):
         # points (np.ndarray): (N, 6) [x, y, z, intensity, laser_number, time]
         self.points = points
 
     def transform(self, T, in_place=True):
         """Transforms points given a transform, T. x_out = np.matmul(T, x)
         Args:
             T (np.ndarray): 4x4 transformation matrix
             in_place (bool): if True, self.points is updated
         Returns:
             points (np.ndarray): The transformed points
         """
-        assert (T.shape[0] == 4 and T.shape[1] == 4)
+        assert T.shape[0] == 4 and T.shape[1] == 4
         if in_place:
             points = self.points
         else:
             points = np.copy(self.points)
         p = np.hstack((points[:, :3], np.ones((points.shape[0], 1))))
         points[:, :3] = np.matmul(p, T.transpose())[:, :3]
         return points
@@ -34,15 +37,15 @@
         Args:
             body_rate (np.ndarray): (6, 1) [vx, vy, vz, wx, wy, wz] in sensor frame
             tref (float): reference time to transform the points towards
             in_place (bool): if True, self.points is updated
         Returns:
             points (np.ndarray): points with motion distortion removed
         """
-        assert(body_rate.shape[0] == 6 and body_rate.shape[1] == 1)
+        assert body_rate.shape[0] == 6 and body_rate.shape[1] == 1
         tmin = np.min(self.points[:, 5])
         tmax = np.max(self.points[:, 5])
         if tref is None:
             tref = (tmin + tmax) / 2
         # Precompute finite number of transforms for speed
         bins = 21
         delta = (tmax - tmin) / float(bins - 1)
@@ -64,18 +67,19 @@
         def _process_motion(i):
             index = int((points[i, 5] - tmin) / delta)
             pbar = np.vstack((points[i, :3].reshape(3, 1), 1))
             pbar = np.matmul(T_undistorts[index], pbar)
             points[i, :3] = pbar[:3, 0]
 
         # This function is ~10x faster if the pointcloud is sorted by timestamp (default)
-        sections = []
         if is_sorted(points[:, 5]):
             for i in range(len(tbins) - 1):
-                locs = np.where((points[:, 5] >= tbins[i]) & (points[:, 5] < tbins[i+1]))
+                locs = np.where(
+                    (points[:, 5] >= tbins[i]) & (points[:, 5] < tbins[i + 1])
+                )
                 p = points[locs]
                 p = np.hstack((p[:, :3], np.ones((p.shape[0], 1))))
                 p = np.matmul(p, T_undistorts[i].transpose())
                 p = np.hstack((p[:, :3], points[locs][:, 3:]))
                 points[locs] = p
         else:
             p = Pool(multiprocessing.cpu_count())
@@ -91,30 +95,36 @@
         Args:
             bounds (list): [xmin, xmax, ymin, ymax, zmin, zmax]
             in_place (bool): if True, self.points is updated
         Returns:
             points (np.ndarray): the remaining points after the filter is applied
         """
         if len(bounds) < 6:
-            print('Warning: len(bounds) = {} < 6 is incorrect!'.format(len(bounds)))
+            print("Warning: len(bounds) = {} < 6 is incorrect!".format(len(bounds)))
             return self.points
-        p = self.points[np.where((self.points[:, 0] >= bounds[0]) &
-                                 (self.points[:, 0] <= bounds[1]) &
-                                 (self.points[:, 1] >= bounds[2]) &
-                                 (self.points[:, 1] <= bounds[3]) &
-                                 (self.points[:, 2] >= bounds[4]) &
-                                 (self.points[:, 2] <= bounds[5]))]
+        p = self.points[
+            np.where(
+                (self.points[:, 0] >= bounds[0])
+                & (self.points[:, 0] <= bounds[1])
+                & (self.points[:, 1] >= bounds[2])
+                & (self.points[:, 1] <= bounds[3])
+                & (self.points[:, 2] >= bounds[4])
+                & (self.points[:, 2] <= bounds[5])
+            )
+        ]
         if in_place:
             self.points = p
         return p
 
     # Assumes pointcloud has already been transformed into the camera frame
     # color options: depth, intensity
     # returns pixel locations for lidar point projections onto an image plane
-    def project_onto_image(self, P, width=2448, height=2048, color='depth', checkdims=True):
+    def project_onto_image(
+        self, P, width=2448, height=2048, color="depth", checkdims=True
+    ):
         """Projects 3D points onto a 2D image plane
         Args:
             P (np.ndarray): [fx 0 cx 0; 0 fy cy 0; 0 0 1 0; 0 0 0 1] cam projection
             width (int): width of image
             height (int): height of image
             color (str): 'depth' or 'intensity' to pick colors output
         Return:
@@ -124,34 +134,39 @@
         """
         colors = []
         x = np.hstack((self.points[:, :3], np.ones((self.points.shape[0], 1))))
         x /= x[:, 2:3]
         x[:, 3] = 1
         x = np.matmul(x, P.transpose())
         if checkdims:
-            mask = np.where((x[:, 0] >= 0) &
-                            (x[:, 0] <= width - 1) &
-                            (x[:, 1] >= 0) &
-                            (x[:, 1] <= height - 1))
+            mask = np.where(
+                (x[:, 0] >= 0)
+                & (x[:, 0] <= width - 1)
+                & (x[:, 1] >= 0)
+                & (x[:, 1] <= height - 1)
+            )
         else:
-            mask = np.ones(x.shape[0], dtype=np.bool)
+            mask = np.ones(x.shape[0], dtype=bool)
         x = x[mask]
-        if color == 'depth':
+        if color == "depth":
             colors = self.points[mask][:, 2]
-        elif color == 'intensity':
+        elif color == "intensity":
             colors = self.points[mask][:, 3]
         else:
-            print('Warning: {} is not a valid color'.format(color))
+            print("Warning: {} is not a valid color".format(color))
             colors = self.points[mask][:, 2]
         return x[:, :2], colors, mask
 
     def random_downsample(self, downsample_rate, in_place=True):
-        rand_idx = np.random.choice(self.points.shape[0],
-                                    size=int(self.points.shape[0] * downsample_rate),
-                                    replace=False)
+        rand_idx = np.random.choice(
+            self.points.shape[0],
+            size=int(self.points.shape[0] * downsample_rate),
+            replace=False,
+        )
         p = self.points[rand_idx, :]
         if in_place:
             self.points = p
         return p
 
+
 # TODO: remove_ground(self, bool: in_place)
-# TODO: voxelize(self)
+# TODO: voxelize(self)
```

### Comparing `asrl-pyboreas-1.0.4/pyboreas/data/sensors.py` & `asrl-pyboreas-1.0.5/pyboreas/data/sensors.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,97 @@
 import os.path as osp
 from pathlib import Path
-import numpy as np
+
 import cv2
-import matplotlib.pyplot as plt
-from matplotlib import cm
+import numpy as np
 
+from pyboreas.data.bounding_boxes import BoundingBoxes
 from pyboreas.data.pointcloud import PointCloud
-from pyboreas.utils.utils import get_transform, yawPitchRollToRot, get_time_from_filename, load_lidar
-from pyboreas.utils.utils import get_gt_data_for_frame, get_closest_index, get_inverse_tf
 from pyboreas.utils.radar import load_radar, radar_polar_to_cartesian
-from pyboreas.vis.vis_utils import vis_lidar, vis_camera, vis_radar
-from pyboreas.data.bounding_boxes import BoundingBoxes
+from pyboreas.utils.utils import (
+    get_closest_index,
+    get_gt_data_for_frame,
+    get_inverse_tf,
+    get_time_from_filename,
+    get_time_from_filename_microseconds,
+    get_transform,
+    load_lidar,
+)
+from pyboreas.vis.vis_utils import vis_camera, vis_lidar, vis_radar
 
 
 class Sensor:
     def __init__(self, path):
         self.path = path
+        self.labelFolder = "labels"
         p = Path(path)
         self.frame = p.stem
         self.sensType = p.parts[-2]
         self.seqID = p.parts[-3]
         self.seq_root = str(Path(*p.parts[:-2]))
         self.sensor_root = osp.join(self.seq_root, self.sensType)
         self.pose = np.identity(4, dtype=np.float64)  # T_enu_sensor
-        self.velocity = np.zeros((6, 1))   # 6 x 1 velocity in ENU frame [v_se_in_e; w_se_in_e] 
-        self.body_rate = np.zeros((6, 1))  # 6 x 1 velocity in sensor frame [v_se_in_s; w_se_in_s]
+        self.velocity = np.zeros(
+            (6, 1)
+        )  # 6 x 1 velocity in ENU frame [v_se_in_e; w_se_in_e]
+        self.body_rate = np.zeros(
+            (6, 1)
+        )  # 6 x 1 velocity in sensor frame [v_se_in_s; w_se_in_s]
         self.timestamp = get_time_from_filename(self.frame)
+        self.timestamp_micro = get_time_from_filename_microseconds(self.frame)
 
     def init_pose(self, data=None):
         """Initializes pose variables with ground truth applanix data
         Args:
             data (list): A list of floats corresponding to the line from the sensor_pose.csv file
                 with the matching timestamp
         """
         if data is not None:
             gt = [float(x) for x in data]
         else:
             gt = get_gt_data_for_frame(self.seq_root, self.sensType, self.frame)
         self.pose = get_transform(gt)
         wbar = np.array([gt[12], gt[11], gt[10]]).reshape(3, 1)
         wbar = np.matmul(self.pose[:3, :3], wbar).squeeze()
-        self.velocity = np.array([gt[4], gt[5], gt[6], wbar[0], wbar[1], wbar[2]]).reshape(6, 1)
+        self.velocity = np.array(
+            [gt[4], gt[5], gt[6], wbar[0], wbar[1], wbar[2]]
+        ).reshape(6, 1)
         vbar = np.array([gt[4], gt[5], gt[6]]).reshape(3, 1)
         vbar = np.matmul(self.pose[:3, :3].T, vbar).squeeze()
-        self.body_rate = np.array([vbar[0], vbar[1], vbar[2], gt[12], gt[11], gt[10]]).reshape(6, 1)
+        self.body_rate = np.array(
+            [vbar[0], vbar[1], vbar[2], gt[12], gt[11], gt[10]]
+        ).reshape(6, 1)
 
     def get_bounding_boxes(self, seqLabelFiles=[], seqLabelTimes=[], seqLabelPoses=[]):
         self.bbs = BoundingBoxes()
-        labelPath = osp.join(self.seq_root, 'labels', self.frame + '.txt')
+        labelPath = osp.join(self.seq_root, self.labelFolder, self.frame + ".txt")
         if osp.exists(labelPath):
             self.bbs.load_from_file(labelPath)
         else:
-            if len(seqLabelFiles) == 0 or len(seqLabelTimes) == 0 or len(seqLabelPoses) == 0:
+            if (
+                len(seqLabelFiles) == 0
+                or len(seqLabelTimes) == 0
+                or len(seqLabelPoses) == 0
+            ):
                 return None
             idx = get_closest_index(self.timestamp, seqLabelTimes)
             if idx == 0 or idx == len(seqLabelTimes) - 1:
                 self.bbs.load_from_file(seqLabelFiles[idx])
                 T_enu_lidar = seqLabelPoses[idx]
                 T = np.matmul(get_inverse_tf(self.pose), T_enu_lidar)
                 self.bbs.transform(T)
             else:
-                self.bbs.interpolate(idx, self.timestamp, self.pose, seqLabelFiles, seqLabelTimes, seqLabelPoses)
+                self.bbs.interpolate(
+                    idx,
+                    self.timestamp,
+                    self.pose,
+                    seqLabelFiles,
+                    seqLabelTimes,
+                    seqLabelPoses,
+                )
         return self.bbs
 
 
 class Lidar(Sensor, PointCloud):
     def __init__(self, path):
         Sensor.__init__(self, path)
         self.points = None
@@ -77,19 +104,17 @@
     def visualize(self, **kwargs):
         return vis_lidar(self, **kwargs)
 
     def unload_data(self):
         self.points = None
 
     def has_bbs(self):
-        labelPath = osp.join(self.seq_root, 'labels', self.frame + '.txt')
+        labelPath = osp.join(self.seq_root, self.labelFolder, self.frame + ".txt")
         return osp.exists(labelPath)
 
-    # TODO: get_semantics()
-
 
 class Camera(Sensor):
     def __init__(self, path):
         Sensor.__init__(self, path)
         self.img = None
 
     def load_data(self):
@@ -99,58 +124,60 @@
 
     def visualize(self, **kwargs):
         return vis_camera(self, **kwargs)
 
     def unload_data(self):
         self.img = None
 
-    # TODO: get_bounding_boxes() # retrieve from file, cache to class variable
-
 
 class Radar(Sensor):
     def __init__(self, path):
         Sensor.__init__(self, path)
         self.resolution = 0.0596
         self.timestamps = None
         self.azimuths = None
         self.polar = None
         self.cartesian = None
         self.mask = None
 
     def load_data(self):
         # Loads polar radar data, timestamps, azimuths, and resolution value
         # Additionally, loads a pre-computed cartesian radar image and binary mask if they exist.
-        self.timestamps, self.azimuths, _, self.polar, self.resolution = load_radar(self.path)
-        cart_path = osp.join(self.sensor_root, 'cart', self.frame + '.png')
+        self.timestamps, self.azimuths, _, self.polar, self.resolution = load_radar(
+            self.path
+        )
+        cart_path = osp.join(self.sensor_root, "cart", self.frame + ".png")
         if osp.exists(cart_path):
             self.cartesian = cv2.imread(cart_path, cv2.IMREAD_GRAYSCALE)
-        mask_path = osp.join(self.sensor_root, 'mask', self.frame + '.png')
+        mask_path = osp.join(self.sensor_root, "mask", self.frame + ".png")
         if osp.exists(mask_path):
             self.mask = cv2.imread(mask_path, cv2.IMREAD_GRAYSCALE)
         return self.timestamps, self.azimuths, self.polar
 
     def unload_data(self):
         self.timestamps = None
         self.azimuths = None
         self.polar = None
         self.cartesian = None
         self.mask = None
 
-    def polar_to_cart(self, cart_resolution, cart_pixel_width, polar=None, in_place=True):
+    def polar_to_cart(
+        self, cart_resolution, cart_pixel_width, polar=None, in_place=True
+    ):
         """Converts a polar scan from polar to Cartesian format
         Args:
             cart_resolution (float): resolution of the output Cartesian image in (m / pixel)
             cart_pixel_width (int): width of the output Cartesian image in pixels
             polar (np.ndarray): if supplied, this function will use this input and not self.polar.
             in_place (bool): if True, self.cartesian is updated.
         """
         if polar is None:
             polar = self.polar
-        cartesian = radar_polar_to_cartesian(self.azimuths, polar, self.resolution,
-                                             cart_resolution, cart_pixel_width)
+        cartesian = radar_polar_to_cartesian(
+            self.azimuths, polar, self.resolution, cart_resolution, cart_pixel_width
+        )
         if in_place:
             self.cartesian = cartesian
         return cartesian
 
     def visualize(self, **kwargs):
         return vis_radar(self, **kwargs)
-
```

### Comparing `asrl-pyboreas-1.0.4/pyboreas/data/sequence.py` & `asrl-pyboreas-1.0.5/pyboreas/data/sequence.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,53 +6,58 @@
 from pyboreas.utils.utils import get_closest_frame
 
 
 class Sequence:
     """
     Class for working with an individual Boreas dataset sequence
     """
-    def __init__(self, boreas_root, seqSpec):
+
+    def __init__(self, boreas_root, seqSpec, labelFolder="labels"):
         """init
         Args:
             boreas_root (str): path to root folder ex: /path/to/data/boreas/
             seqSpec (list): defines sequence ID, start_time, and end_time
         """
         self.ID = seqSpec[0]
         if len(seqSpec) > 2:
-            assert seqSpec[2] > seqSpec[1], 'Sequence timestamps must go forward in time'
+            assert (
+                seqSpec[2] > seqSpec[1]
+            ), "Sequence timestamps must go forward in time"
             self.start_ts = str(seqSpec[1])
             self.end_ts = str(seqSpec[2])
         else:
-            self.start_ts = '0'  # dummy start and end if not specified
-            self.end_ts = '9' * 21
+            self.start_ts = "0"  # dummy start and end if not specified
+            self.end_ts = "9" * 21
+        self.labelFolder = labelFolder
         self.seq_root = osp.join(boreas_root, self.ID)
-        self.applanix_root = osp.join(self.seq_root, 'applanix')
-        self.calib_root = osp.join(self.seq_root, 'calib')
-        self.camera_root = osp.join(self.seq_root, 'camera')
-        self.lidar_root = osp.join(self.seq_root, 'lidar')
-        self.radar_root = osp.join(self.seq_root, 'radar')
+        self.applanix_root = osp.join(self.seq_root, "applanix")
+        self.calib_root = osp.join(self.seq_root, "calib")
+        self.aeva_root = osp.join(self.seq_root, "aeva")
+        self.camera_root = osp.join(self.seq_root, "camera")
+        self.lidar_root = osp.join(self.seq_root, "lidar")
+        self.radar_root = osp.join(self.seq_root, "radar")
 
         self._check_dataroot_valid()  # Check if folder structure correct
 
         self.calib = Calib(self.calib_root)
         # Creates list of frame objects for cam, lidar, radar, and inits poses
         self.get_all_frames()
 
         self.load_label_files()
 
         self._check_download()  # prints warning when sensor data missing
 
     def print(self):
-        print('SEQ: {}'.format(self.ID))
-        if self.end_ts != '9' * 21:
-            print('START: {} END: {}'.format(self.start_ts, self.end_ts))
-        print('camera frames: {}'.format(len(self.camera_frames)))
-        print('lidar frames: {}'.format(len(self.lidar_frames)))
-        print('radar frames: {}'.format(len(self.radar_frames)))
-        print('-------------------------------')
+        print("SEQ: {}".format(self.ID))
+        if self.end_ts != "9" * 21:
+            print("START: {} END: {}".format(self.start_ts, self.end_ts))
+        print("camera frames: {}".format(len(self.camera_frames)))
+        print("lidar frames: {}".format(len(self.lidar_frames)))
+        print("radar frames: {}".format(len(self.radar_frames)))
+        print("-------------------------------")
 
     def get_camera(self, idx):
         self.camera_frames[idx].load_data()
         return self.camera_frames[idx]
 
     @property
     def camera(self):
@@ -94,101 +99,130 @@
 
     def _check_dataroot_valid(self):
         """Checks if the sequence folder structure is valid"""
         if not osp.isdir(self.applanix_root):
             raise ValueError("ERROR: applanix dir missing from dataroot")
         if not osp.isdir(self.calib_root):
             raise ValueError("ERROR: calib dir missing from dataroot")
-        if not osp.isdir(self.camera_root):
-            os.mkdir(self.camera_root)
-        if not osp.isdir(self.lidar_root):
-            os.mkdir(self.lidar_root)
-        if not osp.isdir(self.radar_root):
-            os.mkdir(self.radar_root)
 
     def _check_download(self):
         """Checks if all sensor data has been downloaded, prints a warning otherwise"""
-        if len(os.listdir(self.camera_root)) < len(self.camera_frames):
-            print('WARNING: camera images are not all downloaded')
-        if len(os.listdir(self.lidar_root)) < len(self.lidar_frames):
-            print('WARNING: lidar frames are not all downloaded')
-        if len(os.listdir(self.radar_root)) < len(self.radar_frames):
-            print('WARNING: radar scans are not all downloaded')
-        gtfile = osp.join(self.applanix_root, 'gps_post_process.csv')
+        if osp.isdir(self.aeva_root) and len(os.listdir(self.aeva_root)) < len(
+            self.aeva_frames
+        ):
+            print("WARNING: aeva frames are not all downloaded")
+        if osp.isdir(self.camera_root) and len(os.listdir(self.camera_root)) < len(
+            self.camera_frames
+        ):
+            print("WARNING: camera images are not all downloaded: {}".format(self.ID))
+        if osp.isdir(self.lidar_root) and len(os.listdir(self.lidar_root)) < len(
+            self.lidar_frames
+        ):
+            print("WARNING: lidar frames are not all downloaded: {}".format(self.ID))
+        if osp.isdir(self.radar_root) and len(os.listdir(self.radar_root)) < len(
+            self.radar_frames
+        ):
+            print("WARNING: radar scans are not all downloaded: {}".format(self.ID))
+        gtfile = osp.join(self.applanix_root, "gps_post_process.csv")
         if not osp.exists(gtfile):
-            print('WARNING: this may be a test sequence, or the groundtruth is not yet available')
+            print(
+                "WARNING: this may be a test sequence, or the groundtruth is not yet available: {}".format(
+                    self.ID
+                )
+            )
 
     def _get_frames(self, posefile, root, ext, SensorType):
         """Initializes sensor frame objects with their ground truth pose information
         Args:
             posefile (str): path to ../sensor_poses.csv
             root (str): path to the root of the sensor folder ../sensor/
             ext (str): file extension specific to this sensor type
             SensorType (cls): sensor class specific to this sensor type
         Returns:
             frames (list): list of sensor frame objects
         """
         frames = []
-        if not osp.isdir(root):
-            return frames
         if osp.exists(posefile):
-            with open(posefile, 'r') as f:
+            with open(posefile, "r") as f:
                 f.readline()  # header
                 for line in f:
-                    data = line.split(',')
+                    data = line.split(",")
                     ts = data[0]
                     if self.start_ts <= ts and ts <= self.end_ts:
                         frame = SensorType(osp.join(root, ts + ext))
                         frame.init_pose(data)
+                        frame.labelFolder = self.labelFolder
                         frames.append(frame)
-        else:
-            framenames = sorted([f for f in os.listdir(root) if ext in f])
+        elif osp.isdir(root):
+            framenames = sorted([f for f in os.listdir(root) if f.endswith(ext)])
             for framename in framenames:
-                ts = framename.split(',')[0]
+                ts = framename.split(",")[0]
                 if self.start_ts <= ts and ts <= self.end_ts:
-                    frames.append(SensorType(osp.join(root, framename)))
+                    frame = SensorType(osp.join(root, framename))
+                    frame.labelFolder = self.labelFolder
+                    frames.append(frame)
         return frames
 
     def get_all_frames(self):
         """Convenience method for retrieving sensor frames of all types"""
-        cfile = osp.join(self.applanix_root, 'camera_poses.csv')
-        lfile = osp.join(self.applanix_root, 'lidar_poses.csv')
-        rfile = osp.join(self.applanix_root, 'radar_poses.csv')
-        self.camera_frames = self._get_frames(cfile, self.camera_root, '.png', Camera)
-        self.lidar_frames = self._get_frames(lfile, self.lidar_root, '.bin', Lidar)
-        self.radar_frames = self._get_frames(rfile, self.radar_root, '.png', Radar)
+        afile = osp.join(self.applanix_root, "aeva_poses.csv")
+        cfile = osp.join(self.applanix_root, "camera_poses.csv")
+        lfile = osp.join(self.applanix_root, "lidar_poses.csv")
+        rfile = osp.join(self.applanix_root, "radar_poses.csv")
+        self.aeva_frames = self._get_frames(afile, self.aeva_root, ".bin", Lidar)
+        self.camera_frames = self._get_frames(cfile, self.camera_root, ".png", Camera)
+        self.lidar_frames = self._get_frames(lfile, self.lidar_root, ".bin", Lidar)
+        self.radar_frames = self._get_frames(rfile, self.radar_root, ".png", Radar)
 
     def reset_frames(self):
         """Resets all frames, removes downloaded data"""
         self.get_all_frames()
 
-    def synchronize_frames(self, ref='camera'):
+    def synchronize_frames(self, ref="camera"):
         """Simulates having synchronous measurements
         Note: measurements still won't be at the exact same timestamp and will have different poses
         However, for a given reference index, the other measurements will be as close to the reference
         in time as they can be.
         Args:
             ref (str): [camera, lidar, or radar] this determines which sensor's frames will be used as the
                 reference for synchronization. This sensor's list of frames will not be modified. However,
                 the other two list of sensor frames will be modified so that each index will approximately
                 align with the reference in time.
         """
         cstamps = [frame.timestamp for frame in self.camera_frames]
         lstamps = [frame.timestamp for frame in self.lidar_frames]
         rstamps = [frame.timestamp for frame in self.radar_frames]
 
-        if ref == 'camera':
-            self.lidar_frames = [get_closest_frame(cstamp, lstamps, self.lidar_frames) for cstamp in cstamps]
-            self.radar_frames = [get_closest_frame(cstamp, rstamps, self.radar_frames) for cstamp in cstamps]
-        elif ref == 'lidar':
-            self.camera_frames = [get_closest_frame(lstamp, cstamps, self.camera_frames) for lstamp in lstamps]
-            self.radar_frames = [get_closest_frame(lstamp, rstamps, self.radar_frames) for lstamp in lstamps]
-        elif ref == 'radar':
-            self.camera_frames = [get_closest_frame(rstamp, cstamps, self.camera_frames) for rstamp in rstamps]
-            self.lidar_frames = [get_closest_frame(rstamp, lstamps, self.lidar_frames) for rstamp in rstamps]
+        if ref == "camera":
+            self.lidar_frames = [
+                get_closest_frame(cstamp, lstamps, self.lidar_frames)
+                for cstamp in cstamps
+            ]
+            self.radar_frames = [
+                get_closest_frame(cstamp, rstamps, self.radar_frames)
+                for cstamp in cstamps
+            ]
+        elif ref == "lidar":
+            self.camera_frames = [
+                get_closest_frame(lstamp, cstamps, self.camera_frames)
+                for lstamp in lstamps
+            ]
+            self.radar_frames = [
+                get_closest_frame(lstamp, rstamps, self.radar_frames)
+                for lstamp in lstamps
+            ]
+        elif ref == "radar":
+            self.camera_frames = [
+                get_closest_frame(rstamp, cstamps, self.camera_frames)
+                for rstamp in rstamps
+            ]
+            self.lidar_frames = [
+                get_closest_frame(rstamp, lstamps, self.lidar_frames)
+                for rstamp in rstamps
+            ]
 
     def filter_frames_gt(self):
         # Only keep lidar frames that were labelled, NO interpolated frames
         keep = []
         for frame in self.lidar_frames:
             if frame.has_bbs():
                 keep.append(frame)
@@ -196,10 +230,12 @@
 
     def load_label_files(self):
         self.labelFiles = []
         self.labelTimes = []
         self.labelPoses = []
         for frame in self.lidar_frames:
             if frame.has_bbs():
-                self.labelFiles.append(osp.join(self.seq_root, 'labels', frame.frame + '.txt'))
+                self.labelFiles.append(
+                    osp.join(self.seq_root, self.labelFolder, frame.frame + ".txt")
+                )
                 self.labelTimes.append(frame.timestamp)
-                self.labelPoses.append(frame.pose)
+                self.labelPoses.append(frame.pose)
```

### Comparing `asrl-pyboreas-1.0.4/pyboreas/eval/odometry_benchmark.py` & `asrl-pyboreas-1.0.5/pyboreas/eval/interpolate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,66 @@
 import argparse
 import os
-from pyboreas.utils.odometry import get_sequences, get_sequence_poses, get_sequence_poses_gt, \
-    compute_kitti_metrics, compute_interpolation, get_sequence_times_gt
 
-if __name__ == '__main__':
+from pyboreas.utils.odometry import (
+    compute_interpolation,
+    get_sequence_poses,
+    get_sequence_times_gt,
+    get_sequences,
+)
+
+if __name__ == "__main__":
     # parse arguments
     parser = argparse.ArgumentParser()
-    parser.add_argument('--pred', default='test/demo/pred/3d', type=str, help='path to prediction files')
-    parser.add_argument('--gt', default='test/demo/gt', type=str, help='path to groundtruth files')
-    parser.add_argument('--radar', dest='radar', action='store_true', help='evaluate radar odometry in SE(2)')
-    parser.set_defaults(radar=False)
-    parser.add_argument('--interp', default='', type=str, help='path to interpolation output, do not set if evaluating')
-    parser.add_argument('--processes', default=os.cpu_count(), type=int, help='number of workers to use for built-in interpolation')
-    parser.add_argument('--no-solver', dest='solver', action='store_false', help='disable solver for built-in interpolation')
+    parser.add_argument(
+        "--pred", default="test/demo/pred/3d", type=str, help="path to prediction files"
+    )
+    parser.add_argument(
+        "--gt", default="test/demo/gt", type=str, help="path to groundtruth files"
+    )
+    parser.add_argument(
+        "--interp", default="", type=str, help="path to interpolation output"
+    )
+    parser.add_argument(
+        "--processes",
+        default=os.cpu_count(),
+        type=int,
+        help="number of workers to use for built-in interpolation",
+    )
+    parser.add_argument(
+        "--no-solver",
+        dest="solver",
+        action="store_false",
+        help="disable solver for built-in interpolation",
+    )
     parser.set_defaults(solver=True)
     args = parser.parse_args()
 
-    # evaluation mode
-    dim = 2 if args.radar else 3
-    if dim == 2:
-        args.interp = ''  # force interpolation to be off for radar (2D) evaluation
-
     # parse sequences
-    seq = get_sequences(args.pred, '.txt')
+    seq = get_sequences(args.pred, ".txt")
     T_pred, times_pred, seq_lens_pred = get_sequence_poses(args.pred, seq)
 
-    if args.interp:     # if we are interpolating...
-        # can't be the same as pred
-        if args.interp == args.pred:
-            raise ValueError('`interp` directory path cannot be the same as the `pred` directory path')
-
-        # get corresponding groundtruth times
-        times_gt, seq_lens_gt, _ = get_sequence_times_gt(args.gt, seq)
-
-        # make interp directory if it doesn't exist
-        if not os.path.exists(args.interp):
-            os.mkdir(args.interp)
-
-        # interpolate
-        compute_interpolation(T_pred, times_gt, times_pred, seq_lens_gt, seq_lens_pred, seq, args.interp, args.solver, args.processes)
-    else:
-        # get corresponding groundtruth poses
-        T_gt, _, seq_lens_gt, crop = get_sequence_poses_gt(args.gt, seq, dim)
-
-        # compute errors
-        t_err, r_err, _ = compute_kitti_metrics(T_gt, T_pred, seq_lens_gt, seq_lens_pred, seq, args.pred, dim, crop)
-
-        # print out results
-        print('Evaluated sequences: ', seq)
-        print('Overall error: ', t_err, ' %, ', r_err, ' deg/m')
+    # can't be the same as pred
+    if args.interp == args.pred:
+        raise ValueError(
+            "`interp` directory path cannot be the same as the `pred` directory path"
+        )
+
+    # get corresponding groundtruth times
+    times_gt, seq_lens_gt, _ = get_sequence_times_gt(args.gt, seq)
+
+    # make interp directory if it doesn't exist
+    if not os.path.exists(args.interp):
+        os.mkdir(args.interp)
+
+    # interpolate
+    compute_interpolation(
+        T_pred,
+        times_gt,
+        times_pred,
+        seq_lens_gt,
+        seq_lens_pred,
+        seq,
+        args.interp,
+        args.solver,
+        args.processes,
+    )
```

### Comparing `asrl-pyboreas-1.0.4/pyboreas/test/test_odometry.py` & `asrl-pyboreas-1.0.5/pyboreas/test/test_odometry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,141 @@
 """Tests for odometry benchmark"""
+import math
 import os
 import unittest
-import numpy as np
-import math
 
+import numpy as np
 from pylgmath import Transformation, se3op
+
+from pyboreas.utils.odometry import (
+    compute_interpolation,
+    compute_kitti_metrics,
+    get_sequence_poses,
+    get_sequence_poses_gt,
+    get_sequences,
+    interpolate_poses,
+    read_traj_file,
+    write_traj_file,
+)
 from pyboreas.utils.utils import get_inverse_tf
-from pyboreas.utils.odometry import interpolate_poses, write_traj_file, read_traj_file, \
-    get_sequences, get_sequence_poses, get_sequence_poses_gt, compute_kitti_metrics, compute_interpolation
 
 
 class OdometryTestCase(unittest.TestCase):
     """This class contains tests for the odometry benchmark script."""
+
     def test_interpolate(self):
         """Checks the pysteam interpolation against a known constant-velocity groundtruth."""
         # setup groundtruth
-        delt = 0.05     # seconds
+        delt = 0.05  # seconds
         num_poses = 50  # total frames
 
         # constant velocity
         v_x = -1.0
         omega_z = 0.01
-        velocity_prior = np.array([[v_x, 0., 0., 0., 0., omega_z]]).T
-        init_pose_vec = np.array([[0., 0., 0., 0., 0., 0.]]).T
+        velocity_prior = np.array([[v_x, 0.0, 0.0, 0.0, 0.0, omega_z]]).T
+        init_pose_vec = np.array([[0.0, 0.0, 0.0, 0.0, 0.0, 0.0]]).T
         init_pose = Transformation(xi_ab=init_pose_vec)
 
         # create trajectory
-        poses = [se3op.vec2tran(i*delt*velocity_prior)
-                 @ init_pose.matrix() for i in range(num_poses)]
-        times = [int(i*delt*1e6) for i in range(num_poses)]     # microseconds
+        poses = [
+            se3op.vec2tran(i * delt * velocity_prior) @ init_pose.matrix()
+            for i in range(num_poses)
+        ]
+        times = [int(i * delt * 1e6) for i in range(num_poses)]  # microseconds
 
         query_poses = interpolate_poses(poses[::2], times[::2], times[1:-1:2])
         gt_poses = poses[1:-1:2]
         for query_pose, gt_pose in zip(query_poses, gt_poses):
-            delta = gt_pose@get_inverse_tf(query_pose)
+            delta = gt_pose @ get_inverse_tf(query_pose)
             self.assertTrue(np.linalg.norm(se3op.tran2vec(delta)) < 1e-6)
 
     def test_read_write(self):
         """Checks read and write functions for trajectory."""
         # setup groundtruth
         delt = 0.05
         num_poses = 50
 
         # constant velocity
         v_x = -1.0
         omega_z = 0.01
-        velocity_prior = np.array([[v_x, 0., 0., 0., 0., omega_z]]).T
-        init_pose_vec = np.array([[0., 0., 0., 0., 0., 0.]]).T
+        velocity_prior = np.array([[v_x, 0.0, 0.0, 0.0, 0.0, omega_z]]).T
+        init_pose_vec = np.array([[0.0, 0.0, 0.0, 0.0, 0.0, 0.0]]).T
         init_pose = Transformation(xi_ab=init_pose_vec)
 
         # create trajectory
-        write_poses = [se3op.vec2tran(i*delt*velocity_prior)
-                       @ init_pose.matrix() for i in range(num_poses)]
-        write_times = [int(i*delt*1e6) for i in range(num_poses)]     # microseconds
+        write_poses = [
+            se3op.vec2tran(i * delt * velocity_prior) @ init_pose.matrix()
+            for i in range(num_poses)
+        ]
+        write_times = [int(i * delt * 1e6) for i in range(num_poses)]  # microseconds
 
         # write out trajectory to file, then read it back
-        write_traj_file('pyboreas/test/test_traj.txt', write_poses, write_times)
-        read_poses, read_times = read_traj_file('pyboreas/test/test_traj.txt')
+        write_traj_file("pyboreas/test/test_traj.txt", write_poses, write_times)
+        read_poses, read_times = read_traj_file("pyboreas/test/test_traj.txt")
 
         # compare write and read
-        for wpose, wtime, rpose, rtime in zip(write_poses, write_times, read_poses, read_times):
-            delta = wpose@get_inverse_tf(rpose)
+        for wpose, wtime, rpose, rtime in zip(
+            write_poses, write_times, read_poses, read_times
+        ):
+            delta = wpose @ get_inverse_tf(rpose)
             self.assertTrue(np.linalg.norm(se3op.tran2vec(delta)) < 1e-6)
             self.assertTrue(wtime == rtime)
 
         # delete file
-        os.remove('pyboreas/test/test_traj.txt')
+        os.remove("pyboreas/test/test_traj.txt")
 
     def test_module(self):
-        pred = 'pyboreas/test/demo/pred/3d'
-        gt = 'pyboreas/test/demo/gt'
+        pred = "pyboreas/test/demo/pred/3d"
+        gt = "pyboreas/test/demo/gt"
         dim = 3
-        interp = 'pyboreas/test/demo/pred/3d/interptest'
+        interp = "pyboreas/test/demo/pred/3d/interptest"
         solver = False
         processes = 2
 
         # make interp directory if it doesn't exist
         if not os.path.exists(interp):
             os.mkdir(interp)
 
         # parse sequences
-        seq = get_sequences(pred, '.txt')
+        seq = get_sequences(pred, ".txt")
         T_pred, times_pred, seq_lens_pred = get_sequence_poses(pred, seq)
         T_gt, times_gt, seq_lens_gt, crop = get_sequence_poses_gt(gt, seq, dim)
 
         # interpolate
-        compute_interpolation(T_pred, times_gt, times_pred, seq_lens_gt, seq_lens_pred, seq, interp, solver, processes)
+        compute_interpolation(
+            T_pred,
+            times_gt,
+            times_pred,
+            seq_lens_gt,
+            seq_lens_pred,
+            seq,
+            interp,
+            solver,
+            processes,
+        )
 
         # read in interpolated sequences
         T_pred, times_pred, seq_lens_pred = get_sequence_poses(interp, seq)
 
         # compute errors
-        _, _, err_list = compute_kitti_metrics(T_gt, T_pred, seq_lens_gt, seq_lens_pred, seq, '', dim, crop)
+        _, _, err_list = compute_kitti_metrics(
+            T_gt, T_pred, seq_lens_gt, seq_lens_pred, seq, "", dim, crop
+        )
 
         # first sequence should be close to kitti C++ results: 0.011094 0.000077
-        self.assertTrue(math.fabs(err_list[0][0] - 0.011094*100) < 1e-4)
-        self.assertTrue(math.fabs(err_list[0][1] - 0.000077*180/math.pi) < 1e-5)
+        self.assertTrue(math.fabs(err_list[0][0] - 0.011094 * 100) < 1e-4)
+        self.assertTrue(math.fabs(err_list[0][1] - 0.000077 * 180 / math.pi) < 1e-5)
 
         # second sequence should be close to 0
         self.assertTrue(err_list[1][0] < 1e-1)
         self.assertTrue(err_list[1][1] < 1e-2)
 
         # delete file
         for i in range(2):
             file = os.path.join(interp, seq[i])
             os.remove(file)
         os.rmdir(interp)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # run 'python -m unittest' from root directory (one above pyboreas directory)
     unittest.main()
```

### Comparing `asrl-pyboreas-1.0.4/pyboreas/utils/radar.py` & `asrl-pyboreas-1.0.5/pyboreas/utils/radar.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 # Attribution-NonCommercial-ShareAlike 4.0 International License.
 # To view a copy of this license, visit
 # http://creativecommons.org/licenses/by-nc-sa/4.0/ or send a letter to
 # Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.
 #
 ###############################################################################
 
-import numpy as np
 import cv2
+import numpy as np
+
 from pyboreas.utils.utils import get_time_from_filename
 
 upgrade_time = 1632182400  # before: resolution = 0.0596, after: resolution = 0.04381
 
 
 def load_radar(example_path):
     """Decode a single Oxford Radar RobotCar Dataset radar example
@@ -34,25 +35,37 @@
     encoder_size = 5600
     resolution = 0.0596
     t = get_time_from_filename(example_path)
     if t > upgrade_time:
         resolution = 0.04381
     raw_example_data = cv2.imread(example_path, cv2.IMREAD_GRAYSCALE)
     timestamps = raw_example_data[:, :8].copy().view(np.int64)
-    azimuths = (raw_example_data[:, 8:10].copy().view(np.uint16) / float(encoder_size) * 2 * np.pi).astype(np.float32)
+    azimuths = (
+        raw_example_data[:, 8:10].copy().view(np.uint16)
+        / float(encoder_size)
+        * 2
+        * np.pi
+    ).astype(np.float32)
     valid = raw_example_data[:, 10:11] == 255
-    fft_data = raw_example_data[:, 11:].astype(np.float32)[:, :, np.newaxis] / 255.
+    fft_data = raw_example_data[:, 11:].astype(np.float32)[:, :, np.newaxis] / 255.0
     min_range = int(round(2.5 / resolution))
     fft_data[:, :min_range] = 0
     fft_data = np.squeeze(fft_data)
     return timestamps, azimuths, valid, fft_data, resolution
 
 
-def radar_polar_to_cartesian(azimuths, fft_data, radar_resolution, cart_resolution, cart_pixel_width,
-                             interpolate_crossover=True, fix_wobble=True):
+def radar_polar_to_cartesian(
+    azimuths,
+    fft_data,
+    radar_resolution,
+    cart_resolution,
+    cart_pixel_width,
+    interpolate_crossover=True,
+    fix_wobble=True,
+):
     """Convert a polar radar scan to cartesian.
     Args:
         azimuths (np.ndarray): Rotation for each polar radar azimuth (radians)
         fft_data (np.ndarray): Polar radar power readings
         radar_resolution (float): Resolution of the polar radar data (metres per pixel)
         cart_resolution (float): Cartesian resolution (metres per pixel)
         cart_pixel_width (int): Width and height of the returned square cartesian output (pixels). Please see the Notes
@@ -63,19 +76,21 @@
     Returns:
         np.ndarray: Cartesian radar power readings
     """
     if (cart_pixel_width % 2) == 0:
         cart_min_range = (cart_pixel_width / 2 - 0.5) * cart_resolution
     else:
         cart_min_range = cart_pixel_width // 2 * cart_resolution
-    coords = np.linspace(-cart_min_range, cart_min_range, cart_pixel_width, dtype=np.float32)
+    coords = np.linspace(
+        -cart_min_range, cart_min_range, cart_pixel_width, dtype=np.float32
+    )
     Y, X = np.meshgrid(coords, -1 * coords)
     sample_range = np.sqrt(Y * Y + X * X)
     sample_angle = np.arctan2(Y, X)
-    sample_angle += (sample_angle < 0).astype(np.float32) * 2. * np.pi
+    sample_angle += (sample_angle < 0).astype(np.float32) * 2.0 * np.pi
 
     # Interpolate Radar Data Coordinates
     azimuth_step = (azimuths[-1] - azimuths[0]) / (azimuths.shape[0] - 1)
     sample_u = (sample_range - radar_resolution / 2) / radar_resolution
     sample_v = (sample_angle - azimuths[0]) / azimuth_step
     # This fixes the wobble in the old CIR204 data from Boreas
     M = azimuths.shape[0]
```

### Comparing `asrl-pyboreas-1.0.4/pyboreas/utils/utils.py` & `asrl-pyboreas-1.0.5/pyboreas/utils/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,82 @@
-from bisect import bisect_left
 import os.path as osp
+from bisect import bisect_left
 from pathlib import Path
+
 import numpy as np
-import cv2
+
+from pyboreas.utils.lgmath import _tran2vec, _vec2tran, carrot
 
 
 def load_lidar(path):
     """Loads a pointcloud (np.ndarray) (N, 6) from path [x, y, z, intensity, laser_number, time]"""
     # dtype MUST be float32 to load this properly!
     points = np.fromfile(path, dtype=np.float32).reshape((-1, 6)).astype(np.float64)
     t = get_time_from_filename(path)
     points[:, 5] += t
     return points
 
 
 def roll(r):
-    return np.array([[1, 0, 0], [0, np.cos(r), np.sin(r)], [0, -np.sin(r), np.cos(r)]], dtype=np.float64)
+    return np.array(
+        [[1, 0, 0], [0, np.cos(r), np.sin(r)], [0, -np.sin(r), np.cos(r)]],
+        dtype=np.float64,
+    )
 
 
 def pitch(p):
-    return np.array([[np.cos(p), 0, -np.sin(p)], [0, 1, 0], [np.sin(p), 0, np.cos(p)]], dtype=np.float64)
+    return np.array(
+        [[np.cos(p), 0, -np.sin(p)], [0, 1, 0], [np.sin(p), 0, np.cos(p)]],
+        dtype=np.float64,
+    )
 
 
 def yaw(y):
-    return np.array([[np.cos(y), np.sin(y), 0], [-np.sin(y), np.cos(y), 0], [0, 0, 1]], dtype=np.float64)
+    return np.array(
+        [[np.cos(y), np.sin(y), 0], [-np.sin(y), np.cos(y), 0], [0, 0, 1]],
+        dtype=np.float64,
+    )
 
 
 def yawPitchRollToRot(y, p, r):
-    Y = yaw(y)
-    P = pitch(p)
-    R = roll(r)
-    C = np.matmul(P, Y)
-    return np.matmul(R, C)
+    return roll(r) @ pitch(p) @ yaw(y)
 
 
 def rotToYawPitchRoll(C):
     i = 2
     j = 1
     k = 0
-    c_y = np.sqrt(C[i, i]**2 + C[j, i]**2)
+    c_y = np.sqrt(C[i, i] ** 2 + C[j, i] ** 2)
     if c_y > 1e-14:
         r = np.arctan2(C[j, i], C[i, i])
         p = np.arctan2(-C[k, i], c_y)
         y = np.arctan2(C[k, j], C[k, k])
     else:
         r = 0
         p = np.arctan2(-C[k, i], c_y)
         y = np.arctan2(-C[j, k], C[j, j])
     return y, p, r
 
 
+def rotToRollPitchYaw(C):
+    i = 2
+    j = 1
+    k = 0
+    c_y = np.sqrt(C[i, i] ** 2 + C[j, i] ** 2)
+    if c_y > 1e-14:
+        r = np.arctan2(C[j, i], C[i, i])
+        p = np.arctan2(-C[k, i], c_y)
+        y = np.arctan2(C[k, j], C[k, k])
+    else:
+        r = 0
+        p = np.arctan2(-C[k, i], c_y)
+        y = np.arctan2(-C[j, k], C[j, j])
+    return r, p, y
+
+
 def get_transform(gt):
     """Retrieve 4x4 homogeneous transform for a given parsed line of the ground truth pose csv
     Args:
         gt (List[float]): parsed line from ground truth csv file
     Returns:
         np.ndarray: 4x4 transformation matrix (pose of sensor)
     """
@@ -86,15 +109,17 @@
         x (float): x-translation
         y (float): y-translation
         theta (float): rotation
     Returns:
         np.ndarray: 4x4 transformation matrix
     """
     T = np.identity(4, dtype=dtype)
-    T[0:2, 0:2] = np.array([[np.cos(theta), np.sin(theta)], [-np.sin(theta), np.cos(theta)]])
+    T[0:2, 0:2] = np.array(
+        [[np.cos(theta), np.sin(theta)], [-np.sin(theta), np.cos(theta)]]
+    )
     T[0, 3] = x
     T[1, 3] = y
     return T
 
 
 def quaternionToRot(qin):
     """Converts a quaternion to a rotation  matrix
@@ -104,16 +129,19 @@
         C (np.ndarray) (3,3) rotation matrix
     """
     q = qin.copy().reshape(4, 1)
     if np.matmul(q.transpose(), q) < 1e-14:
         return np.identity(3)
     xi = q[:3].reshape(3, 1)
     eta = q[3, 0]
-    C = (eta**2 - np.matmul(xi.transpose(), xi)) * np.identity(3) + \
-        2 * np.matmul(xi, xi.transpose()) - 2 * eta * carrot(xi)
+    C = (
+        (eta**2 - np.matmul(xi.transpose(), xi)) * np.identity(3)
+        + 2 * np.matmul(xi, xi.transpose())
+        - 2 * eta * carrot(xi)
+    )
     return C
 
 
 def rotToQuaternion(C):
     """Converts a rotation matrix to a quaternion
     Note that the space of unit-length quaternions is a double-cover of SO(3)
     which means that, C maps to +/- q, so q --> C --> +/- q
@@ -124,33 +152,33 @@
     """
     eta = 0.5 * np.sqrt((1 + np.trace(C)))
     if np.abs(eta) < 1e-14:
         eta = 0
         xi = np.sqrt(np.diag(0.5 * (C + np.identity(3))))
         q = np.array([xi[0], xi[1], xi[2], eta]).reshape(4, 1)
     else:
-        phi = wrapto2pi(2 * np.arccos(eta))
+        phi = wrapto2pi(2 * np.arccos(max(min(eta, 1.0), -1.0)))
         eta = np.cos(phi / 2)
         xi_cross = (C.T - C) / (4 * eta)
-        q = np.array([xi_cross[2, 1], xi_cross[0, 2], xi_cross[1, 0], eta]).reshape(4, 1)
+        q = np.array([xi_cross[2, 1], xi_cross[0, 2], xi_cross[1, 0], eta]).reshape(
+            4, 1
+        )
     return q
 
 
 def get_inverse_tf(T):
     """Returns the inverse of a given 4x4 homogeneous transform.
     Args:
         T (np.ndarray): 4x4 transformation matrix
     Returns:
         np.ndarray: inv(T)
     """
-    T2 = np.identity(4, dtype=T.dtype)
-    R = T[:3, :3]
-    t = T[:3, 3:]
-    T2[:3, :3] = R.transpose()
-    T2[:3, 3:] = np.matmul(-1 * R.transpose(), t)
+    T2 = T.copy()
+    T2[:3, :3] = T2[:3, :3].transpose()
+    T2[:3, 3:] = -1 * T2[:3, :3] @ T2[:3, 3:]
     return T2
 
 
 def enforce_orthog(T, dim=3):
     """Enforces orthogonality of a 3x3 rotation matrix within a 4x4 homogeneous transformation matrix.
     Args:
         T (np.ndarray): 4x4 transformation matrix
@@ -187,89 +215,34 @@
         newcol1 = np.cross(c2, newcol0)
         T[0:3, 0] = newcol0
         T[0:3, 1] = newcol1
         T[0:3, 2] = c2
     return T
 
 
-def carrot(xbar):
-    """Overloaded operator. converts 3x1 vectors into a member of Lie Alebra so(3)
-        Also, converts 6x1 vectors into a member of Lie Algebra se(3)
-    Args:
-        xbar (np.ndarray): if 3x1, xbar is a vector of rotation angles, if 6x1 a vector of 3 trans and 3 rot angles.
-    Returns:
-        np.ndarray: Lie Algebra 3x3 matrix so(3) if input 3x1, 4x4 matrix se(3) if input 6x1.
-    """
-    x = xbar.squeeze()
-    if x.shape[0] == 3:
-        return np.array([[0, -x[2], x[1]],
-                         [x[2], 0, -x[0]],
-                         [-x[1], x[0], 0]])
-    elif x.shape[0] == 6:
-        return np.array([[0, -x[5], x[4], x[0]],
-                         [x[5], 0, -x[3], x[1]],
-                         [-x[4], x[3], 0, x[2]],
-                         [0, 0, 0, 1]])
-    print('WARNING: attempted carrot operator on invalid vector shape')
-    return xbar
-
-
 def se3ToSE3(xi):
     """Converts 6x1 vectors representing the Lie Algebra, se(3) into a 4x4 homogeneous transform in SE(3)
         Lie Vector xi = [rho, phi]^T (6 x 1) --> SE(3) T = [C, r; 0 0 0 1] (4 x 4)
     Args:
         xi (np.ndarray): 6x1 vector
     Returns:
         np.ndarray: 4x4 transformation matrix
     """
-    T = np.identity(4, dtype=np.float64)
-    rho = xi[0:3].reshape(3, 1)
-    phibar = xi[3:6].reshape(3, 1)
-    phi = np.linalg.norm(phibar)
-    R = np.identity(3)
-    if phi != 0:
-        phibar /= phi  # normalize
-        I = np.identity(3)
-        R = np.cos(phi) * I + (1 - np.cos(phi)) * phibar @ phibar.T + np.sin(phi) * carrot(phibar)
-        J = I * np.sin(phi) / phi + (1 - np.sin(phi) / phi) * phibar @ phibar.T + \
-            carrot(phibar) * (1 - np.cos(phi)) / phi
-        rho = J @ rho
-    T[0:3, 0:3] = R
-    T[0:3, 3:] = rho
-    return T
+    return _vec2tran(xi)
 
 
-def SE3Tose3(T):
+def SE3Tose3(TIn):
     """Converts 4x4 homogeneous transforms in SE(3) to 6x1 vectors representing the Lie Algebra, se(3)
         SE(3) T = [C, r; 0 0 0 1] (4 x 4) --> Lie Vector xi = [rho, phi]^T (6 x 1)
     Args:
         T (np.ndarray): 4x4 transformation matrix
     Returns:
         np.ndarray: 6x1 vector
     """
-    R = T[0:3, 0:3]
-    evals, evecs = np.linalg.eig(R)
-    idx = -1
-    for i in range(3):
-        if evals[i].real != 0 and evals[i].imag == 0:
-            idx = i
-            break
-    assert(idx != -1)
-    abar = evecs[idx].real.reshape(3, 1)
-    phi = np.arccos((np.trace(R) - 1) / 2)
-    rho = T[0:3, 3:]
-    if phi != 0:
-        I = np.identity(3)
-        J = I * np.sin(phi) / phi + (1 - np.sin(phi) / phi) * abar @ abar.T + \
-            carrot(abar) * (1 - np.cos(phi)) / phi
-        rho = np.linalg.inv(J) @ rho
-    xi = np.zeros((6, 1))
-    xi[0:3, 0:] = rho
-    xi[3:, 0:] = phi * abar
-    return xi
+    return _tran2vec(TIn)
 
 
 def rotation_error(T):
     """Calculates a single rotation value corresponding to the upper-left 3x3 rotation matrix.
         Uses axis-angle representation to get a single number for rotation
     Args:
         T (np.ndarray): 4x4 transformation matrix T = [C, r; 0 0 0 1]
@@ -285,16 +258,16 @@
     Args:
         T (np.ndarray): 4x4 transformation matrix T = [C, r; 0 0 0 1]
         dim (int): If dim=2 we only use x,y, otherwise we use all dims.
     Returns:
         float: translation distance
     """
     if dim == 2:
-        return np.sqrt(T[0, 3]**2 + T[1, 3]**2)
-    return np.sqrt(T[0, 3]**2 + T[1, 3]**2 + T[2, 3]**2)
+        return np.sqrt(T[0, 3] ** 2 + T[1, 3] ** 2)
+    return np.sqrt(T[0, 3] ** 2 + T[1, 3] ** 2 + T[2, 3] ** 2)
 
 
 def wrapto2pi(phi):
     """Ensures that the output angle phi is within the interval [0, 2*pi)"""
     if phi < 0:
         return phi + 2 * np.pi * np.ceil(phi / (-2 * np.pi))
     elif phi >= 2 * np.pi:
@@ -304,33 +277,42 @@
 
 def get_time_from_filename(file):
     """Retrieves an epoch time from a file name in seconds"""
     tstr = str(Path(file).stem)
     gpstime = float(tstr)
     timeconvert = 1e-6
     if len(tstr) != 16 and len(tstr) > 10:
-        timeconvert = 10**(-1 * (len(tstr) - 10))
+        timeconvert = 10 ** (-1 * (len(tstr) - 10))
     return gpstime * timeconvert
 
+
+def get_time_from_filename_microseconds(file):
+    tstr = str(Path(file).stem)
+    gpstime = int(tstr)
+    return gpstime
+
+
 def get_gt_data_for_frame(root, sensType, frame):
     """Retrieves ground truth applanix data for a given sensor frame
     Args:
         root (str): path to the sequence root
         sensType (str): [camera, lidar, or radar]
         frame (str): name/timestampd of the given sensor frame (without the extension)
     Returns:
         gt (list): A list of ground truth values from the applanix sensor_poses.scv
     """
-    posepath = osp.join(root, 'applanix', sensType + '_poses.csv')
-    with open(posepath, 'r') as f:
+    posepath = osp.join(root, "applanix", sensType + "_poses.csv")
+    with open(posepath, "r") as f:
         f.readline()  # header
         for line in f:
-            if line.split(',')[0] == frame:
-                return [float(x) for x in line.split(',')]
-    assert(0), 'gt not found for root: {} sensType: {} frame: {}'.format(root, sensType, frame)
+            if line.split(",")[0] == frame:
+                return [float(x) for x in line.split(",")]
+    assert 0, "gt not found for root: {} sensType: {} frame: {}".format(
+        root, sensType, frame
+    )
     return None
 
 
 def get_closest_index(query, targets):
     """Retrieves the index of the element in targets that is closest to query O(log n)
     Args:
         query (float): query value
@@ -359,26 +341,30 @@
         query_time (float)
         frame_times (list): list of timestamps which corresponds to the frames list
         frames: (list): list of frames
     Returns:
         closest_frame (SensorType)
     """
     closest = get_closest_index(query_time, frame_times)
-    assert(abs(query_time - frame_times[closest]) < 3.0), 'query: {}'.format(query_time)
+    assert abs(query_time - frame_times[closest]) < 3.0, "query: {}".format(query_time)
     return frames[closest]
 
 
 def is_sorted(x):
     """Returns True is x is a sorted list, otherwise False"""
     return (np.diff(x) >= 0).all()
 
 
 def get_T_bev_metric(resolution, width):
     alpha = 1 / resolution
     if (width % 2) == 0:
-        min_range = (width / 2 - 0.5)
+        min_range = width / 2 - 0.5
     else:
         min_range = width // 2
-    return np.array([[0, alpha, 0, min_range],
-                   [-alpha, 0, 0, min_range],
-                   [0, 0, 1, 0],
-                   [0, 0, 0, 1]])
+    return np.array(
+        [
+            [0, alpha, 0, min_range],
+            [-alpha, 0, 0, min_range],
+            [0, 0, 1, 0],
+            [0, 0, 0, 1],
+        ]
+    )
```

### Comparing `asrl-pyboreas-1.0.4/pyboreas/vis/vis_utils.py` & `asrl-pyboreas-1.0.5/pyboreas/vis/vis_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,97 +1,128 @@
 import io
-import PIL
-import numpy as np
-import matplotlib.pyplot as plt
-import cv2
 
-from pyboreas.utils.utils import rotToYawPitchRoll, yaw, get_transform2
+import cv2
+import matplotlib.pyplot as plt
+import numpy as np
+import PIL
 
 
 def convert_plt_to_img(dpi=128):
     buf = io.BytesIO()
-    plt.savefig(buf, format='png', dpi=dpi, bbox_inches='tight', pad_inches=0)
+    plt.savefig(buf, format="png", dpi=dpi, bbox_inches="tight", pad_inches=0)
     plt.close()
     buf.seek(0)
     return PIL.Image.open(buf)
 
 
 def vis_camera(cam, figsize=(24.48, 20.48), dpi=100, show=True, save=None):
     fig = plt.figure(figsize=figsize, dpi=dpi)
     ax = fig.add_subplot()
     ax.imshow(cam.img)
     ax.set_axis_off()
     if show:
         plt.show()
     if save is not None:
-        plt.savefig(save, bbox_inches='tight')
+        plt.savefig(save, bbox_inches="tight")
     return ax
 
 
-def vis_lidar(lid, figsize=(10, 10), cmap='winter',
-              color='intensity', colorvec=None, vmin=None, vmax=None, azim_delta=-75, elev_delta=-5,
-              show=True, save=None):
+def vis_lidar(
+    lid,
+    figsize=(10, 10),
+    cmap="winter",
+    color="intensity",
+    colorvec=None,
+    vmin=None,
+    vmax=None,
+    azim_delta=-75,
+    elev_delta=-5,
+    show=True,
+    save=None,
+):
     p = lid.points
-    if color == 'x':
+    if color == "x":
         c = p[:, 0]
-    elif color == 'y':
+    elif color == "y":
         c = p[:, 1]
-    elif color == 'z':
+    elif color == "z":
         c = p[:, 2]
-    elif color == 'intensity':
+    elif color == "intensity":
         c = p[:, 3]
-    elif color == 'ring':
+    elif color == "ring":
         c = p[:, 4]
-    elif color == 'time':
+    elif color == "time":
         c = p[:, 5]
+    elif color == "distance":
+        c = np.sqrt(p[:, 0] ** 2 + p[:, 1] ** 2)
     else:
-        print('warning: color: {} is not valid'.format(color))
+        print("warning: color: {} is not valid".format(color))
         c = p[:, 2]
     if colorvec is not None:
         c = colorvec
     if vmin is None or vmax is None:
         vmin = np.min(c)
         vmax = np.max(c)
     fig = plt.figure(figsize=figsize)
-    ax = fig.add_subplot(projection='3d')
+    ax = fig.add_subplot(projection="3d")
     ax.azim += azim_delta
     ax.elev += elev_delta
     xs = p[:, 0]
     ys = p[:, 1]
     zs = p[:, 2]
     ax.set_box_aspect((np.ptp(xs), np.ptp(ys), np.ptp(zs)))
     ax.set_axis_off()
     if colorvec is None:
-        ax.scatter(xs=xs, ys=ys, zs=zs, s=0.1, c=c, cmap=cmap,
-                   vmin=vmin, vmax=vmax, depthshade=False)
+        ax.scatter(
+            xs=xs,
+            ys=ys,
+            zs=zs,
+            s=0.1,
+            c=c,
+            cmap=cmap,
+            vmin=vmin,
+            vmax=vmax,
+            depthshade=False,
+        )
     else:
         ax.scatter(xs=xs, ys=ys, zs=zs, s=0.1, c=c, depthshade=False)
     if show:
         plt.show()
     if save is not None:
-        plt.savefig(save, bbox_inches='tight')
+        plt.savefig(save, bbox_inches="tight")
     return ax
 
 
-def vis_radar(rad, figsize=(10, 10), dpi=100, cart_resolution=0.2384, cart_pixel_width=640, cmap='gray',
-              show=True, save=None):
-    cart = rad.polar_to_cart(cart_resolution=cart_resolution, cart_pixel_width=cart_pixel_width, in_place=False)
+def vis_radar(
+    rad,
+    figsize=(10, 10),
+    dpi=100,
+    cart_resolution=0.2384,
+    cart_pixel_width=640,
+    cmap="gray",
+    show=True,
+    save=None,
+):
+    cart = rad.polar_to_cart(
+        cart_resolution=cart_resolution,
+        cart_pixel_width=cart_pixel_width,
+        in_place=False,
+    )
     fig = plt.figure(figsize=figsize, dpi=dpi)
     ax = fig.add_subplot()
     ax.imshow(cart, cmap=cmap)
     ax.set_axis_off()
     if show:
         plt.show()
     if save is not None:
-        plt.savefig(save, bbox_inches='tight')
+        plt.savefig(save, bbox_inches="tight")
     return ax
 
 
 def bilinear_interp(img, X, Y):
-
     x = np.array(X).squeeze()
     y = np.array(Y).squeeze()
 
     x1 = np.floor(x).astype(np.int32)
     x2 = np.ceil(x).astype(np.int32)
     y1 = np.floor(y).astype(np.int32)
     y2 = np.ceil(y).astype(np.int32)
@@ -100,77 +131,85 @@
 
     q11 = img[y1, x1]  # N x 3
     q12 = img[y2, x1]
     q21 = img[y1, x2]
     q22 = img[y2, x2]
 
     EPS = 1e-14
-    x_21 = (x2 - x1 + EPS)
+    x_21 = x2 - x1 + EPS
     x_2 = ((x2 - x) / x_21).reshape(-1, 1)
     x_1 = ((x - x1) / x_21).reshape(-1, 1)
 
     f_y1 = q11 * x_2 + q21 * x_1
     f_y2 = q12 * x_2 + q22 * x_1
 
     f_y1[mask] = q11[mask]
     f_y2[mask] = q22[mask]
 
     mask = np.where(y1 == y2)
 
-    y_21 = (y2 - y1 + EPS)
+    y_21 = y2 - y1 + EPS
     y_2 = ((y2 - y) / y_21).reshape(-1, 1)
     y_1 = ((y - y1) / y_21).reshape(-1, 1)
 
     f = y_2 * f_y1 + y_1 * f_y2
     f[mask] = f_y1[mask]
 
     return f.squeeze()
 
 
 def draw_point(img, pixels, color=[0, 0, 255], diameter=3, line_width=4):
-    cv2.circle(img,(pixels[0],pixels[1]), diameter, color, line_width)
+    cv2.circle(img, (pixels[0], pixels[1]), diameter, color, line_width)
 
 
 def draw_box(img, uv, color, line_width, draw_corners=False, draw_box=True):
-    assert(uv.shape[0] == 8 and uv.shape[1] >= 2)
+    assert uv.shape[0] == 8 and uv.shape[1] >= 2
     box = []
     for i in range(uv.shape[0]):
         box.append(tuple(uv[i, :].astype(np.int32)))
 
-    corner_map = {'ftr':0, 'ftl':1, 'btl':2, 'btr':3,
-              'fbr':4, 'fbl':5, 'bbl':6, 'bbr':7}
+    corner_map = {
+        "ftr": 0,
+        "ftl": 1,
+        "btl": 2,
+        "btr": 3,
+        "fbr": 4,
+        "fbl": 5,
+        "bbl": 6,
+        "bbr": 7,
+    }
     if draw_corners:
-        draw_point(img, box[corner_map['ftl']], [0, 0, 255], 3, 4) # [b,g,r]
-        draw_point(img, box[corner_map['ftr']], [0, 255, 0], 3, 4)
-        draw_point(img, box[corner_map['fbl']], [255, 0, 0], 3, 4)
-        draw_point(img, box[corner_map['fbr']], [255, 255, 0], 3, 4)
-        draw_point(img, box[corner_map['btl']], [0, 0, 128], 3, 4)
-        draw_point(img, box[corner_map['btr']], [0, 128, 0], 3, 4)
-        draw_point(img, box[corner_map['bbl']], [128, 0, 0], 3, 4)
-        draw_point(img, box[corner_map['bbr']], [255, 255, 0], 3, 4)
+        draw_point(img, box[corner_map["ftl"]], [0, 0, 255], 3, 4)  # [b,g,r]
+        draw_point(img, box[corner_map["ftr"]], [0, 255, 0], 3, 4)
+        draw_point(img, box[corner_map["fbl"]], [255, 0, 0], 3, 4)
+        draw_point(img, box[corner_map["fbr"]], [255, 255, 0], 3, 4)
+        draw_point(img, box[corner_map["btl"]], [0, 0, 128], 3, 4)
+        draw_point(img, box[corner_map["btr"]], [0, 128, 0], 3, 4)
+        draw_point(img, box[corner_map["bbl"]], [128, 0, 0], 3, 4)
+        draw_point(img, box[corner_map["bbr"]], [255, 255, 0], 3, 4)
 
     if draw_box:
-        cv2.line(img, box[corner_map['ftl']], box[corner_map['ftr']], color, line_width)
-        cv2.line(img, box[corner_map['ftl']], box[corner_map['fbl']], color, line_width)
-        cv2.line(img, box[corner_map['ftr']], box[corner_map['fbr']], color, line_width)
-        cv2.line(img, box[corner_map['fbl']], box[corner_map['fbr']], color, line_width)
-
-        cv2.line(img, box[corner_map['ftl']], box[corner_map['fbr']], color, line_width)
-        cv2.line(img, box[corner_map['ftr']], box[corner_map['fbl']], color, line_width)
-
-        cv2.line(img, box[corner_map['btl']], box[corner_map['btr']], color, line_width)
-        cv2.line(img, box[corner_map['btl']], box[corner_map['bbl']], color, line_width)
-        cv2.line(img, box[corner_map['btr']], box[corner_map['bbr']], color, line_width)
-        cv2.line(img, box[corner_map['bbl']], box[corner_map['bbr']], color, line_width)
-
-        cv2.line(img, box[corner_map['ftl']], box[corner_map['btl']], color, line_width)
-        cv2.line(img, box[corner_map['ftr']], box[corner_map['btr']], color, line_width)
-        cv2.line(img, box[corner_map['fbl']], box[corner_map['bbl']], color, line_width)
-        cv2.line(img, box[corner_map['fbr']], box[corner_map['bbr']], color, line_width)
+        cv2.line(img, box[corner_map["ftl"]], box[corner_map["ftr"]], color, line_width)
+        cv2.line(img, box[corner_map["ftl"]], box[corner_map["fbl"]], color, line_width)
+        cv2.line(img, box[corner_map["ftr"]], box[corner_map["fbr"]], color, line_width)
+        cv2.line(img, box[corner_map["fbl"]], box[corner_map["fbr"]], color, line_width)
+
+        cv2.line(img, box[corner_map["ftl"]], box[corner_map["fbr"]], color, line_width)
+        cv2.line(img, box[corner_map["ftr"]], box[corner_map["fbl"]], color, line_width)
+
+        cv2.line(img, box[corner_map["btl"]], box[corner_map["btr"]], color, line_width)
+        cv2.line(img, box[corner_map["btl"]], box[corner_map["bbl"]], color, line_width)
+        cv2.line(img, box[corner_map["btr"]], box[corner_map["bbr"]], color, line_width)
+        cv2.line(img, box[corner_map["bbl"]], box[corner_map["bbr"]], color, line_width)
+
+        cv2.line(img, box[corner_map["ftl"]], box[corner_map["btl"]], color, line_width)
+        cv2.line(img, box[corner_map["ftr"]], box[corner_map["btr"]], color, line_width)
+        cv2.line(img, box[corner_map["fbl"]], box[corner_map["bbl"]], color, line_width)
+        cv2.line(img, box[corner_map["fbr"]], box[corner_map["bbr"]], color, line_width)
 
 
-def draw_boxes(img, UV, color=[0,0,255], line_width=2, draw_corners=False):
+def draw_boxes(img, UV, color=[0, 0, 255], line_width=2, draw_corners=False):
     # UV: list of 8x2 np arrays corresponding to BB corners projected onto image coordinates
     for uv in UV:
         if uv is None:
             continue
-        draw_box(img, uv, color, line_width, draw_corners)
+        draw_box(img, uv, color, line_width, draw_corners)
```

### Comparing `asrl-pyboreas-1.0.4/setup.py` & `asrl-pyboreas-1.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 
 this_directory = Path(__file__).parent
 with open(str(this_directory / "README.md"), encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(
 	name='asrl-pyboreas',
-	version='1.0.4',
+	version='1.0.5',
 	description='A toolkit for working with the Boreas dataset in Python',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	author='Keenan Burnett, Andrew Li, Shichen Lu, Jingxing Qian, Yuchen Wu, David Yoon',
 	author_email='boreas@robotics.utias.utoronto.ca',
 	url='https://github.com/utiasASRL/boreas-devkit',
 	license='BSD',
 	packages=setuptools.find_packages(),
 	python_requires='>=3.8',
-	install_requires=["numpy>=1.21.0",
-					  "opencv-python>=4.5.3.56",
-					  "matplotlib>=3.4.2",
-					  "tqdm>=4.60.0",
-					  "pyproj>=3.1.0",
-					  "utm>=0.7.0",
-					  "asrl-pysteam>=1.0.4",
-					  "dash>=2.0.0"]
+	install_requires=[
+		"numpy>=1.21.0",
+		"opencv-python>=4.5.3.56",
+		"matplotlib>=3.4.2",
+		"asrl-pysteam>=1.1.0",
+	]
 )
```

