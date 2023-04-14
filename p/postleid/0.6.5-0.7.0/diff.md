# Comparing `tmp/postleid-0.6.5.tar.gz` & `tmp/postleid-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postleid-0.6.5.tar", last modified: Wed Apr 12 16:51:12 2023, max compression
+gzip compressed data, was "postleid-0.7.0.tar", last modified: Fri Apr 14 16:02:32 2023, max compression
```

## Comparing `postleid-0.6.5.tar` & `postleid-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.817507 postleid-0.6.5/
--rw-r--r--   0 rainer    (1000) rainer    (1000)     1075 2023-04-05 15:58:25.000000 postleid-0.6.5/LICENSE
--rw-r--r--   0 rainer    (1000) rainer    (1000)     2949 2023-04-12 16:51:12.817507 postleid-0.6.5/PKG-INFO
--rw-r--r--   0 rainer    (1000) rainer    (1000)      317 2023-04-12 16:42:54.000000 postleid-0.6.5/README.md
--rw-r--r--   0 rainer    (1000) rainer    (1000)     1712 2023-04-07 14:20:30.000000 postleid-0.6.5/pyproject.toml
--rw-r--r--   0 rainer    (1000) rainer    (1000)       38 2023-04-12 16:51:12.817507 postleid-0.6.5/setup.cfg
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.813507 postleid-0.6.5/src/
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.813507 postleid-0.6.5/src/postleid/
--rw-r--r--   0 rainer    (1000) rainer    (1000)      580 2023-04-11 11:31:07.000000 postleid-0.6.5/src/postleid/__init__.py
--rwxr-xr-x   0 rainer    (1000) rainer    (1000)     7013 2023-04-09 19:19:40.000000 postleid-0.6.5/src/postleid/__main__.py
--rw-r--r--   0 rainer    (1000) rainer    (1000)     5403 2023-04-09 19:15:27.000000 postleid-0.6.5/src/postleid/commons.py
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.817507 postleid-0.6.5/src/postleid/data/
--rw-r--r--   0 rainer    (1000) rainer    (1000)     8989 2023-04-12 16:36:53.000000 postleid-0.6.5/src/postleid/data/country_names_by_cc.yaml
--rw-r--r--   0 rainer    (1000) rainer    (1000)     1490 2023-04-11 07:13:07.000000 postleid-0.6.5/src/postleid/data/default_user_settings.yaml
--rw-r--r--   0 rainer    (1000) rainer    (1000)    19220 2023-04-12 16:33:57.000000 postleid-0.6.5/src/postleid/data/postal_code_rules_by_cc.yaml
--rw-r--r--   0 rainer    (1000) rainer    (1000)    12391 2023-04-12 11:18:02.000000 postleid-0.6.5/src/postleid/fix_excel_files.py
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.813507 postleid-0.6.5/src/postleid/locale/
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.813507 postleid-0.6.5/src/postleid/locale/de/
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.817507 postleid-0.6.5/src/postleid/locale/de/LC_MESSAGES/
--rw-r--r--   0 rainer    (1000) rainer    (1000)     3749 2023-04-05 15:58:26.000000 postleid-0.6.5/src/postleid/locale/de/LC_MESSAGES/argparse.mo
--rw-r--r--   0 rainer    (1000) rainer    (1000)      738 2023-04-09 19:13:52.000000 postleid-0.6.5/src/postleid/paths.py
--rw-r--r--   0 rainer    (1000) rainer    (1000)     1194 2023-04-06 08:11:50.000000 postleid-0.6.5/src/postleid/presets.py
--rw-r--r--   0 rainer    (1000) rainer    (1000)    13925 2023-04-05 15:58:26.000000 postleid-0.6.5/src/postleid/rule_checks.py
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.817507 postleid-0.6.5/src/postleid.egg-info/
--rw-r--r--   0 rainer    (1000) rainer    (1000)     2949 2023-04-12 16:51:12.000000 postleid-0.6.5/src/postleid.egg-info/PKG-INFO
--rw-r--r--   0 rainer    (1000) rainer    (1000)      660 2023-04-12 16:51:12.000000 postleid-0.6.5/src/postleid.egg-info/SOURCES.txt
--rw-r--r--   0 rainer    (1000) rainer    (1000)        1 2023-04-12 16:51:12.000000 postleid-0.6.5/src/postleid.egg-info/dependency_links.txt
--rw-r--r--   0 rainer    (1000) rainer    (1000)       52 2023-04-12 16:51:12.000000 postleid-0.6.5/src/postleid.egg-info/entry_points.txt
--rw-r--r--   0 rainer    (1000) rainer    (1000)       54 2023-04-12 16:51:12.000000 postleid-0.6.5/src/postleid.egg-info/requires.txt
--rw-r--r--   0 rainer    (1000) rainer    (1000)        9 2023-04-12 16:51:12.000000 postleid-0.6.5/src/postleid.egg-info/top_level.txt
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-12 16:51:12.817507 postleid-0.6.5/tests/
--rw-r--r--   0 rainer    (1000) rainer    (1000)    13336 2023-04-05 15:58:26.000000 postleid-0.6.5/tests/test_commons.py
--rw-r--r--   0 rainer    (1000) rainer    (1000)     3630 2023-04-05 15:58:26.000000 postleid-0.6.5/tests/test_rule_checks.py
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-14 16:02:32.752840 postleid-0.7.0/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     1075 2023-04-05 15:58:25.000000 postleid-0.7.0/LICENSE
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     3651 2023-04-14 16:02:32.752840 postleid-0.7.0/PKG-INFO
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     1019 2023-04-14 15:32:14.000000 postleid-0.7.0/README.md
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     1712 2023-04-07 14:20:30.000000 postleid-0.7.0/pyproject.toml
+-rw-r--r--   0 rainer    (1000) rainer    (1000)       38 2023-04-14 16:02:32.752840 postleid-0.7.0/setup.cfg
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-14 16:02:32.752840 postleid-0.7.0/src/
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-14 16:02:32.752840 postleid-0.7.0/src/postleid/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)      580 2023-04-13 06:52:45.000000 postleid-0.7.0/src/postleid/__init__.py
+-rwxr-xr-x   0 rainer    (1000) rainer    (1000)    10023 2023-04-14 15:10:38.000000 postleid-0.7.0/src/postleid/__main__.py
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     5709 2023-04-13 10:34:27.000000 postleid-0.7.0/src/postleid/commons.py
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-14 16:02:32.752840 postleid-0.7.0/src/postleid/data/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)    21825 2023-04-14 13:39:20.000000 postleid-0.7.0/src/postleid/data/country_names_by_cc.yaml
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     1490 2023-04-11 07:13:07.000000 postleid-0.7.0/src/postleid/data/default_user_settings.yaml
+-rw-r--r--   0 rainer    (1000) rainer    (1000)    29674 2023-04-14 14:15:13.000000 postleid-0.7.0/src/postleid/data/postal_code_rules_by_cc.yaml
+-rw-r--r--   0 rainer    (1000) rainer    (1000)    12391 2023-04-12 11:18:02.000000 postleid-0.7.0/src/postleid/fix_excel_files.py
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-14 16:02:32.752840 postleid-0.7.0/src/postleid/locale/
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-14 16:02:32.752840 postleid-0.7.0/src/postleid/locale/de/
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-14 16:02:32.752840 postleid-0.7.0/src/postleid/locale/de/LC_MESSAGES/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     3749 2023-04-05 15:58:26.000000 postleid-0.7.0/src/postleid/locale/de/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 rainer    (1000) rainer    (1000)      738 2023-04-09 19:13:52.000000 postleid-0.7.0/src/postleid/paths.py
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     1194 2023-04-06 08:11:50.000000 postleid-0.7.0/src/postleid/presets.py
+-rw-r--r--   0 rainer    (1000) rainer    (1000)    14056 2023-04-13 07:41:52.000000 postleid-0.7.0/src/postleid/rule_checks.py
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-14 16:02:32.752840 postleid-0.7.0/src/postleid.egg-info/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     3651 2023-04-14 16:02:32.000000 postleid-0.7.0/src/postleid.egg-info/PKG-INFO
+-rw-r--r--   0 rainer    (1000) rainer    (1000)      660 2023-04-14 16:02:32.000000 postleid-0.7.0/src/postleid.egg-info/SOURCES.txt
+-rw-r--r--   0 rainer    (1000) rainer    (1000)        1 2023-04-14 16:02:32.000000 postleid-0.7.0/src/postleid.egg-info/dependency_links.txt
+-rw-r--r--   0 rainer    (1000) rainer    (1000)       52 2023-04-14 16:02:32.000000 postleid-0.7.0/src/postleid.egg-info/entry_points.txt
+-rw-r--r--   0 rainer    (1000) rainer    (1000)       54 2023-04-14 16:02:32.000000 postleid-0.7.0/src/postleid.egg-info/requires.txt
+-rw-r--r--   0 rainer    (1000) rainer    (1000)        9 2023-04-14 16:02:32.000000 postleid-0.7.0/src/postleid.egg-info/top_level.txt
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-14 16:02:32.752840 postleid-0.7.0/tests/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)    13336 2023-04-05 15:58:26.000000 postleid-0.7.0/tests/test_commons.py
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     3630 2023-04-05 15:58:26.000000 postleid-0.7.0/tests/test_rule_checks.py
```

### Comparing `postleid-0.6.5/LICENSE` & `postleid-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `postleid-0.6.5/pyproject.toml` & `postleid-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `postleid-0.6.5/src/postleid/__init__.py` & `postleid-0.7.0/src/postleid/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
 
