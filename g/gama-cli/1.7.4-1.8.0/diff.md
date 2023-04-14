# Comparing `tmp/gama_cli-1.7.4.tar.gz` & `tmp/gama_cli-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gama_cli-1.7.4.tar", last modified: Wed Apr 12 01:54:12 2023, max compression
+gzip compressed data, was "gama_cli-1.8.0.tar", last modified: Fri Apr 14 02:18:10 2023, max compression
```

## Comparing `gama_cli-1.7.4.tar` & `gama_cli-1.8.0.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-12 01:54:12.072901 gama_cli-1.7.4/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2302 2023-04-12 01:54:12.072901 gama_cli-1.7.4/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1664 2023-04-12 01:53:22.000000 gama_cli-1.7.4/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-12 01:54:12.068901 gama_cli-1.7.4/gama_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/__init__.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-12 01:54:12.068901 gama_cli-1.7.4/gama_cli/assets/
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-12 01:54:12.068901 gama_cli-1.7.4/gama_cli/assets/greenstream/
--rw-rw-r--   0 runner    (1000) runner    (1001)      173 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/assets/greenstream/config.sim.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)      597 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/assets/greenstream/config.stubs.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)      583 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/assets/greenstream/config.variant.bravo.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)      184 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/assets/greenstream/config.variant.educat.yml
--rw-rw-r--   0 runner    (1000) runner    (1001)     2539 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/banner.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1231 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/cli.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-12 01:54:12.068901 gama_cli-1.7.4/gama_cli/config/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1417 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/config/gama_gs.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1995 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/config/gama_vessel.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-12 01:54:12.068901 gama_cli-1.7.4/gama_cli/docker/
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-12 01:54:12.068901 gama_cli-1.7.4/gama_cli/docker/gs/
--rw-rw-r--   0 runner    (1000) runner    (1001)      503 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/gs/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       73 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/gs/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      172 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/gs/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      640 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/gs/docker-compose.network-vpn.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/gs/docker-compose.prod.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      157 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/gs/docker-compose.warthog-combo.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      430 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/gs/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-12 01:54:12.068901 gama_cli-1.7.4/gama_cli/docker/sim/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1038 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/sim/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      744 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/sim/docker-compose.standalone.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-12 01:54:12.072901 gama_cli-1.7.4/gama_cli/docker/vessel/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2582 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      193 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.gpu.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      175 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      459 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      912 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.network-vpn.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      308 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.prod.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      723 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      607 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.variant-educat.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)     1942 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-12 01:54:12.072901 gama_cli-1.7.4/gama_cli/groups/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/groups/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1061 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/groups/attach.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      445 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/groups/docker.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      353 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/groups/git.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     7231 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/groups/gs.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2523 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/groups/misc.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1435 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/groups/setup.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     5830 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/groups/sim.py
--rw-rw-r--   0 runner    (1000) runner    (1001)    14887 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/groups/vessel.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     4959 2023-04-12 01:53:22.000000 gama_cli-1.7.4/gama_cli/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-12 01:54:12.068901 gama_cli-1.7.4/gama_cli.egg-info/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2302 2023-04-12 01:54:12.000000 gama_cli-1.7.4/gama_cli.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1701 2023-04-12 01:54:12.000000 gama_cli-1.7.4/gama_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-12 01:54:12.000000 gama_cli-1.7.4/gama_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       46 2023-04-12 01:54:12.000000 gama_cli-1.7.4/gama_cli.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-04-12 01:54:12.000000 gama_cli-1.7.4/gama_cli.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        9 2023-04-12 01:54:12.000000 gama_cli-1.7.4/gama_cli.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-12 01:54:01.000000 gama_cli-1.7.4/gama_cli.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      980 2023-04-12 01:54:12.072901 gama_cli-1.7.4/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-04-12 01:53:22.000000 gama_cli-1.7.4/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2302 2023-04-14 02:18:10.343063 gama_cli-1.8.0/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1664 2023-04-14 02:17:24.000000 gama_cli-1.8.0/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/__init__.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.339063 gama_cli-1.8.0/gama_cli/assets/
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/assets/greenstream/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      173 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/assets/greenstream/config.sim.yml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      597 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/assets/greenstream/config.stubs.yml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      583 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/assets/greenstream/config.variant.bravo.yml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      184 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/assets/greenstream/config.variant.educat.yml
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2539 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/banner.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     3133 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/cli.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/config/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1632 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/config/gama_gs.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2418 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/config/gama_vessel.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.339063 gama_cli-1.8.0/gama_cli/docker/
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/docker/gs/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      503 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       73 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      172 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      640 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.network-vpn.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.prod.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      157 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.warthog-combo.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      430 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/docker/sim/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1038 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/sim/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      744 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/sim/docker-compose.standalone.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/docker/vessel/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2582 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      193 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.gpu.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      175 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      459 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      912 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.network-vpn.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      308 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.prod.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      723 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      607 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.variant-educat.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1942 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/groups/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      839 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/attach.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      327 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/docker.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      249 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/git.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     5893 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/gs.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1905 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/misc.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1168 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/setup.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     4772 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/sim.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)    12547 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/groups/vessel.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     5037 2023-04-14 02:17:24.000000 gama_cli-1.8.0/gama_cli/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli/schemas/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1118 2023-04-14 02:17:58.000000 gama_cli-1.8.0/gama_cli/schemas/gama_gs.schema.json
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2976 2023-04-14 02:17:58.000000 gama_cli-1.8.0/gama_cli/schemas/gama_vessel.schema.json
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-14 02:18:10.343063 gama_cli-1.8.0/gama_cli.egg-info/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2302 2023-04-14 02:18:10.000000 gama_cli-1.8.0/gama_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1779 2023-04-14 02:18:10.000000 gama_cli-1.8.0/gama_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-14 02:18:10.000000 gama_cli-1.8.0/gama_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       46 2023-04-14 02:18:10.000000 gama_cli-1.8.0/gama_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       78 2023-04-14 02:18:10.000000 gama_cli-1.8.0/gama_cli.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        9 2023-04-14 02:18:10.000000 gama_cli-1.8.0/gama_cli.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-14 02:17:57.000000 gama_cli-1.8.0/gama_cli.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1002 2023-04-14 02:18:10.343063 gama_cli-1.8.0/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-04-14 02:17:24.000000 gama_cli-1.8.0/setup.py
```

### Comparing `gama_cli-1.7.4/PKG-INFO` & `gama_cli-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama_cli
-Version: 1.7.4
+Version: 1.8.0
 Summary: A CLI for interacting with the GAMA platform
 Home-page: https://github.com/Greenroom-Robotics/gama_cli
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `gama_cli-1.7.4/README.md` & `gama_cli-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.4/gama_cli/assets/greenstream/config.stubs.yml` & `gama_cli-1.8.0/gama_cli/assets/greenstream/config.stubs.yml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.4/gama_cli/assets/greenstream/config.variant.bravo.yml` & `gama_cli-1.8.0/gama_cli/assets/greenstream/config.variant.bravo.yml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.4/gama_cli/banner.py` & `gama_cli-1.8.0/gama_cli/banner.py`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.4/gama_cli/config/gama_gs.py` & `gama_cli-1.8.0/gama_cli/config/gama_gs.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from enum import Enum
 from dacite import from_dict, Config
 import yaml
 import click
 from gama_cli.helpers import dacite_to_dict
 
 GAMA_GS_CONFIG_PATH = ".gama/gama_gs.yml"
+GAMA_GS_SCHEMA_URL = "https://greenroom-robotics.github.io/gama/schemas/gama_gs.schema.json"
 
 
 class Mode(str, Enum):
     NONE = "none"
     XBOX = "xbox"
     THRUSTMASTER = "thrustmaster"
     THRUSTMASTER_COMBO = "thrustmaster_combo"
@@ -47,8 +48,10 @@
         click.echo(click.style(f"{GAMA_GS_CONFIG_PATH} not found. Using default values..", fg="yellow"))  # type: ignore
         return GamaGsConfig()
 
 
 def write_gama_gs_config(config: GamaGsConfig):
     with open(GAMA_GS_CONFIG_PATH, "w") as stream:
         click.echo(click.style(f"Writing {GAMA_GS_CONFIG_PATH}...", fg="green"))  # type: ignore
