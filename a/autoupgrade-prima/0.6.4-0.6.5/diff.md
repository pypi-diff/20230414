# Comparing `tmp/autoupgrade_prima-0.6.4-py2.py3-none-any.whl.zip` & `tmp/autoupgrade_prima-0.6.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5482 bytes, number of entries: 7
--rw-r-----  2.0 unx     3403 b- defN 23-Mar-22 07:45 autoupgrade/__init__.py
--rw-r-----  2.0 unx     1190 b- defN 23-Mar-22 07:49 autoupgrade_prima-0.6.4.dist-info/LICENSE.md
--rw-r-----  2.0 unx     5815 b- defN 23-Mar-22 07:49 autoupgrade_prima-0.6.4.dist-info/METADATA
--rw-r-----  2.0 unx      110 b- defN 23-Mar-22 07:49 autoupgrade_prima-0.6.4.dist-info/WHEEL
--rw-r-----  2.0 unx       12 b- defN 23-Mar-22 07:49 autoupgrade_prima-0.6.4.dist-info/top_level.txt
--rw-r-----  2.0 unx        1 b- defN 23-Mar-22 07:49 autoupgrade_prima-0.6.4.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      616 b- defN 23-Mar-22 07:49 autoupgrade_prima-0.6.4.dist-info/RECORD
-7 files, 11147 bytes uncompressed, 4374 bytes compressed:  60.8%
+Zip file size: 5427 bytes, number of entries: 7
+-rw-r-----  2.0 unx     3103 b- defN 23-Apr-14 12:54 autoupgrade/__init__.py
+-rw-r-----  2.0 unx     1190 b- defN 23-Apr-14 12:55 autoupgrade_prima-0.6.5.dist-info/LICENSE.md
+-rw-r-----  2.0 unx     5815 b- defN 23-Apr-14 12:55 autoupgrade_prima-0.6.5.dist-info/METADATA
+-rw-r-----  2.0 unx      110 b- defN 23-Apr-14 12:55 autoupgrade_prima-0.6.5.dist-info/WHEEL
+-rw-r-----  2.0 unx       12 b- defN 23-Apr-14 12:55 autoupgrade_prima-0.6.5.dist-info/top_level.txt
+-rw-r-----  2.0 unx        1 b- defN 23-Mar-22 07:49 autoupgrade_prima-0.6.5.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      616 b- defN 23-Apr-14 12:55 autoupgrade_prima-0.6.5.dist-info/RECORD
+7 files, 10847 bytes uncompressed, 4319 bytes compressed:  60.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: autoupgrade/__init__.py
 Comment: 
 
-Filename: autoupgrade_prima-0.6.4.dist-info/LICENSE.md
+Filename: autoupgrade_prima-0.6.5.dist-info/LICENSE.md
 Comment: 
 
-Filename: autoupgrade_prima-0.6.4.dist-info/METADATA
+Filename: autoupgrade_prima-0.6.5.dist-info/METADATA
 Comment: 
 
-Filename: autoupgrade_prima-0.6.4.dist-info/WHEEL
+Filename: autoupgrade_prima-0.6.5.dist-info/WHEEL
 Comment: 
 
-Filename: autoupgrade_prima-0.6.4.dist-info/top_level.txt
+Filename: autoupgrade_prima-0.6.5.dist-info/top_level.txt
 Comment: 
 
-Filename: autoupgrade_prima-0.6.4.dist-info/zip-safe
+Filename: autoupgrade_prima-0.6.5.dist-info/zip-safe
 Comment: 
 
-Filename: autoupgrade_prima-0.6.4.dist-info/RECORD
+Filename: autoupgrade_prima-0.6.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## autoupgrade/__init__.py

```diff
@@ -56,24 +56,19 @@
         if self._is_user_installed():
             pip_args.append("--user")
 
         proxy = os.environ.get("http_proxy")
         if proxy:
             pip_args.extend(["--proxy", proxy])
 
-        try:
-            subprocess.run(pip_args, check=True)
-            version_after = self._get_installed_version()
-
-            if semver.compare(version_after, self.version_before) == 1:
-                restart = True
+        subprocess.run(pip_args, check=True)
+        version_after = self._get_installed_version()
 
-        except (CalledProcessError) as e:
-            print(f"Errore eseguendo il comando: {e}")
-            sys.exit(-1)
+        if semver.compare(version_after, self.version_before) == 1:
+            restart = True
 
         if restart:
             self.restart()
 
     def restart(self):
         """
         Restart application with same args as it was started.
@@ -93,21 +88,17 @@
             return installation_path.startswith(user_site_directory)
         except AttributeError:
             # Some versions of virtualenv ship with their own version of the
             # site module without the getusersitepacakges function.
             return False
 
     def _get_installed_version(self):
-        try:
-            output = subprocess.run(
-                [self._find_pip(), "show", self.pkg], check=True, stdout=subprocess.PIPE
-            ).stdout.decode("utf-8")
-
-            return re.search(self.regex, output).group(1)
-        except (CalledProcessError) as e:
-            print(f"Errore eseguendo il comando: {e}")
-            sys.exit(-1)
+        output = subprocess.run(
+            [self._find_pip(), "show", self.pkg], check=True, stdout=subprocess.PIPE
+        ).stdout.decode("utf-8")
+
+        return re.search(self.regex, output).group(1)
 
     def _find_pip(self):
-        if sys.base_prefix != sys.prefix: # running from venv
-            return sys.prefix+"/bin/pip3"
+        if sys.base_prefix != sys.prefix:  # running from venv
+            return sys.prefix + "/bin/pip3"
         return "pip3"
```

## Comparing `autoupgrade_prima-0.6.4.dist-info/LICENSE.md` & `autoupgrade_prima-0.6.5.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `autoupgrade_prima-0.6.4.dist-info/METADATA` & `autoupgrade_prima-0.6.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoupgrade-prima
-Version: 0.6.4
+Version: 0.6.5
 Summary: Automatic upgrade of PyPI packages
 Home-page: https://github.com/primait/autoupgrade
 Download-URL: https://github.com/primait/autoupgrade/releases
 Author: Walter Purcaro
 Author-email: vuolter@gmail.com
 License: MIT License
 Keywords: autoupgrade,pip-upgrade,pip
```

