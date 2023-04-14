# Comparing `tmp/npe2-0.6.2.tar.gz` & `tmp/npe2-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npe2-0.6.2.tar", last modified: Thu Jan 12 23:59:30 2023, max compression
+gzip compressed data, was "npe2-0.7.0.tar", last modified: Fri Apr 14 13:05:40 2023, max compression
```

## Comparing `npe2-0.6.2.tar` & `npe2-0.7.0.tar`

### file list

```diff
@@ -1,141 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.097723 npe2-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.073722 npe2-0.6.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-12 23:59:08.000000 npe2-0.6.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-12 23:59:08.000000 npe2-0.6.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.073722 npe2-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-01-12 23:59:08.000000 npe2-0.6.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-01-12 23:59:08.000000 npe2-0.6.2/.github/workflows/test_all_plugins.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-01-12 23:59:08.000000 npe2-0.6.2/.github/workflows/test_conversion.yml
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-01-12 23:59:08.000000 npe2-0.6.2/.github/workflows/update_changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-01-12 23:59:08.000000 npe2-0.6.2/.github_changelog_generator
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-01-12 23:59:08.000000 npe2-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-01-12 23:59:08.000000 npe2-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23717 2023-01-12 23:59:08.000000 npe2-0.6.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-01-12 23:59:08.000000 npe2-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-01-12 23:59:08.000000 npe2-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-01-12 23:59:08.000000 npe2-0.6.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-01-12 23:59:30.097723 npe2-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-01-12 23:59:08.000000 npe2-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.073722 npe2-0.6.2/_docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-01-12 23:59:08.000000 npe2-0.6.2/_docs/example_manifest.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.073722 npe2-0.6.2/_docs/example_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:08.000000 npe2-0.6.2/_docs/example_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-01-12 23:59:08.000000 npe2-0.6.2/_docs/example_plugin/some_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-01-12 23:59:08.000000 npe2-0.6.2/_docs/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.077723 npe2-0.6.2/_docs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-01-12 23:59:08.000000 npe2-0.6.2/_docs/templates/_npe2_contributions.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-01-12 23:59:08.000000 npe2-0.6.2/_docs/templates/_npe2_manifest.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-01-12 23:59:08.000000 npe2-0.6.2/_docs/templates/_npe2_readers_guide.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-01-12 23:59:08.000000 npe2-0.6.2/_docs/templates/_npe2_sample_data_guide.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-01-12 23:59:08.000000 npe2-0.6.2/_docs/templates/_npe2_widgets_guide.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-01-12 23:59:08.000000 npe2-0.6.2/_docs/templates/_npe2_writers_guide.md.jinja
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-12 23:59:08.000000 npe2-0.6.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.077723 npe2-0.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-01-12 23:59:08.000000 npe2-0.6.2/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-12 23:59:08.000000 npe2-0.6.2/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-12 23:59:08.000000 npe2-0.6.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-12 23:59:08.000000 npe2-0.6.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.081723 npe2-0.6.2/npe2/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/_command_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/_dynamic_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.081723 npe2-0.6.2/npe2/_inspection/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/_inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/_inspection/_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/_inspection/_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    23193 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/_inspection/_from_npe1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/_inspection/_full_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/_inspection/_setuputils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19666 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/_inspection/_visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)    28353 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/_plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/_setuptools_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-12 23:59:29.000000 npe2-0.6.2/npe2/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16072 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/implements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/implements.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/io_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.085723 npe2-0.6.2/npe2/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/_bases.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/_npe1_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/_package_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.085723 npe2-0.6.2/npe2/manifest/contributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/_contributions.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/_icon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/_json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/_keybindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/_menus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/_submenu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/_themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/contributions/_writers.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/menus.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/package_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/manifest/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-01-12 23:59:08.000000 npe2-0.6.2/npe2/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.081723 npe2-0.6.2/npe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-01-12 23:59:30.000000 npe2-0.6.2/npe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-01-12 23:59:30.000000 npe2-0.6.2/npe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 23:59:30.000000 npe2-0.6.2/npe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-12 23:59:30.000000 npe2-0.6.2/npe2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 23:59:30.000000 npe2-0.6.2/npe2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-12 23:59:30.000000 npe2-0.6.2/npe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-12 23:59:30.000000 npe2-0.6.2/npe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-12 23:59:08.000000 npe2-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-01-12 23:59:30.097723 npe2-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.093723 npe2-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.069723 npe2-0.6.2/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.093723 npe2-0.6.2/tests/fixtures/my-compiled-plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.093723 npe2-0.6.2/tests/fixtures/my-compiled-plugin/my_module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/fixtures/my-compiled-plugin/my_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/fixtures/my-compiled-plugin/my_module/_a.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/fixtures/my-compiled-plugin/my_module/_b.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/fixtures/my-compiled-plugin/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.097723 npe2-0.6.2/tests/npe1-plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.097723 npe2-0.6.2/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/METADATA
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.097723 npe2-0.6.2/tests/npe1-plugin/npe1_module/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/npe1-plugin/npe1_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/npe1-plugin/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.097723 npe2-0.6.2/tests/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/sample/_with_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.097723 npe2-0.6.2/tests/sample/my_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/sample/my_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/sample/my_plugin/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:59:30.097723 npe2-0.6.2/tests/sample/my_plugin-1.2.3.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/sample/my_plugin-1.2.3.dist-info/METADATA
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/sample/my_plugin-1.2.3.dist-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/sample/my_plugin-1.2.3.dist-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test__io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_all_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_config_contribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_contributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_implements.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_npe1_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_package_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_pm_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_setuptools_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_tmp_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-01-12 23:59:08.000000 npe2-0.6.2/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.288337 npe2-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.272337 npe2-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-14 13:05:24.000000 npe2-0.7.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-14 13:05:24.000000 npe2-0.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.272337 npe2-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-14 13:05:24.000000 npe2-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-14 13:05:24.000000 npe2-0.7.0/.github/workflows/test_all_plugins.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-14 13:05:24.000000 npe2-0.7.0/.github/workflows/test_conversion.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-14 13:05:24.000000 npe2-0.7.0/.github/workflows/update_changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-14 13:05:24.000000 npe2-0.7.0/.github_changelog_generator
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-14 13:05:24.000000 npe2-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-14 13:05:24.000000 npe2-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    25594 2023-04-14 13:05:24.000000 npe2-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-14 13:05:24.000000 npe2-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 13:05:24.000000 npe2-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-14 13:05:24.000000 npe2-0.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-14 13:05:40.288337 npe2-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-14 13:05:24.000000 npe2-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-14 13:05:24.000000 npe2-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 13:05:40.288337 npe2-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.272337 npe2-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.276337 npe2-0.7.0/src/npe2/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_command_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_dynamic_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.276337 npe2-0.7.0/src/npe2/_inspection/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23320 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/_from_npe1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/_full_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/_setuputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19618 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28433 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_setuptools_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/implements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/implements.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/io_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.280337 npe2-0.7.0/src/npe2/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/_bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/_npe1_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/_package_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.280337 npe2-0.7.0/src/npe2/manifest/contributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_keybindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_menus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_submenu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/menus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/package_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20080 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.276337 npe2-0.7.0/src/npe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.284337 npe2-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.272337 npe2-0.7.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.284337 npe2-0.7.0/tests/fixtures/my-compiled-plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.284337 npe2-0.7.0/tests/fixtures/my-compiled-plugin/my_module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/fixtures/my-compiled-plugin/my_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/fixtures/my-compiled-plugin/my_module/_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/fixtures/my-compiled-plugin/my_module/_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/fixtures/my-compiled-plugin/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.284337 npe2-0.7.0/tests/npe1-plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.284337 npe2-0.7.0/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/METADATA
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.284337 npe2-0.7.0/tests/npe1-plugin/npe1_module/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/npe1-plugin/npe1_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/npe1-plugin/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.288337 npe2-0.7.0/tests/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/sample/_with_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.288337 npe2-0.7.0/tests/sample/my_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/sample/my_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/sample/my_plugin/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.288337 npe2-0.7.0/tests/sample/my_plugin-1.2.3.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/sample/my_plugin-1.2.3.dist-info/METADATA
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/sample/my_plugin-1.2.3.dist-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/sample/my_plugin-1.2.3.dist-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test__io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_all_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_config_contribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_implements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_npe1_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_package_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_pm_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_setuptools_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_tmp_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_validations.py
```

### Comparing `npe2-0.6.2/.github/workflows/ci.yml` & `npe2-0.7.0/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,22 @@
       - main
     tags:
       - "v*"
   pull_request: {}
   workflow_dispatch:
 
 jobs:
+  check-manifest:
+    name: Check Manifest
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - name: Check
+        run: pipx run check-manifest
+
   test:
     name: ${{ matrix.platform }} (${{ matrix.python-version }})
     runs-on: ${{ matrix.platform }}
     strategy:
       fail-fast: false
       matrix:
         python-version: [3.8, 3.9, "3.10"]
```

### Comparing `npe2-0.6.2/.github/workflows/test_all_plugins.yml` & `npe2-0.7.0/.github/workflows/test_all_plugins.yml`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/.github/workflows/test_conversion.yml` & `npe2-0.7.0/.github/workflows/test_conversion.yml`

 * *Files 4% similar despite different names*

```diff
@@ -56,33 +56,33 @@
           fetch-depth: 0
 
       - name: Install ${{ matrix.plugin }}
         run: pip install -e ./plugin_repo
 
       - name: Test Conversion
         id: test-without-napari
-        uses: GabrielBB/xvfb-action@v1
+        uses: aganders3/headless-gui@v1
         continue-on-error: true
         with:
           run: npe2 convert ./plugin_repo
 
       - name: Install napari
         if: ${{ steps.test-without-napari.outcome == 'failure' }}
         run: pip install napari
 
       - name: Test Conversion again with napari
         id: test-with-napari
         if: ${{ steps.test-without-napari.outcome == 'failure' }}
-        uses: GabrielBB/xvfb-action@v1
+        uses: aganders3/headless-gui@v1
         with:
           run: npe2 convert ./plugin_repo
 
       - name: Test Conversion again with napari
         if: ${{ steps.test-without-napari.outcome == 'failure' && steps.test-with-napari.outcome == 'failure' }}
-        uses: GabrielBB/xvfb-action@v1
+        uses: aganders3/headless-gui@v1
         with:
           # try without modifying directory
           run: npe2 convert -n ${{ matrix.plugin }}
 
       # this won't work, we'd need to first fork the repo somewhere we have write permissions
       # then push changes that that repository, and then create a PR to the original repo
       # - name: Create Pull Request
```

