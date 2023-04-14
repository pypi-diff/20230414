# Comparing `tmp/Stackinator-1.0.tar.gz` & `tmp/Stackinator-1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/stackinator/stackinator/dist/tmphp7abwga/Stackinator-1.0.tar", last modified: Wed Feb 15 16:34:19 2023, max compression
+gzip compressed data, was "/home/runner/work/stackinator/stackinator/dist/tmpj8g_rbv7/Stackinator-1.1.dev0.tar", last modified: Fri Apr 14 20:14:29 2023, max compression
```

## Comparing `Stackinator-1.0.tar` & `Stackinator-1.1.dev0.tar`

### file list

```diff
@@ -1,60 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-02-15 16:34:19.000000 Stackinator-1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/stackinator/
--rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/stackinator/schema/
--rw-r--r--   0 runner    (1001) docker     (122)     1573 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/schema/config.json
--rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/schema/environments.json
--rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/schema/compilers.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/stackinator/share/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/stackinator/share/cluster-config/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/stackinator/share/cluster-config/balfrin/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/share/cluster-config/balfrin/concretizer.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/share/cluster-config/balfrin/compilers.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/share/cluster-config/balfrin/packages.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/stackinator/share/cluster-config/clariden/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/share/cluster-config/clariden/concretizer.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/share/cluster-config/clariden/compilers.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      353 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/share/cluster-config/clariden/packages.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/stackinator/share/cluster-config/hohgant/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/share/cluster-config/hohgant/concretizer.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/share/cluster-config/hohgant/compilers.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      449 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/share/cluster-config/hohgant/packages.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      381 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/share/cluster-config/hohgant/mirrors.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/stackinator/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/templates/compilers.gcc.spack.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/templates/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/templates/Make.user
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/templates/compilers.llvm.spack.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/templates/environments.spack.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/templates/Makefile.environments
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/templates/repos.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/templates/Makefile.generate-config
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/templates/compilers.bootstrap.spack.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2423 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/templates/Makefile.compilers
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     9645 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/stackinator/etc/
--rw-r--r--   0 runner    (1001) docker     (122)     6286 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/etc/cray-mpich-binary-package.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/etc/Make.inc
--rwxr-xr-x   0 runner    (1001) docker     (122)      115 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/etc/bwrap-mutable-root.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/stackinator/repo/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/repo/repo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/stackinator/repo/packages/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/stackinator/repo/packages/cray-mpich/
--rw-r--r--   0 runner    (1001) docker     (122)     7622 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/repo/packages/cray-mpich/package.py
--rw-r--r--   0 runner    (1001) docker     (122)    10932 2023-02-15 16:34:06.000000 Stackinator-1.0/stackinator/recipe.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (122)      351 2023-02-15 16:34:06.000000 Stackinator-1.0/bin/stack-config
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-02-15 16:34:06.000000 Stackinator-1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-02-15 16:34:19.000000 Stackinator-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-02-15 16:34:06.000000 Stackinator-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-02-15 16:34:06.000000 Stackinator-1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 16:34:19.000000 Stackinator-1.0/Stackinator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-02-15 16:34:19.000000 Stackinator-1.0/Stackinator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-15 16:34:19.000000 Stackinator-1.0/Stackinator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-02-15 16:34:19.000000 Stackinator-1.0/Stackinator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-15 16:34:19.000000 Stackinator-1.0/Stackinator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-15 16:34:19.000000 Stackinator-1.0/Stackinator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8488 2023-02-15 16:34:06.000000 Stackinator-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (122)     9780 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8860 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/Stackinator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9780 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/Stackinator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/Stackinator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/Stackinator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/Stackinator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/Stackinator.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      350 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/bin/stack-config
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/stackinator/
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11411 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11210 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/stackinator/etc/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      115 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/etc/bwrap-mutable-root.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/etc/Make.inc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/stackinator/repo/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/stackinator/repo/packages/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/stackinator/repo/packages/cray-mpich/
+-rw-r--r--   0 runner    (1001) docker     (122)    10091 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/repo/packages/cray-mpich/package.py
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/repo/repo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/stackinator/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/templates/environments.spack.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/templates/compilers.gcc.spack.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/templates/compilers.bootstrap.spack.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/templates/compilers.llvm.spack.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/templates/Makefile.generate-config
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/templates/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/templates/Makefile.environments
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/templates/repos.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2423 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/templates/Makefile.compilers
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/templates/Make.user
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 20:14:29.000000 Stackinator-1.1.dev0/stackinator/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)     1573 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/schema/config.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2056 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/schema/environments.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/stackinator/schema/compilers.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1512 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-14 20:14:19.000000 Stackinator-1.1.dev0/MANIFEST.in
```

### Comparing `Stackinator-1.0/setup.cfg` & `Stackinator-1.1.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `Stackinator-1.0/stackinator/schema.py` & `Stackinator-1.1.dev0/stackinator/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 import json
-import jsonschema
 import pathlib
-import yaml
+
+import jsonschema
 
 prefix = pathlib.Path(__file__).parent.resolve()
 
 # create a validator that will insert optional fields with their default values
 # if they have not been provided.
 
+
 def extend_with_default(validator_class):
     validate_properties = validator_class.VALIDATORS["properties"]
 
     def set_defaults(validator, properties, instance, schema):
         for property, subschema in properties.items():
             if "default" in subschema:
                 instance.setdefault(property, subschema["default"])
 
         for error in validate_properties(
-            validator, properties, instance, schema,
+            validator,
+            properties,
+            instance,
+            schema,
         ):
             yield error
 
     return jsonschema.validators.extend(
-        validator_class, {"properties" : set_defaults},
+        validator_class,
+        {"properties": set_defaults},
     )
 
+
 validator = extend_with_default(jsonschema.Draft7Validator)
 
 # load recipe yaml schema
-config_schema = json.load(open(prefix / 'schema/config.json'))
+config_schema = json.load(open(prefix / "schema/config.json"))
 config_validator = validator(config_schema)
-compilers_schema = json.load(open(prefix / 'schema/compilers.json'))
+compilers_schema = json.load(open(prefix / "schema/compilers.json"))
 compilers_validator = validator(compilers_schema)
-environments_schema = json.load(open(prefix / 'schema/environments.json'))
+environments_schema = json.load(open(prefix / "schema/environments.json"))
 environments_validator = validator(environments_schema)
```

### Comparing `Stackinator-1.0/stackinator/schema/config.json` & `Stackinator-1.1.dev0/stackinator/schema/config.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,24 +1,31 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "title": "Schema for Spack Stack config.yaml recipe file",
     "type": "object",
+    "additionalProperties": false,
+    "required": [
+        "name",
+        "system",
+        "spack"
+    ],
     "properties": {
         "name": {
             "type": "string"
         },
         "store": {
             "type": "string",
             "default": "/user-environment"
         },
         "system": {
             "type": "string"
         },
         "spack": {
             "type": "object",
+            "additionalProperties": false,
             "properties": {
                 "repo": {
                     "type": "string"
                 },
                 "commit": {
                     "oneOf": [
                         {
@@ -26,19 +33,23 @@
                         },
                         {
                             "type": "null"
                         }
                     ],
                     "default": null
                 }
-            },
-            "additionalProperties": false
+            }
         },
         "mirror": {
             "type": "object",
+            "additionalProperties": false,
+            "default": {
+                "enable": true,
+                "key": null
+            },
             "properties": {
                 "enable": {
                     "type": "boolean",
                     "default": true
                 },
                 "key": {
                     "oneOf": [
@@ -47,26 +58,15 @@
                         },
                         {
                             "type": "null"
                         }
                     ],
                     "default": null
                 }
-            },
-            "additionalProperties": false,
-            "default": {
-                "enable": true,
-                "key": null
             }
         },
         "modules": {
             "type": "boolean",
             "default": true
         }
