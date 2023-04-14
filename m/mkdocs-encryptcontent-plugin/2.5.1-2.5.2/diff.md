# Comparing `tmp/mkdocs-encryptcontent-plugin-2.5.1.tar.gz` & `tmp/mkdocs-encryptcontent-plugin-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-encryptcontent-plugin-2.5.1.tar", last modified: Thu Apr 13 19:40:36 2023, max compression
+gzip compressed data, was "mkdocs-encryptcontent-plugin-2.5.2.tar", last modified: Fri Apr 14 08:38:14 2023, max compression
```

## Comparing `mkdocs-encryptcontent-plugin-2.5.1.tar` & `mkdocs-encryptcontent-plugin-2.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 19:40:36.683699 mkdocs-encryptcontent-plugin-2.5.1/
--rw-rw-rw-   0        0        0     1070 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.1/LICENSE.md
--rw-rw-rw-   0        0        0    33922 2023-04-13 19:40:36.682707 mkdocs-encryptcontent-plugin-2.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    27028 2023-04-13 19:36:57.000000 mkdocs-encryptcontent-plugin-2.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 19:40:36.648699 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/
--rw-rw-rw-   0        0        0        0 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:40:36.640704 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/
-drwxrwxrwx   0        0        0        0 2023-04-13 19:40:36.640704 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/
-drwxrwxrwx   0        0        0        0 2023-04-13 19:40:36.652701 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/
--rw-rw-rw-   0        0        0    99860 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/lunr.js
--rw-rw-rw-   0        0        0     3670 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/main.js
--rw-rw-rw-   0        0        0     4195 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/worker.js
--rw-rw-rw-   0        0        0    14540 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/decrypt-contents.tpl.js
--rw-rw-rw-   0        0        0     1206 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/decrypt-form.tpl.html
--rw-rw-rw-   0        0        0    36211 2023-04-13 19:36:16.000000 mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/plugin.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:40:36.680698 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/
--rw-rw-rw-   0        0        0    33922 2023-04-13 19:40:36.000000 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-04-13 19:40:36.000000 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 19:40:36.000000 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-04-13 19:40:36.000000 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 19:40:36.000000 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-13 19:40:36.000000 mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 19:40:36.683699 mkdocs-encryptcontent-plugin-2.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1780 2023-04-13 19:37:10.000000 mkdocs-encryptcontent-plugin-2.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:38:14.409063 mkdocs-encryptcontent-plugin-2.5.2/
+-rw-rw-rw-   0        0        0     1070 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.2/LICENSE.md
+-rw-rw-rw-   0        0        0    33922 2023-04-14 08:38:14.402063 mkdocs-encryptcontent-plugin-2.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    27028 2023-04-14 08:37:56.000000 mkdocs-encryptcontent-plugin-2.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 08:38:14.379067 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/
+-rw-rw-rw-   0        0        0        0 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:38:14.374068 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/
+drwxrwxrwx   0        0        0        0 2023-04-14 08:38:14.374068 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/
+drwxrwxrwx   0        0        0        0 2023-04-14 08:38:14.381068 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/
+-rw-rw-rw-   0        0        0    99860 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/lunr.js
+-rw-rw-rw-   0        0        0     3670 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/main.js
+-rw-rw-rw-   0        0        0     4195 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/worker.js
+-rw-rw-rw-   0        0        0    14540 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/decrypt-contents.tpl.js
+-rw-rw-rw-   0        0        0     1206 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/decrypt-form.tpl.html
+-rw-rw-rw-   0        0        0    36217 2023-04-14 08:37:01.000000 mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/plugin.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:38:14.400065 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/
+-rw-rw-rw-   0        0        0    33922 2023-04-14 08:38:14.000000 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-04-14 08:38:14.000000 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 08:38:14.000000 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-04-14 08:38:14.000000 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 08:38:14.000000 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 08:38:14.000000 mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 08:38:14.410066 mkdocs-encryptcontent-plugin-2.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1780 2023-04-14 08:37:53.000000 mkdocs-encryptcontent-plugin-2.5.2/setup.py
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.1/LICENSE.md` & `mkdocs-encryptcontent-plugin-2.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.1/PKG-INFO` & `mkdocs-encryptcontent-plugin-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-encryptcontent-plugin
-Version: 2.5.1
+Version: 2.5.2
 Summary: A MkDocs plugin that encrypt/decrypt markdown content with AES
 Home-page: https://github.com/unverbuggt/mkdocs-encryptcontent-plugin
 Author: unverbuggt
 Author-email: unverbuggt@xn--rthlein-n2a.de
 License: MIT
 Description: # mkdocs-encryptcontent-plugin
         
