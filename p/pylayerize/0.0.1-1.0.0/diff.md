# Comparing `tmp/pylayerize-0.0.1.tar.gz` & `tmp/pylayerize-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylayerize-0.0.1.tar", last modified: Wed Mar 22 22:59:39 2023, max compression
+gzip compressed data, was "pylayerize-1.0.0.tar", last modified: Fri Apr 14 15:08:16 2023, max compression
```

## Comparing `pylayerize-0.0.1.tar` & `pylayerize-1.0.0.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 22:59:39.223338 pylayerize-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-03-22 22:58:35.000000 pylayerize-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0       53 2023-03-22 22:06:59.000000 pylayerize-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4204 2023-03-22 22:59:39.223837 pylayerize-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2978 2023-03-22 22:53:46.000000 pylayerize-0.0.1/README.md
--rw-rw-rw-   0        0        0       99 2023-03-22 21:50:21.000000 pylayerize-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-03-22 22:59:39.231336 pylayerize-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1795 2023-03-22 22:47:42.000000 pylayerize-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 22:59:39.150336 pylayerize-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-22 22:59:39.168836 pylayerize-0.0.1/src/pylayerize/
--rw-rw-rw-   0        0        0       48 2023-03-22 22:36:57.000000 pylayerize-0.0.1/src/pylayerize/__init__.py
--rw-rw-rw-   0        0        0     3322 2023-03-22 22:10:11.000000 pylayerize-0.0.1/src/pylayerize/__main__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 22:59:39.199837 pylayerize-0.0.1/src/pylayerize/core/
--rw-rw-rw-   0        0        0        0 2023-01-31 22:46:16.000000 pylayerize-0.0.1/src/pylayerize/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 22:59:39.202336 pylayerize-0.0.1/src/pylayerize/core/docker/
--rw-rw-rw-   0        0        0       90 2023-01-31 22:46:16.000000 pylayerize-0.0.1/src/pylayerize/core/docker/__init__.py
--rw-rw-rw-   0        0        0     1938 2023-03-22 21:44:06.000000 pylayerize-0.0.1/src/pylayerize/core/docker/docker.py
-drwxrwxrwx   0        0        0        0 2023-03-22 22:59:39.217336 pylayerize-0.0.1/src/pylayerize/dockerfiles/
--rw-rw-rw-   0        0        0      539 2023-01-31 23:46:12.000000 pylayerize-0.0.1/src/pylayerize/dockerfiles/git_private_package.Dockerfile
--rw-rw-rw-   0        0        0      439 2023-01-31 23:46:12.000000 pylayerize-0.0.1/src/pylayerize/dockerfiles/local_install.Dockerfile
--rw-rw-rw-   0        0        0      383 2023-01-31 23:15:02.000000 pylayerize-0.0.1/src/pylayerize/dockerfiles/single_pypi_package.Dockerfile
-drwxrwxrwx   0        0        0        0 2023-03-22 22:59:39.222338 pylayerize-0.0.1/src/pylayerize/util/
--rw-rw-rw-   0        0        0      592 2023-03-22 22:10:48.000000 pylayerize-0.0.1/src/pylayerize/util/__init__.py
--rw-rw-rw-   0        0        0     3146 2023-03-22 22:30:28.000000 pylayerize-0.0.1/src/pylayerize/util/args_util.py
--rw-rw-rw-   0        0        0     1212 2023-01-31 22:46:16.000000 pylayerize-0.0.1/src/pylayerize/util/logging_util.py
-drwxrwxrwx   0        0        0        0 2023-03-22 22:59:39.198336 pylayerize-0.0.1/src/pylayerize.egg-info/
--rw-rw-rw-   0        0        0     4204 2023-03-22 22:59:39.000000 pylayerize-0.0.1/src/pylayerize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      727 2023-03-22 22:59:39.000000 pylayerize-0.0.1/src/pylayerize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 22:59:39.000000 pylayerize-0.0.1/src/pylayerize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-03-22 22:59:39.000000 pylayerize-0.0.1/src/pylayerize.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2023-03-22 22:59:39.000000 pylayerize-0.0.1/src/pylayerize.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-22 22:59:39.000000 pylayerize-0.0.1/src/pylayerize.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:16.480254 pylayerize-1.0.0/
+-rw-rw-rw-   0        0        0     1090 2023-04-14 13:52:06.000000 pylayerize-1.0.0/LICENSE.md
+-rw-rw-rw-   0        0        0      224 2023-04-14 13:52:06.000000 pylayerize-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4182 2023-04-14 15:08:16.480254 pylayerize-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3009 2023-04-14 13:52:06.000000 pylayerize-1.0.0/README.md
+-rw-rw-rw-   0        0        0       99 2023-04-14 13:52:06.000000 pylayerize-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-04-14 15:08:16.482275 pylayerize-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1745 2023-04-14 13:52:06.000000 pylayerize-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:16.393465 pylayerize-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:16.425748 pylayerize-1.0.0/src/pylayerize/
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:16.468210 pylayerize-1.0.0/src/pylayerize/Dockerfiles/
+-rw-rw-rw-   0        0        0      539 2023-04-14 13:52:06.000000 pylayerize-1.0.0/src/pylayerize/Dockerfiles/git_private_package.Dockerfile
+-rw-rw-rw-   0        0        0      439 2023-04-14 13:52:06.000000 pylayerize-1.0.0/src/pylayerize/Dockerfiles/local_install.Dockerfile
+-rw-rw-rw-   0        0        0      383 2023-04-14 13:52:06.000000 pylayerize-1.0.0/src/pylayerize/Dockerfiles/single_pypi_package.Dockerfile
+-rw-rw-rw-   0        0        0       48 2023-04-14 14:59:24.000000 pylayerize-1.0.0/src/pylayerize/__init__.py
+-rw-rw-rw-   0        0        0     3974 2023-04-14 14:41:32.000000 pylayerize-1.0.0/src/pylayerize/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:16.469718 pylayerize-1.0.0/src/pylayerize/core/
+-rw-rw-rw-   0        0        0        0 2023-04-14 13:52:06.000000 pylayerize-1.0.0/src/pylayerize/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:16.472727 pylayerize-1.0.0/src/pylayerize/core/docker/
+-rw-rw-rw-   0        0        0       90 2023-04-14 13:52:06.000000 pylayerize-1.0.0/src/pylayerize/core/docker/__init__.py
+-rw-rw-rw-   0        0        0     1938 2023-04-14 13:52:06.000000 pylayerize-1.0.0/src/pylayerize/core/docker/docker.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:16.476726 pylayerize-1.0.0/src/pylayerize/util/
+-rw-rw-rw-   0        0        0      592 2023-04-14 13:52:06.000000 pylayerize-1.0.0/src/pylayerize/util/__init__.py
+-rw-rw-rw-   0        0        0     3146 2023-04-14 13:52:06.000000 pylayerize-1.0.0/src/pylayerize/util/args_util.py
+-rw-rw-rw-   0        0        0     1212 2023-04-14 13:52:06.000000 pylayerize-1.0.0/src/pylayerize/util/logging_util.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:16.463936 pylayerize-1.0.0/src/pylayerize.egg-info/
+-rw-rw-rw-   0        0        0     4182 2023-04-14 15:08:16.000000 pylayerize-1.0.0/src/pylayerize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      937 2023-04-14 15:08:16.000000 pylayerize-1.0.0/src/pylayerize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 15:08:16.000000 pylayerize-1.0.0/src/pylayerize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-14 15:08:16.000000 pylayerize-1.0.0/src/pylayerize.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2023-04-14 15:08:16.000000 pylayerize-1.0.0/src/pylayerize.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-14 15:08:16.000000 pylayerize-1.0.0/src/pylayerize.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 15:08:16.478725 pylayerize-1.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-14 13:52:06.000000 pylayerize-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      167 2023-04-14 13:52:06.000000 pylayerize-1.0.0/tests/test_1.py
+-rw-rw-rw-   0        0        0      290 2023-04-14 13:52:06.000000 pylayerize-1.0.0/tox.ini
```

### Comparing `pylayerize-0.0.1/LICENSE.md` & `pylayerize-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pylayerize-0.0.1/PKG-INFO` & `pylayerize-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: pylayerize
-Version: 0.0.1
+Version: 1.0.0
 Summary: pylayerize simplifies the process of creating AWS Lambda Layers by leveraging Docker to compile and package Python dependencies for any targeted runtime. With support for custom packages and private GitHub repos, pylayerize optimizes the creation and deployment of Lambda Layers for improved development efficiency.
 Home-page: https://github.com/JamMassey/lambda-layer-builder
 Author: James Massey
 Author-email: jammassey@hotmail.com
 Keywords: aws lambda layer pylayerize pylayerizer pylayerize
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Pylayerize
 Pylayerize simplifies the process of creating AWS Lambda Layers by leveraging Docker to compile and package Python dependencies for any targeted runtime. With support for custom packages and private GitHub repos, pylayerize optimizes the creation and deployment of Lambda Layers for improved development efficiency.
 
 ### General Usage
