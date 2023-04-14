# Comparing `tmp/favicons-0.1.1.tar.gz` & `tmp/favicons-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "favicons-0.1.1.tar", max compression
+gzip compressed data, was "favicons-0.2.0.tar", max compression
```

## Comparing `favicons-0.1.1.tar` & `favicons-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1683 2021-09-27 00:01:40.265726 favicons-0.1.1/LICENSE
--rw-r--r--   0        0        0    12956 2021-09-27 00:01:40.265726 favicons-0.1.1/README.md
--rw-r--r--   0        0        0      212 2021-09-27 00:01:40.265726 favicons-0.1.1/favicons/__init__.py
--rw-r--r--   0        0        0       39 2021-09-27 00:01:40.265726 favicons-0.1.1/favicons/_cli/__init__.py
--rw-r--r--   0        0        0     3518 2021-09-27 00:01:40.265726 favicons-0.1.1/favicons/_cli/main.py
--rw-r--r--   0        0        0     2617 2021-09-27 00:01:40.265726 favicons-0.1.1/favicons/_constants.py
--rw-r--r--   0        0        0     2702 2021-09-27 00:01:40.265726 favicons-0.1.1/favicons/_exceptions.py
--rw-r--r--   0        0        0     6208 2021-09-27 00:01:40.265726 favicons-0.1.1/favicons/_generate.py
--rw-r--r--   0        0        0      139 2021-09-27 00:01:40.265726 favicons-0.1.1/favicons/_types/__init__.py
--rw-r--r--   0        0        0     4273 2021-09-27 00:01:40.265726 favicons-0.1.1/favicons/_types/color.py
--rw-r--r--   0        0        0     1968 2021-09-27 00:01:40.265726 favicons-0.1.1/favicons/_types/properties.py
--rw-r--r--   0        0        0     1776 2021-09-27 00:01:40.265726 favicons-0.1.1/favicons/_util.py
--rw-r--r--   0        0        0      115 2021-09-27 00:01:40.265726 favicons-0.1.1/favicons/cli.py
--rw-r--r--   0        0        0        0 2021-09-27 00:01:40.265726 favicons-0.1.1/favicons/py.typed
--rw-r--r--   0        0        0     1677 2021-09-27 00:01:40.269726 favicons-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    14794 2021-09-27 00:01:52.995849 favicons-0.1.1/setup.py
--rw-r--r--   0        0        0    14136 2021-09-27 00:01:52.996639 favicons-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1683 2023-04-14 04:20:00.199362 favicons-0.2.0/LICENSE
+-rw-r--r--   0        0        0    12897 2023-04-14 04:20:00.199362 favicons-0.2.0/README.md
+-rw-r--r--   0        0        0      359 2023-04-14 04:20:00.199362 favicons-0.2.0/favicons/__init__.py
+-rw-r--r--   0        0        0       39 2023-04-14 04:20:00.199362 favicons-0.2.0/favicons/_cli/__init__.py
+-rw-r--r--   0        0        0     3568 2023-04-14 04:20:00.199362 favicons-0.2.0/favicons/_cli/main.py
+-rw-r--r--   0        0        0     2617 2023-04-14 04:20:00.199362 favicons-0.2.0/favicons/_constants.py
+-rw-r--r--   0        0        0     2712 2023-04-14 04:20:00.199362 favicons-0.2.0/favicons/_exceptions.py
+-rw-r--r--   0        0        0     6476 2023-04-14 04:20:00.199362 favicons-0.2.0/favicons/_generate.py
+-rw-r--r--   0        0        0      139 2023-04-14 04:20:00.199362 favicons-0.2.0/favicons/_types/__init__.py
+-rw-r--r--   0        0        0     4289 2023-04-14 04:20:00.199362 favicons-0.2.0/favicons/_types/color.py
+-rw-r--r--   0        0        0     1968 2023-04-14 04:20:00.199362 favicons-0.2.0/favicons/_types/properties.py
+-rw-r--r--   0        0        0     1820 2023-04-14 04:20:00.199362 favicons-0.2.0/favicons/_util.py
+-rw-r--r--   0        0        0      115 2023-04-14 04:20:00.199362 favicons-0.2.0/favicons/cli.py
+-rw-r--r--   0        0        0        0 2023-04-14 04:20:00.199362 favicons-0.2.0/favicons/py.typed
+-rw-r--r--   0        0        0     1637 2023-04-14 04:20:00.203363 favicons-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    14192 1970-01-01 00:00:00.000000 favicons-0.2.0/PKG-INFO
```

### Comparing `favicons-0.1.1/LICENSE` & `favicons-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `favicons-0.1.1/README.md` & `favicons-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 <hr/>
 
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/favicons?style=for-the-badge)](https://pypi.org/project/favicons/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/favicons?style=for-the-badge)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/thatmattlove/favicons/Tests?style=for-the-badge)](https://github.com/thatmattlove/favicons/actions/workflows/ci.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/thatmattlove/favicons/ci.yml?style=for-the-badge)
 
 [![GitHub Contributors](https://img.shields.io/github/contributors/thatmattlove/favicons?style=for-the-badge&color=blueviolet)](https://github.com/thatmattlove/favicons)
 
 
 <br/>
 
 ### [Changelog](https://github.com/thatmattlove/favicons/blob/master/CHANGELOG.md)
```

