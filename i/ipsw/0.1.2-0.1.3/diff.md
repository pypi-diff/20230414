# Comparing `tmp/ipsw-0.1.2.tar.gz` & `tmp/ipsw-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipsw-0.1.2.tar", last modified: Fri Apr 14 05:30:00 2023, max compression
+gzip compressed data, was "ipsw-0.1.3.tar", last modified: Fri Apr 14 06:20:47 2023, max compression
```

## Comparing `ipsw-0.1.2.tar` & `ipsw-0.1.3.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.958048 ipsw-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-14 05:29:50.000000 ipsw-0.1.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.950049 ipsw-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 05:29:50.000000 ipsw-0.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.950049 ipsw-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 05:29:50.000000 ipsw-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-14 05:29:50.000000 ipsw-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-14 05:29:50.000000 ipsw-0.1.2/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.950049 ipsw-0.1.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 05:29:50.000000 ipsw-0.1.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-14 05:29:50.000000 ipsw-0.1.2/Dockerfile-docs
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 05:29:50.000000 ipsw-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-14 05:29:50.000000 ipsw-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-14 05:29:50.000000 ipsw-0.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-14 05:30:00.958048 ipsw-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-14 05:29:50.000000 ipsw-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.950049 ipsw-0.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-14 05:29:50.000000 ipsw-0.1.2/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 05:29:50.000000 ipsw-0.1.2/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-14 05:29:50.000000 ipsw-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-14 05:29:50.000000 ipsw-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 05:29:50.000000 ipsw-0.1.2/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/ipsw/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/ipsw/api/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15416 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/api/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/api/macho.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/ipsw/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/models/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/models/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/models/macho.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/models/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/ipsw/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/transport/basehttpadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/transport/npipeconn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/transport/npipesocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/transport/sshconn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/transport/unixconn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/ipsw/types/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/types/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.958048 ipsw-0.1.2/ipsw/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/json_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-14 05:29:50.000000 ipsw-0.1.2/ipsw/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.954048 ipsw-0.1.2/ipsw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 05:30:00.000000 ipsw-0.1.2/ipsw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 05:29:50.000000 ipsw-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 05:29:50.000000 ipsw-0.1.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:30:00.958048 ipsw-0.1.2/scripts /
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-14 05:29:50.000000 ipsw-0.1.2/scripts /release.sh
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-14 05:30:00.958048 ipsw-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-14 05:29:50.000000 ipsw-0.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 05:29:50.000000 ipsw-0.1.2/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-14 05:29:50.000000 ipsw-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-14 06:20:37.000000 ipsw-0.1.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 06:20:37.000000 ipsw-0.1.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 06:20:37.000000 ipsw-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-14 06:20:37.000000 ipsw-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-14 06:20:37.000000 ipsw-0.1.3/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 06:20:37.000000 ipsw-0.1.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-14 06:20:37.000000 ipsw-0.1.3/Dockerfile-docs
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 06:20:37.000000 ipsw-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-14 06:20:37.000000 ipsw-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-14 06:20:37.000000 ipsw-0.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-14 06:20:47.702191 ipsw-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-14 06:20:37.000000 ipsw-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-14 06:20:37.000000 ipsw-0.1.3/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 06:20:37.000000 ipsw-0.1.3/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-14 06:20:37.000000 ipsw-0.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-14 06:20:37.000000 ipsw-0.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 06:20:37.000000 ipsw-0.1.3/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/ipsw/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/ipsw/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/api/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/api/dsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/api/macho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/ipsw/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/models/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/models/dsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/models/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/models/macho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/models/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/ipsw/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/transport/basehttpadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/transport/npipeconn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/transport/npipesocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/transport/sshconn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/transport/unixconn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/ipsw/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/types/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/ipsw/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/json_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-14 06:20:37.000000 ipsw-0.1.3/ipsw/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.698191 ipsw-0.1.3/ipsw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 06:20:47.000000 ipsw-0.1.3/ipsw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 06:20:37.000000 ipsw-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 06:20:37.000000 ipsw-0.1.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:20:47.702191 ipsw-0.1.3/scripts /
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-14 06:20:37.000000 ipsw-0.1.3/scripts /release.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-14 06:20:47.702191 ipsw-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-14 06:20:37.000000 ipsw-0.1.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 06:20:37.000000 ipsw-0.1.3/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-14 06:20:37.000000 ipsw-0.1.3/tox.ini
```

### Comparing `ipsw-0.1.2/.github/dependabot.yml` & `ipsw-0.1.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.2/.github/workflows/python-publish.yml` & `ipsw-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.2/.gitignore` & `ipsw-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.2/LICENSE` & `ipsw-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.2/README.md` & `ipsw-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -46,28 +46,66 @@
 
 ```bash
 pip install ipsw
 ```
 
 ## Geting Started
 
+Get IPSW info
+
 ```python
 import ipsw
 
 client = ipsw.IpswClient(base_url='tcp://127.0.0.1:3993')
+
 info = client.info.get("iPhone15,2_16.5_20F5028e_Restore.ipsw")
 print(f'{info.version} ({info.build})')
 for device in info.devices:
     print(f'- {device}')
 ```
 ```bash
 16.5 (20F5028e)
 - iPhone 14 Pro
 ```
 
