# Comparing `tmp/mo-json-config-3.7.19316.tar.gz` & `tmp/mo-json-config-3.77.20190.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mo-json-config-3.7.19316.tar", last modified: Tue Nov 12 22:46:20 2019, max compression
+gzip compressed data, was "dist\mo-json-config-3.77.20190.tar", last modified: Wed Jul  8 11:17:06 2020, max compression
```

## Comparing `mo-json-config-3.7.19316.tar` & `mo-json-config-3.77.20190.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2019-11-12 22:46:20.000000 mo-json-config-3.7.19316/
-drwxrwxrwx   0        0        0        0 2019-11-12 22:46:20.000000 mo-json-config-3.7.19316/mo_json_config/
--rw-rw-rw-   0        0        0      756 2019-11-12 22:11:16.000000 mo-json-config-3.7.19316/mo_json_config/convert.py
--rw-rw-rw-   0        0        0     8059 2019-11-12 22:11:16.000000 mo-json-config-3.7.19316/mo_json_config/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-12 22:46:20.000000 mo-json-config-3.7.19316/mo_json_config.egg-info/
--rw-rw-rw-   0        0        0        1 2019-11-12 22:46:20.000000 mo-json-config-3.7.19316/mo_json_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    12165 2019-11-12 22:46:20.000000 mo-json-config-3.7.19316/mo_json_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      107 2019-11-12 22:46:20.000000 mo-json-config-3.7.19316/mo_json_config.egg-info/requires.txt
--rw-rw-rw-   0        0        0      260 2019-11-12 22:46:20.000000 mo-json-config-3.7.19316/mo_json_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       15 2019-11-12 22:46:20.000000 mo-json-config-3.7.19316/mo_json_config.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12165 2019-11-12 22:46:20.000000 mo-json-config-3.7.19316/PKG-INFO
--rw-rw-rw-   0        0        0     8601 2019-11-12 21:32:56.000000 mo-json-config-3.7.19316/README.md
--rw-rw-rw-   0        0        0       42 2019-11-12 22:46:20.000000 mo-json-config-3.7.19316/setup.cfg
--rw-rw-rw-   0        0        0     9932 2019-11-12 22:46:20.000000 mo-json-config-3.7.19316/setup.py
+drwxrwxrwx   0        0        0        0 2020-07-08 11:17:06.000000 mo-json-config-3.77.20190/
+-rw-rw-rw-   0        0        0    12166 2020-07-08 11:17:06.000000 mo-json-config-3.77.20190/PKG-INFO
+-rw-rw-rw-   0        0        0     8601 2019-11-12 21:32:56.000000 mo-json-config-3.77.20190/README.md
+drwxrwxrwx   0        0        0        0 2020-07-08 11:17:06.000000 mo-json-config-3.77.20190/mo_json_config/
+-rw-rw-rw-   0        0        0     8844 2020-07-08 11:16:54.000000 mo-json-config-3.77.20190/mo_json_config/__init__.py
+-rw-rw-rw-   0        0        0      763 2020-07-08 11:16:54.000000 mo-json-config-3.77.20190/mo_json_config/convert.py
+drwxrwxrwx   0        0        0        0 2020-07-08 11:17:06.000000 mo-json-config-3.77.20190/mo_json_config.egg-info/
+-rw-rw-rw-   0        0        0    12166 2020-07-08 11:17:06.000000 mo-json-config-3.77.20190/mo_json_config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2020-07-08 11:17:06.000000 mo-json-config-3.77.20190/mo_json_config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-07-08 11:17:06.000000 mo-json-config-3.77.20190/mo_json_config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2020-07-08 11:17:06.000000 mo-json-config-3.77.20190/mo_json_config.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2020-07-08 11:17:06.000000 mo-json-config-3.77.20190/mo_json_config.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-07-08 11:17:06.000000 mo-json-config-3.77.20190/setup.cfg
+-rw-rw-rw-   0        0        0     9892 2020-07-08 11:16:54.000000 mo-json-config-3.77.20190/setup.py
```

### Comparing `mo-json-config-3.7.19316/mo_json_config/convert.py` & `mo-json-config-3.77.20190/mo_json_config/convert.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # encoding: utf-8
 #
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
-# Author: Kyle Lahnakoski (kyle@lahnakoski.com)
+# Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 from __future__ import absolute_import, division, unicode_literals
 
