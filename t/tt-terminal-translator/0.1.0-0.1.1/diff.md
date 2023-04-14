# Comparing `tmp/tt_terminal_translator-0.1.0.tar.gz` & `tmp/tt_terminal_translator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tt_terminal_translator-0.1.0.tar", max compression
+gzip compressed data, was "tt_terminal_translator-0.1.1.tar", max compression
```

## Comparing `tt_terminal_translator-0.1.0.tar` & `tt_terminal_translator-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1895 2023-04-01 04:26:17.248355 tt_terminal_translator-0.1.0/README.md
--rw-r--r--   0        0        0     1725 2023-04-01 04:25:30.141802 tt_terminal_translator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2219 2023-04-01 04:05:18.905475 tt_terminal_translator-0.1.0/src/terminal_translator/config.py
--rw-r--r--   0        0        0     2257 2023-04-01 04:06:17.748559 tt_terminal_translator-0.1.0/src/terminal_translator/main.py
--rw-r--r--   0        0        0     3070 1970-01-01 00:00:00.000000 tt_terminal_translator-0.1.0/setup.py
--rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 tt_terminal_translator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1895 2023-04-01 04:28:41.641347 tt_terminal_translator-0.1.1/README.md
+-rw-r--r--   0        0        0     1725 2023-04-14 02:59:49.209719 tt_terminal_translator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2214 2023-04-14 02:50:58.093918 tt_terminal_translator-0.1.1/src/terminal_translator/config.py
+-rw-r--r--   0        0        0     2297 2023-04-14 02:58:35.636506 tt_terminal_translator-0.1.1/src/terminal_translator/main.py
+-rw-r--r--   0        0        0     3070 1970-01-01 00:00:00.000000 tt_terminal_translator-0.1.1/setup.py
+-rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 tt_terminal_translator-0.1.1/PKG-INFO
```

### Comparing `tt_terminal_translator-0.1.0/README.md` & `tt_terminal_translator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.0/pyproject.toml` & `tt_terminal_translator-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tt-terminal-translator"
-version = "0.1.0"
+version = "0.1.1"
 description = "Terminal Translator is a translation CLI that uses the Google Cloud API. "
 authors = ["gbPagano <guilhermebpagano@gmail.com>"]
 readme = "README.md"
 packages = [{include = "terminal_translator", from = "src"}]
 classifiers = [  
     "Environment :: Console",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `tt_terminal_translator-0.1.0/src/terminal_translator/config.py` & `tt_terminal_translator-0.1.1/src/terminal_translator/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 config_path = Path.home() / ".config" / "terminal_translator" / "credentials.toml"
 config_path.parent.parent.mkdir(exist_ok=True)  # create .config/
 config_path.parent.mkdir(exist_ok=True)  # create terminal_translator/
 config_path.touch()
 
 settings = Dynaconf(
-    envvar_prefix="DYNACONF",
+    envvar_prefix="",
     settings_files=[config_path],
 )
 
 console = Console()
 app_config = Typer(add_completion=False)
 
 
@@ -25,15 +25,15 @@
         ..., help="Project ID of Google Cloud API", show_default=False
     ),
     google_api_credentials: str = Argument(
         ..., help="Path of the json API service key", show_default=False
     ),
 ):
     set_project_id(project_id)
-    set_google_aplication_credentials(google_api_credentials)
+    set_google_application_credentials(google_api_credentials)
 
 
 def set_project_id(credential: str) -> None:
     """Receives the project-id as a parameter and puts it in the configuration file
 
     Args:
         credential (str): project-id
@@ -42,15 +42,15 @@
     configs_json["project_id"] = credential
 
     configs_toml = toml.dumps(configs_json)
     config_path.write_text(configs_toml)
     console.print("The project id has been set", style="green")
 
 
-def set_google_aplication_credentials(json_path: str) -> None:
+def set_google_application_credentials(json_path: str) -> None:
     """Receives the json_path credentials as a parameter,move the file to the
     configuration directory and update its path in the configuration file
 
     Args:
         json_path (str): json_path credentials
     """
     json_path = json_path.replace("~", str(Path().home()))
@@ -58,14 +58,14 @@
     json_file.replace(config_path.parent / json_file.name)
     console.print(
         f"The credential file has been moved to: {config_path.parent / json_file.name}",
         style="yellow",
     )
 
     configs_json = toml.load(config_path)
-    configs_json["google_aplication_credentials"] = str(
+    configs_json["google_application_credentials"] = str(
         config_path.parent / json_file.name
     )
 
     configs_toml = toml.dumps(configs_json)
     config_path.write_text(configs_toml)
     console.print("The google aplication credential has been set", style="green")
```

### Comparing `tt_terminal_translator-0.1.0/src/terminal_translator/main.py` & `tt_terminal_translator-0.1.1/src/terminal_translator/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import os
 from typing import List
 
 import pyperclip
 from google.cloud import translate
 from rich.console import Console
 from typer import Argument, Option, Typer
 
 from .config import settings
 
 try:
-    GOOGLE_APLICATION_CREDENTIALS = settings.google_aplication_credentials
+    os.environ[
+        "GOOGLE_APPLICATION_CREDENTIALS"
+    ] = settings.google_application_credentials
     PROJECT_ID = settings.project_id
 except AttributeError:
     raise Exception(
         "Please configure your credentials with the command: `tt-configure`"
     )
```

### Comparing `tt_terminal_translator-0.1.0/setup.py` & `tt_terminal_translator-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['tt = terminal_translator.main:app',
                      'tt-configure = terminal_translator.config:app_config']}
 
 setup_kwargs = {
     'name': 'tt-terminal-translator',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Terminal Translator is a translation CLI that uses the Google Cloud API. ',
     'long_description': '# Terminal Translator \n[![Documentation Status](https://readthedocs.org/projects/terminal-translator/badge/?version=latest)](https://terminal-translator.readthedocs.io/en/latest/?badge=latest)\n\nTerminal Translator is a translation CLI that uses the [Google Cloud API](https://cloud.google.com/translate).\n\n## Documentation\n\nSee the [full documentation](https://terminal-translator.readthedocs.io/en/latest/)\n\n## Installation\n\nInstallation is very simple, just run the following command in the terminal:\n\n```bash\npip install tt-terminal-translator\n```\n\n## Basic Usage\n\nThe CLI consists of two commands, `tt` and `tt-configure`.\n\n### tt\n\n`tt` is the main CLI command.\n\n**Usage**\n\nBasically we call the command passing the text to be translated\n\nBy default the text will be translated to `en-us`\n\n```bash\ntt ola mundo\n```\n![tt](./docs/assets/images/tt.png)\n\nWe can also inform the target language for the translation\n\n```bash\ntt ola mundo --target es  # spanish\n```\n![tt-2](./docs/assets/images/tt-2.png)\n\nThere is also a parameter to translate directly into Portuguese\n\n```bash\ntt hello world -p\n```\n![tt-3](./docs/assets/images/tt-3.png)\n\n\nIn addition there is a parameter to copy the output directly to the clipboard\n\n```bash\ntt -c hola mundo\n```\n![tt-4](./docs/assets/images/tt-4.png)\n\nFor more information use the parameter `--help`\n\n```bash\ntt --help\n```\n\n![tt-5](./docs/assets/images/tt-5.png)\n\n\n\n### tt-configure\n\n`tt-configure` is only for the initial configuration of the Google Cloud API credentials, as seen in the [settings section](/#configuration).\n\n**Usage**\n\nBasically we call the command passing two arguments, first the project-id followed by the path of the credentials Json file.\n\n```bash\ntt-configure <project-id> <google-api-credentials>\n```\n\nFor quick help use the `--help` argument.\n\n\n```bash\ntt-configure --help\n```\n![tt-configure](./docs/assets/images/tt-configure.png)\n\n',
     'author': 'gbPagano',
     'author_email': 'guilhermebpagano@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tt_terminal_translator-0.1.0/PKG-INFO` & `tt_terminal_translator-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tt-terminal-translator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Terminal Translator is a translation CLI that uses the Google Cloud API. 
 Author: gbPagano
 Author-email: guilhermebpagano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

