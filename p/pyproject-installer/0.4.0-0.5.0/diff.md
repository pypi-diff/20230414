# Comparing `tmp/pyproject_installer-0.4.0.tar.gz` & `tmp/pyproject_installer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_installer-0.4.0.tar", last modified: Wed Jan 11 09:00:08 2023, max compression
+gzip compressed data, was "pyproject_installer-0.5.0.tar", last modified: Fri Apr 14 12:17:06 2023, max compression
```

## Comparing `pyproject_installer-0.4.0.tar` & `pyproject_installer-0.5.0.tar`

### file list

```diff
@@ -1,57 +1,87 @@
--rw-r--r--   0        0        0       78 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/__init__.py
--rw-r--r--   0        0        0    10084 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/__main__.py
--rw-r--r--   0        0        0      271 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/codes.py
--rw-r--r--   0        0        0      208 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/errors.py
--rw-r--r--   0        0        0       18 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/version.py
--rw-r--r--   0        0        0      134 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/build_cmd/__init__.py
--rw-r--r--   0        0        0    11104 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/build_cmd/_build.py
--rw-r--r--   0        0        0        0 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/build_cmd/_vendor/__init__.py
--rw-r--r--   0        0        0      396 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/build_cmd/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/build_cmd/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/build_cmd/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/build_cmd/_vendor/tomli/_types.py
--rw-r--r--   0        0        0        0 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/build_cmd/helper/__init__.py
--rw-r--r--   0        0        0     5785 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/build_cmd/helper/backend_caller.py
--rw-r--r--   0        0        0       73 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/install_cmd/__init__.py
--rw-r--r--   0        0        0     6215 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/install_cmd/_install.py
--rw-r--r--   0        0        0      913 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/lib/entry_points.py
--rw-r--r--   0        0        0      193 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/lib/normalization.py
--rw-r--r--   0        0        0     1811 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/lib/scripts.py
--rw-r--r--   0        0        0    10893 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/lib/wheel.py
--rw-r--r--   0        0        0       65 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/run_cmd/__init__.py
--rw-r--r--   0        0        0      430 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/run_cmd/_run_command.py
--rw-r--r--   0        0        0     7008 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/src/pyproject_installer/run_cmd/_run_env.py
--rw-r--r--   0        0        0      172 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/backend/__init__.py
--rw-r--r--   0        0        0      367 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/backend/common.py
--rw-r--r--   0        0        0     2092 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/backend/config.py
--rw-r--r--   0        0        0     8581 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/backend/metadata.py
--rw-r--r--   0        0        0     5559 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/backend/sdist.py
--rw-r--r--   0        0        0     6922 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/backend/wheel.py
--rw-r--r--   0        0        0        0 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/backend/_vendor/__init__.py
--rw-r--r--   0        0        0      396 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/backend/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/backend/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/backend/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/backend/_vendor/tomli/_types.py
--rw-r--r--   0        0        0        0 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     4517 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     5169 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     4144 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/integration/test_backends.py
--rw-r--r--   0        0        0     1719 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/integration/test_buildable.py
--rw-r--r--   0        0        0     2238 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/integration/test_config_settings.py
--rw-r--r--   0        0        0        0 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/unit/__init__.py
--rw-r--r--   0        0        0    16773 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/unit/test_main.py
--rw-r--r--   0        0        0       92 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/unit/test_version.py
--rw-r--r--   0        0        0        0 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/unit/test_build/__init__.py
--rw-r--r--   0        0        0      505 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/unit/test_build/conftest.py
--rw-r--r--   0        0        0    14952 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/unit/test_build/test_backend_caller.py
--rw-r--r--   0        0        0     8852 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/unit/test_build/test_builder.py
--rw-r--r--   0        0        0     8178 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/unit/test_build/test_pyproject_parser.py
--rw-r--r--   0        0        0        0 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/unit/test_install/__init__.py
--rw-r--r--   0        0        0    17931 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/unit/test_install/test_installer.py
--rw-r--r--   0        0        0        0 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/unit/test_run/__init__.py
--rw-r--r--   0        0        0    17349 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/tests/unit/test_run/test_env.py
--rw-r--r--   0        0        0    11049 2023-01-11 09:00:08.000000 pyproject_installer-0.4.0/PKG-INFO
--rw-r--r--   0        0        0     3464 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    10097 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/README.md
--rw-r--r--   0        0        0     1024 2023-01-11 08:59:09.000000 pyproject_installer-0.4.0/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/__init__.py
+-rw-r--r--   0        0        0    16053 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/__main__.py
+-rw-r--r--   0        0        0      317 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/codes.py
+-rw-r--r--   0        0        0      391 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/errors.py
+-rw-r--r--   0        0        0       18 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/version.py
+-rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/__init__.py
+-rw-r--r--   0        0        0      501 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9399 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5148 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8161 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     3264 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39046 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18065 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16295 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      396 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0      134 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/build_cmd/__init__.py
+-rw-r--r--   0        0        0     1872 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/build_cmd/_build.py
+-rw-r--r--   0        0        0      206 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/__init__.py
+-rw-r--r--   0        0        0      181 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/_deps_command.py
+-rw-r--r--   0        0        0     9067 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/deps_config.py
+-rw-r--r--   0        0        0      618 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/collector.py
+-rw-r--r--   0        0        0     1653 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/metadata.py
+-rw-r--r--   0        0        0      825 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/pep517.py
+-rw-r--r--   0        0        0      679 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/pep518.py
+-rw-r--r--   0        0        0     1062 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/pip_reqfile.py
+-rw-r--r--   0        0        0     2481 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/poetry.py
+-rw-r--r--   0        0        0     2239 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/tox.py
+-rw-r--r--   0        0        0       73 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/install_cmd/__init__.py
+-rw-r--r--   0        0        0     6215 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/install_cmd/_install.py
+-rw-r--r--   0        0        0      270 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/__init__.py
+-rw-r--r--   0        0        0     9335 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/build_backend.py
+-rw-r--r--   0        0        0      913 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/entry_points.py
+-rw-r--r--   0        0        0      193 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/normalization.py
+-rw-r--r--   0        0        0     1811 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/scripts.py
+-rw-r--r--   0        0        0    10893 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/wheel.py
+-rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/backend_helper/__init__.py
+-rw-r--r--   0        0        0     5872 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/backend_helper/backend_caller.py
+-rw-r--r--   0        0        0       65 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/run_cmd/__init__.py
+-rw-r--r--   0        0        0      430 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/run_cmd/_run_command.py
+-rw-r--r--   0        0        0     7104 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/run_cmd/_run_env.py
+-rw-r--r--   0        0        0      172 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/__init__.py
+-rw-r--r--   0        0        0      367 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/common.py
+-rw-r--r--   0        0        0     2092 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/config.py
+-rw-r--r--   0        0        0     8581 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/metadata.py
+-rw-r--r--   0        0        0     5559 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/sdist.py
+-rw-r--r--   0        0        0     6922 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/wheel.py
+-rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/_vendor/__init__.py
+-rw-r--r--   0        0        0      396 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     4612 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     5082 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     4144 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/integration/test_backends.py
+-rw-r--r--   0        0        0     1719 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/integration/test_buildable.py
+-rw-r--r--   0        0        0     2238 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/integration/test_config_settings.py
+-rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0    31635 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_main.py
+-rw-r--r--   0        0        0       92 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_version.py
+-rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_build/__init__.py
+-rw-r--r--   0        0        0      509 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_build/conftest.py
+-rw-r--r--   0        0        0    15784 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_build/test_backend_caller.py
+-rw-r--r--   0        0        0     8736 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_build/test_builder.py
+-rw-r--r--   0        0        0     8179 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_build/test_pyproject_parser.py
+-rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_deps/__init__.py
+-rw-r--r--   0        0        0      495 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_deps/conftest.py
+-rw-r--r--   0        0        0    22637 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_deps/test_collectors.py
+-rw-r--r--   0        0        0    23966 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_deps/test_deps_config.py
+-rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_install/__init__.py
+-rw-r--r--   0        0        0    17931 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_install/test_installer.py
+-rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_run/__init__.py
+-rw-r--r--   0        0        0    18875 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_run/test_env.py
+-rw-r--r--   0        0        0    16949 2023-04-14 12:17:06.000000 pyproject_installer-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3464 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    15997 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/README.md
+-rw-r--r--   0        0        0     1024 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/LICENSE
```

### Comparing `pyproject_installer-0.4.0/src/pyproject_installer/build_cmd/_build.py` & `pyproject_installer-0.5.0/src/pyproject_installer/lib/build_backend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 from contextlib import suppress
 from pathlib import Path
 import json
 import logging
 import os
 import subprocess
