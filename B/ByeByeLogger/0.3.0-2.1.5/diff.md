# Comparing `tmp/ByeByeLogger-0.3.0.tar.gz` & `tmp/ByeByeLogger-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ByeByeLogger-0.3.0.tar", last modified: Fri Apr 14 11:27:54 2023, max compression
+gzip compressed data, was "ByeByeLogger-2.1.5.tar", last modified: Fri Apr 14 13:11:46 2023, max compression
```

## Comparing `ByeByeLogger-0.3.0.tar` & `ByeByeLogger-2.1.5.tar`

### file list

```diff
@@ -1,28 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.996265 ByeByeLogger-0.3.0/
--rw-rw-rw-   0        0        0     1159 2023-04-14 11:27:54.995266 ByeByeLogger-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-04-14 09:14:53.000000 ByeByeLogger-0.3.0/README.md
--rw-rw-rw-   0        0        0      959 2023-04-14 11:26:40.000000 ByeByeLogger-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 11:27:54.996265 ByeByeLogger-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.944265 ByeByeLogger-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.968279 ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/
--rw-rw-rw-   0        0        0     1159 2023-04-14 11:27:54.000000 ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2023-04-14 11:27:54.000000 ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 11:27:54.000000 ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-14 11:27:54.000000 ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-14 11:27:54.000000 ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.970271 ByeByeLogger-0.3.0/src/byebyelogger/
--rw-rw-rw-   0        0        0        0 2023-04-11 17:13:48.000000 ByeByeLogger-0.3.0/src/byebyelogger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.984264 ByeByeLogger-0.3.0/src/byebyelogger/core/
--rw-rw-rw-   0        0        0      154 2023-04-14 11:26:03.000000 ByeByeLogger-0.3.0/src/byebyelogger/core/ByeByeLogger.py
--rw-rw-rw-   0        0        0        0 2023-04-13 15:02:15.000000 ByeByeLogger-0.3.0/src/byebyelogger/core/__init__.py
--rw-rw-rw-   0        0        0      425 2023-04-14 08:52:54.000000 ByeByeLogger-0.3.0/src/byebyelogger/core/abstract.py
--rw-rw-rw-   0        0        0     1968 2023-04-14 08:45:06.000000 ByeByeLogger-0.3.0/src/byebyelogger/core/repository.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.988263 ByeByeLogger-0.3.0/src/byebyelogger/presets/
--rw-rw-rw-   0        0        0        0 2023-04-13 15:05:43.000000 ByeByeLogger-0.3.0/src/byebyelogger/presets/__init__.py
--rw-rw-rw-   0        0        0     1579 2023-04-14 11:23:02.000000 ByeByeLogger-0.3.0/src/byebyelogger/presets/datascience.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.992264 ByeByeLogger-0.3.0/src/byebyelogger/style/
--rw-rw-rw-   0        0        0        0 2023-04-14 11:23:20.000000 ByeByeLogger-0.3.0/src/byebyelogger/style/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-04-14 06:36:00.000000 ByeByeLogger-0.3.0/src/byebyelogger/style/colorizer.py
--rw-rw-rw-   0        0        0      500 2023-04-13 15:17:12.000000 ByeByeLogger-0.3.0/src/byebyelogger/style/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.994263 ByeByeLogger-0.3.0/tests/
--rw-rw-rw-   0        0        0      217 2023-04-14 08:52:33.000000 ByeByeLogger-0.3.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:11:46.159439 ByeByeLogger-2.1.5/
+-rw-rw-rw-   0        0        0      978 2023-04-14 13:11:46.159439 ByeByeLogger-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:11:46.160442 ByeByeLogger-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      964 2023-04-14 13:11:43.000000 ByeByeLogger-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:11:46.124441 ByeByeLogger-2.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 13:11:46.142438 ByeByeLogger-2.1.5/src/ByeByeLogger.egg-info/
+-rw-rw-rw-   0        0        0      978 2023-04-14 13:11:45.000000 ByeByeLogger-2.1.5/src/ByeByeLogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-04-14 13:11:45.000000 ByeByeLogger-2.1.5/src/ByeByeLogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:11:45.000000 ByeByeLogger-2.1.5/src/ByeByeLogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-14 13:11:45.000000 ByeByeLogger-2.1.5/src/ByeByeLogger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 13:11:45.000000 ByeByeLogger-2.1.5/src/ByeByeLogger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 13:11:46.144441 ByeByeLogger-2.1.5/src/byebyelogger/
+-rw-rw-rw-   0        0        0      496 2023-04-14 12:46:34.000000 ByeByeLogger-2.1.5/src/byebyelogger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:11:46.151441 ByeByeLogger-2.1.5/src/byebyelogger/core/
+-rw-rw-rw-   0        0        0        0 2023-04-13 15:02:15.000000 ByeByeLogger-2.1.5/src/byebyelogger/core/__init__.py
+-rw-rw-rw-   0        0        0     1692 2023-04-14 12:54:13.000000 ByeByeLogger-2.1.5/src/byebyelogger/core/datascience.py
+-rw-rw-rw-   0        0        0     1898 2023-04-14 12:53:47.000000 ByeByeLogger-2.1.5/src/byebyelogger/core/repository.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:11:46.157441 ByeByeLogger-2.1.5/src/byebyelogger/style/
+-rw-rw-rw-   0        0        0        0 2023-04-14 11:23:20.000000 ByeByeLogger-2.1.5/src/byebyelogger/style/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-04-14 06:36:00.000000 ByeByeLogger-2.1.5/src/byebyelogger/style/colorizer.py
+-rw-rw-rw-   0        0        0      500 2023-04-13 15:17:12.000000 ByeByeLogger-2.1.5/src/byebyelogger/style/constants.py
```

### Comparing `ByeByeLogger-0.3.0/PKG-INFO` & `ByeByeLogger-2.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: ByeByeLogger
-Version: 0.3.0
+Version: 2.1.5
 Summary: A simple, yet powerful Python logging library that makes you say goodbye to your standard logger.