-from mo_dots import wrap
+from mo_dots import to_data
 from mo_future import ConfigParser, StringIO
 
 
 def ini2value(ini_content):
     """
     INI FILE CONTENT TO Data
     """
@@ -23,8 +23,8 @@
     config._read(buff, "dummy")
 
     output = {}
     for section in config.sections():
         output[section] = s = {}
         for k, v in config.items(section):
             s[k] = v
-    return wrap(output)
+    return to_data(output)
```

### Comparing `mo-json-config-3.7.19316/mo_json_config/__init__.py` & `mo-json-config-3.77.20190/mo_json_config/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # encoding: utf-8
 #
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
-# Author: Kyle Lahnakoski (kyle@lahnakoski.com)
+# Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 from __future__ import absolute_import, division, unicode_literals
 
-from mo_future import is_text, is_binary
 import os
 
-import mo_dots
-from mo_dots import is_data, is_list, set_default, unwrap, wrap
+from mo_dots import is_data, is_list, set_default, unwrap, to_data, is_sequence, coalesce, get_attr, listwrap, unwraplist, \
+    dict_to_data
 from mo_files import File
 from mo_files.url import URL
+from mo_future import is_text
 from mo_future import text
 from mo_json import json2value
 from mo_json_config.convert import ini2value
 from mo_logs import Except, Log
 
 DEBUG = False
 
 
 def get_file(file):
     file = File(file)
-    if os.sep=="\\":
+    if os.sep == "\\":
         return get("file:///" + file.abspath)
     else:
         return get("file://" + file.abspath)
 
 
 def get(url):
     """
@@ -46,18 +46,18 @@
         if os.sep=="\\":
             base = URL("file:///" + os.getcwd().replace(os.sep, "/").rstrip("/") + "/.")
         else:
             base = URL("file://" + os.getcwd().rstrip("/") + "/.")
     elif url[url.find("://") + 3] != "/":
         Log.error("{{url}} must be absolute", url=url)
 
-    phase1 = _replace_ref(wrap({"$ref": url}), base)  # BLANK URL ONLY WORKS IF url IS ABSOLUTE
+    phase1 = _replace_ref(dict_to_data({"$ref": url}), base)  # BLANK URL ONLY WORKS IF url IS ABSOLUTE
     try:
         phase2 = _replace_locals(phase1, [phase1])
-        return wrap(phase2)
+        return to_data(phase2)
     except Exception as e:
         Log.error("problem replacing locals in\n{{phase1}}", phase1=phase1, cause=e)
 
 
 def expand(doc, doc_url="param://", params=None):
     """
     ASSUMING YOU ALREADY PULED THE doc FROM doc_url, YOU CAN STILL USE THE
@@ -73,65 +73,76 @@
     if doc_url.find("://") == -1:
         Log.error("{{url}} must have a prototcol (eg http://) declared", url=doc_url)
 
     url = URL(doc_url)
     url.query = set_default(url.query, params)
     phase1 = _replace_ref(doc, url)  # BLANK URL ONLY WORKS IF url IS ABSOLUTE
     phase2 = _replace_locals(phase1, [phase1])
-    return wrap(phase2)
+    return to_data(phase2)
 
 
 def _replace_ref(node, url):
     if url.path.endswith("/"):
         url.path = url.path[:-1]
 
     if is_data(node):
-        ref = None
+        refs = None
         output = {}
         for k, v in node.items():
             if k == "$ref":
-                ref = URL(v)
+                refs = URL(v)
             else:
                 output[k] = _replace_ref(v, url)
 
-        if not ref:
+        if not refs:
             return output
 
-        node = output
-
-        if not ref.scheme and not ref.path:
-            # DO NOT TOUCH LOCAL REF YET
-            output["$ref"] = ref
-            return output
+        ref_found = False
+        ref_error = None
+        ref_remain = []
+        for ref in listwrap(refs):
+            if not ref.scheme and not ref.path:
+                # DO NOT TOUCH LOCAL REF YET
+                ref_remain.append(ref)
+                ref_found = True
+                continue
 
