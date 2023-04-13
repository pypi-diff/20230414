# Comparing `tmp/cbra-2.0.0a8.tar.gz` & `tmp/cbra-3.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbra-2.0.0a8.tar", last modified: Wed Mar  1 22:26:23 2023, max compression
+gzip compressed data, was "cbra-3.0.0a7.tar", last modified: Wed Mar  1 11:11:23 2023, max compression
```

## Comparing `cbra-2.0.0a8.tar` & `cbra-3.0.0a7.tar`

### file list

```diff
@@ -1,285 +1,284 @@
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.497236 cbra-2.0.0a8/
--rw-r--r--   0 cochise    (501) staff       (20)      348 2023-02-23 23:31:32.000000 cbra-2.0.0a8/MANIFEST.in
--rw-r--r--   0 cochise    (501) staff       (20)     1606 2023-03-01 22:26:23.497034 cbra-2.0.0a8/PKG-INFO
--rw-r--r--   0 cochise    (501) staff       (20)      667 2023-02-23 23:31:32.000000 cbra-2.0.0a8/README.md
--rw-r--r--   0 cochise    (501) staff       (20)       12 2023-03-01 22:26:19.000000 cbra-2.0.0a8/VERSION
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.454022 cbra-2.0.0a8/cbra/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.456405 cbra-2.0.0a8/cbra/core/
--rw-r--r--   0 cochise    (501) staff       (20)     3494 2023-02-28 17:21:37.000000 cbra-2.0.0a8/cbra/core/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     5775 2023-03-01 22:22:52.000000 cbra-2.0.0a8/cbra/core/application.py
--rw-r--r--   0 cochise    (501) staff       (20)    11405 2023-03-01 22:25:15.000000 cbra-2.0.0a8/cbra/core/conf.py
--rw-r--r--   0 cochise    (501) staff       (20)     2104 2023-02-28 17:15:47.000000 cbra-2.0.0a8/cbra/core/endpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     3293 2023-02-26 16:38:33.000000 cbra-2.0.0a8/cbra/core/endpointtype.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.457337 cbra-2.0.0a8/cbra/core/iam/
--rw-r--r--   0 cochise    (501) staff       (20)     5076 2023-02-26 14:40:20.000000 cbra-2.0.0a8/cbra/core/iam/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1040 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/iam/authenticatedcontext.py
--rw-r--r--   0 cochise    (501) staff       (20)     2899 2023-02-27 00:53:49.000000 cbra-2.0.0a8/cbra/core/iam/authenticationservice.py
--rw-r--r--   0 cochise    (501) staff       (20)     5337 2023-02-26 14:30:31.000000 cbra-2.0.0a8/cbra/core/iam/authorizationcontextfactory.py
--rw-r--r--   0 cochise    (501) staff       (20)     1164 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/iam/isubjectrepository.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.458132 cbra-2.0.0a8/cbra/core/iam/models/
--rw-r--r--   0 cochise    (501) staff       (20)      588 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/iam/models/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      978 2023-02-24 09:14:37.000000 cbra-2.0.0a8/cbra/core/iam/models/emailprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     1233 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/iam/models/externalprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     1996 2023-02-24 11:02:31.000000 cbra-2.0.0a8/cbra/core/iam/models/principal.py
--rw-r--r--   0 cochise    (501) staff       (20)      499 2023-02-24 09:14:50.000000 cbra-2.0.0a8/cbra/core/iam/models/principalmodel.py
--rw-r--r--   0 cochise    (501) staff       (20)     1117 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/iam/models/publicidentifierprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     2235 2023-02-24 11:35:17.000000 cbra-2.0.0a8/cbra/core/iam/models/subject.py
--rw-r--r--   0 cochise    (501) staff       (20)     2597 2023-02-25 11:57:16.000000 cbra-2.0.0a8/cbra/core/iam/principalhasher.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.458341 cbra-2.0.0a8/cbra/core/iam/services/
--rw-r--r--   0 cochise    (501) staff       (20)      669 2023-02-24 09:33:47.000000 cbra-2.0.0a8/cbra/core/iam/services/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     5165 2023-02-24 13:36:08.000000 cbra-2.0.0a8/cbra/core/iam/services/useronboarding.py
--rw-r--r--   0 cochise    (501) staff       (20)     1314 2023-02-26 14:42:54.000000 cbra-2.0.0a8/cbra/core/iam/subject.py
--rw-r--r--   0 cochise    (501) staff       (20)     2688 2023-02-26 14:28:24.000000 cbra-2.0.0a8/cbra/core/iam/subjectresolver.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.459534 cbra-2.0.0a8/cbra/core/iam/types/
--rw-r--r--   0 cochise    (501) staff       (20)      764 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/iam/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1015 2023-02-24 10:08:16.000000 cbra-2.0.0a8/cbra/core/iam/types/isubjectrepository.py
--rw-r--r--   0 cochise    (501) staff       (20)     1065 2023-02-24 10:06:00.000000 cbra-2.0.0a8/cbra/core/iam/types/iuseronboardingservice.py
--rw-r--r--   0 cochise    (501) staff       (20)      495 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/iam/types/principal.py
--rw-r--r--   0 cochise    (501) staff       (20)      294 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/iam/types/principaltype.py
--rw-r--r--   0 cochise    (501) staff       (20)      656 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/iam/types/publicidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      880 2023-02-24 11:10:55.000000 cbra-2.0.0a8/cbra/core/iam/types/subject.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.460802 cbra-2.0.0a8/cbra/core/ioc/
--rw-r--r--   0 cochise    (501) staff       (20)     1318 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/ioc/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      845 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/ioc/config.py
--rw-r--r--   0 cochise    (501) staff       (20)     1972 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/ioc/container.py
--rw-r--r--   0 cochise    (501) staff       (20)     1074 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/ioc/dependency.py
--rw-r--r--   0 cochise    (501) staff       (20)      476 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/ioc/dependencynotsatisfied.py
--rw-r--r--   0 cochise    (501) staff       (20)     1528 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/ioc/inheriteddependencydecorator.py
--rw-r--r--   0 cochise    (501) staff       (20)     1246 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/ioc/injected.py
--rw-r--r--   0 cochise    (501) staff       (20)      844 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/ioc/instance.py
--rw-r--r--   0 cochise    (501) staff       (20)     2225 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/ioc/loader.py
--rw-r--r--   0 cochise    (501) staff       (20)     1527 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/ioc/requirement.py
--rw-r--r--   0 cochise    (501) staff       (20)     1532 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/ioc/setting_.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.460906 cbra-2.0.0a8/cbra/core/ioc/test/
--rw-r--r--   0 cochise    (501) staff       (20)     1105 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/ioc/test/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      673 2023-02-28 17:24:40.000000 cbra-2.0.0a8/cbra/core/messagepublisher.py
--rw-r--r--   0 cochise    (501) staff       (20)     1237 2023-02-24 00:54:18.000000 cbra-2.0.0a8/cbra/core/optionsrequesthandler.py
--rw-r--r--   0 cochise    (501) staff       (20)     1605 2023-03-01 21:12:15.000000 cbra-2.0.0a8/cbra/core/package.json
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.461022 cbra-2.0.0a8/cbra/core/params/
--rw-r--r--   0 cochise    (501) staff       (20)      790 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/params/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)    16189 2023-03-01 11:06:07.000000 cbra-2.0.0a8/cbra/core/requesthandler.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.465239 cbra-2.0.0a8/cbra/core/resource/
--rw-r--r--   0 cochise    (501) staff       (20)     1120 2023-02-26 16:22:34.000000 cbra-2.0.0a8/cbra/core/resource/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1309 2023-02-26 16:27:20.000000 cbra-2.0.0a8/cbra/core/resource/collection.py
--rw-r--r--   0 cochise    (501) staff       (20)      701 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/collectionaction.py
--rw-r--r--   0 cochise    (501) staff       (20)     1321 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/create.py
--rw-r--r--   0 cochise    (501) staff       (20)     2169 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/createaction.py
--rw-r--r--   0 cochise    (501) staff       (20)     1655 2023-02-26 18:45:57.000000 cbra-2.0.0a8/cbra/core/resource/customaction.py
--rw-r--r--   0 cochise    (501) staff       (20)     1486 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/delete.py
--rw-r--r--   0 cochise    (501) staff       (20)     1506 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/deleteaction.py
--rw-r--r--   0 cochise    (501) staff       (20)      546 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/detail.py
--rw-r--r--   0 cochise    (501) staff       (20)     2448 2023-02-26 18:43:37.000000 cbra-2.0.0a8/cbra/core/resource/detailaction.py
--rw-r--r--   0 cochise    (501) staff       (20)      832 2023-02-26 16:34:31.000000 cbra-2.0.0a8/cbra/core/resource/iresource.py
--rw-r--r--   0 cochise    (501) staff       (20)      875 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/listaction.py
--rw-r--r--   0 cochise    (501) staff       (20)      711 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/persister.py
--rw-r--r--   0 cochise    (501) staff       (20)      740 2023-02-26 16:22:20.000000 cbra-2.0.0a8/cbra/core/resource/queryresult.py
--rw-r--r--   0 cochise    (501) staff       (20)      684 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/replace.py
--rw-r--r--   0 cochise    (501) staff       (20)     1093 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/replaceaction.py
--rw-r--r--   0 cochise    (501) staff       (20)     1687 2023-02-26 18:39:53.000000 cbra-2.0.0a8/cbra/core/resource/resource.py
--rw-r--r--   0 cochise    (501) staff       (20)     6201 2023-02-26 18:50:19.000000 cbra-2.0.0a8/cbra/core/resource/resourceaction.py
--rw-r--r--   0 cochise    (501) staff       (20)      901 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/resourceidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      670 2023-02-26 15:33:10.000000 cbra-2.0.0a8/cbra/core/resource/resourcelist.py
--rw-r--r--   0 cochise    (501) staff       (20)     1252 2023-02-26 15:23:44.000000 cbra-2.0.0a8/cbra/core/resource/resourcelistmetadata.py
--rw-r--r--   0 cochise    (501) staff       (20)     1304 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/resourcemodel.py
--rw-r--r--   0 cochise    (501) staff       (20)     5732 2023-02-26 15:17:35.000000 cbra-2.0.0a8/cbra/core/resource/resourcemodeltype.py
--rw-r--r--   0 cochise    (501) staff       (20)     1222 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/resourceoptionsrequesthandler.py
--rw-r--r--   0 cochise    (501) staff       (20)      506 2023-02-26 15:43:35.000000 cbra-2.0.0a8/cbra/core/resource/resourceprotocol.py
--rw-r--r--   0 cochise    (501) staff       (20)     4552 2023-02-26 18:40:03.000000 cbra-2.0.0a8/cbra/core/resource/resourcetype.py
--rw-r--r--   0 cochise    (501) staff       (20)      715 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/retrieve.py
--rw-r--r--   0 cochise    (501) staff       (20)      967 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/retrieveaction.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.465686 cbra-2.0.0a8/cbra/core/resource/test/
--rw-r--r--   0 cochise    (501) staff       (20)      519 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/test/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      698 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/test/book.py
--rw-r--r--   0 cochise    (501) staff       (20)      528 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/test/bookpublication.py
--rw-r--r--   0 cochise    (501) staff       (20)     1711 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/test/bookresource.py
--rw-r--r--   0 cochise    (501) staff       (20)     1512 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/update.py
--rw-r--r--   0 cochise    (501) staff       (20)     1090 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/updateaction.py
--rw-r--r--   0 cochise    (501) staff       (20)      546 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/resource/viewer.py
--rw-r--r--   0 cochise    (501) staff       (20)     2729 2023-02-27 00:53:17.000000 cbra-2.0.0a8/cbra/core/secretkey.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.465901 cbra-2.0.0a8/cbra/core/sessions/
--rw-r--r--   0 cochise    (501) staff       (20)      490 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/sessions/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     3275 2023-02-27 00:24:50.000000 cbra-2.0.0a8/cbra/core/sessions/requestsession.py
--rw-r--r--   0 cochise    (501) staff       (20)     1107 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/core/utils.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.451509 cbra-2.0.0a8/cbra/ext/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.469274 cbra-2.0.0a8/cbra/ext/google/
--rw-r--r--   0 cochise    (501) staff       (20)     3653 2023-02-28 17:26:30.000000 cbra-2.0.0a8/cbra/ext/google/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1695 2023-02-28 17:36:58.000000 cbra-2.0.0a8/cbra/ext/google/aortaendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)      504 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/ext/google/datastorecursor.py
--rw-r--r--   0 cochise    (501) staff       (20)      726 2023-02-26 16:25:00.000000 cbra-2.0.0a8/cbra/ext/google/datastorequeryresult.py
--rw-r--r--   0 cochise    (501) staff       (20)     7030 2023-02-26 16:51:13.000000 cbra-2.0.0a8/cbra/ext/google/datastorerepository.py
--rw-r--r--   0 cochise    (501) staff       (20)     4746 2023-02-26 14:42:12.000000 cbra-2.0.0a8/cbra/ext/google/datastoresubjectrepository.py
--rw-r--r--   0 cochise    (501) staff       (20)     1658 2023-02-26 14:44:09.000000 cbra-2.0.0a8/cbra/ext/google/datastoresubjectresolver.py
--rw-r--r--   0 cochise    (501) staff       (20)      666 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/ext/google/environ.py
--rw-r--r--   0 cochise    (501) staff       (20)     1689 2023-02-28 17:59:59.000000 cbra-2.0.0a8/cbra/ext/google/eventarcendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1837 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/ext/google/googleendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1294 2023-02-28 16:12:25.000000 cbra-2.0.0a8/cbra/ext/google/googlepubsubtransport.py
--rw-r--r--   0 cochise    (501) staff       (20)      591 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/ext/google/googleserviceaccountprincipal.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.451246 cbra-2.0.0a8/cbra/ext/google/impl/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.470088 cbra-2.0.0a8/cbra/ext/google/impl/oauth2/
--rw-r--r--   0 cochise    (501) staff       (20)      464 2023-02-25 23:31:32.000000 cbra-2.0.0a8/cbra/ext/google/impl/oauth2/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1026 2023-02-25 23:47:40.000000 cbra-2.0.0a8/cbra/ext/google/impl/oauth2/storage.py
--rw-r--r--   0 cochise    (501) staff       (20)     1021 2023-03-01 22:16:49.000000 cbra-2.0.0a8/cbra/ext/google/logging.py
--rw-r--r--   0 cochise    (501) staff       (20)      496 2023-02-28 17:35:28.000000 cbra-2.0.0a8/cbra/ext/google/messagediscarded.py
--rw-r--r--   0 cochise    (501) staff       (20)     1130 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/ext/google/messagepublished.py
--rw-r--r--   0 cochise    (501) staff       (20)     2852 2023-02-28 18:12:33.000000 cbra-2.0.0a8/cbra/ext/google/messagerunner.py
--rw-r--r--   0 cochise    (501) staff       (20)     3262 2023-02-28 15:37:54.000000 cbra-2.0.0a8/cbra/ext/google/pubsubmessage.py
--rw-r--r--   0 cochise    (501) staff       (20)      917 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/ext/google/resourcemetadata.py
--rw-r--r--   0 cochise    (501) staff       (20)      729 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/ext/google/runner.py
--rw-r--r--   0 cochise    (501) staff       (20)     2173 2023-03-01 22:10:32.000000 cbra-2.0.0a8/cbra/ext/google/service.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.470995 cbra-2.0.0a8/cbra/ext/oauth2/
--rw-r--r--   0 cochise    (501) staff       (20)     1157 2023-02-25 22:48:42.000000 cbra-2.0.0a8/cbra/ext/oauth2/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     4017 2023-02-25 23:48:33.000000 cbra-2.0.0a8/cbra/ext/oauth2/authorizationcodecallbackendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1551 2023-02-24 01:22:55.000000 cbra-2.0.0a8/cbra/ext/oauth2/authorizationendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1238 2023-02-25 23:46:59.000000 cbra-2.0.0a8/cbra/ext/oauth2/basestorage.py
--rw-r--r--   0 cochise    (501) staff       (20)     1459 2023-02-25 22:50:10.000000 cbra-2.0.0a8/cbra/ext/oauth2/endpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     4852 2023-02-26 13:22:04.000000 cbra-2.0.0a8/cbra/ext/oauth2/loginendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1511 2023-02-25 23:51:05.000000 cbra-2.0.0a8/cbra/ext/oauth2/memorystorage.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.471476 cbra-2.0.0a8/cbra/ext/oauth2/models/
--rw-r--r--   0 cochise    (501) staff       (20)      677 2023-02-25 23:27:34.000000 cbra-2.0.0a8/cbra/ext/oauth2/models/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      985 2023-02-24 02:23:22.000000 cbra-2.0.0a8/cbra/ext/oauth2/models/authorization.py
--rw-r--r--   0 cochise    (501) staff       (20)     1327 2023-02-25 23:34:52.000000 cbra-2.0.0a8/cbra/ext/oauth2/models/authorizationstate.py
--rw-r--r--   0 cochise    (501) staff       (20)      473 2023-02-25 23:27:21.000000 cbra-2.0.0a8/cbra/ext/oauth2/models/sector.py
--rw-r--r--   0 cochise    (501) staff       (20)     2163 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/ext/oauth2/oidcregistrationendpoint.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.473667 cbra-2.0.0a8/cbra/ext/oauth2/types/
--rw-r--r--   0 cochise    (501) staff       (20)     1379 2023-02-25 22:44:57.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      694 2023-02-24 01:40:14.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/authorizationlifecycle.py
--rw-r--r--   0 cochise    (501) staff       (20)     5357 2023-02-24 00:44:41.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/authorizationrequest.py
--rw-r--r--   0 cochise    (501) staff       (20)      483 2023-02-24 00:31:50.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/authorizationrequestobject.py
--rw-r--r--   0 cochise    (501) staff       (20)      490 2023-02-24 00:06:09.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/authorizationrequestreference.py
--rw-r--r--   0 cochise    (501) staff       (20)      590 2023-02-25 23:18:46.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/iauthorizationflowstate.py
--rw-r--r--   0 cochise    (501) staff       (20)      867 2023-02-25 23:46:40.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/iauthorizationserverstorage.py
--rw-r--r--   0 cochise    (501) staff       (20)      763 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/invalidauthorizeresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)      685 2023-02-25 23:04:12.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/jarmauthorizeresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)      702 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/loginresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)     1067 2023-02-25 23:16:14.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/queryauthorizeresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)     4139 2023-02-25 23:15:11.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/redirectparameters.py
--rw-r--r--   0 cochise    (501) staff       (20)     3014 2023-02-24 00:04:27.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/redirecturi.py
--rw-r--r--   0 cochise    (501) staff       (20)      774 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/responsemodenotsupported.py
--rw-r--r--   0 cochise    (501) staff       (20)      725 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/responsevalidationfailure.py
--rw-r--r--   0 cochise    (501) staff       (20)      752 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/ext/oauth2/types/unsupportedauthorizationresponse.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.474232 cbra-2.0.0a8/cbra/ext/picqer/
--rw-r--r--   0 cochise    (501) staff       (20)     1048 2023-02-25 04:58:32.000000 cbra-2.0.0a8/cbra/ext/picqer/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     4065 2023-02-25 11:25:08.000000 cbra-2.0.0a8/cbra/ext/picqer/picqerwebhookendpoint.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.474763 cbra-2.0.0a8/cbra/ext/picqer/v1/
--rw-r--r--   0 cochise    (501) staff       (20)      799 2023-02-28 19:39:45.000000 cbra-2.0.0a8/cbra/ext/picqer/v1/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1105 2023-02-25 04:17:59.000000 cbra-2.0.0a8/cbra/ext/picqer/v1/event.py
--rw-r--r--   0 cochise    (501) staff       (20)      700 2023-02-25 09:56:51.000000 cbra-2.0.0a8/cbra/ext/picqer/v1/orderevent.py
--rw-r--r--   0 cochise    (501) staff       (20)      717 2023-02-25 09:56:58.000000 cbra-2.0.0a8/cbra/ext/picqer/v1/picklistevent.py
--rw-r--r--   0 cochise    (501) staff       (20)      725 2023-02-28 19:39:23.000000 cbra-2.0.0a8/cbra/ext/picqer/v1/purchaseorderevent.py
--rw-r--r--   0 cochise    (501) staff       (20)      951 2023-02-25 01:54:30.000000 cbra-2.0.0a8/cbra/ext/picqer/webhookresponse.py
--rw-r--r--   0 cochise    (501) staff       (20)      901 2023-02-25 04:56:47.000000 cbra-2.0.0a8/cbra/ext/picqer/webhooksecret.py
--rw-r--r--   0 cochise    (501) staff       (20)     1622 2023-02-25 04:57:09.000000 cbra-2.0.0a8/cbra/ext/picqer/webhooksignature.py
--rw-r--r--   0 cochise    (501) staff       (20)     1000 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/package.json
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.483550 cbra-2.0.0a8/cbra/types/
--rw-r--r--   0 cochise    (501) staff       (20)     3660 2023-02-27 00:47:33.000000 cbra-2.0.0a8/cbra/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      911 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/abortable.py
--rw-r--r--   0 cochise    (501) staff       (20)     4141 2023-02-25 23:42:27.000000 cbra-2.0.0a8/cbra/types/basemodel.py
--rw-r--r--   0 cochise    (501) staff       (20)      518 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/conflict.py
--rw-r--r--   0 cochise    (501) staff       (20)      519 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/forbidden.py
--rw-r--r--   0 cochise    (501) staff       (20)      725 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/hints.py
--rw-r--r--   0 cochise    (501) staff       (20)      787 2023-02-27 00:52:53.000000 cbra-2.0.0a8/cbra/types/hmacsignature.py
--rw-r--r--   0 cochise    (501) staff       (20)     1666 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/httpheaderprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     1973 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/iauthorizationcontext.py
--rw-r--r--   0 cochise    (501) staff       (20)     1155 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/iauthorizationcontextfactory.py
--rw-r--r--   0 cochise    (501) staff       (20)      699 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/icredential.py
--rw-r--r--   0 cochise    (501) staff       (20)      877 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/icredentialverifier.py
--rw-r--r--   0 cochise    (501) staff       (20)      446 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/icursor.py
--rw-r--r--   0 cochise    (501) staff       (20)     1423 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/ideferred.py
--rw-r--r--   0 cochise    (501) staff       (20)     1414 2023-02-28 16:57:21.000000 cbra-2.0.0a8/cbra/types/idependant.py
--rw-r--r--   0 cochise    (501) staff       (20)     5648 2023-03-01 21:36:25.000000 cbra-2.0.0a8/cbra/types/iendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1792 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/ihashable.py
--rw-r--r--   0 cochise    (501) staff       (20)     1360 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/imodelrepository.py
--rw-r--r--   0 cochise    (501) staff       (20)      755 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/integerpathparameter.py
--rw-r--r--   0 cochise    (501) staff       (20)      581 2023-02-26 15:28:16.000000 cbra-2.0.0a8/cbra/types/iqueryresult.py
--rw-r--r--   0 cochise    (501) staff       (20)     3046 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/irequestprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)      673 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/irequestprincipalintrospecter.py
--rw-r--r--   0 cochise    (501) staff       (20)      677 2023-02-26 16:35:24.000000 cbra-2.0.0a8/cbra/types/iroutable.py
--rw-r--r--   0 cochise    (501) staff       (20)     1522 2023-02-27 00:35:48.000000 cbra-2.0.0a8/cbra/types/isessiondata.py
--rw-r--r--   0 cochise    (501) staff       (20)      608 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/isessionfactory.py
--rw-r--r--   0 cochise    (501) staff       (20)     1495 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/isessionmanager.py
--rw-r--r--   0 cochise    (501) staff       (20)     1074 2023-02-26 19:12:06.000000 cbra-2.0.0a8/cbra/types/isubject.py
--rw-r--r--   0 cochise    (501) staff       (20)      785 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/isubjectresolver.py
--rw-r--r--   0 cochise    (501) staff       (20)      675 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/jsonwebtoken.py
--rw-r--r--   0 cochise    (501) staff       (20)     1473 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/jsonwebtokenprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     1508 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/modelautoassignedidentity.py
--rw-r--r--   0 cochise    (501) staff       (20)     1525 2023-02-25 22:43:16.000000 cbra-2.0.0a8/cbra/types/modelidentity.py
--rw-r--r--   0 cochise    (501) staff       (20)     1600 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/mutablesignature.py
--rw-r--r--   0 cochise    (501) staff       (20)      523 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/notauthorized.py
--rw-r--r--   0 cochise    (501) staff       (20)      518 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/notfound.py
--rw-r--r--   0 cochise    (501) staff       (20)      644 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/nullrequestprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     1036 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/nullsubject.py
--rw-r--r--   0 cochise    (501) staff       (20)      713 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/nullsubjectesolver.py
--rw-r--r--   0 cochise    (501) staff       (20)     1806 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/oidcrequestprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)      845 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/opaquebearertokenprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     1280 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/operation.py
--rw-r--r--   0 cochise    (501) staff       (20)     1133 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/pathparameter.py
--rw-r--r--   0 cochise    (501) staff       (20)      844 2023-02-25 23:40:52.000000 cbra-2.0.0a8/cbra/types/persistedmodel.py
--rw-r--r--   0 cochise    (501) staff       (20)     1717 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/requestprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     1768 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/rfc9068requestprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)     2380 2023-02-27 00:36:50.000000 cbra-2.0.0a8/cbra/types/session.py
--rw-r--r--   0 cochise    (501) staff       (20)      618 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/sessionclaims.py
--rw-r--r--   0 cochise    (501) staff       (20)     1134 2023-02-27 00:36:57.000000 cbra-2.0.0a8/cbra/types/sessionmodel.py
--rw-r--r--   0 cochise    (501) staff       (20)     2090 2023-02-27 00:49:22.000000 cbra-2.0.0a8/cbra/types/sessionrequestprincipal.py
--rw-r--r--   0 cochise    (501) staff       (20)      753 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/stringpathparameter.py
--rw-r--r--   0 cochise    (501) staff       (20)      483 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/subjectidentifier.py
--rw-r--r--   0 cochise    (501) staff       (20)     1023 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/unauthenticatedauthorizationcontext.py
--rw-r--r--   0 cochise    (501) staff       (20)      800 2023-02-23 23:31:32.000000 cbra-2.0.0a8/cbra/types/uuidpathparameter.py
--rw-r--r--   0 cochise    (501) staff       (20)      564 2023-02-27 00:52:11.000000 cbra-2.0.0a8/cbra/types/verifier.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.454680 cbra-2.0.0a8/cbra.egg-info/
--rw-r--r--   0 cochise    (501) staff       (20)     1606 2023-03-01 22:26:23.000000 cbra-2.0.0a8/cbra.egg-info/PKG-INFO
--rw-r--r--   0 cochise    (501) staff       (20)     8062 2023-03-01 22:26:23.000000 cbra-2.0.0a8/cbra.egg-info/SOURCES.txt
--rw-r--r--   0 cochise    (501) staff       (20)        1 2023-03-01 22:26:23.000000 cbra-2.0.0a8/cbra.egg-info/dependency_links.txt
--rw-r--r--   0 cochise    (501) staff       (20)      117 2023-03-01 22:26:23.000000 cbra-2.0.0a8/cbra.egg-info/entry_points.txt
--rw-r--r--   0 cochise    (501) staff       (20)      341 2023-03-01 22:26:23.000000 cbra-2.0.0a8/cbra.egg-info/requires.txt
--rw-r--r--   0 cochise    (501) staff       (20)       54 2023-03-01 22:26:23.000000 cbra-2.0.0a8/cbra.egg-info/top_level.txt
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.452244 cbra-2.0.0a8/docs/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.483675 cbra-2.0.0a8/docs/source/
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.483963 cbra-2.0.0a8/docs/source/_ext/
--rw-r--r--   0 cochise    (501) staff       (20)    15901 2023-02-23 23:31:32.000000 cbra-2.0.0a8/docs/source/_ext/djangodocs.py
--rw-r--r--   0 cochise    (501) staff       (20)     2934 2023-02-23 23:31:32.000000 cbra-2.0.0a8/docs/source/conf.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.489395 cbra-2.0.0a8/examples/
--rw-r--r--   0 cochise    (501) staff       (20)      904 2023-02-23 23:31:32.000000 cbra-2.0.0a8/examples/authentication.py
--rw-r--r--   0 cochise    (501) staff       (20)     1631 2023-02-23 23:31:32.000000 cbra-2.0.0a8/examples/dependency-injection.py
--rw-r--r--   0 cochise    (501) staff       (20)      754 2023-02-23 23:31:32.000000 cbra-2.0.0a8/examples/endpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1029 2023-02-23 23:31:32.000000 cbra-2.0.0a8/examples/fastapi-authentication.py
--rw-r--r--   0 cochise    (501) staff       (20)      557 2023-02-23 23:31:32.000000 cbra-2.0.0a8/examples/google-cloud-platform.py
--rw-r--r--   0 cochise    (501) staff       (20)     1673 2023-02-23 18:20:54.000000 cbra-2.0.0a8/examples/oauth2-callback-google.py
--rw-r--r--   0 cochise    (501) staff       (20)      677 2023-02-24 00:39:57.000000 cbra-2.0.0a8/examples/oauth2-server.py
--rw-r--r--   0 cochise    (501) staff       (20)     1387 2023-02-25 05:00:28.000000 cbra-2.0.0a8/examples/picqer-webhook.py
--rw-r--r--   0 cochise    (501) staff       (20)     2128 2023-02-23 23:31:32.000000 cbra-2.0.0a8/examples/resource.py
--rw-r--r--   0 cochise    (501) staff       (20)      899 2023-02-23 23:31:32.000000 cbra-2.0.0a8/examples/session.py
--rw-r--r--   0 cochise    (501) staff       (20)       38 2023-03-01 22:26:23.497288 cbra-2.0.0a8/setup.cfg
--rw-r--r--   0 cochise    (501) staff       (20)     1280 2023-02-23 23:31:32.000000 cbra-2.0.0a8/setup.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.492647 cbra-2.0.0a8/tests/
--rw-r--r--   0 cochise    (501) staff       (20)      399 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      550 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/conftest.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.492941 cbra-2.0.0a8/tests/core/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/core/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.493041 cbra-2.0.0a8/tests/core/iam/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/core/iam/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.493249 cbra-2.0.0a8/tests/core/iam/models/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/core/iam/models/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2695 2023-02-24 11:07:32.000000 cbra-2.0.0a8/tests/core/iam/models/test_unit_subject.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.493647 cbra-2.0.0a8/tests/ext/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/ext/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.494068 cbra-2.0.0a8/tests/ext/google/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/ext/google/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.494674 cbra-2.0.0a8/tests/ext/google/system/
--rw-r--r--   0 cochise    (501) staff       (20)     1339 2023-02-25 04:00:03.000000 cbra-2.0.0a8/tests/ext/google/system/conftest.py
--rw-r--r--   0 cochise    (501) staff       (20)     2387 2023-02-28 17:14:16.000000 cbra-2.0.0a8/tests/ext/google/system/test_system_googleendpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1928 2023-02-28 18:14:15.000000 cbra-2.0.0a8/tests/ext/google/test_integration_aorta.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.495091 cbra-2.0.0a8/tests/ext/oauth2/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/ext/oauth2/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     2267 2023-02-23 23:48:41.000000 cbra-2.0.0a8/tests/ext/oauth2/test_unit_redirecturi.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.495702 cbra-2.0.0a8/tests/ext/picqer/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-25 03:36:34.000000 cbra-2.0.0a8/tests/ext/picqer/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     3876 2023-02-25 04:58:38.000000 cbra-2.0.0a8/tests/ext/picqer/test_unit_signature.py
--rw-r--r--   0 cochise    (501) staff       (20)     3599 2023-03-01 11:10:13.000000 cbra-2.0.0a8/tests/test_unit_endpoint.py
--rw-r--r--   0 cochise    (501) staff       (20)     1465 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/test_unit_endpoint_authentication.py
--rw-r--r--   0 cochise    (501) staff       (20)      399 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/test_unit_ioc.py
--rw-r--r--   0 cochise    (501) staff       (20)     4480 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/test_unit_principal.py
--rw-r--r--   0 cochise    (501) staff       (20)     3162 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/test_unit_resource.py
--rw-r--r--   0 cochise    (501) staff       (20)     4380 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/test_unit_session.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 22:26:23.496648 cbra-2.0.0a8/tests/types/
--rw-r--r--   0 cochise    (501) staff       (20)      394 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/types/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     4378 2023-02-23 23:31:32.000000 cbra-2.0.0a8/tests/types/test_unit_basemodel_identity.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.128428 cbra-3.0.0a7/
+-rw-r--r--   0 cochise    (501) staff       (20)      348 2023-02-23 23:31:32.000000 cbra-3.0.0a7/MANIFEST.in
+-rw-r--r--   0 cochise    (501) staff       (20)     1606 2023-03-01 11:11:23.128244 cbra-3.0.0a7/PKG-INFO
+-rw-r--r--   0 cochise    (501) staff       (20)      667 2023-02-23 23:31:32.000000 cbra-3.0.0a7/README.md
+-rw-r--r--   0 cochise    (501) staff       (20)       12 2023-03-01 11:11:07.000000 cbra-3.0.0a7/VERSION
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.097025 cbra-3.0.0a7/cbra/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.099274 cbra-3.0.0a7/cbra/core/
+-rw-r--r--   0 cochise    (501) staff       (20)     3494 2023-02-28 17:21:37.000000 cbra-3.0.0a7/cbra/core/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5199 2023-02-28 17:24:16.000000 cbra-3.0.0a7/cbra/core/application.py
+-rw-r--r--   0 cochise    (501) staff       (20)     9725 2023-02-27 00:14:50.000000 cbra-3.0.0a7/cbra/core/conf.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2104 2023-02-28 17:15:47.000000 cbra-3.0.0a7/cbra/core/endpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3293 2023-02-26 16:38:33.000000 cbra-3.0.0a7/cbra/core/endpointtype.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.100169 cbra-3.0.0a7/cbra/core/iam/
+-rw-r--r--   0 cochise    (501) staff       (20)     5076 2023-02-26 14:40:20.000000 cbra-3.0.0a7/cbra/core/iam/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1040 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/authenticatedcontext.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2899 2023-02-27 00:53:49.000000 cbra-3.0.0a7/cbra/core/iam/authenticationservice.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5337 2023-02-26 14:30:31.000000 cbra-3.0.0a7/cbra/core/iam/authorizationcontextfactory.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1164 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/isubjectrepository.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.100995 cbra-3.0.0a7/cbra/core/iam/models/
+-rw-r--r--   0 cochise    (501) staff       (20)      588 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/models/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      978 2023-02-24 09:14:37.000000 cbra-3.0.0a7/cbra/core/iam/models/emailprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1233 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/models/externalprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1996 2023-02-24 11:02:31.000000 cbra-3.0.0a7/cbra/core/iam/models/principal.py
+-rw-r--r--   0 cochise    (501) staff       (20)      499 2023-02-24 09:14:50.000000 cbra-3.0.0a7/cbra/core/iam/models/principalmodel.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1117 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/models/publicidentifierprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2235 2023-02-24 11:35:17.000000 cbra-3.0.0a7/cbra/core/iam/models/subject.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2597 2023-02-25 11:57:16.000000 cbra-3.0.0a7/cbra/core/iam/principalhasher.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.101245 cbra-3.0.0a7/cbra/core/iam/services/
+-rw-r--r--   0 cochise    (501) staff       (20)      669 2023-02-24 09:33:47.000000 cbra-3.0.0a7/cbra/core/iam/services/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5165 2023-02-24 13:36:08.000000 cbra-3.0.0a7/cbra/core/iam/services/useronboarding.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1314 2023-02-26 14:42:54.000000 cbra-3.0.0a7/cbra/core/iam/subject.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2688 2023-02-26 14:28:24.000000 cbra-3.0.0a7/cbra/core/iam/subjectresolver.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.102096 cbra-3.0.0a7/cbra/core/iam/types/
+-rw-r--r--   0 cochise    (501) staff       (20)      764 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1015 2023-02-24 10:08:16.000000 cbra-3.0.0a7/cbra/core/iam/types/isubjectrepository.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1065 2023-02-24 10:06:00.000000 cbra-3.0.0a7/cbra/core/iam/types/iuseronboardingservice.py
+-rw-r--r--   0 cochise    (501) staff       (20)      495 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/types/principal.py
+-rw-r--r--   0 cochise    (501) staff       (20)      294 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/types/principaltype.py
+-rw-r--r--   0 cochise    (501) staff       (20)      656 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/iam/types/publicidentifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)      880 2023-02-24 11:10:55.000000 cbra-3.0.0a7/cbra/core/iam/types/subject.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.103277 cbra-3.0.0a7/cbra/core/ioc/
+-rw-r--r--   0 cochise    (501) staff       (20)     1318 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      845 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/config.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1972 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/container.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1074 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/dependency.py
+-rw-r--r--   0 cochise    (501) staff       (20)      476 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/dependencynotsatisfied.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1528 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/inheriteddependencydecorator.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1246 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/injected.py
+-rw-r--r--   0 cochise    (501) staff       (20)      844 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/instance.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2225 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/loader.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1527 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/requirement.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1532 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/setting_.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.103383 cbra-3.0.0a7/cbra/core/ioc/test/
+-rw-r--r--   0 cochise    (501) staff       (20)     1105 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/ioc/test/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      673 2023-02-28 17:24:40.000000 cbra-3.0.0a7/cbra/core/messagepublisher.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1237 2023-02-24 00:54:18.000000 cbra-3.0.0a7/cbra/core/optionsrequesthandler.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1527 2023-02-28 18:16:08.000000 cbra-3.0.0a7/cbra/core/package.json
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.103588 cbra-3.0.0a7/cbra/core/params/
+-rw-r--r--   0 cochise    (501) staff       (20)      790 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/params/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)    16189 2023-03-01 11:06:07.000000 cbra-3.0.0a7/cbra/core/requesthandler.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.107881 cbra-3.0.0a7/cbra/core/resource/
+-rw-r--r--   0 cochise    (501) staff       (20)     1120 2023-02-26 16:22:34.000000 cbra-3.0.0a7/cbra/core/resource/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1309 2023-02-26 16:27:20.000000 cbra-3.0.0a7/cbra/core/resource/collection.py
+-rw-r--r--   0 cochise    (501) staff       (20)      701 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/collectionaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1321 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/create.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2169 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/createaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1655 2023-02-26 18:45:57.000000 cbra-3.0.0a7/cbra/core/resource/customaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1486 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/delete.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1506 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/deleteaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)      546 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/detail.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2448 2023-02-26 18:43:37.000000 cbra-3.0.0a7/cbra/core/resource/detailaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)      832 2023-02-26 16:34:31.000000 cbra-3.0.0a7/cbra/core/resource/iresource.py
+-rw-r--r--   0 cochise    (501) staff       (20)      875 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/listaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)      711 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/persister.py
+-rw-r--r--   0 cochise    (501) staff       (20)      740 2023-02-26 16:22:20.000000 cbra-3.0.0a7/cbra/core/resource/queryresult.py
+-rw-r--r--   0 cochise    (501) staff       (20)      684 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/replace.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1093 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/replaceaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1687 2023-02-26 18:39:53.000000 cbra-3.0.0a7/cbra/core/resource/resource.py
+-rw-r--r--   0 cochise    (501) staff       (20)     6201 2023-02-26 18:50:19.000000 cbra-3.0.0a7/cbra/core/resource/resourceaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)      901 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/resourceidentifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)      670 2023-02-26 15:33:10.000000 cbra-3.0.0a7/cbra/core/resource/resourcelist.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1252 2023-02-26 15:23:44.000000 cbra-3.0.0a7/cbra/core/resource/resourcelistmetadata.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1304 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/resourcemodel.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5732 2023-02-26 15:17:35.000000 cbra-3.0.0a7/cbra/core/resource/resourcemodeltype.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1222 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/resourceoptionsrequesthandler.py
+-rw-r--r--   0 cochise    (501) staff       (20)      506 2023-02-26 15:43:35.000000 cbra-3.0.0a7/cbra/core/resource/resourceprotocol.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4552 2023-02-26 18:40:03.000000 cbra-3.0.0a7/cbra/core/resource/resourcetype.py
+-rw-r--r--   0 cochise    (501) staff       (20)      715 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/retrieve.py
+-rw-r--r--   0 cochise    (501) staff       (20)      967 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/retrieveaction.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.108457 cbra-3.0.0a7/cbra/core/resource/test/
+-rw-r--r--   0 cochise    (501) staff       (20)      519 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/test/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      698 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/test/book.py
+-rw-r--r--   0 cochise    (501) staff       (20)      528 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/test/bookpublication.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1711 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/test/bookresource.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1512 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/update.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1090 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/updateaction.py
+-rw-r--r--   0 cochise    (501) staff       (20)      546 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/resource/viewer.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2729 2023-02-27 00:53:17.000000 cbra-3.0.0a7/cbra/core/secretkey.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.109571 cbra-3.0.0a7/cbra/core/sessions/
+-rw-r--r--   0 cochise    (501) staff       (20)      490 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/sessions/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3275 2023-02-27 00:24:50.000000 cbra-3.0.0a7/cbra/core/sessions/requestsession.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1107 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/core/utils.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.095348 cbra-3.0.0a7/cbra/ext/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.112506 cbra-3.0.0a7/cbra/ext/google/
+-rw-r--r--   0 cochise    (501) staff       (20)     3653 2023-02-28 17:26:30.000000 cbra-3.0.0a7/cbra/ext/google/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1695 2023-02-28 17:36:58.000000 cbra-3.0.0a7/cbra/ext/google/aortaendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)      504 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/datastorecursor.py
+-rw-r--r--   0 cochise    (501) staff       (20)      726 2023-02-26 16:25:00.000000 cbra-3.0.0a7/cbra/ext/google/datastorequeryresult.py
+-rw-r--r--   0 cochise    (501) staff       (20)     7030 2023-02-26 16:51:13.000000 cbra-3.0.0a7/cbra/ext/google/datastorerepository.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4746 2023-02-26 14:42:12.000000 cbra-3.0.0a7/cbra/ext/google/datastoresubjectrepository.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1658 2023-02-26 14:44:09.000000 cbra-3.0.0a7/cbra/ext/google/datastoresubjectresolver.py
+-rw-r--r--   0 cochise    (501) staff       (20)      666 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/environ.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1689 2023-02-28 17:59:59.000000 cbra-3.0.0a7/cbra/ext/google/eventarcendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1837 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/googleendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1294 2023-02-28 16:12:25.000000 cbra-3.0.0a7/cbra/ext/google/googlepubsubtransport.py
+-rw-r--r--   0 cochise    (501) staff       (20)      591 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/googleserviceaccountprincipal.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.095097 cbra-3.0.0a7/cbra/ext/google/impl/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.112767 cbra-3.0.0a7/cbra/ext/google/impl/oauth2/
+-rw-r--r--   0 cochise    (501) staff       (20)      464 2023-02-25 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/impl/oauth2/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1026 2023-02-25 23:47:40.000000 cbra-3.0.0a7/cbra/ext/google/impl/oauth2/storage.py
+-rw-r--r--   0 cochise    (501) staff       (20)      496 2023-02-28 17:35:28.000000 cbra-3.0.0a7/cbra/ext/google/messagediscarded.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1130 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/messagepublished.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2852 2023-02-28 18:12:33.000000 cbra-3.0.0a7/cbra/ext/google/messagerunner.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3262 2023-02-28 15:37:54.000000 cbra-3.0.0a7/cbra/ext/google/pubsubmessage.py
+-rw-r--r--   0 cochise    (501) staff       (20)      917 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/resourcemetadata.py
+-rw-r--r--   0 cochise    (501) staff       (20)      729 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/runner.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1547 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/google/service.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.113675 cbra-3.0.0a7/cbra/ext/oauth2/
+-rw-r--r--   0 cochise    (501) staff       (20)     1157 2023-02-25 22:48:42.000000 cbra-3.0.0a7/cbra/ext/oauth2/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4017 2023-02-25 23:48:33.000000 cbra-3.0.0a7/cbra/ext/oauth2/authorizationcodecallbackendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1551 2023-02-24 01:22:55.000000 cbra-3.0.0a7/cbra/ext/oauth2/authorizationendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1238 2023-02-25 23:46:59.000000 cbra-3.0.0a7/cbra/ext/oauth2/basestorage.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1459 2023-02-25 22:50:10.000000 cbra-3.0.0a7/cbra/ext/oauth2/endpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4852 2023-02-26 13:22:04.000000 cbra-3.0.0a7/cbra/ext/oauth2/loginendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1511 2023-02-25 23:51:05.000000 cbra-3.0.0a7/cbra/ext/oauth2/memorystorage.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.114099 cbra-3.0.0a7/cbra/ext/oauth2/models/
+-rw-r--r--   0 cochise    (501) staff       (20)      677 2023-02-25 23:27:34.000000 cbra-3.0.0a7/cbra/ext/oauth2/models/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      985 2023-02-24 02:23:22.000000 cbra-3.0.0a7/cbra/ext/oauth2/models/authorization.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1327 2023-02-25 23:34:52.000000 cbra-3.0.0a7/cbra/ext/oauth2/models/authorizationstate.py
+-rw-r--r--   0 cochise    (501) staff       (20)      473 2023-02-25 23:27:21.000000 cbra-3.0.0a7/cbra/ext/oauth2/models/sector.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2163 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/oauth2/oidcregistrationendpoint.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.115811 cbra-3.0.0a7/cbra/ext/oauth2/types/
+-rw-r--r--   0 cochise    (501) staff       (20)     1379 2023-02-25 22:44:57.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      694 2023-02-24 01:40:14.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/authorizationlifecycle.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5357 2023-02-24 00:44:41.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/authorizationrequest.py
+-rw-r--r--   0 cochise    (501) staff       (20)      483 2023-02-24 00:31:50.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/authorizationrequestobject.py
+-rw-r--r--   0 cochise    (501) staff       (20)      490 2023-02-24 00:06:09.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/authorizationrequestreference.py
+-rw-r--r--   0 cochise    (501) staff       (20)      590 2023-02-25 23:18:46.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/iauthorizationflowstate.py
+-rw-r--r--   0 cochise    (501) staff       (20)      867 2023-02-25 23:46:40.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/iauthorizationserverstorage.py
+-rw-r--r--   0 cochise    (501) staff       (20)      763 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/invalidauthorizeresponse.py
+-rw-r--r--   0 cochise    (501) staff       (20)      685 2023-02-25 23:04:12.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/jarmauthorizeresponse.py
+-rw-r--r--   0 cochise    (501) staff       (20)      702 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/loginresponse.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1067 2023-02-25 23:16:14.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/queryauthorizeresponse.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4139 2023-02-25 23:15:11.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/redirectparameters.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3014 2023-02-24 00:04:27.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/redirecturi.py
+-rw-r--r--   0 cochise    (501) staff       (20)      774 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/responsemodenotsupported.py
+-rw-r--r--   0 cochise    (501) staff       (20)      725 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/responsevalidationfailure.py
+-rw-r--r--   0 cochise    (501) staff       (20)      752 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/ext/oauth2/types/unsupportedauthorizationresponse.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.116325 cbra-3.0.0a7/cbra/ext/picqer/
+-rw-r--r--   0 cochise    (501) staff       (20)     1048 2023-02-25 04:58:32.000000 cbra-3.0.0a7/cbra/ext/picqer/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4065 2023-02-25 11:25:08.000000 cbra-3.0.0a7/cbra/ext/picqer/picqerwebhookendpoint.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.116856 cbra-3.0.0a7/cbra/ext/picqer/v1/
+-rw-r--r--   0 cochise    (501) staff       (20)      799 2023-02-28 19:39:45.000000 cbra-3.0.0a7/cbra/ext/picqer/v1/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1105 2023-02-25 04:17:59.000000 cbra-3.0.0a7/cbra/ext/picqer/v1/event.py
+-rw-r--r--   0 cochise    (501) staff       (20)      700 2023-02-25 09:56:51.000000 cbra-3.0.0a7/cbra/ext/picqer/v1/orderevent.py
+-rw-r--r--   0 cochise    (501) staff       (20)      717 2023-02-25 09:56:58.000000 cbra-3.0.0a7/cbra/ext/picqer/v1/picklistevent.py
+-rw-r--r--   0 cochise    (501) staff       (20)      725 2023-02-28 19:39:23.000000 cbra-3.0.0a7/cbra/ext/picqer/v1/purchaseorderevent.py
+-rw-r--r--   0 cochise    (501) staff       (20)      951 2023-02-25 01:54:30.000000 cbra-3.0.0a7/cbra/ext/picqer/webhookresponse.py
+-rw-r--r--   0 cochise    (501) staff       (20)      901 2023-02-25 04:56:47.000000 cbra-3.0.0a7/cbra/ext/picqer/webhooksecret.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1622 2023-02-25 04:57:09.000000 cbra-3.0.0a7/cbra/ext/picqer/webhooksignature.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1000 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/package.json
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.124122 cbra-3.0.0a7/cbra/types/
+-rw-r--r--   0 cochise    (501) staff       (20)     3660 2023-02-27 00:47:33.000000 cbra-3.0.0a7/cbra/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      911 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/abortable.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4141 2023-02-25 23:42:27.000000 cbra-3.0.0a7/cbra/types/basemodel.py
+-rw-r--r--   0 cochise    (501) staff       (20)      518 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/conflict.py
+-rw-r--r--   0 cochise    (501) staff       (20)      519 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/forbidden.py
+-rw-r--r--   0 cochise    (501) staff       (20)      725 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/hints.py
+-rw-r--r--   0 cochise    (501) staff       (20)      787 2023-02-27 00:52:53.000000 cbra-3.0.0a7/cbra/types/hmacsignature.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1666 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/httpheaderprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1973 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/iauthorizationcontext.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1155 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/iauthorizationcontextfactory.py
+-rw-r--r--   0 cochise    (501) staff       (20)      699 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/icredential.py
+-rw-r--r--   0 cochise    (501) staff       (20)      877 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/icredentialverifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)      446 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/icursor.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1423 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/ideferred.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1414 2023-02-28 16:57:21.000000 cbra-3.0.0a7/cbra/types/idependant.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5642 2023-03-01 11:05:07.000000 cbra-3.0.0a7/cbra/types/iendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1792 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/ihashable.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1360 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/imodelrepository.py
+-rw-r--r--   0 cochise    (501) staff       (20)      755 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/integerpathparameter.py
+-rw-r--r--   0 cochise    (501) staff       (20)      581 2023-02-26 15:28:16.000000 cbra-3.0.0a7/cbra/types/iqueryresult.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3046 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/irequestprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)      673 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/irequestprincipalintrospecter.py
+-rw-r--r--   0 cochise    (501) staff       (20)      677 2023-02-26 16:35:24.000000 cbra-3.0.0a7/cbra/types/iroutable.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1522 2023-02-27 00:35:48.000000 cbra-3.0.0a7/cbra/types/isessiondata.py
+-rw-r--r--   0 cochise    (501) staff       (20)      608 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/isessionfactory.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1495 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/isessionmanager.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1074 2023-02-26 19:12:06.000000 cbra-3.0.0a7/cbra/types/isubject.py
+-rw-r--r--   0 cochise    (501) staff       (20)      785 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/isubjectresolver.py
+-rw-r--r--   0 cochise    (501) staff       (20)      675 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/jsonwebtoken.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1473 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/jsonwebtokenprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1508 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/modelautoassignedidentity.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1525 2023-02-25 22:43:16.000000 cbra-3.0.0a7/cbra/types/modelidentity.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1600 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/mutablesignature.py
+-rw-r--r--   0 cochise    (501) staff       (20)      523 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/notauthorized.py
+-rw-r--r--   0 cochise    (501) staff       (20)      518 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/notfound.py
+-rw-r--r--   0 cochise    (501) staff       (20)      644 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/nullrequestprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1036 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/nullsubject.py
+-rw-r--r--   0 cochise    (501) staff       (20)      713 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/nullsubjectesolver.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1806 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/oidcrequestprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)      845 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/opaquebearertokenprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1280 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/operation.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1133 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/pathparameter.py
+-rw-r--r--   0 cochise    (501) staff       (20)      844 2023-02-25 23:40:52.000000 cbra-3.0.0a7/cbra/types/persistedmodel.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1717 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/requestprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1768 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/rfc9068requestprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2380 2023-02-27 00:36:50.000000 cbra-3.0.0a7/cbra/types/session.py
+-rw-r--r--   0 cochise    (501) staff       (20)      618 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/sessionclaims.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1134 2023-02-27 00:36:57.000000 cbra-3.0.0a7/cbra/types/sessionmodel.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2090 2023-02-27 00:49:22.000000 cbra-3.0.0a7/cbra/types/sessionrequestprincipal.py
+-rw-r--r--   0 cochise    (501) staff       (20)      753 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/stringpathparameter.py
+-rw-r--r--   0 cochise    (501) staff       (20)      483 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/subjectidentifier.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1023 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/unauthenticatedauthorizationcontext.py
+-rw-r--r--   0 cochise    (501) staff       (20)      800 2023-02-23 23:31:32.000000 cbra-3.0.0a7/cbra/types/uuidpathparameter.py
+-rw-r--r--   0 cochise    (501) staff       (20)      564 2023-02-27 00:52:11.000000 cbra-3.0.0a7/cbra/types/verifier.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.098090 cbra-3.0.0a7/cbra.egg-info/
+-rw-r--r--   0 cochise    (501) staff       (20)     1606 2023-03-01 11:11:22.000000 cbra-3.0.0a7/cbra.egg-info/PKG-INFO
+-rw-r--r--   0 cochise    (501) staff       (20)     8035 2023-03-01 11:11:23.000000 cbra-3.0.0a7/cbra.egg-info/SOURCES.txt
+-rw-r--r--   0 cochise    (501) staff       (20)        1 2023-03-01 11:11:22.000000 cbra-3.0.0a7/cbra.egg-info/dependency_links.txt
+-rw-r--r--   0 cochise    (501) staff       (20)      117 2023-03-01 11:11:22.000000 cbra-3.0.0a7/cbra.egg-info/entry_points.txt
+-rw-r--r--   0 cochise    (501) staff       (20)      299 2023-03-01 11:11:22.000000 cbra-3.0.0a7/cbra.egg-info/requires.txt
+-rw-r--r--   0 cochise    (501) staff       (20)       54 2023-03-01 11:11:22.000000 cbra-3.0.0a7/cbra.egg-info/top_level.txt
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.095579 cbra-3.0.0a7/docs/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.124237 cbra-3.0.0a7/docs/source/
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.124348 cbra-3.0.0a7/docs/source/_ext/
+-rw-r--r--   0 cochise    (501) staff       (20)    15901 2023-02-23 23:31:32.000000 cbra-3.0.0a7/docs/source/_ext/djangodocs.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2934 2023-02-23 23:31:32.000000 cbra-3.0.0a7/docs/source/conf.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.125435 cbra-3.0.0a7/examples/
+-rw-r--r--   0 cochise    (501) staff       (20)      904 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/authentication.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1631 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/dependency-injection.py
+-rw-r--r--   0 cochise    (501) staff       (20)      754 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/endpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1029 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/fastapi-authentication.py
+-rw-r--r--   0 cochise    (501) staff       (20)      557 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/google-cloud-platform.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1673 2023-02-23 18:20:54.000000 cbra-3.0.0a7/examples/oauth2-callback-google.py
+-rw-r--r--   0 cochise    (501) staff       (20)      677 2023-02-24 00:39:57.000000 cbra-3.0.0a7/examples/oauth2-server.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1387 2023-02-25 05:00:28.000000 cbra-3.0.0a7/examples/picqer-webhook.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2128 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/resource.py
+-rw-r--r--   0 cochise    (501) staff       (20)      899 2023-02-23 23:31:32.000000 cbra-3.0.0a7/examples/session.py
+-rw-r--r--   0 cochise    (501) staff       (20)       38 2023-03-01 11:11:23.128466 cbra-3.0.0a7/setup.cfg
+-rw-r--r--   0 cochise    (501) staff       (20)     1280 2023-02-23 23:31:32.000000 cbra-3.0.0a7/setup.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.126401 cbra-3.0.0a7/tests/
+-rw-r--r--   0 cochise    (501) staff       (20)      399 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      550 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/conftest.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.126520 cbra-3.0.0a7/tests/core/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/core/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.126618 cbra-3.0.0a7/tests/core/iam/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/core/iam/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.126808 cbra-3.0.0a7/tests/core/iam/models/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/core/iam/models/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2695 2023-02-24 11:07:32.000000 cbra-3.0.0a7/tests/core/iam/models/test_unit_subject.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.126939 cbra-3.0.0a7/tests/ext/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/ext/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.127125 cbra-3.0.0a7/tests/ext/google/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/ext/google/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.127374 cbra-3.0.0a7/tests/ext/google/system/
+-rw-r--r--   0 cochise    (501) staff       (20)     1339 2023-02-25 04:00:03.000000 cbra-3.0.0a7/tests/ext/google/system/conftest.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2387 2023-02-28 17:14:16.000000 cbra-3.0.0a7/tests/ext/google/system/test_system_googleendpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1928 2023-02-28 18:14:15.000000 cbra-3.0.0a7/tests/ext/google/test_integration_aorta.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.127572 cbra-3.0.0a7/tests/ext/oauth2/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/ext/oauth2/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2267 2023-02-23 23:48:41.000000 cbra-3.0.0a7/tests/ext/oauth2/test_unit_redirecturi.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.127773 cbra-3.0.0a7/tests/ext/picqer/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2023-02-25 03:36:34.000000 cbra-3.0.0a7/tests/ext/picqer/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3876 2023-02-25 04:58:38.000000 cbra-3.0.0a7/tests/ext/picqer/test_unit_signature.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3599 2023-03-01 11:10:13.000000 cbra-3.0.0a7/tests/test_unit_endpoint.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1465 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/test_unit_endpoint_authentication.py
+-rw-r--r--   0 cochise    (501) staff       (20)      399 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/test_unit_ioc.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4480 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/test_unit_principal.py
+-rw-r--r--   0 cochise    (501) staff       (20)     3162 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/test_unit_resource.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4380 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/test_unit_session.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-01 11:11:23.127993 cbra-3.0.0a7/tests/types/
+-rw-r--r--   0 cochise    (501) staff       (20)      394 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/types/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4378 2023-02-23 23:31:32.000000 cbra-3.0.0a7/tests/types/test_unit_basemodel_identity.py
```

### Comparing `cbra-2.0.0a8/PKG-INFO` & `cbra-3.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbra
-Version: 2.0.0a8
+Version: 3.0.0a7
 Summary: A class-based REStful API framework built on FastAPI
 Home-page: https://docs.cochise.io/python/cbra/latest
 Author: Cochise Ruhulessin
 Author-email: cochiseruhulessin@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `cbra-2.0.0a8/README.md` & `cbra-3.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/__init__.py` & `cbra-3.0.0a7/cbra/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/application.py` & `cbra-3.0.0a7/cbra/core/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 #
 # All rights reserved. No warranty, explicit or implicit, provided. In
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-import copy
 import inspect
-import logging.config
 from typing import Any
 from typing import Callable
 
 import aorta
 import fastapi
 from fastapi import FastAPI
 from fastapi.routing import DecoratedCallable
@@ -42,38 +40,26 @@
         handlers: dict[type, Any] = kwargs.setdefault('exception_handlers', {})
         handlers[Abortable] = self.on_aborted
 
         kwargs.setdefault('root_path', settings.ASGI_ROOT_PATH)
         self.inject('MessagePublisher', MessagePublisher)
         self.inject('MessageTransport', aorta.NullTransport())
         super().__init__(*args, **kwargs)
-        self.add_event_handler('startup', self.setup_logging) # type: ignore
 
     def add(
         self,
         routable: type[Endpoint | Resource],
         *args: Any, **kwargs: Any
     ) -> None:
         routable.add_to_router(self, *args, **kwargs)
 
     def inject(self, name: str, value: Any) -> None:
         """Inject a value into the dependencies container."""
         self.container.inject(name, value)
 
-    def logging_config(self):
-        config = copy.deepcopy(settings.LOGGING)
-        if not settings.DEBUG and not settings.LOG_CONSOLE:
-            # Remove console handler when not running in debug mode and its
-            # not explicitely enabled in the settings.
-            config['handlers']['console'] = {'class': 'logging.NullHandler'}
-        return config
-
-    def setup_logging(self) -> None:
-        logging.config.dictConfig(self.logging_config())
-
     async def on_aborted(
         self,
         request: fastapi.Request,
         exc: Abortable
     ) -> fastapi.Response:
         return await exc.as_response()
```

