# Comparing `tmp/unigbsa-0.1.3.tar.gz` & `tmp/unigbsa-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unigbsa-0.1.3.tar", last modified: Fri Apr  7 07:27:48 2023, max compression
+gzip compressed data, was "unigbsa-0.1.4.tar", last modified: Fri Apr 14 15:52:50 2023, max compression
```

## Comparing `unigbsa-0.1.3.tar` & `unigbsa-0.1.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:48.647512 unigbsa-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-07 07:27:39.000000 unigbsa-0.1.3/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 07:27:39.000000 unigbsa-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-07 07:27:48.647512 unigbsa-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-07 07:27:39.000000 unigbsa-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:48.643512 unigbsa-0.1.3/launching/
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-04-07 07:27:39.000000 unigbsa-0.1.3/launching/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-07 07:27:39.000000 unigbsa-0.1.3/launching/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-07 07:27:39.000000 unigbsa-0.1.3/launching/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 07:27:48.647512 unigbsa-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-07 07:27:39.000000 unigbsa-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:48.643512 unigbsa-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-07 07:27:39.000000 unigbsa-0.1.3/tests/test_pipline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:48.643512 unigbsa-0.1.3/unigbsa/
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/CLI.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:48.643512 unigbsa-0.1.3/unigbsa/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:48.643512 unigbsa-0.1.3/unigbsa/data/Calibri/
--rw-r--r--   0 runner    (1001) docker     (123)   327124 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/data/Calibri/Calibri.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   327124 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/data/Calibri/calibribold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/data/default.ini
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/data/default.json
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/data/mmpbsa.in
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/data/scan.json
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/data/template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:48.647512 unigbsa-0.1.3/unigbsa/gbsa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/gbsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/gbsa/gbsarun.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/gbsa/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/gbsa/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/gbsa/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/gbsa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:48.647512 unigbsa-0.1.3/unigbsa/scanparas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/scanparas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18546 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/scanparas/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:48.647512 unigbsa-0.1.3/unigbsa/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:48.647512 unigbsa-0.1.3/unigbsa/simulation/mdp/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdp/ions.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdp/md.mdp
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdp/mdout.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdp/minim.mdp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:48.647512 unigbsa-0.1.3/unigbsa/simulation/mdp/minimization/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdp/minimization/s1-cg.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdp/minimization/s1-steep.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdp/minimization/s2-cg.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdp/minimization/s2-steep.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdp/minimization/s3-steep.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdp/minimization/s4-cg.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdp/npt.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdp/nvt.mdp
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdp/vaccum.mdp
--rw-r--r--   0 runner    (1001) docker     (123)    20758 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/mdrun.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/openmm-em.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/topology.py
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/simulation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-07 07:27:39.000000 unigbsa-0.1.3/unigbsa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 07:27:48.643512 unigbsa-0.1.3/unigbsa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-07 07:27:48.000000 unigbsa-0.1.3/unigbsa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-07 07:27:48.000000 unigbsa-0.1.3/unigbsa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 07:27:48.000000 unigbsa-0.1.3/unigbsa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-07 07:27:48.000000 unigbsa-0.1.3/unigbsa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 07:27:48.000000 unigbsa-0.1.3/unigbsa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-07 07:27:48.000000 unigbsa-0.1.3/unigbsa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 07:27:48.000000 unigbsa-0.1.3/unigbsa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.982078 unigbsa-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 15:52:36.000000 unigbsa-0.1.4/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 15:52:36.000000 unigbsa-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-14 15:52:50.982078 unigbsa-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-14 15:52:36.000000 unigbsa-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.962078 unigbsa-0.1.4/launching/
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-04-14 15:52:36.000000 unigbsa-0.1.4/launching/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-14 15:52:36.000000 unigbsa-0.1.4/launching/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-14 15:52:36.000000 unigbsa-0.1.4/launching/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:52:50.982078 unigbsa-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-14 15:52:36.000000 unigbsa-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.962078 unigbsa-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-14 15:52:36.000000 unigbsa-0.1.4/tests/test_pipline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.962078 unigbsa-0.1.4/unigbsa/
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/CLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.970078 unigbsa-0.1.4/unigbsa/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.970078 unigbsa-0.1.4/unigbsa/data/Calibri/
+-rw-r--r--   0 runner    (1001) docker     (123)   327124 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/Calibri/Calibri.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   327124 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/Calibri/calibribold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/default.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/default.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/mmpbsa.in
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/scan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/data/template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.974078 unigbsa-0.1.4/unigbsa/gbsa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/gbsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/gbsa/gbsarun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/gbsa/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/gbsa/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/gbsa/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/gbsa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.974078 unigbsa-0.1.4/unigbsa/scanparas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/scanparas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18641 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/scanparas/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.978078 unigbsa-0.1.4/unigbsa/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.978078 unigbsa-0.1.4/unigbsa/simulation/mdp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/ions.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/md.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/mdout.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minim.mdp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.982078 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s1-cg.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s1-steep.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s2-cg.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s2-steep.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s3-steep.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s4-cg.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/npt.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/nvt.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdp/vaccum.mdp
+-rw-r--r--   0 runner    (1001) docker     (123)    20758 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/mdrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/openmm-em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/simulation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 15:52:36.000000 unigbsa-0.1.4/unigbsa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:52:50.966078 unigbsa-0.1.4/unigbsa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 15:52:50.000000 unigbsa-0.1.4/unigbsa.egg-info/top_level.txt
```

### Comparing `unigbsa-0.1.3/LICENCE.txt` & `unigbsa-0.1.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/PKG-INFO` & `unigbsa-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigbsa
-Version: 0.1.3
+Version: 0.1.4
 Summary: MMPB(GB)SA tools for calculate energy.
 Home-page: https://github.com/dptech-corp/Uni-GBSA
 Author: dptech.net
 Author-email: hermite@dptech.net
 Keywords: MMPBSA MMGBSA
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `unigbsa-0.1.3/README.md` & `unigbsa-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/launching/app.py` & `unigbsa-0.1.4/launching/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,23 +57,53 @@
     gb5 = 'GB-OBC2'
     gb7 = 'GB-Neck'
     gb8 = 'GB-Neck2'
     pb1 = 'PB-1'
     pb2 = 'PB-2'
 
 
+expfiledes = """
+Input experiment file.  
+    example:
+[ligands.csv](https://labs.dp.tech/download/artifacts/applications/uni-gbsa/artifacts/ligands.csv)
+"""
+protfiledes = """
+Input protein file with pdb format.  
+    example:
+[protein.pdb](https://labs.dp.tech/download/artifacts/applications/uni-gbsa/artifacts/protein.pdb)
+"""
+ligfiledes ="""
+Ligand files to perform the calculation.  
+    example:
+[1a.sdf](https://labs.dp.tech/download/artifacts/applications/uni-gbsa/artifacts/1a.sdf)
+"""
+ligfiledes2 = """
+Ligand files to perform the calculation.  
+    example:
+[ligands.zip](https://labs.dp.tech/download/artifacts/applications/uni-gbsa/artifacts/ligands.zip)
+"""
+
+
 class SCANUploadFilesModel(BaseModel):
     experiment_info: InputFilePath = \
-        Field(ftypes=['csv'], description='Input experiment file.')
-    input_protein: InputFilePath = \
+        Field(ftypes=['csv'],
+              description=expfiledes,
+              description_type="markdown",
+              max_file_size='2MB')
+    input_protein: List[InputFilePath] = \
         Field(ftypes=['pdb'],
-              description="Input protein file with pdb format.")
+              description=protfiledes,
+              description_type="markdown",
+              max_file_size='2MB')
     input_ligands: List[InputFilePath] = \
         Field(ftypes=['sdf'],
-              description='Ligand files to perform the calculation.')
+              description=ligfiledes2,
+              description_type="markdown",
+              max_file_size='1MB',
+              max_file_count=100)
 
 
 class SCANArgs(BaseModel):
     modes: Set[AlgorithmMode] = Field(default=AlgorithmMode.gb2, render_type="radio",
                                       description="MM PB/GBSA calculation mode.")
     indi: str = Field(default="1.0, 2.0, 2.5, 3.0, 3.5, 4.0",
                       description='Internal dielectric constant')
@@ -109,23 +139,29 @@
                 BaseModel):
     pass
 
 
 class GBSAUploadFilesModel(BaseModel):
     input_protein: InputFilePath = \
         Field(ftypes=['pdb'],
-              description="Input protein file with pdb format.")
+              description=protfiledes,
+              description_type="markdown",
+              max_file_size='2MB')
+
     input_ligands: List[InputFilePath] = \
         Field(ftypes=['sdf'],
-              description='Ligand files to perform the calculation.')
+              description=ligfiledes,
+              description_type="markdown",
+              max_file_count=100,
+              max_file_size='1MB')
 
 
 class AlgorithmOptions(BaseModel):
     protein_forcefield = Field(default=AlgorithmProteinForcefield.amber03,
-                               description='Protein forcefiled.')
+                               description='Protein forcefield.')
     ligand_forcefield = Field(default=AlgorithmLigandForcefield.gaff,
                               description='Ligand forcefield.')
     ligand_charge = Field(default=AlgorithmLigandCharge.bcc,
                           description='Ligand charge method.')
     mode = Field(default=AlgorithmMode.gb2,
                  description="MM PB/GBSA calculation mode.")
     indi: Float = Field(default=4.0,
@@ -199,19 +235,22 @@
         ]
 
         for line in cmd(*args, _iter=True):
             print(line)
         with open(csvoutfile) as fr:
             lines = fr.readlines()
         with open(csvoutfile, 'w') as fw:
-            for line in lines:
+            for i, line in enumerate(lines):
                 llist = line.strip().split(',')
-                newlist = [llist[0]]
-                for li in llist[2:-1]:
-                    newlist.append(str(round(float(li), 4)))
+                if i == 0:
+                    newlist = [llist[0]] + llist[2:-1]
+                else:
+                    newlist = [llist[0], llist[2]]
+                    for li in llist[3:-1]:
+                        newlist.append(str(round(float(li), 4)))
                 newline = ','.join(newlist) + '\n'
                 fw.write(newline)
         table_section = ReportSection(
                 title='GBSA output',
                 elements=[
                     AutoReportElement(title="",
                                       path='GBSA-output.csv',
@@ -254,22 +293,22 @@
                 "indi": [float(indi) for indi in opts.indi.split(',')],
                 "exdi": opts.endi,
                 "nonpolarsurfConst": "0.0",
                 "surften": "0.0072"
             }
         }
 
-        input_protein = opts.input_protein.get_path()
+        input_protein = os.path.abspath(opts.input_protein[0].get_path())
         input_dir = os.path.dirname(input_protein)
         configfile = Path(os.path.join(input_dir, 'config.json'))
         with open(configfile,  'w') as fw:
             json.dump(default, fw, indent='  ')
         cmd = sh.Command('unigbsa-scan')
         args = [
-            '-i', input_protein,
+            '-pd', input_dir,
             '-l', opts.input_ligands,
             '-e', opts.experiment_info.get_path(),
             '-c', configfile,
             '-o', opts.output_dir,
         ]
         for line in cmd(*args, _iter=True):
             print(line)
@@ -277,14 +316,16 @@
         with open(csvfile) as fr:
             lines = fr.readlines()
         with open(csvfile, 'w') as fw:
             for i, line in enumerate(lines):
                 llist = line.strip().split(',')
                 if i == 1:
                     best_parafile = llist[-1]
+                if i == 0:
+                    newlist = llist[:-1]
                 else:
                     newlist = [llist[0]]
                     for li in llist[1:-1]:
                         newlist.append(str(round(float(li), 3)))
                 newline = ','.join(newlist) + '\n'
                 fw.write(newline)
         with open(best_parafile) as fr:
```

