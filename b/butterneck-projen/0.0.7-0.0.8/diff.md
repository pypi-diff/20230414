# Comparing `tmp/butterneck-projen-0.0.7.tar.gz` & `tmp/butterneck-projen-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butterneck-projen-0.0.7.tar", last modified: Fri Apr 14 20:33:14 2023, max compression
+gzip compressed data, was "butterneck-projen-0.0.8.tar", last modified: Fri Apr 14 21:24:21 2023, max compression
```

## Comparing `butterneck-projen-0.0.7.tar` & `butterneck-projen-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:14.746700 butterneck-projen-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 20:33:14.746700 butterneck-projen-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 20:33:14.746700 butterneck-projen-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:14.742700 butterneck-projen-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:14.742700 butterneck-projen-0.0.7/src/butterneck_projen/
--rw-r--r--   0 runner    (1001) docker     (123)   113875 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/src/butterneck_projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:14.742700 butterneck-projen-0.0.7/src/butterneck_projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/src/butterneck_projen/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24872 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/src/butterneck_projen/_jsii/butterneck-projen@0.0.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/src/butterneck_projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:14.742700 butterneck-projen-0.0.7/src/butterneck_projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 20:33:14.000000 butterneck-projen-0.0.7/src/butterneck_projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-14 20:33:14.000000 butterneck-projen-0.0.7/src/butterneck_projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:33:14.000000 butterneck-projen-0.0.7/src/butterneck_projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 20:33:14.000000 butterneck-projen-0.0.7/src/butterneck_projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 20:33:14.000000 butterneck-projen-0.0.7/src/butterneck_projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:24:21.156535 butterneck-projen-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 21:24:09.000000 butterneck-projen-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 21:24:09.000000 butterneck-projen-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 21:24:21.156535 butterneck-projen-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 21:24:09.000000 butterneck-projen-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 21:24:09.000000 butterneck-projen-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:24:21.156535 butterneck-projen-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-14 21:24:09.000000 butterneck-projen-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:24:21.156535 butterneck-projen-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:24:21.156535 butterneck-projen-0.0.8/src/butterneck_projen/
+-rw-r--r--   0 runner    (1001) docker     (123)   115515 2023-04-14 21:24:09.000000 butterneck-projen-0.0.8/src/butterneck_projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:24:21.156535 butterneck-projen-0.0.8/src/butterneck_projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-14 21:24:09.000000 butterneck-projen-0.0.8/src/butterneck_projen/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25219 2023-04-14 21:24:09.000000 butterneck-projen-0.0.8/src/butterneck_projen/_jsii/butterneck-projen@0.0.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:24:09.000000 butterneck-projen-0.0.8/src/butterneck_projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:24:21.156535 butterneck-projen-0.0.8/src/butterneck_projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 21:24:21.000000 butterneck-projen-0.0.8/src/butterneck_projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-14 21:24:21.000000 butterneck-projen-0.0.8/src/butterneck_projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:24:21.000000 butterneck-projen-0.0.8/src/butterneck_projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 21:24:21.000000 butterneck-projen-0.0.8/src/butterneck_projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 21:24:21.000000 butterneck-projen-0.0.8/src/butterneck_projen.egg-info/top_level.txt
```

### Comparing `butterneck-projen-0.0.7/LICENSE` & `butterneck-projen-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `butterneck-projen-0.0.7/PKG-INFO` & `butterneck-projen-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butterneck-projen
-Version: 0.0.7
+Version: 0.0.8
 Summary: butterneck-projen
 Home-page: https://github.com/butterneck/butterneck-projen.git
 Author: Filippo Pinton<pinton.filippo@protonmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/butterneck/butterneck-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `butterneck-projen-0.0.7/setup.py` & `butterneck-projen-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "butterneck-projen",
