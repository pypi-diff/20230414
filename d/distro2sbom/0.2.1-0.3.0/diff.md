# Comparing `tmp/distro2sbom-0.2.1-py2.py3-none-any.whl.zip` & `tmp/distro2sbom-0.3.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 18171 bytes, number of entries: 14
+Zip file size: 20056 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:04 distro2sbom/__init__.py
--rw-r--r--  2.0 unx     7108 b- defN 23-Mar-02 20:14 distro2sbom/cli.py
--rw-r--r--  2.0 unx      100 b- defN 23-Apr-03 17:15 distro2sbom/version.py
+-rw-r--r--  2.0 unx     7510 b- defN 23-Apr-10 17:00 distro2sbom/cli.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Apr-10 18:25 distro2sbom/version.py
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:04 distro2sbom/distrobuilder/__init__.py
--rw-r--r--  2.0 unx     2314 b- defN 23-Mar-23 23:04 distro2sbom/distrobuilder/distrobuilder.py
--rw-r--r--  2.0 unx     7272 b- defN 23-Mar-02 20:15 distro2sbom/distrobuilder/dpkgbuilder.py
--rw-r--r--  2.0 unx     9744 b- defN 23-Apr-03 17:14 distro2sbom/distrobuilder/rpmbuilder.py
+-rw-r--r--  2.0 unx     2582 b- defN 23-Apr-11 16:33 distro2sbom/distrobuilder/distrobuilder.py
+-rw-r--r--  2.0 unx    12435 b- defN 23-Apr-13 13:17 distro2sbom/distrobuilder/dpkgbuilder.py
+-rw-r--r--  2.0 unx    12251 b- defN 23-Apr-13 13:15 distro2sbom/distrobuilder/rpmbuilder.py
 -rw-r--r--  2.0 unx     4421 b- defN 23-Mar-02 20:15 distro2sbom/distrobuilder/windowsbuilder.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-03 17:16 distro2sbom-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     8781 b- defN 23-Apr-03 17:16 distro2sbom-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-03 17:16 distro2sbom-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Apr-03 17:16 distro2sbom-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-03 17:16 distro2sbom-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1222 b- defN 23-Apr-03 17:16 distro2sbom-0.2.1.dist-info/RECORD
-14 files, 52646 bytes uncompressed, 16111 bytes compressed:  69.4%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:13 distro2sbom-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10305 b- defN 23-Apr-14 15:13 distro2sbom-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:13 distro2sbom-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Apr-14 15:13 distro2sbom-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-14 15:13 distro2sbom-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1225 b- defN 23-Apr-14 15:13 distro2sbom-0.3.0.dist-info/RECORD
+14 files, 62513 bytes uncompressed, 17996 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: distro2sbom/distrobuilder/rpmbuilder.py
 Comment: 
 
 Filename: distro2sbom/distrobuilder/windowsbuilder.py
 Comment: 
 
-Filename: distro2sbom-0.2.1.dist-info/LICENSE
+Filename: distro2sbom-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: distro2sbom-0.2.1.dist-info/METADATA
+Filename: distro2sbom-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: distro2sbom-0.2.1.dist-info/WHEEL
+Filename: distro2sbom-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: distro2sbom-0.2.1.dist-info/entry_points.txt
+Filename: distro2sbom-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: distro2sbom-0.2.1.dist-info/top_level.txt
+Filename: distro2sbom-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: distro2sbom-0.2.1.dist-info/RECORD
+Filename: distro2sbom-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## distro2sbom/cli.py

