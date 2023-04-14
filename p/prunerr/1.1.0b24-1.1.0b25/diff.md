# Comparing `tmp/prunerr-1.1.0b24.tar.gz` & `tmp/prunerr-1.1.0b25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prunerr-1.1.0b24.tar", last modified: Tue Apr 11 23:08:35 2023, max compression
+gzip compressed data, was "prunerr-1.1.0b25.tar", last modified: Fri Apr 14 00:48:36 2023, max compression
```

## Comparing `prunerr-1.1.0b24.tar` & `prunerr-1.1.0b25.tar`

### file list

```diff
@@ -1,1373 +1,1377 @@
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      543 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.dir-locals.el.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1503 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.dockerignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1226 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.env.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.118917 prunerr-1.1.0b24/.github/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/.github/workflows/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3938 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.github/workflows/build-test.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1503 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2764 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.gitlab-ci.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      779 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.pre-commit-config.yaml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2448 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.prospector.yaml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3897 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/CONTRIBUTING.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2430 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/Dockerfile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2753 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/Dockerfile.devel
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1081 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/LICENSE
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    57155 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3631 2023-04-11 23:08:29.000000 prunerr-1.1.0b24/NEWS.rst
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    14120 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/PKG-INFO
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13132 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/README.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3999 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/TODO.rst
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/bin/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2792 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/bin/cz-check-bump
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      918 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/bin/entrypoint
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     1101 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/bin/get-base-version
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      321 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/bin/hadolint
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/build-host/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1994 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/build-host/Dockerfile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1404 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/build-host/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      746 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/build-host/README.rst
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/build-host/bin/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2041 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/build-host/bin/entrypoint
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      731 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/build-host/requirements-py310.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      674 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/build-host/requirements-py311.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      948 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/build-host/requirements-py37.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      729 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/build-host/requirements-py38.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      729 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/build-host/requirements-py39.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        4 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/build-host/requirements.txt.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/dist/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/dist/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1397 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/docker-compose-servarr.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5034 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/docker-compose.override.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4029 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/docker-compose.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/gitlab-runner/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       46 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/gitlab-runner/.gitignore
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/gitlab-runner/config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1323 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/gitlab-runner/config/config.toml.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/home/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       64 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/home/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      327 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/home/.pypirc.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2979 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/pyproject.toml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/requirements/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      578 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/requirements/build.txt.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/requirements/py310/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2414 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/requirements/py310/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5273 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py310/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py310/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/requirements/py311/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2414 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/requirements/py311/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5024 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py311/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py311/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/requirements/py37/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2645 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/requirements/py37/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     6115 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py37/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1398 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py37/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/requirements/py38/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2142 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/requirements/py38/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5591 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py38/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py38/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/requirements/py39/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2412 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/requirements/py39/build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5578 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py39/devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py39/user.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/s6/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/s6/etc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/s6/etc/s6-overlay/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/s6/etc/s6-overlay/s6-rc.d/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/s6/etc/s6-overlay/s6-rc.d/svc-transmission/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      243 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1764 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/setup.cfg
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/src/prunerr/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8431 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/__init__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      201 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/__main__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    15438 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/downloadclient.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11377 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/downloaditem.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/home/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/src/prunerr/home/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9913 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/home/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/src/prunerr/newsfragments/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       91 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/newsfragments/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     7937 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/operations.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    19064 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/runner.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11415 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/servarr.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      911 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    22019 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/__init__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    67861 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/example-5s.mkv
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/daemon/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/daemon/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3204 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/daemon/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/download-client-only/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/download-client-only/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/download-client-only/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/download-clients/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/download-clients/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2957 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/download-clients/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/download-items/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/download-items/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/download-items/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/empty/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/empty/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/empty/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/move-exec/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/move-exec/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       88 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/move-exec/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/review-edge-cases/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/review-edge-cases/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      820 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:07:25.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1077 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9537 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:07:25.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13662 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5081 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      126 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1484 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1495 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1498 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2102 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:07:25.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16163 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5383 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5495 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:07:25.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:07:25.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    27061 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       61 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10807 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      123 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4730 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_cli.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2906 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_daemon.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8822 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_downloadclient.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3745 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_downloaditem.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11350 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_free_space.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17208 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_move.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8074 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_operations.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13110 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_review.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1468 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_runner.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_servarr.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1204 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_verify.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1374 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/utils.py
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      163 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr/version.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/src/prunerr.egg-info/
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    14120 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr.egg-info/PKG-INFO
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    64631 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr.egg-info/SOURCES.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)        1 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr.egg-info/dependency_links.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)       41 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr.egg-info/entry_points.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      327 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr.egg-info/requires.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)        8 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr.egg-info/top_level.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3321 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/tox.ini
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      543 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/.dir-locals.el.in
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1485 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/.dockerignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1226 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/.env.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.634627 prunerr-1.1.0b25/.github/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/.github/workflows/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3938 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/.github/workflows/build-test.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1485 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4149 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/.gitlab-ci.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      779 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/.pre-commit-config.yaml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2448 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/.prospector.yaml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3895 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/CONTRIBUTING.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2430 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/Dockerfile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2753 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/Dockerfile.devel
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1081 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/LICENSE
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    57756 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/Makefile
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)       86 2023-04-14 00:37:04.000000 prunerr-1.1.0b25/NEWS-VERSION.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3718 2023-04-14 00:37:06.000000 prunerr-1.1.0b25/NEWS.rst
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    14120 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/PKG-INFO
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13132 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/README.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3999 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/TODO.rst
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/bin/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2792 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/bin/cz-check-bump
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      918 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/bin/entrypoint
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     1101 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/bin/get-base-version
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      321 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/bin/hadolint
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/build-host/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1994 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/build-host/Dockerfile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1464 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/build-host/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      746 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/build-host/README.rst
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/build-host/bin/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2041 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/build-host/bin/entrypoint
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      731 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/build-host/requirements-py310.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      674 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/build-host/requirements-py311.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      948 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/build-host/requirements-py37.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      729 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/build-host/requirements-py38.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      729 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/build-host/requirements-py39.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        4 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/build-host/requirements.txt.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/dist/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/dist/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1397 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/docker-compose-servarr.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5034 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/docker-compose.override.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4029 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/docker-compose.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/gitlab-runner/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       46 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/gitlab-runner/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/gitlab-runner/config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1323 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/gitlab-runner/config/config.toml.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/home/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       64 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/home/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      327 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/home/.pypirc.in
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3008 2023-04-14 00:37:06.000000 prunerr-1.1.0b25/pyproject.toml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/requirements/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      578 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/requirements/build.txt.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/requirements/py310/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2414 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/requirements/py310/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5273 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/requirements/py310/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/requirements/py310/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/requirements/py311/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2414 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/requirements/py311/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5024 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/requirements/py311/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/requirements/py311/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/requirements/py37/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2645 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/requirements/py37/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     6115 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/requirements/py37/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1398 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/requirements/py37/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/requirements/py38/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2142 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/requirements/py38/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5591 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/requirements/py38/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/requirements/py38/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/requirements/py39/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2412 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/requirements/py39/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5578 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/requirements/py39/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-14 00:37:21.000000 prunerr-1.1.0b25/requirements/py39/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.634627 prunerr-1.1.0b25/s6/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.634627 prunerr-1.1.0b25/s6/etc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.634627 prunerr-1.1.0b25/s6/etc/s6-overlay/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.634627 prunerr-1.1.0b25/s6/etc/s6-overlay/s6-rc.d/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/s6/etc/s6-overlay/s6-rc.d/svc-transmission/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      243 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1764 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/setup.cfg
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8431 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/__init__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      201 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/__main__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    15438 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/downloadclient.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11377 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/downloaditem.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.634627 prunerr-1.1.0b25/src/prunerr/home/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/home/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9913 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/home/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/newsfragments/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       91 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/newsfragments/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     7937 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/operations.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    19064 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/runner.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11415 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/servarr.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      911 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    22019 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/__init__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    67861 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/example-5s.mkv
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/home/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.634627 prunerr-1.1.0b25/src/prunerr/tests/home/daemon/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/home/daemon/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3204 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/home/daemon/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.634627 prunerr-1.1.0b25/src/prunerr/tests/home/download-client-only/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/home/download-client-only/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/home/download-client-only/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.634627 prunerr-1.1.0b25/src/prunerr/tests/home/download-clients/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/home/download-clients/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2957 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/home/download-clients/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/home/download-items/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/home/download-items/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/home/download-items/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/home/empty/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/home/empty/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/home/empty/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/home/move-exec/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/home/move-exec/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       88 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/home/move-exec/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/home/review-edge-cases/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/home/review-edge-cases/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      820 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:47:34.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1077 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9537 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:47:34.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13662 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.638628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5081 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      126 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.666628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1484 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.642628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1495 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1498 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.670628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.646628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.650628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.674628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2102 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:47:34.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16163 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5383 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5495 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:47:34.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:47:34.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    27061 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       61 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.654628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.678628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10807 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      123 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4730 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/test_cli.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2906 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/test_daemon.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8822 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/test_downloadclient.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3745 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/test_downloaditem.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11350 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/test_free_space.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17208 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/test_move.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8074 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/test_operations.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13110 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/test_review.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1468 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/test_runner.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/test_servarr.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1204 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/tests/test_verify.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1374 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/prunerr/utils.py
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)      163 2023-04-14 00:48:36.000000 prunerr-1.1.0b25/src/prunerr/version.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.662628 prunerr-1.1.0b25/src/prunerr.egg-info/
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    14120 2023-04-14 00:48:36.000000 prunerr-1.1.0b25/src/prunerr.egg-info/PKG-INFO
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    64721 2023-04-14 00:48:36.000000 prunerr-1.1.0b25/src/prunerr.egg-info/SOURCES.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)        1 2023-04-14 00:48:36.000000 prunerr-1.1.0b25/src/prunerr.egg-info/dependency_links.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)       41 2023-04-14 00:48:36.000000 prunerr-1.1.0b25/src/prunerr.egg-info/entry_points.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)      327 2023-04-14 00:48:36.000000 prunerr-1.1.0b25/src/prunerr.egg-info/requires.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)        8 2023-04-14 00:48:36.000000 prunerr-1.1.0b25/src/prunerr.egg-info/top_level.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.658628 prunerr-1.1.0b25/src/pythonprojectstructure/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-14 00:48:36.682628 prunerr-1.1.0b25/src/pythonprojectstructure/newsfragments/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       87 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/src/pythonprojectstructure/newsfragments/upgrade-requirements.bugfix.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3321 2023-04-14 00:36:13.000000 prunerr-1.1.0b25/tox.ini
```

### Comparing `prunerr-1.1.0b24/.dir-locals.el.in` & `prunerr-1.1.0b25/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/.dockerignore` & `prunerr-1.1.0b25/.dockerignore`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,14 @@
 .ropeproject
 
 # Emacs editor settings
 /.dir-locals.el
 
 # Project-specific artifacts
 /README.md
-/NEWS-release.rst
 /radarr
 /sonarr
 /transmission
 
 # Explicit ignores for the Docker build context.
 .local
 **/.local
```

