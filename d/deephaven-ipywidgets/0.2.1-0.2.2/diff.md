# Comparing `tmp/deephaven_ipywidgets-0.2.1.tar.gz` & `tmp/deephaven_ipywidgets-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephaven_ipywidgets-0.2.1.tar", last modified: Thu Jan 26 13:19:36 2023, max compression
+gzip compressed data, was "deephaven_ipywidgets-0.2.2.tar", last modified: Fri Apr 14 19:25:57 2023, max compression
```

## Comparing `deephaven_ipywidgets-0.2.1.tar` & `deephaven_ipywidgets-0.2.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/
--rw-rw-r--   0 bender    (1000) bender    (1000)     1508 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/LICENSE.txt
--rw-rw-r--   0 bender    (1000) bender    (1000)     5565 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/PKG-INFO
--rw-rw-r--   0 bender    (1000) bender    (1000)     4603 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/README.md
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.496229 deephaven_ipywidgets-0.2.1/css/
--rw-rw-r--   0 bender    (1000) bender    (1000)      437 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/css/widget.css
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/
--rw-rw-r--   0 bender    (1000) bender    (1000)     1865 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/__init__.py
--rw-rw-r--   0 bender    (1000) bender    (1000)      268 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/_frontend.py
--rw-rw-r--   0 bender    (1000) bender    (1000)      212 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/_version.py
--rw-rw-r--   0 bender    (1000) bender    (1000)     3091 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/deephaven.py
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/
--rw-rw-r--   0 bender    (1000) bender    (1000)     3738 2023-01-26 13:19:33.596164 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/package.json
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/static/
--rw-rw-r--   0 bender    (1000) bender    (1000)     9693 2023-01-26 13:19:33.592164 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/static/480.0f4281f61b6879ab4405.js
--rw-rw-r--   0 bender    (1000) bender    (1000)     9272 2023-01-26 13:19:33.592164 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/static/568.1c6b1b42819be15c8a89.js
--rw-rw-r--   0 bender    (1000) bender    (1000)    17340 2023-01-26 13:19:33.592164 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/static/701.c67db7c3d6d969fcf22b.js
--rw-rw-r--   0 bender    (1000) bender    (1000)     6860 2023-01-26 13:19:33.592164 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/static/remoteEntry.aefc6da13048e00900c3.js
--rw-rw-r--   0 bender    (1000) bender    (1000)      118 2023-01-26 13:19:32.596142 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/static/style.js
--rw-rw-r--   0 bender    (1000) bender    (1000)    15446 2023-01-26 13:19:33.592164 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/static/third-party-licenses.json
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/nbextension/
--rw-rw-r--   0 bender    (1000) bender    (1000)      391 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/nbextension/extension.js
--rw-rw-r--   0 bender    (1000) bender    (1000)    25901 2023-01-26 13:19:31.112109 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/nbextension/index.js
--rw-rw-r--   0 bender    (1000) bender    (1000)    95786 2023-01-26 13:19:31.112109 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/nbextension/index.js.map
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/tests/
--rw-rw-r--   0 bender    (1000) bender    (1000)        0 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/tests/__init__.py
--rw-rw-r--   0 bender    (1000) bender    (1000)     1421 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/tests/conftest.py
--rw-rw-r--   0 bender    (1000) bender    (1000)      483 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/tests/test_nbextension_path.py
--rw-rw-r--   0 bender    (1000) bender    (1000)      697 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/tests/test_table.py
--rw-rw-r--   0 bender    (1000) bender    (1000)       74 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/deephaven_ipywidgets.json
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/docs/
--rw-rw-r--   0 bender    (1000) bender    (1000)      622 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/docs/Makefile
--rw-rw-r--   0 bender    (1000) bender    (1000)      180 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/docs/environment.yml
--rw-rw-r--   0 bender    (1000) bender    (1000)      792 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/docs/make.bat
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/docs/source/
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/docs/source/_static/
--rw-rw-r--   0 bender    (1000) bender    (1000)    25378 2023-01-26 13:19:31.092108 deephaven_ipywidgets-0.2.1/docs/source/_static/embed-bundle.js
--rw-rw-r--   0 bender    (1000) bender    (1000)    94888 2023-01-26 13:19:31.092108 deephaven_ipywidgets-0.2.1/docs/source/_static/embed-bundle.js.map
--rw-rw-r--   0 bender    (1000) bender    (1000)      120 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/docs/source/_static/helper.js
--rw-rw-r--   0 bender    (1000) bender    (1000)     6457 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/docs/source/conf.py
--rw-rw-r--   0 bender    (1000) bender    (1000)      879 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/docs/source/develop-install.rst
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/docs/source/examples/
--rw-rw-r--   0 bender    (1000) bender    (1000)      385 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/docs/source/examples/index.rst
--rw-rw-r--   0 bender    (1000) bender    (1000)       53 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/docs/source/examples/introduction.nblink
--rw-rw-r--   0 bender    (1000) bender    (1000)      672 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/docs/source/index.rst
--rw-rw-r--   0 bender    (1000) bender    (1000)     1078 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/docs/source/installing.rst
--rw-rw-r--   0 bender    (1000) bender    (1000)      109 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/docs/source/introduction.rst
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/examples/
--rw-rw-r--   0 bender    (1000) bender    (1000)     2004 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/examples/introduction.ipynb
--rw-rw-r--   0 bender    (1000) bender    (1000)      201 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/install.json
--rw-rw-r--   0 bender    (1000) bender    (1000)     3622 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/package.json
--rw-rw-r--   0 bender    (1000) bender    (1000)      145 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/pyproject.toml
--rw-rw-r--   0 bender    (1000) bender    (1000)      137 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/pytest.ini
--rw-rw-r--   0 bender    (1000) bender    (1000)      146 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/setup.cfg
--rw-rw-r--   0 bender    (1000) bender    (1000)     3350 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/setup.py
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/src/
-drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2023-01-26 13:19:36.500229 deephaven_ipywidgets-0.2.1/src/__tests__/
--rw-rw-r--   0 bender    (1000) bender    (1000)      697 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/src/__tests__/index.spec.ts
--rw-rw-r--   0 bender    (1000) bender    (1000)     2802 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/src/__tests__/utils.ts
--rw-rw-r--   0 bender    (1000) bender    (1000)      728 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/src/extension.ts
--rw-rw-r--   0 bender    (1000) bender    (1000)      155 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/src/index.ts
--rw-rw-r--   0 bender    (1000) bender    (1000)     1264 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/src/plugin.ts
--rw-rw-r--   0 bender    (1000) bender    (1000)      583 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/src/version.ts
--rw-rw-r--   0 bender    (1000) bender    (1000)     2175 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/src/widget.ts
--rw-rw-r--   0 bender    (1000) bender    (1000)      553 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/tsconfig.json
--rw-rw-r--   0 bender    (1000) bender    (1000)     2179 2023-01-25 22:13:56.929954 deephaven_ipywidgets-0.2.1/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.201803 deephaven_ipywidgets-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-14 19:25:57.201803 deephaven_ipywidgets-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/css/widget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/deephaven.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-14 19:24:24.497498 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-04-14 19:24:24.493498 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/480.26bcd834ece40109d1df.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-04-14 19:24:24.493498 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/568.8c7c3ea60a12c60e6eb1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17340 2023-04-14 19:24:24.493498 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/701.c67db7c3d6d969fcf22b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-14 19:24:24.493498 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/remoteEntry.6443de594d4e2715e64f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-14 19:24:21.909489 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15446 2023-04-14 19:24:24.493498 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25901 2023-04-14 19:24:18.705479 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/nbextension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95786 2023-04-14 19:24:18.705479 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/nbextension/index.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/test_nbextension_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/deephaven_ipywidgets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.197803 deephaven_ipywidgets-0.2.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    25378 2023-04-14 19:24:18.589478 deephaven_ipywidgets-0.2.2/docs/source/_static/embed-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94888 2023-04-14 19:24:18.589478 deephaven_ipywidgets-0.2.2/docs/source/_static/embed-bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/_static/helper.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/develop-install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.201803 deephaven_ipywidgets-0.2.2/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/examples/introduction.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/docs/source/introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.201803 deephaven_ipywidgets-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/examples/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-14 19:22:30.929126 deephaven_ipywidgets-0.2.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.201803 deephaven_ipywidgets-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:25:57.201803 deephaven_ipywidgets-0.2.2/src/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/__tests__/index.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/__tests__/utils.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/extension.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/plugin.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/src/widget.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-14 19:22:30.933126 deephaven_ipywidgets-0.2.2/webpack.config.js
```

### Comparing `deephaven_ipywidgets-0.2.1/LICENSE.txt` & `deephaven_ipywidgets-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/PKG-INFO` & `deephaven_ipywidgets-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven_ipywidgets
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Custom Jupyter Widget Library
 Home-page: https://github.com/deephaven/deephaven-ipywidgets
 Author: Deephaven Data Labs LLC
 Author-email: operations@deephaven.io
 License: BSD
 Keywords: Jupyter,Widgets,IPython
 Platform: Linux