-__version__ = "0.6.5"
+__version__ = "0.7.0"
 
 
 # vim: fileencoding=utf-8 sw=4 ts=4 sts=4 expandtab autoindent syntax=python:
```

### Comparing `postleid-0.6.5/src/postleid/commons.py` & `postleid-0.7.0/src/postleid/commons.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import bisect
 import dataclasses
 import logging
 import textwrap
 
 from collections import Counter
 
-from typing import Any, List, Tuple, Union
+from typing import Any, Iterator, List, Tuple, Union
 
 import yaml
 
 # local imports
 from postleid import paths
 from postleid import presets
 
@@ -119,14 +119,23 @@
 def separator_line(
     element: str = "–", width: int = presets.LOG_MESSAGE_MAX_WIDTH
 ) -> str:
     """Return a separator line"""
     return element * width
 
 
+def dump_yaml(data_structure: Any, sort_keys: bool = False) -> Iterator[str]:
+    """Return an iterator over the lines of a yaml dump"""
+    for line in yaml.safe_dump(
+        data_structure, indent=2, default_flow_style=False, sort_keys=sort_keys
+    ).splitlines():
+        yield line
+    #
+
+
 def evaluate_results(statistics: List[str]) -> Tuple[bool, bool]:
     """Evaluate results, show a summary,
     and return two flags: "everything is fine" and "data changed"
     """
     statistics.sort()
     results = Counter(statistics)
     data_changed = bool(results[S_FIXED])
