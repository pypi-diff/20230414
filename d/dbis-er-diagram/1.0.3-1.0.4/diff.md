# Comparing `tmp/dbis-er-diagram-1.0.3.tar.gz` & `tmp/dbis-er-diagram-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-er-diagram-1.0.3.tar", last modified: Fri Apr  7 08:38:50 2023, max compression
+gzip compressed data, was "dbis-er-diagram-1.0.4.tar", last modified: Fri Apr 14 08:19:34 2023, max compression
```

## Comparing `dbis-er-diagram-1.0.3.tar` & `dbis-er-diagram-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-07 08:38:50.861687 dbis-er-diagram-1.0.3/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-04-07 08:08:01.000000 dbis-er-diagram-1.0.3/LICENSE
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-04-07 08:38:50.861687 dbis-er-diagram-1.0.3/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15133 2023-04-07 08:08:01.000000 dbis-er-diagram-1.0.3/README.md
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-07 08:38:50.859687 dbis-er-diagram-1.0.3/dbis_er_diagram.egg-info/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-04-07 08:38:50.000000 dbis-er-diagram-1.0.3/dbis_er_diagram.egg-info/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      529 2023-04-07 08:38:50.000000 dbis-er-diagram-1.0.3/dbis_er_diagram.egg-info/SOURCES.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-04-07 08:38:50.000000 dbis-er-diagram-1.0.3/dbis_er_diagram.egg-info/dependency_links.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       48 2023-04-07 08:38:50.000000 dbis-er-diagram-1.0.3/dbis_er_diagram.egg-info/requires.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       10 2023-04-07 08:38:50.000000 dbis-er-diagram-1.0.3/dbis_er_diagram.egg-info/top_level.txt
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-07 08:38:50.860687 dbis-er-diagram-1.0.3/erdiagram/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      246 2023-04-07 08:08:01.000000 dbis-er-diagram-1.0.3/erdiagram/__init__.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7697 2023-04-07 08:08:01.000000 dbis-er-diagram-1.0.3/erdiagram/drawing.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    38914 2023-04-07 08:08:01.000000 dbis-er-diagram-1.0.3/erdiagram/er.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    27610 2023-04-07 08:38:37.000000 dbis-er-diagram-1.0.3/erdiagram/grading.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6591 2023-04-07 08:08:01.000000 dbis-er-diagram-1.0.3/erdiagram/merging.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      306 2023-04-07 08:08:01.000000 dbis-er-diagram-1.0.3/erdiagram/node_type.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      881 2023-04-07 08:38:37.000000 dbis-er-diagram-1.0.3/pyproject.toml
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-04-07 08:38:50.861687 dbis-er-diagram-1.0.3/setup.cfg
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-07 08:38:50.861687 dbis-er-diagram-1.0.3/tests/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     5117 2023-04-07 08:08:01.000000 dbis-er-diagram-1.0.3/tests/test_adders.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1728 2023-04-07 08:08:01.000000 dbis-er-diagram-1.0.3/tests/test_drawing.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11855 2023-04-07 08:08:01.000000 dbis-er-diagram-1.0.3/tests/test_getters.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1916 2023-04-07 08:08:01.000000 dbis-er-diagram-1.0.3/tests/test_grading_components.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     5802 2023-04-07 08:38:37.000000 dbis-er-diagram-1.0.3/tests/test_grading_diagrams.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1148 2023-04-07 08:08:01.000000 dbis-er-diagram-1.0.3/tests/test_merging.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1035 2023-04-07 08:08:01.000000 dbis-er-diagram-1.0.3/tests/test_other_methods.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-14 08:19:34.764445 dbis-er-diagram-1.0.4/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/LICENSE
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-04-14 08:19:34.764445 dbis-er-diagram-1.0.4/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15133 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/README.md
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-14 08:19:34.763445 dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-04-14 08:19:34.000000 dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      529 2023-04-14 08:19:34.000000 dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/SOURCES.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-04-14 08:19:34.000000 dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/dependency_links.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       48 2023-04-14 08:19:34.000000 dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/requires.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       10 2023-04-14 08:19:34.000000 dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/top_level.txt
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-14 08:19:34.763445 dbis-er-diagram-1.0.4/erdiagram/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      246 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/erdiagram/__init__.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7697 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/erdiagram/drawing.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    38914 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/erdiagram/er.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    27657 2023-04-14 08:19:15.000000 dbis-er-diagram-1.0.4/erdiagram/grading.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6591 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/erdiagram/merging.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      306 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/erdiagram/node_type.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      881 2023-04-14 08:19:15.000000 dbis-er-diagram-1.0.4/pyproject.toml
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-04-14 08:19:34.764445 dbis-er-diagram-1.0.4/setup.cfg
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-14 08:19:34.764445 dbis-er-diagram-1.0.4/tests/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     5117 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/tests/test_adders.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1728 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/tests/test_drawing.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11855 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/tests/test_getters.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1916 2023-04-14 08:15:42.000000 dbis-er-diagram-1.0.4/tests/test_grading_components.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7118 2023-04-14 08:19:15.000000 dbis-er-diagram-1.0.4/tests/test_grading_diagrams.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1148 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/tests/test_merging.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1035 2023-04-14 08:01:51.000000 dbis-er-diagram-1.0.4/tests/test_other_methods.py
```

### Comparing `dbis-er-diagram-1.0.3/LICENSE` & `dbis-er-diagram-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.3/PKG-INFO` & `dbis-er-diagram-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-er-diagram
-Version: 1.0.3
+Version: 1.0.4
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Michal Slupczynski <slupczynski@dbis.rwth-aachen.de>, Beyza Akyüz <beyza.akyuez@rwth-aachen.de>, Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-er-diagram
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-er-diagram-1.0.3/README.md` & `dbis-er-diagram-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.3/dbis_er_diagram.egg-info/PKG-INFO` & `dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-er-diagram
-Version: 1.0.3
+Version: 1.0.4
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Michal Slupczynski <slupczynski@dbis.rwth-aachen.de>, Beyza Akyüz <beyza.akyuez@rwth-aachen.de>, Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-er-diagram
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-er-diagram-1.0.3/dbis_er_diagram.egg-info/SOURCES.txt` & `dbis-er-diagram-1.0.4/dbis_er_diagram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.3/erdiagram/drawing.py` & `dbis-er-diagram-1.0.4/erdiagram/drawing.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.3/erdiagram/er.py` & `dbis-er-diagram-1.0.4/erdiagram/er.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.3/erdiagram/grading.py` & `dbis-er-diagram-1.0.4/erdiagram/grading.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,16 +464,16 @@
         )["label"]
         submission_sub_labels = [
             submission.get_entity_by_id(sub_id)["label"]
             for sub_id in submission_is_a[0]["subclass_ids"]
         ]
 
         set_ratio = setratio(
-            set([sanitize(label) for label in solution_sub_labels]),
-            set([sanitize(label) for label in submission_sub_labels]),
+            list(set([sanitize(label) for label in solution_sub_labels])),
+            list(set([sanitize(label) for label in submission_sub_labels])),
         )
 
         if set_ratio < ratio_threshold:
             s = scores["missing_is_a_property"] * len(solution_sub_labels) * set_ratio
             score += s
             log += f"\t✗ The is-a relation {solution_super_label} -> {solution_sub_labels} is not comparable to {submission_super_label} -> {submission_sub_labels} with a set ratio of {set_ratio:.2f}. ({s})\n"
 