### Comparing `npe2-0.6.2/.github/workflows/update_changelog.yml` & `npe2-0.7.0/.github/workflows/update_changelog.yml`

 * *Files 0% similar despite different names*

```diff
@@ -15,13 +15,13 @@
       - name: "✏️ Generate release changelog"
         uses: heinrichreimer/github-changelog-generator-action@v2.3
         with:
           futureRelease: ${{ github.event.inputs.next_tag }}
           token: ${{ secrets.GITHUB_TOKEN }}
           repo: napari/npe2
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@v4
+        uses: peter-evans/create-pull-request@v5
         with:
           token: ${{ secrets.GITHUB_TOKEN }}
           commit-message: Automatic changelog update
           title: changelog ${{ github.event.inputs.next_tag }}
           branch: update-changelog
```

### Comparing `npe2-0.6.2/.github_changelog_generator` & `npe2-0.7.0/.github_changelog_generator`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/.gitignore` & `npe2-0.7.0/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -99,12 +99,12 @@
 /site
 
 # mypy
 .mypy_cache/
 
 # IDE settings
 .vscode/
-npe2/_version.py
+src/npe2/_version.py
 
 # ignore everything that gets rendered from _docs
 docs/plugins/*.md
 schema.json
```

### Comparing `npe2-0.6.2/.pre-commit-config.yaml` & `npe2-0.7.0/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -3,45 +3,31 @@
   autofix_commit_msg: "style: [pre-commit.ci] auto fixes [...]"
   autoupdate_commit_msg: "ci: [pre-commit.ci] autoupdate"
 
 exclude: _docs/example_plugin/some_module.py
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
       - id: trailing-whitespace
-  - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.4
-    hooks:
-      - id: flake8
-        additional_dependencies:
-        - flake8-typing-imports
-        - flake8-bugbear
-  - repo: https://github.com/PyCQA/autoflake
-    rev: v1.7.7
-    hooks:
-      - id: autoflake
-        args: ["--in-place", "--remove-all-unused-imports"]
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
+
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.2.0
+
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: v0.0.261
     hooks:
-      - id: pyupgrade
-        args: [--py38-plus, --keep-runtime-typing]
+      - id: ruff
+
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.982
+    rev: v1.1.1
     hooks:
       - id: mypy
         additional_dependencies:
           - types-toml
           - types-PyYAML
-        exclude: npe2/implements.pyi
+        exclude: npe2/implements.pyi|_docs/render.py
```

### Comparing `npe2-0.6.2/CHANGELOG.md` & `npe2-0.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,38 @@
 # Changelog
 
+## [v0.7.0](https://github.com/napari/npe2/tree/v0.7.0) (2023-04-14)
+
+[Full Changelog](https://github.com/napari/npe2/compare/v0.6.2...v0.7.0)
+
+**Fixed bugs:**
+
+- fix: pass command registry to rdr.exec in io\_utils.\_read [\#285](https://github.com/napari/npe2/pull/285) ([tlambert03](https://github.com/tlambert03))
+- fix: use logger instead of warning for TestPluginManager.discover [\#283](https://github.com/napari/npe2/pull/283) ([tlambert03](https://github.com/tlambert03))
+- Add specific error when reader plugin was chosen but failed [\#276](https://github.com/napari/npe2/pull/276) ([DragaDoncila](https://github.com/DragaDoncila))
+
+**Tests & CI:**
+
+- Fix tests: use npe1 version \(0.1.2\) of napari-ndtiffs [\#277](https://github.com/napari/npe2/pull/277) ([psobolewskiPhD](https://github.com/psobolewskiPhD))
+- ci: update pre-commit, use ruff and fix mypy [\#273](https://github.com/napari/npe2/pull/273) ([tlambert03](https://github.com/tlambert03))
+- Switch from GabrielBB/xvfb-action to aganders3/headless-gui [\#269](https://github.com/napari/npe2/pull/269) ([Czaki](https://github.com/Czaki))
+
+**Refactors:**
+
+- refactor: use src layout and pyproject.toml [\#281](https://github.com/napari/npe2/pull/281) ([tlambert03](https://github.com/tlambert03))
+
+**Documentation:**
+
+- Fix link to magicgui objects.inv in intersphinx [\#270](https://github.com/napari/npe2/pull/270) ([melissawm](https://github.com/melissawm))
+
+**Merged pull requests:**
+
+- ci\(dependabot\): bump peter-evans/create-pull-request from 4 to 5 [\#284](https://github.com/napari/npe2/pull/284) ([dependabot[bot]](https://github.com/apps/dependabot))
+- Pin pydantic bellow 2.0 [\#279](https://github.com/napari/npe2/pull/279) ([Czaki](https://github.com/Czaki))
+
 ## [v0.6.2](https://github.com/napari/npe2/tree/v0.6.2) (2023-01-12)
 
 [Full Changelog](https://github.com/napari/npe2/compare/v0.6.1...v0.6.2)
 
 **Implemented enhancements:**
 
 - Expose `syntax_style` [\#261](https://github.com/napari/npe2/pull/261) ([brisvag](https://github.com/brisvag))
@@ -28,14 +57,15 @@
 **Documentation:**
 
 - Move to sphinx-design tabs [\#259](https://github.com/napari/npe2/pull/259) ([melissawm](https://github.com/melissawm))
 - Fix a few broken links [\#258](https://github.com/napari/npe2/pull/258) ([melissawm](https://github.com/melissawm))
 
 **Merged pull requests:**
 
+- changelog v0.6.2 [\#268](https://github.com/napari/npe2/pull/268) ([github-actions[bot]](https://github.com/apps/github-actions))
 - ci\(dependabot\): bump styfle/cancel-workflow-action from 0.10.1 to 0.11.0 [\#252](https://github.com/napari/npe2/pull/252) ([dependabot[bot]](https://github.com/apps/dependabot))
 - ci\(dependabot\): bump styfle/cancel-workflow-action from 0.10.0 to 0.10.1 [\#246](https://github.com/napari/npe2/pull/246) ([dependabot[bot]](https://github.com/apps/dependabot))
 - Add setuptools plugin to compile manifest at build [\#194](https://github.com/napari/npe2/pull/194) ([tlambert03](https://github.com/tlambert03))
 
 ## [v0.6.1](https://github.com/napari/npe2/tree/v0.6.1) (2022-08-08)
 
 [Full Changelog](https://github.com/napari/npe2/compare/v0.6.0...v0.6.1)
@@ -153,15 +183,15 @@
 
 **Fixed bugs:**
 
 - hide docs again in napari menus \(Fix napari docs build\) [\#178](https://github.com/napari/npe2/pull/178) ([tlambert03](https://github.com/tlambert03))
 
 ## [v0.4.0](https://github.com/napari/npe2/tree/v0.4.0) (2022-06-13)
 
-[Full Changelog](https://github.com/napari/npe2/compare/v0.3.0.rc0...v0.4.0)
+[Full Changelog](https://github.com/napari/npe2/compare/v0.3.0...v0.4.0)
 
 **Implemented enhancements:**
 
 - Turn menus contributions into dict of arbitrary key to list of MenuItems [\#175](https://github.com/napari/npe2/pull/175) ([tlambert03](https://github.com/tlambert03))
 - Add minor conveniences for DynamicPlugin [\#173](https://github.com/napari/npe2/pull/173) ([tlambert03](https://github.com/tlambert03))
 - Add `plugin_manager` module for global singleton convenience  [\#164](https://github.com/napari/npe2/pull/164) ([tlambert03](https://github.com/tlambert03))
 - Allow arbitrary menu locations in npe2 [\#160](https://github.com/napari/npe2/pull/160) ([sofroniewn](https://github.com/sofroniewn))
@@ -183,21 +213,21 @@
 - Push stack=... through all the reader internal API, take II [\#142](https://github.com/napari/npe2/pull/142) ([Carreau](https://github.com/Carreau))
 
 **Documentation:**
 
 - Add doc links to README [\#158](https://github.com/napari/npe2/pull/158) ([nclack](https://github.com/nclack))
 - Fix codeblock directive in docstring [\#156](https://github.com/napari/npe2/pull/156) ([melissawm](https://github.com/melissawm))
 
-## [v0.3.0.rc0](https://github.com/napari/npe2/tree/v0.3.0.rc0) (2022-04-05)
+## [v0.3.0](https://github.com/napari/npe2/tree/v0.3.0) (2022-04-05)
 
-[Full Changelog](https://github.com/napari/npe2/compare/v0.3.0...v0.3.0.rc0)
+[Full Changelog](https://github.com/napari/npe2/compare/v0.3.0.rc0...v0.3.0)
 
-## [v0.3.0](https://github.com/napari/npe2/tree/v0.3.0) (2022-04-05)
+## [v0.3.0.rc0](https://github.com/napari/npe2/tree/v0.3.0.rc0) (2022-04-05)
 
-[Full Changelog](https://github.com/napari/npe2/compare/v0.2.2...v0.3.0)
+[Full Changelog](https://github.com/napari/npe2/compare/v0.2.2...v0.3.0.rc0)
 
 **Implemented enhancements:**
 
 - NPE1Adapter Part 3 - caching of adapter manifests [\#126](https://github.com/napari/npe2/pull/126) ([tlambert03](https://github.com/tlambert03))
 - NPE1Adapter Part 2 - adding the NPE1Adapter object. [\#125](https://github.com/napari/npe2/pull/125) ([tlambert03](https://github.com/tlambert03))
 - NPE1Adapter Part 1 - updated \_from\_npe1 conversion logic to prepare for locally defined objects [\#124](https://github.com/napari/npe2/pull/124) ([tlambert03](https://github.com/tlambert03))
```

### Comparing `npe2-0.6.2/LICENSE` & `npe2-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/Makefile` & `npe2-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/PKG-INFO` & `npe2-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: npe2
-Version: 0.6.2
-Summary: proposal for napari plugin refactor
-Home-page: https://github.com/napari/npe2
-Author: Talley Lambert, Nathan Clack
-Author-email: talley.lambert@gmail.com
+Version: 0.7.0
+Summary: napari plugin engine v2
+Author: Nathan Clack
+Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD-3-Clause
-Project-URL: Source Code, https://github.com/napari/npe2
+Project-URL: homepage, https://github.com/napari/npe2
+Project-URL: repository, https://github.com/napari/npe2
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: json
-Provides-Extra: testing
 License-File: LICENSE
 
 # npe2
 
 [![CI](https://github.com/napari/npe2/actions/workflows/ci.yml/badge.svg)](https://github.com/napari/npe2/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/napari/npe2/branch/main/graph/badge.svg?token=FTH635x542)](https://codecov.io/gh/napari/npe2)
```

### Comparing `npe2-0.6.2/README.md` & `npe2-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/npe2/__init__.py` & `npe2-0.7.0/src/npe2/__init__.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/npe2/_command_registry.py` & `npe2-0.7.0/src/npe2/_command_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# flake8: noqa
 from __future__ import annotations
 
 from dataclasses import dataclass
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Union
 
 from psygnal import Signal
```

### Comparing `npe2-0.6.2/npe2/_dynamic_plugin.py` & `npe2-0.7.0/src/npe2/_dynamic_plugin.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/npe2/_inspection/_compile.py` & `npe2-0.7.0/src/npe2/_inspection/_compile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
 from typing import Iterator, List, Sequence, Tuple, Union, cast
 
-from ..manifest import PluginManifest, contributions
-from ..manifest.utils import merge_contributions, merge_manifests
+from npe2.manifest import PluginManifest, contributions
+from npe2.manifest.utils import merge_contributions, merge_manifests
+
 from ._setuputils import get_package_dir_info
 from ._visitors import find_npe2_module_contributions
 
 
 def find_packages(where: Union[str, Path] = ".") -> List[Path]:
     """Return all folders that have an __init__.py file"""
     return [p.parent for p in Path(where).resolve().rglob("**/__init__.py")]