```

### Comparing `postleid-0.6.5/src/postleid/data/default_user_settings.yaml` & `postleid-0.7.0/src/postleid/data/default_user_settings.yaml`

 * *Files identical despite different names*

### Comparing `postleid-0.6.5/src/postleid/data/postal_code_rules_by_cc.yaml` & `postleid-0.7.0/src/postleid/data/postal_code_rules_by_cc.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 #
 # postleid is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the LICENSE file for more details.
 #
 # The rules are adapted from
-# <https://github.com/zauberware/postal-codes-json-xml-csv>,
 # <https://en.wikipedia.org/wiki/List_of_postal_codes>,
-# <https://en.youbianku.com/>
+# <https://en.youbianku.com/> (where not outdated)
 # and linked pages/websites
 #
 ad:
   comment: Andorra
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Andorra"
   compound:
@@ -35,14 +34,16 @@
   compound:
   - pattern: nn
     min: 10
     max: 43
   - pattern: nn
 ai:
   comment: Anguilla
+  urls:
+  - "https://en.youbianku.com/Anguilla"
   compound:
   - pattern: cc
   - literal: "-2640"
 al:
   comment: Albania
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Albania"
@@ -76,17 +77,18 @@
     - pattern: a
       except: [I, O]
     - pattern: n
       min: 1
     - pattern: nnn
     - pattern: aaa
 as:
-  comment: American Samoa (part of US system)
+  comment: American Samoa
+  part_of_system: US
   urls:
-  - "https://en.wikipedia.org/wiki/Postal_codes_in_Oceania"
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Oceania#American_states,_territories,_and_states_of_association"
   variants:
   - compound:
     - literal: "96799-"
     - pattern: nnnn
   - literal: "96799"
 at:
   comment: Austria
@@ -101,15 +103,16 @@
   urls:
   - "https://en.wikipedia.org/wiki/Postcodes_in_Australia"
   compound:
   - pattern: nn
     min: 2
   - pattern: nn
 ax:
-  comment: Åland (part of Finnish system)
+  comment: Åland
+  part_of_system: Finland
   compound:
   - pattern: cc
   - literal: "-22"
   - pattern: nnn
 az:
   comment: Azerbaijan
   urls:
@@ -119,14 +122,16 @@
   - literal: " "
   - pattern: nn
     min: 1
     max: 69
   - pattern: nn
 ba:
   comment: Bosnia and Herzegovina
+  urls:
+  - "https://en.youbianku.com/Bosnia_and_Herzegovina"
   pattern: nnnnn
 bb:
   comment: Barbados
   urls:
   - "https://en.wikipedia.org/wiki/Barbados_Postal_Service#Postal_codes"
   compound:
   - pattern: cc
@@ -153,18 +158,26 @@
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Bulgaria"
   compound:
   - pattern: n
     min: 1
   - pattern: nnn
 bh:
   comment: Bahrain
+  urls:
+  - "https://en.youbianku.com/Bahrain"
   pattern: nnnn
   min: 101
   max: 1216
   remove_leading_zeroes: yes
+bl:
+  comment: Saint-Bathélemy
+  part_of_system: France
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
+  literal: "97133"
 bm:
   comment: Bermuda
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Bermuda"
   variants:
   - compound:
     - pattern: aa
@@ -196,14 +209,17 @@
 bt:
   comment: Bhutan
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Bhutan"
   pattern: nnnnn
 by:
   comment: Belarus
+  urls:
+  - "https://en.youbianku.com/Belarus"
+  part_of_system: inherited from former Soviet Union
   pattern: nnnnnn
 ca:
   comment: Canada
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Canada"
   compound:
   - pattern: a
@@ -213,15 +229,18 @@
     except: [D, F, I, O, Q, U]
   - literal: " "
   - pattern: n
   - pattern: a
     except: [D, F, I, O, Q, U]
   - pattern: n
 cc:
-  comment: Cocos (Keeling) Island (part of Australian system)
+  comment: Cocos (Keeling) Islands
+  part_of_system: Australia
+  urls:
+  - "https://en.youbianku.com/Cocos_(Keeling)_Islands"
   pattern: nnnn
 ch:
   comment: Switzerland
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Switzerland_and_Liechtenstein"
   compound:
   - pattern: n
@@ -273,35 +292,43 @@
       min: 1
       max: 7
     - pattern: nnnn
     - literal: "-"
     - pattern: nnnn
 cu:
   comment: Cuba
+  urls:
+  - "https://en.youbianku.com/Cuba"
   variants:
   - pattern: nnnnn
   - compound:
     - literal: "CP "
     - pattern: nnnnn
 cv:
   comment: Cape Verde
+  urls:
+  - "https://en.youbianku.com/Cape_Verde"
   pattern: nnnn
 cx:
   comment: Christmas Island
+  part_of_system: Australia
+  urls:
+  - "https://en.youbianku.com/Christmas_Island"
   pattern: nnnn
 cy:
   comment: Cyprus
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Cyprus"
   compound:
   - pattern: n
     min: 1
   - pattern: nnn
 cz:
-  comment: Czech Republic (common system with Slovakia)
+  comment: Czech Republic
+  part_of_system: CZ/SK
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_the_Czech_Republic"
   compound:
   - pattern: n
     min: 1
     max: 7
   - pattern: nn
@@ -322,14 +349,16 @@
   - pattern: nnnn
   - compound:
     - pattern: cc
     - literal: "-"
     - pattern: nnnn
 do:
   comment: Dominican Republic
+  urls:
+  - "https://en.youbianku.com/Dominican_Republic"
   pattern: nnnnn
 dz:
   comment: Algeria
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Algeria"
   - "https://en.wikipedia.org/wiki/ISO_3166-2:DZ"
   compound:
@@ -344,31 +373,51 @@
   compound:
   - pattern: nn
     min: 1
     max: 24
   - pattern: nnnn
 ee:
   comment: Estonia
+  urls:
+  - "https://en.youbianku.com/Estonia"
   pattern: nnnnn
 eg:
   comment: Egypt
+  urls:
+  - "https://en.youbianku.com/Egypt"
   pattern: nnnnn
+es:
+  comment: Spain
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Spain"
+  compound:
+  - pattern: nn
+    min: 1
+    max: 52
+  - pattern: nnn
 et:
   comment: Ethiopia
+  urls:
+  - "https://en.youbianku.com/Ethiopia"
   pattern: nnnn
 fi:
   comment: Finland
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Finland"
   pattern: nnnnn
 fk:
   comment: Falkland Islands
+  urls:
+  - "https://en.youbianku.com/Falkland_Islands"
   literal: "FIQQ 1ZZ"
 fm:
-  comment: Micronesia (part of US system)
+  comment: Micronesia
+  part_of_system: US
+  urls:
+  - "https://en.youbianku.com/Micronesia"
   variants:
   - compound:
     - pattern: nnnnn
       min: 96941
       max: 96944
     - literal: "-"
     - pattern: nnnn
@@ -400,25 +449,29 @@
   - pattern: n
   - pattern: "[a/n]"
     except: [C, I, K, M, O, V]
   - literal: " "
   - pattern: naa
 ge:
   comment: Georgia
+  urls:
+  - "https://en.youbianku.com/Georgia"
   pattern: nnnn
 gf:
   comment: French Guiana
+  part_of_system: France
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
   compound:
     - literal: "973"
     - pattern: nn
       max: 90
 gg:
-  comment: Guernsey (part of UK system)
+  comment: Guernsey
+  part_of_system: UK
   urls:
   - "https://en.wikipedia.org/wiki/GY_postcode_area"
   compound:
   - literal: "GY"
   - pattern: nn
     min: 1
     max: 10
@@ -442,26 +495,30 @@
     - pattern: nnnnn
 gi:
   comment: Gibraltar
   urls:
   - "https://en.wikipedia.org/wiki/Postal_addresses_in_Gibraltar"
   literal: "GX11 1AA"
 gl:
-  comment: Greenland (part of Danish system)
+  comment: Greenland
+  part_of_system: Denmark
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Greenland"
   compound:
   - pattern: cc
   - literal: "-39"
   - pattern: nn
 gn:
   comment: Guinea
+  urls:
+  - "https://en.youbianku.com/Guinea"
   pattern: nnn
 gp:
   comment: Guadeloupe
+  part_of_system: France
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
   compound:
     - literal: "971"
     - pattern: nn
       max: 90
 gr:
@@ -470,25 +527,34 @@
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Greece"
   compound:
   - pattern: nnn
     min: 100
     max: 899
   - literal: " "
   - pattern: nn
+gs:
+  comment: South Georgia and the South Sandwich Islands
+  urls:
+  - "https://en.youbianku.com/South_Georgia_and_the_South_Sandwich_Islands"
+  literal: "SIQQ 1ZZ"
 gt:
   comment: Guatemala
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Guatemala"
   - "https://en.wikipedia.org/wiki/Departments_of_Guatemala"
+  compound:
   - pattern: nn
     min: 1
     max: 22
   - pattern: nnn
 gu:
-  comment: Guam (part of US system)
+  comment: Guam
+  part_of_system: US
+  urls:
+  - "https://en.youbianku.com/Guam"
   variants:
   - compound:
     - literal: "969"
     - pattern: nn
       min: 10
       max: 32
   - compound:
@@ -496,37 +562,40 @@
     - pattern: nn
       min: 10
       max: 32
     - literal: "-"
     - pattern: nnnn
 gw:
   comment: Guinea-Bissau
+  urls:
+  - "https://en.youbianku.com/Guinea-Bissau"
   pattern: nnnn
 hn:
   comment: Honduras
   urls:
-  - "https://www.grcdi.nl/gsb/honduras.html"
   - "https://en.youbianku.com/honduras"
   variants:
+  - pattern: nnnnn
   - compound:
     - pattern: aa
     - pattern: nnnn
     deprecated: probably to avoid confusion of the department with an ISO-3166 code
-  - pattern: nnnnn
 hr:
   comment: Croatia
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Croatia"
   compound:
   - pattern: nn
     min: 10
     max: 53
   - pattern: nnn
 ht:
   comment: Haiti