-    },
-    "additionalProperties": false,
-    "required": [
-        "name",
-        "system",
-        "spack"
-    ]
+    }
 }
```

### Comparing `Stackinator-1.0/stackinator/schema/environments.json` & `Stackinator-1.1.dev0/stackinator/schema/environments.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874348958333334%*

 * *Differences: {"'patternProperties'": "{'\\\\w[\\\\w-]*': {'properties': {'compiler': {'items': "*

 * *                        "{'additionalProperties': False}}, 'mpi': {'oneOf': {0: "*

 * *                        "{'additionalProperties': False}}}}, 'additionalProperties': False}}"}*

```diff
@@ -1,15 +1,17 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "patternProperties": {
         "\\w[\\w-]*": {
+            "additionalProperties": false,
             "properties": {
                 "compiler": {
                     "items": {
+                        "additionalProperties": false,
                         "properties": {
                             "spec": {
                                 "type": "string"
                             },
                             "toolchain": {
                                 "type": "string"
                             }
@@ -18,14 +20,15 @@
                     },
                     "type": "array"
                 },
                 "mpi": {
                     "default": null,
                     "oneOf": [
                         {
+                            "additionalProperties": false,
                             "properties": {
                                 "gpu": {
                                     "enum": [
                                         "cuda",
                                         "rocm",
                                         null,
                                         false
```

### Comparing `Stackinator-1.0/stackinator/schema/compilers.json` & `Stackinator-1.1.dev0/stackinator/schema/compilers.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,11 +1,16 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "title": "Schema for Spack Stack compilers.yaml recipe file",
     "type": "object",
+    "additionalProperties": false,
+    "required": [
+        "bootstrap",
+        "gcc"
+    ],
     "defs": {
         "gcc_version_spec": {
             "type": "string",
             "pattern": "^gcc@\\d{1,2}(\\.\\d{1}(\\.\\d{1})?)?$"
         },
         "gcc_version_spec_list": {
             "type": "array",
@@ -82,14 +87,9 @@
                 },
                 {
                     "type": "null"
                 }
             ],
             "default": null
         }
-    },
-    "additionalProperties": false,
-    "required": [
-        "bootstrap",
-        "gcc"
-    ]
+    }
 }
```

### Comparing `Stackinator-1.0/stackinator/templates/Makefile` & `Stackinator-1.1.dev0/stackinator/templates/Makefile`

 * *Files identical despite different names*

### Comparing `Stackinator-1.0/stackinator/templates/Make.user` & `Stackinator-1.1.dev0/stackinator/templates/Make.user`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,14 @@
 
 # Output the full build log to stdout.
 {% if verbose %}
 export SPACK_INSTALL_FLAGS := --verbose
 {% endif %}
 
 # Reproducibility
-export LC_ALL := C
+export LC_ALL := en_US.UTF-8
 export TZ := UTC
 
 # I tried UNIX epoch 0 here, but it results in build errors with Python
 # packages using wheels, since they rely on zipfiles, and zipfiles can only
 # handle DOS epoch, which is the magic number below (1980-01-01).
 export SOURCE_DATE_EPOCH := 315576060
```

### Comparing `Stackinator-1.0/stackinator/templates/environments.spack.yaml` & `Stackinator-1.1.dev0/stackinator/templates/environments.spack.yaml`

 * *Files identical despite different names*

### Comparing `Stackinator-1.0/stackinator/templates/Makefile.environments` & `Stackinator-1.1.dev0/stackinator/templates/Makefile.environments`

 * *Files identical despite different names*

### Comparing `Stackinator-1.0/stackinator/templates/Makefile.generate-config` & `Stackinator-1.1.dev0/stackinator/templates/Makefile.generate-config`

 * *Files identical despite different names*

### Comparing `Stackinator-1.0/stackinator/templates/Makefile.compilers` & `Stackinator-1.1.dev0/stackinator/templates/Makefile.compilers`

 * *Files identical despite different names*

### Comparing `Stackinator-1.0/stackinator/main.py` & `Stackinator-1.1.dev0/stackinator/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,88 @@
 import argparse
 import hashlib
 import logging
 import os
 import platform
 import sys
 import time
+import traceback
 
-from . import root_logger, VERSION
+from . import VERSION, root_logger
 from .builder import Builder
 from .recipe import Recipe
 
 
-def generate_logfile_name(name=''):
-    idstr = f'{time.localtime()}{os.getpid}{platform.uname()}'
+def generate_logfile_name(name=""):
+    idstr = f"{time.localtime()}{os.getpid}{platform.uname()}"
     return f'log{name}_{hashlib.md5(idstr.encode("utf-8")).hexdigest()}'
 
 
 def configure_logging(logfile):
     root_logger.setLevel(logging.DEBUG)
 
     # create stdout handler and set level to info
     ch = logging.StreamHandler(stream=sys.stdout)
     ch.setLevel(logging.INFO)
-    ch.setFormatter(logging.Formatter('%(message)s'))
+    ch.setFormatter(logging.Formatter("%(message)s"))
     root_logger.addHandler(ch)
 
     # create log file handler and set level to debug
-    fh = logging.FileHandler(logfile) #, mode='w')
+    fh = logging.FileHandler(logfile)  # , mode='w')
     fh.setLevel(logging.DEBUG)
-    fh.setFormatter(
-        logging.Formatter('%(asctime)s : %(levelname)-7s : %(message)s'))
+    fh.setFormatter(logging.Formatter("%(asctime)s : %(levelname)-7s : %(message)s"))
     root_logger.addHandler(fh)
 
 
 def log_header(args):
-    root_logger.info('Stackinator')
-    root_logger.info(f'  recipe path: {args.recipe}')
-    root_logger.info(f'  build path : {args.build}')
+    root_logger.info("Stackinator")
+    root_logger.info(f"  recipe path: {args.recipe}")
+    root_logger.info(f"  build path : {args.build}")
+    system = args.system if args.system is not None else "default"
+    root_logger.info(f"  system     : {system}")
 
 
 def make_argparser():
     parser = argparse.ArgumentParser(
-        description=('Generate a build configuration for a spack stack from '
-                     'a recipe.')
+        description=(
+            "Generate a build configuration for a spack stack from " "a recipe."
+        )
+    )
+    parser.add_argument(
+        "--version", action="version", version=f"stackinator version {VERSION}"
     )
-    parser.add_argument('--version', action='version',
-                        version=f'stackinator version {VERSION}')
-    parser.add_argument('-b', '--build', required=True, type=str)
-    parser.add_argument('-r', '--recipe', required=True, type=str)
-    parser.add_argument('-d', '--debug', action='store_true')
+    parser.add_argument("-b", "--build", required=True, type=str)
+    parser.add_argument("-r", "--recipe", required=True, type=str)
+    parser.add_argument("-s", "--system", required=False, type=str)
+    parser.add_argument("-d", "--debug", action="store_true")
     return parser
 
 
 def main():
-    logfile = generate_logfile_name('_config')
+    logfile = generate_logfile_name("_config")
     configure_logging(logfile)
 
     try:
         parser = make_argparser()
         args = parser.parse_args()
-        root_logger.debug(f'Command line arguments: {args}')
+        root_logger.debug(f"Command line arguments: {args}")
         log_header(args)
 
         recipe = Recipe(args)
         builder = Builder(args)
 
         builder.generate(recipe)
 
         root_logger.info(
-            '\nConfiguration finished, run the following to build the '
-            'environment:\n'
+            "\nConfiguration finished, run the following to build the " "environment:\n"
+        )
+        root_logger.info(f"cd {builder.path}")
+        root_logger.info(
+            "env --ignore-environment PATH=/usr/bin:/bin:`pwd`"
+            "/spack/bin make store.squashfs -j32"
         )
