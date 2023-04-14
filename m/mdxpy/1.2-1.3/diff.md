# Comparing `tmp/mdxpy-1.2.tar.gz` & `tmp/mdxpy-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdxpy-1.2.tar", last modified: Thu Jan 19 11:38:13 2023, max compression
+gzip compressed data, was "mdxpy-1.3.tar", last modified: Fri Apr 14 13:03:11 2023, max compression
```

## Comparing `mdxpy-1.2.tar` & `mdxpy-1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-01-19 11:38:13.789415 mdxpy-1.2/
--rw-rw-rw-   0        0        0       88 2020-05-07 19:15:45.000000 mdxpy-1.2/.gitignore
--rw-rw-rw-   0        0        0     1099 2020-04-25 16:07:06.000000 mdxpy-1.2/LICENSE
--rw-rw-rw-   0        0        0     9294 2023-01-19 11:38:13.788417 mdxpy-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-19 11:38:13.727580 mdxpy-1.2/images/
--rw-rw-rw-   0        0        0    65252 2020-05-07 21:01:00.000000 mdxpy-1.2/images/logo.png
-drwxrwxrwx   0        0        0        0 2023-01-19 11:38:13.752513 mdxpy-1.2/mdxpy/
--rw-rw-rw-   0        0        0      192 2022-10-09 19:46:22.000000 mdxpy-1.2/mdxpy/__init__.py
--rw-rw-rw-   0        0        0    48261 2022-12-06 16:57:53.000000 mdxpy-1.2/mdxpy/mdx.py
-drwxrwxrwx   0        0        0        0 2023-01-19 11:38:13.784428 mdxpy-1.2/mdxpy.egg-info/
--rw-rw-rw-   0        0        0     9294 2023-01-19 11:38:13.000000 mdxpy-1.2/mdxpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-01-19 11:38:13.000000 mdxpy-1.2/mdxpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-19 11:38:13.000000 mdxpy-1.2/mdxpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-01-19 11:38:13.000000 mdxpy-1.2/mdxpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-01-19 11:32:22.000000 mdxpy-1.2/pyproject.toml
--rw-rw-rw-   0        0        0     8260 2022-10-10 13:17:58.000000 mdxpy-1.2/readme.md
--rw-rw-rw-   0        0        0       42 2023-01-19 11:38:13.790412 mdxpy-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1334 2023-01-19 11:32:22.000000 mdxpy-1.2/setup.py
--rw-rw-rw-   0        0        0    44492 2022-12-06 16:57:53.000000 mdxpy-1.2/test.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:03:11.512216 mdxpy-1.3/
+-rw-rw-rw-   0        0        0       88 2020-05-07 19:15:45.000000 mdxpy-1.3/.gitignore
+-rw-rw-rw-   0        0        0     1099 2020-04-25 16:07:06.000000 mdxpy-1.3/LICENSE
+-rw-rw-rw-   0        0        0     9292 2023-04-14 13:03:11.512216 mdxpy-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-14 13:03:11.505698 mdxpy-1.3/images/
+-rw-rw-rw-   0        0        0    65252 2020-05-07 21:01:00.000000 mdxpy-1.3/images/logo.png
+drwxrwxrwx   0        0        0        0 2023-04-14 13:03:11.512216 mdxpy-1.3/mdxpy/
+-rw-rw-rw-   0        0        0      192 2022-10-09 19:46:22.000000 mdxpy-1.3/mdxpy/__init__.py
+-rw-rw-rw-   0        0        0    49610 2023-04-05 20:27:37.000000 mdxpy-1.3/mdxpy/mdx.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:03:11.512216 mdxpy-1.3/mdxpy.egg-info/
+-rw-rw-rw-   0        0        0     9292 2023-04-14 13:03:11.000000 mdxpy-1.3/mdxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-14 13:03:11.000000 mdxpy-1.3/mdxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:03:11.000000 mdxpy-1.3/mdxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-14 13:03:11.000000 mdxpy-1.3/mdxpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-01-19 11:32:22.000000 mdxpy-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0     8260 2022-10-10 13:17:58.000000 mdxpy-1.3/readme.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:03:11.512216 mdxpy-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1334 2023-04-04 20:28:04.000000 mdxpy-1.3/setup.py
+-rw-rw-rw-   0        0        0    47119 2023-04-05 20:31:29.000000 mdxpy-1.3/test.py
```

### Comparing `mdxpy-1.2/LICENSE` & `mdxpy-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mdxpy-1.2/PKG-INFO` & `mdxpy-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdxpy
-Version: 1.2
+Version: 1.3
 Summary: A simple, yet elegant MDX library for TM1
 Home-page: https://github.com/cubewise-code/mdxpy
 Maintainer: Marius Wirtz
 Maintainer-email: MWirtz@cubewise.com
 License: MIT-LICENSE
 Keywords: MDX,TM1,IBM Cognos TM1,Planning Analytics,PA,Cognos
 Platform: any