+Get DSC info
+
+```python
+import ipsw
+
+client = ipsw.IpswClient(base_url='tcp://127.0.0.1:3993')
+
+dsc = client.dsc.get_info("20F5028e__iPhone15,2/dyld_shared_cache_arm64e")
+print(dsc)
+print(dsc.dylibs[0])
+
+dylib = client.dsc.get_dylib("20F5028e__iPhone15,2/dyld_shared_cache_arm64e", "libswiftCore.dylib")
+print(dylib)
+```
+```bash
+<DSC: '(dyld_v1  arm64e) - iOS - FAEC7714-4CCD-3B99-B18F-F5EAB60DE31E'>
+{'index': 1, 'name': '/usr/lib/libobjc.A.dylib', 'version': '876.0.0.0.0', 'uuid': '085A190C-6214-38EA-ACCB-428C3E8AFA65', 'load_address': 6443204608}
+
+<Dylib: '64-bit MachO AARCH64 (ARM64e)'>
+```
+
+Get MachO info
+
+```python
+import ipsw
+
+client = ipsw.IpswClient(base_url='tcp://127.0.0.1:3993')
+
+macho = client.macho.get("/bin/ls", arch="arm64e")
+print(macho)
+```
+```bash
+<Macho: '64-bit MachO AARCH64 (ARM64e)'>
+```
+
 ## Community
 
 You have questions, need support and or just want to talk about `ipsw-py`?
 
 Here are ways to get in touch with the `ipsw-py` community:
 
 [![Join Discord](https://img.shields.io/badge/Join_our_Discord_server-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/xx2y9yrcgs)
```

#### html2text {}

```diff
@@ -7,19 +7,30 @@
 ## `NOTE:` This is a work in progress â ï¸ ## Getting Started Start the
 `ipsw` daemon: ### macOS ```bash brew install blacktop/tap/ipswd brew services
 start blacktop/tap/ipswd ``` ### Linux > â ï¸ UNTESTED â ï¸ ```bash sudo
 snap install ipswd ``` ### Docker ```bash docker run -d -p 3993:3993 -v `pwd`:/
 data blacktop/ipswd start ``` ## Installing The latest stable version is
 [available on PyPI](https://pypi.org/project/ipsw/). Either add `ipsw` to your
 `requirements.txt` file or install with **pip**: ```bash pip install ipsw ```
-## Geting Started ```python import ipsw client = ipsw.IpswClient(base_url='tcp:
-//127.0.0.1:3993') info = client.info.get
+## Geting Started Get IPSW info ```python import ipsw client = ipsw.IpswClient
+(base_url='tcp://127.0.0.1:3993') info = client.info.get
 ("iPhone15,2_16.5_20F5028e_Restore.ipsw") print(f'{info.version} (
 {info.build})') for device in info.devices: print(f'- {device}') ``` ```bash
-16.5 (20F5028e) - iPhone 14 Pro ``` ## Community You have questions, need
+16.5 (20F5028e) - iPhone 14 Pro ``` Get DSC info ```python import ipsw client =
+ipsw.IpswClient(base_url='tcp://127.0.0.1:3993') dsc = client.dsc.get_info
+("20F5028e__iPhone15,2/dyld_shared_cache_arm64e") print(dsc) print(dsc.dylibs
+[0]) dylib = client.dsc.get_dylib("20F5028e__iPhone15,2/
+dyld_shared_cache_arm64e", "libswiftCore.dylib") print(dylib) ``` ```bash
+(dyld_v1 arm64e) - iOS - FAEC7714-4CCD-3B99-B18F-F5EAB60DE31E'> {'index': 1,
+'name': '/usr/lib/libobjc.A.dylib', 'version': '876.0.0.0.0', 'uuid':
+'085A190C-6214-38EA-ACCB-428C3E8AFA65', 'load_address': 6443204608}
+64-bit MachO AARCH64 (ARM64e)'> ``` Get MachO info ```python import ipsw client
+= ipsw.IpswClient(base_url='tcp://127.0.0.1:3993') macho = client.macho.get("/
+bin/ls", arch="arm64e") print(macho) ``` ```bash
+64-bit MachO AARCH64 (ARM64e)'> ``` ## Community You have questions, need
 support and or just want to talk about `ipsw-py`? Here are ways to get in touch
 with the `ipsw-py` community: [![Join Discord](https://img.shields.io/badge/
 Join_our_Discord_server-5865F2?style=for-the-
 badge&logo=discord&logoColor=white)](https://discord.gg/xx2y9yrcgs) [![Follow
 Twitter](https://img.shields.io/badge/follow_on_twitter-1DA1F2?style=for-the-
 badge&logo=twitter&logoColor=white)](https://twitter.com/blacktop__) [![Follow
 Mastodon](https://img.shields.io/badge/follow_on_mastodon-6364FF?style=for-the-
```

### Comparing `ipsw-0.1.2/docs/conf.py` & `ipsw-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.2/docs/index.rst` & `ipsw-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.2/ipsw/api/client.py` & `ipsw-0.1.3/ipsw/api/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,45 +3,47 @@
 import urllib
 from functools import partial
 
 import requests
 import requests.exceptions
 import websocket
 
-from ..constants import (DEFAULT_MAX_POOL_SIZE, DEFAULT_NUM_POOLS,
-                         DEFAULT_NUM_POOLS_SSH, DEFAULT_TIMEOUT_SECONDS,
-                         DEFAULT_USER_AGENT, IS_WINDOWS_PLATFORM,
-                         MINIMUM_IPSW_API_VERSION, STREAM_HEADER_SIZE_BYTES)
-from ..errors import (InvalidVersion, IpswException,
-                      create_api_error_from_http_exception)
+from ..constants import (
+    DEFAULT_MAX_POOL_SIZE,
+    DEFAULT_NUM_POOLS,
+    DEFAULT_NUM_POOLS_SSH,
+    DEFAULT_TIMEOUT_SECONDS,
+    DEFAULT_USER_AGENT,
+    IS_WINDOWS_PLATFORM,
+    MINIMUM_IPSW_API_VERSION,
+    STREAM_HEADER_SIZE_BYTES,
+)
+from ..errors import InvalidVersion, IpswException, create_api_error_from_http_exception
 from ..transport import UnixHTTPAdapter
 from ..utils import config, update_headers, utils
 from ..utils.json_stream import json_stream
 from ..utils.proxy import ProxyConfig
 from ..utils.socket import consume_socket_output, demux_adaptor, frames_iter
 from .daemon import DaemonApiMixin
+from .dsc import DscApiMixin
 from .info import InfoApiMixin
 from .macho import MachoApiMixin
 
 try:
     from ..transport import NpipeHTTPAdapter
 except ImportError:
     pass
 
 try:
     from ..transport import SSHHTTPAdapter
 except ImportError:
     pass
 
 
-class APIClient(
-        requests.Session,
-        DaemonApiMixin,
-        InfoApiMixin,
-        MachoApiMixin):
+class APIClient(requests.Session, DaemonApiMixin, DscApiMixin, InfoApiMixin, MachoApiMixin):
     """
     A low-level client for the ipsw API.
 
     Example:
 
         >>> import ipsw
         >>> client = ipsw.APIClient(base_url='unix://var/run/ipsw.sock')
@@ -64,126 +66,106 @@
         use_ssh_client (bool): If set to `True`, an ssh connection is made
             via shelling out to the ssh client. Ensure the ssh client is
             installed and configured on the host.
         max_pool_size (int): The maximum number of connections
             to save in the pool.
     """
 
-    __attrs__ = requests.Session.__attrs__ + ['_general_configs',
-                                              '_version',
-                                              'base_url',
-                                              'timeout']
-
-    def __init__(self, base_url=None, version=None,
-                 timeout=DEFAULT_TIMEOUT_SECONDS,
-                 user_agent=DEFAULT_USER_AGENT, num_pools=None,
-                 use_ssh_client=False,
-                 max_pool_size=DEFAULT_MAX_POOL_SIZE):
+    __attrs__ = requests.Session.__attrs__ + ["_general_configs", "_version", "base_url", "timeout"]
+
+    def __init__(
+        self,
+        base_url=None,
+        version=None,
+        timeout=DEFAULT_TIMEOUT_SECONDS,
+        user_agent=DEFAULT_USER_AGENT,
+        num_pools=None,
+        use_ssh_client=False,
+        max_pool_size=DEFAULT_MAX_POOL_SIZE,
+    ):
         super().__init__()
 
         self.base_url = base_url
         self.timeout = timeout
-        self.headers['User-Agent'] = user_agent
+        self.headers["User-Agent"] = user_agent
 
         self._general_configs = config.load_general_config()
 
-        proxy_config = self._general_configs.get('proxies', {})
+        proxy_config = self._general_configs.get("proxies", {})
         try:
             proxies = proxy_config[base_url]
         except KeyError:
-            proxies = proxy_config.get('default', {})
+            proxies = proxy_config.get("default", {})
 
         self._proxy_configs = ProxyConfig.from_dict(proxies)
 
         base_url = utils.parse_host(
-            base_url, IS_WINDOWS_PLATFORM,
+            base_url,
+            IS_WINDOWS_PLATFORM,
         )
         # SSH has a different default for num_pools to all other adapters
-        num_pools = num_pools or DEFAULT_NUM_POOLS_SSH if \
-            base_url.startswith('ssh://') else DEFAULT_NUM_POOLS
+        num_pools = num_pools or DEFAULT_NUM_POOLS_SSH if base_url.startswith("ssh://") else DEFAULT_NUM_POOLS
 
-        if base_url.startswith('http+unix://'):
+        if base_url.startswith("http+unix://"):
             self._custom_adapter = UnixHTTPAdapter(
-                base_url, timeout, pool_connections=num_pools,
-                max_pool_size=max_pool_size
+                base_url, timeout, pool_connections=num_pools, max_pool_size=max_pool_size
             )
-            self.mount('http+ipsw://', self._custom_adapter)
-            self._unmount('http://', 'https://')
+            self.mount("http+ipsw://", self._custom_adapter)
+            self._unmount("http://", "https://")
             # host part of URL should be unused, but is resolved by requests
             # module in proxy_bypass_macosx_sysconf()
-            self.base_url = 'http+ipsw://localhost'
-        elif base_url.startswith('npipe://'):
+            self.base_url = "http+ipsw://localhost"
+        elif base_url.startswith("npipe://"):
             if not IS_WINDOWS_PLATFORM:
-                raise IpswException(
-                    'The npipe:// protocol is only supported on Windows'
-                )
+                raise IpswException("The npipe:// protocol is only supported on Windows")
             try:
                 self._custom_adapter = NpipeHTTPAdapter(
-                    base_url, timeout, pool_connections=num_pools,
-                    max_pool_size=max_pool_size
+                    base_url, timeout, pool_connections=num_pools, max_pool_size=max_pool_size
                 )
             except NameError:
-                raise IpswException(
-                    'Install pypiwin32 package to enable npipe:// support'
-                )
-            self.mount('http+ipsw://', self._custom_adapter)
-            self.base_url = 'http+ipsw://localnpipe'
-        elif base_url.startswith('ssh://'):
+                raise IpswException("Install pypiwin32 package to enable npipe:// support")
+            self.mount("http+ipsw://", self._custom_adapter)
+            self.base_url = "http+ipsw://localnpipe"
+        elif base_url.startswith("ssh://"):
             try:
                 self._custom_adapter = SSHHTTPAdapter(
-                    base_url, timeout, pool_connections=num_pools,
-                    max_pool_size=max_pool_size, shell_out=use_ssh_client
+                    base_url, timeout, pool_connections=num_pools, max_pool_size=max_pool_size, shell_out=use_ssh_client
                 )
             except NameError:
-                raise IpswException(
-                    'Install paramiko package to enable ssh:// support'
-                )
-            self.mount('http+ipsw://ssh', self._custom_adapter)
-            self._unmount('http://', 'https://')
-            self.base_url = 'http+ipsw://ssh'
+                raise IpswException("Install paramiko package to enable ssh:// support")
+            self.mount("http+ipsw://ssh", self._custom_adapter)
+            self._unmount("http://", "https://")
+            self.base_url = "http+ipsw://ssh"
         else:
             self.base_url = base_url
 
         # version detection needs to be after unix adapter mounting
-        if version is None or (isinstance(
-                                version,
-                                str
-                                ) and version.lower() == 'auto'):
+        if version is None or (isinstance(version, str) and version.lower() == "auto"):
             self._version = self._retrieve_server_version()
         else:
             self._version = version
         if not isinstance(self._version, str):
-            raise IpswException(
-                'Version parameter must be a string or None. Found {}'.format(
-                    type(version).__name__
-                )
-            )
+            raise IpswException("Version parameter must be a string or None. Found {}".format(type(version).__name__))
         if utils.version_lt(self._version, MINIMUM_IPSW_API_VERSION):
             raise InvalidVersion(
-                'API versions below {} are no longer supported by this '
-                'library.'.format(MINIMUM_IPSW_API_VERSION)
+                "API versions below {} are no longer supported by this " "library.".format(MINIMUM_IPSW_API_VERSION)
             )
 
     def _retrieve_server_version(self):
         try:
             return self.version(api_version=False)["ApiVersion"]
         except KeyError:
-            raise IpswException(
-                'Invalid response from ipsw daemon: key "ApiVersion"'
-                ' is missing.'
-            )
+            raise IpswException('Invalid response from ipsw daemon: key "ApiVersion"' " is missing.")
         except Exception as e:
-            raise IpswException(
-                f'Error while fetching server API version: {e}'
-            )
+            raise IpswException(f"Error while fetching server API version: {e}")
 
     def _set_request_timeout(self, kwargs):
         """Prepare the kwargs for an HTTP request by inserting the timeout
         parameter, if not already present."""
-        kwargs.setdefault('timeout', self.timeout)
+        kwargs.setdefault("timeout", self.timeout)
         return kwargs
 
     @update_headers
     def _post(self, url, **kwargs):
         return self.post(url, **self._set_request_timeout(kwargs))
 
     @update_headers
@@ -197,28 +179,23 @@
     @update_headers
     def _delete(self, url, **kwargs):
         return self.delete(url, **self._set_request_timeout(kwargs))
 
     def _url(self, pathfmt, *args, **kwargs):
         for arg in args:
             if not isinstance(arg, str):
-                raise ValueError(
-                    'Expected a string but found {} ({}) '
-                    'instead'.format(arg, type(arg))
-                )
+                raise ValueError("Expected a string but found {} ({}) " "instead".format(arg, type(arg)))
 
         quote_f = partial(urllib.parse.quote, safe="/:")
         args = map(quote_f, args)
 
-        if kwargs.get('versioned_api', True):
-            return '{}/v{}{}'.format(
-                self.base_url, self._version, pathfmt.format(*args)
-            )
+        if kwargs.get("versioned_api", True):
+            return "{}/v{}{}".format(self.base_url, self._version, pathfmt.format(*args))
         else:
-            return f'{self.base_url}{pathfmt.format(*args)}'
+            return f"{self.base_url}{pathfmt.format(*args)}"
 
     def _raise_for_status(self, response):
         """Raises stored :class:`APIError`, if one occurred."""
         try:
             response.raise_for_status()
         except requests.exceptions.HTTPError as e:
             raise create_api_error_from_http_exception(e) from e
@@ -240,34 +217,30 @@
         if data is not None and isinstance(data, dict):
             for k, v in iter(data.items()):
                 if v is not None:
                     data2[k] = v
         elif data is not None:
             data2 = data
 
-        if 'headers' not in kwargs:
-            kwargs['headers'] = {}
-        kwargs['headers']['Content-Type'] = 'application/json'
+        if "headers" not in kwargs:
+            kwargs["headers"] = {}
+        kwargs["headers"]["Content-Type"] = "application/json"
         return self._post(url, data=json.dumps(data2), **kwargs)
 
     def _attach_params(self, override=None):
-        return override or {
-            'stdout': 1,
-            'stderr': 1,
-            'stream': 1
-        }
+        return override or {"stdout": 1, "stderr": 1, "stream": 1}
 
     def _create_websocket_connection(self, url):
         return websocket.create_connection(url)
 
     def _get_raw_response_socket(self, response):
         self._raise_for_status(response)
         if self.base_url == "http+ipsw://localnpipe":
             sock = response.raw._fp.fp.raw.sock
-        elif self.base_url.startswith('http+ipsw://ssh'):
+        elif self.base_url.startswith("http+ipsw://ssh"):
             sock = response.raw._fp.fp.channel
         else:
             sock = response.raw._fp.fp.raw
             if self.base_url.startswith("https://"):
                 sock = sock._sock
         try:
             # Keep a reference to the response to stop it being garbage
@@ -307,16 +280,16 @@
         response."""
         buf = self._result(response, binary=True)
         buf_length = len(buf)
         walker = 0
         while True:
             if buf_length - walker < STREAM_HEADER_SIZE_BYTES:
                 break
-            header = buf[walker:walker + STREAM_HEADER_SIZE_BYTES]
-            _, length = struct.unpack_from('>BxxxL', header)
+            header = buf[walker : walker + STREAM_HEADER_SIZE_BYTES]
+            _, length = struct.unpack_from(">BxxxL", header)
             start = walker + STREAM_HEADER_SIZE_BYTES
             end = start + length
             walker = end
             yield buf[start:end]
 
     def _multiplexed_response_stream_helper(self, response):
         """A generator of multiplexed data blocks coming from a response
@@ -327,24 +300,24 @@
         socket = self._get_raw_response_socket(response)
         self._disable_socket_timeout(socket)
 
         while True:
             header = response.raw.read(STREAM_HEADER_SIZE_BYTES)
             if not header:
                 break
-            _, length = struct.unpack('>BxxxL', header)
+            _, length = struct.unpack(">BxxxL", header)
             if not length:
                 continue
             data = response.raw.read(length)
             if not data:
                 break
             yield data
 
     def _stream_raw_result(self, response, chunk_size=1, decode=True):
-        ''' Stream result for TTY-enabled container and raw binary data'''
+        """Stream result for TTY-enabled container and raw binary data"""
         self._raise_for_status(response)
 
         # Disable timeout on the underlying socket to prevent
         # Read timed out(s) for long running processes
         socket = self._get_raw_response_socket(response)
         self._disable_socket_timeout(socket)
 
@@ -372,33 +345,33 @@
             try:
                 # Wait for all frames, concatenate them, and return the result
                 return consume_socket_output(gen, demux=demux)
             finally:
                 response.close()
 
     def _disable_socket_timeout(self, socket):
-        """ Depending on the combination of python version and whether we're
+        """Depending on the combination of python version and whether we're
         connecting over http or https, we might need to access _sock, which
         may or may not exist; or we may need to just settimeout on socket
         itself, which also may or may not have settimeout on it. To avoid
         missing the correct one, we try both.
 
         We also do not want to set the timeout if it is already disabled, as
         you run the risk of changing a socket that was non-blocking to
         blocking, for example when using gevent.
         """
-        sockets = [socket, getattr(socket, '_sock', None)]
+        sockets = [socket, getattr(socket, "_sock", None)]
 
         for s in sockets:
-            if not hasattr(s, 'settimeout'):
+            if not hasattr(s, "settimeout"):
                 continue
 
             timeout = -1
 
-            if hasattr(s, 'gettimeout'):
+            if hasattr(s, "gettimeout"):
                 timeout = s.gettimeout()
 
             # Don't change the timeout if it is already disabled.
             if timeout is None or timeout == 0.0:
                 continue
 
             s.settimeout(None)
```

### Comparing `ipsw-0.1.2/ipsw/api/daemon.py` & `ipsw-0.1.3/ipsw/api/daemon.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         Returns:
             (bool) The response from the server.
 
         Raises:
             :py:class:`ipsw.errors.APIError`
                 If the server returns an error.
         """
-        return self._result(self._get(self._url('/_ping'))) == 'OK'
+        return self._result(self._get(self._url("/_ping"))) == "OK"
 
     def version(self, api_version=True):
         """
         Returns version information from the server. Similar to the ``ipsw
         version`` command.
 
         Returns:
```

### Comparing `ipsw-0.1.2/ipsw/api/info.py` & `ipsw-0.1.3/ipsw/api/info.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.2/ipsw/client.py` & `ipsw-0.1.3/ipsw/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .api.client import APIClient
-from .constants import (DEFAULT_TIMEOUT_SECONDS, DEFAULT_MAX_POOL_SIZE)
+from .constants import DEFAULT_TIMEOUT_SECONDS, DEFAULT_MAX_POOL_SIZE
+from .models.dsc import DscCollection
 from .models.info import InfoCollection
 from .models.macho import MachoCollection
 from .utils import kwargs_from_env
 
 
 class IpswClient:
     """
@@ -23,14 +24,15 @@
         user_agent (str): Set a custom user agent for requests to the server.
         use_ssh_client (bool): If set to `True`, an ssh connection is made
             via shelling out to the ssh client. Ensure the ssh client is
             installed and configured on the host.
         max_pool_size (int): The maximum number of connections
             to save in the pool.
     """
+
     def __init__(self, *args, **kwargs):
         self.api = APIClient(*args, **kwargs)
 
     @classmethod
     def from_env(cls, **kwargs):
         """
         Return a client configured from environment variables.
@@ -55,59 +57,71 @@
                 made via shelling out to the ssh client. Ensure the ssh
                 client is installed and configured on the host.
 
         Example:
 
             >>> import ipsw
             >>> client = ipsw.from_env()
-            
+
         """
-        timeout = kwargs.pop('timeout', DEFAULT_TIMEOUT_SECONDS)
-        max_pool_size = kwargs.pop('max_pool_size', DEFAULT_MAX_POOL_SIZE)
-        version = kwargs.pop('version', None)
-        use_ssh_client = kwargs.pop('use_ssh_client', False)
+        timeout = kwargs.pop("timeout", DEFAULT_TIMEOUT_SECONDS)
+        max_pool_size = kwargs.pop("max_pool_size", DEFAULT_MAX_POOL_SIZE)
+        version = kwargs.pop("version", None)
+        use_ssh_client = kwargs.pop("use_ssh_client", False)
         return cls(
             timeout=timeout,
             max_pool_size=max_pool_size,
             version=version,
             use_ssh_client=use_ssh_client,
-            **kwargs_from_env(**kwargs)
+            **kwargs_from_env(**kwargs),
         )
 
     @property
+    def dsc(self):
+        """
+        An object for getting DSC info.
+        """
+        return DscCollection(client=self)
+
+    @property
     def info(self):
         """
         An object for getting local/remote IPSW/OTA info.
         """
         return InfoCollection(client=self)
-    
+
     @property
     def macho(self):
         """
         An object for getting MachO info.
         """
         return MachoCollection(client=self)
 
     # Top-level methods
     def ping(self, *args, **kwargs):
         return self.api.ping(*args, **kwargs)
+
     ping.__doc__ = APIClient.ping.__doc__
 
     def version(self, *args, **kwargs):
         return self.api.version(*args, **kwargs)
+
     version.__doc__ = APIClient.version.__doc__
 
     def close(self):
         return self.api.close()
+
     close.__doc__ = APIClient.close.__doc__
 
     def __getattr__(self, name):
         s = [f"'IpswClient' object has no attribute '{name}'"]
         # If a user calls a method on APIClient, they
         if hasattr(APIClient, name):
-            s.append("In ipsw SDK for Python 2.0, this method is now on the "
-                     "object APIClient. See the low-level API section of the "
-                     "documentation for more details.")
-        raise AttributeError(' '.join(s))
+            s.append(
+                "In ipsw SDK for Python 2.0, this method is now on the "
+                "object APIClient. See the low-level API section of the "
+                "documentation for more details."
+            )
+        raise AttributeError(" ".join(s))
 
 
-from_env = IpswClient.from_env
+from_env = IpswClient.from_env
```

### Comparing `ipsw-0.1.2/ipsw/constants.py` & `ipsw-0.1.3/ipsw/constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 import sys
 from .version import __version__
 
-DEFAULT_IPSW_API_VERSION = '1.0'
-MINIMUM_IPSW_API_VERSION = '1.0'
+DEFAULT_IPSW_API_VERSION = "1.0"
+MINIMUM_IPSW_API_VERSION = "1.0"
 DEFAULT_TIMEOUT_SECONDS = 60
 STREAM_HEADER_SIZE_BYTES = 8
 
 DEFAULT_HTTP_HOST = "127.0.0.1"
 DEFAULT_UNIX_SOCKET = "http+unix:///var/run/ipsw.sock"
-DEFAULT_NPIPE = 'npipe:////./pipe/ipsw'
+DEFAULT_NPIPE = "npipe:////./pipe/ipsw"
 
-BYTE_UNITS = {
-    'b': 1,
-    'k': 1024,
-    'm': 1024 * 1024,
-    'g': 1024 * 1024 * 1024
-}
+BYTE_UNITS = {"b": 1, "k": 1024, "m": 1024 * 1024, "g": 1024 * 1024 * 1024}
 
-IS_WINDOWS_PLATFORM = (sys.platform == 'win32')
-WINDOWS_LONGPATH_PREFIX = '\\\\?\\'
+IS_WINDOWS_PLATFORM = sys.platform == "win32"
+WINDOWS_LONGPATH_PREFIX = "\\\\?\\"
 
 DEFAULT_USER_AGENT = f"ipsw-sdk-python/{__version__}"
 DEFAULT_NUM_POOLS = 25
 
 # The OpenSSH server default value for MaxSessions is 10 which means we can
 # use up to 9, leaving the final session for the underlying SSH connection.
 DEFAULT_NUM_POOLS_SSH = 9
```

### Comparing `ipsw-0.1.2/ipsw/errors.py` & `ipsw-0.1.3/ipsw/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
             return False
         return 500 <= self.status_code < 600
 
 
 class NotFound(APIError):
     pass
 
+
 class InvalidVersion(IpswException):
     pass
 
 
 class StreamParseError(RuntimeError):
     def __init__(self, reason):
         self.msg = reason
```

### Comparing `ipsw-0.1.2/ipsw/models/configs.py` & `ipsw-0.1.3/ipsw/models/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from ..api import APIClient
 from .resource import Model, Collection
 
 
 class Config(Model):
     """A config."""
-    id_attribute = 'ID'
+
+    id_attribute = "ID"
 
     def __repr__(self):
         return f"<{self.__class__.__name__}: '{self.name}'>"
 
     @property
     def name(self):
-        return self.attrs['Spec']['Name']
+        return self.attrs["Spec"]["Name"]
 
     def remove(self):
         """
         Remove this config.
 
         Raises:
             :py:class:`ipsw.errors.APIError`
@@ -25,14 +26,15 @@
 
     """Configs on the ipsw server."""
     model = Config
 
     def create(self, **kwargs):
         obj = self.client.api.create_config(**kwargs)
         return self.prepare_model(obj)
+
     create.__doc__ = APIClient.create_config.__doc__
 
     def get(self, config_id):
         """
         Get a config.
 
         Args:
@@ -60,8 +62,8 @@
             (list of :py:class:`Config`): The configs.
 
         Raises:
             :py:class:`ipsw.errors.APIError`
                 If the server returns an error.
         """
         resp = self.client.api.configs(**kwargs)
-        return [self.prepare_model(obj) for obj in resp]
+        return [self.prepare_model(obj) for obj in resp]
```

### Comparing `ipsw-0.1.2/ipsw/models/info.py` & `ipsw-0.1.3/ipsw/models/info.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,25 +25,25 @@
 
     @property
     def build(self):
         """
         The iOS version.
         """
         return self.attrs["info"]["Plists"]["restore"].get("ProductBuildVersion", None)
-    
+
     @property
     def devices(self):
         """
         The iOS devices.
         """
         devices = set()
-        for dt in self.attrs['info']['DeviceTrees'].values():
-            for child in dt['device-tree']['children']:
-                if 'product' in child:
-                    devices.add(child['product']['product-name'])
+        for dt in self.attrs["info"]["DeviceTrees"].values():
+            for child in dt["device-tree"]["children"]:
+                if "product" in child:
+                    devices.add(child["product"]["product-name"])
         devlist = list(devices)
         devlist.sort()
         return devlist
 
 
 class InfoCollection(Collection):
     model = Info
```

### Comparing `ipsw-0.1.2/ipsw/models/macho.py` & `ipsw-0.1.3/ipsw/models/macho.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,32 +18,39 @@
         )
 
     @property
     def magic(self):
         """
         The header magic.
         """
-        return self.attrs["info"]['header'].get("magic", None)
+        return self.attrs["info"]["header"].get("magic", None)
 
     @property
     def cpu(self):
         """
         The header CPU.
         """
-        return self.attrs["info"]['header'].get("cpu", None)
-    
+        return self.attrs["info"]["header"].get("cpu", None)
+
     @property
     def sub_cpu(self):
         """
         The header sub CPU.
         """
-        return self.attrs["info"]['header'].get("subcpu", None)
+        return self.attrs["info"]["header"].get("subcpu", None)
+
+    @property
+    def header(self):
+        """
+        The header.
+        """
+        return self.attrs["info"].get("header", None)
 
 
 class MachoCollection(Collection):
     model = Macho
 
     def get(self, path=None, arch=None):
         """
         Get MachO info.
         """
-        return self.prepare_model(self.client.api.macho_info(path, arch))
+        return self.prepare_model(self.client.api.macho_info(path, arch))
```

### Comparing `ipsw-0.1.2/ipsw/models/resource.py` & `ipsw-0.1.3/ipsw/models/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 class Model:
     """
     A base class for representing a single object on the server.
     """
-    id_attribute = 'Id'
+
+    id_attribute = "Id"
 
     def __init__(self, attrs=None, client=None, collection=None):
         #: A client pointing at the server that this object is on.
         self.client = client
 
         #: The collection that this model is part of.
         self.collection = collection
@@ -61,16 +62,16 @@
         #: The client pointing at the server that this collection of objects
         #: is on.
         self.client = client
 
     def __call__(self, *args, **kwargs):
         raise TypeError(
             "'{}' object is not callable. You might be trying to use the old "
-            "(pre-2.0) API - use ipsw.APIClient if so."
-            .format(self.__class__.__name__))
+            "(pre-2.0) API - use ipsw.APIClient if so.".format(self.__class__.__name__)
+        )
 
     def list(self):
         raise NotImplementedError
 
     def get(self, key):
         raise NotImplementedError
 
@@ -84,9 +85,8 @@
         if isinstance(attrs, Model):
             attrs.client = self.client
             attrs.collection = self
             return attrs
         elif isinstance(attrs, dict):
             return self.model(attrs=attrs, client=self.client, collection=self)
         else:
-            raise Exception("Can't create %s from %s" %
-                            (self.model.__name__, attrs))
+            raise Exception("Can't create %s from %s" % (self.model.__name__, attrs))
```

### Comparing `ipsw-0.1.2/ipsw/transport/npipeconn.py` & `ipsw-0.1.3/ipsw/transport/npipeconn.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,39 +13,33 @@
     import urllib3
 
 RecentlyUsedContainer = urllib3._collections.RecentlyUsedContainer
 
 
 class NpipeHTTPConnection(httplib.HTTPConnection):
     def __init__(self, npipe_path, timeout=60):
-        super().__init__(
-            'localhost', timeout=timeout
-        )
+        super().__init__("localhost", timeout=timeout)
         self.npipe_path = npipe_path
         self.timeout = timeout
 
     def connect(self):
         sock = NpipeSocket()
         sock.settimeout(self.timeout)
         sock.connect(self.npipe_path)
         self.sock = sock
 
 
 class NpipeHTTPConnectionPool(urllib3.connectionpool.HTTPConnectionPool):
     def __init__(self, npipe_path, timeout=60, maxsize=10):
-        super().__init__(
-            'localhost', timeout=timeout, maxsize=maxsize
-        )
+        super().__init__("localhost", timeout=timeout, maxsize=maxsize)
         self.npipe_path = npipe_path
         self.timeout = timeout
 
     def _new_conn(self):
-        return NpipeHTTPConnection(
-            self.npipe_path, self.timeout
-        )
+        return NpipeHTTPConnection(self.npipe_path, self.timeout)
 
     # When re-using connections, urllib3 tries to call select() on our
     # NpipeSocket instance, causing a crash. To circumvent this, we override
     # _get_conn, where that check happens.
     def _get_conn(self, timeout):
         conn = None
         try:
@@ -53,51 +47,44 @@
 
         except AttributeError:  # self.pool is None
             raise urllib3.exceptions.ClosedPoolError(self, "Pool is closed.")
 
         except queue.Empty:
             if self.block:
                 raise urllib3.exceptions.EmptyPoolError(
-                    self,
-                    "Pool reached maximum size and no more "
-                    "connections are allowed."
+                    self, "Pool reached maximum size and no more " "connections are allowed."
                 )
             # Oh well, we'll create a new connection then
 
         return conn or self._new_conn()
 
 
 class NpipeHTTPAdapter(BaseHTTPAdapter):
+    __attrs__ = requests.adapters.HTTPAdapter.__attrs__ + ["npipe_path", "pools", "timeout", "max_pool_size"]
 
-    __attrs__ = requests.adapters.HTTPAdapter.__attrs__ + ['npipe_path',
-                                                           'pools',
-                                                           'timeout',
-                                                           'max_pool_size']
-
-    def __init__(self, base_url, timeout=60,
-                 pool_connections=constants.DEFAULT_NUM_POOLS,
-                 max_pool_size=constants.DEFAULT_MAX_POOL_SIZE):
-        self.npipe_path = base_url.replace('npipe://', '')
+    def __init__(
+        self,
+        base_url,
+        timeout=60,
+        pool_connections=constants.DEFAULT_NUM_POOLS,
+        max_pool_size=constants.DEFAULT_MAX_POOL_SIZE,
+    ):
+        self.npipe_path = base_url.replace("npipe://", "")
         self.timeout = timeout
         self.max_pool_size = max_pool_size
-        self.pools = RecentlyUsedContainer(
-            pool_connections, dispose_func=lambda p: p.close()
-        )
+        self.pools = RecentlyUsedContainer(pool_connections, dispose_func=lambda p: p.close())
         super().__init__()
 
     def get_connection(self, url, proxies=None):
         with self.pools.lock:
             pool = self.pools.get(url)
             if pool:
                 return pool
 
-            pool = NpipeHTTPConnectionPool(
-                self.npipe_path, self.timeout,
-                maxsize=self.max_pool_size
-            )
+            pool = NpipeHTTPConnectionPool(self.npipe_path, self.timeout, maxsize=self.max_pool_size)
             self.pools[url] = pool
 
         return pool
 
     def request_url(self, request, proxies):
         # The select_proxy utility in requests errors out when the provided URL
         # doesn't have a hostname, like is the case when using a UNIX socket.
```

### Comparing `ipsw-0.1.2/ipsw/transport/npipesocket.py` & `ipsw-0.1.3/ipsw/transport/npipesocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import functools
 import time
 import io
 
 import win32file
 import win32pipe
 
-cERROR_PIPE_BUSY = 0xe7
+cERROR_PIPE_BUSY = 0xE7
 cSECURITY_SQOS_PRESENT = 0x100000
 cSECURITY_ANONYMOUS = 0
 
 MAXIMUM_RETRY_COUNT = 10
 
 
 def check_closed(f):
     @functools.wraps(f)
     def wrapped(self, *args, **kwargs):
         if self._closed:
-            raise RuntimeError(
-                'Can not reuse socket after connection was closed.'
-            )
+            raise RuntimeError("Can not reuse socket after connection was closed.")
         return f(self, *args, **kwargs)
+
     return wrapped
 
 
 class NpipeSocket:
-    """ Partial implementation of the socket API over windows named pipes.
-        This implementation is only designed to be used as a client socket,
-        and server-specific methods (bind, listen, accept...) are not
-        implemented.
+    """Partial implementation of the socket API over windows named pipes.
+    This implementation is only designed to be used as a client socket,
+    and server-specific methods (bind, listen, accept...) are not
+    implemented.
     """
 
     def __init__(self, handle=None):
         self._timeout = win32pipe.NMPWAIT_USE_DEFAULT_WAIT
         self._handle = handle
         self._closed = False
 
@@ -51,25 +50,25 @@
             handle = win32file.CreateFile(
                 address,
                 win32file.GENERIC_READ | win32file.GENERIC_WRITE,
                 0,
                 None,
                 win32file.OPEN_EXISTING,
                 cSECURITY_ANONYMOUS | cSECURITY_SQOS_PRESENT,
-                0
+                0,
             )
         except win32pipe.error as e:
             # See Remarks:
             # https://msdn.microsoft.com/en-us/library/aa365800.aspx
             if e.winerror == cERROR_PIPE_BUSY:
                 # Another program or thread has grabbed our pipe instance
                 # before we got to it. Wait for availability and attempt to
                 # connect again.
                 retry_count = retry_count + 1
-                if (retry_count < MAXIMUM_RETRY_COUNT):
+                if retry_count < MAXIMUM_RETRY_COUNT:
                     time.sleep(1)
                     return self.connect(address, retry_count)
             raise e
 
         self.flags = win32pipe.GetNamedPipeInfo(handle)[0]
 
         self._handle = handle
@@ -100,15 +99,15 @@
     def ioctl(self, control, option):
         raise NotImplementedError()
 
     def listen(self, backlog):
         raise NotImplementedError()
 
     def makefile(self, mode=None, bufsize=None):
-        if mode.strip('b') != 'r':
+        if mode.strip("b") != "r":
             raise NotImplementedError()
         rawio = NpipeFileIOBase(self)
         if bufsize is None or bufsize <= 0:
             bufsize = io.DEFAULT_BUFFER_SIZE
         return io.BufferedReader(rawio, buffer_size=bufsize)
 
     @check_closed
@@ -127,18 +126,15 @@
 
     @check_closed
     def recv_into(self, buf, nbytes=0):
         readbuf = buf
         if not isinstance(buf, memoryview):
             readbuf = memoryview(buf)
 
-        err, data = win32file.ReadFile(
-            self._handle,
-            readbuf[:nbytes] if nbytes else readbuf
-        )
+        err, data = win32file.ReadFile(self._handle, readbuf[:nbytes] if nbytes else readbuf)
         return len(data)
 
     def _recv_into_py2(self, buf, nbytes):
         err, data = win32file.ReadFile(self._handle, nbytes or len(buf))
         n = len(data)
         buf[:n] = data
         return n
@@ -163,15 +159,15 @@
         return self.settimeout(0)
 
     def settimeout(self, value):
         if value is None:
             # Blocking mode
             self._timeout = win32pipe.NMPWAIT_WAIT_FOREVER
         elif not isinstance(value, (float, int)) or value < 0:
-            raise ValueError('Timeout value out of range')
+            raise ValueError("Timeout value out of range")
         elif value == 0:
             # Non-blocking mode
             self._timeout = win32pipe.NMPWAIT_NO_WAIT
         else:
             # Timeout mode - Value converted to milliseconds
             self._timeout = value * 1000
```

### Comparing `ipsw-0.1.2/ipsw/transport/sshconn.py` & `ipsw-0.1.3/ipsw/transport/sshconn.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,119 +19,111 @@
     import urllib3
 
 RecentlyUsedContainer = urllib3._collections.RecentlyUsedContainer
 
 
 class SSHSocket(socket.socket):
     def __init__(self, host):
-        super().__init__(
-            socket.AF_INET, socket.SOCK_STREAM)
+        super().__init__(socket.AF_INET, socket.SOCK_STREAM)
         self.host = host
         self.port = None
         self.user = None
-        if ':' in self.host:
-            self.host, self.port = self.host.split(':')
-        if '@' in self.host:
-            self.user, self.host = self.host.split('@')
+        if ":" in self.host:
+            self.host, self.port = self.host.split(":")
+        if "@" in self.host:
+            self.user, self.host = self.host.split("@")
 
         self.proc = None
 
     def connect(self, **kwargs):
-        args = ['ssh']
+        args = ["ssh"]
         if self.user:
-            args = args + ['-l', self.user]
+            args = args + ["-l", self.user]
 
         if self.port:
-            args = args + ['-p', self.port]
+            args = args + ["-p", self.port]
 
-        args = args + ['--', self.host, 'ipsw system dial-stdio']
+        args = args + ["--", self.host, "ipsw system dial-stdio"]
 
         preexec_func = None
         if not constants.IS_WINDOWS_PLATFORM:
+
             def f():
                 signal.signal(signal.SIGINT, signal.SIG_IGN)
+
             preexec_func = f
 
         env = dict(os.environ)
 
         # drop LD_LIBRARY_PATH and SSL_CERT_FILE
-        env.pop('LD_LIBRARY_PATH', None)
-        env.pop('SSL_CERT_FILE', None)
+        env.pop("LD_LIBRARY_PATH", None)
+        env.pop("SSL_CERT_FILE", None)
 
         self.proc = subprocess.Popen(
-            args,
-            env=env,
-            stdout=subprocess.PIPE,
-            stdin=subprocess.PIPE,
-            preexec_fn=preexec_func)
+            args, env=env, stdout=subprocess.PIPE, stdin=subprocess.PIPE, preexec_fn=preexec_func
+        )
 
     def _write(self, data):
         if not self.proc or self.proc.stdin.closed:
-            raise Exception('SSH subprocess not initiated.'
-                            'connect() must be called first.')
+            raise Exception("SSH subprocess not initiated." "connect() must be called first.")
         written = self.proc.stdin.write(data)
         self.proc.stdin.flush()
         return written
 
     def sendall(self, data):
         self._write(data)
 
     def send(self, data):
         return self._write(data)
 
     def recv(self, n):
         if not self.proc:
-            raise Exception('SSH subprocess not initiated.'
-                            'connect() must be called first.')
+            raise Exception("SSH subprocess not initiated." "connect() must be called first.")
         return self.proc.stdout.read(n)
 
     def makefile(self, mode):
         if not self.proc:
             self.connect()
         self.proc.stdout.channel = self
 
         return self.proc.stdout
 
     def close(self):
         if not self.proc or self.proc.stdin.closed:
             return
-        self.proc.stdin.write(b'\n\n')
+        self.proc.stdin.write(b"\n\n")
         self.proc.stdin.flush()
         self.proc.terminate()
 
 
 class SSHConnection(httplib.HTTPConnection):
     def __init__(self, ssh_transport=None, timeout=60, host=None):
-        super().__init__(
-            'localhost', timeout=timeout
-        )
+        super().__init__("localhost", timeout=timeout)
         self.ssh_transport = ssh_transport
         self.timeout = timeout
         self.ssh_host = host
 
     def connect(self):
         if self.ssh_transport:
             sock = self.ssh_transport.open_session()
             sock.settimeout(self.timeout)
-            sock.exec_command('ipsw system dial-stdio')
+            sock.exec_command("ipsw system dial-stdio")
         else:
             sock = SSHSocket(self.ssh_host)
             sock.settimeout(self.timeout)
             sock.connect()
 
         self.sock = sock
 
 
 class SSHConnectionPool(urllib3.connectionpool.HTTPConnectionPool):
-    scheme = 'ssh'
+    scheme = "ssh"
 
     def __init__(self, ssh_client=None, timeout=60, maxsize=10, host=None):
-        super().__init__(
-            'localhost', timeout=timeout, maxsize=maxsize
-        )
+        super().__init__("localhost", timeout=timeout, maxsize=maxsize)
         self.ssh_transport = None
         self.timeout = timeout
         if ssh_client:
             self.ssh_transport = ssh_client.get_transport()
         self.ssh_host = host
 
     def _new_conn(self):
@@ -147,106 +139,97 @@
 
         except AttributeError:  # self.pool is None
             raise urllib3.exceptions.ClosedPoolError(self, "Pool is closed.")
 
         except queue.Empty:
             if self.block:
                 raise urllib3.exceptions.EmptyPoolError(
-                    self,
-                    "Pool reached maximum size and no more "
-                    "connections are allowed."
+                    self, "Pool reached maximum size and no more " "connections are allowed."
                 )
             # Oh well, we'll create a new connection then
 
         return conn or self._new_conn()
 
 
 class SSHHTTPAdapter(BaseHTTPAdapter):
-
     __attrs__ = requests.adapters.HTTPAdapter.__attrs__ + [
-        'pools', 'timeout', 'ssh_client', 'ssh_params', 'max_pool_size'
+        "pools",
+        "timeout",
+        "ssh_client",
+        "ssh_params",
+        "max_pool_size",
     ]
 
-    def __init__(self, base_url, timeout=60,
-                 pool_connections=constants.DEFAULT_NUM_POOLS,
-                 max_pool_size=constants.DEFAULT_MAX_POOL_SIZE,
-                 shell_out=False):
+    def __init__(
+        self,
+        base_url,
+        timeout=60,
+        pool_connections=constants.DEFAULT_NUM_POOLS,
+        max_pool_size=constants.DEFAULT_MAX_POOL_SIZE,
+        shell_out=False,
+    ):
         self.ssh_client = None
         if not shell_out:
             self._create_paramiko_client(base_url)
             self._connect()
 
         self.ssh_host = base_url
-        if base_url.startswith('ssh://'):
-            self.ssh_host = base_url[len('ssh://'):]
+        if base_url.startswith("ssh://"):
+            self.ssh_host = base_url[len("ssh://") :]
 
         self.timeout = timeout
         self.max_pool_size = max_pool_size
-        self.pools = RecentlyUsedContainer(
-            pool_connections, dispose_func=lambda p: p.close()
-        )
+        self.pools = RecentlyUsedContainer(pool_connections, dispose_func=lambda p: p.close())
         super().__init__()
 
     def _create_paramiko_client(self, base_url):
         logging.getLogger("paramiko").setLevel(logging.WARNING)
         self.ssh_client = paramiko.SSHClient()
         base_url = urllib.parse.urlparse(base_url)
-        self.ssh_params = {
-            "hostname": base_url.hostname,
-            "port": base_url.port,
-            "username": base_url.username
-            }
+        self.ssh_params = {"hostname": base_url.hostname, "port": base_url.port, "username": base_url.username}
         ssh_config_file = os.path.expanduser("~/.ssh/config")
         if os.path.exists(ssh_config_file):
             conf = paramiko.SSHConfig()
             with open(ssh_config_file) as f:
                 conf.parse(f)
             host_config = conf.lookup(base_url.hostname)
-            if 'proxycommand' in host_config:
-                self.ssh_params["sock"] = paramiko.ProxyCommand(
-                    host_config['proxycommand']
-                )
-            if 'hostname' in host_config:
-                self.ssh_params['hostname'] = host_config['hostname']
-            if base_url.port is None and 'port' in host_config:
-                self.ssh_params['port'] = host_config['port']
-            if base_url.username is None and 'user' in host_config:
-                self.ssh_params['username'] = host_config['user']
-            if 'identityfile' in host_config:
-                self.ssh_params['key_filename'] = host_config['identityfile']
+            if "proxycommand" in host_config:
+                self.ssh_params["sock"] = paramiko.ProxyCommand(host_config["proxycommand"])
+            if "hostname" in host_config:
+                self.ssh_params["hostname"] = host_config["hostname"]
+            if base_url.port is None and "port" in host_config:
+                self.ssh_params["port"] = host_config["port"]
+            if base_url.username is None and "user" in host_config:
+                self.ssh_params["username"] = host_config["user"]
+            if "identityfile" in host_config:
+                self.ssh_params["key_filename"] = host_config["identityfile"]
 
         self.ssh_client.load_system_host_keys()
         self.ssh_client.set_missing_host_key_policy(paramiko.RejectPolicy())
 
     def _connect(self):
         if self.ssh_client:
             self.ssh_client.connect(**self.ssh_params)
 
     def get_connection(self, url, proxies=None):
         if not self.ssh_client:
             return SSHConnectionPool(
-                ssh_client=self.ssh_client,
-                timeout=self.timeout,
-                maxsize=self.max_pool_size,
-                host=self.ssh_host
+                ssh_client=self.ssh_client, timeout=self.timeout, maxsize=self.max_pool_size, host=self.ssh_host
             )
         with self.pools.lock:
             pool = self.pools.get(url)
             if pool:
                 return pool
 
             # Connection is closed try a reconnect
             if self.ssh_client and not self.ssh_client.get_transport():
                 self._connect()
 
             pool = SSHConnectionPool(
-                ssh_client=self.ssh_client,
-                timeout=self.timeout,
-                maxsize=self.max_pool_size,
-                host=self.ssh_host
+                ssh_client=self.ssh_client, timeout=self.timeout, maxsize=self.max_pool_size, host=self.ssh_host
             )
             self.pools[url] = pool
 
         return pool
 
     def close(self):
         super().close()
```

### Comparing `ipsw-0.1.2/ipsw/transport/unixconn.py` & `ipsw-0.1.3/ipsw/transport/unixconn.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,19 +11,16 @@
     import urllib3
 
 
 RecentlyUsedContainer = urllib3._collections.RecentlyUsedContainer
 
 
 class UnixHTTPConnection(httplib.HTTPConnection):
-
     def __init__(self, base_url, unix_socket, timeout=60):
-        super().__init__(
-            'localhost', timeout=timeout
-        )
+        super().__init__("localhost", timeout=timeout)
         self.base_url = base_url
         self.unix_socket = unix_socket
         self.timeout = timeout
 
     def connect(self):
         sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
         sock.settimeout(self.timeout)
@@ -35,58 +32,49 @@
 
     def response_class(self, sock, *args, **kwargs):
         return httplib.HTTPResponse(sock, *args, **kwargs)
 
 
 class UnixHTTPConnectionPool(urllib3.connectionpool.HTTPConnectionPool):
     def __init__(self, base_url, socket_path, timeout=60, maxsize=10):
-        super().__init__(
-            'localhost', timeout=timeout, maxsize=maxsize
-        )
+        super().__init__("localhost", timeout=timeout, maxsize=maxsize)
         self.base_url = base_url
         self.socket_path = socket_path
         self.timeout = timeout
 
     def _new_conn(self):
-        return UnixHTTPConnection(
-            self.base_url, self.socket_path, self.timeout
-        )
+        return UnixHTTPConnection(self.base_url, self.socket_path, self.timeout)
 
 
 class UnixHTTPAdapter(BaseHTTPAdapter):
+    __attrs__ = requests.adapters.HTTPAdapter.__attrs__ + ["pools", "socket_path", "timeout", "max_pool_size"]
 
-    __attrs__ = requests.adapters.HTTPAdapter.__attrs__ + ['pools',
-                                                           'socket_path',
-                                                           'timeout',
-                                                           'max_pool_size']
-
-    def __init__(self, socket_url, timeout=60,
-                 pool_connections=constants.DEFAULT_NUM_POOLS,
-                 max_pool_size=constants.DEFAULT_MAX_POOL_SIZE):
-        socket_path = socket_url.replace('http+unix://', '')
-        if not socket_path.startswith('/'):
-            socket_path = '/' + socket_path
+    def __init__(
+        self,
+        socket_url,
+        timeout=60,
+        pool_connections=constants.DEFAULT_NUM_POOLS,
+        max_pool_size=constants.DEFAULT_MAX_POOL_SIZE,
+    ):
+        socket_path = socket_url.replace("http+unix://", "")
+        if not socket_path.startswith("/"):
+            socket_path = "/" + socket_path
         self.socket_path = socket_path
         self.timeout = timeout
         self.max_pool_size = max_pool_size
-        self.pools = RecentlyUsedContainer(
-            pool_connections, dispose_func=lambda p: p.close()
-        )
+        self.pools = RecentlyUsedContainer(pool_connections, dispose_func=lambda p: p.close())
         super().__init__()
 
     def get_connection(self, url, proxies=None):
         with self.pools.lock:
             pool = self.pools.get(url)
             if pool:
                 return pool
 
-            pool = UnixHTTPConnectionPool(
-                url, self.socket_path, self.timeout,
-                maxsize=self.max_pool_size
-            )
+            pool = UnixHTTPConnectionPool(url, self.socket_path, self.timeout, maxsize=self.max_pool_size)
             self.pools[url] = pool
 
         return pool
 
     def request_url(self, request, proxies):
         # The select_proxy utility in requests errors out when the provided URL
         # doesn't have a hostname, like is the case when using a UNIX socket.
```

### Comparing `ipsw-0.1.2/ipsw/types/daemon.py` & `ipsw-0.1.3/ipsw/types/daemon.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,31 +44,28 @@
 
         if not self._response.raw.closed:
             # find the underlying socket object
             # based on api.client._get_raw_response_socket
 
             sock_fp = self._response.raw._fp.fp
 
-            if hasattr(sock_fp, 'raw'):
+            if hasattr(sock_fp, "raw"):
                 sock_raw = sock_fp.raw
 
-                if hasattr(sock_raw, 'sock'):
+                if hasattr(sock_raw, "sock"):
                     sock = sock_raw.sock
 
-                elif hasattr(sock_raw, '_sock'):
+                elif hasattr(sock_raw, "_sock"):
                     sock = sock_raw._sock
 
-            elif hasattr(sock_fp, 'channel'):
+            elif hasattr(sock_fp, "channel"):
                 # We're working with a paramiko (SSH) channel, which doesn't
                 # support cancelable streams with the current implementation
-                raise IpswException(
-                    'Cancellable streams not supported for the SSH protocol'
-                )
+                raise IpswException("Cancellable streams not supported for the SSH protocol")
             else:
                 sock = sock_fp._sock
 
-            if hasattr(urllib3.contrib, 'pyopenssl') and isinstance(
-                    sock, urllib3.contrib.pyopenssl.WrappedSocket):
+            if hasattr(urllib3.contrib, "pyopenssl") and isinstance(sock, urllib3.contrib.pyopenssl.WrappedSocket):
                 sock = sock.socket
 
             sock.shutdown(socket.SHUT_RDWR)
-            sock.close()
+            sock.close()
```

### Comparing `ipsw-0.1.2/ipsw/utils/config.py` & `ipsw-0.1.3/ipsw/utils/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,58 @@
 import yaml
 import logging
 import os
 
 from ..constants import IS_WINDOWS_PLATFORM
 
-IPSW_CONFIG_FILENAME = os.path.join('.config', 'ipsw', 'config.yml')
+IPSW_CONFIG_FILENAME = os.path.join(".config", "ipsw", "config.yml")
 
 log = logging.getLogger(__name__)
 
 
 def find_config_file(config_path=None):
-    paths = list(filter(None, [
-        config_path,  # 1
-        config_path_from_environment(),  # 2
-        os.path.join(home_dir(), IPSW_CONFIG_FILENAME),  # 3
-    ]))
+    paths = list(
+        filter(
+            None,
+            [
+                config_path,  # 1
+                config_path_from_environment(),  # 2
+                os.path.join(home_dir(), IPSW_CONFIG_FILENAME),  # 3
+            ],
+        )
+    )
 
     log.debug(f"Trying paths: {repr(paths)}")
 
     for path in paths:
         if os.path.exists(path):
             log.debug(f"Found file at path: {path}")
             return path
 
     log.debug("No config file found")
 
     return None
 
 
 def config_path_from_environment():
-    config_dir = os.environ.get('IPSW_CONFIG')
+    config_dir = os.environ.get("IPSW_CONFIG")
     if not config_dir:
         return None
     return os.path.join(config_dir, os.path.basename(IPSW_CONFIG_FILENAME))
 
 
 def home_dir():
     """
     Get the user's home directory, using the same logic as the ipsw
     client - use %USERPROFILE% on Windows, $HOME/getuid on POSIX.
     """
     if IS_WINDOWS_PLATFORM:
-        return os.environ.get('USERPROFILE', '')
+        return os.environ.get("USERPROFILE", "")
     else:
-        return os.path.expanduser('~')
+        return os.path.expanduser("~")
 
 
 def load_general_config(config_path=None):
     config_file = find_config_file(config_path)
 
     if not config_file:
         return {}
@@ -55,8 +60,8 @@
     try:
         with open(config_file) as f:
             return yaml.safe_load(f)
     except (OSError, ValueError) as e:
         log.debug(e)
 
     log.debug("All parsing attempts failed - returning empty config")
-    return {}
+    return {}
```

### Comparing `ipsw-0.1.2/ipsw/utils/decorators.py` & `ipsw-0.1.3/ipsw/utils/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,41 +7,40 @@
 def check_resource(resource_name):
     def decorator(f):
         @functools.wraps(f)
         def wrapped(self, resource_id=None, *args, **kwargs):
             if resource_id is None and kwargs.get(resource_name):
                 resource_id = kwargs.pop(resource_name)
             if isinstance(resource_id, dict):
-                resource_id = resource_id.get('Id', resource_id.get('ID'))
+                resource_id = resource_id.get("Id", resource_id.get("ID"))
             if not resource_id:
-                raise errors.NullResource(
-                    'Resource ID was not provided'
-                )
+                raise errors.NullResource("Resource ID was not provided")
             return f(self, resource_id, *args, **kwargs)
+
         return wrapped
+
     return decorator
 
 
 def minimum_version(version):
     def decorator(f):
         @functools.wraps(f)
         def wrapper(self, *args, **kwargs):
             if utils.version_lt(self._version, version):
-                raise errors.InvalidVersion(
-                    '{} is not available for version < {}'.format(
-                        f.__name__, version
-                    )
-                )
+                raise errors.InvalidVersion("{} is not available for version < {}".format(f.__name__, version))
             return f(self, *args, **kwargs)
+
         return wrapper
+
     return decorator
 
 
 def update_headers(f):
     def inner(self, *args, **kwargs):
-        if 'HttpHeaders' in self._general_configs:
-            if not kwargs.get('headers'):
-                kwargs['headers'] = self._general_configs['HttpHeaders']
+        if "HttpHeaders" in self._general_configs:
+            if not kwargs.get("headers"):
+                kwargs["headers"] = self._general_configs["HttpHeaders"]
             else:
-                kwargs['headers'].update(self._general_configs['HttpHeaders'])
+                kwargs["headers"].update(self._general_configs["HttpHeaders"])
         return f(self, *args, **kwargs)
+
     return inner
```

### Comparing `ipsw-0.1.2/ipsw/utils/json_stream.py` & `ipsw-0.1.3/ipsw/utils/json_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,55 +12,55 @@
     Given a stream of bytes or text, if any of the items in the stream
     are bytes convert them to text.
     This function can be removed once we return text streams
     instead of byte streams.
     """
     for data in stream:
         if not isinstance(data, str):
-            data = data.decode('utf-8', 'replace')
+            data = data.decode("utf-8", "replace")
         yield data
 
 
 def json_splitter(buffer):
     """Attempt to parse a json object from a buffer. If there is at least one
     object, return it and the rest of the buffer, otherwise return None.
     """
     buffer = buffer.strip()
     try:
         obj, index = json_decoder.raw_decode(buffer)
-        rest = buffer[json.decoder.WHITESPACE.match(buffer, index).end():]
+        rest = buffer[json.decoder.WHITESPACE.match(buffer, index).end() :]
         return obj, rest
     except ValueError:
         return None
 
 
 def json_stream(stream):
     """Given a stream of text, return a stream of json objects.
     This handles streams which are inconsistently buffered (some entries may
     be newline delimited, and others are not).
     """
     return split_buffer(stream, json_splitter, json_decoder.decode)
 
 
-def line_splitter(buffer, separator='\n'):
+def line_splitter(buffer, separator="\n"):
     index = buffer.find(str(separator))
     if index == -1:
         return None
-    return buffer[:index + 1], buffer[index + 1:]
+    return buffer[: index + 1], buffer[index + 1 :]
 
 
 def split_buffer(stream, splitter=None, decoder=lambda a: a):
     """Given a generator which yields strings and a splitter function,
     joins all input, splits on the separator and yields each chunk.
     Unlike string.split(), each chunk includes the trailing
     separator, except for the last one if none was found on the end
     of the input.
     """
     splitter = splitter or line_splitter
-    buffered = ''
+    buffered = ""
 
     for data in stream_as_text(stream):
         buffered += data
         while True:
             buffer_split = splitter(buffered)
             if buffer_split is None:
                 break
@@ -68,8 +68,8 @@
             item, buffered = buffer_split
             yield item
 
     if buffered:
         try:
             yield decoder(buffered)
         except Exception as e:
-            raise StreamParseError(e)
+            raise StreamParseError(e)
```

### Comparing `ipsw-0.1.2/ipsw/utils/proxy.py` & `ipsw-0.1.3/ipsw/utils/proxy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 from .utils import format_environment
 
 
 class ProxyConfig(dict):
-    '''
+    """
     Hold the client's proxy configuration
-    '''
+    """
+
     @property
     def http(self):
-        return self.get('http')
+        return self.get("http")
 
     @property
     def https(self):
-        return self.get('https')
+        return self.get("https")
 
     @property
     def ftp(self):
-        return self.get('ftp')
+        return self.get("ftp")
 
     @property
     def no_proxy(self):
-        return self.get('no_proxy')
+        return self.get("no_proxy")
 
     @staticmethod
     def from_dict(config):
-        '''
+        """
         Instantiate a new ProxyConfig from a dictionary that represents a
         client configuration, as described in `the documentation`_.
-        '''
+        """
         return ProxyConfig(
-            http=config.get('httpProxy'),
-            https=config.get('httpsProxy'),
-            ftp=config.get('ftpProxy'),
-            no_proxy=config.get('noProxy'),
+            http=config.get("httpProxy"),
+            https=config.get("httpsProxy"),
+            ftp=config.get("ftpProxy"),
+            no_proxy=config.get("noProxy"),
         )
 
     def get_environment(self):
-        '''
+        """
         Return a dictionary representing the environment variables used to
         set the proxy settings.
-        '''
+        """
         env = {}
         if self.http:
-            env['http_proxy'] = env['HTTP_PROXY'] = self.http
+            env["http_proxy"] = env["HTTP_PROXY"] = self.http
         if self.https:
-            env['https_proxy'] = env['HTTPS_PROXY'] = self.https
+            env["https_proxy"] = env["HTTPS_PROXY"] = self.https
         if self.ftp:
-            env['ftp_proxy'] = env['FTP_PROXY'] = self.ftp
+            env["ftp_proxy"] = env["FTP_PROXY"] = self.ftp
         if self.no_proxy:
-            env['no_proxy'] = env['NO_PROXY'] = self.no_proxy
+            env["no_proxy"] = env["NO_PROXY"] = self.no_proxy
         return env
 
     def inject_proxy_environment(self, environment):
-        '''
+        """
         Given a list of strings representing environment variables, prepend the
         environment variables corresponding to the proxy settings.
-        '''
+        """
         if not self:
             return environment
 
         proxy_env = format_environment(self.get_environment())
         if not environment:
             return proxy_env
         # It is important to prepend our variables, because we want the
         # variables defined in "environment" to take precedence.
         return proxy_env + environment
 
     def __str__(self):
-        return 'ProxyConfig(http={}, https={}, ftp={}, no_proxy={})'.format(
-            self.http, self.https, self.ftp, self.no_proxy)
+        return "ProxyConfig(http={}, https={}, ftp={}, no_proxy={})".format(
+            self.http, self.https, self.ftp, self.no_proxy
+        )
```

### Comparing `ipsw-0.1.2/ipsw/utils/socket.py` & `ipsw-0.1.3/ipsw/utils/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,30 +30,28 @@
 
     recoverable_errors = (errno.EINTR, errno.EDEADLK, errno.EWOULDBLOCK)
 
     if not isinstance(socket, NpipeSocket):
         select.select([socket], [], [])
 
     try:
-        if hasattr(socket, 'recv'):
+        if hasattr(socket, "recv"):
             return socket.recv(n)
-        if isinstance(socket, getattr(pysocket, 'SocketIO')):
+        if isinstance(socket, getattr(pysocket, "SocketIO")):
             return socket.read(n)
         return os.read(socket.fileno(), n)
     except OSError as e:
         if e.errno not in recoverable_errors:
             raise
     except Exception as e:
-        is_pipe_ended = (isinstance(socket, NpipeSocket) and
-                         len(e.args) > 0 and
-                         e.args[0] == NPIPE_ENDED)
+        is_pipe_ended = isinstance(socket, NpipeSocket) and len(e.args) > 0 and e.args[0] == NPIPE_ENDED
         if is_pipe_ended:
             # npipes don't support duplex sockets, so we interpret
             # a PIPE_ENDED error as a close operation (0-length read).
-            return ''
+            return ""
         raise
 
 
 def read_exactly(socket, n):
     """
     Reads exactly n bytes from socket
     Raises SocketError if there isn't enough data
@@ -73,15 +71,15 @@
     from socket, according to the protocol defined here:
     """
     try:
         data = read_exactly(socket, 8)
     except SocketError:
         return (-1, -1)
 
-    stream, actual = struct.unpack('>BxxxL', data)
+    stream, actual = struct.unpack(">BxxxL", data)
     return (stream, actual)
 
 
 def frames_iter(socket, tty):
     """
     Return a generator of frames read from socket. A frame is a tuple where
     the first item is the stream number and the second item is a chunk of data.
@@ -172,8 +170,8 @@
     socket.
     """
     if stream_id == STDOUT:
         return (data, None)
     elif stream_id == STDERR:
         return (None, data)
     else:
-        raise ValueError(f'{stream_id} is not a valid stream')
+        raise ValueError(f"{stream_id} is not a valid stream")
```

### Comparing `ipsw-0.1.2/ipsw/utils/utils.py` & `ipsw-0.1.3/ipsw/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.2/ipsw/version.py` & `ipsw-0.1.3/ipsw/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,13 +2,14 @@
     from ._version import __version__
 except ImportError:
     try:
         # importlib.metadata available in Python 3.8+, the fallback (0.0.0)
         # is fine because release builds use _version (above) rather than
         # this code path, so it only impacts developing w/ 3.7
         from importlib.metadata import version, PackageNotFoundError
+
         try:
-            __version__ = version('ipsw')
+            __version__ = version("ipsw")
         except PackageNotFoundError:
-            __version__ = '0.0.0'
+            __version__ = "0.0.0"
     except ImportError:
-        __version__ = '0.0.0'
+        __version__ = "0.0.0"
```

### Comparing `ipsw-0.1.2/ipsw.egg-info/SOURCES.txt` & `ipsw-0.1.3/ipsw.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -31,18 +31,20 @@
 ipsw.egg-info/dependency_links.txt
 ipsw.egg-info/not-zip-safe
 ipsw.egg-info/requires.txt
 ipsw.egg-info/top_level.txt
 ipsw/api/__init__.py
 ipsw/api/client.py
 ipsw/api/daemon.py
+ipsw/api/dsc.py
 ipsw/api/info.py
 ipsw/api/macho.py
 ipsw/models/__init__.py
 ipsw/models/configs.py
+ipsw/models/dsc.py
 ipsw/models/info.py
 ipsw/models/macho.py
 ipsw/models/resource.py
 ipsw/transport/__init__.py
 ipsw/transport/basehttpadapter.py
 ipsw/transport/npipeconn.py
 ipsw/transport/npipesocket.py
```

### Comparing `ipsw-0.1.2/scripts /release.sh` & `ipsw-0.1.3/scripts /release.sh`

 * *Files identical despite different names*

### Comparing `ipsw-0.1.2/setup.py` & `ipsw-0.1.3/setup.py`

 * *Files identical despite different names*

