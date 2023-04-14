# Comparing `tmp/radicli-0.0.8.tar.gz` & `tmp/radicli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radicli-0.0.8.tar", last modified: Sun Feb 19 16:51:10 2023, max compression
+gzip compressed data, was "radicli-0.0.9.tar", last modified: Tue Feb 21 12:38:16 2023, max compression
```

## Comparing `radicli-0.0.8.tar` & `radicli-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 16:51:10.138556 radicli-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-19 16:51:01.000000 radicli-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-19 16:51:01.000000 radicli-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    27813 2023-02-19 16:51:10.138556 radicli-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26841 2023-02-19 16:51:01.000000 radicli-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-19 16:51:01.000000 radicli-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 16:51:10.138556 radicli-0.0.8/radicli/
--rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-02-19 16:51:01.000000 radicli-0.0.8/radicli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-02-19 16:51:01.000000 radicli-0.0.8/radicli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 16:51:01.000000 radicli-0.0.8/radicli/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 16:51:10.138556 radicli-0.0.8/radicli/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 16:51:01.000000 radicli-0.0.8/radicli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20049 2023-02-19 16:51:01.000000 radicli-0.0.8/radicli/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-02-19 16:51:01.000000 radicli-0.0.8/radicli/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-02-19 16:51:01.000000 radicli-0.0.8/radicli/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 16:51:10.138556 radicli-0.0.8/radicli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27813 2023-02-19 16:51:10.000000 radicli-0.0.8/radicli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-19 16:51:10.000000 radicli-0.0.8/radicli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 16:51:10.000000 radicli-0.0.8/radicli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-19 16:51:10.000000 radicli-0.0.8/radicli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 16:51:09.000000 radicli-0.0.8/radicli.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-02-19 16:51:10.138556 radicli-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-19 16:51:01.000000 radicli-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:38:16.274052 radicli-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-21 12:38:07.000000 radicli-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-21 12:38:07.000000 radicli-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    34474 2023-02-21 12:38:16.274052 radicli-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33502 2023-02-21 12:38:07.000000 radicli-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-21 12:38:07.000000 radicli-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:38:16.274052 radicli-0.0.9/radicli/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-02-21 12:38:07.000000 radicli-0.0.9/radicli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-02-21 12:38:07.000000 radicli-0.0.9/radicli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-02-21 12:38:07.000000 radicli-0.0.9/radicli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 12:38:07.000000 radicli-0.0.9/radicli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-21 12:38:07.000000 radicli-0.0.9/radicli/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:38:16.274052 radicli-0.0.9/radicli/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 12:38:07.000000 radicli-0.0.9/radicli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22404 2023-02-21 12:38:07.000000 radicli-0.0.9/radicli/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-02-21 12:38:07.000000 radicli-0.0.9/radicli/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-02-21 12:38:07.000000 radicli-0.0.9/radicli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:38:16.274052 radicli-0.0.9/radicli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    34474 2023-02-21 12:38:16.000000 radicli-0.0.9/radicli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-21 12:38:16.000000 radicli-0.0.9/radicli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 12:38:16.000000 radicli-0.0.9/radicli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-21 12:38:16.000000 radicli-0.0.9/radicli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 12:38:16.000000 radicli-0.0.9/radicli.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-02-21 12:38:16.274052 radicli-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-21 12:38:07.000000 radicli-0.0.9/setup.py
```

### Comparing `radicli-0.0.8/LICENSE` & `radicli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `radicli-0.0.8/PKG-INFO` & `radicli-0.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,12 @@
-Metadata-Version: 2.1
-Name: radicli
-Version: 0.0.8
-Summary: Radically lightweight command-line interfaces
-Home-page: https://github.com/explosion/radicli
-Author: Explosion
-Author-email: contact@explosion.ai
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # radicli: Radically lightweight command-line interfaces
 
-`radicli` is a small, zero-dependency Python package for creating command line interfaces, built on top of Python's [`argparse`](https://docs.python.org/3/library/argparse.html) module. It introduces minimal overhead, preserves your original Python functions and uses type hints to parse values provided on the CLI. It supports all common types out-of-the-box, including complex ones like `List[str]`, `Literal` and `Enum`, and allows registering custom types with custom converters, as well as custom CLI-only error handling.
+`radicli` is a small, zero-dependency Python package for creating command line interfaces, built on top of Python's [`argparse`](https://docs.python.org/3/library/argparse.html) module. It introduces minimal overhead, preserves your original Python functions and uses **type hints** to parse values provided on the CLI. It supports all common types out-of-the-box, including complex ones like `List[str]`, `Literal` and `Enum`, and allows registering **custom types** with custom converters, as well as custom CLI-only **error handling** and exporting a **static representation** for faster `--help` and errors.
 
 > **Important note:** This package aims to be a simple option based on the requirements of our libraries. If you're looking for a more full-featured CLI toolkit, check out [`typer`](https://typer.tiangolo.com), [`click`](https://click.palletsprojects.com) or [`plac`](https://plac.readthedocs.io/en/latest/).
 
 [![GitHub Actions](https://github.com/explosion/radicli/actions/workflows/test.yml/badge.svg)](https://github.com/explosion/radicli/actions/workflows/test.yml)
 [![Current Release Version](https://img.shields.io/github/v/release/explosion/radicli.svg?style=flat-square&include_prereleases&logo=github)](https://github.com/explosion/radicli/releases)
 [![pypi Version](https://img.shields.io/pypi/v/radicli.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/radicli/)
 
@@ -306,14 +280,41 @@
 
 def handle_custom_error(error: CustomError) -> int:
     print(colored(error.text, "red"))
     print(error.additional_info)
     return 1
 ```
 
