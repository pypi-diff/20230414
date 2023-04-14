# Comparing `tmp/openabc-1.0.1.tar.gz` & `tmp/openabc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openabc-1.0.1.tar", last modified: Fri Apr 14 21:16:41 2023, max compression
+gzip compressed data, was "openabc-1.0.2.tar", last modified: Fri Apr 14 21:42:59 2023, max compression
```

## Comparing `openabc-1.0.1.tar` & `openabc-1.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:16:41.000000 openabc-1.0.1/
--rw-rw----   0 sliu     (61642) sliu     (61642)     1080 2023-04-14 18:10:57.000000 openabc-1.0.1/LICENSE
--rw-rw----   0 sliu     (61642) sliu     (61642)      121 2023-04-14 20:42:49.000000 openabc-1.0.1/MANIFEST.in
--rw-rw----   0 sliu     (61642) sliu     (61642)     1377 2023-04-14 21:16:41.000000 openabc-1.0.1/PKG-INFO
--rw-rw----   0 sliu     (61642) sliu     (61642)     1094 2023-04-14 21:02:42.000000 openabc-1.0.1/README.md
--rw-rw----   0 sliu     (61642) sliu     (61642)      428 2023-04-14 21:04:09.000000 openabc-1.0.1/pyproject.toml
--rw-rw----   0 sliu     (61642) sliu     (61642)       38 2023-04-14 21:16:41.000000 openabc-1.0.1/setup.cfg
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:16:40.000000 openabc-1.0.1/src/
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:16:40.000000 openabc-1.0.1/src/openabc/
--rw-rw----   0 sliu     (61642) sliu     (61642)       23 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/__init__.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:16:40.000000 openabc-1.0.1/src/openabc/forcefields/
--rw-rw----   0 sliu     (61642) sliu     (61642)       73 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/__init__.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    11969 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/cg_model.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:16:41.000000 openabc-1.0.1/src/openabc/forcefields/functional_terms/
--rw-rw----   0 sliu     (61642) sliu     (61642)      114 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/functional_terms/__init__.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     1317 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/functional_terms/angle_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     4121 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/functional_terms/bond_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)      717 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/functional_terms/dihedral_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     9168 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/functional_terms/nonbonded_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     3281 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     4779 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/hps_model.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     3058 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/hps_zero_offset_model.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     9863 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/moff_mrg_model.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:16:41.000000 openabc-1.0.1/src/openabc/forcefields/parameters/
--rw-rw----   0 sliu     (61642) sliu     (61642)     4287 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/parameters/HPS_KR_parameters.csv
--rw-rw----   0 sliu     (61642) sliu     (61642)     4904 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/parameters/HPS_Urry_parameters.csv
--rw-rw----   0 sliu     (61642) sliu     (61642)    11557 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/parameters/MOFF_contact_parameters.csv
--rw-rw----   0 sliu     (61642) sliu     (61642)     3372 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/parameters/parse_hps_parameters.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     1231 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/parameters/parse_moff_parameters.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    12545 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/parameters/template_MOFF.top
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:16:41.000000 openabc-1.0.1/src/openabc/forcefields/parsers/
--rw-rw----   0 sliu     (61642) sliu     (61642)      110 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/parsers/__init__.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     4016 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/parsers/hps_parser.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     9129 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/parsers/moff_parser.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     7485 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/parsers/mrg_parser.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     7347 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/forcefields/rigid.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:16:41.000000 openabc-1.0.1/src/openabc/utils/
--rw-rw----   0 sliu     (61642) sliu     (61642)     9312 2023-04-14 18:10:25.000000 openabc-1.0.1/src/openabc/utils/CA2AA.py
--rw-rw----   0 sliu     (61642) sliu     (61642)        0 2023-04-14 18:10:24.000000 openabc-1.0.1/src/openabc/utils/__init__.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    11095 2023-04-14 18:10:25.000000 openabc-1.0.1/src/openabc/utils/helper_functions.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     4916 2023-04-14 18:10:25.000000 openabc-1.0.1/src/openabc/utils/insert.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    11519 2023-04-14 18:10:25.000000 openabc-1.0.1/src/openabc/utils/legacy_shadow_map.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     9102 2023-04-14 18:10:25.000000 openabc-1.0.1/src/openabc/utils/replica_exchange.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    15174 2023-04-14 18:10:25.000000 openabc-1.0.1/src/openabc/utils/shadow_map.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:16:40.000000 openabc-1.0.1/src/openabc.egg-info/
--rw-rw----   0 sliu     (61642) sliu     (61642)     1377 2023-04-14 21:16:40.000000 openabc-1.0.1/src/openabc.egg-info/PKG-INFO
--rw-rw----   0 sliu     (61642) sliu     (61642)     1562 2023-04-14 21:16:40.000000 openabc-1.0.1/src/openabc.egg-info/SOURCES.txt
--rw-rw----   0 sliu     (61642) sliu     (61642)        1 2023-04-14 21:16:40.000000 openabc-1.0.1/src/openabc.egg-info/dependency_links.txt
--rw-rw----   0 sliu     (61642) sliu     (61642)        8 2023-04-14 21:16:40.000000 openabc-1.0.1/src/openabc.egg-info/top_level.txt
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1080 2023-04-14 18:10:57.000000 openabc-1.0.2/LICENSE
+-rw-rw----   0 sliu     (61642) sliu     (61642)      121 2023-04-14 20:42:49.000000 openabc-1.0.2/MANIFEST.in
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1377 2023-04-14 21:42:59.000000 openabc-1.0.2/PKG-INFO
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1094 2023-04-14 21:02:42.000000 openabc-1.0.2/README.md
+-rw-rw----   0 sliu     (61642) sliu     (61642)      428 2023-04-14 21:37:17.000000 openabc-1.0.2/pyproject.toml
+-rw-rw----   0 sliu     (61642) sliu     (61642)       38 2023-04-14 21:42:59.000000 openabc-1.0.2/setup.cfg
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc/
+-rw-rw----   0 sliu     (61642) sliu     (61642)       23 2023-04-14 21:37:29.000000 openabc-1.0.2/src/openabc/__init__.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc/forcefields/
+-rw-rw----   0 sliu     (61642) sliu     (61642)       73 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/__init__.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    11969 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/cg_model.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/
+-rw-rw----   0 sliu     (61642) sliu     (61642)      114 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/__init__.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1317 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/angle_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4121 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/bond_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)      717 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/dihedral_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     9168 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/nonbonded_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     3281 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4779 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/hps_model.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     3058 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/hps_zero_offset_model.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     9863 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/moff_mrg_model.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc/forcefields/parameters/
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4287 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parameters/HPS_KR_parameters.csv
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4904 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parameters/HPS_Urry_parameters.csv
+-rw-rw----   0 sliu     (61642) sliu     (61642)    11557 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parameters/MOFF_contact_parameters.csv
+-rw-rw----   0 sliu     (61642) sliu     (61642)     3372 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parameters/parse_hps_parameters.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1231 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parameters/parse_moff_parameters.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    12545 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parameters/template_MOFF.top
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc/forcefields/parsers/
+-rw-rw----   0 sliu     (61642) sliu     (61642)      110 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parsers/__init__.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4016 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parsers/hps_parser.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     9129 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parsers/moff_parser.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     7485 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parsers/mrg_parser.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     7347 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/rigid.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc/utils/
+-rw-rw----   0 sliu     (61642) sliu     (61642)     9312 2023-04-14 18:10:25.000000 openabc-1.0.2/src/openabc/utils/CA2AA.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)        0 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/utils/__init__.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    11095 2023-04-14 18:10:25.000000 openabc-1.0.2/src/openabc/utils/helper_functions.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4916 2023-04-14 18:10:25.000000 openabc-1.0.2/src/openabc/utils/insert.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    11519 2023-04-14 18:10:25.000000 openabc-1.0.2/src/openabc/utils/legacy_shadow_map.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     9102 2023-04-14 18:10:25.000000 openabc-1.0.2/src/openabc/utils/replica_exchange.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    15174 2023-04-14 18:10:25.000000 openabc-1.0.2/src/openabc/utils/shadow_map.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc.egg-info/
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1377 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc.egg-info/PKG-INFO
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1562 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc.egg-info/SOURCES.txt
+-rw-rw----   0 sliu     (61642) sliu     (61642)        1 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc.egg-info/dependency_links.txt
+-rw-rw----   0 sliu     (61642) sliu     (61642)        8 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc.egg-info/top_level.txt
```

### Comparing `openabc-1.0.1/LICENSE` & `openabc-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/PKG-INFO` & `openabc-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openabc
-Version: 1.0.1
+Version: 1.0.2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `openabc-1.0.1/README.md` & `openabc-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/cg_model.py` & `openabc-1.0.2/src/openabc/forcefields/cg_model.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/functional_terms/angle_terms.py` & `openabc-1.0.2/src/openabc/forcefields/functional_terms/angle_terms.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/functional_terms/bond_terms.py` & `openabc-1.0.2/src/openabc/forcefields/functional_terms/bond_terms.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/functional_terms/dihedral_terms.py` & `openabc-1.0.2/src/openabc/forcefields/functional_terms/dihedral_terms.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/functional_terms/nonbonded_terms.py` & `openabc-1.0.2/src/openabc/forcefields/functional_terms/nonbonded_terms.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py` & `openabc-1.0.2/src/openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/hps_model.py` & `openabc-1.0.2/src/openabc/forcefields/hps_model.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/hps_zero_offset_model.py` & `openabc-1.0.2/src/openabc/forcefields/hps_zero_offset_model.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/moff_mrg_model.py` & `openabc-1.0.2/src/openabc/forcefields/moff_mrg_model.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/parameters/HPS_KR_parameters.csv` & `openabc-1.0.2/src/openabc/forcefields/parameters/HPS_KR_parameters.csv`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/parameters/HPS_Urry_parameters.csv` & `openabc-1.0.2/src/openabc/forcefields/parameters/HPS_Urry_parameters.csv`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/parameters/MOFF_contact_parameters.csv` & `openabc-1.0.2/src/openabc/forcefields/parameters/MOFF_contact_parameters.csv`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/parameters/parse_hps_parameters.py` & `openabc-1.0.2/src/openabc/forcefields/parameters/parse_hps_parameters.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/parameters/parse_moff_parameters.py` & `openabc-1.0.2/src/openabc/forcefields/parameters/parse_moff_parameters.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/parameters/template_MOFF.top` & `openabc-1.0.2/src/openabc/forcefields/parameters/template_MOFF.top`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/parsers/hps_parser.py` & `openabc-1.0.2/src/openabc/forcefields/parsers/hps_parser.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/parsers/moff_parser.py` & `openabc-1.0.2/src/openabc/forcefields/parsers/moff_parser.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/parsers/mrg_parser.py` & `openabc-1.0.2/src/openabc/forcefields/parsers/mrg_parser.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/forcefields/rigid.py` & `openabc-1.0.2/src/openabc/forcefields/rigid.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/utils/CA2AA.py` & `openabc-1.0.2/src/openabc/utils/CA2AA.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/utils/helper_functions.py` & `openabc-1.0.2/src/openabc/utils/helper_functions.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/utils/insert.py` & `openabc-1.0.2/src/openabc/utils/insert.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/utils/legacy_shadow_map.py` & `openabc-1.0.2/src/openabc/utils/legacy_shadow_map.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/utils/replica_exchange.py` & `openabc-1.0.2/src/openabc/utils/replica_exchange.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc/utils/shadow_map.py` & `openabc-1.0.2/src/openabc/utils/shadow_map.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.1/src/openabc.egg-info/PKG-INFO` & `openabc-1.0.2/src/openabc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openabc
-Version: 1.0.1
+Version: 1.0.2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `openabc-1.0.1/src/openabc.egg-info/SOURCES.txt` & `openabc-1.0.2/src/openabc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