@@ -30,29 +29,30 @@
 $ pip install pylayerize
 ```
 Once pylayerize is installed, you can run it from the command line by invoking the pylayerize command.
 ```ruby
 $ pylayerize -tp <target_package> [OPTIONS]
 ```
 
+
 #### Required Options:
 
 -tp, --target-package: The target package to build a layer for.
 
 #### Optional Options:
 
--h, --help: Show the help message and exit.
--op, --output-path: The output path for the layer .zip file. Default is the current directory (.).
--n, --output-layer-name: The name of the output .zip file. Default is lambda_layer.
--ll, --log-level: The log level of logging. Default is INFO.
--gu, --git-username: The git username to use for the git clone.
--gp, --git-password: The git password to use for the git clone.
--rt, --runtime: The runtime to use for the layer. Default is python3.8.
---console-log, --no-console-log: Log to console. Default is True.
---local, --no-local: Set to True if you want to use a requirments.txt file or a custom lib stored locally. Default is False.
+1. -h, --help: Show the help message and exit.
+2. -op, --output-path: The output path for the layer .zip file. Default is the current directory (.).
+3. -n, --output-layer-name: The name of the output .zip file. Default is lambda_layer.
+4. -ll, --log-level: The log level of logging. Default is INFO.
+5. -gu, --git-username: The git username to use for the git clone.
+6. -gp, --git-password: The git password to use for the git clone.
+7. -rt, --runtime: The runtime to use for the layer. Default is python3.8.
+8. --console-log, --no-console-log: Log to console. Default is True.
+9. --local, --no-local: Set to True if you want to use a requirments.txt file or a custom lib stored locally. Default is False.
 
 #### Examples
 To build a layer for numpy using the default options, run:
 
 ```ruby
 $ pylayerize -tp my_package
 ```
```

