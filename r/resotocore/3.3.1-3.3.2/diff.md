# Comparing `tmp/resotocore-3.3.1.tar.gz` & `tmp/resotocore-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotocore-3.3.1.tar", last modified: Fri Mar 31 23:56:26 2023, max compression
+gzip compressed data, was "resotocore-3.3.2.tar", last modified: Fri Apr 14 16:19:08 2023, max compression
```

## Comparing `resotocore-3.3.1.tar` & `resotocore-3.3.2.tar`

### file list

```diff
@@ -1,683 +1,688 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.129379 resotocore-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-31 23:51:32.000000 resotocore-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-31 23:51:32.000000 resotocore-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-03-31 23:56:26.129379 resotocore-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-03-31 23:51:32.000000 resotocore-3.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-31 23:51:32.000000 resotocore-3.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-31 23:51:32.000000 resotocore-3.3.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-31 23:51:32.000000 resotocore-3.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.929377 resotocore-3.3.1/resotocore/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.933377 resotocore-3.3.1/resotocore/action_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/action_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/action_handlers/merge_outer_edge_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.933377 resotocore-3.3.1/resotocore/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/analytics/posthog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/analytics/recurrent_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/async_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.933377 resotocore-3.3.1/resotocore/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25378 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   185738 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    24733 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/cli/tip_of_the_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.937377 resotocore-3.3.1/resotocore/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/config/config_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/config/config_override_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/config/core_config_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/console_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    33828 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/core_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.937377 resotocore-3.3.1/resotocore/db/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/arango_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/arangodb_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/arangodb_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21075 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/async_arangodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/configdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/db_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/deferred_edge_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (123)    59961 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/graphdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/jobdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/modeldb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/runningtaskdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/subscriberdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/db/templatedb.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.941377 resotocore-3.3.1/resotocore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/infra_apps/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.941377 resotocore-3.3.1/resotocore/jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.917377 resotocore-3.3.1/resotocore/jupyterlite/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.941377 resotocore-3.3.1/resotocore/jupyterlite/api/contents/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-31 23:56:19.000000 resotocore-3.3.1/resotocore/jupyterlite/api/contents/all.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.941377 resotocore-3.3.1/resotocore/jupyterlite/api/translations/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-31 23:56:19.000000 resotocore-3.3.1/resotocore/jupyterlite/api/translations/all.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-31 23:56:19.000000 resotocore-3.3.1/resotocore/jupyterlite/api/translations/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/bootstrap.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.065378 resotocore-3.3.1/resotocore/jupyterlite/build/
--rw-r--r--   0 runner    (1001) docker     (123)    19955 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1008.7423996.js
--rw-r--r--   0 runner    (1001) docker     (123)     3607 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1013.c600eaa.js
--rw-r--r--   0 runner    (1001) docker     (123)     3827 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1018.8daaa2a.js
--rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1036.3f84b7c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1068.3482326.js
--rw-r--r--   0 runner    (1001) docker     (123)    31618 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1120.3846654.js
--rw-r--r--   0 runner    (1001) docker     (123)      628 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1169.ba935ce.js
--rw-r--r--   0 runner    (1001) docker     (123)     3416 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1198.25d5ea9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1735 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/125.3ad5abd.js
--rw-r--r--   0 runner    (1001) docker     (123)     9527 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1261.88c6a9a.js
--rw-r--r--   0 runner    (1001) docker     (123)    10029 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1272.44b5a6a.js
--rw-r--r--   0 runner    (1001) docker     (123)    10988 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1320.b53dabd.js
--rw-r--r--   0 runner    (1001) docker     (123)     3578 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1337.9881c6c.js
--rw-r--r--   0 runner    (1001) docker     (123)     4180 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1356.78d0573.js
--rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1385.8d43090.js
--rw-r--r--   0 runner    (1001) docker     (123)    30004 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/143.086aef9.js
--rw-r--r--   0 runner    (1001) docker     (123)    74217 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1432.2760be9.js
--rw-r--r--   0 runner    (1001) docker     (123)  1187381 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1473.34de206.js
--rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1483.b0f9bd2.js
--rw-r--r--   0 runner    (1001) docker     (123)    16451 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1496.03867f8.js
--rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1542.3a90078.js
--rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1542.3a90078.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5547 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/157.bfadd48.js
--rw-r--r--   0 runner    (1001) docker     (123)     9058 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/160.0356d0a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2329 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1615.ea9b05f.js
--rw-r--r--   0 runner    (1001) docker     (123)     2492 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1647.f9bf0fd.js
--rw-r--r--   0 runner    (1001) docker     (123)     3375 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1682.3a03166.js
--rw-r--r--   0 runner    (1001) docker     (123)     3403 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1696.8b77f15.js
--rw-r--r--   0 runner    (1001) docker     (123)     9075 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/170.c870d05.js
--rw-r--r--   0 runner    (1001) docker     (123)     3578 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1809.b7d8942.js
--rw-r--r--   0 runner    (1001) docker     (123)    12991 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1835.acefed2.js
--rw-r--r--   0 runner    (1001) docker     (123)    13117 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1898.2b94c2e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9487 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/1989.e917572.js
--rw-r--r--   0 runner    (1001) docker     (123)     5724 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2007.0515cb2.js
--rw-r--r--   0 runner    (1001) docker     (123)   114199 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2048.ae5f8ce.js
--rw-r--r--   0 runner    (1001) docker     (123)    16161 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2067.0e50352.js
--rw-r--r--   0 runner    (1001) docker     (123)     3151 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2088.e45e68d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9665 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2089.6e82794.js
--rw-r--r--   0 runner    (1001) docker     (123)     6162 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2118.57bfcca.js
--rw-r--r--   0 runner    (1001) docker     (123)      622 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2122.808d508.js
--rw-r--r--   0 runner    (1001) docker     (123)     3435 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2125.9f428bb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2492 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2167.300d308.js
--rw-r--r--   0 runner    (1001) docker     (123)     9296 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2169.a6cfcb2.js
--rw-r--r--   0 runner    (1001) docker     (123)    17632 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/217.7562b70.js
--rw-r--r--   0 runner    (1001) docker     (123)     9471 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2303.0753f62.js
--rw-r--r--   0 runner    (1001) docker     (123)     8669 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2351.b511713.js
--rw-r--r--   0 runner    (1001) docker     (123)     7915 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2359.8c659ae.js
--rw-r--r--   0 runner    (1001) docker     (123)     1736 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2363.c625bc2.js
--rw-r--r--   0 runner    (1001) docker     (123)    41794 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2364.deac00c.js
--rw-r--r--   0 runner    (1001) docker     (123)     9291 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/237.cd99ebb.js
--rw-r--r--   0 runner    (1001) docker     (123)    24451 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2401.df2b831.js
--rw-r--r--   0 runner    (1001) docker     (123)     3607 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2469.9cb78b6.js
--rw-r--r--   0 runner    (1001) docker     (123)    16704 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2476.9aabb04.js
--rw-r--r--   0 runner    (1001) docker     (123)     3335 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2526.c2108e3.js
--rw-r--r--   0 runner    (1001) docker     (123)    65885 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2527.5a42b8a.js
--rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2527.5a42b8a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2622.e5bba4b.js
--rw-r--r--   0 runner    (1001) docker     (123)     8925 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2629.26b2200.js
--rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2697.ef870be.js
--rw-r--r--   0 runner    (1001) docker     (123)    12172 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2738.6fb9dd1.js
--rw-r--r--   0 runner    (1001) docker     (123)    20976 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2753.70f3b00.js
--rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2756.3d6eaee.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2813.01f1491.js
--rw-r--r--   0 runner    (1001) docker     (123)     8593 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2834.42db52f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4206 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2897.069c887.js
--rw-r--r--   0 runner    (1001) docker     (123)     8872 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/2956.c1d7da9.js
--rw-r--r--   0 runner    (1001) docker     (123)     8062 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3004.56b6d8c.js
--rw-r--r--   0 runner    (1001) docker     (123)     8562 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3037.7c53495.js
--rw-r--r--   0 runner    (1001) docker     (123)    10138 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3051.5ce4d5e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9467 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3062.e9a281a.js
--rw-r--r--   0 runner    (1001) docker     (123)    36572 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3079.4750bec.js
--rw-r--r--   0 runner    (1001) docker     (123)    20518 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3151.a561877.js
--rw-r--r--   0 runner    (1001) docker     (123)     2949 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3154.9ecf019.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3245.c999c94.js
--rw-r--r--   0 runner    (1001) docker     (123)     8849 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/330.61992f4.js
--rw-r--r--   0 runner    (1001) docker     (123)     9565 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3301.9facff2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3325.c195954.js
--rw-r--r--   0 runner    (1001) docker     (123)     2210 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3539.29df431.js
--rw-r--r--   0 runner    (1001) docker     (123)     9556 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3546.e91daf4.js
--rw-r--r--   0 runner    (1001) docker     (123)   270612 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3562.691155b.js
--rw-r--r--   0 runner    (1001) docker     (123)     2574 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3566.ca843b7.js
--rw-r--r--   0 runner    (1001) docker     (123)    18104 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3580.9be1770.js
--rw-r--r--   0 runner    (1001) docker     (123)    83399 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3676.ebf1d93.js
--rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3733.f94f6ea.js
--rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3752.8735345.js
--rw-r--r--   0 runner    (1001) docker     (123)     9489 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3814.b631d63.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3863.2ca50c0.js
--rw-r--r--   0 runner    (1001) docker     (123)     3335 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3904.6010839.js
--rw-r--r--   0 runner    (1001) docker     (123)     2892 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3937.00a9e88.js
--rw-r--r--   0 runner    (1001) docker     (123)    10218 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/3970.1e7d81e.js
--rw-r--r--   0 runner    (1001) docker     (123)    11333 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/400.449f9c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    11918 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4018.beb2c84.js
--rw-r--r--   0 runner    (1001) docker     (123)    17697 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4030.ee05a21.js
--rw-r--r--   0 runner    (1001) docker     (123)    32438 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/404.2cfb2cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     2211 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4058.851cb1d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9853 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/406.fc80499.js
--rw-r--r--   0 runner    (1001) docker     (123)     2542 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/409.35f299f.js
--rw-r--r--   0 runner    (1001) docker     (123)      628 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4091.bd4a548.js
--rw-r--r--   0 runner    (1001) docker     (123)     2985 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4151.ef963eb.js
--rw-r--r--   0 runner    (1001) docker     (123)   244572 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4170.b007dfe.js
--rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4170.b007dfe.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8381 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4171.5fe294f.js
--rw-r--r--   0 runner    (1001) docker     (123)   119598 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4174.16d7ff2.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4174.16d7ff2.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10888 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4182.8168565.js
--rw-r--r--   0 runner    (1001) docker     (123)    34899 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4196.90d47c2.js
--rw-r--r--   0 runner    (1001) docker     (123)     9226 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4206.ce4d631.js
--rw-r--r--   0 runner    (1001) docker     (123)     8527 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4207.fcd0f7b.js
--rw-r--r--   0 runner    (1001) docker     (123)     2892 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4212.667105a.js
--rw-r--r--   0 runner    (1001) docker     (123)    10618 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4262.4153361.js
--rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4271.73da189.js
--rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4291.31bc388.js
--rw-r--r--   0 runner    (1001) docker     (123)     1550 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4354.6cee0b6.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4507.8b41ef4.js
--rw-r--r--   0 runner    (1001) docker     (123)     7854 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/451.b2fe0fb.js
--rw-r--r--   0 runner    (1001) docker     (123)     6218 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4526.b3bcff7.js
--rw-r--r--   0 runner    (1001) docker     (123)    16343 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4558.522eff3.js
--rw-r--r--   0 runner    (1001) docker     (123)    22222 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4569.ee0bb18.js
--rw-r--r--   0 runner    (1001) docker     (123)   257853 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4630.f8aa924.js
--rw-r--r--   0 runner    (1001) docker     (123)     4697 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4690.f7dbd7f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1146 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4710.705dfd0.js
--rw-r--r--   0 runner    (1001) docker     (123)    17340 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4738.7a8db62.js
--rw-r--r--   0 runner    (1001) docker     (123)    10284 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4749.d95260b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9655 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4750.dcc0917.js
--rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4758.428a798.js
--rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/48.182a12b.js
--rw-r--r--   0 runner    (1001) docker     (123)    18014 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4805.0d84a4d.js
--rw-r--r--   0 runner    (1001) docker     (123)     5148 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4811.285f48b.js
--rw-r--r--   0 runner    (1001) docker     (123)    22664 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4884.d5dcfb1.js
--rw-r--r--   0 runner    (1001) docker     (123)      626 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4885.4e89207.js
--rw-r--r--   0 runner    (1001) docker     (123)     6352 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/489.c5d6e7c.js
--rw-r--r--   0 runner    (1001) docker     (123)    15839 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4897.5fd1369.js
--rw-r--r--   0 runner    (1001) docker     (123)     4731 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/4940.d2cb952.js
--rw-r--r--   0 runner    (1001) docker     (123)    14996 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5088.b363823.js
--rw-r--r--   0 runner    (1001) docker     (123)    10344 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5115.65cbeea.js
--rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5115.65cbeea.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4569 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5126.39244e1.js
--rw-r--r--   0 runner    (1001) docker     (123)     3375 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5135.d3ad8e8.js
--rw-r--r--   0 runner    (1001) docker     (123)     6274 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5153.01e90e9.js
--rw-r--r--   0 runner    (1001) docker     (123)     2654 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5154.6495ddd.js
--rw-r--r--   0 runner    (1001) docker     (123)    15853 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/517.9f09c12.js
--rw-r--r--   0 runner    (1001) docker     (123)     1456 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/518.b1a14b5.js
--rw-r--r--   0 runner    (1001) docker     (123)   432940 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/519.87883c1.js
--rw-r--r--   0 runner    (1001) docker     (123)     9810 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5213.a606fa8.js
--rw-r--r--   0 runner    (1001) docker     (123)     8505 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5227.8d213ff.js
--rw-r--r--   0 runner    (1001) docker     (123)    27801 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5228.3d71388.js
--rw-r--r--   0 runner    (1001) docker     (123)     7677 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5234.f48a464.js
--rw-r--r--   0 runner    (1001) docker     (123)     3667 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5286.f84b4a4.js
--rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5297.8e6bad9.js
--rw-r--r--   0 runner    (1001) docker     (123)     4160 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5342.6aa187c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1071 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5394.d9ffb63.js
--rw-r--r--   0 runner    (1001) docker     (123)      597 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5426.81db440.js
--rw-r--r--   0 runner    (1001) docker     (123)   317509 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5449.484f7e1.js
--rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5449.484f7e1.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5451.e1ee9b2.js
--rw-r--r--   0 runner    (1001) docker     (123)    10582 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5489.cb188b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     9070 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/554.ce7f40d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5597.6f70034.js
--rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5614.4272b09.js
--rw-r--r--   0 runner    (1001) docker     (123)     8630 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5710.c3b4e36.js
--rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5733.4f6f25c.js
--rw-r--r--   0 runner    (1001) docker     (123)    14076 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/582.1236fdf.js
--rw-r--r--   0 runner    (1001) docker     (123)     9296 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5823.4baed9c.js
--rw-r--r--   0 runner    (1001) docker     (123)     4381 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5859.6ac4fe2.js
--rw-r--r--   0 runner    (1001) docker     (123)     9734 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/590.c297c01.js
--rw-r--r--   0 runner    (1001) docker     (123)     3667 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5914.832df6a.js
--rw-r--r--   0 runner    (1001) docker     (123)      857 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/5945.d39af99.js
--rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6061.bc854e2.js
--rw-r--r--   0 runner    (1001) docker     (123)   179193 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6118.c02b404.js
--rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6118.c02b404.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3827 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6139.ee85a5a.js
--rw-r--r--   0 runner    (1001) docker     (123)    10598 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6186.17f6a4a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2793 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6191.2feb6e6.js
--rw-r--r--   0 runner    (1001) docker     (123)     4731 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6197.15397b4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/62.d057833.js
--rw-r--r--   0 runner    (1001) docker     (123)    11113 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6256.10417ed.js
--rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6433.9e8992a.js
--rw-r--r--   0 runner    (1001) docker     (123)    82439 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/644.e6ff479.js
--rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/644.e6ff479.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6475.fe6bde7.js
--rw-r--r--   0 runner    (1001) docker     (123)     7234 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6517.7379adf.js
--rw-r--r--   0 runner    (1001) docker     (123)     9340 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6553.5e1599f.js
--rw-r--r--   0 runner    (1001) docker     (123)    10588 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6576.d5ddce4.js
--rw-r--r--   0 runner    (1001) docker     (123)     3151 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6604.715e4c0.js
--rw-r--r--   0 runner    (1001) docker     (123)     7390 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6612.2f9795e.js
--rw-r--r--   0 runner    (1001) docker     (123)      592 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6627.53ac590.js
--rw-r--r--   0 runner    (1001) docker     (123)     4801 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6648.bfe5243.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6648.bfe5243.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16152 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6664.1b4a72f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4801 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6731.5beaf61.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6731.5beaf61.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   478371 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6787.2bc4778.js
--rw-r--r--   0 runner    (1001) docker     (123)     2275 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6815.24389cc.js
--rw-r--r--   0 runner    (1001) docker     (123)     8963 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6870.af50acc.js
--rw-r--r--   0 runner    (1001) docker     (123)     6734 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6891.f98d014.js
--rw-r--r--   0 runner    (1001) docker     (123)    10258 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6952.f9a7329.js
--rw-r--r--   0 runner    (1001) docker     (123)     2210 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6962.db53086.js
--rw-r--r--   0 runner    (1001) docker     (123)   897353 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6974.6305cd0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6974.6305cd0.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4964 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6981.bcfe168.js
--rw-r--r--   0 runner    (1001) docker     (123)    28402 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/6990.9bf8f0c.js
--rw-r--r--   0 runner    (1001) docker     (123)     4642 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7010.d9a3d9a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2945 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7071.ac3061a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2654 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7125.6e03225.js
--rw-r--r--   0 runner    (1001) docker     (123)    35481 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7144.7b79049.js
--rw-r--r--   0 runner    (1001) docker     (123)    89401 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/724.6d5bce9.js
--rw-r--r--   0 runner    (1001) docker     (123)     2056 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7252.1b222e2.js
--rw-r--r--   0 runner    (1001) docker     (123)    35262 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7334.4b1185b.js
--rw-r--r--   0 runner    (1001) docker     (123)     2985 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7353.1f669cb.js
--rw-r--r--   0 runner    (1001) docker     (123)     8499 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7359.3fb41a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     3570 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7364.5e98a3d.js
--rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7378.9a1e27c.js
--rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7378.9a1e27c.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9119 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7380.1f65978.js
--rw-r--r--   0 runner    (1001) docker     (123)     5148 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7386.39139e0.js
--rw-r--r--   0 runner    (1001) docker     (123)    28014 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7495.54216ce.js
--rw-r--r--   0 runner    (1001) docker     (123)     4642 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7505.3011f14.js
--rw-r--r--   0 runner    (1001) docker     (123)    10360 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7509.5ca0029.js
--rw-r--r--   0 runner    (1001) docker     (123)    10080 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7692.7e69e41.js
--rw-r--r--   0 runner    (1001) docker     (123)    91612 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7702.0a89622.js
--rw-r--r--   0 runner    (1001) docker     (123)    22414 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7749.06b09da.js
--rw-r--r--   0 runner    (1001) docker     (123)    10756 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7808.d290935.js
--rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7819.9d50d5e.js
--rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7821.254b995.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7821.254b995.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9194 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7858.cdac98e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7892.762d4af.js
--rw-r--r--   0 runner    (1001) docker     (123)     3004 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/7900.9103464.js
--rw-r--r--   0 runner    (1001) docker     (123)     7968 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8028.1bab409.js
--rw-r--r--   0 runner    (1001) docker     (123)      626 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8072.dc7057b.js
--rw-r--r--   0 runner    (1001) docker     (123)     7134 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8131.aeaee1d.js
--rw-r--r--   0 runner    (1001) docker     (123)     8588 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8199.7c3ab4f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1070 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/827.5f79f4c.js
--rw-r--r--   0 runner    (1001) docker     (123)    16357 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/835.4e4132e.js
--rw-r--r--   0 runner    (1001) docker     (123)     4160 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8370.1f0c2e7.js
--rw-r--r--   0 runner    (1001) docker     (123)     2949 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8393.f15a1fb.js
--rw-r--r--   0 runner    (1001) docker     (123)     4964 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8402.41ac88b.js
--rw-r--r--   0 runner    (1001) docker     (123)     6827 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8412.a71c56e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9363 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8427.a0a5b2f.js
--rw-r--r--   0 runner    (1001) docker     (123)     7234 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8445.12eb406.js
--rw-r--r--   0 runner    (1001) docker     (123)     4005 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8476.c861e5b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4180 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8498.51d4fad.js
--rw-r--r--   0 runner    (1001) docker     (123)    31212 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/850.4167ce1.js
--rw-r--r--   0 runner    (1001) docker     (123)    10443 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8579.76adee3.js
--rw-r--r--   0 runner    (1001) docker     (123)     7430 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8590.675efe0.js
--rw-r--r--   0 runner    (1001) docker     (123)     4206 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8633.4815201.js
--rw-r--r--   0 runner    (1001) docker     (123)    80814 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8695.7f3578a.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8741.b138cb8.js
--rw-r--r--   0 runner    (1001) docker     (123)     4381 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8754.a42dc19.js
--rw-r--r--   0 runner    (1001) docker     (123)      857 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8800.ee578b6.js
--rw-r--r--   0 runner    (1001) docker     (123)     3416 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8907.f1da997.js
--rw-r--r--   0 runner    (1001) docker     (123)     3004 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8928.eff2684.js
--rw-r--r--   0 runner    (1001) docker     (123)   131445 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8929.ae99e1f.js
--rw-r--r--   0 runner    (1001) docker     (123)    17920 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/893.39e9e3c.js
--rw-r--r--   0 runner    (1001) docker     (123)     9760 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/8976.976490c.js
--rw-r--r--   0 runner    (1001) docker     (123)     7969 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/901.d40d0d6.js
--rw-r--r--   0 runner    (1001) docker     (123)     9691 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9077.19ea7ca.js
--rw-r--r--   0 runner    (1001) docker     (123)   170789 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/911.07e91f9.js
--rw-r--r--   0 runner    (1001) docker     (123)     9227 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9156.8248119.js
--rw-r--r--   0 runner    (1001) docker     (123)    10651 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9196.ed69b45.js
--rw-r--r--   0 runner    (1001) docker     (123)     3038 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9208.057fe7d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9222.03d0ecd.js
--rw-r--r--   0 runner    (1001) docker     (123)     8835 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9244.f067be9.js
--rw-r--r--   0 runner    (1001) docker     (123)     3038 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9282.60b94bc.js
--rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9334.d61a1e4.js
--rw-r--r--   0 runner    (1001) docker     (123)    47298 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9341.3bb43d7.js
--rw-r--r--   0 runner    (1001) docker     (123)     1342 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9372.a388c7b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9208 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9602.7bfe4d6.js
--rw-r--r--   0 runner    (1001) docker     (123)     9383 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9621.7698d7d.js
--rw-r--r--   0 runner    (1001) docker     (123)    10561 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9647.329ecda.js
--rw-r--r--   0 runner    (1001) docker     (123)     1550 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9684.c0b5cc1.js
--rw-r--r--   0 runner    (1001) docker     (123)     2056 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9685.9c6e5f6.js
--rw-r--r--   0 runner    (1001) docker     (123)     8835 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9847.75e3ee6.js
--rw-r--r--   0 runner    (1001) docker     (123)      433 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9866.fd87dbe.js
--rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9934.0330010.js
--rw-r--r--   0 runner    (1001) docker     (123)     4766 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/9939.a757e1d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/add-above.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/add-below.svg
--rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/add.svg
--rw-r--r--   0 runner    (1001) docker     (123)       57 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/all.json
--rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/bug-dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/bug.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/build.svg
--rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/caret-down-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/caret-down-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/caret-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/caret-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/caret-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/caret-up-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/caret-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/case-sensitive.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/check.svg
--rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/circle-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/circle.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/clear.svg
--rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/console.svg
--rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/copy.svg
--rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/copyright.svg
--rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/cut.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/delete.svg
--rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/duplicate.svg
--rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/edit.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/ellipses.svg
--rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/extension.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/fast-forward.svg
--rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/file-upload.svg
--rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/filter-list.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/folder-favorite.svg
--rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/html5.svg
--rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/inspector.svg
--rw-r--r--   0 runner    (1001) docker     (123)       81 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/ipykernel-6.9.2-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/json.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/julia.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/jupyter-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/jupyter.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/keyboard.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.065378 resotocore-3.3.1/resotocore/jupyterlite/build/lab/
--rw-r--r--   0 runner    (1001) docker     (123)    55096 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/lab/bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/launch.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/launcher.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/line-form.svg
--rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/list.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/listings-info.svg
--rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/markdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/move-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/move-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/new-folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/not-trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/notebook.svg
--rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/numbering.svg
--rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/offline-bolt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/palette.svg
--rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/paste.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)       82 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/piplite-0.1.0b13-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)       82 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/pyolite-0.1.0b13-py3-none-any.whl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.069378 resotocore-3.3.1/resotocore/jupyterlite/build/pypi/
--rw-r--r--   0 runner    (1001) docker     (123)     4267 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/pypi/all.json
--rw-r--r--   0 runner    (1001) docker     (123)     4203 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/pypi/ipykernel-6.9.2-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     4857 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/pypi/piplite-0.1.0b13-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     6716 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/pypi/pyolite-0.1.0b13-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     2302 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/pypi/widgetsnbextension-3.6.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     2300 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/pypi/widgetsnbextension-4.0.2-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/python.svg
--rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/r-kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/react.svg
--rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/redo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/regex.svg
--rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/run.svg
--rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/running.svg
--rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/save.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.069378 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.921377 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.069378 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
--rw-r--r--   0 runner    (1001) docker     (123)      529 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
--rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.073378 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
--rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
--rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.073378 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.073378 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.073378 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.073378 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
--rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.077379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.077379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)     3358 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.077379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.077379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     5785 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
--rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
--rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.077379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.081379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
--rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
--rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.081379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.081379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.081379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.081379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.081379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.081379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.085379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.085379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
--rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
--rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.085379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
--rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.085379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.085379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.085379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.085379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.089379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.921377 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@retrolab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.089379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.089379 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
--rw-r--r--   0 runner    (1001) docker     (123)    78986 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/schemas/all.json
--rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/search.svg
--rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/settings.svg
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/spreadsheet.svg
--rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/table-rows.svg
--rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/tag.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/terminal.svg
--rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/text-editor.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.921377 resotocore-3.3.1/resotocore/jupyterlite/build/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.921377 resotocore-3.3.1/resotocore/jupyterlite/build/themes/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.089379 resotocore-3.3.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.089379 resotocore-3.3.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)   330163 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/toc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/tree-view.svg
--rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/vega.svg
--rw-r--r--   0 runner    (1001) docker     (123)       90 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/widgetsnbextension-3.6.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)       90 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/widgetsnbextension-4.0.2-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/build/yaml.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/config-utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.921377 resotocore-3.3.1/resotocore/jupyterlite/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.089379 resotocore-3.3.1/resotocore/jupyterlite/doc/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/doc/workspaces/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.921377 resotocore-3.3.1/resotocore/jupyterlite/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.089379 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-03-31 23:56:03.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.101379 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-03-31 23:56:03.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.e171e024d2412b46d706.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-03-31 23:56:03.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
--rw-rw-rw-   0 runner    (1001) docker     (123)  3573673 2023-03-31 23:56:03.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.04c1d88665796339989c.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-03-31 23:56:03.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.04c1d88665796339989c.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-03-31 23:56:03.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-03-31 23:56:03.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-03-31 23:56:03.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.e12be0c175cda2484e38.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-03-31 23:56:03.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-03-31 23:56:03.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.5a61eaf4adea42288d59.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-03-31 23:56:03.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-03-31 23:56:03.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.101379 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/
--rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-03-31 23:55:58.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-03-31 23:55:58.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.101379 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-03-31 23:55:58.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-03-31 23:55:58.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-03-31 23:55:58.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-03-31 23:55:58.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-03-31 23:55:58.000000 resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.105379 resotocore-3.3.1/resotocore/jupyterlite/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/jupyterlite/files/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/icon-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-03-31 23:56:19.000000 resotocore-3.3.1/resotocore/jupyterlite/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    12959 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/jupyterlite.schema.v0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.105379 resotocore-3.3.1/resotocore/jupyterlite/kernelspecs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/kernelspecs/javascript.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/kernelspecs/python.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.105379 resotocore-3.3.1/resotocore/jupyterlite/lab/
--rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/lab/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/lab/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/lab/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/lab/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    10497 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/lab/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.105379 resotocore-3.3.1/resotocore/jupyterlite/lab/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/lab/tree/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.105379 resotocore-3.3.1/resotocore/jupyterlite/lab/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/lab/workspaces/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     1261 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2632 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/piplite.schema.v0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2531 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.109379 resotocore-3.3.1/resotocore/jupyterlite/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.3.1/resotocore/jupyterlite/tree/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.109379 resotocore-3.3.1/resotocore/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/model/adjust_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/model/db_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    24326 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/model/graph_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/model/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    54844 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/model/model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/model/resolve_in_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/model/transform_kind_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/model/typed_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.113379 resotocore-3.3.1/resotocore/query/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43690 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/query/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14490 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/query/query_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/query/template_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/query/template_expander_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.117379 resotocore-3.3.1/resotocore/report/
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/report/inspector_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/report/report_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.117379 resotocore-3.3.1/resotocore/static/
--rw-r--r--   0 runner    (1001) docker     (123)   112506 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/api-doc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/ck-unicode-truecolor.ans
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.121379 resotocore-3.3.1/resotocore/static/report/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.925377 resotocore-3.3.1/resotocore/static/report/benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.121379 resotocore-3.3.1/resotocore/static/report/benchmark/aws/
--rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/report/benchmark_template.json
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/report/check_template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.925377 resotocore-3.3.1/resotocore/static/report/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.121379 resotocore-3.3.1/resotocore/static/report/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/report/checks/aws/aws_apigateway.json
--rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/report/checks/aws/aws_cloudtrail.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/report/checks/aws/aws_config.json
--rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/report/checks/aws/aws_ec2.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/report/checks/aws/aws_efs.json
--rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/report/checks/aws/aws_iam.json
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/report/checks/aws/aws_kms.json
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/report/checks/aws/aws_lambda.json
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/report/checks/aws/aws_rds.json
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/static/report/checks/aws/aws_s3.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.125379 resotocore-3.3.1/resotocore/task/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/task/job_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/task/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/task/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/task/start_workflow_on_first_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/task/subscribers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30960 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/task/task_description.py
--rw-r--r--   0 runner    (1001) docker     (123)    27785 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/task/task_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:26.129379 resotocore-3.3.1/resotocore/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58108 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/web/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/web/certificate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/web/content_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/web/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/web/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/web/tsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-03-31 23:51:32.000000 resotocore-3.3.1/resotocore/worker_task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 23:56:25.933377 resotocore-3.3.1/resotocore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-03-31 23:56:25.000000 resotocore-3.3.1/resotocore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28786 2023-03-31 23:56:25.000000 resotocore-3.3.1/resotocore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 23:56:25.000000 resotocore-3.3.1/resotocore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-31 23:56:25.000000 resotocore-3.3.1/resotocore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-31 23:56:25.000000 resotocore-3.3.1/resotocore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-31 23:56:25.000000 resotocore-3.3.1/resotocore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-31 23:56:26.129379 resotocore-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-03-31 23:51:32.000000 resotocore-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.204301 resotocore-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 16:15:47.000000 resotocore-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-14 16:15:47.000000 resotocore-3.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-04-14 16:19:08.204301 resotocore-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-14 16:15:47.000000 resotocore-3.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-14 16:15:47.000000 resotocore-3.3.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-14 16:15:47.000000 resotocore-3.3.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-14 16:15:47.000000 resotocore-3.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.108301 resotocore-3.3.2/resotocore/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.108301 resotocore-3.3.2/resotocore/action_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/action_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/action_handlers/merge_outer_edge_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.108301 resotocore-3.3.2/resotocore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/analytics/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/analytics/recurrent_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/async_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.108301 resotocore-3.3.2/resotocore/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27590 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   207248 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26213 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/cli/tip_of_the_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.108301 resotocore-3.3.2/resotocore/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/config/config_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/config/config_override_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/config/core_config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/console_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33828 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/core_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.120301 resotocore-3.3.2/resotocore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/arango_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/arangodb_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/arangodb_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21075 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/async_arangodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/configdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/db_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/deferred_edge_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59961 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/graphdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/jobdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/modeldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/packagedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/runningtaskdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/subscriberdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/db/templatedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.124301 resotocore-3.3.2/resotocore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/infra_apps/local_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/infra_apps/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/infra_apps/package_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/infra_apps/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.124301 resotocore-3.3.2/resotocore/jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.088302 resotocore-3.3.2/resotocore/jupyterlite/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.124301 resotocore-3.3.2/resotocore/jupyterlite/api/contents/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-14 16:19:03.000000 resotocore-3.3.2/resotocore/jupyterlite/api/contents/all.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.124301 resotocore-3.3.2/resotocore/jupyterlite/api/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 16:19:03.000000 resotocore-3.3.2/resotocore/jupyterlite/api/translations/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 16:19:03.000000 resotocore-3.3.2/resotocore/jupyterlite/api/translations/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/bootstrap.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.184301 resotocore-3.3.2/resotocore/jupyterlite/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    19955 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1008.7423996.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1013.c600eaa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1018.8daaa2a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1036.3f84b7c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1068.3482326.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31618 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1120.3846654.js
+-rw-r--r--   0 runner    (1001) docker     (123)      628 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1169.ba935ce.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1198.25d5ea9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/125.3ad5abd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1261.88c6a9a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10029 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1272.44b5a6a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1320.b53dabd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1337.9881c6c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1356.78d0573.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1385.8d43090.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30004 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/143.086aef9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74217 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1432.2760be9.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1187381 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1473.34de206.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1483.b0f9bd2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16451 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1496.03867f8.js
+-rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1542.3a90078.js
+-rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1542.3a90078.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/157.bfadd48.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/160.0356d0a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1615.ea9b05f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1647.f9bf0fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1682.3a03166.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1696.8b77f15.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/170.c870d05.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1809.b7d8942.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1835.acefed2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13117 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1898.2b94c2e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/1989.e917572.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2007.0515cb2.js
+-rw-r--r--   0 runner    (1001) docker     (123)   114199 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2048.ae5f8ce.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16161 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2067.0e50352.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2088.e45e68d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2089.6e82794.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2118.57bfcca.js
+-rw-r--r--   0 runner    (1001) docker     (123)      622 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2122.808d508.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2125.9f428bb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2167.300d308.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2169.a6cfcb2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/217.7562b70.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2303.0753f62.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2351.b511713.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2359.8c659ae.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2363.c625bc2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41794 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2364.deac00c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/237.cd99ebb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24451 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2401.df2b831.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2469.9cb78b6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16704 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2476.9aabb04.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2526.c2108e3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    65885 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2527.5a42b8a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2527.5a42b8a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2622.e5bba4b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2629.26b2200.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2697.ef870be.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12172 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2738.6fb9dd1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20976 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2753.70f3b00.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2756.3d6eaee.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2813.01f1491.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2834.42db52f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2897.069c887.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/2956.c1d7da9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3004.56b6d8c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3037.7c53495.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3051.5ce4d5e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3062.e9a281a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36572 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3079.4750bec.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20518 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3151.a561877.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3154.9ecf019.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3245.c999c94.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/330.61992f4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3301.9facff2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3325.c195954.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3539.29df431.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3546.e91daf4.js
+-rw-r--r--   0 runner    (1001) docker     (123)   270612 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3562.691155b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3566.ca843b7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18104 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3580.9be1770.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83399 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3676.ebf1d93.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3733.f94f6ea.js
+-rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3752.8735345.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9489 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3814.b631d63.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3863.2ca50c0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3904.6010839.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3937.00a9e88.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/3970.1e7d81e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/400.449f9c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11918 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4018.beb2c84.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17697 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4030.ee05a21.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32438 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/404.2cfb2cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4058.851cb1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9853 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/406.fc80499.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/409.35f299f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      628 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4091.bd4a548.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4151.ef963eb.js
+-rw-r--r--   0 runner    (1001) docker     (123)   244572 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4170.b007dfe.js
+-rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4170.b007dfe.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4171.5fe294f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   119598 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4174.16d7ff2.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4174.16d7ff2.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4182.8168565.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34899 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4196.90d47c2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4206.ce4d631.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4207.fcd0f7b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4212.667105a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4262.4153361.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4271.73da189.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4291.31bc388.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4354.6cee0b6.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4507.8b41ef4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/451.b2fe0fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4526.b3bcff7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16343 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4558.522eff3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22222 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4569.ee0bb18.js
+-rw-r--r--   0 runner    (1001) docker     (123)   257853 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4630.f8aa924.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4690.f7dbd7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4710.705dfd0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17340 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4738.7a8db62.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4749.d95260b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9655 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4750.dcc0917.js
+-rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4758.428a798.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/48.182a12b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4805.0d84a4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4811.285f48b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22664 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4884.d5dcfb1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      626 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4885.4e89207.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/489.c5d6e7c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15839 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4897.5fd1369.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/4940.d2cb952.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14996 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5088.b363823.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5115.65cbeea.js
+-rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5115.65cbeea.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5126.39244e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5135.d3ad8e8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5153.01e90e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5154.6495ddd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15853 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/517.9f09c12.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/518.b1a14b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)   432940 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/519.87883c1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5213.a606fa8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5227.8d213ff.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27801 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5228.3d71388.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5234.f48a464.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5286.f84b4a4.js
+-rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5297.8e6bad9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5342.6aa187c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5394.d9ffb63.js
+-rw-r--r--   0 runner    (1001) docker     (123)      597 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5426.81db440.js
+-rw-r--r--   0 runner    (1001) docker     (123)   317509 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5449.484f7e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5449.484f7e1.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5451.e1ee9b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5489.cb188b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/554.ce7f40d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5597.6f70034.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5614.4272b09.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5710.c3b4e36.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5733.4f6f25c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14076 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/582.1236fdf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5823.4baed9c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5859.6ac4fe2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/590.c297c01.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5914.832df6a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      857 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/5945.d39af99.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6061.bc854e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)   179193 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6118.c02b404.js
+-rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6118.c02b404.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6139.ee85a5a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6186.17f6a4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6191.2feb6e6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6197.15397b4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/62.d057833.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6256.10417ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6433.9e8992a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    82439 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/644.e6ff479.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/644.e6ff479.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6475.fe6bde7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6517.7379adf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6553.5e1599f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6576.d5ddce4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6604.715e4c0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6612.2f9795e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      592 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6627.53ac590.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6648.bfe5243.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6648.bfe5243.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16152 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6664.1b4a72f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6731.5beaf61.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6731.5beaf61.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   478371 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6787.2bc4778.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6815.24389cc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6870.af50acc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6891.f98d014.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6952.f9a7329.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6962.db53086.js
+-rw-r--r--   0 runner    (1001) docker     (123)   897353 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6974.6305cd0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6974.6305cd0.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6981.bcfe168.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28402 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/6990.9bf8f0c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7010.d9a3d9a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7071.ac3061a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7125.6e03225.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35481 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7144.7b79049.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89401 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/724.6d5bce9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7252.1b222e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35262 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7334.4b1185b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7353.1f669cb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7359.3fb41a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7364.5e98a3d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7378.9a1e27c.js
+-rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7378.9a1e27c.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9119 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7380.1f65978.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7386.39139e0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28014 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7495.54216ce.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7505.3011f14.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7509.5ca0029.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7692.7e69e41.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91612 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7702.0a89622.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22414 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7749.06b09da.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7808.d290935.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7819.9d50d5e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7821.254b995.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7821.254b995.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7858.cdac98e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7892.762d4af.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/7900.9103464.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8028.1bab409.js
+-rw-r--r--   0 runner    (1001) docker     (123)      626 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8072.dc7057b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8131.aeaee1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8199.7c3ab4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/827.5f79f4c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16357 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/835.4e4132e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8370.1f0c2e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8393.f15a1fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8402.41ac88b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8412.a71c56e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8427.a0a5b2f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8445.12eb406.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8476.c861e5b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8498.51d4fad.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31212 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/850.4167ce1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8579.76adee3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8590.675efe0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8633.4815201.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80814 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8695.7f3578a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8741.b138cb8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8754.a42dc19.js
+-rw-r--r--   0 runner    (1001) docker     (123)      857 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8800.ee578b6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8907.f1da997.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8928.eff2684.js
+-rw-r--r--   0 runner    (1001) docker     (123)   131445 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8929.ae99e1f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17920 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/893.39e9e3c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/8976.976490c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/901.d40d0d6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9077.19ea7ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)   170789 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/911.07e91f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9156.8248119.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9196.ed69b45.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9208.057fe7d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9222.03d0ecd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9244.f067be9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9282.60b94bc.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9334.d61a1e4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    47298 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9341.3bb43d7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9372.a388c7b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9602.7bfe4d6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9621.7698d7d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9647.329ecda.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9684.c0b5cc1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9685.9c6e5f6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9847.75e3ee6.js
+-rw-r--r--   0 runner    (1001) docker     (123)      433 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9866.fd87dbe.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9934.0330010.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/9939.a757e1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/add-above.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/add-below.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/add.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       57 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/bug-dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/bug.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/build.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/caret-down-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/caret-down-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/caret-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/caret-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/caret-up-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/caret-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/case-sensitive.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/check.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/circle-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/clear.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/console.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/copyright.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/cut.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/duplicate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/ellipses.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/extension.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/fast-forward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/file-upload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/filter-list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/folder-favorite.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/html5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/inspector.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       81 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/ipykernel-6.9.2-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/json.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/julia.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/jupyter-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/jupyter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/keyboard.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.184301 resotocore-3.3.2/resotocore/jupyterlite/build/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)    55096 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/lab/bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/launch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/launcher.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/line-form.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/listings-info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/markdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/move-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/move-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/new-folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/not-trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/notebook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/numbering.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/offline-bolt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/palette.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/paste.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       82 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/piplite-0.1.0b13-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)       82 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/pyolite-0.1.0b13-py3-none-any.whl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.184301 resotocore-3.3.2/resotocore/jupyterlite/build/pypi/
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/pypi/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/pypi/ipykernel-6.9.2-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/pypi/piplite-0.1.0b13-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/pypi/pyolite-0.1.0b13-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/pypi/widgetsnbextension-3.6.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/pypi/widgetsnbextension-4.0.2-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/python.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/r-kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/react.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/regex.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/run.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/running.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/save.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.184301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.096301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.184301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      529 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.184301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.184301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.184301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.184301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.184301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
+-rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.188301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.192301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.192301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.096301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@retrolab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.192301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.192301 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
+-rw-r--r--   0 runner    (1001) docker     (123)    78986 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/schemas/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/spreadsheet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/table-rows.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/tag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/text-editor.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.096301 resotocore-3.3.2/resotocore/jupyterlite/build/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.096301 resotocore-3.3.2/resotocore/jupyterlite/build/themes/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.192301 resotocore-3.3.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.192301 resotocore-3.3.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)   330163 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/toc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/tree-view.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/vega.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       90 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/widgetsnbextension-3.6.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)       90 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/widgetsnbextension-4.0.2-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/build/yaml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/config-utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.096301 resotocore-3.3.2/resotocore/jupyterlite/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.192301 resotocore-3.3.2/resotocore/jupyterlite/doc/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/doc/workspaces/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.096301 resotocore-3.3.2/resotocore/jupyterlite/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.192301 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-04-14 16:18:53.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.196301 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-04-14 16:18:53.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.e171e024d2412b46d706.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-04-14 16:18:53.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)  3573673 2023-04-14 16:18:53.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.04c1d88665796339989c.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-04-14 16:18:53.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.04c1d88665796339989c.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-04-14 16:18:53.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-04-14 16:18:53.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-04-14 16:18:53.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.e12be0c175cda2484e38.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-04-14 16:18:53.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-04-14 16:18:53.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.5a61eaf4adea42288d59.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-04-14 16:18:53.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-04-14 16:18:53.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.196301 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-04-14 16:18:50.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-04-14 16:18:50.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.196301 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-04-14 16:18:50.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-04-14 16:18:50.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-04-14 16:18:50.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-04-14 16:18:50.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-04-14 16:18:50.000000 resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.196301 resotocore-3.3.2/resotocore/jupyterlite/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/jupyterlite/files/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/icon-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-04-14 16:19:03.000000 resotocore-3.3.2/resotocore/jupyterlite/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/jupyterlite.schema.v0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.196301 resotocore-3.3.2/resotocore/jupyterlite/kernelspecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/kernelspecs/javascript.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/kernelspecs/python.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.200301 resotocore-3.3.2/resotocore/jupyterlite/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/lab/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/lab/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/lab/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/lab/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10497 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/lab/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.200301 resotocore-3.3.2/resotocore/jupyterlite/lab/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/lab/tree/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.200301 resotocore-3.3.2/resotocore/jupyterlite/lab/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/lab/workspaces/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/piplite.schema.v0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.200301 resotocore-3.3.2/resotocore/jupyterlite/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.3.2/resotocore/jupyterlite/tree/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.200301 resotocore-3.3.2/resotocore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/model/adjust_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/model/db_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24326 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/model/graph_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/model/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54880 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/model/model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/model/resolve_in_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/model/transform_kind_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/model/typed_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.200301 resotocore-3.3.2/resotocore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43690 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/query/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14490 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/query/query_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/query/template_expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/query/template_expander_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.200301 resotocore-3.3.2/resotocore/report/
+-rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/report/benchmark_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17911 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/report/inspector_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/report/report_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.200301 resotocore-3.3.2/resotocore/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   112506 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/api-doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/ck-unicode-truecolor.ans
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.200301 resotocore-3.3.2/resotocore/static/report/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.104301 resotocore-3.3.2/resotocore/static/report/benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.200301 resotocore-3.3.2/resotocore/static/report/benchmark/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/report/benchmark_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/report/check_template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.104301 resotocore-3.3.2/resotocore/static/report/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.204301 resotocore-3.3.2/resotocore/static/report/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/report/checks/aws/aws_apigateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/report/checks/aws/aws_cloudtrail.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/report/checks/aws/aws_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/report/checks/aws/aws_ec2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/report/checks/aws/aws_efs.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/report/checks/aws/aws_iam.json
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/report/checks/aws/aws_kms.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/report/checks/aws/aws_lambda.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/report/checks/aws/aws_rds.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/static/report/checks/aws/aws_s3.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.204301 resotocore-3.3.2/resotocore/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/task/job_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/task/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/task/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/task/start_workflow_on_first_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/task/subscribers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30960 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/task/task_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27785 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/task/task_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.204301 resotocore-3.3.2/resotocore/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58057 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/web/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/web/certificate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/web/content_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/web/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/web/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/web/tsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-14 16:15:47.000000 resotocore-3.3.2/resotocore/worker_task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:08.108301 resotocore-3.3.2/resotocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-04-14 16:19:08.000000 resotocore-3.3.2/resotocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28966 2023-04-14 16:19:08.000000 resotocore-3.3.2/resotocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:19:08.000000 resotocore-3.3.2/resotocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 16:19:08.000000 resotocore-3.3.2/resotocore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-14 16:19:08.000000 resotocore-3.3.2/resotocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 16:19:08.000000 resotocore-3.3.2/resotocore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-14 16:19:08.204301 resotocore-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-14 16:15:47.000000 resotocore-3.3.2/setup.py
```

### Comparing `resotocore-3.3.1/LICENSE` & `resotocore-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/PKG-INFO` & `resotocore-3.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.3.1
+Version: 3.3.2
 Summary: Keeps all the things.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotocore
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `resotocore-3.3.1/README.md` & `resotocore-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/requirements.txt` & `resotocore-3.3.2/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 python-dateutil==2.8.2
 toolz==0.12.0
 transitions==0.9.0
 APScheduler==3.10.0
 aiostream==0.4.5
 tzlocal==4.2
 frozendict==2.1.3 # 2.2.0 can not be marshalled as json any longer
-resotolib==3.3.1
+resotolib==3.3.2
 jq==1.4.0
 posthog==2.3.1
 ustache==0.1.5
 aiofiles==23.1.0
 cryptography>=38.0.4
-rich==13.3.1
+rich==13.3.2
 Cerberus~=1.3.4
 setuptools>=65.5.3 # not directly required, pinned by Snyk to avoid a vulnerability
 resotoui==3.3.1
 deepdiff==6.2.3
-Jinja2==3.1.2
+Jinja2==3.1.2
```