```

### Comparing `deephaven_ipywidgets-0.2.1/README.md` & `deephaven_ipywidgets-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/__init__.py` & `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/deephaven.py` & `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/deephaven.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import __main__
 from ipywidgets import DOMWidget
 from traitlets import Unicode, Integer
 from deephaven_server import Server
 from uuid import uuid4
 from ._frontend import module_name, module_version
-
+import os
 
 def _str_object_type(obj):
     """Returns the object type as a string value"""
     return f"{obj.__class__.__module__}.{obj.__class__.__name__}"
 
 
 def _path_for_object(obj):
@@ -59,22 +59,29 @@
         """
         super(DeephavenWidget, self).__init__()
 
         # Generate a new table ID using a UUID prepended with a `t_` prefix
         object_id = f"t_{str(uuid4()).replace('-', '_')}"
 
         port = Server.instance.port
+
         server_url = f"http://localhost:{Server.instance.port}/"
 
+        if "DEEPHAVEN_IPY_URL" in os.environ:
+            server_url = os.environ["DEEPHAVEN_IPY_URL"]
+
         try:
             from google.colab.output import eval_js
             server_url = eval_js(f"google.colab.kernel.proxyPort({port})")
         except ImportError:
             pass
 
+        if not server_url.endswith("/"):
+            server_url = f"{server_url}/"
+
         # Generate the iframe_url from the object type
         iframe_url = f"{server_url}iframe/{_path_for_object(deephaven_object)}/?name={object_id}"
 
         # Add the table to the main modules globals list so it can be retrieved by the iframe
         __main__.__dict__[object_id] = deephaven_object
 
         self.set_trait('server_url', server_url)
```

### Comparing `deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/package.json` & `deephaven_ipywidgets-0.2.2/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}"}*

```diff
@@ -57,18 +57,14 @@
     "files": [
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/deephaven/deephaven-ipywidgets",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.aefc6da13048e00900c3.js"
-        },
         "extension": "lib/plugin",
         "outputDir": "deephaven_ipywidgets/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
```

### Comparing `deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/static/480.0f4281f61b6879ab4405.js` & `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/480.26bcd834ece40109d1df.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -48,15 +48,15 @@
             t.default = d
         },
         657: (e, t, n) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.MODULE_NAME = t.MODULE_VERSION = void 0;
-            const i = n(147);
+            const i = n(598);
             t.MODULE_VERSION = i.version, t.MODULE_NAME = i.name
         },
         367: function(e, t, n) {
             "use strict";
             var i = this && this.__importDefault || function(e) {
                 return e && e.__esModule ? e : {
                     default: e
@@ -270,13 +270,13 @@
                             0 === a[u].references && (a[u].updater(), a.splice(u, 1))
                         }
                         n = l
                     }
                 }
             }
         },
-        147: e => {
+        598: e => {
             "use strict";
             e.exports = JSON.parse('{"name":"@deephaven/ipywidgets","version":"0.1.0","description":"Deephaven ipython widget library","keywords":["ipywidgets","jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/deephaven/deephaven-ipywidgets","bugs":{"url":"https://github.com/deephaven/deephaven-ipywidgets/issues"},"license":"BSD-3-Clause","author":{"name":"Deephaven Data Labs LLC","email":"operations@deephaven.io"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/deephaven/deephaven-ipywidgets"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf deephaven_ipywidgets/labextension","clean:nbextension":"rimraf deephaven_ipywidgets/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@deephaven/jsapi-shim":"0.15.0","@deephaven/log":"0.15.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","uuid":"8.3.2"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@deephaven/eslint-config":"0.15.0","@deephaven/prettier-config":"0.15.0","@jupyterlab/builder":"^3.0.0","@phosphor/application":"^1.6.0","@phosphor/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"8.3.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^4.28.0","@typescript-eslint/parser":"^4.28.0","acorn":"^7.2.0","babel-eslint":"^10.1.0","css-loader":"^3.2.0","eslint":"^7.22.0","eslint-import-resolver-typescript":"^2.5.0","eslint-config-prettier":"^6.11.0","eslint-plugin-import":"^2.26.0","eslint-plugin-es":"^4.1.0","eslint-plugin-flowtype":"^5.2.0","eslint-plugin-jsx-a11y":"^6.6.0","eslint-plugin-prettier":"^3.3.1","eslint-plugin-react":"7.30.1","eslint-plugin-react-hooks":"4.6.0","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"deephaven_ipywidgets/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"prettier":"@deephaven/prettier-config","publishConfig":{"access":"public"}}')
         }
     }
 ]);
```

### Comparing `deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/static/568.1c6b1b42819be15c8a89.js` & `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/568.8c7c3ea60a12c60e6eb1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -20,15 +20,15 @@
             }), r(n(657), t), r(n(367), t)
         },
         657: (e, t, n) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.MODULE_NAME = t.MODULE_VERSION = void 0;
-            const i = n(147);
+            const i = n(598);
             t.MODULE_VERSION = i.version, t.MODULE_NAME = i.name
         },
         367: function(e, t, n) {
             "use strict";
             var i = this && this.__importDefault || function(e) {
                 return e && e.__esModule ? e : {
                     default: e
@@ -242,13 +242,13 @@
                             0 === a[u].references && (a[u].updater(), a.splice(u, 1))
                         }
                         n = l
                     }
                 }
             }
         },
-        147: e => {
+        598: e => {
             "use strict";
             e.exports = JSON.parse('{"name":"@deephaven/ipywidgets","version":"0.1.0","description":"Deephaven ipython widget library","keywords":["ipywidgets","jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/deephaven/deephaven-ipywidgets","bugs":{"url":"https://github.com/deephaven/deephaven-ipywidgets/issues"},"license":"BSD-3-Clause","author":{"name":"Deephaven Data Labs LLC","email":"operations@deephaven.io"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/deephaven/deephaven-ipywidgets"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf deephaven_ipywidgets/labextension","clean:nbextension":"rimraf deephaven_ipywidgets/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@deephaven/jsapi-shim":"0.15.0","@deephaven/log":"0.15.0","@jupyter-widgets/base":"^1.1.10 || ^2.0.0 || ^3.0.0 || ^4.0.0","uuid":"8.3.2"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@deephaven/eslint-config":"0.15.0","@deephaven/prettier-config":"0.15.0","@jupyterlab/builder":"^3.0.0","@phosphor/application":"^1.6.0","@phosphor/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"8.3.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^4.28.0","@typescript-eslint/parser":"^4.28.0","acorn":"^7.2.0","babel-eslint":"^10.1.0","css-loader":"^3.2.0","eslint":"^7.22.0","eslint-import-resolver-typescript":"^2.5.0","eslint-config-prettier":"^6.11.0","eslint-plugin-import":"^2.26.0","eslint-plugin-es":"^4.1.0","eslint-plugin-flowtype":"^5.2.0","eslint-plugin-jsx-a11y":"^6.6.0","eslint-plugin-prettier":"^3.3.1","eslint-plugin-react":"7.30.1","eslint-plugin-react-hooks":"4.6.0","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"deephaven_ipywidgets/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}},"prettier":"@deephaven/prettier-config","publishConfig":{"access":"public"}}')
         }
     }
 ]);
```

### Comparing `deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/static/701.c67db7c3d6d969fcf22b.js` & `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/701.c67db7c3d6d969fcf22b.js`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/static/remoteEntry.aefc6da13048e00900c3.js` & `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/remoteEntry.6443de594d4e2715e64f.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, d, u, l, s, f, p, c, h, v, g, b, m = {
-            393: (e, r, t) => {
+    var e, r, t, n, o, i, a, u, l, s, d, f, p, c, h, v, g, b, m = {
+            690: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(790), t.e(568)]).then((() => () => t(568))),
                         "./extension": () => Promise.all([t.e(790), t.e(480)]).then((() => () => t(480)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
@@ -37,53 +37,53 @@
     }
     w.m = m, w.c = y, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        480: "0f4281f61b6879ab4405",
-        568: "1c6b1b42819be15c8a89",
+        480: "26bcd834ece40109d1df",
+        568: "8c7c3ea60a12c60e6eb1",
         701: "c67db7c3d6d969fcf22b",
         790: "b21bef9f80316178ddf0"
     } [e] + ".js?v=" + {
-        480: "0f4281f61b6879ab4405",
-        568: "1c6b1b42819be15c8a89",
+        480: "26bcd834ece40109d1df",
+        568: "8c7c3ea60a12c60e6eb1",
         701: "c67db7c3d6d969fcf22b",
         790: "b21bef9f80316178ddf0"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@deephaven/ipywidgets:", w.l = (t, n, o, i) => {
         if (e[t]) e[t].push(n);
         else {
-            var a, d;
+            var a, u;
             if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), l = 0; l < u.length; l++) {
-                    var s = u[l];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        a = s;
+                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
+                    var d = l[s];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        a = d;
                         break
                     }
                 }
-            a || (d = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, w.nc && a.setAttribute("nonce", w.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
+            a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, w.nc && a.setAttribute("nonce", w.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
             var f = (r, n) => {
                     a.onerror = a.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
-            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), d && document.head.appendChild(a)
+            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), u && document.head.appendChild(a)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -95,25 +95,25 @@
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
                 w.o(w.S, t) || (w.S[t] = {});
                 var i = w.S[t],
                     a = "@deephaven/ipywidgets",
-                    d = (e, r, t, n) => {
+                    u = (e, r, t, n) => {
                         var o = i[e] = i[e] || {},
-                            d = o[r];
-                        (!d || !d.loaded && (!n != !d.eager ? n : a > d.from)) && (o[r] = {
+                            u = o[r];
+                        (!u || !u.loaded && (!n != !u.eager ? n : a > u.from)) && (o[r] = {
                             get: t,
                             from: a,
                             eager: !!n
                         })
                     },
-                    u = [];
-                return "default" === t && (d("@deephaven/ipywidgets", "0.1.0", (() => Promise.all([w.e(790), w.e(568)]).then((() => () => w(568))))), d("@deephaven/log", "0.15.0", (() => w.e(701).then((() => () => w(701)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    l = [];
+                return "default" === t && (u("@deephaven/ipywidgets", "0.1.0", (() => Promise.all([w.e(790), w.e(568)]).then((() => () => w(568))))), u("@deephaven/log", "0.15.0", (() => w.e(701).then((() => () => w(701)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -131,91 +131,91 @@
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var o = e[n],
                 i = (typeof o)[0];
             if (n >= r.length) return "u" == i;
             var a = r[n],
-                d = (typeof a)[0];
-            if (i != d) return "o" == i && "n" == d || "s" == d || "u" == i;
+                u = (typeof a)[0];
+            if (i != u) return "o" == i && "n" == u || "s" == u || "u" == i;
             if ("o" != i && "u" != i && o != a) return o < a;
             n++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(d = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, d);
+            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(u = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var a = [];
         for (i = 1; i < e.length; i++) {
-            var d = e[i];
-            a.push(0 === d ? "not(" + u() + ")" : 1 === d ? "(" + u() + " || " + u() + ")" : 2 === d ? a.pop() + " " + a.pop() : o(d))
+            var u = e[i];
+            a.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
         }
-        return u();
+        return l();
 
-        function u() {
+        function l() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var a = 0, d = 1, u = !0;; d++, a++) {
-                var l, s, f = d < e.length ? (typeof e[d])[0] : "";
-                if (a >= r.length || "o" == (s = (typeof(l = r[a]))[0])) return !u || ("u" == f ? d > n && !o : "" == f != o);
-                if ("u" == s) {
-                    if (!u || "u" != f) return !1
-                } else if (u)
-                    if (f == s)
-                        if (d <= n) {
-                            if (l != e[d]) return !1
+            for (var a = 0, u = 1, l = !0;; u++, a++) {
+                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
+                if (a >= r.length || "o" == (d = (typeof(s = r[a]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
+                if ("u" == d) {
+                    if (!l || "u" != f) return !1
+                } else if (l)
+                    if (f == d)
+                        if (u <= n) {
+                            if (s != e[u]) return !1
                         } else {
-                            if (o ? l > e[d] : l < e[d]) return !1;
-                            l != e[d] && (u = !1)
+                            if (o ? s > e[u] : s < e[u]) return !1;
+                            s != e[u] && (l = !1)
                         }
                 else if ("s" != f && "n" != f) {
-                    if (o || d <= n) return !1;
-                    u = !1, d--
+                    if (o || u <= n) return !1;
+                    l = !1, u--
                 } else {
-                    if (d <= n || s < f != o) return !1;
-                    u = !1
-                } else "s" != f && "n" != f && (u = !1, d--)
+                    if (u <= n || d < f != o) return !1;
+                    l = !1
+                } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
         }
         return !!c()
     }, a = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, d = (e, r) => {
+    }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
-        var o = d(e, t);
-        return i(n, o) || "undefined" != typeof console && console.warn && console.warn(u(e, t, o, n)), f(e[t][o])
-    }, s = (e, r, t) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+        var o = u(e, t);
+        return i(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), f(e[t][o])
+    }, d = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, f = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, o) {
         var i = w.I(r);
         return i && i.then ? i.then(e.bind(e, r, w.S[r], t, n, o)) : e(r, w.S[r], t, n, o)
-    })(((e, r, t, n) => (a(e, t), l(r, 0, t, n)))), h = p(((e, r, t, n, o) => {
-        var i = r && w.o(r, t) && s(r, t, n);
+    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), h = p(((e, r, t, n, o) => {
+        var i = r && w.o(r, t) && d(r, t, n);
         return i ? f(i) : o()
     })), v = {}, g = {
         565: () => c("default", "@jupyter-widgets/base", [, [1, 4, 0, 0],
             [1, 3, 0, 0],
             [1, 2, 0, 0],
             [1, 1, 1, 10], 1, 1, 1
         ]),
@@ -261,21 +261,21 @@
                             i = t && t.target && t.target.src;
                         a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, o, [i, a, d] = t,
-                    u = 0;
+                var n, o, [i, a, u] = t,
+                    l = 0;
                 if (i.some((r => 0 !== e[r]))) {
                     for (n in a) w.o(a, n) && (w.m[n] = a[n]);
-                    d && d(w)
+                    u && u(w)
                 }
-                for (r && r(t); u < i.length; u++) o = i[u], w.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < i.length; l++) o = i[l], w.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_deephaven_ipywidgets = self.webpackChunk_deephaven_ipywidgets || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), w.nc = void 0;
-    var S = w(393);
+    var S = w(690);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@deephaven/ipywidgets"] = S
 })();
```

### Comparing `deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/labextension/static/third-party-licenses.json` & `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/nbextension/index.js` & `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/nbextension/index.js`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/nbextension/index.js.map` & `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/tests/conftest.py` & `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/deephaven_ipywidgets/tests/test_table.py` & `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/docs/Makefile` & `deephaven_ipywidgets-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/docs/make.bat` & `deephaven_ipywidgets-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/docs/source/_static/embed-bundle.js` & `deephaven_ipywidgets-0.2.2/docs/source/_static/embed-bundle.js`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/docs/source/_static/embed-bundle.js.map` & `deephaven_ipywidgets-0.2.2/docs/source/_static/embed-bundle.js.map`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/docs/source/conf.py` & `deephaven_ipywidgets-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/docs/source/develop-install.rst` & `deephaven_ipywidgets-0.2.2/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/docs/source/index.rst` & `deephaven_ipywidgets-0.2.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/docs/source/installing.rst` & `deephaven_ipywidgets-0.2.2/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/examples/introduction.ipynb` & `deephaven_ipywidgets-0.2.2/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/package.json` & `deephaven_ipywidgets-0.2.2/deephaven_ipywidgets/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.6443de594d4e2715e64f.js'), "*

 * *                 "('extension', './extension')])}"}*

```diff
@@ -57,14 +57,18 @@
     "files": [
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/deephaven/deephaven-ipywidgets",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.6443de594d4e2715e64f.js"
+        },
         "extension": "lib/plugin",
         "outputDir": "deephaven_ipywidgets/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
```

### Comparing `deephaven_ipywidgets-0.2.1/setup.py` & `deephaven_ipywidgets-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/src/__tests__/index.spec.ts` & `deephaven_ipywidgets-0.2.2/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/src/__tests__/utils.ts` & `deephaven_ipywidgets-0.2.2/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/src/extension.ts` & `deephaven_ipywidgets-0.2.2/src/extension.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/src/plugin.ts` & `deephaven_ipywidgets-0.2.2/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/src/version.ts` & `deephaven_ipywidgets-0.2.2/src/version.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/src/widget.ts` & `deephaven_ipywidgets-0.2.2/src/widget.ts`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/tsconfig.json` & `deephaven_ipywidgets-0.2.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `deephaven_ipywidgets-0.2.1/webpack.config.js` & `deephaven_ipywidgets-0.2.2/webpack.config.js`

 * *Files identical despite different names*