-import sys
 import threading
 
-try:
-    # Python 3.11+
-    import tomllib
-except ModuleNotFoundError:
-    from ._vendor import tomli as tomllib
+from . import tomllib
 
 
 __all__ = [
-    "build_wheel",
-    "build_sdist",
-    "WHEEL_TRACKER",
+    "backend_hook",
+    "parse_build_system_spec",
 ]
 
 logger = logging.getLogger(__name__)
 
-BACKEND_CALLER = Path(__file__).parent / "helper" / "backend_caller.py"
-WHEEL_TRACKER = ".wheeltracker"
-
-SUPPORTED_BUILD_HOOKS = ("build_wheel", "build_sdist")
+BACKEND_CALLER = Path(__file__).parent / "backend_helper" / "backend_caller.py"
 
 
 class RaisingThread(threading.Thread):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._exc = None
 
@@ -187,15 +178,15 @@
                 ) from None
 
         bs["backend-path"] = backend_path
 
     return bs
 
 
-def make_args(python, result_fd, verbose, build_system, hook, hook_args):
+def make_helper_args(python, result_fd, verbose, build_system, hook, hook_args):
     args = [
         python,
         BACKEND_CALLER,
         "--result-fd",
         str(result_fd),
     ]
     if verbose:
@@ -230,73 +221,16 @@
     ):
         # not a Python project
         raise ValueError("Required either pyproject.toml or setup.py")
 
     return srcdir
 
 