@@ -613,15 +613,16 @@
         submission_composed_attribute_labels = [
             sanitize(submission.get_label_by_id(composed_attribute_id))
             for composed_attribute_id in submission_attribute[0][
                 "composed_of_attribute_ids"
             ]
         ]
         set_ratio = setratio(
-            solution_composed_attribute_labels, submission_composed_attribute_labels
+            list(set(solution_composed_attribute_labels)),
+            list(set(submission_composed_attribute_labels)),
         )
         if set_ratio < ratio_threshold:
             s = (
                 scores["missing_composed_attribute"]
                 * len(solution_attribute["composed_of_attribute_ids"])
                 * set_ratio
             )
```

### Comparing `dbis-er-diagram-1.0.3/erdiagram/merging.py` & `dbis-er-diagram-1.0.4/erdiagram/merging.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.3/pyproject.toml` & `dbis-er-diagram-1.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbis-er-diagram"
-version = "1.0.3"
+version = "1.0.4"
 description = "RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 authors = [
 	{ name = "Michal Slupczynski", email = "slupczynski@dbis.rwth-aachen.de" },
 	{ name = "Beyza Akyüz", email = "beyza.akyuez@rwth-aachen.de" },
 	{ name = "Til Mohr", email = "til.mohr@rwth-aachen.de" },
 ]
 readme = "README.md"
