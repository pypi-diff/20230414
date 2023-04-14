# Comparing `tmp/jupyterlab_pachyderm-2.6.0a3.tar.gz` & `tmp/jupyterlab_pachyderm-2.6.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_pachyderm-2.6.0a3.tar", last modified: Thu Mar 30 20:29:36 2023, max compression
+gzip compressed data, was "jupyterlab_pachyderm-2.6.0a5.tar", last modified: Fri Apr 14 16:43:35 2023, max compression
```

## Comparing `jupyterlab_pachyderm-2.6.0a3.tar` & `jupyterlab_pachyderm-2.6.0a5.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      749 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10656 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9679 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/babel.config.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/install.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jest.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.934847 jupyterlab_pachyderm-2.6.0a3/jupyter-config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.942847 jupyterlab_pachyderm-2.6.0a3/jupyter-config/nb-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyter-config/nb-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.942847 jupyterlab_pachyderm-2.6.0a3/jupyter-config/server-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyter-config/server-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.942847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/dev_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/env.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/filemanager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11627 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/handlers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.942847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4388 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.934847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.946847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-03-30 20:29:24.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-03-30 20:29:24.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-03-30 20:29:24.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4246 2023-03-30 20:29:24.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-03-30 20:29:24.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.946847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15787 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/747.4bacb4613a4fbdd0e8a7.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   156706 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/869.aa9313c5e001be51e97f.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8237 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/remoteEntry.8cf7225b6da9d05077a7.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-03-30 20:29:24.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/style.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/log.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6171 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/mount_server_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/pachyderm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4355 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/pps_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.946847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.946847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16212 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/test_handlers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12887 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/test_integrations.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.942847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10656 2023-03-30 20:29:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4592 2023-03-30 20:29:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-30 20:29:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-30 20:29:09.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-03-30 20:29:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-03-30 20:29:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4246 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/schema/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/schema/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/schema/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/schema/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/schema/telemetry.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      958 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/global.d.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/handler.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.938847 jupyterlab_pachyderm-2.6.0a3/src/plugins/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/__test__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/__test__/examples.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/examples.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/__tests__/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/__tests__/__snapshots__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/__tests__/help.test.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/help.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/help.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4685 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/__tests__/mount.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.938847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/Config.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/__tests__/Config.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/hooks/useConfig.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/Datum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/hooks/useDatum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/FullPageError/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/FullPageError/FullPageError.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/FullPageError/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4996 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/Pipeline.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2234 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3255 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/ListMount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/ListUnmount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3415 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/SortableList.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14680 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/customFileBrowser.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      864 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7755 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/mount.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18827 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/mount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/mountDrive.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3658 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/pollMounts.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2430 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/types.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/__tests__/telemetry.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/telemetry.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/setupTests.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/utils/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.938847 jupyterlab_pachyderm-2.6.0a3/src/utils/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Circle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Circle/Circle.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Circle/circle.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/utils/components/LoadingDots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/LoadingDots/LoadingDots.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/LoadingDots/loadingDots.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/GenericError.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/KubernetesElephant.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/PachydermLogo.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/StatusWarning.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/src/utils/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/hooks/usePreviousValue.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/hooks/useSort.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/icons.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/testUtils.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/style/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/base.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/style/components/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1415 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/components/button.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/components/input.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/style/icons/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/icons/file.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/icons/info.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/icons/mount-logo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/icons/repo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/index.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/tsconfig.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.858220 jupyterlab_pachyderm-2.6.0a5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      749 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-04-14 16:43:35.858220 jupyterlab_pachyderm-2.6.0a5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/babel.config.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/install.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jest.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.838220 jupyterlab_pachyderm-2.6.0a5/jupyter-config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.842220 jupyterlab_pachyderm-2.6.0a5/jupyter-config/nb-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyter-config/nb-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.842220 jupyterlab_pachyderm-2.6.0a5/jupyter-config/server-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyter-config/server-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.842220 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/dev_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/env.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/filemanager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11597 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/handlers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.842220 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4388 2023-04-14 16:43:33.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.838220 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/schemas/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.846220 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-04-14 16:43:24.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-04-14 16:43:24.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-04-14 16:43:24.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4246 2023-04-14 16:43:24.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-04-14 16:43:24.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.846220 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-04-14 16:43:33.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-04-14 16:43:33.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-04-14 16:43:33.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-04-14 16:43:33.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-04-14 16:43:33.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-04-14 16:43:33.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15787 2023-04-14 16:43:33.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/747.4bacb4613a4fbdd0e8a7.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   157293 2023-04-14 16:43:33.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/869.74d0c84d4f9c3908c376.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8237 2023-04-14 16:43:33.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/remoteEntry.29814ef51cca10c332b8.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-04-14 16:43:24.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/style.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-04-14 16:43:33.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/log.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6171 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/mount_server_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/pachyderm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7538 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/pps_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.850220 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      100 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.850220 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16249 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/tests/test_handlers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13603 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/tests/test_integrations.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.842220 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-04-14 16:43:35.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4592 2023-04-14 16:43:35.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-14 16:43:35.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-14 16:43:09.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-04-14 16:43:35.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-14 16:43:35.000000 jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4246 2023-04-14 16:41:22.000000 jupyterlab_pachyderm-2.6.0a5/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.850220 jupyterlab_pachyderm-2.6.0a5/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/schema/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/schema/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/schema/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/schema/telemetry.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      967 2023-04-14 16:43:35.858220 jupyterlab_pachyderm-2.6.0a5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.850220 jupyterlab_pachyderm-2.6.0a5/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/global.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/handler.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.838220 jupyterlab_pachyderm-2.6.0a5/src/plugins/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.850220 jupyterlab_pachyderm-2.6.0a5/src/plugins/examples/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.850220 jupyterlab_pachyderm-2.6.0a5/src/plugins/examples/__test__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/examples/__test__/examples.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/examples/examples.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/examples/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.850220 jupyterlab_pachyderm-2.6.0a5/src/plugins/help/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.850220 jupyterlab_pachyderm-2.6.0a5/src/plugins/help/__tests__/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.850220 jupyterlab_pachyderm-2.6.0a5/src/plugins/help/__tests__/__snapshots__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/help/__tests__/help.test.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/help/help.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/help/help.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/help/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5418 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/__tests__/mount.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.838220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Config/Config.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Config/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Config/__tests__/Config.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Config/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Config/hooks/useConfig.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Datum/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Datum/Datum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Datum/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Datum/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Datum/hooks/useDatum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/FullPageError/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/FullPageError/FullPageError.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/FullPageError/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5172 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Pipeline/Pipeline.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Pipeline/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Pipeline/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3645 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/SortableList/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/SortableList/ListMount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/SortableList/ListUnmount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3415 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/SortableList/SortableList.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/SortableList/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14680 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/customFileBrowser.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      864 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7755 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/mount.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19578 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/mount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/mountDrive.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3658 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/pollMounts.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2702 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/types.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/telemetry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/plugins/telemetry/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/telemetry/__tests__/telemetry.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/telemetry/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/plugins/telemetry/telemetry.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/setupTests.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/utils/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.838220 jupyterlab_pachyderm-2.6.0a5/src/utils/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/utils/components/Circle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/utils/components/Circle/Circle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/utils/components/Circle/circle.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.854220 jupyterlab_pachyderm-2.6.0a5/src/utils/components/LoadingDots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/utils/components/LoadingDots/LoadingDots.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/utils/components/LoadingDots/loadingDots.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.858220 jupyterlab_pachyderm-2.6.0a5/src/utils/components/Svgs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/utils/components/Svgs/GenericError.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/utils/components/Svgs/KubernetesElephant.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/utils/components/Svgs/PachydermLogo.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/utils/components/Svgs/StatusWarning.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/utils/components/Svgs/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.858220 jupyterlab_pachyderm-2.6.0a5/src/utils/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/utils/hooks/usePreviousValue.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/utils/hooks/useSort.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/utils/icons.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/src/utils/testUtils.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.858220 jupyterlab_pachyderm-2.6.0a5/style/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/style/base.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.858220 jupyterlab_pachyderm-2.6.0a5/style/components/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1415 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/style/components/button.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/style/components/input.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 16:43:35.858220 jupyterlab_pachyderm-2.6.0a5/style/icons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/style/icons/file.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/style/icons/info.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/style/icons/mount-logo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/style/icons/repo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/style/index.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/style/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-04-14 16:41:21.000000 jupyterlab_pachyderm-2.6.0a5/tsconfig.json
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/LICENSE` & `jupyterlab_pachyderm-2.6.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/MANIFEST.in` & `jupyterlab_pachyderm-2.6.0a5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/PKG-INFO` & `jupyterlab_pachyderm-2.6.0a5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: jupyterlab_pachyderm
-Version: 2.6.0a3
-Summary: A JupyterLab extension.
-Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
-Author: 
-Author-email: 
-License: BSD-3-Clause
-Keywords: jupyter,jupyterlab,jupyterlab-extension
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: <4,>=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # jupyterlab-pachyderm
 
 [![CircleCI](https://circleci.com/gh/pachyderm/jupyterlab-pachyderm/tree/main.svg?style=shield&circle-token=23e1645bde6312d903e50be2dec7073bf0bcfbd0)](https://circleci.com/gh/pachyderm/jupyterlab-pachyderm/tree/main)
 [![PyPI version](https://badge.fury.io/py/jupyterlab-pachyderm.svg)](https://pypi.org/project/jupyterlab-pachyderm)
 
 A JupyterLab extension for integrations with Pachyderm.
 
@@ -62,21 +34,20 @@
 kubectl port-forward service/pachd 30650:30650
 ```
 
 Start a bash session in the `pachyderm/notebooks-user` container from the top-level `jupyterlab-pachyderm` repo.
 
 ```
 docker run --name jupyterlab_pachyderm_frontend_dev \
-  --net=host \
-  --rm \
+  -p 8888:8888 \
   -it -e GRANT_SUDO=yes --user root \
   --device /dev/fuse --privileged \
   -v $(pwd):/home/jovyan/extension-wd \
   -w /home/jovyan/extension-wd \
-  pachyderm/notebooks-user:77ce3a1ef2c73bf34d064cd0bdb5a64262bf3280 \
+  pachyderm/notebooks-user:<latest master SHA> \
   bash
 ```
 
 If you are running the frontend container on Linux, and want to be able to talk to pachd in minikube on `grpc://localhost:30650`, use `--net=host` at the start of the the `docker run` command as shown above. If you are on macOS, you will want to remove `--net=host` as it is not supported. On macOS you can specify `grpc://host.docker.internal:30650` to get the same effect.
 
 Install the project in editable mode, and start JupyterLab
 
@@ -98,15 +69,28 @@
 
 Within container run:
 
 ```
 npm run watch
 ```
 
+Note: Once run above, you can start the dev container again in future sessions using
+
+```
+docker start <container id>
+```
+
+and then running
+
+```
+docker exec -it <container id> bash
+```
+
 Iterating on the mount server, from inside a `pachyderm` checkout:
+
 ```
 CGO_ENABLED=0 make install
 docker cp /home/luke/gocode/bin/pachctl jupyterlab_pachyderm_frontend_dev:/usr/local/bin/pachctl
 docker exec -ti jupyterlab_pachyderm_frontend_dev pkill -f pachctl
 ```
 
 ## Local Virtual Environment Setup 
@@ -216,14 +200,24 @@
 
 First make sure the server extension is enabled:
 
 ```
 jupyter server extension list 2>&1 | grep -ie "jupyterlab_pachyderm.*OK"
 ```
 
+# Install Jupyterhub locally (Sidecar mode testing)
+
+```
+helm repo add jupyterhub https://jupyterhub.github.io/helm-chart/
+helm repo update
+helm install jhub jupyterhub/jupyterhub --version 2.0.0 --values scripts/jhub-dev-helm-values.yml
+```
+
+Note: Use any username and no password to login
+
 ### API endpoints
 
 ```
 GET /repos # returns a list of all repos/branches
 GET /mounts # returns a list of all active mounts and unmounted repos/branches
 PUT /_mount # mounts a single repo
 PUT /_unmount # unmounts a single repo
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/README.md` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: jupyterlab-pachyderm
+Version: 2.6.0a5
+Summary: A JupyterLab extension.
+Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
+Author: 
+Author-email: 
+License: BSD-3-Clause
+Keywords: jupyter,jupyterlab,jupyterlab-extension
+Platform: Linux
+Platform: Mac OS X
+Platform: Windows
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Framework :: Jupyter :: JupyterLab :: 3
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
+Requires-Python: <4,>=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # jupyterlab-pachyderm
 
 [![CircleCI](https://circleci.com/gh/pachyderm/jupyterlab-pachyderm/tree/main.svg?style=shield&circle-token=23e1645bde6312d903e50be2dec7073bf0bcfbd0)](https://circleci.com/gh/pachyderm/jupyterlab-pachyderm/tree/main)
 [![PyPI version](https://badge.fury.io/py/jupyterlab-pachyderm.svg)](https://pypi.org/project/jupyterlab-pachyderm)
 
 A JupyterLab extension for integrations with Pachyderm.
 
@@ -34,21 +62,20 @@
 kubectl port-forward service/pachd 30650:30650
 ```
 
 Start a bash session in the `pachyderm/notebooks-user` container from the top-level `jupyterlab-pachyderm` repo.
 
 ```
 docker run --name jupyterlab_pachyderm_frontend_dev \
-  --net=host \
-  --rm \
+  -p 8888:8888 \
   -it -e GRANT_SUDO=yes --user root \
   --device /dev/fuse --privileged \
   -v $(pwd):/home/jovyan/extension-wd \
   -w /home/jovyan/extension-wd \
-  pachyderm/notebooks-user:77ce3a1ef2c73bf34d064cd0bdb5a64262bf3280 \
+  pachyderm/notebooks-user:<latest master SHA> \
   bash
 ```
 
 If you are running the frontend container on Linux, and want to be able to talk to pachd in minikube on `grpc://localhost:30650`, use `--net=host` at the start of the the `docker run` command as shown above. If you are on macOS, you will want to remove `--net=host` as it is not supported. On macOS you can specify `grpc://host.docker.internal:30650` to get the same effect.
 
 Install the project in editable mode, and start JupyterLab
 
@@ -70,15 +97,28 @@
 
 Within container run:
 
 ```
 npm run watch
 ```
 
+Note: Once run above, you can start the dev container again in future sessions using
+
+```
+docker start <container id>
+```
+
+and then running
+
+```
+docker exec -it <container id> bash
+```
+
 Iterating on the mount server, from inside a `pachyderm` checkout:
+
 ```
 CGO_ENABLED=0 make install
 docker cp /home/luke/gocode/bin/pachctl jupyterlab_pachyderm_frontend_dev:/usr/local/bin/pachctl
 docker exec -ti jupyterlab_pachyderm_frontend_dev pkill -f pachctl
 ```
 
 ## Local Virtual Environment Setup 
@@ -188,14 +228,24 @@
 
 First make sure the server extension is enabled:
 
 ```
 jupyter server extension list 2>&1 | grep -ie "jupyterlab_pachyderm.*OK"
 ```
 
+# Install Jupyterhub locally (Sidecar mode testing)
+
+```
+helm repo add jupyterhub https://jupyterhub.github.io/helm-chart/
+helm repo update
+helm install jhub jupyterhub/jupyterhub --version 2.0.0 --values scripts/jhub-dev-helm-values.yml
+```
+
+Note: Use any username and no password to login
+
 ### API endpoints
 
 ```
 GET /repos # returns a list of all repos/branches
 GET /mounts # returns a list of all active mounts and unmounted repos/branches
 PUT /_mount # mounts a single repo
 PUT /_unmount # unmounts a single repo
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/__init__.py` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/_version.py` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/env.py` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/env.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/handlers.py` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,24 +271,23 @@
 
 
 class PPSCreateHandler(BaseHandler):
 
     @tornado.web.authenticated
     async def get(self, path):
         """Get the pipeline spec for the specified notebook."""
-        body = self.get_json_body()
-        response = await self.pps_client.generate(path, body)
-        self.finish(response)
+        response = await self.pps_client.generate(path)
+        await self.finish(response)
 
     @tornado.web.authenticated
     async def put(self, path):
         """Create the pipeline for the specified notebook."""
         body = self.get_json_body()
         response = await self.pps_client.create(path, body)
-        self.finish(response)
+        await self.finish(response)
 
 
 def setup_handlers(web_app):
     get_logger().info(f"Using PFS_MOUNT_DIR={PFS_MOUNT_DIR}")
     web_app.settings["pfs_contents_manager"] = PFSContentsManager(PFS_MOUNT_DIR)
     web_app.settings["pachyderm_mount_client"] = MountServerClient(PFS_MOUNT_DIR)
     web_app.settings["pachyderm_pps_client"] = PPSClient()
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/package.json` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9758597883597885%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.29814ef51cca10c332b8.js'}}",*

 * * "'version'": "'2.6.0-alpha.5'"}*

```diff
@@ -67,15 +67,15 @@
                 "npm"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.8cf7225b6da9d05077a7.js",
+            "load": "static/remoteEntry.29814ef51cca10c332b8.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "jupyterlab-pachyderm:examples"
         ],
         "discovery": {
             "server": {
@@ -132,9 +132,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.0-alpha.3"
+    "version": "2.6.0-alpha.5"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.6.0-alpha.5'"}*

```diff
@@ -127,9 +127,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.0-alpha.3"
+    "version": "2.6.0-alpha.5"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/747.4bacb4613a4fbdd0e8a7.js` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/747.4bacb4613a4fbdd0e8a7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/869.aa9313c5e001be51e97f.js` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/869.74d0c84d4f9c3908c376.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunkjupyterlab_pachyderm = self.webpackChunkjupyterlab_pachyderm || []).push([
     [869], {
         1979: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => ue
             });
-            var r = a(3279),
-                n = a.n(r),
+            var n = a(3279),
+                r = a.n(n),
                 l = a(4234);
-            const s = n()((e => {
+            const s = r()((e => {
                     const t = e.target.getAttribute("data-testid");
                     t && (0, l.track)("notebook:click", {
                         clickId: t
                     })
                 }), 500, {
                     leading: !0,
                     trailing: !1
@@ -20,18 +20,18 @@
                 i = {
                     id: "jupyterlab-pachyderm:telemetry",
                     autoStart: !0,
                     activate: e => {
                         (0, l.load)("20C6D2xFLRmyFTqtvYDEgNfwcRG", "https://pachyderm-dataplane.rudderstack.com"), window.document.onclick !== s && window.document.addEventListener("click", s)
                     }
                 };
-            var c = a(9448),
+            var c = a(5344),
                 o = a(6271),
                 m = a.n(o),
-                d = a(2884);
+                d = a(3033);
             const u = e => o.createElement("svg", Object.assign({
                 xmlns: "http://www.w3.org/2000/svg",
                 xmlnsXlink: "http://www.w3.org/1999/xlink",
                 viewBox: "0 0 100 170"
             }, e), o.createElement("defs", null, o.createElement("linearGradient", {
                 id: "pachydermLogo_svg__b",
                 x1: "90.51%",
@@ -301,18 +301,18 @@
                             command: h.openDocs
                         }, {
                             command: h.contactSupport
                         }], 20))
                     })(e, t)
                 }
             };
-            var f = a(8529),
-                E = a(6848),
-                _ = a(5613),
-                g = a(3215);
+            var f = a(1467),
+                E = a(8142),
+                _ = a(8820),
+                g = a(2502);
             const v = new g.LabIcon({
                     name: "jupyterlab-pachyderm:file",
                     svgstr: '<svg  viewBox="0 0 21 31" width="21px" height="31px" xmlns="http://www.w3.org/2000/svg">\n  <path d="M.85.001C.365.055-.003.491 0 1.008v28.19c0 .556.425 1.007.95 1.007h18.98c.524 0 .949-.45.949-1.007V6.608a1.04 1.04 0 00-.277-.713l-5.299-5.6a.923.923 0 00-.662-.294H.949a.895.895 0 00-.099 0zm1.048 2.014h11.705v4.698c0 .556.425 1.007.949 1.007h4.429v20.472H1.898V2.015zm13.603 1.332l2.234 2.36h-2.234v-2.36zM4.646 12.083a.949.949 0 00-.797.549c-.154.32-.135.704.05 1.007a.935.935 0 00.846.457h6.327a.94.94 0 00.833-.499 1.06 1.06 0 000-1.015.94.94 0 00-.833-.5H4.745a.895.895 0 00-.099 0zm0 4.698a.949.949 0 00-.797.549c-.154.32-.135.705.05 1.007a.935.935 0 00.846.458h11.389a.94.94 0 00.833-.5 1.06 1.06 0 000-1.015.94.94 0 00-.833-.499H4.745a.895.895 0 00-.099 0zm0 4.699a.949.949 0 00-.797.548c-.154.321-.135.705.05 1.007a.935.935 0 00.846.458h11.389a.94.94 0 00.833-.5 1.06 1.06 0 000-1.014.94.94 0 00-.833-.5H4.745a.895.895 0 00-.099 0z" fill="#582F6B" fill-rule="nonzero"/>\n</svg>\n'
                 }),
                 k = new g.LabIcon({
                     name: "jupyterlab-pachyderm:mount-logo",
                     svgstr: '<?xml version="1.0" encoding="UTF-8"?>\n<svg width="20px" height="20px" viewBox="0 0 20 20" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">\n    <defs>\n        <path d="M14,13 L14,17.041 L10,19 L6,17.041 L6,13 L10,14.8365 L14,13 Z M10,10 L14,12.0852339 L10,14 L6,12.0852339 L10,10 Z M10.9899912,1 L10.9899912,5.72256 L12.5999411,4.16117749 L14,5.51882251 L10.7000295,8.71882251 C10.3617408,9.04686292 9.83953975,9.08786797 9.455273,8.84183766 L9.37515866,8.78472348 L9.29997054,8.71882251 L6,5.51882251 L7.40005893,4.16117749 L9.01000884,5.72256 L9.01000884,1 L10.9899912,1 Z" id="path-1"></path>\n    </defs>\n    <g id="Icons" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">\n        <g id="Icon/notebook-mount/black">\n            <rect id="Bounding-Box"  class="jp-icon3" fill-opacity="0" fill="#FFFFFF" x="0" y="0" width="20" height="20"></rect>\n            <mask id="mask-2" fill="white">\n                <use xlink:href="#path-1"></use>\n            </mask>\n            <use id="Combined-Shape" fill="#926AA1" fill-rule="nonzero" xlink:href="#path-1"></use>\n            <g class="jp-icon3" id="Group" mask="url(#mask-2)" fill="#0F1012">\n                <g id="Color">\n                    <rect x="0" y="0" width="20" height="20"></rect>\n                </g>\n            </g>\n        </g>\n    </g>\n</svg>'
@@ -320,39 +320,39 @@
                 y = (new g.LabIcon({
                     name: "jupyterlab-pachyderm:repo",
                     svgstr: '<?xml version="1.0" encoding="UTF-8"?>\n<svg width="20px" height="20px" viewBox="0 0 20 20" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">\n    <title>Icon/notebook-repo/black</title>\n    <defs>\n        <path d="M18,7 L18,15.082 L10,19 L2,15.082 L2,7 L10,10.673 L18,7 Z M10,1 L18,5.17046787 L10,9 L2,5.17046787 L10,1 Z" id="path-1"></path>\n    </defs>\n    <g id="Icons" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">\n        <g id="Icon/notebook-repo/black">\n            <mask id="mask-2" fill="white">\n                <use xlink:href="#path-1"></use>\n            </mask>\n            <use id="Combined-Shape" fill="#926AA1" fill-rule="nonzero" xlink:href="#path-1"></use>\n            <g id="Group" mask="url(#mask-2)" fill="#0F1012">\n                <g id="Color">\n                    <rect x="0" y="0" width="20" height="20"></rect>\n                </g>\n            </g>\n        </g>\n    </g>\n</svg>'
                 }), new g.LabIcon({
                     name: "jupyterlab-pachyderm:info",
                     svgstr: '<svg width="20" height="20" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"><defs><path d="M10 0c5.5228475 0 10 4.4771525 10 10s-4.4771525 10-10 10S0 15.5228475 0 10 4.4771525 0 10 0Zm0 2c-4.418278 0-8 3.581722-8 8s3.581722 8 8 8 8-3.581722 8-8-3.581722-8-8-8Zm1.52 7.76v6.672H8.48V9.76h3.04ZM10 3.568c.5546667 0 1.0026667.14666667 1.344.44.3413333.29333333.512.66933333.512 1.128 0 .48-.1706667.87733333-.512 1.192-.3413333.31466667-.7893333.472-1.344.472-.55466667 0-1.00266667-.15466667-1.344-.464-.34133333-.30933333-.512-.69333333-.512-1.152 0-.45866667.17066667-.84266667.512-1.152.34133333-.30933333.78933333-.464 1.344-.464Z" id="infoa"/></defs><g fill="none" fill-rule="evenodd"><path fill="none" d="M0 0h20v20H0z"/><mask id="infob" fill="#fff"><use xlink:href="#infoa"/></mask><use fill="#000" fill-rule="nonzero" xlink:href="#infoa"/><g mask="url(#infob)" fill="currentcolor"><path d="M0 0h20v20H0z"/></g></g></svg>'
                 }));
-            var b = function(e, t, a, r) {
-                return new(a || (a = Promise))((function(n, l) {
+            var b = function(e, t, a, n) {
+                return new(a || (a = Promise))((function(r, l) {
                     function s(e) {
                         try {
-                            c(r.next(e))
+                            c(n.next(e))
                         } catch (e) {
                             l(e)
                         }
                     }
 
                     function i(e) {
                         try {
-                            c(r.throw(e))
+                            c(n.throw(e))
                         } catch (e) {
                             l(e)
                         }
                     }
 
                     function c(e) {
                         var t;
-                        e.done ? n(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
+                        e.done ? r(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                             e(t)
                         }))).then(s, i)
                     }
-                    c((r = r.apply(e, t || [])).next())
+                    c((n = n.apply(e, t || [])).next())
                 }))
             };
             const w = [{
                     path: "examples/Intro to Pachyderm Tutorial.ipynb",
                     title: "Intro to Pachyderm",
                     command: "jupyterlab-pachyderm:open-example-intro",
                     rank: 1
@@ -364,19 +364,19 @@
                 }],
                 x = {
                     id: "jupyterlab-pachyderm:examples",
                     autoStart: !0,
                     requires: [f.ILauncher],
                     activate: (e, t) => ((e, t) => b(void 0, void 0, void 0, (function*() {
                         yield Promise.all(w.map((a => ((e, t, a) => b(void 0, void 0, void 0, (function*() {
-                            var r;
-                            (yield(r = e.path, b(void 0, void 0, void 0, (function*() {
+                            var n;
+                            (yield(n = e.path, b(void 0, void 0, void 0, (function*() {
                                 try {
                                     const e = _.ServerConnection.makeSettings();
-                                    return 200 === (yield fetch(E.URLExt.join(e.baseUrl, "api/contents", r))).status
+                                    return 200 === (yield fetch(E.URLExt.join(e.baseUrl, "api/contents", n))).status
                                 } catch (e) {
                                     return !1
                                 }
                             })))) && (t.commands.addCommand(e.command, {
                                 icon: v,
                                 label: e.title,
                                 execute: () => t.commands.execute("docmanager:open", {
@@ -386,33 +386,33 @@
                                 command: e.command,
                                 category: "Pachyderm Examples",
                                 rank: e.rank
                             }))
                         })))(a, e, t))))
                     })))(e, t)
                 };
-            var C = a(9239),
-                M = a(3619),
-                z = a(5643),
-                S = a(5679),
-                L = a(1431),
-                B = a(1840),
+            var C = a(5687),
+                M = a(7986),
+                z = a(7280),
+                S = a(1123),
+                L = a(1840),
+                B = a(8832),
                 O = a(3114);
 
-            function D(e = "", t = "GET", a = null, r = "pachyderm/v2") {
-                return n = this, l = void 0, i = function*() {
-                    const n = _.ServerConnection.makeSettings(),
-                        l = E.URLExt.join(n.baseUrl, r, e),
+            function A(e = "", t = "GET", a = null, n = "pachyderm/v2") {
+                return r = this, l = void 0, i = function*() {
+                    const r = _.ServerConnection.makeSettings(),
+                        l = E.URLExt.join(r.baseUrl, n, e),
                         s = {
                             method: t,
                             body: a ? JSON.stringify(a) : void 0
                         };
                     let i;
                     try {
-                        i = yield _.ServerConnection.makeRequest(l, s, n)
+                        i = yield _.ServerConnection.makeRequest(l, s, r)
                     } catch (e) {
                         throw new _.ServerConnection.NetworkError(e)
                     }
                     let c = yield i.text();
                     if (c.length > 0) try {
                         c = JSON.parse(c)
                     } catch (e) {
@@ -431,78 +431,78 @@
                         try {
                             c(i.next(e))
                         } catch (e) {
                             t(e)
                         }
                     }
 
-                    function r(e) {
+                    function n(e) {
                         try {
                             c(i.throw(e))
                         } catch (e) {
                             t(e)
                         }
                     }
 
                     function c(t) {
-                        var n;
-                        t.done ? e(t.value) : (n = t.value, n instanceof s ? n : new s((function(e) {
-                            e(n)
-                        }))).then(a, r)
+                        var r;
+                        t.done ? e(t.value) : (r = t.value, r instanceof s ? r : new s((function(e) {
+                            e(r)
+                        }))).then(a, n)
                     }
-                    c((i = i.apply(n, l || [])).next())
+                    c((i = i.apply(r, l || [])).next())
                 }));
-                var n, l, s, i
+                var r, l, s, i
             }
-            var A = function(e, t, a, r) {
-                return new(a || (a = Promise))((function(n, l) {
+            var D = function(e, t, a, n) {
+                return new(a || (a = Promise))((function(r, l) {
                     function s(e) {
                         try {
-                            c(r.next(e))
+                            c(n.next(e))
                         } catch (e) {
                             l(e)
                         }
                     }
 
                     function i(e) {
                         try {
-                            c(r.throw(e))
+                            c(n.throw(e))
                         } catch (e) {
                             l(e)
                         }
                     }
 
                     function c(e) {
                         var t;
-                        e.done ? n(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
+                        e.done ? r(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                             e(t)
                         }))).then(s, i)
                     }
-                    c((r = r.apply(e, t || [])).next())
+                    c((n = n.apply(e, t || [])).next())
                 }))
             };
             class N {
                 constructor(e) {
                     this._rawData = {}, this._mounted = [], this._unmounted = [], this._status = {
                         code: 999,
                         message: ""
                     }, this._config = {
                         pachd_address: "",
                         cluster_status: "INVALID"
-                    }, this._mountedSignal = new B.Signal(this), this._unmountedSignal = new B.Signal(this), this._statusSignal = new B.Signal(this), this._configSignal = new B.Signal(this), this._dataPoll = new O.n_({
+                    }, this._mountedSignal = new L.Signal(this), this._unmountedSignal = new L.Signal(this), this._statusSignal = new L.Signal(this), this._configSignal = new L.Signal(this), this._dataPoll = new O.n_({
                         auto: !0,
-                        factory: () => A(this, void 0, void 0, (function*() {
+                        factory: () => D(this, void 0, void 0, (function*() {
                             return this.getData()
                         })),
                         frequency: {
                             interval: 2e3,
                             backoff: !0,
                             max: 5e3
                         }
-                    }), this.refresh = () => A(this, void 0, void 0, (function*() {
+                    }), this.refresh = () => D(this, void 0, void 0, (function*() {
                         yield this._dataPoll.refresh(), yield this._dataPoll.tick
                     })), this.updateData = e => {
                         JSON.stringify(e) !== JSON.stringify(this._rawData) && (this._rawData = e, this.mounted = Array.from(Object.values(e.mounted)), this.unmounted = Array.from(Object.values(e.unmounted)))
                     }, this.name = e
                 }
                 get mounted() {
                     return this._mounted
@@ -540,19 +540,19 @@
                 get configSignal() {
                     return this._configSignal
                 }
                 get poll() {
                     return this._dataPoll
                 }
                 getData() {
-                    return A(this, void 0, void 0, (function*() {
+                    return D(this, void 0, void 0, (function*() {
                         try {
-                            const e = yield D("config", "GET");
+                            const e = yield A("config", "GET");
                             if (this.config = e, "INVALID" !== e.cluster_status) {
-                                const e = yield D("mounts", "GET");
+                                const e = yield A("mounts", "GET");
                                 this.status = {
                                     code: 200
                                 }, this.updateData(e)
                             }
                         } catch (e) {
                             e instanceof _.ServerConnection.ResponseError && (this.status = {
                                 code: e.response.status,
@@ -562,47 +562,47 @@
                     }))
                 }
             }
             var F = a(6057),
                 j = a(8918);
             class H {
                 constructor(e) {
-                    this._fileChanged = new B.Signal(this), this._serverSettings = _.ServerConnection.makeSettings(), this._isDisposed = !1, this._registry = e
+                    this._fileChanged = new L.Signal(this), this._serverSettings = _.ServerConnection.makeSettings(), this._isDisposed = !1, this._registry = e
                 }
                 get name() {
                     return "mount-browser"
                 }
                 get fileChanged() {
                     return this._fileChanged
                 }
                 get serverSettings() {
                     return this._serverSettings
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 get(e, t) {
-                    return a = this, r = void 0, l = function*() {
+                    return a = this, n = void 0, l = function*() {
                         try {
-                            return yield D(E.URLExt.join("pfs", e), "GET")
+                            return yield A(E.URLExt.join("pfs", e), "GET")
                         } catch (e) {
                             return console.log("/pfs not found"), {
                                 name: "",
                                 path: "",
                                 last_modified: "2022-04-26T16:28:48.015858Z",
                                 created: "2022-04-26T16:28:48.015858Z",
                                 content: [],
                                 format: "json",
                                 mimetype: "",
                                 size: void 0,
                                 writable: !0,
                                 type: "directory"
                             }
                         }
-                    }, new((n = void 0) || (n = Promise))((function(e, t) {
+                    }, new((r = void 0) || (r = Promise))((function(e, t) {
                         function s(e) {
                             try {
                                 c(l.next(e))
                             } catch (e) {
                                 t(e)
                             }
                         }
@@ -613,21 +613,21 @@
                             } catch (e) {
                                 t(e)
                             }
                         }
 
                         function c(t) {
                             var a;
-                            t.done ? e(t.value) : (a = t.value, a instanceof n ? a : new n((function(e) {
+                            t.done ? e(t.value) : (a = t.value, a instanceof r ? a : new r((function(e) {
                                 e(a)
                             }))).then(s, i)
                         }
-                        c((l = l.apply(a, r || [])).next())
+                        c((l = l.apply(a, n || [])).next())
                     }));
-                    var a, r, n, l
+                    var a, n, r, l
                 }
                 getDownloadUrl(e) {
                     throw new Error("Method not implemented.")
                 }
                 newUntitled(e) {
                     throw new Error("Method not implemented.")
                 }
@@ -655,42 +655,42 @@
                 restoreCheckpoint(e, t) {
                     return Promise.resolve()
                 }
                 deleteCheckpoint(e, t) {
                     return Promise.resolve()
                 }
                 dispose() {
-                    this.isDisposed || (this._isDisposed = !0, B.Signal.clearData(this))
+                    this.isDisposed || (this._isDisposed = !0, L.Signal.clearData(this))
                 }
             }
-            var I = function(e, t, a, r) {
-                return new(a || (a = Promise))((function(n, l) {
+            var I = function(e, t, a, n) {
+                return new(a || (a = Promise))((function(r, l) {
                     function s(e) {
                         try {
-                            c(r.next(e))
+                            c(n.next(e))
                         } catch (e) {
                             l(e)
                         }
                     }
 
                     function i(e) {
                         try {
-                            c(r.throw(e))
+                            c(n.throw(e))
                         } catch (e) {
                             l(e)
                         }
                     }
 
                     function c(e) {
                         var t;
-                        e.done ? n(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
+                        e.done ? r(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                             e(t)
                         }))).then(s, i)
                     }
-                    c((r = r.apply(e, t || [])).next())
+                    c((n = n.apply(e, t || [])).next())
                 }))
             };
             const P = () => m().createElement("div", {
                     className: "jp-dots-container"
                 }, m().createElement("div", {
                     className: "jp-dots-base",
                     role: "status",
@@ -2338,20 +2338,20 @@
                     fill: "#000",
                     filter: "url(#kubernetesElephant_svg__an)",
                     xlinkHref: "#kubernetesElephant_svg__ao"
                 }), o.createElement("use", {
                     fill: "#F69279",
                     xlinkHref: "#kubernetesElephant_svg__ao"
                 })))),
-                U = ({
+                R = ({
                     showConfig: e,
                     setShowConfig: t,
                     reposStatus: a,
-                    updateConfig: r,
-                    authConfig: n,
+                    updateConfig: n,
+                    authConfig: r,
                     refresh: l
                 }) => {
                     const {
                         addressField: s,
                         setAddressField: i,
                         errorMessage: c,
                         setErrorMessage: d,
@@ -2362,19 +2362,19 @@
                         callLogout: E,
                         shouldShowLogin: _,
                         loading: v,
                         showAdvancedOptions: k,
                         setShowAdvancedOptions: b,
                         serverCa: w,
                         setServerCa: x
-                    } = ((e, t, a, r, n, l) => {
+                    } = ((e, t, a, n, r, l) => {
                         const [s, i] = (0, o.useState)(!1), [c, m] = (0, o.useState)(""), [d, u] = (0, o.useState)(""), [h, p] = (0, o.useState)(!1), [f, E] = (0, o.useState)(!1), [_, g] = (0, o.useState)(!1), [v, k] = (0, o.useState)("");
                         (0, o.useEffect)((() => {
-                            e && (p("AUTH_ENABLED" === r.cluster_status), E("INVALID" === r.cluster_status)), u(""), m(""), k(""), g(!1)
-                        }), [e, r]);
+                            e && (p("AUTH_ENABLED" === n.cluster_status), E("INVALID" === n.cluster_status)), u(""), m(""), k(""), g(!1)
+                        }), [e, n]);
                         const y = (e => {
                             const t = (0, o.useRef)();
                             return (0, o.useEffect)((() => {
                                 t.current = e
                             })), t.current
                         })(l);
                         return (0, o.useEffect)((() => {
@@ -2387,15 +2387,15 @@
                             shouldShowAddressInput: f,
                             setShouldShowAddressInput: E,
                             updatePachdAddress: () => I(void 0, void 0, void 0, (function*() {
                                 i(!0);
                                 try {
                                     const e = c.trim();
                                     if (/^((grpc|grpcs|http|https|unix):\/\/)/.test(e)) {
-                                        const t = yield D("config", "PUT", v ? {
+                                        const t = yield A("config", "PUT", v ? {
                                             pachd_address: e,
                                             server_cas: v
                                         } : {
                                             pachd_address: e
                                         });
                                         "INVALID" === t.cluster_status ? u("Invalid address.") : (a(t), p("AUTH_ENABLED" === t.cluster_status))
                                     } else u("Cluster address should start with grpc://, grpcs://, http://, https:// or unix://")
@@ -2403,43 +2403,43 @@
                                     u("Unable to connect to cluster."), console.log(e)
                                 }
                                 i(!1)
                             })),
                             callLogin: () => I(void 0, void 0, void 0, (function*() {
                                 i(!0);
                                 try {
-                                    const e = yield D("auth/_login", "PUT");
+                                    const e = yield A("auth/_login", "PUT");
                                     if (e.auth_url) {
                                         const t = `width=500,height=500,left=${window.screenX+(window.outerWidth-500)/2},top=${window.screenY+(window.outerHeight-500)/2.5}`;
                                         window.open(e.auth_url, "", t)
                                     }
                                 } catch (e) {
                                     console.log(e)
                                 }
                                 setTimeout((() => {
                                     i(!1)
                                 }), 2e3)
                             })),
                             callLogout: () => I(void 0, void 0, void 0, (function*() {
                                 i(!0);
                                 try {
-                                    yield D("auth/_logout", "PUT"), yield n()
+                                    yield A("auth/_logout", "PUT"), yield r()
                                 } catch (e) {
                                     console.log(e)
                                 }
                                 i(!1)
                             })),
                             shouldShowLogin: h,
                             loading: s,
                             showAdvancedOptions: _,
                             setShowAdvancedOptions: g,
                             serverCa: v,
                             setServerCa: k
                         }
-                    })(e, t, r, n, l, a);
+                    })(e, t, n, r, l, a);
                     return m().createElement(m().Fragment, null, m().createElement("div", {
                         className: "pachyderm-mount-config-form-base"
                     }, 200 === a && m().createElement("div", {
                         className: "pachyderm-mount-config-back"
                     }, m().createElement("button", {
                         "data-testid": "Config__back",
                         className: "pachyderm-button-link",
@@ -2449,21 +2449,21 @@
                         className: "pachyderm-mount-icon-padding"
                     }))), m().createElement("div", {
                         className: "pachyderm-mount-config-heading"
                     }, "Pachyderm", m().createElement("span", {
                         className: "pachyderm-mount-config-subheading"
                     }, "Mount Extension")), m().createElement("div", {
                         className: "pachyderm-mount-config-address-wrapper"
-                    }, n.pachd_address && !u ? m().createElement(m().Fragment, null, m().createElement("label", {
+                    }, r.pachd_address && !u ? m().createElement(m().Fragment, null, m().createElement("label", {
                         htmlFor: "pachd",
                         className: "pachyderm-mount-config-address-label"
                     }, "Cluster Address"), m().createElement("span", {
                         "data-testid": "Config__pachdAddress",
                         className: "pachyderm-mount-config-address"
-                    }, n.pachd_address), m().createElement("button", {
+                    }, r.pachd_address), m().createElement("button", {
                         "data-testid": "Config__pachdAddressUpdate",
                         className: "pachyderm-button-link",
                         onClick: () => h(!0)
                     }, "Change Address")) : m().createElement("div", {
                         style: {
                             width: "100%",
                             display: "flex",
@@ -2474,15 +2474,15 @@
                             width: "100%",
                             display: "flex",
                             justifyContent: "space-between",
                             marginBottom: "1rem"
                         }
                     }, m().createElement("span", {
                         className: "pachyderm-mount-config-subheading"
-                    }, n.pachd_address ? "Update Configuration" : "Connect To a Cluster"), n.pachd_address && m().createElement("button", {
+                    }, r.pachd_address ? "Update Configuration" : "Connect To a Cluster"), r.pachd_address && m().createElement("button", {
                         "data-testid": "Config__pachdAddressCancel",
                         className: "pachyderm-button-link",
                         disabled: v,
                         onClick: () => {
                             d(""), i(""), x(""), h(!1), b(!1)
                         }
                     }, m().createElement(g.closeIcon.react, {
@@ -2575,50 +2575,50 @@
                     }, m().createElement("div", {
                         className: "pachyderm-mount-config-graphic-container"
                     }, m().createElement(W, {
                         width: "230px",
                         height: "230px"
                     }))))
                 };
-            var R = a(930),
-                G = a.n(R),
+            var U = a(930),
+                G = a.n(U),
                 V = a(4439),
-                $ = function(e, t, a, r) {
-                    return new(a || (a = Promise))((function(n, l) {
+                $ = function(e, t, a, n) {
+                    return new(a || (a = Promise))((function(r, l) {
                         function s(e) {
                             try {
-                                c(r.next(e))
+                                c(n.next(e))
                             } catch (e) {
                                 l(e)
                             }
                         }
 
                         function i(e) {
                             try {
-                                c(r.throw(e))
+                                c(n.throw(e))
                             } catch (e) {
                                 l(e)
                             }
                         }
 
                         function c(e) {
                             var t;
-                            e.done ? n(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
+                            e.done ? r(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                                 e(t)
                             }))).then(s, i)
                         }
-                        c((r = r.apply(e, t || [])).next())
+                        c((n = n.apply(e, t || [])).next())
                     }))
                 };
             const T = ({
                 showDatum: e,
                 setShowDatum: t,
                 keepMounted: a,
-                setKeepMounted: r,
-                open: n,
+                setKeepMounted: n,
+                open: r,
                 pollRefresh: l,
                 currentDatumInfo: s,
                 repoViewInputSpec: i
             }) => {
                 const c = (0, o.useRef)(null),
                     {
                         loading: d,
@@ -2629,15 +2629,15 @@
                         inputSpec: E,
                         setInputSpec: v,
                         callMountDatums: k,
                         callUnmountAll: y,
                         errorMessage: b,
                         saveInputSpec: w,
                         initialInputSpec: x
-                    } = ((e, t, a, r, n, l, s) => {
+                    } = ((e, t, a, n, r, l, s) => {
                         const [i, c] = (0, o.useState)(!1), [m, d] = (0, o.useState)(!1), [u, h] = (0, o.useState)(-1), [p, f] = (0, o.useState)({
                             id: "",
                             idx: -1,
                             num_datums: 0
                         }), [E, g] = (0, o.useState)(""), [v, k] = (0, o.useState)({}), [y, b] = (0, o.useState)(""), [w, x] = (0, o.useState)({});
                         (0, o.useEffect)((() => {
                             e && -1 !== u && z()
@@ -2671,25 +2671,25 @@
                                 } catch (t) {
                                     return G().stringify(e, null, 2)
                                 }
                             },
                             z = () => $(void 0, void 0, void 0, (function*() {
                                 c(!0);
                                 try {
-                                    const e = yield D(`_show_datum?idx=${u}`, "PUT");
-                                    r(""), f(e)
+                                    const e = yield A(`_show_datum?idx=${u}`, "PUT");
+                                    n(""), f(e)
                                 } catch (e) {
                                     console.log(e)
                                 }
                                 c(!1)
                             })),
                             S = () => $(void 0, void 0, void 0, (function*() {
                                 c(!0);
                                 try {
-                                    r(""), yield D("_unmount_all", "PUT"), r(""), yield n(), h(-1), f({
+                                    n(""), yield A("_unmount_all", "PUT"), n(""), yield r(), h(-1), f({
                                         id: "",
                                         idx: -1,
                                         num_datums: 0
                                     }), d(!1)
                                 } catch (e) {
                                     console.log(e)
                                 }
@@ -2703,18 +2703,18 @@
                             setCurrIdx: h,
                             inputSpec: E,
                             setInputSpec: g,
                             callMountDatums: () => $(void 0, void 0, void 0, (function*() {
                                 c(!0), b("");
                                 try {
                                     const e = C(),
-                                        t = yield D("_mount_datums", "PUT", {
+                                        t = yield A("_mount_datums", "PUT", {
                                             input: e
                                         });
-                                    r(""), h(0), f(t), d(!0), g(M(e))
+                                    n(""), h(0), f(t), d(!0), g(M(e))
                                 } catch (e) {
                                     console.log(e), e instanceof G().YAMLParseError ? b("Poorly formatted input spec- must be either YAML or JSON") : e instanceof _.ServerConnection.ResponseError ? b("Bad data in input spec") : b("Error mounting datums")
                                 }
                                 c(!1)
                             })),
                             callUnmountAll: S,
                             errorMessage: y,
@@ -2725,51 +2725,51 @@
                                 } catch (e) {
                                     if (!(e instanceof G().YAMLParseError)) throw e;
                                     x(E)
                                 }
                             },
                             initialInputSpec: v
                         }
-                    })(e, a, r, n, l, i, s);
+                    })(e, a, n, r, l, i, s);
                 return m().createElement("div", {
                     className: "pachyderm-mount-datum-base"
                 }, m().createElement("div", {
                     className: "pachyderm-mount-datum-back"
                 }, m().createElement("button", {
                     "data-testid": "Datum__back",
                     className: "pachyderm-button-link",
                     onClick: () => {
                         return e = void 0, a = void 0, l = function*() {
-                            yield y(), w(), r(!1), yield t(!1)
-                        }, new((n = void 0) || (n = Promise))((function(t, r) {
+                            yield y(), w(), n(!1), yield t(!1)
+                        }, new((r = void 0) || (r = Promise))((function(t, n) {
                             function s(e) {
                                 try {
                                     c(l.next(e))
                                 } catch (e) {
-                                    r(e)
+                                    n(e)
                                 }
                             }
 
                             function i(e) {
                                 try {
                                     c(l.throw(e))
                                 } catch (e) {
-                                    r(e)
+                                    n(e)
                                 }
                             }
 
                             function c(e) {
                                 var a;
-                                e.done ? t(e.value) : (a = e.value, a instanceof n ? a : new n((function(e) {
+                                e.done ? t(e.value) : (a = e.value, a instanceof r ? a : new r((function(e) {
                                     e(a)
                                 }))).then(s, i)
                             }
                             c((l = l.apply(e, a || [])).next())
                         }));
-                        var e, a, n, l
+                        var e, a, r, l
                     }
                 }, "Back", " ", m().createElement(g.closeIcon.react, {
                     tag: "span",
                     className: "pachyderm-mount-icon-padding"
                 }))), m().createElement("span", {
                     className: "pachyderm-mount-datum-subheading"
                 }, "Test Datums"), m().createElement("div", {
@@ -2793,18 +2793,18 @@
                 }), m().createElement("span", {
                     className: "pachyderm-mount-datum-error",
                     "data-testid": "Datum__errorMessage"
                 }, b), m().createElement("span", {
                     className: "pachyderm-mount-datum-info",
                     "data-testid": "Datum__infoMessage"
                 }, ! function(e) {
-                    const [t, a] = (0, o.useState)(!1), r = (0, o.useMemo)((() => new IntersectionObserver((([e]) => a(e.isIntersecting)))), [e]);
+                    const [t, a] = (0, o.useState)(!1), n = (0, o.useMemo)((() => new IntersectionObserver((([e]) => a(e.isIntersecting)))), [e]);
                     return (0, o.useEffect)((() => {
-                        if (e.current) return r.observe(e.current), () => {
-                            r.disconnect()
+                        if (e.current) return n.observe(e.current), () => {
+                            n.disconnect()
                         }
                     })), t
                 }(c) && u && "Drag line below to show datum cycler"), m().createElement("button", {
                     "data-testid": "Datum__mountDatums",
                     className: "pachyderm-button-link",
                     onClick: k,
                     style: {
@@ -2836,295 +2836,304 @@
                         p < h.num_datums - 1 && f(p + 1)
                     }
                 }, m().createElement(g.caretRightIcon.react, {
                     tag: "span",
                     className: "pachyderm-mount-datum-right"
                 }))))))
             };
-            var Z = function(e, t, a, r) {
-                return new(a || (a = Promise))((function(n, l) {
+            var Z = function(e, t, a, n) {
+                return new(a || (a = Promise))((function(r, l) {
                     function s(e) {
                         try {
-                            c(r.next(e))
+                            c(n.next(e))
                         } catch (e) {
                             l(e)
                         }
                     }
 
                     function i(e) {
                         try {
-                            c(r.throw(e))
+                            c(n.throw(e))
                         } catch (e) {
                             l(e)
                         }
                     }
 
                     function c(e) {
                         var t;
-                        e.done ? n(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
+                        e.done ? r(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                             e(t)
                         }))).then(s, i)
                     }
-                    c((r = r.apply(e, t || [])).next())
+                    c((n = n.apply(e, t || [])).next())
                 }))
             };
             const J = ({
-                    setShowPipeline: e,
-                    notebookPath: t,
-                    saveNotebookMetadata: a,
-                    metadata: r
+                    ppsContext: e,
+                    setShowPipeline: t,
+                    saveNotebookMetadata: a
                 }) => {
                     const {
                         loading: n,
-                        pipelineName: l,
-                        setPipelineName: s,
-                        imageName: i,
-                        setImageName: c,
-                        inputSpec: d,
-                        setInputSpec: u,
-                        requirements: h,
-                        setRequirements: p,
-                        callCreatePipeline: f,
-                        callSavePipeline: E,
-                        errorMessage: v
-                    } = ((e, t, a) => {
-                        const [r, n] = (0, o.useState)(!1), [l, s] = (0, o.useState)(""), [i, c] = (0, o.useState)(""), [m, d] = (0, o.useState)(""), [u, h] = (0, o.useState)(""), [p, f] = (0, o.useState)("");
-                        (0, o.useEffect)((() => {
-                            var t, a, r;
-                            if (c(null !== (t = null == e ? void 0 : e.environments.default.image_tag) && void 0 !== t ? t : ""), s(null !== (a = null == e ? void 0 : e.metadata.name) && void 0 !== a ? a : ""), h(null !== (r = null == e ? void 0 : e.notebook.requirements) && void 0 !== r ? r : ""), null == e ? void 0 : e.run.input) {
-                                const t = JSON.parse(null == e ? void 0 : e.run.input);
-                                d(G().stringify(t))
-                            } else d("")
-                        }), [e]);
-                        const E = () => {
-                            let e;
-                            try {
-                                e = G().parse(m)
-                            } catch (t) {
-                                if (!(t instanceof G().YAMLParseError)) throw t;
-                                e = JSON.parse(m)
-                            }
-                            return {
-                                apiVersion: "sameproject.ml/v1alpha1",
-                                environments: {
-                                    default: {
-                                        image_tag: i
-                                    }
-                                },
-                                metadata: {
-                                    name: l,
-                                    version: "0.0.0"
-                                },
-                                notebook: {
-                                    requirements: u
-                                },
-                                run: {
-                                    name: l,
-                                    input: JSON.stringify(e)
-                                }
-                            }
-                        };
-                        return {
-                            loading: r,
-                            pipelineName: l,
-                            setPipelineName: s,
-                            imageName: i,
-                            setImageName: c,
-                            inputSpec: m,
-                            setInputSpec: d,
-                            requirements: u,
-                            setRequirements: h,
-                            callCreatePipeline: () => Z(void 0, void 0, void 0, (function*() {
-                                n(!0), f("");
-                                const e = E();
+                        pipelineName: r,
+                        setPipelineName: l,
+                        imageName: s,
+                        setImageName: i,
+                        inputSpec: c,
+                        setInputSpec: d,
+                        requirements: u,
+                        setRequirements: h,
+                        callCreatePipeline: p,
+                        callSavePipeline: f,
+                        errorMessage: E,
+                        responseMessage: v
+                    } = ((e, t) => {
+                        const [a, n] = (0, o.useState)(!1), [r, l] = (0, o.useState)(""), [s, i] = (0, o.useState)(""), [c, m] = (0, o.useState)(""), [d, u] = (0, o.useState)(""), [h, p] = (0, o.useState)(""), [f, E] = (0, o.useState)("");
+                        let g;
+                        if ((0, o.useEffect)((() => {
+                                var t, a, n, r, s, c, o;
+                                if (i(null !== (a = null === (t = null == e ? void 0 : e.config) || void 0 === t ? void 0 : t.environments.default.image_tag) && void 0 !== a ? a : ""), l(null !== (r = null === (n = null == e ? void 0 : e.config) || void 0 === n ? void 0 : n.metadata.name) && void 0 !== r ? r : ""), u(null !== (c = null === (s = null == e ? void 0 : e.config) || void 0 === s ? void 0 : s.notebook.requirements) && void 0 !== c ? c : ""), E(""), null === (o = null == e ? void 0 : e.config) || void 0 === o ? void 0 : o.run.input) {
+                                    const t = JSON.parse(e.config.run.input);
+                                    m(G().stringify(t))
+                                } else m("")
+                            }), [e]), null == e ? void 0 : e.notebookModel) {
+                            const t = e.notebookModel;
+                            g = () => Z(void 0, void 0, void 0, (function*() {
+                                n(!0), p(""), E("");
                                 try {
-                                    yield D(`pps/_create/${t}`, "PUT", e)
+                                    const e = yield A(`pps/_create/${encodeURI(t.path)}`, "PUT", {
+                                        last_modified_time: t.last_modified
+                                    });
+                                    null !== e.message && E(e.message)
                                 } catch (e) {
                                     if (!(e instanceof _.ServerConnection.ResponseError)) throw e;
-                                    f(e.message)
+                                    p(e.message)
                                 }
-                                console.log("create pipeline called"), n(!1)
-                            })),
+                                n(!1)
+                            }))
+                        } else g = () => Z(void 0, void 0, void 0, (function*() {
+                            p("Error: No notebook in focus")
+                        }));
+                        return {
+                            loading: a,
+                            pipelineName: r,
+                            setPipelineName: l,
+                            imageName: s,
+                            setImageName: i,
+                            inputSpec: c,
+                            setInputSpec: m,
+                            requirements: d,
+                            setRequirements: u,
+                            callCreatePipeline: g,
                             callSavePipeline: () => Z(void 0, void 0, void 0, (function*() {
-                                const e = E();
-                                a(e), console.log("save pipeline called")
+                                let e;
+                                try {
+                                    e = G().parse(c)
+                                } catch (t) {
+                                    if (!(t instanceof G().YAMLParseError)) throw t;
+                                    e = JSON.parse(c)
+                                }
+                                const a = {
+                                    apiVersion: "sameproject.ml/v1alpha1",
+                                    environments: {
+                                        default: {
+                                            image_tag: s
+                                        }
+                                    },
+                                    metadata: {
+                                        name: r,
+                                        version: "0.0.0"
+                                    },
+                                    notebook: {
+                                        requirements: d
+                                    },
+                                    run: {
+                                        name: r,
+                                        input: JSON.stringify(e)
+                                    }
+                                };
+                                t(a)
                             })),
-                            errorMessage: p
+                            errorMessage: h,
+                            responseMessage: f
                         }
-                    })(r, t, a);
+                    })(e, a);
                     return m().createElement("div", {
                         className: "pachyderm-mount-pipeline-base"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-pipeline-back"
                     }, m().createElement("button", {
                         "data-testid": "Pipeline__back",
                         className: "pachyderm-button-link",
                         onClick: () => {
-                            return t = void 0, a = void 0, n = function*() {
-                                e(!1)
-                            }, new((r = void 0) || (r = Promise))((function(e, l) {
+                            return e = void 0, a = void 0, r = function*() {
+                                t(!1)
+                            }, new((n = void 0) || (n = Promise))((function(t, l) {
                                 function s(e) {
                                     try {
-                                        c(n.next(e))
+                                        c(r.next(e))
                                     } catch (e) {
                                         l(e)
                                     }
                                 }
 
                                 function i(e) {
                                     try {
-                                        c(n.throw(e))
+                                        c(r.throw(e))
                                     } catch (e) {
                                         l(e)
                                     }
                                 }
 
-                                function c(t) {
+                                function c(e) {
                                     var a;
-                                    t.done ? e(t.value) : (a = t.value, a instanceof r ? a : new r((function(e) {
+                                    e.done ? t(e.value) : (a = e.value, a instanceof n ? a : new n((function(e) {
                                         e(a)
                                     }))).then(s, i)
                                 }
-                                c((n = n.apply(t, a || [])).next())
+                                c((r = r.apply(e, a || [])).next())
                             }));
-                            var t, a, r, n
+                            var e, a, n, r
                         }
                     }, "Back", " ", m().createElement(g.closeIcon.react, {
                         tag: "span",
                         className: "pachyderm-mount-icon-padding"
                     }))), m().createElement("span", {
                         className: "pachyderm-mount-pipeline-subheading"
                     }, "Notebook-to-Pipeline"), m().createElement("div", {
                         className: "pachyderm-pipeline-buttons"
                     }, m().createElement("button", {
                         "data-testid": "Pipeline__save",
                         className: "pachyderm-button-link",
-                        onClick: E
+                        onClick: f
                     }, "Save"), m().createElement("button", {
                         "data-testid": "Pipeline__create_pipeline",
                         className: "pachyderm-button-link",
-                        onClick: f
+                        onClick: p
                     }, "Create Pipeline")), m().createElement("span", {
                         className: "pachyderm-pipeline-error",
                         "data-testid": "Pipeline__errorMessage"
+                    }, E), m().createElement("span", {
+                        className: "pachyderm-pipeline-response",
+                        "data-testid": "Pipeline__responseMessage"
                     }, v), m().createElement("div", {
                         className: "pachyderm-pipeline-input-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-input-label",
                         htmlFor: "pipelineName"
-                    }, "*Name:", "  "), m().createElement("input", {
+                    }, "*Pipeline Name:", "  "), m().createElement("input", {
                         className: "pachyderm-pipeline-input",
                         "data-testid": "Pipeline__inputPipelineName",
                         name: "pipelineName",
-                        value: l,
+                        value: r,
                         onChange: e => {
-                            s(e.target.value)
+                            l(e.target.value)
                         },
                         disabled: n
                     })), m().createElement("div", {
                         className: "pachyderm-pipeline-input-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-input-label",
                         htmlFor: "imageName"
-                    }, "*Image:", "  "), m().createElement("input", {
+                    }, "*Container Image Name:", "  "), m().createElement("input", {
                         className: "pachyderm-pipeline-input",
                         "data-testid": "Pipeline__inputImageName",
                         name: "imageName",
-                        value: i,
+                        value: s,
                         onChange: e => {
-                            c(e.target.value)
+                            i(e.target.value)
                         },
                         disabled: n
                     })), m().createElement("div", {
                         className: "pachyderm-pipeline-input-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-input-label",
                         htmlFor: "requirements"
-                    }, "Requirements:", "  "), m().createElement("input", {
+                    }, "Requirements File:", "  "), m().createElement("input", {
                         className: "pachyderm-pipeline-input",
                         "data-testid": "Pipeline__inputRequirements",
                         name: "requirements",
-                        value: h,
+                        value: u,
                         onChange: e => {
-                            p(e.target.value)
+                            h(e.target.value)
                         },
                         disabled: n,
                         placeholder: "./requirements.txt"
                     })), m().createElement("div", {
                         className: "pachyderm-pipeline-textarea-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-textarea-label",
                         htmlFor: "inputSpec"
-                    }, "Input Spec"), m().createElement("textarea", {
+                    }, "Pipeline Input Spec:"), m().createElement("textarea", {
                         className: "pachyderm-pipeline-textarea pachyderm-input",
                         "data-testid": "Pipeline__inputSpecInput",
                         name: "inputSpec",
-                        value: d,
+                        value: c,
                         onChange: e => {
-                            u(e.target.value)
+                            d(e.target.value)
                         },
                         disabled: n,
                         placeholder: "pfs:\n  repo: images\n  branch: dev\n  glob: /*\n"
                     })), m().createElement("div", {
                         className: "pachyderm-pipeline-spec-preview pachyderm-pipeline-textarea-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-preview-label"
                     }, "Pipeline Spec Preview: ", "  "), m().createElement("textarea", {
                         className: "pachyderm-pipeline-spec-preview-textarea",
                         style: {
                             backgroundColor: "#80808080"
                         },
                         "data-testid": "Pipeline__specPreview",
                         name: "specPreview",
-                        value: `name: ${l}\ntransform:\n  image: ${i}\ninput:\n${d.split("\n").map(((e,t,a)=>"  "+e)).join("\n")}\n`,
+                        value: `name: ${r}\ntransform:\n  image: ${s}\ninput:\n${c.split("\n").map(((e,t,a)=>"  "+e)).join("\n")}\n`,
                         readOnly: !0
                     })))
                 },
                 q = (e, t) => e > t ? 1 : e < t ? -1 : 0,
                 Y = (e, t) => e - t;
             var X = a(4184),
                 K = a.n(X);
             const Q = e => {
                 var {
                     children: t,
                     className: a,
-                    color: r = "gray"
-                } = e, n = function(e, t) {
+                    color: n = "gray"
+                } = e, r = function(e, t) {
                     var a = {};
-                    for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (a[r] = e[r]);
+                    for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
                     if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
-                        var n = 0;
-                        for (r = Object.getOwnPropertySymbols(e); n < r.length; n++) t.indexOf(r[n]) < 0 && Object.prototype.propertyIsEnumerable.call(e, r[n]) && (a[r[n]] = e[r[n]])
+                        var r = 0;
+                        for (n = Object.getOwnPropertySymbols(e); r < n.length; r++) t.indexOf(n[r]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[r]) && (a[n[r]] = e[n[r]])
                     }
                     return a
                 }(e, ["children", "className", "color"]);
                 const l = K()("jp-circle-base", a, {
-                    "jp-circle-green": "green" === r,
-                    "jp-circle-red": "red" === r,
-                    "jp-circle-yellow": "yellow" === r,
-                    "jp-circle-gray": "gray" === r
+                    "jp-circle-green": "green" === n,
+                    "jp-circle-red": "red" === n,
+                    "jp-circle-yellow": "yellow" === n,
+                    "jp-circle-gray": "gray" === n
                 });
                 return m().createElement("div", Object.assign({
                     className: l
-                }, n), t)
+                }, r), t)
             };
             const ee = ["unmounting", "mounting", "error"],
                 te = ({
                     item: e,
                     open: t,
                     updateData: a
                 }) => {
-                    const [r, n] = (0, o.useState)(!1), l = e.branch, s = "Unmount", i = e.how_many_commits_behind;
+                    const [n, r] = (0, o.useState)(!1), l = e.branch, s = "Unmount", i = e.how_many_commits_behind;
                     return (0, o.useEffect)((() => {
-                        n(ee.includes(e.state))
+                        r(ee.includes(e.state))
                     }), [e]), m().createElement("li", {
                         className: "pachyderm-mount-sortableList-item",
                         "data-testid": "ListItem__repo"
                     }, m().createElement("span", {
-                        className: "pachyderm-mount-list-item-name-branch-wrapper " + (r ? "pachyderm-mount-sortableList-disabled" : ""),
+                        className: "pachyderm-mount-list-item-name-branch-wrapper " + (n ? "pachyderm-mount-sortableList-disabled" : ""),
                         onClick: () => {
                             t(e.name)
                         }
                     }, m().createElement("span", {
                         className: "pachyderm-mount-list-item-name",
                         title: e.name
                     }, e.name), m().createElement("span", {
@@ -3135,28 +3144,28 @@
                         style: {
                             marginLeft: "7px"
                         },
                         "data-testid": "ListItem__commitBehindness"
                     }, (e => 0 === e ? m().createElement("span", null, "✅ up to date") : 1 === e ? m().createElement("span", null, "⌛ ", e, " commit behind") : m().createElement("span", null, "⌛ ", e, " commits behind"))(i))))), m().createElement("span", {
                         className: "pachyderm-mount-list-item-action"
                     }, m().createElement("button", {
-                        disabled: r,
+                        disabled: n,
                         onClick: () => {
-                            return t = void 0, r = void 0, s = function*() {
-                                n(!0);
+                            return t = void 0, n = void 0, s = function*() {
+                                r(!0);
                                 try {
-                                    const t = yield D("_unmount", "PUT", {
+                                    const t = yield A("_unmount", "PUT", {
                                         mounts: [`${e.name}`]
                                     });
                                     a(t)
                                 } catch (e) {
                                     console.log("error unmounting repo")
                                 }
                             }, new((l = void 0) || (l = Promise))((function(e, a) {
-                                function n(e) {
+                                function r(e) {
                                     try {
                                         c(s.next(e))
                                     } catch (e) {
                                         a(e)
                                     }
                                 }
 
@@ -3168,64 +3177,64 @@
                                     }
                                 }
 
                                 function c(t) {
                                     var a;
                                     t.done ? e(t.value) : (a = t.value, a instanceof l ? a : new l((function(e) {
                                         e(a)
-                                    }))).then(n, i)
+                                    }))).then(r, i)
                                 }
-                                c((s = s.apply(t, r || [])).next())
+                                c((s = s.apply(t, n || [])).next())
                             }));
-                            var t, r, l, s
+                            var t, n, l, s
                         },
                         className: "pachyderm-button-link",
                         "data-testid": `ListItem__${s.toLowerCase()}`
                     }, s), m().createElement("span", {
                         className: "pachyderm-mount-list-item-status",
                         "data-testid": "ListItem__status"
                     }, ((e, t) => {
                         let a = "gray",
-                            r = "";
+                            n = "";
                         switch (e) {
                             case "mounted":
                                 a = "green";
                                 break;
                             case "unmounting":
                             case "mounting":
                                 a = "yellow";
                                 break;
                             case "error":
                                 a = "red"
                         }
-                        return r = t ? `${(0,V.capitalize)(e||"Unknown")}: ${t}` : (0, V.capitalize)(e || "Unknown"), m().createElement(m().Fragment, null, m().createElement(Q, {
+                        return n = t ? `${(0,V.capitalize)(e||"Unknown")}: ${t}` : (0, V.capitalize)(e || "Unknown"), m().createElement(m().Fragment, null, m().createElement(Q, {
                             color: a,
                             className: "pachyderm-mount-list-item-status-circle"
                         }), m().createElement("div", {
                             "data-testid": "ListItem__statusIcon",
                             className: "pachyderm-mount-list-item-status-icon",
-                            title: r
+                            title: n
                         }, m().createElement(y.react, {
                             tag: "span"
                         })))
                     })(e.state, e.status))))
                 };
             const ae = ({
                     item: e,
                     updateData: t,
                     mountedItems: a
                 }) => {
-                    var r;
-                    const [n, l] = (0, o.useState)(""), [s, i] = (0, o.useState)(!1), [c, d] = (0, o.useState)(!1), [u, h] = (0, o.useState)(!1), p = (null === (r = null == e ? void 0 : e.branches) || void 0 === r ? void 0 : r.length) > 0, f = "Mount";
+                    var n;
+                    const [r, l] = (0, o.useState)(""), [s, i] = (0, o.useState)(!1), [c, d] = (0, o.useState)(!1), [u, h] = (0, o.useState)(!1), p = (null === (n = null == e ? void 0 : e.branches) || void 0 === n ? void 0 : n.length) > 0, f = "Mount";
                     return (0, o.useEffect)((() => {
                         h("none" !== e.authorization)
                     }), [e]), (0, o.useEffect)((() => {
-                        const t = a.find((t => t.repo === e.repo && t.project === e.project && t.branch === n));
+                        const t = a.find((t => t.repo === e.repo && t.project === e.project && t.branch === r));
                         i(!!t)
-                    }), [a, n]), (0, o.useEffect)((() => {
+                    }), [a, r]), (0, o.useEffect)((() => {
                         if (p) {
                             const t = e.branches.find((e => "master" === e));
                             l(t || e.branches[0]), d(!1)
                         }
                     }), [e]), u ? p ? m().createElement("li", {
                         className: "pachyderm-mount-sortableList-item",
                         "data-testid": "ListItem__repo"
@@ -3235,48 +3244,48 @@
                         className: "pachyderm-mount-list-item-name",
                         title: `${e.project}_${e.repo}`
                     }, `${e.project}_${e.repo}`), m().createElement("span", {
                         className: "pachyderm-mount-list-item-branch"
                     }, m().createElement(m().Fragment, null, m().createElement("span", null, "@ "), m().createElement("select", {
                         disabled: c,
                         name: "branch",
-                        value: n,
+                        value: r,
                         className: "pachyderm-mount-list-item-branch-select",
                         onChange: e => {
                             l(e.target.value)
                         },
                         "data-testid": "ListItem__select"
                     }, e.branches.map((e => m().createElement("option", {
                         key: e,
                         value: e
                     }, e))))))), m().createElement("span", {
                         className: "pachyderm-mount-list-item-action"
                     }, m().createElement("button", {
                         disabled: c || s,
                         onClick: () => {
-                            return a = void 0, r = void 0, s = function*() {
+                            return a = void 0, n = void 0, s = function*() {
                                 d(!0);
                                 try {
-                                    if (n) {
-                                        const a = yield D("_mount", "PUT", {
+                                    if (r) {
+                                        const a = yield A("_mount", "PUT", {
                                             mounts: [{
-                                                name: "master" === n ? `${e.project}_${e.repo}` : `${e.project}_${e.repo}_${n}`,
+                                                name: "master" === r ? `${e.project}_${e.repo}` : `${e.project}_${e.repo}_${r}`,
                                                 repo: e.repo,
-                                                branch: n,
+                                                branch: r,
                                                 project: e.project,
                                                 mode: "ro"
                                             }]
                                         });
                                         t(a)
                                     }
                                 } catch (e) {
                                     console.log("error mounting or unmounting repo")
                                 }
                             }, new((l = void 0) || (l = Promise))((function(e, t) {
-                                function n(e) {
+                                function r(e) {
                                     try {
                                         c(s.next(e))
                                     } catch (e) {
                                         t(e)
                                     }
                                 }
 
@@ -3288,19 +3297,19 @@
                                     }
                                 }
 
                                 function c(t) {
                                     var a;
                                     t.done ? e(t.value) : (a = t.value, a instanceof l ? a : new l((function(e) {
                                         e(a)
-                                    }))).then(n, i)
+                                    }))).then(r, i)
                                 }
-                                c((s = s.apply(a, r || [])).next())
+                                c((s = s.apply(a, n || [])).next())
                             }));
-                            var a, r, l, s
+                            var a, n, l, s
                         },
                         className: "pachyderm-button-link",
                         "data-testid": `ListItem__${f.toLowerCase()}`
                     }, f))) : m().createElement("li", {
                         className: "pachyderm-mount-sortableList-item",
                         "data-testid": "ListItem__noBranches",
                         title: "Repo doesn't have a branch"
@@ -3323,25 +3332,25 @@
                     }, m().createElement("span", {
                         className: "pachyderm-mount-list-item-name",
                         title: `${e.project}_${e.repo}`
                     }, `${e.project}_${e.repo}`), m().createElement("span", {
                         className: "pachyderm-mount-list-item-branch"
                     }, "No read access")))
                 },
-                re = {
+                ne = {
                     name: "Name",
                     func: q,
                     accessor: e => "name" in e ? e.name : `${e.project}_${e.repo}`
                 },
-                ne = ({
+                re = ({
                     open: e,
                     items: t,
                     updateData: a,
-                    mountedItems: r,
-                    type: n
+                    mountedItems: n,
+                    type: r
                 }) => {
                     const l = "All projects",
                         s = [...new Set(t.map((e => e.project)))],
                         [i, c] = (0, o.useState)(l),
                         {
                             sortedData: d,
                             setComparator: u,
@@ -3351,36 +3360,36 @@
                             initialSort: t = {
                                 func: () => 1,
                                 name: "",
                                 accessor: e => e
                             },
                             initialDirection: a = 1
                         }) => {
-                            const [r, n] = (0, o.useState)(a), [l, s] = (0, o.useState)(t), i = (0, o.useCallback)((e => {
-                                s((t => (e.name === t.name || e.reverse ? n(-1 * r) : n(1), e)))
-                            }), [r]);
+                            const [n, r] = (0, o.useState)(a), [l, s] = (0, o.useState)(t), i = (0, o.useCallback)((e => {
+                                s((t => (e.name === t.name || e.reverse ? r(-1 * n) : r(1), e)))
+                            }), [n]);
                             return {
-                                sortedData: (0, o.useMemo)((() => [...e].sort(((e, t) => r * l.func(l.accessor(e), l.accessor(t))))), [l, e, r]),
-                                reversed: -1 === r,
+                                sortedData: (0, o.useMemo)((() => [...e].sort(((e, t) => n * l.func(l.accessor(e), l.accessor(t))))), [l, e, n]),
+                                reversed: -1 === n,
                                 setComparator: i,
                                 comparatorName: l.name,
                                 numberComparator: Y,
                                 stringComparator: q
                             }
                         })({
                             data: t,
-                            initialSort: re,
+                            initialSort: ne,
                             initialDirection: 1
                         }),
                         p = (0, o.useCallback)((() => {
-                            u(re)
+                            u(ne)
                         }), [u]);
                     return m().createElement("div", {
                         className: "pachyderm-mount-sortableList"
-                    }, "unmounted" === n && m().createElement("div", {
+                    }, "unmounted" === r && m().createElement("div", {
                         className: "pachyderm-mount-sortableList-projectFilter"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-projectFilter-headerItem"
                     }, m().createElement("span", null, "Project: "), m().createElement("select", {
                         name: "project",
                         value: i,
                         className: "pachyderm-mount-project-list-select",
@@ -3406,15 +3415,15 @@
                         key: t.name,
                         open: e,
                         updateData: a
                     }) : (i === t.project || i === l) && m().createElement(ae, {
                         item: t,
                         key: `${t.project}_${t.repo}`,
                         updateData: a,
-                        mountedItems: r
+                        mountedItems: n
                     })))))
                 },
                 le = e => o.createElement("svg", Object.assign({
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 400,
                     height: 180,
                     viewBox: "320 -20 180 270",
@@ -3973,56 +3982,64 @@
                 }, m().createElement(se, null), m().createElement("span", {
                     style: {
                         paddingLeft: ".5rem"
                     }
                 }, "Looks like there was an error")), m().createElement("div", {
                     "data-testid": "FullPageError__message"
                 }, e.message));
-            var ce = function(e, t, a, r) {
-                return new(a || (a = Promise))((function(n, l) {
+            var ce = function(e, t, a, n) {
+                return new(a || (a = Promise))((function(r, l) {
                     function s(e) {
                         try {
-                            c(r.next(e))
+                            c(n.next(e))
                         } catch (e) {
                             l(e)
                         }
                     }
 
                     function i(e) {
                         try {
-                            c(r.throw(e))
+                            c(n.throw(e))
                         } catch (e) {
                             l(e)
                         }
                     }
 
                     function c(e) {
                         var t;
-                        e.done ? n(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
+                        e.done ? r(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                             e(t)
                         }))).then(s, i)
                     }
-                    c((r = r.apply(e, t || [])).next())
+                    c((n = n.apply(e, t || [])).next())
                 }))
             };
             const oe = "mount-browser:",
                 me = "same_config";
             class de {
-                constructor(e, t, a, r, n) {
-                    this._showConfig = !1, this._showConfigSignal = new B.Signal(this), this._readyPromise = Promise.resolve(), this._showDatum = !1, this._showPipeline = !1, this._keepMounted = !1, this._showDatumSignal = new B.Signal(this), this._repoViewInputSpec = {}, this._saveInputSpecSignal = new B.Signal(this), this._showPipelineSignal = new B.Signal(this), this._showMetadataSignal = new B.Signal(this), this.getActiveNotebook = () => this._tracker.currentWidget, this.handleNotebookChanged = (e, t) => ce(this, void 0, void 0, (function*() {
-                        var e;
-                        if (t) {
-                            yield t.sessionContext.ready;
-                            const a = null === (e = null == t ? void 0 : t.model) || void 0 === e ? void 0 : e.metadata.get(me);
-                            this._showMetadataSignal.emit(a), yield Promise.resolve()
-                        } else yield Promise.resolve()
+                constructor(e, t, a, n, r) {
+                    this._showConfig = !1, this._showConfigSignal = new L.Signal(this), this._readyPromise = Promise.resolve(), this._showDatum = !1, this._showPipeline = !1, this._keepMounted = !1, this._showDatumSignal = new L.Signal(this), this._repoViewInputSpec = {}, this._saveInputSpecSignal = new L.Signal(this), this._showPipelineSignal = new L.Signal(this), this._ppsContextSignal = new L.Signal(this), this.getActiveNotebook = () => this._tracker.currentWidget, this.handleNotebookChanged = (e, t) => ce(this, void 0, void 0, (function*() {
+                        let e;
+                        t ? (yield t.sessionContext.ready, t.context.fileChanged.connect(this.handleNotebookReload), e = {
+                            config: this.getNotebookMetadata(t),
+                            notebookModel: t.context.contentsModel
+                        }) : e = {
+                            config: null,
+                            notebookModel: null
+                        }, this._ppsContextSignal.emit(e), yield Promise.resolve()
+                    })), this.handleNotebookReload = (e, t) => ce(this, void 0, void 0, (function*() {
+                        const e = {
+                            config: this.getNotebookMetadata(),
+                            notebookModel: t
+                        };
+                        this._ppsContextSignal.emit(e), yield Promise.resolve()
                     })), this.getNotebookMetadata = e => {
                         var t;
-                        return null === (t = null == e ? void 0 : e.model) || void 0 === t ? void 0 : t.metadata.get(me)
-                    }, this.saveNotebookMetaData = e => {
+                        return null === (t = null == (e = null != e ? e : this.getActiveNotebook()) ? void 0 : e.model) || void 0 === t ? void 0 : t.metadata.get(me)
+                    }, this.saveNotebookMetadata = e => {
                         var t;
                         const a = this.getActiveNotebook();
                         null !== a ? (null === (t = null == a ? void 0 : a.model) || void 0 === t || t.metadata.set(me, e), console.log("notebook metadata saved")) : console.log("No active notebook")
                     }, this.open = e => {
                         this._app.commands.execute("filebrowser:open-path", {
                             path: oe + e
                         })
@@ -4036,30 +4053,30 @@
                         this.open("")
                     }, this.setShowDatum = e => ce(this, void 0, void 0, (function*() {
                         e ? (this._datum.setHidden(!1), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this.saveMountedReposList()) : (this._datum.setHidden(!0), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), yield this.restoreMountedReposList()), this._mountBrowser.setHidden(!1), this._config.setHidden(!0), this._pipeline.setHidden(!0), this._fullPageError.setHidden(!0), this._showDatum = e, this._showDatumSignal.emit(e)
                     })), this.saveMountedReposList = () => {
                         const e = this._poller.mounted,
                             t = [];
                         for (let a = 0; a < e.length; a++) {
-                            const r = {
+                            const n = {
                                 pfs: Object.assign(Object.assign(Object.assign(Object.assign(Object.assign({
                                     name: `${e[a].project}_${e[a].repo}`
                                 }, "master" !== e[a].branch && {
                                     name: `${e[a].project}_${e[a].repo}_${e[a].branch}`
                                 }), {
                                     repo: e[a].repo
                                 }), "default" !== e[a].project && {
                                     project: e[a].project
                                 }), "master" !== e[a].branch && {
                                     branch: e[a].branch
                                 }), {
                                     glob: "/"
                                 })
                             };
-                            t.push(r)
+                            t.push(n)
                         }
                         0 === e.length ? this._repoViewInputSpec = {} : 1 === e.length ? this._repoViewInputSpec = t[0] : this._repoViewInputSpec = {
                             cross: t
                         }, this._saveInputSpecSignal.emit(this._repoViewInputSpec)
                     }, this.restoreMountedReposList = () => ce(this, void 0, void 0, (function*() {
                         const e = [];
                         if (Object.prototype.hasOwnProperty.call(this._repoViewInputSpec, "cross") && Array.isArray(this._repoViewInputSpec.cross))
@@ -4078,53 +4095,53 @@
                                     name: t.name ? t.name : t.repo,
                                     repo: t.repo,
                                     project: t.project ? t.project : "default",
                                     branch: t.branch ? t.branch : "master",
                                     mode: "ro"
                                 })
                             } if (e.length > 0) {
-                            const t = yield D("_mount", "PUT", {
+                            const t = yield A("_mount", "PUT", {
                                 mounts: e
                             });
                             this._poller.updateData(t)
                         }
                         this.open("")
                     })), this.setShowPipeline = e => {
-                        e ? (this._pipeline.setHidden(!1), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0)) : (this._pipeline.setHidden(!0), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1)), this._mountBrowser.setHidden(!0), this._config.setHidden(!0), this._datum.setHidden(!0), this._fullPageError.setHidden(!0), this._showPipeline = e, this._showPipelineSignal.emit(e)
+                        e ? (this._pipeline.setHidden(!1), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._mountBrowser.setHidden(!0)) : (this._pipeline.setHidden(!0), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), this._mountBrowser.setHidden(!1)), this._config.setHidden(!0), this._datum.setHidden(!0), this._fullPageError.setHidden(!0), this._showPipeline = e, this._showPipelineSignal.emit(e)
                     }, this.setKeepMounted = e => {
                         this._keepMounted = e
                     }, this.setShowConfig = e => {
                         e ? (this._config.setHidden(!1), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._mountBrowser.setHidden(!0)) : (this._config.setHidden(!0), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), this._mountBrowser.setHidden(!1)), this._datum.setHidden(!0), this._pipeline.setHidden(!0), this._fullPageError.setHidden(!0), this._showConfig = e, this._showConfigSignal.emit(e)
                     }, this.setShowFullPageError = e => {
                         e ? (this._fullPageError.setHidden(!1), this._config.setHidden(!0), this._datum.setHidden(!0), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._mountBrowser.setHidden(!0), this._pipeline.setHidden(!0)) : (this._fullPageError.setHidden(!0), this._config.setHidden(!1), this._datum.setHidden(!1), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), this._mountBrowser.setHidden(!1), this._pipeline.setHidden(!1))
                     }, this.updateConfig = e => {
                         this._poller.config = e
                     }, this.setup = () => ce(this, void 0, void 0, (function*() {
                         if (yield this._poller.refresh(), 500 === this._poller.status.code) this.setShowFullPageError(!0);
                         else if (this.setShowConfig("INVALID" === this._poller.config.cluster_status || 200 !== this._poller.status.code), 200 === this._poller.status.code) try {
-                            const e = yield D("datums", "GET");
+                            const e = yield A("datums", "GET");
                             e.num_datums > 0 && (this._keepMounted = !0, this._currentDatumInfo = e, yield this.setShowDatum(!0))
                         } catch (e) {
                             console.log(e)
                         }
                         this._loader.setHidden(!0)
-                    })), this._app = e, this._poller = new N("PollMounts"), this._repoViewInputSpec = {}, this._tracker = n, this._poller.configSignal.connect(((e, t) => {
+                    })), this._app = e, this._poller = new N("PollMounts"), this._repoViewInputSpec = {}, this._tracker = r, this._poller.configSignal.connect(((e, t) => {
                         "INVALID" !== t.cluster_status || this._showConfig || this.setShowConfig(!0)
                     })), this._poller.statusSignal.connect(((e, t) => {
                         500 === t.code && this.setShowFullPageError(!0), 401 !== t.code || this._showConfig || this.setShowConfig(!0)
                     })), this._readyPromise = this.setup(), this._config = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._showConfigSignal
                     }, ((e, t) => m().createElement(d.UseSignal, {
                         signal: this._poller.configSignal
                     }, ((e, a) => m().createElement(d.UseSignal, {
                         signal: this._poller.statusSignal
-                    }, ((e, r) => m().createElement(U, {
+                    }, ((e, n) => m().createElement(R, {
                         showConfig: t || this._showConfig,
                         setShowConfig: this.setShowConfig,
-                        reposStatus: r ? r.code : this._poller.status.code,
+                        reposStatus: n ? n.code : this._poller.status.code,
                         updateConfig: this.updateConfig,
                         authConfig: a || this._poller.config,
                         refresh: this._poller.refresh
                     })))))))), this._config.addClass("pachyderm-mount-config-wrapper"), this._mountedList = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._poller.mountedSignal
                     }, ((e, t) => m().createElement("div", {
                         className: "pachyderm-mount-base"
@@ -4154,27 +4171,27 @@
                         className: "pachyderm-mount-icon-padding"
                     })), m().createElement("button", {
                         className: "pachyderm-button-link",
                         onClick: () => this.setShowConfig(!0)
                     }, "Config", " ", m().createElement(g.settingsIcon.react, {
                         tag: "span",
                         className: "pachyderm-mount-icon-padding"
-                    })))), m().createElement(ne, {
+                    })))), m().createElement(re, {
                         open: this.open,
                         items: t || this._poller.mounted,
                         updateData: this._poller.updateData,
                         mountedItems: [],
                         type: "mounted"
                     }))))), this._mountedList.addClass("pachyderm-mount-react-wrapper"), this._unmountedList = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._poller.unmountedSignal
                     }, ((e, t) => m().createElement("div", {
                         className: "pachyderm-mount-base"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-base-title"
-                    }, "Unmounted Repositories"), m().createElement(ne, {
+                    }, "Unmounted Repositories"), m().createElement(re, {
                         open: this.open,
                         items: t || this._poller.unmounted,
                         updateData: this._poller.updateData,
                         mountedItems: this._poller.mounted,
                         type: "unmounted"
                     }))))), this._unmountedList.addClass("pachyderm-mount-react-wrapper"), this._datum = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._showDatumSignal
@@ -4186,48 +4203,44 @@
                         keepMounted: this._keepMounted,
                         setKeepMounted: this.setKeepMounted,
                         open: this.open,
                         pollRefresh: this._poller.refresh,
                         currentDatumInfo: this._currentDatumInfo,
                         repoViewInputSpec: a || this._repoViewInputSpec
                     })))))), this._datum.addClass("pachyderm-mount-datum-wrapper"), this._pipeline = d.ReactWidget.create(m().createElement(d.UseSignal, {
-                        signal: this._showMetadataSignal
-                    }, ((e, t) => {
-                        var a, r, n;
-                        return m().createElement(m().Fragment, null, m().createElement(J, {
-                            setShowPipeline: this.setShowPipeline,
-                            notebookPath: null === (n = null === (r = null === (a = this.getActiveNotebook()) || void 0 === a ? void 0 : a.sessionContext) || void 0 === r ? void 0 : r.session) || void 0 === n ? void 0 : n.path,
-                            saveNotebookMetadata: this.saveNotebookMetaData,
-                            metadata: t
-                        }))
-                    }))), this._pipeline.addClass("pachyderm-mount-pipeline-wrapper"), this._loader = d.ReactWidget.create(m().createElement(P, null)), this._loader.addClass("pachyderm-mount-react-wrapper"), this._fullPageError = d.ReactWidget.create(m().createElement(d.UseSignal, {
+                        signal: this._ppsContextSignal
+                    }, ((e, t) => m().createElement(J, {
+                        ppsContext: t,
+                        setShowPipeline: this.setShowPipeline,
+                        saveNotebookMetadata: this.saveNotebookMetadata
+                    })))), this._pipeline.addClass("pachyderm-mount-pipeline-wrapper"), this._loader = d.ReactWidget.create(m().createElement(P, null)), this._loader.addClass("pachyderm-mount-react-wrapper"), this._fullPageError = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._poller.statusSignal
                     }, ((e, t) => m().createElement(ie, {
                         status: t || this._poller.status
                     })))), this._fullPageError.addClass("pachyderm-mount-react-wrapper"), this._mountBrowser = ((e, t, a) => {
-                        var r;
-                        const n = new H(e.docRegistry);
-                        t.services.contents.addDrive(n);
+                        var n;
+                        const r = new H(e.docRegistry);
+                        t.services.contents.addDrive(r);
                         const l = a.createFileBrowser("jupyterlab-pachyderm-browser", {
-                            driveName: n.name,
+                            driveName: r.name,
                             state: null,
                             refreshInterval: 1e4
                         });
                         try {
                             const e = l.toolbar.node.childNodes[0],
                                 a = l.toolbar.node.childNodes[1];
                             l.toolbar.node.removeChild(e), l.toolbar.node.removeChild(a);
-                            const n = l.layout.widgets || [],
-                                s = n.find((e => e instanceof z.BreadCrumbs));
+                            const r = l.layout.widgets || [],
+                                s = r.find((e => e instanceof z.BreadCrumbs));
                             if (s) {
-                                null === (r = s.node.querySelector('svg[data-icon="ui-components:folder"]')) || void 0 === r || r.replaceWith("/ pfs");
+                                null === (n = s.node.querySelector('svg[data-icon="ui-components:folder"]')) || void 0 === n || n.replaceWith("/ pfs");
                                 const e = s.node.querySelector('span[title="~/extension-wd"]');
                                 e && (e.className = "jp-BreadCrumbs-item")
                             }
-                            const i = n.find((e => e instanceof z.DirListing));
+                            const i = r.find((e => e instanceof z.DirListing));
                             if (i) {
                                 const e = new F.CommandRegistry;
                                 e.addCommand("file-open", {
                                     label: "Open",
                                     icon: "fa fa-folder",
                                     mnemonic: 0,
                                     execute: () => {
@@ -4241,35 +4254,35 @@
                                     mnemonic: 0,
                                     execute: () => {
                                         (0, j.each)(l.selectedItems(), (e => {
                                             d.Clipboard.copyToSystem(e.path.replace(oe, "/pfs/"))
                                         }))
                                     }
                                 });
-                                const a = new L.Menu({
+                                const a = new B.Menu({
                                     commands: e
                                 });
                                 a.addItem({
                                     command: "file-open"
                                 }), a.addItem({
                                     command: "copy-path"
                                 }), i.node.getElementsByClassName("jp-DirListing-content")[0].addEventListener("contextmenu", (e => {
                                     e.stopPropagation(), e.preventDefault();
                                     const t = e.clientX,
-                                        r = e.clientY;
-                                    a.open(t, r)
+                                        n = e.clientY;
+                                    a.open(t, n)
                                 }))
                             }
                         } catch (e) {
                             console.log("Failed to edit default browser.")
                         }
                         return l
-                    })(e, t, a), this._poller.mountedSignal.connect(this.verifyBrowserPath), this._poller.mountedSignal.connect(this.refresh), this._poller.unmountedSignal.connect(this.refresh), this._tracker.currentChanged.connect(this.handleNotebookChanged, this), this._panel = new L.SplitPanel, this._panel.orientation = "vertical", this._panel.spacing = 0, this._panel.title.icon = k, this._panel.title.caption = "Pachyderm Mount", this._panel.id = "pachyderm-mount", this._panel.addWidget(this._mountedList), this._panel.addWidget(this._unmountedList), this._panel.addWidget(this._datum), this._panel.addWidget(this._pipeline), this._panel.addWidget(this._mountBrowser), this._panel.setRelativeSizes([1, 1, 3, 3]), this._panel.addWidget(this._loader), this._panel.addWidget(this._config), this._panel.addWidget(this._fullPageError), this._config.setHidden(!0), this._fullPageError.setHidden(!0), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._datum.setHidden(!0), this._pipeline.setHidden(!0), this._mountBrowser.setHidden(!0), window.addEventListener("resize", (() => {
+                    })(e, t, a), this._poller.mountedSignal.connect(this.verifyBrowserPath), this._poller.mountedSignal.connect(this.refresh), this._poller.unmountedSignal.connect(this.refresh), this._tracker.currentChanged.connect(this.handleNotebookChanged, this), this._panel = new B.SplitPanel, this._panel.orientation = "vertical", this._panel.spacing = 0, this._panel.title.icon = k, this._panel.title.caption = "Pachyderm Mount", this._panel.id = "pachyderm-mount", this._panel.addWidget(this._mountedList), this._panel.addWidget(this._unmountedList), this._panel.addWidget(this._datum), this._panel.addWidget(this._pipeline), this._panel.addWidget(this._mountBrowser), this._panel.setRelativeSizes([1, 1, 3, 3]), this._panel.addWidget(this._loader), this._panel.addWidget(this._config), this._panel.addWidget(this._fullPageError), this._config.setHidden(!0), this._fullPageError.setHidden(!0), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._datum.setHidden(!0), this._pipeline.setHidden(!0), this._mountBrowser.setHidden(!0), window.addEventListener("resize", (() => {
                         this._panel.update()
-                    })), r.add(this._panel, "jupyterlab-pachyderm"), e.shell.add(this._panel, "left", {
+                    })), n.add(this._panel, "jupyterlab-pachyderm"), e.shell.add(this._panel, "left", {
                         rank: 100
                     })
                 }
                 get mountedRepos() {
                     return this._poller.poll.tick, this._poller.mounted
                 }
                 get unmountedRepos() {
@@ -4282,12 +4295,12 @@
                     return this._readyPromise
                 }
             }
             const ue = [{
                 id: "jupyterlab-pachyderm:mount",
                 autoStart: !0,
                 requires: [M.IDocumentManager, z.IFileBrowserFactory, C.ILayoutRestorer, S.INotebookTracker],
-                activate: (e, t, a, r, n) => new de(e, t, a, r, n)
+                activate: (e, t, a, n, r) => new de(e, t, a, n, r)
             }, i, p, x]
         }
     }
 ]);
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/remoteEntry.8cf7225b6da9d05077a7.js` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/remoteEntry.29814ef51cca10c332b8.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -49,22 +49,22 @@
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         67: "9d3e2934cfe0e102619e",
         371: "8ac933b7fbb0f688b6f4",
         486: "003d1d2cc9cc6927471e",
         676: "95f9b834e9f9b133c00b",
         747: "4bacb4613a4fbdd0e8a7",
-        869: "aa9313c5e001be51e97f"
+        869: "74d0c84d4f9c3908c376"
     } [e] + ".js?v=" + {
         67: "9d3e2934cfe0e102619e",
         371: "8ac933b7fbb0f688b6f4",
         486: "003d1d2cc9cc6927471e",
         676: "95f9b834e9f9b133c00b",
         747: "4bacb4613a4fbdd0e8a7",
-        869: "aa9313c5e001be51e97f"
+        869: "74d0c84d4f9c3908c376"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -116,15 +116,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : l > u.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === t && (u("jupyterlab-pachyderm", "2.6.0-alpha.3", (() => Promise.all([j.e(371), j.e(869)]).then((() => () => j(1979))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyterlab-pachyderm", "2.6.0-alpha.5", (() => Promise.all([j.e(371), j.e(869)]).then((() => () => j(1979))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -222,34 +222,34 @@
         var o = j.I(r);
         return o && o.then ? o.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
     })(((e, r, t, a) => (l(e, t), d(r, 0, t, a)))), h = p(((e, r, t, a, n) => {
         var o = r && j.o(r, t) && f(r, t, a);
         return o ? s(o) : n()
     })), b = {}, v = {
         930: () => h("default", "yaml", [1, 2, 1, 1], (() => j.e(676).then((() => () => j(5676))))),
-        1431: () => c("default", "@lumino/widgets", [1, 1, 37, 1]),
+        1123: () => c("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
+        1467: () => c("default", "@jupyterlab/launcher", [1, 3, 6, 3]),
         1526: () => c("default", "@lumino/coreutils", [1, 1, 11, 0]),
         1840: () => c("default", "@lumino/signaling", [1, 1, 10, 0]),
-        2884: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 2]),
-        3215: () => c("default", "@jupyterlab/ui-components", [1, 3, 6, 2]),
-        3619: () => c("default", "@jupyterlab/docmanager", [1, 3, 6, 2]),
+        2502: () => c("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
+        3033: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
         4234: () => h("default", "rudder-sdk-js", [1, 1, 2, 1], (() => j.e(67).then((() => () => j(3067))))),
         4439: () => h("default", "lodash", [1, 4, 17, 21], (() => j.e(486).then((() => () => j(6486))))),
-        5613: () => c("default", "@jupyterlab/services", [1, 6, 6, 2]),
-        5643: () => c("default", "@jupyterlab/filebrowser", [1, 3, 6, 2]),
-        5679: () => c("default", "@jupyterlab/notebook", [1, 3, 6, 2]),
+        5344: () => c("default", "@jupyterlab/mainmenu", [1, 3, 6, 3]),
+        5687: () => c("default", "@jupyterlab/application", [1, 3, 6, 3]),
         6057: () => c("default", "@lumino/commands", [1, 1, 19, 0]),
         6271: () => c("default", "react", [1, 17, 0, 1]),
-        6848: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 2]),
-        8529: () => c("default", "@jupyterlab/launcher", [1, 3, 6, 2]),
-        8918: () => c("default", "@lumino/algorithm", [1, 1, 9, 0]),
-        9239: () => c("default", "@jupyterlab/application", [1, 3, 6, 2]),
-        9448: () => c("default", "@jupyterlab/mainmenu", [1, 3, 6, 2])
+        7280: () => c("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
+        7986: () => c("default", "@jupyterlab/docmanager", [1, 3, 6, 3]),
+        8142: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        8820: () => c("default", "@jupyterlab/services", [1, 6, 6, 3]),
+        8832: () => c("default", "@lumino/widgets", [1, 1, 37, 2]),
+        8918: () => c("default", "@lumino/algorithm", [1, 1, 9, 0])
     }, m = {
-        869: [930, 1431, 1526, 1840, 2884, 3215, 3619, 4234, 4439, 5613, 5643, 5679, 6057, 6271, 6848, 8529, 8918, 9239, 9448]
+        869: [930, 1123, 1467, 1526, 1840, 2502, 3033, 4234, 4439, 5344, 5687, 6057, 6271, 7280, 7986, 8142, 8820, 8832, 8918]
     }, j.f.consumes = (e, r) => {
         j.o(m, e) && m[e].forEach((e => {
             if (j.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, j.m[e] = t => {
                         delete j.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/third-party-licenses.json` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/mount_server_client.py` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/mount_server_client.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/pachyderm.py` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/pachyderm.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/test_handlers.py` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/tests/test_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import json
+import os
 import sys
+from pathlib import Path
 from unittest.mock import patch
 
 import pytest
 import tornado
 
 from jupyterlab_pachyderm.handlers import NAMESPACE, VERSION
 from jupyterlab_pachyderm.pachyderm import MountInterface
 
+from . import TEST_NOTEBOOK
 
 pytest_plugins = ["jupyter_server.pytest_plugin"]
 
 
 class ErrorWithCode(Exception):
     def __init__(self, code):
         self.code = code
@@ -534,15 +537,15 @@
 @patch("jupyterlab_pachyderm.handlers.HealthHandler.mount_client", spec=MountInterface)
 async def test_health(mock_client, jp_fetch):
     mock_client.health.return_value = json.dumps({"status": "running"})
     r = await jp_fetch(f"/{NAMESPACE}/{VERSION}/health")
     assert json.loads(r.body) == {"status": "running"}
 
 
-@pytest.mark.skipif(sys.version_info < (3, 7), reason="requires python3.7 or higher")
 async def test_pps_get(jp_fetch):
-    response = await jp_fetch(f"/{NAMESPACE}/{VERSION}/pps/_create/NOT_REAL.ipynb")
+    notebook_path = TEST_NOTEBOOK.relative_to(os.getcwd())
+    response = await jp_fetch(f"/{NAMESPACE}/{VERSION}/pps/_create/{notebook_path}")
     assert response.code == 200
     body = json.loads(response.body)
     for expected_key in ("pipeline", "description", "transform", "input"):
         assert expected_key in body
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/test_integrations.py` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm/tests/test_integrations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import os
 import sys
 import subprocess
 import time
 import json
+from datetime import datetime
 from pathlib import Path
+from random import randint
 
 import pytest
 import requests
 
 from jupyterlab_pachyderm.handlers import NAMESPACE, VERSION
 from jupyterlab_pachyderm.env import PFS_MOUNT_DIR
-from jupyterlab_pachyderm.pps_client import SAME_METADATA_FIELDS
 
+from . import TEST_NOTEBOOK
 
 ADDRESS = "http://localhost:8888"
 BASE_URL = f"{ADDRESS}/{NAMESPACE}/{VERSION}"
 CONFIG_PATH = "~/.pachyderm/config.json"
 ROOT_TOKEN = "iamroot"
 DEFAULT_PROJECT = "default"
 
-TEST_NOTEBOOK = Path(__file__).parent.joinpath('data/TestNotebook.ipynb')
-
 
 @pytest.fixture()
 def pachyderm_resources():
     print("creating pachyderm resources")
     import python_pachyderm
     from python_pachyderm.pfs import Commit
 
@@ -384,44 +384,57 @@
 
 
 @pytest.fixture
 def simple_pachyderm_env():
     from python_pachyderm import Client
     client = Client()
 
-    repo_name = f"images_194837"
-    pipeline_name = f"test_pipeline_194837"
+    suffix = str(randint(100000, 999999))
+    repo_name = f"images_{suffix}"
+    pipeline_name = f"test_pipeline_{suffix}"
     client.delete_repo(repo_name, force=True)
     client.create_repo(repo_name)
     yield client, repo_name, pipeline_name
     client.delete_pipeline(pipeline_name, force=True)
+    client.delete_pipeline(f"{pipeline_name}__context", force=True)
     client.delete_repo(repo_name, force=True)
 
 
-def test_pps(dev_server, simple_pachyderm_env):
+@pytest.fixture
+def notebook_path(simple_pachyderm_env) -> Path:
+    """Yields a path to a notebook file suitable for testing.
+
+    This writes a temporary notebook file with its metadata populated
+      with the expected pipeline and repo names provided by the
+      simple_pachyderm_env fixture.
+    """
+    _client, repo_name, pipeline_name = simple_pachyderm_env
+
+    # Do a considerable amount of data munging.
+    notebook_data = json.loads(TEST_NOTEBOOK.read_bytes())
+    notebook_data['metadata']['same_config']['metadata']['name'] = pipeline_name
+    input_spec = json.loads(notebook_data['metadata']['same_config']['run']['input'])
+    input_spec['pfs']['repo'] = repo_name
+    notebook_data['metadata']['same_config']['run']['input'] = json.dumps(input_spec)
+
+    notebook_path = TEST_NOTEBOOK.with_stem(f"{TEST_NOTEBOOK.stem}_generated")
+    notebook_path.write_text(json.dumps(notebook_data))
+    yield notebook_path.relative_to(os.getcwd())
+    if notebook_path.exists():
+        notebook_path.unlink()
+
+
+def test_pps(dev_server, simple_pachyderm_env, notebook_path):
     client, repo_name, pipeline_name = simple_pachyderm_env
-    path = TEST_NOTEBOOK.relative_to(Path.cwd())
-    image = "combinatorml/jupyterlab-tensorflow-opencv:0.9"
-    input_spec = dict(pfs=dict(repo=repo_name, glob="/*"))
-    data = dict(
-        apiVersion='sameproject.ml/v1alpha1',
-        environments=dict(default=dict(image_tag=image)),
-        metadata=dict(name=pipeline_name, version='0.0.0'),
-        notebook=dict(requirements=''),
-        run=dict(name=pipeline_name, input=json.dumps(input_spec)),
-    )
-    r = requests.put(f"{BASE_URL}/pps/_create/{path}", data=json.dumps(data))
+    last_modified = datetime.utcfromtimestamp(os.path.getmtime(notebook_path))
+    data = dict(last_modified_time=f"{datetime.isoformat(last_modified)}Z")
+    r = requests.put(f"{BASE_URL}/pps/_create/{notebook_path}", data=json.dumps(data))
     assert r.status_code == 200
     assert next(client.inspect_pipeline(pipeline_name))
+    assert r.json()["message"] == ("Create pipeline request sent. You may monitor its "
+    "status by running \"pachctl list pipelines\" in a terminal.")
 
 
-@pytest.mark.parametrize('excluded_field', SAME_METADATA_FIELDS)
-def test_pps_validation_errors(dev_server, excluded_field):
-    path = TEST_NOTEBOOK.relative_to(Path.cwd())
-    data = dict()
-    for field in SAME_METADATA_FIELDS:
-        if field != excluded_field:
-            data[field] = dict()
-
-    r = requests.put(f"{BASE_URL}/pps/_create/{path}", data=json.dumps(data))
+def test_pps_validation_errors(dev_server, notebook_path):
+    r = requests.put(f"{BASE_URL}/pps/_create/{notebook_path}", data=json.dumps({}))
     assert r.status_code == 500
-    assert r.json()['reason'] == f"Bad Request: field {excluded_field} not set"
+    assert r.json()['reason'] == f"Bad Request: last_modified_time not specified"
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/PKG-INFO` & `jupyterlab_pachyderm-2.6.0a5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyterlab-pachyderm
-Version: 2.6.0a3
+Name: jupyterlab_pachyderm
+Version: 2.6.0a5
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
@@ -62,21 +62,20 @@
 kubectl port-forward service/pachd 30650:30650
 ```
 
 Start a bash session in the `pachyderm/notebooks-user` container from the top-level `jupyterlab-pachyderm` repo.
 
 ```
 docker run --name jupyterlab_pachyderm_frontend_dev \
-  --net=host \
-  --rm \
+  -p 8888:8888 \
   -it -e GRANT_SUDO=yes --user root \
   --device /dev/fuse --privileged \
   -v $(pwd):/home/jovyan/extension-wd \
   -w /home/jovyan/extension-wd \
-  pachyderm/notebooks-user:77ce3a1ef2c73bf34d064cd0bdb5a64262bf3280 \
+  pachyderm/notebooks-user:<latest master SHA> \
   bash
 ```
 
 If you are running the frontend container on Linux, and want to be able to talk to pachd in minikube on `grpc://localhost:30650`, use `--net=host` at the start of the the `docker run` command as shown above. If you are on macOS, you will want to remove `--net=host` as it is not supported. On macOS you can specify `grpc://host.docker.internal:30650` to get the same effect.
 
 Install the project in editable mode, and start JupyterLab
 
@@ -98,15 +97,28 @@
 
 Within container run:
 
 ```
 npm run watch
 ```
 
+Note: Once run above, you can start the dev container again in future sessions using
+
+```
+docker start <container id>
+```
+
+and then running
+
+```
+docker exec -it <container id> bash
+```
+
 Iterating on the mount server, from inside a `pachyderm` checkout:
+
 ```
 CGO_ENABLED=0 make install
 docker cp /home/luke/gocode/bin/pachctl jupyterlab_pachyderm_frontend_dev:/usr/local/bin/pachctl
 docker exec -ti jupyterlab_pachyderm_frontend_dev pkill -f pachctl
 ```
 
 ## Local Virtual Environment Setup 
@@ -216,14 +228,24 @@
 
 First make sure the server extension is enabled:
 
 ```
 jupyter server extension list 2>&1 | grep -ie "jupyterlab_pachyderm.*OK"
 ```
 
+# Install Jupyterhub locally (Sidecar mode testing)
+
+```
+helm repo add jupyterhub https://jupyterhub.github.io/helm-chart/
+helm repo update
+helm install jhub jupyterhub/jupyterhub --version 2.0.0 --values scripts/jhub-dev-helm-values.yml
+```
+
+Note: Use any username and no password to login
+
 ### API endpoints
 
 ```
 GET /repos # returns a list of all repos/branches
 GET /mounts # returns a list of all active mounts and unmounted repos/branches
 PUT /_mount # mounts a single repo
 PUT /_unmount # unmounts a single repo
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/SOURCES.txt` & `jupyterlab_pachyderm-2.6.0a5/jupyterlab_pachyderm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
 jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
 jupyterlab_pachyderm/labextension/static/747.4bacb4613a4fbdd0e8a7.js
-jupyterlab_pachyderm/labextension/static/869.aa9313c5e001be51e97f.js
-jupyterlab_pachyderm/labextension/static/remoteEntry.8cf7225b6da9d05077a7.js
+jupyterlab_pachyderm/labextension/static/869.74d0c84d4f9c3908c376.js
+jupyterlab_pachyderm/labextension/static/remoteEntry.29814ef51cca10c332b8.js
 jupyterlab_pachyderm/labextension/static/style.js
 jupyterlab_pachyderm/labextension/static/third-party-licenses.json
 jupyterlab_pachyderm/tests/__init__.py
 jupyterlab_pachyderm/tests/test_handlers.py
 jupyterlab_pachyderm/tests/test_integrations.py
 jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
 schema/examples.json
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/package.json` & `jupyterlab_pachyderm-2.6.0a5/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.6.0-alpha.5'"}*

```diff
@@ -127,9 +127,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.0-alpha.3"
+    "version": "2.6.0-alpha.5"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/pyproject.toml` & `jupyterlab_pachyderm-2.6.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/setup.cfg` & `jupyterlab_pachyderm-2.6.0a5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Framework :: Jupyter :: JupyterLab :: Extensions
 	Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 
 [options]
 packages = find:
 install_requires = 
 	jupyter_server>=1.6,<2
-	sameproject==0.2.5
+	python-pachyderm>=v7.4.0,<8
 include_package_data = True
 zip_safe = False
 python_requires = >=3.8,<4
 
 [options.extras_require]
 dev = 
 	black
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/setup.py` & `jupyterlab_pachyderm-2.6.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/handler.ts` & `jupyterlab_pachyderm-2.6.0a5/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/__test__/examples.test.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/examples/__test__/examples.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/examples.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/examples/examples.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/help/__tests__/help.test.ts` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/help/__tests__/help.test.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/help/help.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/help/help.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/__tests__/mount.test.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/__tests__/mount.test.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import {CommandRegistry} from '@lumino/commands';
 import {Widget} from '@lumino/widgets';
 import {mockedRequestAPI} from 'utils/testUtils';
 import {MountPlugin} from '../mount';
 import * as requestAPI from '../../../handler';
 import {waitFor} from '@testing-library/react';
 import {INotebookTracker, NotebookTracker} from '@jupyterlab/notebook';
+import Pipeline from '../components/Pipeline/Pipeline';
 
 jest.mock('../../../handler');
 
 const items = {
   unmounted: [
     {
       repo: 'images',
@@ -136,8 +137,27 @@
     expect(plugin.layout.widgets[2]).toBeInstanceOf(ReactWidget);
     expect(plugin.layout.widgets[3]).toBeInstanceOf(ReactWidget);
     expect(plugin.layout.widgets[4]).toBeInstanceOf(FileBrowser);
     expect(plugin.layout.widgets[5]).toBeInstanceOf(ReactWidget);
     expect(plugin.layout.widgets[6]).toBeInstanceOf(ReactWidget);
     expect(plugin.layout.widgets[7]).toBeInstanceOf(ReactWidget);
   });
+
+  it('return from pipeline view to the correct layout', async () => {
+    const plugin = new MountPlugin(app, docManager, factory, restorer, tracker);
+    const pipeline = plugin.layout.widgets[3];
+    const fileBrowser = plugin.layout.widgets[4];
+    expect(fileBrowser).toBeInstanceOf(FileBrowser);
+
+    plugin.setShowConfig(false);
+    expect(pipeline.isHidden).toBe(true);
+    expect(fileBrowser.isHidden).toBe(false);
+
+    plugin.setShowPipeline(true);
+    expect(pipeline.isHidden).toBe(false);
+    expect(fileBrowser.isHidden).toBe(true);
+
+    plugin.setShowPipeline(false);
+    expect(pipeline.isHidden).toBe(true);
+    expect(fileBrowser.isHidden).toBe(false);
+  });
 });
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/Config.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Config/Config.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/__tests__/Config.test.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Config/__tests__/Config.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/hooks/useConfig.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Config/hooks/useConfig.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/Datum.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Datum/Datum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/hooks/useDatum.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Datum/hooks/useDatum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/FullPageError/FullPageError.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/FullPageError/FullPageError.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/Pipeline.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Pipeline/Pipeline.tsx`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 import React from 'react';
 import {closeIcon} from '@jupyterlab/ui-components';
 import {usePipeline} from './hooks/usePipeline';
-import {SameMetadata} from '../../types';
+import {PpsContext, SameMetadata} from '../../types';
 
 type PipelineProps = {
+  ppsContext: PpsContext | undefined;
   setShowPipeline: (shouldShow: boolean) => void;
-  notebookPath: string | undefined;
-  saveNotebookMetadata: (metadata: any) => void;
-  metadata: SameMetadata | undefined;
+  saveNotebookMetadata: (metadata: SameMetadata) => void;
 };
 
 const placeholderInputSpec = `pfs:
   repo: images
   branch: dev
   glob: /*
 `;
 const placeholderRequirements = './requirements.txt';
 
 const Pipeline: React.FC<PipelineProps> = ({
+  ppsContext,
   setShowPipeline,
-  notebookPath,
   saveNotebookMetadata,
-  metadata,
 }) => {
   const {
     loading,
     pipelineName,
     setPipelineName,
     imageName,
     setImageName,
     inputSpec,
     setInputSpec,
     requirements,
     setRequirements,
     callCreatePipeline,
     callSavePipeline,
     errorMessage,
-  } = usePipeline(metadata, notebookPath, saveNotebookMetadata);
+    responseMessage,
+  } = usePipeline(ppsContext, saveNotebookMetadata);
 
   return (
     <div className="pachyderm-mount-pipeline-base">
       <div className="pachyderm-mount-pipeline-back">
         <button
           data-testid="Pipeline__back"
           className="pachyderm-button-link"
@@ -80,35 +79,42 @@
       <span
         className="pachyderm-pipeline-error"
         data-testid="Pipeline__errorMessage"
       >
         {errorMessage}
       </span>
 
+      <span
+        className="pachyderm-pipeline-response"
+        data-testid="Pipeline__responseMessage"
+      >
+        {responseMessage}
+      </span>
+
       <div className="pachyderm-pipeline-input-wrapper">
         <label
           className="pachyderm-pipeline-input-label"
           htmlFor="pipelineName"
         >
-          *Name:{'  '}
+          *Pipeline Name:{'  '}
         </label>
         <input
           className="pachyderm-pipeline-input"
           data-testid="Pipeline__inputPipelineName"
           name="pipelineName"
           value={pipelineName}
           onChange={(e: any) => {
             setPipelineName(e.target.value);
           }}
           disabled={loading}
         ></input>
       </div>
       <div className="pachyderm-pipeline-input-wrapper">
         <label className="pachyderm-pipeline-input-label" htmlFor="imageName">
-          *Image:{'  '}
+          *Container Image Name:{'  '}
         </label>
         <input
           className="pachyderm-pipeline-input"
           data-testid="Pipeline__inputImageName"
           name="imageName"
           value={imageName}
           onChange={(e: any) => {
@@ -118,15 +124,15 @@
         ></input>
       </div>
       <div className="pachyderm-pipeline-input-wrapper">
         <label
           className="pachyderm-pipeline-input-label"
           htmlFor="requirements"
         >
-          Requirements:{'  '}
+          Requirements File:{'  '}
         </label>
         <input
           className="pachyderm-pipeline-input"
           data-testid="Pipeline__inputRequirements"
           name="requirements"
           value={requirements}
           onChange={(e: any) => {
@@ -137,15 +143,15 @@
         ></input>
       </div>
       <div className="pachyderm-pipeline-textarea-wrapper">
         <label
           className="pachyderm-pipeline-textarea-label"
           htmlFor="inputSpec"
         >
-          Input Spec
+          Pipeline Input Spec:
         </label>
         <textarea
           className="pachyderm-pipeline-textarea pachyderm-input"
           data-testid="Pipeline__inputSpecInput"
           name="inputSpec"
           value={inputSpec}
           onChange={(e: any) => {
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import {render} from '@testing-library/react';
 import userEvent from '@testing-library/user-event';
 
 import * as requestAPI from '../../../../../handler';
 import {mockedRequestAPI} from 'utils/testUtils';
 import Pipeline from '../Pipeline';
 jest.mock('../../../../../handler');
-import {SameMetadata} from '../../../types';
+import {PpsContext, SameMetadata} from '../../../types';
 
 describe('PPS screen', () => {
   let setShowPipeline = jest.fn();
   const saveNotebookMetaData = jest.fn();
   const md: SameMetadata = {
     apiVersion: '',
     environments: {
@@ -24,29 +24,29 @@
     notebook: {
       requirements: '',
     },
     run: {
       name: '',
     },
   };
+  const context: PpsContext = {config: md, notebookModel: null};
 
   const mockRequestAPI = requestAPI as jest.Mocked<typeof requestAPI>;
 
   beforeEach(() => {
     setShowPipeline = jest.fn();
     mockRequestAPI.requestAPI.mockImplementation(mockedRequestAPI({}));
   });
 
   describe('spec preview', () => {
     it('proper preview', async () => {
       const {getByTestId, findByTestId} = render(
         <Pipeline
-          metadata={md}
+          ppsContext={context}
           setShowPipeline={setShowPipeline}
-          notebookPath={'FakeNotebook.ipynb'}
           saveNotebookMetadata={saveNotebookMetaData}
         />,
       );
 
       const inputPipelineName = await findByTestId(
         'Pipeline__inputPipelineName',
       );
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,100 @@
 import YAML from 'yaml';
-
 import {useEffect, useState} from 'react';
-import {CreatePipelineResponse, SameMetadata} from '../../../types';
-import {requestAPI} from '../../../../../handler';
-import {ReadonlyJSONObject} from '@lumino/coreutils';
 import {ServerConnection} from '@jupyterlab/services';
 
+import {CreatePipelineResponse, PpsContext, SameMetadata} from '../../../types';
+import {requestAPI} from '../../../../../handler';
+
 export type usePipelineResponse = {
   loading: boolean;
   pipelineName: string;
   setPipelineName: (input: string) => void;
   imageName: string;
   setImageName: (input: string) => void;
   inputSpec: string;
   setInputSpec: (input: string) => void;
   requirements: string;
   setRequirements: (input: string) => void;
   callCreatePipeline: () => Promise<void>;
   callSavePipeline: () => void;
   errorMessage: string;
+  responseMessage: string;
 };
 
 export const usePipeline = (
-  metadata: SameMetadata | undefined,
-  notebookPath: string | undefined,
-  saveNotebookMetaData: (metadata: any) => void,
+  ppsContext: PpsContext | undefined,
+  saveNotebookMetaData: (metadata: SameMetadata) => void,
 ): usePipelineResponse => {
   const [loading, setLoading] = useState(false);
   const [pipelineName, setPipelineName] = useState('');
   const [imageName, setImageName] = useState('');
   const [inputSpec, setInputSpec] = useState('');
   const [requirements, setRequirements] = useState('');
   const [errorMessage, setErrorMessage] = useState('');
+  const [responseMessage, setResponseMessage] = useState('');
 
   useEffect(() => {
-    setImageName(metadata?.environments.default.image_tag ?? '');
-    setPipelineName(metadata?.metadata.name ?? '');
-    setRequirements(metadata?.notebook.requirements ?? '');
-    if (metadata?.run.input) {
-      const input = JSON.parse(metadata?.run.input); //TODO: Catch errors
+    setImageName(ppsContext?.config?.environments.default.image_tag ?? '');
+    setPipelineName(ppsContext?.config?.metadata.name ?? '');
+    setRequirements(ppsContext?.config?.notebook.requirements ?? '');
+    setResponseMessage('');
+    if (ppsContext?.config?.run.input) {
+      const input = JSON.parse(ppsContext.config.run.input); //TODO: Catch errors
       setInputSpec(YAML.stringify(input));
     } else {
       setInputSpec('');
     }
-  }, [metadata]);
+  }, [ppsContext]);
 
-  const createSameMetadata = (): SameMetadata => {
+  let callCreatePipeline: () => Promise<void>;
+  if (ppsContext?.notebookModel) {
+    const notebook = ppsContext.notebookModel;
+    callCreatePipeline = async () => {
+      setLoading(true);
+      setErrorMessage('');
+      setResponseMessage('');
+      try {
+        const response = await requestAPI<CreatePipelineResponse>(
+          `pps/_create/${encodeURI(notebook.path)}`,
+          'PUT',
+          {last_modified_time: notebook.last_modified},
+        );
+        if (response.message !== null) {
+          setResponseMessage(response.message);
+        }
+      } catch (e) {
+        if (e instanceof ServerConnection.ResponseError) {
+          setErrorMessage(e.message);
+        } else {
+          throw e;
+        }
+      }
+      setLoading(false);
+    };
+  } else {
+    // If no notebookModel is defined, we cannot create a pipeline.
+    callCreatePipeline = async () => {
+      setErrorMessage('Error: No notebook in focus');
+    };
+  }
+
+  const callSavePipeline = async () => {
     let input: string;
     try {
       input = YAML.parse(inputSpec);
     } catch (e) {
       if (e instanceof YAML.YAMLParseError) {
         input = JSON.parse(inputSpec);
       } else {
         throw e;
       }
     }
 
-    return {
+    const sameMetadata = {
       apiVersion: 'sameproject.ml/v1alpha1',
       environments: {
         default: {
           image_tag: imageName,
         },
       },
       metadata: {
@@ -72,42 +105,15 @@
         requirements: requirements,
       },
       run: {
         name: pipelineName,
         input: JSON.stringify(input),
       },
     };
-  };
-
-  const callCreatePipeline = async () => {
-    setLoading(true);
-    setErrorMessage('');
-
-    const sameMetadata = createSameMetadata();
-    try {
-      const response = await requestAPI<CreatePipelineResponse>(
-        `pps/_create/${notebookPath}`,
-        'PUT',
-        sameMetadata as ReadonlyJSONObject,
-      );
-    } catch (e) {
-      if (e instanceof ServerConnection.ResponseError) {
-        setErrorMessage(e.message);
-      } else {
-        throw e;
-      }
-    }
-    console.log('create pipeline called');
-    setLoading(false);
-  };
-
-  const callSavePipeline = async () => {
-    const sameMetadata = createSameMetadata();
     saveNotebookMetaData(sameMetadata);
-    console.log('save pipeline called');
   };
 
   return {
     loading,
     pipelineName,
     setPipelineName,
     imageName,
@@ -115,9 +121,10 @@
     inputSpec,
     setInputSpec,
     requirements,
     setRequirements,
     callCreatePipeline,
     callSavePipeline,
     errorMessage,
+    responseMessage,
   };
 };
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/ListMount.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/SortableList/ListMount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/ListUnmount.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/SortableList/ListUnmount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/SortableList.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/SortableList/SortableList.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/customFileBrowser.ts` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/customFileBrowser.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/index.ts` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/mount.css` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/mount.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/mount.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/mount.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import React from 'react';
 import {ILayoutRestorer, JupyterFrontEnd} from '@jupyterlab/application';
-import {INotebookTracker, NotebookPanel} from '@jupyterlab/notebook';
-import {IDocumentManager} from '@jupyterlab/docmanager';
-import {SplitPanel} from '@lumino/widgets';
 import {ReactWidget, UseSignal} from '@jupyterlab/apputils';
+import {IDocumentManager} from '@jupyterlab/docmanager';
+import {DocumentRegistry} from '@jupyterlab/docregistry';
 import {FileBrowser, IFileBrowserFactory} from '@jupyterlab/filebrowser';
+import {
+  INotebookModel,
+  INotebookTracker,
+  NotebookPanel,
+} from '@jupyterlab/notebook';
+import {Contents} from '@jupyterlab/services';
 import {settingsIcon, spreadsheetIcon} from '@jupyterlab/ui-components';
-import {Signal} from '@lumino/signaling';
 import {JSONObject} from '@lumino/coreutils';
+import {Signal} from '@lumino/signaling';
+import {SplitPanel} from '@lumino/widgets';
 
 import {mountLogoIcon} from '../../utils/icons';
 import {PollMounts} from './pollMounts';
 import createCustomFileBrowser from './customFileBrowser';
 import {
   AuthConfig,
   IMountPlugin,
   Repo,
   Mount,
   CurrentDatumResponse,
   PfsInput,
   ListMountsResponse,
   CrossInputSpec,
   SameMetadata,
+  PpsContext,
 } from './types';
 import Config from './components/Config/Config';
 import Datum from './components/Datum/Datum';
 import Pipeline from './components/Pipeline/Pipeline';
 import SortableList from './components/SortableList/SortableList';
 import LoadingDots from '../../utils/components/LoadingDots/LoadingDots';
 import FullPageError from './components/FullPageError/FullPageError';
@@ -59,15 +66,15 @@
   private _currentDatumInfo: CurrentDatumResponse | undefined;
   private _showDatumSignal = new Signal<this, boolean>(this);
   private _repoViewInputSpec: CrossInputSpec | PfsInput = {};
   private _saveInputSpecSignal = new Signal<this, CrossInputSpec | PfsInput>(
     this,
   );
   private _showPipelineSignal = new Signal<this, boolean>(this);
-  private _showMetadataSignal = new Signal<this, SameMetadata>(this);
+  private _ppsContextSignal = new Signal<this, PpsContext>(this);
 
   constructor(
     app: JupyterFrontEnd,
     manager: IDocumentManager,
     factory: IFileBrowserFactory,
     restorer: ILayoutRestorer,
     tracker: INotebookTracker,
@@ -222,26 +229,21 @@
           </UseSignal>
         )}
       </UseSignal>,
     );
     this._datum.addClass('pachyderm-mount-datum-wrapper');
 
     this._pipeline = ReactWidget.create(
-      <UseSignal signal={this._showMetadataSignal}>
-        {(_, metadata) => (
-          <>
-            <Pipeline
-              setShowPipeline={this.setShowPipeline}
-              notebookPath={
-                this.getActiveNotebook()?.sessionContext?.session?.path
-              }
-              saveNotebookMetadata={this.saveNotebookMetaData}
-              metadata={metadata}
-            />
-          </>
+      <UseSignal signal={this._ppsContextSignal}>
+        {(_, context) => (
+          <Pipeline
+            ppsContext={context}
+            setShowPipeline={this.setShowPipeline}
+            saveNotebookMetadata={this.saveNotebookMetadata}
+          />
         )}
       </UseSignal>,
     );
     this._pipeline.addClass('pachyderm-mount-pipeline-wrapper');
 
     this._loader = ReactWidget.create(<LoadingDots />);
 
@@ -306,30 +308,51 @@
    * The parameters are automatically passed from the signal when a switch occurs.
    */
   handleNotebookChanged = async (
     tracker: INotebookTracker,
     notebook: NotebookPanel | null,
   ): Promise<void> => {
     // Set the current notebook and wait for the session to be ready
+    let context: PpsContext;
     if (notebook) {
       await notebook.sessionContext.ready;
-      const md = notebook?.model?.metadata.get(METADATA_KEY);
-
-      this._showMetadataSignal.emit(md as SameMetadata);
-      await Promise.resolve();
+      notebook.context.fileChanged.connect(this.handleNotebookReload);
+      context = {
+        config: this.getNotebookMetadata(notebook),
+        notebookModel: notebook.context.contentsModel,
+      };
     } else {
-      await Promise.resolve();
+      context = {config: null, notebookModel: null};
     }
+    this._ppsContextSignal.emit(context);
+    await Promise.resolve();
+  };
+
+  /**
+   * This handles when a ContentModel of NotebookPanel is changed.
+   * This occurs when a notebook file is saved and reloaded from disk.
+   */
+  handleNotebookReload = async (
+    _docContext: DocumentRegistry.IContext<INotebookModel>,
+    model: Contents.IModel,
+  ): Promise<void> => {
+    const context: PpsContext = {
+      config: this.getNotebookMetadata(),
+      notebookModel: model,
+    };
+    this._ppsContextSignal.emit(context);
+    await Promise.resolve();
   };
 
-  getNotebookMetadata = (notebook: NotebookPanel | null): any | null => {
+  getNotebookMetadata = (notebook?: NotebookPanel | null): any | null => {
+    notebook = notebook ?? this.getActiveNotebook();
     return notebook?.model?.metadata.get(METADATA_KEY);
   };
 
-  saveNotebookMetaData = (metadata: any): void => {
+  saveNotebookMetadata = (metadata: SameMetadata): void => {
     const currentNotebook = this.getActiveNotebook();
 
     if (currentNotebook !== null) {
       currentNotebook?.model?.metadata.set(METADATA_KEY, metadata);
       console.log('notebook metadata saved');
     } else {
       console.log('No active notebook');
@@ -463,20 +486,21 @@
   };
 
   setShowPipeline = (shouldShow: boolean): void => {
     if (shouldShow) {
       this._pipeline.setHidden(false);
       this._mountedList.setHidden(true);
       this._unmountedList.setHidden(true);
+      this._mountBrowser.setHidden(true);
     } else {
       this._pipeline.setHidden(true);
       this._mountedList.setHidden(false);
       this._unmountedList.setHidden(false);
+      this._mountBrowser.setHidden(false);
     }
-    this._mountBrowser.setHidden(true);
     this._config.setHidden(true);
     this._datum.setHidden(true);
     this._fullPageError.setHidden(true);
     this._showPipeline = shouldShow;
     this._showPipelineSignal.emit(shouldShow);
   };
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/mountDrive.ts` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/mountDrive.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/pollMounts.ts` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/pollMounts.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/types.ts` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/mount/types.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import {Contents} from '@jupyterlab/services';
 import {SplitPanel} from '@lumino/widgets';
 import {JSONObject} from '@lumino/coreutils';
 
 export type mountState =
   | 'unmounting'
   | 'mounted'
   | 'mounting'
@@ -82,14 +83,26 @@
 export interface IMountPlugin {
   mountedRepos: Mount[];
   unmountedRepos: Repo[];
   layout: SplitPanel;
   ready: Promise<void>;
 }
 
+export type PpsConfig = {
+  pipeline_name: string;
+  image: string;
+  requirements: string | null;
+  input_spec: any;
+};
+
+export type PpsContext = {
+  config: SameMetadata | null;
+  notebookModel: Contents.IModel | null;
+};
+
 export type SameMetadata = {
   apiVersion: string;
   environments: SameEnv;
   metadata: SameMetaMetadata;
   notebook: SameNotebookMetadata;
   run: SameRunMetadata;
 };
```

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/__tests__/telemetry.test.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/telemetry/__tests__/telemetry.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/telemetry.ts` & `jupyterlab_pachyderm-2.6.0a5/src/plugins/telemetry/telemetry.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/utils/components/Circle/Circle.tsx` & `jupyterlab_pachyderm-2.6.0a5/src/utils/components/Circle/Circle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/utils/components/LoadingDots/loadingDots.css` & `jupyterlab_pachyderm-2.6.0a5/src/utils/components/LoadingDots/loadingDots.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/GenericError.js` & `jupyterlab_pachyderm-2.6.0a5/src/utils/components/Svgs/GenericError.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/KubernetesElephant.js` & `jupyterlab_pachyderm-2.6.0a5/src/utils/components/Svgs/KubernetesElephant.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/PachydermLogo.js` & `jupyterlab_pachyderm-2.6.0a5/src/utils/components/Svgs/PachydermLogo.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/StatusWarning.js` & `jupyterlab_pachyderm-2.6.0a5/src/utils/components/Svgs/StatusWarning.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/utils/hooks/useSort.ts` & `jupyterlab_pachyderm-2.6.0a5/src/utils/hooks/useSort.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/src/utils/icons.ts` & `jupyterlab_pachyderm-2.6.0a5/src/utils/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/style/base.css` & `jupyterlab_pachyderm-2.6.0a5/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/style/components/button.css` & `jupyterlab_pachyderm-2.6.0a5/style/components/button.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/style/icons/file.svg` & `jupyterlab_pachyderm-2.6.0a5/style/icons/file.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/style/icons/info.svg` & `jupyterlab_pachyderm-2.6.0a5/style/icons/info.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/style/icons/mount-logo.svg` & `jupyterlab_pachyderm-2.6.0a5/style/icons/mount-logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a3/style/icons/repo.svg` & `jupyterlab_pachyderm-2.6.0a5/style/icons/repo.svg`

 * *Files identical despite different names*

