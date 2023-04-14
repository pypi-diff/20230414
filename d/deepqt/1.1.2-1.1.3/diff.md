# Comparing `tmp/deepqt-1.1.2.tar.gz` & `tmp/deepqt-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepqt-1.1.2.tar", last modified: Mon Apr  3 01:57:25 2023, max compression
+gzip compressed data, was "deepqt-1.1.3.tar", last modified: Fri Apr 14 15:59:17 2023, max compression
```

## Comparing `deepqt-1.1.2.tar` & `deepqt-1.1.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-03 01:57:25.044207 deepqt-1.1.2/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2022-08-22 17:31:33.000000 deepqt-1.1.2/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-03 01:57:25.044207 deepqt-1.1.2/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1822 2022-10-03 21:56:52.000000 deepqt-1.1.2/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-03 01:57:25.044207 deepqt-1.1.2/deepqt/
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-03 01:57:25.044207 deepqt-1.1.2/deepqt/CustomQ/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1027 2022-08-23 23:21:07.000000 deepqt-1.1.2/deepqt/CustomQ/CComboBox.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3206 2022-08-27 14:37:25.000000 deepqt-1.1.2/deepqt/CustomQ/CTableWidget.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2021-11-04 23:10:16.000000 deepqt-1.1.2/deepqt/CustomQ/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)       95 2023-04-03 01:56:30.000000 deepqt-1.1.2/deepqt/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    18001 2022-10-03 22:02:43.000000 deepqt-1.1.2/deepqt/api_interface.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5447 2022-10-14 20:43:00.000000 deepqt-1.1.2/deepqt/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1706 2022-10-14 20:43:00.000000 deepqt-1.1.2/deepqt/driver_api_config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4980 2022-10-03 21:56:52.000000 deepqt-1.1.2/deepqt/driver_epub_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    34986 2023-04-03 00:53:22.000000 deepqt-1.1.2/deepqt/driver_mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3171 2022-10-03 21:56:52.000000 deepqt-1.1.2/deepqt/driver_text_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20199 2023-04-03 01:29:33.000000 deepqt-1.1.2/deepqt/file_table.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7574 2022-11-29 16:04:36.000000 deepqt-1.1.2/deepqt/glossary.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6260 2022-10-03 21:56:52.000000 deepqt-1.1.2/deepqt/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3169 2023-04-03 01:56:09.000000 deepqt-1.1.2/deepqt/main.py
--rwxr-xr-x   0 corbin    (1000) corbin    (1001)     3559 2022-08-31 20:58:56.000000 deepqt-1.1.2/deepqt/quote_protection.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-03 01:57:25.044207 deepqt-1.1.2/deepqt/rc_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-09-02 14:05:58.000000 deepqt-1.1.2/deepqt/rc_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    87635 2022-10-03 21:56:52.000000 deepqt-1.1.2/deepqt/rc_generated_files/fallback_icons_rc.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    16395 2023-04-03 00:54:10.000000 deepqt-1.1.2/deepqt/structures.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5151 2022-10-03 21:56:52.000000 deepqt-1.1.2/deepqt/term_extractor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1846 2022-09-07 01:14:43.000000 deepqt-1.1.2/deepqt/trie.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-03 01:57:25.044207 deepqt-1.1.2/deepqt/ui_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-08-23 11:40:40.000000 deepqt-1.1.2/deepqt/ui_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2579 2022-10-14 20:41:09.000000 deepqt-1.1.2/deepqt/ui_generated_files/ui_api_config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5604 2022-09-06 01:28:45.000000 deepqt-1.1.2/deepqt/ui_generated_files/ui_epub_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    24110 2022-10-03 21:56:52.000000 deepqt-1.1.2/deepqt/ui_generated_files/ui_mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2687 2022-08-26 16:44:10.000000 deepqt-1.1.2/deepqt/ui_generated_files/ui_text_preview.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3203 2022-10-03 21:56:52.000000 deepqt-1.1.2/deepqt/worker_thread.py
--rwxr-xr-x   0 corbin    (1000) corbin    (1001)    10809 2022-10-03 21:56:52.000000 deepqt-1.1.2/deepqt/xml_parser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-03 01:57:25.044207 deepqt-1.1.2/deepqt.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-03 01:57:25.000000 deepqt-1.1.2/deepqt.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1000 2023-04-03 01:57:25.000000 deepqt-1.1.2/deepqt.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-03 01:57:25.000000 deepqt-1.1.2/deepqt.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       44 2023-04-03 01:57:25.000000 deepqt-1.1.2/deepqt.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      118 2023-04-03 01:57:25.000000 deepqt-1.1.2/deepqt.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        7 2023-04-03 01:57:25.000000 deepqt-1.1.2/deepqt.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2022-09-01 16:09:10.000000 deepqt-1.1.2/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)      865 2023-04-03 01:57:25.047541 deepqt-1.1.2/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2022-09-01 20:32:32.000000 deepqt-1.1.2/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 15:59:17.837984 deepqt-1.1.3/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2022-08-22 17:31:33.000000 deepqt-1.1.3/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-14 15:59:17.837984 deepqt-1.1.3/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1822 2022-10-03 21:56:52.000000 deepqt-1.1.3/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 15:59:17.834651 deepqt-1.1.3/deepqt/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 15:59:17.837984 deepqt-1.1.3/deepqt/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1027 2022-08-23 23:21:07.000000 deepqt-1.1.3/deepqt/CustomQ/CComboBox.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3206 2022-08-27 14:37:25.000000 deepqt-1.1.3/deepqt/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2021-11-04 23:10:16.000000 deepqt-1.1.3/deepqt/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       95 2023-04-14 15:57:00.000000 deepqt-1.1.3/deepqt/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    18001 2022-10-03 22:02:43.000000 deepqt-1.1.3/deepqt/api_interface.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5701 2023-04-14 15:55:16.000000 deepqt-1.1.3/deepqt/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1706 2022-10-14 20:43:00.000000 deepqt-1.1.3/deepqt/driver_api_config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4980 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/driver_epub_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    34986 2023-04-03 00:53:22.000000 deepqt-1.1.3/deepqt/driver_mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3171 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/driver_text_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20199 2023-04-03 01:29:33.000000 deepqt-1.1.3/deepqt/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7574 2022-11-29 16:04:36.000000 deepqt-1.1.3/deepqt/glossary.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6260 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3202 2023-04-14 15:56:08.000000 deepqt-1.1.3/deepqt/main.py
+-rwxr-xr-x   0 corbin    (1000) corbin    (1001)     3559 2022-08-31 20:58:56.000000 deepqt-1.1.3/deepqt/quote_protection.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 15:59:17.837984 deepqt-1.1.3/deepqt/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-09-02 14:05:58.000000 deepqt-1.1.3/deepqt/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    87635 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/rc_generated_files/fallback_icons_rc.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    16395 2023-04-03 00:54:10.000000 deepqt-1.1.3/deepqt/structures.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5151 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/term_extractor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1846 2022-09-07 01:14:43.000000 deepqt-1.1.3/deepqt/trie.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 15:59:17.837984 deepqt-1.1.3/deepqt/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-08-23 11:40:40.000000 deepqt-1.1.3/deepqt/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2579 2022-10-14 20:41:09.000000 deepqt-1.1.3/deepqt/ui_generated_files/ui_api_config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5604 2022-09-06 01:28:45.000000 deepqt-1.1.3/deepqt/ui_generated_files/ui_epub_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    24110 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/ui_generated_files/ui_mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2687 2022-08-26 16:44:10.000000 deepqt-1.1.3/deepqt/ui_generated_files/ui_text_preview.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3203 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/worker_thread.py
+-rwxr-xr-x   0 corbin    (1000) corbin    (1001)    10809 2022-10-03 21:56:52.000000 deepqt-1.1.3/deepqt/xml_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 15:59:17.837984 deepqt-1.1.3/deepqt.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2389 2023-04-14 15:59:17.000000 deepqt-1.1.3/deepqt.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1000 2023-04-14 15:59:17.000000 deepqt-1.1.3/deepqt.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-14 15:59:17.000000 deepqt-1.1.3/deepqt.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       44 2023-04-14 15:59:17.000000 deepqt-1.1.3/deepqt.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      118 2023-04-14 15:59:17.000000 deepqt-1.1.3/deepqt.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        7 2023-04-14 15:59:17.000000 deepqt-1.1.3/deepqt.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2022-09-01 16:09:10.000000 deepqt-1.1.3/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      865 2023-04-14 15:59:17.837984 deepqt-1.1.3/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2022-09-01 20:32:32.000000 deepqt-1.1.3/setup.py
```

### Comparing `deepqt-1.1.2/LICENSE` & `deepqt-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/PKG-INFO` & `deepqt-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepqt
-Version: 1.1.2
+Version: 1.1.3
 Summary: Harness the power of the DeepL API with this friendly user interface.
 Home-page: https://github.com/VoxelCubes/DeepQt
 Keywords: deepl,deepl api,qt,pyside6
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `deepqt-1.1.2/README.md` & `deepqt-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/CustomQ/CComboBox.py` & `deepqt-1.1.3/deepqt/CustomQ/CComboBox.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/CustomQ/CTableWidget.py` & `deepqt-1.1.3/deepqt/CustomQ/CTableWidget.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/api_interface.py` & `deepqt-1.1.3/deepqt/api_interface.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/config.py` & `deepqt-1.1.3/deepqt/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,28 +102,32 @@
     """
     if platform.system() == "Linux":
         from xdg import XDG_CONFIG_HOME
 
         return Path(XDG_CONFIG_HOME, __program__.lower() + "rc")
     elif platform.system() == "Windows":
         return Path(os.getenv("APPDATA"), __program__.lower(), "config.ini")
+    elif platform.system() == "Darwin":
+        return Path(os.getenv("HOME"), "Library", "Preferences", __program__.lower() + "rc")
     else:  # ???
         raise NotImplementedError("Your OS is currently not supported.")
 
 
 def cache_path() -> Path:
     """
     Get the path to the cache directory.
     """
     if platform.system() == "Linux":
         from xdg import XDG_CACHE_HOME
 
         return Path(XDG_CACHE_HOME, __program__.lower())
     elif platform.system() == "Windows":
         return Path(os.getenv("APPDATA"), __program__.lower())
+    elif platform.system() == "Darwin":
+        return Path(os.getenv("HOME"), "Library", "Caches", __program__.lower())
     else:  # ???
         raise NotImplementedError("Your OS is currently not supported.")
 
 
 def epub_cache_path(epub_path: None | Path = None) -> Path:
     """
     Get the path to the epub cache directory for this epub.
```