@@ -73,15 +73,15 @@
         ```
         
         Install the package from source with pip:
         
         ```bash
         cd mkdocs-encryptcontent-plugin/
         python setup.py sdist bdist_wheel
-        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.1-py3-none-any.whl
+        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.2-py3-none-any.whl
         ```
         
         Enable the plugin in your `mkdocs.yml`:
         
         ```yaml
         plugins:
             - search: {}
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.1/README.md` & `mkdocs-encryptcontent-plugin-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 ```
 
 Install the package from source with pip:
 
 ```bash
 cd mkdocs-encryptcontent-plugin/
 python setup.py sdist bdist_wheel
-pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.1-py3-none-any.whl
+pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.2-py3-none-any.whl
 ```
 
 Enable the plugin in your `mkdocs.yml`:
 
 ```yaml
 plugins:
     - search: {}
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/lunr.js` & `mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/lunr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/main.js` & `mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/main.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/contrib/templates/search/worker.js` & `mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/contrib/templates/search/worker.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/decrypt-contents.tpl.js` & `mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/decrypt-contents.tpl.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/decrypt-form.tpl.html` & `mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/decrypt-form.tpl.html`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.1/encryptcontent/plugin.py` & `mkdocs-encryptcontent-plugin-2.5.2/encryptcontent/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
         # optionally selfhost cryptojs
         js_libraries = []
         for jsurl in JS_LIBRARIES:
             if self.config["selfhost"]:
                 js_libraries.append(base_path + 'assets/javascripts/cryptojs/' + jsurl[0].rsplit('/',1)[1])
             else:
-                js_libraries = jsurl[0]
+                js_libraries.append(jsurl[0])
 
         obfuscate = encryptcontent.get('obfuscate')
         if obfuscate:
             obfuscate_password = encryptcontent['password']
         else:
             obfuscate_password = None
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO` & `mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-encryptcontent-plugin
-Version: 2.5.1
+Version: 2.5.2
 Summary: A MkDocs plugin that encrypt/decrypt markdown content with AES
 Home-page: https://github.com/unverbuggt/mkdocs-encryptcontent-plugin
 Author: unverbuggt
 Author-email: unverbuggt@xn--rthlein-n2a.de
 License: MIT
 Description: # mkdocs-encryptcontent-plugin
         
@@ -73,15 +73,15 @@
         ```
         
         Install the package from source with pip:
         
         ```bash
         cd mkdocs-encryptcontent-plugin/
         python setup.py sdist bdist_wheel
-        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.1-py3-none-any.whl
+        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.2-py3-none-any.whl
         ```
         
         Enable the plugin in your `mkdocs.yml`:
         
         ```yaml
         plugins:
             - search: {}
```

### Comparing `mkdocs-encryptcontent-plugin-2.5.1/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt` & `mkdocs-encryptcontent-plugin-2.5.2/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.5.1/setup.py` & `mkdocs-encryptcontent-plugin-2.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     with open(file_path) as file:
         content = file.read()
     return content if content else 'no content read'
 
 
 setup(
     name='mkdocs-encryptcontent-plugin',
-    version='2.5.1',
+    version='2.5.2',
     author='unverbuggt',
     author_email='unverbuggt@xn--rthlein-n2a.de',
     description='A MkDocs plugin that encrypt/decrypt markdown content with AES',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown encrypt decrypt content',
     url='https://github.com/unverbuggt/mkdocs-encryptcontent-plugin',
```