```diff
@@ -84,14 +84,21 @@
     )
     input_group.add_argument(
         "-p",
         "--package",
         action="store",
         help="identity of package within distribution",
     )
+    input_group.add_argument(
+        "-s",
+        "--system",
+        action="store_true",
+        default=False,
+        help="generate SBOM for installed system",
+    )
 
     output_group = parser.add_argument_group("Output")
     output_group.add_argument(
         "-d",
         "--debug",
         action="store_true",
         default=False,
@@ -128,14 +135,15 @@
         "output_file": "",
         "sbom": "spdx",
         "debug": False,
         "format": "tag",
         "name": "",
         "release": "",
         "package": "",
+        "system": False,
     }
 
     raw_args = parser.parse_args(argv[1:])
     args = {key: value for key, value in vars(raw_args).items() if value}
     args = ChainMap(args, defaults)
 
     # Validate CLI parameters
@@ -145,15 +153,15 @@
         return -1
     elif args["name"] == "":
         print("[ERROR] distro name must be specified.")
         return -1
     elif args["release"] == "":
         print("[ERROR] distro release must be specified.")
         return -1
-    elif args["input_file"] == "" and args["package"] == "":
+    elif args["input_file"] == "" and args["package"] == "" and not args["system"]:
         print("[ERROR] distro file or package name must be specified.")
         return -1
 
     # Ensure format is aligned with type of SBOM
     bom_format = args["format"]
     if args["sbom"] != "spdx" and bom_format in ["tag", "yaml"]:
         # Only json format valid for CycloneDX
@@ -161,14 +169,15 @@
 
     if args["debug"]:
         print("Distro type:", args["distro"])
         print("Input file:", args["input_file"])
         print("Distro name:", args["name"])
         print("Distro release:", args["release"])
         print("Package:", args["package"])
+        print("System SBOM:", args["system"])
         print("SBOM type:", args["sbom"])
         print("Format:", bom_format)
         print("Output file:", args["output_file"])
 
     if args["distro"] == "auto":
         # determine distro type based on availability of key application
         distro_type = None
@@ -201,14 +210,18 @@
         # Check path exists and is a valid file
         if filePath.exists() and filePath.is_file():
             # Assume that processing can proceed
             sbom_build.parse_data(args["input_file"])
         else:
             print(f"[ERROR] Unable to locate file {args['input_file']}")
             return -1
+    elif args["system"]:
+        if args["debug"]:
+            print("This may take some time...")
+        sbom_build.process_system()
     else:
         sbom_build.process_distro_package(args["package"])
 
     # Only generate if we have some data to process
 
     if len(sbom_build.get_packages()) > 0:
         # Generate SBOM file
```

## distro2sbom/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.2.1"
+VERSION: str = "0.3.0"
```

## distro2sbom/distrobuilder/distrobuilder.py

```diff
@@ -14,14 +14,17 @@
 
     def get_data(self):
         pass
 
     def parse_data(self):
         pass
 
+    def process_system(self):
+        print("[ERROR] Feature not available")
+
     def run_program(self, command_line):
         # Remove any null bytes
         command_line = command_line.replace("\x00", "")
         # Split command line into individual elements
         params = command_line.split()
         res = subprocess.run(params, capture_output=True, text=True)
         return res.stdout.splitlines()
@@ -30,16 +33,20 @@
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
```

## distro2sbom/distrobuilder/dpkgbuilder.py

```diff
@@ -1,23 +1,26 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
 import re
+from pathlib import Path
 
 from lib4sbom.data.package import SBOMPackage
 from lib4sbom.data.relationship import SBOMRelationship
+from lib4sbom.license import LicenseScanner
 
 from distro2sbom.distrobuilder.distrobuilder import DistroBuilder
 
 
 class DpkgBuilder(DistroBuilder):
     def __init__(self, name, release, debug=False):
         super().__init__(debug)
         self.sbom_package = SBOMPackage()
         self.sbom_relationship = SBOMRelationship()
+        self.license = LicenseScanner()
         self.distro_packages = []
         self.name = name.replace(" ", "-")
         self.release = release
         self.parent = f"Distro-{self.name}"
 
     def parse_data(self, filename):
         # Process file containing installed applications
@@ -29,14 +32,15 @@
             self.sbom_package.initialise()
             self.sbom_package.set_name(distro_root)
             self.sbom_package.set_version(self.release)
             self.sbom_package.set_type("operating-system")
             self.sbom_package.set_filesanalysis(False)
             license = "NOASSERTION"
             self.sbom_package.set_licensedeclared(license)