### Comparing `prunerr-1.1.0b24/.env.in` & `prunerr-1.1.0b25/.env.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/.github/workflows/build-test.yml` & `prunerr-1.1.0b25/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/.gitignore` & `prunerr-1.1.0b25/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,14 @@
 .ropeproject
 
 # Emacs editor settings
 /.dir-locals.el
 
 # Project-specific artifacts
 /README.md
-/NEWS-release.rst
 /radarr
 /sonarr
 /transmission
 
 # Explicit ignores for the Docker build context.
 .local
 **/.local
```

### Comparing `prunerr-1.1.0b24/.gitlab-ci.yml` & `prunerr-1.1.0b25/.gitlab-ci.yml`

 * *Files 24% similar despite different names*

```diff
@@ -20,23 +20,35 @@
   GH_TOKEN: "$PROJECT_GITHUB_PAT"
   # Uncomment to get more debugging output:
   # DEBUG: "true"
 
 stages:
   - "build-test"
   - "release"
+  - "release-bump"
+  - "release-version"
   - "scheduled"
 
 build-test:
   stage: "build-test"
   rules:
     - if: >-
-        ($CI_COMMIT_TAG == null || $CI_COMMIT_TAG == "")
-        && $CI_PIPELINE_SOURCE != "schedule"
-        && $CI_COMMIT_MESSAGE !~ /(?ims).*\[actions skip\].*/
+        $CI_COMMIT_BRANCH != null
+        && (
+          $CI_COMMIT_BRANCH !~ /^(develop|master)$/
+          || (
+            $CI_COMMIT_BRANCH == "develop"
+            && $CI_COMMIT_TITLE =~
+        /^build\(release\): Version [0-9]+\.[0-9]+\.[0-9]+.* → [0-9]+\.[0-9]+\.[0-9]+[^0-9].+$/
+          ) || (
+            $CI_COMMIT_BRANCH == "master"
+            && $CI_COMMIT_TITLE =~
+        /^build\(release\): Version [0-9]+\.[0-9]+\.[0-9]+.* → [0-9]+\.[0-9]+\.[0-9]+$/
+          )
+        )
   interruptible: true
   parallel:
     matrix:
       - PYTHON_MINORS:
           - "3.11"
           - "3.10"
           - "3.9"