### Comparing `deepqt-1.1.2/deepqt/driver_api_config.py` & `deepqt-1.1.3/deepqt/driver_api_config.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/driver_epub_preview.py` & `deepqt-1.1.3/deepqt/driver_epub_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/driver_mainwindow.py` & `deepqt-1.1.3/deepqt/driver_mainwindow.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/driver_text_preview.py` & `deepqt-1.1.3/deepqt/driver_text_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/file_table.py` & `deepqt-1.1.3/deepqt/file_table.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/glossary.py` & `deepqt-1.1.3/deepqt/glossary.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/helpers.py` & `deepqt-1.1.3/deepqt/helpers.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/main.py` & `deepqt-1.1.3/deepqt/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             logger.info("Using Breeze icon theme.")
             Qg.QIcon.setThemeName("Breeze")
         elif args.icon_theme == "BreezeDark":
             logger.info("Using BreezeDark icon theme.")
             Qg.QIcon.setThemeName("BreezeDark")
         else:
             raise ValueError(f"Unknown icon theme: {args.icon_theme}")
-    elif platform.system() == "Windows":
+    elif platform.system() == "Windows" or platform.system() == "Darwin":
         # Default to Breeze on Windows.
         logger.info("Using Breeze icon theme.")
         Qg.QIcon.setThemeName("Breeze")
 
     # Start the main window.
     app = Qw.QApplication(sys.argv)