+  urls:
+  - "https://en.youbianku.com/Haiti"
   pattern: nnnn
 hu:
   comment: Hungary
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Hungary"
   compound:
   - pattern: n
@@ -540,30 +609,30 @@
   - pattern: nn
     min: 10
   - pattern: nnn
 ie:
   comment: Ireland
   urls:
   - "https://en.wikipedia.org/wiki/Postal_addresses_in_the_Republic_of_Ireland"
-  - "https://en.youbianku.com/Ireland"
   compound:
   - pattern: a
     except: [B, G, I, J, L, M, O, Q, S, U, Z]
   - pattern: n
   - pattern: "?"
     except: [B, G, I, J, L, M, O, Q, S, U, Z]
   - literal: " "
   - pattern: ????
 il:
   comment: Israel
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Israel"
   pattern: nnnnnnn
 im:
-  comment: Isle of Man (part of UK system)
+  comment: Isle of Man
+  part_of_system: UK
   urls:
   - "https://en.wikipedia.org/wiki/IM_postcode_area"
   compound:
   - pattern: cc
   - pattern: nn
     remove_leading_zeroes: yes
   - literal: " "
@@ -582,29 +651,29 @@
     - pattern: nn
       min: 11
     - pattern: n
     - literal: " "
     - pattern: nnn
 io:
   comment: British Indian Ocean Territory
+  urls:
+  - "https://en.youbianku.com/British_Indian_Ocean_Territory"
   literal: "BBND 1ZZ"
 iq:
   comment: Iraq
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Iraq"
-  - "https://en.youbianku.com/Iraq"
   compound:
   - pattern: nn
     min: 10
   - pattern: nnn
 ir:
   comment: Iran
   urls:
   - "https://en.wikipedia.org/wiki/Identity_documents_in_Iran#Postal_code_in_Iran"
-  - "https://en.youbianku.com/Iran"
   variants:
   - compound:
     - pattern: nnnnn
     - literal: "-"
     - pattern: nnnnn
   - compound:
     - pattern: nnnnn
@@ -616,89 +685,139 @@
   pattern: nnn
 it:
   comment: Italy
   urls:
   - "https://en.wikipedia.org/wiki/Codice_di_avviamento_postale"
   pattern: nnnnn
 je:
-  comment: Jersey (part of UK system)
+  comment: Jersey
+  part_of_system: UK
   urls:
   - "https://en.wikipedia.org/wiki/JE_postcode_area"
   compound:
   - literal: cc
   - pattern: nn
     remove_leading_zeroes: yes
   - literal: " "
   - pattern: n
   - pattern: aa
 jo:
   comment: Jordan
+  urls:
+  - "https://en.youbianku.com/Jordan"
   pattern: nnnnn
 jp:
   comment: Japan
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Japan"
   compound:
   - pattern: nnn
     literal: "-"
   - pattern: nnnn
 ke:
   comment: Kenya
+  urls:
+  - "https://en.youbianku.com/Kenya"
   pattern: nnnnn
 kg:
   comment: Kyrgyzstan
+  urls:
+  - "https://en.youbianku.com/Kyrgyzstan"
   pattern: nnnnnn
 kh:
   comment: Cambodia
+  urls:
+  - "https://en.youbianku.com/Cambodia"
   pattern: nnnnnn
+kn:
+  comment: Saint Kitts and Nevis
+  urls:
+  - "https://en.youbianku.com/Saint_Kitts_and_Nevis"
+  compound:
+  - pattern: cc
+  - pattern: nnnn
 kr:
   comment: South Korea
+  urls:
+  - "https://en.youbianku.com/Republic_of_Korea"
   pattern: nnnnn
 kw:
   comment: Kuwait
+  urls:
+  - "https://en.youbianku.com/Kuwait"
   pattern: nnnnn
 ky:
   comment: Cayman Islands
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_the_Cayman_Islands"
   compound:
   - pattern: cc
   - pattern: n
     min: 1
     max: 3
   - literal: "-"
   - pattern: nnnn
 kz:
   comment: Kazakhstan
+  urls:
+  - "https://en.youbianku.com/Kazakhstan"
   pattern: nnnnnn
 la:
   comment: Laos
+  urls:
+  - "https://en.youbianku.com/Laos"
   pattern: nnnnn
 lb:
   comment: Lebanon
+  urls:
+  - "https://en.youbianku.com/Lebanon"
   variants:
   - compound:
     - pattern: nnnn
     - literal: " "
     - pattern: nnnn
   - pattern: nnnn
+lc:
+  comment: Saint Lucia
+  variants:
+  - compound:
+    - pattern: cc
+    - pattern: nn
+    - literal: "  "
+    - pattern: nnn
+  - compound:
+    - pattern: cc
+    - pattern: nn
+    - literal: " "
+    - pattern: nnn
+    comment: compatibility variant using a single-space separator
 li:
-  comment: Liechtenstein (part of Swiss system)
+  comment: Liechtenstein
+  part_of_system: Switzerland
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Liechtenstein"
   compound:
   - pattern: nnn
     min: 948
     max: 949
   - pattern: n
+lk:
+  comment: Sri Lanka
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Sri_Lanka"
+  pattern: nnnnn
 lr:
   comment: Liberia
+  urls:
+  - "https://en.youbianku.com/Liberia"
   pattern : nnnn
 ls:
   comment: Lesotho