@@ -74,28 +86,70 @@
   # Avoid unnecessary artifact downloads:
   # https://docs.gitlab.com/ee/ci/yaml/#dependencies
   dependencies: []
   variables:
     DOCKER_BUILD_PULL: "true"
   rules:
     - if: >-
-        ($CI_COMMIT_TAG == null || $CI_COMMIT_TAG == "")
+        (
+          (
+            $CI_COMMIT_BRANCH == "develop"
+            && $CI_COMMIT_TITLE =~
+        /^build\(release\): Version [0-9]+\.[0-9]+\.[0-9]+.* → [0-9]+\.[0-9]+\.[0-9]+[^0-9].+$/
+          ) || (
+            $CI_COMMIT_BRANCH == "master"
+            && $CI_COMMIT_TITLE =~
+        /^build\(release\): Version [0-9]+\.[0-9]+\.[0-9]+.* → [0-9]+\.[0-9]+\.[0-9]+$/
+          )
+        )
         && $CI_PROJECT_NAMESPACE == "rpatterson"
-        && $CI_COMMIT_BRANCH != null
-        && $CI_COMMIT_BRANCH =~ "^(develop|master)$"
-        && $CI_PIPELINE_SOURCE != "schedule"
-        && $CI_COMMIT_MESSAGE !~ /(?ims).*\[actions skip\].*/
   script:
     - >-
       entrypoint make -e release-python test-clean
   artifacts:
     paths:
-      - "./NEWS-release.rst"
       - "./dist/prunerr-*"
 
+release-bump:
+  stage: "release-bump"
+  needs: []
+  dependencies: []
+  variables:
+    DOCKER_BUILD_PULL: "true"
+  rules:
+    - if: >-
+        (
+          (
+            $CI_COMMIT_BRANCH == "master"
+            && $CI_COMMIT_TITLE !~
+        /^build\(release\): Version [0-9]+\.[0-9]+\.[0-9]+.* → [0-9]+\.[0-9]+\.[0-9]+$/
+          ) || (
+            $CI_COMMIT_BRANCH == "develop"
+            && $CI_COMMIT_TITLE !~
+        /^build\(release\): Version [0-9]+\.[0-9]+\.[0-9]+.* → [0-9]+\.[0-9]+\.[0-9].*$/
+          )
+        )
+  script:
+    - >-
+      entrypoint make -e release-bump
+
+# Workaround GitLab's handling of pipeline status when pushing both a branch and a tag:
+release-version:
+  stage: "release-version"
+  needs: []
+  dependencies: []
+  rules:
+    - if: >-
+        $CI_COMMIT_TAG =~ /^v[0-9]+\.[0-9]+\.[0-9]+.*$/
+  inherit:
+    default: false
+  script:
+    - >-
+      true
+
 scheduled:
   stage: "scheduled"
   rules:
     - if: >-
         $CI_PIPELINE_SOURCE == "schedule"
   script:
     - >-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `prunerr-1.1.0b24/.pre-commit-config.yaml` & `prunerr-1.1.0b25/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/.prospector.yaml` & `prunerr-1.1.0b25/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/CONTRIBUTING.rst` & `prunerr-1.1.0b25/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
   $ make
 
 If there's not already `an issue/ticket`_ for the changes you'll be making, create one.
 Regardless, take note of the issue/ticket number, e.g. ``#123``.  Then create a
 branch/fork off of the ``develop`` branch::
 
-  $ git checkout -b feat-123-foo-bar origin/develop
+  $ git switch -c feat-123-foo-bar origin/develop
 
 This project uses `towncrier`_ to manage it's release notes, AKA changelog and thus
 requires at least one `news fragment`_ before merging back into ``develop``.  The VCS
 hooks enforce this when pushing to ``develop`` or ``master``::
 
   $ towncrier create 123.feature
```

### Comparing `prunerr-1.1.0b24/Dockerfile` & `prunerr-1.1.0b25/Dockerfile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/Dockerfile.devel` & `prunerr-1.1.0b25/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/LICENSE` & `prunerr-1.1.0b25/LICENSE`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/Makefile` & `prunerr-1.1.0b25/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -95,21 +95,43 @@
 PYTHON_SHORT_MINORS=$(subst .,,$(PYTHON_MINORS))
 PYTHON_ENVS=$(PYTHON_SHORT_MINORS:%=py%)
 PYTHON_ALL_ENVS=$(PYTHON_ENVS) build
 export PYTHON_WHEEL=
 
 # Values derived from VCS/git:
 VCS_LOCAL_BRANCH:=$(shell git branch --show-current)
-CI_COMMIT_REF_NAME=
+CI_COMMIT_BRANCH=
+GITHUB_REF_TYPE=
 GITHUB_REF_NAME=
