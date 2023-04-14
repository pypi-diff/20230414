# Comparing `tmp/jira-assistant-0.1.7.tar.gz` & `tmp/jira-assistant-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira-assistant-0.1.7.tar", last modified: Tue Apr 11 06:21:25 2023, max compression
+gzip compressed data, was "jira-assistant-0.1.8.tar", last modified: Fri Apr 14 15:33:14 2023, max compression
```

## Comparing `jira-assistant-0.1.7.tar` & `jira-assistant-0.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:21:25.592825 jira-assistant-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-04-11 06:21:25.592825 jira-assistant-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:21:25.592825 jira-assistant-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:21:25.588825 jira-assistant-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:21:25.588825 jira-assistant-0.1.7/src/jira_assistant/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:21:25.592825 jira-assistant-0.1.7/src/jira_assistant/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/assets/excel_definition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/assets/sprint_schedule.json
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/console_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    23368 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/excel_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/excel_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/jira_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/sprint_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16691 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/src/jira_assistant/story.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:21:25.592825 jira-assistant-0.1.7/src/jira_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-04-11 06:21:25.000000 jira-assistant-0.1.7/src/jira_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-11 06:21:25.000000 jira-assistant-0.1.7/src/jira_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:21:25.000000 jira-assistant-0.1.7/src/jira_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-11 06:21:25.000000 jira-assistant-0.1.7/src/jira_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-11 06:21:25.000000 jira-assistant-0.1.7/src/jira_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 06:21:25.000000 jira-assistant-0.1.7/src/jira_assistant.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:21:25.592825 jira-assistant-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_console_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_excel_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_excel_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_jira_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_sprint_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-11 06:21:15.000000 jira-assistant-0.1.7/tests/test_story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:33:14.626610 jira-assistant-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-04-14 15:33:14.626610 jira-assistant-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:33:14.626610 jira-assistant-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:33:14.622610 jira-assistant-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:33:14.622610 jira-assistant-0.1.8/src/jira_assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:33:14.626610 jira-assistant-0.1.8/src/jira_assistant/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/assets/excel_definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/assets/sprint_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/console_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23368 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/excel_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15774 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/excel_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/jira_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/sprint_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/src/jira_assistant/story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:33:14.626610 jira-assistant-0.1.8/src/jira_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-04-14 15:33:14.000000 jira-assistant-0.1.8/src/jira_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-14 15:33:14.000000 jira-assistant-0.1.8/src/jira_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:33:14.000000 jira-assistant-0.1.8/src/jira_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-14 15:33:14.000000 jira-assistant-0.1.8/src/jira_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-14 15:33:14.000000 jira-assistant-0.1.8/src/jira_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 15:33:14.000000 jira-assistant-0.1.8/src/jira_assistant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:33:14.626610 jira-assistant-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_console_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_excel_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_excel_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_jira_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_sprint_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-14 15:33:04.000000 jira-assistant-0.1.8/tests/test_story.py
```

### Comparing `jira-assistant-0.1.7/LICENSE` & `jira-assistant-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/PKG-INFO` & `jira-assistant-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-assistant
-Version: 0.1.7
+Version: 0.1.8
 Summary: Useful Jira tools
 Author-email: Sharry Xu <sharry.xu@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Sharry Xu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,37 +21,57 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/SharryXu/jira-assistant
-Keywords: jira,excel,jira-cloud
+Project-URL: Documentation, https://jira-assistant.readthedocs.io/en/stable
+Project-URL: Source, https://github.com/SharryXu/jira-assistant
+Project-URL: Tracker, https://github.com/SharryXu/jira-assistant/issues
+Keywords: jira,excel,sorting,project management,tool
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 6 - Mature
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Natural Language :: English
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 Jira Assistant - userful jira tools
 =============================================
 
