# Comparing `tmp/py-mlm-0.0.4.tar.gz` & `tmp/py-mlm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-mlm-0.0.4.tar", last modified: Sun Mar 26 06:43:52 2023, max compression
+gzip compressed data, was "py-mlm-0.0.5.tar", last modified: Fri Apr 14 00:33:03 2023, max compression
```

## Comparing `py-mlm-0.0.4.tar` & `py-mlm-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-03-26 06:43:52.043350 py-mlm-0.0.4/
--rw-r--r--   0 anon      (1000) wheel      (998)    35049 2022-11-14 05:29:48.000000 py-mlm-0.0.4/LICENSE
--rw-r--r--   0 anon      (1000) wheel      (998)      484 2023-03-26 06:43:52.043350 py-mlm-0.0.4/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      150 2023-03-23 05:11:28.000000 py-mlm-0.0.4/README.md
--rw-r--r--   0 anon      (1000) wheel      (998)      558 2023-03-26 06:43:15.000000 py-mlm-0.0.4/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-03-26 06:43:52.043350 py-mlm-0.0.4/setup.cfg
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-03-26 06:43:52.043350 py-mlm-0.0.4/src/
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-03-26 06:43:52.043350 py-mlm-0.0.4/src/mlm/
--rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 py-mlm-0.0.4/src/mlm/__init__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2356 2023-03-26 05:01:03.000000 py-mlm-0.0.4/src/mlm/__main__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     5287 2023-03-26 05:31:33.000000 py-mlm-0.0.4/src/mlm/build.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2216 2023-03-23 03:17:40.000000 py-mlm-0.0.4/src/mlm/config.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4113 2023-03-23 03:57:31.000000 py-mlm-0.0.4/src/mlm/g_dl.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 py-mlm-0.0.4/src/mlm/initial_setup.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     3526 2023-03-26 06:19:39.000000 py-mlm-0.0.4/src/mlm/media.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     6189 2023-03-26 05:00:23.000000 py-mlm-0.0.4/src/mlm/options.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1648 2023-03-21 22:37:52.000000 py-mlm-0.0.4/src/mlm/prompts.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1968 2023-03-26 06:41:39.000000 py-mlm-0.0.4/src/mlm/search.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4933 2023-03-23 03:56:24.000000 py-mlm-0.0.4/src/mlm/system.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     4224 2023-03-26 06:30:48.000000 py-mlm-0.0.4/src/mlm/utils.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-03-26 06:43:52.043350 py-mlm-0.0.4/src/py_mlm.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)      484 2023-03-26 06:43:52.000000 py-mlm-0.0.4/src/py_mlm.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      462 2023-03-26 06:43:52.000000 py-mlm-0.0.4/src/py_mlm.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-03-26 06:43:52.000000 py-mlm-0.0.4/src/py_mlm.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       42 2023-03-26 06:43:52.000000 py-mlm-0.0.4/src/py_mlm.egg-info/entry_points.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       30 2023-03-26 06:43:52.000000 py-mlm-0.0.4/src/py_mlm.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        4 2023-03-26 06:43:52.000000 py-mlm-0.0.4/src/py_mlm.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:33:03.237342 py-mlm-0.0.5/
+-rw-r--r--   0 anon      (1000) wheel      (998)    35049 2022-11-14 05:29:48.000000 py-mlm-0.0.5/LICENSE
+-rw-r--r--   0 anon      (1000) wheel      (998)      484 2023-04-14 00:33:03.237342 py-mlm-0.0.5/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      150 2023-03-23 05:11:28.000000 py-mlm-0.0.5/README.md
+-rw-r--r--   0 anon      (1000) wheel      (998)      558 2023-04-14 00:32:04.000000 py-mlm-0.0.5/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-14 00:33:03.237342 py-mlm-0.0.5/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:33:03.230675 py-mlm-0.0.5/src/
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:33:03.234009 py-mlm-0.0.5/src/mlm/
+-rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-22 02:48:23.000000 py-mlm-0.0.5/src/mlm/__init__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2335 2023-04-10 21:07:50.000000 py-mlm-0.0.5/src/mlm/__main__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     5287 2023-03-26 05:31:33.000000 py-mlm-0.0.5/src/mlm/build.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2216 2023-03-23 03:17:40.000000 py-mlm-0.0.5/src/mlm/config.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     4113 2023-03-23 03:57:31.000000 py-mlm-0.0.5/src/mlm/g_dl.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)      166 2022-09-22 02:48:23.000000 py-mlm-0.0.5/src/mlm/initial_setup.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     3526 2023-03-26 06:19:39.000000 py-mlm-0.0.5/src/mlm/media.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     6582 2023-04-10 20:40:11.000000 py-mlm-0.0.5/src/mlm/options.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1651 2023-04-14 00:27:42.000000 py-mlm-0.0.5/src/mlm/prompts.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1968 2023-03-26 06:41:39.000000 py-mlm-0.0.5/src/mlm/search.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     5963 2023-04-10 21:06:52.000000 py-mlm-0.0.5/src/mlm/system.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     4224 2023-03-26 06:30:48.000000 py-mlm-0.0.5/src/mlm/utils.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:33:03.237342 py-mlm-0.0.5/src/py_mlm.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)      484 2023-04-14 00:33:03.000000 py-mlm-0.0.5/src/py_mlm.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      462 2023-04-14 00:33:03.000000 py-mlm-0.0.5/src/py_mlm.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-14 00:33:03.000000 py-mlm-0.0.5/src/py_mlm.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       42 2023-04-14 00:33:03.000000 py-mlm-0.0.5/src/py_mlm.egg-info/entry_points.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       30 2023-04-14 00:33:03.000000 py-mlm-0.0.5/src/py_mlm.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        4 2023-04-14 00:33:03.000000 py-mlm-0.0.5/src/py_mlm.egg-info/top_level.txt
```

### Comparing `py-mlm-0.0.4/LICENSE` & `py-mlm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.4/pyproject.toml` & `py-mlm-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-mlm"
-version = "0.0.4"
+version = "0.0.5"
 description = "mlm - Manga Library Manager. Local, and simple method for reading and tracking manga."
 readme = "README.md"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 keywords = [ "zathura" ]
 dependencies = [
     "python-magic",
     "loadconf",
```

### Comparing `py-mlm-0.0.4/src/mlm/__main__.py` & `py-mlm-0.0.5/src/mlm/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,18 +41,18 @@
         return read_manga(user, latest=args.latest, new=args.new)
     elif args.url is not None and args.dir is not None:
         return add_url(url=args.url, dir=args.dir, user=user)
     elif args.add is not None:
         return bulk_new(user=user, args=args)
     elif args.download_new:
         return bulk_latest(user=user, args=args)
-    elif args.zip is not None:
-        cprint("green", f"(Re)zipping '{args.zip}'")
+    elif args.zip:
         return re_zip(user=user, args=args)
     else:
+        cprint("green", "Updating library")
         return update_library(user, args)
 
 
 def main():
     """
     Command line application to view and track media
     """
```

### Comparing `py-mlm-0.0.4/src/mlm/build.py` & `py-mlm-0.0.5/src/mlm/build.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.4/src/mlm/config.py` & `py-mlm-0.0.5/src/mlm/config.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.4/src/mlm/g_dl.py` & `py-mlm-0.0.5/src/mlm/g_dl.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.4/src/mlm/media.py` & `py-mlm-0.0.5/src/mlm/media.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.4/src/mlm/options.py` & `py-mlm-0.0.5/src/mlm/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,16 +56,16 @@
         help="""List your latest tracked manga to resume reading.""",
     )
     group.add_argument(
         "-o",
         "--open",
         metavar="FILE",
         help="""
-        This is a sort of wrapper for mpv which will also track the anime when
-        closed.
+        This is a sort of wrapper for zathura which will also track the anime
+        when closed.
         """,
     )
     group.add_argument(
         "-r",
         "--read",
         action="store_true",
         help="""
@@ -120,18 +120,19 @@
         help="""
         URL to associate with DIR.
         """,
     )
     group.add_argument(
         "-z",
         "--zip",
-        metavar="PATH",
-        action="store",
+        action="store_true",
         help="""
-        (Re)zip the title in question. This will create a cbz file for each dir matching the following regex: ^.*[0-9]\\.[0-9]$
+        (Re)zip the PATH given by --path or the $PWD if not supplied. This will
+        create a cbz file for each dir matching the following regex:
+        ^.*[0-9]\\.[0-9]$
         """,
     )
     parser.add_argument(
         "-c",
         "--clean",
         action="store_true",
         help="""
@@ -140,15 +141,15 @@
     )
     parser.add_argument(
         "-d",
         "--dir",
         metavar="DIR",
         action="store",
         help="""
-        DIR to use for other options like --url...
+        DIR to use for other options like --url, and --move
         """,
     )
     parser.add_argument(
         "-i",
         "--interactive",
         action="store_true",
         help="""
@@ -185,18 +186,34 @@
         "--new",
         action="store_true",
         help="""
         Use with --read to list manga in order of update order.
         """,
     )
     parser.add_argument(
+        "--move",
+        action="store_true",
+        help="""
+        Used with --zip. If DIR is given the zipped files will be placed in
+        """,
+    )
+    parser.add_argument(
         "-p",
         "--page",
         action="store",
         type=int,
         default=-1,
         help="""
         Used for better accuracy when tracking a file.
         """,
     )
+    parser.add_argument(
+        "-P",
+        "--path",
+        metavar="PATH",
+        action="store",
+        help="""
+        The PATH to --zip.
+        """,
+    )
     args = parser.parse_args()
     return args
```

### Comparing `py-mlm-0.0.4/src/mlm/prompts.py` & `py-mlm-0.0.5/src/mlm/prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,8 +61,8 @@
 
     choice = p.ask(
         options=options,
         prompt=prompt,
         additional_args=cmd_args,
     )
 
-    return choice
+    return choice[0]
```

### Comparing `py-mlm-0.0.4/src/mlm/search.py` & `py-mlm-0.0.5/src/mlm/search.py`

 * *Files identical despite different names*

### Comparing `py-mlm-0.0.4/src/mlm/system.py` & `py-mlm-0.0.5/src/mlm/system.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,16 +105,33 @@
 def make_cbz(path: pathlib.Path):
     files = get_files(path)
     for file in files:
         name = file.name.replace("zip", "cbz")
         file.rename(file.parent.as_posix() + "/" + name)
 
 
+def move_cbz(dest, path: pathlib.Path):
+    target_dir = pathlib.Path(dest, path.name)
+    for file in os.listdir(path):
+        if not file.endswith("cbz"):
+            continue
+        dest_file = pathlib.Path(target_dir / file)
+        if dest_file.exists() and dest_file.is_file():
+            dest_file.unlink()
+        elif dest_file.is_dir():
+            raise OSError(f"Destination is a directory {dest_file}")
+        shutil.move(file, target_dir)
+
+
 def move_to_raw(base_dir, path: pathlib.Path):
-    target_dir = pathlib.Path(base_dir, "raw_manga", path.name)
+    move_to_x(base_dir, "raw_manga", path)
+
+
+def move_to_x(base_dir, x: str, path: pathlib.Path):
+    target_dir = pathlib.Path(base_dir, x, path.name)
     dirs = get_dirs(path)
     for dir in dirs:
         target_path = target_dir / dir.name
         shutil.move(dir, target_path)
 
 
 def open_process(opener, out=subprocess.DEVNULL, err=subprocess.STDOUT):
@@ -138,16 +155,31 @@
     """
     proc = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     stdout, stderr = proc.communicate()
     return {"stdout": stdout.decode("utf-8"), "stderr": stderr.decode("utf-8")}
 
 
 def re_zip(user, args):
-    path = pathlib.Path(args.zip)
+    if args.path is None:
+        path = pathlib.Path().absolute()
+    else:
+        path = pathlib.Path(args.path)
+    cprint("green", f"(Re)zipping '{path}'")
     zip_dirs_in_path(path)
+    make_cbz(path)
+    if args.dir is None:
+        base = user.settings["base_dir"]
+    else:
+        base = args.dir
+    if args.move:
+        move_cbz(base, path)
+    # if args.move is not None and args.move == "base_dir":
+    #     move_to_x(user.settings["base_dir"], "", path)
+    # elif args.move is not None:
+    #     move_cbz_to(args.move, path)
 
 
 def run_cmd(cmd):
     subprocess.run(cmd)
 
 
 def zip_dirs_in_path(path: pathlib.Path):
```

### Comparing `py-mlm-0.0.4/src/mlm/utils.py` & `py-mlm-0.0.5/src/mlm/utils.py`

 * *Files identical despite different names*

