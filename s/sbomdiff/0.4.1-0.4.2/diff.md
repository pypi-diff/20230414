# Comparing `tmp/sbomdiff-0.4.1-py2.py3-none-any.whl.zip` & `tmp/sbomdiff-0.4.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13375 bytes, number of entries: 12
+Zip file size: 13521 bytes, number of entries: 12
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-02 07:31 sbomdiff/__init__.py
--rw-r--r--  2.0 unx     5680 b- defN 22-Oct-20 16:05 sbomdiff/cli.py
--rw-r--r--  2.0 unx     4440 b- defN 23-Mar-23 23:07 sbomdiff/cyclonedx_parser.py
+-rw-r--r--  2.0 unx     6174 b- defN 23-Apr-10 17:04 sbomdiff/cli.py
+-rw-r--r--  2.0 unx     4470 b- defN 23-Mar-28 20:15 sbomdiff/cyclonedx_parser.py
 -rw-r--r--  2.0 unx     1298 b- defN 22-Oct-20 16:02 sbomdiff/output.py
--rw-r--r--  2.0 unx     7803 b- defN 22-Oct-20 16:30 sbomdiff/spdx_parser.py
--rw-r--r--  2.0 unx      100 b- defN 23-Mar-23 20:55 sbomdiff/version.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-27 14:15 sbomdiff-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6336 b- defN 23-Mar-27 14:15 sbomdiff-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-27 14:15 sbomdiff-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Mar-27 14:15 sbomdiff-0.4.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Mar-27 14:15 sbomdiff-0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      949 b- defN 23-Mar-27 14:15 sbomdiff-0.4.1.dist-info/RECORD
-12 files, 38129 bytes uncompressed, 11785 bytes compressed:  69.1%
+-rw-r--r--  2.0 unx     7841 b- defN 23-Apr-13 20:22 sbomdiff/spdx_parser.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Apr-10 18:30 sbomdiff/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:13 sbomdiff-0.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6336 b- defN 23-Apr-14 15:13 sbomdiff-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:13 sbomdiff-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Apr-14 15:13 sbomdiff-0.4.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-14 15:13 sbomdiff-0.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      949 b- defN 23-Apr-14 15:13 sbomdiff-0.4.2.dist-info/RECORD
+12 files, 38691 bytes uncompressed, 11931 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: sbomdiff/spdx_parser.py
 Comment: 
 
 Filename: sbomdiff/version.py
 Comment: 
 
-Filename: sbomdiff-0.4.1.dist-info/LICENSE
+Filename: sbomdiff-0.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: sbomdiff-0.4.1.dist-info/METADATA
+Filename: sbomdiff-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: sbomdiff-0.4.1.dist-info/WHEEL
+Filename: sbomdiff-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: sbomdiff-0.4.1.dist-info/entry_points.txt
+Filename: sbomdiff-0.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbomdiff-0.4.1.dist-info/top_level.txt
+Filename: sbomdiff-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sbomdiff-0.4.1.dist-info/RECORD
+Filename: sbomdiff-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbomdiff/cli.py

