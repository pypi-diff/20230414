# Comparing `tmp/pyautogui_simplified_edition-1.0a1.tar.gz` & `tmp/pyautogui_simplified_edition-1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautogui_simplified_edition-1.0a1.tar", last modified: Fri Apr 14 15:23:27 2023, max compression
+gzip compressed data, was "pyautogui_simplified_edition-1.0a2.tar", last modified: Fri Apr 14 15:31:00 2023, max compression
```

## Comparing `pyautogui_simplified_edition-1.0a1.tar` & `pyautogui_simplified_edition-1.0a2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 15:23:27.228748 pyautogui_simplified_edition-1.0a1/
--rw-rw-rw-   0        0        0     3061 2023-04-14 15:23:27.228748 pyautogui_simplified_edition-1.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     2362 2023-04-14 15:00:54.000000 pyautogui_simplified_edition-1.0a1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 15:23:27.212581 pyautogui_simplified_edition-1.0a1/pyautogui_simplified_edition/
--rw-rw-rw-   0        0        0       13 2023-04-14 15:13:41.000000 pyautogui_simplified_edition-1.0a1/pyautogui_simplified_edition/__init__.py
--rw-rw-rw-   0        0        0     5465 2023-04-14 14:31:51.000000 pyautogui_simplified_edition-1.0a1/pyautogui_simplified_edition/screen.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:23:27.226751 pyautogui_simplified_edition-1.0a1/pyautogui_simplified_edition.egg-info/
--rw-rw-rw-   0        0        0     3061 2023-04-14 15:23:27.000000 pyautogui_simplified_edition-1.0a1/pyautogui_simplified_edition.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-04-14 15:23:27.000000 pyautogui_simplified_edition-1.0a1/pyautogui_simplified_edition.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 15:23:27.000000 pyautogui_simplified_edition-1.0a1/pyautogui_simplified_edition.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-14 15:23:27.000000 pyautogui_simplified_edition-1.0a1/pyautogui_simplified_edition.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      785 2023-04-14 15:22:46.000000 pyautogui_simplified_edition-1.0a1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 15:23:27.228748 pyautogui_simplified_edition-1.0a1/setup.cfg
--rw-rw-rw-   0        0        0     1093 2023-04-14 15:23:11.000000 pyautogui_simplified_edition-1.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:31:00.226982 pyautogui_simplified_edition-1.0a2/
+-rw-rw-rw-   0        0        0     2160 2023-04-14 15:31:00.226982 pyautogui_simplified_edition-1.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0     1461 2023-04-14 15:29:10.000000 pyautogui_simplified_edition-1.0a2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 15:31:00.209906 pyautogui_simplified_edition-1.0a2/pyautogui_simplified_edition/
+-rw-rw-rw-   0        0        0       13 2023-04-14 15:13:41.000000 pyautogui_simplified_edition-1.0a2/pyautogui_simplified_edition/__init__.py
+-rw-rw-rw-   0        0        0     5465 2023-04-14 14:31:51.000000 pyautogui_simplified_edition-1.0a2/pyautogui_simplified_edition/screen.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:31:00.225982 pyautogui_simplified_edition-1.0a2/pyautogui_simplified_edition.egg-info/
+-rw-rw-rw-   0        0        0     2160 2023-04-14 15:31:00.000000 pyautogui_simplified_edition-1.0a2/pyautogui_simplified_edition.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-04-14 15:31:00.000000 pyautogui_simplified_edition-1.0a2/pyautogui_simplified_edition.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 15:31:00.000000 pyautogui_simplified_edition-1.0a2/pyautogui_simplified_edition.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-14 15:31:00.000000 pyautogui_simplified_edition-1.0a2/pyautogui_simplified_edition.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      785 2023-04-14 15:30:38.000000 pyautogui_simplified_edition-1.0a2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 15:31:00.226982 pyautogui_simplified_edition-1.0a2/setup.cfg
+-rw-rw-rw-   0        0        0      148 2023-04-14 15:25:09.000000 pyautogui_simplified_edition-1.0a2/setup.py
```

### Comparing `pyautogui_simplified_edition-1.0a1/PKG-INFO` & `pyautogui_simplified_edition-1.0a2/pyautogui_simplified_edition.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyautogui_simplified_edition
-Version: 1.0a1
+Name: pyautogui-simplified-edition
+Version: 1.0a2
 Summary: A simplified edition of the PyAutoGUI library
 Author: Жужелица
 Project-URL: Homepage, https://github.com/immacool/pyautogui-simplified-edition
 Project-URL: Bug Tracker, https://github.com/immacool/pyautogui-simplified-edition/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -28,27 +28,34 @@
 
 ```bash
 pip install pyautogui_simplified_edition
 ```
 
 ## Usage
 
-Here are the available functions in this package:
+Here are some available functions in this package:
 
-- `wait_until_found(image: str, timeout: float = 10.0, interval: float = 0.5, **kwargs) -> None`: waits until an image is found on the screen.
-- `wait_until_not_found(image: str, timeout: float = 10.0, interval: float = 0.5, **kwargs) -> None`: waits until an image is not found on the screen.
-- `find_in(image: str, region: Box | None = None, grayscale: bool = False, confidence: float = 0.9, **kwargs) -> Tuple[int, int]`: finds an image in a given region on the screen.
-- `easy_find(image: str, grayscale: bool = True, confidence: float = 0.75, **kwargs) -> Box | None`: finds an image on the screen using easier parameters.
-- `hard_find(image: str, grayscale: bool = False, confidence: float = 0.93, **kwargs) -> Box | None`: finds an image on the screen using harder parameters.
-- `find_any(images: List[str], grayscale: bool = False, confidence: float = 0.9, **kwargs) -> Tuple[str, Box]`: finds any of the given images on the screen.
-- `find_any_center(images: List[str], grayscale: bool = False, confidence: float = 0.9, **kwargs) -> Tuple[str, Tuple[int, int]]`: finds the center of any of the given images on the screen.
-- `take(image: str, region: Box | None = None, **kwargs) -> None`: takes a screenshot of a given region on the screen.
+```py
+import pyautogui_simplified_edition.screen as screen
+
+# Wait until an image is found on the screen
+pyse.wait_until_found('example.png')
+
+# Find an image in a specific region
+location = pyse.find_in('example.png', region=(100, 100, 500, 500))
+
+# Find any of a list of images on the screen
+image, location = pyse.find_any(['example1.png', 'example2.png'])
+
+# Take a screenshot and save it to a file
+pyse.take('screenshot.png')
+```
 
 For detailed information on the usage of each function, please refer to the docstrings in the code.
 
 ## Acknowledgements
 
 This package is based on the PyAutoGUI library, which can be found at https://pypi.org/project/PyAutoGUI/.
 
 ## License
 
-This package is licensed under the MIT License. Please see the LICENSE file for more information.
+...
```

### Comparing `pyautogui_simplified_edition-1.0a1/pyautogui_simplified_edition/screen.py` & `pyautogui_simplified_edition-1.0a2/pyautogui_simplified_edition/screen.py`

 * *Files identical despite different names*

### Comparing `pyautogui_simplified_edition-1.0a1/pyproject.toml` & `pyautogui_simplified_edition-1.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyautogui_simplified_edition"
-version = "1.0a1"
+version = "1.0a2"
 authors = [
   { name="Жужелица" }
 ]
 description = "A simplified edition of the PyAutoGUI library"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