### Comparing `favicons-0.1.1/favicons/_cli/main.py` & `favicons-0.2.0/favicons/_cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 # Project
 from favicons._generate import Favicons
 from favicons._types.properties import FaviconProperties
 
 cli = Typer(name="Favicons", add_completion=False)
 console = Console()
 
+DEFAULT_OUTPUT_PATH = Path.cwd()
+
 
 def item_name(item: FaviconProperties) -> str:
     """Format favicon name."""
     return f"[bold green]{str(item)}[/bold green]"
 
 
 DEFAULT_SOURCE = Option(..., help="Source Image")
-DEFAULT_OUTPUT_DIR = Option(..., help="Output Directory")
+DEFAULT_OUTPUT_DIR = Option(DEFAULT_OUTPUT_PATH, help="Output Directory")
 DEFAULT_BG = Option("#000000", help="Background Color")
 DEFAULT_TRANSPARENT = Option(True, help="Transparent Background")
 DEFAULT_BASE_URL = Option("/", help="Base URL for HTML output")
 
 
 @cli.command()
 def generate(
```

### Comparing `favicons-0.1.1/favicons/_constants.py` & `favicons-0.2.0/favicons/_constants.py`

 * *Files identical despite different names*

### Comparing `favicons-0.1.1/favicons/_exceptions.py` & `favicons-0.2.0/favicons/_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,23 +51,23 @@
         }
 
     def json(self) -> str:
         """Represent exception as JSON string."""
         return _json.dumps(self.dict())
 
 
-class FaviconNotFound(FaviconsError):
+class FaviconNotFoundError(FaviconsError):
     """Raised if the source favicon doesn't exist."""
 
     def __init__(self, file: Path) -> None:
         """Set message."""
         super().__init__("{} does not exit.", str(file))
 
 
