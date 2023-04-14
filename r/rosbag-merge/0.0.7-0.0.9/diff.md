# Comparing `tmp/rosbag_merge-0.0.7.tar.gz` & `tmp/rosbag_merge-0.0.9.tar.gz`

## Comparing `rosbag_merge-0.0.7.tar` & `rosbag_merge-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/INSTALL.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/requirements.txt
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/.github/workflows/publish-to-pypi-and-test-pypi.yml
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/examples/main_direct.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/src/rosbag_merge/__init__.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/src/rosbag_merge/bag_stream.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/src/rosbag_merge/csv_merge.py
--rwxr-xr-x   0        0        0     6382 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/src/rosbag_merge/main.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/src/rosbag_merge/merge_bags.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/src/rosbag_merge/rosbag_to_csv.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/tests/topic_list.txt
--rw-r--r--   0        0        0    20625 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag
--rw-r--r--   0        0        0   331893 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag
--rw-r--r--   0        0        0   121303 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/.gitignore
--rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/LICENSE
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/README.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    16001 2020-02-02 00:00:00.000000 rosbag_merge-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/INSTALL.md
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/.github/workflows/publish-to-pypi-and-test-pypi.yml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/examples/main_direct.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/src/rosbag_merge/__init__.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/src/rosbag_merge/bag_stream.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/src/rosbag_merge/csv_merge.py
+-rwxr-xr-x   0        0        0     6382 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/src/rosbag_merge/main.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/src/rosbag_merge/merge_bags.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/src/rosbag_merge/rosbag_to_csv.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/tests/topic_list.txt
+-rw-r--r--   0        0        0    20625 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag
+-rw-r--r--   0        0        0   331893 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag
+-rw-r--r--   0        0        0   121303 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/.gitignore
+-rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/README.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    16023 2020-02-02 00:00:00.000000 rosbag_merge-0.0.9/PKG-INFO
```

### Comparing `rosbag_merge-0.0.7/.github/workflows/publish-to-pypi-and-test-pypi.yml` & `rosbag_merge-0.0.9/.github/workflows/publish-to-pypi-and-test-pypi.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 name: Publish rosbag-merge 📦 to to PyPI and TestPyPI
 
-on: release
+on:
+  push:
+    tags:        
+      - 'v*'
 
 jobs:
   build-n-publish:
     name: Build and publish rosbag-merge 📦 to to PyPI and TestPyPI
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@main
```

### Comparing `rosbag_merge-0.0.7/examples/main_direct.py` & `rosbag_merge-0.0.9/examples/main_direct.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.7/src/rosbag_merge/bag_stream.py` & `rosbag_merge-0.0.9/src/rosbag_merge/bag_stream.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.7/src/rosbag_merge/csv_merge.py` & `rosbag_merge-0.0.9/src/rosbag_merge/csv_merge.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.7/src/rosbag_merge/main.py` & `rosbag_merge-0.0.9/src/rosbag_merge/main.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.7/src/rosbag_merge/merge_bags.py` & `rosbag_merge-0.0.9/src/rosbag_merge/merge_bags.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.7/src/rosbag_merge/rosbag_to_csv.py` & `rosbag_merge-0.0.9/src/rosbag_merge/rosbag_to_csv.py`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.7/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag` & `rosbag_merge-0.0.9/tests/data/raw/TB3_WAFFLE_SLAM_cmd_vel_only.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.7/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag` & `rosbag_merge-0.0.9/tests/data/raw/TB3_WAFFLE_SLAM_imu_only.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.7/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag` & `rosbag_merge-0.0.9/tests/data/raw/TB3_WAFFLE_SLAM_odom_tf_static.bag`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.7/LICENSE` & `rosbag_merge-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.7/README.md` & `rosbag_merge-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rosbag_merge-0.0.7/pyproject.toml` & `rosbag_merge-0.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project]
 # add the distribution name of the package, the tar ball and python wheel use this name, this name goes the /home/$USER/.local/lib/python3.8/site-packages/
 name = "rosbag_merge"
 
 # version is the package version. See the version specifier specification
 # for more details on versions. Some build backends allow it to be 
 # specified another way, such as from a file or a git tag.
-version = "0.0.7"
+version = "0.0.9"
 authors = [
   { name="Jonathan Sanabria", email="jonsanria@gmail.com" },
 ]
 description = "A gathering of tools for merging rosbags and saving their topic information to csv."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `rosbag_merge-0.0.7/PKG-INFO` & `rosbag_merge-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosbag_merge
-Version: 0.0.7
+Version: 0.0.9
 Summary: A gathering of tools for merging rosbags and saving their topic information to csv.
 Project-URL: Homepage, https://github.com/1hada/rosbag-merge/
 Project-URL: Bug Tracker, https://github.com/1hada/rosbag-merge/issues/
 Author-email: Jonathan Sanabria <jonsanria@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -191,14 +191,15 @@
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
+License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: dask
```