+  urls:
+  - "https://en.youbianku.com/Lesotho"
   pattern : nnn
 lt:
   comment: Lithuania
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Lithuania"
   compound:
   - pattern: cc
@@ -720,15 +839,16 @@
   - pattern: nnnn
 ma:
   comment: Morocco
   urls:
   - "https://en.youbianku.com/Morocco"
   pattern: nnnnn
 mc:
-  comment: Monaco (part of French system)
+  comment: Monaco
+  part_of_system: France
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_France#Monaco"
   compound:
   - literal: "980"
   - pattern: nn
 md:
   comment: Moldova
@@ -739,19 +859,30 @@
   - literal: "-"
   - pattern: nnnn
 me:
   comment: Montenegro
   urls:
   - "https://en.youbianku.com/Montenegro"
   pattern: nnnnn
+mf:
+  comment: Saint-Martin
+  part_of_system: France
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
+  literal: "97150"
 mg:
   comment: Madagascar
+  urls:
+  - "https://en.youbianku.com/Madagascar"
   pattern: nnn
 mh:
-  comment: Marshall Islands (part of US system)
+  comment: Marshall Islands
+  part_of_system: US
+  urls:
+  - "https://en.youbianku.com/Marshall_Islands"
   variants:
   - compound:
     - pattern: nnnnn
       min: 96960
       max: 96970
     - literal: "-"
     - pattern: nnnn
@@ -774,27 +905,31 @@
   - pattern: nnn
 mn:
   comment: Mongolia
   urls:
   - "https://en.youbianku.com/Mongolia"
   pattern: nnnnn
 mp:
-  comment: Northern Marianas (part of US system)
+  comment: Northern Marianas
+  part_of_system: US
+  urls:
+  - "https://en.youbianku.com/Northern_Mariana_Islands"
   variants:
   - compound:
     - pattern: nnnnn
       min: 96950
       max: 96952
     - literal: "-"
     - pattern: nnnn
   - pattern: nnnnn
     min: 96950
     max: 96952
 mq:
   comment: Martinique
+  part_of_system: France
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
   compound:
   - literal: "972"
   - pattern: nn
     max: 90
 ms:
@@ -826,14 +961,16 @@
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Mauritius"
   compound:
   - pattern: "?"
     only: ["1", "2", "3", "4", "5", "6", "7", "8", "9", "A", "R"]
   - pattern: nnnn
 mv:
   comment: Maldives
+  urls:
+  - "https://en.youbianku.com/Maldives"
   pattern: nnnnn
 mw:
   comment: Malawi
   pattern: nnnnnn
 mx:
   comment: Mexico
   urls:
@@ -852,27 +989,29 @@
 na:
   comment: Namibia
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Namibia"
   pattern: nnnnn
 nc:
   comment: New Caledonia
+  part_of_system: France
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
   compound:
   - literal: "988"
   - pattern: nn
     max: 90
 ne:
   comment: Niger
   urls:
   - "https://en.youbianku.com/Niger"
   pattern: nnnn
 nf:
-  comment: Norfolk Island (part of Australian system)
+  comment: Norfolk Island
+  part_of_system: Australia
   urls:
   - "https://en.youbianku.com/Norfolk_Island"
   pattern: nnnn
 ng:
   comment: Nigeria
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Nigeria"
@@ -911,75 +1050,446 @@
   - "https://en.wikipedia.org/wiki/Postcodes_in_New_Zealand"
   pattern: nnnn
 om:
   comment:  Oman
   urls:
   - "https://en.youbianku.com/Oman"
   pattern: nnn
+pa:
+  comment: Panama
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Panama"
+  pattern: nnnn
+pe:
+  comment: Peru
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Peru"
+  pattern: nnnnn
 pf:
   comment: French Polynesia
+  part_of_system: France
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Oceania#French_overseas_territories"
   compound:
   - literal: "987"
   - pattern: nn
     max: 90
+pg:
+  comment: Papua New Guinea
+  urls:
+  - "https://en.youbianku.com/Papua_New_Guinea"
+  pattern: nnn
+ph:
+  comment: Philippines
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Philippines"
+  pattern: nnnn
+pk:
+  comment: Pakistan
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Pakistan"
+  pattern: nnnnn
 pl:
   comment: Poland
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Poland"
   compound:
   - pattern: nn
   - literal: "-"
   - pattern: nnn
+pm:
+  comment: Saint-Pierre and Miquelon
+  part_of_system: France
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
+  literal: "97500"
+pn:
+  comment: Pitcairn Islands
+  literal: "PCRN 1ZZ"
+pr:
+  comment: Puerto Rico
+  part_of_system: US
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Puerto_Rico"
+  variants:
+  - compound:
+    - pattern: nnn
+      only: ["006", "007", "009"]
+    - pattern: nn
+    - literal: "-"
+    - pattern: nnnn
+  -compound:
+    - pattern: nnn
+      only: ["006", "007", "009"]
+    - pattern: nn
+ps:
+  comment: Palestine
+  pattern: nnn
 pt:
   comment: Portugal
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Portugal"
   compound:
   - pattern: nnnn
     min: 1000
   - literal: "-"
   - pattern: nnn