-ifneq ($(CI_COMMIT_REF_NAME),)
-VCS_LOCAL_BRANCH=$(CI_COMMIT_REF_NAME)
-else ifneq ($(GITHUB_REF_NAME),)
+ifeq ($(VCS_LOCAL_BRANCH),)
+ifneq ($(CI_COMMIT_BRANCH),)
+VCS_LOCAL_BRANCH=$(CI_COMMIT_BRANCH)
+else ifeq ($(GITHUB_REF_TYPE),branch)
 VCS_LOCAL_BRANCH=$(GITHUB_REF_NAME)
 endif
+endif
+VCS_TAG=
+CI_COMMIT_TAG=
+ifeq ($(VCS_TAG),)
+ifneq ($(CI_COMMIT_TAG),)
+VCS_TAG=$(CI_COMMIT_TAG)
+else ifeq ($(GITHUB_REF_TYPE),tag)
+VCS_TAG=$(GITHUB_REF_NAME)
+endif
+endif
+ifeq ($(VCS_LOCAL_BRANCH),)
+# Guess branch name from tag:
+ifneq ($(shell echo "$(VCS_TAG)" | grep -E '^v[0-9]+\.[0-9]+\.[0-9]+$$'),)
+# Final release, should be from master:
+VCS_LOCAL_BRANCH=master
+else ifneq ($(shell echo "$(VCS_TAG)" | grep -E '^v[0-9]+\.[0-9]+\.[0-9]+.+$$'),)
+# Pre-release, should be from develop:
+VCS_LOCAL_BRANCH=develop
+endif
+endif
 # Reproduce what we need of git's branch and remote configuration and logic:
 VCS_CLONE_REMOTE:=$(shell git config "clone.defaultRemoteName")
 ifeq ($(VCS_CLONE_REMOTE),)
 VCS_CLONE_REMOTE=origin
 endif
 VCS_PUSH_REMOTE:=$(shell git config "branch.$(VCS_LOCAL_BRANCH).pushRemote")
 ifeq ($(VCS_PUSH_REMOTE),)
@@ -427,28 +449,28 @@
 
 .PHONY: $(DOCKER_REGISTRIES:%=build-docker-tags-%)
 ### Print the list of image tags for the current registry and variant.
 $(DOCKER_REGISTRIES:%=build-docker-tags-%): \
 		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
 		./var/log/tox/build/build.log
 	docker_image=$(DOCKER_IMAGE_$(@:build-docker-tags-%=%))
+	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)
+ifeq ($(VCS_BRANCH),master)
+# Only update tags end users may depend on to be stable from the `master` branch
 	VERSION=$$(./.tox/build/bin/cz version --project)
 	major_version=$$(echo $${VERSION} | sed -nE 's|([0-9]+).*|\1|p')
 	minor_version=$$(
 	    echo $${VERSION} | sed -nE 's|([0-9]+\.[0-9]+).*|\1|p'
 	)
-	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)
-ifeq ($(VCS_BRANCH),master)
-# Only update tags end users may depend on to be stable from the `master` branch
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$${minor_version}
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$${major_version}
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)
 endif
 # This variant is the default used for tags such as `latest`
-ifeq ($(PYTHON_ENV),$(PYTHON_LATEST_ENV))
+ifeq ($(PYTHON_MINOR),$(PYTHON_HOST_MINOR))
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(DOCKER_BRANCH_TAG)
 ifeq ($(VCS_BRANCH),master)
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$${minor_version}
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$${major_version}
 ifeq ($(DOCKER_VARIANT),)
 	echo $${docker_image}:latest
 else
@@ -619,72 +641,34 @@
 ### Publish installable Python packages and container images as required by commits.
 release: release-python release-docker
 
 .PHONY: release-python
 ### Publish installable Python packages to PyPI.
 release-python: ./var/log/tox/build/build.log $(VCS_RELEASE_FETCH_TARGETS) \
 		~/.pypirc ./.env build-docker-volumes-$(PYTHON_ENV)
-ifeq ($(VCS_BRANCH),master)
-	if ! ./.tox/build/bin/python ./bin/get-base-version $$(
-	    ./.tox/build/bin/cz version --project
-	)
-	then
-# There's no pre-release for which to publish a final release:
-	    exit
-	fi
-else
-# Only release if required by conventional commits:
-	exit_code=0
-	./.tox/build/bin/python ./bin/cz-check-bump || exit_code=$$?
-	if (( $$exit_code == 3 || $$exit_code == 21 ))
-	then
-# No commits require a release:
-	    exit
-	elif (( $$exit_code != 0 ))
-	then
-	    exit $$exit_code
-	fi
-endif
 # Only release from the `master` or `develop` branches:
 ifeq ($(RELEASE_PUBLISH),true)
 # Import the private signing key from CI secrets
 	$(MAKE) -e ./var/log/gpg-import.log
 # Bump the version and build the final release packages:
-	$(MAKE) -e release-bump build-pkgs
+	$(MAKE) -e build-pkgs
 # https://twine.readthedocs.io/en/latest/#using-twine
 	./.tox/build/bin/twine check ./dist/prunerr-*
 # The VCS remote should reflect the release before the release is published to ensure
 # that a published release is never *not* reflected in VCS.  Also ensure the tag is in
 # place on any mirrors, using multiple `pushurl` remotes, for those project hosts as
 # well:
 	$(MAKE) -e test-clean
-ifeq ($(VCS_BRANCH),master)
-# Merge the bumped version back into `develop`:
-	bump_rev="$$(git rev-parse HEAD)"
-	git checkout --track "$(VCS_COMPARE_REMOTE)/develop" --
-	git merge --ff --gpg-sign \
-	    -m "Merge branch 'master' release back into develop" "$${bump_rev}"
-	git push --no-verify --tags "$(VCS_COMPARE_REMOTE)" "HEAD:develop"
-	git checkout "$${bump_rev}" --
-endif
-ifneq ($(GITHUB_ACTIONS),true)
-ifneq ($(PROJECT_GITHUB_PAT),)
-# Ensure the tag is available for creating the GitHub release below but push *before* to
-# GitLab to avoid a race with repository mirrorying:
-	git push --no-verify --tags "github" "HEAD:$(VCS_BRANCH)"
-endif
-endif
-	git push --no-verify --tags "$(VCS_REMOTE)" "HEAD:$(VCS_BRANCH)"
 	./.tox/build/bin/twine upload -s -r "$(PYPI_REPO)" \
 	    ./dist/prunerr-*
 	export VERSION=$$(./.tox/build/bin/cz version --project)
 # Create a GitLab release:
 	./.tox/build/bin/twine upload -s -r "gitlab" \
 	    ./dist/prunerr-*
