# Comparing `tmp/pyxll_jupyter-0.3.3-py3-none-any.whl.zip` & `tmp/pyxll_jupyter-0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 34070 bytes, number of entries: 21
+Zip file size: 34114 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat      496 b- defN 20-Sep-14 16:14 pyxll_jupyter/__init__.py
--rw-rw-rw-  2.0 fat    22969 b- defN 23-Jan-26 10:15 pyxll_jupyter/kernel.py
+-rw-rw-rw-  2.0 fat    22985 b- defN 23-Apr-14 14:22 pyxll_jupyter/kernel.py
 -rw-rw-rw-  2.0 fat     9105 b- defN 23-Jan-26 10:15 pyxll_jupyter/magic.py
 -rw-rw-rw-  2.0 fat    10122 b- defN 22-Jan-12 15:35 pyxll_jupyter/pyxll.py
 -rw-rw-rw-  2.0 fat       50 b- defN 23-Jan-26 10:15 pyxll_jupyter/kernel_managers/__init__.py
 -rw-rw-rw-  2.0 fat     4196 b- defN 23-Jan-26 10:15 pyxll_jupyter/kernel_managers/extipy.py
 -rw-rw-rw-  2.0 fat       43 b- defN 23-Jan-26 10:15 pyxll_jupyter/provisioning/__init__.py
 -rw-rw-rw-  2.0 fat     1729 b- defN 23-Jan-26 10:15 pyxll_jupyter/provisioning/existing.py
 -rw-rw-rw-  2.0 fat     5704 b- defN 21-Jul-27 09:57 pyxll_jupyter/resources/browser.png
 -rw-rw-rw-  2.0 fat     4436 b- defN 20-Sep-14 08:15 pyxll_jupyter/resources/jupyter.png
 -rw-rw-rw-  2.0 fat     1658 b- defN 21-Jul-27 09:57 pyxll_jupyter/resources/ribbon.xml
 -rw-rw-rw-  2.0 fat       64 b- defN 21-Jul-27 09:57 pyxll_jupyter/widgets/__init__.py
 -rw-rw-rw-  2.0 fat     4786 b- defN 21-Jul-27 09:57 pyxll_jupyter/widgets/browser.py
 -rw-rw-rw-  2.0 fat     1856 b- defN 22-Jan-12 15:35 pyxll_jupyter/widgets/jupyter.py
 -rw-rw-rw-  2.0 fat     3302 b- defN 22-Jan-12 15:35 pyxll_jupyter/widgets/qtimports.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Mar-10 18:08 pyxll_jupyter-0.3.3.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat     5262 b- defN 23-Mar-10 18:08 pyxll_jupyter-0.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-10 18:08 pyxll_jupyter-0.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      187 b- defN 23-Mar-10 18:08 pyxll_jupyter-0.3.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       14 b- defN 23-Mar-10 18:08 pyxll_jupyter-0.3.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1854 b- defN 23-Mar-10 18:08 pyxll_jupyter-0.3.3.dist-info/RECORD
-21 files, 79012 bytes uncompressed, 31010 bytes compressed:  60.8%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Apr-14 14:25 pyxll_jupyter-0.3.4.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     5415 b- defN 23-Apr-14 14:25 pyxll_jupyter-0.3.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-14 14:25 pyxll_jupyter-0.3.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      187 b- defN 23-Apr-14 14:25 pyxll_jupyter-0.3.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-14 14:25 pyxll_jupyter-0.3.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1854 b- defN 23-Apr-14 14:25 pyxll_jupyter-0.3.4.dist-info/RECORD
+21 files, 79181 bytes uncompressed, 31054 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -39,26 +39,26 @@
 
 Filename: pyxll_jupyter/widgets/jupyter.py
 Comment: 
 
 Filename: pyxll_jupyter/widgets/qtimports.py
 Comment: 
 
-Filename: pyxll_jupyter-0.3.3.dist-info/LICENSE.md
+Filename: pyxll_jupyter-0.3.4.dist-info/LICENSE.md
 Comment: 
 
-Filename: pyxll_jupyter-0.3.3.dist-info/METADATA
+Filename: pyxll_jupyter-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: pyxll_jupyter-0.3.3.dist-info/WHEEL
+Filename: pyxll_jupyter-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: pyxll_jupyter-0.3.3.dist-info/entry_points.txt
+Filename: pyxll_jupyter-0.3.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyxll_jupyter-0.3.3.dist-info/top_level.txt
+Filename: pyxll_jupyter-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pyxll_jupyter-0.3.3.dist-info/RECORD
+Filename: pyxll_jupyter-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyxll_jupyter/kernel.py

