# Comparing `tmp/streamflow-0.2.0.dev3.tar.gz` & `tmp/streamflow-0.2.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamflow-0.2.0.dev3.tar", last modified: Mon Mar 13 13:41:48 2023, max compression
+gzip compressed data, was "streamflow-0.2.0.dev4.tar", last modified: Fri Apr 14 13:07:17 2023, max compression
```

## Comparing `streamflow-0.2.0.dev3.tar` & `streamflow-0.2.0.dev4.tar`

### file list

```diff
@@ -1,160 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.890254 streamflow-0.2.0.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-03-13 13:41:48.890254 streamflow-0.2.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/bandit-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.862254 streamflow-0.2.0.dev3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/lint-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/report-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 13:41:48.890254 streamflow-0.2.0.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.862254 streamflow-0.2.0.dev3/streamflow/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.866253 streamflow-0.2.0.dev3/streamflow/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.854253 streamflow-0.2.0.dev3/streamflow/config/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.866253 streamflow-0.2.0.dev3/streamflow/config/schemas/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/config/schemas/v1.0/config_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/config/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.866253 streamflow-0.2.0.dev3/streamflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/core/asyncache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/core/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/core/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/core/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/core/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/core/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/core/scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24035 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.870254 streamflow-0.2.0.dev3/streamflow/cwl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.874254 streamflow-0.2.0.dev3/streamflow/cwl/antlr/
--rw-r--r--   0 runner    (1001) docker     (123)    51958 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/antlr/ECMAScriptLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    33090 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/antlr/ECMAScriptListener.py
--rw-r--r--   0 runner    (1001) docker     (123)   228628 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/antlr/ECMAScriptParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/antlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/combinator.py
--rw-r--r--   0 runner    (1001) docker     (123)    52827 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22258 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)   113337 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)    39963 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/cwl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.874254 streamflow-0.2.0.dev3/streamflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/data/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/data/remotepath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.874254 streamflow-0.2.0.dev3/streamflow/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/data/schemas/data_manager.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.874254 streamflow-0.2.0.dev3/streamflow/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36140 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/aiotarstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.878254 streamflow-0.2.0.dev3/streamflow/deployment/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    47417 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/occam.py
--rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.878254 streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/docker-compose.json
--rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/docker.json
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/helm3.json
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/local.json
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/occam.json
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/queue_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/singularity.json
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/ssh.json
--rw-r--r--   0 runner    (1001) docker     (123)    25535 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/connector/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/deployment_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.878254 streamflow-0.2.0.dev3/streamflow/deployment/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.882254 streamflow-0.2.0.dev3/streamflow/deployment/filter/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/filter/schemas/shuffle.json
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/filter/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/future.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.882254 streamflow-0.2.0.dev3/streamflow/deployment/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/schemas/deployment_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/deployment/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.882254 streamflow-0.2.0.dev3/streamflow/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/ext/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/ext/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.882254 streamflow-0.2.0.dev3/streamflow/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/persistence/loading_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.882254 streamflow-0.2.0.dev3/streamflow/persistence/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/persistence/schemas/sqlite.json
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/persistence/schemas/sqlite.sql
--rw-r--r--   0 runner    (1001) docker     (123)    19471 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/persistence/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.882254 streamflow-0.2.0.dev3/streamflow/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53948 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/provenance/run_crate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.882254 streamflow-0.2.0.dev3/streamflow/recovery/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/recovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/recovery/checkpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/recovery/failure_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/recovery/recovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.886254 streamflow-0.2.0.dev3/streamflow/recovery/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/recovery/schemas/default_checkpoint_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/recovery/schemas/default_failure_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/recovery/schemas/dummy_checkpoint_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/recovery/schemas/dummy_failure_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.886254 streamflow-0.2.0.dev3/streamflow/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/scheduling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.886254 streamflow-0.2.0.dev3/streamflow/scheduling/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/scheduling/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/scheduling/policy/data_locality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.886254 streamflow-0.2.0.dev3/streamflow/scheduling/policy/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/scheduling/policy/schemas/data_locality.json
--rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/scheduling/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.886254 streamflow-0.2.0.dev3/streamflow/scheduling/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/scheduling/schemas/scheduler.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.890254 streamflow-0.2.0.dev3/streamflow/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/workflow/combinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/workflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/workflow/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    62216 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/workflow/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/workflow/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/workflow/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/streamflow/workflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.862254 streamflow-0.2.0.dev3/streamflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-03-13 13:41:48.000000 streamflow-0.2.0.dev3/streamflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-03-13 13:41:48.000000 streamflow-0.2.0.dev3/streamflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 13:41:48.000000 streamflow-0.2.0.dev3/streamflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-13 13:41:48.000000 streamflow-0.2.0.dev3/streamflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-13 13:41:48.000000 streamflow-0.2.0.dev3/streamflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-13 13:41:48.000000 streamflow-0.2.0.dev3/streamflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 13:41:48.000000 streamflow-0.2.0.dev3/streamflow.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:41:48.890254 streamflow-0.2.0.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/tests/test_cwl_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    24802 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/tests/test_cwl_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/tests/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/tests/test_remotepath.py
--rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-03-13 13:41:32.000000 streamflow-0.2.0.dev3/tests/test_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/bandit-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.130355 streamflow-0.2.0.dev4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/lint-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/report-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.130355 streamflow-0.2.0.dev4/streamflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.134355 streamflow-0.2.0.dev4/streamflow/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.126355 streamflow-0.2.0.dev4/streamflow/config/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.134355 streamflow-0.2.0.dev4/streamflow/config/schemas/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/config/schemas/v1.0/config_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/config/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.134355 streamflow-0.2.0.dev4/streamflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/asyncache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24035 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.134355 streamflow-0.2.0.dev4/streamflow/cwl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/cwl/antlr/
+-rw-r--r--   0 runner    (1001) docker     (123)    51958 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/antlr/ECMAScriptLexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33090 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/antlr/ECMAScriptListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)   228628 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/antlr/ECMAScriptParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/antlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/combinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52552 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/cwl/requirement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/kubernetes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/docker.json
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/kubernetes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/singularity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22258 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113737 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39908 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/cwl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/data/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/data/remotepath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/data/schemas/data_manager.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.138355 streamflow-0.2.0.dev4/streamflow/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36140 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/aiotarstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/deployment/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53904 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43913 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/occam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22133 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/docker-compose.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/docker.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/helm3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/kubernetes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/local.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/occam.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/queue_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/singularity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/ssh.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25573 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/connector/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/deployment_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/deployment/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/deployment/filter/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/filter/schemas/shuffle.json
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/filter/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/future.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/deployment/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/schemas/deployment_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/deployment/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/ext/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/ext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/persistence/loading_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/persistence/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/persistence/schemas/sqlite.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/persistence/schemas/sqlite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    19471 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/persistence/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53948 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/provenance/run_crate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/recovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/checkpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/failure_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/recovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/recovery/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/schemas/default_checkpoint_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/schemas/default_failure_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/schemas/dummy_checkpoint_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/recovery/schemas/dummy_failure_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.142355 streamflow-0.2.0.dev4/streamflow/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/scheduling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/streamflow/scheduling/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/scheduling/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/scheduling/policy/data_locality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/streamflow/scheduling/policy/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/scheduling/policy/schemas/data_locality.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/scheduling/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/streamflow/scheduling/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/scheduling/schemas/scheduler.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/streamflow/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/combinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62216 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/streamflow/workflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.130355 streamflow-0.2.0.dev4/streamflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-04-14 13:07:17.000000 streamflow-0.2.0.dev4/streamflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-14 13:07:17.000000 streamflow-0.2.0.dev4/streamflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:07:17.000000 streamflow-0.2.0.dev4/streamflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-14 13:07:17.000000 streamflow-0.2.0.dev4/streamflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 13:07:17.000000 streamflow-0.2.0.dev4/streamflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 13:07:17.000000 streamflow-0.2.0.dev4/streamflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:07:16.000000 streamflow-0.2.0.dev4/streamflow.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:17.146355 streamflow-0.2.0.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/tests/test_cwl_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24802 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/tests/test_cwl_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/tests/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/tests/test_remotepath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-04-14 13:07:07.000000 streamflow-0.2.0.dev4/tests/test_transfer.py
```

### Comparing `streamflow-0.2.0.dev3/LICENSE` & `streamflow-0.2.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/PKG-INFO` & `streamflow-0.2.0.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow
-Version: 0.2.0.dev3
+Version: 0.2.0.dev4
 Summary: StreamFlow framework
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://streamflow.di.unito.it
 Project-URL: Package, https://pypi.org/project/streamflow
 Project-URL: Repository, https://github.com/alpha-unito/streamflow
 Project-URL: Docker, https://hub.docker.com/r/alphaunito/streamflow
```

### Comparing `streamflow-0.2.0.dev3/README.md` & `streamflow-0.2.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/pyproject.toml` & `streamflow-0.2.0.dev4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 [tool.setuptools]
 packages = [
     "streamflow",
     "streamflow.config",
     "streamflow.core",
     "streamflow.cwl",
     "streamflow.cwl.antlr",
+    "streamflow.cwl.requirement",
+    "streamflow.cwl.requirement.docker",
     "streamflow.data",
     "streamflow.deployment",
     "streamflow.deployment.connector",
     "streamflow.deployment.filter",
     "streamflow.ext",
     "streamflow.persistence",
     "streamflow.provenance",
@@ -58,14 +60,15 @@
     "streamflow.scheduling.policy",
     "streamflow.workflow"
 ]
 zip-safe = true
 
 [tool.setuptools.package-data]
 "streamflow.config" = ["schemas/v1.0/*.json"]
+"streamflow.cwl.requirement.docker" = ["schemas/*.jinja2", "schemas/*.json"]
 "streamflow.data" = ["schemas/*.json"]
 "streamflow.deployment" = ["schemas/*.json"]
 "streamflow.deployment.connector" = ["schemas/*.json"]
 "streamflow.deployment.filter" = ["schemas/*.json"]
 "streamflow.persistence" = ["schemas/*.sql", "schemas/*.json"]
 "streamflow.recovery" = ["schemas/*.json"]
 "streamflow.scheduling" = ["schemas/*.json"]
```

### Comparing `streamflow-0.2.0.dev3/streamflow/config/config.py` & `streamflow-0.2.0.dev4/streamflow/config/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,26 +55,15 @@
                 for b in binding:
                     self._process_binding(b)
                 self.scheduling_groups[utils.random_name()] = binding
             else:
                 self._process_binding(binding)
         set_targets(self.filesystem, None)
 
-    def _build_config(self, path: PurePosixPath) -> MutableMapping[str, Any]:
-        current_node = self.filesystem
-        for part in path.parts:
-            if part not in current_node["children"]:
-                current_node["children"][part] = {"children": {}}
-            current_node = current_node["children"][part]
-        return current_node
-
     def _process_binding(self, binding: MutableMapping[str, Any]):
-        current_config = self._build_config(
-            PurePosixPath(binding["step"] if "step" in binding else binding["port"])
-        )
         targets = (
             binding["target"]
             if isinstance(binding["target"], MutableSequence)
             else [binding["target"]]
         )
         for target in targets:
             policy = target.get(
@@ -93,15 +82,16 @@
             )
         config = {"targets": targets, "filters": []}
         for f in binding.get("filters", []):
             if f in self.binding_filters:
                 config["filters"].append(self.binding_filters[f])
             else:
                 raise WorkflowDefinitionException(f"Binding filter {f} is not defined")
-        current_config[target_type] = config
+        path = PurePosixPath(binding["step"] if "step" in binding else binding["port"])
+        self.put(path, target_type, config)
 
     def get(
         self, path: PurePosixPath, name: str, default: Any | None = None
     ) -> Any | None:
         current_node = self.filesystem
         for part in path.parts:
             if part not in current_node["children"]:
@@ -115,7 +105,15 @@
         for part in path.parts:
             if part not in current_node["children"]:
                 return value
             current_node = current_node["children"][part]
             if name in current_node:
                 value = current_node[name]
         return value
+
+    def put(self, path: PurePosixPath, name: str, value: Any) -> None:
+        current_node = self.filesystem
+        for part in path.parts:
+            if part not in current_node["children"]:
+                current_node["children"][part] = {"children": {}}
+            current_node = current_node["children"][part]
+        current_node[name] = value
```

### Comparing `streamflow-0.2.0.dev3/streamflow/config/schemas/v1.0/config_schema.json` & `streamflow-0.2.0.dev4/streamflow/config/schemas/v1.0/config_schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935852920227921%*

 * *Differences: {"'definitions'": "{'workflow': {'definitions': {'cwl': {'properties': {'docker': "*

 * *                  "OrderedDict([('type', 'array'), ('items', OrderedDict([('type', 'object'), "*

 * *                  "('properties', OrderedDict([('step', OrderedDict([('type', 'string')])), "*

 * *                  "('deployment', OrderedDict([('type', 'object'), ('$ref', "*

 * *                  "'#/definitions/cwl/docker')]))])), ('additionalProperties', False), "*

 * *                  "('required', ['step', 'deployment'])]))])}}}}, 'cwl' […]*

```diff
@@ -99,14 +99,38 @@
                 "required": [
                     "type",
                     "config"
                 ]
             },
             "type": "object"
         },
+        "cwl": {
+            "$id": "#/definitions/cwl",
+            "docker": {
+                "$comment": "The `config` property is injected by each CWLDockerTranslator extension",
+                "$id": "#/definitions/cwl/docker",
+                "definitions": {},
+                "properties": {
+                    "type": {
+                        "type": "string"
+                    },
+                    "wrapper": {
+                        "default": true,
+                        "description": "If true, the Docker target wraps the original target bound to the step. If false, it overrides it.",
+                        "type": "boolean"
+                    }
+                },
+                "required": [
+                    "type",
+                    "config"
+                ],
+                "type": "object"
+            },
+            "type": "object"
+        },
         "dataManager": {
             "$comment": "The `config` property is injected by each DataManager extension",
             "$id": "#/definitions/dataManager",
             "definitions": {},
             "properties": {
                 "type": {
                     "type": "string"
@@ -317,14 +341,34 @@
                 }
             ],
             "definitions": {
                 "cwl": {
                     "$id": "#/definitions/workflow/definitions/cwl",
                     "additionalProperties": false,
                     "properties": {
+                        "docker": {
+                            "items": {
+                                "additionalProperties": false,
+                                "properties": {
+                                    "deployment": {
+                                        "$ref": "#/definitions/cwl/docker",
+                                        "type": "object"
+                                    },
+                                    "step": {
+                                        "type": "string"
+                                    }
+                                },
+                                "required": [
+                                    "step",
+                                    "deployment"
+                                ],
+                                "type": "object"
+                            },
+                            "type": "array"
+                        },
                         "file": {
                             "type": "string"
                         },
                         "settings": {
                             "type": "string"
                         }
                     },
```

### Comparing `streamflow-0.2.0.dev3/streamflow/config/validator.py` & `streamflow-0.2.0.dev4/streamflow/config/validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pkg_resources
 from jsonref import loads
 from jsonschema import Draft7Validator
 from ruamel.yaml import YAML
 
 from streamflow.core import utils
 from streamflow.core.exception import WorkflowDefinitionException
+from streamflow.cwl.requirement.docker import cwl_docker_translator_classes
 from streamflow.data import data_manager_classes
 from streamflow.deployment import deployment_manager_classes
 from streamflow.deployment.connector import connector_classes
 from streamflow.deployment.filter import binding_filter_classes
 from streamflow.persistence import database_classes
 from streamflow.recovery import checkpoint_manager_classes, failure_manager_classes
 from streamflow.scheduling import scheduler_classes
@@ -58,14 +59,15 @@
             streamflow_config = self.yaml.load(f)
         return self.validate(streamflow_config)
 
     def validate(self, streamflow_config: MutableMapping[str, Any]):
         schema = load_jsonschema(streamflow_config)
         utils.inject_schema(schema, binding_filter_classes, "bindingFilter")
         utils.inject_schema(schema, checkpoint_manager_classes, "checkpointManager")
+        utils.inject_schema(schema, cwl_docker_translator_classes, "cwl/docker")
         utils.inject_schema(schema, database_classes, "database")
         utils.inject_schema(schema, data_manager_classes, "dataManager")
         utils.inject_schema(schema, connector_classes, "deployment")
         utils.inject_schema(schema, deployment_manager_classes, "deploymentManager")
         utils.inject_schema(schema, failure_manager_classes, "failureManager")
         utils.inject_schema(schema, policy_classes, "policy")
         utils.inject_schema(schema, scheduler_classes, "scheduler")
```

### Comparing `streamflow-0.2.0.dev3/streamflow/core/asyncache.py` & `streamflow-0.2.0.dev4/streamflow/core/asyncache.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/core/config.py` & `streamflow-0.2.0.dev4/streamflow/core/config.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/core/context.py` & `streamflow-0.2.0.dev4/streamflow/core/context.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/core/data.py` & `streamflow-0.2.0.dev4/streamflow/core/data.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/core/deployment.py` & `streamflow-0.2.0.dev4/streamflow/core/deployment.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/core/exception.py` & `streamflow-0.2.0.dev4/streamflow/core/exception.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/core/persistence.py` & `streamflow-0.2.0.dev4/streamflow/core/persistence.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/core/provenance.py` & `streamflow-0.2.0.dev4/streamflow/core/provenance.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/core/recovery.py` & `streamflow-0.2.0.dev4/streamflow/core/recovery.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/core/scheduling.py` & `streamflow-0.2.0.dev4/streamflow/core/scheduling.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,21 +125,21 @@
 class JobAllocation:
     __slots__ = ("job", "target", "locations", "status", "hardware")
 
     def __init__(
         self,
         job: str,
         target: Target,
-        locations: MutableSequence[Location],
+        locations: MutableSequence[AvailableLocation],
         status: Status,
         hardware: Hardware,
     ):
         self.job: str = job
         self.target: Target = target
-        self.locations: MutableSequence[Location] = locations
+        self.locations: MutableSequence[AvailableLocation] = locations
         self.status: Status = status
         self.hardware: Hardware = hardware
 
 
 class AvailableLocation(Location):
     __slots__ = ("hostname", "hardware", "slots")
 
@@ -228,15 +228,15 @@
             )
             if allocation
             else None
         )
 
     def get_locations(
         self, job_name: str, statuses: MutableSequence[Status] | None = None
-    ) -> MutableSequence[Location]:
+    ) -> MutableSequence[AvailableLocation]:
         allocation = self.get_allocation(job_name)
         return (
             allocation.locations
             if allocation is not None
             and (statuses is None or allocation.status in statuses)
             else []
         )