### Comparing `unigbsa-0.1.3/launching/pipeline.py` & `unigbsa-0.1.4/launching/pipeline.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/launching/scan.py` & `unigbsa-0.1.4/launching/scan.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/setup.py` & `unigbsa-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/tests/test_pipline.py` & `unigbsa-0.1.4/tests/test_pipline.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,9 +61,10 @@
         self.pipeline_minima(pdbfile, ligandfiles)
 
     def test_md(self):
         pdbfile = '../example/1ceb/1ceb_protein.pdb'
         ligandfiles = ['../example/1ceb/1ceb_ligand.sdf']
         self.pipeline_md(pdbfile, ligandfiles)
 
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `unigbsa-0.1.3/unigbsa/CLI.py` & `unigbsa-0.1.4/unigbsa/CLI.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/data/Calibri/Calibri.ttf` & `unigbsa-0.1.4/unigbsa/data/Calibri/Calibri.ttf`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/data/Calibri/calibribold.ttf` & `unigbsa-0.1.4/unigbsa/data/Calibri/calibribold.ttf`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/data/default.ini` & `unigbsa-0.1.4/unigbsa/data/default.ini`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/data/default.json` & `unigbsa-0.1.4/unigbsa/data/default.json`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/data/mmpbsa.in` & `unigbsa-0.1.4/unigbsa/data/mmpbsa.in`

 * *Files 1% similar despite different names*

