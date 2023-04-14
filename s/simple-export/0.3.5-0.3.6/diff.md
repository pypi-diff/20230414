# Comparing `tmp/simple_export-0.3.5.tar.gz` & `tmp/simple_export-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_export-0.3.5.tar", max compression
+gzip compressed data, was "simple_export-0.3.6.tar", max compression
```

## Comparing `simple_export-0.3.5.tar` & `simple_export-0.3.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11558 2022-12-29 08:49:42.034585 simple_export-0.3.5/LICENSE
--rw-r--r--   0        0        0      490 2023-02-28 08:31:39.549880 simple_export-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     5642 2023-02-14 07:32:15.756247 simple_export-0.3.5/README.md
--rw-r--r--   0        0        0       50 2023-02-13 07:58:17.521852 simple_export-0.3.5/src/simple_export/.idea/.gitignore
--rw-r--r--   0        0        0      174 2023-02-13 07:58:17.390823 simple_export-0.3.5/src/simple_export/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1897 2023-02-13 07:58:17.159769 simple_export-0.3.5/src/simple_export/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      195 2023-02-22 07:49:57.015250 simple_export-0.3.5/src/simple_export/.idea/misc.xml
--rw-r--r--   0        0        0      285 2023-02-13 07:58:17.366817 simple_export-0.3.5/src/simple_export/.idea/modules.xml
--rw-r--r--   0        0        0      492 2023-02-22 07:49:56.994245 simple_export-0.3.5/src/simple_export/.idea/simple_export.iml
--rw-r--r--   0        0        0      197 2023-02-13 07:58:17.399824 simple_export-0.3.5/src/simple_export/.idea/vcs.xml
--rw-r--r--   0        0        0        0 2023-02-13 08:28:24.823233 simple_export-0.3.5/src/simple_export/__init__.py
--rw-r--r--   0        0        0   154079 2023-02-28 08:31:14.167481 simple_export-0.3.5/src/simple_export/example.py
--rw-r--r--   0        0        0    15739 2023-02-28 08:30:18.895889 simple_export-0.3.5/src/simple_export/excel.py
--rw-r--r--   0        0        0    41114 2023-02-14 07:29:25.331551 simple_export-0.3.5/src/simple_export/template/excel1.xlsx
--rw-r--r--   0        0        0    11352 2023-01-12 03:17:12.536000 simple_export-0.3.5/src/simple_export/template/excel2.xlsx
--rw-r--r--   0        0        0    10967 2023-02-20 08:13:21.039107 simple_export-0.3.5/src/simple_export/template/excel3.xlsx
--rw-r--r--   0        0        0    22872 2023-02-20 08:38:58.217000 simple_export-0.3.5/src/simple_export/template/excel4.xlsx
--rw-r--r--   0        0        0    35163 2023-02-21 15:29:11.649864 simple_export-0.3.5/src/simple_export/template/excel5.xlsx
--rw-r--r--   0        0        0    17711 2023-02-23 08:39:03.895000 simple_export-0.3.5/src/simple_export/template/excel6.xlsx
--rw-r--r--   0        0        0      149 2022-12-29 08:49:42.040587 simple_export-0.3.5/src/simple_export/utils/__init__.py
--rw-r--r--   0        0        0      174 2023-01-12 03:40:59.563232 simple_export-0.3.5/src/simple_export/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2674 2023-02-13 08:57:59.220807 simple_export-0.3.5/src/simple_export/utils/__pycache__/tool.cpython-38.pyc
--rw-r--r--   0        0        0     2007 2023-02-27 03:58:32.179073 simple_export-0.3.5/src/simple_export/utils/__pycache__/util.cpython-38.pyc
--rw-r--r--   0        0        0     2331 2023-02-21 09:20:15.346033 simple_export-0.3.5/src/simple_export/utils/tool.py
--rw-r--r--   0        0        0     2356 2023-02-27 06:25:24.905543 simple_export-0.3.5/src/simple_export/utils/util.py
--rw-r--r--   0        0        0    57060 2023-02-28 08:30:55.324361 simple_export-0.3.5/src/simple_export/val1.xlsx
--rw-r--r--   0        0        0     6220 1970-01-01 00:00:00.000000 simple_export-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11558 2022-12-29 08:49:42.034585 simple_export-0.3.6/LICENSE
+-rw-r--r--   0        0        0      490 2023-04-14 07:53:38.895147 simple_export-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     5642 2023-02-14 07:32:15.756247 simple_export-0.3.6/README.md
+-rw-r--r--   0        0        0       50 2023-02-13 07:58:17.521852 simple_export-0.3.6/src/simple_export/.idea/.gitignore
+-rw-r--r--   0        0        0      174 2023-02-13 07:58:17.390823 simple_export-0.3.6/src/simple_export/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1897 2023-02-13 07:58:17.159769 simple_export-0.3.6/src/simple_export/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      195 2023-02-22 07:49:57.015250 simple_export-0.3.6/src/simple_export/.idea/misc.xml
+-rw-r--r--   0        0        0      285 2023-02-13 07:58:17.366817 simple_export-0.3.6/src/simple_export/.idea/modules.xml
+-rw-r--r--   0        0        0      492 2023-02-22 07:49:56.994245 simple_export-0.3.6/src/simple_export/.idea/simple_export.iml
+-rw-r--r--   0        0        0      197 2023-02-13 07:58:17.399824 simple_export-0.3.6/src/simple_export/.idea/vcs.xml
+-rw-r--r--   0        0        0        0 2023-02-13 08:28:24.823233 simple_export-0.3.6/src/simple_export/__init__.py
+-rw-r--r--   0        0        0   154079 2023-02-28 08:31:14.167481 simple_export-0.3.6/src/simple_export/example.py
+-rw-r--r--   0        0        0    15739 2023-02-28 08:30:18.895889 simple_export-0.3.6/src/simple_export/excel.py
+-rw-r--r--   0        0        0    41114 2023-02-14 07:29:25.331551 simple_export-0.3.6/src/simple_export/template/excel1.xlsx
+-rw-r--r--   0        0        0    11352 2023-01-12 03:17:12.536000 simple_export-0.3.6/src/simple_export/template/excel2.xlsx
+-rw-r--r--   0        0        0    10967 2023-02-20 08:13:21.039107 simple_export-0.3.6/src/simple_export/template/excel3.xlsx
+-rw-r--r--   0        0        0    22872 2023-02-20 08:38:58.217000 simple_export-0.3.6/src/simple_export/template/excel4.xlsx
+-rw-r--r--   0        0        0    35163 2023-02-21 15:29:11.649864 simple_export-0.3.6/src/simple_export/template/excel5.xlsx
+-rw-r--r--   0        0        0    17711 2023-02-23 08:39:03.895000 simple_export-0.3.6/src/simple_export/template/excel6.xlsx
+-rw-r--r--   0        0        0      149 2022-12-29 08:49:42.040587 simple_export-0.3.6/src/simple_export/utils/__init__.py
+-rw-r--r--   0        0        0      174 2023-01-12 03:40:59.563232 simple_export-0.3.6/src/simple_export/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2674 2023-02-13 08:57:59.220807 simple_export-0.3.6/src/simple_export/utils/__pycache__/tool.cpython-38.pyc
+-rw-r--r--   0        0        0     2007 2023-02-27 03:58:32.179073 simple_export-0.3.6/src/simple_export/utils/__pycache__/util.cpython-38.pyc
+-rw-r--r--   0        0        0     2331 2023-02-21 09:20:15.346033 simple_export-0.3.6/src/simple_export/utils/tool.py
+-rw-r--r--   0        0        0     4024 2023-04-14 07:52:05.555606 simple_export-0.3.6/src/simple_export/utils/util.py
+-rw-r--r--   0        0        0    57060 2023-02-28 08:30:55.324361 simple_export-0.3.6/src/simple_export/val1.xlsx
+-rw-r--r--   0        0        0     6220 1970-01-01 00:00:00.000000 simple_export-0.3.6/PKG-INFO
```

### Comparing `simple_export-0.3.5/LICENSE` & `simple_export-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/README.md` & `simple_export-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/src/simple_export/.idea/inspectionProfiles/Project_Default.xml` & `simple_export-0.3.6/src/simple_export/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/src/simple_export/example.py` & `simple_export-0.3.6/src/simple_export/example.py`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/src/simple_export/excel.py` & `simple_export-0.3.6/src/simple_export/excel.py`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/src/simple_export/template/excel1.xlsx` & `simple_export-0.3.6/src/simple_export/template/excel1.xlsx`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/src/simple_export/template/excel2.xlsx` & `simple_export-0.3.6/src/simple_export/template/excel2.xlsx`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/src/simple_export/template/excel3.xlsx` & `simple_export-0.3.6/src/simple_export/template/excel3.xlsx`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/src/simple_export/template/excel4.xlsx` & `simple_export-0.3.6/src/simple_export/template/excel4.xlsx`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/src/simple_export/template/excel5.xlsx` & `simple_export-0.3.6/src/simple_export/template/excel5.xlsx`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/src/simple_export/template/excel6.xlsx` & `simple_export-0.3.6/src/simple_export/template/excel6.xlsx`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/src/simple_export/utils/__pycache__/tool.cpython-38.pyc` & `simple_export-0.3.6/src/simple_export/utils/__pycache__/tool.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/src/simple_export/utils/__pycache__/util.cpython-38.pyc` & `simple_export-0.3.6/src/simple_export/utils/__pycache__/util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/src/simple_export/utils/tool.py` & `simple_export-0.3.6/src/simple_export/utils/tool.py`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/src/simple_export/utils/util.py` & `simple_export-0.3.6/src/simple_export/utils/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -43,13 +43,48 @@
         p = pos_mapping[row]
         start_row, end_row = p[0], p[-1]
         start = start_row - 1
         align = Alignment(horizontal='center', vertical='center', wrap_text=True)
         for i in range(start_row, end_row):
             current_cell, prev_cell = pos[i][col], pos[i - 1][col]
             if isinstance(current_cell, Cell) and isinstance(prev_cell, Cell) and current_cell.value != prev_cell.value:
-                sheet.merge_cells(start_row=start + 1, start_column=col + 1, end_column=col + 1, end_row=i)
-                sheet[num_to_pos_char((col + 1, start + 1))].alignment = align
+                if i > start + 1:
+                    sheet.merge_cells(start_row=start + 1, start_column=col + 1, end_column=col + 1, end_row=i)
+                    sheet[num_to_pos_char((col + 1, start + 1))].alignment = align
                 start = i
         if end_row - start > 1:
             sheet.merge_cells(start_row=start + 1, start_column=col + 1, end_column=col + 1, end_row=end_row)
-            sheet[num_to_pos_char((col + 1, start + 1))].alignment = align
+            sheet[num_to_pos_char((col + 1, start + 1))].alignment = align
+
+    """
+    合并单元格向左合并
+    """
+    def merge_left(self, coordinate: str, sheet: Worksheet, pos_mapping: collections.defaultdict, pos: collections.defaultdict ) -> None:
+        """
+        将指定单元格下方的所有单元格合并为一个单元格。
+        :param coordinate: 单元格的坐标，例如 "A1"。
+        :param sheet: 工作表对象。
+        :param pos_mapping: 单元格坐标到行列号的映射。
+        :return: 无返回值。
+        """
+        col, row = char_to_num(coordinate)
+        col -= 1
+        row -= 1
+        p = pos_mapping[row]
+        c = pos_mapping[col]
+        start_row, end_row = p[0], p[-1]
+        start = 0
+        end_col = col + 1
+        align = Alignment(horizontal='center', vertical='center', wrap_text=True)
+
+        for i in range(start_row, end_row):
+            for j in range(1, end_col):
+                current_cell, prev_cell = pos[i][col], pos[i][col - j]
+                if isinstance(current_cell, Cell) and isinstance(prev_cell, Cell) and current_cell.value != prev_cell.value:
+                    if end_col - j + 1 != i+1:
+                        sheet.merge_cells(start_row=i+1, start_column=end_col - j + 1, end_column=end_col, end_row=i+1)
+                        sheet[num_to_pos_char((end_col - j + 1, i+1))].alignment = align
+                        break
+                start = j
+            if end_col - start <= 1:
+                sheet.merge_cells(start_row=i+1, start_column=1, end_column=end_col, end_row=i+1)
+                sheet[num_to_pos_char((1, i+1))].alignment = align
```

### Comparing `simple_export-0.3.5/src/simple_export/val1.xlsx` & `simple_export-0.3.6/src/simple_export/val1.xlsx`

 * *Files identical despite different names*

### Comparing `simple_export-0.3.5/PKG-INFO` & `simple_export-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-export
-Version: 0.3.5
+Version: 0.3.6
 Summary: 简单的模板导出工具
 License: Apache
 Author: mtl
 Author-email: 576694002@qq.com
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

