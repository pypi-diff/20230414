# Comparing `tmp/sbom4files-0.2.1-py2.py3-none-any.whl.zip` & `tmp/sbom4files-0.2.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11893 bytes, number of entries: 11
+Zip file size: 11999 bytes, number of entries: 11
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:03 sbom4files/__init__.py
 -rw-r--r--  2.0 unx     5579 b- defN 23-Feb-21 14:56 sbom4files/cli.py
--rw-r--r--  2.0 unx     6835 b- defN 23-Mar-23 18:55 sbom4files/filescanner.py
--rw-r--r--  2.0 unx      100 b- defN 23-Mar-23 22:51 sbom4files/version.py
+-rw-r--r--  2.0 unx     6782 b- defN 23-Apr-10 17:02 sbom4files/filescanner.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Apr-10 18:28 sbom4files/version.py
 -rw-r--r--  2.0 unx      217 b- defN 23-Mar-02 18:44 sbom4files/filetypes/filetypes.txt
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-27 14:06 sbom4files-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4916 b- defN 23-Mar-27 14:06 sbom4files-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-27 14:06 sbom4files-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Mar-27 14:06 sbom4files-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Mar-27 14:06 sbom4files-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      901 b- defN 23-Mar-27 14:06 sbom4files-0.2.1.dist-info/RECORD
-11 files, 30153 bytes uncompressed, 10363 bytes compressed:  65.6%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:13 sbom4files-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5296 b- defN 23-Apr-14 15:13 sbom4files-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:13 sbom4files-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Apr-14 15:13 sbom4files-0.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-14 15:13 sbom4files-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      901 b- defN 23-Apr-14 15:13 sbom4files-0.2.2.dist-info/RECORD
+11 files, 30480 bytes uncompressed, 10469 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: sbom4files/version.py
 Comment: 
 
 Filename: sbom4files/filetypes/filetypes.txt
 Comment: 
 
-Filename: sbom4files-0.2.1.dist-info/LICENSE
+Filename: sbom4files-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: sbom4files-0.2.1.dist-info/METADATA
+Filename: sbom4files-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: sbom4files-0.2.1.dist-info/WHEEL
+Filename: sbom4files-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: sbom4files-0.2.1.dist-info/entry_points.txt
+Filename: sbom4files-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbom4files-0.2.1.dist-info/top_level.txt
+Filename: sbom4files-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sbom4files-0.2.1.dist-info/RECORD
+Filename: sbom4files-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbom4files/filescanner.py

```diff
@@ -129,27 +129,26 @@
             found_license, found_copyright, copyright_text = self._find_licence(
                 filename
             )
             if found_license is not None:
                 for license in found_license:
                     self.sbom_file.set_licenseinfoinfile(license)
                     self.sbom_file.set_licensecomment(
-                        "<text>This information was automatically"
-                        " extracted from the file.</text>"
+                        "This information was automatically extracted from the file."
                     )
                 if len(found_license) == 1:
                     self.sbom_file.set_licenseconcluded(found_license[0])
                 else:
                     concluded_licence = " AND ".join(f for f in found_license)
                     self.sbom_file.set_licenseconcluded(concluded_licence)
             else:
                 # Default licence status
                 self.sbom_file.set_licenseinfoinfile("NONE")
                 self.sbom_file.set_licensecomment(
-                    "<text>Unable to determine license from the file.</text>"
+                    "Unable to determine license from the file."
                 )
                 self.sbom_file.set_licenseconcluded("NOASSERTION")
             if not found_copyright:
                 self.sbom_file.set_copyrighttext("NOASSERTION")
             else:
                 self.sbom_file.set_copyrighttext(copyright_text)
         return processed
```

## sbom4files/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.2.1"
+VERSION: str = "0.2.2"
```

## Comparing `sbom4files-0.2.1.dist-info/LICENSE` & `sbom4files-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbom4files-0.2.1.dist-info/METADATA` & `sbom4files-0.2.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbom4files
-Version: 0.2.1
+Version: 0.2.2
 Summary: SBOM generator for files in a directory
 Home-page: https://github.com/anthonyharrison/sbom4files
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lib4sbom (>=0.3.0)
+Requires-Dist: lib4sbom (>=0.3.1)
 Requires-Dist: python-magic
 
 # SBOM4Files
 
 SBOM4Files generates a SBOM (Software Bill of Materials) for a directory in a number of formats including
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org).
 It identifies all files within a directory and includes license and copyright information, where possible, for each file.
@@ -107,10 +107,13 @@
 
 ## Limitations
 
 This tool is meant to support software development and security audit functions. The usefulness of the tool is dependent on the SBOM data
 which is provided to the tool. Unfortunately, the tool is unable to determine the validity or completeness of such a SBOM file; users of the tool
 are therefore reminded that they should assert the quality of any data which is provided to the tool.
 
+When processing and validating licenses, the application will use a set of synonyms to attempt to map some license identifiers to the correct [SPDX License Identifiers](https://spdx.org/licenses/). However, the
+user of the tool is reminded that they should assert the quality of any data which is provided by the tool particularly where the license identifier has been modified.
+
 ## Feedback and Contributions
 
 Bugs and feature requests can be made via GitHub Issues.
```

