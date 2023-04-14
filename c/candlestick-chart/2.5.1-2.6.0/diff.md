# Comparing `tmp/candlestick-chart-2.5.1.tar.gz` & `tmp/candlestick-chart-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "candlestick-chart-2.5.1.tar", last modified: Fri Oct 21 10:08:28 2022, max compression
+gzip compressed data, was "candlestick-chart-2.6.0.tar", last modified: Fri Apr 14 19:55:36 2023, max compression
```

## Comparing `candlestick-chart-2.5.1.tar` & `candlestick-chart-2.6.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 10:08:28.773561 candlestick-chart-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7219 2022-10-21 10:08:28.773561 candlestick-chart-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5578 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-10-21 10:08:28.777561 candlestick-chart-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 10:08:28.769561 candlestick-chart-2.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 10:08:28.773561 candlestick-chart-2.5.1/src/candlestick_chart/
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/src/candlestick_chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2223 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/src/candlestick_chart/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/src/candlestick_chart/candle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/src/candlestick_chart/candle_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     4952 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/src/candlestick_chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/src/candlestick_chart/chart_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4137 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/src/candlestick_chart/chart_renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/src/candlestick_chart/colors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/src/candlestick_chart/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/src/candlestick_chart/info_bar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1783 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/src/candlestick_chart/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/src/candlestick_chart/volume_pane.py
--rw-r--r--   0 runner    (1001) docker     (121)     3844 2022-10-21 10:08:26.000000 candlestick-chart-2.5.1/src/candlestick_chart/y_axis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 10:08:28.773561 candlestick-chart-2.5.1/src/candlestick_chart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7219 2022-10-21 10:08:28.000000 candlestick-chart-2.5.1/src/candlestick_chart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-10-21 10:08:28.000000 candlestick-chart-2.5.1/src/candlestick_chart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 10:08:28.000000 candlestick-chart-2.5.1/src/candlestick_chart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-21 10:08:28.000000 candlestick-chart-2.5.1/src/candlestick_chart.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-21 10:08:28.000000 candlestick-chart-2.5.1/src/candlestick_chart.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:55:36.772699 candlestick-chart-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-14 19:55:36.772699 candlestick-chart-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-14 19:55:36.772699 candlestick-chart-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:55:36.768699 candlestick-chart-2.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:55:36.772699 candlestick-chart-2.6.0/src/candlestick_chart/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/candle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/candle_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/chart_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/chart_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/info_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/volume_pane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart/y_axis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:55:36.772699 candlestick-chart-2.6.0/src/candlestick_chart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 19:55:36.000000 candlestick-chart-2.6.0/src/candlestick_chart.egg-info/top_level.txt
```

### Comparing `candlestick-chart-2.5.1/LICENSE` & `candlestick-chart-2.6.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 MIT License
-Copyright (c) 2022, Mickaël 'Tiger-222' Schoentgen
+Copyright (c) 2022-2023, Mickaël 'Tiger-222' Schoentgen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `candlestick-chart-2.5.1/PKG-INFO` & `candlestick-chart-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candlestick-chart
-Version: 2.5.1
+Version: 2.6.0
 Summary: Draw candlesticks charts right into your terminal, using Python!
 Home-page: https://github.com/BoboTiG/py-candlestick-chart
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: LICENSE
 Project-URL: Documentation, https://github.com/BoboTiG/py-candlestick-chart
 Project-URL: Source, https://github.com/BoboTiG/py-candlestick-chart
@@ -181,14 +181,15 @@
 ## API 
 
 - [Basic example with CSV parsing](examples/basic-from-csv-file.py): run with `$ python examples/basic-from-csv-file.py`
 - [Basic example with JSON parsing](examples/basic-from-json-file.py): run with `$ python examples/basic-from-json-file.py`
 - [Basic example with stdin parsing](examples/basic-from-stdin.sh): run with `$ ./examples/basic-from-stdin.sh`
 - [Fetch candles from Binance](examples/fetch-from-binance.py): run with `$ python examples/fetch-from-binance.py`
 - [Integration with Rich](examples/integrate-with-rich.py): run with `$ python examples/integrate-with-rich.py`
+- [Using a custom chart renderer class](examples/custom-renderer-class.py): run with `$ python examples/custom-renderer-class.py`
 
 ## Binary 
 
 ### Read CSV from file
 
 ```bash
 $ candlestick-chart \
