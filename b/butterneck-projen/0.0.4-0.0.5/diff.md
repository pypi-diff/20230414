# Comparing `tmp/butterneck-projen-0.0.4.tar.gz` & `tmp/butterneck-projen-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butterneck-projen-0.0.4.tar", last modified: Fri Apr 14 11:08:48 2023, max compression
+gzip compressed data, was "butterneck-projen-0.0.5.tar", last modified: Fri Apr 14 18:27:53 2023, max compression
```

## Comparing `butterneck-projen-0.0.4.tar` & `butterneck-projen-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:08:48.933396 butterneck-projen-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 11:08:37.000000 butterneck-projen-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 11:08:37.000000 butterneck-projen-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 11:08:48.933396 butterneck-projen-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 11:08:37.000000 butterneck-projen-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 11:08:37.000000 butterneck-projen-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 11:08:48.933396 butterneck-projen-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-14 11:08:37.000000 butterneck-projen-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:08:48.933396 butterneck-projen-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:08:48.933396 butterneck-projen-0.0.4/src/butterneck_projen/
--rw-r--r--   0 runner    (1001) docker     (123)    94607 2023-04-14 11:08:37.000000 butterneck-projen-0.0.4/src/butterneck_projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:08:48.933396 butterneck-projen-0.0.4/src/butterneck_projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-14 11:08:37.000000 butterneck-projen-0.0.4/src/butterneck_projen/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18137 2023-04-14 11:08:37.000000 butterneck-projen-0.0.4/src/butterneck_projen/_jsii/butterneck-projen@0.0.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:08:37.000000 butterneck-projen-0.0.4/src/butterneck_projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:08:48.933396 butterneck-projen-0.0.4/src/butterneck_projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 11:08:48.000000 butterneck-projen-0.0.4/src/butterneck_projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-14 11:08:48.000000 butterneck-projen-0.0.4/src/butterneck_projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:08:48.000000 butterneck-projen-0.0.4/src/butterneck_projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 11:08:48.000000 butterneck-projen-0.0.4/src/butterneck_projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 11:08:48.000000 butterneck-projen-0.0.4/src/butterneck_projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/src/butterneck_projen/
+-rw-r--r--   0 runner    (1001) docker     (123)   113414 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/src/butterneck_projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/src/butterneck_projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/src/butterneck_projen/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23821 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/src/butterneck_projen/_jsii/butterneck-projen@0.0.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:27:38.000000 butterneck-projen-0.0.5/src/butterneck_projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:27:53.094009 butterneck-projen-0.0.5/src/butterneck_projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 18:27:53.000000 butterneck-projen-0.0.5/src/butterneck_projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-14 18:27:53.000000 butterneck-projen-0.0.5/src/butterneck_projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:27:53.000000 butterneck-projen-0.0.5/src/butterneck_projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 18:27:53.000000 butterneck-projen-0.0.5/src/butterneck_projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 18:27:53.000000 butterneck-projen-0.0.5/src/butterneck_projen.egg-info/top_level.txt
```

### Comparing `butterneck-projen-0.0.4/LICENSE` & `butterneck-projen-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `butterneck-projen-0.0.4/PKG-INFO` & `butterneck-projen-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butterneck-projen
-Version: 0.0.4
+Version: 0.0.5
 Summary: butterneck-projen
 Home-page: https://github.com/butterneck/butterneck-projen.git
 Author: Filippo Pinton<pinton.filippo@protonmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/butterneck/butterneck-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `butterneck-projen-0.0.4/setup.py` & `butterneck-projen-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "butterneck-projen",
-    "version": "0.0.4",
+    "version": "0.0.5",
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
-            "butterneck-projen@0.0.4.jsii.tgz"
+            "butterneck-projen@0.0.5.jsii.tgz"
         ],
         "butterneck_projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `butterneck-projen-0.0.4/src/butterneck_projen/__init__.py` & `butterneck-projen-0.0.5/src/butterneck_projen/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,69 +14,32 @@
 from typeguard import check_type
 
 from ._jsii import *
 
 import projen as _projen_04054675
 import projen.awscdk as _projen_awscdk_04054675
 import projen.github as _projen_github_04054675
