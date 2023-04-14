# Comparing `tmp/sbol-utilities-1.0a8.tar.gz` & `tmp/sbol-utilities-1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sbol-utilities-1.0a8.tar", last modified: Thu Sep 16 11:08:14 2021, max compression
+gzip compressed data, was "dist/sbol-utilities-1.0a9.tar", last modified: Sat Sep 18 19:04:49 2021, max compression
```

## Comparing `sbol-utilities-1.0a8.tar` & `sbol-utilities-1.0a9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jakebeal   (502) staff       (20)        0 2021-09-16 11:08:14.000000 sbol-utilities-1.0a8/
--rw-r--r--   0 jakebeal   (502) staff       (20)      600 2021-09-16 11:08:14.000000 sbol-utilities-1.0a8/PKG-INFO
-drwxr-xr-x   0 jakebeal   (502) staff       (20)        0 2021-09-16 11:08:14.000000 sbol-utilities-1.0a8/test/
--rw-r--r--   0 jakebeal   (502) staff       (20)     3761 2021-09-12 01:12:55.000000 sbol-utilities-1.0a8/test/test_expand_combinatorial_derivations.py
--rw-r--r--   0 jakebeal   (502) staff       (20)     1543 2021-09-12 01:12:55.000000 sbol-utilities-1.0a8/test/test_helpers.py
--rw-r--r--   0 jakebeal   (502) staff       (20)     4951 2021-09-12 01:12:55.000000 sbol-utilities-1.0a8/test/test_excel_to_sbol.py
--rw-r--r--   0 jakebeal   (502) staff       (20)     5929 2021-09-12 01:12:55.000000 sbol-utilities-1.0a8/test/test_calculate_sequences.py
--rwxr-xr-x   0 jakebeal   (502) staff       (20)     5097 2021-08-08 14:22:22.000000 sbol-utilities-1.0a8/graph-sbol
--rw-r--r--   0 jakebeal   (502) staff       (20)     1290 2021-09-12 01:12:55.000000 sbol-utilities-1.0a8/README.md
--rw-r--r--   0 jakebeal   (502) staff       (20)     1818 2021-09-16 11:08:11.000000 sbol-utilities-1.0a8/setup.py
-drwxr-xr-x   0 jakebeal   (502) staff       (20)        0 2021-09-16 11:08:14.000000 sbol-utilities-1.0a8/sbol_utilities/
--rw-r--r--   0 jakebeal   (502) staff       (20)     6338 2021-09-12 01:12:55.000000 sbol-utilities-1.0a8/sbol_utilities/helper_functions.py
--rw-r--r--   0 jakebeal   (502) staff       (20)    11117 2021-09-12 01:12:55.000000 sbol-utilities-1.0a8/sbol_utilities/expand_combinatorial_derivations.py
--rw-r--r--   0 jakebeal   (502) staff       (20)     5074 2021-08-08 14:22:22.000000 sbol-utilities-1.0a8/sbol_utilities/graph_sbol.py
--rw-r--r--   0 jakebeal   (502) staff       (20)        0 2021-08-08 14:22:22.000000 sbol-utilities-1.0a8/sbol_utilities/__init__.py
--rw-r--r--   0 jakebeal   (502) staff       (20)     8197 2021-09-12 01:12:55.000000 sbol-utilities-1.0a8/sbol_utilities/calculate_sequences.py
--rw-r--r--   0 jakebeal   (502) staff       (20)    25552 2021-09-12 01:12:55.000000 sbol-utilities-1.0a8/sbol_utilities/excel_to_sbol.py
--rw-r--r--   0 jakebeal   (502) staff       (20)       38 2021-09-16 11:08:14.000000 sbol-utilities-1.0a8/setup.cfg
-drwxr-xr-x   0 jakebeal   (502) staff       (20)        0 2021-09-16 11:08:14.000000 sbol-utilities-1.0a8/sbol_utilities.egg-info/
--rw-r--r--   0 jakebeal   (502) staff       (20)      600 2021-09-16 11:08:14.000000 sbol-utilities-1.0a8/sbol_utilities.egg-info/PKG-INFO
--rw-r--r--   0 jakebeal   (502) staff       (20)      598 2021-09-16 11:08:14.000000 sbol-utilities-1.0a8/sbol_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 jakebeal   (502) staff       (20)      215 2021-09-16 11:08:14.000000 sbol-utilities-1.0a8/sbol_utilities.egg-info/entry_points.txt
--rw-r--r--   0 jakebeal   (502) staff       (20)       36 2021-09-16 11:08:14.000000 sbol-utilities-1.0a8/sbol_utilities.egg-info/requires.txt
--rw-r--r--   0 jakebeal   (502) staff       (20)       15 2021-09-16 11:08:14.000000 sbol-utilities-1.0a8/sbol_utilities.egg-info/top_level.txt
--rw-r--r--   0 jakebeal   (502) staff       (20)        1 2021-09-16 11:08:14.000000 sbol-utilities-1.0a8/sbol_utilities.egg-info/dependency_links.txt
+drwxr-xr-x   0 jakebeal   (502) staff       (20)        0 2021-09-18 19:04:49.000000 sbol-utilities-1.0a9/
+-rw-r--r--   0 jakebeal   (502) staff       (20)      600 2021-09-18 19:04:49.000000 sbol-utilities-1.0a9/PKG-INFO
+drwxr-xr-x   0 jakebeal   (502) staff       (20)        0 2021-09-18 19:04:49.000000 sbol-utilities-1.0a9/test/
+-rw-r--r--   0 jakebeal   (502) staff       (20)     3761 2021-09-12 01:12:55.000000 sbol-utilities-1.0a9/test/test_expand_combinatorial_derivations.py
+-rw-r--r--   0 jakebeal   (502) staff       (20)     2242 2021-09-18 19:04:27.000000 sbol-utilities-1.0a9/test/test_helpers.py
+-rw-r--r--   0 jakebeal   (502) staff       (20)     4951 2021-09-12 01:12:55.000000 sbol-utilities-1.0a9/test/test_excel_to_sbol.py
+-rw-r--r--   0 jakebeal   (502) staff       (20)     5929 2021-09-12 01:12:55.000000 sbol-utilities-1.0a9/test/test_calculate_sequences.py
+-rwxr-xr-x   0 jakebeal   (502) staff       (20)     5097 2021-08-08 14:22:22.000000 sbol-utilities-1.0a9/graph-sbol
+-rw-r--r--   0 jakebeal   (502) staff       (20)     1290 2021-09-12 01:12:55.000000 sbol-utilities-1.0a9/README.md
+-rw-r--r--   0 jakebeal   (502) staff       (20)     1818 2021-09-18 19:04:27.000000 sbol-utilities-1.0a9/setup.py
+drwxr-xr-x   0 jakebeal   (502) staff       (20)        0 2021-09-18 19:04:49.000000 sbol-utilities-1.0a9/sbol_utilities/
+-rw-r--r--   0 jakebeal   (502) staff       (20)     9429 2021-09-18 19:04:27.000000 sbol-utilities-1.0a9/sbol_utilities/helper_functions.py
+-rw-r--r--   0 jakebeal   (502) staff       (20)    11117 2021-09-12 01:12:55.000000 sbol-utilities-1.0a9/sbol_utilities/expand_combinatorial_derivations.py
+-rw-r--r--   0 jakebeal   (502) staff       (20)     5074 2021-08-08 14:22:22.000000 sbol-utilities-1.0a9/sbol_utilities/graph_sbol.py
+-rw-r--r--   0 jakebeal   (502) staff       (20)        0 2021-08-08 14:22:22.000000 sbol-utilities-1.0a9/sbol_utilities/__init__.py
+-rw-r--r--   0 jakebeal   (502) staff       (20)     8197 2021-09-12 01:12:55.000000 sbol-utilities-1.0a9/sbol_utilities/calculate_sequences.py
+-rw-r--r--   0 jakebeal   (502) staff       (20)    24613 2021-09-18 19:04:27.000000 sbol-utilities-1.0a9/sbol_utilities/excel_to_sbol.py
+-rw-r--r--   0 jakebeal   (502) staff       (20)       38 2021-09-18 19:04:49.000000 sbol-utilities-1.0a9/setup.cfg
+drwxr-xr-x   0 jakebeal   (502) staff       (20)        0 2021-09-18 19:04:49.000000 sbol-utilities-1.0a9/sbol_utilities.egg-info/
+-rw-r--r--   0 jakebeal   (502) staff       (20)      600 2021-09-18 19:04:49.000000 sbol-utilities-1.0a9/sbol_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 jakebeal   (502) staff       (20)      598 2021-09-18 19:04:49.000000 sbol-utilities-1.0a9/sbol_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 jakebeal   (502) staff       (20)      215 2021-09-18 19:04:49.000000 sbol-utilities-1.0a9/sbol_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 jakebeal   (502) staff       (20)       36 2021-09-18 19:04:49.000000 sbol-utilities-1.0a9/sbol_utilities.egg-info/requires.txt
+-rw-r--r--   0 jakebeal   (502) staff       (20)       15 2021-09-18 19:04:49.000000 sbol-utilities-1.0a9/sbol_utilities.egg-info/top_level.txt
+-rw-r--r--   0 jakebeal   (502) staff       (20)        1 2021-09-18 19:04:49.000000 sbol-utilities-1.0a9/sbol_utilities.egg-info/dependency_links.txt
```

### Comparing `sbol-utilities-1.0a8/PKG-INFO` & `sbol-utilities-1.0a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbol-utilities
-Version: 1.0a8
+Version: 1.0a9
 Summary: SBOL utilities
 Home-page: https://github.com/SynBioDex/SBOL-utilities
 License: MIT License
 Description: SBOL-utilities is a collection of scripts and functions for manipulating SBOL 3 data that can be imported as packages or run from the command line.
 Keywords: synthetic biology
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sbol-utilities-1.0a8/test/test_expand_combinatorial_derivations.py` & `sbol-utilities-1.0a9/test/test_expand_combinatorial_derivations.py`

 * *Files identical despite different names*

### Comparing `sbol-utilities-1.0a8/test/test_excel_to_sbol.py` & `sbol-utilities-1.0a9/test/test_excel_to_sbol.py`

 * *Files identical despite different names*

### Comparing `sbol-utilities-1.0a8/test/test_calculate_sequences.py` & `sbol-utilities-1.0a9/test/test_calculate_sequences.py`

 * *Files identical despite different names*

### Comparing `sbol-utilities-1.0a8/graph-sbol` & `sbol-utilities-1.0a9/graph-sbol`

 * *Files identical despite different names*

### Comparing `sbol-utilities-1.0a8/README.md` & `sbol-utilities-1.0a9/README.md`

 * *Files identical despite different names*

### Comparing `sbol-utilities-1.0a8/setup.py` & `sbol-utilities-1.0a9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 setup(name='sbol-utilities',
       description='SBOL utilities',
       long_description='SBOL-utilities is a collection of scripts and functions for manipulating SBOL 3 data that '
                        'can be imported as packages or run from the command line.',
       long_description_content_type='text/markdown',
       url='https://github.com/SynBioDex/SBOL-utilities',
       license='MIT License',
-      version='1.0a8',
+      version='1.0a9',
       # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
       classifiers=[
             # How mature is this project? Common values are
             #   3 - Alpha
             #   4 - Beta
             #   5 - Production/Stable
             'Development Status :: 3 - Alpha',
```

### Comparing `sbol-utilities-1.0a8/sbol_utilities/expand_combinatorial_derivations.py` & `sbol-utilities-1.0a9/sbol_utilities/expand_combinatorial_derivations.py`

 * *Files identical despite different names*

### Comparing `sbol-utilities-1.0a8/sbol_utilities/graph_sbol.py` & `sbol-utilities-1.0a9/sbol_utilities/graph_sbol.py`

 * *Files identical despite different names*

### Comparing `sbol-utilities-1.0a8/sbol_utilities/calculate_sequences.py` & `sbol-utilities-1.0a9/sbol_utilities/calculate_sequences.py`

 * *Files identical despite different names*

### Comparing `sbol-utilities-1.0a8/sbol_utilities/excel_to_sbol.py` & `sbol-utilities-1.0a9/sbol_utilities/excel_to_sbol.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import warnings
 import logging
 import re
 import argparse
 
 import sbol3
 import openpyxl
-import tyto
-from .helper_functions import toplevel_named, strip_sbol2_version, type_to_standard_extension, is_plasmid
+from .helper_functions import toplevel_named, strip_sbol2_version, type_to_standard_extension, is_plasmid, \
+    tyto_lookup_with_caching, string_to_display_id, url_to_identity, strip_filetype_suffix
 
 BASIC_PARTS_COLLECTION = 'BasicParts'
 COMPOSITE_PARTS_COLLECTION = 'CompositeParts'
 LINEAR_PRODUCTS_COLLECTION = 'LinearDNAProducts'
 FINAL_PRODUCTS_COLLECTION = 'FinalProducts'
 
 
@@ -64,32 +64,14 @@
             if k not in default_values:
                 raise ValueError(f'Sheet configuration has no setting "{k}"')
             values_to_use[k] = v
     # initialize the dictionary
     return values_to_use
 
 
-# TODO: remove after resolution of https://github.com/SynBioDex/pySBOL3/issues/191
-def string_to_display_id(name):
-    def sanitize_character(c):
-        replacements = {' ': '_', '-': '_', '.': '_'}
-        c = replacements.get(c, c)  # first, see if there is a wired replacement
-        if c.isalnum() or c == '_':  # keep allowed characters
-            return c
-        else:  # all others are changed into a reduced & compatible form of their unicode name
-            return f'_{unicodedata.name(c).replace(" SIGN","").replace(" ","_")}'
-
-    # make replacements in order to get a compliant displayID
-    display_id = "".join([sanitize_character(c) for c in name.strip()])
-    # prepend underscore if there is an initial digit
-    if display_id[0].isdigit():
-        display_id = "_"+display_id
-    return display_id
-
-
 def read_metadata(wb: openpyxl.Workbook, doc: sbol3.Document, config: dict):
     """
     Extract metadata and build collections
     :param wb: Excel workbook to extract material from
     :param doc: SBOL document to build collections in
     :param config: dictionary of sheet parsing configuration variables
     :return: Tuple of SBOL collections for basic, composite, linear, and final parts
@@ -119,34 +101,21 @@
     doc.add(linear_products)
 
     final_products = sbol3.Collection(FINAL_PRODUCTS_COLLECTION, name='Final Products',
                                       description='Final products desired for actual fabrication')
     doc.add(final_products)
 
     # also collect any necessary data tables from extra sheets
-    source_table = {row[config['source_name_col']].value:row[config['source_uri_col']].value
+    source_table = {row[config['source_name_col']].value: row[config['source_uri_col']].value
                     for row in wb[config['sources_sheet']].iter_rows(min_row=config['sources_first_row'])
                     if row[config['source_literal_col']].value}
 
     # return the set of created collections
     return basic_parts, composite_parts, linear_products, final_products, source_table
 
-# TODO: remove kludge after resolution of https://github.com/SynBioDex/tyto/issues/21
-tyto_cache = {}
-def tyto_lookup_with_caching(term: str) -> str:
-    if term not in tyto_cache:
-        try:
-            tyto_cache[term] = tyto.SO.get_uri_by_term(term)
-        except LookupError as e:
-            tyto_cache[term] = e
-    if isinstance(tyto_cache[term], LookupError):
-        raise tyto_cache[term]
-    else:
-        return tyto_cache[term]
-
 
 def row_to_basic_part(doc: sbol3.Document, row, basic_parts: sbol3.Collection, linear_products: sbol3.Collection,
                       final_products: sbol3.Collection, config: dict, source_table: dict):
     """
     Read a row for a basic part and turn it into SBOL Component
     :param doc: Document to add parts to
     :param row: Excel row to be processed
@@ -157,16 +126,16 @@
     :param source_table: dictionary mapping source names to namespaces
     :return: None
     """
     # Parse material from sheet row
     name = row[config['basic_name_col']].value
     if name is None:
         return  # skip lines without names
-    try:
-        raw_role = row[config['basic_role_col']].value  # look up with tyto; if fail, leave blank or add to description
+    raw_role = row[config['basic_role_col']].value
+    try:  # look up with tyto; if fail, leave blank or add to description
         role = (tyto_lookup_with_caching(raw_role) if raw_role else None)
     except LookupError:
         logging.warning(f'Role "{raw_role}" could not be found in Sequence Ontology')
         role = None
     design_notes = (row[config['basic_notes_col']].value if row[config['basic_notes_col']].value else "")
     description = (row[config['basic_description_col']].value if row[config['basic_description_col']].value else "")
     source_prefix = row[config['basic_source_prefix_col']].value
@@ -177,35 +146,41 @@
     raw_sequence = row[config['basic_sequence_col']].value
     sequence = (None if raw_sequence is None else "".join(unicodedata.normalize("NFKD", raw_sequence).upper().split()))
     if not ((sequence is None and length == 0) or len(sequence) == length):
         raise ValueError(f'Part "{name}" has mismatched sequence length: check for bad characters and extra whitespace')
 
     # identity comes from source if set to a literal table, from display_id if not set
     identity = None
+    display_id = None
+    was_derived_from = None
     if source_id and source_prefix:
         source_prefix = source_prefix.strip()
         if source_prefix in source_table:
             if source_table[source_prefix]:
                 display_id = string_to_display_id(source_id.strip())
                 identity = f'{source_table[source_prefix]}/{display_id}'
             else:  # when there is no prefix, use the bare value (in SBOL3 format)
-                identity = strip_sbol2_version(source_id.strip())
+                raw_url = source_id.strip()
+                identity = url_to_identity(strip_filetype_suffix(strip_sbol2_version(raw_url)))
+                was_derived_from = raw_url
         else:
             logging.info(f'Part "{name}" ignoring non-literal source: {source_prefix}')
     elif source_id:
         logging.warning(f'Part "{name}" has source ID specified but not prefix: {source_id}')
     elif source_prefix:
         logging.warning(f'Part "{name}" has source prefix specified but not ID: {source_prefix}')
     if not identity:
         display_id = string_to_display_id(name)
 
     # build a component from the material
     logging.debug(f'Creating basic part "{name}"')
     component = sbol3.Component(identity or display_id, sbol3.SBO_DNA, name=name,
                                 description=f'{design_notes}\n{description}'.strip())
+    if was_derived_from:
+        component.derived_from.append(was_derived_from)
     doc.add(component)
     if role:
         component.roles.append(role)
     if circular:
         component.types.append(sbol3.SO_CIRCULAR)
     if sequence:
         sbol_seq = sbol3.Sequence(f'{display_id}_sequence', encoding=sbol3.IUPAC_DNA_ENCODING, elements=sequence)
@@ -280,15 +255,15 @@
 def make_constraint(constraint, part_list):
     m = constraint_pattern.match(constraint)
     if not m:
         raise ValueError(f'Constraint "{constraint}" does not match pattern "Part X relation Part Y"')
     try:
         restriction = constraint_dict[m.group(2)]
     except KeyError:
-        raise ValueError(f'Do not recognize constraint relation "{restriction}"')
+        raise ValueError(f'Do not recognize constraint relation in "{constraint}"')
     x = int(m.group(1))
     y = int(m.group(3))
     if x is y:
         raise ValueError(f'A part cannot constrain itself: {constraint}')
     for n in [x,y]:
        if not (0 < n <= len(part_list)):
            raise ValueError(f'Part number "{str(n)}" is not between 1 and {len(part_list)}')
```

### Comparing `sbol-utilities-1.0a8/sbol_utilities.egg-info/PKG-INFO` & `sbol-utilities-1.0a9/sbol_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbol-utilities
-Version: 1.0a8
+Version: 1.0a9
 Summary: SBOL utilities
 Home-page: https://github.com/SynBioDex/SBOL-utilities
 License: MIT License
 Description: SBOL-utilities is a collection of scripts and functions for manipulating SBOL 3 data that can be imported as packages or run from the command line.
 Keywords: synthetic biology
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sbol-utilities-1.0a8/sbol_utilities.egg-info/SOURCES.txt` & `sbol-utilities-1.0a9/sbol_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

