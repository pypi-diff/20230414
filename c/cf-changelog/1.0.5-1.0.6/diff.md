# Comparing `tmp/cf_changelog-1.0.5.tar.gz` & `tmp/cf_changelog-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\DELL\Documents\cf_changelog\dist\.tmp-2csto_un\cf_changelog-1.0.5.tar", last modified: Thu Apr 13 16:08:24 2023, max compression
+gzip compressed data, was "C:\Users\psalek\Documents\cf_changelog\dist\.tmp-x19o_2dp\cf_changelog-1.0.6.tar", last modified: Fri Apr 14 13:35:11 2023, max compression
```

## Comparing `cf_changelog-1.0.5.tar` & `cf_changelog-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 16:08:24.000000 cf_changelog-1.0.5/
--rw-rw-rw-   0        0        0     1070 2023-04-11 19:59:57.000000 cf_changelog-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     2230 2023-04-13 16:08:24.000000 cf_changelog-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1885 2023-04-13 16:07:24.000000 cf_changelog-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 16:08:24.000000 cf_changelog-1.0.5/cf_changelog/
--rw-rw-rw-   0        0        0       31 2023-04-11 21:02:35.000000 cf_changelog-1.0.5/cf_changelog/__init__.py
--rw-rw-rw-   0        0        0     6944 2023-04-13 15:45:53.000000 cf_changelog-1.0.5/cf_changelog/cf_changelog.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:08:24.000000 cf_changelog-1.0.5/cf_changelog.egg-info/
--rw-rw-rw-   0        0        0     2230 2023-04-13 16:08:24.000000 cf_changelog-1.0.5/cf_changelog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-13 16:08:24.000000 cf_changelog-1.0.5/cf_changelog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 16:08:24.000000 cf_changelog-1.0.5/cf_changelog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-13 16:08:24.000000 cf_changelog-1.0.5/cf_changelog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-13 16:08:24.000000 cf_changelog-1.0.5/cf_changelog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 16:08:24.000000 cf_changelog-1.0.5/cf_changelog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 16:08:24.000000 cf_changelog-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      832 2023-04-13 16:05:15.000000 cf_changelog-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:35:11.000000 cf_changelog-1.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-04-14 13:32:58.000000 cf_changelog-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2215 2023-04-14 13:35:11.000000 cf_changelog-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1920 2023-04-14 13:32:58.000000 cf_changelog-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 13:35:11.000000 cf_changelog-1.0.6/cf_changelog/
+-rw-rw-rw-   0        0        0       32 2023-04-14 13:32:58.000000 cf_changelog-1.0.6/cf_changelog/__init__.py
+-rw-rw-rw-   0        0        0     6962 2023-04-14 13:33:15.000000 cf_changelog-1.0.6/cf_changelog/cf_changelog.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:35:11.000000 cf_changelog-1.0.6/cf_changelog.egg-info/
+-rw-rw-rw-   0        0        0     2215 2023-04-14 13:35:11.000000 cf_changelog-1.0.6/cf_changelog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-14 13:35:11.000000 cf_changelog-1.0.6/cf_changelog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:35:11.000000 cf_changelog-1.0.6/cf_changelog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-14 13:35:11.000000 cf_changelog-1.0.6/cf_changelog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-14 13:35:11.000000 cf_changelog-1.0.6/cf_changelog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 13:35:11.000000 cf_changelog-1.0.6/cf_changelog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:35:11.000000 cf_changelog-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      832 2023-04-14 13:33:51.000000 cf_changelog-1.0.6/setup.py
```

### Comparing `cf_changelog-1.0.5/LICENSE` & `cf_changelog-1.0.6/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Paweł Sałek
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Paweł Sałek
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `cf_changelog-1.0.5/PKG-INFO` & `cf_changelog-1.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: cf_changelog
-Version: 1.0.5
-Summary: Conflict-Free Changelog manager
-Home-page: https://gitlab.com/salekpawel/cf_changelog
-Author: Paweł Sałek
-Author-email: salekpawel@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cf_changelog - Conflict-Free Changelog manager
 
 Simple tool to support changelog modifications on different git branches without conflicts on merging.
 Written in python, installable with pip.
 
 ## Usage
 1. Install it from pip:
@@ -20,26 +9,22 @@
 pip install cf_changelog
 ```
 2. Create some changelog on different branches entries using:
 ```bash
 cf_changelog add
 ```
 It is required to run this from root of your repository.