### Comparing `pylayerize-0.0.1/README.md` & `pylayerize-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 $ pip install pylayerize
 ```
 Once pylayerize is installed, you can run it from the command line by invoking the pylayerize command.
 ```ruby
 $ pylayerize -tp <target_package> [OPTIONS]
 ```
 
+
 #### Required Options:
 
 -tp, --target-package: The target package to build a layer for.
 
 #### Optional Options:
 
--h, --help: Show the help message and exit.
--op, --output-path: The output path for the layer .zip file. Default is the current directory (.).
--n, --output-layer-name: The name of the output .zip file. Default is lambda_layer.
--ll, --log-level: The log level of logging. Default is INFO.
--gu, --git-username: The git username to use for the git clone.
--gp, --git-password: The git password to use for the git clone.
--rt, --runtime: The runtime to use for the layer. Default is python3.8.
---console-log, --no-console-log: Log to console. Default is True.
---local, --no-local: Set to True if you want to use a requirments.txt file or a custom lib stored locally. Default is False.
+1. -h, --help: Show the help message and exit.
+2. -op, --output-path: The output path for the layer .zip file. Default is the current directory (.).
+3. -n, --output-layer-name: The name of the output .zip file. Default is lambda_layer.
+4. -ll, --log-level: The log level of logging. Default is INFO.
+5. -gu, --git-username: The git username to use for the git clone.
+6. -gp, --git-password: The git password to use for the git clone.
+7. -rt, --runtime: The runtime to use for the layer. Default is python3.8.
+8. --console-log, --no-console-log: Log to console. Default is True.
+9. --local, --no-local: Set to True if you want to use a requirments.txt file or a custom lib stored locally. Default is False.
 
 #### Examples
 To build a layer for numpy using the default options, run:
 
 ```ruby
 $ pylayerize -tp my_package
 ```
@@ -65,8 +66,8 @@
 Contributions are welcome! Here are some guidelines for contributing to this project:
 
 Fork this repository and create a new branch for your feature or bug fix.
 Make your changes and commit them with descriptive commit messages.
 Create a pull request against the dev branch and describe your changes and the problem they solve.
 Ensure that your code passes all tests and meets the project's code standards.
 Respond to any feedback from maintainers and make any necessary changes.
-If you'd like to contribute but aren't sure where to start, take a look at the project's issue tracker. Issues marked as "help wanted" or "good first issue" are a good place to start.
+If you'd like to contribute but aren't sure where to start, take a look at the project's issue tracker. Issues marked as "help wanted" or "good first issue" are a good place to start.
```