```diff
@@ -67,24 +67,28 @@
         "debug": False,
     }
     raw_args = parser.parse_args(argv[1:])
     args = {key: value for key, value in vars(raw_args).items() if value}
     args = ChainMap(args, defaults)
 
     # Validate CLI parameters
-
-    # Check both files exist
-    file_found = True
-    if not pathlib.Path(args["FILE1"]).exists():
-        print(f"{args['FILE1']} does not exist")
-        file_found = False
-    if not pathlib.Path(args["FILE2"]).exists():
-        print(f"{args['FILE2']} does not exist")
-        file_found = False
-    if not file_found:
+    if args["FILE1"] != args["FILE2"]:
+        # Check both files exist
+        file_found = True
+        if not pathlib.Path(args["FILE1"]).exists():
+            print(f"{args['FILE1']} does not exist")
+            file_found = False
+        if not pathlib.Path(args["FILE2"]).exists():
+            print(f"{args['FILE2']} does not exist")
+            file_found = False
+        if not file_found:
+            return -1
+    else:
+        # Same filename specified
+        print("Must specify different filenames")
         return -1
 
     spdx = SPDXParser()
     cyclonedx = CycloneDXParser()
 
     if args["sbom"] == "spdx":
         file1_type = file2_type = "SPDX"
@@ -128,34 +132,42 @@
 
     for package in packages1:
         if package in packages2:
             # Compare values for common package
             version1, license1 = packages1[package]
             version2, license2 = packages2[package]
             if version1 != version2:
+                if len(version1) == 0:
+                    version1 = "UNKNOWN"
+                if len(version2) == 0:
+                    version2 = "UNKNOWN"
                 sbom_out.send_output(
                     f"[VERSION] {package}: "
                     f"Version changed from {version1} to {version2}"
                 )
                 version_changes += 1
             if not args["exclude_license"] and license1 != license2:
                 sbom_out.send_output(
                     f"[LICENSE] {package}: "
                     f"License changed from {license1} to {license2}"
                 )
                 license_changes += 1
         else:
             # Package must have been removed
             version1, license1 = packages1[package]
+            if len(version1) == 0:
+                version1 = "UNKNOWN"
             sbom_out.send_output(f"[REMOVED] {package}: (Version {version1})")
             removed_packages += 1
     # Check for any new packages
     for package in packages2:
         if package not in packages1:
             version2, license2 = packages2[package]
+            if len(version2) == 0:
+                version2 = "UNKNOWN"
             sbom_out.send_output(f"[ADDED  ] {package}: (Version {version2})")
             new_packages += 1
     sbom_out.send_output("\nSummary\n-------")
     sbom_out.send_output(f"Version changes:  {version_changes}")
     if not args["exclude_license"]:
         sbom_out.send_output(f"License changes:  {license_changes}")
     sbom_out.send_output(f"Removed packages: {removed_packages}")
```

## sbomdiff/cyclonedx_parser.py

```diff
@@ -24,15 +24,15 @@
         data = json.load(open(sbom_file))
         packages = {}
         # Check that valid CycloneDX JSON file is being processed
         if "components" in data:
             for d in data["components"]:
                 if d["type"] in ["library", "application", "operating-system"]:
                     package = d["name"]
-                    version = d["version"]
+                    version = d["version"] if "version" in d else "UNKNOWN"
                     license = "NOT FOUND"
                     license_data = None
                     # Multiple ways of defining license data
                     if "licenses" in d and len(d["licenses"]) > 0:
                         license_data = d["licenses"][0]
                     elif "evidence" in d and len(d["evidence"]["licenses"]) > 0:
                         license_data = d["evidence"]["licenses"][0]
@@ -75,16 +75,17 @@
                         if component_name is None:
                             raise KeyError(f"Could not find package in {component}")
                         package = component_name.text
                         if package is None:
                             raise KeyError(f"Could not find package in {component}")
                         component_version = component.find(schema + "version")
                         if component_version is None:
-                            raise KeyError(f"Could not find version in {component}")
-                        version = component_version.text
+                            version = "UNKNOWN"
+                        else:
+                            version = component_version.text
                         license = "NOT FOUND"
                         component_license = component.find(schema + "licenses")
                         if component_license is not None:
                             license_data = component_license.find(schema + "expression")
                             if license_data is not None:
                                 license = license_data.text
                         if version is not None:
```

## sbomdiff/spdx_parser.py