```

### Comparing `npe2-0.6.2/npe2/_inspection/_fetch.py` & `npe2-0.7.0/src/npe2/_inspection/_fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,16 +72,16 @@
     mf.package_metadata = PackageMetadata.from_dist_metadata(dist.metadata)
     return mf
 
 
 def _manifest_from_npe1_dist(dist: metadata.PathDistribution) -> PluginManifest:
     """Extract plugin manifest from a distribution with an npe1 entry point."""
     from npe2.manifest import PluginManifest
+    from npe2.manifest.utils import merge_contributions
 
-    from ..manifest.utils import merge_contributions
     from . import find_npe1_module_contributions
 
     name = dist.metadata["Name"]
     contribs = []
     for ep in dist.entry_points:
         if ep.group == NPE1_ENTRY_POINT and (match := ep.pattern.match(ep.value)):
             module = match.group("module")
@@ -171,26 +171,26 @@
 
 
 def _get_manifest_from_wheel_url(url: str) -> PluginManifest:
     """Extract a manifest from a remote wheel file.
 
     Examples
     --------
-    $ npe2 fetch https://files.pythonhosted.org/packages/b0/93/a00a1ee154d5ce3540dd5ae081dc53fcfa7498f34ba68a7345ac027a4f96/pycudadecon-0.3.0-py3-none-any.whl  # noqa
+    $ npe2 fetch https://files.pythonhosted.org/packages/b0/93/a00a1ee154d5ce3540dd5ae081dc53fcfa7498f34ba68a7345ac027a4f96/pycudadecon-0.3.0-py3-none-any.whl
     """
     with _tmp_zip_download(url) as wheel_dir:
         return _manifest_from_extracted_wheel(wheel_dir)
 
 
 def _get_manifest_from_targz_url(url: str) -> PluginManifest:
     """Extract a manifest from a remote source directory tar.gz file.
 
     Examples
     --------
-    $ npe2 fetch https://files.pythonhosted.org/packages/4a/84/de031ba465f183c319cb37633c49dfebd57f1ff42bc9744db3f80f7f4093/pycudadecon-0.3.0.tar.gz  # noqa
+    $ npe2 fetch https://files.pythonhosted.org/packages/4a/84/de031ba465f183c319cb37633c49dfebd57f1ff42bc9744db3f80f7f4093/pycudadecon-0.3.0.tar.gz
     """
     with _tmp_targz_download(url) as targz_path:
         src_dir = next(Path(targz_path).iterdir())  # find first directory
         return _build_src_and_extract_manifest(src_dir)
 
 
 def _get_manifest_from_git_url(url: str) -> PluginManifest:
@@ -230,15 +230,15 @@
     Examples
     --------
     >>> fetch_manifest("napari-dv")
     >>> fetch_manifest("napari-dv", "0.3.0")
     >>> fetch_manifest("https://github.com/tlambert03/napari-dv")
     >>> fetch_manifest("git+https://github.com/tlambert03/napari-dv.git")
     >>> fetch_manifest("https://github.com/org/project/archive/refs/heads/master.zip")
-    >>> fetch_manifest("https://files.pythonhosted.org/.../package-0.3.0-py3-none-any.whl")  # noqa
+    >>> fetch_manifest("https://files.pythonhosted.org/.../package-0.3.0-py3-none-any.whl")
     >>> fetch_manifest("https://files.pythonhosted.org/.../package-0.3.0.tar.gz")
     """
     # not on PyPI check various URL forms
     if package_or_url.startswith(("http", "git+http")):
         if package_or_url.endswith(".zip"):
             return _get_manifest_from_zip_url(package_or_url)
         if package_or_url.endswith(".whl"):
```

### Comparing `npe2-0.6.2/npe2/_inspection/_from_npe1.py` & `npe2-0.7.0/src/npe2/_inspection/_from_npe1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 import inspect
 import re
 import sys
 import warnings
 from configparser import ConfigParser
-from functools import lru_cache
+from functools import lru_cache, partial
 from importlib import import_module, metadata
 from logging import getLogger
 from pathlib import Path
 from types import ModuleType
 from typing import (
     Any,
     Callable,
@@ -96,15 +96,15 @@
         )
 
     return packages
 
 
 def manifest_from_npe1(
     plugin: Union[str, metadata.Distribution, None] = None,
-    module: Any = None,
+    module: Optional[Any] = None,
     adapter=False,
 ) -> PluginManifest:
     """Return manifest object given npe1 plugin or package name.
 
     One of `plugin` or `module` must be provide.
 
     Parameters
@@ -122,15 +122,14 @@
         python_names that are not supported natively by npe2. by default False
     """
     if module is not None:
         modules: List[str] = [module]
         package_name = "dynamic"
         plugin_name = getattr(module, "__name__", "dynamic_plugin")
     elif isinstance(plugin, str):
-
         modules = []
         plugin_name = plugin
         for pp in plugin_packages():
             if plugin in (pp.ep_name, pp.package_name):
                 modules.append(pp.ep_value)
                 package_name = pp.package_name
         if not modules:
@@ -203,15 +202,16 @@
         for impl in iter_hookimpls(module, plugin_name=self.plugin_name):
             if impl.plugin_name == self.plugin_name:
                 # call the corresponding hookimpl parser
                 try:
                     getattr(self, impl.specname)(impl)
                 except Exception as e:  # pragma: no cover
                     warnings.warn(
-                        f"Failed to convert {impl.specname} in {self.package!r}: {e}"
+                        f"Failed to convert {impl.specname} in {self.package!r}: {e}",
+                        stacklevel=2,
                     )
 
     def napari_experimental_provide_theme(self, impl: HookImplementation):
         ThemeDict = Dict[str, Union[str, Tuple, List]]
         d: Dict[str, ThemeDict] = impl.function()
         for name, theme_dict in d.items():
             colors = ThemeColors(**theme_dict)
@@ -223,15 +223,14 @@
                     "id": name.lower().replace(" ", "_"),
                     "type": "dark" if luma < 128 else "light",
                     "colors": colors,
                 }
             )
 
     def napari_get_reader(self, impl: HookImplementation):
-
         patterns = _guess_fname_patterns(impl.function)
 
         self.contributions["readers"].append(
             {
                 "command": self.add_command(impl),
                 "accepts_directories": True,
                 "filename_patterns": patterns,
@@ -275,15 +274,14 @@
 
     def napari_experimental_provide_function(self, impl: HookImplementation):
         items: Union[Callable, List[Callable]] = impl.function()
         items = [items] if not isinstance(items, list) else items
 
         for idx, item in enumerate(items):
             try:
-
                 cmd = f"{self.package}.{item.__name__}"
                 py_name = _python_name(
                     item, impl.function, hook_idx=idx if self.adapter else None
                 )
                 docsum = item.__doc__.splitlines()[0] if item.__doc__ else None
                 cmd_contrib = CommandContribution(
                     id=cmd, python_name=py_name, title=docsum or item.__name__
@@ -298,15 +296,15 @@
                 self.contributions["widgets"].append(wdg_contrib)
 
             except Exception as e:  # pragma: no cover
                 msg = (
                     f"Error converting function [{idx}] "
                     f"from {impl.function.__module__!r}:\n{e}"
                 )
-                warnings.warn(msg)
+                warnings.warn(msg, stacklevel=2)
 
     def napari_experimental_provide_dock_widget(self, impl: HookImplementation):
         WidgetCallable = Union[Callable, Tuple[Callable, dict]]
         items: Union[WidgetCallable, List[WidgetCallable]] = impl.function()
         if not isinstance(items, list):
             items = [items]  # pragma: no cover
 
@@ -317,29 +315,31 @@
                 wdg_creator = item[0]
                 kwargs = item[1] if len(item) > 1 else {}
             else:
                 wdg_creator, kwargs = (item, {})
             if not callable(wdg_creator) and isinstance(
                 kwargs, dict
             ):  # pragma: no cover
-                warnings.warn(f"Invalid widget spec: {wdg_creator}, {kwargs}")
+                warnings.warn(
+                    f"Invalid widget spec: {wdg_creator}, {kwargs}", stacklevel=2
+                )
                 continue
 
             try:
                 func_name = getattr(wdg_creator, "__name__", "")
                 wdg_name = str(kwargs.get("name", "")) or _camel_to_spaces(func_name)
                 self._create_widget_contrib(
                     wdg_creator, display_name=wdg_name, idx=idx, hook=impl.function
                 )
             except Exception as e:  # pragma: no cover
                 msg = (
                     f"Error converting dock widget [{idx}] "
                     f"from {impl.function.__module__!r}:\n{e}"
                 )
-                warnings.warn(msg)
+                warnings.warn(msg, stacklevel=2)
 
     def _create_widget_contrib(
         self,
         wdg_creator: WidgetCreator,
         display_name: str,
         idx: int,
         hook: Callable,
@@ -368,15 +368,16 @@
         wdg_contrib = WidgetContribution(command=cmd, display_name=display_name)
         self.contributions["commands"].append(cmd_contrib)
         self.contributions["widgets"].append(wdg_contrib)
 
     def napari_get_writer(self, impl: HookImplementation):
         warnings.warn(
             f"Found a multi-layer writer in {self.package!r} - {impl.specname!r}, "
-            "but it's not convertable. Please add the writer manually."
+            "but it's not convertable. Please add the writer manually.",
+            stacklevel=2,
         )
         return NotImplemented  # pragma: no cover
 
     def napari_write_image(self, impl: HookImplementation):
         self._parse_writer(impl, "image")
 
     def napari_write_labels(self, impl: HookImplementation):
@@ -410,23 +411,19 @@
             py_name = _python_name(impl.function)
         c = CommandContribution(id=id, python_name=py_name, title=title)
         self.contributions["commands"].append(c)
         return id
 
 
 def _is_magicgui_magic_factory(obj):
-    try:
-        import magicgui
-    except ImportError:
-        return False
-    return isinstance(obj, magicgui._magicgui.MagicFactory)
+    return "magicgui" in sys.modules and isinstance(obj, partial)
 
 
 def _python_name(
-    obj: Any, hook: Callable = None, hook_idx: Optional[int] = None
+    obj: Any, hook: Optional[Callable] = None, hook_idx: Optional[int] = None
 ) -> str:
     """Get resolvable python name for `obj` returned from an npe1 `hook` implentation.
 
     Parameters
     ----------
     obj : Any
         a python obj