```diff
@@ -195,15 +195,15 @@
     sys.__stdout__ = sys_stdout = sys.stdout
     sys.__stderr__ = sys_stderr = sys.stderr
 
     # Get or create the IPKernelApp instance and set the 'connection_dir' property
     if IPKernelApp.initialized():
         ipy = IPKernelApp.instance()
     else:
-        ipy = IPKernelApp.instance(local_ns={})
+        ipy = IPKernelApp.instance()
         ipy.connection_dir = _get_connection_dir(ipy)
         ipy.initialize([])
 
     # call the API embed function, which will use the monkey-patched method above
     embed_kernel(local_ns={})
 
     # register the magic functions
@@ -500,15 +500,15 @@
             _log.debug("Waiting for background thread to complete...")
             thread.join(timeout=1)
             if thread.is_alive():
                 _log.warning("Timed out waiting for background thread.")
 
         raise RuntimeError("Timed-out waiting for the Jupyter notebook URL.")
 
-    root, params = url.split("?", 1)
+    root, params = url.split("?", 1) if "?" in url else url, ""
     params = params.split("&")
     params.extend(_subcommand_query_params[subcommand])
 
     # Update the URL to point to the notebook
     if notebook is not None:
         root = root.rstrip("/") + "/notebooks/" + notebook
```

