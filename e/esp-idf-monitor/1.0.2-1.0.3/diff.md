# Comparing `tmp/esp-idf-monitor-1.0.2.tar.gz` & `tmp/esp-idf-monitor-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-monitor/esp-idf-monitor/dist/.tmp-u75ro79g/esp-idf-monitor-1.0.2.tar", last modified: Mon Mar 27 15:21:15 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-monitor/esp-idf-monitor/dist/.tmp-1by69ntq/esp-idf-monitor-1.0.3.tar", last modified: Fri Apr 14 12:49:12 2023, max compression
```

## Comparing `esp-idf-monitor-1.0.2.tar` & `esp-idf-monitor-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:21:15.000000 esp-idf-monitor-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-27 15:21:15.000000 esp-idf-monitor-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:21:15.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:21:15.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/ansi_color_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/chip_specific_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/console_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/console_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/coredump.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/gdbhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/line_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/output_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/pc_address_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/serial_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/base/web_socket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/gdb_panic_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17131 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/esp_idf_monitor/idf_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:21:15.000000 esp-idf-monitor-1.0.2/esp_idf_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-27 15:21:15.000000 esp-idf-monitor-1.0.2/esp_idf_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-27 15:21:15.000000 esp-idf-monitor-1.0.2/esp_idf_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 15:21:15.000000 esp-idf-monitor-1.0.2/esp_idf_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-27 15:21:15.000000 esp-idf-monitor-1.0.2/esp_idf_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-27 15:21:15.000000 esp-idf-monitor-1.0.2/esp_idf_monitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 15:21:15.000000 esp-idf-monitor-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-27 15:20:56.000000 esp-idf-monitor-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/ansi_color_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/chip_specific_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/console_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/console_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/coredump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/gdbhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/line_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/output_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/pc_address_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/serial_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/web_socket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/gdb_panic_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17131 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/idf_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/setup.py
```

### Comparing `esp-idf-monitor-1.0.2/LICENSE` & `esp-idf-monitor-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/PKG-INFO` & `esp-idf-monitor-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-monitor
-Version: 1.0.2
+Version: 1.0.3
 Summary: Serial monitor for esp-idf
 Home-page: https://github.com/espressif/esp-idf-monitor
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,monitor,serial
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-monitor-1.0.2/README.md` & `esp-idf-monitor-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/ansi_color_converter.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/ansi_color_converter.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/argument_parser.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/argument_parser.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/chip_specific_config.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/chip_specific_config.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/console_parser.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/console_parser.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/console_reader.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/console_reader.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/constants.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 CTRL_T = '\x14'
 CTRL_Y = '\x19'
 CTRL_P = '\x10'
 CTRL_X = '\x18'
 CTRL_L = '\x0c'
 CTRL_RBRACKET = '\x1d'  # Ctrl+]
 
+# VT100 escape sequences
+CONSOLE_STATUS_QUERY = b'\x1b[5n'
+
 # Command parsed from console inputs
 CMD_STOP = 1
 CMD_RESET = 2
 CMD_MAKE = 3
 CMD_APP_FLASH = 4
 CMD_OUTPUT_TOGGLE = 5
 CMD_TOGGLE_LOGGING = 6
```

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/coredump.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/coredump.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/gdbhelper.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/gdbhelper.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/line_matcher.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/line_matcher.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/logger.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/logger.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/output_helpers.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/output_helpers.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/pc_address_matcher.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/pc_address_matcher.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/serial_handler.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/serial_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 
 from .chip_specific_config import get_chip_config
 from .console_parser import ConsoleParser, prompt_next_action  # noqa: F401
 from .console_reader import ConsoleReader  # noqa: F401
 from .constants import (CMD_APP_FLASH, CMD_ENTER_BOOT, CMD_MAKE,
                         CMD_OUTPUT_TOGGLE, CMD_RESET, CMD_STOP,
                         CMD_TOGGLE_LOGGING, CMD_TOGGLE_TIMESTAMPS,
-                        PANIC_DECODE_DISABLE, PANIC_END, PANIC_IDLE,
-                        PANIC_READING, PANIC_STACK_DUMP, PANIC_START)
+                        CONSOLE_STATUS_QUERY, PANIC_DECODE_DISABLE, PANIC_END,
+                        PANIC_IDLE, PANIC_READING, PANIC_STACK_DUMP,
+                        PANIC_START)
 from .coredump import CoreDump  # noqa: F401
 from .exceptions import SerialStopException
 from .gdbhelper import GDBHelper  # noqa: F401
 from .line_matcher import LineMatcher  # noqa: F401
 from .logger import Logger  # noqa: F401
 from .output_helpers import yellow_print
 from .serial_reader import Reader  # noqa: F401
@@ -111,14 +112,19 @@
             with coredump.check(line_strip):
                 if self._force_line_print or line_matcher.match(line_strip.decode(errors='ignore')):
                     self.logger.print(line)
                     self.compare_elf_sha256(line.decode(errors='ignore'))
                     self.logger.handle_possible_pc_address_in_line(line_strip)
             check_gdb_stub_and_run(line_strip)
             self._force_line_print = False
+
+        if self._last_line_part.startswith(CONSOLE_STATUS_QUERY):
+            self.logger.print(CONSOLE_STATUS_QUERY)
+            self._last_line_part = self._last_line_part[len(CONSOLE_STATUS_QUERY):]
+
         # Now we have the last part (incomplete line) in _last_line_part. By
         # default we don't touch it and just wait for the arrival of the rest
         # of the line. But after some time when we didn't received it we need
         # to make a decision.
         force_print_or_matched = any((
             self._force_line_print,
             (finalize_line and line_matcher.match(self._last_line_part.decode(errors='ignore')))
@@ -251,14 +257,18 @@
             if self._serial_check_exit and line.strip() == console_parser.exit_key.encode('latin-1'):
                 raise SerialStopException()
 
             self.logger.print(line)
             self.compare_elf_sha256(line.decode(errors='ignore'))
             self._force_line_print = False
 
+        if self._last_line_part.startswith(CONSOLE_STATUS_QUERY):
+            self.logger.print(CONSOLE_STATUS_QUERY)
+            self._last_line_part = self._last_line_part[len(CONSOLE_STATUS_QUERY):]
+
         force_print_or_matched = any((
             self._force_line_print,
             (finalize_line and line_matcher.match(self._last_line_part.decode(errors='ignore')))
         ))
 
         if self._last_line_part != b'' and force_print_or_matched:
             self._force_line_print = True
```

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/serial_reader.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/serial_reader.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/stoppable_thread.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/base/web_socket_client.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/base/web_socket_client.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/gdb_panic_server.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/gdb_panic_server.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor/idf_monitor.py` & `esp-idf-monitor-1.0.3/esp_idf_monitor/idf_monitor.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor.egg-info/PKG-INFO` & `esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-monitor
-Version: 1.0.2
+Version: 1.0.3
 Summary: Serial monitor for esp-idf
 Home-page: https://github.com/espressif/esp-idf-monitor
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,monitor,serial
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-monitor-1.0.2/esp_idf_monitor.egg-info/SOURCES.txt` & `esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.2/setup.py` & `esp-idf-monitor-1.0.3/setup.py`

 * *Files identical despite different names*