-        root_logger.info(f'cd {builder.path}')
-        root_logger.info('env --ignore-environment PATH=/usr/bin:/bin:`pwd`'
-                    '/spack/bin make store.squashfs -j32')
         return 0
     except Exception as e:
-        root_logger.exception(e)
-        root_logger.info(f'see {logfile} for more information')
+        root_logger.debug(traceback.format_exc())
+        root_logger.error(str(e))
+        root_logger.info(f"see {logfile} for more information")
         return 1
```

### Comparing `Stackinator-1.0/stackinator/builder.py` & `Stackinator-1.1.dev0/stackinator/builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,243 +1,288 @@
-from datetime import datetime
 import json
-import logging
 import os
 import pathlib
 import platform
 import shutil
 import subprocess
 import sys
+from datetime import datetime
 
 import jinja2
 import yaml
 
-from . import root_logger
-from . import VERSION 
+from . import VERSION, root_logger
 
 
 class Builder:
     def __init__(self, args):
-        self._logger = root_logger 
+        self._logger = root_logger
         path = pathlib.Path(args.build)
         if not path.is_absolute():
             path = pathlib.Path.cwd() / path
 
+        # check that if the path exists that it is not a file
         if path.exists():
             if not path.is_dir():
-                raise IOError('build path is not a directory')
+                raise IOError("build path is not a directory")
+
+        parts = path.parts
+
+        # the build path can't be root
+        if len(parts) == 1:
+            raise IOError("build path can't be root '/'")
+
+        # the build path can't be in /tmp because the build step rebinds /tmp.
+        if parts[1] == "tmp":
+            raise IOError("build path can't be in '/tmp'")
 
         self.path = path
-        self.root = prefix = pathlib.Path(__file__).parent.resolve()
+        self.root = pathlib.Path(__file__).parent.resolve()
 
     def generate(self, recipe):
         # make the paths
-        store_path = self.path / 'store'
-        tmp_path = self.path / 'tmp'
+        store_path = self.path / "store"
+        tmp_path = self.path / "tmp"
 
         self.path.mkdir(exist_ok=True, parents=True)
         store_path.mkdir(exist_ok=True)
         tmp_path.mkdir(exist_ok=True)
 
         # check out the version of spack
-        spack = recipe.config['spack']
-        spack_path = self.path / 'spack'
+        spack = recipe.config["spack"]
+        spack_path = self.path / "spack"
 
         # generate configuration meta data
         meta = {}
-        meta['time'] = datetime.now().strftime("%Y%m%d %H:%M:%S")
+        meta["time"] = datetime.now().strftime("%Y%m%d %H:%M:%S")
         host_data = platform.uname()
-        meta['host'] = {
-                'machine': host_data.machine,
-                'node': host_data.node,
-                'processor': host_data.processor,
-                'release': host_data.release,
-                'system': host_data.system,
-                'version': host_data.version
+        meta["host"] = {
+            "machine": host_data.machine,
+            "node": host_data.node,
+            "processor": host_data.processor,
+            "release": host_data.release,
+            "system": host_data.system,
+            "version": host_data.version,
         }
-        meta['cluster'] = os.getenv('CLUSTER_NAME', default='unknown')
-        meta['stackinator'] = {
-                'version': VERSION,
-                'args': sys.argv,
-                'python': sys.executable
+        meta["cluster"] = os.getenv("CLUSTER_NAME", default="unknown")
+        meta["stackinator"] = {
+            "version": VERSION,
+            "args": sys.argv,
+            "python": sys.executable,
         }
-        meta['spack'] = recipe.config['spack']
+        meta["spack"] = recipe.config["spack"]
         self.meta = meta
 
         # Clone the spack repository if it has not already been checked out
-        if not (spack_path / '.git').is_dir():
+        if not (spack_path / ".git").is_dir():
             self._logger.info(f'spack: clone repository {spack["repo"]}')
 
             # clone the repository
             capture = subprocess.run(
-                ["git", "clone", spack['repo'], spack_path],
+                ["git", "clone", spack["repo"], spack_path],
                 shell=False,
                 stdout=subprocess.PIPE,
-                stderr=subprocess.STDOUT)
-            self._logger.debug(capture.stdout.decode('utf-8'))
+                stderr=subprocess.STDOUT,
+            )
+            self._logger.debug(capture.stdout.decode("utf-8"))
 
             if capture.returncode != 0:
                 self._logger.debug(f'error cloning the repository {spack["repo"]}')
                 capture.check_returncode()
 
         # Check out a branch or commit if one was specified
-        if spack['commit']:
+        if spack["commit"]:
             self._logger.info(f'spack: checkout branch/commit {spack["commit"]}')
             capture = subprocess.run(
-                ["git", "-C", spack_path, "checkout", spack['commit']],
+                ["git", "-C", spack_path, "checkout", spack["commit"]],
                 shell=False,
                 stdout=subprocess.PIPE,
-                stderr=subprocess.STDOUT)
-            self._logger.debug(capture.stdout.decode('utf-8'))
+                stderr=subprocess.STDOUT,
+            )
+            self._logger.debug(capture.stdout.decode("utf-8"))
 
             if capture.returncode != 0:
                 self._logger.debug(
-                    f'unable to change to the requested commit {spack["commit"]}')
+                    f'unable to change to the requested commit {spack["commit"]}'
+                )
                 capture.check_returncode()
 
         # load the jinja templating environment
-        template_path = self.root / 'templates'
+        template_path = self.root / "templates"
         env = jinja2.Environment(
-            loader = jinja2.FileSystemLoader(template_path),
-            trim_blocks=True, lstrip_blocks=True)
+            loader=jinja2.FileSystemLoader(template_path),
+            trim_blocks=True,
+            lstrip_blocks=True,
+        )
 
         # generate top level makefiles
-        makefile_template = env.get_template('Makefile')
-        with (self.path / 'Makefile').open('w') as f:
-            cache = {'key': recipe.mirror.key, 'enabled': recipe.mirror.source}
-            f.write(makefile_template.render(
-                cache=cache, modules=recipe.config['modules'], verbose=False))
-            f.write('\n')
-
-        make_user_template = env.get_template('Make.user')
-        with (self.path / 'Make.user').open('w') as f:
-            f.write(make_user_template.render(
-                build_path=self.path, store=recipe.config['store'],
-                verbose=False))
-            f.write('\n')
-
-        etc_path = self.root / 'etc'
-        for f in ['Make.inc', 'bwrap-mutable-root.sh']:
-            shutil.copy2(etc_path / f, self.path / f)
+        makefile_template = env.get_template("Makefile")
+        with (self.path / "Makefile").open("w") as f:
+            cache = {"key": recipe.mirror.key, "enabled": recipe.mirror.source}
+            f.write(
+                makefile_template.render(
+                    cache=cache, modules=recipe.config["modules"], verbose=False
+                )
+            )
+            f.write("\n")
+
+        make_user_template = env.get_template("Make.user")
+        with (self.path / "Make.user").open("w") as f:
+            f.write(
+                make_user_template.render(
+                    build_path=self.path, store=recipe.config["store"], verbose=False
+                )
+            )
+            f.write("\n")
+
+        etc_path = self.root / "etc"
+        for f_etc in ["Make.inc", "bwrap-mutable-root.sh"]:
+            shutil.copy2(etc_path / f_etc, self.path / f_etc)
 
         # Generate the system configuration: the compilers, environments,
         # mirrors etc. that are defined for the target cluster.
-        config_path = self.path / 'config'
+        config_path = self.path / "config"
         config_path.mkdir(exist_ok=True)
         system_configs_path = pathlib.Path(recipe.configs_path)
 
         # Copy the yaml files to the spack config path