### Comparing `cbra-2.0.0a8/cbra/core/conf.py` & `cbra-3.0.0a7/cbra/core/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,25 +25,14 @@
 
 Default: ``None``
 
 The root path of the application. Use this setting when running behind
 a proxy and the application is served from something else than ``/``
 e.g. ``/api/v1``.
 
-.. setting:: DEBUG
-
-``DEBUG``
----------
-
-Default: ``False``
-
-A boolean that turns on/off debug mode.
-
-Never deploy an application into production with :setting:`DEBUG` turned on.
-
 
 .. setting:: DEPENDENCIES
 
 ``DEPENDENCIES``
 ================
 
 The list of dependencies that are injected during application boot-time. It
@@ -71,24 +60,14 @@
 Default: ``'production'``
 
 The current deployment environment. This defaults to the string
 ``production`` in order to prevent applications being deployed
 with less secure settings from other environments.
 
 
-.. setting:: LOG_CONSOLE
-
-``LOG_CONSOLE``
----------------
-
-Default: ``False``
-
-Enable logging to ``stdout``.
-
-
 .. setting: OAUTH2_CLIENTS
 
 ``OAUTH2_CLIENTS``
 ==================
 The list of OAuth 2.x/OpenID Connect clients that are used by the
 application. Example:
 