-	release_cli_args="--description ./NEWS-release.rst"
+	release_cli_args="--description ./NEWS-VERSION.rst"
 	release_cli_args+=" --tag-name v$${VERSION}"
 	release_cli_args+=" --assets-link {\
 	\"name\":\"PyPI\",\
 	\"url\":\"https://$(PYPI_HOSTNAME)/project/$(CI_PROJECT_NAME)/$${VERSION}/\",\
 	\"link_type\":\"package\"\
 	}"
 	release_cli_args+=" --assets-link {\
@@ -699,29 +683,29 @@
 	}"
 	docker compose pull gitlab-release-cli
 	docker compose run --rm gitlab-release-cli release-cli \
 	    --server-url "$(CI_SERVER_URL)" --project-id "$(CI_PROJECT_ID)" \
 	    create $${release_cli_args}
 # Create a GitHub release
 	gh release create "v$${VERSION}" $(GITHUB_RELEASE_ARGS) \
-	    --notes-file "./NEWS-release.rst" ./dist/prunerr-*
+	    --notes-file "./NEWS-VERSION.rst" ./dist/prunerr-*
 endif
 
 .PHONY: release-docker
 ### Publish all container images to all container registries.
 release-docker: build-docker-volumes-$(PYTHON_ENV) build-docker \
 		$(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log)
 	$(MAKE) -e -j $(PYTHON_MINORS:%=release-docker-%)
 
 .PHONY: $(PYTHON_MINORS:%=release-docker-%)
 ### Publish the container images for one Python version to all container registry.
 $(PYTHON_MINORS:%=release-docker-%): $(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log)
 	export PYTHON_ENV="py$(subst .,,$(@:release-docker-%=%))"
 	$(MAKE) -e -j $(DOCKER_REGISTRIES:%=release-docker-registry-%)
-ifeq ($${PYTHON_ENV},$(PYTHON_LATEST_ENV))
+ifeq ($${PYTHON_ENV},$(PYTHON_HOST_ENV))
 	$(MAKE) -e "./var/log/docker-login-DOCKER.log"
 	docker compose pull pandoc docker-pushrm
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) docker-pushrm
 endif
 
 .PHONY: $(DOCKER_REGISTRIES:%=release-docker-registry-%)
 ### Publish all container images to one container registry.
@@ -751,14 +735,37 @@
 		./.env build-docker-volumes-$(PYTHON_ENV)
 	if ! git diff --cached --exit-code
 	then
 	    set +x
 	    echo "CRITICAL: Cannot bump version with staged changes"
 	    false
 	fi
+# Ensure the local branch is updated to the forthcoming version bump commit:
+	git switch -C "$(VCS_BRANCH)" "$$(git rev-parse HEAD)" --
+ifeq ($(VCS_BRANCH),master)
+	if ! ./.tox/build/bin/python ./bin/get-base-version $$(
+	    ./.tox/build/bin/cz version --project
+	)
+	then
+# There's no pre-release for which to publish a final release:
+	    exit
+	fi
+else
+# Only release if required by conventional commits:
+	exit_code=0
+	./.tox/build/bin/python ./bin/cz-check-bump || exit_code=$$?
+	if (( $$exit_code == 3 || $$exit_code == 21 ))
+	then
+# No commits require a release:
+	    exit
+	elif (( $$exit_code != 0 ))
+	then
+	    exit $$exit_code
+	fi
+endif
 # Collect the versions involved in this release according to conventional commits:
 	cz_bump_args="--check-consistency --no-verify"
 ifneq ($(VCS_BRANCH),master)
 	cz_bump_args+=" --prerelease beta"
 endif
 ifeq ($(RELEASE_PUBLISH),true)
 	cz_bump_args+=" --gpg-sign"
@@ -768,33 +775,56 @@
 # Capture the release notes for *just this* release for creating the GitHub release.
 # Have to run before the real `$ towncrier build` run without the `--draft` option
 # because after that the `newsfragments` will have been deleted.
 	next_version=$$(
 	    $(TOX_EXEC_BUILD_ARGS) cz bump $${cz_bump_args} --yes --dry-run |
 	    sed -nE 's|.* ([^ ]+) *→ *([^ ]+).*|\2|p'
 	) || true
-	docker compose run --rm prunerr-devel $(TOX_EXEC_ARGS) \
-	    towncrier build --version "$${next_version}" --draft --yes \
-	        >"./NEWS-release.rst"
 # Build and stage the release notes to be commited by `$ cz bump`
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) prunerr-devel \
+	    tox exec $(TOX_EXEC_OPTS) -e "$(PYTHON_ENV)" -qq -- \
+	    towncrier build --version "$${next_version}" --draft --yes \
+	    >"./NEWS-VERSION.rst"
+	git add -- "./NEWS-VERSION.rst"
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) prunerr-devel \
 	    $(TOX_EXEC_ARGS) towncrier build --version "$${next_version}" --yes
 # Increment the version in VCS
 	$(TOX_EXEC_BUILD_ARGS) cz bump $${cz_bump_args}
 # Ensure the container image reflects the version bump but we don't need to update the
 # requirements again.
 	touch \
 	    $(PYTHON_ENVS:%=./requirements/%/user.txt) \
 	    $(PYTHON_ENVS:%=./requirements/%/devel.txt) \
 	    $(PYTHON_ENVS:%=./build-host/requirements-%.txt)
 ifneq ($(CI),true)
 # If running under CI/CD then the image will be updated in the next pipeline stage.
 # For testing locally, however, ensure the image is up-to-date for subsequent recipes.
 	$(MAKE) -e "./var/docker/$(PYTHON_ENV)/log/build-user.log"
 endif