```diff
@@ -12,15 +12,15 @@
     def __init__(self):
         pass
 
     def parse(self, sbom_file):
         """parses SPDX BOM file extracting package name, version and license"""
         if sbom_file.endswith(".spdx"):
             return self.parse_spdx_tag(sbom_file)
-        elif sbom_file.endswith(".spdx.json"):
+        elif sbom_file.endswith((".spdx.json", ".json")):
             return self.parse_spdx_json(sbom_file)
         elif sbom_file.endswith(".spdx.rdf"):
             return self.parse_spdx_rdf(sbom_file)
         elif sbom_file.endswith(".spdx.xml"):
             return self.parse_spdx_xml(sbom_file)
         elif sbom_file.endswith((".spdx.yaml", "spdx.yml")):
             return self.parse_spdx_yaml(sbom_file)
@@ -37,15 +37,15 @@
         for line in lines:
             line_elements = line.split(":")
             if line_elements[0] == "PackageName":
                 package = line_elements[1].strip().rstrip("\n")
                 version = None
                 license = None
             if line_elements[0] == "PackageVersion":
-                version = line_elements[1].strip().rstrip("\n")
+                version = line[16:].strip().rstrip("\n")
                 version = version.split("-")[0]
                 version = version.split("+")[0]
             if line_elements[0] == "PackageLicenseConcluded":
                 license = line_elements[1].strip().rstrip("\n")
             if package not in packages and version is not None and license is not None:
                 packages[package] = [version, license]
 
@@ -56,16 +56,16 @@
         data = json.load(open(sbom_file))
         packages = {}
         # Check that valid SPDX JSON file is being processed
         if "packages" in data:
             for d in data["packages"]:
                 package = d["name"]
                 try:
-                    version = d["versionInfo"]
-                    license = d["licenseConcluded"]
+                    version = d.get("versionInfo", "UNKNOWN")
+                    license = d.get("licenseConcluded", "NOT FOUND")
                     if package not in packages:
                         packages[package] = [version, license]
                 except KeyError:
                     pass
 
         return packages
 
@@ -82,27 +82,27 @@
                     stripped_line = line.strip().rstrip("\n")
                     package_match = re.search(
                         "<spdx:name>(.+?)</spdx:name>", stripped_line
                     )
                     if not package_match:
                         raise KeyError(f"Could not find package in {stripped_line}")
                     package = package_match.group(1)
-                    version = None
+                    version = "UNKNOWN"
                 elif line.strip().startswith("<spdx:versionInfo>"):
                     stripped_line = line.strip().rstrip("\n")
                     version_match = re.search(
                         "<spdx:versionInfo>(.+?)</spdx:versionInfo>", stripped_line
                     )
                     if not version_match:
                         raise KeyError(f"Could not find version in {stripped_line}")
                     version = version_match.group(1)
                     # To handle case where license appears before version
                     if package not in packages and license is not None:
                         packages[package] = [version, license]
-                        version = None
+                        version = "UNKNOWN"
                 elif line.strip().startswith("<spdx:licenseConcluded"):
                     stripped_line = line.strip().rstrip("\n")
                     # Assume license tag is on a single line
                     license_match = re.search(
                         "<spdx:licenseConcluded rdf:resource=(.+?)/>", stripped_line
                     )
                     if license_match is None:
@@ -134,16 +134,16 @@
 
         packages = {}
         # Check that valid SPDX YAML file is being processed
         if "packages" in data:
             for d in data["packages"]:
                 package = d["name"]
                 try:
-                    version = d["versionInfo"]
-                    license = d["licenseConcluded"]
+                    version = d.get("versionInfo", "UNKNOWN")
+                    license = d.get("licenseConcluded", "NOT FOUND")
                     if package not in packages:
                         packages[package] = [version, license]
                 except KeyError:
                     pass
 
         return packages
 
@@ -163,18 +163,19 @@
                 if package_match is None:
                     raise KeyError(f"Could not find package in {component}")
                 package = package_match.text
                 if package is None:
                     raise KeyError(f"Could not find package in {component}")
                 version_match = component.find(schema + "versionInfo")
                 if version_match is None:
-                    raise KeyError(f"Could not find version in {component}")
-                version = version_match.text
-                if version is None:
-                    raise KeyError(f"Could not find version in {component}")
+                    version = "UNKNOWN"
+                else:
+                    version = version_match.text
+                    if version is None:
+                        version = "UNKNOWN"
                 component_license = component.find(schema + "licenseConcluded")
                 if component_license is None:
                     license = "NOT FOUND"
                 else:
                     license = component_license.text
 
                 if version is not None:
```

## sbomdiff/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2022 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.4.1"
+VERSION: str = "0.4.2"
```

## Comparing `sbomdiff-0.4.1.dist-info/LICENSE` & `sbomdiff-0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbomdiff-0.4.1.dist-info/METADATA` & `sbomdiff-0.4.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbomdiff
-Version: 0.4.1
+Version: 0.4.2
 Summary: Software Bill of Material (SBOM) difference tool
 Home-page: https://github.com/anthonyharrison/sbomdiff
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -31,15 +31,15 @@
 SBOMDiff is a tool to compare two Software Bill of Materials (SBOM) files and
 reports the differences. It supports SBOMs created in both
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org) formats.
 
 The following differences are detected:
 
 - Package version changes
-- Package licence changes
+- Package license changes
 - Package removed
 - Package added
 
 ## Installation
 
 To install use the following command:
 