-def build(srcdir, outdir, hook, config=None, verbose=False):
-    logger.info("Source tree: %s", srcdir)
-    logger.info("Output dir: %s", outdir)
-    if config is not None:
-        logger.info("Ad-hoc backend config: %r", config)
-
-    if hook not in SUPPORTED_BUILD_HOOKS:
-        raise ValueError(
-            f"Unknown build hook: {hook}, "
-            f"supported: {', '.join(SUPPORTED_BUILD_HOOKS)}"
-        )
+def backend_hook(python, srcdir, verbose, hook, hook_args=[(), {}]):
     srcdir = validate_source_dir(srcdir)
-
-    try:
-        outdir.mkdir(parents=True, exist_ok=True)
-    except PermissionError:
-        raise ValueError(
-            f"Unable to create path for outdir: {outdir}"
-        ) from None
-    outdir = outdir.resolve(strict=True)
-
-    hook_result = call_hook(
-        python=sys.executable,
-        srcdir=srcdir,
-        verbose=verbose,
-        hook=hook,
-        hook_args=[(str(outdir),), {"config_settings": config}],
-    )
-    return hook_result["result"]
-
-
-def build_wheel(srcdir, outdir, config=None, verbose=False):
-    logger.info("Building wheel")
-    wheel_filename = build(
-        srcdir,
-        outdir=outdir,
-        hook="build_wheel",
-        config=config,
-        verbose=verbose,
-    )
-
-    # track result for wheel installer
-    (outdir / WHEEL_TRACKER).write_text(f"{wheel_filename}\n", encoding="utf-8")
-    logger.info("Built wheel: %s", wheel_filename)
-
-
-def build_sdist(srcdir, outdir, config=None, verbose=False):
-    logger.info("Building sdist")
-    sdist_filename = build(
-        srcdir,
-        outdir=outdir,
-        hook="build_sdist",
-        config=config,
-        verbose=verbose,
-    )
-    logger.info("Built sdist: %s", sdist_filename)
-
-
-def call_hook(python, srcdir, verbose, hook, hook_args=[(), {}]):
     build_system = parse_build_system_spec(srcdir)
     read = b""
 
     rfd, wfd = os.pipe()
 
     try:
 
