# Comparing `tmp/sbomaudit-0.1.1-py2.py3-none-any.whl.zip` & `tmp/sbomaudit-0.1.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 14252 bytes, number of entries: 10
+Zip file size: 14807 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:08 sbomaudit/__init__.py
--rw-r--r--  2.0 unx    17382 b- defN 23-Mar-23 23:08 sbomaudit/audit.py
+-rw-r--r--  2.0 unx    21953 b- defN 23-Apr-10 17:31 sbomaudit/audit.py
 -rw-r--r--  2.0 unx     4416 b- defN 23-Mar-02 17:59 sbomaudit/cli.py
--rw-r--r--  2.0 unx      100 b- defN 23-Mar-23 20:57 sbomaudit/version.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-27 14:17 sbomaudit-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    13752 b- defN 23-Mar-27 14:17 sbomaudit-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-27 14:17 sbomaudit-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-Mar-27 14:17 sbomaudit-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Mar-27 14:17 sbomaudit-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      797 b- defN 23-Mar-27 14:17 sbomaudit-0.1.1.dist-info/RECORD
-10 files, 48049 bytes uncompressed, 12898 bytes compressed:  73.2%
+-rw-r--r--  2.0 unx      100 b- defN 23-Apr-10 18:36 sbomaudit/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:13 sbomaudit-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14069 b- defN 23-Apr-14 15:13 sbomaudit-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:13 sbomaudit-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-Apr-14 15:13 sbomaudit-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-14 15:13 sbomaudit-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      797 b- defN 23-Apr-14 15:13 sbomaudit-0.1.2.dist-info/RECORD
+10 files, 52937 bytes uncompressed, 13453 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: sbomaudit/cli.py
 Comment: 
 
 Filename: sbomaudit/version.py
 Comment: 
 
-Filename: sbomaudit-0.1.1.dist-info/LICENSE
+Filename: sbomaudit-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: sbomaudit-0.1.1.dist-info/METADATA
+Filename: sbomaudit-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: sbomaudit-0.1.1.dist-info/WHEEL
+Filename: sbomaudit-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: sbomaudit-0.1.1.dist-info/entry_points.txt
+Filename: sbomaudit-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbomaudit-0.1.1.dist-info/top_level.txt
+Filename: sbomaudit-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sbomaudit-0.1.1.dist-info/RECORD
+Filename: sbomaudit-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbomaudit/audit.py

