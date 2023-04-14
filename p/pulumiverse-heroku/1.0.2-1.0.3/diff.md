# Comparing `tmp/pulumiverse_heroku-1.0.2.tar.gz` & `tmp/pulumiverse_heroku-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_heroku-1.0.2.tar", last modified: Mon Dec  5 08:41:28 2022, max compression
+gzip compressed data, was "pulumiverse_heroku-1.0.3.tar", last modified: Fri Apr 14 06:21:48 2023, max compression
```

## Comparing `pulumiverse_heroku-1.0.2.tar` & `pulumiverse_heroku-1.0.3.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.128646 pulumiverse_heroku-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2022-12-05 08:41:28.128646 pulumiverse_heroku-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.124647 pulumiverse_heroku-1.0.2/pulumiverse_heroku/
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.124647 pulumiverse_heroku-1.0.2/pulumiverse_heroku/account/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/account/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.124647 pulumiverse_heroku-1.0.2/pulumiverse_heroku/addon/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/addon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/addon/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/addon/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/addon/get_addon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.124647 pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21514 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7018 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/config_association.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/get_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/release.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.124647 pulumiverse_heroku-1.0.2/pulumiverse_heroku/build/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/build/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/build/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/build/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.124647 pulumiverse_heroku-1.0.2/pulumiverse_heroku/cert/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/cert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/cert/cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.124647 pulumiverse_heroku-1.0.2/pulumiverse_heroku/collaborator/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/collaborator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/collaborator/collaborator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.124647 pulumiverse_heroku-1.0.2/pulumiverse_heroku/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.128646 pulumiverse_heroku-1.0.2/pulumiverse_heroku/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/domain/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.128646 pulumiverse_heroku-1.0.2/pulumiverse_heroku/drain/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/drain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/drain/drain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.128646 pulumiverse_heroku-1.0.2/pulumiverse_heroku/formation/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/formation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/formation/formation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.128646 pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10812 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/config_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/coupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/get_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.128646 pulumiverse_heroku-1.0.2/pulumiverse_heroku/review/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/review/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/review/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16326 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/review/app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/review/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.128646 pulumiverse_heroku-1.0.2/pulumiverse_heroku/slug/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/slug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/slug/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/slug/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18449 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/slug/slug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.128646 pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/app_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/get_peering_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/get_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/inbound_ruleset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/peering_connection_accepter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/vpn_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.128646 pulumiverse_heroku-1.0.2/pulumiverse_heroku/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/ssl/ssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.128646 pulumiverse_heroku-1.0.2/pulumiverse_heroku/team/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/team/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/team/collaborator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/team/get_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/team/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/team/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku/team/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:41:28.124647 pulumiverse_heroku-1.0.2/pulumiverse_heroku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2022-12-05 08:41:28.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2022-12-05 08:41:28.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 08:41:28.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 08:41:28.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-05 08:41:28.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-05 08:41:28.000000 pulumiverse_heroku-1.0.2/pulumiverse_heroku.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-05 08:41:28.128646 pulumiverse_heroku-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2022-12-05 08:41:27.000000 pulumiverse_heroku-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.542508 pulumiverse_heroku-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-14 06:21:48.542508 pulumiverse_heroku-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.534508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.534508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/account/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/account/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.534508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/addon/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/addon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/addon/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/addon/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/addon/get_addon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.534508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21514 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/config_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.538508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/build/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/build/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/build/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.538508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/cert/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/cert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/cert/cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.538508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/collaborator/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/collaborator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/collaborator/collaborator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.538508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.538508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/domain/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.538508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/drain/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/drain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/drain/drain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.538508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/formation/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/formation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/formation/formation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.538508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/config_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/coupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/get_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.538508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/review/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/review/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/review/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/review/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/review/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.538508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/slug/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/slug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/slug/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/slug/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18449 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/slug/slug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.542508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/app_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/get_peering_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/get_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/inbound_ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/peering_connection_accepter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/vpn_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.542508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/ssl/ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.542508 pulumiverse_heroku-1.0.3/pulumiverse_heroku/team/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/team/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/team/collaborator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/team/get_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/team/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/team/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku/team/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:21:48.534508 pulumiverse_heroku-1.0.3/pulumiverse_heroku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/pulumiverse_heroku.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:21:48.542508 pulumiverse_heroku-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-14 06:21:48.000000 pulumiverse_heroku-1.0.3/setup.py
```

### Comparing `pulumiverse_heroku-1.0.2/PKG-INFO` & `pulumiverse_heroku-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_heroku
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Pulumi package for creating and managing heroku cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-heroku
 Keywords: pulumi heroku category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumiverse_heroku-1.0.2/README.md` & `pulumiverse_heroku-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/__init__.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/_inputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/_inputs.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,27 +6,39 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'ProviderCustomizationsArgs',
