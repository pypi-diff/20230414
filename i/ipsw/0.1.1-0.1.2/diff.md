# Comparing `tmp/ipsw-0.1.1.tar.gz` & `tmp/ipsw-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipsw-0.1.1.tar", last modified: Sat Apr  8 15:31:23 2023, max compression
+gzip compressed data, was "ipsw-0.1.2.tar", last modified: Fri Apr 14 05:30:00 2023, max compression
```

## Comparing `ipsw-0.1.1.tar` & `ipsw-0.1.2.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.084587 ipsw-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-08 15:31:12.000000 ipsw-0.1.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.080587 ipsw-0.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-08 15:31:12.000000 ipsw-0.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.080587 ipsw-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-08 15:31:12.000000 ipsw-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-08 15:31:12.000000 ipsw-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-08 15:31:12.000000 ipsw-0.1.1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.080587 ipsw-0.1.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-08 15:31:12.000000 ipsw-0.1.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-08 15:31:12.000000 ipsw-0.1.1/Dockerfile-docs
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-08 15:31:12.000000 ipsw-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-08 15:31:12.000000 ipsw-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-08 15:31:12.000000 ipsw-0.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-08 15:31:23.084587 ipsw-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-08 15:31:12.000000 ipsw-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.080587 ipsw-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.080587 ipsw-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-08 15:31:12.000000 ipsw-0.1.1/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.080587 ipsw-0.1.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-08 15:31:12.000000 ipsw-0.1.1/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-08 15:31:12.000000 ipsw-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-08 15:31:12.000000 ipsw-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-08 15:31:12.000000 ipsw-0.1.1/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.080587 ipsw-0.1.1/ipsw/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-08 15:31:23.000000 ipsw-0.1.1/ipsw/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.080587 ipsw-0.1.1/ipsw/api/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/api/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.080587 ipsw-0.1.1/ipsw/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/models/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/models/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/models/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.080587 ipsw-0.1.1/ipsw/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/transport/basehttpadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/transport/npipeconn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/transport/npipesocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/transport/sshconn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/transport/unixconn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.080587 ipsw-0.1.1/ipsw/types/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/types/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.084587 ipsw-0.1.1/ipsw/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/utils/json_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/utils/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-08 15:31:12.000000 ipsw-0.1.1/ipsw/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.080587 ipsw-0.1.1/ipsw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-08 15:31:23.000000 ipsw-0.1.1/ipsw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-08 15:31:23.000000 ipsw-0.1.1/ipsw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 15:31:23.000000 ipsw-0.1.1/ipsw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 15:31:23.000000 ipsw-0.1.1/ipsw.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-08 15:31:23.000000 ipsw-0.1.1/ipsw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-08 15:31:23.000000 ipsw-0.1.1/ipsw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-08 15:31:12.000000 ipsw-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-08 15:31:12.000000 ipsw-0.1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:31:23.084587 ipsw-0.1.1/scripts /
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-08 15:31:12.000000 ipsw-0.1.1/scripts /release.sh
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-08 15:31:23.084587 ipsw-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-08 15:31:12.000000 ipsw-0.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-08 15:31:12.000000 ipsw-0.1.1/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-08 15:31:12.000000 ipsw-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.958048 ipsw-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-14 05:29:50.000000 ipsw-0.1.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.950049 ipsw-0.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 05:29:50.000000 ipsw-0.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.950049 ipsw-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 05:29:50.000000 ipsw-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-14 05:29:50.000000 ipsw-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-14 05:29:50.000000 ipsw-0.1.2/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.950049 ipsw-0.1.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 05:29:50.000000 ipsw-0.1.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-14 05:29:50.000000 ipsw-0.1.2/Dockerfile-docs
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 05:29:50.000000 ipsw-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-14 05:29:50.000000 ipsw-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-14 05:29:50.000000 ipsw-0.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-14 05:30:00.958048 ipsw-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-14 05:29:50.000000 ipsw-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.950049 ipsw-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-14 05:29:50.000000 ipsw-0.1.2/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 05:29:50.000000 ipsw-0.1.2/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-14 05:29:50.000000 ipsw-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-14 05:29:50.000000 ipsw-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 05:29:50.000000 ipsw-0.1.2/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/ipsw/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/ipsw/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15416 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/api/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/api/macho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/ipsw/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/models/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/models/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/models/macho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/models/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/ipsw/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/transport/basehttpadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/transport/npipeconn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/transport/npipesocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/transport/sshconn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/transport/unixconn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/ipsw/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/types/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.958048 ipsw-0.1.2/ipsw/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/json_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/ipsw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 05:29:50.000000 ipsw-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 05:29:50.000000 ipsw-0.1.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.958048 ipsw-0.1.2/scripts /
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-14 05:29:50.000000 ipsw-0.1.2/scripts /release.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-14 05:30:00.958048 ipsw-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-14 05:29:50.000000 ipsw-0.1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 05:29:50.000000 ipsw-0.1.2/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-14 05:29:50.000000 ipsw-0.1.2/tox.ini
```

### Comparing `ipsw-0.1.1/.github/dependabot.yml` & `ipsw-0.1.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/.github/workflows/python-publish.yml` & `ipsw-0.1.2/.github/workflows/python-publish.yml`

 * *Files 17% similar despite different names*

```diff
@@ -31,11 +31,11 @@
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
       env:
         SETUPTOOLS_SCM_PRETEND_VERSION_FOR_IPSW: ${{ inputs.tag }}      
     - name: Publish package