## Comparing `pyxll_jupyter-0.3.3.dist-info/LICENSE.md` & `pyxll_jupyter-0.3.4.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pyxll_jupyter-0.3.3.dist-info/METADATA` & `pyxll_jupyter-0.3.4.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-Metadata-Version: 2.1
-Name: pyxll-jupyter
-Version: 0.3.3
-Summary: Adds Jupyter notebooks to Microsoft Excel using PyXLL.
-Project-URL: Source, https://github.com/pyxll/pyxll-jupyter
-Project-URL: Tracker, https://github.com/pyxll/pyxll-jupyter/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: pyxll (>=5.1.0)
-Requires-Dist: jupyter (>=1.0.0)
-Requires-Dist: notebook (>=6.0.0)
-Requires-Dist: PySide2 ; python_version < "3.10"
-Requires-Dist: PySide6 (!=6.4.2) ; python_version >= "3.10"
-
-# PyXLL-Jupyter
-
-Integration for Jupyter notebooks and Microsoft Excel.
-
-See the [Python Jupyter Notebooks in Excel](https://www.pyxll.com/blog/python-jupyter-notebooks-in-excel/) blog post for more details.
-
-## Requirements
-
-- PyXLL >= 5.1.0
-- Jupyter >= 1.0.0
-- notebook >= 6.0.0
-- PySide2, or PySide6 for Python >= 3.10
-  
-### Optional
-
-- jupyterlab >= 4.0.0
-
-## Installation
-
-To install this package use:
-
-    pip install pyxll-jupyter
-
-Once installed a "Jupyter Notebook" button will be added to the PyXLL ribbon tab in Excel, so
-long as you have PyXLL 5 or above already installed.
-
-When using Jupyter in Excel the Python kernel runs inside the Excel process using PyXLL. You
-can interact with Excel from code in the Jupyter notebook, and write Excel functions
-using the PyXLL decorators @xl_menu and @xl_macro etc.
-
-As the kernel runs in the existing Python interpreter in the Excel process it is not possible
-to restart the kernel or to use other Python versions or other languages.
-
-## Configuration
-
-To configure add the following to your pyxll.cfg file (default values shown):
-
-    [JUPYTER]
-    use_workbook_dir = 0
-    notebook_dir = Documents
-    subcommand = notebook
-    timeout = 30
-    qt = PySide2
-    disable_ribbon = 0
-
-If *use_workbook_dir* is set and the current workbook is saved then Jupyter will open in the same folder
-as the current workbook.
-
-The *subcommand* option can be used to switch the Jupyter subcommand used to launch the Jupyter web server.
-It can be set to either `notebook` for the default Jupyter notebook interface, or `lab` if using Jupyterlab
-*(experimental)*.
-
-If *disable_ribbon* is set then the ribbon button to start Jupyter will not be shown, however Jupyter
-may still be opened using the "OpenJupyterNotebook" macro.
-
-## Experimental JupyterLab Support
-
-Jupyterlab can be used instead of the default Jupyter Notebook interface by specifying
-`subcommand = lab` in the ``[JUPYTER]`` section of the pyxll.cfg file.
-
-This requires Jupyterlab >= 4.0.0 to be installed. At the time of writing, version 4 of Jupyterlab is in
-pre-release and can be installed using:
-
-    pip install --pre jupyterlab
-
-### Qt
-
-The pyxll-jupyter package uses the Qt [QWebEngineView](https://doc.qt.io/qt-5/qwebengineview.html) widget, and by
-default will use the [PySide2](https://pypi.org/project/PySide2/) package for Python <= 3.9 or
-the [PySide6](https://pypi.org/project/PySide6/) package for Python >= 3.10.
-
-This can be changed to use [PyQt5](https://www.riverbankcomputing.com/software/pyqt/) by setting `qt = PyQt5` in
-the `JUPYTER` section of the config. You will need to have both the `pyqt5` and `pyqtwebengine` packages installed
-if using this option. Both can be installed using pip as follows:
-
-    pip install pyqt5 pyqtwebengine
-
-## Magic Functions
-
-The following magic functions are available in addition to the standard Jupyter magic functions:
-
-```
-%xl_get [-c CELL] [-t TYPE] [-x]
-
-Get the current selection in Excel into Python.
-
-optional arguments:
-  -c CELL, --cell CELL  Address of cell to get value of.
-  -t TYPE, --type TYPE  Datatype to convert the value to.
-  -x, --no-auto-resize  Don't auto-resize the range.
-```
-
-```
-%xl_set [-c CELL] [-t TYPE] [-f FORMATTER] [-x] value
-
-Set a value to the current selection in Excel.
-
-positional arguments:
-  value                 Value to set in Excel.
-
-optional arguments:
-  -c CELL, --cell CELL  Address of cell to get value of.
-  -t TYPE, --type TYPE  Datatype to convert the value to.
-  -f FORMATTER, --formatter FORMATTER
-                        PyXLL Formatter to use when setting the value.
-  -x, --no-auto-resize  Don't auto-resize the range.
-```
-
-```
-%xl_plot [-n NAME] [-c CELL] [-w WIDTH] [-h HEIGHT] figure
-
-Plot a figure to Excel in the same way as pyxll.plot.
-
-The figure is exported as an image and inserted into Excel as a Picture object.
-
-If the --name argument is used and the picture already exists then it will not
-be resized or moved.
-
-positional arguments:
-  figure                Figure to plot.
-
-optional arguments:
-  -n NAME, --name NAME  Name of the picture object in Excel to use.
-  -c CELL, --cell CELL  Address of cell to use when creating the Picture in
-                        Excel.
-  -w WIDTH, --width WIDTH
-                        Width in points to use when creating the Picture in
-                        Excel.
-  -h HEIGHT, --height HEIGHT
-                        Height in points to use when creating the Picture in
-                        Excel.
-```
-
-For more information about installing and using PyXLL see https://www.pyxll.com.
-
-Copyright (c) PyXLL Ltd
+Metadata-Version: 2.1
+Name: pyxll-jupyter
+Version: 0.3.4
+Summary: Adds Jupyter notebooks to Microsoft Excel using PyXLL.
+Project-URL: Source, https://github.com/pyxll/pyxll-jupyter
+Project-URL: Tracker, https://github.com/pyxll/pyxll-jupyter/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: pyxll (>=5.1.0)
+Requires-Dist: jupyter (>=1.0.0)
+Requires-Dist: notebook (>=6.0.0)
+Requires-Dist: PySide2 ; python_version < "3.10"
+Requires-Dist: PySide6 (!=6.4.2) ; python_version >= "3.10"
+
+# PyXLL-Jupyter
+
+Integration for Jupyter notebooks and Microsoft Excel.
+
+See the [Python Jupyter Notebooks in Excel](https://www.pyxll.com/blog/python-jupyter-notebooks-in-excel/) blog post for more details.
+
+## Requirements
+
+- PyXLL >= 5.1.0
+- Jupyter >= 1.0.0
+- notebook >= 6.0.0
+- PySide2, or PySide6 for Python >= 3.10
+  
+### Optional
+
+- jupyterlab >= 4.0.0
+
+## Installation
+
+To install this package use:
+
+    pip install pyxll-jupyter
+
+Once installed a "Jupyter Notebook" button will be added to the PyXLL ribbon tab in Excel, so
+long as you have PyXLL 5 or above already installed.
+
+When using Jupyter in Excel the Python kernel runs inside the Excel process using PyXLL. You
+can interact with Excel from code in the Jupyter notebook, and write Excel functions
+using the PyXLL decorators @xl_menu and @xl_macro etc.
+
+As the kernel runs in the existing Python interpreter in the Excel process it is not possible
+to restart the kernel or to use other Python versions or other languages.
+
+## Configuration
+
+To configure add the following to your pyxll.cfg file (default values shown):
+
+    [JUPYTER]
+    use_workbook_dir = 0
+    notebook_dir = Documents
+    subcommand = notebook
+    timeout = 30
+    qt = PySide2
+    disable_ribbon = 0
+
+If *use_workbook_dir* is set and the current workbook is saved then Jupyter will open in the same folder
+as the current workbook.
+
+The *subcommand* option can be used to switch the Jupyter subcommand used to launch the Jupyter web server.
+It can be set to either `notebook` for the default Jupyter notebook interface, or `lab` if using Jupyterlab
+*(experimental)*.
+
+If *disable_ribbon* is set then the ribbon button to start Jupyter will not be shown, however Jupyter
+may still be opened using the "OpenJupyterNotebook" macro.
+
+## Experimental JupyterLab Support
+
+Jupyterlab can be used instead of the default Jupyter Notebook interface by specifying
+`subcommand = lab` in the ``[JUPYTER]`` section of the pyxll.cfg file.
+
+This requires Jupyterlab >= 4.0.0 to be installed. At the time of writing, version 4 of Jupyterlab is in
+pre-release and can be installed using:
+
+    pip install --pre jupyterlab
+
+### Qt
+
+The pyxll-jupyter package uses the Qt [QWebEngineView](https://doc.qt.io/qt-5/qwebengineview.html) widget, and by
+default will use the [PySide2](https://pypi.org/project/PySide2/) package for Python <= 3.9 or
+the [PySide6](https://pypi.org/project/PySide6/) package for Python >= 3.10.
+
+This can be changed to use [PyQt5](https://www.riverbankcomputing.com/software/pyqt/) by setting `qt = PyQt5` in
+the `JUPYTER` section of the config. You will need to have both the `pyqt5` and `pyqtwebengine` packages installed
+if using this option. Both can be installed using pip as follows:
+
+    pip install pyqt5 pyqtwebengine
+
+## Magic Functions
+
+The following magic functions are available in addition to the standard Jupyter magic functions:
+
+```
+%xl_get [-c CELL] [-t TYPE] [-x]
+
+Get the current selection in Excel into Python.
+
+optional arguments:
+  -c CELL, --cell CELL  Address of cell to get value of.
+  -t TYPE, --type TYPE  Datatype to convert the value to.
+  -x, --no-auto-resize  Don't auto-resize the range.
+```
+
+```
+%xl_set [-c CELL] [-t TYPE] [-f FORMATTER] [-x] value
+
+Set a value to the current selection in Excel.
+
+positional arguments:
+  value                 Value to set in Excel.
+
+optional arguments:
+  -c CELL, --cell CELL  Address of cell to get value of.
+  -t TYPE, --type TYPE  Datatype to convert the value to.
+  -f FORMATTER, --formatter FORMATTER
+                        PyXLL Formatter to use when setting the value.
+  -x, --no-auto-resize  Don't auto-resize the range.
+```
+
+```
+%xl_plot [-n NAME] [-c CELL] [-w WIDTH] [-h HEIGHT] figure
+
+Plot a figure to Excel in the same way as pyxll.plot.
+
+The figure is exported as an image and inserted into Excel as a Picture object.
+
+If the --name argument is used and the picture already exists then it will not
+be resized or moved.
+
+positional arguments:
+  figure                Figure to plot.
+
+optional arguments:
+  -n NAME, --name NAME  Name of the picture object in Excel to use.
+  -c CELL, --cell CELL  Address of cell to use when creating the Picture in
+                        Excel.
+  -w WIDTH, --width WIDTH
+                        Width in points to use when creating the Picture in
+                        Excel.
+  -h HEIGHT, --height HEIGHT
+                        Height in points to use when creating the Picture in
+                        Excel.
+```
+
+For more information about installing and using PyXLL see https://www.pyxll.com.
+
+Copyright (c) PyXLL Ltd
```

## Comparing `pyxll_jupyter-0.3.3.dist-info/RECORD` & `pyxll_jupyter-0.3.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 pyxll_jupyter/__init__.py,sha256=mdO9kpbRcBx_UPSU8Zyk6vWvvZnWk-Eand3_Q7ns8RI,496
-pyxll_jupyter/kernel.py,sha256=0ZzMVfl60f0odhIVflOcsm_2oPLgTYzQ7KGCbbtXp8M,22969
+pyxll_jupyter/kernel.py,sha256=9Lmn6rZxg2z5PimohdzlwZMk3f3pm8qo0nNsANo44rA,22985
 pyxll_jupyter/magic.py,sha256=KMd_yLfBT6fT-A0EgHGdKJs54hwDmomy6_cQDkmguKo,9105
 pyxll_jupyter/pyxll.py,sha256=gG8BF4LU68BkJKVPLta77GkJms6TAdB7oVYM1oZspng,10122
 pyxll_jupyter/kernel_managers/__init__.py,sha256=BGLY9OvRJSMCQwhpiz7NVG6DL2XeJIE1agExSBFVrH0,50
 pyxll_jupyter/kernel_managers/extipy.py,sha256=brHXOVCDKFgTfAHORXljrPdPkY9YLMJpKJ4BsM4rlCg,4196
 pyxll_jupyter/provisioning/__init__.py,sha256=SSQgCsR_Jfjwk3FgHRRbIicdnXb2NBXY5q9eya5f_JU,43
 pyxll_jupyter/provisioning/existing.py,sha256=kh003AwVk6GpTQcQT2WQI1fy46uxBXGKEOwLjJx1mf4,1729
 pyxll_jupyter/resources/browser.png,sha256=fFQoWhmOzguG-mzOSfQw1aBgu54zM7RcUrO8dC1qD60,5704
 pyxll_jupyter/resources/jupyter.png,sha256=H6BglrUs-6rd-Y4kOZxelx4G3cg0yDKbRZNtTQf4KV0,4436
 pyxll_jupyter/resources/ribbon.xml,sha256=w5jIm_Z77Gb7K_NXPMrV1YixcvYEvZIUvt0EPp0zaV8,1658
 pyxll_jupyter/widgets/__init__.py,sha256=1eX2naiOVjgOqQ8UxsKYX1_c_IRAGK7FU-YBSjdGzWs,64
 pyxll_jupyter/widgets/browser.py,sha256=yUiiAl_G2TuZi_bz9Eovt7ViK6Z2NMsHYzvHsakqd-Q,4786
 pyxll_jupyter/widgets/jupyter.py,sha256=cRI2_sWYZBUN5zLtOwj3ozHz934pSrtVTv5Y1GwwphY,1856
 pyxll_jupyter/widgets/qtimports.py,sha256=gHzHDEC-48Q2VIEdD-_PUFws9lNQatESTpjQAqpJNxo,3302
-pyxll_jupyter-0.3.3.dist-info/LICENSE.md,sha256=_Lv_zhFvdAlSe69UkLShEwwRh7pdMDdjzRZcnxMRj2I,1087
-pyxll_jupyter-0.3.3.dist-info/METADATA,sha256=IsJhjpbkJI8vLP7xXWmSbK8BhVgAPp3XP2lj3G8wq0w,5262
-pyxll_jupyter-0.3.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyxll_jupyter-0.3.3.dist-info/entry_points.txt,sha256=i_TC66oleWSd3gOkTNbNHU6oIqzvfszSGhiU8UNcI9U,187
-pyxll_jupyter-0.3.3.dist-info/top_level.txt,sha256=O8yEET2io_Bn_UyxBhokmuBOysbyrxVg2jGa1OVWQ8M,14
-pyxll_jupyter-0.3.3.dist-info/RECORD,,
+pyxll_jupyter-0.3.4.dist-info/LICENSE.md,sha256=_Lv_zhFvdAlSe69UkLShEwwRh7pdMDdjzRZcnxMRj2I,1087
+pyxll_jupyter-0.3.4.dist-info/METADATA,sha256=w9LIGdmOgLH6gA1ZY5otHhn3xj_kfCC9CK3KQnBpGo0,5415
+pyxll_jupyter-0.3.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pyxll_jupyter-0.3.4.dist-info/entry_points.txt,sha256=i_TC66oleWSd3gOkTNbNHU6oIqzvfszSGhiU8UNcI9U,187
+pyxll_jupyter-0.3.4.dist-info/top_level.txt,sha256=O8yEET2io_Bn_UyxBhokmuBOysbyrxVg2jGa1OVWQ8M,14
+pyxll_jupyter-0.3.4.dist-info/RECORD,,
```