-|pypi| |Download| |GithubIssues| |Linux| |Windows| |Mac OS| |Pylint| |CodeQL| |Documentation| |Codecov| |CodeClimate| |License|
+|pypi| |Download| |Package Size| |GithubIssues| |Linux| |Windows| |Mac OS| |Pylint| |CodeQL| |Documentation| |Codecov| |CodeClimate| |License|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/jira-assistant.svg?style=flat-square
     :target https://pypi.org/project/jira-assistant/
     :alt: pypi version
 
 .. |Download| image:: https://static.pepy.tech/personalized-badge/jira-assistant?period=month&units=international_system&left_color=black&right_color=blue&left_text=downloads/month
     :target: https://pepy.tech/project/jira-assistant
     :alt: download
 
+.. |Package Size| image:: https://img.shields.io/github/repo-size/sharryxu/jira-assistant
+    :target: https://img.shields.io/github/repo-size/sharryxu/jira-assistant
+    :alt: Package Size
+
 .. |GitHubIssues| image:: https://img.shields.io/github/issues/sharryxu/jira-assistant
    :target: https://img.shields.io/github/issues/sharryxu/jira-assistant
    :alt: GitHub issues
 
 .. |Linux| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml/badge.svg
     :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml
     :alt: python 3.11 (Linux)
@@ -112,14 +132,19 @@
 ========
 
 * Parsing the excel file which usually been downloaded from the Jira platform.
 * Sorting the excel records using some specific logic.
 * Generating the target excel file which contains the result.
 * The excel file structure can be customized by JSON file.
 
+Documentation
+=============
+
+For full documentation, including installation, tutorials and PDF documents, please see https://jira-assistant.readthedocs.io/en/stable/
+
 A Simple Example
 ================
 You can run below command in the PowerShell (Windows OS) or Shell (UNIX OS) to process the excel files.
 
 .. code-block:: console
 
     process-excel-file source.xlsx
```

### Comparing `jira-assistant-0.1.7/README.rst` & `jira-assistant-0.1.8/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Jira Assistant - userful jira tools
 =============================================
 
-|pypi| |Download| |GithubIssues| |Linux| |Windows| |Mac OS| |Pylint| |CodeQL| |Documentation| |Codecov| |CodeClimate| |License|
+|pypi| |Download| |Package Size| |GithubIssues| |Linux| |Windows| |Mac OS| |Pylint| |CodeQL| |Documentation| |Codecov| |CodeClimate| |License|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/jira-assistant.svg?style=flat-square
     :target https://pypi.org/project/jira-assistant/
     :alt: pypi version
 
 .. |Download| image:: https://static.pepy.tech/personalized-badge/jira-assistant?period=month&units=international_system&left_color=black&right_color=blue&left_text=downloads/month
     :target: https://pepy.tech/project/jira-assistant
     :alt: download
 
+.. |Package Size| image:: https://img.shields.io/github/repo-size/sharryxu/jira-assistant
+    :target: https://img.shields.io/github/repo-size/sharryxu/jira-assistant
+    :alt: Package Size
+
 .. |GitHubIssues| image:: https://img.shields.io/github/issues/sharryxu/jira-assistant
    :target: https://img.shields.io/github/issues/sharryxu/jira-assistant
    :alt: GitHub issues
 
 .. |Linux| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml/badge.svg
     :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml
     :alt: python 3.11 (Linux)
@@ -75,14 +79,19 @@
 ========
 
 * Parsing the excel file which usually been downloaded from the Jira platform.
 * Sorting the excel records using some specific logic.
 * Generating the target excel file which contains the result.
 * The excel file structure can be customized by JSON file.
 
+Documentation
+=============
+
+For full documentation, including installation, tutorials and PDF documents, please see https://jira-assistant.readthedocs.io/en/stable/
+
 A Simple Example
 ================
 You can run below command in the PowerShell (Windows OS) or Shell (UNIX OS) to process the excel files.
 
 .. code-block:: console
 
     process-excel-file source.xlsx