+ifeq ($(VCS_BRANCH),master)
+# Merge the bumped version back into `develop`:
+	bump_rev="$$(git rev-parse HEAD)"
+	git switch -C "develop" --track "$(VCS_COMPARE_REMOTE)/develop" --
+	git merge --ff --gpg-sign \
+	    -m "Merge branch 'master' release back into develop" "$${bump_rev}"
+ifeq ($(CI),true)
+	git push --no-verify --tags "$(VCS_COMPARE_REMOTE)" "HEAD:develop"
+endif
+	git switch -C "$(VCS_BRANCH)" "$${bump_rev}" --
+endif
+ifneq ($(GITHUB_ACTIONS),true)
+ifneq ($(PROJECT_GITHUB_PAT),)
+# Ensure the tag is available for creating the GitHub release below but push *before* to
+# GitLab to avoid a race with repository mirrorying:
+	git push --no-verify --tags "github" "HEAD:$(VCS_BRANCH)"
+endif
+endif
+ifeq ($(CI),true)
+	git push --no-verify --tags "$(VCS_REMOTE)" "HEAD:$(VCS_BRANCH)"
+endif
 
 
 ## Development Targets:
 #
 # Recipes used by developers to make changes to the code.
 
 .PHONY: devel-format
@@ -823,23 +853,15 @@
 devel-upgrade-branch: ~/.gitconfig ./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
 		./var/log/git-remotes.log
 	remote_branch_exists=false
 	if git fetch "$(VCS_REMOTE)" "$(VCS_BRANCH)-upgrade"
 	then
 	    remote_branch_exists=true
 	fi
-	if git show-ref -q --heads "$(VCS_BRANCH)-upgrade"
-	then
-# Reset an existing local branch to the latest upstream before upgrading
-	    git checkout "$(VCS_BRANCH)-upgrade"
-	    git reset --hard "$(VCS_BRANCH)" --
-	else
-# Create a new local branch from the latest upstream before upgrading
-	    git checkout -b "$(VCS_BRANCH)-upgrade" "$(VCS_BRANCH)"
-	fi
+	git switch -C "$(VCS_BRANCH)-upgrade" --track "$(VCS_BRANCH)" --
 	now=$$(date -u)
 	$(MAKE) -e devel-upgrade
 	if $(MAKE) -e "test-clean"
 	then
 # No changes from upgrade, exit successfully but push nothing
 	    exit
 	fi
@@ -988,18 +1010,14 @@
 else
 # https://github.com/moby/moby/issues/39003#issuecomment-879441675
 	docker_build_args="$(DOCKER_BUILD_ARGS) \
 	    --build-arg BUILDKIT_INLINE_CACHE=1 \
 	    --build-arg PYTHON_MINOR=$(PYTHON_MINOR) \
 	    --build-arg PYTHON_ENV=$(PYTHON_ENV) \
 	    --build-arg VERSION=$${VERSION}"
-ifeq ($(CI),true)
-# Workaround broken interactive session detection
-	docker pull "python:${PYTHON_MINOR}"
-endif
 	docker_build_devel_tags=""
 	for devel_tag in $$(
 	    $(MAKE) -e DOCKER_VARIANT="devel" --no-print-directory build-docker-tags
 	)
 	do
 	    docker_build_devel_tags+="--tag $${devel_tag} "
 	done
@@ -1021,14 +1039,18 @@
 	if $(MAKE) -e DOCKER_VARIANT="devel" pull-docker
 	then
 	    docker_build_caches+=" --cache-from \
 	$(DOCKER_IMAGE_GITHUB):devel-$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
 	fi
 endif
 endif
+ifeq ($(CI),true)
+# Workaround broken interactive session detection
+	docker pull "python:${PYTHON_MINOR}"
+endif
 	docker buildx build $${docker_build_args} $${docker_build_devel_tags} \
 	    $${docker_build_caches} --file "./Dockerfile.devel" "./"
 # Ensure any subsequent builds have optimal caches
 ifeq ($(GITLAB_CI),true)
 	docker push \
 	    "$(DOCKER_IMAGE_GITLAB):devel-$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
 endif
@@ -1228,14 +1250,15 @@
 # Ensure minimal VCS configuration, mostly useful in automation such as CI.
 ~/.gitconfig:
 	git config --global user.name "$(USER_FULL_NAME)"
 	git config --global user.email "$(USER_EMAIL)"
 
 ./var/log/git-remotes.log:
 ifeq ($(RELEASE_PUBLISH),true)
+	mkdir -pv "$(dir $(@))"
 	set +x
 ifneq ($(VCS_REMOTE_PUSH_URL),)
 	if ! git remote get-url --push --all "origin" |
 	    grep -q -F "$(VCS_REMOTE_PUSH_URL)"
 	then
 	    git remote set-url --push --add "origin" "$(VCS_REMOTE_PUSH_URL)" |
 	        tee -a "$(@)"
```

### Comparing `prunerr-1.1.0b24/NEWS.rst` & `prunerr-1.1.0b25/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+prunerr 1.1.0b25 (2023-04-14)
+=============================
+
+No significant changes.
+
+
 prunerr 1.1.0b24 (2023-04-11)
 =============================
 
 Bugfixes
 --------
 
 - Upgrade all requirements to the latest versions as of Tue Apr 11 08:15:25 PM UTC 2023. (upgrade-requirements)
```

### Comparing `prunerr-1.1.0b24/PKG-INFO` & `prunerr-1.1.0b25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prunerr
-Version: 1.1.0b24
+Version: 1.1.0b25
 Summary: Perma-seed Servarr media libraries
 Home-page: https://gitlab.com/rpatterson/prunerr
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `prunerr-1.1.0b24/README.rst` & `prunerr-1.1.0b25/README.rst`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/TODO.rst` & `prunerr-1.1.0b25/TODO.rst`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/bin/cz-check-bump` & `prunerr-1.1.0b25/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/bin/entrypoint` & `prunerr-1.1.0b25/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/bin/get-base-version` & `prunerr-1.1.0b25/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/build-host/Dockerfile` & `prunerr-1.1.0b25/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/build-host/Makefile` & `prunerr-1.1.0b25/build-host/Makefile`

 * *Files 15% similar despite different names*