-      uses: pypa/gh-action-pypi-publish@29930c9cf57955dc1b98162d0d8bc3ec80d9e75c
+      uses: pypa/gh-action-pypi-publish@0bf742be3ebe032c25dd15117957dc15d0cfc38d
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `ipsw-0.1.1/.gitignore` & `ipsw-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/LICENSE` & `ipsw-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/PKG-INFO` & `ipsw-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipsw
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for the ipsw Engine API.
 Home-page: https://github.com/blacktop/ipsw-py
 Maintainer: Blacktop
 License: MIT
 Project-URL: Documentation, https://ipsw-py.readthedocs.io
 Project-URL: Changelog, https://ipsw-py.readthedocs.io/en/stable/change-log.html
 Project-URL: Source, https://github.com/blacktop/ipsw-py
@@ -46,18 +46,33 @@
 
 ## `NOTE:` This is a work in progress ⚠️
 
 ## Getting Started
 
 Start the `ipsw` daemon:
 
+### macOS
+
+```bash
+brew install blacktop/tap/ipswd
+brew services start blacktop/tap/ipswd
+```
+
+### Linux
+
+> ⚠️ UNTESTED ⚠️
+
 ```bash
-git clone -b feature/api https://github.com/blacktop/ipsw.git
-cd ipsw
-IPSW_DAEMON_PORT=8080 go run ./cmd/ipswd/main.go start
+sudo snap install ipswd
+```
+
+### Docker
+
+```bash
+docker run -d -p 3993:3993 -v `pwd`:/data blacktop/ipswd start
 ```
 
 ## Installing
 
 The latest stable version is [available on PyPI](https://pypi.org/project/ipsw/). Either add `ipsw` to your `requirements.txt` file or install with **pip**:
 
 ```bash
@@ -65,17 +80,23 @@
 ```
 
 ## Geting Started
 
 ```python
 import ipsw
 
-client = ipsw.IpswClient(base_url='tcp://127.0.0.1:8080')
-info = client.info.get("iPhone15,2_16.4_20E246_Restore.ipsw")
+client = ipsw.IpswClient(base_url='tcp://127.0.0.1:3993')
+info = client.info.get("iPhone15,2_16.5_20F5028e_Restore.ipsw")
 print(f'{info.version} ({info.build})')
