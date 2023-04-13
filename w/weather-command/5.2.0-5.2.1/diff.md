# Comparing `tmp/weather_command-5.2.0.tar.gz` & `tmp/weather_command-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_command-5.2.0.tar", max compression
+gzip compressed data, was "weather_command-5.2.1.tar", max compression
```

## Comparing `weather_command-5.2.0.tar` & `weather_command-5.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-03-27 03:35:14.648837 weather_command-5.2.0/LICENSE
--rw-r--r--   0        0        0     2881 2023-03-27 03:35:14.648837 weather_command-5.2.0/README.md
--rw-r--r--   0        0        0     1848 2023-03-27 03:35:14.652837 weather_command-5.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-27 03:35:14.652837 weather_command-5.2.0/weather_command/__init__.py
--rw-r--r--   0        0        0       95 2023-03-27 03:35:14.652837 weather_command-5.2.0/weather_command/__main__.py
--rw-r--r--   0        0        0    18640 2023-03-27 03:35:14.652837 weather_command-5.2.0/weather_command/_builder.py
--rw-r--r--   0        0        0     5260 2023-03-27 03:35:14.652837 weather_command-5.2.0/weather_command/_cache.py
--rw-r--r--   0        0        0     5262 2023-03-27 03:35:14.652837 weather_command-5.2.0/weather_command/_config.py
--rw-r--r--   0        0        0     2546 2023-03-27 03:35:14.652837 weather_command-5.2.0/weather_command/_location.py
--rw-r--r--   0        0        0      473 2023-03-27 03:35:14.652837 weather_command-5.2.0/weather_command/_utils.py
--rw-r--r--   0        0        0     2921 2023-03-27 03:35:14.656837 weather_command-5.2.0/weather_command/_weather.py
--rw-r--r--   0        0        0      459 2023-03-27 03:35:14.656837 weather_command-5.2.0/weather_command/errors.py
--rw-r--r--   0        0        0     9000 2023-03-27 03:35:14.656837 weather_command-5.2.0/weather_command/main.py
--rw-r--r--   0        0        0        0 2023-03-27 03:35:14.656837 weather_command-5.2.0/weather_command/models/__init__.py
--rw-r--r--   0        0        0      133 2023-03-27 03:35:14.656837 weather_command-5.2.0/weather_command/models/location.py
--rw-r--r--   0        0        0     3053 2023-03-27 03:35:14.656837 weather_command-5.2.0/weather_command/models/weather.py
--rw-r--r--   0        0        0        0 2023-03-27 03:35:14.656837 weather_command-5.2.0/weather_command/py.typed
--rw-r--r--   0        0        0     2816 2023-03-27 03:35:14.656837 weather_command-5.2.0/weather_command/settings_commands.py
--rw-r--r--   0        0        0     3928 1970-01-01 00:00:00.000000 weather_command-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-13 14:54:55.800279 weather_command-5.2.1/LICENSE
+-rw-r--r--   0        0        0     2881 2023-04-13 14:54:55.800279 weather_command-5.2.1/README.md
+-rw-r--r--   0        0        0     1849 2023-04-13 14:54:55.804279 weather_command-5.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/__init__.py
+-rw-r--r--   0        0        0       95 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/__main__.py
+-rw-r--r--   0        0        0    18640 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/_builder.py
+-rw-r--r--   0        0        0     5260 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/_cache.py
+-rw-r--r--   0        0        0     5262 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/_config.py
+-rw-r--r--   0        0        0     2546 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/_location.py
+-rw-r--r--   0        0        0      473 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/_utils.py
+-rw-r--r--   0        0        0     2921 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/_weather.py
+-rw-r--r--   0        0        0      459 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/errors.py
+-rw-r--r--   0        0        0     9000 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/main.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/models/__init__.py
+-rw-r--r--   0        0        0      133 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/models/location.py
+-rw-r--r--   0        0        0     3053 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/models/weather.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/py.typed
+-rw-r--r--   0        0        0     2816 2023-04-13 14:54:55.808279 weather_command-5.2.1/weather_command/settings_commands.py
+-rw-r--r--   0        0        0     3928 1970-01-01 00:00:00.000000 weather_command-5.2.1/PKG-INFO
```

### Comparing `weather_command-5.2.0/LICENSE` & `weather_command-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.0/README.md` & `weather_command-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.0/pyproject.toml` & `weather_command-5.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [tool.poetry]
 name = "weather-command"