@@ -562,15 +559,16 @@
             f"""
        entry_points={{
            "{NPE2_EP}": [
                "{info.package_name} = {info.top_module}:{mf_name}",
            ],
        }},
        package_data={{"{info.top_module}": ["{mf_name}"]}},
-"""
+""",
+            stacklevel=2,
         )
 
     # write the yaml to top_module/napari.yaml
     mf_path.write_text(manifest.yaml())
     return manifest, mf_path
```

### Comparing `npe2-0.6.2/npe2/_inspection/_full_install.py` & `npe2-0.7.0/src/npe2/_inspection/_full_install.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/npe2/_inspection/_setuputils.py` & `npe2-0.7.0/src/npe2/_inspection/_setuputils.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,9 +135,9 @@
             return dict(zip(keys, values))
         if isinstance(node, ast.List):
             return [self._get_val(k) for k in node.elts]
         if isinstance(node, ast.Tuple):  # pragma: no cover
             return tuple(self._get_val(k) for k in node.elts)
         return str(node)  # pragma: no cover
 
-    def get(self, key: str, default: Any = None) -> Any:
+    def get(self, key: str, default: Optional[Any] = None) -> Any:
         return self._setup_kwargs.get(key, default)
```

### Comparing `npe2-0.6.2/npe2/_inspection/_visitors.py` & `npe2-0.7.0/src/npe2/_inspection/_visitors.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import inspect
 from abc import ABC, abstractmethod
 from importlib.metadata import Distribution
 from pathlib import Path
 from types import ModuleType
 from typing import TYPE_CHECKING, Any, DefaultDict, Dict, List, Tuple, Type, Union
 
-from ..manifest import contributions
+from npe2.manifest import contributions
 
 if TYPE_CHECKING:
     from pydantic import BaseModel
 
 
 CONTRIB_MAP: Dict[str, Tuple[Type["BaseModel"], str]] = {
     "writer": (contributions.WriterContribution, "writers"),
@@ -41,35 +41,35 @@
     """
 
     def __init__(self, module_name: str, match: str) -> None:
         self.module_name = module_name
         self._match = match
         self._names: Dict[str, str] = {}
 
-    def visit_Import(self, node: ast.Import) -> Any:  # noqa: D102
+    def visit_Import(self, node: ast.Import) -> Any:
         # https://docs.python.org/3/library/ast.html#ast.Import
         for alias in node.names:
             self._names[alias.asname or alias.name] = alias.name
         return super().generic_visit(node)
 
-    def visit_ImportFrom(self, node: ast.ImportFrom) -> Any:  # noqa: D102
+    def visit_ImportFrom(self, node: ast.ImportFrom) -> Any:
         # https://docs.python.org/3/library/ast.html#ast.ImportFrom
         module = node.module
         if node.level > 0:
             root = self.module_name.rsplit(".", node.level)[0]
             module = f"{root}.{module}"
         for alias in node.names:
             self._names[alias.asname or alias.name] = f"{module}.{alias.name}"
         return super().generic_visit(node)
 
-    def visit_FunctionDef(self, node: ast.FunctionDef) -> Any:  # noqa: D102
+    def visit_FunctionDef(self, node: ast.FunctionDef) -> Any:
         # https://docs.python.org/3/library/ast.html#ast.FunctionDef
         self._find_decorators(node)
 
-    def visit_ClassDef(self, node: ast.ClassDef) -> Any:  # noqa: D102
+    def visit_ClassDef(self, node: ast.ClassDef) -> Any:
         self._find_decorators(node)
 
     def _find_decorators(self, node: Union[ast.ClassDef, ast.FunctionDef]):
         # for each in the decorator list ...
         for call in node.decorator_list:
             # https://docs.python.org/3/library/ast.html#ast.Call
             if isinstance(call, ast.Name) and self._names.get(call.id, "").startswith(
@@ -166,15 +166,15 @@
         decorator_name: str,
         node: Union[ast.ClassDef, ast.FunctionDef],
         decorator_kwargs: dict,
     ):
         self._store_contrib(decorator_name, node.name, decorator_kwargs)
 
     def _store_contrib(self, contrib_type: str, name: str, kwargs: Dict[str, Any]):
-        from ..implements import CHECK_ARGS_PARAM  # circ import
+        from npe2.implements import CHECK_ARGS_PARAM  # circ import
 
         kwargs.pop(CHECK_ARGS_PARAM, None)
         ContribClass, contrib_name = CONTRIB_MAP[contrib_type]
         contrib = ContribClass(**self._store_command(name, kwargs))
         existing: List[dict] = self.contribution_points.setdefault(contrib_name, [])
         existing.append(contrib.dict(exclude_unset=True))
 
@@ -254,15 +254,15 @@
         cmd = self._add_command(node)
         wrt_contrib = contributions.WriterContribution(
             command=cmd.id, layer_types=[layer_type], display_name=layer_type
         )
         self.contribution_points["writers"].append(wrt_contrib)
 
     def napari_provide_sample_data(self, node: ast.FunctionDef):
-        from ..manifest.utils import safe_key
+        from npe2.manifest.utils import safe_key
 
         return_ = next(n for n in node.body if isinstance(n, ast.Return))
         if not isinstance(return_.value, ast.Dict):
             raise TypeError(  # pragma: no cover
                 f"napari_provide_sample_data must return a dict, not {type(return_)}"
             )
 
@@ -273,15 +273,14 @@
 
             assert isinstance(key, ast.Constant)
             display_name = key.value
             key = safe_key(display_name)  # type: ignore
 
             # sample should now either be a callable, or a string
             if isinstance(val, ast.Name):