```

### Comparing `dbis-er-diagram-1.0.3/tests/test_adders.py` & `dbis-er-diagram-1.0.4/tests/test_adders.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.3/tests/test_drawing.py` & `dbis-er-diagram-1.0.4/tests/test_drawing.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.3/tests/test_getters.py` & `dbis-er-diagram-1.0.4/tests/test_getters.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.3/tests/test_grading_components.py` & `dbis-er-diagram-1.0.4/tests/test_grading_components.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.3/tests/test_grading_diagrams.py` & `dbis-er-diagram-1.0.4/tests/test_grading_diagrams.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,57 @@
 import pytest
 
 from erdiagram import ER, grade_submission
 
 
+def test_had_issue():
+    solution = ER()
+    solution.add_relation(
+        {"Freizeitpark": "1"},
+        "angestellt",
+        {"Mitarbeiter": "n"},
+    )
+    solution.add_attribute("Mitarbeiter", "Gehalt")
+    solution.add_attribute("Mitarbeiter", "Geschlecht")
+    solution.add_attribute("Mitarbeiter", "PersonalNummer", is_pk=True)
+    solution.add_relation(
+        {"Mitarbeiter": "1"},
+        "verwaltet",
+        {"Mitarbeiter": "n"},
+    )
+    solution.add_is_a(
+        "Mitarbeiter",
+        ["Manager", "Mechaniker", "Animateur", "Kaufmann", "Koch"],
+        is_total=False,
+        is_disjunct=True,
+    )
+    submission = ER()
+    submission.add_relation(
+        {"Freizeitpark": "1"},
+        "angestellt",
+        {"Mitarbeiter": "n"},
+    )
+    submission.add_attribute("Mitarbeiter", "Gehalt")
+    submission.add_attribute("Mitarbeiter", "Geschlecht")
+    submission.add_attribute("Mitarbeiter", "PersonalNummer", is_pk=True)
+    submission.add_relation(
+        {"Mitarbeiter": "1"},
+        "verwaltet",
+        {"Mitarbeiter": "n"},
+    )
+    submission.add_is_a(
+        "Mitarbeiter",
+        ["Manager", "Mechaniker", "Animateur", "Kaufmann", "Koch"],
+        is_total=False,
+        is_disjunct=True,
+    )
+    score, log = grade_submission(solution, submission)
+    assert score == 0
+
+
 def test_exc_score_comparison():
     solution = ER()
     solution.add_entity("Hersteller")
     solution.add_attribute("Hersteller", "Name", is_pk=True)
     solution.add_attribute("Hersteller", "Sitz")  # 0.25 missing attribute
     solution.add_entity("Käse")  # 1p missing node
```

### Comparing `dbis-er-diagram-1.0.3/tests/test_merging.py` & `dbis-er-diagram-1.0.4/tests/test_merging.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.3/tests/test_other_methods.py` & `dbis-er-diagram-1.0.4/tests/test_other_methods.py`

 * *Files identical despite different names*