```

### Comparing `deepqt-1.1.2/deepqt/quote_protection.py` & `deepqt-1.1.3/deepqt/quote_protection.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/rc_generated_files/fallback_icons_rc.py` & `deepqt-1.1.3/deepqt/rc_generated_files/fallback_icons_rc.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/structures.py` & `deepqt-1.1.3/deepqt/structures.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/term_extractor.py` & `deepqt-1.1.3/deepqt/term_extractor.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/trie.py` & `deepqt-1.1.3/deepqt/trie.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/ui_generated_files/ui_api_config.py` & `deepqt-1.1.3/deepqt/ui_generated_files/ui_api_config.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/ui_generated_files/ui_epub_preview.py` & `deepqt-1.1.3/deepqt/ui_generated_files/ui_epub_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/ui_generated_files/ui_mainwindow.py` & `deepqt-1.1.3/deepqt/ui_generated_files/ui_mainwindow.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/ui_generated_files/ui_text_preview.py` & `deepqt-1.1.3/deepqt/ui_generated_files/ui_text_preview.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/worker_thread.py` & `deepqt-1.1.3/deepqt/worker_thread.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt/xml_parser.py` & `deepqt-1.1.3/deepqt/xml_parser.py`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/deepqt.egg-info/PKG-INFO` & `deepqt-1.1.3/deepqt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepqt
-Version: 1.1.2
+Version: 1.1.3
 Summary: Harness the power of the DeepL API with this friendly user interface.
 Home-page: https://github.com/VoxelCubes/DeepQt
 Keywords: deepl,deepl api,qt,pyside6
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `deepqt-1.1.2/deepqt.egg-info/SOURCES.txt` & `deepqt-1.1.3/deepqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepqt-1.1.2/setup.cfg` & `deepqt-1.1.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deepqt
-version = 1.1.2
+version = 1.1.3
 description = Harness the power of the DeepL API with this friendly user interface.
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/VoxelCubes/DeepQt
 keywords = deepl, deepl api, qt, pyside6
 license_files = LICENSE
 classifiers =
```