+for device in info.devices:
+    print(f'- {device}')
+```
+```bash
+16.5 (20F5028e)
+- iPhone 14 Pro
 ```
 
 ## Community
 
 You have questions, need support and or just want to talk about `ipsw-py`?
 
 Here are ways to get in touch with the `ipsw-py` community:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ipsw Version: 0.1.1 Summary: A Python library for
+Metadata-Version: 2.1 Name: ipsw Version: 0.1.2 Summary: A Python library for
 the ipsw Engine API. Home-page: https://github.com/blacktop/ipsw-py Maintainer:
 Blacktop License: MIT Project-URL: Documentation, https://ipsw-
 py.readthedocs.io Project-URL: Changelog, https://ipsw-py.readthedocs.io/en/
 stable/change-log.html Project-URL: Source, https://github.com/blacktop/ipsw-py
 Project-URL: Tracker, https://github.com/blacktop/ipsw-py/issues Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Other
 Environment Classifier: Intended Audience :: Developers Classifier: Operating
@@ -18,24 +18,27 @@
                              ****** ipsw-py ******
 *** ipsw SDK for Python ð§ ***
   [https://github.com/blacktop/ipsw-py/actions/workflows/python-publish.yml/
 badge.svg] [https://img.shields.io/pypi/v/ipsw.svg] [PyPI_-_Downloads] [https:/
                     /img.shields.io/:license-mit-blue.svg]
 
 ## `NOTE:` This is a work in progress â ï¸ ## Getting Started Start the
-`ipsw` daemon: ```bash git clone -b feature/api https://github.com/blacktop/
-ipsw.git cd ipsw IPSW_DAEMON_PORT=8080 go run ./cmd/ipswd/main.go start ``` ##
-Installing The latest stable version is [available on PyPI](https://pypi.org/
-project/ipsw/). Either add `ipsw` to your `requirements.txt` file or install
-with **pip**: ```bash pip install ipsw ``` ## Geting Started ```python import
-ipsw client = ipsw.IpswClient(base_url='tcp://127.0.0.1:8080') info =
-client.info.get("iPhone15,2_16.4_20E246_Restore.ipsw") print(f'{info.version} (
-{info.build})') ``` ## Community You have questions, need support and or just
-want to talk about `ipsw-py`? Here are ways to get in touch with the `ipsw-py`
-community: [![Join Discord](https://img.shields.io/badge/
+`ipsw` daemon: ### macOS ```bash brew install blacktop/tap/ipswd brew services
+start blacktop/tap/ipswd ``` ### Linux > â ï¸ UNTESTED â ï¸ ```bash sudo
+snap install ipswd ``` ### Docker ```bash docker run -d -p 3993:3993 -v `pwd`:/
+data blacktop/ipswd start ``` ## Installing The latest stable version is
+[available on PyPI](https://pypi.org/project/ipsw/). Either add `ipsw` to your
+`requirements.txt` file or install with **pip**: ```bash pip install ipsw ```
+## Geting Started ```python import ipsw client = ipsw.IpswClient(base_url='tcp:
+//127.0.0.1:3993') info = client.info.get
+("iPhone15,2_16.5_20F5028e_Restore.ipsw") print(f'{info.version} (
+{info.build})') for device in info.devices: print(f'- {device}') ``` ```bash
+16.5 (20F5028e) - iPhone 14 Pro ``` ## Community You have questions, need
+support and or just want to talk about `ipsw-py`? Here are ways to get in touch
+with the `ipsw-py` community: [![Join Discord](https://img.shields.io/badge/
 Join_our_Discord_server-5865F2?style=for-the-
 badge&logo=discord&logoColor=white)](https://discord.gg/xx2y9yrcgs) [![Follow
 Twitter](https://img.shields.io/badge/follow_on_twitter-1DA1F2?style=for-the-
 badge&logo=twitter&logoColor=white)](https://twitter.com/blacktop__) [![Follow
 Mastodon](https://img.shields.io/badge/follow_on_mastodon-6364FF?style=for-the-
 badge&logo=mastodon&logoColor=white)](https://mastodon.social/@blacktop) [!
 [GitHub Discussions](https://img.shields.io/badge/GITHUB_DISCUSSION-
```

### Comparing `ipsw-0.1.1/README.md` & `ipsw-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -15,18 +15,33 @@
 
 ## `NOTE:` This is a work in progress ⚠️
 
 ## Getting Started
 
 Start the `ipsw` daemon:
 
+### macOS
+
+```bash
+brew install blacktop/tap/ipswd
+brew services start blacktop/tap/ipswd
+```
+
+### Linux
+
+> ⚠️ UNTESTED ⚠️
+
 ```bash
-git clone -b feature/api https://github.com/blacktop/ipsw.git
-cd ipsw
-IPSW_DAEMON_PORT=8080 go run ./cmd/ipswd/main.go start
+sudo snap install ipswd
+```
+
+### Docker
+
+```bash
+docker run -d -p 3993:3993 -v `pwd`:/data blacktop/ipswd start
 ```
 
 ## Installing
 
 The latest stable version is [available on PyPI](https://pypi.org/project/ipsw/). Either add `ipsw` to your `requirements.txt` file or install with **pip**:
 
 ```bash
@@ -34,17 +49,23 @@
 ```
 
 ## Geting Started
 
 ```python
 import ipsw
 
-client = ipsw.IpswClient(base_url='tcp://127.0.0.1:8080')
-info = client.info.get("iPhone15,2_16.4_20E246_Restore.ipsw")
+client = ipsw.IpswClient(base_url='tcp://127.0.0.1:3993')
+info = client.info.get("iPhone15,2_16.5_20F5028e_Restore.ipsw")
 print(f'{info.version} ({info.build})')
+for device in info.devices:
+    print(f'- {device}')
+```
+```bash
+16.5 (20F5028e)
+- iPhone 14 Pro
 ```
 
 ## Community
 
 You have questions, need support and or just want to talk about `ipsw-py`?
 
 Here are ways to get in touch with the `ipsw-py` community:
```

#### html2text {}

```diff
@@ -1,24 +1,27 @@
                              ****** ipsw-py ******
 *** ipsw SDK for Python ð§ ***
   [https://github.com/blacktop/ipsw-py/actions/workflows/python-publish.yml/
 badge.svg] [https://img.shields.io/pypi/v/ipsw.svg] [PyPI_-_Downloads] [https:/
                     /img.shields.io/:license-mit-blue.svg]
 
 ## `NOTE:` This is a work in progress â ï¸ ## Getting Started Start the
-`ipsw` daemon: ```bash git clone -b feature/api https://github.com/blacktop/
-ipsw.git cd ipsw IPSW_DAEMON_PORT=8080 go run ./cmd/ipswd/main.go start ``` ##
-Installing The latest stable version is [available on PyPI](https://pypi.org/
-project/ipsw/). Either add `ipsw` to your `requirements.txt` file or install
-with **pip**: ```bash pip install ipsw ``` ## Geting Started ```python import
-ipsw client = ipsw.IpswClient(base_url='tcp://127.0.0.1:8080') info =
-client.info.get("iPhone15,2_16.4_20E246_Restore.ipsw") print(f'{info.version} (
-{info.build})') ``` ## Community You have questions, need support and or just
-want to talk about `ipsw-py`? Here are ways to get in touch with the `ipsw-py`
-community: [![Join Discord](https://img.shields.io/badge/
+`ipsw` daemon: ### macOS ```bash brew install blacktop/tap/ipswd brew services
+start blacktop/tap/ipswd ``` ### Linux > â ï¸ UNTESTED â ï¸ ```bash sudo
+snap install ipswd ``` ### Docker ```bash docker run -d -p 3993:3993 -v `pwd`:/
+data blacktop/ipswd start ``` ## Installing The latest stable version is
+[available on PyPI](https://pypi.org/project/ipsw/). Either add `ipsw` to your
+`requirements.txt` file or install with **pip**: ```bash pip install ipsw ```
+## Geting Started ```python import ipsw client = ipsw.IpswClient(base_url='tcp:
+//127.0.0.1:3993') info = client.info.get
+("iPhone15,2_16.5_20F5028e_Restore.ipsw") print(f'{info.version} (
+{info.build})') for device in info.devices: print(f'- {device}') ``` ```bash
+16.5 (20F5028e) - iPhone 14 Pro ``` ## Community You have questions, need
+support and or just want to talk about `ipsw-py`? Here are ways to get in touch
+with the `ipsw-py` community: [![Join Discord](https://img.shields.io/badge/
 Join_our_Discord_server-5865F2?style=for-the-
 badge&logo=discord&logoColor=white)](https://discord.gg/xx2y9yrcgs) [![Follow
 Twitter](https://img.shields.io/badge/follow_on_twitter-1DA1F2?style=for-the-
 badge&logo=twitter&logoColor=white)](https://twitter.com/blacktop__) [![Follow
 Mastodon](https://img.shields.io/badge/follow_on_mastodon-6364FF?style=for-the-
 badge&logo=mastodon&logoColor=white)](https://mastodon.social/@blacktop) [!
 [GitHub Discussions](https://img.shields.io/badge/GITHUB_DISCUSSION-
```

### Comparing `ipsw-0.1.1/docs/conf.py` & `ipsw-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/docs/index.rst` & `ipsw-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/api/client.py` & `ipsw-0.1.2/ipsw/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from ..transport import UnixHTTPAdapter
 from ..utils import config, update_headers, utils
 from ..utils.json_stream import json_stream
 from ..utils.proxy import ProxyConfig
 from ..utils.socket import consume_socket_output, demux_adaptor, frames_iter
 from .daemon import DaemonApiMixin
 from .info import InfoApiMixin
+from .macho import MachoApiMixin
 
 try:
     from ..transport import NpipeHTTPAdapter
 except ImportError:
     pass
 
 try:
@@ -31,15 +32,16 @@
 except ImportError:
     pass
 
 
 class APIClient(
         requests.Session,
         DaemonApiMixin,
-        InfoApiMixin):
+        InfoApiMixin,
+        MachoApiMixin):
     """
     A low-level client for the ipsw API.
 
     Example:
 
         >>> import ipsw
         >>> client = ipsw.APIClient(base_url='unix://var/run/ipsw.sock')
```

### Comparing `ipsw-0.1.1/ipsw/api/daemon.py` & `ipsw-0.1.2/ipsw/api/daemon.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/api/info.py` & `ipsw-0.1.2/ipsw/api/info.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/client.py` & `ipsw-0.1.2/ipsw/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .api.client import APIClient
 from .constants import (DEFAULT_TIMEOUT_SECONDS, DEFAULT_MAX_POOL_SIZE)
 from .models.info import InfoCollection
+from .models.macho import MachoCollection
 from .utils import kwargs_from_env
 
 
 class IpswClient:
     """
     A client for communicating with a ipsw server.
 
@@ -74,14 +75,21 @@
 
     @property
     def info(self):
         """
         An object for getting local/remote IPSW/OTA info.
         """
         return InfoCollection(client=self)
+    
+    @property
+    def macho(self):
+        """
+        An object for getting MachO info.
+        """
+        return MachoCollection(client=self)
 
     # Top-level methods
     def ping(self, *args, **kwargs):
         return self.api.ping(*args, **kwargs)
     ping.__doc__ = APIClient.ping.__doc__
 
     def version(self, *args, **kwargs):
```

### Comparing `ipsw-0.1.1/ipsw/constants.py` & `ipsw-0.1.2/ipsw/constants.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/errors.py` & `ipsw-0.1.2/ipsw/errors.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/models/configs.py` & `ipsw-0.1.2/ipsw/models/configs.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/models/info.py` & `ipsw-0.1.2/ipsw/models/macho.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 import os
 
 from ..api import APIClient
 from .resource import Collection, Model
 
 
-class Info(Model):
+class Macho(Model):
     """
-    IPSW/OTA info.
+    MachO info.
     """
 
     def __repr__(self):
-        return "<{}: '{} ({})'>".format(
+        return "<{}: '{} {} ({})'>".format(
             self.__class__.__name__,
-            self.version,
-            self.build,
+            self.magic,
+            self.cpu,
+            self.sub_cpu,
         )
 
     @property
-    def version(self):
+    def magic(self):
         """
-        The iOS version.
+        The header magic.
         """
-        return self.attrs["info"]["Plists"]["restore"].get("ProductVersion", None)
+        return self.attrs["info"]['header'].get("magic", None)
 
     @property
-    def build(self):
+    def cpu(self):
         """
-        The iOS version.
+        The header CPU.
         """
-        return self.attrs["info"]["Plists"]["restore"].get("ProductBuildVersion", None)
+        return self.attrs["info"]['header'].get("cpu", None)
+    
+    @property
+    def sub_cpu(self):
+        """
+        The header sub CPU.
+        """
+        return self.attrs["info"]['header'].get("subcpu", None)
 
 
-class InfoCollection(Collection):
-    model = Info
+class MachoCollection(Collection):
+    model = Macho
 
-    def get(self, ipsw=None, ota=None, url=None):
+    def get(self, path=None, arch=None):
         """
-        The iOS version.
+        Get MachO info.
         """
-        if url:
-            return self.prepare_model(self.client.api.remote_ipsw_info(url))
-        else:
-            if ipsw:
-                return self.prepare_model(self.client.api.ipsw_info(os.path.abspath(ipsw)))
-            elif ota:
-                return self.prepare_model(self.client.api.ipsw_info(os.path.abspath(ipsw)))
+        return self.prepare_model(self.client.api.macho_info(path, arch))
```

### Comparing `ipsw-0.1.1/ipsw/models/resource.py` & `ipsw-0.1.2/ipsw/models/resource.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/transport/npipeconn.py` & `ipsw-0.1.2/ipsw/transport/npipeconn.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/transport/npipesocket.py` & `ipsw-0.1.2/ipsw/transport/npipesocket.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/transport/sshconn.py` & `ipsw-0.1.2/ipsw/transport/sshconn.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/transport/unixconn.py` & `ipsw-0.1.2/ipsw/transport/unixconn.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/types/daemon.py` & `ipsw-0.1.2/ipsw/types/daemon.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/utils/config.py` & `ipsw-0.1.2/ipsw/utils/config.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/utils/decorators.py` & `ipsw-0.1.2/ipsw/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/utils/json_stream.py` & `ipsw-0.1.2/ipsw/utils/json_stream.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/utils/proxy.py` & `ipsw-0.1.2/ipsw/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/utils/socket.py` & `ipsw-0.1.2/ipsw/utils/socket.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/utils/utils.py` & `ipsw-0.1.2/ipsw/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw/version.py` & `ipsw-0.1.2/ipsw/version.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/ipsw.egg-info/PKG-INFO` & `ipsw-0.1.2/ipsw.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipsw
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for the ipsw Engine API.
 Home-page: https://github.com/blacktop/ipsw-py
 Maintainer: Blacktop
 License: MIT
 Project-URL: Documentation, https://ipsw-py.readthedocs.io
 Project-URL: Changelog, https://ipsw-py.readthedocs.io/en/stable/change-log.html
 Project-URL: Source, https://github.com/blacktop/ipsw-py
@@ -46,18 +46,33 @@
 
 ## `NOTE:` This is a work in progress ⚠️
 
 ## Getting Started
 
 Start the `ipsw` daemon:
 
+### macOS
+
+```bash
+brew install blacktop/tap/ipswd
+brew services start blacktop/tap/ipswd
+```
+
+### Linux
+
+> ⚠️ UNTESTED ⚠️
+
 ```bash
-git clone -b feature/api https://github.com/blacktop/ipsw.git
-cd ipsw
-IPSW_DAEMON_PORT=8080 go run ./cmd/ipswd/main.go start
+sudo snap install ipswd
+```
+
+### Docker
+
+```bash
+docker run -d -p 3993:3993 -v `pwd`:/data blacktop/ipswd start
 ```
 
 ## Installing
 
 The latest stable version is [available on PyPI](https://pypi.org/project/ipsw/). Either add `ipsw` to your `requirements.txt` file or install with **pip**:
 
 ```bash
@@ -65,17 +80,23 @@
 ```
 
 ## Geting Started
 
 ```python
 import ipsw
 
-client = ipsw.IpswClient(base_url='tcp://127.0.0.1:8080')
-info = client.info.get("iPhone15,2_16.4_20E246_Restore.ipsw")
+client = ipsw.IpswClient(base_url='tcp://127.0.0.1:3993')
+info = client.info.get("iPhone15,2_16.5_20F5028e_Restore.ipsw")
 print(f'{info.version} ({info.build})')
+for device in info.devices:
+    print(f'- {device}')
+```
+```bash
+16.5 (20F5028e)
+- iPhone 14 Pro
 ```
 
 ## Community
 
 You have questions, need support and or just want to talk about `ipsw-py`?
 
 Here are ways to get in touch with the `ipsw-py` community:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ipsw Version: 0.1.1 Summary: A Python library for
+Metadata-Version: 2.1 Name: ipsw Version: 0.1.2 Summary: A Python library for
 the ipsw Engine API. Home-page: https://github.com/blacktop/ipsw-py Maintainer:
 Blacktop License: MIT Project-URL: Documentation, https://ipsw-
 py.readthedocs.io Project-URL: Changelog, https://ipsw-py.readthedocs.io/en/
 stable/change-log.html Project-URL: Source, https://github.com/blacktop/ipsw-py
 Project-URL: Tracker, https://github.com/blacktop/ipsw-py/issues Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Other
 Environment Classifier: Intended Audience :: Developers Classifier: Operating
@@ -18,24 +18,27 @@
                              ****** ipsw-py ******
 *** ipsw SDK for Python ð§ ***
   [https://github.com/blacktop/ipsw-py/actions/workflows/python-publish.yml/
 badge.svg] [https://img.shields.io/pypi/v/ipsw.svg] [PyPI_-_Downloads] [https:/
                     /img.shields.io/:license-mit-blue.svg]
 
 ## `NOTE:` This is a work in progress â ï¸ ## Getting Started Start the
-`ipsw` daemon: ```bash git clone -b feature/api https://github.com/blacktop/
-ipsw.git cd ipsw IPSW_DAEMON_PORT=8080 go run ./cmd/ipswd/main.go start ``` ##
-Installing The latest stable version is [available on PyPI](https://pypi.org/
-project/ipsw/). Either add `ipsw` to your `requirements.txt` file or install
-with **pip**: ```bash pip install ipsw ``` ## Geting Started ```python import
-ipsw client = ipsw.IpswClient(base_url='tcp://127.0.0.1:8080') info =
-client.info.get("iPhone15,2_16.4_20E246_Restore.ipsw") print(f'{info.version} (
-{info.build})') ``` ## Community You have questions, need support and or just
-want to talk about `ipsw-py`? Here are ways to get in touch with the `ipsw-py`
-community: [![Join Discord](https://img.shields.io/badge/
+`ipsw` daemon: ### macOS ```bash brew install blacktop/tap/ipswd brew services
+start blacktop/tap/ipswd ``` ### Linux > â ï¸ UNTESTED â ï¸ ```bash sudo
+snap install ipswd ``` ### Docker ```bash docker run -d -p 3993:3993 -v `pwd`:/
+data blacktop/ipswd start ``` ## Installing The latest stable version is
+[available on PyPI](https://pypi.org/project/ipsw/). Either add `ipsw` to your
+`requirements.txt` file or install with **pip**: ```bash pip install ipsw ```
+## Geting Started ```python import ipsw client = ipsw.IpswClient(base_url='tcp:
+//127.0.0.1:3993') info = client.info.get
+("iPhone15,2_16.5_20F5028e_Restore.ipsw") print(f'{info.version} (
+{info.build})') for device in info.devices: print(f'- {device}') ``` ```bash
+16.5 (20F5028e) - iPhone 14 Pro ``` ## Community You have questions, need
+support and or just want to talk about `ipsw-py`? Here are ways to get in touch
+with the `ipsw-py` community: [![Join Discord](https://img.shields.io/badge/
 Join_our_Discord_server-5865F2?style=for-the-
 badge&logo=discord&logoColor=white)](https://discord.gg/xx2y9yrcgs) [![Follow
 Twitter](https://img.shields.io/badge/follow_on_twitter-1DA1F2?style=for-the-
 badge&logo=twitter&logoColor=white)](https://twitter.com/blacktop__) [![Follow
 Mastodon](https://img.shields.io/badge/follow_on_mastodon-6364FF?style=for-the-
 badge&logo=mastodon&logoColor=white)](https://mastodon.social/@blacktop) [!
 [GitHub Discussions](https://img.shields.io/badge/GITHUB_DISCUSSION-
```

### Comparing `ipsw-0.1.1/ipsw.egg-info/SOURCES.txt` & `ipsw-0.1.2/ipsw.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,19 @@
 ipsw.egg-info/not-zip-safe
 ipsw.egg-info/requires.txt
 ipsw.egg-info/top_level.txt
 ipsw/api/__init__.py
 ipsw/api/client.py
 ipsw/api/daemon.py
 ipsw/api/info.py
+ipsw/api/macho.py
 ipsw/models/__init__.py
 ipsw/models/configs.py
 ipsw/models/info.py
+ipsw/models/macho.py
 ipsw/models/resource.py
 ipsw/transport/__init__.py
 ipsw/transport/basehttpadapter.py
 ipsw/transport/npipeconn.py
 ipsw/transport/npipesocket.py
 ipsw/transport/sshconn.py
 ipsw/transport/unixconn.py
```

### Comparing `ipsw-0.1.1/scripts /release.sh` & `ipsw-0.1.2/scripts /release.sh`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.1/setup.py` & `ipsw-0.1.2/setup.py`

 * *Files identical despite different names*