@@ -290,74 +269,31 @@
 from typing import Any
 
 
 class Settings:
     user: types.ModuleType | None = None
     ASGI_ROOT_PATH: str | None
     DEPLOYMENT_ENV: str
-    DEBUG: bool
     LOGIN_AUTHORIZED_DOMAINS: set[str]
-    LOG_CONSOLE: bool
-    LOGGING: dict[str, Any]
     OAUTH2_CLIENTS: list[Any]
     OAUTH2_ISSUER: str
     SECRET_KEY: str
     SESSION_COOKIE_AGE: int
     SESSION_COOKIE_DOMAIN: str | None
     SESSION_COOKIE_HTTPONLY: bool
     SESSION_COOKIE_NAME: str
     SESSION_COOKIE_PATH: str
     SESSION_COOKIE_SAMESITE: bool | str | None
     SESSION_COOKIE_SECURE: bool
     TRUSTED_AUTHORIZATION_SERVERS: list[str]
 
     __defaults__: dict[str, Any] = {
         'ASGI_ROOT_PATH': os.environ.get('ASGI_ROOT_PATH'),
-        'DEBUG': False,
         'DEPLOYMENT_ENV': os.environ.get('DEPLOYMENT_ENV') or 'production',
         'LOGIN_AUTHORIZED_DOMAINS': set(),
-        'LOG_CONSOLE': False,
-        'LOGGING': {
-            'version': 1,
-            'disable_existing_loggers': False,
-            'formatters': {
-                "uvicorn": {
-                    "()": "uvicorn.logging.DefaultFormatter",
-                    "fmt": "%(levelprefix)s %(message)s",
-                    "use_colors": None,
-                },
-                "stdout": {
-                    "fmt": "%(message)s",
-                },
-            },
-            'handlers': {
-                'default': {
-                    'formatter': "uvicorn",
-                    'class': "logging.StreamHandler",
-                    'stream': "ext://sys.stdout",
-                },
-                'console': {
-                    'class': 'logging.StreamHandler',
-                    'stream': "ext://sys.stdout",
-                    'formatter': 'uvicorn'
-                }
-            },
-            'loggers': {
-                'aorta': {
-                    'handlers': ['console', 'default'],
-                    'propagate': False,
-                    'level': 'INFO'
-                },
-                'cbra': {
-                    'handlers': ['console', 'default'],
-                    'propagate': False,
-                    'level': 'INFO'
-                }
-            }
-        },
         'OAUTH2_CLIENTS': [],
         'OAUTH2_ISSUER': None,
         'SECRET_KEY': os.environ.get('SECRET_KEY') or bytes.hex(os.urandom(32)),
         'SESSION_COOKIE_AGE': 1209600,
         'SESSION_COOKIE_DOMAIN': None,
         'SESSION_COOKIE_HTTPONLY': True,
         'SESSION_COOKIE_NAME': 'session',
```

### Comparing `cbra-2.0.0a8/cbra/core/endpoint.py` & `cbra-3.0.0a7/cbra/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/endpointtype.py` & `cbra-3.0.0a7/cbra/core/endpointtype.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/__init__.py` & `cbra-3.0.0a7/cbra/core/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/authenticatedcontext.py` & `cbra-3.0.0a7/cbra/core/iam/authenticatedcontext.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/authenticationservice.py` & `cbra-3.0.0a7/cbra/core/iam/authenticationservice.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/authorizationcontextfactory.py` & `cbra-3.0.0a7/cbra/core/iam/authorizationcontextfactory.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/isubjectrepository.py` & `cbra-3.0.0a7/cbra/core/iam/isubjectrepository.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/models/__init__.py` & `cbra-3.0.0a7/cbra/core/iam/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/models/emailprincipal.py` & `cbra-3.0.0a7/cbra/core/iam/models/emailprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/models/externalprincipal.py` & `cbra-3.0.0a7/cbra/core/iam/models/externalprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/models/principal.py` & `cbra-3.0.0a7/cbra/core/iam/models/principal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/models/publicidentifierprincipal.py` & `cbra-3.0.0a7/cbra/core/iam/models/publicidentifierprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/models/subject.py` & `cbra-3.0.0a7/cbra/core/iam/models/subject.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/principalhasher.py` & `cbra-3.0.0a7/cbra/core/iam/principalhasher.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/services/__init__.py` & `cbra-3.0.0a7/cbra/core/iam/services/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/services/useronboarding.py` & `cbra-3.0.0a7/cbra/core/iam/services/useronboarding.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/subject.py` & `cbra-3.0.0a7/cbra/core/iam/subject.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/subjectresolver.py` & `cbra-3.0.0a7/cbra/core/iam/subjectresolver.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/types/__init__.py` & `cbra-3.0.0a7/cbra/core/iam/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/types/isubjectrepository.py` & `cbra-3.0.0a7/cbra/core/iam/types/isubjectrepository.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/types/iuseronboardingservice.py` & `cbra-3.0.0a7/cbra/core/iam/types/iuseronboardingservice.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/types/publicidentifier.py` & `cbra-3.0.0a7/cbra/core/iam/types/publicidentifier.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/iam/types/subject.py` & `cbra-3.0.0a7/cbra/core/iam/types/subject.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/ioc/__init__.py` & `cbra-3.0.0a7/cbra/core/ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/ioc/config.py` & `cbra-3.0.0a7/cbra/core/ioc/config.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/ioc/container.py` & `cbra-3.0.0a7/cbra/core/ioc/container.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/ioc/dependency.py` & `cbra-3.0.0a7/cbra/core/ioc/dependency.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/ioc/inheriteddependencydecorator.py` & `cbra-3.0.0a7/cbra/core/ioc/inheriteddependencydecorator.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/ioc/injected.py` & `cbra-3.0.0a7/cbra/core/ioc/injected.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/ioc/instance.py` & `cbra-3.0.0a7/cbra/core/ioc/instance.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/ioc/loader.py` & `cbra-3.0.0a7/cbra/core/ioc/loader.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/ioc/requirement.py` & `cbra-3.0.0a7/cbra/core/ioc/requirement.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/ioc/setting_.py` & `cbra-3.0.0a7/cbra/core/ioc/setting_.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/ioc/test/__init__.py` & `cbra-3.0.0a7/cbra/core/ioc/test/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/messagepublisher.py` & `cbra-3.0.0a7/cbra/core/messagepublisher.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/optionsrequesthandler.py` & `cbra-3.0.0a7/cbra/core/optionsrequesthandler.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/package.json` & `cbra-3.0.0a7/cbra/core/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333333%*

 * *Differences: {"'extras_require'": "{'all': {delete: [3, 2]}, 'google': {delete: [3]}}"}*

```diff
@@ -23,28 +23,25 @@
             "cbra.ext.service = cbra.ext.service.runlevel:init"
         ]
     },
     "extras_require": {
         "all": [
             "aorta[all]>=3.0.0a3",
             "google-cloud-datastore>=2.13.2",
-            "google-cloud-logging",
-            "gunicorn",
             "gunicorn",
             "httpx",
             "jwcrypto",
             "google.auth",
             "pyjwt",
             "unimatrix.ext.kms[all]"
         ],
         "google": [
             "aorta[google]>=3.0.0a3",
             "ckms[google]>=0.60",
-            "google-cloud-datastore>=2.13.2",
-            "google-cloud-logging"
+            "google-cloud-datastore>=2.13.2"
         ],
         "gunicorn": [
             "gunicorn"
         ]
     },
     "install_requires": [
         "ckms>=0.60.0",
```

### Comparing `cbra-2.0.0a8/cbra/core/params/__init__.py` & `cbra-3.0.0a7/cbra/core/params/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/requesthandler.py` & `cbra-3.0.0a7/cbra/core/requesthandler.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/__init__.py` & `cbra-3.0.0a7/cbra/core/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/collection.py` & `cbra-3.0.0a7/cbra/core/resource/collection.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/collectionaction.py` & `cbra-3.0.0a7/cbra/core/resource/collectionaction.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/create.py` & `cbra-3.0.0a7/cbra/core/resource/create.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/createaction.py` & `cbra-3.0.0a7/cbra/core/resource/createaction.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/customaction.py` & `cbra-3.0.0a7/cbra/core/resource/customaction.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/delete.py` & `cbra-3.0.0a7/cbra/core/resource/delete.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/deleteaction.py` & `cbra-3.0.0a7/cbra/core/resource/deleteaction.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/detail.py` & `cbra-3.0.0a7/cbra/core/resource/detail.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/detailaction.py` & `cbra-3.0.0a7/cbra/core/resource/detailaction.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/iresource.py` & `cbra-3.0.0a7/cbra/core/resource/iresource.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/listaction.py` & `cbra-3.0.0a7/cbra/core/resource/listaction.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/persister.py` & `cbra-3.0.0a7/cbra/core/resource/persister.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/queryresult.py` & `cbra-3.0.0a7/cbra/core/resource/queryresult.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/replace.py` & `cbra-3.0.0a7/cbra/core/resource/replace.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/replaceaction.py` & `cbra-3.0.0a7/cbra/core/resource/replaceaction.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/resource.py` & `cbra-3.0.0a7/cbra/core/resource/resource.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/resourceaction.py` & `cbra-3.0.0a7/cbra/core/resource/resourceaction.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/resourceidentifier.py` & `cbra-3.0.0a7/cbra/core/resource/resourceidentifier.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/resourcelist.py` & `cbra-3.0.0a7/cbra/core/resource/resourcelist.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/resourcelistmetadata.py` & `cbra-3.0.0a7/cbra/core/resource/resourcelistmetadata.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/resourcemodel.py` & `cbra-3.0.0a7/cbra/core/resource/resourcemodel.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/resourcemodeltype.py` & `cbra-3.0.0a7/cbra/core/resource/resourcemodeltype.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/resourceoptionsrequesthandler.py` & `cbra-3.0.0a7/cbra/core/resource/resourceoptionsrequesthandler.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/resourcetype.py` & `cbra-3.0.0a7/cbra/core/resource/resourcetype.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/retrieve.py` & `cbra-3.0.0a7/cbra/core/resource/retrieve.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/retrieveaction.py` & `cbra-3.0.0a7/cbra/core/resource/retrieveaction.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/test/__init__.py` & `cbra-3.0.0a7/cbra/core/resource/test/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/test/book.py` & `cbra-3.0.0a7/cbra/core/resource/test/book.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/test/bookpublication.py` & `cbra-3.0.0a7/cbra/core/resource/test/bookpublication.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/test/bookresource.py` & `cbra-3.0.0a7/cbra/core/resource/test/bookresource.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/update.py` & `cbra-3.0.0a7/cbra/core/resource/update.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/updateaction.py` & `cbra-3.0.0a7/cbra/core/resource/updateaction.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/resource/viewer.py` & `cbra-3.0.0a7/cbra/core/resource/viewer.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/secretkey.py` & `cbra-3.0.0a7/cbra/core/secretkey.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/sessions/requestsession.py` & `cbra-3.0.0a7/cbra/core/sessions/requestsession.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/core/utils.py` & `cbra-3.0.0a7/cbra/core/utils.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/__init__.py` & `cbra-3.0.0a7/cbra/ext/google/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/aortaendpoint.py` & `cbra-3.0.0a7/cbra/ext/google/aortaendpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/datastorequeryresult.py` & `cbra-3.0.0a7/cbra/ext/google/datastorequeryresult.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/datastorerepository.py` & `cbra-3.0.0a7/cbra/ext/google/datastorerepository.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/datastoresubjectrepository.py` & `cbra-3.0.0a7/cbra/ext/google/datastoresubjectrepository.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/datastoresubjectresolver.py` & `cbra-3.0.0a7/cbra/ext/google/datastoresubjectresolver.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/environ.py` & `cbra-3.0.0a7/cbra/ext/google/environ.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/eventarcendpoint.py` & `cbra-3.0.0a7/cbra/ext/google/eventarcendpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/googleendpoint.py` & `cbra-3.0.0a7/cbra/ext/google/googleendpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/googlepubsubtransport.py` & `cbra-3.0.0a7/cbra/ext/google/googlepubsubtransport.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/googleserviceaccountprincipal.py` & `cbra-3.0.0a7/cbra/ext/google/googleserviceaccountprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/impl/oauth2/storage.py` & `cbra-3.0.0a7/cbra/ext/google/impl/oauth2/storage.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/messagepublished.py` & `cbra-3.0.0a7/cbra/ext/google/messagepublished.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/messagerunner.py` & `cbra-3.0.0a7/cbra/ext/google/messagerunner.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/pubsubmessage.py` & `cbra-3.0.0a7/cbra/ext/google/pubsubmessage.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/resourcemetadata.py` & `cbra-3.0.0a7/cbra/ext/google/resourcemetadata.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/runner.py` & `cbra-3.0.0a7/cbra/ext/google/runner.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/google/service.py` & `cbra-3.0.0a7/cbra/ext/google/service.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # no event shall the author(s) be liable for any claim or damages.
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 from typing import Any
 
-from google.cloud import logging
-
 from cbra.core import Application
 from cbra.core.utils import parent_signature
 from .aortaendpoint import AortaEndpoint
 from .environ import GOOGLE_DATASTORE_NAMESPACE
 from .environ import GOOGLE_SERVICE_PROJECT
 
 
@@ -34,25 +32,8 @@
             )
             self.container.provide('SubjectResolver', {
                 'qualname': 'cbra.ext.google.DatastoreSubjectResolver'
             })
             self.container.provide('SubjectRepository', {
                 'qualname': 'cbra.ext.google.DatastoreSubjectRepository'
             })
