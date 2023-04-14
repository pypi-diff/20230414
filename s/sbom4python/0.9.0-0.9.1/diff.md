# Comparing `tmp/sbom4python-0.9.0-py2.py3-none-any.whl.zip` & `tmp/sbom4python-0.9.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 40501 bytes, number of entries: 14
+Zip file size: 40715 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:00 sbom4python/__init__.py
 -rw-r--r--  2.0 unx     4573 b- defN 23-Mar-26 14:18 sbom4python/cli.py
 -rw-r--r--  2.0 unx     1820 b- defN 23-Jan-11 12:22 sbom4python/license.py
--rw-r--r--  2.0 unx     9319 b- defN 23-Mar-23 23:00 sbom4python/scanner.py
--rw-r--r--  2.0 unx      100 b- defN 23-Mar-18 12:37 sbom4python/version.py
+-rw-r--r--  2.0 unx     9607 b- defN 23-Apr-13 13:20 sbom4python/scanner.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Apr-10 18:34 sbom4python/version.py
 -rw-r--r--  2.0 unx   222585 b- defN 22-Oct-14 16:39 sbom4python/license_data/spdx_licenses.json
 -rw-r--r--  2.0 unx       75 b- defN 23-Mar-21 14:58 test/__init__.py
 -rw-r--r--  2.0 unx     1976 b- defN 23-Mar-21 16:30 test/test_license.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-27 14:04 sbom4python-0.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5910 b- defN 23-Mar-27 14:04 sbom4python-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-27 14:04 sbom4python-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Mar-27 14:04 sbom4python-0.9.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Mar-27 14:04 sbom4python-0.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1146 b- defN 23-Mar-27 14:04 sbom4python-0.9.0.dist-info/RECORD
-14 files, 259112 bytes uncompressed, 38597 bytes compressed:  85.1%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:13 sbom4python-0.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6301 b- defN 23-Apr-14 15:13 sbom4python-0.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:13 sbom4python-0.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Apr-14 15:13 sbom4python-0.9.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-14 15:13 sbom4python-0.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1146 b- defN 23-Apr-14 15:13 sbom4python-0.9.1.dist-info/RECORD
+14 files, 259791 bytes uncompressed, 38811 bytes compressed:  85.1%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_license.py
 Comment: 
 
-Filename: sbom4python-0.9.0.dist-info/LICENSE
+Filename: sbom4python-0.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: sbom4python-0.9.0.dist-info/METADATA
+Filename: sbom4python-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: sbom4python-0.9.0.dist-info/WHEEL
+Filename: sbom4python-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: sbom4python-0.9.0.dist-info/entry_points.txt
+Filename: sbom4python-0.9.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbom4python-0.9.0.dist-info/top_level.txt
+Filename: sbom4python-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sbom4python-0.9.0.dist-info/RECORD
+Filename: sbom4python-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbom4python/scanner.py

```diff
@@ -46,16 +46,20 @@
         # See https://stackoverflow.com/questions/1207457/convert-a-unicode-string-to-a-string-in-python-containing-extra-symbols
         # And convert byte object to a string
         name_str = (
             unicodedata.normalize("NFKD", supplier_info)
             .encode("ascii", "ignore")
             .decode("utf-8")
         )
-        # Get names
-        names = re.findall(r"[a-zA-Z\.\]+ [A-Za-z]+ ", name_str)
+        if " " in name_str:
+            # Get names assumed to be at least two names <first> <surname>
+            names = re.findall(r"[a-zA-Z\.\]+ [A-Za-z]+ ", name_str)
+        else:
+            # Handle case where only single name provided
+            names = [name_str]
         # Get email addresses
         # Use RFC-5322 compliant regex (https://regex101.com/library/6EL6YF)
         emails = re.findall(
             r"((?:[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*|\"(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21\x23-\x5b\x5d-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])*\")@(?:(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?|\[(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?|[a-z0-9-]*[a-z0-9]:(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21-\x5a\x53-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])+)\]))",
             supplier_info,
         )
         supplier = " ".join(n for n in names)
@@ -80,27 +84,29 @@
             if self.debug:
                 print(f"Metadata for {module}\n{self.metadata}")
             self.sbom_package.initialise()
             package = self.get("Name").lower().replace("_", "-")
             version = self.get("Version")
             self.sbom_package.set_name(package)
             self.sbom_package.set_version(version)
+            if parent == "-":
+                self.sbom_package.set_type("application")
             self.sbom_package.set_filesanalysis(self.include_file)
             license = self.license.find_license(self.get("License"))
             # Report license as reported by metadata. If not valid SPDX, report NOASSERTION
             if license != self.get("License"):
                 self.sbom_package.set_licensedeclared("NOASSERTION")
             else:
                 self.sbom_package.set_licensedeclared(license)
             # Report license if valid SPDX identifier
             self.sbom_package.set_licenseconcluded(license)
             # Add comment if metadata license was modified
             if len(self.get("License")) > 0 and license != self.get("License"):
                 self.sbom_package.set_licensecomments(
-                    f"{self.get('Name')} declares {self.get('License')} which is not a valid SPDX License identifier or expression."
+                    f"{self.get('Name')} declares {self.get('License')} which is not currently a valid SPDX License identifier or expression."
                 )
             supplier = self.get("Author") + " " + self.get("Author-email")
             if len(supplier.split()) > 3:
                 self.sbom_package.set_supplier(
                     "Organization", self._format_supplier(supplier)
                 )
             elif len(supplier) > 1:
```