```diff
@@ -48,14 +48,32 @@
 
     def _check_value(self, text, values, data_item):
         self._show_result(text, data_item in values, data_item)
 
     def _check(self, text, value, failure_text="MISSING"):
         self._show_result(text, value, failure_text=failure_text)
 
+    def find_latest_version_maven(self, name):
+        """Returns the latest version of the package available at Maven Central."""
+
+        url: str = f"https://search.maven.org/solrsearch/select?q=a:{name}&wt=json"
+        maven_version = None
+        try:
+            package_json = requests.get(url).json()
+            maven_version = package_json["response"]["docs"][0]["latestVersion"]
+        except Exception as error:
+            print(
+                f"""
+            -------------------------- Can't check Maven Central for the latest version -------
+            Exception details: {error}
+            Please make sure you have a working internet connection or try again later.
+            """
+            )
+        return maven_version
+
     def find_latest_version(self, name):
         """Returns the latest version of the package available at PyPI."""
 
         url: str = f"https://pypi.org/pypi/{name}/json"
         pypi_version = None
         try:
             package_json = requests.get(url).json()
@@ -66,14 +84,40 @@
             -------------------------- Can't check PyPi for the latest version -------
             Exception details: {error}
             Please make sure you have a working internet connection or try again later.
             """
             )
         return pypi_version
 
+    def get_latest_version(self, name, backend="PyPI"):
+        url: str = f"https://release-monitoring.org/api/v2/projects/?name={name}"
+        latest_version = None
+        try:
+            package_json = requests.get(url).json()
+            if (
+                package_json["total_items"] == 1
+                and package_json["items"][0]["backend"].lower() == backend.lower()
+            ):
+                latest_version = package_json["items"][0]["stable_versions"][0]
+            else:
+                for item in package_json["items"]:
+                    if item["backend"].lower() == backend.lower():
+                        latest_version = item["stable_versions"][0]
+                        break
+
+        except Exception as error:
+            print(
+                f"""
+            -------------------------- Can't check for the latest version -------
+            Exception details: {error}
+            Please make sure you have a working internet connection or try again later.
+            """
+            )
+        return latest_version
+
     def process_file(self, filename, allow):
         # Only process if file exists
         if Path(filename).resolve().exists():
             if allow:
                 self._setup(filename, self.allow_list)
             else:
                 self._setup(filename, self.deny_list)
@@ -165,24 +209,28 @@
                     self._check(f"File name specified - {name}", name)
                     if name is not None:
                         self._check(
                             f"File type identified - {name} : {file_type}",
                             filetype is not None,
                         )
                         self._check(
-                            f"Licence specified - {name} : {license}",
+                            f"License specified - {name} : {license}",
                             not (license in [None, "NOASSERTION"]),
                             failure_text="",
                         )
                         if self.license_check:
                             self._check(
                                 f"SPDX Compatible License id included for {name}",
                                 spdx_license,
                                 failure_text=f"{license}",
                             )
+                            self._check(
+                                f"OSI Approved license for {name}",
+                                self.license_scanner.osi_approved(license),
+                            )
                         if allow_licenses is not None:
                             self._check(
                                 f"Allowed License check for {name}",
                                 license in allow_licenses,
                                 failure_text=f"{license} not allowed",
                             )
                         if deny_licenses is not None:
@@ -198,24 +246,28 @@
                         )
                     else:
                         self._check(
                             f"File type identified - {id} : {file_type}",
                             filetype is not None,
                         )
                         self._check(
-                            f"Licence specified - {id} : {license}",
+                            f"License specified - {id} : {license}",
                             not (license in [None, "NOASSERTION"]),
                             failure_text="",
                         )
                         if self.license_check:
                             self._check(
                                 f"SPDX Compatible License id included for {id}",
                                 spdx_license,
                                 failure_text=f"{license}",
                             )
+                            self._check(
+                                f"OSI Approved license for {id}",
+                                self.license_scanner.osi_approved(license),
+                            )
                         if allow_licenses is not None:
                             self._check(
                                 f"Allowed License check for {id}",
                                 license in allow_licenses,
                                 failure_text=f"{license} not allowed",
                             )
                         if deny_licenses is not None:
@@ -267,19 +319,36 @@
                         for external_ref in external_refs:
                             # Can be two specifications of PACKAGE MANAGER attribute!
                             if external_ref[0] in [
                                 "PACKAGE-MANAGER",
                                 "PACKAGE_MANAGER",
                             ]:
                                 purl_used = True
-                                purl = PackageURL.from_string(external_ref[2]).to_dict()
-                                if purl["type"] == "pypi" and not self.offline:
-                                    # Python package detected
-                                    latest_version = self.find_latest_version(name)
-                                purl_name = purl["name"]
+                                try:
+                                    purl = PackageURL.from_string(
+                                        external_ref[2]
+                                    ).to_dict()
+                                    if not self.offline:
+                                        if purl["type"] == "pypi":
+                                            # Python package detected
+                                            latest_version = self.find_latest_version(
+                                                name
+                                            )
+                                        elif purl["type"] == "maven":
+                                            # Maven package detected
+                                            latest_version = (
+                                                self.find_latest_version_maven(name)
+                                            )
+                                        else:
+                                            latest_version = self.get_latest_version(
+                                                name, backend=purl["type"]
+                                            )
+                                    purl_name = purl["name"]
+                                except ValueError:
+                                    purl_used = False
                             elif external_ref[1] in ["cpe22Type", "cpe23Type"]:
                                 cpe_used = True
 
                     # Now summarise
                     if name is not None:
                         if allow_packages is not None:
                             self._check(
@@ -304,14 +373,18 @@
                             "NOASSERTION",
                         ]:
                             self._check(
                                 f"SPDX Compatible License id included for package {name}",
                                 spdx_license,
                                 failure_text=f"{license}",
                             )
+                            self._check(
+                                f"OSI Approved license for {name}",
+                                self.license_scanner.osi_approved(license),
+                            )
                         if allow_licenses is not None:
                             self._check(
                                 f"Allowed License check for package {name}",
                                 license in allow_licenses,
                                 failure_text=f"{license} not allowed",
                             )
                         if deny_licenses is not None:
@@ -328,15 +401,19 @@
                                 failure_text=report,
                             )
                         if self.cpe_check:
                             self._check(
                                 f"CPE name included for package {name}", cpe_used
                             )
                         if self.purl_check:
-                            self._check(f"PURL included for package {name}", purl_used)
+                            self._check(
+                                f"PURL included for package {name}",
+                                purl_used,
+                                failure_text="MISSING or INVALID",
+                            )
                             if purl_used:
                                 # Check name is consistent with package name
                                 self._check(
                                     f"PURL name compatible with package {name}",
                                     purl_name == name,
                                 )
                     else:
@@ -361,14 +438,36 @@
         self._heading("Relationships Summary")
         fail_count = self.check_count["Fail"]
 
         self._check(
             "Dependency relationships provided for NTIA compliance", relationships_valid
         )
 
+        # Check all files/packages included in at least one relationship
+        if len(files) > 0:
+            for file in files:
+                name = file.get("name", None)
+                dep_check = False
+                if name is not None:
+                    for r in relationships:
+                        if name in [r.get("source"), r.get("target")]:
+                            dep_check = True
+                            break
+                self._check(f"Dependency relationship found for {name}", dep_check)
+        if len(packages) > 0:
+            for package in packages:
+                name = package.get("name", None)
+                dep_check = False
+                if name is not None:
+                    for r in relationships:
+                        if name in [r.get("source"), r.get("target")]:
+                            dep_check = True
+                            break
+                self._check(f"Dependency relationship found for {name}", dep_check)
+
         # Report if all checks passed
         if not self.verbose:
             if self.check_count["Fail"] == fail_count:
                 # No tests failed
                 self._show_text("Relationships Summary")
 
         self._heading("NTIA Summary")
```