-        self.add(AortaEndpoint, path="/.well-known/aorta")
-
-    def logging_config(self):
-        client = logging.Client(project=GOOGLE_SERVICE_PROJECT)
-        client.setup_logging() # type: ignore
-        config = super().logging_config()
-        config['formatters']['google-cloud'] = {
-            '()': "cbra.ext.google.logging.JSONFormatter",
-        }
-        config['handlers']['default'] = {
-            'class': 'google.cloud.logging.handlers.CloudLoggingHandler',
-            'client': client,
-            'formatter': 'google-cloud',
-            'labels': {
-                'kind': 'service'
-            }
-        }
-        return config
+        self.add(AortaEndpoint, path="/.well-known/aorta")
```

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/__init__.py` & `cbra-3.0.0a7/cbra/ext/oauth2/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/authorizationcodecallbackendpoint.py` & `cbra-3.0.0a7/cbra/ext/oauth2/authorizationcodecallbackendpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/authorizationendpoint.py` & `cbra-3.0.0a7/cbra/ext/oauth2/authorizationendpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/basestorage.py` & `cbra-3.0.0a7/cbra/ext/oauth2/basestorage.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/endpoint.py` & `cbra-3.0.0a7/cbra/ext/oauth2/endpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/loginendpoint.py` & `cbra-3.0.0a7/cbra/ext/oauth2/loginendpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/memorystorage.py` & `cbra-3.0.0a7/cbra/ext/oauth2/memorystorage.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/models/__init__.py` & `cbra-3.0.0a7/cbra/ext/oauth2/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/models/authorization.py` & `cbra-3.0.0a7/cbra/ext/oauth2/models/authorization.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/models/authorizationstate.py` & `cbra-3.0.0a7/cbra/ext/oauth2/models/authorizationstate.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/oidcregistrationendpoint.py` & `cbra-3.0.0a7/cbra/ext/oauth2/oidcregistrationendpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/__init__.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/authorizationlifecycle.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/authorizationlifecycle.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/authorizationrequest.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/authorizationrequest.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/iauthorizationflowstate.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/iauthorizationflowstate.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/iauthorizationserverstorage.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/iauthorizationserverstorage.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/invalidauthorizeresponse.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/invalidauthorizeresponse.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/jarmauthorizeresponse.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/jarmauthorizeresponse.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/loginresponse.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/loginresponse.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/queryauthorizeresponse.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/queryauthorizeresponse.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/redirectparameters.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/redirectparameters.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/redirecturi.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/redirecturi.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/responsemodenotsupported.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/responsemodenotsupported.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/responsevalidationfailure.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/responsevalidationfailure.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/oauth2/types/unsupportedauthorizationresponse.py` & `cbra-3.0.0a7/cbra/ext/oauth2/types/unsupportedauthorizationresponse.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/picqer/__init__.py` & `cbra-3.0.0a7/cbra/ext/picqer/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/picqer/picqerwebhookendpoint.py` & `cbra-3.0.0a7/cbra/ext/picqer/picqerwebhookendpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/picqer/v1/__init__.py` & `cbra-3.0.0a7/cbra/ext/picqer/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/picqer/v1/event.py` & `cbra-3.0.0a7/cbra/ext/picqer/v1/event.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/picqer/v1/orderevent.py` & `cbra-3.0.0a7/cbra/ext/picqer/v1/orderevent.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/picqer/v1/picklistevent.py` & `cbra-3.0.0a7/cbra/ext/picqer/v1/picklistevent.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/picqer/v1/purchaseorderevent.py` & `cbra-3.0.0a7/cbra/ext/picqer/v1/purchaseorderevent.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/picqer/webhookresponse.py` & `cbra-3.0.0a7/cbra/ext/picqer/webhookresponse.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/picqer/webhooksecret.py` & `cbra-3.0.0a7/cbra/ext/picqer/webhooksecret.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/ext/picqer/webhooksignature.py` & `cbra-3.0.0a7/cbra/ext/picqer/webhooksignature.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/package.json` & `cbra-3.0.0a7/cbra/package.json`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/__init__.py` & `cbra-3.0.0a7/cbra/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/abortable.py` & `cbra-3.0.0a7/cbra/types/abortable.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/basemodel.py` & `cbra-3.0.0a7/cbra/types/basemodel.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/conflict.py` & `cbra-3.0.0a7/cbra/types/conflict.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/forbidden.py` & `cbra-3.0.0a7/cbra/types/forbidden.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/hints.py` & `cbra-3.0.0a7/cbra/types/hints.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/hmacsignature.py` & `cbra-3.0.0a7/cbra/types/hmacsignature.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/httpheaderprincipal.py` & `cbra-3.0.0a7/cbra/types/httpheaderprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/iauthorizationcontext.py` & `cbra-3.0.0a7/cbra/types/iauthorizationcontext.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/iauthorizationcontextfactory.py` & `cbra-3.0.0a7/cbra/types/iauthorizationcontextfactory.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/icredential.py` & `cbra-3.0.0a7/cbra/types/icredential.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/icredentialverifier.py` & `cbra-3.0.0a7/cbra/types/icredentialverifier.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/ideferred.py` & `cbra-3.0.0a7/cbra/types/ideferred.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/idependant.py` & `cbra-3.0.0a7/cbra/types/idependant.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/iendpoint.py` & `cbra-3.0.0a7/cbra/types/iendpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 class IEndpoint:
     __module__: str = 'cbra.types'
     allowed_http_methods: list[str]
     context_factory: IAuthorizationContextFactory
     handlers: list[IRoutable]
     include_in_schema: bool = True
     name: str | None = None