@@ -117,15 +117,15 @@
 3. SBOMs which do not match the format of the SBOM to be processed when specified using the `--sbom` option is likely to result in incorrect differences being reported.
 
 4. In SPDX format, the tool assumes that the name of a package is followed by the version and license of the package.
 
 5. If there are multiple instances of a package included in the SBOM, only the first instance will be processed.
 
 6. In CycloneDX format, if the _licenses_ section is not present for a component but the _evidence_ section is, the
-licence contained within the _evidence_ section shall be used.
+license contained within the _evidence_ section shall be used.
 
 7. If a license cannot be detected, the tool uses 'NOT FOUND' as the license to be used in the difference comparison.
 
 8. A non-zero return value indicates that differences were detected.
 
 ## Sample Output
 
@@ -142,15 +142,15 @@
 License changes:  2
 Removed packages: 1
 New packages:     0
 ```
 
 ## License
 
-Licensed under the Apache 2.0 Licence.
+Licensed under the Apache 2.0 License.
 
 ## Limitations
 
 This tool is meant to support software development and security audit functions. However the usefulness of the tool is dependent on the SBOM data
 which is provided to the tool. Unfortunately, the tool is unable to determine the validity or completeness of such a SBOM file; users of the tool
 are therefore reminded that they should assert the quality of any data which is provided to the tool.
```

## Comparing `sbomdiff-0.4.1.dist-info/RECORD` & `sbomdiff-0.4.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 sbomdiff/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sbomdiff/cli.py,sha256=Fr2F3BFtV-ZbiNY3e9PFjYz0C5dVgXs-5H-vu5r8Phw,5680
-sbomdiff/cyclonedx_parser.py,sha256=cH9xFnhHkkYWjmLmIDVrGu9w-O0rejvNYyapixmHrQM,4440
+sbomdiff/cli.py,sha256=-WhHmTKi9zj2HihBxc-poiMA3WsYVaKhFpZM91ljqO8,6174
+sbomdiff/cyclonedx_parser.py,sha256=lBp9SvYnVNxqlznYajTQWVIcTB-rn6bCTs5Ji9bFm0g,4470
 sbomdiff/output.py,sha256=G9tbsqlbCapnTyPgo6ROnSXVoVM2c4Hp1QfhvvvcQcQ,1298
-sbomdiff/spdx_parser.py,sha256=0EYdc__EQsNSEYJ-8eyr_62rySfXKyiip3nQk48m5eY,7803
-sbomdiff/version.py,sha256=QiH0fH4PX8IS-kwfDNx38XfHPK6yDUYKgeh4V0A53xg,100
-sbomdiff-0.4.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbomdiff-0.4.1.dist-info/METADATA,sha256=bxfx_hBsjw9NlzhPDTXiPzVFTo2Axrg4G-jy_K-vjhk,6336
-sbomdiff-0.4.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-sbomdiff-0.4.1.dist-info/entry_points.txt,sha256=fcONsvnGhylyVE47AbBD9yrXj47ScGZbVyJ7jGRcx9o,47
-sbomdiff-0.4.1.dist-info/top_level.txt,sha256=vt1EhODe3hHuS5SesbQue8uX-pOojrBfdtCwYdbEUgg,9
-sbomdiff-0.4.1.dist-info/RECORD,,
+sbomdiff/spdx_parser.py,sha256=Wtpjg8PhL_6BS7l5GQvNlMMfMo0_Z59vMl13FBP0F5s,7841
+sbomdiff/version.py,sha256=of7zNevWtgkB2MkHViOqddYl3CG4lSvYLWFUoceBUlo,100
+sbomdiff-0.4.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbomdiff-0.4.2.dist-info/METADATA,sha256=lh1_3yLl3bXRtLUb_j2seKWW3Jv9XSzNkKF-JNdjCRM,6336
+sbomdiff-0.4.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+sbomdiff-0.4.2.dist-info/entry_points.txt,sha256=fcONsvnGhylyVE47AbBD9yrXj47ScGZbVyJ7jGRcx9o,47
+sbomdiff-0.4.2.dist-info/top_level.txt,sha256=vt1EhODe3hHuS5SesbQue8uX-pOojrBfdtCwYdbEUgg,9
+sbomdiff-0.4.2.dist-info/RECORD,,
```

