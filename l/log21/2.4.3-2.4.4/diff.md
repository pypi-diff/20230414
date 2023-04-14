# Comparing `tmp/log21-2.4.3.tar.gz` & `tmp/log21-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log21-2.4.3.tar", last modified: Thu Apr  6 08:26:28 2023, max compression
+gzip compressed data, was "log21-2.4.4.tar", last modified: Fri Apr 14 18:35:28 2023, max compression
```

## Comparing `log21-2.4.3.tar` & `log21-2.4.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:26:28.672809 log21-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-06 08:26:19.000000 log21-2.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-04-06 08:26:28.672809 log21-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-06 08:26:19.000000 log21-2.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:26:28.672809 log21-2.4.3/log21/
--rw-r--r--   0 runner    (1001) docker     (123)    21618 2023-04-06 08:26:19.000000 log21-2.4.3/log21/Argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-06 08:26:19.000000 log21-2.4.3/log21/Colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:26:28.672809 log21-2.4.3/log21/CrashReporter/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-06 08:26:19.000000 log21-2.4.3/log21/CrashReporter/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-06 08:26:19.000000 log21-2.4.3/log21/CrashReporter/Reporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-06 08:26:19.000000 log21-2.4.3/log21/CrashReporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-06 08:26:19.000000 log21-2.4.3/log21/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-04-06 08:26:19.000000 log21-2.4.3/log21/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-06 08:26:19.000000 log21-2.4.3/log21/Levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-04-06 08:26:19.000000 log21-2.4.3/log21/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-04-06 08:26:19.000000 log21-2.4.3/log21/LoggingWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-06 08:26:19.000000 log21-2.4.3/log21/Manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-04-06 08:26:19.000000 log21-2.4.3/log21/PPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-04-06 08:26:19.000000 log21-2.4.3/log21/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-06 08:26:19.000000 log21-2.4.3/log21/StreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-06 08:26:19.000000 log21-2.4.3/log21/TreePrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20787 2023-04-06 08:26:19.000000 log21-2.4.3/log21/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:26:28.672809 log21-2.4.3/log21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-04-06 08:26:28.000000 log21-2.4.3/log21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-06 08:26:28.000000 log21-2.4.3/log21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:26:28.000000 log21-2.4.3/log21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 08:26:28.000000 log21-2.4.3/log21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-06 08:26:28.000000 log21-2.4.3/log21.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 08:26:28.672809 log21-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-06 08:26:19.000000 log21-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:35:28.828293 log21-2.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-14 18:35:20.000000 log21-2.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10104 2023-04-14 18:35:28.828293 log21-2.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-04-14 18:35:20.000000 log21-2.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:35:28.828293 log21-2.4.4/log21/
+-rw-r--r--   0 runner    (1001) docker     (123)    21618 2023-04-14 18:35:20.000000 log21-2.4.4/log21/Argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-14 18:35:20.000000 log21-2.4.4/log21/Colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:35:28.828293 log21-2.4.4/log21/CrashReporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-14 18:35:20.000000 log21-2.4.4/log21/CrashReporter/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-14 18:35:20.000000 log21-2.4.4/log21/CrashReporter/Reporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 18:35:20.000000 log21-2.4.4/log21/CrashReporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-14 18:35:20.000000 log21-2.4.4/log21/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-04-14 18:35:20.000000 log21-2.4.4/log21/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-14 18:35:20.000000 log21-2.4.4/log21/Levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-04-14 18:35:20.000000 log21-2.4.4/log21/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-04-14 18:35:20.000000 log21-2.4.4/log21/LoggingWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-14 18:35:20.000000 log21-2.4.4/log21/Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-04-14 18:35:20.000000 log21-2.4.4/log21/PPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-04-14 18:35:20.000000 log21-2.4.4/log21/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-14 18:35:20.000000 log21-2.4.4/log21/StreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-14 18:35:20.000000 log21-2.4.4/log21/TreePrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20803 2023-04-14 18:35:20.000000 log21-2.4.4/log21/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:35:28.828293 log21-2.4.4/log21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10104 2023-04-14 18:35:28.000000 log21-2.4.4/log21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-14 18:35:28.000000 log21-2.4.4/log21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:35:28.000000 log21-2.4.4/log21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 18:35:28.000000 log21-2.4.4/log21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 18:35:28.000000 log21-2.4.4/log21.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:35:28.828293 log21-2.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-14 18:35:20.000000 log21-2.4.4/setup.py
```

### Comparing `log21-2.4.3/LICENSE.txt` & `log21-2.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/PKG-INFO` & `log21-2.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.4.3
+Version: 2.4.4
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Home-page: https://github.com/MPCodeWriter21/log21
 Author: CodeWriter21(Mehrad Pooryoussof)
 Author-email: <CodeWriter21@gmail.com>
 License: Apache-2.0 License
 Keywords: python,log,colorize,color,logging
 Classifier: Intended Audience :: Developers