-        if not ref.scheme:
-            # SCHEME RELATIVE IMPLIES SAME PROTOCOL AS LAST TIME, WHICH
-            # REQUIRES THE CURRENT DOCUMENT'S SCHEME
-            ref.scheme = url.scheme
-
-        # FIND THE SCHEME AND LOAD IT
-        if ref.scheme in scheme_loaders:
-            new_value = scheme_loaders[ref.scheme](ref, url)
-        else:
-            raise Log.error("unknown protocol {{scheme}}", scheme=ref.scheme)
+            if not ref.scheme:
+                # SCHEME RELATIVE IMPLIES SAME PROTOCOL AS LAST TIME, WHICH
+                # REQUIRES THE CURRENT DOCUMENT'S SCHEME
+                ref.scheme = url.scheme
+
+            # FIND THE SCHEME AND LOAD IT
+            if ref.scheme not in scheme_loaders:
+                raise Log.error("unknown protocol {{scheme}}", scheme=ref.scheme)
+            try:
+                new_value = scheme_loaders[ref.scheme](ref, url)
+                ref_found = True
+            except Exception as e:
+                e = Except.wrap(e)
+                ref_error = e
+                continue
 
-        if ref.fragment:
-            new_value = mo_dots.get_attr(new_value, ref.fragment)
+            if ref.fragment:
+                new_value = get_attr(new_value, ref.fragment)
 
-        DEBUG and Log.note("Replace {{ref}} with {{new_value}}", ref=ref, new_value=new_value)
+            DEBUG and Log.note("Replace {{ref}} with {{new_value}}", ref=ref, new_value=new_value)
 
-        if not output:
-            output = new_value
-        elif is_text(output):
-            Log.error("Can not handle set_default({{output}},{{new_value}})", output=output, new_value=new_value)
-        else:
-            output = unwrap(set_default(output, new_value))
+            if not output:
+                output = new_value
+            elif is_text(output):
+                pass  # WE HAVE A VALUE
+            else:
+                set_default(output, new_value)
 
+        if not ref_found:
+            raise ref_error
+        if ref_remain:
+            output["$ref"] = unwraplist(ref_remain)
         DEBUG and Log.note("Return {{output}}", output=output)
-
         return output
     elif is_list(node):
         output = [_replace_ref(n, url) for n in node]
         # if all(p[0] is p[1] for p in zip(output, node)):
         #     return node
         return output
 
@@ -142,14 +153,18 @@
     if is_data(node):
         # RECURS, DEEP COPY
         ref = None
         output = {}
         for k, v in node.items():
             if k == "$ref":
                 ref = v
+            elif k == "$concat":
+                if not is_sequence(v):
+                    Log.error("$concat expects an array of strings")
+                return coalesce(node.get("separator"), "").join(v)
             elif v == None:
                 continue
             else:
                 output[k] = _replace_locals(v, [v] + doc_path)
 
         if not ref:
             return output
@@ -158,21 +173,21 @@
         frag = ref.fragment
         if frag[0] == ".":
             # RELATIVE
             for i, p in enumerate(frag):
                 if p != ".":
                     if i>len(doc_path):
                         Log.error("{{frag|quote}} reaches up past the root document",  frag=frag)
-                    new_value = mo_dots.get_attr(doc_path[i-1], frag[i::])
+                    new_value = get_attr(doc_path[i-1], frag[i::])
                     break
             else:
                 new_value = doc_path[len(frag) - 1]
         else:
             # ABSOLUTE
-            new_value = mo_dots.get_attr(doc_path[-1], frag)
+            new_value = get_attr(doc_path[-1], frag)
 
         new_value = _replace_locals(new_value, [new_value] + doc_path)
 
         if not output:
             return new_value  # OPTIMIZATION FOR CASE WHEN node IS {}
         else:
             return unwrap(set_default(output, new_value))
@@ -241,18 +256,22 @@
     new_value = json2value(requests.get(ref), params=params, flexible=True, leaves=True)
     return new_value
 
 
 def _get_env(ref, url):
     # GET ENVIRONMENT VARIABLES
     ref = ref.host