-    "version": "0.0.7",
+    "version": "0.0.8",
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
-            "butterneck-projen@0.0.7.jsii.tgz"
+            "butterneck-projen@0.0.8.jsii.tgz"
         ],
         "butterneck_projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `butterneck-projen-0.0.7/src/butterneck_projen/__init__.py` & `butterneck-projen-0.0.8/src/butterneck_projen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1051,14 +1051,16 @@
     :extends: awscdk.AwsCdkPythonApp *
     :pjid: go-app
     '''
 
     def __init__(
         self,
         *,
+        infra: typing.Union[ButterneckAwsCdkPythonAppOptions, typing.Dict[builtins.str, typing.Any]],
+        service: typing.Union["GoProjectOptions", typing.Dict[builtins.str, typing.Any]],
         auto_approve_options: typing.Optional[typing.Union[_projen_github_04054675.AutoApproveOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         auto_merge: typing.Optional[builtins.bool] = None,
         auto_merge_options: typing.Optional[typing.Union[_projen_github_04054675.AutoMergeOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         clobber: typing.Optional[builtins.bool] = None,
         dev_container: typing.Optional[builtins.bool] = None,
         github: typing.Optional[builtins.bool] = None,
         github_options: typing.Optional[typing.Union[_projen_github_04054675.GitHubOptions, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -1082,14 +1084,16 @@
         projen_command: typing.Optional[builtins.str] = None,
         projenrc_json: typing.Optional[builtins.bool] = None,
         projenrc_json_options: typing.Optional[typing.Union[_projen_04054675.ProjenrcJsonOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         renovatebot: typing.Optional[builtins.bool] = None,
         renovatebot_options: typing.Optional[typing.Union[_projen_04054675.RenovatebotOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
+        :param infra: 
+        :param service: 
         :param auto_approve_options: (experimental) Enable and configure the 'auto approve' workflow. Default: - auto approve is disabled
         :param auto_merge: (experimental) Enable automatic merging on GitHub. Has no effect if ``github.mergify`` is set to false. Default: true
         :param auto_merge_options: (experimental) Configure options for automatic merging on GitHub. Has no effect if ``github.mergify`` or ``autoMerge`` is set to false. Default: - see defaults in ``AutoMergeOptions``
         :param clobber: (experimental) Add a ``clobber`` task which resets the repo to origin. Default: - true, but false for subprojects
         :param dev_container: (experimental) Add a VSCode development environment (used for GitHub Codespaces). Default: false
         :param github: (experimental) Enable GitHub integration. Enabled by default for root projects. Disabled for non-root projects. Default: true
         :param github_options: (experimental) Options for GitHub integration. Default: - see GitHubOptions
@@ -1113,14 +1117,16 @@
         :param projen_command: (experimental) The shell command to use in order to run the projen CLI. Can be used to customize in special environments. Default: "npx projen"
         :param projenrc_json: (experimental) Generate (once) .projenrc.json (in JSON). Set to ``false`` in order to disable .projenrc.json generation. Default: false
         :param projenrc_json_options: (experimental) Options for .projenrc.json. Default: - default options
         :param renovatebot: (experimental) Use renovatebot to handle dependency upgrades. Default: false
         :param renovatebot_options: (experimental) Options for renovatebot. Default: - default options
         '''
         options = GoAppOptions(
+            infra=infra,
+            service=service,
             auto_approve_options=auto_approve_options,
             auto_merge=auto_merge,
             auto_merge_options=auto_merge_options,
             clobber=clobber,
             dev_container=dev_container,
             github=github,
             github_options=github_options,
@@ -1147,36 +1153,36 @@
             renovatebot=renovatebot,
             renovatebot_options=renovatebot_options,
         )
 
         jsii.create(self.__class__, self, [options])
 
     @builtins.property
-    @jsii.member(jsii_name="infraProject")
-    def infra_project(self) -> ButterneckAwsCdkPythonApp:
-        return typing.cast(ButterneckAwsCdkPythonApp, jsii.get(self, "infraProject"))
+    @jsii.member(jsii_name="infra")
+    def infra(self) -> ButterneckAwsCdkPythonApp:
+        return typing.cast(ButterneckAwsCdkPythonApp, jsii.get(self, "infra"))
 
-    @infra_project.setter
-    def infra_project(self, value: ButterneckAwsCdkPythonApp) -> None:
+    @infra.setter
+    def infra(self, value: ButterneckAwsCdkPythonApp) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ee2b3fdb8f9ae93e4279d52a15be8cf3032f8d86cb8a72fb7689c506e4e7d855)
+            type_hints = typing.get_type_hints(_typecheckingstub__111fbf673ea1b0b511acad36d5a4fe59e13d4492686de349d3ec27f6228a6171)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "infraProject", value)
+        jsii.set(self, "infra", value)
 
     @builtins.property
-    @jsii.member(jsii_name="serviceProject")
-    def service_project(self) -> "GoProject":
-        return typing.cast("GoProject", jsii.get(self, "serviceProject"))
+    @jsii.member(jsii_name="service")
+    def service(self) -> "GoProject":
+        return typing.cast("GoProject", jsii.get(self, "service"))
 