### Comparing `resotocore-3.3.1/resotocore/__main__.py` & `resotocore-3.3.2/resotocore/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 from resotocore.task.scheduler import Scheduler
 from resotocore.task.subscribers import SubscriptionHandler
 from resotocore.task.task_handler import TaskHandlerService
 from resotocore.util import shutdown_process, utc
 from resotocore.web.api import Api
 from resotocore.web.certificate_handler import CertificateHandler
 from resotocore.worker_task_queue import WorkerTaskQueue
+from resotocore.infra_apps.local_runtime import LocalResotocoreAppRuntime
+from resotocore.infra_apps.package_manager import PackageManager
 from resotolib.asynchronous.web import runner
 
 log = logging.getLogger("resotocore")
 
 
 def main() -> None:
     """
@@ -173,14 +175,18 @@
         db.running_task_db, db.job_db, message_bus, event_sender, subscriptions, scheduler, cli, config
     )
     core_config_handler = CoreConfigHandler(
         config, message_bus, worker_task_queue, config_handler, event_sender, inspector
     )
     merge_outer_edges_handler = MergeOuterEdgesHandler(message_bus, subscriptions, task_handler, db, model)
     cli_deps.extend(task_handler=task_handler, inspector=inspector)
+    infra_apps_runtime = LocalResotocoreAppRuntime(cli)
+    cli_deps.extend(infra_apps_runtime=infra_apps_runtime)
+    infra_apps_package_manager = PackageManager(db.package_entity_db, config_handler)
+    cli_deps.extend(infra_apps_package_manager=infra_apps_package_manager)
     api = Api(
         db,
         model,
         subscriptions,
         task_handler,
         message_bus,
         event_sender,
@@ -212,14 +218,15 @@
         await config_override_service.start()
         await config_handler.start()
         await core_config_handler.start()
         await merge_outer_edges_handler.start()
         await cert_handler.start()
         await log_ship.start()
         await api.start()
+        await infra_apps_package_manager.start()
         if created:
             docker = inside_docker()
             kubernetes = inside_kubernetes()
             helm = helm_installation()
             await event_sender.core_event(
                 CoreEvent.SystemInstalled,
                 {
@@ -241,14 +248,15 @@
             cpu_count=info.cpus,
             mem_total=info.mem_total,
             mem_available=info.mem_available,
         )
 
     async def on_stop() -> None:
         duration = utc() - info.started_at
+        await infra_apps_package_manager.stop()
         await api.stop()
         await log_ship.stop()
         await cert_handler.stop()
         await config_override_service.stop()
         await core_config_handler.stop()
         await merge_outer_edges_handler.stop()
         await task_handler.stop()
```

### Comparing `resotocore-3.3.1/resotocore/action_handlers/merge_outer_edge_handler.py` & `resotocore-3.3.2/resotocore/action_handlers/merge_outer_edge_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/analytics/__init__.py` & `resotocore-3.3.2/resotocore/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/analytics/posthog.py` & `resotocore-3.3.2/resotocore/analytics/posthog.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/analytics/recurrent_events.py` & `resotocore-3.3.2/resotocore/analytics/recurrent_events.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/async_extensions.py` & `resotocore-3.3.2/resotocore/async_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/cli/__init__.py` & `resotocore-3.3.2/resotocore/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/cli/cli.py` & `resotocore-3.3.2/resotocore/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     SearchCLIPart,
     ExecuteSearchCommand,
     JobsCommand,
     WelcomeCommand,
     SortPart,
     LimitPart,
     HistoryPart,
+    ReportCommand,
+    WriteCommand,
 )
 from resotocore.cli.model import (
     ParsedCommand,
     ParsedCommands,
     ExecutableCommand,
     ParsedCommandLine,
     CLICommand,
@@ -51,14 +53,16 @@
     CLISource,
     NoTerminalOutput,
     AliasTemplate,
     ArgsInfo,
     ArgInfo,
     AliasTemplateParameter,
     WorkerCustomCommand,
+    OutputTransformer,
+    PreserveOutputFormat,
 )
 from resotocore.console_renderer import ConsoleRenderer
 from resotocore.error import CLIParseError
 from resotocore.model.typed_model import class_fqn
 from resotocore.query.model import (
     Query,
     Navigation,
@@ -289,28 +293,30 @@
                     res = await task
                     log.info(f"Spawned task {info} completed with: {res}")
                 except Exception as ex:
                     log.info(f"Spawned task {info} failed. Reason {ex}")
             except Exception as ex:
                 log.warning(f"Error in main loop: {ex}")
 
-    def command(self, name: str, arg: Optional[str] = None, ctx: CLIContext = EmptyContext) -> ExecutableCommand:
+    def command(
+        self, name: str, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any
+    ) -> ExecutableCommand:
         """
         Create an executable command for given command name, args and context.
         :param name: the name of the command to execute (must be a known command)
         :param arg: the arg of the command (must be parsable by the command)
         :param ctx: the context of this command.
         :return: the ready to run executable command.
         :raises:
             CLIParseError: if the name of the command is not known, or the argument fails to parse.
         """
         if name in self.commands:
             command = self.commands[name]
             try:
-                action = command.parse(arg, ctx, cmd_name=name)
+                action = command.parse(arg, ctx, cmd_name=name, **kwargs)
                 return ExecutableCommand(name, command, arg, action)
             except Exception as ex:
                 raise CLIParseError(f"{name} can not parse arg {arg}. Reason: {ex}") from ex
         else:
             raise CLIParseError(f"Command >{name}< is not known. Typo?")
 
     async def create_query(
@@ -451,29 +457,70 @@
                 query, options, query_parts = await self.create_query(parts, ctx)
                 ctx_wq = evolve(ctx, query=query, query_options=options)
                 # re-evaluate remaining commands - to take the adapted context into account
                 remaining = [self.command(c.name, c.arg, ctx_wq) for c in commands[len(parts) :]]  # noqa: E203
                 return ctx_wq, [*query_parts, *remaining]
             return ctx, commands
 
+        def rewrite_command_line(cmds: List[ExecutableCommand]) -> List[ExecutableCommand]:
+            """
+            Rewrite the command line to make it more user-friendly.
+            Rules:
+            - add the list command if no output format is defined
+            - add a format to write commands if no output format is defined
+            - report benchmark run will be formatted as benchmark result automatically
+            """
+            if context.env.get("no_rewrite") or len(cmds) == 0:
+                return cmds
+            first_cmd = cmds[0]
+            last_cmd = cmds[-1]
+            single = cmds[0] if len(cmds) == 1 else None
+            result = cmds
+
+            def no_format() -> bool:
+                return not any(c for c in result if isinstance(c.command, (OutputTransformer, PreserveOutputFormat)))
+
+            def fmt_benchmark() -> ExecutableCommand:
+                return self.command("format", "--benchmark-result", context)
+
+            def fmt_list() -> ExecutableCommand:
+                return self.command("list", None, context)
+
+            # benchmark run as single command is rewritten to benchmark run | format --benchmark-result
+            if single and isinstance(single.command, ReportCommand) and ReportCommand.is_run_action(single.arg):
+                result = [single, fmt_benchmark()]
+            # if the last command is a write command without any format: add the format
+            elif isinstance(last_cmd.command, WriteCommand) and no_format():
+                # format is either list (default) or benchmark
+                fmt = fmt_benchmark() if isinstance(first_cmd.command, ReportCommand) else fmt_list()
+                result = [*cmds[0:-1], fmt, cmds[-1]]
+
+            # produces text and no resulting output transformer is defined: add the default `list` command
+            if last_cmd.action.produces.text and no_format():
+                result = [*result, fmt_list()]
+            return result
+
         def adjust_context(parsed: ParsedCommands) -> CLIContext:
             cmd_env = {**self.cli_env, **context.env, **parsed.env}
             ctx = evolve(context, env=cmd_env)
             last_command = self.commands.get(parsed.commands[-1].cmd) if parsed.commands else None
             if isinstance(last_command, NoTerminalOutput) and ctx.console_renderer:
                 return evolve(ctx, env=cmd_env, console_renderer=ConsoleRenderer.default_renderer())
             else:
                 return evolve(context, env=cmd_env)
 
         async def parse_line(parsed: ParsedCommands) -> ParsedCommandLine:
             ctx = adjust_context(parsed)
-            ctx, commands = await combine_query_parts([self.command(c.cmd, c.args, ctx) for c in parsed.commands], ctx)
-            not_met = [r for cmd in commands for r in cmd.action.required if r.name not in context.uploaded_files]
-            envelope = {k: v for cmd in commands for k, v in cmd.action.envelope.items()}
-            return ParsedCommandLine(ctx, parsed, commands, not_met, envelope)
+            ctx, commands = await combine_query_parts(
+                [self.command(c.cmd, c.args, ctx, position=i) for i, c in enumerate(parsed.commands)], ctx
+            )
+            rewritten = rewrite_command_line(commands)
+            not_met = [r for cmd in rewritten for r in cmd.action.required if r.name not in context.uploaded_files]
+            envelope = {k: v for cmd in rewritten for k, v in cmd.action.envelope.items()}
+            return ParsedCommandLine(ctx, parsed, rewritten, not_met, envelope)
 
         def expand_aliases(line: ParsedCommands) -> ParsedCommands:
             def expand_alias(alias_cmd: ParsedCommand) -> List[ParsedCommand]:
                 alias: AliasTemplate = self.alias_templates[alias_cmd.cmd]
                 available: Dict[str, AliasTemplateParameter] = {p.name: p for p in alias.parameters}
                 props: Dict[str, JsonElement] = self.replacements(**{**self.cli_env, **context.env})  # type: ignore
                 props["args"] = alias_cmd.args
```

### Comparing `resotocore-3.3.1/resotocore/cli/command.py` & `resotocore-3.3.2/resotocore/cli/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import logging
 import os.path
 import re
 import shutil
 import tarfile
 import tempfile
 from abc import abstractmethod, ABC
+from argparse import Namespace
 from asyncio import Future, Task
 from asyncio.subprocess import Process
 from collections import defaultdict
 from contextlib import suppress
 from datetime import timedelta
 from functools import partial, lru_cache
 from itertools import dropwhile, chain
@@ -42,19 +43,14 @@
 from aiohttp import ClientTimeout, JsonPayload, BasicAuth
 from aiostream import stream, pipe
 from aiostream.aiter_utils import is_async_iterable
 from aiostream.core import Stream
 from attrs import define, field
 from dateutil import parser as date_parser
 from parsy import Parser, string
-from rich.padding import Padding
-from rich.panel import Panel
-from rich.table import Table
-from rich.text import Text
-
 from resotocore import version
 from resotocore.async_extensions import run_async
 from resotocore.cli import (
     JsGen,
     NoExitArgumentParser,
     args_parts_parser,
     args_parts_unquoted_parser,
@@ -86,44 +82,49 @@
 )
 from resotocore.cli.tip_of_the_day import SuggestionPolicy, SuggestionStrategy, get_suggestion_strategy
 from resotocore.config import ConfigEntity
 from resotocore.db.async_arangodb import AsyncCursor
 from resotocore.db.graphdb import HistoryChange
 from resotocore.db.model import QueryModel
 from resotocore.db.runningtaskdb import RunningTaskData
+from resotocore.db.packagedb import InstallationSource, FromGit, FromHttp
+from resotocore.infra_apps.package_manager import Failure
+from resotocore.infra_apps.manifest import AppManifest
 from resotocore.dependencies import system_info
 from resotocore.error import CLIParseError, ClientError, CLIExecutionError
-from resotocore.ids import ConfigId, TaskId
+from resotocore.ids import ConfigId, TaskId, InfraAppName
 from resotocore.ids import TaskDescriptorId
 from resotocore.model.graph_access import Section, EdgeTypes
 from resotocore.model.model import (
     Model,
     Kind,
     ComplexKind,
     DictionaryKind,
     SimpleKind,
     Property,
     ArrayKind,
     PropertyPath,
 )
 from resotocore.model.resolve_in_graph import NodePath
-from resotocore.model.typed_model import to_json, to_js
+from resotocore.model.typed_model import to_json, to_js, from_js
 from resotocore.query.model import (
     Query,
     P,
     Template,
     NavigateUntilRoot,
     Term,
     AggregateFunction,
     AggregateVariableName,
     AggregateVariableCombined,
     Aggregate,
 )
 from resotocore.query.query_parser import parse_query, aggregate_parameter_parser
 from resotocore.query.template_expander import tpl_props_p
+from resotocore.report import BenchmarkConfigPrefix, ReportSeverity
+from resotocore.report.benchmark_renderer import respond_benchmark_result
 from resotocore.task.task_description import Job, TimeTrigger, EventTrigger, ExecuteCommand, Workflow, RunningTask
 from resotocore.types import Json, JsonElement, EdgeType
 from resotocore.util import (
     uuid_str,
     utc,
     if_set,
     duration,
@@ -152,14 +153,18 @@
     comma_p,
     variable_p,
     equals_p,
     json_value_p,
 )
 from resotolib.utils import safe_members_in_tarfile, get_local_tzinfo
 from resotolib.x509 import write_cert_to_file, write_key_to_file
+from rich.padding import Padding
+from rich.panel import Panel
+from rich.table import Table
+from rich.text import Text
 
 log = logging.getLogger(__name__)
 
 
 # A SearchCLIPart is a command that can be used on the command line.
 # Such a part is not executed, but builds a search, which is executed.
 # Therefore, the parse method is implemented in a dummy fashion here.
@@ -1364,15 +1369,15 @@
             result.append(f"--{key}")
             if value is not True:
                 result.append(f"'{value}'")  # put the value into single quotes to maintain the spaces
         return " ".join(result) + " " if result else ""
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLISource:
         # db name is coming from the env
-        graph_name = ctx.env["graph"]
+        graph_name = ctx.graph_name
         if not arg:
             raise CLIParseError("search command needs a search-statement to execute, but nothing was given!")
 
         # Read all argument flags / options
         parsed, rest = self.parse_known(arg)
         with_edges: bool = parsed.get("with-edges", False)
         explain: bool = parsed.get("explain", False)
@@ -1888,15 +1893,15 @@
     @abstractmethod
     def patch(self, arg: Optional[str], ctx: CLIContext) -> Json:
         # deriving classes need to define how to patch
         pass
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIFlow:
         buffer_size = 1000
-        func = partial(self.set_desired, arg, ctx.env["graph"], self.patch(arg, ctx))
+        func = partial(self.set_desired, arg, ctx.graph_name, self.patch(arg, ctx))
         return CLIFlow(lambda in_stream: stream.flatmap(stream.chunks(in_stream, buffer_size), func))
 
     async def set_desired(
         self, arg: Optional[str], graph_name: str, patch: Json, items: List[Json]
     ) -> AsyncIterator[JsonElement]:
         model = await self.dependencies.model_handler.load_model()
         db = self.dependencies.db_access.get_graph_db(graph_name)
@@ -2024,15 +2029,15 @@
     @abstractmethod
     def patch(self, arg: Optional[str], ctx: CLIContext) -> Json:
         # deriving classes need to define how to patch
         pass
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIFlow:
         buffer_size = 1000
-        func = partial(self.set_metadata, ctx.env["graph"], self.patch(arg, ctx))
+        func = partial(self.set_metadata, ctx.graph_name, self.patch(arg, ctx))
         return CLIFlow(lambda in_stream: stream.flatmap(stream.chunks(in_stream, buffer_size), func))
 
     async def set_metadata(self, graph_name: str, patch: Json, items: List[Json]) -> AsyncIterator[JsonElement]:
         model = await self.dependencies.model_handler.load_model()
         db = self.dependencies.db_access.get_graph_db(graph_name)
         node_ids = []
         for item in items:
@@ -2131,14 +2136,17 @@
     def args_info(self) -> ArgsInfo:
         return []
 
     def patch(self, arg: Optional[str], ctx: CLIContext) -> Json:
         return {"protected": True}
 
 
+ConvertFn = Callable[[AsyncIterator[JsonElement]], AsyncIterator[JsonElement]]
+
+
 class FormatCommand(CLICommand, OutputTransformer):
     """
     ```
     format [--json][--ndjson][--text][--cytoscape][--graphml][--dot] [format string]
     ```
 
     This command creates a string from the json input based on the format string.