-    logger: logging.Logger = logging.getLogger('cbra.endpoint')
+    logger: logging.Logger = logging.getLogger('uvicorn')
     response_model_by_alias: bool = False
     session: ISessionManager[Any]
     with_options: bool = True
 
     #: The set of permissions supported by this endpoint. These must be
     #: defined beforehand to limit the number of calls to remote IAM
     #: systems.
```

### Comparing `cbra-2.0.0a8/cbra/types/ihashable.py` & `cbra-3.0.0a7/cbra/types/ihashable.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/imodelrepository.py` & `cbra-3.0.0a7/cbra/types/imodelrepository.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/integerpathparameter.py` & `cbra-3.0.0a7/cbra/types/integerpathparameter.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/iqueryresult.py` & `cbra-3.0.0a7/cbra/types/iqueryresult.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/irequestprincipal.py` & `cbra-3.0.0a7/cbra/types/irequestprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/irequestprincipalintrospecter.py` & `cbra-3.0.0a7/cbra/types/irequestprincipalintrospecter.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/iroutable.py` & `cbra-3.0.0a7/cbra/types/iroutable.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/isessiondata.py` & `cbra-3.0.0a7/cbra/types/isessiondata.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/isessionfactory.py` & `cbra-3.0.0a7/cbra/types/isessionfactory.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/isessionmanager.py` & `cbra-3.0.0a7/cbra/types/isessionmanager.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/isubject.py` & `cbra-3.0.0a7/cbra/types/isubject.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/isubjectresolver.py` & `cbra-3.0.0a7/cbra/types/isubjectresolver.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/jsonwebtoken.py` & `cbra-3.0.0a7/cbra/types/jsonwebtoken.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/jsonwebtokenprincipal.py` & `cbra-3.0.0a7/cbra/types/jsonwebtokenprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/modelautoassignedidentity.py` & `cbra-3.0.0a7/cbra/types/modelautoassignedidentity.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/modelidentity.py` & `cbra-3.0.0a7/cbra/types/modelidentity.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/mutablesignature.py` & `cbra-3.0.0a7/cbra/types/mutablesignature.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/notauthorized.py` & `cbra-3.0.0a7/cbra/types/notauthorized.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/notfound.py` & `cbra-3.0.0a7/cbra/types/notfound.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/nullrequestprincipal.py` & `cbra-3.0.0a7/cbra/types/nullrequestprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/nullsubject.py` & `cbra-3.0.0a7/cbra/types/nullsubject.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/nullsubjectesolver.py` & `cbra-3.0.0a7/cbra/types/nullsubjectesolver.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/oidcrequestprincipal.py` & `cbra-3.0.0a7/cbra/types/oidcrequestprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/opaquebearertokenprincipal.py` & `cbra-3.0.0a7/cbra/types/opaquebearertokenprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/operation.py` & `cbra-3.0.0a7/cbra/types/operation.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/pathparameter.py` & `cbra-3.0.0a7/cbra/types/pathparameter.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/persistedmodel.py` & `cbra-3.0.0a7/cbra/types/persistedmodel.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/requestprincipal.py` & `cbra-3.0.0a7/cbra/types/requestprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/rfc9068requestprincipal.py` & `cbra-3.0.0a7/cbra/types/rfc9068requestprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/session.py` & `cbra-3.0.0a7/cbra/types/session.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/sessionclaims.py` & `cbra-3.0.0a7/cbra/types/sessionclaims.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/sessionmodel.py` & `cbra-3.0.0a7/cbra/types/sessionmodel.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/sessionrequestprincipal.py` & `cbra-3.0.0a7/cbra/types/sessionrequestprincipal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/stringpathparameter.py` & `cbra-3.0.0a7/cbra/types/stringpathparameter.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/unauthenticatedauthorizationcontext.py` & `cbra-3.0.0a7/cbra/types/unauthenticatedauthorizationcontext.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/uuidpathparameter.py` & `cbra-3.0.0a7/cbra/types/uuidpathparameter.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra/types/verifier.py` & `cbra-3.0.0a7/cbra/types/verifier.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/cbra.egg-info/PKG-INFO` & `cbra-3.0.0a7/cbra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbra
-Version: 2.0.0a8
+Version: 3.0.0a7
 Summary: A class-based REStful API framework built on FastAPI
 Home-page: https://docs.cochise.io/python/cbra/latest
 Author: Cochise Ruhulessin
 Author-email: cochiseruhulessin@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `cbra-2.0.0a8/cbra.egg-info/SOURCES.txt` & `cbra-3.0.0a7/cbra.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
 cbra/ext/google/datastoresubjectrepository.py
 cbra/ext/google/datastoresubjectresolver.py
 cbra/ext/google/environ.py
 cbra/ext/google/eventarcendpoint.py
 cbra/ext/google/googleendpoint.py
 cbra/ext/google/googlepubsubtransport.py
 cbra/ext/google/googleserviceaccountprincipal.py
-cbra/ext/google/logging.py
 cbra/ext/google/messagediscarded.py
 cbra/ext/google/messagepublished.py
 cbra/ext/google/messagerunner.py
 cbra/ext/google/pubsubmessage.py
 cbra/ext/google/resourcemetadata.py
 cbra/ext/google/runner.py
 cbra/ext/google/service.py
```

