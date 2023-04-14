# Comparing `tmp/butterneck-projen-0.0.5.tar.gz` & `tmp/butterneck-projen-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butterneck-projen-0.0.5.tar", last modified: Fri Apr 14 18:27:53 2023, max compression
+gzip compressed data, was "butterneck-projen-0.0.6.tar", last modified: Fri Apr 14 20:03:32 2023, max compression
```

## Comparing `butterneck-projen-0.0.5.tar` & `butterneck-projen-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/src/butterneck_projen/
--rw-r--r--   0 runner    (1001) docker     (123)   113414 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/src/butterneck_projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/src/butterneck_projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/src/butterneck_projen/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23821 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/src/butterneck_projen/_jsii/butterneck-projen@0.0.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/src/butterneck_projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/src/butterneck_projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 18:27:53.000000 butterneck-projen-0.0.5/src/butterneck_projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-14 18:27:53.000000 butterneck-projen-0.0.5/src/butterneck_projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:27:53.000000 butterneck-projen-0.0.5/src/butterneck_projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 18:27:53.000000 butterneck-projen-0.0.5/src/butterneck_projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 18:27:53.000000 butterneck-projen-0.0.5/src/butterneck_projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/src/butterneck_projen/
+-rw-r--r--   0 runner    (1001) docker     (123)   113875 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/src/butterneck_projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/src/butterneck_projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/src/butterneck_projen/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24227 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/src/butterneck_projen/_jsii/butterneck-projen@0.0.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/src/butterneck_projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/src/butterneck_projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 20:03:32.000000 butterneck-projen-0.0.6/src/butterneck_projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-14 20:03:32.000000 butterneck-projen-0.0.6/src/butterneck_projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:03:32.000000 butterneck-projen-0.0.6/src/butterneck_projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 20:03:32.000000 butterneck-projen-0.0.6/src/butterneck_projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 20:03:32.000000 butterneck-projen-0.0.6/src/butterneck_projen.egg-info/top_level.txt
```

### Comparing `butterneck-projen-0.0.5/LICENSE` & `butterneck-projen-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `butterneck-projen-0.0.5/PKG-INFO` & `butterneck-projen-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butterneck-projen
-Version: 0.0.5
+Version: 0.0.6
 Summary: butterneck-projen
 Home-page: https://github.com/butterneck/butterneck-projen.git
 Author: Filippo Pinton<pinton.filippo@protonmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/butterneck/butterneck-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `butterneck-projen-0.0.5/setup.py` & `butterneck-projen-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "butterneck-projen",