## sbomaudit/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.1.1"
+VERSION: str = "0.1.2"
```

## Comparing `sbomaudit-0.1.1.dist-info/LICENSE` & `sbomaudit-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbomaudit-0.1.1.dist-info/METADATA` & `sbomaudit-0.1.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbomaudit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Audit SBOM contents
 Home-page: https://github.com/anthonyharrison/sbomaudit
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
 Requires-Dist: rich
 Requires-Dist: requests
 Requires-Dist: packageurl-python
 
 # SBOMAUIDT
 
 SBOMAUDIT reports on the quality of the contents of an SBOM (Software Bill of Materials) by performing a number of checks. SBOMs are supported in a number of formats including
@@ -142,19 +142,21 @@
 
 The following checks are performed for each file item:
 
 - Check that a file name is specified.
 
 - Check that the file type is specified.
 
-- Check that a licence is specified and that the licence identified is a valid [SPDX Licence identifier](https://spdx.org/licenses/). Note that NOASSERTION is not considered a valid licence.
+- Check that a license is specified and that the license identified is a valid [SPDX License identifier](https://spdx.org/licenses/). Note that NOASSERTION is not considered a valid license.
+
+- Check that the license is an [OSI Approved](https://opensource.org/licenses/) license.
 
 - Optionally check that the license is allowed as specified in the ALLOW list
 
-- Optionally check that the licence is not included in the licenses specified in the DENY list
+- Optionally check that the license is not included in the licenses specified in the DENY list
 
 - Check that a copyright statement is specified. Note that NOASSERTION is not considered a valid copyright statement.
 
 ### Packages
 
 The following checks are performed on each package item:
 
@@ -166,30 +168,36 @@
 
 - Check that a supplier is specified.
 
 - Check that a version is specified.
 
 - Check that the package version is the latest released version of the package. The latest version checks are only performed if the `--offline` option is not specified and is only performed for Python modules available on the [Python Package Index (PyPi)](https://pypi.org/).
 
-- Check that a licence is specified and that the licence identified is a valid [SPDX Licence identifier](https://spdx.org/licenses/). Note that NOASSERTION is not considered a valid licence.
+- Check that a license is specified and that the license identified is a valid [SPDX License identifier](https://spdx.org/licenses/). Note that NOASSERTION is not considered a valid license.
+
+- Check that the license is an [OSI Approved](https://opensource.org/licenses/) license.
 
 - Optionally check that the license is allowed as specified in the ALLOW list
 
-- Optionally check that the licence is not included in the licenses specified in the DENY list
+- Optionally check that the license is not included in the licenses specified in the DENY list
 
 - Check that a [PURL specification](https://github.com/package-url/purl-spec) is provided for the package.
 
 - Check that a [CPE specification](https://nvd.nist.gov/products/cpe) is provided for the package.
 
 ### Relationships
 
 The following checks are performed:
 
 - Check that relationships are defined.
 
+- Check that every file is included in at least one relationship.
+
+- Check that every package is included in at least one relationship.
+
 ### NTIA Conformance
 
 The following checks are performed:
 
 - Check that the contents of the SBOM meet the minimum requirements for an SBOM as defined by the [NTIA](https://www.ntia.doc.gov/files/ntia/publications/sbom_minimum_elements_report.pdf).
 
 ## Example
@@ -359,17 +367,17 @@
 ╭────────────────────╮
 │ SBOM Audit Summary │
 ╰────────────────────╯
 [x] Checks passed 42
 [x] Checks failed 12                                                   
 ```
 
-## Licence
+## License
 
-Licenced under the Apache 2.0 Licence.
+Licensed under the Apache 2.0 License.
 
 ## Limitations
 
 The tool has the following limitations:
 
 - The latest version checks are only performed on Python modules available on the [Python Package Index (PyPi)](https://pypi.org/).
```