-        yaml.dump(dacite_to_dict(config), stream)
+        headers = f"# yaml-language-server: $schema={GAMA_GS_SCHEMA_URL}"
+        data = "\n".join([headers, yaml.dump(dacite_to_dict(config))])
+        stream.write(data)
```

### Comparing `gama_cli-1.7.4/gama_cli/config/gama_vessel.py` & `gama_cli-1.8.0/gama_cli/config/gama_vessel.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 import click
 from typing import Optional
 import os
 from pathlib import Path
 from gama_cli.helpers import dacite_to_dict
 
 GAMA_VESSEL_CONFIG_PATH = ".gama/gama_vessel.yml"
+GAMA_VESSEL_SCHEMA_URL = (
+    "https://greenroom-robotics.github.io/gama/schemas/gama_vessel.schema.json"
+)
 
 
 class Mode(str, Enum):
     SIMULATOR = "simulator"
     HARDWARE = "hardware"
     STUBS = "stubs"
 
@@ -47,14 +50,18 @@
     extensions: GamaVesselConfigExtensions = GamaVesselConfigExtensions()
     network: Network = Network.SHARED
     prod: bool = False
     log_level: LogLevel = LogLevel.INFO
     ubiquity_user: Optional[str] = None
     ubiquity_pass: Optional[str] = None
     ubiquity_ip: Optional[str] = None