+    'ProviderCustomizationArgs',
     'ProviderDelaysArgs',
     'ProviderTimeoutsArgs',
 ]
 
 @pulumi.input_type
-class ProviderCustomizationsArgs:
+class ProviderCustomizationArgs:
     def __init__(__self__, *,
+                 set_addon_config_vars_in_state: Optional[pulumi.Input[bool]] = None,
                  set_app_all_config_vars_in_state: Optional[pulumi.Input[bool]] = None):
+        if set_addon_config_vars_in_state is not None:
+            pulumi.set(__self__, "set_addon_config_vars_in_state", set_addon_config_vars_in_state)
         if set_app_all_config_vars_in_state is not None:
             pulumi.set(__self__, "set_app_all_config_vars_in_state", set_app_all_config_vars_in_state)
 
     @property
+    @pulumi.getter(name="setAddonConfigVarsInState")
+    def set_addon_config_vars_in_state(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "set_addon_config_vars_in_state")
+
+    @set_addon_config_vars_in_state.setter
+    def set_addon_config_vars_in_state(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "set_addon_config_vars_in_state", value)
+
+    @property
     @pulumi.getter(name="setAppAllConfigVarsInState")
     def set_app_all_config_vars_in_state(self) -> Optional[pulumi.Input[bool]]:
         return pulumi.get(self, "set_app_all_config_vars_in_state")
 
     @set_app_all_config_vars_in_state.setter
     def set_app_all_config_vars_in_state(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "set_app_all_config_vars_in_state", value)
