# Comparing `tmp/fabrictestbed-mflib-0.1.0b0.tar.gz` & `tmp/fabrictestbed-mflib-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-mflib-0.1.0b0.tar", last modified: Thu Apr 13 20:11:51 2023, max compression
+gzip compressed data, was "fabrictestbed-mflib-0.1.0b1.tar", last modified: Fri Apr 14 03:22:48 2023, max compression
```

## Comparing `fabrictestbed-mflib-0.1.0b0.tar` & `fabrictestbed-mflib-0.1.0b1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0      647 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.1.0b0/.gitignore
--rw-r--r--   0        0        0      145 2023-04-13 19:31:49.113559 fabrictestbed-mflib-0.1.0b0/.pypirc
--rw-r--r--   0        0        0      575 2023-03-29 18:17:09.721091 fabrictestbed-mflib-0.1.0b0/.readthedocs.yaml
--rw-r--r--   0        0        0     1071 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.1.0b0/LICENSE
--rw-r--r--   0        0        0       24 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.1.0b0/MANIFEST.in
--rw-r--r--   0        0        0   197138 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/MFLib.pdf
--rw-r--r--   0        0        0     3730 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/README.md
--rwxr-xr-x   0        0        0      817 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/create_html_doc.sh
--rwxr-xr-x   0        0        0      687 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/create_pdf_doc.sh
--rwxr-xr-x   0        0        0      668 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/create_release.sh
--rw-r--r--   0        0        0      638 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/docs/Makefile
--rw-r--r--   0        0        0      804 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/docs/make.bat
--rw-r--r--   0        0        0       55 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/docs/requirements.txt
-lrwxr-xr-x   0        0        0        0 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/docs/source/README.md -> ../../README.md
--rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/docs/source/_static/placeholder
--rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/docs/source/_templates/placeholder
--rw-r--r--   0        0        0     1297 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/docs/source/conf.py
--rw-r--r--   0        0        0      204 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/docs/source/core.rst
--rw-r--r--   0        0        0      262 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/docs/source/index.rst
--rw-r--r--   0        0        0      215 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/docs/source/mflib.rst
--rw-r--r--   0        0        0     7308 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b0/mflib/README.md
--rw-r--r--   0        0        0      539 2023-04-13 19:31:49.113559 fabrictestbed-mflib-0.1.0b0/mflib/__init__.py
--rw-r--r--   0        0        0    41613 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/mflib/core.py
--rw-r--r--   0        0        0    11653 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/mflib/mf_timestamp.py
--rw-r--r--   0        0        0    31859 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b0/mflib/mflib.py
--rw-r--r--   0        0        0    27967 2023-02-01 16:43:59.712079 fabrictestbed-mflib-0.1.0b0/mflib/mfvis.py
--rw-r--r--   0        0        0      735 2023-04-13 19:34:14.734792 fabrictestbed-mflib-0.1.0b0/pyproject.toml
--rw-r--r--   0        0        0       32 2023-02-01 16:43:59.712079 fabrictestbed-mflib-0.1.0b0/requirements.txt
--rw-r--r--   0        0        0     4240 1970-01-01 00:00:00.000000 fabrictestbed-mflib-0.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0      647 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.1.0b1/.gitignore
+-rw-r--r--   0        0        0      575 2023-03-29 18:17:09.721091 fabrictestbed-mflib-0.1.0b1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1071 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.1.0b1/LICENSE
+-rw-r--r--   0        0        0       24 2023-02-01 16:43:59.704079 fabrictestbed-mflib-0.1.0b1/MANIFEST.in
+-rw-r--r--   0        0        0   197131 2023-04-14 03:21:30.723292 fabrictestbed-mflib-0.1.0b1/MFLib.pdf
+-rw-r--r--   0        0        0     4071 2023-04-13 20:24:08.607249 fabrictestbed-mflib-0.1.0b1/README.md
+-rwxr-xr-x   0        0        0      817 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/create_html_doc.sh
+-rwxr-xr-x   0        0        0      687 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/create_pdf_doc.sh
+-rwxr-xr-x   0        0        0      668 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/create_release.sh
+-rw-r--r--   0        0        0      638 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/docs/make.bat
+-rw-r--r--   0        0        0       55 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/docs/requirements.txt
+lrwxr-xr-x   0        0        0        0 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/docs/source/README.md -> ../../README.md
+-rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/docs/source/_static/placeholder
+-rw-r--r--   0        0        0       41 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/docs/source/_templates/placeholder
+-rw-r--r--   0        0        0     1297 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/docs/source/conf.py
+-rw-r--r--   0        0        0      204 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/docs/source/core.rst
+-rw-r--r--   0        0        0      262 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/docs/source/index.rst
+-rw-r--r--   0        0        0      215 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/docs/source/mflib.rst
+-rw-r--r--   0        0        0     7308 2023-02-01 16:43:59.708079 fabrictestbed-mflib-0.1.0b1/mflib/README.md
+-rw-r--r--   0        0        0      539 2023-04-14 02:31:14.348369 fabrictestbed-mflib-0.1.0b1/mflib/__init__.py
+-rw-r--r--   0        0        0    41757 2023-04-14 02:31:55.528704 fabrictestbed-mflib-0.1.0b1/mflib/core.py
+-rw-r--r--   0        0        0    11653 2023-04-13 17:46:39.734392 fabrictestbed-mflib-0.1.0b1/mflib/mf_timestamp.py
+-rw-r--r--   0        0        0    31859 2023-04-14 02:22:04.816077 fabrictestbed-mflib-0.1.0b1/mflib/mflib.py
+-rw-r--r--   0        0        0    27967 2023-02-01 16:43:59.712079 fabrictestbed-mflib-0.1.0b1/mflib/mfvis.py
+-rw-r--r--   0        0        0      735 2023-04-13 19:34:14.734792 fabrictestbed-mflib-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-02-01 16:43:59.712079 fabrictestbed-mflib-0.1.0b1/requirements.txt
+-rw-r--r--   0        0        0     4581 1970-01-01 00:00:00.000000 fabrictestbed-mflib-0.1.0b1/PKG-INFO
```

### Comparing `fabrictestbed-mflib-0.1.0b0/.gitignore` & `fabrictestbed-mflib-0.1.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/.readthedocs.yaml` & `fabrictestbed-mflib-0.1.0b1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/LICENSE` & `fabrictestbed-mflib-0.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/MFLib.pdf` & `fabrictestbed-mflib-0.1.0b1/MFLib.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 18% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,9 +1,9 @@
 MFLib
