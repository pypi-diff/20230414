# Comparing `tmp/curl_arguments_url-0.1.1.tar.gz` & `tmp/curl_arguments_url-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curl_arguments_url-0.1.1.tar", last modified: Fri Apr 14 16:47:07 2023, max compression
+gzip compressed data, was "curl_arguments_url-0.1.2.tar", last modified: Fri Apr 14 18:17:24 2023, max compression
```

## Comparing `curl_arguments_url-0.1.1.tar` & `curl_arguments_url-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:47:07.092325 curl_arguments_url-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-04-14 16:47:07.092325 curl_arguments_url-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:47:07.088325 curl_arguments_url-0.1.1/curl_arguments_url/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/curl_arguments_url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/curl_arguments_url/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/curl_arguments_url/click_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    55084 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/curl_arguments_url/curl_arguments_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:47:07.092325 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 16:47:07.000000 curl_arguments_url-0.1.1/curl_arguments_url.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-14 16:47:07.092325 curl_arguments_url-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 16:46:57.000000 curl_arguments_url-0.1.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:24.600050 curl_arguments_url-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-04-14 18:17:24.600050 curl_arguments_url-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:24.600050 curl_arguments_url-0.1.2/curl_arguments_url/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/curl_arguments_url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/curl_arguments_url/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/curl_arguments_url/click_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55084 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/curl_arguments_url/curl_arguments_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:17:24.600050 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 18:17:24.000000 curl_arguments_url-0.1.2/curl_arguments_url.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-14 18:17:24.600050 curl_arguments_url-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 18:17:17.000000 curl_arguments_url-0.1.2/version.txt
```

### Comparing `curl_arguments_url-0.1.1/LICENSE` & `curl_arguments_url-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.1/PKG-INFO` & `curl_arguments_url-0.1.2/curl_arguments_url.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: curl_arguments_url
-Version: 0.1.1
+Name: curl-arguments-url
+Version: 0.1.2
 Summary: Curl with Arguments for Url
 Home-page: https://github.com/valmikirao/curl_arguments_url
 Author: Valmiki Rao
 Author-email: valmikirao@gmail.com
 License: Apache Software License 2.0
 Keywords: curl_arguments_url,carl,curl,zsh,completions,swagger,openapi
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -45,14 +45,17 @@
 # globally
 % pipx install 'curl_arguments_url'
 # or in a particular virtual env
 % pip install 'curl_arguments_url'
 
 # to get the completions to work, add the following to your .zshrc
 eval "$(carl utils zsh-print-script)"
+
+# And copy the OpenAPI spec into ~/.carl/open_api to get the completions and curl-building working
+% cp open_api-spec.yml ~/.carl/open_api
 ```
 
 ### Examples
 
 These examples use [tests/resources/open_api/openapi-demo.yml](tests/resources/open_api/openapi-demo.yml)
 
 * Basic GET
@@ -127,15 +130,18 @@
   -h, --help            show this help message and exit
 
 Environment Variables:
     CARL_DIR: Directory which contains files for carl. Default: ~/.carl
     CARL_OPEN_API_DIR: Directory containing the OpenApi specifications and
                         Yaml files. Default: $CARL_DIR/open_api
     CARL_CACHE_DIR: Directory containing the cache. Default $CARL_DIR/cache
+```
 
+For a specific endpoint:
+```text
 % carl http://demo.io/v0/entities/\{path-item\} POST --help
 usage: carl http://demo.io/v0/entities/{path-item} POST [-h] [-p] [-n] [-R] [-b BODY_JSON] [+field-header FIELD_HEADER] [+field-one FIELD_ONE]
                                                         [+field-two FIELD_TWO [FIELD_TWO ...]] [+field-three FIELD_THREE] +path-item PATH_ITEM
                                                         [passed_to_curl ...]
 
 Demo Post Command
 
@@ -161,14 +167,16 @@
 
 * Generic Optional Args:
 
 ```text
   -p, --print-cmd       Print the resulting curl command to standard out
   -n, --no-run          Don't run the curl command. Useful with -p
   -R, --no-requires     Don't check to see if required parameter values are missing or if values are one of the enumerated values
+  -b BODY_JSON, --body-json BODY_JSON, --body BODY_JSON
+                        Base json object to send in the body. Required body params are still required unless -R option passed. Useful for dealing with incomplete specs.
 ```
 
 * Relevant Environment Variables
 
 ```text
     CARL_DIR: Directory which contains files for carl. Default: ~/.carl
     CARL_OPEN_API_DIR: Directory containing the OpenApi specifications and
