# Comparing `tmp/widgetron-0.1.6.tar.gz` & `tmp/widgetron-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widgetron-0.1.6.tar", last modified: Tue Apr  4 20:00:06 2023, max compression
+gzip compressed data, was "widgetron-0.1.7.tar", last modified: Fri Apr 14 17:06:40 2023, max compression
```

## Comparing `widgetron-0.1.6.tar` & `widgetron-0.1.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:00:06.560877 widgetron-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-04 19:58:46.000000 widgetron-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-04 20:00:06.560877 widgetron-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-04 19:58:46.000000 widgetron-0.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-04 20:00:06.560877 widgetron-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-04 19:58:46.000000 widgetron-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:00:06.556877 widgetron-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:00:06.560877 widgetron-0.1.6/src/widgetron/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/args.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:00:06.560877 widgetron-0.1.6/src/widgetron/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    40675 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/icons/widgetron.icns
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/icons/widgetron.ico
--rw-r--r--   0 runner    (1001) docker     (123)    23698 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/icons/widgetron.png
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/jinja_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/parse_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:00:06.556877 widgetron-0.1.6/src/widgetron/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:00:06.560877 widgetron-0.1.6/src/widgetron/templates/constructor/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/constructor/construct.yaml_template
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/constructor/post_install.sh_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:00:06.560877 widgetron-0.1.6/src/widgetron/templates/electron/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/electron/index.html_template
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/electron/main.js_template
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/electron/package.json_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:00:06.560877 widgetron-0.1.6/src/widgetron/templates/recipe/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/recipe/bld.bat_template
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/recipe/meta.yaml_template
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/recipe/widgetron_shortcut.json_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:00:06.560877 widgetron-0.1.6/src/widgetron/templates/server/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/server/setup.cfg_template
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/server/setup.py_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:00:06.560877 widgetron-0.1.6/src/widgetron/templates/server/widgetron_app/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/server/widgetron_app/__init__.py_template
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/server/widgetron_app/__main__.pyw_template
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/server/widgetron_app/cli.py_template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:00:06.560877 widgetron-0.1.6/src/widgetron/templates/server/widgetron_app/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-04 19:58:46.000000 widgetron-0.1.6/src/widgetron/templates/server/widgetron_app/notebooks/debug.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:00:06.560877 widgetron-0.1.6/src/widgetron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-04 20:00:06.000000 widgetron-0.1.6/src/widgetron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-04 20:00:06.000000 widgetron-0.1.6/src/widgetron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 20:00:06.000000 widgetron-0.1.6/src/widgetron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-04 20:00:06.000000 widgetron-0.1.6/src/widgetron.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 20:00:06.000000 widgetron-0.1.6/src/widgetron.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-04 20:00:06.000000 widgetron-0.1.6/src/widgetron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-04 20:00:06.000000 widgetron-0.1.6/src/widgetron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.900309 widgetron-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 17:04:51.000000 widgetron-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-14 17:06:40.900309 widgetron-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-14 17:04:51.000000 widgetron-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-14 17:06:40.900309 widgetron-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 17:04:51.000000 widgetron-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.892310 widgetron-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.896309 widgetron-0.1.7/src/widgetron/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/args.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.896309 widgetron-0.1.7/src/widgetron/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    40675 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/icons/widgetron.icns
+-rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/icons/widgetron.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    23698 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/icons/widgetron.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/jinja_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/parse_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.892310 widgetron-0.1.7/src/widgetron/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.896309 widgetron-0.1.7/src/widgetron/templates/constructor/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/constructor/construct.yaml_template
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/constructor/post_install.sh_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.900309 widgetron-0.1.7/src/widgetron/templates/electron/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/electron/index.html_template
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/electron/main.js_template
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/electron/package.json_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.900309 widgetron-0.1.7/src/widgetron/templates/recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/recipe/bld.bat_template
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/recipe/meta.yaml_template
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/recipe/widgetron_shortcut.json_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.900309 widgetron-0.1.7/src/widgetron/templates/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/server/setup.cfg_template
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/server/setup.py_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.900309 widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/__init__.py_template
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/__main__.pyw_template
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/cli.py_template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.900309 widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-14 17:04:51.000000 widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/notebooks/debug.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:06:40.896309 widgetron-0.1.7/src/widgetron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 17:06:40.000000 widgetron-0.1.7/src/widgetron.egg-info/top_level.txt
```

### Comparing `widgetron-0.1.6/LICENSE` & `widgetron-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.6/setup.cfg` & `widgetron-0.1.7/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [metadata]
 name = widgetron
 version = attr: widgetron.VERSION
 author = Joel Stansbury
 license = MIT
