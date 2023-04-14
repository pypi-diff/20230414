# Comparing `tmp/domolibrary-0.0.8.tar.gz` & `tmp/domolibrary-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-0.0.8.tar", last modified: Mon Jan 30 14:17:38 2023, max compression
+gzip compressed data, was "domolibrary-0.0.9.tar", last modified: Mon Jan 30 17:31:54 2023, max compression
```

## Comparing `domolibrary-0.0.8.tar` & `domolibrary-0.0.9.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.386252 domolibrary-0.0.8/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.354252 domolibrary-0.0.8/Automation/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.8/Automation/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.0.8/Automation/automation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.354252 domolibrary-0.0.8/DataOcean/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DataOcean/Transport.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DataOcean/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DataOcean/cnfg_athena_highbandwidth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DataOcean/cnfg_pgsql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DataOcean/cnfg_s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DataOcean/cnfg_snowflake.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.362252 domolibrary-0.0.8/DomoClasses/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.0.8/DomoClasses/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoAppDb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4504 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.0.8/DomoClasses/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoCertification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.0.8/DomoClasses/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12089 2023-01-17 21:03:25.000000 domolibrary-0.0.8/DomoClasses/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3370 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.0.8/DomoClasses/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoTag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.370252 domolibrary-0.0.8/DomoClasses/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.0.8/DomoClasses/routes/account_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/activity_log_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/appdb_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/application_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/auth_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/bootstrap_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/card_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/datacenter_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/dataflow_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/dataset_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6036 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/get_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/grant_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/group_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/instance_config_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5695 2023-01-17 21:03:25.000000 domolibrary-0.0.8/DomoClasses/routes/job_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1386 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/page_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/pdp_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/publish_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/role_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/sandbox_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/stream_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.0.8/DomoClasses/routes/user_routes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.370252 domolibrary-0.0.8/GitHub/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.8/GitHub/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.0.8/GitHub/get_github_file.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.0.8/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.0.8/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11771 2023-01-30 14:17:38.386252 domolibrary-0.0.8/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10995 2023-01-25 20:10:33.000000 domolibrary-0.0.8/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.370252 domolibrary-0.0.8/domolibrary/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    78237 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/_modidx.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.374252 domolibrary-0.0.8/domolibrary/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11301 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/classes/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4076 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/classes/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3077 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/classes/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23907 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/classes/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2022 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/classes/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9363 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/classes/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/classes/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.378252 domolibrary-0.0.8/domolibrary/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11578 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/client/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/client/Logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4804 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/client/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8186 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/client/get_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.378252 domolibrary-0.0.8/domolibrary/integrations/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17086 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/integrations/DomoJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/integrations/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.378252 domolibrary-0.0.8/domolibrary/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5183 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/routes/account.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/routes/activity_log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2144 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/routes/bootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15390 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/routes/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5783 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/routes/user.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.382252 domolibrary-0.0.8/domolibrary/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1077 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      988 2023-01-30 14:15:57.000000 domolibrary-0.0.8/domolibrary/utils/convert.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.374252 domolibrary-0.0.8/domolibrary.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11771 2023-01-30 14:17:38.000000 domolibrary-0.0.8/domolibrary.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3079 2023-01-30 14:17:38.000000 domolibrary-0.0.8/domolibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-01-30 14:17:38.000000 domolibrary-0.0.8/domolibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-01-30 14:17:38.000000 domolibrary-0.0.8/domolibrary.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-01-11 00:36:49.000000 domolibrary-0.0.8/domolibrary.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-01-30 14:17:38.000000 domolibrary-0.0.8/domolibrary.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-01-30 14:17:38.000000 domolibrary-0.0.8/domolibrary.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1028 2023-01-30 14:15:24.000000 domolibrary-0.0.8/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-01-30 14:17:38.386252 domolibrary-0.0.8/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.0.8/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 14:17:38.382252 domolibrary-0.0.8/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.0.8/utils/Base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.0.8/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.0.8/utils/Exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.0.8/utils/LoggerClass.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.0.8/utils/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.8/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.0.8/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.0.8/utils/consol_get_creds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.0.8/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.0.8/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3659 2023-01-05 15:38:44.000000 domolibrary-0.0.8/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.796988 domolibrary-0.0.9/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.780988 domolibrary-0.0.9/Automation/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.9/Automation/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.0.9/Automation/automation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.780988 domolibrary-0.0.9/DataOcean/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DataOcean/Transport.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DataOcean/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DataOcean/cnfg_athena_highbandwidth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DataOcean/cnfg_pgsql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DataOcean/cnfg_s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DataOcean/cnfg_snowflake.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.784988 domolibrary-0.0.9/DomoClasses/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoAppDb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4504 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoCertification.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12089 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3370 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoTag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.788988 domolibrary-0.0.9/DomoClasses/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/routes/account_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/activity_log_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/appdb_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/application_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/auth_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/bootstrap_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/card_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/datacenter_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/dataflow_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/dataset_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6036 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/get_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/grant_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/group_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/instance_config_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5695 2023-01-17 21:03:25.000000 domolibrary-0.0.9/DomoClasses/routes/job_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1386 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/page_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/pdp_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/publish_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/role_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/sandbox_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/stream_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.0.9/DomoClasses/routes/user_routes.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.788988 domolibrary-0.0.9/GitHub/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.9/GitHub/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.0.9/GitHub/get_github_file.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.0.9/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.0.9/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11131 2023-01-30 17:31:54.796988 domolibrary-0.0.9/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10355 2023-01-30 17:30:00.000000 domolibrary-0.0.9/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.788988 domolibrary-0.0.9/domolibrary/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    77437 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/_modidx.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.792988 domolibrary-0.0.9/domolibrary/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10073 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3015 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24047 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2108 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9363 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/classes/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.792988 domolibrary-0.0.9/domolibrary/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11517 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/client/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/client/Logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4830 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/client/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11038 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/client/get_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.792988 domolibrary-0.0.9/domolibrary/integrations/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17028 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/integrations/DomoJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/integrations/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.792988 domolibrary-0.0.9/domolibrary/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5153 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/routes/account.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2030 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/routes/activity_log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2116 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/routes/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15781 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/routes/dataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5783 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/routes/user.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.792988 domolibrary-0.0.9/domolibrary/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1077 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      919 2023-01-30 17:29:32.000000 domolibrary-0.0.9/domolibrary/utils/convert.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.788988 domolibrary-0.0.9/domolibrary.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11131 2023-01-30 17:31:54.000000 domolibrary-0.0.9/domolibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3079 2023-01-30 17:31:54.000000 domolibrary-0.0.9/domolibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-01-30 17:31:54.000000 domolibrary-0.0.9/domolibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-01-30 17:31:54.000000 domolibrary-0.0.9/domolibrary.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-01-11 00:36:49.000000 domolibrary-0.0.9/domolibrary.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-01-30 17:31:54.000000 domolibrary-0.0.9/domolibrary.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-01-30 17:31:54.000000 domolibrary-0.0.9/domolibrary.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1028 2023-01-30 17:31:52.000000 domolibrary-0.0.9/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-01-30 17:31:54.796988 domolibrary-0.0.9/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.0.9/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-01-30 17:31:54.796988 domolibrary-0.0.9/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/Base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.0.9/utils/Exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.0.9/utils/LoggerClass.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/consol_get_creds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3659 2023-01-05 15:38:44.000000 domolibrary-0.0.9/utils/upload_data.py
```

### Comparing `domolibrary-0.0.8/Automation/automation.py` & `domolibrary-0.0.9/Automation/automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DataOcean/Transport.py` & `domolibrary-0.0.9/DataOcean/Transport.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DataOcean/cnfg_athena_highbandwidth.py` & `domolibrary-0.0.9/DataOcean/cnfg_athena_highbandwidth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DataOcean/cnfg_pgsql.py` & `domolibrary-0.0.9/DataOcean/cnfg_pgsql.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DataOcean/cnfg_s3.py` & `domolibrary-0.0.9/DataOcean/cnfg_s3.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DataOcean/cnfg_snowflake.py` & `domolibrary-0.0.9/DataOcean/cnfg_snowflake.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoAccount.py` & `domolibrary-0.0.9/DomoClasses/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoActivityLog.py` & `domolibrary-0.0.9/DomoClasses/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoAppDb.py` & `domolibrary-0.0.9/DomoClasses/DomoAppDb.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoApplication.py` & `domolibrary-0.0.9/DomoClasses/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoAuth.py` & `domolibrary-0.0.9/DomoClasses/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoBootstrap.py` & `domolibrary-0.0.9/DomoClasses/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoCard.py` & `domolibrary-0.0.9/DomoClasses/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoCertification.py` & `domolibrary-0.0.9/DomoClasses/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoDatacenter.py` & `domolibrary-0.0.9/DomoClasses/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoDataflow.py` & `domolibrary-0.0.9/DomoClasses/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoDataset.py` & `domolibrary-0.0.9/DomoClasses/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoGrant.py` & `domolibrary-0.0.9/DomoClasses/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoGroup.py` & `domolibrary-0.0.9/DomoClasses/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoInstanceConfig.py` & `domolibrary-0.0.9/DomoClasses/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoJob.py` & `domolibrary-0.0.9/DomoClasses/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoLineage.py` & `domolibrary-0.0.9/DomoClasses/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoPDP.py` & `domolibrary-0.0.9/DomoClasses/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoPage.py` & `domolibrary-0.0.9/DomoClasses/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoPublish.py` & `domolibrary-0.0.9/DomoClasses/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoRole.py` & `domolibrary-0.0.9/DomoClasses/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoSandbox.py` & `domolibrary-0.0.9/DomoClasses/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoStream.py` & `domolibrary-0.0.9/DomoClasses/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoTag.py` & `domolibrary-0.0.9/DomoClasses/DomoTag.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/DomoUser.py` & `domolibrary-0.0.9/DomoClasses/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/account_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/account_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/activity_log_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/activity_log_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/appdb_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/appdb_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/application_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/application_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/auth_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/auth_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/bootstrap_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/bootstrap_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/card_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/card_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/datacenter_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/datacenter_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/dataflow_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/dataflow_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/dataset_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/dataset_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/get_data.py` & `domolibrary-0.0.9/DomoClasses/routes/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/grant_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/grant_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/group_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/group_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/instance_config_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/instance_config_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/job_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/job_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/page_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/page_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/pdp_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/pdp_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/publish_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/publish_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/role_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/role_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/sandbox_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/sandbox_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/stream_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/stream_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/DomoClasses/routes/user_routes.py` & `domolibrary-0.0.9/DomoClasses/routes/user_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/LICENSE` & `domolibrary-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/PKG-INFO` & `domolibrary-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
@@ -49,21 +49,26 @@
 pip install domo_library
 ```
 
 ## How to use
 
 ### Authentication
 
-For each task, consider the appropriate `DomoAuth` mechanism. In most
-cases `DomoFullAuth` or `DomoTokenAuth` will be appropriate as this
-library predominately accesses private APIs.
+For each task, consider the appropriate
+[`DomoAuth`](https://jaewilson07.github.io/domo_library/client/domoauth.html#domoauth)
+mechanism. In most cases
+[`DomoFullAuth`](https://jaewilson07.github.io/domo_library/client/domoauth.html#domofullauth)
+or
+[`DomoTokenAuth`](https://jaewilson07.github.io/domo_library/client/domoauth.html#domotokenauth)
+will be appropriate as this library predominately accesses private APIs.
 
 Any Public routes or methods will be labeled appropriately in which case
-you should use `DomoDeveloperAuth`. Public routes are APIs enumerated
-and documented under
+you should use
+[`DomoDeveloperAuth`](https://jaewilson07.github.io/domo_library/client/domoauth.html#domodeveloperauth).
+Public routes are APIs enumerated and documented under
 <a href = "https://developer.domo.com/" target="_blank">Developer.Domo.com</a>.
 
 Typically each project will begin with configuring an auth object. If
 you are accessing multiple Domo instances, you’ll probably need multiple
 auth objects.
 
 ``` python