@@ -205,11 +213,15 @@
 * Support file uploading and downloading
 * Utilize the authorization part of the OpenAPI spec
 * Better support for nested json objects in the body, so that `+param.sub-param value` would set
     `{"param"{"sub-param":"value"}}`
 * Maybe support older versions of Swagger/OpenApi
 * Speaking of which, in the code I sometimes use the term "swagger" and sometimes "open_api".  I should make this
     consistent.
+* Support bash and fish.  With how I implemented this, I thought it would be easy to implement bash.  But the way bash
+    parses and escapes arguments passed to the completion function made it surprisingly challenging.  The
+    `bash-completion` branch has my so-far attempts to deal with these issues.  It might be close to done, or there
+    might be a slew of other issues I haven't realized yet.
 
 ## Credits
 
 This package was created with _cookiecutter_ and the `audreyr/cookiecutter-pypackage` project template.
```

### Comparing `curl_arguments_url-0.1.1/README.md` & `curl_arguments_url-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 # globally
 % pipx install 'curl_arguments_url'
 # or in a particular virtual env
 % pip install 'curl_arguments_url'
 
 # to get the completions to work, add the following to your .zshrc
 eval "$(carl utils zsh-print-script)"
+
+# And copy the OpenAPI spec into ~/.carl/open_api to get the completions and curl-building working
+% cp open_api-spec.yml ~/.carl/open_api
 ```
 
 ### Examples
 
 These examples use [tests/resources/open_api/openapi-demo.yml](tests/resources/open_api/openapi-demo.yml)
 
 * Basic GET
@@ -104,15 +107,18 @@
   -h, --help            show this help message and exit
 
 Environment Variables:
     CARL_DIR: Directory which contains files for carl. Default: ~/.carl
     CARL_OPEN_API_DIR: Directory containing the OpenApi specifications and
                         Yaml files. Default: $CARL_DIR/open_api
     CARL_CACHE_DIR: Directory containing the cache. Default $CARL_DIR/cache
+```
 
+For a specific endpoint:
+```text
 % carl http://demo.io/v0/entities/\{path-item\} POST --help
 usage: carl http://demo.io/v0/entities/{path-item} POST [-h] [-p] [-n] [-R] [-b BODY_JSON] [+field-header FIELD_HEADER] [+field-one FIELD_ONE]
                                                         [+field-two FIELD_TWO [FIELD_TWO ...]] [+field-three FIELD_THREE] +path-item PATH_ITEM
                                                         [passed_to_curl ...]
 
 Demo Post Command
 
@@ -138,14 +144,16 @@
 
 * Generic Optional Args:
 
 ```text
   -p, --print-cmd       Print the resulting curl command to standard out
   -n, --no-run          Don't run the curl command. Useful with -p
   -R, --no-requires     Don't check to see if required parameter values are missing or if values are one of the enumerated values
+  -b BODY_JSON, --body-json BODY_JSON, --body BODY_JSON
+                        Base json object to send in the body. Required body params are still required unless -R option passed. Useful for dealing with incomplete specs.
 ```
 
 * Relevant Environment Variables
 
 ```text
     CARL_DIR: Directory which contains files for carl. Default: ~/.carl
     CARL_OPEN_API_DIR: Directory containing the OpenApi specifications and
@@ -182,11 +190,15 @@
 * Support file uploading and downloading
 * Utilize the authorization part of the OpenAPI spec
 * Better support for nested json objects in the body, so that `+param.sub-param value` would set
     `{"param"{"sub-param":"value"}}`
 * Maybe support older versions of Swagger/OpenApi
 * Speaking of which, in the code I sometimes use the term "swagger" and sometimes "open_api".  I should make this
     consistent.
+* Support bash and fish.  With how I implemented this, I thought it would be easy to implement bash.  But the way bash
+    parses and escapes arguments passed to the completion function made it surprisingly challenging.  The
+    `bash-completion` branch has my so-far attempts to deal with these issues.  It might be close to done, or there
+    might be a slew of other issues I haven't realized yet.
 
 ## Credits
 
 This package was created with _cookiecutter_ and the `audreyr/cookiecutter-pypackage` project template.