-        for f in system_configs_path.iterdir():
+        for f_config in system_configs_path.iterdir():
             # skip copying mirrors.yaml - this is done in the next step only if
             # mirrors have been enabled and the recipe did not provide a mirror
             # configuration
-            if f.name in ['mirrors.yaml']:
+            if f_config.name in ["mirrors.yaml"]:
                 continue
 
             # construct full file path
-            src = system_configs_path / f.name
-            dst = config_path / f.name
+            src = system_configs_path / f_config.name
+            dst = config_path / f_config.name
             # copy only files
             if src.is_file():
                 shutil.copy(src, dst)
 
         # copy the optional mirrors.yaml file
         if recipe.mirror.source:
-            dst = config_path / 'mirrors.yaml'
+            dst = config_path / "mirrors.yaml"
             shutil.copy(recipe.mirror.source, dst)
 
         # append recipe packages to packages.yaml
         if recipe.packages:
-            system_packages = system_configs_path / 'packages.yaml'
+            system_packages = system_configs_path / "packages.yaml"
             packages_data = {}
             if system_packages.is_file():
                 # load system yaml
                 with system_packages.open() as fid:
                     raw = yaml.load(fid, Loader=yaml.Loader)
-                    packages_data = raw['packages']
-            packages_data.update(recipe.packages['packages'])
-            packages_yaml = yaml.dump({'packages': packages_data})
-            packages_path = config_path / 'packages.yaml'
+                    packages_data = raw["packages"]
+            packages_data.update(recipe.packages["packages"])
+            packages_yaml = yaml.dump({"packages": packages_data})
+            packages_path = config_path / "packages.yaml"
             with packages_path.open("w") as fid:
                 fid.write(packages_yaml)
 
         # Configure the CSCS custom spack environments.
         # Step 1: copy the CSCS repo to store_path where, it will be used to
         #         build the stack, and then be part of the upstream provided
         #         to users of the stack.
-        repo_src = self.root / 'repo'
-        repo_dst = store_path / 'repo'
+        repo_src = self.root / "repo"
+        repo_dst = store_path / "repo"
         if repo_dst.exists():
             shutil.rmtree(repo_dst)
 
         shutil.copytree(repo_src, repo_dst)
 
         # Step 2: Create a repos.yaml file in build_path/config
-        repos_yaml_template = env.get_template('repos.yaml')
-        with (config_path / 'repos.yaml').open('w') as f:
-            repo_path = pathlib.Path(recipe.config['store']) / 'repo'
-            f.write(repos_yaml_template.render(
-                repo_path=repo_path.as_posix(),verbose=False))
-            f.write('\n')
+        repos_yaml_template = env.get_template("repos.yaml")
+        with (config_path / "repos.yaml").open("w") as f:
+            repo_path = pathlib.Path(recipe.config["store"]) / "repo"
+            f.write(
+                repos_yaml_template.render(
+                    repo_path=repo_path.as_posix(), verbose=False
+                )
+            )
+            f.write("\n")
+
+        # Add user-defined repo to internal repo
+        user_repo_path = recipe.path / "repo"
+        if user_repo_path.exists() and user_repo_path.is_dir():
+            user_repo_yaml = user_repo_path / "repo.yaml"
+            if user_repo_yaml.exists():
+                self._logger.warning(f"Found 'repo.yaml' file in {user_repo_path}")
+                self._logger.warning(
+                    "'repo.yaml' is ignored, packages are added to the 'alps' repo"
+                )
+
+            # Copy user-provided recipes into repo
+            user_repo_packages = user_repo_path / "packages"
+            for user_recipe_dir in user_repo_packages.iterdir():
+                if user_recipe_dir.is_dir():  # iterdir() yelds files too
+                    shutil.copytree(
+                        user_recipe_dir, repo_dst / "packages" / user_recipe_dir.name
+                    )
 
         # Generate the makefile and spack.yaml files that describe the compilers
         compilers = recipe.generate_compilers()
-        compiler_path = self.path / 'compilers'
+        compiler_path = self.path / "compilers"
         compiler_path.mkdir(exist_ok=True)
-        with (compiler_path / 'Makefile').open(mode='w') as f:
-            f.write(compilers['makefile'])
+        with (compiler_path / "Makefile").open(mode="w") as f:
+            f.write(compilers["makefile"])
 
-        for name, yml in compilers['config'].items():
+        for name, yml in compilers["config"].items():
             compiler_config_path = compiler_path / name
             compiler_config_path.mkdir(exist_ok=True)
-            with (compiler_config_path / 'spack.yaml').open(mode='w') as f:
+            with (compiler_config_path / "spack.yaml").open(mode="w") as f:
                 f.write(yml)
 
         # generate the makefile and spack.yaml files that describe the environments
         environments = recipe.generate_environments()
-        environments_path = self.path / 'environments'
+        environments_path = self.path / "environments"
         os.makedirs(environments_path, exist_ok=True)
-        with (environments_path / 'Makefile').open(mode='w') as f:
-            f.write(environments['makefile'])
+        with (environments_path / "Makefile").open(mode="w") as f:
+            f.write(environments["makefile"])
 
-        for name, yml in environments['config'].items():
+        for name, yml in environments["config"].items():
             env_config_path = environments_path / name
             env_config_path.mkdir(exist_ok=True)
-            with (env_config_path / 'spack.yaml').open(mode='w') as f:
+            with (env_config_path / "spack.yaml").open(mode="w") as f:
                 f.write(yml)
 
         # generate the makefile that generates the configuration for the spack
         # installation
-        make_config_template = env.get_template('Makefile.generate-config')
-        generate_config_path = self.path / 'generate-config'
+        make_config_template = env.get_template("Makefile.generate-config")
+        generate_config_path = self.path / "generate-config"
         generate_config_path.mkdir(exist_ok=True)
 
         # write the Makefile
-        all_compilers=[x for x in recipe.compilers.keys()]
-        release_compilers=[x for x in all_compilers if x != "bootstrap"]
-        with (generate_config_path / 'Makefile').open('w') as f:
-            f.write(make_config_template.render(
-                build_path=self.path.as_posix(),
-                all_compilers=all_compilers,
-                release_compilers=release_compilers,
-                verbose=False))
+        all_compilers = [x for x in recipe.compilers.keys()]
+        release_compilers = [x for x in all_compilers if x != "bootstrap"]
+        with (generate_config_path / "Makefile").open("w") as f:
+            f.write(
+                make_config_template.render(
+                    build_path=self.path.as_posix(),
+                    all_compilers=all_compilers,
+                    release_compilers=release_compilers,
+                    verbose=False,
+                )
+            )
 
         # write the modules.yaml file
-        modules_yaml=recipe.generate_modules()
-        generate_modules_path = self.path / 'modules'
+        modules_yaml = recipe.generate_modules()
+        generate_modules_path = self.path / "modules"
         generate_modules_path.mkdir(exist_ok=True)
-        with (generate_modules_path / 'modules.yaml').open('w') as f:
+        with (generate_modules_path / "modules.yaml").open("w") as f:
             f.write(modules_yaml)
 
         # write the meta data
-        meta_path = self.path / 'store/meta'
+        meta_path = self.path / "store/meta"
         meta_path.mkdir(exist_ok=True)
         # write a json file with basic meta data
-        with (meta_path / 'configure.json').open('w') as f:
+        with (meta_path / "configure.json").open("w") as f:
             f.write(json.dumps(self.meta, sort_keys=True, indent=2))
-            f.write('\n')
+            f.write("\n")
         # copy the recipe to a recipe subdirectory of the meta path