@@ -72,59 +77,62 @@
 import domolibrary.client.DomoAuth as dmda
 
 token_auth = dmda.DomoTokenAuth( domo_instance = 'domo-dojoo', domo_access_token = os.environ['DOMO_DOJO_ACCESS_TOKEN'])
 ```
 
 ### Option 1: class based programming
 
-In this project domo entities, `DomoActivityLog`, `DomoDataset` are all
-prefixed ‘Domo’ and can be found in the `classes` folder. Each class
-method will call one or more `routes`. Each route will interact with one
-and only one API.
+In this project domo entities,
+[`DomoActivityLog`](https://jaewilson07.github.io/domo_library/classes/domoactivitylog.html#domoactivitylog),
+[`DomoDataset`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset)
+are all prefixed ‘Domo’ and can be found in the `classes` folder. Each
+class method will call one or more `routes`. Each route will interact
+with one and only one API.
 
 Although most methods will be standard methods that will be called after
 creating an instance of the class, some methods will be classmethods
 which return an instance of the class.
 
-In the example below, `DomoDataset.get_from_id` is a classmethod.
+In the example below,
+[`DomoDataset.get_from_id`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset.get_from_id)
+is a classmethod.
 
 Note: DomoLibrary uses the asynchronous `aiohttp` requests library to
 offer users the ability to write concurrently executing code.
 
 ``` python
 import domolibrary.classes.DomoDataset as dmds
 
 # this is a class method
 domo_ds = await dmds.DomoDataset.get_from_id(auth = token_auth, dataset_id = os.environ['DOJO_DATASET_ID'])
 domo_ds
 ```
 
-    _from_httpx_response <Response [200 OK]>
-    ResponseGetData(status=200, response={'id': '04c1574e-c8be-4721-9846-c6ffa491144b', 'displayType': 'domo-jupyterdata', 'dataProviderType': 'domo-jupyterdata', 'type': 'Jupyter', 'name': 'domo_kbs', 'owner': {'id': '1893952720', 'name': 'Jae Wilson', 'type': 'USER', 'group': False}, 'status': 'SUCCESS', 'created': 1668379680000, 'lastTouched': 1668385822000, 'lastUpdated': 1668385822045, 'rowCount': 1185, 'columnCount': 7, 'cardInfo': {'cardCount': 0, 'cardViewCount': 0}, 'properties': {'formulas': {'formulas': {}}}, 'state': 'SUCCESS', 'validConfiguration': True, 'validAccount': True, 'streamId': 825, 'transportType': 'API', 'adc': False, 'adcExternal': False, 'cloudId': 'domo', 'cloudName': 'Domo', 'permissions': 'READ_WRITE_DELETE_SHARE_ADMIN', 'hidden': False, 'tags': '["developer_documentation","hackercore"]', 'scheduleActive': True, 'cryoStatus': 'ADRENALINE'}, is_success=True)
-
     DomoDataset(id='04c1574e-c8be-4721-9846-c6ffa491144b', display_type='domo-jupyterdata', data_provider_type='domo-jupyterdata', name='domo_kbs', description=None, row_count=1185, column_count=7, stream_id=825, owner=DictDot(id='1893952720', name='Jae Wilson', type='USER', group=False), formula=DictDot(), schema=DomoDataset_Schema(dataset=..., columns=[]))
 
 Once instantiated, you can call methods to interact with that object.
 You typically won’t have to pass auth creds again because they are saved
 to the object.
 
-In the example below we are retrieving the `DomoDataset_Schema` which
-consists of subclass `DomoDataset_Schema_Column` using the
-`DomoDataset_Schema.get` method.
+In the example below we are retrieving the
+[`DomoDataset_Schema`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset_schema)
+which consists of subclass
+[`DomoDataset_Schema_Column`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset_schema_column)
+using the
+[`DomoDataset_Schema.get`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset_schema.get)
+method.
 
 We take the approach of where possible converting dictionaries from Domo
 APIs into classes because it provides greater predictability when users
 are creating integrations between platforms (ex. Domo to Trello).
 
 ``` python
 await domo_ds.schema.get()
 ```
 
-    _from_httpx_response <Response [200 OK]>
-
     [DomoDataset_Schema_Column(name='objectID', id='objectID', type='STRING'),
      DomoDataset_Schema_Column(name='url', id='url', type='STRING'),
      DomoDataset_Schema_Column(name='Title', id='Title', type='STRING'),
      DomoDataset_Schema_Column(name='article', id='article', type='STRING'),
      DomoDataset_Schema_Column(name='views', id='views', type='LONG'),
      DomoDataset_Schema_Column(name='created_dt', id='created_dt', type='DATETIME'),
      DomoDataset_Schema_Column(name='published_dt', id='published_dt', type='DATETIME')]
@@ -153,33 +161,35 @@
 
 ### Option 2 functional programming
 
 Although classes add a pretty wrapper for interacting with Domo APIs,
 users can opt to interact directly with APIs by way of `routes`.
 
 All route functions will exclusively call one API and will always return
-a `ResponseGetData` object OR raise an `Exception` if appropriate.
+a
+[`ResponseGetData`](https://jaewilson07.github.io/domo_library/client/responsegetdata.html#responsegetdata)
+object OR raise an `Exception` if appropriate.
 
 For example we can implement similar functionality as the Option 1
-example by calling the `get_dataset_by_id` function.
+example by calling the
+[`get_dataset_by_id`](https://jaewilson07.github.io/domo_library/routes/dataset.html#get_dataset_by_id)
+function.
 
 ``` python
 import domolibrary.routes.dataset as dataset_routes
 
 ds_res = await dataset_routes.get_dataset_by_id( auth = token_auth, dataset_id = os.environ['DOJO_DATASET_ID'])
 ds_res
 ```
 
-    _from_httpx_response <Response [200 OK]>
     ResponseGetData(status=200, response={'id': '04c1574e-c8be-4721-9846-c6ffa491144b', 'displayType': 'domo-jupyterdata', 'dataProviderType': 'domo-jupyterdata', 'type': 'Jupyter', 'name': 'domo_kbs', 'owner': {'id': '1893952720', 'name': 'Jae Wilson', 'type': 'USER', 'group': False}, 'status': 'SUCCESS', 'created': 1668379680000, 'lastTouched': 1668385822000, 'lastUpdated': 1668385822045, 'rowCount': 1185, 'columnCount': 7, 'cardInfo': {'cardCount': 0, 'cardViewCount': 0}, 'properties': {'formulas': {'formulas': {}}}, 'state': 'SUCCESS', 'validConfiguration': True, 'validAccount': True, 'streamId': 825, 'transportType': 'API', 'adc': False, 'adcExternal': False, 'cloudId': 'domo', 'cloudName': 'Domo', 'permissions': 'READ_WRITE_DELETE_SHARE_ADMIN', 'hidden': False, 'tags': '["developer_documentation","hackercore"]', 'scheduleActive': True, 'cryoStatus': 'ADRENALINE'}, is_success=True)
 
-    ResponseGetData(status=200, response={'id': '04c1574e-c8be-4721-9846-c6ffa491144b', 'displayType': 'domo-jupyterdata', 'dataProviderType': 'domo-jupyterdata', 'type': 'Jupyter', 'name': 'domo_kbs', 'owner': {'id': '1893952720', 'name': 'Jae Wilson', 'type': 'USER', 'group': False}, 'status': 'SUCCESS', 'created': 1668379680000, 'lastTouched': 1668385822000, 'lastUpdated': 1668385822045, 'rowCount': 1185, 'columnCount': 7, 'cardInfo': {'cardCount': 0, 'cardViewCount': 0}, 'properties': {'formulas': {'formulas': {}}}, 'state': 'SUCCESS', 'validConfiguration': True, 'validAccount': True, 'streamId': 825, 'transportType': 'API', 'adc': False, 'adcExternal': False, 'cloudId': 'domo', 'cloudName': 'Domo', 'permissions': 'READ_WRITE_DELETE_SHARE_ADMIN', 'hidden': False, 'tags': '["developer_documentation","hackercore"]', 'scheduleActive': True, 'cryoStatus': 'ADRENALINE'}, is_success=True)
-
-`ResponseGetData` will always include a boolean `is_success`, the API
-`status`, and raw API `response`.
+[`ResponseGetData`](https://jaewilson07.github.io/domo_library/client/responsegetdata.html#responsegetdata)
+will always include a boolean `is_success`, the API `status`, and raw
+API `response`.
 
 Typically the route methods will not alter the response unless the API
 does not include a descriptive response (ex,
 `routes.dataset.set_dataset_tags` does not return a response so we
 artificially alter the response in the function.)
 
 ``` python
@@ -229,13 +239,16 @@
      'cryoStatus': 'ADRENALINE'}
 
 ### Access Paginated APIs using the Looper
 
 A hidden advantage of using the DomoLibrary is that paginated API
 requests are baked into the route’s definition.
 