-long_description = file: README.rst
+long_description_content_type = Markdown
+long_description = file: README.md
 description = Application builder for ipython notebooks
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 zip_safe = False
 package_dir =
```

### Comparing `widgetron-0.1.6/src/widgetron/__main__.py` & `widgetron-0.1.7/src/widgetron/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,24 +75,42 @@
 
     if "explicit_lock" in kwargs:
         with open(kwargs["explicit_lock"], "r") as f:
             l = f.readline()
             while "@EXPLICIT" not in l:
                 l = f.readline()
             kwargs["dependencies"] += [s.strip() for s in f.readlines()]
+        cmd = [
+            "jake",
+            "sbom",
+            "-t=CONDA",
+            f"-f={kwargs['explicit_lock']}",
+            "--output-format=json",
+            f"-o={Path(kwargs['outdir'])/'conda-sbom.json'}"
+        ]
+        print(cmd)
+        call(cmd)
     elif "environment_yaml" in kwargs:
         with open(kwargs["environment_yaml"], "r") as f:
             _env = yaml.safe_load(f)
         kwargs["dependencies"] += _env["dependencies"]
         kwargs["channels"] +=  _env["channels"]
 
     kwargs["server_command"] = kwargs.get("server_command", DEFAULT_SERVER_COMMAND)
     if isinstance(kwargs["server_command"], str):
         kwargs["server_command"]=kwargs["server_command"].strip().split()
 
+    kwargs["url_whitelist"] = kwargs.get("url_whitelist", [])
+    if isinstance(kwargs["url_whitelist"], str):
+        kwargs["url_whitelist"]=kwargs["url_whitelist"].strip().split()
+
+    kwargs["domain_whitelist"] = kwargs.get("domain_whitelist", [])
+    if isinstance(kwargs["domain_whitelist"], str):
+        kwargs["domain_whitelist"]=kwargs["domain_whitelist"].strip().split()
+
     assert isinstance(kwargs["server_command"], list)
     assert "version" in kwargs
 
     kwargs["icon"] = kwargs.get("icon", DEFAULT_ICON)
 
     kwargs["name"] = Path(kwargs["notebook"]).stem
 
@@ -150,14 +168,22 @@
 
     os.chdir(str(kwargs["temp_files"] / "electron"))
     os.mkdir("build")
     # assert icon.suffix.lower() == ".png", "WIP: only png currently supported"
     shutil.copy(str(icon), f"build/icon{icon.suffix}")
 
     call("npm install .", shell=True)
+    sbom = Path(kwargs['outdir']) / 'npm-sbom.json'
+    cmd = [
+        "npm", "run", "lock", "--",
+        "--output-format", "json",
+        "--output-file", f"{sbom}"
+    ]
+    print(cmd)
+    call(cmd, shell=True)
     call(
         "npm run build",
         shell=True,
     )
     if OSX or LINUX:
         dist = "dist"
     elif WIN:
```

### Comparing `widgetron-0.1.6/src/widgetron/args.yml` & `widgetron-0.1.7/src/widgetron/args.yml`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 outdir:
     flag: "-o"
     default: "."
     help: "Where to put the installer."
 
 notebook:
     flag: "-nb"
-    help: "Path to notebook to convert. (must be .ipynb)"
+    help: "Path to notebook to convert. (must be .ipynb or a directory)"
 
 version:
     flag: "-v"
     help: "Version number."
 
 environment_yaml:
     flag: "-env"
@@ -62,14 +62,44 @@
     flag: "-icon"
     help: |
         256 by 256 icon file (must be appropriate to OS)
             win: .ico
             osx: .icns
             linux: .png
 
+url_whitelist:
+    flag: "-url_whitelist"
+    nargs: "+"
+    help: |
+        By default external links do nothing. This is for better security.
+        If a url has been whitelisted, then clicking on it will open the url
+        in the user's default web-browser.
+        Alternatively, you may want to whitelist an entire domain via the
+        domain_whitelist argument.
+
+domain_whitelist:
+    flag: "-domain_whitelist"
+    nargs: "+"
+    help: |
+        By default external links do nothing. This is for better security.
+        If a domain has been whitelisted, then clicking on a url with that domain
+        will open the url in the user's default web-browser.
+        Alternatively, you may want to whitelist specific urls via the
+        url_whitelist argument.
+
+window_style:
+    flag: "-window_style"
+    help: |
+        (Windows only) Set the WindowStyle for powershell.
+    default: Minimized
+    choices:
+        - Hidden
+        - Normal
+        - Minimized
+
 # CONSTRUCTOR_PARAMS
 company:
     flag: "-company"
     help: |
         Name of the company/entity who is responsible for the installer.
 
 installer_filename:
```