-This will invoke standard text editor (or notepad/vim if standard editor is not configured), where you can fill a template with new features, bug fixes etc. Example:
-```yaml
-New:
-    - One new cool feature
-    - Another cool feature
-Bugfix:
-    - Fixed bug of previous feature
-    - Fixed another bug
-```
+This will invoke standard text editor (or notepad/vim if standard editor is not configured), where you can fill a template with new features, bug fixes etc. 
+
+Windows example:
+
+![Windows_example of editor with changelog entry](img/windows_template_screenshot.png)
 
 This is simple yaml format. You can use as many types of entries as you wish (New, Bugfix, Changed, Fixed, etc.). Each type should contain a flat list.
-The most important thing is that you don't have to remember anything, just fill in a template.
+The most important thing is that you don't have to remember anything specific related to this tool, just fill in a template.
 
 3. Commit newly created files.
 4. Repeat 2 and 3 on different branches as many times as you need.
 5. Merge all branches.
 6. On merged branch run:
 
 ```bash
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cf_changelog-1.0.5/cf_changelog/cf_changelog.py` & `cf_changelog-1.0.6/cf_changelog/cf_changelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     filename = os.path.join(args.source_directory, getpass.getuser() + '_' + datetime.now(tz=None).strftime("%y-%m-%d_%H-%M-%S") + '.yaml')
     print("Creating source file", filename)
     yaml_content = yaml.load(edited_message, Loader=yaml.Loader)
     try:
         config_schema.validate(yaml_content)
     except SchemaError as se:
         raise se
-    with open(filename, mode='w+') as f:
+    with open(filename, mode='w+', encoding='utf-8') as f:
         f.write(edited_message)
     g = git.cmd.Git(args.repository_root)
     g.add(args.source_directory)
     g.add(filename)
     
 def handle_release(args):
     source_files = [f for f in os.listdir(args.source_directory) if os.path.isfile(os.path.join(args.source_directory, f))]
```

### Comparing `cf_changelog-1.0.5/cf_changelog.egg-info/PKG-INFO` & `cf_changelog-1.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cf-changelog
-Version: 1.0.5
+Name: cf_changelog
+Version: 1.0.6
 Summary: Conflict-Free Changelog manager
 Home-page: https://gitlab.com/salekpawel/cf_changelog
 Author: Paweł Sałek
 Author-email: salekpawel@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -20,26 +20,22 @@
 pip install cf_changelog
 ```
 2. Create some changelog on different branches entries using:
 ```bash
 cf_changelog add
 ```
 It is required to run this from root of your repository.
-This will invoke standard text editor (or notepad/vim if standard editor is not configured), where you can fill a template with new features, bug fixes etc. Example:
-```yaml
-New:
-    - One new cool feature
-    - Another cool feature
-Bugfix:
-    - Fixed bug of previous feature
-    - Fixed another bug
-```
+This will invoke standard text editor (or notepad/vim if standard editor is not configured), where you can fill a template with new features, bug fixes etc. 
+
+Windows example:
+
+![Windows_example of editor with changelog entry](img/windows_template_screenshot.png)
 
 This is simple yaml format. You can use as many types of entries as you wish (New, Bugfix, Changed, Fixed, etc.). Each type should contain a flat list.
-The most important thing is that you don't have to remember anything, just fill in a template.
+The most important thing is that you don't have to remember anything specific related to this tool, just fill in a template.
 
 3. Commit newly created files.
 4. Repeat 2 and 3 on different branches as many times as you need.
 5. Merge all branches.
 6. On merged branch run:
 
 ```bash
```

### Comparing `cf_changelog-1.0.5/setup.py` & `cf_changelog-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='cf_changelog',
       long_description=long_description,
       long_description_content_type='text/markdown',
-      version='1.0.5',
+      version='1.0.6',
       description='Conflict-Free Changelog manager',
       author='Paweł Sałek',
       author_email='salekpawel@gmail.com',
       url='https://gitlab.com/salekpawel/cf_changelog',
       packages=['cf_changelog', ],
       license="MIT",
       install_requires=[
```