-        meta_recipe_path = meta_path / 'recipe'
+        meta_recipe_path = meta_path / "recipe"
         meta_recipe_path.mkdir(exist_ok=True)
         if meta_recipe_path.exists():
             shutil.rmtree(meta_recipe_path)
-        shutil.copytree(recipe.path, meta_recipe_path)
+        shutil.copytree(
+            recipe.path, meta_recipe_path, ignore=shutil.ignore_patterns(".git")
+        )
```

### Comparing `Stackinator-1.0/stackinator/etc/cray-mpich-binary-package.py` & `Stackinator-1.1.dev0/stackinator/repo/packages/cray-mpich/package.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,68 @@
-# Copyright 2013-2022 Lawrence Livermore National Security, LLC and other
+# Copyright 2013-2023 Lawrence Livermore National Security, LLC and other
 # Spack Project Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (Apache-2.0 OR MIT)
 
 import os
 
 import spack.compilers
 from spack.package import *
 
 
-class CrayMpichBinary(Package):
+class CrayMpich(Package):
     """Install cray-mpich as a binary package"""
 
+    """Intended to override the main cray-mpich"""
+
     homepage = "https://www.hpe.com/us/en/compute/hpc/hpc-software.html"
     url = "https://jfrog.svc.cscs.ch/artifactory/cray-mpich/cray-mpich-8.1.18.4-gcc.tar.gz"
 
     maintainers = ["haampie"]
 
-    version("8.1.21.1-gcc",
-            sha256="0a6852ebf06afd249285fd09566e8489300cba96ad66e90c40df36b6af9a631e",
-            url="https://jfrog.svc.cscs.ch/artifactory/cray-mpich/cray-mpich-8.1.21.1-gcc.tar.gz")
-    version("8.1.21.1-nvhpc",
-            sha256="791b39f2ecb933060abaa8c8704e71da01c6962c4211cc99d12b9d964e9be4cb",
-            url="https://jfrog.svc.cscs.ch/artifactory/cray-mpich/cray-mpich-8.1.21.1-nvhpc.tar.gz")
-    version("8.1.18.4-gcc",
-            sha256="776c695aeed62b3f64a1bca11b30a2537a907777a8664d2f092e3deac288e4ad",
-            url="https://jfrog.svc.cscs.ch/artifactory/cray-mpich/cray-mpich-8.1.18.4-gcc.tar.gz")
-    version("8.1.18.4-nvhpc",
-            sha256="2285433363c75a04ccdf4798be5b0e296e0c9a8fb8fcb38eb0aa4ccf8d1e0843",
-            url="https://jfrog.svc.cscs.ch/artifactory/cray-mpich/cray-mpich-8.1.18.4-nvhpc.tar.gz")
+    version(
+        "8.1.24-gcc",
+        sha256="3da0e421c3faaadbe18e57dd033b0ec6513e0d9ed7fbfa77f05a02bada4cd483",
+        url="https://jfrog.svc.cscs.ch/artifactory/cray-mpich/cray-mpich-8.1.24-gcc.tar.gz",
+    )
+    version(
+        "8.1.24-nvhpc",
+        sha256="1b507f4e9150cf188a0571aad0d190fc8ee981def1d6198c998673d73828ed6f",
+        url="https://jfrog.svc.cscs.ch/artifactory/cray-mpich/cray-mpich-8.1.24-nvhpc.tar.gz",
+    )
+    version(
+        "8.1.23-gcc",
+        sha256="2d1dfda811848d278548b0d7735f17341c70380dbf7f91dc680e5afcfb5e0038",
+        url="https://jfrog.svc.cscs.ch/artifactory/cray-mpich/cray-mpich-8.1.23-gcc.tar.gz",
+    )
+    version(
+        "8.1.23-nvhpc",
+        sha256="1dd9b161c538dbac564ecff6f1552220ba40dcc9436dc855087438f29861eba1",
+        url="https://jfrog.svc.cscs.ch/artifactory/cray-mpich/cray-mpich-8.1.23-nvhpc.tar.gz",
+    )
+    version(
+        "8.1.21.1-gcc",
+        sha256="0a6852ebf06afd249285fd09566e8489300cba96ad66e90c40df36b6af9a631e",
+        url="https://jfrog.svc.cscs.ch/artifactory/cray-mpich/cray-mpich-8.1.21.1-gcc.tar.gz",
+    )
+    version(
+        "8.1.21.1-nvhpc",
+        sha256="791b39f2ecb933060abaa8c8704e71da01c6962c4211cc99d12b9d964e9be4cb",
+        url="https://jfrog.svc.cscs.ch/artifactory/cray-mpich/cray-mpich-8.1.21.1-nvhpc.tar.gz",
+    )
+    version(
+        "8.1.18.4-gcc",
+        sha256="776c695aeed62b3f64a1bca11b30a2537a907777a8664d2f092e3deac288e4ad",
+        url="https://jfrog.svc.cscs.ch/artifactory/cray-mpich/cray-mpich-8.1.18.4-gcc.tar.gz",
+    )
+    version(
+        "8.1.18.4-nvhpc",
+        sha256="2285433363c75a04ccdf4798be5b0e296e0c9a8fb8fcb38eb0aa4ccf8d1e0843",
+        url="https://jfrog.svc.cscs.ch/artifactory/cray-mpich/cray-mpich-8.1.18.4-nvhpc.tar.gz",
+    )
 
     variant("cuda", default=False)
     variant("rocm", default=False)
 
     conflicts("+cuda", when="+rocm", msg="Pick either CUDA or ROCM")
 
     provides("mpi")
@@ -48,14 +78,44 @@
         depends_on("hip@5:", type="link")
         # libhsa-runtime64.so.1
         depends_on("hsa-rocr-dev", type="link")
 
     # libfabric.so.1
     depends_on("libfabric@1:", type="link")
 
+    with when("@8.1.24-gcc"):
+        # libgfortran.so.5
+        conflicts("%gcc@:7")
+        for __compiler in spack.compilers.supported_compilers():
+            if __compiler != "gcc":
+                conflicts("%{}".format(__compiler), msg="gcc required")
+
+    with when("@8.1.24-nvhpc"):
+        conflicts("%nvhpc@:20.7")
+        conflicts("+rocm")
+        conflicts("~cuda")
+        for __compiler in spack.compilers.supported_compilers():
+            if __compiler != "nvhpc":
+                conflicts("%{}".format(__compiler), msg="nvhpc required")
+
+    with when("@8.1.23-gcc"):
+        # libgfortran.so.5
+        conflicts("%gcc@:7")
+        for __compiler in spack.compilers.supported_compilers():
+            if __compiler != "gcc":
+                conflicts("%{}".format(__compiler), msg="gcc required")
+
+    with when("@8.1.23-nvhpc"):
+        conflicts("%nvhpc@:20.6")
+        conflicts("+rocm")
+        conflicts("~cuda")
+        for __compiler in spack.compilers.supported_compilers():
+            if __compiler != "nvhpc":
+                conflicts("%{}".format(__compiler), msg="nvhpc required")
+
     with when("@8.1.21.1-gcc"):
         # libgfortran.so.5
         conflicts("%gcc@:7")
         for __compiler in spack.compilers.supported_compilers():
             if __compiler != "gcc":
                 conflicts("%{}".format(__compiler), msg="gcc required")
 
@@ -128,14 +188,18 @@
         rpath = self.get_rpaths()
         for root, _, files in os.walk(self.prefix):
             for name in files:
                 f = os.path.join(root, name)
                 if not self.should_patch(f):
                     continue
                 patchelf("--force-rpath", "--set-rpath", rpath, f, fail_on_error=False)