-Release 0.1.0rc0
+Release 0.1.0b1
 
 Fabric UKY Team
 
 Apr 13, 2023
 
 CONTENTS
 
@@ -57,15 +57,15 @@
 
 Index
 
 14
 
 i
 
-MFLib, Release 0.1.0rc0
+MFLib, Release 0.1.0b1
 
 docs passing
 
 Welcome to the FABRIC Measurement Framework Library. MFLib makes it easy to install monitoring systems to a
 FABRIC experimenter’s slice. The monitoring system makes extensive use of industry standards such as Prometheus,
 Grafana, Elastic Search and Kibana while adding customized monitoring tools and dashboards for quick setup and
 visualization.
@@ -89,15 +89,16 @@
 
 1.2 FABRIC Learn Site
 FABRIC Knowledge Base
 
 1.3 MFLib Python Package Documentation
 Documentation for the package is presented in serveral different forms (and maybe include later in this document):
 • ReadTheDocs
-• MFLib.pdf
+• MFLib.pdf in the source code/GitHub.
+• MFLib HTML Index in the source code/GitHub.
 • Or you may build the documentation from the source code. See Sphinx Documentation later in this document.
 
 2
 
 CHAPTER
 
 TWO
@@ -126,42 +127,45 @@
 This package is documented using sphinx. The source directories are already created and populated with reStructuredText ( .rst ) files. The build directories are deleted and/or are not included in the repository,
 API documentation can also be found at https://fabrictestbed-mflib.readthedocs.io/.
 
 3.1.1 Build HTML Documents
 Install the extra packages required to build API docs: (sphinx, furo theme, and myst-parser for parsing markdown files):
 pip install -r docs/requirements.txt
 Build the documentation by running the following command from the root directory of the repo.