-Consider `query_dataset_private` from the `routes.dataset`.
-
-Inside this function we are using `looper` from `client.get_data` to
-paginate over the API response.
+Consider
+[`query_dataset_private`](https://jaewilson07.github.io/domo_library/routes/dataset.html#query_dataset_private)
+from the `routes.dataset`.
+
+Inside this function we are using
+[`looper`](https://jaewilson07.github.io/domo_library/client/get_data.html#looper)
+from `client.get_data` to paginate over the API response.
```

### Comparing `domolibrary-0.0.8/README.md` & `domolibrary-0.0.9/domolibrary.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: domolibrary
+Version: 0.0.9
+Summary: UNKNOWN
+Home-page: https://github.com/jaewilson07/domo_library
+Author: Jae Wilson
+Author-email: jaewilson07@gmail.com
+License: Apache Software License 2.0
+Keywords: nbdev jupyter notebook python
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 domolibrary: a powerful pydomo alternative
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## What is it?
 
@@ -26,21 +49,26 @@
 pip install domo_library
 ```
 
 ## How to use
 
 ### Authentication
 
-For each task, consider the appropriate `DomoAuth` mechanism. In most
-cases `DomoFullAuth` or `DomoTokenAuth` will be appropriate as this
-library predominately accesses private APIs.
+For each task, consider the appropriate
+[`DomoAuth`](https://jaewilson07.github.io/domo_library/client/domoauth.html#domoauth)
+mechanism. In most cases
+[`DomoFullAuth`](https://jaewilson07.github.io/domo_library/client/domoauth.html#domofullauth)
+or
+[`DomoTokenAuth`](https://jaewilson07.github.io/domo_library/client/domoauth.html#domotokenauth)
+will be appropriate as this library predominately accesses private APIs.
 
 Any Public routes or methods will be labeled appropriately in which case
-you should use `DomoDeveloperAuth`. Public routes are APIs enumerated
-and documented under
+you should use
+[`DomoDeveloperAuth`](https://jaewilson07.github.io/domo_library/client/domoauth.html#domodeveloperauth).
+Public routes are APIs enumerated and documented under
 <a href = "https://developer.domo.com/" target="_blank">Developer.Domo.com</a>.
 
 Typically each project will begin with configuring an auth object. If
 you are accessing multiple Domo instances, you’ll probably need multiple
 auth objects.
 
 ``` python
@@ -49,59 +77,62 @@
 import domolibrary.client.DomoAuth as dmda
 
 token_auth = dmda.DomoTokenAuth( domo_instance = 'domo-dojoo', domo_access_token = os.environ['DOMO_DOJO_ACCESS_TOKEN'])
 ```
 
 ### Option 1: class based programming
 
-In this project domo entities, `DomoActivityLog`, `DomoDataset` are all
-prefixed ‘Domo’ and can be found in the `classes` folder. Each class
-method will call one or more `routes`. Each route will interact with one
-and only one API.
+In this project domo entities,
+[`DomoActivityLog`](https://jaewilson07.github.io/domo_library/classes/domoactivitylog.html#domoactivitylog),
+[`DomoDataset`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset)
+are all prefixed ‘Domo’ and can be found in the `classes` folder. Each
+class method will call one or more `routes`. Each route will interact
+with one and only one API.
 
 Although most methods will be standard methods that will be called after
 creating an instance of the class, some methods will be classmethods
 which return an instance of the class.
 
-In the example below, `DomoDataset.get_from_id` is a classmethod.
+In the example below,
+[`DomoDataset.get_from_id`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset.get_from_id)
+is a classmethod.
 
 Note: DomoLibrary uses the asynchronous `aiohttp` requests library to
 offer users the ability to write concurrently executing code.
 
 ``` python
 import domolibrary.classes.DomoDataset as dmds
 
 # this is a class method
 domo_ds = await dmds.DomoDataset.get_from_id(auth = token_auth, dataset_id = os.environ['DOJO_DATASET_ID'])
 domo_ds
 ```
 
-    _from_httpx_response <Response [200 OK]>
-    ResponseGetData(status=200, response={'id': '04c1574e-c8be-4721-9846-c6ffa491144b', 'displayType': 'domo-jupyterdata', 'dataProviderType': 'domo-jupyterdata', 'type': 'Jupyter', 'name': 'domo_kbs', 'owner': {'id': '1893952720', 'name': 'Jae Wilson', 'type': 'USER', 'group': False}, 'status': 'SUCCESS', 'created': 1668379680000, 'lastTouched': 1668385822000, 'lastUpdated': 1668385822045, 'rowCount': 1185, 'columnCount': 7, 'cardInfo': {'cardCount': 0, 'cardViewCount': 0}, 'properties': {'formulas': {'formulas': {}}}, 'state': 'SUCCESS', 'validConfiguration': True, 'validAccount': True, 'streamId': 825, 'transportType': 'API', 'adc': False, 'adcExternal': False, 'cloudId': 'domo', 'cloudName': 'Domo', 'permissions': 'READ_WRITE_DELETE_SHARE_ADMIN', 'hidden': False, 'tags': '["developer_documentation","hackercore"]', 'scheduleActive': True, 'cryoStatus': 'ADRENALINE'}, is_success=True)
-
     DomoDataset(id='04c1574e-c8be-4721-9846-c6ffa491144b', display_type='domo-jupyterdata', data_provider_type='domo-jupyterdata', name='domo_kbs', description=None, row_count=1185, column_count=7, stream_id=825, owner=DictDot(id='1893952720', name='Jae Wilson', type='USER', group=False), formula=DictDot(), schema=DomoDataset_Schema(dataset=..., columns=[]))
 
 Once instantiated, you can call methods to interact with that object.
 You typically won’t have to pass auth creds again because they are saved
 to the object.
 
-In the example below we are retrieving the `DomoDataset_Schema` which
-consists of subclass `DomoDataset_Schema_Column` using the
-`DomoDataset_Schema.get` method.
+In the example below we are retrieving the
+[`DomoDataset_Schema`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset_schema)
+which consists of subclass
+[`DomoDataset_Schema_Column`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset_schema_column)
+using the
+[`DomoDataset_Schema.get`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset_schema.get)
+method.
 
 We take the approach of where possible converting dictionaries from Domo
 APIs into classes because it provides greater predictability when users
 are creating integrations between platforms (ex. Domo to Trello).
 
 ``` python
 await domo_ds.schema.get()
 ```
 
-    _from_httpx_response <Response [200 OK]>
-
     [DomoDataset_Schema_Column(name='objectID', id='objectID', type='STRING'),
      DomoDataset_Schema_Column(name='url', id='url', type='STRING'),
      DomoDataset_Schema_Column(name='Title', id='Title', type='STRING'),
      DomoDataset_Schema_Column(name='article', id='article', type='STRING'),
      DomoDataset_Schema_Column(name='views', id='views', type='LONG'),
      DomoDataset_Schema_Column(name='created_dt', id='created_dt', type='DATETIME'),
      DomoDataset_Schema_Column(name='published_dt', id='published_dt', type='DATETIME')]
@@ -130,33 +161,35 @@
 
 ### Option 2 functional programming
 
 Although classes add a pretty wrapper for interacting with Domo APIs,
 users can opt to interact directly with APIs by way of `routes`.
 
 All route functions will exclusively call one API and will always return
-a `ResponseGetData` object OR raise an `Exception` if appropriate.
+a
+[`ResponseGetData`](https://jaewilson07.github.io/domo_library/client/responsegetdata.html#responsegetdata)
+object OR raise an `Exception` if appropriate.
 
 For example we can implement similar functionality as the Option 1
-example by calling the `get_dataset_by_id` function.
+example by calling the
+[`get_dataset_by_id`](https://jaewilson07.github.io/domo_library/routes/dataset.html#get_dataset_by_id)
+function.
 
 ``` python
 import domolibrary.routes.dataset as dataset_routes
 
 ds_res = await dataset_routes.get_dataset_by_id( auth = token_auth, dataset_id = os.environ['DOJO_DATASET_ID'])
 ds_res
 ```
 
-    _from_httpx_response <Response [200 OK]>
     ResponseGetData(status=200, response={'id': '04c1574e-c8be-4721-9846-c6ffa491144b', 'displayType': 'domo-jupyterdata', 'dataProviderType': 'domo-jupyterdata', 'type': 'Jupyter', 'name': 'domo_kbs', 'owner': {'id': '1893952720', 'name': 'Jae Wilson', 'type': 'USER', 'group': False}, 'status': 'SUCCESS', 'created': 1668379680000, 'lastTouched': 1668385822000, 'lastUpdated': 1668385822045, 'rowCount': 1185, 'columnCount': 7, 'cardInfo': {'cardCount': 0, 'cardViewCount': 0}, 'properties': {'formulas': {'formulas': {}}}, 'state': 'SUCCESS', 'validConfiguration': True, 'validAccount': True, 'streamId': 825, 'transportType': 'API', 'adc': False, 'adcExternal': False, 'cloudId': 'domo', 'cloudName': 'Domo', 'permissions': 'READ_WRITE_DELETE_SHARE_ADMIN', 'hidden': False, 'tags': '["developer_documentation","hackercore"]', 'scheduleActive': True, 'cryoStatus': 'ADRENALINE'}, is_success=True)
 
-    ResponseGetData(status=200, response={'id': '04c1574e-c8be-4721-9846-c6ffa491144b', 'displayType': 'domo-jupyterdata', 'dataProviderType': 'domo-jupyterdata', 'type': 'Jupyter', 'name': 'domo_kbs', 'owner': {'id': '1893952720', 'name': 'Jae Wilson', 'type': 'USER', 'group': False}, 'status': 'SUCCESS', 'created': 1668379680000, 'lastTouched': 1668385822000, 'lastUpdated': 1668385822045, 'rowCount': 1185, 'columnCount': 7, 'cardInfo': {'cardCount': 0, 'cardViewCount': 0}, 'properties': {'formulas': {'formulas': {}}}, 'state': 'SUCCESS', 'validConfiguration': True, 'validAccount': True, 'streamId': 825, 'transportType': 'API', 'adc': False, 'adcExternal': False, 'cloudId': 'domo', 'cloudName': 'Domo', 'permissions': 'READ_WRITE_DELETE_SHARE_ADMIN', 'hidden': False, 'tags': '["developer_documentation","hackercore"]', 'scheduleActive': True, 'cryoStatus': 'ADRENALINE'}, is_success=True)
-
-`ResponseGetData` will always include a boolean `is_success`, the API
-`status`, and raw API `response`.
+[`ResponseGetData`](https://jaewilson07.github.io/domo_library/client/responsegetdata.html#responsegetdata)
+will always include a boolean `is_success`, the API `status`, and raw
+API `response`.
 
 Typically the route methods will not alter the response unless the API
 does not include a descriptive response (ex,
 `routes.dataset.set_dataset_tags` does not return a response so we
 artificially alter the response in the function.)
 
 ``` python
@@ -206,11 +239,16 @@
      'cryoStatus': 'ADRENALINE'}
 
 ### Access Paginated APIs using the Looper
 
 A hidden advantage of using the DomoLibrary is that paginated API
 requests are baked into the route’s definition.
 
-Consider `query_dataset_private` from the `routes.dataset`.
+Consider
+[`query_dataset_private`](https://jaewilson07.github.io/domo_library/routes/dataset.html#query_dataset_private)
+from the `routes.dataset`.
+
+Inside this function we are using
+[`looper`](https://jaewilson07.github.io/domo_library/client/get_data.html#looper)
+from `client.get_data` to paginate over the API response.
+
 
-Inside this function we are using `looper` from `client.get_data` to
-paginate over the API response.
```

### Comparing `domolibrary-0.0.8/domolibrary/_modidx.py` & `domolibrary-0.0.9/domolibrary/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,40 +29,32 @@
                                                                                                          'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config._from_json': ( 'classes/domoaccount.html#domoaccount_config._from_json',
                                                                                                                     'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config.to_json': ( 'classes/domoaccount.html#domoaccount_config.to_json',
                                                                                                                  'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_AbstractCredential': ( 'classes/domoaccount.html#domoaccount_config_abstractcredential',
                                                                                                                             'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount_Config_AbstractCredential.__post_init_': ( 'classes/domoaccount.html#domoaccount_config_abstractcredential.__post_init_',
-                                                                                                                                         'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_AbstractCredential._from_json': ( 'classes/domoaccount.html#domoaccount_config_abstractcredential._from_json',
                                                                                                                                        'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_AbstractCredential.to_json': ( 'classes/domoaccount.html#domoaccount_config_abstractcredential.to_json',
                                                                                                                                     'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_DatasetCopy': ( 'classes/domoaccount.html#domoaccount_config_datasetcopy',
                                                                                                                      'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount_Config_DatasetCopy.__post_init_': ( 'classes/domoaccount.html#domoaccount_config_datasetcopy.__post_init_',
-                                                                                                                                  'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_DatasetCopy._from_json': ( 'classes/domoaccount.html#domoaccount_config_datasetcopy._from_json',
                                                                                                                                 'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_DatasetCopy.to_json': ( 'classes/domoaccount.html#domoaccount_config_datasetcopy.to_json',
                                                                                                                              'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_Governance': ( 'classes/domoaccount.html#domoaccount_config_governance',
                                                                                                                     'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount_Config_Governance.__post_init_': ( 'classes/domoaccount.html#domoaccount_config_governance.__post_init_',
-                                                                                                                                 'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_Governance._from_json': ( 'classes/domoaccount.html#domoaccount_config_governance._from_json',
                                                                                                                                'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_Governance.to_json': ( 'classes/domoaccount.html#domoaccount_config_governance.to_json',
                                                                                                                             'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_HighBandwidthConnector': ( 'classes/domoaccount.html#domoaccount_config_highbandwidthconnector',
                                                                                                                                 'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.DomoAccount_Config_HighBandwidthConnector.__post_init_': ( 'classes/domoaccount.html#domoaccount_config_highbandwidthconnector.__post_init_',
-                                                                                                                                             'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_HighBandwidthConnector._from_json': ( 'classes/domoaccount.html#domoaccount_config_highbandwidthconnector._from_json',
                                                                                                                                            'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_Config_HighBandwidthConnector.to_json': ( 'classes/domoaccount.html#domoaccount_config_highbandwidthconnector.to_json',
                                                                                                                                         'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_CreateAccount_Error': ( 'classes/domoaccount.html#domoaccount_createaccount_error',
                                                                                                                       'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_CreateAccount_Error.__init__': ( 'classes/domoaccount.html#domoaccount_createaccount_error.__init__',
@@ -77,25 +69,25 @@
                                                                                                                      'domolibrary/classes/DomoActivityLog.py'),
                                                      'domolibrary.classes.DomoActivityLog.DomoActivityLog': ( 'classes/domoactivitylog.html#domoactivitylog',
                                                                                                               'domolibrary/classes/DomoActivityLog.py'),
                                                      'domolibrary.classes.DomoActivityLog.DomoActivityLog._process_activity_log_row': ( 'classes/domoactivitylog.html#domoactivitylog._process_activity_log_row',
                                                                                                                                         'domolibrary/classes/DomoActivityLog.py'),
                                                      'domolibrary.classes.DomoActivityLog.DomoActivityLog.get_activity_log': ( 'classes/domoactivitylog.html#domoactivitylog.get_activity_log',
                                                                                                                                'domolibrary/classes/DomoActivityLog.py')},
-            'domolibrary.classes.DomoBootstrap': { 'domolibrary.classes.DomoBootstrap.DomoBootstrap': ( 'classes/.domobootstrap.html#domobootstrap',
+            'domolibrary.classes.DomoBootstrap': { 'domolibrary.classes.DomoBootstrap.DomoBootstrap': ( 'classes/domobootstrap.html#domobootstrap',
                                                                                                         'domolibrary/classes/DomoBootstrap.py'),
-                                                   'domolibrary.classes.DomoBootstrap.DomoBootstrap.get_all': ( 'classes/.domobootstrap.html#domobootstrap.get_all',
+                                                   'domolibrary.classes.DomoBootstrap.DomoBootstrap.get_all': ( 'classes/domobootstrap.html#domobootstrap.get_all',
                                                                                                                 'domolibrary/classes/DomoBootstrap.py'),
-                                                   'domolibrary.classes.DomoBootstrap.DomoBootstrap.get_features': ( 'classes/.domobootstrap.html#domobootstrap.get_features',
+                                                   'domolibrary.classes.DomoBootstrap.DomoBootstrap.get_features': ( 'classes/domobootstrap.html#domobootstrap.get_features',
                                                                                                                      'domolibrary/classes/DomoBootstrap.py'),
-                                                   'domolibrary.classes.DomoBootstrap.DomoBootstrap.get_pages': ( 'classes/.domobootstrap.html#domobootstrap.get_pages',
+                                                   'domolibrary.classes.DomoBootstrap.DomoBootstrap.get_pages': ( 'classes/domobootstrap.html#domobootstrap.get_pages',
                                                                                                                   'domolibrary/classes/DomoBootstrap.py'),
-                                                   'domolibrary.classes.DomoBootstrap.DomoBootstrap_Feature': ( 'classes/.domobootstrap.html#domobootstrap_feature',
+                                                   'domolibrary.classes.DomoBootstrap.DomoBootstrap_Feature': ( 'classes/domobootstrap.html#domobootstrap_feature',
                                                                                                                 'domolibrary/classes/DomoBootstrap.py'),
-                                                   'domolibrary.classes.DomoBootstrap.DomoBootstrap_Feature._from_json_bootstrap': ( 'classes/.domobootstrap.html#domobootstrap_feature._from_json_bootstrap',
+                                                   'domolibrary.classes.DomoBootstrap.DomoBootstrap_Feature._from_json_bootstrap': ( 'classes/domobootstrap.html#domobootstrap_feature._from_json_bootstrap',
                                                                                                                                      'domolibrary/classes/DomoBootstrap.py')},
             'domolibrary.classes.DomoDataset': { 'domolibrary.classes.DomoDataset.DatasetSchema_AuthNotProvidedError': ( 'classes/domodataset.html#datasetschema_authnotprovidederror',
                                                                                                                          'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DatasetSchema_AuthNotProvidedError.__init__': ( 'classes/domodataset.html#datasetschema_authnotprovidederror.__init__',
                                                                                                                                   'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DatasetSchema_DatasetNotProvidedError': ( 'classes/domodataset.html#datasetschema_datasetnotprovidederror',
                                                                                                                             'domolibrary/classes/DomoDataset.py'),
@@ -165,26 +157,28 @@
                                                                                                                                             'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_UploadData_Error': ( 'classes/domodataset.html#domodataset_uploaddata_error',
                                                                                                                    'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_UploadData_Error.__init__': ( 'classes/domodataset.html#domodataset_uploaddata_error.__init__',
                                                                                                                             'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_UploadData_UploadData_Error': ( 'classes/domodataset.html#domodataset_uploaddata_uploaddata_error',
                                                                                                                               'domolibrary/classes/DomoDataset.py'),
-                                                 'domolibrary.classes.DomoDataset.DomoDataset_UploadData_UploadData_Error.DomoDataset_UploadData_CommitDatasetUploadId_Error': ( 'classes/domodataset.html#domodataset_uploaddata_uploaddata_error.domodataset_uploaddata_commitdatasetuploadid_error',
-                                                                                                                                                                                 'domolibrary/classes/DomoDataset.py'),
+                                                 'domolibrary.classes.DomoDataset.DomoDataset_UploadData_UploadData_Error.DomoDataset_UploadData_DatasetUploadId_Error': ( 'classes/domodataset.html#domodataset_uploaddata_uploaddata_error.domodataset_uploaddata_datasetuploadid_error',
+                                                                                                                                                                           'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.DomoDataset_UploadData_UploadData_Error.__init__': ( 'classes/domodataset.html#domodataset_uploaddata_uploaddata_error.__init__',
                                                                                                                                        'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.QueryExecutionError': ( 'classes/domodataset.html#queryexecutionerror',
                                                                                                           'domolibrary/classes/DomoDataset.py'),
                                                  'domolibrary.classes.DomoDataset.QueryExecutionError.__init__': ( 'classes/domodataset.html#queryexecutionerror.__init__',
                                                                                                                    'domolibrary/classes/DomoDataset.py')},
             'domolibrary.classes.DomoPage': { 'domolibrary.classes.DomoPage.DomoPage': ( 'classes/domopage.html#domopage',
                                                                                          'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage._from_bootstrap': ( 'classes/domopage.html#domopage._from_bootstrap',
                                                                                                          'domolibrary/classes/DomoPage.py'),
+                                              'domolibrary.classes.DomoPage.DomoPage._ol_fn': ( 'classes/domopage.html#domopage._ol_fn',
+                                                                                                'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage.display_url': ( 'classes/domopage.html#domopage.display_url',
                                                                                                      'domolibrary/classes/DomoPage.py')},
             'domolibrary.classes.DomoUser': { 'domolibrary.classes.DomoUser.DomoUser': ( 'classes/domouser.html#domouser',
                                                                                          'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUser._from_bootstrap_json': ( 'classes/domouser.html#domouser._from_bootstrap_json',
                                                                                                               'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUser._from_search_json': ( 'classes/domouser.html#domouser._from_search_json',
@@ -324,15 +318,17 @@
                                              'domolibrary.client.get_data.LooperError.__init__': ( 'client/get_data.html#loopererror.__init__',
                                                                                                    'domolibrary/client/get_data.py'),
                                              'domolibrary.client.get_data.get_data': ( 'client/get_data.html#get_data',
                                                                                        'domolibrary/client/get_data.py'),
                                              'domolibrary.client.get_data.get_data_aiohttp': ( 'client/get_data.html#get_data_aiohttp',
                                                                                                'domolibrary/client/get_data.py'),
                                              'domolibrary.client.get_data.looper': ( 'client/get_data.html#looper',
-                                                                                     'domolibrary/client/get_data.py')},
+                                                                                     'domolibrary/client/get_data.py'),
+                                             'domolibrary.client.get_data.looper_aiohttp': ( 'client/get_data.html#looper_aiohttp',
+                                                                                             'domolibrary/client/get_data.py')},
             'domolibrary.integrations.DomoJupyter': { 'domolibrary.integrations.DomoJupyter.DojoAccount_InstanceAuth': ( 'integrations/domojupyter.html#dojoaccount_instanceauth',
                                                                                                                          'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.DojoAccount_InstanceAuth.__post_init__': ( 'integrations/domojupyter.html#dojoaccount_instanceauth.__post_init__',
                                                                                                                                        'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.DojoAccount_InstanceAuth._clean_account_admin_accounts': ( 'integrations/domojupyter.html#dojoaccount_instanceauth._clean_account_admin_accounts',
                                                                                                                                                        'domolibrary/integrations/DomoJupyter.py'),
                                                       'domolibrary.integrations.DomoJupyter.DojoAccount_InstanceAuth._generate_auth': ( 'integrations/domojupyter.html#dojoaccount_instanceauth._generate_auth',
@@ -435,14 +431,16 @@
                                                                                                        'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.UploadDataError': ( 'routes/dataset.html#uploaddataerror',
                                                                                             'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.UploadDataError.__init__': ( 'routes/dataset.html#uploaddataerror.__init__',
                                                                                                      'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.create': ( 'routes/dataset.html#create',
                                                                                    'domolibrary/routes/dataset.py'),
+                                            'domolibrary.routes.dataset.delete': ( 'routes/dataset.html#delete',
+                                                                                   'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.generate_create_dataset_body': ( 'routes/dataset.html#generate_create_dataset_body',
                                                                                                          'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.generate_list_partitions_body': ( 'routes/dataset.html#generate_list_partitions_body',
                                                                                                           'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.get_dataset_by_id': ( 'routes/dataset.html#get_dataset_by_id',
                                                                                               'domolibrary/routes/dataset.py'),
                                             'domolibrary.routes.dataset.get_schema': ( 'routes/dataset.html#get_schema',
```

### Comparing `domolibrary-0.0.8/domolibrary/classes/DomoAccount.py` & `domolibrary-0.0.9/domolibrary/classes/DomoAccount.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,47 +10,47 @@
 from dataclasses import dataclass, field
 from abc import ABC, abstractclassmethod, abstractmethod
 
 import datetime as dt
 import re
 
 
-import aiohttp
+import httpx
 
 from fastcore.basics import patch_to
 
 import domolibrary.utils.convert as cd
 import domolibrary.utils.DictDot as util_dd
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.routes.account as account_routes
 
+
 # %% ../../nbs/classes/50_DomoAccount.ipynb 5
 class DomoAccount_Config(ABC):
     """DomoAccount Config abstract base class"""
-    data_provider_type : str
 
-    @abstractclassmethod
+    data_provider_type: str
+
+    @classmethod
+    @abstractmethod
     def _from_json(cls, obj):
         """convert accounts API response into a class object"""
         pass
 
     @abstractmethod
     def to_json(self):
         """convert class object into a format the accounts API expects"""
         pass
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 6
 @dataclass
 class DomoAccount_Config_AbstractCredential(DomoAccount_Config):
-    data_provider_type = 'abstract-credential-store'
+    data_provider_type = "abstract-credential-store"
     credentials: dict
 
-    def __post_init_(self):
-        super().__init__(self)
-
     @classmethod
     def _from_json(cls, obj):
 
         dd = util_dd.DictDot(obj)
 
         return cls(
             credentials=dd.credentials,
@@ -61,75 +61,53 @@
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 7
 @dataclass
 class DomoAccount_Config_DatasetCopy(DomoAccount_Config):
     domo_instance: str
     access_token: str = field(repr=False)
 
-    data_provider_type = 'dataset-copy'
-    
-
-    def __post_init_(self):
-        super().__init__(self)
+    data_provider_type = "dataset-copy"
 
     @classmethod
     def _from_json(cls, obj):
 
         dd = util_dd.DictDot(obj)
 
-        return cls(
-            access_token=dd.accessToken,
-            domo_instance=dd.instance
-        )
+        return cls(access_token=dd.accessToken, domo_instance=dd.instance)
 
     def to_json(self):
-        return {"accessToken": self.access_token,
-                "instance": self.domo_instance
-                }
-
+        return {"accessToken": self.access_token, "instance": self.domo_instance}
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 8
 @dataclass
 class DomoAccount_Config_Governance(DomoAccount_Config):
     domo_instance: str
     access_token: str = field(repr=False)
 
-    data_provider_type = 'domo-governance-d14c2fef-49a8-4898-8ddd-f64998005600'
-
-    def __post_init_(self):
-        super().__init__(self)
+    data_provider_type = "domo-governance-d14c2fef-49a8-4898-8ddd-f64998005600"
 
     @classmethod
     def _from_json(cls, obj):
 
         dd = util_dd.DictDot(obj)
 
-        return cls(
-            access_token=dd.apikey,
-            domo_instance=dd.customer
-        )
+        return cls(access_token=dd.apikey, domo_instance=dd.customer)
 
     def to_json(self):
-        return {"apikey": self.access_token,
-                "customer": self.domo_instance
-                }
-
+        return {"apikey": self.access_token, "customer": self.domo_instance}
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 9
 @dataclass
 class DomoAccount_Config_HighBandwidthConnector(DomoAccount_Config):
     aws_access_key: str
     aws_secret_key: str = field(repr=False)
     s3_staging_dir: str
     region: str = "us-west-2"
-    
-    data_provider_type = "amazon-athena-high-bandwidth"
 
-    def __post_init_(self):
-        super().__init__(self)
+    data_provider_type = "amazon-athena-high-bandwidth"
 
     @classmethod
     def _from_json(cls, obj):
 
         dd = util_dd.DictDot(obj)
 
         return cls(
@@ -146,27 +124,26 @@
             "s3StagingDir": self.s3_staging_dir,
             "region": self.region,
         }
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 10
 class AccountConfig(Enum):
     """
-    Enum provides appropriate spelling for data_provider_type and config object.  
+    Enum provides appropriate spelling for data_provider_type and config object.
     The name of the enum should correspond with the data_provider_type with hyphens replaced with underscores.
     """
 
     amazon_athena_high_bandwidth = DomoAccount_Config_HighBandwidthConnector
 
     abstract_credential_store = DomoAccount_Config_AbstractCredential
 
     dataset_copy = DomoAccount_Config_DatasetCopy
 
     domo_governance_d14c2fef_49a8_4898_8ddd_f64998005600 = DomoAccount_Config_Governance
 
-
 # %% ../../nbs/classes/50_DomoAccount.ipynb 12
 @dataclass
 class DomoAccount:
     name: str
     data_provider_type: str
 
     id: int = None
@@ -186,181 +163,201 @@
             id=dd.id,
             name=dd.displayName,
             data_provider_type=dd.dataProviderType,
             created_dt=cd.convert_epoch_millisecond_to_datetime(dd.createdAt),
             modified_dt=cd.convert_epoch_millisecond_to_datetime(dd.modifiedAt),
             auth=auth,
         )
-    
-    async def _get_config(self, session = None, debug_api : bool = None, return_raw: bool = False):
-    
+
+    async def _get_config(
+        self, session=None, debug_api: bool = None, return_raw: bool = False
+    ):
+
         res_config = await account_routes.get_account_config(
             auth=self.auth,
             account_id=self.id,
             data_provider_type=self.data_provider_type,
             session=session,
-            debug_api=debug_api
+            debug_api=debug_api,
         )
 
         if return_raw:
             return res_config
 
         enum_clean = re.sub("-", "_", self.data_provider_type)
 
         if not enum_clean in AccountConfig.__members__:
             return None
 
-        self.config = (
-            AccountConfig[enum_clean].value._from_json(res_config.response)
-        )
+        self.config = AccountConfig[enum_clean].value._from_json(res_config.response)
 
         return self.config
 
-
 # %% ../../nbs/classes/50_DomoAccount.ipynb 13
 @patch_to(DomoAccount, cls_method=True)
 async def get_from_id(
     cls,
     auth: dmda.DomoAuth,
     account_id: int,
-    session: aiohttp.ClientSession = None,
+    session: httpx.AsyncClient = None,
     return_raw: bool = False,
-    debug_api: bool = False
+    debug_api: bool = False,
 ):
 
     res = await account_routes.get_account_from_id(
-        auth=auth, account_id=account_id, session=session, debug_api = debug_api
+        auth=auth, account_id=account_id, session=session, debug_api=debug_api
     )
     if return_raw:
         return res
 
     if not res.is_success:
         return None
 
     obj = res.response
     acc = cls._from_json(obj, auth)
 
-    await acc._get_config(session = session, debug_api = debug_api)
+    await acc._get_config(session=session, debug_api=debug_api)
 
     return acc
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 17
 @patch_to(DomoAccount)
-async def update_config(self: DomoAccount,
-                        auth: dmda.DomoAuth = None,
-                        debug_api: bool = False,
-                        config : DomoAccount_Config = None,
-                        session: aiohttp.ClientSession = None, return_raw: bool = False):
+async def update_config(
+    self: DomoAccount,
+    auth: dmda.DomoAuth = None,
+    debug_api: bool = False,
+    config: DomoAccount_Config = None,
+    session: httpx.AsyncClient = None,
+    return_raw: bool = False,
+):
 
     auth = auth or self.auth
 
     config = config or self.config
 
-    res = await account_routes.update_account_config(auth=auth,
-                                                     account_id=self.id,
-                                                     data_provider_type=self.data_provider_type,
-                                                     config_body=config.to_json(),
-                                                     debug_api=debug_api, session=session)
+    res = await account_routes.update_account_config(
+        auth=auth,
+        account_id=self.id,
+        data_provider_type=self.data_provider_type,
+        config_body=config.to_json(),
+        debug_api=debug_api,
+        session=session,
+    )
 
     if return_raw:
         return res
 
     await self._get_config(session=session, debug_api=debug_api)
 
     return self
 
-
 # %% ../../nbs/classes/50_DomoAccount.ipynb 20
 class DomoAccount_UpdateName_Error(Exception):
     pass
 
+
 @patch_to(DomoAccount)
-async def update_name(self: DomoAccount,
-                      account_name: str = None,
-                      auth: dmda.DomoAuth = None,
-                      debug_api: bool = False,
-                      session: aiohttp.ClientSession = None,
-                      return_raw: bool = False):
+async def update_name(
+    self: DomoAccount,
+    account_name: str = None,
+    auth: dmda.DomoAuth = None,
+    debug_api: bool = False,
+    session: httpx.AsyncClient = None,
+    return_raw: bool = False,
+):
 
     auth = auth or self.auth
 
     # print(auth, self.id, self.data_provider_type, self.config.to_json())
 
-    res = await account_routes.update_account_name(auth=auth,
-                                                   account_id=self.id,
-                                                   account_name=account_name or self.name,
-                                                   debug_api=debug_api,
-                                                   session=session)
+    res = await account_routes.update_account_name(
+        auth=auth,
+        account_id=self.id,
+        account_name=account_name or self.name,
+        debug_api=debug_api,
+        session=session,
+    )
 
     if return_raw:
         return res
 
     if not res.is_success:
         raise DomoAccount_UpdateName_Error()
-    
+
     self = await self.get_from_id(auth=auth, account_id=self.id)
-    
-    return self
 
+    return self
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 24
 class DomoAccount_CreateAccount_Error(Exception):
     def __init__(self, account_name, domo_instance, status, reason):
         message = f"CreateAccount Error :: {account_name} in {domo_instance} :: {status} - {reason}"
-        super.__init__(message)
+        super().__init__(message)
 
 
 @patch_to(DomoAccount, cls_method=True)
 def generate_create_body(cls, account_name, config):
-    return {'displayName': account_name,
-            'dataProviderType': config.data_provider_type,
-            'name': config.data_provider_type,
-            'configurations': config.to_json()}
+    return {
+        "displayName": account_name,
+        "dataProviderType": config.data_provider_type,
+        "name": config.data_provider_type,
+        "configurations": config.to_json(),
+    }
 
 
 @patch_to(DomoAccount, cls_method=True)
-async def create_account(cls: DomoAccount,
-                         account_name: str, 
-                         config: DomoAccount_Config,
-                         auth: dmda.DomoAuth,
-                         debug_api: bool = False,
-                         session: aiohttp.ClientSession = None):
+async def create_account(
+    cls: DomoAccount,
+    account_name: str,
+    config: DomoAccount_Config,
+    auth: dmda.DomoAuth,
+    debug_api: bool = False,
+    session: httpx.AsyncClient = None,
+):
 
     body = cls.generate_create_body(account_name=account_name, config=config)
 
-    res = await account_routes.create_account(auth=auth,
-                                              config_body=body,
-                                              debug_api=debug_api, session=session)
+    res = await account_routes.create_account(
+        auth=auth, config_body=body, debug_api=debug_api, session=session
+    )
 
     if not res.is_success:
-        raise DomoAccount_CreateAccount_Error(account_name=account_name,
-                                              domo_instance=auth.domo_instance,
-                                              status=res.status, reason=res.response)
-
-    return await cls.get_from_id(auth=auth, account_id=res.response.get('id'))
+        raise DomoAccount_CreateAccount_Error(
+            account_name=account_name,
+            domo_instance=auth.domo_instance,
+            status=res.status,
+            reason=res.response,
+        )
 
+    return await cls.get_from_id(auth=auth, account_id=res.response.get("id"))
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 25
 class DomoAccount_DeleteAccount_Error(Exception):
-    def __init__(self, account_id, domo_instance, status, reason) -> bool:
+    def __init__(self, account_id, domo_instance, status, reason):
+
         message = f"DeleteAccount Error :: {account_id} in {domo_instance} :: {status} - {reason}"
-        super.__init__(message)
+        super().__init__(message)
 
 
 @patch_to(DomoAccount)
-async def delete_account(self: DomoAccount,
-                         auth: dmda.DomoAuth = None,
-                         debug_api: bool = False, session: aiohttp.ClientSession = None):
+async def delete_account(
+    self: DomoAccount,
+    auth: dmda.DomoAuth = None,
+    debug_api: bool = False,
+    session: httpx.AsyncClient = None,
+):
 
     auth = auth or self.auth
 
-    res = await account_routes.delete_account(auth=auth,
-                                              account_id=self.id,
-                                              debug_api=debug_api,
-                                              session=session)
+    res = await account_routes.delete_account(
+        auth=auth, account_id=self.id, debug_api=debug_api, session=session
+    )
 
     if not res.is_success:
         raise DomoAccount_DeleteAccount_Error(
-            account_id = self.id, domo_instance = auth.domo_instance, status = res.status, reason = res.response)
+            account_id=self.id,
+            domo_instance=auth.domo_instance,
+            status=res.status,
+            reason=res.response,
+        )
 
     return True
-
```

### Comparing `domolibrary-0.0.8/domolibrary/classes/DomoActivityLog.py` & `domolibrary-0.0.9/domolibrary/classes/DomoActivityLog.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # %% ../../nbs/classes/50_DomoActivityLog.ipynb 3
 from enum import Enum
 from typing import Optional
 
 import datetime as dt
 from pprint import pprint
 
-import aiohttp
+import httpx
 
 import domolibrary.utils.convert as convert
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.routes.activity_log as activity_log_routes
 
 # %% ../../nbs/classes/50_DomoActivityLog.ipynb 4
 class ActivityLog_ObjectType(Enum):
@@ -99,15 +99,15 @@
     async def get_activity_log(
         cls,
         auth: dmda.DomoAuth,
         start_time: dt.datetime,
         end_time: dt.datetime,
         object_type: Optional[ActivityLog_ObjectType] = None,
         maximum: int = 1000,
-        session: Optional[aiohttp.ClientSession] = None,
+        session: Optional[httpx.AsyncClient] = None,
         debug_api: bool = False,
         debug_loop: bool = False,
     ):
         """queries the activity log"""
 
         start_time_epoch = convert.convert_datetime_to_epoch_millisecond(
             start_time)
```

### Comparing `domolibrary-0.0.8/domolibrary/classes/DomoBootstrap.py` & `domolibrary-0.0.9/domolibrary/classes/DomoBootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/classes/50_.DomoBootstrap.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/classes/50_DomoBootstrap.ipynb.
 
 # %% auto 0
 __all__ = ['DomoBootstrap_Feature', 'DomoBootstrap']
 
-# %% ../../nbs/classes/50_.DomoBootstrap.ipynb 2
-from fastcore.basics import patch, patch_to
-
-
-
-# %% ../../nbs/classes/50_.DomoBootstrap.ipynb 3
+# %% ../../nbs/classes/50_DomoBootstrap.ipynb 2
 from dataclasses import dataclass, field
 
 import httpx
 
-import domolibrary.classes.DomoDataset as dmds
 import domolibrary.classes.DomoPage as dmpg
 
 import domolibrary.utils.DictDot as util_dd
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.client.Logger as lc
 import domolibrary.routes.bootstrap as bootstrap_routes
 
 
-# %% ../../nbs/classes/50_.DomoBootstrap.ipynb 4
+# %% ../../nbs/classes/50_DomoBootstrap.ipynb 3
+from fastcore.basics import patch_to
+
+
+
+# %% ../../nbs/classes/50_DomoBootstrap.ipynb 4
 @dataclass
 class DomoBootstrap_Feature:
     id: int
     name: str
     label: str
     type: str
     purchased: bool
@@ -42,35 +41,35 @@
             label=dd.label,
             type=dd.type,
             purchased=dd.purchased,
             enabled=dd.enabled
         )
         return bsf
 
-# %% ../../nbs/classes/50_.DomoBootstrap.ipynb 5
+# %% ../../nbs/classes/50_DomoBootstrap.ipynb 5
 @dataclass
 class DomoBootstrap:
     auth : dmda.DomoAuth = field(repr = False)
     page_ls : list[dmpg.DomoPage] = field(default = None)
     feature_ls : list[DomoBootstrap_Feature] = field(default = None)
     
 
-# %% ../../nbs/classes/50_.DomoBootstrap.ipynb 6
+# %% ../../nbs/classes/50_DomoBootstrap.ipynb 6
 @patch_to(DomoBootstrap)
 async def get_all(self: DomoBootstrap,
                   auth: dmda.DomoAuth = None, debug_api: bool = False):
     
     auth = auth or self.auth
 
     res =  await bootstrap_routes.get_bootstrap(auth=auth, debug_api=debug_api)
 
     return res.response
 
 
-# %% ../../nbs/classes/50_.DomoBootstrap.ipynb 9
+# %% ../../nbs/classes/50_DomoBootstrap.ipynb 9
 @patch_to(DomoBootstrap)
 async def get_pages(self: DomoBootstrap,
                     auth: dmda.DomoAuth = None, return_raw : bool = False, debug_api: bool = False) -> list[dmpg.DomoPage]:
 
     auth = auth or self.auth
 
     res = await bootstrap_routes.get_bootstrap_pages(auth=auth,
@@ -85,15 +84,15 @@
     page_ls = res.response
 
     self.page_ls =  [dmpg.DomoPage._from_bootstrap(page_obj, auth = auth) for page_obj in page_ls]
 
     return self.page_ls
 
 
-# %% ../../nbs/classes/50_.DomoBootstrap.ipynb 12
+# %% ../../nbs/classes/50_DomoBootstrap.ipynb 12
 @patch_to(DomoBootstrap)
 async def get_features(self : DomoBootstrap,
                         auth: dmda.DomoAuth = None,
                         debug_api: bool = False,
                         return_raw:bool = False,
                         session: httpx.AsyncClient = None, 
                         ):
```

### Comparing `domolibrary-0.0.8/domolibrary/classes/DomoDataset.py` & `domolibrary-0.0.9/domolibrary/classes/DomoDataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,31 @@
            'DomoDataset_Schema_Column', 'DomoDataset_Schema', 'DatasetTags_AuthNotProvidedError',
            'DatasetTags_SetTagsError', 'DomoDataset_Tags', 'DomoDataset', 'QueryExecutionError',
            'DomoDataset_DeleteDataset_Error', 'DomoDataset_UploadData_Error',
            'DomoDataset_UploadData_DatasetUploadId_Error', 'DomoDataset_UploadData_UploadData_Error',
            'DomoDataset_CreateDataset_Error']
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 4
-from fastcore.basics import patch, patch_to
+from fastcore.basics import patch_to
 import pandas as pd
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 5
 from dataclasses import dataclass, field
 from typing import Any, List, Optional
 from enum import Enum, auto
 
 import json
+import io
 
-import aiohttp
+import httpx
+import asyncio
 
-import io
 
 # import datetime as dt
 
-# import asyncio
 # import importlib
 # import json
 # from pprint import pprint
 
 # import pandas as pd
 
 # from ..utils import Exceptions as ex
@@ -125,16 +125,16 @@
 
             return self.columns
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 12
 class DatasetTags_AuthNotProvidedError(Exception):
     """return if DatasetTags request cannot access an auth object"""
 
-    def __init__(self, id):
-        message = f"valid Auth object not provided to dataset - {id}"
+    def __init__(self, dataset_id):
+        message = f"valid Auth object not provided to dataset - {dataset_id}"
         super().__init__(message)
 
 
 class DatasetTags_SetTagsError(Exception):
     """return if DatasetTags request is not successfull"""
 
     def __init__(self, dataset_id, domo_instance):
@@ -165,15 +165,15 @@
         return auth, dataset_id
 
     async def get(
         self,
         dataset_id: str = None,
         auth: Optional[dmda.DomoAuth] = None,
         debug_api: bool = False,
-        session: Optional[aiohttp.ClientSession] = None,
+        session: Optional[httpx.AsyncClient] = None,
     ) -> List[str]:  # returns a list of tags
         """gets the existing list of dataset_tags"""
 
         auth, dataset_id = self._have_prereqs(auth=auth, dataset_id=dataset_id)
 
         res = await dataset_routes.get_dataset_by_id(
             dataset_id=dataset_id, auth=auth, debug_api=debug_api, session=session
@@ -191,15 +191,15 @@
 
     async def set(
         self,
         tag_ls: [str],
         dataset_id: str = None,
         auth: Optional[dmda.DomoAuth] = None,
         debug_api: bool = False,
-        session: Optional[aiohttp.ClientSession] = None,
+        session: Optional[httpx.AsyncClient] = None,
     ) -> List[str]: # returns a list of tags
         """replaces all tags with a new list of dataset_tags"""
 
         auth, dataset_id = self._have_prereqs(auth=auth, dataset_id=dataset_id)
 
         res = await dataset_routes.set_dataset_tags(
             auth=auth,
@@ -215,46 +215,47 @@
             )
 
         await self.get(dataset_id=dataset_id, auth=auth)
 
         return self.tag_ls
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 15
-@patch
+@patch_to(DomoDataset_Tags)
 async def add(
     self: DomoDataset_Tags,
     add_tag_ls: [str],
     dataset_id: str = None,
     auth: Optional[dmda.DomoAuth] = None,
     debug_api: bool = False,
-    session: Optional[aiohttp.ClientSession] = None,
+    session: Optional[httpx.AsyncClient] = None,
 ) -> List[str]:  # returns a list of tags
     """appends tags to the list of existing dataset_tags"""
 
     auth, dataset_id = self._have_prereqs(auth=auth, dataset_id=dataset_id)
 
     existing_tag_ls = await self.get(dataset_id=dataset_id, auth=auth)
+    
     add_tag_ls += existing_tag_ls
 
     return await self.set(
         auth=auth,
         dataset_id=dataset_id,
         tag_ls=list(set(add_tag_ls)),
         debug_api=debug_api,
         session=session,
     )
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 17
-@patch
+@patch_to(DomoDataset_Tags)
 async def remove(self: DomoDataset_Tags,
                  remove_tag_ls: [str],
                  dataset_id: str = None,
                  auth: dmda.DomoFullAuth = None,
                  debug_api: bool = False,
-                 session: Optional[aiohttp.ClientSession] = None
+                 session: Optional[httpx.AsyncClient] = None
                  ) -> List[str]:  # returns a list of tags
     """removes tags from the existing list of dataset_tags"""
 
     auth, dataset_id = self._have_prereqs(auth=auth, dataset_id=dataset_id)
 
     existing_tag_ls = await self.get(dataset_id=dataset_id, auth=auth)
 
@@ -299,15 +300,15 @@
 
         # self.PDPPolicies = dmpdp.Dataset_PDP_Policies(self)
 
     def display_url(self):
         return f"https://{self.auth.domo_instance }.domo.com/datasources/{self.id}/details/overview"
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 25
-@patch(cls_method=True)
+@patch_to(DomoDataset, cls_method=True)
 async def get_from_id(
     cls: DomoDataset,
     dataset_id: str,
     auth: dmda.DomoAuth,
     debug_api: bool = False,
     return_raw_res: bool = False,
 ):
@@ -347,23 +348,23 @@
     return ds
 
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 29
 class QueryExecutionError(Exception):
     def __init__(self, sql, dataset_id, domo_instance):
         self.message = f"error executing {sql} against dataset {dataset_id} in {domo_instance}"
-        super.__init__(self, self.message)
+        super().__init__(self, self.message)
 
 
 @patch_to(DomoDataset, cls_method=True)
 async def query_dataset_private(cls: DomoDataset,
                                 auth: dmda.DomoAuth,  # DomoFullAuth or DomoTokenAuth
                                 dataset_id: str,
                                 sql: str,
-                                session: Optional[aiohttp.ClientSession] = None,
+                                session: Optional[httpx.AsyncClient] = None,
                                 loop_until_end: bool = False,  # retrieve all available rows
                                 limit=100,  # maximum rows to return per request.  refers to PAGINATION
                                 skip=0,
                                 maximum=100,  # equivalent to the LIMIT or TOP clause in SQL, the number of rows to return total
                                 debug_api: bool = False,
                                 debug_loop: bool = False,
                                 ) -> pd.DataFrame:
@@ -386,22 +387,22 @@
     return pd.DataFrame(res.response)
 
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 30
 class DomoDataset_DeleteDataset_Error(Exception):
     def __init__(self, status, reason, dataset_id, domo_instance):
         message = f"Error deleting {dataset_id} from {domo_instance}: {status} - {reason}"
-        super.__init__(message)
+        super().__init__(message)
 
 @patch_to(DomoDataset)
 async def delete(self : DomoDataset,
                     dataset_id=None,
                     auth: dmda.DomoAuth = None,
                     debug_api: bool = False,
-                    session: aiohttp.ClientSession = None):
+                    session: httpx.AsyncClient = None):
 
     dataset_id = dataset_id or self.id
     auth = auth or self.auth
 
     res = await dataset_routes.delete(
         auth=auth,
         dataset_id=dataset_id,
@@ -427,14 +428,16 @@
         message_start = f"Stage {stage}:: {message_error} :: API {status} - {reason} :: "
         message_end = f"in {dataset_id} in {domo_instance}"
 
         message_partition = ""
         if partition_key:
             message_partition = f"for partition - '{partition_key}' "
 
+        message = f"{message_start}{message_partition}{message_end}"
+
         super().__init__(message)
 
 
 class DomoDataset_UploadData_DatasetUploadId_Error(DomoDataset_UploadData_Error):
     def __init__(self, domo_instance: str, dataset_id: str,
                  stage: int = 1, status="", reason="",
                  partition_key: str = None):
@@ -443,46 +446,46 @@
 
         super().__init__(message_error=message_error,
                          domo_instance=domo_instance, dataset_id=dataset_id,
                          stage=stage, status=status, reason=reason,
                          partition_key=partition_key)
 
 
-class DomoDataset_UploadData_UploadData_Error(Exception):
+class DomoDataset_UploadData_UploadData_Error(DomoDataset_UploadData_Error):
     def __init__(self, domo_instance: str, dataset_id: str,
                  stage: int = 2, status="", reason="",
                  partition_key: str = None):
 
         message_error = "while uploading data"
 
         super().__init__(message_error=message_error,
                          domo_instance=domo_instance, dataset_id=dataset_id,
                          stage=stage, status=status, reason=reason,
                          partition_key=partition_key)
 
-    class DomoDataset_UploadData_CommitDatasetUploadId_Error(Exception):
+    class DomoDataset_UploadData_DatasetUploadId_Error(DomoDataset_UploadData_Error):
         def __init__(self, domo_instance: str, dataset_id: str,
                      stage: int = 3, status="", reason="",
                      partition_key: str = None):
 
             message_error = "while commiting dataset_upload_id"
 
-            ssuper().__init__(message_error=message_error,
+            super().__init__(message_error=message_error,
                               domo_instance=domo_instance, dataset_id=dataset_id,
                               stage=stage, status=status, reason=reason,
                               partition_key=partition_key)
 
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 34
 @patch_to(DomoDataset)
 async def index_dataset(self: DomoDataset,
                         auth: dmda.DomoAuth = None,
                         dataset_id: str = None,
                         debug_api: bool = False,
-                        session: aiohttp.ClientSession = None
+                        session: httpx.AsyncClient = None
                         ):
 
     auth = auth or self.auth
     dataset_id = dataset_id or self.id
     return await dataset_routes.index_dataset(auth=auth, dataset_id=dataset_id, debug_api=debug_api,
                                               session=session)
 
@@ -500,69 +503,69 @@
                       is_index: bool = True,
 
                       dataset_id: str = None,
                       dataset_upload_id=None,
 
                       auth: dmda.DomoAuth = None,
 
-                      session: aiohttp.ClientSession = None,
+                      session: httpx.AsyncClient = None,
                       debug_api: bool = False,
                       debug_prn: bool = False
                       ):
 
     auth = auth or self.auth
     dataset_id = dataset_id or self.id
 
-    upload_df_list = upload_df_list or [upload_df]
+    upload_df_ls = upload_df_ls or [upload_df]
 
     # stage 1 get uploadId
     if not dataset_upload_id:
         if debug_prn:
             print(f"\n\n🎭 starting Stage 1")
 
         stage_1_res = await dataset_routes.upload_dataset_stage_1(auth=auth,
                                                                   dataset_id=dataset_id,
                                                                   session=session,
-                                                                  data_tag=partition_key,
+                                                                  partition_tag=partition_key,
                                                                   debug_api=debug_api
                                                                   )
         if debug_prn:
             print(f"\n\n🎭 Stage 1 response -- {stage_1_res.status}")
 
         dataset_upload_id = stage_1_res.response.get('uploadId')
 
     if not dataset_upload_id:
         raise DomoDataset_UploadData_DatasetUploadId_Error(
-            domo_instnace=auth.domo_instance,  dataset_id=dataset_id, stage=1, partition_key=partition_key,
+            domo_instance=auth.domo_instance,  dataset_id=dataset_id, stage=1, partition_key=partition_key,
             status=stage_1_res.status, reason=stage_1_res.response)
 
     # stage 2 upload_dataset
     stage_2_res = None
 
     if upload_file:
         if debug_prn:
             print(f"\n\n🎭 starting Stage 2 - upload file")
 
         stage_2_res = await asyncio.gather(*[dataset_routes.upload_dataset_stage_2_file(auth=auth,
                                                                                         dataset_id=dataset_id,
                                                                                         upload_id=dataset_upload_id,
                                                                                         part_id=1,
-                                                                                        file=upload_file,
+                                                                                        data_file=upload_file,
                                                                                         session=session, debug_api=debug_api)])
 
     else:
         if debug_prn:
             print(
-                f"\n\n🎭 starting Stage 2 - {len(upload_df_list)} - number of parts")
+                f"\n\n🎭 starting Stage 2 - {len(upload_df_ls)} - number of parts")
         stage_2_res = await asyncio.gather(*[dataset_routes.upload_dataset_stage_2_df(auth=auth,
                                                                                       dataset_id=dataset_id,
                                                                                       upload_id=dataset_upload_id,
                                                                                       part_id=index + 1,
                                                                                       upload_df=df,
-                                                                                      session=session, debug_api=debug_api) for index, df in enumerate(upload_df_list)])
+                                                                                      session=session, debug_api=debug_api) for index, df in enumerate(upload_df_ls)])
 
     for res in stage_2_res:
         if not res.is_success:
             raise DomoDataset_UploadData_UploadData_Error(
                 domo_instance=auth.domo_instance, dataset_id=dataset_id, stage=2, partition_key=partition_key,
                 status=res.status, reason=res.response)
 
@@ -574,15 +577,15 @@
         print(f"\n\n🎭 starting Stage 3 - commit dataset_upload_id")
 
     await asyncio.sleep(10)  # wait for uploads to finish
     stage3_res = await dataset_routes.upload_dataset_stage_3(auth=auth,
                                                              dataset_id=dataset_id,
                                                              upload_id=dataset_upload_id,
                                                              update_method=upload_method,
-                                                             data_tag=partition_key,
+                                                             partition_tag=partition_key,
                                                              is_index=False,
                                                              session=session,
                                                              debug_api=debug_api)
 
     if not stage3_res.is_success:
         raise DomoDataset_UploadData_CommitDatasetUploadId_Error(
             domo_instance=auth.domo_instance, dataset_id=dataset_id, partition_key=partition_key, stage=3,
@@ -603,15 +606,15 @@
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 37
 @patch_to(DomoDataset)
 async def list_partitions(self : DomoDataset,
                             auth: dmda.DomoAuth = None,
                             dataset_id: str = None,
                             debug_api: bool = False,
-                            session: aiohttp.ClientSession = None
+                            session: httpx.AsyncClient = None
                             ):
 
     auth = auth or self.auth
     dataset_id = dataset_id or self.id
 
     res = await dataset_routes.list_partitions(auth=auth, dataset_id=dataset_id, debug_api=debug_api,
                                                 session=session)
@@ -633,15 +636,15 @@
 
                  schema={"columns": [
                      {"name": 'col1', "type": 'LONG', "upsertKey": False},
                      {"name": 'col2', "type": 'STRING', "upsertKey": False}
                  ]},
                  auth: dmda.DomoAuth = None,
                  debug_api: bool = False, 
-                 session : aiohttp.ClientSession = None
+                 session : httpx.AsyncClient = None
                  ):
     
 
     res = await dataset_routes.create(dataset_name=dataset_name,
                                       dataset_type=dataset_type,
                                       schema=schema, auth=auth, debug_api=debug_api, session=session
                                       )
```

### Comparing `domolibrary-0.0.8/domolibrary/classes/DomoPage.py` & `domolibrary-0.0.9/domolibrary/classes/DomoPage.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # %% ../../nbs/classes/50_DomoPage.ipynb 2
 from fastcore.basics import patch_to
 
 # %% ../../nbs/classes/50_DomoPage.ipynb 3
 from dataclasses import dataclass, field
 
 # import asyncio
-# import aiohttp
+# import httpx
 
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.classes.DomoUser as dmdu
 import domolibrary.utils.DictDot as util_dd
 
 # from .routes import page_routes
 # from ..utils.Base import Base
@@ -62,7 +62,13 @@
         ]
 
         [print(other_dd) for other_dd in dd.children
             if other_dd.type != "page"]
 
     return domo_page
 
+
+# %% ../../nbs/classes/50_DomoPage.ipynb 7
+@patch_to(DomoPage)
+def _ol_fn():
+    pass
+
```

### Comparing `domolibrary-0.0.8/domolibrary/classes/DomoUser.py` & `domolibrary-0.0.9/domolibrary/classes/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/domolibrary/client/DomoAuth.py` & `domolibrary-0.0.9/domolibrary/client/DomoAuth.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,33 +5,33 @@
            'InvalidInstanceError', 'DomoFullAuth', 'DomoTokenAuth', 'DomoDeveloperAuth']
 
 # %% ../../nbs/client/95_DomoAuth.ipynb 3
 from dataclasses import dataclass, field
 from abc import abstractmethod
 from typing import Optional, Union
 
-import aiohttp
+import httpx
 
 import domolibrary.client.ResponseGetData as rgd
 
 # %% ../../nbs/client/95_DomoAuth.ipynb 5
 async def get_full_auth(
     domo_instance: str,  # domo_instance.domo.com
     domo_username: str,  # email address
     domo_password: str,
-    session: Optional[aiohttp.ClientSession] = None,
+    session: Optional[httpx.AsyncClient] = None,
     debug_api: bool = False
 ) -> rgd.ResponseGetData:
     """uses username and password authentication to retrieve a full_auth access token"""
 
     is_close_session = False
 
     if not session:
         is_close_session = True
-        session = aiohttp.ClientSession()
+        session = httpx.AsyncClient()
 
     url = f"https://{domo_instance}.domo.com/api/content/v2/authentication"
 
     tokenHeaders = {"Content-Type": "application/json"}
 
     body = {
         "method": "password",
@@ -41,80 +41,80 @@
 
     if debug_api:
         print(body, url)
 
     res = await session.request(method="POST", url=url, headers=tokenHeaders, json=body)
 
     if is_close_session:
-        await session.close()
+        await session.aclose()
 
-    return await rgd.ResponseGetData._from_aiohttp_response(res)
+    return rgd.ResponseGetData._from_httpx_response(res)
 
 # %% ../../nbs/client/95_DomoAuth.ipynb 12
 async def get_developer_auth(
     domo_client_id: str,
     domo_client_secret: str,
-    session: Optional[aiohttp.ClientSession] = None,
+    session: Optional[httpx.AsyncClient] = None,
     debug_api: bool = False
 ) -> rgd.ResponseGetData:
 
     """
     only use for authenticating against apis documented under developer.domo.com
     """
     is_close_session = False
 
     if not session:
         is_close_session = True
-        session = aiohttp.ClientSession(
-            auth=aiohttp.BasicAuth(domo_client_id, domo_client_secret)
+        session = httpx.AsyncClient(
+            auth=httpx.BasicAuth(domo_client_id, domo_client_secret)
         )
 
     url = f"https://api.domo.com/oauth/token?grant_type=client_credentials"
 
     if debug_api:
         print(url, domo_client_id, domo_client_secret)
 
     res = await session.request(method="GET", url=url)
 
     if is_close_session:
-        await session.close()
+        await session.aclose()
 
-    return await rgd.ResponseGetData._from_aiohttp_response(res)
+    return rgd.ResponseGetData._from_httpx_response(res)
 
 # %% ../../nbs/client/95_DomoAuth.ipynb 16
 async def test_access_token(
     domo_access_token: str,  # as provided in Domo > Admin > Authentication > AccessTokens
     domo_instance: str,  # <domo_instance>.domo.com
-    session: Optional[aiohttp.ClientSession] = None,
+    session: Optional[httpx.AsyncClient] = None,
     debug_api: bool = False
 ):
     """
     will attempt to validate against the 'me' API.
     This is the same authentication test the Domo Java CLI uses.
     """
 
     is_close_session = False
 
     if not session:
         is_close_session = True
-        session = aiohttp.ClientSession()
+        session = httpx.AsyncClient()
 
     url = f"https://{domo_instance}.domo.com/api/content/v2/users/me"
 
     tokenHeaders = {"X-DOMO-Developer-Token": domo_access_token}
 
     if debug_api:
         print(url,tokenHeaders)
 
     res = await session.request(method="GET", headers=tokenHeaders, url=url)
 
     if is_close_session:
-        await session.close()
+        await session.aclose()
 
-    return await rgd.ResponseGetData._from_aiohttp_response(res)
+    return rgd.ResponseGetData._from_httpx_response(res)
 
 # %% ../../nbs/client/95_DomoAuth.ipynb 20
 @dataclass
 class _DomoAuth_Required:
     """required parameters for all Domo Auth classes"""
 
     domo_instance: str
@@ -228,15 +228,15 @@
 
     def generate_auth_header(self, token: str) -> dict:
         self.auth_header = {"x-domo-authentication": token}
         return self.auth_header
 
     async def get_auth_token(
         self,
-        session: Optional[aiohttp.ClientSession] = None,
+        session: Optional[httpx.AsyncClient] = None,
         debug_api : bool = False
     ) -> str:
         """returns `token` if valid credentials provided else raises Exception and returns None"""
 
         res = await get_full_auth(
             domo_instance=self.domo_instance,
             domo_username=self.domo_username,
@@ -266,36 +266,36 @@
         self.auth_header = self.generate_auth_header(token=token)
 
         if not self.token_name:
             self.token_name = "full_auth"
 
         return self.token
 
-# %% ../../nbs/client/95_DomoAuth.ipynb 36
+# %% ../../nbs/client/95_DomoAuth.ipynb 37
 @dataclass
 class _DomoTokenAuth_Required(_DomoAuth_Required):
     """mix requied parameters for DomoFullAuth"""
 
     domo_access_token: str = field(repr=False)
 
-# %% ../../nbs/client/95_DomoAuth.ipynb 37
+# %% ../../nbs/client/95_DomoAuth.ipynb 38
 @dataclass
 class DomoTokenAuth(_DomoAuth_Optional, _DomoTokenAuth_Required):
     """
     use for access_token authentication.
     Tokens are generated in domo > admin > access token
     Necessary in cases where direct sign on is not permitted
     """
 
     def generate_auth_header(self, token: str) -> dict:
         self.auth_header = {"x-domo-developer-token": token}
         return self.auth_header
 
     async def get_auth_token(
-        self, session: Optional[aiohttp.ClientSession] = None,
+        self, session: Optional[httpx.AsyncClient] = None,
         debug_api : bool = False
     ) -> str:
         """
         updates internal attributes
         having an access_token assumes pre-authenticaiton
         """
 
@@ -319,23 +319,23 @@
         self.auth_header = self.generate_auth_header(token=self.token)
 
         if not self.token_name:
             self.token_name = "token_auth"
 
         return self.token
 
-# %% ../../nbs/client/95_DomoAuth.ipynb 41
+# %% ../../nbs/client/95_DomoAuth.ipynb 42
 @dataclass
 class _DomoDeveloperAuth_Required(_DomoAuth_Required):
     """mix requied parameters for DomoFullAuth"""
 
     domo_client_id: str
     domo_client_secret: str = field(repr=False)
 
-# %% ../../nbs/client/95_DomoAuth.ipynb 42
+# %% ../../nbs/client/95_DomoAuth.ipynb 43
 @dataclass(init=False)
 class DomoDeveloperAuth(_DomoAuth_Optional, _DomoDeveloperAuth_Required):
     """use for full authentication token"""
 
     def __init__(self, domo_client_id: str, domo_client_secret: str):
         self.domo_client_id = domo_client_id
         self.domo_client_secret = domo_client_secret
@@ -343,15 +343,15 @@
 
     def generate_auth_header(self, token: str) -> dict:
         self.auth_header = {"Authorization": "bearer " + token}
         return self.auth_header
 
     async def get_auth_token(
         self,
-        session: Optional[aiohttp.ClientSession] = None,
+        session: Optional[httpx.AsyncClient] = None,
         debug_api : bool = False
     ) -> str:
 
         res = await get_developer_auth(
             domo_client_id=self.domo_client_id,
             domo_client_secret=self.domo_client_secret,
             session=session,
```

### Comparing `domolibrary-0.0.8/domolibrary/client/Logger.py` & `domolibrary-0.0.9/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/domolibrary/client/ResponseGetData.py` & `domolibrary-0.0.9/domolibrary/client/ResponseGetData.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/client/99_ResponseGetData.ipynb.
 
 # %% auto 0
 __all__ = ['API_Response', 'STREAM_FILE_PATH', 'ResponseGetData']
 
 # %% ../../nbs/client/99_ResponseGetData.ipynb 2
 # pylint: disable=no-member
+
 from dataclasses import dataclass, field
 from typing import Optional
 
-import json
 import orjson
 
-
 import asyncio
 import requests
+import httpx
 import aiohttp
 
-from fastcore.utils import patch_to, patch
+from fastcore.utils import patch_to
 
 # %% ../../nbs/client/99_ResponseGetData.ipynb 4
 API_Response = any
 
 
 @dataclass
 class ResponseGetData:
@@ -74,15 +74,15 @@
     # errors
     return cls(status=res.status_code, response=res.reason_phrase, is_success=False, auth=auth)
 
 
 # %% ../../nbs/client/99_ResponseGetData.ipynb 15
 STREAM_FILE_PATH = '__large-file.json'
 
-async def _write_stream(res: aiohttp.ClientResponse,
+async def _write_stream(res: httpx.Response,
                         file_name: str = STREAM_FILE_PATH,
                         stream_chunks=10):
     
     print(type(res), type(res.content), stream_chunks)
 
     index = 0
     with open(file_name, 'wb') as fd:
@@ -100,15 +100,15 @@
 
 async def _read_stream(file_name : str = STREAM_FILE_PATH):
     with open(STREAM_FILE_PATH, "rb") as f:
         return f.read()
 
 
 # %% ../../nbs/client/99_ResponseGetData.ipynb 16
-@patch(cls_method=True)
+@patch_to(ResponseGetData, cls_method=True)
 async def _from_aiohttp_response(
     cls: ResponseGetData, 
     res: aiohttp.ClientResponse,  # requests response object
     auth : Optional[any] = None,
     process_stream: bool = False,
     stream_chunks : int = 10,
     debug_api : bool = False
@@ -144,15 +144,15 @@
         return cls(status=res.status, response= data, is_success=True, auth = auth)
 
     # response is error
     else:
         return cls(status=res.status, response=res.reason, is_success=False, auth = auth)
 
 # %% ../../nbs/client/99_ResponseGetData.ipynb 20
-@patch(cls_method=True)
+@patch_to(ResponseGetData, cls_method=True)
 async def _from_looper(cls: ResponseGetData,
                        res: ResponseGetData,  # requests response object
                        array: list
                        ) -> ResponseGetData:
 
     """async method returns ResponseGetData"""
```

### Comparing `domolibrary-0.0.8/domolibrary/client/get_data.py` & `domolibrary-0.0.9/domolibrary/client/get_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/client/10_get_data.ipynb.
 
 # %% auto 0
-__all__ = ['get_data_aiohttp', 'get_data', 'LooperError', 'looper']
+__all__ = ['get_data_aiohttp', 'get_data', 'LooperError', 'looper', 'looper_aiohttp']
 
 # %% ../../nbs/client/10_get_data.ipynb 2
 from typing import Optional, Union
 
 from pprint import pprint
 
-import aiohttp
 import httpx
-
+import aiohttp
 
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.client.ResponseGetData as rgd
 
 
 # %% ../../nbs/client/10_get_data.ipynb 3
 async def get_data_aiohttp(
@@ -36,14 +35,15 @@
     if auth and not auth.token:
         await auth.get_auth_token()
 
     if headers is None:
         headers = {}
 
     is_close_session = False
+
     if session is None:
         is_close_session = True
         session = session or aiohttp.ClientSession()
 
     headers = {
         "Content-Type": content_type or "application/json",
         "Connection": "keep-alive",
@@ -91,15 +91,15 @@
 
     except Exception as e:
         print(e)
 
     finally:
         if is_close_session:
             await session.close()
-    
+        
     return await rgd.ResponseGetData._from_aiohttp_response(res, auth=auth, debug_api=debug_api, process_stream=process_stream, stream_chunks=stream_chunks)
 
 
 # %% ../../nbs/client/10_get_data.ipynb 6
 async def get_data(
     url: str,
     method: str,
@@ -187,23 +187,135 @@
     if return_raw:
         return res
 
 
     return rgd.ResponseGetData._from_httpx_response(res, auth=auth, debug_api=debug_api)
 
 
-# %% ../../nbs/client/10_get_data.ipynb 8
+# %% ../../nbs/client/10_get_data.ipynb 9
 class LooperError(Exception):
     def __init__(self, loop_stage: str, message ):
 
         super().__init__(f"{loop_stage} - {message}")
 
-# %% ../../nbs/client/10_get_data.ipynb 9
+# %% ../../nbs/client/10_get_data.ipynb 10
 async def looper(
     auth: dmda.DomoAuth,
+    session: httpx.AsyncClient,
+    url,
+    offset_params,
+    arr_fn: callable,
+    loop_until_end: bool = False,
+    method="POST",
+    body: dict = None,
+    fixed_params: dict = None,
+    offset_params_in_body: bool = False,
+    body_fn=None,
+    limit=1000,
+    skip = 0,
+    maximum=2000,
+    debug_api: bool = False,
+    debug_loop: bool = False
+) -> rgd.ResponseGetData:
+
+    is_close_session = False
+    
+    if not session:
+        session = httpx.AsyncClient()
+        is_close_session = True
+
+
+    allRows = []
+    isLoop = True
+
+    res = None
+
+    if maximum < limit:
+        limit = maximum
+
+    while isLoop:
+        params = fixed_params or {}
+
+        if offset_params_in_body:
+            body[offset_params.get("offset")] = skip
+            body[offset_params.get("limit")] = limit
+
+        else:
+            params[offset_params.get("offset")] = skip
+            params[offset_params.get("limit")] = limit
+
+        if body_fn:
+            try:
+                body = body_fn(skip, limit)
+            
+            except Exception as e:
+                await session.aclose()
+                raise LooperError(loop_stage = "processing body_fn", message = str(e))
+            
+
+        if debug_loop:
+            print(
+                f"\n🚀 Retrieving records {skip} through {skip + limit} via {url}")
+            # pprint(params)
+
+        
+        res = await get_data(
+            auth=auth,
+            url=url,
+            method=method,
+            params=params,
+            session=session,
+            body=body,
+            debug_api=debug_api,
+        )
+
+        if not res.is_success:
+            if is_close_session:
+                await session.aclose()
+            return res
+
+
+        try:
+            newRecords = arr_fn(res)
+        
+        except Exception as e:
+            await session.aclose()
+            raise LooperError(loop_stage = "processing arr_fn", message = str(e))
+        
+        allRows += newRecords
+
+        if loop_until_end and len(newRecords) != 0:
+            maximum = maximum + limit
+
+        if debug_loop:
+            print({"all_rows": len(allRows), "new_records": len(newRecords)})
+
+        if len(allRows) >= maximum or len(newRecords) == 0:
+            if debug_loop:
+                print(
+                    f"\n🎉 Success - {len(allRows)} records retrieved from {url} in query looper\n")
+
+            break
+
+        skip += len(newRecords)
+        
+        if skip + limit > maximum:
+            limit = maximum - len(allRows)
+
+            if debug_loop:
+                print(f"skip: {skip}, limit: {limit}")
+    
+    if is_close_session:
+        await session.aclose()
+
+    return await rgd.ResponseGetData._from_looper(res = res, array = allRows)
+
+# %% ../../nbs/client/10_get_data.ipynb 14
+async def looper_aiohttp(
+    auth: dmda.DomoAuth,
     session: aiohttp.ClientSession,
     url,
     offset_params,
     arr_fn: callable,
     loop_until_end: bool = False,
     method="POST",
     body: dict = None,
@@ -244,15 +356,15 @@
             params[offset_params.get("limit")] = limit
 
         if body_fn:
             try:
                 body = body_fn(skip, limit)
             
             except Exception as e:
-                await session.close()
+                await session.aclose()
                 raise LooperError(loop_stage = "processing body_fn", message = str(e))
             
 
         if debug_loop:
             print(
                 f"\n🚀 Retrieving records {skip} through {skip + limit} via {url}")
             # pprint(params)
@@ -266,15 +378,15 @@
             session=session,
             body=body,
             debug_api=debug_api,
         )
 
         if not res.is_success:
             if is_close_session:
-                await session.close()
+                await session.aclose()
             return res
 
 
         try:
             newRecords = arr_fn(res)
         
         except Exception as e:
```

### Comparing `domolibrary-0.0.8/domolibrary/integrations/DomoJupyter.py` & `domolibrary-0.0.9/domolibrary/integrations/DomoJupyter.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         self.config = df
 
         message = f"\n⚙️ SUCCESS 🎉 Retrieved company list \nThere are {len(df.index)} companies to update"
 
         if debug_prn:
             print(message)
-        logger.log_info(message, debug_log=debug_log)
+        self.logger.log_info(message, debug_log=debug_log)
 
         return df
 
 
 # %% ../../nbs/integrations/DomoJupyter.ipynb 6
 class GetDomains_Query_Exception_PW_Col_Error(Exception):
     """raise if SQL query fails to return column named 'config_exception_pw'"""
@@ -245,23 +245,20 @@
     retry_attempt = 0
     while not account_properties and retry_attempt <= maximum_retry:
         try:
             account_properties = domojupyter_fn.get_account_property_keys(
                 account_name)
             retry_attempt += 1
 
-        except GetJupyter_ErrorRetrievingAccount as e:
-            return None
-
         except Exception as e:
-            print(f"trying again - {account_name}")
+            print(f"Error:  retry attempt {retry_attempt} - {account_name}")
             time.sleep(2)
     
     if not account_properties:
-        raise GetJupyter_ErrorRetrievingAccountProperty(
+        raise GetJupyter_ErrorRetrievingAccount(
             account_name=account_name)
 
     obj = {}
 
     retry_attempt = 0
     for index, prop in enumerate(account_properties):
         value = None
```

### Comparing `domolibrary-0.0.8/domolibrary/routes/account.py` & `domolibrary-0.0.9/domolibrary/routes/account.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 
 # %% auto 0
 __all__ = ['get_accounts', 'get_account_from_id', 'AccountConfig_InvalidDataProvider', 'get_account_config',
            'update_account_config', 'update_account_name', 'create_account', 'delete_account']
 
 # %% ../../nbs/routes/account.ipynb 3
 from typing import Union
-import aiohttp
+import httpx
 import httpx
 
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoAuth as dmda
 
 # %% ../../nbs/routes/account.ipynb 4
 async def get_accounts(auth: dmda.DomoAuth,
                        debug_api: bool = False, 
-                       session: Union[aiohttp.ClientSession, httpx.AsyncClient, None] = None):
+                       session: Union[httpx.AsyncClient, httpx.AsyncClient, None] = None):
     """retrieve a list of all the accounts the user has read access to.  Note users with "Manage all accounts" will retrieve all account objects"""
     
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/accounts"
 
     return await gd.get_data(
         auth=auth,
         url=url,
         method='GET',
         debug_api=debug_api,
         session=session
     )
 
 # %% ../../nbs/routes/account.ipynb 7
 async def get_account_from_id(auth: dmda.DomoAuth, account_id: int,
-                              debug_api: bool = False, session: aiohttp.ClientSession = None):
+                              debug_api: bool = False, session: httpx.AsyncClient = None):
     """retrieves metadata about an account"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/accounts/{account_id}?unmask=true"
 
     if debug_api:
         print(url)
 
@@ -53,15 +53,15 @@
         message = f"Account - {account_id}, could not be retrieved with data_provider_type, '{data_provider_type}' from {domo_instance}"
         super().__init__( message)
 
 async def get_account_config(auth: dmda.DomoAuth,
                              account_id: int,
                              data_provider_type: str ,
                              debug_api: bool = False, 
-                             session: Union[aiohttp.ClientSession, httpx.AsyncClient, None] = None):
+                             session: Union[httpx.AsyncClient, httpx.AsyncClient, None] = None):
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/providers/{data_provider_type}/account/{account_id}?unmask=true"
 
     if debug_api:
         print(url)
 
     res = await gd.get_data(
@@ -79,15 +79,15 @@
 
 # %% ../../nbs/routes/account.ipynb 14
 async def update_account_config(auth: dmda.DomoAuth,
                                 account_id: int,
                                 config_body: dict,
                                 data_provider_type: str,
                                 debug_api: bool = False, 
-                                session: aiohttp.ClientSession = None):
+                                session: httpx.AsyncClient = None):
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/providers/{data_provider_type}/account/{account_id}"
 
     if debug_api:
         print(url)
 
     return await gd.get_data(
@@ -100,15 +100,15 @@
     )
 
 # %% ../../nbs/routes/account.ipynb 15
 async def update_account_name(auth: dmda.DomoAuth,
                               account_id: int,
                               account_name: str,
                               debug_api: bool = False, 
-                              session: aiohttp.ClientSession = None):
+                              session: httpx.AsyncClient = None):
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/accounts/{account_id}/name"
     
     if debug_api:
         print(url)
 
     return await gd.get_data(
@@ -119,15 +119,15 @@
         content_type = "text/plain",
         debug_api=debug_api,
         session=session
     )
 
 # %% ../../nbs/routes/account.ipynb 16
 async def create_account(auth:dmda.DomoAuth, config_body:dict,
-                         debug_api: bool = False, session: aiohttp.ClientSession = None):
+                         debug_api: bool = False, session: httpx.AsyncClient = None):
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/accounts"
 
     if debug_api:
         print(url)
 
     return await gd.get_data(
@@ -139,15 +139,15 @@
         session=session
     )
 
 # %% ../../nbs/routes/account.ipynb 17
 async def delete_account(auth:dmda.DomoAuth,
                          account_id: str,
                          debug_api: bool = False, 
-                         session: aiohttp.ClientSession = None):
+                         session: httpx.AsyncClient = None):
     
     url = f"https://{auth.domo_instance}.domo.com/api/data/v1/accounts/{account_id}"
 
     if debug_api:
         print(url)
 
     return await gd.get_data(
```

### Comparing `domolibrary-0.0.8/domolibrary/routes/activity_log.py` & `domolibrary-0.0.9/domolibrary/routes/activity_log.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/activity_log.ipynb.
 
 # %% auto 0
 __all__ = ['get_activity_log_object_types', 'search_activity_log']
 
 # %% ../../nbs/routes/activity_log.ipynb 3
-import aiohttp
+import httpx
 
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoAuth as dmda
 
 
 # %% ../../nbs/routes/activity_log.ipynb 4
@@ -22,24 +22,24 @@
 # %% ../../nbs/routes/activity_log.ipynb 7
 async def search_activity_log(
     auth: dmda.DomoAuth,
     start_time: int,  # epoch time in milliseconds
     end_time: int,  # epoch time in milliseconds
     maximum: int,
     object_type: str = None,
-    session: aiohttp.ClientSession = None,
+    session: httpx.AsyncClient = None,
     debug_api: bool = False,
     debug_loop: bool = False,
 ) -> rgd.ResponseGetData:
     """loops over activity log api to retrieve audit logs"""
 
     is_close_session = False
 
     if not session:
-        session = aiohttp.ClientSession()
+        session = httpx.AsyncClient()
         is_close_session = True
 
     url = f"https://{auth.domo_instance}.domo.com/api/audit/v1/user-audits"
 
     if object_type and object_type != 'ACTIVITY_LOG':
         url = f"{url}/objectTypes/{object_type}"
 
@@ -63,11 +63,11 @@
         session=session,
         maximum=maximum,
         debug_loop=debug_loop,
         debug_api=debug_api,
     )
 
     if is_close_session:
-        await session.close()
+        await session.aclose()
 
     return res
```

### Comparing `domolibrary-0.0.8/domolibrary/routes/bootstrap.py` & `domolibrary-0.0.9/domolibrary/routes/bootstrap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/bootstrap.ipynb.
 
 # %% auto 0
 __all__ = ['GetBootstrap_InvalidAuthMethod', 'get_bootstrap', 'get_bootstrap_features', 'get_bootstrap_pages']
 
 # %% ../../nbs/routes/bootstrap.ipynb 3
-import aiohttp
-
 import httpx
 
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoAuth as dmda
 
 # %% ../../nbs/routes/bootstrap.ipynb 4
 class GetBootstrap_InvalidAuthMethod(Exception):
     def __init__(self, domo_instance):
         message = f"invalid auth method sent to {domo_instance} bootstrap API, use DomoFullAuth (username and password) authentication"
         super().__init__(message)
 
 async def get_bootstrap(
     auth: dmda.DomoFullAuth, ## only works with DomoFullAuth authentication, do not use TokenAuth
-    debug_api: bool = False, session: aiohttp.ClientSession = None
+    debug_api: bool = False, session: httpx.AsyncClient = None
 ) -> rgd.ResponseGetData:
     """get bootstrap data"""
 
     # url = f"https://{auth.domo_instance}.domo.com/api/domoweb/bootstrap?v2Navigation=false"
     url = f"https://{auth.domo_instance}.domo.com/api/domoweb/bootstrap?v2Navigation=true"
 
     res = await gd.get_data(
@@ -35,27 +33,27 @@
         raise GetBootstrap_InvalidAuthMethod(auth.domo_instance)
 
     return res
 
 
 # %% ../../nbs/routes/bootstrap.ipynb 8
 async def get_bootstrap_features(   
-    auth: dmda.DomoAuth, session: aiohttp.ClientSession = None, debug_api: bool = False
+    auth: dmda.DomoAuth, session: httpx.AsyncClient = None, debug_api: bool = False
 ) -> rgd.ResponseGetData:
     res = await get_bootstrap(auth=auth, session=session, debug_api=debug_api)
 
     if not res.is_success:
         return None
 
     res.response = res.response.get("data").get("features")
     return res
 
 # %% ../../nbs/routes/bootstrap.ipynb 11
 async def get_bootstrap_pages(
-    auth: dmda.DomoAuth, session: aiohttp.ClientSession = None, debug_api: bool = False
+    auth: dmda.DomoAuth, session: httpx.AsyncClient = None, debug_api: bool = False
 ) -> rgd.ResponseGetData:
     res = await get_bootstrap(auth=auth, session=session, debug_api=debug_api)
 
     if not res.is_success:
         return None
 
     res.response = res.response.get("data").get("pages")
```

### Comparing `domolibrary-0.0.8/domolibrary/routes/dataset.py` & `domolibrary-0.0.9/domolibrary/routes/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/dataset.ipynb.
 
 # %% auto 0
 __all__ = ['DatasetNotFoundError', 'QueryRequestError', 'query_dataset_public', 'query_dataset_private', 'get_dataset_by_id',
            'get_schema', 'set_dataset_tags', 'UploadDataError', 'upload_dataset_stage_1', 'upload_dataset_stage_2_file',
            'upload_dataset_stage_2_df', 'upload_dataset_stage_3', 'index_dataset', 'index_status',
-           'generate_list_partitions_body', 'list_partitions', 'generate_create_dataset_body', 'create']
+           'generate_list_partitions_body', 'list_partitions', 'generate_create_dataset_body', 'create', 'delete']
 
 # %% ../../nbs/routes/dataset.ipynb 3
 from typing import Optional
 
 import io
 import pandas as pd
 
-import aiohttp
+import httpx
 
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoAuth as dmda
 
 # %% ../../nbs/routes/dataset.ipynb 5
 class DatasetNotFoundError(Exception):
@@ -33,15 +33,15 @@
         super().__init__(message)
 
 # typically do not use
 async def query_dataset_public(
     dev_auth: dmda.DomoDeveloperAuth,
     dataset_id: str,
     sql: str,
-    session: aiohttp.ClientSession,
+    session: httpx.AsyncClient,
     debug_api: bool = False,
 ):
 
     """query for hitting public apis, requires client_id and secret authentication"""
 
     url = f"https://api.domo.com/v1/datasets/query/execute/{dataset_id}?IncludeHeaders=true"
 
@@ -52,15 +52,15 @@
         
 
         
 async def query_dataset_private(
     auth: dmda.DomoAuth,  # DomoFullAuth or DomoTokenAuth
     dataset_id: str,
     sql: str,
-    session: Optional[aiohttp.ClientSession] = None,
+    session: Optional[httpx.AsyncClient] = None,
     loop_until_end: bool = False,  # retrieve all available rows
     limit=100,  # maximum rows to return per request.  refers to PAGINATION
     skip=0,
     maximum=100,  # equivalent to the LIMIT or TOP clause in SQL, the number of rows to return total
     debug_api: bool = False,
     debug_loop: bool = False,
 ):
@@ -114,15 +114,15 @@
 
 
 # %% ../../nbs/routes/dataset.ipynb 9
 async def get_dataset_by_id(
     dataset_id: str, # dataset id from URL
     auth: Optional[dmda.DomoAuth] = None, # requires full authentication
     debug_api: bool = False, # for troubleshooting API request
-    session: Optional[aiohttp.ClientSession] = None
+    session: Optional[httpx.AsyncClient] = None
 ) -> rgd.ResponseGetData: # returns metadata about a dataset
     """retrieve dataset metadata"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}"
 
     res= await gd.get_data(
         auth=auth,
@@ -148,15 +148,15 @@
 
 
 # %% ../../nbs/routes/dataset.ipynb 16
 async def set_dataset_tags(auth: dmda.DomoFullAuth,
                            tag_ls: [str], # complete list of tags for dataset
                            dataset_id: str,
                            debug_api: bool = False,
-                           session: Optional[aiohttp.ClientSession] = None,
+                           session: Optional[httpx.AsyncClient] = None,
                            return_raw : bool = False
                            ):
     
     """REPLACE tags on this dataset with a new list"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/ui/v3/datasources/{dataset_id}/tags"
 
@@ -188,15 +188,15 @@
         super().__init__(message)
 
 # %% ../../nbs/routes/dataset.ipynb 20
 async def upload_dataset_stage_1(auth: dmda.DomoAuth,
                                  dataset_id: str,
                                  #  restate_data_tag: str = None, # deprecated
                                  partition_tag: str = None,  # synonymous with data_tag
-                                 session: Optional[aiohttp.ClientSession] = None,
+                                 session: Optional[httpx.AsyncClient] = None,
                                  debug_api: bool = False,
                                  ) -> rgd.ResponseGetData:
 
     """preps dataset for upload by creating an upload_id (upload session key) pass to stage 2 as a parameter"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}/uploads"
 
@@ -229,15 +229,15 @@
 
 # %% ../../nbs/routes/dataset.ipynb 21
 async def upload_dataset_stage_2_file(
     auth: dmda.DomoAuth,
     dataset_id: str,
     upload_id: str,  # must originate from  a stage_1 upload response
     data_file: Optional[io.TextIOWrapper] = None,
-    session: Optional[aiohttp.ClientSession] = None,
+    session: Optional[httpx.AsyncClient] = None,
     # only necessary if streaming multiple files into the same partition (multi-part upload)
     part_id: str = 2,
     debug_api: bool = False,
 ) -> rgd.ResponseGetData:
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}/uploads/{upload_id}/parts/{part_id}"
 
@@ -263,15 +263,15 @@
 
 # %% ../../nbs/routes/dataset.ipynb 22
 async def upload_dataset_stage_2_df(
     auth: dmda.DomoAuth,
     dataset_id: str,
     upload_id: str,  # must originate from  a stage_1 upload response
     upload_df: pd.DataFrame,
-    session: Optional[aiohttp.ClientSession] = None,
+    session: Optional[httpx.AsyncClient] = None,
     part_id: str = 2,  # only necessary if streaming multiple files into the same partition (multi-part upload)
     debug_api: bool = False,
 ) -> rgd.ResponseGetData:
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}/uploads/{upload_id}/parts/{part_id}"
 
     body = upload_df.to_csv(header=False, index=False)
@@ -299,15 +299,15 @@
     return res
 
 # %% ../../nbs/routes/dataset.ipynb 23
 async def upload_dataset_stage_3(
     auth: dmda.DomoAuth,
     dataset_id: str,
     upload_id: str,  # must originate from  a stage_1 upload response
-    session: Optional[aiohttp.ClientSession] = None,
+    session: Optional[httpx.AsyncClient] = None,
     update_method: str = "REPLACE",  # accepts REPLACE or APPEND
     #  restate_data_tag: str = None, # deprecated
     partition_tag: str = None,  # synonymous with data_tag
     is_index: bool = False,  # index after uploading
     debug_api: bool = False,
 ) -> rgd.ResponseGetData:
 
@@ -344,15 +344,15 @@
 
     return res
 
 # %% ../../nbs/routes/dataset.ipynb 24
 async def index_dataset(
     auth: dmda.DomoAuth,
     dataset_id: str,
-    session: Optional[aiohttp.ClientSession] = None,
+    session: Optional[httpx.AsyncClient] = None,
     debug_api: bool = False,
 ) -> rgd.ResponseGetData:
     """manually index a dataset"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}/indexes"
 
     body = {"dataIds": []}
@@ -362,15 +362,15 @@
     )
 
 # %% ../../nbs/routes/dataset.ipynb 25
 async def index_status(
     auth: dmda.DomoAuth,
     dataset_id: str,
     index_id: str,
-    session: Optional[aiohttp.ClientSession] = None,
+    session: Optional[httpx.AsyncClient] = None,
     debug_api: bool = False,
 ) -> rgd.ResponseGetData:
     """get the completion status of an index"""
 
     url = f"https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}/indexes/{index_id}/statuses"
 
     return await gd.get_data(
@@ -395,15 +395,15 @@
         "offset": 0
     }
 
 
 async def list_partitions(auth: dmda.DomoAuth,
                           dataset_id: str,
                           body: dict = None,
-                          session: aiohttp.ClientSession = None,
+                          session: httpx.AsyncClient = None,
                           debug_api: bool = False,
                           debug_loop: bool = False,
 
 
                           ):
 
     body = body or generate_list_partitions_body()
@@ -450,15 +450,15 @@
         "schema": schema
     }
 
 
 async def create(auth: dmda.DomoAuth,
                  dataset_name: str,
                  dataset_type: str = 'api',
-                 session: aiohttp.ClientSession = None,
+                 session: httpx.AsyncClient = None,
                  schema: dict = None,
                  debug_api: bool = False):
 
     body = generate_create_dataset_body(dataset_name=dataset_name,
                                         dataset_type=dataset_type,
                                         schema=schema)
 
@@ -469,7 +469,21 @@
         method="POST",
         url=url,
         body=body,
         session=session,
         debug_api=debug_api
     )
 
+
+# %% ../../nbs/routes/dataset.ipynb 34
+async def delete(auth: dmda.DomoAuth,
+                 dataset_id: str, session: httpx.AsyncClient = None, debug_api: bool = False):
+    url = f"https://{auth.domo_instance}.domo.com/api/data/v3/datasources/{dataset_id}?deleteMethod=hard"
+
+    return await gd.get_data(
+        auth=auth,
+        method="DELETE",
+        url=url,
+        session=session,
+        debug_api=debug_api
+    )
+
```

### Comparing `domolibrary-0.0.8/domolibrary/routes/user.py` & `domolibrary-0.0.9/domolibrary/routes/user.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/domolibrary/utils/DictDot.py` & `domolibrary-0.0.9/domolibrary/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/domolibrary/utils/convert.py` & `domolibrary-0.0.9/domolibrary/utils/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 # %% auto 0
 __all__ = ['convert_epoch_millisecond_to_datetime', 'convert_datetime_to_epoch_millisecond', 'convert_snake_to_pascal']
 
 # %% ../../nbs/utils/convert.ipynb 2
 import datetime as dt
 
-# %% ../../nbs/utils/convert.ipynb 3
-import fastcore.test as fctest
-
 # %% ../../nbs/utils/convert.ipynb 4
 def convert_epoch_millisecond_to_datetime(epoch: int):
     '''convert Epoch time with miliseconds to Date time'''
     return dt.datetime.fromtimestamp(epoch / 1000.0)
 
 # %% ../../nbs/utils/convert.ipynb 5
 def convert_datetime_to_epoch_millisecond(datetime: dt.datetime):
```

### Comparing `domolibrary-0.0.8/domolibrary.egg-info/PKG-INFO` & `domolibrary-0.0.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: domolibrary
-Version: 0.0.8
-Summary: UNKNOWN
-Home-page: https://github.com/jaewilson07/domo_library
-Author: Jae Wilson
-Author-email: jaewilson07@gmail.com
-License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 domolibrary: a powerful pydomo alternative
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## What is it?
 
@@ -49,21 +26,26 @@
 pip install domo_library
 ```
 
 ## How to use
 
 ### Authentication
 
-For each task, consider the appropriate `DomoAuth` mechanism. In most
-cases `DomoFullAuth` or `DomoTokenAuth` will be appropriate as this
-library predominately accesses private APIs.
+For each task, consider the appropriate
+[`DomoAuth`](https://jaewilson07.github.io/domo_library/client/domoauth.html#domoauth)
+mechanism. In most cases
+[`DomoFullAuth`](https://jaewilson07.github.io/domo_library/client/domoauth.html#domofullauth)
+or
+[`DomoTokenAuth`](https://jaewilson07.github.io/domo_library/client/domoauth.html#domotokenauth)
+will be appropriate as this library predominately accesses private APIs.
 
 Any Public routes or methods will be labeled appropriately in which case
-you should use `DomoDeveloperAuth`. Public routes are APIs enumerated
-and documented under
+you should use
+[`DomoDeveloperAuth`](https://jaewilson07.github.io/domo_library/client/domoauth.html#domodeveloperauth).
+Public routes are APIs enumerated and documented under
 <a href = "https://developer.domo.com/" target="_blank">Developer.Domo.com</a>.
 
 Typically each project will begin with configuring an auth object. If
 you are accessing multiple Domo instances, you’ll probably need multiple
 auth objects.
 
 ``` python
@@ -72,59 +54,62 @@
 import domolibrary.client.DomoAuth as dmda
 
 token_auth = dmda.DomoTokenAuth( domo_instance = 'domo-dojoo', domo_access_token = os.environ['DOMO_DOJO_ACCESS_TOKEN'])
 ```
 
 ### Option 1: class based programming
 
-In this project domo entities, `DomoActivityLog`, `DomoDataset` are all
-prefixed ‘Domo’ and can be found in the `classes` folder. Each class
-method will call one or more `routes`. Each route will interact with one
-and only one API.
+In this project domo entities,
+[`DomoActivityLog`](https://jaewilson07.github.io/domo_library/classes/domoactivitylog.html#domoactivitylog),
+[`DomoDataset`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset)
+are all prefixed ‘Domo’ and can be found in the `classes` folder. Each
+class method will call one or more `routes`. Each route will interact
+with one and only one API.
 
 Although most methods will be standard methods that will be called after
 creating an instance of the class, some methods will be classmethods
 which return an instance of the class.
 
-In the example below, `DomoDataset.get_from_id` is a classmethod.
+In the example below,
+[`DomoDataset.get_from_id`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset.get_from_id)
+is a classmethod.
 
 Note: DomoLibrary uses the asynchronous `aiohttp` requests library to
 offer users the ability to write concurrently executing code.
 
 ``` python
 import domolibrary.classes.DomoDataset as dmds
 
 # this is a class method
 domo_ds = await dmds.DomoDataset.get_from_id(auth = token_auth, dataset_id = os.environ['DOJO_DATASET_ID'])
 domo_ds
 ```
 
-    _from_httpx_response <Response [200 OK]>
-    ResponseGetData(status=200, response={'id': '04c1574e-c8be-4721-9846-c6ffa491144b', 'displayType': 'domo-jupyterdata', 'dataProviderType': 'domo-jupyterdata', 'type': 'Jupyter', 'name': 'domo_kbs', 'owner': {'id': '1893952720', 'name': 'Jae Wilson', 'type': 'USER', 'group': False}, 'status': 'SUCCESS', 'created': 1668379680000, 'lastTouched': 1668385822000, 'lastUpdated': 1668385822045, 'rowCount': 1185, 'columnCount': 7, 'cardInfo': {'cardCount': 0, 'cardViewCount': 0}, 'properties': {'formulas': {'formulas': {}}}, 'state': 'SUCCESS', 'validConfiguration': True, 'validAccount': True, 'streamId': 825, 'transportType': 'API', 'adc': False, 'adcExternal': False, 'cloudId': 'domo', 'cloudName': 'Domo', 'permissions': 'READ_WRITE_DELETE_SHARE_ADMIN', 'hidden': False, 'tags': '["developer_documentation","hackercore"]', 'scheduleActive': True, 'cryoStatus': 'ADRENALINE'}, is_success=True)
-
     DomoDataset(id='04c1574e-c8be-4721-9846-c6ffa491144b', display_type='domo-jupyterdata', data_provider_type='domo-jupyterdata', name='domo_kbs', description=None, row_count=1185, column_count=7, stream_id=825, owner=DictDot(id='1893952720', name='Jae Wilson', type='USER', group=False), formula=DictDot(), schema=DomoDataset_Schema(dataset=..., columns=[]))
 
 Once instantiated, you can call methods to interact with that object.
 You typically won’t have to pass auth creds again because they are saved
 to the object.
 
-In the example below we are retrieving the `DomoDataset_Schema` which
-consists of subclass `DomoDataset_Schema_Column` using the
-`DomoDataset_Schema.get` method.
+In the example below we are retrieving the
+[`DomoDataset_Schema`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset_schema)
+which consists of subclass
+[`DomoDataset_Schema_Column`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset_schema_column)
+using the
+[`DomoDataset_Schema.get`](https://jaewilson07.github.io/domo_library/classes/domodataset.html#domodataset_schema.get)
+method.
 
 We take the approach of where possible converting dictionaries from Domo
 APIs into classes because it provides greater predictability when users
 are creating integrations between platforms (ex. Domo to Trello).
 
 ``` python
 await domo_ds.schema.get()
 ```
 
-    _from_httpx_response <Response [200 OK]>
-
     [DomoDataset_Schema_Column(name='objectID', id='objectID', type='STRING'),
      DomoDataset_Schema_Column(name='url', id='url', type='STRING'),
      DomoDataset_Schema_Column(name='Title', id='Title', type='STRING'),
      DomoDataset_Schema_Column(name='article', id='article', type='STRING'),
      DomoDataset_Schema_Column(name='views', id='views', type='LONG'),
      DomoDataset_Schema_Column(name='created_dt', id='created_dt', type='DATETIME'),
      DomoDataset_Schema_Column(name='published_dt', id='published_dt', type='DATETIME')]
@@ -153,33 +138,35 @@
 
 ### Option 2 functional programming
 
 Although classes add a pretty wrapper for interacting with Domo APIs,
 users can opt to interact directly with APIs by way of `routes`.
 
 All route functions will exclusively call one API and will always return
-a `ResponseGetData` object OR raise an `Exception` if appropriate.
+a
+[`ResponseGetData`](https://jaewilson07.github.io/domo_library/client/responsegetdata.html#responsegetdata)
+object OR raise an `Exception` if appropriate.
 
 For example we can implement similar functionality as the Option 1
-example by calling the `get_dataset_by_id` function.
+example by calling the
+[`get_dataset_by_id`](https://jaewilson07.github.io/domo_library/routes/dataset.html#get_dataset_by_id)
+function.
 
 ``` python
 import domolibrary.routes.dataset as dataset_routes
 
 ds_res = await dataset_routes.get_dataset_by_id( auth = token_auth, dataset_id = os.environ['DOJO_DATASET_ID'])
 ds_res
 ```
 
-    _from_httpx_response <Response [200 OK]>
     ResponseGetData(status=200, response={'id': '04c1574e-c8be-4721-9846-c6ffa491144b', 'displayType': 'domo-jupyterdata', 'dataProviderType': 'domo-jupyterdata', 'type': 'Jupyter', 'name': 'domo_kbs', 'owner': {'id': '1893952720', 'name': 'Jae Wilson', 'type': 'USER', 'group': False}, 'status': 'SUCCESS', 'created': 1668379680000, 'lastTouched': 1668385822000, 'lastUpdated': 1668385822045, 'rowCount': 1185, 'columnCount': 7, 'cardInfo': {'cardCount': 0, 'cardViewCount': 0}, 'properties': {'formulas': {'formulas': {}}}, 'state': 'SUCCESS', 'validConfiguration': True, 'validAccount': True, 'streamId': 825, 'transportType': 'API', 'adc': False, 'adcExternal': False, 'cloudId': 'domo', 'cloudName': 'Domo', 'permissions': 'READ_WRITE_DELETE_SHARE_ADMIN', 'hidden': False, 'tags': '["developer_documentation","hackercore"]', 'scheduleActive': True, 'cryoStatus': 'ADRENALINE'}, is_success=True)
 
-    ResponseGetData(status=200, response={'id': '04c1574e-c8be-4721-9846-c6ffa491144b', 'displayType': 'domo-jupyterdata', 'dataProviderType': 'domo-jupyterdata', 'type': 'Jupyter', 'name': 'domo_kbs', 'owner': {'id': '1893952720', 'name': 'Jae Wilson', 'type': 'USER', 'group': False}, 'status': 'SUCCESS', 'created': 1668379680000, 'lastTouched': 1668385822000, 'lastUpdated': 1668385822045, 'rowCount': 1185, 'columnCount': 7, 'cardInfo': {'cardCount': 0, 'cardViewCount': 0}, 'properties': {'formulas': {'formulas': {}}}, 'state': 'SUCCESS', 'validConfiguration': True, 'validAccount': True, 'streamId': 825, 'transportType': 'API', 'adc': False, 'adcExternal': False, 'cloudId': 'domo', 'cloudName': 'Domo', 'permissions': 'READ_WRITE_DELETE_SHARE_ADMIN', 'hidden': False, 'tags': '["developer_documentation","hackercore"]', 'scheduleActive': True, 'cryoStatus': 'ADRENALINE'}, is_success=True)
-
-`ResponseGetData` will always include a boolean `is_success`, the API
-`status`, and raw API `response`.
+[`ResponseGetData`](https://jaewilson07.github.io/domo_library/client/responsegetdata.html#responsegetdata)
+will always include a boolean `is_success`, the API `status`, and raw
+API `response`.
 
 Typically the route methods will not alter the response unless the API
 does not include a descriptive response (ex,
 `routes.dataset.set_dataset_tags` does not return a response so we
 artificially alter the response in the function.)
 
 ``` python
@@ -229,13 +216,14 @@
      'cryoStatus': 'ADRENALINE'}
 
 ### Access Paginated APIs using the Looper
 
 A hidden advantage of using the DomoLibrary is that paginated API
 requests are baked into the route’s definition.
 
-Consider `query_dataset_private` from the `routes.dataset`.
-
-Inside this function we are using `looper` from `client.get_data` to
-paginate over the API response.
-
-
+Consider
+[`query_dataset_private`](https://jaewilson07.github.io/domo_library/routes/dataset.html#query_dataset_private)
+from the `routes.dataset`.
+
+Inside this function we are using
+[`looper`](https://jaewilson07.github.io/domo_library/client/get_data.html#looper)
+from `client.get_data` to paginate over the API response.
```

### Comparing `domolibrary-0.0.8/domolibrary.egg-info/SOURCES.txt` & `domolibrary-0.0.9/domolibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/settings.ini` & `domolibrary-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
```

### Comparing `domolibrary-0.0.8/setup.py` & `domolibrary-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/utils/Base.py` & `domolibrary-0.0.9/utils/Base.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/utils/DictDot.py` & `domolibrary-0.0.9/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/utils/Exceptions.py` & `domolibrary-0.0.9/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/utils/LoggerClass.py` & `domolibrary-0.0.9/utils/LoggerClass.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/utils/chunk_execution.py` & `domolibrary-0.0.9/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/utils/consol_get_creds.py` & `domolibrary-0.0.9/utils/consol_get_creds.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/utils/convert.py` & `domolibrary-0.0.9/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/utils/read_creds_from_dotenv.py` & `domolibrary-0.0.9/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.0.8/utils/upload_data.py` & `domolibrary-0.0.9/utils/upload_data.py`

 * *Files identical despite different names*