### Comparing `pylayerize-0.0.1/setup.py` & `pylayerize-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,23 +22,22 @@
         # see https://pypi.org/classifiers/
         'Development Status :: 5 - Production/Stable',
 
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
 
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3 :: Only',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-	python_requires='>=3.6',
+	python_requires='>=3.7',
     extras_require={
         'dev': ['check-manifest'],
         # 'test': ['coverage'],
     },
     author='James Massey',
     author_email='jammassey@hotmail.com',
     url='https://github.com/JamMassey/lambda-layer-builder',
```

### Comparing `pylayerize-0.0.1/src/pylayerize/__main__.py` & `pylayerize-1.0.0/src/pylayerize/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,95 @@
 from __future__ import annotations
+
 ## There is a Docker SDK for Python that we could use. As for now I'm just using subprocess.run to run the docker commands, at least it saves having to rely on an extra dependency.
 import logging
-from util.args_util import parse_args
-from util.logging_util import setup_logger
-from core.docker import build_and_run_docker_image, copy_file_from_container, remove_container
+import os
 from typing import TYPE_CHECKING
 
+from pylayerize.core.docker import (
+    build_and_run_docker_image,
+    copy_file_from_container,
+    remove_container,
+)
+from pylayerize.util.args_util import parse_args
+from pylayerize.util.logging_util import setup_logger
+
 if TYPE_CHECKING:
     from typing import Dict
 
 logger = logging.getLogger(__name__)
+DOCKERFILE_PATH = os.path.join(os.path.dirname(__file__), "Dockerfiles")
+# get all the dockerfiles in the Dockerfiles folder
+DOCKERFILES = {
+    "single_pypi_package": os.path.join(DOCKERFILE_PATH, "single_pypi_package.Dockerfile"),
+    "git_private_package": os.path.join(DOCKERFILE_PATH, "git_private_package.Dockerfile"),
+    "local_install": os.path.join(DOCKERFILE_PATH, "local_install.Dockerfile"),
+}
+
 
 # For now only supports one package and one container at a time. Package can be a requirement.txt file, a local path or a single package name. All dependant packages will also be installed.