-Author-email: Aleksa Lukic <aleksalukic92@web.de>
-Project-URL: Homepage, https://github.com/N4r0Bs/ByeByeLogger
-Project-URL: Repository, https://github.com/N4r0Bs/ByeByeLogger
+Author: Aleksa Lukic
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # ByeByeLogger
 
 ### Oh, great! Another logging package, because obviously, we need more of those, right? Well, let me introduce you to ByeByeLogger, the one that's going to make you say goodbye to your current logger (whether you like it or not).
```

### Comparing `ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/PKG-INFO` & `ByeByeLogger-2.1.5/src/ByeByeLogger.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: ByeByeLogger
-Version: 0.3.0
+Version: 2.1.5
 Summary: A simple, yet powerful Python logging library that makes you say goodbye to your standard logger.
-Author-email: Aleksa Lukic <aleksalukic92@web.de>
-Project-URL: Homepage, https://github.com/N4r0Bs/ByeByeLogger
-Project-URL: Repository, https://github.com/N4r0Bs/ByeByeLogger
+Author: Aleksa Lukic
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # ByeByeLogger
 
 ### Oh, great! Another logging package, because obviously, we need more of those, right? Well, let me introduce you to ByeByeLogger, the one that's going to make you say goodbye to your current logger (whether you like it or not).
```

### Comparing `ByeByeLogger-0.3.0/src/byebyelogger/core/repository.py` & `ByeByeLogger-2.1.5/src/byebyelogger/core/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Protocol, List, Dict, Tuple, Callable, Union
 from dataclasses import dataclass, field
 
-from core.abstract import AbstractLoggingRepository
 
 @dataclass
 class CustomLogger:
     attributes: Dict[str, Tuple[Union[str, Callable], str]] = field(default_factory=dict)
     order: List[str] = field(default_factory=list)
     separator: str = " - "
     default_style: str = ""
@@ -47,15 +46,16 @@
         log_entry = self.separator.join(formatted_attributes)
         print(log_entry, end=" ")
 
 class Loggable(Protocol):
     def log(self):
         pass
 
-class LogRepository(AbstractLoggingRepository):
+class LogRepository:
 
     def __init__(self, logging: Loggable):
         self.logging = logging
 
     def log(self, msg: str):
         self.logging.log()
-        print(msg)
+        print(msg)
+
```

### Comparing `ByeByeLogger-0.3.0/src/byebyelogger/presets/datascience.py` & `ByeByeLogger-2.1.5/src/byebyelogger/core/datascience.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
-from core.repository import CustomLogger, LogRepository
+from byebyelogger.core.repository import CustomLogger, LogRepository
 
-from style.colorizer import LIGHTCYAN_EX, LIGHTGREEN_EX, LIGHTRED_EX
-from style.constants import SQUARE_BRACKETS
+from byebyelogger.style.colorizer import LIGHTCYAN_EX, LIGHTGREEN_EX, LIGHTRED_EX
+from byebyelogger.style.constants import SQUARE_BRACKETS
 
 def get_class_name_from_stack():
     stack = inspect.stack()
     for frame_info in reversed(stack):
         frame = frame_info.frame
         if 'self' in frame.f_locals:
             name = frame.f_locals['self'].__class__.__name__
@@ -32,11 +32,14 @@
 custom.add(name="method_name", value=lambda: get_method_name_from_stack())
 custom.add(name="level", value="INFO")
 
 
 PRESET_INFO = custom.copy()
 PRESET_INFO.attributes["level"] = (LIGHTCYAN_EX("INFO"), SQUARE_BRACKETS)
 
+INFO = LogRepository(PRESET_INFO)
 
 PRESET_ERROR = custom.copy()
 PRESET_ERROR.attributes["level"] = (LIGHTRED_EX("ERROR"), SQUARE_BRACKETS)
 
+ERROR = LogRepository(PRESET_ERROR)
+
```

### Comparing `ByeByeLogger-0.3.0/src/byebyelogger/style/colorizer.py` & `ByeByeLogger-2.1.5/src/byebyelogger/style/colorizer.py`

 * *Files identical despite different names*