@@ -254,8 +254,7 @@
 ## Tests
 
 All tests in `test.py`
 
 ## Contribution
 
 Contribution is welcome. If you find a bug or feel like you can contribute please fork the repository, update the code and then create a pull request so we can merge in the changes.
-
```

### Comparing `mdxpy-1.2/images/logo.png` & `mdxpy-1.3/images/logo.png`

 * *Files identical despite different names*

### Comparing `mdxpy-1.2/mdxpy/mdx.py` & `mdxpy-1.3/mdxpy/mdx.py`

 * *Files 2% similar despite different names*

```diff
@@ -897,15 +897,15 @@
         return f"{{TM1SORT({self.underlying_hierarchy_set.to_mdx()},{'ASC' if self.ascending else 'DESC'})}}"
 
 
 class HierarchizeSet(MdxHierarchySet):
 
     def __init__(self, underlying_hierarchy_set: MdxHierarchySet):
         super(HierarchizeSet, self).__init__(underlying_hierarchy_set.dimension,
-                                                underlying_hierarchy_set.hierarchy)
+                                             underlying_hierarchy_set.hierarchy)
         self.underlying_hierarchy_set = underlying_hierarchy_set
 
     def to_mdx(self) -> str:
         return f"{{HIERARCHIZE({self.underlying_hierarchy_set.to_mdx()})}}"
 
 
 class HeadHierarchySet(MdxHierarchySet):
@@ -1071,25 +1071,37 @@
 
     def is_empty(self) -> bool:
         return not self.dim_sets and not self.tuples
 
     def set_non_empty(self, non_empty: bool = True):
         self.non_empty = non_empty
 
-    def to_mdx(self, tm1_ignore_bad_tuples=False) -> str:
+    def to_mdx(self, tm1_ignore_bad_tuples: bool = False, head: int = None, tail: int = None) -> str:
         if self.is_empty():
             return "{}"
 
-        return f"""{"NON EMPTY " if self.non_empty else ""}{"TM1IGNORE_BADTUPLES " if tm1_ignore_bad_tuples else ""}{self.dim_sets_to_mdx() if self.dim_sets else self.tuples_to_mdx()}"""
+        return f"""{"NON EMPTY " if self.non_empty else ""}{"TM1IGNORE_BADTUPLES " if tm1_ignore_bad_tuples else ""}{self.dim_sets_to_mdx(head, tail) if self.dim_sets else self.tuples_to_mdx(head, tail)}"""
 
-    def dim_sets_to_mdx(self) -> str:
-        return " * ".join(dim_set.to_mdx() for dim_set in self.dim_sets)
+    def dim_sets_to_mdx(self, head: int = None, tail: int = None) -> str:
+        mdx = " * ".join(dim_set.to_mdx() for dim_set in self.dim_sets)
+        if head is not None:
+            mdx = f"{{HEAD({mdx}, {head})}}"
+        if tail is not None:
+            mdx = f"{{TAIL({mdx}, {tail})}}"
+
+        return mdx
+
+    def tuples_to_mdx(self, head: int = None, tail: int = None) -> str:
+        mdx = f"{{{','.join(tupl.to_mdx() for tupl in self.tuples)}}}"
+        if head is not None:
+            mdx = f"{{HEAD({mdx}, {head})}}"
+        if tail is not None:
+            mdx = f"{{TAIL({mdx}, {tail})}}"
 
-    def tuples_to_mdx(self) -> str:
-        return f"{{{','.join(tupl.to_mdx() for tupl in self.tuples)}}}"
+        return mdx
 
 
 class MdxBuilder:
     def __init__(self, cube: str):
         self.cube = normalize(cube)
         self.axes = {0: MdxAxis.empty()}
         self._where = MdxTuple.empty()
@@ -1205,35 +1217,50 @@
             if not isinstance(member, DimensionProperty):
                 raise ValueError(f"Argument '{member}' must be of type str or DimensionProperty")
 
             self.add_member_to_properties(axis, member)
 
         return self
 
-    def _axis_mdx(self, position):
+    def _axis_mdx(self, position: int, head: int = None, tail: int = None, skip_dimension_properties=False):
         axis = self.axes[position]
         axis_properties = self.axes_properties.get(position, MdxPropertiesTuple.empty())
         if axis.is_empty():
             return ""
 