+    raw_value = os.environ.get(ref)
+    if not raw_value:
+        Log.error("expecting environment variable with name {{env_var}}", env_var=ref)
+
     try:
-        new_value = json2value(os.environ[ref])
+        new_value = json2value(raw_value)
     except Exception as e:
-        new_value = os.environ.get(ref)
+        new_value = raw_value
     return new_value
 
 
 def _get_param(ref, url):
     # GET PARAMETERS FROM url
     param = url.query
     new_value = param[ref.host]
```

### Comparing `mo-json-config-3.7.19316/mo_json_config.egg-info/PKG-INFO` & `mo-json-config-3.77.20190/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json-config
-Version: 3.7.19316
+Version: 3.77.20190
 Summary: More JSON Configuration! JSON configuration files with `$ref` and template overlays
 Home-page: https://github.com/klahnakoski/mo-json-config
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Description: More JSON Configuration!
         ========================
```

### Comparing `mo-json-config-3.7.19316/PKG-INFO` & `mo-json-config-3.77.20190/mo_json_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json-config
-Version: 3.7.19316
+Version: 3.77.20190
 Summary: More JSON Configuration! JSON configuration files with `$ref` and template overlays
 Home-page: https://github.com/klahnakoski/mo-json-config
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Description: More JSON Configuration!
         ========================