-
                 cmd_id = f"{self.plugin_name}.{val.id}"
                 py_name = f"{self.module_name}:{val.id}"
                 cmd_contrib = contributions.CommandContribution(
                     id=cmd_id, python_name=py_name, title=val.id
                 )
                 self.contribution_points["commands"].append(cmd_contrib)
                 contrib = contributions.SampleDataGenerator(
```

### Comparing `npe2-0.6.2/npe2/_plugin_manager.py` & `npe2-0.7.0/src/npe2/_plugin_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,15 +334,16 @@
             raise ValueError(f"A manifest with name {manifest.name!r} already exists.")
 
         self._manifests[manifest.name] = manifest
         if self.is_disabled(manifest.name):
             if warn_disabled:
                 warnings.warn(
                     f"Disabled plugin {manifest.name!r} was registered, but will not "
-                    "be indexed. Use `warn_disabled=False` to suppress this message."
+                    "be indexed. Use `warn_disabled=False` to suppress this message.",
+                    stacklevel=2,
                 )
         elif isinstance(manifest, NPE1Adapter):
             self._npe1_adapters.append(manifest)
         else:
             self._contrib.index_contributions(manifest)
         self.events.plugins_registered.emit({manifest})
 
@@ -488,15 +489,18 @@
             if disabled is True and not self.is_disabled(key):
                 continue
             elif disabled is False and self.is_disabled(key):
                 continue
             yield mf
 
     def dict(
-        self, *, include: InclusionSet = None, exclude: InclusionSet = None
+        self,
+        *,
+        include: Optional[InclusionSet] = None,
+        exclude: Optional[InclusionSet] = None,
     ) -> Dict[str, Any]:
         """Return a dictionary with the state of the plugin manager.
 
         `include` and `exclude` will be passed to each `PluginManifest.dict()`
         See pydantic documentation for details:
         https://pydantic-docs.helpmanual.io/usage/exporting_models/#modeldict
```

### Comparing `npe2-0.6.2/npe2/_pytest_plugin.py` & `npe2-0.7.0/src/npe2/_pytest_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+import logging
 import warnings
 from typing import Optional, Union
 from unittest.mock import patch
 
 import pytest
 
 from npe2 import DynamicPlugin, PluginManager, PluginManifest
 
+logger = logging.getLogger(__name__)
+
 
 class TestPluginManager(PluginManager):
     """A PluginManager subclass suitable for use in testing."""
 
     def discover(self, *_, **__) -> int:
         """Discovery is blocked in the TestPluginManager."""
-        import warnings
-
-        warnings.warn(
-            "TestPluginManager is unable to discover plugins. "
-            "Please use `tmp_plugin()` to add a plugin to this plugin manager."
+        logger.warning(
+            "NOTE: TestPluginManager refusing to discover plugins. "
+            "You may add plugins to this test plugin manager using `tmp_plugin()`."
         )
         return 0
 
     def tmp_plugin(
         self,
         manifest: Optional[Union[PluginManifest, str]] = None,
         package: Optional[str] = None,
@@ -58,24 +59,26 @@
         ...    with npe2pm.tmp_plugin(manifest=str(mf_file)) as plugin:
         ...        ...
         """
         if manifest is not None:
             if package or name:  # pragma: no cover
                 warnings.warn(
                     "`manifest` overrides the `package` and `name` arguments. "
-                    "Please provide only one."
+                    "Please provide only one.",
+                    stacklevel=2,
                 )
             if isinstance(manifest, PluginManifest):
                 mf = manifest
             else:
                 mf = PluginManifest.from_file(manifest)
         elif package:
             if name:  # pragma: no cover
                 warnings.warn(
-                    "`package` overrides the `name` argument. Please provide only one."
+                    "`package` overrides the `name` argument. Please provide only one.",
+                    stacklevel=2,
                 )
             mf = PluginManifest.from_distribution(package)
         else:
             name = name or "tmp_plugin"
             i = 0
             while name in self._manifests:  # pragma: no cover
                 # guarantee that name is unique
```

### Comparing `npe2-0.6.2/npe2/_setuptools_plugin.py` & `npe2-0.7.0/src/npe2/_setuptools_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,21 +54,23 @@
     trace("abs root", repr(locals()))
     if relative_to:
         if (
             os.path.isabs(root)
             and os.path.commonpath([root, relative_to]) != relative_to
         ):
             warnings.warn(
-                f"absolute root path '{root}' overrides relative_to '{relative_to}'"
+                f"absolute root path '{root}' overrides relative_to '{relative_to}'",
+                stacklevel=2,
             )
         if os.path.isdir(relative_to):
             warnings.warn(
                 "relative_to is expected to be a file,"
                 " its the directory {relative_to!r}\n"
-                "assuming the parent directory was passed"
+                "assuming the parent directory was passed",
+                stacklevel=2,
             )
             trace("dir", relative_to)
             root = os.path.join(relative_to, root)
         else:
             trace("file", relative_to)
             root = os.path.join(os.path.dirname(relative_to), root)
     return os.path.abspath(root)
```

### Comparing `npe2-0.6.2/npe2/cli.py` & `npe2-0.7.0/src/npe2/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         help="Show version and exit.",
         is_eager=True,
     ),
 ):
     """npe2: napari plugin engine (v{version})
 
     For additional help on a specific command: type 'npe2 [command] --help'
-    """  # noqa D400
+    """
 
 
 _main.__doc__ = typer.style(
     (_main.__doc__ or "").format(version=__version__), fg="bright_yellow"
 )
 
 SYNTAX_THME = "monokai"
@@ -427,15 +427,15 @@
                     bold=False,
                 )
             typer.echo()
 
     except Exception as e:
         msg = f"Conversion failed:\n{type(e).__name__}: {e}"
         typer.secho(msg, fg=typer.colors.RED, bold=True)
-        raise typer.Exit(1)
+        raise typer.Exit(1) from e
 
     if dry_run or not path.is_dir():
         if path.is_dir():
             typer.secho(
                 f"# Manifest would be written to {mf_path}",
                 fg=typer.colors.BRIGHT_GREEN,
                 bold=False,
```

### Comparing `npe2-0.6.2/npe2/implements.py` & `npe2-0.7.0/src/npe2/implements.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,29 +84,29 @@
 
             # return the original decorated function
             return func
 
         return _store_attrs
 
     # set the signature and return the decorator
-    setattr(_deco, "__signature__", signature)
+    _deco.__signature__ = signature  # type: ignore
     return _deco
 
 
 # builds decorators for each of the contribution types that are essentially just
 # pointers to some command.
 reader = _build_decorator(contributions.ReaderContribution)
 writer = _build_decorator(contributions.WriterContribution)
 widget = _build_decorator(contributions.WidgetContribution)
 sample_data_generator = _build_decorator(contributions.SampleDataGenerator)
 
 
 def on_activate(func):
     """Mark a function to be called when a plugin is activated."""
-    setattr(func, "npe2_on_activate", True)
+    func.npe2_on_activate = True
     return func
 
 
 def on_deactivate(func):
     """Mark a function to be called when a plugin is deactivated."""
-    setattr(func, "npe2_on_deactivate", True)
+    func.npe2_on_deactivate = True
     return func
```

### Comparing `npe2-0.6.2/npe2/implements.pyi` & `npe2-0.7.0/src/npe2/implements.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# flake8: noqa
 from typing import Any, Callable, List, TypeVar
 
 from pydantic import BaseModel as BaseModel
 
 from .manifest import PluginManifest as PluginManifest
 from .manifest import contributions as contributions
 
@@ -21,15 +20,15 @@
     """Mark a function as a reader contribution"""
 
 def writer(
     *,
     id: str,
     title: str,
     layer_types: List[str],
-    filename_extensions: List[str] = [],
+    filename_extensions: List[str] = [],  # noqa: B006
     display_name: str = "",
     ensure_args_valid: bool = False,
 ) -> Callable[[T], T]:
     """Mark function as a writer contribution"""
 
 def widget(
     *,
```

### Comparing `npe2-0.6.2/npe2/io_utils.py` & `npe2-0.7.0/src/npe2/io_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     return _read(paths, plugin_name=plugin_name, stack=stack)
 
 
 def read_get_reader(
     path: Union[str, Sequence[str]],
     *,
     plugin_name: Optional[str] = None,
-    stack: bool = None,
+    stack: Optional[bool] = None,
 ) -> Tuple[List[LayerData], ReaderContribution]:
     """Variant of `read` that also returns the `ReaderContribution` used."""
     if stack is None:
         # "npe1" old path
         # Napari 0.4.15 and older, hopefully we can drop this and make stack mandatory
         new_path, new_stack = v1_to_v2(path)
         return _read(
@@ -153,19 +153,27 @@
     """Execute the `read...` functions above."""
     if _pm is None:
         _pm = PluginManager.instance()
 
     for rdr in _pm.iter_compatible_readers(paths):
         if plugin_name and not rdr.command.startswith(plugin_name):
             continue
-        read_func = rdr.exec(kwargs={"path": paths, "stack": stack})
+        read_func = rdr.exec(
+            kwargs={"path": paths, "stack": stack, "_registry": _pm.commands}
+        )
         if read_func is not None:
             # if the reader function raises an exception here, we don't try to catch it
             if layer_data := read_func(paths, stack=stack):
                 return (layer_data, rdr) if return_reader else layer_data
+
+    if plugin_name:
+        raise ValueError(
+            f"Plugin {plugin_name!r} was selected to open "
+            + f"{paths!r}, but returned no data."
+        )
     raise ValueError(f"No readers returned data for {paths!r}")
 
 
 @overload
 def _write(
     path: str,
     layer_data: List[Union[FullLayerData, napari.layers.Layer]],
@@ -193,15 +201,14 @@
     path: str,
     layer_data: List[Union[FullLayerData, napari.layers.Layer]],
     *,
     plugin_name: Optional[str] = None,
     return_writer: bool = False,
     _pm: Optional[PluginManager] = None,
 ) -> Union[List[str], Tuple[List[str], WriterContribution]]:
-
     if not layer_data:
         raise ValueError("Must provide layer data")
     if _pm is None:
         _pm = PluginManager.instance()
 
     _layer_tuples: List[FullLayerData] = [
         cast("napari.layers.Layer", x).as_layer_data_tuple()
```

### Comparing `npe2-0.6.2/npe2/manifest/_bases.py` & `npe2-0.7.0/src/npe2/manifest/_bases.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/npe2/manifest/_npe1_adapter.py` & `npe2-0.7.0/src/npe2/manifest/_npe1_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from importlib import metadata
 from pathlib import Path
 from shutil import rmtree
 from typing import List, Sequence
 
 from appdirs import user_cache_dir
 
-from .._inspection._from_npe1 import manifest_from_npe1
-from ..manifest import PackageMetadata
+from npe2._inspection._from_npe1 import manifest_from_npe1
+from npe2.manifest import PackageMetadata
+
 from .schema import PluginManifest, discovery_blocked
 
 logger = logging.getLogger(__name__)
 ADAPTER_CACHE = Path(user_cache_dir("napari", "napari")) / "npe2" / "adapter_manifests"
 NPE2_NOCACHE = "NPE2_NOCACHE"
 
 
@@ -99,15 +100,16 @@
 
         with discovery_blocked():
             try:
                 mf = manifest_from_npe1(self._dist, adapter=True)
             except Exception as e:
                 warnings.warn(
                     "Error importing contributions for first-generation "
-                    f"napari plugin {self.name!r}: {e}"
+                    f"napari plugin {self.name!r}: {e}",
+                    stacklevel=2,
                 )
                 return
 
             self.contributions = mf.contributions
             logger.debug("%r npe1 adapter imported", self.name)
 
         if save and not _is_editable_install(self._dist):
@@ -136,9 +138,9 @@
 
 def _is_editable_install(dist: metadata.Distribution) -> bool:
     """Return True if dist is installed as editable.
 
     i.e: if the package isn't in site-packages or user site-packages.
     """
     root = str(dist.locate_file(""))
-    installed_paths = site.getsitepackages() + [site.getusersitepackages()]
+    installed_paths = [*site.getsitepackages(), site.getusersitepackages()]
     return all(loc not in root for loc in installed_paths)
```

### Comparing `npe2-0.6.2/npe2/manifest/_package_metadata.py` & `npe2-0.7.0/src/npe2/manifest/_package_metadata.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/npe2/manifest/_validators.py` & `npe2-0.7.0/src/npe2/manifest/_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 
 _package_name = "([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])"
-_python_identifier = "([a-zA-Z_][a-zA-Z_0-9]*)"  # noqa
+_python_identifier = "([a-zA-Z_][a-zA-Z_0-9]*)"
 
 # how do we deal with keywords ?
 # do we try to validate ? Or do we just
 # assume users won't try to create a command named
 # `npe2_tester.False.if.for.in` ?
 _identifier_plus_dash = "(?:[a-zA-Z_][a-zA-Z_0-9-]+)"
 _dotted_name = f"(?:(?:{_identifier_plus_dash}\\.)*{_identifier_plus_dash})"
```

### Comparing `npe2-0.6.2/npe2/manifest/contributions/__init__.py` & `npe2-0.7.0/src/npe2/manifest/contributions/__init__.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/npe2/manifest/contributions/_commands.py` & `npe2-0.7.0/src/npe2/manifest/contributions/_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import TYPE_CHECKING, Any, Optional, Union
 
 from pydantic import BaseModel, Extra, Field, validator
 
-from ...types import PythonName
-from .. import _validators
+from npe2.manifest import _validators
+from npe2.types import PythonName
+
 from ._icon import Icon
 
 if TYPE_CHECKING:
-    from ..._command_registry import CommandRegistry
+    from npe2._command_registry import CommandRegistry
 
 
 class CommandContribution(BaseModel):
     """Contribute a **command** (a python callable) consisting of a unique `id`,
     a `title` and (optionally) a `python_path` that points to a fully qualified python
     callable.  If a `python_path` is not included in the manifest, it *must* be
     registered during activation with `register_command`.
@@ -87,17 +88,17 @@
 
     class Config:
         extra = Extra.forbid
 
     def exec(
         self,
         args: tuple = (),
-        kwargs: dict = None,
+        kwargs: Optional[dict] = None,
         _registry: Optional["CommandRegistry"] = None,
     ) -> Any:
         if kwargs is None:
             kwargs = {}
         if _registry is None:
-            from ..._plugin_manager import PluginManager
+            from npe2._plugin_manager import PluginManager
 
             _registry = PluginManager.instance().commands
         return _registry.execute(self.id, args, kwargs)
```

### Comparing `npe2-0.6.2/npe2/manifest/contributions/_configuration.py` & `npe2-0.7.0/src/npe2/manifest/contributions/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,16 @@
         for ignored in {"$ref", "ref", "definition", "$def"}:
             if ignored in values:
                 import warnings
 
                 del values[ignored]
                 warnings.warn(
                     f"ignoring {ignored} in configuration property. "
-                    "Configuration schemas must be self-contained."
+                    "Configuration schemas must be self-contained.",
+                    stacklevel=2,
                 )
         return values
 
     def validate_instance(self, instance: object) -> dict:
         """Validate an object (instance) against this schema."""
         try:
             return super().validate_instance(instance)