-import projen.javascript as _projen_javascript_04054675
-import projen.python as _projen_python_04054675
-import projen.typescript as _projen_typescript_04054675
 
 
-class GoApp(
+class ButterneckAwsCdkPythonApp(
     _projen_awscdk_04054675.AwsCdkPythonApp,
     metaclass=jsii.JSIIMeta,
-    jsii_type="butterneck-projen.GoApp",
+    jsii_type="butterneck-projen.ButterneckAwsCdkPythonApp",
 ):
-    '''GoApp Project.
-
-    :class: GoApp
-    :export: true
-    :extends: awscdk.AwsCdkPythonApp *
-    :pjid: go-app
-    '''
-
     def __init__(
         self,
         *,
-        app_entrypoint: typing.Optional[builtins.str] = None,
-        testdir: typing.Optional[builtins.str] = None,
-        module_name: builtins.str,
+        author_email: typing.Optional[builtins.str] = None,
+        author_name: typing.Optional[builtins.str] = None,
+        cdk_version: typing.Optional[builtins.str] = None,
+        constructs_version: typing.Optional[builtins.str] = None,
         deps: typing.Optional[typing.Sequence[builtins.str]] = None,
         dev_deps: typing.Optional[typing.Sequence[builtins.str]] = None,
-        pip: typing.Optional[builtins.bool] = None,
-        poetry: typing.Optional[builtins.bool] = None,
-        projenrc_js: typing.Optional[builtins.bool] = None,
-        projenrc_js_options: typing.Optional[typing.Union[_projen_javascript_04054675.ProjenrcOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        projenrc_python: typing.Optional[builtins.bool] = None,
-        projenrc_python_options: typing.Optional[typing.Union[_projen_python_04054675.ProjenrcOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        projenrc_ts: typing.Optional[builtins.bool] = None,
-        projenrc_ts_options: typing.Optional[typing.Union[_projen_typescript_04054675.ProjenrcTsOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        pytest: typing.Optional[builtins.bool] = None,
-        pytest_options: typing.Optional[typing.Union[_projen_python_04054675.PytestOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        sample: typing.Optional[builtins.bool] = None,
-        setuptools: typing.Optional[builtins.bool] = None,
-        venv: typing.Optional[builtins.bool] = None,
-        venv_options: typing.Optional[typing.Union[_projen_python_04054675.VenvOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        build_command: typing.Optional[builtins.str] = None,
-        cdkout: typing.Optional[builtins.str] = None,
-        context: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
-        feature_flags: typing.Optional[builtins.bool] = None,
-        require_approval: typing.Optional[_projen_awscdk_04054675.ApprovalLevel] = None,
-        watch_excludes: typing.Optional[typing.Sequence[builtins.str]] = None,
-        watch_includes: typing.Optional[typing.Sequence[builtins.str]] = None,
-        cdk_version: builtins.str,
-        cdk_assert: typing.Optional[builtins.bool] = None,
-        cdk_assertions: typing.Optional[builtins.bool] = None,
-        cdk_dependencies: typing.Optional[typing.Sequence[builtins.str]] = None,
-        cdk_dependencies_as_deps: typing.Optional[builtins.bool] = None,
-        cdk_test_dependencies: typing.Optional[typing.Sequence[builtins.str]] = None,
-        cdk_version_pinning: typing.Optional[builtins.bool] = None,
-        constructs_version: typing.Optional[builtins.str] = None,
+        module_name: typing.Optional[builtins.str] = None,
+        version: typing.Optional[builtins.str] = None,
         auto_approve_options: typing.Optional[typing.Union[_projen_github_04054675.AutoApproveOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         auto_merge: typing.Optional[builtins.bool] = None,
         auto_merge_options: typing.Optional[typing.Union[_projen_github_04054675.AutoMergeOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         clobber: typing.Optional[builtins.bool] = None,
         dev_container: typing.Optional[builtins.bool] = None,
         github: typing.Optional[builtins.bool] = None,
         github_options: typing.Optional[typing.Union[_projen_github_04054675.GitHubOptions, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -86,72 +49,43 @@
         project_type: typing.Optional[_projen_04054675.ProjectType] = None,
         projen_credentials: typing.Optional[_projen_github_04054675.GithubCredentials] = None,
         projen_token_secret: typing.Optional[builtins.str] = None,
         readme: typing.Optional[typing.Union[_projen_04054675.SampleReadmeProps, typing.Dict[builtins.str, typing.Any]]] = None,
         stale: typing.Optional[builtins.bool] = None,
         stale_options: typing.Optional[typing.Union[_projen_github_04054675.StaleOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         vscode: typing.Optional[builtins.bool] = None,
-        author_email: builtins.str,
-        author_name: builtins.str,
-        version: builtins.str,
-        classifiers: typing.Optional[typing.Sequence[builtins.str]] = None,
-        description: typing.Optional[builtins.str] = None,
-        homepage: typing.Optional[builtins.str] = None,
-        license: typing.Optional[builtins.str] = None,
-        package_name: typing.Optional[builtins.str] = None,
-        poetry_options: typing.Optional[typing.Union[_projen_python_04054675.PoetryPyprojectOptionsWithoutDeps, typing.Dict[builtins.str, typing.Any]]] = None,
-        setup_config: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+        build_command: typing.Optional[builtins.str] = None,
+        cdkout: typing.Optional[builtins.str] = None,
+        context: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+        feature_flags: typing.Optional[builtins.bool] = None,
+        require_approval: typing.Optional[_projen_awscdk_04054675.ApprovalLevel] = None,
+        watch_excludes: typing.Optional[typing.Sequence[builtins.str]] = None,
+        watch_includes: typing.Optional[typing.Sequence[builtins.str]] = None,
         name: builtins.str,
         commit_generated: typing.Optional[builtins.bool] = None,
         git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         logging: typing.Optional[typing.Union[_projen_04054675.LoggerOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         outdir: typing.Optional[builtins.str] = None,
         parent: typing.Optional[_projen_04054675.Project] = None,
         projen_command: typing.Optional[builtins.str] = None,
         projenrc_json: typing.Optional[builtins.bool] = None,
         projenrc_json_options: typing.Optional[typing.Union[_projen_04054675.ProjenrcJsonOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         renovatebot: typing.Optional[builtins.bool] = None,
         renovatebot_options: typing.Optional[typing.Union[_projen_04054675.RenovatebotOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
-        :param app_entrypoint: (experimental) The CDK app's entrypoint (relative to the source directory, which is "src" by default). Default: "app.py"
-        :param testdir: (experimental) Python sources directory. Default: "tests"
-        :param module_name: (experimental) Name of the python package as used in imports and filenames. Must only consist of alphanumeric characters and underscores. Default: $PYTHON_MODULE_NAME
-        :param deps: (experimental) List of runtime dependencies for this project. Dependencies use the format: ``<module>@<semver>`` Additional dependencies can be added via ``project.addDependency()``. Default: []
-        :param dev_deps: (experimental) List of dev dependencies for this project. Dependencies use the format: ``<module>@<semver>`` Additional dependencies can be added via ``project.addDevDependency()``. Default: []
-        :param pip: (experimental) Use pip with a requirements.txt file to track project dependencies. Default: - true, unless poetry is true, then false
-        :param poetry: (experimental) Use poetry to manage your project dependencies, virtual environment, and (optional) packaging/publishing. This feature is incompatible with pip, setuptools, or venv. If you set this option to ``true``, then pip, setuptools, and venv must be set to ``false``. Default: false
-        :param projenrc_js: (experimental) Use projenrc in javascript. This will install ``projen`` as a JavaScript dependency and add a ``synth`` task which will run ``.projenrc.js``. Default: false
-        :param projenrc_js_options: (experimental) Options related to projenrc in JavaScript. Default: - default options
-        :param projenrc_python: (experimental) Use projenrc in Python. This will install ``projen`` as a Python dependency and add a ``synth`` task which will run ``.projenrc.py``. Default: true
-        :param projenrc_python_options: (experimental) Options related to projenrc in python. Default: - default options
-        :param projenrc_ts: (experimental) Use projenrc in TypeScript. This will create a tsconfig file (default: ``tsconfig.projen.json``) and use ``ts-node`` in the default task to parse the project source files. Default: false
-        :param projenrc_ts_options: (experimental) Options related to projenrc in TypeScript. Default: - default options
-        :param pytest: (experimental) Include pytest tests. Default: true
-        :param pytest_options: (experimental) pytest options. Default: - defaults
-        :param sample: (experimental) Include sample code and test if the relevant directories don't exist. Default: true
-        :param setuptools: (experimental) Use setuptools with a setup.py script for packaging and publishing. Default: - true, unless poetry is true, then false
-        :param venv: (experimental) Use venv to manage a virtual environment for installing dependencies inside. Default: - true, unless poetry is true, then false
-        :param venv_options: (experimental) Venv options. Default: - defaults
-        :param build_command: (experimental) A command to execute before synthesis. This command will be called when running ``cdk synth`` or when ``cdk watch`` identifies a change in your source code before redeployment. Default: - no build command
-        :param cdkout: (experimental) cdk.out directory. Default: "cdk.out"
-        :param context: (experimental) Additional context to include in ``cdk.json``. Default: - no additional context
-        :param feature_flags: (experimental) Include all feature flags in cdk.json. Default: true
-        :param require_approval: (experimental) To protect you against unintended changes that affect your security posture, the AWS CDK Toolkit prompts you to approve security-related changes before deploying them. Default: ApprovalLevel.BROADENING
-        :param watch_excludes: (experimental) Glob patterns to exclude from ``cdk watch``. Default: []
-        :param watch_includes: (experimental) Glob patterns to include in ``cdk watch``. Default: []
-        :param cdk_version: (experimental) Minimum version of the AWS CDK to depend on. Default: "2.1.0"
-        :param cdk_assert: (deprecated) Warning: NodeJS only. Install the @aws-cdk/assert library? Default: - will be included by default for AWS CDK >= 1.0.0 < 2.0.0
-        :param cdk_assertions: (experimental) Install the assertions library? Only needed for CDK 1.x. If using CDK 2.x then assertions is already included in 'aws-cdk-lib' Default: - will be included by default for AWS CDK >= 1.111.0 < 2.0.0
-        :param cdk_dependencies: (deprecated) Which AWS CDKv1 modules this project requires.
-        :param cdk_dependencies_as_deps: (deprecated) If this is enabled (default), all modules declared in ``cdkDependencies`` will be also added as normal ``dependencies`` (as well as ``peerDependencies``). This is to ensure that downstream consumers actually have your CDK dependencies installed when using npm < 7 or yarn, where peer dependencies are not automatically installed. If this is disabled, ``cdkDependencies`` will be added to ``devDependencies`` to ensure they are present during development. Note: this setting only applies to construct library projects Default: true
-        :param cdk_test_dependencies: (deprecated) AWS CDK modules required for testing.
-        :param cdk_version_pinning: (experimental) Use pinned version instead of caret version for CDK. You can use this to prevent mixed versions for your CDK dependencies and to prevent auto-updates. If you use experimental features this will let you define the moment you include breaking changes.
-        :param constructs_version: (experimental) Minimum version of the ``constructs`` library to depend on. Default: - for CDK 1.x the default is "3.2.27", for CDK 2.x the default is "10.0.5".
+        :param author_email: Author's e-mail. Default: "pinton.filippo
+        :param author_name: Author's name. Default: "Filippo Pinton"
+        :param cdk_version: Minimum version of the AWS CDK to depend on. Default: "2.74.0"
+        :param constructs_version: Minimum version of the ``constructs`` library to depend on. Default: "10.0.5".
+        :param deps: List of runtime dependencies for this project. Dependencies use the format: ``<module>@<semver>`` Additional dependencies can be added via ``project.addDependency()``. Default: "[ 'butterneck-cdk-constructs' ]"
+        :param dev_deps: List of dev dependencies for this project. Dependencies use the format: ``<module>@<semver>`` Additional dependencies can be added via ``project.addDevDependency()``. Default: []
+        :param module_name: Name of the python package as used in imports and filenames. Must only consist of alphanumeric characters and underscores. Default: ""
+        :param version: Version of the package. Default: "0.0.0"
         :param auto_approve_options: (experimental) Enable and configure the 'auto approve' workflow. Default: - auto approve is disabled
         :param auto_merge: (experimental) Enable automatic merging on GitHub. Has no effect if ``github.mergify`` is set to false. Default: true
         :param auto_merge_options: (experimental) Configure options for automatic merging on GitHub. Has no effect if ``github.mergify`` or ``autoMerge`` is set to false. Default: - see defaults in ``AutoMergeOptions``
         :param clobber: (experimental) Add a ``clobber`` task which resets the repo to origin. Default: - true, but false for subprojects
         :param dev_container: (experimental) Add a VSCode development environment (used for GitHub Codespaces). Default: false
         :param github: (experimental) Enable GitHub integration. Enabled by default for root projects. Disabled for non-root projects. Default: true
         :param github_options: (experimental) Options for GitHub integration. Default: - see GitHubOptions
@@ -161,72 +95,43 @@
         :param project_type: (deprecated) Which type of project this is (library/app). Default: ProjectType.UNKNOWN
         :param projen_credentials: (experimental) Choose a method of providing GitHub API access for projen workflows. Default: - use a personal access token named PROJEN_GITHUB_TOKEN
         :param projen_token_secret: (deprecated) The name of a secret which includes a GitHub Personal Access Token to be used by projen workflows. This token needs to have the ``repo``, ``workflows`` and ``packages`` scope. Default: "PROJEN_GITHUB_TOKEN"
         :param readme: (experimental) The README setup. Default: - { filename: 'README.md', contents: '# replace this' }
         :param stale: (experimental) Auto-close of stale issues and pull request. See ``staleOptions`` for options. Default: false
         :param stale_options: (experimental) Auto-close stale issues and pull requests. To disable set ``stale`` to ``false``. Default: - see defaults in ``StaleOptions``
         :param vscode: (experimental) Enable VSCode integration. Enabled by default for root projects. Disabled for non-root projects. Default: true
-        :param author_email: (experimental) Author's e-mail. Default: $GIT_USER_EMAIL
-        :param author_name: (experimental) Author's name. Default: $GIT_USER_NAME
-        :param version: (experimental) Version of the package. Default: "0.1.0"
-        :param classifiers: (experimental) A list of PyPI trove classifiers that describe the project.
-        :param description: (experimental) A short description of the package.
-        :param homepage: (experimental) A URL to the website of the project.
-        :param license: (experimental) License of this package as an SPDX identifier.
-        :param package_name: (experimental) Package name.
-        :param poetry_options: (experimental) Additional options to set for poetry if using poetry.
-        :param setup_config: (experimental) Additional fields to pass in the setup() function if using setuptools.
+        :param build_command: (experimental) A command to execute before synthesis. This command will be called when running ``cdk synth`` or when ``cdk watch`` identifies a change in your source code before redeployment. Default: - no build command
+        :param cdkout: (experimental) cdk.out directory. Default: "cdk.out"
+        :param context: (experimental) Additional context to include in ``cdk.json``. Default: - no additional context
+        :param feature_flags: (experimental) Include all feature flags in cdk.json. Default: true
+        :param require_approval: (experimental) To protect you against unintended changes that affect your security posture, the AWS CDK Toolkit prompts you to approve security-related changes before deploying them. Default: ApprovalLevel.BROADENING
+        :param watch_excludes: (experimental) Glob patterns to exclude from ``cdk watch``. Default: []
+        :param watch_includes: (experimental) Glob patterns to include in ``cdk watch``. Default: []
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
         '''
-        options = GoAppOptions(
-            app_entrypoint=app_entrypoint,
-            testdir=testdir,
-            module_name=module_name,
-            deps=deps,
-            dev_deps=dev_deps,
-            pip=pip,
-            poetry=poetry,
-            projenrc_js=projenrc_js,
-            projenrc_js_options=projenrc_js_options,
-            projenrc_python=projenrc_python,
-            projenrc_python_options=projenrc_python_options,
-            projenrc_ts=projenrc_ts,
-            projenrc_ts_options=projenrc_ts_options,
-            pytest=pytest,
-            pytest_options=pytest_options,
-            sample=sample,
-            setuptools=setuptools,
-            venv=venv,
-            venv_options=venv_options,
-            build_command=build_command,
-            cdkout=cdkout,
-            context=context,
-            feature_flags=feature_flags,
-            require_approval=require_approval,
-            watch_excludes=watch_excludes,
-            watch_includes=watch_includes,
+        options = ButterneckAwsCdkPythonAppOptions(
+            author_email=author_email,
+            author_name=author_name,
             cdk_version=cdk_version,
-            cdk_assert=cdk_assert,
-            cdk_assertions=cdk_assertions,
-            cdk_dependencies=cdk_dependencies,
-            cdk_dependencies_as_deps=cdk_dependencies_as_deps,
-            cdk_test_dependencies=cdk_test_dependencies,
-            cdk_version_pinning=cdk_version_pinning,
             constructs_version=constructs_version,
+            deps=deps,
+            dev_deps=dev_deps,
+            module_name=module_name,
+            version=version,
             auto_approve_options=auto_approve_options,
             auto_merge=auto_merge,
             auto_merge_options=auto_merge_options,
             clobber=clobber,
             dev_container=dev_container,
             github=github,
             github_options=github_options,
@@ -236,24 +141,21 @@
             project_type=project_type,
             projen_credentials=projen_credentials,
             projen_token_secret=projen_token_secret,
             readme=readme,
             stale=stale,
             stale_options=stale_options,
             vscode=vscode,
-            author_email=author_email,
-            author_name=author_name,
-            version=version,
-            classifiers=classifiers,
-            description=description,
-            homepage=homepage,
-            license=license,
-            package_name=package_name,
-            poetry_options=poetry_options,
-            setup_config=setup_config,
+            build_command=build_command,
+            cdkout=cdkout,
+            context=context,
+            feature_flags=feature_flags,
+            require_approval=require_approval,
+            watch_excludes=watch_excludes,
+            watch_includes=watch_includes,
             name=name,
             commit_generated=commit_generated,
             git_ignore_options=git_ignore_options,
             git_options=git_options,
             logging=logging,
             outdir=outdir,
             parent=parent,
@@ -264,16 +166,19 @@
             renovatebot_options=renovatebot_options,
         )
 
         jsii.create(self.__class__, self, [options])
 
 
 @jsii.data_type(
-    jsii_type="butterneck-projen.GoAppOptions",
-    jsii_struct_bases=[_projen_awscdk_04054675.AwsCdkPythonAppOptions],
+    jsii_type="butterneck-projen.ButterneckAwsCdkPythonAppOptions",
+    jsii_struct_bases=[
+        _projen_github_04054675.GitHubProjectOptions,
+        _projen_awscdk_04054675.CdkConfigCommonOptions,
+    ],
     name_mapping={
         "name": "name",
         "commit_generated": "commitGenerated",
         "git_ignore_options": "gitIgnoreOptions",
         "git_options": "gitOptions",
         "logging": "logging",
         "outdir": "outdir",
@@ -296,61 +201,35 @@
         "project_type": "projectType",
         "projen_credentials": "projenCredentials",
         "projen_token_secret": "projenTokenSecret",
         "readme": "readme",
         "stale": "stale",
         "stale_options": "staleOptions",
         "vscode": "vscode",
-        "author_email": "authorEmail",
-        "author_name": "authorName",
-        "version": "version",
-        "classifiers": "classifiers",
-        "description": "description",
-        "homepage": "homepage",
-        "license": "license",
-        "package_name": "packageName",
-        "poetry_options": "poetryOptions",
-        "setup_config": "setupConfig",
-        "module_name": "moduleName",
-        "deps": "deps",
-        "dev_deps": "devDeps",
-        "pip": "pip",
-        "poetry": "poetry",
-        "projenrc_js": "projenrcJs",
-        "projenrc_js_options": "projenrcJsOptions",
-        "projenrc_python": "projenrcPython",
-        "projenrc_python_options": "projenrcPythonOptions",
-        "projenrc_ts": "projenrcTs",
-        "projenrc_ts_options": "projenrcTsOptions",
-        "pytest": "pytest",
-        "pytest_options": "pytestOptions",
-        "sample": "sample",
-        "setuptools": "setuptools",
-        "venv": "venv",
-        "venv_options": "venvOptions",
         "build_command": "buildCommand",
         "cdkout": "cdkout",
         "context": "context",
         "feature_flags": "featureFlags",
         "require_approval": "requireApproval",
         "watch_excludes": "watchExcludes",
         "watch_includes": "watchIncludes",
+        "author_email": "authorEmail",
+        "author_name": "authorName",
         "cdk_version": "cdkVersion",
-        "cdk_assert": "cdkAssert",
-        "cdk_assertions": "cdkAssertions",
-        "cdk_dependencies": "cdkDependencies",
-        "cdk_dependencies_as_deps": "cdkDependenciesAsDeps",
-        "cdk_test_dependencies": "cdkTestDependencies",
-        "cdk_version_pinning": "cdkVersionPinning",
         "constructs_version": "constructsVersion",
-        "app_entrypoint": "appEntrypoint",
-        "testdir": "testdir",
+        "deps": "deps",
+        "dev_deps": "devDeps",
+        "module_name": "moduleName",
+        "version": "version",
     },
 )
-class GoAppOptions(_projen_awscdk_04054675.AwsCdkPythonAppOptions):
+class ButterneckAwsCdkPythonAppOptions(
+    _projen_github_04054675.GitHubProjectOptions,
+    _projen_awscdk_04054675.CdkConfigCommonOptions,
+):
     def __init__(
         self,
         *,
         name: builtins.str,
         commit_generated: typing.Optional[builtins.bool] = None,
         git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -375,58 +254,29 @@
         project_type: typing.Optional[_projen_04054675.ProjectType] = None,
         projen_credentials: typing.Optional[_projen_github_04054675.GithubCredentials] = None,
         projen_token_secret: typing.Optional[builtins.str] = None,
         readme: typing.Optional[typing.Union[_projen_04054675.SampleReadmeProps, typing.Dict[builtins.str, typing.Any]]] = None,
         stale: typing.Optional[builtins.bool] = None,
         stale_options: typing.Optional[typing.Union[_projen_github_04054675.StaleOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         vscode: typing.Optional[builtins.bool] = None,
-        author_email: builtins.str,
-        author_name: builtins.str,
-        version: builtins.str,
-        classifiers: typing.Optional[typing.Sequence[builtins.str]] = None,
-        description: typing.Optional[builtins.str] = None,
-        homepage: typing.Optional[builtins.str] = None,
-        license: typing.Optional[builtins.str] = None,
-        package_name: typing.Optional[builtins.str] = None,
-        poetry_options: typing.Optional[typing.Union[_projen_python_04054675.PoetryPyprojectOptionsWithoutDeps, typing.Dict[builtins.str, typing.Any]]] = None,
-        setup_config: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
-        module_name: builtins.str,
-        deps: typing.Optional[typing.Sequence[builtins.str]] = None,
-        dev_deps: typing.Optional[typing.Sequence[builtins.str]] = None,
-        pip: typing.Optional[builtins.bool] = None,
-        poetry: typing.Optional[builtins.bool] = None,
-        projenrc_js: typing.Optional[builtins.bool] = None,
-        projenrc_js_options: typing.Optional[typing.Union[_projen_javascript_04054675.ProjenrcOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        projenrc_python: typing.Optional[builtins.bool] = None,
-        projenrc_python_options: typing.Optional[typing.Union[_projen_python_04054675.ProjenrcOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        projenrc_ts: typing.Optional[builtins.bool] = None,
-        projenrc_ts_options: typing.Optional[typing.Union[_projen_typescript_04054675.ProjenrcTsOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        pytest: typing.Optional[builtins.bool] = None,
-        pytest_options: typing.Optional[typing.Union[_projen_python_04054675.PytestOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-        sample: typing.Optional[builtins.bool] = None,
-        setuptools: typing.Optional[builtins.bool] = None,
-        venv: typing.Optional[builtins.bool] = None,
-        venv_options: typing.Optional[typing.Union[_projen_python_04054675.VenvOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         build_command: typing.Optional[builtins.str] = None,
         cdkout: typing.Optional[builtins.str] = None,
         context: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         feature_flags: typing.Optional[builtins.bool] = None,
         require_approval: typing.Optional[_projen_awscdk_04054675.ApprovalLevel] = None,
         watch_excludes: typing.Optional[typing.Sequence[builtins.str]] = None,
         watch_includes: typing.Optional[typing.Sequence[builtins.str]] = None,
-        cdk_version: builtins.str,
-        cdk_assert: typing.Optional[builtins.bool] = None,
-        cdk_assertions: typing.Optional[builtins.bool] = None,
-        cdk_dependencies: typing.Optional[typing.Sequence[builtins.str]] = None,
-        cdk_dependencies_as_deps: typing.Optional[builtins.bool] = None,
-        cdk_test_dependencies: typing.Optional[typing.Sequence[builtins.str]] = None,
-        cdk_version_pinning: typing.Optional[builtins.bool] = None,
+        author_email: typing.Optional[builtins.str] = None,
+        author_name: typing.Optional[builtins.str] = None,
+        cdk_version: typing.Optional[builtins.str] = None,
         constructs_version: typing.Optional[builtins.str] = None,
-        app_entrypoint: typing.Optional[builtins.str] = None,
-        testdir: typing.Optional[builtins.str] = None,
+        deps: typing.Optional[typing.Sequence[builtins.str]] = None,
+        dev_deps: typing.Optional[typing.Sequence[builtins.str]] = None,
+        module_name: typing.Optional[builtins.str] = None,
+        version: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param name: (experimental) This is the name of your project. Default: $BASEDIR
         :param commit_generated: (experimental) Whether to commit the managed files by default. Default: true
         :param git_ignore_options: (experimental) Configuration options for .gitignore file.
         :param git_options: (experimental) Configuration options for git.
         :param logging: (experimental) Configure logging options such as verbosity. Default: {}
@@ -450,58 +300,29 @@
         :param project_type: (deprecated) Which type of project this is (library/app). Default: ProjectType.UNKNOWN
         :param projen_credentials: (experimental) Choose a method of providing GitHub API access for projen workflows. Default: - use a personal access token named PROJEN_GITHUB_TOKEN
         :param projen_token_secret: (deprecated) The name of a secret which includes a GitHub Personal Access Token to be used by projen workflows. This token needs to have the ``repo``, ``workflows`` and ``packages`` scope. Default: "PROJEN_GITHUB_TOKEN"
         :param readme: (experimental) The README setup. Default: - { filename: 'README.md', contents: '# replace this' }
         :param stale: (experimental) Auto-close of stale issues and pull request. See ``staleOptions`` for options. Default: false
         :param stale_options: (experimental) Auto-close stale issues and pull requests. To disable set ``stale`` to ``false``. Default: - see defaults in ``StaleOptions``
         :param vscode: (experimental) Enable VSCode integration. Enabled by default for root projects. Disabled for non-root projects. Default: true
-        :param author_email: (experimental) Author's e-mail. Default: $GIT_USER_EMAIL
-        :param author_name: (experimental) Author's name. Default: $GIT_USER_NAME
-        :param version: (experimental) Version of the package. Default: "0.1.0"
-        :param classifiers: (experimental) A list of PyPI trove classifiers that describe the project.
-        :param description: (experimental) A short description of the package.
-        :param homepage: (experimental) A URL to the website of the project.
-        :param license: (experimental) License of this package as an SPDX identifier.
-        :param package_name: (experimental) Package name.
-        :param poetry_options: (experimental) Additional options to set for poetry if using poetry.
-        :param setup_config: (experimental) Additional fields to pass in the setup() function if using setuptools.
-        :param module_name: (experimental) Name of the python package as used in imports and filenames. Must only consist of alphanumeric characters and underscores. Default: $PYTHON_MODULE_NAME
-        :param deps: (experimental) List of runtime dependencies for this project. Dependencies use the format: ``<module>@<semver>`` Additional dependencies can be added via ``project.addDependency()``. Default: []
-        :param dev_deps: (experimental) List of dev dependencies for this project. Dependencies use the format: ``<module>@<semver>`` Additional dependencies can be added via ``project.addDevDependency()``. Default: []
-        :param pip: (experimental) Use pip with a requirements.txt file to track project dependencies. Default: - true, unless poetry is true, then false
-        :param poetry: (experimental) Use poetry to manage your project dependencies, virtual environment, and (optional) packaging/publishing. This feature is incompatible with pip, setuptools, or venv. If you set this option to ``true``, then pip, setuptools, and venv must be set to ``false``. Default: false
-        :param projenrc_js: (experimental) Use projenrc in javascript. This will install ``projen`` as a JavaScript dependency and add a ``synth`` task which will run ``.projenrc.js``. Default: false
-        :param projenrc_js_options: (experimental) Options related to projenrc in JavaScript. Default: - default options
-        :param projenrc_python: (experimental) Use projenrc in Python. This will install ``projen`` as a Python dependency and add a ``synth`` task which will run ``.projenrc.py``. Default: true
-        :param projenrc_python_options: (experimental) Options related to projenrc in python. Default: - default options
-        :param projenrc_ts: (experimental) Use projenrc in TypeScript. This will create a tsconfig file (default: ``tsconfig.projen.json``) and use ``ts-node`` in the default task to parse the project source files. Default: false
-        :param projenrc_ts_options: (experimental) Options related to projenrc in TypeScript. Default: - default options
-        :param pytest: (experimental) Include pytest tests. Default: true
-        :param pytest_options: (experimental) pytest options. Default: - defaults
-        :param sample: (experimental) Include sample code and test if the relevant directories don't exist. Default: true
-        :param setuptools: (experimental) Use setuptools with a setup.py script for packaging and publishing. Default: - true, unless poetry is true, then false
-        :param venv: (experimental) Use venv to manage a virtual environment for installing dependencies inside. Default: - true, unless poetry is true, then false
-        :param venv_options: (experimental) Venv options. Default: - defaults
         :param build_command: (experimental) A command to execute before synthesis. This command will be called when running ``cdk synth`` or when ``cdk watch`` identifies a change in your source code before redeployment. Default: - no build command
         :param cdkout: (experimental) cdk.out directory. Default: "cdk.out"
         :param context: (experimental) Additional context to include in ``cdk.json``. Default: - no additional context
         :param feature_flags: (experimental) Include all feature flags in cdk.json. Default: true
         :param require_approval: (experimental) To protect you against unintended changes that affect your security posture, the AWS CDK Toolkit prompts you to approve security-related changes before deploying them. Default: ApprovalLevel.BROADENING
         :param watch_excludes: (experimental) Glob patterns to exclude from ``cdk watch``. Default: []
         :param watch_includes: (experimental) Glob patterns to include in ``cdk watch``. Default: []
-        :param cdk_version: (experimental) Minimum version of the AWS CDK to depend on. Default: "2.1.0"
-        :param cdk_assert: (deprecated) Warning: NodeJS only. Install the @aws-cdk/assert library? Default: - will be included by default for AWS CDK >= 1.0.0 < 2.0.0
-        :param cdk_assertions: (experimental) Install the assertions library? Only needed for CDK 1.x. If using CDK 2.x then assertions is already included in 'aws-cdk-lib' Default: - will be included by default for AWS CDK >= 1.111.0 < 2.0.0
-        :param cdk_dependencies: (deprecated) Which AWS CDKv1 modules this project requires.
-        :param cdk_dependencies_as_deps: (deprecated) If this is enabled (default), all modules declared in ``cdkDependencies`` will be also added as normal ``dependencies`` (as well as ``peerDependencies``). This is to ensure that downstream consumers actually have your CDK dependencies installed when using npm < 7 or yarn, where peer dependencies are not automatically installed. If this is disabled, ``cdkDependencies`` will be added to ``devDependencies`` to ensure they are present during development. Note: this setting only applies to construct library projects Default: true
-        :param cdk_test_dependencies: (deprecated) AWS CDK modules required for testing.
-        :param cdk_version_pinning: (experimental) Use pinned version instead of caret version for CDK. You can use this to prevent mixed versions for your CDK dependencies and to prevent auto-updates. If you use experimental features this will let you define the moment you include breaking changes.
-        :param constructs_version: (experimental) Minimum version of the ``constructs`` library to depend on. Default: - for CDK 1.x the default is "3.2.27", for CDK 2.x the default is "10.0.5".
-        :param app_entrypoint: (experimental) The CDK app's entrypoint (relative to the source directory, which is "src" by default). Default: "app.py"
-        :param testdir: (experimental) Python sources directory. Default: "tests"
+        :param author_email: Author's e-mail. Default: "pinton.filippo
+        :param author_name: Author's name. Default: "Filippo Pinton"
+        :param cdk_version: Minimum version of the AWS CDK to depend on. Default: "2.74.0"
+        :param constructs_version: Minimum version of the ``constructs`` library to depend on. Default: "10.0.5".
+        :param deps: List of runtime dependencies for this project. Dependencies use the format: ``<module>@<semver>`` Additional dependencies can be added via ``project.addDependency()``. Default: "[ 'butterneck-cdk-constructs' ]"
+        :param dev_deps: List of dev dependencies for this project. Dependencies use the format: ``<module>@<semver>`` Additional dependencies can be added via ``project.addDevDependency()``. Default: []
+        :param module_name: Name of the python package as used in imports and filenames. Must only consist of alphanumeric characters and underscores. Default: ""
+        :param version: Version of the package. Default: "0.0.0"
         '''
         if isinstance(git_ignore_options, dict):
             git_ignore_options = _projen_04054675.IgnoreFileOptions(**git_ignore_options)
         if isinstance(git_options, dict):
             git_options = _projen_04054675.GitOptions(**git_options)
         if isinstance(logging, dict):
             logging = _projen_04054675.LoggerOptions(**logging)
@@ -517,28 +338,16 @@
             github_options = _projen_github_04054675.GitHubOptions(**github_options)
         if isinstance(mergify_options, dict):
             mergify_options = _projen_github_04054675.MergifyOptions(**mergify_options)
         if isinstance(readme, dict):
             readme = _projen_04054675.SampleReadmeProps(**readme)
         if isinstance(stale_options, dict):
             stale_options = _projen_github_04054675.StaleOptions(**stale_options)
-        if isinstance(poetry_options, dict):
-            poetry_options = _projen_python_04054675.PoetryPyprojectOptionsWithoutDeps(**poetry_options)
-        if isinstance(projenrc_js_options, dict):
-            projenrc_js_options = _projen_javascript_04054675.ProjenrcOptions(**projenrc_js_options)
-        if isinstance(projenrc_python_options, dict):
-            projenrc_python_options = _projen_python_04054675.ProjenrcOptions(**projenrc_python_options)
-        if isinstance(projenrc_ts_options, dict):
-            projenrc_ts_options = _projen_typescript_04054675.ProjenrcTsOptions(**projenrc_ts_options)
-        if isinstance(pytest_options, dict):
-            pytest_options = _projen_python_04054675.PytestOptions(**pytest_options)
-        if isinstance(venv_options, dict):
-            venv_options = _projen_python_04054675.VenvOptions(**venv_options)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e7cdfb665920a033d76499e282ce137ada7759e9a66b20380e8aae21552e8eb6)
+            type_hints = typing.get_type_hints(_typecheckingstub__28b6701892490b47b0967137d9b99f87f1f16c1b4caa7d15fdcda3eb0e7ac579)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument commit_generated", value=commit_generated, expected_type=type_hints["commit_generated"])
             check_type(argname="argument git_ignore_options", value=git_ignore_options, expected_type=type_hints["git_ignore_options"])
             check_type(argname="argument git_options", value=git_options, expected_type=type_hints["git_options"])
             check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
             check_type(argname="argument outdir", value=outdir, expected_type=type_hints["outdir"])
             check_type(argname="argument parent", value=parent, expected_type=type_hints["parent"])
@@ -560,65 +369,31 @@
             check_type(argname="argument project_type", value=project_type, expected_type=type_hints["project_type"])
             check_type(argname="argument projen_credentials", value=projen_credentials, expected_type=type_hints["projen_credentials"])
             check_type(argname="argument projen_token_secret", value=projen_token_secret, expected_type=type_hints["projen_token_secret"])
             check_type(argname="argument readme", value=readme, expected_type=type_hints["readme"])
             check_type(argname="argument stale", value=stale, expected_type=type_hints["stale"])
             check_type(argname="argument stale_options", value=stale_options, expected_type=type_hints["stale_options"])
             check_type(argname="argument vscode", value=vscode, expected_type=type_hints["vscode"])
-            check_type(argname="argument author_email", value=author_email, expected_type=type_hints["author_email"])
-            check_type(argname="argument author_name", value=author_name, expected_type=type_hints["author_name"])
-            check_type(argname="argument version", value=version, expected_type=type_hints["version"])
-            check_type(argname="argument classifiers", value=classifiers, expected_type=type_hints["classifiers"])
-            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
-            check_type(argname="argument homepage", value=homepage, expected_type=type_hints["homepage"])
-            check_type(argname="argument license", value=license, expected_type=type_hints["license"])
-            check_type(argname="argument package_name", value=package_name, expected_type=type_hints["package_name"])
-            check_type(argname="argument poetry_options", value=poetry_options, expected_type=type_hints["poetry_options"])
-            check_type(argname="argument setup_config", value=setup_config, expected_type=type_hints["setup_config"])
-            check_type(argname="argument module_name", value=module_name, expected_type=type_hints["module_name"])
-            check_type(argname="argument deps", value=deps, expected_type=type_hints["deps"])
-            check_type(argname="argument dev_deps", value=dev_deps, expected_type=type_hints["dev_deps"])
-            check_type(argname="argument pip", value=pip, expected_type=type_hints["pip"])
-            check_type(argname="argument poetry", value=poetry, expected_type=type_hints["poetry"])
-            check_type(argname="argument projenrc_js", value=projenrc_js, expected_type=type_hints["projenrc_js"])
-            check_type(argname="argument projenrc_js_options", value=projenrc_js_options, expected_type=type_hints["projenrc_js_options"])
-            check_type(argname="argument projenrc_python", value=projenrc_python, expected_type=type_hints["projenrc_python"])
-            check_type(argname="argument projenrc_python_options", value=projenrc_python_options, expected_type=type_hints["projenrc_python_options"])
-            check_type(argname="argument projenrc_ts", value=projenrc_ts, expected_type=type_hints["projenrc_ts"])
-            check_type(argname="argument projenrc_ts_options", value=projenrc_ts_options, expected_type=type_hints["projenrc_ts_options"])
-            check_type(argname="argument pytest", value=pytest, expected_type=type_hints["pytest"])
-            check_type(argname="argument pytest_options", value=pytest_options, expected_type=type_hints["pytest_options"])
-            check_type(argname="argument sample", value=sample, expected_type=type_hints["sample"])
-            check_type(argname="argument setuptools", value=setuptools, expected_type=type_hints["setuptools"])
-            check_type(argname="argument venv", value=venv, expected_type=type_hints["venv"])
-            check_type(argname="argument venv_options", value=venv_options, expected_type=type_hints["venv_options"])
             check_type(argname="argument build_command", value=build_command, expected_type=type_hints["build_command"])
             check_type(argname="argument cdkout", value=cdkout, expected_type=type_hints["cdkout"])
             check_type(argname="argument context", value=context, expected_type=type_hints["context"])
             check_type(argname="argument feature_flags", value=feature_flags, expected_type=type_hints["feature_flags"])
             check_type(argname="argument require_approval", value=require_approval, expected_type=type_hints["require_approval"])
             check_type(argname="argument watch_excludes", value=watch_excludes, expected_type=type_hints["watch_excludes"])
             check_type(argname="argument watch_includes", value=watch_includes, expected_type=type_hints["watch_includes"])
+            check_type(argname="argument author_email", value=author_email, expected_type=type_hints["author_email"])
+            check_type(argname="argument author_name", value=author_name, expected_type=type_hints["author_name"])
             check_type(argname="argument cdk_version", value=cdk_version, expected_type=type_hints["cdk_version"])
-            check_type(argname="argument cdk_assert", value=cdk_assert, expected_type=type_hints["cdk_assert"])
-            check_type(argname="argument cdk_assertions", value=cdk_assertions, expected_type=type_hints["cdk_assertions"])
-            check_type(argname="argument cdk_dependencies", value=cdk_dependencies, expected_type=type_hints["cdk_dependencies"])
-            check_type(argname="argument cdk_dependencies_as_deps", value=cdk_dependencies_as_deps, expected_type=type_hints["cdk_dependencies_as_deps"])
-            check_type(argname="argument cdk_test_dependencies", value=cdk_test_dependencies, expected_type=type_hints["cdk_test_dependencies"])
-            check_type(argname="argument cdk_version_pinning", value=cdk_version_pinning, expected_type=type_hints["cdk_version_pinning"])
             check_type(argname="argument constructs_version", value=constructs_version, expected_type=type_hints["constructs_version"])
-            check_type(argname="argument app_entrypoint", value=app_entrypoint, expected_type=type_hints["app_entrypoint"])
-            check_type(argname="argument testdir", value=testdir, expected_type=type_hints["testdir"])
+            check_type(argname="argument deps", value=deps, expected_type=type_hints["deps"])
+            check_type(argname="argument dev_deps", value=dev_deps, expected_type=type_hints["dev_deps"])
+            check_type(argname="argument module_name", value=module_name, expected_type=type_hints["module_name"])
+            check_type(argname="argument version", value=version, expected_type=type_hints["version"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "name": name,
-            "author_email": author_email,
-            "author_name": author_name,
-            "version": version,
-            "module_name": module_name,
-            "cdk_version": cdk_version,
         }
         if commit_generated is not None:
             self._values["commit_generated"] = commit_generated
         if git_ignore_options is not None:
             self._values["git_ignore_options"] = git_ignore_options
         if git_options is not None:
             self._values["git_options"] = git_options
@@ -668,92 +443,44 @@
             self._values["readme"] = readme
         if stale is not None:
             self._values["stale"] = stale
         if stale_options is not None:
             self._values["stale_options"] = stale_options
         if vscode is not None:
             self._values["vscode"] = vscode
-        if classifiers is not None:
-            self._values["classifiers"] = classifiers
-        if description is not None:
-            self._values["description"] = description
-        if homepage is not None:
-            self._values["homepage"] = homepage
-        if license is not None:
-            self._values["license"] = license
-        if package_name is not None:
-            self._values["package_name"] = package_name
-        if poetry_options is not None:
-            self._values["poetry_options"] = poetry_options
-        if setup_config is not None:
-            self._values["setup_config"] = setup_config
-        if deps is not None:
-            self._values["deps"] = deps
-        if dev_deps is not None:
-            self._values["dev_deps"] = dev_deps
-        if pip is not None:
-            self._values["pip"] = pip
-        if poetry is not None:
-            self._values["poetry"] = poetry
-        if projenrc_js is not None:
-            self._values["projenrc_js"] = projenrc_js
-        if projenrc_js_options is not None:
-            self._values["projenrc_js_options"] = projenrc_js_options
-        if projenrc_python is not None:
-            self._values["projenrc_python"] = projenrc_python
-        if projenrc_python_options is not None:
-            self._values["projenrc_python_options"] = projenrc_python_options
-        if projenrc_ts is not None:
-            self._values["projenrc_ts"] = projenrc_ts
-        if projenrc_ts_options is not None:
-            self._values["projenrc_ts_options"] = projenrc_ts_options
-        if pytest is not None:
-            self._values["pytest"] = pytest
-        if pytest_options is not None:
-            self._values["pytest_options"] = pytest_options
-        if sample is not None:
-            self._values["sample"] = sample
-        if setuptools is not None:
-            self._values["setuptools"] = setuptools
-        if venv is not None:
-            self._values["venv"] = venv
-        if venv_options is not None:
-            self._values["venv_options"] = venv_options
         if build_command is not None:
             self._values["build_command"] = build_command
         if cdkout is not None:
             self._values["cdkout"] = cdkout
         if context is not None:
             self._values["context"] = context
         if feature_flags is not None:
             self._values["feature_flags"] = feature_flags
         if require_approval is not None:
             self._values["require_approval"] = require_approval
         if watch_excludes is not None:
             self._values["watch_excludes"] = watch_excludes
         if watch_includes is not None:
             self._values["watch_includes"] = watch_includes
-        if cdk_assert is not None:
-            self._values["cdk_assert"] = cdk_assert
-        if cdk_assertions is not None:
-            self._values["cdk_assertions"] = cdk_assertions
-        if cdk_dependencies is not None:
-            self._values["cdk_dependencies"] = cdk_dependencies
-        if cdk_dependencies_as_deps is not None:
-            self._values["cdk_dependencies_as_deps"] = cdk_dependencies_as_deps
-        if cdk_test_dependencies is not None:
-            self._values["cdk_test_dependencies"] = cdk_test_dependencies
-        if cdk_version_pinning is not None:
-            self._values["cdk_version_pinning"] = cdk_version_pinning
+        if author_email is not None:
+            self._values["author_email"] = author_email
+        if author_name is not None:
+            self._values["author_name"] = author_name
+        if cdk_version is not None:
+            self._values["cdk_version"] = cdk_version
         if constructs_version is not None:
             self._values["constructs_version"] = constructs_version
-        if app_entrypoint is not None:
-            self._values["app_entrypoint"] = app_entrypoint
-        if testdir is not None:
-            self._values["testdir"] = testdir
+        if deps is not None:
+            self._values["deps"] = deps
+        if dev_deps is not None:
+            self._values["dev_deps"] = dev_deps
+        if module_name is not None:
+            self._values["module_name"] = module_name
+        if version is not None:
+            self._values["version"] = version
 
     @builtins.property
     def name(self) -> builtins.str:
         '''(experimental) This is the name of your project.
 
         :default: $BASEDIR
 
@@ -1112,575 +839,1239 @@
 
         :stability: experimental
         '''
         result = self._values.get("vscode")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def author_email(self) -> builtins.str:
-        '''(experimental) Author's e-mail.
+    def build_command(self) -> typing.Optional[builtins.str]:
+        '''(experimental) A command to execute before synthesis.
 
-        :default: $GIT_USER_EMAIL
+        This command will be called when
+        running ``cdk synth`` or when ``cdk watch`` identifies a change in your source
+        code before redeployment.
+
+        :default: - no build command
 
         :stability: experimental
         '''
-        result = self._values.get("author_email")
-        assert result is not None, "Required property 'author_email' is missing"
-        return typing.cast(builtins.str, result)
+        result = self._values.get("build_command")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def author_name(self) -> builtins.str:
-        '''(experimental) Author's name.
+    def cdkout(self) -> typing.Optional[builtins.str]:
+        '''(experimental) cdk.out directory.
 
-        :default: $GIT_USER_NAME
+        :default: "cdk.out"
 
         :stability: experimental
         '''
-        result = self._values.get("author_name")
-        assert result is not None, "Required property 'author_name' is missing"
-        return typing.cast(builtins.str, result)
+        result = self._values.get("cdkout")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def version(self) -> builtins.str:
-        '''(experimental) Version of the package.
+    def context(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''(experimental) Additional context to include in ``cdk.json``.
 
-        :default: "0.1.0"
+        :default: - no additional context
 
         :stability: experimental
-        :featured: true
         '''
-        result = self._values.get("version")
-        assert result is not None, "Required property 'version' is missing"
-        return typing.cast(builtins.str, result)
+        result = self._values.get("context")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
 
     @builtins.property
-    def classifiers(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''(experimental) A list of PyPI trove classifiers that describe the project.
+    def feature_flags(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Include all feature flags in cdk.json.
+
+        :default: true
 
-        :see: https://pypi.org/classifiers/
         :stability: experimental
         '''
-        result = self._values.get("classifiers")
-        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+        result = self._values.get("feature_flags")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def description(self) -> typing.Optional[builtins.str]:
-        '''(experimental) A short description of the package.
+    def require_approval(
+        self,
+    ) -> typing.Optional[_projen_awscdk_04054675.ApprovalLevel]:
+        '''(experimental) To protect you against unintended changes that affect your security posture, the AWS CDK Toolkit prompts you to approve security-related changes before deploying them.
+
+        :default: ApprovalLevel.BROADENING
 
         :stability: experimental
-        :featured: true
         '''
-        result = self._values.get("description")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("require_approval")
+        return typing.cast(typing.Optional[_projen_awscdk_04054675.ApprovalLevel], result)
 
     @builtins.property
-    def homepage(self) -> typing.Optional[builtins.str]:
-        '''(experimental) A URL to the website of the project.
+    def watch_excludes(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''(experimental) Glob patterns to exclude from ``cdk watch``.
+
+        :default: []
 
         :stability: experimental
         '''
-        result = self._values.get("homepage")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("watch_excludes")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
-    def license(self) -> typing.Optional[builtins.str]:
-        '''(experimental) License of this package as an SPDX identifier.
+    def watch_includes(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''(experimental) Glob patterns to include in ``cdk watch``.
+
+        :default: []
 
         :stability: experimental
         '''
-        result = self._values.get("license")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("watch_includes")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
-    def package_name(self) -> typing.Optional[builtins.str]:
-        '''(experimental) Package name.
+    def author_email(self) -> typing.Optional[builtins.str]:
+        '''Author's e-mail.
 
-        :stability: experimental
+        :default: "pinton.filippo
+
+        :protonmail: .com"
         '''
-        result = self._values.get("package_name")
+        result = self._values.get("author_email")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def poetry_options(
-        self,
-    ) -> typing.Optional[_projen_python_04054675.PoetryPyprojectOptionsWithoutDeps]:
-        '''(experimental) Additional options to set for poetry if using poetry.
+    def author_name(self) -> typing.Optional[builtins.str]:
+        '''Author's name.
 
-        :stability: experimental
+        :default: "Filippo Pinton"
         '''
-        result = self._values.get("poetry_options")
-        return typing.cast(typing.Optional[_projen_python_04054675.PoetryPyprojectOptionsWithoutDeps], result)
+        result = self._values.get("author_name")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def setup_config(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
-        '''(experimental) Additional fields to pass in the setup() function if using setuptools.
+    def cdk_version(self) -> typing.Optional[builtins.str]:
+        '''Minimum version of the AWS CDK to depend on.
 
-        :stability: experimental
+        :default: "2.74.0"
         '''
-        result = self._values.get("setup_config")
-        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
+        result = self._values.get("cdk_version")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def module_name(self) -> builtins.str:
-        '''(experimental) Name of the python package as used in imports and filenames.
-
-        Must only consist of alphanumeric characters and underscores.
-
-        :default: $PYTHON_MODULE_NAME
+    def constructs_version(self) -> typing.Optional[builtins.str]:
+        '''Minimum version of the ``constructs`` library to depend on.
 
-        :stability: experimental
+        :default: "10.0.5".
         '''
-        result = self._values.get("module_name")
-        assert result is not None, "Required property 'module_name' is missing"
-        return typing.cast(builtins.str, result)
+        result = self._values.get("constructs_version")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def deps(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''(experimental) List of runtime dependencies for this project.
+        '''List of runtime dependencies for this project.
 
         Dependencies use the format: ``<module>@<semver>``
 
         Additional dependencies can be added via ``project.addDependency()``.
 
-        :default: []
+        :default: "[ 'butterneck-cdk-constructs' ]"
 
-        :stability: experimental
         :featured: true
         '''
         result = self._values.get("deps")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def dev_deps(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''(experimental) List of dev dependencies for this project.
+        '''List of dev dependencies for this project.
 
         Dependencies use the format: ``<module>@<semver>``
 
         Additional dependencies can be added via ``project.addDevDependency()``.
 
         :default: []
 
-        :stability: experimental
         :featured: true
         '''
         result = self._values.get("dev_deps")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
-    def pip(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Use pip with a requirements.txt file to track project dependencies.
+    def module_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the python package as used in imports and filenames.
+
+        Must only consist of alphanumeric characters and underscores.
+
+        :default: ""
+        '''
+        result = self._values.get("module_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def version(self) -> typing.Optional[builtins.str]:
+        '''Version of the package.
 
-        :default: - true, unless poetry is true, then false
+        :default: "0.0.0"
 
-        :stability: experimental
         :featured: true
         '''
-        result = self._values.get("pip")
-        return typing.cast(typing.Optional[builtins.bool], result)
+        result = self._values.get("version")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "ButterneckAwsCdkPythonAppOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class GoApp(
+    _projen_github_04054675.GitHubProject,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="butterneck-projen.GoApp",
+):
+    '''GoApp Project.
+
+    :class: GoApp
+    :export: true
+    :extends: awscdk.AwsCdkPythonApp *
+    :pjid: go-app
+    '''
+
+    def __init__(
+        self,
+        *,
+        auto_approve_options: typing.Optional[typing.Union[_projen_github_04054675.AutoApproveOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        auto_merge: typing.Optional[builtins.bool] = None,
+        auto_merge_options: typing.Optional[typing.Union[_projen_github_04054675.AutoMergeOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        clobber: typing.Optional[builtins.bool] = None,
+        dev_container: typing.Optional[builtins.bool] = None,
+        github: typing.Optional[builtins.bool] = None,
+        github_options: typing.Optional[typing.Union[_projen_github_04054675.GitHubOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        gitpod: typing.Optional[builtins.bool] = None,
+        mergify: typing.Optional[builtins.bool] = None,
+        mergify_options: typing.Optional[typing.Union[_projen_github_04054675.MergifyOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        project_type: typing.Optional[_projen_04054675.ProjectType] = None,
+        projen_credentials: typing.Optional[_projen_github_04054675.GithubCredentials] = None,
+        projen_token_secret: typing.Optional[builtins.str] = None,
+        readme: typing.Optional[typing.Union[_projen_04054675.SampleReadmeProps, typing.Dict[builtins.str, typing.Any]]] = None,
+        stale: typing.Optional[builtins.bool] = None,
+        stale_options: typing.Optional[typing.Union[_projen_github_04054675.StaleOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        vscode: typing.Optional[builtins.bool] = None,
+        name: builtins.str,
+        commit_generated: typing.Optional[builtins.bool] = None,
+        git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        logging: typing.Optional[typing.Union[_projen_04054675.LoggerOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        outdir: typing.Optional[builtins.str] = None,
+        parent: typing.Optional[_projen_04054675.Project] = None,
+        projen_command: typing.Optional[builtins.str] = None,
+        projenrc_json: typing.Optional[builtins.bool] = None,
+        projenrc_json_options: typing.Optional[typing.Union[_projen_04054675.ProjenrcJsonOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        renovatebot: typing.Optional[builtins.bool] = None,
+        renovatebot_options: typing.Optional[typing.Union[_projen_04054675.RenovatebotOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> None:
+        '''
+        :param auto_approve_options: (experimental) Enable and configure the 'auto approve' workflow. Default: - auto approve is disabled
+        :param auto_merge: (experimental) Enable automatic merging on GitHub. Has no effect if ``github.mergify`` is set to false. Default: true
+        :param auto_merge_options: (experimental) Configure options for automatic merging on GitHub. Has no effect if ``github.mergify`` or ``autoMerge`` is set to false. Default: - see defaults in ``AutoMergeOptions``
+        :param clobber: (experimental) Add a ``clobber`` task which resets the repo to origin. Default: - true, but false for subprojects
+        :param dev_container: (experimental) Add a VSCode development environment (used for GitHub Codespaces). Default: false
+        :param github: (experimental) Enable GitHub integration. Enabled by default for root projects. Disabled for non-root projects. Default: true
+        :param github_options: (experimental) Options for GitHub integration. Default: - see GitHubOptions
+        :param gitpod: (experimental) Add a Gitpod development environment. Default: false
+        :param mergify: (deprecated) Whether mergify should be enabled on this repository or not. Default: true
+        :param mergify_options: (deprecated) Options for mergify. Default: - default options
+        :param project_type: (deprecated) Which type of project this is (library/app). Default: ProjectType.UNKNOWN
+        :param projen_credentials: (experimental) Choose a method of providing GitHub API access for projen workflows. Default: - use a personal access token named PROJEN_GITHUB_TOKEN
+        :param projen_token_secret: (deprecated) The name of a secret which includes a GitHub Personal Access Token to be used by projen workflows. This token needs to have the ``repo``, ``workflows`` and ``packages`` scope. Default: "PROJEN_GITHUB_TOKEN"
+        :param readme: (experimental) The README setup. Default: - { filename: 'README.md', contents: '# replace this' }
+        :param stale: (experimental) Auto-close of stale issues and pull request. See ``staleOptions`` for options. Default: false
+        :param stale_options: (experimental) Auto-close stale issues and pull requests. To disable set ``stale`` to ``false``. Default: - see defaults in ``StaleOptions``
+        :param vscode: (experimental) Enable VSCode integration. Enabled by default for root projects. Disabled for non-root projects. Default: true
+        :param name: (experimental) This is the name of your project. Default: $BASEDIR
+        :param commit_generated: (experimental) Whether to commit the managed files by default. Default: true
+        :param git_ignore_options: (experimental) Configuration options for .gitignore file.
+        :param git_options: (experimental) Configuration options for git.
+        :param logging: (experimental) Configure logging options such as verbosity. Default: {}
+        :param outdir: (experimental) The root directory of the project. Relative to this directory, all files are synthesized. If this project has a parent, this directory is relative to the parent directory and it cannot be the same as the parent or any of it's other sub-projects. Default: "."
+        :param parent: (experimental) The parent project, if this project is part of a bigger project.
+        :param projen_command: (experimental) The shell command to use in order to run the projen CLI. Can be used to customize in special environments. Default: "npx projen"
+        :param projenrc_json: (experimental) Generate (once) .projenrc.json (in JSON). Set to ``false`` in order to disable .projenrc.json generation. Default: false
+        :param projenrc_json_options: (experimental) Options for .projenrc.json. Default: - default options
+        :param renovatebot: (experimental) Use renovatebot to handle dependency upgrades. Default: false
+        :param renovatebot_options: (experimental) Options for renovatebot. Default: - default options
+        '''
+        options = GoAppOptions(
+            auto_approve_options=auto_approve_options,
+            auto_merge=auto_merge,
+            auto_merge_options=auto_merge_options,
+            clobber=clobber,
+            dev_container=dev_container,
+            github=github,
+            github_options=github_options,
+            gitpod=gitpod,
+            mergify=mergify,
+            mergify_options=mergify_options,
+            project_type=project_type,
+            projen_credentials=projen_credentials,
+            projen_token_secret=projen_token_secret,
+            readme=readme,
+            stale=stale,
+            stale_options=stale_options,
+            vscode=vscode,
+            name=name,
+            commit_generated=commit_generated,
+            git_ignore_options=git_ignore_options,
+            git_options=git_options,
+            logging=logging,
+            outdir=outdir,
+            parent=parent,
+            projen_command=projen_command,
+            projenrc_json=projenrc_json,
+            projenrc_json_options=projenrc_json_options,
+            renovatebot=renovatebot,
+            renovatebot_options=renovatebot_options,
+        )
+
+        jsii.create(self.__class__, self, [options])
 
     @builtins.property
-    def poetry(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Use poetry to manage your project dependencies, virtual environment, and (optional) packaging/publishing.
+    @jsii.member(jsii_name="infraProject")
+    def infra_project(self) -> ButterneckAwsCdkPythonApp:
+        return typing.cast(ButterneckAwsCdkPythonApp, jsii.get(self, "infraProject"))
 
-        This feature is incompatible with pip, setuptools, or venv.
-        If you set this option to ``true``, then pip, setuptools, and venv must be set to ``false``.
+    @infra_project.setter
+    def infra_project(self, value: ButterneckAwsCdkPythonApp) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ee2b3fdb8f9ae93e4279d52a15be8cf3032f8d86cb8a72fb7689c506e4e7d855)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "infraProject", value)
 
-        :default: false
+    @builtins.property
+    @jsii.member(jsii_name="serviceProject")
+    def service_project(self) -> "GoProject":
+        return typing.cast("GoProject", jsii.get(self, "serviceProject"))
+
+    @service_project.setter
+    def service_project(self, value: "GoProject") -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__217b491360c87c72aaa4ea7ba8a3f98bf9c840fbb010f10d9d1abfee2516eec2)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "serviceProject", value)
+
+
+@jsii.data_type(
+    jsii_type="butterneck-projen.GoAppOptions",
+    jsii_struct_bases=[_projen_github_04054675.GitHubProjectOptions],
+    name_mapping={
+        "name": "name",
+        "commit_generated": "commitGenerated",
+        "git_ignore_options": "gitIgnoreOptions",
+        "git_options": "gitOptions",
+        "logging": "logging",
+        "outdir": "outdir",
+        "parent": "parent",
+        "projen_command": "projenCommand",
+        "projenrc_json": "projenrcJson",
+        "projenrc_json_options": "projenrcJsonOptions",
+        "renovatebot": "renovatebot",
+        "renovatebot_options": "renovatebotOptions",
+        "auto_approve_options": "autoApproveOptions",
+        "auto_merge": "autoMerge",
+        "auto_merge_options": "autoMergeOptions",
+        "clobber": "clobber",
+        "dev_container": "devContainer",
+        "github": "github",
+        "github_options": "githubOptions",
+        "gitpod": "gitpod",
+        "mergify": "mergify",
+        "mergify_options": "mergifyOptions",
+        "project_type": "projectType",
+        "projen_credentials": "projenCredentials",
+        "projen_token_secret": "projenTokenSecret",
+        "readme": "readme",
+        "stale": "stale",
+        "stale_options": "staleOptions",
+        "vscode": "vscode",
+    },
+)
+class GoAppOptions(_projen_github_04054675.GitHubProjectOptions):
+    def __init__(
+        self,
+        *,
+        name: builtins.str,
+        commit_generated: typing.Optional[builtins.bool] = None,
+        git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        logging: typing.Optional[typing.Union[_projen_04054675.LoggerOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        outdir: typing.Optional[builtins.str] = None,
+        parent: typing.Optional[_projen_04054675.Project] = None,
+        projen_command: typing.Optional[builtins.str] = None,
+        projenrc_json: typing.Optional[builtins.bool] = None,
+        projenrc_json_options: typing.Optional[typing.Union[_projen_04054675.ProjenrcJsonOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        renovatebot: typing.Optional[builtins.bool] = None,
+        renovatebot_options: typing.Optional[typing.Union[_projen_04054675.RenovatebotOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        auto_approve_options: typing.Optional[typing.Union[_projen_github_04054675.AutoApproveOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        auto_merge: typing.Optional[builtins.bool] = None,
+        auto_merge_options: typing.Optional[typing.Union[_projen_github_04054675.AutoMergeOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        clobber: typing.Optional[builtins.bool] = None,
+        dev_container: typing.Optional[builtins.bool] = None,
+        github: typing.Optional[builtins.bool] = None,
+        github_options: typing.Optional[typing.Union[_projen_github_04054675.GitHubOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        gitpod: typing.Optional[builtins.bool] = None,
+        mergify: typing.Optional[builtins.bool] = None,
+        mergify_options: typing.Optional[typing.Union[_projen_github_04054675.MergifyOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        project_type: typing.Optional[_projen_04054675.ProjectType] = None,
+        projen_credentials: typing.Optional[_projen_github_04054675.GithubCredentials] = None,
+        projen_token_secret: typing.Optional[builtins.str] = None,
+        readme: typing.Optional[typing.Union[_projen_04054675.SampleReadmeProps, typing.Dict[builtins.str, typing.Any]]] = None,
+        stale: typing.Optional[builtins.bool] = None,
+        stale_options: typing.Optional[typing.Union[_projen_github_04054675.StaleOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        vscode: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''
+        :param name: (experimental) This is the name of your project. Default: $BASEDIR
+        :param commit_generated: (experimental) Whether to commit the managed files by default. Default: true
+        :param git_ignore_options: (experimental) Configuration options for .gitignore file.
+        :param git_options: (experimental) Configuration options for git.
+        :param logging: (experimental) Configure logging options such as verbosity. Default: {}
+        :param outdir: (experimental) The root directory of the project. Relative to this directory, all files are synthesized. If this project has a parent, this directory is relative to the parent directory and it cannot be the same as the parent or any of it's other sub-projects. Default: "."
+        :param parent: (experimental) The parent project, if this project is part of a bigger project.
+        :param projen_command: (experimental) The shell command to use in order to run the projen CLI. Can be used to customize in special environments. Default: "npx projen"
+        :param projenrc_json: (experimental) Generate (once) .projenrc.json (in JSON). Set to ``false`` in order to disable .projenrc.json generation. Default: false
+        :param projenrc_json_options: (experimental) Options for .projenrc.json. Default: - default options
+        :param renovatebot: (experimental) Use renovatebot to handle dependency upgrades. Default: false
+        :param renovatebot_options: (experimental) Options for renovatebot. Default: - default options
+        :param auto_approve_options: (experimental) Enable and configure the 'auto approve' workflow. Default: - auto approve is disabled
+        :param auto_merge: (experimental) Enable automatic merging on GitHub. Has no effect if ``github.mergify`` is set to false. Default: true
+        :param auto_merge_options: (experimental) Configure options for automatic merging on GitHub. Has no effect if ``github.mergify`` or ``autoMerge`` is set to false. Default: - see defaults in ``AutoMergeOptions``
+        :param clobber: (experimental) Add a ``clobber`` task which resets the repo to origin. Default: - true, but false for subprojects
+        :param dev_container: (experimental) Add a VSCode development environment (used for GitHub Codespaces). Default: false
+        :param github: (experimental) Enable GitHub integration. Enabled by default for root projects. Disabled for non-root projects. Default: true
+        :param github_options: (experimental) Options for GitHub integration. Default: - see GitHubOptions
+        :param gitpod: (experimental) Add a Gitpod development environment. Default: false
+        :param mergify: (deprecated) Whether mergify should be enabled on this repository or not. Default: true
+        :param mergify_options: (deprecated) Options for mergify. Default: - default options
+        :param project_type: (deprecated) Which type of project this is (library/app). Default: ProjectType.UNKNOWN
+        :param projen_credentials: (experimental) Choose a method of providing GitHub API access for projen workflows. Default: - use a personal access token named PROJEN_GITHUB_TOKEN
+        :param projen_token_secret: (deprecated) The name of a secret which includes a GitHub Personal Access Token to be used by projen workflows. This token needs to have the ``repo``, ``workflows`` and ``packages`` scope. Default: "PROJEN_GITHUB_TOKEN"
+        :param readme: (experimental) The README setup. Default: - { filename: 'README.md', contents: '# replace this' }
+        :param stale: (experimental) Auto-close of stale issues and pull request. See ``staleOptions`` for options. Default: false
+        :param stale_options: (experimental) Auto-close stale issues and pull requests. To disable set ``stale`` to ``false``. Default: - see defaults in ``StaleOptions``
+        :param vscode: (experimental) Enable VSCode integration. Enabled by default for root projects. Disabled for non-root projects. Default: true
+        '''
+        if isinstance(git_ignore_options, dict):
+            git_ignore_options = _projen_04054675.IgnoreFileOptions(**git_ignore_options)
+        if isinstance(git_options, dict):
+            git_options = _projen_04054675.GitOptions(**git_options)
+        if isinstance(logging, dict):
+            logging = _projen_04054675.LoggerOptions(**logging)
+        if isinstance(projenrc_json_options, dict):
+            projenrc_json_options = _projen_04054675.ProjenrcJsonOptions(**projenrc_json_options)
+        if isinstance(renovatebot_options, dict):
+            renovatebot_options = _projen_04054675.RenovatebotOptions(**renovatebot_options)
+        if isinstance(auto_approve_options, dict):
+            auto_approve_options = _projen_github_04054675.AutoApproveOptions(**auto_approve_options)
+        if isinstance(auto_merge_options, dict):
+            auto_merge_options = _projen_github_04054675.AutoMergeOptions(**auto_merge_options)
+        if isinstance(github_options, dict):
+            github_options = _projen_github_04054675.GitHubOptions(**github_options)
+        if isinstance(mergify_options, dict):
+            mergify_options = _projen_github_04054675.MergifyOptions(**mergify_options)
+        if isinstance(readme, dict):
+            readme = _projen_04054675.SampleReadmeProps(**readme)
+        if isinstance(stale_options, dict):
+            stale_options = _projen_github_04054675.StaleOptions(**stale_options)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__e7cdfb665920a033d76499e282ce137ada7759e9a66b20380e8aae21552e8eb6)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument commit_generated", value=commit_generated, expected_type=type_hints["commit_generated"])
+            check_type(argname="argument git_ignore_options", value=git_ignore_options, expected_type=type_hints["git_ignore_options"])
+            check_type(argname="argument git_options", value=git_options, expected_type=type_hints["git_options"])
+            check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
+            check_type(argname="argument outdir", value=outdir, expected_type=type_hints["outdir"])
+            check_type(argname="argument parent", value=parent, expected_type=type_hints["parent"])
+            check_type(argname="argument projen_command", value=projen_command, expected_type=type_hints["projen_command"])
+            check_type(argname="argument projenrc_json", value=projenrc_json, expected_type=type_hints["projenrc_json"])
+            check_type(argname="argument projenrc_json_options", value=projenrc_json_options, expected_type=type_hints["projenrc_json_options"])
+            check_type(argname="argument renovatebot", value=renovatebot, expected_type=type_hints["renovatebot"])
+            check_type(argname="argument renovatebot_options", value=renovatebot_options, expected_type=type_hints["renovatebot_options"])
+            check_type(argname="argument auto_approve_options", value=auto_approve_options, expected_type=type_hints["auto_approve_options"])
+            check_type(argname="argument auto_merge", value=auto_merge, expected_type=type_hints["auto_merge"])
+            check_type(argname="argument auto_merge_options", value=auto_merge_options, expected_type=type_hints["auto_merge_options"])
+            check_type(argname="argument clobber", value=clobber, expected_type=type_hints["clobber"])
+            check_type(argname="argument dev_container", value=dev_container, expected_type=type_hints["dev_container"])
+            check_type(argname="argument github", value=github, expected_type=type_hints["github"])
+            check_type(argname="argument github_options", value=github_options, expected_type=type_hints["github_options"])
+            check_type(argname="argument gitpod", value=gitpod, expected_type=type_hints["gitpod"])
+            check_type(argname="argument mergify", value=mergify, expected_type=type_hints["mergify"])
+            check_type(argname="argument mergify_options", value=mergify_options, expected_type=type_hints["mergify_options"])
+            check_type(argname="argument project_type", value=project_type, expected_type=type_hints["project_type"])
+            check_type(argname="argument projen_credentials", value=projen_credentials, expected_type=type_hints["projen_credentials"])
+            check_type(argname="argument projen_token_secret", value=projen_token_secret, expected_type=type_hints["projen_token_secret"])
+            check_type(argname="argument readme", value=readme, expected_type=type_hints["readme"])
+            check_type(argname="argument stale", value=stale, expected_type=type_hints["stale"])
+            check_type(argname="argument stale_options", value=stale_options, expected_type=type_hints["stale_options"])
+            check_type(argname="argument vscode", value=vscode, expected_type=type_hints["vscode"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "name": name,
+        }
+        if commit_generated is not None:
+            self._values["commit_generated"] = commit_generated
+        if git_ignore_options is not None:
+            self._values["git_ignore_options"] = git_ignore_options
+        if git_options is not None:
+            self._values["git_options"] = git_options
+        if logging is not None:
+            self._values["logging"] = logging
+        if outdir is not None:
+            self._values["outdir"] = outdir
+        if parent is not None:
+            self._values["parent"] = parent
+        if projen_command is not None:
+            self._values["projen_command"] = projen_command
+        if projenrc_json is not None:
+            self._values["projenrc_json"] = projenrc_json
+        if projenrc_json_options is not None:
+            self._values["projenrc_json_options"] = projenrc_json_options
+        if renovatebot is not None:
+            self._values["renovatebot"] = renovatebot
+        if renovatebot_options is not None:
+            self._values["renovatebot_options"] = renovatebot_options
+        if auto_approve_options is not None:
+            self._values["auto_approve_options"] = auto_approve_options
+        if auto_merge is not None:
+            self._values["auto_merge"] = auto_merge
+        if auto_merge_options is not None:
+            self._values["auto_merge_options"] = auto_merge_options
+        if clobber is not None:
+            self._values["clobber"] = clobber
+        if dev_container is not None:
+            self._values["dev_container"] = dev_container
+        if github is not None:
+            self._values["github"] = github
+        if github_options is not None:
+            self._values["github_options"] = github_options
+        if gitpod is not None:
+            self._values["gitpod"] = gitpod
+        if mergify is not None:
+            self._values["mergify"] = mergify
+        if mergify_options is not None:
+            self._values["mergify_options"] = mergify_options
+        if project_type is not None:
+            self._values["project_type"] = project_type
+        if projen_credentials is not None:
+            self._values["projen_credentials"] = projen_credentials
+        if projen_token_secret is not None:
+            self._values["projen_token_secret"] = projen_token_secret
+        if readme is not None:
+            self._values["readme"] = readme
+        if stale is not None:
+            self._values["stale"] = stale
+        if stale_options is not None:
+            self._values["stale_options"] = stale_options
+        if vscode is not None:
+            self._values["vscode"] = vscode
+
+    @builtins.property
+    def name(self) -> builtins.str:
+        '''(experimental) This is the name of your project.
+
+        :default: $BASEDIR
 
         :stability: experimental
         :featured: true
         '''
-        result = self._values.get("poetry")
+        result = self._values.get("name")
+        assert result is not None, "Required property 'name' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def commit_generated(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Whether to commit the managed files by default.
+
+        :default: true
+
+        :stability: experimental
+        '''
+        result = self._values.get("commit_generated")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def projenrc_js(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Use projenrc in javascript.
+    def git_ignore_options(self) -> typing.Optional[_projen_04054675.IgnoreFileOptions]:
+        '''(experimental) Configuration options for .gitignore file.
 
-        This will install ``projen`` as a JavaScript dependency and add a ``synth``
-        task which will run ``.projenrc.js``.
+        :stability: experimental
+        '''
+        result = self._values.get("git_ignore_options")
+        return typing.cast(typing.Optional[_projen_04054675.IgnoreFileOptions], result)
 
-        :default: false
+    @builtins.property
+    def git_options(self) -> typing.Optional[_projen_04054675.GitOptions]:
+        '''(experimental) Configuration options for git.
 
         :stability: experimental
         '''
-        result = self._values.get("projenrc_js")
-        return typing.cast(typing.Optional[builtins.bool], result)
+        result = self._values.get("git_options")
+        return typing.cast(typing.Optional[_projen_04054675.GitOptions], result)
 
     @builtins.property
-    def projenrc_js_options(
-        self,
-    ) -> typing.Optional[_projen_javascript_04054675.ProjenrcOptions]:
-        '''(experimental) Options related to projenrc in JavaScript.
+    def logging(self) -> typing.Optional[_projen_04054675.LoggerOptions]:
+        '''(experimental) Configure logging options such as verbosity.
 
-        :default: - default options
+        :default: {}
 
         :stability: experimental
         '''
-        result = self._values.get("projenrc_js_options")
-        return typing.cast(typing.Optional[_projen_javascript_04054675.ProjenrcOptions], result)
+        result = self._values.get("logging")
+        return typing.cast(typing.Optional[_projen_04054675.LoggerOptions], result)
 
     @builtins.property
-    def projenrc_python(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Use projenrc in Python.
+    def outdir(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The root directory of the project.
 
-        This will install ``projen`` as a Python dependency and add a ``synth``
-        task which will run ``.projenrc.py``.
+        Relative to this directory, all files are synthesized.
 
-        :default: true
+        If this project has a parent, this directory is relative to the parent
+        directory and it cannot be the same as the parent or any of it's other
+        sub-projects.
+
+        :default: "."
 
         :stability: experimental
         '''
-        result = self._values.get("projenrc_python")
-        return typing.cast(typing.Optional[builtins.bool], result)
+        result = self._values.get("outdir")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def projenrc_python_options(
-        self,
-    ) -> typing.Optional[_projen_python_04054675.ProjenrcOptions]:
-        '''(experimental) Options related to projenrc in python.
-
-        :default: - default options
+    def parent(self) -> typing.Optional[_projen_04054675.Project]:
+        '''(experimental) The parent project, if this project is part of a bigger project.
 
         :stability: experimental
         '''
-        result = self._values.get("projenrc_python_options")
-        return typing.cast(typing.Optional[_projen_python_04054675.ProjenrcOptions], result)
+        result = self._values.get("parent")
+        return typing.cast(typing.Optional[_projen_04054675.Project], result)
 
     @builtins.property
-    def projenrc_ts(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Use projenrc in TypeScript.
+    def projen_command(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The shell command to use in order to run the projen CLI.
+
+        Can be used to customize in special environments.
+
+        :default: "npx projen"
 
-        This will create a tsconfig file (default: ``tsconfig.projen.json``)
-        and use ``ts-node`` in the default task to parse the project source files.
+        :stability: experimental
+        '''
+        result = self._values.get("projen_command")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def projenrc_json(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Generate (once) .projenrc.json (in JSON). Set to ``false`` in order to disable .projenrc.json generation.
 
         :default: false
 
         :stability: experimental
         '''
-        result = self._values.get("projenrc_ts")
+        result = self._values.get("projenrc_json")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def projenrc_ts_options(
+    def projenrc_json_options(
         self,
-    ) -> typing.Optional[_projen_typescript_04054675.ProjenrcTsOptions]:
-        '''(experimental) Options related to projenrc in TypeScript.
+    ) -> typing.Optional[_projen_04054675.ProjenrcJsonOptions]:
+        '''(experimental) Options for .projenrc.json.
 
         :default: - default options
 
         :stability: experimental
         '''
-        result = self._values.get("projenrc_ts_options")
-        return typing.cast(typing.Optional[_projen_typescript_04054675.ProjenrcTsOptions], result)
+        result = self._values.get("projenrc_json_options")
+        return typing.cast(typing.Optional[_projen_04054675.ProjenrcJsonOptions], result)
 
     @builtins.property
-    def pytest(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Include pytest tests.
+    def renovatebot(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Use renovatebot to handle dependency upgrades.
 
-        :default: true
+        :default: false
 
         :stability: experimental
-        :featured: true
         '''
-        result = self._values.get("pytest")
+        result = self._values.get("renovatebot")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def pytest_options(self) -> typing.Optional[_projen_python_04054675.PytestOptions]:
-        '''(experimental) pytest options.
+    def renovatebot_options(
+        self,
+    ) -> typing.Optional[_projen_04054675.RenovatebotOptions]:
+        '''(experimental) Options for renovatebot.
 
-        :default: - defaults
+        :default: - default options
 
         :stability: experimental
         '''
-        result = self._values.get("pytest_options")
-        return typing.cast(typing.Optional[_projen_python_04054675.PytestOptions], result)
+        result = self._values.get("renovatebot_options")
+        return typing.cast(typing.Optional[_projen_04054675.RenovatebotOptions], result)
+
+    @builtins.property
+    def auto_approve_options(
+        self,
+    ) -> typing.Optional[_projen_github_04054675.AutoApproveOptions]:
+        '''(experimental) Enable and configure the 'auto approve' workflow.
+
+        :default: - auto approve is disabled
+
+        :stability: experimental
+        '''
+        result = self._values.get("auto_approve_options")
+        return typing.cast(typing.Optional[_projen_github_04054675.AutoApproveOptions], result)
 
     @builtins.property
-    def sample(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Include sample code and test if the relevant directories don't exist.
+    def auto_merge(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Enable automatic merging on GitHub.
+
+        Has no effect if ``github.mergify``
+        is set to false.
 
         :default: true
 
         :stability: experimental
         '''
-        result = self._values.get("sample")
+        result = self._values.get("auto_merge")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def setuptools(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Use setuptools with a setup.py script for packaging and publishing.
+    def auto_merge_options(
+        self,
+    ) -> typing.Optional[_projen_github_04054675.AutoMergeOptions]:
+        '''(experimental) Configure options for automatic merging on GitHub.
 
-        :default: - true, unless poetry is true, then false
+        Has no effect if
+        ``github.mergify`` or ``autoMerge`` is set to false.
+
+        :default: - see defaults in ``AutoMergeOptions``
 
         :stability: experimental
-        :featured: true
         '''
-        result = self._values.get("setuptools")
-        return typing.cast(typing.Optional[builtins.bool], result)
+        result = self._values.get("auto_merge_options")
+        return typing.cast(typing.Optional[_projen_github_04054675.AutoMergeOptions], result)
 
     @builtins.property
-    def venv(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Use venv to manage a virtual environment for installing dependencies inside.
+    def clobber(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Add a ``clobber`` task which resets the repo to origin.
 
-        :default: - true, unless poetry is true, then false
+        :default: - true, but false for subprojects
 
         :stability: experimental
-        :featured: true
         '''
-        result = self._values.get("venv")
+        result = self._values.get("clobber")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def venv_options(self) -> typing.Optional[_projen_python_04054675.VenvOptions]:
-        '''(experimental) Venv options.
+    def dev_container(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Add a VSCode development environment (used for GitHub Codespaces).
 
-        :default: - defaults
+        :default: false
 
         :stability: experimental
         '''
-        result = self._values.get("venv_options")
-        return typing.cast(typing.Optional[_projen_python_04054675.VenvOptions], result)
+        result = self._values.get("dev_container")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def build_command(self) -> typing.Optional[builtins.str]:
-        '''(experimental) A command to execute before synthesis.
+    def github(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Enable GitHub integration.
 
-        This command will be called when
-        running ``cdk synth`` or when ``cdk watch`` identifies a change in your source
-        code before redeployment.
+        Enabled by default for root projects. Disabled for non-root projects.
 
-        :default: - no build command
+        :default: true
 
         :stability: experimental
         '''
-        result = self._values.get("build_command")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("github")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def cdkout(self) -> typing.Optional[builtins.str]:
-        '''(experimental) cdk.out directory.
+    def github_options(self) -> typing.Optional[_projen_github_04054675.GitHubOptions]:
+        '''(experimental) Options for GitHub integration.
 
-        :default: "cdk.out"
+        :default: - see GitHubOptions
 
         :stability: experimental
         '''
-        result = self._values.get("cdkout")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("github_options")
+        return typing.cast(typing.Optional[_projen_github_04054675.GitHubOptions], result)
 
     @builtins.property
-    def context(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
-        '''(experimental) Additional context to include in ``cdk.json``.
+    def gitpod(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Add a Gitpod development environment.
 
-        :default: - no additional context
+        :default: false
 
         :stability: experimental
         '''
-        result = self._values.get("context")
-        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
+        result = self._values.get("gitpod")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def feature_flags(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Include all feature flags in cdk.json.
+    def mergify(self) -> typing.Optional[builtins.bool]:
+        '''(deprecated) Whether mergify should be enabled on this repository or not.
 
         :default: true
 
-        :stability: experimental
+        :deprecated: use ``githubOptions.mergify`` instead
+
+        :stability: deprecated
         '''
-        result = self._values.get("feature_flags")
+        result = self._values.get("mergify")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def require_approval(
+    def mergify_options(
         self,
-    ) -> typing.Optional[_projen_awscdk_04054675.ApprovalLevel]:
-        '''(experimental) To protect you against unintended changes that affect your security posture, the AWS CDK Toolkit prompts you to approve security-related changes before deploying them.
+    ) -> typing.Optional[_projen_github_04054675.MergifyOptions]:
+        '''(deprecated) Options for mergify.
 
-        :default: ApprovalLevel.BROADENING
+        :default: - default options
 
-        :stability: experimental
+        :deprecated: use ``githubOptions.mergifyOptions`` instead
+
+        :stability: deprecated
         '''
-        result = self._values.get("require_approval")
-        return typing.cast(typing.Optional[_projen_awscdk_04054675.ApprovalLevel], result)
+        result = self._values.get("mergify_options")
+        return typing.cast(typing.Optional[_projen_github_04054675.MergifyOptions], result)
 
     @builtins.property
-    def watch_excludes(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''(experimental) Glob patterns to exclude from ``cdk watch``.
+    def project_type(self) -> typing.Optional[_projen_04054675.ProjectType]:
+        '''(deprecated) Which type of project this is (library/app).
 
-        :default: []
+        :default: ProjectType.UNKNOWN
 
-        :stability: experimental
+        :deprecated: no longer supported at the base project level
+
+        :stability: deprecated
         '''
-        result = self._values.get("watch_excludes")
-        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+        result = self._values.get("project_type")
+        return typing.cast(typing.Optional[_projen_04054675.ProjectType], result)
 
     @builtins.property
-    def watch_includes(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''(experimental) Glob patterns to include in ``cdk watch``.
+    def projen_credentials(
+        self,
+    ) -> typing.Optional[_projen_github_04054675.GithubCredentials]:
+        '''(experimental) Choose a method of providing GitHub API access for projen workflows.
 
-        :default: []
+        :default: - use a personal access token named PROJEN_GITHUB_TOKEN
 
         :stability: experimental
         '''
-        result = self._values.get("watch_includes")
-        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+        result = self._values.get("projen_credentials")
+        return typing.cast(typing.Optional[_projen_github_04054675.GithubCredentials], result)
 
     @builtins.property
-    def cdk_version(self) -> builtins.str:
-        '''(experimental) Minimum version of the AWS CDK to depend on.
+    def projen_token_secret(self) -> typing.Optional[builtins.str]:
+        '''(deprecated) The name of a secret which includes a GitHub Personal Access Token to be used by projen workflows.
 
-        :default: "2.1.0"
+        This token needs to have the ``repo``, ``workflows``
+        and ``packages`` scope.
 
-        :stability: experimental
+        :default: "PROJEN_GITHUB_TOKEN"
+
+        :deprecated: use ``projenCredentials``
+
+        :stability: deprecated
         '''
-        result = self._values.get("cdk_version")
-        assert result is not None, "Required property 'cdk_version' is missing"
-        return typing.cast(builtins.str, result)
+        result = self._values.get("projen_token_secret")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def cdk_assert(self) -> typing.Optional[builtins.bool]:
-        '''(deprecated) Warning: NodeJS only.
+    def readme(self) -> typing.Optional[_projen_04054675.SampleReadmeProps]:
+        '''(experimental) The README setup.
 
-        Install the @aws-cdk/assert library?
+        :default: - { filename: 'README.md', contents: '# replace this' }
 
-        :default: - will be included by default for AWS CDK >= 1.0.0 < 2.0.0
+        :stability: experimental
 
-        :deprecated: The
+        Example::
 
-        :stability: deprecated
-        :aws-cdk: /assertions (in V1) and included in ``aws-cdk-lib`` for V2.
+            "{ filename: 'readme.md', contents: '# title' }"
         '''
-        result = self._values.get("cdk_assert")
-        return typing.cast(typing.Optional[builtins.bool], result)
+        result = self._values.get("readme")
+        return typing.cast(typing.Optional[_projen_04054675.SampleReadmeProps], result)
 
     @builtins.property
-    def cdk_assertions(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Install the assertions library?
+    def stale(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Auto-close of stale issues and pull request.
 
-        Only needed for CDK 1.x. If using CDK 2.x then
-        assertions is already included in 'aws-cdk-lib'
+        See ``staleOptions`` for options.
 
-        :default: - will be included by default for AWS CDK >= 1.111.0 < 2.0.0
+        :default: false
 
         :stability: experimental
         '''
-        result = self._values.get("cdk_assertions")
+        result = self._values.get("stale")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def cdk_dependencies(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''(deprecated) Which AWS CDKv1 modules this project requires.
+    def stale_options(self) -> typing.Optional[_projen_github_04054675.StaleOptions]:
+        '''(experimental) Auto-close stale issues and pull requests.
 
-        :deprecated: For CDK 2.x use "deps" instead. (or "peerDeps" if you're building a library)
+        To disable set ``stale`` to ``false``.
 
-        :stability: deprecated
+        :default: - see defaults in ``StaleOptions``
+
+        :stability: experimental
         '''
-        result = self._values.get("cdk_dependencies")
-        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+        result = self._values.get("stale_options")
+        return typing.cast(typing.Optional[_projen_github_04054675.StaleOptions], result)
 
     @builtins.property
-    def cdk_dependencies_as_deps(self) -> typing.Optional[builtins.bool]:
-        '''(deprecated) If this is enabled (default), all modules declared in ``cdkDependencies`` will be also added as normal ``dependencies`` (as well as ``peerDependencies``).
-
-        This is to ensure that downstream consumers actually have your CDK dependencies installed
-        when using npm < 7 or yarn, where peer dependencies are not automatically installed.
-        If this is disabled, ``cdkDependencies`` will be added to ``devDependencies`` to ensure
-        they are present during development.
+    def vscode(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Enable VSCode integration.
 
-        Note: this setting only applies to construct library projects
+        Enabled by default for root projects. Disabled for non-root projects.
 
         :default: true
 
-        :deprecated: Not supported in CDK v2.
-
-        :stability: deprecated
+        :stability: experimental
         '''
-        result = self._values.get("cdk_dependencies_as_deps")
+        result = self._values.get("vscode")
         return typing.cast(typing.Optional[builtins.bool], result)
 
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "GoAppOptions(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class GoProject(
+    _projen_04054675.Project,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="butterneck-projen.GoProject",
+):
+    def __init__(
+        self,
+        *,
+        name: builtins.str,
+        commit_generated: typing.Optional[builtins.bool] = None,
+        git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        logging: typing.Optional[typing.Union[_projen_04054675.LoggerOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        outdir: typing.Optional[builtins.str] = None,
+        parent: typing.Optional[_projen_04054675.Project] = None,
+        projen_command: typing.Optional[builtins.str] = None,
+        projenrc_json: typing.Optional[builtins.bool] = None,
+        projenrc_json_options: typing.Optional[typing.Union[_projen_04054675.ProjenrcJsonOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        renovatebot: typing.Optional[builtins.bool] = None,
+        renovatebot_options: typing.Optional[typing.Union[_projen_04054675.RenovatebotOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> None:
+        '''
+        :param name: (experimental) This is the name of your project. Default: $BASEDIR
+        :param commit_generated: (experimental) Whether to commit the managed files by default. Default: true
+        :param git_ignore_options: (experimental) Configuration options for .gitignore file.
+        :param git_options: (experimental) Configuration options for git.
+        :param logging: (experimental) Configure logging options such as verbosity. Default: {}
+        :param outdir: (experimental) The root directory of the project. Relative to this directory, all files are synthesized. If this project has a parent, this directory is relative to the parent directory and it cannot be the same as the parent or any of it's other sub-projects. Default: "."
+        :param parent: (experimental) The parent project, if this project is part of a bigger project.
+        :param projen_command: (experimental) The shell command to use in order to run the projen CLI. Can be used to customize in special environments. Default: "npx projen"
+        :param projenrc_json: (experimental) Generate (once) .projenrc.json (in JSON). Set to ``false`` in order to disable .projenrc.json generation. Default: false
+        :param projenrc_json_options: (experimental) Options for .projenrc.json. Default: - default options
+        :param renovatebot: (experimental) Use renovatebot to handle dependency upgrades. Default: false
+        :param renovatebot_options: (experimental) Options for renovatebot. Default: - default options
+        '''
+        options = GoProjectOptions(
+            name=name,
+            commit_generated=commit_generated,
+            git_ignore_options=git_ignore_options,
+            git_options=git_options,
+            logging=logging,
+            outdir=outdir,
+            parent=parent,
+            projen_command=projen_command,
+            projenrc_json=projenrc_json,
+            projenrc_json_options=projenrc_json_options,
+            renovatebot=renovatebot,
+            renovatebot_options=renovatebot_options,
+        )
+
+        jsii.create(self.__class__, self, [options])
+
+
+@jsii.data_type(
+    jsii_type="butterneck-projen.GoProjectOptions",
+    jsii_struct_bases=[_projen_04054675.ProjectOptions],
+    name_mapping={
+        "name": "name",
+        "commit_generated": "commitGenerated",
+        "git_ignore_options": "gitIgnoreOptions",
+        "git_options": "gitOptions",
+        "logging": "logging",
+        "outdir": "outdir",
+        "parent": "parent",
+        "projen_command": "projenCommand",
+        "projenrc_json": "projenrcJson",
+        "projenrc_json_options": "projenrcJsonOptions",
+        "renovatebot": "renovatebot",
+        "renovatebot_options": "renovatebotOptions",
+    },
+)
+class GoProjectOptions(_projen_04054675.ProjectOptions):
+    def __init__(
+        self,
+        *,
+        name: builtins.str,
+        commit_generated: typing.Optional[builtins.bool] = None,
+        git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        logging: typing.Optional[typing.Union[_projen_04054675.LoggerOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        outdir: typing.Optional[builtins.str] = None,
+        parent: typing.Optional[_projen_04054675.Project] = None,
+        projen_command: typing.Optional[builtins.str] = None,
+        projenrc_json: typing.Optional[builtins.bool] = None,
+        projenrc_json_options: typing.Optional[typing.Union[_projen_04054675.ProjenrcJsonOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        renovatebot: typing.Optional[builtins.bool] = None,
+        renovatebot_options: typing.Optional[typing.Union[_projen_04054675.RenovatebotOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> None:
+        '''
+        :param name: (experimental) This is the name of your project. Default: $BASEDIR
+        :param commit_generated: (experimental) Whether to commit the managed files by default. Default: true
+        :param git_ignore_options: (experimental) Configuration options for .gitignore file.
+        :param git_options: (experimental) Configuration options for git.
+        :param logging: (experimental) Configure logging options such as verbosity. Default: {}
+        :param outdir: (experimental) The root directory of the project. Relative to this directory, all files are synthesized. If this project has a parent, this directory is relative to the parent directory and it cannot be the same as the parent or any of it's other sub-projects. Default: "."
+        :param parent: (experimental) The parent project, if this project is part of a bigger project.
+        :param projen_command: (experimental) The shell command to use in order to run the projen CLI. Can be used to customize in special environments. Default: "npx projen"
+        :param projenrc_json: (experimental) Generate (once) .projenrc.json (in JSON). Set to ``false`` in order to disable .projenrc.json generation. Default: false
+        :param projenrc_json_options: (experimental) Options for .projenrc.json. Default: - default options
+        :param renovatebot: (experimental) Use renovatebot to handle dependency upgrades. Default: false
+        :param renovatebot_options: (experimental) Options for renovatebot. Default: - default options
+        '''
+        if isinstance(git_ignore_options, dict):
+            git_ignore_options = _projen_04054675.IgnoreFileOptions(**git_ignore_options)
+        if isinstance(git_options, dict):
+            git_options = _projen_04054675.GitOptions(**git_options)
+        if isinstance(logging, dict):
+            logging = _projen_04054675.LoggerOptions(**logging)
+        if isinstance(projenrc_json_options, dict):
+            projenrc_json_options = _projen_04054675.ProjenrcJsonOptions(**projenrc_json_options)
+        if isinstance(renovatebot_options, dict):
+            renovatebot_options = _projen_04054675.RenovatebotOptions(**renovatebot_options)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__72fce2395af7766c8e6208e5ab5a770a8984251849b99f5975fe6ba624a144cb)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument commit_generated", value=commit_generated, expected_type=type_hints["commit_generated"])
+            check_type(argname="argument git_ignore_options", value=git_ignore_options, expected_type=type_hints["git_ignore_options"])
+            check_type(argname="argument git_options", value=git_options, expected_type=type_hints["git_options"])
+            check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
+            check_type(argname="argument outdir", value=outdir, expected_type=type_hints["outdir"])
+            check_type(argname="argument parent", value=parent, expected_type=type_hints["parent"])
+            check_type(argname="argument projen_command", value=projen_command, expected_type=type_hints["projen_command"])
+            check_type(argname="argument projenrc_json", value=projenrc_json, expected_type=type_hints["projenrc_json"])
+            check_type(argname="argument projenrc_json_options", value=projenrc_json_options, expected_type=type_hints["projenrc_json_options"])
+            check_type(argname="argument renovatebot", value=renovatebot, expected_type=type_hints["renovatebot"])
+            check_type(argname="argument renovatebot_options", value=renovatebot_options, expected_type=type_hints["renovatebot_options"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "name": name,
+        }
+        if commit_generated is not None:
+            self._values["commit_generated"] = commit_generated
+        if git_ignore_options is not None:
+            self._values["git_ignore_options"] = git_ignore_options
+        if git_options is not None:
+            self._values["git_options"] = git_options
+        if logging is not None:
+            self._values["logging"] = logging
+        if outdir is not None:
+            self._values["outdir"] = outdir
+        if parent is not None:
+            self._values["parent"] = parent
+        if projen_command is not None:
+            self._values["projen_command"] = projen_command
+        if projenrc_json is not None:
+            self._values["projenrc_json"] = projenrc_json
+        if projenrc_json_options is not None:
+            self._values["projenrc_json_options"] = projenrc_json_options
+        if renovatebot is not None:
+            self._values["renovatebot"] = renovatebot
+        if renovatebot_options is not None:
+            self._values["renovatebot_options"] = renovatebot_options
+
     @builtins.property
-    def cdk_test_dependencies(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''(deprecated) AWS CDK modules required for testing.
+    def name(self) -> builtins.str:
+        '''(experimental) This is the name of your project.
 
-        :deprecated: For CDK 2.x use 'devDeps' (in node.js projects) or 'testDeps' (in java projects) instead
+        :default: $BASEDIR
 
-        :stability: deprecated
+        :stability: experimental
+        :featured: true
         '''
-        result = self._values.get("cdk_test_dependencies")
-        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+        result = self._values.get("name")
+        assert result is not None, "Required property 'name' is missing"
+        return typing.cast(builtins.str, result)
 
     @builtins.property
-    def cdk_version_pinning(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Use pinned version instead of caret version for CDK.
+    def commit_generated(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Whether to commit the managed files by default.
 
-        You can use this to prevent mixed versions for your CDK dependencies and to prevent auto-updates.
-        If you use experimental features this will let you define the moment you include breaking changes.
+        :default: true
 
         :stability: experimental
         '''
-        result = self._values.get("cdk_version_pinning")
+        result = self._values.get("commit_generated")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def constructs_version(self) -> typing.Optional[builtins.str]:
-        '''(experimental) Minimum version of the ``constructs`` library to depend on.
+    def git_ignore_options(self) -> typing.Optional[_projen_04054675.IgnoreFileOptions]:
+        '''(experimental) Configuration options for .gitignore file.
 
-        :default:
+        :stability: experimental
+        '''
+        result = self._values.get("git_ignore_options")
+        return typing.cast(typing.Optional[_projen_04054675.IgnoreFileOptions], result)
 
-        - for CDK 1.x the default is "3.2.27", for CDK 2.x the default is
-        "10.0.5".
+    @builtins.property
+    def git_options(self) -> typing.Optional[_projen_04054675.GitOptions]:
+        '''(experimental) Configuration options for git.
 
         :stability: experimental
         '''
-        result = self._values.get("constructs_version")
-        return typing.cast(typing.Optional[builtins.str], result)
+        result = self._values.get("git_options")
+        return typing.cast(typing.Optional[_projen_04054675.GitOptions], result)
 
     @builtins.property
-    def app_entrypoint(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The CDK app's entrypoint (relative to the source directory, which is "src" by default).
+    def logging(self) -> typing.Optional[_projen_04054675.LoggerOptions]:
+        '''(experimental) Configure logging options such as verbosity.
 
-        :default: "app.py"
+        :default: {}
 
         :stability: experimental
         '''
-        result = self._values.get("app_entrypoint")
+        result = self._values.get("logging")
+        return typing.cast(typing.Optional[_projen_04054675.LoggerOptions], result)
+
+    @builtins.property
+    def outdir(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The root directory of the project.
+
+        Relative to this directory, all files are synthesized.
+
+        If this project has a parent, this directory is relative to the parent
+        directory and it cannot be the same as the parent or any of it's other
+        sub-projects.
+
+        :default: "."
+
+        :stability: experimental
+        '''
+        result = self._values.get("outdir")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def testdir(self) -> typing.Optional[builtins.str]:
-        '''(experimental) Python sources directory.
+    def parent(self) -> typing.Optional[_projen_04054675.Project]:
+        '''(experimental) The parent project, if this project is part of a bigger project.
+
+        :stability: experimental
+        '''
+        result = self._values.get("parent")
+        return typing.cast(typing.Optional[_projen_04054675.Project], result)
+
+    @builtins.property
+    def projen_command(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The shell command to use in order to run the projen CLI.
 
-        :default: "tests"
+        Can be used to customize in special environments.
+
+        :default: "npx projen"
 
         :stability: experimental
         '''
-        result = self._values.get("testdir")
+        result = self._values.get("projen_command")
         return typing.cast(typing.Optional[builtins.str], result)
 
+    @builtins.property
+    def projenrc_json(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Generate (once) .projenrc.json (in JSON). Set to ``false`` in order to disable .projenrc.json generation.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("projenrc_json")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def projenrc_json_options(
+        self,
+    ) -> typing.Optional[_projen_04054675.ProjenrcJsonOptions]:
+        '''(experimental) Options for .projenrc.json.
+
+        :default: - default options
+
+        :stability: experimental
+        '''
+        result = self._values.get("projenrc_json_options")
+        return typing.cast(typing.Optional[_projen_04054675.ProjenrcJsonOptions], result)
+
+    @builtins.property
+    def renovatebot(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Use renovatebot to handle dependency upgrades.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("renovatebot")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def renovatebot_options(
+        self,
+    ) -> typing.Optional[_projen_04054675.RenovatebotOptions]:
+        '''(experimental) Options for renovatebot.
+
+        :default: - default options
+
+        :stability: experimental
+        '''
+        result = self._values.get("renovatebot_options")
+        return typing.cast(typing.Optional[_projen_04054675.RenovatebotOptions], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "GoAppOptions(%s)" % ", ".join(
+        return "GoProjectOptions(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
+    "ButterneckAwsCdkPythonApp",
+    "ButterneckAwsCdkPythonAppOptions",
     "GoApp",
     "GoAppOptions",
+    "GoProject",
+    "GoProjectOptions",
 ]
 
 publication.publish()
 
-def _typecheckingstub__e7cdfb665920a033d76499e282ce137ada7759e9a66b20380e8aae21552e8eb6(
+def _typecheckingstub__28b6701892490b47b0967137d9b99f87f1f16c1b4caa7d15fdcda3eb0e7ac579(
     *,
     name: builtins.str,
     commit_generated: typing.Optional[builtins.bool] = None,
     git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     logging: typing.Optional[typing.Union[_projen_04054675.LoggerOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     outdir: typing.Optional[builtins.str] = None,
@@ -1703,54 +2094,90 @@
     project_type: typing.Optional[_projen_04054675.ProjectType] = None,
     projen_credentials: typing.Optional[_projen_github_04054675.GithubCredentials] = None,
     projen_token_secret: typing.Optional[builtins.str] = None,
     readme: typing.Optional[typing.Union[_projen_04054675.SampleReadmeProps, typing.Dict[builtins.str, typing.Any]]] = None,
     stale: typing.Optional[builtins.bool] = None,
     stale_options: typing.Optional[typing.Union[_projen_github_04054675.StaleOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     vscode: typing.Optional[builtins.bool] = None,
-    author_email: builtins.str,
-    author_name: builtins.str,
-    version: builtins.str,
-    classifiers: typing.Optional[typing.Sequence[builtins.str]] = None,
-    description: typing.Optional[builtins.str] = None,
-    homepage: typing.Optional[builtins.str] = None,
-    license: typing.Optional[builtins.str] = None,
-    package_name: typing.Optional[builtins.str] = None,
-    poetry_options: typing.Optional[typing.Union[_projen_python_04054675.PoetryPyprojectOptionsWithoutDeps, typing.Dict[builtins.str, typing.Any]]] = None,
-    setup_config: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
-    module_name: builtins.str,
-    deps: typing.Optional[typing.Sequence[builtins.str]] = None,
-    dev_deps: typing.Optional[typing.Sequence[builtins.str]] = None,
-    pip: typing.Optional[builtins.bool] = None,
-    poetry: typing.Optional[builtins.bool] = None,
-    projenrc_js: typing.Optional[builtins.bool] = None,
-    projenrc_js_options: typing.Optional[typing.Union[_projen_javascript_04054675.ProjenrcOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    projenrc_python: typing.Optional[builtins.bool] = None,
-    projenrc_python_options: typing.Optional[typing.Union[_projen_python_04054675.ProjenrcOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    projenrc_ts: typing.Optional[builtins.bool] = None,
-    projenrc_ts_options: typing.Optional[typing.Union[_projen_typescript_04054675.ProjenrcTsOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    pytest: typing.Optional[builtins.bool] = None,
-    pytest_options: typing.Optional[typing.Union[_projen_python_04054675.PytestOptions, typing.Dict[builtins.str, typing.Any]]] = None,
-    sample: typing.Optional[builtins.bool] = None,
-    setuptools: typing.Optional[builtins.bool] = None,
-    venv: typing.Optional[builtins.bool] = None,
-    venv_options: typing.Optional[typing.Union[_projen_python_04054675.VenvOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     build_command: typing.Optional[builtins.str] = None,
     cdkout: typing.Optional[builtins.str] = None,
     context: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     feature_flags: typing.Optional[builtins.bool] = None,
     require_approval: typing.Optional[_projen_awscdk_04054675.ApprovalLevel] = None,
     watch_excludes: typing.Optional[typing.Sequence[builtins.str]] = None,
     watch_includes: typing.Optional[typing.Sequence[builtins.str]] = None,
-    cdk_version: builtins.str,
-    cdk_assert: typing.Optional[builtins.bool] = None,
-    cdk_assertions: typing.Optional[builtins.bool] = None,
-    cdk_dependencies: typing.Optional[typing.Sequence[builtins.str]] = None,
-    cdk_dependencies_as_deps: typing.Optional[builtins.bool] = None,
-    cdk_test_dependencies: typing.Optional[typing.Sequence[builtins.str]] = None,
-    cdk_version_pinning: typing.Optional[builtins.bool] = None,
+    author_email: typing.Optional[builtins.str] = None,
+    author_name: typing.Optional[builtins.str] = None,
+    cdk_version: typing.Optional[builtins.str] = None,
     constructs_version: typing.Optional[builtins.str] = None,
-    app_entrypoint: typing.Optional[builtins.str] = None,
-    testdir: typing.Optional[builtins.str] = None,
+    deps: typing.Optional[typing.Sequence[builtins.str]] = None,
+    dev_deps: typing.Optional[typing.Sequence[builtins.str]] = None,
+    module_name: typing.Optional[builtins.str] = None,
+    version: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ee2b3fdb8f9ae93e4279d52a15be8cf3032f8d86cb8a72fb7689c506e4e7d855(
+    value: ButterneckAwsCdkPythonApp,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__217b491360c87c72aaa4ea7ba8a3f98bf9c840fbb010f10d9d1abfee2516eec2(
+    value: GoProject,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e7cdfb665920a033d76499e282ce137ada7759e9a66b20380e8aae21552e8eb6(
+    *,
+    name: builtins.str,
+    commit_generated: typing.Optional[builtins.bool] = None,
+    git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    logging: typing.Optional[typing.Union[_projen_04054675.LoggerOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    outdir: typing.Optional[builtins.str] = None,
+    parent: typing.Optional[_projen_04054675.Project] = None,
+    projen_command: typing.Optional[builtins.str] = None,
+    projenrc_json: typing.Optional[builtins.bool] = None,
+    projenrc_json_options: typing.Optional[typing.Union[_projen_04054675.ProjenrcJsonOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    renovatebot: typing.Optional[builtins.bool] = None,
+    renovatebot_options: typing.Optional[typing.Union[_projen_04054675.RenovatebotOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    auto_approve_options: typing.Optional[typing.Union[_projen_github_04054675.AutoApproveOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    auto_merge: typing.Optional[builtins.bool] = None,
+    auto_merge_options: typing.Optional[typing.Union[_projen_github_04054675.AutoMergeOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    clobber: typing.Optional[builtins.bool] = None,
+    dev_container: typing.Optional[builtins.bool] = None,
+    github: typing.Optional[builtins.bool] = None,
+    github_options: typing.Optional[typing.Union[_projen_github_04054675.GitHubOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    gitpod: typing.Optional[builtins.bool] = None,
+    mergify: typing.Optional[builtins.bool] = None,
+    mergify_options: typing.Optional[typing.Union[_projen_github_04054675.MergifyOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    project_type: typing.Optional[_projen_04054675.ProjectType] = None,
+    projen_credentials: typing.Optional[_projen_github_04054675.GithubCredentials] = None,
+    projen_token_secret: typing.Optional[builtins.str] = None,
+    readme: typing.Optional[typing.Union[_projen_04054675.SampleReadmeProps, typing.Dict[builtins.str, typing.Any]]] = None,
+    stale: typing.Optional[builtins.bool] = None,
+    stale_options: typing.Optional[typing.Union[_projen_github_04054675.StaleOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    vscode: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__72fce2395af7766c8e6208e5ab5a770a8984251849b99f5975fe6ba624a144cb(
+    *,
+    name: builtins.str,
+    commit_generated: typing.Optional[builtins.bool] = None,
+    git_ignore_options: typing.Optional[typing.Union[_projen_04054675.IgnoreFileOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    git_options: typing.Optional[typing.Union[_projen_04054675.GitOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    logging: typing.Optional[typing.Union[_projen_04054675.LoggerOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    outdir: typing.Optional[builtins.str] = None,
+    parent: typing.Optional[_projen_04054675.Project] = None,
+    projen_command: typing.Optional[builtins.str] = None,
+    projenrc_json: typing.Optional[builtins.bool] = None,
+    projenrc_json_options: typing.Optional[typing.Union[_projen_04054675.ProjenrcJsonOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    renovatebot: typing.Optional[builtins.bool] = None,
+    renovatebot_options: typing.Optional[typing.Union[_projen_04054675.RenovatebotOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `butterneck-projen-0.0.4/src/butterneck_projen.egg-info/PKG-INFO` & `butterneck-projen-0.0.5/src/butterneck_projen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butterneck-projen
-Version: 0.0.4
+Version: 0.0.5
 Summary: butterneck-projen
 Home-page: https://github.com/butterneck/butterneck-projen.git
 Author: Filippo Pinton<pinton.filippo@protonmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/butterneck/butterneck-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