+            self.sbom_package.set_licenseconcluded(license)
             self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
             # Store package data
             self.sbom_packages[
                 (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
             ] = self.sbom_package.get_package()
             self.sbom_relationship.initialise()
             self.sbom_relationship.set_relationship(
@@ -54,14 +58,15 @@
                     version = line_element[1]
                     self.sbom_package.set_name(package)
                     self.sbom_package.set_version(version)
                     self.sbom_package.set_type("application")
                     self.sbom_package.set_filesanalysis(False)
                     license = "NOASSERTION"
                     self.sbom_package.set_licensedeclared(license)
+                    self.sbom_package.set_licenseconcluded(license)
                     self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
                     description = " ".join(n for n in line_element[3:])
                     self.sbom_package.set_summary(description)
                     # Store package data
                     self.sbom_packages[
                         (
                             self.sbom_package.get_name(),
@@ -77,14 +82,46 @@
                     )
 
     def get(self, attribute):
         if attribute in self.metadata:
             return self.metadata[attribute].lstrip()
         return ""
 
+    def get_metadata_from_file(self, package):
+        # Location of Debian copyright files
+        base_file = f"/usr/share/doc/{package}/copyright"
+        copyright_text = ""
+        license_text = "NOASSERTION"
+        filename = Path(base_file)
+        # Check path exists and is a valid file
+        if filename.exists() and filename.is_file():
+            with open(filename, "r") as f:
+                lines = f.readlines()
+                copyright_found = False
+                license_found = False
+                for line in lines:
+                    # Search for first Copyright and License statements
+                    if copyright_found:
+                        copyright_info = line.strip().rstrip("\n")
+                        if len(copyright_info) > 0:
+                            copyright_text = "Copyright: " + copyright_info
+                            copyright_found = False
+                    elif line.startswith("Copyright:") and len(copyright_text) == 0:
+                        copyright_text = line.strip().rstrip("\n")
+                        if len(copyright_text) <= len("Copyright:"):
+                            # Assume copyright is on a following line
+                            copyright_found = True
+                    elif line.startswith("License:") and not license_found:
+                        license_info = line.split("License:", 1)[1].strip().rstrip("\n")
+                        if len(license_info) > 0:
+                            license_text = license_info
+                            license_found = True
+
+        return license_text, copyright_text
+
     def process_package(self, package_name, parent="-"):
         if self.debug:
             print(f"Process package {package_name}. Parent {parent}")
         # Check if we have already processed this package
         if package_name in self.distro_packages:
             self.sbom_relationship.initialise()
             self.sbom_relationship.set_relationship(
@@ -105,31 +142,61 @@
                         line.split(f"{entry[0]}:", 1)[1].strip().rstrip("\n")
                     )
             self.sbom_package.initialise()
             package = self.get("Package").lower().replace("_", "-")
             version = self.get("Version")
             self.sbom_package.set_name(package)
             self.sbom_package.set_version(version)
+            if parent == "-":
+                self.sbom_package.set_type("application")
             self.sbom_package.set_filesanalysis(False)
-            license = "NOASSERTION"
+            license_text, copyright = self.get_metadata_from_file(package_name)
+            license = self.license.find_license(license_text)
             self.sbom_package.set_licensedeclared(license)
             self.sbom_package.set_licenseconcluded(license)
+            if license != "NOASSERTION":
+                license_comment = (
+                    "This information was automatically extracted from the package."
+                )
+                if license_text != "NOASSERTION" and license != license_text:
+                    self.sbom_package.set_licensedeclared("NOASSERTION")
+                    license_comment = f"{license_comment} {self.sbom_package.get_name()} declares {license_text} which is not currently a valid SPDX License identifier or expression."
+                self.sbom_package.set_licensecomments(license_comment)
+            elif license_text != "NOASSERTION":
+                license_comment = f"{self.sbom_package.get_name()} declares {license_text} which is not currently a valid SPDX License identifier or expression."
+                self.sbom_package.set_licensecomments(license_comment)
             supplier = self.get("Maintainer")
             if len(supplier.split()) > 3:
                 self.sbom_package.set_supplier(
                     "Organization", self.format_supplier(supplier)
                 )
             elif len(supplier) > 1:
                 self.sbom_package.set_supplier("Person", self.format_supplier(supplier))
             else:
                 self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
             if self.get("Description") != "":
                 self.sbom_package.set_summary(self.get("Description"))
             if self.get("Homepage") != "":
                 self.sbom_package.set_homepage(self.get("Homepage"))
+            # Add copyright information
+            if len(copyright) > 0:
+                self.sbom_package.set_copyrighttext(copyright)
+            # External references
+            self.sbom_package.set_externalreference(
+                "PACKAGE-MANAGER", "purl", f"pkg:deb/{package}@{version}"
+            )
+            if len(supplier) > 1:
+                component_supplier = self.format_supplier(
+                    supplier, include_email=False
+                )
+                self.sbom_package.set_externalreference(
+                    "SECURITY",
+                    "cpe23Type",
+                    f"cpe:2.3:a:{component_supplier.replace(' ', '_').lower()}:{package}:{version}:*:*:*:*:*:*:*",
+                )
             # Store package data
             self.sbom_packages[
                 (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
             ] = self.sbom_package.get_package()
             # Add relationship
             self.sbom_relationship.initialise()
             if parent != "-":
@@ -155,7 +222,39 @@
                 if len(dependency) > 0 and self.process_package(dependency, parent):
                     self.analyze(dependency.strip(), self.get("Depends"))
 
     def process_distro_package(self, module_name):
         self.parent = f"{self.name}-{self.release}-Package-{module_name}"
         if self.process_package(module_name):
             self.analyze(self.get("Package"), self.get("Depends"))
+
+    def process_system(self):
+        distro_root = self.name.lower().replace("_", "-")
+        self.sbom_package.initialise()
+        self.sbom_package.set_name(distro_root)
+        self.sbom_package.set_version(self.release)
+        self.sbom_package.set_type("operating-system")
+        self.sbom_package.set_filesanalysis(False)
+        license = "NOASSERTION"
+        self.sbom_package.set_licensedeclared(license)
+        self.sbom_package.set_licenseconcluded(license)
+        self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
+        # Store package data
+        self.sbom_packages[
+            (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
+        ] = self.sbom_package.get_package()
+        self.sbom_relationship.initialise()
+        self.sbom_relationship.set_relationship(self.parent, "DESCRIBES", distro_root)
+        self.sbom_relationships.append(self.sbom_relationship.get_relationship())
+        # Get installed packages
+        out = self.run_program(f"dpkg -l")
+        for line in out:
+            if line[:2] == "ii":
+                # For each installed package
+                line_element = re.sub(" +", " ", line[2:].strip().rstrip("\n")).split(
+                    " "
+                )
+                module_name = line_element[0]
+                if self.debug:
+                    print(f"Processing... {module_name}")
+                if self.process_package(module_name, distro_root):
+                    self.analyze(self.get("Package"), self.get("Depends"))
```

## distro2sbom/distrobuilder/rpmbuilder.py

```diff
@@ -35,14 +35,15 @@
             self.sbom_package.initialise()
             self.sbom_package.set_name(distro_root)
             self.sbom_package.set_version(self.release)
             self.sbom_package.set_type("operating-system")
             self.sbom_package.set_filesanalysis(False)
             license = "NOASSERTION"
             self.sbom_package.set_licensedeclared(license)
+            self.sbom_package.set_licenseconcluded(license)
             self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
             # Store package data
             self.sbom_packages[
                 (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
             ] = self.sbom_package.get_package()
             self.sbom_relationship.initialise()
             self.sbom_relationship.set_relationship(
@@ -63,14 +64,15 @@
                     version = product_version.group(0)[1:]
                     self.sbom_package.set_name(package)
                     self.sbom_package.set_version(version)
                     self.sbom_package.set_type("application")
                     self.sbom_package.set_filesanalysis(False)
                     license = "NOASSERTION"
                     self.sbom_package.set_licensedeclared(license)
+                    self.sbom_package.set_licenseconcluded(license)
                     self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
                     # Store package data
                     self.sbom_packages[
                         (
                             self.sbom_package.get_name(),
                             self.sbom_package.get_value("version"),
                         )
@@ -141,53 +143,66 @@
                         and dependency != package_name
                     ):
                         requires.append(dependency)
             self.metadata["Depends"] = ",".join(n for n in requires)
             self.sbom_package.initialise()
             package = self.get("Name")
             version = self.get("Version")
+            if parent == "-":
+                self.sbom_package.set_type("application")
             self.sbom_package.set_name(package)
             self.sbom_package.set_version(version)
             self.sbom_package.set_filesanalysis(False)
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
             supplier = self.get("Packager")
             if len(supplier.split()) > 3:
                 self.sbom_package.set_supplier(
                     "Organization", self.format_supplier(supplier)
                 )
             elif len(supplier) > 1:
                 self.sbom_package.set_supplier("Person", self.format_supplier(supplier))
             else:
                 self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
             if self.get("Summary") != "":
                 self.sbom_package.set_summary(self.get("Summary"))
             if self.get("URL") != "":
                 self.sbom_package.set_homepage(self.get("URL"))
+            # External references
+            self.sbom_package.set_externalreference(
+                "PACKAGE-MANAGER", "purl", f"pkg:rpm/{package}@{version}"
+            )
+            if len(supplier) > 1:
+                component_supplier = self.format_supplier(
+                    supplier, include_email=False
+                )
+                self.sbom_package.set_externalreference(
+                    "SECURITY",
+                    "cpe23Type",
+                    f"cpe:2.3:a:{component_supplier.replace(' ', '_').lower()}:{package}:{version}:*:*:*:*:*:*:*",
+                )
             # Store package data
             self.sbom_packages[
                 (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
             ] = self.sbom_package.get_package()
             # Add relationship
             self.sbom_relationship.initialise()
             if parent != "-":
-                self.sbom_relationship.set_relationship(
-                    parent, "DEPENDS_ON", package
-                )
+                self.sbom_relationship.set_relationship(parent, "DEPENDS_ON", package)
             else:
                 self.sbom_relationship.set_relationship(
                     self.parent, "DESCRIBES", package
                 )
             self.sbom_relationships.append(self.sbom_relationship.get_relationship())
         elif self.debug:
             print(f"Package {package_name} not found")
@@ -203,7 +218,42 @@
                 if len(dependency) > 0 and self.process_package(dependency, parent):
                     self.analyze(dependency.strip(), self.get("Depends"))
 
     def process_distro_package(self, module_name):
         self.parent = f"{self.name}-{self.release}-Package-{module_name}"
         if self.process_package(module_name):
             self.analyze(self.get("Name"), self.get("Depends"))
+
+    def process_system(self):
+        distro_root = self.name.lower().replace("_", "-")
+        self.sbom_package.initialise()
+        self.sbom_package.set_name(distro_root)
+        self.sbom_package.set_version(self.release)
+        self.sbom_package.set_type("operating-system")
+        self.sbom_package.set_filesanalysis(False)
+        license = "NOASSERTION"
+        self.sbom_package.set_licensedeclared(license)
+        self.sbom_package.set_licenseconcluded(license)
+        self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
+        # Store package data
+        self.sbom_packages[
+            (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
+        ] = self.sbom_package.get_package()
+        self.sbom_relationship.initialise()
+        self.sbom_relationship.set_relationship(self.parent, "DESCRIBES", distro_root)
+        self.sbom_relationships.append(self.sbom_relationship.get_relationship())
+        # Get installed packages
+        out = self.run_program(f"rpm -qa")
+        for line in out:
+            # Parse line PRODUCT-VERSION[-Other]?. If pattern not followed ignore...
+            item = os.path.splitext(os.path.basename(line.strip().rstrip("\n")))[
+                0
+            ].lower()
+            # Version assumed to start with digit.
+            product_version = re.search(r"-\d[.\d]*[a-z0-9]*", item)
+            if product_version is None:
+                continue
+            module_name = item[: product_version.start()].lower().replace("_", "-")
+            if self.debug:
+                print(f"Processing... {module_name}")
+            if self.process_package(module_name, distro_root):
+                self.analyze(self.get("Name"), self.get("Depends"))
```

## Comparing `distro2sbom-0.2.1.dist-info/LICENSE` & `distro2sbom-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `distro2sbom-0.2.1.dist-info/METADATA` & `distro2sbom-0.3.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distro2sbom
-Version: 0.2.1
+Version: 0.3.0
 Summary: SBOM generator for system distribution
 Home-page: https://github.com/anthonyharrison/distro2sbom
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
 
 # DISTRO2SBOM
 
 The DISTRO2SBOM generates a
 SBOM (Software Bill of Materials) for either an installed application or a complete system installation in a number of formats including
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org).
 An SBOM for an installed package will identify all of its dependent components.
@@ -50,16 +50,18 @@
 if you are using different versions of python. `virtualenv` is a tool for setting up virtual python environments which
 allows you to have all the dependencies for the tool set up in a single environment, or have different environments set
 up for testing using different versions of Python.
 
 ## Usage
 
 ```
-usage: distro2sbom [-h] [--distro {rpm,deb,windows,auto}] [-i INPUT_FILE] [-n NAME] [-r RELEASE] [-p PACKAGE] [-d] [--sbom {spdx,cyclonedx}] [--format {tag,json,yaml}] [-o OUTPUT_FILE]
-                   [-V]
+usage: distro2sbom [-h] [--distro {rpm,deb,windows,auto}] [-i INPUT_FILE] [-n NAME] [-r RELEASE] [-p PACKAGE] [-s] [-d] [--sbom {spdx,cyclonedx}] [--format {tag,json,yaml}]
+                   [-o OUTPUT_FILE] [-V]
+
+Distro2Sbom generates a Software Bill of Materials for the specified package or distribution.
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
 
 Input:
   --distro {rpm,deb,windows,auto}
@@ -67,14 +69,17 @@
   -i INPUT_FILE, --input-file INPUT_FILE
                         name of distribution file
   -n NAME, --name NAME  name of distribution
   -r RELEASE, --release RELEASE
                         release identity of distribution
   -p PACKAGE, --package PACKAGE
                         identity of package within distribution
+  -s, --system          generate SBOM for installed system
+
+Output:
 
 Output:
   -d, --debug           add debug information
   --sbom {spdx,cyclonedx}
                         specify type of sbom to generate (default: spdx)
   --format {tag,json,yaml}
                         specify format of software bill of materials (sbom) (default: tag)
@@ -141,15 +146,18 @@
     ```
 
 If the specified filename is not found, the tool will terminate.
 
 The `--package` option is used to identify the name of a package or application installed on the system. If the specified package or application is not found, the tool terminates.
 This option is not supported if the `--distro` option is set to 'windows'.
 
-At least one of the `--input-file` or `--package` options must be specified. If both options are specified, the `--input-file` option is assumed.
+The `--system` option is used to generate an SBOM for all the applications installed on the system. Note that this option will take some time to complete as it is dependent on the number of installed applications.
+This option is not supported if the `--distro` option is set to 'windows'.
+
+At least one of the `--input-file`, `--package` or `--system` options must be specified. If multiple options are specified, the `--input-file` option followed by the `--system` option will be assumed.
 
 The `--sbom` option is used to specify the format of the generated SBOM (the default is SPDX). The `--format` option
 can be used to specify the formatting of the SBOM (the default is Tag Value format for a SPDX SBOM). JSON format is supported for both
 SPDX and CycloneDX SBOMs.
 
 The `--output-file` option is used to control the destination of the output generated by the tool. The
 default is to report to the console but can be stored in a file (specified using `--output-file` option).
@@ -172,24 +180,40 @@
 
 ```bash
 distro2sbom --distro deb --name <distro name> --release <distro release> --input-file <distrofile> --sbom cyclonedx --output-file <distrooutfile>
 ```
 
 This will generate an SBOM in CycloneDX JSON value for a distribution file in dpkg format (indicated by the 'deb' option)
 
+### SBOM for System
+
+To generate an SBOM for an installed system.
+
+```bash
+distro2sbom --distro rpm --name <distro name> --release <distro release> --system --format json --output-file <distrooutfile>
+```
+
+This will generate an SBOM in SPDX JSON value for a distribution file in dpkg format (indicated by the 'deb' option)
+
 ## Licence
 
 Licenced under the Apache 2.0 Licence.
 
 ## Limitations
 
 This tool is meant to support software development and security audit functions. However, the usefulness of the tool is dependent on the SBOM data
 which is provided to the tool. Unfortunately, the tool is unable to determine the validity or completeness of such a SBOM file; users of the tool
 are therefore reminded that they should assert the quality of any data which is provided to the tool.
 
-Dependencies between applications are only produced for the `--package` option.
+When processing and validating licenses, the application will use a set of synonyms to attempt to map some license identifiers to the correct [SPDX License Identifiers](https://spdx.org/licenses/). However, the
+user of the tool is reminded that they should assert the quality of any data which is provided by the tool particularly where the license identifier has been modified.
+
+Dependencies between applications are only produced for the `--package` and `--system` options.
 
 The `--package` option is not supported if the `--distro` option is set to 'windows'.
 
+Whilst [PURL](https://github.com/package-url/purl-spec) and [CPE](https://nvd.nist.gov/products/cpe) references are automatically generated for components, the accuracy
+of such references cannot be guaranteed as they are dependent on the validity of the data associated with the component.
+
 ## Feedback and Contributions
 
 Bugs and feature requests can be made via GitHub Issues.
```

## Comparing `distro2sbom-0.2.1.dist-info/RECORD` & `distro2sbom-0.3.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 distro2sbom/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
-distro2sbom/cli.py,sha256=d7AUdnAnjDmmif2rUwL6Fdiblk6VjzV7PDUCehUD4Xc,7108
-distro2sbom/version.py,sha256=Sf4YLFWUpG_pOy51nAMl86uP4c0l_zH7N9PSxWNRR6w,100
+distro2sbom/cli.py,sha256=S3prwgydyg56adp3FwA6xJDrGBn8pK2njbI-RlzjlnM,7510
+distro2sbom/version.py,sha256=_p-y2a7gEF6oU37vmbGAsqrCSIpyaZoCAugkrzEBDQI,100
 distro2sbom/distrobuilder/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
-distro2sbom/distrobuilder/distrobuilder.py,sha256=MWH7I6kepEWDOD7J_WFe01AL2bStg-edrkvfoYXMvJg,2314
-distro2sbom/distrobuilder/dpkgbuilder.py,sha256=c9-xNXIMpRqIJjlqZ3PNqEYOMLyYIvaSkiz7nP_zpHo,7272
-distro2sbom/distrobuilder/rpmbuilder.py,sha256=ihnPPjoHXIE5iepy8_4k_ZXn8Bz_RKFaLgmfnjxJJmk,9744
+distro2sbom/distrobuilder/distrobuilder.py,sha256=PELdB9OP0hoZhSUr0XN5pIn31nwm04glPqoGBRNhGJ4,2582
+distro2sbom/distrobuilder/dpkgbuilder.py,sha256=w5-bA8BEHHVBXORHvTNy9XPt3kXp_reK4zp0aQlRwDE,12435
+distro2sbom/distrobuilder/rpmbuilder.py,sha256=73pXNBgJ7HhBci-0o72affoSv6yZNT0IAvRbS8eGIGk,12251
 distro2sbom/distrobuilder/windowsbuilder.py,sha256=4_qlVL3hD_KW42iEhKoP_N1YF6YL5UJ7uq6uXYwwk_0,4421
-distro2sbom-0.2.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-distro2sbom-0.2.1.dist-info/METADATA,sha256=Ew6SAQVUUEg3e4jINvG99bgy5uav94eb3D1_ocKS7KI,8781
-distro2sbom-0.2.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-distro2sbom-0.2.1.dist-info/entry_points.txt,sha256=r5RioA3bp_Kbd1UJ5L1BTfSea9qEISrGmoSKSAHFBOU,53
-distro2sbom-0.2.1.dist-info/top_level.txt,sha256=wj3FBpfTya_uiJ4egUDQ4vv-BO5G5swycPOUc7qymJM,12
-distro2sbom-0.2.1.dist-info/RECORD,,
+distro2sbom-0.3.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+distro2sbom-0.3.0.dist-info/METADATA,sha256=6kkEOh6LywuQKpcLkOVAGy0nrQpItZ_YsrMUC_GOKqc,10305
+distro2sbom-0.3.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+distro2sbom-0.3.0.dist-info/entry_points.txt,sha256=r5RioA3bp_Kbd1UJ5L1BTfSea9qEISrGmoSKSAHFBOU,53
+distro2sbom-0.3.0.dist-info/top_level.txt,sha256=wj3FBpfTya_uiJ4egUDQ4vv-BO5G5swycPOUc7qymJM,12
+distro2sbom-0.3.0.dist-info/RECORD,,
```