-sphinx-build -b html docs/source/ docs/build/html
+./create_html_doc.sh
 The completed documentation may be accessed by clicking on /docs/build/html/index.html
 
 3.1.2 Build PDF Document
 Latex must be installed. For Debian use:
 sudo apt install texlive-latex-extra
 sudo apt install latexmk
 
 Run the bash script to create the MFLIB.pdf documentation. MFLIB.pdf will be placed in the root directory of the
 repository.
 ./create_pdf_doc.sh
 
 4
 
-MFLib, Release 0.1.0rc0
+MFLib, Release 0.1.0b1
 
 3.2 Distribution Package
 MFLib package is created using Flit Be sure to create and commit the PDF documentation to GitHub before building
 and publishing to PyPi. The MFLib.pdf is included in the distributition.
 python3 -m pip install flit
 To build python package for PyPi run
-flit build
+./create_release.sh
 
 3.2.1 Uploading to PyPI
 First test the package by uploading to test.pypi.org then test the install.
 flit publish --repository testpypi
 Once install is good, upload to PiPy
-flit publish --repository pypi
+flit publish
+Note that Flit places a .pypirc file in your home directory if you do not already have one. Flit may also store your
+password in the keyring which may break if the password is changed. see Flit Controlling package uploads. The
+password can also be added to the .pypirc file. If password contains % signs it will break the .pypirc file.
 
 3.2. Distribution Package
 
 5
 
 CHAPTER
 
@@ -198,15 +202,15 @@
 Parameters
 slice_name (str) – The name of the slice to be monitored.
 Returns
 False if no Measure Node found or a init process fails. True otherwise.
 
 6
 
-MFLib, Release 0.1.0rc0
+MFLib, Release 0.1.0b1
 
 Return type
 Bool
 instrumentize(services=['prometheus', 'elk'])
 Instrumentize the slice. This is a convenience method that sets up & starts the monitoring of the slice. Sets
 up Prometheus, ELK & Grafana.
 Parameters
@@ -263,15 +267,15 @@
 String
 property common_hosts_file
 The full path to a local copy of the hosts.ini file.
 Returns
 The full path to a local copy of the hosts.ini file.
 Return type
 String
-core_class_version = '1.0.36'
+core_class_version = '1.0.37'
 An updatable version for debugging purposes to make sure the correct version of this file is being used.
 Anyone can update this value as they see fit. Should always be increasing.
 Returns
 Version.sub-version.build
 Return type
 String
 create(service, data=None, files=[])
@@ -279,15 +283,15 @@
 Parameters
 • service (String) – The name of the service.
 • data (JSON serializable object) –
 • files (List of Strings) – List of filepaths to be uploaded.
 
 8
 
-MFLib, Release 0.1.0rc0
+MFLib, Release 0.1.0b1
 
 Returns
 Dictionary of creation results.
 Return type
 dict
 download_log_file(service, method)
 Download the log file for the given service and method. Downloaded file will be stored locally for future
@@ -326,15 +330,15 @@
 info(service, data=None)
 Gets inormation from an existing service. Strictly gets information, does not change how the service is
 running.
 Parameters
 • service (String) – The name of the service.
 9
 
-MFLib, Release 0.1.0rc0
+MFLib, Release 0.1.0b1
 
 • data (JSON Serializable Object) – Data to be passed to a JSON file place in the
 service’s meas node directory.
 Returns
 Dictionary of info results.
 Return type
 dict
@@ -373,15 +377,15 @@
 property meas_node
 The fablib node object for the Measurement Node in the slice.
 Returns
 The fablib node object for the Measurement Node in the slice.
 
 10
 
-MFLib, Release 0.1.0rc0
+MFLib, Release 0.1.0b1
 
 Return type
 fablib.node
 property meas_node_ip
 The management ip address for the Measurement Node
 Returns
 ip address