@@ -227,7 +228,9 @@
   }
 ]' | candlestick-chart \
     --mode=stdin \
     --chart-name='My BTC Chart' \
     --bear-color='#b967ff' \
     --bull-color='ff6b99'
 ```
+
+
```

### Comparing `candlestick-chart-2.5.1/README.md` & `candlestick-chart-2.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -147,14 +147,15 @@
 ## API 
 
 - [Basic example with CSV parsing](examples/basic-from-csv-file.py): run with `$ python examples/basic-from-csv-file.py`
 - [Basic example with JSON parsing](examples/basic-from-json-file.py): run with `$ python examples/basic-from-json-file.py`
 - [Basic example with stdin parsing](examples/basic-from-stdin.sh): run with `$ ./examples/basic-from-stdin.sh`
 - [Fetch candles from Binance](examples/fetch-from-binance.py): run with `$ python examples/fetch-from-binance.py`
 - [Integration with Rich](examples/integrate-with-rich.py): run with `$ python examples/integrate-with-rich.py`
+- [Using a custom chart renderer class](examples/custom-renderer-class.py): run with `$ python examples/custom-renderer-class.py`
 
 ## Binary 
 
 ### Read CSV from file
 
 ```bash
 $ candlestick-chart \
```

### Comparing `candlestick-chart-2.5.1/setup.cfg` & `candlestick-chart-2.6.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -41,25 +41,35 @@
 package_dir = 
 	= src
 packages = find:
 
 [options.packages.find]
 where = src
 
+[options.package_data]
+candlestick_chart = py.typed
+
 [options.entry_points]
 console_scripts = 
 	candlestick-chart = candlestick_chart.__main__:main
 
 [flake8]
 max-line-length = 120
 exclude = 
 	*.egg-info
 	.git
 	.mypy_cache
 	__pytest_cache__
 	venv
 inline-quotes = double
 
+[tool:isort]
+multi_line_output = 3
+include_trailing_comma = true
+force_grid_wrap = 0
+use_parentheses = true
+line_length = 120
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart/__init__.py` & `candlestick-chart-2.6.0/src/candlestick_chart/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 This module is maintained by Mickaël Schoentgen <contact@tiger-222.fr>.
 
 You can always get the latest version of this module at:
     https://github.com/BoboTiG/py-candlestrick-charts
 If that URL should fail, try contacting the author.
 """
 
-__version__ = "2.5.1"
+__version__ = "2.6.0"
 __author__ = "Mickaël 'Tiger-222' Schoentgen"
 __copyright__ = """