### Comparing `cbra-2.0.0a8/docs/source/_ext/djangodocs.py` & `cbra-3.0.0a7/docs/source/_ext/djangodocs.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/docs/source/conf.py` & `cbra-3.0.0a7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/examples/authentication.py` & `cbra-3.0.0a7/examples/authentication.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/examples/dependency-injection.py` & `cbra-3.0.0a7/examples/dependency-injection.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/examples/endpoint.py` & `cbra-3.0.0a7/examples/endpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/examples/fastapi-authentication.py` & `cbra-3.0.0a7/examples/fastapi-authentication.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/examples/google-cloud-platform.py` & `cbra-3.0.0a7/examples/google-cloud-platform.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/examples/oauth2-callback-google.py` & `cbra-3.0.0a7/examples/oauth2-callback-google.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/examples/oauth2-server.py` & `cbra-3.0.0a7/examples/oauth2-server.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/examples/picqer-webhook.py` & `cbra-3.0.0a7/examples/picqer-webhook.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/examples/resource.py` & `cbra-3.0.0a7/examples/resource.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/examples/session.py` & `cbra-3.0.0a7/examples/session.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/setup.py` & `cbra-3.0.0a7/setup.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/tests/conftest.py` & `cbra-3.0.0a7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/tests/core/iam/models/test_unit_subject.py` & `cbra-3.0.0a7/tests/core/iam/models/test_unit_subject.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/tests/ext/google/system/conftest.py` & `cbra-3.0.0a7/tests/ext/google/system/conftest.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/tests/ext/google/system/test_system_googleendpoint.py` & `cbra-3.0.0a7/tests/ext/google/system/test_system_googleendpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/tests/ext/google/test_integration_aorta.py` & `cbra-3.0.0a7/tests/ext/google/test_integration_aorta.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/tests/ext/oauth2/test_unit_redirecturi.py` & `cbra-3.0.0a7/tests/ext/oauth2/test_unit_redirecturi.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/tests/ext/picqer/test_unit_signature.py` & `cbra-3.0.0a7/tests/ext/picqer/test_unit_signature.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/tests/test_unit_endpoint.py` & `cbra-3.0.0a7/tests/test_unit_endpoint.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/tests/test_unit_endpoint_authentication.py` & `cbra-3.0.0a7/tests/test_unit_endpoint_authentication.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/tests/test_unit_principal.py` & `cbra-3.0.0a7/tests/test_unit_principal.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/tests/test_unit_resource.py` & `cbra-3.0.0a7/tests/test_unit_resource.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/tests/test_unit_session.py` & `cbra-3.0.0a7/tests/test_unit_session.py`

 * *Files identical despite different names*

### Comparing `cbra-2.0.0a8/tests/types/test_unit_basemodel_identity.py` & `cbra-3.0.0a7/tests/types/test_unit_basemodel_identity.py`

 * *Files identical despite different names*