+        if skip_dimension_properties:
+            return " ".join([
+                axis.to_mdx(self._tm1_ignore_bad_tuples, head, tail),
+                f"ON {position}"
+            ])
+
         return " ".join([
-            axis.to_mdx(self._tm1_ignore_bad_tuples),
+            axis.to_mdx(self._tm1_ignore_bad_tuples, head, tail),
             "DIMENSION PROPERTIES",
             "MEMBER_NAME" if axis_properties.is_empty() else axis_properties.to_mdx(),
             f"ON {position}"
         ])
 
-    def to_mdx(self) -> str:
+    def to_mdx(self, head_columns: int = None, head_rows: int = None, tail_columns: int = None, tail_rows: int = None,
+               skip_dimension_properties: bool = False) -> str:
         mdx_with = "WITH\r\n" + "\r\n".join(
             calculated_member.to_mdx()
             for calculated_member
             in self.calculated_members) + "\r\n"
 
+        head_by_axis_position = {0: head_columns, 1: head_rows}
+        tail_by_axis_position = {0: tail_columns, 1: tail_rows}
+
         mdx_axes = ",\r\n".join(
-            self._axis_mdx(position)
+            self._axis_mdx(
+                position,
+                # default for head, tail is False for axes beyond rows and columns
+                head=head_by_axis_position.get(position, False),
+                tail=tail_by_axis_position.get(position, False),
+                skip_dimension_properties=skip_dimension_properties)
             for position
             in self.axes)
 
         mdx_where = "\r\nWHERE " + self._where.to_mdx() if not self._where.is_empty() else ""
 
         return f"""{mdx_with if self.calculated_members else ""}SELECT\r\n{mdx_axes}\r\nFROM [{self.cube}]{mdx_where}"""
```

### Comparing `mdxpy-1.2/mdxpy.egg-info/PKG-INFO` & `mdxpy-1.3/mdxpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdxpy
-Version: 1.2
+Version: 1.3
 Summary: A simple, yet elegant MDX library for TM1
 Home-page: https://github.com/cubewise-code/mdxpy
 Maintainer: Marius Wirtz
 Maintainer-email: MWirtz@cubewise.com
 License: MIT-LICENSE
 Keywords: MDX,TM1,IBM Cognos TM1,Planning Analytics,PA,Cognos
 Platform: any
@@ -254,8 +254,7 @@
 ## Tests
 
 All tests in `test.py`
 
 ## Contribution
 
 Contribution is welcome. If you find a bug or feel like you can contribute please fork the repository, update the code and then create a pull request so we can merge in the changes.
-
```

### Comparing `mdxpy-1.2/readme.md` & `mdxpy-1.3/readme.md`

 * *Files identical despite different names*

### Comparing `mdxpy-1.2/setup.py` & `mdxpy-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 DESCRIPTION = open('readme.md').read()
 
 setup(
     name="mdxpy",
-    version='1.2',
+    version='1.3',
     maintainer='Marius Wirtz',
     maintainer_email='MWirtz@cubewise.com',
     license="MIT-LICENSE",
     url='https://github.com/cubewise-code/mdxpy',
     platforms=["any"],
     description="A simple, yet elegant MDX library for TM1",
     long_description=DESCRIPTION,
```

### Comparing `mdxpy-1.2/test.py` & `mdxpy-1.3/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,15 @@
 
         self.assertEqual(
             "{{[dimension].[dimension].[element1].CHILDREN}"
             " * {[dimension].[dimension].[element2]}"
             " * {[dimension].[dimension].[element3]}}",
             mdx_set.to_mdx())
 
+
     def test_mdx_set_tuples(self):
         mdx_set = MdxSet.tuples([
             MdxTuple([Member.of("dimension1", "element1"), Member.of("dimension2", "element3")]),
             MdxTuple([Member.of("dimension1", "element2"), Member.of("dimension2", "element2")]),
             MdxTuple([Member.of("dimension1", "element3"), Member.of("dimension2", "element1")])
         ])
 
@@ -839,14 +840,66 @@
             "SELECT\r\n"
             "NON EMPTY {[period].[period].[avg2016],[period].[period].[sum2016]} DIMENSION PROPERTIES MEMBER_NAME ON 0,\r\n"
             "NON EMPTY {TM1FILTERBYLEVEL({TM1SUBSETALL([dim1].[dim1])},0)} DIMENSION PROPERTIES MEMBER_NAME ON 1\r\n"
             "FROM [cube]\r\n"
             "WHERE ([dim2].[dim2].[totaldim2])",
             mdx)
 
