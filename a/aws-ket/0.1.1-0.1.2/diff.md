# Comparing `tmp/aws-ket-0.1.1.tar.gz` & `tmp/aws-ket-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ket-0.1.1.tar", last modified: Fri Mar 24 00:18:09 2023, max compression
+gzip compressed data, was "aws-ket-0.1.2.tar", last modified: Fri Apr 14 14:13:09 2023, max compression
```

## Comparing `aws-ket-0.1.1.tar` & `aws-ket-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-03-24 00:18:09.219641 aws-ket-0.1.1/
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     1452 2023-03-18 01:01:48.000000 aws-ket-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 sayefiqbal   (502) staff       (20)    11357 2023-02-09 13:04:42.000000 aws-ket-0.1.1/LICENSE
--rw-r--r--   0 sayefiqbal   (502) staff       (20)      396 2023-03-24 00:07:58.000000 aws-ket-0.1.1/MANIFEST.in
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     2132 2023-03-08 01:07:31.000000 aws-ket-0.1.1/Makefile
--rw-r--r--   0 sayefiqbal   (502) staff       (20)      329 2023-03-24 00:18:09.219437 aws-ket-0.1.1/PKG-INFO
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     2410 2023-03-08 14:21:35.000000 aws-ket-0.1.1/README.md
-drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-03-24 00:18:09.219134 aws-ket-0.1.1/aws_ket.egg-info/
--rw-r--r--   0 sayefiqbal   (502) staff       (20)      329 2023-03-24 00:18:09.000000 aws-ket-0.1.1/aws_ket.egg-info/PKG-INFO
--rw-r--r--   0 sayefiqbal   (502) staff       (20)      202 2023-03-24 00:18:09.000000 aws-ket-0.1.1/aws_ket.egg-info/SOURCES.txt
--rw-r--r--   0 sayefiqbal   (502) staff       (20)        1 2023-03-24 00:18:09.000000 aws-ket-0.1.1/aws_ket.egg-info/dependency_links.txt
--rw-r--r--   0 sayefiqbal   (502) staff       (20)        1 2023-03-24 00:18:09.000000 aws-ket-0.1.1/aws_ket.egg-info/top_level.txt
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     2244 2023-03-23 23:46:20.000000 aws-ket-0.1.1/pyproject.toml
--rw-r--r--   0 sayefiqbal   (502) staff       (20)       38 2023-03-24 00:18:09.219708 aws-ket-0.1.1/setup.cfg
--rw-r--r--   0 sayefiqbal   (502) staff       (20)      408 2023-03-24 00:16:41.000000 aws-ket-0.1.1/setup.py
+drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-04-14 14:13:09.846471 aws-ket-0.1.2/
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     1452 2023-03-18 01:01:48.000000 aws-ket-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)    11357 2023-02-09 13:04:42.000000 aws-ket-0.1.2/LICENSE
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)      396 2023-03-24 00:07:58.000000 aws-ket-0.1.2/MANIFEST.in
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     2150 2023-04-14 14:05:00.000000 aws-ket-0.1.2/Makefile
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)      329 2023-04-14 14:13:09.846202 aws-ket-0.1.2/PKG-INFO
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     2699 2023-04-14 13:55:20.000000 aws-ket-0.1.2/README.md
+drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-04-14 14:13:09.845838 aws-ket-0.1.2/aws_ket.egg-info/
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)      329 2023-04-14 14:13:09.000000 aws-ket-0.1.2/aws_ket.egg-info/PKG-INFO
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)      202 2023-04-14 14:13:09.000000 aws-ket-0.1.2/aws_ket.egg-info/SOURCES.txt
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)        1 2023-04-14 14:13:09.000000 aws-ket-0.1.2/aws_ket.egg-info/dependency_links.txt
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)        1 2023-04-14 14:13:09.000000 aws-ket-0.1.2/aws_ket.egg-info/top_level.txt
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     2253 2023-04-14 14:05:00.000000 aws-ket-0.1.2/pyproject.toml
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)       38 2023-04-14 14:13:09.846563 aws-ket-0.1.2/setup.cfg
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)      523 2023-04-14 14:05:00.000000 aws-ket-0.1.2/setup.py
```

### Comparing `aws-ket-0.1.1/CONTRIBUTING.md` & `aws-ket-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aws-ket-0.1.1/LICENSE` & `aws-ket-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ket-0.1.1/Makefile` & `aws-ket-0.1.2/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -10,43 +10,43 @@
 install:  ## install library
 	python -m pip install .
 
 #########
 # LINTS #
 #########
 lint:  ## run static analysis with flake8