```diff
@@ -23,18 +23,18 @@
   netcdf               = 0                                              # Use NetCDF intermediate trajectories
   solvated_trajectory  = 1                                              # Define if it is necessary to cleanup the trajectories
   verbose              = 1                                              # How many energy terms to print in the final output
 /
 
 # (AMBER) Generalized-Born namelist variables
 &gb
-  igb                  = 5                                              # GB model to use
-  intdiel              = 1.0                                            # Internal dielectric constant for sander
+  igb                  = 2                                              # GB model to use
+  intdiel              = 4.0                                            # Internal dielectric constant for sander
   extdiel              = 78.5                                           # External dielectric constant for sander
-  saltcon              = 0.0                                            # Salt concentration (M)
+  saltcon              = 0.15                                           # Salt concentration (M)
   surften              = 0.0072                                         # Surface tension
   surfoff              = 0.0                                            # Surface tension offset
   molsurf              = 0                                              # Use Connelly surface ('molsurf' program)
   msoffset             = 0.0                                            # Offset for molsurf calculation
   probe                = 1.4                                            # Solvent probe radius for surface area calc
   ifqnt                = 0                                              # Use QM on part of the system
   qm_theory            = ""                                             # Semi-empirical QM theory to use
```

### Comparing `unigbsa-0.1.3/unigbsa/data/scan.json` & `unigbsa-0.1.4/unigbsa/data/scan.json`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/data/template.json` & `unigbsa-0.1.4/unigbsa/data/template.json`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/gbsa/gbsarun.py` & `unigbsa-0.1.4/unigbsa/gbsa/gbsarun.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import shutil
 import pandas as pd
 
 from unigbsa.settings import gmx_MMPBSA, MPI, logging
 from unigbsa.utils import obtain_id_from_index
