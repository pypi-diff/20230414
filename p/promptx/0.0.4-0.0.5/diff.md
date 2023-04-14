# Comparing `tmp/promptx-0.0.4.tar.gz` & `tmp/promptx-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptx-0.0.4.tar", last modified: Thu Apr 13 19:44:31 2023, max compression
+gzip compressed data, was "promptx-0.0.5.tar", last modified: Fri Apr 14 00:37:15 2023, max compression
```

## Comparing `promptx-0.0.4.tar` & `promptx-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-13 19:44:31.172291 promptx-0.0.4/
--rw-r--r--   0 anon      (1000) wheel      (998)    34880 2022-09-15 20:58:55.000000 promptx-0.0.4/LICENSE.md
--rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-13 19:44:31.172291 promptx-0.0.4/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)     2526 2022-09-21 20:19:44.000000 promptx-0.0.4/README.md
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-13 19:44:31.172291 promptx-0.0.4/promptx/
--rw-r--r--   0 anon      (1000) wheel      (998)      145 2022-09-15 21:02:32.000000 promptx-0.0.4/promptx/__init__.py
--rw-r--r--   0 anon      (1000) wheel      (998)     5572 2023-04-13 19:42:05.000000 promptx-0.0.4/promptx/promptx.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-13 19:44:31.172291 promptx-0.0.4/promptx.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-13 19:44:31.000000 promptx-0.0.4/promptx.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      198 2023-04-13 19:44:31.000000 promptx-0.0.4/promptx.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-13 19:44:31.000000 promptx-0.0.4/promptx.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        8 2023-04-13 19:44:31.000000 promptx-0.0.4/promptx.egg-info/top_level.txt
--rw-r--r--   0 anon      (1000) wheel      (998)      463 2023-04-13 19:42:26.000000 promptx-0.0.4/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-13 19:44:31.172291 promptx-0.0.4/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:37:15.776136 promptx-0.0.5/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34880 2022-09-15 20:58:55.000000 promptx-0.0.5/LICENSE.md
+-rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-14 00:37:15.776136 promptx-0.0.5/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)     2526 2022-09-21 20:19:44.000000 promptx-0.0.5/README.md
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:37:15.772803 promptx-0.0.5/promptx/
+-rw-r--r--   0 anon      (1000) wheel      (998)      145 2022-09-15 21:02:32.000000 promptx-0.0.5/promptx/__init__.py
+-rw-r--r--   0 anon      (1000) wheel      (998)     5056 2023-04-14 00:35:36.000000 promptx-0.0.5/promptx/promptx.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-04-14 00:37:15.776136 promptx-0.0.5/promptx.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)     2839 2023-04-14 00:37:15.000000 promptx-0.0.5/promptx.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      198 2023-04-14 00:37:15.000000 promptx-0.0.5/promptx.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-04-14 00:37:15.000000 promptx-0.0.5/promptx.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        8 2023-04-14 00:37:15.000000 promptx-0.0.5/promptx.egg-info/top_level.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)      463 2023-04-14 00:35:50.000000 promptx-0.0.5/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-04-14 00:37:15.776136 promptx-0.0.5/setup.cfg
```

### Comparing `promptx-0.0.4/LICENSE.md` & `promptx-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `promptx-0.0.4/PKG-INFO` & `promptx-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptx
-Version: 0.0.4
+Version: 0.0.5
 Summary: Flexible prompt wrapper for dmenu, fzf, and rofi.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/promptx
 Keywords: dmenu,fzf,rofi
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `promptx-0.0.4/README.md` & `promptx-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `promptx-0.0.4/promptx/promptx.py` & `promptx-0.0.5/promptx/promptx.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,24 +92,19 @@
         self.temp_args = []
 
     def ask(
         self,
         options: List,
         prompt: str | None = None,
         additional_args: str | None = None,
-        select: str = "first",
         deliminator: str = "\n",
-    ):
+    ) -> List[str]:
         """
         Ask the user to make a selection from the given options
         """
-        # If check that select is properly set
-        if select not in ["first", "last", "all"]:
-            raise PromptXSelectError(select)
-        # Initialize the cmd value
         cmd = []
         cmd.extend(self.base_cmd)
         cmd.extend(self.temp_args)
         # fzf uses stderr to show prompt so we need to check for that
         stderr_file = None if self.prompt_cmd == "fzf" else subprocess.PIPE
         if additional_args is not None:
             cmd.extend(shlex.split(additional_args))
@@ -136,28 +131,19 @@
         # Create one long string similar to choice=$(printf '%s\n' "$@" | dmenu) in bash
         opts_str = deliminator.join(map(str, options))
         # Open stdin and populate choices
         outs, errs = proc.communicate(input=opts_str)
         if proc.wait() != 0:
             # If no err return None as user hit escape
             if errs == "":
-                return None
+                return []
             # Otherwise some error occured
             raise PromptXError(cmd, errs)
 
-        selection = outs.rstrip().splitlines()
-        # Return the requested selection
-        if select == "first" and len(selection) > 0:
-            return selection[0]
-        elif select == "last" and len(selection) > 0:
-            return selection[-1]
-        elif len(selection) > 0:
-            return selection
-        else:
-            return None
+        return outs.rstrip().splitlines()
 
     def add_args(
         self,
         additional_args: List,
         default_args: bool = False,
     ):
         """
```

### Comparing `promptx-0.0.4/promptx.egg-info/PKG-INFO` & `promptx-0.0.5/promptx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptx
-Version: 0.0.4
+Version: 0.0.5
 Summary: Flexible prompt wrapper for dmenu, fzf, and rofi.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/promptx
 Keywords: dmenu,fzf,rofi
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