-class FaviconNotSupported(FaviconsError):
+class FaviconNotSupportedError(FaviconsError):
     """Raised if the source favicon file format is not supported."""
 
     def __init__(self, file: Path) -> None:
         """Set message."""
         one_of = ", ".join(f"'{f}'" for f in SUPPORTED_FORMATS)
         super().__init__(
             "Extension {extension} is not supported ({file}). Must be one of {one_of}.",
```

### Comparing `favicons-0.1.1/favicons/_generate.py` & `favicons-0.2.0/favicons/_generate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Generate common favicon formats from a single source image."""
 
 # Standard Library
 import json as _json
 import math
 import asyncio
+from types import TracebackType
 from typing import (
     Any,
     Type,
     Tuple,
     Union,
     Callable,
     Optional,
@@ -20,15 +21,15 @@
 # Third Party
 from PIL import Image as PILImage
 
 # Project
 from favicons._util import svg_to_png, validate_path, generate_icon_types
 from favicons._types import Color, FaviconProperties
 from favicons._constants import HTML_LINK, SUPPORTED_FORMATS
-from favicons._exceptions import FaviconNotSupported
+from favicons._exceptions import FaviconNotSupportedError
 
 LoosePath = Union[Path, str]
 LooseColor = Union[Collection[int], str]
 
 
 class Favicons:
     """Generate common favicon formats from a single source image."""
@@ -63,37 +64,45 @@
 
     def _validate(self) -> None:
 
         self.source = validate_path(self._source)
         self.output_directory = validate_path(self._output_directory, create=True)
 
         if self.source.suffix.lower() not in SUPPORTED_FORMATS:
-            raise FaviconNotSupported(self.source)
+            raise FaviconNotSupportedError(self.source)
 
         self._validated = True
 
     def __enter__(self) -> "Favicons":
         """Enter Favicons context."""
         self._validate()
         self.generate = self.sgenerate
         return self
 
-    def __exit__(self, exc_type: Type = None, exc_value: Any = None, traceback: str = None) -> None:
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_value: Optional[BaseException] = None,
+        traceback: Optional[TracebackType] = None,
+    ) -> None:
         """Exit Favicons context."""
         self._close_temp_source()
         pass
 
     async def __aenter__(self) -> "Favicons":
         """Enter Favicons context."""
         self._validate()
         self.generate = self.agenerate
         return self
 
     async def __aexit__(
-        self, exc_type: Type = None, exc_value: Any = None, traceback: str = None
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_value: Optional[BaseException] = None,
+        traceback: Optional[TracebackType] = None,
     ) -> None:
         """Exit Favicons context."""
         self._close_temp_source()
         pass
 
     def _close_temp_source(self) -> None:
         """Close temporary file if it exists."""
@@ -162,15 +171,17 @@
 
         await asyncio.gather(*(self._agenerate_single(fmt) for fmt in self._formats))
 
     def html_gen(self) -> Generator:
         """Get generator of HTML strings."""
         for fmt in self._formats:
             yield HTML_LINK.format(
-                rel=fmt.rel, type=f"image/{fmt.image_fmt}", href=self.base_url + str(fmt),
+                rel=fmt.rel,
+                type=f"image/{fmt.image_fmt}",
+                href=self.base_url + str(fmt),
             )
 
     def html(self) -> Tuple:
         """Get tuple of HTML strings."""
         return tuple(self.html_gen())
 
     def formats(self) -> Tuple:
```

### Comparing `favicons-0.1.1/favicons/_types/color.py` & `favicons-0.2.0/favicons/_types/color.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,16 +93,16 @@
 
         for i in rgb_iter:
             try:
                 num = int(i)
                 if num not in range(0, 256):
                     raise FaviconColorError(rgb_iter)
                 yield num
-            except TypeError:
-                raise FaviconColorError(rgb_iter)
+            except TypeError as err:
+                raise FaviconColorError(rgb_iter) from err
 
     @staticmethod
     def _parse_rgbstr(rgbstr: str) -> Generator:
         """Validate & parse color string in rgb(x, y, z) format."""
         for digit in get_matches(_RGB_STR_PATTERN, rgbstr):
             num = int(digit)
             if num not in range(0, 256):
```

### Comparing `favicons-0.1.1/favicons/_types/properties.py` & `favicons-0.2.0/favicons/_types/properties.py`

 * *Files identical despite different names*

### Comparing `favicons-0.1.1/favicons/_util.py` & `favicons-0.2.0/favicons/_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,47 +4,48 @@
 from typing import Union, Mapping, Generator
 from pathlib import Path
 from tempfile import mkstemp
 
 # Project
 from favicons._types import Color, FaviconProperties
 from favicons._constants import ICON_TYPES
-from favicons._exceptions import FaviconsError, FaviconNotFound
+from favicons._exceptions import FaviconsError, FaviconNotFoundError
 
 
 def validate_path(path: Union[Path, str], must_exist: bool = True, create: bool = False) -> Path:
     """Validate a path and ensure it's a Path object."""
 
     if isinstance(path, str):
         try:
             path = Path(path)
-        except TypeError:
-            raise FaviconsError("{path} is not a valid path.", path=path)
+        except TypeError as err:
+            raise FaviconsError("{path} is not a valid path.", path=path) from err
 
     if create:
         if path.is_dir() and not path.exists():
             path.mkdir(parents=True)
         elif not path.is_dir() and not path.parent.exists():
             path.parent.mkdir(parents=True)
 
     if must_exist and not path.exists():
-        raise FaviconNotFound(path)
+        raise FaviconNotFoundError(path)
 
     return path
 
 
 def generate_icon_types() -> Generator[FaviconProperties, None, None]:
     """Get icon type objects."""
     for icon_type in ICON_TYPES:
         if isinstance(icon_type, Mapping):
             yield FaviconProperties(**icon_type)
 
 
 def svg_to_png(svg_path: Path, background_color: Color) -> Path:
     """Convert an SVG vector to a PNG file."""
+    # Third Party
     from svglib.svglib import svg2rlg
     from reportlab.graphics import renderPM
     from reportlab.lib.colors import transparent
 
     _, png_path = mkstemp(suffix=".tiff")
 
     png = Path(png_path)
```

### Comparing `favicons-0.1.1/PKG-INFO` & `favicons-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 Metadata-Version: 2.1
 Name: favicons
-Version: 0.1.1
+Version: 0.2.0
 Summary: Favicon generator for Python 3 with strongly typed sync & async APIs, CLI, & HTML generation.
 Home-page: https://github.com/thatmattlove/favicons
 License: BSD-3-Clause-Clear
 Author: Matt Love
 Author-email: matt@hyperglass.dev
-Requires-Python: >=3.6.1,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Typing :: Typed
-Requires-Dist: pillow (>=7.2,<9.0)
-Requires-Dist: rich (>=6.0,<11.0)
-Requires-Dist: svglib (>=1.0.0,<2.0.0)
-Requires-Dist: typer (>=0.3.1,<1.0)
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: svglib (>=1.5.1,<2.0.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/thatmattlove/favicons
 Description-Content-Type: text/markdown
 
 <div align="center">
   <h1>Favicons</h1>
   <h3>Favicon generator for Python 3 with strongly typed sync & async APIs, CLI, & HTML generation.</h3>
 </div>
 
 <hr/>
 
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/favicons?style=for-the-badge)](https://pypi.org/project/favicons/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/favicons?style=for-the-badge)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/thatmattlove/favicons/Tests?style=for-the-badge)](https://github.com/thatmattlove/favicons/actions/workflows/ci.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/thatmattlove/favicons/ci.yml?style=for-the-badge)
 
 [![GitHub Contributors](https://img.shields.io/github/contributors/thatmattlove/favicons?style=for-the-badge&color=blueviolet)](https://github.com/thatmattlove/favicons)
 
 
 <br/>
 
 ### [Changelog](https://github.com/thatmattlove/favicons/blob/master/CHANGELOG.md)
```