@@ -310,15 +244,15 @@
                 read += read_chunk
 
         t = RaisingThread(target=read_from_pipe)
         t.start()
         capture_output = not verbose
 
         try:
-            args = make_args(
+            args = make_helper_args(
                 python=python,
                 result_fd=wfd,
                 verbose=verbose,
                 build_system=build_system,
                 hook=hook,
                 hook_args=hook_args,
             )
```

### Comparing `pyproject_installer-0.4.0/src/pyproject_installer/build_cmd/_vendor/tomli/_parser.py` & `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/src/pyproject_installer/build_cmd/_vendor/tomli/_re.py` & `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/src/pyproject_installer/build_cmd/helper/backend_caller.py` & `pyproject_installer-0.5.0/src/pyproject_installer/lib/backend_helper/backend_caller.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 # hook name: fallback (None - mandatory hook)
 SUPPORTED_HOOKS = {
     "build_wheel": None,
     "build_sdist": None,
     "get_requires_for_build_wheel": [],
     "get_requires_for_build_sdist": [],
+    # PEP517 doesn't specify default value
+    "prepare_metadata_for_build_wheel": "",
 }
 
 
 def backend_object(backend, backend_path=None):
     if backend_path is not None:
         # Projects can specify that their backend code is hosted in-tree by
         # including the backend-path key in pyproject.toml. This key contains a
```

### Comparing `pyproject_installer-0.4.0/src/pyproject_installer/install_cmd/_install.py` & `pyproject_installer-0.5.0/src/pyproject_installer/install_cmd/_install.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/src/pyproject_installer/lib/entry_points.py` & `pyproject_installer-0.5.0/src/pyproject_installer/lib/entry_points.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/src/pyproject_installer/lib/scripts.py` & `pyproject_installer-0.5.0/src/pyproject_installer/lib/scripts.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/src/pyproject_installer/lib/wheel.py` & `pyproject_installer-0.5.0/src/pyproject_installer/lib/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/src/pyproject_installer/run_cmd/_run_env.py` & `pyproject_installer-0.5.0/src/pyproject_installer/run_cmd/_run_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,16 +122,15 @@
             "pyproject_installer",
             "install",
             str(self.wheel),
         ]
         try:
             self.run(install_args, capture_output=True)
         except RunCommandError as e:
-            err_msg = f"Installation of package failed:\n{str(e)}"
-            raise RunCommandEnvError(err_msg) from None
+            raise RunCommandEnvError("Installation of package failed") from e
 
     def create(self, *args, **kwargs):
         """Calls `post_create` hook after `venv` creation
 
         base implementation of `create` disables system_site_packages
         via pyvenv.cfg due to https://bugs.python.org/issue24875 (unable to
         install pip with --system-site-packages if pip is already installed
@@ -152,15 +151,20 @@
         """
         self.install_console_scripts(context)
         self.install_package(context)
 
     def venv_environ(self):
         """Prepare environ for venv"""
         env = os.environ.copy()
-        env["PATH"] = os.pathsep.join([self.context.bin_path, env["PATH"]])
+        try:
+            current_path = env["PATH"]
+        except KeyError:
+            env["PATH"] = self.context.bin_path
+        else:
+            env["PATH"] = os.pathsep.join([self.context.bin_path, current_path])
         env["VIRTUAL_ENV"] = self.context.env_dir
         return env
 
     def run(self, command, capture_output=False):
         """Run a command in subprocess within venv"""
         logger.info("Running command: %r", command)
         try:
@@ -177,9 +181,9 @@
                 if out_bytes:
                     out_text = out_bytes.decode(
                         encoding="utf-8", errors="replace"
                     )
                     err_msg += f"\n\nCommand's {out_src}:\n{out_text}"
             raise RunCommandError(err_msg) from None
         except Exception as e:
-            raise RunCommandError(str(e)) from None
+            raise RunCommandError(str(e)) from e
         return result