```

### Comparing `npe2-0.6.2/npe2/manifest/contributions/_contributions.py` & `npe2-0.7.0/src/npe2/manifest/contributions/_contributions.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/npe2/manifest/contributions/_json_schema.py` & `npe2-0.7.0/src/npe2/manifest/contributions/_json_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     "object": dict,
     "string": str,
     None: object,
 }
 
 
 class _JsonSchemaBase(BaseModel):
-    class Config:  # noqa: D106
+    class Config:
         alias_generator = _to_camel
         allow_population_by_field_name = True
 
     # underscore here to avoid name collision with pydantic's `schema` method
     schema_: Optional[str] = Field(None, alias="$schema")
     title: Optional[str] = Field(None)
     description: Optional[str] = Field(None)
```

### Comparing `npe2-0.6.2/npe2/manifest/contributions/_keybindings.py` & `npe2-0.7.0/src/npe2/manifest/contributions/_keybindings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
 from pydantic.fields import Field
 
-from ..utils import Executable
+from npe2.manifest.utils import Executable
 
 
 class KeyBindingContribution(Executable):
     command: str = Field(
         description="Identifier of the command to run when keybinding is triggered."
     )
     # the existence of the command is not validated at registration-time,
```

### Comparing `npe2-0.6.2/npe2/manifest/contributions/_menus.py` & `npe2-0.7.0/src/npe2/manifest/contributions/_menus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Union
 
 from pydantic import BaseModel, Field
 