### Comparing `widgetron-0.1.6/src/widgetron/icons/widgetron.icns` & `widgetron-0.1.7/src/widgetron/icons/widgetron.icns`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.6/src/widgetron/icons/widgetron.ico` & `widgetron-0.1.7/src/widgetron/icons/widgetron.ico`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.6/src/widgetron/icons/widgetron.png` & `widgetron-0.1.7/src/widgetron/icons/widgetron.png`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.6/src/widgetron/jinja_functions.py` & `widgetron-0.1.7/src/widgetron/jinja_functions.py`

 * *Files identical despite different names*

### Comparing `widgetron-0.1.6/src/widgetron/parse_args.py` & `widgetron-0.1.7/src/widgetron/parse_args.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 parser = argparse.ArgumentParser(
     prog="widgetron",
     description="Creates an app for displaying the output cells of an interactive notebook.",
 )
 
 
-def defaults():
+def config_file():
     if Path("setup.cfg").is_file():
         setup_cfg = configparser.ConfigParser()
         with Path("setup.cfg").open("r") as f:
             setup_cfg.read_file(f)
         if "tool.widgetron" in setup_cfg:
             print("Initialize from setup.cfg")
             return setup_cfg._sections["tool.widgetron"]
@@ -31,24 +31,52 @@
             if "widgetron" in _toml["tool"]:
                 print("Initialize from pyproject.toml")
                 return _toml["tool"]["widgetron"]
     return {}
 
 
 def config():
+    defaults = {}
     with ARGS_FILE.open() as f:
         args = yaml.safe_load(f)
     for k, v in args.items():
         flags = [v.pop("flag"), "--" + k] if "flag" in v else [k]
+        if "default" in v:
+            defaults[k] = v.pop("default")
         parser.add_argument(*flags, **v)
     kwargs = parser.parse_args()
-    kwargs.outdir = Path(kwargs.outdir).absolute()
-    os.chdir(kwargs.directory)
-    res = defaults()
+
+    # Outdir
+    #  If provided to CLI, then relative to CWD
+    if kwargs.outdir is not None:
+        kwargs.outdir = Path(kwargs.outdir).absolute()
+    #  If unspecified, then CWD
+    defaults["outdir"] = Path(defaults["outdir"]).absolute()
+
+    # CD to the working directory
+    working_dir = kwargs.directory or defaults["directory"]
+    os.chdir(working_dir)
+
+    # Load config file options (setup.cfg)
+    res = config_file()
+
+    #  If outdir was specified in the config file, then it is relative to the config file
+    if "outdir" in res:
+        res["outdir"] = Path(res["outdir"]).absolute()
+
+    # Apply defaults as specified in args.yml
+    for k, v in defaults.items():
+        if k not in res:
+            res[k] = v
+
+
+    # Override config and defaults with cli args
     res.update({k: v for k, v in kwargs.__dict__.items() if v is not None})
+    res["outdir"].mkdir(exist_ok=True)
+
     return res
 
 
 CONFIG = config()
 
 if __name__ == "__main__":
     print(CONFIG)