```

### Comparing `pyproject_installer-0.4.0/backend/config.py` & `pyproject_installer-0.5.0/backend/config.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/backend/metadata.py` & `pyproject_installer-0.5.0/backend/metadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/backend/sdist.py` & `pyproject_installer-0.5.0/backend/sdist.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/backend/wheel.py` & `pyproject_installer-0.5.0/backend/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/backend/_vendor/tomli/_parser.py` & `pyproject_installer-0.5.0/backend/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/backend/_vendor/tomli/_re.py` & `pyproject_installer-0.5.0/backend/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/tests/conftest.py` & `pyproject_installer-0.5.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,16 @@
     def __len__(self):
         return len(self._contents)
 
 
 @pytest.fixture
 def tmpdir(tmp_path):
     yield tmp_path
+    # Solaris: rmtree can't remove current working directory
+    assert Path.cwd() != tmp_path
     shutil.rmtree(tmp_path)
 
 
 @pytest.fixture
 def wheeldir(tmpdir):
     wheeldir = tmpdir / "dist"
     wheeldir.mkdir()
```

### Comparing `pyproject_installer-0.4.0/tests/integration/conftest.py` & `pyproject_installer-0.5.0/tests/integration/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 from pathlib import Path
 from venv import EnvBuilder
 import subprocess
 import sys
 import tempfile
 import textwrap
 
-try:
-    # Python 3.11+
-    import tomllib
-except ModuleNotFoundError:
-    import pyproject_installer.build_cmd._vendor.tomli as tomllib
-
 import pytest
 
 from pyproject_installer import __version__ as installer_version
 from pyproject_installer.build_cmd import WHEEL_TRACKER
-from pyproject_installer.build_cmd._build import call_hook
+from pyproject_installer.lib import tomllib
+from pyproject_installer.lib.build_backend import backend_hook
 
 
 class ContextVenv(EnvBuilder):
     def __init__(self, *args, **kwargs):
         self.context = None
         super().__init__(*args, **kwargs)
 
@@ -108,15 +103,15 @@
                     "install",
                     "-r",
                     f.name,
                 ]
                 subprocess.check_call(install_args)
 
         # get wheel build requirements(PEP517)