-version = "5.2.0"
+version = "5.2.1"
 description = "Command line weather app"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/weather-command"
 homepage = "https://github.com/sanders41/weather-command"
 documentation = "https://github.com/sanders41/weather-command"
 keywords = ["weather", "cli"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-rich = "13.3.2"
-httpx = "0.23.3"
+rich = "13.3.4"
+httpx = "0.24.0"
 pydantic = "1.10.7"
 camel-converter = {version = "3.0.0", extras = ["pydantic"]}
 typer = "0.7.0"
 tenacity = "8.2.2"
 pyyaml = "6.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "23.1.0"
-mypy = "1.1.1"
+black = "23.3.0"
+mypy = "1.2.0"
 pre-commit = "2.21.0"
-pytest = "7.2.2"
+pytest = "7.3.0"
 pytest-cov = "4.0.0"
-tox = "4.4.7"
-ruff = "0.0.259"
+tox = "4.4.11"
+ruff = "0.0.261"
 tomli = {version = "2.0.1", python = "<3.11"}
-types-pyyaml = "6.0.12.8"
+types-pyyaml = "6.0.12.9"
 pytest-asyncio = "0.21.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `weather_command-5.2.0/weather_command/_builder.py` & `weather_command-5.2.1/weather_command/_builder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -233,16 +233,16 @@
             show_lines=True,
             expand=True,
         )
         if show_title
         else Table(header_style=HEADER_ROW_STYLE, show_lines=True, expand=True)
     )
     table.add_column("Date/Day :date:")
-    table.add_column(f"Low ({temp_units}) :thermometer:")
     table.add_column(f"High ({temp_units}) :thermometer:")
+    table.add_column(f"Low ({temp_units}) :thermometer:")
     table.add_column("Humidity")
     table.add_column(f"Dew Point ({temp_units})")
     table.add_column(f"Pressure {pressure_units}")
     table.add_column("Conditions")
     table.add_column("UVI")
     table.add_column("Clouds")
     table.add_column("Precipitation Chance")
@@ -289,16 +289,16 @@
     _, _, _, temp_units = _get_units(units)
     table = Table(
         title=f"Daily weather for {location.display_name}",
         header_style=HEADER_ROW_STYLE,
         show_lines=True,
     )
     table.add_column("Date/Day :date:")
-    table.add_column(f"Low ({temp_units}) :thermometer:")
     table.add_column(f"High ({temp_units}) :thermometer:")
+    table.add_column(f"Low ({temp_units}) :thermometer:")
 
     for daily in weather.daily:
         dt = _format_date_time(am_pm, daily.dt, weather.timezone_offset, "daily")
 
         table.add_row(
             dt,
             str(_round_to_int(daily.temp.min)),
```

### Comparing `weather_command-5.2.0/weather_command/_cache.py` & `weather_command-5.2.1/weather_command/_cache.py`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.0/weather_command/_config.py` & `weather_command-5.2.1/weather_command/_config.py`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.0/weather_command/_location.py` & `weather_command-5.2.1/weather_command/_location.py`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.0/weather_command/_weather.py` & `weather_command-5.2.1/weather_command/_weather.py`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.0/weather_command/main.py` & `weather_command-5.2.1/weather_command/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from weather_command._builder import show_current, show_daily, show_hourly
 from weather_command._cache import Cache
 from weather_command._config import console, load_settings
 from weather_command._location import get_location_details
 from weather_command._utils import build_weather_url
 from weather_command._weather import get_current_weather, get_one_call_weather
 
-__version__ = "5.2.0"
+__version__ = "5.2.1"
 
 app = Typer()
 app.add_typer(settings_commands.app, name="settings", help="Manage saved settings.")
 
 
 class ForecastType(str, Enum):
     CURRENT = "current"
```

### Comparing `weather_command-5.2.0/weather_command/models/weather.py` & `weather_command-5.2.1/weather_command/models/weather.py`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.0/weather_command/settings_commands.py` & `weather_command-5.2.1/weather_command/settings_commands.py`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.0/PKG-INFO` & `weather_command-5.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather-command
-Version: 5.2.0
+Version: 5.2.1
 Summary: Command line weather app
 Home-page: https://github.com/sanders41/weather-command
 License: MIT
 Keywords: weather,cli
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -12,18 +12,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: camel-converter[pydantic] (==3.0.0)
-Requires-Dist: httpx (==0.23.3)
+Requires-Dist: httpx (==0.24.0)
 Requires-Dist: pydantic (==1.10.7)
 Requires-Dist: pyyaml (==6.0)
-Requires-Dist: rich (==13.3.2)
+Requires-Dist: rich (==13.3.4)
 Requires-Dist: tenacity (==8.2.2)
 Requires-Dist: typer (==0.7.0)
 Project-URL: Documentation, https://github.com/sanders41/weather-command
 Project-URL: Repository, https://github.com/sanders41/weather-command
 Description-Content-Type: text/markdown
 
 # Weather Command
```