-    "version": "0.0.5",
+    "version": "0.0.6",
     "description": "butterneck-projen",
     "license": "Apache-2.0",
     "url": "https://github.com/butterneck/butterneck-projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Filippo Pinton<pinton.filippo@protonmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "butterneck_projen",
         "butterneck_projen._jsii"
     ],
     "package_data": {
         "butterneck_projen._jsii": [
-            "butterneck-projen@0.0.5.jsii.tgz"
+            "butterneck-projen@0.0.6.jsii.tgz"
         ],
         "butterneck_projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `butterneck-projen-0.0.5/src/butterneck_projen/__init__.py` & `butterneck-projen-0.0.6/src/butterneck_projen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 
 
 class ButterneckAwsCdkPythonApp(
     _projen_awscdk_04054675.AwsCdkPythonApp,
     metaclass=jsii.JSIIMeta,
     jsii_type="butterneck-projen.ButterneckAwsCdkPythonApp",
 ):
+    '''
+    :class: ButterneckAwsCdkPythonApp
+    :export: true
+    :extends: AwsCdkPythonApp *
+    :pjid: awscdk-app-py
+    '''
+
     def __init__(
         self,
         *,
         author_email: typing.Optional[builtins.str] = None,
         author_name: typing.Optional[builtins.str] = None,
         cdk_version: typing.Optional[builtins.str] = None,
         constructs_version: typing.Optional[builtins.str] = None,
@@ -270,15 +277,16 @@
         cdk_version: typing.Optional[builtins.str] = None,
         constructs_version: typing.Optional[builtins.str] = None,
         deps: typing.Optional[typing.Sequence[builtins.str]] = None,
         dev_deps: typing.Optional[typing.Sequence[builtins.str]] = None,
         module_name: typing.Optional[builtins.str] = None,
         version: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
+        '''TODO.
+
         :param name: (experimental) This is the name of your project. Default: $BASEDIR
         :param commit_generated: (experimental) Whether to commit the managed files by default. Default: true
         :param git_ignore_options: (experimental) Configuration options for .gitignore file.
         :param git_options: (experimental) Configuration options for git.
         :param logging: (experimental) Configure logging options such as verbosity. Default: {}
         :param outdir: (experimental) The root directory of the project. Relative to this directory, all files are synthesized. If this project has a parent, this directory is relative to the parent directory and it cannot be the same as the parent or any of it's other sub-projects. Default: "."
         :param parent: (experimental) The parent project, if this project is part of a bigger project.
@@ -315,14 +323,18 @@
         :param author_name: Author's name. Default: "Filippo Pinton"
         :param cdk_version: Minimum version of the AWS CDK to depend on. Default: "2.74.0"
         :param constructs_version: Minimum version of the ``constructs`` library to depend on. Default: "10.0.5".
         :param deps: List of runtime dependencies for this project. Dependencies use the format: ``<module>@<semver>`` Additional dependencies can be added via ``project.addDependency()``. Default: "[ 'butterneck-cdk-constructs' ]"
         :param dev_deps: List of dev dependencies for this project. Dependencies use the format: ``<module>@<semver>`` Additional dependencies can be added via ``project.addDevDependency()``. Default: []
         :param module_name: Name of the python package as used in imports and filenames. Must only consist of alphanumeric characters and underscores. Default: ""
         :param version: Version of the package. Default: "0.0.0"
+
+        :export: true
+        :extends: CdkConfigCommonOptions
+        :interface: ButterneckAwsCdkPythonAppOptions
         '''
         if isinstance(git_ignore_options, dict):
             git_ignore_options = _projen_04054675.IgnoreFileOptions(**git_ignore_options)
         if isinstance(git_options, dict):
             git_options = _projen_04054675.GitOptions(**git_options)
         if isinstance(logging, dict):
             logging = _projen_04054675.LoggerOptions(**logging)
@@ -1753,14 +1765,22 @@
 
 
 class GoProject(
     _projen_04054675.Project,
     metaclass=jsii.JSIIMeta,
     jsii_type="butterneck-projen.GoProject",
 ):
+    '''TODO.
+
+    :class: GoProject
+    :export: true
+    :extends: Project *
+    :pjid: go-project
+    '''
+
     def __init__(
         self,
         *,
         name: builtins.str,
         commit_generated: typing.Optional[builtins.bool] = None,
         git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -1836,27 +1856,32 @@
         parent: typing.Optional[_projen_04054675.Project] = None,
         projen_command: typing.Optional[builtins.str] = None,
         projenrc_json: typing.Optional[builtins.bool] = None,
         projenrc_json_options: typing.Optional[typing.Union[_projen_04054675.ProjenrcJsonOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         renovatebot: typing.Optional[builtins.bool] = None,
         renovatebot_options: typing.Optional[typing.Union[_projen_04054675.RenovatebotOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
-        '''
+        '''TODO.
+
         :param name: (experimental) This is the name of your project. Default: $BASEDIR
         :param commit_generated: (experimental) Whether to commit the managed files by default. Default: true
         :param git_ignore_options: (experimental) Configuration options for .gitignore file.
         :param git_options: (experimental) Configuration options for git.
         :param logging: (experimental) Configure logging options such as verbosity. Default: {}
         :param outdir: (experimental) The root directory of the project. Relative to this directory, all files are synthesized. If this project has a parent, this directory is relative to the parent directory and it cannot be the same as the parent or any of it's other sub-projects. Default: "."
         :param parent: (experimental) The parent project, if this project is part of a bigger project.
         :param projen_command: (experimental) The shell command to use in order to run the projen CLI. Can be used to customize in special environments. Default: "npx projen"
         :param projenrc_json: (experimental) Generate (once) .projenrc.json (in JSON). Set to ``false`` in order to disable .projenrc.json generation. Default: false
         :param projenrc_json_options: (experimental) Options for .projenrc.json. Default: - default options
         :param renovatebot: (experimental) Use renovatebot to handle dependency upgrades. Default: false
         :param renovatebot_options: (experimental) Options for renovatebot. Default: - default options
+
+        :export: true
+        :extends: ProjectOptions
+        :interface: GoProjectOptions
         '''
         if isinstance(git_ignore_options, dict):
             git_ignore_options = _projen_04054675.IgnoreFileOptions(**git_ignore_options)
         if isinstance(git_options, dict):
             git_options = _projen_04054675.GitOptions(**git_options)
         if isinstance(logging, dict):
             logging = _projen_04054675.LoggerOptions(**logging)
```

### Comparing `butterneck-projen-0.0.5/src/butterneck_projen.egg-info/PKG-INFO` & `butterneck-projen-0.0.6/src/butterneck_projen.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butterneck-projen
-Version: 0.0.5
+Version: 0.0.6
 Summary: butterneck-projen
 Home-page: https://github.com/butterneck/butterneck-projen.git
 Author: Filippo Pinton<pinton.filippo@protonmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/butterneck/butterneck-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