+### Using static data for faster help and errors
+
+CLIs often require various other Python packages that need to be imported – for example, you might need to import `pytorch` and `tensorflow`, or load other resources in the global scope. This all adds to the CLI's load time, so even showing the `--help` message may take several seconds to run. That's all unnecessary and makes for a frustrating developer experience.
+
+`radicli` lets you generate a static representation of your CLI as a JSON file, including everything needed to output help messages and to check that the command exists and the correct and required arguments are provided. If the static CLI doesn't perform a system exit via printing the help message or raising an error, you can import and run the "live" CLI to continue. This lets you **defer the import until it's really needed**, i.e. to convert the arguments to the expected types and executing the command function.
+
+```python
+cli.to_static("./static.json")
+```
+
+```python
+from radicli import StaticRadicli
+
+static = StaticRadicli.load("./static.json")
+
+if __name__ == "__main__":
+    static.run()
+
+    # This only runs if the static CLI doesn't error or print help
+    from .cli import cli
+    cli.run()
+```
+
+If the CLI is part of a Python package, you can generate the static JSON file during your build process and ship the pre-generated JSON file with your package.
+
+`StaticRadicli` also provides a `disable` argument to disable static parsing during development (or if a certain environment variable is set). Setting `debug=True` will print an additional start and optional end marker (if the static CLI didn't exit before) to indicate that the static CLI ran.
+
 ## 🎛 API
 
 ### <kbd>dataclass</kbd> `Arg`
 
 Dataclass for describing argument meta information. This is typically used in the command decorators and only includes information for how the argument should be handled on the CLI. Argument types and defaults are read from the Python function.
 
 | Argument    | Type                             | Description                                                                                                 |
@@ -428,15 +429,15 @@
 $ python cli.py hello world Alex
 Hello world, Alex!
 ```
 
 ```python
 @cli.subcommand_with_extra("hello", "world", name=Arg(help="Your name"))
 def hello_world(name: str, _extra: List[str]) -> None:
-    print(f"Hello world, {name}!", _extra])
+    print(f"Hello world, {name}!", _extra)
 ```
 
 ```
 $ python cli.py hello world Alex --color blue
 Hello world, Alex! ['--color', 'blue']
 ```
 
@@ -474,14 +475,98 @@
     cli.run()
 ```
 
 | Argument | Type                  | Description                                                                               |
 | -------- | --------------------- | ----------------------------------------------------------------------------------------- |
 | `args`   | `Optional[List[str]]` | Optional command to pass in. Will be read from `sys.argv` if not set (standard use case). |
 
