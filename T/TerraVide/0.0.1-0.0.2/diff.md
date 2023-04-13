# Comparing `tmp/TerraVide-0.0.1.tar.gz` & `tmp/TerraVide-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TerraVide-0.0.1.tar", last modified: Thu Apr 13 22:00:59 2023, max compression
+gzip compressed data, was "TerraVide-0.0.2.tar", last modified: Thu Apr 13 22:44:38 2023, max compression
```

## Comparing `TerraVide-0.0.1.tar` & `TerraVide-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 22:00:59.780259 TerraVide-0.0.1/
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1079 2023-04-13 21:41:11.000000 TerraVide-0.0.1/LICENSE.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)      382 2023-04-13 22:00:59.780134 TerraVide-0.0.1/PKG-INFO
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 22:00:59.779980 TerraVide-0.0.1/TerraVide.egg-info/
--rw-r--r--   0 sarangpramode   (501) staff       (20)      382 2023-04-13 22:00:59.000000 TerraVide-0.0.1/TerraVide.egg-info/PKG-INFO
--rw-r--r--   0 sarangpramode   (501) staff       (20)      152 2023-04-13 22:00:59.000000 TerraVide-0.0.1/TerraVide.egg-info/SOURCES.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)        1 2023-04-13 22:00:59.000000 TerraVide-0.0.1/TerraVide.egg-info/dependency_links.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)        5 2023-04-13 22:00:59.000000 TerraVide-0.0.1/TerraVide.egg-info/top_level.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)       38 2023-04-13 22:00:59.780293 TerraVide-0.0.1/setup.cfg
--rw-r--r--   0 sarangpramode   (501) staff       (20)     2384 2023-04-13 21:47:29.000000 TerraVide-0.0.1/setup.py
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 22:44:38.823810 TerraVide-0.0.2/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1079 2023-04-13 21:41:11.000000 TerraVide-0.0.2/LICENSE.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1152 2023-04-13 22:44:38.823618 TerraVide-0.0.2/PKG-INFO
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 22:44:38.823378 TerraVide-0.0.2/TerraVide.egg-info/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1152 2023-04-13 22:44:38.000000 TerraVide-0.0.2/TerraVide.egg-info/PKG-INFO
+-rw-r--r--   0 sarangpramode   (501) staff       (20)      152 2023-04-13 22:44:38.000000 TerraVide-0.0.2/TerraVide.egg-info/SOURCES.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        1 2023-04-13 22:44:38.000000 TerraVide-0.0.2/TerraVide.egg-info/dependency_links.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        5 2023-04-13 22:44:38.000000 TerraVide-0.0.2/TerraVide.egg-info/top_level.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)       38 2023-04-13 22:44:38.823855 TerraVide-0.0.2/setup.cfg
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     2547 2023-04-13 22:43:57.000000 TerraVide-0.0.2/setup.py
```

### Comparing `TerraVide-0.0.1/LICENSE.txt` & `TerraVide-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TerraVide-0.0.1/setup.py` & `TerraVide-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,19 +22,24 @@
 # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 #
 #------------------------------------------------------------------------------------------------------------------------------
 
 import setuptools
 
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
 setuptools.setup(
     name="TerraVide",                     # This is the name of the package
-    version="0.0.1",                        #release version
+    version="0.0.2",                        #release version
     author="Sarang Pramode",                     # Full name of the author
     description="An open source python package to process and simulate large urban environments mapped with LiDAR data",
+    long_description = long_description,
+    long_description_content_type = "text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.6',                # Minimum version requirement of the package
```