```

### Comparing `streamflow-0.2.0.dev3/streamflow/core/utils.py` & `streamflow-0.2.0.dev4/streamflow/core/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -135,48 +135,82 @@
 
 def get_date_from_ns(timestamp: int) -> str:
     base = datetime.datetime(1970, 1, 1)
     delta = datetime.timedelta(microseconds=round(timestamp / 1000))
     return (base + delta).replace(tzinfo=datetime.timezone.utc).isoformat()
 
 
+async def get_local_to_remote_destination(
+    dst_connector: Connector, dst_location: Location, src: str, dst: str
+):
+    is_dst_dir, status = await dst_connector.run(
+        location=dst_location,
+        command=[f'test -d "{dst}"'],
+        capture_output=True,
+    )
+    if status > 1:
+        raise WorkflowExecutionException(is_dst_dir)
+    # If destination path exists and is a directory
+    elif status == 0:
+        # Append src basename to dst
+        return posixpath.join(dst, os.path.basename(src))
+    # Otherwise
+    else:
+        # Keep current dst
+        return dst
+
+
 async def get_remote_to_remote_write_command(
     src_connector: Connector,
     src_location: Location,
     src: str,
     dst_connector: Connector,
     dst_locations: MutableSequence[Location],
     dst: str,
 ) -> MutableSequence[str]:
-    if posixpath.basename(src) != posixpath.basename(dst):
-        result, status = await src_connector.run(
-            location=src_location,
-            command=[f'test -d "{src}"'],
-            capture_output=True,
-        )
-        if status > 1:
-            raise WorkflowExecutionException(result)
-        # If is a directory
-        elif status == 0:
-            await asyncio.gather(
-                *(
-                    asyncio.create_task(
-                        dst_connector.run(
-                            location=dst_location, command=["mkdir", "-p", dst]
+    is_dst_dir, status = await dst_connector.run(
+        location=dst_locations[0],
+        command=[f'test -d "{dst}"'],
+        capture_output=True,
+    )
+    if status > 1:
+        raise WorkflowExecutionException(is_dst_dir)
+    # If destination path exists and is a directory
+    elif status == 0:
+        return ["tar", "xf", "-", "-C", dst]
+    # Otherwise, if destination path does not exist
+    else:
+        # If basename must be renamed during trnasfer
+        if posixpath.basename(src) != posixpath.basename(dst):
+            is_src_dir, status = await src_connector.run(
+                location=src_location,
+                command=[f'test -d "{src}"'],
+                capture_output=True,
+            )
+            if status > 1:
+                raise WorkflowExecutionException(is_src_dir)
+            # If source path is a directory
+            elif status == 0:
+                await asyncio.gather(
+                    *(
+                        asyncio.create_task(
+                            dst_connector.run(
+                                location=dst_location, command=["mkdir", "-p", dst]
+                            )
                         )
+                        for dst_location in dst_locations
                     )
-                    for dst_location in dst_locations
                 )
-            )
-            return ["tar", "xf", "-", "-C", dst, "--strip-components", "1"]
-        # If is a file
+                return ["tar", "xf", "-", "-C", dst, "--strip-components", "1"]
+            # Otherwise, if source path is a file
+            else:
+                return ["tar", "xf", "-", "-O", "|", "tee", dst, ">", "/dev/null"]
+        # Otherwise, if basename must be preserved
         else:
-            return ["tar", "xf", "-", "-O", ">", dst]
-    else:
-        return ["tar", "xf", "-", "-C", posixpath.dirname(dst)]
+            return ["tar", "xf", "-", "-C", posixpath.dirname(dst)]
 
 
 def get_size(path):
     if os.path.isfile(path):
         return os.path.getsize(path)
     else:
         total_size = 0
@@ -204,19 +238,20 @@
         if entity_schema := entity.get_schema():
             with open(entity_schema) as f:
                 entity_schema = loads(
                     f.read(),
                     base_uri=f"file://{os.path.dirname(entity_schema)}/",
                     jsonschema=True,
                 )
-            schema["definitions"][definition_name]["properties"]["type"].setdefault(
-                "enum", []
-            ).append(name)
-            schema["definitions"][definition_name]["definitions"][name] = entity_schema
-            schema["definitions"][definition_name].setdefault("allOf", []).append(
+            definition = schema["definitions"]
+            for el in definition_name.split(posixpath.sep):
+                definition = definition[el]
+            definition["properties"]["type"].setdefault("enum", []).append(name)
+            definition["definitions"][name] = entity_schema
+            definition.setdefault("allOf", []).append(
                 {
                     "if": {"properties": {"type": {"const": name}}},
                     "then": {"properties": {"config": entity_schema}},
                 }
             )
```

### Comparing `streamflow-0.2.0.dev3/streamflow/core/workflow.py` & `streamflow-0.2.0.dev4/streamflow/core/workflow.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/antlr/ECMAScriptLexer.py` & `streamflow-0.2.0.dev4/streamflow/cwl/antlr/ECMAScriptLexer.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/antlr/ECMAScriptListener.py` & `streamflow-0.2.0.dev4/streamflow/cwl/antlr/ECMAScriptListener.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/antlr/ECMAScriptParser.py` & `streamflow-0.2.0.dev4/streamflow/cwl/antlr/ECMAScriptParser.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/combinator.py` & `streamflow-0.2.0.dev4/streamflow/cwl/combinator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/command.py` & `streamflow-0.2.0.dev4/streamflow/cwl/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -774,22 +774,17 @@
                     command=base64.b64encode(" ".join(cmd).encode("utf-8")).decode(
                         "utf-8"
                     )
                 ),
             ]
         # If step is assigned to multiple locations, add the STREAMFLOW_HOSTS environment variable
         if len(locations) > 1:
-            service = self.step.workflow.context.scheduler.get_service(job.name)
-            available_locations = await connector.get_available_locations(
-                service=service
+            parsed_env["STREAMFLOW_HOSTS"] = ",".join(
+                [loc.hostname for loc in locations]
             )
-            hosts = {
-                k: v.hostname for k, v in available_locations.items() if k in locations
-            }
-            parsed_env["STREAMFLOW_HOSTS"] = ",".join(hosts.values())
         # Process streams
         stdin = utils.eval_expression(
             expression=self.stdin,
             context=context,
             full_js=self.full_js,
             expression_lib=self.expression_lib,
         )
```

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/expression.py` & `streamflow-0.2.0.dev4/streamflow/cwl/expression.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/hardware.py` & `streamflow-0.2.0.dev4/streamflow/cwl/hardware.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/main.py` & `streamflow-0.2.0.dev4/streamflow/cwl/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 import argparse
 import json
 import logging
 import os
+from pathlib import PurePosixPath
 
 import cwltool.context
 import cwltool.load_tool
 import cwltool.loghandler
 import cwltool.main
 import cwltool.utils
 
 from streamflow.config.config import WorkflowConfig
 from streamflow.core.context import StreamFlowContext
+from streamflow.cwl.requirement.docker.translator import CWLDockerTranslatorConfig
 from streamflow.cwl.translator import CWLTranslator
 from streamflow.cwl.utils import load_cwl_inputs, load_cwl_workflow
 from streamflow.log_handler import logger
 from streamflow.workflow.executor import StreamFlowExecutor
 
 
 def _parse_arg(path: str, context: StreamFlowContext):
     if "://" in path:
         return path
-    elif os.path.isabs(path):
+    elif not os.path.isabs(path):
         return os.path.join(os.path.dirname(context.config["path"]), path)
     else:
         return path
 
 
-def _parse_args(workflow_config: WorkflowConfig, context: StreamFlowContext):
+def _parse_args(
+    workflow_config: WorkflowConfig,
+    context: StreamFlowContext,
+):
     cwl_config = workflow_config.config
     cwl_config["file"] = _parse_arg(cwl_config["file"], context)
     args = [cwl_config["file"]]
     if "settings" in cwl_config:
         cwl_config["settings"] = _parse_arg(cwl_config["settings"], context)
         args.append(cwl_config["settings"])
+    for entry in cwl_config.get("docker", []):
+        path = PurePosixPath(entry["step"])
+        workflow_config.put(
+            path,
+            "docker",
+            CWLDockerTranslatorConfig(
+                name=str(path),
+                type=entry["deployment"]["type"],
+                config=entry["deployment"].get("config", {}),
+                wrapper=entry["deployment"].get("wrapper", True),
+            ),
+        )
     return args
 
 
 async def main(
     workflow_config: WorkflowConfig,
     context: StreamFlowContext,
     args: argparse.Namespace,
```

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/processor.py` & `streamflow-0.2.0.dev4/streamflow/cwl/processor.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/runner.py` & `streamflow-0.2.0.dev4/streamflow/cwl/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,17 +71,17 @@
             raise WorkflowDefinitionException(
                 "A StreamFlow file must contain only one workflow definition when used with cwl-runner."
             )
     else:
         workflow_name = "cwl-workflow"
         streamflow_config = {"version": "v1.0", "workflows": {workflow_name: {}}}
     streamflow_config["workflows"][workflow_name]["type"] = "cwl"
-    streamflow_config["workflows"][workflow_name]["config"] = {
-        "file": os.path.abspath(args.processfile)
-    }
+    streamflow_config["workflows"][workflow_name].setdefault("config", {}).update(
+        {"file": os.path.abspath(args.processfile)}
+    )
     if args.jobfile:
         streamflow_config["workflows"][workflow_name]["config"][
             "settings"
         ] = os.path.abspath(args.jobfile)
     validator.validate(streamflow_config)
     streamflow_config["path"] = (
         args.streamflow_file if args.streamflow_file is not None else os.getcwd()
```

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/step.py` & `streamflow-0.2.0.dev4/streamflow/cwl/step.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/token.py` & `streamflow-0.2.0.dev4/streamflow/cwl/token.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/transformer.py` & `streamflow-0.2.0.dev4/streamflow/cwl/transformer.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/translator.py` & `streamflow-0.2.0.dev4/streamflow/cwl/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import copy
 import logging
 import os
 import posixpath
-import tempfile
 import urllib.parse
 from enum import Enum
 from pathlib import PurePosixPath
 from types import ModuleType
 from typing import (
     Any,
     MutableMapping,
@@ -31,15 +30,14 @@
     DeploymentConfig,
     LOCAL_LOCATION,
     LocalTarget,
     Location,
     Target,
 )
 from streamflow.core.exception import WorkflowDefinitionException
-from streamflow.core.utils import random_name
 from streamflow.core.workflow import (
     CommandOutputProcessor,
     Port,
     Step,
     Token,
     TokenProcessor,
     Workflow,
@@ -61,14 +59,19 @@
     CWLMapTokenProcessor,
     CWLObjectCommandOutputProcessor,
     CWLObjectTokenProcessor,
     CWLTokenProcessor,
     CWLUnionCommandOutputProcessor,
     CWLUnionTokenProcessor,
 )
+from streamflow.cwl.requirement.docker import cwl_docker_translator_classes
+from streamflow.cwl.requirement.docker.translator import (
+    CWLDockerTranslator,
+    CWLDockerTranslatorConfig,
+)
 from streamflow.cwl.step import (
     CWLConditionalStep,
     CWLEmptyScatterConditionalStep,
     CWLInputInjectorStep,
     CWLLoopConditionalStep,
     CWLLoopOutputAllStep,
     CWLLoopOutputLastStep,
@@ -1059,47 +1062,47 @@
         image_name = docker_requirement["dockerPull"]
     elif "dockerImageId" in docker_requirement:
         image_name = docker_requirement["dockerImageId"]
     else:
         raise WorkflowDefinitionException(
             "DockerRequirements without `dockerPull` or `dockerImageId` are not supported yet"
         )
-    return image_name
+    return str(image_name)
 
 
 def _process_docker_requirement(
-    name: str,
-    target: Target,
+    config_dir: str,
+    config: CWLDockerTranslatorConfig,
     context: MutableMapping[str, Any],
     docker_requirement: MutableMapping[str, Any],
     network_access: bool,
+    target: Target,
 ) -> Target:
-    image_name = _process_docker_image(docker_requirement=docker_requirement)
-    # Build configuration
-    docker_config = {
-        "image": image_name,
-        "logDriver": "none",
-        "network": "default" if network_access else "none",
-        "volume": [f"{target.workdir}:/tmp/streamflow"],
-    }
-    # Manage dockerOutputDirectory directive
+    # Process output directory
     if "dockerOutputDirectory" in docker_requirement:
-        docker_config["workdir"] = docker_requirement["dockerOutputDirectory"]
-        context["output_directory"] = docker_config["workdir"]
-        local_dir = os.path.join(
-            os.path.realpath(tempfile.gettempdir()), "streamflow", random_name()
-        )
-        os.makedirs(local_dir, exist_ok=True)
-        docker_config["volume"].append(f"{local_dir}:{docker_config['workdir']}")
-    # Build step target
-    deployment = DeploymentConfig(name=name, type="docker", config=docker_config)
-    step_target = Target(
-        deployment=deployment, service=image_name, workdir="/tmp/streamflow"  # nosec
+        output_directory = docker_requirement["dockerOutputDirectory"]
+        context["output_directory"] = output_directory
+    else:
+        output_directory = None
+    # Build CWLDockerTranslator
+    if config.type not in cwl_docker_translator_classes:
+        raise WorkflowDefinitionException(
+            f"Container type `{config.type}` not supported"
+        )
+    translator_type = cwl_docker_translator_classes[config.type]
+    translator = cast(
+        CWLDockerTranslator,
+        translator_type(config_dir=config_dir, wrapper=config.wrapper, **config.config),
+    )
+    return translator.get_target(
+        image=_process_docker_image(docker_requirement=docker_requirement),
+        output_directory=output_directory,
+        network_access=network_access,
+        target=target,
     )
-    return step_target
 
 
 def _process_input_value(
     path_processor: ModuleType, output_directory: str, target: Target, value: Any
 ) -> Any:
     if isinstance(value, MutableSequence):
         return [
@@ -1501,37 +1504,43 @@
         # Process DockerRequirement
         if "DockerRequirement" in requirements:
             network_access = (
                 requirements["NetworkAccess"]["networkAccess"]
                 if "NetworkAccess" in requirements
                 else False
             )
-            if (
-                len(binding_config.targets) == 1
-                and binding_config.targets[0].deployment.name == LOCAL_LOCATION
-            ):
-                binding_config.targets[0] = _process_docker_requirement(
-                    name=posixpath.join(name_prefix, "docker-requirement"),
-                    target=binding_config.targets[0],
-                    context=context,
-                    docker_requirement=requirements["DockerRequirement"],
-                    network_access=network_access,
-                )
-            else:
-                for target in binding_config.targets:
-                    if (
-                        target.deployment.type == "docker"
-                        and "image" in target.deployment.config
-                        and target.deployment.config["image"] == ""
-                    ):
-                        # Overwrite image configuration
-                        image_name = _process_docker_image(
-                            docker_requirement=requirements["DockerRequirement"]
+            targets = []
+            for target in binding_config.targets:
+                # If original target is local, use a container
+                if target.deployment.type == "local":
+                    targets.append(
+                        _process_docker_requirement(
+                            config_dir=os.path.dirname(self.context.config["path"]),
+                            config=self.workflow_config.get(
+                                path=PurePosixPath(name_prefix),
+                                name="docker",
+                                default=CWLDockerTranslatorConfig(
+                                    name="default", type="default", config={}
+                                ),
+                            ),
+                            context=context,
+                            docker_requirement=requirements["DockerRequirement"],
+                            network_access=network_access,
+                            target=target,
+                        )
+                    )
+                # Otherwise, throw a warning and skip the DockerRequirement conversion
+                else:
+                    if logger.isEnabledFor(logging.WARN):
+                        logger.warn(
+                            f"Skipping DockerRequirement conversion for step `{name_prefix}` "
+                            f"when executing on `{target.deployment.name}` deployment."
                         )
-                        target.deployment.config["image"] = image_name
+                    targets.append(target)
+            binding_config.targets = targets
         # Create DeploySteps to initialise the execution environment
         deployments = {t.deployment.name: t.deployment for t in binding_config.targets}
         deploy_steps = {
             name: self._get_deploy_step(deployment, workflow)
             for name, deployment in deployments.items()
         }
         # Create a schedule step and connect it to the DeployStep
```

### Comparing `streamflow-0.2.0.dev3/streamflow/cwl/utils.py` & `streamflow-0.2.0.dev4/streamflow/cwl/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
                     context=context,
                     connector=connector,
                     path=real_path,
                     relpath=path_processor.basename(real_path),
                 ):
                     data_location = data_locations[0]
                 else:
-                    raise WorkflowExecutionException(f"Error registering path {path}")
+                    return None
             link_location = context.data_manager.register_path(
                 location=location,
                 path=path,
                 relpath=relpath,
                 data_type=DataType.SYMBOLIC_LINK,
             )
             context.data_manager.register_relation(data_location, link_location)
```

### Comparing `streamflow-0.2.0.dev3/streamflow/data/data_manager.py` & `streamflow-0.2.0.dev4/streamflow/data/data_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/data/remotepath.py` & `streamflow-0.2.0.dev4/streamflow/data/remotepath.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,17 +421,20 @@
         return int(result) if result.isdigit() else 0
 
 
 async def symlink(
     connector: Connector, location: Location | None, src: str, path: str
 ) -> None:
     if isinstance(connector, LocalConnector):
+        src = os.path.abspath(src)
+        if os.path.isdir(path):
+            path = os.path.join(path, os.path.basename(src))
         try:
             os.symlink(
-                os.path.abspath(src), path, target_is_directory=os.path.isdir(path)
+                os.path.abspath(src), path, target_is_directory=os.path.isdir(src)
             )
         except OSError as e:
             if not e.errno == errno.EEXIST:
                 raise
     else:
         await connector.run(location=location, command=["ln", "-snf", src, path])
```

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/aiotarstream.py` & `streamflow-0.2.0.dev4/streamflow/deployment/aiotarstream.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/__init__.py` & `streamflow-0.2.0.dev4/streamflow/deployment/connector/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from streamflow.deployment.connector.container import (
     DockerComposeConnector,
     DockerConnector,
     SingularityConnector,
 )
-from streamflow.deployment.connector.kubernetes import Helm3Connector
+from streamflow.deployment.connector.kubernetes import (
+    Helm3Connector,
+    KubernetesConnector,
+)
 from streamflow.deployment.connector.local import LocalConnector
 from streamflow.deployment.connector.occam import OccamConnector
-from streamflow.deployment.connector.queue_manager import PBSConnector, SlurmConnector
+from streamflow.deployment.connector.queue_manager import (
+    PBSConnector,
+    SlurmConnector,
+    FluxConnector,
+)
 from streamflow.deployment.connector.ssh import SSHConnector
 
 connector_classes = {
     "docker": DockerConnector,
     "docker-compose": DockerComposeConnector,
+    "flux": FluxConnector,
     "helm": Helm3Connector,
     "helm3": Helm3Connector,
+    "kubernetes": KubernetesConnector,
     "local": LocalConnector,
     "occam": OccamConnector,
     "pbs": PBSConnector,
     "singularity": SingularityConnector,
     "slurm": SlurmConnector,
     "ssh": SSHConnector,
 }
```

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/base.py` & `streamflow-0.2.0.dev4/streamflow/deployment/connector/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import asyncio
 import logging
 import os
 import posixpath
 import shlex
 import tarfile
 from abc import ABCMeta, abstractmethod
-from pathlib import Path
 from typing import MutableSequence, TYPE_CHECKING
 
 from streamflow.core import utils
 from streamflow.core.data import StreamWrapperContext
 from streamflow.core.deployment import (
     Connector,
     ConnectorCopyKind,
     LOCAL_LOCATION,
     Location,
 )
 from streamflow.core.exception import WorkflowExecutionException
+from streamflow.core.utils import get_local_to_remote_destination
 from streamflow.deployment import aiotarstream
 from streamflow.deployment.future import FutureConnector
 from streamflow.deployment.stream import (
     StreamReaderWrapper,
     StreamWriterWrapper,
     SubprocessStreamReaderWrapperContext,
 )
@@ -35,32 +35,29 @@
 async def extract_tar_stream(
     tar: aiotarstream.AioTarStream,
     src: str,
     dst: str,
     transferBufferSize: int | None = None,
 ) -> None:
     async for member in tar:
-        if os.path.isdir(dst):
-            if posixpath.join("/", member.path) == src:
-                member.path = posixpath.basename(member.path)
-                await tar.extract(member, dst)
-                if member.isdir():
-                    dst = os.path.join(dst, member.path)
-            else:
-                member.path = posixpath.relpath(posixpath.join("/", member.path), src)
-                await tar.extract(member, dst)
+        if os.path.isdir(dst) and member.path == posixpath.basename(src):
+            await tar.extract(member, dst)
         elif member.isfile():
             async with await tar.extractfile(member) as inputfile:
-                with open(dst, "wb") as outputfile:
+                path = os.path.normpath(
+                    os.path.join(
+                        dst, posixpath.relpath(member.path, posixpath.basename(src))
+                    )
+                )
+                with open(path, "wb") as outputfile:
                     while content := await inputfile.read(transferBufferSize):
                         outputfile.write(content)
         else:
-            parent_dir = str(Path(dst).parent)
-            member.path = posixpath.basename(member.path)
-            await tar.extract(member, parent_dir)
+            member.path = posixpath.relpath(member.path, posixpath.basename(src))
+            await tar.extract(member, os.path.normpath(os.path.join(dst, member.path)))
 
 
 class FutureMeta(ABCMeta):
     def __instancecheck__(cls, instance):
         if isinstance(instance, FutureConnector):
             return super().__subclasscheck__(instance.type)
         else:
@@ -98,14 +95,15 @@
     async def _copy_local_to_remote(
         self,
         src: str,
         dst: str,
         locations: MutableSequence[Location],
         read_only: bool = False,
     ) -> None:
+        dst = await get_local_to_remote_destination(self, locations[0], src, dst)
         await asyncio.gather(
             *(
                 asyncio.create_task(
                     self._copy_local_to_remote_single(
                         src=src, dst=dst, location=location, read_only=read_only
                     )
                 )
@@ -142,22 +140,23 @@
         finally:
             proc.stdin.close()
             await proc.wait()
 
     async def _copy_remote_to_local(
         self, src: str, dst: str, location: Location, read_only: bool = False
     ) -> None:
+        dirname, basename = posixpath.split(src)
         proc = await asyncio.create_subprocess_exec(
             *shlex.split(
                 self._get_run_command(
-                    command="tar chf - -C / " + posixpath.relpath(src, "/"),
+                    command=f"tar chf - -C {dirname} {basename}",
                     location=location,
                 )
             ),
-            stdin=None,
+            stdin=asyncio.subprocess.DEVNULL,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
         )
         try:
             async with aiotarstream.open(
                 stream=StreamReaderWrapper(proc.stdout),
                 mode="r",
@@ -258,15 +257,15 @@
             coro=asyncio.create_subprocess_exec(
                 *shlex.split(
                     self._get_run_command(
                         command=f"tar chf - -C {dirname} {basename}",
                         location=location,
                     )
                 ),
-                stdin=None,
+                stdin=asyncio.subprocess.DEVNULL,
                 stdout=asyncio.subprocess.PIPE,
                 stderr=asyncio.subprocess.PIPE,
             )
         )
 
     async def copy(
         self,
@@ -373,20 +372,24 @@
                 )
             )
         command = utils.encode_command(command, self._get_shell())
         run_command = self._get_run_command(command, location)
         proc = await asyncio.create_subprocess_exec(
             *shlex.split(run_command),
             stdin=None,
-            stdout=asyncio.subprocess.PIPE
-            if capture_output
-            else asyncio.subprocess.DEVNULL,
-            stderr=asyncio.subprocess.PIPE
-            if capture_output
-            else asyncio.subprocess.DEVNULL,
+            stdout=(
+                asyncio.subprocess.PIPE
+                if capture_output
+                else asyncio.subprocess.DEVNULL
+            ),
+            stderr=(
+                asyncio.subprocess.PIPE
+                if capture_output
+                else asyncio.subprocess.DEVNULL
+            ),
         )
         if capture_output:
             stdout, _ = await asyncio.wait_for(proc.communicate(), timeout=timeout)
             return stdout.decode().strip(), proc.returncode
         else:
             await asyncio.wait_for(proc.wait(), timeout=timeout)
             return None
```

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/container.py` & `streamflow-0.2.0.dev4/streamflow/deployment/connector/container.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,43 +3,107 @@
 import asyncio
 import json
 import logging
 import os
 import posixpath
 import shlex
 from abc import ABC, abstractmethod
+from shutil import which
 from typing import Any, MutableMapping, MutableSequence
 
 import pkg_resources
 from cachetools import Cache, TTLCache
 
 from streamflow.core import utils
 from streamflow.core.asyncache import cachedmethod
 from streamflow.core.deployment import Connector, Location
 from streamflow.core.exception import WorkflowExecutionException
 from streamflow.core.scheduling import AvailableLocation
+from streamflow.core.utils import get_local_to_remote_destination
 from streamflow.deployment.connector.base import BaseConnector
 from streamflow.log_handler import logger
 
 
+def _check_docker_compose_installed():
+    if which("docker-compose") is None:
+        raise WorkflowExecutionException(
+            "Docker Compose must be installed on the system to use the Docker Compose connector."
+        )
+
+
+def _check_docker_installed(connector):
+    if which("docker") is None:
+        raise WorkflowExecutionException(
+            f"Docker must be installed on the system to use the {connector} connector."
+        )
+
+
+def _check_singularity_installed():
+    if which("singularity") is None:
+        raise WorkflowExecutionException(
+            "Singularity must be installed on the system to use the Singularity connector."
+        )
+
+
 async def _exists_docker_image(image_name: str) -> bool:
-    exists_command = "".join(["docker ", "image ", "inspect ", image_name])
     proc = await asyncio.create_subprocess_exec(
-        *shlex.split(exists_command),
+        *shlex.split(f"docker image inspect {image_name}"),
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
     )
     await proc.wait()
     return proc.returncode == 0
 
 
+async def _get_docker_compose_version() -> str:
+    proc = await asyncio.create_subprocess_exec(
+        *shlex.split("docker-compose version --short"),
+        stdout=asyncio.subprocess.PIPE,
+        stderr=asyncio.subprocess.DEVNULL,
+    )
+    stdout, _ = await proc.communicate()
+    return stdout.decode().strip()
+
+
+async def _get_docker_version() -> str:
+    proc = await asyncio.create_subprocess_exec(
+        *shlex.split("docker version --format '{{.Client.Version}}'"),
+        stdout=asyncio.subprocess.PIPE,
+        stderr=asyncio.subprocess.DEVNULL,
+    )
+    stdout, _ = await proc.communicate()
+    return stdout.decode().strip()
+
+
+async def _get_singularity_version() -> str:
+    proc = await asyncio.create_subprocess_exec(
+        *shlex.split("singularity --version"),
+        stdout=asyncio.subprocess.PIPE,
+        stderr=asyncio.subprocess.DEVNULL,
+    )
+    stdout, _ = await proc.communicate()
+    return stdout.decode().strip()
+
+
+def _prepare_volumes(binds: MutableSequence[str], mounts: MutableSequence[str]):
+    for b in binds or []:
+        src, dst = b.split(":", 2)
+        if not os.path.exists(src):
+            os.makedirs(src)
+    for m in mounts or []:
+        mount_type = next(part[5:] for part in m.split(",") if part.startswith("type="))
+        if mount_type == "bind":
+            src = next(part[4:] for part in m.split(",") if part.startswith("src="))
+            if not os.path.exists(src):
+                os.makedirs(src)
+
+
 async def _pull_docker_image(image_name: str) -> None:
-    exists_command = "".join(["docker ", "pull ", "--quiet ", image_name])
     proc = await asyncio.create_subprocess_exec(
-        *shlex.split(exists_command),
+        *shlex.split(f"docker pull --quiet {image_name}"),
         stdout=asyncio.subprocess.DEVNULL,
         stderr=asyncio.subprocess.DEVNULL,
     )
     await proc.wait()
 
 
 class ContainerConnector(BaseConnector, ABC):
@@ -83,15 +147,15 @@
         common_paths: MutableMapping[str, Any],
         effective_locations: MutableSequence[Location],
         location: Location,
         path: str,
         source_location: Location | None = None,
     ) -> tuple[MutableMapping[str, Any], MutableSequence[Location]]:
         # Get all container mounts
-        volumes = await self._get_volumes(location.name)
+        volumes = await self._get_volumes(location)
         for volume in volumes:
             # If path is in a persistent volume
             if path.startswith(volume["Destination"]):
                 if path not in common_paths:
                     common_paths[path] = []
                 # Check if path is shared with another location that has been already processed
                 for i, common_path in enumerate(common_paths[path]):
@@ -119,18 +183,19 @@
     async def _copy_local_to_remote(
         self,
         src: str,
         dst: str,
         locations: MutableSequence[Location],
         read_only: bool = False,
     ) -> None:
+        dst = await get_local_to_remote_destination(self, locations[0], src, dst)
         effective_locations = await self._get_effective_locations(locations, dst)
         copy_tasks = []
         for location in effective_locations:
-            if read_only and await self._is_bind_transfer(location.name, src, dst):
+            if read_only and await self._is_bind_transfer(location, src, dst):
                 copy_tasks.append(
                     asyncio.create_task(
                         self.run(
                             location=location,
                             command=["ln", "-snf", posixpath.abspath(src), dst],
                         )
                     )
@@ -158,18 +223,18 @@
         effective_locations = await self._get_effective_locations(
             locations, dst, source_location
         )
         non_bind_locations = []
         if (
             read_only
             and source_connector == self
-            and await self._is_bind_transfer(source_location.name, src, src)
+            and await self._is_bind_transfer(source_location, src, src)
         ):
             for location in effective_locations:
-                if await self._is_bind_transfer(location.name, dst, dst):
+                if await self._is_bind_transfer(location, dst, dst):
                     await self.run(
                         location=location,
                         command=["ln", "-snf", posixpath.abspath(src), dst],
                     )
                     continue
                 non_bind_locations.append(location)
             await super()._copy_remote_to_remote(
@@ -202,45 +267,45 @@
             common_paths, effective_locations = await self._check_effective_location(
                 common_paths, effective_locations, location, dest_path, source_location
             )
         return effective_locations
 
     @abstractmethod
     async def _get_bind_mounts(
-        self, location: str
+        self, location: Location
     ) -> MutableSequence[MutableMapping[str, str]]:
         ...
 
     @abstractmethod
     async def _get_location(self, location_name: str) -> AvailableLocation | None:
         ...
 
     @abstractmethod
     async def _get_volumes(
-        self, location: str
+        self, location: Location
     ) -> MutableSequence[MutableMapping[str, str]]:
         ...
 
     async def _is_bind_transfer(
-        self, location: str, host_path: str, instance_path: str
+        self, location: Location, host_path: str, instance_path: str
     ) -> bool:
         bind_mounts = await self._get_bind_mounts(location)
         host_binds = [b["Source"] for b in bind_mounts]
         instance_binds = [b["Destination"] for b in bind_mounts]
         for host_bind in host_binds:
             if host_path.startswith(host_bind):
                 for instance_bind in instance_binds:
                     if instance_path.startswith(instance_bind):
                         return True
         return False
 
 
 class DockerBaseConnector(ContainerConnector, ABC):
     async def _get_bind_mounts(
-        self, location: str
+        self, location: Location
     ) -> MutableSequence[MutableMapping[str, str]]:
         return [v for v in await self._get_volumes(location) if v["Type"] == "bind"]
 
     async def _get_location(self, location_name: str) -> AvailableLocation:
         inspect_command = "".join(
             [
                 "docker ",
@@ -261,28 +326,21 @@
             deployment=self.deployment_name,
             hostname=stdout.decode().strip(),
         )
 
     def _get_run_command(
         self, command: str, location: Location, interactive: bool = False
     ):
-        return "".join(
-            [
-                "docker ",
-                "exec {}".format("-i " if interactive else ""),
-                f"{location.name} ",
-                f"sh -c '{command}'",
-            ]
-        )
+        return f"docker exec {'-i' if interactive else ''} {location.name} sh -c '{command}'"
 
     async def _get_volumes(
-        self, location: str
+        self, location: Location
     ) -> MutableSequence[MutableMapping[str, str]]:
         inspect_command = "".join(
-            ["docker ", "inspect ", "--format ", "'{{json .Mounts}}' ", location]
+            ["docker ", "inspect ", "--format ", "'{{json .Mounts}}' ", location.name]
         )
         proc = await asyncio.create_subprocess_exec(
             *shlex.split(inspect_command),
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
         )
         stdout, _ = await proc.communicate()
@@ -343,16 +401,16 @@
         ipc: str | None = None,
         isolation: str | None = None,
         kernelMemory: int | None = None,
         label: MutableSequence[str] | None = None,
         labelFile: MutableSequence[str] | None = None,
         link: MutableSequence[str] | None = None,
         linkLocalIP: MutableSequence[str] | None = None,
-        locationsCacheSize: int = None,
-        locationsCacheTTL: int = None,
+        locationsCacheSize: int | None = None,
+        locationsCacheTTL: int | None = None,
         logDriver: str | None = None,
         logOpts: MutableSequence[str] | None = None,
         macAddress: str | None = None,
         memory: int | None = None,
         memoryReservation: int | None = None,
         memorySwap: int | None = None,
         memorySwappiness: int | None = None,
@@ -365,16 +423,16 @@
         pid: str | None = None,
         pidsLimit: int | None = None,
         privileged: bool = False,
         publish: MutableSequence[str] | None = None,
         publishAll: bool = False,
         readOnly: bool = False,
         replicas: int = 1,
-        resourcesCacheSize: int = None,
-        resourcesCacheTTL: int = None,
+        resourcesCacheSize: int | None = None,
+        resourcesCacheTTL: int | None = None,
         restart: str | None = None,
         rm: bool = True,
         runtime: str | None = None,
         securityOpts: MutableSequence[str] | None = None,
         shmSize: int | None = None,
         sigProxy: bool = True,
         stopSignal: str | None = None,
@@ -492,14 +550,18 @@
         self.volume: MutableSequence[str] | None = volume
         self.volumeDriver: str | None = volumeDriver
         self.volumesFrom: MutableSequence[str] | None = volumesFrom
         self.workdir: str | None = workdir
 
     async def deploy(self, external: bool) -> None:
         if not external:
+            _prepare_volumes(self.volume, self.mount)
+            _check_docker_installed("Docker")
+            if logger.isEnabledFor(logging.DEBUG):
+                logger.debug(f"Using Docker {await _get_docker_version()}.")
             # Pull image if it doesn't exist
             if not await _exists_docker_image(self.image):
                 await _pull_docker_image(self.image)
             # Deploy the Docker container
             for _ in range(0, self.replicas):
                 deploy_command = "".join(
                     [
@@ -719,15 +781,15 @@
         self.timeout = timeout
         self.tls = tls
         self.tlscacert = tlscacert
         self.tlscert = tlscert
         self.tlskey = tlskey
         self.tlsverify = tlsverify
 
-    def base_command(self) -> str:
+    def _get_base_command(self) -> str:
         return "".join(
             [
                 "docker-compose ",
                 self.get_option("file", self.files),
                 self.get_option("project-name", self.projectName),
                 self.get_option("verbose", self.verbose),
                 self.get_option("log-level", self.logLevel),
@@ -742,178 +804,178 @@
                 self.get_option("project-directory", self.projectDirectory),
                 self.get_option("compatibility", self.compatibility),
             ]
         )
 
     async def deploy(self, external: bool) -> None:
         if not external:
-            deploy_command = self.base_command() + "".join(
+            _check_docker_installed("Docker Compose")
+            version = await _get_docker_compose_version()
+            if version.startswith("v"):
+                version = version[1:]
+            major = int(version.split(".")[0])
+            if not major >= 2:
+                raise WorkflowExecutionException(
+                    f"Docker Compose {version} is not compatible with DockerComposeConnector. "
+                    f"Docker Compose version 2.x or later is required."
+                )
+            if logger.isEnabledFor(logging.DEBUG):
+                logger.debug(
+                    f"Using Docker {await _get_docker_version()} "
+                    f"and Docker Compose {version}."
+                )
+            deploy_command = self._get_base_command() + "".join(
                 [
                     "up ",
                     "--detach ",
                     self.get_option("no-deps ", self.noDeps),
                     self.get_option("force-recreate", self.forceRecreate),
                     self.get_option("always-recreate-deps", self.alwaysRecreateDeps),
                     self.get_option("no-recreate", self.noRecreate),
                     self.get_option("no-build", self.noBuild),
                     self.get_option("no-start", self.noStart),
                 ]
             )
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(f"EXECUTING command {deploy_command}")
-            proc = await asyncio.create_subprocess_exec(*shlex.split(deploy_command))
-            await proc.wait()
+            proc = await asyncio.create_subprocess_exec(
+                *shlex.split(deploy_command),
+                stderr=asyncio.subprocess.STDOUT,
+                stdout=asyncio.subprocess.PIPE,
+            )
+            stdout, _ = await proc.communicate()
+            if proc.returncode != 0:
+                raise WorkflowExecutionException(
+                    f"FAILED Deployment of {self.deployment_name} environment:\n\t{stdout.decode().strip()}"
+                )
 
     @cachedmethod(lambda self: self.locationsCache)
     async def get_available_locations(
         self,
         service: str | None = None,
         input_directory: str | None = None,
         output_directory: str | None = None,
         tmp_directory: str | None = None,
     ) -> MutableMapping[str, AvailableLocation]:
-        ps_command = self.base_command() + "".join(["ps ", service or ""])
+        ps_command = self._get_base_command() + "".join(
+            ["ps ", "--format ", "json ", service or ""]
+        )
         if logger.isEnabledFor(logging.DEBUG):
             logger.debug(f"EXECUTING command {ps_command}")
         proc = await asyncio.create_subprocess_exec(
             *shlex.split(ps_command),
             stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
+            stderr=asyncio.subprocess.STDOUT,
         )
         stdout, _ = await proc.communicate()
-        lines = (line for line in stdout.decode().strip().split("\n"))
-        locations = {}
-        for line in lines:
-            if line.startswith("---------"):
-                break
-        for line in lines:
-            location_name = line.split()[0].strip()
-            locations[location_name] = await self._get_location(location_name)
-        return locations
+        locations = json.loads(stdout.decode().strip())
+        return {
+            loc["Name"]: v
+            for loc, v in zip(
+                locations,
+                await asyncio.gather(
+                    *(
+                        asyncio.create_task(self._get_location(location["Name"]))
+                        for location in locations
+                    )
+                ),
+            )
+        }
 
     @classmethod
     def get_schema(cls) -> str:
         return pkg_resources.resource_filename(
             __name__, os.path.join("schemas", "docker-compose.json")
         )
 
     async def undeploy(self, external: bool) -> None:
         if not external:
             undeploy_command = (
-                self.base_command()
+                self._get_base_command()
                 + f"down {self.get_option('volumes', self.removeVolumes)}"
             )
             if logger.isEnabledFor(logging.DEBUG):
                 logger.debug(f"EXECUTING command {undeploy_command}")
-            proc = await asyncio.create_subprocess_exec(*shlex.split(undeploy_command))
-            await proc.wait()
-
-
-class SingularityBaseConnector(ContainerConnector, ABC):
-    async def _get_bind_mounts(
-        self, location: Location
-    ) -> MutableSequence[MutableMapping[str, str]]:
-        return await self._get_volumes(location)
-
-    async def _get_location(self, location_name: str) -> AvailableLocation | None:
-        inspect_command = "singularity instance list --json"
-        proc = await asyncio.create_subprocess_exec(
-            *shlex.split(inspect_command),
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
-        )
-        stdout, _ = await proc.communicate()
-        if stdout:
-            json_out = json.loads(stdout)
-            for instance in json_out["instances"]:
-                if instance["instance"] == location_name:
-                    return AvailableLocation(
-                        name=location_name,
-                        deployment=self.deployment_name,
-                        hostname=instance["ip"],
-                    )
-        return None
-
-    def _get_run_command(
-        self, command: str, location: Location, interactive: bool = False
-    ):
-        return "".join(
-            [
-                "singularity ",
-                "exec ",
-                "instance://",
-                location.name,
-                f" sh -c '{command}'",
-            ]
-        )
-
-    async def _get_volumes(
-        self, location: Location
-    ) -> MutableSequence[MutableMapping[str, str]]:
-        bind_mounts, _ = await self.run(
-            location=location,
-            command=["cat", "/proc/1/mountinfo", "|", "awk", "'{print $9,$4,$5}'"],
-            capture_output=True,
-        )
-        # Exclude `overlay` and `tmpfs` mounts
-        return [
-            {"Source": line.split()[1], "Destination": line.split()[2]}
-            for line in bind_mounts.splitlines()
-            if line.split()[0] not in ["tmpfs", "overlay"]
-        ]
+            proc = await asyncio.create_subprocess_exec(
+                *shlex.split(undeploy_command),
+                stderr=asyncio.subprocess.STDOUT,
+                stdout=asyncio.subprocess.PIPE,
+            )
+            stdout, _ = await proc.communicate()
+            if proc.returncode != 0:
+                raise WorkflowExecutionException(
+                    f"FAILED Undeployment of {self.deployment_name} environment:\n\t{stdout.decode().strip()}"
+                )
 
 
-class SingularityConnector(SingularityBaseConnector):
+class SingularityConnector(ContainerConnector):
     def __init__(
         self,
         deployment_name: str,
         config_dir: str,
         image: str,
-        transferBufferSize: int = 2**16,
         addCaps: str | None = None,
         allowSetuid: bool = False,
         applyCgroups: str | None = None,
         bind: MutableSequence[str] | None = None,
+        blkioWeight: int | None = None,
+        blkioWeightDevice: MutableSequence[str] | None = None,
         boot: bool = False,
         cleanenv: bool = False,
         command: MutableSequence[str] | None = None,
+        compat: bool = False,
         contain: bool = False,
         containall: bool = False,
+        cpuShares: int | None = None,
+        cpus: str | None = None,
+        cpusetCpus: str | None = None,
+        cpusetMems: str | None = None,
         disableCache: bool = False,
         dns: str | None = None,
+        dockerHost: str | None = None,
         dropCaps: str | None = None,
         env: MutableSequence[str] | None = None,
         envFile: str | None = None,
         fakeroot: bool = False,
         fusemount: MutableSequence[str] | None = None,
         home: str | None = None,
         hostname: str | None = None,
         instanceNames: MutableSequence[str] | None = None,
+        ipc: bool = False,
         keepPrivs: bool = False,
         locationsCacheSize: int = None,
         locationsCacheTTL: int = None,
+        memory: str | None = None,
+        memoryReservation: str | None = None,
+        memorySwap: str | None = None,
+        mount: MutableSequence[str] | None = None,
         net: bool = False,
         network: str | None = None,
         networkArgs: MutableSequence[str] | None = None,
+        noEval: bool = False,
         noHome: bool = False,
+        noHttps: bool = False,
         noInit: bool = False,
         noMount: MutableSequence[str] | None = None,
         noPrivs: bool = False,
         noUmask: bool = False,
-        nohttps: bool = False,
         nv: bool = False,
+        nvccli: bool = False,
+        oomKillDisable: bool = False,
         overlay: MutableSequence[str] | None = None,
         pemPath: str | None = None,
         pidFile: str | None = None,
+        pidsLimit: int | None = None,
         replicas: int = 1,
         resourcesCacheSize: int = None,
         resourcesCacheTTL: int = None,
         rocm: bool = False,
         scratch: MutableSequence[str] | None = None,
         security: MutableSequence[str] | None = None,
+        transferBufferSize: int = 2**16,
         userns: bool = False,
         uts: bool = False,
         workdir: str | None = None,
         writable: bool = False,
         writableTmpfs: bool = False,
     ):
         super().__init__(
@@ -926,118 +988,200 @@
             resourcesCacheTTL=resourcesCacheTTL,
         )
         self.image: str = image
         self.addCaps: str | None = addCaps
         self.allowSetuid: bool = allowSetuid
         self.applyCgroups: str | None = applyCgroups
         self.bind: MutableSequence[str] | None = bind
+        self.blkioWeight: int | None = blkioWeight
+        self.blkioWeightDevice: MutableSequence[str] | None = blkioWeightDevice
         self.boot: bool = boot
         self.cleanenv: bool = cleanenv
         self.command: MutableSequence[str] = command or []
+        self.compat: bool = compat
         self.contain: bool = contain
         self.containall: bool = containall
+        self.cpuShares: int | None = cpuShares
+        self.cpus: str | None = cpus
+        self.cpusetCpus: str | None = cpusetCpus
+        self.cpusetMems: str | None = cpusetMems
         self.disableCache: bool = disableCache
         self.dns: str | None = dns
         self.dropCaps: str | None = dropCaps
+        self.dockerHost: str | None = dockerHost
         self.env: MutableSequence[str] | None = env
         self.envFile: str | None = envFile
         self.fakeroot: bool = fakeroot
         self.fusemount: MutableSequence[str] | None = fusemount
         self.home: str | None = home
         self.hostname: str | None = hostname
-        self.instanceNames: MutableSequence[str] = instanceNames or []
+        self.ipc: bool = ipc
+        self.instanceNames: MutableSequence[str] | None = instanceNames or []
         self.keepPrivs: bool = keepPrivs
+        self.memory: str | None = memory
+        self.memoryReservation: str | None = memoryReservation
+        self.memorySwap: str | None = memorySwap
+        self.mount: MutableSequence[str] | None = mount
         self.net: bool = net
         self.network: str | None = network
         self.networkArgs: MutableSequence[str] | None = networkArgs
+        self.noEval: bool = noEval
         self.noHome: bool = noHome
+        self.noHttps: bool = noHttps
         self.noInit: bool = noInit
         self.noMount: MutableSequence[str] | None = noMount or []
         self.noPrivs: bool = noPrivs
         self.noUmask: bool = noUmask
-        self.nohttps: bool = nohttps
         self.nv: bool = nv
+        self.nvccli: bool = nvccli
+        self.oomKillDisable: bool = oomKillDisable
         self.overlay: MutableSequence[str] | None = overlay
         self.pemPath: str | None = pemPath
         self.pidFile: str | None = pidFile
+        self.pidsLimit: int | None = pidsLimit
         self.replicas: int = replicas
         self.rocm: bool = rocm
         self.scratch: MutableSequence[str] | None = scratch
         self.security: MutableSequence[str] | None = security
         self.userns: bool = userns
         self.uts: bool = uts
         self.workdir: str | None = workdir
         self.writable: bool = writable
         self.writableTmpfs: bool = writableTmpfs
 
+    async def _get_bind_mounts(
+        self, location: Location
+    ) -> MutableSequence[MutableMapping[str, str]]:
+        return await self._get_volumes(location)
+
+    async def _get_location(self, location_name: str) -> AvailableLocation | None:
+        inspect_command = "singularity instance list --json"
+        proc = await asyncio.create_subprocess_exec(
+            *shlex.split(inspect_command),
+            stdout=asyncio.subprocess.PIPE,
+            stderr=asyncio.subprocess.PIPE,
+        )
+        stdout, _ = await proc.communicate()
+        if stdout:
+            json_out = json.loads(stdout)
+            for instance in json_out["instances"]:
+                if instance["instance"] == location_name:
+                    return AvailableLocation(
+                        name=location_name,
+                        deployment=self.deployment_name,
+                        hostname=instance["ip"],
+                    )
+        return None
+
+    async def _get_volumes(
+        self, location: Location
+    ) -> MutableSequence[MutableMapping[str, str]]:
+        bind_mounts, _ = await self.run(
+            location=location,
+            command=["cat", "/proc/1/mountinfo", "|", "awk", "'{print $9,$4,$5}'"],
+            capture_output=True,
+        )
+        # Exclude `overlay` and `tmpfs` mounts
+        return [
+            {
+                "Source": line.split()[2]
+                if line.split()[1] == "/"
+                else line.split()[1],
+                "Destination": line.split()[2],
+            }
+            for line in bind_mounts.splitlines()
+            if line.split()[0] not in ["tmpfs", "overlay"]
+        ]
+
+    def _get_run_command(
+        self, command: str, location: Location, interactive: bool = False
+    ):
+        return f"singularity exec instance://{location.name} sh -c '{command}'"
+
     async def deploy(self, external: bool) -> None:
         if not external:
+            _check_singularity_installed()
+            if logger.isEnabledFor(logging.DEBUG):
+                logger.debug(f"Using {await _get_singularity_version()}.")
+            _prepare_volumes(self.bind, self.mount)
             for _ in range(0, self.replicas):
                 instance_name = utils.random_name()
-                deploy_command = "".join(
-                    [
-                        "singularity ",
-                        "instance ",
-                        "start ",
-                        self.get_option("add-caps", self.addCaps),
-                        self.get_option("allow-setuid", self.allowSetuid),
-                        self.get_option("apply-cgroups", self.applyCgroups),
-                        self.get_option("bind", self.bind),
-                        self.get_option("boot", self.boot),
-                        self.get_option("cleanenv", self.cleanenv),
-                        self.get_option("contain", self.contain),
-                        self.get_option("containall", self.containall),
-                        self.get_option("disable-cache", self.disableCache),
-                        self.get_option("dns", self.dns),
-                        self.get_option("drop-caps", self.dropCaps),
-                        self.get_option("env", self.env),
-                        self.get_option("env-file", self.envFile),
-                        self.get_option("fakeroot", self.fakeroot),
-                        self.get_option("fusemount", self.fusemount),
-                        self.get_option("home", self.home),
-                        self.get_option("hostname", self.hostname),
-                        self.get_option("keep-privs", self.keepPrivs),
-                        self.get_option("net", self.net),
-                        self.get_option("network", self.network),
-                        self.get_option("network-args", self.networkArgs),
-                        self.get_option("no-home", self.noHome),
-                        self.get_option("no-init", self.noInit),
-                        self.get_option("no-mount", self.noMount),
-                        self.get_option("no-privs", self.noPrivs),
-                        self.get_option("no-umask", self.noUmask),
-                        self.get_option("nohttps", self.nohttps),
-                        self.get_option("nv", self.nv),
-                        self.get_option("overlay", self.overlay),
-                        self.get_option("pem-path", self.pemPath),
-                        self.get_option("pid-file", self.pidFile),
-                        self.get_option("rocm", self.rocm),
-                        self.get_option("scratch", self.scratch),
-                        self.get_option("security", self.security),
-                        self.get_option("userns", self.userns),
-                        self.get_option("uts", self.uts),
-                        self.get_option("workdir", self.workdir),
-                        self.get_option("writable", self.writable),
-                        self.get_option("writable-tmpfs", self.writableTmpfs),
-                        f"{self.image} ",
-                        f"{instance_name} ",
-                        " ".join(self.command) if self.command else "",
-                    ]
+                deploy_command = (
+                    f"singularity instance start "
+                    f"{self.get_option('add-caps', self.addCaps)}"
+                    f"{self.get_option('allow-setuid', self.allowSetuid)}"
+                    f"{self.get_option('apply-cgroups', self.applyCgroups)}"
+                    f"{self.get_option('bind', self.bind)}"
+                    f"{self.get_option('blkio-weight', self.blkioWeight)}"
+                    f"{self.get_option('blkio-weight-device', self.blkioWeightDevice)}"
+                    f"{self.get_option('boot', self.boot)}"
+                    f"{self.get_option('cleanenv', self.cleanenv)}"
+                    f"{self.get_option('compat', self.compat)}"
+                    f"{self.get_option('contain', self.contain)}"
+                    f"{self.get_option('containall', self.containall)}"
+                    f"{self.get_option('cpu-shares', self.cpuShares)}"
+                    f"{self.get_option('cpus', self.cpus)}"
+                    f"{self.get_option('cpuset-cpus', self.cpusetCpus)}"
+                    f"{self.get_option('cpuset-mems', self.cpusetMems)}"
+                    f"{self.get_option('disable-cache', self.disableCache)}"
+                    f"{self.get_option('docker-host', self.dockerHost)}"
+                    f"{self.get_option('dns', self.dns)}"
+                    f"{self.get_option('drop-caps', self.dropCaps)}"
+                    f"{self.get_option('env-file', self.envFile)}"
+                    f"{self.get_option('fakeroot', self.fakeroot)}"
+                    f"{self.get_option('fusemount', self.fusemount)}"
+                    f"{self.get_option('home', self.home)}"
+                    f"{self.get_option('hostname', self.hostname)}"
+                    f"{self.get_option('ipc', self.ipc)}"
+                    f"{self.get_option('keep-privs', self.keepPrivs)}"
+                    f"{self.get_option('memory', self.memory)}"
+                    f"{self.get_option('memory-reservation', self.memoryReservation)}"
+                    f"{self.get_option('memory-swap', self.memorySwap)}"
+                    f"{self.get_option('mount', self.mount)}"
+                    f"{self.get_option('net', self.net)}"
+                    f"{self.get_option('network', self.network)}"
+                    f"{self.get_option('network-args', self.networkArgs)}"
+                    f"{self.get_option('no-eval', self.noEval)}"
+                    f"{self.get_option('no-home', self.noHome)}"
+                    f"{self.get_option('no-https', self.noHttps)}"
+                    f"{self.get_option('no-init', self.noInit)}"
+                    f"{self.get_option('no-mount', self.noMount)}"
+                    f"{self.get_option('no-privs', self.noPrivs)}"
+                    f"{self.get_option('no-umask', self.noUmask)}"
+                    f"{self.get_option('nv', self.nv)}"
+                    f"{self.get_option('nvccli', self.nvccli)}"
+                    f"{self.get_option('oom-kill-disable', self.oomKillDisable)}"
+                    f"{self.get_option('overlay', self.overlay)}"
+                    f"{self.get_option('pem-path', self.pemPath)}"
+                    f"{self.get_option('pid-file', self.pidFile)}"
+                    f"{self.get_option('pids-limit', self.pidsLimit)}"
+                    f"{self.get_option('rocm', self.rocm)}"
+                    f"{self.get_option('scratch', self.scratch)}"
+                    f"{self.get_option('security', self.security)}"
+                    f"{self.get_option('userns', self.userns)}"
+                    f"{self.get_option('uts', self.uts)}"
+                    f"{self.get_option('workdir', self.workdir)}"
+                    f"{self.get_option('writable', self.writable)}"
+                    f"{self.get_option('writable-tmpfs', self.writableTmpfs)}"
+                    f"{self.image} "
+                    f"{instance_name} "
+                    f"{' '.join(self.command) if self.command else ''}"
                 )
                 if logger.isEnabledFor(logging.DEBUG):
                     logger.debug(f"EXECUTING command {deploy_command}")
                 proc = await asyncio.create_subprocess_exec(
                     *shlex.split(deploy_command),
                     stdout=asyncio.subprocess.PIPE,
-                    stderr=asyncio.subprocess.PIPE,
+                    stderr=asyncio.subprocess.STDOUT,
                 )
-                stdout, stderr = await proc.communicate()
+                stdout, _ = await proc.communicate()
                 if proc.returncode == 0:
                     self.instanceNames.append(instance_name)
                 else:
-                    raise WorkflowExecutionException(stderr.decode().strip())
+                    raise WorkflowExecutionException(stdout.decode().strip())
 
     @cachedmethod(lambda self: self.locationsCache)
     async def get_available_locations(
         self,
         service: str | None = None,
         input_directory: str | None = None,
         output_directory: str | None = None,
@@ -1061,19 +1205,17 @@
         return pkg_resources.resource_filename(
             __name__, os.path.join("schemas", "singularity.json")
         )
 
     async def undeploy(self, external: bool) -> None:
         if not external and self.instanceNames:
             for instance_name in self.instanceNames:
-                undeploy_command = "".join(
-                    ["singularity ", "instance ", "stop ", instance_name]
-                )
+                undeploy_command = f"singularity instance stop {instance_name}"
                 if logger.isEnabledFor(logging.DEBUG):
                     logger.debug(f"EXECUTING command {undeploy_command}")
                 proc = await asyncio.create_subprocess_exec(
                     *shlex.split(undeploy_command),
                     stdout=asyncio.subprocess.PIPE,
-                    stderr=asyncio.subprocess.PIPE,
+                    stderr=asyncio.subprocess.STDOUT,
                 )
-                await proc.wait()
+                stdout, _ = await proc.communicate()
             self.instanceNames = []
```

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/kubernetes.py` & `streamflow-0.2.0.dev4/streamflow/deployment/connector/ssh.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,715 +1,657 @@
 from __future__ import annotations
 
 import asyncio
-import io
+import contextlib
 import logging
 import os
 import posixpath
-import shlex
 import tarfile
-import uuid
-from abc import ABC
-from pathlib import Path
-from shutil import which
-from typing import (
-    Any,
-    Awaitable,
-    Coroutine,
-    MutableMapping,
-    MutableSequence,
-    cast,
-)
+from pathlib import PurePosixPath
+from typing import Any, MutableMapping, MutableSequence
 
+import asyncssh
 import pkg_resources
-import yaml
-from cachetools import Cache, TTLCache
-from kubernetes_asyncio import client
-from kubernetes_asyncio.client import ApiClient, Configuration, V1Container
-from kubernetes_asyncio.config import (
-    ConfigException,
-    load_incluster_config,
-    load_kube_config,
-)
-from kubernetes_asyncio.stream import WsApiClient, ws_client
+from cachetools import Cache, LRUCache
 
 from streamflow.core import utils
 from streamflow.core.asyncache import cachedmethod
 from streamflow.core.data import StreamWrapperContext
 from streamflow.core.deployment import Connector, Location
 from streamflow.core.exception import WorkflowExecutionException
-from streamflow.core.scheduling import AvailableLocation
+from streamflow.core.scheduling import AvailableLocation, Hardware
 from streamflow.deployment import aiotarstream
-from streamflow.deployment.aiotarstream import BaseStreamWrapper
 from streamflow.deployment.connector.base import BaseConnector, extract_tar_stream
+from streamflow.deployment.stream import StreamReaderWrapper, StreamWriterWrapper
+from streamflow.deployment.template import CommandTemplateMap
 from streamflow.log_handler import logger
 
-SERVICE_NAMESPACE_FILENAME = "/var/run/secrets/kubernetes.io/serviceaccount/namespace"
 
-
-def _check_helm_installed():
-    if which("helm") is None:
-        raise WorkflowExecutionException(
-            "Helm must be installed on the system to use the Helm connector."
+async def _get_disk_usage(
+    ssh_client: asyncssh.SSHClientConnection, directory: str
+) -> float:
+    if directory:
+        result = await ssh_client.run(
+            f"df {directory} | tail -n 1 | awk '{{print $2}}'",
+            stderr=asyncio.subprocess.STDOUT,
         )
+        if result.returncode == 0:
+            return float(result.stdout.strip()) / 2**10
+        else:
+            raise WorkflowExecutionException(result.returncode)
+    else:
+        return float("inf")
+
+
+def _parse_hostname(hostname):
+    if ":" in hostname:
+        hostname, port = hostname.split(":")
+        port = int(port)
+    else:
+        port = 22
+    return hostname, port
+
+
+class SSHContext:
+    def __init__(
+        self,
+        streamflow_config_dir: str,
+        config: SSHConfig,
+        max_concurrent_sessions: int,
+    ):
+        self._streamflow_config_dir: str = streamflow_config_dir
+        self._config: SSHConfig = config
+        self._max_concurrent_sessions: int = max_concurrent_sessions
+        self._ssh_connection: asyncssh.SSHClientConnection | None = None
+        self._sessions: int = 0
+
+    async def __aenter__(self):
+        if self._ssh_connection is None:
+            self._ssh_connection = await self._get_connection(self._config)
+        self._sessions += 1
+        return self._ssh_connection
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        self._sessions -= 1
+
+    async def _get_connection(
+        self, config: SSHConfig
+    ) -> asyncssh.SSHClientConnection | None:
+        if config is None:
+            return None
+        (hostname, port) = _parse_hostname(config.hostname)
+        passphrase = (
+            self._get_param_from_file(config.ssh_key_passphrase_file)
+            if config.ssh_key_passphrase_file
+            else None
+        )
+        password = (
+            self._get_param_from_file(config.password_file)
+            if config.password_file
+            else None
+        )
+        return await asyncssh.connect(
+            client_keys=config.client_keys,
+            compression_algs=None,
+            encryption_algs=[
+                "aes128-gcm@openssh.com",
+                "aes256-ctr",
+                "aes192-ctr",
+                "aes128-ctr",
+            ],
+            known_hosts=() if config.check_host_key else None,
+            host=hostname,
+            passphrase=passphrase,
+            password=password,
+            port=port,
+            tunnel=await self._get_connection(config.tunnel),
+            username=config.username,
+        )
+
+    def _get_param_from_file(self, file_path: str):
+        if not os.path.isabs(file_path):
+            file_path = os.path.join(self._streamflow_config_dir, file_path)
+        with open(file_path) as f:
+            return f.read().strip()
+
+    async def close(self):
+        if self._ssh_connection is not None:
+            self._ssh_connection.close()
+
+    def full(self) -> bool:
+        return self._sessions == self._max_concurrent_sessions
+
+
+class SSHContextManager:
+    def __init__(
+        self, condition: asyncio.Condition, contexts: MutableSequence[SSHContext]
+    ):
+        self._condition: asyncio.Condition = condition
+        self._contexts: MutableSequence[SSHContext] = contexts
+        self._selected_context: SSHContext | None = None
+
+    async def __aenter__(self):
+        async with self._condition:
+            while True:
+                for context in self._contexts:
+                    if not context.full():
+                        ssh_connection = await context.__aenter__()
+                        self._selected_context = context
+                        return ssh_connection
+                await self._condition.wait()
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        async with self._condition:
+            if self._selected_context:
+                await self._selected_context.__aexit__(exc_type, exc_val, exc_tb)
+                self._condition.notify_all()
+
+
+class SSHContextFactory:
+    def __init__(
+        self,
+        streamflow_config_dir: str,
+        config: SSHConfig,
+        max_concurrent_sessions: int,
+        max_connections: int,
+    ):
+        self._condition: asyncio.Condition = asyncio.Condition()
+        self._contexts: MutableSequence[SSHContext] = [
+            SSHContext(
+                streamflow_config_dir=streamflow_config_dir,
+                config=config,
+                max_concurrent_sessions=max_concurrent_sessions,
+            )
+            for _ in range(max_connections)
+        ]
+
+    async def close(self):
+        await asyncio.gather(*(asyncio.create_task(c.close()) for c in self._contexts))
+
+    def get(self):
+        return SSHContextManager(condition=self._condition, contexts=self._contexts)
 
 
-async def _get_helm_version():
-    proc = await asyncio.create_subprocess_exec(
-        *shlex.split("helm version --template '{{.Version}}'"),
-        stdout=asyncio.subprocess.PIPE,
-        stderr=asyncio.subprocess.DEVNULL,
-    )
-    stdout, _ = await proc.communicate()
-    return stdout.decode().strip()
-
-
-class KubernetesResponseWrapper(BaseStreamWrapper):
-    async def read(self, size: int | None = None):
-        while not self.stream.closed:
-            async for msg in self.stream:
-                channel = msg.data[0]
-                data = msg.data[1:]
-                if data and channel == ws_client.STDOUT_CHANNEL:
-                    return data
-        return None
-
-    async def write(self, data: Any):
-        channel_prefix = bytes(chr(ws_client.STDIN_CHANNEL), "ascii")
-        payload = channel_prefix + data
-        await self.stream.send_bytes(payload)
-
-
-class KubernetesResponseWrapperContext(StreamWrapperContext):
-    def __init__(self, coro: Coroutine):
-        self.coro: Coroutine = coro
-        self.response: KubernetesResponseWrapper | None = None
+class SSHStreamWrapperContext(StreamWrapperContext):
+    def __init__(self, src: str, ssh_context: SSHContextManager):
+        super().__init__()
+        self.src: str = src
+        self.ssh_context: SSHContextManager = ssh_context
+        self.ssh_process: asyncssh.SSHClientProcess | None = None
+        self.stream: StreamReaderWrapper | None = None
 
     async def __aenter__(self):
-        response = await self.coro
-        self.response = KubernetesResponseWrapper(response)
-        return self.response
+        ssh_client = await self.ssh_context.__aenter__()
+        dirname, basename = posixpath.split(self.src)
+        self.ssh_process = await (
+            await ssh_client.create_process(
+                f"tar chf - -C {dirname} {basename}",
+                stdin=asyncio.subprocess.DEVNULL,
+                encoding=None,
+            )
+        ).__aenter__()
+        self.stream = StreamReaderWrapper(self.ssh_process.stdout)
+        return self.stream
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
-        if self.response:
-            await self.response.close()
+        if self.stream:
+            await self.stream.close()
+        if self.ssh_process:
+            await self.ssh_process.__aexit__(exc_type, exc_val, exc_tb)
+        await self.ssh_context.__aexit__(exc_type, exc_val, exc_tb)
+
 
+class SSHConfig:
+    def __init__(
+        self,
+        check_host_key: bool,
+        client_keys: MutableSequence[str],
+        hostname: str,
+        password_file: str | None,
+        ssh_key_passphrase_file: str | None,
+        tunnel: SSHConfig | None,
+        username: str,
+    ):
+        self.check_host_key: bool = check_host_key
+        self.client_keys: MutableSequence[str] = client_keys
+        self.hostname: str = hostname
+        self.password_file: str | None = password_file
+        self.ssh_key_passphrase_file: str | None = ssh_key_passphrase_file
+        self.tunnel: SSHConfig | None = tunnel
+        self.username: str = username
+
+
+class SSHConnector(BaseConnector):
+    @staticmethod
+    def _get_command(
+        location: Location,
+        command: MutableSequence[str],
+        environment: MutableMapping[str, str] = None,
+        workdir: str | None = None,
+        stdin: int | str | None = None,
+        stdout: int | str = asyncio.subprocess.STDOUT,
+        stderr: int | str = asyncio.subprocess.STDOUT,
+        job_name: str | None = None,
+    ):
+        command = utils.create_command(
+            command=command,
+            environment=environment,
+            workdir=workdir,
+            stdin=stdin,
+            stdout=stdout,
+            stderr=stderr,
+        )
+        if logger.isEnabledFor(logging.DEBUG):
+            logger.debug(
+                f"EXECUTING command {command} on {location}" f" for job {job_name}"
+                if job_name
+                else ""
+            )
+        return utils.encode_command(command)
 
-class BaseKubernetesConnector(BaseConnector, ABC):
     def __init__(
         self,
         deployment_name: str,
         config_dir: str,
-        inCluster: bool | None = False,
-        kubeconfig: str | None = None,
-        namespace: str | None = None,
-        locationsCacheSize: int = None,
-        locationsCacheTTL: int = None,
-        resourcesCacheSize: int = None,
-        resourcesCacheTTL: int = None,
-        transferBufferSize: int = (2**25) - 1,
-        maxConcurrentConnections: int = 4096,
-    ):
+        nodes: MutableSequence[Any],
+        username: str,
+        checkHostKey: bool = True,
+        dataTransferConnection: str | MutableMapping[str, Any] | None = None,
+        file: str | None = None,
+        maxConcurrentSessions: int = 10,
+        maxConnections: int = 1,
+        passwordFile: str | None = None,
+        services: MutableMapping[str, str] | None = None,
+        sharedPaths: MutableSequence[str] | None = None,
+        sshKey: str | None = None,
+        sshKeyPassphraseFile: str | None = None,
+        tunnel: MutableMapping[str, Any] | None = None,
+        transferBufferSize: int = 2**16,
+    ) -> None:
         super().__init__(
             deployment_name=deployment_name,
             config_dir=config_dir,
             transferBufferSize=transferBufferSize,
         )
-        self.inCluster = inCluster
-        self.kubeconfig = (
-            kubeconfig
-            if kubeconfig is not None
-            else os.path.join(str(Path.home()), ".kube", "config")
-        )
-        self.namespace = namespace
-        cacheSize = locationsCacheSize
-        if cacheSize is None:
-            cacheSize = resourcesCacheSize
-            if cacheSize is not None:
-                if logger.isEnabledFor(logging.WARN):
-                    logger.warn(
-                        "The `resourcesCacheSize` keyword is deprecated and will be removed in StreamFlow 0.3.0. "
-                        "Use `locationsCacheSize` instead."
-                    )
-            else:
-                cacheSize = 10
-        cacheTTL = locationsCacheTTL
-        if cacheTTL is None:
-            cacheTTL = resourcesCacheTTL
-            if cacheTTL is not None:
-                if logger.isEnabledFor(logging.WARN):
-                    logger.warn(
-                        "The `resourcesCacheTTL` keyword is deprecated and will be removed in StreamFlow 0.3.0. "
-                        "Use `locationsCacheTTL` instead."
-                    )
-            else:
-                cacheTTL = 10
-        self.locationsCache: Cache = TTLCache(maxsize=cacheSize, ttl=cacheTTL)
-        self.configuration: Configuration | None = None
-        self.client: client.CoreV1Api | None = None
-        self.client_ws: client.CoreV1Api | None = None
-        self.maxConcurrentConnections: int = maxConcurrentConnections
-
-    def _configure_incluster_namespace(self):
-        if self.namespace is None:
-            if not os.path.isfile(SERVICE_NAMESPACE_FILENAME):
-                raise ConfigException("Service namespace file does not exists.")
-
-            with open(SERVICE_NAMESPACE_FILENAME) as f:
-                self.namespace = f.read()
-                if not self.namespace:
-                    raise ConfigException("Namespace file exists but empty.")
-
-    async def _copy_local_to_remote(
-        self,
-        src: str,
-        dst: str,
-        locations: MutableSequence[Location],
-        read_only: bool = False,
-    ):
-        effective_locations = await self._get_effective_locations(locations, dst)
-        await super()._copy_local_to_remote(
-            src=src, dst=dst, locations=effective_locations, read_only=read_only
-        )
+        services_map: MutableMapping[str, Any] = {}
+        if services:
+            for name, service in services.items():
+                with open(os.path.join(self.config_dir, service)) as f:
+                    services_map[name] = f.read()
+        if file is not None:
+            if logger.isEnabledFor(logging.WARN):
+                logger.warn(
+                    "The `file` keyword is deprecated and will be removed in StreamFlow 0.3.0. "
+                    "Use `services` instead."
+                )
+            with open(os.path.join(self.config_dir, file)) as f:
+                self.template_map: CommandTemplateMap = CommandTemplateMap(
+                    default=f.read(), template_map=services_map
+                )
+        else:
+            self.template_map: CommandTemplateMap = CommandTemplateMap(
+                default="#!/bin/sh\n\n{{streamflow_command}}",
+                template_map=services_map,
+            )
+        self.checkHostKey: bool = checkHostKey
+        self.passwordFile: str | None = passwordFile
+        self.maxConcurrentSessions: int = maxConcurrentSessions
+        self.maxConnections: int = maxConnections
+        self.sharedPaths: MutableSequence[str] = sharedPaths or []
+        self.sshKey: str | None = sshKey
+        self.sshKeyPassphraseFile: str | None = sshKeyPassphraseFile
+        self.ssh_context_factories: MutableMapping[str, SSHContextFactory] = {}
+        self.data_transfer_context_factories: MutableMapping[
+            str, SSHContextFactory
+        ] = {}
+        self.username: str = username
+        self.tunnel: SSHConfig | None = self._get_config(tunnel)
+        self.dataTransferConfig: SSHConfig | None = self._get_config(
+            dataTransferConnection
+        )
+        self.nodes: MutableMapping[str, SSHConfig] = {
+            n.hostname: n for n in [self._get_config(n) for n in nodes]
+        }
+        self.hardwareCache: Cache = LRUCache(maxsize=len(self.nodes))
 
     async def _copy_local_to_remote_single(
         self, src: str, dst: str, location: Location, read_only: bool = False
-    ) -> None:
-        pod, container = location.name.split(":")
-        command = ["tar", "xf", "-", "-C", "/"]
-        # noinspection PyUnresolvedReferences
-        response = await self.client_ws.connect_get_namespaced_pod_exec(
-            name=pod,
-            namespace=self.namespace or "default",
-            container=container,
-            command=command,
-            stderr=False,
-            stdin=True,
-            stdout=False,
-            tty=False,
-            _preload_content=False,
-        )
-        try:
-            async with aiotarstream.open(
-                stream=KubernetesResponseWrapper(response),
-                format=tarfile.GNU_FORMAT,
-                mode="w",
-                dereference=True,
-                copybufsize=self.transferBufferSize,
-            ) as tar:
-                await tar.add(src, arcname=dst)
-        except tarfile.TarError as e:
-            raise WorkflowExecutionException(
-                f"Error copying {src} to {dst} on location {location}: {e}"
-            ) from e
-        finally:
-            await response.close()
+    ):
+        async with self._get_data_transfer_client(location.name) as ssh_client:
+            async with ssh_client.create_process(
+                "tar xf - -C /",
+                stderr=asyncio.subprocess.DEVNULL,
+                stdout=asyncio.subprocess.DEVNULL,
+                encoding=None,
+            ) as proc:
+                try:
+                    async with aiotarstream.open(
+                        stream=StreamWriterWrapper(proc.stdin),
+                        format=tarfile.GNU_FORMAT,
+                        mode="w",
+                        dereference=True,
+                        copybufsize=self.transferBufferSize,
+                    ) as tar:
+                        await tar.add(src, arcname=dst)
+                except tarfile.TarError as e:
+                    raise WorkflowExecutionException(
+                        f"Error copying {src} to {dst} on location {location}: {e}"
+                    ) from e
 
     async def _copy_remote_to_local(
         self, src: str, dst: str, location: Location, read_only: bool = False
-    ):
-        pod, container = location.name.split(":")
-        command = ["tar", "chf", "-", "-C", "/", posixpath.relpath(src, "/")]
-        # noinspection PyUnresolvedReferences
-        response = await self.client_ws.connect_get_namespaced_pod_exec(
-            name=pod,
-            namespace=self.namespace or "default",
-            container=container,
-            command=command,
-            stderr=True,
-            stdin=False,
-            stdout=True,
-            tty=False,
-            _preload_content=False,
-        )
-        try:
-            async with aiotarstream.open(
-                stream=KubernetesResponseWrapper(response),
-                mode="r",
-                copybufsize=self.transferBufferSize,
-            ) as tar:
-                await extract_tar_stream(tar, src, dst, self.transferBufferSize)
-        except tarfile.TarError as e:
-            raise WorkflowExecutionException(
-                f"Error copying {src} from location {location} to {dst}: {e}"
-            ) from e
-        finally:
-            await response.close()
+    ) -> None:
+        dirname, basename = posixpath.split(src)
+        async with self._get_data_transfer_client(location.name) as ssh_client:
+            async with ssh_client.create_process(
+                f"tar chf - -C {dirname} {basename}",
+                stdin=asyncio.subprocess.DEVNULL,
+                encoding=None,
+            ) as proc:
+                try:
+                    async with aiotarstream.open(
+                        stream=StreamReaderWrapper(proc.stdout),
+                        mode="r",
+                        copybufsize=self.transferBufferSize,
+                    ) as tar:
+                        await extract_tar_stream(tar, src, dst, self.transferBufferSize)
+                except tarfile.TarError as e:
+                    raise WorkflowExecutionException(
+                        f"Error copying {src} from location {location} to {dst}: {e}"
+                    ) from e
 
     async def _copy_remote_to_remote(
         self,
         src: str,
         dst: str,
         locations: MutableSequence[Location],
         source_location: Location,
         source_connector: Connector | None = None,
         read_only: bool = False,
     ) -> None:
         source_connector = source_connector or self
-        locations = await self._get_effective_locations(locations, dst)
-        if source_connector == self and source_location in locations:
+        if source_connector == self and source_location.name in [
+            loc.name for loc in locations
+        ]:
             if src != dst:
                 command = ["/bin/cp", "-rf", src, dst]
                 await self.run(source_location, command)
                 locations.remove(source_location)
-        if locations:
-            # Get write command
-            write_command = await utils.get_remote_to_remote_write_command(
+        write_command = " ".join(
+            await utils.get_remote_to_remote_write_command(
                 src_connector=source_connector,
                 src_location=source_location,
                 src=src,
                 dst_connector=self,
                 dst_locations=locations,
                 dst=dst,
             )
+        )
+        if locations:
             async with source_connector._get_stream_reader(
                 source_location, src
             ) as reader:
-                # Open a target response for each location
-                writers = [
-                    KubernetesResponseWrapper(w)
-                    for w in await asyncio.gather(
+                async with contextlib.AsyncExitStack() as exit_stack:
+                    # Open a target StreamWriter for each location
+                    writer_clients = await asyncio.gather(
                         *(
                             asyncio.create_task(
-                                cast(
-                                    Coroutine,
-                                    self.client_ws.connect_get_namespaced_pod_exec(
-                                        name=location.name.split(":")[0],
-                                        namespace=self.namespace or "default",
-                                        container=location.name.split(":")[1],
-                                        command=write_command,
-                                        stderr=True,
-                                        stdin=False,
-                                        stdout=True,
-                                        tty=False,
-                                        _preload_content=False,
-                                    ),
+                                exit_stack.enter_async_context(
+                                    self._get_data_transfer_client(location.name)
                                 )
                             )
                             for location in locations
                         )
                     )
-                ]
-                # Multiplex the reader output to all the writers
-                while content := await reader.read(source_connector.transferBufferSize):
-                    await asyncio.gather(
-                        *(
-                            asyncio.create_task(writer.write(content))
-                            for writer in writers
+                    async with contextlib.AsyncExitStack() as writers_stack:
+                        writers = await asyncio.gather(
+                            *(
+                                asyncio.create_task(
+                                    writers_stack.enter_async_context(
+                                        client.create_process(
+                                            write_command,
+                                            stderr=asyncio.subprocess.DEVNULL,
+                                            stdout=asyncio.subprocess.DEVNULL,
+                                            encoding=None,
+                                        )
+                                    )
+                                )
+                                for client in writer_clients
+                            )
                         )
-                    )
+                        # Multiplex the reader output to all the writers
+                        while content := await reader.read(
+                            source_connector.transferBufferSize
+                        ):
+                            for writer in writers:
+                                writer.stdin.write(content)
+                            await asyncio.gather(
+                                *(
+                                    asyncio.create_task(writer.stdin.drain())
+                                    for writer in writers
+                                )
+                            )
+
+    def _get_config(self, node: str | MutableMapping[str, Any]):
+        if node is None:
+            return None
+        elif isinstance(node, str):
+            node = {"hostname": node}
+        ssh_key = node["sshKey"] if "sshKey" in node else self.sshKey
+        return SSHConfig(
+            hostname=node["hostname"],
+            username=node["username"] if "username" in node else self.username,
+            check_host_key=node["checkHostKey"]
+            if "checkHostKey" in node
+            else self.checkHostKey,
+            client_keys=[ssh_key] if ssh_key is not None else [],
+            password_file=node["passwordFile"]
+            if "passwordFile" in node
+            else self.passwordFile,
+            ssh_key_passphrase_file=(
+                node["sshKeyPassphraseFile"]
+                if "sshKeyPassphraseFile" in node
+                else self.sshKeyPassphraseFile
+            ),
+            tunnel=(
+                self._get_config(node["tunnel"])
+                if "tunnel" in node
+                else self.tunnel
+                if hasattr(self, "tunnel")
+                else None
+            ),
+        )
+
+    def _get_data_transfer_client(self, location: str) -> SSHContextManager:
+        if self.dataTransferConfig:
+            if location not in self.data_transfer_context_factories:
+                self.data_transfer_context_factories[location] = SSHContextFactory(
+                    streamflow_config_dir=self.config_dir,
+                    config=self.dataTransferConfig,
+                    max_concurrent_sessions=self.maxConcurrentSessions,
+                    max_connections=self.maxConnections,
+                )
+            return self.data_transfer_context_factories[location].get()
+        else:
+            return self._get_ssh_client(location)
 
-    async def _get_container(self, location: Location) -> tuple[str, V1Container]:
-        pod_name, container_name = location.name.split(":")
-        pod = await self.client.read_namespaced_pod(
-            name=pod_name, namespace=self.namespace or "default"
-        )
-        for container in pod.spec.containers:
-            if container.name == container_name:
-                return container.name, container
-        raise WorkflowExecutionException(
-            f"No container with name {container_name} available on pod {pod_name}."
-        )
-
-    async def _get_configuration(self) -> Configuration:
-        if self.configuration is None:
-            self.configuration = Configuration()
-            if self.inCluster:
-                load_incluster_config(client_configuration=self.configuration)
-                self._configure_incluster_namespace()
-            else:
-                await load_kube_config(
-                    config_file=self.kubeconfig, client_configuration=self.configuration
+    async def _get_existing_parent(self, location: str, directory: str):
+        if directory is None:
+            return None
+        async with self._get_ssh_client(location) as ssh_client:
+            while True:
+                result = await ssh_client.run(
+                    f'test -e "{directory}"',
+                    stderr=asyncio.subprocess.STDOUT,
                 )
-        return self.configuration
+                if result.returncode == 0:
+                    return directory
+                elif result.returncode == 1:
+                    directory = PurePosixPath(directory).parent
+                else:
+                    raise WorkflowExecutionException(result.stdout.strip())
 
-    async def _get_effective_locations(
+    @cachedmethod(lambda self: self.hardwareCache)
+    async def _get_location_hardware(
         self,
-        locations: MutableSequence[Location],
-        dest_path: str,
-        source_location: Location | None = None,
-    ) -> MutableSequence[Location]:
-        # Get containers
-        container_tasks = []
-        for location in locations:
-            container_tasks.append(asyncio.create_task(self._get_container(location)))
-        containers = {k: v for (k, v) in await asyncio.gather(*container_tasks)}
-        # Check if some locations share volume mounts to the same path
-        common_paths = {}
-        effective_locations = []
-        for location in locations:
-            container = containers[location.name.split(":")[1]]
-            add_location = True
-            for volume in container.volume_mounts:
-                if dest_path.startswith(volume.mount_path):
-                    path = ":".join([volume.name, dest_path])
-                    if path not in common_paths:
-                        common_paths[path] = location
-                    elif location.name == source_location.name:
-                        effective_locations.remove(common_paths[path])
-                        common_paths[path] = location
-                    else:
-                        add_location = False
-                    break
-            if add_location:
-                effective_locations.append(location)
-        return effective_locations
+        location: str,
+        input_directory: str,
+        output_directory: str,
+        tmp_directory: str,
+    ) -> Hardware:
+        try:
+            async with self._get_ssh_client(location) as ssh_client:
+                (
+                    cores,
+                    memory,
+                    input_directory,
+                    output_directory,
+                    tmp_directory,
+                ) = await asyncio.gather(
+                    asyncio.create_task(
+                        ssh_client.run("nproc", stderr=asyncio.subprocess.STDOUT)
+                    ),
+                    asyncio.create_task(
+                        ssh_client.run(
+                            "free | grep Mem | awk '{print $2}'",
+                            stderr=asyncio.subprocess.STDOUT,
+                        )
+                    ),
+                    asyncio.create_task(_get_disk_usage(ssh_client, input_directory)),
+                    asyncio.create_task(_get_disk_usage(ssh_client, output_directory)),
+                    asyncio.create_task(_get_disk_usage(ssh_client, tmp_directory)),
+                )
+                if cores.returncode == 0 and memory.returncode == 0:
+                    return Hardware(
+                        cores=float(cores.stdout.strip()),
+                        memory=float(memory.stdout.strip()) / 2**10,
+                        input_directory=input_directory,
+                        output_directory=output_directory,
+                        tmp_directory=tmp_directory,
+                    )
+                else:
+                    raise WorkflowExecutionException(
+                        f"Impossible to retrieve locations for {location}"
+                    )
+        except WorkflowExecutionException:
+            raise WorkflowExecutionException(
+                f"Impossible to retrieve locations for {location}"
+            )
 
     def _get_run_command(
         self, command: str, location: Location, interactive: bool = False
     ):
-        pod, container = location.name.split(":")
-        return "".join(
-            [
-                "kubectl ",
-                self.get_option("namespace", self.namespace),
-                self.get_option("kubeconfig", self.kubeconfig),
-                "exec ",
-                f"{pod} ",
-                self.get_option("i", interactive),
-                self.get_option("container", container),
-                "-- ",
-                command,
-            ]
-        )
+        return f"ssh {location.name} {command}"
+
+    def _get_ssh_client(self, location: str) -> SSHContextManager:
+        if location not in self.ssh_context_factories:
+            self.ssh_context_factories[location] = SSHContextFactory(
+                streamflow_config_dir=self.config_dir,
+                config=self.nodes[location],
+                max_concurrent_sessions=self.maxConcurrentSessions,
+                max_connections=self.maxConnections,
+            )
+        return self.ssh_context_factories[location].get()
 
     def _get_stream_reader(self, location: Location, src: str) -> StreamWrapperContext:
-        pod, container = location.name.split(":")
-        dirname, basename = posixpath.split(src)
-        return KubernetesResponseWrapperContext(
-            coro=cast(
-                Coroutine,
-                self.client_ws.connect_get_namespaced_pod_exec(
-                    name=pod,
-                    namespace=self.namespace or "default",
-                    container=container,
-                    command=["tar", "chf", "-", "-C", dirname, basename],
-                    stderr=False,
-                    stdin=True,
-                    stdout=False,
-                    tty=False,
-                    _preload_content=False,
+        return SSHStreamWrapperContext(
+            src=src, ssh_context=self._get_data_transfer_client(location.name)
+        )
+
+    async def deploy(self, external: bool) -> None:
+        pass
+
+    async def get_available_locations(
+        self,
+        service: str | None = None,
+        input_directory: str | None = None,
+        output_directory: str | None = None,
+        tmp_directory: str | None = None,
+    ) -> MutableMapping[str, AvailableLocation]:
+        locations = {}
+        for location_obj in self.nodes.values():
+            inpdir, outdir, tmpdir = await asyncio.gather(
+                asyncio.create_task(
+                    self._get_existing_parent(location_obj.hostname, input_directory)
+                ),
+                asyncio.create_task(
+                    self._get_existing_parent(location_obj.hostname, output_directory)
+                ),
+                asyncio.create_task(
+                    self._get_existing_parent(location_obj.hostname, tmp_directory)
                 ),
             )
-        )
+            hardware = await self._get_location_hardware(
+                location=location_obj.hostname,
+                input_directory=inpdir,
+                output_directory=outdir,
+                tmp_directory=tmpdir,
+            )
+            locations[location_obj.hostname] = AvailableLocation(
+                name=location_obj.hostname,
+                deployment=self.deployment_name,
+                service=service,
+                hostname=location_obj.hostname,
+                hardware=hardware,
+            )
+        return locations
 
-    async def deploy(self, external: bool):
-        # Init standard client
-        configuration = await self._get_configuration()
-        configuration.connection_pool_maxsize = self.maxConcurrentConnections
-        self.client = client.CoreV1Api(
-            api_client=ApiClient(configuration=configuration)
-        )
-        # Init WebSocket client
-        configuration = await self._get_configuration()
-        configuration.connection_pool_maxsize = self.maxConcurrentConnections
-        ws_api_client = WsApiClient(configuration=configuration, heartbeat=30)
-        ws_api_client.set_default_header("Connection", "upgrade,keep-alive")
-        self.client_ws = client.CoreV1Api(api_client=ws_api_client)
+    @classmethod
+    def get_schema(cls) -> str:
+        return pkg_resources.resource_filename(
+            __name__, os.path.join("schemas", "ssh.json")
+        )
 
     async def run(
         self,
         location: Location,
         command: MutableSequence[str],
         environment: MutableMapping[str, str] = None,
         workdir: str | None = None,
         stdin: int | str | None = None,
         stdout: int | str = asyncio.subprocess.STDOUT,
         stderr: int | str = asyncio.subprocess.STDOUT,
         capture_output: bool = False,
         timeout: int | None = None,
         job_name: str | None = None,
     ) -> tuple[Any | None, int] | None:
-        command = utils.create_command(
-            command, environment, workdir, stdin, stdout, stderr
-        )
-        if logger.isEnabledFor(logging.DEBUG):
-            logger.debug(
-                "EXECUTING command {command} on {location} {job}".format(
-                    command=command,
-                    location=location,
-                    job=f"for job {job_name}" if job_name else "",
-                )
+        command = self._get_command(
+            location=location,
+            command=command,
+            environment=environment,
+            workdir=workdir,
+            stdin=stdin,
+            stdout=stdout,
+            stderr=stderr,
+            job_name=job_name,
+        )
+        if job_name is not None:
+            command = self.template_map.get_command(
+                command=command,
+                template=location.service,
+                environment=environment,
+                workdir=workdir,
             )
-        command = utils.encode_command(command)
-        pod, container = location.name.split(":")
-        # noinspection PyUnresolvedReferences
-        response = await asyncio.wait_for(
-            cast(
-                Awaitable,
-                self.client_ws.connect_get_namespaced_pod_exec(
-                    name=pod,
-                    namespace=self.namespace or "default",
-                    container=container,
-                    command=["sh", "-c", f"{command}"],
-                    stderr=True,
-                    stdin=False,
-                    stdout=True,
-                    tty=False,
-                    _preload_content=not capture_output,
-                ),
-            ),
-            timeout=timeout,
-        )
-        if capture_output:
-            with io.StringIO() as out_buffer, io.StringIO() as err_buffer:
-                while not response.closed:
-                    async for msg in response:
-                        data = msg.data.decode("utf-8", "replace")
-                        channel = ord(data[0])
-                        data = data[1:]
-                        if data and channel in [
-                            ws_client.STDOUT_CHANNEL,
-                            ws_client.STDERR_CHANNEL,
-                        ]:
-                            out_buffer.write(data)
-                        elif data and channel == ws_client.ERROR_CHANNEL:
-                            err_buffer.write(data)
-                await response.close()
-                err = yaml.safe_load(err_buffer.getvalue())
-                if err["status"] == "Success":
-                    return out_buffer.getvalue(), 0
-                else:
-                    if "code" in err:
-                        return err["message"], int(err["code"])
-                    else:
-                        return err["message"], int(
-                            err["details"]["causes"][0]["message"]
-                        )
+            command = utils.encode_command(command)
+            async with self._get_ssh_client(location.name) as ssh_client:
+                result = await asyncio.wait_for(
+                    ssh_client.run(command, stderr=asyncio.subprocess.STDOUT),
+                    timeout=timeout,
+                )
         else:
-            return None
-
-    async def undeploy(self, external: bool):
-        if self.client is not None:
-            await self.client.api_client.close()
-            self.client = None
-        if self.client_ws is not None:
-            await self.client_ws.api_client.close()
-            self.client_ws = None
-        self.configuration = None
-
-
-class Helm3Connector(BaseKubernetesConnector):
-    def __init__(
-        self,
-        deployment_name: str,
-        config_dir: str,
-        chart: str,
-        debug: bool | None = False,
-        kubeContext: str | None = None,
-        kubeconfig: str | None = None,
-        atomic: bool | None = False,
-        caFile: str | None = None,
-        certFile: str | None = None,
-        depUp: bool | None = False,
-        devel: bool | None = False,
-        inCluster: bool | None = False,
-        keepHistory: bool | None = False,
-        keyFile: str | None = None,
-        keyring: str | None = None,
-        locationsCacheSize: int = None,
-        locationsCacheTTL: int = None,
-        nameTemplate: str | None = None,
-        namespace: str | None = None,
-        noHooks: bool | None = False,
-        password: str | None = None,
-        renderSubchartNotes: bool | None = False,
-        repo: str | None = None,
-        commandLineValues: MutableSequence[str] | None = None,
-        fileValues: MutableSequence[str] | None = None,
-        stringValues: MutableSequence[str] | None = None,
-        registryConfig: str | None = None,
-        releaseName: str | None = None,
-        repositoryCache: str | None = None,
-        repositoryConfig: str | None = None,
-        resourcesCacheSize: int = None,
-        resourcesCacheTTL: int = None,
-        skipCrds: bool | None = False,
-        timeout: str | None = "1000m",
-        transferBufferSize: int = (32 << 20) - 1,
-        username: str | None = None,
-        yamlValues: MutableSequence[str] | None = None,
-        verify: bool | None = False,
-        chartVersion: str | None = None,
-        wait: bool | None = True,
-    ):
-        super().__init__(
-            deployment_name=deployment_name,
-            config_dir=config_dir,
-            inCluster=inCluster,
-            kubeconfig=kubeconfig,
-            namespace=namespace,
-            locationsCacheSize=locationsCacheSize,
-            locationsCacheTTL=locationsCacheTTL,
-            resourcesCacheSize=resourcesCacheSize,
-            resourcesCacheTTL=resourcesCacheTTL,
-            transferBufferSize=transferBufferSize,
-        )
-        self.chart: str = os.path.join(self.config_dir, chart)
-        self.debug: bool = debug
-        self.kubeContext: str | None = kubeContext
-        self.atomic: bool = atomic
-        self.caFile: str | None = caFile
-        self.certFile: str | None = certFile
-        self.depUp: bool = depUp
-        self.devel: bool = devel
-        self.keepHistory: bool = keepHistory
-        self.keyFile: str | None = keyFile
-        self.keyring: str | None = keyring
-        self.nameTemplate: str | None = nameTemplate
-        self.noHooks: bool = noHooks
-        self.password: str | None = password
-        self.renderSubchartNotes: bool = renderSubchartNotes
-        self.repo: str | None = repo
-        self.commandLineValues: MutableSequence[str] | None = commandLineValues
-        self.fileValues: MutableSequence[str] | None = fileValues
-        self.stringValues: MutableSequence[str] | None = stringValues
-        self.skipCrds: bool = skipCrds
-        self.registryConfig = (
-            registryConfig
-            if registryConfig is not None
-            else os.path.join(str(Path.home()), ".config/helm/registry.json")
-        )
-        self.releaseName: str = (
-            releaseName if releaseName is not None else f"release-{uuid.uuid1()}"
-        )
-        self.repositoryCache = (
-            repositoryCache
-            if repositoryCache is not None
-            else os.path.join(str(Path.home()), ".cache/helm/repository")
-        )
-        self.repositoryConfig = (
-            repositoryConfig
-            if repositoryConfig is not None
-            else os.path.join(str(Path.home()), ".config/helm/repositories.yaml")
-        )
-        self.timeout: str | None = timeout
-        self.username: str | None = username
-        self.yamlValues: MutableSequence[str] | None = yamlValues
-        self.verify: bool = verify
-        self.chartVersion: str | None = chartVersion
-        self.wait: bool = wait
-
-    def base_command(self) -> str:
-        return "".join(
-            [
-                "helm ",
-                self.get_option("debug", self.debug),
-                self.get_option("kube-context", self.kubeContext),
-                self.get_option("kubeconfig", self.kubeconfig),
-                self.get_option("namespace", self.namespace),
-                self.get_option("registry-config", self.registryConfig),
-                self.get_option("repository-cache", self.repositoryCache),
-                self.get_option("repository-config", self.repositoryConfig),
-            ]
-        )
-
-    async def deploy(self, external: bool) -> None:
-        # Create clients
-        await super().deploy(external)
-        if not external:
-            # Check if Helm is installed
-            _check_helm_installed()
-            # Check correct version of Helm
-            version = await _get_helm_version()
-            if not version.startswith("v3"):
-                raise WorkflowExecutionException(
-                    f"Helm {version} is not compatible with Helm3Connector"
+            async with self._get_ssh_client(location.name) as ssh_client:
+                result = await asyncio.wait_for(
+                    ssh_client.run(
+                        command,
+                        stderr=asyncio.subprocess.STDOUT,
+                    ),
+                    timeout=timeout,
                 )
-            # Deploy Helm charts
-            deploy_command = self.base_command() + "".join(
-                [
-                    "install ",
-                    self.get_option("atomic", self.atomic),
-                    self.get_option("ca-file", self.caFile),
-                    self.get_option("cert-file", self.certFile),
-                    self.get_option("dep-up", self.depUp),
-                    self.get_option("devel", self.devel),
-                    self.get_option("key-file", self.keyFile),
-                    self.get_option("keyring", self.keyring),
-                    self.get_option("name-template", self.nameTemplate),
-                    self.get_option("no-hooks", self.noHooks),
-                    self.get_option("password", self.password),
-                    self.get_option("render-subchart-notes", self.renderSubchartNotes),
-                    self.get_option("repo", self.repo),
-                    self.get_option("set", self.commandLineValues),
-                    self.get_option("set-file", self.fileValues),
-                    self.get_option("set-string", self.stringValues),
-                    self.get_option("skip-crds", self.skipCrds),
-                    self.get_option("timeout", self.timeout),
-                    self.get_option("username", self.username),
-                    self.get_option("values", self.yamlValues),
-                    self.get_option("verify", self.verify),
-                    self.get_option("version", self.chartVersion),
-                    self.get_option("wait", self.wait),
-                    f"{self.releaseName} ",
-                    self.chart,
-                ]
-            )
-            if logger.isEnabledFor(logging.DEBUG):
-                logger.debug(f"EXECUTING {deploy_command}")
-            proc = await asyncio.create_subprocess_exec(
-                *shlex.split(deploy_command),
-                stderr=asyncio.subprocess.DEVNULL,
-                stdout=asyncio.subprocess.DEVNULL,
-            )
-            await proc.wait()
-
-    @cachedmethod(lambda self: self.locationsCache)
-    async def get_available_locations(
-        self,
-        service: str | None = None,
-        input_directory: str | None = None,
-        output_directory: str | None = None,
-        tmp_directory: str | None = None,
-    ) -> MutableMapping[str, AvailableLocation]:
-        pods = await self.client.list_namespaced_pod(
-            namespace=self.namespace or "default",
-            label_selector=f"app.kubernetes.io/instance={self.releaseName}",
-            field_selector="status.phase=Running",
-        )
-        valid_targets = {}
-        for pod in pods.items:
-            # Check if pod is ready
-            is_ready = True
-            for condition in pod.status.conditions:
-                if condition.status != "True":
-                    is_ready = False
-                    break
-            # Filter out not ready and Terminating locations
-            if is_ready and pod.metadata.deletion_timestamp is None:
-                for container in pod.spec.containers:
-                    if not service or service == container.name:
-                        location_name = pod.metadata.name + ":" + service
-                        valid_targets[location_name] = AvailableLocation(
-                            name=location_name,
-                            deployment=self.deployment_name,
-                            service=service,
-                            hostname=pod.status.pod_ip,
-                        )
-                        break
-        return valid_targets
-
-    @classmethod
-    def get_schema(cls) -> str:
-        return pkg_resources.resource_filename(
-            __name__, os.path.join("schemas", "helm3.json")
-        )
+        return result.stdout.strip(), result.returncode if capture_output else None
 
     async def undeploy(self, external: bool) -> None:
-        if not external:
-            # Undeploy
-            undeploy_command = self.base_command() + "".join(
-                [
-                    "uninstall ",
-                    self.get_option("keep-history", self.keepHistory),
-                    self.get_option("no-hooks", self.noHooks),
-                    self.get_option("timeout", self.timeout),
-                    self.releaseName,
-                ]
-            )
-            if logger.isEnabledFor(logging.DEBUG):
-                logger.debug(f"EXECUTING {undeploy_command}")
-            proc = await asyncio.create_subprocess_exec(*shlex.split(undeploy_command))
-            await proc.wait()
-        # Close connections
-        await super().undeploy(external)
+        for ssh_context in self.ssh_context_factories.values():
+            await ssh_context.close()
+        self.ssh_context_factories = {}
+        for ssh_context in self.data_transfer_context_factories.values():
+            await ssh_context.close()
+        self.data_transfer_context_factories = {}
```

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/local.py` & `streamflow-0.2.0.dev4/streamflow/deployment/connector/local.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/occam.py` & `streamflow-0.2.0.dev4/streamflow/deployment/connector/occam.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/queue_manager.py` & `streamflow-0.2.0.dev4/streamflow/deployment/connector/queue_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -498,7 +498,128 @@
             logger.debug(f"Running command {command}")
         stdout, _ = await self.connector.run(
             location=location,
             command=command,
             capture_output=True,
         )
         return stdout.strip()
+
+
+class FluxConnector(QueueManagerConnector):
+    async def _get_output(self, job_id: str, location: Location) -> str:
+        # This will hang if the job is not complete
+        command = [
+            "flux",
+            "job",
+            "attach",
+            job_id,
+        ]
+        if logger.isEnabledFor(logging.DEBUG):
+            logger.debug(f"Running command {' '.join(command)}")
+        stdout, _ = await self.connector.run(
+            location=location,
+            command=command,
+            capture_output=True,
+        )
+        if output_path := stdout.strip():
+            stdout, _ = await self.connector.run(
+                location=location, command=["cat", output_path], capture_output=True
+            )
+            return stdout.strip()
+        else:
+            return ""
+
+    async def _get_returncode(self, job_id: str, location: Location) -> int:
+        command = [
+            "flux",
+            "jobs",
+            "--no-header",
+            "-o",
+            "{returncode}",
+            job_id,
+        ]
+        if logger.isEnabledFor(logging.DEBUG):
+            logger.debug(f"Running command {' '.join(command)}")
+        stdout, _ = await self.connector.run(
+            location=location,
+            command=command,
+            capture_output=True,
+        )
+        return int(stdout.strip())
+
+    @cachedmethod(
+        lambda self: self.jobsCache,
+        key=partial(cachetools.keys.hashkey, "running_jobs"),
+    )
+    async def _get_running_jobs(self, location: Location) -> MutableSequence[str]:
+        # If we add the job id, the filter is ignored
+        command = [
+            "flux",
+            "jobs",
+            "--no-header",
+            "--filter=pending,running",
+            '-o "{id}"',
+        ]
+        if logger.isEnabledFor(logging.DEBUG):
+            logger.debug(f"Running command {' '.join(command)}")
+        stdout, _ = await self.connector.run(
+            location=location,
+            command=command,
+            capture_output=True,
+        )
+        # Filter down to the job ids we are interested in
+        return [
+            j.strip()
+            for j in stdout.strip().splitlines()
+            if j.strip() in self.scheduledJobs
+        ]
+
+    async def _remove_jobs(self, location: Location) -> None:
+        await self.connector.run(
+            location=location,
+            command=["flux", "job", "cancel", " ".join(self.scheduledJobs)],
+        )
+
+    async def _run_batch_command(
+        self,
+        command: str,
+        job_name: str,
+        location: Location,
+        workdir: str | None = None,
+        stdin: int | str | None = None,
+        stdout: int | str = asyncio.subprocess.STDOUT,
+        stderr: int | str = asyncio.subprocess.STDOUT,
+        timeout: int | None = None,
+    ) -> str:
+        batch_command = [
+            "echo",
+            base64.b64encode(command.encode("utf-8")).decode("utf-8"),
+            "|",
+            "base64",
+            "-d",
+            "|",
+            "flux",
+            "batch",
+            "-N",
+            "1",
+        ]
+        if workdir is not None:
+            batch_command.extend(["--cwd", workdir])
+        if stdin is not None:
+            batch_command.extend(["--input", shlex.quote(stdin)])
+        if stdout != asyncio.subprocess.STDOUT:
+            batch_command.extend(["--output", shlex.quote(stdout)])
+        if stderr != asyncio.subprocess.STDOUT and stderr != stdout:
+            batch_command.extend(["--error", shlex.quote(stderr)])
+        if timeout:
+            batch_command.extend(["-t", utils.format_seconds_to_hhmmss(timeout)])
+        if logger.isEnabledFor(logging.DEBUG):
+            logger.debug(f"Running command {' '.join(batch_command)}")
+        stdout, returncode = await self.connector.run(
+            location=location, command=batch_command, capture_output=True
+        )
+        if returncode == 0:
+            return stdout.strip()
+        else:
+            raise WorkflowExecutionException(
+                f"Error submitting job {job_name} to Flux: {stdout.strip()}"
+            )
```

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/docker-compose.json` & `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/docker-compose.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/docker.json` & `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/docker.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/helm3.json` & `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/helm3.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/occam.json` & `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/occam.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/queue_manager.json` & `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/queue_manager.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/singularity.json` & `streamflow-0.2.0.dev4/streamflow/cwl/requirement/docker/schemas/singularity.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.803872053872054%*

 * *Differences: {"'properties'": "{'cleanenv': {'default': True}, 'contain': {'default': True}, 'blkioWeight': "*

 * *                 "OrderedDict([('type', 'integer'), ('description', 'Block IO relative weight in "*

 * *                 "range 10-1000, 0 to disable')]), 'blkioWeightDevice': OrderedDict([('type', "*

 * *                 "'array'), ('items', OrderedDict([('type', 'string')])), ('description', 'Device "*

 * *                 "specific block IO relative weight')]), 'compat': OrderedDict([('type', "*

 * *                 "'boolean'), […]*

```diff
@@ -19,45 +19,82 @@
             "description": "A user-bind path specification, in the format src[:dest[:opts]]",
             "items": {
                 "type": "string"
             },
             "type": "array",
             "uniqueItems": true
         },
+        "blkioWeight": {
+            "description": "Block IO relative weight in range 10-1000, 0 to disable",
+            "type": "integer"
+        },
+        "blkioWeightDevice": {
+            "description": "Device specific block IO relative weight",
+            "items": {
+                "type": "string"
+            },
+            "type": "array"
+        },
         "boot": {
             "description": "Execute /sbin/init to boot container (root only)",
             "type": "boolean"
         },
         "cleanenv": {
+            "default": true,
             "description": "Clean environment before running container",
             "type": "boolean"
         },
         "command": {
             "description": "Command to run when deploying the container",
             "items": {
                 "type": "string"
             },
             "type": "array"
         },
+        "compat": {
+            "description": "Apply settings for increased OCI/Docker compatibility. Infers --containall, --no-init, --no-umask, --no-eval, --writable-tmpfs.",
+            "type": "boolean"
+        },
         "contain": {
+            "default": true,
             "description": "Use minimal /dev and empty other directories (e.g. /tmp and $HOME) instead of sharing filesystems from your host",
             "type": "boolean"
         },
         "containall": {
             "description": "Contain not only file systems, but also PID, IPC, and environment",
             "type": "boolean"
         },
+        "cpuShares": {
+            "description": "CPU shares for container (default -1)",
+            "type": "integer"
+        },
+        "cpus": {
+            "description": "Number of CPUs available to container",
+            "type": "string"
+        },
+        "cpusetCpus": {
+            "description": "List of host CPUs available to container",
+            "type": "string"
+        },
+        "cpusetMems": {
+            "description": "List of host memory nodes available to container",
+            "type": "string"
+        },
         "disableCache": {
             "description": "Don't use cache and don't create cache",
             "type": "boolean"
         },
         "dns": {
             "description": "List of DNS server separated by commas to add in resolv.conf",
             "type": "string"
         },
+        "dockerHost": {
+            "description": "Specify a custom Docker daemon host",
+            "type": "string"
+        },
         "dropCaps": {
             "description": "A comma separated capability list to drop",
             "type": "string"
         },
         "env": {
             "description": "Pass environment variable to contained process",
             "items": {
@@ -87,25 +124,17 @@
             "description": "A home directory specification, in the format src[:dest]",
             "type": "string"
         },
         "hostname": {
             "description": "Set container hostname",
             "type": "string"
         },
-        "image": {
-            "description": "The name of the Singularity image to run",
-            "type": "string"
-        },
-        "instanceNames": {
-            "description": "When referencing an external environment, names of existing instances must be explicitly listed",
-            "items": {
-                "type": "string"
-            },
-            "type": "array",
-            "uniqueItems": true
+        "ipc": {
+            "description": "Run container in a new IPC namespace",
+            "type": "boolean"
         },
         "keepPrivs": {
             "description": "Let root user keep privileges in container (root only)",
             "type": "boolean"
         },
         "locationsCacheSize": {
             "default": 10,
@@ -113,14 +142,33 @@
             "type": "integer"
         },
         "locationsCacheTTL": {
             "default": 10,
             "description": "Available locations cache TTL (in seconds). When such cache expires, the connector performs a new request to check locations availability",
             "type": "integer"
         },
+        "memory": {
+            "description": "Memory limit in bytes",
+            "type": "string"
+        },
+        "memoryReservation": {
+            "description": "Memory soft limit in bytes",
+            "type": "string"
+        },
+        "memorySwap": {
+            "description": "Swap limit, use -1 for unlimited swap",
+            "type": "string"
+        },
+        "mount": {
+            "description": "A mount specification (e.g., type=bind,source=/opt,destination=/hostopt)",
+            "items": {
+                "type": "string"
+            },
+            "type": "array"
+        },
         "net": {
             "description": "Run container in a new network namespace (sets up a bridge network interface by default)",
             "type": "boolean"
         },
         "network": {
             "default": "bridge",
             "description": "Specify desired network type separated by commas, each network will bring up a dedicated interface inside container",
@@ -130,18 +178,26 @@
             "description": "Specify network arguments to pass to CNI plugins",
             "items": {
                 "type": "string"
             },
             "type": "array",
             "uniqueItems": true
         },
+        "noEval": {
+            "description": "Do not shell evaluate env vars or OCI container CMD/ENTRYPOINT/ARGS",
+            "type": "boolean"
+        },
         "noHome": {
             "description": "Do not mount users home directory if /home is not the current working directory",
             "type": "boolean"
         },
+        "noHttps": {
+            "description": "Use HTTP instead of HTTPS for docker:// oras:// and library://<hostname>/... URIs",
+            "type": "boolean"
+        },
         "noInit": {
             "description": "Do not start shim processes with --pid",
             "type": "boolean"
         },
         "noMount": {
             "description": "Disable one or more mount xxx options set in singularity.conf",
             "items": {
@@ -154,22 +210,26 @@
             "description": "Drop all privileges from root user in container",
             "type": "boolean"
         },
         "noUmask": {
             "description": "Do not propagate umask to the container. Set default 0022 umask",
             "type": "boolean"
         },
-        "nohttps": {
-            "description": "Do not use HTTPS with the docker:// transport",
-            "type": "boolean"
-        },
         "nv": {
             "description": "Enable experimental NVIDIA support",
             "type": "boolean"
         },
+        "nvccli": {
+            "description": "Use nvidia-container-cli for GPU setup",
+            "type": "boolean"
+        },
+        "oomKillDisable": {
+            "description": "Disable OOM killer",
+            "type": "boolean"
+        },
         "overlay": {
             "description": "Use an overlayFS image for persistent data storage or as read-only layer of container",
             "items": {
                 "type": "string"
             },
             "type": "array",
             "uniqueItems": true
@@ -178,29 +238,23 @@
             "description": "Enter a path to a PEM formatted RSA key for an encrypted container",
             "type": "string"
         },
         "pidFile": {
             "description": "Write instance PID to the file with the given name",
             "type": "string"
         },
+        "pidsLimit": {
+            "description": "Limit number of container PIDs, use -1 for unlimited",
+            "type": "integer"
+        },
         "replicas": {
             "default": 1,
             "description": "Number of instances to be co-allocated",
             "type": "integer"
         },
-        "resourcesCacheSize": {
-            "default": 10,
-            "description": "(**Deprecated.** Use locationsCacheSize.) Available resources cache size",
-            "type": "integer"
-        },
-        "resourcesCacheTTL": {
-            "default": 10,
-            "description": "(**Deprecated.** Use locationsCacheTTL.) Available resources cache TTL (in seconds). When such cache expires, the connector performs a new request to check resources availability",
-            "type": "integer"
-        },
         "rocm": {
             "description": "Enable experimental ROCM support",
             "type": "boolean"
         },
         "scratch": {
             "description": "Include a scratch directory within the container that is linked to a temporary dir",
             "items": {
@@ -239,12 +293,9 @@
             "type": "boolean"
         },
         "writableTmpfs": {
             "description": "Makes the file system accessible as read/write with non persistent data (with overlay support only)",
             "type": "boolean"
         }
     },
-    "required": [
-        "image"
-    ],
     "type": "object"
 }
```

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/connector/schemas/ssh.json` & `streamflow-0.2.0.dev4/streamflow/deployment/connector/schemas/ssh.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/deployment_manager.py` & `streamflow-0.2.0.dev4/streamflow/deployment/deployment_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/filter/shuffle.py` & `streamflow-0.2.0.dev4/streamflow/deployment/filter/shuffle.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/future.py` & `streamflow-0.2.0.dev4/streamflow/deployment/future.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/stream.py` & `streamflow-0.2.0.dev4/streamflow/deployment/stream.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/template.py` & `streamflow-0.2.0.dev4/streamflow/deployment/template.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/utils.py` & `streamflow-0.2.0.dev4/streamflow/deployment/utils.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/deployment/wrapper.py` & `streamflow-0.2.0.dev4/streamflow/deployment/wrapper.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/ext/plugin.py` & `streamflow-0.2.0.dev4/streamflow/ext/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from typing import MutableMapping
 
 from streamflow.core.data import DataManager
 from streamflow.core.deployment import BindingFilter, Connector, DeploymentManager
 from streamflow.core.persistence import Database
 from streamflow.core.recovery import CheckpointManager, FailureManager
 from streamflow.core.scheduling import Policy, Scheduler
+from streamflow.cwl.requirement.docker import cwl_docker_translator_classes
+from streamflow.cwl.requirement.docker.translator import CWLDockerTranslator
 from streamflow.data import data_manager_classes
 from streamflow.deployment import deployment_manager_classes
 from streamflow.deployment.connector import connector_classes
 from streamflow.deployment.filter import binding_filter_classes
 from streamflow.log_handler import logger
 from streamflow.persistence import database_classes
 from streamflow.recovery import checkpoint_manager_classes, failure_manager_classes
@@ -37,14 +39,17 @@
 
     def register_binding_filter(self, name: str, cls: type[BindingFilter]):
         self._register(name, cls, binding_filter_classes)
 
     def register_checkpoint_manager(self, name: str, cls: type[CheckpointManager]):
         self._register(name, cls, checkpoint_manager_classes)
 
+    def register_cwl_docker_translator(self, name: str, cls: type[CWLDockerTranslator]):
+        self._register(name, cls, cwl_docker_translator_classes)
+
     def register_connector(self, name: str, cls: type[Connector]):
         self._register(name, cls, connector_classes)
 
     def register_data_manager(self, name: str, cls: type[DataManager]):
         self._register(name, cls, data_manager_classes)
 
     def register_database(self, name: str, cls: type[Database]):
```

### Comparing `streamflow-0.2.0.dev3/streamflow/ext/utils.py` & `streamflow-0.2.0.dev4/streamflow/ext/utils.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/log_handler.py` & `streamflow-0.2.0.dev4/streamflow/log_handler.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/main.py` & `streamflow-0.2.0.dev4/streamflow/main.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/parser.py` & `streamflow-0.2.0.dev4/streamflow/parser.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/persistence/loading_context.py` & `streamflow-0.2.0.dev4/streamflow/persistence/loading_context.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/persistence/schemas/sqlite.json` & `streamflow-0.2.0.dev4/streamflow/persistence/schemas/sqlite.json`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/persistence/schemas/sqlite.sql` & `streamflow-0.2.0.dev4/streamflow/persistence/schemas/sqlite.sql`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/persistence/sqlite.py` & `streamflow-0.2.0.dev4/streamflow/persistence/sqlite.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/provenance/run_crate.py` & `streamflow-0.2.0.dev4/streamflow/provenance/run_crate.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/recovery/checkpoint_manager.py` & `streamflow-0.2.0.dev4/streamflow/recovery/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/recovery/failure_manager.py` & `streamflow-0.2.0.dev4/streamflow/recovery/failure_manager.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/recovery/recovery.py` & `streamflow-0.2.0.dev4/streamflow/recovery/recovery.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/report.py` & `streamflow-0.2.0.dev4/streamflow/report.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/scheduling/policy/data_locality.py` & `streamflow-0.2.0.dev4/streamflow/scheduling/policy/data_locality.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/scheduling/scheduler.py` & `streamflow-0.2.0.dev4/streamflow/scheduling/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                             else f"on location {selected_locations[0]}"
                         ),
                     )
                 )
             else:
                 logger.debug(
                     f"Job {job.name} allocated on locations "
-                    ", ".join([str(loc) for loc in selected_locations])
+                    f"{', '.join([str(loc) for loc in selected_locations])}"
                 )
         self.job_allocations[job.name] = JobAllocation(
             job=job.name,
             target=target,
             locations=selected_locations,
             status=Status.FIREABLE,
             hardware=hardware or Hardware(),
```

### Comparing `streamflow-0.2.0.dev3/streamflow/workflow/combinator.py` & `streamflow-0.2.0.dev4/streamflow/workflow/combinator.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/workflow/executor.py` & `streamflow-0.2.0.dev4/streamflow/workflow/executor.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/workflow/port.py` & `streamflow-0.2.0.dev4/streamflow/workflow/port.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/workflow/step.py` & `streamflow-0.2.0.dev4/streamflow/workflow/step.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/workflow/token.py` & `streamflow-0.2.0.dev4/streamflow/workflow/token.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/workflow/transformer.py` & `streamflow-0.2.0.dev4/streamflow/workflow/transformer.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow/workflow/utils.py` & `streamflow-0.2.0.dev4/streamflow/workflow/utils.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/streamflow.egg-info/PKG-INFO` & `streamflow-0.2.0.dev4/streamflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow
-Version: 0.2.0.dev3
+Version: 0.2.0.dev4
 Summary: StreamFlow framework
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://streamflow.di.unito.it
 Project-URL: Package, https://pypi.org/project/streamflow
 Project-URL: Repository, https://github.com/alpha-unito/streamflow
 Project-URL: Docker, https://hub.docker.com/r/alphaunito/streamflow
```

### Comparing `streamflow-0.2.0.dev3/streamflow.egg-info/SOURCES.txt` & `streamflow-0.2.0.dev4/streamflow.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,24 @@
 streamflow/cwl/transformer.py
 streamflow/cwl/translator.py
 streamflow/cwl/utils.py
 streamflow/cwl/antlr/ECMAScriptLexer.py
 streamflow/cwl/antlr/ECMAScriptListener.py
 streamflow/cwl/antlr/ECMAScriptParser.py
 streamflow/cwl/antlr/__init__.py
+streamflow/cwl/requirement/__init__.py
+streamflow/cwl/requirement/docker/__init__.py
+streamflow/cwl/requirement/docker/docker.py
+streamflow/cwl/requirement/docker/kubernetes.py
+streamflow/cwl/requirement/docker/singularity.py
+streamflow/cwl/requirement/docker/translator.py
+streamflow/cwl/requirement/docker/schemas/docker.json
+streamflow/cwl/requirement/docker/schemas/kubernetes.jinja2
+streamflow/cwl/requirement/docker/schemas/kubernetes.json
+streamflow/cwl/requirement/docker/schemas/singularity.json
 streamflow/data/__init__.py
 streamflow/data/data_manager.py
 streamflow/data/remotepath.py
 streamflow/data/schemas/data_manager.json
 streamflow/deployment/__init__.py
 streamflow/deployment/aiotarstream.py
 streamflow/deployment/deployment_manager.py
@@ -75,14 +85,15 @@
 streamflow/deployment/connector/local.py
 streamflow/deployment/connector/occam.py
 streamflow/deployment/connector/queue_manager.py
 streamflow/deployment/connector/ssh.py
 streamflow/deployment/connector/schemas/docker-compose.json
 streamflow/deployment/connector/schemas/docker.json
 streamflow/deployment/connector/schemas/helm3.json
+streamflow/deployment/connector/schemas/kubernetes.json
 streamflow/deployment/connector/schemas/local.json
 streamflow/deployment/connector/schemas/occam.json
 streamflow/deployment/connector/schemas/queue_manager.json
 streamflow/deployment/connector/schemas/singularity.json
 streamflow/deployment/connector/schemas/ssh.json
 streamflow/deployment/filter/__init__.py
 streamflow/deployment/filter/shuffle.py
```

### Comparing `streamflow-0.2.0.dev3/streamflow.egg-info/requires.txt` & `streamflow-0.2.0.dev4/streamflow.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 aiohttp==3.8.4
 aiosqlite==0.18.0
 antlr4-python3-runtime==4.12.0
 asyncssh==2.13.1
 bcrypt==4.0.1
 cachetools==5.3.0
-cwltool==3.1.20230302145532
+cwltool==3.1.20230325110543
 cwl-utils==0.23
-importlib_metadata==6.0.0
+importlib_metadata==6.3.0
 Jinja2==3.1.2
 jsonref==1.1.0
 jsonschema==4.17.3
 kubernetes_asyncio==24.2.2
 psutil==5.9.4
-rdflib==6.2.0
+rdflib==6.3.2
 yattag==1.15.1
 
 [bandit]
 bandit==1.7.5
 
 [docs]
 sphinx==6.1.3
 sphinx-jsonschema==1.19.1
 sphinx-rtd-theme==1.2.0
 
 [lint]
-black==23.1.0
+black==23.3.0
 codespell==2.2.4
-flake8-bugbear==23.2.13
+flake8-bugbear==23.3.23
 pyupgrade==3.3.1
 
 [report]
-pandas==1.5.2
-plotly==5.11.0
+pandas==2.0.0
+plotly==5.14.1
 kaleido==0.2.1.post1
 
 [test]
 cwltest==2.3.20230108193615
-pytest==7.2.2
-pytest-asyncio==0.20.3
+pytest==7.3.0
+pytest-asyncio==0.21.0
 pytest-cov==4.0.0
-pytest-xdist==3.2.0
+pytest-xdist==3.2.1
```

### Comparing `streamflow-0.2.0.dev3/tests/test_cwl_loop.py` & `streamflow-0.2.0.dev4/tests/test_cwl_loop.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/tests/test_cwl_persistence.py` & `streamflow-0.2.0.dev4/tests/test_cwl_persistence.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/tests/test_persistence.py` & `streamflow-0.2.0.dev4/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `streamflow-0.2.0.dev3/tests/test_remotepath.py` & `streamflow-0.2.0.dev4/tests/test_remotepath.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import pytest_asyncio
 
 from streamflow.core import utils
 from streamflow.core.data import FileType
 from streamflow.core.deployment import Connector, Location
 from streamflow.data import remotepath
 from streamflow.deployment.utils import get_path_processor
-from tests.conftest import get_location
+from tests.conftest import deployment_types, get_location
 
 
-@pytest_asyncio.fixture(scope="module", params=["local", "docker"])
+@pytest_asyncio.fixture(scope="module", params=deployment_types())
 async def location(context, request) -> Location:
     return await get_location(context, request)
 
 
 @pytest.fixture(scope="module")
 def connector(context, location) -> Connector:
     return context.deployment_manager.get_connector(location.deployment)
```

### Comparing `streamflow-0.2.0.dev3/tests/test_scheduler.py` & `streamflow-0.2.0.dev4/tests/test_scheduler.py`

 * *Files identical despite different names*

