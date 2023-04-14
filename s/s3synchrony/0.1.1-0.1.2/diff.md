# Comparing `tmp/s3synchrony-0.1.1.tar.gz` & `tmp/s3synchrony-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\s3synchrony-0.1.1.tar", last modified: Tue Jan 18 18:17:38 2022, max compression
+gzip compressed data, was "s3synchrony-0.1.2.tar", last modified: Fri Apr 14 21:09:40 2023, max compression
```

## Comparing `s3synchrony-0.1.1.tar` & `s3synchrony-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-01-18 18:17:38.868265 s3synchrony-0.1.1/
--rw-rw-rw-   0        0        0     1937 2022-01-15 22:25:08.000000 s3synchrony-0.1.1/.gitignore
--rw-rw-rw-   0        0        0    35849 2022-01-15 22:26:15.000000 s3synchrony-0.1.1/COPYING.txt
--rw-rw-rw-   0        0        0    35564 2022-01-15 22:26:08.000000 s3synchrony-0.1.1/LICENSE.md
--rw-rw-rw-   0        0        0     6123 2022-01-18 18:17:38.867262 s3synchrony-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5670 2022-01-18 03:04:51.000000 s3synchrony-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-01-18 18:17:38.862265 s3synchrony-0.1.1/s3synchrony.egg-info/
--rw-rw-rw-   0        0        0     6123 2022-01-18 18:17:38.000000 s3synchrony-0.1.1/s3synchrony.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2022-01-18 18:17:38.000000 s3synchrony-0.1.1/s3synchrony.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-18 18:17:38.000000 s3synchrony-0.1.1/s3synchrony.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2022-01-18 18:17:38.000000 s3synchrony-0.1.1/s3synchrony.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-18 18:17:38.868265 s3synchrony-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      625 2022-01-18 18:17:27.000000 s3synchrony-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-18 18:17:38.863262 s3synchrony-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2022-01-18 18:17:38.866261 s3synchrony-0.1.1/src/DataPlatforms/
--rw-rw-rw-   0        0        0     2934 2022-01-15 22:25:08.000000 s3synchrony-0.1.1/src/DataPlatforms/baseconn.py
--rw-rw-rw-   0        0        0    40648 2022-01-18 02:01:19.000000 s3synchrony-0.1.1/src/DataPlatforms/s3conn.py
--rw-rw-rw-   0        0        0     2770 2022-01-15 22:25:08.000000 s3synchrony-0.1.1/src/s3synchrony.py
+drwxrwxrwx   0        0        0        0 2023-04-14 21:09:40.039103 s3synchrony-0.1.2/
+-rw-rw-rw-   0        0        0    35849 2023-04-14 20:57:23.000000 s3synchrony-0.1.2/COPYING.txt
+-rw-rw-rw-   0        0        0    35564 2023-04-14 20:57:23.000000 s3synchrony-0.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0     6100 2023-04-14 21:09:40.039103 s3synchrony-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5670 2023-04-14 20:57:23.000000 s3synchrony-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 21:09:40.023101 s3synchrony-0.1.2/s3synchrony/
+drwxrwxrwx   0        0        0        0 2023-04-14 21:09:40.039103 s3synchrony-0.1.2/s3synchrony/DataPlatforms/
+-rw-rw-rw-   0        0        0        0 2023-04-14 21:00:59.000000 s3synchrony-0.1.2/s3synchrony/DataPlatforms/__init__.py
+-rw-rw-rw-   0        0        0     2934 2023-04-14 20:57:23.000000 s3synchrony-0.1.2/s3synchrony/DataPlatforms/baseconn.py
+-rw-rw-rw-   0        0        0    40648 2023-04-14 20:57:23.000000 s3synchrony-0.1.2/s3synchrony/DataPlatforms/s3conn.py
+-rw-rw-rw-   0        0        0       26 2023-04-14 21:09:14.000000 s3synchrony-0.1.2/s3synchrony/__init__.py
+-rw-rw-rw-   0        0        0     2772 2023-04-14 20:58:47.000000 s3synchrony-0.1.2/s3synchrony/s3synchrony.py
+drwxrwxrwx   0        0        0        0 2023-04-14 21:09:40.035101 s3synchrony-0.1.2/s3synchrony.egg-info/
+-rw-rw-rw-   0        0        0     6100 2023-04-14 21:09:39.000000 s3synchrony-0.1.2/s3synchrony.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-04-14 21:09:39.000000 s3synchrony-0.1.2/s3synchrony.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 21:09:39.000000 s3synchrony-0.1.2/s3synchrony.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 21:09:39.000000 s3synchrony-0.1.2/s3synchrony.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 21:09:40.043103 s3synchrony-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-04-14 21:09:21.000000 s3synchrony-0.1.2/setup.py
```

### Comparing `s3synchrony-0.1.1/COPYING.txt` & `s3synchrony-0.1.2/COPYING.txt`

 * *Files identical despite different names*

### Comparing `s3synchrony-0.1.1/LICENSE.md` & `s3synchrony-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `s3synchrony-0.1.1/PKG-INFO` & `s3synchrony-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: s3synchrony
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package provides a service for synchronizing file creations, deletions, and modifications across users on an AWS S3 prefix.
 Home-page: https://github.com/SevanBrodjian/s3synchrony
 Author: Sevan Brodjian
 Author-email: sevanbro7@gmail.com
 License: LICENSE.md
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: COPYING.txt
 
 # S3Synchrony
 
 _Created by Sevan Brodjian for Ameren at the Innovation Center @ UIUC_
@@ -135,9 +134,7 @@
 Resetting all S3Synchrony services is as simple as deleting the .S3 folders contained locally and on S3. Once these are deleted, synchronization cannot occur until they are recreated, which can be done by simply making a new call to S3Synchrony.
 
 Before resetting, however, a call to reset_confirm **must** occur. The user will then be prompted to confirm that they would like their .S3 folders removed.
 
 ## License
 
 [GNU GPLv3](https://www.gnu.org/licenses/)
-
-
```