-    @service_project.setter
-    def service_project(self, value: "GoProject") -> None:
+    @service.setter
+    def service(self, value: "GoProject") -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__217b491360c87c72aaa4ea7ba8a3f98bf9c840fbb010f10d9d1abfee2516eec2)
+            type_hints = typing.get_type_hints(_typecheckingstub__54f43a61651d68bba5ff6149a4776c9e1b303b1e1b02a95e789902b97a7d36a3)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "serviceProject", value)
+        jsii.set(self, "service", value)
 
 
 @jsii.data_type(
     jsii_type="butterneck-projen.GoAppOptions",
     jsii_struct_bases=[_projen_github_04054675.GitHubProjectOptions],
     name_mapping={
         "name": "name",
@@ -1204,14 +1210,16 @@
         "project_type": "projectType",
         "projen_credentials": "projenCredentials",
         "projen_token_secret": "projenTokenSecret",
         "readme": "readme",
         "stale": "stale",
         "stale_options": "staleOptions",
         "vscode": "vscode",
+        "infra": "infra",
+        "service": "service",
     },
 )
 class GoAppOptions(_projen_github_04054675.GitHubProjectOptions):
     def __init__(
         self,
         *,
         name: builtins.str,
@@ -1239,14 +1247,16 @@
         project_type: typing.Optional[_projen_04054675.ProjectType] = None,
         projen_credentials: typing.Optional[_projen_github_04054675.GithubCredentials] = None,
         projen_token_secret: typing.Optional[builtins.str] = None,
         readme: typing.Optional[typing.Union[_projen_04054675.SampleReadmeProps, typing.Dict[builtins.str, typing.Any]]] = None,
         stale: typing.Optional[builtins.bool] = None,
         stale_options: typing.Optional[typing.Union[_projen_github_04054675.StaleOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         vscode: typing.Optional[builtins.bool] = None,
+        infra: typing.Union[ButterneckAwsCdkPythonAppOptions, typing.Dict[builtins.str, typing.Any]],
+        service: typing.Union["GoProjectOptions", typing.Dict[builtins.str, typing.Any]],
     ) -> None:
         '''
         :param name: (experimental) This is the name of your project. Default: $BASEDIR
         :param commit_generated: (experimental) Whether to commit the managed files by default. Default: true
         :param git_ignore_options: (experimental) Configuration options for .gitignore file.
         :param git_options: (experimental) Configuration options for git.
         :param logging: (experimental) Configure logging options such as verbosity. Default: {}
@@ -1270,14 +1280,16 @@
         :param project_type: (deprecated) Which type of project this is (library/app). Default: ProjectType.UNKNOWN
         :param projen_credentials: (experimental) Choose a method of providing GitHub API access for projen workflows. Default: - use a personal access token named PROJEN_GITHUB_TOKEN
         :param projen_token_secret: (deprecated) The name of a secret which includes a GitHub Personal Access Token to be used by projen workflows. This token needs to have the ``repo``, ``workflows`` and ``packages`` scope. Default: "PROJEN_GITHUB_TOKEN"
         :param readme: (experimental) The README setup. Default: - { filename: 'README.md', contents: '# replace this' }
         :param stale: (experimental) Auto-close of stale issues and pull request. See ``staleOptions`` for options. Default: false
         :param stale_options: (experimental) Auto-close stale issues and pull requests. To disable set ``stale`` to ``false``. Default: - see defaults in ``StaleOptions``
         :param vscode: (experimental) Enable VSCode integration. Enabled by default for root projects. Disabled for non-root projects. Default: true
+        :param infra: 
+        :param service: 
         '''
         if isinstance(git_ignore_options, dict):
             git_ignore_options = _projen_04054675.IgnoreFileOptions(**git_ignore_options)
         if isinstance(git_options, dict):
             git_options = _projen_04054675.GitOptions(**git_options)
         if isinstance(logging, dict):
             logging = _projen_04054675.LoggerOptions(**logging)
@@ -1293,14 +1305,18 @@
             github_options = _projen_github_04054675.GitHubOptions(**github_options)
         if isinstance(mergify_options, dict):
             mergify_options = _projen_github_04054675.MergifyOptions(**mergify_options)
         if isinstance(readme, dict):
             readme = _projen_04054675.SampleReadmeProps(**readme)
         if isinstance(stale_options, dict):
             stale_options = _projen_github_04054675.StaleOptions(**stale_options)
+        if isinstance(infra, dict):
+            infra = ButterneckAwsCdkPythonAppOptions(**infra)
+        if isinstance(service, dict):
+            service = GoProjectOptions(**service)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e7cdfb665920a033d76499e282ce137ada7759e9a66b20380e8aae21552e8eb6)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument commit_generated", value=commit_generated, expected_type=type_hints["commit_generated"])
             check_type(argname="argument git_ignore_options", value=git_ignore_options, expected_type=type_hints["git_ignore_options"])
             check_type(argname="argument git_options", value=git_options, expected_type=type_hints["git_options"])
             check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
@@ -1324,16 +1340,20 @@
             check_type(argname="argument project_type", value=project_type, expected_type=type_hints["project_type"])
             check_type(argname="argument projen_credentials", value=projen_credentials, expected_type=type_hints["projen_credentials"])
             check_type(argname="argument projen_token_secret", value=projen_token_secret, expected_type=type_hints["projen_token_secret"])
             check_type(argname="argument readme", value=readme, expected_type=type_hints["readme"])
             check_type(argname="argument stale", value=stale, expected_type=type_hints["stale"])
             check_type(argname="argument stale_options", value=stale_options, expected_type=type_hints["stale_options"])
             check_type(argname="argument vscode", value=vscode, expected_type=type_hints["vscode"])
+            check_type(argname="argument infra", value=infra, expected_type=type_hints["infra"])
+            check_type(argname="argument service", value=service, expected_type=type_hints["service"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "name": name,
+            "infra": infra,
+            "service": service,
         }
         if commit_generated is not None:
             self._values["commit_generated"] = commit_generated
         if git_ignore_options is not None:
             self._values["git_ignore_options"] = git_ignore_options
         if git_options is not None:
             self._values["git_options"] = git_options
@@ -1748,14 +1768,26 @@
         :default: true
 
         :stability: experimental
         '''
         result = self._values.get("vscode")
         return typing.cast(typing.Optional[builtins.bool], result)
 
+    @builtins.property
+    def infra(self) -> ButterneckAwsCdkPythonAppOptions:
+        result = self._values.get("infra")
+        assert result is not None, "Required property 'infra' is missing"
+        return typing.cast(ButterneckAwsCdkPythonAppOptions, result)
+
+    @builtins.property
+    def service(self) -> "GoProjectOptions":
+        result = self._values.get("service")
+        assert result is not None, "Required property 'service' is missing"
+        return typing.cast("GoProjectOptions", result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -2138,21 +2170,21 @@
     dev_deps: typing.Optional[typing.Sequence[builtins.str]] = None,
     module_name: typing.Optional[builtins.str] = None,
     version: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ee2b3fdb8f9ae93e4279d52a15be8cf3032f8d86cb8a72fb7689c506e4e7d855(
+def _typecheckingstub__111fbf673ea1b0b511acad36d5a4fe59e13d4492686de349d3ec27f6228a6171(
     value: ButterneckAwsCdkPythonApp,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__217b491360c87c72aaa4ea7ba8a3f98bf9c840fbb010f10d9d1abfee2516eec2(
+def _typecheckingstub__54f43a61651d68bba5ff6149a4776c9e1b303b1e1b02a95e789902b97a7d36a3(
     value: GoProject,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__e7cdfb665920a033d76499e282ce137ada7759e9a66b20380e8aae21552e8eb6(
     *,
@@ -2181,14 +2213,16 @@
     project_type: typing.Optional[_projen_04054675.ProjectType] = None,
     projen_credentials: typing.Optional[_projen_github_04054675.GithubCredentials] = None,
     projen_token_secret: typing.Optional[builtins.str] = None,
     readme: typing.Optional[typing.Union[_projen_04054675.SampleReadmeProps, typing.Dict[builtins.str, typing.Any]]] = None,
     stale: typing.Optional[builtins.bool] = None,
     stale_options: typing.Optional[typing.Union[_projen_github_04054675.StaleOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     vscode: typing.Optional[builtins.bool] = None,
+    infra: typing.Union[ButterneckAwsCdkPythonAppOptions, typing.Dict[builtins.str, typing.Any]],
+    service: typing.Union[GoProjectOptions, typing.Dict[builtins.str, typing.Any]],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__72fce2395af7766c8e6208e5ab5a770a8984251849b99f5975fe6ba624a144cb(
     *,
     name: builtins.str,
```

### Comparing `butterneck-projen-0.0.7/src/butterneck_projen.egg-info/PKG-INFO` & `butterneck-projen-0.0.8/src/butterneck_projen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butterneck-projen
-Version: 0.0.7
+Version: 0.0.8
 Summary: butterneck-projen
 Home-page: https://github.com/butterneck/butterneck-projen.git
 Author: Filippo Pinton<pinton.filippo@protonmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/butterneck/butterneck-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