+                # The C compiler wrapper can fail because libmpi_gtl_cuda refers to the symbol
+                # __gxx_personality_v0 but wasn't linked against libstdc++.
+                if "libmpi_gtl_cuda.so" in str(f):
+                    patchelf("--add-needed", "libstdc++.so", f, fail_on_error=False)
 
     @run_after("install")
     def fixup_compiler_paths(self):
         filter_file("@@CC@@", self.compiler.cc, self.prefix.bin.mpicc, string=True)
         filter_file("@@CXX@@", self.compiler.cxx, self.prefix.bin.mpicxx, string=True)
         filter_file("@@FC@@", self.compiler.fc, self.prefix.bin.mpifort, string=True)
 
@@ -149,8 +213,47 @@
         elif "+rocm" in self.spec:
             gtl_library = "-lmpi_gtl_hsa"
         else:
             gtl_library = ""
 
         filter_file("@@GTL_LIBRARY@@", gtl_library, self.prefix.bin.mpicc, string=True)
         filter_file("@@GTL_LIBRARY@@", gtl_library, self.prefix.bin.mpicxx, string=True)
-        filter_file("@@GTL_LIBRARY@@", gtl_library, self.prefix.bin.mpifort, string=True)
+        filter_file(
+            "@@GTL_LIBRARY@@", gtl_library, self.prefix.bin.mpifort, string=True
+        )
+ 
+    @property
+    def headers(self):
+        hdrs = find_headers("mpi", self.prefix.include, recursive=True)
+        hdrs += find_headers("cray_version", self.prefix.include, recursive=True) # cray_version.h
+        # cray-mpich depends on cray-pmi
+        hdrs += find_headers("pmi", self.prefix.include, recursive=True) # See cray-pmi package
+        hdrs.directories = os.path.dirname(hdrs[0])
+        return hdrs
+
+    @property
+    def libs(self):
+        query_parameters = self.spec.last_query.extra_parameters
+
+        libraries = ["libmpi", "libmpich"]
+
+        if "f77" in query_parameters:
+            libraries.extend(["libmpifort", "libmpichfort", "libfmpi", "libfmpich"])
+
+        if "f90" in query_parameters:
+            libraries.extend(["libmpif90", "libmpichf90"])
+
+        if "+cuda" in self.spec:
+            libraries.append("libmpi*cuda")
+        
+        if "+rocm" in self.spec:
+            libraries.append("libmpi*hsa")
+
+        libs = []
+        for lib_folder in [self.prefix.lib, self.prefix.lib64]:
+            libs += find_libraries(libraries, root=lib_folder, recursive=True)
+            # cray-mpich depends on cray-pmi
+            libs += find_libraries("libpmi", root=lib_folder, recursive=True)
+            libs += find_libraries("libopa", root=lib_folder, recursive=True)
+            libs += find_libraries("libmpl", root=lib_folder, recursive=True)
+
+        return libs
```

### Comparing `Stackinator-1.0/stackinator/etc/Make.inc` & `Stackinator-1.1.dev0/stackinator/etc/Make.inc`

 * *Files identical despite different names*

### Comparing `Stackinator-1.0/stackinator/recipe.py` & `Stackinator-1.1.dev0/stackinator/recipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,294 +1,324 @@
 import pathlib
-import logging
 
 import jinja2
 import yaml
 
-from . import schema
-from . import root_logger
+from . import root_logger, schema
 
 
 class Mirror:
     def __init__(self, config, source):
         if config:
-            enabled = config.get('enable', True)
-            key = config.get('key', None)
+            enabled = config.get("enable", True)
+            key = config.get("key", None)
             self._source = None if not enabled else source
-            self._key  = key
+            self._key = key
         else:
             self._source = self._key = None
 
     @property
     def key(self):
         return self._key
 
     @property
     def source(self):
         return self._source
 
 
 class Recipe:
     valid_mpi_specs = {
-        "cray-mpich":  (None, None),
-        "mpich":  ("4.1", "device=ch4 netmod=ofi +slurm"),
+        "cray-mpich": (None, None),
+        "mpich": ("4.1", "device=ch4 netmod=ofi +slurm"),
         "mvapich2": (
-            "3.0a", 
-            "+xpmem fabrics=ch4ofi ch4_max_vcis=4 process_managers=slurm"
-        )
+            "3.0a",
+            "+xpmem fabrics=ch4ofi ch4_max_vcis=4 process_managers=slurm",
+        ),
     }
 
     def __init__(self, args):
         self._logger = root_logger
-        self._logger.debug('Generating recipe')
+        self._logger.debug("Generating recipe")
         path = pathlib.Path(args.recipe)
         if not path.is_absolute():
             path = pathlib.Path.cwd() / path
 
-        if not path.is_dir:
+        if not path.is_dir():
             raise FileNotFoundError(f"The recipe path '{path}' does not exist")
 
         self.path = path
-        self.root = prefix = pathlib.Path(__file__).parent.resolve()
-
+        self.root = pathlib.Path(__file__).parent.resolve()
 
         # required compiler.yaml file
-        compiler_path = path / 'compilers.yaml'
-        self._logger.debug(f'opening {compiler_path}')
+        compiler_path = path / "compilers.yaml"
+        self._logger.debug(f"opening {compiler_path}")
         if not compiler_path.is_file():
-            raise FileNotFoundError(f"The recipe path '{compiler_path}' does "
-                                    f"not contain compilers.yaml")
+            raise FileNotFoundError(
+                f"The recipe path '{compiler_path}' does " f"not contain compilers.yaml"
+            )
 
         with compiler_path.open() as fid:
             raw = yaml.load(fid, Loader=yaml.Loader)
-            if 'compilers' in raw:
+            if "compilers" in raw:
                 self._logger.warning(
                     f"{compiler_path} uses deprecated 'compilers:' "
                     f"header. This will be an error in future releases."
                 )
-                raw = raw['compilers']
+                raw = raw["compilers"]
             schema.compilers_validator.validate(raw)
             self.generate_compiler_specs(raw)
 
         # required environments.yaml file
-        environments_path = path / 'environments.yaml'
-        self._logger.debug(f'opening {environments_path}')
+        environments_path = path / "environments.yaml"
+        self._logger.debug(f"opening {environments_path}")
         if not environments_path.is_file():
-            raise FileNotFoundError(f"The recipe path '{environments_path}' does "
-                                    f" not contain environments.yaml")
+            raise FileNotFoundError(
+                f"The recipe path '{environments_path}' does "
+                f" not contain environments.yaml"
+            )
 
         with environments_path.open() as fid:
             raw = yaml.load(fid, Loader=yaml.Loader)
             schema.environments_validator.validate(raw)
             self.generate_environment_specs(raw)
 
         # required config.yaml file
-        config_path = path / 'config.yaml'
-        self._logger.debug(f'opening {config_path}')
+        config_path = path / "config.yaml"
+        self._logger.debug(f"opening {config_path}")
         if not config_path.is_file():
-            raise FileNotFoundError(f"The recipe path '{config_path}' does "
-                                    f"not contain compilers.yaml")
+            raise FileNotFoundError(
+                f"The recipe path '{config_path}' does " f"not contain compilers.yaml"
+            )
 
         with config_path.open() as fid:
             raw = yaml.load(fid, Loader=yaml.Loader)
             schema.config_validator.validate(raw)
             self.config = raw
 
+        # override the system target
+        if args.system:
+            self.config["system"] = args.system
+
         # optional modules.yaml file
-        modules_path = path / 'modules.yaml'
-        self._logger.debug(f'opening {modules_path}')
+        modules_path = path / "modules.yaml"
+        self._logger.debug(f"opening {modules_path}")
         if not modules_path.is_file():