-        wheel_build_requires = call_hook(
+        wheel_build_requires = backend_hook(
             python=python,
             srcdir=srcdir,
             verbose=False,
             hook="get_requires_for_build_wheel",
         )["result"]
 
         if wheel_build_requires:
```

### Comparing `pyproject_installer-0.4.0/tests/integration/test_backends.py` & `pyproject_installer-0.5.0/tests/integration/test_backends.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/tests/integration/test_buildable.py` & `pyproject_installer-0.5.0/tests/integration/test_buildable.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/tests/integration/test_config_settings.py` & `pyproject_installer-0.5.0/tests/integration/test_config_settings.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/tests/unit/test_build/test_backend_caller.py` & `pyproject_installer-0.5.0/tests/unit/test_build/test_backend_caller.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 import json
 import textwrap
 import subprocess
 import sys
 
 import pytest
 
-from pyproject_installer.build_cmd.helper import backend_caller
+from pyproject_installer.lib.backend_helper import backend_caller
+
+
+BACKEND_CALLER_MOD = "pyproject_installer.lib.backend_helper.backend_caller"
 
 
 @pytest.fixture
 def project(tmpdir, monkeypatch):
     project_path = tmpdir / "project"
     project_path.mkdir()
     monkeypatch.chdir(project_path)
@@ -34,14 +37,19 @@
                 return "foo-1.0.tar.gz"
 
             def _get_requires_for_build_wheel(config_settings=None):
                 return ["build_wheel_dep"]
 
             def _get_requires_for_build_sdist(config_settings=None):
                 return ["build_sdist_dep"]
+
+            def _prepare_metadata_for_build_wheel(
+                metadata_directory, config_settings=None
+            ):
+                return "foo-1.0.dist-info"
             """
         )
         if hooks is None:
             hooks = list(backend_caller.SUPPORTED_HOOKS.keys())
 
         if be_object is None:
             for hook in hooks:
@@ -102,37 +110,26 @@
     path = "."
     yield path
     del sys.path_importer_cache[path]
 
 
 def test_help():
     result = subprocess.run(
-        args=[
-            sys.executable,
-            "-m",
-            "pyproject_installer.build_cmd.helper.backend_caller",
-            "--help",
-        ],
+        args=[sys.executable, "-m", BACKEND_CALLER_MOD, "--help"],
         capture_output=True,
     )
     assert result.returncode == 0
     assert result.stdout.rstrip().startswith(b"usage: backend_caller.py ")
     assert result.stderr == b""
 
 
 def test_invalid_hook_choice():
     invalid_hook = "invalid_hook_name"
     result = subprocess.run(
-        args=[
-            sys.executable,
-            "-m",
-            "pyproject_installer.build_cmd.helper.backend_caller",
-            "be",
-            invalid_hook,
-        ],
+        args=[sys.executable, "-m", BACKEND_CALLER_MOD, "be", invalid_hook],
         capture_output=True,
     )
     expected_err_msg = (
         "argument hook_name: invalid choice: '{}' (choose from {})\n"
     ).format(
         invalid_hook,
         ", ".join([f"{x!r}" for x in backend_caller.SUPPORTED_HOOKS]),
@@ -211,15 +208,15 @@
         ("info", "stdout"),
         ("debug", "stdout"),
     ),
 )
 def test_logging_destination(level, destination):
     code = textwrap.dedent(
         f"""\
-            from pyproject_installer.build_cmd.helper import backend_caller
+            import {BACKEND_CALLER_MOD} as backend_caller
 
             backend_caller.setup_logging(verbose=True)
             backend_caller.logger.{level}("{level}")
         """
     )
     cmd = [sys.executable, "-c", code]
     result = subprocess.run(args=cmd, capture_output=True)
@@ -449,14 +446,42 @@
     hook = "get_requires_for_build_sdist"
     hook_result = backend_caller.call_hook(
         be.name, backend_path=None, hook=hook, hook_args=[], hook_kwargs={}
     )
     assert hook_result == ["build_sdist_dep"]
 
 
+def test_missing_prepare_metadata_for_build_wheel(build_backend, wheeldir):
+    hook = "prepare_metadata_for_build_wheel"
+    hooks = list(backend_caller.SUPPORTED_HOOKS)
+    hooks.remove(hook)
+    be = build_backend("be", hooks=hooks)
+    hook_result = backend_caller.call_hook(
+        be.name,
+        backend_path=None,
+        hook=hook,
+        hook_args=[str(wheeldir)],
+        hook_kwargs={},
+    )
+    assert hook_result == ""
+
+
+def test_prepare_metadata_for_build_wheel(build_backend, wheeldir):
+    be = build_backend("be")
+    hook = "prepare_metadata_for_build_wheel"
+    hook_result = backend_caller.call_hook(
+        be.name,
+        backend_path=None,
+        hook=hook,
+        hook_args=[str(wheeldir)],
+        hook_kwargs={},
+    )
+    assert hook_result == "foo-1.0.dist-info"
+
+
 @pytest.mark.parametrize(
     "be_object", (("be",), ("be", "obj")), ids=["module", "module:object"]
 )
 def test_backend_object(be_object, build_backend, wheeldir):
     build_backend(*be_object)
     hook_result = backend_caller.call_hook(
         ":".join(be_object),
```

### Comparing `pyproject_installer-0.4.0/tests/unit/test_build/test_builder.py` & `pyproject_installer-0.5.0/tests/unit/test_build/test_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 from pyproject_installer.build_cmd import (
     build_wheel,
     build_sdist,
     WHEEL_TRACKER,
 )
 from pyproject_installer.build_cmd._build import (
-    BACKEND_CALLER,
     SUPPORTED_BUILD_HOOKS,
     build,
 )
+from pyproject_installer.lib.build_backend import BACKEND_CALLER
 
 
 def test_srcdir_nonexistent(wheeldir):
     with pytest.raises(
         ValueError,
         match="Unable to resolve path for source directory",
     ):
@@ -75,22 +75,21 @@
 def test_verbosity(mock_build, pyproject, build_args):
     """Check verbosity"""
     pyproject_path = pyproject()
     wheeldir = pyproject_path / "dist"
 
     verbose = build_args.get("verbose", False)
     capture = not verbose
+
     # emulate build error to see captured out/err
-    def _raise_process_error(*args, **kwargs):
-        stdout, stderr = (b"stdout", b"stderr") if capture else (None, None)
-        raise CalledProcessError(
-            1, ["command args"], output=stdout, stderr=stderr
-        )
+    stdout, stderr = (b"stdout", b"stderr") if capture else (None, None)
 
-    mock_build.side_effect = _raise_process_error
+    mock_build.side_effect = CalledProcessError(
+        1, ["command args"], output=stdout, stderr=stderr
+    )
 
     expected_err_msg = "build_wheel failed"
     if not verbose:
         expected_err_msg += (
             "\n\nCaptured stdout:\n\nstdout\n\nCaptured stderr:\n\nstderr"
         )
     with pytest.raises(RuntimeError) as e:
@@ -117,15 +116,15 @@
         "cwd": pyproject_path,
         "check": True,
         "pass_fds": (4,),
     }
     mock_build.assert_called_once_with(**b_kwargs)
 
 
-def test_paths_resolved(monkeypatch, mock_build, pyproject):
+def test_paths_resolved(mock_build, pyproject, monkeypatch):
     """Check if srcdir and wheeldir are resolved for backend"""
     pyproject_path = pyproject()
     cwd = pyproject_path.parent
     monkeypatch.chdir(cwd)
 
     wheeldir = cwd / "dist"
 
@@ -285,32 +284,30 @@
 
 def test_raisable_thread(mock_build, pyproject, mocker):
     """Check if build fails on raised thread"""
     pyproject_path = pyproject()
     outdir = pyproject_path / "dist"
 
     # override mock_build's mock for os.read
-    mock_os_read = mocker.patch("pyproject_installer.build_cmd._build.os.read")
-    # emulate os.read error to raise thread
-    def _raise_os_read(*args, **kwargs):
-        raise OSError("oops")
+    mock_os_read = mocker.patch("pyproject_installer.lib.build_backend.os.read")
 
-    mock_os_read.side_effect = _raise_os_read
+    # emulate os.read error to raise thread
+    mock_os_read.side_effect = OSError("oops")
 
     with pytest.raises(RuntimeError, match="oops"):
         build_wheel(pyproject_path, outdir=outdir)
 
 
 def test_received_invalid_data(mock_build, pyproject, mocker):
     """Check if build fails on invalid data"""
     pyproject_path = pyproject()
     outdir = pyproject_path / "dist"
 
     # override mock_build's mock for os.read
-    mock_os_read = mocker.patch("pyproject_installer.build_cmd._build.os.read")
+    mock_os_read = mocker.patch("pyproject_installer.lib.build_backend.os.read")
     mock_os_read.side_effect = [b"invalid_json", b""]
 
     with pytest.raises(
         RuntimeError,
         match="Received invalid JSON data from backend helper: 'invalid_json'",
     ):
         build_wheel(pyproject_path, outdir=outdir)
```

### Comparing `pyproject_installer-0.4.0/tests/unit/test_build/test_pyproject_parser.py` & `pyproject_installer-0.5.0/tests/unit/test_build/test_pyproject_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import textwrap
 import sys
 
 import pytest
 
 from pyproject_installer.build_cmd import build_wheel
-from pyproject_installer.build_cmd._build import BACKEND_CALLER
+from pyproject_installer.lib.build_backend import BACKEND_CALLER
 
 
 def test_pyproject_invalid_toml(pyproject, wheeldir):
     pyproject_path = pyproject("content\n")
 
     with pytest.raises(ValueError, match="Invalid pyproject.toml"):
         build_wheel(pyproject_path, outdir=wheeldir)
```

### Comparing `pyproject_installer-0.4.0/tests/unit/test_install/test_installer.py` & `pyproject_installer-0.5.0/tests/unit/test_install/test_installer.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/tests/unit/test_run/test_env.py` & `pyproject_installer-0.5.0/tests/unit/test_run/test_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import sys
 import textwrap
 
 import pytest
 
 from pyproject_installer.install_cmd import install_wheel
 from pyproject_installer.errors import RunCommandError, RunCommandEnvError
-from pyproject_installer.run_cmd import run_command, _run_env
+from pyproject_installer.run_cmd import run_command, _run_env, _run_command
 from pyproject_installer.lib.scripts import SCRIPT_TEMPLATE, build_shebang
 
 
 @pytest.fixture
 def project(tmpdir, monkeypatch):
     """Prepare everything needed to run a command in project root"""
     project_path = tmpdir / "project"
@@ -202,15 +202,16 @@
         venv_name=expected_name,
         command=cmd,
         capture_output=True,
     )
     assert res.stdout.strip().decode("utf-8") == expected_name
 
 
-def test_env_environ_path(project, wheel_no_csript):
+@pytest.mark.parametrize("env_path", ("path1", "path1:path2"))
+def test_env_environ_path(env_path, project, wheel_no_csript, monkeypatch):
     """Check venv's PATH environ variable"""
     code = textwrap.dedent(
         """\
         import os
         import json
         import sysconfig
 
@@ -221,17 +222,44 @@
                     "bin_dir": sysconfig.get_path("scripts"),
                 }
             )
         )
         """
     )
     cmd = ["python", "-c", code]
+    monkeypatch.setenv("PATH", env_path)
     res = run_command(wheel_no_csript(), command=cmd, capture_output=True)
     json_data = json.loads(res.stdout.decode("utf-8"))
-    assert json_data["env_path"].startswith(json_data["bin_dir"] + os.pathsep)
+    expected_path = os.pathsep.join([json_data["bin_dir"], env_path])
+    assert json_data["env_path"] == expected_path
+
+
+def test_env_environ_path_missing(project, wheel_no_csript, monkeypatch):
+    """Check venv's PATH environ variable if global's one is missing"""
+    code = textwrap.dedent(
+        """\
+        import os
+        import json
+        import sysconfig
+
+        print(
+            json.dumps(
+                {
+                    "env_path": os.environ["PATH"],
+                    "bin_dir": sysconfig.get_path("scripts"),
+                }
+            )
+        )
+        """
+    )
+    cmd = ["python", "-c", code]
+    monkeypatch.delenv("PATH")
+    res = run_command(wheel_no_csript(), command=cmd, capture_output=True)
+    json_data = json.loads(res.stdout.decode("utf-8"))
+    assert json_data["env_path"] == json_data["bin_dir"]
 
 
 def test_env_environ_virtual_env(project, wheel_no_csript):
     """Check venv's VIRTUAL_ENV environ variable"""
     code = textwrap.dedent(
         """\
         import os
@@ -262,14 +290,36 @@
             "nonexistent-1.0-py3-none-any.whl",
             command=command,
             capture_output=True,
         )
     assert "Installation of package failed" in str(exc.value)
 
 
+@pytest.mark.parametrize(
+    "error",
+    (RunCommandEnvError, RunCommandError, Exception),
+)
+def test_env_venv_creation_error(error, project, wheel_no_csript, mocker):
+    """Check the error on failed creation of venv"""
+    err_msg = "some error"
+    mocker.patch.object(
+        _run_command.PyprojectVenv,
+        "create",
+        autospec=True,
+        side_effect=error(err_msg),
+    )
+    command = ["any_command"]
+    with pytest.raises(RunCommandEnvError, match=err_msg):
+        run_command(
+            wheel_no_csript(),
+            command=command,
+            capture_output=True,
+        )
+
+
 def test_env_command_nonexistent(project, wheel_no_csript, monkeypatch):
     """Check the error on nonexistent command"""
     # required for error message
     monkeypatch.setenv("LC_ALL", "C.utf8")
     command = ["nonexistent_cmd"]
     with pytest.raises(RunCommandError) as exc:
         run_command(wheel_no_csript(), command=command, capture_output=True)
```

### Comparing `pyproject_installer-0.4.0/pyproject.toml` & `pyproject_installer-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.4.0/LICENSE` & `pyproject_installer-0.5.0/LICENSE`

 * *Files identical despite different names*

