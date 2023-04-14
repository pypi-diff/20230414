# Comparing `tmp/TerraVide-0.0.3.tar.gz` & `tmp/TerraVide-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TerraVide-0.0.3.tar", last modified: Thu Apr 13 23:30:36 2023, max compression
+gzip compressed data, was "TerraVide-0.1.0.tar", last modified: Fri Apr 14 00:39:24 2023, max compression
```

## Comparing `TerraVide-0.0.3.tar` & `TerraVide-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 23:30:36.000000 TerraVide-0.0.3/
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1305 2023-04-13 23:30:36.000000 TerraVide-0.0.3/PKG-INFO
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 23:30:36.000000 TerraVide-0.0.3/terravide/
--rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-13 23:14:29.000000 TerraVide-0.0.3/terravide/__init__.py
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 23:30:36.000000 TerraVide-0.0.3/terravide/src/
--rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-13 20:29:35.000000 TerraVide-0.0.3/terravide/src/__init__.py
--rw-r--r--   0 sarangpramode   (501) staff       (20)     4188 2023-04-13 23:30:19.000000 TerraVide-0.0.3/terravide/src/dataset.py
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1823 2023-04-13 21:59:13.000000 TerraVide-0.0.3/terravide/src/info.py
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 23:30:36.000000 TerraVide-0.0.3/TerraVide.egg-info/
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1305 2023-04-13 23:30:36.000000 TerraVide-0.0.3/TerraVide.egg-info/PKG-INFO
--rw-r--r--   0 sarangpramode   (501) staff       (20)      247 2023-04-13 23:30:36.000000 TerraVide-0.0.3/TerraVide.egg-info/SOURCES.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)       15 2023-04-13 23:30:36.000000 TerraVide-0.0.3/TerraVide.egg-info/top_level.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)        1 2023-04-13 23:30:36.000000 TerraVide-0.0.3/TerraVide.egg-info/dependency_links.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)     2547 2023-04-13 23:30:31.000000 TerraVide-0.0.3/setup.py
--rw-r--r--   0 sarangpramode   (501) staff       (20)       38 2023-04-13 23:30:36.000000 TerraVide-0.0.3/setup.cfg
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1079 2023-04-13 21:41:11.000000 TerraVide-0.0.3/LICENSE.txt
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-14 00:39:24.484486 TerraVide-0.1.0/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1079 2023-04-13 21:41:11.000000 TerraVide-0.1.0/LICENSE.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1612 2023-04-14 00:39:24.484356 TerraVide-0.1.0/PKG-INFO
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-14 00:39:24.483620 TerraVide-0.1.0/TerraVide.egg-info/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1612 2023-04-14 00:39:24.000000 TerraVide-0.1.0/TerraVide.egg-info/PKG-INFO
+-rw-r--r--   0 sarangpramode   (501) staff       (20)      257 2023-04-14 00:39:24.000000 TerraVide-0.1.0/TerraVide.egg-info/SOURCES.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        1 2023-04-14 00:39:24.000000 TerraVide-0.1.0/TerraVide.egg-info/dependency_links.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        6 2023-04-14 00:39:24.000000 TerraVide-0.1.0/TerraVide.egg-info/requires.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)       13 2023-04-14 00:39:24.000000 TerraVide-0.1.0/TerraVide.egg-info/top_level.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)       38 2023-04-14 00:39:24.484525 TerraVide-0.1.0/setup.cfg
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     2615 2023-04-14 00:30:38.000000 TerraVide-0.1.0/setup.py
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-14 00:39:24.482534 TerraVide-0.1.0/terravide/
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-14 00:39:24.484177 TerraVide-0.1.0/terravide/src/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-13 20:29:35.000000 TerraVide-0.1.0/terravide/src/__init__.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     4331 2023-04-14 00:24:49.000000 TerraVide-0.1.0/terravide/src/dataset.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1823 2023-04-14 00:38:04.000000 TerraVide-0.1.0/terravide/src/info.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `TerraVide-0.0.3/terravide/src/dataset.py` & `TerraVide-0.1.0/terravide/src/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from os import path
 
 ########################################################################################################
 #    FTP functions
 ########################################################################################################
 
-def FTP_download_lasfile(filename, datayear=2017, folderpath="testD/"):
+def FTP_download_lasfile(filename, datayear=2017, folderpath="FTP_files/"):
     """Downlaod a las file from ftp.gis.ny.gov
 
     Args:
         filename (string): lasfile to download from ftp server
         datayear (_type_): which year to look at , 2017, 2021
         folderpath (_type_): where to download the file into
 
@@ -80,15 +80,15 @@
     #enter data directory
     ftp.cwd(ftp_datadir)
     
 
     filenames = ftp.nlst() # get filenames within the directory
     return filenames
 
-def FTP_list_files(datayear=2017):
+def FTP_list_files(datayear=2021):
     """List all files in the lidar directory of NYC scans
 
     Args:
         datayear (int, optional): _description_. Defaults to 2021.
 
     Returns:
         None: _description_
@@ -118,16 +118,22 @@
 if __name__ == '__main__':
 
     DEFAULT_FOLDER_PATH = "Datasets/FTP_files/LiDAR/"
     # Get Year Input from User
     year = int(input("Enter Desired YEAR [2017 and 2021 supported] : "))
     # Get List of filnames on FTP server
     filenames = FTP_GetFileList(year)
+
     # Prepare arguments
-    args = [(i, year,DEFAULT_FOLDER_PATH) for i in filenames]
+
+    #Download all files
+    #NOTE: This is a very slow process, use only if you want to download all files
+    #args = [(i, year,DEFAULT_FOLDER_PATH) for i in filenames]
+
+    #Download a single file
     args = [('25192.las', year,DEFAULT_FOLDER_PATH)]
 
     print("-------------------------")
     print("--DOWNLOADING FTP FILES--")
     print("-------------------------")
 
     with Pool(1) as p:
```

### Comparing `TerraVide-0.0.3/terravide/src/info.py` & `TerraVide-0.1.0/terravide/src/info.py`

 * *Files identical despite different names*

### Comparing `TerraVide-0.0.3/setup.py` & `TerraVide-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,22 +27,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TerraVide",                     # This is the name of the package
-    version="0.0.3",                        #release version
+    version="0.1.0",                        #release version
     author="Sarang Pramode",                     # Full name of the author
     description="An open source python package to process and simulate large urban environments mapped with LiDAR data",
     long_description = long_description,
     long_description_content_type = "text/markdown",
+    license='MIT',
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.6',                # Minimum version requirement of the package
-    py_modules=["info"],             # Name of the python package
-    install_requires=[]                     # Install other dependencies if any
-)
+    py_modules=["info","dataset"],             # Name of the python package
+    install_requires=[              # Install other dependencies if any
+        "numpy",
+
+    ]                     
+)
+
```

### Comparing `TerraVide-0.0.3/LICENSE.txt` & `TerraVide-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