```

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/_utilities.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/account/feature.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/account/feature.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/addon/addon.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/addon/addon.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/addon/attachment.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/addon/attachment.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/addon/get_addon.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/addon/get_addon.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/_inputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/app.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/app.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/config.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/config_association.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/config_association.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/feature.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/feature.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/get_app.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/outputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/release.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/release.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/app/webhook.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/app/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/build/_inputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/build/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/build/build.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/build/build.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/build/outputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/build/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/cert/cert.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/cert/cert.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/collaborator/collaborator.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/collaborator/collaborator.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/config/config.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/config/config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/config/outputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/config/outputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,27 @@
     'Delays',
     'Timeouts',
 ]
 
 @pulumi.output_type
 class Customizations(dict):
     def __init__(__self__, *,
+                 set_addon_config_vars_in_state: Optional[bool] = None,
                  set_app_all_config_vars_in_state: Optional[bool] = None):
+        if set_addon_config_vars_in_state is not None:
+            pulumi.set(__self__, "set_addon_config_vars_in_state", set_addon_config_vars_in_state)
         if set_app_all_config_vars_in_state is not None:
             pulumi.set(__self__, "set_app_all_config_vars_in_state", set_app_all_config_vars_in_state)
 
     @property
+    @pulumi.getter(name="setAddonConfigVarsInState")
+    def set_addon_config_vars_in_state(self) -> Optional[bool]:
+        return pulumi.get(self, "set_addon_config_vars_in_state")
+
+    @property
     @pulumi.getter(name="setAppAllConfigVarsInState")
     def set_app_all_config_vars_in_state(self) -> Optional[bool]:
         return pulumi.get(self, "set_app_all_config_vars_in_state")
 
 
 @pulumi.output_type
 class Delays(dict):
```

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/config/vars.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/domain/domain.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/domain/domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,10 +211,10 @@
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Output[str]:
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter(name="sniEndpointId")
-    def sni_endpoint_id(self) -> pulumi.Output[str]:
+    def sni_endpoint_id(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "sni_endpoint_id")
```

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/drain/drain.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/drain/drain.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/formation/formation.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/formation/formation.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/_inputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/config_var.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/config_var.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/coupling.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/coupling.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/get_pipeline.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/get_pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/outputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/pipeline/pipeline.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/provider.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 __all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
                  api_key: Optional[pulumi.Input[str]] = None,
-                 customizations: Optional[pulumi.Input['ProviderCustomizationsArgs']] = None,
+                 customizations: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderCustomizationArgs']]]] = None,
                  delays: Optional[pulumi.Input['ProviderDelaysArgs']] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  headers: Optional[pulumi.Input[str]] = None,
                  timeouts: Optional[pulumi.Input['ProviderTimeoutsArgs']] = None,
                  url: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
@@ -47,19 +47,19 @@
 
     @api_key.setter
     def api_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_key", value)
 
     @property
     @pulumi.getter
-    def customizations(self) -> Optional[pulumi.Input['ProviderCustomizationsArgs']]:
+    def customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProviderCustomizationArgs']]]]:
         return pulumi.get(self, "customizations")
 
     @customizations.setter
-    def customizations(self, value: Optional[pulumi.Input['ProviderCustomizationsArgs']]):
+    def customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderCustomizationArgs']]]]):
         pulumi.set(self, "customizations", value)
 
     @property
     @pulumi.getter
     def delays(self) -> Optional[pulumi.Input['ProviderDelaysArgs']]:
         return pulumi.get(self, "delays")
 
@@ -106,15 +106,15 @@
 
 class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  api_key: Optional[pulumi.Input[str]] = None,
-                 customizations: Optional[pulumi.Input[pulumi.InputType['ProviderCustomizationsArgs']]] = None,
+                 customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProviderCustomizationArgs']]]]] = None,
                  delays: Optional[pulumi.Input[pulumi.InputType['ProviderDelaysArgs']]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  headers: Optional[pulumi.Input[str]] = None,
                  timeouts: Optional[pulumi.Input[pulumi.InputType['ProviderTimeoutsArgs']]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
@@ -150,15 +150,15 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  api_key: Optional[pulumi.Input[str]] = None,
-                 customizations: Optional[pulumi.Input[pulumi.InputType['ProviderCustomizationsArgs']]] = None,
+                 customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProviderCustomizationArgs']]]]] = None,
                  delays: Optional[pulumi.Input[pulumi.InputType['ProviderDelaysArgs']]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  headers: Optional[pulumi.Input[str]] = None,
                  timeouts: Optional[pulumi.Input[pulumi.InputType['ProviderTimeoutsArgs']]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
```

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/review/_inputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/review/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/review/app_config.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/review/app_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/review/outputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/review/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/slug/_inputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/slug/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/slug/outputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/slug/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/slug/slug.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/slug/slug.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/__init__.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/_inputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/app_access.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/app_access.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/get_peering_info.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/get_peering_info.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/get_space.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/get_space.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/inbound_ruleset.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/inbound_ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/outputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/peering_connection_accepter.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/peering_connection_accepter.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/space.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/space.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/space/vpn_connection.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/space/vpn_connection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/ssl/ssl.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/ssl/ssl.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/team/collaborator.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/team/collaborator.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/team/get_members.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/team/get_members.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/team/get_team.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/team/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/team/member.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/team/member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku/team/outputs.py` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku/team/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku.egg-info/PKG-INFO` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-heroku
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Pulumi package for creating and managing heroku cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-heroku
 Keywords: pulumi heroku category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumiverse_heroku-1.0.2/pulumiverse_heroku.egg-info/SOURCES.txt` & `pulumiverse_heroku-1.0.3/pulumiverse_heroku.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_heroku-1.0.2/setup.py` & `pulumiverse_heroku-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.0.2"
-PLUGIN_VERSION = "1.0.2"
+VERSION = "1.0.3"
+PLUGIN_VERSION = "1.0.3"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'heroku', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse'])
         except OSError as error:
```