-from ..utils import Executable
+from npe2.manifest.utils import Executable
 
 
 # user provides this
 class _MenuItem(BaseModel):
     """Generic menu item contribution."""
 
     when: Optional[str] = Field(
```

### Comparing `npe2-0.6.2/npe2/manifest/contributions/_readers.py` & `npe2-0.7.0/src/npe2/manifest/contributions/_readers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from functools import wraps
 from typing import List, Optional
 
 from pydantic import Extra, Field
 
-from ...types import ReaderFunction
-from ..utils import Executable, v2_to_v1
+from npe2.manifest.utils import Executable, v2_to_v1
+from npe2.types import ReaderFunction
 
 
 class ReaderContribution(Executable[Optional[ReaderFunction]]):
     """Contribute a file reader.
 
     Readers may be associated with specific **filename_patterns** (e.g. "*.tif",
     "*.zip") and are invoked whenever `viewer.open('some/path')` is used on the
```

### Comparing `npe2-0.6.2/npe2/manifest/contributions/_sample_data.py` & `npe2-0.7.0/src/npe2/manifest/contributions/_sample_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, List, Optional, Union
 
 from pydantic.fields import Field
 from pydantic.generics import GenericModel
 
-from ...types import LayerData
-from ..utils import Executable
+from npe2.manifest.utils import Executable
+from npe2.types import LayerData
 
 if TYPE_CHECKING:
-    from ..._command_registry import CommandRegistry
+    from npe2._command_registry import CommandRegistry
 
 
 class _SampleDataContribution(GenericModel, ABC):
     """Contribute sample data for use in napari.
 
     Sample data can take the form of a **command** that returns layer data, or a simple
     path or **uri** to a local or remote resource (assuming there is a reader plugin
@@ -59,15 +59,15 @@
     )
     reader_plugin: Optional[str] = Field(
         None,
         description="Name of plugin to use to open URI",
     )
 
     def open(self, *args, **kwargs) -> List[LayerData]:
-        from ...io_utils import read
+        from npe2.io_utils import read
 
         return read([self.uri], plugin_name=self.reader_plugin, stack=False)
 
     class Config:
         title = "Sample Data URI"
```

### Comparing `npe2-0.6.2/npe2/manifest/contributions/_submenu.py` & `npe2-0.7.0/src/npe2/manifest/contributions/_submenu.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/npe2/manifest/contributions/_themes.py` & `npe2-0.7.0/src/npe2/manifest/contributions/_themes.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/npe2/manifest/contributions/_widgets.py` & `npe2-0.7.0/src/npe2/manifest/contributions/_widgets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Callable, Optional
 
 from pydantic import Extra, Field
 
-from ...types import Widget
-from ..utils import Executable
+from npe2.manifest.utils import Executable
+from npe2.types import Widget
 
 if TYPE_CHECKING:
-    from ..._command_registry import CommandRegistry
+    from npe2._command_registry import CommandRegistry
 
 
 class WidgetContribution(Executable[Widget]):
     """Contribute a widget that can be added to the napari viewer.
 
     Widget contributions point to a **command** that, when called, returns a widget
     *instance*; this includes functions that return a widget instance, (e.g. those
```

### Comparing `npe2-0.6.2/npe2/manifest/contributions/_writers.py` & `npe2-0.7.0/src/npe2/manifest/contributions/_writers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
 from typing import List, Tuple
 
 from pydantic import BaseModel, Extra, Field, validator
 
-from ..utils import Executable
+from npe2.manifest.utils import Executable
 
 
 class LayerType(str, Enum):
     image = "image"
     labels = "labels"
     points = "points"
     shapes = "shapes"
```

### Comparing `npe2-0.6.2/npe2/manifest/schema.py` & `npe2-0.7.0/src/npe2/manifest/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from pathlib import Path
 from typing import Iterator, List, Literal, NamedTuple, Optional, Sequence, Union
 
 from pydantic import Extra, Field, ValidationError, root_validator, validator
 from pydantic.error_wrappers import ErrorWrapper
 from pydantic.main import BaseModel, ModelMetaclass
 
-from ..types import PythonName
+from npe2.types import PythonName
+
 from . import _validators
 from ._bases import ImportExportModel
 from ._package_metadata import PackageMetadata
 from .contributions import ContributionPoints
 from .utils import Executable, Version
 
 logger = getLogger(__name__)
@@ -253,15 +254,16 @@
         current_version = Version.parse(SCHEMA_VERSION)
         if current_version < declared_version:
             import warnings
 
             warnings.warn(
                 f"The declared schema version for plugin {mf_name!r} "
                 f"({declared_version}) is newer than npe2's schema version "
-                f"({current_version}). Things may break, you should upgrade npe2."
+                f"({current_version}). Things may break, you should upgrade npe2.",
+                stacklevel=2,
             )
 
         invalid_commands: List[str] = []
         if values.get("contributions") is not None:
             invalid_commands.extend(
                 command.id
                 for command in values["contributions"].commands or []
@@ -373,15 +375,14 @@
 
     @classmethod
     def _from_entrypoint(
         cls,
         entry_point: metadata.EntryPoint,
         distribution: Optional[metadata.Distribution] = None,
     ) -> PluginManifest:
-
         assert (match := entry_point.pattern.match(entry_point.value))
         module = match.group("module")
 
         spec = util.find_spec(module or "")
         if not spec:  # pragma: no cover
             raise ValueError(
                 f"Cannot find module {module!r} declared in "
@@ -490,19 +491,19 @@
 def _noop(*_, **__):
     return []  # pragma: no cover
 
 
 @contextmanager
 def discovery_blocked():
     orig = PluginManifest.discover
-    setattr(PluginManifest, "discover", _noop)
+    PluginManifest.discover = _noop  # type: ignore [method-assign]
     try:
         yield
     finally:
-        setattr(PluginManifest, "discover", orig)
+        PluginManifest.discover = orig  # type: ignore [method-assign]
 
 
 @contextmanager
 def _temporary_path_additions(paths: Sequence[Union[str, Path]] = ()):
     if paths and (not isinstance(paths, Sequence) or isinstance(paths, str)):
         raise TypeError("paths must be a sequence of strings")  # pragma: no cover
     for p in reversed(paths):
```

### Comparing `npe2-0.6.2/npe2/manifest/utils.py` & `npe2-0.7.0/src/npe2/manifest/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,20 +17,20 @@
     TypeVar,
     Union,
 )
 
 from pydantic import PrivateAttr
 from pydantic.generics import GenericModel
 
-from ..types import PythonName
+from npe2.types import PythonName
 
 if TYPE_CHECKING:
+    from npe2._command_registry import CommandRegistry
     from npe2.manifest.schema import PluginManifest
 
-    from .._command_registry import CommandRegistry
     from .contributions import ContributionPoints
 
 
 def v1_to_v2(path):
     return (path, True) if isinstance(path, list) else ([path], False)
 
 
@@ -50,27 +50,28 @@
     command: str
     # plugin_name gets populated in `PluginManifest.__init__`
     _plugin_name: str = PrivateAttr("")
 
     def exec(
         self,
         args: tuple = (),
-        kwargs: dict = None,
+        kwargs: Optional[dict] = None,
         _registry: Optional[CommandRegistry] = None,
     ) -> R:
         if kwargs is None:
             kwargs = {}
-        return self.get_callable(_registry)(*args, **kwargs)
+        reg = _registry or kwargs.pop("_registry", None)
+        return self.get_callable(reg)(*args, **kwargs)
 
     def get_callable(
         self,
         _registry: Optional[CommandRegistry] = None,
     ) -> Callable[..., R]:
         if _registry is None:
-            from .._plugin_manager import PluginManager
+            from npe2._plugin_manager import PluginManager
 
             _registry = PluginManager.instance().commands
         return _registry.get(self.command)
 
     @property
     def plugin_name(self) -> str:
         """Return the manifest/plugin name for this contribution."""
```

### Comparing `npe2-0.6.2/npe2/plugin_manager.py` & `npe2-0.7.0/src/npe2/plugin_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code=empty-body
 """Convenience module to access methods on the global PluginManager singleton."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict
 
 if TYPE_CHECKING:
     from os import PathLike
@@ -24,15 +25,18 @@
 
 
 def discover(paths: Sequence[str] = (), clear=False, include_npe1=False) -> None:
     """Discover and index plugin manifests in the environment."""
 
 
 def dict(
-    self, *, include: InclusionSet = None, exclude: InclusionSet = None
+    self,
+    *,
+    include: Optional[InclusionSet] = None,
+    exclude: Optional[InclusionSet] = None,
 ) -> Dict[str, Any]:
     """Return a dictionary with the state of the plugin manager."""
 
 
 def index_npe1_adapters() -> None:
     """Import and index any/all npe1 adapters."""
 
@@ -109,17 +113,17 @@
     """Iterate over compatible WriterContributions given a sequence of layer_types."""
 
 
 def iter_widgets() -> Iterator[contributions.WidgetContribution]:
     """Iterate over discovered WidgetContributions."""
 
 
-def iter_sample_data() -> Iterator[
-    Tuple[PluginName, List[contributions.SampleDataContribution]]
-]:
+def iter_sample_data() -> (
+    Iterator[Tuple[PluginName, List[contributions.SampleDataContribution]]]
+):
     """Iterates over (plugin_name, [sample_contribs])."""
 
 
 def get_writer(
     path: str, layer_types: Sequence[str], plugin_name: Optional[str] = None
 ) -> Tuple[Optional[contributions.WriterContribution], str]:
     """Get Writer contribution appropriate for `path`, and `layer_types`."""
```

### Comparing `npe2-0.6.2/npe2/types.py` & `npe2-0.7.0/src/npe2/types.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/npe2.egg-info/PKG-INFO` & `npe2-0.7.0/src/npe2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: npe2
-Version: 0.6.2
-Summary: proposal for napari plugin refactor
-Home-page: https://github.com/napari/npe2
-Author: Talley Lambert, Nathan Clack
-Author-email: talley.lambert@gmail.com
+Version: 0.7.0
+Summary: napari plugin engine v2
+Author: Nathan Clack
+Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD-3-Clause
-Project-URL: Source Code, https://github.com/napari/npe2
+Project-URL: homepage, https://github.com/napari/npe2
+Project-URL: repository, https://github.com/napari/npe2
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: json
-Provides-Extra: testing
 License-File: LICENSE
 
 # npe2
 
 [![CI](https://github.com/napari/npe2/actions/workflows/ci.yml/badge.svg)](https://github.com/napari/npe2/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/napari/npe2/branch/main/graph/badge.svg?token=FTH635x542)](https://codecov.io/gh/napari/npe2)
```

### Comparing `npe2-0.6.2/tests/conftest.py` & `npe2-0.7.0/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                 pth = npe1_repo / "npe1-plugin-0.0.1.dist-info"
                 yield metadata.PathDistribution(pth)
             return
 
     sys.meta_path.append(Importer())
     sys.path.append(str(npe1_repo))
     try:
-        pkgs = site.getsitepackages() + [str(npe1_repo)]
+        pkgs = [*site.getsitepackages(), str(npe1_repo)]
         with patch("site.getsitepackages", return_value=pkgs):
             yield
     finally:
         sys.path.remove(str(npe1_repo))
 
 
 @pytest.fixture
@@ -111,26 +111,26 @@
 
 @pytest.fixture
 def mock_npe1_pm():
     from napari_plugin_engine import PluginManager, napari_hook_specification
 
     # fmt: off
     class HookSpecs:
-        def napari_provide_sample_data(): ...  # type: ignore  # noqa: E704
-        def napari_get_reader(path): ...  # noqa: E704
-        def napari_get_writer(path, layer_types): ...  # noqa: E704
-        def napari_write_image(path, data, meta): ...  # noqa: E704
-        def napari_write_labels(path, data, meta): ...  # noqa: E704
-        def napari_write_points(path, data, meta): ...  # noqa: E704
-        def napari_write_shapes(path, data, meta): ...  # noqa: E704
-        def napari_write_surface(path, data, meta): ...  # noqa: E704
-        def napari_write_vectors(path, data, meta): ...  # noqa: E704
-        def napari_experimental_provide_function(): ...  # type: ignore  # noqa: E704
-        def napari_experimental_provide_dock_widget(): ...  # type: ignore  # noqa: E704
-        def napari_experimental_provide_theme(): ...  # type: ignore  # noqa: E704
+        def napari_provide_sample_data(): ...  # type: ignore
+        def napari_get_reader(path): ...
+        def napari_get_writer(path, layer_types): ...
+        def napari_write_image(path, data, meta): ...
+        def napari_write_labels(path, data, meta): ...
+        def napari_write_points(path, data, meta): ...
+        def napari_write_shapes(path, data, meta): ...
+        def napari_write_surface(path, data, meta): ...
+        def napari_write_vectors(path, data, meta): ...
+        def napari_experimental_provide_function(): ...  # type: ignore
+        def napari_experimental_provide_dock_widget(): ...  # type: ignore
+        def napari_experimental_provide_theme(): ...  # type: ignore
     # fmt: on
 
     for m in dir(HookSpecs):
         if m.startswith("napari"):
             setattr(HookSpecs, m, napari_hook_specification(getattr(HookSpecs, m)))
 
     pm = PluginManager("napari")
```

### Comparing `npe2-0.6.2/tests/fixtures/my-compiled-plugin/my_module/_a.py` & `npe2-0.7.0/tests/fixtures/my-compiled-plugin/my_module/_a.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code=empty-body
 from typing import TYPE_CHECKING, Any, Dict, List, Tuple
 
 # alternative pattern that does not require npe2 at runtime
 if TYPE_CHECKING:
     from npe2 import implements
 else:
     # create no-op `implements.anything(**kwargs)` decorator
```

### Comparing `npe2-0.6.2/tests/fixtures/my-compiled-plugin/my_module/_b.py` & `npe2-0.7.0/tests/fixtures/my-compiled-plugin/my_module/_b.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/tests/npe1-plugin/npe1_module/__init__.py` & `npe2-0.7.0/tests/npe1-plugin/npe1_module/__init__.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/tests/sample/_with_decorators.py` & `npe2-0.7.0/tests/sample/_with_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code=empty-body
 """This module mimics all of the contributions my-plugin...
 but is used to reverse-engineer the manifest."""
 from typing import TYPE_CHECKING, Any, Dict, List, Tuple
 
 # to test various ways that this can be imported, since we're using static parsing.
 import npe2.implements
 import npe2.implements as impls
```

### Comparing `npe2-0.6.2/tests/sample/my_plugin/__init__.py` & `npe2-0.7.0/tests/sample/my_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/tests/sample/my_plugin/napari.yaml` & `npe2-0.7.0/tests/sample/my_plugin/napari.yaml`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/tests/test__io_utils.py` & `npe2-0.7.0/tests/test__io_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 # extra underscore in name to run this first
 
 import pytest
 
-from npe2 import read, read_get_reader, write, write_get_writer
+from npe2 import (
+    DynamicPlugin,
+    PluginManager,
+    io_utils,
+    read,
+    read_get_reader,
+    write,
+    write_get_writer,
+)
 from npe2.types import FullLayerData
 
 SAMPLE_PLUGIN_NAME = "my-plugin"
 
 
 def test_read(uses_sample_plugin):
     assert read(["some.fzzy"], stack=False) == [(None,)]
 
 
-def test_read_with_plugin(uses_sample_plugin):
-    # no such plugin name.... but skips over the sample plugin
-    with pytest.raises(ValueError):
+def test_read_with_unknown_plugin(uses_sample_plugin):
+    # no such plugin name.... skips over the sample plugin & error is specific
+    with pytest.raises(ValueError, match="Plugin 'nope' was selected"):
         read(["some.fzzy"], plugin_name="nope", stack=False)
 
 
+def test_read_with_no_plugin():
+    # no plugin passed and none registered
+    with pytest.raises(ValueError, match="No readers returned"):
+        read(["some.nope"], stack=False)
+
+
 def test_read_return_reader(uses_sample_plugin):
     data, reader = read_get_reader("some.fzzy")
     assert data == [(None,)]
     assert reader.command == f"{SAMPLE_PLUGIN_NAME}.some_reader"
 
 
 def test_read_return_reader_with_stack(uses_sample_plugin):
@@ -62,7 +76,21 @@
         write("test.tif", [null_image, null_image, null_image, null_image, null_image])
 
 
 def test_writer_single_layer_api_exec(uses_sample_plugin):
     # This writer doesn't do anything but type check.
     paths = write("test/path", [([], {}, "labels")])
     assert len(paths) == 1
+
+
+def test_read_non_global_pm():
+    pm = PluginManager()
+    plugin = DynamicPlugin("my-plugin", plugin_manager=pm)
+
+    @plugin.contribute.reader
+    def read_path(path):
+        def _reader(path):
+            return [(None,)]
+
+        return _reader
+
+    assert io_utils._read(["some.fzzy"], stack=False, _pm=pm) == [(None,)]
```

### Comparing `npe2-0.6.2/tests/test_all_plugins.py` & `npe2-0.7.0/tests/test_all_plugins.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/tests/test_cli.py` & `npe2-0.7.0/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 @pytest.mark.parametrize("debug", ["--debug", ""])
 @pytest.mark.parametrize("imports", ["--imports", "--no-imports"])
 def test_cli_validate_ok(sample_path, debug, imports, monkeypatch):
     cmd = ["validate", str(sample_path / "my_plugin" / "napari.yaml"), imports]
     if debug:
         cmd += [debug]
     with monkeypatch.context() as m:
-        m.setattr(sys, "path", sys.path + [str(sample_path)])
+        m.setattr(sys, "path", [*sys.path, str(sample_path)])
         result = runner.invoke(app, cmd)
     assert "✔ Manifest for 'My Plugin' valid!" in result.stdout
     assert result.exit_code == 0
 
 
 def test_cli_validate_invalid(tmp_path, capsys):
     (tmp_path / "manifest.yaml").write_text("name: hi??\n")
```

### Comparing `npe2-0.6.2/tests/test_compile.py` & `npe2-0.7.0/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/tests/test_config_contribution.py` & `npe2-0.7.0/tests/test_config_contribution.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/tests/test_contributions.py` & `npe2-0.7.0/tests/test_contributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from functools import partial
 from unittest.mock import Mock
 
 import pytest
 
 from npe2 import DynamicPlugin, PluginManager, PluginManifest
 from npe2.manifest.contributions import (
     CommandContribution,
@@ -91,25 +92,23 @@
     assert reader.command == f"{SAMPLE_PLUGIN_NAME}.some_reader"
 
     with pytest.raises(ValueError):
         list(plugin_manager.iter_compatible_readers(["a.tif", "b.jpg"]))
 
 
 def test_widgets(uses_sample_plugin, plugin_manager: PluginManager):
-    from magicgui._magicgui import MagicFactory
-
     widgets = list(plugin_manager.iter_widgets())
     assert len(widgets) == 2
     assert widgets[0].command == f"{SAMPLE_PLUGIN_NAME}.some_widget"
     w = widgets[0].exec()
     assert type(w).__name__ == "SomeWidget"
 
     assert widgets[1].command == f"{SAMPLE_PLUGIN_NAME}.some_function_widget"
     w = widgets[1].get_callable()
-    assert isinstance(w, MagicFactory)
+    assert isinstance(w, partial)
 
 
 def test_sample(uses_sample_plugin, plugin_manager: PluginManager):
     plugin, contribs = list(plugin_manager.iter_sample_data())[0]
     assert plugin == SAMPLE_PLUGIN_NAME
     assert len(contribs) == 2
     ctrbA, ctrbB = contribs
```

### Comparing `npe2-0.6.2/tests/test_conversion.py` & `npe2-0.7.0/tests/test_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,18 +121,14 @@
 
 
 def test_conversion_package_is_not_a_plugin():
     with pytest.raises(PackageNotFoundError):
         manifest_from_npe1("pytest")
 
 
-def test_convert_repo():
-    convert_repository
-
-
 def test_get_top_module_path(mock_npe1_pm_with_plugin):
     get_top_module_path("npe1-plugin")
 
 
 def test_python_name_local():
     def f():
         return lambda x: None
```

### Comparing `npe2-0.6.2/tests/test_docs.py` & `npe2-0.7.0/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/tests/test_fetch.py` & `npe2-0.7.0/tests/test_fetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
         with pytest.raises(PackageNotFoundError):
             fetch_manifest("my-package")
 
 
 @pytest.mark.skipif(not os.getenv("CI"), reason="slow, only run on CI")
 def testfetch_manifest_with_full_install():
     # TODO: slowest of the tests ... would be nice to provide a local mock
-    mf = fetch_manifest_with_full_install("napari-ndtiffs")
+    mf = fetch_manifest_with_full_install("napari-ndtiffs", version="0.1.2")
+    # use version 0.1.2 which is npe1
     assert isinstance(mf, NPE1Adapter)
     assert mf.name == "napari-ndtiffs"
     assert mf.contributions
 
 
 @pytest.mark.skipif(not os.getenv("CI"), reason="slow, only run on CI")
 def test_manifest_from_sdist():
```

### Comparing `npe2-0.6.2/tests/test_implements.py` & `npe2-0.7.0/tests/test_implements.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,27 +40,26 @@
     assert sorted(extracted.readers, key=k) == sorted(expected.readers, key=k)
     assert sorted(extracted.writers, key=k) == sorted(expected.writers, key=k)
     assert sorted(extracted.widgets, key=k) == sorted(expected.widgets, key=k)
     assert sorted(extracted.sample_data, key=k) == sorted(expected.sample_data, key=k)
 
 
 def test_dynamic(monkeypatch):
-
     with monkeypatch.context() as m:
-        m.setattr(sys, "path", sys.path + [str(SAMPLE_DIR)])
-        import _with_decorators  # noqa
+        m.setattr(sys, "path", [*sys.path, str(SAMPLE_DIR)])
+        import _with_decorators
 
         assert hasattr(_with_decorators.get_reader, "_npe2_ReaderContribution")
         info = _with_decorators.get_reader._npe2_ReaderContribution
-        assert info == dict(
-            id="some_reader",
-            title="Some Reader",
-            filename_patterns=["*.fzy", "*.fzzy"],
-            accepts_directories=True,
-        )
+        assert info == {
+            "id": "some_reader",
+            "title": "Some Reader",
+            "filename_patterns": ["*.fzy", "*.fzzy"],
+            "accepts_directories": True,
+        }
 
         # we can compile a module object as well as a string path
         extracted = find_npe2_module_contributions(
             _with_decorators,
             plugin_name=SAMPLE_PLUGIN_NAME,
             module_name=SAMPLE_MODULE_NAME,
         )
@@ -68,12 +67,12 @@
         assert extracted.commands
 
 
 @pytest.mark.parametrize("check", [True, False])
 def test_decorator_arg_check(check):
     """Check that the decorators don't check arguments at runtime unless instructed."""
     # tilde is wrong and filename_patterns is missing
-    kwargs = dict(id="some_id", tilde="some_title")
+    kwargs = {"id": "some_id", "tilde": "some_title"}
     kwargs[npe2.implements.CHECK_ARGS_PARAM] = check
     ctx = pytest.raises(TypeError) if check else nullcontext()
     with ctx:
         npe2.implements.reader(**kwargs)(lambda: None)
```

### Comparing `npe2-0.6.2/tests/test_manifest.py` & `npe2-0.7.0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/tests/test_npe1_adapter.py` & `npe2-0.7.0/tests/test_npe1_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from functools import partial
 from importlib import metadata
 from pathlib import Path
 from unittest.mock import patch
 
 import numpy as np
 import pytest
-from magicgui._magicgui import MagicFactory
 
 from npe2 import PluginManager
 from npe2.manifest import _npe1_adapter, utils
 from npe2.manifest.contributions import SampleDataGenerator
 from npe2.manifest.utils import SHIM_NAME_PREFIX
 
 
@@ -67,15 +66,14 @@
     pm.discover(include_npe1=True)
 
     with patch.object(
         _npe1_adapter,
         "manifest_from_npe1",
         wraps=_npe1_adapter.manifest_from_npe1,  # type: ignore
     ) as mock:
-
         # if we clear the cache, it should import again
         mf = pm.get_manifest("npe1-plugin")
         assert isinstance(mf, _npe1_adapter.NPE1Adapter)
         pm.index_npe1_adapters()
         mock.assert_called_once_with(mf._dist, adapter=True)
         assert mf._cache_path().exists()
 
@@ -131,27 +129,27 @@
     mf = _get_mf()
     widgets = mf.contributions.widgets
     assert widgets
     wdg_contrib = next(w for w in widgets if w.display_name == "Local Widget")
 
     with patch.object(utils, "_import_npe1_shim", wraps=utils._import_npe1_shim) as m:
         caller = wdg_contrib.get_callable()
-        assert isinstance(caller, MagicFactory)
+        assert isinstance(caller, partial)
         assert "<locals>.local_widget" in caller.keywords["function"].__qualname__
         pyname = (
             f"{SHIM_NAME_PREFIX}npe1_module:napari_experimental_provide_dock_widget_2"
         )
         m.assert_called_once_with(pyname)
 
         m.reset_mock()
         wdg_contrib2 = next(
             w for w in widgets if w.display_name == "local function" and w.autogenerate
         )
         caller2 = wdg_contrib2.get_callable()
-        assert isinstance(caller2, MagicFactory)
+        assert isinstance(caller2, partial)
         assert "<locals>.local_function" in caller2.keywords["function"].__qualname__
         pyname = f"{SHIM_NAME_PREFIX}npe1_module:napari_experimental_provide_function_1"
         m.assert_called_once_with(pyname)
 
 
 def test_adapter_error_on_import():
     class FakeDist(metadata.Distribution):
@@ -165,22 +163,22 @@
     adapter = _npe1_adapter.NPE1Adapter(FakeDist())
 
     def err():
         raise ImportError("No package found.")
 
     with pytest.warns(UserWarning) as record:
         with patch.object(_npe1_adapter, "manifest_from_npe1", wraps=err):
-            adapter.contributions
+            _ = adapter.contributions
     assert "Error importing contributions for" in str(record[0])
 
 
 def test_adapter_cache_fail(uses_npe1_plugin, mock_cache):
     pm = PluginManager()
     pm.discover(include_npe1=True)
     mf = pm.get_manifest("npe1-plugin")
 
     def err(obj):
         raise OSError("Can't cache")
 
     with patch.object(_npe1_adapter.NPE1Adapter, "_save_to_cache", err):
         # shouldn't reraise the error
-        mf.contributions
+        _ = mf.contributions
```

### Comparing `npe2-0.6.2/tests/test_package_meta.py` & `npe2-0.7.0/tests/test_package_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         "version": "1.0",
         "maintainer": "bob",
         "extra_field_that_is_definitely_not_in_the_model": False,
     }
 
     try:
         p = PackageMetadata(**pkg)
-    except Exception:
+    except Exception as e:
         raise AssertionError(
             "failed to parse PackageMetadata from a dict with an extra field"
-        )
+        ) from e
 
     assert p.name == "test"
     assert p.version == "1.0"
     assert p.maintainer == "bob"
     assert not hasattr(p, "extra_field_that_is_definitely_not_in_the_model")
```

### Comparing `npe2-0.6.2/tests/test_plugin_manager.py` & `npe2-0.7.0/tests/test_plugin_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from npe2.types import PythonName
 
 SAMPLE_PLUGIN_NAME = "my-plugin"
 
 
 @pytest.fixture
 def pm(sample_path):
-
     pm = PluginManager()
     pm.discover()
     assert len(pm._manifests) == 0
     sys.path.append(str(sample_path))
     try:
         pm.discover()
         yield pm
@@ -160,15 +159,14 @@
     assert c if enabled else not c, f"Writer should {_not}be enabled"
 
     d = "SampleTheme" in [t.label for t in plugin_manager.iter_themes()]
     assert d if enabled else not d, f"Theme should {_not}be enabled"
 
 
 def test_enable_disable(uses_sample_plugin, plugin_manager: PluginManager, tmp_path):
-
     _assert_sample_enabled(plugin_manager)
     # just to test the enabled= kwarg on iter_manifests
     # (this would show *only* disabled plugins)
     assert not list(plugin_manager.iter_manifests(disabled=True))
 
     # Do disable
     mock = Mock()
```

### Comparing `npe2-0.6.2/tests/test_pm_module.py` & `npe2-0.7.0/tests/test_pm_module.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/tests/test_pytest_plugin.py` & `npe2-0.7.0/tests/test_pytest_plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,17 +10,19 @@
     assert isinstance(npe2pm, TestPluginManager)
     assert PluginManager.instance() is npe2pm
 """
 
 CASE2 = """
 import pytest
 
-def test_something_2(npe2pm):
-    with pytest.warns(UserWarning, match='unable to discover plugins'):
-        npe2pm.discover()
+def test_something_2(npe2pm, caplog):
+    npe2pm.discover()
+    assert "TestPluginManager refusing to discover plugins" in caplog.text
+    assert len(caplog.records) == 1
+    assert caplog.records[0].levelname == "WARNING"
 """
 
 CASE3 = """
 from npe2 import DynamicPlugin
 
 def test_something_3(npe2pm):
     with npe2pm.tmp_plugin(name='some_name') as plugin:
```

### Comparing `npe2-0.6.2/tests/test_setuptools_plugin.py` & `npe2-0.7.0/tests/test_setuptools_plugin.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/tests/test_tmp_plugin.py` & `npe2-0.7.0/tests/test_tmp_plugin.py`

 * *Files identical despite different names*

### Comparing `npe2-0.6.2/tests/test_utils.py` & `npe2-0.7.0/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 
 
 def test_version():
     v = Version.parse(b"0.1.2")
 
     assert v == "0.1.2"
-    assert v > dict(major=0, minor=1, patch=0)
+    assert v > {"major": 0, "minor": 1, "patch": 0}
     assert v <= (0, 2, 0)
     assert v == Version(0, 1, 2)
     assert list(v) == [0, 1, 2, None, None]
     assert str(v) == "0.1.2"
 
     with pytest.raises(TypeError):
         assert v == 1.2
```

### Comparing `npe2-0.6.2/tests/test_validations.py` & `npe2-0.7.0/tests/test_validations.py`

 * *Files identical despite different names*