## sbom4python/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.9.0"
+VERSION: str = "0.9.1"
```

## Comparing `sbom4python-0.9.0.dist-info/LICENSE` & `sbom4python-0.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbom4python-0.9.0.dist-info/METADATA` & `sbom4python-0.9.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbom4python
-Version: 0.9.0
+Version: 0.9.1
 Summary: SBOM generator for Python modules
 Home-page: https://github.com/anthonyharrison/sbom4python
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -20,16 +20,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lib4sbom (>=0.3.0)
-Requires-Dist: sbom4files
+Requires-Dist: lib4sbom (>=0.3.1)
+Requires-Dist: sbom4files (>=0.2.2)
 Requires-Dist: sbom2dot
 
 # SBOM4Python
 
 The SBOM4Python is a free, open source tool to generate a
 SBOM (Software Bill of Materials) for an installed Python module in a number of formats including
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org).
@@ -96,15 +96,15 @@
 The `--output-file` option is used to control the destination of the output generated by the tool. The
 default is to report to the console but can be stored in a file (specified using `--output-file` option).
 
 The tool attempts to determine the license of each module. This can be suppressed using the `--exclude-license` option in
 which case all licences are reported as 'NOASSERTION'.
 
 The tool can optionally include the files associated with the installed module. This can be specified using the `--include-file` option. As the filenames are
-relative to the directory in which the tool is invoked, it is recommended that the tool is launced in a directory where the source files are available.
+relative to the directory in which the tool is invoked, it is recommended that the tool is launched in a directory where the source files are available.
 
 The `--graph` option is used to generate a dependency graph of the components within the SBOM. The format of the graph
 file is compatible with the [DOT language](https://graphviz.org/doc/info/lang.html) used by the
 [GraphViz](https://graphviz.org/) application.
 
 ## Licence
 
@@ -115,13 +115,16 @@
 
 ## Limitations
 
 This tool is meant to support software development and security audit functions. However the usefulness of the tool is dependent on the SBOM data
 which is provided to the tool. Unfortunately, the tool is unable to determine the validity or completeness of such a SBOM file; users of the tool
 are therefore reminded that they should assert the quality of any data which is provided to the tool.
 
+When processing and validating licenses, the application will use a set of synonyms to attempt to map some license identifiers to the correct [SPDX License Identifiers](https://spdx.org/licenses/). However, the
+user of the tool is reminded that they should assert the quality of any data which is provided by the tool particularly where the license identifier has been modified.
+
 Whilst [PURL](https://github.com/package-url/purl-spec) and [CPE](https://nvd.nist.gov/products/cpe) references are automatically generated for each Python module, the accuracy
 of such references cannot be guaranteed as they are dependent on the validity of the data associated with the Python module.
 
 ## Feedback and Contributions
 
 Bugs and feature requests can be made via GitHub Issues.
```

## Comparing `sbom4python-0.9.0.dist-info/RECORD` & `sbom4python-0.9.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 sbom4python/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
 sbom4python/cli.py,sha256=qu34b36ENBKAMFS835ArVhu7pjpqHznK8wdtQKucwME,4573
 sbom4python/license.py,sha256=5XRAwuvRNd4nt2T7shMQr3jUo9dEMstZF5Hov3IzvIw,1820
-sbom4python/scanner.py,sha256=KfyQJhTyEgTgpXzosM8vVEDfHPZSpF0IYV1-N3e5mLY,9319
-sbom4python/version.py,sha256=OXS1vXaXVYHDVNZuL9ZKGU_C-RcA4ZtR-6rhyBtQI50,100
+sbom4python/scanner.py,sha256=Ub0gyH-pg-YBopfBvesJuGUqfgAHKPxpktF-WnYLrbY,9607
+sbom4python/version.py,sha256=yepdnyC7o4OD8LXWeMAliMLJmFekDrf4Yw5jUW-0KGs,100
 sbom4python/license_data/spdx_licenses.json,sha256=mj836L9ndKZMZBORMqUkjzP0n23RRhleuBdXlER0pVE,222585
 test/__init__.py,sha256=Jdm3si-iktHDtKWwHpYgVfLYF-l1bE6TQDJASgkVpQU,75
 test/test_license.py,sha256=stWDum_UwVGZZsTyjrVICgBh3Azb6dUqZIMK_DUQe4s,1976
-sbom4python-0.9.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbom4python-0.9.0.dist-info/METADATA,sha256=qhteMW91JUkRQlrHbUm10ls7eO1klOUFIJoDHoXfet4,5910
-sbom4python-0.9.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-sbom4python-0.9.0.dist-info/entry_points.txt,sha256=_83UfxTjM06vaj0t1XlOO3YmniXkM1jsyvTdkee7tmk,53
-sbom4python-0.9.0.dist-info/top_level.txt,sha256=udvkgWvzv7RUbiqpZ-ANkgXwwk5fFhl2LiQkh8dJGQg,12
-sbom4python-0.9.0.dist-info/RECORD,,
+sbom4python-0.9.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbom4python-0.9.1.dist-info/METADATA,sha256=FZFSmh6NzSk_lvqQZ6X9ZPloKcR47uLqbiUZKfIll68,6301
+sbom4python-0.9.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+sbom4python-0.9.1.dist-info/entry_points.txt,sha256=_83UfxTjM06vaj0t1XlOO3YmniXkM1jsyvTdkee7tmk,53
+sbom4python-0.9.1.dist-info/top_level.txt,sha256=udvkgWvzv7RUbiqpZ-ANkgXwwk5fFhl2LiQkh8dJGQg,12
+sbom4python-0.9.1.dist-info/RECORD,,
```