```

### Comparing `jira-assistant-0.1.7/src/jira_assistant/__init__.py` & `jira-assistant-0.1.8/src/jira_assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/src/jira_assistant/assets/excel_definition.json` & `jira-assistant-0.1.8/src/jira_assistant/assets/excel_definition.json`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/src/jira_assistant/assets/sprint_schedule.json` & `jira-assistant-0.1.8/src/jira_assistant/assets/sprint_schedule.json`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/src/jira_assistant/console_script.py` & `jira-assistant-0.1.8/src/jira_assistant/console_script.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/src/jira_assistant/excel_definition.py` & `jira-assistant-0.1.8/src/jira_assistant/excel_definition.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/src/jira_assistant/excel_operation.py` & `jira-assistant-0.1.8/src/jira_assistant/excel_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,14 @@
         and not isinstance(work_book.active, Worksheet)
     ):
         work_book.close()
         raise ValueError("The output excel file cannot be generated.")
 
     sheet: Worksheet = work_book.active
 
-    # TODO: Refactor this method to return needed properties list.
     excel_definition_columns = excel_definition.get_columns()
 
     # Use original excel column name first.
     columns = columns_in_excel
     if columns is None:
         columns = [column["name"] for column in excel_definition_columns]
 
@@ -234,24 +233,18 @@
     work_book.save(str(file))
     work_book.close()
 
 
 def _query_jira_information(
     stories: list[Story], excel_definition: ExcelDefinition
 ) -> bool:
-
     load_dotenv(ASSETS / ".env")
 
     jira_url: str | None = environ.get("JIRA_URL", default=None)
-    if (
-        # TODO: Avoid duplicate logic.
-        jira_url is None
-        or jira_url.isspace()
-        or len(jira_url) == 0
-    ):
+    if jira_url is None or jira_url.isspace() or len(jira_url) == 0:
         print(
             "The jira url is invalid. Please use the update-jira-info command to add/update url."
         )
         return False
 
     jira_acccess_token: str | None = environ.get("JIRA_ACCESS_TOKEN", default=None)
     if (
@@ -311,15 +304,15 @@
                         jira_field["jira_name"]
                     ].upper()
                 print(
                     f"Story id has been changed. Previous: {story_id.upper()}, Current: {story['storyId'].upper()}"
                 )
             else:
                 print(f"Cannot find related information for story: {story_id}")