+    def test_mdx_builder_to_mdx_skip_dimension_properties(self):
+        mdx = MdxBuilder.from_cube("cube") \
+            .rows_non_empty() \
+            .add_hierarchy_set_to_row_axis(MdxHierarchySet.all_leaves("Dim1")) \
+            .columns_non_empty() \
+            .add_hierarchy_set_to_column_axis(MdxHierarchySet.member(Member.of("Dim2", "Elem2"))) \
+            .where(Member.of("Dim3", "Elem3"), Member.of("Dim4", "Elem4")) \
+            .to_mdx(skip_dimension_properties=True)
+
+        self.assertEqual(
+            "SELECT\r\n"
+            "NON EMPTY {[dim2].[dim2].[elem2]} ON 0,\r\n"
+            "NON EMPTY {TM1FILTERBYLEVEL({TM1SUBSETALL([dim1].[dim1])},0)} ON 1\r\n"
+            "FROM [cube]\r\n"
+            "WHERE ([dim3].[dim3].[elem3],[dim4].[dim4].[elem4])",
+            mdx)
+
+    def test_mdx_builder_to_mdx_head_tail_columns(self):
+        mdx = MdxBuilder.from_cube("cube") \
+            .add_hierarchy_set_to_column_axis(MdxHierarchySet.all_leaves("Dim1")) \
+            .columns_non_empty() \
+            .add_hierarchy_set_to_column_axis(MdxHierarchySet.member(Member.of("Dim2", "Elem2"))) \
+            .where(Member.of("Dim3", "Elem3"), Member.of("Dim4", "Elem4")) \
+            .to_mdx(head_columns=2, tail_columns=1)
+
+        self.assertEqual(
+            "SELECT\r\n"
+            "NON EMPTY {TAIL({HEAD({TM1FILTERBYLEVEL({TM1SUBSETALL([dim1].[dim1])},0)} * {[dim2].[dim2].[elem2]}, 2)}, 1)} "
+            "DIMENSION PROPERTIES MEMBER_NAME ON 0\r\n"
+            "FROM [cube]\r\n"
+            "WHERE ([dim3].[dim3].[elem3],[dim4].[dim4].[elem4])",
+            mdx)
+
+    def test_mdx_builder_to_mdx_head_tail_rows_and_columns(self):
+        mdx = MdxBuilder.from_cube("cube") \
+            .add_hierarchy_set_to_column_axis(MdxHierarchySet.all_leaves("Dim1")) \
+            .columns_non_empty() \
+            .add_hierarchy_set_to_row_axis(MdxHierarchySet.all_leaves("Dim2")) \
+            .rows_non_empty() \
+            .where(Member.of("Dim3", "Elem3"), Member.of("Dim4", "Elem4")) \
+            .to_mdx(head_columns=4, tail_columns=2, head_rows=2, tail_rows=1)
+
+        self.assertEqual(
+            "SELECT\r\n"
+            "NON EMPTY {TAIL({HEAD({TM1FILTERBYLEVEL({TM1SUBSETALL([dim1].[dim1])},0)}, 4)}, 2)} "
+            "DIMENSION PROPERTIES MEMBER_NAME ON 0,\r\n"
+            "NON EMPTY {TAIL({HEAD({TM1FILTERBYLEVEL({TM1SUBSETALL([dim2].[dim2])},0)}, 2)}, 1)} "
+            "DIMENSION PROPERTIES MEMBER_NAME ON 1\r\n"
+            "FROM [cube]\r\n"
+            "WHERE ([dim3].[dim3].[elem3],[dim4].[dim4].[elem4])",
+            mdx)
+
     def test_OrderType_ASC(self):
         order = Order("asc")
         self.assertEqual(order, Order.ASC)
 
         order = Order("ASC")
         self.assertEqual(order, Order.ASC)
         self.assertEqual("ASC", str(order))
@@ -949,8 +1002,8 @@
 
     def test_level_expression_name(self):
         level = MdxLevelExpression.level_name('NamedLevel', "Dimension1", "Hierarchy1")
         self.assertEqual("[dimension1].[hierarchy1].LEVELS('NamedLevel')", level.to_mdx())
 
     def test_level_expression_member_level(self):
         level = MdxLevelExpression.member_level(Member.of("Dimension1", "Hierarchy1", "Element1"))
-        self.assertEqual("[dimension1].[hierarchy1].[element1].LEVEL", level.to_mdx())
+        self.assertEqual("[dimension1].[hierarchy1].[element1].LEVEL", level.to_mdx())
```

