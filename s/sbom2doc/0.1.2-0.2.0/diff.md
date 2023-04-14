# Comparing `tmp/sbom2doc-0.1.2-py2.py3-none-any.whl.zip` & `tmp/sbom2doc-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 15085 bytes, number of entries: 15
+Zip file size: 16185 bytes, number of entries: 15
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:05 sbom2doc/__init__.py
--rw-r--r--  2.0 unx     2592 b- defN 23-Feb-01 11:20 sbom2doc/cli.py
--rw-r--r--  2.0 unx     4946 b- defN 23-Feb-10 11:14 sbom2doc/generator.py
--rw-r--r--  2.0 unx      100 b- defN 23-Mar-26 18:11 sbom2doc/version.py
--rw-r--r--  2.0 unx       75 b- defN 23-Mar-02 20:21 sbom2doc/docbuilder/__init__.py
--rw-r--r--  2.0 unx     1241 b- defN 23-Feb-01 11:20 sbom2doc/docbuilder/consolebuilder.py
--rw-r--r--  2.0 unx      429 b- defN 23-Feb-01 11:20 sbom2doc/docbuilder/docbuilder.py
--rw-r--r--  2.0 unx     1094 b- defN 23-Feb-01 11:20 sbom2doc/docbuilder/markdownbuilder.py
--rw-r--r--  2.0 unx     5462 b- defN 23-Feb-01 11:21 sbom2doc/docbuilder/pdfbuilder.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-27 14:13 sbom2doc-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    11501 b- defN 23-Mar-27 14:13 sbom2doc-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-27 14:13 sbom2doc-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Mar-27 14:13 sbom2doc-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Mar-27 14:13 sbom2doc-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1243 b- defN 23-Mar-27 14:13 sbom2doc-0.1.2.dist-info/RECORD
-15 files, 40282 bytes uncompressed, 13019 bytes compressed:  67.7%
+-rw-r--r--  2.0 unx     2915 b- defN 23-Apr-04 15:57 sbom2doc/cli.py
+-rw-r--r--  2.0 unx     7083 b- defN 23-Apr-10 17:29 sbom2doc/generator.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Apr-10 18:35 sbom2doc/version.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-04 15:59 sbom2doc/docbuilder/__init__.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Apr-09 20:09 sbom2doc/docbuilder/consolebuilder.py
+-rw-r--r--  2.0 unx      481 b- defN 23-Apr-03 21:56 sbom2doc/docbuilder/docbuilder.py
+-rw-r--r--  2.0 unx     1107 b- defN 23-Apr-03 21:45 sbom2doc/docbuilder/markdownbuilder.py
+-rw-r--r--  2.0 unx     5818 b- defN 23-Apr-13 19:16 sbom2doc/docbuilder/pdfbuilder.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 15:13 sbom2doc-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14054 b- defN 23-Apr-14 15:13 sbom2doc-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 15:13 sbom2doc-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Apr-14 15:13 sbom2doc-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-14 15:13 sbom2doc-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1243 b- defN 23-Apr-14 15:13 sbom2doc-0.2.0.dist-info/RECORD
+15 files, 45843 bytes uncompressed, 14119 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: sbom2doc/docbuilder/markdownbuilder.py
 Comment: 
 
 Filename: sbom2doc/docbuilder/pdfbuilder.py
 Comment: 
 
-Filename: sbom2doc-0.1.2.dist-info/LICENSE
+Filename: sbom2doc-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: sbom2doc-0.1.2.dist-info/METADATA
+Filename: sbom2doc-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: sbom2doc-0.1.2.dist-info/WHEEL
+Filename: sbom2doc-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: sbom2doc-0.1.2.dist-info/entry_points.txt
+Filename: sbom2doc-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbom2doc-0.1.2.dist-info/top_level.txt
+Filename: sbom2doc-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sbom2doc-0.1.2.dist-info/RECORD
+Filename: sbom2doc-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbom2doc/cli.py