```diff
@@ -45,10 +45,11 @@
 .PHONY: debug-github-checkout
 ## Reproduce the GitHub Actions shallow git checkout
 debug-github-checkout:
 	git init "$(CHECKOUT_DIR)"
 	cd "$(CHECKOUT_DIR)"
 	git remote add origin \
 	    "https://github.com/$(GITHUB_REPOSITORY_OWNER)/prunerr"
+	rev_hash="$$(git ls-remote -q "origin" "$(VCS_BRANCH)" | cut -f 1)"
 	git -c protocol.version=2 fetch --no-tags --prune --progress \
-	    --no-recurse-submodules --depth=1 "origin" "$(VCS_BRANCH)"
-	git checkout --progress --detach "origin/$(VCS_BRANCH)"
+	    --no-recurse-submodules --depth=1 "origin" "$${rev_hash}"
+	git checkout --progress --detach "$${rev_hash}"
```

### Comparing `prunerr-1.1.0b24/build-host/README.rst` & `prunerr-1.1.0b25/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/build-host/bin/entrypoint` & `prunerr-1.1.0b25/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/build-host/requirements-py310.txt` & `prunerr-1.1.0b25/build-host/requirements-py37.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py310.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py37.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
 filelock==3.11.0
     # via
     #   tox
     #   virtualenv
-packaging==23.0
+importlib-metadata==6.3.0
+    # via
+    #   pluggy
+    #   tox
+    #   virtualenv
+packaging==23.1
     # via
     #   pyproject-api
     #   tox
 platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
@@ -30,9 +35,16 @@
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.4.11
     # via -r build-host/requirements.txt.in
+typing-extensions==4.5.0
+    # via
+    #   importlib-metadata
+    #   platformdirs
+    #   tox
 virtualenv==20.21.0
     # via tox
+zipp==3.15.0
+    # via importlib-metadata
```

### Comparing `prunerr-1.1.0b24/build-host/requirements-py311.txt` & `prunerr-1.1.0b25/build-host/requirements-py311.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,23 @@
     # via tox
 distlib==0.3.6
     # via virtualenv
 filelock==3.11.0
     # via
     #   tox
     #   virtualenv
-packaging==23.0
+packaging==23.1
     # via
     #   pyproject-api
     #   tox
 platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
-tox==4.4.11
+tox==4.4.12
     # via -r build-host/requirements.txt.in
 virtualenv==20.21.0
     # via tox
```

### Comparing `prunerr-1.1.0b24/build-host/requirements-py37.txt` & `prunerr-1.1.0b25/build-host/requirements-py39.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py37.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py39.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
 filelock==3.11.0
     # via
     #   tox
     #   virtualenv
-importlib-metadata==6.3.0
-    # via
-    #   pluggy
-    #   tox
-    #   virtualenv
-packaging==23.0
+packaging==23.1
     # via
     #   pyproject-api
     #   tox
 platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
@@ -35,16 +30,9 @@
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.4.11
     # via -r build-host/requirements.txt.in
-typing-extensions==4.5.0
-    # via
-    #   importlib-metadata
-    #   platformdirs
-    #   tox
 virtualenv==20.21.0
     # via tox
-zipp==3.15.0
-    # via importlib-metadata
```

### Comparing `prunerr-1.1.0b24/build-host/requirements-py38.txt` & `prunerr-1.1.0b25/build-host/requirements-py310.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py38.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py310.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
 filelock==3.11.0
     # via
     #   tox
     #   virtualenv
-packaging==23.0
+packaging==23.1
     # via
     #   pyproject-api
     #   tox
 platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
@@ -28,11 +28,11 @@
     # via tox
 pyproject-api==1.5.1
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.4.11
+tox==4.4.12
     # via -r build-host/requirements.txt.in
 virtualenv==20.21.0
     # via tox
```

### Comparing `prunerr-1.1.0b24/build-host/requirements-py39.txt` & `prunerr-1.1.0b25/build-host/requirements-py38.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=build-host/requirements-py39.txt --resolver=backtracking build-host/requirements.txt.in
+#    pip-compile --output-file=build-host/requirements-py38.txt --resolver=backtracking build-host/requirements.txt.in
 #
 cachetools==5.3.0
     # via tox
 chardet==5.1.0
     # via tox
 colorama==0.4.6
     # via tox
 distlib==0.3.6
     # via virtualenv
 filelock==3.11.0
     # via
     #   tox
     #   virtualenv
-packaging==23.0
+packaging==23.1
     # via
     #   pyproject-api
     #   tox
 platformdirs==3.2.0
     # via
     #   tox
     #   virtualenv
```

### Comparing `prunerr-1.1.0b24/docker-compose-servarr.yml` & `prunerr-1.1.0b25/docker-compose-servarr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/docker-compose.override.yml` & `prunerr-1.1.0b25/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/docker-compose.yml` & `prunerr-1.1.0b25/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/gitlab-runner/config/config.toml.in` & `prunerr-1.1.0b25/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/pyproject.toml` & `prunerr-1.1.0b25/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -13,21 +13,23 @@
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 changelog_start_rev = "v0.0.0"
-version = "1.1.0b24"
+version = "1.1.0b25"
 tag_format = "v$version"
 annotated_tag = true
+gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
+[ci release]
 """
 [tool.towncrier]
 # https://towncrier.readthedocs.io/en/stable/#quick-start
 package = "prunerr"
 package_dir = "src"
 name = "prunerr"
```

### Comparing `prunerr-1.1.0b24/requirements/build.txt.in` & `prunerr-1.1.0b25/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/requirements/py310/build.txt` & `prunerr-1.1.0b25/requirements/py310/build.txt`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
@@ -88,15 +88,15 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.3
+rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 termcolor==2.2.0
     # via commitizen
```

### Comparing `prunerr-1.1.0b24/requirements/py310/devel.txt` & `prunerr-1.1.0b25/requirements/py310/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
```

### Comparing `prunerr-1.1.0b24/requirements/py310/user.txt` & `prunerr-1.1.0b25/requirements/py310/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/requirements/py311/build.txt` & `prunerr-1.1.0b25/requirements/py311/build.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
@@ -88,15 +88,15 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.3
+rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 termcolor==2.2.0
     # via commitizen
```

### Comparing `prunerr-1.1.0b24/requirements/py311/devel.txt` & `prunerr-1.1.0b25/requirements/py311/devel.txt`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
```

### Comparing `prunerr-1.1.0b24/requirements/py311/user.txt` & `prunerr-1.1.0b25/requirements/py311/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/requirements/py37/build.txt` & `prunerr-1.1.0b25/requirements/py37/build.txt`

 * *Files 8% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
 pre-commit==2.21.0
     # via -r requirements/build.txt.in
@@ -93,15 +93,15 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.3
+rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 termcolor==2.2.0
     # via commitizen
```

### Comparing `prunerr-1.1.0b24/requirements/py37/devel.txt` & `prunerr-1.1.0b25/requirements/py37/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
```

### Comparing `prunerr-1.1.0b24/requirements/py37/user.txt` & `prunerr-1.1.0b25/requirements/py37/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/requirements/py38/build.txt` & `prunerr-1.1.0b25/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/requirements/py38/devel.txt` & `prunerr-1.1.0b25/requirements/py38/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
```

### Comparing `prunerr-1.1.0b24/requirements/py38/user.txt` & `prunerr-1.1.0b25/requirements/py38/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/requirements/py39/build.txt` & `prunerr-1.1.0b25/requirements/py39/build.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
-packaging==23.0
+packaging==23.1
     # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
@@ -88,15 +88,15 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.3
+rich==13.3.4
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 termcolor==2.2.0
     # via commitizen
```

### Comparing `prunerr-1.1.0b24/requirements/py39/devel.txt` & `prunerr-1.1.0b25/requirements/py39/devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==23.0
+packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
     #   pytest
     #   requirements-detector
```

### Comparing `prunerr-1.1.0b24/requirements/py39/user.txt` & `prunerr-1.1.0b25/requirements/py39/user.txt`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/setup.cfg` & `prunerr-1.1.0b25/setup.cfg`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/__init__.py` & `prunerr-1.1.0b25/src/prunerr/__init__.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/downloadclient.py` & `prunerr-1.1.0b25/src/prunerr/downloadclient.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/downloaditem.py` & `prunerr-1.1.0b25/src/prunerr/downloaditem.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/home/.config/prunerr.yml` & `prunerr-1.1.0b25/src/prunerr/home/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/operations.py` & `prunerr-1.1.0b25/src/prunerr/operations.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/runner.py` & `prunerr-1.1.0b25/src/prunerr/runner.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -296,18 +296,18 @@
         self.quiet = False
         while True:
             # Start the clock for the poll loop as early as possible to keep the inner
             # loop duration as accurate as possible.
             start = time.time()
 
             try:
-                # Resume any corrupt download items that have finished verifying
-                self.resume_verified_items()
                 # Refresh the list of download items
                 self.update()
+                # Resume any corrupt download items that have finished verifying
+                self.resume_verified_items()
                 # Run the `exec` sub-command as the inner loop
                 self.exec_()
             except (
                 socket.error,
                 transmission_rpc.TransmissionError,
                 arrapi.exceptions.ConnectionFailure,
             ) as exc:
```

### Comparing `prunerr-1.1.0b24/src/prunerr/servarr.py` & `prunerr-1.1.0b25/src/prunerr/servarr.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/Makefile` & `prunerr-1.1.0b25/src/prunerr/tests/Makefile`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/__init__.py` & `prunerr-1.1.0b25/src/prunerr/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/example-5s.mkv` & `prunerr-1.1.0b25/src/prunerr/tests/example-5s.mkv`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/home/daemon/.config/prunerr.yml` & `prunerr-1.1.0b25/src/prunerr/tests/home/daemon/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/home/download-clients/.config/prunerr.yml` & `prunerr-1.1.0b25/src/prunerr/tests/home/download-clients/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml` & `prunerr-1.1.0b25/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json` & `prunerr-1.1.0b25/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/test_cli.py` & `prunerr-1.1.0b25/src/prunerr/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/test_daemon.py` & `prunerr-1.1.0b25/src/prunerr/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/test_downloadclient.py` & `prunerr-1.1.0b25/src/prunerr/tests/test_downloadclient.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/test_downloaditem.py` & `prunerr-1.1.0b25/src/prunerr/tests/test_downloaditem.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/test_free_space.py` & `prunerr-1.1.0b25/src/prunerr/tests/test_free_space.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/test_move.py` & `prunerr-1.1.0b25/src/prunerr/tests/test_move.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/test_operations.py` & `prunerr-1.1.0b25/src/prunerr/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/test_review.py` & `prunerr-1.1.0b25/src/prunerr/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/test_runner.py` & `prunerr-1.1.0b25/src/prunerr/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/test_servarr.py` & `prunerr-1.1.0b25/src/prunerr/tests/test_servarr.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/tests/test_verify.py` & `prunerr-1.1.0b25/src/prunerr/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr/utils.py` & `prunerr-1.1.0b25/src/prunerr/utils.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.1.0b24/src/prunerr.egg-info/PKG-INFO` & `prunerr-1.1.0b25/src/prunerr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prunerr
-Version: 1.1.0b24
+Version: 1.1.0b25
 Summary: Perma-seed Servarr media libraries
 Home-page: https://gitlab.com/rpatterson/prunerr
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `prunerr-1.1.0b24/src/prunerr.egg-info/SOURCES.txt` & `prunerr-1.1.0b25/src/prunerr.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 .pre-commit-config.yaml
 .prospector.yaml
 CONTRIBUTING.rst
 Dockerfile
 Dockerfile.devel
 LICENSE
 Makefile
+NEWS-VERSION.rst
 NEWS.rst
 README.rst
 TODO.rst
 docker-compose-servarr.yml
 docker-compose.override.yml
 docker-compose.yml
 pyproject.toml
@@ -540,8 +541,9 @@
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
 src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
-src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
+src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
+src/pythonprojectstructure/newsfragments/upgrade-requirements.bugfix.rst
```

### Comparing `prunerr-1.1.0b24/tox.ini` & `prunerr-1.1.0b25/tox.ini`

 * *Files identical despite different names*