-def build_aws_lamda_layer(package: str, output_path: str, output_layer_name: str, local: bool, git_auth: Dict = None, runtime: str = "3.8") -> None:
+def build_aws_lamda_layer(
+    package: str, output_path: str, output_layer_name: str, local: bool, git_auth: Dict = None, runtime: str = "3.8"
+) -> None:
     if local:
         target = package.split("/")[-1]
         if package.endswith(".txt"):
             target = "-r " + target
         build_and_run_docker_image(
-            dockerfile_path="Dockerfiles/local_install.Dockerfile",
+            dockerfile_path=DOCKERFILES["local_install"],
             image_name="lambda-layer-builder",
             build_args={"PATH_TO_LOCAL_FILE": package, "PACKAGE": target, "OUTPUT_NAME": output_layer_name, "RUNTIME": runtime},
-            **{"--name": "lambda-layer-builder"}
+            **{"--name": "lambda-layer-builder"},
         )
-    elif git_auth: # Can maybe do some conditional logic within a RUN call within this Dockerfile and merge it with the single_pypi_package Dockerfile.
+    elif (
+        git_auth
+    ):  # Can maybe do some conditional logic within a RUN call within this Dockerfile and merge it with the single_pypi_package Dockerfile.
         build_and_run_docker_image(
-            dockerfile_path="Dockerfiles/git_private_package.Dockerfile",
+            dockerfile_path=DOCKERFILES["git_private_package"],
             image_name="lambda-layer-builder",
-            build_args={"PACKAGE": package, "OUTPUT_NAME": output_layer_name, "RUNTIME": runtime, "GIT_USERNAME": git_auth["Username"], "GIT_PASSWORD": git_auth["Password"]},
-            **{"--name": "lambda-layer-builder"}
+            build_args={
+                "PACKAGE": package,
+                "OUTPUT_NAME": output_layer_name,
+                "RUNTIME": runtime,
+                "GIT_USERNAME": git_auth["Username"],
+                "GIT_PASSWORD": git_auth["Password"],
+            },
+            **{"--name": "lambda-layer-builder"},
         )
     else:
         build_and_run_docker_image(
-            dockerfile_path="Dockerfiles/single_pypi_package.Dockerfile",
+            dockerfile_path=DOCKERFILES["single_pypi_package"],
             image_name="lambda-layer-builder",
             build_args={"PACKAGE": package, "OUTPUT_NAME": output_layer_name, "RUNTIME": runtime},
-            **{"--name": "lambda-layer-builder"}
+            **{"--name": "lambda-layer-builder"},
         )
     copy_file_from_container("lambda-layer-builder", f"var/task/{output_layer_name}.zip", f"{output_path}/{output_layer_name}.zip")
     remove_container("lambda-layer-builder")
 
 
 def main() -> None:
     args = parse_args()
     setup_logger(
         level=args.log_level,
         stream_logs=args.console_log,
     )
     logger.info("Logger initialised")
     if bool(args.git_username) != bool(args.git_password):
         raise ValueError("I attempting to authenticate for git you must provide both git username and password.")
-    if args.runtime not in ["python3.9","python3.8", "python3.7", "python3.6"]:
+    if args.runtime not in ["python3.9", "python3.8", "python3.7", "python3.6"]:
         raise ValueError("Runtime must be one of 3.8, 3.7 or 3.6")
     if args.git_username and args.git_password:
         git_auth = {"Username": args.git_username, "Password": args.git_password}
     else:
         git_auth = None
-    build_aws_lamda_layer(package=args.target_package, output_path=args.output_path, output_layer_name=args.output_layer_name, local=args.local, git_auth=git_auth, runtime=args.runtime)
-    
+    build_aws_lamda_layer(
+        package=args.target_package,
+        output_path=args.output_path,
+        output_layer_name=args.output_layer_name,
+        local=args.local,
+        git_auth=git_auth,
+        runtime=args.runtime,
+    )
+
+
 if __name__ == "__main__":