### Comparing `s3synchrony-0.1.1/README.md` & `s3synchrony-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `s3synchrony-0.1.1/s3synchrony.egg-info/PKG-INFO` & `s3synchrony-0.1.2/s3synchrony.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: s3synchrony
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package provides a service for synchronizing file creations, deletions, and modifications across users on an AWS S3 prefix.
 Home-page: https://github.com/SevanBrodjian/s3synchrony
 Author: Sevan Brodjian
 Author-email: sevanbro7@gmail.com
 License: LICENSE.md
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: COPYING.txt
 
 # S3Synchrony
 
 _Created by Sevan Brodjian for Ameren at the Innovation Center @ UIUC_
@@ -135,9 +134,7 @@
 Resetting all S3Synchrony services is as simple as deleting the .S3 folders contained locally and on S3. Once these are deleted, synchronization cannot occur until they are recreated, which can be done by simply making a new call to S3Synchrony.
 
 Before resetting, however, a call to reset_confirm **must** occur. The user will then be prompted to confirm that they would like their .S3 folders removed.
 
 ## License
 
 [GNU GPLv3](https://www.gnu.org/licenses/)
-
-
```

### Comparing `s3synchrony-0.1.1/setup.py` & `s3synchrony-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
       long_description = fh.read()
 
 setuptools.setup(
       name='s3synchrony',
-      version='0.1.1',
+      version='0.1.2',
       description='This package provides a service for synchronizing file creations, deletions, and modifications across users on an AWS S3 prefix.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Sevan Brodjian',
       author_email='sevanbro7@gmail.com',
       url='https://github.com/SevanBrodjian/s3synchrony',
       packages=setuptools.find_packages(),
```

### Comparing `s3synchrony-0.1.1/src/DataPlatforms/baseconn.py` & `s3synchrony-0.1.2/s3synchrony/DataPlatforms/baseconn.py`

 * *Files identical despite different names*

### Comparing `s3synchrony-0.1.1/src/DataPlatforms/s3conn.py` & `s3synchrony-0.1.2/s3synchrony/DataPlatforms/s3conn.py`

 * *Files identical despite different names*

### Comparing `s3synchrony-0.1.1/src/s3synchrony.py` & `s3synchrony-0.1.2/s3synchrony/s3synchrony.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from DataPlatforms import baseconn
-from DataPlatforms import s3conn
+from .DataPlatforms import baseconn
+from .DataPlatforms import s3conn
 
 
 _supported_platforms = {"S3": s3conn.S3Connection}
 
 
 def get_supported_platforms():
     """Return a list of the supported data platforms."""
```