-                story.need_sort = False  # TODO: Avoid NoneType compare issue.
+                story.need_sort = False
                 continue
 
     return True
 
 
 def run_steps_and_sort_excel_file(
     input_file: Union[str, Path],
```

### Comparing `jira-assistant-0.1.7/src/jira_assistant/jira_client.py` & `jira-assistant-0.1.8/src/jira_assistant/jira_client.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/src/jira_assistant/milestone.py` & `jira-assistant-0.1.8/src/jira_assistant/milestone.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .sprint_schedule import SprintScheduleStore
 
 __all__ = ["Milestone"]
 
 
 class Milestone:
-    # TODO: __init__ method cannot have classmethod attribute! Otherwise, all instance will point to the same one.
+    # __init__ method cannot have classmethod attribute! Otherwise, all instance will point to the same one.
     def __init__(self, raw: Any) -> None:
         self.raw: str = raw
         self.sprint = self.raw
         self.priority = 0
 
     @property
     def priority(self) -> int:
```

### Comparing `jira-assistant-0.1.7/src/jira_assistant/priority.py` & `jira-assistant-0.1.8/src/jira_assistant/priority.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/src/jira_assistant/sprint_schedule.py` & `jira-assistant-0.1.8/src/jira_assistant/sprint_schedule.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/src/jira_assistant/story.py` & `jira-assistant-0.1.8/src/jira_assistant/story.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
             return ""
         if isinstance(property_value, datetime):
             return property_value.date().isoformat()
         if isinstance(property_value, bool):
             if property_value:
                 return "Yes"
             return "No"
-        # TODO: Support customized format string in JSON.
         if isinstance(property_value, float):
             return str(property_value)
         return str(property_value)
 
     def set_value(self, property_type: Any, property_name: str, property_value: Any):
         if property_type is str:
             setattr(self, property_name, property_value)
```

### Comparing `jira-assistant-0.1.7/src/jira_assistant.egg-info/PKG-INFO` & `jira-assistant-0.1.8/src/jira_assistant.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-assistant
-Version: 0.1.7
+Version: 0.1.8
 Summary: Useful Jira tools
 Author-email: Sharry Xu <sharry.xu@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Sharry Xu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,37 +21,57 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/SharryXu/jira-assistant
-Keywords: jira,excel,jira-cloud
+Project-URL: Documentation, https://jira-assistant.readthedocs.io/en/stable
+Project-URL: Source, https://github.com/SharryXu/jira-assistant
+Project-URL: Tracker, https://github.com/SharryXu/jira-assistant/issues
+Keywords: jira,excel,sorting,project management,tool
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 6 - Mature
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Classifier: Natural Language :: English
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 Jira Assistant - userful jira tools
 =============================================
 
-|pypi| |Download| |GithubIssues| |Linux| |Windows| |Mac OS| |Pylint| |CodeQL| |Documentation| |Codecov| |CodeClimate| |License|
+|pypi| |Download| |Package Size| |GithubIssues| |Linux| |Windows| |Mac OS| |Pylint| |CodeQL| |Documentation| |Codecov| |CodeClimate| |License|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/jira-assistant.svg?style=flat-square
     :target https://pypi.org/project/jira-assistant/
     :alt: pypi version
 
 .. |Download| image:: https://static.pepy.tech/personalized-badge/jira-assistant?period=month&units=international_system&left_color=black&right_color=blue&left_text=downloads/month
     :target: https://pepy.tech/project/jira-assistant
     :alt: download
 
+.. |Package Size| image:: https://img.shields.io/github/repo-size/sharryxu/jira-assistant
+    :target: https://img.shields.io/github/repo-size/sharryxu/jira-assistant
+    :alt: Package Size
+
 .. |GitHubIssues| image:: https://img.shields.io/github/issues/sharryxu/jira-assistant
    :target: https://img.shields.io/github/issues/sharryxu/jira-assistant
    :alt: GitHub issues
 
 .. |Linux| image:: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml/badge.svg
     :target: https://github.com/SharryXu/jira-assistant/actions/workflows/python-3-11-linux-test.yml
     :alt: python 3.11 (Linux)
@@ -112,14 +132,19 @@
 ========
 
 * Parsing the excel file which usually been downloaded from the Jira platform.
 * Sorting the excel records using some specific logic.
 * Generating the target excel file which contains the result.
 * The excel file structure can be customized by JSON file.
 
+Documentation
+=============
+
+For full documentation, including installation, tutorials and PDF documents, please see https://jira-assistant.readthedocs.io/en/stable/
+
 A Simple Example
 ================
 You can run below command in the PowerShell (Windows OS) or Shell (UNIX OS) to process the excel files.
 
 .. code-block:: console
 
     process-excel-file source.xlsx
```

### Comparing `jira-assistant-0.1.7/src/jira_assistant.egg-info/SOURCES.txt` & `jira-assistant-0.1.8/src/jira_assistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/tests/test_console_script.py` & `jira-assistant-0.1.8/tests/test_console_script.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/tests/test_excel_definition.py` & `jira-assistant-0.1.8/tests/test_excel_definition.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/tests/test_excel_operation.py` & `jira-assistant-0.1.8/tests/test_excel_operation.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/tests/test_jira_client.py` & `jira-assistant-0.1.8/tests/test_jira_client.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/tests/test_milestone.py` & `jira-assistant-0.1.8/tests/test_milestone.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/tests/test_priority.py` & `jira-assistant-0.1.8/tests/test_priority.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/tests/test_sprint_schedule.py` & `jira-assistant-0.1.8/tests/test_sprint_schedule.py`

 * *Files identical despite different names*

### Comparing `jira-assistant-0.1.7/tests/test_story.py` & `jira-assistant-0.1.8/tests/test_story.py`

 * *Files identical despite different names*