```

### Comparing `widgetron-0.1.6/src/widgetron/templates/electron/package.json_template` & `widgetron-0.1.7/src/widgetron/templates/electron/package.json_template`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523809523809523%*

 * *Differences: {"'devDependencies'": "{'@cyclonedx/cyclonedx-npm': '^1.9.2'}",*

 * * "'scripts'": "{'lock': 'cyclonedx-npm'}"}*

```diff
@@ -14,18 +14,20 @@
             "target": "dir"
         }
     },
     "dependencies": {
         "electron-store": "^8.1.0"
     },
     "devDependencies": {
+        "@cyclonedx/cyclonedx-npm": "^1.9.2",
         "electron": "^22.3.1",
         "electron-builder": "^23.6.0"
     },
     "main": "main.js",
     "name": "widgetron",
     "scripts": {
         "build": "electron-builder build",
+        "lock": "cyclonedx-npm",
         "start": "electron ."
     },
     "version": "0.1.0"
 }
```

### Comparing `widgetron-0.1.6/src/widgetron/templates/server/widgetron_app/cli.py_template` & `widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/cli.py_template`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     print(url)
     os.environ["widgetron_url"] = url
 
     # open UI
     if SYS == "Darwin":
         UI = ["open", "-W", str(HERE.absolute() / "widgetron.app"), "--env", f"widgetron_url={url}"]
     if SYS == "Linux":
-        UI = [str(next(HERE.rglob("widgetron")).absolute()), "--no-sandbox"]
+        UI = [str(next(HERE.rglob("widgetron")).absolute())]
     if SYS == "Windows":
         UI = str(next(HERE.rglob("widgetron.exe")).absolute())
     
     subprocess.call(UI)
 
     # when UI stops, kill jupyter lab
     def kill(proc_pid):
```

### Comparing `widgetron-0.1.6/src/widgetron/templates/server/widgetron_app/notebooks/debug.ipynb` & `widgetron-0.1.7/src/widgetron/templates/server/widgetron_app/notebooks/debug.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642361111111111%*

 * *Differences: {"'cells'": "{1: {'source': ['!jupyter --config']}, 2: {'source': ['### Jupyter Paths']}, 14: "*

 * *            "{'id': '57a1872e-3ee9-4177-9d22-8a56b3762254'}, insert: [(4, "*

 * *            "OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'e287a7fb-8259-4348-b4f4-38c4db3118fb'), ('metadata', OrderedDict()), ('source', "*

 * *            "['### Jupyter Kernelspecs'])])), (5, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_count', None), ('id', '2adb0a9b-5fa7-453b-9155-4b472cb579be'), "*

 * *     […]*

```diff
@@ -13,23 +13,23 @@
             "execution_count": null,
             "id": "828cf4af-4a6b-4468-9257-c1e201838e86",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "!jupyter --paths"
+                "!jupyter --config"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c3d83d6d-3fa4-47de-ba32-5ab264109c1b",
             "metadata": {},
             "source": [
-                "### Jupyter paths"
+                "### Jupyter Paths"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ca145977-e097-4fbd-8aae-6b37b1727be6",
             "metadata": {
@@ -38,14 +38,34 @@
             "outputs": [],
             "source": [
                 "!jupyter --paths --debug"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "e287a7fb-8259-4348-b4f4-38c4db3118fb",
+            "metadata": {},
+            "source": [
+                "### Jupyter Kernelspecs"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "2adb0a9b-5fa7-453b-9155-4b472cb579be",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "!jupyter kernelspec list"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "d22e74eb-ecd7-4600-beaf-70284a9873fc",
             "metadata": {},
             "source": [
                 "### CONDA config"
             ]
         },
         {
@@ -99,17 +119,35 @@
             "outputs": [],
             "source": [
                 "import sys\n",
                 "sys.executable"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "1696bc6a-edb8-4b70-89cc-bd3b69230658",
+            "metadata": {},
+            "source": [
+                "### Conda Environments"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "d907f43b-2e3e-49ca-a74d-532d6313b780",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "!conda env list"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fcf84a43-94f5-4ac4-8eca-dc8bd1b0e8f2",
+            "id": "57a1872e-3ee9-4177-9d22-8a56b3762254",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `widgetron-0.1.6/src/widgetron.egg-info/SOURCES.txt` & `widgetron-0.1.7/src/widgetron.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE
-README.rst
+README.md
 setup.cfg
 setup.py
 src/widgetron/__init__.py
 src/widgetron/__main__.py
 src/widgetron/args.yml
 src/widgetron/jinja_functions.py
 src/widgetron/parse_args.py
```