-from unigbsa.gbsa.utils import obtain_num_of_frame
+from unigbsa.gbsa.utils import obtain_num_of_frame, mapping_resname
 from unigbsa.gbsa.parameters import generate_input_file
 from unigbsa.gbsa.io import parse_GMXMMPBSA_RESULTS
 
 
 '''
 1. one protein file and many other ligands file
 2. one complex file and a trajectory file.
@@ -80,15 +80,15 @@
             cmd = 'mpirun --use-hwthread-cpus --allow-run-as-root -np {numthread} \
                 {gmx_MMPBSA} MPI -i {mmpbsa} -cs {complexfile} -ci {indexfile} -ct {trajectoryfile} -cp {topolfile} -cg {receptor} {ligand} -nogui >mmpbsa.log 2>&1 '.format(**self.paras)
         else:
             cmd = '{gmx_MMPBSA} MPI -i {mmpbsa} -cs {complexfile} -ci {indexfile} -ct {trajectoryfile} -cp {topolfile} -cg {receptor} {ligand} -nogui >mmpbsa.log 2>&1 '.format(**self.paras)
         RC = os.system(cmd)
         if RC != 0:
             raise Exception('ERROR run: %s \nPlease ckeck the log file for details: %s'%(cmd, os.path.abspath("mmpbsa.log")))
-        self.save_results()
+        self.extract_result()
         self.verbose = verbose
         self.clean(verbose=verbose)
         print('='*80)
         print('Results: Energy.csv Dec.csv')
 
     def clean(self, verbose=0):
         """
@@ -103,15 +103,15 @@
             cmd = '{gmx_MMPBSA} --clean >>mmpbsa.log 2>&1 '.format(gmx_MMPBSA=gmx_MMPBSA)
             RC = os.system(cmd)
             shutil.rmtree(self.workdir)
         os.chdir(self.cwd)
 
     def extract_result(self, energyfile='Energy.csv'):
         if self.deltaG is None:
-             self.save_results()
+            self.save_results()
         return self.deltaG
 
     def extract_result_v14(self, energyfile='FINAL_RESULTS_MMPBSA.dat'):
         """
         Extract the GB and PB energy from the final results file
         
         Args:
@@ -161,15 +161,19 @@
                 elif line.startswith('ΔTOTAL'):
                     if tagName:
                         lineTemp = line.split()
                         detal_G[tagName] = (float(lineTemp[1]), float(lineTemp[2]))
                     else:
                         logging.warning("Found a DELTA G without name!")
         return detal_G
-        
-    def save_results(self, mmxsafile=None):
+   
+    def save_results(self, energyfile='Energy.csv', decfile='../Dec.csv', mmxsafile=None):
         if mmxsafile is None:
             mmxsafile = os.path.join(self.workdir, 'COMPACT_MMXSA_RESULTS.mmxsa')
         if not os.path.exists(mmxsafile):
             logging.warning('Not found mmxsa file!')
             return
         self.deltaG, self.resG = parse_GMXMMPBSA_RESULTS(mmxsafile=mmxsafile)
+        if self.resG is not None:
+            resdic = mapping_resname(self.input_pdb, self.complex)
+            self.resG['resid'] = [k if k not in resdic else resdic[k] for k in self.resG['resid']]
+            self.resG.to_csv(decfile)
```

### Comparing `unigbsa-0.1.3/unigbsa/gbsa/io.py` & `unigbsa-0.1.4/unigbsa/gbsa/io.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/gbsa/parameters.py` & `unigbsa-0.1.4/unigbsa/gbsa/parameters.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/gbsa/plots.py` & `unigbsa-0.1.4/unigbsa/gbsa/plots.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/pipeline.py` & `unigbsa-0.1.4/unigbsa/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from unigbsa.settings import logging, DEFAULT_CONFIGURE_FILE, GMXEXE, set_OMP_NUM_THREADS
 
 from tqdm import tqdm
 from multiprocessing import Pool
 
 
 KEY = ['ligandName', 'Frames', 'mode', 'complex','receptor','ligand','Internal','Van der Waals','Electrostatic','Polar Solvation','Non-Polar Solvation','Gas','Solvation','TOTAL', 'status']
-def traj_pipeline(complexfile, trajfile, topolfile, indexfile, pbsaParas=None, mmpbsafile=None, nt=1, verbose=False):
+def traj_pipeline(complexfile, trajfile, topolfile, indexfile, pbsaParas=None, mmpbsafile=None, nt=1, verbose=False, input_pdb = None):
     """
     A pipeline for calculate GBSA/PBSA for trajectory
     
     Args:
       complexfile: The name of the PDB file containing the protein-ligand complex.
       trajfile: the trajectory file, in pdb format
       topolfile: The topology file of the complex.
@@ -37,14 +37,17 @@
 
     reresfile = complexfile[:-4]+'_reres.pdb'
     cmd = '%s editconf -f %s -o %s -resnr 1 >/dev/null 2>&1'%(GMXEXE, complexfile, reresfile)
     RC = os.system(cmd)
     if RC!=0:
        raise Exception('Error convert %s to %s'%(complexfile, reresfile))
     pbsa = GBSA()
+    pbsa.complex = os.path.abspath(reresfile)
+    if input_pdb:
+        pbsa.input_pdb = os.path.abspath(input_pdb)
     mmpbsafile = pbsa.set_paras(complexfile=reresfile, trajectoryfile=trajfile, topolfile=topolfile, indexfile=indexfile, pbsaParas=pbsaParas, mmpbsafile=mmpbsafile, nt=nt)
     pbsa.run(verbose=verbose)
     detal_G = pbsa.extract_result()
     print("Frames    mode    detal_G(kcal/mole)")
     for i, irow in detal_G.iterrows():
         print('%6d    %4s    %18.4f  '%(irow['Frames'], irow['mode'], irow['TOTAL']))
     return detal_G
@@ -91,15 +94,15 @@
             dl = d
             logging.warning('Failed to generate forcefield for ligand: %s'%ligandName)
 
         indexfile = generate_index_file(grofile)
         
         if statu == 'S':
             try:
-                dl = traj_pipeline(grofile, trajfile=grofile, topolfile=topfile, indexfile=indexfile, pbsaParas=pbsaParas, mmpbsafile=mmpbsafile, verbose=verbose, nt=nt)
+                dl = traj_pipeline(grofile, trajfile=grofile, topolfile=topfile, indexfile=indexfile, pbsaParas=pbsaParas, mmpbsafile=mmpbsafile, verbose=verbose, nt=nt, input_pdb=receptorfile)
             except:
                 if len(ligandfiles)==1:
                     traceback.print_exc()
                 statu = 'F_GBSA'
                 dl = d
                 logging.warning('Failed to run GBSA for ligand: %s'%ligandName)
         ligandnames.extend([ligandName]*len(dl))
@@ -111,15 +114,15 @@
         os.chdir(cwd)
     df['ligandName'] = ligandnames
     df['status'] = status
     df[KEY].to_csv(outfile, index=False)
 
 
 def single(arg):
-    receptor, ligandfile, simParas, ligandfiles, mmpbsafile, nt, pbsaParas, verbose = arg
+    receptor, ligandfile, simParas, ligandfiles, mmpbsafile, nt, pbsaParas, verbose, receptorfile = arg
     d1 = pd.DataFrame({'Frames': 1, 'mode':pbsaParas['modes'], 'complex':0.0,'receptor':0.0,'ligand':0.0,'Internal':0.0,'Van der Waals':0.0,'Electrostatic':0,'Polar Solvation':0.0,'Non-Polar Solvation':0.0,'Gas':0.0,'Solvation':0.0,'TOTAL':0.0}, index=[1])
     cwd = os.getcwd()
     statu = 'S'
     ligandfile = os.path.abspath(ligandfile)
     ligandName = os.path.split(ligandfile)[-1][:-4]
     if not os.path.exists(ligandName):
         os.mkdir(ligandName)
@@ -158,15 +161,15 @@
             traceback.print_exc()
             logging.warning('Failed to run simulation for ligand: %s' % ligandName)
             exit(256)
         statu = 'F_md'
     indexfile = generate_index_file(grofile)
     if statu == 'S':
         try:
-            d1 = traj_pipeline(grofile, trajfile=grofile, topolfile=topfile, indexfile=indexfile, pbsaParas=pbsaParas, mmpbsafile=mmpbsafile, verbose=verbose, nt=nt)
+            d1 = traj_pipeline(grofile, trajfile=grofile, topolfile=topfile, indexfile=indexfile, pbsaParas=pbsaParas, mmpbsafile=mmpbsafile, verbose=verbose, nt=nt, input_pdb=receptorfile)
         except:
             if len(ligandfiles) == 1:
                 logging.warning('Failed to run GBSA for ligand: %s'%ligandName)
                 traceback.print_exc()
             statu = 'F_GBSA'
     if not verbose:
         engine.clean(pdbfile=grofile)
@@ -191,15 +194,15 @@
     receptorfile = os.path.abspath(receptorfile)
     logging.info('Build protein topology.')
     receptor = build_protein(receptorfile, forcefield=simParas['proteinforcefield'])
 
 
     args = [(receptor, ligandfile, simParas,
              ligandfiles, mmpbsafile, 1,
-             pbsaParas, verbose) for ligandfile in sorted(ligandfiles)]
+             pbsaParas, verbose, receptorfile) for ligandfile in sorted(ligandfiles)]
     if len(args) == 1:
         df = single(args[0])
     else:
         with Pool(nt) as pool:
             dlist = list(tqdm(pool.imap(single, args), total=len(args)))
             df = pd.concat(dlist)
     df[KEY].to_csv(outfile, index=False)
@@ -254,15 +257,15 @@
         shutil.copy(topfile, outtop)
         shutil.copy(mdxtc, xtcfile)
 
         #logging.info('Running GBSA: %s'%ligandName)
         indexfile = generate_index_file(grofile)
         if 'startframe' not in pbsaParas:
             pbsaParas["startframe"] = 2
-        deltaG = traj_pipeline(grofile, trajfile=xtcfile, topolfile=topfile, indexfile=indexfile, pbsaParas=pbsaParas, mmpbsafile=mmpbsafile, nt=nt, verbose=verbose)
+        deltaG = traj_pipeline(grofile, trajfile=xtcfile, topolfile=topfile, indexfile=indexfile, pbsaParas=pbsaParas, mmpbsafile=mmpbsafile, nt=nt, verbose=verbose, input_pdb=receptorfile)
         ligandnames.extend([ligandName]*simParas['nframe'])
         status.extend(['S']*simParas['nframe'])
         if df is None:
             df = deltaG
         else:
             df = pd.concat([df, deltaG])
         if not verbose:
```

### Comparing `unigbsa-0.1.3/unigbsa/scanparas/scan.py` & `unigbsa-0.1.4/unigbsa/scanparas/scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,14 +309,16 @@
                 receptors.append(os.path.join(protdir, fileName))
     if ligdir:
         for fileName in os.listdir(ligdir):
             if fileName.endswith(('mol', 'sdf')):
                 ligands.append(os.path.join(ligdir, fileName))
     if len(ligands) == 0 or len(receptors) == 0:
         raise Exception('No ligands or receptors file found.')
+    if len(receptors) == 1 and len(ligands) != 1:
+        receptors = receptors * len(ligands)
     with PathManager(outdir) as pm:
         expdatfile = pm.abspath(expdatfile, parent=True)
         parasfile = pm.abspath(parasfile, parent=True)
         ligands = pm.abspath(sorted([lig for lig in ligands]), parent=True)
         receptors = pm.abspath(sorted([prot for prot in receptors]), parent=True)
         logging.info('load scan paras.')
         parasdicts, simulationparas = load_scan_paras(parasfile)
```

### Comparing `unigbsa-0.1.3/unigbsa/settings.py` & `unigbsa-0.1.4/unigbsa/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 logging.basicConfig(level=logging.INFO, format=LOG_FORMAT, datefmt=DATE_FORMAT)
 
 
 gmx_MMPBSA='gmx_MMPBSA'
 if 'AMBERHOME' not in os.environ:
     #os.environ['AMBERHOME'] = set_amber_home(gmx_MMPBSA)
-    raise Exception("Not found variable AMBERHOME")
+    print("Not found variable AMBERHOME")
 
 if 'OMP_NUM_THREADS' in os.environ:
     OMP_NUM_THREADS = os.environ['OMP_NUM_THREADS']
 else:
     OMP_NUM_THREADS = 1
 
 def set_OMP_NUM_THREADS(nt):
```

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdp/ions.mdp` & `unigbsa-0.1.4/unigbsa/simulation/mdp/ions.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdp/md.mdp` & `unigbsa-0.1.4/unigbsa/simulation/mdp/md.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdp/mdout.mdp` & `unigbsa-0.1.4/unigbsa/simulation/mdp/mdout.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdp/minim.mdp` & `unigbsa-0.1.4/unigbsa/simulation/mdp/minim.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdp/minimization/s1-cg.mdp` & `unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s1-cg.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdp/minimization/s1-steep.mdp` & `unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s1-steep.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdp/minimization/s2-cg.mdp` & `unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s2-cg.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdp/minimization/s2-steep.mdp` & `unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s2-steep.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdp/minimization/s3-steep.mdp` & `unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s3-steep.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdp/minimization/s4-cg.mdp` & `unigbsa-0.1.4/unigbsa/simulation/mdp/minimization/s4-cg.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdp/npt.mdp` & `unigbsa-0.1.4/unigbsa/simulation/mdp/npt.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdp/nvt.mdp` & `unigbsa-0.1.4/unigbsa/simulation/mdp/nvt.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdp/vaccum.mdp` & `unigbsa-0.1.4/unigbsa/simulation/mdp/vaccum.mdp`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/mdrun.py` & `unigbsa-0.1.4/unigbsa/simulation/mdrun.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/openmm-em.py` & `unigbsa-0.1.4/unigbsa/simulation/openmm-em.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/topology.py` & `unigbsa-0.1.4/unigbsa/simulation/topology.py`

 * *Files identical despite different names*

### Comparing `unigbsa-0.1.3/unigbsa/simulation/utils.py` & `unigbsa-0.1.4/unigbsa/simulation/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,15 +288,15 @@
         outfile = molfile
     mol = Chem.MolFromMolFile(molfile)
     mol_out = Chem.rdmolops.AddHs(mol, addCoords=True)
     Chem.MolToMolFile(mol_out, outfile)
     return outfile
 
 
-def obtain_net_charge(molfile):
+def obtain_net_charge_command(molfile):
     import uuid
     ftype = guess_filetype(molfile)
     mol2file = str(uuid.uuid4()) + '.mol2'
     cmd = f'obabel -i {ftype} {molfile} -omol2 -O {mol2file}  >/dev/null 2>&1 '
     RC = os.system(cmd)
     if RC != 0:
         print('Failed to obtain mol charge, use guess')
@@ -304,7 +304,34 @@
     charge = 0
     with open(mol2file) as fr:
         for line in fr:
             llist = line.split()
             if len(llist) >= 8:
                 charge += float(llist[-1])
     return int(round(charge))
+
+
+def obtain_net_charge_rdkit(sdfile):
+    from rdkit import Chem
+    # Read the MOL or SDF file
+    mol = Chem.MolFromMolFile(sdfile)
+
+    # Calculate the net charge of the molecule
+    net_charge = Chem.GetFormalCharge(mol)
+
+    return net_charge
+
+
+def obtain_net_charge(sdfile):
+    from openbabel import openbabel
+    # Read the MOL or SDF file
+    mol = openbabel.OBMol()
+    with open(sdfile, 'r') as file:
+        format = sdfile[-3:]
+        file.seek(0)  # Reset the file pointer
+        obConversion = openbabel.OBConversion()
+        obConversion.SetInFormat(format)
+        obConversion.ReadString(mol, file.read())
+
+    # Calculate the net charge of the molecule
+    net_charge = mol.GetTotalCharge()
+    return net_charge
```

### Comparing `unigbsa-0.1.3/unigbsa/utils.py` & `unigbsa-0.1.4/unigbsa/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,20 +172,24 @@
                 "nframe": 100,
                 "eqsteps": 50000,
                 "proteinforcefield": "amber03",
                 "ligandforcefield": "gaff",
                 "maxsol": 0,
                 "ligandCharge": "bcc"
             }
-        for k,v in default.items():
+        for k, v in default.items():
             if k not in paras['simulation']:
                 paras['simulation'][k] = v
+        if 'PBSA' in paras:
+            paras['GBSA'] = paras['PBSA']
     elif fileformat == 'ini':
         config = configparser.ConfigParser()
         config.read(conf)
+        if 'PBSA' in config:
+            config['GBSA'] = config['PBSA']
         paras = {
                 'simulation':{
                 'mode': config.get('simulation', 'mode', fallback='em'),
                 'boxtype' : config.get('simulation', 'boxtype', fallback='triclinic'),
                 'boxsize' : config.getfloat('simulation', 'boxsize', fallback=0.9),
                 'conc': config.getfloat('simulation', 'conc', fallback=0.15),
                 'nsteps': config.getint('simulation', 'nsteps', fallback=500000),
@@ -194,9 +198,8 @@
                 'proteinforcefield': config.get('simulation', 'proteinforcefield', fallback='amber99sb-ildn'),
                 'ligandforcefield': config.get('simulation', 'ligandforcefield', fallback='gaff2'),
                 'maxsol': config.getint('simulation', 'maxsol', fallback=0),
                 'ligandCharge': config.get('simulation', 'ligandCharge', fallback='bcc'),
             },
             'GBSA':  {k:v for k,v in config.items('GBSA')}
         }
-
-    return paras
+    return paras
```

### Comparing `unigbsa-0.1.3/unigbsa.egg-info/PKG-INFO` & `unigbsa-0.1.4/unigbsa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigbsa
-Version: 0.1.3
+Version: 0.1.4
 Summary: MMPB(GB)SA tools for calculate energy.
 Home-page: https://github.com/dptech-corp/Uni-GBSA
 Author: dptech.net
 Author-email: hermite@dptech.net
 Keywords: MMPBSA MMGBSA
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `unigbsa-0.1.3/unigbsa.egg-info/SOURCES.txt` & `unigbsa-0.1.4/unigbsa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