```diff
@@ -39,14 +39,21 @@
     output_group.add_argument(
         "--debug",
         action="store_true",
         default=False,
         help="add debug information",
     )
 
+    output_group.add_argument(
+        "--include-license",
+        action="store_true",
+        default=False,
+        help="add license text",
+    )
+
     # Add format option
     output_group.add_argument(
         "-f",
         "--format",
         action="store",
         help="Output format (default: output to console)",
         choices=["console", "markdown", "pdf"],
@@ -64,14 +71,15 @@
     parser.add_argument("-V", "--version", action="version", version=VERSION)
 
     defaults = {
         "input_file": "",
         "output_file": "",
         "debug": False,
         "format": "console",
+        "include_license": False,
     }
 
     raw_args = parser.parse_args(argv[1:])
     args = {key: value for key, value in vars(raw_args).items() if value}
     args = ChainMap(args, defaults)
 
     # Validate CLI parameters
@@ -85,22 +93,27 @@
     if args["format"] != "console" and args["output_file"] == "":
         print("[ERROR] Output filename must be specified.")
         return -1
 
     if args["debug"]:
         print("Input file", args["input_file"])
         print("Output file", args["output_file"])
+        print("Include license text", args["include_license"])
 
     sbom_parser = SBOMParser()
     # Load SBOM - will autodetect SBOM type
     try:
         sbom_parser.parse_file(input_file)
 
         generator.generate_document(
-            args["format"], sbom_parser, input_file, args["output_file"]
+            args["format"],
+            sbom_parser,
+            input_file,
+            args["output_file"],
+            args["include_license"],
         )
 
     except FileNotFoundError:
         print(f"{input_file} not found")
 
     return 0
```

## sbom2doc/generator.py

```diff
@@ -1,18 +1,21 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
+import requests
 from lib4sbom.data.document import SBOMDocument
+from lib4sbom.license import LicenseScanner
+from packageurl import PackageURL
 
 from sbom2doc.docbuilder.consolebuilder import ConsoleBuilder
 from sbom2doc.docbuilder.markdownbuilder import MarkdownBuilder
 from sbom2doc.docbuilder.pdfbuilder import PDFBuilder
 
 
-def generate_document(format, sbom_parser, filename, outfile):
+def generate_document(format, sbom_parser, filename, outfile, include_license):
     # Get constituent components of the SBOM
     packages = sbom_parser.get_packages()
     files = sbom_parser.get_files()
     relationships = sbom_parser.get_relationships()
     document = SBOMDocument()
     document.copy_document(sbom_parser.get_document())
 
@@ -69,15 +72,15 @@
                 files_valid = False
         sbom_document.showtable(widths=[3, 2, 4, 5])
 
     if len(packages) > 0:
 
         sbom_document.heading(1, "Package Summary")
         sbom_document.createtable(
-            ["Name", "Version", "Supplier", "License"], [None, 8, 8, None]
+            ["Name", "Version", "Supplier", "License"], [12, 8, 8, 12]
         )
         for package in packages:
             # Minimum elements are ID, Name, Version, Supplier
             id = package.get("id", None)
             name = package.get("name", None)
             version = package.get("version", None)
             supplier = package.get("supplier", None)
@@ -90,16 +93,40 @@
                 or version is None
                 or supplier is None
                 or supplier == "NOASSERTION"
             ):
                 packages_valid = False
         sbom_document.showtable(widths=[5, 2, 2, 5])
 
+        # Too much information so second table required
+        sbom_document.paragraph("")
+        sbom_document.createtable(
+            ["Name", "Version", "Ecosystem", "Download", "Copyright"], [12, 8, 5, 8, 7]
+        )
+        for package in packages:
+            name = package.get("name", None)
+            version = package.get("version", None)
+            external_info = package.get("externalreference", None)
+            ecosystem = "-"
+            if external_info is not None:
+                for reference in external_info:
+                    if reference[1] == "purl":
+                        try:
+                            purl = PackageURL.from_string(reference[2]).to_dict()
+                            ecosystem = purl["type"]
+                        except ValueError:
+                            ecosystem = "INVALID"
+                        break
+            download = package.get("downloadlocation", "NOT KNOWN")
+            copyright = package.get("copyrighttext", "-")
+            sbom_document.addrow([name, version, ecosystem, download, copyright])
+        sbom_document.showtable(widths=[5, 2, 2, 2, 2])
+
     sbom_document.heading(1, "License Summary")
-    sbom_document.createtable(["License", "Count"])
+    sbom_document.createtable(["License", "Count"], [25, 6])
     #
     # Create an empty dictionary
     freq = {}
     for items in sorted(sbom_licenses):
         freq[items] = sbom_licenses.count(items)
     for key, value in freq.items():
         sbom_document.addrow([key, str(value)])
@@ -120,8 +147,27 @@
         files_valid
         and packages_valid
         and creator_identified
         and creation_time
         and relationships_valid
     )
     sbom_document.paragraph(f"NTIA conformant {valid_sbom}")
+
+    if include_license:
+        sbom_document.pagebreak()
+        sbom_document.heading(1, "License Text")
+        license_info = LicenseScanner()
+        for key, value in freq.items():
+            # Ignore undefined licenses or expressions
+            if key == "NOASSERTION" or license_info.license_expression(key):
+                continue
+            license_url = f"https://spdx.org/licenses/{key}.json"
+            try:
+                license_text = requests.get(license_url).json()
+                if license_text.get("licenseText") is not None:
+                    sbom_document.heading(2, key, number=False)
+                    sbom_document.paragraph(license_text["licenseText"])
+            except requests.exceptions.RequestException:
+                sbom_document.heading(2, key, number=False)
+                sbom_document.paragraph("Unable to find license text.")
+
     sbom_document.publish(outfile)
```