@@ -29,15 +29,15 @@
 A simple logging package that helps you log colorized messages in Windows console and other operating systems.
 
 Features
 --------
 
 + Colors : The main reason for this package was to log text in the Windows console with the support of ANSI colors.
 + Argument parsing : log21's argument parser can be used like python's argparse but it also colorizes the output.
-+ Logging : A similar logger to logging.Logger but with colorized output and other options such as levelname
++ Logging : A similar logger to logging. Logger but with colorized output and other options such as levelname
   modifications. It can also decolorize the output if you want to log into a file.
 + Pretty printing : Have you ever wanted to colorize the output of the pprint module? log21's pretty printer can do
   that.
 + Tree printing : You can pass a dict or list to log21.tree_print function and it will print it in a tree-like
   structure. It's also colorized XD.
 + ProgressBar : log21's progress bar can be used to show progress of a process in a beautiful way.
 + LoggingWindow : Helps you to log messages and debug your code in a window other than the console.
@@ -68,17 +68,17 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.3
+### 2.4.4
 
-Improvements.
+Some bug fixes.
 
 [Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.4.3/README.md` & `log21-2.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 A simple logging package that helps you log colorized messages in Windows console and other operating systems.
 
 Features
 --------
 
 + Colors : The main reason for this package was to log text in the Windows console with the support of ANSI colors.
 + Argument parsing : log21's argument parser can be used like python's argparse but it also colorizes the output.
-+ Logging : A similar logger to logging.Logger but with colorized output and other options such as levelname
++ Logging : A similar logger to logging. Logger but with colorized output and other options such as levelname
   modifications. It can also decolorize the output if you want to log into a file.
 + Pretty printing : Have you ever wanted to colorize the output of the pprint module? log21's pretty printer can do
   that.
 + Tree printing : You can pass a dict or list to log21.tree_print function and it will print it in a tree-like
   structure. It's also colorized XD.
 + ProgressBar : log21's progress bar can be used to show progress of a process in a beautiful way.
 + LoggingWindow : Helps you to log messages and debug your code in a window other than the console.
@@ -49,17 +49,17 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.3
+### 2.4.4
 
-Improvements.
+Some bug fixes.
 
 [Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.4.3/log21/Argparse.py` & `log21-2.4.4/log21/Argparse.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/log21/Colors.py` & `log21-2.4.4/log21/Colors.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/log21/CrashReporter/Formatters.py` & `log21-2.4.4/log21/CrashReporter/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/log21/CrashReporter/Reporters.py` & `log21-2.4.4/log21/CrashReporter/Reporters.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/log21/FileHandler.py` & `log21-2.4.4/log21/FileHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/log21/Formatters.py` & `log21-2.4.4/log21/Formatters.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from log21.Colors import get_colors as _gc, ansi_escape
 from log21.Levels import INPUT, CRITICAL, ERROR, WARNING, INFO, DEBUG, PRINT
 
 __all__ = ['ColorizingFormatter', 'DecolorizingFormatter']
 
 
 class _Formatter(__Formatter):
-    level_names: _Dict[int, str] = {
+    _level_names: _Dict[int, str] = {
         DEBUG: 'DEBUG',
         INFO: 'INFO',
         WARNING: 'WARNING',
         ERROR: 'ERROR',
         CRITICAL: 'CRITICAL',
         PRINT: 'PRINT',
         INPUT: 'INPUT'
@@ -48,14 +48,27 @@
         >>>
         """
         super().__init__(fmt=fmt, datefmt=datefmt, style=style)
         if level_names:
             for level, name in level_names.items():
                 self.level_names[level] = name
 
+    @property
+    def level_names(self):
+        return self._level_names
+
+    @level_names.setter
+    def level_names(self, level_names):
+        if level_names:
+            if not isinstance(level_names, _Dict):
+                raise TypeError('`level_names` must be a dictionary!')
+            self._level_names = level_names
+        else:
+            self._level_names = dict()
+
     def format(self, record) -> str:
         record.message = record.getMessage()
         if self.usesTime():
             record.asctime = self.formatTime(record, self.datefmt)
 
         record.levelname = self.level_names.get(record.levelno, 'NOTSET')
```

### Comparing `log21-2.4.3/log21/Logger.py` & `log21-2.4.4/log21/Logger.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/log21/LoggingWindow.py` & `log21-2.4.4/log21/LoggingWindow.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/log21/Manager.py` & `log21-2.4.4/log21/Manager.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/log21/PPrint.py` & `log21-2.4.4/log21/PPrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/log21/ProgressBar.py` & `log21-2.4.4/log21/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/log21/StreamHandler.py` & `log21-2.4.4/log21/StreamHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/log21/TreePrint.py` & `log21-2.4.4/log21/TreePrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/log21/__init__.py` & `log21-2.4.4/log21/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from log21.Argparse import ColorizingArgumentParser
 from log21.FileHandler import DecolorizingFileHandler
 from log21.LoggingWindow import LoggingWindow, LoggingWindowHandler
 from log21.StreamHandler import ColorizingStreamHandler, StreamHandler
 from log21.Formatters import ColorizingFormatter, DecolorizingFormatter
 from log21.Colors import Colors, get_color, get_colors, ansi_escape, get_color_name, closest_color
 
-__version__ = "2.4.3"
+__version__ = "2.4.4"
 __author__ = "CodeWriter21 (Mehrad Pooryoussof)"
 __github__ = "Https://GitHub.com/MPCodeWriter21/log21"
 __all__ = ['ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter', 'DecolorizingFormatter',
            'get_logger', 'Logger', 'Colors', 'get_color', 'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN',
            'INFO', 'DEBUG', 'NOTSET', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter', 'pformat',
            'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager', 'get_color_name', 'closest_color',
            'ansi_escape', '__version__', '__author__', '__github__', 'debug', 'info', 'warning', 'warn', 'error',
@@ -49,15 +49,15 @@
         if show_level:
             fmt = "[%(levelname)s] " + fmt
         if show_time:
             fmt = "[%(asctime)s] " + fmt
         fmt = '\r' + fmt
     # Defines the formatter
     formatter = formatter_class(fmt, datefmt, style=style)
-    if isinstance(formatter, Formatters._Formatter):
+    if isinstance(formatter, Formatters._Formatter) and level_names:
         formatter.level_names = level_names
     if not colorize_time_and_level and isinstance(formatter, ColorizingFormatter):
         for key in formatter.level_colors:
             formatter.level_colors[key] = tuple()
         formatter.time_color = tuple()
 
     return formatter
```

### Comparing `log21-2.4.3/log21.egg-info/PKG-INFO` & `log21-2.4.4/log21.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.4.3
+Version: 2.4.4
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Home-page: https://github.com/MPCodeWriter21/log21
 Author: CodeWriter21(Mehrad Pooryoussof)
 Author-email: <CodeWriter21@gmail.com>
 License: Apache-2.0 License
 Keywords: python,log,colorize,color,logging
 Classifier: Intended Audience :: Developers
@@ -29,15 +29,15 @@
 A simple logging package that helps you log colorized messages in Windows console and other operating systems.
 
 Features
 --------
 
 + Colors : The main reason for this package was to log text in the Windows console with the support of ANSI colors.
 + Argument parsing : log21's argument parser can be used like python's argparse but it also colorizes the output.
-+ Logging : A similar logger to logging.Logger but with colorized output and other options such as levelname
++ Logging : A similar logger to logging. Logger but with colorized output and other options such as levelname
   modifications. It can also decolorize the output if you want to log into a file.
 + Pretty printing : Have you ever wanted to colorize the output of the pprint module? log21's pretty printer can do
   that.
 + Tree printing : You can pass a dict or list to log21.tree_print function and it will print it in a tree-like
   structure. It's also colorized XD.
 + ProgressBar : log21's progress bar can be used to show progress of a process in a beautiful way.
 + LoggingWindow : Helps you to log messages and debug your code in a window other than the console.
@@ -68,17 +68,17 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.3
+### 2.4.4
 
-Improvements.
+Some bug fixes.
 
 [Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.4.3/log21.egg-info/SOURCES.txt` & `log21-2.4.4/log21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `log21-2.4.3/setup.py` & `log21-2.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 DESCRIPTION = 'A simple logging package that helps you log colorized messages in Windows console.'
-VERSION = '2.4.3'
+VERSION = '2.4.4'
 
 setup(
     name='log21',
     version=VERSION,
     url='https://github.com/MPCodeWriter21/log21',
     author='CodeWriter21(Mehrad Pooryoussof)',
     author_email='<CodeWriter21@gmail.com>',
```