+pw:
+  comment: Palau
+  part_of_system: US
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Oceania#American_states,_territories,_and_states_of_association"
+  variants:
+  - compound:
+    - pattern: nnnnn
+      min: 96939
+      max: 96940
+    - literal: "-"
+    - pattern: nnnn
+  - pattern: nnnnn
+    min: 96939
+    max: 96940
+py:
+  comment: Paraguay
+  pattern: nnnn
+re:
+  comment: Réunion
+  part_of_system: France
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
+  compound:
+  - literal: "974"
+  - pattern: nn
+    max: 90
+ro:
+  comment: Romania
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Romania"
+  - "https://en.wikipedia.org/wiki/Counties_of_Romania"
+  compound:
+  - pattern: nn
+    min: 1
+    max: 92
+  - pattern: nnnn
+rs:
+  comment: Serbia
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Serbia"
+  pattern: nnnnnn
+ru:
+  comment: Russia
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Russia"
+  pattern: nnnnnn
+sa:
+  comment: Saudi Arabia
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Saudi_Arabia"
+  variants:
+  - compound:
+    - pattern: nnnnn
+    - literal: "-"
+    - pattern: nnnn
+  - pattern: nnnnn
+sd:
+  comment: Sudan
+  urls:
+  - "https://en.youbianku.com/Sudan"
+  pattern: nnnnn
+se:
+  comment: Sweden
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Sweden"
+  compound:
+  - pattern: nnn
+    min: 100
+    max: 984
+  - literal: " "
+  - pattern: nn
+sg:
+  comment: Singapore
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Singapore"
+  pattern: nnnnnn
+sh:
+  comment: Saint Helena, Ascension and Tristan da Cunha
+  urls:
+  - "https://en.youbianku.com/Saint_Helena"
+  compound:
+  - pattern: aaaa
+    only: [STHL, ASCN, TDCU]
+  - literal: " 1ZZ"
+si:
+  comment: Slovenia
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Slovenia"
+  variants:
+  - compound:
+    - pattern: cc
+    - literal: "-"
+    - pattern: n
+      min: 1
+    - pattern: nnn
+  - compound:
+    - pattern: n
+      min: 1
+    - pattern: nnn
+sj:
+  comment: Svalbard and Jan Mayen
+  part_of_system: Norway
+  urls:
+  - "https://en.wikipedia.org/wiki/Svalbard_and_Jan_Mayen"
+  pattern: nnnn
+sk:
+  comment: Slovakia
+  part_of_system: CZ/SK
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Slovakia"
+  compound:
+  - pattern: n
+    only: ["8", "9", "0"]
+  - pattern: nn
+  - literal: " "
+  - pattern: nn
+sm:
+  comment: San Marino
+  part_of_system: Italy
+  urls:
+  - "https://en.wikipedia.org/wiki/Codice_di_avviamento_postale"
+  compound:
+  - literal: "4789"
+  - pattern: n
+sn:
+  comment: Senegal
+  urls:
+  - "https://en.youbianku.com/Senegal"
+  variants:
+  - pattern: nnnnn
+  - compound:
+    - literal: "CP "
+    - pattern: nnnnn
+  - compound:
+    - literal: "C.P. "
+    - pattern: nnnnn
+so:
+  comment: Somalia
+  compound:
+  - pattern: aa
+  - literal: " "
+  - pattern: nnnnn
 sv:
   comment: El Salvador
-  pattern: nnnn
+  urls:
+  - "https://en.youbianku.com/El_Salvador"
+  variants:
+  - pattern: nnnn
+  - compound:
+    - literal: "CP "
+    - pattern: nnnn
 sz:
   comment: Eswatini
+  urls:
+  - "https://en.youbianku.com/Swaziland"
   compound:
   - pattern: a
     only: [H, M, S, L]
   - pattern: nnn
+tc:
+  comment: Turks and Caicos Islands
+  urls:
+  - "https://en.youbianku.com/Turks_and_Caicos_Islands"
+  literal: "TKCA 1ZZ"
+th:
+  comment: Thailand
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Thailand"
+  compound:
+  - pattern: nn
+    min: 10
+  - pattern: nnn
+tj:
+  comment: Tajikistan
+  urls:
+  - "https://en.youbianku.com/Tajikistan"
+  part_of_system: inherited from former Soviet Union
+  pattern: nnnnnn
+tm:
+  comment: Turkmenistan
+  urls:
+  - "https://en.youbianku.com/Turkmenistan"
+  part_of_system: inherited from former Soviet Union
+  pattern: nnnnnn
+tr:
+  comment: Turkey
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Turkey"
+  compound:
+  - pattern: nn
+    min: 1
+  - pattern: nnn
+tt:
+  comment: Trinidad and Tobago
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Trinidad_and_Tobago"
+  compound:
+  - pattern: nn
+    min: 10
+  - pattern: nnnn
+tu:
+  comment: Tunisia
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Tunisia"
+  compound:
+  - pattern: nn
+    min: 10
+  - pattern: nn
+tw:
+  comment: Taiwan
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Taiwan"
+  variants:
+  - pattern: nnn
+    min: 100
+  - compound:
+    - pattern: nnn
+      min: 100
+    - literal: "-"
+    - pattern: nn
+  - compound:
+    - pattern: nnn
+      min: 100
+    - literal: "-"
+    - pattern: nnn
+tz:
+  comment: Tanzania
+  urls:
+  - "https://en.youbianku.com/Tanzania"
+  pattern: nnnnn
+ua:
+  comment: Ukraine
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Ukraine"
+  compound:
+  - pattern: nn
+    min: 1
+  - pattern: nnn
+um:
+  comment: United States Minor Outlying Islands
+  part_of_system: US
+  literal: "96898"
 us:
   comment: United States
   urls:
   - "https://en.wikipedia.org/wiki/ZIP_Code"
   variants:
   - compound:
     - pattern: nnnnn
     - literal: "-"
     - pattern: nnnn
   - pattern: nnnnn