@@ -2195,54 +2203,66 @@
             ArgInfo("--cytoscape", help_text="output format", option_group="output"),
             ArgInfo("--graphml", help_text="output format", option_group="output"),
             ArgInfo("--dot", help_text="output format", option_group="output"),
             ArgInfo("--yaml", help_text="output format", option_group="output"),
             ArgInfo(expects_value=True, help_text="format definition with {} placeholders", option_group="output"),
         ]
 
-    formats: Dict[str, Callable[[AsyncIterator[JsonElement]], AsyncIterator[JsonElement]]] = {
+    formats: Dict[str, ConvertFn] = {
         "ndjson": respond_ndjson,
         "json": partial(respond_json, indent=2),
         "text": respond_text,
         "yaml": respond_yaml,
         "cytoscape": respond_cytoscape,
         "graphml": respond_graphml,
         "dot": respond_dot,
     }
 
+    render_all = {"benchmark_result": respond_benchmark_result}
+
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIFlow:
         parser = NoExitArgumentParser()
         parser.add_argument("--json", dest="json", action="store_true")
         parser.add_argument("--ndjson", dest="ndjson", action="store_true")
         parser.add_argument("--graphml", dest="graphml", action="store_true")
         parser.add_argument("--text", dest="text", action="store_true")
         parser.add_argument("--yaml", dest="yaml", action="store_true")
         parser.add_argument("--cytoscape", dest="cytoscape", action="store_true")
         parser.add_argument("--dot", dest="dot", action="store_true")
+        parser.add_argument("--benchmark-result", dest="benchmark_result", action="store_true")
         parsed, formatting_string = parser.parse_known_args(arg.split() if arg else [])
         format_to_use = {k for k, v in vars(parsed).items() if v is True}
+        use: Optional[str] = None
+        if format_to_use:
+            if len(format_to_use) > 1:
+                raise AttributeError(f'You can define only one format. Defined: {", ".join(format_to_use)}')
+            if len(formatting_string) > 0:
+                raise AttributeError("A format renderer can not be combined together with a format string!")
+            use = next(iter(format_to_use))
 
-        async def render_format(format_name: str, iss: Stream) -> JsGen:
+        async def render_single(converter: ConvertFn, iss: Stream) -> JsGen:
             async with iss.stream() as streamer:
-                async for elem in self.formats[format_name](streamer):
+                async for elem in converter(streamer):
                     yield elem
 
-        async def format_stream(in_stream: Stream) -> Stream:
-            if format_to_use:
-                if len(format_to_use) > 1:
-                    raise AttributeError(f'You can define only one format. Defined: {", ".join(format_to_use)}')
-                if len(formatting_string) > 0:
-                    raise AttributeError("A format renderer can not be combined together with a format string!")
-                return render_format(next(iter(format_to_use)), in_stream)
+        async def format_stream(in_stream: Stream) -> JsGen:
+            if use:
+                if all_renderer := self.render_all.get(use):
+                    return all_renderer(in_stream)
+                elif single_renderer := self.formats.get(use):
+                    return render_single(single_renderer, in_stream)
+                else:
+                    raise ValueError(f"Unknown format: {use}")
             elif formatting_string:
                 return stream.map(in_stream, ctx.formatter(arg)) if arg else in_stream
             else:
                 return in_stream
 
-        return CLIFlow(format_stream)
+        produces = MediaType.Markdown if use == "benchmark_result" else MediaType.String
+        return CLIFlow(format_stream, produces=produces)
 
 
 @make_parser
 def list_single_arg_parse() -> Parser:
     name = yield variable_dp
     as_name = yield (space_dp >> string("as") >> space_dp >> literal_dp).optional()
     return name, as_name
@@ -2641,15 +2661,15 @@
             if parsed.csv:
                 return csv_stream(in_stream)
             elif parsed.markdown:
                 return markdown_stream(in_stream)
             else:
                 return stream.map(in_stream, lambda elem: fmt_json(elem) if isinstance(elem, dict) else str(elem))
 
-        return CLIFlow(fmt)
+        return CLIFlow(fmt, produces=MediaType.String)
 
 
 class JobsCommand(CLICommand, PreserveOutputFormat):
     """
     ```shell
     jobs list
     jobs show <id>
@@ -4604,14 +4624,454 @@
                 2,
                 produces=MediaType.FilePath,
             )
         else:
             return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
 
 
+class ReportCommand(CLICommand):
+    """
+    ```shell
+    report benchmarks list
+    report benchmark show <benchmark-id>
+    report benchmark run <benchmark-id> [--accounts <account-id>] [--severity <level>] [--only-failing]
+    report checks list
+    report checks show <check-id>
+    report checks run <check-id> [--accounts <account-id>] [--severity <level>] [--only-failing]
+    ```
+
+    List and run benchmarks as well as specific benchmark checks.
+    Benchmarks are a collection of checks that are run against all or specific accounts.
+    Every check has a severity, that can also be used to filter relevant checks.
+
+    The result of a benchmark run is a report in Markdown format.
+    By default, this report is rendered and displayed in the console.
+    It is also possible to write the result to a file and open it in an external viewer.
+
+    ## Parameters
+    - `--accounts` [optional]: List of account ids (space separated) to run the benchmark against.
+        If not specified, the benchmark is run against all accounts.
+    - `--severity` [optional]: Severity level to filter checks. One of `info`, `low`, `medium`, `high`, `critical`
+
+    ## Options
+    - `--only-failing` [optional]: Only include checks that are failing in the report.
+
+    ## Examples
+
+    ```shell
+    # List all available chekcs
+    > report checks list
+    aws_apigateway_authorizers_enabled
+    aws_s3_account_level_public_access_blocks
+
+    # Display the details of a specific check
+    > report check show aws_apigateway_authorizers_enabled
+      ... output suppressed ...
+
+    # Perform the check against all accounts available, showing only a result if the check fails.
+    > report check run aws_apigateway_authorizers_enabled --only-failing
+      ... output suppressed ...
+
+    # Perform the check against all defined accounts, showing only a result if the check fails.
+    > report check run aws_apigateway_authorizers_enabled  --accounts 111 222 --only-failing
+      ... output suppressed ...
+
+    # List all available benchmarks
+    > report benchmarks list
+    aws_cis_1_5
+
+    # Display the details of a specific benchmark
+    > report benchmark show aws_cis_1_5
+    report_benchmark:
+      ... output suppressed ...
+
+    # Run benchmark against all accounts available
+    > report benchmark run aws_cis_1_5
+      ... output suppressed ...
+
+    # Run benchmark against account 111 and 222, check only critical checks
+    # The resulting report should contain only failed checks.
+    > report benchmark run aws_cis_1_5 --accounts 111 222  --severity critical --only-failing
+      ... output suppressed ...
+    ```
+    """
+
+    @property
+    def name(self) -> str:
+        return "report"
+
+    def args_info(self) -> ArgsInfo:
+        run_args = [
+            ArgInfo("--accounts", True, help_text="Space delimited list of accounts"),
+            ArgInfo(
+                "--severity",
+                True,
+                help_text="The severity level to filter checks",
+                possible_values=[s.value for s in ReportSeverity],
+            ),
+            ArgInfo("--only-failing", False, help_text="Filter only failing checks."),
+        ]
+        return {
+            "benchmark": {
+                "list": [],
+                "run": [ArgInfo(None, help_text="<benchmark-id>"), *run_args],
+                "show": [ArgInfo(None, help_text="<benchmark-id>")],
+            },
+            "checks": {
+                "list": [],
+                "run": [ArgInfo(None, help_text="<check-id>"), *run_args],
+                "show": [ArgInfo(None, help_text="<check-id>")],
+            },
+        }
+
+    def info(self) -> str:
+        return "Generate reports."
+
+    @staticmethod
+    def is_run_action(arg: Optional[str]) -> bool:
+        return ReportCommand.action_from_arg(arg) in ("benchmark_run", "check_run")
+
+    @staticmethod
+    def action_from_arg(arg: Optional[str]) -> Optional[str]:
+        args = re.split("\\s+", arg.strip(), maxsplit=3) if arg else []
+        if len(args) == 2 and args[0] in ("benchmark", "benchmarks") and args[1] == "list":
+            return "benchmark_list"
+        elif len(args) == 3 and args[0] in ("benchmark", "benchmarks") and args[1] == "show":
+            return "benchmark_show"
+        elif len(args) >= 3 and args[0] in ("benchmark", "benchmarks") and args[1] == "run":
+            return "benchmark_run"
+        elif len(args) == 2 and args[0] in ("check", "checks") and args[1] == "list":
+            return "check_list"
+        elif len(args) == 3 and args[0] in ("check", "checks") and args[1] == "show":
+            return "check_show"
+        elif len(args) >= 3 and args[0] in ("check", "checks") and args[1] == "run":
+            return "check_run"
+        else:
+            return None
+
+    def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
+        async def list_benchmarks() -> AsyncIterator[str]:
+            for benchmark in await self.dependencies.inspector.list_benchmarks():
+                yield benchmark.id
+
+        async def show_benchmark(bid: str) -> AsyncIterator[Optional[str]]:
+            yield await self.dependencies.config_handler.config_yaml(ConfigId(BenchmarkConfigPrefix + bid))
+
+        async def show_check(cid: str) -> AsyncIterator[Json]:
+            model = await self.dependencies.config_handler.get_configs_model()
+            kind = model.get("resoto_core_report_check")
+            for check in await self.dependencies.inspector.list_checks(check_ids=[cid]):
+                yield kind.create_yaml(to_js(check)) if isinstance(kind, ComplexKind) else yaml.safe_dump(to_js(check))
+
+        async def list_checks() -> AsyncIterator[str]:
+            for check in await self.dependencies.inspector.list_checks():
+                yield check.id
+
+        async def run_benchmark(parsed_args: Namespace) -> AsyncIterator[Json]:
+            result = await self.dependencies.inspector.perform_benchmark(
+                ctx.graph_name,
+                parsed_args.identifier,
+                accounts=parsed_args.accounts,
+                severity=parsed_args.severity,
+                only_failing=parsed_args.only_failing,
+            )
+            if not result.is_empty():
+                for node in result.to_graph():
+                    yield node
+
+        async def run_check(parsed_args: Namespace) -> AsyncIterator[Json]:
+            result = await self.dependencies.inspector.perform_checks(
+                ctx.graph_name,
+                check_ids=[parsed_args.identifier],
+                accounts=parsed_args.accounts,
+                severity=parsed_args.severity,
+                only_failing=parsed_args.only_failing,
+            )
+            if not parsed_args.only_failing or result.has_failed():
+                for node in result.to_graph():
+                    yield node
+
+        async def show_help() -> AsyncIterator[str]:
+            yield f"Do not understand: {arg}\n\n" + self.rendered_help(ctx)
+
+        run_parser = NoExitArgumentParser()
+        run_parser.add_argument("identifier")
+        run_parser.add_argument("--accounts", nargs="+")
+        run_parser.add_argument("--severity", type=ReportSeverity, choices=list(ReportSeverity))
+        run_parser.add_argument("--only-failing", action="store_true", default=False)
+
+        action = self.action_from_arg(arg)
+        args = re.split("\\s+", arg.strip(), maxsplit=2) if arg else []
+        if action == "benchmark_list":
+            return CLISource.no_count(list_benchmarks)
+        elif action == "benchmark_show":
+            return CLISource.no_count(partial(show_benchmark, args[2].strip()))
+        elif action == "benchmark_run":
+            parsed = run_parser.parse_args(args[2].split() if len(args) > 2 else [])
+            return CLISource.no_count(partial(run_benchmark, parsed))
+        elif action == "check_list":
+            return CLISource.no_count(list_checks)
+        elif action == "check_show":
+            return CLISource.no_count(partial(show_check, args[2].strip()))
+        elif action == "check_run":
+            parsed = run_parser.parse_args(args[2].split() if len(args) > 2 else [])
+            return CLISource.no_count(partial(run_check, parsed))
+        else:
+            return CLISource.single(show_help)
+
+
+class InfrastructureAppsCommand(CLICommand):
+    """
+    ```shell
+    apps search [pattern] [--repo someengineering/resoto-apps]
+    app info <app_name> [--repo someengineering/resoto-apps]
+    app install <app_name> [--repo someengineering/resoto-apps]
+    app edit <app_name>
+    app uninstall <app_name>
+    app update <app_name>|all
+    apps list
+    app run <app_name> [--dry-run] --config [config_name]
+    ```
+
+    - `apps search [pattern]`: Lists all apps available in https://github.com/someengineering/resoto-apps/
+    (or other repo if specified). Supports filtering by pattern.
+    - `app info <app_name>`: Show information about an app.
+    - `app install <app_name>`: Install an app.
+    - `app edit <app_name>`: Edit an app.
+    - `app uninstall <app_name>`: Uninstall an app.
+    - `app update <app_name>|all`: Update an app or all apps.
+    - `apps list`: List all installed apps.
+    - `app run <app_name> [--dry-run] [--config <config_name>]`: Run an app.
+
+
+    ## Parameters
+    - `app_name` [required]: The identifier of the infrastructure app.
+    - `pattern` [optional]: Pattern for searching for apps. Supports glob wildcards such as * and ?.
+
+    ## Options
+    - `--repo <repo>`: The repo to use for searching for apps. Defaults to someengineering/resoto-apps.
+    - `--dry-run`: Run the app but do not make any changes.
+    - `--config <config_name>`: The configuration to use to run the app. Defaults to the default configuration.
+    """
+
+    @property
+    def name(self) -> str:
+        return "apps"
+
+    def info(self) -> str:
+        return "Manage infrastructure apps."
+
+    def args_info(self) -> ArgsInfo:
+        return {
+            "search": [ArgInfo(None, True, help_text="<pattern>")],
+            "info": [ArgInfo(None, True, help_text="<app_name>")],
+            "install": [
+                ArgInfo(None, True, help_text="<app_name>"),
+                ArgInfo("--repo", True, help_text="<repo>", option_group="source"),
+                ArgInfo("--url", True, help_text="<url>", option_group="source"),
+            ],
+            "edit": [ArgInfo(None, True, help_text="<app_name>")],
+            "uninstall": [ArgInfo(None, True, help_text="<app_name>")],
+            "update": [ArgInfo(None, True, help_text="<app_name>")],
+            "list": [ArgInfo(None, False)],
+            "run": [
+                ArgInfo(None, True, help_text="<app_name>"),
+                ArgInfo("--dry-run", False),
+                ArgInfo("--validate", False),
+                ArgInfo("--config", True, help_text="<config_name>"),
+            ],
+        }
+
+    def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
+        async def apps_search(pattern: Optional[str]) -> AsyncIterator[JsonElement]:
+            yield f"App search not yet implemented. Pattern: {pattern}"
+
+        async def app_info(app_name: InfraAppName) -> AsyncIterator[JsonElement]:
+            yield await self.dependencies.infra_apps_package_manager.info(app_name)
+
+        async def app_install(app_name: InfraAppName, source: InstallationSource) -> AsyncIterator[JsonElement]:
+            manifest = await self.dependencies.infra_apps_package_manager.install(app_name, source)
+            yield f"App {app_name} version {manifest.version} installed successfully"
+
+        async def send_file(content: str) -> AsyncIterator[str]:
+            temp_dir: str = tempfile.mkdtemp()
+            path = os.path.join(temp_dir, "manifest.yaml")
+            try:
+                async with aiofiles.open(path, "w") as f:
+                    await f.write(content)
+                yield path
+            finally:
+                shutil.rmtree(temp_dir)
+
+        async def edit_app(app_name: InfraAppName) -> AsyncIterator[str]:
+            # Editing a config is a two-step process:
+            # 1) download the config and make it available to edit
+            # 2) upload the config file and update the config from content --> update_config
+            manifest = await self.dependencies.infra_apps_package_manager.get_manifest(app_name)
+            if not manifest:
+                raise AttributeError(f"No app with this name: {app_name}")
+            yml = yaml.safe_dump(to_js(manifest))
+            return send_file(yml)
+
+        async def update_app(app_name: InfraAppName) -> AsyncIterator[str]:
+            # Usually invoked by resh automatically via edit_app, but can also be triggered manually.
+            # An app with given name is changed by the content of uploaded file "app_name.yaml"
+            content = ""
+            try:
+                async with aiofiles.open(ctx.uploaded_files["manifest.yaml"], "r") as f:
+                    content = await f.read()
+                    manifest: AppManifest = from_js(yaml.safe_load(content), AppManifest)
+                await self.dependencies.infra_apps_package_manager.update_from_manifest(manifest)
+            except Exception as ex:
+                log.debug(f"Could not update the app manifest: {ex}.", exc_info=ex)
+                # Yaml file: add the error as comment on top
+                error = "\n".join(f"## {line}" for line in str(ex).splitlines())
+                message = f"## Update the app failed. Please correct.\n{error}\n\n"
+                # Remove error message from previous check
+                config = "\n".join(dropwhile(lambda m: m.startswith("##") or len(m.strip()) == 0, content.splitlines()))
+                async for file in send_file(message + config):
+                    yield file
+
+        async def app_uninstall(app_name: InfraAppName) -> AsyncIterator[JsonElement]:
+            await self.dependencies.infra_apps_package_manager.delete(app_name)
+            yield f"App {app_name} uninstalled"
+
+        async def app_update(app_name: InfraAppName) -> AsyncIterator[JsonElement]:
+            updated_manifest = await self.dependencies.infra_apps_package_manager.update(app_name)
+            yield f"App {app_name} updated sucessfully to the latest version ({updated_manifest.version})"
+
+        async def app_update_all() -> AsyncIterator[JsonElement]:
+            async for name, result in self.dependencies.infra_apps_package_manager.update_all():
+                if isinstance(result, Failure):
+                    yield f"App {name} failed to update: {result}"
+                else:
+                    yield f"App {name} updated sucessfully to the latest version ({result.version})"
+
+        async def apps_list() -> AsyncIterator[JsonElement]:
+            async for app in self.dependencies.infra_apps_package_manager.list():
+                yield app
+
+        async def app_run(
+            in_stream: JsGen, app_name: InfraAppName, dry_run: bool, config: Optional[str]
+        ) -> AsyncIterator[JsonElement]:
+            runtime = self.dependencies.infra_apps_runtime
+            manifest = await self.dependencies.infra_apps_package_manager.get_manifest(app_name)
+            if not manifest:
+                raise ValueError(f"App {app_name} is not installed.")
+            app_config = None
+            if config:
+                ce = await self.dependencies.config_handler.get_config(ConfigId(config))
+                if ce:
+                    app_config = ce.config
+                else:
+                    raise ValueError(f"Config {config} not found.")
+            else:
+                app_config = manifest.default_config or {}
+
+            stdin: AsyncIterator[JsonElement] = (
+                stream.iterate(in_stream) if isinstance(in_stream, Stream) else in_stream
+            )
+
+            if dry_run:
+                return runtime.generate_template(
+                    graph=ctx.graph_name,
+                    manifest=manifest,
+                    config=app_config,
+                    stdin=stdin,
+                    kwargs=Namespace(),
+                )
+            else:
+                return runtime.execute(
+                    graph=ctx.graph_name, manifest=manifest, config=app_config, stdin=stdin, kwargs=Namespace(), ctx=ctx
+                )
+
+        args = re.split("\\s+", arg, maxsplit=2) if arg else []
+        if len(args) == 1 and args[0] == "search":
+            return CLISource.single(partial(apps_search, None))
+        elif len(args) == 2 and args[0] == "search":
+            return CLISource.single(partial(apps_search, args[1]))
+        elif len(args) == 2 and args[0] == "info":
+            return CLISource.single(partial(app_info, InfraAppName(args[1])))
+        elif len(args) >= 2 and args[0] == "install":
+            parser = NoExitArgumentParser()
+            source_group = parser.add_mutually_exclusive_group()
+            source_group.add_argument("--repo", dest="repo", type=str)
+            source_group.add_argument("--url", dest="url", type=str)
+            parser.add_argument("command", type=str)
+            parser.add_argument("app_name", type=str)
+            parsed = parser.parse_args(strip_quotes(arg or "").split())
+
+            source: Optional[InstallationSource] = None
+            if parsed.repo:
+                source = FromGit(parsed.repo)
+            elif parsed.url:
+                source = FromHttp(parsed.url)
+            else:
+                source = FromGit("https://github.com/someengineering/resoto-apps.git")
+
+            return CLISource.single(
+                partial(
+                    app_install,
+                    InfraAppName(parsed.app_name),
+                    source,
+                )
+            )
+        elif arg and len(args) == 2 and args[0] == "edit":
+            app_name = InfraAppName(args[1])
+            return CLISource.single(
+                partial(edit_app, app_name),
+                produces=MediaType.FilePath,
+                envelope={"Resoto-Shell-Action": "edit", "Resoto-Shell-Command": f"apps update {app_name}"},
+            )
+        elif arg and len(args) == 3 and args[0] == "update":
+            app_name = InfraAppName(args[1])
+            return CLISource.single(
+                partial(update_app, app_name),
+                produces=MediaType.FilePath,
+                envelope={"Resoto-Shell-Action": "edit", "Resoto-Shell-Command": f"apps update {app_name}"},
+                requires=[CLIFileRequirement("manifest.yaml", args[2])],
+            )
+        elif len(args) == 2 and args[0] == "uninstall":
+            return CLISource.single(partial(app_uninstall, InfraAppName(args[1])))
+        elif len(args) == 2 and args[0] == "update" and args[1] == "all":
+            return CLISource.single(app_update_all)
+        elif len(args) == 2 and args[0] == "update":
+            return CLISource.single(partial(app_update, InfraAppName(args[1])))
+        elif len(args) == 1 and args[0] == "list":
+            return CLISource.single(apps_list)
+        elif len(args) >= 2 and args[0] == "run":
+            parser = NoExitArgumentParser()
+            parser.add_argument("command", type=str)
+            parser.add_argument("app_name", type=str)
+            parser.add_argument("--dry-run", dest="dry_run", action="store_true", default=False)
+            parser.add_argument("--config", dest="config", type=str, default=None)
+            parsed = parser.parse_args(strip_quotes(arg or "").split())
+
+            in_source_position = kwargs.get("position") == 0
+
+            if in_source_position:
+                return CLISource.no_count(
+                    partial(
+                        app_run,
+                        in_stream=stream.empty(),
+                        app_name=InfraAppName(parsed.app_name),
+                        dry_run=parsed.dry_run,
+                        config=parsed.config,
+                    )
+                )
+            else:
+                return CLIFlow(
+                    partial(
+                        app_run, app_name=InfraAppName(parsed.app_name), dry_run=parsed.dry_run, config=parsed.config
+                    )
+                )
+        else:
+            return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
+
+
 def all_commands(d: CLIDependencies) -> List[CLICommand]:
     commands = [
         AggregateCommand(d, "search"),
         AggregateToCountCommand(d, "search"),
         AncestorsPart(d, "search"),
         CertificateCommand(d, "setup", allowed_in_source_position=True),
         ChunkCommand(d, "misc"),
@@ -4634,32 +5094,39 @@
         JsonCommand(d, "misc", allowed_in_source_position=True),
         KindsCommand(d, "search", allowed_in_source_position=True),
         LimitPart(d, "search"),
         ListCommand(d, "format"),
         TemplatesCommand(d, "search", allowed_in_source_position=True),
         PredecessorsPart(d, "search"),
         ProtectCommand(d, "action"),
+        ReportCommand(d, "misc", allowed_in_source_position=True),
         SearchPart(d, "search", allowed_in_source_position=True),
         SetDesiredCommand(d, "action"),
         SetMetadataCommand(d, "action"),
         SleepCommand(d, "misc", allowed_in_source_position=True),
         SortPart(d, "search"),
         SuccessorsPart(d, "search"),
         SystemCommand(d, "setup", allowed_in_source_position=True),
         TagCommand(d, "action"),
         TailCommand(d, "misc"),
         UniqCommand(d, "misc"),
         WorkflowsCommand(d, "action", allowed_in_source_position=True),
         WelcomeCommand(d, "misc", allowed_in_source_position=True),
         TipOfTheDayCommand(d, "misc", allowed_in_source_position=True),
         WriteCommand(d, "misc"),
+        InfrastructureAppsCommand(d, "apps", allowed_in_source_position=True),
     ]
     # commands that are only available when the system is started in debug mode
     if d.config.runtime.debug:
-        commands.extend([FileCommand(d, "misc"), UploadCommand(d, "misc")])
+        commands.extend(
+            [
+                FileCommand(d, "misc"),
+                UploadCommand(d, "misc"),
+            ]
+        )
 
     return commands
 
 
 def alias_names() -> Dict[str, str]:
     # command alias -> command name
     return {
@@ -4673,9 +5140,10 @@
         "successor": "successors",
         "descendant": "descendants",
         "ancestor": "ancestors",
         "job": "jobs",
         "lists": "list",
         "template": "templates",
         "workflow": "workflows",
+        "app": "apps",
         "man": "help",
     }
```

### Comparing `resotocore-3.3.1/resotocore/cli/model.py` & `resotocore-3.3.2/resotocore/cli/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from abc import ABC, abstractmethod
 from asyncio import Queue, Task, iscoroutine
 from datetime import timedelta
 from enum import Enum
 from functools import reduce
 from operator import attrgetter
 from textwrap import dedent
-from typing import Optional, List, Any, Dict, Tuple, Callable, Union, Awaitable, Type, cast, Set
+from typing import Optional, List, Any, Dict, Tuple, Callable, Union, Awaitable, Type, cast, Set, AsyncIterator
 
 from aiohttp import ClientSession, TCPConnector
 from aiostream import stream
 from aiostream.core import Stream
 from attrs import define, field
 from parsy import test_char, string
 from rich.jupyter import JupyterMixin
@@ -26,30 +26,35 @@
 from resotocore.core_config import CoreConfig, AliasTemplateConfig, AliasTemplateParameterConfig
 from resotocore.db.db_access import DbAccess
 from resotocore.error import CLIParseError
 from resotocore.message_bus import MessageBus
 from resotocore.model.model_handler import ModelHandler
 from resotocore.query.model import Query, variable_to_absolute, PathRoot
 from resotocore.query.template_expander import TemplateExpander, render_template
+from resotocore.report import Inspector
 from resotocore.task import TaskHandler
 from resotocore.types import Json, JsonElement
 from resotocore.util import AccessJson, uuid_str, from_utc, utc, utc_str
 from resotocore.web.certificate_handler import CertificateHandler
 from resotocore.worker_task_queue import WorkerTaskQueue
+from resotocore.infra_apps.runtime import Runtime
+from resotocore.infra_apps.package_manager import PackageManager
 from resotolib.parse_util import l_curly_dp, r_curly_dp
 from resotolib.utils import get_local_tzinfo
 
 
 class MediaType(Enum):
     Json = 1
     FilePath = 2
+    Markdown = 3
+    String = 4
 
     @property
-    def json(self) -> bool:
-        return self == MediaType.Json
+    def text(self) -> bool:
+        return self in (MediaType.Json, MediaType.String, MediaType.Markdown)
 
     @property
     def file_path(self) -> bool:
         return self == MediaType.FilePath
 
     def __repr__(self) -> str:
         return "application/json" if self == MediaType.Json else "application/octet-stream"
@@ -70,27 +75,43 @@
     env: Dict[str, str] = field(factory=dict)
     uploaded_files: Dict[str, str] = field(factory=dict)  # id -> path
     query: Optional[Query] = None
     query_options: Dict[str, Any] = field(factory=dict)
     console_renderer: Optional[ConsoleRenderer] = None
     source: Optional[str] = None  # who is calling
 
+    @property
+    def graph_name(self) -> str:
+        return self.env["graph"]
+
     def variable_in_section(self, variable: str) -> str:
         # if there is no query, always assume the root section
         section = self.env.get("section") if self.query else PathRoot
         return variable_to_absolute(section, variable)
 
     def render_console(self, element: Union[str, JupyterMixin]) -> str:
         if self.console_renderer:
             return self.console_renderer.render(element)
         elif isinstance(element, JupyterMixin):
             return str(element)
         else:
             return element
 
+    def text_generator(
+        self, line: ParsedCommandLine, in_stream: AsyncIterator[JsonElement]
+    ) -> AsyncIterator[JsonElement]:
+        async def render_markdown() -> AsyncIterator[str]:
+            async for e in in_stream:
+                yield self.render_console(e)  # type: ignore
+
+        if line.produces == MediaType.Markdown:
+            return render_markdown()
+        else:
+            return in_stream
+
     def supports_color(self) -> bool:
         return (
             self.console_renderer is not None
             and self.console_renderer.color_system is not None
             and self.console_renderer.color_system != ConsoleColorSystem.monochrome
         )
 
@@ -194,14 +215,26 @@
         return self.lookup["config_handler"]  # type:ignore
 
     @property
     def cert_handler(self) -> CertificateHandler:
         return self.lookup["cert_handler"]  # type:ignore
 
     @property
+    def inspector(self) -> Inspector:
+        return self.lookup["inspector"]  # type:ignore
+
+    @property
+    def infra_apps_runtime(self) -> Runtime:
+        return self.lookup["infra_apps_runtime"]  # type:ignore
+
+    @property
+    def infra_apps_package_manager(self) -> PackageManager:
+        return self.lookup["infra_apps_package_manager"]  # type:ignore
+
+    @property
     def http_session(self) -> ClientSession:
         session: Optional[ClientSession] = self.lookup.get("http_session")
         if not session:
             connector = TCPConnector(limit=0, ssl=False, ttl_dns_cache=300)
             session = ClientSession(connector=connector)
             self.lookup["http_session"] = session
         return session
@@ -247,14 +280,23 @@
 
     async def source(self) -> Tuple[Optional[int], Stream]:
         res = self._fn()
         count, gen = await res if iscoroutine(res) else res
         return count, self.make_stream(await gen if iscoroutine(gen) else gen)
 
     @staticmethod
+    def no_count(
+        fn: Callable[[], Union[JsGen, Awaitable[JsGen]]],
+        produces: MediaType = MediaType.Json,
+        requires: Optional[List[CLICommandRequirement]] = None,
+        envelope: Optional[Dict[str, str]] = None,
+    ) -> CLISource:
+        return CLISource.with_count(fn, None, produces, requires, envelope)
+
+    @staticmethod
     def with_count(
         fn: Callable[[], Union[JsGen, Awaitable[JsGen]]],
         count: Optional[int],
         produces: MediaType = MediaType.Json,
         requires: Optional[List[CLICommandRequirement]] = None,
         envelope: Optional[Dict[str, str]] = None,
     ) -> CLISource:
```

### Comparing `resotocore-3.3.1/resotocore/cli/tip_of_the_day.py` & `resotocore-3.3.2/resotocore/cli/tip_of_the_day.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/config/__init__.py` & `resotocore-3.3.2/resotocore/config/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/config/config_handler_service.py` & `resotocore-3.3.2/resotocore/config/config_handler_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/config/config_override_service.py` & `resotocore-3.3.2/resotocore/config/config_override_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/config/core_config_handler.py` & `resotocore-3.3.2/resotocore/config/core_config_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/console_renderer.py` & `resotocore-3.3.2/resotocore/console_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/constants.py` & `resotocore-3.3.2/resotocore/constants.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/core_config.py` & `resotocore-3.3.2/resotocore/core_config.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/db/__init__.py` & `resotocore-3.3.2/resotocore/db/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/db/arango_query.py` & `resotocore-3.3.2/resotocore/db/arango_query.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/db/arangodb_extensions.py` & `resotocore-3.3.2/resotocore/db/arangodb_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/db/arangodb_functions.py` & `resotocore-3.3.2/resotocore/db/arangodb_functions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/db/async_arangodb.py` & `resotocore-3.3.2/resotocore/db/async_arangodb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/db/configdb.py` & `resotocore-3.3.2/resotocore/db/configdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/db/db_access.py` & `resotocore-3.3.2/resotocore/db/db_access.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from resotocore.db.graphdb import ArangoGraphDB, GraphDB, EventGraphDB
 from resotocore.db.jobdb import job_db
 from resotocore.db.modeldb import ModelDb, model_db
 from resotocore.db.deferred_edge_db import pending_deferred_edge_db
 from resotocore.db.runningtaskdb import running_task_db
 from resotocore.db.subscriberdb import subscriber_db
 from resotocore.db.templatedb import template_entity_db
+from resotocore.db.packagedb import app_package_entity_db
 from resotocore.error import NoSuchGraph, RequiredDependencyMissingError
 from resotocore.model.adjust_node import AdjustNode
 from resotocore.model.typed_model import from_js, to_js
 from resotocore.types import Json
 from resotocore.util import Periodic, utc, shutdown_process, uuid_str
 
 log = logging.getLogger(__name__)
@@ -47,42 +48,45 @@
         running_task_name: str = "running_tasks",
         job_name: str = "jobs",
         deferred_edge_name: str = "deferred_outer_edges",
         config_entity: str = "configs",
         config_validation_entity: str = "config_validation",
         configs_model: str = "configs_model",
         template_entity: str = "templates",
+        infra_app_packages: str = "infra_app_packages",
     ):
         self.event_sender = event_sender
         self.database = arango_database
         self.db = AsyncArangoDB(arango_database)
         self.adjust_node = adjust_node
         self.model_db = EventEntityDb(model_db(self.db, model_name), event_sender, model_name)
         self.subscribers_db = EventEntityDb(subscriber_db(self.db, subscriber_name), event_sender, subscriber_name)
         self.running_task_db = running_task_db(self.db, running_task_name)
         self.pending_deferred_edge_db = pending_deferred_edge_db(self.db, deferred_edge_name)
         self.job_db = job_db(self.db, job_name)
         self.config_entity_db = config_entity_db(self.db, config_entity)
         self.config_validation_entity_db = config_validation_entity_db(self.db, config_validation_entity)
         self.configs_model_db = model_db(self.db, configs_model)
         self.template_entity_db = template_entity_db(self.db, template_entity)
+        self.package_entity_db = app_package_entity_db(self.db, infra_app_packages)
         self.graph_dbs: Dict[str, GraphDB] = {}
         self.config = config
         self.cleaner = Periodic("outdated_updates_cleaner", self.check_outdated_updates, timedelta(seconds=60))
 
     async def start(self) -> None:
         await self.model_db.create_update_schema()
         await self.subscribers_db.create_update_schema()
         await self.running_task_db.create_update_schema()
         await self.job_db.create_update_schema()
         await self.config_entity_db.create_update_schema()
         await self.config_validation_entity_db.create_update_schema()
         await self.configs_model_db.create_update_schema()
         await self.template_entity_db.create_update_schema()
         await self.pending_deferred_edge_db.create_update_schema()
+        await self.package_entity_db.create_update_schema()
         for graph in cast(List[Json], self.database.graphs()):
             log.info(f'Found graph: {graph["name"]}')
             db = self.get_graph_db(graph["name"])
             await db.create_update_schema()
         await self.cleaner.start()
 
     async def stop(self) -> None:
```

### Comparing `resotocore-3.3.1/resotocore/db/deferred_edge_db.py` & `resotocore-3.3.2/resotocore/db/deferred_edge_db.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/db/entitydb.py` & `resotocore-3.3.2/resotocore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/db/graphdb.py` & `resotocore-3.3.2/resotocore/db/graphdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/db/model.py` & `resotocore-3.3.2/resotocore/db/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/db/runningtaskdb.py` & `resotocore-3.3.2/resotocore/db/runningtaskdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/dependencies.py` & `resotocore-3.3.2/resotocore/dependencies.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/error.py` & `resotocore-3.3.2/resotocore/error.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/infra_apps/manifest.py` & `resotocore-3.3.2/resotocore/infra_apps/manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Literal, List, Union, Optional, Any
 from attrs import frozen
 from resotocore.types import Json
 from resotocore.model.typed_model import from_js
+from resotocore.ids import InfraAppName
 from yaml import safe_load
 from jsons import loads as jsons_loads
 
 
 @frozen
 class AppArgs:
     """
@@ -51,52 +52,58 @@
     @param default_config: The default configuration of the app.
     @param args_schema: A list of command line arguments that can be passed to the app.
     Must be compatible with the Python argparse library.
     @param source: The source code of the app.
 
     """
 
-    name: str
+    name: InfraAppName
     description: str
     version: str
     readme: str
-    language: Literal["jinja2"]
+    language: str
     url: str
     icon: str
     categories: List[str]
-    config_schema: Optional[Json]
+    config_schema: Optional[List[Json]]
     default_config: Optional[Json]
-    args_schema: List[AppArgs]
+    args_schema: Optional[List[AppArgs]]
     source: str
 
     # Object creation methods. Use these instead of the __init__ method.
 
     @staticmethod
     def from_json(json: Json) -> "AppManifest":
         return from_js(json, AppManifest)
 
     @staticmethod
     def from_json_str(json_str: str) -> "AppManifest":
-        return AppManifest.from_json(jsons_loads(json_str))
+        json = jsons_loads(json_str)
+        manifest = AppManifest.from_json(json)
+        return manifest
+
+    @staticmethod
+    def from_bytes(b: bytes) -> "AppManifest":
+        return AppManifest.from_json_str(b.decode("utf-8"))
 
     @staticmethod
     def from_yaml_str(yaml_str: str) -> "AppManifest":
         return AppManifest.from_json(safe_load(yaml_str))
 
     @staticmethod
     def new(
-        name: str,
+        name: InfraAppName,
         description: str,
         version: str,
         readme: str,
         language: Literal["jinja2"],
         url: str,
         icon: str,
         categories: List[str],
-        config_schema: Optional[Json],
+        config_schema: Optional[List[Json]],
         default_config: Optional[Json],
         args_schema: List[AppArgs],
         source: str,
     ) -> "AppManifest":
         return AppManifest(
             name=name,
             description=description,
```

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/api/contents/all.json` & `resotocore-3.3.2/resotocore/jupyterlite/api/contents/all.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8949999999999999%*

 * *Differences: {"'content'": "{0: {'created': '2023-04-14T16:19:03.596312Z', 'last_modified': "*

 * *              "'2023-04-14T16:15:47.468749Z'}}",*

 * * "'created'": "'2023-04-14T16:19:03.596312Z'",*

 * * "'last_modified'": "'2023-04-14T16:19:03.596312Z'"}*

```diff
@@ -1,25 +1,25 @@
 {
     "content": [
         {
             "content": null,
-            "created": "2023-03-31T23:56:19.369310Z",
+            "created": "2023-04-14T16:19:03.596312Z",
             "format": null,
-            "last_modified": "2023-03-31T23:51:32.370881Z",
+            "last_modified": "2023-04-14T16:15:47.468749Z",
             "mimetype": null,
             "name": "example.ipynb",
             "path": "example.ipynb",
             "size": 7595,
             "type": "notebook",
             "writable": true
         }
     ],
-    "created": "2023-03-31T23:56:19.369310Z",
+    "created": "2023-04-14T16:19:03.596312Z",
     "format": "json",
-    "last_modified": "2023-03-31T23:56:19.369310Z",
+    "last_modified": "2023-04-14T16:19:03.596312Z",
     "mimetype": null,
     "name": "",
     "path": "",
     "size": null,
     "type": "directory",
     "writable": true
 }
```

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/bootstrap.js` & `resotocore-3.3.2/resotocore/jupyterlite/bootstrap.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1008.7423996.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1008.7423996.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1013.c600eaa.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1013.c600eaa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1018.8daaa2a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1018.8daaa2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1036.3f84b7c.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1036.3f84b7c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1068.3482326.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1068.3482326.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1120.3846654.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1120.3846654.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1169.ba935ce.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1169.ba935ce.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1198.25d5ea9.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1198.25d5ea9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/125.3ad5abd.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/125.3ad5abd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1261.88c6a9a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1261.88c6a9a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1272.44b5a6a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1272.44b5a6a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1320.b53dabd.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1320.b53dabd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1337.9881c6c.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1337.9881c6c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1356.78d0573.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1356.78d0573.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1385.8d43090.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1385.8d43090.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/143.086aef9.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/143.086aef9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1432.2760be9.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1432.2760be9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1473.34de206.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1473.34de206.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1483.b0f9bd2.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1483.b0f9bd2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1496.03867f8.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1496.03867f8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1542.3a90078.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1542.3a90078.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1542.3a90078.js.LICENSE.txt` & `resotocore-3.3.2/resotocore/jupyterlite/build/1542.3a90078.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/157.bfadd48.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/157.bfadd48.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/160.0356d0a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/160.0356d0a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1615.ea9b05f.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1615.ea9b05f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1647.f9bf0fd.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1647.f9bf0fd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1682.3a03166.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1682.3a03166.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1696.8b77f15.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1696.8b77f15.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/170.c870d05.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/170.c870d05.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1809.b7d8942.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1809.b7d8942.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1835.acefed2.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1835.acefed2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1898.2b94c2e.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1898.2b94c2e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/1989.e917572.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/1989.e917572.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2007.0515cb2.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2007.0515cb2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2048.ae5f8ce.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2048.ae5f8ce.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2067.0e50352.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2067.0e50352.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2088.e45e68d.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2088.e45e68d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2089.6e82794.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2089.6e82794.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2118.57bfcca.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2118.57bfcca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2122.808d508.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2122.808d508.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2125.9f428bb.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2125.9f428bb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2167.300d308.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2167.300d308.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2169.a6cfcb2.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2169.a6cfcb2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/217.7562b70.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/217.7562b70.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2303.0753f62.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2303.0753f62.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2351.b511713.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2351.b511713.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2359.8c659ae.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2359.8c659ae.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2363.c625bc2.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2363.c625bc2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2364.deac00c.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2364.deac00c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/237.cd99ebb.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/237.cd99ebb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2401.df2b831.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2401.df2b831.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2469.9cb78b6.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2469.9cb78b6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2476.9aabb04.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2476.9aabb04.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2526.c2108e3.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2526.c2108e3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2527.5a42b8a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2527.5a42b8a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2622.e5bba4b.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2622.e5bba4b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2629.26b2200.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2629.26b2200.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2697.ef870be.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2697.ef870be.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2738.6fb9dd1.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2738.6fb9dd1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2753.70f3b00.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2753.70f3b00.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2756.3d6eaee.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2756.3d6eaee.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2813.01f1491.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2813.01f1491.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2834.42db52f.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2834.42db52f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2897.069c887.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2897.069c887.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/2956.c1d7da9.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/2956.c1d7da9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3004.56b6d8c.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3004.56b6d8c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3037.7c53495.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3037.7c53495.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3051.5ce4d5e.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3051.5ce4d5e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3062.e9a281a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3062.e9a281a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3079.4750bec.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3079.4750bec.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3151.a561877.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3151.a561877.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3154.9ecf019.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3154.9ecf019.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3245.c999c94.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3245.c999c94.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/330.61992f4.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/330.61992f4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3301.9facff2.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3301.9facff2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3325.c195954.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3325.c195954.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3539.29df431.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3539.29df431.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3546.e91daf4.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3546.e91daf4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3562.691155b.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3562.691155b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3566.ca843b7.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3566.ca843b7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3580.9be1770.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3580.9be1770.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3676.ebf1d93.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3676.ebf1d93.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3733.f94f6ea.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3733.f94f6ea.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3814.b631d63.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3814.b631d63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3904.6010839.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3904.6010839.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3937.00a9e88.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3937.00a9e88.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/3970.1e7d81e.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/3970.1e7d81e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/400.449f9c7.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/400.449f9c7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4018.beb2c84.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4018.beb2c84.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4030.ee05a21.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4030.ee05a21.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/404.2cfb2cf.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/404.2cfb2cf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4058.851cb1d.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4058.851cb1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/406.fc80499.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/406.fc80499.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/409.35f299f.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/409.35f299f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4091.bd4a548.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4091.bd4a548.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4151.ef963eb.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4151.ef963eb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4170.b007dfe.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4170.b007dfe.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4171.5fe294f.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4171.5fe294f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4174.16d7ff2.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4174.16d7ff2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4182.8168565.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4182.8168565.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4196.90d47c2.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4196.90d47c2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4206.ce4d631.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4206.ce4d631.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4207.fcd0f7b.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4207.fcd0f7b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4212.667105a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4212.667105a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4262.4153361.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4262.4153361.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4271.73da189.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4271.73da189.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4291.31bc388.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4291.31bc388.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4354.6cee0b6.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4354.6cee0b6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/451.b2fe0fb.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/451.b2fe0fb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4526.b3bcff7.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4526.b3bcff7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4558.522eff3.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4558.522eff3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4569.ee0bb18.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4569.ee0bb18.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4630.f8aa924.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4630.f8aa924.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4690.f7dbd7f.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4690.f7dbd7f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4710.705dfd0.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4710.705dfd0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4738.7a8db62.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4738.7a8db62.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4749.d95260b.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4749.d95260b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4750.dcc0917.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4750.dcc0917.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/48.182a12b.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/48.182a12b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4805.0d84a4d.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4805.0d84a4d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4811.285f48b.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4811.285f48b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4884.d5dcfb1.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4884.d5dcfb1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4885.4e89207.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4885.4e89207.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/489.c5d6e7c.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/489.c5d6e7c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4897.5fd1369.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4897.5fd1369.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/4940.d2cb952.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/4940.d2cb952.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5088.b363823.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5088.b363823.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5115.65cbeea.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5115.65cbeea.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5126.39244e1.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5126.39244e1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5135.d3ad8e8.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5135.d3ad8e8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5153.01e90e9.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5153.01e90e9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5154.6495ddd.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5154.6495ddd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/517.9f09c12.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/517.9f09c12.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/518.b1a14b5.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/518.b1a14b5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/519.87883c1.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/519.87883c1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5213.a606fa8.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5213.a606fa8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5227.8d213ff.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5227.8d213ff.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5228.3d71388.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5228.3d71388.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5234.f48a464.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5234.f48a464.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5286.f84b4a4.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5286.f84b4a4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5342.6aa187c.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5342.6aa187c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5394.d9ffb63.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5394.d9ffb63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5426.81db440.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5426.81db440.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5449.484f7e1.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5449.484f7e1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5451.e1ee9b2.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5451.e1ee9b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5489.cb188b2.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5489.cb188b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/554.ce7f40d.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/554.ce7f40d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5597.6f70034.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5597.6f70034.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5614.4272b09.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5614.4272b09.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5710.c3b4e36.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5710.c3b4e36.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5733.4f6f25c.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5733.4f6f25c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/582.1236fdf.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/582.1236fdf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5823.4baed9c.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5823.4baed9c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5859.6ac4fe2.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5859.6ac4fe2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/590.c297c01.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/590.c297c01.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5914.832df6a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5914.832df6a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/5945.d39af99.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/5945.d39af99.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6061.bc854e2.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6061.bc854e2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6118.c02b404.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6118.c02b404.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6139.ee85a5a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6139.ee85a5a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6186.17f6a4a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6186.17f6a4a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6191.2feb6e6.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6191.2feb6e6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6197.15397b4.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6197.15397b4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/62.d057833.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/62.d057833.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6256.10417ed.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6256.10417ed.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6433.9e8992a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6433.9e8992a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/644.e6ff479.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/644.e6ff479.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/644.e6ff479.js.LICENSE.txt` & `resotocore-3.3.2/resotocore/jupyterlite/build/644.e6ff479.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6475.fe6bde7.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6475.fe6bde7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6517.7379adf.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6517.7379adf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6553.5e1599f.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6553.5e1599f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6576.d5ddce4.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6576.d5ddce4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6604.715e4c0.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6604.715e4c0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6612.2f9795e.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6612.2f9795e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6627.53ac590.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6627.53ac590.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6648.bfe5243.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6648.bfe5243.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6648.bfe5243.js.LICENSE.txt` & `resotocore-3.3.2/resotocore/jupyterlite/build/6648.bfe5243.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6664.1b4a72f.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6664.1b4a72f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6731.5beaf61.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6731.5beaf61.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6731.5beaf61.js.LICENSE.txt` & `resotocore-3.3.2/resotocore/jupyterlite/build/6731.5beaf61.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6787.2bc4778.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6787.2bc4778.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6815.24389cc.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6815.24389cc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6870.af50acc.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6870.af50acc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6891.f98d014.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6891.f98d014.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6952.f9a7329.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6952.f9a7329.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6962.db53086.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6962.db53086.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6974.6305cd0.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6974.6305cd0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6974.6305cd0.js.LICENSE.txt` & `resotocore-3.3.2/resotocore/jupyterlite/build/6974.6305cd0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6981.bcfe168.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6981.bcfe168.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/6990.9bf8f0c.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/6990.9bf8f0c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7010.d9a3d9a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7010.d9a3d9a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7071.ac3061a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7071.ac3061a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7125.6e03225.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7125.6e03225.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7144.7b79049.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7144.7b79049.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/724.6d5bce9.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/724.6d5bce9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7252.1b222e2.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7252.1b222e2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7334.4b1185b.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7334.4b1185b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7353.1f669cb.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7353.1f669cb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7359.3fb41a6.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7359.3fb41a6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7364.5e98a3d.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7364.5e98a3d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7378.9a1e27c.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7378.9a1e27c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7380.1f65978.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7380.1f65978.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7386.39139e0.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7386.39139e0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7495.54216ce.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7495.54216ce.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7505.3011f14.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7505.3011f14.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7509.5ca0029.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7509.5ca0029.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7692.7e69e41.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7692.7e69e41.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7702.0a89622.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7702.0a89622.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7749.06b09da.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7749.06b09da.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7808.d290935.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7808.d290935.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7819.9d50d5e.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7819.9d50d5e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7821.254b995.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7821.254b995.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7821.254b995.js.LICENSE.txt` & `resotocore-3.3.2/resotocore/jupyterlite/build/7821.254b995.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7858.cdac98e.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7858.cdac98e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7892.762d4af.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7892.762d4af.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/7900.9103464.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/7900.9103464.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8028.1bab409.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8028.1bab409.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8072.dc7057b.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8072.dc7057b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8131.aeaee1d.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8131.aeaee1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8199.7c3ab4f.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8199.7c3ab4f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/827.5f79f4c.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/827.5f79f4c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/835.4e4132e.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/835.4e4132e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8370.1f0c2e7.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8370.1f0c2e7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8393.f15a1fb.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8393.f15a1fb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8402.41ac88b.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8402.41ac88b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8412.a71c56e.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8412.a71c56e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8427.a0a5b2f.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8427.a0a5b2f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8445.12eb406.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8445.12eb406.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8476.c861e5b.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8476.c861e5b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8498.51d4fad.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8498.51d4fad.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/850.4167ce1.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/850.4167ce1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8579.76adee3.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8579.76adee3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8590.675efe0.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8590.675efe0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8633.4815201.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8633.4815201.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8695.7f3578a.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8695.7f3578a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8754.a42dc19.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8754.a42dc19.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8800.ee578b6.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8800.ee578b6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8907.f1da997.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8907.f1da997.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8928.eff2684.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8928.eff2684.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8929.ae99e1f.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8929.ae99e1f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/893.39e9e3c.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/893.39e9e3c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/8976.976490c.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/8976.976490c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/901.d40d0d6.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/901.d40d0d6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9077.19ea7ca.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9077.19ea7ca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/911.07e91f9.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/911.07e91f9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9156.8248119.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9156.8248119.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9196.ed69b45.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9196.ed69b45.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9208.057fe7d.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9208.057fe7d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9222.03d0ecd.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9222.03d0ecd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9244.f067be9.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9244.f067be9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9282.60b94bc.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9282.60b94bc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9334.d61a1e4.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9334.d61a1e4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9341.3bb43d7.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9341.3bb43d7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9372.a388c7b.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9372.a388c7b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9602.7bfe4d6.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9602.7bfe4d6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9621.7698d7d.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9621.7698d7d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9647.329ecda.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9647.329ecda.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9684.c0b5cc1.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9684.c0b5cc1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9685.9c6e5f6.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9685.9c6e5f6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9847.75e3ee6.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9847.75e3ee6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9934.0330010.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9934.0330010.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/9939.a757e1d.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/9939.a757e1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/add-above.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/add-above.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/add-below.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/add-below.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/bug-dot.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/bug-dot.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/bug.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/bug.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/build.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/build.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/case-sensitive.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/case-sensitive.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/close.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/close.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/copyright.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/copyright.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/cut.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/cut.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/duplicate.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/duplicate.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/fa-brands-400.woff2` & `resotocore-3.3.2/resotocore/jupyterlite/build/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/fa-regular-400.woff2` & `resotocore-3.3.2/resotocore/jupyterlite/build/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/fa-solid-900.woff2` & `resotocore-3.3.2/resotocore/jupyterlite/build/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/html5.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/html5.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/json.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/json.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/julia.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/julia.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/jupyter-favicon.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/jupyter-favicon.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/jupyter.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/jupyter.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/jupyterlab-wordmark.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/jupyterlab-wordmark.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/lab/bundle.js` & `resotocore-3.3.2/resotocore/jupyterlite/build/lab/bundle.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/listings-info.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/listings-info.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/move-down.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/move-down.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/move-up.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/move-up.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/not-trusted.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/not-trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/palette.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/palette.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/pdf.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/pdf.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/pypi/all.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/pypi/all.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/pypi/ipykernel-6.9.2-py3-none-any.whl` & `resotocore-3.3.2/resotocore/jupyterlite/build/pypi/ipykernel-6.9.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/pypi/piplite-0.1.0b13-py3-none-any.whl` & `resotocore-3.3.2/resotocore/jupyterlite/build/pypi/piplite-0.1.0b13-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/pypi/pyolite-0.1.0b13-py3-none-any.whl` & `resotocore-3.3.2/resotocore/jupyterlite/build/pypi/pyolite-0.1.0b13-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/pypi/widgetsnbextension-3.6.0-py3-none-any.whl` & `resotocore-3.3.2/resotocore/jupyterlite/build/pypi/widgetsnbextension-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/pypi/widgetsnbextension-4.0.2-py3-none-any.whl` & `resotocore-3.3.2/resotocore/jupyterlite/build/pypi/widgetsnbextension-4.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/python.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/python.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/react.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/react.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/regex.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/regex.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/schemas/all.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/schemas/all.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/settings.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/settings.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/tag.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/tag.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/terminal.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/terminal.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css` & `resotocore-3.3.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css` & `resotocore-3.3.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/third-party-licenses.json` & `resotocore-3.3.2/resotocore/jupyterlite/build/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/toc.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/toc.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/build/trusted.svg` & `resotocore-3.3.2/resotocore/jupyterlite/build/trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/config-utils.js` & `resotocore-3.3.2/resotocore/jupyterlite/config-utils.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.e171e024d2412b46d706.js` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.e171e024d2412b46d706.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.04c1d88665796339989c.js` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.04c1d88665796339989c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.04c1d88665796339989c.js.LICENSE.txt` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.04c1d88665796339989c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.e12be0c175cda2484e38.js` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.e12be0c175cda2484e38.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.5a61eaf4adea42288d59.js` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.5a61eaf4adea42288d59.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json` & `resotocore-3.3.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/files/example.ipynb` & `resotocore-3.3.2/resotocore/jupyterlite/files/example.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/icon-120x120.png` & `resotocore-3.3.2/resotocore/jupyterlite/icon-120x120.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/icon-512x512.png` & `resotocore-3.3.2/resotocore/jupyterlite/icon-512x512.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/index.html` & `resotocore-3.3.2/resotocore/jupyterlite/index.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/jupyter-lite.ipynb` & `resotocore-3.3.2/resotocore/jupyterlite/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/jupyter-lite.json` & `resotocore-3.3.2/resotocore/jupyterlite/jupyter-lite.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/jupyterlite.schema.v0.json` & `resotocore-3.3.2/resotocore/jupyterlite/jupyterlite.schema.v0.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/kernelspecs/javascript.svg` & `resotocore-3.3.2/resotocore/jupyterlite/kernelspecs/javascript.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/kernelspecs/python.svg` & `resotocore-3.3.2/resotocore/jupyterlite/kernelspecs/python.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/lab/favicon.ico` & `resotocore-3.3.2/resotocore/jupyterlite/lab/favicon.ico`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/lab/index.html` & `resotocore-3.3.2/resotocore/jupyterlite/lab/index.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/lab/jupyter-lite.ipynb` & `resotocore-3.3.2/resotocore/jupyterlite/lab/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/lab/package.json` & `resotocore-3.3.2/resotocore/jupyterlite/lab/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/manifest.webmanifest` & `resotocore-3.3.2/resotocore/jupyterlite/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/package.json` & `resotocore-3.3.2/resotocore/jupyterlite/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/piplite.schema.v0.json` & `resotocore-3.3.2/resotocore/jupyterlite/piplite.schema.v0.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/jupyterlite/services.js` & `resotocore-3.3.2/resotocore/jupyterlite/services.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/message_bus.py` & `resotocore-3.3.2/resotocore/message_bus.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/metrics.py` & `resotocore-3.3.2/resotocore/metrics.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/model/adjust_node.py` & `resotocore-3.3.2/resotocore/model/adjust_node.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/model/db_updater.py` & `resotocore-3.3.2/resotocore/model/db_updater.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/model/graph_access.py` & `resotocore-3.3.2/resotocore/model/graph_access.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/model/json_schema.py` & `resotocore-3.3.2/resotocore/model/json_schema.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/model/model.py` & `resotocore-3.3.2/resotocore/model/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 @define(order=True, hash=True, frozen=True)
 class Property:
     name: str
     kind: str
     required: bool = False
     synthetic: Optional[SyntheticProperty] = None
     description: Optional[str] = None
+    metadata: Optional[Json] = None
 
     def __attrs_post_init__(self) -> None:
         assert self.synthetic is None or not self.required, "Synthetic properties can not be required!"
 
     def resolve(self, model: Dict[str, Kind]) -> Kind:
         return Property.parse_kind(self.kind, model)
```

### Comparing `resotocore-3.3.1/resotocore/model/model_handler.py` & `resotocore-3.3.2/resotocore/model/model_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/model/resolve_in_graph.py` & `resotocore-3.3.2/resotocore/model/resolve_in_graph.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/model/transform_kind_convert.py` & `resotocore-3.3.2/resotocore/model/transform_kind_convert.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/model/typed_model.py` & `resotocore-3.3.2/resotocore/model/typed_model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/query/__init__.py` & `resotocore-3.3.2/resotocore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/query/model.py` & `resotocore-3.3.2/resotocore/query/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/query/query_parser.py` & `resotocore-3.3.2/resotocore/query/query_parser.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/query/template_expander.py` & `resotocore-3.3.2/resotocore/query/template_expander.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/query/template_expander_service.py` & `resotocore-3.3.2/resotocore/query/template_expander_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     async def get_template(self, name: str) -> Optional[Template]:
         return await self.db.get(name)
 
     async def list_templates(self) -> List[Template]:
         return [t async for t in self.db.all()]
 
     async def parse_query_from_command_line(self, to_parse: str, on_section: str, **env: str) -> str:
-        final_env = {**env, "section": on_section}
+        final_env = {**env, "section": on_section, "no_rewrite": "true"}
         parsed = await self.cli.evaluate_cli_command(to_parse, CLIContext(env=final_env), replace_place_holder=False)
         if len(parsed) == 1:
             first_line = parsed[0]
             if len(first_line.executable_commands) == 1 and first_line.executable_commands[0].name == "execute_search":
                 query = first_line.executable_commands[0].arg or ""
                 return strip_quotes(query)
             else:
```

### Comparing `resotocore-3.3.1/resotocore/report/inspector_service.py` & `resotocore-3.3.2/resotocore/report/inspector_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from resotocore.analytics import CoreEvent
 from resotocore.cli.model import CLIContext, CLI
 from resotocore.config import ConfigEntity, ConfigHandler
 from resotocore.db.model import QueryModel
 from resotocore.error import NotFoundError
 from resotocore.ids import ConfigId
 from resotocore.model.model import Model
+from resotocore.model.resolve_in_graph import NodePath
 from resotocore.query.model import Aggregate, AggregateFunction, Query, P, AggregateVariable, AggregateVariableName
 from resotocore.report import (
     Inspector,
     ReportCheck,
     Benchmark,
     BenchmarkResult,
     CheckCollection,
@@ -24,17 +25,20 @@
     CheckConfigPrefix,
     BenchmarkConfigPrefix,
     CheckConfigRoot,
     ResotoReportValues,
     BenchmarkConfigRoot,
     ResotoReportBenchmark,
     ResotoReportCheck,
+    ReportSeverity,
+    ReportSeverityPriority,
 )
 from resotocore.report.report_config import ReportCheckCollectionConfig, BenchmarkConfig
 from resotocore.types import Json
+from resotocore.util import value_in_path
 from resotocore.web.service import Service
 
 log = logging.getLogger(__name__)
 
 CountByAccount = Dict[str, int]
 
 
@@ -45,16 +49,24 @@
 def check_id(name: str) -> ConfigId:
     return ConfigId(CheckConfigPrefix + name)
 
 
 @define
 class CheckContext:
     accounts: Optional[List[str]] = None
+    severity: Optional[ReportSeverity] = None
+    only_failed: bool = False
     parallel_checks: int = 10
 
+    def includes_severity(self, severity: ReportSeverity) -> bool:
+        if self.severity is None:
+            return True
+        else:
+            return ReportSeverityPriority[self.severity] <= ReportSeverityPriority[severity]
+
 
 class InspectorService(Inspector, Service):
     def __init__(self, cli: CLI) -> None:
         self.config_handler: ConfigHandler = cli.dependencies.config_handler
         self.db_access = cli.dependencies.db_access
         self.cli = cli
         self.template_expander = cli.dependencies.template_expander
@@ -75,16 +87,30 @@
                 await self.config_handler.put_config(ConfigEntity(cid, {BenchmarkConfigRoot: js}), validate=False)
         for name, js in ReportCheckCollectionConfig.from_files().items():
             if overwrite or check_id(name) not in config_ids:
                 cid = check_id(name)
                 log.info(f"Creating check collection config {cid}")
                 await self.config_handler.put_config(ConfigEntity(cid, {CheckConfigRoot: js}), validate=False)
 
+    async def list_benchmarks(self) -> List[Benchmark]:
+        return [
+            await self.__benchmark(i)
+            async for i in self.config_handler.list_config_ids()
+            if i.startswith(BenchmarkConfigPrefix)
+        ]
+
+    async def benchmark(self, name: str) -> Optional[Benchmark]:
+        try:
+            return await self.__benchmark(benchmark_id(name))
+        except ValueError:
+            return None
+
     async def list_checks(
         self,
+        *,
         provider: Optional[str] = None,
         service: Optional[str] = None,
         category: Optional[str] = None,
         kind: Optional[str] = None,
         check_ids: Optional[List[str]] = None,
     ) -> List[ReportCheck]:
         def inspection_matches(inspection: ReportCheck) -> bool:
@@ -95,51 +121,67 @@
                 and (kind is None or kind == inspection.result_kind)
                 and (check_ids is None or inspection.id in check_ids)
             )
 
         return await self.filter_checks(inspection_matches)
 
     async def perform_benchmark(
-        self, benchmark_name: str, graph: str, accounts: Optional[List[str]] = None
+        self,
+        graph: str,
+        benchmark_name: str,
+        *,
+        accounts: Optional[List[str]] = None,
+        severity: Optional[ReportSeverity] = None,
+        only_failing: bool = False,
     ) -> BenchmarkResult:
-        cfg = await self.config_handler.get_config(benchmark_id(benchmark_name))
-        if cfg is None or BenchmarkConfigRoot not in cfg.config:
-            raise ValueError(f"Unknown benchmark: {benchmark_name}")
-        benchmark = BenchmarkConfig.from_config(cfg)
-        context = CheckContext(accounts=accounts)
+        benchmark = await self.__benchmark(benchmark_id(benchmark_name))
+        context = CheckContext(accounts=accounts, severity=severity, only_failed=only_failing)
         return await self.__perform_benchmark(benchmark, graph, context)
 
     async def perform_checks(
         self,
         graph: str,
+        *,
         provider: Optional[str] = None,
         service: Optional[str] = None,
         category: Optional[str] = None,
         kind: Optional[str] = None,
+        check_ids: Optional[List[str]] = None,
         accounts: Optional[List[str]] = None,
+        severity: Optional[ReportSeverity] = None,
+        only_failing: bool = False,
     ) -> BenchmarkResult:
-        checks = await self.list_checks(provider, service, category, kind)
+        checks = await self.list_checks(
+            provider=provider, service=service, category=category, kind=kind, check_ids=check_ids
+        )
         provider_name = f"{provider}_" if provider else ""
         service_name = f"{service}_" if service else ""
         category_name = f"{category}_" if category else ""
         kind_name = f"{kind}_" if kind else ""
-        title = f"{provider_name}{service_name}{category_name}{kind_name}_benchmark"
+        check_id_name = f"{check_ids[0]}_" if check_ids else ""
+        title = f"{provider_name}{service_name}{category_name}{kind_name}{check_id_name}benchmark"
         benchmark = Benchmark(
             id=title,
             title=title,
             description="On demand benchmark",
             documentation="On demand benchmark",
             framework="resoto",
             version="1.0",
             checks=[c.id for c in checks],
             children=[],
         )
-        context = CheckContext(accounts=accounts)
+        context = CheckContext(accounts=accounts, severity=severity, only_failed=only_failing)
         return await self.__perform_benchmark(benchmark, graph, context)
 
+    async def __benchmark(self, cfg_id: ConfigId) -> Benchmark:
+        cfg = await self.config_handler.get_config(cfg_id)
+        if cfg is None or BenchmarkConfigRoot not in cfg.config:
+            raise ValueError(f"Unknown benchmark: {cfg_id}")
+        return BenchmarkConfig.from_config(cfg)
+
     async def filter_checks(self, report_filter: Optional[Callable[[ReportCheck], bool]] = None) -> List[ReportCheck]:
         cfg_ids = [i async for i in self.config_handler.list_config_ids() if i.startswith(CheckConfigPrefix)]
         loaded = await asyncio.gather(*[self.config_handler.get_config(cfg_id) for cfg_id in cfg_ids])
         # fmt: off
         return [
             check
             for entry in loaded if isinstance(entry, ConfigEntity) and CheckConfigRoot in entry.config
@@ -193,35 +235,43 @@
             return perform_search(resoto_search)
         elif resoto_cmd := inspection.detect.get("resoto_cmd"):
             return perform_cmd(resoto_cmd)
         else:
             return stream.empty()  # type: ignore
 
     async def __perform_benchmark(self, benchmark: Benchmark, graph: str, context: CheckContext) -> BenchmarkResult:
+        if context.accounts is None:
+            context.accounts = await self.__list_accounts(benchmark, graph)
+
         perform_checks = await self.list_checks(check_ids=benchmark.nested_checks())
-        check_by_id = {c.id: c for c in perform_checks}
+        check_by_id = {c.id: c for c in perform_checks if context.includes_severity(c.severity)}
         result = await self.__perform_checks(graph, perform_checks, context)
         await self.event_sender.core_event(CoreEvent.BenchmarkPerformed, {"benchmark": benchmark.id})
 
         def to_result(cc: CheckCollection) -> CheckCollectionResult:
-            check_results = [CheckResult(check_by_id[cid], result.get(cid, {})) for cid in cc.checks or []]
+            check_results = [
+                CheckResult(check_by_id[cid], result.get(cid, {})) for cid in cc.checks or [] if cid in check_by_id
+            ]
             children = [to_result(c) for c in cc.children or []]
             return CheckCollectionResult(
                 cc.title, cc.description, documentation=cc.documentation, checks=check_results, children=children
             )
 
-        top = to_result(benchmark)
+        top = to_result(benchmark).filter_result(context.only_failed)
         return BenchmarkResult(
             benchmark.title,
             benchmark.description,
             benchmark.framework,
             benchmark.version,
             documentation=benchmark.documentation,
             checks=top.checks,
             children=top.children,
+            accounts=context.accounts,
+            only_failed=context.only_failed,
+            severity=context.severity,
         )
 
     async def __perform_checks(
         self, graph: str, checks: List[ReportCheck], context: CheckContext
     ) -> Dict[str, CountByAccount]:
         # load model
         model = await self.model_handler.load_model()
@@ -282,14 +332,24 @@
             return await perform_cmd(resoto_cmd)
         elif inspection.detect.get("manual"):
             # let's assume the manual check is successful
             return {}
         else:
             raise ValueError(f"Invalid inspection {inspection.id}: no resoto or resoto_cmd defined")
 
+    async def __list_accounts(self, benchmark: Benchmark, graph: str) -> List[str]:
+        model = await self.model_handler.load_model()
+        gdb = self.db_access.get_graph_db(graph)
+        query = Query.by("account")
+        if benchmark.clouds:
+            query = query.combine(Query.by(P.single("ancestors.cloud.reported.id").is_in(benchmark.clouds)))
+        async with await gdb.search_list(QueryModel(query, model)) as crs:
+            ids = [value_in_path(a, NodePath.reported_id) async for a in crs]
+            return [aid for aid in ids if aid is not None]
+
     async def validate_benchmark_config(self, json: Json) -> Optional[Json]:
         try:
             benchmark = BenchmarkConfig.from_config(ConfigEntity(ResotoReportBenchmark, json))
             all_checks = {c.id for c in await self.filter_checks()}
             missing = []
             for check in benchmark.nested_checks():
                 if check not in all_checks:
```

### Comparing `resotocore-3.3.1/resotocore/report/report_config.py` & `resotocore-3.3.2/resotocore/report/report_config.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/api-doc.yaml` & `resotocore-3.3.2/resotocore/static/api-doc.yaml`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/ck-unicode-truecolor.ans` & `resotocore-3.3.2/resotocore/static/ck-unicode-truecolor.ans`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/report/benchmark/aws/aws_cis_1_5.json` & `resotocore-3.3.2/resotocore/static/report/benchmark/aws/aws_cis_1_5.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/report/check_template.json` & `resotocore-3.3.2/resotocore/static/report/check_template.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/report/checks/aws/aws_apigateway.json` & `resotocore-3.3.2/resotocore/static/report/checks/aws/aws_apigateway.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/report/checks/aws/aws_cloudtrail.json` & `resotocore-3.3.2/resotocore/static/report/checks/aws/aws_cloudtrail.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/report/checks/aws/aws_config.json` & `resotocore-3.3.2/resotocore/static/report/checks/aws/aws_config.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/report/checks/aws/aws_ec2.json` & `resotocore-3.3.2/resotocore/static/report/checks/aws/aws_ec2.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/report/checks/aws/aws_efs.json` & `resotocore-3.3.2/resotocore/static/report/checks/aws/aws_efs.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/report/checks/aws/aws_iam.json` & `resotocore-3.3.2/resotocore/static/report/checks/aws/aws_iam.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/report/checks/aws/aws_kms.json` & `resotocore-3.3.2/resotocore/static/report/checks/aws/aws_kms.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/report/checks/aws/aws_lambda.json` & `resotocore-3.3.2/resotocore/static/report/checks/aws/aws_lambda.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/report/checks/aws/aws_rds.json` & `resotocore-3.3.2/resotocore/static/report/checks/aws/aws_rds.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/static/report/checks/aws/aws_s3.json` & `resotocore-3.3.2/resotocore/static/report/checks/aws/aws_s3.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/task/__init__.py` & `resotocore-3.3.2/resotocore/task/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/task/model.py` & `resotocore-3.3.2/resotocore/task/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/task/scheduler.py` & `resotocore-3.3.2/resotocore/task/scheduler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/task/start_workflow_on_first_subscriber.py` & `resotocore-3.3.2/resotocore/task/start_workflow_on_first_subscriber.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/task/subscribers.py` & `resotocore-3.3.2/resotocore/task/subscribers.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/task/task_description.py` & `resotocore-3.3.2/resotocore/task/task_description.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/task/task_handler.py` & `resotocore-3.3.2/resotocore/task/task_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/types.py` & `resotocore-3.3.2/resotocore/types.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/util.py` & `resotocore-3.3.2/resotocore/util.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/validator.py` & `resotocore-3.3.2/resotocore/validator.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/web/api.py` & `resotocore-3.3.2/resotocore/web/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,26 +44,23 @@
 from aiohttp.hdrs import METH_ANY
 from aiohttp.web import Request, StreamResponse, WebSocketResponse
 from aiohttp.web_exceptions import HTTPNotFound, HTTPNoContent, HTTPOk, HTTPNotAcceptable
 from aiohttp.web_fileresponse import FileResponse
 from aiohttp.web_response import json_response
 from aiohttp_swagger3 import SwaggerFile, SwaggerUiSettings
 from aiostream import stream
-from aiostream.core import Stream
 from attrs import evolve
 from networkx.readwrite import cytoscape_data
 from resotoui import ui_path
 
 from resotocore.analytics import AnalyticsEventSender, AnalyticsEvent
-from resotocore.cli.command import ListCommand, alias_names
+from resotocore.cli.command import alias_names
 from resotocore.cli.model import (
     ParsedCommandLine,
     CLIContext,
-    OutputTransformer,
-    PreserveOutputFormat,
     CLICommand,
     InternalPart,
     AliasTemplate,
     WorkerCustomCommand,
     CLI,
 )
 from resotocore.config import ConfigHandler, ConfigValidation, ConfigEntity
@@ -253,24 +250,27 @@
                 web.static(prefix + "/static", static_path),
                 web.get(prefix + "/notebook", self.forward("/notebook/index.html")),
                 web.static(prefix + "/notebook", jupyterlite_path),
                 # metrics
                 web.get(prefix + "/metrics", self.metrics),
                 # config operations
                 web.get(prefix + "/configs", self.list_configs),
-                web.put(prefix + "/config/{config_id}", self.put_config),
-                web.get(prefix + "/config/{config_id}", self.get_config),
-                web.patch(prefix + "/config/{config_id}", self.patch_config),
-                web.delete(prefix + "/config/{config_id}", self.delete_config),
+                web.patch(prefix + "/config/{config_id:[^{}]+}", self.patch_config),
+                web.delete(prefix + "/config/{config_id:[^{}]+}", self.delete_config),
                 # config model operations
                 web.get(prefix + "/configs/validation", self.list_config_models),
                 web.get(prefix + "/configs/model", self.get_configs_model),
                 web.patch(prefix + "/configs/model", self.update_configs_model),
-                web.put(prefix + "/config/{config_id}/validation", self.put_config_validation),
-                web.get(prefix + "/config/{config_id}/validation", self.get_config_validation),
+                web.put(prefix + "/config_validation/{config_id:[^{}]+}", self.put_config_validation),
+                web.get(prefix + "/config_validation/{config_id:[^{}]+}", self.get_config_validation),
+                web.put(prefix + "/config/{config_id:[^{}]+}/validation", self.put_config_validation),
+                web.get(prefix + "/config/{config_id:[^{}]+}/validation", self.get_config_validation),
+                # config operations, moved here to avoid early matching
+                web.put(prefix + "/config/{config_id:[^{}]+}", self.put_config),
+                web.get(prefix + "/config/{config_id:[^{}]+}", self.get_config),
                 # ca operations
                 web.get(prefix + "/ca/cert", self.certificate),
                 web.post(prefix + "/ca/sign", self.sign_certificate),
                 # system operations
                 web.get(prefix + "/system/ping", self.ping),
                 web.get(prefix + "/system/ready", self.ready),
                 # forwards
@@ -498,34 +498,36 @@
         graph = request.match_info["graph_id"]
         provider = request.query.get("provider")
         service = request.query.get("service")
         category = request.query.get("category")
         kind = request.query.get("kind")
         acc = request.query.get("accounts")
         accounts = [a.strip() for a in acc.split(",")] if acc else None
-        result = await self.inspector.perform_checks(graph, provider, service, category, kind, accounts)
+        result = await self.inspector.perform_checks(
+            graph, provider=provider, service=service, category=category, kind=kind, accounts=accounts
+        )
         return await single_result(request, to_js(result))
 
     async def perform_benchmark(self, request: Request) -> StreamResponse:
         benchmark = request.match_info["benchmark"]
         graph = request.match_info["graph_id"]
         acc = request.query.get("accounts")
         accounts = [a.strip() for a in acc.split(",")] if acc else None
-        result = await self.inspector.perform_benchmark(benchmark, graph, accounts)
+        result = await self.inspector.perform_benchmark(graph, benchmark, accounts=accounts)
         result_graph = result.to_graph()
         async with stream.iterate(result_graph).stream() as streamer:
             await self.stream_response_from_gen(request, streamer, len(result_graph))
         return await single_result(request, to_js(result))
 
     async def inspection_checks(self, request: Request) -> StreamResponse:
         provider = request.query.get("provider")
         service = request.query.get("service")
         category = request.query.get("category")
         kind = request.query.get("kind")
-        inspections = await self.inspector.list_checks(provider, service, category, kind)
+        inspections = await self.inspector.list_checks(provider=provider, service=service, category=category, kind=kind)
         return await single_result(request, to_js(inspections))
 
     async def inspection_results(self, request: Request) -> StreamResponse:
         graph = request.match_info["graph_id"]
         check_id = request.match_info["check_id"]
         acc = request.query.get("accounts")
         accounts = [a.strip() for a in acc.split(",")] if acc else None
@@ -990,68 +992,61 @@
                             writer.write(await part.read_chunk())
                 ctx = evolve(ctx, uploaded_files=files)
             else:
                 raise AttributeError(f"Not able to handle: {request.content_type}")
 
             # we want to eagerly evaluate the command, so that parse exceptions will throw directly here
             parsed = await self.cli.evaluate_cli_command(command, ctx)
-            return await self.execute_parsed(request, command, parsed)
+            return await self.execute_parsed(request, command, parsed, ctx)
         finally:
             if temp_dir:
                 shutil.rmtree(temp_dir)
 
-    async def execute_parsed(self, request: Request, command: str, parsed: List[ParsedCommandLine]) -> StreamResponse:
+    async def execute_parsed(
+        self, request: Request, command: str, parsed: List[ParsedCommandLine], ctx: CLIContext
+    ) -> StreamResponse:
         # make sure, all requirements are fulfilled
         not_met_requirements = [not_met for line in parsed for not_met in line.unmet_requirements]
         # what is the accepted content type
         # only required for multipart requests
         boundary = "cli-part"
         mp_response = web.StreamResponse(
             status=200, reason="OK", headers={"Content-Type": f"multipart/mixed;boundary={boundary}"}
         )
 
-        async def list_or_gen(current: ParsedCommandLine) -> Tuple[Optional[int], Stream]:
-            maybe_count, out_gen = await current.execute()
-            if (
-                request.headers.get("accept") == "text/plain"
-                and current.executable_commands
-                and not isinstance(current.executable_commands[-1].command, (OutputTransformer, PreserveOutputFormat))
-            ):
-                out_gen = await ListCommand(self.cli.dependencies).parse(ctx=current.ctx).flow(out_gen)
-
-            return maybe_count, out_gen
-
         if not_met_requirements:
             requirements = [req for line in parsed for cmd in line.executable_commands for req in cmd.action.required]
             data = {"command": command, "env": dict(request.query), "required": to_json(requirements)}
             return web.json_response(data, status=424)
         elif len(parsed) == 1:
             first_result = parsed[0]
-            count, generator = await list_or_gen(first_result)
+            count, generator = await first_result.execute()
             # flat the results from 0 or 1
             async with generator.stream() as streamer:
                 gen = await force_gen(streamer)
-                if first_result.produces.json:
-                    return await self.stream_response_from_gen(request, gen, count)
+                if first_result.produces.text:
+                    text_gen = ctx.text_generator(first_result, gen)
+                    return await self.stream_response_from_gen(request, text_gen, count)
                 elif first_result.produces.file_path:
                     await mp_response.prepare(request)
                     await Api.multi_file_response(first_result, gen, boundary, mp_response)
                     await Api.close_multi_part_response(mp_response, boundary)
                     return mp_response
                 else:
                     raise AttributeError(f"Can not handle type: {first_result.produces}")
         elif len(parsed) > 1:
             await mp_response.prepare(request)
             for single in parsed:
-                count, generator = await list_or_gen(single)
+                count, generator = await single.execute()
                 async with generator.stream() as streamer:
                     gen = await force_gen(streamer)
-                    if single.produces.json:
+                    if single.produces.text:
                         with MultipartWriter(repr(single.produces), boundary) as mp:
-                            content_type, result_stream = await result_binary_gen(request, gen)
+                            text_gen = ctx.text_generator(single, gen)
+                            content_type, result_stream = await result_binary_gen(request, text_gen)
                             mp.append_payload(
                                 AsyncIterablePayload(result_stream, content_type=content_type, headers=single.envelope)
                             )
                             await mp.write(mp_response, close_boundary=False)
                     elif single.produces.file_path:
                         await Api.multi_file_response(single, gen, boundary, mp_response)
                     else:
```

### Comparing `resotocore-3.3.1/resotocore/web/certificate_handler.py` & `resotocore-3.3.2/resotocore/web/certificate_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/web/content_renderer.py` & `resotocore-3.3.2/resotocore/web/content_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/web/directives.py` & `resotocore-3.3.2/resotocore/web/directives.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/web/tsdb.py` & `resotocore-3.3.2/resotocore/web/tsdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore/worker_task_queue.py` & `resotocore-3.3.2/resotocore/worker_task_queue.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/resotocore.egg-info/PKG-INFO` & `resotocore-3.3.2/resotocore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.3.1
+Version: 3.3.2
 Summary: Keeps all the things.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotocore
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `resotocore-3.3.1/resotocore.egg-info/SOURCES.txt` & `resotocore-3.3.2/resotocore.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,19 +51,23 @@
 resotocore/db/db_access.py
 resotocore/db/deferred_edge_db.py
 resotocore/db/entitydb.py
 resotocore/db/graphdb.py
 resotocore/db/jobdb.py
 resotocore/db/model.py
 resotocore/db/modeldb.py
+resotocore/db/packagedb.py
 resotocore/db/runningtaskdb.py
 resotocore/db/subscriberdb.py
 resotocore/db/templatedb.py
 resotocore/infra_apps/__init__.py
+resotocore/infra_apps/local_runtime.py
 resotocore/infra_apps/manifest.py
+resotocore/infra_apps/package_manager.py
+resotocore/infra_apps/runtime.py
 resotocore/jupyterlite/bootstrap.js
 resotocore/jupyterlite/config-utils.js
 resotocore/jupyterlite/icon-120x120.png
 resotocore/jupyterlite/icon-512x512.png
 resotocore/jupyterlite/index.html
 resotocore/jupyterlite/jupyter-lite.ipynb
 resotocore/jupyterlite/jupyter-lite.json
@@ -569,14 +573,15 @@
 resotocore/model/typed_model.py
 resotocore/query/__init__.py
 resotocore/query/model.py
 resotocore/query/query_parser.py
 resotocore/query/template_expander.py
 resotocore/query/template_expander_service.py
 resotocore/report/__init__.py
+resotocore/report/benchmark_renderer.py
 resotocore/report/inspector_service.py
 resotocore/report/report_config.py
 resotocore/static/api-doc.yaml
 resotocore/static/ck-unicode-truecolor.ans
 resotocore/static/report/benchmark_template.json
 resotocore/static/report/check_template.json
 resotocore/static/report/benchmark/aws/aws_cis_1_5.json
```

### Comparing `resotocore-3.3.1/setup.cfg` & `resotocore-3.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `resotocore-3.3.1/setup.py` & `resotocore-3.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
             pip.main(["install", "-r", "requirements-jupyterlite.txt"])
             check_call(["jupyter", "lite", "build", "--config", "jupyter_lite_config.json"])
 
 
 setup(
     name="resotocore",
-    version="3.3.1",
+    version="3.3.2",
     description="Keeps all the things.",
     python_requires=">=3.5",
     classifiers=["Programming Language :: Python :: 3"],
     entry_points={"console_scripts": ["resotocore=resotocore.__main__:main"]},
     install_requires=read_requirements("requirements.txt"),
     license="Apache Software License 2.0",
     long_description=read("README.md"),
```