+#### <kbd>method</kbd> `Radicli.to_static`
+
+Export a static JSON representation of the CLI for `StaticRadicli`.
+
+```python
+cli.to_static("./static.json")
+```
+
+| Argument    | Type               | Description                     |
+| ----------- | ------------------ | ------------------------------- |
+| `file_path` | `Union[str, Path]` | The path to the JSON file.      |
+| **RETURNS** | `Path`             | The path the data was saved to. |
+
+#### <kbd>method</kbd> `Radicli.to_static_json`
+
+Generate a static representation of the CLI for `StaticRadicli` as a JSON-serializable dict.
+
+```python
+data = cli.to_static_json()
+```
+
+| Argument    | Type             | Description      |
+| ----------- | ---------------- | ---------------- |
+| **RETURNS** | `Dict[str, Any]` | The static data. |
+
+### <kbd>class</kbd> `StaticRadicli`
+
+Subclass of `Radicli` and static version of the CLI that can be loaded from a static representation of the CLI, generated with `Radicli.to_static`. The static CLI can run before importing and running the live CLI and will take care of showing help messages and doing basic argument checks, e.g. to ensure all arguments are correct and present. This can make your CLI help significantly faster by deferring the import of the live CLI until it's really needed, i.e. to convert the values and execute the function.
+
+```python
+static = StaticRadicli.load("./static.json")
+
+if __name__ == "__main__":
+    static.run()
+    # This only runs if the static CLI doesn't error or print help
+    from .cli import cli
+    cli.run()
+```
+
+#### <kbd>classmethod</kbd> `StaticRadicli.load`
+
+Load the static CLI from a JSON file generated with `Radicli.to_static`.
+
+```python
+static = StaticRadicli.load("./static.json")
+```
+
+| Argument    | Type               | Description                                                                                                                                                                  |
+| ----------- | ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `file_path` | `Union[str, Path]` | The JSON file to load.                                                                                                                                                       |
+| `disable`   | `bool`             | Whether to disable static parsing. Can be useful during development. Defaults to `False`.                                                                                    |
+| `debug`     | `bool`             | Enable debugging mode and print an additional start and optional end marker (if the static CLI didn't exit before) to indicate that the static CLI ran. Defaults to `False`. |
+
+#### <kbd>method</kbd> `StaticRadicli.__init__`
+
+Initialize the static CLI with the JSON-serializable static representation.
+
+```python
+data = cli.to_static_json()
+static = StaticRadicli(data)
+```
+
+| Argument  | Type             | Description                                                                                                                                                                  |
+| --------- | ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `data`    | `Dict[str, Any]` | The static data.                                                                                                                                                             |
+| `disable` | `bool`           | Whether to disable static parsing. Can be useful during development. Defaults to `False`.                                                                                    |
+| `debug`   | `bool`           | Enable debugging mode and print an additional start and optional end marker (if the static CLI didn't exit before) to indicate that the static CLI ran. Defaults to `False`. |
+
+#### <kbd>method</kbd> `StaticRadicli.run`
+
+Run the static CLI. Typically called before running the live CLI and will perform a system exit if a help message was printed (`0`) or if argument names were missing or incorrect (`1`). This means you can defer loading the live CLI until it's really needed, , i.e. to convert the values and execute the function.
+
+```python
+if __name__ == "__main__":
+    static.run()
+
+    from .cli import cli
+    cli.run()
+```
+
+| Argument | Type                  | Description                                                                               |
+| -------- | --------------------- | ----------------------------------------------------------------------------------------- |
+| `args`   | `Optional[List[str]]` | Optional command to pass in. Will be read from `sys.argv` if not set (standard use case). |
+
 ### Custom types and converters
 
 The package includes several custom types implemented as `TypeVar`s with pre-defined converter functions. If these custom types are used in the decorated function, the values received from the CLI will be converted and validated accordingly.
 
 | Name                     | Type                        | Description                                                                                                                             |
 | ------------------------ | --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
 | `ExistingPath`           | `Path`                      | Returns a path and checks that it exists.                                                                                               |
```

### Comparing `radicli-0.0.8/README.md` & `radicli-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,38 @@
+Metadata-Version: 2.1
+Name: radicli
+Version: 0.0.9
+Summary: Radically lightweight command-line interfaces
+Home-page: https://github.com/explosion/radicli
+Author: Explosion
+Author-email: contact@explosion.ai
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # radicli: Radically lightweight command-line interfaces
 
-`radicli` is a small, zero-dependency Python package for creating command line interfaces, built on top of Python's [`argparse`](https://docs.python.org/3/library/argparse.html) module. It introduces minimal overhead, preserves your original Python functions and uses type hints to parse values provided on the CLI. It supports all common types out-of-the-box, including complex ones like `List[str]`, `Literal` and `Enum`, and allows registering custom types with custom converters, as well as custom CLI-only error handling.
+`radicli` is a small, zero-dependency Python package for creating command line interfaces, built on top of Python's [`argparse`](https://docs.python.org/3/library/argparse.html) module. It introduces minimal overhead, preserves your original Python functions and uses **type hints** to parse values provided on the CLI. It supports all common types out-of-the-box, including complex ones like `List[str]`, `Literal` and `Enum`, and allows registering **custom types** with custom converters, as well as custom CLI-only **error handling** and exporting a **static representation** for faster `--help` and errors.
 
 > **Important note:** This package aims to be a simple option based on the requirements of our libraries. If you're looking for a more full-featured CLI toolkit, check out [`typer`](https://typer.tiangolo.com), [`click`](https://click.palletsprojects.com) or [`plac`](https://plac.readthedocs.io/en/latest/).
 
 [![GitHub Actions](https://github.com/explosion/radicli/actions/workflows/test.yml/badge.svg)](https://github.com/explosion/radicli/actions/workflows/test.yml)
 [![Current Release Version](https://img.shields.io/github/v/release/explosion/radicli.svg?style=flat-square&include_prereleases&logo=github)](https://github.com/explosion/radicli/releases)
 [![pypi Version](https://img.shields.io/pypi/v/radicli.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/radicli/)
 
@@ -280,14 +306,41 @@
 
 def handle_custom_error(error: CustomError) -> int:
     print(colored(error.text, "red"))
     print(error.additional_info)
     return 1
 ```
 
+### Using static data for faster help and errors
+
+CLIs often require various other Python packages that need to be imported – for example, you might need to import `pytorch` and `tensorflow`, or load other resources in the global scope. This all adds to the CLI's load time, so even showing the `--help` message may take several seconds to run. That's all unnecessary and makes for a frustrating developer experience.
+
+`radicli` lets you generate a static representation of your CLI as a JSON file, including everything needed to output help messages and to check that the command exists and the correct and required arguments are provided. If the static CLI doesn't perform a system exit via printing the help message or raising an error, you can import and run the "live" CLI to continue. This lets you **defer the import until it's really needed**, i.e. to convert the arguments to the expected types and executing the command function.
+
+```python
+cli.to_static("./static.json")
+```
+
+```python
+from radicli import StaticRadicli
+
+static = StaticRadicli.load("./static.json")
+
+if __name__ == "__main__":
+    static.run()
+
+    # This only runs if the static CLI doesn't error or print help
+    from .cli import cli
+    cli.run()
+```
+
+If the CLI is part of a Python package, you can generate the static JSON file during your build process and ship the pre-generated JSON file with your package.
+
+`StaticRadicli` also provides a `disable` argument to disable static parsing during development (or if a certain environment variable is set). Setting `debug=True` will print an additional start and optional end marker (if the static CLI didn't exit before) to indicate that the static CLI ran.
+
 ## 🎛 API
 
 ### <kbd>dataclass</kbd> `Arg`
 
 Dataclass for describing argument meta information. This is typically used in the command decorators and only includes information for how the argument should be handled on the CLI. Argument types and defaults are read from the Python function.
 
 | Argument    | Type                             | Description                                                                                                 |
@@ -402,15 +455,15 @@
 $ python cli.py hello world Alex
 Hello world, Alex!
 ```
 
 ```python
 @cli.subcommand_with_extra("hello", "world", name=Arg(help="Your name"))
 def hello_world(name: str, _extra: List[str]) -> None:
-    print(f"Hello world, {name}!", _extra])
+    print(f"Hello world, {name}!", _extra)
 ```
 
 ```
 $ python cli.py hello world Alex --color blue
 Hello world, Alex! ['--color', 'blue']
 ```
 
@@ -448,14 +501,98 @@
     cli.run()
 ```
 
 | Argument | Type                  | Description                                                                               |
 | -------- | --------------------- | ----------------------------------------------------------------------------------------- |
 | `args`   | `Optional[List[str]]` | Optional command to pass in. Will be read from `sys.argv` if not set (standard use case). |
 
+#### <kbd>method</kbd> `Radicli.to_static`
+
+Export a static JSON representation of the CLI for `StaticRadicli`.
+
+```python
+cli.to_static("./static.json")
+```
+
+| Argument    | Type               | Description                     |
+| ----------- | ------------------ | ------------------------------- |
+| `file_path` | `Union[str, Path]` | The path to the JSON file.      |
+| **RETURNS** | `Path`             | The path the data was saved to. |
+
+#### <kbd>method</kbd> `Radicli.to_static_json`
+
+Generate a static representation of the CLI for `StaticRadicli` as a JSON-serializable dict.
+
+```python
+data = cli.to_static_json()
+```
+
+| Argument    | Type             | Description      |
+| ----------- | ---------------- | ---------------- |
+| **RETURNS** | `Dict[str, Any]` | The static data. |
+
+### <kbd>class</kbd> `StaticRadicli`
+
+Subclass of `Radicli` and static version of the CLI that can be loaded from a static representation of the CLI, generated with `Radicli.to_static`. The static CLI can run before importing and running the live CLI and will take care of showing help messages and doing basic argument checks, e.g. to ensure all arguments are correct and present. This can make your CLI help significantly faster by deferring the import of the live CLI until it's really needed, i.e. to convert the values and execute the function.
+
+```python
+static = StaticRadicli.load("./static.json")
+
+if __name__ == "__main__":
+    static.run()
+    # This only runs if the static CLI doesn't error or print help
+    from .cli import cli
+    cli.run()
+```
+
+#### <kbd>classmethod</kbd> `StaticRadicli.load`
+
+Load the static CLI from a JSON file generated with `Radicli.to_static`.
+
+```python
+static = StaticRadicli.load("./static.json")
+```
+
+| Argument    | Type               | Description                                                                                                                                                                  |
+| ----------- | ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `file_path` | `Union[str, Path]` | The JSON file to load.                                                                                                                                                       |
+| `disable`   | `bool`             | Whether to disable static parsing. Can be useful during development. Defaults to `False`.                                                                                    |
+| `debug`     | `bool`             | Enable debugging mode and print an additional start and optional end marker (if the static CLI didn't exit before) to indicate that the static CLI ran. Defaults to `False`. |
+
+#### <kbd>method</kbd> `StaticRadicli.__init__`
+
+Initialize the static CLI with the JSON-serializable static representation.
+
+```python
+data = cli.to_static_json()
+static = StaticRadicli(data)
+```
+
+| Argument  | Type             | Description                                                                                                                                                                  |
+| --------- | ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `data`    | `Dict[str, Any]` | The static data.                                                                                                                                                             |
+| `disable` | `bool`           | Whether to disable static parsing. Can be useful during development. Defaults to `False`.                                                                                    |
+| `debug`   | `bool`           | Enable debugging mode and print an additional start and optional end marker (if the static CLI didn't exit before) to indicate that the static CLI ran. Defaults to `False`. |
+
+#### <kbd>method</kbd> `StaticRadicli.run`
+
+Run the static CLI. Typically called before running the live CLI and will perform a system exit if a help message was printed (`0`) or if argument names were missing or incorrect (`1`). This means you can defer loading the live CLI until it's really needed, , i.e. to convert the values and execute the function.
+
+```python
+if __name__ == "__main__":
+    static.run()
+
+    from .cli import cli
+    cli.run()
+```
+
+| Argument | Type                  | Description                                                                               |
+| -------- | --------------------- | ----------------------------------------------------------------------------------------- |
+| `args`   | `Optional[List[str]]` | Optional command to pass in. Will be read from `sys.argv` if not set (standard use case). |
+
 ### Custom types and converters
 
 The package includes several custom types implemented as `TypeVar`s with pre-defined converter functions. If these custom types are used in the decorated function, the values received from the CLI will be converted and validated accordingly.
 
 | Name                     | Type                        | Description                                                                                                                             |
 | ------------------------ | --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
 | `ExistingPath`           | `Path`                      | Returns a path and checks that it exists.                                                                                               |
```

### Comparing `radicli-0.0.8/radicli/__init__.py` & `radicli-0.0.9/radicli/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Tuple, cast
+from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Tuple
+from typing import Union, cast
 import sys
 from dataclasses import dataclass
 from inspect import signature
+from pathlib import Path
+import json
 
 from .parser import ArgumentParser, HelpFormatter
 from .util import Arg, ArgparseArg, get_arg, join_strings, format_type, format_table
 from .util import format_arg_help, expand_error_subclasses, SimpleFrozenDict
 from .util import CommandNotFoundError, CliParserError, CommandExistsError
-from .util import ConverterType, ConvertersType, ErrorHandlersType
-from .util import DEFAULT_CONVERTERS, DEFAULT_PLACEHOLDER
-
-# Make available for import
-from .util import ExistingPath, ExistingFilePath, ExistingDirPath
-from .util import ExistingPathOrDash, ExistingFilePathOrDash, PathOrDash
-from .util import ExistingDirPathOrDash
+from .util import ConverterType, ConvertersType, ErrorHandlersType, StaticCommand
+from .util import StaticData, DEFAULT_CONVERTERS, DEFAULT_PLACEHOLDER
 
 
 _CallableT = TypeVar("_CallableT", bound=Callable)
 
 
 @dataclass
 class Command:
@@ -29,18 +27,42 @@
     parent: Optional[str] = None
     is_placeholder: bool = False
 
     @property
     def display_name(self) -> str:
         return f"{self.parent} {self.name}" if self.parent else self.name
 
+    def to_static_json(self) -> StaticCommand:
+        """Convert the command to a JSON-serializable dict."""
+        return {
+            "name": self.name,
+            "args": [arg.to_static_json() for arg in self.args],
+            "description": self.description,
+            "allow_extra": self.allow_extra,
+            "parent": self.parent,
+            "is_placeholder": self.is_placeholder,
+        }
+
+    @classmethod
+    def from_static_json(cls, data: StaticCommand) -> "Command":
+        """Initialize the static command from a JSON-serializable dict."""
+        return cls(
+            name=data["name"],
+            func=lambda *args, **kwargs: None,  # dummy function for static use
+            args=[ArgparseArg.from_static_json(arg) for arg in data["args"]],
+            description=data["description"],
+            allow_extra=data["allow_extra"],
+            parent=data["parent"],
+            is_placeholder=data["is_placeholder"],
+        )
+
 
 class Radicli:
     prog: Optional[str]
-    help: Optional[str]
+    help: str
     version: Optional[str]
     converters: ConvertersType
     extra_key: str
     commands: Dict[str, Command]
     subcommands: Dict[str, Dict[str, Command]]
     errors: ErrorHandlersType
     _subcommand_key: str
@@ -194,82 +216,80 @@
 
     def placeholder(self, name: str, *, description: Optional[str] = None) -> None:
         """Add empty parent command placeholder with help for subcommands."""
         if name in self.commands:
             raise CommandExistsError(name)
 
         def func(*args, **kwargs) -> None:
-            subcommands = self.subcommands.get(name, {})
+            sub = self.subcommands.get(name, {})
             # If this runs, we want to show the help instead of doing nothing
-            self.parse(["--help"], [], subcommands, name=name, description=description)
+            self.parse([self._help_arg], [], sub, name=name, description=description)
 
         dummy = Command(
             name=name, func=func, args=[], description=description, is_placeholder=True
         )
         self.commands[name] = dummy
 
     def run(self, args: Optional[List[str]] = None) -> None:
         """
         Run the CLI. Should typically be used in the __main__.py nested under a
         `if __name__ == "__main__":` block.
         """
-        run_args = args if args is not None else sys.argv
+        run_args = args if args is not None else [*sys.argv]
         if len(run_args) <= 1 or run_args[1] == self._help_arg:
-            print(self._format_info())
-        else:
-            # Make single command CLIs available without command name
-            if len(self.commands) == 1 and len(self.subcommands) <= 1:
-                single_cmd = list(self.commands.keys())[0]
-                if run_args[1] != single_cmd:
-                    run_args.insert(1, single_cmd)
-            command = run_args.pop(1)
-            args = run_args[1:]
-            if self.version and command == self._version_arg:
-                print(self.version)
-                sys.exit(0)
-            subcommands = self.subcommands.get(command, {})
-            if command not in self.commands:
-                if not subcommands:
-                    raise CommandNotFoundError(command, list(self.commands))
-                # Add a dummy parent to support subcommands without parents
-                self.placeholder(command)
-            cmd = self.commands[command]
-            values = self.parse(
-                args,
-                cmd.args,
-                subcommands,
-                name=cmd.name,
-                description=cmd.description,
-                allow_extra=cmd.allow_extra,
-            )
-            sub = values.pop(self._subcommand_key, None)
-            func = subcommands[sub].func if sub else cmd.func
-            # Catch specific error types (and their subclasses), and invoke
-            # their handler callback. Handlers can return an integer exit code,
-            # which will be passed to sys.exit.
-            errors_map = expand_error_subclasses(self.errors)
-            try:
-                func(**values)
-            except tuple(errors_map.keys()) as e:
-                handler = errors_map[e.__class__]
-                err_code = handler(e)
-                if err_code is not None:
-                    sys.exit(err_code)
+            print(self.format_info())
+            sys.exit(0)
+        # Make single command CLIs available without command name
+        if len(self.commands) == 1 and len(self.subcommands) <= 1:
+            single_cmd = list(self.commands.keys())[0]
+            if run_args[1] != single_cmd:
+                run_args.insert(1, single_cmd)
+        command = run_args.pop(1)
+        args = run_args[1:]
+        if self.version and command == self._version_arg:
+            print(self.version)
+            sys.exit(0)
+        subcommands = self.subcommands.get(command, {})
+        if command not in self.commands:
+            if not subcommands:
+                raise CommandNotFoundError(command, list(self.commands))
+            # Add a dummy parent to support subcommands without parents
+            self.placeholder(command)
+        cmd = self.commands[command]
+        values = self.parse(
+            args,
+            cmd.args,
+            subcommands,
+            name=cmd.name,
+            description=cmd.description,
+            allow_extra=cmd.allow_extra,
+        )
+        sub = values.pop(self._subcommand_key, None)
+        func = subcommands[sub].func if sub else cmd.func
+        # Catch specific error types (and their subclasses), and invoke
+        # their handler callback. Handlers can return an integer exit code,
+        # which will be passed to sys.exit.
+        errors_map = expand_error_subclasses(self.errors)
+        try:
+            func(**values)
+        except tuple(errors_map.keys()) as e:
+            handler = errors_map[e.__class__]
+            err_code = handler(e)
+            if err_code is not None:
+                sys.exit(err_code)
 
-    def parse(
+    def get_parsers(
         self,
-        args: List[str],
         arg_info: List[ArgparseArg],
         subcommands: Dict[str, Command] = SimpleFrozenDict(),
         *,
         name: Optional[str] = None,
         description: Optional[str] = None,
-        allow_extra: bool = False,
-    ) -> Dict[str, Any]:
-        """Parse a list of arguments. Can also be used for testing."""
+    ) -> Tuple[ArgumentParser, Dict[str, Tuple[ArgumentParser, Command]]]:
+        """Get parser for a given command."""
         p = ArgumentParser(
             prog=join_strings(self.prog, name),
             description=description,
             formatter_class=HelpFormatter,
             add_help=not any(a.arg.option == self._help_arg for a in arg_info),
             argument_default=DEFAULT_PLACEHOLDER,
         )
@@ -293,14 +313,30 @@
                     prog=join_strings(self.prog, sub_cmd.parent, sub_name),
                     add_help=add_help,
                     formatter_class=HelpFormatter,
                     argument_default=DEFAULT_PLACEHOLDER,
                 )
                 subparsers[sub_cmd.name] = (subp, sub_cmd)
                 self._add_args(subp, sub_cmd.args)
+        return p, subparsers
+
+    def parse(
+        self,
+        args: List[str],
+        arg_info: List[ArgparseArg],
+        subcommands: Dict[str, Command] = SimpleFrozenDict(),
+        *,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        allow_extra: bool = False,
+    ) -> Dict[str, Any]:
+        """Parse a list of arguments. Can also be used for testing."""
+        p, subparsers = self.get_parsers(
+            arg_info, subcommands, name=name, description=description
+        )
         # Handling of subcommands is a bit convoluted
         # https://docs.python.org/3/library/argparse.html#sub-commands
         namespace, extra = p.parse_known_args(args)
         values = {**vars(namespace), self.extra_key: extra}
         sub_key = values.pop(self._subcommand_key, None)
         if not sub_key:  # we're not in a subcommand
             cmds = self.commands[name] if name in self.commands else None
@@ -340,33 +376,45 @@
                 if arg.id not in values or values[arg.id] is DEFAULT_PLACEHOLDER:
                     required.append(arg.arg.option or arg.id)
             if required:
                 err = f"the following arguments are required: {', '.join(required)}"
                 raise CliParserError(err)
         return values
 
-    def _format_info(self) -> str:
+    def format_info(self) -> str:
         """Nicely format the available command overview and add subcommands."""
         data = []
         for name, cmd in self.commands.items():
             data.append((f"  {name}", format_arg_help(cmd.description)))
             if name in self.subcommands:
                 col = f"Subcommands: {', '.join(self.subcommands[name])}"
                 data.append(("", col))
         for name in self.subcommands:
             if name not in self.commands:
                 col = f"Subcommands: {', '.join(self.subcommands[name])}"
                 data.append((f"  {name}", col))
         info = [self.help, "\nAvailable commands:", format_table(data)]
         return join_strings(*info, char="\n")
 
-
-# fmt: off
-__all__ = [
-    "Radicli", "ArgumentParser", "HelpFormatter", "Command", "Arg", "ArgparseArg",
-    "get_arg", "format_type", "CommandNotFoundError", "CliParserError",
-    "CommandExistsError", "ConvertersType", "ConverterType", "ErrorHandlersType",
-    "DEFAULT_PLACEHOLDER", "ExistingPath", "ExistingFilePath", "ExistingDirPath",
-    "ExistingPathOrDash", "ExistingFilePathOrDash", "PathOrDash",
-    "ExistingDirPathOrDash"
-]
-# fmt: on
+    def to_static_json(self) -> StaticData:
+        """Convert the CLI to a JSON-serializable dict."""
+        return {
+            "prog": self.prog,
+            "help": self.help,
+            "version": self.version,
+            "extra_key": self.extra_key,
+            "commands": {
+                cmd.name: cmd.to_static_json() for cmd in self.commands.values()
+            },
+            "subcommands": {
+                parent: {sub.name: sub.to_static_json() for sub in subs.values()}
+                for parent, subs in self.subcommands.items()
+            },
+        }
+
+    def to_static(self, file_path: Union[str, Path]) -> Path:
+        """Generate a static representation of the CLI for StaticRadicli."""
+        data = self.to_static_json()
+        path = Path(file_path)
+        with path.open("w", encoding="utf8") as f:
+            f.write(json.dumps(data))
+        return path
```

### Comparing `radicli-0.0.8/radicli/parser.py` & `radicli-0.0.9/radicli/parser.py`

 * *Files identical despite different names*

### Comparing `radicli-0.0.8/radicli/tests/test_cli.py` & `radicli-0.0.9/radicli/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass
 import pytest
 import sys
 from contextlib import contextmanager
 import tempfile
 import shutil
 from pathlib import Path
-from radicli import Radicli, Arg
+from radicli import Radicli, StaticRadicli, Arg
 from radicli.util import CommandNotFoundError, CliParserError
 from radicli.util import ExistingPath, ExistingFilePath, ExistingDirPath
 from radicli.util import ExistingFilePathOrDash
 
 
 @contextmanager
 def make_tempdir() -> Iterator[Path]:
@@ -662,14 +662,15 @@
     with pytest.raises(SystemExit):
         cli.run(["", "--version"])
     captured = capsys.readouterr()
     assert captured.out.strip() == version
     assert not ran1
     assert not ran2
 
+
 def test_cli_single_command():
     """Test that the name can be left out for CLIs with only one command."""
     cli = Radicli()
     ran = False
 
     @cli.command("test", a=Arg("--a"))
     def test(a: str):
@@ -746,7 +747,83 @@
     elif expect_exit:
         with pytest.raises(SystemExit):
             cli.run(["", "test"])
     else:
         cli.run(["", "test"])
         assert ran
         assert handler_ran is expect_handled
+
+
+def test_cli_static_roundtrip(capsys):
+    cli = Radicli(prog="test")
+
+    @cli.command("hello", a=Arg("--a", help="aaa"), b=Arg("--b", help="bbb"))
+    def hello(a, b):
+        """Hello"""
+        ...
+
+    @cli.command("world", c=Arg(help="ccc"))
+    def world(c):
+        """World"""
+        ...
+
+    with make_tempdir() as dir_path:
+        path = dir_path / "static.json"
+        cli.to_static(path)
+
+        static = StaticRadicli.load(path)
+
+    assert static.prog == cli.prog
+    assert len(static.commands) == len(cli.commands)
+    for parent, commands in static.subcommands:
+        assert parent in cli.subcommands
+        assert len(cli.subcommands[parent]) == len(commands)
+
+    hello1 = static.commands["hello"]
+    hello2 = cli.commands["hello"]
+    assert hello1.name == hello2.name
+    assert hello1.description == hello2.description
+    for arg1, arg2 in zip(hello1.args, hello2.args):
+        assert arg1.help == arg2.help
+        assert arg1.arg.option == arg2.arg.option
+        assert arg1.arg.short == arg2.arg.short
+        assert arg1.arg.help == arg2.arg.help
+
+    with pytest.raises(SystemExit):
+        static.run(["", "--help"])
+    captured1 = capsys.readouterr().out
+    with pytest.raises(SystemExit):
+        cli.run(["", "--help"])
+    captured2 = capsys.readouterr().out
+    assert captured1 == captured2
+
+    with pytest.raises(SystemExit):
+        static.run(["", "hello", "--help"])
+    captured1 = capsys.readouterr().out
+    with pytest.raises(SystemExit):
+        cli.run(["", "hello", "--help"])
+    captured2 = capsys.readouterr().out
+    assert captured1 == captured2
+
+    with pytest.raises(SystemExit):
+        static.run(["", "world", "--help"])
+    captured1 = capsys.readouterr().out
+    with pytest.raises(SystemExit):
+        cli.run(["", "world", "--help"])
+    captured2 = capsys.readouterr().out
+    assert captured1 == captured2
+
+    with make_tempdir() as dir_path:
+        path = dir_path / "static.json"
+        cli.to_static(path)
+
+        static = StaticRadicli.load(path, debug=True)
+
+    with pytest.raises(SystemExit):
+        static.run(["", "hello", "--help"])
+    captured = capsys.readouterr().out
+    assert static._debug_start in captured
+
+    static.disable = True
+    static.run(["", "hello", "--help"])
+    captured = capsys.readouterr().out
+    assert not captured
```

### Comparing `radicli-0.0.8/radicli/tests/test_parser.py` & `radicli-0.0.9/radicli/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `radicli-0.0.8/radicli/util.py` & `radicli-0.0.9/radicli/util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,60 @@
 from typing import Any, Callable, Iterable, Type, Union, Optional, Dict, Tuple
-from typing import List, Literal, NewType, get_args, get_origin, TypeVar
+from typing import List, Literal, NewType, get_args, get_origin, TypeVar, TypedDict
 from enum import Enum
 from dataclasses import dataclass
 from pathlib import Path
 import inspect
 import argparse
 
 # We need this Iterable type, which is the type origin of types.Iterable
 try:
     from collections.abc import Iterable as IterableType  # Python 3.9+
 except ImportError:
     from collections import Iterable as IterableType  # type: ignore
 
-
 DEFAULT_PLACEHOLDER = argparse.SUPPRESS
 BASE_TYPES = [str, int, float, Path]
 ConverterType = Callable[[str], Any]
 ConvertersType = Dict[Union[Type, object], ConverterType]
 _Exc = TypeVar("_Exc", bound=Exception, covariant=True)
 ErrorHandlerType = Callable[[Exception], Optional[int]]
 ErrorHandlersType = Dict[Type[_Exc], Callable[[_Exc], Optional[int]]]
 
 
+class StaticArg(TypedDict):
+    id: str
+    option: Optional[str]
+    short: Optional[str]
+    orig_help: Optional[str]
+    default: str
+    help: Optional[str]
+    action: Optional[str]
+    choices: Optional[List[str]]
+    has_converter: bool
+
+
+class StaticCommand(TypedDict):
+    name: str
+    args: List[StaticArg]
+    description: Optional[str]
+    allow_extra: bool
+    parent: Optional[str]
+    is_placeholder: bool
+
+
+class StaticData(TypedDict):
+    prog: Optional[str]
+    help: str
+    version: Optional[str]
+    extra_key: str
+    commands: Dict[str, StaticCommand]
+    subcommands: Dict[str, Dict[str, StaticCommand]]
+
+
 class CliParserError(SystemExit):
     def __init__(self, message: str) -> None:
         self.message = message
         super().__init__(self.message)
 
 
 class UnsupportedTypeError(Exception):
@@ -111,14 +140,47 @@
         # Not all arguments are valid for all options
         if self.type is not None:
             kwargs["type"] = self.type
         if self.choices is not None:
             kwargs["choices"] = self.choices
         return args, kwargs
 
+    def to_static_json(self) -> StaticArg:
+        """Convert the argument to a JSON-serializable dict."""
+        return {
+            "id": self.id,
+            "option": self.arg.option,
+            "short": self.arg.short,
+            "orig_help": self.arg.help,
+            "default": str(self.default),
+            "help": self.help,
+            "action": str(self.action) if self.action else None,
+            "choices": list(c.value if isinstance(c, Enum) else c for c in self.choices)
+            if self.choices
+            else None,
+            "has_converter": self.has_converter,
+        }
+
+    @classmethod
+    def from_static_json(cls, data: StaticArg) -> "ArgparseArg":
+        """Initialize the static argument from a JSON-serializable dict."""
+        return ArgparseArg(
+            id=data["id"],
+            arg=Arg(data["option"], data["short"], help=data["orig_help"]),
+            type=str if not data["action"] else None,  # dummy, not used
+            orig_type=str if not data["action"] else None,  # dummy, not used
+            default=DEFAULT_PLACEHOLDER
+            if data["default"] == DEFAULT_PLACEHOLDER
+            else data["default"],
+            help=data["help"],
+            action=data["action"],
+            choices=data["choices"],
+            has_converter=data["has_converter"],
+        )
+
 
 def get_arg(
     param: str,
     orig_arg: Arg,
     param_type: Any,
     *,
     orig_type: Optional[Union[Type, Callable[[str], Any]]] = None,
```

### Comparing `radicli-0.0.8/radicli.egg-info/PKG-INFO` & `radicli-0.0.9/radicli.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radicli
-Version: 0.0.8
+Version: 0.0.9
 Summary: Radically lightweight command-line interfaces
 Home-page: https://github.com/explosion/radicli
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -24,15 +24,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # radicli: Radically lightweight command-line interfaces
 
-`radicli` is a small, zero-dependency Python package for creating command line interfaces, built on top of Python's [`argparse`](https://docs.python.org/3/library/argparse.html) module. It introduces minimal overhead, preserves your original Python functions and uses type hints to parse values provided on the CLI. It supports all common types out-of-the-box, including complex ones like `List[str]`, `Literal` and `Enum`, and allows registering custom types with custom converters, as well as custom CLI-only error handling.
+`radicli` is a small, zero-dependency Python package for creating command line interfaces, built on top of Python's [`argparse`](https://docs.python.org/3/library/argparse.html) module. It introduces minimal overhead, preserves your original Python functions and uses **type hints** to parse values provided on the CLI. It supports all common types out-of-the-box, including complex ones like `List[str]`, `Literal` and `Enum`, and allows registering **custom types** with custom converters, as well as custom CLI-only **error handling** and exporting a **static representation** for faster `--help` and errors.
 
 > **Important note:** This package aims to be a simple option based on the requirements of our libraries. If you're looking for a more full-featured CLI toolkit, check out [`typer`](https://typer.tiangolo.com), [`click`](https://click.palletsprojects.com) or [`plac`](https://plac.readthedocs.io/en/latest/).
 
 [![GitHub Actions](https://github.com/explosion/radicli/actions/workflows/test.yml/badge.svg)](https://github.com/explosion/radicli/actions/workflows/test.yml)
 [![Current Release Version](https://img.shields.io/github/v/release/explosion/radicli.svg?style=flat-square&include_prereleases&logo=github)](https://github.com/explosion/radicli/releases)
 [![pypi Version](https://img.shields.io/pypi/v/radicli.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/radicli/)
 
@@ -306,14 +306,41 @@
 
 def handle_custom_error(error: CustomError) -> int:
     print(colored(error.text, "red"))
     print(error.additional_info)
     return 1
 ```
 
+### Using static data for faster help and errors
+
+CLIs often require various other Python packages that need to be imported – for example, you might need to import `pytorch` and `tensorflow`, or load other resources in the global scope. This all adds to the CLI's load time, so even showing the `--help` message may take several seconds to run. That's all unnecessary and makes for a frustrating developer experience.
+
+`radicli` lets you generate a static representation of your CLI as a JSON file, including everything needed to output help messages and to check that the command exists and the correct and required arguments are provided. If the static CLI doesn't perform a system exit via printing the help message or raising an error, you can import and run the "live" CLI to continue. This lets you **defer the import until it's really needed**, i.e. to convert the arguments to the expected types and executing the command function.
+
+```python
+cli.to_static("./static.json")
+```
+
+```python
+from radicli import StaticRadicli
+
+static = StaticRadicli.load("./static.json")
+
+if __name__ == "__main__":
+    static.run()
+
+    # This only runs if the static CLI doesn't error or print help
+    from .cli import cli
+    cli.run()
+```
+
+If the CLI is part of a Python package, you can generate the static JSON file during your build process and ship the pre-generated JSON file with your package.
+
+`StaticRadicli` also provides a `disable` argument to disable static parsing during development (or if a certain environment variable is set). Setting `debug=True` will print an additional start and optional end marker (if the static CLI didn't exit before) to indicate that the static CLI ran.
+
 ## 🎛 API
 
 ### <kbd>dataclass</kbd> `Arg`
 
 Dataclass for describing argument meta information. This is typically used in the command decorators and only includes information for how the argument should be handled on the CLI. Argument types and defaults are read from the Python function.
 
 | Argument    | Type                             | Description                                                                                                 |
@@ -428,15 +455,15 @@
 $ python cli.py hello world Alex
 Hello world, Alex!
 ```
 
 ```python
 @cli.subcommand_with_extra("hello", "world", name=Arg(help="Your name"))
 def hello_world(name: str, _extra: List[str]) -> None:
-    print(f"Hello world, {name}!", _extra])
+    print(f"Hello world, {name}!", _extra)
 ```
 
 ```
 $ python cli.py hello world Alex --color blue
 Hello world, Alex! ['--color', 'blue']
 ```
 
@@ -474,14 +501,98 @@
     cli.run()
 ```
 
 | Argument | Type                  | Description                                                                               |
 | -------- | --------------------- | ----------------------------------------------------------------------------------------- |
 | `args`   | `Optional[List[str]]` | Optional command to pass in. Will be read from `sys.argv` if not set (standard use case). |
 
+#### <kbd>method</kbd> `Radicli.to_static`
+
+Export a static JSON representation of the CLI for `StaticRadicli`.
+
+```python
+cli.to_static("./static.json")
+```
+
+| Argument    | Type               | Description                     |
+| ----------- | ------------------ | ------------------------------- |
+| `file_path` | `Union[str, Path]` | The path to the JSON file.      |
+| **RETURNS** | `Path`             | The path the data was saved to. |
+
+#### <kbd>method</kbd> `Radicli.to_static_json`
+
+Generate a static representation of the CLI for `StaticRadicli` as a JSON-serializable dict.
+
+```python
+data = cli.to_static_json()
+```
+
+| Argument    | Type             | Description      |
+| ----------- | ---------------- | ---------------- |
+| **RETURNS** | `Dict[str, Any]` | The static data. |
+
+### <kbd>class</kbd> `StaticRadicli`
+
+Subclass of `Radicli` and static version of the CLI that can be loaded from a static representation of the CLI, generated with `Radicli.to_static`. The static CLI can run before importing and running the live CLI and will take care of showing help messages and doing basic argument checks, e.g. to ensure all arguments are correct and present. This can make your CLI help significantly faster by deferring the import of the live CLI until it's really needed, i.e. to convert the values and execute the function.
+
+```python
+static = StaticRadicli.load("./static.json")
+
+if __name__ == "__main__":
+    static.run()
+    # This only runs if the static CLI doesn't error or print help
+    from .cli import cli
+    cli.run()
+```
+
+#### <kbd>classmethod</kbd> `StaticRadicli.load`
+
+Load the static CLI from a JSON file generated with `Radicli.to_static`.
+
+```python
+static = StaticRadicli.load("./static.json")
+```
+
+| Argument    | Type               | Description                                                                                                                                                                  |
+| ----------- | ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `file_path` | `Union[str, Path]` | The JSON file to load.                                                                                                                                                       |
+| `disable`   | `bool`             | Whether to disable static parsing. Can be useful during development. Defaults to `False`.                                                                                    |
+| `debug`     | `bool`             | Enable debugging mode and print an additional start and optional end marker (if the static CLI didn't exit before) to indicate that the static CLI ran. Defaults to `False`. |
+
+#### <kbd>method</kbd> `StaticRadicli.__init__`
+
+Initialize the static CLI with the JSON-serializable static representation.
+
+```python
+data = cli.to_static_json()
+static = StaticRadicli(data)
+```
+
+| Argument  | Type             | Description                                                                                                                                                                  |
+| --------- | ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `data`    | `Dict[str, Any]` | The static data.                                                                                                                                                             |
+| `disable` | `bool`           | Whether to disable static parsing. Can be useful during development. Defaults to `False`.                                                                                    |
+| `debug`   | `bool`           | Enable debugging mode and print an additional start and optional end marker (if the static CLI didn't exit before) to indicate that the static CLI ran. Defaults to `False`. |
+
+#### <kbd>method</kbd> `StaticRadicli.run`
+
+Run the static CLI. Typically called before running the live CLI and will perform a system exit if a help message was printed (`0`) or if argument names were missing or incorrect (`1`). This means you can defer loading the live CLI until it's really needed, , i.e. to convert the values and execute the function.
+
+```python
+if __name__ == "__main__":
+    static.run()
+
+    from .cli import cli
+    cli.run()
+```
+
+| Argument | Type                  | Description                                                                               |
+| -------- | --------------------- | ----------------------------------------------------------------------------------------- |
+| `args`   | `Optional[List[str]]` | Optional command to pass in. Will be read from `sys.argv` if not set (standard use case). |
+
 ### Custom types and converters
 
 The package includes several custom types implemented as `TypeVar`s with pre-defined converter functions. If these custom types are used in the decorated function, the values received from the CLI will be converted and validated accordingly.
 
 | Name                     | Type                        | Description                                                                                                                             |
 | ------------------------ | --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
 | `ExistingPath`           | `Path`                      | Returns a path and checks that it exists.                                                                                               |
```

### Comparing `radicli-0.0.8/setup.cfg` & `radicli-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.0.8
+version = 0.0.9
 description = Radically lightweight command-line interfaces
 url = https://github.com/explosion/radicli
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
```