+uy:
+  comment: Uruguay
+  urls:
+  - "https://en.youbianku.com/Uruguay"
+  pattern: nnnnn
+uz:
+  comment: Uzbekistan
+  urls:
+  - "https://en.youbianku.com/Uzbekistan"
+  pattern: nnnnnn
+va:
+  comment: Vatican City
+  part_of_system: Italy
+  urls:
+  - "https://en.wikipedia.org/wiki/Codice_di_avviamento_postale"
+  literal: "00120"
+vc:
+  comment: Saint Vincent and the Grenadines
+  urls:
+  - "https://en.youbianku.com/Saint_Vincent_and_the_Grenadines"
+  compound:
+  - pattern: cc
+  - pattern: nnnn
+ve:
+  comment: Venezuela
+  urls:
+  - "https://en.youbianku.com/Venezuela"
+  variants:
+  - compound:
+    - pattern: nnnn
+    - literal: "-"
+    - pattern: a
+  - pattern: nnnn
 vg:
   comment: British Virgin Islands
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_the_British_Virgin_Islands"
   compound:
   - pattern: cc
   - pattern: nnn
     min: 111
     max: 116
   - pattern: n
+vi:
+  comment: United States Virgin Islands
+  part_of_system: US
+  urls:
+  - "https://en.youbianku.com/United_States_Virgin_Islands"
+  variants:
+  - compound:
+    - pattern: nnnnn
+      min: 801
+      max: 851
+    - literal: "-"
+    - pattern: nnnn
+  - pattern: nnnnn
+    min: 801
+    max: 851
+vn:
+  comment: Vietnam
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Vietnam"
+  compound:
+  - pattern: nn
+    min: 10
+  - pattern: nnn
+wf:
+  comment: Wallis and Futuna
+  part_of_system: France
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
+  compound:
+    - literal: "986"
+    - pattern: nn
+      max: 90
+ws:
+  comment: Samoa
+  urls:
+  - "https://en.youbianku.com/Samoa"
+  compound:
+  - pattern: cc
+  - pattern: nnnn
 xk:
   comment: Kosovo
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Kosovo"
   pattern: nnnnn
   min: 10000
 yt:
   comment: Mayotte
+  part_of_system: France
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
   compound:
   - literal: "976"
   - pattern: nn
     max: 90
+za:
+  comment: South Africa
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_South_Africa"
+  pattern: nnnn
+zm:
+  comment: Zambia
+  urls:
+  - "https://en.youbianku.com/Zambia"
+  pattern: nnnnn
```

### Comparing `postleid-0.6.5/src/postleid/fix_excel_files.py` & `postleid-0.7.0/src/postleid/fix_excel_files.py`

 * *Files identical despite different names*

### Comparing `postleid-0.6.5/src/postleid/locale/de/LC_MESSAGES/argparse.mo` & `postleid-0.7.0/src/postleid/locale/de/LC_MESSAGES/argparse.mo`

 * *Files identical despite different names*

### Comparing `postleid-0.6.5/src/postleid/paths.py` & `postleid-0.7.0/src/postleid/paths.py`

 * *Files identical despite different names*

### Comparing `postleid-0.6.5/src/postleid/presets.py` & `postleid-0.7.0/src/postleid/presets.py`

 * *Files identical despite different names*

### Comparing `postleid-0.6.5/src/postleid/rule_checks.py` & `postleid-0.7.0/src/postleid/rule_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         minimum: Optional[int] = None
         maximum: Optional[int] = None
         remove_leading_zeroes = False
         if "literal" in rules:
             literal = str(rules["literal"])
             only.append(literal)
             self.pattern = literal
-            self.__regex = "." * len(literal)
+            self.__regex = re.escape(literal)
             self.all_numeric = self.prx_all_numeric_literal.match(literal)
         else:
             self.pattern = rules["pattern"]
             if self.pattern == "cc":
                 self.__regex = re.escape(country_code.upper())
             else:
                 self.__regex = self.__translate_pattern(self.pattern)
@@ -263,14 +263,19 @@
         self.__all_numeric = all(part.all_numeric for part in self)
 
     @property
     def full_pattern(self) -> str:
         """Return the full pattern"""
         return self.__full_pattern
 
+    @property
+    def full_prx(self) -> re.Pattern:
+        """Return the compiled full pattern"""
+        return self.__full_prx
+
     def __getitem__(self, index: int) -> PatternComponent:
         """Return pattern component at index"""
         return self.__components[index]
 
     def __iter__(self) -> Iterator[PatternComponent]:
         """Return an iterator over the pattern components"""
         return iter(self.__components)
```

### Comparing `postleid-0.6.5/src/postleid.egg-info/SOURCES.txt` & `postleid-0.7.0/src/postleid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `postleid-0.6.5/tests/test_commons.py` & `postleid-0.7.0/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `postleid-0.6.5/tests/test_rule_checks.py` & `postleid-0.7.0/tests/test_rule_checks.py`

 * *Files identical despite different names*