```

### Comparing `mo-json-config-3.7.19316/README.md` & `mo-json-config-3.77.20190/README.md`

 * *Files identical despite different names*

### Comparing `mo-json-config-3.7.19316/setup.py` & `mo-json-config-3.77.20190/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # encoding: utf-8
 # THIS FILE IS AUTOGENERATED!
 from __future__ import unicode_literals
 from setuptools import setup
 setup(
-    description=str(u'More JSON Configuration! JSON configuration files with `$ref` and template overlays'),
-    license=str(u'MPL 2.0'),
-    author=str(u'Kyle Lahnakoski'),
-    author_email=str(u'kyle@lahnakoski.com'),
-    long_description_content_type=str(u'text/markdown'),
+    author='Kyle Lahnakoski',
+    author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)"],
-    install_requires=["mo-dots>=3.2.19316","mo-files>=3.4.19316","mo-future>=3.1.19316","mo-json>=3.4.19316","mo-logs>=3.5.19316","requests"],
-    version=str(u'3.7.19316'),
-    url=str(u'https://github.com/klahnakoski/mo-json-config'),
+    description='More JSON Configuration! JSON configuration files with `$ref` and template overlays',
+    install_requires=["hjson","mo-dots>=3.77.20190","mo-files>=3.77.20190","mo-future>=3.71.20168","mo-json>=3.77.20190","mo-logs>=3.75.20189","requests"],
+    license='MPL 2.0',
+    long_description='More JSON Configuration!\n========================\n\nA JSON template format intended for configuration files.\n\nMotivation\n----------\n\nThis module has superficial similarity to the [JSON Reference Draft](https://tools.ietf.org/html/draft-pbryan-zyp-json-ref-03), which seems inspired by the committee-driven XPath specification, and as a result, made some poor design choices. Here are the improvements this module makes:\n\n1. This module uses the dot (`.`) as a path separator in the URL fragment. For example, an absolute reference looks like `{"$ref": "#message.type.name"}`, and a relative reference looks like `{"$ref": "#..type.name"}`.   This syntax better matches that used by Javascript.\n2. The properties found in a `$ref` object are not ignored. Rather, they are to *override* the referenced object properties. This allows you to reference a default document, and replace the particular properties as needed. *more below*\n3. References can accept URL parameters: JSON is treated like a string template for more sophisticated value replacement. *see below*\n4. You can reference files and environment variables in addition to general URLs.\n\nUsage\n-----\n\nLoad your application settings with:\n\n    settings = mo_json_config.get(url):\n\n\nComments\n--------\n\nEnd-of-line Comments are allowed, using either `#` or `//` prefix:\n\n```javascript\n    {\n        "key1": "value1",  //Comment 1\n    }\n```\n\n```python\n        "key1": "value1",  #Comment 1\n```\n\nMultiline comments are also allowed, using either Python\'s triple-quotes\n(`""" ... """`) or Javascript\'s block quotes `/*...*/`\n\n```javascript\n    {\n        "key1": /* Comment 1 */ "value1",\n    }\n```\n\n```python\n        "key1": """Comment 1""" "value1",\n```\n\n\nExample References\n------------------\n\nThe `$ref` property is special. Its value is interpreted as a URL pointing to more JSON\n\n### Absolute Internal Reference\n\nThe simplest form of URL is an absolute reference to a node in the same\ndocument:\n\n\n```python\n    {\n        "message": "Hello world",\n        "repeat": {"$ref": "#message"}\n    }\n```\n\nThe reference must start with `#`, and the object with the `$ref` is replaced\nwith the value it points to:\n\n```python\n    {\n        "message": "Hello world",\n        "repeat": "Hello world"\n    }\n```\n\n### Relative Internal References\n\nReferences that start with dot (`.`) are relative, with each additional dot\nreferring to successive parents.   In this case the `..` refers to the\nref-object\'s parent, and expands just like the previous example:\n\n```python\n    {\n        "message": "Hello world",\n        "repeat": {"$ref": "#..message"}\n    }\n```\n\n### File References\n\nConfiguration is often stored on the local file system. You can in-line the\nJSON found in a file by using the `file://` scheme:\n\nIt is good practice to store sensitive data in a secure place...\n\n```python\n    {# LOCATED IN C:\\users\\kyle\\password.json\n        "host": "database.example.com",\n        "username": "kyle",\n        "password": "pass123"\n    }\n```\n...and then refer to it in your configuration file:\n\n```python\n    {\n        "host": "example.com",\n        "port": "8080",\n        "$ref": "file:///C:/users/kyle/password.json"\n    }\n```\n\nwhich will be expanded at run-time to:\n\n```python\n    {\n        "host": "example.com",\n        "port": "8080",\n        "username": "kyle",\n        "password": "pass123"\n    }\n```\n\nPlease notice the triple slash (`///`) is referring to an absolute file\nreference.\n\n### References To Objects\n\nRef-objects that point to other objects (dicts) are not replaced completely,\nbut rather are merged with the target; with the ref-object\nproperties taking precedence.   This is seen in the example above: The "host"\nproperty is not overwritten by the target\'s.\n\n### Relative File Reference\n\nHere is the same, using a relative file reference; which is relative to the\nfile that contains this JSON\n\n```python\n    {#LOCATED IN C:\\users\\kyle\\dev-debug.json\n        "host": "example.com",\n        "port": "8080",\n        "$ref": "file://password.json"\n    }\n```\n\n### Home Directory Reference\n\nYou may also use the tilde (`~`) to refer to the current user\'s home directory.\nHere is the same again, but this example can be anywhere in the file system.\n\n```python\n    {\n        "host": "example.com",\n        "port": "8080",\n        "$ref": "file://~/password.json"\n    }\n```\n\n### HTTP Reference\n\nConfiguration can be stored remotely, especially in the case of larger\nconfigurations which are too unwieldy to inline:\n\n```python\n    {\n        "schema":{"$ref": "http://example.com/sources/my_db.json"}\n    }\n```\n\n### Scheme-Relative Reference\n\nYou are also able to leave the scheme off, so that whole constellations of\nconfiguration files can refer to each other no matter if they are on the local\nfile system, or remote:\n\n```python\n    {# LOCATED AT SOMEWHERE AT http://example.com\n        "schema":{"$ref": "///sources/my_db.json"}\n    }\n```\n\nAnd, of course, relative references are also allowed:\n\n```python\n    {# LOCATED AT http://example.com/sources/dev-debug.json\n        "schema":{"$ref": "//sources/my_db.json"}\n    }\n```\n\n### Fragment Reference\n\nSome remote configuration files are quite large...\n\n```python\n    {# LOCATED IN C:\\users\\kyle\\password.json\n        "database":{\n            "username": "kyle",\n            "password": "pass123"\n        },\n        "email":{\n            "username": "ekyle",\n            "password": "pass123"\n        }\n    }\n```\n\n... and you only need one fragment. For this use the hash (`#`) followed by\nthe dot-delimited path into the document:\n\n```python\n    {\n        "host": "mail.example.com",\n        "username": "ekyle"\n        "password": {"$ref": "//~/password.json#email.password"}\n    }\n```\n\n### Environment Variables Reference\n\n`mo-json-config` uses the unconventional `env` scheme for accessing environment variables:\n\n```python\n    {\n        "host": "mail.example.com",\n        "username": "ekyle"\n        "password": {"$ref": "env://MAIL_PASSWORD"}\n    }\n```\n### Parameters Reference\n\nYou can reference the variables found in `$ref` URL by using the `param` scheme. For example, the following  JSON document demands that it be provided with a `password` parameter:  \n\n    { # LOCATED AT http://example.com/machine_config.json\n        "host": "mail.example.com",\n        "username": "ekyle"\n        "password": {"$ref": "param:///password"}\n    }\n\n**The `param` scheme does not conform to the URL spec: It only accepts dot-delimited paths.**\n\nThis parametric JSON can be expanded with a $ref\n\n\t{"config": {\n\t\t"$ref": "http://example.com/machine_config.json?password=pass123"\n\t}}\n\nexpands to \n\n    {"config": {\n        "host": "mail.example.com",\n        "username": "ekyle"\n        "password": "pass123"\n    }}\n\nURL parameters and `$ref` properties can conflict. Let\'s consider \n\n\t{"config": {\n\t\t"$ref": "http://example.com/machine_config.json?password=pass123",\n\t\t"password": "123456"\n\t}}\n\nthe URL paramters are used to expand the given document, **then** the `$ref` properties override the contents of the document:\n\n    {"config": {\n        "host": "mail.example.com",\n        "username": "ekyle"\n        "password": "123456"\n    }}\n\n\n## Parameterized JSON\n\nThe `param` scheme is a good way to set property values in a document, but sometimes that is not enough.  Sometimes you want to parameterize property names, or change the document structure in unconventional ways. For these cases, JSON documents are allowed named parameters at the unicode level. Parameters are surrounded by moustaches `{{.}}`:\n\n```javascript\n\t{//above_example.json\n\t \t{{var_name}}: "value"\n\t}\n```\n\nParameter replacement is performed on the unicode text before being interpreted by the JSON parser. It is your responsibility to ensure the parameter replacement will result in valid JSON.\n\nYou pass the parameters by including them as URL parameters:\n\n\t{"$ref": "//~/above_example.json?var_name=%22hello%22"}\n\nWhich will expand to\n\n```javascript\n\t{\n\t \t"hello": "value"\n\t}\n```\n\nThe pipe (`|`) symbol can be used to perform some common conversions\n\n\n```javascript\n\t{\n\t \t{{var_name|quote}}: "value"\n\t}\n```\n\nThe `quote` transformation will deal with quoting, so ...\n\n\t{"$ref": "//~/above_example.json?var_name=hello"}\n\n... expands to the same:\n\n```javascript\n\t{\n\t \t"hello": "value"\n\t}\n```\n\nPlease see [`expand_template()` in the `strings` module](https://github.com/klahnakoski/mo-logs/blob/dev/mo_logs/strings.py) for more on the parameter replacement, and transformations available\n\n\n---\n\nalso see [http://tools.ietf.org/id/draft-pbryan-zyp-json-ref-03.html](http://tools.ietf.org/id/draft-pbryan-zyp-json-ref-03.html)\n',
+    long_description_content_type='text/markdown',
+    name='mo-json-config',
     packages=["mo_json_config"],