-	main()
+    main()
```

### Comparing `pylayerize-0.0.1/src/pylayerize/core/docker/docker.py` & `pylayerize-1.0.0/src/pylayerize/core/docker/docker.py`

 * *Files identical despite different names*

### Comparing `pylayerize-0.0.1/src/pylayerize/dockerfiles/git_private_package.Dockerfile` & `pylayerize-1.0.0/src/pylayerize/Dockerfiles/git_private_package.Dockerfile`

 * *Files identical despite different names*

### Comparing `pylayerize-0.0.1/src/pylayerize/util/__init__.py` & `pylayerize-1.0.0/src/pylayerize/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pylayerize-0.0.1/src/pylayerize/util/args_util.py` & `pylayerize-1.0.0/src/pylayerize/util/args_util.py`

 * *Files identical despite different names*

### Comparing `pylayerize-0.0.1/src/pylayerize/util/logging_util.py` & `pylayerize-1.0.0/src/pylayerize/util/logging_util.py`

 * *Files identical despite different names*

### Comparing `pylayerize-0.0.1/src/pylayerize.egg-info/PKG-INFO` & `pylayerize-1.0.0/src/pylayerize.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: pylayerize
-Version: 0.0.1
+Version: 1.0.0
 Summary: pylayerize simplifies the process of creating AWS Lambda Layers by leveraging Docker to compile and package Python dependencies for any targeted runtime. With support for custom packages and private GitHub repos, pylayerize optimizes the creation and deployment of Lambda Layers for improved development efficiency.
 Home-page: https://github.com/JamMassey/lambda-layer-builder
 Author: James Massey
 Author-email: jammassey@hotmail.com
 Keywords: aws lambda layer pylayerize pylayerizer pylayerize
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Pylayerize
 Pylayerize simplifies the process of creating AWS Lambda Layers by leveraging Docker to compile and package Python dependencies for any targeted runtime. With support for custom packages and private GitHub repos, pylayerize optimizes the creation and deployment of Lambda Layers for improved development efficiency.
 
 ### General Usage
@@ -30,29 +29,30 @@
 $ pip install pylayerize
 ```
 Once pylayerize is installed, you can run it from the command line by invoking the pylayerize command.
 ```ruby
 $ pylayerize -tp <target_package> [OPTIONS]
 ```
 
+
 #### Required Options:
 
 -tp, --target-package: The target package to build a layer for.
 
 #### Optional Options:
 
--h, --help: Show the help message and exit.
--op, --output-path: The output path for the layer .zip file. Default is the current directory (.).
--n, --output-layer-name: The name of the output .zip file. Default is lambda_layer.
--ll, --log-level: The log level of logging. Default is INFO.
--gu, --git-username: The git username to use for the git clone.
--gp, --git-password: The git password to use for the git clone.
--rt, --runtime: The runtime to use for the layer. Default is python3.8.
---console-log, --no-console-log: Log to console. Default is True.
---local, --no-local: Set to True if you want to use a requirments.txt file or a custom lib stored locally. Default is False.
+1. -h, --help: Show the help message and exit.
+2. -op, --output-path: The output path for the layer .zip file. Default is the current directory (.).
+3. -n, --output-layer-name: The name of the output .zip file. Default is lambda_layer.
+4. -ll, --log-level: The log level of logging. Default is INFO.
+5. -gu, --git-username: The git username to use for the git clone.
+6. -gp, --git-password: The git password to use for the git clone.
+7. -rt, --runtime: The runtime to use for the layer. Default is python3.8.
+8. --console-log, --no-console-log: Log to console. Default is True.
+9. --local, --no-local: Set to True if you want to use a requirments.txt file or a custom lib stored locally. Default is False.
 
 #### Examples
 To build a layer for numpy using the default options, run:
 
 ```ruby
 $ pylayerize -tp my_package
 ```
```