-            modules_path = (pathlib.Path(args.build) / 
-                'spack/etc/spack/defaults/modules.yaml')
-            self._logger.debug(
-                f'no modules.yaml provided - using the {modules_path}')
+            modules_path = (
+                pathlib.Path(args.build) / "spack/etc/spack/defaults/modules.yaml"
+            )
+            self._logger.debug(f"no modules.yaml provided - using the {modules_path}")
 
         self.modules = modules_path
+        if not self.configs_path.is_dir():
+            raise FileNotFoundError(
+                f"The system {self.config['system']!r} is not a supported cluster"
+            )
 
         # optional packages.yaml file
-        packages_path = path / 'packages.yaml'
-        self._logger.debug(f'opening {packages_path}')
+        packages_path = path / "packages.yaml"
+        self._logger.debug(f"opening {packages_path}")
         self.packages = None
         if packages_path.is_file():
             with packages_path.open() as fid:
                 self.packages = yaml.load(fid, Loader=yaml.Loader)
 
         # Select location of the mirrors.yaml file to use.
         # Look first in the recipe path, then in the system configuration path.
-        mirrors_path = path / 'mirrors.yaml'
+        mirrors_path = path / "mirrors.yaml"
         mirrors_source = mirrors_path if mirrors_path.is_file() else None
-        if mirrors_source == None:
-            mirrors_path = self.configs_path / 'mirrors.yaml'
+        if mirrors_source is None:
+            mirrors_path = self.configs_path / "mirrors.yaml"
             mirrors_source = mirrors_path if mirrors_path.is_file() else None
 
-        self._mirror = Mirror(config=self.config['mirror'],
-                              source=mirrors_source)
+        self._mirror = Mirror(config=self.config["mirror"], source=mirrors_source)
 
     @property
     def mirror(self):
         return self._mirror
 
     def generate_modules(self):
         with self.modules.open() as fid:
             raw = yaml.load(fid, Loader=yaml.Loader)
-            raw['modules']['default']['roots']['tcl'] = (
-                pathlib.Path(self.config['store']) / 'modules').as_posix()
+            raw["modules"]["default"]["roots"]["tcl"] = (
+                pathlib.Path(self.config["store"]) / "modules"
+            ).as_posix()
             return yaml.dump(raw)
 
     # creates the self.environments field that describes the full specifications
     # for all of the environments sets, grouped in environments, from the raw
     # environments.yaml input.
     def generate_environment_specs(self, raw):
         environments = raw
 
         # check the environment descriptions and ammend where features are missing
         for name, config in environments.items():
-            if ("specs" not in config) or (config["specs"] == None):
+            if ("specs" not in config) or (config["specs"] is None):
                 environments[name]["specs"] = []
 
-            if ("mpi" not in config):
+            if "mpi" not in config:
                 environments[name]["mpi"] = {"spec": None, "gpu": None}
 
         for name, config in environments.items():
             if config["mpi"]:
                 mpi = config["mpi"]
                 mpi_spec = mpi["spec"]
                 mpi_gpu = mpi["gpu"]
                 if mpi_spec:
                     try:
-                        mpi_impl, mpi_ver = mpi_spec.strip().split(
-                            sep='@', maxsplit=1)
+                        mpi_impl, mpi_ver = mpi_spec.strip().split(sep="@", maxsplit=1)
                     except ValueError:
                         mpi_impl = mpi_spec.strip()
                         mpi_ver = None
 
                     if mpi_impl in Recipe.valid_mpi_specs:
                         default_ver, options = Recipe.valid_mpi_specs[mpi_impl]
                         if mpi_ver:
-                            version_opt = f"@{mpi_ver}" 
+                            version_opt = f"@{mpi_ver}"
                         else:
                             version_opt = f"@{default_ver}" if default_ver else ""
 
                         spec = f"{mpi_impl}{version_opt} {options or ''}".strip()
 
                         if mpi_gpu:
-                            if mpi_impl != 'cray-mpich':
+                            if mpi_impl != "cray-mpich":
                                 spec = f"{spec} cuda_arch=80"
                             else:
                                 spec = f"{spec} +{mpi_gpu}"
 
                         environments[name]["specs"].append(spec)
                     else:
                         # TODO: Create a custom exception type
-                        raise Exception(f'Unsupported mpi: {mpi_impl}')
+                        raise Exception(f"Unsupported mpi: {mpi_impl}")
 
         self.environments = environments
 
-
     # creates the self.compilers field that describes the full specifications
     # for all of teh compilers from the raw compilers.yaml input
     def generate_compiler_specs(self, raw):
         compilers = {}
 
         bootstrap = {}
-        bootstrap["packages"]= {
-            "external": ["perl", "m4", "autoconf", "automake", "libtool", 
-                         "gawk", "python", "texinfo", "gawk"],
+        bootstrap["packages"] = {
+            "external": [
+                "perl",
+                "m4",
+                "autoconf",
+                "automake",
+                "libtool",
+                "gawk",
+                "python",
+                "texinfo",
+                "gawk",
+            ],
             "variants": {
                 "gcc": "[build_type=Release ~bootstrap +strip]",
                 "mpc": "[libs=static]",
                 "gmp": "[libs=static]",
                 "mpfr": "[libs=static]",
                 "zstd": "[libs=static]",
-                "zlib": "[~shared]"
-            }
+                "zlib": "[~shared]",
+            },
         }
         bootstrap_spec = raw["bootstrap"]["spec"]
-        bootstrap["specs"] = [f"{bootstrap_spec} languages=c,c++",
-                              f"squashfs default_compression=zstd"]
+        bootstrap["specs"] = [
+            f"{bootstrap_spec} languages=c,c++",
+            "squashfs default_compression=zstd",
+        ]
         compilers["bootstrap"] = bootstrap
 
         gcc = {}
         gcc["packages"] = {
-            "external": ["perl", "m4", "autoconf", "automake", "libtool",
-                         "gawk", "python", "texinfo", "gawk"],
+            "external": [
+                "perl",
+                "m4",
+                "autoconf",
+                "automake",
+                "libtool",
+                "gawk",
+                "python",
+                "texinfo",
+                "gawk",
+            ],
             "variants": {
                 "gcc": "[build_type=Release +profiled +strip]",
                 "mpc": "[libs=static]",
                 "gmp": "[libs=static]",
                 "mpfr": "[libs=static]",
                 "zstd": "[libs=static]",
-                "zlib": "[~shared]"
-            }
+                "zlib": "[~shared]",
+            },
         }
         gcc["specs"] = raw["gcc"]["specs"]
         gcc["requires"] = bootstrap_spec
         compilers["gcc"] = gcc
         if raw["llvm"] is not None:
             llvm = {}
             llvm["packages"] = False
             llvm["specs"] = []
             for spec in raw["llvm"]["specs"]:
                 if spec.startswith("nvhpc"):
                     llvm["specs"].append(f"{spec}~mpi~blas~lapack")
 
                 if spec.startswith("llvm"):
                     llvm["specs"].append(
-                        f"{spec} +clang targets=x86 ~gold ^ninja@kitware")
+                        f"{spec} +clang targets=x86 ~gold ^ninja@kitware"
+                    )
 
             llvm["requires"] = raw["llvm"]["requires"]
             compilers["llvm"] = llvm
 
         self.compilers = compilers
 
     # The path of the default configuration for the target system/cluster
     @property
     def configs_path(self):
-        system = self.config['system']
-        return self.root / 'share' / 'cluster-config' / system
+        system = self.config["system"]
+        return self.root / "cluster-config" / system
 
-    # Boolean flag that indicates whether the recipe is configured to use 
+    # Boolean flag that indicates whether the recipe is configured to use
     # a binary cache.
     def generate_compilers(self):
         files = {}
 