## sbom2doc/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2023 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.1.2"
+VERSION: str = "0.2.0"
```

## sbom2doc/docbuilder/__init__.py

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
 # Copyright (C) 2023 Anthony Harrison
-# SPDX-License-Identifier: Apache-2.0
+# SPDX-License-Identifier: Apache-2.0
```

## sbom2doc/docbuilder/consolebuilder.py

```diff
@@ -9,36 +9,38 @@
 from sbom2doc.docbuilder.docbuilder import DocBuilder
 
 
 class ConsoleBuilder(DocBuilder):
     def __init__(self):
         pass
 
-    def heading(self, level, title):
+    def heading(self, level, title, number=True):
         print(Panel(title, style="bold", expand=False))
 
     def paragraph(self, text):
         print(f"\n{text}")
 
     def createtable(self, header, validate=None):
         # Layout is [headings, ....]
         self.table = Table()
         for h in header:
             self.table.add_column(h)
 
     def addrow(self, data):
-        if len(data) > 4:
+        if len(data) > 5:
             print("Ooops - too much data!")
         else:
             # Add row to table
             if len(data) == 1:
                 self.table.add_row(data[0])
             elif len(data) == 2:
                 self.table.add_row(data[0], data[1])
             elif len(data) == 3:
                 self.table.add_row(data[0], data[1], data[2])
-            else:
+            elif len(data) == 4:
                 self.table.add_row(data[0], data[1], data[2], data[3])
+            else:
+                self.table.add_row(data[0], data[1], data[2], data[3], data[4])
 
     def showtable(self, widths=None):
         console = Console()
         console.print(self.table)
```

## sbom2doc/docbuilder/docbuilder.py

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 
 class DocBuilder:
     def __init__(self):
         pass
 
-    def heading(self, level, title):
+    def heading(self, level, title, number=True):
         pass
 
     def paragraph(self, text):
         pass
 
     def createtable(self, header, validate):
         pass
@@ -19,7 +19,10 @@
         pass
 
     def showtable(self, widths=None):
         pass
 
     def publish(self, filename):
         pass
+
+    def pagebreak(self):
+        pass
```

## sbom2doc/docbuilder/markdownbuilder.py

```diff
@@ -6,15 +6,15 @@
 from sbom2doc.docbuilder.docbuilder import DocBuilder
 
 
 class MarkdownBuilder(DocBuilder):
     def __init__(self):
         self.markdown_document = []
 
-    def heading(self, level, title):
+    def heading(self, level, title, number=True):
         heading_field = "#" * level
         self.markdown_document.append(f"\n{heading_field} {title}\n")
 
     def paragraph(self, text):
         self.markdown_document.append(f"{text}")
 
     def createtable(self, header, validate=None):