@@ -420,15 +424,15 @@
 Return type
 List
 stop(services=[])
 Stops a service, does not remove the service, just stops it from using resources.
 
 11
 
-MFLib, Release 0.1.0rc0
+MFLib, Release 0.1.0b1
 
 Parameters
 services (List of Strings) – The names of the services to be stopped.
 Returns
 List of stop result dictionaries.
 Return type
 List
```

### Comparing `fabrictestbed-mflib-0.1.0b0/README.md` & `fabrictestbed-mflib-0.1.0b1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -47,16 +47,17 @@
 
 ```
 pip install -r docs/requirements.txt
 ```
 
 Build the documentation by running the following command from the root directory of the repo.
 ```
-sphinx-build -b html docs/source/ docs/build/html
-```  
+./create_html_doc.sh
+```
+
 The completed documentation may be accessed by clicking on `/docs/build/html/index.html`
 
 #### Build PDF Document
 Latex must be installed. For Debian use: 
 ```
 sudo apt install texlive-latex-extra 
 sudo apt install latexmk
@@ -72,21 +73,21 @@
 MFLib package is created using [Flit](https://flit.pypa.io/en/stable/)
 Be sure to create and commit the PDF documentation to GitHub before building and publishing to PyPi. The MFLib.pdf is included in the distributition.
 ```
 python3 -m pip install flit
 ```
 To build python package for PyPi run  
 ```
-flit build
+./create_release.sh
 ```
 
-
 #### Uploading to PyPI
 
 First test the package by uploading to test.pypi.org then test the install.
 ```
 flit publish --repository testpypi 
 ```
 Once install is good, upload to PiPy  
 ```
-flit publish --repository pypi 
+flit publish
 ```
+Note that Flit places a .pypirc file in your home directory if you do not already have one. Flit may also store your password in the keyring which may break if the password is changed. see [Flit Controlling package uploads](https://flit.pypa.io/en/stable/upload.html). The password can also be added to the .pypirc file. If password contains % signs it will break the .pypirc file.
```

### Comparing `fabrictestbed-mflib-0.1.0b0/create_html_doc.sh` & `fabrictestbed-mflib-0.1.0b1/create_html_doc.sh`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/create_pdf_doc.sh` & `fabrictestbed-mflib-0.1.0b1/create_pdf_doc.sh`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/create_release.sh` & `fabrictestbed-mflib-0.1.0b1/create_release.sh`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/docs/Makefile` & `fabrictestbed-mflib-0.1.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/docs/make.bat` & `fabrictestbed-mflib-0.1.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/docs/source/conf.py` & `fabrictestbed-mflib-0.1.0b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/mflib/README.md` & `fabrictestbed-mflib-0.1.0b1/mflib/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/mflib/__init__.py` & `fabrictestbed-mflib-0.1.0b1/mflib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 FABRIC Measurement Framework Python Client Library - Makes monitoring FABRIC Slice easy.
 """
 # release level is a alpha, b beta, rc candidate, dev development, post post,  or f final
 # (major, minor, micro, release level, release build)
-__version_info__ = [0, 1, 0, "b", 0]
+__version_info__ = [0, 1, 0, "b", 1]
 
 __version__ = f"{__version_info__[0]}.{__version_info__[1]}.{__version_info__[2]}"
 
 if __version_info__[3] != 'f':
     __version__ = f"{__version__}{__version_info__[3]}{__version_info__[4]}"
```

### Comparing `fabrictestbed-mflib-0.1.0b0/mflib/core.py` & `fabrictestbed-mflib-0.1.0b1/mflib/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 class Core:
     """
     MFLib core contains the core methods needed to create and interact with the Measurement Framework installed in a slice.
     It is not intended to be used by itself, but rather, it is the base object for creating Measurement Framework Library objects.
     """
 
-    core_class_version = "1.0.36"
+    core_class_version = "1.0.37"
 
     """
     An updatable version for debugging purposes to make sure the correct version of this file is being used. Anyone can update this value as they see fit.
     Should always be increasing.
 
     Returns:
         String: Version.sub-version.build
@@ -316,22 +316,24 @@
         private_key_file = ""
 
         extra_fm_vars = extra_fm.read_fabric_rc(extra_fm.default_fabric_rc)
         if extra_fm_vars:
             if "FABRIC_ALT_COPY_SSH_CONFIG" in extra_fm_vars:
                 ssh_config = extra_fm_vars["FABRIC_ALT_COPY_SSH_CONFIG"]
             else:
-                errmsg += "FABRIC_ALT_COPY_SSH_CONFIG not found in fabric_rc file. "
+                #errmsg += "FABRIC_ALT_COPY_SSH_CONFIG not found in fabric_rc file. "
+                ssh_config = "~/fabric_tunnel_config/tunnel_ssh_config"
 
             if "FABRIC_ALT_COPY_SLICE_PRIVATE_KEY_FILE" in extra_fm_vars:
                 private_key_file = extra_fm_vars[
                     "FABRIC_ALT_COPY_SLICE_PRIVATE_KEY_FILE"
                 ]
             else:
-                errmsg += "FABRIC_ALT_COPY_SLICE_PRIVATE_KEY_FILE not found in fabric_rc file. "
+                #errmsg += "FABRIC_ALT_COPY_SLICE_PRIVATE_KEY_FILE not found in fabric_rc file. "
+                private_key_file = "~/fabric_tunnel_config/slice_key"
 
         if errmsg:
             self.core_logger.error(
                 f"It appears you have not added alternate ssh config or slice key file locations to the fabric_rc file. {errmsg} "
             )
             return (
                 "It appears you have not added alternate ssh config or slice key file locations to the fabric_rc file. "
```

### Comparing `fabrictestbed-mflib-0.1.0b0/mflib/mf_timestamp.py` & `fabrictestbed-mflib-0.1.0b1/mflib/mf_timestamp.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/mflib/mflib.py` & `fabrictestbed-mflib-0.1.0b1/mflib/mflib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/mflib/mfvis.py` & `fabrictestbed-mflib-0.1.0b1/mflib/mfvis.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/pyproject.toml` & `fabrictestbed-mflib-0.1.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-mflib-0.1.0b0/PKG-INFO` & `fabrictestbed-mflib-0.1.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-mflib
-Version: 0.1.0b0
+Version: 0.1.0b1
 Summary: FABRIC Measurement Framework Python Client Library - Makes monitoring FABRIC Slice easy.
 Author: Song, Pinyi, Hussam
 Author-email: Carpenter <csacarp0@g.uky.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -60,16 +60,17 @@
 
 ```
 pip install -r docs/requirements.txt
 ```
 
 Build the documentation by running the following command from the root directory of the repo.
 ```
-sphinx-build -b html docs/source/ docs/build/html
-```  
+./create_html_doc.sh
+```
+
 The completed documentation may be accessed by clicking on `/docs/build/html/index.html`
 
 #### Build PDF Document
 Latex must be installed. For Debian use: 
 ```
 sudo apt install texlive-latex-extra 
 sudo apt install latexmk
@@ -85,22 +86,22 @@
 MFLib package is created using [Flit](https://flit.pypa.io/en/stable/)
 Be sure to create and commit the PDF documentation to GitHub before building and publishing to PyPi. The MFLib.pdf is included in the distributition.
 ```
 python3 -m pip install flit
 ```
 To build python package for PyPi run  
 ```
-flit build
+./create_release.sh
 ```
 
-
 #### Uploading to PyPI
 
 First test the package by uploading to test.pypi.org then test the install.
 ```
 flit publish --repository testpypi 
 ```
 Once install is good, upload to PiPy  
 ```
-flit publish --repository pypi 
+flit publish
 ```
+Note that Flit places a .pypirc file in your home directory if you do not already have one. Flit may also store your password in the keyring which may break if the password is changed. see [Flit Controlling package uploads](https://flit.pypa.io/en/stable/upload.html). The password can also be added to the .pypirc file. If password contains % signs it will break the .pypirc file.
```