-    long_description=str(u'More JSON Configuration!\n========================\n\nA JSON template format intended for configuration files.\n\nMotivation\n----------\n\nThis module has superficial similarity to the [JSON Reference Draft](https://tools.ietf.org/html/draft-pbryan-zyp-json-ref-03), which seems inspired by the committee-driven XPath specification, and as a result, made some poor design choices. Here are the improvements this module makes:\n\n1. This module uses the dot (`.`) as a path separator in the URL fragment. For example, an absolute reference looks like `{"$ref": "#message.type.name"}`, and a relative reference looks like `{"$ref": "#..type.name"}`.   This syntax better matches that used by Javascript.\n2. The properties found in a `$ref` object are not ignored. Rather, they are to *override* the referenced object properties. This allows you to reference a default document, and replace the particular properties as needed. *more below*\n3. References can accept URL parameters: JSON is treated like a string template for more sophisticated value replacement. *see below*\n4. You can reference files and environment variables in addition to general URLs.\n\nUsage\n-----\n\nLoad your application settings with:\n\n    settings = mo_json_config.get(url):\n\n\nComments\n--------\n\nEnd-of-line Comments are allowed, using either `#` or `//` prefix:\n\n```javascript\n    {\n        "key1": "value1",  //Comment 1\n    }\n```\n\n```python\n        "key1": "value1",  #Comment 1\n```\n\nMultiline comments are also allowed, using either Python\'s triple-quotes\n(`""" ... """`) or Javascript\'s block quotes `/*...*/`\n\n```javascript\n    {\n        "key1": /* Comment 1 */ "value1",\n    }\n```\n\n```python\n        "key1": """Comment 1""" "value1",\n```\n\n\nExample References\n------------------\n\nThe `$ref` property is special. Its value is interpreted as a URL pointing to more JSON\n\n### Absolute Internal Reference\n\nThe simplest form of URL is an absolute reference to a node in the same\ndocument:\n\n\n```python\n    {\n        "message": "Hello world",\n        "repeat": {"$ref": "#message"}\n    }\n```\n\nThe reference must start with `#`, and the object with the `$ref` is replaced\nwith the value it points to:\n\n```python\n    {\n        "message": "Hello world",\n        "repeat": "Hello world"\n    }\n```\n\n### Relative Internal References\n\nReferences that start with dot (`.`) are relative, with each additional dot\nreferring to successive parents.   In this case the `..` refers to the\nref-object\'s parent, and expands just like the previous example:\n\n```python\n    {\n        "message": "Hello world",\n        "repeat": {"$ref": "#..message"}\n    }\n```\n\n### File References\n\nConfiguration is often stored on the local file system. You can in-line the\nJSON found in a file by using the `file://` scheme:\n\nIt is good practice to store sensitive data in a secure place...\n\n```python\n    {# LOCATED IN C:\\users\\kyle\\password.json\n        "host": "database.example.com",\n        "username": "kyle",\n        "password": "pass123"\n    }\n```\n...and then refer to it in your configuration file:\n\n```python\n    {\n        "host": "example.com",\n        "port": "8080",\n        "$ref": "file:///C:/users/kyle/password.json"\n    }\n```\n\nwhich will be expanded at run-time to:\n\n```python\n    {\n        "host": "example.com",\n        "port": "8080",\n        "username": "kyle",\n        "password": "pass123"\n    }\n```\n\nPlease notice the triple slash (`///`) is referring to an absolute file\nreference.\n\n### References To Objects\n\nRef-objects that point to other objects (dicts) are not replaced completely,\nbut rather are merged with the target; with the ref-object\nproperties taking precedence.   This is seen in the example above: The "host"\nproperty is not overwritten by the target\'s.\n\n### Relative File Reference\n\nHere is the same, using a relative file reference; which is relative to the\nfile that contains this JSON\n\n```python\n    {#LOCATED IN C:\\users\\kyle\\dev-debug.json\n        "host": "example.com",\n        "port": "8080",\n        "$ref": "file://password.json"\n    }\n```\n\n### Home Directory Reference\n\nYou may also use the tilde (`~`) to refer to the current user\'s home directory.\nHere is the same again, but this example can be anywhere in the file system.\n\n```python\n    {\n        "host": "example.com",\n        "port": "8080",\n        "$ref": "file://~/password.json"\n    }\n```\n\n### HTTP Reference\n\nConfiguration can be stored remotely, especially in the case of larger\nconfigurations which are too unwieldy to inline:\n\n```python\n    {\n        "schema":{"$ref": "http://example.com/sources/my_db.json"}\n    }\n```\n\n### Scheme-Relative Reference\n\nYou are also able to leave the scheme off, so that whole constellations of\nconfiguration files can refer to each other no matter if they are on the local\nfile system, or remote:\n\n```python\n    {# LOCATED AT SOMEWHERE AT http://example.com\n        "schema":{"$ref": "///sources/my_db.json"}\n    }\n```\n\nAnd, of course, relative references are also allowed:\n\n```python\n    {# LOCATED AT http://example.com/sources/dev-debug.json\n        "schema":{"$ref": "//sources/my_db.json"}\n    }\n```\n\n### Fragment Reference\n\nSome remote configuration files are quite large...\n\n```python\n    {# LOCATED IN C:\\users\\kyle\\password.json\n        "database":{\n            "username": "kyle",\n            "password": "pass123"\n        },\n        "email":{\n            "username": "ekyle",\n            "password": "pass123"\n        }\n    }\n```\n\n... and you only need one fragment. For this use the hash (`#`) followed by\nthe dot-delimited path into the document:\n\n```python\n    {\n        "host": "mail.example.com",\n        "username": "ekyle"\n        "password": {"$ref": "//~/password.json#email.password"}\n    }\n```\n\n### Environment Variables Reference\n\n`mo-json-config` uses the unconventional `env` scheme for accessing environment variables:\n\n```python\n    {\n        "host": "mail.example.com",\n        "username": "ekyle"\n        "password": {"$ref": "env://MAIL_PASSWORD"}\n    }\n```\n### Parameters Reference\n\nYou can reference the variables found in `$ref` URL by using the `param` scheme. For example, the following  JSON document demands that it be provided with a `password` parameter:  \n\n    { # LOCATED AT http://example.com/machine_config.json\n        "host": "mail.example.com",\n        "username": "ekyle"\n        "password": {"$ref": "param:///password"}\n    }\n\n**The `param` scheme does not conform to the URL spec: It only accepts dot-delimited paths.**\n\nThis parametric JSON can be expanded with a $ref\n\n\t{"config": {\n\t\t"$ref": "http://example.com/machine_config.json?password=pass123"\n\t}}\n\nexpands to \n\n    {"config": {\n        "host": "mail.example.com",\n        "username": "ekyle"\n        "password": "pass123"\n    }}\n\nURL parameters and `$ref` properties can conflict. Let\'s consider \n\n\t{"config": {\n\t\t"$ref": "http://example.com/machine_config.json?password=pass123",\n\t\t"password": "123456"\n\t}}\n\nthe URL paramters are used to expand the given document, **then** the `$ref` properties override the contents of the document:\n\n    {"config": {\n        "host": "mail.example.com",\n        "username": "ekyle"\n        "password": "123456"\n    }}\n\n\n## Parameterized JSON\n\nThe `param` scheme is a good way to set property values in a document, but sometimes that is not enough.  Sometimes you want to parameterize property names, or change the document structure in unconventional ways. For these cases, JSON documents are allowed named parameters at the unicode level. Parameters are surrounded by moustaches `{{.}}`:\n\n```javascript\n\t{//above_example.json\n\t \t{{var_name}}: "value"\n\t}\n```\n\nParameter replacement is performed on the unicode text before being interpreted by the JSON parser. It is your responsibility to ensure the parameter replacement will result in valid JSON.\n\nYou pass the parameters by including them as URL parameters:\n\n\t{"$ref": "//~/above_example.json?var_name=%22hello%22"}\n\nWhich will expand to\n\n```javascript\n\t{\n\t \t"hello": "value"\n\t}\n```\n\nThe pipe (`|`) symbol can be used to perform some common conversions\n\n\n```javascript\n\t{\n\t \t{{var_name|quote}}: "value"\n\t}\n```\n\nThe `quote` transformation will deal with quoting, so ...\n\n\t{"$ref": "//~/above_example.json?var_name=hello"}\n\n... expands to the same:\n\n```javascript\n\t{\n\t \t"hello": "value"\n\t}\n```\n\nPlease see [`expand_template()` in the `strings` module](https://github.com/klahnakoski/mo-logs/blob/dev/mo_logs/strings.py) for more on the parameter replacement, and transformations available\n\n\n---\n\nalso see [http://tools.ietf.org/id/draft-pbryan-zyp-json-ref-03.html](http://tools.ietf.org/id/draft-pbryan-zyp-json-ref-03.html)\n'),
-    name=str(u'mo-json-config')
+    url='https://github.com/klahnakoski/mo-json-config',
+    version='3.77.20190'
 )
```