```

### Comparing `curl_arguments_url-0.1.1/curl_arguments_url/cli.py` & `curl_arguments_url-0.1.2/curl_arguments_url/cli.py`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.1/curl_arguments_url/click_test.py` & `curl_arguments_url-0.1.2/curl_arguments_url/click_test.py`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.1/curl_arguments_url/curl_arguments_url.py` & `curl_arguments_url-0.1.2/curl_arguments_url/curl_arguments_url.py`

 * *Files identical despite different names*

### Comparing `curl_arguments_url-0.1.1/curl_arguments_url.egg-info/PKG-INFO` & `curl_arguments_url-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: curl-arguments-url
-Version: 0.1.1
+Name: curl_arguments_url
+Version: 0.1.2
 Summary: Curl with Arguments for Url
 Home-page: https://github.com/valmikirao/curl_arguments_url
 Author: Valmiki Rao
 Author-email: valmikirao@gmail.com
 License: Apache Software License 2.0
 Keywords: curl_arguments_url,carl,curl,zsh,completions,swagger,openapi
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -45,14 +45,17 @@
 # globally
 % pipx install 'curl_arguments_url'
 # or in a particular virtual env
 % pip install 'curl_arguments_url'
 
 # to get the completions to work, add the following to your .zshrc
 eval "$(carl utils zsh-print-script)"
+
+# And copy the OpenAPI spec into ~/.carl/open_api to get the completions and curl-building working
+% cp open_api-spec.yml ~/.carl/open_api
 ```
 
 ### Examples
 
 These examples use [tests/resources/open_api/openapi-demo.yml](tests/resources/open_api/openapi-demo.yml)
 
 * Basic GET
@@ -127,15 +130,18 @@
   -h, --help            show this help message and exit
 
 Environment Variables:
     CARL_DIR: Directory which contains files for carl. Default: ~/.carl
     CARL_OPEN_API_DIR: Directory containing the OpenApi specifications and
                         Yaml files. Default: $CARL_DIR/open_api
     CARL_CACHE_DIR: Directory containing the cache. Default $CARL_DIR/cache
+```
 
+For a specific endpoint:
+```text
 % carl http://demo.io/v0/entities/\{path-item\} POST --help
 usage: carl http://demo.io/v0/entities/{path-item} POST [-h] [-p] [-n] [-R] [-b BODY_JSON] [+field-header FIELD_HEADER] [+field-one FIELD_ONE]
                                                         [+field-two FIELD_TWO [FIELD_TWO ...]] [+field-three FIELD_THREE] +path-item PATH_ITEM
                                                         [passed_to_curl ...]
 
 Demo Post Command
 
@@ -161,14 +167,16 @@
 
 * Generic Optional Args:
 
 ```text
   -p, --print-cmd       Print the resulting curl command to standard out
   -n, --no-run          Don't run the curl command. Useful with -p
   -R, --no-requires     Don't check to see if required parameter values are missing or if values are one of the enumerated values
+  -b BODY_JSON, --body-json BODY_JSON, --body BODY_JSON
+                        Base json object to send in the body. Required body params are still required unless -R option passed. Useful for dealing with incomplete specs.
 ```
 
 * Relevant Environment Variables
 
 ```text
     CARL_DIR: Directory which contains files for carl. Default: ~/.carl
     CARL_OPEN_API_DIR: Directory containing the OpenApi specifications and
@@ -205,11 +213,15 @@
 * Support file uploading and downloading
 * Utilize the authorization part of the OpenAPI spec
 * Better support for nested json objects in the body, so that `+param.sub-param value` would set
     `{"param"{"sub-param":"value"}}`
 * Maybe support older versions of Swagger/OpenApi
 * Speaking of which, in the code I sometimes use the term "swagger" and sometimes "open_api".  I should make this
     consistent.
+* Support bash and fish.  With how I implemented this, I thought it would be easy to implement bash.  But the way bash
+    parses and escapes arguments passed to the completion function made it surprisingly challenging.  The
+    `bash-completion` branch has my so-far attempts to deal with these issues.  It might be close to done, or there
+    might be a slew of other issues I haven't realized yet.
 
 ## Credits
 
 This package was created with _cookiecutter_ and the `audreyr/cookiecutter-pypackage` project template.
```

### Comparing `curl_arguments_url-0.1.1/setup.py` & `curl_arguments_url-0.1.2/setup.py`

 * *Files identical despite different names*