-        template_path = self.root / 'templates'
+        template_path = self.root / "templates"
         env = jinja2.Environment(
-            loader = jinja2.FileSystemLoader(template_path),
-            trim_blocks=True, lstrip_blocks=True)
+            loader=jinja2.FileSystemLoader(template_path),
+            trim_blocks=True,
+            lstrip_blocks=True,
+        )
 
-        makefile_template = env.get_template('Makefile.compilers')
+        makefile_template = env.get_template("Makefile.compilers")
         push_to_cache = self.mirror.source and self.mirror.key
-        files['makefile'] = makefile_template.render(
-            compilers=self.compilers,
-            push_to_cache=push_to_cache)
+        files["makefile"] = makefile_template.render(
+            compilers=self.compilers, push_to_cache=push_to_cache
+        )
 
         # generate compilers/<compiler>/spack.yaml
-        files['config'] = {}
+        files["config"] = {}
         for compiler, config in self.compilers.items():
-            spack_yaml_template = env.get_template(
-                f'compilers.{compiler}.spack.yaml')
-            files['config'][compiler] = spack_yaml_template.render(
-                config=config)
+            spack_yaml_template = env.get_template(f"compilers.{compiler}.spack.yaml")
+            files["config"][compiler] = spack_yaml_template.render(config=config)
 
         return files
 
     def generate_environments(self):
         files = {}
 
-        template_path = self.root / 'templates'
+        template_path = self.root / "templates"
         jenv = jinja2.Environment(
-            loader = jinja2.FileSystemLoader(template_path),
-            trim_blocks=True, lstrip_blocks=True)
+            loader=jinja2.FileSystemLoader(template_path),
+            trim_blocks=True,
+            lstrip_blocks=True,
+        )
 
-        makefile_template = jenv.get_template('Makefile.environments')
+        makefile_template = jenv.get_template("Makefile.environments")
         push_to_cache = self.mirror.source and self.mirror.key
-        files['makefile'] = makefile_template.render(
-            environments=self.environments,
-            push_to_cache=push_to_cache)
+        files["makefile"] = makefile_template.render(
+            environments=self.environments, push_to_cache=push_to_cache
+        )
 
-        files['config'] = {}
+        files["config"] = {}
         for env, config in self.environments.items():
-            spack_yaml_template = jenv.get_template('environments.spack.yaml')
-            files['config'][env] = spack_yaml_template.render(config=config)
+            spack_yaml_template = jenv.get_template("environments.spack.yaml")
+            files["config"][env] = spack_yaml_template.render(config=config)
 
         return files
```

### Comparing `Stackinator-1.0/PKG-INFO` & `Stackinator-1.1.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Stackinator
-Version: 1.0
+Version: 1.1.dev0
 Summary: Stackinator is a tool for building a scientific software stack from a recipe for vClusters on CSCS' Alps infrastructure
 Home-page: https://github.com/eth-cscs/stackinator
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich)
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
@@ -287,14 +287,18 @@
   - tmux
   - reframe
   packages:
     all:
       compiler: [gcc@11.3]
 ```
 
+### repo
+
+New Spack packages or custom versions of a package can be added to the `alps` repo. If a `repo/` folder is provided, `stackinator` will copy all the Spack packages in `repo/packages/` into the `alps` repo (the same repo providing `cray-mpich`). If the user provides a `repo.yaml` file in the `repo/` folder, the file will be ignored (and a warning is emitted).
+
 ### modules
 
 Modules are generated for the installed compilers and packages by spack. The default module generation rules set by the version of spack specified in `config.yaml` will be used if no `modules.yaml` file is provided.
 
 To set rules for module generation, provide a `module.yaml` file as per the [spack documentation](https://spack.readthedocs.io/en/latest/module_file_support.html).
 
 To disable module generation, set the field `config:modules:False` in `config.yaml`.
```

### Comparing `Stackinator-1.0/LICENSE` & `Stackinator-1.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `Stackinator-1.0/Stackinator.egg-info/SOURCES.txt` & `Stackinator-1.1.dev0/Stackinator.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -12,30 +12,19 @@
 stackinator/__init__.py
 stackinator/builder.py
 stackinator/main.py
 stackinator/recipe.py
 stackinator/schema.py
 stackinator/etc/Make.inc
 stackinator/etc/bwrap-mutable-root.sh
-stackinator/etc/cray-mpich-binary-package.py
 stackinator/repo/repo.yaml
 stackinator/repo/packages/cray-mpich/package.py
 stackinator/schema/compilers.json
 stackinator/schema/config.json
 stackinator/schema/environments.json
-stackinator/share/cluster-config/balfrin/compilers.yaml
-stackinator/share/cluster-config/balfrin/concretizer.yaml
-stackinator/share/cluster-config/balfrin/packages.yaml
-stackinator/share/cluster-config/clariden/compilers.yaml
-stackinator/share/cluster-config/clariden/concretizer.yaml
-stackinator/share/cluster-config/clariden/packages.yaml
-stackinator/share/cluster-config/hohgant/compilers.yaml
-stackinator/share/cluster-config/hohgant/concretizer.yaml
-stackinator/share/cluster-config/hohgant/mirrors.yaml
-stackinator/share/cluster-config/hohgant/packages.yaml
 stackinator/templates/Make.user
 stackinator/templates/Makefile
 stackinator/templates/Makefile.compilers
 stackinator/templates/Makefile.environments
 stackinator/templates/Makefile.generate-config
 stackinator/templates/compilers.bootstrap.spack.yaml
 stackinator/templates/compilers.gcc.spack.yaml
```

### Comparing `Stackinator-1.0/Stackinator.egg-info/PKG-INFO` & `Stackinator-1.1.dev0/Stackinator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Stackinator
-Version: 1.0
+Version: 1.1.dev0
 Summary: Stackinator is a tool for building a scientific software stack from a recipe for vClusters on CSCS' Alps infrastructure
 Home-page: https://github.com/eth-cscs/stackinator
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich)
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
@@ -287,14 +287,18 @@
   - tmux
   - reframe
   packages:
     all:
       compiler: [gcc@11.3]
 ```
 
+### repo
+
+New Spack packages or custom versions of a package can be added to the `alps` repo. If a `repo/` folder is provided, `stackinator` will copy all the Spack packages in `repo/packages/` into the `alps` repo (the same repo providing `cray-mpich`). If the user provides a `repo.yaml` file in the `repo/` folder, the file will be ignored (and a warning is emitted).
+
 ### modules
 
 Modules are generated for the installed compilers and packages by spack. The default module generation rules set by the version of spack specified in `config.yaml` will be used if no `modules.yaml` file is provided.
 
 To set rules for module generation, provide a `module.yaml` file as per the [spack documentation](https://spack.readthedocs.io/en/latest/module_file_support.html).
 
 To disable module generation, set the field `config:modules:False` in `config.yaml`.
```

### Comparing `Stackinator-1.0/README.md` & `Stackinator-1.1.dev0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -265,14 +265,18 @@
   - tmux
   - reframe
   packages:
     all:
       compiler: [gcc@11.3]
 ```
 
+### repo
+
+New Spack packages or custom versions of a package can be added to the `alps` repo. If a `repo/` folder is provided, `stackinator` will copy all the Spack packages in `repo/packages/` into the `alps` repo (the same repo providing `cray-mpich`). If the user provides a `repo.yaml` file in the `repo/` folder, the file will be ignored (and a warning is emitted).
+
 ### modules
 
 Modules are generated for the installed compilers and packages by spack. The default module generation rules set by the version of spack specified in `config.yaml` will be used if no `modules.yaml` file is provided.
 
 To set rules for module generation, provide a `module.yaml` file as per the [spack documentation](https://spack.readthedocs.io/en/latest/module_file_support.html).
 
 To disable module generation, set the field `config:modules:False` in `config.yaml`.
```