```

## sbom2doc/docbuilder/pdfbuilder.py

```diff
@@ -55,15 +55,15 @@
             ("FONT", (0, 0), (-1, -1), document_font, 12),
             ("FONT", (0, 0), (-1, 0), document_font_bold),
         ]
     )
 
     list = ListStyle(
         name="list",
-        fontSize=12,
+        fontSize=10,
         fontName=document_font,
         leading=12,
         textColor=black,
         textTransform=None,
         firstLineIndent=12,
         wordWrap=True,
         uriWasteReduce=None,
@@ -86,28 +86,37 @@
         # Set default configuration parameters
         rl_config.trustedHosts = ["localhost", "127.0.0.1"]
         rl_config.trustedSchemes = ["http", "https"]
 
     def _spacer(self):
         self.contents.append(self.spacer)
 
-    def heading(self, level, title):
+    def heading(self, level, title, number=True):
         self._spacer()
         if level == 1:
             self.headingnumber[level] += 1
+            self.headingnumber[level + 1] = 1
+        elif level == 2:
+            self.headingnumber[level] += 1
+        elif level > 2:
+            print("Ooops.... Level", level)
+        if number:
             self.contents.append(
                 Paragraph(str(self.headingnumber[level]) + ". " + title, self.h1)
             )
         else:
-            print("Ooops.... Level", level)
+            self.contents.append(Paragraph(title, self.h1))
         self._spacer()
 
     def paragraph(self, text):
-        self.contents.append(Paragraph(text, self.body))
-        self._spacer()
+        # Line breaks preserved if required
+        text_elements = text.splitlines()
+        for t in text_elements:
+            self.contents.append(Paragraph(t, self.body))
+            self._spacer()
 
     def _notes_paragraph(self, text):
         self.contents.append(Paragraph(text, self.list))
         self._spacer()
 
     def createtable(self, header, validate=None):
         # Layout is [headings, ....]
@@ -149,15 +158,15 @@
         self.contents.append(tbl)
         self.table_ident = None
         # Optional notes if data in columns truncated
         if len(self.note_data) > 0:
             notes = ["<br/><u>Notes</u><br/><ul>"]
             i = 1
             for d in self.note_data:
-                notes.append(f"<li>{str(i)} . {d}</li>")
+                notes.append(f"<li>{str(i):>4} . {d}</li>")
                 i += 1
             self._notes_paragraph("</ul><br/>".join(notes))
             self.note_data = []
         self._spacer()
 
     def pagebreak(self):
         self.contents.append(PageBreak())
```

## Comparing `sbom2doc-0.1.2.dist-info/LICENSE` & `sbom2doc-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbom2doc-0.1.2.dist-info/METADATA` & `sbom2doc-0.2.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbom2doc
-Version: 0.1.2
+Version: 0.2.0
 Summary: SBOM generator for Python modules
 Home-page: https://github.com/anthonyharrison/sbom2doc
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -20,17 +20,18 @@
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
 Requires-Dist: reportlab
+Requires-Dist: packageurl-python
 
 # SBOM2DOC
 
 SBOM2DOC documents and summarises the components within an SBOM (Software Bill of Materials). SBOMS are supported in a number of formats including
 [SPDX](https://www.spdx.org) and [CycloneDX](https://www.cyclonedx.org).
 
 ## Installation
@@ -47,31 +48,31 @@
 if you are using different versions of python. `virtualenv` is a tool for setting up virtual python environments which
 allows you to have all the dependencies for the tool set up in a single environment, or have different environments set
 up for testing using different versions of Python.
 
 ## Usage
 
 ```
-usage: sbom2doc [-h] [-i INPUT_FILE] [--debug] [-f {console,markdown,pdf}] [-o OUTPUT_FILE] [-V]
+usage: sbom2doc [-h] [-i INPUT_FILE] [--debug] [--include-license] [-f {console,markdown,pdf}] [-o OUTPUT_FILE] [-V]
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
 
 Input:
   -i INPUT_FILE, --input-file INPUT_FILE
                         Name of SBOM file
 
 Output:
   --debug               add debug information
+  --include-license     add license text
   -f {console,markdown,pdf}, --format {console,markdown,pdf}
                         Output format (default: output to console)
   -o OUTPUT_FILE, --output-file OUTPUT_FILE
                         output filename (default: output to stdout)
-
 ```
 					
 ## Operation
 
 The `--input-file` option is used to specify the SBOM to be processed. The format of the SBOM is determined according to
 the following filename conventions.
 
@@ -80,129 +81,149 @@
 | SPDX      | TagValue  | .spdx              |
 | SPDX      | JSON      | .spdx.json         |
 | SPDX      | YAML      | .spdx.yaml         |
 | SPDX      | YAML      | .spdx.yml          |
 | CycloneDX | JSON      | .json              |
 
 The `--output-file` option is used to control the destination of the output generated by the tool. The
-default is to report to the console but it can be stored in a file (specified using `--output-file` option).
+default is to report to the console, but it can also be stored in a file (specified using `--output-file` option).
+
+The `--include-license` option is used to indicate if the text for the licenses is to be included in the output.
 
 ## Example
 
 Given the following SBOM (flask.spdx)
 
-```
-SPDXVersion: SPDX-2.2
+```bash
+SPDXVersion: SPDX-2.3
 DataLicense: CC0-1.0
 SPDXID: SPDXRef-DOCUMENT
-DocumentName: flask
-DocumentNamespace: http://spdx.org/spdxdocs/flask-529abb33-fcd0-4d40-9de8-38e97ff00df9
-LicenseListVersion: 3.18
-Creator: Tool: sbom4python-0.7.0
-Created: 2023-01-27T16:16:26Z
+DocumentName: Python-flask
+DocumentNamespace: http://spdx.org/spdxdocs/Python-flask-0d6084b4-1a7b-42f7-97e2-65bc4b109783
+LicenseListVersion: 3.20
+Creator: Tool: sbom4python-0.9.0
+Created: 2023-03-31T11:01:17Z
 CreatorComment: <text>This document has been automatically generated.</text>
+##### 
 
 PackageName: flask
 SPDXID: SPDXRef-Package-1-flask
-PackageSupplier: Person: Armin Ronacher (armin.ronacher@active-4.com)
 PackageVersion: 2.2.2
-PackageDownloadLocation: NOASSERTION
+PackageSupplier: Person: Armin Ronacher (armin.ronacher@active-4.com)
+PackageDownloadLocation: https://pypi.org/project/Flask/2.2.2
 FilesAnalyzed: false
-PackageLicenseConcluded: BSD-3-Clause
+PackageHomePage: https://palletsprojects.com/p/flask
 PackageLicenseDeclared: BSD-3-Clause
+PackageLicenseConcluded: BSD-3-Clause
 PackageCopyrightText: NOASSERTION
+PackageSummary: A simple framework for building complex web applications.
 ExternalRef: PACKAGE-MANAGER purl pkg:pypi/flask@2.2.2
 ExternalRef: SECURITY cpe23Type cpe:2.3:a:armin_ronacher:flask:2.2.2:*:*:*:*:*:*:*
+##### 
 
 PackageName: click
 SPDXID: SPDXRef-Package-2-click
-PackageSupplier: Person: Armin Ronacher (armin.ronacher@active-4.com)
 PackageVersion: 8.0.3
-PackageDownloadLocation: NOASSERTION
+PackageSupplier: Person: Armin Ronacher (armin.ronacher@active-4.com)
+PackageDownloadLocation: https://pypi.org/project/click/8.0.3
 FilesAnalyzed: false
-PackageLicenseConcluded: BSD-3-Clause
+PackageHomePage: https://palletsprojects.com/p/click/
 PackageLicenseDeclared: BSD-3-Clause
+PackageLicenseConcluded: BSD-3-Clause
 PackageCopyrightText: NOASSERTION
+PackageSummary: Composable command line interface toolkit
 ExternalRef: PACKAGE-MANAGER purl pkg:pypi/click@8.0.3
 ExternalRef: SECURITY cpe23Type cpe:2.3:a:armin_ronacher:click:8.0.3:*:*:*:*:*:*:*
+##### 
 
 PackageName: itsdangerous
 SPDXID: SPDXRef-Package-3-itsdangerous
-PackageSupplier: Person: Armin Ronacher (armin.ronacher@active-4.com)
 PackageVersion: 2.1.2
-PackageDownloadLocation: NOASSERTION
+PackageSupplier: Person: Armin Ronacher (armin.ronacher@active-4.com)
+PackageDownloadLocation: https://pypi.org/project/itsdangerous/2.1.2
 FilesAnalyzed: false
-PackageLicenseConcluded: BSD-3-Clause
+PackageHomePage: https://palletsprojects.com/p/itsdangerous/
 PackageLicenseDeclared: BSD-3-Clause
+PackageLicenseConcluded: BSD-3-Clause
 PackageCopyrightText: NOASSERTION
+PackageSummary: Safely pass data to untrusted environments and back.
 ExternalRef: PACKAGE-MANAGER purl pkg:pypi/itsdangerous@2.1.2
 ExternalRef: SECURITY cpe23Type cpe:2.3:a:armin_ronacher:itsdangerous:2.1.2:*:*:*:*:*:*:*
+##### 
 
 PackageName: jinja2
 SPDXID: SPDXRef-Package-4-jinja2
-PackageSupplier: Person: Armin Ronacher (armin.ronacher@active-4.com)
 PackageVersion: 3.0.2
-PackageDownloadLocation: NOASSERTION
+PackageSupplier: Person: Armin Ronacher (armin.ronacher@active-4.com)
+PackageDownloadLocation: https://pypi.org/project/Jinja2/3.0.2
 FilesAnalyzed: false
-PackageLicenseConcluded: BSD-3-Clause
+PackageHomePage: https://palletsprojects.com/p/jinja/
 PackageLicenseDeclared: BSD-3-Clause
+PackageLicenseConcluded: BSD-3-Clause
 PackageCopyrightText: NOASSERTION
+PackageSummary: A very fast and expressive template engine.
 ExternalRef: PACKAGE-MANAGER purl pkg:pypi/jinja2@3.0.2
 ExternalRef: SECURITY cpe23Type cpe:2.3:a:armin_ronacher:jinja2:3.0.2:*:*:*:*:*:*:*
+##### 
 
 PackageName: markupsafe
 SPDXID: SPDXRef-Package-5-markupsafe
-PackageSupplier: Person: Armin Ronacher (armin.ronacher@active-4.com)
 PackageVersion: 2.1.1
-PackageDownloadLocation: NOASSERTION
+PackageSupplier: Person: Armin Ronacher (armin.ronacher@active-4.com)
+PackageDownloadLocation: https://pypi.org/project/MarkupSafe/2.1.1
 FilesAnalyzed: false
-PackageLicenseConcluded: BSD-3-Clause
+PackageHomePage: https://palletsprojects.com/p/markupsafe/
 PackageLicenseDeclared: BSD-3-Clause
+PackageLicenseConcluded: BSD-3-Clause
 PackageCopyrightText: NOASSERTION
+PackageSummary: Safely add untrusted strings to HTML/XML markup.
 ExternalRef: PACKAGE-MANAGER purl pkg:pypi/markupsafe@2.1.1
 ExternalRef: SECURITY cpe23Type cpe:2.3:a:armin_ronacher:markupsafe:2.1.1:*:*:*:*:*:*:*
+##### 
 
 PackageName: werkzeug
 SPDXID: SPDXRef-Package-6-werkzeug
-PackageSupplier: Person: Armin Ronacher (armin.ronacher@active-4.com)
 PackageVersion: 2.2.2
-PackageDownloadLocation: NOASSERTION
+PackageSupplier: Person: Armin Ronacher (armin.ronacher@active-4.com)
+PackageDownloadLocation: https://pypi.org/project/Werkzeug/2.2.2
 FilesAnalyzed: false
-PackageLicenseConcluded: BSD-3-Clause
+PackageHomePage: https://palletsprojects.com/p/werkzeug/
 PackageLicenseDeclared: BSD-3-Clause
+PackageLicenseConcluded: BSD-3-Clause
 PackageCopyrightText: NOASSERTION
+PackageSummary: The comprehensive WSGI web application library.
 ExternalRef: PACKAGE-MANAGER purl pkg:pypi/werkzeug@2.2.2
 ExternalRef: SECURITY cpe23Type cpe:2.3:a:armin_ronacher:werkzeug:2.2.2:*:*:*:*:*:*:*
+##### 
+
 Relationship: SPDXRef-DOCUMENT DESCRIBES SPDXRef-Package-1-flask
 Relationship: SPDXRef-Package-1-flask DEPENDS_ON SPDXRef-Package-2-click
 Relationship: SPDXRef-Package-1-flask DEPENDS_ON SPDXRef-Package-3-itsdangerous
 Relationship: SPDXRef-Package-1-flask DEPENDS_ON SPDXRef-Package-4-jinja2
 Relationship: SPDXRef-Package-1-flask DEPENDS_ON SPDXRef-Package-6-werkzeug
 Relationship: SPDXRef-Package-4-jinja2 DEPENDS_ON SPDXRef-Package-5-markupsafe
 Relationship: SPDXRef-Package-6-werkzeug DEPENDS_ON SPDXRef-Package-5-markupsafe
-
 ```
 
 The following commands will generate a summary of the contents of the SBOM to the console.
 
-```
+```bash
 sbom2doc --input flask.spdx 
 
-╭──────────────╮
 │ SBOM Summary │
 ╰──────────────╯
 ┏━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━┓
 ┃ Item          ┃ Details                ┃
 ┡━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━┩
 │ SBOM File     │ /tmp/flask.spdx        │
 │ SBOM Type     │ spdx                   │
-│ Version       │ SPDX-2.2               │
-│ Name          │ flask                  │
-│ Creator       │ Tool:sbom4python-0.7.0 │
-│ Created       │ 2023-01-30T18:10:18Z   │
+│ Version       │ SPDX-2.3               │
+│ Name          │ Python-flask           │
+│ Creator       │ Tool:sbom4python-0.9.0 │
+│ Created       │ 2023-03-31T11:01:17Z   │
 │ Files         │ 0                      │
 │ Packages      │ 6                      │
 │ Relationships │ 7                      │
 └───────────────┴────────────────────────┘
 ╭─────────────────╮
 │ Package Summary │
 ╰─────────────────╯
@@ -212,14 +233,24 @@
 │ flask        │ 2.2.2   │ Armin Ronacher (armin.ronacher@active-4.com) │ BSD-3-Clause │
 │ click        │ 8.0.3   │ Armin Ronacher (armin.ronacher@active-4.com) │ BSD-3-Clause │
 │ itsdangerous │ 2.1.2   │ Armin Ronacher (armin.ronacher@active-4.com) │ BSD-3-Clause │
 │ jinja2       │ 3.0.2   │ Armin Ronacher (armin.ronacher@active-4.com) │ BSD-3-Clause │
 │ markupsafe   │ 2.1.1   │ Armin Ronacher (armin.ronacher@active-4.com) │ BSD-3-Clause │
 │ werkzeug     │ 2.2.2   │ Armin Ronacher (armin.ronacher@active-4.com) │ BSD-3-Clause │
 └──────────────┴─────────┴──────────────────────────────────────────────┴──────────────┘
+┏━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━┓
+┃ Name         ┃ Version ┃ Download                                    ┃ Copyright ┃
+┡━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━┩
+│ flask        │ 2.2.2   │ https://pypi.org/project/Flask/2.2.2        │ -         │
+│ click        │ 8.0.3   │ https://pypi.org/project/click/8.0.3        │ -         │
+│ itsdangerous │ 2.1.2   │ https://pypi.org/project/itsdangerous/2.1.2 │ -         │
+│ jinja2       │ 3.0.2   │ https://pypi.org/project/Jinja2/3.0.2       │ -         │
+│ markupsafe   │ 2.1.1   │ https://pypi.org/project/MarkupSafe/2.1.1   │ -         │
+│ werkzeug     │ 2.2.2   │ https://pypi.org/project/Werkzeug/2.2.2     │ -         │
+└──────────────┴─────────┴─────────────────────────────────────────────┴───────────┘
 ╭─────────────────╮
 │ License Summary │
 ╰─────────────────╯
 ┏━━━━━━━━━━━━━━┳━━━━━━━┓
 ┃ License      ┃ Count ┃
 ┡━━━━━━━━━━━━━━╇━━━━━━━┩
 │ BSD-3-Clause │ 6     │
```

## Comparing `sbom2doc-0.1.2.dist-info/RECORD` & `sbom2doc-0.2.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 sbom2doc/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
-sbom2doc/cli.py,sha256=WXbbYh5s0d6lFuwWTwflejnobHCzSB9Sl2BEQvCmstA,2592
-sbom2doc/generator.py,sha256=OtGDgTaw30QAXAyw5n77JSExdSLbhsAbARA1aeV1MzY,4946
-sbom2doc/version.py,sha256=hrPdaOLNANEcNndLBVrZaUWgb423W5Fht_jiswwp470,100
-sbom2doc/docbuilder/__init__.py,sha256=Jdm3si-iktHDtKWwHpYgVfLYF-l1bE6TQDJASgkVpQU,75
-sbom2doc/docbuilder/consolebuilder.py,sha256=DFRjiVKnEyzUPvtBDoEW32WqztPWFuRO6hqkzIQry4g,1241
-sbom2doc/docbuilder/docbuilder.py,sha256=TOpP6lWz7pZl0X3w1riXYDCqsrn-crRFlvOhHesNsog,429
-sbom2doc/docbuilder/markdownbuilder.py,sha256=5KoRi-UgLVzNEapyPDjJ81q33-qR3mN1AsyNej1j3P8,1094
-sbom2doc/docbuilder/pdfbuilder.py,sha256=f4l121liCKxfkT2lrpRww0MXGLhMTffMCxzO98PJl8E,5462
-sbom2doc-0.1.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbom2doc-0.1.2.dist-info/METADATA,sha256=xUJWIjRLwGOtGUK-HKicwTMCnks6SsFidiiBD4EJ3yc,11501
-sbom2doc-0.1.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-sbom2doc-0.1.2.dist-info/entry_points.txt,sha256=-bmvwIx9D5RZ0FGkoBtdSqwTXAE5wSiDHhY4jCsdCOk,47
-sbom2doc-0.1.2.dist-info/top_level.txt,sha256=SgNoJfZaHup5cF818Xlucq4NcZ-Ukxtm0E99YmxDc3c,9
-sbom2doc-0.1.2.dist-info/RECORD,,
+sbom2doc/cli.py,sha256=DmYEtaBzQ5qvLQg7alD-tC13mqXJNJ7Pr-WN54ofoY0,2915
+sbom2doc/generator.py,sha256=iMIL9V14oTxJ62mXQ7JL7ymK9xhy1PSD5TBE-peHa2k,7083
+sbom2doc/version.py,sha256=Mustbl9r6LIU5iErNlnCJ7lyI7PZQHJcJDUDLTkW-p8,100
+sbom2doc/docbuilder/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
+sbom2doc/docbuilder/consolebuilder.py,sha256=QGFAcgk7q7eL2Y8141xPWFBUEwDiQ0XNwCRFbC7-BL8,1367
+sbom2doc/docbuilder/docbuilder.py,sha256=U8mvemVpbRg2a2NR0x-eaGAIpd6bY2bq_MZ3_IbcAi4,481
+sbom2doc/docbuilder/markdownbuilder.py,sha256=Io56grxZYX3yNnEBbFehty8zxq1V8XPEXANPPgtb8Ao,1107
+sbom2doc/docbuilder/pdfbuilder.py,sha256=I7sFtSW-Wrg3zDbPU1NKEGhARAZQr-zShe-yVbG_UCA,5818
+sbom2doc-0.2.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbom2doc-0.2.0.dist-info/METADATA,sha256=w5J7LYt8j_WRsglmISk5i7-a2wrdeEY3cib-e-GXMTU,14054
+sbom2doc-0.2.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+sbom2doc-0.2.0.dist-info/entry_points.txt,sha256=-bmvwIx9D5RZ0FGkoBtdSqwTXAE5wSiDHhY4jCsdCOk,47
+sbom2doc-0.2.0.dist-info/top_level.txt,sha256=SgNoJfZaHup5cF818Xlucq4NcZ-Ukxtm0E99YmxDc3c,9
+sbom2doc-0.2.0.dist-info/RECORD,,
```