-Copyright (c) 2022, Mickaël 'Tiger-222' Schoentgen
+Copyright (c) 2022-2023, Mickaël 'Tiger-222' Schoentgen
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
 granted, provided that the above copyright notice appear in all copies
 and that both that copyright notice and this permission notice appear
 in supporting documentation or portions thereof, including
 modifications, that you make.
 """
```

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart/__main__.py` & `candlestick-chart-2.6.0/src/candlestick_chart/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,23 +27,17 @@
         "--mode",
         help="Select the method for retrieving the candles.",
         choices=["stdin", "csv-file", "json-file"],
         required=True,
     )
     parser.add_argument("-f", "--file", help="[MODE:*-file] File to read candles from.")
     parser.add_argument("--chart-name", help="Sets the chart name.")
-    parser.add_argument(
-        "--bear-color", help="Sets the descending candles color in hexadecimal."
-    )
-    parser.add_argument(
-        "--bull-color", help="Sets the ascending candles color in hexadecimal."
-    )
-    parser.add_argument(
-        "--version", action="version", version=f"%(prog)s {__version__}"
-    )
+    parser.add_argument("--bear-color", help="Sets the descending candles color in hexadecimal.")
+    parser.add_argument("--bull-color", help="Sets the ascending candles color in hexadecimal.")
+    parser.add_argument("--version", action="version", version=f"%(prog)s {__version__}")
     return parser.parse_args(sys.argv[1:])
 
 
 def main() -> int:
     options = get_args()
 
     if options.mode == "csv-file":
```

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart/candle.py` & `candlestick-chart-2.6.0/src/candlestick_chart/candle.py`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart/candle_set.py` & `candlestick-chart-2.6.0/src/candlestick_chart/candle_set.py`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart/chart.py` & `candlestick-chart-2.6.0/src/candlestick_chart/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Dict, Iterable, Tuple
+from typing import TYPE_CHECKING, Dict, Iterable, Tuple, Type
 
 from .candle import Candles
 from .chart_data import ChartData
 from .chart_renderer import ChartRenderer
 from .info_bar import InfoBar
 from .volume_pane import VolumePane
 from .y_axis import YAxis
@@ -18,28 +18,31 @@
         "renderer",
         "highlights",
         "volume_pane",
         "y_axis",
     )
 
     def __init__(
-        self, candles: Candles, title: str = "My chart", width: int = 0, height: int = 0
+        self,
+        candles: Candles,
+        title: str = "My chart",
+        width: int = 0,
+        height: int = 0,
+        renderer_cls: Type[ChartRenderer] = ChartRenderer,
     ) -> None:
-        self.renderer = ChartRenderer()
+        self.renderer = renderer_cls()
         self.chart_data = ChartData(candles, width=width, height=height)
         self.y_axis = YAxis(self.chart_data)
         self.info_bar = InfoBar(title)
         self.volume_pane = VolumePane(int(self.chart_data.height / 6))
 
         # A dict of price -> color to display custom colors on specific prices on the Y-axis
         self.highlights: Dict[str, str | Tuple[int, int, int]] = {}
 
-    def __rich_console__(
-        self, console: "Console", options: "ConsoleOptions"
-    ) -> Iterable[str]:
+    def __rich_console__(self, console: "Console", options: "ConsoleOptions") -> Iterable[str]:
         from rich.ansi import AnsiDecoder
         from rich.console import Group
 
         self.update_size(
             options.max_width or console.width,
             options.height or console.height,
         )
```

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart/chart_data.py` & `candlestick-chart-2.6.0/src/candlestick_chart/chart_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,28 +23,21 @@
             width, height = get_terminal_size()
         self.set_size(width, height)
 
         self.compute_visible_candles()
 
     def compute_height(self, volume_pane: VolumePane) -> None:
         volume_pane_height = volume_pane.height if volume_pane.enabled else 0
-        self.height: int = (
-            self.terminal_size[1]
-            - constants.MARGIN_TOP
-            - constants.HEIGHT
-            - volume_pane_height
-        )
+        self.height: int = self.terminal_size[1] - constants.MARGIN_TOP - constants.HEIGHT - volume_pane_height
 
     def compute_visible_candles(self) -> None:
         nb_visible_candles = self.width - constants.WIDTH
         if not constants.Y_AXIS_ON_THE_RIGHT:
             nb_visible_candles -= constants.MARGIN_RIGHT
-        self.visible_candle_set.set_candles(
-            self.main_candle_set.candles[-nb_visible_candles:]
-        )
+        self.visible_candle_set.set_candles(self.main_candle_set.candles[-nb_visible_candles:])
 
     def reset_candles(self) -> None:
         self.main_candle_set.set_candles([])
         self.visible_candle_set.set_candles([])
 
     def add_candles(self, candles: Candles) -> None:
         self.main_candle_set.add_candles(candles)
```

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart/chart_renderer.py` & `candlestick-chart-2.6.0/src/candlestick_chart/chart_renderer.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,19 +13,15 @@
 
 @dataclass(slots=True)
 class ChartRenderer:
     bearish_color: Tuple[int, int, int] = (234, 74, 90)
     bullish_color: Tuple[int, int, int] = (52, 208, 88)
 
     def _colorize(self, candle_type: int, string: str) -> str:
-        color = (
-            self.bearish_color
-            if candle_type == CandleType.bearish
-            else self.bullish_color
-        )
+        color = self.bearish_color if candle_type == CandleType.bearish else self.bullish_color
         return truecolor(string, *color)
 
     def _render_candle(self, candle: Candle, y: int, y_axis: YAxis) -> str:
         height_unit = float(y)
         high_y, low_y, max_y, min_y = y_axis.price_to_heights(candle)
         output = constants.UNICODE_VOID
 
@@ -80,17 +76,15 @@
 
         for y in range(chart_data.height, 0, -1):
             if graduations_on_right:
                 output.append("\n")
             else:
                 output.extend(("\n", render_line(y, highlights)))
 
-            output.extend(
-                self._render_candle(candle, y, chart.y_axis) for candle in candles
-            )
+            output.extend(self._render_candle(candle, y, chart.y_axis) for candle in candles)
 
             if graduations_on_right:
                 output.append(render_line(y, highlights))
 
         if chart.volume_pane.enabled:
             render_empty = chart.y_axis.render_empty
             render = chart.volume_pane.render
@@ -103,12 +97,10 @@
                     output.extend(("\n", render_empty()))
 
                 output.extend(render(candle, y, max_volume) for candle in candles)
 
                 if graduations_on_right:
                     output.append(render_empty())
 
-        output.append(
-            chart.info_bar.render(chart_data.main_candle_set, chart_data.width)
-        )
+        output.append(chart.info_bar.render(chart_data.main_candle_set, chart_data.width))
 
         return "".join(output)
```

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart/colors.py` & `candlestick-chart-2.6.0/src/candlestick_chart/colors.py`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart/constants.py` & `candlestick-chart-2.6.0/src/candlestick_chart/constants.py`

 * *Files identical despite different names*

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart/info_bar.py` & `candlestick-chart-2.6.0/src/candlestick_chart/info_bar.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,49 +25,35 @@
             else green
             if candle_set.last_price < candle_set.average
             else yellow
         )
         return f"{self.labels.average}: {color(fnum(candle_set.last_price))}"
 
     def _render_highest(self, candle_set: "CandleSet") -> str:
-        return (
-            f"{self.labels.highest}: {green(fnum(candle_set.max_price))}"
-            if self.labels.highest
-            else ""
-        )
+        return f"{self.labels.highest}: {green(fnum(candle_set.max_price))}" if self.labels.highest else ""
 
     def _render_lowest(self, candle_set: "CandleSet") -> str:
-        return (
-            f"{self.labels.lowest}: {red(fnum(candle_set.min_price))}"
-            if self.labels.lowest
-            else ""
-        )
+        return f"{self.labels.lowest}: {red(fnum(candle_set.min_price))}" if self.labels.lowest else ""
 
     def _render_price(self, candle_set: "CandleSet") -> str:
         price = f"{self.labels.price}: {bold(green(fnum(candle_set.last_price)))}"
         if self.labels.currency:
             price += f" {self.labels.currency}"
         return price
 
     def _render_variation(self, candle_set: "CandleSet") -> str:
         if not self.labels.variation:
             return ""
 
         variation_output = ("↖", green) if candle_set.variation > 0.0 else ("↙", red)
-        var = variation_output[1](
-            f"{variation_output[0]} {candle_set.variation:>+.2f}%"
-        )
+        var = variation_output[1](f"{variation_output[0]} {candle_set.variation:>+.2f}%")
         return f"{self.labels.variation}: {var}"
 
     def _render_volume(self, candle_set: "CandleSet") -> str:
-        return (
-            f"{self.labels.volume}: {green(fnum(int(candle_set.cumulative_volume)))}"
-            if self.labels.volume
-            else ""
-        )
+        return f"{self.labels.volume}: {green(fnum(int(candle_set.cumulative_volume)))}" if self.labels.volume else ""
 
     def render(self, candle_set: "CandleSet", available_width: int) -> str:
         return "".join(
             (
                 "\n",
                 "─" * available_width,
                 "\n",
```

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart/utils.py` & `candlestick-chart-2.6.0/src/candlestick_chart/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,24 +19,18 @@
         try:
             value = int(value)
         except ValueError:
             value = float(value)
 
     # 0, 0.00, > 1, and > 1.00 (same for negative numbers)
     if not value or abs(value) >= 1:
-        return (
-            f"{value:,}"
-            if isinstance(value, int)
-            else f"{value:,.{constants.PRECISION}f}"
-        )
+        return f"{value:,}" if isinstance(value, int) else f"{value:,.{constants.PRECISION}f}"
 
     # 0.000000000012345678 -> 0.⦗0×10⦘1234
-    formatted = REPLACE_CONSECUTIVE_ZEROES(
-        fnum_replace_consecutive_zeroes, f"{value:.18f}"
-    )
+    formatted = REPLACE_CONSECUTIVE_ZEROES(fnum_replace_consecutive_zeroes, f"{value:.18f}")
     return formatted if "0×" in formatted else f"{value:.{constants.PRECISION_SMALL}f}"
 
 
 def hexa_to_rgb(hex_code: str) -> Tuple[int, int, int]:
     hex_code = hex_code.lstrip("#")
     r = int(hex_code[:2], 16)
     g = int(hex_code[2:4], 16)
```

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart/volume_pane.py` & `candlestick-chart-2.6.0/src/candlestick_chart/volume_pane.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,15 @@
     height: int
     enabled: bool = True
     bearish_color: Tuple[int, int, int] = (234, 74, 90)
     bullish_color: Tuple[int, int, int] = (52, 208, 88)
     unicode_fill: str = constants.UNICODE_FILL
 
     def _colorize(self, candle_type: int, string: str) -> str:
-        color = (
-            self.bearish_color
-            if candle_type == CandleType.bearish
-            else self.bullish_color
-        )
+        color = self.bearish_color if candle_type == CandleType.bearish else self.bullish_color
         return truecolor(string, *color)
 
     def render(self, candle: Candle, y: int, max_volume: float) -> str:
         volume_percent_of_max = candle.volume / (max_volume or 1)
         ratio = volume_percent_of_max * self.height
 
         if y < ceil(ratio):
```

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart/y_axis.py` & `candlestick-chart-2.6.0/src/candlestick_chart/y_axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,29 +16,28 @@
     chart_data: "ChartData"
 
     def price_to_heights(self, candle: Candle) -> Tuple[float, ...]:
         chart_data = self.chart_data
         height = chart_data.height
         candle_set = chart_data.visible_candle_set
 
+        # sourcery skip: min-max-identity
         min_open = candle.open if candle.open < candle.close else candle.close
         max_open = candle.open if candle.open > candle.close else candle.close
         min_value = candle_set.min_price
         diff = (candle_set.max_price - min_value) or 1
 
         return (
             (candle.high - min_value) / diff * height,  # high_y
             (candle.low - min_value) / diff * height,  # low_y
             (max_open - min_value) / diff * height,  # max_y
             (min_open - min_value) / diff * height,  # min_y
         )
 
-    def render_line(
-        self, y: int, highlights: Dict[str, str | Tuple[int, int, int]] = None
-    ) -> str:
+    def render_line(self, y: int, highlights: Dict[str, str | Tuple[int, int, int]] = None) -> str:
         return (
             self.render_empty(y=y, highlights=highlights)
             if y % constants.Y_AXIS_SPACING
             else self._render_tick(y, highlights or {})
         )
 
     def _round_price(
@@ -51,27 +50,23 @@
             multiplier = constants.Y_AXIS_ROUND_MULTIPLIER
             if constants.Y_AXIS_ROUND_DIR == "down":
                 value = fn_down(value * multiplier) / multiplier
             else:
                 value = fn_up(value * multiplier) / multiplier
         return fnum(value)
 
-    def _render_price(
-        self, y: float, highlights: Dict[str, str | Tuple[int, int, int]]
-    ) -> Tuple[bool, str]:
+    def _render_price(self, y: float, highlights: Dict[str, str | Tuple[int, int, int]]) -> Tuple[bool, str]:
         chart_data = self.chart_data
         min_value = chart_data.visible_candle_set.min_price
         max_value = chart_data.visible_candle_set.max_price
         height = chart_data.height
 
         cell_min_length = constants.CHAR_PRECISION + constants.DEC_PRECISION + 1
         price = self._round_price(min_value + (y * (max_value - min_value) / height))
-        price_upper = self._round_price(
-            min_value + ((y + 1) * (max_value - min_value) / height)
-        )
+        price_upper = self._round_price(min_value + ((y + 1) * (max_value - min_value) / height))
 
         has_special_price = False
         custom_color: str | Tuple[int, int, int] = ""
 
         for target_price, target_color in highlights.items():
             if not (price <= target_price < price_upper):
                 continue
@@ -84,27 +79,23 @@
             f" {color(f'├ {price:<{cell_min_length}}', custom_color)}"
             if constants.Y_AXIS_ON_THE_RIGHT
             else f"{color(f'{price:<{cell_min_length}} ┤', custom_color)}{' ' * constants.MARGIN_RIGHT}"
         )
 
         return has_special_price, price
 
-    def render_empty(
-        self, y: float = None, highlights: Dict[str, str | Tuple[int, int, int]] = None
-    ) -> str:
+    def render_empty(self, y: float = None, highlights: Dict[str, str | Tuple[int, int, int]] = None) -> str:
         if highlights and y:
             has_special_price, price = self._render_price(y, highlights)
             if has_special_price:
                 return price
 
         if constants.Y_AXIS_ON_THE_RIGHT:
             return " │"
 
         cell = " " * (constants.CHAR_PRECISION + constants.DEC_PRECISION + 2)
-        margin = " " * (constants.MARGIN_RIGHT + 1)
+        margin = " " * constants.MARGIN_RIGHT
         return f"{cell}│{margin}"
 
-    def _render_tick(
-        self, y: int, highlights: Dict[str, str | Tuple[int, int, int]]
-    ) -> str:
+    def _render_tick(self, y: int, highlights: Dict[str, str | Tuple[int, int, int]]) -> str:
         _, price = self._render_price(y, highlights)
         return price
```

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart.egg-info/PKG-INFO` & `candlestick-chart-2.6.0/src/candlestick_chart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candlestick-chart
-Version: 2.5.1
+Version: 2.6.0
 Summary: Draw candlesticks charts right into your terminal, using Python!
 Home-page: https://github.com/BoboTiG/py-candlestick-chart
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: LICENSE
 Project-URL: Documentation, https://github.com/BoboTiG/py-candlestick-chart
 Project-URL: Source, https://github.com/BoboTiG/py-candlestick-chart
@@ -181,14 +181,15 @@
 ## API 
 
 - [Basic example with CSV parsing](examples/basic-from-csv-file.py): run with `$ python examples/basic-from-csv-file.py`
 - [Basic example with JSON parsing](examples/basic-from-json-file.py): run with `$ python examples/basic-from-json-file.py`
 - [Basic example with stdin parsing](examples/basic-from-stdin.sh): run with `$ ./examples/basic-from-stdin.sh`
 - [Fetch candles from Binance](examples/fetch-from-binance.py): run with `$ python examples/fetch-from-binance.py`
 - [Integration with Rich](examples/integrate-with-rich.py): run with `$ python examples/integrate-with-rich.py`
+- [Using a custom chart renderer class](examples/custom-renderer-class.py): run with `$ python examples/custom-renderer-class.py`
 
 ## Binary 
 
 ### Read CSV from file
 
 ```bash
 $ candlestick-chart \
@@ -227,7 +228,9 @@
   }
 ]' | candlestick-chart \
     --mode=stdin \
     --chart-name='My BTC Chart' \
     --bear-color='#b967ff' \
     --bull-color='ff6b99'
 ```
+
+
```

### Comparing `candlestick-chart-2.5.1/src/candlestick_chart.egg-info/SOURCES.txt` & `candlestick-chart-2.6.0/src/candlestick_chart.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/candlestick_chart/candle_set.py
 src/candlestick_chart/chart.py
 src/candlestick_chart/chart_data.py
 src/candlestick_chart/chart_renderer.py
 src/candlestick_chart/colors.py
 src/candlestick_chart/constants.py
 src/candlestick_chart/info_bar.py
+src/candlestick_chart/py.typed
 src/candlestick_chart/utils.py
 src/candlestick_chart/volume_pane.py
 src/candlestick_chart/y_axis.py
 src/candlestick_chart.egg-info/PKG-INFO
 src/candlestick_chart.egg-info/SOURCES.txt
 src/candlestick_chart.egg-info/dependency_links.txt
 src/candlestick_chart.egg-info/entry_points.txt
```