-	python -m black src
+	python -m black awsket
 scan:
-	python -m flake8 src
+	python -m flake8 awsket
 # Alias
 lints: lint
 
 format:  ## run autoformatting with black
-	python -m src/ 
+	python -m awsket/ 
 
 # alias
 fix: format
 
 check:  ## check assets for packaging
 	check-manifest -v
 
 # Alias
 checks: check
 
 annotate:  ## run type checking
-	python -m mypy ./src
+	python -m mypy ./awsket
 
 #########
 # TESTS #
 #########
 test: ## clean and run unit tests
-	python -m pytest -v src/tests
+	python -m pytest -v awsket/tests
 
 coverage:  ## clean and run unit tests with coverage
-	coverage run -m pytest -v src/tests
+	coverage run -m pytest -v awsket/tests
 	coverage html
 	coverage report -m
 
 # Alias
 tests: test
 
 ###########
```

### Comparing `aws-ket-0.1.1/README.md` & `aws-ket-0.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ## Overview
 AWS-KET (AWS KMS Encryption Tool) uses AWS KMS Key to encrypt and decrypt files/contents based on user provided kms keys and push them to a datastore backend (S3, RDS or DynamoDB).
 
 
 ![GitHub issues](https://img.shields.io/github/issues/sayefiqb/aws-ket)
-[![CodeQL](https://github.com/sayefiqb/aws-ket/actions/workflows/github-code-scanning/codeql/badge.svg?branch=main)](https://github.com/sayefiqb/aws-ket/actions/workflows/github-code-scanning/codeql) [![Build Status](https://github.com/sayefiqb/aws-ket/actions/workflows/build.yaml/badge.svg)](https://github.com/sayefiqb/aws-ket/actions/workflows/build.yaml) [![codecov](https://codecov.io/gh/sayefiqb/aws-ket/branch/main/graph/badge.svg?token=13922GT547)](https://codecov.io/gh/sayefiqb/aws-ket)
+[![CodeQL](https://github.com/sayefiqb/aws-ket/actions/workflows/github-code-scanning/codeql/badge.svg?branch=main)](https://github.com/sayefiqb/aws-ket/actions/workflows/github-code-scanning/codeql) [![Build Status](https://github.com/sayefiqb/aws-ket/actions/workflows/build.yaml/badge.svg)](https://github.com/sayefiqb/aws-ket/actions/workflows/build.yaml) [![codecov](https://codecov.io/gh/sayefiqb/aws-ket/branch/main/graph/badge.svg?token=13922GT547)](https://codecov.io/gh/sayefiqb/aws-ket)[![PyPI](https://img.shields.io/pypi/v/aws-ket)](https://pypi.org/project/aws-ket)[![Documentation Status](https://readthedocs.org/projects/aws-ket/badge/?version=latest)](https://aws-ket.readthedocs.io/en/latest/?badge=latest)
 
 #### Setup
 
 This application will only work if you have AWS account with full privileges on KMS and S3 services in AWS. You should also have aws cli tool installed.
 
 [Setup AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)
 
@@ -55,7 +55,12 @@
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make lint`: perform lint using `black`
 - `make scan`: run static analysis on code using `flake8`
 - `make test`: run automated tests with `pytest`
 - `make coverage`: run automated tests with `pytest` and collect coverage information
 
 `coverage` output can also be found in html format in `htmlcover` directory.
+
+#### Example
+
+First download the source code
+![](aws-ket.gif)
```

### Comparing `aws-ket-0.1.1/pyproject.toml` & `aws-ket-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "aws-ket"
 authors = [{name = "Sayef Iqbal", email = "si2400@columbia.edu"}]
 description="Utility tool to encrypt data using AWS KMS and store it in preferred backend."
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.9"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
@@ -63,18 +63,18 @@
 ignore = [
 ]
 
 [tool.flake8]
 ignore = ['E203', 'W503']
 max-line-length=120
 exclude=[
-    'src/tests/*'
+    'awsket/tests/*'
 ]
 per-file-ignores= [
-    'src/__init__.py:F401, F403'
+    'awsket/__init__.py:F401, F403'
 ]
 
 
 [tool.isort]
 line_length = 120
 known_first_party = 'pydantic'
 multi_line_output = 3
@@ -96,8 +96,8 @@
 # disallow_subclassing_any = true
 # disallow_incomplete_defs = true
 # disallow_untyped_decorators = true
 # disallow_untyped_calls = true
 
 [tool.pytest.ini_options]
 asyncio_mode = 'strict'
-testpaths = 'src/tests'
+testpaths = 'awsket/tests'
```