+    ddsrouter_remote_ip: Optional[str] = None
+    ddsrouter_remote_port: Optional[str] = None
+    ddsrouter_listen_ip: Optional[str] = None
+    ddsrouter_listen_port: Optional[str] = None
 
 
 def read_gama_vessel_config():
     try:
         with open(GAMA_VESSEL_CONFIG_PATH) as stream:
             return from_dict(
                 GamaVesselConfig,
@@ -68,8 +75,10 @@
 
 def write_gama_vessel_config(config: GamaVesselConfig):
     # Make the config dir if it doesn't exist
     os.makedirs(Path(GAMA_VESSEL_CONFIG_PATH).parent, exist_ok=True)
 
     with open(GAMA_VESSEL_CONFIG_PATH, "w") as stream:
         click.echo(click.style(f"Writing {GAMA_VESSEL_CONFIG_PATH}...", fg="green"))  # type: ignore
-        yaml.dump(dacite_to_dict(config), stream)
+        headers = f"# yaml-language-server: $schema={GAMA_VESSEL_SCHEMA_URL}"
+        data = "\n".join([headers, yaml.dump(dacite_to_dict(config))])
+        stream.write(data)
```

### Comparing `gama_cli-1.7.4/gama_cli/docker/gs/docker-compose.network-vpn.yaml` & `gama_cli-1.8.0/gama_cli/docker/gs/docker-compose.network-vpn.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.4/gama_cli/docker/sim/docker-compose.dev.yaml` & `gama_cli-1.8.0/gama_cli/docker/sim/docker-compose.dev.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.4/gama_cli/docker/sim/docker-compose.standalone.yaml` & `gama_cli-1.8.0/gama_cli/docker/sim/docker-compose.standalone.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.dev.yaml` & `gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.dev.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.network-vpn.yaml` & `gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.network-vpn.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml` & `gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.variant-bravo.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.variant-educat.yaml` & `gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.variant-educat.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.4/gama_cli/docker/vessel/docker-compose.yaml` & `gama_cli-1.8.0/gama_cli/docker/vessel/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `gama_cli-1.7.4/gama_cli/groups/attach.py` & `gama_cli-1.8.0/gama_cli/groups/attach.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import click
 
 from gama_cli.helpers import call
 
 
-class Attach:
-    def __init__(self, cli: click.Group):
-        @cli.group(help="Attaches vscode to a running container")
-        def attach():
-            pass
-
-        @attach.command(name="vessel")
-        def vessel():
-            """Attaches vscode to the vessel container"""
-            container = b"gama_vessel".hex()
-            path = "/home/ros/gama_vessel"
-            call(f"code --folder-uri=vscode-remote://attached-container+{container}/{path}")
-
-        @attach.command(name="gs")
-        def gs():
-            """Attaches vscode to the gs container"""
-            container = b"gama_gs".hex()
-            path = "/home/ros/gama_gs"
-            call(f"code --folder-uri=vscode-remote://attached-container+{container}/{path}")
-
-        @attach.command(name="ui")
-        def ui():
-            """Attaches vscode to the ui container"""
-            container = b"gama_ui".hex()
-            path = "/app"
-            call(f"code --folder-uri=vscode-remote://attached-container+{container}/{path}")
+@click.group(help="Attaches vscode to a running container")
+def attach():
+    pass
+
+
+@click.command(name="vessel")
+def vessel():
+    """Attaches vscode to the vessel container"""
+    container = b"gama_vessel".hex()
+    path = "/home/ros/gama_vessel"
+    call(f"code --folder-uri=vscode-remote://attached-container+{container}/{path}")
+
+
+@click.command(name="gs")
+def gs():
+    """Attaches vscode to the gs container"""
+    container = b"gama_gs".hex()
+    path = "/home/ros/gama_gs"
+    call(f"code --folder-uri=vscode-remote://attached-container+{container}/{path}")
+
+
+@click.command(name="ui")
+def ui():
+    """Attaches vscode to the ui container"""
+    container = b"gama_ui".hex()
+    path = "/app"
+    call(f"code --folder-uri=vscode-remote://attached-container+{container}/{path}")
```

### Comparing `gama_cli-1.7.4/gama_cli/groups/gs.py` & `gama_cli-1.8.0/gama_cli/groups/gs.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,175 +26,178 @@
 DOCKER_GS_DEV = docker_compose_path("./gs/docker-compose.dev.yaml")
 DOCKER_GS_NETWORK_SHARED = docker_compose_path("./gs/docker-compose.network-shared.yaml")
 DOCKER_GS_NETWORK_HOST = docker_compose_path("./gs/docker-compose.network-host.yaml")
 DOCKER_GS_NETWORK_VPN = docker_compose_path("./gs/docker-compose.network-vpn.yaml")
 DOCKER_GS_WARTHOG_COMBO = docker_compose_path("./gs/docker-compose.warthog-combo.yaml")
 
 
-class Gs:
-    def _get_compose_files(
-        self, mode: Optional[Mode] = None, network: Network = Network.SHARED, prod: bool = False
-    ) -> List[ValidPath]:
-        compose_files: List[ValidPath] = [DOCKER_GS]
-
-        if not prod:
-            compose_files.append(DOCKER_GS_DEV)
-        if mode == Mode.WARTHOG_COMBO:
-            compose_files.append(DOCKER_GS_WARTHOG_COMBO)
-        if network == Network.SHARED:
-            compose_files.append(DOCKER_GS_NETWORK_SHARED)
-        if network == Network.VPN:
-            compose_files.append(DOCKER_GS_NETWORK_VPN)
-        if network == Network.HOST:
-            compose_files.append(DOCKER_GS_NETWORK_HOST)
-
-        return compose_files
-
-    def _get_container_name(self, mode: Mode) -> str:
-        return f"gama_gs_{mode.value}"
-
-    def __init__(self, cli: click.Group, dev_mode: bool = False):
-        @cli.group(help="Commands for the ground-station")
-        def gs():
-            pass
-
-        @gs.command(name="up")
-        @click.option(
-            "--build",
-            type=bool,
-            default=False,
-            help="Should we rebuild the docker containers? Default: False",
-        )
-        @click.argument("args", nargs=-1)
-        def up(
-            build: bool,
-            args: List[str],
-        ):
-            """Starts the ground-station"""
-            config = read_gama_gs_config()
-            build = maybe_ignore_build(dev_mode, build)
-            prod = maybe_ignore_prod(dev_mode, config.prod)
-
-            docker = DockerClient(
-                compose_files=self._get_compose_files(
-                    mode=config.mode, network=config.network, prod=prod
-                ),
-                compose_project_directory=get_project_root(),
+def _get_compose_files(
+    mode: Optional[Mode] = None, network: Network = Network.SHARED, prod: bool = False
+) -> List[ValidPath]:
+    compose_files: List[ValidPath] = [DOCKER_GS]
+
+    if not prod:
+        compose_files.append(DOCKER_GS_DEV)
+    if mode == Mode.WARTHOG_COMBO:
+        compose_files.append(DOCKER_GS_WARTHOG_COMBO)
+    if network == Network.SHARED:
+        compose_files.append(DOCKER_GS_NETWORK_SHARED)
+    if network == Network.VPN:
+        compose_files.append(DOCKER_GS_NETWORK_VPN)
+    if network == Network.HOST:
+        compose_files.append(DOCKER_GS_NETWORK_HOST)
+
+    return compose_files
+
+
+@click.group(help="Commands for the ground-station")
+def gs():
+    pass
+
+
+@click.command(name="up")
+@click.option(
+    "--build",
+    type=bool,
+    default=False,
+    help="Should we rebuild the docker containers? Default: False",
+)
+@click.argument("args", nargs=-1)
+def up(
+    build: bool,
+    args: List[str],
+):
+    """Starts the ground-station"""
+    dev_mode = os.environ["GAMA_CLI_DEV_MODE"] == "true"
+
+    config = read_gama_gs_config()
+    build = maybe_ignore_build(dev_mode, build)
+    prod = maybe_ignore_prod(dev_mode, config.prod)
+
+    docker = DockerClient(
+        compose_files=_get_compose_files(mode=config.mode, network=config.network, prod=prod),
+        compose_project_directory=get_project_root(),
+    )
+
+    buttons = "True" if config.mode == Mode.WARTHOG_COMBO else "False"
+
+    gama_gs_command_args = f"mode:={config.mode.value} buttons:={buttons} remote_cmd_override:={config.remote_cmd_override}"
+
+    if config.log_level:
+        gama_gs_command_args += f" log_level:={config.log_level.value}"
+
+    os.environ["GAMA_GS_COMMAND_ARGS"] = gama_gs_command_args
+    docker.compose.up(detach=True, build=build)
+
+
+@click.command(name="down")
+@click.argument("args", nargs=-1)
+def down(args: List[str]):
+    """Stops the ground-station"""
+    config = read_gama_gs_config()
+
+    docker = DockerClient(
+        compose_files=_get_compose_files(config.mode),
+        compose_project_directory=get_project_root(),
+    )
+    docker.compose.down()
+
+
+@click.command(name="install")
+def install():  # type: ignore
+    """Install GAMA on a gs"""
+    docker = DockerClient(
+        compose_files=_get_compose_files(),
+        compose_project_directory=get_project_root(),
+    )
+    try:
+        docker.compose.pull()
+    except Exception:
+        click.echo(
+            click.style(
+                "Failed to pull GAMA files. Have you ran `gama_cli authenticate` ?",
+                fg="yellow",
             )
+        )
 
-            buttons = "True" if config.mode == Mode.WARTHOG_COMBO else "False"
-
-            gama_gs_command_args = f"mode:={config.mode.value} buttons:={buttons} remote_cmd_override:={config.remote_cmd_override}"
-
-            if config.log_level:
-                gama_gs_command_args += f" log_level:={config.log_level.value}"
-
-            os.environ["GAMA_GS_COMMAND_ARGS"] = gama_gs_command_args
-            docker.compose.up(detach=True, build=build)
-
-        @gs.command(name="down")
-        @click.argument("args", nargs=-1)
-        def down(args: List[str]):
-            """Stops the ground-station"""
-            config = read_gama_gs_config()
-
-            docker = DockerClient(
-                compose_files=self._get_compose_files(config.mode),
-                compose_project_directory=get_project_root(),
-            )
-            docker.compose.down()
 
-        @gs.command(name="install")
-        def install():  # type: ignore
-            """Install GAMA on a gs"""
-            docker = DockerClient(
-                compose_files=self._get_compose_files(),
-                compose_project_directory=get_project_root(),
-            )
-            try:
-                docker.compose.pull()
-            except Exception:
-                click.echo(
-                    click.style(
-                        "Failed to pull GAMA files. Have you ran `gama_cli authenticate` ?",
-                        fg="yellow",
-                    )
-                )
-
-        @gs.command(name="configure")
-        def configure():  # type: ignore
-            """Configure GAMA Ground Station"""
-            # Check if the file exists
-            if os.path.exists(GAMA_GS_CONFIG_PATH):
-                click.echo(
-                    click.style(
-                        f"GAMA Ground Station config already exists: {GAMA_GS_CONFIG_PATH}",
-                        fg="yellow",
-                    )
-                )
-                result = click.prompt(
-                    "Do you want to overwrite it?", default="y", type=click.Choice(["y", "n"])
-                )
-                if result == "n":
-                    return
-
-            config = GamaGsConfig(
-                mode=click.prompt("Mode", type=click.Choice([mode.value for mode in Mode])),
-                network=click.prompt(
-                    "Network", type=click.Choice([network.value for network in Network])
-                ),
-                prod=click.prompt("Prod", type=bool, default=True),
-                remote_cmd_override=click.prompt(
-                    "Remote Command Override", type=bool, default=False
-                ),
-                log_level=click.prompt(
-                    "Log Level",
-                    type=click.Choice([log_level.value for log_level in LogLevel]),
-                    default=LogLevel.INFO.value,
-                ),
+@click.command(name="configure")
+def configure():  # type: ignore
+    """Configure GAMA Ground Station"""
+    # Check if the file exists
+    if os.path.exists(GAMA_GS_CONFIG_PATH):
+        click.echo(
+            click.style(
+                f"GAMA Ground Station config already exists: {GAMA_GS_CONFIG_PATH}",
+                fg="yellow",
             )
-            write_gama_gs_config(config)
-
-        if dev_mode:
+        )
+        result = click.prompt(
+            "Do you want to overwrite it?", default="y", type=click.Choice(["y", "n"])
+        )
+        if result == "n":
+            return
 
-            @gs.command(name="build")
-            def build():
-                """Builds the ground-station"""
-                docker = DockerClient(
-                    compose_files=self._get_compose_files(),
-                    compose_project_directory=get_project_root(),
-                )
-                docker.compose.build()
-
-            @gs.command(name="bake")
-            @click.option(
-                "--version",
-                type=str,
-                required=True,
-                help="The version to bake. Default: latest",
-            )
-            @click.option(
-                "--push",
-                type=bool,
-                default=False,
-                is_flag=True,
-                help="Should we push the images to the registry? Default: False",
-            )
-            @click.argument("services", nargs=-1)
-            def bake(version: str, push: bool, services: List[str]):  # type: ignore
-                """Bakes the gs docker containers"""
-                compose_files = self._get_compose_files()
-                docker_bake(
-                    version=version,
-                    services=services,
-                    push=push,
-                    compose_files=compose_files,
-                )
-
-            @gs.command(name="test")
-            def test():
-                """Tests the ground-station"""
-                docker = DockerClient(
-                    compose_files=self._get_compose_files(),
-                    compose_project_directory=get_project_root(),
-                )
-                docker.compose.run("gama_gs", "platform ros test".split(" "))
+    config = GamaGsConfig(
+        mode=click.prompt(
+            "Mode", type=click.Choice([mode.value for mode in Mode]), default=Mode.WARTHOG_COMBO
+        ),
+        network=click.prompt(
+            "Network",
+            type=click.Choice([network.value for network in Network]),
+            default=Network.HOST,
+        ),
+        prod=click.prompt("Prod", type=bool, default=True),
+        remote_cmd_override=click.prompt("Remote Command Override", type=bool, default=False),
+        log_level=click.prompt(
+            "Log Level",
+            type=click.Choice([log_level.value for log_level in LogLevel]),
+            default=LogLevel.INFO.value,
+        ),
+    )
+    write_gama_gs_config(config)
+
+
+@click.command(name="build")
+def build():
+    """Builds the ground-station"""
+    docker = DockerClient(
+        compose_files=_get_compose_files(),
+        compose_project_directory=get_project_root(),
+    )
+    docker.compose.build()
+
+
+@click.command(name="bake")
+@click.option(
+    "--version",
+    type=str,
+    required=True,
+    help="The version to bake. Default: latest",
+)
+@click.option(
+    "--push",
+    type=bool,
+    default=False,
+    is_flag=True,
+    help="Should we push the images to the registry? Default: False",
+)
+@click.argument("services", nargs=-1)
+def bake(version: str, push: bool, services: List[str]):  # type: ignore
+    """Bakes the gs docker containers"""
+    compose_files = _get_compose_files()
+    docker_bake(
+        version=version,
+        services=services,
+        push=push,
+        compose_files=compose_files,
+    )
+
+
+@click.command(name="test")
+def test():
+    """Tests the ground-station"""
+    docker = DockerClient(
+        compose_files=_get_compose_files(),
+        compose_project_directory=get_project_root(),
+    )
+    docker.compose.run("gama_gs", "platform ros test".split(" "))
```

### Comparing `gama_cli-1.7.4/gama_cli/groups/misc.py` & `gama_cli-1.8.0/gama_cli/groups/misc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,67 @@
 import click
 
 from gama_cli.helpers import call, get_gama_version
 import subprocess
 
 
-class Misc:
-    def __init__(self, cli: click.Group, dev_mode: bool = False):
-        if dev_mode:
-
-            @cli.command(name="lint")
-            def lint():
-                """Lints all the things"""
-                call("pre-commit run --all")
-                call("gama_cli vessel lint-ui")
-
-            @cli.command(name="test")
-            def test():
-                """Tests all the things"""
-                call("gama_cli lint")
-                # call("gama_cli gs test")
-                call("gama_cli vessel test-ui")
-                # call("gama_cli vessel test-ros")
-
-            @cli.command(name="test-e2e")
-            def test_e2e():
-                """Brings up all containers and runs the e2e tests"""
-                call("gama_cli gs up")
-                call("gama_cli vessel up --mode stubs")
-                call("gama_cli vessel test-e2e")
-
-        @cli.command(name="upgrade")
-        @click.option("--version", help="The version to upgrade to.")
-        def upgrade(version: str):
-            """Upgrade GAMA CLI"""
-            click.echo(f"Current version: {get_gama_version()}")
-            result = click.prompt(
-                "Are you sure you want to upgrade?", default="y", type=click.Choice(["y", "n"])
-            )
-            if result == "n":
-                return
-
-            if version:
-                call(f"pip install --upgrade gama-cli=={version}")
-            else:
-                call("pip install --upgrade gama-cli")
-
-            click.echo(click.style("Upgrade of GAMA CLI complete.", fg="green"))
-            click.echo(
-                click.style(
-                    "Run `gama vessel install` or `gama gs install` to upgrade GAMA.", fg="green"
-                )
-            )
-
-        @cli.command(name="authenticate")
-        @click.option(
-            "--username",
-            help="The username to use for authentication.",
-            required=True,
-            prompt=True,
-        )
-        @click.option(
-            "--token", help="The token to use for authentication.", required=True, prompt=True
-        )
-        def authenticate(username: str, token: str):
-            """
-            Authenticate with the GAMA package repository so that you can pull images.
-
-            To get a username and token you'll need to contact a Greenroom Robotics employee.
-            """
-            call(f"echo {token} | docker login ghcr.io -u {username} --password-stdin")
+@click.command(name="lint")
+def lint():
+    """Lints all the things"""
+    call("pre-commit run --all")
+    call("gama_cli vessel lint-ui")
+
+
+@click.command(name="test")
+def test():
+    """Tests all the things"""
+    call("gama_cli lint")
+    # call("gama_cli gs test")
+    call("gama_cli vessel test-ui")
+    # call("gama_cli vessel test-ros")
+
+
+@click.command(name="test-e2e")
+def test_e2e():
+    """Brings up all containers and runs the e2e tests"""
+    call("gama_cli gs up")
+    call("gama_cli vessel up --mode stubs")
+    call("gama_cli vessel test-e2e")
+
+
+@click.command(name="upgrade")
+@click.option("--version", help="The version to upgrade to.")
+def upgrade(version: str):
+    """Upgrade GAMA CLI"""
+    click.echo(f"Current version: {get_gama_version()}")
+    result = click.prompt(
+        "Are you sure you want to upgrade?", default="y", type=click.Choice(["y", "n"])
+    )
+    if result == "n":
+        return
+
+    if version:
+        call(f"pip install --upgrade gama-cli=={version}")
+    else:
+        call("pip install --upgrade gama-cli")
+
+    click.echo(click.style("Upgrade of GAMA CLI complete.", fg="green"))
+    click.echo(
+        click.style("Run `gama vessel install` or `gama gs install` to upgrade GAMA.", fg="green")
+    )
+
+
+@click.command(name="authenticate")
+@click.option(
+    "--username",
+    help="The username to use for authentication.",
+    required=True,
+    prompt=True,
+)
+@click.option("--token", help="The token to use for authentication.", required=True, prompt=True)
+def authenticate(username: str, token: str):
+    """
+    Authenticate with the GAMA package repository so that you can pull images.
+
+    To get a username and token you'll need to contact a Greenroom Robotics employee.
+    """
+    call(f"echo {token} | docker login ghcr.io -u {username} --password-stdin")
```

### Comparing `gama_cli-1.7.4/gama_cli/groups/setup.py` & `gama_cli-1.8.0/gama_cli/groups/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,40 +9,40 @@
 def write_file(path: str, content: str):
     project_root = get_project_root() or Path()
     click.echo(f"Writing file {project_root / path}")
     with open(project_root / path, "w") as f:
         f.write(content)
 
 
-class Setup:
-    def __init__(self, cli: click.Group):
-        @cli.group(help="Setup commands")
-        def setup():
-            pass
-
-        @setup.command(name="secrets")
-        @click.argument("pat")
-        def secrets(pat: str):  # type: ignore
-            """Setup the .secrets files as docker secrets needs these to build containers"""
-            write_file(".secrets/API_TOKEN_GITHUB", pat)
-
-            greenroom_apt_conf = "\n".join(
-                [
-                    "machine raw.githubusercontent.com/Greenroom-Robotics",
-                    f"login {pat}",
-                    "password",
-                ]
-            )
-            write_file(".secrets/apt.conf", greenroom_apt_conf)
-
-        @setup.command(name="env")
-        def env():  # type: ignore
-            """Setup the .env file"""
-
-            random_domain_id_int = random.randint(0, 10000)
-            env = "\n".join(
-                [
-                    f"DISPLAY={os.environ['DISPLAY']}",
-                    f"ROS_DOMAIN_ID={random_domain_id_int}",
-                ]
-            )
-            write_file(".env", env)
+@click.group(help="Setup commands")
+def setup():
+    pass
+
+
+@click.command(name="secrets")
+@click.argument("pat")
+def secrets(pat: str):  # type: ignore
+    """Setup the .secrets files as docker secrets needs these to build containers"""
+    write_file(".secrets/API_TOKEN_GITHUB", pat)
+
+    greenroom_apt_conf = "\n".join(
+        [
+            "machine raw.githubusercontent.com/Greenroom-Robotics",
+            f"login {pat}",
+            "password",
+        ]
+    )
+    write_file(".secrets/apt.conf", greenroom_apt_conf)
+
+
+@click.command(name="env")
+def env():  # type: ignore
+    """Setup the .env file"""
+
+    random_domain_id_int = random.randint(0, 10000)
+    env = "\n".join(
+        [
+            f"DISPLAY={os.environ['DISPLAY']}",
+            f"ROS_DOMAIN_ID={random_domain_id_int}",
+        ]
+    )
+    write_file(".env", env)
```

### Comparing `gama_cli-1.7.4/gama_cli/groups/sim.py` & `gama_cli-1.8.0/gama_cli/groups/sim.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,144 +20,143 @@
 
 Mode: Enum = Enum("mode", ("dev", "standalone"))
 
 mode_default = "standalone"
 mode_help = f"The mode to run the sim. Default: {mode_default}"
 
 
-class Sim:
-    def _get_compose_files(self, mode: str) -> List[ValidPath]:
-        if mode == "dev":
-            return [DOCKER_SIM_DEV]
-        else:
-            return [DOCKER_SIM_STANDALONE]
-
-    def __init__(self, cli: click.Group):
-        @cli.group(help="Commands for the sim")
-        def sim():
-            pass
-
-        @sim.command(name="build")
-        @click.option(
-            "-m",
-            "--mode",
-            type=click.Choice(list(map(lambda x: x.name, Mode)), case_sensitive=False),
-            default=mode_default,
-            help=mode_help,
-        )
-        @click.option(
-            "-c",
-            "--clean",
-            help="Should the ue4 build assets be cleaned?",
-            type=bool,
-        )
-        @click.argument("args", nargs=-1)
-        def build(mode: str, clean: bool, args: List[str]):
-            """Builds the sim"""
-            # If building standalone, we first build the dev sim
-            # TODO move this to a multistage build
-
-            # check UE cache dir
-            prj_root = get_project_root()
-            if not prj_root:
-                raise RuntimeError("Could not find project root")
-
-            cache_dir = Path(prj_root / ".cache")
-            Path(cache_dir).mkdir(exist_ok=True)
-
-            if not check_directory_ownership(cache_dir):
-                raise click.ClickException(
-                    "'.cache' directory does not belong to current user/group."
-                )
-
-            docker_standalone = DockerClient(
-                compose_files=self._get_compose_files("standalone"),
-                compose_project_directory=get_project_root(),
-            )
-            docker_dev = DockerClient(
-                compose_files=self._get_compose_files("dev"),
-                compose_project_directory=get_project_root(),
-            )
-
-            # build ue-dev container
-            docker_dev.compose.build()
-
-            if mode == "standalone":
-                if clean:
-                    clean_command = (
-                        """cd "${PROJECTS_HOME}/${PROJECT_NAME}" && ue4 clean && rm -rf dist"""
-                    )
-                    docker_dev.compose.run("whiskey_ue", ["bash", "-c", clean_command])
-
-                # run UE package command to compile and cook the UE project, making the `dist` directory
-                ue_project_package_command = """cd "${PROJECTS_HOME}/${PROJECT_NAME}" && source ${ROS_OVERLAY}/setup.bash && ue4 package Development"""
-                docker_dev.compose.run("whiskey_ue", ["bash", "-c", ue_project_package_command])
-                docker_standalone.compose.build()
-
-        @sim.command(name="up")
-        @click.option(
-            "--build",
-            type=bool,
-            default=False,
-            help="Should we rebuild the docker containers? Default: False",
-        )
-        @click.option(
-            "-m",
-            "--mode",
-            type=click.Choice(list(map(lambda x: x.name, Mode)), case_sensitive=False),
-            default=mode_default,
-            help=mode_help,
-        )
-        @click.argument("args", nargs=-1)
-        def up(build: bool, mode: str, args: List[str]):
-            """Starts the sim"""
-            docker = DockerClient(
-                compose_files=self._get_compose_files(mode),
-                compose_project_directory=get_project_root(),
-            )
-            docker.compose.up(detach=True, build=build)
-
-        @sim.command(name="down")
-        @click.option(
-            "-m",
-            "--mode",
-            type=click.Choice(list(map(lambda x: x.name, Mode)), case_sensitive=False),
-            default=mode_default,
-            help=mode_help,
-        )
-        @click.argument("args", nargs=-1)
-        def down(mode: str, args: List[str]):
-            """Stops the sim"""
-            docker = DockerClient(
-                compose_files=self._get_compose_files(mode),
-                compose_project_directory=get_project_root(),
-            )
-            docker.compose.down()
-
-        @sim.command(name="base-ue")
-        @click.option(
-            "--ue-version",
-            type=str,
-            default="4.27.2",
-            help="The release version of Unreal Engine to build",
-        )
-        @click.option(
-            "--memory",
-            type=str,
-            default=None,
-            help="Set maximum memory for the docker build",
-        )
-        def base_ue(ue_version: str, memory: str):
-            """Builds the base Unreal Engine image for development"""
-
-            cuda_ver = "11.8.0"
-            ubuntu_ver = "22.04"
-
-            args = ""
-            if memory is not None:
-                args += f" --memory {memory}"
-
-            # docker org has to be provided as long as we have to build our own cudagl images. requires https://github.com/adamrehn/ue4-docker/pull/276
-            call(
-                f"ue4-docker build {ue_version} --cuda={cuda_ver} -basetag=ubuntu{ubuntu_ver} -baseorg={DOCKER_ORG} -username={os.environ['GHCR_USERNAME']} -password={os.environ['API_TOKEN_GITHUB']}{args} --opt credential_mode=secrets --exclude ddc",
-                env={"UE4DOCKER_TAG_NAMESPACE": DOCKER_ORG},
-            )
+def _get_compose_files(mode: str) -> List[ValidPath]:
+    if mode == "dev":
+        return [DOCKER_SIM_DEV]
+    else:
+        return [DOCKER_SIM_STANDALONE]
+
+
+@click.group(help="Commands for the sim")
+def sim():
+    pass
+
+
+@click.command(name="build")
+@click.option(
+    "-m",
+    "--mode",
+    type=click.Choice(list(map(lambda x: x.name, Mode)), case_sensitive=False),
+    default=mode_default,
+    help=mode_help,
+)
+@click.option(
+    "-c",
+    "--clean",
+    help="Should the ue4 build assets be cleaned?",
+    type=bool,
+)
+@click.argument("args", nargs=-1)
+def build(mode: str, clean: bool, args: List[str]):
+    """Builds the sim"""
+    # If building standalone, we first build the dev sim
+    # TODO move this to a multistage build
+
+    # check UE cache dir
+    prj_root = get_project_root()
+    if not prj_root:
+        raise RuntimeError("Could not find project root")
+
+    cache_dir = Path(prj_root / ".cache")
+    Path(cache_dir).mkdir(exist_ok=True)
+
+    if not check_directory_ownership(cache_dir):
+        raise click.ClickException("'.cache' directory does not belong to current user/group.")
+
+    docker_standalone = DockerClient(
+        compose_files=_get_compose_files("standalone"),
+        compose_project_directory=get_project_root(),
+    )
+    docker_dev = DockerClient(
+        compose_files=_get_compose_files("dev"),
+        compose_project_directory=get_project_root(),
+    )
+
+    # build ue-dev container
+    docker_dev.compose.build()
+
+    if mode == "standalone":
+        if clean:
+            clean_command = """cd "${PROJECTS_HOME}/${PROJECT_NAME}" && ue4 clean && rm -rf dist"""
+            docker_dev.compose.run("whiskey_ue", ["bash", "-c", clean_command])
+
+        # run UE package command to compile and cook the UE project, making the `dist` directory
+        ue_project_package_command = """cd "${PROJECTS_HOME}/${PROJECT_NAME}" && source ${ROS_OVERLAY}/setup.bash && ue4 package Development"""
+        docker_dev.compose.run("whiskey_ue", ["bash", "-c", ue_project_package_command])
+        docker_standalone.compose.build()
+
+
+@click.command(name="up")
+@click.option(
+    "--build",
+    type=bool,
+    default=False,
+    help="Should we rebuild the docker containers? Default: False",
+)
+@click.option(
+    "-m",
+    "--mode",
+    type=click.Choice(list(map(lambda x: x.name, Mode)), case_sensitive=False),
+    default=mode_default,
+    help=mode_help,
+)
+@click.argument("args", nargs=-1)
+def up(build: bool, mode: str, args: List[str]):
+    """Starts the sim"""
+    docker = DockerClient(
+        compose_files=_get_compose_files(mode),
+        compose_project_directory=get_project_root(),
+    )
+    docker.compose.up(detach=True, build=build)
+
+
+@click.command(name="down")
+@click.option(
+    "-m",
+    "--mode",
+    type=click.Choice(list(map(lambda x: x.name, Mode)), case_sensitive=False),
+    default=mode_default,
+    help=mode_help,
+)
+@click.argument("args", nargs=-1)
+def down(mode: str, args: List[str]):
+    """Stops the sim"""
+    docker = DockerClient(
+        compose_files=_get_compose_files(mode),
+        compose_project_directory=get_project_root(),
+    )
+    docker.compose.down()
+
+
+@click.command(name="base-ue")
+@click.option(
+    "--ue-version",
+    type=str,
+    default="4.27.2",
+    help="The release version of Unreal Engine to build",
+)
+@click.option(
+    "--memory",
+    type=str,
+    default=None,
+    help="Set maximum memory for the docker build",
+)
+def base_ue(ue_version: str, memory: str):
+    """Builds the base Unreal Engine image for development"""
+
+    cuda_ver = "11.8.0"
+    ubuntu_ver = "22.04"
+
+    args = ""
+    if memory is not None:
+        args += f" --memory {memory}"
+
+    # docker org has to be provided as long as we have to build our own cudagl images. requires https://github.com/adamrehn/ue4-docker/pull/276
+    call(
+        f"ue4-docker build {ue_version} --cuda={cuda_ver} -basetag=ubuntu{ubuntu_ver} -baseorg={DOCKER_ORG} -username={os.environ['GHCR_USERNAME']} -password={os.environ['API_TOKEN_GITHUB']}{args} --opt credential_mode=secrets --exclude ddc",
+        env={"UE4DOCKER_TAG_NAMESPACE": DOCKER_ORG},
+    )
```

### Comparing `gama_cli-1.7.4/gama_cli/groups/vessel.py` & `gama_cli-1.8.0/gama_cli/groups/vessel.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,355 +48,375 @@
     "gama_greenstream",
     "gama_docs",
     "lookout",
     "groot",
 ]
 
 
-class Vessel:
-    def _get_compose_files(
-        self,
-        network: Network = Network.SHARED,
-        gpu: bool = False,
-        variant: Variant = Variant.WHISKEY_BRAVO,
-        prod: bool = False,
-    ) -> List[ValidPath]:
-        compose_files: List[ValidPath] = [DOCKER_VESSEL]
-
-        if not prod:
-            compose_files.append(DOCKER_VESSEL_DEV)
-        if variant == variant.EDUCAT:
-            compose_files.append(DOCKER_VESSEL_VARIANT_EDUCAT)
-        if variant == variant.WHISKEY_BRAVO:
-            compose_files.append(DOCKER_VESSEL_VARIANT_BRAVO)
-        if gpu:
-            compose_files.append(DOCKER_VESSEL_GPU)
-        if network == Network.SHARED:
-            compose_files.append(DOCKER_VESSEL_NETWORK_SHARED)
-        if network == Network.VPN:
-            compose_files.append(DOCKER_VESSEL_NETWORK_VPN)
-        if network == Network.HOST:
-            compose_files.append(DOCKER_VESSEL_NETWORK_HOST)
-        if prod:
-            compose_files.append(DOCKER_VESSEL_PROD)
-
-        return compose_files
-
-    def _get_greenstream_config(self, variant: Variant, mode: Mode):
-        if mode == Mode.STUBS:
-            return "config.stubs.yml"
-        if mode == Mode.SIMULATOR:
-            print("SIM VIDEO STREAMING NO LONGER SUPPORTED")
-            return "config.sim.yml"
-        if mode == Mode.HARDWARE:
-            if variant == Variant.WHISKEY_BRAVO:
-                return "config.variant.bravo.yml"
-            if variant == Variant.EDUCAT:
-                return "config.variant.educat.yml"
-        raise Exception("Invalid mode/variant combination")
-
-    def __init__(self, cli: click.Group, dev_mode: bool = False):
-        @cli.group(help="Commands for the vessel")
-        def vessel():
-            pass
-
-        if dev_mode:
-
-            @vessel.command(name="build")
-            @click.argument(
-                "service",
-                required=False,
-                type=click.Choice(SERVICES),
-            )
-            @click.argument("args", nargs=-1)
-            def build(service: str, args: List[str]):  # type: ignore
-                """Build the vessel"""
-                config = read_gama_vessel_config()
-
-                docker = DockerClient(
-                    compose_files=self._get_compose_files(),
-                    compose_project_directory=get_project_root(),
-                )
-
-                os.environ["GAMA_VARIANT"] = config.variant.value
-
-                if service:
-                    docker.compose.build([service])
-                    return
-
-                docker.compose.build(
-                    ["gama_ui", "gama_chart_tiler", "gama_chart_api", "gama_vessel"]
-                )
-
-                if config.extensions.lookout:
-                    docker.compose.build(["lookout"])
-
-                if config.extensions.groot:
-                    docker.compose.build(["groot"])
-
-            @vessel.command(name="bake")
-            @click.option(
-                "--variant",
-                type=click.Choice(Variant),  # type: ignore
-                required=True,
-                help="The variant to bake",
-            )
-            @click.option(
-                "--version",
-                type=str,
-                required=True,
-                help="The version to bake. Default: latest",
-            )
-            @click.option(
-                "--push",
-                type=bool,
-                default=False,
-                is_flag=True,
-                help="Should we push the images to the registry? Default: False",
-            )
-            @click.argument("services", nargs=-1)
-            def bake(variant: Variant, version: str, push: bool, services: List[str]):  # type: ignore
-                """Bakes the vessel docker containers"""
-                compose_files = self._get_compose_files(variant=variant)
-                docker_bake(
-                    version=version,
-                    services=services,
-                    push=push,
-                    compose_files=compose_files,
-                )
-
-            @vessel.command(name="test-ui")
-            def test_ui():  # type: ignore
-                """Runs test for the ui"""
-                docker = DockerClient(
-                    compose_files=self._get_compose_files(),
-                    compose_project_directory=get_project_root(),
-                )
-                docker.compose.run("gama_ui", ["yarn", "test"])
-
-            @vessel.command(name="test-ros")
-            def test_ros():  # type: ignore
-                """Runs test for the ros nodes"""
-                docker = DockerClient(
-                    compose_files=self._get_compose_files(),
-                    compose_project_directory=get_project_root(),
-                )
-                docker.compose.run(
-                    "gama_vessel",
-                    ["/bin/bash", "-c", "source /home/ros/.profile && platform ros test"],
-                )
-
-            @vessel.command(name="test-e2e")
-            def test_e2e():  # type: ignore
-                """Runs UI e2e tests (assuming all the containers are up)"""
-                call("cd ./projects/gama_ui && yarn test:e2e")
-
-            @vessel.command(name="test")
-            def test():  # type: ignore
-                """Runs test for the all vessel code"""
-                call("gama_cli vessel test-ui")
-                call("gama_cli vessel test-ros")
-
-            @vessel.command(name="lint-ui")
-            @click.argument("args", nargs=-1)
-            def lint_ui(args: List[str]):  # type: ignore
-                """Runs lints for the ui"""
-                docker = DockerClient(
-                    compose_files=self._get_compose_files(),
-                    compose_project_directory=get_project_root(),
-                )
-                docker.compose.run("gama_ui", ["yarn", "lint", *args])
-
-            @vessel.command(name="type-generate")
-            def type_generate():  # type: ignore
-                """Generates typescript types for all ros messages"""
-                docker = DockerClient(
-                    compose_files=self._get_compose_files(),
-                    compose_project_directory=get_project_root(),
-                )
-                docker.compose.run("gama_vessel", ["npx", "ros-typescript-generator"])
-
-        @vessel.command(name="up")
-        @click.option(
-            "--build",
-            type=bool,
-            default=False,
-            is_flag=True,
-            help="Should we rebuild the docker containers? Default: False",
-        )
-        @click.argument(
-            "service",
-            required=False,
-            type=click.Choice(SERVICES),
+def _get_compose_files(
+    network: Network = Network.SHARED,
+    gpu: bool = False,
+    variant: Variant = Variant.WHISKEY_BRAVO,
+    prod: bool = False,
+) -> List[ValidPath]:
+    compose_files: List[ValidPath] = [DOCKER_VESSEL]
+
+    if not prod:
+        compose_files.append(DOCKER_VESSEL_DEV)
+    if variant == variant.EDUCAT:
+        compose_files.append(DOCKER_VESSEL_VARIANT_EDUCAT)
+    if variant == variant.WHISKEY_BRAVO:
+        compose_files.append(DOCKER_VESSEL_VARIANT_BRAVO)
+    if gpu:
+        compose_files.append(DOCKER_VESSEL_GPU)
+    if network == Network.SHARED:
+        compose_files.append(DOCKER_VESSEL_NETWORK_SHARED)
+    if network == Network.VPN:
+        compose_files.append(DOCKER_VESSEL_NETWORK_VPN)
+    if network == Network.HOST:
+        compose_files.append(DOCKER_VESSEL_NETWORK_HOST)
+    if prod:
+        compose_files.append(DOCKER_VESSEL_PROD)
+
+    return compose_files
+
+
+def _get_greenstream_config(variant: Variant, mode: Mode):
+    if mode == Mode.STUBS:
+        return "config.stubs.yml"
+    if mode == Mode.SIMULATOR:
+        print("SIM VIDEO STREAMING NO LONGER SUPPORTED")
+        return "config.sim.yml"
+    if mode == Mode.HARDWARE:
+        if variant == Variant.WHISKEY_BRAVO:
+            return "config.variant.bravo.yml"
+        if variant == Variant.EDUCAT:
+            return "config.variant.educat.yml"
+    raise Exception("Invalid mode/variant combination")
+
+
+@click.group(help="Commands for the vessel")
+def vessel():
+    pass
+
+
+@click.command(name="build")
+@click.argument(
+    "service",
+    required=False,
+    type=click.Choice(SERVICES),
+)
+@click.argument("args", nargs=-1)
+def build(service: str, args: List[str]):  # type: ignore
+    """Build the vessel"""
+    config = read_gama_vessel_config()
+
+    docker = DockerClient(
+        compose_files=_get_compose_files(),
+        compose_project_directory=get_project_root(),
+    )
+
+    os.environ["GAMA_VARIANT"] = config.variant.value
+
+    if service:
+        docker.compose.build([service])
+        return
+
+    docker.compose.build(["gama_ui", "gama_chart_tiler", "gama_chart_api", "gama_vessel"])
+
+    if config.extensions.lookout:
+        docker.compose.build(["lookout"])
+
+    if config.extensions.groot:
+        docker.compose.build(["groot"])
+
+
+@click.command(name="bake")
+@click.option(
+    "--variant",
+    type=click.Choice(Variant),  # type: ignore
+    required=True,
+    help="The variant to bake",
+)
+@click.option(
+    "--version",
+    type=str,
+    required=True,
+    help="The version to bake. Default: latest",
+)
+@click.option(
+    "--push",
+    type=bool,
+    default=False,
+    is_flag=True,
+    help="Should we push the images to the registry? Default: False",
+)
+@click.argument("services", nargs=-1)
+def bake(variant: Variant, version: str, push: bool, services: List[str]):  # type: ignore
+    """Bakes the vessel docker containers"""
+    compose_files = _get_compose_files(variant=variant)
+    docker_bake(
+        version=version,
+        services=services,
+        push=push,
+        compose_files=compose_files,
+    )
+
+
+@click.command(name="test-ui")
+def test_ui():  # type: ignore
+    """Runs test for the ui"""
+    docker = DockerClient(
+        compose_files=_get_compose_files(),
+        compose_project_directory=get_project_root(),
+    )
+    docker.compose.run("gama_ui", ["yarn", "test"])
+
+
+@click.command(name="test-ros")
+def test_ros():  # type: ignore
+    """Runs test for the ros nodes"""
+    docker = DockerClient(
+        compose_files=_get_compose_files(),
+        compose_project_directory=get_project_root(),
+    )
+    docker.compose.run(
+        "gama_vessel",
+        ["/bin/bash", "-c", "source /home/ros/.profile && platform ros test"],
+    )
+
+
+@click.command(name="test-e2e")
+def test_e2e():  # type: ignore
+    """Runs UI e2e tests (assuming all the containers are up)"""
+    call("cd ./projects/gama_ui && yarn test:e2e")
+
+
+@click.command(name="test")
+def test():  # type: ignore
+    """Runs test for the all vessel code"""
+    call("gama_cli vessel test-ui")
+    call("gama_cli vessel test-ros")
+
+
+@click.command(name="lint-ui")
+@click.argument("args", nargs=-1)
+def lint_ui(args: List[str]):  # type: ignore
+    """Runs lints for the ui"""
+    docker = DockerClient(
+        compose_files=_get_compose_files(),
+        compose_project_directory=get_project_root(),
+    )
+    docker.compose.run("gama_ui", ["yarn", "lint", *args])
+
+
+@click.command(name="type-generate")
+def type_generate():  # type: ignore
+    """Generates typescript types for all ros messages"""
+    docker = DockerClient(
+        compose_files=_get_compose_files(),
+        compose_project_directory=get_project_root(),
+    )
+    docker.compose.run("gama_vessel", ["npx", "ros-typescript-generator"])
+
+
+@click.command(name="up")
+@click.option(
+    "--build",
+    type=bool,
+    default=False,
+    is_flag=True,
+    help="Should we rebuild the docker containers? Default: False",
+)
+@click.argument(
+    "service",
+    required=False,
+    type=click.Choice(SERVICES),
+)
+@click.argument("args", nargs=-1)
+def up(
+    build: bool,
+    service: str,
+    args: List[str],
+):
+    """Starts the vessel"""
+    dev_mode = os.environ["GAMA_CLI_DEV_MODE"] == "true"
+
+    config = read_gama_vessel_config()
+    build = maybe_ignore_build(dev_mode, build)
+    prod = maybe_ignore_prod(dev_mode, config.prod)
+
+    docker = DockerClient(
+        compose_files=_get_compose_files(
+            gpu=config.extensions.lookout,
+            network=config.network,
+            variant=config.variant,
+            prod=prod,
+        ),
+        compose_project_directory=get_project_root(),
+    )
+
+    vessel_launch_command_args = f"mode:='{config.mode.value}' rviz:='{config.extensions.rviz}'"
+    if config.ubiquity_user:
+        vessel_launch_command_args += f" ubiquity_user:='{config.ubiquity_user}'"
+    if config.ubiquity_pass:
+        vessel_launch_command_args += f" ubiquity_pass:='{config.ubiquity_pass}'"
+    if config.ubiquity_ip:
+        vessel_launch_command_args += f" ubiquity_ip:='{config.ubiquity_ip}'"
+    if config.log_level:
+        vessel_launch_command_args += f" log_level:='{config.log_level.value}'"
+
+    # TODO - use config.__dataclass_fields__ and iterate through the Dict[str, Field]
+    fields = [
+        "ddsrouter_remote_ip",
+        "ddsrouter_remote_port",
+        "ddsrouter_listen_ip",
+        "ddsrouter_listen_port",
+    ]
+    for field in fields:
+        if getattr(config, field):
+            vessel_launch_command_args += f" {field}:='{getattr(config, field)}'"
+
+    os.environ["GAMA_VERSION"] = get_gama_version()
+    os.environ["GAMA_VARIANT"] = config.variant.value
+    os.environ["GAMA_VESSEL_COMMAND_ARGS"] = vessel_launch_command_args
+    os.environ["LOOKOUT_COMMAND_ARGS"] = f"mode:='{config.mode.value}'"
+    os.environ["GREENSTREAM_CONFIG_FILE"] = _get_greenstream_config(config.variant, config.mode)
+
+    services = (
+        [service]
+        if service
+        else [
+            "gama_ui",
+            "gama_chart_tiler",
+            "gama_chart_api",
+            "gama_vessel",
+            "gama_greenstream",
+            "gama_docs",
+        ]
+    )
+
+    docker.compose.up(
+        services,
+        detach=True,
+        build=build,
+    )
+
+    if config.extensions.lookout:
+        docker.compose.up(
+            ["lookout"],
+            detach=True,
+            build=build,
         )
-        @click.argument("args", nargs=-1)
-        def up(
-            build: bool,
-            service: str,
-            args: List[str],
-        ):
-            """Starts the vessel"""
-
-            config = read_gama_vessel_config()
-            build = maybe_ignore_build(dev_mode, build)
-            prod = maybe_ignore_prod(dev_mode, config.prod)
-
-            docker = DockerClient(
-                compose_files=self._get_compose_files(
-                    gpu=config.extensions.lookout,
-                    network=config.network,
-                    variant=config.variant,
-                    prod=prod,
-                ),
-                compose_project_directory=get_project_root(),
-            )
 
-            vessel_launch_command_args = (
-                f"mode:='{config.mode.value}' rviz:='{config.extensions.rviz}'"
-            )
-            if config.ubiquity_user:
-                vessel_launch_command_args += f" ubiquity_user:={config.ubiquity_user}"
-            if config.ubiquity_pass:
-                vessel_launch_command_args += f" ubiquity_pass:='{config.ubiquity_pass}'"
-            if config.ubiquity_ip:
-                vessel_launch_command_args += f" ubiquity_ip:='{config.ubiquity_ip}'"
-            if config.log_level:
-                vessel_launch_command_args += f" log_level:='{config.log_level.value}'"
-
-            os.environ["GAMA_VERSION"] = get_gama_version()
-            os.environ["GAMA_VARIANT"] = config.variant.value
-            os.environ["GAMA_VESSEL_COMMAND_ARGS"] = vessel_launch_command_args
-            os.environ["LOOKOUT_COMMAND_ARGS"] = f"mode:='{config.mode.value}'"
-            os.environ["GREENSTREAM_CONFIG_FILE"] = self._get_greenstream_config(
-                config.variant, config.mode
-            )
+    if config.extensions.groot:
+        docker.compose.up(["groot"], detach=True, build=build)
 
-            services = (
-                [service]
-                if service
-                else [
-                    "gama_ui",
-                    "gama_chart_tiler",
-                    "gama_chart_api",
-                    "gama_vessel",
-                    "gama_greenstream",
-                    "gama_docs",
-                ]
-            )
 
-            docker.compose.up(
-                services,
-                detach=True,
-                build=build,
+@click.command(name="down")
+@click.argument("args", nargs=-1)
+def down(args: List[str]):  # type: ignore
+    """Stops the vessel"""
+    docker = DockerClient(
+        compose_files=_get_compose_files(),
+        compose_project_directory=get_project_root(),
+    )
+    docker.compose.down()
+
+
+@click.command(name="install")
+@click.option(
+    "--variant",
+    type=click.Choice(Variant),  # type: ignore
+    help="Which variant of GAMA to install?",
+)
+def install(variant: Variant):  # type: ignore
+    """Install GAMA on a vessel"""
+    config = read_gama_vessel_config()
+    variant = variant or config.variant
+    docker = DockerClient(
+        compose_files=_get_compose_files(variant=variant),
+        compose_project_directory=get_project_root(),
+    )
+    try:
+        docker.compose.pull(
+            [
+                "gama_ui",
+                "gama_chart_tiler",
+                "gama_chart_api",
+                "gama_vessel",
+                "gama_greenstream",
+                "gama_docs",
+            ]
+        )
+    except Exception:
+        click.echo(
+            click.style(
+                "Failed to pull GAMA files. Have you ran `gama_cli authenticate` ?",
+                fg="yellow",
             )
+        )
 
-            if config.extensions.lookout:
-                docker.compose.up(
-                    ["lookout"],
-                    detach=True,
-                    build=build,
-                )
-
-            if config.extensions.groot:
-                docker.compose.up(["groot"], detach=True, build=build)
-
-        @vessel.command(name="down")
-        @click.argument("args", nargs=-1)
-        def down(args: List[str]):  # type: ignore
-            """Stops the vessel"""
-            docker = DockerClient(
-                compose_files=self._get_compose_files(),
-                compose_project_directory=get_project_root(),
-            )
-            docker.compose.down()
 
-        @vessel.command(name="install")
-        @click.option(
-            "--variant",
-            type=click.Choice(Variant),  # type: ignore
-            help="Which variant of GAMA to install?",
-        )
-        def install(variant: Variant):  # type: ignore
-            """Install GAMA on a vessel"""
-            config = read_gama_vessel_config()
-            variant = variant or config.variant
-            docker = DockerClient(
-                compose_files=self._get_compose_files(variant=variant),
-                compose_project_directory=get_project_root(),
+@click.command(name="configure")
+def configure():  # type: ignore
+    """Configure GAMA Vessel"""
+
+    # Check if the file exists
+    if os.path.exists(GAMA_VESSEL_CONFIG_PATH):
+        click.echo(
+            click.style(
+                f"GAMA Vessel config already exists: {GAMA_VESSEL_CONFIG_PATH}",
+                fg="yellow",
             )
-            try:
-                docker.compose.pull(
-                    [
-                        "gama_ui",
-                        "gama_chart_tiler",
-                        "gama_chart_api",
-                        "gama_vessel",
-                        "gama_greenstream",
-                        "gama_docs",
-                    ]
-                )
-            except Exception:
-                click.echo(
-                    click.style(
-                        "Failed to pull GAMA files. Have you ran `gama_cli authenticate` ?",
-                        fg="yellow",
-                    )
-                )
-
-        @vessel.command(name="configure")
-        def configure():  # type: ignore
-            """Configure GAMA Vessel"""
-
-            # Check if the file exists
-            if os.path.exists(GAMA_VESSEL_CONFIG_PATH):
-                click.echo(
-                    click.style(
-                        f"GAMA Vessel config already exists: {GAMA_VESSEL_CONFIG_PATH}",
-                        fg="yellow",
-                    )
-                )
-                result = click.prompt(
-                    "Do you want to overwrite it?", default="y", type=click.Choice(["y", "n"])
-                )
-                if result == "n":
-                    return
-
-            config = GamaVesselConfig(
-                variant=click.prompt(
-                    "Variant",
-                    default=Variant.WHISKEY_BRAVO,
-                    type=click.Choice([item.value for item in Variant]),
-                ),
-                ubiquity_user=click.prompt("Ubiquity username", default=""),
-                ubiquity_pass=click.prompt("Ubiquity password", default=""),
-                ubiquity_ip=click.prompt("Ubiquity ip", default=""),
-                mode=click.prompt(
-                    "Mode", default=Mode.HARDWARE, type=click.Choice([item.value for item in Mode])
-                ),
-                prod=click.prompt("Prod", default=True, type=bool),
-                log_level=click.prompt(
-                    "Log level",
-                    default=LogLevel.INFO,
-                    type=click.Choice([item.value for item in LogLevel]),
-                ),
-            )
-            write_gama_vessel_config(config)
+        )
+        result = click.prompt(
+            "Do you want to overwrite it?", default="y", type=click.Choice(["y", "n"])
+        )
+        if result == "n":
+            return
 
-            # Now that the GAMA config has been written. Let's write the greenstream config...
-            # Check if it exists
-            if os.path.exists(GREENSTREAM_CONFIG_DEST_PATH):
-                click.echo(
-                    click.style(
-                        f"Greenstream config already exists: {GREENSTREAM_CONFIG_DEST_PATH}",
-                        fg="yellow",
-                    )
-                )
-                result = click.prompt(
-                    "Do you want to overwrite it?", default="y", type=click.Choice(["y", "n"])
-                )
-                if result == "n":
-                    return
-
-            # Copy the directory from the assets. If it exists, it will be overwritten
-            shutil.copytree(
-                GREENSTREAM_CONFIG_SOURCE_PATH, GREENSTREAM_CONFIG_DEST_PATH, dirs_exist_ok=True
+    config = GamaVesselConfig(
+        variant=click.prompt(
+            "Variant",
+            default=Variant.WHISKEY_BRAVO,
+            type=click.Choice([item.value for item in Variant]),
+        ),
+        ubiquity_user=click.prompt("Ubiquity username", default=""),
+        ubiquity_pass=click.prompt("Ubiquity password", default=""),
+        ubiquity_ip=click.prompt("Ubiquity ip", default=""),
+        mode=click.prompt(
+            "Mode", default=Mode.HARDWARE, type=click.Choice([item.value for item in Mode])
+        ),
+        prod=click.prompt("Prod", default=True, type=bool),
+        network=click.prompt(
+            "Network",
+            default=Network.HOST,
+            type=click.Choice([item.value for item in Network]),
+        ),
+        log_level=click.prompt(
+            "Log level",
+            default=LogLevel.INFO,
+            type=click.Choice([item.value for item in LogLevel]),
+        ),
+    )
+    write_gama_vessel_config(config)
+
+    # Now that the GAMA config has been written. Let's write the greenstream config...
+    # Check if it exists
+    if os.path.exists(GREENSTREAM_CONFIG_DEST_PATH):
+        click.echo(
+            click.style(
+                f"Greenstream config already exists: {GREENSTREAM_CONFIG_DEST_PATH}",
+                fg="yellow",
             )
+        )
+        result = click.prompt(
+            "Do you want to overwrite it?", default="y", type=click.Choice(["y", "n"])
+        )
+        if result == "n":
+            return
+
+    # Copy the directory from the assets. If it exists, it will be overwritten
+    shutil.copytree(
+        GREENSTREAM_CONFIG_SOURCE_PATH, GREENSTREAM_CONFIG_DEST_PATH, dirs_exist_ok=True
+    )
```

### Comparing `gama_cli-1.7.4/gama_cli/helpers.py` & `gama_cli-1.8.0/gama_cli/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,20 @@
     version = pkg_resources.require("gama-cli")[0].version
     if version == "0.0.0":
         version = "latest"
     return version
 
 
 def is_dev_version():
-    return (
-        pkg_resources.require("gama_cli")[0].version == "0.0.0"
-        or os.environ.get("GAMA_CLI_DEV_MODE") == "true"
-    )
+    if os.environ.get("GAMA_CLI_DEV_MODE") == "false":
+        return False
+
+    if os.environ.get("GAMA_CLI_DEV_MODE") == "true":
+        return True
+    return pkg_resources.require("gama_cli")[0].version == "0.0.0"
 
 
 def docker_compose_path(path: str) -> Path:
     current_file_dir = Path(__file__).parent
     return current_file_dir / "docker" / path
```

### Comparing `gama_cli-1.7.4/gama_cli.egg-info/PKG-INFO` & `gama_cli-1.8.0/gama_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama-cli
-Version: 1.7.4
+Version: 1.8.0
 Summary: A CLI for interacting with the GAMA platform
 Home-page: https://github.com/Greenroom-Robotics/gama_cli
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `gama_cli-1.7.4/gama_cli.egg-info/SOURCES.txt` & `gama_cli-1.8.0/gama_cli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -40,8 +40,10 @@
 gama_cli/groups/attach.py
 gama_cli/groups/docker.py
 gama_cli/groups/git.py
 gama_cli/groups/gs.py
 gama_cli/groups/misc.py
 gama_cli/groups/setup.py
 gama_cli/groups/sim.py
-gama_cli/groups/vessel.py
+gama_cli/groups/vessel.py
+gama_cli/schemas/gama_gs.schema.json
+gama_cli/schemas/gama_vessel.schema.json
```

### Comparing `gama_cli-1.7.4/setup.cfg` & `gama_cli-1.8.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gama_cli
-version = 1.7.4
+version = 1.8.0
 url = https://github.com/Greenroom-Robotics/gama_cli
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
@@ -25,18 +25,20 @@
 	toml~=0.10
 	setuptools
 	colorama
 	click
 	python-on-whales
 	dacite
 	PyYAML
+	dc-schema
 zip_safe = true
 
 [options.package_data]
 gama_cli = 
+	**/*.json
 	**/*.py
 	**/**/*.yaml
 	**/**/*.yml
 
 [options.entry_points]
 console_scripts = 
 	gama_cli = gama_cli.cli:cli
```

